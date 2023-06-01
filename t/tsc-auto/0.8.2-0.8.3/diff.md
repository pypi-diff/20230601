# Comparing `tmp/tsc-auto-0.8.2.tar.gz` & `tmp/tsc-auto-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-auto-0.8.2.tar", last modified: Fri Dec 24 15:31:51 2021, max compression
+gzip compressed data, was "tsc-auto-0.8.3.tar", last modified: Fri Dec 24 15:42:26 2021, max compression
```

## Comparing `tsc-auto-0.8.2.tar` & `tsc-auto-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 15:31:51.109538 tsc-auto-0.8.2/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2021-12-03 07:10:12.000000 tsc-auto-0.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2021-12-03 09:11:46.000000 tsc-auto-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1569 2021-12-24 15:31:51.109538 tsc-auto-0.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-24 15:31:51.109538 tsc-auto-0.8.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1089 2021-12-24 15:31:37.000000 tsc-auto-0.8.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 15:31:51.105538 tsc-auto-0.8.2/tsc_auto/
--rwxrwxrwx   0 root         (0) root         (0)      202 2021-12-24 09:05:33.000000 tsc-auto-0.8.2/tsc_auto/__init__.py
--rw-r--r--   0 root         (0) root         (0)      485 2021-12-03 09:08:45.000000 tsc-auto-0.8.2/tsc_auto/auto.py
--rwxrwxrwx   0 root         (0) root         (0)     6911 2021-12-24 09:00:02.000000 tsc-auto-0.8.2/tsc_auto/auto.sh
--rw-r--r--   0 root         (0) root         (0)      358 2021-12-03 09:12:53.000000 tsc-auto-0.8.2/tsc_auto/info.py
--rw-r--r--   0 root         (0) root         (0)    12451 2021-12-24 09:10:55.000000 tsc-auto-0.8.2/tsc_auto/kill.py
--rw-r--r--   0 root         (0) root         (0)     6696 2021-12-03 09:13:23.000000 tsc-auto-0.8.2/tsc_auto/query.py
--rw-r--r--   0 root         (0) root         (0)     5561 2021-12-24 15:31:15.000000 tsc-auto-0.8.2/tsc_auto/set_gpu.py
--rw-r--r--   0 root         (0) root         (0)     3390 2021-12-03 09:15:56.000000 tsc-auto-0.8.2/tsc_auto/srun.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 15:31:51.105538 tsc-auto-0.8.2/tsc_auto.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1569 2021-12-24 15:31:51.000000 tsc-auto-0.8.2/tsc_auto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      335 2021-12-24 15:31:51.000000 tsc-auto-0.8.2/tsc_auto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-24 15:31:51.000000 tsc-auto-0.8.2/tsc_auto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2021-12-24 15:31:51.000000 tsc-auto-0.8.2/tsc_auto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2021-12-24 15:31:51.000000 tsc-auto-0.8.2/tsc_auto.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 15:42:26.874760 tsc-auto-0.8.3/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2021-12-03 07:10:12.000000 tsc-auto-0.8.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2021-12-03 09:11:46.000000 tsc-auto-0.8.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1569 2021-12-24 15:42:26.874760 tsc-auto-0.8.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2021-12-24 15:42:26.874760 tsc-auto-0.8.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2021-12-24 15:41:57.000000 tsc-auto-0.8.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 15:42:26.874760 tsc-auto-0.8.3/tsc_auto/
+-rwxrwxrwx   0 root         (0) root         (0)      202 2021-12-24 09:05:33.000000 tsc-auto-0.8.3/tsc_auto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      485 2021-12-03 09:08:45.000000 tsc-auto-0.8.3/tsc_auto/auto.py
+-rwxrwxrwx   0 root         (0) root         (0)     6911 2021-12-24 09:00:02.000000 tsc-auto-0.8.3/tsc_auto/auto.sh
+-rw-r--r--   0 root         (0) root         (0)      358 2021-12-03 09:12:53.000000 tsc-auto-0.8.3/tsc_auto/info.py
+-rw-r--r--   0 root         (0) root         (0)    12451 2021-12-24 09:10:55.000000 tsc-auto-0.8.3/tsc_auto/kill.py
+-rw-r--r--   0 root         (0) root         (0)     6696 2021-12-03 09:13:23.000000 tsc-auto-0.8.3/tsc_auto/query.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2021-12-24 15:41:38.000000 tsc-auto-0.8.3/tsc_auto/set_gpu.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2021-12-03 09:15:56.000000 tsc-auto-0.8.3/tsc_auto/srun.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-24 15:42:26.874760 tsc-auto-0.8.3/tsc_auto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1569 2021-12-24 15:42:26.000000 tsc-auto-0.8.3/tsc_auto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      335 2021-12-24 15:42:26.000000 tsc-auto-0.8.3/tsc_auto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-24 15:42:26.000000 tsc-auto-0.8.3/tsc_auto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2021-12-24 15:42:26.000000 tsc-auto-0.8.3/tsc_auto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2021-12-24 15:42:26.000000 tsc-auto-0.8.3/tsc_auto.egg-info/top_level.txt
```

### Comparing `tsc-auto-0.8.2/LICENSE` & `tsc-auto-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-auto-0.8.2/PKG-INFO` & `tsc-auto-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-auto
-Version: 0.8.2
+Version: 0.8.3
 Summary: Auto selector for GPU and CUDA, support the detection of tensorflow or torch
 Home-page: https://github.com/aitsc/tsc-auto
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `tsc-auto-0.8.2/setup.py` & `tsc-auto-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = '教程: https://github.com/aitsc/tsc-auto'
 
 setup(
     name='tsc-auto',
-    version='0.8.2',
+    version='0.8.3',
     description="Auto selector for GPU and CUDA, support the detection of tensorflow or torch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tanshicheng',
     license='GPLv3',
     url='https://github.com/aitsc/tsc-auto',
     keywords='tools',
```

### Comparing `tsc-auto-0.8.2/tsc_auto/auto.sh` & `tsc-auto-0.8.3/tsc_auto/auto.sh`

 * *Files identical despite different names*

### Comparing `tsc-auto-0.8.2/tsc_auto/kill.py` & `tsc-auto-0.8.3/tsc_auto/kill.py`

 * *Files identical despite different names*

### Comparing `tsc-auto-0.8.2/tsc_auto/query.py` & `tsc-auto-0.8.3/tsc_auto/query.py`

 * *Files identical despite different names*

### Comparing `tsc-auto-0.8.2/tsc_auto/set_gpu.py` & `tsc-auto-0.8.3/tsc_auto/set_gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     if status == 0:
         if showAllGpu:
             print(result)
         r = re.findall(r'(?<=[|/])[\s\d]+?(?=MiB)', result)
         all_gpu_mem = [int(r[i + 1]) for i in range(0, len(r), 2)]
         r = [int(r[i + 1]) - int(r[i]) for i in range(0, len(r), 2)]
         w = [i.replace(' ', '') for i in re.findall(w_re, result)]
-        gpu_usage = [int(re.search(r'(?<= )[0-9.]+?(?=[%])', i).group()) for i in result.split('\n') if re.search(w_re, i)]
+        gpu_usage = [int(re.search(r'(?<= )[0-9.]+?(?=%)', i.split('MiB', 1)[1]).group())
+                     for i in result.split('\n') if re.search(w_re, i)]
         i_m = [(i, j) for i, j in enumerate(r)]
         if i_m:
             i_m = sorted(i_m, key=lambda t: t[1])
             gpu = i_m[-1][0]
             ext_gpu_mem = i_m[-1][1]
         if w:
             power = w[gpu]
```

### Comparing `tsc-auto-0.8.2/tsc_auto/srun.sh` & `tsc-auto-0.8.3/tsc_auto/srun.sh`

 * *Files identical despite different names*

### Comparing `tsc-auto-0.8.2/tsc_auto.egg-info/PKG-INFO` & `tsc-auto-0.8.3/tsc_auto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-auto
-Version: 0.8.2
+Version: 0.8.3
 Summary: Auto selector for GPU and CUDA, support the detection of tensorflow or torch
 Home-page: https://github.com/aitsc/tsc-auto
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

