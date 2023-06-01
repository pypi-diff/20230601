# Comparing `tmp/conan_package_tools-0.8.5.tar.gz` & `tmp/conan_package_tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan_package_tools-0.8.5.tar", last modified: Wed Jan 10 08:30:54 2018, max compression
+gzip compressed data, was "dist/conan_package_tools-0.9.0.tar", last modified: Mon Jan 15 15:29:24 2018, max compression
```

## Comparing `conan_package_tools-0.8.5.tar` & `conan_package_tools-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/
--rw-r--r--   0 luism    (1884520237) staff       (20)      732 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/PKG-INFO
--rw-r--r--   0 luism    (1884520237) staff       (20)    37724 2018-01-04 16:32:55.000000 conan_package_tools-0.8.5/README.md
--rw-r--r--   0 luism    (1884520237) staff       (20)     3998 2017-10-27 08:04:05.000000 conan_package_tools-0.8.5/setup.py
-drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan/
--rw-r--r--   0 luism    (1884520237) staff       (20)       45 2018-01-10 08:27:52.000000 conan_package_tools-0.8.5/conan/requirements.txt
-drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan/test/
--rw-r--r--   0 luism    (1884520237) staff       (20)        0 2017-05-03 16:03:53.000000 conan_package_tools-0.8.5/conan/test/__init__.py
--rw-r--r--   0 luism    (1884520237) staff       (20)    25606 2018-01-10 08:30:10.000000 conan_package_tools-0.8.5/conan/test/packager_test.py
--rw-r--r--   0 luism    (1884520237) staff       (20)    31546 2017-12-28 10:36:07.000000 conan_package_tools-0.8.5/conan/test/generators_test.py
--rw-r--r--   0 luism    (1884520237) staff       (20)     1461 2017-10-31 13:10:53.000000 conan_package_tools-0.8.5/conan/log.py
--rw-r--r--   0 luism    (1884520237) staff       (20)      135 2017-10-31 13:09:22.000000 conan_package_tools-0.8.5/conan/tools.py
--rw-r--r--   0 luism    (1884520237) staff       (20)    27392 2018-01-10 08:30:30.000000 conan_package_tools-0.8.5/conan/packager.py
--rw-r--r--   0 luism    (1884520237) staff       (20)       23 2018-01-10 08:30:30.000000 conan_package_tools-0.8.5/conan/__init__.py
--rw-r--r--   0 luism    (1884520237) staff       (20)      351 2018-01-09 09:51:47.000000 conan_package_tools-0.8.5/conan/run_in_docker.py
--rw-r--r--   0 luism    (1884520237) staff       (20)       11 2017-05-03 16:03:53.000000 conan_package_tools-0.8.5/conan/requirements_test.txt
--rw-r--r--   0 luism    (1884520237) staff       (20)    11889 2017-12-28 10:36:07.000000 conan_package_tools-0.8.5/conan/builds_generator.py
--rw-r--r--   0 luism    (1884520237) staff       (20)     8852 2018-01-09 09:51:47.000000 conan_package_tools-0.8.5/conan/create_runner.py
--rw-r--r--   0 luism    (1884520237) staff       (20)       59 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/setup.cfg
-drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan_package_tools.egg-info/
--rw-r--r--   0 luism    (1884520237) staff       (20)      732 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan_package_tools.egg-info/PKG-INFO
--rw-r--r--   0 luism    (1884520237) staff       (20)      546 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan_package_tools.egg-info/SOURCES.txt
--rw-r--r--   0 luism    (1884520237) staff       (20)       66 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan_package_tools.egg-info/entry_points.txt
--rw-r--r--   0 luism    (1884520237) staff       (20)       45 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan_package_tools.egg-info/requires.txt
--rw-r--r--   0 luism    (1884520237) staff       (20)        6 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan_package_tools.egg-info/top_level.txt
--rw-r--r--   0 luism    (1884520237) staff       (20)        1 2018-01-10 08:30:54.000000 conan_package_tools-0.8.5/conan_package_tools.egg-info/dependency_links.txt
+drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/
+-rw-r--r--   0 luism    (1884520237) staff       (20)      766 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/PKG-INFO
+-rw-r--r--   0 luism    (1884520237) staff       (20)    39017 2018-01-15 15:28:46.000000 conan_package_tools-0.9.0/README.md
+-rw-r--r--   0 luism    (1884520237) staff       (20)     3998 2017-10-27 08:04:05.000000 conan_package_tools-0.9.0/setup.py
+drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan/
+-rw-r--r--   0 luism    (1884520237) staff       (20)       45 2018-01-10 08:27:52.000000 conan_package_tools-0.9.0/conan/requirements.txt
+drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan/test/
+-rw-r--r--   0 luism    (1884520237) staff       (20)        0 2017-05-03 16:03:53.000000 conan_package_tools-0.9.0/conan/test/__init__.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)    25606 2018-01-10 08:30:10.000000 conan_package_tools-0.9.0/conan/test/packager_test.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)    31546 2017-12-28 10:36:07.000000 conan_package_tools-0.9.0/conan/test/generators_test.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)     1461 2017-10-31 13:10:53.000000 conan_package_tools-0.9.0/conan/log.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)      135 2017-10-31 13:09:22.000000 conan_package_tools-0.9.0/conan/tools.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)    27613 2018-01-15 15:28:46.000000 conan_package_tools-0.9.0/conan/packager.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)       23 2018-01-15 15:28:52.000000 conan_package_tools-0.9.0/conan/__init__.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)      351 2018-01-09 09:51:47.000000 conan_package_tools-0.9.0/conan/run_in_docker.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)       11 2017-05-03 16:03:53.000000 conan_package_tools-0.9.0/conan/requirements_test.txt
+-rw-r--r--   0 luism    (1884520237) staff       (20)    11889 2017-12-28 10:36:07.000000 conan_package_tools-0.9.0/conan/builds_generator.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)     9071 2018-01-15 15:28:46.000000 conan_package_tools-0.9.0/conan/create_runner.py
+-rw-r--r--   0 luism    (1884520237) staff       (20)       38 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/setup.cfg
+drwxr-xr-x   0 luism    (1884520237) staff       (20)        0 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan_package_tools.egg-info/
+-rw-r--r--   0 luism    (1884520237) staff       (20)      766 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan_package_tools.egg-info/PKG-INFO
+-rw-r--r--   0 luism    (1884520237) staff       (20)      546 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan_package_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 luism    (1884520237) staff       (20)       66 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan_package_tools.egg-info/entry_points.txt
+-rw-r--r--   0 luism    (1884520237) staff       (20)       45 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan_package_tools.egg-info/requires.txt
+-rw-r--r--   0 luism    (1884520237) staff       (20)        6 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan_package_tools.egg-info/top_level.txt
+-rw-r--r--   0 luism    (1884520237) staff       (20)        1 2018-01-15 15:29:24.000000 conan_package_tools-0.9.0/conan_package_tools.egg-info/dependency_links.txt
```

### Comparing `conan_package_tools-0.8.5/PKG-INFO` & `conan_package_tools-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: conan_package_tools
-Version: 0.8.5
+Version: 0.9.0
 Summary: Packaging tools for Conan C/C++ package manager
 Home-page: https://github.com/conan-io/conan-package-tools
 Author: JFrog LTD. Luis Martinez de Bartolome
 Author-email: luism@jfrog.com
 License: MIT
+Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Keywords: conan,C/C++,package,libraries,developer,manager,dependency,tool,c,c++,cpp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `conan_package_tools-0.8.5/README.md` & `conan_package_tools-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -307,18 +307,45 @@
     $ export CONAN_DOCKER_IMAGE=lasote/conangcc49
     $ export CONAN_USE_DOCKER=1
     $ python build.py
 
 
 It will generate a set of build configurations (profiles) for gcc 4.9 and will run it inside a container of the ``lasote/conangcc49`` image.
 
+### Running scripts and executing commands before to build on Docker
+
+When Conan Package Tools uses Docker to build your packages, sometimes you need to execute a "before build" step. If
+you need to install packages, change files or create a setup, there is an option for that: **docker_entry_script**
+
+**Example**:
+
+This example shows how to install *tzdata* package by apt-get, before to build the Conan package.
+
+    from conan.packager import ConanMultiPackager
+
+	if __name__ == "__main__":
+        command = "sudo apt-get -qq update && sudo apt-get -qq install -y tzdata"
+	    builder = ConanMultiPackager(use_docker=True, docker_image='lasote/conangcc7', docker_entry_script=command)
+	    builder.add_common_builds()
+	    builder.run()
+
+Also, it's possible to run some internal script, before to build the package:
+
+    from conan.packager import ConanMultiPackager
+
+    if __name__ == "__main__":
+        command = "python bootstrap.py"
+        builder = ConanMultiPackager(use_docker=True, docker_image='lasote/conangcc7', docker_entry_script=command)
+        builder.add_common_builds()
+        builder.run()
+
 
 ## Specifying a different base profile
 
-The options, settings and environment variables that the ``add_common_builds()`` method generate, are applied into the default profile 
+The options, settings and environment variables that the ``add_common_builds()`` method generate, are applied into the default profile
 of the conan installation. If you want to use a different default profile you can pass the name of the profile in the ``run()`` method.
 
 
  **Example**:
 
 
     from conan.packager import ConanMultiPackager
@@ -719,15 +746,15 @@
 ### Generating multiple references for the same recipe
 
 You can add a different reference in the builds tuple, so for example, if your recipe has no "version"
 field, you could generate several versions in the same build script. Conan package tools will export
 the recipe using the different reference automatically:
 
     from conan.packager import ConanMultiPackager
-    
+
     if __name__ == '__main__':
         builder = ConanMultiPackager()
         builder.add_common_builds(reference="mylib/1.0@conan/stable")
         builder.add_common_builds(reference="mylib/2.0@conan/stable")
         builder.run()
 
 
@@ -818,15 +845,16 @@
 - **clang_versions**: List with a subset of clang_versions. Default ["3.8", "3.9", "4.0"]
 - **apple_clang_versions**: List with a subset of apple-clang versions. Default ["6.1", "7.3", "8.0"]
 - **visual_versions**: List with a subset of Visual Studio versions. Default [10, 12, 14]
 - **visual_runtimes**: List containing Visual Studio runtimes to use in builds. Default ["MT", "MD", "MTd", "MDd"]
 - **mingw_configurations**: Configurations for MinGW
 - **archs**: List containing specific architectures to build for. Default ["x86", "x86_64"]
 - **use_docker**: Use docker for package creation in Linux systems.
-- **docker_image_skip_update**: If defined, it will skip the initialisation update of "conan package tools" and "conan" in the docker image. By default is False.
+- **docker_image_skip_update**: If defined, it will skip the initialization update of "conan package tools" and "conan" in the docker image. By default is False.
+- **docker_entry_script**: Command to be executed before to build when running Docker.
 - **curpage**: Current page of packages to create
 - **total_pages**: Total number of pages
 - **vs10_x86_64_enabled**: Flag indicating whether or not to build for VS10 64bits. Default [False]
 - **upload_retry**: Num retries in upload in case of failure.
 - **remotes**: List of URLs separated by "," for the additional remotes (read).
 - **upload**: URL of the repository where we want to use to upload the packages.
 - **upload_only_when_stable**: Will try to upload only if the channel is the stable channel
@@ -875,26 +903,27 @@
 - **CONAN_REFERENCE**: Reference of the package to upload, e.g. "zlib/1.2.8"
 - **CONAN_PASSWORD**: Conan Password, or API key if you are using Bintray.
 - **CONAN_REMOTES**: List of URLs separated by "," for the additional remotes (read).
 - **CONAN_UPLOAD**: URL of the repository where we want to use to upload the packages.
 - **CONAN_UPLOAD_RETRY**: If defined, in case of fail retries to upload again the specified times
 - **CONAN_UPLOAD_ONLY_WHEN_STABLE**: If defined, will try to upload the packages only when the current channel is the stable one.
 - **CONAN_SKIP_CHECK_CREDENTIALS**: Force to check user credentials before to build when upload is required. By default is False.
+- **CONAN_DOCKER_ENTRY_SCRIPT**: Command to be executed before to build when running Docker.
 - **CONAN_GCC_VERSIONS**: Gcc versions, comma separated, e.g. "4.6,4.8,5,6"
 - **CONAN_CLANG_VERSIONS**: Clang versions, comma separated, e.g. "3.8,3.9,4.0"
 - **CONAN_APPLE_CLANG_VERSIONS**: Apple clang versions, comma separated, e.g. "6.1,8.0"
 - **CONAN_ARCHS**: Architectures to build for, comma separated, e.g. "x86,x86_64"
 - **CONAN_BUILD_TYPES**: Build types to build for, comma separated, e.g. "Release,Debug"
 - **CONAN_VISUAL_VERSIONS**: Visual versions, comma separated, e.g. "12,14"
 - **CONAN_VISUAL_RUNTIMES**: Visual runtimes, comma separated, e.g. "MT,MD"
 - **CONAN_USE_DOCKER**: If defined will use docker
 - **CONAN_CURRENT_PAGE**:  Current page of packages to create
 - **CONAN_TOTAL_PAGES**: Total number of pages
 - **CONAN_DOCKER_IMAGE**: If defined and docker is being used, it will use this dockerimage instead of the default images, e.g. "lasote/conangcc63"
-- **CONAN_DOCKER_IMAGE_SKIP_UPDATE**: If defined, it will skip the initialisation update of "conan package tools" and "conan" in the docker image. By default is False.
+- **CONAN_DOCKER_IMAGE_SKIP_UPDATE**: If defined, it will skip the initialization update of "conan package tools" and "conan" in the docker image. By default is False.
 - **CONAN_STABLE_BRANCH_PATTERN**: Regular expression, if current git branch matches this pattern, the packages will be uploaded to *CONAN_STABLE_CHANNEL* channel. Default "master". E.j: "release/*"
 - **CONAN_STABLE_CHANNEL**: Stable channel name, default "stable"
 - **CONAN_STABLE_USERNAME**: Your conan username in case the `CONAN_STABLE_BRANCH_PATTERN` matches. Optional. If not defined `CONAN_USERNAME` is used.
 - **CONAN_STABLE_PASSWORD**: Password for `CONAN_STABLE_USERNAME`. Default: `CONAN_PASSWORD`
 - **CONAN_CHANNEL**: Channel where your packages will be uploaded if the previous parameter doesn't match
 - **CONAN_PIP_PACKAGE**: Specify a conan package to install (by default, installs the latest) e.j conan==0.0.1rc7
 - **MINGW_CONFIGURATIONS**: Specify a list of MinGW builds. See MinGW builds section.
@@ -903,8 +932,7 @@
 - **CONAN_DOCKER_USE_SUDO** Force to use "sudo" when invoking conan. By default, only with Windows. "False" to deactivate.
 - **CONAN_ALLOW_GCC_MINORS** Declare this variable if you want to allow gcc >=5 versions with the minor (5.1, 6.3 etc).
 - **CONAN_EXCLUDE_VCVARS_PRECOMMAND** For Visual Studio builds, it exclude the vcvars call to set the environment.
 
 # Full example
 
 You can see the full zlib example [here](https://github.com/lasote/conan-zlib)
-
```

### Comparing `conan_package_tools-0.8.5/setup.py` & `conan_package_tools-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `conan_package_tools-0.8.5/conan/test/packager_test.py` & `conan_package_tools-0.9.0/conan/test/packager_test.py`

 * *Files identical despite different names*

### Comparing `conan_package_tools-0.8.5/conan/test/generators_test.py` & `conan_package_tools-0.9.0/conan/test/generators_test.py`

 * *Files identical despite different names*

### Comparing `conan_package_tools-0.8.5/conan/log.py` & `conan_package_tools-0.9.0/conan/log.py`

 * *Files identical despite different names*

### Comparing `conan_package_tools-0.8.5/conan/packager.py` & `conan_package_tools-0.9.0/conan/packager.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,16 @@
                  clang_versions=None,
                  login_username=None,
                  upload_only_when_stable=False,
                  build_types=None,
                  skip_check_credentials=False,
                  allow_gcc_minors=False,
                  exclude_vcvars_precommand=False,
-                 docker_image_skip_update=False):
+                 docker_image_skip_update=False,
+                 docker_entry_script=None):
 
         self.sudo_command = ""
         if "CONAN_DOCKER_USE_SUDO" in os.environ:
             if get_bool_from_env("CONAN_DOCKER_USE_SUDO"):
                 self.sudo_command = "sudo"
         elif platform.system() == "Linux":
             self.sudo_command = "sudo"
@@ -157,14 +158,17 @@
             self.reference = ConanFileReference.loads("%s@%s/%s" % (self.reference,
                                                                     self.username, self.channel))
         self.upload_only_when_stable = upload_only_when_stable or \
                                        os.getenv("CONAN_UPLOAD_ONLY_WHEN_STABLE", False)
         self.skip_check_credentials = skip_check_credentials or \
                                       os.getenv("CONAN_SKIP_CHECK_CREDENTIALS", False)
 
+        self.docker_entry_script = docker_entry_script or \
+                                      os.getenv("CONAN_DOCKER_ENTRT_SCRIPT", None)
+
         if self.upload:
             if self.upload in ("0", "None", "False"):
                 self.upload = None
             elif self.upload == "1":
                 raise Exception("WARNING! 'upload' argument has changed. Use 'upload' argument or "
                                 "CONAN_UPLOAD environment variable to specify a remote URL to "
                                 "upload your packages. e.j: "
@@ -185,25 +189,25 @@
         if not self.gcc_versions and self.clang_versions == self.default_clang_versions:
             self.gcc_versions = self.default_gcc_versions
 
         if self.gcc_versions and not self.allow_gcc_minors:
             for a_version in self.gcc_versions:
                 if Version(a_version) >= Version("5") and "." in a_version:
                     raise Exception("""
-******************* DEPRECATED GCC MINOR VERSIONS! ***************************************                    
-                    
+******************* DEPRECATED GCC MINOR VERSIONS! ***************************************
+
 - The use of gcc versions >= 5 and specifying the minor version (e.j "5.4") is deprecated.
 - The ABI of gcc >= 5 (5, 6, and 7) is compatible between minor versions (e.j 5.3 is compatible with 5.4)
-- Specify only the major in your script: 
+- Specify only the major in your script:
    - CONAN_GCC_VERSIONS="5,6,7" if you are using environment variables.
    - gcc_versions=["5", "6", "7"] if you are using the constructor parameter.
-   
+
 You can still keep using the same docker images, or use the new "lasote/conangcc5", "lasote/conangcc6", "lasote/conangcc7"
 
-If you still want to keep the old behavior, set the environment var CONAN_ALLOW_GCC_MINORS or pass the 
+If you still want to keep the old behavior, set the environment var CONAN_ALLOW_GCC_MINORS or pass the
 "allow_gcc_minors=True" parameter. But it is not recommended, if your packages are public most users
 won't be able to use them.
 
 ******************************************************************************************
 
 """)
 
@@ -438,15 +442,16 @@
                                    build.reference,
                                    self.mingw_installer_reference, self.runner,
                                    self.args,
                                    docker_image=self.docker_image,
                                    conan_pip_package=self.conan_pip_package,
                                    docker_image_skip_update=self.docker_image_skip_update)
 
-                build_runner.run(pull_image=not pulled_docker_images[build_runner.docker_image])
+                build_runner.run(pull_image=not pulled_docker_images[build_runner.docker_image],
+                                 docker_entry_script=self.docker_entry_script)
                 pulled_docker_images[build_runner.docker_image] = True
             else:
                 build_runner = TestPackageRunner(profile, self.username, self.channel,
                                                  build.reference,
                                                  self.mingw_installer_reference, self.runner,
                                                  self.args,
                                                  conan_pip_package=self.conan_pip_package,
```

### Comparing `conan_package_tools-0.8.5/conan/builds_generator.py` & `conan_package_tools-0.9.0/conan/builds_generator.py`

 * *Files identical despite different names*

### Comparing `conan_package_tools-0.8.5/conan/create_runner.py` & `conan_package_tools-0.9.0/conan/create_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,16 @@
         self.sudo_command = ""
         if "CONAN_DOCKER_USE_SUDO" in os.environ:
             if get_bool_from_env("CONAN_DOCKER_USE_SUDO"):
                 self.sudo_command = "sudo"
         elif platform.system() == "Linux":
             self.sudo_command = "sudo"
 
-    def run(self, pull_image=True):
 
+    def run(self, pull_image=True, docker_entry_script=None):
         if pull_image:
             self.pull_image()
             if not self.docker_image_skip_update:
                 # Update the downloaded image
                 command = "%s docker run --name conan_runner %s /bin/sh -c " \
                         "\"sudo pip install conan_package_tools==%s " \
                         "--upgrade" % (self.sudo_command, self.docker_image, package_tools_version)
@@ -157,14 +157,19 @@
         command = "%s docker run --rm -v %s:/home/conan/project -v " \
                   "%s:/home/conan/.conan %s %s /bin/sh -c \"" \
                   "rm -f /home/conan/.conan/conan.conf && cd project && " \
                   "rm -f /home/conan/.conan/profiles/default && " \
                   "(conan profile new default --detect || true) && " \
                   "run_create_in_docker\"" % (self.sudo_command, os.getcwd(), self.conan_home,
                                               env_vars, self.docker_image)
+
+        # Push entry command before to build
+        if docker_entry_script:
+            command = command.replace("run_create_in_docker", "%s && run_create_in_docker" % docker_entry_script)
+
         ret = self._runner(command)
         if ret != 0:
             raise Exception("Error building: %s" % command)
 
     def pull_image(self):
         datadir = os.path.expanduser(self.data_home)
         if not os.path.exists(datadir):
```

### Comparing `conan_package_tools-0.8.5/conan_package_tools.egg-info/PKG-INFO` & `conan_package_tools-0.9.0/conan_package_tools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: conan-package-tools
-Version: 0.8.5
+Version: 0.9.0
 Summary: Packaging tools for Conan C/C++ package manager
 Home-page: https://github.com/conan-io/conan-package-tools
 Author: JFrog LTD. Luis Martinez de Bartolome
 Author-email: luism@jfrog.com
 License: MIT
+Description-Content-Type: UNKNOWN
 Description: UNKNOWN
 Keywords: conan,C/C++,package,libraries,developer,manager,dependency,tool,c,c++,cpp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `conan_package_tools-0.8.5/conan_package_tools.egg-info/SOURCES.txt` & `conan_package_tools-0.9.0/conan_package_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

