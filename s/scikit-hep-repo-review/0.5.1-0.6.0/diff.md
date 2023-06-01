# Comparing `tmp/scikit_hep_repo_review-0.5.1.tar.gz` & `tmp/scikit_hep_repo_review-0.6.0.tar.gz`

## Comparing `scikit_hep_repo_review-0.5.1.tar` & `scikit_hep_repo_review-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,38 @@
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/noxfile.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/docs/.nojekyll
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/docs/index.html
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/docs/webapp.js
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/__init__.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/__main__.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ghpath.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/py.typed
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/__init__.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/general.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/github.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/mypy.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/precommit.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/pyproject.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/ruff.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/tests/test_package.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/LICENSE
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/README.md
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/noxfile.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/docs/.nojekyll
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/docs/index.html
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/docs/webapp.js
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/__init__.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/__main__.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/families.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/fixtures.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/ghpath.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/general.py
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/github.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_checks.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_cmd.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_fixtures.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_package.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/README.md
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/PKG-INFO
```

### Comparing `scikit_hep_repo_review-0.5.1/.pre-commit-config.yaml` & `scikit_hep_repo_review-0.6.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# Needed because we don't support anything before 3.10
-default_language_version:
-  python: python3.10
-
 ci:
   autoupdate_commit_msg: "chore(deps): update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/psf/black
     rev: 23.3.0
@@ -15,15 +11,15 @@
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.1.0]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.267"
+    rev: "v0.0.270"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
@@ -53,22 +49,23 @@
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
       - id: mypy
-        files: src
+        files: (src|web|tests)
         args: []
         additional_dependencies:
           - click
+          - markdown-it-py
+          - pytest
           - rich
+          - tomli
           - types-PyYAML
-          - tomli;python_version<"3.11"
-          - markdown-it-py
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
         args: ["-Lhist,absense"]
```

### Comparing `scikit_hep_repo_review-0.5.1/noxfile.py` & `scikit_hep_repo_review-0.6.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 @nox.session
 def pylint(session: nox.Session) -> None:
     """
     Run PyLint.
     """
     # This needs to be installed into the package environment, and is slower
     # than a pre-commit check
-    session.install(".[cli]", "pylint")
+    session.install("-e.[cli]", "pylint")
     session.run("pylint", "src", *session.posargs)
 
 
 @nox.session
 def tests(session: nox.Session) -> None:
     """
     Run the unit and regular tests.
     """
-    session.install(".[test]")
+    session.install("-e.[test,cli]")
     session.run("pytest", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
```

### Comparing `scikit_hep_repo_review-0.5.1/.github/CONTRIBUTING.md` & `scikit_hep_repo_review-0.6.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.1/.github/matchers/pylint.json` & `scikit_hep_repo_review-0.6.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.1/.github/workflows/ci.yml` & `scikit_hep_repo_review-0.6.0/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     branches:
       - main
   release:
     types:
       - published
 
 concurrency:
-  group: ci-${{ github.head_ref }}
+  group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   pre-commit:
     name: Format
     runs-on: ubuntu-latest
     steps:
@@ -34,29 +34,31 @@
   checks:
     name: Check Python ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     needs: [pre-commit]
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12-dev"]
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install package
-        run: python -m pip install .[test]
+        run: python -m pip install .[test,cli]
 
       - name: Test package
         run: python -m pytest -ra
+        env:
+          PYTHONUTF8: "1"
 
   dist:
     name: Distribution build
     runs-on: ubuntu-latest
     needs: [pre-commit]
 
     steps:
```

### Comparing `scikit_hep_repo_review-0.5.1/docs/index.html` & `scikit_hep_repo_review-0.6.0/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <head>
     <meta
       charset="utf-8"
       name="viewport"
       content="initial-scale=1, width=device-width"
     />
     <script
-      src="https://cdn.jsdelivr.net/pyodide/v0.23.1/full/pyodide.js"
+      src="https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js"
       crossorigin
     ></script>
     <!-- Production -->
     <script
       src="https://unpkg.com/react@18/umd/react.production.min.js"
       crossorigin
     ></script>
```

### Comparing `scikit_hep_repo_review-0.5.1/docs/webapp.js` & `scikit_hep_repo_review-0.6.0/docs/webapp.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -163,15 +163,15 @@
 
 async function prepare_pyodide() {
     const pyodide = await loadPyodide();
 
     await pyodide.loadPackage("micropip");
     await pyodide.runPythonAsync(`
         import micropip
-        await micropip.install(["scikit_hep_repo_review==0.5.0"])
+        await micropip.install(["scikit_hep_repo_review==0.5.1"])
     `);
     return pyodide;
 }
 
 const pyodide_promise = prepare_pyodide();
 
 function MyThemeProvider(props) {
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ghpath.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/ghpath.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,29 @@
+# pylint: disable=arguments-differ
+
 from __future__ import annotations
 
 import dataclasses
 import io
 import json
+import typing
 from collections.abc import Iterator
-from typing import Literal, overload
+from typing import Literal
+
+from ._compat.importlib.resources.abc import Traversable
+
+__all__ = ["GHPath"]
+
+
+def __dir__() -> list[str]:
+    return __all__
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
-class GHPath:
+class GHPath(Traversable):
     repo: str
     branch: str
     path: str = ""
     _info: list[dict[str, str]] = dataclasses.field(
         hash=False, default_factory=list, repr=False
     )
 
@@ -32,43 +43,50 @@
             try:
                 object.__setattr__(self, "_info", vals["tree"])
             except KeyError:
                 print("Failed to find tree. Result:")  # noqa: T201
                 print(vals)  # noqa: T201
                 raise
 
+    def __str__(self) -> str:
+        return f"gh:{self.repo}@{self.branch}:{self.path or '.'}"
+
     @property
     def name(self) -> str:
         return (self.path or self.repo).split("/")[-1]
 
-    @overload
-    def open(self, mode: Literal["r"]) -> io.StringIO:
+    @typing.overload  # type: ignore[override]
+    def open(self, mode: Literal["r"], encoding: str | None = ...) -> io.StringIO:
         ...
 
-    @overload
+    @typing.overload
     def open(self, mode: Literal["rb"]) -> io.BytesIO:
         ...
 
-    def open(self, mode: Literal["r", "rb"] = "r") -> io.IOBase:
+    def open(
+        self, mode: Literal["r", "rb"] = "r", encoding: str | None = "utf-8"
+    ) -> io.IOBase:
+        assert encoding is None or encoding == "utf-8", "Only utf-8 is supported"
         val: io.StringIO = self.open_url(
             f"https://raw.githubusercontent.com/{self.repo}/{self.branch}/{self.path}"
         )
         if "b" in mode:
             return io.BytesIO(val.read().encode("utf-8"))
         return val
 
     def _with_path(self, path: str) -> GHPath:
         return GHPath(
             repo=self.repo, branch=self.branch, path=path.lstrip("/"), _info=self._info
         )
 
-    def joinpath(self, path: str) -> GHPath:
-        return self._with_path(f"{self.path}/{path}")
+    def joinpath(self, child: str) -> GHPath:
+        return self._with_path(f"{self.path}/{child}")
 
-    __truediv__ = joinpath
+    def __truediv__(self, child: str) -> GHPath:
+        return self._with_path(f"{self.path}/{child}")
 
     def iterdir(self) -> Iterator[GHPath]:
         if self.path:
             yield from (
                 self._with_path(d["path"])
                 for d in self._info
                 if d["path"].startswith(self.path)
@@ -80,12 +98,12 @@
 
     def is_dir(self) -> bool:
         return self.path in {d["path"] for d in self._info if d["type"] == "tree"}
 
     def is_file(self) -> bool:
         return self.path in {d["path"] for d in self._info if d["type"] == "blob"}
 
-    def read_text(self) -> str:
-        return self.open("r").read()
+    def read_text(self, encoding: str | None = "utf-8") -> str:
+        return self.open("r", encoding=encoding).read()
 
     def read_bytes(self) -> bytes:
         return self.open("rb").read()
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/processor.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,128 @@
 from __future__ import annotations
 
 import dataclasses
-import importlib.metadata
-import inspect
+import graphlib
 import textwrap
-from collections.abc import Callable, Iterable
-from graphlib import TopologicalSorter
-from importlib.abc import Traversable
-from typing import Any
+import typing
+from collections.abc import Sequence
 
-from markdown_it import MarkdownIt
+import markdown_it
 
-from .ratings import Rating
+from ._compat.importlib.resources.abc import Traversable
+from .checks import Check, collect_checks, is_allowed
+from .families import Family, collect_families
+from .fixtures import apply_fixtures, collect_fixtures, compute_fixtures, pyproject
 
-# Use module-level entry names
-# repo_review_fixtures = {"pyproject"}
-# repo_review_checks = set(p.__name___ for p in General.__subclasses__())
+__all__ = ["Result", "ResultDict", "ProcessReturn", "process", "as_simple_dict"]
 
-md = MarkdownIt()
+
+def __dir__() -> list[str]:
+    return __all__
+
+
+md = markdown_it.MarkdownIt()
+
+
+# Helper to get the type in the JSON style returns
+class ResultDict(typing.TypedDict):
+    family: str
+    description: str
+    result: bool | None
+    err_msg: str
 
 
 @dataclasses.dataclass(frozen=True, kw_only=True)
 class Result:
+    family: str
     name: str
     description: str
     result: bool | None
     err_msg: str = ""
 
     def err_markdown(self) -> str:
         result: str = md.render(self.err_msg)
         return result
 
 
-def build(
-    check: type[Rating],
-    package: Traversable,
-    fixtures: Iterable[Callable[[Traversable], Any]],
-) -> bool | None:
-    kwargs: dict[str, Any] = {}
-    signature = inspect.signature(check.check)  # type: ignore[attr-defined]
-    if "package" in signature.parameters:
-        kwargs["package"] = package
-
-    for func in fixtures:
-        if func.__name__ in signature.parameters:
-            kwargs[func.__name__] = func(package)
-
-    return check.check(**kwargs)  # type: ignore[attr-defined, no-any-return]
-
-
-def process(package: Traversable) -> dict[str, list[Result]]:
-    modules: list[str] = [
-        ep.load()
-        for ep in importlib.metadata.entry_points(
-            group="scikit_hep_repo_review.ratings"
-        )
-    ]
-
-    ratings = [
-        getattr(mod, rat)
-        for mod in modules
-        for rat in getattr(mod, "repo_review_checks", ())
-    ]
-
-    fixtures = [
-        getattr(mod, fixt)
-        for mod in modules
-        for fixt in getattr(mod, "repo_review_fixtures", ())
-    ]
+class ProcessReturn(typing.NamedTuple):
+    families: dict[str, Family]
+    results: list[Result]
+
+
+def process(package: Traversable, *, ignore: Sequence[str] = ()) -> ProcessReturn:
+    """
+    Process the package and return a dictionary of results.
+
+    Parameters
+    ----------
+    package: Traversable | Path
+        The Path(like) package to process
+
+    ignore: Sequence[str]
+        A list of checks to ignore
+    """
+    # Collect the fixtures
+    fixture_functions = collect_fixtures()
+    fixtures = compute_fixtures(package, fixture_functions)
+
+    # Collect the checks
+    checks = collect_checks(fixtures)
+
+    # Collect families.
+    families = collect_families()
+
+    # These are optional, so fill in missing families.
+    for name in {c.family for c in checks.values()}:
+        if name not in families:
+            families[name] = Family()
+
+    # Collect our own config
+    config = pyproject(package).get("tool", {}).get("repo-review", {})
+    skip_checks = set(ignore) | set(config.get("ignore", ()))
 
-    tasks = {t.__name__: t for t in ratings}
+    tasks: dict[str, Check] = {
+        n: r for n, r in checks.items() if is_allowed(skip_checks, n)
+    }
     graph: dict[str, set[str]] = {
         n: getattr(t, "requires", set()) for n, t in tasks.items()
     }
     completed: dict[str, bool | None] = {}
 
-    # A few families are here to make sure they print first
-    families: dict[str, set[str]] = {"general": set(), "pyproject": set()}
-    for name, task in tasks.items():
-        families.setdefault(task.family, set()).add(name)
-
-    ts = TopologicalSorter(graph)
+    # Run all the checks in topological order
+    ts = graphlib.TopologicalSorter(graph)
     for name in ts.static_order():
         if all(completed.get(n, False) for n in graph[name]):
-            completed[name] = build(tasks[name], package, fixtures)
+            completed[name] = apply_fixtures(fixtures, tasks[name].check)
         else:
             completed[name] = None
 
-    results_dict = {}
-    for family, ftasks in families.items():
-        result_list = []
-        for task_name in sorted(ftasks):
-            check = tasks[task_name]
-            result = completed[task_name]
-
-            result_list.append(
-                Result(
-                    name=task_name,
-                    description=check.__doc__,
-                    result=result,
-                    err_msg=textwrap.dedent(check.check.__doc__.format(cls=check)),
-                )
+    # Collect the results
+    result_list = []
+    for task_name, check in sorted(
+        tasks.items(),
+        key=lambda x: (families[x[1].family].get("order", 0), x[1].family, x[0]),
+    ):
+        result = completed[task_name]
+        doc = check.__doc__ or ""
+
+        result_list.append(
+            Result(
+                family=check.family,
+                name=task_name,
+                description=doc,
+                result=result,
+                err_msg=textwrap.dedent(doc.format(cls=check)),
             )
-        results_dict[family] = result_list
+        )
 
-    return results_dict
+    return ProcessReturn(families, result_list)
+
+
+def as_simple_dict(results: list[Result]) -> dict[str, ResultDict]:
+    return {
+        result.name: typing.cast(
+            ResultDict,
+            {k: v for k, v in dataclasses.asdict(result).items() if k != "name"},
+        )
+        for result in results
+    }
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/general.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from importlib.abc import Traversable
+from .._compat.importlib.resources.abc import Traversable
 
 # PY: Python Project
 ## 0xx: File existence
 
 
 class General:
     family = "general"
@@ -80,9 +80,9 @@
         """
         return (
             package.joinpath("noxfile.py").is_file()
             or package.joinpath("tox.ini").is_file()
         )
 
 
-repo_review_fixtures = set[str]()
-repo_review_checks = {p.__name__ for p in General.__subclasses__()}
+def repo_review_checks() -> dict[str, General]:
+    return {p.__name__: p() for p in General.__subclasses__()}
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/github.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # GH: GitHub Actions
 ## GH1xx: Normal actions
 
 from __future__ import annotations
 
-import functools
-from importlib.abc import Traversable
 from pathlib import Path
 from typing import Any
 
 import yaml
 
+from .._compat.importlib.resources.abc import Traversable
+
 
-@functools.cache
 def workflows(package: Traversable) -> dict[str, Any]:
     workflows_base_path = package.joinpath(".github/workflows")
     workflows_dict: dict[str, Any] = {}
     if workflows_base_path.is_dir():
         for workflow_path in workflows_base_path.iterdir():
             if workflow_path.name.endswith(".yml"):
                 with workflow_path.open("rb") as f:
                     workflows_dict[Path(workflow_path.name).stem] = yaml.safe_load(f)
 
     return workflows_dict
 
 
-@functools.cache
 def dependabot(package: Traversable) -> dict[str, Any]:
     dependabot_path = package.joinpath(".github/dependabot.yml")
     if dependabot_path.is_file():
         with dependabot_path.open("rb") as f:
             result: dict[str, Any] = yaml.safe_load(f)
             return result
 
@@ -163,9 +161,9 @@
             if ecosystem.get("package-ecosystem", "") == "github-actions":
                 for ignore in ecosystem.get("ignore", []):
                     if "actions/*" in ignore.get("dependency-name", ""):
                         return False
         return True
 
 
-repo_review_fixtures = {"workflows", "dependabot"}
-repo_review_checks = {p.__name__ for p in GitHub.__subclasses__()}
+def repo_review_checks() -> dict[str, GitHub]:
+    return {p.__name__: p() for p in GitHub.__subclasses__()}
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/mypy.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,9 +142,9 @@
         match pyproject:
             case {"tool": {"mypy": {"enable_error_code": list(codes)}}}:
                 return "truthy-bool" in codes
             case _:
                 return False
 
 
-repo_review_fixtures = set[str]()
-repo_review_checks = {p.__name__ for p in MyPy.__subclasses__()}
+def repo_review_checks() -> dict[str, MyPy]:
+    return {p.__name__: p() for p in MyPy.__subclasses__()}
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/precommit.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/precommit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # PC: Pre-commit
 ## PC0xx: pre-commit-hooks
 
 from __future__ import annotations
 
-import functools
-from importlib.abc import Traversable
 from typing import Any, ClassVar, Protocol
 
 import yaml
 
+from .._compat.importlib.resources.abc import Traversable
+
 
-@functools.cache
 def precommit(package: Traversable) -> dict[str, Any]:
     precommit_path = package.joinpath(".pre-commit-config.yaml")
     if precommit_path.is_file():
         with precommit_path.open("rb") as f:
             return yaml.safe_load(f)  # type: ignore[no-any-return]
 
     return {}
@@ -121,9 +120,9 @@
           autoupdate_commit_msg: 'chore: update pre-commit hooks'
         ```
         """
 
         return "autoupdate_commit_msg" in precommit.get("ci", {})
 
 
-repo_review_fixtures = {"precommit"}
-repo_review_checks = {p.__name__ for p in PreCommit.__subclasses__()}
+def repo_review_checks() -> dict[str, PreCommit]:
+    return {p.__name__: p() for p in PreCommit.__subclasses__()}
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/pyproject.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/pyproject.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,11 @@
 from __future__ import annotations
 
-import functools
-import sys
-from importlib.abc import Traversable
 from typing import Any
 
-if sys.version_info < (3, 11):
-    import tomli as tomllib
-else:
-    import tomllib
-
-
-@functools.cache
-def pyproject(package: Traversable) -> dict[str, Any]:
-    pyproject_path = package.joinpath("pyproject.toml")
-    if pyproject_path.is_file():
-        with pyproject_path.open("rb") as f:
-            return tomllib.load(f)
-    return {}
-
-
 # PP: PyProject.toml
 ## PP0xx: Build system
 
 
 class PyProject:
     family = "pyproject"
 
@@ -188,9 +170,9 @@
         `filterwarnings` must be set (probably to at least `['error']`). Python
         will hide important warnings otherwise, like deprecations.
         """
         options = pyproject["tool"]["pytest"]["ini_options"]
         return "filterwarnings" in options
 
 
-repo_review_fixtures = {"pyproject"}
-repo_review_checks = {p.__name__ for p in PyProject.__subclasses__()}
+def repo_review_checks() -> dict[str, PyProject]:
+    return {p.__name__: p() for p in PyProject.__subclasses__()}
```

### Comparing `scikit_hep_repo_review-0.5.1/src/scikit_hep_repo_review/ratings/ruff.py` & `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/ruff.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-from importlib.abc import Traversable
 from typing import Any, ClassVar, Protocol
 
+from .._compat.importlib.resources.abc import Traversable
+
 ## R0xx: Ruff general
 ## R1xx: Ruff checks
 
 
 class Ruff:
     family = "ruff"
     requires = {"PY001"}
@@ -111,12 +112,12 @@
 
 class R103(R1xx):
     "pyupgrade must be selected"
     code = "UP"
     name = "pyupgrade"
 
 
-base_classes = {p.__name__ for p in Ruff.__subclasses__()} - {"R1xx"}
-r1xx_classes = {p.__name__ for p in R1xx.__subclasses__()}
-
-repo_review_fixtures = set[str]()
-repo_review_checks = base_classes | r1xx_classes
+def repo_review_checks() -> dict[str, Ruff]:
+    base_classes = set(Ruff.__subclasses__()) - {R1xx}
+    r1xx_classes = set(R1xx.__subclasses__())
+    repo_review_checks = base_classes | r1xx_classes
+    return {p.__name__: p() for p in repo_review_checks}
```

### Comparing `scikit_hep_repo_review-0.5.1/.gitignore` & `scikit_hep_repo_review-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.1/LICENSE` & `scikit_hep_repo_review-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.5.1/README.md` & `scikit_hep_repo_review-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,45 +35,47 @@
 You are not required to be in Scikit-HEP to find this useful, however -
 examples of repositories that at least partially follow the guidelines include
 `pypa/cibuildwheel`, `pypa/build`, and `pybind/pybind11`.
 
 ### Development
 
 This repository is intended to be fun to develop - it requires and uses Python
-3.10, and makes a few potentially... uncommon decisions. You might not want to
-design your library this way, but this is not a library. It's a fun and
-enjoyable app.
+3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
+entirely conventional, but it's fun.
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
 Checks can request fixtures (like pytest) as arguments. Check files can add new
-fixtures as needed. The end of every check file has a list of checks (usually
-pulled from subclasses of a common ancestor) and a list of fixtures it
-provides.
+fixtures as needed. Fixtures are are specified with entry points, and take any
+other fixture as arguments as well - the `package` fixture represents the root
+of the package you are checking, and is the basis for all other fixtures.
+Checks are specified via an entrypoint that returns a dict of checks; this also
+can accept fixtures, allowing dynamic check listings.
 
 Check files do not depend on the main library, and can be extended (similar to
 Flake8). You register new check files via entry-points - so extending this is
 with custom checks or custom fixtures is easy and trivial. There's no need to
 subclass or do anything with the base library - no dependency required.
 
 Checks are as simple as possible so they are easy to write. A check is a class
 with the name (1-2 letters + number) and a docstring (the check message). It
 should define a set of `requires` with any checks it depends on (by name), and
 have a check classmethod. The docstring of this method is the failure message,
 and supports substitution. Arguments to this method are fixtures, and `package`
 is the built-in one providing the package directory as a Traversable. Any other
 fixtures are available by name. A new fixture is given the package Traversable,
-and can produce anything (recommended to be cached via `functools.cache`).
+and can produce anything; fixtures are topologically sorted, pre-computed and
+cached.
 
 The runner will topologically sort the checks, and checks that do not run will
-get a `None` result and the check classmethod will not run. The front-end (Rich
+get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
 # Links
 
 This project inspired [Try-PyHF](https://kratsg.github.io/try-pyhf/), an
 interface for a High Energy Physics package in Scikit-HEP.
```

### Comparing `scikit_hep_repo_review-0.5.1/PKG-INFO` & `scikit_hep_repo_review-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_hep_repo_review
-Version: 0.5.1
+Version: 0.6.0
 Summary: Review repos for compliance to the Scikit-HEP developer guidelines
 Project-URL: homepage, https://github.com/Scikit-HEP/repo-review
 Project-URL: webpage, https://scikit-hep.github.io/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -41,14 +41,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Requires-Dist: markdown-it-py
 Requires-Dist: pyyaml
 Requires-Dist: tomli; python_version < '3.11'
 Provides-Extra: cli
 Requires-Dist: click>=8; extra == 'cli'
@@ -96,45 +97,47 @@
 You are not required to be in Scikit-HEP to find this useful, however -
 examples of repositories that at least partially follow the guidelines include
 `pypa/cibuildwheel`, `pypa/build`, and `pybind/pybind11`.
 
 ### Development
 
 This repository is intended to be fun to develop - it requires and uses Python
-3.10, and makes a few potentially... uncommon decisions. You might not want to
-design your library this way, but this is not a library. It's a fun and
-enjoyable app.
+3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
+entirely conventional, but it's fun.
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
 
 Checks can request fixtures (like pytest) as arguments. Check files can add new
-fixtures as needed. The end of every check file has a list of checks (usually
-pulled from subclasses of a common ancestor) and a list of fixtures it
-provides.
+fixtures as needed. Fixtures are are specified with entry points, and take any
+other fixture as arguments as well - the `package` fixture represents the root
+of the package you are checking, and is the basis for all other fixtures.
+Checks are specified via an entrypoint that returns a dict of checks; this also
+can accept fixtures, allowing dynamic check listings.
 
 Check files do not depend on the main library, and can be extended (similar to
 Flake8). You register new check files via entry-points - so extending this is
 with custom checks or custom fixtures is easy and trivial. There's no need to
 subclass or do anything with the base library - no dependency required.
 
 Checks are as simple as possible so they are easy to write. A check is a class
 with the name (1-2 letters + number) and a docstring (the check message). It
 should define a set of `requires` with any checks it depends on (by name), and
 have a check classmethod. The docstring of this method is the failure message,
 and supports substitution. Arguments to this method are fixtures, and `package`
 is the built-in one providing the package directory as a Traversable. Any other
 fixtures are available by name. A new fixture is given the package Traversable,
-and can produce anything (recommended to be cached via `functools.cache`).
+and can produce anything; fixtures are topologically sorted, pre-computed and
+cached.
 
 The runner will topologically sort the checks, and checks that do not run will
-get a `None` result and the check classmethod will not run. The front-end (Rich
+get a `None` result and the check method will not run. The front-end (Rich
 powered CLI or Pyodide webapp) will render the markdown-formatted check
 docstring only if the result is `False`.
 
 # Links
 
 This project inspired [Try-PyHF](https://kratsg.github.io/try-pyhf/), an
 interface for a High Energy Physics package in Scikit-HEP.
```

