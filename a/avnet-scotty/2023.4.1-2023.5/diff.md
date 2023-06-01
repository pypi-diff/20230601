# Comparing `tmp/avnet-scotty-2023.4.1.tar.gz` & `tmp/avnet-scotty-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avnet-scotty-2023.4.1.tar", last modified: Sat May  6 11:07:01 2023, max compression
+gzip compressed data, was "avnet-scotty-2023.5.tar", last modified: Thu Jun  1 13:07:20 2023, max compression
```

## Comparing `avnet-scotty-2023.4.1.tar` & `avnet-scotty-2023.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/
--rw-r--r--   0 root         (0) root         (0)    32879 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    18967 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18667 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/avnet_scotty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18967 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-06 11:07:01.000000 avnet-scotty-2023.4.1/avnet_scotty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/bumper/
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/bumper/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4006 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/bumper/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     6698 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scotty
--rwxr-xr-x   0 root         (0) root         (0)     1580 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scotty-runqemu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      811 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scripts/vm_bundle.sh
--rw-r--r--   0 root         (0) root         (0)     1137 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/scripts/vm_create.sh.template
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 11:07:01.230428 avnet-scotty-2023.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-06 11:06:53.000000 avnet-scotty-2023.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/
+-rw-r--r--   0 root         (0) root         (0)    32879 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    19899 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/avnet_scotty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19899 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 13:07:20.000000 avnet-scotty-2023.5/avnet_scotty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/bumper/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/bumper/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4006 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/bumper/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6713 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scotty
+-rwxr-xr-x   0 root         (0) root         (0)     1637 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scotty-runqemu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      811 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scripts/vm_bundle.sh
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/scripts/vm_create.sh.template
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 13:07:20.484009 avnet-scotty-2023.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-06-01 13:07:12.000000 avnet-scotty-2023.5/setup.py
```

### Comparing `avnet-scotty-2023.4.1/LICENSE` & `avnet-scotty-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4.1/PKG-INFO` & `avnet-scotty-2023.5/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: avnet-scotty
-Version: 2023.4.1
-Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
-Home-page: https://github.com/avnet-embedded/simplecore-tools
-Author: Avnet Embedded GmbH
-License: GPL-3.0-only
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ***************
 The Scotty tool
 ***************
 
 Scotty
 ======
 
@@ -323,14 +313,47 @@
 .. code-block:: bash
 
    $ export DISTRO=simplecore-distro MACHINE=qemux86-64
    $ scotty setup --features-layers-set examples
    $ scotty bitbake simplecore-weston-demo-image
    $ scotty-runqemu simplecore-weston-demo-image
 
+.. note::
+
+  In case your machine does not offer KVM support run
+
+  .. code-block:: bash
+    
+    $ SCOTTY_QEMUNOKVM=1 scotty-runqemu simplecore-weston-demo-image
+
+scotty-test
+===========
+
+``scotty-test`` is a helper tool to run tests on real hardware.
+It will guide the user through the needed steps and create a test report.
+
+To run you will need
+
+- an Azure access token ``SAS_TOKEN``
+- access to `simplecore-tools <https://github.com/avnet-embedded/simplecore-tools>`_ repository
+- a Github account
+- a computer running Linux
+  - ``sudo``, ``dd``, ``git`` installed
+  - your git client propely setup
+- a SDCard
+- Internet access
+- the hardware you want to test
+
+.. code-block:: bash
+  
+  $ SAS_TOKEN=abcdef scotty-test
+
+The tool will download the necessary images and SDKs, run the tests and create a Markdown report that will
+be pushed to the `simplecore-tools repository <https://github.com/avnet-embedded/simplecore-tools>`_.
+
 scotty-layers.yaml
 ==================
 
 All the information ``scotty`` uses is defined in ``scotty-layers.yaml`` in the ``manifest`` repository.
 This file is a ``yaml`` file containing the following sections
 
 base section
```

### Comparing `avnet-scotty-2023.4.1/README.rst` & `avnet-scotty-2023.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: avnet-scotty
+Version: 2023.5
+Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
+Home-page: https://github.com/avnet-embedded/simplecore-tools
+Author: Avnet Embedded GmbH
+License: GPL-3.0-only
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ***************
 The Scotty tool
 ***************
 
 Scotty
 ======
 
@@ -313,14 +323,47 @@
 .. code-block:: bash
 
    $ export DISTRO=simplecore-distro MACHINE=qemux86-64
    $ scotty setup --features-layers-set examples
    $ scotty bitbake simplecore-weston-demo-image
    $ scotty-runqemu simplecore-weston-demo-image
 
+.. note::
+
+  In case your machine does not offer KVM support run
+
+  .. code-block:: bash
+    
+    $ SCOTTY_QEMUNOKVM=1 scotty-runqemu simplecore-weston-demo-image
+
+scotty-test
+===========
+
+``scotty-test`` is a helper tool to run tests on real hardware.
+It will guide the user through the needed steps and create a test report.
+
+To run you will need
+
+- an Azure access token ``SAS_TOKEN``
+- access to `simplecore-tools <https://github.com/avnet-embedded/simplecore-tools>`_ repository
+- a Github account
+- a computer running Linux
+  - ``sudo``, ``dd``, ``git`` installed
+  - your git client propely setup
+- a SDCard
+- Internet access
+- the hardware you want to test
+
+.. code-block:: bash
+  
+  $ SAS_TOKEN=abcdef scotty-test
+
+The tool will download the necessary images and SDKs, run the tests and create a Markdown report that will
+be pushed to the `simplecore-tools repository <https://github.com/avnet-embedded/simplecore-tools>`_.
+
 scotty-layers.yaml
 ==================
 
 All the information ``scotty`` uses is defined in ``scotty-layers.yaml`` in the ``manifest`` repository.
 This file is a ``yaml`` file containing the following sections
 
 base section
```

### Comparing `avnet-scotty-2023.4.1/avnet_scotty.egg-info/PKG-INFO` & `avnet-scotty-2023.5/avnet_scotty.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.4.1
+Version: 2023.5
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -323,14 +323,47 @@
 .. code-block:: bash
 
    $ export DISTRO=simplecore-distro MACHINE=qemux86-64
    $ scotty setup --features-layers-set examples
    $ scotty bitbake simplecore-weston-demo-image
    $ scotty-runqemu simplecore-weston-demo-image
 
+.. note::
+
+  In case your machine does not offer KVM support run
+
+  .. code-block:: bash
+    
+    $ SCOTTY_QEMUNOKVM=1 scotty-runqemu simplecore-weston-demo-image
+
+scotty-test
+===========
+
+``scotty-test`` is a helper tool to run tests on real hardware.
+It will guide the user through the needed steps and create a test report.
+
+To run you will need
+
+- an Azure access token ``SAS_TOKEN``
+- access to `simplecore-tools <https://github.com/avnet-embedded/simplecore-tools>`_ repository
+- a Github account
+- a computer running Linux
+  - ``sudo``, ``dd``, ``git`` installed
+  - your git client propely setup
+- a SDCard
+- Internet access
+- the hardware you want to test
+
+.. code-block:: bash
+  
+  $ SAS_TOKEN=abcdef scotty-test
+
+The tool will download the necessary images and SDKs, run the tests and create a Markdown report that will
+be pushed to the `simplecore-tools repository <https://github.com/avnet-embedded/simplecore-tools>`_.
+
 scotty-layers.yaml
 ==================
 
 All the information ``scotty`` uses is defined in ``scotty-layers.yaml`` in the ``manifest`` repository.
 This file is a ``yaml`` file containing the following sections
 
 base section
```

### Comparing `avnet-scotty-2023.4.1/bumper/__main__.py` & `avnet-scotty-2023.5/bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4.1/scotty` & `avnet-scotty-2023.5/scotty`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 	LICENSE_FLAGS_ACCEPTED \
 	LINES \
 	MACHINE \
 	SCOTTY_DEBUG \
 	SCOTTY_DEFAULT_MANIFEST_BRANCH \
 	SCOTTY_DEFAULT_MANIFEST_NAME \
 	SCOTTY_FEATURE_LAYERS \
+	SCOTTY_QEMUNOKVM \
 	SCOTTY_QEMUPARAMS \
 	TEMPLATECONF \
 	TERM \
 	UBOOT_ENV_VARS \
 	"
 # SCOTTY_FEATURES_LAYERS REPO_URL SCOTTY_MACHINE_DIR BUILDDIR
 declare -r scotty_whitelist=${SCOTTY_WHITELIST:-${scotty_whitelist_default}}
 
 if [ "${SCOTTY_DOCKER_IMAGE:-1}" == "1" ]; then
-    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:kirkstone"
+    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2023.5"
 else
     declare -r docker_default_image="${SCOTTY_DOCKER_IMAGE}"
 fi
 
-export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.4.1"
+export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.5"
 export SCOTTY_DEFAULT_MANIFEST_NAME="default-release.xml"
 
 debug() {
 	if [ "${SCOTTY_DEBUG:-0}" == "1" ]; then
 		echo -e "\033[1;38m${*}\033[0m"
 	fi
 }
```

### Comparing `avnet-scotty-2023.4.1/scotty-runqemu` & `avnet-scotty-2023.5/scotty-runqemu`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/bash
 # SPDX-FileCopyrightText: (C) 2022 Avnet Embedded GmbH
 # SPDX-License-Identifier: GPL-3.0-only
 
 scotty_dir=$(dirname "${0}")
-SCOTTY_QEMUPARAMS="${SCOTTY_QEMUPARAMS:--smp 4 -serial mon:stdio}"
+SCOTTY_QEMUPARAMS="${SCOTTY_QEMUPARAMS:--smp 4}"
 
 # Prints script info
 #
 function print_help() {
 	printf "Scotty-runqemu: A tool script for running qemu using compiled images\n"
 	printf "Usage: scotty-runqemu [option] <image-name>\n"
 	printf "  -h, --help\t\t show this help message and exit\n"
@@ -31,16 +31,16 @@
 function test_image() {
 	read -ra scotty_options <<< "${SCOTTY_RUNQEMU_TEST_IMAGE_OPTIONS}"
 	bitbake_command=("${scotty_options[@]}" "bitbake" "${@} -c testimage")
 	# Invoking "--network host" is not possible, as it causes recipe parsing to hang.
 	DOCKER_EXTRA_ARGS="${DOCKER_EXTRA_ARGS} --privileged"
 
 	# This qemu requirement is not explicitly stated in case of an error.
-	if echo "${@}" | grep -v "image-\|-image"; then
-		echo "Image name must include \"image-\" or \"-image\" substrings"
+	if echo "${@}" | grep -v "image-\|-image\|simplecore-simpleswitch-sdk"; then
+		echo "Image name must include \"image-\" or \"-image\" substrings or it must be \"simplecore-simpleswitch-sdk\""
 		exit 1
 	fi
 
 	# shellcheck source=/dev/null
 	source "${scotty_dir}"/scotty
 	run_command scotty.py "${bitbake_command[@]}"
 }
```

### Comparing `avnet-scotty-2023.4.1/scripts/vm_bundle.sh` & `avnet-scotty-2023.5/scripts/vm_bundle.sh`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4.1/scripts/vm_create.sh.template` & `avnet-scotty-2023.5/scripts/vm_create.sh.template`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.4.1/setup.py` & `avnet-scotty-2023.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,18 +13,21 @@
     long_description=open('README.rst', 'r').read(),
     long_description_content_type='text/x-rst',
     license='GPL-3.0-only',
     license_files=('LICENSE',),
     entry_points={
         'console_scripts': [
             'bumper = bumper.__main__:main',
+            'scotty-test = scotty_test.__main__:main',
         ],
     },
     packages=['bumper'],
-    install_requires=['GitPython >= 3.1, < 4.0'],
+    install_requires=['GitPython ~= 3.1',
+                      'azure-storage-blob ~= 12.16',
+                      'inquirer ~= 3.0'],
     # As scotty is already in use on PyPi our package is called
     # avnet-scotty
     name='avnet-scotty',
     scripts=[
         'scotty',
         'scotty-runqemu',
         'scripts/vm_bundle.sh',
```

