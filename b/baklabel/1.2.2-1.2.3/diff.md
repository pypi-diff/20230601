# Comparing `tmp/baklabel-1.2.2.tar.gz` & `tmp/baklabel-1.2.3.tar.gz`

## Comparing `baklabel-1.2.2.tar` & `baklabel-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.2/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 baklabel-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 baklabel-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/about.txt
--rw-r--r--   0        0        0    20914 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/backup_howto.txt
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/examples.txt
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/release_note.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/synopsis.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/baklabel/__init__.py
--rw-r--r--   0        0        0    24228 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/baklabel/baklabel.py
--rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/baklabel/test_baklabel.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 baklabel-1.2.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 baklabel-1.2.2/LICENSE
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 baklabel-1.2.2/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 baklabel-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 baklabel-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 baklabel-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 baklabel-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.3/baklabel/__init__.py
+-rw-r--r--   0        0        0    24228 2020-02-02 00:00:00.000000 baklabel-1.2.3/baklabel/baklabel.py
+-rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 baklabel-1.2.3/baklabel/test_baklabel.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 baklabel-1.2.3/doc/about.txt
+-rw-r--r--   0        0        0    20914 2020-02-02 00:00:00.000000 baklabel-1.2.3/doc/backup_howto.txt
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 baklabel-1.2.3/doc/instructions.txt
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 baklabel-1.2.3/doc/release_note.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 baklabel-1.2.3/doc/synopsis.txt
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 baklabel-1.2.3/src/.backlabel.py.swp
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 baklabel-1.2.3/src/.baklabel.py.swp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.3/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.3/src/baklabel/__init__.py
+-rw-r--r--   0        0        0    24201 2020-02-02 00:00:00.000000 baklabel-1.2.3/src/baklabel/baklabel.py
+-rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 baklabel-1.2.3/src/baklabel/test_baklabel.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 baklabel-1.2.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 baklabel-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 baklabel-1.2.3/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 baklabel-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 baklabel-1.2.3/PKG-INFO
```

### Comparing `baklabel-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `baklabel-1.2.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `baklabel-1.2.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/doc/backup_howto.txt` & `baklabel-1.2.3/doc/backup_howto.txt`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/doc/examples.txt` & `baklabel-1.2.3/doc/instructions.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Examples for date 8 October 2010 at 5:15am
 ==========================================
 
-These instructions apply to command-line execution and when baklabel is called from a shell script or batch file. See also synopsis.txt for command line options used in the examples below.
+These instructions apply to command-line execution and when baklabel is called from a
+shell script or batch file. See also synopsis.txt for command line options used in the
+examples below.
 
 When baklabel is imported into another program, usual Python rules apply.
 
-In the following examples, please note that on Friday 8 October 2010 at 5:15am, it is the second Friday of the month. The default time for switching the label from yesterday to today is 4am. By default, if baklabel is run earlier than 4am it will return 'thu'.
-
-Note also that the 6am and 5am examples below need to be considered from the viewpoint that it is currently 5:15am.
-
-In particular, this means the 5am trigger point shown in the example is in the past so baklabel produces a label for today (fri_2). In the case of the 6am switch, the current time (5:15am) is before 6am so baklabel assumes the backup is labelled for yesterday (thu).
+In the following examples, please note that on Friday 8 October 2010 at 5:15am, it is
+the second Friday of the month. The default time for switching the label from yesterday
+to today is 4am. By default, if baklabel is run earlier than 4am it will return 'thu'.
+
+Note also that the 6am and 5am examples below need to be considered from the viewpoint
+that it is currently 5:15am.
+
+In particular, this means the 5am trigger point shown in the example is in the past so
+baklabel produces a label for today (fri_2). In the case of the 6am switch, the current
+time (5:15am) is before 6am so baklabel assumes the backup is labelled for yesterday
+(thu).
 
 Remember that all the examples here were run at 05:15 on Friday 8 Oct 2010.
 
 
 C:\baklabel>python baklabel.py
 fri_2
```

### Comparing `baklabel-1.2.2/doc/release_note.txt` & `baklabel-1.2.3/doc/release_note.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 baklabel - see Description below
 ========
 
 Version    Who  When/What
 =========================
 
+ver 1.2.3   md  1 Jun 2023 - Repair missing -- for --weekly-day option (-w)
+
 ver 1.2.2   md  1 Jun 2023 - Further clean up documentation
 
 ver 1.2.1   md  30 May 2023 - Clean up documentation
 
 ver 1.2.0   md  29 May 2023 - Improve guessdate() to resolve ambiguous dates
 
 ver 1.1.0   md  23 May 2023 - Change from GPL3 to MIT license, change to pyproject.toml
@@ -25,20 +27,20 @@
 ver 1.0.0   md  3 Nov 2010 - New option to append current year to any month-end label,
                 not just end-of-year.
 
 ver 0.2.0   md  27 Oct 2010 - Help now respects defaults which have been adjusted in
                 the source code. A new default now permits adjustment of new_year_month
                 which sets the end-of-year label to any desired month.
 
-ver 0.1.0b   md 8 Oct 2010 - Added -d numeric option for setting the label to x days
+ver 0.1.0b  md  8 Oct 2010 - Added -d numeric option for setting the label to x days
                 ago. Eg., -1 = yesterday. Also added a time trigger option in the -d
                 switch such that, for example, -d 3am will produce yesterday's label
                 if baklabel is called prior to 3am
 
-ver 0.0.0a   md 1 Jul 2010 - first written
+ver 0.0.0a  md  1 Jul 2010 - first written
 
 
 Description
 ===========
 Baklabel is intended for use in automated scripts to deliver a sensible directory path
 fragment (or label) each day to construct a grandfathered local backup.
 
@@ -114,21 +116,19 @@
 month-end. baklabel defaults to appending the year to the December backup label. This
 can be defeated with the '-y False' option.
 
 If the new year begins in July rather than January, for example, use the '-n 7' option.
 This makes June 30 the end-of-year backup rather than December 31. The June label would
 then be 'jun_2023'.
 
-If you prefer a different day than Friday for these week-end backups there is no
-command line option. You need to edit the baklabel code and change WEEKLY_DAY to
-represent a different day of the week. Use the Python number of the day-of-week.
-
-To defeat week-end backups altogether and make Friday just another day, make WEEKLY_DAY
-greater than or equal to 7. Skipping week-end backups would not be recommended by most
-grandfathers!
+If you prefer a different day than Friday for these week-end backups the command line
+option is -w. Use the Python number of the day-of-week: 0 is Monday and Friday is 4.
+
+To defeat week-end backups altogether and make Friday just another day, use -w 7.
+Skipping week-end backups would not be recommended by most grandfathers!
 
 
 Source:  https://github.com/mdewhirst/baklabel
 
 Mike Dewhirst
 miked@dewhirst.com.au
```

### Comparing `baklabel-1.2.2/doc/synopsis.txt` & `baklabel-1.2.3/doc/synopsis.txt`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/src/baklabel/baklabel.py` & `baklabel-1.2.3/baklabel/baklabel.py`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/src/baklabel/test_baklabel.py` & `baklabel-1.2.3/baklabel/test_baklabel.py`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/LICENSE` & `baklabel-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/README.md` & `baklabel-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.2/pyproject.toml` & `baklabel-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baklabel"
-version = '1.2.2'
+version = '1.2.3'
 authors = [
   { name="Mike Dewhirst", email="miked@dewhirst.com.au" },
 ]
 description = "Baklabel delivers a daily label fragment for grandfathered backups"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `baklabel-1.2.2/PKG-INFO` & `baklabel-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baklabel
-Version: 1.2.2
+Version: 1.2.3
 Summary: Baklabel delivers a daily label fragment for grandfathered backups
 Project-URL: Homepage, https://svn.climate.com.au/repos/pysrc/foss/baklabel
 Author-email: Mike Dewhirst <miked@dewhirst.com.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

