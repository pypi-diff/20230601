# Comparing `tmp/rqrisk-1.0.6.tar.gz` & `tmp/rqrisk-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqrisk/rqrisk/dist/.tmp-bhm7ww4x/rqrisk-1.0.6.tar", last modified: Wed Mar  1 08:00:34 2023, max compression
+gzip compressed data, was "/home/runner/work/rqrisk/rqrisk/dist/.tmp-vc2g7udk/rqrisk-1.0.7.tar", last modified: Thu Jun  1 02:33:04 2023, max compression
```

## Comparing `rqrisk-1.0.6.tar` & `rqrisk-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:00:34.000000 rqrisk-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-01 08:00:22.000000 rqrisk-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-01 08:00:22.000000 rqrisk-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-01 08:00:34.000000 rqrisk-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 08:00:22.000000 rqrisk-1.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-01 08:00:22.000000 rqrisk-1.0.6/rqrisk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-03-01 08:00:22.000000 rqrisk-1.0.6/rqrisk/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-03-01 08:00:22.000000 rqrisk-1.0.6/rqrisk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-01 08:00:34.000000 rqrisk-1.0.6/rqrisk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-01 08:00:34.000000 rqrisk-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-01 08:00:22.000000 rqrisk-1.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    79920 2023-03-01 08:00:22.000000 rqrisk-1.0.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:33:04.000000 rqrisk-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-01 02:32:55.000000 rqrisk-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 02:32:55.000000 rqrisk-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 02:33:04.000000 rqrisk-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:32:55.000000 rqrisk-1.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-01 02:32:55.000000 rqrisk-1.0.7/rqrisk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-06-01 02:32:55.000000 rqrisk-1.0.7/rqrisk/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-01 02:32:55.000000 rqrisk-1.0.7/rqrisk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 02:33:04.000000 rqrisk-1.0.7/rqrisk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 02:33:04.000000 rqrisk-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-01 02:32:55.000000 rqrisk-1.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79849 2023-06-01 02:32:55.000000 rqrisk-1.0.7/versioneer.py
```

### Comparing `rqrisk-1.0.6/LICENSE.txt` & `rqrisk-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rqrisk-1.0.6/rqrisk/risk.py` & `rqrisk-1.0.7/rqrisk/risk.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,23 +175,31 @@
     @indicator_property()
     def calmar(self):
         if np.isclose(self.max_drawdown, 0):
             return np.inf * np.sign(self.annual_return)
         else:
             return self.annual_return / self.max_drawdown
 
+    @indicator_property(min_period_count=1)
+    def _excess_return_rate(self):
+        return np.expm1(np.log1p(self._active_returns).sum())
+
     @deprecate_property
     def excess_return_rate(self):
         # activate return rate
-        return np.expm1(np.log1p(self._active_returns).sum())
+        return self._excess_return_rate
 
     @deprecate_property
     def excess_annual_return(self):
+        return self._excess_annual_return
+
+    @indicator_property(min_period_count=1)
+    def _excess_annual_return(self):
         # active annual return
-        return (1 + self.excess_return_rate) ** (self._annual_factor / self.period_count) - 1
+        return (1 + self._excess_return_rate) ** safe_div(self._annual_factor, self.period_count) - 1
 
     @indicator_property(min_period_count=2, value_when_pc_not_satisfied=0.)
     def excess_volatility(self):
         # volatility of active returns
         return self._active_returns.std(ddof=1)
 
     @indicator_property()
```

### Comparing `rqrisk-1.0.6/rqrisk/utils.py` & `rqrisk-1.0.7/rqrisk/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、
 #         本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，
 #         否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 import numpy as np
-import logging
-
-
-logger = logging.getLogger()
+import warnings
 
 
 class IndicatorProperty:
     pass
 
 
 def indicator_property(min_period_count=None, value_when_pc_not_satisfied=np.nan):
@@ -84,12 +81,12 @@
     return dividend / divisor
 
 
 def deprecate_property(func):
 
     @property
     def inner(self):
-        logger.warning("\"{}\" is deprecate.".format(func.__name__))
+        warnings.warn("'{}' is deprecate.".format(func.__name__))
         return func(self)
 
     return inner
```

### Comparing `rqrisk-1.0.6/setup.py` & `rqrisk-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `rqrisk-1.0.6/versioneer.py` & `rqrisk-1.0.7/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1390,31 +1390,31 @@
             if parsed_working.base_version == parsed_tag.base_version:
                 if not parsed_tag.is_postrelease:
                     raise Exception("Only post release tag allowed, tag %s" % tag)
                 if parsed_tag._version.post[0] != "post":
                     raise Exception("Only post release tag allowed, tag %s" % tag)
                 if pieces["distance"] > 0:
                     rendered += ".post%d" % (parsed_tag._version.post[1] + 1)
-                    rendered += ".dev%d-g%s" % (pieces["distance"], pieces["short"])
+                    rendered += ".dev%d" % pieces["distance"]
                 elif pieces["distance"] == 0:
                     rendered += ".post%d" % parsed_tag._version.post[1]
                 if pieces["dirty"]:
                     rendered += ".dirty"
             else:
                 raise Exception("Developing version can not go back in time: %s < %s" % (working, tag))
         # 如果最近的tag是正式版tag，那么就是在开发该系列的.post1
         elif parsed_working == parsed_tag:
             if pieces["distance"] > 0:
-                rendered += ".post1.dev%d-g%s" % (pieces["distance"], pieces["short"])
+                rendered += ".post1.dev%d" % pieces["distance"]
             if pieces["dirty"]:
                 rendered += ".dirty"
         # 如果正在开发到是一个新的系列，那么就从该系列的.dev0开始
         else:
             if pieces["distance"] >= 0:
-                rendered += ".dev%d-g%s"  % (pieces["distance"], pieces["short"])
+                rendered += ".dev%d" % pieces["distance"]
 
             if pieces["dirty"]:
                 rendered += ".dirty"
     # 没有最近的tag等价于正在开发到是一个新的系列，那么就从该系列的.dev0开始
     else:
         if pieces["distance"] >= 0:
             rendered += ".dev%d" % pieces["distance"]
@@ -1424,15 +1424,15 @@
 
     tracking_branch = git_tracking_branch()
     # # 如果是dev和master分支或者hotfix分支来的，或者是一个tag，那就用pep440的版本号，否则带上git commit id
     if tracking_branch in ["origin/develop", "origin/master"] or tracking_branch.startswith("origin/hotfix/") or pieces[
         "distance"] == 0:
         return rendered
 
-    rendered += ".g%s" % pieces["short"]
+    rendered += "+%s" % pieces["short"]
     return rendered
 
 
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
```

