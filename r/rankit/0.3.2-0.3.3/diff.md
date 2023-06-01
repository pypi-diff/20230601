# Comparing `tmp/rankit-0.3.2.tar.gz` & `tmp/rankit-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankit-0.3.2.tar", last modified: Sat Sep  3 07:54:40 2022, max compression
+gzip compressed data, was "rankit-0.3.3.tar", last modified: Thu Jun  1 00:06:20 2023, max compression
```

## Comparing `rankit-0.3.2.tar` & `rankit-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:40.305120 rankit-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-03 07:54:18.000000 rankit-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-03 07:54:18.000000 rankit-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-09-03 07:54:40.305120 rankit-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17508 2022-09-03 07:54:18.000000 rankit-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-09-03 07:54:18.000000 rankit-0.3.2/Readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:40.305120 rankit-0.3.2/rankit/
--rw-r--r--   0 runner    (1001) docker     (121)     4645 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Merge.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:40.305120 rankit-0.3.2/rankit/Ranker/
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Ranker/LeastViolatedRank.py
--rw-r--r--   0 runner    (1001) docker     (121)    26806 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Ranker/TimeSeriesRanker.py
--rw-r--r--   0 runner    (1001) docker     (121)    14697 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Ranker/UnsupervisedRanker.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Ranker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:40.305120 rankit-0.3.2/rankit/Ranker/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Ranker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2258 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Ranker/tests/test_ranker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5656 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Ranker/tests/test_timeseries_ranker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:40.305120 rankit-0.3.2/rankit/Table/
--rw-r--r--   0 runner    (1001) docker     (121)     6759 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Table/Table.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:40.305120 rankit-0.3.2/rankit/Table/test/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Table/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/Table/test/test_table.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-03 07:54:18.000000 rankit-0.3.2/rankit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 07:54:40.305120 rankit-0.3.2/rankit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-09-03 07:54:40.000000 rankit-0.3.2/rankit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-03 07:54:40.000000 rankit-0.3.2/rankit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-03 07:54:40.000000 rankit-0.3.2/rankit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-03 07:54:40.000000 rankit-0.3.2/rankit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-03 07:54:40.000000 rankit-0.3.2/rankit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-03 07:54:18.000000 rankit-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-03 07:54:40.305120 rankit-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-09-03 07:54:18.000000 rankit-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:06:20.964267 rankit-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 00:05:44.000000 rankit-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 00:05:44.000000 rankit-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-01 00:06:20.960267 rankit-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-06-01 00:05:44.000000 rankit-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-01 00:05:44.000000 rankit-0.3.3/Readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:06:20.960267 rankit-0.3.3/rankit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:06:20.960267 rankit-0.3.3/rankit/Ranker/
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Ranker/LeastViolatedRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26806 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Ranker/TimeSeriesRanker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Ranker/UnsupervisedRanker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Ranker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:06:20.960267 rankit-0.3.3/rankit/Ranker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Ranker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Ranker/tests/test_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Ranker/tests/test_timeseries_ranker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:06:20.960267 rankit-0.3.3/rankit/Table/
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Table/Table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:06:20.960267 rankit-0.3.3/rankit/Table/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Table/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/Table/test/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 00:05:44.000000 rankit-0.3.3/rankit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:06:20.960267 rankit-0.3.3/rankit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-01 00:06:20.000000 rankit-0.3.3/rankit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-01 00:06:20.000000 rankit-0.3.3/rankit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 00:06:20.000000 rankit-0.3.3/rankit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 00:06:20.000000 rankit-0.3.3/rankit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 00:06:20.000000 rankit-0.3.3/rankit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 00:05:44.000000 rankit-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 00:06:20.964267 rankit-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 00:05:44.000000 rankit-0.3.3/setup.py
```

### Comparing `rankit-0.3.2/LICENSE` & `rankit-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/PKG-INFO` & `rankit-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rankit
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple ranking solution for matches.
 Home-page: http://github.com/wattlebird/ranking
 Author: Ronnie Wang
 Author-email: geniusxiaoguai@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `rankit-0.3.2/README.md` & `rankit-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/Readme.rst` & `rankit-0.3.3/Readme.rst`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/rankit/Merge.py` & `rankit-0.3.3/rankit/Merge.py`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/rankit/Ranker/LeastViolatedRank.py` & `rankit-0.3.3/rankit/Ranker/LeastViolatedRank.py`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/rankit/Ranker/TimeSeriesRanker.py` & `rankit-0.3.3/rankit/Ranker/TimeSeriesRanker.py`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/rankit/Ranker/UnsupervisedRanker.py` & `rankit-0.3.3/rankit/Ranker/UnsupervisedRanker.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         """
         drawMargin = self.drawMargin
         data = table.table[['hidx', 'vidx', 'hscore', 'vscore', 'weight']]
 
         m = data.shape[0]
         n = table.itemnum
         y = np.zeros(m)
-        dat = np.zeros(m*2, dtype=np.float)
+        dat = np.zeros(m*2, dtype=np.float32)
         col = np.zeros(m*2, dtype=int)
         row = np.zeros(m*2, dtype=int)
         for i, itm in enumerate(data.itertuples(index=False, name=None)):
             row[i*2]=i; col[i*2]=itm[0]; dat[i*2]=itm[4];
             row[i*2+1]=i; col[i*2+1]=itm[1]; dat[i*2+1]=-itm[4];
             if np.abs(itm[2]-itm[3])<=drawMargin:
                 y[i]=0.0
@@ -116,19 +116,19 @@
         Returns
         -------
         pandas.DataFrame, with column ['name', 'rating', 'rank']
         """
         drawMargin = self.drawMargin
         C = np.zeros((table.itemnum, table.itemnum))
         b = np.zeros(table.itemnum)
-        for (i, j), c in table.table.groupby(['hidx', 'vidx'])['weight'].agg('count').iteritems():
+        for (i, j), c in table.table.groupby(['hidx', 'vidx'])['weight'].agg('count').items():
             C[i][j] -= c
-        for inx, val in table.table.groupby('hidx').apply(colleyAgg, drawMargin, False).iteritems():
+        for inx, val in table.table.groupby('hidx').apply(colleyAgg, drawMargin, False).items():
             b[inx] += val
-        for inx, val in table.table.groupby('vidx').apply(colleyAgg, drawMargin, True).iteritems():
+        for inx, val in table.table.groupby('vidx').apply(colleyAgg, drawMargin, True).items():
             b[inx] += val
         C = C + C.T
         np.fill_diagonal(C, -np.sum(C, axis=0)+2)
         b = b/2 + 1
 
         rating = sp.linalg.solve(C, b)
         if hasattr(self, "rating"):
```

### Comparing `rankit-0.3.2/rankit/Ranker/tests/test_ranker.py` & `rankit-0.3.3/rankit/Ranker/tests/test_ranker.py`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/rankit/Ranker/tests/test_timeseries_ranker.py` & `rankit-0.3.3/rankit/Ranker/tests/test_timeseries_ranker.py`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/rankit/Table/Table.py` & `rankit-0.3.3/rankit/Table/Table.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,35 +73,33 @@
                 idx+=1
 
         self.itemlut = itemlut
         self.indexlut = indexlut
         self.itemnum = idx
 
         # raw table need to be converted to standard indexed table.
-        raw_table['hidx'] = np.require(list(map(lambda x: itemlut[x], raw_table["host"].tolist())), dtype=np.int)
-        raw_table['vidx'] = np.require(list(map(lambda x: itemlut[x], raw_table["visit"].tolist())), dtype=np.int)
+        raw_table['hidx'] = np.require(list(map(lambda x: itemlut[x], raw_table["host"].tolist())), dtype=np.int32)
+        raw_table['vidx'] = np.require(list(map(lambda x: itemlut[x], raw_table["visit"].tolist())), dtype=np.int32)
 
         self.table = raw_table
 
     def update_single(self, host, visit, hscore, vscore, time=None, weight=1.0):
         if host not in self.itemlut:
             self.itemlut[host] = len(self.indexlut)
             self.indexlut.append(host)
             self.itemnum += 1
         if visit not in self.itemlut:
             self.itemlut[visit] = len(self.indexlut)
             self.indexlut.append(visit)
             self.itemnum += 1
         
-        self.table.append(
-            pd.DataFrame([[host, visit, hscore, vscore, weight, time, self.itemlut[host], self.itemlut[visit]]],
+        t = pd.DataFrame([[host, visit, hscore, vscore, weight, time, self.itemlut[host], self.itemlut[visit]]],
               columns=['host', 'visit', 'hscore', 'vscore', 'weight', 'time', 'hidx', 'vidx']
-            ),
-            ignore_index=True
-        )
+            )
+        self.table = pd.concat([self.table, t], ignore_index=True)
 
     def setup(self, itemlut, indexlut, itemnum):
         self.itemlut = itemlut
         self.indexlut = indexlut
         self.itemnum = itemnum
 
     def iteritem(self):
```

### Comparing `rankit-0.3.2/rankit/Table/test/test_table.py` & `rankit-0.3.3/rankit/Table/test/test_table.py`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/rankit.egg-info/PKG-INFO` & `rankit-0.3.3/rankit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rankit
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple ranking solution for matches.
 Home-page: http://github.com/wattlebird/ranking
 Author: Ronnie Wang
 Author-email: geniusxiaoguai@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `rankit-0.3.2/rankit.egg-info/SOURCES.txt` & `rankit-0.3.3/rankit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rankit-0.3.2/setup.py` & `rankit-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if os.path.exists('MANIFEST'):
     os.remove('MANIFEST')
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(name="rankit",
-      version="0.3.2",
+      version="0.3.3",
       packages=find_packages(exclude=['example']),
       install_requires=required,
       include_package_data=True,
       description="A simple ranking solution for matches.",
       long_description=open('Readme.rst').read(),
       author="Ronnie Wang",
       author_email="geniusxiaoguai@gmail.com",
```

