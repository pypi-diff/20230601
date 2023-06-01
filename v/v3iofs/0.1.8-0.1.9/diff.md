# Comparing `tmp/v3iofs-0.1.8.tar.gz` & `tmp/v3iofs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/v3iofs-0.1.8.tar", last modified: Wed Nov  3 16:09:31 2021, max compression
+gzip compressed data, was "v3iofs-0.1.9.tar", last modified: Thu Jan 13 08:43:31 2022, max compression
```

## Comparing `v3iofs-0.1.8.tar` & `v3iofs-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 katyak     (501) staff       (20)        0 2021-11-03 16:09:31.000000 v3iofs-0.1.8/
--rw-r--r--   0 katyak     (501) staff       (20)     3106 2021-11-03 16:09:31.000000 v3iofs-0.1.8/PKG-INFO
-drwxr-xr-x   0 katyak     (501) staff       (20)        0 2021-11-03 16:09:31.000000 v3iofs-0.1.8/v3iofs.egg-info/
--rw-r--r--   0 katyak     (501) staff       (20)     3106 2021-11-03 16:09:31.000000 v3iofs-0.1.8/v3iofs.egg-info/PKG-INFO
--rw-r--r--   0 katyak     (501) staff       (20)      552 2021-11-03 16:09:31.000000 v3iofs-0.1.8/v3iofs.egg-info/SOURCES.txt
--rw-r--r--   0 katyak     (501) staff       (20)       26 2021-11-03 16:09:31.000000 v3iofs-0.1.8/v3iofs.egg-info/requires.txt
--rw-r--r--   0 katyak     (501) staff       (20)        7 2021-11-03 16:09:31.000000 v3iofs-0.1.8/v3iofs.egg-info/top_level.txt
--rw-r--r--   0 katyak     (501) staff       (20)        1 2021-11-03 16:09:31.000000 v3iofs-0.1.8/v3iofs.egg-info/dependency_links.txt
--rw-r--r--   0 katyak     (501) staff       (20)       26 2021-01-27 13:38:48.000000 v3iofs-0.1.8/requirements.txt
--rw-r--r--   0 katyak     (501) staff       (20)      128 2021-01-27 13:38:48.000000 v3iofs-0.1.8/dev-requirements.txt
--rw-r--r--   0 katyak     (501) staff       (20)     1625 2021-01-28 14:14:13.000000 v3iofs-0.1.8/Makefile
-drwxr-xr-x   0 katyak     (501) staff       (20)        0 2021-11-03 16:09:31.000000 v3iofs-0.1.8/tests/
--rw-r--r--   0 katyak     (501) staff       (20)     2991 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/conftest.py
--rw-r--r--   0 katyak     (501) staff       (20)      830 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/test_setup.py
--rw-r--r--   0 katyak     (501) staff       (20)      841 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/test_v3iofs.py
--rw-r--r--   0 katyak     (501) staff       (20)      363 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/Dockerfile
--rw-r--r--   0 katyak     (501) staff       (20)      414 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/Dockerfile.fsspec-6
--rw-r--r--   0 katyak     (501) staff       (20)     4024 2021-11-03 16:01:04.000000 v3iofs-0.1.8/tests/test_fs.py
--rw-r--r--   0 katyak     (501) staff       (20)     1472 2021-01-28 13:09:10.000000 v3iofs-0.1.8/tests/test_file.py
--rw-r--r--   0 katyak     (501) staff       (20)     3553 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/sanchez.pq
--rw-r--r--   0 katyak     (501) staff       (20)     1877 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/test_dask.py
--rw-r--r--   0 katyak     (501) staff       (20)     1139 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/test_pandas.py
--rw-r--r--   0 katyak     (501) staff       (20)     1097 2021-06-27 08:20:04.000000 v3iofs-0.1.8/tests/test_path.py
--rw-r--r--   0 katyak     (501) staff       (20)     1191 2021-01-27 13:38:48.000000 v3iofs-0.1.8/tests/test_install.py
--rw-r--r--   0 katyak     (501) staff       (20)      159 2021-01-27 13:38:48.000000 v3iofs-0.1.8/MANIFEST.in
--rw-r--r--   0 katyak     (501) staff       (20)     1620 2021-01-27 13:38:48.000000 v3iofs-0.1.8/README.md
--rw-r--r--   0 katyak     (501) staff       (20)     2398 2021-01-27 13:38:48.000000 v3iofs-0.1.8/setup.py
--rw-r--r--   0 katyak     (501) staff       (20)       38 2021-11-03 16:09:31.000000 v3iofs-0.1.8/setup.cfg
-drwxr-xr-x   0 katyak     (501) staff       (20)        0 2021-11-03 16:09:31.000000 v3iofs-0.1.8/v3iofs/
--rw-r--r--   0 katyak     (501) staff       (20)     1229 2021-11-03 16:08:36.000000 v3iofs-0.1.8/v3iofs/__init__.py
--rw-r--r--   0 katyak     (501) staff       (20)     2215 2021-02-21 09:38:16.000000 v3iofs-0.1.8/v3iofs/file.py
--rw-r--r--   0 katyak     (501) staff       (20)      356 2021-01-27 13:38:48.000000 v3iofs-0.1.8/v3iofs/utils.py
--rw-r--r--   0 katyak     (501) staff       (20)     9540 2021-11-03 16:01:04.000000 v3iofs-0.1.8/v3iofs/fs.py
--rw-r--r--   0 katyak     (501) staff       (20)     1531 2021-06-27 08:20:04.000000 v3iofs-0.1.8/v3iofs/path.py
--rw-r--r--   0 katyak     (501) staff       (20)    11357 2021-01-27 13:38:48.000000 v3iofs-0.1.8/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 08:43:31.403910 v3iofs-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-13 08:38:54.000000 v3iofs-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-01-13 08:38:54.000000 v3iofs-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-01-13 08:38:54.000000 v3iofs-0.1.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     2503 2022-01-13 08:43:31.403910 v3iofs-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-01-13 08:38:54.000000 v3iofs-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-01-13 08:38:54.000000 v3iofs-0.1.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-13 08:38:54.000000 v3iofs-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-01-13 08:43:31.403910 v3iofs-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-01-13 08:38:54.000000 v3iofs-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 08:43:31.403910 v3iofs-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/Dockerfile.fsspec-6
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/sanchez.pq
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-01-13 08:38:54.000000 v3iofs-0.1.9/tests/test_v3iofs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 08:43:31.403910 v3iofs-0.1.9/v3iofs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-01-13 08:43:28.000000 v3iofs-0.1.9/v3iofs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2215 2022-01-13 08:38:54.000000 v3iofs-0.1.9/v3iofs/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11047 2022-01-13 08:38:54.000000 v3iofs-0.1.9/v3iofs/fs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-01-13 08:38:54.000000 v3iofs-0.1.9/v3iofs/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-01-13 08:38:54.000000 v3iofs-0.1.9/v3iofs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 08:43:31.403910 v3iofs-0.1.9/v3iofs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2503 2022-01-13 08:43:31.000000 v3iofs-0.1.9/v3iofs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-01-13 08:43:31.000000 v3iofs-0.1.9/v3iofs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 08:43:31.000000 v3iofs-0.1.9/v3iofs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-13 08:43:31.000000 v3iofs-0.1.9/v3iofs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-13 08:43:31.000000 v3iofs-0.1.9/v3iofs.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `v3iofs-0.1.8/PKG-INFO` & `v3iofs-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 Metadata-Version: 2.1
 Name: v3iofs
-Version: 0.1.8
+Version: 0.1.9
 Summary: fsspec driver for v3io
 Home-page: https://github.com/v3io/v3iofs-py
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: MIT
-Description: # v3iofs
-        
-        <!--
-        [![CI](https://github.com/v3io/v3io-fs/workflows/CI/badge.svg)](https://github.com/v3io/v3io-fs/actions?query=workflow%3ACI)
-        -->
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        
-        
-        An [fsspec][fsspec] driver for [v3io][v3io].
-        
-        
-        ## Examples
-        
-        
-        ### Python
-        
-        ```python
-        >>> from v3iofs import V3ioFS  # Will register 'v3io' protocol in ffspec
-        >>> fs = V3ioFS('api.app.yh48.iguazio-cd2.com', v3io_access_key='s3cr3t')
-        >>> fs.ls('/container/path')
-        ```
-        
-        ### Pandas
-        
-        ```python
-        # Use V3IO_ACCESS_KEY & V3IO_API from environment
-        >> df = pd.read_csv('v3io://container/path/to/file.csv')
-        ```
-        
-        ### Dask
-        
-        ```python
-        >>> from v3iofs import V3ioFS
-        >>> from dask import bag
-        
-        # Use V3IO_ACCESS_KEY & V3IO_API from environment
-        >>> url = 'v3io://container/path'
-        >>> file = bag.read_text(url)
-        >>> data, _ = file.compute()
-        
-        # Pass key in storage_options
-        >>> storage_options={
-        ...     'v3io_api': 'webapi.app.iguazio.com',
-        ...     'v3io_access_key': 's3cr3t',
-        ... }
-        >>> file = bag.read_text(url, storage_options=storage_options)
-        >>> data, _ = file.compute()
-        ```
-        
-        ## Development
-        
-        
-        ### Testing
-        
-        You need to set `V3IO_ACCESS_KEY` and `V3IO_API` environment variables.
-        Then run `make test` to run the tests.
-        
-        
-        ### Environment
-        
-        Deployment requirements are in `requirements.txt` and development requirements
-        are in `dev-requirements.txt`.
-        
-        ```
-        $ python -m venv venv
-        $ ./venv/bin/python -m pip install -r dev-requirements.txt
-        ```
-        
-        
-        [fsspec]: https://filesystem-spec.readthedocs.io
-        [v3io]: https://www.iguazio.com/docs/tutorials/latest-release/getting-started/containers/
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# v3iofs
+
+<!--
+[![CI](https://github.com/v3io/v3io-fs/workflows/CI/badge.svg)](https://github.com/v3io/v3io-fs/actions?query=workflow%3ACI)
+-->
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+
+An [fsspec][fsspec] driver for [v3io][v3io].
+
+
+## Examples
+
+
+### Python
+
+```python
+>>> from v3iofs import V3ioFS  # Will register 'v3io' protocol in ffspec
+>>> fs = V3ioFS('api.app.yh48.iguazio-cd2.com', v3io_access_key='s3cr3t')
+>>> fs.ls('/container/path')
+```
+
+### Pandas
+
+```python
+# Use V3IO_ACCESS_KEY & V3IO_API from environment
+>> df = pd.read_csv('v3io://container/path/to/file.csv')
+```
+
+### Dask
+
+```python
+>>> from v3iofs import V3ioFS
+>>> from dask import bag
+
+# Use V3IO_ACCESS_KEY & V3IO_API from environment
+>>> url = 'v3io://container/path'
+>>> file = bag.read_text(url)
+>>> data, _ = file.compute()
+
+# Pass key in storage_options
+>>> storage_options={
+...     'v3io_api': 'webapi.app.iguazio.com',
+...     'v3io_access_key': 's3cr3t',
+... }
+>>> file = bag.read_text(url, storage_options=storage_options)
+>>> data, _ = file.compute()
+```
+
+## Development
+
+
+### Testing
+
+You need to set `V3IO_ACCESS_KEY` and `V3IO_API` environment variables.
+Then run `make test` to run the tests.
+
+
+### Environment
+
+Deployment requirements are in `requirements.txt` and development requirements
+are in `dev-requirements.txt`.
+
+```
+$ python -m venv venv
+$ ./venv/bin/python -m pip install -r dev-requirements.txt
+```
+
+
+[fsspec]: https://filesystem-spec.readthedocs.io
+[v3io]: https://www.iguazio.com/docs/tutorials/latest-release/getting-started/containers/
+
+
```

### Comparing `v3iofs-0.1.8/v3iofs.egg-info/PKG-INFO` & `v3iofs-0.1.9/v3iofs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 Metadata-Version: 2.1
 Name: v3iofs
-Version: 0.1.8
+Version: 0.1.9
 Summary: fsspec driver for v3io
 Home-page: https://github.com/v3io/v3iofs-py
 Author: Iguazio
 Author-email: yaronh@iguazio.com
 License: MIT
-Description: # v3iofs
-        
-        <!--
-        [![CI](https://github.com/v3io/v3io-fs/workflows/CI/badge.svg)](https://github.com/v3io/v3io-fs/actions?query=workflow%3ACI)
-        -->
-        [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        
-        
-        An [fsspec][fsspec] driver for [v3io][v3io].
-        
-        
-        ## Examples
-        
-        
-        ### Python
-        
-        ```python
-        >>> from v3iofs import V3ioFS  # Will register 'v3io' protocol in ffspec
-        >>> fs = V3ioFS('api.app.yh48.iguazio-cd2.com', v3io_access_key='s3cr3t')
-        >>> fs.ls('/container/path')
-        ```
-        
-        ### Pandas
-        
-        ```python
-        # Use V3IO_ACCESS_KEY & V3IO_API from environment
-        >> df = pd.read_csv('v3io://container/path/to/file.csv')
-        ```
-        
-        ### Dask
-        
-        ```python
-        >>> from v3iofs import V3ioFS
-        >>> from dask import bag
-        
-        # Use V3IO_ACCESS_KEY & V3IO_API from environment
-        >>> url = 'v3io://container/path'
-        >>> file = bag.read_text(url)
-        >>> data, _ = file.compute()
-        
-        # Pass key in storage_options
-        >>> storage_options={
-        ...     'v3io_api': 'webapi.app.iguazio.com',
-        ...     'v3io_access_key': 's3cr3t',
-        ... }
-        >>> file = bag.read_text(url, storage_options=storage_options)
-        >>> data, _ = file.compute()
-        ```
-        
-        ## Development
-        
-        
-        ### Testing
-        
-        You need to set `V3IO_ACCESS_KEY` and `V3IO_API` environment variables.
-        Then run `make test` to run the tests.
-        
-        
-        ### Environment
-        
-        Deployment requirements are in `requirements.txt` and development requirements
-        are in `dev-requirements.txt`.
-        
-        ```
-        $ python -m venv venv
-        $ ./venv/bin/python -m pip install -r dev-requirements.txt
-        ```
-        
-        
-        [fsspec]: https://filesystem-spec.readthedocs.io
-        [v3io]: https://www.iguazio.com/docs/tutorials/latest-release/getting-started/containers/
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# v3iofs
+
+<!--
+[![CI](https://github.com/v3io/v3io-fs/workflows/CI/badge.svg)](https://github.com/v3io/v3io-fs/actions?query=workflow%3ACI)
+-->
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+
+An [fsspec][fsspec] driver for [v3io][v3io].
+
+
+## Examples
+
+
+### Python
+
+```python
+>>> from v3iofs import V3ioFS  # Will register 'v3io' protocol in ffspec
+>>> fs = V3ioFS('api.app.yh48.iguazio-cd2.com', v3io_access_key='s3cr3t')
+>>> fs.ls('/container/path')
+```
+
+### Pandas
+
+```python
+# Use V3IO_ACCESS_KEY & V3IO_API from environment
+>> df = pd.read_csv('v3io://container/path/to/file.csv')
+```
+
+### Dask
+
+```python
+>>> from v3iofs import V3ioFS
+>>> from dask import bag
+
+# Use V3IO_ACCESS_KEY & V3IO_API from environment
+>>> url = 'v3io://container/path'
+>>> file = bag.read_text(url)
+>>> data, _ = file.compute()
+
+# Pass key in storage_options
+>>> storage_options={
+...     'v3io_api': 'webapi.app.iguazio.com',
+...     'v3io_access_key': 's3cr3t',
+... }
+>>> file = bag.read_text(url, storage_options=storage_options)
+>>> data, _ = file.compute()
+```
+
+## Development
+
+
+### Testing
+
+You need to set `V3IO_ACCESS_KEY` and `V3IO_API` environment variables.
+Then run `make test` to run the tests.
+
+
+### Environment
+
+Deployment requirements are in `requirements.txt` and development requirements
+are in `dev-requirements.txt`.
+
+```
+$ python -m venv venv
+$ ./venv/bin/python -m pip install -r dev-requirements.txt
+```
+
+
+[fsspec]: https://filesystem-spec.readthedocs.io
+[v3io]: https://www.iguazio.com/docs/tutorials/latest-release/getting-started/containers/
+
+
```

### Comparing `v3iofs-0.1.8/v3iofs.egg-info/SOURCES.txt` & `v3iofs-0.1.9/v3iofs.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.md
 dev-requirements.txt
 requirements.txt
+setup.cfg
 setup.py
 tests/Dockerfile
 tests/Dockerfile.fsspec-6
 tests/conftest.py
 tests/sanchez.pq
 tests/test_dask.py
 tests/test_file.py
```

### Comparing `v3iofs-0.1.8/Makefile` & `v3iofs-0.1.9/Makefile`

 * *Files 27% similar despite different names*

```diff
@@ -8,49 +8,56 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+.PHONY: all
 all:
 	$(error please pick a target)
 
-test:
-	find v3iofs -name '*.pyc' -exec rm {} \;
-	find tests -name '*.pyc' -exec rm {} \;
+.PHONY: lint
+lint:
 	flake8 v3iofs tests
+
+.PHONY: test
+test:
 	python -m pytest \
 	    -rf -v \
 	    --disable-warnings \
 	    --doctest-modules \
 	    tests v3iofs
 
+.PHONY: test-docker
 test-docker:
 	docker build \
 	    -f tests/Dockerfile \
 	    --rm \
 	    --build-arg V3IO_API=$(V3IO_API) \
 	    --build-arg V3IO_ACCESS_KEY=$(V3IO_ACCESS_KEY) \
 	    .
 
+.PHONY: test-docker-fsspec-6
 test-docker-fsspec-6:
 	docker build \
 	    -f tests/Dockerfile.fsspec-6 \
 	    --rm \
 	    --build-arg V3IO_API=$(V3IO_API) \
 	    --build-arg V3IO_ACCESS_KEY=$(V3IO_ACCESS_KEY) \
 	    .
 
-publish:
-	@echo Checking clean tree
-	test -z "$(shell git status -su)"
-	@echo "Checking for VERSION in environment (make publish VERSION=1.2.3)"
-	test -n "$(VERSION)"
-	sed -i "s/__version__ = '.*'/__version__ = '$(VERSION)'/" \
-	    v3iofs/__init__.py
-	git commit -m 'version $(VERSION)' v3iofs/__init__.py
-	rm -fr dist build
-	python setup.py sdist
-	python -m twine upload dist/*.tar.gz
-	git tag version-$(VERSION)
-	git push && git push --tags
+.PHONY: env
+env:
+	pip install -r requirements.txt
+
+.PHONY: dev-env
+dev-env: env
+	pip install -r dev-requirements.txt
+
+.PHONY: set-version
+set-version:
+	python set-version.py
+
+.PHONY: dist
+dist:
+	python -m build --sdist --wheel --outdir dist/ .
```

### Comparing `v3iofs-0.1.8/tests/conftest.py` & `v3iofs-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_setup.py` & `v3iofs-0.1.9/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_v3iofs.py` & `v3iofs-0.1.9/tests/test_v3iofs.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_fs.py` & `v3iofs-0.1.9/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_file.py` & `v3iofs-0.1.9/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/sanchez.pq` & `v3iofs-0.1.9/tests/sanchez.pq`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_dask.py` & `v3iofs-0.1.9/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_pandas.py` & `v3iofs-0.1.9/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_path.py` & `v3iofs-0.1.9/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/tests/test_install.py` & `v3iofs-0.1.9/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/README.md` & `v3iofs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/setup.py` & `v3iofs-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: MacOS',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Libraries',
     ],
     tests_require=tests_require,
```

### Comparing `v3iofs-0.1.8/v3iofs/__init__.py` & `v3iofs-0.1.9/v3iofs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 
 __all__ = [
     '__version__',
     'V3ioFS',
     'V3ioFile',
 ]
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 import fsspec
 
 from .file import V3ioFile  # noqa: F401
 from .fs import V3ioFS  # noqa: F401
 
 if hasattr(fsspec, 'register_implementation'):
     # TODO: Not sure about clobber=True
     fsspec.register_implementation('v3io', V3ioFS, clobber=True)
 else:
     from fsspec.registry import known_implementations
+
     known_implementations['v3io'] = {
         'class': 'v3iofs.V3ioFS',
         'err': 'Please install v3iofs to use the v3io fileysstem class'
     }
 
     del known_implementations
```

### Comparing `v3iofs-0.1.8/v3iofs/file.py` & `v3iofs-0.1.9/v3iofs/file.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/v3iofs/path.py` & `v3iofs-0.1.9/v3iofs/path.py`

 * *Files identical despite different names*

### Comparing `v3iofs-0.1.8/LICENSE.txt` & `v3iofs-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

