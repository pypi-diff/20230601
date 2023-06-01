# Comparing `tmp/pymsbuild-0.2.2.tar.gz` & `tmp/pymsbuild-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymsbuild-0.2.2.tar", last modified: Fri Mar 31 13:29:36 2023, max compression
+gzip compressed data, was "pymsbuild-1.0.0a1.tar", last modified: Thu Jun  1 00:08:11 2023, max compression
```

## Comparing `pymsbuild-0.2.2.tar` & `pymsbuild-1.0.0a1.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 13:29:35.842613 pymsbuild-0.2.2/
--rw-rw-rw-   0        0        0    19715 2023-03-31 13:29:09.319762 pymsbuild-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2222 2023-03-31 13:28:29.515927 pymsbuild-0.2.2/_msbuild.py
-drwxrwxrwx   0        0        0        0 2023-03-31 13:29:35.842613 pymsbuild-0.2.2/pymsbuild/
--rw-rw-rw-   0        0        0     1012 2023-03-31 13:28:29.515927 pymsbuild-0.2.2/pymsbuild/__init__.py
--rw-rw-rw-   0        0        0     3855 2023-03-31 13:28:29.515927 pymsbuild-0.2.2/pymsbuild/__main__.py
--rw-rw-rw-   0        0        0    23950 2023-03-31 13:28:29.524439 pymsbuild-0.2.2/pymsbuild/_build.py
--rw-rw-rw-   0        0        0    11807 2023-03-31 13:28:29.524439 pymsbuild-0.2.2/pymsbuild/_generate.py
--rw-rw-rw-   0        0        0     4892 2023-03-31 13:28:29.524439 pymsbuild-0.2.2/pymsbuild/_init.py
--rw-rw-rw-   0        0        0     1505 2023-03-31 13:28:29.524439 pymsbuild-0.2.2/pymsbuild/_load_sysconfig.py
--rw-rw-rw-   0        0        0      802 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/_locate_dotnet.py
--rw-rw-rw-   0        0        0     1956 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/_locate_vs.py
--rw-rw-rw-   0        0        0     1893 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/_msbuild.py.in
--rw-rw-rw-   0        0        0     5417 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/_tags.py
--rw-rw-rw-   0        0        0     8385 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/_types.py
--rw-rw-rw-   0        0        0     5557 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/_writer.py
--rw-rw-rw-   0        0        0      735 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/cython.py
--rw-rw-rw-   0        0        0     1276 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/dllpack.py
--rw-rw-rw-   0        0        0       74 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/pyproject.toml.in
-drwxrwxrwx   0        0        0        0 2023-03-31 13:29:35.858181 pymsbuild-0.2.2/pymsbuild/targets/
--rw-rw-rw-   0        0        0     1013 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/common.props
--rw-rw-rw-   0        0        0     5785 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/common.targets
--rw-rw-rw-   0        0        0      119 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-ARM.props
--rw-rw-rw-   0        0        0      197 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-ARM.targets
--rw-rw-rw-   0        0        0      119 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-ARM64.props
--rw-rw-rw-   0        0        0      197 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-ARM64.targets
--rw-rw-rw-   0        0        0      367 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-POSIX_x64-GCC.props
--rw-rw-rw-   0        0        0      232 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-POSIX_x64.props
--rw-rw-rw-   0        0        0     3464 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-POSIX_x64.targets
--rw-rw-rw-   0        0        0      119 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-Win32.props
--rw-rw-rw-   0        0        0      197 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-Win32.targets
--rw-rw-rw-   0        0        0      127 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-default-ARM.props
--rw-rw-rw-   0        0        0      127 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-default-ARM64.props
--rw-rw-rw-   0        0        0      120 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-default-POSIX_x64.props
--rw-rw-rw-   0        0        0      127 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-default-Win32.props
--rw-rw-rw-   0        0        0      127 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-default-x64.props
--rw-rw-rw-   0        0        0      119 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-x64.props
--rw-rw-rw-   0        0        0      197 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cpp-x64.targets
--rw-rw-rw-   0        0        0     3869 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/cython.targets
--rw-rw-rw-   0        0        0     6430 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/dllpack-generate.py
--rw-rw-rw-   0        0        0    11010 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/dllpack.c
--rw-rw-rw-   0        0        0     1602 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/dllpack.targets
--rw-rw-rw-   0        0        0     2506 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/dllpack_main.py
--rw-rw-rw-   0        0        0       23 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/package.targets
--rw-rw-rw-   0        0        0      929 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/pyd.props
--rw-rw-rw-   0        0        0      515 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/pyd.targets
--rw-rw-rw-   0        0        0     1840 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pymsbuild/targets/sdist.targets
--rw-rw-rw-   0        0        0       71 2023-03-31 13:28:29.525983 pymsbuild-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0    19717 2023-06-01 00:07:40.031116 PKG-INFO
+-rw-rw-rw-   0        0        0       71 2023-06-01 00:06:39.699320 pyproject.toml
+-rw-rw-rw-   0        0        0     2222 2023-06-01 00:06:39.699320 _msbuild.py
+-rw-rw-rw-   0        0        0      936 2023-06-01 00:06:39.699320 pymsbuild/cython.py
+-rw-rw-rw-   0        0        0     1276 2023-06-01 00:06:39.699320 pymsbuild/dllpack.py
+-rw-rw-rw-   0        0        0       74 2023-06-01 00:06:39.699320 pymsbuild/pyproject.toml.in
+-rw-rw-rw-   0        0        0    21286 2023-06-01 00:06:39.699320 pymsbuild/_build.py
+-rw-rw-rw-   0        0        0    11558 2023-06-01 00:06:39.699320 pymsbuild/_generate.py
+-rw-rw-rw-   0        0        0     4892 2023-06-01 00:06:39.699320 pymsbuild/_init.py
+-rw-rw-rw-   0        0        0     1505 2023-06-01 00:06:39.699320 pymsbuild/_load_sysconfig.py
+-rw-rw-rw-   0        0        0      802 2023-06-01 00:06:39.699320 pymsbuild/_locate_dotnet.py
+-rw-rw-rw-   0        0        0     1956 2023-06-01 00:06:39.699320 pymsbuild/_locate_vs.py
+-rw-rw-rw-   0        0        0     2013 2023-06-01 00:06:39.699320 pymsbuild/_msbuild.py.in
+-rw-rw-rw-   0        0        0     5417 2023-06-01 00:06:39.699320 pymsbuild/_tags.py
+-rw-rw-rw-   0        0        0     8560 2023-06-01 00:06:39.699320 pymsbuild/_types.py
+-rw-rw-rw-   0        0        0     5557 2023-06-01 00:06:39.699320 pymsbuild/_writer.py
+-rw-rw-rw-   0        0        0     1225 2023-06-01 00:06:39.699320 pymsbuild/__init__.py
+-rw-rw-rw-   0        0        0     4047 2023-06-01 00:06:39.699320 pymsbuild/__main__.py
+-rw-rw-rw-   0        0        0      973 2023-06-01 00:06:39.699320 pymsbuild/targets/common.props
+-rw-rw-rw-   0        0        0     4143 2023-06-01 00:06:39.699320 pymsbuild/targets/common.targets
+-rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM.props
+-rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM.targets
+-rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM64.props
+-rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-ARM64.targets
+-rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-ARM.props
+-rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-ARM64.props
+-rw-rw-rw-   0        0        0      120 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-POSIX_x64.props
+-rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-Win32.props
+-rw-rw-rw-   0        0        0      127 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-default-x64.props
+-rw-rw-rw-   0        0        0      367 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-POSIX_x64-GCC.props
+-rw-rw-rw-   0        0        0      232 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-POSIX_x64.props
+-rw-rw-rw-   0        0        0     3572 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-POSIX_x64.targets
+-rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-Win32.props
+-rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-Win32.targets
+-rw-rw-rw-   0        0        0      119 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-x64.props
+-rw-rw-rw-   0        0        0      690 2023-06-01 00:06:39.699320 pymsbuild/targets/cpp-x64.targets
+-rw-rw-rw-   0        0        0     3921 2023-06-01 00:06:39.699320 pymsbuild/targets/cython.targets
+-rw-rw-rw-   0        0        0     6430 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack-generate.py
+-rw-rw-rw-   0        0        0    11010 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack.c
+-rw-rw-rw-   0        0        0     1835 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack.targets
+-rw-rw-rw-   0        0        0     2506 2023-06-01 00:06:39.699320 pymsbuild/targets/dllpack_main.py
+-rw-rw-rw-   0        0        0      292 2023-06-01 00:06:39.699320 pymsbuild/targets/package.override.targets
+-rw-rw-rw-   0        0        0       23 2023-06-01 00:06:39.699320 pymsbuild/targets/package.props
+-rw-rw-rw-   0        0        0     5390 2023-06-01 00:06:39.699320 pymsbuild/targets/package.targets
+-rw-rw-rw-   0        0        0      935 2023-06-01 00:06:39.699320 pymsbuild/targets/pyd.props
+-rw-rw-rw-   0        0        0      917 2023-06-01 00:06:39.699320 pymsbuild/targets/pyd.targets
+-rw-rw-rw-   0        0        0       23 2023-06-01 00:06:39.699320 pymsbuild/targets/sdist.targets
```

### Comparing `pymsbuild-0.2.2/PKG-INFO` & `PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymsbuild
-Version: 0.2.2
+Version: 1.0.0a1
 Author: Steve Dower
 Author-email: steve.dower@python.org
 Home-page: https://github.com/zooba/pymsbuild
 Project-url: Bug Tracker, https://github.com/zooba/pymsbuild/issues
 Summary: The pymsbuild build backend.
 Description-Content-Type: text/markdown
 Keywords: build,pep-517,msbuild,packaging,cython
```

### Comparing `pymsbuild-0.2.2/_msbuild.py` & `_msbuild.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/__init__.py` & `pymsbuild/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """The pymsbuild build backend.
 """
 
 __version__ = "%VERSION%"
+try:
+    NEXT_INCOMPATIBLE_VERSION = "{}.0".format(int(__version__.partition(".")[0]) + 1)
+    PYMSBUILD_REQUIRES_SPEC = f"pymsbuild>={__version__},<{NEXT_INCOMPATIBLE_VERSION}"
+except ValueError:
+    PYMSBUILD_REQUIRES_SPEC = "pymsbuild"
 
-PYMSBUILD_REQUIRES_SPEC = f"pymsbuild>={__version__},<1.0"
 
 from pymsbuild._build import BuildState as _BuildState
 from pymsbuild._types import *
 
 
 def get_current_build_state():
     return _BuildState.current
@@ -21,15 +25,16 @@
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
     bs = _BuildState(wheel_directory)
     return bs.build_wheel()
 
 
 def prepare_metadata_for_build_wheel(metadata_directory, config_settings=None):
     bs = _BuildState(metadata_directory)
-    return bs.prepare_wheel_distinfo(bs.output_dir)
+    bs.metadata_dir = metadata_directory
+    return bs.prepare_wheel_distinfo()
 
 
 def get_requires_for_build_sdist(config_settings=None):
     bs = _BuildState()
     return bs.get_requires_for_build_sdist()
```

### Comparing `pymsbuild-0.2.2/pymsbuild/__main__.py` & `pymsbuild/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -121,25 +121,35 @@
     sys.exit(0)
 
 bs = BuildState()
 bs.source_dir = Path.cwd() / (ns.source_dir or "")
 bs.output_dir = bs.source_dir / (ns.dist_dir or "dist")
 bs.config_file = ns.config
 root_dir = bs.source_dir / (ns.temp_dir or "build")
-bs.build_dir = root_dir / "layout"
+bs.build_dir = root_dir / "bin"
 bs.temp_dir = root_dir / "temp"
 bs.layout_dir = ns.layout_dir
 bs.layout_extra_files = ns.add
 bs.verbose = ns.verbose
 bs.quiet = ns.quiet
 bs.force = ns.force
 if ns.debug:
     bs.configuration = "Debug"
 
-for cmd in ns.command:
-    cmd = {
+if ns.layout_dir:
+    COMMANDS = {
+        "sdist": "layout_sdist",
+        "wheel": "layout_wheel",
+        "distinfo": "prepare_wheel_distinfo",
+    }
+else:
+    COMMANDS = {
         "sdist": "build_sdist",
         "wheel": "build_wheel",
         "distinfo": "prepare_wheel_distinfo",
-    }.get(cmd, cmd)
+    }
+
+
+for cmd in ns.command:
+    cmd = COMMANDS.get(cmd, cmd)
     f = getattr(bs, cmd)
     f()
```

### Comparing `pymsbuild-0.2.2/pymsbuild/_build.py` & `pymsbuild/_build.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,27 +40,40 @@
             hashalg,
             base64.urlsafe_b64encode(hasher.digest()).rstrip(b"=").decode(),
             l,
         )
     return "{},,".format(relpath)
 
 
+def _relative_to_layout(files, root):
+    if not files:
+        files = root.rglob("**/*")
+    for n in files:
+        n = root / n
+        try:
+            rn = n.relative_to(root)
+        except ValueError:
+            self.write("Not including", n, "from outside of layout directory")
+            continue
+        if n.is_file():
+            yield n, rn
+
+
 def _quote(s, start='"', end='"'):
     if end and s.endswith("\\"):
         end = "\\" + end
     return start + s + end
 
 
 class BuildState:
     # Updated around init_METADATA and init_PACKAGE calls
     current = None
 
     def __init__(self, output_dir=None):
         self._finalized = False
-        self._is_sdist = False
         self.verbose = False
         self.quiet = False
         self.force = False
         self.config = None
         self.package = None
         self.metadata = None
         self.project = None
@@ -68,39 +81,46 @@
         self.target = None
         self.msbuild_exe = None
         self.output_dir = Path(output_dir) if output_dir else None
         self.build_dir = None
         self.temp_dir = None
         self.layout_dir = None
         self.layout_extra_files = []
+        self.metadata_dir = None
         self.pkginfo = None
         self.source_dir = Path.cwd()
         self.config_file = None
+        self.state_file = None
         self.targets = Path(__file__).absolute().parent / "targets"
         self.wheel_tag = None
         self.abi_tag = None
         self.ext_suffix = None
         self.platform = None
         self.build_number = None
         self.python_cflags = None
         self.python_ldflags = None
         self.python_includes = None
         self.python_libs = None
 
-    def finalize(self, getenv=os.getenv):
+    def finalize(self, getenv=os.getenv, sdist=False, in_place=False):
         if self._finalized:
             return
         self._finalized = True
 
         self.output_dir = self.source_dir / (self.output_dir or "dist")
-        self.build_dir = self.source_dir / (self.build_dir or "build/layout")
+        self.build_dir = self.source_dir / (self.build_dir or "build/bin")
+        self.layout_dir = self.source_dir / (self.layout_dir or "build/layout")
         self.temp_dir = self.source_dir / (self.temp_dir or "build/temp")
         self.pkginfo = self.source_dir / (self.pkginfo or "PKG-INFO")
+        self.metadata_dir = self.temp_dir / (self.metadata_dir or "metadata")
 
         self._set_best("config_file", None, "PYMSBUILD_CONFIG", "_msbuild.py", getenv)
+        self._set_best("state_file", None, "PYMSBUILD_STATE_FILE", (self.layout_dir / "__state.txt"), getenv)
+        if self.state_file:
+            self.state_file = Path(self.state_file)
 
         type(self).current = self
 
         if self.config is None:
             import importlib.util
             file = self.source_dir / (self.config_file or "_msbuild.py")
             spec = importlib.util.spec_from_file_location("_msbuild", file)
@@ -121,14 +141,16 @@
                     self.metadata = self.config.init_METADATA()
                     if self.metadata:
                         self.config.METADATA = self.metadata
                     else:
                         self.metadata = self.config.METADATA
                 if hasattr(self.config, "METADATA"):
                     self.metadata = self.config.METADATA
+        if self.metadata is None:
+            raise RuntimeError("failed to locate METADATA")
 
         self._set_best("msbuild_exe", None, "MSBUILD", None, getenv)
         if self.msbuild_exe is None:
             self.msbuild_exe = locate_msbuild()
         if isinstance(self.msbuild_exe, str):
             if Path(self.msbuild_exe).is_file():
                 self.msbuild_exe = [self.msbuild_exe]
@@ -140,25 +162,40 @@
 
         self._set_best("ext_suffix", "ExtSuffix", "PYMSBUILD_EXT_SUFFIX", None, getenv)
         self._set_best("abi_tag", "AbiTag", "PYMSBUILD_ABI_TAG", None, getenv)
         self._set_best("wheel_tag", "WheelTag", "PYMSBUILD_WHEEL_TAG", None, getenv)
         self._set_best("platform", None, "PYMSBUILD_PLATFORM", None, getenv)
         self._set_best("configuration", None, "PYMSBUILD_CONFIGURATION", "Release", getenv)
 
+        if in_place:
+            default_target = "RelayoutInPlace" if self.force else "LayoutInPlace"
+        elif sdist:
+            default_target = "RelayoutSdist" if self.force else "LayoutSdist"
+        else:
+            default_target = "Relayout" if self.force else "Layout"
+        self._set_best("target", None, "PYMSBUILD_TARGET", default_target, getenv)
+
         tags = _tags.choose_best_tags(
             ext_suffix = self.ext_suffix,
             abi_tag = self.abi_tag,
             wheel_tag = self.wheel_tag,
             platform_tag = self.platform,
         )
         self.ext_suffix = tags.ext_suffix
         self.abi_tag = tags.abi_tag
         self.wheel_tag = tags.wheel_tag
         self.platform = tags.platform_tag
 
+        name, version = self.metadata["Name"], self.metadata["Version"]
+        name = re.sub(r"[^\w\d.]+", "_", name, re.UNICODE)
+        version = re.sub(r"[^\w\d.]+", "_", version, re.UNICODE)
+        self._set_best("sdist_name", None, "PYMSBUILD_SDIST_NAME", "{}-{}.tar.gz".format(name, version), getenv)
+        self._set_best("wheel_name", None, "PYMSBUILD_WHEEL_NAME", "{}-{}-{}.whl".format(name, version, self.wheel_tag), getenv)
+        self._set_best("distinfo_name", None, "PYMSBUILD_DISTINFO_NAME", "{}-{}.dist-info".format(name, version), getenv)
+
         self._set_best("python_config", None, "PYTHON_CONFIG", None, getenv)
         self._set_best("python_includes", None, "PYTHON_INCLUDES", getenv("PYMSBUILD_PYTHON_INCLUDES"), getenv)
         self._set_best("python_libs", None, "PYTHON_LIBS", getenv("PYMSBUILD_PYTHON_LIBS"), getenv)
 
         if not self.python_includes:
             self.python_includes = sysconfig.get_config_var("INCLUDEPY")
         if not self.python_libs:
@@ -166,15 +203,15 @@
                 self.python_libs = PurePath(sysconfig.get_config_var("installed_base")) / "libs"
             else:
                 self.python_libs = sysconfig.get_config_var("LIBPL")
 
         if self.package is None:
             if hasattr(self.config, "init_PACKAGE"):
                 self.log("Dynamically initialising PACKAGE")
-                if self._is_sdist:
+                if sdist:
                     pack = self.config.init_PACKAGE(None)
                 else:
                     pack = self.config.init_PACKAGE(str(self.wheel_tag))
                 if pack:
                     self.config.PACKAGE = self.package
             self.package = self.config.PACKAGE
 
@@ -208,15 +245,16 @@
         if not self.quiet:
             print(*values, sep=sep)
 
     def generate(self):
         if self.project:
             return self.project
 
-        self.finalize()
+        if not self._finalized:
+            raise RuntimeError("BuildState must be finalized before generating the project")
 
         self.temp_dir.mkdir(parents=True, exist_ok=True)
         if self.metadata is not None:
             self.pkginfo = self.temp_dir / "PKG-INFO"
             self.log("Generating", self.pkginfo)
             _generate.generate_distinfo(self.metadata, self.temp_dir, self.source_dir)
 
@@ -238,16 +276,14 @@
         self.log("Generated", self.project)
 
         return self.project
 
     def build(self, **properties):
         self.finalize()
         project = self.generate()
-        if self.target is None:
-            self.target = "Rebuild" if self.force else "Build"
         self.log("Compiling", project, "with", *self.msbuild_exe, "({})".format(self.target))
         if not project.is_file():
             raise FileNotFoundError(project)
         properties.setdefault("Configuration", self.configuration)
         if not properties.get("Platform"):
             try:
                 properties["Platform"] = _tags.remap_platform_to_msbuild(self.platform)
@@ -256,14 +292,15 @@
                 properties["Platform"] = self.platform
         properties.setdefault("HostPython", sys.executable)
         properties.setdefault("PyMsbuildTargets", self.targets)
         properties.setdefault("_ProjectBuildTarget", self.target)
         properties.setdefault("SourceRootDir", self.source_dir)
         properties.setdefault("OutDir", self.build_dir)
         properties.setdefault("IntDir", self.temp_dir)
+        properties.setdefault("LayoutDir", self.layout_dir)
         properties.setdefault("PythonConfig", self.python_config)
         properties.setdefault("PythonIncludes", self.python_includes)
         properties.setdefault("PythonLibs", self.python_libs)
         rsp = self.temp_dir / f"{project}.{os.getpid()}.rsp"
         with rsp.open("w", encoding="utf-8-sig") as f:
             print(project, file=f)
             print("/nologo", file=f)
@@ -272,15 +309,15 @@
                 print("/v:n", file=f)
             else:
                 print("/v:m", file=f)
             print("/t:", self.target, sep="", file=f)
             for k, v in properties.items():
                 if v is None:
                     continue
-                if k in {"IntDir", "OutDir", "SourceDir"}:
+                if k in {"IntDir", "OutDir", "SourceDir", "LayoutDir"}:
                     v = f"{PurePath(v)}{os.path.sep}"
                 print(_quote(f"/p:{k}={v}"), file=f)
         if self.verbose:
             with rsp.open("r", encoding="utf-8-sig") as f:
                 self.log(" ".join(map(str.strip, f)))
             self.log()
         _run = subprocess.check_output if self.quiet else subprocess.check_call
@@ -296,309 +333,210 @@
         else:
             try:
                 rsp.unlink()
             except OSError:
                 pass
 
     def build_in_place(self):
-        self.finalize()
+        self.finalize(in_place=True)
         self.generate()
-        assert self.project
-        self.target = "RebuildInPlace" if self.force else "BuildInPlace"
         self.build()
 
     def clean(self):
         self.finalize()
         p = self.config.PACKAGE
         self.project = self.temp_dir / (p.name + ".proj")
         if self.project.is_file():
             self.target = "Clean"
             self.build()
 
     def get_requires_for_build_sdist(self):
-        self._is_sdist = True
-        self.finalize()
+        self.finalize(sdist=True)
         return self.metadata.get("BuildSdistRequires", [])
 
-    def build_sdist(self):
-        self._is_sdist = True
-        self.finalize()
-        self.target = "RebuildSdist" if self.force else "BuildSdist"
-        if self.build_dir.is_dir():
-            shutil.rmtree(self.build_dir)
-            self.build_dir.mkdir(parents=True, exist_ok=True)
+    def layout_sdist(self, statefile=True):
+        self.finalize(sdist=True)
         self.generate()
+
+        if self.layout_dir.is_dir():
+            self.log("Removing existing layout directory", self.layout_dir)
+            shutil.rmtree(self.layout_dir)
+
         self.build()
-        if self.layout_dir:
-            return self.layout_sdist()
+
+        if not self.layout_dir.is_dir():
+            raise RuntimeError(f"Build failed to create {self.layout_dir}")
+
+        if statefile:
+            self._write_state("pack_sdist")
+            self.write("Wrote layout to", self.layout_dir)
+
+    def build_sdist(self):
+        self.finalize(sdist=True)
+        self.layout_sdist(statefile=False)
         return self.pack_sdist()
 
-    def pack_sdist(self):
-        self._is_sdist = True
-        self.finalize()
-        import gzip, tarfile
+    def pack_sdist(self, files=None):
+        self.finalize(sdist=True)
         self.output_dir.mkdir(parents=True, exist_ok=True)
-        name, version = self.metadata["Name"], self.metadata["Version"]
-        sdist_basename = "{}-{}".format(
-            re.sub(r"[^\w\d.]+", "_", name, re.UNICODE),
-            re.sub(r"[^\w\d.]+", "_", version, re.UNICODE),
-        )
-        sdist = self.output_dir / (sdist_basename + ".tar.gz")
+        sdist = self.output_dir / self.sdist_name
+
+        if self.sdist_name.casefold().endswith(".tar.gz".casefold()):
+            tar_name = self.sdist_name[:-3]
+        else:
+            tar_name = self.sdist_name + ".tar"
+
+        rel_files = _relative_to_layout(files, self.layout_dir)
+        import gzip, tarfile
         with gzip.open(sdist, "w") as f_gz:
-            with tarfile.TarFile.open(
-                sdist_basename + ".tar",
-                "w",
-                fileobj=f_gz,
-                format=tarfile.PAX_FORMAT
-            ) as f:
-                f.add(
-                    self.build_dir,
-                    arcname=sdist_basename,
-                    recursive=True,
-                )
+            with tarfile.TarFile.open(tar_name, "w", fileobj=f_gz, format=tarfile.PAX_FORMAT) as f:
+                self.log("Packing files into", sdist)
+                for n, rn in rel_files:
+                    if n == self.state_file:
+                        continue
+                    self.log("-", rn)
+                    f.add(n, arcname=rn)
+                self.log()
         self.write("Wrote sdist to", sdist)
         return sdist.name
 
     def get_requires_for_build_wheel(self):
-        self._is_sdist = True
         self.finalize()
         return self.metadata.get("BuildWheelRequires", [])
 
-    def build_wheel(self, metadata_dir=None):
+    def layout_wheel(self, statefile=True):
         self.finalize()
-        self.target = "Rebuild" if self.force else "Build"
-        if self.build_dir.is_dir():
-            shutil.rmtree(self.build_dir)
-        if metadata_dir is None:
-            metadata_dir = self.temp_dir / "metadata"
-            if metadata_dir.is_dir():
-                shutil.rmtree(metadata_dir)
-        else:
-            metadata_dir = Path(metadata_dir)
-
         self.generate()
-        if not metadata_dir.is_dir():
-            self.prepare_wheel_distinfo(metadata_dir)
+
+        if self.layout_dir.is_dir():
+            self.log("Removing existing layout directory", self.layout_dir)
+            shutil.rmtree(self.layout_dir)
 
         self.build()
-        if self.layout_dir:
-            return self.layout_wheel(metadata_dir)
-        return self.pack_wheel(metadata_dir)
 
-    def pack_wheel(self, metadata_dir):
+        if not self.layout_dir.is_dir():
+            raise RuntimeError(f"Build failed to create {self.layout_dir}")
+
+        if not self.metadata_dir.is_dir():
+            self.prepare_wheel_distinfo()
+
+        # Copy metadata_dir into layout_dir
+        if self.metadata_dir != self.layout_dir:
+            for n, rn in _relative_to_layout(None, self.metadata_dir):
+                n2 = self.layout_dir / rn
+                n2.parent.mkdir(parents=True, exist_ok=True)
+                shutil.copy(n, n2)
+
+        if statefile:
+            self._write_state("pack_wheel")
+            self.write("Wrote layout to", self.layout_dir)
+
+    def build_wheel(self, metadata_dir=None):
+        self.finalize()
+        if metadata_dir:
+            self.metadata_dir = Path(metadata_dir)
+            if not self.metadata_dir.is_dir():
+                self.prepare_wheel_distinfo()
+        else:
+            self.prepare_wheel_distinfo()
+        self.layout_wheel()
+        return self.pack_wheel()
+
+    def pack_wheel(self, files=None):
         self.finalize()
-        import zipfile
         self.output_dir.mkdir(parents=True, exist_ok=True)
 
-        name, version = self.metadata["Name"], self.metadata["Version"]
-        wheel = self.output_dir / "{}-{}-{}.whl".format(
-            re.sub(r"[^\w\d.]+", "_", name, re.UNICODE),
-            re.sub(r"[^\w\d.]+", "_", version, re.UNICODE),
-            self.wheel_tag,
-        )
+        wheel = self.output_dir / self.wheel_name
         record = []
+        record_files = []
+        rel_files = _relative_to_layout(files, self.layout_dir)
+
+        import zipfile
         with zipfile.ZipFile(wheel, "w", compression=zipfile.ZIP_DEFLATED) as f:
-            for n in metadata_dir.rglob(r"**/*"):
-                if n.is_file():
-                    record.append(_add_and_record(f, n, n.relative_to(metadata_dir)))
-            for n in self.build_dir.rglob(r"**/*"):
-                if n.is_file():
-                    record.append(_add_and_record(f, n, n.relative_to(self.build_dir)))
-            record_files = []
-            for n in metadata_dir.glob("*.dist-info"):
-                if not n.is_dir():
+            self.log("Packing files into", wheel)
+            for n, rn in rel_files:
+                if n == self.state_file:
                     continue
-                record_files.append(r"{}/RECORD".format(n.name))
-                record.append(r"{}/RECORD,,".format(n.name))
+                self.log("-", rn)
+                record.append(_add_and_record(f, n, rn))
+            for n in self.metadata_dir.glob("*.dist-info"):
+                if n.is_dir():
+                    record_files.append(rf"{n.name}/RECORD")
+                    record.append(rf"{n.name}/RECORD,,")
             record_file = "\n".join(record).encode("utf-8")
             for n in record_files:
+                self.log("-", n)
                 f.writestr(n, record_file)
+            self.log()
         self.write("Wrote wheel to", wheel)
         return wheel.name
 
-    def prepare_wheel_distinfo(self, metadata_dir=None):
+    def prepare_wheel_distinfo(self):
         self.finalize()
-        metadata_dir = Path(metadata_dir or self.output_dir)
         self.generate()
-        name, version = self.metadata["Name"], self.metadata["Version"]
-        outdir = metadata_dir / "{}-{}.dist-info".format(
-            re.sub(r"[^\w\d.]+", "_", name, re.UNICODE),
-            re.sub(r"[^\w\d.]+", "_", version, re.UNICODE),
-        )
+        outdir = self.metadata_dir / self.distinfo_name
         outdir.mkdir(parents=True, exist_ok=True)
         from pymsbuild import __version__
         with open(outdir / "WHEEL", "w", encoding="utf-8") as f:
             print("Wheel-Version: 1.0", file=f)
             print("Generator: pymsbuild", __version__, file=f)
             print("Root-Is-Purelib: false", file=f)
             for t in sorted(self.wheel_tag):
                 print("Tag:", t, file=f)
             if self.build_number:
                 print("Build:", self.build_number, file=f)
         shutil.copy(self.pkginfo, outdir / "METADATA")
         return outdir.name
 
-    def _write_state(self, state_file, outfile, outfmt):
-        print("output-format=", outfmt, sep="", file=state_file)
-        print("output-file=", outfile, sep="", file=state_file)
-        for k in dir(self):
-            if not k.startswith("_") and not hasattr(type(self), k):
-                v = getattr(self, k)
-                if isinstance(v, (str, PurePath)):
-                    print(k, "=", getattr(self, k), sep="", file=state_file)
-        print("# BEGIN FILES", file=state_file)
-
-    def layout_sdist(self):
-        self.finalize()
-        import zipfile
-        root = Path(self.layout_dir).absolute()
-        assert root
-        try:
-            shutil.rmtree(root)
-        except OSError:
-            pass
-        root.mkdir(parents=True, exist_ok=True)
-
-        name, version = self.metadata["Name"], self.metadata["Version"]
-        sdist_basename = "{}-{}".format(
-            re.sub(r"[^\w\d.]+", "_", name, re.UNICODE),
-            re.sub(r"[^\w\d.]+", "_", version, re.UNICODE),
-        )
-        sdist = self.output_dir / (sdist_basename + ".tar.gz")
-        with (root / "__state.txt").open("w", encoding="utf-8") as f:
-            self._write_state(f, sdist, "targz")
-            for n in self.build_dir.rglob("**/*"):
-                if n.is_file():
-                    rn = root / n.relative_to(self.build_dir)
-                    rn.parent.mkdir(parents=True, exist_ok=True)
-                    shutil.copy(n, rn)
-                    print(rn, file=f)
-        self.write("Wrote layout to", root)
-        return sdist.name
-
-    def layout_wheel(self, metadata_dir):
-        self.finalize()
-        import zipfile
-        root = Path(self.layout_dir).absolute()
-        assert root
-        try:
-            shutil.rmtree(root)
-        except OSError:
-            pass
-        root.mkdir(parents=True, exist_ok=True)
-
-        name, version = self.metadata["Name"], self.metadata["Version"]
-        wheel = self.output_dir / "{}-{}-{}.whl".format(
-            re.sub(r"[^\w\d.]+", "_", name, re.UNICODE),
-            re.sub(r"[^\w\d.]+", "_", version, re.UNICODE),
-            self.wheel_tag,
-        )
-        with (root / "__state.txt").open("w", encoding="utf-8") as f:
-            self._write_state(f, wheel, "whl")
-            for n in metadata_dir.rglob("**/*"):
-                if n.is_file():
-                    rn = root / n.relative_to(metadata_dir)
-                    rn.parent.mkdir(parents=True, exist_ok=True)
-                    shutil.copy(n, rn)
-                    print(rn, file=f)
-            for n in self.build_dir.rglob("**/*"):
-                if n.is_file():
-                    rn = root / n.relative_to(self.build_dir)
-                    rn.parent.mkdir(parents=True, exist_ok=True)
-                    shutil.copy(n, rn)
-                    print(rn, file=f)
-        self.write("Wrote layout to", root)
-        return wheel.name
+    def _write_state(self, cmd):
+        with self.state_file.open("w", encoding="utf-8") as f:
+            print("pack-command=", cmd, sep="", file=f)
+            for k in dir(self):
+                if not k.startswith("_") and not hasattr(type(self), k) and k not in {"layout_dir"}:
+                    v = getattr(self, k)
+                    if isinstance(v, (str, PurePath)):
+                        print(k, "=", getattr(self, k), sep="", file=f)
+            print("# BEGIN FILES", file=f)
+            for n, rn in _relative_to_layout(None, self.layout_dir):
+                print(rn, file=f)
 
     def pack(self):
-        root = Path(self.layout_dir)
-        if not root:
+        self.finalize()
+        if not self.state_file or not self.state_file.is_file():
             print(
                 "'--layout-dir' argument is required when invoking the 'pack' command",
                 file=sys.stderr
             )
             return
-        root = root.absolute()
-        outfile = None
-        outfmt = None
-        with (root / "__state.txt").open("r", encoding="utf-8-sig") as f:
+        cmd = None
+        with self.state_file.open("r", encoding="utf-8-sig") as f:
             for i in f:
                 k, sep, v = i.strip().partition("=")
                 if not sep:
                     break
-                if k == "output-file":
-                    outfile = Path(v)
-                elif k == "output-format":
-                    outfmt = v
+                if k == "pack-command":
+                    cmd = v
                 elif not k.startswith("_") and hasattr(self, k) and not hasattr(type(self), k):
                     setattr(self, k, v)
                 else:
                     self.log("Property", k, "from layout directory is ignored")
-            files = [root / i.strip() for i in f if i.strip()]
-            extra = list(self.layout_extra_files or ())
-            seen = set()
-            while extra:
-                i = (extra.pop(0) or "").strip()
-                if i in seen:
-                    continue
-                seen.add(i)
-                if i.startswith("@"):
-                    with Path(i[1:]).open("r", encoding="utf-8-sig") as f2:
-                        extra.extend(f2)
-                elif i:
-                    files.append(root / i)
-        if not outfmt or not outfile:
-            print("Layout appears to be corrupted. Please rerun the first stage again.", file=sys.stderr)
+            for k in ["layout_dir", "output_dir", "build_dir", "temp_dir", "metadata_dir"]:
+                v = getattr(self, k, None)
+                if v:
+                    setattr(self, k, Path(v))
+            files = [self.layout_dir / i.strip() for i in f if i.strip()]
+        extra = list(self.layout_extra_files or ())
+        seen = set()
+        while extra:
+            i = (extra.pop(0) or "").strip()
+            if i in seen:
+                continue
+            seen.add(i)
+            if i.startswith("@"):
+                with Path(i[1:]).open("r", encoding="utf-8-sig") as f:
+                    extra.extend(f)
+            elif i:
+                files.append(self.layout_dir / i)
+        if not cmd or cmd not in {'pack_sdist', 'pack_wheel'}:
+            self.write("Layout appears to be corrupted. Please rerun the first stage again.")
             return
-        if outfmt == "targz":
-            import gzip, tarfile
-            outfile.parent.mkdir(parents=True, exist_ok=True)
-            self.log("Writing .tar.gz to", outfile)
-            with gzip.open(outfile, "w") as f_gz:
-                with tarfile.TarFile.open(
-                    PurePath(outfile).with_suffix(""),
-                    "w",
-                    fileobj=f_gz,
-                    format=tarfile.PAX_FORMAT
-                ) as f:
-                    for n in files:
-                        if n.is_file():
-                            try:
-                                rn = n.relative_to(root)
-                            except ValueError:
-                                self.write("Not including", n, "from outside of layout directory")
-                            else:
-                                self.log("Adding", rn)
-                                f.add(n, arcname=rn)
-            self.write("Wrote sdist to", outfile)
-        elif outfmt == "whl":
-            import zipfile
-            record = []
-            record_files = []
-            outfile.parent.mkdir(parents=True, exist_ok=True)
-            self.log("Writing .whl to", outfile)
-            with zipfile.ZipFile(outfile, "w", compression=zipfile.ZIP_DEFLATED) as f:
-                for n in files:
-                    if n.is_file():
-                        try:
-                            rn = n.relative_to(root)
-                        except ValueError:
-                            self.write("Not including", n, "from outside of layout directory")
-                        else:
-                            self.log("Adding", rn)
-                            record.append(_add_and_record(f, n, rn))
-                    if n.match("*.dist-info/*"):
-                        n2 = "{}{}RECORD".format(n.parent.name, os.path.sep)
-                        if n2 not in record_files:
-                            record_files.append(n2)
-                            record.append("{},,".format(n2))
-                record_file = "\n".join(record).encode("utf-8")
-                for n in record_files:
-                    f.writestr(n, record_file)
-            self.write("Wrote wheel to", outfile)
-        else:
-            print(
-                "Unsupported output format '{}'. Please do not modify the state file".format(
-                    outfmt,
-                ),
-                file=sys.stderr,
-            )
+        return getattr(self, cmd)(files)
```

### Comparing `pymsbuild-0.2.2/pymsbuild/_generate.py` & `pymsbuild/_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,22 +125,20 @@
 
     tpath = project.options.get("TargetName", project.name) + (project.options.get("TargetExt") or ".pyd")
     tname, tdot, text = tpath.rpartition(".")
     with ProjectFileWriter(proj, tname, vc_platforms=True, root_namespace=project.name) as f:
         with f.group("PropertyGroup", Label="Globals"):
             f.add_property("SourceDir", ConditionalValue(source_dir, if_empty=True))
             f.add_property("SourceRootDir", ConditionalValue(root_dir, if_empty=True))
-            f.add_property("OutDir", f"layout{SEP}")
-            f.add_property("IntDir", ConditionalValue(f"build{SEP}", if_empty=True))
             f.add_property("__TargetExt", tdot + text)
             for k, v in project.options.items():
                 if k not in {"ConfigurationType", "TargetExt"}:
                     f.add_property(k, v)
-        f.add_import(f"$(PyMsbuildTargets){SEP}cpp-default-$(Platform).props")
         f.add_import(f"$(PyMsbuildTargets){SEP}common.props")
+        f.add_import(f"$(PyMsbuildTargets){SEP}cpp-default-$(Platform).props")
         with f.group("PropertyGroup", Label="Configuration"):
             f.add_property("ConfigurationType", project.options.get("ConfigurationType", "DynamicLibrary"))
             f.add_property("PlatformToolset", "$(DefaultPlatformToolset)")
             f.add_property("BasePlatformToolset", "$(DefaultPlatformToolset)")
             f.add_property("CharacterSet", "Unicode")
         f.add_import(f"$(PyMsbuildTargets){SEP}cpp-$(Platform).props")
         f.add_import(f"$(PyMsbuildTargets){SEP}pyd.props")
@@ -190,19 +188,18 @@
     if isinstance(project, PydFile):
         return _generate_pyd(project, build_dir, root_dir)
 
     with ProjectFileWriter(proj, project.name) as f:
         with f.group("PropertyGroup"):
             f.add_property("SourceDir", ConditionalValue(source_dir, if_empty=True))
             f.add_property("SourceRootDir", ConditionalValue(root_dir, if_empty=True))
-            f.add_property("OutDir", ConditionalValue(f"layout{SEP}", if_empty=True))
-            f.add_property("IntDir", ConditionalValue(f"build{SEP}", if_empty=True))
             for k, v in project.options.items():
                 f.add_property(k, v)
         f.add_import(f"$(PyMsbuildTargets){SEP}common.props")
+        f.add_import(f"$(PyMsbuildTargets){SEP}package.props")
         with f.group("ItemGroup", Label="ProjectReferences"):
             for n, p in _all_members(project, return_if=lambda m: m is not project and isinstance(m, PydFile)):
                 fn = PurePath(n)
                 pdir = _generate_pyd(p, build_dir, source_dir)
                 try:
                     pdir = pdir.relative_to(proj.parent)
                 except ValueError:
```

### Comparing `pymsbuild-0.2.2/pymsbuild/_init.py` & `pymsbuild/_init.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/_load_sysconfig.py` & `pymsbuild/_load_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/_locate_dotnet.py` & `pymsbuild/_locate_dotnet.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/_locate_vs.py` & `pymsbuild/_locate_vs.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/_msbuild.py.in` & `pymsbuild/_msbuild.py.in`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         # https://packaging.python.org/en/latest/specifications/dependency-specifiers/
     ],
 
     # Universal wheel? Uncomment this to target all Python 3 installs.
     #"WheelTag": "py3-none-any",
 
     # Limited ABI wheel? Uncomment this for abi3 on the target platform.
+    # (Remember to also specify the build variables to actually enable it)
     #"WheelTag": "py3-abi3-*",
 
     # Additional build dependencies? If they can't go in pyproject.toml, they go here.
     #"BuildSdistRequires": [],
     #"BuildWheelRequires": [],
 }
 
@@ -40,15 +41,15 @@
 
 # OPTIONAL: Update METADATA entries while building an sdist
 # These are kept in the sdist, and sdist builds will not call this again
 def init_METADATA():
     # EXAMPLE: Extract version-like tags from GitHub Actions builds
     import os, re
     _, sep, version = os.getenv("GITHUB_REF", "").rpartition("/")
-    if sep and re.match(r"\d+(\.\d+)+$", version):
+    if sep and re.match(r"(\d+!)?\d+(\.\d+)+((a|b|rc)\d+)?(\.post\d+)?(\.dev\d+)?$", version):
         # Looks like a version tag
         METADATA["Version"] = version
 
 
 # OPTIONAL: Update PACKAGE entries while building an sdist or wheel.
 # 'tag' will be the wheel tag, or 'None' for an sdist.
 # In general, you  want all entries to be present for sdist builds, but might remove
```

### Comparing `pymsbuild-0.2.2/pymsbuild/_tags.py` & `pymsbuild/_tags.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/_types.py` & `pymsbuild/_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -180,15 +180,18 @@
 When added to `Package`, the file will be copied into the resulting
 package directory.
 
 When added to another project, behaviour will depend on how that
 project treats "Content" elements.
 """
     _ITEMNAME = "Content"
-    options = {}
+    options = {
+        "IncludeInSdist": True,
+        "IncludeInWheel": True,
+    }
     has_condition = False
     condition = None
 
     def __init__(self, source, name=None, **metadata):
         self.source = PurePath(source)
         self.name = name or self.source.name
         self.members = []
@@ -206,87 +209,91 @@
 
 
 class PyFile(File):
     r"""Add a Python source file to a package.
 
 Currently does nothing special. One day will generate .pyc files.
 """
-    options = {"GeneratePyc": True}
+    options = {
+        "GeneratePyc": True,
+        "IncludeInSdist": True,
+        "IncludeInWheel": True,
+    }
 
 
 class Project(File):
     r"""Add a reference to an external MSBuild project.
 
-This project should either provide Build, BuildSdist and BuildInPlace
-targets, or import "$(PyMsbuildTargets)\common.targets". Otherwise,
-files referenced or generated by this project are not automatically
-included in sdists or wheels, or the projcet may cause the build to
-fail.
+This project should provide Build, GetPackageFiles and GetSdistFiles
+targets, or import "$(PyMsbuildTargets)\common.{props,targets}".
+Otherwise, files referenced or generated by this project are not
+automatically included in sdists or wheels, or the project may cause
+the build to fail.
 """
     _ITEMNAME = "Project"
 
 
 class SourceFile(File):
     r"""Add a generic file to use for building.
 
 These files will be included in the sdist, but will not be copied
 in-place or included in wheels.
 """
     _ITEMNAME = "None"
+    options = {
+        "IncludeInSdist": True,
+        "IncludeInWheel": False,
+    }
 
 
-class CSourceFile(File):
+class CSourceFile(SourceFile):
     r"""Add a C/C++ source file.
 
 These files will be included in the sdist, but will not be copied
 in-place or included in wheels, except as built output.
 
 Incremental rebuilds will be triggered when these files are modified,
 and each file is expected to produce a linkable file.
 """
     _ITEMNAME = "ClCompile"
 
 
-class LinkFile(File):
+class LinkFile(SourceFile):
     r"""Add a linker input file.
 
 These files will be included in the sdist, but will not be copied
 in-place or included in wheels, except as built output.
 
 Incremental rebuilds will be triggered when these files are modified,
 and each file will be linked into the final output.
 """
     _ITEMNAME = "Link"
 
-class IncludeFile(File):
+
+class IncludeFile(SourceFile):
     r"""Add a header file.
 
 These files will be included in the sdist, but will not be copied
 in-place or included in wheels, except as built output.
 
 Incremental rebuilds will be triggered when these files are modified,
 but they do not produce linkable outputs.
 """
     _ITEMNAME = "ClInclude"
 
-class RemoveFile:
-    r"""Removes a file that has already been added.
-
-This must appear after the files that were added, and must specify the
-same kind (either the class used to create it, or the string literal
-matching the MSBuild item name).
-"""
-    _ITEMNAME = None
-    name = None
-    members = ()
-    has_condition = True
-    condition = None
 
-    def __init__(self, kind, pattern):
-        self._ITEMNAME = getattr(kind, "_ITEMNAME", None) or str(kind)
-        self.exclude = pattern
+class RemoveFile(File):
+    r"""Removes a file that has already been added.
 
-    def if_(self, condition):
-        self.condition = condition
+Note that all matching files will be removed. You cannot add the file
+again after this has been specified. The 'Kind' is accepted as either
+a string or the type object, but is not used.
+"""
+    _ITEMNAME = "_ExcludeFile"
+    options = {}
 
-    def __str__(self):
-        return ""
+    def __init__(self, kind, source, name=None):
+        super().__init__(
+            source,
+            name, 
+            Kind=getattr(kind, "_ITEMNAME", None) or str(kind),
+        )
```

### Comparing `pymsbuild-0.2.2/pymsbuild/_writer.py` & `pymsbuild/_writer.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/cython.py` & `pymsbuild/cython.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+import os
+
 from pathlib import Path
 from pymsbuild._types import *
 
 class CythonPydFile(PydFile):
     def __init__(self, name, *members, project_file=None, **kwargs):
         super().__init__(name, *members, project_file=project_file, **kwargs)
         self.members = [
             Property("BeforeBuildGenerateSourcesTargets", "Cythonize;$(BeforeBuildGenerateSourcesTargets)"),
             ItemDefinition("PyxCompile", TargetExt=".c", Dependencies=""),
             *self.members,
-            LiteralXML('<Import Project="$(PyMsbuildTargets)/cython.targets" />'),
+            LiteralXML(f'<Import Project="$(PyMsbuildTargets){os.path.sep}cython.targets" />'),
         ]
 
 
 class PyxFile(File):
     _ITEMNAME = "PyxCompile"
-    options = {"TargetExt": ".c"}
+    options = {
+        "TargetExt": ".c",
+        "IncludeInSdist": True,
+        "IncludeInWheel": False,
+    }
 
 
 class CythonIncludeFile(File):
     _ITEMNAME = "CythonInclude"
+    options = {
+        "IncludeInSdist": True,
+        "IncludeInWheel": False,
+    }
```

### Comparing `pymsbuild-0.2.2/pymsbuild/dllpack.py` & `pymsbuild/dllpack.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/common.targets` & `pymsbuild/targets/package.targets`

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,121 @@
 <Project>
-  <!-- Managing content files -->
-  <Target Name="_AssignContentProperties">
-    <ItemGroup>
-      <Content>
-        <TargetDir Condition="%(TargetDir) == ''">$([msbuild]::EnsureTrailingSlash($([System.IO.Path]::GetDirectoryName(%(Name)))))</TargetDir>
-        <TargetName Condition="%(TargetName) == ''">$([System.IO.Path]::GetFileNameWithoutExtension(%(Name)))</TargetName>
-        <TargetExt Condition="%(TargetExt) == ''">$([System.IO.Path]::GetExtension(%(Name)))</TargetExt>
-      </Content>
-      <Content>
-        <RelativeSource Condition="%(RelativeSource) == ''">$([msbuild]::MakeRelative($(SourceDir.TrimEnd($(_Sep))), %(FullPath)))</RelativeSource>
-        <Destination Condition="%(IncludeInWheel)">$([msbuild]::EnsureTrailingSlash($(OutDir)))%(TargetDir)%(TargetName)%(TargetExt)</Destination>
-        <Source>$([msbuild]::EnsureTrailingSlash($(OutDir)))%(RelativeSource)</Source>
-      </Content>
-    </ItemGroup>
-  </Target>
-
-  <Target Name="_MkdirContent" DependsOnTargets="_AssignContentProperties">
-    <ItemGroup>
-      <_Outputs Include="%(Content.Destination)" />
-    </ItemGroup>
-    <MakeDir Directories="%(_Outputs.RootDir)%(_Outputs.Directory)" />
-  </Target>
-
-  <Target Name="_CopyContent" Inputs="@(Content)" Outputs="%(Content.Destination)" DependsOnTargets="_MkdirContent">
-    <Copy SourceFiles="%(Content.FullPath)" DestinationFiles="%(Content.Destination)" Condition="%(Content.Destination) != ''">
-      <Output TaskParameter="CopiedFiles" ItemName="FileWrites" />
-    </Copy>
-  </Target>
-
   <!-- Managing dependencies -->
   <Target Name="_AssignProjectProperties">
     <ItemGroup>
       <Project>
-        <Properties>
+        <Properties Condition="%(Project.Properties) == ''"></Properties>
+        <PyMSBuild_Properties>
         _ProjectBuildTarget=$(_ProjectBuildTarget);
         IntDir=$([msbuild]::EnsureTrailingSlash(`%(IntDir)`))$(_EscapeSep);
         SourceRootDir=$([msbuild]::EnsureTrailingSlash(`$(SourceRootDir)`))$(_EscapeSep);
         SourceDir=$([msbuild]::EnsureTrailingSlash($(SourceDir)))$([msbuild]::EnsureTrailingSlash(%(TargetDir)))$(_EscapeSep);
+        OutDir=$([msbuild]::EnsureTrailingSlash($(OutDir)))$([msbuild]::EnsureTrailingSlash(%(TargetDir)))$(_EscapeSep);
         TargetName=%(TargetName);
-        TargetExt=%(TargetExt);
-        %(Properties)
-        </Properties>
+        TargetExt=%(TargetExt)
+        </PyMSBuild_Properties>
       </Project>
+    </ItemGroup>
+    <ItemGroup>
       <Project>
-        <Properties Condition="$(_ProjectBuildTarget) != 'BuildSdist'">
-        OutDir=$([msbuild]::EnsureTrailingSlash($(OutDir)))$([msbuild]::EnsureTrailingSlash(%(TargetDir)))$(_EscapeSep);%(Properties)
-        </Properties>
-        <Properties Condition="$(_ProjectBuildTarget) == 'BuildSdist'">
-        OutDir=$([msbuild]::EnsureTrailingSlash(`$(OutDir)`))$(_EscapeSep);%(Properties)
-        </Properties>
+        <Properties Condition="%(Properties) != ''">%(PyMSBuild_Properties);%(Properties)</Properties>
+        <Properties Condition="%(Properties) == ''">%(PyMSBuild_Properties)</Properties>
       </Project>
     </ItemGroup>
   </Target>
 
   <Target Name="BuildDependencies" DependsOnTargets="_AssignProjectProperties" Condition="@(Project) != ''">
     <Message Text="Building %(Project.Name) with %(Project.Properties)" Importance="$(_Low)" />
-    <MSBuild Projects="@(Project)" Targets="$(_ProjectBuildTarget)" Properties="%(Project.Properties)" />
+    <MSBuild Projects="@(Project)" Targets="Build" Properties="%(Project.Properties)" />
   </Target>
 
   <Target Name="CleanDependencies" DependsOnTargets="_AssignProjectProperties" Condition="@(Project) != ''">
     <MSBuild Projects="@(Project)" Targets="Clean" Properties="%(Project.Properties)" />
   </Target>
 
-  <!-- Standard builds -->
-  <Target Name="PrepareForBuild" />
-  <Target Name="CoreBuild" />
-  <Target Name="Build" DependsOnTargets="PrepareForBuild;_AssignContentProperties;BuildDependencies;CoreBuild;_CopyContent" />
-  <Target Name="Clean" />
-  <Target Name="Rebuild" DependsOnTargets="Clean;Build" />
-
-  <!-- In-place builds -->
-  <Target Name="CalculateInPlace">
+  <!-- Layout support -->
+  <Target Name="_Layout_Mkdir">
     <ItemGroup>
-      <InPlace Include="@(Content)" />
-      <InPlace>
-        <Destination>$([msbuild]::EnsureTrailingSlash($(SourceDir)))%(Name)</Destination>
-      </InPlace>
+      <_Outputs Include="%(_DistFiles.Destination)" />
     </ItemGroup>
+    <MakeDir Directories="%(_Outputs.RootDir)%(_Outputs.Directory)" />
   </Target>
 
-  <Target Name="_InPlace_Exclude" AfterTargets="CalculateInPlace">
+  <Target Name="_Layout_Copy" Inputs="@(_DistFiles)" Outputs="%(_DistFiles.Destination)">
     <ItemGroup>
-      <_ToRemove Include="@(InPlace)" Condition="%(Extension) == '.exp'" />
-      <InPlace Remove="@(_ToRemove)" />
+      <FileWrites Include="%(_DistFiles.Destination)" />
     </ItemGroup>
-  </Target> 
+    <Copy SourceFiles="%(_DistFiles.FullPath)"
+          DestinationFiles="%(_DistFiles.Destination)"
+          UseHardLinksIfPossible="true">
+      <Output TaskParameter="CopiedFiles" ItemName="_CopiedDistFiles" />
+    </Copy>
+  </Target>
 
-  <Target Name="_MkdirInPlace">
+  <Target Name="_Layout_Calculate">
     <ItemGroup>
-      <_Outputs Include="%(InPlace.Destination)" />
+      <_DistFiles Remove="@(_DistFiles)" />
+      <_DistFiles Include="@(PyMSBuild_PackageFiles)">
+        <Destination>$([msbuild]::EnsureTrailingSlash($(LayoutDir)))%(TargetDir)%(TargetName)%(TargetExt)</Destination>
+      </_DistFiles>
     </ItemGroup>
-    <MakeDir Directories="%(_Outputs.RootDir)%(_Outputs.Directory)" />
   </Target>
 
-  <Target Name="_CopyInPlace" Inputs="@(InPlace)" Outputs="%(InPlace.Destination)">
+  <Target Name="_LayoutSdist_Calculate">
     <ItemGroup>
-      <FileWrites Include="%(InPlace.Destination)" Condition="!Exists(%(InPlace.Destination))" />
+      <_DistFiles Remove="@(_DistFiles)" />
+      <_DistFiles Include="@(PyMSBuild_SDistFiles)">
+        <Destination>$([msbuild]::EnsureTrailingSlash($(LayoutDir)))%(RelativeSource)</Destination>
+      </_DistFiles>
     </ItemGroup>
-    <Copy SourceFiles="%(InPlace.FullPath)" DestinationFiles="%(InPlace.Destination)" />
   </Target>
 
-  <Target Name="BuildInPlace" DependsOnTargets="$(BuildInPlaceDependsOn)">
-    <Message Text="Copied to source tree:" Importance="high" Condition="@(InPlace) != ''" />
-    <Message Text=" - %(InPlace.Destination)" Importance="high" Condition="@(InPlace) != ''" />
+  <Target Name="_LayoutInPlace_Calculate">
+    <ItemGroup>
+      <_DistFiles Remove="@(_DistFiles)" />
+      <_DistFiles Include="@(PyMSBuild_PackageFiles)" Condition="%(IncludeInWheel)">
+        <Destination>$([msbuild]::EnsureTrailingSlash($(SourceDir)))%(TargetDir)%(TargetName)%(TargetExt)</Destination>
+      </_DistFiles>
+      <!-- Remove anything that is being copied directly from the source tree -->
+      <_Removing Include="@(_DistFiles)" Condition="%(FullPath) == %(Destination)" />
+      <_DistFiles Remove="@(_Removing)" />
+    </ItemGroup>
   </Target>
 
-  <Target Name="RebuildInPlace" DependsOnTargets="Clean;BuildInPlace" />
 
+  <PropertyGroup>
+    <CoreBuildTargetName Condition="$(CoreBuildTargetName) == ''">CoreBuild</CoreBuildTargetName>
+  </PropertyGroup>
 
-  <!-- Clean support -->
-  <Target Name="_SaveFileWrites" AfterTargets="Build;BuildSdist;BuildInPlace">
-    <WriteLinesToFile File="$(IntDir)/$(TargetName).writes.txt"
-                      Lines="@(FileWrites)"
-                      Overwrite="true" />
-    <Message Text="Files written:%0A -@(FileWrites, '%0A -')"
-             Importance="$(_Low)"
-             Condition="@(FileWrites) != ''" />
+  <Target Name="Layout"
+          DependsOnTargets="
+            PrepareForBuild;BuildDependencies;$(CoreBuildTargetName);GetPackageFiles;
+            _Layout_Calculate;
+            _Layout_Mkdir;_Layout_Copy;_SaveFileWrites">
+    <Message Text="Copied to layout:" Importance="high" Condition="@(_CopiedDistFiles) != ''" />
+    <Message Text=" - %(_CopiedDistFiles.Identity)" Importance="high" Condition="@(_CopiedDistFiles) != ''" />
   </Target>
 
-  <Target Name="_CleanFileWrites" BeforeTargets="Clean" DependsOnTargets="CleanDependencies">
-    <ReadLinesFromFile File="$(IntDir)/$(TargetName).writes.txt">
-      <Output TaskParameter="Lines" ItemName="FileWrites" />
-    </ReadLinesFromFile>
-    <Delete Files="@(FileWrites)" />
-    <ItemGroup>
-      <FileWrites Remove="@(FileWrites)" />
-    </ItemGroup>
+  <Target Name="LayoutSdist"
+          DependsOnTargets="
+            PrepareForBuild;GetSdistFiles;
+            _LayoutSdist_Calculate;
+            _Layout_Mkdir;_Layout_Copy;_SaveFileWrites">
+    <Message Text="Copied to layout:" Importance="high" Condition="@(_CopiedDistFiles) != ''" />
+    <Message Text=" - %(_CopiedDistFiles.Identity)" Importance="high" Condition="@(_CopiedDistFiles) != ''" />
   </Target>
 
-  <Import Project="sdist.targets" />
+  <Target Name="LayoutInPlace"
+          DependsOnTargets="
+            PrepareForBuild;BuildDependencies;$(CoreBuildTargetName);GetPackageFiles;
+            _LayoutInPlace_Calculate;
+            _Layout_Mkdir;_Layout_Copy;_SaveFileWrites">
+    <Message Text="Copied to source tree:" Importance="high" Condition="@(_CopiedDistFiles) != ''" />
+    <Message Text=" - %(_CopiedDistFiles.Identity)" Importance="high" Condition="@(_CopiedDistFiles) != ''" />
+  </Target>
+
+  <Target Name="Relayout" DependsOnTargets="Clean;Layout" />
+  <Target Name="RelayoutSdist" DependsOnTargets="Clean;LayoutSdist" />
+  <Target Name="RelayoutInPlace" DependsOnTargets="Clean;LayoutInPlace" />
+
+  <Import Project="$(MSBuildThisFileDirectory)package.override.targets" Condition="$(SuppressBasicTargetOverrides) != 'true'" />
 </Project>
```

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/cpp-POSIX_x64.targets` & `pymsbuild/targets/cpp-POSIX_x64.targets`

 * *Files 12% similar despite different names*

```diff
@@ -75,11 +75,12 @@
     <Exec Command="$(_Cmd)" />
     <ItemGroup>
       <FileWrites Include="$(TargetPath)" />
     </ItemGroup>
   </Target>
 
   <Target Name="CoreBuild" DependsOnTargets="_CalculateFlags;PrepareForBuild;$(BeforeBuildGenerateSourcesTargets);ClCompile;Link" />
-  <Target Name="Clean">
+  <Target Name="Build" DependsOnTargets="CoreBuild;_SaveFileWrites" />
+  <Target Name="Clean" DependsOnTargets="_CleanFileWrites">
     <RemoveDir Directories="$(IntDir)" />
   </Target>
 </Project>
```

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/cython.targets` & `pymsbuild/targets/cython.targets`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     </_PyxCompileWithOutput>
   </ItemGroup>
   <ItemGroup>
     <ClCompile Include="@(_PyxCompileWithOutput->'%(TargetPath)')">
       <RelativeSource>%(RelativeOutput)</RelativeSource>
       <PreprocessorDefinitions Condition="%(ClPreprocessorDefinitions) != ''">%(ClPreprocessorDefinitions);%(PreprocessorDefinitions)</PreprocessorDefinitions>
       <ObjectFile>$([msbuild]::MakeRelative($(IntDir), %(FullPath))).o</ObjectFile>
+      <IncludeInSdist>true</IncludeInSdist>
+      <IncludeInWheel>false</IncludeInWheel>
     </ClCompile>
   </ItemGroup>
 
 
   <Target Name="_CythonWarnings" BeforeTargets="PrepareForBuild">
     <Error Text="Do not specify PreprocessorDefinitions on PyxCompile elements. Use ClPreprocessorDefinitions or CythonPreprocessorDefinitions, depending on which preprocessor you are targeting."
            Condition="@(PyxCompile->'%(PreprocessorDefinitions)','') != ''" />
@@ -54,19 +56,24 @@
 
   <Target Name="Cythonize" DependsOnTargets="PrepareForBuild;_ForceCythonize;_CythonizeAll">
     <ItemGroup>
       <FileWrites Include="%(_PyxCompileWithOutput.TargetPath)" />
     </ItemGroup>
   </Target>
 
-  <Target Name="_BuildCythonSdist" DependsOnTargets="Cythonize" BeforeTargets="CalculateSdist">
+  <Target Name="_BuildCythonSdist" DependsOnTargets="Cythonize">
     <ItemGroup>
-      <Sdist Include="@(_PyxCompileWithOutput)">
-        <RelativeSource>%(RelativeSource)</RelativeSource>
-      </Sdist>
-      <Sdist Include="@(CythonInclude)">
-        <RelativeSource Condition="%(CythonInclude.RelativeSource) != ''">%(CythonInclude.RelativeSource)</RelativeSource>
-        <RelativeSource Condition="%(CythonInclude.RelativeSource) == ''">$([msbuild]::MakeRelative($(SourceRootDir.TrimEnd($(_Sep))), %(FullPath)))</RelativeSource>
-      </Sdist>
+      <AllSourceFiles Include="@(PyxCompile)">
+        <TargetName>%(Filename)</TargetName>
+        <TargetExt>%(Extension)</TargetExt>
+        <IncludeInSdist>true</IncludeInSdist>
+      </AllSourceFiles>
+      <AllSourceFiles Include="@(CythonInclude)">
+        <IncludeInSdist>true</IncludeInSdist>
+      </AllSourceFiles>
     </ItemGroup>
   </Target>
+
+  <PropertyGroup>
+    <GetSdistFilesTargets>_BuildCythonSdist;$(GetSdistFilesTargets)</GetSdistFilesTargets>
+  </PropertyGroup>
 </Project>
```

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/dllpack-generate.py` & `pymsbuild/targets/dllpack-generate.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/dllpack.c` & `pymsbuild/targets/dllpack.c`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/dllpack.targets` & `pymsbuild/targets/dllpack.targets`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,14 @@
     <ItemGroup>
       <ClCompile Include="$(MSBuildThisFileDirectory)dllpack.c">
         <AdditionalIncludeDirectories>$(IntDir);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
       </ClCompile>
       <ResourceCompile Include="$(IntDir)\dllpack.rc" />
     </ItemGroup>
   </Target>
+
+  <PropertyGroup>
+    <SuppressBasicTargetOverrides>true</SuppressBasicTargetOverrides>
+    <CoreBuildTargetName>Build</CoreBuildTargetName>
+  </PropertyGroup>
+  <Import Project="$(MSBuildThisFileDirectory)package.targets" />
 </Project>
```

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/dllpack_main.py` & `pymsbuild/targets/dllpack_main.py`

 * *Files identical despite different names*

### Comparing `pymsbuild-0.2.2/pymsbuild/targets/pyd.props` & `pymsbuild/targets/pyd.props`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <Project>
   <PropertyGroup>
     <TargetExt Condition="$(__TargetExt) != ''">$(__TargetExt)</TargetExt>
-    <TargetPath>$([System.IO.Path]::Combine($(ProjectDir),$(OutDir),$(TargetName)$(TargetExt)))</TargetPath>
+    <TargetPath>$([System.IO.Path]::Combine(`$(ProjectDir)`,`$(OutDir)`,`$(TargetName)$(TargetExt)`))</TargetPath>
     <LinkIncremental>false</LinkIncremental>
   </PropertyGroup>
   <ItemDefinitionGroup>
     <ClCompile>
       <AdditionalIncludeDirectories>$(SourceRootDir.TrimEnd($(_Sep)));$(PythonIncludes);%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
       <Optimization>Full</Optimization>
       <Optimization Condition="$(Configuration) == 'Debug'">Disabled</Optimization>
```

