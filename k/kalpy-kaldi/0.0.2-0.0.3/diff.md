# Comparing `tmp/kalpy-kaldi-0.0.2.tar.gz` & `tmp/kalpy-kaldi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalpy-kaldi-0.0.2.tar", last modified: Wed May 31 22:04:43 2023, max compression
+gzip compressed data, was "kalpy-kaldi-0.0.3.tar", last modified: Wed May 31 22:48:36 2023, max compression
```

## Comparing `kalpy-kaldi-0.0.2.tar` & `kalpy-kaldi-0.0.3.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.311642 kalpy-kaldi-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.295641 kalpy-kaldi-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 22:04:43.311642 kalpy-kaldi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/_kalpy.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/extensions/chain/
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/chain/chain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/chain/pybind_chain.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/extensions/cudamatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/cudamatrix/cudamatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/cudamatrix/pybind_cudamatrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/extensions/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)    85592 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/decoder/decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/decoder/pybind_decoder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/extensions/feat/
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/feat/feat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/feat/pybind_feat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/fstext/
--rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/fstext/fstext.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/fstext/pybind_fstext.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)    53595 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/gmm/pybind_gmm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/hmm/
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/hmm/hmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/hmm/pybind_hmm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/itf/
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/itf/itf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/itf/pybind_itf.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/ivector/
--rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/ivector/ivector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/ivector/pybind_ivector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/kws/
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/kws/kws.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/kws/pybind_kws.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/lat/
--rw-r--r--   0 runner    (1001) docker     (123)    63318 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/lat/lat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/lat/pybind_lat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/lm/
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/lm/lm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/lm/pybind_lm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/matrix/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/matrix/pybind_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/nnet/
--rw-r--r--   0 runner    (1001) docker     (123)    78126 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/nnet/nnet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/nnet/pybind_nnet.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/nnet2/
--rw-r--r--   0 runner    (1001) docker     (123)   122159 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/nnet2/nnet2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/nnet2/pybind_nnet2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/nnet3/
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/nnet3/nnet3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/nnet3/pybind_nnet3.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/online/
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/online/online.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/online/pybind_online.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/online2/
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/online2/online2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/online2/pybind_online2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/pybind/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/pybind/kaldi_pybind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.303641 kalpy-kaldi-0.0.2/extensions/rnnlm/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/rnnlm/pybind_rnnlm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/rnnlm/rnnlm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/extensions/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/transform/pybind_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)    39892 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/transform/transform.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/extensions/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/tree/pybind_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    52278 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/tree/tree.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/extensions/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/util/pybind_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/extensions/util/util.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/kalpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 22:04:43.000000 kalpy-kaldi-0.0.2/kalpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/kalpy/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/decoder/training_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/kalpy/feat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/feat/mfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/kalpy/fstext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/fstext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/fstext/lexicon.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/kalpy/fstext/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 22:04:43.000000 kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-31 22:04:43.000000 kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:04:43.000000 kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:04:43.000000 kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 22:04:43.000000 kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 22:04:43.000000 kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:04:43.311642 kalpy-kaldi-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.299641 kalpy-kaldi-0.0.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/tests/data/acoustic_models/
--rw-r--r--   0 runner    (1001) docker     (123)    55713 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/data/acoustic_models/final.mdl
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/data/acoustic_models/tree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/tests/data/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/data/dictionaries/test_basic.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:04:43.307641 kalpy-kaldi-0.0.2/tests/data/wav/
--rw-r--r--   0 runner    (1001) docker     (123)   855188 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/data/wav/acoustic_corpus.wav
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/test_hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/test_mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 22:04:22.000000 kalpy-kaldi-0.0.2/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.578258 kalpy-kaldi-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/_kalpy.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/chain/
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/chain/chain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/chain/pybind_chain.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/cudamatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/cudamatrix/cudamatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/cudamatrix/pybind_cudamatrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)    85592 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/decoder/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/decoder/pybind_decoder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/extensions/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/feat/feat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/feat/pybind_feat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/fstext/
+-rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/fstext/fstext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/fstext/pybind_fstext.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)    53595 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/gmm/pybind_gmm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/hmm/hmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/hmm/pybind_hmm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/itf/
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/itf/itf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/itf/pybind_itf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/ivector/
+-rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/ivector/ivector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/ivector/pybind_ivector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/kws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/kws/kws.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/kws/pybind_kws.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/lat/
+-rw-r--r--   0 runner    (1001) docker     (123)    63318 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lat/lat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lat/pybind_lat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lm/lm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/lm/pybind_lm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/matrix/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/matrix/pybind_matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/nnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    78126 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet/nnet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet/pybind_nnet.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/nnet2/
+-rw-r--r--   0 runner    (1001) docker     (123)   122159 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet2/nnet2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet2/pybind_nnet2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/nnet3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet3/nnet3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/nnet3/pybind_nnet3.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/online/
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online/online.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online/pybind_online.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.586258 kalpy-kaldi-0.0.3/extensions/online2/
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online2/online2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/online2/pybind_online2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/pybind/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/pybind/kaldi_pybind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/rnnlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/rnnlm/pybind_rnnlm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/rnnlm/rnnlm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/transform/pybind_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39892 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/transform/transform.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/tree/pybind_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52278 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/tree/tree.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/extensions/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/util/pybind_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/extensions/util/util.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/decoder/training_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/feat/mfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy/fstext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/fstext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/fstext/lexicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/kalpy/fstext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 22:48:36.000000 kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.590258 kalpy-kaldi-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.582258 kalpy-kaldi-0.0.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/tests/data/acoustic_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    55713 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/acoustic_models/final.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/acoustic_models/tree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/tests/data/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/dictionaries/test_basic.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:48:36.594258 kalpy-kaldi-0.0.3/tests/data/wav/
+-rw-r--r--   0 runner    (1001) docker     (123)   855188 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/data/wav/acoustic_corpus.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 22:48:20.000000 kalpy-kaldi-0.0.3/tests/test_tree.py
```

### Comparing `kalpy-kaldi-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md` & `kalpy-kaldi-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/.github/workflows/main.yml` & `kalpy-kaldi-0.0.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/.github/workflows/publish.yml` & `kalpy-kaldi-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/.gitignore` & `kalpy-kaldi-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/.pre-commit-config.yaml` & `kalpy-kaldi-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/CMakeLists.txt` & `kalpy-kaldi-0.0.3/CMakeLists.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,15 @@
                             extensions/nnet3/nnet3.cpp
                             extensions/transform/transform.cpp
                             extensions/tree/tree.cpp
                             extensions/util/util.cpp
                             )
 target_link_libraries(_kalpy PUBLIC kaldi-base kaldi-chain
                                     kaldi-matrix
+                                    kaldi-cudamatrix
                                     kaldi-hmm
                                     kaldi-online kaldi-online2 kaldi-rnnlm
                                     kaldi-nnet3
                                     kaldi-nnet2 kaldi-nnet
                                     kaldi-kws
                                     kaldi-decoder
                                     kaldi-lat
@@ -106,15 +107,14 @@
                                     kaldi-util
                                     fst
                                     )
 
 if(CUDA_FOUND)
 
 target_link_libraries(_kalpy PUBLIC kaldi-cudadecoder kaldi-cudafeat
-                                    kaldi-cudamatrix
                                     )
 endif()
 target_compile_definitions(_kalpy
                            PRIVATE VERSION_INFO="5.5.1068")
 if(MSVC)
 set_target_properties(_kalpy PROPERTIES
     DEFINE_SYMBOL "KALDI_DLL_IMPORTS"
```

### Comparing `kalpy-kaldi-0.0.2/LICENSE` & `kalpy-kaldi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/PKG-INFO` & `kalpy-kaldi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalpy-kaldi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pybind11 bindings for Kaldi for use with the Montreal Forced Aligner
 Author: Michael McAuliffe
 Author-email: michael.e.mcauliffe@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `kalpy-kaldi-0.0.2/README.md` & `kalpy-kaldi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/_kalpy.cpp` & `kalpy-kaldi-0.0.3/extensions/_kalpy.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/chain/chain.cpp` & `kalpy-kaldi-0.0.3/extensions/chain/chain.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/chain/pybind_chain.h` & `kalpy-kaldi-0.0.3/extensions/chain/pybind_chain.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/cudamatrix/cudamatrix.cpp` & `kalpy-kaldi-0.0.3/extensions/cudamatrix/cudamatrix.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/decoder/decoder.cpp` & `kalpy-kaldi-0.0.3/extensions/decoder/decoder.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/decoder/pybind_decoder.h` & `kalpy-kaldi-0.0.3/extensions/decoder/pybind_decoder.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/feat/feat.cpp` & `kalpy-kaldi-0.0.3/extensions/feat/feat.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/fstext/fstext.cpp` & `kalpy-kaldi-0.0.3/extensions/fstext/fstext.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/fstext/pybind_fstext.h` & `kalpy-kaldi-0.0.3/extensions/fstext/pybind_fstext.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/gmm/gmm.cpp` & `kalpy-kaldi-0.0.3/extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/gmm/pybind_gmm.h` & `kalpy-kaldi-0.0.3/extensions/gmm/pybind_gmm.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/hmm/hmm.cpp` & `kalpy-kaldi-0.0.3/extensions/hmm/hmm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/itf/itf.cpp` & `kalpy-kaldi-0.0.3/extensions/itf/itf.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/ivector/ivector.cpp` & `kalpy-kaldi-0.0.3/extensions/ivector/ivector.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/kws/kws.cpp` & `kalpy-kaldi-0.0.3/extensions/kws/kws.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/lat/lat.cpp` & `kalpy-kaldi-0.0.3/extensions/lat/lat.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/lat/pybind_lat.h` & `kalpy-kaldi-0.0.3/extensions/lat/pybind_lat.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/lm/lm.cpp` & `kalpy-kaldi-0.0.3/extensions/lm/lm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/matrix/matrix.cpp` & `kalpy-kaldi-0.0.3/extensions/matrix/matrix.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/nnet/nnet.cpp` & `kalpy-kaldi-0.0.3/extensions/nnet/nnet.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/nnet/pybind_nnet.h` & `kalpy-kaldi-0.0.3/extensions/nnet/pybind_nnet.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/nnet2/nnet2.cpp` & `kalpy-kaldi-0.0.3/extensions/nnet2/nnet2.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/nnet2/pybind_nnet2.h` & `kalpy-kaldi-0.0.3/extensions/nnet2/pybind_nnet2.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/nnet3/nnet3.cpp` & `kalpy-kaldi-0.0.3/extensions/nnet3/nnet3.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/nnet3/pybind_nnet3.h` & `kalpy-kaldi-0.0.3/extensions/nnet3/pybind_nnet3.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/online/online.cpp` & `kalpy-kaldi-0.0.3/extensions/online/online.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/online2/online2.cpp` & `kalpy-kaldi-0.0.3/extensions/online2/online2.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/online2/pybind_online2.h` & `kalpy-kaldi-0.0.3/extensions/online2/pybind_online2.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/pybind/kaldi_pybind.h` & `kalpy-kaldi-0.0.3/extensions/pybind/kaldi_pybind.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/rnnlm/pybind_rnnlm.h` & `kalpy-kaldi-0.0.3/extensions/rnnlm/pybind_rnnlm.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/rnnlm/rnnlm.cpp` & `kalpy-kaldi-0.0.3/extensions/rnnlm/rnnlm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/transform/pybind_transform.h` & `kalpy-kaldi-0.0.3/extensions/transform/pybind_transform.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/transform/transform.cpp` & `kalpy-kaldi-0.0.3/extensions/transform/transform.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/tree/tree.cpp` & `kalpy-kaldi-0.0.3/extensions/tree/tree.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/util/pybind_util.h` & `kalpy-kaldi-0.0.3/extensions/util/pybind_util.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/extensions/util/util.cpp` & `kalpy-kaldi-0.0.3/extensions/util/util.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/kalpy/decoder/training_graphs.py` & `kalpy-kaldi-0.0.3/kalpy/decoder/training_graphs.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/kalpy/feat/mfcc.py` & `kalpy-kaldi-0.0.3/kalpy/feat/mfcc.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/kalpy/fstext/lexicon.py` & `kalpy-kaldi-0.0.3/kalpy/fstext/lexicon.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/kalpy/fstext/utils.py` & `kalpy-kaldi-0.0.3/kalpy/fstext/utils.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/PKG-INFO` & `kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kalpy-kaldi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pybind11 bindings for Kaldi for use with the Montreal Forced Aligner
 Author: Michael McAuliffe
 Author-email: michael.e.mcauliffe@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `kalpy-kaldi-0.0.2/kalpy_kaldi.egg-info/SOURCES.txt` & `kalpy-kaldi-0.0.3/kalpy_kaldi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/pyproject.toml` & `kalpy-kaldi-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/setup.py` & `kalpy-kaldi-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/tests/conftest.py` & `kalpy-kaldi-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/tests/data/acoustic_models/final.mdl` & `kalpy-kaldi-0.0.3/tests/data/acoustic_models/final.mdl`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/tests/data/acoustic_models/tree` & `kalpy-kaldi-0.0.3/tests/data/acoustic_models/tree`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/tests/data/dictionaries/test_basic.txt` & `kalpy-kaldi-0.0.3/tests/data/dictionaries/test_basic.txt`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/tests/data/wav/acoustic_corpus.wav` & `kalpy-kaldi-0.0.3/tests/data/wav/acoustic_corpus.wav`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/tests/test_decoder.py` & `kalpy-kaldi-0.0.3/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.2/tests/test_mfcc.py` & `kalpy-kaldi-0.0.3/tests/test_mfcc.py`

 * *Files identical despite different names*

