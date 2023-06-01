# Comparing `tmp/gwsci-pastro-0.0.3.tar.gz` & `tmp/gwsci-pastro-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwsci-pastro-0.0.3.tar", last modified: Thu Oct 27 16:01:31 2022, max compression
+gzip compressed data, was "gwsci-pastro-1.0.0.tar", last modified: Thu Jun  1 03:44:55 2023, max compression
```

## Comparing `gwsci-pastro-0.0.3.tar` & `gwsci-pastro-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 victoria   (501) staff       (20)        0 2022-10-27 16:01:31.925931 gwsci-pastro-0.0.3/
--rw-r--r--   0 victoria   (501) staff       (20)      683 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/LICENSE
--rw-r--r--   0 victoria   (501) staff       (20)     5829 2022-10-27 16:01:31.925777 gwsci-pastro-0.0.3/PKG-INFO
--rw-r--r--   0 victoria   (501) staff       (20)     5260 2022-10-27 15:59:13.000000 gwsci-pastro-0.0.3/README.md
-drwxr-xr-x   0 victoria   (501) staff       (20)        0 2022-10-27 16:01:31.924908 gwsci-pastro-0.0.3/bin/
--rwxr-xr-x   0 victoria   (501) staff       (20)      919 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/calculate_pastro_fgmc
--rwxr-xr-x   0 victoria   (501) staff       (20)     2726 2022-10-27 15:59:13.000000 gwsci-pastro-0.0.3/bin/calculate_pastro_fgmc_test_inj
--rwxr-xr-x   0 victoria   (501) staff       (20)     2678 2022-10-27 15:59:13.000000 gwsci-pastro-0.0.3/bin/calculate_rates
--rwxr-xr-x   0 victoria   (501) staff       (20)     1527 2022-10-27 15:59:13.000000 gwsci-pastro-0.0.3/bin/initialize_pastro_fgmc_model
--rwxr-xr-x   0 victoria   (501) staff       (20)     1994 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_bg_dist_from_gstlal
--rwxr-xr-x   0 victoria   (501) staff       (20)     1671 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_build_gstlal_model
--rwxr-xr-x   0 victoria   (501) staff       (20)     2201 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_calculate_VT
--rwxr-xr-x   0 victoria   (501) staff       (20)     1310 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_count_coinc
--rwxr-xr-x   0 victoria   (501) staff       (20)      993 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_inj_dist_from_gstlal
--rwxr-xr-x   0 victoria   (501) staff       (20)     3067 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_plot_p_lr
--rwxr-xr-x   0 victoria   (501) staff       (20)     1189 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_prepare_config
--rwxr-xr-x   0 victoria   (501) staff       (20)     1210 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_set_lthresh_from_bg_gstlal
--rwxr-xr-x   0 victoria   (501) staff       (20)     1848 2022-07-08 17:30:05.000000 gwsci-pastro-0.0.3/bin/pastro_test_model
-drwxr-xr-x   0 victoria   (501) staff       (20)        0 2022-10-27 16:01:31.925439 gwsci-pastro-0.0.3/gwsci_pastro.egg-info/
--rw-r--r--   0 victoria   (501) staff       (20)     5829 2022-10-27 16:01:31.000000 gwsci-pastro-0.0.3/gwsci_pastro.egg-info/PKG-INFO
--rw-r--r--   0 victoria   (501) staff       (20)      548 2022-10-27 16:01:31.000000 gwsci-pastro-0.0.3/gwsci_pastro.egg-info/SOURCES.txt
--rw-r--r--   0 victoria   (501) staff       (20)        1 2022-10-27 16:01:31.000000 gwsci-pastro-0.0.3/gwsci_pastro.egg-info/dependency_links.txt
--rw-r--r--   0 victoria   (501) staff       (20)        7 2022-10-27 16:01:31.000000 gwsci-pastro-0.0.3/gwsci_pastro.egg-info/top_level.txt
-drwxr-xr-x   0 victoria   (501) staff       (20)        0 2022-10-27 16:01:31.925572 gwsci-pastro-0.0.3/pastro/
--rw-r--r--   0 victoria   (501) staff       (20)    16240 2022-10-27 15:59:13.000000 gwsci-pastro-0.0.3/pastro/pastro.py
--rw-r--r--   0 victoria   (501) staff       (20)       38 2022-10-27 16:01:31.925988 gwsci-pastro-0.0.3/setup.cfg
--rw-r--r--   0 victoria   (501) staff       (20)      743 2022-10-27 16:01:26.000000 gwsci-pastro-0.0.3/setup.py
+drwxr-xr-x   0 victoria   (501) staff       (20)        0 2023-06-01 03:44:55.848264 gwsci-pastro-1.0.0/
+-rw-r--r--   0 victoria   (501) staff       (20)      683 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/LICENSE
+-rw-r--r--   0 victoria   (501) staff       (20)     8429 2023-06-01 03:44:55.848062 gwsci-pastro-1.0.0/PKG-INFO
+-rw-r--r--   0 victoria   (501) staff       (20)     7860 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/README.md
+drwxr-xr-x   0 victoria   (501) staff       (20)        0 2023-06-01 03:44:55.847191 gwsci-pastro-1.0.0/bin/
+-rwxr-xr-x   0 victoria   (501) staff       (20)      919 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/calculate_pastro_fgmc
+-rwxr-xr-x   0 victoria   (501) staff       (20)     2726 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/calculate_pastro_fgmc_test_inj
+-rwxr-xr-x   0 victoria   (501) staff       (20)     2678 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/calculate_rates
+-rwxr-xr-x   0 victoria   (501) staff       (20)     1539 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/initialize_pastro_fgmc_model
+-rwxr-xr-x   0 victoria   (501) staff       (20)     1994 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_bg_dist_from_gstlal
+-rwxr-xr-x   0 victoria   (501) staff       (20)     1671 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_build_gstlal_model
+-rwxr-xr-x   0 victoria   (501) staff       (20)     2201 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_calculate_VT
+-rwxr-xr-x   0 victoria   (501) staff       (20)     1310 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_count_coinc
+-rwxr-xr-x   0 victoria   (501) staff       (20)      993 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_inj_dist_from_gstlal
+-rwxr-xr-x   0 victoria   (501) staff       (20)     3067 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_plot_p_lr
+-rwxr-xr-x   0 victoria   (501) staff       (20)     1189 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_prepare_config
+-rwxr-xr-x   0 victoria   (501) staff       (20)     1210 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_set_lthresh_from_bg_gstlal
+-rwxr-xr-x   0 victoria   (501) staff       (20)     1848 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/bin/pastro_test_model
+drwxr-xr-x   0 victoria   (501) staff       (20)        0 2023-06-01 03:44:55.847679 gwsci-pastro-1.0.0/gwsci_pastro.egg-info/
+-rw-r--r--   0 victoria   (501) staff       (20)     8429 2023-06-01 03:44:55.000000 gwsci-pastro-1.0.0/gwsci_pastro.egg-info/PKG-INFO
+-rw-r--r--   0 victoria   (501) staff       (20)      548 2023-06-01 03:44:55.000000 gwsci-pastro-1.0.0/gwsci_pastro.egg-info/SOURCES.txt
+-rw-r--r--   0 victoria   (501) staff       (20)        1 2023-06-01 03:44:55.000000 gwsci-pastro-1.0.0/gwsci_pastro.egg-info/dependency_links.txt
+-rw-r--r--   0 victoria   (501) staff       (20)        7 2023-06-01 03:44:55.000000 gwsci-pastro-1.0.0/gwsci_pastro.egg-info/top_level.txt
+drwxr-xr-x   0 victoria   (501) staff       (20)        0 2023-06-01 03:44:55.847795 gwsci-pastro-1.0.0/pastro/
+-rw-r--r--   0 victoria   (501) staff       (20)    25965 2023-06-01 03:44:18.000000 gwsci-pastro-1.0.0/pastro/pastro.py
+-rw-r--r--   0 victoria   (501) staff       (20)       38 2023-06-01 03:44:55.848317 gwsci-pastro-1.0.0/setup.cfg
+-rw-r--r--   0 victoria   (501) staff       (20)      743 2023-06-01 03:44:42.000000 gwsci-pastro-1.0.0/setup.py
```

### Comparing `gwsci-pastro-0.0.3/LICENSE` & `gwsci-pastro-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/PKG-INFO` & `gwsci-pastro-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsci-pastro
-Version: 0.0.3
+Version: 1.0.0
 Summary: Tools for calculating astrophysical probability of GW events
 Home-page: https://git.ligo.org/gstlal/pastro
 Author: Chad Hanna, Victoria Niu, Leo Tsukada, Anarya Ray
 Author-email: chad.hanna@ligo.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,26 +12,28 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pastro
 
-This repository tests and builds our p_astro model for the evaluation of p(c|x) with BNS, BBH, NSBH, and Terrestial (noise) events.
+Pastro is a package to estimate the probabilities of astrophysical origins of the gravitational wave candidates detected by the GstLAL pipeline, for the purpose of assisting in real-time multi-messenger follow-up observations. This repository develops and operates our p_astro model for the evaluation of p(category|data) with BNS, BBH, NSBH, and Terrestial (noise) events. 
 
+For more detailed information on the operation manual of pastro, please find the information on **gwsci.org**: https://gwsci.org/ops/pastro 
 
-# Install & Setup (on ICDS, similar in CIT)
 
-We want to execute our package in singularity. Start by making a directory to try this out in e.g. (for testing the fgmc, preferebly use CIT),
+## Install & Setup (on ICDS, similar on CIT)
+
+We want to execute our package in singularity. Start by making a directory to try this out in e.g.:
 
 ```
 $ mkdir /ligo/home/ligo.org/user.name/pastro_test
 $ cd /ligo/home/ligo.org/user.name/pastro_test
 ```
-wherever you want to install the p-astro package at. 
+wherever you want to install the p-astro package at. For using the fgmc model, preferebly use CIT. 
 
 We will install everything in a writable gstlal container. Start by 
 
 ```
 $ singularity build --sandbox --fix-perms gstlal-dev docker://containers.ligo.org/lscsoft/gstlal:master
 ```
 
@@ -55,32 +57,89 @@
 After going into the repo directory, you can setup the environment
 
 
 ```
 Singularity> python3 setup.py install --old-and-unmanageable
 ```
 
-Notice: You need to repeat the `python3 setup.py` step each time you `git pull` the p-astro repo. 
+**Notice**: You need to repeat the `python3 setup.py` step each time you `git pull` the p-astro repo. 
 
 Now you should have a working container with this repo installed. To test it, exit the contaier (e.g., ctrl+D) and try it out
 
 ```
 [chad.hanna@comp-hd-002 pastro_test]$ singularity exec gstlal-dev python3 
 Python 3.6.8 (default, Nov 10 2020, 07:30:01) 
 [GCC 4.8.5 20150623 (Red Hat 4.8.5-44)] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import pastro
 >>>
 ```
 
 It works! the pastro package is installed.
 
-# mchirp method
+## FGMC method (O4 low-latency)
+
+**Ray, Anarya. et. al. (2023)**, dcc-link: https://dcc.ligo.org/P2300141
+
+After installing a writable GstLAL container with pastro package complied, you can generate the pastro model of fgmc method following the example code below (on CIT). If you want to run the code on the ICDS, simply change the environment variable from `$TMPDIR` to `/ligo`. The `Makefile` in `examples/fgmc/` of the pastro repo provides an example of creating the pastro model, which contains the estimated rate of O4 observation, and template-weights of O4 mass model. If you don't want to estimate the O4 rates and template weights, please skip to the example section below. 
+
+README.md for rate estimation and template weights: 
+
+- **Rate Estimation (O4)**: https://git.ligo.org/gstlal/pastro/-/blob/main/Rates_for_O4.md 
+
+- **Template Weights (O4)**: https://git.ligo.org/gstlal/pastro/-/blob/main/template-weights-fgmc-using-manifold.md 
+
+To generate the pastro model, one needs to prepare a mass model with mass cuts implemented for the NS boundaries. In O4, GstLAL uses manifold to generate the mass models and mass models with mass cuts. The README.md above shows how to create this template-weights file from manifold. 
+
+After you have the estimated rates, template-weight files, a ranking-statistic file, and a picked FAR threshold, you can **create the pastro-model file** for the final posterior probability: 
 
-## Executing the Jobs
+```
+singularity exec -B $TMPDIR /path/to/gstlal-dev/ initialize_pastro_fgmc_model --rankstat-filename <your-rank-stat-pdf-file> --weights-dir <path-to-your-template-weights> --V-new <your-sensitive-volume V> --far-threshold <far-threshold> --output <output-model-h5file-name> --rates <rates> --rates-inj <injection-rate>
+```
+
+Once you have the pastro model generated, you can **estimate the events** by:
+
+```
+singularity exec -B $TMPDIR /path/to/gstlal-dev/ calculate_pastro_fgmc --fgmc-model pastro_model_fgmc.h5 --templateid {template_id} --snr {snr-thresh}  --lnlr {likelihood-thresh} {"BBH": <estimated-BBH-rate>, "BNS": <estimated-BNS-rate>, "NSBH": <estimated-NSBH-rate>, "Terr": <noise-rate>}
+```
+
+For example, you can **estimate the p-astro of injection events**:
+
+```
+singularity exec -B  /path/to/gstlal-dev/ calculate_pastro_fgmc_test --output-file pastro_inj.txt --fgmc-model pastro_model_fgmc.h5 --injection-file ${injdb}
+
+```
+
+
+#### (a) Example: Makefile
+
+or, alternatively, using the example in `Makefile`: 
+
+```
+$ cp gstlal-dev/src/pastro/example/fgmc/Makefile .
+$ make
+$singularity exec -B $TMPDIR gstlal-dev ./calculate_pastro_fgmc --fgmc-model fgmc_model.h5 --templateid 7012.0 --snr  14.48703297189981  --lnlr 52.61944811540472
+{"BBH": 0., "BNS": 0.9999929320428521, "NSBH": 4.1997623780371124e-16, "Terr": 0.}
+```
+To calculate pastros of all injection triggers in mdc and save it on a text file,
+```
+$ cp gstlal-dev/src/pastro/example/fgmc/test_model/Makefile .
+$ X509_USER_PROXY=x509_proxy liho-proxy-init user.name
+$ make
+```
+If different Rate and VT numbers from older runs were to be used, run the following script with the different numbers than whats currently in the argument.
+```
+$ signularity exec -B $TMPDIR gstlal-dev/ ./calculate_rates --runtime-old '{"O2":0.75,"O1":0.333333333333}' --dbns-old '{"O1":0.08,"O2":0.1}' --threshold-old 8760.12 --dbns-new 0.13 --T-inj 0.109589 --rates-astro '{"BBH": 18.0730098234, "NSBH":52.9087878433,"BNS":662.448825556 }' --VT-old '{"BBH":0.644707742859,"NSBH":0.0225894859494,"BNS":0.00250795809983}' --z-max '{"BBH":1.9, "BNS":0.15, "NSBH":0.25}' --N-inj '{"BBH":118036.67,"BNS":118036.67, "NSBH":118036.67}' --output rates_V.json --terrestrial-old 3924
+```
+Then copy the Rates and V's from the output of this to the make files and run them again.
+
+
+## Mchirp Method (O3 offline)
+
+### 1. Executing the Jobs
 
 Makefile in `/ligo/home/ligo.org/user.name/pastro_test/gstlal-dev/src/examples/Makefile` provides a good example of running the p-astro jobs.
 
 
 If you want to use the Makefile, follow the instructions below:
 
 make sure you are in your original directory, e.g., `/ligo/home/ligo.org/user.name/pastro_test` then do
@@ -136,15 +195,15 @@
 
 To (end-to-end) test the p-astro model, try:
 
 ```
 make bns-test bbh-test nsbh-test noise-test
 ```
 
-### Optional
+### 2. Optional
 
 1. If you want to calculate the likelihood threshold L* for expected count of noise event N = 1, do
 
 ```
 $ make l-thresh
 ```
 
@@ -157,36 +216,11 @@
 
 3. If you want to calculate the expected count number for O3a analysis, do
 
 ```
 $ make bns-expected-O3a-count bbh-expected-O3a-count nsbh-expected-O3a-count
 ```
 
-# FGMC method
-
-
-creating a container and installing module same as mentioned before
-
-once module is installed create model file and test on example non-injection trigger (go to the directory on CIT inside which the singularity container gstlal-dev is installed):
-
-```
-$ cp gstlal-dev/src/pastro/example/fgmc/Makefile .
-$ make
-$singularity exec -B $TMPDIR gstlal-dev ./calculate_pastro_fgmc --fgmc-model fgmc_model.h5 --templateid 7012.0 --snr  14.48703297189981  --lnlr 52.61944811540472
-{"BBH": 0., "BNS": 0.9999929320428521, "NSBH": 4.1997623780371124e-16, "Terr": 0.}
-```
-To calculate pastros of all injection triggers in mdc7 and save it on a text file,
-```
-$ cp gstlal-dev/src/pastro/example/fgmc/test_model/Makefile .
-$ X509_USER_PROXY=x509_proxy liho-proxy-init user.name
-$ make
-```
-If different Rate and VT numbers from older runs were to be used, run the following script with the different numbers than whats currently in the argument.
-```
-$ signularity exec -B $TMPDIR gstlal-dev/ ./calculate_rates --runtime-old '{"O2":0.75,"O1":0.333333333333}' --dbns-old '{"O1":0.08,"O2":0.1}' --threshold-old 8760.12 --dbns-new 0.13 --T-inj 0.109589 --rates-astro '{"BBH": 18.0730098234, "NSBH":52.9087878433,"BNS":662.448825556 }' --VT-old '{"BBH":0.644707742859,"NSBH":0.0225894859494,"BNS":0.00250795809983}' --z-max '{"BBH":1.9, "BNS":0.15, "NSBH":0.25}' --N-inj '{"BBH":118036.67,"BNS":118036.67, "NSBH":118036.67}' --output rates_V.json --terrestrial-old 3924
-```
-Then copy the Rates and V's from the output of this (^) to the make files and run them again.
-
```

### Comparing `gwsci-pastro-0.0.3/README.md` & `gwsci-pastro-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Pastro
 
-This repository tests and builds our p_astro model for the evaluation of p(c|x) with BNS, BBH, NSBH, and Terrestial (noise) events.
+Pastro is a package to estimate the probabilities of astrophysical origins of the gravitational wave candidates detected by the GstLAL pipeline, for the purpose of assisting in real-time multi-messenger follow-up observations. This repository develops and operates our p_astro model for the evaluation of p(category|data) with BNS, BBH, NSBH, and Terrestial (noise) events. 
 
+For more detailed information on the operation manual of pastro, please find the information on **gwsci.org**: https://gwsci.org/ops/pastro 
 
-# Install & Setup (on ICDS, similar in CIT)
 
-We want to execute our package in singularity. Start by making a directory to try this out in e.g. (for testing the fgmc, preferebly use CIT),
+## Install & Setup (on ICDS, similar on CIT)
+
+We want to execute our package in singularity. Start by making a directory to try this out in e.g.:
 
 ```
 $ mkdir /ligo/home/ligo.org/user.name/pastro_test
 $ cd /ligo/home/ligo.org/user.name/pastro_test
 ```
-wherever you want to install the p-astro package at. 
+wherever you want to install the p-astro package at. For using the fgmc model, preferebly use CIT. 
 
 We will install everything in a writable gstlal container. Start by 
 
 ```
 $ singularity build --sandbox --fix-perms gstlal-dev docker://containers.ligo.org/lscsoft/gstlal:master
 ```
 
@@ -39,32 +41,89 @@
 After going into the repo directory, you can setup the environment
 
 
 ```
 Singularity> python3 setup.py install --old-and-unmanageable
 ```
 
-Notice: You need to repeat the `python3 setup.py` step each time you `git pull` the p-astro repo. 
+**Notice**: You need to repeat the `python3 setup.py` step each time you `git pull` the p-astro repo. 
 
 Now you should have a working container with this repo installed. To test it, exit the contaier (e.g., ctrl+D) and try it out
 
 ```
 [chad.hanna@comp-hd-002 pastro_test]$ singularity exec gstlal-dev python3 
 Python 3.6.8 (default, Nov 10 2020, 07:30:01) 
 [GCC 4.8.5 20150623 (Red Hat 4.8.5-44)] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import pastro
 >>>
 ```
 
 It works! the pastro package is installed.
 
-# mchirp method
+## FGMC method (O4 low-latency)
+
+**Ray, Anarya. et. al. (2023)**, dcc-link: https://dcc.ligo.org/P2300141
+
+After installing a writable GstLAL container with pastro package complied, you can generate the pastro model of fgmc method following the example code below (on CIT). If you want to run the code on the ICDS, simply change the environment variable from `$TMPDIR` to `/ligo`. The `Makefile` in `examples/fgmc/` of the pastro repo provides an example of creating the pastro model, which contains the estimated rate of O4 observation, and template-weights of O4 mass model. If you don't want to estimate the O4 rates and template weights, please skip to the example section below. 
+
+README.md for rate estimation and template weights: 
+
+- **Rate Estimation (O4)**: https://git.ligo.org/gstlal/pastro/-/blob/main/Rates_for_O4.md 
+
+- **Template Weights (O4)**: https://git.ligo.org/gstlal/pastro/-/blob/main/template-weights-fgmc-using-manifold.md 
+
+To generate the pastro model, one needs to prepare a mass model with mass cuts implemented for the NS boundaries. In O4, GstLAL uses manifold to generate the mass models and mass models with mass cuts. The README.md above shows how to create this template-weights file from manifold. 
+
+After you have the estimated rates, template-weight files, a ranking-statistic file, and a picked FAR threshold, you can **create the pastro-model file** for the final posterior probability: 
 
-## Executing the Jobs
+```
+singularity exec -B $TMPDIR /path/to/gstlal-dev/ initialize_pastro_fgmc_model --rankstat-filename <your-rank-stat-pdf-file> --weights-dir <path-to-your-template-weights> --V-new <your-sensitive-volume V> --far-threshold <far-threshold> --output <output-model-h5file-name> --rates <rates> --rates-inj <injection-rate>
+```
+
+Once you have the pastro model generated, you can **estimate the events** by:
+
+```
+singularity exec -B $TMPDIR /path/to/gstlal-dev/ calculate_pastro_fgmc --fgmc-model pastro_model_fgmc.h5 --templateid {template_id} --snr {snr-thresh}  --lnlr {likelihood-thresh} {"BBH": <estimated-BBH-rate>, "BNS": <estimated-BNS-rate>, "NSBH": <estimated-NSBH-rate>, "Terr": <noise-rate>}
+```
+
+For example, you can **estimate the p-astro of injection events**:
+
+```
+singularity exec -B  /path/to/gstlal-dev/ calculate_pastro_fgmc_test --output-file pastro_inj.txt --fgmc-model pastro_model_fgmc.h5 --injection-file ${injdb}
+
+```
+
+
+#### (a) Example: Makefile
+
+or, alternatively, using the example in `Makefile`: 
+
+```
+$ cp gstlal-dev/src/pastro/example/fgmc/Makefile .
+$ make
+$singularity exec -B $TMPDIR gstlal-dev ./calculate_pastro_fgmc --fgmc-model fgmc_model.h5 --templateid 7012.0 --snr  14.48703297189981  --lnlr 52.61944811540472
+{"BBH": 0., "BNS": 0.9999929320428521, "NSBH": 4.1997623780371124e-16, "Terr": 0.}
+```
+To calculate pastros of all injection triggers in mdc and save it on a text file,
+```
+$ cp gstlal-dev/src/pastro/example/fgmc/test_model/Makefile .
+$ X509_USER_PROXY=x509_proxy liho-proxy-init user.name
+$ make
+```
+If different Rate and VT numbers from older runs were to be used, run the following script with the different numbers than whats currently in the argument.
+```
+$ signularity exec -B $TMPDIR gstlal-dev/ ./calculate_rates --runtime-old '{"O2":0.75,"O1":0.333333333333}' --dbns-old '{"O1":0.08,"O2":0.1}' --threshold-old 8760.12 --dbns-new 0.13 --T-inj 0.109589 --rates-astro '{"BBH": 18.0730098234, "NSBH":52.9087878433,"BNS":662.448825556 }' --VT-old '{"BBH":0.644707742859,"NSBH":0.0225894859494,"BNS":0.00250795809983}' --z-max '{"BBH":1.9, "BNS":0.15, "NSBH":0.25}' --N-inj '{"BBH":118036.67,"BNS":118036.67, "NSBH":118036.67}' --output rates_V.json --terrestrial-old 3924
+```
+Then copy the Rates and V's from the output of this to the make files and run them again.
+
+
+## Mchirp Method (O3 offline)
+
+### 1. Executing the Jobs
 
 Makefile in `/ligo/home/ligo.org/user.name/pastro_test/gstlal-dev/src/examples/Makefile` provides a good example of running the p-astro jobs.
 
 
 If you want to use the Makefile, follow the instructions below:
 
 make sure you are in your original directory, e.g., `/ligo/home/ligo.org/user.name/pastro_test` then do
@@ -120,15 +179,15 @@
 
 To (end-to-end) test the p-astro model, try:
 
 ```
 make bns-test bbh-test nsbh-test noise-test
 ```
 
-### Optional
+### 2. Optional
 
 1. If you want to calculate the likelihood threshold L* for expected count of noise event N = 1, do
 
 ```
 $ make l-thresh
 ```
 
@@ -141,34 +200,9 @@
 
 3. If you want to calculate the expected count number for O3a analysis, do
 
 ```
 $ make bns-expected-O3a-count bbh-expected-O3a-count nsbh-expected-O3a-count
 ```
 
-# FGMC method
-
-
-creating a container and installing module same as mentioned before
-
-once module is installed create model file and test on example non-injection trigger (go to the directory on CIT inside which the singularity container gstlal-dev is installed):
-
-```
-$ cp gstlal-dev/src/pastro/example/fgmc/Makefile .
-$ make
-$singularity exec -B $TMPDIR gstlal-dev ./calculate_pastro_fgmc --fgmc-model fgmc_model.h5 --templateid 7012.0 --snr  14.48703297189981  --lnlr 52.61944811540472
-{"BBH": 0., "BNS": 0.9999929320428521, "NSBH": 4.1997623780371124e-16, "Terr": 0.}
-```
-To calculate pastros of all injection triggers in mdc7 and save it on a text file,
-```
-$ cp gstlal-dev/src/pastro/example/fgmc/test_model/Makefile .
-$ X509_USER_PROXY=x509_proxy liho-proxy-init user.name
-$ make
-```
-If different Rate and VT numbers from older runs were to be used, run the following script with the different numbers than whats currently in the argument.
-```
-$ signularity exec -B $TMPDIR gstlal-dev/ ./calculate_rates --runtime-old '{"O2":0.75,"O1":0.333333333333}' --dbns-old '{"O1":0.08,"O2":0.1}' --threshold-old 8760.12 --dbns-new 0.13 --T-inj 0.109589 --rates-astro '{"BBH": 18.0730098234, "NSBH":52.9087878433,"BNS":662.448825556 }' --VT-old '{"BBH":0.644707742859,"NSBH":0.0225894859494,"BNS":0.00250795809983}' --z-max '{"BBH":1.9, "BNS":0.15, "NSBH":0.25}' --N-inj '{"BBH":118036.67,"BNS":118036.67, "NSBH":118036.67}' --output rates_V.json --terrestrial-old 3924
-```
-Then copy the Rates and V's from the output of this (^) to the make files and run them again.
-
```

### Comparing `gwsci-pastro-0.0.3/bin/calculate_pastro_fgmc` & `gwsci-pastro-1.0.0/bin/calculate_pastro_fgmc`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/calculate_pastro_fgmc_test_inj` & `gwsci-pastro-1.0.0/bin/calculate_pastro_fgmc_test_inj`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/calculate_rates` & `gwsci-pastro-1.0.0/bin/calculate_rates`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/initialize_pastro_fgmc_model` & `gwsci-pastro-1.0.0/bin/initialize_pastro_fgmc_model`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 
 from optparse import OptionParser
-import pastro
+from pastro import pastro
 import json
 
 def parse_command_line():
   parser = OptionParser()
   parser.add_option("-v", "--verbose", action = "store_true", help = "Be verbose.",default=False)
   parser.add_option("--rankstat-filename", help = "the rankingstatpdf .xml.gz filename")
   parser.add_option("--rates", help="string of dictionary containing merger rates of each category in MPc^-3 months^-1")
```

### Comparing `gwsci-pastro-0.0.3/bin/pastro_bg_dist_from_gstlal` & `gwsci-pastro-1.0.0/bin/pastro_bg_dist_from_gstlal`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_build_gstlal_model` & `gwsci-pastro-1.0.0/bin/pastro_build_gstlal_model`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_calculate_VT` & `gwsci-pastro-1.0.0/bin/pastro_calculate_VT`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_count_coinc` & `gwsci-pastro-1.0.0/bin/pastro_count_coinc`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_inj_dist_from_gstlal` & `gwsci-pastro-1.0.0/bin/pastro_inj_dist_from_gstlal`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_plot_p_lr` & `gwsci-pastro-1.0.0/bin/pastro_plot_p_lr`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_prepare_config` & `gwsci-pastro-1.0.0/bin/pastro_prepare_config`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_set_lthresh_from_bg_gstlal` & `gwsci-pastro-1.0.0/bin/pastro_set_lthresh_from_bg_gstlal`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/bin/pastro_test_model` & `gwsci-pastro-1.0.0/bin/pastro_test_model`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/gwsci_pastro.egg-info/PKG-INFO` & `gwsci-pastro-1.0.0/gwsci_pastro.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwsci-pastro
-Version: 0.0.3
+Version: 1.0.0
 Summary: Tools for calculating astrophysical probability of GW events
 Home-page: https://git.ligo.org/gstlal/pastro
 Author: Chad Hanna, Victoria Niu, Leo Tsukada, Anarya Ray
 Author-email: chad.hanna@ligo.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,26 +12,28 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pastro
 
-This repository tests and builds our p_astro model for the evaluation of p(c|x) with BNS, BBH, NSBH, and Terrestial (noise) events.
+Pastro is a package to estimate the probabilities of astrophysical origins of the gravitational wave candidates detected by the GstLAL pipeline, for the purpose of assisting in real-time multi-messenger follow-up observations. This repository develops and operates our p_astro model for the evaluation of p(category|data) with BNS, BBH, NSBH, and Terrestial (noise) events. 
 
+For more detailed information on the operation manual of pastro, please find the information on **gwsci.org**: https://gwsci.org/ops/pastro 
 
-# Install & Setup (on ICDS, similar in CIT)
 
-We want to execute our package in singularity. Start by making a directory to try this out in e.g. (for testing the fgmc, preferebly use CIT),
+## Install & Setup (on ICDS, similar on CIT)
+
+We want to execute our package in singularity. Start by making a directory to try this out in e.g.:
 
 ```
 $ mkdir /ligo/home/ligo.org/user.name/pastro_test
 $ cd /ligo/home/ligo.org/user.name/pastro_test
 ```
-wherever you want to install the p-astro package at. 
+wherever you want to install the p-astro package at. For using the fgmc model, preferebly use CIT. 
 
 We will install everything in a writable gstlal container. Start by 
 
 ```
 $ singularity build --sandbox --fix-perms gstlal-dev docker://containers.ligo.org/lscsoft/gstlal:master
 ```
 
@@ -55,32 +57,89 @@
 After going into the repo directory, you can setup the environment
 
 
 ```
 Singularity> python3 setup.py install --old-and-unmanageable
 ```
 
-Notice: You need to repeat the `python3 setup.py` step each time you `git pull` the p-astro repo. 
+**Notice**: You need to repeat the `python3 setup.py` step each time you `git pull` the p-astro repo. 
 
 Now you should have a working container with this repo installed. To test it, exit the contaier (e.g., ctrl+D) and try it out
 
 ```
 [chad.hanna@comp-hd-002 pastro_test]$ singularity exec gstlal-dev python3 
 Python 3.6.8 (default, Nov 10 2020, 07:30:01) 
 [GCC 4.8.5 20150623 (Red Hat 4.8.5-44)] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import pastro
 >>>
 ```
 
 It works! the pastro package is installed.
 
-# mchirp method
+## FGMC method (O4 low-latency)
+
+**Ray, Anarya. et. al. (2023)**, dcc-link: https://dcc.ligo.org/P2300141
+
+After installing a writable GstLAL container with pastro package complied, you can generate the pastro model of fgmc method following the example code below (on CIT). If you want to run the code on the ICDS, simply change the environment variable from `$TMPDIR` to `/ligo`. The `Makefile` in `examples/fgmc/` of the pastro repo provides an example of creating the pastro model, which contains the estimated rate of O4 observation, and template-weights of O4 mass model. If you don't want to estimate the O4 rates and template weights, please skip to the example section below. 
+
+README.md for rate estimation and template weights: 
+
+- **Rate Estimation (O4)**: https://git.ligo.org/gstlal/pastro/-/blob/main/Rates_for_O4.md 
+
+- **Template Weights (O4)**: https://git.ligo.org/gstlal/pastro/-/blob/main/template-weights-fgmc-using-manifold.md 
+
+To generate the pastro model, one needs to prepare a mass model with mass cuts implemented for the NS boundaries. In O4, GstLAL uses manifold to generate the mass models and mass models with mass cuts. The README.md above shows how to create this template-weights file from manifold. 
+
+After you have the estimated rates, template-weight files, a ranking-statistic file, and a picked FAR threshold, you can **create the pastro-model file** for the final posterior probability: 
 
-## Executing the Jobs
+```
+singularity exec -B $TMPDIR /path/to/gstlal-dev/ initialize_pastro_fgmc_model --rankstat-filename <your-rank-stat-pdf-file> --weights-dir <path-to-your-template-weights> --V-new <your-sensitive-volume V> --far-threshold <far-threshold> --output <output-model-h5file-name> --rates <rates> --rates-inj <injection-rate>
+```
+
+Once you have the pastro model generated, you can **estimate the events** by:
+
+```
+singularity exec -B $TMPDIR /path/to/gstlal-dev/ calculate_pastro_fgmc --fgmc-model pastro_model_fgmc.h5 --templateid {template_id} --snr {snr-thresh}  --lnlr {likelihood-thresh} {"BBH": <estimated-BBH-rate>, "BNS": <estimated-BNS-rate>, "NSBH": <estimated-NSBH-rate>, "Terr": <noise-rate>}
+```
+
+For example, you can **estimate the p-astro of injection events**:
+
+```
+singularity exec -B  /path/to/gstlal-dev/ calculate_pastro_fgmc_test --output-file pastro_inj.txt --fgmc-model pastro_model_fgmc.h5 --injection-file ${injdb}
+
+```
+
+
+#### (a) Example: Makefile
+
+or, alternatively, using the example in `Makefile`: 
+
+```
+$ cp gstlal-dev/src/pastro/example/fgmc/Makefile .
+$ make
+$singularity exec -B $TMPDIR gstlal-dev ./calculate_pastro_fgmc --fgmc-model fgmc_model.h5 --templateid 7012.0 --snr  14.48703297189981  --lnlr 52.61944811540472
+{"BBH": 0., "BNS": 0.9999929320428521, "NSBH": 4.1997623780371124e-16, "Terr": 0.}
+```
+To calculate pastros of all injection triggers in mdc and save it on a text file,
+```
+$ cp gstlal-dev/src/pastro/example/fgmc/test_model/Makefile .
+$ X509_USER_PROXY=x509_proxy liho-proxy-init user.name
+$ make
+```
+If different Rate and VT numbers from older runs were to be used, run the following script with the different numbers than whats currently in the argument.
+```
+$ signularity exec -B $TMPDIR gstlal-dev/ ./calculate_rates --runtime-old '{"O2":0.75,"O1":0.333333333333}' --dbns-old '{"O1":0.08,"O2":0.1}' --threshold-old 8760.12 --dbns-new 0.13 --T-inj 0.109589 --rates-astro '{"BBH": 18.0730098234, "NSBH":52.9087878433,"BNS":662.448825556 }' --VT-old '{"BBH":0.644707742859,"NSBH":0.0225894859494,"BNS":0.00250795809983}' --z-max '{"BBH":1.9, "BNS":0.15, "NSBH":0.25}' --N-inj '{"BBH":118036.67,"BNS":118036.67, "NSBH":118036.67}' --output rates_V.json --terrestrial-old 3924
+```
+Then copy the Rates and V's from the output of this to the make files and run them again.
+
+
+## Mchirp Method (O3 offline)
+
+### 1. Executing the Jobs
 
 Makefile in `/ligo/home/ligo.org/user.name/pastro_test/gstlal-dev/src/examples/Makefile` provides a good example of running the p-astro jobs.
 
 
 If you want to use the Makefile, follow the instructions below:
 
 make sure you are in your original directory, e.g., `/ligo/home/ligo.org/user.name/pastro_test` then do
@@ -136,15 +195,15 @@
 
 To (end-to-end) test the p-astro model, try:
 
 ```
 make bns-test bbh-test nsbh-test noise-test
 ```
 
-### Optional
+### 2. Optional
 
 1. If you want to calculate the likelihood threshold L* for expected count of noise event N = 1, do
 
 ```
 $ make l-thresh
 ```
 
@@ -157,36 +216,11 @@
 
 3. If you want to calculate the expected count number for O3a analysis, do
 
 ```
 $ make bns-expected-O3a-count bbh-expected-O3a-count nsbh-expected-O3a-count
 ```
 
-# FGMC method
-
-
-creating a container and installing module same as mentioned before
-
-once module is installed create model file and test on example non-injection trigger (go to the directory on CIT inside which the singularity container gstlal-dev is installed):
-
-```
-$ cp gstlal-dev/src/pastro/example/fgmc/Makefile .
-$ make
-$singularity exec -B $TMPDIR gstlal-dev ./calculate_pastro_fgmc --fgmc-model fgmc_model.h5 --templateid 7012.0 --snr  14.48703297189981  --lnlr 52.61944811540472
-{"BBH": 0., "BNS": 0.9999929320428521, "NSBH": 4.1997623780371124e-16, "Terr": 0.}
-```
-To calculate pastros of all injection triggers in mdc7 and save it on a text file,
-```
-$ cp gstlal-dev/src/pastro/example/fgmc/test_model/Makefile .
-$ X509_USER_PROXY=x509_proxy liho-proxy-init user.name
-$ make
-```
-If different Rate and VT numbers from older runs were to be used, run the following script with the different numbers than whats currently in the argument.
-```
-$ signularity exec -B $TMPDIR gstlal-dev/ ./calculate_rates --runtime-old '{"O2":0.75,"O1":0.333333333333}' --dbns-old '{"O1":0.08,"O2":0.1}' --threshold-old 8760.12 --dbns-new 0.13 --T-inj 0.109589 --rates-astro '{"BBH": 18.0730098234, "NSBH":52.9087878433,"BNS":662.448825556 }' --VT-old '{"BBH":0.644707742859,"NSBH":0.0225894859494,"BNS":0.00250795809983}' --z-max '{"BBH":1.9, "BNS":0.15, "NSBH":0.25}' --N-inj '{"BBH":118036.67,"BNS":118036.67, "NSBH":118036.67}' --output rates_V.json --terrestrial-old 3924
-```
-Then copy the Rates and V's from the output of this (^) to the make files and run them again.
-
```

### Comparing `gwsci-pastro-0.0.3/gwsci_pastro.egg-info/SOURCES.txt` & `gwsci-pastro-1.0.0/gwsci_pastro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwsci-pastro-0.0.3/pastro/pastro.py` & `gwsci-pastro-1.0.0/pastro/pastro.py`

 * *Files 23% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     for cat in self.categories:
       self.p_ci[cat] = self.expected_counts_above_thresh[cat] / Nsum / int_p_x_given_ci_above_L[cat]
    
   # This does nothing
   def update_rankstatpdf(self,newrankstatpdffile=None):
     pass
 
-  def __call__(self, data):
+  def __call__(self, data,inj=False):
     mc = data["mchirp"]
     lr = data["likelihood"]
     out = {}
     for cat in self.categories:
       out[cat] = numpy.exp(self.lnp_x_given_ci[cat](mc, lr)) * self.p_ci[cat]
     norm = sum(out.values())
 
@@ -168,60 +168,60 @@
     return json.dumps(p_a)
 
   def to_h5(self, fname):
     """
     read to h5 file
 
     """
-    f = h5py.File(fname, "w")
-    # FIXME not elegant
-    f.attrs['model'] = 0
-    dist = f.create_group("distributions")
-    dist.create_dataset("mcbins", data=numpy.array([self.mcstart, self.mcstop, self.mcnum]))
-    dist.create_dataset("lrbins", data=numpy.array([self.lrstart, self.lrstop, self.lrnum]))
-    counts = dist.create_group("counts")
-    for category in self.LnPDF:
-      counts.create_dataset(category, data = self.LnPDF[category].array)
-    if self.lr_thresh is not None:
-      dist.create_dataset("lr_thresh", data=self.lr_thresh)
-    if self.expected_counts_above_thresh is not None:
-      expected = dist.create_group("expected_counts_above_thresh")
-      for category in self.expected_counts_above_thresh:
-        expected.create_dataset(category, data=self.expected_counts_above_thresh[category])
+    with h5py.File(fname, "w") as f:
+        # FIXME not elegant
+        f.attrs['model'] = 0
+        dist = f.create_group("distributions")
+        dist.create_dataset("mcbins", data=numpy.array([self.mcstart, self.mcstop, self.mcnum]))
+        dist.create_dataset("lrbins", data=numpy.array([self.lrstart, self.lrstop, self.lrnum]))
+        counts = dist.create_group("counts")
+        for category in self.LnPDF:
+          counts.create_dataset(category, data = self.LnPDF[category].array)
+        if self.lr_thresh is not None:
+          dist.create_dataset("lr_thresh", data=self.lr_thresh)
+        if self.expected_counts_above_thresh is not None:
+          expected = dist.create_group("expected_counts_above_thresh")
+          for category in self.expected_counts_above_thresh:
+            expected.create_dataset(category, data=self.expected_counts_above_thresh[category])
 
-    f.close()
+        f.close()
 
   @classmethod
   def from_h5(cls, fname):
     """
     read from h5 file
     
     """
-    f = h5py.File(fname)
-    dist = f["distributions"]
-    mcstart, mcstop, mcnum = dist["mcbins"]
-    lrstart, lrstop, lrnum = dist["lrbins"]
-    categories = set(dist["counts"].keys())
-
-    model = pastro_model(mcstart, mcstop, mcnum, lrstart, lrstop, lrnum, categories)
-
-    for category in categories:
-      model.LnPDF[category].count.array[:] = numpy.array(dist["counts"][category])[:]
-    if "expected_counts_above_thresh" in dist:
-      model.expected_counts_above_thresh = {}
-      for category in dist["expected_counts_above_thresh"]:
-        model.expected_counts_above_thresh[category] = numpy.array(dist["expected_counts_above_thresh"][category]).item()
-    if "lr_thresh" in dist:
-        model.lr_thresh = numpy.array(dist["lr_thresh"]).item()
-    f.close()
+    with h5py.File(fname) as f:
+        dist = f["distributions"]
+        mcstart, mcstop, mcnum = dist["mcbins"]
+        lrstart, lrstop, lrnum = dist["lrbins"]
+        categories = set(dist["counts"].keys())
+
+        model = pastro_model(mcstart, mcstop, mcnum, lrstart, lrstop, lrnum, categories)
+
+        for category in categories:
+          model.LnPDF[category].count.array[:] = numpy.array(dist["counts"][category])[:]
+        if "expected_counts_above_thresh" in dist:
+          model.expected_counts_above_thresh = {}
+          for category in dist["expected_counts_above_thresh"]:
+            model.expected_counts_above_thresh[category] = numpy.array(dist["expected_counts_above_thresh"][category]).item()
+        if "lr_thresh" in dist:
+            model.lr_thresh = numpy.array(dist["lr_thresh"]).item()
+        f.close()
     return model
 
 class p_astro_fgmc(object):
     
-    def __init__(self, A_init=0.0, coefficients=0.0, SNR=0.0, indextoid=None, rates={'BBH':0.,'BNS':0.,'NSBH':0.},rates_inj={'BBH':0.,'BNS':0.,'NSBH':0.},far_th=2.78e-4,V={'BBH':0.,'BNS':0.,'NSBH':0.}):
+    def __init__(self, A_init=1.0, coefficients=0.0, SNR=0.0, indextoid=None, rates={'BBH':0.,'BNS':0.,'NSBH':0.},rates_inj={'BBH':0.,'BNS':0.,'NSBH':0.},far_th=2.78e-4,V={'BBH':0.,'BNS':0.,'NSBH':0.}):
         
         categories=list(rates.keys())
         self.categories=categories
         
         self.template_weight_coefficients=coefficients
         self.template_weight_SNR=SNR
         
@@ -233,15 +233,15 @@
         self.rates_inj=rates_inj
         self.far_th=far_th
         self.counts={c:self.rates[c]*self.V[c] for c in self.categories}
         self.counts_inj={c:self.rates_inj[c]*self.V[c] for c in self.categories}
         self.counts['Terr']=self.far_th
         self.counts_inj['Terr']=self.far_th
     
-    def read_dir(self, template_weight_dir, rankstat_file, template_bank_database=None):
+    def read_dir(self, template_weight_dir, rankstat_file=None, template_bank_database=None):
       """
       read template_weight, rankstat, and template_bank from the directory path. 
       """
       # set self.template_bank_database
       if(template_bank_database is not None):
           connection=sqlite3.connect(template_bank_database)
           cur=connection.cursor()
@@ -254,33 +254,37 @@
           self.indextoid=np.zeros(len(indextoid['k']))
           self.indextoid[indextoid['k']]=indextoid['template_id']
           self.indextoid=self.indextoid.tolist()
       else:
           self.indextoid=[]
       
       # set self.A
-      A,B, fapfar,rankstatpdf,xmin=self.normalize_f_over_b(rankstat_file)
-      far_th_file=fapfar.far_from_rank(xmin)
-      if self.far_th is None:
-          self.far_th=far_th_file
-      self.A=A
+      if rankstat_file is not None:
+          A,B, fapfar,rankstatpdf,xmin=self.normalize_f_over_b(rankstat_file)
+          far_th_file=fapfar.far_from_rank(xmin)
+          if self.far_th is None:
+              self.far_th=far_th_file
+          self.A=A
 
+      else:
+          pass
+      
       # set self.template_weights*
       coefficients,SNR=self.load_template_weights(template_weight_dir)
       self.template_weight_coefficients=coefficients
       self.template_weight_SNR=SNR
 
       # return self  # not needed
     
     def update_rankstatpdf(self,newrankstatpdffile=None):
         if newrankstatpdffile is None:
             pass
         else:
               A,B, fapfar,rankstatpdf,xmin=self.normalize_f_over_b(newrankstatpdffile)
-              far_th_file=fapfar.far_from_rank(xmin)
+              far_th_file=fapfar.far_from_rank(xmin)/3.17098e-8
               if self.far_th is None:
                   self.far_th=far_th_file
               self.A=A
     
     def load_template_weights(self,template_weight_dir):
         filenames=glob.glob(template_weight_dir+'/ceff*.h5')
         coefficients={}
@@ -316,15 +320,15 @@
     
     
         rankingstatpdf = rankingstatpdf.new_with_extinction()
         fapfar = far.FAPFAR(rankingstatpdf)
         
         
         
-        xmin=max(fapfar.rank_from_far(self.far_th),ln_likelihood_ratio_threshold)
+        xmin=max(fapfar.rank_from_far(self.far_th*3.17098e-8),ln_likelihood_ratio_threshold)
     
         rankingstatpdf.noise_lr_lnpdf.array[: rankingstatpdf.noise_lr_lnpdf.bins[0][xmin]]=0.
         rankingstatpdf.noise_lr_lnpdf.normalize()
         rankingstatpdf.signal_lr_lnpdf.array[: rankingstatpdf.signal_lr_lnpdf.bins[0][xmin]]=0.
         rankingstatpdf.signal_lr_lnpdf.normalize()
         rankingstatpdf.zero_lag_lr_lnpdf.array[:rankingstatpdf.zero_lag_lr_lnpdf.bins[0][xmin]]=0.
         rankingstatpdf.zero_lag_lr_lnpdf.normalize()
@@ -388,88 +392,362 @@
 
     # This does nothing
     def finalize(self, prior=None):
         pass
         
     def to_h5(self,filename):
         
-        hf=h5py.File(filename,'w')
-        # FIXME not elegant
-        hf.attrs['model'] = 1
-        coefficients=hf.create_group('coefficients')
-        for c in self.categories:
-            coefficients.create_dataset(c,data=self.template_weight_coefficients[c].astype(np.float16))
-        hf.create_dataset('SNR',data=self.template_weight_SNR.astype(np.float16))
+        with h5py.File(filename,'w') as hf:
+            # FIXME not elegant
+            hf.attrs['model'] = 1
+            coefficients=hf.create_group('coefficients')
+            for c in self.categories:
+                coefficients.create_dataset(c,data=self.template_weight_coefficients[c].astype(np.float16))
+            hf.create_dataset('SNR',data=self.template_weight_SNR.astype(np.float16))
+
+            hf.create_dataset('A',data=np.array([self.A]))
+
+
+            rates=hf.create_group('rates')
+            for c in list(self.rates.keys()):
+                rates.create_dataset(c,data=np.array([self.rates[c]]))
+
+            rates_inj=hf.create_group('rates_inj')
+            for c in list(self.rates_inj.keys()):
+                rates_inj.create_dataset(c,data=np.array([self.rates_inj[c]]))
+
+            V=hf.create_group('V')
+            for c in list(self.V.keys()):
+                V.create_dataset(c,data=np.array([self.V[c]]))
+
+            hf.create_dataset('far_th',data=np.array([self.far_th]))
+
+            hf.create_dataset('indextoid',data=np.array(self.indextoid).astype(np.int32))
+
+            hf.close()
+        
+    @classmethod
+    def from_h5(cls,filename):
         
-        hf.create_dataset('A',data=np.array([self.A]))
+        self=cls.__new__(cls)
+        with h5py.File(filename,'r') as hf:
         
+            coefficients=hf['coefficients']
+            coeff={}
+            for c in list(coefficients.keys()):
+                coeff[c]=coefficients[c][()].astype(np.float16)
+            self.template_weight_coefficients=coeff
+            self.categories=list(coeff.keys())
+            self.template_weight_SNR=hf['SNR'][()].astype(np.float16)
+
+            self.A=hf['A'][()][0]
+
+
+            self.rates={}
+            rates=hf['rates']
+            for c in list(rates.keys()):
+                self.rates[c]=rates[c][()][0]
+
+            self.rates_inj={}
+            rates_inj=hf['rates_inj']
+            for c in list(rates_inj.keys()):
+                self.rates_inj[c]=rates_inj[c][()][0]
+
+            self.V={}
+            V=hf['V']
+            for c in list(V.keys()):
+                self.V[c]=V[c][()][0]
+
+            self.far_th=hf['far_th'][()][0]
+
+            self.counts={c:self.rates[c]*self.V[c] for c in self.categories}
+            self.counts_inj={c:self.rates_inj[c]*self.V[c] for c in self.categories}
+            self.counts['Terr']=self.far_th
+            self.counts_inj['Terr']=self.far_th
+
+            self.indextoid=hf['indextoid'][()].astype(np.int32).tolist()
+            hf.close()
         
-        rates=hf.create_group('rates')
-        for c in list(self.rates.keys()):
-            rates.create_dataset(c,data=np.array([self.rates[c]]))
+        return self
+    
+class p_astro_ew(object):
+    
+    def __init__(self,N_BNS_O123=2,N_terr_O123=11541,d_BNS={'O4':190.,'O3':130.,'O2':100.,'O1':80.},
+                VT_ratios={'29':0.0660,'32':0.0995,'38':0.187,'49':0.376,'56':0.487,'1024':1},
+                Far_th_new_per_year=8760,T_run_in_year={'O3':1.,'O2':0.75,'O1':0.333},
+                Far_th_old_per_year=8760,R_inj=None,V_BNS_O123=None,new_run='O4',rankstatpdf_file=None):
         
-        rates_inj=hf.create_group('rates_inj')
-        for c in list(self.rates_inj.keys()):
-            rates_inj.create_dataset(c,data=np.array([self.rates_inj[c]]))
         
-        V=hf.create_group('V')
-        for c in list(self.V.keys()):
-            V.create_dataset(c,data=np.array([self.V[c]]))
         
-        hf.create_dataset('far_th',data=np.array([self.far_th]))
+        self.N_astro_1024=N_BNS_O123*(d_BNS[new_run]**3/sum([d_BNS[k]**3*T_r for k,T_r in T_run_in_year.items()]))*sum(list(T_run_in_year.values()))*Far_th_old_per_year/N_terr_O123
         
-        hf.create_dataset('indextoid',data=np.array(self.indextoid).astype(np.int32))
-       
-        hf.close()
+        if R_inj is not None:
+            assert V_BNS_O123 is not None
+            self.N_inj_1024 = (R_inj*V_BNS_O123)*(d_BNS[new_run]**3/sum([d_BNS[k]**3*T_r for k,T_r in T_run_in_year.items()]))*sum(list(T_run_in_year.values()))*Far_th_old_per_year/N_terr_O123
+        else:
+            self.N_inj_1024=self.N_astro_1024
+        
+        self.N_astro_fhigh={k:self.N_astro_1024*VT_ratio for k,VT_ratio in VT_ratios.items()}
+        self.N_inj_fhigh={k:self.N_inj_1024*VT_ratio for k,VT_ratio in VT_ratios.items()}
+        
+        self.far_th=Far_th_new_per_year
+        
+        if rankstatpdf_file is not None:
+            A,_,_,_,_=self.normalize_f_over_b(rankstatpdf_file,far_th=Far_th_new_per_year/3.154e+7)
+            self.A=A
+        else:
+            self.A=1.
+        
+    
+    def normalize_f_over_b(self,rankstatpdf_file,far_th=1/3.154e+7):
+        
+        rankingstatpdf = far.marginalize_pdf_urls([rankstatpdf_file], "RankingStatPDF", verbose=True)
+    
+        zero_lag_lr_lnpdf = rankingstatpdf.zero_lag_lr_lnpdf
+        zl = rankingstatpdf.zero_lag_lr_lnpdf.copy()
+        zl.array[:40] = 0.
+    
+        if not zl.array.any():
+            raise ValueError("zero-lag counts are all zero")
+        ln_likelihood_ratio_threshold, = zl.argmax()
+    
+    
+        rankingstatpdf = rankingstatpdf.new_with_extinction()
+        fapfar = far.FAPFAR(rankingstatpdf)
+        
+        
+        
+        xmin=max(fapfar.rank_from_far(self.far_th*3.17098e-8),ln_likelihood_ratio_threshold)
+    
+        rankingstatpdf.noise_lr_lnpdf.array[: rankingstatpdf.noise_lr_lnpdf.bins[0][xmin]]=0.
+        rankingstatpdf.noise_lr_lnpdf.normalize()
+        rankingstatpdf.signal_lr_lnpdf.array[: rankingstatpdf.signal_lr_lnpdf.bins[0][xmin]]=0.
+        rankingstatpdf.signal_lr_lnpdf.normalize()
+        rankingstatpdf.zero_lag_lr_lnpdf.array[:rankingstatpdf.zero_lag_lr_lnpdf.bins[0][xmin]]=0.
+        rankingstatpdf.zero_lag_lr_lnpdf.normalize()
+    
+    
+        noise_lr_lnpdf=rankingstatpdf.noise_lr_lnpdf.mkinterp()
+        lnb=np.vectorize(lambda x: noise_lr_lnpdf(x))
+    
+        B,dB=quad(lambda x: np.exp(lnb(x)),xmin,np.inf,limit=1000)
+    
+        A,dA=quad( lambda x : np.exp(x+lnb(x)-np.log(B)),xmin,np.inf,limit=1000)
+        
+        lnb=None
+        
+        return A,B, fapfar,rankingstatpdf,xmin
+    
+    
+    
+    def update_rankstatpdf(self,newrankstatpdffile=None):
+        if newrankstatpdffile is None:
+            pass
+        else:
+              A,B, fapfar,rankstatpdf,xmin=self.normalize_f_over_b(newrankstatpdffile)
+              far_th_file=fapfar.far_from_rank(xmin)/3.17098e-8
+              if self.far_th is None:
+                  self.far_th=far_th_file
+              self.A=A
+    
+    
+    def __call__(self, data, inj=False):
+        
+        rankstat = float(data['likelihood'])
+        fhigh = data['fhigh']
+        
+        f_over_b=np.exp(rankstat)/self.A
+        N_terr=self.far_th
+        if not inj:
+            N_astro=self.N_astro_fhigh[str(int(fhigh))]
+        else:
+            N_astro=self.N_inj_fhigh[str(int(fhigh))]
+        
+        pastro=N_astro*f_over_b/(N_terr+N_astro*f_over_b)
+        p_astro={'BNS':pastro,'BBH':0.,'NSBH':0.,'Terrestrial':1-pastro}
+
+        return json.dumps(p_astro)
+
+    def prior(self, p=None):
+        pass
+
+    def finalize(self, prior=None):
+        pass
+    
+    def to_h5(self,filename):
+        
+        with h5py.File(filename,'w') as hf:
+            # FIXME not elegant
+            hf.attrs['model'] = 2
+            N_astro_fhigh = hf.create_group('N_astro_fhigh')
+
+            for fhigh,N in self.N_astro_fhigh.items():
+                N_astro_fhigh.create_dataset(fhigh,data=np.array([N]))
+            
+            N_inj_fhigh = hf.create_group('N_inj_fhigh')
+
+            for fhigh,N in self.N_inj_fhigh.items():
+                N_inj_fhigh.create_dataset(fhigh,data=np.array([N]))
+
+            
+            hf.create_dataset('A',data=np.array([self.A]))
+
+            hf.create_dataset('N_astro_1024',data=np.array([self.N_astro_1024]))
+            
+            hf.create_dataset('N_inj_1024',data=np.array([self.N_inj_1024]))
+
+            hf.create_dataset('far_th',data=np.array([self.far_th]))
+
+            hf.close()
         
     @classmethod
     def from_h5(cls,filename):
-        
         self=cls.__new__(cls)
-        hf=h5py.File(filename,'r')
+        with h5py.File(filename,'r') as hf:
         
-        coefficients=hf['coefficients']
-        coeff={}
-        for c in list(coefficients.keys()):
-            coeff[c]=coefficients[c][()].astype(np.float16)
-        self.template_weight_coefficients=coeff
-        self.categories=list(coeff.keys())
-        self.template_weight_SNR=hf['SNR'][()].astype(np.float16)
-        
-        self.A=hf['A'][()][0]
-        
-        
-        self.rates={}
-        rates=hf['rates']
-        for c in list(rates.keys()):
-            self.rates[c]=rates[c][()][0]
-        
-        self.rates_inj={}
-        rates_inj=hf['rates_inj']
-        for c in list(rates_inj.keys()):
-            self.rates_inj[c]=rates_inj[c][()][0]
-        
-        self.V={}
-        V=hf['V']
-        for c in list(V.keys()):
-            self.V[c]=V[c][()][0]
+            N_astro_fhigh = hf['N_astro_fhigh']
+            self.N_astro_fhigh={}
+            for fhigh in list(N_astro_fhigh.keys()):
+                self.N_astro_fhigh[fhigh]=N_astro_fhigh[fhigh][()][0]
+                
+            N_inj_fhigh = hf['N_inj_fhigh']
+            self.N_inj_fhigh={}
+            for fhigh in list(N_inj_fhigh.keys()):
+                self.N_inj_fhigh[fhigh]=N_inj_fhigh[fhigh][()][0]
+
+            self.A = hf['A'][()][0]
+
+            self.N_astro_1024 = hf['N_astro_1024'][()][0]
+            
+            self.N_inj_1024 = hf['N_inj_1024'][()][0]
+            
+            self.far_th = hf['far_th'][()][0]
+
+            hf.close()
         
-        self.far_th=hf['far_th'][()][0]
+        return self
+
+class p_astro_ssm(object):
+    
+    def __init__(self,N_astro=1.,Far_th_new_per_year=8760,T_run_year=1,rankstatpdf_file=None):
         
-        self.counts={c:self.rates[c]*self.V[c] for c in self.categories}
-        self.counts_inj={c:self.rates_inj[c]*self.V[c] for c in self.categories}
-        self.counts['Terr']=self.far_th
-        self.counts_inj['Terr']=self.far_th
+        self.N_terr=Far_th_new_per_year*T_run_year
+        self.N_astro=1.
+        self.far_th= Far_th_new_per_year
+        if rankstatpdf_file is not None:
+            A,_,_,_,_=self.normalize_f_over_b(rankstatpdf_file,far_th=Far_th_new_per_year/3.154e+7)
+            self.A=A
+        else:
+            self.A=1.
         
-        self.indextoid=hf['indextoid'][()].astype(np.int32).tolist()
-        hf.close()
+    
+    def normalize_f_over_b(self,rankstatpdf_file,far_th=1/3.154e+7):
         
-        return self
+        rankingstatpdf = far.marginalize_pdf_urls([rankstatpdf_file], "RankingStatPDF", verbose=True)
+    
+        zero_lag_lr_lnpdf = rankingstatpdf.zero_lag_lr_lnpdf
+        zl = rankingstatpdf.zero_lag_lr_lnpdf.copy()
+        zl.array[:40] = 0.
+    
+        if not zl.array.any():
+            raise ValueError("zero-lag counts are all zero")
+        ln_likelihood_ratio_threshold, = zl.argmax()
+    
+    
+        rankingstatpdf = rankingstatpdf.new_with_extinction()
+        fapfar = far.FAPFAR(rankingstatpdf)
+        
+        
+        
+        xmin=max(fapfar.rank_from_far(self.far_th),ln_likelihood_ratio_threshold)
+    
+        rankingstatpdf.noise_lr_lnpdf.array[: rankingstatpdf.noise_lr_lnpdf.bins[0][xmin]]=0.
+        rankingstatpdf.noise_lr_lnpdf.normalize()
+        rankingstatpdf.signal_lr_lnpdf.array[: rankingstatpdf.signal_lr_lnpdf.bins[0][xmin]]=0.
+        rankingstatpdf.signal_lr_lnpdf.normalize()
+        rankingstatpdf.zero_lag_lr_lnpdf.array[:rankingstatpdf.zero_lag_lr_lnpdf.bins[0][xmin]]=0.
+        rankingstatpdf.zero_lag_lr_lnpdf.normalize()
+    
+    
+        noise_lr_lnpdf=rankingstatpdf.noise_lr_lnpdf.mkinterp()
+        lnb=np.vectorize(lambda x: noise_lr_lnpdf(x))
+    
+        B,dB=quad(lambda x: np.exp(lnb(x)),xmin,np.inf,limit=1000)
+    
+        A,dA=quad( lambda x : np.exp(x+lnb(x)-np.log(B)),xmin,np.inf,limit=1000)
+        
+        lnb=None
+        
+        return A,B, fapfar,rankingstatpdf,xmin
+    
+    
+    
+    def update_rankstatpdf(self,newrankstatpdffile=None):
+        if newrankstatpdffile is None:
+            pass
+        else:
+              A,B, fapfar,rankstatpdf,xmin=self.normalize_f_over_b(newrankstatpdffile)
+              far_th_file=fapfar.far_from_rank(xmin)
+              if self.far_th is None:
+                  self.far_th=far_th_file
+              self.A=A
+    
+    
+    def __call__(self, data,inj=False):
+        
+        rankstat = float(data['likelihood'])
+        f_over_b=np.exp(rankstat)/self.A
+        pastro=self.N_astro*f_over_b/(self.N_terr+self.N_astro*f_over_b)
+        p_astro={"BBH":pastro, "BNS":0.0, "NSBH":0.0, 'Terrestrial':1-pastro}
+
+        return json.dumps(p_astro)
+
+    def prior(self, p=None):
+        pass
+
+    def finalize(self, prior=None):
+        pass
+    
+    def to_h5(self,filename):
+        
+        with h5py.File(filename,'w') as hf:
+            # FIXME not elegant
+            hf.attrs['model'] = 3
+            hf.create_dataset('N_astro',data=np.array([self.N_astro]))
+
+            hf.create_dataset('N_terr',data=np.array([self.N_terr]))
+
+            hf.create_dataset('A',data=np.array([self.A]))
 
+            hf.create_dataset('far_th',data=np.array([self.far_th]))
+
+            hf.close()
+        
+    @classmethod
+    def from_h5(cls,filename):
+        self=cls.__new__(cls)
+        with h5py.File(filename,'r') as hf:
+        
+            self.N_astro = hf['N_astro'][()][0]
+
+            self.N_terr = hf['N_terr'][()][0]
+
+            self.A = hf['A'][()][0]
+
+            self.far_th = hf['far_th'][()][0]
+
+            hf.close()
+        
+        return self
+    
+    
 MODELS = {
           0: pastro_model(),
-          1: p_astro_fgmc()
+          1: p_astro_fgmc(),
+          2: p_astro_ew(),
+          3: p_astro_ssm(),
          }
 
 def load(fname):
-  f = h5py.File(fname)
-  return MODELS[f.attrs["model"]].from_h5(fname)
+  with h5py.File(fname,'r') as f:
+      model = f.attrs["model"]
+  return MODELS[model].from_h5(fname)
```

### Comparing `gwsci-pastro-0.0.3/setup.py` & `gwsci-pastro-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import glob
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="gwsci-pastro",
-  version="0.0.3",
+  version="1.0.0",
   author="Chad Hanna, Victoria Niu, Leo Tsukada, Anarya Ray",
   author_email="chad.hanna@ligo.org",
   description="Tools for calculating astrophysical probability of GW events",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://git.ligo.org/gstlal/pastro",
   packages=["pastro",],
```

