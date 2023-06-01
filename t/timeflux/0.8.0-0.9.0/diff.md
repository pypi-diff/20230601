# Comparing `tmp/timeflux-0.8.0.tar.gz` & `tmp/timeflux-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeflux-0.8.0.tar", last modified: Thu Mar  4 15:34:59 2021, max compression
+gzip compressed data, was "timeflux-0.9.0.tar", last modified: Wed Mar 10 19:58:33 2021, max compression
```

## Comparing `timeflux-0.8.0.tar` & `timeflux-0.9.0.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.029953 timeflux-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.009953 timeflux-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (116)       58 2021-03-04 15:34:34.000000 timeflux-0.8.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.009953 timeflux-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1260 2021-03-04 15:34:34.000000 timeflux-0.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)      605 2021-03-04 15:34:34.000000 timeflux-0.8.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)      176 2021-03-04 15:34:34.000000 timeflux-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      205 2021-03-04 15:34:34.000000 timeflux-0.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     5221 2021-03-04 15:34:34.000000 timeflux-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)      488 2021-03-04 15:34:34.000000 timeflux-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)     1092 2021-03-04 15:34:34.000000 timeflux-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2385 2021-03-04 15:34:59.029953 timeflux-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1247 2021-03-04 15:34:34.000000 timeflux-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.009953 timeflux-0.8.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.009953 timeflux-0.8.0/doc/extending/
--rw-r--r--   0 runner    (1001) docker     (116)      607 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/extending/best_practices.rst
--rw-r--r--   0 runner    (1001) docker     (116)      527 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/extending/branches.rst
--rw-r--r--   0 runner    (1001) docker     (116)      670 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/extending/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.009953 timeflux-0.8.0/doc/general/
--rw-r--r--   0 runner    (1001) docker     (116)      915 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/general/about.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2953 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/general/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1239 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/general/getting_help.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2860 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.005953 timeflux-0.8.0/doc/static/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.009953 timeflux-0.8.0/doc/static/apps/
--rw-r--r--   0 runner    (1001) docker     (116)      530 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/apps/helloworld_1.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      528 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/apps/helloworld_2.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/apps/helloworld_3.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     2121 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/apps/neurofeedback.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.013953 timeflux-0.8.0/doc/static/img/
--rw-r--r--   0 runner    (1001) docker     (116)     5697 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/dag.png
--rw-r--r--   0 runner    (1001) docker     (116)     9227 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/email.png
--rw-r--r--   0 runner    (1001) docker     (116)    15406 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)    12087 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/helloworld_1.png
--rw-r--r--   0 runner    (1001) docker     (116)    21774 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/helloworld_2.png
--rw-r--r--   0 runner    (1001) docker     (116)    41932 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/helloworld_3.png
--rw-r--r--   0 runner    (1001) docker     (116)     7485 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (116)    26754 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/static/img/neurofeedback.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.013953 timeflux-0.8.0/doc/usage/
--rw-r--r--   0 runner    (1001) docker     (116)     5214 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/usage/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2759 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/usage/going_further.rst
--rw-r--r--   0 runner    (1001) docker     (116)     9162 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/usage/hello_world.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4445 2021-03-04 15:34:34.000000 timeflux-0.8.0/doc/usage/use_case.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.013953 timeflux-0.8.0/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      102 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/broker.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      474 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/epoch.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      770 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/hdf5_string.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       49 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/import.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      322 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/import2.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       39 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/import3.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      613 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/lsl.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     1379 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/lsl_multiple.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      729 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/osc.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      274 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/pub.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      521 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/replay.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      334 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/replay2.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      821 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/save.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      289 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/sub.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      469 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/test.json
--rw-r--r--   0 runner    (1001) docker     (116)      506 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/test.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      614 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/ui.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      462 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/window.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      725 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/zmq.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      899 2021-03-04 15:34:34.000000 timeflux-0.8.0/examples/zmq2.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      358 2021-03-04 15:34:34.000000 timeflux-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1595 2021-03-04 15:34:59.029953 timeflux-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      147 2021-03-04 15:34:34.000000 timeflux-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.013953 timeflux-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)      559 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.017953 timeflux-0.8.0/test/core/
--rw-r--r--   0 runner    (1001) docker     (116)     2569 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/core/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2871 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/core/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (116)     2985 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/core/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (116)      874 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/core/test_node.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/core/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1480 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/core/test_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.017953 timeflux-0.8.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (116)    29907 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/data/replay.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.017953 timeflux-0.8.0/test/graphs/
--rw-r--r--   0 runner    (1001) docker     (116)      102 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/broker.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       49 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/import.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      322 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/import2.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       39 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/import3.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      274 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/pub.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      289 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/sub.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       86 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/template.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      469 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/test.json
--rw-r--r--   0 runner    (1001) docker     (116)      506 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/graphs/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.017953 timeflux-0.8.0/test/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)     1124 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/helpers/test_background.py
--rw-r--r--   0 runner    (1001) docker     (116)     1513 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/helpers/test_mne.py
--rw-r--r--   0 runner    (1001) docker     (116)     1616 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/helpers/test_port.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.021953 timeflux-0.8.0/test/launcher/
--rw-r--r--   0 runner    (1001) docker     (116)      117 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/.env
--rw-r--r--   0 runner    (1001) docker     (116)      127 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/.env.alt
--rw-r--r--   0 runner    (1001) docker     (116)      526 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/dummy.py
--rw-r--r--   0 runner    (1001) docker     (116)      339 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/dummy_exception.py
--rw-r--r--   0 runner    (1001) docker     (116)     3689 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/launcher.py
--rw-r--r--   0 runner    (1001) docker     (116)       94 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/post.py
--rw-r--r--   0 runner    (1001) docker     (116)       99 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/post_exception.py
--rw-r--r--   0 runner    (1001) docker     (116)      252 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test.bat
--rwxr-xr-x   0 runner    (1001) docker     (116)      869 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test.sh
--rw-r--r--   0 runner    (1001) docker     (116)      146 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_1.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      183 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_2.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      238 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_3.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      275 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_4.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      288 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_5.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      221 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_6.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      260 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_7.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      303 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_8.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      275 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/launcher/test_9.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      204 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/lsl_api.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.021953 timeflux-0.8.0/test/nodes/
--rw-r--r--   0 runner    (1001) docker     (116)     2439 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_accumulate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1749 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (116)     1126 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_axis.py
--rw-r--r--   0 runner    (1001) docker     (116)     3424 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_dejitter.py
--rw-r--r--   0 runner    (1001) docker     (116)    11882 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_epoch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2808 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (116)     4971 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_gate.py
--rw-r--r--   0 runner    (1001) docker     (116)      973 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (116)    20549 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_ml.py
--rw-r--r--   0 runner    (1001) docker     (116)     2670 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_query.py
--rw-r--r--   0 runner    (1001) docker     (116)     2308 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/nodes/test_window.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.021953 timeflux-0.8.0/test/tools/
--rw-r--r--   0 runner    (1001) docker     (116)     1243 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (116)      936 2021-03-04 15:34:34.000000 timeflux-0.8.0/test/tools/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.021953 timeflux-0.8.0/timeflux/
--rw-r--r--   0 runner    (1001) docker     (116)      368 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      115 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.025953 timeflux-0.8.0/timeflux/core/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1939 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/branch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1378 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3068 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (116)      924 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/io.py
--rw-r--r--   0 runner    (1001) docker     (116)     3782 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (116)     5048 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     1179 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/message.py
--rw-r--r--   0 runner    (1001) docker     (116)     3830 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/node.py
--rw-r--r--   0 runner    (1001) docker     (116)      120 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (116)     2156 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (116)     2873 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     1964 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/validate.py
--rw-r--r--   0 runner    (1001) docker     (116)     3127 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/core/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.025953 timeflux-0.8.0/timeflux/estimators/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/estimators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.025953 timeflux-0.8.0/timeflux/estimators/classifiers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/estimators/classifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.025953 timeflux-0.8.0/timeflux/estimators/transformers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/estimators/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      956 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/estimators/transformers/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.025953 timeflux-0.8.0/timeflux/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4314 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/background.py
--rw-r--r--   0 runner    (1001) docker     (116)     1878 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/clock.py
--rw-r--r--   0 runner    (1001) docker     (116)     4378 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/handler.py
--rw-r--r--   0 runner    (1001) docker     (116)      307 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (116)      305 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/lsl.py
--rw-r--r--   0 runner    (1001) docker     (116)     5514 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/mne.py
--rw-r--r--   0 runner    (1001) docker     (116)     1796 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/port.py
--rw-r--r--   0 runner    (1001) docker     (116)     5655 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/testing.py
--rw-r--r--   0 runner    (1001) docker     (116)     4806 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/helpers/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.029953 timeflux-0.8.0/timeflux/nodes/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3878 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/accumulate.py
--rw-r--r--   0 runner    (1001) docker     (116)     5811 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/apply.py
--rw-r--r--   0 runner    (1001) docker     (116)     2158 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/axis.py
--rw-r--r--   0 runner    (1001) docker     (116)      794 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/debug.py
--rw-r--r--   0 runner    (1001) docker     (116)     5396 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/dejitter.py
--rw-r--r--   0 runner    (1001) docker     (116)     9805 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/epoch.py
--rw-r--r--   0 runner    (1001) docker     (116)     4951 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/events.py
--rw-r--r--   0 runner    (1001) docker     (116)     4843 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/expression.py
--rw-r--r--   0 runner    (1001) docker     (116)     4013 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/gate.py
--rw-r--r--   0 runner    (1001) docker     (116)     7527 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (116)     6310 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/lsl.py
--rw-r--r--   0 runner    (1001) docker     (116)    17358 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/ml.py
--rw-r--r--   0 runner    (1001) docker     (116)      291 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/monitor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2294 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/osc.py
--rw-r--r--   0 runner    (1001) docker     (116)     8211 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/query.py
--rw-r--r--   0 runner    (1001) docker     (116)      944 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/random.py
--rw-r--r--   0 runner    (1001) docker     (116)      282 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/sequence.py
--rw-r--r--   0 runner    (1001) docker     (116)     3855 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/window.py
--rw-r--r--   0 runner    (1001) docker     (116)     1905 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/xarray.py
--rw-r--r--   0 runner    (1001) docker     (116)     8334 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/nodes/zmq.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.029953 timeflux-0.8.0/timeflux/schema/
--rw-r--r--   0 runner    (1001) docker     (116)     3082 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/schema/app.json
--rw-r--r--   0 runner    (1001) docker     (116)     2241 2021-03-04 15:34:34.000000 timeflux-0.8.0/timeflux/timeflux.py
--rw-r--r--   0 runner    (1001) docker     (116)      142 2021-03-04 15:34:58.000000 timeflux-0.8.0/timeflux/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-04 15:34:59.021953 timeflux-0.8.0/timeflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2385 2021-03-04 15:34:58.000000 timeflux-0.8.0/timeflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4118 2021-03-04 15:34:58.000000 timeflux-0.8.0/timeflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-04 15:34:58.000000 timeflux-0.8.0/timeflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       53 2021-03-04 15:34:58.000000 timeflux-0.8.0/timeflux.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      341 2021-03-04 15:34:58.000000 timeflux-0.8.0/timeflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-03-04 15:34:58.000000 timeflux-0.8.0/timeflux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.552186 timeflux-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.532186 timeflux-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2021-03-10 19:58:08.000000 timeflux-0.9.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.532186 timeflux-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1260 2021-03-10 19:58:08.000000 timeflux-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      605 2021-03-10 19:58:08.000000 timeflux-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      176 2021-03-10 19:58:08.000000 timeflux-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      205 2021-03-10 19:58:08.000000 timeflux-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     5221 2021-03-10 19:58:08.000000 timeflux-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)      488 2021-03-10 19:58:08.000000 timeflux-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1092 2021-03-10 19:58:08.000000 timeflux-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     2385 2021-03-10 19:58:33.552186 timeflux-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1247 2021-03-10 19:58:08.000000 timeflux-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.532186 timeflux-0.9.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.532186 timeflux-0.9.0/doc/extending/
+-rw-r--r--   0 runner    (1001) docker     (116)      607 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/extending/best_practices.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      527 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/extending/branches.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      670 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/extending/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.532186 timeflux-0.9.0/doc/general/
+-rw-r--r--   0 runner    (1001) docker     (116)      915 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/general/about.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2953 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/general/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1239 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/general/getting_help.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2860 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.532186 timeflux-0.9.0/doc/static/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.532186 timeflux-0.9.0/doc/static/apps/
+-rw-r--r--   0 runner    (1001) docker     (116)      530 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/apps/helloworld_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      528 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/apps/helloworld_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1053 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/apps/helloworld_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     2121 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/apps/neurofeedback.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.536186 timeflux-0.9.0/doc/static/img/
+-rw-r--r--   0 runner    (1001) docker     (116)     5697 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/dag.png
+-rw-r--r--   0 runner    (1001) docker     (116)     9227 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/email.png
+-rw-r--r--   0 runner    (1001) docker     (116)    15406 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (116)    12087 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/helloworld_1.png
+-rw-r--r--   0 runner    (1001) docker     (116)    21774 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/helloworld_2.png
+-rw-r--r--   0 runner    (1001) docker     (116)    41932 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/helloworld_3.png
+-rw-r--r--   0 runner    (1001) docker     (116)     7485 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (116)    26754 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/static/img/neurofeedback.png
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.536186 timeflux-0.9.0/doc/usage/
+-rw-r--r--   0 runner    (1001) docker     (116)     5214 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/usage/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2759 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/usage/going_further.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     9162 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/usage/hello_world.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4445 2021-03-10 19:58:08.000000 timeflux-0.9.0/doc/usage/use_case.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.536186 timeflux-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/broker.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      474 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/epoch.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      770 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/hdf5_string.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/import.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      322 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/import2.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/import3.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      613 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/lsl.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1379 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/lsl_multiple.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      729 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/osc.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      274 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/pub.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      521 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/replay.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      334 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/replay2.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      821 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/save.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      289 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/sub.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      469 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/test.json
+-rw-r--r--   0 runner    (1001) docker     (116)      506 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      614 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/ui.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      462 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/window.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      725 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/zmq.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      899 2021-03-10 19:58:08.000000 timeflux-0.9.0/examples/zmq2.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      358 2021-03-10 19:58:08.000000 timeflux-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     1612 2021-03-10 19:58:33.552186 timeflux-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      147 2021-03-10 19:58:08.000000 timeflux-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.536186 timeflux-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (116)      559 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.536186 timeflux-0.9.0/test/core/
+-rw-r--r--   0 runner    (1001) docker     (116)     2569 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/core/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2871 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/core/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2985 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/core/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)      874 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/core/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/core/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1480 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/core/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.536186 timeflux-0.9.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (116)    29907 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/data/replay.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.540186 timeflux-0.9.0/test/graphs/
+-rw-r--r--   0 runner    (1001) docker     (116)      102 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/broker.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/import.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      322 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/import2.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       39 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/import3.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      274 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/pub.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      289 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/sub.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)       86 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/template.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      469 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/test.json
+-rw-r--r--   0 runner    (1001) docker     (116)      506 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/graphs/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.540186 timeflux-0.9.0/test/helpers/
+-rw-r--r--   0 runner    (1001) docker     (116)     1497 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/helpers/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1513 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/helpers/test_mne.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1616 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/helpers/test_port.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.540186 timeflux-0.9.0/test/launcher/
+-rw-r--r--   0 runner    (1001) docker     (116)      117 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/.env
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/.env.alt
+-rw-r--r--   0 runner    (1001) docker     (116)      526 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (116)      339 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/dummy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3689 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (116)       94 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/post.py
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/post_exception.py
+-rw-r--r--   0 runner    (1001) docker     (116)      252 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test.bat
+-rwxr-xr-x   0 runner    (1001) docker     (116)      869 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test.sh
+-rw-r--r--   0 runner    (1001) docker     (116)      146 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      238 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      275 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_4.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      288 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_5.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      221 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_6.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      260 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_7.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      303 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_8.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      275 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/launcher/test_9.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      222 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/lsl_api.cfg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.544186 timeflux-0.9.0/test/nodes/
+-rw-r--r--   0 runner    (1001) docker     (116)     2439 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1749 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1126 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_axis.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3424 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_dejitter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11882 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_epoch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2808 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4971 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_gate.py
+-rw-r--r--   0 runner    (1001) docker     (116)      973 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    21062 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_ml.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2670 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2308 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/nodes/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.544186 timeflux-0.9.0/test/tools/
+-rw-r--r--   0 runner    (1001) docker     (116)     1243 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (116)      936 2021-03-10 19:58:08.000000 timeflux-0.9.0/test/tools/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.544186 timeflux-0.9.0/timeflux/
+-rw-r--r--   0 runner    (1001) docker     (116)      368 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      115 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.544186 timeflux-0.9.0/timeflux/core/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1939 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/branch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1378 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3068 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (116)      924 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/io.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3782 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5048 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1179 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3830 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (116)      120 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2156 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2873 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1964 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/validate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3127 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/core/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.548186 timeflux-0.9.0/timeflux/estimators/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/estimators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.548186 timeflux-0.9.0/timeflux/estimators/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/estimators/classifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.548186 timeflux-0.9.0/timeflux/estimators/transformers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/estimators/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      956 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/estimators/transformers/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.548186 timeflux-0.9.0/timeflux/helpers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4314 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/background.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1878 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/clock.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4378 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)      307 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (116)      305 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/lsl.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5514 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/mne.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1796 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/port.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5655 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/testing.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4806 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/helpers/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.552186 timeflux-0.9.0/timeflux/nodes/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3878 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5811 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/apply.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2158 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/axis.py
+-rw-r--r--   0 runner    (1001) docker     (116)      794 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/debug.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5396 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/dejitter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9805 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4951 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/events.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4843 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/expression.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4013 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/gate.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7527 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6310 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/lsl.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17728 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/ml.py
+-rw-r--r--   0 runner    (1001) docker     (116)      291 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2294 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/osc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8211 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/query.py
+-rw-r--r--   0 runner    (1001) docker     (116)      944 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/random.py
+-rw-r--r--   0 runner    (1001) docker     (116)      282 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3855 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/window.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1905 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8334 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/nodes/zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.552186 timeflux-0.9.0/timeflux/schema/
+-rw-r--r--   0 runner    (1001) docker     (116)     3082 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/schema/app.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2241 2021-03-10 19:58:08.000000 timeflux-0.9.0/timeflux/timeflux.py
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2021-03-10 19:58:33.000000 timeflux-0.9.0/timeflux/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:58:33.544186 timeflux-0.9.0/timeflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2385 2021-03-10 19:58:33.000000 timeflux-0.9.0/timeflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4118 2021-03-10 19:58:33.000000 timeflux-0.9.0/timeflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-10 19:58:33.000000 timeflux-0.9.0/timeflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2021-03-10 19:58:33.000000 timeflux-0.9.0/timeflux.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      357 2021-03-10 19:58:33.000000 timeflux-0.9.0/timeflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2021-03-10 19:58:33.000000 timeflux-0.9.0/timeflux.egg-info/top_level.txt
```

### Comparing `timeflux-0.8.0/.github/workflows/build.yml` & `timeflux-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/.github/workflows/publish.yml` & `timeflux-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/CODE_OF_CONDUCT.md` & `timeflux-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/LICENSE` & `timeflux-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/PKG-INFO` & `timeflux-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeflux
-Version: 0.8.0
+Version: 0.9.0
 Summary: Acquisition and real-time processing of biosignals
 Home-page: https://timeflux.io
 Author: Pierre Clisson
 Author-email: contact@timeflux.io
 License: MIT
 Project-URL: Documentation, https://doc.timeflux.io
 Project-URL: Source Code, https://github.com/timeflux/timeflux
```

### Comparing `timeflux-0.8.0/README.rst` & `timeflux-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/extending/best_practices.rst` & `timeflux-0.9.0/doc/extending/best_practices.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/extending/branches.rst` & `timeflux-0.9.0/doc/extending/branches.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/extending/plugins.rst` & `timeflux-0.9.0/doc/extending/plugins.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/general/about.rst` & `timeflux-0.9.0/doc/general/about.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/general/concepts.rst` & `timeflux-0.9.0/doc/general/concepts.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/general/getting_help.rst` & `timeflux-0.9.0/doc/general/getting_help.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/index.rst` & `timeflux-0.9.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/apps/helloworld_1.yaml` & `timeflux-0.9.0/doc/static/apps/helloworld_1.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/apps/helloworld_2.yaml` & `timeflux-0.9.0/doc/static/apps/helloworld_2.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/apps/helloworld_3.yaml` & `timeflux-0.9.0/doc/static/apps/helloworld_3.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/apps/neurofeedback.yaml` & `timeflux-0.9.0/doc/static/apps/neurofeedback.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/dag.png` & `timeflux-0.9.0/doc/static/img/dag.png`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/email.png` & `timeflux-0.9.0/doc/static/img/email.png`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/favicon.ico` & `timeflux-0.9.0/doc/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/helloworld_1.png` & `timeflux-0.9.0/doc/static/img/helloworld_1.png`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/helloworld_2.png` & `timeflux-0.9.0/doc/static/img/helloworld_2.png`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/helloworld_3.png` & `timeflux-0.9.0/doc/static/img/helloworld_3.png`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/logo.png` & `timeflux-0.9.0/doc/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/static/img/neurofeedback.png` & `timeflux-0.9.0/doc/static/img/neurofeedback.png`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/usage/getting_started.rst` & `timeflux-0.9.0/doc/usage/getting_started.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/usage/going_further.rst` & `timeflux-0.9.0/doc/usage/going_further.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/usage/hello_world.rst` & `timeflux-0.9.0/doc/usage/hello_world.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/doc/usage/use_case.rst` & `timeflux-0.9.0/doc/usage/use_case.rst`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/hdf5_string.yaml` & `timeflux-0.9.0/examples/hdf5_string.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/lsl.yaml` & `timeflux-0.9.0/examples/lsl.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/lsl_multiple.yaml` & `timeflux-0.9.0/examples/lsl_multiple.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/osc.yaml` & `timeflux-0.9.0/examples/osc.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/replay.yaml` & `timeflux-0.9.0/examples/replay.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/save.yaml` & `timeflux-0.9.0/examples/save.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/ui.yaml` & `timeflux-0.9.0/examples/ui.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/zmq.yaml` & `timeflux-0.9.0/examples/zmq.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/examples/zmq2.yaml` & `timeflux-0.9.0/examples/zmq2.yaml`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/setup.cfg` & `timeflux-0.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 	pylsl>=1.12.2
 	python-osc>=1.7.0
 	python-dotenv>=0.10
 	jsonschema>=3.0
 	graphviz>=0.13
 	scikit-learn>=0.21.3
 	Jinja2>=2.11
+	colorama>=0.4.4
 
 [options.extras_require]
 dev = 
 	pytest>=5.3
 	sphinx>=2.2
 	sphinx_rtd_theme>=0.4
 	setuptools_scm
```

### Comparing `timeflux-0.8.0/test/conftest.py` & `timeflux-0.9.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/core/test_branch.py` & `timeflux-0.9.0/test/core/test_branch.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/core/test_graph.py` & `timeflux-0.9.0/test/core/test_graph.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/core/test_manager.py` & `timeflux-0.9.0/test/core/test_manager.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/core/test_node.py` & `timeflux-0.9.0/test/core/test_node.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/core/test_worker.py` & `timeflux-0.9.0/test/core/test_worker.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/data/replay.hdf5` & `timeflux-0.9.0/test/data/replay.hdf5`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/helpers/test_background.py` & `timeflux-0.9.0/test/helpers/test_background.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,7 +30,21 @@
 
 def test_exception(working_path):
     task = Task(DummyWorker(), 'echo', fail=True).start()
     while not task.done:
         status = task.status()
     assert status['success'] == False
     assert status['exception'].args[0] == 'failed'
+
+def test_stop_running(working_path):
+    task = Task(DummyWorker(), 'echo', delay=5).start()
+    sleep(.5)
+    assert task.done == False
+    task.stop()
+    assert task.done == True
+
+def test_stop_not_running(working_path):
+    task = Task(DummyWorker(), 'echo').start()
+    while not task.done:
+        status = task.status()
+    task.stop()
+    assert task.done == True
```

### Comparing `timeflux-0.8.0/test/helpers/test_mne.py` & `timeflux-0.9.0/test/helpers/test_mne.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/helpers/test_port.py` & `timeflux-0.9.0/test/helpers/test_port.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/launcher/dummy.py` & `timeflux-0.9.0/test/launcher/dummy.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/launcher/launcher.py` & `timeflux-0.9.0/test/launcher/launcher.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/launcher/test.sh` & `timeflux-0.9.0/test/launcher/test.sh`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_accumulate.py` & `timeflux-0.9.0/test/nodes/test_accumulate.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_apply.py` & `timeflux-0.9.0/test/nodes/test_apply.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_axis.py` & `timeflux-0.9.0/test/nodes/test_axis.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_dejitter.py` & `timeflux-0.9.0/test/nodes/test_dejitter.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_epoch.py` & `timeflux-0.9.0/test/nodes/test_epoch.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_expression.py` & `timeflux-0.9.0/test/nodes/test_expression.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_gate.py` & `timeflux-0.9.0/test/nodes/test_gate.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_misc.py` & `timeflux-0.9.0/test/nodes/test_misc.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_ml.py` & `timeflux-0.9.0/test/nodes/test_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,28 @@
             node.update()
     assert caplog.record_tuples[0][2].startswith('An error occured while fitting')
 
 def test_fit_interrupt():
     node = Pipeline(steps=dummy_classifier)
     node.terminate()
 
+def test_fit_reset(caplog):
+    caplog.set_level(logging.DEBUG)
+    node = Pipeline(steps=dummy_classifier, event_reset='reset')
+    node._status = -1 # bypass accumulation
+    node._X_train = np.array([-1, 1, 1, 1])
+    node._y_train = np.array([0, 1, 1, 1])
+    node.i_events.data = make_event('training_starts')
+    node.update()
+    node.i_events.data = make_event('reset')
+    node.update()
+    assert caplog.record_tuples[0][2] == 'Start training'
+    assert caplog.record_tuples[1][2].startswith('Reset')
+    assert node._status == 0
+
 def test_receive_2D():
     node = Pipeline(steps=dummy_transformer, fit=False, mode='transform')
     node.i.data = DummyData().next()
     node.update()
     assert node._X.shape == (10, 5)
     assert node._dimensions == 2
 
@@ -552,11 +566,7 @@
     node.i_0.data.columns = columns
     node.i_1.data.columns = columns
     node.update()
     assert len(list(node.iterate('o_*'))) == 2
     assert np.array_equal(node.i_0.data.index.values, node.o_0.data.index.values)
     assert list(node.i_0.data.columns) == columns
     assert list(node.i_1.data.columns) == columns
-
-def test_reset():
-    pass
-
```

### Comparing `timeflux-0.8.0/test/nodes/test_query.py` & `timeflux-0.9.0/test/nodes/test_query.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/nodes/test_window.py` & `timeflux-0.9.0/test/nodes/test_window.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/tools/convert.py` & `timeflux-0.9.0/test/tools/convert.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/test/tools/sync.py` & `timeflux-0.9.0/test/tools/sync.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/branch.py` & `timeflux-0.9.0/timeflux/core/branch.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/exceptions.py` & `timeflux-0.9.0/timeflux/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/graph.py` & `timeflux-0.9.0/timeflux/core/graph.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/io.py` & `timeflux-0.9.0/timeflux/core/io.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/logging.py` & `timeflux-0.9.0/timeflux/core/logging.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/manager.py` & `timeflux-0.9.0/timeflux/core/manager.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/message.py` & `timeflux-0.9.0/timeflux/core/message.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/node.py` & `timeflux-0.9.0/timeflux/core/node.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/scheduler.py` & `timeflux-0.9.0/timeflux/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/sync.py` & `timeflux-0.9.0/timeflux/core/sync.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/validate.py` & `timeflux-0.9.0/timeflux/core/validate.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/core/worker.py` & `timeflux-0.9.0/timeflux/core/worker.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/estimators/transformers/shape.py` & `timeflux-0.9.0/timeflux/estimators/transformers/shape.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/helpers/background.py` & `timeflux-0.9.0/timeflux/helpers/background.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/helpers/clock.py` & `timeflux-0.9.0/timeflux/helpers/clock.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/helpers/handler.py` & `timeflux-0.9.0/timeflux/helpers/handler.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/helpers/mne.py` & `timeflux-0.9.0/timeflux/helpers/mne.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/helpers/port.py` & `timeflux-0.9.0/timeflux/helpers/port.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/helpers/testing.py` & `timeflux-0.9.0/timeflux/helpers/testing.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/helpers/viz.py` & `timeflux-0.9.0/timeflux/helpers/viz.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/accumulate.py` & `timeflux-0.9.0/timeflux/nodes/accumulate.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/apply.py` & `timeflux-0.9.0/timeflux/nodes/apply.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/axis.py` & `timeflux-0.9.0/timeflux/nodes/axis.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/debug.py` & `timeflux-0.9.0/timeflux/nodes/debug.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/dejitter.py` & `timeflux-0.9.0/timeflux/nodes/dejitter.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/epoch.py` & `timeflux-0.9.0/timeflux/nodes/epoch.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/events.py` & `timeflux-0.9.0/timeflux/nodes/events.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/expression.py` & `timeflux-0.9.0/timeflux/nodes/expression.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/gate.py` & `timeflux-0.9.0/timeflux/nodes/gate.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/hdf5.py` & `timeflux-0.9.0/timeflux/nodes/hdf5.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/lsl.py` & `timeflux-0.9.0/timeflux/nodes/lsl.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/ml.py` & `timeflux-0.9.0/timeflux/nodes/ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         steps,
         fit=True,
         mode="predict",
         meta_label=("epoch", "context", "target"),
         event_start_accumulation="accumulation_starts",
         event_stop_accumulation="accumulation_stops",
         event_start_training="training_starts",
+        event_reset=None,
         buffer_size="5s",
         passthrough=False,
         resample=False,
         resample_direction="right",
         resample_rate=None,
         model=None,
         cv=None,
@@ -81,27 +82,37 @@
         # TODO: provide more context for errors
         self.fit = fit
         self.mode = mode
         self.meta_label = meta_label
         self.event_start_accumulation = event_start_accumulation
         self.event_stop_accumulation = event_stop_accumulation
         self.event_start_training = event_start_training
+        self.event_reset = event_reset
         self.passthrough = passthrough
         self.resample = resample
         self.resample_direction = resample_direction
         self.resample_rate = resample_rate
         self._buffer_size = pd.Timedelta(buffer_size)
         self._make_pipeline(steps)
         self._reset()
 
     def update(self):
 
         # Let's get ready
         self._clear()
 
+        # Reset
+        if self.event_reset:
+            matches = match_events(self.i_events, self.event_reset)
+            if matches is not None:
+                self.logger.debug("Reset")
+                if self._status == FITTING:
+                    self._task.stop()
+                self._reset()
+
         # Are we dealing with continuous data or epochs?
         if self._dimensions is None:
             port_name = "i_training" if self.fit else "i"
             if getattr(self, port_name).ready():
                 self._dimensions = 2
             elif len(list(self.iterate(port_name + "_*"))) > 0:
                 self._dimensions = 3
```

### Comparing `timeflux-0.8.0/timeflux/nodes/osc.py` & `timeflux-0.9.0/timeflux/nodes/osc.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/query.py` & `timeflux-0.9.0/timeflux/nodes/query.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/random.py` & `timeflux-0.9.0/timeflux/nodes/random.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/window.py` & `timeflux-0.9.0/timeflux/nodes/window.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/xarray.py` & `timeflux-0.9.0/timeflux/nodes/xarray.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/nodes/zmq.py` & `timeflux-0.9.0/timeflux/nodes/zmq.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/schema/app.json` & `timeflux-0.9.0/timeflux/schema/app.json`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux/timeflux.py` & `timeflux-0.9.0/timeflux/timeflux.py`

 * *Files identical despite different names*

### Comparing `timeflux-0.8.0/timeflux.egg-info/PKG-INFO` & `timeflux-0.9.0/timeflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeflux
-Version: 0.8.0
+Version: 0.9.0
 Summary: Acquisition and real-time processing of biosignals
 Home-page: https://timeflux.io
 Author: Pierre Clisson
 Author-email: contact@timeflux.io
 License: MIT
 Project-URL: Documentation, https://doc.timeflux.io
 Project-URL: Source Code, https://github.com/timeflux/timeflux
```

### Comparing `timeflux-0.8.0/timeflux.egg-info/SOURCES.txt` & `timeflux-0.9.0/timeflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

