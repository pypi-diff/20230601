# Comparing `tmp/vdk-plugin-control-cli-0.1.868861548.tar.gz` & `tmp/vdk-plugin-control-cli-0.1.886059298.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-plugin-control-cli-0.1.868861548.tar", last modified: Tue May 16 12:39:55 2023, max compression
+gzip compressed data, was "vdk-plugin-control-cli-0.1.886059298.tar", last modified: Thu Jun  1 13:09:50 2023, max compression
```

## Comparing `vdk-plugin-control-cli-0.1.868861548.tar` & `vdk-plugin-control-cli-0.1.886059298.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-16 12:39:45.000000 vdk-plugin-control-cli-0.1.868861548/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     4460 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py
--rw-rw-rw-   0 root         (0) root         (0)     7407 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/execution_skip.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/properties_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     3854 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      837 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3283 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_control_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     7812 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_execution_skip.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_properties_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_vdk_plugin_control_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-06-01 13:09:41.000000 vdk-plugin-control-cli-0.1.886059298/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4460 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7435 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/execution_skip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/properties_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3854 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      837 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3283 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_control_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     7812 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_execution_skip.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_properties_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_vdk_plugin_control_cli.py
```

### Comparing `vdk-plugin-control-cli-0.1.868861548/PKG-INFO` & `vdk-plugin-control-cli-0.1.886059298/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-plugin-control-cli
-Version: 0.1.868861548
+Version: 0.1.886059298
 Summary: Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-plugin-control-cli-0.1.868861548/README.md` & `vdk-plugin-control-cli-0.1.886059298/README.md`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/setup.py` & `vdk-plugin-control-cli-0.1.886059298/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.868861548"
+__version__ = "0.1.886059298"
 
 setuptools.setup(
     name="vdk-plugin-control-cli",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py` & `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_configuration.py` & `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py` & `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/execution_skip.py` & `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/execution_skip.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,16 @@
             writer_plugin.write_termination_message(
                 configuration=configuration, execution_skipped=True
             )
             _skip_job_run(job_name)  # calls os._exit(0)
             return 1  # All other branches return None
     except Exception as exc:
         log.warning(
-            f"Error while checking for another data job excecution: {str(exc)} "
+            f"Error while checking for another data job excecution: {str(exc)} ",
+            exc_info=True,
         )
         log.warning("Printing stack trace and proceeding with execution:")
     return None
 
 
 @hookimpl(tryfirst=True)
 def vdk_configure(config_builder: ConfigurationBuilder):
```

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/properties_plugin.py` & `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/properties_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py` & `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/PKG-INFO` & `vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-plugin-control-cli
-Version: 0.1.868861548
+Version: 0.1.886059298
 Summary: Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/SOURCES.txt` & `vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/tests/test_control_service_properties.py` & `vdk-plugin-control-cli-0.1.886059298/tests/test_control_service_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/tests/test_execution_skip.py` & `vdk-plugin-control-cli-0.1.886059298/tests/test_execution_skip.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/tests/test_properties_plugin.py` & `vdk-plugin-control-cli-0.1.886059298/tests/test_properties_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.868861548/tests/test_vdk_plugin_control_cli.py` & `vdk-plugin-control-cli-0.1.886059298/tests/test_vdk_plugin_control_cli.py`

 * *Files identical despite different names*

