# Comparing `tmp/Ekidna-0.0.4.tar.gz` & `tmp/Ekidna-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ekidna-0.0.4.tar", last modified: Wed Feb 22 20:17:28 2023, max compression
+gzip compressed data, was "Ekidna-0.0.5.tar", last modified: Wed May 31 23:52:13 2023, max compression
```

## Comparing `Ekidna-0.0.4.tar` & `Ekidna-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 20:17:28.886778 Ekidna-0.0.4/
--rw-rw-rw-   0        0        0     1199 2023-02-21 21:35:28.000000 Ekidna-0.0.4/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-02-22 20:17:28.868251 Ekidna-0.0.4/Ekidna/
--rw-rw-rw-   0        0        0    12087 2023-02-22 14:22:01.000000 Ekidna-0.0.4/Ekidna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-22 20:17:28.884200 Ekidna-0.0.4/Ekidna.egg-info/
--rw-rw-rw-   0        0        0     2076 2023-02-22 20:17:28.000000 Ekidna-0.0.4/Ekidna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-02-22 20:17:28.000000 Ekidna-0.0.4/Ekidna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 20:17:28.000000 Ekidna-0.0.4/Ekidna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-22 20:17:28.000000 Ekidna-0.0.4/Ekidna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1059 2023-02-15 22:31:00.000000 Ekidna-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-02-15 22:31:00.000000 Ekidna-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2076 2023-02-22 20:17:28.885939 Ekidna-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-02-22 20:17:03.000000 Ekidna-0.0.4/README.txt
--rw-rw-rw-   0        0        0       42 2023-02-22 20:17:28.887148 Ekidna-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      734 2023-02-22 14:33:48.000000 Ekidna-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:52:13.948625 Ekidna-0.0.5/
+-rw-rw-rw-   0        0        0      466 2023-05-31 23:49:16.000000 Ekidna-0.0.5/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 23:52:13.920670 Ekidna-0.0.5/Ekidna/
+-rw-rw-rw-   0        0        0    11395 2023-05-31 23:46:41.000000 Ekidna-0.0.5/Ekidna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 23:52:13.946630 Ekidna-0.0.5/Ekidna.egg-info/
+-rw-rw-rw-   0        0        0     1347 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 23:52:13.000000 Ekidna-0.0.5/Ekidna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1059 2023-05-31 23:45:24.000000 Ekidna-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-31 23:45:24.000000 Ekidna-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6657 2023-05-31 23:49:51.000000 Ekidna-0.0.5/Module Contents.txt
+-rw-rw-rw-   0        0        0     1347 2023-05-31 23:52:13.948625 Ekidna-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-05-31 23:45:24.000000 Ekidna-0.0.5/README.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 23:52:13.949620 Ekidna-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      734 2023-05-31 23:50:24.000000 Ekidna-0.0.5/setup.py
```

### Comparing `Ekidna-0.0.4/Ekidna/__init__.py` & `Ekidna-0.0.5/Ekidna/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -180,30 +180,21 @@
         
         start = window_size*num_averages + 1
         
         for i in range(start, num_samples):
             baseline[i] = current[i]
             
             
-    baseline_fig, ax = plt.subplots(nrows = 1, ncols = 1, figsize=(12,7))
-    #plot the current values and generated baseline
-    
-    if forward:
-        ax.plot(baseline[0:num_averages*window_size], linewidth = 2, label='Baseline')
-        ax.plot(current[0:num_averages*window_size], linewidth = 2, label='Voltammogram', alpha = 0.5)
-    else:
-        ax.plot(np.flip(baseline[0:num_averages*window_size]), linewidth = 2, label='Baseline')
-        ax.plot(np.flip(np.array(current[0:num_averages*window_size])), linewidth = 2, label='Voltammogram', alpha = 0.5)
+
+
     
       
         
-    ax.set_ylabel('Current\n(A)', fontsize = 14)
-    ax.set_xlabel('Potential Sample', fontsize = 14)
-    
-    return baseline, baseline_fig
+
+    return baseline
 
 
 
 
 
 def get_groupwise_intervals(xdom, yran):
     '''
```

### Comparing `Ekidna-0.0.4/LICENSE.txt` & `Ekidna-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ekidna-0.0.4/setup.py` & `Ekidna-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='Ekidna',
-    version='0.0.4',
+    version='0.0.5',
     description='Electrochemistry data analysis tools',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='OzymandiasTheDead',
     author_email='jacob@ekidnasensing.com',
     license='MIT',
     classifiers=classifiers,
```

