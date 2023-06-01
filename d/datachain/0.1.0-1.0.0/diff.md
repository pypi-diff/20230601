# Comparing `tmp/datachain-0.1.0.tar.gz` & `tmp/datachain-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datachain-0.1.0.tar", max compression
+gzip compressed data, was "datachain-1.0.0.tar", max compression
```

## Comparing `datachain-0.1.0.tar` & `datachain-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    35060 2023-03-26 22:49:34.715348 datachain-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-03-26 22:49:34.715403 datachain-0.1.0/README.md
--rw-r--r--   0        0        0      246 2023-03-26 22:49:34.715564 datachain-0.1.0/datachain/__init__.py
--rw-r--r--   0        0        0       32 2023-03-26 22:49:34.715707 datachain-0.1.0/datachain/core/__init__.py
--rw-r--r--   0        0        0    12290 2023-03-26 22:49:34.715863 datachain-0.1.0/datachain/core/common.py
--rw-r--r--   0        0        0     3044 2023-03-26 22:49:34.715970 datachain-0.1.0/datachain/core/lazy.py
--rw-r--r--   0        0        0       48 2023-03-26 22:49:34.716048 datachain-0.1.0/datachain/core/logging.py
--rw-r--r--   0        0        0     2248 2023-03-26 22:49:34.716145 datachain-0.1.0/datachain/core/sync.py
--rw-r--r--   0        0        0      617 2023-03-26 22:49:34.716236 datachain-0.1.0/datachain/core/utils.py
--rw-r--r--   0        0        0       32 2023-03-26 22:49:34.716372 datachain-0.1.0/datachain/sources/__init__.py
--rw-r--r--   0        0        0      636 2023-03-26 22:58:29.615157 datachain-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 datachain-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35060 2023-03-26 22:49:34.715348 datachain-1.0.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-26 22:49:34.715403 datachain-1.0.0/README.md
+-rw-r--r--   0        0        0      187 2023-03-27 10:55:56.699305 datachain-1.0.0/datachain/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-01 01:19:09.359858 datachain-1.0.0/datachain/config/__init__.py
+-rw-r--r--   0        0        0     2629 2023-03-31 02:43:07.470280 datachain-1.0.0/datachain/config/logging.py
+-rw-r--r--   0        0        0      748 2023-06-01 01:19:09.359983 datachain-1.0.0/datachain/config/params.py
+-rw-r--r--   0        0        0       32 2023-03-26 22:49:34.715707 datachain-1.0.0/datachain/core/__init__.py
+-rw-r--r--   0        0        0    17603 2023-06-01 01:19:09.360230 datachain-1.0.0/datachain/core/common.py
+-rw-r--r--   0        0        0     3044 2023-03-27 10:29:58.237300 datachain-1.0.0/datachain/core/lazy.py
+-rw-r--r--   0        0        0     2243 2023-03-31 01:27:20.943629 datachain-1.0.0/datachain/core/sync.py
+-rw-r--r--   0        0        0       32 2023-03-26 22:49:34.716372 datachain-1.0.0/datachain/sources/__init__.py
+-rw-r--r--   0        0        0      617 2023-03-28 17:59:32.602567 datachain-1.0.0/datachain/utils/func.py
+-rw-r--r--   0        0        0      577 2023-06-01 01:19:59.948926 datachain-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 datachain-1.0.0/PKG-INFO
```

### Comparing `datachain-0.1.0/LICENSE` & `datachain-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datachain-0.1.0/datachain/core/common.py` & `datachain-1.0.0/datachain/core/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """@Author: Rayane AMROUCHE
 
 Common classes.
 """
+
 from __future__ import annotations
 
 import json
 import uuid
 import inspect
 
 try:
@@ -14,14 +15,17 @@
     pass
 
 from typing import Any, Union, Optional, Tuple, Dict, List, Callable
 
 from datachain.core.lazy import Lazy, LazyLoadingRequired
 from datachain.core.sync import unwrap_async
 
+from datachain.config.logging import Logger
+from datachain.config.params import Params
+
 session_uuid = uuid.uuid4()
 
 
 class Pipe:
     """A class representing a transformation function."""
 
     def __init__(self, func: Callable, *args: Any, **kwds: Any) -> None:
@@ -127,15 +131,15 @@
         params = self.params.copy()
         params.update(kwds)
         if self.func:
             return self.func(*args, **params)
         return None
 
 
-def _transform(obj: Any, func: Callable, args: Tuple, kwds: Dict) -> Any:
+def _transform(obj: Any, func: Any, args: Tuple, kwds: Dict) -> Any:
     """Apply a given function to transform data using the given arguments.
 
     Args:
         obj (Any): Data to transform.
         func (Callable): Transforming function.
         args (Tuple): Arguments to pass to the transforming function.
         kwds (Dict): Keyword arguments to pass to the transforming function.
@@ -149,19 +153,31 @@
     data = obj.data
     target = None
 
     # If the function is a string, get the method with that name from the data object
     if isinstance(func, str):
         # Put a value in target because data is in the method
         target = func
-        func = getattr(data, func)
-        # If the attribute is not callable then it is not a method so it is returned
-        if not callable(func):
-            # We actually should check if args and kwds are given and raise an error
-            return func
+        kwds["__target"] = target
+
+        def get_attr(__data, *args, **kwargs):
+            func = getattr(__data, kwargs["__target"])
+            # If the attribute is not callable then it is not a method so it is returned
+            if not callable(func):
+                # Check if args and kwds are given while func is not callable
+                if not args and not kwargs:
+                    raise TypeError(f"'{type(func)}' object is not callable")
+                Logger.logger.info("Reading attribute '%s'", kwargs["__target"])
+                return func
+            del kwargs["__target"]
+            return func(*args, **kwargs)
+
+        func = get_attr
+        target = None
+
     elif isinstance(func, tuple):
         func, target = func
         # If the pipe target name is the same as a keyword argument name, raise an error
         if target in kwds:
             msg = f"{target} is both the pipe target and a keyword argument"
             raise ValueError(msg)
         # Add the data to the keyword arguments
@@ -169,84 +185,117 @@
 
     # If the data is awaitable then await it
     if inspect.isawaitable(data):
         func = unwrap_async(func, target)
 
     # If no target is given then obj is the first argument
     if target is None:
-        return func(data, *args, **kwds)
+        return Logger.log_func(func)(data, *args, **kwds)
     # Otherwhise
-    return func(*args, **kwds)
+    return Logger.log_func(func)(*args, **kwds)
 
 
 class Data(Lazy):
     """Data class."""
 
     def __init__(
         self,
         extractor: Optional[Callable] = None,
-        params: Optional[Dict] = None,
+        args: Optional[Tuple] = None,
+        kwds: Optional[Dict] = None,
         cached: bool = True,
     ) -> None:
         """Initializes a new Data instance.
 
         Args:
             extractor (Optional[Callable]): The data extraction function to use.
             params (Optional[Dict]): Parameters to pass to the extraction function.
             cached (bool): Whether the data should be cached or loaded on demand.
         """
         self.extractor = extractor
-        self.params = {} if params is None else params
+        self.params = inspect.signature(extractor).bind(*args, **kwds)
         self.cached = cached
 
     @Lazy.property
     def data(self) -> Any:
-        """Returns the value of the `__data` attribute, loading it lazily if necessary.
+        """Returns the value of the `_data` attribute, loading it lazily if necessary.
 
         Raises:
-            LazyLoadingRequired: If the `__data` attribute has not yet been loaded.
+            LazyLoadingRequired: If the `_data` attribute has not yet been loaded.
 
         Returns:
-            Any: The value of the `__data` attribute.
+            Any: The value of the `_data` attribute.
         """
         if not self.cached:
             self.__load__("data")
         try:
-            return self.__data  # type: ignore
+            return self._data  # type: ignore
         except AttributeError as err:
             raise LazyLoadingRequired from err
 
     def __load__(self, attr: Any) -> None:
         if attr == "data":
             if self.extractor is None:
                 return None
 
-            self.__data = (  # pylint: disable=attribute-defined-outside-init
-                self.extractor(**self.params)
+            self._data = (  # pylint: disable=attribute-defined-outside-init
+                self.extractor(*self.params.args, **self.params.kwargs)
             )
-            return self.__data
+            return self._data
         return None
 
     def force_data(self, value: Any):
         """Force the data value of the instance.
 
         Args:
             value (Any): The new value to set for the data.
         """
-        self.__data = value  # pylint: disable=attribute-defined-outside-init
+        self._data = value  # pylint: disable=attribute-defined-outside-init
+        return self
+
+    def load_data(self):
+        """Force the data value of the instance.
+
+        Args:
+            value (Any): The new value to set for the data.
+        """
+        self.__load__("data")
+        return self
+
+    def load_cache(self, datamanager: DataManager, key: str):
+        """Load data to a DataManager cache
+
+        Args:
+            datamanager (DataManager): A DataManager object used to load data in cache.
+            key (str): A string key used to retrieve cached data from the DataManager.
+
+        Returns:
+            self: The instance which is now cached.
+        """
+        datamanager.load_cache(self, key)
+        return self
 
     def __repr__(self) -> str:
         try:
-            return repr(self.__data)
+            return repr(self._data)
         except AttributeError:
             return "<Data not loaded>"
 
+    def serialize(self):
+        """Serialize the data, extractor, and parameters into a UUID string.
+
+        Returns:
+            str: A UUID string representing the serialized data, extractor, and
+            parameters.
+        """
+        return f"<{repr(self.extractor)}{repr(self.params)}>"
+
     def _ipython_display_(self):
         try:
-            display(self.__data)
+            display(self._data)
         except AttributeError:
             print("<Data not loaded>")
 
     def transform(self, func: Any, *args: Any, **kwds: Any) -> Data:
         """Transforms the current instance's data by applying a function to it and
         returns a new Data instance.
 
@@ -255,17 +304,15 @@
             *args (Any): Additional positional arguments to pass to the function.
             **kwds (Any): Additional keyword arguments to pass to the function.
 
         Returns:
             Any: A new Data instance with the transformed data.
         """
         sign = inspect.signature(_transform).bind(self, func, args, kwds)
-        sign.apply_defaults()
-        params = sign.arguments
-        return Data(_transform, params, self.cached)
+        return Data(_transform, sign.args, sign.kwargs, self.cached)
 
     def chain(self, *pipes: Pipe) -> Union[Any, Tuple[Any, List[Any]]]:
         """Chains multiple transformation functions together and applies them
         sequentially to the data stored in the current instance of Data.
 
         Args:
             *pipes (Pipe): One or more Pipe objects representing transformation
@@ -305,89 +352,192 @@
 
         Returns:
             Any: The original Data instance.
         """
         decorator(_transform(self, func, args, kwds))
         return self
 
+    @staticmethod
+    def __setup_extract(
+        extractor: Callable, key: Optional[str], args: Any, kwds: Any
+    ) -> Any:
+        """Set up the extraction process.
+
+        Args:
+            extractor (Callable): A function or class that extracts data from a source.
+            *args (Any): Positional arguments for the extractor.
+            **kwds (Any): Keyword arguments for the extractor.
+
+        Returns:
+            Any: The arguments to pass to the extractor function.
+        """
+        if key is not None:
+            try:
+                params = Params.config[key]
+            except KeyError as _:
+                params = {}
+        else:
+            params = {}
+        params.update(kwds)
+        extractor_func = getattr(extractor, "func", extractor)
+        sign = inspect.signature(extractor_func).bind(*args, **params)
+        Logger.logger.info(
+            "Extract data from extractor '%s' using these arguments: %s",
+            extractor_func.__name__,
+            str(sign.arguments),
+        )
+        return sign
+
+    @staticmethod
+    def extract(
+        extractor: Callable, *args: Any, key: Optional[str] = None, **kwds: Any
+    ) -> Any:
+        """Extract data from a data source using the config and an appropriate
+        extractor.
+
+        Args:
+            extractor (Callable): A function or class that extracts data from a source.
+            *args (Any): Positional arguments for the extractor.
+            key (Optional[str], optional): Optional config key to access config params.
+            Defaults to None.
+            **kwds (Any): Keyword arguments for the extractor.
+
+        Returns:
+            Any: The extracted data.
+        """
+        params = Data.__setup_extract(extractor, key, args, kwds)
+        data = Data(extractor, params.args, params.kwargs, True)
+        return data
+
+    def load(
+        self, loader: Callable, *args: Any, key: Optional[str] = None, **kwds: Any
+    ) -> Any:
+        """Load data to a data source using the config and an appropriate loader.
+
+        Args:
+            loader (Callable): A function or class that load data to a source.
+            *args (Any): Positional arguments for the extractor.
+            key (Optional[str], optional): Optional config key to access config params.
+            Defaults to None.
+            **kwds (Any): Keyword arguments for the extractor.
+
+        Returns:
+            Any: The original data.
+        """
+        if key is not None:
+            try:
+                params = Params.config[key]
+            except KeyError as _:
+                params = {}
+        else:
+            params = {}
+        params.update(kwds)
+        sign = inspect.signature(_transform).bind(self, loader, args, params)
+        _transform(*sign.args, **sign.kwargs)
+        return self
+
 
 class DataManager:
     """
     Data Manager class.
 
     Args:
         metadata (Dict): A dictionary of data metadata.
         cache (Optional): A data cache to store cached data. Defaults to None.
 
     """
 
-    def __init__(self, metadata: Dict, cache: Any = None) -> None:
+    def __init__(self, metadata: Optional[Dict] = None, cache: Any = None) -> None:
         """Initialize a Data Manager instance."""
+        if metadata is None:
+            metadata = {}
         self.config = metadata
         if cache is None:
             cache = {}
         self.__cache: Any = cache
         self.__params: Dict = {}
 
     def __getitem__(self, key: str):
         self.__params = self.config[key]
         return self
 
     def __repr__(self) -> str:
         """Return the string representation of the Data Manager instance."""
         return json.dumps(self.config, indent=4)
 
-    def __setup_extract(self, extractor: Callable, *args: Any, **kwds: Any) -> Any:
+    def __setup_extract(self, extractor: Callable, args: Any, kwds: Any) -> Any:
         """Set up the extraction process.
 
         Args:
             extractor (Callable): A function or class that extracts data from a source.
             *args (Any): Positional arguments for the extractor.
             **kwds (Any): Keyword arguments for the extractor.
 
         Returns:
             Any: The arguments to pass to the extractor function.
         """
-        params = self.__params
-        params.update(kwds)
+        self.__params.update(kwds)
         extractor_func = getattr(extractor, "func", extractor)
-        sign = inspect.signature(extractor_func).bind(*args, **params)
+        sign = inspect.signature(extractor_func).bind(*args, **self.__params)
         self.__params = {}
-        sign.apply_defaults()
-        return sign.arguments
+        Logger.logger.info(
+            "Extract data from extractor '%s' using these arguments: %s",
+            extractor_func.__name__,
+            str(sign.arguments),
+        )
+        return sign
 
     def extract(self, extractor: Callable, *args: Any, **kwds: Any) -> Any:
         """Extract data from a data source using the config and an appropriate
         extractor.
 
         Args:
             extractor (Callable): A function or class that extracts data from a source.
             *args (Any): Positional arguments for the extractor.
             **kwds (Any): Keyword arguments for the extractor.
 
         Returns:
             Any: The extracted data.
         """
-        params = self.__setup_extract(extractor, *args, **kwds)
-        cache_key = str(uuid.uuid5(session_uuid, str(params)))
-        data = Data(extractor, params, True)
+        params = self.__setup_extract(extractor, args, kwds)
+        data = Data(extractor, params.args, params.kwargs, True)
+        cache_key = str(uuid.uuid5(session_uuid, data.serialize()))
         if cache_key in self.__cache.keys():
+            Logger.logger.info("Load data from cache")
             data.force_data(self.__cache[cache_key])
         else:
-            self.__cache[cache_key] = data
+            self.load_cache(data, data.serialize())
         return data
 
     def uncached_extract(self, extractor: Callable, *args: Any, **kwds: Any) -> Data:
         """Extract data from a data source using the config and an appropriate
         extractor.
 
         Args:
             extractor (Callable): A function or class that extracts data from a source.
             *args (Any): Positional arguments for the extractor.
             **kwds (Any): Keyword arguments for the extractor.
 
         Returns:
             Any: The extracted data.
         """
-        params = self.__setup_extract(extractor, *args, **kwds)
-        data = Data(extractor, params, False)
+        params = self.__setup_extract(extractor, args, kwds)
+        data = Data(extractor, params.args, params.kwargs, False)
         return data
+
+    def load_cache(self, data: Any, key: str) -> None:
+        """Load data into the cache.
+
+        Args:
+            data (Any): The data to be cached.
+            key (str): A string key used to retrieve cached data from the DataManager.
+
+        Raises:
+            NotImplementedError: If the data is an awaitable object, as these cannot be
+            cached.
+        """
+        Logger.logger.info("Load data to cache")
+        if not inspect.isawaitable(data.data):
+            key = str(uuid.uuid5(session_uuid, key))
+            self.__cache[key] = data.data
+        else:
+            raise NotImplementedError("Awaitable extraction is not cacheable")
```

### Comparing `datachain-0.1.0/datachain/core/lazy.py` & `datachain-1.0.0/datachain/core/lazy.py`

 * *Files identical despite different names*

### Comparing `datachain-0.1.0/datachain/core/sync.py` & `datachain-1.0.0/datachain/core/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """@Author Rayane AMROUCHE
 
 Async tools.
 """
+
 import functools
 import asyncio
 
 from typing import Any, Optional, Callable, Tuple
 
 from concurrent.futures import ThreadPoolExecutor
 
 import nest_asyncio  # type: ignore
 
-
 nest_asyncio.apply()
 
 
 def force_async(func: Any) -> Any:
     """Turns a sync function to async function using threads.
 
     Args:
@@ -24,16 +24,16 @@
     Returns:
         Any: Function wrapped with async transparency.
     """
 
     pool = ThreadPoolExecutor()
 
     @functools.wraps(func)
-    async def wrapper(*args, **kwargs) -> asyncio.Future:
-        future = pool.submit(func, *args, **kwargs)
+    async def wrapper(*args, **kwds) -> asyncio.Future:
+        future = pool.submit(func, *args, **kwds)
         return await asyncio.wrap_future(future)  # make it awaitable
 
     return wrapper
 
 
 def force_sync(func: Any) -> Any:
     """Turn an async function to sync function.
@@ -42,16 +42,16 @@
         func (Any): Function to wrap.
 
     Returns:
         Any: Function wrapped with sync transparency.
     """
 
     @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        res = func(*args, **kwargs)
+    def wrapper(*args, **kwds):
+        res = func(*args, **kwds)
         if asyncio.iscoroutine(res):
             return asyncio.get_event_loop().run_until_complete(res)
         return res
 
     return wrapper
 
 
@@ -80,18 +80,18 @@
     Returns:
         Callable: The wrapped function.
     """
     functools.wraps(func)
 
     if target is None:
 
-        async def wrapper(obj, *args, **kwargs):
+        async def wrapper_target(obj, *args, **kwds):
             obj = await obj
-            return func(obj, *args, **kwargs)
+            return func(obj, *args, **kwds)
 
-    else:
+        return wrapper_target
 
-        async def wrapper(*args, **kwargs):
-            kwargs[target] = await kwargs[target]
-            return func(*args, **kwargs)
+    async def wrapper(*args, **kwds):
+        kwds[target] = await kwds[target]
+        return func(*args, **kwds)
 
     return wrapper
```

### Comparing `datachain-0.1.0/datachain/core/utils.py` & `datachain-1.0.0/datachain/utils/func.py`

 * *Files identical despite different names*

### Comparing `datachain-0.1.0/PKG-INFO` & `datachain-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: datachain
-Version: 0.1.0
+Version: 1.0.0
 Summary: Tools to build data pipelines.
 License: GPL-3.0-or-later
 Author: Rayane AMROUCHE
 Author-email: rayaneamrouche@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
-Requires-Dist: notebook (>=6.5.3,<7.0.0)
 Description-Content-Type: text/markdown
```

