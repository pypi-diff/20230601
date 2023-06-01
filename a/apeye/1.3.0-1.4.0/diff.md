# Comparing `tmp/apeye-1.3.0.tar.gz` & `tmp/apeye-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeye-1.3.0.tar", last modified: Mon Dec 12 16:41:01 2022, max compression
+gzip compressed data, was "apeye-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apeye-1.3.0.tar` & `apeye-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     7622 2022-12-12 16:40:34.714631 apeye-1.3.0/LICENSE
--rw-r--r--   0        0        0     5460 2022-12-12 16:40:34.714631 apeye-1.3.0/README.rst
--rw-r--r--   0        0        0     1260 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/__init__.py
--rw-r--r--   0        0        0     4173 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/cache.py
--rw-r--r--   0        0        0     1903 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/email_validator.py
--rw-r--r--   0        0        0   241256 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/public_suffix_list.dat
--rw-r--r--   0        0        0        0 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/py.typed
--rw-r--r--   0        0        0     7404 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/rate_limiter.py
--rw-r--r--   0        0        0     8354 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/requests_url.py
--rw-r--r--   0        0        0    14539 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/slumber_url/__init__.py
--rw-r--r--   0        0        0     2299 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/slumber_url/exceptions.py
--rw-r--r--   0        0        0     5780 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/slumber_url/serializers/__init__.py
--rw-r--r--   0        0        0     2205 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/slumber_url/serializers/_abc.py
--rw-r--r--   0        0        0     2008 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/slumber_url/serializers/_pyyaml_serializer.py
--rw-r--r--   0        0        0     2224 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/slumber_url/serializers/_ruamel_serializer.py
--rw-r--r--   0        0        0     2360 2022-12-12 16:40:34.714631 apeye-1.3.0/apeye/url.py
--rw-r--r--   0        0        0     5066 2022-12-12 16:40:34.718632 apeye-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7338 1970-01-01 00:00:00.000000 apeye-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7622 2023-06-01 13:26:51.848225 apeye-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5460 2023-06-01 13:26:51.848225 apeye-1.4.0/README.rst
+-rw-r--r--   0        0        0     1260 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/__init__.py
+-rw-r--r--   0        0        0     4173 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/cache.py
+-rw-r--r--   0        0        0     1903 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/email_validator.py
+-rw-r--r--   0        0        0   241256 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/public_suffix_list.dat
+-rw-r--r--   0        0        0        0 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/py.typed
+-rw-r--r--   0        0        0     7532 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/rate_limiter.py
+-rw-r--r--   0        0        0     8354 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/requests_url.py
+-rw-r--r--   0        0        0    14539 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/slumber_url/__init__.py
+-rw-r--r--   0        0        0     2299 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/slumber_url/exceptions.py
+-rw-r--r--   0        0        0     5780 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/slumber_url/serializers/__init__.py
+-rw-r--r--   0        0        0     2205 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/slumber_url/serializers/_abc.py
+-rw-r--r--   0        0        0     2008 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/slumber_url/serializers/_pyyaml_serializer.py
+-rw-r--r--   0        0        0     2224 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/slumber_url/serializers/_ruamel_serializer.py
+-rw-r--r--   0        0        0     2360 2023-06-01 13:26:51.848225 apeye-1.4.0/apeye/url.py
+-rw-r--r--   0        0        0     5221 2023-06-01 13:26:51.852225 apeye-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 apeye-1.4.0/PKG-INFO
```

### Comparing `apeye-1.3.0/LICENSE` & `apeye-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/README.rst` & `apeye-1.4.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/apeye
 	:target: https://github.com/domdfcoding/apeye/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/apeye
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye/v1.3.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye/v1.4.0
 	:target: https://github.com/domdfcoding/apeye/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/apeye
 	:target: https://github.com/domdfcoding/apeye/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/apeye
 	:target: https://pypi.org/project/apeye/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `apeye-1.3.0/apeye/__init__.py` & `apeye-1.4.0/apeye/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # this package
 from apeye.url import URL, Domain, URLPath
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "GNU Lesser General Public License v3 or later (LGPLv3+)"
-__version__: str = "1.3.0"
+__version__: str = "1.4.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = [
 		"URL",
 		"Domain",
 		"URLPath",
 		]
```

### Comparing `apeye-1.3.0/apeye/cache.py` & `apeye-1.4.0/apeye/cache.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/email_validator.py` & `apeye-1.4.0/apeye/email_validator.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/public_suffix_list.dat` & `apeye-1.4.0/apeye/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/rate_limiter.py` & `apeye-1.4.0/apeye/rate_limiter.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,27 +32,28 @@
 #  https://github.com/ionrock/cachecontrol
 #  Apache-2.0 Licensed
 #
 
 # stdlib
 import datetime
 import logging
+import os
 import shutil
 import time
 import warnings
 import zlib
 from functools import wraps
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Collection, Dict, Optional
 
 # 3rd party
 import platformdirs
 import requests
-from cachecontrol import CacheControl, CacheControlAdapter  # type: ignore[import]  # nodep
-from cachecontrol.caches.file_cache import FileCache  # type: ignore[import]  # nodep
-from cachecontrol.heuristics import ExpiresAfter  # type: ignore[import]  # nodep
+from cachecontrol import CacheControl, CacheControlAdapter  # nodep
+from cachecontrol.caches.file_cache import FileCache  # nodep
+from cachecontrol.heuristics import ExpiresAfter  # nodep
 from domdf_python_tools.paths import PathPlus
 
 # import codetiming
 
 __all__ = [
 		"rate_limit",
 		"RateLimitAdapter",
@@ -123,23 +124,28 @@
 	:param heuristic:
 	:param cacheable_methods:
 
 	.. autosummary-widths:: 7/16
 	.. latex:clearpage::
 	"""
 
-	def send(self, request: requests.PreparedRequest, cacheable_methods=None, **kwargs) -> requests.Response:
+	def send(  # type: ignore[override]  # Latest cachecontrol has changed the signature to put cacheable_methods last
+		self,
+		request: requests.PreparedRequest,
+		cacheable_methods: Optional[Collection[str]] = None,
+		**kwargs,
+		) -> requests.Response:
 		r"""
 		Send a request.
 
 		Use the request information to see if it exists in the cache and cache the response if we need to and can.
 
 		:param request: The :class:`requests.PreparedRequest` being sent.
 		:param cacheable_methods:
-		:param \*\*kwargs: Additional arguments take by :meth:`requests.adapters.HTTPAdapter.send`.
+		:param \*\*kwargs: Additional arguments taken by :meth:`requests.adapters.HTTPAdapter.send` (e.g. ``timeout``).
 		"""
 
 		cacheable = cacheable_methods or self.cacheable_methods
 		if request.method in cacheable:
 			try:
 				cached_response = self.controller.cached_request(request)
 			except zlib.error:  # pragma: no cover
@@ -179,15 +185,15 @@
 	def __init__(self, app_name: str, expires_after: datetime.timedelta = datetime.timedelta(days=28)):
 		self.app_name: str = str(app_name)
 		self.cache_dir = PathPlus(platformdirs.user_cache_dir(self.app_name))
 		self.cache_dir.maybe_make(parents=True)
 
 		self.session: requests.Session = CacheControl(
 				sess=requests.Session(),
-				cache=FileCache(self.cache_dir),
+				cache=FileCache(os.fspath(self.cache_dir)),
 				heuristic=ExpiresAfter(
 						days=expires_after.days,
 						seconds=expires_after.seconds,
 						microseconds=expires_after.microseconds,
 						),
 				adapter_class=RateLimitAdapter
 				)
```

### Comparing `apeye-1.3.0/apeye/requests_url.py` & `apeye-1.4.0/apeye/requests_url.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/slumber_url/__init__.py` & `apeye-1.4.0/apeye/slumber_url/__init__.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/slumber_url/exceptions.py` & `apeye-1.4.0/apeye/slumber_url/exceptions.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/slumber_url/serializers/__init__.py` & `apeye-1.4.0/apeye/slumber_url/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/slumber_url/serializers/_abc.py` & `apeye-1.4.0/apeye/slumber_url/serializers/_abc.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/slumber_url/serializers/_pyyaml_serializer.py` & `apeye-1.4.0/apeye/slumber_url/serializers/_pyyaml_serializer.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/slumber_url/serializers/_ruamel_serializer.py` & `apeye-1.4.0/apeye/slumber_url/serializers/_ruamel_serializer.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/apeye/url.py` & `apeye-1.4.0/apeye/url.py`

 * *Files identical despite different names*

### Comparing `apeye-1.3.0/pyproject.toml` & `apeye-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "flit-core<4,>=3.2",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apeye"
-version = "1.3.0"
+version = "1.4.0"
 description = "Handy tools for working with URLs and APIs."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "api", "cache", "requests", "rest", "url",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -24,15 +24,21 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-dependencies = [ "apeye-core>=1.0.0b2", "domdf-python-tools>=2.6.0", "platformdirs>=2.3.0", "requests>=2.24.0",]
+dependencies = [
+    "apeye-core>=1.0.0b2",
+    'cryptography<40; implementation_name == "pypy" and python_version <= "3.7"',
+    "domdf-python-tools>=2.6.0",
+    "platformdirs>=2.3.0",
+    "requests>=2.24.0",
+]
 dynamic = []
 
 [[project.authors]]
 name = "Dominic Davis-Foster"
 email = "dominic@davis-foster.co.uk"
 
 
@@ -158,14 +164,17 @@
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
 directives = [ "code-block",]
 
+[tool.dep_checker]
+allowed_unused = [ "cryptography",]
+
 [tool.dependency-dash."requirements.txt"]
 order = 10
 
 [tool.dependency-dash."tests/requirements.txt"]
 order = 20
 include = false
```

### Comparing `apeye-1.3.0/PKG-INFO` & `apeye-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeye
-Version: 1.3.0
+Version: 1.4.0
 Summary: Handy tools for working with URLs and APIs.
 Keywords: api,cache,requests,rest,url
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: apeye-core>=1.0.0b2
+Requires-Dist: cryptography<40; implementation_name == "pypy" and python_version <= "3.7"
 Requires-Dist: domdf-python-tools>=2.6.0
 Requires-Dist: platformdirs>=2.3.0
 Requires-Dist: requests>=2.24.0
 Requires-Dist: cachecontrol[filecache]>=0.12.6 ; extra == "all"
 Requires-Dist: lockfile>=0.12.2 ; extra == "all"
 Requires-Dist: cachecontrol[filecache]>=0.12.6 ; extra == "limiter"
 Requires-Dist: lockfile>=0.12.2 ; extra == "limiter"
@@ -137,23 +138,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/apeye
 	:target: https://github.com/domdfcoding/apeye/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/apeye
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye/v1.3.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/apeye/v1.4.0
 	:target: https://github.com/domdfcoding/apeye/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/apeye
 	:target: https://github.com/domdfcoding/apeye/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/apeye
 	:target: https://pypi.org/project/apeye/
 	:alt: PyPI - Downloads
 
 .. end shields
```

