# Comparing `tmp/scikit_hep_repo_review-0.6.0.tar.gz` & `tmp/scikit_hep_repo_review-0.6.1.tar.gz`

## Comparing `scikit_hep_repo_review-0.6.0.tar` & `scikit_hep_repo_review-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/noxfile.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/docs/.nojekyll
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/docs/index.html
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/docs/webapp.js
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/__init__.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/__main__.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/families.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/fixtures.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/ghpath.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/processor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/__init__.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/general.py
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/github.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/mypy.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/precommit.py
--rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/pyproject.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/ruff.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_checks.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_cmd.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_fixtures.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/tests/test_package.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/LICENSE
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/README.md
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/noxfile.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/docs/.nojekyll
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/docs/index.html
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/docs/webapp.js
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/__init__.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/__main__.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/families.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/fixtures.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/ghpath.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/processor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/__init__.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/general.py
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/github.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/mypy.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/precommit.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/pyproject.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/ruff.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/tests/test_checks.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/tests/test_cmd.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/tests/test_fixtures.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/tests/test_package.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/README.md
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 scikit_hep_repo_review-0.6.1/PKG-INFO
```

### Comparing `scikit_hep_repo_review-0.6.0/.pre-commit-config.yaml` & `scikit_hep_repo_review-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/noxfile.py` & `scikit_hep_repo_review-0.6.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/.github/CONTRIBUTING.md` & `scikit_hep_repo_review-0.6.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/.github/matchers/pylint.json` & `scikit_hep_repo_review-0.6.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/.github/workflows/ci.yml` & `scikit_hep_repo_review-0.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/docs/index.html` & `scikit_hep_repo_review-0.6.1/docs/index.html`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/docs/webapp.js` & `scikit_hep_repo_review-0.6.1/docs/webapp.js`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/__main__.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/__main__.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/families.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/families.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/fixtures.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/ghpath.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/processor.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     family: str
     name: str
     description: str
     result: bool | None
     err_msg: str = ""
 
     def err_markdown(self) -> str:
-        result: str = md.render(self.err_msg)
-        return result
+        result: str = md.render(self.err_msg).strip()
+        return result.removeprefix("<p>").removesuffix("</p>").strip()
 
 
 class ProcessReturn(typing.NamedTuple):
     families: dict[str, Family]
     results: list[Result]
 
 
@@ -100,22 +100,23 @@
     result_list = []
     for task_name, check in sorted(
         tasks.items(),
         key=lambda x: (families[x[1].family].get("order", 0), x[1].family, x[0]),
     ):
         result = completed[task_name]
         doc = check.__doc__ or ""
+        err_msg = check.check.__doc__ or ""
 
         result_list.append(
             Result(
                 family=check.family,
                 name=task_name,
                 description=doc,
                 result=result,
-                err_msg=textwrap.dedent(doc.format(cls=check)),
+                err_msg=textwrap.dedent(err_msg.format(cls=check)),
             )
         )
 
     return ProcessReturn(families, result_list)
 
 
 def as_simple_dict(results: list[Result]) -> dict[str, ResultDict]:
```

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/__init__.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/general.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/general.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/github.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/github.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/mypy.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/mypy.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/precommit.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/precommit.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/pyproject.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/pyproject.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/src/scikit_hep_repo_review/checks/ruff.py` & `scikit_hep_repo_review-0.6.1/src/scikit_hep_repo_review/checks/ruff.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/tests/test_checks.py` & `scikit_hep_repo_review-0.6.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/tests/test_fixtures.py` & `scikit_hep_repo_review-0.6.1/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/tests/test_package.py` & `scikit_hep_repo_review-0.6.1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/.gitignore` & `scikit_hep_repo_review-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/LICENSE` & `scikit_hep_repo_review-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/README.md` & `scikit_hep_repo_review-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/pyproject.toml` & `scikit_hep_repo_review-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_hep_repo_review-0.6.0/PKG-INFO` & `scikit_hep_repo_review-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_hep_repo_review
-Version: 0.6.0
+Version: 0.6.1
 Summary: Review repos for compliance to the Scikit-HEP developer guidelines
 Project-URL: homepage, https://github.com/Scikit-HEP/repo-review
 Project-URL: webpage, https://scikit-hep.github.io/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 Maintainer-email: The Scikit-HEP admins <scikit-hep-admins@googlegroups.com>
 License: BSD 3-Clause License
```

