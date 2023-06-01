# Comparing `tmp/testbench-cli-reporter-1.2.2.tar.gz` & `tmp/testbench-cli-reporter-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testbench-cli-reporter-1.2.2.tar", last modified: Tue May  9 11:33:47 2023, max compression
+gzip compressed data, was "testbench-cli-reporter-1.2.3.tar", last modified: Thu Jun  1 14:47:12 2023, max compression
```

## Comparing `testbench-cli-reporter-1.2.2.tar` & `testbench-cli-reporter-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.152586 testbench-cli-reporter-1.2.2/
--rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.2/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)       29 2021-08-03 23:07:08.000000 testbench-cli-reporter-1.2.2/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)     9165 2023-05-09 11:33:47.152397 testbench-cli-reporter-1.2.2/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)     8447 2023-05-09 09:49:19.000000 testbench-cli-reporter-1.2.2/README.md
--rw-r--r--   0 rener      (502) wheel        (0)      171 2022-09-12 17:05:38.000000 testbench-cli-reporter-1.2.2/createPip_whl_tar.sh
--rw-r--r--   0 rener      (502) wheel        (0)     2102 2023-05-09 09:49:26.000000 testbench-cli-reporter-1.2.2/pyproject.toml
--rw-r--r--   0 rener      (502) wheel        (0)       38 2023-05-09 11:33:47.152624 testbench-cli-reporter-1.2.2/setup.cfg
--rw-r--r--   0 rener      (502) wheel        (0)     1559 2023-05-09 09:56:03.000000 testbench-cli-reporter-1.2.2/setup.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.148684 testbench-cli-reporter-1.2.2/src/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.151267 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/
--rw-r--r--   0 rener      (502) wheel        (0)      583 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)     3855 2023-05-09 11:19:28.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__main__.py
--rw-r--r--   0 rener      (502) wheel        (0)    13223 2023-05-09 11:23:34.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/actions.py
--rw-r--r--   0 rener      (502) wheel        (0)     8260 2023-05-09 11:21:17.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/config_model.py
--rw-r--r--   0 rener      (502) wheel        (0)     7297 2023-05-09 11:19:01.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/execution.py
--rw-r--r--   0 rener      (502) wheel        (0)     1048 2023-05-09 11:19:28.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/log.py
--rw-r--r--   0 rener      (502) wheel        (0)    14540 2023-05-09 11:25:08.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/questions.py
--rw-r--r--   0 rener      (502) wheel        (0)    16030 2023-05-09 10:02:34.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/testbench.py
--rw-r--r--   0 rener      (502) wheel        (0)    17489 2023-05-09 10:00:00.000000 testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/util.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-05-09 11:33:47.152185 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/
--rw-r--r--   0 rener      (502) wheel        (0)     9165 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)      706 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 rener      (502) wheel        (0)      136 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/entry_points.txt
--rw-r--r--   0 rener      (502) wheel        (0)       63 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/requires.txt
--rw-r--r--   0 rener      (502) wheel        (0)       21 2023-05-09 11:33:47.000000 testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-01 14:47:12.768317 testbench-cli-reporter-1.2.3/
+-rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.3/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)       29 2021-08-03 23:07:08.000000 testbench-cli-reporter-1.2.3/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)     9165 2023-06-01 14:47:12.768126 testbench-cli-reporter-1.2.3/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     8447 2023-05-09 09:49:19.000000 testbench-cli-reporter-1.2.3/README.md
+-rw-r--r--   0 rener      (502) wheel        (0)      171 2022-09-12 17:05:38.000000 testbench-cli-reporter-1.2.3/createPip_whl_tar.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     2102 2023-05-09 09:49:26.000000 testbench-cli-reporter-1.2.3/pyproject.toml
+-rw-r--r--   0 rener      (502) wheel        (0)       38 2023-06-01 14:47:12.768365 testbench-cli-reporter-1.2.3/setup.cfg
+-rw-r--r--   0 rener      (502) wheel        (0)     1601 2023-06-01 12:00:35.000000 testbench-cli-reporter-1.2.3/setup.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-01 14:47:12.764653 testbench-cli-reporter-1.2.3/src/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-01 14:47:12.766978 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/
+-rw-r--r--   0 rener      (502) wheel        (0)      583 2021-08-03 22:56:57.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)     3857 2023-06-01 14:43:21.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/__main__.py
+-rw-r--r--   0 rener      (502) wheel        (0)    13895 2023-06-01 14:47:04.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/actions.py
+-rw-r--r--   0 rener      (502) wheel        (0)     8721 2023-06-01 14:45:25.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/config_model.py
+-rw-r--r--   0 rener      (502) wheel        (0)     7318 2023-06-01 12:20:14.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/execution.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1048 2023-05-09 11:19:28.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/log.py
+-rw-r--r--   0 rener      (502) wheel        (0)    14540 2023-05-09 11:25:08.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/questions.py
+-rw-r--r--   0 rener      (502) wheel        (0)    16236 2023-06-01 14:46:21.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/testbench.py
+-rw-r--r--   0 rener      (502) wheel        (0)    17560 2023-06-01 14:45:25.000000 testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/util.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-01 14:47:12.767915 testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)     9165 2023-06-01 14:47:12.000000 testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)      706 2023-06-01 14:47:12.000000 testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-06-01 14:47:12.000000 testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      136 2023-06-01 14:47:12.000000 testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       63 2023-06-01 14:47:12.000000 testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       21 2023-06-01 14:47:12.000000 testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/top_level.txt
```

### Comparing `testbench-cli-reporter-1.2.2/LICENSE` & `testbench-cli-reporter-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.2/PKG-INFO` & `testbench-cli-reporter-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testbench-cli-reporter
-Version: 1.2.2
+Version: 1.2.3
 Summary: CLI Tool to Export XML-Full-Reports from TestBench
 Home-page: https://github.com/imbus/testbench-cli-reporter
 Author: imbus AG | Zacharias Daum & René Rohner
 Author-email: rene.rohner@imbus.de
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `testbench-cli-reporter-1.2.2/README.md` & `testbench-cli-reporter-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.2/pyproject.toml` & `testbench-cli-reporter-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.2/setup.py` & `testbench-cli-reporter-1.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 CURDIR = Path(__file__).absolute().parent
 
 with (CURDIR / "src" / "TestBenchCliReporter" / "__main__.py").open(encoding="utf-8") as f:
-    VERSION = re.search('\n__version__ = "(.*)"', f.read()).group(1)
+    match = re.search('\n__version__ = "(.*)"', f.read())
+    VERSION = match.group(1) if match else "unknown"
 
 with Path("README.md").open() as fh:
     long_description = fh.read()
 
 setup(
     name="testbench-cli-reporter",
     version=VERSION,
```

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__init__.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/__init__.py`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/__main__.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ImportAction,
     ImportParameters,
     loggingConfiguration,
 )
 from .execution import run_automatic_mode, run_manual_mode
 from .util import close_program, get_configuration, parser, resolve_server_name
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 
 def main():
     arg = parser.parse_args()
     try:
         if arg.config:
             cli_config = get_configuration(arg.config)
@@ -49,15 +49,15 @@
                     Configuration(
                         server_url=server,
                         verify=False,
                         basicAuth=base64.b64encode(f"{arg.login}:{arg.password}".encode()).decode(),
                         actions=[],
                     )
                 ],
-                loggingConfiguration=loggingConfiguration.from_dict({}),
+                logging_configuration=loggingConfiguration.from_dict({}),
             )
             if arg.type == "e":
                 cli_config.configuration[0].actions.append(
                     ExportAction(
                         ExportParameters(
                             outputPath=arg.path,
                             projectPath=[e for e in [arg.project, arg.version, arg.cycle] if e],
@@ -91,15 +91,15 @@
                         server_url=server,
                         verify=False,
                         loginname=arg.login,
                         password=arg.password,
                         actions=[],
                     )
                 ],
-                loggingConfiguration=loggingConfiguration.from_dict({}),
+                logging_configuration=loggingConfiguration.from_dict({}),
             )
             print("No config file given")
             run_manual_mode(cli_config)
     except KeyboardInterrupt:
         close_program()
```

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/actions.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import base64
 import contextlib
+import re
 import sys
 import traceback
 from pathlib import Path
-from typing import Any, Dict, Union
+from typing import Any, Dict, List, Union
 from xml.etree import ElementTree
 from zipfile import ZipFile
 
 from . import questions, testbench
 from .config_model import ExportParameters, ImportParameters
 from .log import logger
 from .testbench import ConnectionLog
 from .util import (
+    TYPICAL_IMPORT_CONFIG,
     AbstractAction,
-    ImportConfig,
     XmlExportConfig,
     close_program,
     get_project_keys,
     parser,
     pretty_print_project_selection,
     pretty_print_success_message,
     pretty_print_test_cases,
@@ -41,19 +42,23 @@
 
 class UnloggedAction(AbstractAction):
     def export(self):
         return None
 
 
 class ExportXMLReport(AbstractAction):
-    def __init__(self, parameters: Union[ExportParameters, Dict[str, Any]] = None):
-        if parameters and not isinstance(parameters, ExportParameters):
-            parameters = ExportParameters.from_dict(parameters)
+    def __init__(self, parameters: Union[ExportParameters, Dict[str, Any], None] = None):
+        if parameters and isinstance(parameters, ExportParameters):
+            exp_parameters = parameters
+        elif parameters is None:
+            exp_parameters = ExportParameters("report.zip")
+        else:
+            exp_parameters = ExportParameters.from_dict(parameters or {})
         super().__init__()
-        self.parameters: ExportParameters = parameters or ExportParameters("report.zip")
+        self.parameters: ExportParameters = exp_parameters
         self.filters = []
 
     def prepare(self, connection_log: ConnectionLog) -> bool:
         all_projects = connection_log.active_connection.get_all_projects()
         selected_project = questions.ask_to_select_project(all_projects)
         selected_tov = questions.ask_to_select_tov(selected_project)
         self.parameters.tovKey = selected_tov["key"]["serial"]
@@ -99,29 +104,29 @@
             self.parameters.cycleKey,
             self.parameters.reportRootUID or "ROOT",
             self.parameters.filters or [],
             self.parameters.report_config or XmlExportConfig["Itep Export"],
         )
         return self.job_id
 
-    def wait(self, connection_log: ConnectionLog) -> Union[bool, str]:
+    def wait(self, connection_log: ConnectionLog) -> bool:
         try:
             self.report_tmp_name = connection_log.active_connection.wait_for_tmp_xml_report_name(
                 self.job_id
             )
-            return self.report_tmp_name
+            return bool(self.report_tmp_name)
         except KeyError:
             logger.debug(traceback.format_exc())
             return False
 
     def poll(self, connection_log: ConnectionLog) -> bool:
         result = connection_log.active_connection.get_exp_job_result(self.job_id)
         if result is not None:
             self.report_tmp_name = result
-        return result
+        return bool(result)
 
     def finish(self, connection_log: ConnectionLog) -> bool:
         report = connection_log.active_connection.get_xml_report_data(self.report_tmp_name)
         with Path(self.parameters.outputPath).open("wb") as output_file:
             output_file.write(report)
         pretty_print_success_message(
             "Report", Path(self.parameters.outputPath).resolve(), "was generated"
@@ -134,19 +139,23 @@
         return globals()[class_name](parameters)
     except AttributeError:
         logger.error(f"Failed to create class {class_name}")
         close_program()
 
 
 class ImportExecutionResults(AbstractAction):
-    def __init__(self, parameters: Union[ImportParameters, Dict[str, Any]] = None):
-        if parameters and not isinstance(parameters, ImportParameters):
-            parameters = ImportParameters.from_dict(parameters)
+    def __init__(self, parameters: Union[ImportParameters, Dict[str, Any], None] = None):
+        if parameters and isinstance(parameters, ImportParameters):
+            imp_parameters = parameters
+        elif parameters is None:
+            imp_parameters = ImportParameters("result.zip")
+        else:
+            imp_parameters = ImportParameters.from_dict(parameters)
         super().__init__()
-        self.parameters: ImportParameters = parameters or ImportParameters("result.zip")
+        self.parameters: ImportParameters = imp_parameters
 
     def prepare(self, connection_log: ConnectionLog) -> bool:
         self.parameters.inputPath = questions.ask_for_input_path()
         project = version = cycle = None
         with contextlib.suppress(Exception):
             project, version, cycle = self.get_project_path_from_report()
 
@@ -165,77 +174,86 @@
         )
         self.parameters.defaultTester = questions.ask_to_select_default_tester(available_testers)
         all_filters = connection_log.active_connection.get_all_filters()
         self.parameters.filters = questions.ask_to_select_filters(all_filters)
         self.parameters.importConfig = questions.ask_to_config_import()
         return True
 
-    def get_project_path_from_report(self):
+    def get_project_path_from_report(self) -> List:
         with ZipFile(self.parameters.inputPath) as zip_file:
             xml = ElementTree.fromstring(zip_file.read("report.xml"))
-            project = xml.find("./header/project").get("name")
-            version = xml.find("./header/version").get("name")
-            cycle = xml.find("./header/cycle").get("name")
-            return project, version, cycle
+            project_element = xml.find("./header/project")
+            project = project_element.get("name") if project_element is not None else ""
+            version_element = xml.find("./header/version")
+            version = version_element.get("name") if version_element is not None else ""
+            cycle_element = xml.find("./header/cycle")
+            cycle = cycle_element.get("name") if cycle_element is not None else ""
+            return [project, version, cycle]
 
     def trigger(self, connection_log: ConnectionLog) -> bool:
         if not self.parameters.cycleKey:
             if len(self.parameters.projectPath or []) != 3:  # noqa: PLR2004
                 self.parameters.projectPath = self.get_project_path_from_report()
             self.set_cycle_key_from_path(connection_log)
 
         with Path(self.parameters.inputPath).open("rb") as execution_report:
             execution_report_base64 = base64.b64encode(execution_report.read()).decode()
 
         serverside_file_name = connection_log.active_connection.upload_execution_results(
             execution_report_base64
         )
+        if not self.parameters.cycleKey:
+            raise ValueError("Invalid Config! 'cycleKey' missing.")
         if serverside_file_name:
             self.job_id = connection_log.active_connection.trigger_execution_results_import(
                 self.parameters.cycleKey,
                 self.parameters.reportRootUID or "ROOT",
                 serverside_file_name,
                 self.parameters.defaultTester,
                 self.parameters.filters or [],
-                self.parameters.importConfig or ImportConfig["Typical"],
+                self.parameters.importConfig or TYPICAL_IMPORT_CONFIG,
             )
             return True
-        return None
+        return False
 
     def set_cycle_key_from_path(self, connection_log: ConnectionLog):
         all_projects = connection_log.active_connection.get_all_projects()
-        (
-            project_key,
-            tov_key,
-            self.parameters.cycleKey,
-        ) = get_project_keys(all_projects, *self.parameters.projectPath)
+        if (
+            isinstance(self.parameters.projectPath, list)
+            and len(self.parameters.projectPath) == 3  # noqa: PLR2004
+        ):
+            (
+                project_key,
+                tov_key,
+                self.parameters.cycleKey,
+            ) = get_project_keys(all_projects, *self.parameters.projectPath)
         if not self.parameters.cycleKey:
             raise ValueError("Invalid Config! 'cycleKey' missing.")
 
     def wait(self, connection_log: ConnectionLog) -> bool:
         self.report_tmp_name = (
             connection_log.active_connection.wait_for_execution_results_import_to_finish(
                 self.job_id
             )
         )
-        return self.report_tmp_name
+        return bool(self.report_tmp_name)
 
     def poll(self, connection_log: ConnectionLog) -> bool:
         result = connection_log.active_connection.get_imp_job_result(self.job_id)
         if result is not None:
             self.report_tmp_name = result
-        return result
+        return bool(result)
 
     def finish(self, connection_log: ConnectionLog) -> bool:
         if self.report_tmp_name:
             pretty_print_success_message(
                 "Report", Path(self.parameters.inputPath).resolve(), "was imported"
             )
             return True
-        return None
+        return False
 
 
 class BrowseProjects(UnloggedAction):
     def prepare(self, connection_log: ConnectionLog) -> bool:
         arg = parser.parse_args()
         project = arg.project
         version = arg.version
@@ -251,32 +269,28 @@
             )
         else:
             tttree_structure = connection_log.active_connection.get_test_cycle_structure(
                 selected_cycle["key"]["serial"]
             )
         selected_uid = questions.ask_to_select_report_root_uid(tttree_structure)
         for tse in tttree_structure:
-            if tse.get("TestTheme_structure"):
-                info = tse.get("TestTheme_structure")
-                typ = "TestTheme"
-            elif tse.get("TestCaseSet_structure"):
-                info = tse.get("TestCaseSet_structure")
-                typ = "TestCaseSet"
-            elif tse.get("Root_structure"):
-                info = tse.get("Root_structure")
-                typ = "Root"
-            else:
-                raise ValueError(f"Unknown Element Type: {str(tse)}")
+            info, typ = self.get_test_structure_element_info(tse)
             if info.get("uniqueID") == selected_uid:
                 pretty_print_tse_information(tse, typ, info)
                 if typ == "TestCaseSet":
                     test_cases = connection_log.active_connection.get_test_cases(tse)
                     pretty_print_test_cases(test_cases)
         return True
 
+    def get_test_structure_element_info(self, tse):
+        for key, value in tse.items():
+            if re.match(r".*_structure$", key):
+                return value, re.sub(r"_structure$", "", key)
+        raise ValueError(f"Unknown Element Type: {str(tse)}")
+
     def trigger(self, connection_log: ConnectionLog) -> bool:
         return True
 
 
 class ExportActionLog(UnloggedAction):
     def prepare(self, connection_log: ConnectionLog):
         self.parameters["outputPath"] = questions.ask_for_output_path("config.json")
```

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/config_model.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/config_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -227,28 +227,40 @@
 
 
 @dataclass
 class loggingConfiguration:  # noqa: N801
     console: Optional[ConsoleLoggerConfig] = None
     file: Optional[FileLoggerConfig] = None
 
+    def __post_init__(self):
+        if self.console is None:
+            self.console = ConsoleLoggerConfig.from_dict({})
+        if self.file is None:
+            self.file = FileLoggerConfig.from_dict({})
+
     @classmethod
     def from_dict(cls, dictionary):
         return cls(
             console=ConsoleLoggerConfig.from_dict(dictionary.get("console") or {}),
             file=FileLoggerConfig.from_dict(dictionary.get("file") or {}),
         )
 
 
 @dataclass
 class CliReporterConfig:
-    configuration: List[Configuration]
-    loggingConfiguration: loggingConfiguration
+    configuration: Optional[List[Configuration]] = None
+    logging_configuration: Optional[loggingConfiguration] = None
+
+    def __post_init__(self):
+        if self.configuration is None:
+            self.configuration = []
+        if self.logging_configuration is None:
+            self.logging_configuration = loggingConfiguration()
 
     @classmethod
     def from_dict(cls, dictionary):
         return cls(
             configuration=[Configuration.from_dict(c) for c in dictionary.get("configuration", [])],
-            loggingConfiguration=loggingConfiguration.from_dict(
+            logging_configuration=loggingConfiguration.from_dict(
                 dictionary.get("loggingConfiguration") or {}
             ),
         )
```

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/execution.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import traceback
 from time import sleep
 from typing import Any, Dict, Optional, Union
 
-import requests.exceptions
+import requests.exceptions  # type: ignore
 from requests import Timeout
 
 from . import questions
 from .actions import Action
 from .config_model import CliReporterConfig, Configuration, LogLevel
 from .log import logger, setup_logger
 from .testbench import Connection, ConnectionLog, login
 from .util import rotate, spin_spinner
 
 
 def run_manual_mode(configuration: Optional[CliReporterConfig] = None):
     cli_config: CliReporterConfig = (
         CliReporterConfig(configuration=[]) if configuration is None else configuration
     )
-    cli_config.loggingConfiguration.file = None
-    cli_config.loggingConfiguration.console.logLevel = LogLevel.INFO
-    cli_config.loggingConfiguration.console.logFormat = "%(message)s"
-    setup_logger(cli_config.loggingConfiguration)
+    cli_config.logging_configuration.file = None
+    cli_config.logging_configuration.console.logLevel = LogLevel.INFO
+    cli_config.logging_configuration.console.logFormat = "%(message)s"
+    setup_logger(cli_config.logging_configuration)
 
     print("Starting manual mode")
     connection_log = ConnectionLog()
 
     while True:
         config = cli_config.configuration[0] if len(cli_config.configuration) else Configuration("")
         active_connection = login(config.server_url, config.loginname, config.password)
@@ -64,15 +64,15 @@
     raise_exceptions: bool = False,
 ):
     config = (
         configuration
         if isinstance(configuration, CliReporterConfig)
         else CliReporterConfig.from_dict(configuration)
     )
-    setup_logger(config.loggingConfiguration)
+    setup_logger(config.logging_configuration)
     logger.info("Run Automatic Mode")
     connection_queue = ConnectionLog()
     try:
         fill_connection_queue(config, connection_queue, loginname, password)
         trigger_all_actions(connection_queue, raise_exceptions)
         poll_and_finish_actions(connection_queue, raise_exceptions)
         logger.info("All jobs finished.")
```

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/log.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/log.py`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/questions.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/questions.py`

 * *Files identical despite different names*

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/testbench.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/testbench.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 import base64
 import dataclasses
 import json
 import traceback
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
-import requests
+import requests  # type: ignore
 import urllib3
 from questionary import print as pprint
 
 from . import questions
 from .config_model import (
     CliReporterConfig,
     Configuration,
     ExecutionResultsImportOptions,
+    FilterInfo,
 )
 from .log import logger
 from .util import (
+    TYPICAL_IMPORT_CONFIG,
     AbstractAction,
-    ImportConfig,
     XmlExportConfig,
     close_program,
     spin_spinner,
 )
 
 
 class Connection:
@@ -44,26 +45,26 @@
         self,
         server_url: str,
         verify: Union[bool, str],
         basicAuth: Optional[str] = None,
         loginname: Optional[str] = None,
         password: Optional[str] = None,
         job_timeout_sec: int = 4 * 60 * 60,
-        connection_timeout_sec: int = None,
+        connection_timeout_sec: Optional[int] = None,
         actions: Optional[List] = None,
         **kwargs,
     ):
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
         self.server_url = server_url
         if basicAuth:
             credentials = base64.b64decode(basicAuth.encode()).decode("utf-8")
             self.loginname, self.password = credentials.split(":", 1)
         else:
-            self.loginname = loginname
-            self.password = password
+            self.loginname = loginname or ""
+            self.password = password or ""
         self.job_timeout_sec = job_timeout_sec
         self.action_log: List[AbstractAction] = []
         self.actions_to_trigger: List[dict] = actions or []
         self.actions_to_wait_for: List[AbstractAction] = []
         self.actions_to_finish: List[AbstractAction] = []
         self.connection_timeout = connection_timeout_sec
         self.verify_ssl = verify
@@ -114,18 +115,20 @@
         )
 
         response.json()
 
         return True
 
     def get_all_projects(self) -> Dict:
-        all_projects = self.session.get(
-            f"{self.server_url}projects",
-            params={"includeTOVs": "true", "includeCycles": "true"},
-        ).json()
+        all_projects = dict(
+            self.session.get(
+                f"{self.server_url}projects",
+                params={"includeTOVs": "true", "includeCycles": "true"},
+            ).json()
+        )
         all_projects["projects"].sort(key=lambda proj: proj["name"].casefold())
         return all_projects
 
     def get_all_filters(self) -> List[dict]:
         all_filters = self.session.get(
             f"{self.server_url}filters",
         )
@@ -226,31 +229,33 @@
 
     def trigger_execution_results_import(
         self,
         cycle_key: str,
         report_root_uid: str,
         serverside_file_name: str,
         default_tester: str,
-        filters: List[Dict[str, str]],
+        filters: Union[List[FilterInfo], List[Dict[str, str]]],
         import_config: Optional[ExecutionResultsImportOptions] = None,
     ) -> str:
         if import_config is None:
-            import_config = ImportConfig["Typical"]
-        import_config.fileName = serverside_file_name
-        import_config.filters = filters
+            used_import_config = TYPICAL_IMPORT_CONFIG
+        else:
+            used_import_config = import_config
+        used_import_config.fileName = serverside_file_name
+        used_import_config.filters = filters
         if default_tester:
-            import_config.defaultTester = default_tester
+            used_import_config.defaultTester = default_tester
         if report_root_uid and report_root_uid != "ROOT":
-            import_config.reportRootUID = report_root_uid
+            used_import_config.reportRootUID = report_root_uid
 
         try:
             job_id = self.session.post(
                 f"{self.server_url}cycle/{cycle_key}/executionResultsImport",
                 headers={"Accept": "application/zip"},
-                json=dataclasses.asdict(import_config),
+                json=dataclasses.asdict(used_import_config),
             )
             return job_id.json()["jobID"]
         except requests.exceptions.HTTPError as e:
             self.render_import_error(e)
             raise e
 
     def wait_for_execution_results_import_to_finish(self, job_id: str) -> bool:
@@ -260,15 +265,15 @@
                 if import_status is not None:
                     break
                 spin_spinner("Waiting until import of execution results is done")
 
             result = import_status["result"]
 
             if "Right" in result:
-                return result["Right"]
+                return True
             raise AssertionError(result)
         except requests.exceptions.RequestException as e:
             self.render_import_error(e)
             raise e
 
     def render_import_error(self, e):
         pprint("!!!ERROR DURING IMPORT!!!", style="#ff0e0e italic")
```

### Comparing `testbench-cli-reporter-1.2.2/src/TestBenchCliReporter/util.py` & `testbench-cli-reporter-1.2.3/src/TestBenchCliReporter/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import sys
 import time
 import traceback
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from pathlib import Path
 from re import fullmatch
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 
 from questionary import print as pprint
 
 from .config_model import (
     CliReporterConfig,
     ExecutionResultsImportOptions,
     ExportAction,
@@ -35,25 +35,27 @@
 )
 from .log import logger
 
 BLUE_ITALIC = "#06c8ff italic"
 
 BLUE_BOLD_ITALIC = "#06c8ff bold italic"
 
+TYPICAL_IMPORT_CONFIG: ExecutionResultsImportOptions = ExecutionResultsImportOptions(
+    fileName="",
+    reportRootUID=None,
+    ignoreNonExecutedTestCases=True,
+    defaultTester=None,
+    checkPaths=True,
+    filters=None,
+    discardTesterInformation=True,
+    useExistingDefect=True,
+)
+
 ImportConfig = {
-    "Typical": ExecutionResultsImportOptions(
-        fileName="",
-        reportRootUID=None,
-        ignoreNonExecutedTestCases=True,
-        defaultTester=None,
-        checkPaths=True,
-        filters=None,
-        discardTesterInformation=True,
-        useExistingDefect=True,
-    ),
+    "Typical": TYPICAL_IMPORT_CONFIG,
     "<CUSTOM>": False,
 }
 
 
 XmlExportConfig = {
     "Itep Export": TestCycleXMLReportOptions(
         exportAttachments=True,
@@ -250,15 +252,15 @@
     return li
 
 
 def pretty_print(*print_statements: dict):
     try:
         for statement in print_statements:
             pprint(
-                statement.get("value"),
+                statement.get("value", ""),
                 style=statement.get("style", None),
                 end=statement.get("end", "\r\n"),
             )
     except Exception:
         print("".join([statement["value"] for statement in print_statements]))
 
 
@@ -583,15 +585,15 @@
 
 ACTION_TYPES = {"ImportExecutionResults": ImportAction, "ExportXMLReport": ExportAction}
 
 
 class AbstractAction(ABC):
     def __init__(self, parameters: Optional[dict] = None):
         self.parameters = parameters or {}
-        self.report_tmp_name = ""
+        self.report_tmp_name: Union[str, bool] = ""
         self.job_id = ""
 
     def prepare(self, connection_log) -> bool:
         return True
 
     @abstractmethod
     def trigger(self, connection_log) -> bool:
```

### Comparing `testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/PKG-INFO` & `testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testbench-cli-reporter
-Version: 1.2.2
+Version: 1.2.3
 Summary: CLI Tool to Export XML-Full-Reports from TestBench
 Home-page: https://github.com/imbus/testbench-cli-reporter
 Author: imbus AG | Zacharias Daum & René Rohner
 Author-email: rene.rohner@imbus.de
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `testbench-cli-reporter-1.2.2/src/testbench_cli_reporter.egg-info/SOURCES.txt` & `testbench-cli-reporter-1.2.3/src/testbench_cli_reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

