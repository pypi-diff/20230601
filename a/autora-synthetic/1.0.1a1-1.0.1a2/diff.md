# Comparing `tmp/autora-synthetic-1.0.1a1.tar.gz` & `tmp/autora-synthetic-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-synthetic-1.0.1a1.tar", last modified: Thu Jun  1 15:40:00 2023, max compression
+gzip compressed data, was "autora-synthetic-1.0.1a2.tar", last modified: Thu Jun  1 17:47:08 2023, max compression
```

## Comparing `autora-synthetic-1.0.1a1.tar` & `autora-synthetic-1.0.1a2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.939991 autora-synthetic-1.0.1a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.947991 autora-synthetic-1.0.1a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.github/workflows/docs-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/autora-synthetic.iml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   171060 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/docs/Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.943991 autora-synthetic-1.0.1a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.943991 autora-synthetic-1.0.1a1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.943991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/abstract/template_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.951991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/prospect_theory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/psychophysics/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 15:40:00.000000 autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:40:00.955991 autora-synthetic-1.0.1a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/tests/test_bundled_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-01 15:39:47.000000 autora-synthetic-1.0.1a1/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.005811 autora-synthetic-1.0.1a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:07.997811 autora-synthetic-1.0.1a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.001811 autora-synthetic-1.0.1a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.github/workflows/docs-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.001811 autora-synthetic-1.0.1a2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.idea/autora-synthetic.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-01 17:47:08.005811 autora-synthetic-1.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.001811 autora-synthetic-1.0.1a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   171044 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/docs/Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.001811 autora-synthetic-1.0.1a2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.001811 autora-synthetic-1.0.1a2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:47:08.005811 autora-synthetic-1.0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:07.997811 autora-synthetic-1.0.1a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:07.997811 autora-synthetic-1.0.1a2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:07.997811 autora-synthetic-1.0.1a2/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.001811 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.001811 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/abstract/template_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.005811 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/economics/
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/economics/prospect_theory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.005811 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/psychophysics/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.005811 autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-01 17:47:07.000000 autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-01 17:47:07.000000 autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:47:07.000000 autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-01 17:47:07.000000 autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 17:47:07.000000 autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:08.005811 autora-synthetic-1.0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/tests/test_bundled_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-01 17:46:53.000000 autora-synthetic-1.0.1a2/tests/test_synthetic_inventory.py
```

### Comparing `autora-synthetic-1.0.1a1/.github/workflows/python-publish.yml` & `autora-synthetic-1.0.1a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/.github/workflows/test-pytest.yml` & `autora-synthetic-1.0.1a2/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/.gitignore` & `autora-synthetic-1.0.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/.idea/autora-synthetic.iml` & `autora-synthetic-1.0.1a2/.idea/autora-synthetic.iml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/.pre-commit-config.yaml` & `autora-synthetic-1.0.1a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/CONTRIBUTING.md` & `autora-synthetic-1.0.1a2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/PKG-INFO` & `autora-synthetic-1.0.1a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: AutoRA Synthetic Experiments
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic
 Project-URL: documentation, https://autoresearch.github.io/autora-synthetic/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -16,18 +16,18 @@
 
 ## User Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
-Install the synthetic data package:
+Install the synthetic data package (as part of `autora`):
 
 ```shell
-pip install -U "autora[synthetic-data]" --pre
+pip install -U "autora" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
 python -c "
```

### Comparing `autora-synthetic-1.0.1a1/README.md` & `autora-synthetic-1.0.1a2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 ## User Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
-Install the synthetic data package:
+Install the synthetic data package (as part of `autora`):
 
 ```shell
-pip install -U "autora[synthetic-data]" --pre
+pip install -U "autora" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
 python -c "
```

### Comparing `autora-synthetic-1.0.1a1/docs/Example.ipynb` & `autora-synthetic-1.0.1a2/docs/Example.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996376811594203%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(1, \'# !pip install "autora" --pre\')], delete: [1]}}}'}*

```diff
@@ -10,15 +10,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Uncomment the following line when running on Google Colab\n",
-                "# !pip install \"autora[synthetic-data]\" --pre"
+                "# !pip install \"autora\" --pre"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Load the Weber-Fechner Law:"
```

### Comparing `autora-synthetic-1.0.1a1/docs/index.md` & `autora-synthetic-1.0.1a2/docs/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
 Install the synthetic data package:
 
 ```shell
-pip install -U "autora[synthetic-data]" --pre
+pip install -U "autora" --pre
 ```
 
 !!! success
     It is recommended to use a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
```

### Comparing `autora-synthetic-1.0.1a1/mkdocs/base.yml` & `autora-synthetic-1.0.1a2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/pyproject.toml` & `autora-synthetic-1.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/abstract/template_experiment.py` & `autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/abstract/template_experiment.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py` & `autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/economics/expected_value_theory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/economics/prospect_theory.py` & `autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/economics/prospect_theory.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py` & `autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/psychophysics/weber_fechner_law.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/src/autora/experiment_runner/synthetic/utilities.py` & `autora-synthetic-1.0.1a2/src/autora/experiment_runner/synthetic/utilities.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/PKG-INFO` & `autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-synthetic
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: AutoRA Synthetic Experiments
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-synthetic
 Project-URL: documentation, https://autoresearch.github.io/autora-synthetic/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -16,18 +16,18 @@
 
 ## User Guide
 
 You will need:
 
 - `python` 3.8 or greater: [https://www.python.org/downloads/](https://www.python.org/downloads/)
 
-Install the synthetic data package:
+Install the synthetic data package (as part of `autora`):
 
 ```shell
-pip install -U "autora[synthetic-data]" --pre
+pip install -U "autora" --pre
 ```
 
 > 💡We recommend using a `python` environment manager like `virtualenv`.
 
 Print a description of the prospect theory model by Kahneman and Tversky by running:
 ```shell
 python -c "
```

### Comparing `autora-synthetic-1.0.1a1/src/autora_synthetic.egg-info/SOURCES.txt` & `autora-synthetic-1.0.1a2/src/autora_synthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/tests/test_bundled_models.py` & `autora-synthetic-1.0.1a2/tests/test_bundled_models.py`

 * *Files identical despite different names*

### Comparing `autora-synthetic-1.0.1a1/tests/test_synthetic_inventory.py` & `autora-synthetic-1.0.1a2/tests/test_synthetic_inventory.py`

 * *Files identical despite different names*

