# Comparing `tmp/kattis-problem-setup-1.0.2.tar.gz` & `tmp/kattis-problem-setup-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kattis-problem-setup-1.0.2.tar", last modified: Wed Jun  9 20:30:37 2021, max compression
+gzip compressed data, was "kattis-problem-setup-1.0.3.tar", last modified: Wed May 31 23:06:54 2023, max compression
```

## Comparing `kattis-problem-setup-1.0.2.tar` & `kattis-problem-setup-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 20:30:37.086574 kattis-problem-setup-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2021-06-09 20:30:37.086574 kattis-problem-setup-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2021-06-09 20:30:30.000000 kattis-problem-setup-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 20:30:37.086574 kattis-problem-setup-1.0.2/kattis_download/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 20:30:30.000000 kattis-problem-setup-1.0.2/kattis_download/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4672 2021-06-09 20:30:30.000000 kattis-problem-setup-1.0.2/kattis_download/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 20:30:37.086574 kattis-problem-setup-1.0.2/kattis_problem_setup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2021-06-09 20:30:36.000000 kattis-problem-setup-1.0.2/kattis_problem_setup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-06-09 20:30:37.000000 kattis-problem-setup-1.0.2/kattis_problem_setup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-09 20:30:36.000000 kattis-problem-setup-1.0.2/kattis_problem_setup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-06-09 20:30:36.000000 kattis-problem-setup-1.0.2/kattis_problem_setup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-06-09 20:30:36.000000 kattis-problem-setup-1.0.2/kattis_problem_setup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-06-09 20:30:36.000000 kattis-problem-setup-1.0.2/kattis_problem_setup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-09 20:30:37.086574 kattis-problem-setup-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      905 2021-06-09 20:30:30.000000 kattis-problem-setup-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:06:54.992593 kattis-problem-setup-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-31 23:06:54.992593 kattis-problem-setup-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-31 23:06:46.000000 kattis-problem-setup-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:06:54.992593 kattis-problem-setup-1.0.3/kattis_download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:06:46.000000 kattis-problem-setup-1.0.3/kattis_download/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4597 2023-05-31 23:06:46.000000 kattis-problem-setup-1.0.3/kattis_download/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:06:54.992593 kattis-problem-setup-1.0.3/kattis_problem_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-31 23:06:54.000000 kattis-problem-setup-1.0.3/kattis_problem_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-31 23:06:54.000000 kattis-problem-setup-1.0.3/kattis_problem_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:06:54.000000 kattis-problem-setup-1.0.3/kattis_problem_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 23:06:54.000000 kattis-problem-setup-1.0.3/kattis_problem_setup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 23:06:54.000000 kattis-problem-setup-1.0.3/kattis_problem_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 23:06:54.000000 kattis-problem-setup-1.0.3/kattis_problem_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:06:54.992593 kattis-problem-setup-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-31 23:06:46.000000 kattis-problem-setup-1.0.3/setup.py
```

### Comparing `kattis-problem-setup-1.0.2/README.md` & `kattis-problem-setup-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kattis-problem-setup-1.0.2/kattis_download/main.py` & `kattis-problem-setup-1.0.3/kattis_download/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,27 +32,27 @@
 
     # Parse into a dictionary
     p = dict()
 
     # Store the actual title of the problem
     p["title"] = soup.find("h1").text
 
-    # Nested "sidebar-info" divs; recursively move inwards until at deepest
-    sidebar = soup.find("div", {"class": "sidebar-info"})
-    while sidebar.find("div", {"class": "sidebar-info"}):
-        sidebar = sidebar.find("div", {"class": "sidebar-info"})
-
-    # Last level deep has 2, the first is the buttons, second is problem data
-    sidebar = sidebar.find_next_sibling("div")
-
-    # Take the value in each attribute, ignore first (ID)
-    attributes = [p.text.split(":")[1].strip() for p in sidebar.findChildren("p")][1:]
-    attribute_keys = ["cpu", "memory", "difficulty"]
-    for _ in range(len(attribute_keys)):
-        p[attribute_keys[_]] = attributes[_]
+    # Get the cpu time limit, memory limit, and difficulty of the problem 
+    metadata = soup.find_all("div", {"class":"metadata_list-item"})
+    tag_attr_name_mapping = {'cpu_limit':'cpu',
+                     'mem_limit':'memory', 
+                     'difficulty':'difficulty'}
+    for item in metadata:
+        try:
+            data_name = item.attrs['data-name'].split('-')[1]
+            if data_name in tag_attr_name_mapping:
+                children = item.findChildren('span')
+                p[tag_attr_name_mapping[data_name]] = children[-1].text
+        except:
+            pass
 
     # Find all tables with sample data in the Soup
     tables = soup.findAll("table", {"summary": "sample data"})
     p["tables"] = []
     for table in tables:
         p["tables"].append([j.text for j in table.findAll("pre")])
```

### Comparing `kattis-problem-setup-1.0.2/setup.py` & `kattis-problem-setup-1.0.3/setup.py`

 * *Files identical despite different names*

