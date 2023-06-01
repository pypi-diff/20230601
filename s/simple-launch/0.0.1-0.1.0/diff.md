# Comparing `tmp/simple_launch-0.0.1-py3-none-any.whl.zip` & `tmp/simple_launch-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13302 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat    27017 b- defN 23-May-31 07:40 simple_launch.py
--rw-rw-rw-  2.0 fat    11554 b- defN 23-May-31 08:20 simple_launch-0.0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3422 b- defN 23-May-31 08:20 simple_launch-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 08:20 simple_launch-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       53 b- defN 23-May-31 08:20 simple_launch-0.0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-31 08:20 simple_launch-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      596 b- defN 23-May-31 08:20 simple_launch-0.0.1.dist-info/RECORD
-7 files, 42748 bytes uncompressed, 12238 bytes compressed:  71.4%
+Zip file size: 13905 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat    27930 b- defN 23-May-31 22:37 simple_launch.py
+-rw-rw-rw-  2.0 fat    11554 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4367 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      596 b- defN 23-Jun-01 00:56 simple_launch-0.1.0.dist-info/RECORD
+7 files, 44606 bytes uncompressed, 12841 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: simple_launch.py
 Comment: 
 
-Filename: simple_launch-0.0.1.dist-info/LICENSE.txt
+Filename: simple_launch-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: simple_launch-0.0.1.dist-info/METADATA
+Filename: simple_launch-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: simple_launch-0.0.1.dist-info/WHEEL
+Filename: simple_launch-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: simple_launch-0.0.1.dist-info/entry_points.txt
+Filename: simple_launch-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: simple_launch-0.0.1.dist-info/top_level.txt
+Filename: simple_launch-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_launch-0.0.1.dist-info/RECORD
+Filename: simple_launch-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_launch.py

```diff
@@ -1,26 +1,28 @@
 import argparse
 from contextlib import suppress
 from ctypes import ArgumentError
 import asyncio
 import gc
 import importlib
+import shutil
 import yaml
 from typing import NamedTuple, List, Dict
 from enum import Enum
 import threading
 import traceback
 import appdirs
 from pathlib import Path
 import sys
 from datetime import datetime
 import os
 import time
 import signal
 import subprocess
+import simple_launch_process
 
 
 class SimpleTask(NamedTuple):
     name: str
     program: str
     cwd: str
     args: List[str]
@@ -47,19 +49,20 @@
         self.task_launch = task_launch
         self.log_dir = log_dir
         self.loop = loop
         self._keep_going = True
         self._process = None
         self._term_attempts = 0
         self.screen = parent.screen
+        self.exit_status = -1
     
     async def run(self):
         s = self.task_launch
-        stdout_log_fname = self.log_dir.joinpath(f"{s.name}.txt")
-        stderr_log_fname = self.log_dir.joinpath(f"{s.name}.stderr.txt")
+        stdout_log_fname = self.log_dir.joinpath(f"{s.name}.log")
+        stderr_log_fname = self.log_dir.joinpath(f"{s.name}.stderr.log")
         with open(stdout_log_fname,"w") as stdout_log, open(stderr_log_fname,"w") as stderr_log:
             if s.start_delay > 0:
                 stderr_log.write(f"Delaying starting {s.name} for {s.start_delay} seconds...\n")
                 with suppress(asyncio.TimeoutError):
                     await asyncio.wait_for(self.parent.exit_event.wait(),timeout=s.start_delay)
                 if not self._keep_going:
                     return
@@ -70,15 +73,15 @@
                     python_exe = sys.executable
                     self._process = await create_subprocess_exec(s.program, s.args, s.environment, s.cwd)
                     # print(f"process pid: {self._process.pid}")
                     stderr_log.write(f"Process {s.name} started\n\n")                   
                     self.parent.process_state_changed(s.name,ProcessState.RUNNING)
                     stdout_read_task = asyncio.ensure_future(self._process.stdout.readline())
                     stderr_read_task = asyncio.ensure_future(self._process.stderr.readline())
-                    while self._keep_going:
+                    while True: #self._keep_going:
                         wait_tasks = list(filter(lambda x: x is not None, [stdout_read_task, stderr_read_task]))
                         if len(wait_tasks) == 0:
                             break
                         done, pending = await asyncio.wait(wait_tasks,return_when=asyncio.FIRST_COMPLETED)
                         if stderr_read_task in done:
                             stderr_line = await stderr_read_task
                             if len(stderr_line) == 0:
@@ -95,15 +98,22 @@
                                 stdout_read_task = None
                             else:
                                 stdout_log.write(stdout_line.decode("utf-8"))
                                 stdout_log.flush()
                                 stdout_read_task = asyncio.ensure_future(self._process.stdout.readline())
                                 if self.screen:
                                     print(f"[{self.task_launch.name}]  " + stdout_line.decode("utf-8"),end="",file=sys.stdout)
+                        if stdout_read_task is None and stderr_read_task is None:
+                            break
                     await self._process.wait()
+                    self.exit_status = self._process.get_exit_status()
+                    if self.exit_status != 0:
+                        stderr_log.write(f"Process {s.name} exited with status {self.exit_status}\n")
+                        if self.screen:
+                            print(f"[{self.task_launch.name}]  Process {s.name} exited with status {self.exit_status}",file=sys.stderr)
                     self.parent.process_state_changed(s.name,ProcessState.STOPPED)
                 except:
                     self._process = None
                     self.parent.process_state_changed(s.name,ProcessState.STOPPED)
                     traceback.print_exc()
                     stderr_log.write(f"\nProcess {s.name} error:\n")
                     stderr_log.write(traceback.format_exc())
@@ -241,23 +251,31 @@
                 print("Sending processes still running SIGKILL")                
                 time.sleep(2)               
 
             #self._loop.stop()
         except:
             traceback.print_exc()
 
+    def get_exit_status(self):
+        exit_status = 0
+        with self._lock:
+            for p in self._subprocesses.values():
+                if p.exit_status != 0:
+                    exit_status = p.exit_status
+        return exit_status
+
 
 async def create_subprocess_exec(process, args, env, cwd):
     if sys.platform == "win32":
         job_handle = subprocess_impl_win32.win32_create_job_object()
 
         process = await asyncio.create_subprocess_exec(process,*args, \
             stdout=asyncio.subprocess.PIPE,stderr=asyncio.subprocess.PIPE,\
-            env=env, cwd=cwd, creationflags=subprocess_impl_win32.CREATE_SUSPENDED # \
-            #| subprocess.CREATE_NEW_PROCESS_GROUP 
+            env=env, cwd=cwd, creationflags=subprocess_impl_win32.CREATE_SUSPENDED \
+            | subprocess.CREATE_NEW_PROCESS_GROUP 
             ,close_fds=True)
 
         subprocess_impl_win32.win32_attach_job_and_resume_process(process, job_handle)
 
         return SimpleSubprocessImpl(process,job_handle)
 
     else:
@@ -313,14 +331,18 @@
             subprocess_impl_win32.win32_close_job_object(self._job_handle)
         else:
             try:
                 self._process.kill()
             except Exception:
                 pass
 
+    def get_exit_status(self):
+        return self._process.returncode
+
+
 if sys.platform == "win32":
     import ctypes.wintypes
     class _JOBOBJECT_BASIC_LIMIT_INFORMATION(ctypes.Structure):
         _fields_ = [
                 ('PerProcessUserTimeLimit', ctypes.wintypes.LARGE_INTEGER),
                 ('PerJobUserTimeLimit', ctypes.wintypes.LARGE_INTEGER),
                 ('LimitFlags', ctypes.wintypes.DWORD),
@@ -490,46 +512,31 @@
                 return
 
         def _win32_send_ctrl_c_event(pid):
             ctypes.windll.kernel32.GenerateConsoleCtrlEvent(1,pid)
 
     _CtrlCHandlerRoutine = ctypes.WINFUNCTYPE(ctypes.wintypes.BOOL, ctypes.wintypes.DWORD)
 
-class _ConfigCtrlCPressedHandler:
-
-    def __init__(self, handler):
-        self.handler = handler
-        
-        if sys.platform == "win32":
-            # Configure win32 callback for ctrl-c            
-            self.ctrl_c_handler_ptr = _CtrlCHandlerRoutine(self.win_ctrl_c_handler)
-            
-            ctypes.windll.kernel32.SetConsoleCtrlHandler(self.ctrl_c_handler_ptr, 1)
-        else:
-            signal.signal(signal.SIGINT, handler)
-            signal.signal(signal.SIGTERM, handler)
-
-    def win_ctrl_c_handler(self,code):
-        try:
-            print("Ctrl-C pressed")
-            self.handler(signal.SIGINT,0)
-        except:
-            traceback.print_exc()
-        return True
-
 def parse_task_launch_from_yaml(yaml_dict, cwd):
     # parse yaml_dict into SimpleTask tuple
     name = yaml_dict["name"]
     program = yaml_dict["program"]
     cwd = yaml_dict.get("cwd", cwd)
     args = yaml_dict.get("args", None)
     if args is None:
         args = []
     else:
-        args = args.split()
+        if isinstance(args,str):
+            args = args.split()
+        if isinstance(args,bool) or isinstance(args,int) or isinstance(args,float):
+            # Corner case where args is another yaml type
+            args = [str(args)]
+        else:
+            assert isinstance(args,list), "process args must be a string or list"
+            args = [str(a) for a in args]
     restart = yaml_dict.get("restart", False)
     restart_backoff = yaml_dict.get("restart-backoff", 5)
     tags = yaml_dict.get("tags", [])
     env = os.environ.copy()
     env.update(yaml_dict.get("environment", {}))
     start_delay = yaml_dict.get("start-delay", 0)
     quit_on_terminate = yaml_dict.get("quit-on-terminate", False)
@@ -547,14 +554,19 @@
                         # remove trailing comment
                         env_line = env_line.split("#", 1)[0]
                     env_line_split = env_line.split("=", 1)
                     if len(env_line_split) == 2:
                         env[env_line_split[0]] = env_line_split[1]
                 env_line = f.readline()
 
+    if(Path(program).name == program):
+        program = shutil.which(program, path=env["PATH"])
+        if program is None:
+            raise Exception("Could not find program: {}".format(program))
+
     return SimpleTask(
         name=name,
         program=program,
         cwd=cwd,
         args=args,
         restart=restart,
         restart_backoff=restart_backoff,
@@ -652,41 +664,46 @@
         with open(parser_results.config, "r") as f:
             name, task_launch = parse_task_launches_from_yaml(f, parser_results.cwd)
 
         name = parser_results.name if parser_results.name is not None else name
         if name is None:
             name = "simple-launch"
 
-        timestamp = datetime.now().strftime("simple-launch-%Y-%m-%d--%H-%M-%S")
-        log_dir = Path(appdirs.user_log_dir(appname="simple-launch")).joinpath(name).joinpath(timestamp)
+        timestamp = datetime.now().strftime("-%Y-%m-%d--%H-%M-%S")
+        log_dir = Path(appdirs.user_log_dir(appname="simple-launch")).joinpath(name).joinpath(name + timestamp)
         log_dir.mkdir(parents=True, exist_ok=True)        
         loop = asyncio.get_event_loop()
                         
         exit_event = asyncio.Event()
         core = SimpleCore(parser_results.name, task_launch, exit_event, log_dir, not parser_results.quiet, loop)
         gui = None
         if parser_results.gui:
             gui = SimpleGui(name, core, exit_event)
             gui.start()
         loop.call_soon(lambda: core.start_all())
-        def ctrl_c_pressed(signum, frame):
+        def ctrl_c_pressed():
             loop.call_soon_threadsafe(lambda: exit_event.set())
             loop.call_soon_threadsafe(lambda: core.close())
-        exit_handler = _ConfigCtrlCPressedHandler(ctrl_c_pressed)
+        simple_launch_process.wait_exit_callback(ctrl_c_pressed)
         print("Press Ctrl-C to exit")        
         loop.run_until_complete(exit_event.wait())
         print("Exit received, closing")
         core.close()
         loop.run_until_complete(core.wait_all_closed())
         #pending = asyncio.all_tasks(loop)
         # pending = asyncio.all_tasks()
         #loop.run_until_complete(asyncio.gather(*pending))
         if gui is not None:
             gui.close()
         print("Exiting!")
+        exit_status = core.get_exit_status()
+        if exit_status != 0:
+            print(f"Exit status: {exit_status}")
+        sys.exit(exit_status)
     except Exception:
         traceback.print_exc()
+        raise
     
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `simple_launch-0.0.1.dist-info/LICENSE.txt` & `simple_launch-0.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `simple_launch-0.0.1.dist-info/METADATA` & `simple_launch-0.1.0.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 Metadata-Version: 2.1
 Name: simple-launch
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple launcher for Robotics applications
 Author-email: John Wason <wason@wasontech.com>
 License: Apache-2.0
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyyaml
 Requires-Dist: appdirs
+Provides-Extra: test
+Requires-Dist: pytest ; extra == 'test'
+Requires-Dist: pywin32 ; (platform_system == "Windows") and extra == 'test'
 
 # Simple Launch
 
 **WARNING: THIS IS UNFINISHED SOFTWARE**
 
 `simple-launch` is a simple tool to launch and manage multiple processes. It is based on the process management code
 extracted from the `pyri-core` module, part of the PyRI Open-Source Teach Pendant
 
 `simple-launch` has a similar goal to `roslaunch`, but
 designed to be simpler and independent of ROS. It also has improvements in handling Windows process management
 using Windows Job Objects. Yaml files are used to configure the processes to launch.
 
+`simple-launch` will show a minimal GUI windows when the `--gui` is specified. This window shows same basic
+information, and has a "Stop All" button that will shut down all tasks. This GUI is useful if `simple-launch` is 
+started interactively by the user rather than running as a background service.
+
+See also `simple-launch-process`, a companion library that contains utility functions to use within processes
+hosted by `simple-launch`. The functions `wait_exit()` and `wait_exit_callback()` assist in receiving shutdown
+signals in a reliable cross-platform manner.
+
+See `simple-launch-process`: https://github.com/johnwason/simple-launch-process
+
 ## Installation
 
 ```
 python -m pip install --user simple-launch
 ```
 
 On Ubuntu, it may be necessary to replace `python` with `python3`.
@@ -35,23 +48,27 @@
 file that launches two Python servers.
 
 ```yaml
 name: example_http_servers
 tasks:
   - name: http_server_1
     program: python.exe
-    args: -m http.server 8100
-    cwd: ./server1
+    args: example_http_server.py 8100 Server1
+    cwd: .
   - name: http_server_2
     program: python.exe
-    args: -m http.server 8101
-    cwd: ./server2
+    args:
+      - example_http_server.py
+      - 8101
+      - Hello from Server2!
     start-delay: 1
 ```
 
+The `example_http_server.py` program uses `simple-launch-process` to wait for the shutdown signal.
+
 In this example, the `name` field is the name of the launch group. The `tasks` section contains a list of tasks to 
 launch. The following fields are used to configure the launch of each task:
 
 * `name`: The name of the process
 * `program`: The program to execute
 * `args`: The command line arguments to pass to `program`
 * `cwd` (optional): The working directory to run the program. Defaults to current directory.
```

