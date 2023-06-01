# Comparing `tmp/pakler-0.1.0.tar.gz` & `tmp/pakler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pakler-0.1.0.tar", last modified: Fri Sep  3 23:08:41 2021, max compression
+gzip compressed data, was "pakler-0.2.0.tar", last modified: Thu Jun  1 05:07:53 2023, max compression
```

## Comparing `pakler-0.1.0.tar` & `pakler-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxr-xr-x   0 vince      (502) staff       (20)        0 2021-09-03 23:08:41.518757 pakler-0.1.0/
--rw-r--r--   0 vince      (502) staff       (20)     3630 2021-09-03 20:41:14.000000 pakler-0.1.0/.gitignore
-drwxr-xr-x   0 vince      (502) staff       (20)        0 2021-09-03 23:08:41.516187 pakler-0.1.0/.idea/
--rw-r--r--   0 vince      (502) staff       (20)      176 2021-06-28 22:30:22.000000 pakler-0.1.0/.idea/.gitignore
--rw-r--r--   0 vince      (502) staff       (20)      191 2021-06-28 22:30:16.000000 pakler-0.1.0/.idea/encodings.xml
-drwxr-xr-x   0 vince      (502) staff       (20)        0 2021-09-03 23:08:41.516478 pakler-0.1.0/.idea/inspectionProfiles/
--rw-r--r--   0 vince      (502) staff       (20)      511 2021-09-03 21:35:33.000000 pakler-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 vince      (502) staff       (20)      297 2021-06-28 22:30:17.000000 pakler-0.1.0/.idea/misc.xml
--rw-r--r--   0 vince      (502) staff       (20)      252 2021-09-03 21:42:47.000000 pakler-0.1.0/.idea/modules.xml
--rw-r--r--   0 vince      (502) staff       (20)      167 2021-06-28 23:33:36.000000 pakler-0.1.0/.idea/vcs.xml
--rw-r--r--   0 vince      (502) staff       (20)     1071 2021-09-03 00:07:44.000000 pakler-0.1.0/LICENSE
--rw-r--r--   0 vince      (502) staff       (20)     8944 2021-09-03 23:08:41.518422 pakler-0.1.0/PKG-INFO
--rw-r--r--   0 vince      (502) staff       (20)     8456 2021-09-03 22:16:05.000000 pakler-0.1.0/README.md
--rw-r--r--   0 vince      (502) staff       (20)      142 2021-09-03 23:08:41.000000 pakler-0.1.0/_version.py
-drwxr-xr-x   0 vince      (502) staff       (20)        0 2021-09-03 23:08:41.518016 pakler-0.1.0/pakler.egg-info/
--rw-r--r--   0 vince      (502) staff       (20)     8944 2021-09-03 23:08:41.000000 pakler-0.1.0/pakler.egg-info/PKG-INFO
--rw-r--r--   0 vince      (502) staff       (20)      352 2021-09-03 23:08:41.000000 pakler-0.1.0/pakler.egg-info/SOURCES.txt
--rw-r--r--   0 vince      (502) staff       (20)        1 2021-09-03 23:08:41.000000 pakler-0.1.0/pakler.egg-info/dependency_links.txt
--rw-r--r--   0 vince      (502) staff       (20)       62 2021-09-03 23:08:41.000000 pakler-0.1.0/pakler.egg-info/entry_points.txt
--rw-r--r--   0 vince      (502) staff       (20)       16 2021-09-03 23:08:41.000000 pakler-0.1.0/pakler.egg-info/top_level.txt
--rw-r--r--   0 vince      (502) staff       (20)      338 2021-09-03 21:42:47.000000 pakler-0.1.0/pakler.iml
--rwxr-xr-x   0 vince      (502) staff       (20)    18250 2021-09-03 23:02:11.000000 pakler-0.1.0/pakler.py
--rw-r--r--   0 vince      (502) staff       (20)       38 2021-09-03 23:08:41.518860 pakler-0.1.0/setup.cfg
--rw-r--r--   0 vince      (502) staff       (20)      944 2021-09-03 21:35:33.000000 pakler-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:07:53.691187 pakler-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 05:07:39.000000 pakler-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 05:07:39.000000 pakler-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-06-01 05:07:53.691187 pakler-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-06-01 05:07:39.000000 pakler-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:07:53.687186 pakler-0.2.0/pakler/
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-06-01 05:07:39.000000 pakler-0.2.0/pakler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-01 05:07:39.000000 pakler-0.2.0/pakler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 05:07:53.000000 pakler-0.2.0/pakler/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:07:53.691187 pakler-0.2.0/pakler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-06-01 05:07:53.000000 pakler-0.2.0/pakler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 05:07:53.000000 pakler-0.2.0/pakler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 05:07:53.000000 pakler-0.2.0/pakler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 05:07:53.000000 pakler-0.2.0/pakler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 05:07:53.000000 pakler-0.2.0/pakler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-01 05:07:39.000000 pakler-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 05:07:53.691187 pakler-0.2.0/setup.cfg
```

### Comparing `pakler-0.1.0/LICENSE` & `pakler-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pakler-0.1.0/PKG-INFO` & `pakler-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,17 @@
-Metadata-Version: 2.1
-Name: pakler
-Version: 0.1.0
-Summary: Manipulate .PAK firmware files from Swann and Reolink
-Home-page: https://github.com/vmallet/pakler
-Author: Vincent Mallet
-Author-email: vmallet@gmail.com
-License: MIT License
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pakler
 
-Pakler is a command-line tool used to manipulate `.pak` firmware files
+Pakler is a command-line tool and library used to manipulate `.pak` firmware files
 used by Swann and Reolink devices. You can list, extract, and replace their
 content. It makes it easy to explore and patch firmwares used by various
 NVRs, DVRs and IP cameras.
 
 ## Installing
 
-Note: pakler requires Python 3
+Note: pakler requires Python 3.6+
 
 ### Recommended
 
 ```shell
 pip install pakler
 ```
 
@@ -48,46 +32,47 @@
  * [replace content](#replacing-content-of-pak-files): `pakler file.pak -r -n ... -f ... -o newfile.pak`
 
 Help can be had with:
 ```shell
 pakler -h
 ```
 
+Note: list and extract also work with ZIPs that contain `.pak` files.
+
 ### Viewing content of `.pak` files
 
 Listing the contents of a `.pak` file is pretty straightforward: invoke the
 tool with the name of the firmware file on the command line.
 
 ```shell
 pakler NVR8-7400_1705_3438_1103.pak
 ```
 
 ```
-Attempting to guess number of sections... guessed: 10
 Header  magic=32725913  crc32=0250e72d  type=00002302  sections=<10>  mtd_parts=<10>
-    Section  0 name="uboot1"         version="v1.0.0.1"       start=00000584  len=000437d0  (start=    1412 len=  276432)
-    Section  1 name=""               version=""               start=00043d54  len=00000000  (start=  277844 len=       0)
-    Section  2 name="bootargs"       version="v1.0.0.1"       start=00043d54  len=00020000  (start=  277844 len=  131072)
-    Section  3 name="kernel"         version="v1.0.0.1"       start=00063d54  len=0023fdc8  (start=  408916 len= 2358728)
-    Section  4 name="fs"             version="v1.0.0.442"     start=002a3b1c  len=00402000  (start= 2767644 len= 4202496)
-    Section  5 name="app"            version="v1.0.0.421"     start=006a5b1c  len=00947000  (start= 6970140 len= 9728000)
-    Section  6 name=""               version=""               start=00fecb1c  len=00000000  (start=16698140 len=       0)
-    Section  7 name="logo"           version="v1.0.0.1"       start=00fecb1c  len=0000f1fd  (start=16698140 len=   61949)
-    Section  8 name=""               version=""               start=00ffbd19  len=00000000  (start=16760089 len=       0)
-    Section  9 name=""               version=""               start=00ffbd19  len=00000000  (start=16760089 len=       0)
-    Mtd_part name="uboot1"         mtd="/dev/mtd9"       a=00000000  start=00000000  len=00080000
-    Mtd_part name="uboot2"         mtd="/dev/mtd9"       a=00080000  start=00080000  len=001e0000
-    Mtd_part name="bootargs"       mtd="/dev/mtd9"       a=00260000  start=00260000  len=00020000
-    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=00280000  start=00280000  len=00440000
-    Mtd_part name="fs"             mtd="/dev/mtd9"       a=006c0000  start=006c0000  len=00c00000
-    Mtd_part name="app"            mtd="/dev/mtd9"       a=012c0000  start=012c0000  len=02000000
-    Mtd_part name="para"           mtd="/dev/mtd9"       a=032c0000  start=032c0000  len=00800000
-    Mtd_part name="logo"           mtd="/dev/mtd9"       a=03ac0000  start=03ac0000  len=00200000
-    Mtd_part name="ipc_img"        mtd="/dev/mtd9"       a=03cc0000  start=03cc0000  len=00b00000
-    Mtd_part name="version"        mtd="/dev/mtd9"       a=ffffffff  start=ffffffff  len=00000000
+    Section  0 name="uboot1"         version="v1.0.0.1"       start=0x00000584  len=0x000437d0  (start=    1412 len=  276432)
+    Section  1 name=""               version=""               start=0x00043d54  len=0x00000000  (start=  277844 len=       0)
+    Section  2 name="bootargs"       version="v1.0.0.1"       start=0x00043d54  len=0x00020000  (start=  277844 len=  131072)
+    Section  3 name="kernel"         version="v1.0.0.1"       start=0x00063d54  len=0x0023fdc8  (start=  408916 len= 2358728)
+    Section  4 name="fs"             version="v1.0.0.442"     start=0x002a3b1c  len=0x00402000  (start= 2767644 len= 4202496)
+    Section  5 name="app"            version="v1.0.0.421"     start=0x006a5b1c  len=0x00947000  (start= 6970140 len= 9728000)
+    Section  6 name=""               version=""               start=0x00fecb1c  len=0x00000000  (start=16698140 len=       0)
+    Section  7 name="logo"           version="v1.0.0.1"       start=0x00fecb1c  len=0x0000f1fd  (start=16698140 len=   61949)
+    Section  8 name=""               version=""               start=0x00ffbd19  len=0x00000000  (start=16760089 len=       0)
+    Section  9 name=""               version=""               start=0x00ffbd19  len=0x00000000  (start=16760089 len=       0)
+    Mtd_part name="uboot1"         mtd="/dev/mtd9"       a=0x00000000  start=0x00000000  len=0x00080000
+    Mtd_part name="uboot2"         mtd="/dev/mtd9"       a=0x00080000  start=0x00080000  len=0x001e0000
+    Mtd_part name="bootargs"       mtd="/dev/mtd9"       a=0x00260000  start=0x00260000  len=0x00020000
+    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=0x00280000  start=0x00280000  len=0x00440000
+    Mtd_part name="fs"             mtd="/dev/mtd9"       a=0x006c0000  start=0x006c0000  len=0x00c00000
+    Mtd_part name="app"            mtd="/dev/mtd9"       a=0x012c0000  start=0x012c0000  len=0x02000000
+    Mtd_part name="para"           mtd="/dev/mtd9"       a=0x032c0000  start=0x032c0000  len=0x00800000
+    Mtd_part name="logo"           mtd="/dev/mtd9"       a=0x03ac0000  start=0x03ac0000  len=0x00200000
+    Mtd_part name="ipc_img"        mtd="/dev/mtd9"       a=0x03cc0000  start=0x03cc0000  len=0x00b00000
+    Mtd_part name="version"        mtd="/dev/mtd9"       a=0xffffffff  start=0xffffffff  len=0x00000000
 File passes CRC check: NVR8-7400_1705_3438_1103.pak
 ```
 
 ### Extracting content of `.pak` files
 
 Contents of a `.pak` file can be extracted using the `-e` command. If no
 output directory is specified using the `-d` parameter, a default unique
@@ -95,15 +80,14 @@
 the `.pak` file.
 
 example:
 ```shell
 pakler ./NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak -e -d newdir
 ```
 ```
-Attempting to guess number of sections... guessed: 11
 output: newdir
 Extracting section 0 (131072 bytes) into newdir/00_header.bin
 Extracting section 1 (18096 bytes) into newdir/01_loader.bin
 Extracting section 2 (26404 bytes) into newdir/02_fdt.bin
 Extracting section 3 (414552 bytes) into newdir/03_uboot.bin
 Extracting section 4 (3022896 bytes) into newdir/04_kernel.bin
 Extracting section 5 (12210176 bytes) into newdir/05_fs.bin
@@ -118,23 +102,22 @@
 
 A `.pak` file is made up of multiple sections, and at the moment you can
 replace only one section at a time. To replace a section you need to 
 use the `-r` command, specify the number of the section to replace with `-n`,
 the file to use as a replacement with `-f`, and the output file to write
 the resulting patched file with `-o`.
 
-Here is an example where we replace the `.pak` file's section #3 with the
-file ""
+Here is an example where we replace the `.pak` file's section #5 with the
+file `patched_fs.bin`
 
 ```shell
 pakler NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak -r -n 5 -f patched_fs.bin -o patched_fw.pak
 ````
 
 ```
-Attempting to guess number of sections... guessed: 11
 Input            : NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak
 Output           : patched_fw.pak
 Replacing section: 5
 Replacement file : new_fs.bin
 Copying section 0 (131072 bytes)
 Copying section 1 (18096 bytes)
 Copying section 2 (26404 bytes)
@@ -146,42 +129,67 @@
 Copying section 8 (122036 bytes)
 Copying section 9 (0 bytes)
 Copying section 10 (0 bytes)
 Writing header... (1552 bytes)
 Updating CRC...
 Replacement completed. New header:
 Header  magic=32725913  crc32=41ee801c  type=00006202  sections=<11>  mtd_parts=<11>
-    Section  0 name="header"         version="v1.0.0.0"       start=00000610  len=00020000  (start=    1552 len=  131072)
-    Section  1 name="loader"         version="v1.0.0.0"       start=00020610  len=000046b0  (start=  132624 len=   18096)
-    Section  2 name="fdt"            version="v1.0.0.0"       start=00024cc0  len=00006724  (start=  150720 len=   26404)
-    Section  3 name="uboot"          version="v1.0.0.0"       start=0002b3e4  len=00065358  (start=  177124 len=  414552)
-    Section  4 name="kernel"         version="v1.0.0.0"       start=0009073c  len=002e2030  (start=  591676 len= 3022896)
-    Section  5 name="fs"             version="v1.0.0.0"       start=0037276c  len=00ba557a  (start= 3614572 len=12211578)
-    Section  6 name="app"            version="v1.0.0.0"       start=00f17ce6  len=01052000  (start=15826150 len=17113088)
-    Section  7 name=""               version=""               start=01f69ce6  len=00000000  (start=32939238 len=       0)
-    Section  8 name="logo"           version="v1.0.0.0"       start=01f69ce6  len=0001dcb4  (start=32939238 len=  122036)
-    Section  9 name=""               version=""               start=01f8799a  len=00000000  (start=33061274 len=       0)
-    Section 10 name=""               version=""               start=01f8799a  len=00000000  (start=33061274 len=       0)
-    Mtd_part name="header"         mtd="/dev/mtd9"       a=00000000  start=00000000  len=00020000
-    Mtd_part name="loader"         mtd="/dev/mtd9"       a=00020000  start=00020000  len=00080000
-    Mtd_part name="fdt"            mtd="/dev/mtd9"       a=000a0000  start=000a0000  len=00080000
-    Mtd_part name="uboot"          mtd="/dev/mtd9"       a=00120000  start=00120000  len=000e0000
-    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=00200000  start=00200000  len=00500000
-    Mtd_part name="fs"             mtd="/dev/mtd9"       a=00700000  start=00700000  len=00f00000
-    Mtd_part name="app"            mtd="/dev/mtd9"       a=01600000  start=01600000  len=02000000
-    Mtd_part name="para"           mtd="/dev/mtd9"       a=03600000  start=03600000  len=00800000
-    Mtd_part name="logo"           mtd="/dev/mtd9"       a=03e00000  start=03e00000  len=00100000
-    Mtd_part name="uid"            mtd="/dev/mtd9"       a=03f00000  start=03f00000  len=00100000
-    Mtd_part name="version"        mtd="/dev/mtd9"       a=ffffffff  start=ffffffff  len=00000000
+    Section  0 name="header"         version="v1.0.0.0"       start=0x00000610  len=0x00020000  (start=    1552 len=  131072)
+    Section  1 name="loader"         version="v1.0.0.0"       start=0x00020610  len=0x000046b0  (start=  132624 len=   18096)
+    Section  2 name="fdt"            version="v1.0.0.0"       start=0x00024cc0  len=0x00006724  (start=  150720 len=   26404)
+    Section  3 name="uboot"          version="v1.0.0.0"       start=0x0002b3e4  len=0x00065358  (start=  177124 len=  414552)
+    Section  4 name="kernel"         version="v1.0.0.0"       start=0x0009073c  len=0x002e2030  (start=  591676 len= 3022896)
+    Section  5 name="fs"             version="v1.0.0.0"       start=0x0037276c  len=0x00ba557a  (start= 3614572 len=12211578)
+    Section  6 name="app"            version="v1.0.0.0"       start=0x00f17ce6  len=0x01052000  (start=15826150 len=17113088)
+    Section  7 name=""               version=""               start=0x01f69ce6  len=0x00000000  (start=32939238 len=       0)
+    Section  8 name="logo"           version="v1.0.0.0"       start=0x01f69ce6  len=0x0001dcb4  (start=32939238 len=  122036)
+    Section  9 name=""               version=""               start=0x01f8799a  len=0x00000000  (start=33061274 len=       0)
+    Section 10 name=""               version=""               start=0x01f8799a  len=0x00000000  (start=33061274 len=       0)
+    Mtd_part name="header"         mtd="/dev/mtd9"       a=0x00000000  start=0x00000000  len=0x00020000
+    Mtd_part name="loader"         mtd="/dev/mtd9"       a=0x00020000  start=0x00020000  len=0x00080000
+    Mtd_part name="fdt"            mtd="/dev/mtd9"       a=0x000a0000  start=0x000a0000  len=0x00080000
+    Mtd_part name="uboot"          mtd="/dev/mtd9"       a=0x00120000  start=0x00120000  len=0x000e0000
+    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=0x00200000  start=0x00200000  len=0x00500000
+    Mtd_part name="fs"             mtd="/dev/mtd9"       a=0x00700000  start=0x00700000  len=0x00f00000
+    Mtd_part name="app"            mtd="/dev/mtd9"       a=0x01600000  start=0x01600000  len=0x02000000
+    Mtd_part name="para"           mtd="/dev/mtd9"       a=0x03600000  start=0x03600000  len=0x00800000
+    Mtd_part name="logo"           mtd="/dev/mtd9"       a=0x03e00000  start=0x03e00000  len=0x00100000
+    Mtd_part name="uid"            mtd="/dev/mtd9"       a=0x03f00000  start=0x03f00000  len=0x00100000
+    Mtd_part name="version"        mtd="/dev/mtd9"       a=0xffffffff  start=0xffffffff  len=0x00000000
+```
+
+### As a library
+
+Here are a few things you can do with pakler's API:
+
+```py
+from pakler import PAK
+
+with PAK.from_file("firmware.pak") as pak:  # Also from_bytes() and from_fd()
+    assert pak.crc == pak.calc_crc()
+    pak.extract("firmware_extracted")
+    print(pak.partitions)
+    section = pak.sections[0]
+    pak.save_section(section, f"{section.name}.bin")
+    section_bytes = pak.extract_section(section)
 ```
 
-
 ## Naming
 
 Why pakler? Take a **pak** and **L**ist it, **E**xtract it, or **R**eplace 
 parts of it... pakler? Makes sense! (Naming suggestions are welcome :) )
 
-## Licensing
+## Version history
 
-pakler is licensed under MIT license. See [LICENSE](LICENSE)
+* v0.2.0 - 2023/05/31 - The [AT0myks](https://github.com/AT0myks) release
+  
+  A big thanks to AT0myks for all the changes brought in this release.
+  - Make Pakler usable as a library (author: AT0myks)
+  - Support for 64-bit PAK files (author: AT0myks)
+  - Support for handling PAK files directly from ZIP archives (author: AT0myks)
+  - Several code layout and packaging improvements (author: AT0myks)
+
+* v0.1.0 - 2021/09/03 - Initial release
 
+## Licensing
 
+pakler is licensed under MIT license. See [LICENSE](LICENSE)
```

### Comparing `pakler-0.1.0/README.md` & `pakler-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,46 @@
+Metadata-Version: 2.1
+Name: pakler
+Version: 0.2.0
+Summary: Manipulate .PAK firmware files from Swann and Reolink
+Author-email: Vincent Mallet <vmallet@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/vmallet/pakler
+Project-URL: Issues, https://github.com/vmallet/pakler/issues
+Keywords: swann,reolink,firmware,pak
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pakler
 
-Pakler is a command-line tool used to manipulate `.pak` firmware files
+Pakler is a command-line tool and library used to manipulate `.pak` firmware files
 used by Swann and Reolink devices. You can list, extract, and replace their
 content. It makes it easy to explore and patch firmwares used by various
 NVRs, DVRs and IP cameras.
 
 ## Installing
 
-Note: pakler requires Python 3
+Note: pakler requires Python 3.6+
 
 ### Recommended
 
 ```shell
 pip install pakler
 ```
 
@@ -32,46 +61,47 @@
  * [replace content](#replacing-content-of-pak-files): `pakler file.pak -r -n ... -f ... -o newfile.pak`
 
 Help can be had with:
 ```shell
 pakler -h
 ```
 
+Note: list and extract also work with ZIPs that contain `.pak` files.
+
 ### Viewing content of `.pak` files
 
 Listing the contents of a `.pak` file is pretty straightforward: invoke the
 tool with the name of the firmware file on the command line.
 
 ```shell
 pakler NVR8-7400_1705_3438_1103.pak
 ```
 
 ```
-Attempting to guess number of sections... guessed: 10
 Header  magic=32725913  crc32=0250e72d  type=00002302  sections=<10>  mtd_parts=<10>
-    Section  0 name="uboot1"         version="v1.0.0.1"       start=00000584  len=000437d0  (start=    1412 len=  276432)
-    Section  1 name=""               version=""               start=00043d54  len=00000000  (start=  277844 len=       0)
-    Section  2 name="bootargs"       version="v1.0.0.1"       start=00043d54  len=00020000  (start=  277844 len=  131072)
-    Section  3 name="kernel"         version="v1.0.0.1"       start=00063d54  len=0023fdc8  (start=  408916 len= 2358728)
-    Section  4 name="fs"             version="v1.0.0.442"     start=002a3b1c  len=00402000  (start= 2767644 len= 4202496)
-    Section  5 name="app"            version="v1.0.0.421"     start=006a5b1c  len=00947000  (start= 6970140 len= 9728000)
-    Section  6 name=""               version=""               start=00fecb1c  len=00000000  (start=16698140 len=       0)
-    Section  7 name="logo"           version="v1.0.0.1"       start=00fecb1c  len=0000f1fd  (start=16698140 len=   61949)
-    Section  8 name=""               version=""               start=00ffbd19  len=00000000  (start=16760089 len=       0)
-    Section  9 name=""               version=""               start=00ffbd19  len=00000000  (start=16760089 len=       0)
-    Mtd_part name="uboot1"         mtd="/dev/mtd9"       a=00000000  start=00000000  len=00080000
-    Mtd_part name="uboot2"         mtd="/dev/mtd9"       a=00080000  start=00080000  len=001e0000
-    Mtd_part name="bootargs"       mtd="/dev/mtd9"       a=00260000  start=00260000  len=00020000
-    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=00280000  start=00280000  len=00440000
-    Mtd_part name="fs"             mtd="/dev/mtd9"       a=006c0000  start=006c0000  len=00c00000
-    Mtd_part name="app"            mtd="/dev/mtd9"       a=012c0000  start=012c0000  len=02000000
-    Mtd_part name="para"           mtd="/dev/mtd9"       a=032c0000  start=032c0000  len=00800000
-    Mtd_part name="logo"           mtd="/dev/mtd9"       a=03ac0000  start=03ac0000  len=00200000
-    Mtd_part name="ipc_img"        mtd="/dev/mtd9"       a=03cc0000  start=03cc0000  len=00b00000
-    Mtd_part name="version"        mtd="/dev/mtd9"       a=ffffffff  start=ffffffff  len=00000000
+    Section  0 name="uboot1"         version="v1.0.0.1"       start=0x00000584  len=0x000437d0  (start=    1412 len=  276432)
+    Section  1 name=""               version=""               start=0x00043d54  len=0x00000000  (start=  277844 len=       0)
+    Section  2 name="bootargs"       version="v1.0.0.1"       start=0x00043d54  len=0x00020000  (start=  277844 len=  131072)
+    Section  3 name="kernel"         version="v1.0.0.1"       start=0x00063d54  len=0x0023fdc8  (start=  408916 len= 2358728)
+    Section  4 name="fs"             version="v1.0.0.442"     start=0x002a3b1c  len=0x00402000  (start= 2767644 len= 4202496)
+    Section  5 name="app"            version="v1.0.0.421"     start=0x006a5b1c  len=0x00947000  (start= 6970140 len= 9728000)
+    Section  6 name=""               version=""               start=0x00fecb1c  len=0x00000000  (start=16698140 len=       0)
+    Section  7 name="logo"           version="v1.0.0.1"       start=0x00fecb1c  len=0x0000f1fd  (start=16698140 len=   61949)
+    Section  8 name=""               version=""               start=0x00ffbd19  len=0x00000000  (start=16760089 len=       0)
+    Section  9 name=""               version=""               start=0x00ffbd19  len=0x00000000  (start=16760089 len=       0)
+    Mtd_part name="uboot1"         mtd="/dev/mtd9"       a=0x00000000  start=0x00000000  len=0x00080000
+    Mtd_part name="uboot2"         mtd="/dev/mtd9"       a=0x00080000  start=0x00080000  len=0x001e0000
+    Mtd_part name="bootargs"       mtd="/dev/mtd9"       a=0x00260000  start=0x00260000  len=0x00020000
+    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=0x00280000  start=0x00280000  len=0x00440000
+    Mtd_part name="fs"             mtd="/dev/mtd9"       a=0x006c0000  start=0x006c0000  len=0x00c00000
+    Mtd_part name="app"            mtd="/dev/mtd9"       a=0x012c0000  start=0x012c0000  len=0x02000000
+    Mtd_part name="para"           mtd="/dev/mtd9"       a=0x032c0000  start=0x032c0000  len=0x00800000
+    Mtd_part name="logo"           mtd="/dev/mtd9"       a=0x03ac0000  start=0x03ac0000  len=0x00200000
+    Mtd_part name="ipc_img"        mtd="/dev/mtd9"       a=0x03cc0000  start=0x03cc0000  len=0x00b00000
+    Mtd_part name="version"        mtd="/dev/mtd9"       a=0xffffffff  start=0xffffffff  len=0x00000000
 File passes CRC check: NVR8-7400_1705_3438_1103.pak
 ```
 
 ### Extracting content of `.pak` files
 
 Contents of a `.pak` file can be extracted using the `-e` command. If no
 output directory is specified using the `-d` parameter, a default unique
@@ -79,15 +109,14 @@
 the `.pak` file.
 
 example:
 ```shell
 pakler ./NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak -e -d newdir
 ```
 ```
-Attempting to guess number of sections... guessed: 11
 output: newdir
 Extracting section 0 (131072 bytes) into newdir/00_header.bin
 Extracting section 1 (18096 bytes) into newdir/01_loader.bin
 Extracting section 2 (26404 bytes) into newdir/02_fdt.bin
 Extracting section 3 (414552 bytes) into newdir/03_uboot.bin
 Extracting section 4 (3022896 bytes) into newdir/04_kernel.bin
 Extracting section 5 (12210176 bytes) into newdir/05_fs.bin
@@ -102,23 +131,22 @@
 
 A `.pak` file is made up of multiple sections, and at the moment you can
 replace only one section at a time. To replace a section you need to 
 use the `-r` command, specify the number of the section to replace with `-n`,
 the file to use as a replacement with `-f`, and the output file to write
 the resulting patched file with `-o`.
 
-Here is an example where we replace the `.pak` file's section #3 with the
-file ""
+Here is an example where we replace the `.pak` file's section #5 with the
+file `patched_fs.bin`
 
 ```shell
 pakler NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak -r -n 5 -f patched_fs.bin -o patched_fw.pak
 ````
 
 ```
-Attempting to guess number of sections... guessed: 11
 Input            : NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak
 Output           : patched_fw.pak
 Replacing section: 5
 Replacement file : new_fs.bin
 Copying section 0 (131072 bytes)
 Copying section 1 (18096 bytes)
 Copying section 2 (26404 bytes)
@@ -130,40 +158,67 @@
 Copying section 8 (122036 bytes)
 Copying section 9 (0 bytes)
 Copying section 10 (0 bytes)
 Writing header... (1552 bytes)
 Updating CRC...
 Replacement completed. New header:
 Header  magic=32725913  crc32=41ee801c  type=00006202  sections=<11>  mtd_parts=<11>
-    Section  0 name="header"         version="v1.0.0.0"       start=00000610  len=00020000  (start=    1552 len=  131072)
-    Section  1 name="loader"         version="v1.0.0.0"       start=00020610  len=000046b0  (start=  132624 len=   18096)
-    Section  2 name="fdt"            version="v1.0.0.0"       start=00024cc0  len=00006724  (start=  150720 len=   26404)
-    Section  3 name="uboot"          version="v1.0.0.0"       start=0002b3e4  len=00065358  (start=  177124 len=  414552)
-    Section  4 name="kernel"         version="v1.0.0.0"       start=0009073c  len=002e2030  (start=  591676 len= 3022896)
-    Section  5 name="fs"             version="v1.0.0.0"       start=0037276c  len=00ba557a  (start= 3614572 len=12211578)
-    Section  6 name="app"            version="v1.0.0.0"       start=00f17ce6  len=01052000  (start=15826150 len=17113088)
-    Section  7 name=""               version=""               start=01f69ce6  len=00000000  (start=32939238 len=       0)
-    Section  8 name="logo"           version="v1.0.0.0"       start=01f69ce6  len=0001dcb4  (start=32939238 len=  122036)
-    Section  9 name=""               version=""               start=01f8799a  len=00000000  (start=33061274 len=       0)
-    Section 10 name=""               version=""               start=01f8799a  len=00000000  (start=33061274 len=       0)
-    Mtd_part name="header"         mtd="/dev/mtd9"       a=00000000  start=00000000  len=00020000
-    Mtd_part name="loader"         mtd="/dev/mtd9"       a=00020000  start=00020000  len=00080000
-    Mtd_part name="fdt"            mtd="/dev/mtd9"       a=000a0000  start=000a0000  len=00080000
-    Mtd_part name="uboot"          mtd="/dev/mtd9"       a=00120000  start=00120000  len=000e0000
-    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=00200000  start=00200000  len=00500000
-    Mtd_part name="fs"             mtd="/dev/mtd9"       a=00700000  start=00700000  len=00f00000
-    Mtd_part name="app"            mtd="/dev/mtd9"       a=01600000  start=01600000  len=02000000
-    Mtd_part name="para"           mtd="/dev/mtd9"       a=03600000  start=03600000  len=00800000
-    Mtd_part name="logo"           mtd="/dev/mtd9"       a=03e00000  start=03e00000  len=00100000
-    Mtd_part name="uid"            mtd="/dev/mtd9"       a=03f00000  start=03f00000  len=00100000
-    Mtd_part name="version"        mtd="/dev/mtd9"       a=ffffffff  start=ffffffff  len=00000000
+    Section  0 name="header"         version="v1.0.0.0"       start=0x00000610  len=0x00020000  (start=    1552 len=  131072)
+    Section  1 name="loader"         version="v1.0.0.0"       start=0x00020610  len=0x000046b0  (start=  132624 len=   18096)
+    Section  2 name="fdt"            version="v1.0.0.0"       start=0x00024cc0  len=0x00006724  (start=  150720 len=   26404)
+    Section  3 name="uboot"          version="v1.0.0.0"       start=0x0002b3e4  len=0x00065358  (start=  177124 len=  414552)
+    Section  4 name="kernel"         version="v1.0.0.0"       start=0x0009073c  len=0x002e2030  (start=  591676 len= 3022896)
+    Section  5 name="fs"             version="v1.0.0.0"       start=0x0037276c  len=0x00ba557a  (start= 3614572 len=12211578)
+    Section  6 name="app"            version="v1.0.0.0"       start=0x00f17ce6  len=0x01052000  (start=15826150 len=17113088)
+    Section  7 name=""               version=""               start=0x01f69ce6  len=0x00000000  (start=32939238 len=       0)
+    Section  8 name="logo"           version="v1.0.0.0"       start=0x01f69ce6  len=0x0001dcb4  (start=32939238 len=  122036)
+    Section  9 name=""               version=""               start=0x01f8799a  len=0x00000000  (start=33061274 len=       0)
+    Section 10 name=""               version=""               start=0x01f8799a  len=0x00000000  (start=33061274 len=       0)
+    Mtd_part name="header"         mtd="/dev/mtd9"       a=0x00000000  start=0x00000000  len=0x00020000
+    Mtd_part name="loader"         mtd="/dev/mtd9"       a=0x00020000  start=0x00020000  len=0x00080000
+    Mtd_part name="fdt"            mtd="/dev/mtd9"       a=0x000a0000  start=0x000a0000  len=0x00080000
+    Mtd_part name="uboot"          mtd="/dev/mtd9"       a=0x00120000  start=0x00120000  len=0x000e0000
+    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=0x00200000  start=0x00200000  len=0x00500000
+    Mtd_part name="fs"             mtd="/dev/mtd9"       a=0x00700000  start=0x00700000  len=0x00f00000
+    Mtd_part name="app"            mtd="/dev/mtd9"       a=0x01600000  start=0x01600000  len=0x02000000
+    Mtd_part name="para"           mtd="/dev/mtd9"       a=0x03600000  start=0x03600000  len=0x00800000
+    Mtd_part name="logo"           mtd="/dev/mtd9"       a=0x03e00000  start=0x03e00000  len=0x00100000
+    Mtd_part name="uid"            mtd="/dev/mtd9"       a=0x03f00000  start=0x03f00000  len=0x00100000
+    Mtd_part name="version"        mtd="/dev/mtd9"       a=0xffffffff  start=0xffffffff  len=0x00000000
+```
+
+### As a library
+
+Here are a few things you can do with pakler's API:
+
+```py
+from pakler import PAK
+
+with PAK.from_file("firmware.pak") as pak:  # Also from_bytes() and from_fd()
+    assert pak.crc == pak.calc_crc()
+    pak.extract("firmware_extracted")
+    print(pak.partitions)
+    section = pak.sections[0]
+    pak.save_section(section, f"{section.name}.bin")
+    section_bytes = pak.extract_section(section)
 ```
 
-
 ## Naming
 
 Why pakler? Take a **pak** and **L**ist it, **E**xtract it, or **R**eplace 
 parts of it... pakler? Makes sense! (Naming suggestions are welcome :) )
 
+## Version history
+
+* v0.2.0 - 2023/05/31 - The [AT0myks](https://github.com/AT0myks) release
+  
+  A big thanks to AT0myks for all the changes brought in this release.
+  - Make Pakler usable as a library (author: AT0myks)
+  - Support for 64-bit PAK files (author: AT0myks)
+  - Support for handling PAK files directly from ZIP archives (author: AT0myks)
+  - Several code layout and packaging improvements (author: AT0myks)
+
+* v0.1.0 - 2021/09/03 - Initial release
+
 ## Licensing
 
 pakler is licensed under MIT license. See [LICENSE](LICENSE)
```

### Comparing `pakler-0.1.0/pakler.egg-info/PKG-INFO` & `pakler-0.2.0/pakler.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 Metadata-Version: 2.1
 Name: pakler
-Version: 0.1.0
+Version: 0.2.0
 Summary: Manipulate .PAK firmware files from Swann and Reolink
-Home-page: https://github.com/vmallet/pakler
-Author: Vincent Mallet
-Author-email: vmallet@gmail.com
+Author-email: Vincent Mallet <vmallet@gmail.com>
 License: MIT License
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/vmallet/pakler
+Project-URL: Issues, https://github.com/vmallet/pakler/issues
+Keywords: swann,reolink,firmware,pak
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pakler
 
-Pakler is a command-line tool used to manipulate `.pak` firmware files
+Pakler is a command-line tool and library used to manipulate `.pak` firmware files
 used by Swann and Reolink devices. You can list, extract, and replace their
 content. It makes it easy to explore and patch firmwares used by various
 NVRs, DVRs and IP cameras.
 
 ## Installing
 
-Note: pakler requires Python 3
+Note: pakler requires Python 3.6+
 
 ### Recommended
 
 ```shell
 pip install pakler
 ```
 
@@ -48,46 +61,47 @@
  * [replace content](#replacing-content-of-pak-files): `pakler file.pak -r -n ... -f ... -o newfile.pak`
 
 Help can be had with:
 ```shell
 pakler -h
 ```
 
+Note: list and extract also work with ZIPs that contain `.pak` files.
+
 ### Viewing content of `.pak` files
 
 Listing the contents of a `.pak` file is pretty straightforward: invoke the
 tool with the name of the firmware file on the command line.
 
 ```shell
 pakler NVR8-7400_1705_3438_1103.pak
 ```
 
 ```
-Attempting to guess number of sections... guessed: 10
 Header  magic=32725913  crc32=0250e72d  type=00002302  sections=<10>  mtd_parts=<10>
-    Section  0 name="uboot1"         version="v1.0.0.1"       start=00000584  len=000437d0  (start=    1412 len=  276432)
-    Section  1 name=""               version=""               start=00043d54  len=00000000  (start=  277844 len=       0)
-    Section  2 name="bootargs"       version="v1.0.0.1"       start=00043d54  len=00020000  (start=  277844 len=  131072)
-    Section  3 name="kernel"         version="v1.0.0.1"       start=00063d54  len=0023fdc8  (start=  408916 len= 2358728)
-    Section  4 name="fs"             version="v1.0.0.442"     start=002a3b1c  len=00402000  (start= 2767644 len= 4202496)
-    Section  5 name="app"            version="v1.0.0.421"     start=006a5b1c  len=00947000  (start= 6970140 len= 9728000)
-    Section  6 name=""               version=""               start=00fecb1c  len=00000000  (start=16698140 len=       0)
-    Section  7 name="logo"           version="v1.0.0.1"       start=00fecb1c  len=0000f1fd  (start=16698140 len=   61949)
-    Section  8 name=""               version=""               start=00ffbd19  len=00000000  (start=16760089 len=       0)
-    Section  9 name=""               version=""               start=00ffbd19  len=00000000  (start=16760089 len=       0)
-    Mtd_part name="uboot1"         mtd="/dev/mtd9"       a=00000000  start=00000000  len=00080000
-    Mtd_part name="uboot2"         mtd="/dev/mtd9"       a=00080000  start=00080000  len=001e0000
-    Mtd_part name="bootargs"       mtd="/dev/mtd9"       a=00260000  start=00260000  len=00020000
-    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=00280000  start=00280000  len=00440000
-    Mtd_part name="fs"             mtd="/dev/mtd9"       a=006c0000  start=006c0000  len=00c00000
-    Mtd_part name="app"            mtd="/dev/mtd9"       a=012c0000  start=012c0000  len=02000000
-    Mtd_part name="para"           mtd="/dev/mtd9"       a=032c0000  start=032c0000  len=00800000
-    Mtd_part name="logo"           mtd="/dev/mtd9"       a=03ac0000  start=03ac0000  len=00200000
-    Mtd_part name="ipc_img"        mtd="/dev/mtd9"       a=03cc0000  start=03cc0000  len=00b00000
-    Mtd_part name="version"        mtd="/dev/mtd9"       a=ffffffff  start=ffffffff  len=00000000
+    Section  0 name="uboot1"         version="v1.0.0.1"       start=0x00000584  len=0x000437d0  (start=    1412 len=  276432)
+    Section  1 name=""               version=""               start=0x00043d54  len=0x00000000  (start=  277844 len=       0)
+    Section  2 name="bootargs"       version="v1.0.0.1"       start=0x00043d54  len=0x00020000  (start=  277844 len=  131072)
+    Section  3 name="kernel"         version="v1.0.0.1"       start=0x00063d54  len=0x0023fdc8  (start=  408916 len= 2358728)
+    Section  4 name="fs"             version="v1.0.0.442"     start=0x002a3b1c  len=0x00402000  (start= 2767644 len= 4202496)
+    Section  5 name="app"            version="v1.0.0.421"     start=0x006a5b1c  len=0x00947000  (start= 6970140 len= 9728000)
+    Section  6 name=""               version=""               start=0x00fecb1c  len=0x00000000  (start=16698140 len=       0)
+    Section  7 name="logo"           version="v1.0.0.1"       start=0x00fecb1c  len=0x0000f1fd  (start=16698140 len=   61949)
+    Section  8 name=""               version=""               start=0x00ffbd19  len=0x00000000  (start=16760089 len=       0)
+    Section  9 name=""               version=""               start=0x00ffbd19  len=0x00000000  (start=16760089 len=       0)
+    Mtd_part name="uboot1"         mtd="/dev/mtd9"       a=0x00000000  start=0x00000000  len=0x00080000
+    Mtd_part name="uboot2"         mtd="/dev/mtd9"       a=0x00080000  start=0x00080000  len=0x001e0000
+    Mtd_part name="bootargs"       mtd="/dev/mtd9"       a=0x00260000  start=0x00260000  len=0x00020000
+    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=0x00280000  start=0x00280000  len=0x00440000
+    Mtd_part name="fs"             mtd="/dev/mtd9"       a=0x006c0000  start=0x006c0000  len=0x00c00000
+    Mtd_part name="app"            mtd="/dev/mtd9"       a=0x012c0000  start=0x012c0000  len=0x02000000
+    Mtd_part name="para"           mtd="/dev/mtd9"       a=0x032c0000  start=0x032c0000  len=0x00800000
+    Mtd_part name="logo"           mtd="/dev/mtd9"       a=0x03ac0000  start=0x03ac0000  len=0x00200000
+    Mtd_part name="ipc_img"        mtd="/dev/mtd9"       a=0x03cc0000  start=0x03cc0000  len=0x00b00000
+    Mtd_part name="version"        mtd="/dev/mtd9"       a=0xffffffff  start=0xffffffff  len=0x00000000
 File passes CRC check: NVR8-7400_1705_3438_1103.pak
 ```
 
 ### Extracting content of `.pak` files
 
 Contents of a `.pak` file can be extracted using the `-e` command. If no
 output directory is specified using the `-d` parameter, a default unique
@@ -95,15 +109,14 @@
 the `.pak` file.
 
 example:
 ```shell
 pakler ./NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak -e -d newdir
 ```
 ```
-Attempting to guess number of sections... guessed: 11
 output: newdir
 Extracting section 0 (131072 bytes) into newdir/00_header.bin
 Extracting section 1 (18096 bytes) into newdir/01_loader.bin
 Extracting section 2 (26404 bytes) into newdir/02_fdt.bin
 Extracting section 3 (414552 bytes) into newdir/03_uboot.bin
 Extracting section 4 (3022896 bytes) into newdir/04_kernel.bin
 Extracting section 5 (12210176 bytes) into newdir/05_fs.bin
@@ -118,23 +131,22 @@
 
 A `.pak` file is made up of multiple sections, and at the moment you can
 replace only one section at a time. To replace a section you need to 
 use the `-r` command, specify the number of the section to replace with `-n`,
 the file to use as a replacement with `-f`, and the output file to write
 the resulting patched file with `-o`.
 
-Here is an example where we replace the `.pak` file's section #3 with the
-file ""
+Here is an example where we replace the `.pak` file's section #5 with the
+file `patched_fs.bin`
 
 ```shell
 pakler NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak -r -n 5 -f patched_fs.bin -o patched_fw.pak
 ````
 
 ```
-Attempting to guess number of sections... guessed: 11
 Input            : NT98312_NVR_8IP_REOLINK_L300_130_21060706.pak
 Output           : patched_fw.pak
 Replacing section: 5
 Replacement file : new_fs.bin
 Copying section 0 (131072 bytes)
 Copying section 1 (18096 bytes)
 Copying section 2 (26404 bytes)
@@ -146,42 +158,67 @@
 Copying section 8 (122036 bytes)
 Copying section 9 (0 bytes)
 Copying section 10 (0 bytes)
 Writing header... (1552 bytes)
 Updating CRC...
 Replacement completed. New header:
 Header  magic=32725913  crc32=41ee801c  type=00006202  sections=<11>  mtd_parts=<11>
-    Section  0 name="header"         version="v1.0.0.0"       start=00000610  len=00020000  (start=    1552 len=  131072)
-    Section  1 name="loader"         version="v1.0.0.0"       start=00020610  len=000046b0  (start=  132624 len=   18096)
-    Section  2 name="fdt"            version="v1.0.0.0"       start=00024cc0  len=00006724  (start=  150720 len=   26404)
-    Section  3 name="uboot"          version="v1.0.0.0"       start=0002b3e4  len=00065358  (start=  177124 len=  414552)
-    Section  4 name="kernel"         version="v1.0.0.0"       start=0009073c  len=002e2030  (start=  591676 len= 3022896)
-    Section  5 name="fs"             version="v1.0.0.0"       start=0037276c  len=00ba557a  (start= 3614572 len=12211578)
-    Section  6 name="app"            version="v1.0.0.0"       start=00f17ce6  len=01052000  (start=15826150 len=17113088)
-    Section  7 name=""               version=""               start=01f69ce6  len=00000000  (start=32939238 len=       0)
-    Section  8 name="logo"           version="v1.0.0.0"       start=01f69ce6  len=0001dcb4  (start=32939238 len=  122036)
-    Section  9 name=""               version=""               start=01f8799a  len=00000000  (start=33061274 len=       0)
-    Section 10 name=""               version=""               start=01f8799a  len=00000000  (start=33061274 len=       0)
-    Mtd_part name="header"         mtd="/dev/mtd9"       a=00000000  start=00000000  len=00020000
-    Mtd_part name="loader"         mtd="/dev/mtd9"       a=00020000  start=00020000  len=00080000
-    Mtd_part name="fdt"            mtd="/dev/mtd9"       a=000a0000  start=000a0000  len=00080000
-    Mtd_part name="uboot"          mtd="/dev/mtd9"       a=00120000  start=00120000  len=000e0000
-    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=00200000  start=00200000  len=00500000
-    Mtd_part name="fs"             mtd="/dev/mtd9"       a=00700000  start=00700000  len=00f00000
-    Mtd_part name="app"            mtd="/dev/mtd9"       a=01600000  start=01600000  len=02000000
-    Mtd_part name="para"           mtd="/dev/mtd9"       a=03600000  start=03600000  len=00800000
-    Mtd_part name="logo"           mtd="/dev/mtd9"       a=03e00000  start=03e00000  len=00100000
-    Mtd_part name="uid"            mtd="/dev/mtd9"       a=03f00000  start=03f00000  len=00100000
-    Mtd_part name="version"        mtd="/dev/mtd9"       a=ffffffff  start=ffffffff  len=00000000
+    Section  0 name="header"         version="v1.0.0.0"       start=0x00000610  len=0x00020000  (start=    1552 len=  131072)
+    Section  1 name="loader"         version="v1.0.0.0"       start=0x00020610  len=0x000046b0  (start=  132624 len=   18096)
+    Section  2 name="fdt"            version="v1.0.0.0"       start=0x00024cc0  len=0x00006724  (start=  150720 len=   26404)
+    Section  3 name="uboot"          version="v1.0.0.0"       start=0x0002b3e4  len=0x00065358  (start=  177124 len=  414552)
+    Section  4 name="kernel"         version="v1.0.0.0"       start=0x0009073c  len=0x002e2030  (start=  591676 len= 3022896)
+    Section  5 name="fs"             version="v1.0.0.0"       start=0x0037276c  len=0x00ba557a  (start= 3614572 len=12211578)
+    Section  6 name="app"            version="v1.0.0.0"       start=0x00f17ce6  len=0x01052000  (start=15826150 len=17113088)
+    Section  7 name=""               version=""               start=0x01f69ce6  len=0x00000000  (start=32939238 len=       0)
+    Section  8 name="logo"           version="v1.0.0.0"       start=0x01f69ce6  len=0x0001dcb4  (start=32939238 len=  122036)
+    Section  9 name=""               version=""               start=0x01f8799a  len=0x00000000  (start=33061274 len=       0)
+    Section 10 name=""               version=""               start=0x01f8799a  len=0x00000000  (start=33061274 len=       0)
+    Mtd_part name="header"         mtd="/dev/mtd9"       a=0x00000000  start=0x00000000  len=0x00020000
+    Mtd_part name="loader"         mtd="/dev/mtd9"       a=0x00020000  start=0x00020000  len=0x00080000
+    Mtd_part name="fdt"            mtd="/dev/mtd9"       a=0x000a0000  start=0x000a0000  len=0x00080000
+    Mtd_part name="uboot"          mtd="/dev/mtd9"       a=0x00120000  start=0x00120000  len=0x000e0000
+    Mtd_part name="kernel"         mtd="/dev/mtd9"       a=0x00200000  start=0x00200000  len=0x00500000
+    Mtd_part name="fs"             mtd="/dev/mtd9"       a=0x00700000  start=0x00700000  len=0x00f00000
+    Mtd_part name="app"            mtd="/dev/mtd9"       a=0x01600000  start=0x01600000  len=0x02000000
+    Mtd_part name="para"           mtd="/dev/mtd9"       a=0x03600000  start=0x03600000  len=0x00800000
+    Mtd_part name="logo"           mtd="/dev/mtd9"       a=0x03e00000  start=0x03e00000  len=0x00100000
+    Mtd_part name="uid"            mtd="/dev/mtd9"       a=0x03f00000  start=0x03f00000  len=0x00100000
+    Mtd_part name="version"        mtd="/dev/mtd9"       a=0xffffffff  start=0xffffffff  len=0x00000000
+```
+
+### As a library
+
+Here are a few things you can do with pakler's API:
+
+```py
+from pakler import PAK
+
+with PAK.from_file("firmware.pak") as pak:  # Also from_bytes() and from_fd()
+    assert pak.crc == pak.calc_crc()
+    pak.extract("firmware_extracted")
+    print(pak.partitions)
+    section = pak.sections[0]
+    pak.save_section(section, f"{section.name}.bin")
+    section_bytes = pak.extract_section(section)
 ```
 
-
 ## Naming
 
 Why pakler? Take a **pak** and **L**ist it, **E**xtract it, or **R**eplace 
 parts of it... pakler? Makes sense! (Naming suggestions are welcome :) )
 
-## Licensing
+## Version history
 
-pakler is licensed under MIT license. See [LICENSE](LICENSE)
+* v0.2.0 - 2023/05/31 - The [AT0myks](https://github.com/AT0myks) release
+  
+  A big thanks to AT0myks for all the changes brought in this release.
+  - Make Pakler usable as a library (author: AT0myks)
+  - Support for 64-bit PAK files (author: AT0myks)
+  - Support for handling PAK files directly from ZIP archives (author: AT0myks)
+  - Several code layout and packaging improvements (author: AT0myks)
+
+* v0.1.0 - 2021/09/03 - Initial release
 
+## Licensing
 
+pakler is licensed under MIT license. See [LICENSE](LICENSE)
```

### Comparing `pakler-0.1.0/pakler.py` & `pakler-0.2.0/pakler/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,502 +1,563 @@
-#!/usr/bin/env python3
+# SPDX-FileCopyrightText: 2021 Vincent Mallet <vmallet@gmail.com>
+# SPDX-License-Identifier: MIT
 
 """Simple tool to manipulate PAK firmware files (list, extract, replace) for Swann and Reolink devices. See -h."""
 
-import argparse
-import itertools
-import os.path
+import io
 import struct
-import textwrap
 import zlib
+from pathlib import Path
 from typing import Optional
+from zipfile import ZipExtFile
 
 try:
-    from _version import version
+    from ._version import __version__
 except ModuleNotFoundError:
-    version = 'dev-local'
-
-EPILOG_MARKER = "##MYEPILOG##"
+    __version__ = 'dev-local'
 
 CHUNK_SIZE = 128 * 1024
 
 PAK_MAGIC = 0x32725913
+PAK_MAGIC_BYTES = PAK_MAGIC.to_bytes(4, "little")
 
 SECTION_FORMAT = "<32s24sII"
+SECTION_FORMAT_64 = "<32s24sQQ"
 SECTION_FIELDS = ['name',  # TODO: Docs
                   'version',
                   'start',
                   'len']
 SECTION_STRINGS = ['name', 'version']
 SECTION_SIZE = struct.calcsize(SECTION_FORMAT)  # 64
-SECTION_COUNT = 10
+SECTION_SIZE_64 = struct.calcsize(SECTION_FORMAT_64)  # 72
 
 MTD_PART_FORMAT = "<32sI32sII"
 MTD_PART_FIELDS = ['name',
                    'a',
                    'mtd',
                    'start',
                    'len']
 MTD_PART_STRINGS = ['name',
                     'mtd']
-MTD_PART_SIZE = struct.calcsize(MTD_PART_FORMAT)
-MTD_PART_COUNT = 10
+MTD_PART_SIZE = struct.calcsize(MTD_PART_FORMAT)  # 76
 
 HEADER_FORMAT = "<III"
+HEADER_FORMAT_64 = "<QQQ"
 HEADER_FIELDS = ['magic',
                  'crc32',
                  'type']
 HEADER_CRC_OFFSET = 4  # Offset of the CRC in the file
+HEADER_CRC_OFFSET_64 = 8
 HEADER_HEADER_SIZE = struct.calcsize(HEADER_FORMAT)  # Size of the header's header (first 12 bytes)
+HEADER_HEADER_SIZE_64 = struct.calcsize(HEADER_FORMAT_64)  # First 24 bytes
 
 
-def calc_header_size(section_count, mtd_part_count=None):
+def calc_header_size(section_count, mtd_part_count=None, is64=False):
     """Return the calculated size of the header given a number of sections (and optionally of mtd_parts)."""
     if not mtd_part_count:
         mtd_part_count = section_count
 
-    return struct.calcsize(HEADER_FORMAT) + (section_count * SECTION_SIZE) + (mtd_part_count * MTD_PART_SIZE)
+    if is64:
+        return HEADER_HEADER_SIZE_64 + (section_count * SECTION_SIZE_64) + (mtd_part_count * MTD_PART_SIZE)
+    return HEADER_HEADER_SIZE + (section_count * SECTION_SIZE) + (mtd_part_count * MTD_PART_SIZE)
 
 
 def decode_strings(obj, fields):
     """Decode (utf-8) 0-padded binary strings in the obj's fields to normal strings."""
     for field in fields:
         cstr = getattr(obj, field)
         fixed = cstr.rstrip(b'\0').decode('utf-8')
         setattr(obj, field, fixed)
 
 
 def quote_string(string):
     """Return the string surrounded with double-quotes."""
-    return '"{}"'.format(string)
+    return f'"{string}"'
 
 
-class Section(object):
-    """A header's 'section'"""
+class Section:
+    """A header's 'section'."""
 
-    def __init__(self, buf, num):
+    def __init__(self, buf, num, is64=False):
         self.num = num
         self.name = None
         self.version = None
         self.start = 0
         self.len = 0
+        self.section_format = SECTION_FORMAT_64 if is64 else SECTION_FORMAT
 
-        fields = dict(zip(SECTION_FIELDS, struct.unpack(SECTION_FORMAT, buf)))
-        for key, val in fields.items():
+        fields = zip(SECTION_FIELDS, struct.unpack(self.section_format, buf))
+        for key, val in fields:
             setattr(self, key, val)
 
         decode_strings(self, SECTION_STRINGS)
 
     def __repr__(self):
-        return 'Section {:2} name={:16} version={:16} start={:08x}  len={:08x}  (start={:8} len={:8})'.format(
-            self.num, quote_string(self.name), quote_string(self.version), self.start, self.len, self.start, self.len)
+        return f"{self.__class__.__qualname__}({self.name!r})"
 
     def __iter__(self):
         for key in dir(self):
             if not key.startswith('_'):
                 yield key, getattr(self, key)
 
-    def serialize(self):
-        return struct.pack(SECTION_FORMAT, self.name.encode(), self.version.encode(), self.start, self.len)
+    def __bytes__(self):
+        return struct.pack(self.section_format, self.name.encode(), self.version.encode(), self.start, self.len)
+
+    def debug_str(self):
+        return 'Section {:2} name={:16} version={:16} start=0x{:08x}  len=0x{:08x}  (start={:8} len={:8})'.format(
+            self.num, quote_string(self.name), quote_string(self.version), self.start, self.len, self.start, self.len)
 
 
-class MtdPart(object):
-    """A header's 'Mtd_Part'"""
+class MtdPart:
+    """A header's 'Mtd_Part'."""
 
     def __init__(self, buf):
         self.name = None
         self.a = 0
         self.mtd = None
         self.start = 0
         self.len = 0
 
-        fields = dict(zip(MTD_PART_FIELDS, struct.unpack(MTD_PART_FORMAT, buf)))
-        for key, val in fields.items():
+        fields = zip(MTD_PART_FIELDS, struct.unpack(MTD_PART_FORMAT, buf))
+        for key, val in fields:
             setattr(self, key, val)
 
         decode_strings(self, MTD_PART_STRINGS)
 
     def __repr__(self):
-        return 'Mtd_part name={:16} mtd={:16}  a={:08x}  start={:08x}  len={:08x}'.format(
-            quote_string(self.name), quote_string(self.mtd), self.a, self.start, self.len)
+        return f"{self.__class__.__qualname__}({self.name!r})"
 
     def __iter__(self):
         for key in dir(self):
             if not key.startswith('_'):
                 yield key, getattr(self, key)
 
-    def serialize(self):
+    def __bytes__(self):
         return struct.pack(MTD_PART_FORMAT, self.name.encode(), self.a, self.mtd.encode(), self.start, self.len)
 
+    def debug_str(self):
+        return 'Mtd_part name={:16} mtd={:16}  a=0x{:08x}  start=0x{:08x}  len=0x{:08x}'.format(
+            quote_string(self.name), quote_string(self.mtd), self.a, self.start, self.len)
 
-class Header(object):
-    """PAK file header"""
 
-    def __init__(self, buf, section_count, mtd_part_count):
+class Header:
+    """PAK file header."""
+
+    def __init__(self, buf, section_count, mtd_part_count, is64=False):
         self.magic = 0
         self.crc32 = 0
         self.type = 0
         self.sections = []
         self.mtd_parts = []
+        self.is64 = is64
+        if is64:
+            self.header_format = HEADER_FORMAT_64
+            self.header_header_size = HEADER_HEADER_SIZE_64
+            self.section_size = SECTION_SIZE_64
+        else:
+            self.header_format = HEADER_FORMAT
+            self.header_header_size = HEADER_HEADER_SIZE
+            self.section_size = SECTION_SIZE
 
-        self.size = calc_header_size(section_count, mtd_part_count)
+        self.size = calc_header_size(section_count, mtd_part_count, is64)
         if len(buf) != self.size:
-            raise Exception("Invalid header buffer size, expected: {}, got: {}".format(self.size, len(buf)))
+            raise Exception(f"Invalid header buffer size, expected: {self.size}, got: {len(buf)}")
 
-        fields = dict(zip(HEADER_FIELDS, struct.unpack(HEADER_FORMAT, buf[:HEADER_HEADER_SIZE])))
-        for key, val in fields.items():
+        fields = zip(HEADER_FIELDS, struct.unpack(self.header_format, buf[:self.header_header_size]))
+        for key, val in fields:
             setattr(self, key, val)
 
-        buf = buf[HEADER_HEADER_SIZE:]
+        buf = buf[self.header_header_size:]
         for num in range(section_count):
-            self.sections.append(Section(buf[:SECTION_SIZE], num))
-            buf = buf[SECTION_SIZE:]
+            self.sections.append(Section(buf[:self.section_size], num, is64))
+            buf = buf[self.section_size:]
 
-        for num in range(mtd_part_count):
+        for _ in range(mtd_part_count):
             self.mtd_parts.append(MtdPart(buf[:MTD_PART_SIZE]))
             buf = buf[MTD_PART_SIZE:]
 
         self._check_errors(buf[:-4])
 
     def __repr__(self):
-        return 'Header  magic={:08x}  crc32={:08x}  type={:08x}  sections=<{}>  mtd_parts=<{}>'.format(
-            self.magic, self.crc32, self.type, len(self.sections), len(self.mtd_parts))
+        return '{}(magic=0x{:08x}, crc32=0x{:08x}, type=0x{:08x})'.format(
+            self.__class__.__qualname__, self.magic, self.crc32, self.type, len(self.sections), len(self.mtd_parts))
 
     def __iter__(self):
         for key in dir(self):
             if not key.startswith('_'):
                 yield key, getattr(self, key)
 
+    def __bytes__(self):
+        buf = struct.pack(self.header_format, self.magic, self.crc32, self.type)
+        for section in self.sections:
+            buf += bytes(section)
+        for mtd_part in self.mtd_parts:
+            buf += bytes(mtd_part)
+
+        if len(buf) != self.size:
+            raise Exception(f"Serialization error: should have been {self.size} bytes, but produced: {len(buf)} bytes")
+
+        return buf
+
     def _check_errors(self, buf_crc):
         if self.magic != PAK_MAGIC:
-            raise Exception("Wrong header magic: expected {:08x}, got {:08x}".format(PAK_MAGIC, self.magic))
+            raise Exception(f"Wrong header magic: expected 0x{PAK_MAGIC:08x}, got 0x{self.magic:08x}")
+
+    def debug_str(self):
+        return 'Header  magic=0x{:08x}  crc32=0x{:08x}  type=0x{:08x}  sections=<{}>  mtd_parts=<{}>'.format(
+            self.magic, self.crc32, self.type, len(self.sections), len(self.mtd_parts))
 
     def print_debug(self):
-        print(self)
+        print(self.debug_str())
         for section in self.sections:
-            print("    {}".format(section))
+            print(f"    {section.debug_str()}")
         for part in self.mtd_parts:
-            print("    {}".format(part))
+            print(f"    {part.debug_str()}")
 
-    def serialize(self):
-        buf = struct.pack(HEADER_FORMAT, self.magic, self.crc32, self.type)
-        for section in self.sections:
-            buf += section.serialize()
-        for mtd_part in self.mtd_parts:
-            buf += mtd_part.serialize()
 
-        if len(buf) != self.size:
-            raise Exception("Serialization error: should have been {} bytes, but produced: {} bytes".format(
-                self.size, len(buf)))
+class PAK:
 
-        return buf
+    def __init__(self, fd, header: Header, closefd=True) -> None:
+        self._fd = fd
+        self._header = header
+        self._closefd = closefd
 
+    def __enter__(self):
+        return self
 
-def read_header(filename, section_count, mtd_part_count=None):
-    """Read and parse the header of a PAK firmware file.
+    def __exit__(self, exc_type, exc_value, traceback):
+        if self._closefd:
+            self.close()
 
-    :param filename: name of the PAK firmware file
-    :param section_count: number of sections present in the header
-    :param mtd_part_count: optional number of mtd_parts, defaults to section_count
-    :return: the parsed Header object
-    """
-    if not mtd_part_count:
-        mtd_part_count = section_count
+    @property
+    def magic(self):
+        return self._header.magic
 
-    header_size = calc_header_size(section_count, mtd_part_count)
+    @property
+    def crc(self):
+        return self._header.crc32
 
-    with open(filename, "rb") as f:
-        buf = f.read(header_size)
-        if len(buf) != header_size:
-            raise Exception("Header size error, expected: {}, got: {}".format(header_size, len(buf)))
+    @property
+    def type(self):
+        return self._header.type
 
-    return Header(buf, section_count, mtd_part_count)
+    @property
+    def header(self):
+        return self._header
 
+    @property
+    def sections(self):
+        return self._header.sections
 
-def calc_crc(filename, section_count):
-    """Calculate the PAK file's CRC (which should match the header's CRC)"""
-    header_size = calc_header_size(section_count)
-    crc = 0xffffffff
-    with open(filename, "rb") as f:
-        f.seek(header_size)
+    @property
+    def partitions(self):
+        return self._header.mtd_parts
+
+    @property
+    def is64(self):
+        return self._header.is64
+
+    def close(self):
+        self._fd.close()
+
+    def calc_crc(self):
+        """Calculate the PAK file's CRC (which should match the header's CRC)."""
+        crc = 0xffffffff
+        self._fd.seek(self.header.size)
 
-        for chunk in iter(lambda: f.read(CHUNK_SIZE), b''):
+        for chunk in iter(lambda: self._fd.read(CHUNK_SIZE), b''):
             crc = zlib.crc32(chunk, crc)
 
         buf = b'\2\0\0\0'  # TODO explain...
         crc = zlib.crc32(buf, crc)
 
-        f.seek(HEADER_HEADER_SIZE)
-        buf = f.read(section_count * SECTION_SIZE)
+        self._fd.seek(self.header.header_header_size)
+        buf = self._fd.read(len(self.sections) * self.header.section_size)
         crc = zlib.crc32(buf, crc)
 
-    crc = crc ^ 0xffffffff
-    return crc
+        crc = crc ^ 0xffffffff
+        return crc
 
+    def extract_section(self, section: Section):
+        self._fd.seek(section.start)
+        return self._fd.read(section.len)
+
+    def save_section(self, section: Section, out_filename):
+        self._fd.seek(section.start)
+        with open(out_filename, "wb") as fout:
+            copy(self._fd, fout, section.len)
+
+    def extract(self, output_dir: Path, include_empty=False, quiet=True):
+        """Extract all sections from the PAK file into individual files."""
+        if not output_dir.exists():
+            output_dir.mkdir()
+
+        if not output_dir.exists() or not output_dir.is_dir():
+            raise Exception(f"Invalid output directory: {output_dir}")
+
+        for section in self.sections:
+            out_filename = output_dir / make_section_filename(section)
+            if section.len or include_empty:
+                _print(f"Extracting section {section.num} ({section.len} bytes) into {out_filename}", quiet=quiet)
+                self.save_section(section, out_filename)
+            else:
+                _print(f"Skipping empty section {section.num}", quiet=quiet)
 
-def check_crc(filename, section_count, mtd_part_count=None):
+    @staticmethod
+    def is_64bit(fd):
+        """Determine the firmware's target bitness.
+
+        Firmwares for 64-bit devices have 8 bytes long header fields
+        instead of 4, with zero padding. That means the three "extra"
+        groups of bytes are all zeroes. For 32-bit devices, the first
+        group corresponds to the CRC and the second is a part of the
+        first section's name, therefore they can never be all zeroes.
+        """
+        fmt = "<IIIIII"
+        struct_size = struct.calcsize(fmt)
+        _, group1, _, group2, _, group3 = struct.unpack(fmt, fd.read(struct_size))
+        return sum((group1, group2, group3)) == 0
+
+    @staticmethod
+    def get_section_count(fd, is64) -> Optional[int]:
+        """
+        Attempt to guess the number of sections for the given PAK firmware file.
+
+        :return: Guessed number of sections, or None if it couldn't be guessed
+        """
+        offset = HEADER_HEADER_SIZE_64 if is64 else HEADER_HEADER_SIZE
+        section_size = SECTION_SIZE_64 if is64 else SECTION_SIZE
+        fd.seek(offset, 1)
+        first_section = Section(fd.read(section_size), 0, is64)
+        first_section_name = first_section.name.encode("utf-8")
+        for count in range(30):
+            data = fd.read(section_size)
+            if data.startswith(first_section_name):
+                return count + 1
+        return None
+
+    @staticmethod
+    def read_header(fd, section_count, is64):
+        """Read and parse the header of a PAK firmware file.
+
+        :param fd: file object representing the PAK firmware file
+        :param section_count: number of sections present in the header
+        :param is64: bitness of the PAK firmware
+        :return: the parsed Header object
+        """
+        header_size = calc_header_size(section_count, section_count, is64)
+        buf = fd.read(header_size)
+        if len(buf) != header_size:
+            raise Exception(f"Header size error, expected: {header_size}, got: {len(buf)}")
+        return Header(buf, section_count, section_count, is64)
+
+    @classmethod
+    def from_fd(cls, fd, offset=0, closefd=True):
+        fd.seek(offset)
+        is64 = cls.is_64bit(fd)
+        fd.seek(offset)
+        section_count = cls.get_section_count(fd, is64)
+        fd.seek(offset)
+        header = cls.read_header(fd, section_count, is64)
+        return cls(fd, header, closefd)
+
+    @classmethod
+    def from_bytes(cls, bytes_, offset=0):
+        return cls.from_fd(io.BytesIO(bytes_), offset)
+
+    @classmethod
+    def from_file(cls, path, offset=0):
+        return cls.from_fd(open(path, "rb"), offset)
+
+
+def read_header(filename, section_count=None, mtd_part_count=None, is64=None):
+    """Read and parse the header of a PAK firmware file.
+
+    :param filename: name of the PAK firmware file
+    :param section_count: number of sections present in the header
+    :param mtd_part_count: optional number of mtd_parts, defaults to section_count
+    :param is64: bitness of the PAK firmware
+    :return: the parsed Header object
+    """
+    with PAK.from_file(filename) as pak:
+        return pak.header
+
+
+def calc_crc(filename, section_count=None, is64=None):
+    """Calculate the PAK file's CRC (which should match the header's CRC)."""
+    with PAK.from_file(filename) as pak:
+        return pak.calc_crc()
+
+
+def check_crc(filename, section_count=None, mtd_part_count=None, is64=None):
     """Check the PAK file's crc matches the crc in its header."""
-    header = read_header(filename, section_count, mtd_part_count)
-    crc = calc_crc(filename, section_count)
+    if isinstance(filename, ZipExtFile):
+        with PAK.from_fd(filename) as pak:
+            header = pak.header
+            crc = pak.calc_crc()
+        filename = filename.name
+    else:
+        with PAK.from_file(filename) as pak:
+            header = pak.header
+            crc = pak.calc_crc()
 
     if crc != header.crc32:
-        print("CRC MISMATCH, file: {}, header.crc={:08x}, got={:08x}".format(filename, header.crc32, crc))
+        print(f"CRC MISMATCH, file: {filename}, header.crc=0x{header.crc32:08x}, got=0x{crc:08x}")
         return False
 
-    print("File passes CRC check: {}".format(filename))
+    print(f"File passes CRC check: {filename}")
     return True
 
 
-def update_crc(filename, section_count):
+def update_crc(filename, section_count=None, is64=None):
     """Recompute the PAK file's crc and store it in its header.
 
     Note: the PAK file is modified by this operation.
     """
-    crc = calc_crc(filename, section_count)
+    with PAK.from_file(filename) as pak:
+        crc = pak.calc_crc()
+        offset = HEADER_CRC_OFFSET_64 if pak.is64 else HEADER_CRC_OFFSET
+        fmt = "<Q" if pak.is64 else "<I"
 
     with open(filename, "r+b") as f:
-        f.seek(HEADER_CRC_OFFSET)
-        f.write(struct.pack("<I", crc))
+        f.seek(offset)
+        f.write(struct.pack(fmt, crc))
 
 
 def make_section_filename(section):
     # TODO: should sanitize section name before turning it into a filename
     if section.name:
-        return "{:02}_{}.bin".format(section.num, section.name)
-    return "{:02}.bin".format(section.num)
-
-
-def find_new_name(base):
-    name = base
-    suffix = 0
-    while os.path.exists(name):
-        suffix += 1
-        if suffix == 1000:
-            raise Exception("Could not find a non-existing file/directory for base: {}".format(base))
-        name = "{}.{:03}".format(base, suffix)
-
-    return name
-
-
-def make_output_file_name(filename):
-    base = filename + ".replaced"
-    return find_new_name(base)
-
-
-def make_output_dir_name(filename):
-    base = filename + ".extracted"
-    return find_new_name(base)
+        return f"{section.num:02}_{section.name}.bin"
+    return f"{section.num:02}.bin"
 
 
 def copy(fin, fout, length):
     chunk_size = CHUNK_SIZE
     while length > 0:
         if length < chunk_size:
             chunk_size = length
         chunk = fin.read(chunk_size)
         if not chunk:
-            raise Exception("Read error with chunk_size={} length={}".format(chunk_size, length))
+            raise Exception(f"Read error with chunk_size={chunk_size} length={length}")
         fout.write(chunk)
         length -= chunk_size
 
 
 def extract_section(f, section, out_filename):
     f.seek(section.start)
     with open(out_filename, "wb") as fout:
         copy(f, fout, section.len)
 
 
-def extract(filename, output_dir, include_empty, section_count, mtd_part_count=None):
+def extract(filename, output_dir: Path, include_empty=False, section_count=None, mtd_part_count=None):
     """Extract all sections from the given PAK file into individual files."""
-    header = read_header(filename, section_count, mtd_part_count)
-
-    if not os.path.exists(output_dir):
-        os.mkdir(output_dir)
+    if not output_dir.exists():
+        output_dir.mkdir()
 
-    if not os.path.exists(output_dir) or not os.path.isdir(output_dir):
-        raise Exception("Invalid output directory: {}".format(output_dir))
+    if not output_dir.exists() or not output_dir.is_dir():
+        raise Exception(f"Invalid output directory: {output_dir}")
 
-    with open(filename, "rb") as f:
-        for section in header.sections:
-            out_filename = os.path.join(output_dir, make_section_filename(section))
+    with PAK.from_file(filename) as pak:
+        for section in pak.sections:
+            out_filename = output_dir / make_section_filename(section)
             if section.len or include_empty:
-                print("Extracting section {} ({} bytes) into {}".format(section.num, section.len, out_filename))
-                extract_section(f, section, out_filename)
+                print(f"Extracting section {section.num} ({section.len} bytes) into {out_filename}")
+                pak.save_section(section, out_filename)
             else:
-                print("Skipping empty section {}".format(section.num))
+                print(f"Skipping empty section {section.num}")
 
 
-def replace_section(filename, section_file, section_num, output_file, section_count, mtd_part_count=None):
-    """Copy the given PAK file into new output_file, replacing the specified section
+def replace_section(filename, section_file: Path, section_num, output_file: Path, section_count=None, mtd_part_count=None):
+    """Copy the given PAK file into new output_file, replacing the specified section.
 
     :param filename: name of the input PAK firmware file
     :param section_file: name of the file containing the section to be swapped-in
     :param section_num: number of the section to be replaced
     :param output_file: name of the output file which will contained the modified PAK file
     :param section_count: number of sections in the input PAK file
     :param mtd_part_count:  optional number of mtd_parts in the input PAK file
     """
-    header = read_header(filename, section_count, mtd_part_count)
-    new_header = read_header(filename, section_count, mtd_part_count)
+    with PAK.from_file(filename) as pak:
+        new_header = pak.header
+        section_count = len(pak.sections)
 
-    if not os.path.isfile(section_file):
-        raise Exception("Section file doesn't exist or is not a file: {}".format(section_file))
+    if not section_file.is_file():
+        raise Exception(f"Section file doesn't exist or is not a file: {section_file}")
 
-    section_len = os.path.getsize(section_file)
+    section_len = section_file.stat().st_size
 
     if section_num < 0 or section_num >= section_count:
-        raise Exception("Invalid section number: {} (should be between 0 and {})".format(section_num, section_count))
+        raise Exception(f"Invalid section number: {section_num} (should be between 0 and {section_count})")
 
-    print("Input            : {}".format(filename))
-    print("Output           : {}".format(output_file))
-    print("Replacing section: {}".format(section_num))
-    print("Replacement file : {}".format(section_file))
+    print(f"Input            : {filename}")
+    print(f"Output           : {output_file}")
+    print(f"Replacing section: {section_num}")
+    print(f"Replacement file : {section_file}")
 
-    with open(filename, "rb") as f, open(section_file, "rb") as fsection, open(output_file, "wb") as fout:
+    with PAK.from_file(filename) as pak, open(section_file, "rb") as fsection, open(output_file, "wb") as fout:
         # Write placeholder header
         fout.write(bytearray(new_header.size))
 
-        for section in header.sections:
-            f.seek(section.start)
+        for section in pak.sections:
+            pak._fd.seek(section.start)
             new_header.sections[section.num].start = fout.tell()  # TODO: set up a check in Header.init() to validate sections[num].num==num
             if section.num == section_num:
                 new_header.sections[section.num].len = section_len
-                print("Replacing section {} ({} bytes) with {} bytes".format(section.num, section.len, section_len))
+                print(f"Replacing section {section.num} ({section.len} bytes) with {section_len} bytes")
                 copy(fsection, fout, section_len)
             else:
-                print("Copying section {} ({} bytes)".format(section.num, section.len))
-                copy(f, fout, section.len)
+                print(f"Copying section {section.num} ({section.len} bytes)")
+                copy(pak._fd, fout, section.len)
 
-        print("Writing header... ({} bytes)".format(new_header.size))
+        print(f"Writing header... ({new_header.size} bytes)")
         fout.seek(0)
-        fout.write(new_header.serialize())
+        fout.write(bytes(new_header))
 
     print("Updating CRC...")
-    update_crc(output_file, section_count)
+    update_crc(output_file)
 
     print("Replacement completed. New header: ")
-    replaced_header = read_header(output_file, section_count)
-    replaced_header.print_debug()
+    with PAK.from_file(output_file) as pak:
+        pak.header.print_debug()
+
 
+def guess_section_count(filename, is64=None) -> Optional[int]:
+    """
+    Attempt to guess the number of sections for the given PAK firmware file.
 
-def make_epilogue_text(prog, indent, width):
-    lines = [
-        '{} ~/fw/CAM_FW.pak'.format(prog),
-        'List the content of CAM_FW.pak, auto-detecting the number of sections',
-        '',
-        '{} ~/fw/CAM_FW.pak -e -d /tmp/extracted/'.format(prog),
-        'Extract all sections of CAM_FW.pak into /tmp/extracted',
-        '',
-        '{} ~/fw/CAM_FW.pak -r -n 4 -f ~/fw/new_fs.cramfs -o ~/fw/CAM_FW_PATCHED.pak'.format(prog),
-        'From firmware file ~/fw/CAM_FW.pak, replace the 4th section with new file ~/fw/new_fs.cramfs, writing'
-        ' the output to ~/fw/CAM_FW_PATCHED.pak'
-    ]
+    :return: Guessed number of sections, or None if it couldn't be guessed
+    """
+    if is64 is None:
+        is64 = is_64bit(filename)
+    with open(filename, "rb") as f:
+        return PAK.get_section_count(f, is64)
 
-    wrapper = textwrap.TextWrapper(width, initial_indent=indent, subsequent_indent=indent)
 
-    return "\n".join(["examples:"] + [wrapper.fill(line) for line in lines])
+def is_64bit(filename):
+    with open(filename, "rb") as f:
+        return PAK.is_64bit(f)
 
 
-class EpilogizerHelpFormatter(argparse.HelpFormatter):
-    """
-    Help message formatter which injects a pre-formatted epilog text if the text to be formatted is the EPILOG_MARKER.
-    """
+def _print(*args, **kwargs):
+    if not kwargs.pop("quiet", False):
+        print(*args, **kwargs)
 
-    def __init__(self, prog, indent_increment=2, max_help_position=24, width=None) -> None:
-        super().__init__(prog, indent_increment, max_help_position, width)
-        self._my_prog = prog
-        self._my_indent = ' ' * indent_increment
-
-    def _fill_text(self, text, width, indent):
-        if text == EPILOG_MARKER:
-            return make_epilogue_text(self._my_prog, self._my_indent, width)
-        return super()._fill_text(text, width, indent)
-
-
-def parse_args():
-    parser = argparse.ArgumentParser(
-        description='%(prog)s {} (by Vincent Mallet 2021) - manipulate Swann / Reolink PAK firmware files'.format(
-            version),
-        formatter_class=EpilogizerHelpFormatter,
-        epilog=EPILOG_MARKER)
-
-    parser.add_argument('-v', '--version', action='version', version="%(prog)s {}".format(version))
-
-    pgroup = parser.add_mutually_exclusive_group()
-    pgroup.add_argument('-l', '--list', dest='list', action='store_true',
-                        help='List contents of PAK firmware file (default)')
-    pgroup.add_argument('-r', '--replace', dest='replace', action='store_true',
-                        help='Replace a section into a new PAK file')
-    pgroup.add_argument('-e', '--extract', dest='extract', action='store_true',
-                        help='Extract sections to a directory')
-    parser.add_argument('-f', '--section-file', dest='section_file', help='Input binary file for section replacement')
-    parser.add_argument('-n', '--section-num', dest='section_num', type=int, help='Section number of replaced section')
-    parser.add_argument('-o', '--output', dest='output_pak', help='Name of output PAK file when replacing a section')
-    parser.add_argument('-d', '--output-dir', dest='output_dir',
-                        help='Name of output directory when extracting sections')
-    parser.add_argument('-c', '--section-count', dest='section_count', type=int, default=None,
-                        help='Number of sections in source PAK file (will try to guess if not specified, or fallback'
-                             ' to default of {})'.format(SECTION_COUNT))
-    parser.add_argument('--empty', dest='include_empty', action='store_true',
-                        help='Include empty sections when extracting')
-    parser.add_argument('filename', nargs=1, help='Name of PAK firmware file')
-
-    args = parser.parse_args()
-
-    # Set default action as "list"
-    if not (args.list or args.replace or args.extract):
-        args.list = True
 
-    return args
+def _is_pak(file):
+    return file.read(4) == PAK_MAGIC_BYTES
 
 
-def guess_section_count(filename) -> Optional[int]:
-    """
-    Attempt to guess the number of sections for the given PAK firmware file.
+def is_pak_file(fileorbytes):
+    """See if a file is a PAK file by checking the magic number.
 
-    :return: Guessed number of sections, or None if it couldn't be guessed
+    The argument may be a bytes object, a file or file-like object.
     """
-    # Attempt all counts between 1 and 30 starting with the most probable first
-    for i in itertools.chain(range(8, 14), range(1, 8), range(14, 30)):
-        try:
-            read_header(filename, i)
-            return i
-        except Exception:  # Broad clause: the goal is to blindly try to parse the header, ignoring ALL errors
-            pass
-
-    return None
-
-
-def main():
-    args = parse_args()
-    filename = args.filename[0]
-
-    section_count = args.section_count
-    if not section_count:
-        print("Attempting to guess number of sections... ", end='')
-        section_count = guess_section_count(filename)
-        if section_count:
-            print("guessed: {}".format(section_count))
+    if isinstance(fileorbytes, (bytes, bytearray)):
+        return _is_pak(io.BytesIO(fileorbytes[:4]))
+    try:
+        if hasattr(fileorbytes, "read"):
+            return _is_pak(fileorbytes)
         else:
-            print("failed to guess, using default of {}".format(SECTION_COUNT))
-            section_count = SECTION_COUNT
-
-    if args.list:
-        header = read_header(filename, section_count)
-        header.print_debug()
-        check_crc(filename, section_count)
-
-    elif args.extract:
-        output_dir = args.output_dir or make_output_dir_name(filename)
-        print("output: {}".format(output_dir))
-        extract(filename, output_dir, args.include_empty, section_count)
-
-    elif args.replace:
-        if not args.section_file or not args.section_num:
-            raise Exception("replace error: need both section binary file and section number to do a replacement;"
-                            " see help")
-        output_file = args.output_pak or make_output_file_name(filename)
-        replace_section(filename, args.section_file, args.section_num, output_file, section_count)
-
-
-if __name__ == "__main__":
-    main()
+            with open(fileorbytes, "rb") as f:
+                return _is_pak(f)
+    except OSError:
+        return False
```

