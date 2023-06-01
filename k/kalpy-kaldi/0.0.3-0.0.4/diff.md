# Comparing `tmp/kalpy-kaldi-0.0.3.tar.gz` & `tmp/kalpy-kaldi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalpy-kaldi-0.0.3.tar", last modified: Wed May 31 22:48:36 2023, max compression
+gzip compressed data, was "kalpy-kaldi-0.0.4.tar", last modified: Thu Jun  1 21:15:47 2023, max compression
```

## Comparing `kalpy-kaldi-0.0.3.tar` & `kalpy-kaldi-0.0.4.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.578258 kalpy-kaldi-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/_kalpy.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/chain/
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/chain/chain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/chain/pybind_chain.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/cudamatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/cudamatrix/cudamatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/cudamatrix/pybind_cudamatrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)    85592 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/decoder/decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/decoder/pybind_decoder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/feat/
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/feat/feat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/feat/pybind_feat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/fstext/
--rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/fstext/fstext.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/fstext/pybind_fstext.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)    53595 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/gmm/pybind_gmm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/hmm/
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/hmm/hmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/hmm/pybind_hmm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/itf/
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/itf/itf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/itf/pybind_itf.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/ivector/
--rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/ivector/ivector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/ivector/pybind_ivector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/kws/
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/kws/kws.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/kws/pybind_kws.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/lat/
--rw-r--r--   0 runner    (1001) docker     (123)    63318 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lat/lat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lat/pybind_lat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/lm/
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lm/lm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lm/pybind_lm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/matrix/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/matrix/pybind_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/nnet/
--rw-r--r--   0 runner    (1001) docker     (123)    78126 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet/nnet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet/pybind_nnet.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/nnet2/
--rw-r--r--   0 runner    (1001) docker     (123)   122159 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet2/nnet2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet2/pybind_nnet2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/nnet3/
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet3/nnet3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet3/pybind_nnet3.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/online/
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online/online.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online/pybind_online.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/online2/
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online2/online2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online2/pybind_online2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/pybind/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/pybind/kaldi_pybind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/rnnlm/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/rnnlm/pybind_rnnlm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/rnnlm/rnnlm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/transform/pybind_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)    39892 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/transform/transform.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/tree/pybind_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    52278 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/tree/tree.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/util/pybind_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/util/util.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/decoder/training_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/feat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/feat/mfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/fstext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/fstext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/fstext/lexicon.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/fstext/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/tests/data/acoustic_models/
--rw-r--r--   0 runner    (1001) docker     (123)    55713 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/acoustic_models/final.mdl
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/acoustic_models/tree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/tests/data/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/dictionaries/test_basic.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/tests/data/wav/
--rw-r--r--   0 runner    (1001) docker     (123)   855188 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/wav/acoustic_corpus.wav
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.901612 kalpy-kaldi-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/_kalpy.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/chain/
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/chain/chain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/chain/pybind_chain.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/cudamatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/cudamatrix/cudamatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/cudamatrix/pybind_cudamatrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)    85592 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/decoder/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/decoder/pybind_decoder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/feat/feat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/feat/pybind_feat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/fstext/
+-rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/fstext/fstext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/fstext/pybind_fstext.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)    53595 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/gmm/pybind_gmm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/hmm/hmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/hmm/pybind_hmm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/itf/
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/itf/itf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/itf/pybind_itf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/ivector/
+-rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/ivector/ivector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/ivector/pybind_ivector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.909612 kalpy-kaldi-0.0.4/extensions/kws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/kws/kws.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/kws/pybind_kws.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/lat/
+-rw-r--r--   0 runner    (1001) docker     (123)    63329 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/lat/lat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/lat/pybind_lat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/lm/lm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/lm/pybind_lm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/matrix/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/matrix/pybind_matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/nnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    78126 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/nnet/nnet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/nnet/pybind_nnet.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/nnet2/
+-rw-r--r--   0 runner    (1001) docker     (123)   122159 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/nnet2/nnet2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/nnet2/pybind_nnet2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/nnet3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/nnet3/nnet3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/nnet3/pybind_nnet3.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/online/
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/online/online.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/online/pybind_online.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/online2/
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/online2/online2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/online2/pybind_online2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/pybind/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/pybind/kaldi_pybind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/rnnlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/rnnlm/pybind_rnnlm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/rnnlm/rnnlm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/transform/pybind_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39892 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/transform/transform.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/tree/pybind_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52285 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/tree/tree.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/extensions/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/util/pybind_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/extensions/util/util.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/kalpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 21:15:47.000000 kalpy-kaldi-0.0.4/kalpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/kalpy/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/decoder/training_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.913612 kalpy-kaldi-0.0.4/kalpy/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/feat/mfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/kalpy/fstext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/fstext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/fstext/lexicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/kalpy/fstext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-01 21:15:47.000000 kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-01 21:15:47.000000 kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:15:47.000000 kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:15:47.000000 kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 21:15:47.000000 kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 21:15:47.000000 kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.905612 kalpy-kaldi-0.0.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/tests/data/acoustic_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    55713 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/data/acoustic_models/final.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/data/acoustic_models/tree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/tests/data/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/data/dictionaries/test_basic.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:15:47.917612 kalpy-kaldi-0.0.4/tests/data/wav/
+-rw-r--r--   0 runner    (1001) docker     (123)   855188 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/data/wav/acoustic_corpus.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/test_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/test_mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 21:15:32.000000 kalpy-kaldi-0.0.4/tests/test_tree.py
```

### Comparing `kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `kalpy-kaldi-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `kalpy-kaldi-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/.github/workflows/main.yml` & `kalpy-kaldi-0.0.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/.github/workflows/publish.yml` & `kalpy-kaldi-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/.gitignore` & `kalpy-kaldi-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/.pre-commit-config.yaml` & `kalpy-kaldi-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/CMakeLists.txt` & `kalpy-kaldi-0.0.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/LICENSE` & `kalpy-kaldi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/PKG-INFO` & `kalpy-kaldi-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalpy-kaldi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pybind11 bindings for Kaldi for use with the Montreal Forced Aligner
 Author: Michael McAuliffe
 Author-email: michael.e.mcauliffe@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `kalpy-kaldi-0.0.3/README.md` & `kalpy-kaldi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/_kalpy.cpp` & `kalpy-kaldi-0.0.4/extensions/_kalpy.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/chain/chain.cpp` & `kalpy-kaldi-0.0.4/extensions/chain/chain.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/chain/pybind_chain.h` & `kalpy-kaldi-0.0.4/extensions/chain/pybind_chain.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/cudamatrix/cudamatrix.cpp` & `kalpy-kaldi-0.0.4/extensions/cudamatrix/cudamatrix.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/decoder/decoder.cpp` & `kalpy-kaldi-0.0.4/extensions/decoder/decoder.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/decoder/pybind_decoder.h` & `kalpy-kaldi-0.0.4/extensions/decoder/pybind_decoder.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/feat/feat.cpp` & `kalpy-kaldi-0.0.4/extensions/feat/feat.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/fstext/fstext.cpp` & `kalpy-kaldi-0.0.4/extensions/fstext/fstext.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/fstext/pybind_fstext.h` & `kalpy-kaldi-0.0.4/extensions/fstext/pybind_fstext.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/gmm/gmm.cpp` & `kalpy-kaldi-0.0.4/extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/gmm/pybind_gmm.h` & `kalpy-kaldi-0.0.4/extensions/gmm/pybind_gmm.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/hmm/hmm.cpp` & `kalpy-kaldi-0.0.4/extensions/hmm/hmm.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
       .def(py::init<const ContextDependencyInterface&, const HmmTopology&>(),
            "Initialize the object [e.g. at the start of training]. The class "
            "keeps a copy of the HmmTopology object, but not the "
            "ContextDependency object.",
            py::arg("ctx_dep"), py::arg("hmm_topo"))
      .def_static("read_from_file", [](std::string file_path) {
 
-               TransitionModel trans_model;
+               static TransitionModel trans_model;
                ReadKaldiObject(file_path, &trans_model);
                return &trans_model;
           }, py::return_value_policy::reference)
       .def("Read", &PyClass::Read, py::arg("is"), py::arg("binary"))
       .def("Write", &PyClass::Write, py::arg("os"), py::arg("binary"))
       .def("GetTopo", &PyClass::GetTopo, py::return_value_policy::reference)
       .def("TupleToTransitionState", &PyClass::TupleToTransitionState,
```

### Comparing `kalpy-kaldi-0.0.3/extensions/itf/itf.cpp` & `kalpy-kaldi-0.0.4/extensions/itf/itf.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/ivector/ivector.cpp` & `kalpy-kaldi-0.0.4/extensions/ivector/ivector.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/kws/kws.cpp` & `kalpy-kaldi-0.0.4/extensions/kws/kws.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/lat/lat.cpp` & `kalpy-kaldi-0.0.4/extensions/lat/lat.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1047,25 +1047,26 @@
         "determinization in general, but for deeper lattices it is a bit faster, "
         "despite the fact that we now have two passes of determinization by default.",
         py::arg("trans_model"),
         py::arg("ifst"),
         py::arg("prune"),
         py::arg("ofst"),
         py::arg("opts")= DeterminizeLatticePhonePrunedOptions());
-  m.def("DeterminizeLatticeInsertPhones",
+  /*m.def("DeterminizeLatticeInsertPhones",
         &DeterminizeLatticeInsertPhones<kaldi::LatticeWeight>,
         "This function takes in lattices and inserts phones at phone boundaries. It "
         "uses the transition model to work out the transition_id to phone map. The "
         "returning value is the starting index of the phone label. Typically we pick "
         "(maximum_output_label_index + 1) as this value. The inserted phones are then "
         "mapped to (returning_value + original_phone_label) in the new lattice. The "
         "returning value will be used by DeterminizeLatticeDeletePhones() where it "
         "works out the phones according to this value.",
         py::arg("trans_model"),
         py::arg("fst"));
+      */
   m.def("DeterminizeLatticeDeletePhones",
         &DeterminizeLatticeDeletePhones<kaldi::LatticeWeight>,
         "This function takes in lattices and deletes \"phones\" from them. The \"phones\" "
         "here are actually any label that is larger than first_phone_label because "
         "when we insert phones into the lattice, we map the original phone label to "
         "(first_phone_label + original_phone_label). It is supposed to be used "
         "together with DeterminizeLatticeInsertPhones()",
```

### Comparing `kalpy-kaldi-0.0.3/extensions/lat/pybind_lat.h` & `kalpy-kaldi-0.0.4/extensions/lat/pybind_lat.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/lm/lm.cpp` & `kalpy-kaldi-0.0.4/extensions/lm/lm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/matrix/matrix.cpp` & `kalpy-kaldi-0.0.4/extensions/matrix/matrix.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/nnet/nnet.cpp` & `kalpy-kaldi-0.0.4/extensions/nnet/nnet.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/nnet/pybind_nnet.h` & `kalpy-kaldi-0.0.4/extensions/nnet/pybind_nnet.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/nnet2/nnet2.cpp` & `kalpy-kaldi-0.0.4/extensions/nnet2/nnet2.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/nnet2/pybind_nnet2.h` & `kalpy-kaldi-0.0.4/extensions/nnet2/pybind_nnet2.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/nnet3/nnet3.cpp` & `kalpy-kaldi-0.0.4/extensions/nnet3/nnet3.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/nnet3/pybind_nnet3.h` & `kalpy-kaldi-0.0.4/extensions/nnet3/pybind_nnet3.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/online/online.cpp` & `kalpy-kaldi-0.0.4/extensions/online/online.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/online2/online2.cpp` & `kalpy-kaldi-0.0.4/extensions/online2/online2.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/online2/pybind_online2.h` & `kalpy-kaldi-0.0.4/extensions/online2/pybind_online2.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/pybind/kaldi_pybind.h` & `kalpy-kaldi-0.0.4/extensions/pybind/kaldi_pybind.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/rnnlm/pybind_rnnlm.h` & `kalpy-kaldi-0.0.4/extensions/rnnlm/pybind_rnnlm.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/rnnlm/rnnlm.cpp` & `kalpy-kaldi-0.0.4/extensions/rnnlm/rnnlm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/transform/pybind_transform.h` & `kalpy-kaldi-0.0.4/extensions/transform/pybind_transform.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/transform/transform.cpp` & `kalpy-kaldi-0.0.4/extensions/transform/transform.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/tree/tree.cpp` & `kalpy-kaldi-0.0.4/extensions/tree/tree.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -984,15 +984,15 @@
         "of actually using them, we do not put any training code into the ContextDependency class.");
 
     context_dependency.def(py::init<>())
       .def(py::init<int32, int32, EventMap *>(), py::arg("N"),
            py::arg("P"), py::arg("to_pdf"))
         .def_static("read_from_file",[](const std::string file_path){
 
-                  ContextDependency ctx_dep;
+                  static ContextDependency ctx_dep;
                   ReadKaldiObject(file_path, &ctx_dep);
                   return &ctx_dep;
               }, py::arg("file_path"))
         .def("Read", &PyClass::Read, py::arg("is"), py::arg("binary"))
         .def("Write", &PyClass::Write, py::arg("os"), py::arg("binary"))
         .def("ContextWidth", &PyClass::ContextWidth)
         .def("CentralPosition", &PyClass::CentralPosition)
```

### Comparing `kalpy-kaldi-0.0.3/extensions/util/pybind_util.h` & `kalpy-kaldi-0.0.4/extensions/util/pybind_util.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/extensions/util/util.cpp` & `kalpy-kaldi-0.0.4/extensions/util/util.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/kalpy/decoder/training_graphs.py` & `kalpy-kaldi-0.0.4/kalpy/decoder/training_graphs.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/kalpy/feat/mfcc.py` & `kalpy-kaldi-0.0.4/kalpy/feat/mfcc.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/kalpy/fstext/lexicon.py` & `kalpy-kaldi-0.0.4/kalpy/fstext/lexicon.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/kalpy/fstext/utils.py` & `kalpy-kaldi-0.0.4/kalpy/fstext/utils.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/PKG-INFO` & `kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalpy-kaldi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pybind11 bindings for Kaldi for use with the Montreal Forced Aligner
 Author: Michael McAuliffe
 Author-email: michael.e.mcauliffe@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/SOURCES.txt` & `kalpy-kaldi-0.0.4/kalpy_kaldi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/pyproject.toml` & `kalpy-kaldi-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/setup.py` & `kalpy-kaldi-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/tests/conftest.py` & `kalpy-kaldi-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/tests/data/acoustic_models/final.mdl` & `kalpy-kaldi-0.0.4/tests/data/acoustic_models/final.mdl`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/tests/data/acoustic_models/tree` & `kalpy-kaldi-0.0.4/tests/data/acoustic_models/tree`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/tests/data/dictionaries/test_basic.txt` & `kalpy-kaldi-0.0.4/tests/data/dictionaries/test_basic.txt`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/tests/data/wav/acoustic_corpus.wav` & `kalpy-kaldi-0.0.4/tests/data/wav/acoustic_corpus.wav`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/tests/test_decoder.py` & `kalpy-kaldi-0.0.4/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.3/tests/test_mfcc.py` & `kalpy-kaldi-0.0.4/tests/test_mfcc.py`

 * *Files identical despite different names*

