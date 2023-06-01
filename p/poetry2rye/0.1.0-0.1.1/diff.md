# Comparing `tmp/poetry2rye-0.1.0.tar.gz` & `tmp/poetry2rye-0.1.1.tar.gz`

## Comparing `poetry2rye-0.1.0.tar` & `poetry2rye-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,21 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.python-version
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/requirements.lock
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/poetry2rye.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.gitignore
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.python-version
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/pyproject.toml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/requirements-dev.lock
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/requirements.lock
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/.gitignore
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/modules.xml
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/poetry2rye.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/vcs.xml
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/workspace.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/src/poetry2rye/__init__.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/src/poetry2rye/convert.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/src/poetry2rye/main.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/__p2r_backup_/src/poetry2rye/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/src/poetry2rye/__init__.py
--rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/src/poetry2rye/convert.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/src/poetry2rye/main.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/src/poetry2rye/project.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 poetry2rye-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.python-version
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/requirements.lock
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/poetry2rye.iml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/__init__.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/convert.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/main.py
+-rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/project.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/src/poetry2rye/utils.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 poetry2rye-0.1.1/PKG-INFO
```

### Comparing `poetry2rye-0.1.0/requirements-dev.lock` & `poetry2rye-0.1.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `poetry2rye-0.1.0/requirements.lock` & `poetry2rye-0.1.1/requirements-dev.lock`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,28 @@
 #   features: []
 #   all-features: false
 
 -e file:.
 apeye==1.3.0
 apeye-core==1.1.2
 attrs==23.1.0
+black==23.3.0
 certifi==2023.5.7
 charset-normalizer==3.1.0
+click==8.1.3
 dist-meta==0.8.0
 dom-toml==0.6.1
 domdf-python-tools==3.6.1
 handy-archives==0.1.4
 idna==3.4
+isort==5.12.0
+mypy-extensions==1.0.0
 natsort==8.3.1
 packaging==23.1
+pathspec==0.11.1
 platformdirs==3.5.1
 poetry-core==1.6.1
 pydantic==1.10.8
 pyproject-parser==0.9.0
 python-slugify==8.0.1
 requests==2.31.0
 shippinglabel==1.5.0
```

### Comparing `poetry2rye-0.1.0/.idea/workspace.xml` & `poetry2rye-0.1.1/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `poetry2rye-0.1.0/.idea/workspace.xml` & `poetry2rye-0.1.1/.idea/workspace.xml`

```diff
@@ -1,17 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="fd34f470-3de9-4a99-986d-899ced410e33" name="変更" comment="">
+    <list default="true" id="fd34f470-3de9-4a99-986d-899ced410e33" name="変更" comment="created">
       <change afterPath="$PROJECT_DIR$/src/poetry2rye/convert.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/poetry2rye/main.py" afterDir="false"/>
       <change afterPath="$PROJECT_DIR$/src/poetry2rye/project.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/src/poetry2rye/utils.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/requirements-dev.lock" beforeDir="false" afterPath="$PROJECT_DIR$/requirements-dev.lock" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/requirements.lock" beforeDir="false" afterPath="$PROJECT_DIR$/requirements.lock" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
@@ -44,14 +46,16 @@
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
     "last_opened_file_path": "/home/nahco314/PycharmProjects/__test_0",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
+    "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "preferences.lookFeel",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RunManager" selected="Python.convert">
     <configuration name="convert" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="poetry2rye"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
@@ -108,14 +112,16 @@
     <task active="true" id="Default" summary="デフォルトタスク">
       <changelist id="fd34f470-3de9-4a99-986d-899ced410e33" name="変更" comment=""/>
       <created>1685387054971</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1685387054971</updated>
       <workItem from="1685387055969" duration="10367000"/>
+      <workItem from="1685464921251" duration="5970000"/>
+      <workItem from="1685473028177" duration="10864000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
```

### Comparing `poetry2rye-0.1.0/__p2r_backup_/src/poetry2rye/convert.py` & `poetry2rye-0.1.1/src/poetry2rye/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import os
-from pathlib import Path
-
-from poetry.core.constraints.version import Version, VersionUnion
-
-from poetry2rye.project import PoetryProject
-from poetry.core.constraints.version.version_constraint import VersionConstraint
-from poetry.core.version.helpers import format_python_constraint, PYTHON_VERSION
-from poetry.core.constraints.version.parser import parse_constraint
-
-from copy import deepcopy
-
 import shutil
-
+from copy import deepcopy
 from itertools import filterfalse
+from pathlib import Path
+from typing import Any
 
 import tomlkit
+from poetry.core.version.helpers import format_python_constraint
+
+from poetry2rye.project import BasicDependency
+from poetry2rye.project import PoetryProject
+from poetry2rye.utils import get_next_backup_path
 
 
 def convert(project_path: Path) -> None:
-    backup_path = project_path.parent / f"__p2r_backup_{project_path.name}"
-    shutil.rmtree(backup_path, ignore_errors=True)
-    shutil.copytree(project_path, backup_path, dirs_exist_ok=True)
-    print(f"created backup: {backup_path}")
+    project_backup = get_next_backup_path(project_path)
+    shutil.copytree(project_path, project_backup, dirs_exist_ok=True, symlinks=True)
+    print(f"created backup: {project_backup}")
 
     poetry_project = PoetryProject(project_path)
 
     project_sec = {}
     urls_sec = {}
+    tool_rye_sec: dict[str, Any] = {"managed": True}
 
     # required
     project_sec["name"] = poetry_project.project_name
     project_sec["version"] = poetry_project.poetry["version"]
     project_sec["description"] = poetry_project.poetry["description"]
 
     # license (not used due to different format)
@@ -78,18 +74,23 @@
     if poetry_project.poetry.get("packages"):
         # ToDo
         pass
 
     # dependencies
     project_sec["dependencies"] = []
     for dep in poetry_project.dependencies:
-        if dep.name == "python":
+        if dep.is_python_dep():
+            assert isinstance(dep, BasicDependency)
             project_sec["requires-python"] = format_python_constraint(dep.version)
         else:
-            project_sec["dependencies"].append(f"{dep.name}{format_python_constraint(dep.version)}")
+            if dep.is_dev:
+                tool_rye_sec.setdefault("dev-dependencies", [])
+                tool_rye_sec["dev-dependencies"].append(dep.to_str())
+            else:
+                project_sec["dependencies"].append(dep.to_str())
 
     with open(project_path / "pyproject.toml") as f:
         pyproject = tomlkit.load(f)
 
     # create result
     result = tomlkit.document()
 
@@ -101,31 +102,37 @@
         if name == "project":
             continue
         elif name == "tool":
             result["tool"] = deepcopy(pyproject["tool"])
             result["tool"].pop("poetry")
         elif name == "build-system":
             result["build-system"] = deepcopy(pyproject["build-system"])
-            result["build-system"]["requires"] = list(filterfalse(lambda x: "poetry-core" in x, result["build-system"]["requires"]))
+            result["build-system"]["requires"] = list(
+                filterfalse(
+                    lambda x: "poetry-core" in x, result["build-system"]["requires"]
+                )
+            )
             result["build-system"]["requires"].append("hatchling")
             result["build-system"]["build-backend"] = "hatchling.build"
         else:
             result[name] = deepcopy(pyproject[name])
 
-    result["tool"]["rye"] = {"managed": True}
-    result["tool"]["hatch"] = {
-        "metadata": {"allow-direct-references": True}
-    }
+    result["tool"]["rye"] = tool_rye_sec
+    result["tool"]["hatch"] = {"metadata": {"allow-direct-references": True}}
 
     with open(project_path / "pyproject.toml", "w") as f:
         f.write(tomlkit.dumps(result))
 
     # find "poetry" in pyproject.toml and print it
     with open(project_path / "pyproject.toml") as f:
         for num, content in enumerate(f.readlines(), start=1):
             if "poetry" in content:
                 print(f"Found 'poetry' in line {num}: {content}")
 
-    os.remove(project_path / "poetry.lock")
+    if (project_path / "poetry.lock").exists():
+        os.remove(project_path / "poetry.lock")
     if not (project_path / "src").exists():
         (project_path / "src").mkdir()
-        shutil.move(poetry_project.module_path, project_path / "src" / poetry_project.module_name)
+        shutil.move(
+            poetry_project.module_path,
+            project_path / "src" / poetry_project.module_name,
+        )
```

### Comparing `poetry2rye-0.1.0/__p2r_backup_/src/poetry2rye/project.py` & `poetry2rye-0.1.1/src/poetry2rye/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from pathlib import Path
 import re
+from abc import abstractmethod
+from dataclasses import dataclass
+from pathlib import Path
+from typing import Any
 from typing import Optional
 
-import slugify
 import pyproject_parser
-from pydantic import BaseModel
-from dataclasses import dataclass
-
+import slugify
+from poetry.core.constraints.version.parser import parse_constraint
 from poetry.core.constraints.version.version_constraint import VersionConstraint
 from poetry.core.version.helpers import format_python_constraint
-from poetry.core.constraints.version.parser import parse_constraint
 
 
 # unused
 def poetry_canonicalize_name(project_name: str) -> str:
     """
     Convert a project name to a canonical form by Poetry-Style.
     """
@@ -30,77 +30,116 @@
 def rye_module_name(project_name: str) -> str:
     return rye_canonicalize_name(project_name).replace("-", "_")
 
 
 @dataclass
 class Dependency:
     name: str
+    is_dev: bool
+
+    def is_python_dep(self) -> bool:
+        return False
+
+    @abstractmethod
+    def to_str(self) -> str:
+        raise NotImplementedError
+
+
+@dataclass
+class BasicDependency(Dependency):
     version: VersionConstraint
     extras: Optional[list[str]]
-    is_dev: bool
+
+    def is_python_dep(self) -> bool:
+        return self.name == "python"
+
+    def to_str(self) -> str:
+        return f"{self.name}{format_python_constraint(self.version)}"
+
+
+@dataclass
+class GitDependency(Dependency):
+    git_link: str
+
+    def to_str(self) -> str:
+        return f"{self.name} @ git+{self.git_link}"
 
 
 class PoetryProject:
     def __init__(self, project_path: Path) -> None:
         self.path = project_path
         self.project_name = rye_canonicalize_name(self.path.name)
         self.module_name = rye_module_name(self.path.name)
 
         assert (self.path / "pyproject.toml").exists(), "pyproject.toml not found"
 
         self.pyproject = pyproject_parser.PyProject.load(self.path / "pyproject.toml")
         self.poetry = self.pyproject.tool["poetry"]
 
-        assert self.pyproject.project is None, "for now, poetry2rye only supports " \
-                                               "pyproject.toml written using " \
-                                               "tool.poetry. this may change in the " \
-                                               "future."
+        assert self.pyproject.project is None, (
+            "for now, poetry2rye only supports "
+            "pyproject.toml written using "
+            "tool.poetry. this may change in the "
+            "future."
+        )
         assert self.poetry is not None, "poetry section not found in pyproject.toml"
 
         self.src_path: Path
         # this method is not exact, but tentatively we do this
         if (self.path / "src").exists():
             self.src_path = self.path / "src"
         else:
             self.src_path = self.path
 
         self.module_path = self.src_path / self.module_name
         assert self.module_path.exists(), "module not found"
 
-    @property
-    def dependencies(self) -> list[Dependency]:
+    def process_dependencies_dict(
+        self, dct: dict[str, Any], is_dev: bool
+    ) -> list[Dependency]:
         res = []
 
-        dep = self.poetry["dependencies"]
-        if dep is not None:
-            for name, item in dep.items():
-                if isinstance(item, str):
-                    res.append(Dependency(name=name, version=parse_constraint(item), extras=None, is_dev=False))
+        for name, item in dct.items():
+            if isinstance(item, str):
+                res.append(
+                    BasicDependency(
+                        name=name,
+                        version=parse_constraint(item),
+                        extras=None,
+                        is_dev=is_dev,
+                    )
+                )
+            else:
+                assert isinstance(item, dict)
+
+                if "git" in item:
+                    res.append(
+                        GitDependency(name=name, git_link=item["git"], is_dev=is_dev)
+                    )
                 else:
                     res.append(
-                        Dependency(
+                        BasicDependency(
                             name=name,
                             version=parse_constraint(item["version"]),
                             extras=item["extras"],
-                            is_dev=False,
+                            is_dev=is_dev,
                         )
                     )
 
+        return res
+
+    @property
+    def dependencies(self) -> list[Dependency]:
+        res = []
+
+        dep = self.poetry["dependencies"]
+        if dep is not None:
+            res.extend(self.process_dependencies_dict(dep, is_dev=False))
+
         try:
             dev_dep = self.poetry["group"]["dev"]["dependencies"]
         except KeyError:
             dev_dep = None
         if dev_dep is not None:
-            for name, item in dev_dep.items():
-                if isinstance(item, str):
-                    res.append(Dependency(name=name, version=parse_constraint(item), extras=None, is_dev=True))
-                else:
-                    res.append(
-                        Dependency(
-                            name=name,
-                            version=parse_constraint(item["version"]),
-                            extras=item["extras"],
-                            is_dev=True,
-                        )
-                    )
+            res.extend(self.process_dependencies_dict(dev_dep, is_dev=True))
 
         return res
```

