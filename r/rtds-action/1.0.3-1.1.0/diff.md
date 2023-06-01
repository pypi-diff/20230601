# Comparing `tmp/rtds_action-1.0.3.tar.gz` & `tmp/rtds_action-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtds_action-1.0.3.tar", last modified: Sun Apr 11 13:15:29 2021, max compression
+gzip compressed data, was "rtds_action-1.1.0.tar", last modified: Thu Jun  1 11:43:14 2023, max compression
```

## Comparing `rtds_action-1.0.3.tar` & `rtds_action-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 13:15:29.455968 rtds_action-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-11 13:15:18.000000 rtds_action-1.0.3/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-04-11 13:15:18.000000 rtds_action-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-04-11 13:15:18.000000 rtds_action-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8310 2021-04-11 13:15:29.455968 rtds_action-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6371 2021-04-11 13:15:18.000000 rtds_action-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 13:15:29.455968 rtds_action-1.0.3/compiled/
--rw-r--r--   0 runner    (1001) docker     (121)    57526 2021-04-11 13:15:18.000000 rtds_action-1.0.3/compiled/index.js
--rw-r--r--   0 runner    (1001) docker     (121)      463 2021-04-11 13:15:18.000000 rtds_action-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-11 13:15:29.455968 rtds_action-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2021-04-11 13:15:18.000000 rtds_action-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 13:15:29.455968 rtds_action-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 13:15:29.455968 rtds_action-1.0.3/src/rtds_action/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-04-11 13:15:18.000000 rtds_action-1.0.3/src/rtds_action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2021-04-11 13:15:18.000000 rtds_action-1.0.3/src/rtds_action/rtds_action.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-04-11 13:15:29.000000 rtds_action-1.0.3/src/rtds_action/rtds_action_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-11 13:15:29.455968 rtds_action-1.0.3/src/rtds_action.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8310 2021-04-11 13:15:29.000000 rtds_action-1.0.3/src/rtds_action.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-04-11 13:15:29.000000 rtds_action-1.0.3/src/rtds_action.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-11 13:15:29.000000 rtds_action-1.0.3/src/rtds_action.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-11 13:15:28.000000 rtds_action-1.0.3/src/rtds_action.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      140 2021-04-11 13:15:29.000000 rtds_action-1.0.3/src/rtds_action.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-11 13:15:29.000000 rtds_action-1.0.3/src/rtds_action.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:43:14.780199 rtds_action-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 11:42:59.000000 rtds_action-1.1.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 11:42:59.000000 rtds_action-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 11:42:59.000000 rtds_action-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-01 11:43:14.780199 rtds_action-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-06-01 11:42:59.000000 rtds_action-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:43:14.776199 rtds_action-1.1.0/compiled/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 11:42:59.000000 rtds_action-1.1.0/compiled/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)   370866 2023-06-01 11:42:59.000000 rtds_action-1.1.0/compiled/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-01 11:42:59.000000 rtds_action-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:43:14.780199 rtds_action-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-01 11:42:59.000000 rtds_action-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:43:14.776199 rtds_action-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:43:14.780199 rtds_action-1.1.0/src/rtds_action/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-01 11:42:59.000000 rtds_action-1.1.0/src/rtds_action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-01 11:42:59.000000 rtds_action-1.1.0/src/rtds_action/rtds_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 11:43:14.000000 rtds_action-1.1.0/src/rtds_action/rtds_action_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:43:14.780199 rtds_action-1.1.0/src/rtds_action.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-01 11:43:14.000000 rtds_action-1.1.0/src/rtds_action.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 11:43:14.000000 rtds_action-1.1.0/src/rtds_action.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:43:14.000000 rtds_action-1.1.0/src/rtds_action.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:43:14.000000 rtds_action-1.1.0/src/rtds_action.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-01 11:43:14.000000 rtds_action-1.1.0/src/rtds_action.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 11:43:14.000000 rtds_action-1.1.0/src/rtds_action.egg-info/top_level.txt
```

### Comparing `rtds_action-1.0.3/LICENSE` & `rtds_action-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtds_action-1.0.3/PKG-INFO` & `rtds_action-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,159 @@
-Metadata-Version: 2.1
-Name: rtds_action
-Version: 1.0.3
-Summary: Interface GitHub Actions and ReadTheDocs
-Home-page: https://github.com/dfm/rtds-action
-Author: Daniel Foreman-Mackey
-Author-email: foreman.mackey@gmail.com
-Maintainer: Daniel Foreman-Mackey
-Maintainer-email: foreman.mackey@gmail.com
-License: MIT
-Description: # Interface ReadTheDocs and GitHub Actions
-        
-        [![Docs](https://github.com/dfm/rtds-action/workflows/Docs/badge.svg)](https://github.com/dfm/rtds-action/actions?query=workflow%3ADocs)
-        [![Documentation Status](https://readthedocs.org/projects/rtds-action/badge/?version=latest)](https://rtds-action.readthedocs.io/en/latest/?badge=latest)
-        
-        I like to use [ReadTheDocs](https://readthedocs.org/) to build (and version!) my
-        docs, but I _also_ like to use [Jupyter notebooks](https://jupyter.org/) to
-        write tutorials. Unfortunately, this has always meant that I needed to check
-        executed notebooks (often with large images) into my git repository, causing
-        huge amounts of bloat. Futhermore, the executed notebooks would often get out of
-        sync with the development of the code. **No more!!**
-        
-        _This library avoids these issues by executing code on [GitHub
-        Actions](https://github.com/features/actions), uploading build artifacts (in
-        this case, executed Jupter notebooks), and then (only then!) triggering a
-        ReadTheDocs build that can download the executed notebooks._
-        
-        There is still some work required to set up this workflow, but this library has
-        three pieces that make it a bit easier:
-        
-        1. A GitHub action that can be used to trigger a build for the current branch on
-           ReadTheDocs.
-        2. A Sphinx extension that interfaces with the GitHub API to download the
-           artifact produced for the target commit hash.
-        3. Some documentation that shows you how to set all this up!
-        
-        ## Usage
-        
-        The following gives the detailed steps of the process of setting up a project
-        using this workflow. But you can also see a fully functional example in this
-        repository. The documentation source is the `docs` directory and the
-        `.github/workflows` directory includes a workflow that is executed to build the
-        docs using this package. The rendered page is available at
-        [rtds-action.readthedocs.io](https://rtds-action.readthedocs.io).
-        
-        ### 1. Set up ReadTheDocs
-        
-        1. First, you'll need to import your project as usual. If you've already done
-           that, don't worry: this will also work with existing ReadTheDocs projects.
-        2. Next, go to the admin page for your project on ReadTheDocs, click on
-           `Integrations` (the URL is something like
-           `https://readthedocs.org/dashboard/YOUR_PROJECT_NAME/integrations/`).
-        3. Click `Add integration` and select `Generic API incoming webhook`.
-        4. Take note of the webhook `URL` and `token` on this page for use later.
-        
-        You should also edit your webhook settings on GitHub by going to
-        `https://github.com/USERNAME/REPONAME/settings/hooks` and clicking "Edit"
-        next to the ReadTheDocs hook. On that page, you should un-check the `Pushes`
-        option.
-        
-        ### 2. Set up GitHub Actions workflow
-        
-        In this example, we'll assume that we have tutorials written as Jupyter
-        notebooks, saved as Python scripts using
-        [Jupytext](https://jupytext.readthedocs.io/en/latest/introduction.html) (because
-        that's probably what you should be doing anyways!) in a directory called
-        `docs/tutorials`.
-        
-        First, you'll need to add the ReadTheDocs webhook URL and token that you
-        recorded above as "secrets" for your GitHub project by going to the URL
-        `https://github.com/USERNAME/REPONAME/settings/secrets`. I'll call them
-        `RTDS_WEBHOOK_URL` (include the `https`!) and `RTDS_WEBHOOK_TOKEN` respectively.
-        
-        For this use case, we can create the workflow `.github/workflows/docs.yml` as
-        follows:
-        
-        ```yaml
-        name: Docs
-        on: [push, release]
-        
-        jobs:
-          notebooks:
-            name: "Build the notebooks for the docs"
-            runs-on: ubuntu-latest
-            steps:
-              - uses: actions/checkout@v2
-        
-              - name: Set up Python
-                uses: actions/setup-python@v2
-                with:
-                  python-version: 3.8
-        
-              - name: Install dependencies
-                run: |
-                  python -m pip install -U pip
-                  python -m pip install -r .github/workflows/requirements.txt
-        
-              - name: Execute the notebooks
-                run: |
-                  jupytext --to ipynb --execute docs/tutorials/*.py
-        
-              - uses: actions/upload-artifact@v2
-                with:
-                  name: notebooks-for-${{ github.sha }}
-                  path: docs/tutorials
-        
-              - name: Trigger RTDs build
-                uses: dfm/rtds-action@v1
-                with:
-                  webhook_url: ${{ secrets.RTDS_WEBHOOK_URL }}
-                  webhook_token: ${{ secrets.RTDS_WEBHOOK_TOKEN }}
-                  commit_ref: ${{ github.ref }}
-        ```
-        
-        Here, we're also assuming that we've added a `pip` requirements file at
-        `.github/workflows/requirements.txt` with the dependencies required to execute
-        the notebooks. Also note that in the `upload-artifact` step we give our artifact
-        that depends on the hash of the current commit. This is crucial! We also need to
-        take note of the `notebooks-for-` prefix because we'll use that later.
-        
-        It's worth emphasizing here that the only "special" steps in this workflow are
-        the last two. You can do whatever you want to generate your artifact in the
-        previous steps (for example, you could use `conda` instead of `pip`) because
-        this workflow is not picky about how you get there!
-        
-        ### 3. Set up Sphinx
-        
-        Finally, you can edit the `conf.py` for your Sphinx documentation to add support
-        for fetching the artifact produced by your action. Here is a minimal example:
-        
-        ```python
-        import os
-        
-        extensions = [... "rtds_action"]
-        
-        # The name of your GitHub repository
-        rtds_action_github_repo = "USERNAME/REPONAME"
-        
-        # The path where the artifact should be extracted
-        # Note: this is relative to the conf.py file!
-        rtds_action_path = "tutorials"
-        
-        # The "prefix" used in the `upload-artifact` step of the action
-        rtds_action_artifact_prefix = "notebooks-for-"
-        
-        # A GitHub personal access token is required, more info below
-        rtds_action_github_token = os.environ["GITHUB_TOKEN"]
-        
-        # Whether or not to raise an error on ReadTheDocs if the
-        # artifact containing the notebooks can't be downloaded (optional)
-        rtds_action_error_if_missing = False
-        ```
-        
-        Where we have added the custom extension and set the required configuration
-        parameters.
-        
-        You'll need to provide ReadTheDocs with a GitHub personal access token (it only
-        needs the `public_repo` scope if your repo is public). You can generate a new
-        token by going to [your GitHub settings
-        page](https://github.com/settings/tokens). Then, save it as an environment
-        variable (called `GITHUB_TOKEN` in this case) on ReadTheDocs.
-        
-        ## Development
-        
-        For now, just a note: if you edit `src/js/index.js`, you _must_ run `npm run package` to generate the compiled action source.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: dev
+# Interface Read the Docs and GitHub Actions
+
+[![Docs](https://github.com/dfm/rtds-action/workflows/Docs/badge.svg)](https://github.com/dfm/rtds-action/actions?query=workflow%3ADocs)
+[![Documentation Status](https://readthedocs.org/projects/rtds-action/badge/?version=latest)](https://rtds-action.readthedocs.io/en/latest/?badge=latest)
+
+I like to use [Read the Docs](https://readthedocs.org/) to build (and version!) my
+docs, but I _also_ like to use [Jupyter notebooks](https://jupyter.org/) to
+write tutorials. Unfortunately, even though
+[notebooks can be executed on Read the Docs](https://docs.readthedocs.io/en/stable/guides/jupyter.html),
+some of them take a very long time to run or
+need special Docker environments to execute,
+which goes beyond what the platform supports. In these cases I needed to check
+executed notebooks (often with large images) into my git repository, causing
+huge amounts of bloat. Futhermore, the executed notebooks would often get out of
+sync with the development of the code. **No more!!**
+
+_This library avoids these issues by executing code on [GitHub
+Actions](https://github.com/features/actions), uploading build artifacts (in
+this case, executed Jupter notebooks), and then (only then!) triggering a
+Read the Docs build that can download the executed notebooks._
+
+There is still some work required to set up this workflow, but this library has
+three pieces that make it a bit easier:
+
+1. A GitHub action that can be used to trigger a build for the current branch on
+   Read the Docs.
+2. A Sphinx extension that interfaces with the GitHub API to download the
+   artifact produced for the target commit hash.
+3. Some documentation that shows you how to set all this up!
+
+## Usage
+
+The following gives the detailed steps of the process of setting up a project
+using this workflow. But you can also see a fully functional example in this
+repository. The documentation source is the `docs` directory and the
+`.github/workflows` directory includes a workflow that is executed to build the
+docs using this package. The rendered page is available at
+[rtds-action.readthedocs.io](https://rtds-action.readthedocs.io).
+
+### 1. Set up Read the Docs
+
+1. First, you'll need to import your project as usual. If you've already done
+   that, don't worry: this will also work with existing Read the Docs projects.
+2. Next, go to the admin page for your project on Read the Docs, click on
+   `Integrations` (the URL is something like
+   `https://readthedocs.org/dashboard/YOUR_PROJECT_NAME/integrations/`).
+3. Click `Add integration` and select `Generic API incoming webhook`.
+4. Take note of the webhook `URL` and `token` on this page for use later.
+
+You should also edit your webhook settings on GitHub by going to
+`https://github.com/USERNAME/REPONAME/settings/hooks` and clicking "Edit"
+next to the Read the Docs hook. On that page, you should un-check the `Pushes`
+option.
+
+### 2. Set up GitHub Actions workflow
+
+In this example, we'll assume that we have tutorials written as Jupyter
+notebooks, saved as Python scripts using
+[Jupytext](https://jupytext.readthedocs.io/en/latest/introduction.html) (because
+that's probably what you should be doing anyways!) in a directory called
+`docs/tutorials`.
+
+First, you'll need to add the Read the Docs webhook URL and token that you
+recorded above as "secrets" for your GitHub project by going to the URL
+`https://github.com/USERNAME/REPONAME/settings/secrets`. I'll call them
+`RTDS_WEBHOOK_URL` (include the `https`!) and `RTDS_WEBHOOK_TOKEN` respectively.
+
+For this use case, we can create the workflow `.github/workflows/docs.yml` as
+follows:
+
+```yaml
+name: Docs
+on: [push, release]
+
+jobs:
+  notebooks:
+    name: "Build the notebooks for the docs"
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v2
+
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.8
+
+      - name: Install dependencies
+        run: |
+          python -m pip install -U pip
+          python -m pip install -r .github/workflows/requirements.txt
+
+      - name: Execute the notebooks
+        run: |
+          jupytext --to ipynb --execute docs/tutorials/*.py
+
+      - uses: actions/upload-artifact@v2
+        with:
+          name: notebooks-for-${{ github.sha }}
+          path: docs/tutorials
+
+      - name: Trigger RTDs build
+        uses: dfm/rtds-action@v1
+        with:
+          webhook_url: ${{ secrets.RTDS_WEBHOOK_URL }}
+          webhook_token: ${{ secrets.RTDS_WEBHOOK_TOKEN }}
+          commit_ref: ${{ github.ref }}
+```
+
+Here, we're also assuming that we've added a `pip` requirements file at
+`.github/workflows/requirements.txt` with the dependencies required to execute
+the notebooks. Also note that in the `upload-artifact` step we give our artifact
+that depends on the hash of the current commit. This is crucial! We also need to
+take note of the `notebooks-for-` prefix because we'll use that later.
+
+It's worth emphasizing here that the only "special" steps in this workflow are
+the last two. You can do whatever you want to generate your artifact in the
+previous steps (for example, you could use `conda` instead of `pip`) because
+this workflow is not picky about how you get there!
+
+### 3. Set up Sphinx
+
+Finally, you can edit the `conf.py` for your Sphinx documentation to add support
+for fetching the artifact produced by your action. Here is a minimal example:
+
+```python
+import os
+
+extensions = [... "rtds_action"]
+
+# The name of your GitHub repository
+rtds_action_github_repo = "USERNAME/REPONAME"
+
+# The path where the artifact should be extracted
+# Note: this is relative to the conf.py file!
+rtds_action_path = "tutorials"
+
+# The "prefix" used in the `upload-artifact` step of the action
+rtds_action_artifact_prefix = "notebooks-for-"
+
+# A GitHub personal access token is required, more info below
+rtds_action_github_token = os.environ["GITHUB_TOKEN"]
+
+# Whether or not to raise an error on Read the Docs if the
+# artifact containing the notebooks can't be downloaded (optional)
+rtds_action_error_if_missing = False
+```
+
+Where we have added the custom extension and set the required configuration
+parameters.
+
+You'll need to provide Read the Docs with a GitHub personal access token (it only
+needs the `public_repo` scope if your repo is public). You can generate a new
+token by going to [your GitHub settings
+page](https://github.com/settings/tokens). Then, save it as an environment
+variable (called `GITHUB_TOKEN` in this case) on Read the Docs.
+
+## Development
+
+For now, just a note: if you edit `src/js/index.js`, you _must_ run `npm run package` to generate the compiled action source.
```

### Comparing `rtds_action-1.0.3/README.md` & `rtds_action-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,91 @@
-# Interface ReadTheDocs and GitHub Actions
+Metadata-Version: 2.1
+Name: rtds_action
+Version: 1.1.0
+Summary: Interface GitHub Actions and ReadTheDocs
+Home-page: https://github.com/dfm/rtds-action
+Author: Daniel Foreman-Mackey
+Author-email: foreman.mackey@gmail.com
+Maintainer: Daniel Foreman-Mackey
+Maintainer-email: foreman.mackey@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: dev
+License-File: LICENSE
+
+# Interface Read the Docs and GitHub Actions
 
 [![Docs](https://github.com/dfm/rtds-action/workflows/Docs/badge.svg)](https://github.com/dfm/rtds-action/actions?query=workflow%3ADocs)
 [![Documentation Status](https://readthedocs.org/projects/rtds-action/badge/?version=latest)](https://rtds-action.readthedocs.io/en/latest/?badge=latest)
 
-I like to use [ReadTheDocs](https://readthedocs.org/) to build (and version!) my
+I like to use [Read the Docs](https://readthedocs.org/) to build (and version!) my
 docs, but I _also_ like to use [Jupyter notebooks](https://jupyter.org/) to
-write tutorials. Unfortunately, this has always meant that I needed to check
+write tutorials. Unfortunately, even though
+[notebooks can be executed on Read the Docs](https://docs.readthedocs.io/en/stable/guides/jupyter.html),
+some of them take a very long time to run or
+need special Docker environments to execute,
+which goes beyond what the platform supports. In these cases I needed to check
 executed notebooks (often with large images) into my git repository, causing
 huge amounts of bloat. Futhermore, the executed notebooks would often get out of
 sync with the development of the code. **No more!!**
 
 _This library avoids these issues by executing code on [GitHub
 Actions](https://github.com/features/actions), uploading build artifacts (in
 this case, executed Jupter notebooks), and then (only then!) triggering a
-ReadTheDocs build that can download the executed notebooks._
+Read the Docs build that can download the executed notebooks._
 
 There is still some work required to set up this workflow, but this library has
 three pieces that make it a bit easier:
 
 1. A GitHub action that can be used to trigger a build for the current branch on
-   ReadTheDocs.
+   Read the Docs.
 2. A Sphinx extension that interfaces with the GitHub API to download the
    artifact produced for the target commit hash.
 3. Some documentation that shows you how to set all this up!
 
 ## Usage
 
 The following gives the detailed steps of the process of setting up a project
 using this workflow. But you can also see a fully functional example in this
 repository. The documentation source is the `docs` directory and the
 `.github/workflows` directory includes a workflow that is executed to build the
 docs using this package. The rendered page is available at
 [rtds-action.readthedocs.io](https://rtds-action.readthedocs.io).
 
-### 1. Set up ReadTheDocs
+### 1. Set up Read the Docs
 
 1. First, you'll need to import your project as usual. If you've already done
-   that, don't worry: this will also work with existing ReadTheDocs projects.
-2. Next, go to the admin page for your project on ReadTheDocs, click on
+   that, don't worry: this will also work with existing Read the Docs projects.
+2. Next, go to the admin page for your project on Read the Docs, click on
    `Integrations` (the URL is something like
    `https://readthedocs.org/dashboard/YOUR_PROJECT_NAME/integrations/`).
 3. Click `Add integration` and select `Generic API incoming webhook`.
 4. Take note of the webhook `URL` and `token` on this page for use later.
 
 You should also edit your webhook settings on GitHub by going to
 `https://github.com/USERNAME/REPONAME/settings/hooks` and clicking "Edit"
-next to the ReadTheDocs hook. On that page, you should un-check the `Pushes`
+next to the Read the Docs hook. On that page, you should un-check the `Pushes`
 option.
 
 ### 2. Set up GitHub Actions workflow
 
 In this example, we'll assume that we have tutorials written as Jupyter
 notebooks, saved as Python scripts using
 [Jupytext](https://jupytext.readthedocs.io/en/latest/introduction.html) (because
 that's probably what you should be doing anyways!) in a directory called
 `docs/tutorials`.
 
-First, you'll need to add the ReadTheDocs webhook URL and token that you
+First, you'll need to add the Read the Docs webhook URL and token that you
 recorded above as "secrets" for your GitHub project by going to the URL
 `https://github.com/USERNAME/REPONAME/settings/secrets`. I'll call them
 `RTDS_WEBHOOK_URL` (include the `https`!) and `RTDS_WEBHOOK_TOKEN` respectively.
 
 For this use case, we can create the workflow `.github/workflows/docs.yml` as
 follows:
 
@@ -132,24 +157,24 @@
 
 # The "prefix" used in the `upload-artifact` step of the action
 rtds_action_artifact_prefix = "notebooks-for-"
 
 # A GitHub personal access token is required, more info below
 rtds_action_github_token = os.environ["GITHUB_TOKEN"]
 
-# Whether or not to raise an error on ReadTheDocs if the
+# Whether or not to raise an error on Read the Docs if the
 # artifact containing the notebooks can't be downloaded (optional)
 rtds_action_error_if_missing = False
 ```
 
 Where we have added the custom extension and set the required configuration
 parameters.
 
-You'll need to provide ReadTheDocs with a GitHub personal access token (it only
+You'll need to provide Read the Docs with a GitHub personal access token (it only
 needs the `public_repo` scope if your repo is public). You can generate a new
 token by going to [your GitHub settings
 page](https://github.com/settings/tokens). Then, save it as an environment
-variable (called `GITHUB_TOKEN` in this case) on ReadTheDocs.
+variable (called `GITHUB_TOKEN` in this case) on Read the Docs.
 
 ## Development
 
 For now, just a note: if you edit `src/js/index.js`, you _must_ run `npm run package` to generate the compiled action source.
```

### Comparing `rtds_action-1.0.3/setup.py` & `rtds_action-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `rtds_action-1.0.3/src/rtds_action/rtds_action.py` & `rtds_action-1.1.0/src/rtds_action/rtds_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     except subprocess.CalledProcessError:
         logger.warn("rtds_action: can't get git hash")
         return
 
     r = requests.get(
         f"https://api.github.com/repos/{repo}/actions/artifacts",
         params=dict(per_page=100),
+        headers={"Authorization": f"token {token}"},
     )
     if r.status_code != 200:
         logger.warn(f"Can't list files ({r.status_code})")
         return
 
     expected_name = f"{prefix}{git_hash}"
     result = r.json()
```

### Comparing `rtds_action-1.0.3/src/rtds_action.egg-info/PKG-INFO` & `rtds_action-1.1.0/src/rtds_action.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,180 @@
 Metadata-Version: 2.1
 Name: rtds-action
-Version: 1.0.3
+Version: 1.1.0
 Summary: Interface GitHub Actions and ReadTheDocs
 Home-page: https://github.com/dfm/rtds-action
 Author: Daniel Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Maintainer: Daniel Foreman-Mackey
 Maintainer-email: foreman.mackey@gmail.com
 License: MIT
-Description: # Interface ReadTheDocs and GitHub Actions
-        
-        [![Docs](https://github.com/dfm/rtds-action/workflows/Docs/badge.svg)](https://github.com/dfm/rtds-action/actions?query=workflow%3ADocs)
-        [![Documentation Status](https://readthedocs.org/projects/rtds-action/badge/?version=latest)](https://rtds-action.readthedocs.io/en/latest/?badge=latest)
-        
-        I like to use [ReadTheDocs](https://readthedocs.org/) to build (and version!) my
-        docs, but I _also_ like to use [Jupyter notebooks](https://jupyter.org/) to
-        write tutorials. Unfortunately, this has always meant that I needed to check
-        executed notebooks (often with large images) into my git repository, causing
-        huge amounts of bloat. Futhermore, the executed notebooks would often get out of
-        sync with the development of the code. **No more!!**
-        
-        _This library avoids these issues by executing code on [GitHub
-        Actions](https://github.com/features/actions), uploading build artifacts (in
-        this case, executed Jupter notebooks), and then (only then!) triggering a
-        ReadTheDocs build that can download the executed notebooks._
-        
-        There is still some work required to set up this workflow, but this library has
-        three pieces that make it a bit easier:
-        
-        1. A GitHub action that can be used to trigger a build for the current branch on
-           ReadTheDocs.
-        2. A Sphinx extension that interfaces with the GitHub API to download the
-           artifact produced for the target commit hash.
-        3. Some documentation that shows you how to set all this up!
-        
-        ## Usage
-        
-        The following gives the detailed steps of the process of setting up a project
-        using this workflow. But you can also see a fully functional example in this
-        repository. The documentation source is the `docs` directory and the
-        `.github/workflows` directory includes a workflow that is executed to build the
-        docs using this package. The rendered page is available at
-        [rtds-action.readthedocs.io](https://rtds-action.readthedocs.io).
-        
-        ### 1. Set up ReadTheDocs
-        
-        1. First, you'll need to import your project as usual. If you've already done
-           that, don't worry: this will also work with existing ReadTheDocs projects.
-        2. Next, go to the admin page for your project on ReadTheDocs, click on
-           `Integrations` (the URL is something like
-           `https://readthedocs.org/dashboard/YOUR_PROJECT_NAME/integrations/`).
-        3. Click `Add integration` and select `Generic API incoming webhook`.
-        4. Take note of the webhook `URL` and `token` on this page for use later.
-        
-        You should also edit your webhook settings on GitHub by going to
-        `https://github.com/USERNAME/REPONAME/settings/hooks` and clicking "Edit"
-        next to the ReadTheDocs hook. On that page, you should un-check the `Pushes`
-        option.
-        
-        ### 2. Set up GitHub Actions workflow
-        
-        In this example, we'll assume that we have tutorials written as Jupyter
-        notebooks, saved as Python scripts using
-        [Jupytext](https://jupytext.readthedocs.io/en/latest/introduction.html) (because
-        that's probably what you should be doing anyways!) in a directory called
-        `docs/tutorials`.
-        
-        First, you'll need to add the ReadTheDocs webhook URL and token that you
-        recorded above as "secrets" for your GitHub project by going to the URL
-        `https://github.com/USERNAME/REPONAME/settings/secrets`. I'll call them
-        `RTDS_WEBHOOK_URL` (include the `https`!) and `RTDS_WEBHOOK_TOKEN` respectively.
-        
-        For this use case, we can create the workflow `.github/workflows/docs.yml` as
-        follows:
-        
-        ```yaml
-        name: Docs
-        on: [push, release]
-        
-        jobs:
-          notebooks:
-            name: "Build the notebooks for the docs"
-            runs-on: ubuntu-latest
-            steps:
-              - uses: actions/checkout@v2
-        
-              - name: Set up Python
-                uses: actions/setup-python@v2
-                with:
-                  python-version: 3.8
-        
-              - name: Install dependencies
-                run: |
-                  python -m pip install -U pip
-                  python -m pip install -r .github/workflows/requirements.txt
-        
-              - name: Execute the notebooks
-                run: |
-                  jupytext --to ipynb --execute docs/tutorials/*.py
-        
-              - uses: actions/upload-artifact@v2
-                with:
-                  name: notebooks-for-${{ github.sha }}
-                  path: docs/tutorials
-        
-              - name: Trigger RTDs build
-                uses: dfm/rtds-action@v1
-                with:
-                  webhook_url: ${{ secrets.RTDS_WEBHOOK_URL }}
-                  webhook_token: ${{ secrets.RTDS_WEBHOOK_TOKEN }}
-                  commit_ref: ${{ github.ref }}
-        ```
-        
-        Here, we're also assuming that we've added a `pip` requirements file at
-        `.github/workflows/requirements.txt` with the dependencies required to execute
-        the notebooks. Also note that in the `upload-artifact` step we give our artifact
-        that depends on the hash of the current commit. This is crucial! We also need to
-        take note of the `notebooks-for-` prefix because we'll use that later.
-        
-        It's worth emphasizing here that the only "special" steps in this workflow are
-        the last two. You can do whatever you want to generate your artifact in the
-        previous steps (for example, you could use `conda` instead of `pip`) because
-        this workflow is not picky about how you get there!
-        
-        ### 3. Set up Sphinx
-        
-        Finally, you can edit the `conf.py` for your Sphinx documentation to add support
-        for fetching the artifact produced by your action. Here is a minimal example:
-        
-        ```python
-        import os
-        
-        extensions = [... "rtds_action"]
-        
-        # The name of your GitHub repository
-        rtds_action_github_repo = "USERNAME/REPONAME"
-        
-        # The path where the artifact should be extracted
-        # Note: this is relative to the conf.py file!
-        rtds_action_path = "tutorials"
-        
-        # The "prefix" used in the `upload-artifact` step of the action
-        rtds_action_artifact_prefix = "notebooks-for-"
-        
-        # A GitHub personal access token is required, more info below
-        rtds_action_github_token = os.environ["GITHUB_TOKEN"]
-        
-        # Whether or not to raise an error on ReadTheDocs if the
-        # artifact containing the notebooks can't be downloaded (optional)
-        rtds_action_error_if_missing = False
-        ```
-        
-        Where we have added the custom extension and set the required configuration
-        parameters.
-        
-        You'll need to provide ReadTheDocs with a GitHub personal access token (it only
-        needs the `public_repo` scope if your repo is public). You can generate a new
-        token by going to [your GitHub settings
-        page](https://github.com/settings/tokens). Then, save it as an environment
-        variable (called `GITHUB_TOKEN` in this case) on ReadTheDocs.
-        
-        ## Development
-        
-        For now, just a note: if you edit `src/js/index.js`, you _must_ run `npm run package` to generate the compiled action source.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: dev
+License-File: LICENSE
+
+# Interface Read the Docs and GitHub Actions
+
+[![Docs](https://github.com/dfm/rtds-action/workflows/Docs/badge.svg)](https://github.com/dfm/rtds-action/actions?query=workflow%3ADocs)
+[![Documentation Status](https://readthedocs.org/projects/rtds-action/badge/?version=latest)](https://rtds-action.readthedocs.io/en/latest/?badge=latest)
+
+I like to use [Read the Docs](https://readthedocs.org/) to build (and version!) my
+docs, but I _also_ like to use [Jupyter notebooks](https://jupyter.org/) to
+write tutorials. Unfortunately, even though
+[notebooks can be executed on Read the Docs](https://docs.readthedocs.io/en/stable/guides/jupyter.html),
+some of them take a very long time to run or
+need special Docker environments to execute,
+which goes beyond what the platform supports. In these cases I needed to check
+executed notebooks (often with large images) into my git repository, causing
+huge amounts of bloat. Futhermore, the executed notebooks would often get out of
+sync with the development of the code. **No more!!**
+
+_This library avoids these issues by executing code on [GitHub
+Actions](https://github.com/features/actions), uploading build artifacts (in
+this case, executed Jupter notebooks), and then (only then!) triggering a
+Read the Docs build that can download the executed notebooks._
+
+There is still some work required to set up this workflow, but this library has
+three pieces that make it a bit easier:
+
+1. A GitHub action that can be used to trigger a build for the current branch on
+   Read the Docs.
+2. A Sphinx extension that interfaces with the GitHub API to download the
+   artifact produced for the target commit hash.
+3. Some documentation that shows you how to set all this up!
+
+## Usage
+
+The following gives the detailed steps of the process of setting up a project
+using this workflow. But you can also see a fully functional example in this
+repository. The documentation source is the `docs` directory and the
+`.github/workflows` directory includes a workflow that is executed to build the
+docs using this package. The rendered page is available at
+[rtds-action.readthedocs.io](https://rtds-action.readthedocs.io).
+
+### 1. Set up Read the Docs
+
+1. First, you'll need to import your project as usual. If you've already done
+   that, don't worry: this will also work with existing Read the Docs projects.
+2. Next, go to the admin page for your project on Read the Docs, click on
+   `Integrations` (the URL is something like
+   `https://readthedocs.org/dashboard/YOUR_PROJECT_NAME/integrations/`).
+3. Click `Add integration` and select `Generic API incoming webhook`.
+4. Take note of the webhook `URL` and `token` on this page for use later.
+
+You should also edit your webhook settings on GitHub by going to
+`https://github.com/USERNAME/REPONAME/settings/hooks` and clicking "Edit"
+next to the Read the Docs hook. On that page, you should un-check the `Pushes`
+option.
+
+### 2. Set up GitHub Actions workflow
+
+In this example, we'll assume that we have tutorials written as Jupyter
+notebooks, saved as Python scripts using
+[Jupytext](https://jupytext.readthedocs.io/en/latest/introduction.html) (because
+that's probably what you should be doing anyways!) in a directory called
+`docs/tutorials`.
+
+First, you'll need to add the Read the Docs webhook URL and token that you
+recorded above as "secrets" for your GitHub project by going to the URL
+`https://github.com/USERNAME/REPONAME/settings/secrets`. I'll call them
+`RTDS_WEBHOOK_URL` (include the `https`!) and `RTDS_WEBHOOK_TOKEN` respectively.
+
+For this use case, we can create the workflow `.github/workflows/docs.yml` as
+follows:
+
+```yaml
+name: Docs
+on: [push, release]
+
+jobs:
+  notebooks:
+    name: "Build the notebooks for the docs"
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v2
+
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: 3.8
+
+      - name: Install dependencies
+        run: |
+          python -m pip install -U pip
+          python -m pip install -r .github/workflows/requirements.txt
+
+      - name: Execute the notebooks
+        run: |
+          jupytext --to ipynb --execute docs/tutorials/*.py
+
+      - uses: actions/upload-artifact@v2
+        with:
+          name: notebooks-for-${{ github.sha }}
+          path: docs/tutorials
+
+      - name: Trigger RTDs build
+        uses: dfm/rtds-action@v1
+        with:
+          webhook_url: ${{ secrets.RTDS_WEBHOOK_URL }}
+          webhook_token: ${{ secrets.RTDS_WEBHOOK_TOKEN }}
+          commit_ref: ${{ github.ref }}
+```
+
+Here, we're also assuming that we've added a `pip` requirements file at
+`.github/workflows/requirements.txt` with the dependencies required to execute
+the notebooks. Also note that in the `upload-artifact` step we give our artifact
+that depends on the hash of the current commit. This is crucial! We also need to
+take note of the `notebooks-for-` prefix because we'll use that later.
+
+It's worth emphasizing here that the only "special" steps in this workflow are
+the last two. You can do whatever you want to generate your artifact in the
+previous steps (for example, you could use `conda` instead of `pip`) because
+this workflow is not picky about how you get there!
+
+### 3. Set up Sphinx
+
+Finally, you can edit the `conf.py` for your Sphinx documentation to add support
+for fetching the artifact produced by your action. Here is a minimal example:
+
+```python
+import os
+
+extensions = [... "rtds_action"]
+
+# The name of your GitHub repository
+rtds_action_github_repo = "USERNAME/REPONAME"
+
+# The path where the artifact should be extracted
+# Note: this is relative to the conf.py file!
+rtds_action_path = "tutorials"
+
+# The "prefix" used in the `upload-artifact` step of the action
+rtds_action_artifact_prefix = "notebooks-for-"
+
+# A GitHub personal access token is required, more info below
+rtds_action_github_token = os.environ["GITHUB_TOKEN"]
+
+# Whether or not to raise an error on Read the Docs if the
+# artifact containing the notebooks can't be downloaded (optional)
+rtds_action_error_if_missing = False
+```
+
+Where we have added the custom extension and set the required configuration
+parameters.
+
+You'll need to provide Read the Docs with a GitHub personal access token (it only
+needs the `public_repo` scope if your repo is public). You can generate a new
+token by going to [your GitHub settings
+page](https://github.com/settings/tokens). Then, save it as an environment
+variable (called `GITHUB_TOKEN` in this case) on Read the Docs.
+
+## Development
+
+For now, just a note: if you edit `src/js/index.js`, you _must_ run `npm run package` to generate the compiled action source.
```

