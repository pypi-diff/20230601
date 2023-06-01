# Comparing `tmp/ffmpeg-progress-yield-0.7.7.tar.gz` & `tmp/ffmpeg-progress-yield-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg-progress-yield-0.7.7.tar", last modified: Tue May 30 14:51:49 2023, max compression
+gzip compressed data, was "ffmpeg-progress-yield-0.7.8.tar", last modified: Thu Jun  1 07:00:14 2023, max compression
```

## Comparing `ffmpeg-progress-yield-0.7.7.tar` & `ffmpeg-progress-yield-0.7.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.009763 ffmpeg-progress-yield-0.7.7/
--rw-r--r--   0 werner     (501) staff       (20)     2473 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/CHANGELOG.md
--rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.7/LICENSE
--rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 14:51:49.009870 ffmpeg-progress-yield-0.7.7/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.7/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.007881 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/
--rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-30 14:51:46.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     1283 2023-05-30 06:56:19.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)     7903 2023-05-30 07:05:38.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/ffmpeg_progress_yield.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.008745 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/not-zip-safe
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-30 14:51:48.000000 ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-30 14:51:49.010215 ffmpeg-progress-yield-0.7.7/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.7/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 14:51:49.009508 ffmpeg-progress-yield-0.7.7/test/
--rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.7/test/test.mp4
--rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-30 07:03:53.000000 ffmpeg-progress-yield-0.7.7/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-01 07:00:14.321584 ffmpeg-progress-yield-0.7.8/
+-rw-r--r--   0 werner     (501) staff       (20)     2602 2023-06-01 07:00:13.000000 ffmpeg-progress-yield-0.7.8/CHANGELOG.md
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.8/LICENSE
+-rw-r--r--   0 werner     (501) staff       (20)    10151 2023-06-01 07:00:14.321695 ffmpeg-progress-yield-0.7.8/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.8/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-01 07:00:14.319866 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield/
+-rw-r--r--   0 werner     (501) staff       (20)      103 2023-06-01 07:00:12.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     1283 2023-05-30 06:56:19.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)     9472 2023-06-01 07:00:00.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield/ffmpeg_progress_yield.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-01 07:00:14.320667 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    10151 2023-06-01 07:00:14.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      494 2023-06-01 07:00:14.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-06-01 07:00:14.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       78 2023-06-01 07:00:14.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-06-01 07:00:14.000000 ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      279 2023-06-01 07:00:14.322016 ffmpeg-progress-yield-0.7.8/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.8/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-06-01 07:00:14.321456 ffmpeg-progress-yield-0.7.8/test/
+-rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.8/test/test.mp4
+-rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-30 07:03:53.000000 ffmpeg-progress-yield-0.7.8/test/test.py
```

### Comparing `ffmpeg-progress-yield-0.7.7/CHANGELOG.md` & `ffmpeg-progress-yield-0.7.8/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Changelog
 
 
+## v0.7.8 (2023-06-01)
+
+* Image handling.
+
+  Check if image2 inputs use looping or not, and set duration to infinity if needed
+
+
 ## v0.7.6 (2023-05-30)
 
 * Always use duration_override if present.
 
 
 ## v0.7.5 (2023-05-30)
```

### Comparing `ffmpeg-progress-yield-0.7.7/LICENSE` & `ffmpeg-progress-yield-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.7/PKG-INFO` & `ffmpeg-progress-yield-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.7
+Version: 0.7.8
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,21 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.8 (2023-06-01)
+
+* Image handling.
+
+  Check if image2 inputs use looping or not, and set duration to infinity if needed
+
+
 ## v0.7.6 (2023-05-30)
 
 * Always use duration_override if present.
 
 
 ## v0.7.5 (2023-05-30)
```

### Comparing `ffmpeg-progress-yield-0.7.7/README.md` & `ffmpeg-progress-yield-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/__main__.py` & `ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield/ffmpeg_progress_yield.py` & `ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield/ffmpeg_progress_yield.py`

 * *Files 13% similar despite different names*

```diff
@@ -69,14 +69,50 @@
             return True
         else:
             return False
     except ValueError:
         return False
 
 
+def _get_inputs_with_options(cmd: List[str]) -> List[List[str]]:
+    """
+    Collect all inputs with their options.
+    For example, input is:
+
+        ffmpeg -i input1.mp4 -i input2.mp4 -i input3.mp4 -filter_complex ...
+
+    Output is:
+
+        [
+            ["-i", "input1.mp4"],
+            ["-i", "input2.mp4"],
+            ["-i", "input3.mp4"],
+        ]
+
+    Another example:
+
+        ffmpeg -f lavfi -i color=c=black:s=1920x1080 -loop 1 -i image.png -filter_complex ...
+
+    Output is:
+
+        [
+            ["-f", "lavfi", "-i", "color=c=black:s=1920x1080"],
+            ["-loop", "1", "-i", "image.png"],
+        ]
+    """
+    inputs = []
+    prev_index = 0
+    for i, arg in enumerate(cmd):
+        if arg == "-i":
+            inputs.append(cmd[prev_index : i + 2])
+            prev_index = i + 2
+
+    return inputs
+
+
 class FfmpegProgress:
     DUR_REGEX = re.compile(
         r"Duration: (?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
     )
     TIME_REGEX = re.compile(
         r"out_time=(?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
     )
@@ -145,26 +181,31 @@
         if duration_override is not None:
             total_dur = int(duration_override * 1000)
 
         cmd_with_progress = (
             [self.cmd[0]] + ["-progress", "-", "-nostats"] + self.cmd[1:]
         )
 
+        # collect all inputs with their options, e.g.
+        inputs_with_options = _get_inputs_with_options(self.cmd)
+
         stderr = []
         base_popen_kwargs = self.base_popen_kwargs.copy()
         if popen_kwargs is not None:
             base_popen_kwargs.update(popen_kwargs)
 
         self.process = subprocess.Popen(
             cmd_with_progress,
             **base_popen_kwargs,
         )  # type: ignore
 
         yield 0
 
+        input_idx = 0
+
         while True:
             if self.process.stdout is None:
                 continue
 
             stderr_line = (
                 self.process.stdout.readline().decode("utf-8", errors="replace").strip()
             )
@@ -178,25 +219,38 @@
             stderr.append(stderr_line.strip())
 
             self.stderr = "\n".join(stderr)
 
             # assign the total duration if it was found. this can happen multiple times for multiple inputs,
             # in which case we have to determine the overall duration by taking the min/max (dependent on -shortest being present)
             if (
-                total_dur_match := self.DUR_REGEX.search(stderr_line)
+                current_dur_match := self.DUR_REGEX.search(stderr_line)
             ) and duration_override is None:
-                total_dur_ms = to_ms(**total_dur_match.groupdict())
-                if total_dur is not None:
+                input_options = inputs_with_options[input_idx]
+
+                current_dur_ms: int = to_ms(**current_dur_match.groupdict())
+                # if the previous line had "image2", it's a single image and we assume a really short intrinsic duration (4ms),
+                # but if it's a loop, we assume infinity
+                if "image2" in stderr[-2] and "-loop 1" in " ".join(input_options):
+                    # infinity
+                    current_dur_ms = 2**64
+                if "-shortest" in self.cmd:
                     total_dur = (
-                        min(total_dur, total_dur_ms)
-                        if "-shortest" in self.cmd
-                        else max(total_dur, total_dur_ms)
+                        min(total_dur, current_dur_ms)
+                        if total_dur is not None
+                        else current_dur_ms
                     )
                 else:
-                    total_dur = total_dur_ms
+                    total_dur = (
+                        max(total_dur, current_dur_ms)
+                        if total_dur is not None
+                        else current_dur_ms
+                    )
+
+                input_idx += 1
 
             if (
                 progress_time := FfmpegProgress.TIME_REGEX.search(stderr_line)
             ) and total_dur is not None:
                 elapsed_time = to_ms(**progress_time.groupdict())
                 yield min(max(round(elapsed_time / total_dur * 100, 2), 0), 100)
```

### Comparing `ffmpeg-progress-yield-0.7.7/ffmpeg_progress_yield.egg-info/PKG-INFO` & `ffmpeg-progress-yield-0.7.8/ffmpeg_progress_yield.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.7
+Version: 0.7.8
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,21 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.8 (2023-06-01)
+
+* Image handling.
+
+  Check if image2 inputs use looping or not, and set duration to infinity if needed
+
+
 ## v0.7.6 (2023-05-30)
 
 * Always use duration_override if present.
 
 
 ## v0.7.5 (2023-05-30)
```

### Comparing `ffmpeg-progress-yield-0.7.7/setup.py` & `ffmpeg-progress-yield-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.7/test/test.mp4` & `ffmpeg-progress-yield-0.7.8/test/test.mp4`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.7/test/test.py` & `ffmpeg-progress-yield-0.7.8/test/test.py`

 * *Files identical despite different names*

