# Comparing `tmp/pypickup-0.3.4.tar.gz` & `tmp/pypickup-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypickup-0.3.4.tar", last modified: Fri Dec  2 20:18:27 2022, max compression
+gzip compressed data, was "pypickup-0.3.5.tar", last modified: Thu Jun  1 12:35:45 2023, max compression
```

## Comparing `pypickup-0.3.4.tar` & `pypickup-0.3.5.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-02 20:18:27.174596 pypickup-0.3.4/
--rwxrwxrwx   0 root         (0) root         (0)    11599 2022-08-10 10:26:06.000000 pypickup-0.3.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)    18633 2022-12-02 20:18:27.167598 pypickup-0.3.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5110 2022-11-25 16:51:20.000000 pypickup-0.3.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-02 20:18:26.569159 pypickup-0.3.4/pypickup/
--rwxrwxrwx   0 root         (0) root         (0)       20 2022-09-15 14:07:25.000000 pypickup-0.3.4/pypickup/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       36 2022-09-15 14:07:25.000000 pypickup-0.3.4/pypickup/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)      772 2022-11-10 14:11:39.000000 pypickup-0.3.4/pypickup/cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-02 20:18:27.007931 pypickup-0.3.4/pypickup/cmd/
--rwxrwxrwx   0 root         (0) root         (0)      134 2022-11-25 16:51:20.000000 pypickup-0.3.4/pypickup/cmd/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3765 2022-11-25 15:04:23.000000 pypickup-0.3.4/pypickup/cmd/add.py
--rwxrwxrwx   0 root         (0) root         (0)      611 2022-11-25 16:51:20.000000 pypickup-0.3.4/pypickup/cmd/config.py
--rwxrwxrwx   0 root         (0) root         (0)     1192 2022-09-19 11:29:14.000000 pypickup-0.3.4/pypickup/cmd/list.py
--rwxrwxrwx   0 root         (0) root         (0)     1213 2022-09-19 11:48:26.000000 pypickup-0.3.4/pypickup/cmd/remove.py
--rwxrwxrwx   0 root         (0) root         (0)     3305 2022-11-25 15:04:32.000000 pypickup-0.3.4/pypickup/cmd/update.py
--rwxrwxrwx   0 root         (0) root         (0)    24685 2022-12-02 20:01:53.000000 pypickup-0.3.4/pypickup/controller.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-02 20:18:27.080451 pypickup-0.3.4/pypickup/settings/
--rwxrwxrwx   0 root         (0) root         (0)     8306 2022-11-25 17:05:36.000000 pypickup-0.3.4/pypickup/settings/wheelFilters.py
--rwxrwxrwx   0 root         (0) root         (0)      811 2022-11-25 16:51:20.000000 pypickup-0.3.4/pypickup/settings/wheelFiltersSettings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-02 20:18:27.141990 pypickup-0.3.4/pypickup/utils/
--rwxrwxrwx   0 root         (0) root         (0)    16988 2022-11-25 16:51:20.000000 pypickup-0.3.4/pypickup/utils/htmlManager.py
--rwxrwxrwx   0 root         (0) root         (0)     3070 2022-09-20 16:28:38.000000 pypickup-0.3.4/pypickup/utils/networkManager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-12-02 20:18:26.736199 pypickup-0.3.4/pypickup.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    18633 2022-12-02 20:18:26.000000 pypickup-0.3.4/pypickup.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      592 2022-12-02 20:18:26.000000 pypickup-0.3.4/pypickup.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2022-12-02 20:18:26.000000 pypickup-0.3.4/pypickup.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      203 2022-12-02 20:18:26.000000 pypickup-0.3.4/pypickup.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      122 2022-12-02 20:18:26.000000 pypickup-0.3.4/pypickup.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2022-12-02 20:18:26.000000 pypickup-0.3.4/pypickup.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1349 2022-12-02 20:17:00.000000 pypickup-0.3.4/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2022-12-02 20:18:27.176611 pypickup-0.3.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       56 2022-11-25 16:51:20.000000 pypickup-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:35:45.240774 pypickup-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-01 12:35:34.000000 pypickup-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20613 2023-06-01 12:35:45.240774 pypickup-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-01 12:35:34.000000 pypickup-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:35:45.236774 pypickup-0.3.5/pypickup/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:35:45.240774 pypickup-0.3.5/pypickup/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/cmd/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/cmd/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/cmd/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/cmd/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/cmd/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28697 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:35:45.240774 pypickup-0.3.5/pypickup/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/settings/wheelFilters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:35:45.240774 pypickup-0.3.5/pypickup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/utils/htmlManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-01 12:35:34.000000 pypickup-0.3.5/pypickup/utils/networkManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:35:45.236774 pypickup-0.3.5/pypickup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20613 2023-06-01 12:35:45.000000 pypickup-0.3.5/pypickup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-01 12:35:45.000000 pypickup-0.3.5/pypickup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:35:45.000000 pypickup-0.3.5/pypickup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-01 12:35:45.000000 pypickup-0.3.5/pypickup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 12:35:45.000000 pypickup-0.3.5/pypickup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 12:35:45.000000 pypickup-0.3.5/pypickup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-01 12:35:34.000000 pypickup-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:35:45.240774 pypickup-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 12:35:34.000000 pypickup-0.3.5/setup.py
```

### Comparing `pypickup-0.3.4/LICENSE` & `pypickup-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypickup-0.3.4/PKG-INFO` & `pypickup-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypickup
-Version: 0.3.4
+Version: 0.3.5
 Summary: An utility to generate a local PyPI cache for selected packages based on the PyPI.org repositories.
 Author-email: German Navarro <ge.najim@gmail.com>, Sergio Sánchez Ramírez <sergio.sanchez.ramirez@bsc.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -297,15 +297,32 @@
 ```
 
 ## Examples
 
 To check what are all the available packages in the remote repository and which of them would be downloaded:
 
 ```
-pypickup add -a --dry-run [package]
+pypickup config --show                  # Shows the filters that will be applied for commands 'add' and 'update'
+
+pypickup add numpy                      # Downloads the whole package 'numpy', considering the active filters
+pypickup rm numpy                       # Removes the whole package 'numpy'
+
+pypickup add numpy==1.8                 # Downloads the package 'numpy' (version 1.8, all patches) to the local repository for the first time
+pypickup add -a --dry-run numpy         # Performs a test for command 'add', with the package 'numpy'. Prints the packages in the remote (PyPI), the ones that will be filtered out, and the actual ones that will be downloaded
+
+pypickup update numpy==1.9              # Downloads numpy version 1.9 (all patches) to the current local repository
+pypickup list numpy                     # Lists all the currently downloaded packages for the package 'numpy'
+pypickup rm numpy==1.8                  # Removes only numpy version 1.8 (and patches)
+pypickup rm numpy==1                    # Removes only numpy version 1 (and minors)
+
+pypickup add -s numpy                   # Downloads only the source files (not wheels)
+pypickup add --ps numpy                 # Downloads all the platform-specific packages for package 'numpy'. Some packages' wheels will only be able to be downloaded by means of this command, depending on how have they been built ('$ pypickup add --help' for documentation).
+
+pypickup list -r pandas                 # Lists the whole set of available packages in the remote repository for 'pandas'. Does not filter out any package, i.e shows everything. Please, consider that if you do now '$ pypickup add pandas', not all the previously shown packages will be downloaded, since the command 'add' is filtering out some packages by default, like the developement releases (alphas, betas...), the release candidates, and so on. See --help for more details on command 'add'
+pypickup list -r scipy==1.7.2           # Lists available packages for scipy, version 1.7.2
 ```
 
 ## Development
 
 ### Add new commands
 
 To add new commands to the application, follow these steps:
```

### Comparing `pypickup-0.3.4/README.md` & `pypickup-0.3.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -82,15 +82,32 @@
 ```
 
 ## Examples
 
 To check what are all the available packages in the remote repository and which of them would be downloaded:
 
 ```
-pypickup add -a --dry-run [package]
+pypickup config --show                  # Shows the filters that will be applied for commands 'add' and 'update'
+
+pypickup add numpy                      # Downloads the whole package 'numpy', considering the active filters
+pypickup rm numpy                       # Removes the whole package 'numpy'
+
+pypickup add numpy==1.8                 # Downloads the package 'numpy' (version 1.8, all patches) to the local repository for the first time
+pypickup add -a --dry-run numpy         # Performs a test for command 'add', with the package 'numpy'. Prints the packages in the remote (PyPI), the ones that will be filtered out, and the actual ones that will be downloaded
+
+pypickup update numpy==1.9              # Downloads numpy version 1.9 (all patches) to the current local repository
+pypickup list numpy                     # Lists all the currently downloaded packages for the package 'numpy'
+pypickup rm numpy==1.8                  # Removes only numpy version 1.8 (and patches)
+pypickup rm numpy==1                    # Removes only numpy version 1 (and minors)
+
+pypickup add -s numpy                   # Downloads only the source files (not wheels)
+pypickup add --ps numpy                 # Downloads all the platform-specific packages for package 'numpy'. Some packages' wheels will only be able to be downloaded by means of this command, depending on how have they been built ('$ pypickup add --help' for documentation).
+
+pypickup list -r pandas                 # Lists the whole set of available packages in the remote repository for 'pandas'. Does not filter out any package, i.e shows everything. Please, consider that if you do now '$ pypickup add pandas', not all the previously shown packages will be downloaded, since the command 'add' is filtering out some packages by default, like the developement releases (alphas, betas...), the release candidates, and so on. See --help for more details on command 'add'
+pypickup list -r scipy==1.7.2           # Lists available packages for scipy, version 1.7.2
 ```
 
 ## Development
 
 ### Add new commands
 
 To add new commands to the application, follow these steps:
```

### Comparing `pypickup-0.3.4/pypickup/cli.py` & `pypickup-0.3.5/pypickup/cli.py`

 * *Files identical despite different names*

### Comparing `pypickup-0.3.4/pypickup/cmd/add.py` & `pypickup-0.3.5/pypickup/cmd/update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 import argparse
 import os
 
 from typing import List
 
-from pypickup.controller import Add
+from pypickup.controller import Update
 
 
-class AddEP:
+class UpdateEP:
     @staticmethod
     def init_subparser(parser: argparse.ArgumentParser):
-        parser.add_argument("packageNameList", type=str, nargs="+", default="", help="Python packages list to add to the local repository.")
-        parser.add_argument("-p", "--index-path", dest="pypiLocalPath", type=str, default=os.getenv("PYPICKUP_INDEX_PATH", default="./.pypickup/"), help="Local root path in which the package from the PyPI repository will be downloaded.")
+        parser.add_argument("packageNameList", type=str, nargs="+", default="", help="Python packages list to add to the local repository. E.g. 'numpy', 'scipy pandas', 'numpy==1.8 tensorflow=1.12.2'.")
+        parser.add_argument("-p", "--index-path", dest="pypiLocalPath", type=str, default=os.getenv("PYPICKUP_INDEX_PATH", default="./.pypickup/"), help="Local root path in which the package from the PyPI repository will be synchronized.")
+
+        parser.add_argument("-r", "--requirements", dest="packageIsRequirementsFile", default=False, action="store_true", help="Used to indicate that the input is a requirements file instead of a package or list of packages.")
 
         parser.add_argument("--df", "--print-default-config", dest="printDefaultConfig", default=False, action="store_true", help="Prints the default settings.")
         parser.add_argument("-a", "--print-all-file-names", dest="printAllFileNames", default=False, action="store_true", help="Prints all the package files before being filtered whatsoever, prints the ones being filtered and finally prints the resulting subset that will be actually downloaded.")
         parser.add_argument("-v", "--verbose", dest="printVerbose", default=False, action="store_true", help="Prints the downloads in a more verbose fashion. WARNING! It slows down the execution.")
         parser.add_argument("--show-retries", dest="showRetries", default=False, action="store_true", help="Shows the retries in case there are any (e.g. due to a faulty network connection.")
-
+        
         parser.add_argument("-s", "--only-src", dest="onlySources", default=False, action="store_true", help="Download only the source files (.zip and .tar.gz). Disabled by default.")
         parser.add_argument("--dev", dest="includeDevs", default=False, action="store_true", help="Download also the new development releases (alpha, betas), which are not included by default.")
         parser.add_argument("--rc", dest="includeRCs", default=False, action="store_true", help="Download also the release candidates (rc), which are not included by default.")
-        parser.add_argument("--ps", "--platform-specific", dest="includePlatformSpecific", default=False, action="store_true", help="Download also the platform-specific wheels, which are not included by default. If this flag is not set, only platform-agnostic files are considered (-any.whl).")
-        
+        parser.add_argument("--ps", "--platform-specific", dest="includePlatformSpecific", default=False, action="store_true", help="Download also the platform-specific wheels, which are not included by default. If this flag is not set, only platform-agnostic files are considered.")
+
         parser.add_argument("-d", "--dry-run", dest="dryRun", default=False, action="store_true", help="Display the changes that would be performed without actually making them. Can be combined with the printing options in order to know what is the exact behaviour. E.g. pypickup add -d --nf numpy.")
 
     @staticmethod
     def run(args: argparse.Namespace):
         listOfPackages: List[str] = args.packageNameList
+        if args.packageIsRequirementsFile:
+
+            requirementsFile = ''.join(listOfPackages)
+            listOfPackages = []
+            with open(requirementsFile, "r") as reqsFile:
+                listOfPackages.extend(package.strip("\r\n") for package in reqsFile.readlines())
+
         for packageName in listOfPackages:
 
             args.packageName = packageName
 
-            controllerInstance = Add()
+            controllerInstance = Update()
             controllerInstance.parseScriptArguments(args)
 
             controllerInstance.printDefaultConfigIfRequired()
 
-            print("Adding '" + packageName + "' to the local index (" + os.path.abspath(args.pypiLocalPath) + "/" + "):")
-            if controllerInstance.validPackageName():
-                controllerInstance.initLocalRepo()
-
-                needToAddPackage: bool = controllerInstance.canAddNewPackage()
-                if needToAddPackage:
-                    controllerInstance.addPackage()
-                else:
-                    print("Package " + controllerInstance.packageName + " has been already added to the local repository. Try to run the 'update' command instead to synchronize changes against the remote PyPI.")
+            print("Updating the local index for '" + packageName + "':")
+            if controllerInstance.packageExists():
+                controllerInstance.synchronizeWithRemote()
             else:
-                print("Package " + controllerInstance.packageName + " does not exist in the remote repository (" + controllerInstance.remotePyPIRepository + ")")
+                print("Package " + controllerInstance.packageName + " has not been added to the local repository yet. Run the 'add' command first.")
 
             print()
```

### Comparing `pypickup-0.3.4/pypickup/cmd/config.py` & `pypickup-0.3.5/pypickup/cmd/config.py`

 * *Files identical despite different names*

### Comparing `pypickup-0.3.4/pypickup/cmd/list.py` & `pypickup-0.3.5/pypickup/cmd/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,25 @@
 
 class ListEP:
     @staticmethod
     def init_subparser(parser: argparse.ArgumentParser):
         parser.add_argument("packageName", type=str, nargs="?", default="", help="Python package for which the list of downloaded files will be shown.")
         parser.add_argument("-p", "--index-path", dest="pypiLocalPath", type=str, default=os.getenv("PYPICKUP_INDEX_PATH", default="./.pypickup/"), help="Local root path in which the specified package is expected to be.")
 
+        parser.add_argument("-r", "--remote", dest="remote", default=False, action="store_true", help="List all packages available in the remote repository.")
+
     @staticmethod
     def run(args: argparse.Namespace):
         controllerInstance = List()
         controllerInstance.parseScriptArguments(args)
 
-        if not controllerInstance.repositoryExists():
-            print("No local repository has been initialized yet. Download at least one package running the 'add' command.")
+        if args.remote:
+                controllerInstance.listPackagesInTheRemote()
+        elif not controllerInstance.repositoryExists():
+            print("No local repository has been initialized yet.\n" + \
+                  "    - Download at least one package running the 'add' command,\n" + \
+                  "    - Or use 'pypickup list -r package_name[==version]' to remotely list all the available packages.")
         else:
             if args.packageName != "" and not controllerInstance.packageExists():
                 print("Package " + controllerInstance.packageName + " has not been added to the local repository yet. Run the 'add' command first.")
             else:
                 controllerInstance.listPackages()
```

### Comparing `pypickup-0.3.4/pypickup/cmd/remove.py` & `pypickup-0.3.5/pypickup/cmd/remove.py`

 * *Files identical despite different names*

### Comparing `pypickup-0.3.4/pypickup/cmd/update.py` & `pypickup-0.3.5/pypickup/cmd/add.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,60 @@
 import argparse
 import os
 
 from typing import List
 
-from pypickup.controller import Update
+from pypickup.controller import Add
 
 
-class UpdateEP:
+class AddEP:
     @staticmethod
     def init_subparser(parser: argparse.ArgumentParser):
-        parser.add_argument("packageNameList", type=str, nargs="+", default="", help="Python packages list to add to the local repository.")
-        parser.add_argument("-p", "--index-path", dest="pypiLocalPath", type=str, default=os.getenv("PYPICKUP_INDEX_PATH", default="./.pypickup/"), help="Local root path in which the package from the PyPI repository will be synchronized.")
+        parser.add_argument("packageNameList", type=str, nargs="+", default="", help="Python packages list to add to the local repository. E.g. 'numpy', 'scipy pandas', 'numpy==1.8 tensorflow=1.12.2'.")
+        parser.add_argument("-p", "--index-path", dest="pypiLocalPath", type=str, default=os.getenv("PYPICKUP_INDEX_PATH", default="./.pypickup/"), help="Local root path in which the package from the PyPI repository will be downloaded.")
+
+        parser.add_argument("-r", "--requirements", dest="packageIsRequirementsFile", default=False, action="store_true", help="Used to indicate that the input is a requirements file instead of a package or list of packages.")
 
         parser.add_argument("--df", "--print-default-config", dest="printDefaultConfig", default=False, action="store_true", help="Prints the default settings.")
         parser.add_argument("-a", "--print-all-file-names", dest="printAllFileNames", default=False, action="store_true", help="Prints all the package files before being filtered whatsoever, prints the ones being filtered and finally prints the resulting subset that will be actually downloaded.")
         parser.add_argument("-v", "--verbose", dest="printVerbose", default=False, action="store_true", help="Prints the downloads in a more verbose fashion. WARNING! It slows down the execution.")
         parser.add_argument("--show-retries", dest="showRetries", default=False, action="store_true", help="Shows the retries in case there are any (e.g. due to a faulty network connection.")
-        
+
         parser.add_argument("-s", "--only-src", dest="onlySources", default=False, action="store_true", help="Download only the source files (.zip and .tar.gz). Disabled by default.")
         parser.add_argument("--dev", dest="includeDevs", default=False, action="store_true", help="Download also the new development releases (alpha, betas), which are not included by default.")
         parser.add_argument("--rc", dest="includeRCs", default=False, action="store_true", help="Download also the release candidates (rc), which are not included by default.")
-        parser.add_argument("--ps", "--platform-specific", dest="includePlatformSpecific", default=False, action="store_true", help="Download also the platform-specific wheels, which are not included by default. If this flag is not set, only platform-agnostic files are considered.")
-
+        parser.add_argument("--ps", "--platform-specific", dest="includePlatformSpecific", default=False, action="store_true", help="Download also the platform-specific wheels, which are not included by default. If this flag is not set, only platform-agnostic files are considered (-any.whl).")
+        
         parser.add_argument("-d", "--dry-run", dest="dryRun", default=False, action="store_true", help="Display the changes that would be performed without actually making them. Can be combined with the printing options in order to know what is the exact behaviour. E.g. pypickup add -d --nf numpy.")
 
     @staticmethod
     def run(args: argparse.Namespace):
         listOfPackages: List[str] = args.packageNameList
+        if args.packageIsRequirementsFile:
+
+            requirementsFile = ''.join(listOfPackages)
+            listOfPackages = []
+            with open(requirementsFile, "r") as reqsFile:
+                listOfPackages.extend(package.strip("\r\n") for package in reqsFile.readlines())
+
         for packageName in listOfPackages:
 
             args.packageName = packageName
 
-            controllerInstance = Update()
+            controllerInstance = Add()
             controllerInstance.parseScriptArguments(args)
 
             controllerInstance.printDefaultConfigIfRequired()
 
-            print("Updating the local index for '" + packageName + "':")
-            if controllerInstance.packageExists():
-                controllerInstance.synchronizeWithRemote()
+            print("Adding '" + packageName + "' to the local index (" + os.path.abspath(args.pypiLocalPath) + "/" + "):")
+            if controllerInstance.validPackageName():
+                controllerInstance.initLocalRepo()
+
+                needToAddPackage: bool = controllerInstance.canAddNewPackage()
+                if needToAddPackage:
+                    controllerInstance.addPackage()
+                else:
+                    print("Package " + controllerInstance.packageName + " has been already added to the local repository. Try to run the 'update' command instead to synchronize changes against the remote PyPI.")
             else:
-                print("Package " + controllerInstance.packageName + " has not been added to the local repository yet. Run the 'add' command first.")
+                print("Package " + controllerInstance.packageName + " does not exist in the remote repository (" + controllerInstance.remotePyPIRepository + ")")
 
             print()
```

### Comparing `pypickup-0.3.4/pypickup/controller.py` & `pypickup-0.3.5/pypickup/controller.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #! /usr/bin/python
 from io import TextIOWrapper
 import os
+import re
 import argparse
 import shutil
 from typing import Dict, List
 
 from tqdm import tqdm
 
 from pypickup.utils.htmlManager import HTMLManager
@@ -21,14 +22,16 @@
     _networkManager = NetworkManager()
 
     _baseHTMLFileName: str = "index.html"
     _packageHTMLFileName: str = "index.html"
     _remotePypiBaseDir: str = "https://pypi.org/simple/"
 
     _regexZIPAndTars = r"^(.*)\.(zip|tar.gz|tar.bz2|tar.xz|tar.Z|tar)$"
+    _regexVersion = r"^(.*)==(\d+(?:\.\d+)*)$"
+    # _regexVersion = r"^(.*)==(\d+\.\d+(?:\.\d+)?)$"
 
     _dryRunsTmpDir = "./.pypickup_tmp/"
 
     def __init__(self):
         self._packageName: str = None
         self._pypiLocalPath: str = None
 
@@ -41,14 +44,16 @@
         self._printVerbose: bool = None
         self._showRetries: bool = None
 
         self._onlySources: bool = None
         self._includeDevs: bool = None
         self._includeRCs: bool = None
         self._includePlatformSpecific: bool = None
+        
+        self._packageVersion: str = ""
 
         self._dryRun: bool = None
 
     def __del__(self):
         self._removeDir(self._dryRunsTmpDir, True)
 
     @property
@@ -104,14 +109,18 @@
         return self._includeRCs
 
     @property
     def includePlatformSpecific(self):
         return self._includePlatformSpecific
 
     @property
+    def packageVersion(self):
+        return self._packageVersion
+
+    @property
     def dryRun(self):
         return self._dryRun
 
     @packageName.setter
     def packageName(self, new_PackageName: str):
         self._packageName = new_PackageName
 
@@ -177,29 +186,45 @@
     def includeRCs(self, new_includeRCs: bool):
         self._includeRCs = new_includeRCs
 
     @includePlatformSpecific.setter
     def includePlatformSpecific(self, new_includePlatformSpecific: bool):
         self._includePlatformSpecific = new_includePlatformSpecific
 
+    @packageVersion.setter
+    def packageVersion(self, new_packageVersion: bool):
+        self._packageVersion = new_packageVersion
+
     @dryRun.setter
     def dryRun(self, new_dryRun: bool):
         self._dryRun = new_dryRun
 
+    def _removeFile(self, fileName: str):
+        if os.path.exists(fileName):
+            os.remove(fileName)
+
     def _removeDir(self, directory: str, recursively: bool = False):
         if os.path.exists(directory):
             if recursively:
                 shutil.rmtree(directory)
             else:
                 os.rmdir(directory)
 
     def parseScriptArguments(self, args: argparse.ArgumentParser):
-        """Parse the incoming arguments. A packageName and and pypiLocalPath are expected. Besides, it initializes derived class attributes."""
+        """Parse the incoming arguments. A packageName and pypiLocalPath are expected. Besides, it initializes derived class attributes."""
 
         self.packageName = str(args.packageName).lower()
+        specifiedVersion = re.match(self._regexVersion, self.packageName)
+        if specifiedVersion:
+            self.packageName = specifiedVersion[1]
+            self.packageVersion = self.packageName + "-" + specifiedVersion[2]
+        elif "=" in self.packageName:
+            print("Incorrect version format.")
+            exit(0)
+
         self.pypiLocalPath = args.pypiLocalPath
 
     def printDefaultConfigIfRequired(self):
         if self.printDefaultConfig:
             print("")
             print("DEFAULT CONFIGURATION VARIABLES:")
             print("\tIndex path (current): " + self.pypiLocalPath)
@@ -293,15 +318,15 @@
         self.includeDevs = args.includeDevs
         self.includeRCs = args.includeRCs
         self.includePlatformSpecific = args.includePlatformSpecific
 
         self.dryRun = args.dryRun
 
         # 2. Use only the ones we have set:
-        self._htmlManager.setFlags(self.printAllFileNames, self.onlySources, self.includeDevs, self.includeRCs, self.includePlatformSpecific)
+        self._htmlManager.setFlags(self.printAllFileNames, self.onlySources, self.includeDevs, self.includeRCs, self.includePlatformSpecific, self.packageVersion)
 
         if (self.includeDevs or self.includeRCs) and self._htmlManager.areWheelFiltersEnabled():
             print("\tWARNING! Development releases (devX) or release candidates (RCs) flags are enabled, as well as the wheel filters, so they could be discarded anyway. This is caused because of the order of application: (1st) flags, (2nd) wheel filters.")
             print("\tPLEASE, CHECK OUT YOUR WHEEL FILTERS.")
 
         if self.dryRun:
             shutil.copytree(self.pypiLocalPath, self._dryRunsTmpDir)
@@ -403,15 +428,15 @@
         self.includeDevs = args.includeDevs
         self.includeRCs = args.includeRCs
         self.includePlatformSpecific = args.includePlatformSpecific
 
         self.dryRun = args.dryRun
 
         # 2. Use only the ones we have set:
-        self._htmlManager.setFlags(self.printAllFileNames, self.onlySources, self.includeDevs, self.includeRCs, self.includePlatformSpecific)
+        self._htmlManager.setFlags(self.printAllFileNames, self.onlySources, self.includeDevs, self.includeRCs, self.includePlatformSpecific, self.packageVersion)
 
         if (self.includeDevs or self.includeRCs) and self._htmlManager.areWheelFiltersEnabled():
             print("\tWARNING! Development releases (devX) or release candidates (RCs) flags are enabled, as well as the wheel filters, so they could be discarded anyway. This is caused because of the order of application: (1st) flags, (2nd) wheel filters.")
             print("\tPLEASE, CHECK OUT YOUR WHEEL FILTERS.")
 
         if self.dryRun:
             shutil.copytree(self.pypiLocalPath, self._dryRunsTmpDir)
@@ -432,17 +457,18 @@
     def __getNewPackagesInRemote(self, remoteIndexHRefs: Dict[str, str], localIndexHRefs: Dict[str, str]) -> Dict[str, str]:
         resultingDict: Dict[str, str] = dict()
 
         for remotePackageName, remotePackageURL in remoteIndexHRefs.items():
             if not remotePackageName in localIndexHRefs:
                 resultingDict[remotePackageName] = remotePackageURL
 
-        additionalPackagesMessage: str = self.__checkPackagesInLocalButNotInRemote(remoteIndexHRefs, localIndexHRefs)
-        if additionalPackagesMessage != "":
-            print("WARNING! " + additionalPackagesMessage)
+        if not self.packageVersion:
+            additionalPackagesMessage: str = self.__checkPackagesInLocalButNotInRemote(remoteIndexHRefs, localIndexHRefs)
+            if additionalPackagesMessage != "":
+                print("WARNING! " + additionalPackagesMessage)
 
         return resultingDict
 
     def synchronizeWithRemote(self):
         """Synchronize the self.packageName against the PyPI remote repository. It adds the new available packages to the packageName/index.html and download them. Assumes the folders exists."""
 
         ok, status, pypiRemoteIndex = self._networkManager.getLink(self._remotePypiBaseDir + self.packageName)
@@ -484,42 +510,104 @@
         self.dryRun = args.dryRun
 
         # 2. Use only the ones we have set:
         if self.dryRun:
             shutil.copytree(self.pypiLocalPath, self._dryRunsTmpDir)
             self.pypiLocalPath = self._dryRunsTmpDir
 
-    def removePackage(self):
-        """Removes the self.packageName from the local repository. Assumes it exists."""
+    def __removeWholePackage(self, htmlFile: TextIOWrapper):
+        htmlFile.seek(0)
 
-        with open(self.baseHTMLFileFullName, "r+") as baseHTMLFile:
-            baseHTMLStr: str = baseHTMLFile.read()
-            packageExisted, updatedHTML = self._htmlManager.removeHTMLEntry(baseHTMLStr, "a", self.packageName)
+        _, updatedHTML = self._htmlManager.removeHTMLEntry(htmlFile.read(), "a", self.packageName)
+        self._writeFileFromTheStart(htmlFile, updatedHTML)
 
-            if not packageExisted:
-                print("Package '" + self.packageName + "' was not being tracked yet.")
-                return
+    def __removePackages(self, htmlFile: TextIOWrapper, subPackages: List[str]):
+        htmlFile.seek(0)
 
-            self._writeFileFromTheStart(baseHTMLFile, updatedHTML)
+        updatedHTML: str = htmlFile.read()
+        for subpackage in subPackages:
+            _, updatedHTML = self._htmlManager.removeHTMLEntry(updatedHTML, "a", subpackage)
+        
+        self._writeFileFromTheStart(htmlFile, updatedHTML)
+
+        # Actually remove the package after having updated the index
+        for subpackage in subPackages:
+            self._removeFile(os.path.join(self.packageLocalPath, subpackage))
 
-        self._removeDir(self.packageLocalPath, True)
+    def removePackage(self):
+        """Removes the specified version for the self.packageName from the local repository, or the whole package if it has not being specified. Assumes that the package exists."""
+
+        baseHTMLFile = open(self.baseHTMLFileFullName, "r+")
+        packageExist = self._htmlManager.existsHTMLEntry(baseHTMLFile.read(), "a", self.packageName)
 
-        print("'" + self.packageName + "' package successfully removed.")
+        if not packageExist:
+            print("Package '" + self.packageName + "' was not being tracked yet.")
+            return
+
+        localPackageHTMLFile = open(self.packageHTMLFileFullName, "r+")
+        localPackageHTMLIndex = localPackageHTMLFile.read()
+        currentLocalPackages = self._htmlManager.getHRefsList(localPackageHTMLIndex).keys()
+
+        localSubPackagesToRemove: List[str] = list()
+        for package in currentLocalPackages:
+            if self.packageVersion in package:
+                localSubPackagesToRemove.append(package)
+        
+        removeWholePackage: bool = len(localSubPackagesToRemove) == len(currentLocalPackages)
+        if removeWholePackage:
+            self.__removeWholePackage(baseHTMLFile)
+        else:
+            self.__removePackages(localPackageHTMLFile, localSubPackagesToRemove)
+
+        # Must close files in case the whole directory (package) needs to be erased
+        localPackageHTMLFile.close()
+        baseHTMLFile.close()
 
+        print("Subpackages from package '" + self.packageName + "' successfully removed:\n" + '\n'.join(localSubPackagesToRemove) + "\n")
 
+        if removeWholePackage:
+            self._removeDir(self.packageLocalPath, True)
+            print("Whole package '" + self.packageName + "' successfully removed.")
+            
+        
 class List(LocalPyPIController):
     def __init__(self):
         LocalPyPIController.__init__(self)
 
     def parseScriptArguments(self, args: argparse.ArgumentParser):
         LocalPyPIController.parseScriptArguments(self, args)
 
     def repositoryExists(self) -> bool:
         return os.path.exists(self.baseHTMLFileFullName)
 
+    def filterByVersion(self, packagesList) -> List[str]:
+        resultingList: List[str] = list()
+        for packageName in packagesList:
+            if self.packageVersion in packageName:
+                resultingList.append(packageName)
+
+        return resultingList
+
+    def listPackagesInTheRemote(self):
+        self._htmlManager.setFlags(None, None, None, None, None, self.packageVersion)
+
+        ok, status, pypiPackageHTML = self._networkManager.getLink(self._remotePypiBaseDir + self.packageName)
+        if not ok:
+            print(status)
+        else:
+            pypiPackageHTMLStr: str = pypiPackageHTML.decode("utf-8")
+
+        packageFiles: List[str] = self._htmlManager.getHRefsList(pypiPackageHTMLStr).keys()
+
+        filteredPackageFiles = self.filterByVersion(packageFiles)
+        filteredPackageFiles.sort()
+
+        print("Found " + str(len(filteredPackageFiles)) + " packages (IN THE REMOTE, i.e. NOT DOWNLOADED - perform the 'add' command to add the the package to the local repository):")
+        print('\n'.join(filteredPackageFiles))
+
     def listPackages(self):
         """Lists all the packages in the root HTML index, if self.packageName == None. Lists the downloaded files for package self.packageName otherwise."""
 
         printMessage: str = ""
 
         htmlString: str = ""
         if self.packageName == "":
@@ -527,21 +615,23 @@
                 htmlString = baseHTMLFile.read()
 
             printMessage = "Found {} packages:"
         else:
             with open(self.packageHTMLFileFullName, "r") as packageHTMLFile:
                 htmlString = packageHTMLFile.read()
 
-            printMessage = "Found {} files for package '" + self.packageName + "':"
+            printMessage = "Found {} files for package '" + str(self.packageVersion if self.packageVersion else self.packageName) + "':"
 
-        packagesDict: Dict[str, str] = self._htmlManager.getHRefsList(htmlString)
+        packageFiles: List[str] = self._htmlManager.getHRefsList(htmlString).keys()
 
-        print(printMessage.format(len(packagesDict)))
-        for key, _ in packagesDict.items():
-            print(key)
+        filteredPackageFiles = self.filterByVersion(packageFiles)
+        filteredPackageFiles.sort()
+        
+        print(printMessage.format(len(filteredPackageFiles)))
+        print('\n'.join(filteredPackageFiles))
 
 class Config(LocalPyPIController):
     def __init__(self):
         self._printWheelFilters: bool = None
 
     @property
     def printWheelFilters(self):
```

### Comparing `pypickup-0.3.4/pypickup/settings/wheelFilters.py` & `pypickup-0.3.5/pypickup/settings/wheelFilters.py`

 * *Files identical despite different names*

### Comparing `pypickup-0.3.4/pypickup/utils/htmlManager.py` & `pypickup-0.3.5/pypickup/utils/htmlManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,14 +202,16 @@
         self._printAllFileNames: bool
 
         self._onlySources: bool
         self._includeDevs: bool
         self._includeRCs: bool
         self._includePlatformSpecific: bool
 
+        self._packageVersion: str
+
     @property
     def printAllFileNames(self):
         return self._printAllFileNames
 
     @property
     def onlySources(self):
         return self._onlySources
@@ -221,14 +223,18 @@
     @property
     def includeRCs(self):
         return self._includeRCs
 
     @property
     def includePlatformSpecific(self):
         return self._includePlatformSpecific
+    
+    @property
+    def packageVersion(self):
+        return self._packageVersion
 
     @printAllFileNames.setter
     def printAllFileNames(self, new_printAllFileNames: bool):
         self._printAllFileNames = new_printAllFileNames
 
     @onlySources.setter
     def onlySources(self, new_onlySources: bool):
@@ -242,21 +248,27 @@
     def includeRCs(self, new_includeRCs: bool):
         self._includeRCs = new_includeRCs
 
     @includePlatformSpecific.setter
     def includePlatformSpecific(self, new_includePlatformSpecific: bool):
         self._includePlatformSpecific = new_includePlatformSpecific
 
-    def setFlags(self, printAllFileNames: bool, onlySources: bool, includeDevs: bool, includeRCs: bool, includePlatformSpecific: bool):
+    @packageVersion.setter
+    def packageVersion(self, new_packageVersion: bool):
+        self._packageVersion = new_packageVersion
+
+    def setFlags(self, printAllFileNames: bool, onlySources: bool, includeDevs: bool, includeRCs: bool, includePlatformSpecific: bool, packageVersion: str):
         self.printAllFileNames = printAllFileNames
         self.onlySources = onlySources
         self.includeDevs = includeDevs
         self.includeRCs = includeRCs
         self.includePlatformSpecific = includePlatformSpecific
 
+        self.packageVersion = packageVersion
+
     def getWheelFiltersSettingsFilePath(self) -> str:
         return self._wheelsManager.getWheelFiltersSettingsFilePath()
 
     def areWheelFiltersEnabled(self) -> bool:
         return self._wheelsManager.areWheelFiltersEnabled()
 
     def inOrOutFilterEnabled(self) -> str:
@@ -356,14 +368,17 @@
             return False
 
         if re.search(rf"-any.whl", fileName):
             return False
 
         return True
 
+    def __isRequiredVersion(self, fileName):
+        return self.packageVersion in fileName
+
     def _printFilteredOutFiles(self, nonFilteredEntries: bs4Element.ResultSet[bs4Element.Tag], filteredEntries: List[bs4Element.Tag]):
         filteredCounter = 0
         print("Filtered out entries:")
         for nonFilteredEntry in nonFilteredEntries:
             if not nonFilteredEntry in filteredEntries:
                 print(nonFilteredEntry.string)
 
@@ -385,17 +400,20 @@
         for aEntry in aEntries:
             if (self.__isDevFile(aEntry.string) and not self.includeDevs) or (self.__isRCFile(aEntry.string) and not self.includeRCs):
                 continue
 
             if self.__isPlatformSpecificWheel(aEntry.string) and not self.includePlatformSpecific:
                 continue
 
-            if not self.onlySources and self._wheelsManager.isValidWheel(aEntry.string):
+            if not self.__isRequiredVersion(aEntry.string):
+                continue
+
+            if not self.onlySources and self._wheelsManager.isValidWheel(aEntry.string):    # Checking wheels
                 aEntriesOutput.append(aEntry)
-            else:
+            else:                                                                           # Checking source codes
                 reSult = re.match(regexZIPAndTars, aEntry.string)
                 if reSult:
                     reSultName: str = reSult.group(1)
                     reSultExtension: str = reSult.group(2)
 
                     if reSultExtension == "zip":
                         zipAndTarsDict[reSultName] = reSultExtension
```

### Comparing `pypickup-0.3.4/pypickup/utils/networkManager.py` & `pypickup-0.3.5/pypickup/utils/networkManager.py`

 * *Files identical despite different names*

### Comparing `pypickup-0.3.4/pypickup.egg-info/PKG-INFO` & `pypickup-0.3.5/pypickup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypickup
-Version: 0.3.4
+Version: 0.3.5
 Summary: An utility to generate a local PyPI cache for selected packages based on the PyPI.org repositories.
 Author-email: German Navarro <ge.najim@gmail.com>, Sergio Sánchez Ramírez <sergio.sanchez.ramirez@bsc.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -297,15 +297,32 @@
 ```
 
 ## Examples
 
 To check what are all the available packages in the remote repository and which of them would be downloaded:
 
 ```
-pypickup add -a --dry-run [package]
+pypickup config --show                  # Shows the filters that will be applied for commands 'add' and 'update'
+
+pypickup add numpy                      # Downloads the whole package 'numpy', considering the active filters
+pypickup rm numpy                       # Removes the whole package 'numpy'
+
+pypickup add numpy==1.8                 # Downloads the package 'numpy' (version 1.8, all patches) to the local repository for the first time
+pypickup add -a --dry-run numpy         # Performs a test for command 'add', with the package 'numpy'. Prints the packages in the remote (PyPI), the ones that will be filtered out, and the actual ones that will be downloaded
+
+pypickup update numpy==1.9              # Downloads numpy version 1.9 (all patches) to the current local repository
+pypickup list numpy                     # Lists all the currently downloaded packages for the package 'numpy'
+pypickup rm numpy==1.8                  # Removes only numpy version 1.8 (and patches)
+pypickup rm numpy==1                    # Removes only numpy version 1 (and minors)
+
+pypickup add -s numpy                   # Downloads only the source files (not wheels)
+pypickup add --ps numpy                 # Downloads all the platform-specific packages for package 'numpy'. Some packages' wheels will only be able to be downloaded by means of this command, depending on how have they been built ('$ pypickup add --help' for documentation).
+
+pypickup list -r pandas                 # Lists the whole set of available packages in the remote repository for 'pandas'. Does not filter out any package, i.e shows everything. Please, consider that if you do now '$ pypickup add pandas', not all the previously shown packages will be downloaded, since the command 'add' is filtering out some packages by default, like the developement releases (alphas, betas...), the release candidates, and so on. See --help for more details on command 'add'
+pypickup list -r scipy==1.7.2           # Lists available packages for scipy, version 1.7.2
 ```
 
 ## Development
 
 ### Add new commands
 
 To add new commands to the application, follow these steps:
```

### Comparing `pypickup-0.3.4/pypickup.egg-info/SOURCES.txt` & `pypickup-0.3.5/pypickup.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -15,10 +15,9 @@
 pypickup/cmd/__init__.py
 pypickup/cmd/add.py
 pypickup/cmd/config.py
 pypickup/cmd/list.py
 pypickup/cmd/remove.py
 pypickup/cmd/update.py
 pypickup/settings/wheelFilters.py
-pypickup/settings/wheelFiltersSettings.yaml
 pypickup/utils/htmlManager.py
 pypickup/utils/networkManager.py
```

### Comparing `pypickup-0.3.4/pyproject.toml` & `pypickup-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pypickup"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="German Navarro", email="ge.najim@gmail.com" },
   { name="Sergio Sánchez Ramírez", email="sergio.sanchez.ramirez@bsc.es" },
 ]
 description = "An utility to generate a local PyPI cache for selected packages based on the PyPI.org repositories."
 readme = "README.md"
 license = { file="LICENSE" }
@@ -19,15 +19,15 @@
     "Operating System :: OS Independent",
     "Topic :: System :: Archiving :: Mirroring"
 ]
 dependencies = [
   "beautifulsoup4==4.11.1",
   "wheel-filename==1.4.1",
   "multimethod==1.9",
-  "requests==2.28.1",
+  "requests==2.31.0",
   "tqdm==4.64.1",
   "PyYAML==6.0",
   "pytest-cov==4.0.0",
 ]
 
 [tool.setuptools]
 packages = ["pypickup", "pypickup.cmd", "pypickup.settings", "pypickup.utils"]
```

