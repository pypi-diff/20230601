# Comparing `tmp/pisoundtrack-0.2.3.tar.gz` & `tmp/pisoundtrack-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisoundtrack-0.2.3.tar", last modified: Thu Jun  1 13:10:00 2023, max compression
+gzip compressed data, was "pisoundtrack-0.2.4.tar", last modified: Thu Jun  1 14:32:30 2023, max compression
```

## Comparing `pisoundtrack-0.2.3.tar` & `pisoundtrack-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:10:00.670876 pisoundtrack-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 13:09:48.000000 pisoundtrack-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 13:10:00.670876 pisoundtrack-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 13:09:48.000000 pisoundtrack-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:10:00.670876 pisoundtrack-0.2.3/pisoundtrack/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 13:09:48.000000 pisoundtrack-0.2.3/pisoundtrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 13:09:48.000000 pisoundtrack-0.2.3/pisoundtrack/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-01 13:09:48.000000 pisoundtrack-0.2.3/pisoundtrack/soundtrack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:10:00.670876 pisoundtrack-0.2.3/pisoundtrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 13:10:00.000000 pisoundtrack-0.2.3/pisoundtrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-01 13:10:00.000000 pisoundtrack-0.2.3/pisoundtrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:10:00.000000 pisoundtrack-0.2.3/pisoundtrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 13:10:00.000000 pisoundtrack-0.2.3/pisoundtrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 13:10:00.000000 pisoundtrack-0.2.3/pisoundtrack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:10:00.670876 pisoundtrack-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-01 13:09:48.000000 pisoundtrack-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:30.834955 pisoundtrack-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 14:32:30.834955 pisoundtrack-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:30.830953 pisoundtrack-0.2.4/pisoundtrack/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/pisoundtrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/pisoundtrack/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/pisoundtrack/soundtrack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:32:30.830953 pisoundtrack-0.2.4/pisoundtrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 14:32:30.000000 pisoundtrack-0.2.4/pisoundtrack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:32:30.834955 pisoundtrack-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-01 14:32:19.000000 pisoundtrack-0.2.4/setup.py
```

### Comparing `pisoundtrack-0.2.3/LICENSE` & `pisoundtrack-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pisoundtrack-0.2.3/PKG-INFO` & `pisoundtrack-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisoundtrack
-Version: 0.2.3
+Version: 0.2.4
 Summary: Raspberry Pi Sound tracking and influx output
 Home-page: https://github.com/Phornee/pisoundtrack
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pisoundtrack-0.2.3/pisoundtrack/soundtrack.py` & `pisoundtrack-0.2.4/pisoundtrack/soundtrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,29 +105,28 @@
                 decibels = 0.0
             else:
                 decibels = 20 * math.log10(max_read/MIN_AUDIBLE_LEVEL)
 
             self.logger.info(f"Decibels = {decibels}")
             points = [
                 {
-                    "measurement": "sound",
                     "tags": {
                         "soundid": self.config['id']
                     },
-                    "time": datetime.utcnow(),
                     "fields": {
                         "max": float(max_read),
                         "max_raw": float(max_read / SHORT_NORMALIZE),
                         "db_raw": 20 * math.log10(max_read),
                         "db": float(decibels)
                     }
                 }
             ]
+
             try:
-                self.conn.insert("DHT22", points)
+                self.conn.insert("sound", points)
             except Exception as ex:
                 self.logger.error(f"RuntimeError: {ex}")
                 url = self.config['influxdbconn']['url']
                 token = self.config['influxdbconn']['token']
                 self.logger.error(f"influxDBURL={url} | influxDBToken={token}")
 
 if __name__ == "__main__":
```

### Comparing `pisoundtrack-0.2.3/pisoundtrack.egg-info/PKG-INFO` & `pisoundtrack-0.2.4/pisoundtrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisoundtrack
-Version: 0.2.3
+Version: 0.2.4
 Summary: Raspberry Pi Sound tracking and influx output
 Home-page: https://github.com/Phornee/pisoundtrack
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pisoundtrack-0.2.3/setup.py` & `pisoundtrack-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pisoundtrack",
-    version="0.2.3",
+    version="0.2.4",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Sound tracking and influx output",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/pisoundtrack",
     packages=setuptools.find_packages(),
```

