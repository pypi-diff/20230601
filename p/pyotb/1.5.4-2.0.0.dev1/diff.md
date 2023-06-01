# Comparing `tmp/pyotb-1.5.4.tar.gz` & `tmp/pyotb-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyotb-1.5.4.tar", last modified: Sat Oct  1 19:29:58 2022, max compression
+gzip compressed data, was "pyotb-2.0.0.dev1.tar", last modified: Thu Jun  1 19:22:00 2023, max compression
```

## Comparing `pyotb-1.5.4.tar` & `pyotb-2.0.0.dev1.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-01 19:29:58.773445 pyotb-1.5.4/
--rw-rw-rw-   0 root         (0) root         (0)    11354 2022-09-21 07:37:28.000000 pyotb-1.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13179 2022-10-01 19:29:58.773445 pyotb-1.5.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12317 2022-09-29 10:17:21.000000 pyotb-1.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-01 19:29:58.773445 pyotb-1.5.4/pyotb/
--rw-rw-rw-   0 root         (0) root         (0)      318 2022-10-01 19:21:10.000000 pyotb-1.5.4/pyotb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6327 2022-10-01 19:07:46.000000 pyotb-1.5.4/pyotb/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    55271 2022-10-01 19:07:46.000000 pyotb-1.5.4/pyotb/core.py
--rw-rw-rw-   0 root         (0) root         (0)    20833 2022-10-01 19:07:46.000000 pyotb-1.5.4/pyotb/functions.py
--rw-rw-rw-   0 root         (0) root         (0)    12442 2022-10-01 19:07:46.000000 pyotb-1.5.4/pyotb/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-01 19:29:58.773445 pyotb-1.5.4/pyotb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13179 2022-10-01 19:29:58.000000 pyotb-1.5.4/pyotb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      249 2022-10-01 19:29:58.000000 pyotb-1.5.4/pyotb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-01 19:29:58.000000 pyotb-1.5.4/pyotb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-10-01 19:29:58.000000 pyotb-1.5.4/pyotb.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-09-21 07:37:28.000000 pyotb-1.5.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-10-01 19:29:58.773445 pyotb-1.5.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1149 2022-10-01 19:10:44.000000 pyotb-1.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-31 10:05:27.000000 pyotb-2.0.0.dev1/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-05-24 08:56:49.000000 pyotb-2.0.0.dev1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    16453 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2023-05-31 10:05:27.000000 pyotb-2.0.0.dev1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.035908 pyotb-2.0.0.dev1/pyotb/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5556 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    66822 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    22175 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13150 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyotb/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.035908 pyotb-2.0.0.dev1/pyotb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16453 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-01 19:22:00.000000 pyotb-2.0.0.dev1/pyotb.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-06-01 18:37:23.000000 pyotb-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:22:00.039908 pyotb-2.0.0.dev1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9942 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/test_numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/test_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2023-05-24 08:56:50.000000 pyotb-2.0.0.dev1/tests/tests_data.py
```

### Comparing `pyotb-1.5.4/LICENSE` & `pyotb-2.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyotb-1.5.4/pyotb/apps.py` & `pyotb-2.0.0.dev1/pyotb/apps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # -*- coding: utf-8 -*-
 """Search for OTB (set env if necessary), subclass core.App for each available application."""
+from __future__ import annotations
+
 import os
+import subprocess
 import sys
 from pathlib import Path
 
-from .helpers import logger, find_otb
+import otbApplication as otb  # pylint: disable=import-error
 
-otb = find_otb()
+from .core import App
+from .helpers import logger
 
 
-def get_available_applications(as_subprocess=False):
+def get_available_applications(as_subprocess: bool = False) -> list[str]:
     """Find available OTB applications.
 
     Args:
         as_subprocess: indicate if function should list available applications using subprocess call
 
     Returns:
         tuple of available applications
@@ -24,117 +28,110 @@
         # Currently, there is an incompatibility between OTBTF and Tensorflow that causes segfault
         # when OTBTF apps are used in a script where tensorflow has already been imported.
         # See https://github.com/remicres/otbtf/issues/28
         # Thus, we run this piece of code in a clean independent `subprocess` that doesn't interact with Tensorflow
         env = os.environ.copy()
         if "PYTHONPATH" not in env:
             env["PYTHONPATH"] = ""
-        env["PYTHONPATH"] = ":" + str(Path(otb.__file__).parent)
-        env["OTB_LOGGER_LEVEL"] = "CRITICAL"  # in order to suppress warnings while listing applications
+        env["PYTHONPATH"] += ":" + str(Path(otb.__file__).parent)
+        env[
+            "OTB_LOGGER_LEVEL"
+        ] = "CRITICAL"  # in order to suppress warnings while listing applications
         pycmd = "import otbApplication; print(otbApplication.Registry.GetAvailableApplications())"
         cmd_args = [sys.executable, "-c", pycmd]
-
         try:
-            import subprocess  # pylint: disable=import-outside-toplevel
             params = {"env": env, "stdout": subprocess.PIPE, "stderr": subprocess.PIPE}
-            with subprocess.Popen(cmd_args, **params) as p:
-                logger.debug('Exec "%s \'%s\'"', ' '.join(cmd_args[:-1]), pycmd)
-                stdout, stderr = p.communicate()
+            with subprocess.Popen(cmd_args, **params) as process:
+                logger.debug("Exec \"%s '%s'\"", " ".join(cmd_args[:-1]), pycmd)
+                stdout, stderr = process.communicate()
                 stdout, stderr = stdout.decode(), stderr.decode()
                 # ast.literal_eval is secure and will raise more handy Exceptions than eval
                 from ast import literal_eval  # pylint: disable=import-outside-toplevel
+
                 app_list = literal_eval(stdout.strip())
                 assert isinstance(app_list, (tuple, list))
         except subprocess.SubprocessError:
             logger.debug("Failed to call subprocess")
         except (ValueError, SyntaxError, AssertionError):
-            logger.debug("Failed to decode output or convert to tuple:\nstdout=%s\nstderr=%s", stdout, stderr)
-
+            logger.debug(
+                "Failed to decode output or convert to tuple:\nstdout=%s\nstderr=%s",
+                stdout,
+                stderr,
+            )
         if not app_list:
-            logger.info("Failed to list applications in an independent process. Falling back to local python import")
+            logger.debug(
+                "Failed to list applications in an independent process. Falling back to local python import"
+            )
     # Find applications using the normal way
     if not app_list:
         app_list = otb.Registry.GetAvailableApplications()
     if not app_list:
-        logger.warning("Unable to load applications. Set env variable OTB_APPLICATION_PATH then try again")
-        return ()
-
+        raise SystemExit(
+            "Unable to load applications. Set env variable OTB_APPLICATION_PATH and try again."
+        )
     logger.info("Successfully loaded %s OTB applications", len(app_list))
     return app_list
 
 
-AVAILABLE_APPLICATIONS = get_available_applications(as_subprocess=True)
-
-# First core.py call (within __init__ scope)
-from .core import App  # pylint: disable=wrong-import-position
-
-# This is to enable aliases of Apps, i.e. using apps like `pyotb.AppName(...)` instead of `pyotb.App("AppName", ...)`
-_CODE_TEMPLATE = """
-class {name}(App):
-    """ """
-    def __init__(self, *args, **kwargs):
-        super().__init__('{name}', *args, **kwargs)
-"""
-
-
 class OTBTFApp(App):
     """Helper for OTBTF."""
+
     @staticmethod
-    def set_nb_sources(*args, n_sources=None):
+    def set_nb_sources(*args, n_sources: int = None):
         """Set the number of sources of TensorflowModelServe. Can be either user-defined or deduced from the args.
 
         Args:
             *args: arguments (dict). NB: we don't need kwargs because it cannot contain source#.il
             n_sources: number of sources. Default is None (resolves the number of sources based on the
                        content of the dict passed in args, where some 'source' str is found)
 
         """
         if n_sources:
-            os.environ['OTB_TF_NSOURCES'] = str(int(n_sources))
+            os.environ["OTB_TF_NSOURCES"] = str(int(n_sources))
         else:
             # Retrieving the number of `source#.il` parameters
-            params_dic = {k: v for arg in args if isinstance(arg, dict) for k, v in arg.items()}
-            n_sources = len([k for k in params_dic if 'source' in k and k.endswith('.il')])
+            params_dic = {
+                k: v for arg in args if isinstance(arg, dict) for k, v in arg.items()
+            }
+            n_sources = len(
+                [k for k in params_dic if "source" in k and k.endswith(".il")]
+            )
             if n_sources >= 1:
-                os.environ['OTB_TF_NSOURCES'] = str(n_sources)
+                os.environ["OTB_TF_NSOURCES"] = str(n_sources)
 
-    def __init__(self, app_name, *args, n_sources=None, **kwargs):
+    def __init__(self, name: str, *args, n_sources: int = None, **kwargs):
         """Constructor for an OTBTFApp object.
 
         Args:
-            app_name: name of the OTBTF app
+            name: name of the OTBTF app
             *args: arguments (dict). NB: we don't need kwargs because it cannot contain source#.il
             n_sources: number of sources. Default is None (resolves the number of sources based on the
                        content of the dict passed in args, where some 'source' str is found)
             **kwargs: kwargs
+
         """
         self.set_nb_sources(*args, n_sources=n_sources)
-        super().__init__(app_name, *args, **kwargs)
+        super().__init__(name, *args, **kwargs)
 
 
-for _app in AVAILABLE_APPLICATIONS:
-    # Customize the behavior for some OTBTF applications. The user doesn't need to set the env variable
-    # `OTB_TF_NSOURCES`, it is handled in pyotb
-    if _app == 'TensorflowModelServe':
-        class TensorflowModelServe(OTBTFApp):
-            """Serve a Tensorflow model using OTBTF."""
-            def __init__(self, *args, n_sources=None, **kwargs):
-                """Constructor for a TensorflowModelServe object."""
-                super().__init__('TensorflowModelServe', *args, n_sources=n_sources, **kwargs)
-
-    elif _app == 'PatchesExtraction':
-        class PatchesExtraction(OTBTFApp):
-            """Extract patches using OTBTF."""
-            def __init__(self, *args, n_sources=None, **kwargs):
-                """Constructor for a PatchesExtraction object."""
-                super().__init__('PatchesExtraction', *args, n_sources=n_sources, **kwargs)
-
-    elif _app == 'TensorflowModelTrain':
-        class TensorflowModelTrain(OTBTFApp):
-            """Train a Tensorflow model using OTBTF."""
-            def __init__(self, *args, n_sources=None, **kwargs):
-                """Constructor for a TensorflowModelTrain object."""
-                super().__init__('TensorflowModelTrain', *args, n_sources=n_sources, **kwargs)
+AVAILABLE_APPLICATIONS = get_available_applications(as_subprocess=True)
+
+# This is to enable aliases of Apps, i.e. using apps like `pyotb.AppName(...)` instead of `pyotb.App("AppName", ...)`
+_CODE_TEMPLATE = (
+    """
+class {name}(App):
+    """
+    """
+    def __init__(self, *args, **kwargs):
+        super().__init__('{name}', *args, **kwargs)
+"""
+)
 
+for _app in AVAILABLE_APPLICATIONS:
+    # Customize the behavior for some OTBTF applications. `OTB_TF_NSOURCES` is now handled by pyotb
+    if _app in ("PatchesExtraction", "TensorflowModelTrain", "TensorflowModelServe"):
+        exec(  # pylint: disable=exec-used
+            _CODE_TEMPLATE.format(name=_app).replace("(App)", "(OTBTFApp)")
+        )
     # Default behavior for any OTB application
     else:
         exec(_CODE_TEMPLATE.format(name=_app))  # pylint: disable=exec-used
```

### Comparing `pyotb-1.5.4/pyotb/core.py` & `pyotb-2.0.0.dev1/pyotb/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,493 +1,320 @@
 # -*- coding: utf-8 -*-
 """This module is the core of pyotb."""
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from ast import literal_eval
 from pathlib import Path
+from time import perf_counter
+from typing import Any
 
 import numpy as np
-import otbApplication as otb
+import otbApplication as otb  # pylint: disable=import-error
 
 from .helpers import logger
 
 
-class otbObject:
-    """Base class that gathers common operations for any OTB in-memory raster."""
-    _name = ""
-    app = None
-    output_param = ""
+class OTBObject(ABC):
+    """Abstraction of an image object."""
 
     @property
-    def name(self):
-        """Application name that will be printed in logs.
-
-        Returns:
-            user's defined name or appname
+    @abstractmethod
+    def name(self) -> str:
+        """By default, should return the application name, but a custom name may be passed during init."""
 
-        """
-        return self._name or self.app.GetName()
+    @property
+    @abstractmethod
+    def app(self) -> otb.Application:
+        """Reference to the main (or last in pipeline) otb.Application instance linked to this object."""
 
-    @name.setter
-    def name(self, val):
-        """Set custom name.
+    @property
+    @abstractmethod
+    def output_image_key(self) -> str:
+        """Return the name of a parameter key associated to the main output image of the object."""
 
-        Args:
-          val: new name
+    @property
+    @abstractmethod
+    def exports_dic(self) -> dict[str, dict]:
+        """Return an internal dict object containing np.array exports, to avoid duplicated ExportImage() calls."""
 
-        """
-        self._name = val
+    @property
+    def metadata(self) -> dict[str, (str, float, list[float])]:
+        """Return first output image metadata dictionary."""
+        return dict(self.app.GetMetadataDictionary(self.output_image_key))
 
     @property
-    def dtype(self):
-        """Expose the pixel type of an output image using numpy convention.
+    def dtype(self) -> np.dtype:
+        """Expose the pixel type of output image using numpy convention.
 
         Returns:
             dtype: pixel type of the output image
 
         """
-        try:
-            enum = self.app.GetParameterOutputImagePixelType(self.output_param)
-            return self.app.ConvertPixelTypeToNumpy(enum)
-        except RuntimeError:
-            return None
+        enum = self.app.GetParameterOutputImagePixelType(self.output_image_key)
+        return self.app.ConvertPixelTypeToNumpy(enum)
 
     @property
-    def shape(self):
+    def shape(self) -> tuple[int]:
         """Enables to retrieve the shape of a pyotb object using numpy convention.
 
         Returns:
             shape: (height, width, bands)
 
         """
-        width, height = self.app.GetImageSize(self.output_param)
-        bands = self.app.GetImageNbBands(self.output_param)
-        return (height, width, bands)
-
-    def write(self, *args, filename_extension="", pixel_type=None, **kwargs):
-        """Trigger execution, set output pixel type and write the output.
+        width, height = self.app.GetImageSize(self.output_image_key)
+        bands = self.app.GetImageNbBands(self.output_image_key)
+        return height, width, bands
 
-        Args:
-            *args: Can be : - dictionary containing key-arguments enumeration. Useful when a key contains
-                              non-standard characters such as a point, e.g. {'io.out':'output.tif'}
-                            - string, useful when there is only one output, e.g. 'output.tif'
-                            - None if output file was passed during App init
-            filename_extension: Optional, an extended filename as understood by OTB (e.g. "&gdal:co:TILED=YES")
-                                Will be used for all outputs (Default value = "")
-            pixel_type: Can be : - dictionary {output_parameter_key: pixeltype} when specifying for several outputs
-                                 - str (e.g. 'uint16') or otbApplication.ImagePixelType_... When there are several
-                                   outputs, all outputs are written with this unique type.
-                                   Valid pixel types are uint8, uint16, uint32, int16, int32, float, double,
-                                   cint16, cint32, cfloat, cdouble. (Default value = None)
-            **kwargs: keyword arguments e.g. out='output.tif'
-        """
-        # Gather all input arguments in kwargs dict
-        for arg in args:
-            if isinstance(arg, dict):
-                kwargs.update(arg)
-            elif isinstance(arg, str) and kwargs:
-                logger.warning('%s: keyword arguments specified, ignoring argument "%s"', self.name, arg)
-            elif isinstance(arg, str):
-                kwargs.update({self.output_param: arg})
-
-        dtypes = {}
-        if isinstance(pixel_type, dict):
-            dtypes = {k: parse_pixel_type(v) for k, v in pixel_type.items()}
-        elif pixel_type is not None:
-            typ = parse_pixel_type(pixel_type)
-            if isinstance(self, App):
-                dtypes = {key: typ for key in self.output_parameters_keys}
-            elif isinstance(self, otbObject):
-                dtypes = {self.output_param: typ}
-
-        if filename_extension:
-            logger.debug('%s: using extended filename for outputs: %s', self.name, filename_extension)
-            if not filename_extension.startswith('?'):
-                filename_extension = "?" + filename_extension
-
-        # Case output parameter was set during App init
-        if not kwargs:
-            if self.output_param in self.parameters:
-                if dtypes:
-                    self.app.SetParameterOutputImagePixelType(self.output_param, dtypes[self.output_param])
-                if filename_extension:
-                    new_val = self.parameters[self.output_param] + filename_extension
-                    self.app.SetParameterString(self.output_param, new_val)
-            else:
-                raise ValueError(f'{self.app.GetName()}: Output parameter is missing.')
-
-        # Parse kwargs
-        for key, output_filename in kwargs.items():
-            # Stop process if a bad parameter is given
-            if key not in self.app.GetParametersKeys():
-                raise KeyError(f'{self.app.GetName()}: Unknown parameter key "{key}"')
-            # Check if extended filename was not provided twice
-            if '?' in output_filename and filename_extension:
-                logger.warning('%s: extended filename was provided twice. Using the one found in path.', self.name)
-            elif filename_extension:
-                output_filename += filename_extension
-
-            logger.debug('%s: "%s" parameter is %s', self.name, key, output_filename)
-            self.app.SetParameterString(key, output_filename)
-
-            if key in dtypes:
-                self.app.SetParameterOutputImagePixelType(key, dtypes[key])
+    @property
+    def transform(self) -> tuple[int]:
+        """Get image affine transform, rasterio style (see https://www.perrygeo.com/python-affine-transforms.html).
 
-        logger.debug('%s: flushing data to disk', self.name)
-        try:
-            self.app.WriteOutput()
-        except RuntimeError:
-            logger.debug('%s: failed to simply write output, executing once again then writing', self.name)
-            self.app.ExecuteAndWriteOutput()
+        Returns:
+            transform: (X spacing, X offset, X origin, Y offset, Y spacing, Y origin)
+        """
+        spacing_x, spacing_y = self.app.GetImageSpacing(self.output_image_key)
+        origin_x, origin_y = self.app.GetImageOrigin(self.output_image_key)
+        # Shift image origin since OTB is giving coordinates of pixel center instead of corners
+        origin_x, origin_y = origin_x - spacing_x / 2, origin_y - spacing_y / 2
+        return spacing_x, 0.0, origin_x, 0.0, spacing_y, origin_y
 
-    def to_numpy(self, preserve_dtype=True, copy=False):
+    def get_info(self) -> dict[str, (str, float, list[float])]:
+        """Return a dict output of ReadImageInfo for the first image output."""
+        return App("ReadImageInfo", self, quiet=True).data
+
+    def get_statistics(self) -> dict[str, (str, float, list[float])]:
+        """Return a dict output of ComputeImagesStatistics for the first image output."""
+        return App("ComputeImagesStatistics", self, quiet=True).data
+
+    def get_values_at_coords(
+        self, row: int, col: int, bands: int = None
+    ) -> list[int | float] | int | float:
+        """Get pixel value(s) at a given YX coordinates.
+
+        Args:
+            row: index along Y / latitude axis
+            col: index along X / longitude axis
+            bands: band number, list or slice to fetch values from
+
+        Returns:
+            single numerical value or a list of values for each band
+
+        """
+        channels = []
+        app = App("PixelValue", self, coordx=col, coordy=row, frozen=True, quiet=True)
+        if bands is not None:
+            if isinstance(bands, int):
+                if bands < 0:
+                    bands = self.shape[2] + bands
+                channels = [bands]
+            elif isinstance(bands, slice):
+                channels = self.channels_list_from_slice(bands)
+            elif not isinstance(bands, list):
+                raise TypeError(
+                    f"{self.name}: type '{type(bands)}' cannot be interpreted as a valid slicing"
+                )
+            if channels:
+                app.app.Execute()
+                app.set_parameters({"cl": [f"Channel{n + 1}" for n in channels]})
+        app.execute()
+        data = literal_eval(app.app.GetParameterString("value"))
+        return data[0] if len(channels) == 1 else data
+
+    def channels_list_from_slice(self, bands: int) -> list[int]:
+        """Get list of channels to read values at, from a slice."""
+        nb_channels = self.shape[2]
+        start, stop, step = bands.start, bands.stop, bands.step
+        start = nb_channels + start if isinstance(start, int) and start < 0 else start
+        stop = nb_channels + stop if isinstance(stop, int) and stop < 0 else stop
+        step = 1 if step is None else step
+        if start is not None and stop is not None:
+            return list(range(start, stop, step))
+        if start is not None and stop is None:
+            return list(range(start, nb_channels, step))
+        if start is None and stop is not None:
+            return list(range(0, stop, step))
+        if start is None and stop is None:
+            return list(range(0, nb_channels, step))
+        raise ValueError(
+            f"{self.name}: '{bands}' cannot be interpreted as valid slicing."
+        )
+
+    def export(
+        self, key: str = None, preserve_dtype: bool = True
+    ) -> dict[str, dict[str, np.ndarray]]:
+        """Export a specific output image as numpy array and store it in object exports_dic.
+
+        Args:
+            key: parameter key to export, if None then the default one will be used
+            preserve_dtype: when set to True, the numpy array is converted to the same pixel type as
+                            the App first output. Default is True
+
+        Returns:
+            the exported numpy array
+
+        """
+        if key is None:
+            key = self.output_image_key
+        if key not in self.exports_dic:
+            self.exports_dic[key] = self.app.ExportImage(key)
+        if preserve_dtype:
+            self.exports_dic[key]["array"] = self.exports_dic[key]["array"].astype(
+                self.dtype
+            )
+        return self.exports_dic[key]
+
+    def to_numpy(
+        self, key: str = None, preserve_dtype: bool = True, copy: bool = False
+    ) -> np.ndarray:
         """Export a pyotb object to numpy array.
 
         Args:
-            preserve_dtype: when set to True, the numpy array is created with the same pixel type as
-                                  the otbObject first output. Default is True.
+            key: the output parameter name to export as numpy array
+            preserve_dtype: when set to True, the numpy array is converted to the same pixel type as
+                            the App first output. Default is True
             copy: whether to copy the output array, default is False
                   required to True if preserve_dtype is False and the source app reference is lost
 
         Returns:
-          a numpy array
+            a numpy array
 
         """
-        array = self.app.ExportImage(self.output_param)['array']
-        if preserve_dtype:
-            return array.astype(self.dtype)
-        if copy:
-            return array.copy()
-        return array
+        data = self.export(key, preserve_dtype)
+        return data["array"].copy() if copy else data["array"]
 
-    def to_rasterio(self):
+    def to_rasterio(self) -> tuple[np.ndarray, dict[str, Any]]:
         """Export image as a numpy array and its metadata compatible with rasterio.
 
         Returns:
           array : a numpy array in the (bands, height, width) order
           profile: a metadata dict required to write image using rasterio
 
         """
+        profile = {}
         array = self.to_numpy(preserve_dtype=True, copy=False)
-        array = np.moveaxis(array, 2, 0)
-        proj = self.app.GetImageProjection(self.output_param)
-        spacing_x, spacing_y = self.app.GetImageSpacing(self.output_param)
-        origin_x, origin_y = self.app.GetImageOrigin(self.output_param)
-        # Shift image origin since OTB is giving coordinates of pixel center instead of corners
-        origin_x, origin_y = origin_x - spacing_x / 2, origin_y - spacing_y / 2
-        profile = {
-            'crs': proj, 'dtype': array.dtype,
-            'count': array.shape[0], 'height': array.shape[1], 'width': array.shape[2],
-            'transform': (spacing_x, 0.0, origin_x, 0.0, spacing_y, origin_y)  # here we force pixel rotation to 0 !
-        }
-        return array, profile
+        proj = self.app.GetImageProjection(self.output_image_key)
+        profile.update({"crs": proj, "dtype": array.dtype, "transform": self.transform})
+        height, width, count = array.shape
+        profile.update({"count": count, "height": height, "width": width})
+        return np.moveaxis(array, 2, 0), profile
 
-    # Special methods
-    def __getitem__(self, key):
-        """Override the default __getitem__ behaviour.
-
-        This function enables 2 things :
-        - access attributes like that : object['any_attribute']
-        - slicing, i.e. selecting ROI/bands. For example, selecting first 3 bands: object[:, :, :3]
-                                                          selecting bands 1, 2 & 5 : object[:, :, [0, 1, 4]]
-                                                          selecting 1000x1000 subset : object[:1000, :1000]
+    def get_rowcol_from_xy(self, x: float, y: float) -> tuple[int, int]:
+        """Find (row, col) index using (x, y) projected coordinates - image CRS is expected.
 
         Args:
-            key: attribute key
-
-        Returns:
-            attribute or Slicer
-        """
-        # Accessing string attributes
-        if isinstance(key, str):
-            return self.__dict__.get(key)
-        # Slicing
-        if not isinstance(key, tuple) or (isinstance(key, tuple) and (len(key) < 2 or len(key) > 3)):
-            raise ValueError(f'"{key}"cannot be interpreted as valid slicing. Slicing should be 2D or 3D.')
-        if isinstance(key, tuple) and len(key) == 2:
-            # Adding a 3rd dimension
-            key = key + (slice(None, None, None),)
-        (rows, cols, channels) = key
-        return Slicer(self, rows, cols, channels)
-
-    def __getattr__(self, name):
-        """This method is called when the default attribute access fails.
-
-        We choose to access the attribute `name` of self.app.
-        Thus, any method of otbApplication can be used transparently on otbObject objects,
-        e.g. SetParameterOutputImagePixelType() or ExportImage() work
-
-        Args:
-            name: attribute name
-
-        Returns:
-            attribute
-
-        Raises:
-            AttributeError: when `name` is not an attribute of self.app
-
-        """
-        try:
-            res = getattr(self.app, name)
-            return res
-        except AttributeError as e:
-            raise AttributeError(f'{self.name}: could not find attribute `{name}`') from e
-
-    def __add__(self, other):
-        """Overrides the default addition and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             self + other
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('+', self, other)
-
-    def __sub__(self, other):
-        """Overrides the default subtraction and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             self - other
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('-', self, other)
-
-    def __mul__(self, other):
-        """Overrides the default subtraction and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
+            x: longitude or projected X
+            y: latitude or projected Y
 
         Returns:
-             self * other
-
+            pixel index: (row, col)
         """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('*', self, other)
-
-    def __truediv__(self, other):
-        """Overrides the default subtraction and flavours it with BandMathX.
+        spacing_x, _, origin_x, _, spacing_y, origin_y = self.transform
+        row, col = (origin_y - y) / spacing_y, (x - origin_x) / spacing_x
+        return abs(int(row)), int(col)
 
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             self / other
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('/', self, other)
-
-    def __radd__(self, other):
-        """Overrides the default reverse addition and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             other + self
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('+', other, self)
-
-    def __rsub__(self, other):
-        """Overrides the default subtraction and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             other - self
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('-', other, self)
-
-    def __rmul__(self, other):
-        """Overrides the default multiplication and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             other * self
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('*', other, self)
-
-    def __rtruediv__(self, other):
-        """Overrides the default division and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             other / self
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return Operation('/', other, self)
-
-    def __abs__(self):
-        """Overrides the default abs operator and flavours it with BandMathX.
-
-        Returns:
-            abs(self)
-
-        """
-        return Operation('abs', self)
-
-    def __ge__(self, other):
-        """Overrides the default greater or equal and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             self >= other
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('>=', self, other)
-
-    def __le__(self, other):
-        """Overrides the default less or equal and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             self <= other
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('<=', self, other)
-
-    def __gt__(self, other):
-        """Overrides the default greater operator and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
-
-        Returns:
-             self > other
-
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('>', self, other)
-
-    def __lt__(self, other):
-        """Overrides the default less operator and flavours it with BandMathX.
+    @staticmethod
+    def __create_operator(op_cls, name, x, y) -> Operation:
+        """Create an operator.
 
         Args:
-            other: the other member of the operation
+            op_cls: Operator class
+            name: operator expression
+            x: first element
+            y: second element
 
-        Returns:
-             self < other
+        Return:
+            operator
 
         """
-        if isinstance(other, (np.ndarray, np.generic)):
+        if isinstance(y, (np.ndarray, np.generic)):
             return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('<', self, other)
-
-    def __eq__(self, other):
-        """Overrides the default eq operator and flavours it with BandMathX.
-
-        Args:
-            other: the other member of the operation
+        return op_cls(name, x, y)
 
-        Returns:
-             self == other
+    def __add__(self, other: OTBObject | str | int | float) -> Operation:
+        """Addition."""
+        return self.__create_operator(Operation, "+", self, other)
 
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('==', self, other)
+    def __sub__(self, other: OTBObject | str | int | float) -> Operation:
+        """Subtraction."""
+        return self.__create_operator(Operation, "-", self, other)
 
-    def __ne__(self, other):
-        """Overrides the default different operator and flavours it with BandMathX.
+    def __mul__(self, other: OTBObject | str | int | float) -> Operation:
+        """Multiplication."""
+        return self.__create_operator(Operation, "*", self, other)
 
-        Args:
-            other: the other member of the operation
+    def __truediv__(self, other: OTBObject | str | int | float) -> Operation:
+        """Division."""
+        return self.__create_operator(Operation, "/", self, other)
 
-        Returns:
-             self != other
+    def __radd__(self, other: OTBObject | str | int | float) -> Operation:
+        """Right addition."""
+        return self.__create_operator(Operation, "+", other, self)
 
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('!=', self, other)
+    def __rsub__(self, other: OTBObject | str | int | float) -> Operation:
+        """Right subtraction."""
+        return self.__create_operator(Operation, "-", other, self)
 
-    def __or__(self, other):
-        """Overrides the default or operator and flavours it with BandMathX.
+    def __rmul__(self, other: OTBObject | str | int | float) -> Operation:
+        """Right multiplication."""
+        return self.__create_operator(Operation, "*", other, self)
 
-        Args:
-            other: the other member of the operation
+    def __rtruediv__(self, other: OTBObject | str | int | float) -> Operation:
+        """Right division."""
+        return self.__create_operator(Operation, "/", other, self)
 
-        Returns:
-             self || other
+    def __abs__(self) -> Operation:
+        """Absolute value."""
+        return Operation("abs", self)
 
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('||', self, other)
+    def __ge__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Greater of equal than."""
+        return self.__create_operator(LogicalOperation, ">=", self, other)
 
-    def __and__(self, other):
-        """Overrides the default and operator and flavours it with BandMathX.
+    def __le__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Lower of equal than."""
+        return self.__create_operator(LogicalOperation, "<=", self, other)
 
-        Args:
-            other: the other member of the operation
+    def __gt__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Greater than."""
+        return self.__create_operator(LogicalOperation, ">", self, other)
 
-        Returns:
-             self && other
+    def __lt__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Lower than."""
+        return self.__create_operator(LogicalOperation, "<", self, other)
 
-        """
-        if isinstance(other, (np.ndarray, np.generic)):
-            return NotImplemented  # this enables to fallback on numpy emulation thanks to __array_ufunc__
-        return logicalOperation('&&', self, other)
+    def __eq__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Equality."""
+        return self.__create_operator(LogicalOperation, "==", self, other)
 
-    # TODO: other operations ?
-    #  e.g. __pow__... cf https://docs.python.org/3/reference/datamodel.html#emulating-numeric-types
+    def __ne__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Inequality."""
+        return self.__create_operator(LogicalOperation, "!=", self, other)
 
-    def __hash__(self):
-        """Override the default behaviour of the hash function.
+    def __or__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Logical or."""
+        return self.__create_operator(LogicalOperation, "||", self, other)
 
-        Returns:
-            self hash
+    def __and__(self, other: OTBObject | str | int | float) -> LogicalOperation:
+        """Logical and."""
+        return self.__create_operator(LogicalOperation, "&&", self, other)
 
-        """
-        return id(self)
+    # Some other operations could be implemented with the same pattern
+    # e.g. __pow__... cf https://docs.python.org/3/reference/datamodel.html#emulating-numeric-types
 
-    def __array__(self):
+    def __array__(self) -> np.ndarray:
         """This is called when running np.asarray(pyotb_object).
 
         Returns:
             a numpy array
 
         """
         return self.to_numpy()
 
-    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs) -> App:
         """This is called whenever a numpy function is called on a pyotb object.
 
         Operation is performed in numpy, then imported back to pyotb with the same georeference as input.
 
         Args:
             ufunc: numpy function
             method: an internal numpy argument
@@ -495,449 +322,716 @@
                     the same georeference and pixel size.
             **kwargs: kwargs of the numpy function
 
         Returns:
             a pyotb object
 
         """
-        if method == '__call__':
+        if method == "__call__":
             # Converting potential pyotb inputs to arrays
             arrays = []
             image_dic = None
             for inp in inputs:
                 if isinstance(inp, (float, int, np.ndarray, np.generic)):
                     arrays.append(inp)
-                elif isinstance(inp, otbObject):
-                    image_dic = inp.app.ExportImage(self.output_param)
-                    array = image_dic['array']
-                    arrays.append(array)
+                elif isinstance(inp, OTBObject):
+                    image_dic = inp.export()
+                    arrays.append(image_dic["array"])
                 else:
-                    print(type(self))
+                    logger.debug(type(self))
                     return NotImplemented
-
             # Performing the numpy operation
             result_array = ufunc(*arrays, **kwargs)
             result_dic = image_dic
-            result_dic['array'] = result_array
-
-            # Importing back to OTB
-            app = App('ExtractROI', frozen=True, image_dic=result_dic)  # pass the result_dic just to keep reference
+            result_dic["array"] = result_array
+            # Importing back to OTB, pass the result_dic just to keep reference
+            pyotb_app = App("ExtractROI", frozen=True, quiet=True)
             if result_array.shape[2] == 1:
-                app.ImportImage('in', result_dic)
+                pyotb_app.app.ImportImage("in", result_dic)
             else:
-                app.ImportVectorImage('in', result_dic)
-            app.execute()
-            return app
-
+                pyotb_app.app.ImportVectorImage("in", result_dic)
+            pyotb_app.execute()
+            return pyotb_app
         return NotImplemented
 
-    def summarize(self):
-        """Return a nested dictionary summarizing the otbObject.
+    def __hash__(self) -> int:
+        """Override the default behaviour of the hash function.
 
         Returns:
-            Nested dictionary summarizing the otbObject
+            self hash
 
         """
-        params = self.parameters
-        for k, p in params.items():
-            # In the following, we replace each parameter which is an otbObject, with its summary.
-            if isinstance(p, otbObject):  # single parameter
-                params[k] = p.summarize()
-            elif isinstance(p, list):  # parameter list
-                params[k] = [pi.summarize() if isinstance(pi, otbObject) else pi for pi in p]
+        return id(self)
+
+    def __getitem__(self, key) -> Any | list[float] | float | Slicer:
+        """Override the default __getitem__ behaviour.
+
+        This function enables 2 things :
+        - slicing, i.e. selecting ROI/bands. For example, selecting first 3 bands: object[:, :, :3]
+                                                          selecting bands 1, 2 & 5 : object[:, :, [0, 1, 4]]
+                                                          selecting 1000x1000 subset : object[:1000, :1000]
+        - access pixel value(s) at a specified row, col index
 
-        return {"name": self.name, "parameters": params}
+        Args:
+            key: attribute key
 
+        Returns:
+            list of pixel values if vector image, or pixel value, or Slicer
+
+        """
+        # Accessing pixel value(s) using Y/X coordinates
+        if isinstance(key, tuple) and len(key) >= 2:
+            row, col = key[0], key[1]
+            if isinstance(row, int) and isinstance(col, int):
+                if row < 0 or col < 0:
+                    raise ValueError(
+                        f"{self.name} cannot read pixel value at negative coordinates ({row}, {col})"
+                    )
+                channels = key[2] if len(key) == 3 else None
+                return self.get_values_at_coords(row, col, channels)
+        # Slicing
+        if not isinstance(key, tuple) or (
+            isinstance(key, tuple) and (len(key) < 2 or len(key) > 3)
+        ):
+            raise ValueError(
+                f'"{key}" cannot be interpreted as valid slicing. Slicing should be 2D or 3D.'
+            )
+        if isinstance(key, tuple) and len(key) == 2:
+            # Adding a 3rd dimension
+            key = key + (slice(None, None, None),)
+        return Slicer(self, *key)
 
-class App(otbObject):
-    """Class of an OTB app."""
-    def __init__(self, appname, *args, frozen=False, quiet=False,
-                 preserve_dtype=False, image_dic=None, **kwargs):
-        """Enables to init an OTB application as a oneliner. Handles in-memory connection between apps.
+    def __repr__(self) -> str:
+        """Return a string representation with object id, this is a key used to store image ref in Operation dicts."""
+        return f"<pyotb.{self.__class__.__name__} object, id {id(self)}>"
+
+
+class App(OTBObject):
+    """Base class that gathers common operations for any OTB application."""
+
+    INPUT_IMAGE_TYPES = [
+        # Images only
+        otb.ParameterType_InputImage,
+        otb.ParameterType_InputImageList,
+    ]
+    INPUT_PARAM_TYPES = INPUT_IMAGE_TYPES + [
+        # Vectors
+        otb.ParameterType_InputVectorData,
+        otb.ParameterType_InputVectorDataList,
+        # Filenames
+        otb.ParameterType_InputFilename,
+        otb.ParameterType_InputFilenameList,
+    ]
+
+    OUTPUT_IMAGE_TYPES = [
+        # Images only
+        otb.ParameterType_OutputImage
+    ]
+    OUTPUT_PARAM_TYPES = OUTPUT_IMAGE_TYPES + [
+        # Vectors
+        otb.ParameterType_OutputVectorData,
+        # Filenames
+        otb.ParameterType_OutputFilename,
+    ]
+
+    INPUT_LIST_TYPES = [
+        otb.ParameterType_InputImageList,
+        otb.ParameterType_StringList,
+        otb.ParameterType_InputFilenameList,
+        otb.ParameterType_ListView,
+        otb.ParameterType_InputVectorDataList,
+    ]
+    INPUT_IMAGES_LIST_TYPES = [
+        otb.ParameterType_InputImageList,
+        otb.ParameterType_InputFilenameList,
+    ]
+
+    def __init__(
+        self,
+        appname: str,
+        *args,
+        frozen: bool = False,
+        quiet: bool = False,
+        name: str = "",
+        **kwargs,
+    ):
+        """Common constructor for OTB applications. Handles in-memory connection between apps.
 
         Args:
-            appname: name of the app, e.g. 'Smoothing'
+            appname: name of the OTB application to initialize, e.g. 'BandMath'
             *args: used for passing application parameters. Can be :
                            - dictionary containing key-arguments enumeration. Useful when a key is python-reserved
                              (e.g. "in") or contains reserved characters such as a point (e.g."mode.extent.unit")
                            - string, App or Output, useful when the user wants to specify the input "in"
                            - list, useful when the user wants to specify the input list 'il'
             frozen: freeze OTB app in order to use execute() later and avoid blocking process during __init___
             quiet: whether to print logs of the OTB app
-            preserve_dtype: propagate the pixel type from inputs to output. If several inputs, the type of an
-                                  arbitrary input is considered. If several outputs, all will have the same type.
-            image_dic: enables to keep a reference to image_dic. image_dic is a dictionary, such as
-                       the result of app.ExportImage(). Use it when the app takes a numpy array as input.
-                       See this related issue for why it is necessary to keep reference of object:
-                       https://gitlab.orfeo-toolbox.org/orfeotoolbox/otb/-/issues/1824
+            name: custom name that will show up in logs, appname will be used if not provided
+
             **kwargs: used for passing application parameters.
                       e.g. il=['input1.tif', App_object2, App_object3.out], out='output.tif'
 
         """
-        self.appname = appname
-        self.frozen = frozen
-        self.quiet = quiet
-        self.preserve_dtype = preserve_dtype
-        self.image_dic = image_dic
-        if self.quiet:
-            self.app = otb.Registry.CreateApplicationWithoutLogger(appname)
-        else:
-            self.app = otb.Registry.CreateApplication(appname)
-        self.description = self.app.GetDocLongDescription()
-        self.output_parameters_keys = self.__get_output_parameters_keys()
-        if self.output_parameters_keys:
-            self.output_param = self.output_parameters_keys[0]
-
-        self.parameters = {}
-        if (args or kwargs):
+        # Attributes and data structures used by properties
+        create = (
+            otb.Registry.CreateApplicationWithoutLogger
+            if quiet
+            else otb.Registry.CreateApplication
+        )
+        self._app = create(appname)
+        self._name = name or appname
+        self._exports_dic = {}
+        self._settings, self._auto_parameters = {}, {}
+        self._time_start, self._time_end = 0.0, 0.0
+        self.data, self.outputs = {}, {}
+        self.quiet, self.frozen = quiet, frozen
+        # Param keys and types
+        self.parameters_keys = tuple(self.app.GetParametersKeys())
+        self._all_param_types = {
+            k: self.app.GetParameterType(k) for k in self.parameters_keys
+        }
+        types = (
+            otb.ParameterType_OutputImage,
+            otb.ParameterType_OutputVectorData,
+            otb.ParameterType_OutputFilename,
+        )
+        self._out_param_types = {
+            k: v for k, v in self._all_param_types.items() if v in types
+        }
+        # Init, execute and write (auto flush only when output param was provided)
+        if args or kwargs:
             self.set_parameters(*args, **kwargs)
+        # Create Output image objects
+        for key in filter(
+            lambda k: self._out_param_types[k] == otb.ParameterType_OutputImage,
+            self._out_param_types,
+        ):
+            self.outputs[key] = Output(self, key, self._settings.get(key))
         if not self.frozen:
             self.execute()
+            if any(key in self._settings for key in self._out_param_types):
+                self.flush()
+
+    @property
+    def name(self) -> str:
+        """Returns appname by default, or a custom name if passed during App init."""
+        return self._name
+
+    @property
+    def app(self) -> otb.Application:
+        """Property to return an internal _app instance."""
+        return self._app
+
+    @property
+    def parameters(self):
+        """Return used OTB application parameters."""
+        return {**self._auto_parameters, **self.app.GetParameters(), **self._settings}
+
+    @property
+    def exports_dic(self) -> dict[str, dict]:
+        """Returns internal _exports_dic object that contains numpy array exports."""
+        return self._exports_dic
+
+    def __is_one_of_types(self, key: str, param_types: list[int]) -> bool:
+        """Helper to factor is_input and is_output."""
+        if key not in self._all_param_types:
+            raise KeyError(f"key {key} not found in the application parameters types")
+        return self._all_param_types[key] in param_types
+
+    def is_input(self, key: str) -> bool:
+        """Returns True if the key is an input.
+
+        Args:
+            key: parameter key
+
+        Returns:
+            True if the parameter is an input, else False
+
+        """
+        return self.__is_one_of_types(key=key, param_types=self.INPUT_PARAM_TYPES)
+
+    def is_output(self, key: str) -> bool:
+        """Returns True if the key is an output.
+
+        Args:
+            key: parameter key
+
+        Returns:
+            True if the parameter is an output, else False
+
+        """
+        return self.__is_one_of_types(key=key, param_types=self.OUTPUT_PARAM_TYPES)
+
+    def is_key_list(self, key: str) -> bool:
+        """Check if a parameter key is an input parameter list."""
+        return self.app.GetParameterType(key) in self.INPUT_LIST_TYPES
+
+    def is_key_images_list(self, key: str) -> bool:
+        """Check if a parameter key is an input parameter image list."""
+        return self.app.GetParameterType(key) in self.INPUT_IMAGES_LIST_TYPES
+
+    def get_first_key(self, param_types: list[int]) -> str:
+        """Get the first param key for specific file types, try each list in args."""
+        for param_type in param_types:
+            # Return the first key, from the alphabetically sorted keys of the
+            # application, which has the parameter type matching param_type.
+            for key, value in sorted(self._all_param_types.items()):
+                if value == param_type:
+                    return key
+        raise TypeError(
+            f"{self.name}: could not find any parameter key matching the provided types"
+        )
+
+    @property
+    def input_key(self) -> str:
+        """Get the name of first input parameter, raster > vector > file."""
+        return self.get_first_key(self.INPUT_PARAM_TYPES)
+
+    @property
+    def input_image_key(self) -> str:
+        """Name of the first input image parameter."""
+        return self.get_first_key(self.INPUT_IMAGE_TYPES)
+
+    @property
+    def output_key(self) -> str:
+        """Name of the first output parameter, raster > vector > file."""
+        return self.get_first_key(self.OUTPUT_PARAM_TYPES)
+
+    @property
+    def output_image_key(self) -> str:
+        """Get the name of first output image parameter."""
+        return self.get_first_key(self.OUTPUT_IMAGE_TYPES)
+
+    @property
+    def elapsed_time(self) -> float:
+        """Get elapsed time between app init and end of exec or file writing."""
+        return self._time_end - self._time_start
 
     def set_parameters(self, *args, **kwargs):
         """Set some parameters of the app.
 
         When useful, e.g. for images list, this function appends the parameters
         instead of overwriting them. Handles any parameters, i.e. in-memory & filepaths
 
         Args:
             *args: Can be : - dictionary containing key-arguments enumeration. Useful when a key is python-reserved
                               (e.g. "in") or contains reserved characters such as a point (e.g."mode.extent.unit")
-                            - string, App or Output, useful when the user implicitly wants to set the param "in"
+                            - string or OTBObject, useful when the user implicitly wants to set the param "in"
                             - list, useful when the user implicitly wants to set the param "il"
             **kwargs: keyword arguments e.g. il=['input1.tif', oApp_object2, App_object3.out], out='output.tif'
 
         Raises:
             Exception: when the setting of a parameter failed
 
         """
         parameters = kwargs
         parameters.update(self.__parse_args(args))
         # Going through all arguments
-        for param, obj in parameters.items():
-            if param not in self.app.GetParametersKeys():
-                raise Exception(f"{self.name}: parameter '{param}' was not recognized. "
-                                f"Available keys are {self.app.GetParametersKeys()}")
+        for key, obj in parameters.items():
+            if "_" in key:
+                key = key.replace("_", ".")
+            if key not in self.parameters_keys:
+                raise KeyError(
+                    f"{self.name}: parameter '{key}' was not recognized. Available keys are {self.parameters_keys}"
+                )
             # When the parameter expects a list, if needed, change the value to list
-            if self.__is_key_list(param) and not isinstance(obj, (list, tuple)):
-                parameters[param] = [obj]
+            if self.is_key_list(key) and not isinstance(obj, (list, tuple)):
                 obj = [obj]
-                logger.warning('%s: argument for parameter "%s" was converted to list', self.name, param)
+                logger.info(
+                    '%s: argument for parameter "%s" was converted to list',
+                    self.name,
+                    key,
+                )
             try:
-                # This is when we actually call self.app.SetParameter*
-                self.__set_param(param, obj)
+                if self.is_input(key):
+                    if self.is_key_images_list(key):
+                        self.__set_param(key, [add_vsi_prefix(p) for p in obj])
+                    else:
+                        self.__set_param(key, add_vsi_prefix(obj))
+                else:
+                    self.__set_param(key, obj)
             except (RuntimeError, TypeError, ValueError, KeyError) as e:
-                raise Exception(f"{self.name}: something went wrong before execution "
-                                f"(while setting parameter '{param}' to '{obj}')") from e
-        # Update _parameters using values from OtbApplication object
-        otb_params = self.app.GetParameters().items()
-        otb_params = {k: str(v) if isinstance(v, otb.ApplicationProxy) else v for k, v in otb_params}
-        self.parameters.update({**parameters, **otb_params})
-        # Update output images pixel types
-        if self.preserve_dtype:
-            self.__propagate_pixel_type()
+                raise RuntimeError(
+                    f"{self.name}: error before execution, while setting parameter '{key}' to '{obj}': {e})"
+                ) from e
+            # Save / update setting value and update the Output object initialized in __init__ without a filepath
+            self._settings[key] = obj
+            if key in self.outputs:
+                self.outputs[key].filepath = obj
+
+    def propagate_dtype(self, target_key: str = None, dtype: int = None):
+        """Propagate a pixel type from main input to every outputs, or to a target output key only.
+
+        With multiple inputs (if dtype is not provided), the type of the first input is considered.
+        With multiple outputs (if target_key is not provided), all outputs will be converted to the same pixel type.
+
+        Args:
+            target_key: output param key to change pixel type
+            dtype: data type to use
+
+        """
+        if not dtype:
+            param = self._settings.get(self.input_image_key)
+            if not param:
+                logger.warning(
+                    "%s: could not propagate pixel type from inputs to output",
+                    self.name,
+                )
+                return
+            if isinstance(param, (list, tuple)):
+                param = param[0]  # first image in "il"
+            try:
+                dtype = get_pixel_type(param)
+            except (TypeError, RuntimeError):
+                logger.warning(
+                    '%s: unable to identify pixel type of key "%s"', self.name, param
+                )
+                return
+        if target_key:
+            keys = [target_key]
+        else:
+            keys = [
+                k
+                for k, v in self._out_param_types.items()
+                if v == otb.ParameterType_OutputImage
+            ]
+        for key in keys:
+            self.app.SetParameterOutputImagePixelType(key, dtype)
 
     def execute(self):
         """Execute and write to disk if any output parameter has been set during init."""
         logger.debug("%s: run execute() with parameters=%s", self.name, self.parameters)
+        self._time_start = perf_counter()
         try:
             self.app.Execute()
         except (RuntimeError, FileNotFoundError) as e:
-            raise Exception(f'{self.name}: error during during app execution') from e
+            raise RuntimeError(
+                f"{self.name}: error during during app execution ({e}"
+            ) from e
         self.frozen = False
+        self._time_end = perf_counter()
         logger.debug("%s: execution ended", self.name)
-        if self.__has_output_param_key():
-            logger.debug('%s: flushing data to disk', self.name)
+        self.__sync_parameters()  # this is required for apps like ReadImageInfo or ComputeImagesStatistics
+
+    def flush(self):
+        """Flush data to disk, this is when WriteOutput is actually called."""
+        try:
+            logger.debug("%s: flushing data to disk", self.name)
             self.app.WriteOutput()
-        self.__save_objects()
+        except RuntimeError:
+            logger.debug(
+                "%s: failed with WriteOutput, executing once again with ExecuteAndWriteOutput",
+                self.name,
+            )
+            self._time_start = perf_counter()
+            self.app.ExecuteAndWriteOutput()
+        self._time_end = perf_counter()
 
-    def find_output(self):
-        """Find output files on disk using path found in parameters.
+    def write(
+        self,
+        path: str | Path | dict[str, str] = None,
+        ext_fname: str = "",
+        pixel_type: dict[str, str] | str = None,
+        preserve_dtype: bool = False,
+        **kwargs,
+    ) -> bool:
+        """Set output pixel type and write the output raster files.
+
+        Args:
+            path: Can be : - filepath, useful when there is only one output, e.g. 'output.tif'
+                           - dictionary containing key-arguments enumeration. Useful when a key contains
+                             non-standard characters such as a point, e.g. {'io.out':'output.tif'}
+                           - None if output file was passed during App init
+            ext_fname: Optional, an extended filename as understood by OTB (e.g. "&gdal:co:TILED=YES")
+                                Will be used for all outputs (Default value = "")
+            pixel_type: Can be : - dictionary {out_param_key: pixeltype} when specifying for several outputs
+                                 - str (e.g. 'uint16') or otbApplication.ImagePixelType_... When there are several
+                                   outputs, all outputs are written with this unique type.
+                                   Valid pixel types are uint8, uint16, uint32, int16, int32, float, double,
+                                   cint16, cint32, cfloat, cdouble. (Default value = None)
+            preserve_dtype: propagate main input pixel type to outputs, in case pixel_type is None
+            **kwargs: keyword arguments e.g. out='output.tif'
 
         Returns:
-            list of files found on disk
+            True if all files are found on disk
 
         """
-        files = []
-        missing = []
-        outputs = [p for p in self.output_parameters_keys if p in self.parameters]
-        for param in outputs:
-            filename = self.parameters[param]
-            # Remove filename extension
-            if '?' in filename:
-                filename = filename.split('?')[0]
-            path = Path(filename)
-            if path.exists():
-                files.append(str(path.absolute()))
-            else:
-                missing.append(str(path.absolute()))
-        if missing:
-            missing = tuple(missing)
-            for filename in missing:
-                logger.error("%s: execution seems to have failed, %s does not exist", self.name, filename)
-
-        return files
+        # Gather all input arguments in kwargs dict
+        if isinstance(path, dict):
+            kwargs.update(path)
+        elif isinstance(path, str) and kwargs:
+            logger.warning(
+                '%s: keyword arguments specified, ignoring argument "%s"',
+                self.name,
+                path,
+            )
+        elif isinstance(path, (str, Path)) and self.output_key:
+            kwargs.update({self.output_key: str(path)})
+        elif path is not None:
+            raise TypeError(f"{self.name}: unsupported filepath type ({type(path)})")
+        if not (kwargs or any(k in self._settings for k in self._out_param_types)):
+            raise KeyError(
+                f"{self.name}: at least one filepath is required, if not provided during App init"
+            )
+        parameters = kwargs.copy()
+
+        # Append filename extension to filenames
+        if ext_fname:
+            logger.debug(
+                "%s: using extended filename for outputs: %s", self.name, ext_fname
+            )
+            if not ext_fname.startswith("?"):
+                ext_fname = "?&" + ext_fname
+            elif not ext_fname.startswith("?&"):
+                ext_fname = "?&" + ext_fname[1:]
+            for key, value in kwargs.items():
+                if (
+                    self._out_param_types[key] == otb.ParameterType_OutputImage
+                    and "?" not in value
+                ):
+                    parameters[key] = value + ext_fname
+        # Manage output pixel types
+        data_types = {}
+        if pixel_type:
+            if isinstance(pixel_type, str):
+                dtype = parse_pixel_type(pixel_type)
+                type_name = self.app.ConvertPixelTypeToNumpy(dtype)
+                logger.debug(
+                    '%s: output(s) will be written with type "%s"', self.name, type_name
+                )
+                for key in parameters:
+                    if self._out_param_types[key] == otb.ParameterType_OutputImage:
+                        data_types[key] = dtype
+            elif isinstance(pixel_type, dict):
+                data_types = {
+                    key: parse_pixel_type(dtype) for key, dtype in pixel_type.items()
+                }
+        elif preserve_dtype:
+            self.propagate_dtype()  # all outputs will have the same type as the main input raster
+
+        # Set parameters and flush to disk
+        for key, filepath in parameters.items():
+            if Path(filepath.split("?")[0]).exists():
+                logger.warning("%s: overwriting file %s", self.name, filepath)
+            if key in data_types:
+                self.propagate_dtype(key, data_types[key])
+            self.set_parameters({key: filepath})
+        if self.frozen:
+            self.execute()
+        self.flush()
+        if not parameters:
+            return True
+        # Search and log missing files
+        files, missing = [], []
+        for key, filepath in parameters.items():
+            if not filepath.startswith("/vsi"):
+                filepath = Path(filepath.split("?")[0])
+                dest = files if filepath.exists() else missing
+                dest.append(str(filepath.absolute()))
+        for filename in missing:
+            logger.error(
+                "%s: execution seems to have failed, %s does not exist",
+                self.name,
+                filename,
+            )
+        return bool(files) and not missing
 
     # Private functions
-    def __get_output_parameters_keys(self):
-        """Get raster output parameter keys.
-
-        Returns:
-            output parameters keys
-        """
-        return [param for param in self.app.GetParametersKeys()
-                if self.app.GetParameterType(param) == otb.ParameterType_OutputImage]
-
-    def __has_output_param_key(self):
-        """Check if App has any output parameter key."""
-        if not self.output_param:
-            return True  # apps like ReadImageInfo with no filetype output param still needs to WriteOutput
-        types = (otb.ParameterType_OutputFilename, otb.ParameterType_OutputImage, otb.ParameterType_OutputVectorData)
-        outfile_params = [param for param in self.app.GetParametersKeys() if self.app.GetParameterType(param) in types]
-        return any(key in self.parameters for key in outfile_params)
-
-    @staticmethod
-    def __parse_args(args):
+    def __parse_args(self, args: list[str | OTBObject | dict | list]) -> dict[str, Any]:
         """Gather all input arguments in kwargs dict.
 
+        Args:
+            args: the list of arguments passed to set_parameters()
+
         Returns:
             a dictionary with the right keyword depending on the object
 
         """
         kwargs = {}
         for arg in args:
             if isinstance(arg, dict):
                 kwargs.update(arg)
-            elif isinstance(arg, (str, otbObject)):
-                kwargs.update({'in': arg})
-            elif isinstance(arg, list):
-                kwargs.update({'il': arg})
+            elif (
+                isinstance(arg, (str, OTBObject))
+                or isinstance(arg, list)
+                and self.is_key_list(self.input_key)
+            ):
+                kwargs.update({self.input_key: arg})
         return kwargs
 
-    def __set_param(self, param, obj):
+    def __set_param(
+        self, key: str, obj: list | tuple | OTBObject | otb.Application | list[Any]
+    ):
         """Set one parameter, decide which otb.Application method to use depending on target object."""
-        if obj is not None:
-            # Single-parameter cases
-            if isinstance(obj, otbObject):
-                self.app.ConnectImage(param, obj.app, obj.output_param)
-            elif isinstance(obj, otb.Application):  # this is for backward comp with plain OTB
-                outparamkey = [param for param in obj.GetParametersKeys()
-                               if obj.GetParameterType(param) == otb.ParameterType_OutputImage][0]
-                self.app.ConnectImage(param, obj, outparamkey)
-            elif param == 'ram':  # SetParameterValue in OTB<7.4 doesn't work for ram parameter cf gitlab OTB issue 2200
-                self.app.SetParameterInt('ram', int(obj))
-            elif not isinstance(obj, list):  # any other parameters (str, int...)
-                self.app.SetParameterValue(param, obj)
-            # Images list
-            elif self.__is_key_images_list(param):
-                # To enable possible in-memory connections, we go through the list and set the parameters one by one
-                for inp in obj:
-                    if isinstance(inp, otbObject):
-                        self.app.ConnectImage(param, inp.app, inp.output_param)
-                    elif isinstance(inp, otb.Application):  # this is for backward comp with plain OTB
-                        outparamkey = [param for param in inp.GetParametersKeys() if
-                                       inp.GetParameterType(param) == otb.ParameterType_OutputImage][0]
-                        self.app.ConnectImage(param, inp, outparamkey)
-                    else:  # here `input` should be an image filepath
-                        # Append `input` to the list, do not overwrite any previously set element of the image list
-                        self.app.AddParameterStringList(param, inp)
-            # List of any other types (str, int...)
-            else:
-                self.app.SetParameterValue(param, obj)
-
-    def __propagate_pixel_type(self):
-        """Propagate the pixel type from inputs to output.
-
-        For several inputs, or with an image list, the type of the first input is considered.
-        If several outputs, all outputs will have the same type.
-
-        """
-        pixel_type = None
-        for key, param in self.parameters.items():
-            if self.__is_key_input_image(key):
-                if not param:
-                    continue
-                if isinstance(param, list):
-                    param = param[0]  # first image in "il"
-                try:
-                    pixel_type = get_pixel_type(param)
-                    type_name = self.app.ConvertPixelTypeToNumpy(pixel_type)
-                    logger.debug('%s: output(s) will be written with type "%s"', self.name, type_name)
-                    for out_key in self.output_parameters_keys:
-                        self.app.SetParameterOutputImagePixelType(out_key, pixel_type)
-                    return
-                except TypeError:
-                    pass
-
-        logger.warning("%s: could not propagate pixel type from inputs to output, no valid input found", self.name)
-
-    def __save_objects(self):
-        """Saving app parameters and outputs as attributes, so that they can be accessed with `obj.key`.
+        if obj is None or (isinstance(obj, (list, tuple)) and not obj):
+            self.app.ClearValue(key)
+            return
+        # Single-parameter cases
+        if isinstance(obj, OTBObject):
+            self.app.ConnectImage(key, obj.app, obj.output_image_key)
+        elif isinstance(
+            obj, otb.Application
+        ):  # this is for backward comp with plain OTB
+            self.app.ConnectImage(key, obj, get_out_images_param_keys(obj)[0])
+        elif (
+            key == "ram"
+        ):  # SetParameterValue in OTB<7.4 doesn't work for ram parameter cf gitlab OTB issue 2200
+            self.app.SetParameterInt("ram", int(obj))
+        elif not isinstance(obj, list):  # any other parameters (str, int...)
+            self.app.SetParameterValue(key, obj)
+        # Images list
+        elif self.is_key_images_list(key):
+            # To enable possible in-memory connections, we go through the list and set the parameters one by one
+            for inp in obj:
+                if isinstance(inp, OTBObject):
+                    self.app.ConnectImage(key, inp.app, inp.output_image_key)
+                elif isinstance(
+                    inp, otb.Application
+                ):  # this is for backward comp with plain OTB
+                    self.app.ConnectImage(key, obj, get_out_images_param_keys(inp)[0])
+                else:  # here `input` should be an image filepath
+                    # Append `input` to the list, do not overwrite any previously set element of the image list
+                    self.app.AddParameterStringList(key, inp)
+        # List of any other types (str, int...)
+        else:
+            self.app.SetParameterValue(key, obj)
 
-        This is useful when the key contains reserved characters such as a point eg "io.out"
-        """
-        for key in self.app.GetParametersKeys():
-            if key == 'parameters':  # skip forbidden attribute since it is already used by the App class
+    def __sync_parameters(self):
+        """Save OTB parameters in _settings, data and outputs dict, for a list of keys or all parameters."""
+        for key in self.parameters_keys:
+            if not self.app.HasValue(key):
                 continue
-            value = None
-            if key in self.output_parameters_keys:  # raster outputs
-                value = Output(self, key)
-            elif key in self.parameters:  # user or default app parameters
-                value = self.parameters[key]
-            else:  # any other app attribute (e.g. ReadImageInfo results)
+            value = self.app.GetParameterValue(key)
+            # TODO: here we *should* use self.app.IsParameterEnabled, but it seems broken
+            if isinstance(value, otb.ApplicationProxy) and self.app.HasAutomaticValue(
+                key
+            ):
                 try:
-                    value = self.app.GetParameterValue(key)
+                    value = str(
+                        value
+                    )  # some default str values like "mode" or "interpolator"
+                    self._auto_parameters[key] = value
+                    continue
                 except RuntimeError:
-                    pass  # this is when there is no value for key
-            if value is not None:
-                setattr(self, key, value)
-
-    def __is_key_input_image(self, key):
-        """Check if a key of the App is an input parameter image list."""
-        return self.app.GetParameterType(key) in (otb.ParameterType_InputImage, otb.ParameterType_InputImageList)
-
-    def __is_key_list(self, key):
-        """Check if a key of the App is an input parameter list."""
-        return self.app.GetParameterType(key) in (otb.ParameterType_InputImageList, otb.ParameterType_StringList,
-                                                  otb.ParameterType_InputFilenameList, otb.ParameterType_ListView,
-                                                  otb.ParameterType_InputVectorDataList)
-
-    def __is_key_images_list(self, key):
-        """Check if a key of the App is an input parameter image list."""
-        return self.app.GetParameterType(key) in (otb.ParameterType_InputImageList, otb.ParameterType_InputFilenameList)
-
-    # Special methods
-    def __str__(self):
-        """Return a nice string representation with object id."""
-        return f'<pyotb.App {self.appname} object id {id(self)}>'
+                    continue  # grouped parameters
+            # Save static output data (ReadImageInfo, ComputeImageStatistics, etc.)
+            elif self.app.GetParameterRole(key) == 1 and bool(value) or value == 0:
+                if isinstance(value, str):
+                    try:
+                        value = literal_eval(value)
+                    except (ValueError, SyntaxError):
+                        pass
+                self.data[key] = value
+
+    # Special functions
+    def __getitem__(self, key: str) -> Any | list[int | float] | int | float | Slicer:
+        """This function is called when we use App()[...].
+
+        We allow to return attr if key is a parameter, or call OTBObject __getitem__ for pixel values or Slicer
+        """
+        if isinstance(key, tuple):
+            return super().__getitem__(key)  # to read pixel values, or slice
+        if isinstance(key, str):
+            if key in self.data:
+                return self.data[key]
+            if key in self.outputs:
+                return self.outputs[key]
+            if key in self.parameters:
+                return self.parameters[key]
+            raise KeyError(f"{self.name}: unknown or undefined parameter '{key}'")
+        raise TypeError(
+            f"{self.name}: cannot access object item or slice using {type(key)} object"
+        )
 
 
 class Slicer(App):
     """Slicer objects i.e. when we call something like raster[:, :, 2] from Python."""
 
-    def __init__(self, x, rows, cols, channels):
+    def __init__(
+        self,
+        obj: OTBObject,
+        rows: slice,
+        cols: slice,
+        channels: slice | list[int] | int,
+    ):
         """Create a slicer object, that can be used directly for writing or inside a BandMath.
 
         It contains :
         - an ExtractROI app that handles extracting bands and ROI and can be written to disk or used in pipelines
         - in case the user only wants to extract one band, an expression such as "im1b#"
 
         Args:
-            x: input
+            obj: input
             rows: slice along Y / Latitude axis
             cols: slice along X / Longitude axis
             channels: channels, can be slicing, list or int
 
         """
-        # Initialize the app that will be used for writing the slicer
-        self.name = 'Slicer'
+        super().__init__(
+            "ExtractROI",
+            obj,
+            mode="extent",
+            quiet=True,
+            frozen=True,
+            name=f"Slicer from {obj.name}",
+        )
+        self.rows, self.cols = rows, cols
+        parameters = {}
 
-        self.output_parameter_key = 'out'
-        parameters = {'in': x, 'mode': 'extent'}
-        super().__init__('ExtractROI', parameters, preserve_dtype=True, frozen=True)
         # Channel slicing
         if channels != slice(None, None, None):
             # Trigger source app execution if needed
-            nb_channels = get_nbchannels(x)
+            nb_channels = get_nbchannels(obj)
             self.app.Execute()  # this is needed by ExtractROI for setting the `cl` parameter
             # if needed, converting int to list
             if isinstance(channels, int):
                 channels = [channels]
             # if needed, converting slice to list
             elif isinstance(channels, slice):
-                channels_start = channels.start if channels.start is not None else 0
-                channels_start = channels_start if channels_start >= 0 else nb_channels + channels_start
-                channels_end = channels.stop if channels.stop is not None else nb_channels
-                channels_end = channels_end if channels_end >= 0 else nb_channels + channels_end
-                channels_step = channels.step if channels.step is not None else 1
-                channels = range(channels_start, channels_end, channels_step)
+                channels = self.channels_list_from_slice(channels)
             elif isinstance(channels, tuple):
                 channels = list(channels)
             elif not isinstance(channels, list):
-                raise ValueError(f'Invalid type for channels, should be int, slice or list of bands. : {channels}')
-
+                raise ValueError(
+                    f"Invalid type for channels, should be int, slice or list of bands. : {channels}"
+                )
             # Change the potential negative index values to reverse index
             channels = [c if c >= 0 else nb_channels + c for c in channels]
-            parameters.update({'cl': [f'Channel{i + 1}' for i in channels]})
+            parameters.update({"cl": [f"Channel{i + 1}" for i in channels]})
 
         # Spatial slicing
         spatial_slicing = False
-        # TODO: handle PixelValue app so that accessing value is possible, e.g. raster[120, 200, 0]
-        # TODO TBD: handle the step value in the slice so that NN undersampling is possible ? e.g. raster[::2, ::2]
+        # TODO: handle the step value in the slice so that NN undersampling is possible ? e.g. raster[::2, ::2]
         if rows.start is not None:
-            parameters.update({'mode.extent.uly': rows.start})
+            parameters.update({"mode.extent.uly": rows.start})
             spatial_slicing = True
         if rows.stop is not None and rows.stop != -1:
             parameters.update(
-                {'mode.extent.lry': rows.stop - 1})  # subtract 1 to be compliant with python convention
+                {"mode.extent.lry": rows.stop - 1}
+            )  # subtract 1 to respect python convention
             spatial_slicing = True
         if cols.start is not None:
-            parameters.update({'mode.extent.ulx': cols.start})
+            parameters.update({"mode.extent.ulx": cols.start})
             spatial_slicing = True
         if cols.stop is not None and cols.stop != -1:
             parameters.update(
-                {'mode.extent.lrx': cols.stop - 1})  # subtract 1 to be compliant with python convention
+                {"mode.extent.lrx": cols.stop - 1}
+            )  # subtract 1 to respect python convention
             spatial_slicing = True
-        # Execute app
-        self.set_parameters(**parameters)
-        self.execute()
-
         # These are some attributes when the user simply wants to extract *one* band to be used in an Operation
         if not spatial_slicing and isinstance(channels, list) and len(channels) == 1:
-            self.one_band_sliced = channels[0] + 1  # OTB convention: channels start at 1
-            self.input = x
-
-
-class Input(App):
-    """Class for transforming a filepath to pyOTB object."""
-
-    def __init__(self, filepath):
-        """Constructor for an Input object.
-
-        Args:
-            filepath: raster file path
-
-        """
-        self.filepath = filepath
-        super().__init__('ExtractROI', {'in': self.filepath}, preserve_dtype=True)
-
-    def __str__(self):
-        """Return a nice string representation with input file path."""
-        return f'<pyotb.Input object from {self.filepath}>'
-
-
-class Output(otbObject):
-    """Class for output of an app."""
-
-    def __init__(self, app, output_parameter_key):
-        """Constructor for an Output object.
-
-        Args:
-            app: The pyotb App
-            output_parameter_key: Output parameter key
-
-        """
-        # Keeping the OTB app and the pyotb app
-        self.pyotb_app, self.app = app, app.app
-        self.parameters = self.pyotb_app.parameters
-        self.output_param = output_parameter_key
-        self.name = f'Output {output_parameter_key} from {self.app.GetName()}'
-
-    def summarize(self):
-        """Return the summary of the pipeline that generates the Output object.
-
-        Returns:
-            Nested dictionary summarizing the pipeline that generates the Output object.
+            self.one_band_sliced = (
+                channels[0] + 1
+            )  # OTB convention: channels start at 1
+            self.input = obj
 
-        """
-        return self.pyotb_app.summarize()
-
-    def __str__(self):
-        """Return a nice string representation with object id."""
-        return f'<pyotb.Output {self.app.GetName()} object, id {id(self)}>'
+        # Execute app
+        self.set_parameters(parameters)
+        self.propagate_dtype()
+        self.execute()
 
 
 class Operation(App):
     """Class for arithmetic/math operations done in Python.
 
     Example:
         Consider the python expression (input1 + 2 * input2)  >  0.
@@ -953,128 +1047,140 @@
               Operation2, with expression im2 + 2 * im1
         |__________________________|
                             |
                       Operation3, with expression (im2 + 2 * im1) > 0 ? 1 : 0
 
     """
 
-    def __init__(self, operator, *inputs, nb_bands=None):
+    def __init__(self, operator: str, *inputs, nb_bands: int = None, name: str = None):
         """Given some inputs and an operator, this function enables to transform this into an OTB application.
 
         Operations generally involve 2 inputs (+, -...). It can have only 1 input for `abs` operator.
         It can have 3 inputs for the ternary operator `cond ? x : y`.
 
         Args:
             operator: (str) one of +, -, *, /, >, <, >=, <=, ==, !=, &, |, abs, ?
-            *inputs: inputs. Can be App, Output, Input, Operation, Slicer, filepath, int or float
+            *inputs: inputs. Can be OTBObject, filepath, int or float
             nb_bands: to specify the output nb of bands. Optional. Used only internally by pyotb.where
+            name: override the Operation name
 
         """
         self.operator = operator
         # We first create a 'fake' expression. E.g for the operation `input1 + input2` , we create a fake expression
         # that is like "str(input1) + str(input2)"
         self.inputs = []
         self.nb_channels = {}
         self.fake_exp_bands = []
-        self.logical_fake_exp_bands = []
-
-        self.create_fake_exp(operator, inputs, nb_bands=nb_bands)
-
+        self.build_fake_expressions(operator, inputs, nb_bands=nb_bands)
         # Transforming images to the adequate im#, e.g. `input1` to "im1"
         # creating a dictionary that is like {str(input1): 'im1', 'image2.tif': 'im2', ...}.
         # NB: the keys of the dictionary are strings-only, instead of 'complex' objects, to enable easy serialization
         self.im_dic = {}
         self.im_count = 1
-        mapping_str_to_input = {}  # to be able to retrieve the real python object from its string representation
+        map_repr_to_input = (
+            {}
+        )  # to be able to retrieve the real python object from its string representation
         for inp in self.inputs:
             if not isinstance(inp, (int, float)):
                 if str(inp) not in self.im_dic:
-                    self.im_dic[str(inp)] = f'im{self.im_count}'
-                    mapping_str_to_input[str(inp)] = inp
+                    self.im_dic[repr(inp)] = f"im{self.im_count}"
+                    map_repr_to_input[repr(inp)] = inp
                     self.im_count += 1
-
-        # getting unique image inputs, in the order im1, im2, im3 ...
-        self.unique_inputs = [mapping_str_to_input[str_input] for str_input in sorted(self.im_dic, key=self.im_dic.get)]
-        self.output_param = 'out'
-
-        # Computing the BandMath or BandMathX app
+        # Getting unique image inputs, in the order im1, im2, im3 ...
+        self.unique_inputs = [
+            map_repr_to_input[id_str]
+            for id_str in sorted(self.im_dic, key=self.im_dic.get)
+        ]
         self.exp_bands, self.exp = self.get_real_exp(self.fake_exp_bands)
-        self.name = f'Operation exp="{self.exp}"'
-
-        appname = 'BandMath' if len(self.exp_bands) == 1 else 'BandMathX'
-        super().__init__(appname, il=self.unique_inputs, exp=self.exp)
-
-    def create_fake_exp(self, operator, inputs, nb_bands=None):
-        """Create a 'fake' expression.
+        appname = "BandMath" if len(self.exp_bands) == 1 else "BandMathX"
+        name = f'Operation exp="{self.exp}"'
+        super().__init__(
+            appname, il=self.unique_inputs, exp=self.exp, quiet=True, name=name
+        )
+
+    def build_fake_expressions(
+        self,
+        operator: str,
+        inputs: list[OTBObject | str | int | float],
+        nb_bands: int = None,
+    ):
+        """Create a list of 'fake' expressions, one for each band.
 
         E.g for the operation input1 + input2, we create a fake expression that is like "str(input1) + str(input2)"
 
         Args:
             operator: (str) one of +, -, *, /, >, <, >=, <=, ==, !=, &, |, abs, ?
-            inputs: inputs. Can be App, Output, Input, Operation, Slicer, filepath, int or float
+            inputs: inputs. Can be OTBObject, filepath, int or float
             nb_bands: to specify the output nb of bands. Optional. Used only internally by pyotb.where
 
         """
         self.inputs.clear()
         self.nb_channels.clear()
-
         logger.debug("%s, %s", operator, inputs)
-        # this is when we use the ternary operator with `pyotb.where` function. The output nb of bands is already known
-        if operator == '?' and nb_bands:
+        # This is when we use the ternary operator with `pyotb.where` function. The output nb of bands is already known
+        if operator == "?" and nb_bands:
             pass
         # For any other operations, the output number of bands is the same as inputs
         else:
-            if any(isinstance(inp, Slicer) and hasattr(inp, 'one_band_sliced') for inp in inputs):
+            if any(
+                isinstance(inp, Slicer) and hasattr(inp, "one_band_sliced")
+                for inp in inputs
+            ):
                 nb_bands = 1
             else:
-                nb_bands_list = [get_nbchannels(inp) for inp in inputs if not isinstance(inp, (float, int))]
+                nb_bands_list = [
+                    get_nbchannels(inp)
+                    for inp in inputs
+                    if not isinstance(inp, (float, int))
+                ]
                 # check that all inputs have the same nb of bands
-                if len(nb_bands_list) > 1:
-                    if not all(x == nb_bands_list[0] for x in nb_bands_list):
-                        raise Exception('All images do not have the same number of bands')
+                if len(nb_bands_list) > 1 and not all(
+                    x == nb_bands_list[0] for x in nb_bands_list
+                ):
+                    raise ValueError("All images do not have the same number of bands")
                 nb_bands = nb_bands_list[0]
 
         # Create a list of fake expressions, each item of the list corresponding to one band
         self.fake_exp_bands.clear()
         for i, band in enumerate(range(1, nb_bands + 1)):
-            fake_exps = []
+            expressions = []
             for k, inp in enumerate(inputs):
-                # Generating the fake expression of the current input
+                # Generating the fake expression of the current input,
                 # this is a special case for the condition of the ternary operator `cond ? x : y`
                 if len(inputs) == 3 and k == 0:
-                    # when cond is monoband whereas the result is multiband, we expand the cond to multiband
-                    if nb_bands != inp.shape[2]:
-                        cond_band = 1
-                    else:
-                        cond_band = band
-                    fake_exp, corresponding_inputs, nb_channels = self.create_one_input_fake_exp(inp, cond_band,
-                                                                                                 keep_logical=True)
-                # any other input
+                    # When cond is monoband whereas the result is multiband, we expand the cond to multiband
+                    cond_band = 1 if nb_bands != inp.shape[2] else band
+                    fake_exp, corresponding_inputs, nb_channels = self.make_fake_exp(
+                        inp, cond_band, keep_logical=True
+                    )
                 else:
-                    fake_exp, corresponding_inputs, nb_channels = self.create_one_input_fake_exp(inp, band,
-                                                                                                 keep_logical=False)
-                fake_exps.append(fake_exp)
+                    # Any other input
+                    fake_exp, corresponding_inputs, nb_channels = self.make_fake_exp(
+                        inp, band, keep_logical=False
+                    )
+                expressions.append(fake_exp)
                 # Reference the inputs and nb of channels (only on first pass in the loop to avoid duplicates)
                 if i == 0 and corresponding_inputs and nb_channels:
                     self.inputs.extend(corresponding_inputs)
                     self.nb_channels.update(nb_channels)
 
             # Generating the fake expression of the whole operation
             if len(inputs) == 1:  # this is only for 'abs'
-                fake_exp = f'({operator}({fake_exps[0]}))'
+                fake_exp = f"({operator}({expressions[0]}))"
             elif len(inputs) == 2:
                 # We create here the "fake" expression. For example, for a BandMathX expression such as '2 * im1 + im2',
                 # the false expression stores the expression 2 * str(input1) + str(input2)
-                fake_exp = f'({fake_exps[0]} {operator} {fake_exps[1]})'
-            elif len(inputs) == 3 and operator == '?':  # this is only for ternary expression
-                fake_exp = f'({fake_exps[0]} ? {fake_exps[1]} : {fake_exps[2]})'
-
+                fake_exp = f"({expressions[0]} {operator} {expressions[1]})"
+            elif (
+                len(inputs) == 3 and operator == "?"
+            ):  # this is only for ternary expression
+                fake_exp = f"({expressions[0]} ? {expressions[1]} : {expressions[2]})"
             self.fake_exp_bands.append(fake_exp)
 
-    def get_real_exp(self, fake_exp_bands):
+    def get_real_exp(self, fake_exp_bands: str) -> tuple[list[str], str]:
         """Generates the BandMathX expression.
 
         Args:
             fake_exp_bands: list of fake expressions, each item corresponding to one band
 
         Returns:
             exp_bands: BandMath expression, split in a list, each item corresponding to one band
@@ -1082,216 +1188,442 @@
 
         """
         # Create a list of expression, each item corresponding to one band (e.g. ['im1b1 + 1', 'im1b2 + 1'])
         exp_bands = []
         for one_band_fake_exp in fake_exp_bands:
             one_band_exp = one_band_fake_exp
             for inp in self.inputs:
-                # replace the name of in-memory object (e.g. '<pyotb.App object>b1' by 'im1b1')
-                one_band_exp = one_band_exp.replace(str(inp), self.im_dic[str(inp)])
+                # Replace the name of in-memory object (e.g. '<pyotb.App object>b1' by 'im1b1')
+                one_band_exp = one_band_exp.replace(repr(inp), self.im_dic[repr(inp)])
             exp_bands.append(one_band_exp)
-
         # Form the final expression (e.g. 'im1b1 + 1; im1b2 + 1')
-        exp = ';'.join(exp_bands)
-
-        return exp_bands, exp
+        return exp_bands, ";".join(exp_bands)
 
     @staticmethod
-    def create_one_input_fake_exp(x, band, keep_logical=False):
-        """This an internal function, only to be used by `create_fake_exp`.
+    def make_fake_exp(
+        x: OTBObject | str, band: int, keep_logical: bool = False
+    ) -> tuple[str, list[OTBObject], int]:
+        """This an internal function, only to be used by `build_fake_expressions`.
 
         Enable to create a fake expression just for one input and one band.
 
         Args:
             x: input
             band: which band to consider (bands start at 1)
             keep_logical: whether to keep the logical expressions "as is" in case the input is a logical operation.
                           ex: if True, for `input1 > input2`, returned fake expression is "str(input1) > str(input2)"
-                          if False, for `input1 > input2`, returned fake exp is "str(input1) > str(input2) ? 1 : 0".
+                          if False, for `input1 > input2`, returned fake exp is "str(input1) > str(input2) ? 1 : 0"]
                           Default False
 
         Returns:
             fake_exp: the fake expression for this band and input
             inputs: if the input is an Operation, we returns its own inputs
             nb_channels: if the input is an Operation, we returns its own nb_channels
 
         """
         # Special case for one-band slicer
-        if isinstance(x, Slicer) and hasattr(x, 'one_band_sliced'):
-            if keep_logical and isinstance(x.input, logicalOperation):
+        if isinstance(x, Slicer) and hasattr(x, "one_band_sliced"):
+            if keep_logical and isinstance(x.input, LogicalOperation):
                 fake_exp = x.input.logical_fake_exp_bands[x.one_band_sliced - 1]
-                inputs = x.input.inputs
-                nb_channels = x.input.nb_channels
+                inputs, nb_channels = x.input.inputs, x.input.nb_channels
             elif isinstance(x.input, Operation):
-                # keep only one band of the expression
+                # Keep only one band of the expression
                 fake_exp = x.input.fake_exp_bands[x.one_band_sliced - 1]
-                inputs = x.input.inputs
-                nb_channels = x.input.nb_channels
+                inputs, nb_channels = x.input.inputs, x.input.nb_channels
             else:
                 # Add the band number (e.g. replace '<pyotb.App object>' by '<pyotb.App object>b1')
-                fake_exp = str(x.input) + f'b{x.one_band_sliced}'
-                inputs = [x.input]
-                nb_channels = {x.input: 1}
-        # For logicalOperation, we save almost the same attributes as an Operation
-        elif keep_logical and isinstance(x, logicalOperation):
+                fake_exp = f"{repr(x.input)}b{x.one_band_sliced}"
+                inputs, nb_channels = [x.input], {repr(x.input): 1}
+        # For LogicalOperation, we save almost the same attributes as an Operation
+        elif keep_logical and isinstance(x, LogicalOperation):
             fake_exp = x.logical_fake_exp_bands[band - 1]
-            inputs = x.inputs
-            nb_channels = x.nb_channels
+            inputs, nb_channels = x.inputs, x.nb_channels
         elif isinstance(x, Operation):
             fake_exp = x.fake_exp_bands[band - 1]
-            inputs = x.inputs
-            nb_channels = x.nb_channels
+            inputs, nb_channels = x.inputs, x.nb_channels
         # For int or float input, we just need to save their value
         elif isinstance(x, (int, float)):
             fake_exp = str(x)
-            inputs = None
-            nb_channels = None
+            inputs, nb_channels = None, None
         # We go on with other inputs, i.e. pyotb objects, filepaths...
         else:
-            nb_channels = {x: get_nbchannels(x)}
-            inputs = [x]
             # Add the band number (e.g. replace '<pyotb.App object>' by '<pyotb.App object>b1')
-            fake_exp = str(x) + f'b{band}'
+            fake_exp = f"{repr(x)}b{band}"
+            inputs, nb_channels = [x], {repr(x): get_nbchannels(x)}
 
         return fake_exp, inputs, nb_channels
 
-    def __str__(self):
-        """Return a nice string representation with object id."""
-        return f'<pyotb.Operation `{self.operator}` object, id {id(self)}>'
+    def __repr__(self) -> str:
+        """Return a nice string representation with operator and object id."""
+        return f"<pyotb.Operation `{self.operator}` object, id {id(self)}>"
 
 
-class logicalOperation(Operation):
+class LogicalOperation(Operation):
     """A specialization of Operation class for boolean logical operations i.e. >, <, >=, <=, ==, !=, `&` and `|`.
 
     The only difference is that not only the BandMath expression is saved (e.g. "im1b1 > 0 ? 1 : 0"), but also the
     logical expression (e.g. "im1b1 > 0")
 
     """
 
-    def __init__(self, operator, *inputs, nb_bands=None):
-        """Constructor for a logicalOperation object.
+    def __init__(self, operator: str, *inputs, nb_bands: int = None):
+        """Constructor for a LogicalOperation object.
 
         Args:
             operator: string operator (one of >, <, >=, <=, ==, !=, &, |)
             *inputs: inputs
             nb_bands: to specify the output nb of bands. Optional. Used only internally by pyotb.where
 
         """
-        super().__init__(operator, *inputs, nb_bands=nb_bands)
-        self.logical_exp_bands, self.logical_exp = self.get_real_exp(self.logical_fake_exp_bands)
-
-    def create_fake_exp(self, operator, inputs, nb_bands=None):
-        """Create a 'fake' expression.
+        self.logical_fake_exp_bands = []
+        super().__init__(operator, *inputs, nb_bands=nb_bands, name="LogicalOperation")
+        self.logical_exp_bands, self.logical_exp = self.get_real_exp(
+            self.logical_fake_exp_bands
+        )
+
+    def build_fake_expressions(
+        self,
+        operator: str,
+        inputs: list[OTBObject | str | int | float],
+        nb_bands: int = None,
+    ):
+        """Create a list of 'fake' expressions, one for each band.
 
-        E.g for the operation input1 > input2, we create a fake expression that is like
+        e.g for the operation input1 > input2, we create a fake expression that is like
         "str(input1) > str(input2) ? 1 : 0" and a logical fake expression that is like "str(input1) > str(input2)"
 
         Args:
             operator: str (one of >, <, >=, <=, ==, !=, &, |)
-            inputs: Can be App, Output, Input, Operation, Slicer, filepath, int or float
+            inputs: Can be OTBObject, filepath, int or float
             nb_bands: to specify the output nb of bands. Optional. Used only internally by pyotb.where
 
         """
         # For any other operations, the output number of bands is the same as inputs
-        if any(isinstance(inp, Slicer) and hasattr(inp, 'one_band_sliced') for inp in inputs):
+        if any(
+            isinstance(inp, Slicer) and hasattr(inp, "one_band_sliced")
+            for inp in inputs
+        ):
             nb_bands = 1
         else:
-            nb_bands_list = [get_nbchannels(inp) for inp in inputs if not isinstance(inp, (float, int))]
+            nb_bands_list = [
+                get_nbchannels(inp)
+                for inp in inputs
+                if not isinstance(inp, (float, int))
+            ]
             # check that all inputs have the same nb of bands
-            if len(nb_bands_list) > 1:
-                if not all(x == nb_bands_list[0] for x in nb_bands_list):
-                    raise Exception('All images do not have the same number of bands')
+            if len(nb_bands_list) > 1 and not all(
+                x == nb_bands_list[0] for x in nb_bands_list
+            ):
+                raise ValueError("All images do not have the same number of bands")
             nb_bands = nb_bands_list[0]
-
         # Create a list of fake exp, each item of the list corresponding to one band
         for i, band in enumerate(range(1, nb_bands + 1)):
-            fake_exps = []
+            expressions = []
             for inp in inputs:
-                fake_exp, corresponding_inputs, nb_channels = super().create_one_input_fake_exp(inp, band,
-                                                                                                keep_logical=True)
-                fake_exps.append(fake_exp)
+                fake_exp, corresp_inputs, nb_channels = super().make_fake_exp(
+                    inp, band, keep_logical=True
+                )
+                expressions.append(fake_exp)
                 # Reference the inputs and nb of channels (only on first pass in the loop to avoid duplicates)
-                if i == 0 and corresponding_inputs and nb_channels:
-                    self.inputs.extend(corresponding_inputs)
+                if i == 0 and corresp_inputs and nb_channels:
+                    self.inputs.extend(corresp_inputs)
                     self.nb_channels.update(nb_channels)
-
             # We create here the "fake" expression. For example, for a BandMathX expression such as 'im1 > im2',
             # the logical fake expression stores the expression "str(input1) > str(input2)"
-            logical_fake_exp = f'({fake_exps[0]} {operator} {fake_exps[1]})'
-
+            logical_fake_exp = f"({expressions[0]} {operator} {expressions[1]})"
             # We keep the logical expression, useful if later combined with other logical operations
             self.logical_fake_exp_bands.append(logical_fake_exp)
             # We create a valid BandMath expression, e.g. "str(input1) > str(input2) ? 1 : 0"
-            fake_exp = f'({logical_fake_exp} ? 1 : 0)'
+            fake_exp = f"({logical_fake_exp} ? 1 : 0)"
             self.fake_exp_bands.append(fake_exp)
 
 
-def get_nbchannels(inp):
+class Input(App):
+    """Class for transforming a filepath to pyOTB object."""
+
+    def __init__(self, filepath: str):
+        """Default constructor.
+
+        Args:
+            filepath: Anything supported by GDAL (local file on the filesystem, remote resource e.g. /vsicurl/.., etc.)
+
+        """
+        super().__init__("ExtractROI", {"in": filepath}, frozen=True)
+        self._name = f"Input from {filepath}"
+        if not filepath.startswith(("/vsi", "http://", "https://", "ftp://")):
+            filepath = Path(filepath)
+        self.filepath = filepath
+        self.propagate_dtype()
+        self.execute()
+
+    def __repr__(self) -> str:
+        """Return a string representation with file path, used in Operation to store file ref."""
+        return f"<pyotb.Input object, from {self.filepath}>"
+
+
+class Output(OTBObject):
+    """Object that behave like a pointer to a specific application output file."""
+
+    _filepath: str | Path = None
+
+    def __init__(
+        self,
+        pyotb_app: App,
+        param_key: str = None,
+        filepath: str = None,
+        mkdir: bool = True,
+    ):
+        """Constructor for an Output object.
+
+        Args:
+            pyotb_app: The pyotb App to store reference from
+            param_key: Output parameter key of the target app
+            filepath: path of the output file (if not in memory)
+            mkdir: create missing parent directories
+
+        """
+        self.parent_pyotb_app = pyotb_app  # keep trace of parent app
+        self.param_key = param_key
+        self.filepath = filepath
+        if mkdir and filepath is not None:
+            self.make_parent_dirs()
+
+    @property
+    def name(self) -> str:
+        """Return Output name containing filepath."""
+        return f"Output {self.param_key} from {self.parent_pyotb_app.name}"
+
+    @property
+    def app(self) -> otb.Application:
+        """Reference to the parent pyotb otb.Application instance."""
+        return self.parent_pyotb_app.app
+
+    @property
+    def exports_dic(self) -> dict[str, dict]:
+        """Returns internal _exports_dic object that contains numpy array exports."""
+        return self.parent_pyotb_app.exports_dic
+
+    @property
+    def output_image_key(self) -> str:
+        """Force the right key to be used when accessing the OTBObject."""
+        return self.param_key
+
+    @property
+    def filepath(self) -> str | Path:
+        """Property to manage output URL."""
+        if self._filepath is None:
+            raise ValueError("Filepath is not set")
+        return self._filepath
+
+    @filepath.setter
+    def filepath(self, path: str):
+        if isinstance(path, str):
+            if path and not path.startswith(("/vsi", "http://", "https://", "ftp://")):
+                path = Path(path.split("?")[0])
+            self._filepath = path
+
+    def exists(self) -> bool:
+        """Check file exist."""
+        if not isinstance(self.filepath, Path):
+            raise ValueError("Filepath is not set or points to a remote URL")
+        return self.filepath.exists()
+
+    def make_parent_dirs(self):
+        """Create missing parent directories."""
+        if not isinstance(self.filepath, Path):
+            raise ValueError("Filepath is not set or points to a remote URL")
+        self.filepath.parent.mkdir(parents=True, exist_ok=True)
+
+    def write(self, filepath: None | str | Path = None, **kwargs) -> bool:
+        """Write output to disk, filepath is not required if it was provided to parent App during init."""
+        if filepath is None:
+            return self.parent_pyotb_app.write(
+                {self.output_image_key: self.filepath}, **kwargs
+            )
+        return self.parent_pyotb_app.write({self.output_image_key: filepath}, **kwargs)
+
+    def __str__(self) -> str:
+        """Return string representation of Output filepath."""
+        return str(self.filepath)
+
+
+def add_vsi_prefix(filepath: str | Path) -> str:
+    """Append vsi prefixes to file URL or path if needed.
+
+    Args:
+        filepath: file path or URL
+
+    Returns:
+        string with new /vsi prefix(es)
+
+    """
+    if isinstance(filepath, Path):
+        filepath = str(filepath)
+    if isinstance(filepath, str) and not filepath.startswith("/vsi"):
+        # Remote file. TODO: add support for S3 / GS / AZ
+        if filepath.startswith(("https://", "http://", "ftp://")):
+            filepath = "/vsicurl/" + filepath
+        # Compressed file
+        prefixes = {
+            ".tar": "vsitar",
+            ".tgz": "vsitar",
+            ".gz": "vsigzip",
+            ".7z": "vsi7z",
+            ".zip": "vsizip",
+            ".rar": "vsirar",
+        }
+        basename = filepath.split("?")[0]
+        ext = Path(basename).suffix
+        if ext in prefixes:
+            filepath = f"/{prefixes[ext]}/{filepath}"
+    return filepath
+
+
+def get_nbchannels(inp: str | Path | OTBObject) -> int:
     """Get the nb of bands of input image.
 
     Args:
-        inp: can be filepath or pyotb object
+        inp: can be filepath or OTBObject object
 
     Returns:
         number of bands in image
 
     """
-    if isinstance(inp, otbObject):
-        nb_channels = inp.shape[-1]
-    else:
+    if isinstance(inp, OTBObject):
+        return inp.shape[-1]
+    if isinstance(inp, (str, Path)):
         # Executing the app, without printing its log
         try:
             info = App("ReadImageInfo", inp, quiet=True)
-            nb_channels = info.GetParameterInt("numberbands")
-        except Exception as e:  # this happens when we pass a str that is not a filepath
-            raise TypeError(f'Could not get the number of channels of `{inp}`. Not a filepath or wrong filepath') from e
-    return nb_channels
+            return info["numberbands"]
+        except (
+            RuntimeError
+        ) as info_err:  # this happens when we pass a str that is not a filepath
+            raise TypeError(
+                f"Could not get the number of channels file '{inp}' ({info_err})"
+            ) from info_err
+    raise TypeError(f"Can't read number of channels of type '{type(inp)}' object {inp}")
 
 
-def get_pixel_type(inp):
+def get_pixel_type(inp: str | Path | OTBObject) -> str:
     """Get the encoding of input image pixels.
 
     Args:
         inp: can be filepath or pyotb object
 
     Returns:
         pixel_type: OTB enum e.g. `otbApplication.ImagePixelType_uint8', which actually is an int.
-                    For an App with several outputs, only the pixel type of the first output is returned
+                    For an OTBObject with several outputs, only the pixel type of the first output is returned
 
     """
-    if isinstance(inp, str):
-        # Executing the app, without printing its log
+    if isinstance(inp, OTBObject):
+        return inp.app.GetParameterOutputImagePixelType(inp.output_image_key)
+    if isinstance(inp, (str, Path)):
         try:
             info = App("ReadImageInfo", inp, quiet=True)
-        except Exception as info_err:  # this happens when we pass a str that is not a filepath
-            raise TypeError(f'Could not get the pixel type of `{inp}`. Not a filepath or wrong filepath') from info_err
-        datatype = info.GetParameterString("datatype")  # which is such as short, float...
-        if not datatype:
-            raise Exception(f'Unable to read pixel type of image {inp}')
-        datatype_to_pixeltype = {'unsigned_char': 'uint8', 'short': 'int16', 'unsigned_short': 'uint16',
-                                 'int': 'int32', 'unsigned_int': 'uint32', 'long': 'int32', 'ulong': 'uint32',
-                                 'float': 'float', 'double': 'double'}
-        pixel_type = datatype_to_pixeltype[datatype]
-        pixel_type = getattr(otb, f'ImagePixelType_{pixel_type}')
-    elif isinstance(inp, (otbObject)):
-        pixel_type = inp.GetParameterOutputImagePixelType(inp.output_param)
-    else:
-        raise TypeError(f'Could not get the pixel type. Not supported type: {inp}')
-
-    return pixel_type
+            datatype = info["datatype"]  # which is such as short, float...
+        except (
+            RuntimeError
+        ) as info_err:  # this happens when we pass a str that is not a filepath
+            raise TypeError(
+                f"Could not get the pixel type of `{inp}` ({info_err})"
+            ) from info_err
+        if datatype:
+            return parse_pixel_type(datatype)
+    raise TypeError(f"Could not get the pixel type of {type(inp)} object {inp}")
 
 
-def parse_pixel_type(pixel_type):
+def parse_pixel_type(pixel_type: str | int) -> int:
     """Convert one str pixel type to OTB integer enum if necessary.
 
     Args:
         pixel_type: pixel type. can be str, int or dict
 
     Returns:
         pixel_type integer value
 
     """
-    if isinstance(pixel_type, str):  # this correspond to 'uint8' etc...
-        return getattr(otb, f'ImagePixelType_{pixel_type}')
-    if isinstance(pixel_type, int):
+    if isinstance(pixel_type, int):  # normal OTB int enum
         return pixel_type
-    raise ValueError(f'Bad pixel type specification ({pixel_type})')
+    if isinstance(pixel_type, str):  # correspond to 'uint8' etc...
+        datatype_to_pixeltype = {
+            "unsigned_char": "uint8",
+            "short": "int16",
+            "unsigned_short": "uint16",
+            "int": "int32",
+            "unsigned_int": "uint32",
+            "long": "int32",
+            "ulong": "uint32",
+            "float": "float",
+            "double": "double",
+        }
+        if pixel_type in datatype_to_pixeltype.values():
+            return getattr(otb, f"ImagePixelType_{pixel_type}")
+        if pixel_type in datatype_to_pixeltype:
+            return getattr(otb, f"ImagePixelType_{datatype_to_pixeltype[pixel_type]}")
+        raise KeyError(
+            f"Unknown data type `{pixel_type}`. Available ones: {datatype_to_pixeltype}"
+        )
+    raise TypeError(
+        f"Bad pixel type specification ({pixel_type} of type {type(pixel_type)})"
+    )
+
+
+def get_out_images_param_keys(app: OTBObject) -> list[str]:
+    """Return every output parameter keys of an OTB app."""
+    return [
+        key
+        for key in app.GetParametersKeys()
+        if app.GetParameterType(key) == otb.ParameterType_OutputImage
+    ]
+
+
+def summarize(
+    obj: App | Output | Any,
+    strip_input_paths: bool = False,
+    strip_output_paths: bool = False,
+) -> dict[str, str | dict[str, Any]]:
+    """Recursively summarize parameters of an App or Output object and its parents.
+
+    Args:
+        obj: input object to summarize
+        strip_input_paths: strip all input paths: If enabled, paths related to
+            inputs are truncated after the first "?" character. Can be useful
+            to remove URLs tokens (e.g. SAS or S3 credentials).
+        strip_output_paths: strip all output paths: If enabled, paths related
+            to outputs are truncated after the first "?" character. Can be
+            useful to remove extended filenames.
+
+    Returns:
+        nested dictionary with serialized App(s) containing name and
+        parameters of an app and its parents
+
+    """
+
+    def strip_path(param: str | Any):
+        if not isinstance(param, str):
+            return summarize(param)
+        return param.split("?")[0]
+
+    if isinstance(obj, list):
+        return [summarize(o) for o in obj]
+    if isinstance(obj, Output):
+        return summarize(obj.parent_pyotb_app)
+    if not isinstance(obj, App):
+        return obj
+
+    parameters = {}
+    for key, param in obj.parameters.items():
+        if (
+            strip_input_paths
+            and obj.is_input(key)
+            or strip_output_paths
+            and obj.is_output(key)
+        ):
+            parameters[key] = (
+                [strip_path(p) for p in param]
+                if isinstance(param, list)
+                else strip_path(param)
+            )
+        else:
+            parameters[key] = summarize(param)
+    return {"name": obj.app.GetName(), "parameters": parameters}
```

### Comparing `pyotb-1.5.4/pyotb/functions.py` & `pyotb-2.0.0.dev1/pyotb/functions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,98 @@
 # -*- coding: utf-8 -*-
 """This module provides a set of functions for pyotb."""
+from __future__ import annotations
+
 import inspect
 import os
+import subprocess
 import sys
 import textwrap
 import uuid
 from collections import Counter
 
-from .core import (otbObject, App, Input, Operation, logicalOperation, get_nbchannels)
+from .core import App, Input, LogicalOperation, Operation, get_nbchannels
 from .helpers import logger
 
 
-def where(cond, x, y):
+def where(
+    cond: App | str, x: App | str | int | float, y: App | str | int | float
+) -> Operation:
     """Functionally similar to numpy.where. Where cond is True (!=0), returns x. Else returns y.
 
     Args:
         cond: condition, must be a raster (filepath, App, Operation...). If cond is monoband whereas x or y are
               multiband, cond channels are expanded to match x & y ones.
-        x: value if cond is True. Can be float, int, App, filepath, Operation...
-        y: value if cond is False. Can be float, int, App, filepath, Operation...
+        x: value if cond is True. Can be: float, int, App, filepath, Operation...
+        y: value if cond is False. Can be: float, int, App, filepath, Operation...
 
     Returns:
         an output where pixels are x if cond is True, else y
 
     """
     # Checking the number of bands of rasters. Several cases :
     # - if cond is monoband, x and y can be multibands. Then cond will adapt to match x and y nb of bands
     # - if cond is multiband, x and y must have the same nb of bands if they are rasters.
     x_nb_channels, y_nb_channels = None, None
     if not isinstance(x, (int, float)):
         x_nb_channels = get_nbchannels(x)
     if not isinstance(y, (int, float)):
         y_nb_channels = get_nbchannels(y)
-
     if x_nb_channels and y_nb_channels:
         if x_nb_channels != y_nb_channels:
-            raise ValueError('X and Y images do not have the same number of bands. '
-                             f'X has {x_nb_channels} bands whereas Y has {y_nb_channels} bands')
+            raise ValueError(
+                "X and Y images do not have the same number of bands. "
+                f"X has {x_nb_channels} bands whereas Y has {y_nb_channels} bands"
+            )
 
     x_or_y_nb_channels = x_nb_channels if x_nb_channels else y_nb_channels
     cond_nb_channels = get_nbchannels(cond)
+    if (
+        cond_nb_channels != 1
+        and x_or_y_nb_channels
+        and cond_nb_channels != x_or_y_nb_channels
+    ):
+        raise ValueError(
+            "Condition and X&Y do not have the same number of bands. Condition has "
+            f"{cond_nb_channels} bands whereas X&Y have {x_or_y_nb_channels} bands"
+        )
+    # If needed, duplicate the single band binary mask to multiband to match the dimensions of x & y
+    if cond_nb_channels == 1 and x_or_y_nb_channels and x_or_y_nb_channels != 1:
+        logger.info(
+            "The condition has one channel whereas X/Y has/have %s channels. Expanding number"
+            " of channels of condition to match the number of channels of X/Y",
+            x_or_y_nb_channels,
+        )
 
     # Get the number of bands of the result
     if x_or_y_nb_channels:  # if X or Y is a raster
         out_nb_channels = x_or_y_nb_channels
     else:  # if only cond is a raster
         out_nb_channels = cond_nb_channels
 
-    if cond_nb_channels != 1 and x_or_y_nb_channels and cond_nb_channels != x_or_y_nb_channels:
-        raise ValueError('Condition and X&Y do not have the same number of bands. Condition has '
-                         f'{cond_nb_channels} bands whereas X&Y have {x_or_y_nb_channels} bands')
-
-    # If needed, duplicate the single band binary mask to multiband to match the dimensions of x & y
-    if cond_nb_channels == 1 and x_or_y_nb_channels and x_or_y_nb_channels != 1:
-        logger.info('The condition has one channel whereas X/Y has/have %s channels. Expanding number'
-                    ' of channels of condition to match the number of channels of X/Y', x_or_y_nb_channels)
+    return Operation("?", cond, x, y, nb_bands=out_nb_channels)
 
-    operation = Operation('?', cond, x, y, nb_bands=out_nb_channels)
 
-    return operation
-
-
-def clip(a, a_min, a_max):
+def clip(
+    image: App | str, v_min: App | str | int | float, v_max: App | str | int | float
+):
     """Clip values of image in a range of values.
 
     Args:
-        a: input raster, can be filepath or any pyotb object
-        a_min: minimum value of the range
-        a_max: maximum value of the range
+        image: input raster, can be filepath or any pyotb object
+        v_min: minimum value of the range
+        v_max: maximum value of the range
 
     Returns:
         raster whose values are clipped in the range
 
     """
-    if isinstance(a, str):
-        a = Input(a)
-
-    res = where(a <= a_min, a_min,
-                where(a >= a_max, a_max, a))
+    if isinstance(image, str):
+        image = Input(image)
+    res = where(image <= v_min, v_min, where(image >= v_max, v_max, image))
     return res
 
 
 def all(*inputs):  # pylint: disable=redefined-builtin
     """Check if value is different than 0 everywhere along the band axis.
 
     For only one image, this function checks that all bands of the image are True (i.e. !=0) and outputs
@@ -96,44 +107,44 @@
     Returns:
         AND intersection
 
     """
     # If necessary, flatten inputs
     if len(inputs) == 1 and isinstance(inputs[0], (list, tuple)):
         inputs = inputs[0]
-
     # Add support for generator inputs (to have the same behavior as built-in `all` function)
-    if isinstance(inputs, tuple) and len(inputs) == 1 and inspect.isgenerator(inputs[0]):
+    if (
+        isinstance(inputs, tuple)
+        and len(inputs) == 1
+        and inspect.isgenerator(inputs[0])
+    ):
         inputs = list(inputs[0])
-
     # Transforming potential filepaths to pyotb objects
     inputs = [Input(inp) if isinstance(inp, str) else inp for inp in inputs]
 
     # Checking that all bands of the single image are True
     if len(inputs) == 1:
         inp = inputs[0]
-        if isinstance(inp, logicalOperation):
+        if isinstance(inp, LogicalOperation):
             res = inp[:, :, 0]
         else:
-            res = (inp[:, :, 0] != 0)
-
+            res = inp[:, :, 0] != 0
         for band in range(1, inp.shape[-1]):
-            if isinstance(inp, logicalOperation):
+            if isinstance(inp, LogicalOperation):
                 res = res & inp[:, :, band]
             else:
                 res = res & (inp[:, :, band] != 0)
-
     # Checking that all images are True
     else:
-        if isinstance(inputs[0], logicalOperation):
+        if isinstance(inputs[0], LogicalOperation):
             res = inputs[0]
         else:
-            res = (inputs[0] != 0)
+            res = inputs[0] != 0
         for inp in inputs[1:]:
-            if isinstance(inp, logicalOperation):
+            if isinstance(inp, LogicalOperation):
                 res = res & inp
             else:
                 res = res & (inp != 0)
 
     return res
 
 
@@ -151,44 +162,46 @@
     Returns:
         OR intersection
 
     """
     # If necessary, flatten inputs
     if len(inputs) == 1 and isinstance(inputs[0], (list, tuple)):
         inputs = inputs[0]
-
     # Add support for generator inputs (to have the same behavior as built-in `any` function)
-    if isinstance(inputs, tuple) and len(inputs) == 1 and inspect.isgenerator(inputs[0]):
+    if (
+        isinstance(inputs, tuple)
+        and len(inputs) == 1
+        and inspect.isgenerator(inputs[0])
+    ):
         inputs = list(inputs[0])
-
     # Transforming potential filepaths to pyotb objects
     inputs = [Input(inp) if isinstance(inp, str) else inp for inp in inputs]
 
     # Checking that at least one band of the image is True
     if len(inputs) == 1:
         inp = inputs[0]
-        if isinstance(inp, logicalOperation):
+        if isinstance(inp, LogicalOperation):
             res = inp[:, :, 0]
         else:
-            res = (inp[:, :, 0] != 0)
+            res = inp[:, :, 0] != 0
 
         for band in range(1, inp.shape[-1]):
-            if isinstance(inp, logicalOperation):
+            if isinstance(inp, LogicalOperation):
                 res = res | inp[:, :, band]
             else:
                 res = res | (inp[:, :, band] != 0)
 
     # Checking that at least one image is True
     else:
-        if isinstance(inputs[0], logicalOperation):
+        if isinstance(inputs[0], LogicalOperation):
             res = inputs[0]
         else:
-            res = (inputs[0] != 0)
+            res = inputs[0] != 0
         for inp in inputs[1:]:
-            if isinstance(inp, logicalOperation):
+            if isinstance(inp, LogicalOperation):
                 res = res | inp
             else:
                 res = res | (inp != 0)
 
     return res
 
 
@@ -210,18 +223,22 @@
         func: function taking one or several inputs and returning *one* output
 
     Returns:
         wrapper: a function that returns a pyotb object
 
     """
     try:
-        from .apps import TensorflowModelServe
+        from .apps import (  # pylint: disable=import-outside-toplevel
+            TensorflowModelServe,
+        )
     except ImportError:
-        logger.error('Could not run Tensorflow function: failed to import TensorflowModelServe.'
-                     'Check that you have OTBTF configured (https://github.com/remicres/otbtf#how-to-install)')
+        logger.error(
+            "Could not run Tensorflow function: failed to import TensorflowModelServe."
+            "Check that you have OTBTF configured (https://github.com/remicres/otbtf#how-to-install)"
+        )
         raise
 
     def get_tf_pycmd(output_dir, channels, scalar_inputs):
         """Create a string containing all python instructions necessary to create and save the Keras model.
 
         Args:
             output_dir: directory under which to save the model
@@ -234,17 +251,17 @@
         """
         # Getting the string definition of the tf function (e.g. "def multiply(x1, x2):...")
         # TODO: maybe not entirely foolproof, maybe we should use dill instead? but it would add a dependency
         func_def_str = inspect.getsource(func)
         func_name = func.__name__
 
         create_and_save_model_str = func_def_str
-
         # Adding the instructions to create the model and save it to output dir
-        create_and_save_model_str += textwrap.dedent(f"""
+        create_and_save_model_str += textwrap.dedent(
+            f"""
             import tensorflow as tf
 
             model_inputs = []
             tf_inputs = []
             for channel, scalar_input in zip({channels}, {scalar_inputs}):
                 if channel:
                     input = tf.keras.Input((None, None, channel))
@@ -256,19 +273,20 @@
                     tf_inputs.append(scalar_input)
 
             output = {func_name}(*tf_inputs)
 
             # Create and save the .pb model
             model = tf.keras.Model(inputs=model_inputs, outputs=output)
             model.save("{output_dir}")
-            """)
+            """
+        )
 
         return create_and_save_model_str
 
-    def wrapper(*inputs, tmp_dir='/tmp'):
+    def wrapper(*inputs, tmp_dir="/tmp"):
         """For the user point of view, this function simply applies some TensorFlow operations to some rasters.
 
         Implicitly, it saves a .pb model that describe the TF operations, then creates an OTB ModelServe application
         that applies this .pb model to the inputs.
 
         Args:
             *inputs: a list of pyotb objects, filepaths or int/float numbers
@@ -292,41 +310,59 @@
             except TypeError:
                 # this is for other inputs (float, int)
                 channels.append(None)
                 scalar_inputs.append(inp)
 
         # Create and save the model. This is executed **inside an independent process** because (as of 2022-03),
         # tensorflow python library and OTBTF are incompatible
-        out_savedmodel = os.path.join(tmp_dir, f'tmp_otbtf_model_{uuid.uuid4()}')
+        out_savedmodel = os.path.join(tmp_dir, f"tmp_otbtf_model_{uuid.uuid4()}")
         pycmd = get_tf_pycmd(out_savedmodel, channels, scalar_inputs)
         cmd_args = [sys.executable, "-c", pycmd]
         try:
-            import subprocess
-            subprocess.run(cmd_args, env=os.environ, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=True)
+            subprocess.run(
+                cmd_args,
+                env=os.environ,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                check=True,
+            )
         except subprocess.SubprocessError:
             logger.debug("Failed to call subprocess")
         if not os.path.isdir(out_savedmodel):
             logger.info("Failed to save the model")
 
         # Initialize the OTBTF model serving application
-        model_serve = TensorflowModelServe({'model.dir': out_savedmodel, 'optim.disabletiling': 'on',
-                                            'model.fullyconv': 'on'}, n_sources=len(raster_inputs), frozen=True)
+        model_serve = TensorflowModelServe(
+            {
+                "model.dir": out_savedmodel,
+                "optim.disabletiling": "on",
+                "model.fullyconv": "on",
+            },
+            n_sources=len(raster_inputs),
+            frozen=True,
+        )
         # Set parameters and execute
         for i, inp in enumerate(raster_inputs):
-            model_serve.set_parameters({f'source{i + 1}.il': [inp]})
+            model_serve.set_parameters({f"source{i + 1}.il": [inp]})
         model_serve.execute()
         # TODO: handle the deletion of the temporary model ?
 
         return model_serve
 
     return wrapper
 
 
-def define_processing_area(*args, window_rule='intersection', pixel_size_rule='minimal', interpolator='nn',
-                           reference_window_input=None, reference_pixel_size_input=None):
+def define_processing_area(
+    *args,
+    window_rule: str = "intersection",
+    pixel_size_rule: str = "minimal",
+    interpolator: str = "nn",
+    reference_window_input: dict = None,
+    reference_pixel_size_input: str = None,
+) -> list[App]:
     """Given several inputs, this function handles the potential resampling and cropping to same extent.
 
     WARNING: Not fully implemented / tested
 
     Args:
         *args: list of raster inputs. Can be str (filepath) or pyotb objects
         window_rule: Can be 'intersection', 'union', 'same_as_input', 'specify' (Default value = 'intersection')
@@ -342,146 +378,192 @@
     # Flatten all args into one list
     inputs = []
     for arg in args:
         if isinstance(arg, (list, tuple)):
             inputs.extend(arg)
         else:
             inputs.append(arg)
-
     # Getting metadatas of inputs
     metadatas = {}
     for inp in inputs:
         if isinstance(inp, str):  # this is for filepaths
-            metadata = Input(inp).GetImageMetaData('out')
-        elif isinstance(inp, otbObject):
-            metadata = inp.GetImageMetaData(inp.output_param)
+            metadata = Input(inp).app.GetImageMetaData("out")
+        elif isinstance(inp, App):
+            metadata = inp.app.GetImageMetaData(inp.output_param)
         else:
             raise TypeError(f"Wrong input : {inp}")
         metadatas[inp] = metadata
 
     # Get a metadata of an arbitrary image. This is just to compare later with other images
     any_metadata = next(iter(metadatas.values()))
-
     # Checking if all images have the same projection
-    if not all(metadata['ProjectionRef'] == any_metadata['ProjectionRef']
-               for metadata in metadatas.values()):
-        logger.warning('All images may not have the same CRS, which might cause unpredictable results')
+    if not all(
+        metadata["ProjectionRef"] == any_metadata["ProjectionRef"]
+        for metadata in metadatas.values()
+    ):
+        logger.warning(
+            "All images may not have the same CRS, which might cause unpredictable results"
+        )
 
     # Handling different spatial footprints
     # TODO: there seems to have a bug, ImageMetaData is not updated when running an app,
     #  cf https://gitlab.orfeo-toolbox.org/orfeotoolbox/otb/-/issues/2234. Should we use ImageOrigin instead?
-    if not all(metadata['UpperLeftCorner'] == any_metadata['UpperLeftCorner']
-               and metadata['LowerRightCorner'] == any_metadata['LowerRightCorner']
-               for metadata in metadatas.values()):
+    if not all(
+        metadata["UpperLeftCorner"] == any_metadata["UpperLeftCorner"]
+        and metadata["LowerRightCorner"] == any_metadata["LowerRightCorner"]
+        for metadata in metadatas.values()
+    ):
         # Retrieving the bounding box that will be common for all inputs
-        if window_rule == 'intersection':
+        if window_rule == "intersection":
             # The coordinates depend on the orientation of the axis of projection
-            if any_metadata['GeoTransform'][1] >= 0:
-                ulx = max(metadata['UpperLeftCorner'][0] for metadata in metadatas.values())
-                lrx = min(metadata['LowerRightCorner'][0] for metadata in metadatas.values())
+            if any_metadata["GeoTransform"][1] >= 0:
+                ulx = max(
+                    metadata["UpperLeftCorner"][0] for metadata in metadatas.values()
+                )
+                lrx = min(
+                    metadata["LowerRightCorner"][0] for metadata in metadatas.values()
+                )
             else:
-                ulx = min(metadata['UpperLeftCorner'][0] for metadata in metadatas.values())
-                lrx = max(metadata['LowerRightCorner'][0] for metadata in metadatas.values())
-            if any_metadata['GeoTransform'][-1] >= 0:
-                lry = min(metadata['LowerRightCorner'][1] for metadata in metadatas.values())
-                uly = max(metadata['UpperLeftCorner'][1] for metadata in metadatas.values())
+                ulx = min(
+                    metadata["UpperLeftCorner"][0] for metadata in metadatas.values()
+                )
+                lrx = max(
+                    metadata["LowerRightCorner"][0] for metadata in metadatas.values()
+                )
+            if any_metadata["GeoTransform"][-1] >= 0:
+                lry = min(
+                    metadata["LowerRightCorner"][1] for metadata in metadatas.values()
+                )
+                uly = max(
+                    metadata["UpperLeftCorner"][1] for metadata in metadatas.values()
+                )
             else:
-                lry = max(metadata['LowerRightCorner'][1] for metadata in metadatas.values())
-                uly = min(metadata['UpperLeftCorner'][1] for metadata in metadatas.values())
-
-        elif window_rule == 'same_as_input':
-            ulx = metadatas[reference_window_input]['UpperLeftCorner'][0]
-            lrx = metadatas[reference_window_input]['LowerRightCorner'][0]
-            lry = metadatas[reference_window_input]['LowerRightCorner'][1]
-            uly = metadatas[reference_window_input]['UpperLeftCorner'][1]
-        elif window_rule == 'specify':
+                lry = max(
+                    metadata["LowerRightCorner"][1] for metadata in metadatas.values()
+                )
+                uly = min(
+                    metadata["UpperLeftCorner"][1] for metadata in metadatas.values()
+                )
+
+        elif window_rule == "same_as_input":
+            ulx = metadatas[reference_window_input]["UpperLeftCorner"][0]
+            lrx = metadatas[reference_window_input]["LowerRightCorner"][0]
+            lry = metadatas[reference_window_input]["LowerRightCorner"][1]
+            uly = metadatas[reference_window_input]["UpperLeftCorner"][1]
+        elif window_rule == "specify":
             pass
             # TODO : it is when the user explicitly specifies the bounding box -> add some arguments in the function
-        elif window_rule == 'union':
+        elif window_rule == "union":
             pass
             # TODO : it is when the user wants the final bounding box to be the union of all bounding box
             #  It should replace any 'outside' pixel by some NoData -> add `fillvalue` argument in the function
 
-        logger.info('Cropping all images to extent Upper Left (%s, %s), Lower Right (%s, %s)', ulx, uly, lrx, lry)
-
         # Applying this bounding box to all inputs
+        logger.info(
+            "Cropping all images to extent Upper Left (%s, %s), Lower Right (%s, %s)",
+            ulx,
+            uly,
+            lrx,
+            lry,
+        )
         new_inputs = []
         for inp in inputs:
             try:
                 params = {
-                    'in': inp, 'mode': 'extent', 'mode.extent.unit': 'phy',
-                    'mode.extent.ulx': ulx, 'mode.extent.uly': lry,  # bug in OTB <= 7.3 :
-                    'mode.extent.lrx': lrx, 'mode.extent.lry': uly,  # ULY/LRY are inverted
+                    "in": inp,
+                    "mode": "extent",
+                    "mode.extent.unit": "phy",
+                    "mode.extent.ulx": ulx,
+                    "mode.extent.uly": lry,  # bug in OTB <= 7.3 :
+                    "mode.extent.lrx": lrx,
+                    "mode.extent.lry": uly,  # ULY/LRY are inverted
                 }
-                new_input = App('ExtractROI', params)
+                new_input = App("ExtractROI", params)
                 # TODO: OTB 7.4 fixes this bug, how to handle different versions of OTB?
                 new_inputs.append(new_input)
                 # Potentially update the reference inputs for later resampling
-                if str(inp) == str(reference_pixel_size_input):  # we use comparison of string because calling '=='
+                if str(inp) == str(
+                    reference_pixel_size_input
+                ):  # we use comparison of string because calling '=='
                     # on pyotb objects implicitly calls BandMathX application, which is not desirable
                     reference_pixel_size_input = new_input
             except RuntimeError as e:
-                logger.error('Cannot define the processing area for input %s: %s', inp, e)
+                logger.error(
+                    "Cannot define the processing area for input %s: %s", inp, e
+                )
                 raise
         inputs = new_inputs
-
         # Update metadatas
-        metadatas = {input: input.GetImageMetaData('out') for input in inputs}
+        metadatas = {input: input.app.GetImageMetaData("out") for input in inputs}
 
     # Get a metadata of an arbitrary image. This is just to compare later with other images
     any_metadata = next(iter(metadatas.values()))
-
     # Handling different pixel sizes
-    if not all(metadata['GeoTransform'][1] == any_metadata['GeoTransform'][1]
-               and metadata['GeoTransform'][5] == any_metadata['GeoTransform'][5]
-               for metadata in metadatas.values()):
+    if not all(
+        metadata["GeoTransform"][1] == any_metadata["GeoTransform"][1]
+        and metadata["GeoTransform"][5] == any_metadata["GeoTransform"][5]
+        for metadata in metadatas.values()
+    ):
         # Retrieving the pixel size that will be common for all inputs
-        if pixel_size_rule == 'minimal':
+        if pixel_size_rule == "minimal":
             # selecting the input with the smallest x pixel size
-            reference_input = min(metadatas, key=lambda x: metadatas[x]['GeoTransform'][1])
-        if pixel_size_rule == 'maximal':
+            reference_input = min(
+                metadatas, key=lambda x: metadatas[x]["GeoTransform"][1]
+            )
+        if pixel_size_rule == "maximal":
             # selecting the input with the highest x pixel size
-            reference_input = max(metadatas, key=lambda x: metadatas[x]['GeoTransform'][1])
-        elif pixel_size_rule == 'same_as_input':
+            reference_input = max(
+                metadatas, key=lambda x: metadatas[x]["GeoTransform"][1]
+            )
+        elif pixel_size_rule == "same_as_input":
             reference_input = reference_pixel_size_input
-        elif pixel_size_rule == 'specify':
+        elif pixel_size_rule == "specify":
             pass
             # TODO : when the user explicitly specify the pixel size -> add argument inside the function
-        pixel_size = metadatas[reference_input]['GeoTransform'][1]
-        logger.info('Resampling all inputs to resolution: %s', pixel_size)
+        pixel_size = metadatas[reference_input]["GeoTransform"][1]
 
         # Perform resampling on inputs that do not comply with the target pixel size
+        logger.info("Resampling all inputs to resolution: %s", pixel_size)
         new_inputs = []
         for inp in inputs:
-            if metadatas[inp]['GeoTransform'][1] != pixel_size:
-                superimposed = App('Superimpose', inr=reference_input, inm=inp, interpolator=interpolator)
+            if metadatas[inp]["GeoTransform"][1] != pixel_size:
+                superimposed = App(
+                    "Superimpose",
+                    inr=reference_input,
+                    inm=inp,
+                    interpolator=interpolator,
+                )
                 new_inputs.append(superimposed)
             else:
                 new_inputs.append(inp)
         inputs = new_inputs
-
-        # Update metadatas
-        metadatas = {inp: inp.GetImageMetaData('out') for inp in inputs}
+        metadatas = {inp: inp.app.GetImageMetaData("out") for inp in inputs}
 
     # Final superimposition to be sure to have the exact same image sizes
-    # Getting the sizes of images
     image_sizes = {}
     for inp in inputs:
         if isinstance(inp, str):
             inp = Input(inp)
         image_sizes[inp] = inp.shape[:2]
-
     # Selecting the most frequent image size. It will be used as reference.
     most_common_image_size, _ = Counter(image_sizes.values()).most_common(1)[0]
-    same_size_images = [inp for inp, image_size in image_sizes.items() if image_size == most_common_image_size]
+    same_size_images = [
+        inp
+        for inp, image_size in image_sizes.items()
+        if image_size == most_common_image_size
+    ]
 
     # Superimposition for images that do not have the same size as the others
     new_inputs = []
     for inp in inputs:
         if image_sizes[inp] != most_common_image_size:
-            superimposed = App('Superimpose', inr=same_size_images[0], inm=inp, interpolator=interpolator)
+            superimposed = App(
+                "Superimpose",
+                inr=same_size_images[0],
+                inm=inp,
+                interpolator=interpolator,
+            )
             new_inputs.append(superimposed)
         else:
             new_inputs.append(inp)
-    inputs = new_inputs
 
-    return inputs
+    return new_inputs
```

### Comparing `pyotb-1.5.4/pyotb/helpers.py` & `pyotb-2.0.0.dev1/pyotb/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 # -*- coding: utf-8 -*-
-"""This module provides some helpers to properly initialize pyotb."""
+"""This module helps to ensure we properly initialize pyotb: only in case OTB is found and apps are available."""
+import logging
 import os
 import sys
-import logging
 from pathlib import Path
 from shutil import which
 
-
 # Allow user to switch between OTB directories without setting every env variable
 OTB_ROOT = os.environ.get("OTB_ROOT")
 
 # Logging
 # User can also get logger with `logging.getLogger("pyOTB")`
 # then use pyotb.set_logger_level() to adjust logger verbosity
 logger = logging.getLogger("pyOTB")
 logger_handler = logging.StreamHandler(sys.stdout)
-formatter = logging.Formatter(fmt="%(asctime)s (%(levelname)-4s) [pyOTB] %(message)s", datefmt="%Y-%m-%d %H:%M:%S")
+formatter = logging.Formatter(
+    fmt="%(asctime)s (%(levelname)-4s) [pyOTB] %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
+)
 logger_handler.setFormatter(formatter)
 # Search for PYOTB_LOGGER_LEVEL, else use OTB_LOGGER_LEVEL as pyOTB level, or fallback to INFO
-LOG_LEVEL = os.environ.get("PYOTB_LOGGER_LEVEL") or os.environ.get("OTB_LOGGER_LEVEL") or "INFO"
+LOG_LEVEL = (
+    os.environ.get("PYOTB_LOGGER_LEVEL") or os.environ.get("OTB_LOGGER_LEVEL") or "INFO"
+)
 logger.setLevel(getattr(logging, LOG_LEVEL))
 # Here it would be possible to use a different level for a specific handler
 # A more verbose one can go to text file while print only errors to stdout
 logger_handler.setLevel(getattr(logging, LOG_LEVEL))
 logger.addHandler(logger_handler)
 
 
-def set_logger_level(level):
+def set_logger_level(level: str):
     """Allow user to change the current logging level.
 
     Args:
         level: logging level string ('DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL')
     """
     logger.setLevel(getattr(logging, level))
     logger_handler.setLevel(getattr(logging, level))
 
 
-def find_otb(prefix=OTB_ROOT, scan=True, scan_userdir=True):
+def find_otb(prefix: str = OTB_ROOT, scan: bool = True, scan_userdir: bool = True):
     """Try to load OTB bindings or scan system, help user in case of failure, set env variables.
 
     Path precedence :                                OTB_ROOT > python bindings directory
         OR search for releases installations    :    HOME
-        OR (for linux)                          :    /opt/otbtf > /opt/otb > /usr/local > /usr
-        OR (for windows)                        :    C:/Program Files
+        OR (for Linux)                          :    /opt/otbtf > /opt/otb > /usr/local > /usr
+        OR (for MacOS)                          :    ~/Applications
+        OR (for Windows)                        :    C:/Program Files
 
     Args:
         prefix: prefix to search OTB in (Default value = OTB_ROOT)
         scan: find otb in system known locations (Default value = True)
         scan_userdir: search for OTB release in user's home directory (Default value = True)
 
     Returns:
@@ -55,67 +59,72 @@
     """
     otb = None
     # Try OTB_ROOT env variable first (allow override default OTB version)
     if prefix:
         try:
             set_environment(prefix)
             import otbApplication as otb  # pylint: disable=import-outside-toplevel
+
             return otb
         except EnvironmentError as e:
             raise SystemExit(f"Failed to import OTB with prefix={prefix}") from e
         except ImportError as e:
             __suggest_fix_import(str(e), prefix)
             raise SystemExit("Failed to import OTB. Exiting.") from e
     # Else try import from actual Python path
     try:
         # Here, we can't properly set env variables before OTB import. We assume user did this before running python
         # For LD_LIBRARY_PATH problems, use OTB_ROOT instead of PYTHONPATH
         import otbApplication as otb  # pylint: disable=import-outside-toplevel
+
         if "OTB_APPLICATION_PATH" not in os.environ:
             lib_dir = __find_lib(otb_module=otb)
             apps_path = __find_apps_path(lib_dir)
             otb.Registry.SetApplicationPath(apps_path)
         return otb
     except ImportError as e:
-        PYTHONPATH = os.environ.get("PYTHONPATH")
+        pythonpath = os.environ.get("PYTHONPATH")
         if not scan:
-            raise SystemExit(f"Failed to import OTB with env PYTHONPATH={PYTHONPATH}") from e
+            raise SystemExit(
+                f"Failed to import OTB with env PYTHONPATH={pythonpath}"
+            ) from e
     # Else search system
     logger.info("Failed to import OTB. Searching for it...")
     prefix = __find_otb_root(scan_userdir)
     # Try to import one last time before raising error
     try:
         set_environment(prefix)
         import otbApplication as otb  # pylint: disable=import-outside-toplevel
+
         return otb
     except EnvironmentError as e:
         raise SystemExit("Auto setup for OTB env failed. Exiting.") from e
     # Unknown error
     except ModuleNotFoundError as e:
         raise SystemExit("Can't run without OTB installed. Exiting.") from e
     # Help user to fix this
     except ImportError as e:
         __suggest_fix_import(str(e), prefix)
         raise SystemExit("Failed to import OTB. Exiting.") from e
 
 
-def set_environment(prefix):
+def set_environment(prefix: str):
     """Set environment variables (before OTB import), raise error if anything is wrong.
 
     Args:
         prefix: path to OTB root directory
 
     """
     logger.info("Preparing environment for OTB in %s", prefix)
     # OTB root directory
     prefix = Path(prefix)
     if not prefix.exists():
         raise FileNotFoundError(str(prefix))
     built_from_source = False
-    if not (prefix / 'README').exists():
+    if not (prefix / "README").exists():
         built_from_source = True
     # External libraries
     lib_dir = __find_lib(prefix)
     if not lib_dir:
         raise EnvironmentError("Can't find OTB external libraries")
     # This does not seems to work
     if sys.platform == "linux" and built_from_source:
@@ -131,48 +140,49 @@
     os.environ["PATH"] = f"{prefix / 'bin'}{os.pathsep}{os.environ['PATH']}"
     # Applications path  (this can be tricky since OTB import will succeed even without apps)
     apps_path = __find_apps_path(lib_dir)
     if Path(apps_path).exists():
         os.environ["OTB_APPLICATION_PATH"] = apps_path
     else:
         raise EnvironmentError("Can't find OTB applications directory")
-
     os.environ["LC_NUMERIC"] = "C"
     os.environ["GDAL_DRIVER_PATH"] = "disable"
+
     if (prefix / "share/gdal").exists():
         # Local GDAL (OTB Superbuild, .run, .exe)
         gdal_data = str(prefix / "share/gdal")
         proj_lib = str(prefix / "share/proj")
     elif sys.platform == "linux":
         # If installed using apt or built from source with system deps
         gdal_data = "/usr/share/gdal"
         proj_lib = "/usr/share/proj"
     elif sys.platform == "win32":
         gdal_data = str(prefix / "share/data")
         proj_lib = str(prefix / "share/proj")
     else:
-        raise EnvironmentError(f"Can't find GDAL location with current OTB prefix '{prefix}' or in /usr")
-
+        raise EnvironmentError(
+            f"Can't find GDAL location with current OTB prefix '{prefix}' or in /usr"
+        )
     os.environ["GDAL_DATA"] = gdal_data
     os.environ["PROJ_LIB"] = proj_lib
 
 
-def __find_lib(prefix=None, otb_module=None):
+def __find_lib(prefix: str = None, otb_module=None):
     """Try to find OTB external libraries directory.
 
     Args:
         prefix: try with OTB root directory
         otb_module: try with OTB python module (otbApplication) library path if found, else None
 
     Returns:
         lib path
 
     """
     if prefix is not None:
-        lib_dir = prefix / 'lib'
+        lib_dir = prefix / "lib"
         if lib_dir.exists():
             return lib_dir.absolute()
     if otb_module is not None:
         lib_dir = Path(otb_module.__file__).parent.parent
         # Case OTB .run file
         if lib_dir.name == "lib":
             return lib_dir.absolute()
@@ -183,15 +193,15 @@
         # Case built from source (/usr/local, /opt/otb, ...)
         lib_dir = lib_dir.parent
         if lib_dir.name == "lib":
             return lib_dir.absolute()
     return None
 
 
-def __find_python_api(lib_dir):
+def __find_python_api(lib_dir: Path):
     """Try to find the python path.
 
     Args:
         prefix: prefix
 
     Returns:
         python API path if found, else None
@@ -202,15 +212,15 @@
         otb_api = lib_dir / "otb/python"
     if otb_api.exists():
         return str(otb_api.absolute())
     logger.debug("Failed to find OTB python bindings directory")
     return None
 
 
-def __find_apps_path(lib_dir):
+def __find_apps_path(lib_dir: Path):
     """Try to find the OTB applications path.
 
     Args:
         lib_dir: library path
 
     Returns:
         application path if found, else empty string
@@ -221,15 +231,15 @@
         if otb_application_path.exists():
             return str(otb_application_path.absolute())
         # This should not happen, may be with failed builds ?
         logger.error("Library directory found but 'applications' is missing")
     return ""
 
 
-def __find_otb_root(scan_userdir=False):
+def __find_otb_root(scan_userdir: bool = False):
     """Search for OTB root directory in well known locations.
 
     Args:
         scan_userdir: search with glob in $HOME directory
 
     Returns:
         str path of the OTB directory
@@ -255,55 +265,76 @@
                 prefix = path.parent.parent
             prefix = prefix.absolute()
     elif sys.platform == "win32":
         for path in Path("c:/Program Files").glob("**/OTB-*/lib"):
             logger.info("Found %s", path.parent)
             prefix = path.parent.absolute()
     elif sys.platform == "darwin":
-        # TODO: find OTB in macOS
-        pass
-
+        for path in (Path.home() / "Applications").glob("**/OTB-*/lib"):
+            logger.info("Found %s", path.parent)
+            prefix = path.parent.absolute()
     # If possible, use OTB found in user's HOME tree (this may take some time)
     if scan_userdir:
-        for path in Path().home().glob("**/OTB-*/lib"):
+        for path in Path.home().glob("**/OTB-*/lib"):
             logger.info("Found %s", path.parent)
             prefix = path.parent.absolute()
-
+    # Return latest found prefix (and version), see precedence in function def find_otb()
     return prefix
 
 
-def __suggest_fix_import(error_message, prefix):
+def __suggest_fix_import(error_message: str, prefix: str):
     """Help user to fix the OTB installation with appropriate log messages."""
     logger.critical("An error occurred while importing OTB Python API")
     logger.critical("OTB error message was '%s'", error_message)
     if sys.platform == "linux":
-        if error_message.startswith('libpython3.'):
-            logger.critical("It seems like you need to symlink or recompile python bindings")
-            if sys.executable.startswith('/usr/bin'):
-                lib = f"/usr/lib/x86_64-linux-gnu/libpython3.{sys.version_info.minor}.so"
-                if which('ctest'):
-                    logger.critical("To recompile python bindings, use 'cd %s ; source otbenv.profile ; "
-                                    "ctest -S share/otb/swig/build_wrapping.cmake -VV'", prefix)
+        if error_message.startswith("libpython3."):
+            logger.critical(
+                "It seems like you need to symlink or recompile python bindings"
+            )
+            if sys.executable.startswith("/usr/bin"):
+                lib = (
+                    f"/usr/lib/x86_64-linux-gnu/libpython3.{sys.version_info.minor}.so"
+                )
+                if which("ctest"):
+                    logger.critical(
+                        "To recompile python bindings, use 'cd %s ; source otbenv.profile ; "
+                        "ctest -S share/otb/swig/build_wrapping.cmake -VV'",
+                        prefix,
+                    )
                 elif Path(lib).exists():
                     expect_minor = int(error_message[11])
                     if expect_minor != sys.version_info.minor:
-                        logger.critical("Python library version mismatch (OTB was expecting 3.%s) : "
-                                        "a simple symlink may not work, depending on your python version", expect_minor)
+                        logger.critical(
+                            "Python library version mismatch (OTB was expecting 3.%s) : "
+                            "a simple symlink may not work, depending on your python version",
+                            expect_minor,
+                        )
                     target_lib = f"{prefix}/lib/libpython3.{expect_minor}.so.rh-python3{expect_minor}-1.0"
                     logger.critical("Use 'ln -s %s %s'", lib, target_lib)
                 else:
-                    logger.critical("You may need to install cmake in order to recompile python bindings")
+                    logger.critical(
+                        "You may need to install cmake in order to recompile python bindings"
+                    )
             else:
-                logger.critical("Unable to automatically locate python dynamic library of %s", sys.executable)
-            return
+                logger.critical(
+                    "Unable to automatically locate python dynamic library of %s",
+                    sys.executable,
+                )
     elif sys.platform == "win32":
         if error_message.startswith("DLL load failed"):
             if sys.version_info.minor != 7:
-                logger.critical("You need Python 3.5 (OTB releases 6.4 to 7.4) or Python 3.7 (since OTB 8)")
-                issue_link = "https://gitlab.orfeo-toolbox.org/orfeotoolbox/otb/-/issues/2010"
-                logger.critical("Another workaround is to recompile Python bindings with cmake, see %s", issue_link)
+                logger.critical(
+                    "You need Python 3.5 (OTB releases 6.4 to 7.4) or Python 3.7 (since OTB 8)"
+                )
             else:
-                logger.critical("It seems that your env variables aren't properly set,"
-                                " first use 'call otbenv.bat' then try to import pyotb once again")
-            return
+                logger.critical(
+                    "It seems that your env variables aren't properly set,"
+                    " first use 'call otbenv.bat' then try to import pyotb once again"
+                )
     docs_link = "https://www.orfeo-toolbox.org/CookBook/Installation.html"
-    logger.critical("You can verify installation requirements for your OS at %s", docs_link)
+    logger.critical(
+        "You can verify installation requirements for your OS at %s", docs_link
+    )
+
+
+# Since helpers is the first module to be inititialized, this will prevent pyotb to run if OTB is not found
+find_otb()
```

