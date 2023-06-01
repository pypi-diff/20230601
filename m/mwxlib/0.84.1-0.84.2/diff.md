# Comparing `tmp/mwxlib-0.84.1-py3-none-any.whl.zip` & `tmp/mwxlib-0.84.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 162377 bytes, number of entries: 22
+Zip file size: 162402 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-May-02 16:40 mwx/__init__.py
--rw-rw-rw-  2.0 fat    43445 b- defN 23-May-02 17:15 mwx/controls.py
--rw-rw-rw-  2.0 fat    73753 b- defN 23-May-30 08:08 mwx/framework.py
--rw-rw-rw-  2.0 fat    69520 b- defN 23-May-25 03:20 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    43499 b- defN 23-May-31 05:42 mwx/controls.py
+-rw-rw-rw-  2.0 fat    73753 b- defN 23-Jun-01 04:39 mwx/framework.py
+-rw-rw-rw-  2.0 fat    69662 b- defN 23-Jun-01 04:39 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-May-17 04:56 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-May-17 11:19 mwx/matplot2g.py
--rw-rw-rw-  2.0 fat    27606 b- defN 23-Apr-27 09:45 mwx/matplot2lg.py
+-rw-rw-rw-  2.0 fat    27598 b- defN 23-Jun-01 04:39 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   138760 b- defN 23-May-30 08:08 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat   138759 b- defN 23-May-31 05:41 mwx/nutshell.py
 -rw-rw-rw-  2.0 fat    37431 b- defN 23-May-30 08:08 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-May-16 07:42 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-May-16 07:42 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-May-16 07:42 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-May-16 07:42 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Apr-27 09:45 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-May-30 08:37 mwxlib-0.84.1.dist-info/RECORD
-22 files, 615302 bytes uncompressed, 159875 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-01 04:41 mwxlib-0.84.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-01 04:41 mwxlib-0.84.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 04:41 mwxlib-0.84.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-01 04:41 mwxlib-0.84.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-01 04:41 mwxlib-0.84.2.dist-info/RECORD
+22 files, 615489 bytes uncompressed, 159900 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.84.1.dist-info/LICENSE
+Filename: mwxlib-0.84.2.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.84.1.dist-info/METADATA
+Filename: mwxlib-0.84.2.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.84.1.dist-info/WHEEL
+Filename: mwxlib-0.84.2.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.84.1.dist-info/top_level.txt
+Filename: mwxlib-0.84.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.84.1.dist-info/RECORD
+Filename: mwxlib-0.84.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/controls.py

```diff
@@ -7,15 +7,15 @@
 from itertools import chain
 import wx
 import wx.lib.platebtn as pb
 import wx.lib.scrolledpanel as scrolled
 
 from . import images
 from .utilus import SSM
-from .framework import pack, Menu, CtrlInterface
+from .framework import pack, Menu
 
 import numpy as np
 from numpy import nan, inf
 
 
 class Param(object):
     """Standard Parameter
@@ -50,15 +50,17 @@
         self.__value = value if value is not None else self.min
         self.__check = check
         if fmt is hex:
             self.__eval = lambda v: int(v, 16)
             self.__format = lambda v: '{:04X}'.format(int(v))
         else:
             self.__eval = lambda v: eval(v)
-            self.__format = fmt if callable(fmt) else (lambda v: (fmt or "%g") % v)
+            if isinstance(fmt, str):  # support % format:str
+                fmt = lambda v: fmt % v
+            self.__format = fmt or "{:,g}".format
         self.callback = SSM({
             'control' : [ handler ] if handler else [],
              'update' : [ updater ] if updater else [],
               'check' : [ updater ] if updater else [],
            'overflow' : [],
           'underflow' : [],
         })
@@ -761,16 +763,16 @@
                     p.value = v
                 except Exception as e: # failed to eval
                     print("- Failed to reset {!r}: {}".format(p, e))
                     pass
     
     def copy_to_clipboard(self, checked_only=False):
         params = self.get_params(checked_only)
-        text = '\t'.join(str(p) if isinstance(p, Param)
-                         else str(p.value) for p in params)
+        text = '\t'.join(str(p) if isinstance(p, Param) else
+                         str(p.value) for p in params)
         Clipboard.write(text)
     
     def paste_from_clipboard(self, checked_only=False):
         text = Clipboard.read()
         if text:
             self.reset_params(text.split('\t'), checked_only)
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.84.1"
+__version__ = "0.84.2"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
```

## mwx/graphman.py

```diff
@@ -377,15 +377,16 @@
         lambda self,v: self.Show(v))
     
     def IsShown(self):
         return self.parent.get_pane(self).IsShown()
     
     def Show(self, show=True):
         """Show associated pane (override) window."""
-        self.parent.show_pane(self, show)
+        ## Note: This might be called from a thread.
+        wx.CallAfter(self.parent.show_pane, self, show)
     
     Drawn = property(
         lambda self: self.IsDrawn(),
         lambda self,v: self.Draw(v))
     
     def IsDrawn(self):
         return any(art.get_visible() for art in self.Arts)
@@ -414,14 +415,15 @@
     def __init__(self, parent, session=None, **kwargs):
         ControlPanel.__init__(self, parent, **kwargs)
         LayerInterface.__init__(self, parent, session)
     
     ## Explicit (override) precedence
     message = LayerInterface.message
     IsShown = LayerInterface.IsShown
+    Shown = LayerInterface.Shown
     Show = LayerInterface.Show
 
 
 class Graph(GraphPlot):
     """GraphPlot (override) to better make use for graph manager
     
     Attributes:
@@ -1013,14 +1015,15 @@
             def __init__(self, parent, session=None, **kwargs):
                 cls.__init__(self, parent, **kwargs)
                 LayerInterface.__init__(self, parent, session)
             
             ## Explicit (override) precedence
             message = LayerInterface.message
             IsShown = LayerInterface.IsShown
+            Shown = LayerInterface.Shown
             Show = LayerInterface.Show
             
             ## Implicit (override) precedence
             ## cls.Init / cls.save_session / cls.load_session
         
         _Plugin.__module__ = cls.__module__ = module.__name__
         _Plugin.__name__ = cls.__name__ + str("~")
@@ -1747,15 +1750,15 @@
                     path = path[:-12]
                 session = {}
                 try:
                     plug.save_session(session)
                 except Exception:
                     traceback.print_exc()
                     print("- Failed to save session: {}".format(plug))
-                o.write("self.load_plug({!r}, session={!r})\n".format(path, session or None))
+                o.write("self.load_plug({!r}, session={})\n".format(path, session or None))
             o.write("self._mgr.LoadPerspective({!r})\n".format(self._mgr.SavePerspective()))
             
             ## set-global-unit
             o.write("self.graph.unit = {:g}\n".format(self.graph.unit))
             o.write("self.output.unit = {:g}\n".format(self.output.unit))
             
             ## stack-frame
```

## mwx/matplot2lg.py

```diff
@@ -218,18 +218,18 @@
                  'frame_shown' : [ None, self.hreplot ],
               'frame_selected' : [ None, self.hreplot ],
               'frame_modified' : [ None, self.hplot ],
             }
         }
         self.modeline.Show(0)
         
-        def destroy(evt):
+        def destroy(v):
             for graph in self.__graphs:
                 self.detach(graph)
-            evt.Skip()
+            v.Skip()
         self.Bind(wx.EVT_WINDOW_DESTROY, destroy)
     
     def clear(self):
         LinePlot.clear(self)
         
         self.__graphs = []
         self.__frame = None
@@ -437,18 +437,18 @@
                 lambda v: v.Check(self.__logicp)),
                 
             (mwx.ID_(512), "Pixel length", "Set axis-unit in pxiel base", wx.ITEM_RADIO,
                 lambda v: self.set_logic(0),
                 lambda v: v.Check(not self.__logicp)),
         ]
         
-        def destroy(evt):
+        def destroy(v):
             for graph in self.__graphs:
                 self.detach(graph)
-            evt.Skip()
+            v.Skip()
         self.Bind(wx.EVT_WINDOW_DESTROY, destroy)
     
     def clear(self):
         LinePlot.clear(self)
         
         self.__graphs = []
         self.__frame = None
```

## mwx/nutshell.py

```diff
@@ -1092,15 +1092,15 @@
     
     def on_itext_enter(self, evt):
         """Called when entering filter_text mode."""
         if not self.__itextlines:
             self.handler('quit', evt)
             return
         def _format(ln):
-            return "{:4d} {}".format(ln+1, self.GetLine(ln).rstrip())
+            return "{:4d} {}".format(ln+1, self.GetLine(ln).strip())
         self.AutoCompSetSeparator(ord('\n'))
         self.AutoCompShow(0, '\n'.join(map(_format, self.__itextlines))) # cf. gen_autocomp
         self.AutoCompSelect("{:4d}".format(self.cline+1))
         self.Bind(stc.EVT_STC_AUTOCOMP_SELECTION, self.on_itext_selection)
     
     def on_itext_exit(self, evt):
         """Called when exiting filter_text mode."""
```

## Comparing `mwxlib-0.84.1.dist-info/LICENSE` & `mwxlib-0.84.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.84.1.dist-info/METADATA` & `mwxlib-0.84.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.84.1
+Version: 0.84.2
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.84.1.dist-info/RECORD` & `mwxlib-0.84.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
-mwx/controls.py,sha256=7hnSimA3bKDgTct29l6Hqpq7BCKqCeOjZJ6JQ1xjh7I,43445
-mwx/framework.py,sha256=aL7sUwXqezgImLrtUYHhTNDGJUHGoEflOmgdfHG4wFA,73753
-mwx/graphman.py,sha256=v11sec3cS5Od__pmWecCi_ivJe65wvr-DzYYnL2Lwb0,69520
+mwx/controls.py,sha256=pD1IjgkwdvD-ebntnAH-6Jo7KY5hDq30Ne6rTE_i9fE,43499
+mwx/framework.py,sha256=jEbi33rN4VmtGvTqeXBGT6avlh3foAJf3lDl_2I0Jog,73753
+mwx/graphman.py,sha256=dJoVzwRdcXRTh-oORs0db3icxcrTgQ8zCkTGAk9PxJw,69662
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
-mwx/matplot2lg.py,sha256=h_aFij_7ksG2DXuYCaGmjtlcl122vZnwbMTv21Mprcg,27606
+mwx/matplot2lg.py,sha256=vVlBulRQDyYonI9EKfqp-3SpNbGyIJQ6ldkw6bZlalo,27598
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
-mwx/nutshell.py,sha256=SLt4Q1-2w-hoQycvneBDIVPgSJrTmP6BgYV-CH4B24g,138760
+mwx/nutshell.py,sha256=ajJBsC9o_21DuYuw5mwRGpB4GgwWT2rOjlf-DS-ntLI,138759
 mwx/utilus.py,sha256=ADA8I7qg339TJOvbrWWD91jqICWfc5C-ENFE-a7YBvU,37431
 mwx/wxmon.py,sha256=hEXto7dD5JunPf-iv2hhcwTIILLkNPlcl6wRt20_Wqc,11343
 mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=UG361QTUheO_hlSIRgkprrGUYh0IzHB8ZqOoJeeMzUs,7424
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.84.1.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.84.1.dist-info/METADATA,sha256=krEJAfNG4WtQ4Z7Nq8FtNpMJRFhzzO9pVKww7Mo0P9g,1893
-mwxlib-0.84.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.84.1.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.84.1.dist-info/RECORD,,
+mwxlib-0.84.2.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.84.2.dist-info/METADATA,sha256=N3-3F8X4LSbgWKM7bLD2fBwbh0BJk5k-mDalmt9rKZw,1893
+mwxlib-0.84.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.84.2.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.84.2.dist-info/RECORD,,
```

