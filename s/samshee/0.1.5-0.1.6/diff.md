# Comparing `tmp/samshee-0.1.5.tar.gz` & `tmp/samshee-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samshee-0.1.5.tar", last modified: Fri May 12 08:55:22 2023, max compression
+gzip compressed data, was "samshee-0.1.6.tar", last modified: Thu Jun  1 10:47:26 2023, max compression
```

## Comparing `samshee-0.1.5.tar` & `samshee-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.798524 samshee-0.1.5/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.5/LICENSE
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-05-12 08:55:22.798524 samshee-0.1.5/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.5/README.md
--rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-05-12 08:52:33.000000 samshee-0.1.5/pyproject.toml
--rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-05-12 08:55:22.798524 samshee-0.1.5/setup.cfg
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.795190 samshee-0.1.5/src/
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.795190 samshee-0.1.5/src/samshee/
--rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.5/src/samshee/__init__.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.5/src/samshee/samplesheetv2.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.5/src/samshee/sectionedsheet.py
--rw-r--r--   0 jakob     (1000) jakob     (1000)    26204 2023-05-12 08:51:18.000000 samshee-0.1.5/src/samshee/validation.py
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.798524 samshee-0.1.5/src/samshee.egg-info/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/PKG-INFO
--rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/SOURCES.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/dependency_links.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/requires.txt
--rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-05-12 08:55:22.000000 samshee-0.1.5/src/samshee.egg-info/top_level.txt
-drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-05-12 08:55:22.798524 samshee-0.1.5/tests/
--rw-r--r--   0 jakob     (1000) jakob     (1000)     6574 2023-02-25 05:46:18.000000 samshee-0.1.5/tests/test_validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-01 10:47:26.698886 samshee-0.1.6/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     1068 2023-01-20 14:22:02.000000 samshee-0.1.6/LICENSE
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-06-01 10:47:26.698886 samshee-0.1.6/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     6621 2023-02-13 06:26:50.000000 samshee-0.1.6/README.md
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      919 2023-06-01 10:40:04.000000 samshee-0.1.6/pyproject.toml
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       38 2023-06-01 10:47:26.698886 samshee-0.1.6/setup.cfg
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-01 10:47:26.695552 samshee-0.1.6/src/
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-01 10:47:26.695552 samshee-0.1.6/src/samshee/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      134 2023-02-13 05:48:16.000000 samshee-0.1.6/src/samshee/__init__.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     4281 2023-02-15 05:05:57.000000 samshee-0.1.6/src/samshee/samplesheetv2.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     5605 2023-03-20 07:31:49.000000 samshee-0.1.6/src/samshee/sectionedsheet.py
+-rw-r--r--   0 jakob     (1000) jakob     (1000)    26705 2023-06-01 10:39:47.000000 samshee-0.1.6/src/samshee/validation.py
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-01 10:47:26.698886 samshee-0.1.6/src/samshee.egg-info/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8620 2023-06-01 10:47:26.000000 samshee-0.1.6/src/samshee.egg-info/PKG-INFO
+-rw-r--r--   0 jakob     (1000) jakob     (1000)      340 2023-06-01 10:47:26.000000 samshee-0.1.6/src/samshee.egg-info/SOURCES.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        1 2023-06-01 10:47:26.000000 samshee-0.1.6/src/samshee.egg-info/dependency_links.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)       17 2023-06-01 10:47:26.000000 samshee-0.1.6/src/samshee.egg-info/requires.txt
+-rw-r--r--   0 jakob     (1000) jakob     (1000)        8 2023-06-01 10:47:26.000000 samshee-0.1.6/src/samshee.egg-info/top_level.txt
+drwxr-xr-x   0 jakob     (1000) jakob     (1000)        0 2023-06-01 10:47:26.698886 samshee-0.1.6/tests/
+-rw-r--r--   0 jakob     (1000) jakob     (1000)     8092 2023-06-01 10:46:57.000000 samshee-0.1.6/tests/test_validation.py
```

### Comparing `samshee-0.1.5/LICENSE` & `samshee-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `samshee-0.1.5/PKG-INFO` & `samshee-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.5
+Version: 0.1.6
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.5/README.md` & `samshee-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `samshee-0.1.5/pyproject.toml` & `samshee-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "samshee"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Jakob Simeth", email="jakob.simeth@ukr.de" }
 ]
 description="A schema-agnostic parser and writer for illumina sample sheets v2."
 readme = "README.md"
 license={file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `samshee-0.1.5/src/samshee/samplesheetv2.py` & `samshee-0.1.6/src/samshee/samplesheetv2.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.5/src/samshee/sectionedsheet.py` & `samshee-0.1.6/src/samshee/sectionedsheet.py`

 * *Files identical despite different names*

### Comparing `samshee-0.1.5/src/samshee/validation.py` & `samshee-0.1.6/src/samshee/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,24 @@
         cyc = expand(cycles[1])
         if is_read(cyc):
             res["Read2Cycles"] = cyc
         else:
             res["Index1Cycles"] = cyc
     elif len(cycles) == 3:
         res["Index1Cycles"] = expand(cycles[1])
-        res["Read2Cycles"] = expand(cycles[2])
+        # there may be two indices but just one read
+        if "Y" in cycles[2]:
+            res["Read2Cycles"] = expand(cycles[2])
+        elif "I" in cycles[2] or "N" in cycles[2] or "U" in cycles[2]:
+            res["Index2Cycles"] = expand(cycles[2])
+        else:
+            # there may be edge cases. If these occur, then probably one needs to resort to the sequencing settings section.
+            raise Exception(
+                "cannot determine type of third element in OverrideCycles. Probably an implementation error."
+            )
     elif len(cycles) == 4:
         res["Index1Cycles"] = expand(cycles[1])
         res["Index2Cycles"] = expand(cycles[2])
         res["Read2Cycles"] = expand(cycles[3])
     elif len(cycles) == 1:
         pass
     else:
```

### Comparing `samshee-0.1.5/src/samshee.egg-info/PKG-INFO` & `samshee-0.1.6/src/samshee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samshee
-Version: 0.1.5
+Version: 0.1.6
 Summary: A schema-agnostic parser and writer for illumina sample sheets v2.
 Author-email: Jakob Simeth <jakob.simeth@ukr.de>
 License: MIT License
         
         Copyright © 2023 Jakob Simeth
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `samshee-0.1.5/tests/test_validation.py` & `samshee-0.1.6/tests/test_validation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 import pytest
-from samshee.validation import check_index_distance
+from samshee.validation import check_index_distance, parse_overrideCycles
 from samshee.sectionedsheet import SectionedSheet
 
 
 def test_if_check_index_distance_accepts_only_mindists_larger_than_0():
     with pytest.raises(ValueError):
         check_index_distance(
             SectionedSheet(
@@ -171,7 +171,35 @@
                         {"Sample_ID": "b", "Index": "TTTT", "Index2": "ACAC"},
                         {"Sample_ID": "b", "Index": "TTTA", "Index2": "ACAC"},
                     ],
                 }
             ),
             mindist=1,  # index2 has mindist of 2, which should be okay.
         )
+
+
+def test_if_overrideCycles_finds_index_and_reads_correctly():
+    cycles = parse_overrideCycles("Y4")
+    assert "Read1Cycles" in cycles and cycles["Read1Cycles"] == "YYYY"
+    assert "Index1Cycles" not in cycles
+    assert "Index2Cycles" not in cycles
+    assert "Read2Cycles" not in cycles
+    cycles = parse_overrideCycles("Y4;I3")
+    assert "Read1Cycles" in cycles and cycles["Read1Cycles"] == "YYYY"
+    assert "Index1Cycles" in cycles and cycles["Index1Cycles"] == "III"
+    assert "Index2Cycles" not in cycles
+    assert "Read2Cycles" not in cycles
+    cycles = parse_overrideCycles("Y4;I3;I1N2")
+    assert "Read1Cycles" in cycles and cycles["Read1Cycles"] == "YYYY"
+    assert "Index1Cycles" in cycles and cycles["Index1Cycles"] == "III"
+    assert "Index2Cycles" in cycles and cycles["Index2Cycles"] == "INN"
+    assert "Read2Cycles" not in cycles
+    cycles = parse_overrideCycles("Y4;I3;Y2N1")
+    assert "Read1Cycles" in cycles and cycles["Read1Cycles"] == "YYYY"
+    assert "Index1Cycles" in cycles and cycles["Index1Cycles"] == "III"
+    assert "Index2Cycles" not in cycles
+    assert "Read2Cycles" in cycles and cycles["Read2Cycles"] == "YYN"
+    cycles = parse_overrideCycles("Y4;I3;I4;Y2")
+    assert "Read1Cycles" in cycles and cycles["Read1Cycles"] == "YYYY"
+    assert "Index1Cycles" in cycles and cycles["Index1Cycles"] == "III"
+    assert "Index2Cycles" in cycles and cycles["Index2Cycles"] == "IIII"
+    assert "Read2Cycles" in cycles and cycles["Read2Cycles"] == "YY"
```

