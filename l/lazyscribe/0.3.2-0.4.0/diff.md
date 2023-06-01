# Comparing `tmp/lazyscribe-0.3.2-py3-none-any.whl.zip` & `tmp/lazyscribe-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,20 @@
-Zip file size: 10490 bytes, number of entries: 10
--rw-r--r--  2.0 unx      243 b- defN 23-Feb-01 02:08 lazyscribe/__init__.py
--rw-r--r--  2.0 unx       38 b- defN 23-Feb-01 02:08 lazyscribe/_meta.py
--rw-r--r--  2.0 unx     8015 b- defN 23-Feb-01 02:08 lazyscribe/experiment.py
--rw-r--r--  2.0 unx     2639 b- defN 23-Feb-01 02:08 lazyscribe/linked.py
--rw-r--r--  2.0 unx    14374 b- defN 23-Feb-01 02:08 lazyscribe/project.py
--rw-r--r--  2.0 unx     1253 b- defN 23-Feb-01 02:08 lazyscribe/test.py
--rw-r--r--  2.0 unx     4546 b- defN 23-Feb-01 02:09 lazyscribe-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-01 02:09 lazyscribe-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Feb-01 02:09 lazyscribe-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      774 b- defN 23-Feb-01 02:09 lazyscribe-0.3.2.dist-info/RECORD
-10 files, 31985 bytes uncompressed, 9180 bytes compressed:  71.3%
+Zip file size: 22988 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      243 b- defN 23-Jun-01 17:28 lazyscribe/__init__.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-01 17:28 lazyscribe/_meta.py
+-rw-r--r--  2.0 unx    14421 b- defN 23-Jun-01 17:28 lazyscribe/experiment.py
+-rw-r--r--  2.0 unx     2639 b- defN 23-Jun-01 17:28 lazyscribe/linked.py
+-rw-r--r--  2.0 unx    16855 b- defN 23-Jun-01 17:28 lazyscribe/project.py
+-rw-r--r--  2.0 unx     1253 b- defN 23-Jun-01 17:28 lazyscribe/test.py
+-rw-r--r--  2.0 unx      831 b- defN 23-Jun-01 17:28 lazyscribe/artifacts/__init__.py
+-rw-r--r--  2.0 unx     3835 b- defN 23-Jun-01 17:28 lazyscribe/artifacts/base.py
+-rw-r--r--  2.0 unx     4762 b- defN 23-Jun-01 17:28 lazyscribe/artifacts/joblib.py
+-rw-r--r--  2.0 unx     3140 b- defN 23-Jun-01 17:28 lazyscribe/artifacts/json.py
+-rw-r--r--  2.0 unx      529 b- defN 23-Jun-01 17:28 lazyscribe/prefect/__init__.py
+-rw-r--r--  2.0 unx     8475 b- defN 23-Jun-01 17:28 lazyscribe/prefect/experiment.py
+-rw-r--r--  2.0 unx     9269 b- defN 23-Jun-01 17:28 lazyscribe/prefect/project.py
+-rw-r--r--  2.0 unx     2100 b- defN 23-Jun-01 17:28 lazyscribe/prefect/test.py
+-rw-r--r--  2.0 unx     4726 b- defN 23-Jun-01 17:29 lazyscribe-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 17:29 lazyscribe-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-01 17:29 lazyscribe-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1464 b- defN 23-Jun-01 17:29 lazyscribe-0.4.0.dist-info/RECORD
+18 files, 74683 bytes uncompressed, 20600 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -12,20 +12,44 @@
 
 Filename: lazyscribe/project.py
 Comment: 
 
 Filename: lazyscribe/test.py
 Comment: 
 
-Filename: lazyscribe-0.3.2.dist-info/METADATA
+Filename: lazyscribe/artifacts/__init__.py
 Comment: 
 
-Filename: lazyscribe-0.3.2.dist-info/WHEEL
+Filename: lazyscribe/artifacts/base.py
 Comment: 
 
-Filename: lazyscribe-0.3.2.dist-info/top_level.txt
+Filename: lazyscribe/artifacts/joblib.py
 Comment: 
 
-Filename: lazyscribe-0.3.2.dist-info/RECORD
+Filename: lazyscribe/artifacts/json.py
+Comment: 
+
+Filename: lazyscribe/prefect/__init__.py
+Comment: 
+
+Filename: lazyscribe/prefect/experiment.py
+Comment: 
+
+Filename: lazyscribe/prefect/project.py
+Comment: 
+
+Filename: lazyscribe/prefect/test.py
+Comment: 
+
+Filename: lazyscribe-0.4.0.dist-info/METADATA
+Comment: 
+
+Filename: lazyscribe-0.4.0.dist-info/WHEEL
+Comment: 
+
+Filename: lazyscribe-0.4.0.dist-info/top_level.txt
+Comment: 
+
+Filename: lazyscribe-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lazyscribe/_meta.py

```diff
@@ -1,3 +1,3 @@
 """Version."""
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
```

## lazyscribe/experiment.py

```diff
@@ -1,19 +1,24 @@
 """Experiment dataclass."""
 
 import getpass
+import inspect
+import json
 import logging
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Union
 
-from attrs import Factory, asdict, define, field, frozen
+from attrs import Factory, asdict, define, field, fields, filters, frozen
+from fsspec.implementations.local import LocalFileSystem
+from fsspec.spec import AbstractFileSystem
 from slugify import slugify
 
+from .artifacts import Artifact, _get_handler
 from .test import Test
 
 LOG = logging.getLogger(__name__)
 
 
 def serializer(inst, field, value):
     """Datetime and dependencies converter for :meth:`attrs.asdict`.
@@ -36,14 +41,34 @@
         return value.isoformat(timespec="seconds")
     if field is not None and field.name == "dependencies":
         new = [f"{exp.project}|{exp.slug}" for exp in value.values()]
         return new
     if field is not None and field.name == "tests":
         new = [asdict(test) for test in value]
         return new
+    if field is not None and field.name == "artifacts":
+        new = [
+            {
+                **asdict(
+                    artifact,
+                    filter=filters.exclude(
+                        fields(type(artifact)).value,
+                        fields(type(artifact)).writer_kwargs,
+                    ),
+                    value_serializer=lambda _, __, value: value.isoformat(
+                        timespec="seconds"
+                    )
+                    if isinstance(value, datetime)
+                    else value,
+                ),
+                "handler": artifact.alias,
+            }
+            for artifact in value
+        ]
+        return new
 
     return value
 
 
 @define
 class Experiment:
     """Experiment data class.
@@ -72,36 +97,49 @@
         A dictionary of upstream project experiments. The key is the short slug for the upstream
         experiment and the value is an :class:`Experiment` instance.
     """
 
     name: str
     project: Path = field(eq=False)
     dir: Path = field(eq=False)
+    fs: AbstractFileSystem = field(eq=False)
     author: str = Factory(getpass.getuser)
     last_updated_by: str = field()
     metrics: Dict = Factory(lambda: {})
     parameters: Dict = Factory(lambda: {})
     created_at: datetime = Factory(datetime.now)
     last_updated: datetime = Factory(datetime.now)
     dependencies: Dict = field(eq=False, factory=lambda: {})
     short_slug: str = field()
     slug: str = field()
     tests: List = Factory(lambda: [])
+    artifacts: List[Artifact] = Factory(factory=lambda: [])
 
     @dir.default
     def _dir_factory(self) -> Path:
         """Get the default directory for the project and experiment.
 
         Returns
         -------
         Path
             Absolute path to the directory.
         """
         return self.project.parent
 
+    @fs.default
+    def _fs_default(self) -> AbstractFileSystem:
+        """Define a default local filesystem implementation.
+
+        Returns
+        -------
+        LocalFileSystem
+            A standard local filesystem through ``fsspec``.
+        """
+        return LocalFileSystem()
+
     @last_updated_by.default
     def _last_updated_by_factory(self) -> str:
         """Last editor."""
         return self.author
 
     @short_slug.default
     def _short_slug_factory(self) -> str:
@@ -165,14 +203,138 @@
             The name of the parameter.
         value : Any
             The parameter itself.
         """
         self.last_updated = datetime.now()
         self.parameters[name] = value
 
+    def log_artifact(
+        self,
+        name: str,
+        value: Any,
+        handler: str,
+        fname: Optional[str] = None,
+        overwrite: bool = False,
+        **kwargs,
+    ):
+        """Log an artifact to the experiment.
+
+        This method associates an artifact with the experiment, but the artifact will
+        not be written until :py:meth:`lazyscribe.Project.save` is called.
+
+        Parameters
+        ----------
+        name : str
+            The name of the artifact.
+        value : Any
+            The object to persist to the filesystem.
+        handler : str
+            The name of the handler to use for the object.
+        fname : str, optional (default None)
+            The filename for the artifact. If not provided, it will be derived from the
+            name of the artifact and the builtin suffix for each handler.
+        overwrite : bool, optional (default False)
+            Whether or not to overwrite an existing artifact with the same name. If set to ``True``,
+            the previous artifact will be removed and overwritten with the current artifact.
+        **kwargs : dict
+            Keyword arguments for the write function of the handler.
+
+        Raises
+        ------
+        RuntimeError
+            Raised if an artifact is supplied with the same name as an existing artifact and
+            ``overwrite`` is set to ``False``.
+        """
+        # Retrieve and construct the handler
+        self.last_updated = datetime.now()
+        handler_cls = _get_handler(handler)
+        artifact_handler = handler_cls.construct(
+            name=name,
+            value=value,
+            fname=fname,
+            created_at=self.last_updated,
+            writer_kwargs=kwargs,
+        )
+        for index, artifact in enumerate(self.artifacts):
+            if artifact.name == name:
+                if overwrite:
+                    self.artifacts[index] = artifact_handler
+                    break
+                else:
+                    raise RuntimeError(
+                        f"An artifact with name {name} already exists in the experiment. Please "
+                        "use another name or set ``overwrite=True`` to replace the artifact."
+                    )
+        else:
+            self.artifacts.append(artifact_handler)
+
+    def load_artifact(self, name: str, validate: bool = True, **kwargs) -> Any:
+        """Load a single artifact.
+
+        Parameters
+        ----------
+        name : str
+            The name of the artifact to load.
+        validate : bool, optional (default True)
+            Whether or not to validate the runtime environment against the artifact
+            metadata.
+        **kwargs : dict
+            Keyword arguments for the handler read function.
+
+        Returns
+        -------
+        object
+            The artifact.
+        """
+        for artifact in self.artifacts:
+            if artifact.name == name:
+                # Construct the handler with relevant parameters.
+                artifact_attrs = {
+                    x: y
+                    for x, y in inspect.getmembers(artifact)
+                    if not x.startswith("_") and not inspect.ismethod(y)
+                }
+                exclude_params = ["value", "fname", "created_at"]
+                construct_params = [
+                    param
+                    for param in inspect.signature(artifact.construct).parameters
+                    if param not in exclude_params
+                ]
+                artifact_attrs = {
+                    key: value
+                    for key, value in artifact_attrs.items()
+                    if key in construct_params
+                }
+
+                curr_handler = type(artifact).construct(**artifact_attrs)
+
+                # Validate the handler
+                if validate and curr_handler != artifact:
+                    field_filters = filters.exclude(
+                        fields(type(artifact)).name,
+                        fields(type(artifact)).fname,
+                        fields(type(artifact)).value,
+                        fields(type(artifact)).created_at,
+                    )
+                    raise RuntimeError(
+                        "Runtime environments do not match. Artifact parameters:\n\n"
+                        f"{json.dumps(asdict(artifact, filter=field_filters))}"
+                        "\n\nCurrent parameters:\n\n"
+                        f"{json.dumps(asdict(curr_handler, filter=field_filters))}"
+                    )
+                # Read in the artifact
+                mode = "rb" if curr_handler.binary else "r"
+                with self.fs.open(self.dir / self.path / artifact.fname, mode) as buf:
+                    out = curr_handler.read(buf, **kwargs)
+                break
+        else:
+            raise ValueError(f"No artifact with name {name}")
+
+        return out
+
     @contextmanager
     def log_test(self, name: str, description: Optional[str] = None) -> Iterator[Test]:
         """Add a test to the experiment using a context handler.
 
         A test is a specific location for non-global metrics.
 
         Parameters
@@ -202,15 +364,19 @@
         -------
         Dict
             The experiment dictionary.
         """
         return asdict(
             self,
             value_serializer=serializer,
-            filter=lambda attr, _: attr.name not in ["dir", "project"],
+            filter=filters.exclude(
+                fields(Experiment).dir,
+                fields(Experiment).project,
+                fields(Experiment).fs,
+            ),
         )
 
     def __gt__(self, other):
         """Determine whether this experiment is newer than another experiment.
 
         If the experiments have the same ``slug``, this function will compare using the
         ``last_updated`` attribute. If the ``slug`` is different, this function will use
```

## lazyscribe/project.py

```diff
@@ -1,25 +1,29 @@
 """Project storing and logging."""
 
 from __future__ import annotations
 
 import getpass
 import json
+import logging
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, Iterator, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import fsspec
 
+from .artifacts import _get_handler
 from .experiment import Experiment, ReadOnlyExperiment
 from .linked import LinkedList, merge
 from .test import ReadOnlyTest, Test
 
+LOG = logging.getLogger(__name__)
+
 
 class Project:
     """Project class.
 
     Parameters
     ----------
     fpath : str, optional (default "project.json")
@@ -89,72 +93,124 @@
         with self.fs.open(self.fpath, "r") as infile:
             data = json.load(infile)
         for idx, entry in enumerate(data):
             data[idx]["created_at"] = datetime.fromisoformat(entry["created_at"])
             data[idx]["last_updated"] = datetime.fromisoformat(entry["last_updated"])
 
         parent = self.fpath.parent
+        upstream_projects = {}
         for exp in data:
             dependencies = {}
             if "dependencies" in exp:
                 deplist = exp.pop("dependencies")
                 for dep in deplist:
-                    project = Project(
-                        fpath=parent / dep.split("|")[0],
-                        mode="r",
-                        **self.storage_options,
-                    )
-                    project.load()
-                    depexp = project[dep.split("|")[1]]
+                    project_name, exp_name = dep.split("|")
+                    project = upstream_projects.get(project_name)
+                    if not project:
+                        project = Project(
+                            fpath=parent / project_name,
+                            mode="r",
+                            **self.storage_options,
+                        )
+                        project.load()
+                        upstream_projects[project_name] = project
+                    depexp = project[exp_name]
                     dependencies[depexp.short_slug] = depexp
 
             tests = []
             if "tests" in exp:
                 testlist = exp.pop("tests")
                 for test in testlist:
                     if self.mode in ("r", "a"):
                         tests.append(ReadOnlyTest(**test))
                     else:
                         tests.append(Test(**test))
 
+            artifacts = []
+            if "artifacts" in exp:
+                artifactlist = exp.pop("artifacts")
+                for artifact in artifactlist:
+                    handler_cls = _get_handler(artifact.pop("handler"))
+                    created_at = datetime.fromisoformat(artifact.pop("created_at"))
+                    artifacts.append(
+                        handler_cls.construct(**artifact, created_at=created_at)
+                    )
+
             if self.mode in ("r", "a"):
                 self.experiments.append(
                     ReadOnlyExperiment(
                         **exp,
                         project=self.fpath,
+                        fs=self.fs,
                         dependencies=dependencies,
                         tests=tests,
+                        artifacts=artifacts,
                     )
                 )
             else:
                 self.experiments.append(
                     Experiment(
                         **exp,
                         project=self.fpath,
+                        fs=self.fs,
                         dependencies=dependencies,
                         tests=tests,
+                        artifacts=artifacts,
                     )
                 )
             self.snapshot[self.experiments[-1].slug] = self.experiments[-1].last_updated
 
     def save(self):
-        """Save the project data."""
+        """Save the project data.
+
+        This includes saving any artifact data.
+        """
         if self.mode == "r":
             raise RuntimeError("Project is in read-only mode.")
         elif self.mode == "w+":
             for slug, last_updated in self.snapshot.items():
                 if slug not in self:
                     continue
                 if self[slug].last_updated > last_updated:
                     self[slug].last_updated_by = self.author
 
         data = list(self)
-        with open(self.fpath, "w") as outfile:
+        with self.fs.open(self.fpath, "w") as outfile:
             json.dump(data, outfile, sort_keys=True, indent=4)
 
+        for exp in self.experiments:
+            if isinstance(exp, ReadOnlyExperiment):
+                LOG.debug(f"{exp.slug} was opened in read-only mode. Skipping...")
+                continue
+            if (
+                exp.slug in self.snapshot
+                and exp.last_updated == self.snapshot[exp.slug]
+            ):
+                LOG.debug(f"{exp.slug} has not been updated. Skipping...")
+                continue
+            # Write the artifact data
+            LOG.info(f"Saving artifacts for {exp.slug}")
+            for artifact in exp.artifacts:
+                fmode = "wb" if artifact.binary else "w"
+                fpath = exp.dir / exp.path / artifact.fname
+                if self.fs.isfile(
+                    fpath
+                ) and artifact.created_at <= datetime.fromtimestamp(
+                    self.fs.info(fpath)["created"]
+                ):
+                    LOG.debug(
+                        f"Artifact '{artifact.name}' already exists and has not been updated"
+                    )
+                    continue
+
+                self.fs.makedirs(exp.dir / exp.path, exist_ok=True)
+                LOG.debug(f"Saving '{artifact.name}' to {str(fpath)}...")
+                with self.fs.open(fpath, fmode) as buf:
+                    artifact.write(artifact.value, buf, **artifact.writer_kwargs)
+
     def merge(self, other: Project) -> Project:
         """Merge two projects.
 
         The new project will inherit the current project ``fpath``,
         ``author``, and ``mode``.
 
         Returns
@@ -218,15 +274,17 @@
         ------
         RuntimeError
             Raised when trying to log a new experiment when the project is in
             read-only mode.
         """
         if self.mode == "r":
             raise RuntimeError("Project is in read-only mode.")
-        experiment = Experiment(name=name, project=self.fpath, author=self.author)
+        experiment = Experiment(
+            name=name, project=self.fpath, fs=self.fs, author=self.author
+        )
 
         try:
             yield experiment
 
             self.append(experiment)
         except Exception as exc:
             raise exc
```

## Comparing `lazyscribe-0.3.2.dist-info/METADATA` & `lazyscribe-0.4.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyscribe
-Version: 0.3.2
+Version: 0.4.0
 Summary: Lightweight and lazy experiment logging
 Author-email: Akshay Gupta <akgcodes@gmail.com>
 License: MIT license
 Project-URL: documentation, https://lazyscribe.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lazyscribe/lazyscribe
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,18 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: attrs (<=22.2.0,>=21.2.0)
-Requires-Dist: python-slugify (<=7.0.0,>=5.0.0)
-Requires-Dist: fsspec (<=2023.1.0,>=0.4.0)
+Requires-Dist: attrs (<=23.1.0,>=21.2.0)
+Requires-Dist: importlib-metadata (<=6.6.0,>=6.0)
+Requires-Dist: python-slugify (<=8.0.1,>=5.0.0)
+Requires-Dist: fsspec (<=2023.5.0,>=0.4.0)
 Provides-Extra: build
 Requires-Dist: build ; extra == 'build'
 Requires-Dist: bumpver ; extra == 'build'
 Requires-Dist: twine ; extra == 'build'
 Requires-Dist: wheel ; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: lazyscribe[build] ; extra == 'dev'
@@ -31,30 +32,31 @@
 Requires-Dist: lazyscribe[qa] ; extra == 'dev'
 Requires-Dist: lazyscribe[tests] ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo ; extra == 'docs'
 Requires-Dist: matplotlib ; extra == 'docs'
 Requires-Dist: pandas ; extra == 'docs'
 Requires-Dist: pillow ; extra == 'docs'
-Requires-Dist: prefect (<=1.1.0,>=0.5.0) ; extra == 'docs'
+Requires-Dist: prefect (<2,>=1.0) ; extra == 'docs'
 Requires-Dist: scikit-learn ; extra == 'docs'
 Requires-Dist: sphinx ; extra == 'docs'
 Requires-Dist: sphinx-gallery ; extra == 'docs'
 Requires-Dist: sphinx-inline-tabs ; extra == 'docs'
 Provides-Extra: qa
 Requires-Dist: black ; extra == 'qa'
 Requires-Dist: edgetest ; extra == 'qa'
 Requires-Dist: flake8 ; extra == 'qa'
 Requires-Dist: isort ; extra == 'qa'
 Requires-Dist: mypy ; extra == 'qa'
 Requires-Dist: pip-tools ; extra == 'qa'
 Requires-Dist: pydocstyle ; extra == 'qa'
 Requires-Dist: types-python-slugify ; extra == 'qa'
 Provides-Extra: tests
-Requires-Dist: prefect (<=1.1.0,>=0.5.0) ; extra == 'tests'
+Requires-Dist: scikit-learn ; extra == 'tests'
+Requires-Dist: prefect (<2,>=1.0) ; extra == 'tests'
 Requires-Dist: pytest ; extra == 'tests'
 Requires-Dist: pytest-cov ; extra == 'tests'
 
 [![codecov](https://codecov.io/github/lazyscribe/lazyscribe/branch/main/graph/badge.svg?token=M5BHYS2SSU)](https://codecov.io/github/lazyscribe/lazyscribe) ![PyPI](https://img.shields.io/pypi/v/lazyscribe) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lazyscribe) [![Documentation Status](https://readthedocs.org/projects/lazyscribe/badge/?version=latest)](https://lazyscribe.readthedocs.io/en/latest/?badge=latest)
 
 # Lightweight, lazy experiment logging
 
@@ -74,43 +76,49 @@
 
 # Basic Usage
 
 The basic usage involves instantiating a ``Project`` and using the context manager to log
 an experiment:
 
 ```python
+import json
+
 from lazyscribe import Project
 
 project = Project(fpath="project.json")
 with project.log(name="My experiment") as exp:
     exp.log_metric("auroc", 0.5)
     exp.log_parameter("algorithm", "lightgbm")
 ```
 
 You've created an experiment! You can view the experimental data by using ``list``:
 
 ```python
-from pprint import pprint
-
-pprint(list(project))
+print(json.dumps(list(project), indent=4))
 ```
 
 ```json
 [
     {
         "name": "My experiment",
         "author": "<AUTHOR>",
         "last_updated_by": "<AUTHOR>",
-        "metrics": {"auroc": 0.5},
-        "parameters": {"algorithm": "lightgbm"},
+        "metrics": {
+            "auroc": 0.5
+        },
+        "parameters": {
+            "algorithm": "lightgbm"
+        },
         "created_at": "<CREATED_AT>",
         "last_updated": "<LAST_UPDATED>",
         "dependencies": [],
         "short_slug": "my-experiment",
-        "slug": "my-experiment-<CREATED_AT>"
+        "slug": "my-experiment-<CREATED_AT>",
+        "tests": [],
+        "artifacts": []
     }
 ]
 ```
 
 Once you've finished, save the project to ``project.json``:
 
 ```python
```

