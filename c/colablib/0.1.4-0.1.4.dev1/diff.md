# Comparing `tmp/colablib-0.1.4.tar.gz` & `tmp/colablib-0.1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.4.tar", last modified: Thu Jun  1 10:50:16 2023, max compression
+gzip compressed data, was "colablib-0.1.4.dev1.tar", last modified: Thu Jun  1 11:13:02 2023, max compression
```

## Comparing `colablib-0.1.4.tar` & `colablib-0.1.4.dev1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 10:50:16.339156 colablib-0.1.4/
--rw-rw-rw-   0        0        0      213 2023-06-01 10:50:16.338155 colablib-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 10:50:16.316938 colablib-0.1.4/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.4/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.4/colablib/cprint.py
--rw-rw-rw-   0        0        0     1337 2023-06-01 10:48:41.000000 colablib-0.1.4/colablib/deb_utils.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.4/colablib/git_utils.py
--rw-rw-rw-   0        0        0     2594 2023-06-01 10:44:06.000000 colablib-0.1.4/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 10:50:16.337253 colablib-0.1.4/colablib.egg-info/
--rw-rw-rw-   0        0        0      213 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 10:50:16.000000 colablib-0.1.4/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 10:50:16.339156 colablib-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      311 2023-06-01 10:49:13.000000 colablib-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:13:02.109045 colablib-0.1.4.dev1/
+-rw-rw-rw-   0        0        0      218 2023-06-01 11:13:02.109045 colablib-0.1.4.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.4.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 11:13:02.096471 colablib-0.1.4.dev1/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.4.dev1/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.4.dev1/colablib/cprint.py
+-rw-rw-rw-   0        0        0     1181 2023-06-01 11:12:05.000000 colablib-0.1.4.dev1/colablib/deb_utils.py
+-rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.4.dev1/colablib/git_utils.py
+-rw-rw-rw-   0        0        0     2594 2023-06-01 10:44:06.000000 colablib-0.1.4.dev1/colablib/py_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:13:02.108071 colablib-0.1.4.dev1/colablib.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 11:13:01.000000 colablib-0.1.4.dev1/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 11:13:02.109045 colablib-0.1.4.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      316 2023-06-01 11:12:27.000000 colablib-0.1.4.dev1/setup.py
```

### Comparing `colablib-0.1.4/colablib/cprint.py` & `colablib-0.1.4.dev1/colablib/cprint.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.4/colablib/deb_utils.py` & `colablib-0.1.4.dev1/colablib/deb_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,26 +17,23 @@
     """
     os.makedirs(dst, exist_ok=True)
     filename = get_filename(url)
     response = requests.get(url, stream=True)
     response.raise_for_status()
 
     with open(filename, "wb") as file:
-        for chunk in tqdm(response.iter_content(chunk_size=8192), desc="Downloading"):
+        for chunk in response.iter_content(chunk_size=8192):
             if chunk:
                 file.write(chunk)
 
     with zipfile.ZipFile(filename, "r") as deps:
         deps.extractall(dst)
 
     if desc is None:
-        desc = "installing"
+        desc = cprint("Installing", color="green", tqdm_desc=True)
+
     for file in tqdm(os.listdir(dst), desc=desc):
         if file.endswith(".deb"):
-            try:
-                subprocess.run(["dpkg", "-i", os.path.join(dst, file)], stdout=subprocess.DEVNULL, check=True)
-            except subprocess.CalledProcessError as e:
-                cprint(f"Error installing {file}: {e}", color="red")
-                raise
+            subprocess.run(["dpkg", "-i", os.path.join(dst, file)], stdout=subprocess.DEVNULL, check=True)
 
     os.remove(filename)
     shutil.rmtree(dst)
```

### Comparing `colablib-0.1.4/colablib/git_utils.py` & `colablib-0.1.4.dev1/colablib/git_utils.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.4/colablib/py_utils.py` & `colablib-0.1.4.dev1/colablib/py_utils.py`

 * *Files identical despite different names*

