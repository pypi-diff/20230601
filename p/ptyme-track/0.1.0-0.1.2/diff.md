# Comparing `tmp/ptyme_track-0.1.0.tar.gz` & `tmp/ptyme_track-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptyme_track-0.1.0.tar", max compression
+gzip compressed data, was "ptyme_track-0.1.2.tar", max compression
```

## Comparing `ptyme_track-0.1.0.tar` & `ptyme_track-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2023-06-01 02:08:22.624777 ptyme_track-0.1.0/LICENSE
--rw-r--r--   0        0        0     1969 2023-06-01 02:08:22.624777 ptyme_track-0.1.0/README.md
--rw-r--r--   0        0        0       43 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/__init__.py
--rw-r--r--   0        0        0     1021 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/cement.py
--rw-r--r--   0        0        0     6492 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/client.py
--rw-r--r--   0        0        0      221 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/cur_times.py
--rw-r--r--   0        0        0     2771 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/git_ci_diff.py
--rw-r--r--   0        0        0     3333 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/main.py
--rw-r--r--   0        0        0      936 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/ptyme_env.py
--rw-r--r--   0        0        0      234 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/secret.py
--rw-r--r--   0        0        0     2993 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/server.py
--rw-r--r--   0        0        0      204 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/signature.py
--rw-r--r--   0        0        0      300 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/signed_time.py
--rw-r--r--   0        0        0     1951 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/time_blocks.py
--rw-r--r--   0        0        0     1231 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/ptyme_track/validation.py
--rw-r--r--   0        0        0      776 2023-06-01 02:08:22.628777 ptyme_track-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 ptyme_track-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2020 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/README.md
+-rw-r--r--   0        0        0       43 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/cement.py
+-rw-r--r--   0        0        0     6818 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/client.py
+-rw-r--r--   0        0        0      221 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/cur_times.py
+-rw-r--r--   0        0        0     2771 2023-06-01 04:30:12.754795 ptyme_track-0.1.2/ptyme_track/git_ci_diff.py
+-rw-r--r--   0        0        0     3333 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/main.py
+-rw-r--r--   0        0        0      936 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/ptyme_env.py
+-rw-r--r--   0        0        0      234 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/secret.py
+-rw-r--r--   0        0        0     2993 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/server.py
+-rw-r--r--   0        0        0      204 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/signature.py
+-rw-r--r--   0        0        0      300 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/signed_time.py
+-rw-r--r--   0        0        0     1951 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/time_blocks.py
+-rw-r--r--   0        0        0     1231 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/ptyme_track/validation.py
+-rw-r--r--   0        0        0      798 2023-06-01 04:30:12.758795 ptyme_track-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2654 1970-01-01 00:00:00.000000 ptyme_track-0.1.2/PKG-INFO
```

### Comparing `ptyme_track-0.1.0/LICENSE` & `ptyme_track-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/README.md` & `ptyme_track-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Ptyme Track
 The obnoxiously hard to spell time tracking based on file modifications and signed time reporting. The P is silent like in Pterodactyl
 
 ## Usage
 
+### Installation
+`pip install ptyme-track`
+
 ### Server / client
 Simply run the server with `ptyme_track --server`
 
-For the client, use ptyme_track --client
+For the client, use `ptyme_track --client`
 
 ### Running locally
 Simply run `ptyme_track --standalone` in the background.
 
 ### Setting directories to watch
 By default, the current working directory is used and hidden directories are ignored. To manually set paths, use the `PTYME_WATCHED_DIRS` environment variable.
 
@@ -41,14 +44,14 @@
 on:
   pull_request:
     paths:
       - '.ptyme_track/*'
 
 jobs:
   track-time:
-    uses: JamesHutchison/ptyme-track/.github/workflows/time_tracking.yaml
+    uses: JamesHutchison/ptyme-track/.github/workflows/time_tracking.yaml@main
     permissions:
       pull-requests: write
     with:
       base-branch: origin/${{ github.event.pull_request.base.ref }}
       pr-number: ${{ github.event.pull_request.number }}
 ```
```

### Comparing `ptyme_track-0.1.0/ptyme_track/cement.py` & `ptyme_track-0.1.2/ptyme_track/cement.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/ptyme_track/client.py` & `ptyme_track-0.1.2/ptyme_track/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,34 +36,37 @@
         self.server_url = server_url
         self._file_hash_cache: Dict[str, bytes] = {}
         self._last_update: Union[float, None] = None
         self._watched_dirs = watched_dirs
         self._cur_times = cur_times
         self._ignored_dirs = ignored_dirs
 
-    def run_forever(self) -> None:
+    def run_forever(self, cemented_file=Path(CEMENTED_PATH)) -> None:
         print("Starting ptyme-track", flush=True)
         prev_files_hash = None
         stopped = False
-        cemented_file = Path(CEMENTED_PATH)
+        freshly_cemented = False
         while True:
             if cemented_file.exists():
                 prev_files_hash = cemented_file.read_text().strip()
                 stopped = True
                 cemented_file.unlink()
-            prev_files_hash, stopped = self._run_loop(prev_files_hash, stopped)
+                freshly_cemented = True
+            prev_files_hash, stopped = self._run_loop(prev_files_hash, stopped, freshly_cemented)
+            freshly_cemented = False
 
     def _run_loop(
-        self, prev_files_hash: Optional[str], stopped: bool
+        self, prev_files_hash: Optional[str], stopped: bool, freshly_cemented: bool = False
     ) -> Tuple[Union[str, None], bool]:
         start = time.time()
         files_hash = self._get_files_hash_for_watched_dirs()
         # _last_update should be set BEFORE the hash is calculated to avoid a race condition
         self._last_update = start
-        stopped = self._record_time_or_stop(files_hash, prev_files_hash, stopped)
+        if not freshly_cemented:
+            stopped = self._record_time_or_stop(files_hash, prev_files_hash, stopped)
         prev_files_hash = files_hash
         end = time.time()
         logger.debug(f"Hash took {(end - start):.1f} seconds")
         next_time = start + PTYME_WATCH_INTERVAL_MIN * 60
         cur_time = time.time()
         if cur_time < next_time:
             self._perform_sleep(next_time - cur_time)
@@ -109,15 +112,19 @@
                 for ignored_dir in self._ignored_dirs:
                     if ignored_dir in str(file):
                         ignored_count += 1
                         if ignored_count % IGNORED_COUNT_MOD == 0:
                             time.sleep(0.01)
                         break
                 else:
-                    if not last_update or file.stat().st_mtime > last_update:
+                    if (
+                        not last_update
+                        or str(file) not in self._file_hash_cache
+                        or file.stat().st_mtime > last_update
+                    ):
                         count += 1
                         if count % COUNT_MOD == 0:
                             time.sleep(0.01)
                         with file.open("rb") as f:
                             file_hash = hashlib.md5()
                             file_hash.update(f.read())
                         self._file_hash_cache[str(file)] = file_hash.hexdigest().encode("utf-8")
```

### Comparing `ptyme_track-0.1.0/ptyme_track/git_ci_diff.py` & `ptyme_track-0.1.2/ptyme_track/git_ci_diff.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/ptyme_track/main.py` & `ptyme_track-0.1.2/ptyme_track/main.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/ptyme_track/ptyme_env.py` & `ptyme_track-0.1.2/ptyme_track/ptyme_env.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/ptyme_track/server.py` & `ptyme_track-0.1.2/ptyme_track/server.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/ptyme_track/time_blocks.py` & `ptyme_track-0.1.2/ptyme_track/time_blocks.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/ptyme_track/validation.py` & `ptyme_track-0.1.2/ptyme_track/validation.py`

 * *Files identical despite different names*

### Comparing `ptyme_track-0.1.0/pyproject.toml` & `ptyme_track-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 [tool.black]
 # soft limit, wrap just before 100 chars
 line-length = 98
 
 [tool.poetry]
 name = "ptyme-track"
-version = "0.1.0"
-description = "Time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl"
+version = "0.1.2"
+description = "The obnoxiously named time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl"
 authors = ["James Hutchison <JamesGHutchison@proton.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ptyme_track" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ptyme_track-0.1.0/PKG-INFO` & `ptyme_track-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ptyme-track
-Version: 0.1.0
-Summary: Time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl
+Version: 0.1.2
+Summary: The obnoxiously named time tracking based on file modifications and signed reporting. The P is silent like in Pterodactyl
 License: MIT
 Author: James Hutchison
 Author-email: JamesGHutchison@proton.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,18 +15,21 @@
 Description-Content-Type: text/markdown
 
 # Ptyme Track
 The obnoxiously hard to spell time tracking based on file modifications and signed time reporting. The P is silent like in Pterodactyl
 
 ## Usage
 
+### Installation
+`pip install ptyme-track`
+
 ### Server / client
 Simply run the server with `ptyme_track --server`
 
-For the client, use ptyme_track --client
+For the client, use `ptyme_track --client`
 
 ### Running locally
 Simply run `ptyme_track --standalone` in the background.
 
 ### Setting directories to watch
 By default, the current working directory is used and hidden directories are ignored. To manually set paths, use the `PTYME_WATCHED_DIRS` environment variable.
 
@@ -57,15 +60,15 @@
 on:
   pull_request:
     paths:
       - '.ptyme_track/*'
 
 jobs:
   track-time:
-    uses: JamesHutchison/ptyme-track/.github/workflows/time_tracking.yaml
+    uses: JamesHutchison/ptyme-track/.github/workflows/time_tracking.yaml@main
     permissions:
       pull-requests: write
     with:
       base-branch: origin/${{ github.event.pull_request.base.ref }}
       pr-number: ${{ github.event.pull_request.number }}
 ```
```

