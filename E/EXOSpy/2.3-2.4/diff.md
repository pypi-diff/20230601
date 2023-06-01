# Comparing `tmp/EXOSpy-2.3.tar.gz` & `tmp/EXOSpy-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EXOSpy-2.3.tar", last modified: Thu Aug 18 01:54:35 2022, max compression
+gzip compressed data, was "EXOSpy-2.4.tar", last modified: Thu Jun  1 17:16:41 2023, max compression
```

## Comparing `EXOSpy-2.3.tar` & `EXOSpy-2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2022-08-18 01:54:35.043974 EXOSpy-2.3/
--rw-r--r--   0 gcuchopa   (503) staff       (20)      274 2022-08-18 01:54:35.044115 EXOSpy-2.3/PKG-INFO
--rw-rw-r--   0 gcuchopa   (503) staff       (20)      156 2022-08-17 23:05:40.000000 EXOSpy-2.3/README.rst
--rw-rw-r--   0 gcuchopa   (503) staff       (20)      107 2022-08-18 01:54:35.044577 EXOSpy-2.3/setup.cfg
--rw-rw-r--   0 gcuchopa   (503) staff       (20)      438 2022-08-18 01:52:44.000000 EXOSpy-2.3/setup.py
-drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2022-08-18 01:54:35.039747 EXOSpy-2.3/src/
-drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2022-08-18 01:54:35.042367 EXOSpy-2.3/src/EXOSpy.egg-info/
--rw-r--r--   0 gcuchopa   (503) staff       (20)      274 2022-08-18 01:54:34.000000 EXOSpy-2.3/src/EXOSpy.egg-info/PKG-INFO
--rw-r--r--   0 gcuchopa   (503) staff       (20)      242 2022-08-18 01:54:35.000000 EXOSpy-2.3/src/EXOSpy.egg-info/SOURCES.txt
--rw-r--r--   0 gcuchopa   (503) staff       (20)        1 2022-08-18 01:54:34.000000 EXOSpy-2.3/src/EXOSpy.egg-info/dependency_links.txt
--rw-r--r--   0 gcuchopa   (503) staff       (20)       36 2022-08-18 01:54:34.000000 EXOSpy-2.3/src/EXOSpy.egg-info/requires.txt
--rw-r--r--   0 gcuchopa   (503) staff       (20)        7 2022-08-18 01:54:34.000000 EXOSpy-2.3/src/EXOSpy.egg-info/top_level.txt
-drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2022-08-18 01:54:35.042914 EXOSpy-2.3/src/exospy/
--rw-rw-r--   0 gcuchopa   (503) staff       (20)        0 2022-01-08 23:56:05.000000 EXOSpy-2.3/src/exospy/__init__.py
--rw-rw-r--   0 gcuchopa   (503) staff       (20)    39750 2022-08-18 01:51:53.000000 EXOSpy-2.3/src/exospy/exospy.py
+drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2023-06-01 17:16:41.857619 EXOSpy-2.4/
+-rw-r--r--   0 gcuchopa   (503) staff       (20)      274 2023-06-01 17:16:41.857760 EXOSpy-2.4/PKG-INFO
+-rw-rw-r--   0 gcuchopa   (503) staff       (20)      156 2022-08-17 23:05:40.000000 EXOSpy-2.4/README.rst
+-rw-rw-r--   0 gcuchopa   (503) staff       (20)      107 2023-06-01 17:16:41.858307 EXOSpy-2.4/setup.cfg
+-rw-rw-r--   0 gcuchopa   (503) staff       (20)      438 2023-06-01 17:09:51.000000 EXOSpy-2.4/setup.py
+drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2023-06-01 17:16:41.852131 EXOSpy-2.4/src/
+drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2023-06-01 17:16:41.856242 EXOSpy-2.4/src/EXOSpy.egg-info/
+-rw-r--r--   0 gcuchopa   (503) staff       (20)      274 2023-06-01 17:16:41.000000 EXOSpy-2.4/src/EXOSpy.egg-info/PKG-INFO
+-rw-r--r--   0 gcuchopa   (503) staff       (20)      242 2023-06-01 17:16:41.000000 EXOSpy-2.4/src/EXOSpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gcuchopa   (503) staff       (20)        1 2023-06-01 17:16:41.000000 EXOSpy-2.4/src/EXOSpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gcuchopa   (503) staff       (20)       36 2023-06-01 17:16:41.000000 EXOSpy-2.4/src/EXOSpy.egg-info/requires.txt
+-rw-r--r--   0 gcuchopa   (503) staff       (20)        7 2023-06-01 17:16:41.000000 EXOSpy-2.4/src/EXOSpy.egg-info/top_level.txt
+drwxr-xr-x   0 gcuchopa   (503) staff       (20)        0 2023-06-01 17:16:41.857113 EXOSpy-2.4/src/exospy/
+-rw-rw-r--   0 gcuchopa   (503) staff       (20)        0 2022-01-08 23:56:05.000000 EXOSpy-2.4/src/exospy/__init__.py
+-rw-rw-r--   0 gcuchopa   (503) staff       (20)    39745 2023-06-01 17:12:43.000000 EXOSpy-2.4/src/exospy/exospy.py
```

### Comparing `EXOSpy-2.3/src/exospy/exospy.py` & `EXOSpy-2.4/src/exospy/exospy.py`

 * *Files 0% similar despite different names*

```diff
@@ -917,15 +917,15 @@
         phi = phi + 360.0
       colat = 90.0-theta*180.0/np.pi
 
       if (r>maxRAD) or (r < minRAD):
         #print(radius)
         break
       # Calculate intensity
-      intensity = intensity + (pf*g_factor/10.0**6)*get_density(model,radius,colat*np.pi/180,phi*np.pi/180)*dl*(6371*10**5)
+      intensity = intensity + (pf*g_factor/10.0**6)*get_density(model,r,colat*np.pi/180,phi*np.pi/180)*dl*(6371*10**5)
       # Update the current position
       current_pos = current_pos + dl*r_los[i,:] #in RE
 
     # Save Intensity
     Intensity_v[i,0] = intensity
   
   return Intensity_v
```

