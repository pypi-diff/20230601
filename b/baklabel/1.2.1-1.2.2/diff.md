# Comparing `tmp/baklabel-1.2.1.tar.gz` & `tmp/baklabel-1.2.2.tar.gz`

## Comparing `baklabel-1.2.1.tar` & `baklabel-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.1/__init__.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 baklabel-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 baklabel-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/about.txt
--rw-r--r--   0        0        0    20706 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/backup_howto.txt
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/examples.txt
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/release_note.txt
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 baklabel-1.2.1/doc/synopsis.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/baklabel/__init__.py
--rw-r--r--   0        0        0    24161 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/baklabel/baklabel.py
--rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 baklabel-1.2.1/src/baklabel/test_baklabel.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 baklabel-1.2.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 baklabel-1.2.1/LICENSE
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 baklabel-1.2.1/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 baklabel-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 baklabel-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.2/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 baklabel-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 baklabel-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/about.txt
+-rw-r--r--   0        0        0    20914 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/backup_howto.txt
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/examples.txt
+-rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/release_note.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 baklabel-1.2.2/doc/synopsis.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/baklabel/__init__.py
+-rw-r--r--   0        0        0    24228 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/baklabel/baklabel.py
+-rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 baklabel-1.2.2/src/baklabel/test_baklabel.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 baklabel-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 baklabel-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 baklabel-1.2.2/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 baklabel-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 baklabel-1.2.2/PKG-INFO
```

### Comparing `baklabel-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `baklabel-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `baklabel-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.1/doc/backup_howto.txt` & `baklabel-1.2.2/doc/backup_howto.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,56 @@
-Target Audience - baklabel
-==========================
+Target Audience
+===============
 
-The 'baklabel' utility is intended for a system administrator to install and set up to suit the system owner. The instructions are intended to be more or less understandable by most users but the detailed sections will require some experience or at least moderate confidence.
-
-This document describes grandfathered backups. It then explains in overview how to install the necessary components to make a grandfathered backup system actually work. Finally, it contains the exact (five line) Python script needed to use baklabel and two example Windows batch files which employ xcopy in one and robocopy in the other to perform the backups.
-
-All Windows systems have xcopy and some also have robocopy. Robocopy is more reliable for larger backups.
-
-Linux or Mac based systems will require a bash script similar to the batch file. Also, the examples are based on Windows so drive letters will need to be replaced by network paths on non-Windows machines.
+'baklabel' is intended for a system administrator to install and set up to suit the
+business owner. The instructions are intended to be more or less understandable by
+most users but the detailed sections will require some experience or at least moderate
+confidence.
+
+This document describes grandfathered backups. It then explains in overview how to
+install the necessary components to make a grandfathered backup system actually work.
+Finally, it contains the exact (five line) Python script needed to use baklabel and
+two sample Windows batch files which employ xcopy in one and robocopy in the other to
+perform the backups.
+
+All Windows systems have xcopy and some also have robocopy. Robocopy is more reliable
+for larger backups.
+
+Linux or Mac based systems will require a bash script similar to the batch file. Also,
+the examples are based on Windows so drive letters will need to be replaced by network
+paths on non-Windows machines.
 
 
 Grandfathered Backups
 =====================
 
-In a small office or home office environment it is often quite economical to use a high capacity USB connected portable drive as backup media. They are large in the multiple terabyte range and inexpensive costing less than $500.
-
-With more than one portable drive, off-site backup is feasible.
-
-Grandfathered backups mean users can go back to almost any earlier time and retrieve information as it was then. Essentially it means that today's backup will never overwrite yesterday's backup.
-
-The secret of success is _automatic_ creation and selection of the correct destination folder for the overnight backup. The Python program which nominates the folder name for the date of the backup is called baklabel.
+Grandfathered backups mean that today's backup will never overwrite yesterday's backup.
 
-baklabel has a number of sensible defaults so it doesn't need tweaking. Eg., if the backup kicks off between midnight and 4am it defaults to yesterday's backup label.
+In a small office or home office environment it is often quite economical to use a high
+capacity USB connected portable drive as backup media. They are large in the multiple
+terabyte range and becoming less expensive.
 
-This "how to" assumes you have a very large USB drive F: and a typical backup load of less than a 24th (4 percent) the size of the drive. Your media should be big enough to permit expected growth in the load over time. There will be up to 24 copies of the backup for all the grandfathering including one manual backup and one saved annual backup.
+With more than one portable drive, off-site backup is feasible.
 
-The following pattern of 23 automatic grandfather folders and one manual folder would normally be entirely adequate because backups only get overwritten periodically rather than frequently.
+The secret of success is _automatic_ creation and selection of the correct destination
+folder for the overnight backup. The Python program which nominates the folder name
+for  the date of the backup is baklabel.py
+
+baklabel has a number of sensible defaults so it probably doesn't need tweaking. Eg.,
+if the backup kicks off between midnight and 4am it defaults to yesterday's backup
+label.
+
+This "how to" assumes you have a very large USB drive F: and a typical backup load of
+less than a 24th (4 percent) the size of the drive. Your media should be big enough to
+permit expected growth in the load over time. There will be up to 24 copies of the
+backup for all the grandfathering including one manual backup.
+
+The following pattern of 23 automatically (default) named folders and one manual folder
+would normally be entirely adequate because backups only get overwritten periodically
+rather than frequently.
 
 F:\backups\manual   (most recent manually initiated backup)
 F:\backups\mon      (most recent Monday backup)
 F:\backups\tue      (most recent Tuesday backup)
 F:\backups\wed      (most recent Wednesday backup)
 F:\backups\thu      (most recent Thursday backup)
 F:\backups\fri_1    (most recent 1st Friday of the month backup)
@@ -54,91 +75,136 @@
 
 
 How to set up Grandfathered backups
 ===================================
 
 - Install Python (see below) and baklabel
 
-- Write and test backup.bat (actually copy/paste and adjust) to copy files
-
 - Write a tiny Python program (actually copy/paste) to call backup.bat
 
+- Write and test backup.bat (actually copy/paste and adjust) to copy files
+
 - Schedule the backup to run each day (or night)
 
 
 Preparations
 ============
 
 Create an admin folder
 ----------------------
-You need a folder set aside for managing backups. Let's assume you create C:\admin for this purpose.
+You need a folder set aside for managing backups. Let's assume you create C:\admin for
+this purpose.
 
 Put scripts into the admin folder
 ---------------------------------
-This admin folder will contain backup.py, backup.bat and eventually all the log files written during both scheduled and manual backups. Log files will be named after the above directory names eg., log-wed.txt, log-manual.txt etc.
+This admin folder will contain scripts and eventually all the log files written during
+both scheduled and manual backups. Log files will be named after the bove directory
+names eg., log-wed.txt, log-manual.txt etc.
 
 Install Python
 --------------
-If you don't already have Python on your machine, download and install it from http://www.python.org.
+If you don't already have Python on your machine, download and install it from
+http://www.python.org.
 
+Install baklabel
+----------------
 pip install baklabel
 
 Install a large portable disk drive
 -----------------------------------
-Install a very large removable USB connected drive (eg drive F:) and, staying with the example above, create a root folder for the backups eg., F:\backups
-
-Schedule the nightly backup
----------------------------
-Schedule the backup to run once daily some time after all activity ceases and in time to complete before the next day's activity commences. Perhaps 1 or 2 in the morning. As indicated above, if it starts before 4am it will automatically produce the correct label for the previous day. This is the command line to schedule ...
+Install a very large removable USB connected drive (eg drive F:) and, staying with the
+example above, create a root folder for the backups eg., F:\backups
 
-python C:\admin\backup.py
-
-... with a start-in directory of C:\admin
-
-Now for the two backup components mentioned above which you must write.
+Your system administrator can postpone acquistion of the portable disk drive pending
+calculation of the size required. Do this by using a network or local drive, performing
+a manual backup and noting the disk space it occupies.
 
 
 backup.py - Python script
 =========================
 
-Create a new C:\admin\backup.py file using Notepad (not Word) then copy
-and paste the following few lines (with or without the # lines):
+Create a new C:\admin\backup.py file using Notepad (not Word) then copy and paste
+the following lines:
+
+Note that lines beginning with a # symbol are comments as is everything between pairs of triple-quotes.
 
-#########################################################
+## Start copying from here ############################# Notes
 import baklabel                                         # 1
+
 baklab = baklabel.Grandad()                             # 2
+
 baklabcmd = f'{backup.bat} {baklab.label()}'            # 3
+
 import os                                               # 4
+
 os.system(baklabcmd)                                    # 5
-#########################################################
 
-Here are some numbered notes on backup.py. Skip them if you have no interest.
+"""
+1. import baklabel imports the baklabel module installed earlier and gives this
+backup.py script direct access to the python code which calculates the correct backup
+label.
+
+2. baklab = baklabel.Grandad() is python code which creates an object called baklab
+(it could be called anything) having all the capabilities set up in the Grandad()
+class inside the baklabel module installed earlier.
+
+3. baklabcmd = <some hieroglyphics> is just creating a command line to run the backup.
+The curly brackets content get replaced with 'backup.bat' and whatever the label()
+method of baklab delivers - let's say 'mon' if today is Monday (after 4am of course).
+Then baklabcmd will become "backup.bat mon". See backup.bat below.
+
+Note that scripts are assumed to be in the same C:\admin folder. If not you need to at
+least include the full path to backup.bat.
+
+4. import os is python code which imports the os module. This is part of Python which
+figures out which operating system you are running (eg., Windows, Mac, Linux etc) so
+that the next line works properly.
 
-1. import baklabel imports the baklabel module installed in the first preparation step and gives this backup.py script direct access to the python code which calculates the correct backup label.
+5. os.system(baklabcmd) is just like typing "backup.bat mon" at a command prompt. It
+calls the operating system to execute the command.
 
-2. baklab = baklabel.Grandad() is python code which creates an object called baklab (it could be called anything) having all the capabilities set up in the Grandad() class inside the baklabel module installed earlier.
+"""
+## finish copy here #############################
 
-3. baklabcmd = <some hieroglyphics> is just creating a command line to run the backup. The curly brackets content get replaced with 'backup.bat' and whatever the label() method of baklab delivers - let's say 'mon' if today is Monday (after 4am of course). Then baklabcmd becomes "backup.bat mon".
 
-4. import os is python code which imports the os module. This is part of Python which figures out which operating system you are running (eg., Windows, Mac, Linux etc) so that the next line works properly.
+Create your preferred backup.bat
+================================
+Here are two simple examples. One is for xcopy and the other uses robocopy. Both are
+designed to produce the same results. robocopy has sophisticated options to control
+logging and here, we choose to report only the directories copied. For xcopy, the
+logging is handled manually.
+
+Copy and paste whichever example you prefer into a separate batch file. The name of the
+batch file is assumed to be backup.bat in the above Python script so if you choose a
+different name make sure you update the Python script accordingly.
+
+Both examples are repeated at the end of this document with all the rem lines stripped
+out to provide a cleaner view.
+
+Execute either batch file at any time manually without any parameters to obtain a
+backup in the F:\backups\manual folder. Otherwise schedule it to run as described in
+Preparations above to get backups in (for example) F:\backups\mon and of course other
+baklabel'd directories.
 
-5. os.system(baklabcmd) is just like typing "backup.bat mon" at a command prompt. It calls the operating system to execute the command.
+Schedule the nightly backup
+===========================
+Schedule the backup to run once daily some time after all activity ceases and in time
+to complete before the next day's activity commences. Perhaps 1 or 2 in the morning.
+As indicated above, if it starts before 4am it will automatically produce the correct
+label for the previous day. This is the command line to schedule ...
 
+C:\admin\backup.py
 
-Create your preferred backup.bat
-================================
-Here are two simple examples. One is for xcopy and the other uses robocopy. Both are designed to produce the same results. robocopy has sophisticated options to control logging and here, we choose to report only the directories copied. For xcopy, the logging is handled manually.
+... with a start-in directory of C:\admin
 
-Copy and paste whichever example you prefer into a separate batch file. The name of the batch file is assumed to be backup.bat in the above Python script so if you choose a different name make sure you update the Python script accordingly.
 
-Both examples are repeated at the end of this document with all the rem lines stripped out to provide a cleaner view.
 
-Execute either batch file at any time manually without any parameters to obtain a backup in the F:\backups\manual folder. Otherwise schedule it to run as described in Preparations above to get backups in (for example) F:\backups\mon and of course other baklabel'd directories.
 
-The xcopy and robocopy switches used are typical. See xcopy /? or robocopy /? for more detail.
+The xcopy and robocopy switches used are typical. See xcopy /? or robocopy /? for more
+detail.
 
 Each batch file begins with @echo off and ends with :end.
 
 -------------------------------------
 xcopy backup.bat - batch file example
 -------------------------------------
 @echo off
```

### Comparing `baklabel-1.2.1/doc/release_note.txt` & `baklabel-1.2.2/doc/release_note.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 baklabel - see Description below
 ========
 
 Version    Who  When/What
 =========================
 
+ver 1.2.2   md  1 Jun 2023 - Further clean up documentation
+
 ver 1.2.1   md  30 May 2023 - Clean up documentation
 
 ver 1.2.0   md  29 May 2023 - Improve guessdate() to resolve ambiguous dates
 
 ver 1.1.0   md  23 May 2023 - Change from GPL3 to MIT license, change to pyproject.toml
                 and clean up strings using f-strings
 
@@ -19,24 +21,24 @@
                 dates as a calling convenience
 
 ver 1.0.1   md  4 Nov 2010 - Minor refactoring and tidying comments
 
 ver 1.0.0   md  3 Nov 2010 - New option to append current year to any month-end label,
                 not just end-of-year.
 
-ver 0.2.0   md  27 oct 2010 - Help now respects defaults which have been adjusted in
+ver 0.2.0   md  27 Oct 2010 - Help now respects defaults which have been adjusted in
                 the source code. A new default now permits adjustment of new_year_month
                 which sets the end-of-year label to any desired month.
 
-ver 0.1.0b   md 8 oct 2010 - Added -d numeric option for setting the label to x days
+ver 0.1.0b   md 8 Oct 2010 - Added -d numeric option for setting the label to x days
                 ago. Eg., -1 = yesterday. Also added a time trigger option in the -d
                 switch such that, for example, -d 3am will produce yesterday's label
                 if baklabel is called prior to 3am
 
-ver 0.0.0a   md 1 jul 2010 - first written
+ver 0.0.0a   md 1 Jul 2010 - first written
 
 
 Description
 ===========
 Baklabel is intended for use in automated scripts to deliver a sensible directory path
 fragment (or label) each day to construct a grandfathered local backup.
 
@@ -47,15 +49,15 @@
 It is also a stand-alone utility to find the backup label produced for any given date
 and set of options.
 
 python3 baklabel.py -h  to see command line usage and options.
 
 Python 3.x (Python 2.7 should also work but is no longer tested)
 
-In the doc directory after installing, see release_note.txt for more detail on the
+In the doc directory of the baklabel repo, see release_note.txt for more detail on the
 package, examples.txt for baklabel output examples and backup_howto.txt for a sample
 backup script for Windows.
 
 
 Grandfathered Backups
 =====================
 Properly grandfathered, there needs to be a daily backup to one of 23 separate tapes,
```

### Comparing `baklabel-1.2.1/doc/synopsis.txt` & `baklabel-1.2.2/doc/synopsis.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,106 +29,106 @@
 000001c0: 636f 6d6d 616e 6420 6c69 6e65 2075 7361  command line usa
 000001d0: 6765 2061 6e64 206f 7074 696f 6e73 2e0d  ge and options..
 000001e0: 0a0d 0a50 7974 686f 6e20 332e 7820 2850  ...Python 3.x (P
 000001f0: 7974 686f 6e20 322e 3720 7368 6f75 6c64  ython 2.7 should
 00000200: 2061 6c73 6f20 776f 726b 2062 7574 2069   also work but i
 00000210: 7320 6e6f 206c 6f6e 6765 7220 7465 7374  s no longer test
 00000220: 6564 290d 0a0d 0a49 6e20 7468 6520 646f  ed)....In the do
-00000230: 6320 6469 7265 6374 6f72 7920 6166 7465  c directory afte
-00000240: 7220 696e 7374 616c 6c69 6e67 2c20 7365  r installing, se
-00000250: 6520 7265 6c65 6173 655f 6e6f 7465 2e74  e release_note.t
-00000260: 7874 2066 6f72 206d 6f72 6520 6465 7461  xt for more deta
-00000270: 696c 206f 6e20 7468 650d 0a70 6163 6b61  il on the..packa
-00000280: 6765 2c20 6578 616d 706c 6573 2e74 7874  ge, examples.txt
-00000290: 2066 6f72 2062 616b 6c61 6265 6c20 6f75   for baklabel ou
-000002a0: 7470 7574 2065 7861 6d70 6c65 7320 616e  tput examples an
-000002b0: 6420 6261 636b 7570 5f68 6f77 746f 2e74  d backup_howto.t
-000002c0: 7874 2066 6f72 2061 2073 616d 706c 650d  xt for a sample.
-000002d0: 0a62 6163 6b75 7020 7363 7269 7074 2066  .backup script f
-000002e0: 6f72 2057 696e 646f 7773 2e0d 0a0d 0a55  or Windows.....U
-000002f0: 7361 6765 3a0d 0a20 2020 2062 616b 6c61  sage:..    bakla
-00000300: 6265 6c2e 7079 205b 4f70 7469 6f6e 735d  bel.py [Options]
-00000310: 0d0a 0d0a 4f70 7469 6f6e 733a 0d0a 2020  ....Options:..  
-00000320: 2020 5769 7468 6f75 7420 6f70 7469 6f6e    Without option
-00000330: 732c 2070 726f 6475 6365 2074 6f64 6179  s, produce today
-00000340: 2773 2064 6566 6175 6c74 206c 6162 656c  's default label
-00000350: 2e20 4966 2074 6865 2063 7572 7265 6e74  . If the current
-00000360: 2074 696d 6520 6973 0d0a 2020 2020 7072   time is..    pr
-00000370: 696f 7220 746f 2034 616d 2028 7377 6974  ior to 4am (swit
-00000380: 6368 6f76 6572 2074 696d 6529 2074 6865  chover time) the
-00000390: 6e20 7072 6f64 7563 6520 7965 7374 6572  n produce yester
-000003a0: 6461 7927 7320 6c61 6265 6c2e 0d0a 0d0a  day's label.....
-000003b0: 2020 2020 2d64 2028 6465 6661 756c 7420      -d (default 
-000003c0: 6461 7465 2069 7320 746f 6461 7929 204f  date is today) O
-000003d0: 7220 7573 6520 6567 2e2c 2027 2d64 2032  r use eg., '-d 2
-000003e0: 3031 302f 332f 3330 2720 6f72 2027 2d64  010/3/30' or '-d
-000003f0: 2033 302d 332d 3230 3130 270d 0a20 2020   30-3-2010'..   
-00000400: 2020 2020 5573 6520 2f20 6f72 202d 2061      Use / or - a
-00000410: 7320 6461 7465 2073 6570 6172 6174 6f72  s date separator
-00000420: 732e 2044 6174 6520 666f 726d 6174 2069  s. Date format i
-00000430: 7320 6775 6573 7365 642e 204d 7468 2d64  s guessed. Mth-d
-00000440: 6179 2d79 6561 720d 0a20 2020 2020 2020  ay-year..       
-00000450: 6f6e 6c79 2077 6f72 6b73 2069 6620 6461  only works if da
-00000460: 7920 3e20 3132 2e0d 0a0d 0a20 2020 2020  y > 12.....     
-00000470: 2020 5573 6520 2d31 2066 6f72 2079 6573    Use -1 for yes
-00000480: 7465 7264 6179 2773 206c 6162 656c 206f  terday's label o
-00000490: 7220 2d37 2066 6f72 206c 6173 7420 7765  r -7 for last we
-000004a0: 656b 2773 206c 6162 656c 2e20 5573 6520  ek's label. Use 
-000004b0: 2b32 2066 6f72 0d0a 2020 2020 2020 2061  +2 for..       a
-000004c0: 206c 6162 656c 2066 6f72 2074 6865 2064   label for the d
-000004d0: 6179 2061 6674 6572 2074 6f6d 6f72 726f  ay after tomorro
-000004e0: 772e 2041 6e79 206e 756d 6265 7220 7769  w. Any number wi
-000004f0: 6c6c 2062 6520 636f 6d70 7574 6564 2e0d  ll be computed..
-00000500: 0a0d 0a20 2020 2020 2020 546f 2061 646a  ...       To adj
-00000510: 7573 7420 7468 6520 7377 6974 6368 6f76  ust the switchov
-00000520: 6572 2074 696d 6520 7573 6520 6567 2e2c  er time use eg.,
-00000530: 272d 6420 3661 6d27 206f 7220 272d 6420  '-d 6am' or '-d 
-00000540: 3670 6d27 2065 7463 2e0d 0a0d 0a20 2020  6pm' etc.....   
-00000550: 202d 7320 2864 6566 6175 6c74 2069 7320   -s (default is 
-00000560: 626c 616e 6b29 2073 6572 7665 7220 6e61  blank) server na
-00000570: 6d65 2075 7365 6420 746f 2070 7265 6669  me used to prefi
-00000580: 7820 7468 6520 6261 636b 7570 206c 6162  x the backup lab
-00000590: 656c 0d0a 0d0a 2020 2020 2d79 2028 6465  el....    -y (de
-000005a0: 6661 756c 7420 6973 2054 7275 6529 2041  fault is True) A
-000005b0: 7070 656e 6420 7965 6172 2074 6f20 656e  ppend year to en
-000005c0: 642d 6f66 2d79 6561 7220 6c61 6265 6c2e  d-of-year label.
-000005d0: 204f 7220 7573 6520 272d 7920 4661 6c73   Or use '-y Fals
-000005e0: 6527 0d0a 2020 2020 2020 206f 7220 272d  e'..       or '-
-000005f0: 7920 4e6f 272e 2041 6e79 7468 696e 6720  y No'. Anything 
-00000600: 656c 7365 206d 6561 6e73 2054 7275 652e  else means True.
-00000610: 0d0a 0d0a 2020 2020 2d6d 2028 6465 6661  ....    -m (defa
-00000620: 756c 7420 6973 2046 616c 7365 2920 4170  ult is False) Ap
-00000630: 7065 6e64 2079 6561 7220 746f 2065 6e64  pend year to end
-00000640: 2d6f 662d 6d6f 6e74 6820 6c61 6265 6c2e  -of-month label.
-00000650: 204f 7220 7573 6520 272d 6d20 5472 7565   Or use '-m True
-00000660: 270d 0a20 2020 2020 2020 6f72 2027 2d6d  '..       or '-m
-00000670: 2059 6573 272e 2041 6e79 7468 696e 6720   Yes'. Anything 
-00000680: 656c 7365 206d 6561 6e73 2046 616c 7365  else means False
-00000690: 2e0d 0a0d 0a20 2020 202d 6e20 2864 6566  .....    -n (def
-000006a0: 6175 6c74 2069 7320 3129 204d 6f6e 7468  ault is 1) Month
-000006b0: 206e 756d 6265 7220 636f 6d6d 656e 6369   number commenci
-000006c0: 6e67 2074 6865 206e 6577 2079 6561 722e  ng the new year.
-000006d0: 204a 616e 7561 7279 2069 7320 312e 0d0a   January is 1...
-000006e0: 0d0a 2020 2020 2d65 2028 6465 6661 756c  ..    -e (defaul
-000006f0: 7420 6973 2027 626c 616e 6b27 2920 656e  t is 'blank') en
-00000700: 642d 6f66 2d79 6561 7220 6c61 6265 6c20  d-of-year label 
-00000710: 6f6e 6c79 2068 6173 2061 6e20 6566 6665  only has an effe
-00000720: 6374 206f 6e20 6e65 7720 7965 6172 2773  ct on new year's
-00000730: 0d0a 2020 2020 2020 2065 7665 2069 6e20  ..       eve in 
-00000740: 616e 7920 7965 6172 2e20 596f 7520 6d61  any year. You ma
-00000750: 7920 7072 6566 6572 2027 2d65 2065 6f79  y prefer '-e eoy
-00000760: 2720 6f72 2027 2d65 2065 6e64 2d6f 662d  ' or '-e end-of-
-00000770: 7965 6172 2720 6966 2079 6f75 0d0a 2020  year' if you..  
-00000780: 2020 2020 2064 6f6e 2774 2077 616e 7420       don't want 
-00000790: 6120 6c61 6265 6c20 6c69 6b65 2027 6465  a label like 'de
-000007a0: 635f 3230 3130 2720 6f72 2027 6465 6327  c_2010' or 'dec'
-000007b0: 2e0d 0a0d 0a20 2020 202d 7720 2864 6566  .....    -w (def
-000007c0: 6175 6c74 2069 7320 3429 2044 6179 206e  ault is 4) Day n
-000007d0: 756d 6265 7220 6f66 2077 6565 6b6c 7920  umber of weekly 
-000007e0: 6261 636b 7570 732e 204d 6f6e 6461 7920  backups. Monday 
-000007f0: 6973 2030 2c20 5375 6e64 6179 2069 7320  is 0, Sunday is 
-00000800: 360d 0a0d 0a20 2020 202d 6820 286f 7220  6....    -h (or 
-00000810: 2d3f 2920 7368 6f77 7320 7468 6973 2068  -?) shows this h
-00000820: 656c 7020 7465 7874 2061 6e64 2074 6865  elp text and the
-00000830: 2064 6566 6175 6c74 206c 6162 656c 2066   default label f
-00000840: 6f72 2074 6f64 6179 202e 2e2e 0d0a 2020  or today .....  
-00000850: 2020                                       
+00000230: 6320 6469 7265 6374 6f72 7920 6f66 2074  c directory of t
+00000240: 6865 2062 616b 6c61 6265 6c20 7265 706f  he baklabel repo
+00000250: 2c20 7365 6520 7265 6c65 6173 655f 6e6f  , see release_no
+00000260: 7465 2e74 7874 2066 6f72 206d 6f72 6520  te.txt for more 
+00000270: 6465 7461 696c 206f 6e20 7468 650d 0a70  detail on the..p
+00000280: 6163 6b61 6765 2c20 6578 616d 706c 6573  ackage, examples
+00000290: 2e74 7874 2066 6f72 2062 616b 6c61 6265  .txt for baklabe
+000002a0: 6c20 6f75 7470 7574 2065 7861 6d70 6c65  l output example
+000002b0: 7320 616e 6420 6261 636b 7570 5f68 6f77  s and backup_how
+000002c0: 746f 2e74 7874 2066 6f72 2061 2073 616d  to.txt for a sam
+000002d0: 706c 650d 0a62 6163 6b75 7020 7363 7269  ple..backup scri
+000002e0: 7074 2066 6f72 2057 696e 646f 7773 2e0d  pt for Windows..
+000002f0: 0a0d 0a55 7361 6765 3a0d 0a20 2020 2062  ...Usage:..    b
+00000300: 616b 6c61 6265 6c2e 7079 205b 4f70 7469  aklabel.py [Opti
+00000310: 6f6e 735d 0d0a 0d0a 4f70 7469 6f6e 733a  ons]....Options:
+00000320: 0d0a 2020 2020 5769 7468 6f75 7420 6f70  ..    Without op
+00000330: 7469 6f6e 732c 2070 726f 6475 6365 2074  tions, produce t
+00000340: 6f64 6179 2773 2064 6566 6175 6c74 206c  oday's default l
+00000350: 6162 656c 2e20 4966 2074 6865 2063 7572  abel. If the cur
+00000360: 7265 6e74 2074 696d 6520 6973 0d0a 2020  rent time is..  
+00000370: 2020 7072 696f 7220 746f 2034 616d 2028    prior to 4am (
+00000380: 7377 6974 6368 6f76 6572 2074 696d 6529  switchover time)
+00000390: 2074 6865 6e20 7072 6f64 7563 6520 7965   then produce ye
+000003a0: 7374 6572 6461 7927 7320 6c61 6265 6c2e  sterday's label.
+000003b0: 0d0a 0d0a 2020 2020 2d64 2028 6465 6661  ....    -d (defa
+000003c0: 756c 7420 6461 7465 2069 7320 746f 6461  ult date is toda
+000003d0: 7929 204f 7220 7573 6520 6567 2e2c 2027  y) Or use eg., '
+000003e0: 2d64 2032 3031 302f 332f 3330 2720 6f72  -d 2010/3/30' or
+000003f0: 2027 2d64 2033 302d 332d 3230 3130 270d   '-d 30-3-2010'.
+00000400: 0a20 2020 2020 2020 5573 6520 2f20 6f72  .       Use / or
+00000410: 202d 2061 7320 6461 7465 2073 6570 6172   - as date separ
+00000420: 6174 6f72 732e 2044 6174 6520 666f 726d  ators. Date form
+00000430: 6174 2069 7320 6775 6573 7365 642e 204d  at is guessed. M
+00000440: 7468 2d64 6179 2d79 6561 720d 0a20 2020  th-day-year..   
+00000450: 2020 2020 6f6e 6c79 2077 6f72 6b73 2069      only works i
+00000460: 6620 6461 7920 3e20 3132 2e0d 0a0d 0a20  f day > 12..... 
+00000470: 2020 2020 2020 5573 6520 2d31 2066 6f72        Use -1 for
+00000480: 2079 6573 7465 7264 6179 2773 206c 6162   yesterday's lab
+00000490: 656c 206f 7220 2d37 2066 6f72 206c 6173  el or -7 for las
+000004a0: 7420 7765 656b 2773 206c 6162 656c 2e20  t week's label. 
+000004b0: 5573 6520 2b32 2066 6f72 0d0a 2020 2020  Use +2 for..    
+000004c0: 2020 2061 206c 6162 656c 2066 6f72 2074     a label for t
+000004d0: 6865 2064 6179 2061 6674 6572 2074 6f6d  he day after tom
+000004e0: 6f72 726f 772e 2041 6e79 206e 756d 6265  orrow. Any numbe
+000004f0: 7220 7769 6c6c 2062 6520 636f 6d70 7574  r will be comput
+00000500: 6564 2e0d 0a0d 0a20 2020 2020 2020 546f  ed.....       To
+00000510: 2061 646a 7573 7420 7468 6520 7377 6974   adjust the swit
+00000520: 6368 6f76 6572 2074 696d 6520 7573 6520  chover time use 
+00000530: 6567 2e2c 272d 6420 3661 6d27 206f 7220  eg.,'-d 6am' or 
+00000540: 272d 6420 3670 6d27 2065 7463 2e0d 0a0d  '-d 6pm' etc....
+00000550: 0a20 2020 202d 7320 2864 6566 6175 6c74  .    -s (default
+00000560: 2069 7320 626c 616e 6b29 2073 6572 7665   is blank) serve
+00000570: 7220 6e61 6d65 2075 7365 6420 746f 2070  r name used to p
+00000580: 7265 6669 7820 7468 6520 6261 636b 7570  refix the backup
+00000590: 206c 6162 656c 0d0a 0d0a 2020 2020 2d79   label....    -y
+000005a0: 2028 6465 6661 756c 7420 6973 2054 7275   (default is Tru
+000005b0: 6529 2041 7070 656e 6420 7965 6172 2074  e) Append year t
+000005c0: 6f20 656e 642d 6f66 2d79 6561 7220 6c61  o end-of-year la
+000005d0: 6265 6c2e 204f 7220 7573 6520 272d 7920  bel. Or use '-y 
+000005e0: 4661 6c73 6527 0d0a 2020 2020 2020 206f  False'..       o
+000005f0: 7220 272d 7920 4e6f 272e 2041 6e79 7468  r '-y No'. Anyth
+00000600: 696e 6720 656c 7365 206d 6561 6e73 2054  ing else means T
+00000610: 7275 652e 0d0a 0d0a 2020 2020 2d6d 2028  rue.....    -m (
+00000620: 6465 6661 756c 7420 6973 2046 616c 7365  default is False
+00000630: 2920 4170 7065 6e64 2079 6561 7220 746f  ) Append year to
+00000640: 2065 6e64 2d6f 662d 6d6f 6e74 6820 6c61   end-of-month la
+00000650: 6265 6c2e 204f 7220 7573 6520 272d 6d20  bel. Or use '-m 
+00000660: 5472 7565 270d 0a20 2020 2020 2020 6f72  True'..       or
+00000670: 2027 2d6d 2059 6573 272e 2041 6e79 7468   '-m Yes'. Anyth
+00000680: 696e 6720 656c 7365 206d 6561 6e73 2046  ing else means F
+00000690: 616c 7365 2e0d 0a0d 0a20 2020 202d 6e20  alse.....    -n 
+000006a0: 2864 6566 6175 6c74 2069 7320 3129 204d  (default is 1) M
+000006b0: 6f6e 7468 206e 756d 6265 7220 636f 6d6d  onth number comm
+000006c0: 656e 6369 6e67 2074 6865 206e 6577 2079  encing the new y
+000006d0: 6561 722e 204a 616e 7561 7279 2069 7320  ear. January is 
+000006e0: 312e 0d0a 0d0a 2020 2020 2d65 2028 6465  1.....    -e (de
+000006f0: 6661 756c 7420 6973 2027 626c 616e 6b27  fault is 'blank'
+00000700: 2920 656e 642d 6f66 2d79 6561 7220 6c61  ) end-of-year la
+00000710: 6265 6c20 6f6e 6c79 2068 6173 2061 6e20  bel only has an 
+00000720: 6566 6665 6374 206f 6e20 6e65 7720 7965  effect on new ye
+00000730: 6172 2773 0d0a 2020 2020 2020 2065 7665  ar's..       eve
+00000740: 2069 6e20 616e 7920 7965 6172 2e20 596f   in any year. Yo
+00000750: 7520 6d61 7920 7072 6566 6572 2027 2d65  u may prefer '-e
+00000760: 2065 6f79 2720 6f72 2027 2d65 2065 6e64   eoy' or '-e end
+00000770: 2d6f 662d 7965 6172 2720 6966 2079 6f75  -of-year' if you
+00000780: 0d0a 2020 2020 2020 2064 6f6e 2774 2077  ..       don't w
+00000790: 616e 7420 6120 6c61 6265 6c20 6c69 6b65  ant a label like
+000007a0: 2027 6465 635f 3230 3130 2720 6f72 2027   'dec_2010' or '
+000007b0: 6465 6327 2e0d 0a0d 0a20 2020 202d 7720  dec'.....    -w 
+000007c0: 2864 6566 6175 6c74 2069 7320 3429 2044  (default is 4) D
+000007d0: 6179 206e 756d 6265 7220 6f66 2077 6565  ay number of wee
+000007e0: 6b6c 7920 6261 636b 7570 732e 204d 6f6e  kly backups. Mon
+000007f0: 6461 7920 6973 2030 2c20 5375 6e64 6179  day is 0, Sunday
+00000800: 2069 7320 360d 0a0d 0a20 2020 202d 6820   is 6....    -h 
+00000810: 286f 7220 2d3f 2920 7368 6f77 7320 7468  (or -?) shows th
+00000820: 6973 2068 656c 7020 7465 7874 2061 6e64  is help text and
+00000830: 2074 6865 2064 6566 6175 6c74 206c 6162   the default lab
+00000840: 656c 2066 6f72 2074 6f64 6179 202e 2e2e  el for today ...
+00000850: 0d0a 2020 2020                           ..
```

### Comparing `baklabel-1.2.1/src/baklabel/baklabel.py` & `baklabel-1.2.2/src/baklabel/baklabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 It is also a stand-alone utility to find the backup label produced for any given date
 and set of options.
 
 python3 baklabel.py -h  to see command line usage and options.
 
 Python 3.x (Python 2.7 should also work but is no longer tested)
 
-In the doc directory after installing, see release_note.txt for more detail on the
+In the doc directory of the baklabel repo, see release_note.txt for more detail on the
 package, examples.txt for baklabel output examples and backup_howto.txt for a sample
 backup script for Windows.
 """
 
 longerdesc = """
 Properly grandfathered, there needs to be a daily backup to one of 23 separate tapes,
 sets of media or local directories on a storage device. This complement is made up of
@@ -40,14 +40,16 @@
 
 relnote = """baklabel - see Description below
 ========
 
 Version    Who  When/What
 =========================
 
+ver 1.2.2   md  1 Jun 2023 - Further clean up documentation
+
 ver 1.2.1   md  30 May 2023 - Clean up documentation
 
 ver 1.2.0   md  29 May 2023 - Improve guessdate() to resolve ambiguous dates
 
 ver 1.1.0   md  23 May 2023 - Change from GPL3 to MIT license, change to pyproject.toml
                 and clean up strings using f-strings
 
@@ -59,24 +61,24 @@
                 dates as a calling convenience
 
 ver 1.0.1   md  4 Nov 2010 - Minor refactoring and tidying comments
 
 ver 1.0.0   md  3 Nov 2010 - New option to append current year to any month-end label,
                 not just end-of-year.
 
-ver 0.2.0   md  27 oct 2010 - Help now respects defaults which have been adjusted in
+ver 0.2.0   md  27 Oct 2010 - Help now respects defaults which have been adjusted in
                 the source code. A new default now permits adjustment of new_year_month
                 which sets the end-of-year label to any desired month.
 
-ver 0.1.0b   md 8 oct 2010 - Added -d numeric option for setting the label to x days
+ver 0.1.0b   md 8 Oct 2010 - Added -d numeric option for setting the label to x days
                 ago. Eg., -1 = yesterday. Also added a time trigger option in the -d
                 switch such that, for example, -d 3am will produce yesterday's label
                 if baklabel is called prior to 3am
 
-ver 0.0.0a   md 1 jul 2010 - first written
+ver 0.0.0a   md 1 Jul 2010 - first written
 
 
 Description
 ==========={0}
 
 Grandfathered Backups
 ====================={1}
```

### Comparing `baklabel-1.2.1/src/baklabel/test_baklabel.py` & `baklabel-1.2.2/src/baklabel/test_baklabel.py`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.1/LICENSE` & `baklabel-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baklabel-1.2.1/README.md` & `baklabel-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 It is also a stand-alone utility to find the backup label produced for any given date
 and set of options.
 
 python3 baklabel.py -h  to see command line usage and options.
 
 Python 3.x (Python 2.7 should also work but is no longer tested)
 
-In the doc directory after installing, see release_note.txt for more detail on the
+In the doc directory of the baklabel repo, see release_note.txt for more detail on the
 package, examples.txt for baklabel output examples and backup_howto.txt for a sample
 backup script for Windows.
 
 
 Properly grandfathered, there needs to be a daily backup to one of 23 separate tapes,
 sets of media or local directories on a storage device. This complement is made up of
 6 weekday backups, 5 week-end backups, 11 month-end backups plus one for year-end.
```

### Comparing `baklabel-1.2.1/pyproject.toml` & `baklabel-1.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baklabel"
-version               = '1.2.1'
+version = '1.2.2'
 authors = [
   { name="Mike Dewhirst", email="miked@dewhirst.com.au" },
 ]
 description = "Baklabel delivers a daily label fragment for grandfathered backups"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `baklabel-1.2.1/PKG-INFO` & `baklabel-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baklabel
-Version: 1.2.1
+Version: 1.2.2
 Summary: Baklabel delivers a daily label fragment for grandfathered backups
 Project-URL: Homepage, https://svn.climate.com.au/repos/pysrc/foss/baklabel
 Author-email: Mike Dewhirst <miked@dewhirst.com.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 It is also a stand-alone utility to find the backup label produced for any given date
 and set of options.
 
 python3 baklabel.py -h  to see command line usage and options.
 
 Python 3.x (Python 2.7 should also work but is no longer tested)
 
-In the doc directory after installing, see release_note.txt for more detail on the
+In the doc directory of the baklabel repo, see release_note.txt for more detail on the
 package, examples.txt for baklabel output examples and backup_howto.txt for a sample
 backup script for Windows.
 
 
 Properly grandfathered, there needs to be a daily backup to one of 23 separate tapes,
 sets of media or local directories on a storage device. This complement is made up of
 6 weekday backups, 5 week-end backups, 11 month-end backups plus one for year-end.
```

