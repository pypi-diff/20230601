# Comparing `tmp/alive-progress-3.1.3.tar.gz` & `tmp/alive-progress-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alive-progress-3.1.3.tar", last modified: Fri May 26 03:44:59 2023, max compression
+gzip compressed data, was "dist/alive-progress-3.1.4.tar", last modified: Thu Jun  1 01:16:20 2023, max compression
```

## Comparing `alive-progress-3.1.3.tar` & `alive-progress-3.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/
--rw-r--r--   0 rogerio    (501) staff       (20)     1084 2019-08-05 05:55:53.000000 alive-progress-3.1.3/LICENSE
--rw-r--r--   0 rogerio    (501) staff       (20)    75919 2023-05-26 03:44:59.000000 alive-progress-3.1.3/PKG-INFO
--rw-r--r--   0 rogerio    (501) staff       (20)    67113 2023-05-26 03:41:18.000000 alive-progress-3.1.3/README.md
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/
--rw-r--r--   0 rogerio    (501) staff       (20)      417 2023-05-26 03:40:31.000000 alive-progress-3.1.3/alive_progress/__init__.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/animations/
--rw-r--r--   0 rogerio    (501) staff       (20)      481 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/animations/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     9721 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/animations/bars.py
--rw-r--r--   0 rogerio    (501) staff       (20)    13834 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/animations/spinner_compiler.py
--rw-r--r--   0 rogerio    (501) staff       (20)    11443 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/animations/spinners.py
--rw-r--r--   0 rogerio    (501) staff       (20)     4723 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/animations/utils.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/core/
--rw-r--r--   0 rogerio    (501) staff       (20)        0 2020-07-28 14:16:28.000000 alive-progress-3.1.3/alive_progress/core/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1351 2022-02-02 06:03:46.000000 alive-progress-3.1.3/alive_progress/core/calibration.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8876 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/core/configuration.py
--rw-r--r--   0 rogerio    (501) staff       (20)     5627 2023-05-26 03:43:17.000000 alive-progress-3.1.3/alive_progress/core/hook_manager.py
--rw-r--r--   0 rogerio    (501) staff       (20)    23674 2023-05-26 03:42:11.000000 alive-progress-3.1.3/alive_progress/core/progress.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/styles/
--rw-r--r--   0 rogerio    (501) staff       (20)      614 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/styles/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)    11233 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/styles/exhibit.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8454 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/styles/internal.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/tools/
--rw-r--r--   0 rogerio    (501) staff       (20)       58 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     3002 2022-03-22 04:49:57.000000 alive-progress-3.1.3/alive_progress/tools/demo.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1024 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/repl.py
--rw-r--r--   0 rogerio    (501) staff       (20)     2717 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/tools/sampling.py
--rw-r--r--   0 rogerio    (501) staff       (20)     6634 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/unicode_breaks.py
--rw-r--r--   0 rogerio    (501) staff       (20)      399 2021-08-26 23:38:44.000000 alive-progress-3.1.3/alive_progress/tools/utils.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/utils/
--rw-r--r--   0 rogerio    (501) staff       (20)        0 2022-10-31 01:30:29.000000 alive-progress-3.1.3/alive_progress/utils/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)     8811 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/utils/cells.py
--rw-r--r--   0 rogerio    (501) staff       (20)     2308 2022-02-11 05:29:12.000000 alive-progress-3.1.3/alive_progress/utils/colors.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress/utils/terminal/
--rw-r--r--   0 rogerio    (501) staff       (20)     2100 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/__init__.py
--rw-r--r--   0 rogerio    (501) staff       (20)      747 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/jupyter.py
--rw-r--r--   0 rogerio    (501) staff       (20)      418 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/utils/terminal/non_tty.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1284 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/tty.py
--rw-r--r--   0 rogerio    (501) staff       (20)      550 2023-03-24 02:50:30.000000 alive-progress-3.1.3/alive_progress/utils/terminal/void.py
--rw-r--r--   0 rogerio    (501) staff       (20)     1411 2022-12-22 05:23:53.000000 alive-progress-3.1.3/alive_progress/utils/timing.py
-drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/
--rw-r--r--   0 rogerio    (501) staff       (20)    75919 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/PKG-INFO
--rw-r--r--   0 rogerio    (501) staff       (20)     1223 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/SOURCES.txt
--rw-r--r--   0 rogerio    (501) staff       (20)        1 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/dependency_links.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       34 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/requires.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       15 2023-05-26 03:44:59.000000 alive-progress-3.1.3/alive_progress.egg-info/top_level.txt
--rw-r--r--   0 rogerio    (501) staff       (20)       38 2023-05-26 03:44:59.000000 alive-progress-3.1.3/setup.cfg
--rw-r--r--   0 rogerio    (501) staff       (20)     2306 2022-12-22 05:23:53.000000 alive-progress-3.1.3/setup.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/
+-rw-r--r--   0 rogerio    (501) staff       (20)     1084 2019-08-05 05:55:53.000000 alive-progress-3.1.4/LICENSE
+-rw-r--r--   0 rogerio    (501) staff       (20)    75999 2023-06-01 01:16:20.000000 alive-progress-3.1.4/PKG-INFO
+-rw-r--r--   0 rogerio    (501) staff       (20)    67185 2023-06-01 01:11:03.000000 alive-progress-3.1.4/README.md
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress/
+-rw-r--r--   0 rogerio    (501) staff       (20)      417 2023-06-01 01:11:03.000000 alive-progress-3.1.4/alive_progress/__init__.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress/animations/
+-rw-r--r--   0 rogerio    (501) staff       (20)      481 2021-08-26 23:38:44.000000 alive-progress-3.1.4/alive_progress/animations/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     9721 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/animations/bars.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    13834 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/animations/spinner_compiler.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    11443 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/animations/spinners.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     4723 2021-08-26 23:38:44.000000 alive-progress-3.1.4/alive_progress/animations/utils.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress/core/
+-rw-r--r--   0 rogerio    (501) staff       (20)        0 2020-07-28 14:16:28.000000 alive-progress-3.1.4/alive_progress/core/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1351 2022-02-02 06:03:46.000000 alive-progress-3.1.4/alive_progress/core/calibration.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8822 2023-06-01 01:14:03.000000 alive-progress-3.1.4/alive_progress/core/configuration.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     5627 2023-05-26 03:43:17.000000 alive-progress-3.1.4/alive_progress/core/hook_manager.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    23674 2023-05-26 03:42:11.000000 alive-progress-3.1.4/alive_progress/core/progress.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress/styles/
+-rw-r--r--   0 rogerio    (501) staff       (20)      614 2021-08-26 23:38:44.000000 alive-progress-3.1.4/alive_progress/styles/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)    11233 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/styles/exhibit.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8454 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/styles/internal.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress/tools/
+-rw-r--r--   0 rogerio    (501) staff       (20)       58 2021-08-26 23:38:44.000000 alive-progress-3.1.4/alive_progress/tools/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     3002 2022-03-22 04:49:57.000000 alive-progress-3.1.4/alive_progress/tools/demo.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1024 2021-08-26 23:38:44.000000 alive-progress-3.1.4/alive_progress/tools/repl.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     2717 2022-12-22 05:23:53.000000 alive-progress-3.1.4/alive_progress/tools/sampling.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     6634 2021-08-26 23:38:44.000000 alive-progress-3.1.4/alive_progress/tools/unicode_breaks.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      399 2021-08-26 23:38:44.000000 alive-progress-3.1.4/alive_progress/tools/utils.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress/utils/
+-rw-r--r--   0 rogerio    (501) staff       (20)      131 2023-06-01 00:57:44.000000 alive-progress-3.1.4/alive_progress/utils/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     8737 2023-06-01 00:58:10.000000 alive-progress-3.1.4/alive_progress/utils/cells.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     2308 2022-02-11 05:29:12.000000 alive-progress-3.1.4/alive_progress/utils/colors.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress/utils/terminal/
+-rw-r--r--   0 rogerio    (501) staff       (20)     2100 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/utils/terminal/__init__.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      747 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/utils/terminal/jupyter.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      418 2022-12-22 05:23:53.000000 alive-progress-3.1.4/alive_progress/utils/terminal/non_tty.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1284 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/utils/terminal/tty.py
+-rw-r--r--   0 rogerio    (501) staff       (20)      550 2023-03-24 02:50:30.000000 alive-progress-3.1.4/alive_progress/utils/terminal/void.py
+-rw-r--r--   0 rogerio    (501) staff       (20)     1411 2022-12-22 05:23:53.000000 alive-progress-3.1.4/alive_progress/utils/timing.py
+drwxr-xr-x   0 rogerio    (501) staff       (20)        0 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress.egg-info/
+-rw-r--r--   0 rogerio    (501) staff       (20)    75999 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress.egg-info/PKG-INFO
+-rw-r--r--   0 rogerio    (501) staff       (20)     1223 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress.egg-info/SOURCES.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)        1 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress.egg-info/dependency_links.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       34 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress.egg-info/requires.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       15 2023-06-01 01:16:20.000000 alive-progress-3.1.4/alive_progress.egg-info/top_level.txt
+-rw-r--r--   0 rogerio    (501) staff       (20)       38 2023-06-01 01:16:20.000000 alive-progress-3.1.4/setup.cfg
+-rw-r--r--   0 rogerio    (501) staff       (20)     2306 2022-12-22 05:23:53.000000 alive-progress-3.1.4/setup.py
```

### Comparing `alive-progress-3.1.3/LICENSE` & `alive-progress-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/PKG-INFO` & `alive-progress-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alive-progress
-Version: 3.1.3
+Version: 3.1.4
 Summary: A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
 Home-page: https://github.com/rsalmei/alive-progress
 Author: Rogério Sampaio de Almeida
 Author-email: rsalmei@gmail.com
 License: MIT
 Description: [<img align="right" src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/rsalmei)
         [<img align="right" alt="Donate with PayPal button" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://www.paypal.com/donate?business=6SWSHEB5ZNS5N&no_recurring=0&item_name=I%27m+the+author+of+alive-progress%2C+clearly+and+about-time.+Thank+you+for+appreciating+my+work%21&currency_code=USD)
@@ -896,17 +896,18 @@
         </details>
         
         <details>
         <summary>Changelog highlights</summary>
         
         <br>Complete [here](https://github.com/rsalmei/alive-progress/blob/main/CHANGELOG.md).
         
-        - 3.1.3: better error handling of invalid alive_it calls, better error message when detecting nested uses of alive_progress
+        - 3.1.4: support spaces at the start and end of titles and units
+        - 3.1.3: better error handling of invalid `alive_it` calls, detect nested uses of alive_progress and throw a clearer error message
         - 3.1.2: fix some exotic ANSI Escape Codes not being printed (OSC)
-        - 3.1.1: support for printing ANSI Escape Codes like set console title, typing annotations in `alive_it`
+        - 3.1.1: support for printing ANSI Escape Codes without extra newlines, typing annotations in `alive_it`
         - 3.1.0: new resuming computations support with `skipped` items, new `max_cols` config setting for jupyter, fix fetching the size of the terminal when using stderr, officially supports Python 3.11
         - 3.0.1: fix for logging streams that extend StreamHandler but doesn't allow changing streams
         - 3.0.0: units support with automatic and configurable scaling and precision, automatic stats scaling for slow throughputs, support for using `sys.stderr` and other files instead of `sys.stdout`, smoothed out the rate estimation, more queries into the currently running widgets' data, help system in configuration errors
         - 2.4.1: fix a crash when dual-line and disabled are set
         - 2.4.0: support dual line text mode; finalize function parameter in alive_it; improve logging support, detecting customized ones
         - 2.3.1: introduce ctrl_c config param; print the final receipt even when interrupted
         - 2.3.0: customizable `monitor`, `elapsed`, and `stats` core widgets, new `monitor_end`, `elapsed_end`, and `stats_end` core widgets, better support for CTRL+C, which makes `alive_bar` stop prematurely
```

### Comparing `alive-progress-3.1.3/README.md` & `alive-progress-3.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -888,17 +888,18 @@
 </details>
 
 <details>
 <summary>Changelog highlights</summary>
 
 <br>Complete [here](https://github.com/rsalmei/alive-progress/blob/main/CHANGELOG.md).
 
-- 3.1.3: better error handling of invalid alive_it calls, better error message when detecting nested uses of alive_progress
+- 3.1.4: support spaces at the start and end of titles and units
+- 3.1.3: better error handling of invalid `alive_it` calls, detect nested uses of alive_progress and throw a clearer error message
 - 3.1.2: fix some exotic ANSI Escape Codes not being printed (OSC)
-- 3.1.1: support for printing ANSI Escape Codes like set console title, typing annotations in `alive_it`
+- 3.1.1: support for printing ANSI Escape Codes without extra newlines, typing annotations in `alive_it`
 - 3.1.0: new resuming computations support with `skipped` items, new `max_cols` config setting for jupyter, fix fetching the size of the terminal when using stderr, officially supports Python 3.11
 - 3.0.1: fix for logging streams that extend StreamHandler but doesn't allow changing streams
 - 3.0.0: units support with automatic and configurable scaling and precision, automatic stats scaling for slow throughputs, support for using `sys.stderr` and other files instead of `sys.stdout`, smoothed out the rate estimation, more queries into the currently running widgets' data, help system in configuration errors
 - 2.4.1: fix a crash when dual-line and disabled are set
 - 2.4.0: support dual line text mode; finalize function parameter in alive_it; improve logging support, detecting customized ones
 - 2.3.1: introduce ctrl_c config param; print the final receipt even when interrupted
 - 2.3.0: customizable `monitor`, `elapsed`, and `stats` core widgets, new `monitor_end`, `elapsed_end`, and `stats_end` core widgets, better support for CTRL+C, which makes `alive_bar` stop prematurely
```

### Comparing `alive-progress-3.1.3/alive_progress/animations/bars.py` & `alive-progress-3.1.4/alive_progress/animations/bars.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/animations/spinner_compiler.py` & `alive-progress-3.1.4/alive_progress/animations/spinner_compiler.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/animations/spinners.py` & `alive-progress-3.1.4/alive_progress/animations/spinners.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/animations/utils.py` & `alive-progress-3.1.4/alive_progress/animations/utils.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/core/calibration.py` & `alive-progress-3.1.4/alive_progress/core/calibration.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/core/configuration.py` & `alive-progress-3.1.4/alive_progress/core/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 This module must always be importable, even without the required libs for install!
 It's because I import metadata from main init, directly in setup.py, which imports this.
 """
 import os
-import re
 import sys
 from collections import namedtuple
 from string import Formatter
 from types import FunctionType
 
+from ..utils import sanitize
+
 ERROR = object()  # represents a config value not accepted.
-PATTERN_SANITIZE = re.compile(r'[\r\n]+')
 
 
 def _spinner_input_factory(default):
     from ..animations import spinner_compiler
     from ..styles.internal import SPINNERS
     return __style_input(SPINNERS, spinner_compiler, 'spinner_compiler_dispatcher_factory', default)
 
@@ -91,15 +91,15 @@
         return None if x is None else bool(x)
 
     return _input
 
 
 def _text_input_factory():
     def _input(x):
-        return None if x is None else ' '.join(PATTERN_SANITIZE.split(str(x))).strip()
+        return None if x is None else sanitize(str(x))
 
     return _input
 
 
 def _options_input_factory(valid: tuple, alias: dict):
     def _input(x):
         x = alias.get(x, x)
```

### Comparing `alive-progress-3.1.3/alive_progress/core/hook_manager.py` & `alive-progress-3.1.4/alive_progress/core/hook_manager.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/core/progress.py` & `alive-progress-3.1.4/alive_progress/core/progress.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/styles/__init__.py` & `alive-progress-3.1.4/alive_progress/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/styles/exhibit.py` & `alive-progress-3.1.4/alive_progress/styles/exhibit.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/styles/internal.py` & `alive-progress-3.1.4/alive_progress/styles/internal.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/tools/demo.py` & `alive-progress-3.1.4/alive_progress/tools/demo.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/tools/repl.py` & `alive-progress-3.1.4/alive_progress/tools/repl.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/tools/sampling.py` & `alive-progress-3.1.4/alive_progress/tools/sampling.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/tools/unicode_breaks.py` & `alive-progress-3.1.4/alive_progress/tools/unicode_breaks.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/utils/cells.py` & `alive-progress-3.1.4/alive_progress/utils/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,18 @@
     title, exhibit, and of course the alive_bar rendering itself... All of them needed to learn this
     new architecture: mainly change ordinary strings into tuples of cells (marked graphemes)...
 14. And finally... Profit!!! Only no, this project only feels my soul, not my pocket...
     But what a ride! 😅
 
 """
 
-import re
 import unicodedata
 
-PATTERN_SANITIZE = re.compile(r'[\r\n]+')
+from . import sanitize
+
 VS_15 = '\ufe0e'
 
 
 def print_cells(fragments, cols, term, last_line_len=0):
     """Print a tuple of fragments of tuples of cells on the terminal, until a given number of
     cols is achieved, slicing over cells when needed.
 
@@ -155,16 +155,15 @@
 
     start = (' ',) if chars[0] is None else ()
     end = (' ',) if chars[-1] is not None and is_wide(chars[-1]) else ()
     return (*start, *chars[bool(start):-1 if end else None], *end)  # noqa
 
 
 def to_cells(text):
-    text = ' '.join(PATTERN_SANITIZE.split(text or ''))
-    return mark_graphemes(split_graphemes(text))
+    return mark_graphemes(split_graphemes(sanitize(text)))
 
 
 def split_graphemes(text):
     from grapheme import graphemes
     return tuple(graphemes(text))
```

### Comparing `alive-progress-3.1.3/alive_progress/utils/colors.py` & `alive-progress-3.1.4/alive_progress/utils/colors.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/utils/terminal/__init__.py` & `alive-progress-3.1.4/alive_progress/utils/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/utils/terminal/jupyter.py` & `alive-progress-3.1.4/alive_progress/utils/terminal/jupyter.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/utils/terminal/tty.py` & `alive-progress-3.1.4/alive_progress/utils/terminal/tty.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/utils/terminal/void.py` & `alive-progress-3.1.4/alive_progress/utils/terminal/void.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress/utils/timing.py` & `alive-progress-3.1.4/alive_progress/utils/timing.py`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/alive_progress.egg-info/PKG-INFO` & `alive-progress-3.1.4/alive_progress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alive-progress
-Version: 3.1.3
+Version: 3.1.4
 Summary: A new kind of Progress Bar, with real-time throughput, ETA, and very cool animations!
 Home-page: https://github.com/rsalmei/alive-progress
 Author: Rogério Sampaio de Almeida
 Author-email: rsalmei@gmail.com
 License: MIT
 Description: [<img align="right" src="https://cdn.buymeacoffee.com/buttons/default-orange.png" width="217px" height="51x">](https://www.buymeacoffee.com/rsalmei)
         [<img align="right" alt="Donate with PayPal button" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif">](https://www.paypal.com/donate?business=6SWSHEB5ZNS5N&no_recurring=0&item_name=I%27m+the+author+of+alive-progress%2C+clearly+and+about-time.+Thank+you+for+appreciating+my+work%21&currency_code=USD)
@@ -896,17 +896,18 @@
         </details>
         
         <details>
         <summary>Changelog highlights</summary>
         
         <br>Complete [here](https://github.com/rsalmei/alive-progress/blob/main/CHANGELOG.md).
         
-        - 3.1.3: better error handling of invalid alive_it calls, better error message when detecting nested uses of alive_progress
+        - 3.1.4: support spaces at the start and end of titles and units
+        - 3.1.3: better error handling of invalid `alive_it` calls, detect nested uses of alive_progress and throw a clearer error message
         - 3.1.2: fix some exotic ANSI Escape Codes not being printed (OSC)
-        - 3.1.1: support for printing ANSI Escape Codes like set console title, typing annotations in `alive_it`
+        - 3.1.1: support for printing ANSI Escape Codes without extra newlines, typing annotations in `alive_it`
         - 3.1.0: new resuming computations support with `skipped` items, new `max_cols` config setting for jupyter, fix fetching the size of the terminal when using stderr, officially supports Python 3.11
         - 3.0.1: fix for logging streams that extend StreamHandler but doesn't allow changing streams
         - 3.0.0: units support with automatic and configurable scaling and precision, automatic stats scaling for slow throughputs, support for using `sys.stderr` and other files instead of `sys.stdout`, smoothed out the rate estimation, more queries into the currently running widgets' data, help system in configuration errors
         - 2.4.1: fix a crash when dual-line and disabled are set
         - 2.4.0: support dual line text mode; finalize function parameter in alive_it; improve logging support, detecting customized ones
         - 2.3.1: introduce ctrl_c config param; print the final receipt even when interrupted
         - 2.3.0: customizable `monitor`, `elapsed`, and `stats` core widgets, new `monitor_end`, `elapsed_end`, and `stats_end` core widgets, better support for CTRL+C, which makes `alive_bar` stop prematurely
```

### Comparing `alive-progress-3.1.3/alive_progress.egg-info/SOURCES.txt` & `alive-progress-3.1.4/alive_progress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alive-progress-3.1.3/setup.py` & `alive-progress-3.1.4/setup.py`

 * *Files identical despite different names*

