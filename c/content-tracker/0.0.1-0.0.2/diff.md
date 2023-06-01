# Comparing `tmp/content_tracker-0.0.1.tar.gz` & `tmp/content_tracker-0.0.2.tar.gz`

## Comparing `content_tracker-0.0.1.tar` & `content_tracker-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 content_tracker-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 content_tracker-0.0.1/Makefile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 content_tracker-0.0.1/requirements.txt
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 content_tracker-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 content_tracker-0.0.1/.github/release.yml
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 content_tracker-0.0.1/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 content_tracker-0.0.1/src/content_tracker/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 content_tracker-0.0.1/src/content_tracker/_version.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 content_tracker-0.0.1/tests/test_version.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 content_tracker-0.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 content_tracker-0.0.1/LICENSE
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 content_tracker-0.0.1/README.md
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 content_tracker-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 content_tracker-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 content_tracker-0.0.2/Makefile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 content_tracker-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.github/release.yml
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 content_tracker-0.0.2/src/content_tracker/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 content_tracker-0.0.2/src/content_tracker/_version.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 content_tracker-0.0.2/tests/test_version.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 content_tracker-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 content_tracker-0.0.2/LICENSE
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 content_tracker-0.0.2/README.md
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 content_tracker-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 content_tracker-0.0.2/PKG-INFO
```

### Comparing `content_tracker-0.0.1/.github/workflows/python-tests.yml` & `content_tracker-0.0.2/.github/workflows/python-tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Python Tests
 
 on:
-  push:
-    tags: ["v[0-9]+.[0-9]+.[0-9]+**"]
   pull_request:
+  release:
+    types: [published]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.x"
+          python-version: "3.11"
           cache: pip
 
       - name: Install dependencies
         run: python3 -m pip install build
 
       - name: Build
         run: make dist
@@ -57,37 +57,20 @@
         run: make test
 
       - name: Upload coverage reports
         uses: codecov/codecov-action@v3
 
   publish:
     needs: test
-    if: github.ref_type == 'tag'
+    if: github.event_name == 'release' && github.event.action == 'published'
     runs-on: ubuntu-latest
     steps:
       - name: Download artifact
         uses: actions/download-artifact@v3
         with:
           name: packages
           path: ./dist
 
       - name: Publish
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_TOKEN }}
-
-  release:
-    needs: publish
-    if: github.ref_type == 'tag'
-    runs-on: ubuntu-latest
-    steps:
-      - name: Release
-        uses: actions/github-script@v6
-        with:
-          script: |
-            github.rest.repos.createRelease({
-              owner: context.repo.owner,
-              repo: context.repo.repo,
-              tag_name: "${{ github.ref_name }}",
-              name: "${{ github.ref_name }}",
-              generate_release_notes: true
-            })
```

### Comparing `content_tracker-0.0.1/.gitignore` & `content_tracker-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `content_tracker-0.0.1/LICENSE` & `content_tracker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `content_tracker-0.0.1/README.md` & `content_tracker-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `content_tracker-0.0.1/pyproject.toml` & `content_tracker-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `content_tracker-0.0.1/PKG-INFO` & `content_tracker-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: content-tracker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tracking changes in arbitrary content.
 Project-URL: Homepage, https://github.com/speg03/content-tracker
 Project-URL: Repository, https://github.com/speg03/content-tracker
 Author-email: Takahiro Yano <speg03@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: changes,content,diff,tracking
```

