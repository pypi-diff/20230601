# Comparing `tmp/motion_python-0.1.47.tar.gz` & `tmp/motion_python-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.47.tar", max compression
+gzip compressed data, was "motion_python-0.1.48.tar", max compression
```

## Comparing `motion_python-0.1.47.tar` & `motion_python-0.1.48.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3319 2023-06-01 00:18:54.137276 motion_python-0.1.47/README.md
--rw-r--r--   0        0        0      202 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/component.py
--rw-r--r--   0        0        0    12098 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/execute.py
--rw-r--r--   0        0        0     4392 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/fit_task.py
--rw-r--r--   0        0        0     7489 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-01 00:18:54.137276 motion_python-0.1.47/motion/utils.py
--rw-r--r--   0        0        0     1773 2023-06-01 00:19:15.190517 motion_python-0.1.47/pyproject.toml
--rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 motion_python-0.1.47/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-01 19:39:38.490110 motion_python-0.1.48/README.md
+-rw-r--r--   0        0        0      202 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/component.py
+-rw-r--r--   0        0        0    13729 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/execute.py
+-rw-r--r--   0        0        0     4961 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/fit_task.py
+-rw-r--r--   0        0        0     9364 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-06-01 19:39:38.490110 motion_python-0.1.48/motion/utils.py
+-rw-r--r--   0        0        0     1517 2023-06-01 19:40:01.520150 motion_python-0.1.48/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.48/PKG-INFO
```

### Comparing `motion_python-0.1.47/README.md` & `motion_python-0.1.48/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![motion](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"motion")
 [![lint (via ruff)](https://github.com/dm4ml/motion/workflows/lint/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"lint")
 [![docs](https://github.com/dm4ml/motion/workflows/docs/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"docs")
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub tag](https://img.shields.io/github/tag/dm4ml/motion?include_prereleases=&sort=semver&color=blue)](https://github.com/dm4ml/motion/releases/)
-[![PyPI version](https://badge.fury.io/py/motion-python.svg)](https://badge.fury.io/py/motion-python)
+[![PyPI version](https://badge.fury.io/py/motion-python.svg?branch=main&kill_cache=1)](https://badge.fury.io/py/motion-python)
 
 Motion is a lightweight **framework** for building machine learning (ML) applications, designed to **reduce the MLOps burdens** of making sure your models, prompts, and other stateful objects are **up-to-date with your data.**
 
 ## Why Motion?
 
 While building an ML application demo is easier than ever thanks to state-of-the-art models and open-source libraries, making sure ML applications _update with new data over time_ is still a challenge. As a result, developers painstakingly stitch together and maintain pipelines that run on a schedule (e.g., fine-tuning, updating indexes).
```

### Comparing `motion_python-0.1.47/motion/cli.py` & `motion_python-0.1.48/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.47/motion/component.py` & `motion_python-0.1.48/motion/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         @AdderComponent.fit("add")
         def add(state, values, infer_results):
             return {"value": state["value"] + sum(values)}
 
         if __name__ == "__main__":
             c = AdderComponent() # Create instance of AdderComponent
-            c.run(add=1, force_fit=True) # Will return 1, blocking until fit
+            c.run(add=1, flush_fit=True) # Will return 1, blocking until fit
             # is done. Resulting state is {"value": 1}
             c.run(add=2) # Will return 3, not waiting for fit operation.
             # Resulting state will eventually be {"value": 3}
         ```
 
     === "Multiple Dataflows"
         ```python
@@ -63,17 +63,17 @@
 
         @Calculator.fit("subtract")
         def decrement(state, values, infer_results):
             return {"value": state["value"] - sum(values)}
 
         if __name__ == "__main__":
             c = Calculator()
-            c.run(add=1, force_fit=True) # Will return 1, blocking until fit
+            c.run(add=1, flush_fit=True) # Will return 1, blocking until fit
             # is done. Resulting state is {"value": 1}
-            c.run(subtract=1, force_fit=True) # Will return 0, blocking
+            c.run(subtract=1, flush_fit=True) # Will return 0, blocking
             # until fit is done. Resulting state is {"value": 0}
         ```
 
     === "Batch Size > 1"
 
         ```python
         from motion import Component
@@ -331,15 +331,15 @@
             return state["value"] + value
 
         @MyComponent.infer("multiply")
         def multiply(state, value):
             return state["value"] * value
 
         c = MyComponent()
-        c.run(add=1, force_fit=True) # Returns 1
+        c.run(add=1, flush_fit=True) # Returns 1
         c.run(multiply=2) # Returns 2
         ```
 
         Args:
             key (str): Keyword for the infer dataflow.
 
         Returns:
@@ -422,15 +422,15 @@
         def multiply(state, values, infer_results):
             product = 1
             for value in values:
                 product *= value
             return state["value"] * product
 
         c = MyComponent()
-        c.run(add=1, force_fit=True) # Returns 1
+        c.run(add=1, flush_fit=True) # Returns 1
         c.run(multiply=2) # Returns 2, fit not executed yet
         c.run(multiply=3) # Returns 3, fit will execute; state["value"] = 6
         # Some time later...
         c.run(multiply=4) # Returns 24
         ```
 
         Args:
```

### Comparing `motion_python-0.1.47/motion/execute.py` & `motion_python-0.1.48/motion/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -227,15 +227,15 @@
 
     def run(
         self,
         key: str,
         value: Any,
         cache_ttl: int,
         force_refresh: bool,
-        force_fit: bool,
+        flush_fit: bool,
     ) -> Any:
         route_hit = False
         infer_result = None
 
         # Run the infer route
         if key in self._infer_routes.keys():
             route_hit = True
@@ -298,15 +298,15 @@
                 queue_identifier: str = self._get_queue_identifier(key, fit_udf_name)
                 channel_identifier: str = self._get_channel_identifier(
                     key, fit_udf_name
                 )
 
                 identifier = str(uuid4())
 
-                if force_fit:
+                if flush_fit:
                     # Add pubsub channel to listen to
                     fit_event = FitEvent(
                         self._redis_con, channel_identifier, identifier
                     )
                     fit_events.add(fit_udf_name, fit_event)
 
                 # Add to fit queue
@@ -315,20 +315,20 @@
                     cloudpickle.dumps(
                         (
                             {
                                 "value": value,
                                 "infer_result": infer_result,
                                 "identifier": identifier,
                             },
-                            force_fit,
+                            flush_fit,
                         )
                     ),
                 )
 
-            if force_fit:
+            if flush_fit:
                 # Wait for fit result to finish
                 fit_events.wait()
                 # Update state
                 self._state = self._loadState()
                 v = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
                 if not v:
                     raise ValueError(
@@ -337,7 +337,55 @@
                     )
                 self.version = int(v)
 
         if not route_hit:
             raise KeyError(f"Key {key} not in routes.")
 
         return infer_result
+
+    def flush_fit(self, dataflow_key: str) -> None:
+        # Check if key has fit ops
+        if dataflow_key not in self._fit_routes.keys():
+            return
+
+        # Push a noop into the relevant queues
+        fit_events = FitEventGroup(dataflow_key)
+        for fit_udf_name in self._fit_routes[dataflow_key].keys():
+            queue_identifier: str = self._get_queue_identifier(
+                dataflow_key, fit_udf_name
+            )
+            channel_identifier: str = self._get_channel_identifier(
+                dataflow_key, fit_udf_name
+            )
+
+            identifier = "NOOP_" + str(uuid4())
+
+            # Add pubsub channel to listen to
+            fit_event = FitEvent(self._redis_con, channel_identifier, identifier)
+            fit_events.add(fit_udf_name, fit_event)
+
+            # Add to fit queue
+            self._redis_con.rpush(
+                queue_identifier,
+                cloudpickle.dumps(
+                    (
+                        {
+                            "value": None,
+                            "infer_result": None,
+                            "identifier": identifier,
+                        },
+                        True,
+                    )
+                ),
+            )
+
+        # Wait for fit result to finish
+        fit_events.wait()
+        # Update state
+        self._state = self._loadState()
+        v = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
+        if not v:
+            raise ValueError(
+                f"Error loading state for {self._instance_name}." + " No version found."
+            )
+
+        self.version = int(v)
```

### Comparing `motion_python-0.1.47/motion/fit_task.py` & `motion_python-0.1.48/motion/fit_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,17 +67,17 @@
                     item = redis_con.blpop(self.queue_identifier, timeout=1)
                     if item is None:
                         if not self.running:
                             break  # no more items in the list
                         else:
                             continue
 
-                    item, force_fit = cloudpickle.loads(item[1])
+                    item, flush_fit = cloudpickle.loads(item[1])
                     self.batch.append(item)
-                    if force_fit:
+                    if flush_fit:
                         break
             except redis.exceptions.ConnectionError:
                 if not self.running:
                     logger.error("Connection to redis lost.")
 
                 break
 
@@ -85,39 +85,53 @@
             if not self.running:
                 self.cleanup()
                 break
 
             if not self.batch:
                 continue
 
-            values = [job["value"] for job in self.batch]
-            infer_results = [job["infer_result"] for job in self.batch]
-            identifiers = [job["identifier"] for job in self.batch]
+            # Remove from batch if it was a noop
+            values = []
+            infer_results = []
+            identifiers = []
+            for job in self.batch:
+                if not job["identifier"].startswith("NOOP_"):
+                    values.append(job["value"])
+                    infer_results.append(job["infer_result"])
+                identifiers.append(job["identifier"])
 
+            # Check that there are elements in values and infer_results
             # Acquire lock and run op
-            acquired_lock = lock.acquire(blocking=True)
-            if acquired_lock:
-                old_state = loadState(
-                    redis_con, self.instance_name, self.load_state_func
-                )
-                state_update = self.route.run(
-                    state=old_state, values=values, infer_results=infer_results
-                )
+            if len(values) >= 1:
+                acquired_lock = lock.acquire(blocking=True)
+                if acquired_lock:
+                    old_state = loadState(
+                        redis_con, self.instance_name, self.load_state_func
+                    )
+                    state_update = self.route.run(
+                        state=old_state,
+                        values=values,
+                        infer_results=infer_results,
+                    )
 
-                if not isinstance(state_update, dict):
-                    logger.error("fit methods should return a dict of state updates.")
+                    if not isinstance(state_update, dict):
+                        logger.error(
+                            "fit methods should return a dict of state updates."
+                        )
+                    else:
+                        old_state.update(state_update)
+                        saveState(
+                            old_state,
+                            redis_con,
+                            self.instance_name,
+                            self.save_state_func,
+                        )
+                    lock.release()
                 else:
-                    old_state.update(state_update)
-                    saveState(
-                        old_state,
-                        redis_con,
-                        self.instance_name,
-                        self.save_state_func,
-                    )
-                lock.release()
+                    logger.error("Lock not acquired; batch lost.")
 
             for identifier in identifiers:
                 redis_con.publish(
                     self.channel_identifier,
                     identifier,
                 )
```

### Comparing `motion_python-0.1.47/motion/instance.py` & `motion_python-0.1.48/motion/instance.py`

 * *Files 20% similar despite different names*

```diff
@@ -68,16 +68,17 @@
     def instance_name(self) -> str:
         """Component name with a random phrase to represent
         the name of this instance."""
         return self._instance_name
 
     def shutdown(self) -> None:
         """Shuts down a Motion component instance, saving state.
-        The state saving functionality is not implemented yet, but the
-        graceful shutdown is.
+
+        Warning: if you don't shutdown a component instance when you are
+        finished using it, your program may infinitely hang!
 
         Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
@@ -101,14 +102,37 @@
         if is_open:
             logger.info(f"Shutting down {self._instance_name}...")
 
         self._executor.shutdown(is_open=is_open)
 
         self.running = False
 
+    def get_version(self) -> int:
+        """
+        Gets the state version (might be outdated) currently being
+        used for infer ops.
+
+        Usage:
+        ```python
+        from motion import Component
+
+        C = Component("MyComponent")
+
+        @C.init_state
+        def setUp():
+            return {"value": 0}
+
+        # Define infer and fit operations
+
+        c_instance = C()
+        c_instance.get_version() # Returns 1 (first version)
+        ```
+        """
+        return self._executor.version  # type: ignore
+
     def read_state(self, key: str) -> Any:
         """Gets the current value for the key in the component's state.
 
         Usage:
         ```python
         from motion import Component
 
@@ -131,20 +155,64 @@
             key (str): Key in the state to get the value for.
 
         Returns:
             Any: Current value for the key.
         """
         return self._executor._loadState()[key]
 
+    def flush_fit(self, dataflow_key: str) -> None:
+        """Flushes the fit queue corresponding to the dataflow
+        key, if it exists, and updates the instance state.
+        Warning: this is a blocking operation and could take
+        a while if your fit op takes a long time!
+
+        The fit queue will be flushed even if there aren't
+        the predefined batch_size number of elements.
+
+        Example Usage:
+        ```python
+        from motion import Component
+
+        C = Component("MyComponent")
+
+        @C.init_state
+        def setUp():
+            return {"value": 0}
+
+        @C.infer("add")
+        def add(state, value):
+            return state["value"] + value
+
+        @C.fit("add", batch_size=2)
+        def add(state, values, infer_results):
+            return {"value": state["value"] + sum(values)}
+
+        @C.infer("multiply")
+        def multiply(state, value):
+            return state["value"] * value
+
+        c = C() # Create instance of C
+        c.run(add=1)
+        c.flush_fit("add") # (1)!
+        c.run(add=2) # This will use the updated state
+
+        # 1. Runs the fit op even though only one element is in the batch
+        ```
+
+        Args:
+            dataflow_key (str): Key of the dataflow.
+        """
+        self._executor.flush_fit(dataflow_key)
+
     def run(
         self,
         *,
         cache_ttl: int = DEFAULT_KEY_TTL,
         force_refresh: bool = False,
-        force_fit: bool = False,
+        flush_fit: bool = False,
         **kwargs: Any,
     ) -> Union[Any, Tuple[Any, FitEventGroup]]:
         """Runs the dataflow (infer and fit ops) for the keyword argument
         passed in. If the key is not found to have any ops, an error
         is raised. Only one keyword argument should be passed in.
         Fit ops are only executed when the batch size is reached.
 
@@ -167,21 +235,21 @@
             return {"value": state["value"] + sum(values)}
 
         @C.infer("multiply")
         def multiply(state, value):
             return state["value"] * value
 
         c = C() # Create instance of C
-        c.run(add=1, force_fit=True) # (1)!
+        c.run(add=1, flush_fit=True) # (1)!
         c.run(add=1) # Returns 1
-        c.run(add=2, force_fit=True) # Returns 2, result state["value"] = 4
+        c.run(add=2, flush_fit=True) # Returns 2, result state["value"] = 4
         # Previous line called fit function and flushed fit queue
         c.run(add=3) # No fit op runs since batch size = 1
         c.run(multiply=2) # Returns 8 since state["value"] = 4
-        c.run(multiply=3, force_fit=True) # (2)!
+        c.run(multiply=3, flush_fit=True) # (2)!
 
         # 1. This forces the fit op to run even though the batch size
         #   isn't reached, and waits for the fit op to finish running
         # 2. This doesn't force or wait for any fit ops, since there are
         #   no fit ops defined for `multiply`
         ```
 
@@ -193,38 +261,38 @@
                 time is extended if there are subsequent infer calls
                 for the same value.
             force_refresh (bool, optional): Read the latest value of the
                 state before running an inference call, otherwise a stale
                 version of the state or a cached result may be used.
                 If you do not want to read from the cache, set force_refresh
                 = True. Defaults to False.
-            force_fit (bool, optional):
+            flush_fit (bool, optional):
                 If True, waits for the fit op to finish executing before
                 returning. If the fit queue hasn't reached batch_size
                 yet, the fit op runs anyways. Force refreshes the
                 state after the fit op completes. Defaults to False.
             **kwargs:
                 Keyword arguments for the infer and fit ops. You can only
                 pass in one pair.
 
         Raises:
             ValueError: If more than one dataflow key-value pair is passed.
 
         Returns:
             Any: Result of the inference call. Might take a long time
-            to run if `force_fit = True` and the fit operation is
+            to run if `flush_fit = True` and the fit operation is
             computationally expensive.
         """
         if len(kwargs) != 1:
             raise ValueError("Only one key-value pair is allowed in kwargs.")
 
         key, value = next(iter(kwargs.items()))
 
         infer_result = self._executor.run(
             key=key,
             value=value,
             cache_ttl=cache_ttl,
             force_refresh=force_refresh,
-            force_fit=force_fit,
+            flush_fit=flush_fit,
         )
 
         return infer_result
```

### Comparing `motion_python-0.1.47/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.48/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.47/motion/route.py` & `motion_python-0.1.48/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.47/motion/utils.py` & `motion_python-0.1.48/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.47/pyproject.toml` & `motion_python-0.1.48/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,20 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.47"
+version = "0.1.48"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-duckdb = "^0.7.1"
 click = "^8.1.3"
 colorlog = "^6.7.0"
-croniter = "^1.3.8"
-fastapi = "^0.95.0"
-pandas = "^1.5.3"
-pyarrow = "^11.0.0"
-numpy = "^1.24.2"
-requests = "^2.28.2"
-uvicorn = "^0.21.1"
-httpx = "^0.23.3"
-python-multipart = "^0.0.6"
 pydantic = "^1.10.7"
-urllib3 = "^1.26.15"
-flask = "^2.2.3"
-rich = "^13.3.4"
 cloudpickle = "^2.0"
 redis = "^4.5.5"
 psutil = "^5.9.5"
 
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
```

### Comparing `motion_python-0.1.47/PKG-INFO` & `motion_python-0.1.48/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,35 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.47
+Version: 0.1.48
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudpickle (>=2.0,<3.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: croniter (>=1.3.8,<2.0.0)
-Requires-Dist: duckdb (>=0.7.1,<0.8.0)
-Requires-Dist: fastapi (>=0.95.0,<0.96.0)
-Requires-Dist: flask (>=2.2.3,<3.0.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: redis (>=4.5.5,<5.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: rich (>=13.3.4,<14.0.0)
-Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
-Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Motion
 
 [![motion](https://github.com/dm4ml/motion/workflows/motion/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"motion")
 [![lint (via ruff)](https://github.com/dm4ml/motion/workflows/lint/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"lint")
 [![docs](https://github.com/dm4ml/motion/workflows/docs/badge.svg)](https://github.com/dm4ml/motion/actions?query=workflow:"docs")
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub tag](https://img.shields.io/github/tag/dm4ml/motion?include_prereleases=&sort=semver&color=blue)](https://github.com/dm4ml/motion/releases/)
-[![PyPI version](https://badge.fury.io/py/motion-python.svg)](https://badge.fury.io/py/motion-python)
+[![PyPI version](https://badge.fury.io/py/motion-python.svg?branch=main&kill_cache=1)](https://badge.fury.io/py/motion-python)
 
 Motion is a lightweight **framework** for building machine learning (ML) applications, designed to **reduce the MLOps burdens** of making sure your models, prompts, and other stateful objects are **up-to-date with your data.**
 
 ## Why Motion?
 
 While building an ML application demo is easier than ever thanks to state-of-the-art models and open-source libraries, making sure ML applications _update with new data over time_ is still a challenge. As a result, developers painstakingly stitch together and maintain pipelines that run on a schedule (e.g., fine-tuning, updating indexes).
```

