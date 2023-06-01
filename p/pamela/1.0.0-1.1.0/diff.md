# Comparing `tmp/pamela-1.0.0.tar.gz` & `tmp/pamela-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pamela-1.0.0.tar", last modified: Thu Jan 17 15:21:24 2019, max compression
+gzip compressed data, was "pamela-1.1.0.tar", last modified: Thu Jun  1 09:44:30 2023, max compression
```

## Comparing `pamela-1.0.0.tar` & `pamela-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 benjaminrk   (501) staff       (20)        0 2019-01-17 15:21:24.000000 pamela-1.0.0/
--rw-r--r--   0 benjaminrk   (501) staff       (20)     1738 2019-01-17 15:21:24.000000 pamela-1.0.0/PKG-INFO
--rw-r--r--   0 benjaminrk   (501) staff       (20)       34 2015-09-08 12:25:25.000000 pamela-1.0.0/MANIFEST.in
--rw-r--r--   0 benjaminrk   (501) staff       (20)      813 2015-09-09 11:08:35.000000 pamela-1.0.0/README.md
--rw-r--r--   0 benjaminrk   (501) staff       (20)     1326 2015-09-08 11:50:52.000000 pamela-1.0.0/COPYING
--rw-r--r--   0 benjaminrk   (501) staff       (20)     1736 2019-01-17 15:19:41.000000 pamela-1.0.0/setup.py
-drwxr-xr-x   0 benjaminrk   (501) staff       (20)        0 2019-01-17 15:21:24.000000 pamela-1.0.0/pamela.egg-info/
--rw-r--r--   0 benjaminrk   (501) staff       (20)     1738 2019-01-17 15:21:24.000000 pamela-1.0.0/pamela.egg-info/PKG-INFO
--rw-r--r--   0 benjaminrk   (501) staff       (20)      178 2019-01-17 15:21:24.000000 pamela-1.0.0/pamela.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminrk   (501) staff       (20)        7 2019-01-17 15:21:24.000000 pamela-1.0.0/pamela.egg-info/top_level.txt
--rw-r--r--   0 benjaminrk   (501) staff       (20)        1 2019-01-17 15:21:24.000000 pamela-1.0.0/pamela.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminrk   (501) staff       (20)       67 2019-01-17 15:21:24.000000 pamela-1.0.0/setup.cfg
--rw-r--r--   0 benjaminrk   (501) staff       (20)    15137 2019-01-17 15:21:23.000000 pamela-1.0.0/pamela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:44:30.341100 pamela-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-01 09:44:19.000000 pamela-1.1.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 09:44:19.000000 pamela-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 09:44:30.341100 pamela-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 09:44:19.000000 pamela-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 09:44:30.341100 pamela-1.1.0/pamela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-01 09:44:30.000000 pamela-1.1.0/pamela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-01 09:44:30.000000 pamela-1.1.0/pamela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 09:44:30.000000 pamela-1.1.0/pamela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 09:44:30.000000 pamela-1.1.0/pamela.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-01 09:44:19.000000 pamela-1.1.0/pamela.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-01 09:44:19.000000 pamela-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 09:44:30.341100 pamela-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-01 09:44:19.000000 pamela-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pamela-1.0.0/PKG-INFO` & `pamela-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: pamela
-Version: 1.0.0
+Version: 1.1.0
 Summary: PAM interface using ctypes
 Home-page: https://github.com/minrk/pamela
 Author: Min RK
 Author-email: benjaminrk@gmail.com
 License: MIT
-Description: # Pamela: yet another Python wrapper for PAM
-        
-        There seems to be a glut of Python wrappers for PAM that have since been abandoned.
-        This repo merges two separate efforts:
-        
-        - [gnosek/python-pam](https://github.com/gnosek/python-pam)
-          - adds wrappers for a few more calls, e.g. opening sessions
-          - raises PamError on failure instead of returning False, with informative error messages
-        - [simplepam](https://github.com/leonnnn/python3-simplepam)
-          - adds Python 3 support
-          - resets credentials after authentication, apparently for kerberos users
-        
-        ## Why?
-        
-        Both projects appear to be abandoned, with no response to issues or pull requests in at least a year, and I need it for [JupyterHub](https://github.com/jupyter/jupyterhub).
-        
-        ## Use it
-        
-        Install:
-        
-            pip install pamela
-        
-        Test:
-        
-            python -m pamela -a `whoami`
-        
 Keywords: pam,authentication
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Description-Content-Type: text/markdown
+License-File: COPYING
+
+# Pamela: yet another Python wrapper for PAM
+
+There seems to be a glut of Python wrappers for PAM that have since been abandoned.
+This repo merges two separate efforts:
+
+- [gnosek/python-pam](https://github.com/gnosek/python-pam)
+  - adds wrappers for a few more calls, e.g. opening sessions
+  - raises PamError on failure instead of returning False, with informative error messages
+- [simplepam](https://github.com/leonnnn/python3-simplepam)
+  - adds Python 3 support
+  - resets credentials after authentication, apparently for kerberos users
+
+## Why?
+
+Both projects appear to be abandoned, with no response to issues or pull requests in at least a year, and I need it for [JupyterHub](https://github.com/jupyter/jupyterhub).
+
+## Use it
+
+Install:
+
+    pip install pamela
+
+Test:
+
+    python -m pamela -a `whoami`
```

### Comparing `pamela-1.0.0/README.md` & `pamela-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pamela-1.0.0/COPYING` & `pamela-1.1.0/COPYING`

 * *Files identical despite different names*

### Comparing `pamela-1.0.0/setup.py` & `pamela-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,50 +5,55 @@
 """
 
 import sys
 
 from setuptools import setup
 from setuptools.command.bdist_egg import bdist_egg
 
+
 class bdist_egg_disabled(bdist_egg):
     """Disabled version of bdist_egg
 
     Prevents setup.py install from performing setuptools' default easy_install,
     which it should never ever do.
     """
+
     def run(self):
-        sys.exit("Aborting implicit building of eggs. Use `pip install .` to install from source.")
+        sys.exit(
+            "Aborting implicit building of eggs. Use `pip install .` to install from source."
+        )
 
 
 with open('pamela.py') as f:
     for line in f:
         if line.startswith('__version__'):
             version_ns = {}
             exec(line, version_ns)
             version = version_ns['__version__']
 
 
-setup(name='pamela',
-      version=version,
-      description="PAM interface using ctypes",
-      long_description=open("README.md").read(),
-      long_description_content_type="text/markdown",
-      classifiers=[
-          "Development Status :: 4 - Beta",
-          "Intended Audience :: Developers",
-          "License :: OSI Approved :: MIT License",
-          "Operating System :: POSIX :: Linux",
-          "Operating System :: MacOS :: MacOS X",
-          "Programming Language :: Python",
-          "Topic :: Software Development :: Libraries :: Python Modules",
-          "Topic :: System :: Systems Administration :: Authentication/Directory"
-          ],
-      cmdclass={
-          "bdist_egg": bdist_egg if "bdist_egg" in sys.argv else bdist_egg_disabled,
-      },
-      keywords=['pam', 'authentication'],
-      author='Min RK',
-      author_email='benjaminrk@gmail.com',
-      url='https://github.com/minrk/pamela',
-      license='MIT',
-      py_modules=["pamela"],
+setup(
+    name='pamela',
+    version=version,
+    description="PAM interface using ctypes",
+    long_description=open("README.md").read(),
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: POSIX :: Linux",
+        "Operating System :: MacOS :: MacOS X",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Topic :: System :: Systems Administration :: Authentication/Directory",
+    ],
+    cmdclass={
+        "bdist_egg": bdist_egg if "bdist_egg" in sys.argv else bdist_egg_disabled,
+    },
+    keywords=['pam', 'authentication'],
+    author='Min RK',
+    author_email='benjaminrk@gmail.com',
+    url='https://github.com/minrk/pamela',
+    license='MIT',
+    py_modules=["pamela"],
 )
```

### Comparing `pamela-1.0.0/pamela.egg-info/PKG-INFO` & `pamela-1.1.0/pamela.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: pamela
-Version: 1.0.0
+Version: 1.1.0
 Summary: PAM interface using ctypes
 Home-page: https://github.com/minrk/pamela
 Author: Min RK
 Author-email: benjaminrk@gmail.com
 License: MIT
-Description: # Pamela: yet another Python wrapper for PAM
-        
-        There seems to be a glut of Python wrappers for PAM that have since been abandoned.
-        This repo merges two separate efforts:
-        
-        - [gnosek/python-pam](https://github.com/gnosek/python-pam)
-          - adds wrappers for a few more calls, e.g. opening sessions
-          - raises PamError on failure instead of returning False, with informative error messages
-        - [simplepam](https://github.com/leonnnn/python3-simplepam)
-          - adds Python 3 support
-          - resets credentials after authentication, apparently for kerberos users
-        
-        ## Why?
-        
-        Both projects appear to be abandoned, with no response to issues or pull requests in at least a year, and I need it for [JupyterHub](https://github.com/jupyter/jupyterhub).
-        
-        ## Use it
-        
-        Install:
-        
-            pip install pamela
-        
-        Test:
-        
-            python -m pamela -a `whoami`
-        
 Keywords: pam,authentication
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Description-Content-Type: text/markdown
+License-File: COPYING
+
+# Pamela: yet another Python wrapper for PAM
+
+There seems to be a glut of Python wrappers for PAM that have since been abandoned.
+This repo merges two separate efforts:
+
+- [gnosek/python-pam](https://github.com/gnosek/python-pam)
+  - adds wrappers for a few more calls, e.g. opening sessions
+  - raises PamError on failure instead of returning False, with informative error messages
+- [simplepam](https://github.com/leonnnn/python3-simplepam)
+  - adds Python 3 support
+  - resets credentials after authentication, apparently for kerberos users
+
+## Why?
+
+Both projects appear to be abandoned, with no response to issues or pull requests in at least a year, and I need it for [JupyterHub](https://github.com/jupyter/jupyterhub).
+
+## Use it
+
+Install:
+
+    pip install pamela
+
+Test:
+
+    python -m pamela -a `whoami`
```

### Comparing `pamela-1.0.0/pamela.py` & `pamela-1.1.0/pamela.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,42 +7,53 @@
 PAM module for python
 
 Provides an authenticate function that will allow the caller to authenticate
 a user against the Pluggable Authentication Modules (PAM) on the system.
 
 Implemented using ctypes, so no compilation is necessary.
 """
-from __future__ import print_function
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 
 __all__ = [
     'PAMError',
     'authenticate',
     'open_session',
     'close_session',
     'check_account',
     'change_password',
 ]
 
-from ctypes import CDLL, POINTER, Structure, CFUNCTYPE, cast, pointer, sizeof, byref
-from ctypes import c_void_p, c_uint, c_char_p, c_char, c_int
-from ctypes.util import find_library
 import getpass
 import sys
+from ctypes import (
+    CDLL,
+    CFUNCTYPE,
+    POINTER,
+    Structure,
+    byref,
+    c_char,
+    c_char_p,
+    c_int,
+    c_uint,
+    c_void_p,
+    cast,
+    pointer,
+    sizeof,
+)
+from ctypes.util import find_library
 
 # Python 3 bytes/unicode compat
-if sys.version_info >= (3,):
-    unicode = str
-    raw_input = input
-    def _bytes_to_str(s, encoding='utf8'):
-        return s.decode(encoding)
-else:
-    def _bytes_to_str(s, encoding='utf8'):
-        return s
+unicode = str
+raw_input = input
+
+
+def _bytes_to_str(s, encoding='utf8'):
+    return s.decode(encoding)
+
 
 def _cast_bytes(s, encoding='utf8'):
     if isinstance(s, unicode):
         return s.encode(encoding)
     return s
 
 
@@ -51,15 +62,15 @@
 
 CALLOC = LIBC.calloc
 CALLOC.restype = c_void_p
 CALLOC.argtypes = [c_uint, c_uint]
 
 STRDUP = LIBC.strdup
 STRDUP.argstypes = [c_char_p]
-STRDUP.restype = POINTER(c_char) # NOT c_char_p !!!!
+STRDUP.restype = POINTER(c_char)  # NOT c_char_p !!!!
 
 # Various constants
 PAM_PROMPT_ECHO_OFF = 1
 PAM_PROMPT_ECHO_ON = 2
 PAM_ERROR_MSG = 3
 PAM_TEXT_INFO = 4
 
@@ -79,17 +90,16 @@
 # PAM error codes
 PAM_SUCCESS = 0
 PAM_BAD_ITEM = 29
 
 
 class PamHandle(Structure):
     """wrapper class for pam_handle_t"""
-    _fields_ = [
-            ("handle", c_void_p)
-            ]
+
+    _fields_ = [("handle", c_void_p)]
 
     def __init__(self):
         Structure.__init__(self)
         self.handle = 0
 
     def get_item(self, item_type, encoding='utf-8'):
         voidPointer = c_void_p()
@@ -113,24 +123,20 @@
         ret = PAM_GETENV(self, var.encode(encoding))
         if ret is None:
             raise PAMError()
         else:
             return ret.decode(encoding)
 
     def put_env(self, k, v, encoding='utf-8'):
-        retval = PAM_PUTENV(
-            self,
-            ('%s=%s' % (k, v)).encode(encoding))
+        retval = PAM_PUTENV(self, (f'{k}={v}').encode(encoding))
         if retval != PAM_SUCCESS:
             raise PAMError(errno=retval)
 
     def del_env(self, k, encoding='utf-8'):
-        retval = PAM_PUTENV(
-            self,
-            k.encode(encoding))
+        retval = PAM_PUTENV(self, k.encode(encoding))
         if retval != PAM_SUCCESS:
             raise PAMError(errno=retval)
 
     def get_envlist(self, encoding='utf-8'):
         ret = PAM_GETENVLIST(self)
         if ret is None:
             raise PAMError()
@@ -155,74 +161,81 @@
             raise PAMError(errno=retval)
 
 
 PAM_STRERROR = LIBPAM.pam_strerror
 PAM_STRERROR.restype = c_char_p
 PAM_STRERROR.argtypes = [PamHandle, c_int]
 
+
 def pam_strerror(handle, errno):
     """Wrap bytes-only PAM_STRERROR in native str"""
     return _bytes_to_str(PAM_STRERROR(handle, errno))
 
+
 class PAMError(Exception):
     errno = None
     message = ''
+
     def __init__(self, message='', errno=None):
         self.errno = errno
         if message:
             self.message = message
         else:
             if errno is None:
                 self.message = "Unknown"
             else:
                 self.message = pam_strerror(PamHandle(), errno)
 
     def __repr__(self):
         en = '' if self.errno is None else ' %i' % self.errno
-        return "<PAM Error%s: '%s'>" % (en, self.message)
+        return f"<PAM Error{en}: '{self.message}'>"
 
     def __str__(self):
         en = '' if self.errno is None else ' %i' % self.errno
-        return '[PAM Error%s] %s' % (en, self.message)
+        return f'[PAM Error{en}] {self.message}'
+
 
 class PamMessage(Structure):
     """wrapper class for pam_message structure"""
+
     _fields_ = [
-            ("msg_style", c_int),
-            ("msg", POINTER(c_char)),
-            ]
+        ("msg_style", c_int),
+        ("msg", POINTER(c_char)),
+    ]
 
     def __repr__(self):
         return "<PamMessage %i '%s'>" % (self.msg_style, _bytes_to_str(self.msg))
 
+
 class PamResponse(Structure):
     """wrapper class for pam_response structure"""
+
     _fields_ = [
-            ("resp", POINTER(c_char)),
-            ("resp_retcode", c_int),
-            ]
+        ("resp", POINTER(c_char)),
+        ("resp_retcode", c_int),
+    ]
 
     def __repr__(self):
         return "<PamResponse %i '%s'>" % (self.resp_retcode, _bytes_to_str(self.resp))
 
-CONV_FUNC = CFUNCTYPE(c_int,
-        c_int, POINTER(POINTER(PamMessage)),
-               POINTER(POINTER(PamResponse)), c_void_p)
+
+CONV_FUNC = CFUNCTYPE(
+    c_int, c_int, POINTER(POINTER(PamMessage)), POINTER(POINTER(PamResponse)), c_void_p
+)
+
 
 class PamConv(Structure):
     """wrapper class for pam_conv structure"""
-    _fields_ = [
-            ("conv", CONV_FUNC),
-            ("appdata_ptr", c_void_p)
-            ]
+
+    _fields_ = [("conv", CONV_FUNC), ("appdata_ptr", c_void_p)]
+
 
 PAM_START = LIBPAM.pam_start
 PAM_START.restype = c_int
-PAM_START.argtypes = [c_char_p, c_char_p, POINTER(PamConv),
-        POINTER(PamHandle)]
+PAM_START.argtypes = [c_char_p, c_char_p, POINTER(PamConv), POINTER(PamHandle)]
 
 PAM_END = LIBPAM.pam_end
 PAM_END.restype = c_int
 PAM_END.argtypes = [PamHandle, c_int]
 
 PAM_AUTHENTICATE = LIBPAM.pam_authenticate
 PAM_AUTHENTICATE.restype = c_int
@@ -264,14 +277,15 @@
 PAM_SET_ITEM.restype = c_int
 PAM_SET_ITEM.argtypes = [PamHandle, c_int, c_char_p]
 
 PAM_GET_ITEM = LIBPAM.pam_get_item
 PAM_GET_ITEM.restype = c_int
 PAM_GET_ITEM.argtypes = [PamHandle, c_int, POINTER(c_void_p)]
 
+
 @CONV_FUNC
 def default_conv(n_messages, messages, p_response, app_data):
     addr = CALLOC(n_messages, sizeof(PamResponse))
     p_response[0] = cast(addr, POINTER(PamResponse))
     if not sys.stdin.isatty():
         return 0
     for i in range(n_messages):
@@ -292,17 +306,19 @@
             pw_copy = STRDUP(_cast_bytes(read_pw(msg_string)))
             p_response.contents[i].resp = pw_copy
             p_response.contents[i].resp_retcode = 0
         else:
             print(repr(messages[i].contents))
     return 0
 
+
 def new_simple_password_conv(passwords, encoding):
     passwords = [_cast_bytes(password, encoding) for password in passwords]
     passwords.reverse()
+
     @CONV_FUNC
     def conv_func(n_messages, messages, p_response, app_data):
         """Simple conversation function that responds to any
         prompt where the echo is off with the supplied password"""
         # Create an array of n_messages response objects
         addr = CALLOC(n_messages, sizeof(PamResponse))
         p_response[0] = cast(addr, POINTER(PamResponse))
@@ -310,46 +326,57 @@
             if messages[i].contents.msg_style == PAM_PROMPT_ECHO_OFF:
                 if not passwords:
                     return 1
                 pw_copy = STRDUP(passwords.pop())
                 p_response.contents[i].resp = pw_copy
                 p_response.contents[i].resp_retcode = 0
         return 0
+
     return conv_func
 
+
 def pam_start(service, username, conv_func=default_conv, encoding='utf8'):
     service = _cast_bytes(service, encoding)
     username = _cast_bytes(username, encoding)
 
     handle = PamHandle()
     conv = pointer(PamConv(conv_func, 0))
     retval = PAM_START(service, username, conv, pointer(handle))
 
     if retval != 0:
         PAM_END(handle, retval)
         raise PAMError(errno=retval)
 
     return handle
 
+
 def pam_end(handle, retval=0):
     e = PAM_END(handle, retval)
     if retval == 0 and e == 0:
         return
     if retval == 0:
         retval = e
     raise PAMError(errno=retval)
 
-def authenticate(username, password=None, service='login', encoding='utf-8',
-                 resetcred=PAM_REINITIALIZE_CRED, close=True):
+
+def authenticate(
+    username,
+    password=None,
+    service='login',
+    encoding='utf-8',
+    resetcred=PAM_REINITIALIZE_CRED,
+    close=True,
+):
     """Returns None if the given username and password authenticate for the
     given service.  Raises PAMError otherwise
 
     ``username``: the username to authenticate
 
-    ``password``: the password in plain text
+    ``password``: the password in plain text. It can also be an iterable of
+                  passwords when using multifactor authentication.
                   Defaults to None to use PAM's conversation interface
 
     ``service``: the PAM service to authenticate against.
                  Defaults to 'login'
 
     The above parameters can be strings or bytes.  If they are strings,
     they will be encoded using the encoding given by:
@@ -365,16 +392,17 @@
                    authentication; if False the (open) PamHandle instance
                    will be returned.
     """
 
     if password is None:
         conv_func = default_conv
     else:
-        password = _cast_bytes(password, encoding)
-        conv_func = new_simple_password_conv((password, ), encoding)
+        if isinstance(password, str):
+            password = (password,)
+        conv_func = new_simple_password_conv(password, encoding)
 
     handle = pam_start(service, username, conv_func=conv_func, encoding=encoding)
 
     retval = PAM_AUTHENTICATE(handle, 0)
     # Re-initialize credentials (for Kerberos users, etc)
     # Don't check return code of pam_setcred(), it shouldn't matter
     # if this fails
@@ -384,66 +412,108 @@
     if close:
         return pam_end(handle, retval)
     elif retval != 0:
         raise PAMError(errno=retval)
     else:
         return handle
 
+
 def open_session(username, service='login', encoding='utf-8'):
     handle = pam_start(service, username, encoding=encoding)
     return pam_end(handle, PAM_OPEN_SESSION(handle, 0))
 
+
 def close_session(username, service='login', encoding='utf-8'):
     handle = pam_start(service, username, encoding=encoding)
     return pam_end(handle, PAM_CLOSE_SESSION(handle, 0))
 
+
 def check_account(username, service='login', encoding='utf-8'):
     handle = pam_start(service, username, encoding=encoding)
     return pam_end(handle, PAM_ACCT_MGMT(handle, 0))
 
+
 def change_password(username, password=None, service='login', encoding='utf-8'):
     if password is None:
         conv_func = default_conv
     else:
         # Password x2 to answer the "Retype new UNIX password:" prompt
         # TODO: If we're not running as root the first prompt will be
         # 'current password' which we will not answer, so this will not work
         # in that case.
         conv_func = new_simple_password_conv((password, password), encoding)
     handle = pam_start(service, username, conv_func=conv_func, encoding=encoding)
     return pam_end(handle, PAM_CHAUTHTOK(handle, 0))
 
+
 if __name__ == "__main__":
     import optparse
 
     usage = "usage: %prog [options] [username]"
     parser = optparse.OptionParser(usage=usage)
-    parser.add_option('-a', '--authenticate', dest='authenticate',
-        action='store_true', help='authenticate user')
-    parser.add_option('-o', '--open-session', dest='open_session',
-        action='store_true', help='open session')
-    parser.add_option('-c', '--close-session', dest='close_session',
-        action='store_true', help='close session')
-    parser.add_option('-v', '--validate-account', dest='validate_account',
-        action='store_true', help='check account validity')
-    parser.add_option('-p', '--change-password', dest='change_password',
-        action='store_true', help='change password')
-    parser.add_option('-s', '--service', dest='service',
-        action='store', default='login',
-        help='PAM service to use [default: %default]')
-    parser.add_option('-P', '--ask-password', dest='ask_password',
-        action='store_true', help="own password prompt instead of PAM's")
+    parser.add_option(
+        '-a',
+        '--authenticate',
+        dest='authenticate',
+        action='store_true',
+        help='authenticate user',
+    )
+    parser.add_option(
+        '-o',
+        '--open-session',
+        dest='open_session',
+        action='store_true',
+        help='open session',
+    )
+    parser.add_option(
+        '-c',
+        '--close-session',
+        dest='close_session',
+        action='store_true',
+        help='close session',
+    )
+    parser.add_option(
+        '-v',
+        '--validate-account',
+        dest='validate_account',
+        action='store_true',
+        help='check account validity',
+    )
+    parser.add_option(
+        '-p',
+        '--change-password',
+        dest='change_password',
+        action='store_true',
+        help='change password',
+    )
+    parser.add_option(
+        '-s',
+        '--service',
+        dest='service',
+        action='store',
+        default='login',
+        help='PAM service to use [default: %default]',
+    )
+    parser.add_option(
+        '-P',
+        '--ask-password',
+        dest='ask_password',
+        action='store_true',
+        help="own password prompt instead of PAM's",
+    )
 
     (o, a) = parser.parse_args()
 
-    if not (o.authenticate or \
-        o.open_session or \
-        o.close_session or \
-        o.validate_account or \
-        o.change_password):
+    if not (
+        o.authenticate
+        or o.open_session
+        or o.close_session
+        or o.validate_account
+        or o.change_password
+    ):
         parser.error("One of -a, -o, -c, -v or -p is mandatory")
 
     try:
         user = a[0]
     except IndexError:
         user = getpass.getuser()
```

