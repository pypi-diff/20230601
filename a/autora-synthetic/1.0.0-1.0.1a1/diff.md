# Comparing `tmp/autora-synthetic-1.0.0.tar.gz` & `tmp/autora-synthetic-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-synthetic-1.0.0.tar", last modified: Wed May 31 19:06:09 2023, max compression
+gzip compressed data, was "autora-synthetic-1.0.1a1.tar", last modified: Thu Jun  1 15:40:00 2023, max compression
```

## Comparing `autora-synthetic-1.0.0.tar` & `autora-synthetic-1.0.1a1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.934526 autora-synthetic-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.914526 autora-synthetic-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.922526 autora-synthetic-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.926526 autora-synthetic-1.0.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.idea/autora-synthetic.iml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-31 19:06:09.934526 autora-synthetic-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.926526 autora-synthetic-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   171006 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/docs/Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.926526 autora-synthetic-1.0.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.926526 autora-synthetic-1.0.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:06:09.934526 autora-synthetic-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.918526 autora-synthetic-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.918526 autora-synthetic-1.0.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.930526 autora-synthetic-1.0.0/src/autora/synthetic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.930526 autora-synthetic-1.0.0/src/autora/synthetic/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/src/autora/synthetic/abstract/template_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.930526 autora-synthetic-1.0.0/src/autora/synthetic/economics/
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/src/autora/synthetic/economics/expected_value_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/src/autora/synthetic/economics/prospect_theory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.930526 autora-synthetic-1.0.0/src/autora/synthetic/psychophysics/
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/src/autora/synthetic/psychophysics/weber_fechner_law.py
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/src/autora/synthetic/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.934526 autora-synthetic-1.0.0/src/autora_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-31 19:06:09.000000 autora-synthetic-1.0.0/src/autora_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-31 19:06:09.000000 autora-synthetic-1.0.0/src/autora_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:06:09.000000 autora-synthetic-1.0.0/src/autora_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-31 19:06:09.000000 autora-synthetic-1.0.0/src/autora_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:06:09.000000 autora-synthetic-1.0.0/src/autora_synthetic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:06:09.934526 autora-synthetic-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/tests/test_bundled_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-31 19:05:55.000000 autora-synthetic-1.0.0/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.939991 autora-synthetic-1.0.1a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.947991 autora-synthetic-1.0.1a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/autora-synthetic.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   171060 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/docs/Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.943991 autora-synthetic-1.0.1a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.943991 autora-synthetic-1.0.1a1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.943991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/abstract/template_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/prospect_theory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/psychophysics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/tests/test_bundled_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-1.0.0/.github/workflows/python-publish.yml` & `autora-synthetic-1.0.1a1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.0/.github/workflows/test-pytest.yml` & `autora-synthetic-1.0.1a1/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.0/.gitignore` & `autora-synthetic-1.0.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.0/.idea/autora-synthetic.iml` & `autora-synthetic-1.0.1a1/.idea/autora-synthetic.iml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.0/.pre-commit-config.yaml` & `autora-synthetic-1.0.1a1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,14 @@
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
         args:
         - "--max-line-length=100"
         - "--extend-ignore=E203"
-        - "--per-file-ignores=__init__.py:F401"
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.3.0"
     hooks:
       - id: mypy
         additional_dependencies: [types-requests]
         language_version: python3.8
   - repo: https://github.com/srstevenson/nb-clean
```

### Comparing `autora-synthetic-1.0.0/CONTRIBUTING.md` & `autora-synthetic-1.0.1a1/CONTRIBUTING.md`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 Activate the pre-commit hooks:
 ```shell
 pre-commit install
 ```
 
 ## Add a new dataset
 
-New datasets should match existing examples in [`src/autora/synthetic/`](src/autora/synthetic/). 
+New datasets should match existing examples in 
+[`src/autora/experiment_runner/synthetic/`](src/autora/experiment_runner/synthetic/). 
 > 💡A good starting point might be to duplicate an existing example.
 
 Each experiment is described in a single file which includes a "factory function" which:
 - constructs the experiment, and 
 - optionally takes parameters to tune aspects of the experiment.  
 
 New experiments fulfilling these requirements can be submitted as pull requests.
```

### Comparing `autora-synthetic-1.0.0/PKG-INFO` & `autora-synthetic-1.0.1a1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic
-Version: 1.0.0
+Version: 1.0.1a1
 Summary: AutoRA Synthetic Experiments
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic
 Project-URL: documentation, https://autoresearch.github.io/autora-synthetic/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -26,10 +26,16 @@
 pip install -U "autora[synthetic-data]" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
-python -c "from autora.synthetic.economics.prospect_theory import prospect_theory; print(prospect_theory().description)"
+python -c "
+from autora.experiment_runner.synthetic.economics.prospect_theory import prospect_theory
+study = prospect_theory()
+print(study.description)
+"
 ```
 
+For more information, see the
+[documentation](https://autoresearch.github.io/autora/user-guide/experiment-runners/synthetic/).
```

### Comparing `autora-synthetic-1.0.0/README.md` & `autora-synthetic-1.0.1a1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -14,10 +14,16 @@
 pip install -U "autora[synthetic-data]" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
-python -c "from autora.synthetic.economics.prospect_theory import prospect_theory; print(prospect_theory().description)"
+python -c "
+from autora.experiment_runner.synthetic.economics.prospect_theory import prospect_theory
+study = prospect_theory()
+print(study.description)
+"
 ```
 
+For more information, see the
+[documentation](https://autoresearch.github.io/autora/user-guide/experiment-runners/synthetic/).
```

### Comparing `autora-synthetic-1.0.0/docs/Example.ipynb` & `autora-synthetic-1.0.1a1/docs/Example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994435817805383%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(1, 'from "*

 * *            'autora.experiment_runner.synthetic.psychophysics.weber_fechner_law import '*

 * *            "weber_fechner_law\\n')], delete: [1]}}, 5: {'outputs': {0: {'text': {insert: [(0, "*

 * *            "'Help on function weber_fechner_law in module "*

 * *            "autora.experiment_runner.synthetic.psychophysics.weber_fechner_law:\\n')], delete: "*

 * *            "[0]}}}}, 7: {'source': {insert: [(0, 'from "*

 * *            "autora.experiment_runner.synthetic.utilities i […]*

```diff
@@ -27,15 +27,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
-                "from autora.synthetic.psychophysics.weber_fechner_law import weber_fechner_law\n",
+                "from autora.experiment_runner.synthetic.psychophysics.weber_fechner_law import weber_fechner_law\n",
                 "s = weber_fechner_law(random_state=None)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -47,15 +47,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Help on function weber_fechner_law in module autora.synthetic.psychophysics.weber_fechner_law:\n",
+                        "Help on function weber_fechner_law in module autora.experiment_runner.synthetic.psychophysics.weber_fechner_law:\n",
                         "\n",
                         "weber_fechner_law(name='Weber-Fechner Law', resolution=100, constant=1.0, maximum_stimulus_intensity=5.0, added_noise=0.01, random_state: Optional[int] = None)\n",
                         "    Weber-Fechner Law\n",
                         "    \n",
                         "    Args:\n",
                         "        name: name of the experiment\n",
                         "        resolution: number of allowed values for stimulus 1 and 2\n",
@@ -99,15 +99,15 @@
                         "        random_state: integer used to seed the random number generator\n",
                         "\n",
                         "    \n"
                     ]
                 }
             ],
             "source": [
-                "from autora.synthetic.utilities import describe\n",
+                "from autora.experiment_runner.synthetic.utilities import describe\n",
                 "\n",
                 "print(describe(s))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `autora-synthetic-1.0.0/docs/index.md` & `autora-synthetic-1.0.1a1/docs/index.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,9 +15,13 @@
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
-python -c "from autora.synthetic.economics.prospect_theory import prospect_theory; print(prospect_theory().description)"
+python -c "
+from autora.experiment_runner.synthetic.economics.prospect_theory import prospect_theory
+study = prospect_theory()
+print(study.description)
+"
 ```
```

### Comparing `autora-synthetic-1.0.0/mkdocs/base.yml` & `autora-synthetic-1.0.1a1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.0/pyproject.toml` & `autora-synthetic-1.0.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.0/src/autora/synthetic/abstract/template_experiment.py` & `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/abstract/template_experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 A template synthetic experiment.
 
 Examples:
-    >>> from autora.synthetic.abstract.template_experiment import template_experiment
+    >>> from autora.experiment_runner.synthetic.abstract.template_experiment import (
+    ...     template_experiment
+    ... )
 
     We can instantiate the experiment using the imported function
     >>> s = template_experiment()
     >>> s  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
     SyntheticExperimentCollection(name='Template Experiment', description='...',
         params={'name': ...}, ...)
 
@@ -60,15 +62,15 @@
 
 
 from functools import partial
 
 import numpy as np
 from numpy.typing import ArrayLike
 
-from autora.synthetic.utilities import SyntheticExperimentCollection
+from autora.experiment_runner.synthetic.utilities import SyntheticExperimentCollection
 from autora.variable import DV, IV, VariableCollection
 
 
 def template_experiment(
     # Add any configurable parameters with their defaults here:
     name: str = "Template Experiment",
     added_noise: float = 0.1,
```

### Comparing `autora-synthetic-1.0.0/src/autora/synthetic/economics/expected_value_theory.py` & `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import partial
 
 import numpy as np
 
-from autora.synthetic.utilities import SyntheticExperimentCollection
+from autora.experiment_runner.synthetic.utilities import SyntheticExperimentCollection
 from autora.variable import DV, IV, ValueType, VariableCollection
 
 
 def get_variables(minimum_value, maximum_value, resolution):
     v_a = IV(
         name="V_A",
         allowed_values=np.linspace(
```

### Comparing `autora-synthetic-1.0.0/src/autora/synthetic/economics/prospect_theory.py` & `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/prospect_theory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from functools import partial
 
 import numpy as np
 
-from autora.synthetic.economics.expected_value_theory import get_variables
-from autora.synthetic.utilities import SyntheticExperimentCollection
+from autora.experiment_runner.synthetic.economics.expected_value_theory import (
+    get_variables,
+)
+from autora.experiment_runner.synthetic.utilities import SyntheticExperimentCollection
 
 
 def prospect_theory(
     name="Prospect Theory",
     added_noise=0.01,
     choice_temperature=0.1,
     value_alpha=0.88,
```

### Comparing `autora-synthetic-1.0.0/src/autora/synthetic/psychophysics/weber_fechner_law.py` & `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 from typing import Optional
 
 import numpy as np
 
-from autora.synthetic.utilities import SyntheticExperimentCollection
+from autora.experiment_runner.synthetic.utilities import SyntheticExperimentCollection
 from autora.variable import DV, IV, ValueType, VariableCollection
 
 
 def weber_fechner_law(
     name="Weber-Fechner Law",
     resolution=100,
     constant=1.0,
```

### Comparing `autora-synthetic-1.0.0/src/autora/synthetic/utilities.py` & `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Examples:
     To add and recover a new model from the inventory, we need to define it using a factory
     function.
     We start by importing the modules we'll need:
     >>> from functools import partial
     >>> import matplotlib.pyplot as plt
     >>> import numpy as np
-    >>> from autora.synthetic.utilities import (register, retrieve, describe,
+    >>> from autora.experiment_runner.synthetic.utilities import (register, retrieve, describe,
     ...     SyntheticExperimentCollection)
     >>> from autora.variable import IV, DV, VariableCollection
 
     Then we can define the function. We define all the arguments we want and add them to a
     dictionary. The factory_function – in this case `sinusoid_experiment` – is the scope for all
     the parameters we need.
     >>> def sinusoid_experiment(omega=np.pi/3, delta=np.pi/2., m=0.3, resolution=1000,
```

### Comparing `autora-synthetic-1.0.0/src/autora_synthetic.egg-info/PKG-INFO` & `autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic
-Version: 1.0.0
+Version: 1.0.1a1
 Summary: AutoRA Synthetic Experiments
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic
 Project-URL: documentation, https://autoresearch.github.io/autora-synthetic/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -26,10 +26,16 @@
 pip install -U "autora[synthetic-data]" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
-python -c "from autora.synthetic.economics.prospect_theory import prospect_theory; print(prospect_theory().description)"
+python -c "
+from autora.experiment_runner.synthetic.economics.prospect_theory import prospect_theory
+study = prospect_theory()
+print(study.description)
+"
 ```
 
+For more information, see the
+[documentation](https://autoresearch.github.io/autora/user-guide/experiment-runners/synthetic/).
```

### Comparing `autora-synthetic-1.0.0/src/autora_synthetic.egg-info/SOURCES.txt` & `autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 .idea/misc.xml
 .idea/modules.xml
 .idea/vcs.xml
 docs/Example.ipynb
 docs/index.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
-src/autora/synthetic/utilities.py
-src/autora/synthetic/abstract/template_experiment.py
-src/autora/synthetic/economics/expected_value_theory.py
-src/autora/synthetic/economics/prospect_theory.py
-src/autora/synthetic/psychophysics/weber_fechner_law.py
+src/autora/experiment_runner/synthetic/utilities.py
+src/autora/experiment_runner/synthetic/abstract/template_experiment.py
+src/autora/experiment_runner/synthetic/economics/expected_value_theory.py
+src/autora/experiment_runner/synthetic/economics/prospect_theory.py
+src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py
 src/autora_synthetic.egg-info/PKG-INFO
 src/autora_synthetic.egg-info/SOURCES.txt
 src/autora_synthetic.egg-info/dependency_links.txt
 src/autora_synthetic.egg-info/requires.txt
 src/autora_synthetic.egg-info/top_level.txt
 tests/test_bundled_models.py
 tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-1.0.0/tests/test_bundled_models.py` & `autora-synthetic-1.0.1a1/tests/test_bundled_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from hypothesis import given
 from hypothesis import strategies as st
 
-from autora.synthetic.abstract.template_experiment import template_experiment
-from autora.synthetic.economics.expected_value_theory import expected_value_theory
-from autora.synthetic.economics.prospect_theory import prospect_theory
-from autora.synthetic.psychophysics.weber_fechner_law import weber_fechner_law
-from autora.synthetic.utilities import describe, register, retrieve
+from autora.experiment_runner.synthetic.abstract.template_experiment import (
+    template_experiment,
+)
+from autora.experiment_runner.synthetic.economics.expected_value_theory import (
+    expected_value_theory,
+)
+from autora.experiment_runner.synthetic.economics.prospect_theory import prospect_theory
+from autora.experiment_runner.synthetic.psychophysics.weber_fechner_law import (
+    weber_fechner_law,
+)
+from autora.experiment_runner.synthetic.utilities import describe, register, retrieve
 
 all_bundled_models = [
     ("expected_value_theory", expected_value_theory),
     ("prospect_theory", prospect_theory),
     ("template_experiment", template_experiment),
     ("weber_fechner_law", weber_fechner_law),
 ]
```

### Comparing `autora-synthetic-1.0.0/tests/test_synthetic_inventory.py` & `autora-synthetic-1.0.1a1/tests/test_synthetic_inventory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from hypothesis import assume, given
 from hypothesis import strategies as st
 
-from autora.synthetic.utilities import SyntheticExperimentCollection, register, retrieve
+from autora.experiment_runner.synthetic.utilities import (
+    SyntheticExperimentCollection,
+    register,
+    retrieve,
+)
 
 
 @given(st.text())
 def test_model_registration_retrieval_allows_any_string(name):
     model = SyntheticExperimentCollection()
     register(name, lambda: model)
```

