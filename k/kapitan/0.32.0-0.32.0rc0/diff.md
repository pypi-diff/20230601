# Comparing `tmp/kapitan-0.32.0.tar.gz` & `tmp/kapitan-0.32.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kapitan-0.32.0.tar", max compression
+gzip compressed data, was "kapitan-0.32.0rc0.tar", max compression
```

## Comparing `kapitan-0.32.0.tar` & `kapitan-0.32.0rc0.tar`

### file list

```diff
@@ -1,258 +1,258 @@
--rw-r--r--   0        0        0    11357 2023-06-01 16:08:29.992906 kapitan-0.32.0/LICENSE
--rw-r--r--   0        0        0     2443 2023-06-01 16:08:29.992906 kapitan-0.32.0/README.md
--rwxr-xr-x   0        0        0     1088 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/__init__.py
--rw-r--r--   0        0        0      223 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/__main__.py
--rw-r--r--   0        0        0     1889 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/cached.py
--rw-r--r--   0        0        0    21712 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/cli.py
--rw-r--r--   0        0        0      719 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/defaults.py
--rw-r--r--   0        0        0      125 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/dependency_manager/__init__.py
--rw-r--r--   0        0        0    11955 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/dependency_manager/base.py
--rw-r--r--   0        0        0     1411 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/errors.py
--rw-r--r--   0        0        0      951 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/helm_cli.py
--rw-r--r--   0        0        0     1423 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/initialiser.py
--rw-r--r--   0        0        0      125 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/__init__.py
--rw-r--r--   0        0        0     7390 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/base.py
--rw-r--r--   0        0        0     1904 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/copy.py
--rw-r--r--   0        0        0     3324 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/external.py
--rw-r--r--   0        0        0     9501 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/helm.py
--rw-r--r--   0        0        0     2705 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/jinja2.py
--rw-r--r--   0        0        0     6327 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/jinja2_filters.py
--rw-r--r--   0        0        0     6087 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/jsonnet.py
--rw-r--r--   0        0        0     7966 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/kadet.py
--rw-r--r--   0        0        0     1137 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/remove.py
--rw-r--r--   0        0        0      163 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/templates/components/my_component/my_component.jsonnet
--rw-r--r--   0        0        0      267 2023-06-01 16:08:30.012906 kapitan-0.32.0/kapitan/inputs/templates/components/other_component/__init__.py
--rw-r--r--   0        0        0       62 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/inputs/templates/inventory/classes/common.yml
--rw-r--r--   0        0        0      629 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/inputs/templates/inventory/classes/my_component.yml
--rw-r--r--   0        0        0       75 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/inputs/templates/inventory/targets/my_target.yml
--rw-r--r--   0        0        0      129 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/inputs/templates/templates/docs/my_readme.md
--rw-r--r--   0        0        0      145 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/inputs/templates/templates/scripts/my_script.sh
--rw-r--r--   0        0        0     1008 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/lib/kapitan.libjsonnet
--rw-r--r--   0        0        0     8444 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/lint.py
--rw-r--r--   0        0        0       43 2023-06-01 16:08:30.484908 kapitan-0.32.0/kapitan/reclass/.git
--rw-r--r--   0        0        0       97 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/.gitignore
--rwxr-xr-x   0        0        0      526 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/.kitchen-verify.sh
--rw-r--r--   0        0        0      868 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/.kitchen.yml
--rw-r--r--   0        0        0       31 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/.pylintrc
--rw-r--r--   0        0        0     2522 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/.travis.yml
--rw-r--r--   0        0        0     9350 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/LICENSE
--rw-r--r--   0        0        0      385 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/MANIFEST.in
--rw-r--r--   0        0        0     1366 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/Makefile
--rw-r--r--   0        0        0      282 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/Pipfile
--rw-r--r--   0        0        0    17685 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/README-extensions.rst
--rw-r--r--   0        0        0     1260 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/README.rst
--rw-r--r--   0        0        0        7 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/.gitignore
--rw-r--r--   0        0        0     5580 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/Makefile
--rw-r--r--   0        0        0     8228 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/ansible.rst
--rw-r--r--   0        0        0     3593 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/changelog.rst
--rw-r--r--   0        0        0     6304 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/concepts.rst
--rw-r--r--   0        0        0     7858 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/conf.py
--rw-r--r--   0        0        0     1398 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/configfile.rst
--rw-r--r--   0        0        0      304 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/extrefs.inc
--rw-r--r--   0        0        0     2084 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/hacking.rst
--rw-r--r--   0        0        0     2250 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/index.rst
--rw-r--r--   0        0        0     3078 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/install.rst
--rw-r--r--   0        0        0     1415 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/intro.inc
--rw-r--r--   0        0        0     1473 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/manpage.rst
--rw-r--r--   0        0        0     7147 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/operations.rst
--rw-r--r--   0        0        0      518 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/puppet.rst
--rw-r--r--   0        0        0     1261 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/refs.rst
--rw-r--r--   0        0        0     8144 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/salt.rst
--rw-r--r--   0        0        0       35 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/substs.inc
--rw-r--r--   0        0        0     6233 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/todo.rst
--rw-r--r--   0        0        0     1895 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/doc/source/usage.rst
--rwxr-xr-x   0        0        0       96 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/ansible/hosts
--rw-r--r--   0        0        0       23 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/ansible/reclass-config.yml
--rw-r--r--   0        0        0      131 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/ansible/test.yml
--rw-r--r--   0        0        0     1362 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/init.yml
--rw-r--r--   0        0        0       72 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/release/jessie.yml
--rw-r--r--   0        0        0       72 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/release/lenny.yml
--rw-r--r--   0        0        0       70 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/release/sid.yml
--rw-r--r--   0        0        0       75 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/release/squeeze.yml
--rw-r--r--   0        0        0       71 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/release/wheezy.yml
--rw-r--r--   0        0        0      492 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/archived.yml
--rw-r--r--   0        0        0      351 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/include_backports.yml
--rw-r--r--   0        0        0      346 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/include_experimental.yml
--rw-r--r--   0        0        0      320 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/include_multimedia.yml
--rw-r--r--   0        0        0      545 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml
--rw-r--r--   0        0        0      148 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/oldstable.yml
--rw-r--r--   0        0        0      146 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/stable.yml
--rw-r--r--   0        0        0      146 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/testing.yml
--rw-r--r--   0        0        0      146 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/unstable.yml
--rw-r--r--   0        0        0      563 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/example.org.yml
--rw-r--r--   0        0        0      143 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/hosted@munich.yml
--rw-r--r--   0        0        0      142 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/hosted@zurich.yml
--rw-r--r--   0        0        0       26 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/mail/init.yml
--rw-r--r--   0        0        0       68 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/mail/relay.yml
--rw-r--r--   0        0        0      200 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/mail/satellite.yml
--rw-r--r--   0        0        0       55 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/mail/server.yml
--rw-r--r--   0        0        0      177 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/salt.minion.yml
--rw-r--r--   0        0        0      320 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/sudo.yml
--rw-r--r--   0        0        0       25 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/classes/webserver.yml
--rw-r--r--   0        0        0      175 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/nodes/munich/black.example.org.yml
--rw-r--r--   0        0        0      157 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/nodes/munich/yellow.example.org.yml
--rw-r--r--   0        0        0      211 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/nodes/zurich/blue.example.org.yml
--rw-r--r--   0        0        0      159 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/nodes/zurich/white.example.org.yml
--rwxr-xr-x   0        0        0       93 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/salt/reclass
--rw-r--r--   0        0        0       23 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/examples/salt/reclass-config.yml
--rw-r--r--   0        0        0     1058 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/reclass/__init__.py
--rwxr-xr-x   0        0        0      366 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/reclass/adapters/__init__.py
--rwxr-xr-x   0        0        0     4348 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/adapters/ansible.py
--rwxr-xr-x   0        0        0     5517 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/adapters/salt.py
--rw-r--r--   0        0        0     1811 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/cli.py
--rw-r--r--   0        0        0     9536 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/config.py
--rw-r--r--   0        0        0      594 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/constants.py
--rw-r--r--   0        0        0    11835 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/core.py
--rw-r--r--   0        0        0      527 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/__init__.py
--rw-r--r--   0        0        0     2407 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/applications.py
--rw-r--r--   0        0        0     2349 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/classes.py
--rw-r--r--   0        0        0     4510 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/entity.py
--rw-r--r--   0        0        0     3644 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/exports.py
--rw-r--r--   0        0        0    14190 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/parameters.py
--rw-r--r--   0        0        0      169 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/__init__.py
--rw-r--r--   0        0        0     2483 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_applications.py
--rw-r--r--   0        0        0     4054 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_classes.py
--rw-r--r--   0        0        0    15579 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_entity.py
--rw-r--r--   0        0        0     5875 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_exports.py
--rw-r--r--   0        0        0    35361 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_parameters.py
--rw-r--r--   0        0        0     1770 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/defaults.py
--rw-r--r--   0        0        0    11777 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/errors.py
--rw-r--r--   0        0        0     1086 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/output/__init__.py
--rw-r--r--   0        0        0      697 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/output/json_outputter.py
--rw-r--r--   0        0        0      971 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/output/yaml_outputter.py
--rw-r--r--   0        0        0     2966 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/settings.py
--rw-r--r--   0        0        0     1611 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/__init__.py
--rw-r--r--   0        0        0     1294 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/common.py
--rw-r--r--   0        0        0     1284 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/loader.py
--rw-r--r--   0        0        0     2294 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/memcache_proxy.py
--rw-r--r--   0        0        0     2419 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/mixed/__init__.py
--rw-r--r--   0        0        0      169 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/tests/__init__.py
--rw-r--r--   0        0        0      725 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/tests/test_loader.py
--rw-r--r--   0        0        0     4070 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py
--rw-r--r--   0        0        0     1254 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/tests/test_yamldata.py
--rw-r--r--   0        0        0     4031 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/yaml_fs/__init__.py
--rw-r--r--   0        0        0     2258 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/yaml_fs/directory.py
--rw-r--r--   0        0        0    12803 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/yaml_git/__init__.py
--rw-r--r--   0        0        0     3721 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/storage/yamldata.py
--rw-r--r--   0        0        0      169 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/__init__.py
--rw-r--r--   0        0        0       48 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/01/classes/standard.yml
--rw-r--r--   0        0        0       63 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/01/nodes/class_notfound.yml
--rw-r--r--   0        0        0       22 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/01/nodes/data_types.yml
--rw-r--r--   0        0        0       28 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/classes/four.yml
--rw-r--r--   0        0        0       27 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/classes/init.yml
--rw-r--r--   0        0        0      183 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/classes/one/alpha.yml
--rw-r--r--   0        0        0       26 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/classes/one/beta.yml
--rw-r--r--   0        0        0       22 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/classes/three.yml
--rw-r--r--   0        0        0       26 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/classes/two/beta.yml
--rw-r--r--   0        0        0       27 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/classes/two/gamma.yml
--rw-r--r--   0        0        0       23 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/nodes/relative.yml
--rw-r--r--   0        0        0       19 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/02/nodes/top_relative.yml
--rw-r--r--   0        0        0       57 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/classes/a.yml
--rw-r--r--   0        0        0       57 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/classes/b.yml
--rw-r--r--   0        0        0       57 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/classes/c.yml
--rw-r--r--   0        0        0       57 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/classes/d.yml
--rw-r--r--   0        0        0       17 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/nodes/alpha/one.yml
--rw-r--r--   0        0        0       17 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/nodes/alpha/two.yml
--rw-r--r--   0        0        0       17 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/nodes/beta/one.yml
--rw-r--r--   0        0        0       17 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/03/nodes/beta/two.yml
--rw-r--r--   0        0        0       23 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/04/classes/one.yml
--rw-r--r--   0        0        0       23 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/04/classes/three.yml
--rw-r--r--   0        0        0       23 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/04/classes/two.yml
--rw-r--r--   0        0        0       17 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/04/nodes/alpha/node1.yml
--rw-r--r--   0        0        0       53 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v0.yml
--rw-r--r--   0        0        0       53 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v1.yml
--rw-r--r--   0        0        0      134 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/components/common.yml
--rw-r--r--   0        0        0       43 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v0.yml
--rw-r--r--   0        0        0       43 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v1.yml
--rw-r--r--   0        0        0       75 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/versions/default_versions.yml
--rw-r--r--   0        0        0      114 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/versions/dev.yml
--rw-r--r--   0        0        0       52 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/versions/prd.yml
--rw-r--r--   0        0        0       87 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/classes/versions/stg.yml
--rw-r--r--   0        0        0      101 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/nodes/dev.yml
--rw-r--r--   0        0        0      101 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/nodes/prd.yml
--rw-r--r--   0        0        0      101 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/05/nodes/stg.yml
--rw-r--r--   0        0        0       50 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/06/classes/applications/shared.yml
--rw-r--r--   0        0        0       98 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/06/classes/environments/envA.yml
--rw-r--r--   0        0        0       67 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/06/classes/environments/envB.yml
--rw-r--r--   0        0        0      140 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/06/nodes/A_node.yml
--rw-r--r--   0        0        0      140 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/data/06/nodes/B_node.yml
--rw-r--r--   0        0        0     6811 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/tests/test_core.py
--rw-r--r--   0        0        0      169 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/utils/__init__.py
--rw-r--r--   0        0        0     5289 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/utils/dictpath.py
--rw-r--r--   0        0        0      281 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/utils/parameterdict.py
--rw-r--r--   0        0        0      281 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/utils/parameterlist.py
--rw-r--r--   0        0        0      169 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/utils/tests/__init__.py
--rw-r--r--   0        0        0     4504 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/utils/tests/test_dictpath.py
--rw-r--r--   0        0        0      173 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/__init__.py
--rw-r--r--   0        0        0      848 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/compitem.py
--rw-r--r--   0        0        0      170 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/dictitem.py
--rw-r--r--   0        0        0     9225 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/invitem.py
--rw-r--r--   0        0        0     2355 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/item.py
--rw-r--r--   0        0        0      392 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/listitem.py
--rw-r--r--   0        0        0     3031 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/parser.py
--rw-r--r--   0        0        0     7207 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/parser_funcs.py
--rw-r--r--   0        0        0     1364 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/refitem.py
--rw-r--r--   0        0        0      777 2023-06-01 16:08:31.144912 kapitan-0.32.0/kapitan/reclass/reclass/values/scaitem.py
--rw-r--r--   0        0        0        0 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/__init__.py
--rw-r--r--   0        0        0     4043 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_compitem.py
--rw-r--r--   0        0        0     1398 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_item.py
--rw-r--r--   0        0        0      979 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_listitem.py
--rw-r--r--   0        0        0     4512 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_parser_functions.py
--rw-r--r--   0        0        0     1727 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_refitem.py
--rw-r--r--   0        0        0     1176 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_scaitem.py
--rw-r--r--   0        0        0     4587 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_value.py
--rw-r--r--   0        0        0     2780 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/value.py
--rw-r--r--   0        0        0     6797 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/values/valuelist.py
--rw-r--r--   0        0        0      966 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/reclass/version.py
--rwxr-xr-x   0        0        0      426 2023-06-01 16:08:31.140912 kapitan-0.32.0/kapitan/reclass/reclass.py
--rw-r--r--   0        0        0     1948 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/releasenotes/config.yaml
--rw-r--r--   0        0        0      109 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/releasenotes/notes/escaping-references-e76699d8ca010013.yaml
--rw-r--r--   0        0        0       32 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/requirements.txt
--rwxr-xr-x   0        0        0      502 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/run_tests.py
--rw-r--r--   0        0        0      254 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/setup.cfg
--rw-r--r--   0        0        0     1780 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/setup.py
--rw-r--r--   0        0        0      413 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/default/classes/first.yml
--rw-r--r--   0        0        0       34 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/default/classes/lab/env/dev.yml
--rw-r--r--   0        0        0      109 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/default/classes/second.yml
--rw-r--r--   0        0        0      361 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/default/classes/third.yml
--rw-r--r--   0        0        0       18 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/default/nodes/reclass.yml
--rw-r--r--   0        0        0       22 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/default/reclass-config.yml
--rw-r--r--   0        0        0       42 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/defaults.yml
--rw-r--r--   0        0        0       77 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/first.yml
--rw-r--r--   0        0        0       34 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/lab/env/dev.yml
--rw-r--r--   0        0        0       22 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/relative/init.yml
--rw-r--r--   0        0        0       63 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/relative/nested/common.yml
--rw-r--r--   0        0        0       53 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/common.yml
--rw-r--r--   0        0        0       91 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/init.yml
--rw-r--r--   0        0        0       53 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/relative/nested/dive/session.yml
--rw-r--r--   0        0        0      100 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/relative/nested/init.yml
--rw-r--r--   0        0        0      104 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/second.yml
--rw-r--r--   0        0        0      191 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/classes/third.yml
--rw-r--r--   0        0        0       19 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/nodes/reclass.yml
--rw-r--r--   0        0        0       78 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/test/model/extensions/reclass-config.yml
--rw-r--r--   0        0        0      976 2023-06-01 16:08:31.148912 kapitan-0.32.0/kapitan/reclass/tox.ini
--rw-r--r--   0        0        0      125 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/__init__.py
--rw-r--r--   0        0        0    26916 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/base.py
--rw-r--r--   0        0        0     2833 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/base64.py
--rw-r--r--   0        0        0    24002 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/cmd_parser.py
--rw-r--r--   0        0        0     1453 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/env.py
--rw-r--r--   0        0        0     7277 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/functions.py
--rw-r--r--   0        0        0      125 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/secrets/__init__.py
--rw-r--r--   0        0        0     4904 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/secrets/awskms.py
--rw-r--r--   0        0        0     5867 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/secrets/azkms.py
--rw-r--r--   0        0        0     5814 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/secrets/gkms.py
--rw-r--r--   0        0        0     7299 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/secrets/gpg.py
--rw-r--r--   0        0        0     9041 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/secrets/vaultkv.py
--rw-r--r--   0        0        0    11361 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/refs/secrets/vaulttransit.py
--rw-r--r--   0        0        0        0 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/remoteinventory/__init__.py
--rw-r--r--   0        0        0     4346 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/remoteinventory/fetch.py
--rw-r--r--   0        0        0    14266 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/resources.py
--rw-r--r--   0        0        0    35492 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/targets.py
--rw-r--r--   0        0        0    21894 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/utils.py
--rw-r--r--   0        0        0      125 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/validator/__init__.py
--rw-r--r--   0        0        0      369 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/validator/base.py
--rw-r--r--   0        0        0     3805 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/validator/kubernetes_validator.py
--rw-r--r--   0        0        0      508 2023-06-01 16:08:30.016906 kapitan-0.32.0/kapitan/version.py
--rw-r--r--   0        0        0     1852 2023-06-01 16:08:30.016906 kapitan-0.32.0/pyproject.toml
--rw-r--r--   0        0        0    10228 1970-01-01 00:00:00.000000 kapitan-0.32.0/setup.py
--rw-r--r--   0        0        0     4630 1970-01-01 00:00:00.000000 kapitan-0.32.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-02 21:01:54.811166 kapitan-0.32.0rc0/LICENSES/
+-rw-r--r--   0        0        0     2443 2023-05-02 21:01:54.811166 kapitan-0.32.0rc0/README.md
+-rwxr-xr-x   0        0        0     1088 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/__main__.py
+-rw-r--r--   0        0        0     1889 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/cached.py
+-rw-r--r--   0        0        0    21712 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/cli.py
+-rw-r--r--   0        0        0      719 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/defaults.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/dependency_manager/__init__.py
+-rw-r--r--   0        0        0    11773 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/dependency_manager/base.py
+-rw-r--r--   0        0        0     1411 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/errors.py
+-rw-r--r--   0        0        0      951 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/helm_cli.py
+-rw-r--r--   0        0        0     1423 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/initialiser.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/__init__.py
+-rw-r--r--   0        0        0     7390 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/base.py
+-rw-r--r--   0        0        0     1904 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/copy.py
+-rw-r--r--   0        0        0     3324 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/external.py
+-rw-r--r--   0        0        0     9501 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/helm.py
+-rw-r--r--   0        0        0     2705 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/jinja2.py
+-rw-r--r--   0        0        0     6327 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/jinja2_filters.py
+-rw-r--r--   0        0        0     6087 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/jsonnet.py
+-rw-r--r--   0        0        0     7966 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/kadet.py
+-rw-r--r--   0        0        0     1137 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/remove.py
+-rw-r--r--   0        0        0      163 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/components/my_component/my_component.jsonnet
+-rw-r--r--   0        0        0      267 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/components/other_component/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/classes/common.yml
+-rw-r--r--   0        0        0      629 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/classes/my_component.yml
+-rw-r--r--   0        0        0       75 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/targets/my_target.yml
+-rw-r--r--   0        0        0      129 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/templates/docs/my_readme.md
+-rw-r--r--   0        0        0      145 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/inputs/templates/templates/scripts/my_script.sh
+-rw-r--r--   0        0        0     1008 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/lib/kapitan.libjsonnet
+-rw-r--r--   0        0        0     8444 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/lint.py
+-rw-r--r--   0        0        0       43 2023-05-02 21:01:55.343198 kapitan-0.32.0rc0/kapitan/reclass/.git
+-rw-r--r--   0        0        0       97 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.gitignore
+-rwxr-xr-x   0        0        0      526 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.kitchen-verify.sh
+-rw-r--r--   0        0        0      868 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.kitchen.yml
+-rw-r--r--   0        0        0       31 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.pylintrc
+-rw-r--r--   0        0        0     2522 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/.travis.yml
+-rw-r--r--   0        0        0     9350 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/LICENSE
+-rw-r--r--   0        0        0      385 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/MANIFEST.in
+-rw-r--r--   0        0        0     1366 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/Makefile
+-rw-r--r--   0        0        0      282 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/Pipfile
+-rw-r--r--   0        0        0    17685 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/README-extensions.rst
+-rw-r--r--   0        0        0     1260 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/README.rst
+-rw-r--r--   0        0        0        7 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/.gitignore
+-rw-r--r--   0        0        0     5580 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/Makefile
+-rw-r--r--   0        0        0     8228 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/ansible.rst
+-rw-r--r--   0        0        0     3593 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/changelog.rst
+-rw-r--r--   0        0        0     6304 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/concepts.rst
+-rw-r--r--   0        0        0     7858 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/conf.py
+-rw-r--r--   0        0        0     1398 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/configfile.rst
+-rw-r--r--   0        0        0      304 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/extrefs.inc
+-rw-r--r--   0        0        0     2084 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/hacking.rst
+-rw-r--r--   0        0        0     2250 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/index.rst
+-rw-r--r--   0        0        0     3078 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/install.rst
+-rw-r--r--   0        0        0     1415 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/intro.inc
+-rw-r--r--   0        0        0     1473 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/manpage.rst
+-rw-r--r--   0        0        0     7147 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/operations.rst
+-rw-r--r--   0        0        0      518 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/puppet.rst
+-rw-r--r--   0        0        0     1261 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/refs.rst
+-rw-r--r--   0        0        0     8144 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/salt.rst
+-rw-r--r--   0        0        0       35 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/substs.inc
+-rw-r--r--   0        0        0     6233 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/todo.rst
+-rw-r--r--   0        0        0     1895 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/doc/source/usage.rst
+-rwxr-xr-x   0        0        0       96 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/ansible/hosts
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/ansible/reclass-config.yml
+-rw-r--r--   0        0        0      131 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/ansible/test.yml
+-rw-r--r--   0        0        0     1362 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/init.yml
+-rw-r--r--   0        0        0       72 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/jessie.yml
+-rw-r--r--   0        0        0       72 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/lenny.yml
+-rw-r--r--   0        0        0       70 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/sid.yml
+-rw-r--r--   0        0        0       75 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/squeeze.yml
+-rw-r--r--   0        0        0       71 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/release/wheezy.yml
+-rw-r--r--   0        0        0      492 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/archived.yml
+-rw-r--r--   0        0        0      351 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_backports.yml
+-rw-r--r--   0        0        0      346 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_experimental.yml
+-rw-r--r--   0        0        0      320 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_multimedia.yml
+-rw-r--r--   0        0        0      545 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml
+-rw-r--r--   0        0        0      148 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/oldstable.yml
+-rw-r--r--   0        0        0      146 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/stable.yml
+-rw-r--r--   0        0        0      146 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/testing.yml
+-rw-r--r--   0        0        0      146 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/unstable.yml
+-rw-r--r--   0        0        0      563 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/example.org.yml
+-rw-r--r--   0        0        0      143 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/hosted@munich.yml
+-rw-r--r--   0        0        0      142 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/hosted@zurich.yml
+-rw-r--r--   0        0        0       26 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/init.yml
+-rw-r--r--   0        0        0       68 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/relay.yml
+-rw-r--r--   0        0        0      200 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/satellite.yml
+-rw-r--r--   0        0        0       55 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/mail/server.yml
+-rw-r--r--   0        0        0      177 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/salt.minion.yml
+-rw-r--r--   0        0        0      320 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/sudo.yml
+-rw-r--r--   0        0        0       25 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/classes/webserver.yml
+-rw-r--r--   0        0        0      175 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/munich/black.example.org.yml
+-rw-r--r--   0        0        0      157 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/munich/yellow.example.org.yml
+-rw-r--r--   0        0        0      211 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/zurich/blue.example.org.yml
+-rw-r--r--   0        0        0      159 2023-05-02 21:01:55.955235 kapitan-0.32.0rc0/kapitan/reclass/examples/nodes/zurich/white.example.org.yml
+-rwxr-xr-x   0        0        0       93 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/examples/salt/reclass
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/examples/salt/reclass-config.yml
+-rw-r--r--   0        0        0     1058 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/__init__.py
+-rwxr-xr-x   0        0        0      366 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/__init__.py
+-rwxr-xr-x   0        0        0     4348 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/ansible.py
+-rwxr-xr-x   0        0        0     5517 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/salt.py
+-rw-r--r--   0        0        0     1811 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/cli.py
+-rw-r--r--   0        0        0     9536 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/config.py
+-rw-r--r--   0        0        0      594 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/constants.py
+-rw-r--r--   0        0        0    11835 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/core.py
+-rw-r--r--   0        0        0      527 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/__init__.py
+-rw-r--r--   0        0        0     2407 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/applications.py
+-rw-r--r--   0        0        0     2349 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/classes.py
+-rw-r--r--   0        0        0     4510 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/entity.py
+-rw-r--r--   0        0        0     3644 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/exports.py
+-rw-r--r--   0        0        0    14190 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/parameters.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/__init__.py
+-rw-r--r--   0        0        0     2483 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_applications.py
+-rw-r--r--   0        0        0     4054 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_classes.py
+-rw-r--r--   0        0        0    15579 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_entity.py
+-rw-r--r--   0        0        0     5875 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_exports.py
+-rw-r--r--   0        0        0    35361 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_parameters.py
+-rw-r--r--   0        0        0     1770 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/defaults.py
+-rw-r--r--   0        0        0    11777 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/errors.py
+-rw-r--r--   0        0        0     1086 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/output/__init__.py
+-rw-r--r--   0        0        0      697 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/output/json_outputter.py
+-rw-r--r--   0        0        0      971 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/output/yaml_outputter.py
+-rw-r--r--   0        0        0     2966 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/settings.py
+-rw-r--r--   0        0        0     1611 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/__init__.py
+-rw-r--r--   0        0        0     1294 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/common.py
+-rw-r--r--   0        0        0     1284 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/loader.py
+-rw-r--r--   0        0        0     2294 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/memcache_proxy.py
+-rw-r--r--   0        0        0     2419 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/mixed/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/__init__.py
+-rw-r--r--   0        0        0      725 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_loader.py
+-rw-r--r--   0        0        0     4070 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py
+-rw-r--r--   0        0        0     1254 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_yamldata.py
+-rw-r--r--   0        0        0     4031 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/__init__.py
+-rw-r--r--   0        0        0     2258 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/directory.py
+-rw-r--r--   0        0        0    12803 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_git/__init__.py
+-rw-r--r--   0        0        0     3721 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yamldata.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/01/classes/standard.yml
+-rw-r--r--   0        0        0       63 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/01/nodes/class_notfound.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/01/nodes/data_types.yml
+-rw-r--r--   0        0        0       28 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/four.yml
+-rw-r--r--   0        0        0       27 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/init.yml
+-rw-r--r--   0        0        0      183 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/one/alpha.yml
+-rw-r--r--   0        0        0       26 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/one/beta.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/three.yml
+-rw-r--r--   0        0        0       26 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/two/beta.yml
+-rw-r--r--   0        0        0       27 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/classes/two/gamma.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/nodes/relative.yml
+-rw-r--r--   0        0        0       19 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/02/nodes/top_relative.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/a.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/b.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/c.yml
+-rw-r--r--   0        0        0       57 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/classes/d.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/alpha/one.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/alpha/two.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/beta/one.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/03/nodes/beta/two.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/classes/one.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/classes/three.yml
+-rw-r--r--   0        0        0       23 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/classes/two.yml
+-rw-r--r--   0        0        0       17 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/04/nodes/alpha/node1.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v0.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/cluster-autoscaler/v1.yml
+-rw-r--r--   0        0        0      134 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/common.yml
+-rw-r--r--   0        0        0       43 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v0.yml
+-rw-r--r--   0        0        0       43 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/components/core-dns/v1.yml
+-rw-r--r--   0        0        0       75 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/default_versions.yml
+-rw-r--r--   0        0        0      114 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/dev.yml
+-rw-r--r--   0        0        0       52 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/prd.yml
+-rw-r--r--   0        0        0       87 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/classes/versions/stg.yml
+-rw-r--r--   0        0        0      101 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/nodes/dev.yml
+-rw-r--r--   0        0        0      101 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/nodes/prd.yml
+-rw-r--r--   0        0        0      101 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/05/nodes/stg.yml
+-rw-r--r--   0        0        0       50 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/classes/applications/shared.yml
+-rw-r--r--   0        0        0       98 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/classes/environments/envA.yml
+-rw-r--r--   0        0        0       67 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/classes/environments/envB.yml
+-rw-r--r--   0        0        0      140 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/nodes/A_node.yml
+-rw-r--r--   0        0        0      140 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/data/06/nodes/B_node.yml
+-rw-r--r--   0        0        0     6811 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/test_core.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/dictpath.py
+-rw-r--r--   0        0        0      281 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/parameterdict.py
+-rw-r--r--   0        0        0      281 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/parameterlist.py
+-rw-r--r--   0        0        0      169 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/tests/__init__.py
+-rw-r--r--   0        0        0     4504 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/tests/test_dictpath.py
+-rw-r--r--   0        0        0      173 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/__init__.py
+-rw-r--r--   0        0        0      848 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/compitem.py
+-rw-r--r--   0        0        0      170 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/dictitem.py
+-rw-r--r--   0        0        0     9225 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/invitem.py
+-rw-r--r--   0        0        0     2355 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/item.py
+-rw-r--r--   0        0        0      392 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/listitem.py
+-rw-r--r--   0        0        0     3031 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser.py
+-rw-r--r--   0        0        0     7207 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser_funcs.py
+-rw-r--r--   0        0        0     1364 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/refitem.py
+-rw-r--r--   0        0        0      777 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/scaitem.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/__init__.py
+-rw-r--r--   0        0        0     4043 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_compitem.py
+-rw-r--r--   0        0        0     1398 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_item.py
+-rw-r--r--   0        0        0      979 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_listitem.py
+-rw-r--r--   0        0        0     4512 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_parser_functions.py
+-rw-r--r--   0        0        0     1727 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_refitem.py
+-rw-r--r--   0        0        0     1176 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_scaitem.py
+-rw-r--r--   0        0        0     4587 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_value.py
+-rw-r--r--   0        0        0     2780 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/value.py
+-rw-r--r--   0        0        0     6797 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/values/valuelist.py
+-rw-r--r--   0        0        0      966 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/reclass/version.py
+-rwxr-xr-x   0        0        0      426 2023-05-02 21:01:55.959235 kapitan-0.32.0rc0/kapitan/reclass/reclass.py
+-rw-r--r--   0        0        0     1948 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/releasenotes/config.yaml
+-rw-r--r--   0        0        0      109 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/releasenotes/notes/escaping-references-e76699d8ca010013.yaml
+-rw-r--r--   0        0        0       32 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/requirements.txt
+-rwxr-xr-x   0        0        0      502 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/run_tests.py
+-rw-r--r--   0        0        0      254 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/setup.cfg
+-rw-r--r--   0        0        0     1780 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/setup.py
+-rw-r--r--   0        0        0      413 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/first.yml
+-rw-r--r--   0        0        0       34 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/lab/env/dev.yml
+-rw-r--r--   0        0        0      109 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/second.yml
+-rw-r--r--   0        0        0      361 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/classes/third.yml
+-rw-r--r--   0        0        0       18 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/nodes/reclass.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/default/reclass-config.yml
+-rw-r--r--   0        0        0       42 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/defaults.yml
+-rw-r--r--   0        0        0       77 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/first.yml
+-rw-r--r--   0        0        0       34 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/lab/env/dev.yml
+-rw-r--r--   0        0        0       22 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/init.yml
+-rw-r--r--   0        0        0       63 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/common.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/common.yml
+-rw-r--r--   0        0        0       91 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/deep/init.yml
+-rw-r--r--   0        0        0       53 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/dive/session.yml
+-rw-r--r--   0        0        0      100 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/relative/nested/init.yml
+-rw-r--r--   0        0        0      104 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/second.yml
+-rw-r--r--   0        0        0      191 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/classes/third.yml
+-rw-r--r--   0        0        0       19 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/nodes/reclass.yml
+-rw-r--r--   0        0        0       78 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/test/model/extensions/reclass-config.yml
+-rw-r--r--   0        0        0      976 2023-05-02 21:01:55.963236 kapitan-0.32.0rc0/kapitan/reclass/tox.ini
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/__init__.py
+-rw-r--r--   0        0        0    26916 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/base.py
+-rw-r--r--   0        0        0     2833 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/base64.py
+-rw-r--r--   0        0        0    24002 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/cmd_parser.py
+-rw-r--r--   0        0        0     1453 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/env.py
+-rw-r--r--   0        0        0     7277 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/functions.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/__init__.py
+-rw-r--r--   0        0        0     4904 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/awskms.py
+-rw-r--r--   0        0        0     5867 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/azkms.py
+-rw-r--r--   0        0        0     5814 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/gkms.py
+-rw-r--r--   0        0        0     7299 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/gpg.py
+-rw-r--r--   0        0        0     9041 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/vaultkv.py
+-rw-r--r--   0        0        0    11361 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/refs/secrets/vaulttransit.py
+-rw-r--r--   0        0        0        0 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/remoteinventory/__init__.py
+-rw-r--r--   0        0        0     4346 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/remoteinventory/fetch.py
+-rw-r--r--   0        0        0    14266 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/resources.py
+-rw-r--r--   0        0        0    35433 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/targets.py
+-rw-r--r--   0        0        0    21894 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/utils.py
+-rw-r--r--   0        0        0      125 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/validator/__init__.py
+-rw-r--r--   0        0        0      369 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/validator/base.py
+-rw-r--r--   0        0        0     3805 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/validator/kubernetes_validator.py
+-rw-r--r--   0        0        0      511 2023-05-02 21:01:54.839167 kapitan-0.32.0rc0/kapitan/version.py
+-rw-r--r--   0        0        0     1855 2023-05-02 21:01:54.843168 kapitan-0.32.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    10231 1970-01-01 00:00:00.000000 kapitan-0.32.0rc0/setup.py
+-rw-r--r--   0        0        0     4633 1970-01-01 00:00:00.000000 kapitan-0.32.0rc0/PKG-INFO
```

### Comparing `kapitan-0.32.0/README.md` & `kapitan-0.32.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/__init__.py` & `kapitan-0.32.0rc0/kapitan/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/cached.py` & `kapitan-0.32.0rc0/kapitan/cached.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/cli.py` & `kapitan-0.32.0rc0/kapitan/cli.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/defaults.py` & `kapitan-0.32.0rc0/kapitan/defaults.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/dependency_manager/base.py` & `kapitan-0.32.0rc0/kapitan/dependency_manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,14 @@
         copy_src_path = cached_repo_path
         if "ref" in dep:
             ref = dep["ref"]
             repo.git.checkout(ref)
         else:
             repo.git.checkout("master")  # default ref
 
-        # initialising submodules
-        if "submodules" not in dep or dep["submodules"]:
-            for submodule in repo.submodules:
-                submodule.update(init=True)
-
         if "subdir" in dep:
             sub_dir = dep["subdir"]
             full_subdir = os.path.join(cached_repo_path, sub_dir)
             if os.path.isdir(full_subdir):
                 copy_src_path = full_subdir
             else:
                 raise GitSubdirNotFoundError(
```

### Comparing `kapitan-0.32.0/kapitan/errors.py` & `kapitan-0.32.0rc0/kapitan/errors.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/helm_cli.py` & `kapitan-0.32.0rc0/kapitan/helm_cli.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/initialiser.py` & `kapitan-0.32.0rc0/kapitan/initialiser.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/base.py` & `kapitan-0.32.0rc0/kapitan/inputs/base.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/copy.py` & `kapitan-0.32.0rc0/kapitan/inputs/copy.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/external.py` & `kapitan-0.32.0rc0/kapitan/inputs/external.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/helm.py` & `kapitan-0.32.0rc0/kapitan/inputs/helm.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/jinja2.py` & `kapitan-0.32.0rc0/kapitan/inputs/jinja2.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/jinja2_filters.py` & `kapitan-0.32.0rc0/kapitan/inputs/jinja2_filters.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/jsonnet.py` & `kapitan-0.32.0rc0/kapitan/inputs/jsonnet.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/kadet.py` & `kapitan-0.32.0rc0/kapitan/inputs/kadet.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/remove.py` & `kapitan-0.32.0rc0/kapitan/inputs/remove.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/inputs/templates/inventory/classes/my_component.yml` & `kapitan-0.32.0rc0/kapitan/inputs/templates/inventory/classes/my_component.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/lib/kapitan.libjsonnet` & `kapitan-0.32.0rc0/kapitan/lib/kapitan.libjsonnet`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/lint.py` & `kapitan-0.32.0rc0/kapitan/lint.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/.kitchen-verify.sh` & `kapitan-0.32.0rc0/kapitan/reclass/.kitchen-verify.sh`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/.kitchen.yml` & `kapitan-0.32.0rc0/kapitan/reclass/.kitchen.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/.travis.yml` & `kapitan-0.32.0rc0/kapitan/reclass/.travis.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/LICENSE` & `kapitan-0.32.0rc0/kapitan/reclass/LICENSE`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/Makefile` & `kapitan-0.32.0rc0/kapitan/reclass/Makefile`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/README-extensions.rst` & `kapitan-0.32.0rc0/kapitan/reclass/README-extensions.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/README.rst` & `kapitan-0.32.0rc0/kapitan/reclass/README.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/Makefile` & `kapitan-0.32.0rc0/kapitan/reclass/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/ansible.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/ansible.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/changelog.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/concepts.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/concepts.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/conf.py` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/configfile.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/configfile.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/hacking.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/hacking.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/index.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/install.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/intro.inc` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/intro.inc`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/manpage.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/manpage.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/operations.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/operations.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/puppet.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/puppet.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/refs.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/refs.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/salt.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/salt.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/todo.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/todo.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/doc/source/usage.rst` & `kapitan-0.32.0rc0/kapitan/reclass/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/examples/classes/debian/init.yml` & `kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/init.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml` & `kapitan-0.32.0rc0/kapitan/reclass/examples/classes/debian/suite/include_volatile.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/examples/classes/example.org.yml` & `kapitan-0.32.0rc0/kapitan/reclass/examples/classes/example.org.yml`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/adapters/ansible.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/ansible.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/adapters/salt.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/adapters/salt.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/cli.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/cli.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/config.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/config.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/constants.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/constants.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/core.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/core.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/applications.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/applications.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/classes.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/entity.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/entity.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/exports.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/exports.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/parameters.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/parameters.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_applications.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_applications.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_classes.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_entity.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_exports.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_exports.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/datatypes/tests/test_parameters.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/datatypes/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/defaults.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/defaults.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/errors.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/errors.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/output/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/output/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/output/json_outputter.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/output/json_outputter.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/output/yaml_outputter.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/output/yaml_outputter.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/settings.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/settings.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/common.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/common.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/loader.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/loader.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/memcache_proxy.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/memcache_proxy.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/mixed/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/mixed/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/tests/test_loader.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_memcache_proxy.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/tests/test_yamldata.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/tests/test_yamldata.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/yaml_fs/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/yaml_fs/directory.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_fs/directory.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/yaml_git/__init__.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yaml_git/__init__.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/storage/yamldata.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/storage/yamldata.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/tests/test_core.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/utils/dictpath.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/dictpath.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/utils/tests/test_dictpath.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/utils/tests/test_dictpath.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/compitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/compitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/invitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/invitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/item.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/item.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/parser.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/parser_funcs.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/parser_funcs.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/refitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/refitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/scaitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/scaitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_compitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_compitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_item.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_listitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_listitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_parser_functions.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_parser_functions.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_refitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_refitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_scaitem.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_scaitem.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/tests/test_value.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/tests/test_value.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/value.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/value.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/values/valuelist.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/values/valuelist.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/reclass/version.py` & `kapitan-0.32.0rc0/kapitan/reclass/reclass/version.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/releasenotes/config.yaml` & `kapitan-0.32.0rc0/kapitan/reclass/releasenotes/config.yaml`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/setup.py` & `kapitan-0.32.0rc0/kapitan/reclass/setup.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/reclass/tox.ini` & `kapitan-0.32.0rc0/kapitan/reclass/tox.ini`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/base.py` & `kapitan-0.32.0rc0/kapitan/refs/base.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/base64.py` & `kapitan-0.32.0rc0/kapitan/refs/base64.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/cmd_parser.py` & `kapitan-0.32.0rc0/kapitan/refs/cmd_parser.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/env.py` & `kapitan-0.32.0rc0/kapitan/refs/env.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/functions.py` & `kapitan-0.32.0rc0/kapitan/refs/functions.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/secrets/awskms.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/awskms.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/secrets/azkms.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/azkms.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/secrets/gkms.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/gkms.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/secrets/gpg.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/gpg.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/secrets/vaultkv.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/vaultkv.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/refs/secrets/vaulttransit.py` & `kapitan-0.32.0rc0/kapitan/refs/secrets/vaulttransit.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/remoteinventory/fetch.py` & `kapitan-0.32.0rc0/kapitan/remoteinventory/fetch.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/resources.py` & `kapitan-0.32.0rc0/kapitan/resources.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/targets.py` & `kapitan-0.32.0rc0/kapitan/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,15 +654,14 @@
                         "output_path": {"type": "string"},
                         "source": {"type": "string"},
                         "subdir": {"type": "string"},
                         "ref": {"type": "string"},
                         "unpack": {"type": "boolean"},
                         "version": {"type": "string"},
                         "force_fetch": {"type": "boolean"},
-                        "submodules": {"type": "boolean"},
                     },
                     "required": ["type", "output_path", "source"],
                     "additionalProperties": False,
                     "allOf": [
                         {
                             "if": {"properties": {"type": {"enum": ["http", "https"]}}},
                             "then": {
```

### Comparing `kapitan-0.32.0/kapitan/utils.py` & `kapitan-0.32.0rc0/kapitan/utils.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/kapitan/validator/kubernetes_validator.py` & `kapitan-0.32.0rc0/kapitan/validator/kubernetes_validator.py`

 * *Files identical despite different names*

### Comparing `kapitan-0.32.0/pyproject.toml` & `kapitan-0.32.0rc0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 license = "Apache-2.0"
-version = "0.32.0"
+version = "0.32.0rc0"
 packages = [
     { include = "kapitan" },
     { include = "kapitan/reclass" },
 ]
 
 [tool.poetry.scripts]
 kapitan = 'kapitan.cli:main'
```

### Comparing `kapitan-0.32.0/setup.py` & `kapitan-0.32.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 {'gojsonnet': ['gojsonnet>=0.17.0,<0.18.0'], 'test': ['docker>=5.0.0,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['kapitan = kapitan.cli:main']}
 
 setup_kwargs = {
     'name': 'kapitan',
-    'version': '0.32.0',
+    'version': '0.32.0rc0',
     'description': 'Generic templated configuration management for Kubernetes, Terraform and other things',
     'long_description': '# Kapitan: advanced configuration management tool\n\n![Unit Tests](https://github.com/kapicorp/kapitan/actions/workflows/test.yml/badge.svg)\n![Python Version](https://img.shields.io/pypi/pyversions/kapitan)\n![Downloads](https://img.shields.io/pypi/dm/kapitan)\n![Docker Pulls](https://img.shields.io/docker/pulls/kapicorp/kapitan)\n[![Docker](https://github.com/kapicorp/kapitan/workflows/Docker%20Build%20and%20Push/badge.svg)](https://github.com/kapicorp/kapitan/actions?query=workflow%3A%22Docker+Build+and+Push%22)\n[![Releases](https://img.shields.io/github/release/kapicorp/kapitan.svg)](https://github.com/kapicorp/kapitan/releases)\n[![Docker Image Size](https://img.shields.io/docker/image-size/kapicorp/kapitan/latest.svg)](https://hub.docker.com/r/kapicorp/kapitan)\n\n<img src="docs/images/kapitan_logo.png" width="25">\n\n\n**`Kapitan`** aims to be your *one-stop tool* to help you manage the ever growing complexity of your configurations.\n\nJoin the community [`#kapitan`](https://kubernetes.slack.com/archives/C981W2HD3)\n\n## [**Official site**](https://kapitan.dev) <https://kapitan.dev>\n\n\n## [**Quick Start**](https://kapitan.dev/kapitan_overview/#quickstart)\n\n## Install Kapitan\n\n### Docker (recommended)\n\n```shell\ndocker run -t --rm -v $(pwd):/src:delegated kapicorp/kapitan -h\n```\n\nOn Linux you can add `-u $(id -u)` to `docker run` to preserve file permissions.\n\n### Pip\n\nKapitan needs Python 3.7.\n\n#### Install Python 3.7\n\n* Linux: `sudo apt-get update && sudo apt-get install -y python3.7-dev python3-pip python3-yaml git`\n* Mac: `brew install python3 libyaml git libmagic`\n\n#### Install Kapitan\n\nUser (`$HOME/.local/lib/python3.7/bin` on Linux or `$HOME/Library/Python/3.7/bin` on macOS):\n\n```shell\npip3 install --user --upgrade kapitan\n```\n\nSystem-wide (not recommended):\n\n```shell\nsudo pip3 install --upgrade kapitan\n```\n\n## Build Kapitan\n\n### Docker\n\nTo build a docker image for the architecture of your machine, run `docker build . -t you-kapitan-image`, and to build for a specific platform, add `--platform linux/arm64`.\n\nTo build a multi-platform image (as the CI does), follow [the docker multi-platform documentation](https://docs.docker.com/build/building/multi-platform/).\n\n## Related projects\n\n* [Tesoro](https://github.com/kapicorp/tesoro) - Kubernetes Admission Controller for Kapitan Secrets\n* [Kapitan Reference](https://github.com/kapicorp/kapitan-reference) - our reference repository to get started with Kapitan\n',
     'author': 'Ricardo Amaro',
     'author_email': 'ramaro@kapicorp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kapicorp/kapitan',
```

### Comparing `kapitan-0.32.0/PKG-INFO` & `kapitan-0.32.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kapitan
-Version: 0.32.0
+Version: 0.32.0rc0
 Summary: Generic templated configuration management for Kubernetes, Terraform and other things
 Home-page: https://github.com/kapicorp/kapitan
 License: Apache-2.0
 Keywords: jsonnet,kubernetes,reclass,jinja
 Author: Ricardo Amaro
 Author-email: ramaro@kapicorp.com
 Requires-Python: >=3.8,<4.0
```

