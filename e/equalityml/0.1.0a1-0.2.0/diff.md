# Comparing `tmp/equalityml-0.1.0a1.tar.gz` & `tmp/equalityml-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equalityml-0.1.0a1.tar", last modified: Mon Jan  2 21:25:31 2023, max compression
+gzip compressed data, was "equalityml-0.2.0.tar", max compression
```

## Comparing `equalityml-0.1.0a1.tar` & `equalityml-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,9 @@
-drwxr-xr-x   0 Granja     (501) staff       (20)        0 2023-01-02 21:25:31.019905 equalityml-0.1.0a1/
--rw-r--r--   0 Granja     (501) staff       (20)    11360 2022-12-01 17:07:39.000000 equalityml-0.1.0a1/LICENSE
--rw-r--r--   0 Granja     (501) staff       (20)    17259 2023-01-02 21:25:31.019662 equalityml-0.1.0a1/PKG-INFO
--rw-r--r--   0 Granja     (501) staff       (20)    16557 2023-01-02 21:20:22.000000 equalityml-0.1.0a1/README.md
-drwxr-xr-x   0 Granja     (501) staff       (20)        0 2023-01-02 21:25:31.006739 equalityml-0.1.0a1/equalityml/
--rw-r--r--   0 Granja     (501) staff       (20)      189 2023-01-02 21:25:03.000000 equalityml-0.1.0a1/equalityml/__init__.py
--rw-r--r--   0 Granja     (501) staff       (20)     3969 2022-12-20 11:06:33.000000 equalityml-0.1.0a1/equalityml/check_equalityml.py
--rw-r--r--   0 Granja     (501) staff       (20)    22038 2023-01-02 21:16:49.000000 equalityml-0.1.0a1/equalityml/fair.py
-drwxr-xr-x   0 Granja     (501) staff       (20)        0 2023-01-02 21:25:31.012252 equalityml-0.1.0a1/equalityml.egg-info/
--rw-r--r--   0 Granja     (501) staff       (20)    17259 2023-01-02 21:25:30.000000 equalityml-0.1.0a1/equalityml.egg-info/PKG-INFO
--rw-r--r--   0 Granja     (501) staff       (20)      633 2023-01-02 21:25:30.000000 equalityml-0.1.0a1/equalityml.egg-info/SOURCES.txt
--rw-r--r--   0 Granja     (501) staff       (20)        1 2023-01-02 21:25:30.000000 equalityml-0.1.0a1/equalityml.egg-info/dependency_links.txt
--rw-r--r--   0 Granja     (501) staff       (20)        1 2022-12-03 17:24:13.000000 equalityml-0.1.0a1/equalityml.egg-info/not-zip-safe
--rw-r--r--   0 Granja     (501) staff       (20)      165 2023-01-02 21:25:30.000000 equalityml-0.1.0a1/equalityml.egg-info/requires.txt
--rw-r--r--   0 Granja     (501) staff       (20)       17 2023-01-02 21:25:30.000000 equalityml-0.1.0a1/equalityml.egg-info/top_level.txt
--rw-r--r--   0 Granja     (501) staff       (20)       38 2023-01-02 21:25:31.019953 equalityml-0.1.0a1/setup.cfg
--rw-r--r--   0 Granja     (501) staff       (20)    17921 2023-01-02 21:22:42.000000 equalityml-0.1.0a1/setup.py
-drwxr-xr-x   0 Granja     (501) staff       (20)        0 2023-01-02 21:25:31.012546 equalityml-0.1.0a1/tests/
--rw-r--r--   0 Granja     (501) staff       (20)        0 2022-12-01 17:07:39.000000 equalityml-0.1.0a1/tests/__init__.py
--rw-r--r--   0 Granja     (501) staff       (20)     5463 2022-12-26 17:59:54.000000 equalityml-0.1.0a1/tests/test_fair.py
-drwxr-xr-x   0 Granja     (501) staff       (20)        0 2023-01-02 21:25:30.999827 equalityml-0.1.0a1/venv/
-drwxr-xr-x   0 Granja     (501) staff       (20)        0 2023-01-02 21:25:31.017648 equalityml-0.1.0a1/venv/bin/
--rw-r--r--   0 Granja     (501) staff       (20)     1200 2022-12-01 17:07:57.000000 equalityml-0.1.0a1/venv/bin/activate_this.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      632 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2html.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      754 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2html4.py
--rwxr-xr-x   0 Granja     (501) staff       (20)     1099 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2html5.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      831 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2latex.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      654 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2man.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      820 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2odt.py
--rwxr-xr-x   0 Granja     (501) staff       (20)     1758 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      639 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      675 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2s5.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      911 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      640 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rst2xml.py
--rwxr-xr-x   0 Granja     (501) staff       (20)      708 2022-12-01 17:38:08.000000 equalityml-0.1.0a1/venv/bin/rstpep2html.py
+-rw-r--r--   0        0        0    11360 2022-12-01 17:07:39.535653 equalityml-0.2.0/LICENSE
+-rw-r--r--   0        0        0    16152 2023-06-01 13:32:12.715361 equalityml-0.2.0/PyPI_README.md
+-rw-r--r--   0        0        0      292 2023-05-30 17:20:17.687439 equalityml-0.2.0/equalityml/__init__.py
+-rw-r--r--   0        0        0     7866 2023-05-26 07:56:39.859889 equalityml-0.2.0/equalityml/check_equalityml.py
+-rw-r--r--   0        0        0    40336 2023-05-30 17:17:30.606480 equalityml-0.2.0/equalityml/fair.py
+-rw-r--r--   0        0        0    19133 2023-05-09 16:37:09.878548 equalityml-0.2.0/equalityml/stats.py
+-rw-r--r--   0        0        0    28255 2023-05-09 16:37:09.878874 equalityml-0.2.0/equalityml/threshold.py
+-rw-r--r--   0        0        0     1365 2023-06-01 14:39:48.836824 equalityml-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17765 1970-01-01 00:00:00.000000 equalityml-0.2.0/PKG-INFO
```

### Comparing `equalityml-0.1.0a1/LICENSE` & `equalityml-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `equalityml-0.1.0a1/PKG-INFO` & `equalityml-0.2.0/PyPI_README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,147 +1,123 @@
-Metadata-Version: 2.1
-Name: equalityml
-Version: 0.1.0a1
-Summary: Algorithms for evaluating fairness metrics and mitigating unfairness in supervised machine learning
-Home-page: https://equalityai.com
-Author: Ben Brintz, Mark Zhang, James Ng, Janice Davis, Jared Hansen, Ji won Chang, João Granja, Rizwan Muhammad
-Author-email: support@equalityai.com
-Project-URL: Website, https://equalityai.com
-Project-URL: Manifesto, https://equalityai.com/community/#manifesto
-Project-URL: GitHub, https://github.com/EqualityAI/EqualityML
-Project-URL: Slack, https://equalityai.slack.com/ssb/redirect#/shared-invite/email
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: doc
-License-File: LICENSE
-
-
 [![Continuous Integration](https://github.com/EqualityAI/EqualityML/actions/workflows/ci.yml/badge.svg)](https://github.com/EqualityAI/EqualityML/actions/workflows/ci.yml)
 [![License](https://img.shields.io/github/license/EqualityAI/EqualityML.svg?color=blue)](https://github.com/EqualityAI/EqualityML/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](https://github.com/EqualityAI/EqualityML/blob/main/CODE_OF_CONDUCT.md)
 <!---
 [![Documentation](https://readthedocs.org/projects/aif360/badge/?version=latest)](http://aif360.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/equalityml.svg)](https://badge.fury.io/py/equalityml)
-[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/equalityml)](https://cran.r-project.org/package=equalityml)
+[![CRAN_Status_Badge](http://www.r-pkg.org/badges/version/equalityml)](https://cran.r-project.org/package=equalityml)
 --->
 # Equality AI `EqualityML`
 
 ### Let's end algorithmic bias together!
 
-[Equality AI (EAI)](https://equalityai.com/) is a public-benefit corporation dedicated to providing developers with 
-evidence-based tools to end algorithmic bias. Our tools are built by developers for developers. So, we know that 
-developers want their models to be fair, but we also understand that bias is <b> difficult and intimidating.</b> 
+[Equality AI (EAI)](https://equalityai.com/) is a public-benefit corporation dedicated to providing developers with
+evidence-based tools to end algorithmic bias. Our tools are built by developers for developers. So, we know that
+developers want their models to be fair, but we also understand that bias is <b> difficult and intimidating.</b>
 
-The EAI `EqualityML` repository provides tools and guidance on how to include fairness and bias mitigation methods to 
-model fitting so as to safeguard the people on the receiving end of our models from bias. 
+The EAI `EqualityML` repository provides tools and guidance on how to include fairness and bias mitigation methods to
+model fitting so as to safeguard the people on the receiving end of our models from bias.
 
 If you like what we're doing, give us a star and join our [EAI Manifesto!](https://equalityai.com/community/#manifesto)!</br>
 
->We have extented `EqualityML` to include other aspects of Responsible AI (see full framework <b>Figure 1.</b>) and 
-collaboration features to create our Beta MLOps Developer Studio. <b>Become a Beta user by going to our 
+>We have extented `EqualityML` to include other aspects of Responsible AI (see full framework <b>Figure 1.</b>) and
+collaboration features to create our Beta MLOps Developer Studio. <b>Become a Beta user by going to our
 [website!](https://equalityai.com/)</b>
 
 ![](https://github.com/EqualityAI/EqualityML/blob/main/img/framework.png?raw=true)
 <sub><b>Figure 1:</b> Full Responsible AI Framework.</sub>
 
 ## Introduction
-Incorporating bias mitigation methods and fairness metrics into the traditional end-to-end MLOps is called 
-fairness-based machine learning (ML) or fair machine learning. However, fair ML comes with its own challenges. 
-We assembled a diverse team of statisticians and ML experts to provide evidence-based guidance on fairness metrics 
+Incorporating bias mitigation methods and fairness metrics into the traditional end-to-end MLOps is called
+fairness-based machine learning (ML) or fair machine learning. However, fair ML comes with its own challenges.
+We assembled a diverse team of statisticians and ML experts to provide evidence-based guidance on fairness metrics
 use/selection and validated code to properly run bias mitigation methods.
 
 <details>
   <summary> Click to read our findings: </summary>
-  
+
 #### Fairness Metric
 * Statistical measure of the output of a machine learning model based a mathematical definition of fairness.
 
 > [Fairness Metric Guide:](https://github.com/EqualityAI/EqualityML/raw/main/Fairness%20Metrics%20User%20Manual.pdf)
-We have combined fairness metrics and bias mitigation into a unified syntax.</br><sub> Statistical Parity | 
-Conditional Statistical Parity | Negative Predictive Parity | Equal Opportunity | Balance for Positive Class | 
-Predictive Parity | Well Calibration | Calibration | Conditional Use Accuracy | Predictive Equality | Balance for 
+We have combined fairness metrics and bias mitigation into a unified syntax.</br><sub> Statistical Parity |
+Conditional Statistical Parity | Negative Predictive Parity | Equal Opportunity | Balance for Positive Class |
+Predictive Parity | Well Calibration | Calibration | Conditional Use Accuracy | Predictive Equality | Balance for
 Negative Class | Equalized Odds | Overall Balance
 </sub>
 
 #### Bias Mitigation
-* Methods or algorithms applied to a machine learning dataset or model to improve the fairness of the model output. 
-Many mitigation methods have been proposed in the literature, which can be broadly classified into the application of 
-a mitigation method on the data set (pre-processing), in the model fitting (in-processing), and to the model 
+* Methods or algorithms applied to a machine learning dataset or model to improve the fairness of the model output.
+Many mitigation methods have been proposed in the literature, which can be broadly classified into the application of
+a mitigation method on the data set (pre-processing), in the model fitting (in-processing), and to the model
 predictions (post-processing).
 
 > [Bias Mitigation Guide:](https://github.com/EqualityAI/EqualityML/blob/main/Fairness%20Metrics%20User%20Manual.pdf)</br>
-<sub> Resampling | Reweighting | Disparate Impact Remover | Correlation Remover 
+<sub> Resampling | Reweighting | Disparate Impact Remover | Correlation Remover
 </sub>
 
 ![](https://github.com/EqualityAI/EqualityML/blob/main/img/pre_in_post_nw.png?raw=true)
 <sub><b>Figure 2:</b> Bias mitigation can be performed in the pre-processing, in-processing, and post-processing of a model.</sub>
 <br>
 
 > Need a specific metric or method? [Just let us know!](https://equalityai.slack.com/join/shared_invite/zt-1claqpebo-MnGnGoqCM9Do~40HqbSaww#/shared-invite/email)
 
 #### Potential Uses
 
 * Bias mitigation methods are employed to address bias in data and/or machine learning models and fairness metrics are needed to mathematically represent the fairness or bias levels of a ML model.
-  
+
 | Use                                                         | Description                                                                                                                                                                                                    |
 |:-------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | As a metric                                      | Quantify a measure of fairness (a.k.a a fairness metric) targeting a bias                                                                                                                                      |
 | Evaluate fairness                                            | Fairness metrics can be used to mathematically represent the fairness levels of a ML model. This can also be used to monitor a model.                                                                          |
 | Create parity on fairness                                    | Unlike model performance metrics (e.g., loss, accuracy, etc.), fairness metrics affect your final model selection by creating parity (i.e., equality) on appropriate fairness metrics before model deployment. |
 | Select most fair model                                       | Balance fairness with performance metrics when selecting the final model.                                                                                                                                      |
 | Apply methods to improve the fairness & performance tradeoff | Methods to improve the fairness by applying a.k.a bias mitigation methods                                                                                                                                      |
 
 <sub><b>Table 1:</b> The potential uses for fairness metrics and bias mitigation methods.
 </sub>
 
-<b>Note:</b> Parity is achieved when a fairness metric (such as the percent of positive predictions) have the same value across all levels of a sensitive attribute.  <i>Sensitive attributes</i> are attributes such as race, gender, age, and other patient attributes that are of primary concern when it comes to fairness, and are typically protected by law. 
+<b>Note:</b> Parity is achieved when a fairness metric (such as the percent of positive predictions) have the same value across all levels of a sensitive attribute.  <i>Sensitive attributes</i> are attributes such as race, gender, age, and other patient attributes that are of primary concern when it comes to fairness, and are typically protected by law.
   <br></br>
 
 Through these steps we <b>safeguard against bias</b> by:
 > 1. Creating metrics targeting sources of bias to balance alongside our performance metrics in evaluation, model selection, and monitoring.
 > 2. Applying bias mitigation methods to improve fairness without compromising performance.
  <br></br>
-  
+
 </details>
 
 
 ## EAI `EqualityML` Workflow
-We have conducted extensive literature review and theoretical analysis on dozens of fairness metrics and mitigation methods. Theoretical properties of those fairness mitigation methods were analyzed to determine their suitability under various conditions to create our framework for a pre-processing workflow. 
+We have conducted extensive literature review and theoretical analysis on dozens of fairness metrics and mitigation methods. Theoretical properties of those fairness mitigation methods were analyzed to determine their suitability under various conditions to create our framework for a pre-processing workflow.
 
 | Pre-processing Workflow                                                  | Tool or Guidance provided                                                                                                                                                                                                               |
 |:-------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | 1. Select Fairness Metric                                                | Use our [Fairness Metric Selection Questionnaire & Tree](https://github.com/EqualityAI/EqualityML/blob/main/Equality%20AI%20Fairness%20Metric%20Selection%20Questionnaire%20%26%20Tree.pdf) to determine appropriate fairness metric(s) |
 | 2. Data Preparation                                                      ||
 | 3. Fit Prediction Model                                                  ||
 | 4. Compute Model Results and Evaluate Fairness Metric                    | Use `EqualityML` method `fairness_metric` to evaluate the fairness of a model                                                                                                                                                           |
 | 5. Run Bias Mitigation                                                   | Use `EqualityML` method `bias_mitigation` to run various bias mitigation methods on your dataset                                                                                                                                        |
 | 6. Compute Model Results and Fairness Metric After Mitigation            | `fairness_metric` `bias_mitigation`                                                                                                                                                                                                     |
 | 7. Compare Model Results and Fairness Metric Before and After Mitigation | `fairness_metric` `bias_mitigation`                                                                                                                                                                                                     |
 
 <sub><b>Table 2:</b> The Equality AI recommended pre-processing workflow with tools and guidance made available per step.
 </sub> </br>
 
-We recommend assessing the fairness of the same ML model after bias mitigation is applied. By comparing the predictions before and 
-after mitigation, we will be able to assess whether and to what extent the fairness can be improved. Furthermore, 
+We recommend assessing the fairness of the same ML model after bias mitigation is applied. By comparing the predictions before and
+after mitigation, we will be able to assess whether and to what extent the fairness can be improved. Furthermore,
 the trade-offs between the accuracy and fairness of the machine learning model will be examined.
 
 > In-processing and Post-processing are still under development. Do you need this now? [Let us know!](https://equalityai.slack.com/join/shared_invite/zt-1claqpebo-MnGnGoqCM9Do~40HqbSaww#/shared-invite/email)
 
 ## Guidance on selecting Fairness Metrics
-To make fairness metric selection easy we have provided a few essential questions you must answer to identify the 
+To make fairness metric selection easy we have provided a few essential questions you must answer to identify the
 appropriate fairness metric for your use case. [Click here for the questionnaire](https://github.com/EqualityAI/EqualityML/blob/main/Equality%20AI%20Fairness%20Metric%20Selection%20Questionnaire%20%26%20Tree.pdf). Complete the answers to this questionnaire, then refer to the scoring guide to map your inputs to the desired metrics.
 
-After identifying the important fairness criteria, we recommend you attempt to use multiple bias mitigation strategies 
+After identifying the important fairness criteria, we recommend you attempt to use multiple bias mitigation strategies
 to try to optimize the efficiency-fairness tradeoff.</br>
 
 ## `EqualityML` Installation
 
 ## Python
 The `EqualityML` python package can be installed from [PyPI](https://pypi.org/project/equalityml/).
 
@@ -152,27 +128,27 @@
 ### Manual Installation
 Clone the last version of this repository:
 ```bash
 https://github.com/EqualityAI/EqualityML.git
 ```
 In the root directory of the project run the command:
 ```bash
-pip install -e '.[all]'
+poetry install
 ```
 
 ### Package Testing
 To run the bunch of tests over the EqualityML package, dependencies shall be first installed before calling pytest.
 
 ```sh
-pip install -e '.[tests]'
+poetry install --with test
 pytest tests
 ```
 ### Quick Tour
 
-Check out the example below to see how EqualityML can be used to assess fairness metrics and mitigate unwanted bias in 
+Check out the example below to see how EqualityML can be used to assess fairness metrics and mitigate unwanted bias in
 the dataset.
 
 ```python
 from sklearn.linear_model import LogisticRegression
 from equalityml import FAIR
 import numpy as np
 import pandas as pd
@@ -181,40 +157,40 @@
 random_col = np.random.normal(size=30)
 sex_col = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
            0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
 weight_col = [80, 75, 70, 65, 60, 85, 70, 75, 70, 70, 70, 80, 70, 70, 70, 80, 75, 70, 65, 70,
               70, 75, 80, 75, 75, 70, 65, 70, 75, 65]
 target_col = [1, 1, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 0, 1, 0, 1, 1, 0, 1, 1,
               0, 1, 0, 1, 1, 0, 0, 1, 1, 0]
-training_data = pd.DataFrame({"random": random_col, "sex": sex_col, "weight": weight_col, 
+training_data = pd.DataFrame({"random": random_col, "sex": sex_col, "weight": weight_col,
                               "Y": target_col})
-    
+
 # Train a machine learning model (for example LogisticRegression)
 ml_model = LogisticRegression()
 ml_model.fit(training_data.drop(columns="Y"), training_data["Y"])
 
 # Instantiate a FAIR object
-fair_obj = FAIR(ml_model=ml_model, 
+fair_obj = FAIR(ml_model=ml_model,
                 training_data=training_data,
                 target_variable="Y",
-                protected_variable="sex", 
+                protected_variable="sex",
                 privileged_class=1)
 
 # Evaluate a fairness metric (for example statistical parity ratio)
 metric_name = 'statistical_parity_ratio'
 fairness_metric = fair_obj.fairness_metric(metric_name)
 
-# In case the model is unfair in terms of checked fairness metric (value is not close to 1), 
-# EqualityML provides a range of methods to try to mitigate bias in Machine Learning models. 
+# In case the model is unfair in terms of checked fairness metric (value is not close to 1),
+# EqualityML provides a range of methods to try to mitigate bias in Machine Learning models.
 # For example, we can use 'resampling' to perform mitigation on training dataset.
 
 mitigation_method = "resampling"
 mitigation_result = fair_obj.bias_mitigation(mitigation_method)
 
-# Now we can re-train the machine learning model based on that mitigated data and 
+# Now we can re-train the machine learning model based on that mitigated data and
 # evaluate again the fairness metric
 mitigated_data = mitigation_result['training_data']
 ml_model.fit(mitigated_data.drop(columns="Y"), mitigated_data["Y"])
 
 fair_obj.update_classifier(ml_model)
 new_fairness_metric = fair_obj.fairness_metric(metric_name)
 
@@ -234,31 +210,30 @@
 ```
 install.packages("equalityml")
 ```
 or developer version from GitHub:
 ```
 devtools::install_github("EqualityAI/equalityml/equalityml-r")
 ```
-For more details regarding the R package, please check [here](https://github.com/EqualityAI/EqualityML/tree/main/equalityml-r). 
+For more details regarding the R package, please check [here](https://github.com/EqualityAI/EqualityML/tree/main/equalityml-r).
 
 
 ## Responsible AI Takes a Community
-The connections and trade-offs between fairness, explainability, and privacy require a holistic approach to Responsible 
-AI development in the machine learning community. We are starting with the principle of fairness and working towards a 
-solution that incorporates multiple aspects of Responsible AI for data scientists and healthcare professionals. We have 
-much more in the works, and we want to know—what do you need? Do you have a Responsible AI challenge you need to solve? 
+The connections and trade-offs between fairness, explainability, and privacy require a holistic approach to Responsible
+AI development in the machine learning community. We are starting with the principle of fairness and working towards a
+solution that incorporates multiple aspects of Responsible AI for data scientists and healthcare professionals. We have
+much more in the works, and we want to know—what do you need? Do you have a Responsible AI challenge you need to solve?
 [Drop us a line and let’s see how we can help!](https://equalityai.slack.com/join/shared_invite/zt-1claqpebo-MnGnGoqCM9Do~40HqbSaww#/shared-invite/email)
 
 ## Contributing to the project
 Equality AI uses both GitHub and Slack to manage our open source community. To participate:
 
 1. Join the Slack community (https://equalityai.com/slack)
     + Introduce yourself in the #Introductions channel. We're all friendly people!
-2. Check out the [CONTRIBUTING](https://github.com/EqualityAI/EqualityML/blob/main/CONTRIBUTING.md) file to learn how 
+2. Check out the [CONTRIBUTING](https://github.com/EqualityAI/EqualityML/blob/main/CONTRIBUTING.md) file to learn how
 to contribute to our project, report bugs, or make feature requests.
 3. Try out the [`EqualityML`](https://github.com/EqualityAI/EqualityML)
     + Hit the top right "star" button on GitHub to show your love!
-    + Follow the recipe above to use the code. 
-4. Provide feedback on your experience using the [GitHub discussions](https://github.com/EqualityAI/EqualityML/discussions) 
+    + Follow the recipe above to use the code.
+4. Provide feedback on your experience using the [GitHub discussions](https://github.com/EqualityAI/EqualityML/discussions)
 or the [Slack #support](https://equalityai.slack.com/archives/C03HF7G4N0Y) channel
     + For any questions or problems, send a message on Slack, or send an email to support@equalityai.com.
-
```

### Comparing `equalityml-0.1.0a1/README.md` & `equalityml-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,159 @@
-<img src="img/natural-bird.png"  align="left" alt="EqualityAI Logo" width="100"/>
+Metadata-Version: 2.1
+Name: equalityml
+Version: 0.2.0
+Summary: Algorithms for evaluating fairness metrics and mitigating unfairness in supervised machine learning
+Home-page: https://equalityai.com
+License: Apache-2.0
+Author: Ben Brintz, Mark Zhang, James Ng, Janice Davis, Jared Hansen, Ji won Chang, João Granja, Rizwan Muhammad
+Author-email: support@equalityai.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: BlackBoxAuditing (>=0.1.54,<0.2.0)
+Requires-Dist: aif360-fork2 (==0.5.0)
+Requires-Dist: dalex (>=1.5.0,<2.0.0)
+Requires-Dist: fairlearn (>=0.7.0,<0.8.0)
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
+Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: pandas (>=1.2.5,<2.0.0)
+Requires-Dist: scikit-learn (>=1.0,<2.0)
+Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: GitHub, https://github.com/EqualityAI/EqualityML
+Project-URL: Manifesto, https://equalityai.com/community/#manifesto
+Project-URL: Slack, https://equalityai.slack.com/ssb/redirect#/shared-invite/email
+Project-URL: Website, https://equalityai.com
+Description-Content-Type: text/markdown
 
 [![Continuous Integration](https://github.com/EqualityAI/EqualityML/actions/workflows/ci.yml/badge.svg)](https://github.com/EqualityAI/EqualityML/actions/workflows/ci.yml)
 [![License](https://img.shields.io/github/license/EqualityAI/EqualityML.svg?color=blue)](https://github.com/EqualityAI/EqualityML/blob/main/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](https://github.com/EqualityAI/EqualityML/blob/main/CODE_OF_CONDUCT.md)
 <!---
 [![Documentation](https://readthedocs.org/projects/aif360/badge/?version=latest)](http://aif360.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/equalityml.svg)](https://badge.fury.io/py/equalityml)
-[![CRAN\_Status\_Badge](http://www.r-pkg.org/badges/version/equalityml)](https://cran.r-project.org/package=equalityml)
+[![CRAN_Status_Badge](http://www.r-pkg.org/badges/version/equalityml)](https://cran.r-project.org/package=equalityml)
 --->
 # Equality AI `EqualityML`
 
-### Let's end algorithmic bias together! 
+### Let's end algorithmic bias together!
 
-[Equality AI (EAI)](https://equalityai.com/) is a public-benefit corporation dedicated to providing developers with evidence-based tools to end algorithmic bias. Our tools are built by developers for developers. So, we know that developers want their models to be fair, but we also understand that bias is <b> difficult and intimidating.</b> 
+[Equality AI (EAI)](https://equalityai.com/) is a public-benefit corporation dedicated to providing developers with
+evidence-based tools to end algorithmic bias. Our tools are built by developers for developers. So, we know that
+developers want their models to be fair, but we also understand that bias is <b> difficult and intimidating.</b>
 
-The EAI `EqualityML` repository provides tools and guidance on how to include fairness and bias mitigation methods to model fitting so as to safeguard the people on the receiving end of our models from bias. 
+The EAI `EqualityML` repository provides tools and guidance on how to include fairness and bias mitigation methods to
+model fitting so as to safeguard the people on the receiving end of our models from bias.
 
-If you like what we're doing, give us a :star: and join our [EAI Manifesto!](https://equalityai.com/community/#manifesto)!</br>
-<img src="img/star.png" align="center" alt="" width="400" /><br></br>
+If you like what we're doing, give us a star and join our [EAI Manifesto!](https://equalityai.com/community/#manifesto)!</br>
 
+>We have extented `EqualityML` to include other aspects of Responsible AI (see full framework <b>Figure 1.</b>) and
+collaboration features to create our Beta MLOps Developer Studio. <b>Become a Beta user by going to our
+[website!](https://equalityai.com/)</b>
 
->We have extented `EqualityML` to include other aspects of Responsible AI (see full framework <b>Figure 1.</b>) and collaboration features to create our Beta MLOps Developer Studio. <b>Become a Beta user by going to our [website!](https://equalityai.com/)</b>
-
-<center>
-<img src="img/framework.png" align="center" alt="" width="500" />
+![](https://github.com/EqualityAI/EqualityML/blob/main/img/framework.png?raw=true)
 <sub><b>Figure 1:</b> Full Responsible AI Framework.</sub>
-</center>
 
 ## Introduction
-Incorporating bias mitigation methods and fairness metrics into the traditional end-to-end MLOps is called fairness-based machine learning (ML) or fair machine learning. However, fair ML comes with its own challenges. We assembled a diverse team of statisticians and ML experts to provide evidence-based guidance on fairness metrics use/selection and validated code to properly run bias mitigation methods.
+Incorporating bias mitigation methods and fairness metrics into the traditional end-to-end MLOps is called
+fairness-based machine learning (ML) or fair machine learning. However, fair ML comes with its own challenges.
+We assembled a diverse team of statisticians and ML experts to provide evidence-based guidance on fairness metrics
+use/selection and validated code to properly run bias mitigation methods.
 
 <details>
   <summary> Click to read our findings: </summary>
-  
+
 #### Fairness Metric
 * Statistical measure of the output of a machine learning model based a mathematical definition of fairness.
 
 > [Fairness Metric Guide:](https://github.com/EqualityAI/EqualityML/raw/main/Fairness%20Metrics%20User%20Manual.pdf)
-We have combined fairness metrics and bias mitigation into a unified syntax.</br><sub> Statistical Parity | Conditional Statistical Parity | Negative Predictive Parity | Equal Opportunity | Balance for Positive Class | Predictive Parity | Well Calibration | Calibration | Conditional Use Accuracy | Predictive Equality | Balance for Negative Class | Equalized Odds | Overall Balance
+We have combined fairness metrics and bias mitigation into a unified syntax.</br><sub> Statistical Parity |
+Conditional Statistical Parity | Negative Predictive Parity | Equal Opportunity | Balance for Positive Class |
+Predictive Parity | Well Calibration | Calibration | Conditional Use Accuracy | Predictive Equality | Balance for
+Negative Class | Equalized Odds | Overall Balance
 </sub>
 
 #### Bias Mitigation
-* Methods or algorithms applied to a machine learning dataset or model to improve the fairness of the model output. Many mitigation methods have been proposed in the literature, which can be broadly classified into the application of a mitigation method on the data set (pre-processing), in the model fitting (in-processing), and to the model predictions (post-processing).
+* Methods or algorithms applied to a machine learning dataset or model to improve the fairness of the model output.
+Many mitigation methods have been proposed in the literature, which can be broadly classified into the application of
+a mitigation method on the data set (pre-processing), in the model fitting (in-processing), and to the model
+predictions (post-processing).
 
 > [Bias Mitigation Guide:](https://github.com/EqualityAI/EqualityML/blob/main/Fairness%20Metrics%20User%20Manual.pdf)</br>
-<sub> Resampling | Reweighting | Disparate Impact Remover | Correlation Remover 
+<sub> Resampling | Reweighting | Disparate Impact Remover | Correlation Remover
 </sub>
 
-<img src="img/pre_in_post_nw.png" align="center" alt="" width="350" />
+![](https://github.com/EqualityAI/EqualityML/blob/main/img/pre_in_post_nw.png?raw=true)
 <sub><b>Figure 2:</b> Bias mitigation can be performed in the pre-processing, in-processing, and post-processing of a model.</sub>
 <br>
 
 > Need a specific metric or method? [Just let us know!](https://equalityai.slack.com/join/shared_invite/zt-1claqpebo-MnGnGoqCM9Do~40HqbSaww#/shared-invite/email)
 
 #### Potential Uses
 
 * Bias mitigation methods are employed to address bias in data and/or machine learning models and fairness metrics are needed to mathematically represent the fairness or bias levels of a ML model.
-  
+
 | Use                                                         | Description                                                                                                                                                                                                    |
 |:-------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | As a metric                                      | Quantify a measure of fairness (a.k.a a fairness metric) targeting a bias                                                                                                                                      |
 | Evaluate fairness                                            | Fairness metrics can be used to mathematically represent the fairness levels of a ML model. This can also be used to monitor a model.                                                                          |
 | Create parity on fairness                                    | Unlike model performance metrics (e.g., loss, accuracy, etc.), fairness metrics affect your final model selection by creating parity (i.e., equality) on appropriate fairness metrics before model deployment. |
 | Select most fair model                                       | Balance fairness with performance metrics when selecting the final model.                                                                                                                                      |
 | Apply methods to improve the fairness & performance tradeoff | Methods to improve the fairness by applying a.k.a bias mitigation methods                                                                                                                                      |
 
 <sub><b>Table 1:</b> The potential uses for fairness metrics and bias mitigation methods.
 </sub>
 
-<b>Note:</b> Parity is achieved when a fairness metric (such as the percent of positive predictions) have the same value across all levels of a sensitive attribute.  <i>Sensitive attributes</i> are attributes such as race, gender, age, and other patient attributes that are of primary concern when it comes to fairness, and are typically protected by law. 
+<b>Note:</b> Parity is achieved when a fairness metric (such as the percent of positive predictions) have the same value across all levels of a sensitive attribute.  <i>Sensitive attributes</i> are attributes such as race, gender, age, and other patient attributes that are of primary concern when it comes to fairness, and are typically protected by law.
   <br></br>
 
 Through these steps we <b>safeguard against bias</b> by:
 > 1. Creating metrics targeting sources of bias to balance alongside our performance metrics in evaluation, model selection, and monitoring.
 > 2. Applying bias mitigation methods to improve fairness without compromising performance.
  <br></br>
-  
+
 </details>
 
 
 ## EAI `EqualityML` Workflow
-We have conducted extensive literature review and theoretical analysis on dozens of fairness metrics and mitigation methods. Theoretical properties of those fairness mitigation methods were analyzed to determine their suitability under various conditions to create our framework for a pre-processing workflow. 
+We have conducted extensive literature review and theoretical analysis on dozens of fairness metrics and mitigation methods. Theoretical properties of those fairness mitigation methods were analyzed to determine their suitability under various conditions to create our framework for a pre-processing workflow.
 
 | Pre-processing Workflow                                                  | Tool or Guidance provided                                                                                                                                                                                                               |
 |:-------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | 1. Select Fairness Metric                                                | Use our [Fairness Metric Selection Questionnaire & Tree](https://github.com/EqualityAI/EqualityML/blob/main/Equality%20AI%20Fairness%20Metric%20Selection%20Questionnaire%20%26%20Tree.pdf) to determine appropriate fairness metric(s) |
 | 2. Data Preparation                                                      ||
 | 3. Fit Prediction Model                                                  ||
 | 4. Compute Model Results and Evaluate Fairness Metric                    | Use `EqualityML` method `fairness_metric` to evaluate the fairness of a model                                                                                                                                                           |
 | 5. Run Bias Mitigation                                                   | Use `EqualityML` method `bias_mitigation` to run various bias mitigation methods on your dataset                                                                                                                                        |
 | 6. Compute Model Results and Fairness Metric After Mitigation            | `fairness_metric` `bias_mitigation`                                                                                                                                                                                                     |
 | 7. Compare Model Results and Fairness Metric Before and After Mitigation | `fairness_metric` `bias_mitigation`                                                                                                                                                                                                     |
 
 <sub><b>Table 2:</b> The Equality AI recommended pre-processing workflow with tools and guidance made available per step.
 </sub> </br>
 
-We recommend assessing the fairness of the same ML model after bias mitigation is applied. By comparing the predictions before and after mitigation, we will be able to assess whether and to what extent the fairness can be improved. Furthermore, the trade-offs between the accuracy and fairness of the machine learning model will be examined.
+We recommend assessing the fairness of the same ML model after bias mitigation is applied. By comparing the predictions before and
+after mitigation, we will be able to assess whether and to what extent the fairness can be improved. Furthermore,
+the trade-offs between the accuracy and fairness of the machine learning model will be examined.
 
 > In-processing and Post-processing are still under development. Do you need this now? [Let us know!](https://equalityai.slack.com/join/shared_invite/zt-1claqpebo-MnGnGoqCM9Do~40HqbSaww#/shared-invite/email)
 
 ## Guidance on selecting Fairness Metrics
-To make fairness metric selection easy we have provided a few essential questions you must answer to identify the appropriate fairness metric for your use case. [Click here for the questionnaire](https://github.com/EqualityAI/EqualityML/blob/main/Equality%20AI%20Fairness%20Metric%20Selection%20Questionnaire%20%26%20Tree.pdf). Complete the answers to this questionnaire, then refer to the scoring guide to map your inputs to the desired metrics.
+To make fairness metric selection easy we have provided a few essential questions you must answer to identify the
+appropriate fairness metric for your use case. [Click here for the questionnaire](https://github.com/EqualityAI/EqualityML/blob/main/Equality%20AI%20Fairness%20Metric%20Selection%20Questionnaire%20%26%20Tree.pdf). Complete the answers to this questionnaire, then refer to the scoring guide to map your inputs to the desired metrics.
 
-<img src="img/fairnesstree.png" align="center" alt="" width="800"/></br>
-<sub><b>Figure 3:</b> Tree representation of questionnaire.</sub></br>
-
-After identifying the important fairness criteria, we recommend you attempt to use multiple bias mitigation strategies to try to optimize the efficiency-fairness tradeoff.</br>
+After identifying the important fairness criteria, we recommend you attempt to use multiple bias mitigation strategies
+to try to optimize the efficiency-fairness tradeoff.</br>
 
 ## `EqualityML` Installation
 
 ## Python
 The `EqualityML` python package can be installed from [PyPI](https://pypi.org/project/equalityml/).
 
 ```bash
@@ -119,27 +163,27 @@
 ### Manual Installation
 Clone the last version of this repository:
 ```bash
 https://github.com/EqualityAI/EqualityML.git
 ```
 In the root directory of the project run the command:
 ```bash
-pip install -e '.[all]'
+poetry install
 ```
 
 ### Package Testing
 To run the bunch of tests over the EqualityML package, dependencies shall be first installed before calling pytest.
 
 ```sh
-pip install -e '.[tests]'
+poetry install --with test
 pytest tests
 ```
 ### Quick Tour
 
-Check out the example below to see how EqualityML can be used to assess fairness metrics and mitigate unwanted bias in 
+Check out the example below to see how EqualityML can be used to assess fairness metrics and mitigate unwanted bias in
 the dataset.
 
 ```python
 from sklearn.linear_model import LogisticRegression
 from equalityml import FAIR
 import numpy as np
 import pandas as pd
@@ -148,40 +192,40 @@
 random_col = np.random.normal(size=30)
 sex_col = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1,
            0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
 weight_col = [80, 75, 70, 65, 60, 85, 70, 75, 70, 70, 70, 80, 70, 70, 70, 80, 75, 70, 65, 70,
               70, 75, 80, 75, 75, 70, 65, 70, 75, 65]
 target_col = [1, 1, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 0, 1, 0, 1, 1, 0, 1, 1,
               0, 1, 0, 1, 1, 0, 0, 1, 1, 0]
-training_data = pd.DataFrame({"random": random_col, "sex": sex_col, "weight": weight_col, 
+training_data = pd.DataFrame({"random": random_col, "sex": sex_col, "weight": weight_col,
                               "Y": target_col})
-    
+
 # Train a machine learning model (for example LogisticRegression)
 ml_model = LogisticRegression()
 ml_model.fit(training_data.drop(columns="Y"), training_data["Y"])
 
 # Instantiate a FAIR object
-fair_obj = FAIR(ml_model=ml_model, 
+fair_obj = FAIR(ml_model=ml_model,
                 training_data=training_data,
                 target_variable="Y",
-                protected_variable="sex", 
+                protected_variable="sex",
                 privileged_class=1)
 
 # Evaluate a fairness metric (for example statistical parity ratio)
 metric_name = 'statistical_parity_ratio'
 fairness_metric = fair_obj.fairness_metric(metric_name)
 
-# In case the model is unfair in terms of checked fairness metric (value is not close to 1), 
-# EqualityML provides a range of methods to try to mitigate bias in Machine Learning models. 
+# In case the model is unfair in terms of checked fairness metric (value is not close to 1),
+# EqualityML provides a range of methods to try to mitigate bias in Machine Learning models.
 # For example, we can use 'resampling' to perform mitigation on training dataset.
 
 mitigation_method = "resampling"
 mitigation_result = fair_obj.bias_mitigation(mitigation_method)
 
-# Now we can re-train the machine learning model based on that mitigated data and 
+# Now we can re-train the machine learning model based on that mitigated data and
 # evaluate again the fairness metric
 mitigated_data = mitigation_result['training_data']
 ml_model.fit(mitigated_data.drop(columns="Y"), mitigated_data["Y"])
 
 fair_obj.update_classifier(ml_model)
 new_fairness_metric = fair_obj.fairness_metric(metric_name)
 
@@ -201,26 +245,31 @@
 ```
 install.packages("equalityml")
 ```
 or developer version from GitHub:
 ```
 devtools::install_github("EqualityAI/equalityml/equalityml-r")
 ```
-For more details regarding the R package, please check [here](https://github.com/EqualityAI/EqualityML/tree/main/equalityml-r). 
+For more details regarding the R package, please check [here](https://github.com/EqualityAI/EqualityML/tree/main/equalityml-r).
 
 
 ## Responsible AI Takes a Community
-The connections and trade-offs between fairness, explainability, and privacy require a holistic approach to Responsible AI development in the machine learning community. We are starting with the principle of fairness and working towards a solution that incorporates multiple aspects of Responsible AI for data scientists and healthcare professionals. We have much more in the works, and we want to know—what do you need? Do you have a Responsible AI challenge you need to solve? [Drop us a line and let’s see how we can help!](https://equalityai.slack.com/join/shared_invite/zt-1claqpebo-MnGnGoqCM9Do~40HqbSaww#/shared-invite/email)
-
-<img src="img/color logo only.PNG" align="left" alt="EqualityAI Logo" width="50"/>
+The connections and trade-offs between fairness, explainability, and privacy require a holistic approach to Responsible
+AI development in the machine learning community. We are starting with the principle of fairness and working towards a
+solution that incorporates multiple aspects of Responsible AI for data scientists and healthcare professionals. We have
+much more in the works, and we want to know—what do you need? Do you have a Responsible AI challenge you need to solve?
+[Drop us a line and let’s see how we can help!](https://equalityai.slack.com/join/shared_invite/zt-1claqpebo-MnGnGoqCM9Do~40HqbSaww#/shared-invite/email)
 
 ## Contributing to the project
 Equality AI uses both GitHub and Slack to manage our open source community. To participate:
 
 1. Join the Slack community (https://equalityai.com/slack)
     + Introduce yourself in the #Introductions channel. We're all friendly people!
-2. Check out the [CONTRIBUTING](https://github.com/EqualityAI/EqualityML/blob/main/CONTRIBUTING.md) file to learn how to contribute to our project, report bugs, or make feature requests.
+2. Check out the [CONTRIBUTING](https://github.com/EqualityAI/EqualityML/blob/main/CONTRIBUTING.md) file to learn how
+to contribute to our project, report bugs, or make feature requests.
 3. Try out the [`EqualityML`](https://github.com/EqualityAI/EqualityML)
     + Hit the top right "star" button on GitHub to show your love!
-    + Follow the recipe above to use the code. 
-4. Provide feedback on your experience using the [GitHub discussions](https://github.com/EqualityAI/EqualityML/discussions) or the [Slack #support](https://equalityai.slack.com/archives/C03HF7G4N0Y) channel
+    + Follow the recipe above to use the code.
+4. Provide feedback on your experience using the [GitHub discussions](https://github.com/EqualityAI/EqualityML/discussions)
+or the [Slack #support](https://equalityai.slack.com/archives/C03HF7G4N0Y) channel
     + For any questions or problems, send a message on Slack, or send an email to support@equalityai.com.
+
```

