# Comparing `tmp/hatch_build_scripts-0.0.2.tar.gz` & `tmp/hatch_build_scripts-0.0.3.tar.gz`

## Comparing `hatch_build_scripts-0.0.2.tar` & `hatch_build_scripts-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/435c9e25cb5ee1fb
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/4586f2c83492ef12
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/63153e74ae9448e3
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/74fc00111a6357de
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/c7e9480ae051d10c
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.ruff_cache/content/fc26102941cba458
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/hatch_build_scripts/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/hatch_build_scripts/hooks.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/hatch_build_scripts/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/tests/test_plugin.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/tests/utils.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/LICENSE
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/README.md
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/pull_request_template.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/ISSUE_TEMPLATE/issue-form.yml
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/workflows/.hatch-run.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/workflows/check.yml
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/hatch_build_scripts/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/hatch_build_scripts/hooks.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/hatch_build_scripts/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/tests/test_plugin.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/tests/utils.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/README.md
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 hatch_build_scripts-0.0.3/PKG-INFO
```

### Comparing `hatch_build_scripts-0.0.2/hatch_build_scripts/plugin.py` & `hatch_build_scripts-0.0.3/hatch_build_scripts/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 import shutil
-from dataclasses import dataclass
+from dataclasses import MISSING, dataclass, fields
 from functools import cached_property
 from pathlib import Path
 from subprocess import run
 from typing import Any, Sequence
 
 import pathspec
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
@@ -18,96 +18,80 @@
 class BuildScriptsHook(BuildHookInterface):
     PLUGIN_NAME = "build-scripts"
 
     def initialize(
         self,
         version: str,  # noqa: ARG002
         build_data: dict[str, Any],
-    ) -> bool | None:
+    ) -> None:
         created: set[Path] = set()
 
         all_scripts = load_scripts(self.config)
 
-        for script in all_scripts.scripts:
+        for script in all_scripts:
             if script.clean_out_dir:
                 out_dir = Path(self.root, script.out_dir)
                 logger.info(f"Cleaning {out_dir}")
                 shutil.rmtree(out_dir, ignore_errors=True)
             elif script.clean_artifacts:
-                for file in script.out_files(self.root):
-                    file.unlink(missing_ok=True)
+                for out_file in script.out_files(self.root):
+                    out_file.unlink(missing_ok=True)
 
-        for script in all_scripts.scripts:
+        for script in all_scripts:
             work_dir = Path(self.root, script.work_dir)
             out_dir = Path(self.root, script.out_dir)
             out_dir.mkdir(parents=True, exist_ok=True)
 
             for cmd in script.commands:
                 run(cmd, cwd=str(work_dir), check=True, shell=True)  # noqa: S602
 
             logger.info(f"Copying artifacts to {out_dir}")
-            for file in script.artifacts_spec.match_tree(work_dir):
-                src_file = work_dir / file
-                out_file = out_dir / file
+            for artifact_file in script.artifact_files():
+                src_file = work_dir / artifact_file
+                out_file = out_dir / artifact_file
                 if src_file not in created:
                     out_file.parent.mkdir(parents=True, exist_ok=True)
                     shutil.copyfile(src_file, out_file)
                     created.add(out_file)
 
             build_data["artifacts"].append(str(out_dir.relative_to(self.root)))
 
 
-def load_scripts(config: dict[str, Any]) -> AllScriptsConfig:
-    script_defaults = {
-        "work_dir": config.get("work_dir", "."),
-        "out_dir": config.get("out_dir", "."),
-        "clean_artifacts": config.get("clean_artifacts", True),
-        "clean_out_dir": config.get("clean_out_dir", False),
-    }
-
-    return AllScriptsConfig(
-        scripts=[
-            OneScriptConfig(**{**script_defaults, **script_config})
-            for script_config in config.get("scripts", [])
-        ],
-    )
-
-
-@dataclass
-class AllScriptsConfig:
-    """A configuration for a set of build scripts."""
-
-    scripts: Sequence[OneScriptConfig]
-    """A list of build scripts to run"""
+def load_scripts(config: dict[str, Any]) -> Sequence[OneScriptConfig]:
+    script_defaults = dataclass_defaults(OneScriptConfig)
+    script_defaults.update({k: config[k] for k in script_defaults if k in config})
+    return [
+        OneScriptConfig(**{**script_defaults, **script_config})
+        for script_config in config.get("scripts", [])
+    ]
 
 
 @dataclass
 class OneScriptConfig:
     """A configuration for a single build script."""
 
     commands: Sequence[str]
     """The commands to run"""
 
     artifacts: Sequence[str]
-    """A list of file patterns relative to the work_dir to save as build artifacts"""
+    """Git file patterns relative to the work_dir to save as build artifacts"""
 
-    out_dir: str
+    out_dir: str = "."
     """The path where build artifacts will be saved"""
 
-    work_dir: str
+    work_dir: str = "."
     """The path where the build script will be run"""
 
-    clean_artifacts: bool
+    clean_artifacts: bool = True
     """Whether to clean the build directory before running the scripts"""
 
-    clean_out_dir: bool
+    clean_out_dir: bool = False
     """Whether to clean the output directory before running the scripts"""
 
     def __post_init__(self) -> None:
-        self.artifacts = [conv_path(a) for a in self.artifacts]
         self.out_dir = conv_path(self.out_dir)
         self.work_dir = conv_path(self.work_dir)
 
     def work_files(self, root: str | Path) -> Sequence[Path]:
         """Get the files that will be used by the script."""
         work_dir = Path(root, self.work_dir)
         if not work_dir.exists():
@@ -117,16 +101,29 @@
     def out_files(self, root: str | Path) -> Sequence[Path]:
         """Get the files that will be created by the script."""
         out_dir = Path(root, self.out_dir)
         if not out_dir.exists():
             return []
         return [Path(root, self.out_dir, f) for f in self.artifacts_spec.match_tree(out_dir)]
 
+    def artifact_files(self) -> Sequence[Path]:
+        return [Path(conv_path(p)) for p in self.artifacts_spec.match_tree(self.work_dir)]
+
     @cached_property
-    def artifacts_spec(self) -> pathspec.GitIgnoreSpec:
+    def artifacts_spec(self) -> pathspec.PathSpec:
         """A pathspec for the artifacts."""
         return pathspec.PathSpec.from_lines(pathspec.patterns.GitWildMatchPattern, self.artifacts)
 
 
+def dataclass_defaults(obj: Any) -> dict[str, Any]:
+    defaults: dict[str, Any] = {}
+    for f in fields(obj):
+        if f.default is not MISSING:
+            defaults[f.name] = f.default
+        elif f.default_factory is not MISSING:
+            defaults[f.name] = f.default_factory()
+    return defaults
+
+
 def conv_path(path: str) -> str:
     """Convert a unix path to a platform-specific path."""
     return path.replace("/", os.sep)
```

### Comparing `hatch_build_scripts-0.0.2/tests/test_plugin.py` & `hatch_build_scripts-0.0.3/tests/test_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from os.path import join as joinpath
-
 from hatch_build_scripts.plugin import OneScriptConfig
 
 from .utils import create_project
 
 
 def test_plugin(tmpdir):
     (tmpdir / "some-dir").mkdir()
@@ -53,11 +51,11 @@
     )
 
     proj.build()
 
     with proj.dist() as dist:
         files = {file.filename for file in dist.filelist}
 
-        assert joinpath("fake", "fake.txt") in files
-        assert joinpath("some-dir-out", "module.py") in files
-        assert joinpath("another-dir-out", "module.py") not in files
-        assert joinpath("some-dir-out", "f3.txt") not in files
+        assert "fake/fake.txt" in files
+        assert "some-dir-out/module.py" in files
+        assert "another-dir-out/module.py" not in files
+        assert "some-dir-out/f3.txt" not in files
```

### Comparing `hatch_build_scripts-0.0.2/tests/utils.py` & `hatch_build_scripts-0.0.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.2/.gitignore` & `hatch_build_scripts-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.2/LICENSE` & `hatch_build_scripts-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_build_scripts-0.0.2/README.md` & `hatch_build_scripts-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 an array of scripts to the `tool.hatch.build.hooks.build-scripts.scripts` key in your
 `pyproject.toml` file. Each script is configured with the following keys:
 
 | Key | Default | Description |
 | --- | ------- | ----------- |
 | `commands` | required | An array of commands to run. Each command is run in a separate shell. |
 | `artifacts` | required | An array of artifact patterns (same as `.gitignore`) to include in your package distributions. |
-| `out_dir` | `"."` | The directory to run the commands in. |
+| `out_dir` | `"."` | The directory to copy artifacts into. |
 | `work_dir` | `"."` | The directory to run the commands in. All artifact patterns are relative to this directory. |
 | `clean_artifacts` | `true` | Whether to clean files from the `out_dir` that match the artifact patterns before running the commands. |
 | `clean_out_dir` | `false` | Whether to clean the `out_dir` before running the commands. |
 
 In practice this looks like:
 
 ```toml
@@ -48,11 +48,11 @@
 # you can add more scripts here...
 ```
 
 You can configure script defaults for scripts by adding a `[tool.hatch.build.hooks.build-scripts]` table to your `pyproject.toml` file. The following keys are supported:
 
 | Key | Default | Description |
 | --- | ------- | ----------- |
-| `out_dir` | `"."` | The directory to run the commands in. |
+| `out_dir` | `"."` | The directory to copy artifacts into. |
 | `work_dir` | `"."` | The directory to run the commands in. All artifact patterns are relative to this directory. |
 | `clean_artifacts` | `true` | Whether to clean files from the `out_dir` that match the artifact patterns before running the commands. |
 | `clean_out_dir` | `false` | Whether to clean the `out_dir` before running the commands. |
```

### Comparing `hatch_build_scripts-0.0.2/pyproject.toml` & `hatch_build_scripts-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -31,41 +31,32 @@
 Source = "https://github.com/rmorshea/hatch-build-scripts"
 
 [tool.hatch.version]
 path = "hatch_build_scripts/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
-  "coverage[toml]>=6.5",
   "pytest",
   "hatch",
   "toml",
   "build",
 ]
 [tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
-cov-report = [
-  "- coverage combine",
-  "coverage report",
-]
-cov = [
-  "test-cov",
-  "cov-report",
-]
+test = "pytest -vv {args:tests}"
 
 [project.entry-points.hatch]
 build-script = "hatch_build_scripts.hooks"
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
+  "hatchling",
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:hatch_build_scripts tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
@@ -134,26 +125,7 @@
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
-
-[tool.coverage.run]
-source_pkgs = ["hatch_build_scripts", "tests"]
-branch = true
-parallel = true
-omit = [
-  "hatch_build_scripts/__init__.py",
-]
-
-[tool.coverage.paths]
-hatch_build_scripts = ["hatch_build_scripts", "*/hatch-build-scripts/hatch_build_scripts"]
-tests = ["tests", "*/hatch-build-scripts/tests"]
-
-[tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
```

### Comparing `hatch_build_scripts-0.0.2/PKG-INFO` & `hatch_build_scripts-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-build-scripts
-Version: 0.0.2
+Version: 0.0.3
 Summary: A plugin for Hatch for writing build scripts
 Project-URL: Documentation, https://github.com/rmorshea/hatch-build-scripts#readme
 Project-URL: Issues, https://github.com/rmorshea/hatch-build-scripts/issues
 Project-URL: Source, https://github.com/rmorshea/hatch-build-scripts
 Author-email: rmorshea <ryan.morshead@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -44,15 +44,15 @@
 an array of scripts to the `tool.hatch.build.hooks.build-scripts.scripts` key in your
 `pyproject.toml` file. Each script is configured with the following keys:
 
 | Key | Default | Description |
 | --- | ------- | ----------- |
 | `commands` | required | An array of commands to run. Each command is run in a separate shell. |
 | `artifacts` | required | An array of artifact patterns (same as `.gitignore`) to include in your package distributions. |
-| `out_dir` | `"."` | The directory to run the commands in. |
+| `out_dir` | `"."` | The directory to copy artifacts into. |
 | `work_dir` | `"."` | The directory to run the commands in. All artifact patterns are relative to this directory. |
 | `clean_artifacts` | `true` | Whether to clean files from the `out_dir` that match the artifact patterns before running the commands. |
 | `clean_out_dir` | `false` | Whether to clean the `out_dir` before running the commands. |
 
 In practice this looks like:
 
 ```toml
@@ -71,11 +71,11 @@
 # you can add more scripts here...
 ```
 
 You can configure script defaults for scripts by adding a `[tool.hatch.build.hooks.build-scripts]` table to your `pyproject.toml` file. The following keys are supported:
 
 | Key | Default | Description |
 | --- | ------- | ----------- |
-| `out_dir` | `"."` | The directory to run the commands in. |
+| `out_dir` | `"."` | The directory to copy artifacts into. |
 | `work_dir` | `"."` | The directory to run the commands in. All artifact patterns are relative to this directory. |
 | `clean_artifacts` | `true` | Whether to clean files from the `out_dir` that match the artifact patterns before running the commands. |
 | `clean_out_dir` | `false` | Whether to clean the `out_dir` before running the commands. |
```

