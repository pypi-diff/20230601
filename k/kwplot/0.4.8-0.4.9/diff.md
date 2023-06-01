# Comparing `tmp/kwplot-0.4.8.tar.gz` & `tmp/kwplot-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwplot-0.4.8.tar", last modified: Thu Apr 22 21:54:59 2021, max compression
+gzip compressed data, was "kwplot-0.4.9.tar", last modified: Mon Aug 23 14:50:31 2021, max compression
```

## Comparing `kwplot-0.4.8.tar` & `kwplot-0.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 21:54:59.625676 kwplot-0.4.8/
--rw-r--r--   0 root         (0) root         (0)     4499 2021-04-22 21:54:59.625676 kwplot-0.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2966 2021-04-22 21:54:47.000000 kwplot-0.4.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 21:54:59.625676 kwplot-0.4.8/kwplot/
--rw-rw-rw-   0 root         (0) root         (0)     1484 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12791 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/auto_backends.py
--rw-rw-rw-   0 root         (0) root         (0)    12482 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/draw_conv.py
--rw-rw-rw-   0 root         (0) root         (0)     3665 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/mpl_3d.py
--rw-rw-rw-   0 root         (0) root         (0)     4468 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/mpl_color.py
--rw-rw-rw-   0 root         (0) root         (0)    21434 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/mpl_core.py
--rw-rw-rw-   0 root         (0) root         (0)    12339 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/mpl_draw.py
--rw-rw-rw-   0 root         (0) root         (0)     7780 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/mpl_make.py
--rw-rw-rw-   0 root         (0) root         (0)    29680 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/mpl_multiplot.py
--rw-rw-rw-   0 root         (0) root         (0)     6224 2021-04-22 21:54:47.000000 kwplot-0.4.8/kwplot/mpl_plotnums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-22 21:54:59.625676 kwplot-0.4.8/kwplot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4499 2021-04-22 21:54:59.000000 kwplot-0.4.8/kwplot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2021-04-22 21:54:59.000000 kwplot-0.4.8/kwplot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-22 21:54:59.000000 kwplot-0.4.8/kwplot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      199 2021-04-22 21:54:59.000000 kwplot-0.4.8/kwplot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2021-04-22 21:54:59.000000 kwplot-0.4.8/kwplot.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      142 2021-04-22 21:54:47.000000 kwplot-0.4.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-04-22 21:54:59.625676 kwplot-0.4.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     6985 2021-04-22 21:54:47.000000 kwplot-0.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 14:50:31.291664 kwplot-0.4.9/
+-rw-r--r--   0 root         (0) root         (0)     4499 2021-08-23 14:50:31.291664 kwplot-0.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2966 2021-08-23 14:50:16.000000 kwplot-0.4.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 14:50:31.287664 kwplot-0.4.9/kwplot/
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13180 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/auto_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)    12482 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/draw_conv.py
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/mpl_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)     4468 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/mpl_color.py
+-rw-rw-rw-   0 root         (0) root         (0)    21434 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/mpl_core.py
+-rw-rw-rw-   0 root         (0) root         (0)    12339 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/mpl_draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     7780 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/mpl_make.py
+-rw-rw-rw-   0 root         (0) root         (0)    29680 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/mpl_multiplot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6215 2021-08-23 14:50:16.000000 kwplot-0.4.9/kwplot/mpl_plotnums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-23 14:50:31.287664 kwplot-0.4.9/kwplot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4499 2021-08-23 14:50:31.000000 kwplot-0.4.9/kwplot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2021-08-23 14:50:31.000000 kwplot-0.4.9/kwplot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-23 14:50:31.000000 kwplot-0.4.9/kwplot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2021-08-23 14:50:31.000000 kwplot-0.4.9/kwplot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2021-08-23 14:50:31.000000 kwplot-0.4.9/kwplot.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      142 2021-08-23 14:50:16.000000 kwplot-0.4.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-23 14:50:31.291664 kwplot-0.4.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     6985 2021-08-23 14:50:16.000000 kwplot-0.4.9/setup.py
```

### Comparing `kwplot-0.4.8/PKG-INFO` & `kwplot-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwplot
-Version: 0.4.8
+Version: 0.4.9
 Summary: A wrapper around matplotlib
 Home-page: https://gitlab.kitware.com/computer-vision/kwplot
 Author: Kitware Inc., Jon Crall
 Author-email: kitware@kitware.com, jon.crall@kitware.com
 License: Apache 2
 Description: The Kitware Plot Module
         =======================
```

### Comparing `kwplot-0.4.8/README.rst` & `kwplot-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/__init__.py` & `kwplot-0.4.9/kwplot/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 mkinit ~/code/kwplot/kwplot/__init__.py -w --relative --nomods
+mkinit ~/code/kwplot/kwplot/__init__.py --diff --relative --nomods
 """
 
-__version__ = '0.4.8'
+__version__ = '0.4.9'
 
-from .auto_backends import (BackendContext, autompl, autoplt, set_mpl_backend,)
+from .auto_backends import (BackendContext, autompl, autoplt, autosns,
+                            set_mpl_backend,)
 from .draw_conv import (make_conv_images, plot_convolutional_features,)
 from .mpl_3d import (plot_surface3d,)
 from .mpl_color import (Color,)
 from .mpl_core import (distinct_colors, distinct_markers, ensure_fnum, figure,
                        imshow, legend, next_fnum, set_figtitle,
                        show_if_requested,)
 from .mpl_draw import (draw_boxes, draw_boxes_on_image, draw_clf_on_image,
@@ -16,15 +18,15 @@
                        plot_matrix,)
 from .mpl_make import (make_heatmask, make_legend_img, make_orimask,
                        make_vector_field,)
 from .mpl_multiplot import (multi_plot,)
 from .mpl_plotnums import (PlotNums,)
 
 __all__ = ['BackendContext', 'Color', 'PlotNums', 'autompl', 'autoplt',
-           'distinct_colors', 'distinct_markers', 'draw_boxes',
+           'autosns', 'distinct_colors', 'distinct_markers', 'draw_boxes',
            'draw_boxes_on_image', 'draw_clf_on_image', 'draw_line_segments',
            'draw_points', 'draw_text_on_image', 'ensure_fnum', 'figure',
            'imshow', 'legend', 'make_conv_images', 'make_heatmask',
            'make_legend_img', 'make_orimask', 'make_vector_field',
            'multi_plot', 'next_fnum', 'plot_convolutional_features',
            'plot_matrix', 'plot_surface3d', 'set_figtitle', 'set_mpl_backend',
            'show_if_requested']
```

### Comparing `kwplot-0.4.8/kwplot/auto_backends.py` & `kwplot-0.4.9/kwplot/auto_backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, division, print_function, unicode_literals
 import sys
 import os
 import ubelt as ub
 
 __all__ = [
-    'autompl', 'autoplt', 'set_mpl_backend', 'BackendContext',
+    'autompl', 'autoplt', 'autosns', 'set_mpl_backend', 'BackendContext',
 ]
 
 
 _qtensured = False
 
 
 def _current_ipython_session():
@@ -135,21 +135,22 @@
             print('AUTOMPL')
         if sys.platform.startswith('win32'):
             # TODO: something reasonable
             pass
         else:
             DISPLAY = os.environ.get('DISPLAY', '')
             if DISPLAY:
-                # Check if we can actually connect to X
-                # NOTE: this call takes a significant amount of time
-                info = ub.cmd('xdpyinfo', shell=True)
-                if verbose:
-                    print('xdpyinfo-info = {}'.format(ub.repr2(info)))
-                if info['ret'] != 0:
-                    DISPLAY = None
+                if sys.platform.startswith('linux') and ub.find_exe('xdpyinfo'):
+                    # On Linux, check if we can actually connect to X
+                    # NOTE: this call takes a significant amount of time
+                    info = ub.cmd('xdpyinfo', shell=True)
+                    if verbose:
+                        print('xdpyinfo-info = {}'.format(ub.repr2(info)))
+                    if info['ret'] != 0:
+                        DISPLAY = None
 
             if verbose:
                 print(' * DISPLAY = {!r}'.format(DISPLAY))
 
             if not DISPLAY:
                 backend = 'agg'
             else:
@@ -265,14 +266,25 @@
     convenience.
     """
     autompl(verbose=verbose, recheck=recheck)
     from matplotlib import pyplot as plt
     return plt
 
 
+def autosns(verbose=0, recheck=False):
+    """
+    Like autosns, but also calls `seaborn.set` and returns the `seaborn` module
+    for convenience.
+    """
+    autompl(verbose=verbose, recheck=recheck)
+    import seaborn as sns
+    sns.set()
+    return sns
+
+
 class BackendContext(object):
     """
     Context manager that ensures a specific backend, but then reverts after the
     context has ended.
 
     Checks:
         xdoctest -m kwplot.auto_backends BackendContext --check
```

### Comparing `kwplot-0.4.8/kwplot/draw_conv.py` & `kwplot-0.4.9/kwplot/draw_conv.py`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/mpl_3d.py` & `kwplot-0.4.9/kwplot/mpl_3d.py`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/mpl_color.py` & `kwplot-0.4.9/kwplot/mpl_color.py`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/mpl_core.py` & `kwplot-0.4.9/kwplot/mpl_core.py`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/mpl_draw.py` & `kwplot-0.4.9/kwplot/mpl_draw.py`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/mpl_make.py` & `kwplot-0.4.9/kwplot/mpl_make.py`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/mpl_multiplot.py` & `kwplot-0.4.9/kwplot/mpl_multiplot.py`

 * *Files identical despite different names*

### Comparing `kwplot-0.4.8/kwplot/mpl_plotnums.py` & `kwplot-0.4.9/kwplot/mpl_plotnums.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Example:
         >>> import ubelt as ub
         >>> pnum_ = PlotNums(nRows=2, nCols=2)
         >>> # Indexable
         >>> print(pnum_[0])
         (2, 2, 1)
         >>> # Iterable
-        >>> print(ub.repr2(list(pnum_), nl=0, nobr=True))
+        >>> print(ub.repr2(list(pnum_), nl=0, nobr=1))
         (2, 2, 1), (2, 2, 2), (2, 2, 3), (2, 2, 4)
         >>> # Callable (iterates through a default iterator)
         >>> print(pnum_())
         (2, 2, 1)
         >>> print(pnum_())
         (2, 2, 2)
     """
@@ -67,29 +67,29 @@
         r"""
         Yields:
             tuple : pnum
 
         Example:
             >>> import ubelt as ub
             >>> pnum_ = iter(PlotNums(nRows=3, nCols=2))
-            >>> result = ub.repr2(list(pnum_), nl=1, nobr=True)
+            >>> result = ub.repr2(list(pnum_), nl=1, nobr=1)
             >>> print(result)
             (3, 2, 1),
             (3, 2, 2),
             (3, 2, 3),
             (3, 2, 4),
             (3, 2, 5),
             (3, 2, 6),
 
         Example:
             >>> import ubelt as ub
             >>> nRows = 3
             >>> nCols = 2
             >>> pnum_ = iter(PlotNums(nRows, nCols, start=3))
-            >>> result = ub.repr2(list(pnum_), nl=1, nobr=True)
+            >>> result = ub.repr2(list(pnum_), nl=1, nobr=1)
             >>> print(result)
             (3, 2, 4),
             (3, 2, 5),
             (3, 2, 6),
         """
         for px in range(self.start, len(self)):
             yield self[px]
```

### Comparing `kwplot-0.4.8/kwplot.egg-info/PKG-INFO` & `kwplot-0.4.9/kwplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwplot
-Version: 0.4.8
+Version: 0.4.9
 Summary: A wrapper around matplotlib
 Home-page: https://gitlab.kitware.com/computer-vision/kwplot
 Author: Kitware Inc., Jon Crall
 Author-email: kitware@kitware.com, jon.crall@kitware.com
 License: Apache 2
 Description: The Kitware Plot Module
         =======================
```

### Comparing `kwplot-0.4.8/setup.py` & `kwplot-0.4.9/setup.py`

 * *Files identical despite different names*

