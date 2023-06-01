# Comparing `tmp/gdb_plus-6.2.0.tar.gz` & `tmp/gdb_plus-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb_plus-6.2.0.tar", last modified: Sat May  6 10:25:50 2023, max compression
+gzip compressed data, was "gdb_plus-6.3.0.tar", last modified: Thu Jun  1 20:45:46 2023, max compression
```

## Comparing `gdb_plus-6.2.0.tar` & `gdb_plus-6.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.876994 gdb_plus-6.2.0/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.2.0/LICENSE
--rwxrwxrwx   0 edo       (1000) edo       (1000)    12629 2023-05-06 10:25:50.875850 gdb_plus-6.2.0/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)    12410 2023-05-06 08:12:37.000000 gdb_plus-6.2.0/README.md
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.833814 gdb_plus-6.2.0/gdb_plus/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    11259 2023-05-06 01:40:48.000000 gdb_plus-6.2.0/gdb_plus/Inner_Debugger.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-05-05 17:49:09.000000 gdb_plus-6.2.0/gdb_plus/__init__.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    84636 2023-05-06 08:12:37.000000 gdb_plus-6.2.0/gdb_plus/gdb_plus.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    74194 2023-05-06 08:12:30.000000 gdb_plus-6.2.0/gdb_plus/gdb_plus_dev_libdebug.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)     5031 2023-05-06 01:38:11.000000 gdb_plus-6.2.0/gdb_plus/utils.py
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.863436 gdb_plus-6.2.0/gdb_plus.egg-info/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    12629 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)      326 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/requires.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-05-06 10:25:50.000000 gdb_plus-6.2.0/gdb_plus.egg-info/top_level.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)      656 2023-05-06 01:40:57.000000 gdb_plus-6.2.0/pyproject.toml
--rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-05-06 10:25:50.877347 gdb_plus-6.2.0/setup.cfg
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-05-06 10:25:50.865858 gdb_plus-6.2.0/tests/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    17513 2023-05-06 01:38:11.000000 gdb_plus-6.2.0/tests/test.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.975666 gdb_plus-6.3.0/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.3.0/LICENSE
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:45:46.975336 gdb_plus-6.3.0/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    13367 2023-06-01 20:44:31.000000 gdb_plus-6.3.0/README.md
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.971183 gdb_plus-6.3.0/gdb_plus/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    12472 2023-05-31 21:09:49.000000 gdb_plus-6.3.0/gdb_plus/Inner_Debugger.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-06-01 20:03:48.000000 gdb_plus-6.3.0/gdb_plus/__init__.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    99843 2023-06-01 20:01:57.000000 gdb_plus-6.3.0/gdb_plus/gdb_plus.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    99228 2023-06-01 20:05:39.000000 gdb_plus-6.3.0/gdb_plus/gdb_plus_arm_dev.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)     5125 2023-05-22 18:36:02.000000 gdb_plus-6.3.0/gdb_plus/utils.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.974073 gdb_plus-6.3.0/gdb_plus.egg-info/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      321 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/requires.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      657 2023-06-01 20:45:08.000000 gdb_plus-6.3.0/pyproject.toml
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-06-01 20:45:46.975764 gdb_plus-6.3.0/setup.cfg
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.974584 gdb_plus-6.3.0/tests/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    20197 2023-06-01 16:55:57.000000 gdb_plus-6.3.0/tests/test.py
```

### Comparing `gdb_plus-6.2.0/LICENSE` & `gdb_plus-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.2.0/PKG-INFO` & `gdb_plus-6.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb_plus
-Version: 6.2.0
+Version: 6.3.0
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -34,15 +34,15 @@
 ```
 or dev branch
 ```
 pip3 install git+https://github.com/Angelo942/gdb_plus.git@dev
 ```
 
 **Warning for pwndbg users:**  
-Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork.
+Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork, making it almost impossible to use features such as the emulation of ptrace.   
 you are strongly advised to use [GEF](https://github.com/hugsy/gef) instead.
 
 ## Debugging
 
 You can debug a program using the path to the binary.   
 If you really have to you can also use a process or even just his pid. 
 For pwn challenges set the remote address with `Debugger().remote(<host>, <port>)` and use the argument `REMOTE` once you want to exploit the server
@@ -112,15 +112,15 @@
 dbg.p.sendline(b"4")
 done.wait()
 # Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
 ...
 ```
 
 **Warning**  
-* `finish` can only work if the stack frame hasn't been corrupted
+* `finish` can only work if the stack frame hasn't been corrupted. With libdebug it will fail if the function doesn't use the base pointer.
 * Try avoiding `interrupt` as much as possible. 
 * You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
 
 If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
 
 ```py
 def MyCallback(dbg):
@@ -269,19 +269,41 @@
 
 **Note**  
 You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
 
 **Warning**  
 If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
 
-## Alternatives
-from version 6.0 gdb_plus should be able to script anything you can imagine, but you it can be slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit development you may prefer something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
+## Libdebug
+By default GDB+ uses a gdbserver to debug the process. This is verry usefull when you also have to check manually gdb while you are writing a script, but can be verry slow. For this reason we now support libdebug (from version >= 0.4) as an alternative debugger. It is lacking a lot of features but can do the job for most tasks and it can be 50 times faster. 
+
+The debugger will always start with dbg, but you can switch back and forth
+
+```py
+dbg = Debugger(<binary>)
+# switch to libdebug
+dbg.migrate(libdebug=True)
+# switch to gdb
+dbg.migrate(gdb=True)
+```
+
+To access properties of libdebug that haven't been wrapped you can simply use `dbg.libdebug` as you would with `dbg.gdb`.
+
+When you switch the breakpoints and callbacks will be preserved except for those needed to emulate ptrace. Please migrate to libdebug before setting the emulator up or disable it and set it up again right after.
+
+Since libdebug isn't on PyPI yet we could't include it in the dependencies. 
+You can install it manually:
+`pip3 install git+https://github.com/Angelo942/libdebug.git@parallel`
 
 # TODO
 
-* Add option to use libdebug instead of gdb
-* Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
     * register waitpid return value
-* Maybe nop split_on_fork&co while debugging is False
+* Stack multiple callbacks on the same breakpoint
+* handle Hardware breakpoint
+* support ARM binaries
+* support multithread applications
+* setup gdbinit for forked processes
+* catch sigsegv as an exit instead of user interaction
+* enable signal() with libdebug
```

### Comparing `gdb_plus-6.2.0/README.md` & `gdb_plus-6.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```
 or dev branch
 ```
 pip3 install git+https://github.com/Angelo942/gdb_plus.git@dev
 ```
 
 **Warning for pwndbg users:**  
-Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork.
+Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork, making it almost impossible to use features such as the emulation of ptrace.   
 you are strongly advised to use [GEF](https://github.com/hugsy/gef) instead.
 
 ## Debugging
 
 You can debug a program using the path to the binary.   
 If you really have to you can also use a process or even just his pid. 
 For pwn challenges set the remote address with `Debugger().remote(<host>, <port>)` and use the argument `REMOTE` once you want to exploit the server
@@ -98,15 +98,15 @@
 dbg.p.sendline(b"4")
 done.wait()
 # Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
 ...
 ```
 
 **Warning**  
-* `finish` can only work if the stack frame hasn't been corrupted
+* `finish` can only work if the stack frame hasn't been corrupted. With libdebug it will fail if the function doesn't use the base pointer.
 * Try avoiding `interrupt` as much as possible. 
 * You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
 
 If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
 
 ```py
 def MyCallback(dbg):
@@ -255,19 +255,41 @@
 
 **Note**  
 You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
 
 **Warning**  
 If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
 
-## Alternatives
-from version 6.0 gdb_plus should be able to script anything you can imagine, but you it can be slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit development you may prefer something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
+## Libdebug
+By default GDB+ uses a gdbserver to debug the process. This is verry usefull when you also have to check manually gdb while you are writing a script, but can be verry slow. For this reason we now support libdebug (from version >= 0.4) as an alternative debugger. It is lacking a lot of features but can do the job for most tasks and it can be 50 times faster. 
+
+The debugger will always start with dbg, but you can switch back and forth
+
+```py
+dbg = Debugger(<binary>)
+# switch to libdebug
+dbg.migrate(libdebug=True)
+# switch to gdb
+dbg.migrate(gdb=True)
+```
+
+To access properties of libdebug that haven't been wrapped you can simply use `dbg.libdebug` as you would with `dbg.gdb`.
+
+When you switch the breakpoints and callbacks will be preserved except for those needed to emulate ptrace. Please migrate to libdebug before setting the emulator up or disable it and set it up again right after.
+
+Since libdebug isn't on PyPI yet we could't include it in the dependencies. 
+You can install it manually:
+`pip3 install git+https://github.com/Angelo942/libdebug.git@parallel`
 
 # TODO
 
-* Add option to use libdebug instead of gdb
-* Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
     * register waitpid return value
-* Maybe nop split_on_fork&co while debugging is False
+* Stack multiple callbacks on the same breakpoint
+* handle Hardware breakpoint
+* support ARM binaries
+* support multithread applications
+* setup gdbinit for forked processes
+* catch sigsegv as an exit instead of user interaction
+* enable signal() with libdebug
```

### Comparing `gdb_plus-6.2.0/gdb_plus/Inner_Debugger.py` & `gdb_plus-6.3.0/gdb_plus/Inner_Debugger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from gdb_plus import *
 from os import kill
 from time import sleep
 from functools import partial
 from capstone import Cs, CS_ARCH_X86
 from gdb_plus.utils import Inner_Breakpoint
 
+#import logging
+#log = logging.getLogger("gdb_plus-inner_debugger")
+
 INT3 = b"\xcc"
 constants.PTRACE_GETREGS = 0xc
 constants.PTRACE_SETREGS = 0xd
 
 # Only work if parent is tracing child (otherwise why would you need this class ?) and if the child is at a stop [02/03/23]
 class Inner_Debugger:
     def __init__(self, dbg: Debugger, pid: int):
         self.dbg = dbg
         self.pid = pid
         self._mem_file = None # instead of opening it every time
         self.breakpoints = {}
+        # We can not cache the registers because we don't know if the child continues due to the parrent [31/05/23]
+        # We could change the ptrace emulation too, but for know we are going fast enough [31/05/23]
+        #self.__registers = None
+        self.__pointer_registers = None
 
         self.dbg.restore_arch()
 
     def get_regs(self):
         registers = user_regs_struct()
-        pointer_registers = self.dbg.alloc(registers.size)
-        res = self.dbg.call("ptrace", [constants.PTRACE_GETREGS, self.pid, 0, pointer_registers])
+        if self.__pointer_registers is None:
+            self.__pointer_registers = self.dbg.alloc(registers.size)
+        res = self.dbg.call("ptrace", [constants.PTRACE_GETREGS, self.pid, 0, self.__pointer_registers])
         assert res != 2**context.bits - 1
-        #self.dbg.syscall(constants.SYS_ptrace, [constants.PTRACE_GETREGS, self.pid, 0, pointer_registers])
-        registers.set(self.dbg.read(pointer_registers, registers.size))
-        self.dbg.dealloc(pointer_registers)
+        #self.dbg.syscall(constants.SYS_ptrace, [constants.PTRACE_GETREGS, self.pid, 0, self.__pointer_registers])
+        registers.set(self.dbg.read(self.__pointer_registers, registers.size))
         return registers
 
     def set_regs(self, registers):
-        pointer_registers = self.dbg.alloc(registers.size)
-        self.dbg.write(pointer_registers, registers.get())
-        self.dbg.call("ptrace", [constants.PTRACE_SETREGS, self.pid, 0, pointer_registers])
-        self.dbg.dealloc(pointer_registers)
+        self.dbg.write(self.__pointer_registers, registers.get())
+        self.dbg.call("ptrace", [constants.PTRACE_SETREGS, self.pid, 0, self.__pointer_registers])
         return registers
-
+    
     def read_memory(self, addr, size) -> bytes:
         buffer = self.dbg.alloc(size)
         self.dbg.syscall(constants.SYS_lseek.real, [self.mem_file, addr, constants.SEEK_SET.real])
         self.dbg.syscall(constants.SYS_read.real, [self.mem_file, buffer, size])
         data = self.dbg.read(buffer, size)
         self.dbg.dealloc(buffer)
         return data
@@ -87,28 +92,45 @@
 
     # Per evitare chiamate ciclice provando a gestire i breakpoints
     def _cont(self, wait = False):
         self.dbg.call("ptrace", [constants.PTRACE_CONT, self.pid, 0, 0])
         if wait:
             self.wait()
 
-    # Please, never ever put two breakpoints next to each others as a user (using next is fine) [03/03/23]
+    # Please, never ever put two breakpoints next to each others as a user (using next is fine) [03/03/23] # Maybe not needed anymore
+    # Clear last_breakpoint ?
     def cont(self, *, wait=False, until=None) -> None:
         if until is not None:
             log.warn_once("dbg.cont(until=ADDRESS) is deprecated, use dbg.continue_until(ADDRESS) instead!")  
             self.continue_until(until)  
         self.step()
-        if self.instruction_pointer not in self.breakpoints:    
+        # Wait, handle the case where breakpoints are temporary!! [26/05/23]
+        # This can't work with libdebug...
+        #if self._stop_reason != "SINGLE STEP":
+        #    if "BREAKPOINT" not in self._stop_reason:
+        #        if DEBUG:
+        #            log.warn(f"unknown interuption! {self._stop_reason}")
+        #    if DEBUG:
+        #        log.debug(f"step in continue already reached the breakpoint")
+        #    return
+        if self.instruction_pointer not in self.breakpoints: # Add last deleted breakpoint ?    
             self._cont(wait)
 
     c = cont
 
-    def continue_until(self, location):
+    def continue_until(self, location, loop=False):
         ip = self.instruction_pointer
         address = self.dbg.parse_address(location)
+        if address == ip:
+            if not loop:
+                if DEBUG:
+                    log.debug(f"I'm already at {self.dbg.reverse_lookup(address)}")
+                    log.warn_once("Be careful that the default behaviour changed. Use loop=True if you want to continue anyway")
+            else:
+                self.step()
         self.b(address, temporary=True)
         self.cont(wait=True)
         if address != self.instruction_pointer:
             log.critical(f"couldn't reach address {hex(address)}. Stopped at address {hex(self.instruction_pointer)} instead")
 
     until = continue_until
```

### Comparing `gdb_plus-6.2.0/gdb_plus/gdb_plus.py` & `gdb_plus-6.3.0/gdb_plus/gdb_plus_arm_dev.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from pwn import *
+import pwn
 import os
 from time import sleep
 from functools import partial
-from capstone import Cs, CS_ARCH_X86
+from capstone import Cs, CS_ARCH_X86, CS_ARCH_ARM64, CS_MODE_ARM
 from threading import Event
 from queue import Queue
 from gdb_plus.utils import Arguments, user_regs_struct, context, MyEvent, Breakpoint
+from libdebug import Debugger as lib_Debugger
 
 RET = b"\xc3"
 DEBUG_OFF = "Debug is off, commands won't be executed"
+# Yah, there should be a way to handle the logs and hide those from the library, but will look into it another day.
+DEBUG = True # Flag for when I'm debugging the library
 
 class Debugger:
     # If possible patch the rpath (spwn and pwninit do it automatically) instead of using env to load the correct libc. This will let you get a shell not having problems trying to preload bash too
-    def __init__(self, target: [int, process, str, list], env={}, aslr:bool=True, script:str="", from_start:bool=True, binary:str=None, debug_from: int=None, timeout: int=0.5):
+    def __init__(self, target: [int, process, str, list], env={}, aslr:bool=True, script:str="", from_start:bool=True, binary:str=None, debug_from: int=None, timeout: int=0.5, qemu_arch=None, qemu_path=None, qemu_port=10001):
         log.debug(f"debugging {target if binary is None else binary} using arch: {context.arch} [{context.bits}bits]")
 
         self._capstone = None #To decompile assembly for next_inst
         self._auxiliary_vector = None #only used to locate the canary
         self._base_libc = None
         self._base_elf = None
         self._canary = None
@@ -30,28 +34,29 @@
         self._wait_signal = None
         self._free_bss = None #Used to allocate data in the bss if you can't use the heap
         # Do we want to save temporary breakpoints too ? [17/04/23]
         self.breakpoints = {} #Save all non temporary breakpoints for easy access # The fact that they can't be temporary is used by the callback [21/03/23]
         self.gdbscript = script # For non blocking debug_from
         self.debug_from_done = Event()
 
+        # MyEvent allows calls to wait in parallel
+        self.myStopped = MyEvent() # Include original event
+        self.myStopped.set() # we call __setup_gdb after an attach so the process isn't running. Make just sure this doesn't cause troubles [17/04/23]
+
         # To know that I'm responsible for the interruption even if there is no callback
         self.stepped = False
         self.interrupted = False
         # Maybe not needed (see set_split_on_fork)
         self.last_breakpoint_deleted = 0 # Keep track of the last temporary breakpoint deleted if we realy have to know if we hit something
 
         if args.REMOTE or context.noptrace:
             self.debugging = False
         else:
             self.debugging = True
 
-        # The idea was to let gdb interrupt only one inferior while letting the other one run, but this doesn't work [29/04/23]
-        #script = "set target-async on\nset pagination off\nset non-stop on" + script
-
         if type(target) is int:
             self.p = None
             self.pid = target
             assert binary is not None, "I need a file to work from a pid" # Not really... Let's keep it like this for now, but continue assuming we don't have a real file
             self.elf = ELF(binary, checksec=False)
             _, self.gdb = gdb.attach(target, gdbscript=script, api=True)
 
@@ -86,43 +91,38 @@
                     del self.elf.symbols[name]
 
         # Because pwntools context isn't perfect
         self.restore_arch()
 
         if self.debugging:
             self.elf.address = self.get_base_elf()
+            self.__setup_gdb()
 
             # Start debugging from a specific address. Wait timeout seconds for the program to reach that address. Is blocking so you may need to use context.Thread() in some cases
             # WARNING don't use 'continue' in your gdbscript when using debug_from ! [17/04/23]
             # I don't like that this is blocking, so you can't interact while waiting... Can we do it differently ? [17/04/23]
             if debug_from is not None:
                 address_debug_from = self.parse_address(debug_from)
                 backup = self.inject_sleep(address_debug_from)
                 while True:  
                     self.detach()
                     sleep(timeout)
                     # what happens if there is a continue in script ? It should break the script, but usually it's the last instruction so who cares ? Just warn them in the docs [06/04/23]
                     _, self.gdb = gdb.attach(self.pid, gdbscript=script, api=True) # P is gdbserver...
+                    self.__setup_gdb()
                     if self.instruction_pointer - address_debug_from in range(0, len(backup)): # I'm in the sleep shellcode
                         self.write(address_debug_from, backup)
-                        # To allow call to wait inside the jump
-                        self.myStopped = self.gdb.stopped
-                        self.myStopped.priority = 0
-                        # should maybe rename priority_wait into wait and avoid this line [17/04/23]
-                        self.myStopped.priority_wait = lambda: self.myStopped.wait()
                         self.jump(address_debug_from)
                         break
                     else:
                         log.warn(f"{timeout}s timeout isn't enought to reach the code... Retrying...")
 
-            self.__setup_gdb()
-
     # We stopped using gdb's implementation of temporary breakpoints so that we can differentiate an interruption caused by my debugger and cause by the manual use of gdb 
     # Event could tell me which breakpoint has been hit or which signal cause the interruption
-    def __stop_handler(self):
+    def __stop_handler_gdb(self):
         """
         Actions that the debugger performs every time the process is interrupted
         Handle temporary breakpoints and callbacks
         """
         self.restore_arch()
 
         ## I don't want to use interrupt in split_on_fork
@@ -130,22 +130,25 @@
         #    pid = self.to_split.get()
         #    log.debug(f"found child {pid} to split out")
         #    self.children[pid] = self.split_child(pid=pid)
 
         # Current inferior will change to the inferior who stopped last
         ip = self.instruction_pointer
         bp = self.breakpoints.get(ip)
+
         log.debug(f"{self.current_inferior.pid} stopped at address: {hex(ip)} for {self._stop_reason}")
         
         if bp is None:
             if self.stepped or self.interrupted or self._stop_reason in ["SIGSTOP", "SIGTRAP"]: # SIGTRAP to handle known int3 in the code
                 # I hope that the case where we step and still end up on a breakpoint won't cause problems because we would not reset stepped... [29/04/23]
                 self.stepped = False
                 self.interrupted = False
                 self.__set_stop()
+            else:
+                log.debug("I stopped for a manual interaction")
             return            
         
         if bp.temporary:
             self.delete_breakpoint(ip)
 
         # TODO, it may be interesting to have the option to put an array of breakpoints for recursive functions [21/03/23]
         # something like
@@ -154,195 +157,301 @@
         #   if len(self.real_callbacks[ip]) == 0:
         #       del self.real_callbacks[ip]
         #else:
                         
         # This should let us keep control of the debugger even if we use gdb manually while emulating ptrace
         # Doesn't handle the case where we use ni and hit the breakpoint though... [17/04/23] TODO!
         # Doesn't even handle the case where I step, but I'm waiting in continue until
-        if bp.callback is not None and bp.callback(self) == False and self._stop_reason != "SINGLE STEP":
+        # Damn, gdb detects the breakpoint even if we don't run over the INT3... so this doesn't work. We never have reason SINGLE STEP with a breakpoint. We need another indication [10/05/23]
+        if bp.callback is not None and bp.callback(self) == False:# and self._stop_reason != "SINGLE STEP": 
             self.execute("c")
         else:
             self.__set_stop()  
+
+    def __stop_handler_libdebug(self):
+        """
+        Actions that the debugger performs every time the process is interrupted
+        Handle temporary breakpoints and callbacks
+        """
+        self.restore_arch()
+
+        # Current inferior will change to the inferior who stopped last
+        ip = self.instruction_pointer
+        bp = self.breakpoints.get(ip)
+
+        log.debug(f"{self.libdebug.__stopped_pid} stopped at address: {hex(ip)} with status: {hex(self.libdebug.__stop_status)}")
+
+        # I hope I won't touch a breakpoint at the same time
+        # Usually if I hit a breakpoint it should stop again. At least with step we have the step and then the sigchld 
+        # Will be a problem while stepping, but amen
+        if self.libdebug.__stop_status == 0x117f:
+            if DEBUG:
+                log.info("the child stopped and libdebug caught it. Let's continue waiting for Mario to change the options...")
+            # We have problems with the wait after the step...
+            #self.libdebug.cont(blocking=False)
+            #return
+        
+        if bp is None:
+            if self.stepped or self.interrupted:
+                self.stepped = False
+                self.interrupted = False
+            elif self.libdebug.__stop_status == 0x57f:
+                # Look into how to handle steps in libdebug [21/05/23]
+                if DEBUG:
+                    log.warn("I supose libdebug just stepped so let's pretend nothing happened")
+                return
+            else:
+                log.warn("why did I stop ???")
+            self.__set_stop()
+            return            
+        
+        if bp.temporary:
+            self.delete_breakpoint(ip)
+                
+        if bp.callback is not None and bp.callback(self) == False:
+            self.libdebug.cont(blocking=False)
+        else:
+            self.__set_stop()  
         
     def __setup_gdb(self):
         """
         setup of gdb's events
         """
-        # MyEvent allows calls to wait in parallel
-        self.myStopped = MyEvent() # Include original event
-        self.myStopped.set() # we call __setup_gdb after an attach so the process isn't running. Make just sure this doesn't cause troubles [17/04/23]
-
-        self.gdb.events.stop.connect(lambda event: context.Thread(target=self.__stop_handler).start())
+        self.gdb.events.stop.connect(lambda event: context.Thread(target=self.__stop_handler_gdb).start())
         
         def exit_handler(event):
             log.debug("setting stop because process exited")
             self.myStopped.pid = self.current_inferior.pid
             self.myStopped.set()
             self.closed.set()
 
         self.gdb.events.exited.connect(exit_handler)
 
         # Manually set by split_child
         self.split = Queue()
 
         # Ptrace_cont
         self.master_wants_you_to_continue = Event()
-        self.slave_has_stopped = Event()    
+        self.slave_has_stopped = Event()  
+
+    def __setup_libdebug(self):
+        self.libdebug.handle_stop = self.__stop_handler_libdebug
 
+        #def exit_handler(event):
+        #    ... 
+        #self.libdebug.handle_exit = exit_handler
+
+    # È già successo che wait ritorni -1 e crashi libdebug [08/05/23]
+    # Legacy callbacks won't be transfered over... It's really time to get rid of them [21/05/23]
+    def migrate(self, *, gdb=False, libdebug=False):
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
+        address = self.instruction_pointer
+        backup = self.inject_sleep(address)
+        self.detach()
+        if gdb:
+            assert self.gdb is None
+            log.debug("migrating to gdb")
+            self.libdebug = None
+            _, self.gdb = pwn.gdb.attach(self.pid, api=True)
+            self.__setup_gdb()
+            for address in self.breakpoints:
+                self.__breakpoint_gdb(address)
+        else:
+            assert self.libdebug is None
+            log.debug("migrating to libdebug")
+            self.gdb = None
+            self.libdebug = lib_Debugger()
+            self.libdebug.attach(self.pid)
+            assert not self.libdebug.running
+            self.__setup_libdebug()
+            for address in self.breakpoints:
+                self.__breakpoint_libdebug(address)
+        self.write(address, backup)
+        self.jump(address)
+ 
     # Because pwntools isn't perfect
     def restore_arch(self):
         """
         check that the context used by pwntools is correct
         """
+        global context
         if self.elf is not None and context.arch != self.elf.arch:
             log.debug("wrong context ! Updating...")
         context.arch = self.elf.arch
         context.bits = self.elf.bits
 
     def debug_from(self, location: [int, str], *, event=None, timeout=0.5):
         """
         Alternative debug_from which isn't blocking
         wait dbg.debug_from_done to know when to continue
 
         event: optional event to signal that you have finished the actions you needed to perform. Otherwise a timeout of 0.5s will be used
         """
-        address = self.parse_address(location)
-
-        if self.debugging:
-            def action():
-                backup = self.inject_sleep(address)
-                while True:  
-                    self.detach()
-                    if event is not None:
-                        event.wait()
-                        log.debug("user finished interaction. Proceeding with debug_from")
-                    log.warn("you haven't set an event to let me know when you finished interactiong with the process. I will give you half a second.")
-                    sleep(timeout)
-                    # Maybe the process is being traced and I can't attach to it yet
-                    try:
-                        # what happens if there is a continue in script ? It should break the script, but usually it's the last instruction so who cares ? Just warn them in the docs [06/04/23]
-                        _, self.gdb = gdb.attach(self.p.pid, gdbscript=self.gdbscript, api=True) # P is gdbserver...
-                    except Exception as e:
-                        log.debug(f"can't attach in debug_from because of {e}... Retrying...")
-                        continue
-                    self.__setup_gdb()
-                    if self.instruction_pointer - address in range(0, len(backup)): # I'm in the sleep shellcode
-                        self.write(address, backup)
-                        self.jump(address)
-                        self.debug_from_done.set()
-                        break
-                    else:
-                        log.warn(f"{timeout}s timeout isn't enought to reach the code... Retrying...")
-
-            context.Thread(target=action).start()
-        else:
+        if not self.debugging:
             log.warn_once(DEBUG_OFF)
             self.debug_from_done.set()
+            return
+
+        address = self.parse_address(location)
+
+        def action():
+            backup = self.inject_sleep(address)
+            while True:  
+                self.detach()
+                if event is not None:
+                    event.wait()
+                    log.debug("user finished interaction. Proceeding with debug_from")
+                log.warn("you haven't set an event to let me know when you finished interactiong with the process. I will give you half a second.")
+                sleep(timeout)
+                # Maybe the process is being traced and I can't attach to it yet
+                try:
+                    # what happens if there is a continue in script ? It should break the script, but usually it's the last instruction so who cares ? Just warn them in the docs [06/04/23]
+                    _, self.gdb = gdb.attach(self.p.pid, gdbscript=self.gdbscript, api=True) # P is gdbserver...
+                except Exception as e:
+                    log.debug(f"can't attach in debug_from because of {e}... Retrying...")
+                    continue
+                self.__setup_gdb()
+                if self.instruction_pointer - address in range(0, len(backup)): # I'm in the sleep shellcode
+                    self.write(address, backup)
+                    self.jump(address)
+                    self.debug_from_done.set()
+                    break
+                else:
+                    log.warn(f"{timeout}s timeout isn't enought to reach the code... Retrying...")
+        context.Thread(target=action).start()
         return self
 
     # Use as : dbg = Debugger("file").remote(IP, PORT)
     def remote(self, host: str, port: int):
         """
         Define the connection to use when the script is called with argument REMOTE
         """
         if args.REMOTE:
             self.p = remote(host, port)
         return self
 
     def detach(self, quit = True):
-        try:
-            self.execute("detach")
-        except:
-            log.debug("process already stopped")
-        try:
-            self.execute("quit") # Doesn't always work if after interacting manually
-        except EOFError:
-            log.debug("GDB successfully closed")
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
+        if self.gdb is not None:
+            try:
+                self.execute("detach")
+            except:
+                log.debug("process already stopped")
+            try:
+                self.execute("quit") # Doesn't always work if after interacting manually
+            except EOFError:
+                log.debug("GDB successfully closed")
+
+        elif self.libdebug is not None:
+            self.libdebug.detach()
+
+        else:
+            ...
 
     def close(self):
         self.detach()
         # Can't close the process if I just attached to the pid
         if self.p:
             self.p.close()
 
     # Now we may have problems if the user try calling it...
     # should warn to use execute_action and wait if they are doing something that will let the process run
     def execute(self, code: str):
         """ 
         Execute a command that does NOT require a wait later
         """
-        if self.debugging:
-            return self.gdb.execute(code, to_string=True)
-        else:
+        if not self.debugging:
             log.warn_once(DEBUG_OFF)
-
+            return ""
+        
+        if DEBUG:
+            log.debug(f"executing {code}")
+        return self.gdb.execute(code, to_string=True)
+        
     # I want a function to restart the process without closing and opening a new one
     # Not working properly
     def reset(self, argv=None, reload_elf=False):
         ...
 
     # Since reset doesn't work
     # Could be expanded with memory regions
     def backup(self) -> list:
         """
         Save the state of all registers
         """
+        if not self.debugging:
+            return
+
         values = []
         for register in self.special_registers + self.registers[:-1]: # exclude ip
             values.append(getattr(self, register))
         return values
         
     def restore_backup(self, backup: list):
         """
         Reset the state of all registers from a backup
         """
+        if not self.debugging:
+            return
+
         for name, value in zip(self.special_registers + self.registers[:-1], backup):
                 setattr(self, name, value)
 
     # Return old_inferior to know where to go back
     def switch_inferior(self, n: int) -> int:
         """
         For multi-process applications change the process you are working with in gdb
         """
+        if not self.debugging:
+            return
+
         # May not be accurate if you switched manually before
         old_inferior = self._inferior
         while self.gdb.selected_inferior().num != n:
             log.debug(f"switching to inferior {n}")
             self.execute(f"inferior {n}")
             log.debug(f"I'm inferior {self.gdb.selected_inferior()}")
             self._inferior = n
+        self.pid = self.current_inferior.pid
         return old_inferior
 
     @property
     def inferiors(self):
         return {inferior.num: inferior for inferior in self.gdb.inferiors()}
         #return (None,) + self.gdb.inferiors()
 
-    # Useless ? I wanted it for the interrupt, but info inferior requires to be at a halt [07/03/23]
     @property
     def current_inferior(self):
-        # trova ultimo id
-        # prendi ultima riga non nulla
-        #data = self.execute("info inferior").split("\n") # shouldn't it be "info inferiorS" ?
-        #for line in data:
-        #    line = line.split()
-        #    if line[0] == "*":
-        #        n = int(line[1])
-        #        return self.inferiors[n]
-        return self.gdb.selected_inferior()
+        if not self.debugging:
+            return
+
+        if self.gdb is not None:
+            return self.gdb.selected_inferior()
+
+        #elif self.libdebug is not None:
+        #   return ... 
 
     @property
     def args(self):
         """
         Access arguments of the current function
         Can be use to read and write
         Can only access a single argument at a time
         dbg.args[5] = 1 # Valid
         a, b = dbg.args[:2] # Not valid!
         """
+        if not self.debugging:
+            return
+
         if self._args is None:
             self._args = Arguments(self)
         return self._args 
 
     # Taken from GEF to handle slave interruption
     @property
     def _stop_reason(self) -> str:
@@ -383,92 +492,151 @@
    ########################## CONTROL FLOW ##########################
 
     # For commands that will make the process run and should handle priority
     def execute_action(self, command, sender=None):
         """
         Wrapper around execute to handle commands that will require a wait
         """
-        if self.debugging:
-            self.priority += 1
-            self.__clear_stop(sender if sender is not None else command)
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
+        self.priority += 1
+        self.__clear_stop(sender if sender is not None else command)
+        if self.gdb is not None:
             self.execute(command)
+        elif self.libdebug is not None and command != "":
+            command()
         else:
-            log.warn_once(DEBUG_OFF)
+            ...
+
+    def __continue_gdb(self, force, wait, done):
+        self.step(force=force)
+        if self._stop_reason != "SINGLE STEP":
+            if "BREAKPOINT" not in self._stop_reason:
+                if DEBUG:
+                    log.warn(f"unknown interuption! {self._stop_reason}")
+            if DEBUG:
+                log.debug(f"step in continue already reached the breakpoint")
+            done.set()
+            return
+        self.execute_action("continue", sender="continue")
+        # Damn, I may not want to wait at all... [22/05/23]
+        if wait:
+            self.priority_wait()
+            done.set()
 
+    def __continue_libdebug(self, force, wait, done):
+        # Continue in libdebug is already stepping [21/05/23]
+        # Maybe keep the step if force = True [22/O5/23]
+        #self.step(force=force)
+        ## I hit a breakpoint
+        #if self.instruction_pointer in self.breakpoints or self.instruction_pointer == self.last_breakpoint_deleted:
+        #    return
+        self.execute_action(lambda: context.Thread(target=self.libdebug.cont, kwargs={"blocking": False}).start(), sender="continue")
+        if wait:
+            self.priority_wait()
+            done.set()
+        
     # TODO make the option to have "until" be non blocking with an event when we reach the address [28/04/23] In other words migrate wait=False to wait=Event()
     def c(self, *, wait=True, force = False, until = None):
         """
         Continue execution of the process
 
         Arguments:
             wait: Should block your script until the next interruption ?
             until: Continue until a specified location. Your script will wait if you have to play with gdb manually.
 
-            force: gdb may bug and keep you at the same address after a jump or if the stackframe as been edited. If you notice this problem use force to bypass it 
+            force: gdb may bug and keep you at the same address after a jump or if the stackframe as been edited. If you notice this problem use force to bypass it. If you don't worry about a callback being called twice don't bother
         """
         self.restore_arch()
 
         if not self.debugging:
             log.warn_once(DEBUG_OFF)
             return
 
-        # I always step so if we catch a broken instruction we can inform the user [05/05/23]
-        # In case of force=False the program should continue anywhay since we are already stepping, but the program will still raise a warning. [05/05/23]
-        self.step(force=force)
-
         if until is not None:
             log.warn_once("dbg.cont(until=ADDRESS) is deprecated, use dbg.continue_until(ADDRESS) instead!")
             return self.continue_until(until, wait=True)
-        
-        self.execute_action("continue", sender="continue")
-        
+    
+        # I have to use an event instead of priority_wait() because I may have to stop after the step [22/05/23]
+        done = Event()
+
+        if self.gdb is not None:
+            self.__continue_gdb(force, wait, done)
+
+        elif self.libdebug is not None:
+            self.__continue_libdebug(force, wait, done)
+
+        else:
+            ...
+
         if wait:
-            self.priority_wait()
-        elif until is not None:
-            return done
+            done.wait()
         else:
             pass
             # I would like to return done too, but I'm sure the average user will try dbg.wait instead of done.wait
 
     cont = c
 
-    def __continue_until(self, address, done):
-        self.execute_action("continue", sender="continue_until")
-        self.priority_wait()
+    def __continue_until_gdb(self, address, done, force):
+        #Force = True is not needed since once we step the sigint will be caught and continue won't stop. I disable the warning since the user can do nothing about it [08/05/23]
+        #Force = True IS needed if you have a callback on that address... [10/05/23]
+        # I will keep the step this way to warn the user
+        self.cont(wait=True, force=force)
         # Should we take into consideration the inferior too ? [29/04/23]
         while self.instruction_pointer != address:
             log.info(f"debugger {self.pid} stopped at {hex(self.instruction_pointer)} for '{self._stop_reason}' instead of {hex(address)}")
             log.warn_once("I assume this happened because you are using gdb manually. Finish what you are doing and let the process run. I will handle the rest")
             self.execute_action("", sender="continue just to reset the wait")
             self.priority_wait()
         done.set()
 
-    def continue_until(self, location, /, *, wait=True):
+    def __continue_until_libdebug(self, address, done, force):
+        self.cont(wait=True, force=force)
+        if self.instruction_pointer != address:
+            log.critical("error in continue until")
+            raise Exception(f"debugger {self.pid} stopped at {hex(self.instruction_pointer)} with status {hex(self.libdebug.__stop_status)} instead of {hex(address)}")
+        done.set()
+            
+
+    def continue_until(self, location, /, *, wait=True, force=False, loop = False):
         """
         Continue until a specific address
         can be blocking or non blocking thanks to wait
-        It the function is called from the address you want to reach the intended behaviour is to supose you are in a loop and continue anyway
+        It the function is called from the address you want to reach the intended behaviour is to do nothing and return. Set loop=True to continue anyway
+        
         """ 
         done = Event()
+
         if not self.debugging:
             done.set()
             log.warn_once(DEBUG_OFF)
             return done
 
         self.restore_arch()
-        
-        self.step(force=True) # force=True just to be sure 
+
         address = self.parse_address(location)
-        if address == self.instruction_pointer:
+        if not loop and address == self.instruction_pointer:
+            if DEBUG:
+                log.debug(f"I'm already at {self.reverse_lookup(address)}")
+                log.warn_once("Be careful that the default behaviour changed. Use loop=True if you want to continue anyway")
             return
             
         self.b(address, temporary=True)
-        log.debug(f"{self.pid} continuing until {hex(address)}")
+        if DEBUG:
+            log.debug(f"{self.pid} continuing until {self.reverse_lookup(address)}")
 
-        context.Thread(target=self.__continue_until, args=(address, done)).start()
+        if self.gdb is not None:
+            context.Thread(target=self.__continue_until_gdb, args=(address, done, force)).start()
+        elif self.libdebug is not None:
+            context.Thread(target=self.__continue_until_libdebug, args=(address, done, force)).start()
+        else:
+            ...
+            
         if wait:
             done.wait()
         else:
             return done
 
     until = continue_until
 
@@ -505,36 +673,53 @@
         return self.myStopped.priority
 
     @priority.setter
     def priority(self, value):
         self.myStopped.priority = value
 
     def __clear_stop(self, name="someone", /):
-        log.debug(f"{self.current_inferior.pid} stopped has been cleared by {name}")
-        self.myStopped.clear()
+        if self.gdb is not None:
+            pid = self.current_inferior.pid
+        elif self.libdebug is not None:
+            pid = self.pid # Handle thread
+        else:
+            ...
+        if self.myStopped.is_set():
+            log.debug(f"{pid} stopped has been cleared by {name}")
+            self.myStopped.clear()
 
     def __set_stop(self):
-        log.debug(f"{self.current_inferior.pid} setting stopped in {hex(self.instruction_pointer)}")
+        if self.gdb is not None:
+            pid = self.current_inferior.pid
+        elif self.libdebug is not None:
+            pid = self.pid # Handle thread
+        else:
+            ...        
+        log.debug(f"{pid} setting stopped in {hex(self.instruction_pointer)}")
         # handle case where no action are performed after the end of a callback with high priority 
+        self.myStopped.pid = pid
         self.__clear_stop("__set_stop")
-        self.myStopped.pid = self.current_inferior.pid
         self.myStopped.set()
 
     #def wait_fork(self):
     #    self.gdb.forked.wait()
     #    self.gdb.forked.clear()
 
     def wait_split(self):
         """
         Wait for the process to fork
         set_split_on_fork() must be set before the call to fork
 
         Return:
             pid: pid of the child process
         """
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return 0
+
         pid = self.split.get()
         if pid == 0:
             raise Exception("What the fuck happened with split ???")
         return pid
 
     def advanced_continue_and_wait_split(self):
         log.warn("advanced_continue_and_wait_split is deprecated. Use cont(until=\"fork\"); finish(); wait_split() instead")
@@ -551,14 +736,20 @@
         self.master_wants_you_to_continue.clear()
 
     # Should handle multiple slaves ?
     def wait_slave(self):
         self.slave_has_stopped.wait()
         self.slave_has_stopped.clear()
 
+    def __interrupt_gdb(self):
+        pass
+
+    def __interrupt_libdebug(self):
+        pass
+
     # temporarily interrupt the execution of our process to get back control of gdb (equivalent of a manual ctrl+C)
     # don't worry about the "kill"
     # May cause problem with the priority [26/04/23]
     # Why does it allways interrupt the first inferior even when I switch to another one ?? [29/04/23]
     def interrupt(self):
         """
         Stop the process as you would with ctrl+C in gdb
@@ -578,16 +769,48 @@
             #self.wait(legacy=True, timeout=0.1)
             # Need priority if calling interrupt in callback for split while waiting for finish in another thread
             log.debug(f"interrupting inferior: {self.current_inferior} [pid:{self.current_inferior.pid}]")
             self.execute_action("interrupt", sender="interrupt")
             #os.kill(self.inferiors[self._inferior].pid, signal.SIGSTOP)
             self.priority_wait()
 
+    def interrupt(self):
+        # claim priority asap
+        self.execute_action("", sender="interrupt")
+
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
+        # Still not working properly, so let's wait before using running
+        #if not self.running:
+        #    return
+
+        if self.gdb is not None:
+            pid = self.current_inferior.pid
+        elif self.libdebug is not None:
+            pid = self.pid
+        else:
+            ...
+        log.debug(f"interrupting [pid:{self.pid}]")
+        os.kill(pid, signal.SIGSTOP)
+        self.priority_wait()
+
     manual = interrupt
 
+    def __step_gdb(self):
+        self.execute_action("si", sender="step")
+        self.priority_wait() 
+            
+    def __step_libdebug(self):
+        #self.libdebug.step() # Already waits
+        # shouldn't I use execute_action anyway ? # What if I hit a callback ?
+        # And is needed for clear_stop
+        self.execute_action(self.libdebug.step, sender="step")
+        self.priority_wait()
 
     # Next may break again on the same address, but not step
     # Why isn't force = True the default behaviour ? [29/04/23]
     # I don't use force=True by default because there are instructions that keep the instruction pointer at the same address even if executed [05/05/23]
     def step(self, repeat:int=1, *, force=False):
         """
         execute a single instruction
@@ -596,42 +819,51 @@
             repeat: step n times
             force : if the stackframe has been tampered with gdb may stay stuck on the current instruction. Use force to handle this bug in gdb
         """
         if not self.debugging:
             log.warn_once(DEBUG_OFF)
             return
         
+        log.debug(f"{self.pid} stepping")
+        # Should only be the first step, right ? [08/05/23]
+        if force:
+            self.__broken_step()
+            repeat -= 1
+
         for _ in range(repeat):
             address = self.instruction_pointer
+            
             self.stepped = True
-            self.execute_action("si", sender="step")
-            self.priority_wait() 
+
+            if self.gdb is not None:
+                self.__step_gdb()
+            elif self.libdebug is not None:
+                self.__step_libdebug()
+            else:
+                ...
+
             if address == self.instruction_pointer:
-                # If I want to handle here the case where gdb updates the stack_frame, but stays on the same address. Currently handled by "exit_broken_function" [23/03/23]
-                if force:
-                    self.step(force=True)
-                else:
-                    log.warn("You stepped, but the address didn't change. This may be due to a bug in gdb. If this wasn't the intended behaviour use force=True in the function step or continue you just called")
+                log.warn("You stepped, but the address didn't change. This may be due to a bug in gdb. If this wasn't the intended behaviour use force=True in the function step or continue you just called")
 
     si = step
 
     def __broken_step(self):
         old_ip = self.instruction_pointer
         callback = None
 
         # Remove callback to avoid calling it twice (Nice, this wasn't possible with legacy_callbacks) (I'm not sure if we could simply disable a breakpoint for a turn)
         if (bp := self.breakpoints.get(old_ip)) is not None:
             callback = bp.callback
             bp.callback = None
 
-        self.step()
-
-        while self.instruction_pointer == old_ip:
-                log.debug("Bug ret still present")
-                self.step()
+        n = self.step_until_condition(lambda self: self.instruction_pointer == old_ip, limit=5)
+        if n == -1:
+            raise Exception("Could not force step!")
+        if n > 0:
+            log.debug("Bug still present. Had to force {n} time(s)")
 
         if callback is not None:
             bp.callback = callback
 
     # For backward compatibility
     exit_broken_function = __broken_step
 
@@ -642,14 +874,18 @@
         Useful to analyse self modifying functions.
         
         Arguments:
             location: address or symbol to reach
             callback: optional function to call at each step
             limit: number of step before giving up. Set at 10.000 by default
         """
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
         address = self.parse_address(location)
         for i in range(limit):
             if callback is not None:
                 callback(self)
             if self.instruction_pointer == address:
                 return i
                 break
@@ -662,14 +898,18 @@
         """
         step until the end of the function
 
         Arguments:
             callback: optional function to call at each step
             limit: number of step before giving up. Set at 10.000 by default
         """
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
         for i in range(limit):
             if callback is not None:
                 callback(self)
             if self.next_inst.mnemonic == "ret":
                 return i
                 break
             self.step()
@@ -677,135 +917,164 @@
             log.warn_once(f"I made {limit} steps and haven't reached the end of the function...")
             return -1
 
     def step_until_condition(self, condition, limit=10_000):
         """
         Step until condition(self) returns True or limit exceeded
         """
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
         for i in range(limit):
             if condition(self):
                 return i
             self.step()
 
+        # Why not raise exception ? [10/05/23]
         log.warn_once(f"I made {limit} steps and haven't found what you are looking for...")
         return -1
 
-    def __next(self, repeat, done=None):
+    def __next(self, repeat, done):
         for _ in range(repeat):
             next_inst = self.next_inst
             if next_inst.mnemonic == "call":
-                self.c(until=self.instruction_pointer+next_inst.size)
+                self.continue_until(self.instruction_pointer+next_inst.size)
             else:
                 self.step()
-        if done is not None:
-            done.set()
+        done.set()
 
     # May not want to wait if you are going over a functions that need user interaction
     def next(self, wait:bool=True, repeat:int=1):
         done = Event()
 
         if not self.debugging:
             done.set()
             log.warn_once(DEBUG_OFF)
             return done
         
+        context.Thread(target=self.__next, args=(repeat, done)).start()
         if wait:
-            self.__next(repeat)
+            done.wait()
         else:
-            context.Thread(target=self.__next, args=(repeat, done)).start()
             return done
 
     ni = next
 
-    def __finish(self, repeat, done):
+    def __finish(self, repeat, force, done):
         # Should be possible to take immediatly the corresponding stack frame instead of using a loop [28/04/23]
         for _ in range(repeat):
             ip = self.__saved_ip
             log.debug(f"finish found next ip : {hex(ip)}")
             if ip == 0:
                 raise Exception("stack frame is broken or we are not in a function")
-            self.c(until=ip)
+            self.continue_until(ip, force=force)
         if done is not None:
             done.set()
 
     # May be dependent on the stack frame and cause problems after a jump [27/04/23]
-    def finish(self, *, wait:bool=True, repeat = 1):
+    def finish(self, *, wait:bool=True, repeat = 1, force = False):
         done = Event()    
         
         if not self.debugging:
             done.set()
             log.warn_once(DEBUG_OFF)
             return done
         
-        context.Thread(target=self.__finish, args=(repeat, done)).start()
+        context.Thread(target=self.__finish, args=(repeat, force, done)).start()
         if wait:
             done.wait()
         else:
             return done
 
+    def __jump_gdb(self, address):
+        # BUG setting rip this way may cause problems with si [30/04/23] 
+        #self.instruction_pointer = address
+        self.b(address, temporary=True)
+        self.execute_action(f"jump *{hex(address)}", sender="jump")
+        self.priority_wait()
+
+    def __jump_libdebug(self, address):
+        self.instruction_pointer = address
+
     # How to handle a jump no wait without destroying the priority queue ? [17/04/23]
     # Don't let it as an option... [17/04/23]
-    def jump(self, location: [int, str], stop = True):
+    def jump(self, location: [int, str]):
         """
         Jump to specified location
         """
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
         #log.warn_once("jump is deprecated. Overwrite directly the instruction pointer instead")
         address = self.parse_address(location)
-        # BUG setting rip this way may cause problems with si [30/04/23] 
-        #self.instruction_pointer = address
-        self.b(address, temporary=True)
-        self.execute_action(f"jump *{hex(address)}", sender="jump")
-        self.priority_wait()
 
+        if address == self.instruction_pointer:
+            log.debug(f"not jumping because I'm already at {self.reverse_lookup(address)}")
+            return
+        
+        if DEBUG:
+            log.debug(f"jumping to {self.reverse_lookup(address)}")
+        if self.gdb is not None:
+            self.__jump_gdb(address)
+        elif self.libdebug is not None:
+            self.__jump_libdebug(address)
+        else:
+            ...
+        
     # Now can return from anywhere in the function
     # Works only for standard functions (push rbp; mov rbp, rsp; ...; leave; ret;). May crash if used in the libc
     # Can't I use __saved_ip now ? [28/04/23]
     def ret(self, value: int = None):
         """
         Exit from current function without executing it. 
 
         Warning: Experimental and depends on the stack frame
         """
-        #log.warn_once(f"ret is still at an experimental stage and may not work properly")
-        #if self.next_inst.toString() in ["endbr64", "push rbp", "push ebp"]:
-        #    pass
-        #elif self.next_inst.toString() in ["mov rbp, rsp", "mov ebp, esp"]:
-        #    self.pop() # Remove the base pointer # No need to place it back in rbp
-        #else:
-        #    self.stack_pointer = self.base_pointer
-        #    self.base_pointer = self.pop()
-        #ret_address = self.pop()
-        #self.instruction_pointer = ret_address
-        self.instruction_pointer = self.__saved_ip
+        if self.next_inst.toString() in ["endbr64", "push rbp", "push ebp"]:
+            pass
+        elif self.next_inst.toString() in ["mov rbp, rsp", "mov ebp, esp"]:
+            self.pop() # Remove the base pointer # No need to place it back in rbp
+        else:
+            self.stack_pointer = self.base_pointer
+            self.base_pointer = self.pop()
+        ret_address = self.pop()
+        self.jump(ret_address)
         if value is not None:
             self.return_value = value
 
     # For some reasons we get int3 some times
-    def gdb_call(self, function: str, args: list, *, cast = "long"):
+    def gdb_call(self, function: str, args: list, *, cast = "long", inferior=None):
         if not self.elf.statically_linked:
+            if inferior is None:
+                inferior = self.current_inferior
+            old_inferior = self.switch_inferior(inferior.num)
             try:
                 ans = self.execute(f"call ({cast}) {function} ({', '.join([hex(arg) for arg in args])})")
                 if cast == "void":
-                    return None
+                    ret = None
                 ans = ans.split()[-1]
                 # GEF prints logs as base 16, but pwndbg as base 10
-                return int(ans, 16) if "0x" in ans else int(ans)
+                ret = int(ans, 16) if "0x" in ans else int(ans)
             except Exception: #gdb.error: The program being debugged was signalled while in a function called from GDB.
                 log.debug(f"gdb got int3 executing {function}. Retrying...")
                 self.finish()
                 # For some reason I just get 0x0
                 #return self.return_value()
-                return self.gdb_call(function, args) # Should work this time
-        
+                ret = self.gdb_call(function, args) # Should work this time
+            self.switch_inferior(old_inferior)
         elif function in self.symbols:
-            return self.call(self.symbols[function], args)
+            ret = self.call(self.symbols[function], args, inferior=inferior)
             
         else:
             raise Exception(f"I don't know how to handle this function! {function} not in symbols")
 
+        return ret
+
     def __convert_args(self, args, heap = True):
         """
         Save any string present in the args and return a pointer to it instead
         """
         parsed_args, to_free = [], []
         
         for arg in args:
@@ -820,52 +1089,65 @@
                 self.write(pointer, arg + b"\x00")
                 arg = pointer
 
             parsed_args.append(arg)
 
         return parsed_args, to_free
 
-    def __continue_call(self, backup, to_free, heap, end_pointer, return_value):
-        if end_pointer is None:
-            self.finish() # Finish can only work if the stack-frame isn't broken
+    def __continue_call(self, backup, to_free, heap, end_pointer, return_value, alignement):
+        #if end_pointer == self.instruction_pointer: # We called the function while on the first instruction, let's just step and continue normaly [21/05/23] Wait, why bother ?
+        self.continue_until(end_pointer)
+        while unpack(self.read(self.stack_pointer - context.bytes, context.bytes)) != end_pointer:
+            assert self.instruction_pointer == end_pointer, "Something strange happened in a call"
+            log.warn_once("Are you sure you called the function from outside ?")
+            self.continue_until(end_pointer)
+
+        if DEBUG:
             log.debug("call finished")
                 
-        else:
-            self.c(until=end_pointer)
-            # Exit the function
-            self.step()
-        
         res = self.return_value
+        for _ in range(alignement):
+            self.pop()
         self.restore_backup(backup)
         for pointer, n in to_free[::-1]: #I do it backward to have a coherent behaviour with heap=False, but I still don't really know if I should implement a free in that case
             self.dealloc(pointer, len=n, heap=heap)
         return_value.put(res) # will be the event that tells me I finished
 
     # I still need end_pointer even if I would like to put the breakpoint on the address from which we call the function because I can't be sure that someone won't want to call a function from inside 
-    def call(self, function: [int, str], args: list = [], *, end_pointer=None, heap=True, wait = True):
+    # Wait, finish is doing it anyway... So let's require that call isn't used while you are inside the function, but still handle it just in case. Like a check that *(rsp - bytes) -> rip. It's not perfect, but it should at least always be true if we used the function properly [21/05/23]
+    def call(self, function: [int, str], args: list = [], *, heap=True, wait = True):
         """
         Call any function in the binary with the parameters you want
 
         Parameters
         ----------
         function : [str, int]
             Pointer to the function to call
         args : list[int | str | bytes]
             List of parameters to pass to the function
             All strings passed this way will be saved in the binary with a null terminator
             Byte arrays will be saved as they are
         end_pointer : int, optional
-            The function will run with a 'finish' command. If for some reason you know that it won't work this way you can set an instruction to stop at. (I currently expect it to be a ret and will step on it to leave)
+            The function will run with a 'finish' command. If you aren't calling a standard function use this parameter. (I currently expect it to be a ret and will step on it to leave)
         heap : bool, optional
             Byte arrays and strings passed to the functions are by default saved on the heap with a malloc(). If you can't set this to False to save them on the bss (WARNING I can't guaranty I won't overwrite data this way)
+        
+        Return:
+        return_value: [int, Queue]
+        if wait = True the functions return the content of rax, othewise the queue where it will be put once the function finishes
         """
         self.restore_arch()
         
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+
         address = self.parse_address(function)
-        
+        if DEBUG:
+            log.debug(f"calling {self.reverse_lookup(address)}")
+
         args, to_free  = self.__convert_args(args, heap)
 
         #save registers 
         backup = self.backup()    
         
         if context.bits == 64:
             calling_convention = ["rdi", "rsi", "rdx", "rcx", "r8", "r9"]
@@ -875,21 +1157,25 @@
                 log.debug("%s setted to %s", register, args[0])
                 setattr(self, register, args.pop(0))
             
         #Should I offset the stack pointer to preserve the stack frame ? No, right ?
         for arg in args:
             self.push(arg)
         
-        # May be useful later
         return_address = self.instruction_pointer
+        
+        # Libc functions may die otherwise
+        alignement = 0
+        while self.stack_pointer % 0x10 != 0x0:
+            self.push(0)
         self.push(return_address)
         self.jump(address)
 
         return_value = Queue()
-        context.Thread(target=self.__continue_call, args=(backup, to_free, heap, end_pointer, return_value)).start()
+        context.Thread(target=self.__continue_call, args=(backup, to_free, heap, return_address, return_value, alignement)).start()
         if wait:
             return return_value.get()
         else:
             log.warn_once("you decided not to wait for the call to finish. I return a queue to the return value of the function. When you need it use .get() to wait for the call to finish")
             return return_value
 
     # Can be used with signal code or name. Case insensitive.
@@ -990,14 +1276,53 @@
             raise f"parse_breakpoint is asking what is the type of {location}"
         
         return address
 
     # Legacy
     parse_for_breakpoint = parse_address
 
+    def reverse_lookup(self, address: [int, str]) -> str:
+        if type(address) is str:
+            return address
+        elif type(address) is int:
+            if address in self.symbols.values():
+                function = list(self.symbols.keys())[list(self.symbols.values()).index(address)]
+                return f"{function}({hex(address)})"
+            else:
+                return hex(address)
+        else:
+            ...
+
+
+
+    def __breakpoint_gdb(self, address, legacy_callback=None):
+        # Still needed for hidden breakpoint with return False when you want to also use gdb manually [17/04/23]
+        if legacy_callback is not None:
+            log.warn_once("if your callbacks crash you may not notice it and you have to scroll a bit to find the error messages hidden in the gdb terminal")
+            # I don't know yet how to handle the conn if I don't go through self.gdb.Breakpoint so I create the class here :(
+            class MyBreakpoint(self.gdb.Breakpoint):
+                def __init__(_self, address):
+                    super().__init__(address)
+                    _self.callback = legacy_callback
+                # WARNING IF A TEMPORARY BREAKPOINT DOESN'T STOP IT WON'T COUNT AS HIT AND STAY ACTIVE. May cause problems with the callback if you pass multiple times [26/02/23]
+                def stop(_self, *args):
+                    _break = _self.callback(self) 
+                    if _break is None:
+                        return True
+                    return _break
+            res = MyBreakpoint(f"*{hex(address)}")
+
+        else:
+            res = self.gdb.Breakpoint(f"*{hex(address)}")
+        
+        return res
+
+    def __breakpoint_libdebug(self, address):
+        return self.libdebug.breakpoint(address)
+
     # May want to put breakpoints relative to the libc too?
     # I want to keep legacy breakpoints for the ones I set with the library because we must be able to work manually when emulating ptrace [23/03/23]
     # legacy_callback will be deprecated once I can overwrite gdb's nexti to keep his breakpoint even if the process gets interrupted [27/04/23]
     def b(self, location: [int, str], callback=None, legacy_callback=None, temporary=False):
         """
         Set a breakpoint in your process.
 
@@ -1024,79 +1349,112 @@
         # real_callbacks have problems, but with features not even available with simple callbacks. Furthermore now you can use return False with temporary breakpoints
         if not self.debugging:
             log.warn_once(DEBUG_OFF)
             return
 
         address = self.parse_address(location)
 
-        log.debug(f"putting breakpoint in {hex(address)}")
+        log.debug(f"putting breakpoint in {self.reverse_lookup(address)}")
         
-        # Still needed for hidden breakpoint with return False when you want to also use gdb manually [17/04/23]
-        if legacy_callback is not None:
-            log.warn_once("if your callbacks crash you may not notice it and you have to scroll a bit to find the error messages hidden in the gdb terminal")
-            # I don't know yet how to handle the conn if I don't go through self.gdb.Breakpoint so I create the class here :(
-            class MyBreakpoint(self.gdb.Breakpoint):
-                def __init__(_self, address, callback):
-                    super().__init__(address)
-                    _self.callback = legacy_callback
-                # WARNING IF A TEMPORARY BREAKPOINT DOESN'T STOP IT WON'T COUNT AS HIT AND STAY ACTIVE. May cause problems with the callback if you pass multiple times [26/02/23]
-                def stop(_self, *args):
-                    _break = _self.callback(self) 
-                    if _break is None:
-                        return True
-                    return _break
-            res = MyBreakpoint(f"*{hex(address)}", callback)
-
+        if self.gdb is not None:
+            breakpoint = Breakpoint(self.__breakpoint_gdb(address, legacy_callback).server_breakpoint, callback, temporary)
+        elif self.libdebug is not None:
+            if legacy_callback is not None:
+                callback = legacy_callback
+            breakpoint = Breakpoint(self.__breakpoint_libdebug(address), callback, temporary)
         else:
-            res = self.gdb.Breakpoint(f"*{hex(address)}")
-        
-        self.breakpoints[address] = Breakpoint(res.server_breakpoint, callback, temporary)
-        return res
+            ...
+
+        self.breakpoints[address] = breakpoint
+        return breakpoint
         
     breakpoint = b
 
     def delete_breakpoint(self, location: [int, str]) -> bool:
+        if not self.debugging:
+            log.warn_once(DEBUG_OFF)
+            return
+
         address = self.parse_address(location)
         # Is there a case where it isn't ?? [17/04/23]
         if address in self.breakpoints:
-            self.breakpoints.pop(address).gdb_breakpoint.delete() # Remove from dict and delete from gdb
+            if self.gdb is not None:
+                self.breakpoints.pop(address).gdb_breakpoint.delete() # Remove from dict and delete from gdb
+            elif self.libdebug is not None:
+                self.libdebug.del_bp(self.breakpoints.pop(address).gdb_breakpoint)
+            else:
+                ...
 
     ########################## MEMORY ACCESS ##########################
+    # needed for aarch64. Don't ask why...
+    def __read_gdb(self, address: int, size: int, *, inferior = None) -> bytes:
 
-    def read(self, address: int, size: int, *, inferior = None) -> bytes:
-
+        # clear the convention for inferiors
         if inferior == None:
             inferior = self._inferior
 
         log.debug(f"reading from inferior {inferior}")
-        return self.inferiors[inferior].read_memory(address, size).tobytes()
+        if type(inferior) is int:
+            num = inferior
+        else:
+            num = inferior.num
+        return self.inferiors[num].read_memory(address, size).tobytes()
+
+    def read(self, address: int, size: int, *, inferior = None, pid = None) -> bytes:
+        if self.gdb is not None:
+            return self.__read_gdb(address, size, inferior=inferior)
+
+        if inferior is not None:
+            pid = inferior.pid
+        if pid is None:
+            pid = self.pid
+
+        with open(f"/proc/{pid}/mem", "r+b") as fd:
+            fd.seek(address)
+            return fd.read(size)
 
-    def write(self, address: int, byte_array: bytes, *, inferior = None):
+    def __write_gdb(self, address: int, byte_array: bytes, *, inferior = None):
 
         if inferior == None:
             inferior = self._inferior
         
         inferior = self.inferiors[inferior]
         log.debug(f"writing {byte_array} in {inferior} at address {hex(address)}")
         # BUG: GDB writes in the wrong inferior...
         #inferior.write_memory(address, byte_array)
         fd = os.open(f"/proc/{inferior.pid}/mem", os.O_RDWR)
         os.lseek(fd, address, os.SEEK_SET)
         os.write(fd, byte_array)
         os.close(fd)
 
+    # How to handle multiple processes ?
+    def __write_libdebug(self, address: int, byte_array: bytes, *, pid = None):
+        if pid is not None:
+            ...
+
+    def write(self, address: int, byte_array: bytes, *, inferior = None, pid = None):
+        if inferior is not None:
+            pid = inferior.pid
+        if pid is None:
+            pid = self.pid
+
+        log.debug(f"writing {byte_array.hex()} at {hex(address)}")
+        with open(f"/proc/{pid}/mem", "r+b") as fd:
+            fd.seek(address)
+            fd.write(byte_array)
+
     def push(self, value: int):
         """
         push value (must be uint) on the stack
         """
         if not self.debugging:
             log.warn_once(DEBUG_OFF)
             return
 
-        log.debug(f"pushing {pack(value)}")
+        log.debug(f"pushing {hex(value)}")
         self.stack_pointer -= context.bytes
         self.write(self.stack_pointer, pack(value))
 
     def pop(self) -> int:
         """
         pop value (uint) from the stack
         """
@@ -1130,45 +1488,39 @@
             Set to False if you can't use the heap
             This way it will return a pointer to an area of the bss
         Returns
         -------
         pointer
         """
 
-        if inferior == None:
-            inferior = self._inferior
-        
         if heap:
-            old_inferior = self.switch_inferior(inferior)
-            
-            res = self.gdb_call("malloc", [n])
-
-            self.switch_inferior(old_inferior)
-
-            return res
-
+            if self.gdb is not None:
+                # Do we wan't to use call for both ? [10/05/23]
+                ret = self.gdb_call("malloc", [n], inferior=inferior)
+            elif self.libdebug is not None:
+                ret = self.call("malloc", [n])
+            else:
+                ...
         else:
             if self._free_bss is None:
                 self._free_bss = self.elf.bss() # I have to think about how to preserve eventual data already present
             self._free_bss += n
-            return self._free_bss
+            ret = self._free_bss
         
+        return ret
+
     def dealloc(self, pointer: int, len=0, heap=True, inferior = None):
         
-        if inferior == None:
-            inferior = self._inferior
-        
-        if heap:
-            
-            old_inferior = self.switch_inferior(inferior)
-
-            self.gdb_call("free", [pointer], cast="void")
-
-            self.switch_inferior(old_inferior)
-
+        if heap:    
+            if self.gdb is not None:
+                self.gdb_call("free", [pointer], cast="void", inferior=inferior)
+            elif self.libdebug is not None:
+                self.call("free", [pointer])
+            else:
+                ...
         else:
             # MMMMMMM, not perfect for different inferiors
             self._free_bss -= len
             #I know it's not perfect, but damn I don't want to implement a heap logic for the bss ahahah
             #Just use the heap if you can
 
     # I copied it from pwntools to have access to it even if I attach directly to a pid
@@ -1295,14 +1647,16 @@
     @property
     def special_registers(self):
         return ["eflags", "cs", "ss", "ds", "es", "fs", "gs"]
 
     # WARNING reset expects the last two registers to be sp and ip. backup expects the last register to be ip
     @property
     def registers(self):
+        if context.arch == "aarch64":
+            return [f"x{i}" for i in range(31)] + ["sp", "pc"]
         if context.bits == 32:
             return ["eax", "ebx", "ecx", "edx", "edi", "esi", "ebp", "esp", "eip"]
         elif context.bits == 64:
             return ["rax", "rbx", "rcx", "rdx", "rdi", "rsi", "r8", "r9", "r10", "r11", "r12", "r13", "r14", "r15", "rbp", "rsp", "rip"]
         else:
             log.critical("Bits not known")
 
@@ -1334,48 +1688,67 @@
         inst = next(self.disassemble(self.instruction_pointer, 16)) #15 bytes is the maximum size for an instruction in x64
         inst.toString = partial(lambda self: f"{self.mnemonic} {self.op_str}".strip(), inst)
         return inst
 
     # May be usefull for Inner_Debugger
     def disassemble(self, address, size):
         if self._capstone is None:
-            self._capstone = Cs(CS_ARCH_X86, context.bytes)
+            if context.arch == "aarch64":
+                self._capstone = Cs(CS_ARCH_ARM64, CS_MODE_ARM)
+            else:
+                self._capstone = Cs(CS_ARCH_X86, context.bytes)
         return self._capstone.disasm(self.read(address, size), address)
 
     ########################## Generic references ##########################
 
     @property
     def return_value(self):
+        if context.arch == "aarch64":
+            return self.X0
         if context.bits == 32:
             return self.eax
         else:
             return self.rax
 
     @return_value.setter
     def return_value(self, value):
+        if context.arch == "aarch64":
+            self.x0 = value
         if context.bits == 32:
             self.eax = value
         else:
             self.rax = value
 
     @property
     def stack_pointer(self):
+        if context.arch == "aarch64":
+            return self.sp
         if context.bits == 32:
             return self.esp
         else:
             return self.rsp
 
     # issue: setting $sp is not allowed when other stack frames are selected... https://sourceware.org/gdb/onlinedocs/gdb/Registers.html [04/03/23]
     @stack_pointer.setter
     def stack_pointer(self, value):
+        if context.arch == "aarch64":
+            self.sp = value
         # May move this line to push and pop if someone can argue a good reason to.
+        if context.bits == 32:
+            self.esp = value
+        else:
+            self.rsp = value
+
         while self.stack_pointer != value:
+            if self.gdb is not None:
+                raise Exception("Error setting stack pointer!")
             log.debug("forcing last frame")
             self.execute("select-frame 0") # I don't know what frames are for, but if you need to push or pop you just want to work on the current frame i guess ? [04/03/23]
-            
+            if context.arch == "aarch64":
+                self.sp = value
             if context.bits == 32:
                 self.esp = value
             else:
                 self.rsp = value
 
     @property
     def base_pointer(self):
@@ -1392,34 +1765,51 @@
             self.rbp = value
 
     # Prevent null pointers
     @property
     def instruction_pointer(self):
         ans = 0
         while ans == 0:
+            if context.arch == "aarch64":
+                ans = self.pc
             # what about self.gdb.newest_frame().pc() ? [28/04/23]
-            if context.bits == 32:
+            elif context.bits == 32:
                 ans = self.eip
             else:
                 ans = self.rip
             # log
             if ans == 0:
                 log.debug("null pointer in ip ! retrying...")
         return ans
 
     @instruction_pointer.setter
     def instruction_pointer(self, value):
-        if context.bits == 32:
+        if context.arch == "aarch64":
+            self.pc = value
+        elif context.bits == 32:
             self.eip = value
         else:
             self.rip = value
 
     @property
     def __saved_ip(self):
-        return self.gdb.newest_frame().older().pc()
+        if self.gdb is not None:
+            return self.gdb.newest_frame().older().pc()
+
+        elif self.libdebug is not None:
+            self.restore_arch()
+            # experimental, but should be better that the native one for libdebug        
+            if self.next_inst.toString() in ["endbr64", "push rbp", "push ebp"]:
+                return_pointer = self.read(self.stack_pointer, context.bytes)
+            elif self.next_inst.toString() in ["mov rbp, rsp", "mov ebp, esp"]:
+                return_pointer = self.read(self.stack_pointer + context.bytes, context.bytes) # Remove the base pointer # No need to place it back in rbp
+            else:
+                return_pointer = self.read(self.base_pointer + context.bytes, context.bytes)
+
+            return unpack(return_pointer)        
 
         ## rip = 0x7ffff7fe45b8 in _dl_start_final (./elf/rtld.c:507); saved rip = 0x7ffff7fe32b8
         #data = self.execute("info frame 0").split("\n")
         #print(data)
         #for line in data:
         #    if " saved " in line and "ip = " in line:
         #        ip = line.split("saved ")[-1].split("= ")[-1]
@@ -1449,22 +1839,25 @@
                     raise Exception(f"How am I expected to find which child you whant ??")
 
         log.debug(f"splitting inferior {inferior}")
         n = inferior.num
         pid = inferior.pid
         old_n = self.switch_inferior(n)
         ip = self.instruction_pointer
-        backup = self.inject_sleep(ip, inferior.num)
+        backup = self.inject_sleep(ip, inferior)
 
-        # For some reason it may happend that we receive a SIGINT on the first step. This would kill the process if I detached now [29/04/23] (Always that same bug)
-        self.step() 
+        # Now it should be handled by the interrupt in set_split_on_fork [22/05/23]
+        ## For some reason it may happend that we receive a SIGINT on the first step. This would kill the process if I detached now [29/04/23] (Always that same bug)
+        #self.step() 
         
         self.switch_inferior(old_n)
         log.debug("detaching from child")
         self.execute(f"detach inferiors {n}")
+        # Do we include self.gdbscript ? [08/05/23]
+        # Warn to use it only to setup the debugger in general ? No commands because they will be runned by all childs
         child = Debugger(pid, binary=self.elf.path)
         log.debug("new debugger opened")
         child.write(ip, backup)
         log.debug("shellcode patched")
         child.jump(ip)
         return child  
     
@@ -1494,22 +1887,34 @@
 
             # The interrupt may give me problems with continue_until
             def fork_handler(event):
                 inferior = event.inferior
                 pid = inferior.pid        
                 #self.to_split.put(pid)
                 def split(inferior):
+                    self.restore_arch()
+                    
                     log.info(f"splitting child: {inferior.pid}")
                     stopped = False
                     if self.running:
                         self.interrupt()
                         # How to handle the case where we interrupt at the address of a temporary breakpoint ? [05/05/23]
                         #if self.instruction_pointer not in self.breakpoints and self.instruction_pointer != self.last_breakpoint_deleted:
-                        if self._stop_reason != "BREAKPOINT":
+                        if "BREAKPOINT" not in self._stop_reason:
+                            if DEBUG:
+                                log.debug(f"stopped with {self._stop_reason}")
                             stopped = True
+                        else:
+                            if DEBUG:
+                                log.debug("I tried interrupting, but we where already on a breakpoint, so I won't continue later")
+                            address = self.instruction_pointer
+                            with context.silent:
+                                self.step(repeat=2)
+                            if address != self.instruction_pointer:
+                                log.warn("I made a mistake and stepped thinking we would catch an interrupt. I hope this won't be a problem")
                     self.children[pid] = self.split_child(inferior=inferior)
                     # Should not continue if I reached the breakpoint before the split
                     if not interrupt and stopped:
                         self.execute("c")
                         # What is the difference ? [05/O5/23 20:30]
                         #self.priority -= 1 # Can i do it this way to keep the priority correct ? [05/05/23 20:00]
                         #self.cont(wait=False)
@@ -1518,50 +1923,14 @@
                 ## Non puoi eseguire azioni dentro ad un handler degli eventi quindi lancio in un thread a parte
                 context.Thread(target=split, args = (inferior,)).start()
 
             self.gdb.events.new_inferior.connect(fork_handler)
             
             return self
 
-    # Taken from GEF to handle slave interuption
-    @property
-    def _stop_reason(self) -> str:
-        res = self.gdb.execute("info program", to_string=True).splitlines()
-        if not res:
-            return "NOT RUNNING"
-
-        for line in res:
-            line = line.strip()
-            if line.startswith("It stopped with signal "):
-                return line.replace("It stopped with signal ", "").split(",", 1)[0]
-            if line == "The program being debugged is not being run.":
-                return "NOT RUNNING"
-            if line == "It stopped at a breakpoint that has since been deleted.":
-                return "TEMPORARY BREAKPOINT"
-            if line.startswith("It stopped at breakpoint "):
-                return "BREAKPOINT"
-            if line == "It stopped after being stepped.":
-                return "SINGLE STEP"
-
-        return "STOPPED"
-
-    @property
-    def _details_breakpoint_stopped(self) -> str:
-        """
-        If the program stopped at a breakpoint, return the id of that breakpoint
-        This can be used to identify caught syscall
-        """
-        for line in res:
-            line = line.strip()
-            #It stopped at breakpoint 2.
-            if line.startswith("It stopped at breakpoint "):
-                return line.split(".")[0][len("It stopped at breakpoint "):]
-        else:
-            log.warn("process didn't stop for a breakpoint")
-
     # Non dovrebbe gestire gli int3 piuttosto ? Un set event if not in breakpoints execute code ? [06/03/23]
     # Boh, tanto si ferma e basta... 
     # Però si, dovrebbe dirlo al master
     # Il problema è che spesso si ferma prima di sapere chi sia il master
     # Maybe add a callback for SIGSTOP... [25/03/23]
     # TODO set in __stop_handler an action to sent to the master why we stopped [27/04/23]
     def emulate_ptrace_slave(self, master = None, *, off = False, wait_fun="waitpid"):
@@ -1584,15 +1953,15 @@
             # set breakpoint
             # You can not wait inside the breakpoint otherwise gdb gets blocked before the child can be split away 
             def callback(dbg):
                 log.debug("slave waiting for instructions")
 
                 # Do it for int3 instead
                 #if dbg.master is not None:
-                #    dbg.master.slave_has_stopped.set()
+                #    dbg.master.slave_has_stopped.set() 
 
                 def thread(dbg):
                     log.critical("slave thread stopped")
                     dbg.wait_master()
                     dbg.__clear_stop("thread slave")
                     log.critical("slave thread can continue")
                     #log.debug("I won't run dbg.c(), see if you still get the breakpoint hit twice")
@@ -1700,16 +2069,18 @@
             dbg.return_value = dbg.args[0] #slave.pid # Not really, but just != 0
             status_pointer = dbg.args[1]
             # Should be set in relation to the slave... But for now rip
             wait_signal = self._wait_signal if self._wait_signal is not None else 0x13
             self._wait_signal = None
             dbg.write(status_pointer, p32(wait_signal * 0x100 + 0x7f)) # Random status that currently works. For sigabort it is \x13\x7f \x13 is SIGSTOP \x7f means that the process has stopped
             if stop_at_waitpid:
+                log.info(f"parent is waiting for the child [{dbg.args[0]}]. Continue once you are ready.")
                 return True
             else:
+                log.debug("we hit waitpid")
                 return False
 
         self.b(self.symbols[wait_fun], legacy_callback = callback_wait)
 
         return self
 
     ########################## PTRACE EMULATION ##########################
@@ -1848,26 +2219,21 @@
         size = 0x1000 * ((1 + (address + len(shellcode)) // 0x1000) - address // 0x1000)
         #if not self.elf.statically_linked:
         #    ans = self.execute(f"call (long) mprotect({hex(address)}, {hex(size)}, 7)")
         #else:
         if "mprotect" in self.symbols:
             # I can use gdb call, but there are problems if the symbols are "fake" so put a check elf.staticaly_linked if you want to do it [04/03/23]
             ans = self.call(self.symbols["mprotect"], [address & 0xfffffffffffff000, size, constants.PROT_EXEC | constants.PROT_READ | constants.PROT_WRITE])
-        # I don't want the libc syscall, but a simple \x0f\x05\xc3
-        elif "_syscall" in self.symbols:
-            # Context.arch handles constants.SYS ! I love pwntools <3
+        if DEBUG:
             log.debug("calling sys_mprotect. Should be 0xa on 64bit arch")
             log .debug(f"{context.arch=}")
-            self.restore_arch()
+        self.restore_arch()
+        if DEBUG:
             log .debug(f"{context.arch=}")
-            ans = self.syscall(constants.SYS_mprotect.real, [address & 0xfffffffffffff000, size, constants.PROT_EXEC | constants.PROT_READ | constants.PROT_WRITE])
-        else:
-            log.critical("please, I at least need an address to a syscall ; ret gadget in symbols[\"_syscall\"]")
-            
-        # parse ans == 0 ?
+        ans = self.syscall(constants.SYS_mprotect.real, [address & 0xfffffffffffff000, size, constants.PROT_EXEC | constants.PROT_READ | constants.PROT_WRITE])
         
         self.switch_inferior(old_inferior)
 
         return address
 
     def inject_sleep(self, address, inferior=None):
         """
@@ -1905,27 +2271,43 @@
 
     ########################### Heresies ##########################
     
     def __getattr__(self, name):
     #    log.debug(f"looking for attr {name}")
     #    #getattr is only called when an attribute is NOT found in the instance's dictionary
     #    #I may wan't to use this instead of the 300 lines of registers, but have to check how to handle the setter
-        if name in ["p", "elf", "gdb"]: #If __getattr__ is called with p it means I haven't finished initializing the class so I shouldn't call self.registers in __setattr__
+        if name in ["p", "elf"]: #If __getattr__ is called with p it means I haven't finished initializing the class so I shouldn't call self.registers in __setattr__
             return False
+        if name in ["gdb", "libdebug"]:
+            return None
         if name in self.special_registers + self.registers + self.minor_registers:
-            res = int(self.gdb.parse_and_eval(f"${name}")) % 2**context.bits
+            if self.gdb is not None:
+                try:
+                    res = int(self.gdb.parse_and_eval(f"${name}")) % 2**context.bits
+                except:
+                    log.warn("error reading register. Retrying...")
+                    res = int(self.gdb.parse_and_eval(f"${name}")) % 2**context.bits
+            elif self.libdebug is not None:
+                res = getattr(self.libdebug, name)
             return res
         elif self.p and hasattr(self.p, name):
             return getattr(self.p, name)
         # May want to also expose in case you want to access something like inferiors() 
-        elif self.gdb and hasattr(self.gdb, name):
+        elif self.gdb is not None and hasattr(self.gdb, name):
             return getattr(self.gdb, name)
+        elif self.libdebug is not None and hasattr(self.libdebug, name):
+            return getattr(self.libdebug, name)
         else:
             # Get better errors when can't resolve properties
             self.__getattribute__(name)
 
     def __setattr__(self, name, value):
         if self.elf and name in self.special_registers + self.registers + self.minor_registers:
             self.restore_arch()
-            self.execute(f"set ${name.lower()} = {value % 2**context.bits}")
+            if self.gdb is not None:
+                self.execute(f"set ${name.lower()} = {value % 2**context.bits}")
+            elif self.libdebug is not None:
+                setattr(self.libdebug, name, value)
+            else:
+                ...
         else:
             super().__setattr__(name, value)
```

### Comparing `gdb_plus-6.2.0/gdb_plus/utils.py` & `gdb_plus-6.3.0/gdb_plus/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,16 @@
                 log.debug(f"priority {priority} met for {self.pid}")
                 self.priority -= 1
                 if self.priority < 0:
                     log.warn(f"I think there is something wrong with the wait! We reached priority {self.priority}")
                 break
             # If I call wait again while the event is set it won't block ! [04/04/23]
             self.cleared.wait()
+            # I forgot to clear it somewhere... [22/05/23]
+            self.cleared.clear()
 
     
     def clear(self):
         #self.secret.clear()
         if self.is_set():
             super().clear()
             self.cleared.set()
```

### Comparing `gdb_plus-6.2.0/gdb_plus.egg-info/PKG-INFO` & `gdb_plus-6.3.0/gdb_plus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb-plus
-Version: 6.2.0
+Version: 6.3.0
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
@@ -34,15 +34,15 @@
 ```
 or dev branch
 ```
 pip3 install git+https://github.com/Angelo942/gdb_plus.git@dev
 ```
 
 **Warning for pwndbg users:**  
-Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork.
+Previous bugs in Pwndbg used to break the api for python. While most of GDB+ should work with the current version of pwndbg [19/12/2022], pwndbg can not debug both processes after a fork, making it almost impossible to use features such as the emulation of ptrace.   
 you are strongly advised to use [GEF](https://github.com/hugsy/gef) instead.
 
 ## Debugging
 
 You can debug a program using the path to the binary.   
 If you really have to you can also use a process or even just his pid. 
 For pwn challenges set the remote address with `Debugger().remote(<host>, <port>)` and use the argument `REMOTE` once you want to exploit the server
@@ -112,15 +112,15 @@
 dbg.p.sendline(b"4")
 done.wait()
 # Here the script will wait until you reach the offset 0x43 from main while gdb will break at offset 0x12 and 0x23 to let you look at the process
 ...
 ```
 
 **Warning**  
-* `finish` can only work if the stack frame hasn't been corrupted
+* `finish` can only work if the stack frame hasn't been corrupted. With libdebug it will fail if the function doesn't use the base pointer.
 * Try avoiding `interrupt` as much as possible. 
 * You may be tempted to do `dbg.instruction_pointer = dbg.parse_address(location)`, but a bug in gdb may cause an unexpected behaviour if you do so. Use `dbg.jump(location)` instead
 
 If the function modifies itself you may find yourself unable to set breakpoints where you want. To analyse these function we can run them step by step
 
 ```py
 def MyCallback(dbg):
@@ -269,19 +269,41 @@
 
 **Note**  
 You can pass parameters as strings or byte_arrays. By default they will be saved on the heap with a null terminator in the case of a string. If you can't use the heap set `heap=False`
 
 **Warning**  
 If the stack frame has been corrupted finish() may not work. If this is the case set last address of your function in `call(..., end_pointer= ...)`.
 
-## Alternatives
-from version 6.0 gdb_plus should be able to script anything you can imagine, but you it can be slow as hell for some uses. This tool is meant to help debugging during challenges, if you only want to automate exploit development you may prefer something like [libdebug](https://github.com/JinBlack/libdebug) which doesn't has to communicate with gdb for each command.
+## Libdebug
+By default GDB+ uses a gdbserver to debug the process. This is verry usefull when you also have to check manually gdb while you are writing a script, but can be verry slow. For this reason we now support libdebug (from version >= 0.4) as an alternative debugger. It is lacking a lot of features but can do the job for most tasks and it can be 50 times faster. 
+
+The debugger will always start with dbg, but you can switch back and forth
+
+```py
+dbg = Debugger(<binary>)
+# switch to libdebug
+dbg.migrate(libdebug=True)
+# switch to gdb
+dbg.migrate(gdb=True)
+```
+
+To access properties of libdebug that haven't been wrapped you can simply use `dbg.libdebug` as you would with `dbg.gdb`.
+
+When you switch the breakpoints and callbacks will be preserved except for those needed to emulate ptrace. Please migrate to libdebug before setting the emulator up or disable it and set it up again right after.
+
+Since libdebug isn't on PyPI yet we could't include it in the dependencies. 
+You can install it manually:
+`pip3 install git+https://github.com/Angelo942/libdebug.git@parallel`
 
 # TODO
 
-* Add option to use libdebug instead of gdb
-* Migrate all wait=False to non blocking functions with events set when finished
 * Identify actions performed manually in gdb (overwrite finish and ni)
 * Handle fork and ptrace from syscall instead of libc
 * Improve ptrace emulation
     * register waitpid return value
-* Maybe nop split_on_fork&co while debugging is False
+* Stack multiple callbacks on the same breakpoint
+* handle Hardware breakpoint
+* support ARM binaries
+* support multithread applications
+* setup gdbinit for forked processes
+* catch sigsegv as an exit instead of user interaction
+* enable signal() with libdebug
```

### Comparing `gdb_plus-6.2.0/pyproject.toml` & `gdb_plus-6.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,21 @@
     "setuptools",
     "wheel",
 ]
 
 [project]
 name = "gdb_plus"
 description = "Python library to automate gdb debugging"
-version = "6.2.0"
+version = "6.3.0"
 authors = [{name = "Edoardo"}]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "pwntools>=4.5.0",
-    "capstone"
+    "capstone",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: Unix",
 ]
```

### Comparing `gdb_plus-6.2.0/tests/test.py` & `gdb_plus-6.3.0/tests/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import warnings
 
 gdbinit = """
 handle SIGALRM nopass
 source ~/.gdbinit-gef.py
 """
 
-@unittest.skip
+#@unittest.skip
 class Debugger_process(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		self.debuggers = []
 
 	def tearDown(self):
 		for dbg in self.debuggers:
@@ -98,47 +98,48 @@
 	#@unittest.skip
 	def test_nonblocking_debug_from(self):
 		print("\ntest_nonblocking_debug_from: ", end="")
 
 		with context.local(arch="i386", bits=32):
 			interaction_finished = Event()
 			dbg = Debugger("./start", aslr=False).debug_from(0x804809d, event=interaction_finished, timeout=0.01)
+			self.debuggers.append(dbg)
 			dbg.p.sendline(b"ciao")
 			interaction_finished.set()
 			dbg.debug_from_done.wait()
 			self.assertEqual(dbg.eip, 0x804809d)
 
-@unittest.skip
+#@unittest.skip
 class Debugger_actions(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		with context.local(arch="amd64", bits=64):
 			self.dbg = Debugger("./insaaaaaaane")
 
 	def tearDown(self):
 		self.dbg.close()
 
 	# Fail, ho fatto next a mano e ho perso il controllo
-	#@unittest.skip
+	@unittest.skip
 	def test_continue_until(self):
 		print("\ntest_continue_until: ", end="")
 		self.dbg.b(0x403ad7, temporary=True)
 		print("\nPlay with gdb once we hit address 0x403ad7 and then send continue")
 		self.dbg.c(until=0x403adb)
 		self.assertEqual(self.dbg.instruction_pointer, 0x403adb)
 
 	#@unittest.skip
 	def test_nonblocking_continue_until(self):
 		print("\ntest_nonblocking_continue_until: ", end="")
 		done = self.dbg.continue_until(0x4038c2, wait=False)
-		self.p.sendline(b"ciao")
+		self.dbg.p.sendline(b"ciao")
 		done.wait()
 		self.assertEqual(self.dbg.instruction_pointer, 0x4038c2)
 
-@unittest.skip
+#@unittest.skip
 class Debugger_callbacks(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		self.dbg = Debugger("./insaaaaaaane")
 
 	def tearDown(self):
 		self.dbg.close()
@@ -165,17 +166,14 @@
 		print("\ntest_no_stop: ", end="")
 		def callback(dbg):
 			dbg.b(0x403ad9, temporary=True)
 			return False
 
 		self.dbg.b(0x403ad0, callback=callback, temporary=True)
 		
-		# NOOOOOO don't put a breakpoint !
-		#self.dbg.b(0x403ad9, temporary=True)
-
 		self.dbg.c(wait=True)
 		#self.dbg.interactive()
 		self.assertEqual(self.dbg.rip, 0x403ad9)
 		self.assertFalse(len(self.dbg.breakpoints))
 
 	#@unittest.skip
 	def test_step(self):
@@ -188,44 +186,48 @@
 		self.dbg.b(0x403ad0, callback=callback, temporary=True)
 		self.dbg.c(wait=True)
 		self.assertEqual(self.dbg.rip, 0x403ad2)
 
 	# Ricordati di testare anche finish con callback
 
 
-@unittest.skip
+#@unittest.skip
 class Debugger_memory(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		self.dbg = Debugger("./cube")
 
 	def tearDown(self):
 		if hasattr(self, "dbg"):
 			self.dbg.close()
 		pass
 
+	#@unittest.skip
 	def test_register_access(self):
 		print("\ntest_register_access: ", end="")
 		self.dbg.rax = 0xdeadbeefdeadbeef
 		self.dbg.eax = 0xfafafafa
 		self.dbg.ax  = 0xbabe
 		self.dbg.ah = 0x90
 		self.assertEqual(self.dbg.rax, 0xdeadbeeffafa90be)
 		self.dbg.r11 = 0x134343432342
 		self.assertEqual(self.dbg.r11, 0x134343432342)
 
+	#@unittest.skip
 	def test_special_registers(self):
 		print("\ntest_special_registers: ", end="")
 		self.assertEqual(self.dbg.return_value, self.dbg.rax)
 		self.assertEqual(self.dbg.stack_pointer, self.dbg.rsp)
 		self.assertEqual(self.dbg.instruction_pointer, self.dbg.rip)
 
 	# TODO: Test it with multiple inferiors if possible
+	#@unittest.skip
 	def test_alloc(self):
 		print("\ntest_alloc: ", end="")
+		self.dbg.close()
 		self.dbg = Debugger("./cube", aslr=False, from_start=False) # Wait for the libc to be loaded
 		pointer = self.dbg.alloc(16)
 		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
 		self.assertTrue(hex(pointer) in self.dbg.execute("heap chunks")) # WARNING THIS ONLY WORKS WITH GEF
 		self.dbg.dealloc(pointer)
 		pointer = self.dbg.alloc(16, heap=False)
 		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
@@ -252,15 +254,15 @@
 		request.append(b"authorization: Basic " + auth) 
 		if keepAlive:
 			request.append(b"Connection: keep-alive")
 		else:
 			request.append(b"Connection: close")
 		return LINE_TERMINATOR.join(request + [b""])
 
-	@unittest.skip
+	#@unittest.skip
 	def test_continuous_follow(self):
 		print("\ntest_continuous_follow: ", end="")
 		gdbscript = """
 		set detach-on-fork off
 		set follow-fork-mode child
 		"""
 		self.dbg = Debugger("./httpd", aslr=False, script=gdbscript)
@@ -274,15 +276,15 @@
 		self.dbg.execute("inferior 1") # We can't go back while the child is running
 		self.dbg.c(wait=False)
 		self.dbg.p.sendline(self.http_request(keepAlive=True))
 		self.dbg.wait()
 		self.assertEqual(self.dbg.rip, 0x5555555566d5)
 		self.dbg.close()
 	
-	@unittest.skip
+	#@unittest.skip
 	def test_split(self):
 		print("\ntest_split: ", end="")
 		with context.local(arch = "amd64", bits = 64):
 			CALL_TO_B64DECODE = 0x26d5
 			gdbscript = """
 			set detach-on-fork off
 			continue
@@ -290,29 +292,26 @@
 			dbg = Debugger("./httpd", aslr=False, script=gdbscript)
 			sleep(1) # wait for the child to spwn. The parrent will continue while the child is stopped at fork
 			dbg.interrupt()
 			dbg.b(CALL_TO_B64DECODE)
 			child = dbg.split_child(n=2)
 			dbg.p.sendline(self.http_request(keepAlive=True))
 			child.b(CALL_TO_B64DECODE)
-			#child.c()
-			#child.wait()
 			child.c(wait=True)
 			self.assertEqual(child.rip, 0x5555555566d5)
 			child.c()
+			child.detach()
 			dbg.execute("set follow-fork-mode child")
 			dbg.p.sendline(self.http_request(keepAlive=True))
-			#dbg.c(wait=False)
-			#dbg.wait()
 			dbg.c(wait=True)
 			self.assertEqual(dbg.rip, 0x5555555566d5)
 			dbg.close()
 			child.close()
 
-	@unittest.skip
+	#@unittest.skip
 	def test_my_split(self):
 		print("\ntest_my_split: ", end="")
 		with context.local(arch = 'amd64'):
 			dbg = Debugger("./traps_withSymbols", script="", aslr=False).set_split_on_fork(interrupt=True)
 			dbg.c(wait=False)
 			pid = dbg.wait_split() # and then for the child to split out
 			child = dbg.children[pid]
@@ -370,115 +369,55 @@
 				second_child.c(wait=True)
 			
 			self.assertTrue(b"YES !" in dbg.p.recv())
 
 			second_child.close()
 			dbg.close()
 
-@unittest.skip
+#@unittest.skip
 class Debugger_signals(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 		warnings.simplefilter("ignore", ImportWarning)
 		self.dbg = Debugger("./ExceptionalChecking_patched")
 
 	def tearDown(self):
 		if hasattr(self, "dbg"):
 			self.dbg.close()
 		pass
-
-	#Already present in test_signal_handler. Use it to debug the later if needed
-#	def test_step_until_ret(self):
-#		from queue import Queue
-#		HANDLER_RET = 0x04011ff
-#		CHECK_CALL = 0x0401341
-#		my_instruction_pointer = Queue()
-#		def callback_signal_handler(dbg):
-#			self.dbg.breakpoint(my_instruction_pointer.get(), temporary=True)
-#			return False
-#		self.dbg.breakpoint(HANDLER_RET, callback=callback_signal_handler)
-#		self.dbg.breakpoint(CHECK_CALL, temporary=True)
-#		self.dbg.cont()
-#		self.dbg.p.sendline(b"serial_a_caso")
-#		self.dbg.wait()
-#		self.dbg.step()
-#		self.dbg.next_signal = False
-#		output = []
-#		def callback(dbg):
-#			if self.dbg.next_signal:
-#				my_instruction_pointer.put(self.dbg.instruction_pointer)
-#				self.dbg.execute("signal SIGUSR1")
-#				self.dbg.wait()
-#				self.dbg.next_signal = False
-#			ni = self.dbg.next_inst
-#			if ni.mnemonic == "int3":
-#				self.dbg.next_signal = True
-#				self.dbg.write(self.dbg.instruction_pointer, b"\x90") #Just to avoid problems
-#			else:
-#				output.append(ni.toString())
-#		self.dbg.step_until_ret(callback)
-#		with open("dump_ExceptionalChecking") as fp:
-#			self.assertEqual(output, fp.read().split("\n"))
-
-#	def test_signal_handler(self):
-#		from queue import Queue
-#		HANDLER_RET = 0x04011ff
-#		CHECK_CALL = 0x0401341
-#		self.dbg.breakpoint(CHECK_CALL, temporary=True)
-#		self.dbg.cont()
-#		self.dbg.p.sendline(b"serial_a_caso")
-#		self.dbg.wait()
-#		self.dbg.step()
-#		self.dbg.next_signal = False
-#		output = []
-#		def callback(dbg):
-#			if self.dbg.next_signal:
-#				print("\ncall signal")
-#				self.dbg.signal("SIGUSR1", handler=HANDLER_RET)
-#				self.dbg.next_signal = False
-#			ni = self.dbg.next_inst
-#			if ni.mnemonic == "int3":
-#				print("\nint3")
-#				self.dbg.next_signal = True
-#				self.dbg.write(self.dbg.instruction_pointer, b"\x90") #Just to avoid problems
-#			else:
-#				output.append(ni.toString())
-#		self.dbg.step_until_ret(callback)
-#		with open("dump_ExceptionalChecking") as fp:
-#			self.assertEqual(output, fp.read().split("\n"))
-	
+		
 	# Commented out to not slow down too much the tests
 	#@unittest.skip
 	def test_signal_handler(self):
 		print("\ntest_signal_handler: ", end="")
 		from queue import Queue
 		HANDLER_RET = 0x04011ff
 		CHECK_CALL = 0x0401341
 		self.dbg.p.sendline(b"serial_a_caso")
 		self.dbg.cont(until=CHECK_CALL)
 		self.dbg.step()
 		self.dbg.next_signal = False
 		output = []
 		def callback(dbg):
 			if self.dbg.next_signal:
-				print("\ncall signal")
+				#print("\ncall signal")
 				self.dbg.signal("SIGUSR1", handler=HANDLER_RET)
 				self.dbg.next_signal = False
 			ni = self.dbg.next_inst
 			if ni.mnemonic == "int3":
-				print("\nint3")
+				#print("\nint3")
 				self.dbg.next_signal = True
 				self.dbg.write(self.dbg.instruction_pointer, b"\x90") #Just to avoid problems
 			else:
 				output.append(ni.toString())
 		self.dbg.step_until_ret(callback)
 		with open("dump_ExceptionalChecking") as fp:
 			self.assertEqual(output, fp.read().split("\n"))
 
-@unittest.skip
+#@unittest.skip
 class Debugger_calls(unittest.TestCase):
 	def setUp(self):
 		warnings.simplefilter("ignore", ResourceWarning)
 
 	def tearDown(self):
 		if hasattr(self, "dbg"):
 			self.dbg.close()
@@ -501,14 +440,15 @@
 		#print("\n\n".join(out)) 
 		with open("./dump_Cube") as fd:
 			self.assertEqual(out, fd.read().split("\n"))
 		self.dbg.close()
 
 	#@unittest.skip
 	def test_syscall_64bit(self):
+		print("\ntest_syscall: ", end="")
 		path = "./data.txt"
 		with context.local(arch="amd64", bits=64):
 			with open(path, "wb") as file:
 				file.write(b"")
 			self.dbg = Debugger("./insaaaaaaane", from_start=False) # You must wait for the libc to be loaded to call malloc
 			fd = self.dbg.syscall(constants.SYS_open, [path, constants.O_WRONLY, 0x0])
 			data = b"ciao, come stai ?"
@@ -542,13 +482,153 @@
 #		"""
 #		self.dbg = Debugger("./httpd", script=gdbinit, from_start=False)
 #		pointer = self.dbg.alloc(16)
 #		self.dbg.write(pointer, p64(0xdeadbeeffafa90be))
 #		self.dbg.close()
 
 @unittest.skip
-class Debugger_no_wait(unittest.TestCase):
-	pass	
+class Debugger_libdebug(unittest.TestCase):
+	def setUp(self):
+		warnings.simplefilter("ignore", ResourceWarning)
+
+	def tearDown(self):
+		self.dbg.close()
+
+	#@unittest.skip
+	def test_migrate(self):
+		print("\ntest_migrate: ", end="")
+		with context.local(arch="amd64", bits=64):
+			self.dbg = Debugger("./httpd", aslr=False)
+			self.dbg.migrate(libdebug=True)
+			self.assertEqual(self.dbg.instruction_pointer, 0x7ffff7fe32b0)
+			self.dbg.step()
+			self.assertEqual(self.dbg.instruction_pointer, 0x7ffff7fe32b3)
+			self.dbg.migrate(gdb=True)
+			self.assertEqual(self.dbg.instruction_pointer, 0x7ffff7fe32b3)
+			self.dbg.step()
+			self.assertEqual(self.dbg.instruction_pointer, 0x7ffff7fe4050)
+
+	#@unittest.skip
+	def test_continue_until(self):
+		print("\ntest_continue_until [libdebug]: ", end="")
+		with context.local(arch="amd64", bits=64):
+			self.dbg = Debugger("./httpd", aslr=False)
+			self.dbg.migrate(libdebug=True)
+			self.dbg.continue_until("main")
+			self.assertEqual(self.dbg.instruction_pointer, 0x55555555570c)
+
+	@unittest.skip
+	def test_call(self):
+		print("\ntest_call [libdebug]: ", end="")
+		out = []
+		with context.local(arch="amd64", bits=64):
+			self.dbg = Debugger("./cube", aslr=False, debug_from=0x55555555950a) # You must wait for the libc to be loaded to call malloc
+			self.dbg.migrate(libdebug=True)
+			address = self.dbg.call("malloc", [0x100])
+			self.assertEqual(address, 0x55555555d2a0)
+			
+	#@unittest.skip
+	def test_callbacks(self):
+		print("\ntest_callbacks [libdebug]: ", end="")
+		with context.local(arch = 'amd64'):
+			ANTI_DEBUG_TEST_FINISHED = 0x0401590
+			RWX_SECTION = 0x7ffff7ff8000
+			END_UNPACK  = RWX_SECTION + 0x80
+			SYSCALL_TRAP_PTRACE = RWX_SECTION + 0x9e
+			self.dbg = Debugger("./traps_withSymbols", aslr=False, debug_from=ANTI_DEBUG_TEST_FINISHED).set_split_on_fork()
+			
+			self.dbg.continue_until("fork")
+			self.dbg.finish()
+			pid = self.dbg.wait_split()
+			
+			second_child = self.dbg.children[pid]
+			self.dbg.migrate(libdebug=True)
+			second_child.emulate_ptrace_slave(self.dbg)
+			self.dbg.emulate_ptrace_master(second_child)
+			# Continue after fork
+			self.dbg.c(wait=True)
+			second_child.c(wait=True)
+			return
+			# handle signal
+			self.dbg.c(wait=True)
+			second_child.c(wait=True, force=True)
+			self.dbg.p.sendline(b"CSCG{4ND_4LL_0FF_TH1S_W0RK_JU5T_T0_G3T_TH1S_STUUUP1D_FL44G??!!1}")
+			for i in range(1, 22):
+				if second_child.instruction_pointer == RWX_SECTION + 1:
+					# setup unpack
+					self.dbg.c(wait=True)
+					second_child.c(until=END_UNPACK)
+					if i < 4:
+						second_child.c(wait=True)
+						continue
+					elif i == 4:
+						self.dbg.p.recv() # Just receive the prompt
+						# Pass ptrace check
+						second_child.c(until=SYSCALL_TRAP_PTRACE)
+						second_child.step()
+						second_child.return_value = 0x0
+					else:
+						...
+				# Temporary breakpoint to avoid having a \xCC in the dump 
+				# Use breakpoint instead of until so I can wait for both the breakpoint and the exit of the process
+				second_child.b(END_UNPACK, temporary=True)
+				second_child.c(wait=True)
+			
+			self.assertTrue(b"YES !" in dbg.p.recv())
+
+			second_child.close()
+
+	#@unittest.skip
+	def test_inner_debugger(self):	
+		print("\ntest_inner_debugger [libdebug]:")	
+		from sage.all import IntegerModRing, MatrixSpace, vector
+
+		END_ANTI_TRACING = 0x0401590
+		PTRACE_CONT = 0x0401775
+		RWX_SECTION = 0x7ffff7ff8000
+		END_UNPACK  = RWX_SECTION + 0x80
+		TRAP_PTRACE = RWX_SECTION + 0x9e
+		MATRIX_DATA = RWX_SECTION + 0xc2
+
+		def parse_line(data: bytes):
+		    ans = []
+		    for i in range(0, 0x10):
+		        ans.append(u32(data[i*4: (i+1)*4]))
+		    return ans
+
+		self.dbg = Debugger("./traps_withSymbols", aslr=False, debug_from=END_ANTI_TRACING)
+		self.dbg.next()
+		child_pid = self.dbg.return_value
+		# Wait for parent to attach
+		self.dbg.continue_until("waitpid")
+		self.dbg.finish()
+
+		self.dbg.migrate(libdebug=True)
+		child = Inner_Debugger(self.dbg, child_pid)
+
+		self.dbg.p.sendline(b"A"*0x40)
+		A, b = [], []
+		for i in range(1, 21):
+		    if i <= 4:
+		      self.dbg.continue_until(PTRACE_CONT, loop=True)
+		    child.continue_until(END_UNPACK, loop=True)
+		    if i == 4:
+		      child.continue_until(TRAP_PTRACE)
+		      child.step()
+		      child.return_value = 0x0
+		    if i in range(5, 5+0x10):
+		      A.append(parse_line(child.read(MATRIX_DATA, 0x40)))
+		      b.append(u32(child.read(MATRIX_DATA+ 0x40, 4)))
+		R = IntegerModRing(2**32)
+		M = MatrixSpace(R, 0x10, 0x10)
+		A = M(A)
+		b = vector(b)
+		x = A.solve_right(b)
+		flag = b""
+		for n in x:
+		    flag += p32(n)
+		flag = xor(flag, 0xd)
+		self.assertEqual(flag, b"CSCG{4ND_4LL_0FF_TH1S_W0RK_JU5T_T0_G3T_TH1S_STUUUP1D_FL44G??!!1}")
 
 if __name__ == "__main__":
 	with context.quiet:
 		unittest.main()
```

