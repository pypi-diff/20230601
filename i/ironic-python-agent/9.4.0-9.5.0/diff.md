# Comparing `tmp/ironic-python-agent-9.4.0.tar.gz` & `tmp/ironic-python-agent-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironic-python-agent-9.4.0.tar", last modified: Thu Mar  9 14:14:43 2023, max compression
+gzip compressed data, was "ironic-python-agent-9.5.0.tar", last modified: Thu Jun  1 15:04:03 2023, max compression
```

## Comparing `ironic-python-agent-9.4.0.tar` & `ironic-python-agent-9.5.0.tar`

### file list

```diff
@@ -1,455 +1,462 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8005 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    66866 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3389 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.610610 ironic-python-agent-9.4.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.610610 ironic-python-agent-9.4.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.610610 ironic-python-agent-9.4.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5637 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/admin/hardware_managers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8560 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/admin/how_it_works.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/admin/rescue.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10282 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/admin/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.610610 ironic-python-agent-9.4.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12004 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/contributor/hardware_managers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/contributor/metrics.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/contributor/rescue.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.610610 ironic-python-agent-9.4.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.610610 ironic-python-agent-9.4.0/examples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.614610 ironic-python-agent-9.4.0/examples/business-logic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/business-logic/example_business_logic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/business-logic/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/business-logic/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.614610 ironic-python-agent-9.4.0/examples/custom-disk-erase/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/custom-disk-erase/example_disk_eraser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/custom-disk-erase/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/custom-disk-erase/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.614610 ironic-python-agent-9.4.0/examples/vendor-device/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6669 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/vendor-device/example_device.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/vendor-device/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/examples/vendor-device/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.614610 ironic-python-agent-9.4.0/imagebuild/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/imagebuild/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.618610 ironic-python-agent-9.4.0/ironic_python_agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20176 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.618610 ironic-python-agent-9.4.0/ironic_python_agent/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8659 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16063 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/burnin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.622610 ironic-python-agent-9.4.0/ironic_python_agent/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/cmd/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/cmd/inspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18081 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4090 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/dmi_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15561 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/efi_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2692 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11927 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/errors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.622610 ironic-python-agent-9.4.0/ironic_python_agent/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13990 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/clean.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4307 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1828 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33196 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1700 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/poll.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/rescue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38529 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/extensions/standby.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   138697 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/hardware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.622610 ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3333 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/cna.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6505 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/mlnx.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.622610 ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/nvidia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35106 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9476 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/inject_files.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5148 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/inspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13636 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11683 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/ironic_api_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13537 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10331 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/numa_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27322 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/partition_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17303 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/raid_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.622610 ironic-python-agent-9.4.0/ironic_python_agent/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.626611 ironic-python-agent-9.4.0/ironic_python_agent/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/functional/test_commands.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.630611 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22841 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/dmi_inspector_data.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.630611 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10145 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11831 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_clean.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11843 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_deploy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   110484 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_log.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_poll.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_rescue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77457 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_standby.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.630611 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.634611 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51518 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7608 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.634611 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49597 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/samples/hardware_samples.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50981 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13193 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21146 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_burnin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4833 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_dmi_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24359 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_efi_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_encoding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6022 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   280450 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_hardware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17824 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_inject_files.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22517 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22909 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_ironic_api_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7947 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_multi_hardware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4665 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13272 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_netutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18131 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_numa_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67228 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_partition_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17609 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_raid_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_tls_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49689 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/tls_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32893 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/ironic_python_agent/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.618610 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3389 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22806 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2023-03-09 14:14:43.000000 ironic-python-agent-9.4.0/ironic_python_agent.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/plugin-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.634611 ironic-python-agent-9.4.0/releasenotes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/config.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.674614 ironic-python-agent-9.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/LLDP-ignore-NICs-that-are-not-plugged-in-29213f0a701a72e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ability-to-disable-secure-erase-c3223262726d5aff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-block-device-uuid-c8b38264e1688110.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-coreos-dhcp-rescue-support-1dd8e9d5ac9c7594.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-disk-wait-config-opts-fe805292baca8029.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-erase-devices-express-1df107c75f2b3627.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-hostname-8bbf24712b6a4919.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-inspection-retry-1d385f69607c1452.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-log-extension-35ca22cc0709af4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-more-lan-channels-8f5197ed5f057c25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-named-logfiles-to-burnin-4388309bf7442d53.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-numa-topology-info-8c253fd9e56169f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-optional-tls-support-3ab6a834154fedec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-pci-devices-info-3f86934a505d1b31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-portal-port-arg-6d4faec2f709c8e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-secondary-sorting-by-name-for-root-disks-4de2c0358b9a1e2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-smart-test-to-disk-burnin-d02d31e23e5efa9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-unit-test-cc4a1a05859ad17d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-vendor-info-56be9a8605d80bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_burnin_cpu-9acbb36048246a6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_burnin_disk-12adb5735a41af47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_burnin_memory-4099ca42bd3b99db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_burnin_network-4856153d21c25f4a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_erase_pstore-b109c58ed8f5d351.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_interface_vendor_and_product-74e9815f20ee0cac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/add_mellanox_hardware_manager-edfae87964737df1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/additional-wwn-hints-ffd02ceafcb3dc70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/adds-nvme-secure-erase-0ecfd624e5f50581.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/advertise-address-c3b152fe475fb539.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/advertise-protocol-110ae1587f727e62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/agent-fully-retries-image-downloads-67409a493c6d08ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/agent-token-support-1086218cf2a0c917.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/agent_partition_image-91941adc6683c673.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/append-efi-partition-to-fstab-e9f945a4dd19bd7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/apply-raid-aeca7848c6320d6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/auto-tls-b52b873663f35618.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/avoid-grub2-using-efibootmgr-bd27c0978d1cf71b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/bindmount-run-4c6a31d3ee4e0ed6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/block-device-hctl-e81573812be3d469.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/bmc-mac-introspection-e4c2e203d8529710.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/boot-info-f18336ada089f6dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/bootloader-ignored-uefi-mode-8578a009d5b5be62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/bug-2010123-d4c38d8f6606d0e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/build-tinyipa-with-python3-d4a64aa18f970968.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/build-tinyipa-with-tinycore8-b39d0415b1c25f6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/bumpsipalookupattempts-29de7c949aaf6556.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/capture-early-logging-0f3fa58d75656117.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/change-heartbeat-method-d0119406137022e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/check-if-ESP-is-mounted-f9e0eff3609c2668.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/check-partition-table-after-writing-34efbd557d8de7cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/clarify-heartbeat-connection-errors-2af152bf2d7928e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/clock-skew-1fbf542b193cec17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/coalesce_heartbeats-fb8899a5f9fe4709.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/collect-dmi-output-f2e9feabef16bacf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/collect-manager-a80bcf370048eeec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/collect-more-8bc9ad4c63e873e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/collect-udev-f6ada5163cf4a26c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/command_params-869fa547b5be2236.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/configdrive-dup-3fc46a878fe82485.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/configdrive-ssl-02b069948dfef814.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/container-poweroff-d9ffb637cf1cee6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/coreos-uses-chroot-8a01ba0b38a4a4f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/coreos_ipa_image_poweroff_reboot_in_chroot_by_sysrq-42447fc4cdd7dafe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/correct-uefi-regex-112211c2427cd4d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/correction-failure-output-when-downloading-image-39f93838d1ed2928.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/cpu-flags-e3cec7e5cba069ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/create_raids_with_volume_name-93e0bb59ef210fe4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/de-duplicate-by-label-baa090c5b1bff992.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/detect-endianness-f53a6c4571aba3fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/device-hints-from-node-object-9a689f5a4175a1a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/discover-ipv6-bmc-address-b3b357ff6c5d822c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/disk-label-fix-536897e41a4d817f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/disk-wait-2e0e85e0947f80e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/drop-python2-2006fd8a4a6de56d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/efi-partuuid-5fe933a462eeede1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/enable-skipping-disks-0c4c8b72231715a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/enable-skipping-raids-40263cc3a19cfd27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/enhance-checksum-2256ffdcce13836e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/erase-deploy-step-3e952fa863bca908.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/erase-device-metadata-clean-step-31b4a615c0ff7f18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/erase_metadata_from_partitions-4f1902533d530b8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/executes-gpt-partition-fix-b6156cc16da00dfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/extend-pci-metric-5482284d6a9fe765.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/extend-retry-timeout-30c930a33d97c193.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fail_ipa_start_if_ironic_api_invalid-7b78fcaba2141cc5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fallback-to-findfs-59abde55221e1e84.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fasttrack-stale-cache-fd93b56a955c7ab1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/feature-2010228-cf3a59b88f07c3a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/findbonds-733c7c91a5665b05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-agent-determination-of-partition-table-type-3c78bf78266e8cef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-agent-unable-to-stop-py3-6c210793476968d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-auxillarly-node-lookup-argument-83d3f717c039e454.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-bmc-ip-detection-for-coreos-483be0286593e393.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-boot-mode-for-partition-images-f96cf2b3c27b6533.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-bootloader-install-with-mdraid-0a254035df9d0bed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-bytes-json-serializable-collected-logs-ad61022b287dc3e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-clean-config-for-full-device-28ee09b58d97d122.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-cleaning-read-only-device-c8a0f4cc2f434d99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-coreos-modprobe-75bda45c7bbeb469.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-hardcoded-path-to-grub-7006f29a9ef72e75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-high-cpu-usage-eventlet-1dccf3b81dd42c47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-local-boot-for-partition-images-755f570dc0982868.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-mlnx-hardware-mgr-never-run-72072580be4d6e7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-nic-without-numa-node-b401f97c46afa4a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-nvme-partition-image-handling-b8487133a188fd32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-nvme-software-raid-race-2e0e104de9611228.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-physical-memory-arm64-957755f6cd91ad85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-rescan-device-7b00c6836b687ce8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-rescan-device-raid-29aa1558b036b496.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-softraid-name-poisoning-4e934dd4e60830b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-to-pass-root-uuid-for-whole-disk-image-1c13b70f6b74bce0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-uefi-boot-entry-creation-for-aarch64-2b143c5bf189c2f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix-vfd-mount-for-capitalized-device-name-db7f519e900f4e22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix_chronyd_time_sync-626a14b66ca37677.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix_efi_uuid_fstab-f2edbee9bfbac64a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fix_partition_cleanup-46491861c930db12.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fixes-agent-lookup-retries-1b4bb90b8e783aca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/fixes-error-handling-of-efibootmgr-not-present-in-ramdisk-f11b4241edcf0e81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/get-holder-disks-with-nvme-7d5fa75df2fd5904.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/get-physical-memory-535a32362bcdf83a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/get_md_components_by_uuid-7f08d423ea9e7c94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/handle-configdrive-large-disks-3517e9fcf16c7f39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/handle-fd0-devices-3d1f31c3b34819e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/image-checksum-39b2ceef40933c28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/image-download-retries-65ac31fe4328e438.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/improve-tgtd-status-d17173dc8f67959f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/inject-files-b411369ce6856dac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/inspect-to-clean-b3616d843775c187.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/inspection-to-report-disk-by-path-e3fd4c331d200903.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/inspection-wait-for-ips-223e39b65fef31bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/inspection-wait-for-ips-v2-146016f758d7010c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/inspector-logs-9b7c010c219691d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/instance-info-root-device-02fed0966bb00fb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/inventory-conf-29b59ebe97aefbde.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ip6-addresses-1c2b9bcd9a124de7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ipa-debug-68c86101b1fdc3d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ipmi-address-channel-b6b8010c41d05c1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ipmi-cleanup-a4454f6851d81c4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ipv6-listen-85d40e58156e398f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ipv6-provision-42e9000f6f6a7a3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/ironic-error-97e76d9ddacff039.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/iscsi-detection-on-diskless-hw-f27dcce3aaa35ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/let_crypt_generate_the_salt-99876591325275a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/lib-exc-41ee122eb4a04bc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/limit-qemu-img-malloc-arena-025ed84115481eae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/limit-qemu-img-ram-usage-d7b7a16ac5e9c917.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/lldp-error-handling-5b6576b378ef9c3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/lldp-loop-fdfa584caf33d847.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/log-file-7aaaf31693ddc617.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/logs-collector-non-ascii-010339bf256443c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/lsblk-all-956c1df808a169bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/lshw-cb89894be057bdc9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/lshw-no-memory-bank-size-05ea71987362986e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/manually-configure-ironic-api-version-517afd0a423036ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/md-restart-9e0d47863a086792.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/mdadm-d5b8c186182620b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/mdns-e020484e64d76edb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/min-ironic-ocata-dff80e567783e87c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/move_swraid_to_efibootmgr-d87c1bfde1661fb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/multipath-serial-615fc925984abbf7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/multiple-lan-channels-ee32d80150f990bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/name-root-device-hints-0cfc8c90d03c8bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/new-agent-api-afbe7391493749be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/new-sync-command-6f5fa55df2fd5903.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-bash-for-grub-c38369af8cc7cf26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-coreos-3345cc69009dead9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-iscsi-fd21808edbea5ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-link-local-2e861978c5c7bf30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-mac-54616606ee6b844d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-netboot-d034bb1d1d9166c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-sample-ac11bd0fa27af62a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-standalone-bb34eae2cc468837.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/no-zram-78cc6583f4f90a9c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/old-inspector-data-5e63c9bce72b4fb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/oslo-config-generator-b0f70b9fb7e23997.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/parallel-erase-disk-devices-09ea33d5443aead0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/partition_check_read_only_base_device-5bc15ac2f034aca9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/permit-pre-hashed-rescue-passwords-4275f6e697533cec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/pint-0.5-816aaf3a4f6d4a6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/poll-mode-063bd36b2b18bffb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/prefix-lldp-timeout-50acc656313d8dd2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/prepare-image-49744276cef719d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/preserve-efi-folder-contents-ea1e278b3093ec55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/prevent-needless-iscsi-cleanup-f8d602c0abc7e8ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/prioritize-lsblk-device-serials-8cae406ca5164a01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/qemu-img-ooo-write-721b8a0057ab7b8a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/qemu-write-zeros-2edbf3152c57e2b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/raid-esp-size-2c322adb2d3b9ce7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/raid-hints-604f9ffdd86432eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/raid5-6-support-0807597c3633a26c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/readd_missing_devs-2ed85805388b6e42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/relax-checksum-feeding-11044ae02b411a07.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/remove-lldp-timeout-ea481dbb01a39522.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/remove-switch_port_descr-switch_chassis_descr-40f2bb37b5f1fdd1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/remove-sysrq-2c2804930180f408.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/remove-vendor-passthru-eda3519c322eb4e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/rescan-before-checking-uefi-64597c937880134d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/rescan-device-after-mkfs-3f9d52a2e3b6fff3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/rescue-dhcp_network-for-tinyipa-a14de5fae38a5dce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/respect-listen-directives-94fb863c5b692c07.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/rework-ata-secure-erase-c6684962ef078281.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/root-device-hints-rotational-67e6e61074c26561.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/set-clock-prior-to-poweroff-af6ec210aad8b45a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/skip-lookup-and-heartbeat-if-apiurl-not-configured-5ae8b04ae1e74673.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/skips-bootloader-install-35c463195aa61800.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/sleep-ebe58fbe07d30219.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/softraid-creation-on-nvme-a2fd4c531d200904.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/softraid-zap-superblocks-anywhere.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/software-raid-4a88e6c5af9ea742.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/software-raid-raid-ESPs-25a2aa117b99620a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/software-raid-use-label-as-rootfs-uuid-d9a3827180f1a238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/software_raid_use_rootfs_uuid-9149cc0c8638d5d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/start_passing_agent_version_to_ironic-6fa8670ae0e7eb38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/streaming-partition-images-cdeb260ef8f90012.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/streaming-uuid-fdf136a7745fbb3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/support-collecting-ipv6-address-dd819d543f851a63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/support-image-proxy-e2987a6589375451.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/support-linux-io-6bbd7ff1f0d70a0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/support-prep-partitions-5e273572ab7ce018.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/suse-tinyipa-support-20acecd6d7b20952.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/sw-raid-assemble-9c20fe967f73d1dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/timeout_on_file_download-ed77918318316075.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/tinycore-ipv6-1b620c61402b5720.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/tinyipa-python3-default-b8434793e17465db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/tinyipa-rescue-dhcp-multi-tenant-b32bda7bf2b12679.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/tinyipa-ssh-e8a3a01a3f3ff5f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/udev-settle-f75db34db990ad68.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/udevadm-settle-9d3e5f1f20211857.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/uefi-esp-660fc2c650e6af92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/uefi-fallback-266c647f6aff58fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/uefi-images-38c8536db189ffc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/up-qemuimg-mem-1536183a02b3a235.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/use-latest-coreos-87f826d26b46548d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/use-system-random-00b0721c8ebd0c5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/vmedia-copy-6a58f3183b166c42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/wait-for-interfaces-before-lookup-9bf38852b2f176a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/wait-root-device-504b517c3aec73e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/whole-disk-grub-0b1b8b9c44e31d28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/notes/zero-size-78d3be2ac8fd59c2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9278 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2450 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8385 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/tools/bandit.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/tools/config/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1015 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/tools/config/check_uptodate.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/tools/config/ipa-config-generator.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1233 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/tools/run_bashate.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4445 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-09 14:14:43.678614 ironic-python-agent-9.4.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5210 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/zuul.d/ironic-python-agent-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1529 2023-03-09 14:13:52.000000 ironic-python-agent-9.4.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8005 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67467 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3387 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.816062 ironic-python-agent-9.5.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.816062 ironic-python-agent-9.5.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.816062 ironic-python-agent-9.5.0/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7514 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/admin/hardware_managers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10359 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/admin/how_it_works.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/admin/rescue.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10282 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/admin/troubleshooting.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2394 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.820062 ironic-python-agent-9.5.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12004 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/contributor/hardware_managers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/contributor/metrics.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/contributor/rescue.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.820062 ironic-python-agent-9.5.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.820062 ironic-python-agent-9.5.0/examples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.820062 ironic-python-agent-9.5.0/examples/business-logic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/business-logic/example_business_logic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/business-logic/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/business-logic/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.820062 ironic-python-agent-9.5.0/examples/custom-disk-erase/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/custom-disk-erase/example_disk_eraser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/custom-disk-erase/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/custom-disk-erase/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.820062 ironic-python-agent-9.5.0/examples/vendor-device/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6669 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/vendor-device/example_device.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/vendor-device/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/examples/vendor-device/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.820062 ironic-python-agent-9.5.0/imagebuild/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/imagebuild/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.824062 ironic-python-agent-9.5.0/ironic_python_agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20278 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.824062 ironic-python-agent-9.5.0/ironic_python_agent/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8659 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16063 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/burnin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.824062 ironic-python-agent-9.5.0/ironic_python_agent/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/cmd/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/cmd/inspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18396 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4090 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/dmi_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15965 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/efi_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2692 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11927 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/errors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.828062 ironic-python-agent-9.5.0/ironic_python_agent/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13990 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/clean.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4307 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1828 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33196 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1700 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/poll.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2610 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/rescue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43287 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/extensions/standby.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   140713 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/hardware.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.828062 ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3333 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/cna.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6505 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/mlnx.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.828062 ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/nvidia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35106 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9476 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/inject_files.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5148 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/inspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13918 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11683 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/ironic_api_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14227 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10331 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/numa_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27322 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/partition_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17303 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/raid_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.828062 ironic-python-agent-9.5.0/ironic_python_agent/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.828062 ironic-python-agent-9.5.0/ironic_python_agent/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3838 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3656 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/functional/test_commands.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.832062 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22841 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/dmi_inspector_data.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.832062 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10145 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11831 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_clean.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11843 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_deploy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   110879 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_log.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_poll.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_rescue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    94484 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_standby.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.832062 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.836062 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51518 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7608 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.836062 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52463 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/samples/hardware_samples.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50981 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13193 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21146 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_burnin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4833 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_dmi_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25270 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_efi_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2763 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_encoding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6022 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   277184 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_hardware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17824 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_inject_files.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22517 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22909 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_ironic_api_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7947 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_multi_hardware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4665 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13272 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_netutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18131 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_numa_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67228 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_partition_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17609 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_raid_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_tls_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49689 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/tls_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33708 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/ironic_python_agent/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.824062 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3387 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23215 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2023-06-01 15:04:03.000000 ironic-python-agent-9.5.0/ironic_python_agent.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/plugin-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.836062 ironic-python-agent-9.5.0/releasenotes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/config.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.868062 ironic-python-agent-9.5.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/LLDP-ignore-NICs-that-are-not-plugged-in-29213f0a701a72e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ability-to-disable-secure-erase-c3223262726d5aff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-block-device-uuid-c8b38264e1688110.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-coreos-dhcp-rescue-support-1dd8e9d5ac9c7594.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-disk-wait-config-opts-fe805292baca8029.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-erase-devices-express-1df107c75f2b3627.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-hostname-8bbf24712b6a4919.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-inspection-retry-1d385f69607c1452.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-log-extension-35ca22cc0709af4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-more-lan-channels-8f5197ed5f057c25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-named-logfiles-to-burnin-4388309bf7442d53.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-numa-topology-info-8c253fd9e56169f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-optional-tls-support-3ab6a834154fedec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-pci-devices-info-3f86934a505d1b31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-portal-port-arg-6d4faec2f709c8e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-secondary-sorting-by-name-for-root-disks-4de2c0358b9a1e2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-smart-test-to-disk-burnin-d02d31e23e5efa9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-unit-test-cc4a1a05859ad17d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-vendor-info-56be9a8605d80bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_burnin_cpu-9acbb36048246a6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_burnin_disk-12adb5735a41af47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_burnin_memory-4099ca42bd3b99db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_burnin_network-4856153d21c25f4a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_erase_pstore-b109c58ed8f5d351.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_interface_vendor_and_product-74e9815f20ee0cac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/add_mellanox_hardware_manager-edfae87964737df1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/additional-wwn-hints-ffd02ceafcb3dc70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/adds-nvme-secure-erase-0ecfd624e5f50581.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/advertise-address-c3b152fe475fb539.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/advertise-protocol-110ae1587f727e62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/agent-fully-retries-image-downloads-67409a493c6d08ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/agent-token-support-1086218cf2a0c917.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/agent_partition_image-91941adc6683c673.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/append-efi-partition-to-fstab-e9f945a4dd19bd7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/apply-raid-aeca7848c6320d6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/auto-tls-b52b873663f35618.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/avoid-grub2-using-efibootmgr-bd27c0978d1cf71b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/bindmount-run-4c6a31d3ee4e0ed6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/block-device-hctl-e81573812be3d469.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/bmc-mac-introspection-e4c2e203d8529710.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/bmo-extra-147559c8d1776e8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/boot-info-f18336ada089f6dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/bootloader-ignored-uefi-mode-8578a009d5b5be62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/bug-2010123-d4c38d8f6606d0e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/build-tinyipa-with-python3-d4a64aa18f970968.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/build-tinyipa-with-tinycore8-b39d0415b1c25f6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/bumpsipalookupattempts-29de7c949aaf6556.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/capture-early-logging-0f3fa58d75656117.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/change-heartbeat-method-d0119406137022e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/check-if-ESP-is-mounted-f9e0eff3609c2668.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/check-partition-table-after-writing-34efbd557d8de7cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/clarify-heartbeat-connection-errors-2af152bf2d7928e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/clock-skew-1fbf542b193cec17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/coalesce_heartbeats-fb8899a5f9fe4709.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/collect-dmi-output-f2e9feabef16bacf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/collect-manager-a80bcf370048eeec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/collect-more-8bc9ad4c63e873e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/collect-udev-f6ada5163cf4a26c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/command_params-869fa547b5be2236.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/configdrive-dup-3fc46a878fe82485.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/configdrive-ssl-02b069948dfef814.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/container-poweroff-d9ffb637cf1cee6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/coreos-uses-chroot-8a01ba0b38a4a4f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/coreos_ipa_image_poweroff_reboot_in_chroot_by_sysrq-42447fc4cdd7dafe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/correct-uefi-regex-112211c2427cd4d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/correction-failure-output-when-downloading-image-39f93838d1ed2928.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/cpu-flags-e3cec7e5cba069ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/create_raids_with_volume_name-93e0bb59ef210fe4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/de-duplicate-by-label-baa090c5b1bff992.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1703 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/detect-endianness-f53a6c4571aba3fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/device-hints-from-node-object-9a689f5a4175a1a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/disable-md5-image-checksum-7def176928d36e75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/discover-ipv6-bmc-address-b3b357ff6c5d822c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/disk-label-fix-536897e41a4d817f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/disk-wait-2e0e85e0947f80e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/drop-python2-2006fd8a4a6de56d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/efi-partuuid-5fe933a462eeede1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/enable-skipping-disks-0c4c8b72231715a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/enable-skipping-raids-40263cc3a19cfd27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/enhance-checksum-2256ffdcce13836e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/erase-deploy-step-3e952fa863bca908.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/erase-device-metadata-clean-step-31b4a615c0ff7f18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/erase_metadata_from_partitions-4f1902533d530b8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/executes-gpt-partition-fix-b6156cc16da00dfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/extend-pci-metric-5482284d6a9fe765.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/extend-retry-timeout-30c930a33d97c193.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fail_ipa_start_if_ironic_api_invalid-7b78fcaba2141cc5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fallback-to-findfs-59abde55221e1e84.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fasttrack-stale-cache-fd93b56a955c7ab1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/feature-2010228-cf3a59b88f07c3a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fetc-checksum-support-additional-format-4b29c5cdaa6b8d16.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/findbonds-733c7c91a5665b05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-agent-determination-of-partition-table-type-3c78bf78266e8cef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-agent-unable-to-stop-py3-6c210793476968d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-auxillarly-node-lookup-argument-83d3f717c039e454.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-bmc-ip-detection-for-coreos-483be0286593e393.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-boot-mode-for-partition-images-f96cf2b3c27b6533.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-bootloader-install-with-mdraid-0a254035df9d0bed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-bytes-json-serializable-collected-logs-ad61022b287dc3e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-clean-config-for-full-device-28ee09b58d97d122.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-cleaning-read-only-device-c8a0f4cc2f434d99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-coreos-modprobe-75bda45c7bbeb469.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-hardcoded-path-to-grub-7006f29a9ef72e75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-high-cpu-usage-eventlet-1dccf3b81dd42c47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-local-boot-for-partition-images-755f570dc0982868.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-mlnx-hardware-mgr-never-run-72072580be4d6e7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-nic-without-numa-node-b401f97c46afa4a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-nvme-partition-image-handling-b8487133a188fd32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-nvme-software-raid-race-2e0e104de9611228.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-physical-memory-arm64-957755f6cd91ad85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-rescan-device-7b00c6836b687ce8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-rescan-device-raid-29aa1558b036b496.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-softraid-name-poisoning-4e934dd4e60830b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-to-pass-root-uuid-for-whole-disk-image-1c13b70f6b74bce0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-uefi-boot-entry-creation-for-aarch64-2b143c5bf189c2f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix-vfd-mount-for-capitalized-device-name-db7f519e900f4e22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix_chronyd_time_sync-626a14b66ca37677.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix_efi_uuid_fstab-f2edbee9bfbac64a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fix_partition_cleanup-46491861c930db12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fixes-agent-lookup-retries-1b4bb90b8e783aca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fixes-efibootmgr-character-encoding-19e531ba694824c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/fixes-error-handling-of-efibootmgr-not-present-in-ramdisk-f11b4241edcf0e81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/get-holder-disks-with-nvme-7d5fa75df2fd5904.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/get-physical-memory-535a32362bcdf83a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/get_md_components_by_uuid-7f08d423ea9e7c94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/handle-configdrive-large-disks-3517e9fcf16c7f39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/handle-fd0-devices-3d1f31c3b34819e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/image-checksum-39b2ceef40933c28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/image-download-retries-65ac31fe4328e438.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/improve-tgtd-status-d17173dc8f67959f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/inject-files-b411369ce6856dac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/inspect-to-clean-b3616d843775c187.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/inspection-to-report-disk-by-path-e3fd4c331d200903.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/inspection-wait-for-ips-223e39b65fef31bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/inspection-wait-for-ips-v2-146016f758d7010c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/inspector-logs-9b7c010c219691d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/instance-info-root-device-02fed0966bb00fb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/inventory-conf-29b59ebe97aefbde.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ip6-addresses-1c2b9bcd9a124de7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ipa-debug-68c86101b1fdc3d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ipmi-address-channel-b6b8010c41d05c1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ipmi-cleanup-a4454f6851d81c4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ipv6-listen-85d40e58156e398f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ipv6-provision-42e9000f6f6a7a3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/ironic-error-97e76d9ddacff039.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/iscsi-detection-on-diskless-hw-f27dcce3aaa35ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/let_crypt_generate_the_salt-99876591325275a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lib-exc-41ee122eb4a04bc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/limit-qemu-img-malloc-arena-025ed84115481eae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/limit-qemu-img-ram-usage-d7b7a16ac5e9c917.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lldp-error-handling-5b6576b378ef9c3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lldp-loop-fdfa584caf33d847.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lldp-raw-a09174cb930bca97.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/log-file-7aaaf31693ddc617.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/logs-collector-non-ascii-010339bf256443c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lsblk-all-956c1df808a169bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lshw-cb89894be057bdc9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/lshw-no-memory-bank-size-05ea71987362986e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/manually-configure-ironic-api-version-517afd0a423036ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/md-restart-9e0d47863a086792.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/mdadm-d5b8c186182620b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/mdns-e020484e64d76edb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/min-ironic-ocata-dff80e567783e87c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/move_swraid_to_efibootmgr-d87c1bfde1661fb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/multipath-serial-615fc925984abbf7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/multiple-lan-channels-ee32d80150f990bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/name-root-device-hints-0cfc8c90d03c8bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/net-speed-8854901e2051bb79.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/new-agent-api-afbe7391493749be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/new-sync-command-6f5fa55df2fd5903.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-bash-for-grub-c38369af8cc7cf26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-coreos-3345cc69009dead9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-iscsi-fd21808edbea5ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-link-local-2e861978c5c7bf30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-mac-54616606ee6b844d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-netboot-d034bb1d1d9166c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-sample-ac11bd0fa27af62a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-standalone-bb34eae2cc468837.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/no-zram-78cc6583f4f90a9c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/old-inspector-data-5e63c9bce72b4fb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/oslo-config-generator-b0f70b9fb7e23997.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/parallel-erase-disk-devices-09ea33d5443aead0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/partition_check_read_only_base_device-5bc15ac2f034aca9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/permit-pre-hashed-rescue-passwords-4275f6e697533cec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/pint-0.5-816aaf3a4f6d4a6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/poll-mode-063bd36b2b18bffb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/prefix-lldp-timeout-50acc656313d8dd2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/prepare-image-49744276cef719d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/preserve-efi-folder-contents-ea1e278b3093ec55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/prevent-needless-iscsi-cleanup-f8d602c0abc7e8ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/prioritize-lsblk-device-serials-8cae406ca5164a01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/qemu-img-ooo-write-721b8a0057ab7b8a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/qemu-write-zeros-2edbf3152c57e2b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/raid-esp-size-2c322adb2d3b9ce7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/raid-hints-604f9ffdd86432eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/raid5-6-support-0807597c3633a26c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/readd_missing_devs-2ed85805388b6e42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/relax-checksum-feeding-11044ae02b411a07.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/remove-lldp-timeout-ea481dbb01a39522.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/remove-switch_port_descr-switch_chassis_descr-40f2bb37b5f1fdd1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/remove-sysrq-2c2804930180f408.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/remove-vendor-passthru-eda3519c322eb4e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/rescan-before-checking-uefi-64597c937880134d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/rescan-device-after-mkfs-3f9d52a2e3b6fff3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/rescue-dhcp_network-for-tinyipa-a14de5fae38a5dce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/respect-listen-directives-94fb863c5b692c07.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/rework-ata-secure-erase-c6684962ef078281.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/root-device-hints-rotational-67e6e61074c26561.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/set-clock-prior-to-poweroff-af6ec210aad8b45a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/skip-lookup-and-heartbeat-if-apiurl-not-configured-5ae8b04ae1e74673.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/skips-bootloader-install-35c463195aa61800.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/sleep-ebe58fbe07d30219.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/softraid-creation-on-nvme-a2fd4c531d200904.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/softraid-zap-superblocks-anywhere.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/software-raid-4a88e6c5af9ea742.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/software-raid-raid-ESPs-25a2aa117b99620a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/software-raid-use-label-as-rootfs-uuid-d9a3827180f1a238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/software_raid_use_rootfs_uuid-9149cc0c8638d5d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/start_passing_agent_version_to_ironic-6fa8670ae0e7eb38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/streaming-partition-images-cdeb260ef8f90012.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/streaming-uuid-fdf136a7745fbb3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/support-collecting-ipv6-address-dd819d543f851a63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/support-image-proxy-e2987a6589375451.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/support-linux-io-6bbd7ff1f0d70a0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/support-prep-partitions-5e273572ab7ce018.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/suse-tinyipa-support-20acecd6d7b20952.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/sw-raid-assemble-9c20fe967f73d1dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/timeout_on_file_download-ed77918318316075.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/tinycore-ipv6-1b620c61402b5720.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/tinyipa-python3-default-b8434793e17465db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/tinyipa-rescue-dhcp-multi-tenant-b32bda7bf2b12679.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/tinyipa-ssh-e8a3a01a3f3ff5f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/udev-settle-f75db34db990ad68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/udevadm-settle-9d3e5f1f20211857.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/uefi-esp-660fc2c650e6af92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/uefi-fallback-266c647f6aff58fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/uefi-images-38c8536db189ffc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/up-qemuimg-mem-1536183a02b3a235.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/use-latest-coreos-87f826d26b46548d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/use-system-random-00b0721c8ebd0c5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/vmedia-copy-6a58f3183b166c42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/wait-for-interfaces-before-lookup-9bf38852b2f176a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/wait-root-device-504b517c3aec73e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/whole-disk-grub-0b1b8b9c44e31d28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/notes/zero-size-78d3be2ac8fd59c2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9279 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-06-01 15:04:03.876062 ironic-python-agent-9.5.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8385 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/tools/bandit.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/tools/config/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1015 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/tools/config/check_uptodate.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/tools/config/ipa-config-generator.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1233 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/tools/run_bashate.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4438 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-06-01 15:04:03.872062 ironic-python-agent-9.5.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5210 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/zuul.d/ironic-python-agent-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1529 2023-06-01 15:02:18.000000 ironic-python-agent-9.5.0/zuul.d/project.yaml
```

### Comparing `ironic-python-agent-9.4.0/AUTHORS` & `ironic-python-agent-9.5.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ChangeLog` & `ironic-python-agent-9.5.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 CHANGES
 =======
 
+9.5.0
+-----
+
+* Follow-up Add documentation for MellanoxDeviceHardwareManager
+* Ironic (and IPA) use launchpad now
+* Revert disabling MD5 checksums
+* Add support for CentOS SUM files
+* Add network interface speed to the inventory
+* Fix checksum validation logic
+* Deprecate LLDP in inventory in favour of a new collector
+* Disable MD5 image checksums
+* Upgrade to latest hacking - v6
+* Fix UTF-16 result handling for efibootmgr
+* Report system firmware information in the inventory
+* Trivial: formatting issue in the inventory docs
+* [Trivial] Fix typo in efi\_utils
+* Update master for stable/2023.1
+
 9.4.0
 -----
 
 
 9.3.0
 -----
```

### Comparing `ironic-python-agent-9.4.0/LICENSE` & `ironic-python-agent-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/PKG-INFO` & `ironic-python-agent-9.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironic-python-agent
-Version: 9.4.0
+Version: 9.5.0
 Summary: Ironic Python Agent Ramdisk
 Home-page: https://docs.openstack.org/ironic-python-agent/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: ===================
         Ironic Python Agent
@@ -43,32 +43,32 @@
         
         This is covered in the `Deploying Ironic with DevStack <https://docs.openstack.org/ironic/latest/contributor/dev-quickstart.html#deploying-ironic-with-devstack>`_
         section of the Ironic dev-quickstart guide.
         
         
         Project Resources
         =================
-        Project status, features, and bugs are tracked on StoryBoard:
+        Project bugs are tracked on Launchpad:
         
-          https://storyboard.openstack.org/#!/project/947
+          https://bugs.launchpad.net/ironic-python-agent/+bugs
         
         Developer documentation can be found here:
         
           https://docs.openstack.org/ironic-python-agent/latest/
         
         Release notes for the project are available at:
         
           https://docs.openstack.org/releasenotes/ironic-python-agent/
         
         Source code repository for the project is located at:
         
           https://opendev.org/openstack/ironic-python-agent/
         
         IRC channel:
-            #openstack-ironic
+            #openstack-ironic on irc.oftc.net
         
         To contribute, start here: `Openstack: How to
         contribute <https://docs.openstack.org/infra/manual/developers.html>`_.
         
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
```

### Comparing `ironic-python-agent-9.4.0/README.rst` & `ironic-python-agent-9.5.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -35,28 +35,28 @@
 
 This is covered in the `Deploying Ironic with DevStack <https://docs.openstack.org/ironic/latest/contributor/dev-quickstart.html#deploying-ironic-with-devstack>`_
 section of the Ironic dev-quickstart guide.
 
 
 Project Resources
 =================
-Project status, features, and bugs are tracked on StoryBoard:
+Project bugs are tracked on Launchpad:
 
-  https://storyboard.openstack.org/#!/project/947
+  https://bugs.launchpad.net/ironic-python-agent/+bugs
 
 Developer documentation can be found here:
 
   https://docs.openstack.org/ironic-python-agent/latest/
 
 Release notes for the project are available at:
 
   https://docs.openstack.org/releasenotes/ironic-python-agent/
 
 Source code repository for the project is located at:
 
   https://opendev.org/openstack/ironic-python-agent/
 
 IRC channel:
-    #openstack-ironic
+    #openstack-ironic on irc.oftc.net
 
 To contribute, start here: `Openstack: How to
 contribute <https://docs.openstack.org/infra/manual/developers.html>`_.
```

### Comparing `ironic-python-agent-9.4.0/bindep.txt` & `ironic-python-agent-9.5.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/admin/hardware_managers.rst` & `ironic-python-agent-9.5.0/doc/source/admin/hardware_managers.rst`

 * *Files 27% similar despite different names*

```diff
@@ -139,7 +139,58 @@
 
 These filesystems include IBM General Parallel File System (GPFS),
 VmWare Virtual Machine File System (VMFS), and Red Hat Global File System
 (GFS2).
 
 For information on troubleshooting, and disabling this check,
 see :doc:`/admin/troubleshooting`.
+
+==========================
+Custom hardware managers
+==========================
+
+MellanoxDeviceHardwareManager
+=============================
+
+This is a custom hardware manager for ironic-python-agent. It provides
+support for Nvidia/Mellanox NICs.
+
+* You can get the binraies firmware for all Nvidia/Mellanox NICs from here `Nvidia firmware downloads <https://network.nvidia.com/support/firmware/firmware-downloads/>`_
+
+* And you can get the deviceID from here `Nvidia/Mellanox NICs list <https://pci-ids.ucw.cz/read/PC/15b3>`_
+
+* Also you can check here `MFT decumentation <https://docs.nvidia.com/networking/display/MFTv4240/Using+mlxconfig>`_ for some supported parameters
+
+Clean steps
+-----------
+
+``update_nvidia_nic_firmware_image(node, ports, images)``
+
+A clean step used to update Nvidia/Mellanox NICs firmware images from the
+required parameter ``images`` list. it's disabled by default.
+Each image in the list is a dictionary with the following fields:
+
+``url`` (required)
+    The url of the firmware image (file://, http://).
+``checksum`` (required)
+    checksum of the provided image.
+``checksumType`` (required)
+    checksum type, it could be (md5/sha512/sha256).
+``componentFlavor`` (required)
+    The PSID of the nic.
+``version`` (required)
+    version of the firmware image , it must be the same as in the image file.
+
+``update_nvidia_nic_firmware_settings(node, ports, settings)``
+
+A clean step used to update Nvidia/Mellanox NICs firmware settings from the
+required parameter ``settings`` list. it's disabled by default.
+Each settings in the list is a dictionary with the following fields:
+
+``deviceID`` (required)
+    The ID of the NIC
+``globalConfig``
+    The global configuration for NIC
+``function0Config``
+    The per-function configuration of the first port of the NIC
+``function1Config``
+    The per-function configuration of the second port of the NIC
```

### Comparing `ironic-python-agent-9.4.0/doc/source/admin/how_it_works.rst` & `ironic-python-agent-9.5.0/doc/source/admin/how_it_works.rst`

 * *Files 15% similar despite different names*

```diff
@@ -141,16 +141,24 @@
       * ``ram`` - list of objects with keys ``numa_node`` (node ID) and
         ``size_kb``.
       * ``cpus`` - list of objects with keys ``cpu`` (CPU ID), ``numa_node``
         (node ID) and ``thread_siblings`` (list of sibling threads).
       * ``nics`` - list of objects with keys ``name`` (NIC name) and
         ``numa_node`` (node ID).
 
+``lldp``
+    Collects information about the network connectivity using LLDP_. Provides
+    one key:
+
+    * ``lldp_raw`` - mapping of interface names to lists of raw
+      type-length-value (TLV) records.
+
 .. _hardware: https://pypi.org/project/hardware/
 .. _NUMA: https://en.wikipedia.org/wiki/Non-uniform_memory_access
+.. _LLDP: https://en.wikipedia.org/wiki/Link_Layer_Discovery_Protocol
 
 .. _hardware-inventory:
 
 Hardware Inventory
 ------------------
 IPA collects various hardware information using its
 :doc:`Hardware Managers <../contributor/hardware_managers>`,
@@ -187,27 +195,65 @@
     ``uuid``, ``vendor``, ``wwn_with_extension``, ``wwn_vendor_extension``,
     ``hctl`` and ``by_path`` (the full disk path, in the form
     ``/dev/disk/by-path/<rest-of-path>``).
 
 ``interfaces``
     list of network interfaces with fields: ``name``, ``mac_address``,
     ``ipv4_address``, ``lldp``, ``vendor``, ``product``, and optionally
-    ``biosdevname``(BIOS given NIC name). If configuration option
-    ``collect_lldp`` is set to True the ``lldp`` field will be populated
-    by a list of type-length-value(TLV) fields retrieved using the
-    Link Layer Discovery Protocol (LLDP).
+    ``biosdevname`` (BIOS given NIC name) and ``speed_mbps`` (maximum supported
+    speed).
+
+    .. note::
+       For backward compatibility, interfaces may contain ``lldp`` fields.
+       They are deprecated, consumers should rely on the ``lldp`` inspection
+       collector instead.
 
 ``system_vendor``
     system vendor information from SMBIOS as reported by ``dmidecode``:
-    ``product_name``, ``serial_number`` and ``manufacturer``.
+    ``product_name``, ``serial_number`` and ``manufacturer``, as well as
+    a ``firmware`` structure with fields ``vendor``, ``version`` and
+    ``build_date``.
 
 ``boot``
     boot information with fields: ``current_boot_mode`` (boot mode used for
     the current boot - BIOS or UEFI) and ``pxe_interface`` (interface used
     for PXE booting, if any).
 
 ``hostname``
     hostname for the system
 
     .. note::
         This is most likely to be set by the DHCP server. Could be localhost
         if the DHCP server does not set it.
+
+Image Checksums
+---------------
+
+As part of the process of downloading images to be written to disk as part of
+image deployment, a series of fields are utilized to determine if the
+image which has been downloaded matches what the user stated as the expected
+image checksum utilizing the ``instance_info/image_checksum`` value.
+
+OpenStack, as a whole, has replaced the "legacy" ``checksum`` field with
+``os_hash_value`` and ``os_hash_algo`` fields, which allows for an image
+checksum and value to be asserted. An advantage of this is a variety of
+algorithms are available, if a user/operator is so-inclined.
+
+For the purposes of Ironic, we continue to support the pass-through checksum
+field as we support the checksum being retrieved via a URL.
+
+We also support determining the checksum by length.
+
+The field can be utilized to designate:
+
+* A URL to retreive a checksum from.
+* MD5 (Disabled by default, see ``[DEFAULT]md5_enabled`` in the agent
+  configuration file.)
+* SHA-2 based SHA256
+* SHA-2 based SHA512
+
+SHA-3 based checksums are not supported for auto-determination as they can
+have a variable length checksum result. At of when this documentation was
+added, SHA-2 based checksum algorithms have not been withdrawn from from
+approval. If you need to force use of SHA-3 based checksums, you *must*
+utilize the ``os_hash_algo`` setting along with the ``os_hash_value``
+setting.
```

### Comparing `ironic-python-agent-9.4.0/doc/source/admin/rescue.rst` & `ironic-python-agent-9.5.0/doc/source/admin/rescue.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/admin/troubleshooting.rst` & `ironic-python-agent-9.5.0/doc/source/admin/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/conf.py` & `ironic-python-agent-9.5.0/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 # The theme to use for HTML and HTML Help pages.  Major themes that come with
 # Sphinx are currently 'default' and 'sphinxdoc'.
 html_theme = 'openstackdocs'
 
 # openstackdocstheme options
 openstackdocs_repo_name = 'openstack/ironic-python-agent'
 openstackdocs_pdf_link = True
-openstackdocs_use_storyboard = True
+openstackdocs_use_storyboard = False
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'Ironic Python Agentdoc'
 
 latex_use_xindy = False
 
 # Grouping the document tree into LaTeX files. List of tuples
```

### Comparing `ironic-python-agent-9.4.0/doc/source/contributor/hardware_managers.rst` & `ironic-python-agent-9.5.0/doc/source/contributor/hardware_managers.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/contributor/index.rst` & `ironic-python-agent-9.5.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/contributor/metrics.rst` & `ironic-python-agent-9.5.0/doc/source/contributor/metrics.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/contributor/rescue.rst` & `ironic-python-agent-9.5.0/doc/source/contributor/rescue.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/index.rst` & `ironic-python-agent-9.5.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/doc/source/install/index.rst` & `ironic-python-agent-9.5.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/examples/README.rst` & `ironic-python-agent-9.5.0/examples/README.rst`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/examples/business-logic/example_business_logic.py` & `ironic-python-agent-9.5.0/examples/business-logic/example_business_logic.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/examples/business-logic/setup.cfg` & `ironic-python-agent-9.5.0/examples/business-logic/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/examples/custom-disk-erase/example_disk_eraser.py` & `ironic-python-agent-9.5.0/examples/custom-disk-erase/example_disk_eraser.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/examples/custom-disk-erase/setup.cfg` & `ironic-python-agent-9.5.0/examples/custom-disk-erase/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/examples/vendor-device/example_device.py` & `ironic-python-agent-9.5.0/examples/vendor-device/example_device.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/examples/vendor-device/setup.cfg` & `ironic-python-agent-9.5.0/examples/vendor-device/setup.cfg`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/__init__.py` & `ironic-python-agent-9.5.0/ironic_python_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/agent.py` & `ironic-python-agent-9.5.0/ironic_python_agent/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,16 @@
         config = content.get('config', {})
         if config.get('metrics'):
             for opt, val in config.items():
                 setattr(cfg.CONF.metrics, opt, val)
         if config.get('metrics_statsd'):
             for opt, val in config.items():
                 setattr(cfg.CONF.metrics_statsd, opt, val)
+        if config.get('agent_md5_checksum_enable'):
+            cfg.set_override('md5_enabled', True)
         if config.get('agent_token_required'):
             self.agent_token_required = True
         token = config.get('agent_token')
         if token:
             if len(token) >= 32:
                 LOG.debug('Agent token recorded as designated by '
                           'the ironic installation.')
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/api/app.py` & `ironic-python-agent-9.5.0/ironic_python_agent/api/app.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/burnin.py` & `ironic-python-agent-9.5.0/ironic_python_agent/burnin.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/cmd/agent.py` & `ironic-python-agent-9.5.0/ironic_python_agent/cmd/agent.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/cmd/inspect.py` & `ironic-python-agent-9.5.0/ironic_python_agent/cmd/inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/config.py` & `ironic-python-agent-9.5.0/ironic_python_agent/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,17 @@
                       'kernel parameter.'),
 
     cfg.BoolOpt('collect_lldp',
                 default=APARAMS.get('ipa-collect-lldp', False),
                 help='Whether IPA should attempt to receive LLDP packets for '
                      'each network interface it discovers in the inventory. '
                      'Can be supplied as "ipa-collect-lldp" '
-                     'kernel parameter.'),
+                     'kernel parameter.',
+                deprecated_for_removal=True,
+                deprecated_reason="Use the lldp collector instead"),
 
     cfg.StrOpt('inspection_callback_url',
                default=APARAMS.get('ipa-inspection-callback-url'),
                help='Endpoint of ironic-inspector. If set, hardware inventory '
                     'will be collected and sent to ironic-inspector '
                     'on start up. '
                     'A special value "mdns" can be specified to fetch the '
@@ -322,14 +324,18 @@
                      'methods. If one of these filesystems is detected '
                      'during cleaning, the cleaning process will be aborted '
                      'and infrastructure operator intervention may be '
                      'required as this option is intended to prevent '
                      'cleaning from inadvertently destroying a running '
                      'cluster which may be visible over a storage fabric '
                      'such as FibreChannel.'),
+    cfg.BoolOpt('md5_enabled',
+                default=True,
+                help='If the MD5 algorithm is enabled for file checksums. '
+                     'Will be changed to False in the future.'),
 ]
 
 CONF.register_cli_opts(cli_opts)
 
 
 def list_opts():
     return [('DEFAULT', cli_opts)]
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/dmi_inspector.py` & `ironic-python-agent-9.5.0/ironic_python_agent/dmi_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/efi_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/efi_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         LOG.warning('No UUID information provided in sgdisk output for '
                     'partition %s on device %s', part_num, device)
 
 
 def manage_uefi(device, efi_system_part_uuid=None):
     """Manage the device looking for valid efi bootloaders to update the nvram.
 
-    This method checks for valid efi bootloaders in the device, if they exists
+    This method checks for valid efi bootloaders in the device, if they exist
     it updates the nvram using the efibootmgr.
 
     :param device: the device to be checked.
     :param efi_system_part_uuid: efi partition uuid.
     :raises: DeviceNotFound if the efi partition cannot be found.
     :return: True - if it founds any efi bootloader and the nvram was updated
              using the efibootmgr.
@@ -271,16 +271,23 @@
 
 
 def get_boot_records():
     """Executes efibootmgr and returns boot records.
 
     :return: an iterator yielding pairs (boot number, boot record).
     """
-    efi_output = utils.execute('efibootmgr', '-v')
-    for line in efi_output[0].split('\n'):
+    # Invokes binary=True so we get a bytestream back.
+    efi_output = utils.execute('efibootmgr', '-v', binary=True)
+    # Bytes must be decoded before regex can be run and
+    # matching to work as intended.
+    # Also ignore errors on decoding, as we can basically get
+    # garbage out of the nvram record, this way we don't fail
+    # hard on unrelated records.
+    cmd_output = efi_output[0].decode('utf-16', errors='ignore')
+    for line in cmd_output.split('\n'):
         match = _ENTRY_LABEL.match(line)
         if match is not None:
             yield (match[1], match[2])
 
 
 def add_boot_record(device, efi_partition, loader, label):
     """Add an EFI boot record with efibootmgr.
@@ -289,23 +296,23 @@
     :param efi_partition: the number of the EFI partition on the device
     :param loader: path to the EFI boot loader
     :param label: the record label
     """
     # https://linux.die.net/man/8/efibootmgr
     utils.execute('efibootmgr', '-v', '-c', '-d', device,
                   '-p', str(efi_partition), '-w', '-L', label,
-                  '-l', loader)
+                  '-l', loader, binary=True)
 
 
 def remove_boot_record(boot_num):
     """Remove an EFI boot record with efibootmgr.
 
     :param boot_num: the number of the boot record
     """
-    utils.execute('efibootmgr', '-b', boot_num, '-B')
+    utils.execute('efibootmgr', '-b', boot_num, '-B', binary=True)
 
 
 def _run_efibootmgr(valid_efi_bootloaders, device, efi_partition,
                     mount_point, label_suffix=None):
     """Executes efibootmgr and removes duplicate entries.
 
     :param valid_efi_bootloaders: the list of valid efi bootloaders
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/encoding.py` & `ironic-python-agent-9.5.0/ironic_python_agent/encoding.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/errors.py` & `ironic-python-agent-9.5.0/ironic_python_agent/errors.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/base.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/clean.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/clean.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/deploy.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/deploy.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/flow.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/flow.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/image.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/image.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/log.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/log.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/poll.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/poll.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/rescue.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/rescue.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/extensions/standby.py` & `ironic-python-agent-9.5.0/ironic_python_agent/extensions/standby.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import hashlib
 import os
+import re
 import tempfile
 import time
 from urllib import parse as urlparse
 
 from ironic_lib import disk_utils
 from ironic_lib import exception
 from oslo_concurrency import processutils
@@ -95,39 +96,81 @@
                             url, e)
                 time.sleep(CONF.image_download_connection_retry_interval)
         else:
             break
     return resp
 
 
+def _is_checksum_url(checksum):
+    """Identify if checksum is not a url"""
+    if (checksum.startswith('http://') or checksum.startswith('https://')):
+        return True
+    else:
+        return False
+
+
+MD5_MATCH = r"^([a-fA-F\d]{32})\s"  # MD5 at beginning of line
+MD5_MATCH_END = r"\s([a-fA-F\d]{32})$"  # MD5 at end of line
+MD5_MATCH_ONLY = r"^([a-fA-F\d]{32})$"  # MD5 only
+SHA256_MATCH = r"^([a-fA-F\d]{64})\s"  # SHA256 at beginning of line
+SHA256_MATCH_END = r"\s([a-fA-F\d]{64})$"  # SHA256 at end of line
+SHA256_MATCH_ONLY = r"^([a-fA-F\d]{64})$"  # SHA256 only
+SHA512_MATCH = r"^([a-fA-F\d]{128})\s"  # SHA512 at beginning of line
+SHA512_MATCH_END = r"\s([a-fA-F\d]{128})$"  # SHA512 at end of line
+SHA512_MATCH_ONLY = r"^([a-fA-F\d]{128})$"  # SHA512 only
+FILENAME_MATCH_END = r"\s[*]?{filename}$"  # Filename binary/text end of line
+FILENAME_MATCH_PARENTHESES = r"\s\({filename}\)\s"  # CentOS images
+
+CHECKSUM_MATCHERS = (MD5_MATCH, MD5_MATCH_END, SHA256_MATCH, SHA256_MATCH_END,
+                     SHA512_MATCH, SHA512_MATCH_END)
+CHECKSUM_ONLY_MATCHERS = (MD5_MATCH_ONLY, SHA256_MATCH_ONLY, SHA512_MATCH_ONLY)
+FILENAME_MATCHERS = (FILENAME_MATCH_END, FILENAME_MATCH_PARENTHESES)
+
+
 def _fetch_checksum(checksum, image_info):
     """Fetch checksum from remote location, if needed."""
-    if not (checksum.startswith('http://') or checksum.startswith('https://')):
+    if not _is_checksum_url(checksum):
         # Not a remote checksum, return as it is.
         return checksum
 
     LOG.debug('Downloading checksums file from %s', checksum)
     resp = _download_with_proxy(image_info, checksum, checksum).text
     lines = [line.strip() for line in resp.split('\n') if line.strip()]
     if not lines:
         raise errors.ImageDownloadError(checksum, "Empty checksum file")
     elif len(lines) == 1:
         # Special case - checksums file with only the checksum itself
         if ' ' not in lines[0]:
-            return lines[0]
+            for matcher in CHECKSUM_ONLY_MATCHERS:
+                checksum = re.findall(matcher, lines[0])
+                if checksum:
+                    return checksum[0]
+            raise errors.ImageDownloadError(
+                checksum, ("Invalid checksum file (No valid checksum found) %s"
+                           % lines))
 
     # FIXME(dtantsur): can we assume the same name for all images?
     expected_fname = os.path.basename(urlparse.urlparse(
         image_info['urls'][0]).path)
     for line in lines:
-        checksum, fname = line.strip().split(None, 1)
-        # The star symbol designates binary mode, which is the same as text
-        # mode on GNU systems.
-        if fname.strip().lstrip('*') == expected_fname:
-            return checksum.strip()
+        # Ignore comment lines
+        if line.startswith("#"):
+            continue
+
+        # Ignore checksums for other files
+        for matcher in FILENAME_MATCHERS:
+            if re.findall(matcher.format(filename=expected_fname), line):
+                break
+        else:
+            continue
+
+        for matcher in CHECKSUM_MATCHERS:
+            checksum = re.findall(matcher, line)
+            if checksum:
+                return checksum[0]
 
     raise errors.ImageDownloadError(
         checksum, "Checksum file does not contain name %s" % expected_fname)
 
 
 def _write_partition_image(image, image_info, device, configdrive=None):
     """Call disk_util to create partition and write the partition image.
@@ -259,14 +302,55 @@
     else:
         result_msg = msg + 'root_uuid={}'
         message = result_msg.format(image_info['id'], device, root_uuid)
 
     return message
 
 
+def _get_algorithm_by_length(checksum):
+    """Determine the SHA-2 algorithm by checksum length.
+
+    :param checksum: The requested checksum.
+    :returns: A hashlib object based upon the checksum
+              or ValueError if the algorthm could not be
+              identified.
+    """
+    # NOTE(TheJulia): This is all based on SHA-2 lengths.
+    # SHA-3 would require a hint, thus ValueError because
+    # it may not be a fixed length. That said, SHA-2 is not
+    # as of this not being added, being withdrawn standards wise.
+    checksum_len = len(checksum)
+    if checksum_len == 128:
+        # Sha512 is 512 bits, or 128 characters
+        return hashlib.new('sha512')
+    elif checksum_len == 64:
+        # SHA256 is 256 bits, or 64 characters
+        return hashlib.new('sha256')
+    elif checksum_len == 32:
+        check_md5_enabled()
+        # This is not super great, but opt-in only.
+        return hashlib.new('md5')  # nosec
+    else:
+        # Previously, we would have just assumed the value was
+        # md5 by default. This way we are a little smarter and
+        # gracefully handle things better when md5 is explicitly
+        # disabled.
+        raise ValueError('Unable to identify checksum algorithm '
+                         'used, and a value is not specified in '
+                         'the os_hash_algo setting.')
+
+
+def check_md5_enabled():
+    """Checks if md5 is permitted, otherwise raises ValueError."""
+    if not CONF.md5_enabled:
+        raise ValueError('MD5 support is disabled, and support '
+                         'will be removed in a 2024 version of '
+                         'Ironic.')
+
+
 class ImageDownload(object):
     """Helper class that opens a HTTP connection to download an image.
 
     This class opens a HTTP connection to download an image from a URL
     and create an iterator so the image can be downloaded in chunks. The
     MD5 hash of the image being downloaded is calculated on-the-fly.
     """
@@ -288,46 +372,71 @@
 
         :raises: ImageDownloadError if starting the image download fails for
                  any reason.
         """
         self._time = time_obj or time.time()
         self._image_info = image_info
         self._request = None
+        checksum = image_info.get('checksum')
+        retrieved_checksum = False
 
         # Determine the hash algorithm and value will be used for calculation
         # and verification, fallback to md5 if algorithm is not set or not
         # supported.
         algo = image_info.get('os_hash_algo')
         if algo and algo in hashlib.algorithms_available:
             self._hash_algo = hashlib.new(algo)
             self._expected_hash_value = image_info.get('os_hash_value')
-        elif image_info.get('checksum'):
+        elif checksum and _is_checksum_url(checksum):
+            # Treat checksum urls as first class request citizens, else
+            # fallback to legacy handling.
+            self._expected_hash_value = _fetch_checksum(
+                checksum,
+                image_info)
+            retrieved_checksum = True
+            if not algo:
+                # Override algorithm not suppied as os_hash_algo
+                self._hash_algo = _get_algorithm_by_length(
+                    self._expected_hash_value)
+        elif checksum:
+            # Fallback to md5 path.
             try:
-                self._hash_algo = hashlib.md5()
+                new_algo = _get_algorithm_by_length(checksum)
+
+                if not new_algo:
+                    # Realistically, this should never happen, but for
+                    # compatability...
+                    # TODO(TheJulia): Remove for a 2024 release.
+                    self._hash_algo = hashlib.new('md5')
+                else:
+                    self._hash_algo = new_algo
             except ValueError as e:
-                message = ('Unable to proceed with image {} as the legacy '
-                           'checksum indicator has been used, which makes use '
-                           'the MD5 algorithm. This algorithm failed to load '
-                           'due to the underlying operating system. Error: '
+                message = ('Unable to proceed with image {} as the '
+                           'checksum indicator has been used but the '
+                           'algorithm could not be identified. Error: '
                            '{}').format(image_info['id'], str(e))
                 LOG.error(message)
                 raise errors.RESTError(details=message)
-            self._expected_hash_value = image_info['checksum']
+            self._expected_hash_value = checksum
         else:
             message = ('Unable to verify image {} with available checksums. '
                        'Please make sure the specified \'os_hash_algo\' '
                        '(currently {}) is supported by this ramdisk, or '
                        'provide a md5 checksum via the \'checksum\' '
                        'field'.format(image_info['id'],
                                       image_info.get('os_hash_algo')))
             LOG.error(message)
             raise errors.RESTError(details=message)
 
-        self._expected_hash_value = _fetch_checksum(self._expected_hash_value,
-                                                    image_info)
+        if not retrieved_checksum:
+            # Fallback to retrieve the checksum if we didn't retrieve it
+            # earlier on.
+            self._expected_hash_value = _fetch_checksum(
+                self._expected_hash_value,
+                image_info)
 
         details = []
         for url in image_info['urls']:
             try:
                 LOG.info("Attempting to download image from %s", url)
                 self._request = _download_with_proxy(image_info, url,
                                                      image_info['id'])
@@ -359,15 +468,18 @@
             # While this seems weird and doesn't exactly seem to match the
             # patterns in requests and urllib3, it does appear to be the
             # case. Field testing in environments where TCP sockets were
             # discovered in a read hanged state were navigated with
             # this code.
             if chunk:
                 self._last_chunk_time = time.time()
-                self._hash_algo.update(chunk)
+                if isinstance(chunk, str):
+                    self._hash_algo.update(chunk.encode())
+                else:
+                    self._hash_algo.update(chunk)
                 yield chunk
             elif (time.time() - self._last_chunk_time
                   > CONF.image_download_connection_timeout):
                 LOG.error('Timeout reached waiting for a chunk of data from '
                           'a remote server.')
                 raise errors.ImageDownloadError(
                     self._image_info['id'],
@@ -454,14 +566,15 @@
                    compatibility with async_command validation.
     :raises: InvalidCommandParamsError if the data contained in image_info
              does not match type and key:value pair requirements and
              expectations.
     """
     image_info = image_info or {}
 
+    checksum_avail = False
     md5sum_avail = False
     os_hash_checksum_avail = False
 
     for field in ['id', 'urls']:
         if field not in image_info:
             msg = 'Image is missing \'{}\' field.'.format(field)
             raise errors.InvalidCommandParamsError(msg)
@@ -472,30 +585,36 @@
 
     checksum = image_info.get('checksum')
     if checksum is not None:
         if (not isinstance(image_info['checksum'], str)
                 or not image_info['checksum']):
             raise errors.InvalidCommandParamsError(
                 'Image \'checksum\' must be a non-empty string.')
-        md5sum_avail = True
+        if _is_checksum_url(checksum) or len(checksum) > 32:
+            # Checksum is a URL *or* a greater than 32 characters,
+            # putting it into the realm of sha256 or sha512 and not
+            # the MD5 algorithm.
+            checksum_avail = True
+        elif CONF.md5_enabled:
+            md5sum_avail = True
 
     os_hash_algo = image_info.get('os_hash_algo')
     os_hash_value = image_info.get('os_hash_value')
     if os_hash_algo or os_hash_value:
         if (not isinstance(os_hash_algo, str)
                 or not os_hash_algo):
             raise errors.InvalidCommandParamsError(
                 'Image \'os_hash_algo\' must be a non-empty string.')
         if (not isinstance(os_hash_value, str)
                 or not os_hash_value):
             raise errors.InvalidCommandParamsError(
                 'Image \'os_hash_value\' must be a non-empty string.')
         os_hash_checksum_avail = True
 
-    if not (md5sum_avail or os_hash_checksum_avail):
+    if not (checksum_avail or md5sum_avail or os_hash_checksum_avail):
         raise errors.InvalidCommandParamsError(
             'Image checksum is not available, either the \'checksum\' field '
             'or the \'os_hash_algo\' and \'os_hash_value\' fields pair must '
             'be set for image verification.')
 
 
 def _validate_partitioning(device):
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/hardware.py` & `ironic-python-agent-9.5.0/ironic_python_agent/hardware.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 import binascii
 import collections
+import contextlib
 import functools
 import io
 import ipaddress
 import json
 from multiprocessing.pool import ThreadPool
 import os
 import re
@@ -54,14 +55,17 @@
 CONF = cfg.CONF
 
 WARN_BIOSDEVNAME_NOT_FOUND = False
 
 UNIT_CONVERTER = pint.UnitRegistry(filename=None)
 UNIT_CONVERTER.define('bytes = []')
 UNIT_CONVERTER.define('MB = 1048576 bytes')
+UNIT_CONVERTER.define('bit_s = []')
+UNIT_CONVERTER.define('Mbit_s = 1000000 * bit_s')
+UNIT_CONVERTER.define('Gbit_s = 1000 * Mbit_s')
 _MEMORY_ID_RE = re.compile(r'^memory(:\d+)?$')
 NODE = None
 API_CLIENT = None
 API_LOOKUP_TIMEOUT = None
 API_LOOKUP_INTERVAL = None
 SUPPORTED_SOFTWARE_RAID_LEVELS = frozenset(['0', '1', '1+0', '5', '6'])
 NVME_CLI_FORMAT_SUPPORTED_FLAG = 0b10
@@ -89,36 +93,19 @@
     """Get the device info according to device class and field."""
     try:
         devname = os.path.basename(dev)
         with open('/sys/class/%s/%s/device/%s' % (devclass, devname, field),
                   'r') as f:
             return f.read().strip()
     except IOError:
-        LOG.warning("Can't find field %(field)s for"
+        LOG.warning("Can't find field %(field)s for "
                     "device %(dev)s in device class %(class)s",
                     {'field': field, 'dev': dev, 'class': devclass})
 
 
-def _get_system_lshw_dict():
-    """Get a dict representation of the system from lshw
-
-    Retrieves a json representation of the system from lshw and converts
-    it to a python dict
-
-    :return: A python dict from the lshw json output
-    """
-    out, _e = il_utils.execute('lshw', '-quiet', '-json', log_stdout=False)
-    out = json.loads(out)
-    # Depending on lshw version, output might be a list, starting with
-    # https://github.com/lyonel/lshw/commit/135a853c60582b14c5b67e5cd988a8062d9896f4  # noqa
-    if isinstance(out, list):
-        return out[0]
-    return out
-
-
 def _udev_settle():
     """Wait for the udev event queue to settle.
 
     Wait for the udev event queue to settle to make sure all devices
     are detected once the machine boots up.
 
     """
@@ -335,30 +322,24 @@
     LOG.info('Found component devices for %s: %s',
              raid_device, component_devices)
     return component_devices
 
 
 def _calc_memory(sys_dict):
     physical = 0
-    for sys_child in sys_dict['children']:
-        if sys_child['id'] != 'core':
-            continue
-        for core_child in sys_child['children']:
-            if not _MEMORY_ID_RE.match(core_child['id']):
-                continue
-            if core_child.get('size'):
-                value = ("%(size)s %(units)s" % core_child)
-                physical += int(UNIT_CONVERTER(value).to
-                                ('MB').magnitude)
-            else:
-                for bank in core_child.get('children', ()):
-                    if bank.get('size'):
-                        value = ("%(size)s %(units)s" % bank)
-                        physical += int(UNIT_CONVERTER(value).to
-                                        ('MB').magnitude)
+    core_dict = next(utils.find_in_lshw(sys_dict, 'core'), {})
+    for core_child in utils.find_in_lshw(core_dict, _MEMORY_ID_RE):
+        if core_child.get('size'):
+            value = ("%(size)s %(units)s" % core_child)
+            physical += int(UNIT_CONVERTER(value).to('MB').magnitude)
+        else:
+            for bank in core_child.get('children', ()):
+                if bank.get('size'):
+                    value = ("%(size)s %(units)s" % bank)
+                    physical += int(UNIT_CONVERTER(value).to('MB').magnitude)
     return physical
 
 
 def get_holder_disks(raid_device):
     """Get the holder disks of a Software RAID device.
 
     Examine an md device and return its underlying disks.
@@ -789,28 +770,29 @@
         self.partuuid = partuuid
 
 
 class NetworkInterface(encoding.SerializableComparable):
     serializable_fields = ('name', 'mac_address', 'ipv4_address',
                            'ipv6_address', 'has_carrier', 'lldp',
                            'vendor', 'product', 'client_id',
-                           'biosdevname')
+                           'biosdevname', 'speed_mbps')
 
     def __init__(self, name, mac_addr, ipv4_address=None, ipv6_address=None,
                  has_carrier=True, lldp=None, vendor=None, product=None,
-                 client_id=None, biosdevname=None):
+                 client_id=None, biosdevname=None, speed_mbps=None):
         self.name = name
         self.mac_address = mac_addr
         self.ipv4_address = ipv4_address
         self.ipv6_address = ipv6_address
         self.has_carrier = has_carrier
         self.lldp = lldp
         self.vendor = vendor
         self.product = product
         self.biosdevname = biosdevname
+        self.speed_mbps = speed_mbps
         # client_id is used for InfiniBand only. we calculate the DHCP
         # client identifier Option to allow DHCP to work over InfiniBand.
         # see https://tools.ietf.org/html/rfc4390
         self.client_id = client_id
 
 
 class CPU(encoding.SerializableComparable):
@@ -831,21 +813,32 @@
     # physical = total + kernel binary + reserved space
 
     def __init__(self, total, physical_mb=None):
         self.total = total
         self.physical_mb = physical_mb
 
 
+class SystemFirmware(encoding.SerializableComparable):
+    serializable_fields = ('vendor', 'version', 'build_date')
+
+    def __init__(self, vendor, version, build_date):
+        self.version = version
+        self.build_date = build_date
+        self.vendor = vendor
+
+
 class SystemVendorInfo(encoding.SerializableComparable):
-    serializable_fields = ('product_name', 'serial_number', 'manufacturer')
+    serializable_fields = ('product_name', 'serial_number', 'manufacturer',
+                           'firmware')
 
-    def __init__(self, product_name, serial_number, manufacturer):
+    def __init__(self, product_name, serial_number, manufacturer, firmware):
         self.product_name = product_name
         self.serial_number = serial_number
         self.manufacturer = manufacturer
+        self.firmware = firmware
 
 
 class BootInfo(encoding.SerializableComparable):
     serializable_fields = ('current_boot_mode', 'pxe_interface')
 
     def __init__(self, current_boot_mode, pxe_interface=None):
         self.current_boot_mode = current_boot_mode
@@ -856,14 +849,17 @@
     @abc.abstractmethod
     def evaluate_hardware_support(self):
         pass
 
     def list_network_interfaces(self):
         raise errors.IncompatibleHardwareMethodError
 
+    def collect_lldp_data(self, interface_names=None):
+        raise errors.IncompatibleHardwareMethodError
+
     def get_cpus(self):
         raise errors.IncompatibleHardwareMethodError
 
     def list_block_devices(self, include_partitions=False):
         """List physical block devices
 
         :param include_partitions: If to include partitions
@@ -1189,39 +1185,82 @@
 
 class GenericHardwareManager(HardwareManager):
     HARDWARE_MANAGER_NAME = 'generic_hardware_manager'
     # 1.1 - Added new clean step called erase_devices_metadata
     HARDWARE_MANAGER_VERSION = '1.1'
 
     def __init__(self):
-        self.sys_path = '/sys'
         self.lldp_data = {}
+        self._lshw_cache = None
 
     def evaluate_hardware_support(self):
         # Do some initialization before we declare ourself ready
         _check_for_iscsi()
         _md_scan_and_assemble()
         _load_ipmi_modules()
         global MULTIPATH_ENABLED
         if MULTIPATH_ENABLED is None:
             MULTIPATH_ENABLED = _enable_multipath()
 
         self.wait_for_disks()
         return HardwareSupport.GENERIC
 
-    def collect_lldp_data(self, interface_names):
+    def list_hardware_info(self):
+        """Return full hardware inventory as a serializable dict.
+
+        This inventory is sent to Ironic on lookup and to Inspector on
+        inspection.
+
+        :return: a dictionary representing inventory
+        """
+        with self._cached_lshw():
+            return super().list_hardware_info()
+
+    @contextlib.contextmanager
+    def _cached_lshw(self):
+        if self._lshw_cache:
+            yield  # make this context manager reentrant without purging cache
+            return
+
+        self._lshw_cache = self._get_system_lshw_dict()
+        try:
+            yield
+        finally:
+            self._lshw_cache = None
+
+    def _get_system_lshw_dict(self):
+        """Get a dict representation of the system from lshw
+
+        Retrieves a json representation of the system from lshw and converts
+        it to a python dict
+
+        :return: A python dict from the lshw json output
+        """
+        if self._lshw_cache:
+            return self._lshw_cache
+
+        out, _e = il_utils.execute('lshw', '-quiet', '-json', log_stdout=False)
+        out = json.loads(out)
+        # Depending on lshw version, output might be a list, starting with
+        # https://github.com/lyonel/lshw/commit/135a853c60582b14c5b67e5cd988a8062d9896f4  # noqa
+        if isinstance(out, list):
+            return out[0]
+        return out
+
+    def collect_lldp_data(self, interface_names=None):
         """Collect and convert LLDP info from the node.
 
         In order to process the LLDP information later, the raw data needs to
         be converted for serialization purposes.
 
         :param interface_names: list of names of node's interfaces.
         :return: a dict, containing the lldp data from every interface.
         """
-
+        if interface_names is None:
+            interface_names = netutils.list_interfaces()
         interface_names = [name for name in interface_names if name != 'lo']
         lldp_data = {}
         try:
             raw_lldp_data = netutils.get_lldp_info(interface_names)
         except Exception:
             # NOTE(sambetts) The get_lldp_info function will log this exception
             # and we don't invalidate any existing data in the cache if we fail
@@ -1242,28 +1281,52 @@
             lldp_data[ifname] = processed_tlvs
         return lldp_data
 
     def _get_lldp_data(self, interface_name):
         if self.lldp_data:
             return self.lldp_data.get(interface_name)
 
-    def get_interface_info(self, interface_name):
+    def _get_network_speed(self, interface_name):
+        sys_dict = self._get_system_lshw_dict()
+        try:
+            iface_dict = next(
+                utils.find_in_lshw(sys_dict, by_class='network',
+                                   logicalname=interface_name,
+                                   recursive=True)
+            )
+        except StopIteration:
+            LOG.warning('Cannot find detailed information about interface %s',
+                        interface_name)
+            return None
+
+        # speed is the current speed, capacity is the maximum speed
+        speed = iface_dict.get('capacity') or iface_dict.get('speed')
+        if not speed:
+            LOG.debug('No speed information about in %s', iface_dict)
+            return None
 
+        units = iface_dict.get('units', 'bit_s').replace('/', '_')
+        return int(UNIT_CONVERTER(f'{speed} {units}')
+                   .to(UNIT_CONVERTER.Mbit_s)
+                   .magnitude)
+
+    def get_interface_info(self, interface_name):
         mac_addr = netutils.get_mac_addr(interface_name)
         if mac_addr is None:
             raise errors.IncompatibleHardwareMethodError()
 
         return NetworkInterface(
             interface_name, mac_addr,
             ipv4_address=self.get_ipv4_addr(interface_name),
             ipv6_address=self.get_ipv6_addr(interface_name),
             has_carrier=netutils.interface_has_carrier(interface_name),
             vendor=_get_device_info(interface_name, 'net', 'vendor'),
             product=_get_device_info(interface_name, 'net', 'device'),
-            biosdevname=self.get_bios_given_nic_name(interface_name))
+            biosdevname=self.get_bios_given_nic_name(interface_name),
+            speed_mbps=self._get_network_speed(interface_name))
 
     def get_ipv4_addr(self, interface_id):
         return netutils.get_ipv4_addr(interface_id)
 
     def get_ipv6_addr(self, interface_id):
         """Get the default IPv6 address assigned to the interface.
 
@@ -1283,15 +1346,15 @@
 
         :param interface_name: list of names of node's interfaces.
         :return: the BIOS given NIC name of node's interfaces or default
                  as None.
         """
         global WARN_BIOSDEVNAME_NOT_FOUND
 
-        if self._is_vlan(interface_name):
+        if netutils.is_vlan(interface_name):
             LOG.debug('Interface %s is a VLAN, biosdevname not called',
                       interface_name)
             return
 
         try:
             stdout, _ = il_utils.execute('biosdevname', '-i', interface_name)
             return stdout.rstrip('\n')
@@ -1304,64 +1367,44 @@
             # virtual machine.
             if e.exit_code == 4:
                 LOG.info('The system is a virtual machine, so biosdevname '
                          'utility does not provide names for virtual NICs.')
             else:
                 LOG.warning('Biosdevname returned exit code %s', e.exit_code)
 
-    def _is_device(self, interface_name):
-        device_path = '{}/class/net/{}/device'.format(self.sys_path,
-                                                      interface_name)
-        return os.path.exists(device_path)
-
-    def _is_vlan(self, interface_name):
-        # A VLAN interface does not have /device, check naming convention
-        # used when adding VLAN interface
-
-        interface, sep, vlan = interface_name.partition('.')
-
-        return vlan.isdigit()
-
-    def _is_bond(self, interface_name):
-        device_path = '{}/class/net/{}/bonding'.format(self.sys_path,
-                                                       interface_name)
-        return os.path.exists(device_path)
-
     def list_network_interfaces(self):
-        network_interfaces_list = []
-        iface_names = os.listdir('{}/class/net'.format(self.sys_path))
-        iface_names = [name for name in iface_names
-                       if self._is_vlan(name) or self._is_device(name)
-                       or self._is_bond(name)]
+        iface_names = netutils.list_interfaces()
 
         if CONF.collect_lldp:
             self.lldp_data = dispatch_to_managers('collect_lldp_data',
                                                   interface_names=iface_names)
 
-        for iface_name in iface_names:
-            try:
-                result = dispatch_to_managers(
-                    'get_interface_info', interface_name=iface_name)
-            except errors.HardwareManagerMethodNotFound:
-                LOG.warning('No hardware manager was able to handle '
-                            'interface %s', iface_name)
-                continue
-            result.lldp = self._get_lldp_data(iface_name)
-            network_interfaces_list.append(result)
-
-        # If configured, bring up vlan interfaces. If the actual vlans aren't
-        # defined they are derived from LLDP data
-        if CONF.enable_vlan_interfaces:
-            vlan_iface_names = netutils.bring_up_vlan_interfaces(
-                network_interfaces_list)
-            for vlan_iface_name in vlan_iface_names:
-                result = dispatch_to_managers(
-                    'get_interface_info', interface_name=vlan_iface_name)
+        network_interfaces_list = []
+        with self._cached_lshw():
+            for iface_name in iface_names:
+                try:
+                    result = dispatch_to_managers(
+                        'get_interface_info', interface_name=iface_name)
+                except errors.HardwareManagerMethodNotFound:
+                    LOG.warning('No hardware manager was able to handle '
+                                'interface %s', iface_name)
+                    continue
+                result.lldp = self._get_lldp_data(iface_name)
                 network_interfaces_list.append(result)
 
+            # If configured, bring up vlan interfaces. If the actual vlans
+            # aren't defined they are derived from LLDP data
+            if CONF.enable_vlan_interfaces:
+                vlan_iface_names = netutils.bring_up_vlan_interfaces(
+                    network_interfaces_list)
+                for vlan_iface_name in vlan_iface_names:
+                    result = dispatch_to_managers(
+                        'get_interface_info', interface_name=vlan_iface_name)
+                    network_interfaces_list.append(result)
+
         return network_interfaces_list
 
     def get_cpus(self):
         lines = il_utils.execute('lscpu')[0]
         cpu_info = {k.strip().lower(): v.strip() for k, v in
                     (line.split(':', 1)
                      for line in lines.split('\n')
@@ -1397,15 +1440,15 @@
             # This is explicitly catching all exceptions. We want to catch any
             # situation where a newly upgraded psutil would fail, and instead
             # print an error instead of blowing up the stack on IPA.
             total = None
             LOG.exception(("Cannot fetch total memory size using psutil "
                            "version %s"), psutil.version_info[0])
         try:
-            sys_dict = _get_system_lshw_dict()
+            sys_dict = self._get_system_lshw_dict()
         except (processutils.ProcessExecutionError, OSError, ValueError) as e:
             LOG.warning('Could not get real physical RAM from lshw: %s', e)
             physical = None
         else:
             physical = _calc_memory(sys_dict)
 
             if not physical:
@@ -1504,21 +1547,29 @@
                  'root device hints %(hints)s',
                  {'dev': dev_name, 'hints': root_device_hints,
                   'node': cached_node['uuid'] if cached_node else None})
         return dev_name
 
     def get_system_vendor_info(self):
         try:
-            sys_dict = _get_system_lshw_dict()
+            sys_dict = self._get_system_lshw_dict()
         except (processutils.ProcessExecutionError, OSError, ValueError) as e:
             LOG.warning('Could not retrieve vendor info from lshw: %s', e)
             sys_dict = {}
+
+        core_dict = next(utils.find_in_lshw(sys_dict, 'core'), {})
+        fw_dict = next(utils.find_in_lshw(core_dict, 'firmware'), {})
+
+        firmware = SystemFirmware(vendor=fw_dict.get('vendor', ''),
+                                  version=fw_dict.get('version', ''),
+                                  build_date=fw_dict.get('date', ''))
         return SystemVendorInfo(product_name=sys_dict.get('product', ''),
                                 serial_number=sys_dict.get('serial', ''),
-                                manufacturer=sys_dict.get('vendor', ''))
+                                manufacturer=sys_dict.get('vendor', ''),
+                                firmware=firmware)
 
     def get_boot_info(self):
         boot_mode = 'uefi' if os.path.isdir('/sys/firmware/efi') else 'bios'
         LOG.debug('The current boot mode is %s', boot_mode)
         pxe_interface = utils.get_agent_params().get('BOOTIF')
         return BootInfo(current_boot_mode=boot_mode,
                         pxe_interface=pxe_interface)
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/cna.py` & `ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/cna.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/mlnx.py` & `ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/mlnx.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py` & `ironic-python-agent-9.5.0/ironic_python_agent/hardware_managers/nvidia/nvidia_fw_update.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/inject_files.py` & `ironic-python-agent-9.5.0/ironic_python_agent/inject_files.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/inspect.py` & `ironic-python-agent-9.5.0/ironic_python_agent/inspect.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/inspector.py` & `ironic-python-agent-9.5.0/ironic_python_agent/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,7 +360,16 @@
             'and revision %s', vendor, device, pci_class, pci_revision)
         pci_devices_info.append({'vendor_id': vendor,
                                  'product_id': device,
                                  'class': pci_class,
                                  'revision': pci_revision,
                                  'bus': subdir})
     data['pci_devices'] = pci_devices_info
+
+
+def collect_lldp(data, failures):
+    """Collect LLDP information for network interfaces.
+
+    :param data: mutable data that we'll send to inspector
+    :param failures: AccumulatedFailures object
+    """
+    data['lldp_raw'] = hardware.dispatch_to_managers('collect_lldp_data')
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/ironic_api_client.py` & `ironic-python-agent-9.5.0/ironic_python_agent/ironic_api_client.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/netutils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/netutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import ctypes
 import fcntl
+import os
 import select
 import socket
 import struct
 import sys
 
 import netifaces
 from oslo_config import cfg
@@ -243,14 +244,37 @@
 # Other options...
 # 1. import os; os.uname()[1]
 # 2. import platform; platform.node()
 def get_hostname():
     return socket.gethostname()
 
 
+def is_network_device(interface_name):
+    device_path = f'/sys/class/net/{interface_name}/device'
+    return os.path.exists(device_path)
+
+
+def is_vlan(interface_name):
+    # A VLAN interface does not have /device, check naming convention
+    # used when adding VLAN interface
+    interface, sep, vlan = interface_name.partition('.')
+    return vlan.isdigit()
+
+
+def is_bond(interface_name):
+    device_path = f'/sys/class/net/{interface_name}/bonding'
+    return os.path.exists(device_path)
+
+
+def list_interfaces():
+    iface_names = os.listdir('/sys/class/net')
+    return [name for name in iface_names
+            if is_vlan(name) or is_network_device(name) or is_bond(name)]
+
+
 def interface_has_carrier(interface_name):
     path = '/sys/class/net/{}/carrier'.format(interface_name)
     try:
         with open(path, 'rt') as fp:
             return fp.read().strip() == '1'
     except EnvironmentError:
         LOG.debug('No carrier information for interface %s',
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/numa_inspector.py` & `ironic-python-agent-9.5.0/ironic_python_agent/numa_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/partition_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/partition_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/raid_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/raid_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/functional/base.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/functional/test_commands.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/functional/test_commands.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/base.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/dmi_inspector_data.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/dmi_inspector_data.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_base.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_clean.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_clean.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_deploy.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_deploy.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_flow.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_flow.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_image.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 from ironic_python_agent import hardware
 from ironic_python_agent import partition_utils
 from ironic_python_agent import raid_utils
 from ironic_python_agent.tests.unit import base
 from ironic_python_agent.tests.unit.samples import hardware_samples as hws
 
 
+EFI_RESULT = ''.encode('utf-16')
+
+
 @mock.patch.object(hardware, 'dispatch_to_managers', autospec=True)
 @mock.patch.object(ilib_utils, 'execute', autospec=True)
 @mock.patch.object(tempfile, 'mkdtemp', lambda *_: '/tmp/fake-dir')
 @mock.patch.object(shutil, 'rmtree', lambda *_: None)
 class TestImageExtension(base.IronicAgentTest):
 
     def setUp(self):
@@ -227,28 +230,28 @@
         ]
         mock_get_partition.return_value = self.fake_efi_system_part
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI']
         mock_utils_efi_part.return_value = None
 
         mock_execute.side_effect = iter([('', ''), ('', ''),
                                          ('', ''), ('', ''),
-                                         ('', ''), ('', ''),
+                                         (EFI_RESULT, ''), (EFI_RESULT, ''),
                                          ('', ''), ('', '')])
 
         expected = [mock.call('efibootmgr', '--version'),
                     mock.call('partx', '-av', '/dev/fake', attempts=3,
                               delay_on_retry=True),
                     mock.call('udevadm', 'settle'),
                     mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         self.agent_extension.install_bootloader(
             root_uuid=self.fake_root_uuid,
             efi_system_part_uuid=self.fake_efi_system_part_uuid).join()
@@ -275,28 +278,28 @@
             self.fake_dev, hardware.BootInfo(current_boot_mode='uefi')
         ]
         mock_get_part_path.return_value = self.fake_efi_system_part
         mock_utils_efi_part.return_value = {'number': '1'}
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI']
         mock_execute.side_effect = iter([('', ''), ('', ''),
                                          ('', ''), ('', ''),
-                                         ('', ''), ('', ''),
+                                         (EFI_RESULT, ''), (EFI_RESULT, ''),
                                          ('', ''), ('', '')])
 
         expected = [mock.call('efibootmgr', '--version'),
                     mock.call('partx', '-av', '/dev/fake', attempts=3,
                               delay_on_retry=True),
                     mock.call('udevadm', 'settle'),
                     mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         self.agent_extension.install_bootloader(
             root_uuid=self.fake_root_uuid,
             efi_system_part_uuid=None).join()
@@ -329,32 +332,33 @@
 BootCurrent: 0001
 Timeout: 0 seconds
 BootOrder: 0000,00001
 Boot0000 ironic1 HD(1,GPT,4f3c6294-bf9b-4208-9808-be45dfc34b5c)File(\EFI\Boot\BOOTX64.EFI)
 Boot0001 ironic2 HD(1,GPT,4f3c6294-bf9b-4208-9808-111111111112)File(\EFI\Boot\BOOTX64.EFI)
 Boot0002 VENDMAGIC FvFile(9f3c6294-bf9b-4208-9808-be45dfc34b51)
 """  # noqa This is a giant literal string for testing.
+        stdout_msg = stdout_msg.encode('utf-16')
         mock_execute.side_effect = iter([('', ''), ('', ''),
                                          ('', ''), ('', ''),
-                                         (stdout_msg, ''), ('', ''),
-                                         ('', ''), ('', ''),
+                                         (stdout_msg, ''), (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''), (EFI_RESULT, ''),
                                          ('', ''), ('', '')])
 
         expected = [mock.call('efibootmgr', '--version'),
                     mock.call('partx', '-av', '/dev/fake', attempts=3,
                               delay_on_retry=True),
                     mock.call('udevadm', 'settle'),
                     mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
-                    mock.call('efibootmgr', '-b', '0000', '-B'),
+                    mock.call('efibootmgr', '-v', binary=True),
+                    mock.call('efibootmgr', '-b', '0000', '-B', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         self.agent_extension.install_bootloader(
             root_uuid=self.fake_root_uuid,
             efi_system_part_uuid=None).join()
@@ -392,32 +396,33 @@
 BootOrder: 0000,0003,0002,0001
 Boot0000* ironic1       HD(1,GPT,55db8d03-c8f6-4a5b-9155-790dddc348fa,0x800,0x64000)/File(\EFI\boot\shimx64.efi)
 Boot0001* CD/DVD Rom    VenHw(1fad3248-0000-7950-2166-a1e506fdb83a,02000000)..GO
 Boot0002* Hard Disk     VenHw(1fad3248-0000-7950-2166-a1e506fdb83a,01000000)..GO..NO..........V.U.E.F.I.:. . . .S.C.S.I. .H.a.r.d. .D.r.i.v.e........A....................................*..............@.........U..[J.Uy...H.......BO
 Boot0003* Network       VenHw(1fad3248-0000-7950-2166-a1e506fdb83a,05000000)..GO..NO............U.E.F.I.:. . . .S.L.O.T.2. .(.2.F./.0./.0.). .P.X.E. .I.P.4. . .Q.L.o.g.i.c. .Q.L.4.1.2.6.2. .P.C.I.e. .2.5.G.b. .2.-.P.o.r.t. .S.F.P.2.8. .E.t.h.e.r.n.e.t. .A.d.a.p.t.e.r. .-. .P.X.E........A....................%.4..Z...............................................................Gd-.;.A..MQ..L.P.X.E. .I.P.4. .Q.L.o.g.i.c. .Q.L.4.1.2.6.2. .P.C.I.e. .2.5.G.b. .2.-.P.o.r.t. .S.F.P.2.8. .E.t.h.e.r.n.e.t. .A.d.a.p.t.e.r. .-. .P.X.E.......BO..NO............U.E.F.I.:. . . .S.L.O.T.1. .(.3.0./.0./.0.). .P.X.E. .I.P.4. . .Q.L.o.g.i.c. .Q.L.4.1.2.6.2. .P.C.I.e. .2.5.G.b. .2.-.P.o.r.t. .S.F.P.2.8. .E.t.h.e.r.n.e.t. .A.d.a.p.t.e.r. .-.
 Boot0004* ironic1      HD(1,GPT,55db8d03-c8f6-4a5b-9155-790dddc348fa,0x800,0x64000)/File(\EFI\boot\shimx64.efi)
 """  # noqa This is a giant literal string for testing.
+        stdout_msg = stdout_msg.encode('utf-16')
         mock_execute.side_effect = iter([('', ''), ('', ''),
                                          ('', ''), ('', ''),
                                          (stdout_msg, ''), ('', ''),
                                          ('', ''), ('', ''),
                                          ('', ''), ('', '')])
         expected = [mock.call('efibootmgr', '--version'),
                     mock.call('partx', '-av', '/dev/fake', attempts=3,
                               delay_on_retry=True),
                     mock.call('udevadm', 'settle'),
                     mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
-                    mock.call('efibootmgr', '-b', '0000', '-B'),
-                    mock.call('efibootmgr', '-b', '0004', '-B'),
+                    mock.call('efibootmgr', '-v', binary=True),
+                    mock.call('efibootmgr', '-b', '0000', '-B', binary=True),
+                    mock.call('efibootmgr', '-b', '0004', '-B', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         self.agent_extension.install_bootloader(
             root_uuid=self.fake_root_uuid,
             efi_system_part_uuid=None).join()
@@ -446,33 +451,33 @@
         mock_get_part_path.return_value = self.fake_efi_system_part
         mock_utils_efi_part.return_value = {'number': '1'}
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI',
                                     'WINDOWS/system32/winload.efi']
 
         mock_execute.side_effect = iter([('', ''), ('', ''),
                                          ('', ''), ('', ''),
-                                         ('', ''), ('', ''),
-                                         ('', ''), ('', ''),
+                                         (EFI_RESULT, ''), (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''), ('', ''),
                                          ('', '')])
 
         expected = [mock.call('efibootmgr', '--version'),
                     mock.call('partx', '-av', '/dev/fake', attempts=3,
                               delay_on_retry=True),
                     mock.call('udevadm', 'settle'),
                     mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic2', '-l',
-                              '\\WINDOWS\\system32\\winload.efi'),
+                              '\\WINDOWS\\system32\\winload.efi', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         self.agent_extension.install_bootloader(
             root_uuid=self.fake_root_uuid,
             efi_system_part_uuid=None).join()
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_log.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_log.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_poll.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_poll.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_rescue.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_rescue.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/extensions/test_standby.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/extensions/test_standby.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,50 +15,56 @@
 import os
 import tempfile
 import time
 from unittest import mock
 
 from ironic_lib import exception
 from oslo_concurrency import processutils
+from oslo_config import cfg
 import requests
 
 from ironic_python_agent import errors
 from ironic_python_agent.extensions import standby
 from ironic_python_agent import hardware
 from ironic_python_agent import partition_utils
 from ironic_python_agent.tests.unit import base
 from ironic_python_agent import utils
 
 
+CONF = cfg.CONF
+
+
 def _build_fake_image_info(url='http://example.org'):
     return {
         'id': 'fake_id',
         'node_uuid': '1be26c0b-03f2-4d2e-ae87-c02d7f33c123',
         'urls': [url],
-        'checksum': 'abc123',
         'image_type': 'whole-disk-image',
+        'os_hash_algo': 'sha256',
+        'os_hash_value': 'fake-checksum',
     }
 
 
 def _build_fake_partition_image_info():
     return {
         'id': 'fake_id',
         'urls': [
             'http://example.org',
         ],
         'node_uuid': 'node_uuid',
-        'checksum': 'abc123',
         'root_mb': '10',
         'swap_mb': '10',
         'ephemeral_mb': '10',
         'ephemeral_format': 'abc',
         'preserve_ephemeral': 'False',
         'image_type': 'partition',
         'disk_label': 'msdos',
-        'deploy_boot_mode': 'bios'}
+        'deploy_boot_mode': 'bios',
+        'os_hash_algo': 'sha256',
+        'os_hash_value': 'fake-checksum'}
 
 
 class TestStandbyExtension(base.IronicAgentTest):
     def setUp(self):
         super(TestStandbyExtension, self).setUp()
         self.agent_extension = standby.StandbyExtension()
         self.fake_cpu = hardware.CPU(model_name='fuzzypickles',
@@ -79,28 +85,61 @@
         image_info = _build_fake_image_info()
         image_info['os_hash_algo'] = 'md5'
         image_info['os_hash_value'] = 'fake-checksum'
         standby._validate_image_info(None, image_info)
 
     def test_validate_image_info_success_without_md5(self):
         image_info = _build_fake_image_info()
-        del image_info['checksum']
         image_info['os_hash_algo'] = 'sha512'
         image_info['os_hash_value'] = 'fake-checksum'
         standby._validate_image_info(None, image_info)
 
     def test_validate_image_info_success_ignore_none_md5(self):
         image_info = _build_fake_image_info()
         image_info['checksum'] = None
         image_info['os_hash_algo'] = 'sha512'
         image_info['os_hash_value'] = 'fake-checksum'
         standby._validate_image_info(None, image_info)
 
+    def test_validate_image_info_legacy_md5_checksum_enabled(self):
+        image_info = _build_fake_image_info()
+        CONF.set_override('md5_enabled', True)
+        image_info['checksum'] = 'fake-checksum'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        standby._validate_image_info(None, image_info)
+
+    def test_validate_image_info_url(self):
+        image_info = _build_fake_image_info()
+        image_info['checksum'] = 'https://fake.url'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        standby._validate_image_info(None, image_info)
+
+    def test_validate_image_info_sha256(self):
+        image_info = _build_fake_image_info()
+        image_info['checksum'] = 'a' * 64
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        standby._validate_image_info(None, image_info)
+
+    def test_validate_image_info_legacy_md5_checksum(self):
+        CONF.set_override('md5_enabled', False)
+        image_info = _build_fake_image_info()
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        image_info['checksum'] = 'fake-checksum'
+        self.assertRaisesRegex(errors.InvalidCommandParamsError,
+                               'Image checksum is not',
+                               standby._validate_image_info,
+                               None,
+                               image_info)
+
     def test_validate_image_info_missing_field(self):
-        for field in ['id', 'urls', 'checksum']:
+        for field in ['id', 'urls', 'os_hash_value']:
             invalid_info = _build_fake_image_info()
             del invalid_info[field]
 
             self.assertRaises(errors.InvalidCommandParamsError,
                               standby._validate_image_info,
                               invalid_info)
 
@@ -369,103 +408,109 @@
                                                   preserve_ephemeral=pr_ep,
                                                   boot_mode=boot_mode,
                                                   disk_label=disk_label,
                                                   cpu_arch=cpu_arch)
 
         self.assertEqual(expected_uuid, work_on_disk_mock.return_value)
 
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
-    def test_download_image(self, requests_mock, open_mock, md5_mock):
+    def test_download_image(self, requests_mock, open_mock, hash_mock):
         image_info = _build_fake_image_info()
         response = requests_mock.return_value
         response.status_code = 200
         response.iter_content.return_value = ['some', 'content']
         file_mock = mock.Mock()
         open_mock.return_value.__enter__.return_value = file_mock
         file_mock.read.return_value = None
-        hexdigest_mock = md5_mock.return_value.hexdigest
-        hexdigest_mock.return_value = image_info['checksum']
+        hexdigest_mock = hash_mock.return_value.hexdigest
+        hexdigest_mock.return_value = image_info['os_hash_value']
 
         standby._download_image(image_info)
         requests_mock.assert_called_once_with(image_info['urls'][0],
                                               cert=None, verify=True,
                                               stream=True, proxies={},
                                               timeout=60)
         write = file_mock.write
         write.assert_any_call('some')
         write.assert_any_call('content')
         self.assertEqual(2, write.call_count)
 
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     @mock.patch.dict(os.environ, {})
     def test_download_image_proxy(
-            self, requests_mock, open_mock, md5_mock):
+            self, requests_mock, open_mock, hash_mock):
         image_info = _build_fake_image_info()
         proxies = {'http': 'http://a.b.com',
                    'https': 'https://secure.a.b.com'}
         no_proxy = '.example.org,.b.com'
         image_info['proxies'] = proxies
         image_info['no_proxy'] = no_proxy
+        image_info['os_hash_value'] = 'fake-checksum'
         response = requests_mock.return_value
         response.status_code = 200
         response.iter_content.return_value = ['some', 'content']
         file_mock = mock.Mock()
         open_mock.return_value.__enter__.return_value = file_mock
         file_mock.read.return_value = None
-        hexdigest_mock = md5_mock.return_value.hexdigest
-        hexdigest_mock.return_value = image_info['checksum']
+        hexdigest_mock = hash_mock.return_value.hexdigest
+        hexdigest_mock.return_value = 'fake-checksum'
 
         standby._download_image(image_info)
         self.assertEqual(no_proxy, os.environ['no_proxy'])
         requests_mock.assert_called_once_with(image_info['urls'][0],
                                               cert=None, verify=True,
                                               stream=True, proxies=proxies,
                                               timeout=60)
         write = file_mock.write
         write.assert_any_call('some')
         write.assert_any_call('content')
         self.assertEqual(2, write.call_count)
+        hash_mock.assert_has_calls([
+            mock.call('sha256'),
+            mock.call().update(b'some'),
+            mock.call().update(b'content'),
+            mock.call().hexdigest()])
 
     @mock.patch('requests.get', autospec=True)
     def test_download_image_bad_status(self, requests_mock):
         self.config(image_download_connection_retry_interval=0)
         image_info = _build_fake_image_info()
         response = requests_mock.return_value
         response.status_code = 404
         self.assertRaises(errors.ImageDownloadError,
                           standby._download_image,
                           image_info)
 
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_download_image_verify_fails(self, requests_mock, open_mock,
-                                         md5_mock):
+                                         hash_mock):
         image_info = _build_fake_image_info()
         response = requests_mock.return_value
         response.status_code = 200
-        hexdigest_mock = md5_mock.return_value.hexdigest
+        hexdigest_mock = hash_mock.return_value.hexdigest
         hexdigest_mock.return_value = 'invalid-checksum'
         self.assertRaises(errors.ImageChecksumError,
                           standby._download_image,
                           image_info)
 
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
-    def test_verify_image_success(self, requests_mock, open_mock, md5_mock):
+    def test_verify_image_success(self, requests_mock, open_mock, hash_mock):
         image_info = _build_fake_image_info()
         response = requests_mock.return_value
         response.status_code = 200
-        hexdigest_mock = md5_mock.return_value.hexdigest
-        hexdigest_mock.return_value = image_info['checksum']
+        hexdigest_mock = hash_mock.return_value.hexdigest
+        hexdigest_mock.return_value = image_info['os_hash_value']
         image_location = '/foo/bar'
         image_download = standby.ImageDownload(image_info)
         image_download.verify_image(image_location)
 
     @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
@@ -486,41 +531,65 @@
 
     @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_verify_image_success_without_md5(self, requests_mock,
                                               open_mock, hashlib_mock):
         image_info = _build_fake_image_info()
-        del image_info['checksum']
         image_info['os_hash_algo'] = 'sha512'
         image_info['os_hash_value'] = 'fake-sha512-value'
         response = requests_mock.return_value
         response.status_code = 200
         hexdigest_mock = hashlib_mock.return_value.hexdigest
         hexdigest_mock.return_value = image_info['os_hash_value']
         image_location = '/foo/bar'
         image_download = standby.ImageDownload(image_info)
         image_download.verify_image(image_location)
         hashlib_mock.assert_called_with('sha512')
 
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_verify_image_success_with_md5_fallback(self, requests_mock,
-                                                    open_mock, md5_mock):
+                                                    open_mock, hash_mock):
+        CONF.set_override('md5_enabled', True)
         image_info = _build_fake_image_info()
         image_info['os_hash_algo'] = 'algo-beyond-milky-way'
         image_info['os_hash_value'] = 'mysterious-alien-codes'
+        image_info['checksum'] = 'd41d8cd98f00b204e9800998ecf8427e'
         response = requests_mock.return_value
         response.status_code = 200
-        hexdigest_mock = md5_mock.return_value.hexdigest
+        hexdigest_mock = hash_mock.return_value.hexdigest
         hexdigest_mock.return_value = image_info['checksum']
         image_location = '/foo/bar'
         image_download = standby.ImageDownload(image_info)
         image_download.verify_image(image_location)
+        # NOTE(TheJulia): This is the one test which falls all the
+        # way back to md5 as the default, legacy logic because it
+        # got bad input to start with.
+        hash_mock.assert_has_calls([
+            mock.call('md5'),
+            mock.call().__bool__(),
+            mock.call().hexdigest()])
+
+    @mock.patch('hashlib.new', autospec=True)
+    @mock.patch('builtins.open', autospec=True)
+    @mock.patch('requests.get', autospec=True)
+    def test_verify_image_fails_if_unknown_is_used(self, requests_mock,
+                                                   open_mock, hash_mock):
+        image_info = _build_fake_image_info()
+        image_info['os_hash_algo'] = 'algo-beyond-milky-way'
+        image_info['os_hash_value'] = 'mysterious-alien-codes'
+        self.assertRaisesRegex(
+            errors.RESTError,
+            'An error occurred: Unable to verify image fake_id with '
+            'available checksums.',
+            standby.ImageDownload,
+            image_info)
+        hash_mock.assert_not_called()
 
     @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_verify_image_failure_with_new_hash_fields(self, requests_mock,
                                                        open_mock,
                                                        hashlib_mock):
@@ -534,36 +603,35 @@
         hexdigest_mock = hashlib_mock.return_value.hexdigest
         hexdigest_mock.return_value = 'invalid-checksum'
         self.assertRaises(errors.ImageChecksumError,
                           image_download.verify_image,
                           image_location)
         hashlib_mock.assert_called_with('sha512')
 
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
-    def test_verify_image_failure(self, requests_mock, open_mock, md5_mock):
+    def test_verify_image_failure(self, requests_mock, open_mock, hash_mock):
         image_info = _build_fake_image_info()
         response = requests_mock.return_value
         response.status_code = 200
         image_download = standby.ImageDownload(image_info)
         image_location = '/foo/bar'
-        hexdigest_mock = md5_mock.return_value.hexdigest
+        hexdigest_mock = hash_mock.return_value.hexdigest
         hexdigest_mock.return_value = 'invalid-checksum'
         self.assertRaises(errors.ImageChecksumError,
                           image_download.verify_image,
                           image_location)
 
     @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_verify_image_failure_without_fallback(self, requests_mock,
                                                    open_mock, hashlib_mock):
         image_info = _build_fake_image_info()
-        del image_info['checksum']
         image_info['os_hash_algo'] = 'unsupported-algorithm'
         image_info['os_hash_value'] = 'fake-value'
         response = requests_mock.return_value
         response.status_code = 200
         self.assertRaisesRegex(errors.RESTError,
                                'Unable to verify image.*'
                                'unsupported-algorithm',
@@ -1197,89 +1265,94 @@
                                                     'configdrive_data')
         download_mock.assert_called_once_with(image_info)
         write_mock.assert_called_once_with(image_info, device,
                                            'configdrive_data')
 
     @mock.patch('ironic_lib.disk_utils.block_uuid', autospec=True)
     @mock.patch('ironic_lib.disk_utils.fix_gpt_partition', autospec=True)
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_stream_raw_image_onto_device(self, requests_mock, open_mock,
-                                          md5_mock, fix_gpt_mock,
+                                          hash_mock, fix_gpt_mock,
                                           block_uuid_mock):
         image_info = _build_fake_image_info()
         response = requests_mock.return_value
         response.status_code = 200
         response.iter_content.return_value = ['some', 'content']
         file_mock = mock.Mock()
         open_mock.return_value.__enter__.return_value = file_mock
         file_mock.read.return_value = None
-        hexdigest_mock = md5_mock.return_value.hexdigest
-        hexdigest_mock.return_value = image_info['checksum']
+        hexdigest_mock = hash_mock.return_value.hexdigest
+        hexdigest_mock.return_value = image_info['os_hash_value']
         self.agent_extension.partition_uuids = {}
 
         block_uuid_mock.return_value = 'aaaabbbb'
-
         self.agent_extension._stream_raw_image_onto_device(image_info,
                                                            '/dev/foo')
+        hash_mock.assert_has_calls([
+            mock.call('sha256'),
+            mock.call().update(b'some'),
+            mock.call().update(b'content'),
+            mock.call().hexdigest()])
+
         requests_mock.assert_called_once_with(image_info['urls'][0],
                                               cert=None, verify=True,
                                               stream=True, proxies={},
                                               timeout=60)
         expected_calls = [mock.call('some'), mock.call('content')]
         file_mock.write.assert_has_calls(expected_calls)
         fix_gpt_mock.assert_called_once_with('/dev/foo', node_uuid=None)
         block_uuid_mock.assert_called_once_with('/dev/foo')
         self.assertEqual(
             'aaaabbbb',
             self.agent_extension.partition_uuids['root uuid']
         )
 
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_stream_raw_image_onto_device_write_error(self, requests_mock,
-                                                      open_mock, md5_mock):
+                                                      open_mock, hash_mock):
         self.config(image_download_connection_timeout=1)
         self.config(image_download_connection_retry_interval=0)
         image_info = _build_fake_image_info()
         response = requests_mock.return_value
         response.status_code = 200
-        response.iter_content.return_value = ['some', 'content']
+        response.iter_content.return_value = [b'some', b'content']
         file_mock = mock.Mock()
         open_mock.return_value.__enter__.return_value = file_mock
         file_mock.write.side_effect = Exception('Surprise!!!1!')
-        hexdigest_mock = md5_mock.return_value.hexdigest
-        hexdigest_mock.return_value = image_info['checksum']
+        hexdigest_mock = hash_mock.return_value.hexdigest
+        hexdigest_mock.return_value = image_info['os_hash_value']
 
         self.assertRaises(errors.ImageDownloadError,
                           self.agent_extension._stream_raw_image_onto_device,
                           image_info, '/dev/foo')
         calls = [mock.call('http://example.org', cert=None, proxies={},
                            stream=True, timeout=1, verify=True),
                  mock.call().iter_content(mock.ANY),
                  mock.call('http://example.org', cert=None, proxies={},
                            stream=True, timeout=1, verify=True),
                  mock.call().iter_content(mock.ANY),
                  mock.call('http://example.org', cert=None, proxies={},
                            stream=True, timeout=1, verify=True),
                  mock.call().iter_content(mock.ANY)]
         requests_mock.assert_has_calls(calls)
-        write_calls = [mock.call('some'),
-                       mock.call('some'),
-                       mock.call('some')]
+        write_calls = [mock.call(b'some'),
+                       mock.call(b'some'),
+                       mock.call(b'some')]
         file_mock.write.assert_has_calls(write_calls)
 
     @mock.patch('ironic_lib.disk_utils.fix_gpt_partition', autospec=True)
-    @mock.patch('hashlib.md5', autospec=True)
+    @mock.patch('hashlib.new', autospec=True)
     @mock.patch('builtins.open', autospec=True)
     @mock.patch('requests.get', autospec=True)
     def test_stream_raw_image_onto_device_socket_read_timeout(
-            self, requests_mock, open_mock, md5_mock, fix_gpt_mock):
+            self, requests_mock, open_mock, hash_mock, fix_gpt_mock):
 
         class create_timeout(object):
             status_code = 200
 
             def __init__(self, url, stream, proxies, verify, cert, timeout):
                 self.count = 0
 
@@ -1287,28 +1360,28 @@
                 return self
 
             def __next__(self):
                 if self.count:
                     time.sleep(0.1)
                     return None
                 self.count += 1
-                return "meow"
+                return b"meow"
 
             def iter_content(self, chunk_size):
                 return self
 
         self.config(image_download_connection_timeout=1)
         self.config(image_download_connection_retries=2)
         self.config(image_download_connection_retry_interval=0)
         image_info = _build_fake_image_info()
         file_mock = mock.Mock()
         open_mock.return_value.__enter__.return_value = file_mock
         file_mock.read.return_value = None
-        hexdigest_mock = md5_mock.return_value.hexdigest
-        hexdigest_mock.return_value = image_info['checksum']
+        hexdigest_mock = hash_mock.return_value.hexdigest
+        hexdigest_mock.return_value = image_info['os_hash_value']
         requests_mock.side_effect = create_timeout
         self.assertRaisesRegex(
             errors.ImageDownloadError,
             'Timed out reading next chunk',
             self.agent_extension._stream_raw_image_onto_device,
             image_info,
             '/dev/foo')
@@ -1317,17 +1390,17 @@
                            stream=True, proxies={}, timeout=1),
                  mock.call(image_info['urls'][0], cert=None, verify=True,
                            stream=True, proxies={}, timeout=1),
                  mock.call(image_info['urls'][0], cert=None, verify=True,
                            stream=True, proxies={}, timeout=1)]
         requests_mock.assert_has_calls(calls)
 
-        write_calls = [mock.call('meow'),
-                       mock.call('meow'),
-                       mock.call('meow')]
+        write_calls = [mock.call(b'meow'),
+                       mock.call(b'meow'),
+                       mock.call(b'meow')]
         file_mock.write.assert_has_calls(write_calls)
         fix_gpt_mock.assert_not_called()
 
     def test__message_format_partition_bios(self):
         image_info = _build_fake_partition_image_info()
         msg = ('image ({}) already present on device {} ')
         device = '/dev/fake'
@@ -1432,34 +1505,35 @@
                                                   disk_label='gpt',
                                                   cpu_arch=cpu_arch)
 
         self.assertEqual(expected_uuid, work_on_disk_mock.return_value)
         self.assertIsNone(node_uuid)
 
 
-@mock.patch('hashlib.md5', autospec=True)
+@mock.patch('hashlib.new', autospec=True)
 @mock.patch('requests.get', autospec=True)
 class TestImageDownload(base.IronicAgentTest):
 
-    def test_download_image(self, requests_mock, md5_mock):
+    def test_download_image(self, requests_mock, hash_mock):
         content = ['SpongeBob', 'SquarePants']
         response = requests_mock.return_value
         response.status_code = 200
         response.iter_content.return_value = content
 
         image_info = _build_fake_image_info()
-        md5_mock.return_value.hexdigest.return_value = image_info['checksum']
+        hash_mock.return_value.hexdigest.return_value = image_info[
+            'os_hash_value']
         image_download = standby.ImageDownload(image_info)
 
         self.assertEqual(content, list(image_download))
         requests_mock.assert_called_once_with(image_info['urls'][0],
                                               cert=None, verify=True,
                                               stream=True, proxies={},
                                               timeout=60)
-        self.assertEqual(image_info['checksum'],
+        self.assertEqual(image_info['os_hash_value'],
                          image_download._hash_algo.hexdigest())
 
     @mock.patch('time.sleep', autospec=True)
     def test_download_image_fail(self, sleep_mock, requests_mock, time_mock):
         response = requests_mock.return_value
         response.status_code = 401
         response.text = 'Unauthorized'
@@ -1498,64 +1572,97 @@
                                          timeout=60)
         self.assertEqual(3, requests_mock.call_count)
         sleep_mock.assert_called_with(10)
         self.assertEqual(2, sleep_mock.call_count)
 
     @mock.patch('time.sleep', autospec=True)
     def test_download_image_retries_success(self, sleep_mock, requests_mock,
-                                            md5_mock):
+                                            hash_mock):
         content = ['SpongeBob', 'SquarePants']
         fail_response = mock.Mock()
         fail_response.status_code = 500
         fail_response.text = " "
         response = mock.Mock()
         response.status_code = 200
         response.iter_content.return_value = content
         requests_mock.side_effect = [requests.Timeout, fail_response, response]
 
         image_info = _build_fake_image_info()
-        md5_mock.return_value.hexdigest.return_value = image_info['checksum']
+        hash_mock.return_value.hexdigest.return_value = image_info[
+            'os_hash_value']
         image_download = standby.ImageDownload(image_info)
 
         self.assertEqual(content, list(image_download))
         requests_mock.assert_called_with(image_info['urls'][0],
                                          cert=None, verify=True,
                                          stream=True, proxies={},
                                          timeout=60)
         self.assertEqual(3, requests_mock.call_count)
         sleep_mock.assert_called_with(10)
         self.assertEqual(2, sleep_mock.call_count)
 
-    def test_download_image_and_checksum(self, requests_mock, md5_mock):
+    def test_download_image_and_checksum(self, requests_mock, hash_mock):
         content = ['SpongeBob', 'SquarePants']
         fake_cs = "019fe036425da1c562f2e9f5299820bf"
         cs_response = mock.Mock()
         cs_response.status_code = 200
         cs_response.text = fake_cs + '\n'
         response = mock.Mock()
         response.status_code = 200
         response.iter_content.return_value = content
         requests_mock.side_effect = [cs_response, response]
 
         image_info = _build_fake_image_info()
+        image_info['os_hash_algo'] = 'sha512'
+        image_info['os_hash_value'] = 'http://example.com/checksum'
+        hash_mock.return_value.hexdigest.return_value = fake_cs
+        image_download = standby.ImageDownload(image_info)
+
+        self.assertEqual(content, list(image_download))
+        requests_mock.assert_has_calls([
+            mock.call('http://example.com/checksum', cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+            mock.call(image_info['urls'][0], cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+        ])
+        self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+
+    def test_download_image_and_checksum_md5(self, requests_mock, hash_mock):
+
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = "019fe036425da1c562f2e9f5299820bf"
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = fake_cs + '\n'
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = content
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info()
+        del image_info['os_hash_value']
+        del image_info['os_hash_algo']
+        CONF.set_override('md5_enabled', True)
         image_info['checksum'] = 'http://example.com/checksum'
-        md5_mock.return_value.hexdigest.return_value = fake_cs
+        hash_mock.return_value.hexdigest.return_value = fake_cs
         image_download = standby.ImageDownload(image_info)
 
         self.assertEqual(content, list(image_download))
         requests_mock.assert_has_calls([
             mock.call('http://example.com/checksum', cert=None, verify=True,
                       stream=True, proxies={}, timeout=60),
             mock.call(image_info['urls'][0], cert=None, verify=True,
                       stream=True, proxies={}, timeout=60),
         ])
         self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+        hash_mock.assert_has_calls([
+            mock.call('md5')])
 
-    def test_download_image_and_checksum_multiple(self, requests_mock,
-                                                  md5_mock):
+    def test_download_image_and_checksum_multiple_md5(self, requests_mock,
+                                                      hash_mock):
         content = ['SpongeBob', 'SquarePants']
         fake_cs = "019fe036425da1c562f2e9f5299820bf"
         cs_response = mock.Mock()
         cs_response.status_code = 200
         cs_response.text = """
 foobar  irrelevant file.img
 %s  image.img
@@ -1564,28 +1671,235 @@
         response.status_code = 200
         response.iter_content.return_value = content
         requests_mock.side_effect = [cs_response, response]
 
         image_info = _build_fake_image_info(
             'http://example.com/path/image.img')
         image_info['checksum'] = 'http://example.com/checksum'
-        md5_mock.return_value.hexdigest.return_value = fake_cs
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        CONF.set_override('md5_enabled', True)
+        hash_mock.return_value.hexdigest.return_value = fake_cs
+        image_download = standby.ImageDownload(image_info)
+
+        self.assertEqual(content, list(image_download))
+        requests_mock.assert_has_calls([
+            mock.call('http://example.com/checksum', cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+            mock.call(image_info['urls'][0], cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+        ])
+        self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+
+    def test_download_image_and_centos_checksum_md5(self, requests_mock,
+                                                    hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = "019fe036425da1c562f2e9f5299820bf"
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = """
+# centos-image.img: 1005593088 bytes
+MD5 (centos-image.img) = %s
+""" % fake_cs
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = content
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/centos-image.img')
+        image_info['checksum'] = 'http://example.com/checksum'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        CONF.set_override('md5_enabled', True)
+        hash_mock.return_value.hexdigest.return_value = fake_cs
+        image_download = standby.ImageDownload(image_info)
+
+        self.assertEqual(content, list(image_download))
+        requests_mock.assert_has_calls([
+            mock.call('http://example.com/checksum', cert=None,
+                      verify=True,
+                      stream=True, proxies={}, timeout=60),
+            mock.call(image_info['urls'][0], cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+        ])
+        self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+
+    def test_download_image_and_centos_checksum_sha256(self, requests_mock,
+                                                       hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = ('3b678e4fb651d450f4970e1647abc9b0a38bff3febd3d558753'
+                   '623c66369a633')
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = """
+# centos-image.img: 1005593088 bytes
+SHA256 (centos-image.img) = %s
+""" % fake_cs
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = iter(content)
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/centos-image.img')
+        image_info['checksum'] = 'http://example.com/checksum'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        hash_mock.return_value.hexdigest.return_value = fake_cs
+        image_download = standby.ImageDownload(image_info)
+
+        self.assertEqual(content, list(image_download))
+        requests_mock.assert_has_calls([
+            mock.call('http://example.com/checksum', cert=None,
+                      verify=True,
+                      stream=True, proxies={}, timeout=60),
+            mock.call(image_info['urls'][0], cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+        ])
+        self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+        hash_mock.assert_has_calls([
+            mock.call('sha256')])
+
+    def test_download_image_and_centos_checksum_sha512(self, requests_mock,
+                                                       hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = ('3b678e4fb651d450f4970e1647abc9b0a38bff3febd3d558753'
+                   '623c66369a6333b678e4fb651d450f4970e1647abc9b0a38b'
+                   'ff3febd3d558753623c66369a633')
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = """
+# centos-image.img: 1005593088 bytes
+SHA512 (centos-image.img) = %s
+""" % fake_cs
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = iter(content)
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/centos-image.img')
+        image_info['checksum'] = 'http://example.com/checksum'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        hash_mock.return_value.hexdigest.return_value = fake_cs
+        image_download = standby.ImageDownload(image_info)
+
+        self.assertEqual(content, list(image_download))
+        requests_mock.assert_has_calls([
+            mock.call('http://example.com/checksum', cert=None,
+                      verify=True,
+                      stream=True, proxies={}, timeout=60),
+            mock.call(image_info['urls'][0], cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+        ])
+        self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+        hash_mock.assert_has_calls([
+            mock.call('sha512')])
+
+    def test_download_image_and_checksum_multiple_sha256(self, requests_mock,
+                                                         hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = ('3b678e4fb651d450f4970e1647abc9b0a38bff3febd3d558753'
+                   '623c66369a633')
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = """
+foobar  irrelevant file.img
+%s  image.img
+""" % fake_cs
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = iter(content)
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/image.img')
+        image_info['checksum'] = 'http://example.com/checksum'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        hash_mock.return_value.hexdigest.return_value = fake_cs
         image_download = standby.ImageDownload(image_info)
 
         self.assertEqual(content, list(image_download))
         requests_mock.assert_has_calls([
             mock.call('http://example.com/checksum', cert=None, verify=True,
                       stream=True, proxies={}, timeout=60),
             mock.call(image_info['urls'][0], cert=None, verify=True,
                       stream=True, proxies={}, timeout=60),
         ])
         self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+        hash_mock.assert_has_calls([
+            mock.call('sha256')])
+
+    def test_download_image_and_checksum_multiple_sha512(self, requests_mock,
+                                                         hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = ('3b678e4fb651d450f4970e1647abc9b0a38bff3febd3d558753'
+                   '623c66369a6333b678e4fb651d450f4970e1647abc9b0a38b'
+                   'ff3febd3d558753623c66369a633')
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = """
+foobar  irrelevant file.img
+%s  image.img
+""" % fake_cs
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = iter(content)
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/image.img')
+        image_info['checksum'] = 'http://example.com/checksum'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        hash_mock.return_value.hexdigest.return_value = fake_cs
+        image_download = standby.ImageDownload(image_info)
+
+        self.assertEqual(content, list(image_download))
+        requests_mock.assert_has_calls([
+            mock.call('http://example.com/checksum', cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+            mock.call(image_info['urls'][0], cert=None, verify=True,
+                      stream=True, proxies={}, timeout=60),
+        ])
+        self.assertEqual(fake_cs, image_download._hash_algo.hexdigest())
+        hash_mock.assert_has_calls([
+            mock.call('sha512')])
 
     def test_download_image_and_checksum_unknown_file(self, requests_mock,
-                                                      md5_mock):
+                                                      hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = "019fe036425da1c562f2e9f5299820bf"
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = """
+foobar  irrelevant file.img
+%s  not-my-image.img
+""" % fake_cs
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = content
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/image.img')
+        image_info['os_hash_algo'] = 'sha512'
+        image_info['os_hash_value'] = 'http://example.com/checksum'
+        hash_mock.return_value.hexdigest.return_value = fake_cs
+        self.assertRaisesRegex(errors.ImageDownloadError,
+                               'Checksum file does not contain name image.img',
+                               standby.ImageDownload, image_info)
+
+    def test_download_image_and_checksum_unknown_file_md5(self,
+                                                          requests_mock,
+                                                          hash_mock):
+        CONF.set_override('md5_enabled', True)
         content = ['SpongeBob', 'SquarePants']
         fake_cs = "019fe036425da1c562f2e9f5299820bf"
         cs_response = mock.Mock()
         cs_response.status_code = 200
         cs_response.text = """
 foobar  irrelevant file.img
 %s  not-my-image.img
@@ -1594,38 +1908,88 @@
         response.status_code = 200
         response.iter_content.return_value = content
         requests_mock.side_effect = [cs_response, response]
 
         image_info = _build_fake_image_info(
             'http://example.com/path/image.img')
         image_info['checksum'] = 'http://example.com/checksum'
-        md5_mock.return_value.hexdigest.return_value = fake_cs
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        hash_mock.return_value.hexdigest.return_value = fake_cs
         self.assertRaisesRegex(errors.ImageDownloadError,
                                'Checksum file does not contain name image.img',
                                standby.ImageDownload, image_info)
 
-    def test_download_image_and_checksum_empty_file(self, requests_mock,
-                                                    md5_mock):
+    def test_download_image_and_checksum_empty_file_md5(self, requests_mock,
+                                                        hash_mock):
+        CONF.set_override('md5_enabled', True)
         content = ['SpongeBob', 'SquarePants']
         cs_response = mock.Mock()
         cs_response.status_code = 200
         cs_response.text = " "
         response = mock.Mock()
         response.status_code = 200
         response.iter_content.return_value = content
         requests_mock.side_effect = [cs_response, response]
 
         image_info = _build_fake_image_info(
             'http://example.com/path/image.img')
         image_info['checksum'] = 'http://example.com/checksum'
+        del image_info['os_hash_algo']
+        del image_info['os_hash_value']
+        self.assertRaisesRegex(errors.ImageDownloadError,
+                               'Empty checksum file',
+                               standby.ImageDownload, image_info)
+
+    def test_download_image_and_checksum_empty_file(self, requests_mock,
+                                                    hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = " "
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = content
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/image.img')
+        image_info['os_hash_algo'] = 'sha512'
+        image_info['os_hash_value'] = 'http://example.com/checksum'
         self.assertRaisesRegex(errors.ImageDownloadError,
                                'Empty checksum file',
                                standby.ImageDownload, image_info)
 
-    def test_download_image_and_checksum_failed(self, requests_mock, md5_mock):
+    def test_download_image_and_checksum_failed(self, requests_mock,
+                                                hash_mock):
+        self.config(image_download_connection_retry_interval=0)
+        content = ['SpongeBob', 'SquarePants']
+        cs_response = mock.Mock()
+        cs_response.status_code = 400
+        cs_response.text = " "
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = content
+        # 3 retries on status code
+        requests_mock.side_effect = [cs_response, cs_response, cs_response,
+                                     response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/image.img')
+        image_info['os_hash_value'] = 'http://example.com/checksum'
+        image_info['os_hash_algo'] = 'sha512'
+        self.assertRaisesRegex(errors.ImageDownloadError,
+                               'Received status code 400 from '
+                               'http://example.com/checksum',
+                               standby.ImageDownload, image_info)
+
+    def test_download_image_and_checksum_failed_md5(self,
+                                                    requests_mock,
+                                                    hash_mock):
+        CONF.set_override('md5_enabled', True)
         self.config(image_download_connection_retry_interval=0)
         content = ['SpongeBob', 'SquarePants']
         cs_response = mock.Mock()
         cs_response.status_code = 400
         cs_response.text = " "
         response = mock.Mock()
         response.status_code = 200
@@ -1633,11 +1997,34 @@
         # 3 retries on status code
         requests_mock.side_effect = [cs_response, cs_response, cs_response,
                                      response]
 
         image_info = _build_fake_image_info(
             'http://example.com/path/image.img')
         image_info['checksum'] = 'http://example.com/checksum'
+        del image_info['os_hash_value']
+        del image_info['os_hash_algo']
         self.assertRaisesRegex(errors.ImageDownloadError,
                                'Received status code 400 from '
                                'http://example.com/checksum',
                                standby.ImageDownload, image_info)
+
+    def test_download_image_and_invalid_checksum(self, requests_mock,
+                                                 hash_mock):
+        content = ['SpongeBob', 'SquarePants']
+        fake_cs = "invalid"
+        cs_response = mock.Mock()
+        cs_response.status_code = 200
+        cs_response.text = fake_cs + '\n'
+        response = mock.Mock()
+        response.status_code = 200
+        response.iter_content.return_value = content
+        requests_mock.side_effect = [cs_response, response]
+
+        image_info = _build_fake_image_info(
+            'http://example.com/path/image.img')
+        image_info['os_hash_algo'] = 'sha512'
+        image_info['os_hash_value'] = 'http://example.com/checksum'
+        self.assertRaisesRegex(
+            errors.ImageDownloadError,
+            r"Invalid checksum file \(No valid checksum found\) \['invalid'\]",
+            standby.ImageDownload, image_info)
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/nvidia/test_nvidia_fw_update.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/test_cna.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/hardware_managers/test_mlnx.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/samples/hardware_samples.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/samples/hardware_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -487,14 +487,42 @@
       "vendor" : "ABCD",
       "physid" : "0",
       "version" : "1234",
       "serial" : "1234",
       "slot" : "NULL",
       "children" : [
         {
+          "id": "firmware",
+          "class": "memory",
+          "claimed": true,
+          "description": "BIOS",
+          "vendor": "BIOSVNDR",
+          "physid": "0",
+          "version": "1.2.3",
+          "date": "03/30/2023",
+          "units": "bytes",
+          "size": 65536,
+          "capacity": 16777216,
+          "capabilities": {
+            "isa": "ISA bus",
+            "pci": "PCI bus",
+            "pnp": "Plug-and-Play",
+            "upgrade": "BIOS EEPROM can be upgraded",
+            "shadowing": "BIOS shadowing",
+            "cdboot": "Booting from CD-ROM/DVD",
+            "bootselect": "Selectable boot path",
+            "edd": "Enhanced Disk Drive extensions",
+            "acpi": "ACPI",
+            "usb": "USB legacy emulation",
+            "biosbootspecification": "BIOS boot specification",
+            "netboot": "Function-key initiated network service boot",
+            "uefi": "UEFI specification is supported"
+          }
+        },
+        {
           "id" : "memory:0",
           "class" : "memory",
           "claimed" : true,
           "handle" : "DMI:004A",
           "description" : "System Memory",
           "physid" : "4a",
           "slot" : "System board or motherboard",
@@ -629,14 +657,68 @@
           "class" : "memory",
           "physid" : "1"
         },
         {
           "id" : "memory:5",
           "class" : "memory",
           "physid" : "2"
+        },
+        {
+          "id" : "network:0",
+          "class" : "network",
+          "handle" : "PCI:0000:00:14.3",
+          "description" : "Wireless interface",
+          "product" : "ABCD",
+          "vendor" : "ABCD",
+          "physid" : "14.3",
+          "businfo" : "pci@0000:00:14.3",
+          "logicalname" : "wlp0s20f3",
+          "width" : 64,
+          "clock" : 33000000,
+          "capabilities" : {
+            "pm" : "Power Management",
+            "msi" : "Message Signalled Interrupts",
+            "pciexpress" : "PCI Express",
+            "msix" : "MSI-X",
+            "bus_master" : "bus mastering",
+            "cap_list" : "PCI capabilities listing",
+            "ethernet" : true,
+            "physical" : "Physical interface",
+            "wireless" : "Wireless-LAN"
+          }
+        },
+        {
+          "id" : "network:1",
+          "class" : "network",
+          "handle" : "PCI:0000:00:1f.6",
+          "description" : "Ethernet interface",
+          "product" : "DCBA",
+          "vendor" : "DCBA",
+          "physid" : "1f.6",
+          "businfo" : "pci@0000:00:1f.6",
+          "logicalname" : "eth0",
+          "units" : "bit/s",
+          "capacity" : 1000000000,
+          "width" : 32,
+          "clock" : 33000000,
+          "capabilities" : {
+            "pm" : "Power Management",
+            "msi" : "Message Signalled Interrupts",
+            "bus_master" : "bus mastering",
+            "cap_list" : "PCI capabilities listing",
+            "ethernet" : true,
+            "physical" : "Physical interface",
+            "tp" : "twisted pair",
+            "10bt" : "10Mbit/s",
+            "10bt-fd" : "10Mbit/s (full duplex)",
+            "100bt" : "100Mbit/s",
+            "100bt-fd" : "100Mbit/s (full duplex)",
+            "1000bt-fd" : "1Gbit/s (full duplex)",
+            "autonegotiation" : "Auto-negotiation"
+          }
         }
       ]
     }
   ]
 }
 """, "")
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_agent.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_agent.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_api.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_base.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_burnin.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_burnin.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_dmi_inspector.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_dmi_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_efi_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_efi_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 from ironic_python_agent import partition_utils
 from ironic_python_agent import raid_utils
 from ironic_python_agent.tests.unit import base
 from ironic_python_agent.tests.unit.samples import hardware_samples
 from ironic_python_agent import utils
 
 
+EFI_RESULT = ''.encode('utf-16')
+
+
 @mock.patch.object(os, 'walk', autospec=True)
 @mock.patch.object(os, 'access', autospec=False)
 class TestGetEfiBootloaders(base.IronicAgentTest):
 
     def test__no_efi_bootloaders(self, mock_access, mock_walk):
         # No valid efi file.
         mock_walk.return_value = [
@@ -111,24 +114,24 @@
                                            self.fake_efi_system_part,
                                            self.fake_dir)
         expected = []
         self.assertIsNone(result)
         mock_execute.assert_has_calls(expected)
 
     def test__run_efibootmgr(self, mock_execute):
-        mock_execute.return_value = ('', '')
+        mock_execute.return_value = (''.encode('utf-16'), '')
         result = efi_utils._run_efibootmgr(['EFI/BOOT/BOOTX64.EFI'],
                                            self.fake_dev,
                                            self.fake_efi_system_part,
                                            self.fake_dir)
-        expected = [mock.call('efibootmgr', '-v'),
+        expected = [mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', self.fake_efi_system_part, '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI')]
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True)]
         self.assertIsNone(result)
         mock_execute.assert_has_calls(expected)
 
 
 @mock.patch.object(shutil, 'rmtree', lambda *_: None)
 @mock.patch.object(tempfile, 'mkdtemp', lambda *_: '/tmp/fake-dir')
 @mock.patch.object(utils, 'rescan_device', autospec=True)
@@ -172,27 +175,26 @@
                 mock_utils_efi_part, mock_get_part_path, mock_get_part_uuid,
                 mock_execute, mock_rescan):
         mock_utils_efi_part.return_value = {'number': '1'}
         mock_get_part_path.return_value = self.fake_efi_system_part
         mock_is_md_device.return_value = False
 
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI']
-
-        mock_execute.side_effect = iter([('', ''), ('', ''),
-                                         ('', ''), ('', ''),
+        mock_execute.side_effect = iter([('', ''), (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''), ('', ''),
                                          ('', ''), ('', ''),
                                          ('', '')])
 
         expected = [mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         result = efi_utils.manage_uefi(self.fake_dev, self.fake_root_uuid)
         self.assertTrue(result)
         mkdir_mock.assert_called_once_with(self.fake_dir + '/boot/efi')
@@ -215,38 +217,42 @@
 
         # Format is <file>,<entry_name>,<options>,humanfriendlytextnotused
         # https://www.rodsbooks.com/efi-bootloaders/fallback.html
         # Mild difference, Ubuntu ships a file without a 0xFEFF delimiter
         # at the start of the file, where as Red Hat *does*
         csv_file_data = u'shimx64.efi,Vendor String,,Grub2MadeUSDoThis\n'
         # This test also handles deleting a pre-existing matching vendor
-        # string in advance.
+        # string in advance. This string also includes a UTF16 character
+        # *on* purpose, to force proper decoding to be tested and garbage
+        # characters which can be found in OVMF test VM NVRAM records.
         dupe_entry = """
 BootCurrent: 0001
 Timeout: 0 seconds
 BootOrder: 0000,00001
-Boot0000* Vendor String HD(1,GPT,4f3c6294-bf9b-4208-9808-be45dfc34b5c)File(\EFI\Boot\BOOTX64.EFI)
-Boot0001 Vendor String HD(2,GPT,4f3c6294-bf9b-4208-9808-be45dfc34b5c)File(\EFI\Boot\BOOTX64.EFI)
-Boot0002: VENDMAGIC FvFile(9f3c6294-bf9b-4208-9808-be45dfc34b51)
+Boot0000 UTF16ÿ HD(1,GPT,4f3c6294-bf9b-4208-9808-be45dfc34b5c)File(\EFI\Boot\BOOTX64.EFI)
+Boot0001* Vendor String HD(1,GPT,4f3c6294-bf9b-4208-9808-be45dfc34b5c)File(\EFI\Boot\BOOTX64.EFI)
+Boot0002 Vendor String HD(2,GPT,4f3c6294-bf9b-4208-9808-be45dfc34b5c)File(\EFI\Boot\BOOTX64.EFI)
+Boot0003: VENDMAGIC FvFile(9f3c6294-bf9b-4208-9808-be45dfc34b51)N.....YM....R,Y.
 """  # noqa This is a giant literal string for testing.
-
-        mock_execute.side_effect = iter([('', ''), (dupe_entry, ''),
+        dupe_entry = dupe_entry.encode('utf-16')
+        mock_execute.side_effect = iter([('', ''),
+                                         (dupe_entry, ''),
                                          ('', ''), ('', ''),
                                          ('', ''), ('', ''),
                                          ('', '')])
 
         expected = [mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
-                    mock.call('efibootmgr', '-b', '0000', '-B'),
-                    mock.call('efibootmgr', '-b', '0001', '-B'),
+                    mock.call('efibootmgr', '-v', binary=True),
+                    mock.call('efibootmgr', '-b', '0001', '-B', binary=True),
+                    mock.call('efibootmgr', '-b', '0002', '-B', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'Vendor String', '-l',
-                              '\\EFI\\vendor\\shimx64.efi'),
+                              '\\EFI\\vendor\\shimx64.efi', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
         with mock.patch('builtins.open',
                         mock.mock_open(read_data=csv_file_data)):
             result = efi_utils.manage_uefi(self.fake_dev, self.fake_root_uuid)
         self.assertTrue(result)
@@ -262,27 +268,26 @@
                          mock_utils_efi_part, mock_get_part_path,
                          mock_get_part_uuid, mock_execute, mock_rescan):
         mock_utils_efi_part.return_value = None
         mock_get_part_uuid.return_value = '/dev/fakenvme0p1'
         mock_is_md_device.return_value = False
 
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI']
-
-        mock_execute.side_effect = iter([('', ''), ('', ''),
-                                         ('', ''), ('', ''),
+        mock_execute.side_effect = iter([('', ''), (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''), ('', ''),
                                          ('', ''), ('', ''),
                                          ('', '')])
 
         expected = [mock.call('mount', '/dev/fakenvme0p1',
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', '/dev/fakenvme0',
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         result = efi_utils.manage_uefi('/dev/fakenvme0', self.fake_root_uuid)
         self.assertTrue(result)
         mkdir_mock.assert_called_once_with(self.fake_dir + '/boot/efi')
@@ -297,27 +302,26 @@
                        mock_utils_efi_part, mock_get_part_path,
                        mock_get_part_uuid, mock_execute, mock_rescan):
         mock_utils_efi_part.return_value = {'number': '1'}
         mock_get_part_path.return_value = self.fake_efi_system_part
         mock_is_md_device.return_value = False
 
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI']
-
-        mock_execute.side_effect = iter([('', ''), ('', ''),
-                                         ('', ''), ('', ''),
+        mock_execute.side_effect = iter([('', ''), (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''), ('', ''),
                                          ('', ''), ('', ''),
                                          ('', '')])
 
         expected = [mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', self.fake_dev,
                               '-p', '1', '-w',
                               '-L', 'ironic1', '-l',
-                              '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         result = efi_utils.manage_uefi(self.fake_dev, None)
         self.assertTrue(result)
         mkdir_mock.assert_called_once_with(self.fake_dir + '/boot/efi')
@@ -343,35 +347,38 @@
         mock_get_part_path.return_value = self.fake_efi_system_part
         mock_is_md_device.return_value = True
         mock_get_holder_disks.return_value = ['/dev/sda', '/dev/sdb']
         mock_prepare.return_value = '/dev/md125'
         mock_get_component_devices.return_value = ['/dev/sda3', '/dev/sdb3']
 
         mock_efi_bl.return_value = ['EFI/BOOT/BOOTX64.EFI']
-
-        mock_execute.side_effect = iter([('', ''), ('', ''),
-                                         ('', ''), ('', ''),
-                                         ('', ''), ('', ''),
-                                         ('', ''), ('', ''),
+        mock_execute.side_effect = iter([('', ''),
+                                         ('', ''),
+                                         ('', ''),
+                                         (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''),
+                                         (EFI_RESULT, ''),
+                                         ('', ''),
                                          ('', '')])
 
         expected = [mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', '/dev/sda3',
                               '-p', '3', '-w', '-L', 'ironic1 (RAID, part0)',
-                              '-l', '\\EFI\\BOOT\\BOOTX64.EFI'),
-                    mock.call('efibootmgr', '-v'),
+                              '-l', '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('efibootmgr', '-v', '-c', '-d', '/dev/sdb3',
                               '-p', '3', '-w', '-L', 'ironic1 (RAID, part1)',
-                              '-l', '\\EFI\\BOOT\\BOOTX64.EFI'),
+                              '-l', '\\EFI\\BOOT\\BOOTX64.EFI', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         result = efi_utils.manage_uefi(self.fake_dev, None)
         self.assertTrue(result)
         mkdir_mock.assert_called_once_with(self.fake_dir + '/boot/efi')
@@ -421,15 +428,15 @@
             processutils.ProcessExecutionError('boom'),
             ('', ''),
             ('', ''),
         ]
 
         expected = [mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True),
                     mock.call('sync')]
 
         self.assertRaisesRegex(errors.CommandExecutionError, 'boom',
                                efi_utils.manage_uefi,
                                self.fake_dev, self.fake_root_uuid)
@@ -458,15 +465,15 @@
             processutils.ProcessExecutionError('boom'),
             processutils.ProcessExecutionError('no umount'),
             ('', ''),
         ]
 
         expected = [mock.call('mount', self.fake_efi_system_part,
                               self.fake_dir + '/boot/efi'),
-                    mock.call('efibootmgr', '-v'),
+                    mock.call('efibootmgr', '-v', binary=True),
                     mock.call('umount', self.fake_dir + '/boot/efi',
                               attempts=3, delay_on_retry=True)]
 
         self.assertRaisesRegex(errors.CommandExecutionError, 'boom',
                                efi_utils.manage_uefi,
                                self.fake_dev, self.fake_root_uuid)
         mkdir_mock.assert_called_once_with(self.fake_dir + '/boot/efi')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_encoding.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_encoding.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_errors.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_hardware.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_hardware.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,99 +265,14 @@
                 (1, '666f6f01')],
         }
         result = self.hardware.collect_lldp_data(if_names)
         mock_log.warning.assert_called_once()
         self.assertIn(if_names[0], result)
         self.assertEqual(expected_lldp_data, result)
 
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_interfaces(self,
-                                     mock_has_carrier,
-                                     mock_get_mac,
-                                     mocked_execute,
-                                     mocked_open,
-                                     mocked_exists,
-                                     mocked_listdir,
-                                     mocked_ifaddresses,
-                                     mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        mocked_listdir.return_value = ['lo', 'eth0', 'foobar']
-        mocked_exists.side_effect = [False, False, True, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_execute.return_value = ('em0\n', '')
-        mock_has_carrier.return_value = True
-        mock_get_mac.side_effect = [
-            '00:0c:29:8c:11:b1',
-            None,
-        ]
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(1, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        self.assertIsNone(interfaces[0].lldp)
-        self.assertTrue(interfaces[0].has_carrier)
-        self.assertEqual('em0', interfaces[0].biosdevname)
-
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_interfaces_with_biosdevname(self,
-                                                      mock_has_carrier,
-                                                      mock_get_mac,
-                                                      mocked_execute,
-                                                      mocked_open,
-                                                      mocked_exists,
-                                                      mocked_listdir,
-                                                      mocked_ifaddresses,
-                                                      mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_execute.return_value = ('em0\n', '')
-        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
-        mock_has_carrier.return_value = True
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(1, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        self.assertIsNone(interfaces[0].lldp)
-        self.assertTrue(interfaces[0].has_carrier)
-        self.assertEqual('em0', interfaces[0].biosdevname)
-
     @mock.patch.object(il_utils, 'execute', autospec=True)
     def test_get_bios_given_nic_name_ok(self, mock_execute):
         interface_name = 'eth0'
         mock_execute.return_value = ('em0\n', '')
         result = self.hardware.get_bios_given_nic_name(interface_name)
         self.assertEqual('em0', result)
         mock_execute.assert_called_once_with('biosdevname', '-i',
@@ -401,418 +316,14 @@
 
         mock_log.warning.assert_called_once_with(
             'Biosdevname returned exit code %s', 3)
         self.assertIsNone(result)
         mock_execute.assert_called_once_with('biosdevname', '-i',
                                              interface_name)
 
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('ironic_python_agent.netutils.get_lldp_info', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_interfaces_with_lldp(self,
-                                               mock_has_carrier,
-                                               mock_get_mac,
-                                               mocked_execute,
-                                               mocked_open,
-                                               mocked_exists,
-                                               mocked_listdir,
-                                               mocked_ifaddresses,
-                                               mocked_lldp_info,
-                                               mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        CONF.set_override('collect_lldp', True)
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_lldp_info.return_value = {'eth0': [
-            (0, b''),
-            (1, b'\x04\x88Z\x92\xecTY'),
-            (2, b'\x05Ethernet1/18'),
-            (3, b'\x00x')]
-        }
-        mock_has_carrier.return_value = True
-        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
-        mocked_execute.return_value = ('em0\n', '')
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(1, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        expected_lldp_info = [
-            (0, ''),
-            (1, '04885a92ec5459'),
-            (2, '0545746865726e6574312f3138'),
-            (3, '0078'),
-        ]
-        self.assertEqual(expected_lldp_info, interfaces[0].lldp)
-        self.assertTrue(interfaces[0].has_carrier)
-        self.assertEqual('em0', interfaces[0].biosdevname)
-
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('ironic_python_agent.netutils.get_lldp_info', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    def test_list_network_interfaces_with_lldp_error(
-            self, mocked_execute, mocked_open, mocked_exists, mocked_listdir,
-            mocked_ifaddresses, mocked_lldp_info, mockedget_managers,
-            mock_get_mac, mock_has_carrier):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        CONF.set_override('collect_lldp', True)
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_lldp_info.side_effect = Exception('Boom!')
-        mocked_execute.return_value = ('em0\n', '')
-        mock_has_carrier.return_value = True
-        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(1, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        self.assertIsNone(interfaces[0].lldp)
-        self.assertTrue(interfaces[0].has_carrier)
-        self.assertEqual('em0', interfaces[0].biosdevname)
-
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_interfaces_no_carrier(self,
-                                                mock_has_carrier,
-                                                mock_get_mac,
-                                                mocked_execute,
-                                                mocked_open,
-                                                mocked_exists,
-                                                mocked_listdir,
-                                                mocked_ifaddresses,
-                                                mockedget_managers):
-
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = [OSError('boom')]
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_execute.return_value = ('em0\n', '')
-        mock_has_carrier.return_value = False
-        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(1, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        self.assertFalse(interfaces[0].has_carrier)
-        self.assertIsNone(interfaces[0].vendor)
-        self.assertEqual('em0', interfaces[0].biosdevname)
-
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_interfaces_with_vendor_info(self,
-                                                      mock_has_carrier,
-                                                      mock_get_mac,
-                                                      mocked_execute,
-                                                      mocked_open,
-                                                      mocked_exists,
-                                                      mocked_listdir,
-                                                      mocked_ifaddresses,
-                                                      mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        mac = '00:0c:29:8c:11:b1'
-        read_mock.side_effect = ['0x15b3\n', '0x1014\n']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_execute.return_value = ('em0\n', '')
-        mock_has_carrier.return_value = True
-        mock_get_mac.return_value = mac
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(1, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual(mac, interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        self.assertTrue(interfaces[0].has_carrier)
-        self.assertEqual('0x15b3', interfaces[0].vendor)
-        self.assertEqual('0x1014', interfaces[0].product)
-        self.assertEqual('em0', interfaces[0].biosdevname)
-
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_interfaces_with_bond(self,
-                                               mock_has_carrier,
-                                               mock_get_mac,
-                                               mocked_execute,
-                                               mocked_open,
-                                               mocked_exists,
-                                               mocked_listdir,
-                                               mocked_ifaddresses,
-                                               mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        mocked_listdir.return_value = ['lo', 'bond0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_execute.return_value = ('\n', '')
-        mock_has_carrier.return_value = True
-        mock_get_mac.side_effect = [
-            '00:0c:29:8c:11:b1',
-            None,
-        ]
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(1, len(interfaces))
-        self.assertEqual('bond0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        self.assertIsNone(interfaces[0].lldp)
-        self.assertTrue(interfaces[0].has_carrier)
-        self.assertEqual('', interfaces[0].biosdevname)
-
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_vlan_interfaces(self,
-                                          mock_has_carrier,
-                                          mock_get_mac,
-                                          mocked_execute,
-                                          mocked_open,
-                                          mocked_exists,
-                                          mocked_listdir,
-                                          mocked_ifaddresses,
-                                          mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        CONF.set_override('enable_vlan_interfaces', 'eth0.100')
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_execute.return_value = ('em0\n', '')
-        mock_get_mac.mock_has_carrier = True
-        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(2, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
-        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
-        self.assertIsNone(interfaces[0].lldp)
-        self.assertEqual('eth0.100', interfaces[1].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[1].mac_address)
-        self.assertIsNone(interfaces[1].lldp)
-
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('ironic_python_agent.netutils.get_lldp_info', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_vlan_interfaces_using_lldp(self,
-                                                     mock_has_carrier,
-                                                     mock_get_mac,
-                                                     mocked_execute,
-                                                     mocked_open,
-                                                     mocked_exists,
-                                                     mocked_listdir,
-                                                     mocked_ifaddresses,
-                                                     mocked_lldp_info,
-                                                     mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        CONF.set_override('collect_lldp', True)
-        CONF.set_override('enable_vlan_interfaces', 'eth0')
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_execute.return_value = ('em0\n', '')
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_lldp_info.return_value = {'eth0': [
-            (0, b''),
-            (127, b'\x00\x80\xc2\x03\x00d\x08vlan-100'),
-            (127, b'\x00\x80\xc2\x03\x00e\x08vlan-101')]
-        }
-        mock_has_carrier.return_value = True
-        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(3, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
-        expected_lldp_info = [
-            (0, ''),
-            (127, "0080c203006408766c616e2d313030"),
-            (127, "0080c203006508766c616e2d313031")
-        ]
-        self.assertEqual(expected_lldp_info, interfaces[0].lldp)
-        self.assertEqual('eth0.100', interfaces[1].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[1].mac_address)
-        self.assertIsNone(interfaces[1].lldp)
-        self.assertEqual('eth0.101', interfaces[2].name)
-        self.assertEqual('00:0c:29:8c:11:b1', interfaces[2].mac_address)
-        self.assertIsNone(interfaces[2].lldp)
-
-    @mock.patch.object(netutils, 'LOG', autospec=True)
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('netifaces.ifaddresses', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    @mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
-    def test_list_network_vlan_invalid_int(self,
-                                           mock_has_carrier,
-                                           mock_get_mac,
-                                           mocked_execute,
-                                           mocked_open,
-                                           mocked_exists,
-                                           mocked_listdir,
-                                           mocked_ifaddresses,
-                                           mockedget_managers,
-                                           mocked_log):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        CONF.set_override('collect_lldp', True)
-        CONF.set_override('enable_vlan_interfaces', 'enp0s1')
-        mocked_listdir.return_value = ['lo', 'eth0']
-        mocked_exists.side_effect = [False, False, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_ifaddresses.return_value = {
-            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
-            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
-        }
-        mocked_execute.return_value = ('em0\n', '')
-        mock_get_mac.mock_has_carrier = True
-        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
-
-        self.hardware.list_network_interfaces()
-        mocked_log.warning.assert_called_once_with(
-            'Provided interface name %s was not found', 'enp0s1')
-
-    @mock.patch('ironic_python_agent.hardware.get_managers', autospec=True)
-    @mock.patch('ironic_python_agent.netutils.get_lldp_info', autospec=True)
-    @mock.patch('os.listdir', autospec=True)
-    @mock.patch('os.path.exists', autospec=True)
-    @mock.patch('builtins.open', autospec=True)
-    @mock.patch.object(il_utils, 'execute', autospec=True)
-    @mock.patch.object(netutils, 'get_mac_addr', autospec=True)
-    def test_list_network_vlan_interfaces_using_lldp_all(self,
-                                                         mock_get_mac,
-                                                         mocked_execute,
-                                                         mocked_open,
-                                                         mocked_exists,
-                                                         mocked_listdir,
-                                                         mocked_lldp_info,
-                                                         mockedget_managers):
-        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
-        CONF.set_override('collect_lldp', True)
-        CONF.set_override('enable_vlan_interfaces', 'all')
-        mocked_listdir.return_value = ['lo', 'eth0', 'eth1']
-        mocked_execute.return_value = ('em0\n', '')
-        mocked_exists.side_effect = [False, False, True, True]
-        mocked_open.return_value.__enter__ = lambda s: s
-        mocked_open.return_value.__exit__ = mock.Mock()
-        read_mock = mocked_open.return_value.read
-        read_mock.side_effect = ['1']
-        mocked_lldp_info.return_value = {'eth0': [
-            (0, b''),
-            (127, b'\x00\x80\xc2\x03\x00d\x08vlan-100'),
-            (127, b'\x00\x80\xc2\x03\x00e\x08vlan-101')],
-            'eth1': [
-            (0, b''),
-            (127, b'\x00\x80\xc2\x03\x00f\x08vlan-102'),
-            (127, b'\x00\x80\xc2\x03\x00g\x08vlan-103')]
-        }
-
-        interfaces = self.hardware.list_network_interfaces()
-        self.assertEqual(6, len(interfaces))
-        self.assertEqual('eth0', interfaces[0].name)
-        self.assertEqual('eth1', interfaces[1].name)
-        self.assertEqual('eth0.100', interfaces[2].name)
-        self.assertEqual('eth0.101', interfaces[3].name)
-        self.assertEqual('eth1.102', interfaces[4].name)
-        self.assertEqual('eth1.103', interfaces[5].name)
-
     @mock.patch.object(hardware, 'get_multipath_status', autospec=True)
     @mock.patch.object(os, 'readlink', autospec=True)
     @mock.patch.object(os, 'listdir', autospec=True)
     @mock.patch.object(hardware, 'get_cached_node', autospec=True)
     @mock.patch.object(il_utils, 'execute', autospec=True)
     def test_get_os_install_device(self, mocked_execute, mock_cached_node,
                                    mocked_listdir, mocked_readlink,
@@ -1476,16 +987,19 @@
         mocked_psutil.return_value.total = 3952 * 1024 * 1024
         mocked_execute.return_value = (f"[{hws.LSHW_JSON_OUTPUT_V2[0]}]", "")
         mem = self.hardware.get_memory()
 
         self.assertEqual(3952 * 1024 * 1024, mem.total)
         self.assertEqual(65536, mem.physical_mb)
 
-    @mock.patch('ironic_python_agent.netutils.get_hostname', autospec=True)
-    def test_list_hardware_info(self, mocked_get_hostname):
+    @mock.patch.object(hardware.GenericHardwareManager,
+                       '_get_system_lshw_dict', autospec=True,
+                       return_value={'id': 'host'})
+    @mock.patch.object(netutils, 'get_hostname', autospec=True)
+    def test_list_hardware_info(self, mocked_get_hostname, mocked_lshw):
         self.hardware.list_network_interfaces = mock.Mock()
         self.hardware.list_network_interfaces.return_value = [
             hardware.NetworkInterface('eth0', '00:0c:29:8c:11:b1'),
             hardware.NetworkInterface('eth1', '00:0c:29:8c:11:b2'),
         ]
 
         self.hardware.get_cpus = mock.Mock()
@@ -1521,14 +1035,15 @@
         self.assertEqual(self.hardware.list_block_devices(),
                          hardware_info['disks'])
         self.assertEqual(self.hardware.list_network_interfaces(),
                          hardware_info['interfaces'])
         self.assertEqual(self.hardware.get_boot_info(),
                          hardware_info['boot'])
         self.assertEqual('mock_hostname', hardware_info['hostname'])
+        mocked_lshw.assert_called_once_with(self.hardware)
 
     @mock.patch.object(hardware, 'list_all_block_devices', autospec=True)
     def test_list_block_devices(self, list_mock):
         device = hardware.BlockDevice('/dev/hdaa', 'small', 65535, False)
         list_mock.return_value = [device]
         devices = self.hardware.list_block_devices()
 
@@ -5243,30 +4758,40 @@
     @mock.patch.object(il_utils, 'execute', autospec=True)
     def test_get_system_vendor_info(self, mocked_execute):
         mocked_execute.return_value = hws.LSHW_JSON_OUTPUT_V1
         vendor_info = self.hardware.get_system_vendor_info()
         self.assertEqual('ABC123 (GENERIC_SERVER)', vendor_info.product_name)
         self.assertEqual('1234567', vendor_info.serial_number)
         self.assertEqual('GENERIC', vendor_info.manufacturer)
+        # This sample does not have firmware information
+        self.assertEqual('', vendor_info.firmware.vendor)
+        self.assertEqual('', vendor_info.firmware.build_date)
+        self.assertEqual('', vendor_info.firmware.version)
 
     @mock.patch.object(il_utils, 'execute', autospec=True)
     def test_get_system_vendor_info_lshw_list(self, mocked_execute):
         mocked_execute.return_value = (f"[{hws.LSHW_JSON_OUTPUT_V2[0]}]", "")
         vendor_info = self.hardware.get_system_vendor_info()
         self.assertEqual('ABCD', vendor_info.product_name)
         self.assertEqual('1234', vendor_info.serial_number)
         self.assertEqual('ABCD', vendor_info.manufacturer)
+        self.assertEqual('BIOSVNDR', vendor_info.firmware.vendor)
+        self.assertEqual('03/30/2023', vendor_info.firmware.build_date)
+        self.assertEqual('1.2.3', vendor_info.firmware.version)
 
     @mock.patch.object(il_utils, 'execute', autospec=True)
     def test_get_system_vendor_info_failure(self, mocked_execute):
         mocked_execute.side_effect = processutils.ProcessExecutionError()
         vendor_info = self.hardware.get_system_vendor_info()
         self.assertEqual('', vendor_info.product_name)
         self.assertEqual('', vendor_info.serial_number)
         self.assertEqual('', vendor_info.manufacturer)
+        self.assertEqual('', vendor_info.firmware.vendor)
+        self.assertEqual('', vendor_info.firmware.build_date)
+        self.assertEqual('', vendor_info.firmware.version)
 
     @mock.patch.object(utils, 'get_agent_params',
                        lambda: {'BOOTIF': 'boot:if'})
     @mock.patch.object(os.path, 'isdir', autospec=True)
     def test_get_boot_info_pxe_interface(self, mocked_isdir):
         mocked_isdir.return_value = False
         result = self.hardware.get_boot_info()
@@ -5963,7 +5488,432 @@
 
         io_dict = {}
         file_list = []
         self.hardware.collect_system_logs(io_dict, file_list)
 
         self.assertEqual(commands, expected)
         self.assertGreaterEqual(len(io_dict), len(expected))
+
+
+@mock.patch.object(hardware.GenericHardwareManager, '_get_system_lshw_dict',
+                   autospec=True, return_value={'id': 'host'})
+@mock.patch.object(hardware, 'get_managers', autospec=True,
+                   return_value=[hardware.GenericHardwareManager()])
+@mock.patch('netifaces.ifaddresses', autospec=True)
+@mock.patch('os.listdir', autospec=True)
+@mock.patch('os.path.exists', autospec=True)
+@mock.patch('builtins.open', autospec=True)
+@mock.patch.object(il_utils, 'execute', autospec=True)
+@mock.patch.object(netutils, 'get_mac_addr', autospec=True)
+@mock.patch.object(netutils, 'interface_has_carrier', autospec=True)
+class TestListNetworkInterfaces(base.IronicAgentTest):
+    def setUp(self):
+        super().setUp()
+        self.hardware = hardware.GenericHardwareManager()
+
+    def test_list_network_interfaces(self,
+                                     mock_has_carrier,
+                                     mock_get_mac,
+                                     mocked_execute,
+                                     mocked_open,
+                                     mocked_exists,
+                                     mocked_listdir,
+                                     mocked_ifaddresses,
+                                     mockedget_managers,
+                                     mocked_lshw):
+        mocked_lshw.return_value = json.loads(hws.LSHW_JSON_OUTPUT_V2[0])
+        mocked_listdir.return_value = ['lo', 'eth0', 'foobar']
+        mocked_exists.side_effect = [False, False, True, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_execute.return_value = ('em0\n', '')
+        mock_has_carrier.return_value = True
+        mock_get_mac.side_effect = [
+            '00:0c:29:8c:11:b1',
+            None,
+        ]
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(1, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        self.assertIsNone(interfaces[0].lldp)
+        self.assertTrue(interfaces[0].has_carrier)
+        self.assertEqual('em0', interfaces[0].biosdevname)
+        self.assertEqual(1000, interfaces[0].speed_mbps)
+
+    def test_list_network_interfaces_with_biosdevname(self,
+                                                      mock_has_carrier,
+                                                      mock_get_mac,
+                                                      mocked_execute,
+                                                      mocked_open,
+                                                      mocked_exists,
+                                                      mocked_listdir,
+                                                      mocked_ifaddresses,
+                                                      mockedget_managers,
+                                                      mocked_lshw):
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_execute.return_value = ('em0\n', '')
+        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
+        mock_has_carrier.return_value = True
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(1, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        self.assertIsNone(interfaces[0].lldp)
+        self.assertTrue(interfaces[0].has_carrier)
+        self.assertEqual('em0', interfaces[0].biosdevname)
+        self.assertIsNone(interfaces[0].speed_mbps)
+
+    @mock.patch.object(netutils, 'get_lldp_info', autospec=True)
+    def test_list_network_interfaces_with_lldp(self,
+                                               mocked_lldp_info,
+                                               mock_has_carrier,
+                                               mock_get_mac,
+                                               mocked_execute,
+                                               mocked_open,
+                                               mocked_exists,
+                                               mocked_listdir,
+                                               mocked_ifaddresses,
+                                               mockedget_managers,
+                                               mocked_lshw):
+        CONF.set_override('collect_lldp', True)
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_lldp_info.return_value = {'eth0': [
+            (0, b''),
+            (1, b'\x04\x88Z\x92\xecTY'),
+            (2, b'\x05Ethernet1/18'),
+            (3, b'\x00x')]
+        }
+        mock_has_carrier.return_value = True
+        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
+        mocked_execute.return_value = ('em0\n', '')
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(1, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        expected_lldp_info = [
+            (0, ''),
+            (1, '04885a92ec5459'),
+            (2, '0545746865726e6574312f3138'),
+            (3, '0078'),
+        ]
+        self.assertEqual(expected_lldp_info, interfaces[0].lldp)
+        self.assertTrue(interfaces[0].has_carrier)
+        self.assertEqual('em0', interfaces[0].biosdevname)
+
+    @mock.patch.object(netutils, 'get_lldp_info', autospec=True)
+    def test_list_network_interfaces_with_lldp_error(
+            self, mocked_lldp_info, mock_has_carrier, mock_get_mac,
+            mocked_execute, mocked_open, mocked_exists, mocked_listdir,
+            mocked_ifaddresses, mockedget_managers, mocked_lshw):
+        CONF.set_override('collect_lldp', True)
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_lldp_info.side_effect = Exception('Boom!')
+        mocked_execute.return_value = ('em0\n', '')
+        mock_has_carrier.return_value = True
+        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(1, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        self.assertIsNone(interfaces[0].lldp)
+        self.assertTrue(interfaces[0].has_carrier)
+        self.assertEqual('em0', interfaces[0].biosdevname)
+
+    def test_list_network_interfaces_no_carrier(self,
+                                                mock_has_carrier,
+                                                mock_get_mac,
+                                                mocked_execute,
+                                                mocked_open,
+                                                mocked_exists,
+                                                mocked_listdir,
+                                                mocked_ifaddresses,
+                                                mockedget_managers,
+                                                mocked_lshw):
+
+        mockedget_managers.return_value = [hardware.GenericHardwareManager()]
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = [OSError('boom')]
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_execute.return_value = ('em0\n', '')
+        mock_has_carrier.return_value = False
+        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(1, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        self.assertFalse(interfaces[0].has_carrier)
+        self.assertIsNone(interfaces[0].vendor)
+        self.assertEqual('em0', interfaces[0].biosdevname)
+
+    def test_list_network_interfaces_with_vendor_info(self,
+                                                      mock_has_carrier,
+                                                      mock_get_mac,
+                                                      mocked_execute,
+                                                      mocked_open,
+                                                      mocked_exists,
+                                                      mocked_listdir,
+                                                      mocked_ifaddresses,
+                                                      mockedget_managers,
+                                                      mocked_lshw):
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        mac = '00:0c:29:8c:11:b1'
+        read_mock.side_effect = ['0x15b3\n', '0x1014\n']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_execute.return_value = ('em0\n', '')
+        mock_has_carrier.return_value = True
+        mock_get_mac.return_value = mac
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(1, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual(mac, interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        self.assertTrue(interfaces[0].has_carrier)
+        self.assertEqual('0x15b3', interfaces[0].vendor)
+        self.assertEqual('0x1014', interfaces[0].product)
+        self.assertEqual('em0', interfaces[0].biosdevname)
+
+    def test_list_network_interfaces_with_bond(self,
+                                               mock_has_carrier,
+                                               mock_get_mac,
+                                               mocked_execute,
+                                               mocked_open,
+                                               mocked_exists,
+                                               mocked_listdir,
+                                               mocked_ifaddresses,
+                                               mockedget_managers,
+                                               mocked_lshw):
+        mocked_listdir.return_value = ['lo', 'bond0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_execute.return_value = ('\n', '')
+        mock_has_carrier.return_value = True
+        mock_get_mac.side_effect = [
+            '00:0c:29:8c:11:b1',
+            None,
+        ]
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(1, len(interfaces))
+        self.assertEqual('bond0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        self.assertIsNone(interfaces[0].lldp)
+        self.assertTrue(interfaces[0].has_carrier)
+        self.assertEqual('', interfaces[0].biosdevname)
+
+    def test_list_network_vlan_interfaces(self,
+                                          mock_has_carrier,
+                                          mock_get_mac,
+                                          mocked_execute,
+                                          mocked_open,
+                                          mocked_exists,
+                                          mocked_listdir,
+                                          mocked_ifaddresses,
+                                          mockedget_managers,
+                                          mocked_lshw):
+        CONF.set_override('enable_vlan_interfaces', 'eth0.100')
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_execute.return_value = ('em0\n', '')
+        mock_get_mac.mock_has_carrier = True
+        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(2, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        self.assertEqual('192.168.1.2', interfaces[0].ipv4_address)
+        self.assertEqual('fd00::101', interfaces[0].ipv6_address)
+        self.assertIsNone(interfaces[0].lldp)
+        self.assertEqual('eth0.100', interfaces[1].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[1].mac_address)
+        self.assertIsNone(interfaces[1].lldp)
+
+    @mock.patch.object(netutils, 'get_lldp_info', autospec=True)
+    def test_list_network_vlan_interfaces_using_lldp(self,
+                                                     mocked_lldp_info,
+                                                     mock_has_carrier,
+                                                     mock_get_mac,
+                                                     mocked_execute,
+                                                     mocked_open,
+                                                     mocked_exists,
+                                                     mocked_listdir,
+                                                     mocked_ifaddresses,
+                                                     mockedget_managers,
+                                                     mocked_lshw):
+        CONF.set_override('collect_lldp', True)
+        CONF.set_override('enable_vlan_interfaces', 'eth0')
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_execute.return_value = ('em0\n', '')
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_lldp_info.return_value = {'eth0': [
+            (0, b''),
+            (127, b'\x00\x80\xc2\x03\x00d\x08vlan-100'),
+            (127, b'\x00\x80\xc2\x03\x00e\x08vlan-101')]
+        }
+        mock_has_carrier.return_value = True
+        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(3, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[0].mac_address)
+        expected_lldp_info = [
+            (0, ''),
+            (127, "0080c203006408766c616e2d313030"),
+            (127, "0080c203006508766c616e2d313031")
+        ]
+        self.assertEqual(expected_lldp_info, interfaces[0].lldp)
+        self.assertEqual('eth0.100', interfaces[1].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[1].mac_address)
+        self.assertIsNone(interfaces[1].lldp)
+        self.assertEqual('eth0.101', interfaces[2].name)
+        self.assertEqual('00:0c:29:8c:11:b1', interfaces[2].mac_address)
+        self.assertIsNone(interfaces[2].lldp)
+
+    @mock.patch.object(netutils, 'LOG', autospec=True)
+    def test_list_network_vlan_invalid_int(self,
+                                           mocked_log,
+                                           mock_has_carrier,
+                                           mock_get_mac,
+                                           mocked_execute,
+                                           mocked_open,
+                                           mocked_exists,
+                                           mocked_listdir,
+                                           mocked_ifaddresses,
+                                           mockedget_managers,
+                                           mocked_lshw):
+        CONF.set_override('collect_lldp', True)
+        CONF.set_override('enable_vlan_interfaces', 'enp0s1')
+        mocked_listdir.return_value = ['lo', 'eth0']
+        mocked_exists.side_effect = [False, False, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_ifaddresses.return_value = {
+            netifaces.AF_INET: [{'addr': '192.168.1.2'}],
+            netifaces.AF_INET6: [{'addr': 'fd00::101'}]
+        }
+        mocked_execute.return_value = ('em0\n', '')
+        mock_get_mac.mock_has_carrier = True
+        mock_get_mac.return_value = '00:0c:29:8c:11:b1'
+
+        self.hardware.list_network_interfaces()
+        mocked_log.warning.assert_called_once_with(
+            'Provided interface name %s was not found', 'enp0s1')
+
+    @mock.patch.object(netutils, 'get_lldp_info', autospec=True)
+    def test_list_network_vlan_interfaces_using_lldp_all(self,
+                                                         mocked_lldp_info,
+                                                         mock_has_carrier,
+                                                         mock_get_mac,
+                                                         mocked_execute,
+                                                         mocked_open,
+                                                         mocked_exists,
+                                                         mocked_listdir,
+                                                         mocked_ifaddresses,
+                                                         mockedget_managers,
+                                                         mocked_lshw):
+        CONF.set_override('collect_lldp', True)
+        CONF.set_override('enable_vlan_interfaces', 'all')
+        mocked_listdir.return_value = ['lo', 'eth0', 'eth1']
+        mocked_execute.return_value = ('em0\n', '')
+        mocked_exists.side_effect = [False, False, True, True]
+        mocked_open.return_value.__enter__ = lambda s: s
+        mocked_open.return_value.__exit__ = mock.Mock()
+        read_mock = mocked_open.return_value.read
+        read_mock.side_effect = ['1']
+        mocked_lldp_info.return_value = {'eth0': [
+            (0, b''),
+            (127, b'\x00\x80\xc2\x03\x00d\x08vlan-100'),
+            (127, b'\x00\x80\xc2\x03\x00e\x08vlan-101')],
+            'eth1': [
+            (0, b''),
+            (127, b'\x00\x80\xc2\x03\x00f\x08vlan-102'),
+            (127, b'\x00\x80\xc2\x03\x00g\x08vlan-103')]
+        }
+
+        interfaces = self.hardware.list_network_interfaces()
+        self.assertEqual(6, len(interfaces))
+        self.assertEqual('eth0', interfaces[0].name)
+        self.assertEqual('eth1', interfaces[1].name)
+        self.assertEqual('eth0.100', interfaces[2].name)
+        self.assertEqual('eth0.101', interfaces[3].name)
+        self.assertEqual('eth1.102', interfaces[4].name)
+        self.assertEqual('eth1.103', interfaces[5].name)
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_inject_files.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_inject_files.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_inspector.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_ironic_api_client.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_ironic_api_client.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_multi_hardware.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_multi_hardware.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_multi_hardware_clean_steps.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_netutils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_netutils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_numa_inspector.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_numa_inspector.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_partition_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_partition_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_raid_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_raid_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_tls_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_tls_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tests/unit/test_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/tls_utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/tls_utils.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/utils.py` & `ironic-python-agent-9.5.0/ironic_python_agent/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -913,7 +913,34 @@
         LOG.warning("Couldn't re-read the partition table "
                     "on device %s", device)
     try:
         execute('udevadm', 'settle')
     except processutils.ProcessExecutionError as e:
         LOG.warning('Something went wrong when waiting for udev '
                     'to settle. Error: %s', e)
+
+
+def _lshw_matches(item, by_id, fields):
+    lshw_id = item.get('id', '')
+    if isinstance(by_id, re.Pattern):
+        if by_id.match(lshw_id) is None:
+            return False
+    elif by_id is not None and by_id != lshw_id:
+        return False
+
+    for key, value in fields.items():
+        if item.get(key) != value:
+            return False
+
+    return True
+
+
+def find_in_lshw(lshw, by_id=None, by_class=None, recursive=False, **fields):
+    """Yield all suitable records from lshw."""
+    # Cannot really pass class=... in Python
+    if by_class is not None:
+        fields['class'] = by_class
+    for child in lshw.get('children', ()):
+        if _lshw_matches(child, by_id, fields):
+            yield child
+        if recursive:
+            yield from find_in_lshw(child, by_id, recursive=True, **fields)
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent/version.py` & `ironic-python-agent-9.5.0/ironic_python_agent/version.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent.egg-info/PKG-INFO` & `ironic-python-agent-9.5.0/ironic_python_agent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ironic-python-agent
-Version: 9.4.0
+Version: 9.5.0
 Summary: Ironic Python Agent Ramdisk
 Home-page: https://docs.openstack.org/ironic-python-agent/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Description: ===================
         Ironic Python Agent
@@ -43,32 +43,32 @@
         
         This is covered in the `Deploying Ironic with DevStack <https://docs.openstack.org/ironic/latest/contributor/dev-quickstart.html#deploying-ironic-with-devstack>`_
         section of the Ironic dev-quickstart guide.
         
         
         Project Resources
         =================
-        Project status, features, and bugs are tracked on StoryBoard:
+        Project bugs are tracked on Launchpad:
         
-          https://storyboard.openstack.org/#!/project/947
+          https://bugs.launchpad.net/ironic-python-agent/+bugs
         
         Developer documentation can be found here:
         
           https://docs.openstack.org/ironic-python-agent/latest/
         
         Release notes for the project are available at:
         
           https://docs.openstack.org/releasenotes/ironic-python-agent/
         
         Source code repository for the project is located at:
         
           https://opendev.org/openstack/ironic-python-agent/
         
         IRC channel:
-            #openstack-ironic
+            #openstack-ironic on irc.oftc.net
         
         To contribute, start here: `Openstack: How to
         contribute <https://docs.openstack.org/infra/manual/developers.html>`_.
         
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent.egg-info/SOURCES.txt` & `ironic-python-agent-9.5.0/ironic_python_agent.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml
 releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml
 releasenotes/notes/auto-tls-b52b873663f35618.yaml
 releasenotes/notes/avoid-grub2-using-efibootmgr-bd27c0978d1cf71b.yaml
 releasenotes/notes/bindmount-run-4c6a31d3ee4e0ed6.yaml
 releasenotes/notes/block-device-hctl-e81573812be3d469.yaml
 releasenotes/notes/bmc-mac-introspection-e4c2e203d8529710.yaml
+releasenotes/notes/bmo-extra-147559c8d1776e8c.yaml
 releasenotes/notes/boot-info-f18336ada089f6dd.yaml
 releasenotes/notes/bootloader-ignored-uefi-mode-8578a009d5b5be62.yaml
 releasenotes/notes/bug-2010123-d4c38d8f6606d0e0.yaml
 releasenotes/notes/build-tinyipa-with-python3-d4a64aa18f970968.yaml
 releasenotes/notes/build-tinyipa-with-tinycore8-b39d0415b1c25f6b.yaml
 releasenotes/notes/bumpsipalookupattempts-29de7c949aaf6556.yaml
 releasenotes/notes/capture-early-logging-0f3fa58d75656117.yaml
@@ -203,14 +204,15 @@
 releasenotes/notes/correction-failure-output-when-downloading-image-39f93838d1ed2928.yaml
 releasenotes/notes/cpu-flags-e3cec7e5cba069ef.yaml
 releasenotes/notes/create_raids_with_volume_name-93e0bb59ef210fe4.yaml
 releasenotes/notes/de-duplicate-by-label-baa090c5b1bff992.yaml
 releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml
 releasenotes/notes/detect-endianness-f53a6c4571aba3fe.yaml
 releasenotes/notes/device-hints-from-node-object-9a689f5a4175a1a6.yaml
+releasenotes/notes/disable-md5-image-checksum-7def176928d36e75.yaml
 releasenotes/notes/discover-ipv6-bmc-address-b3b357ff6c5d822c.yaml
 releasenotes/notes/disk-label-fix-536897e41a4d817f.yaml
 releasenotes/notes/disk-wait-2e0e85e0947f80e9.yaml
 releasenotes/notes/drop-python2-2006fd8a4a6de56d.yaml
 releasenotes/notes/efi-partuuid-5fe933a462eeede1.yaml
 releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml
 releasenotes/notes/enable-skipping-disks-0c4c8b72231715a1.yaml
@@ -222,14 +224,15 @@
 releasenotes/notes/executes-gpt-partition-fix-b6156cc16da00dfc.yaml
 releasenotes/notes/extend-pci-metric-5482284d6a9fe765.yaml
 releasenotes/notes/extend-retry-timeout-30c930a33d97c193.yaml
 releasenotes/notes/fail_ipa_start_if_ironic_api_invalid-7b78fcaba2141cc5.yaml
 releasenotes/notes/fallback-to-findfs-59abde55221e1e84.yaml
 releasenotes/notes/fasttrack-stale-cache-fd93b56a955c7ab1.yaml
 releasenotes/notes/feature-2010228-cf3a59b88f07c3a7.yaml
+releasenotes/notes/fetc-checksum-support-additional-format-4b29c5cdaa6b8d16.yaml
 releasenotes/notes/findbonds-733c7c91a5665b05.yaml
 releasenotes/notes/fix-agent-determination-of-partition-table-type-3c78bf78266e8cef.yaml
 releasenotes/notes/fix-agent-unable-to-stop-py3-6c210793476968d1.yaml
 releasenotes/notes/fix-auxillarly-node-lookup-argument-83d3f717c039e454.yaml
 releasenotes/notes/fix-bmc-ip-detection-for-coreos-483be0286593e393.yaml
 releasenotes/notes/fix-boot-mode-for-partition-images-f96cf2b3c27b6533.yaml
 releasenotes/notes/fix-bootloader-install-with-mdraid-0a254035df9d0bed.yaml
@@ -253,14 +256,15 @@
 releasenotes/notes/fix-uefi-boot-entry-creation-for-aarch64-2b143c5bf189c2f6.yaml
 releasenotes/notes/fix-vfd-mount-for-capitalized-device-name-db7f519e900f4e22.yaml
 releasenotes/notes/fix_chronyd_time_sync-626a14b66ca37677.yaml
 releasenotes/notes/fix_efi_uuid_fstab-f2edbee9bfbac64a.yaml
 releasenotes/notes/fix_partition_cleanup-46491861c930db12.yaml
 releasenotes/notes/fixes-agent-lookup-retries-1b4bb90b8e783aca.yaml
 releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml
+releasenotes/notes/fixes-efibootmgr-character-encoding-19e531ba694824c1.yaml
 releasenotes/notes/fixes-error-handling-of-efibootmgr-not-present-in-ramdisk-f11b4241edcf0e81.yaml
 releasenotes/notes/get-holder-disks-with-nvme-7d5fa75df2fd5904.yaml
 releasenotes/notes/get-physical-memory-535a32362bcdf83a.yaml
 releasenotes/notes/get_md_components_by_uuid-7f08d423ea9e7c94.yaml
 releasenotes/notes/handle-configdrive-large-disks-3517e9fcf16c7f39.yaml
 releasenotes/notes/handle-fd0-devices-3d1f31c3b34819e8.yaml
 releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml
@@ -288,14 +292,15 @@
 releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml
 releasenotes/notes/let_crypt_generate_the_salt-99876591325275a1.yaml
 releasenotes/notes/lib-exc-41ee122eb4a04bc4.yaml
 releasenotes/notes/limit-qemu-img-malloc-arena-025ed84115481eae.yaml
 releasenotes/notes/limit-qemu-img-ram-usage-d7b7a16ac5e9c917.yaml
 releasenotes/notes/lldp-error-handling-5b6576b378ef9c3a.yaml
 releasenotes/notes/lldp-loop-fdfa584caf33d847.yaml
+releasenotes/notes/lldp-raw-a09174cb930bca97.yaml
 releasenotes/notes/log-file-7aaaf31693ddc617.yaml
 releasenotes/notes/logs-collector-non-ascii-010339bf256443c8.yaml
 releasenotes/notes/lsblk-all-956c1df808a169bf.yaml
 releasenotes/notes/lshw-cb89894be057bdc9.yaml
 releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml
 releasenotes/notes/lshw-no-memory-bank-size-05ea71987362986e.yaml
 releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml
@@ -305,14 +310,15 @@
 releasenotes/notes/mdns-e020484e64d76edb.yaml
 releasenotes/notes/min-ironic-ocata-dff80e567783e87c.yaml
 releasenotes/notes/move_swraid_to_efibootmgr-d87c1bfde1661fb5.yaml
 releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml
 releasenotes/notes/multipath-serial-615fc925984abbf7.yaml
 releasenotes/notes/multiple-lan-channels-ee32d80150f990bf.yaml
 releasenotes/notes/name-root-device-hints-0cfc8c90d03c8bf0.yaml
+releasenotes/notes/net-speed-8854901e2051bb79.yaml
 releasenotes/notes/new-agent-api-afbe7391493749be.yaml
 releasenotes/notes/new-sync-command-6f5fa55df2fd5903.yaml
 releasenotes/notes/no-bash-for-grub-c38369af8cc7cf26.yaml
 releasenotes/notes/no-coreos-3345cc69009dead9.yaml
 releasenotes/notes/no-iscsi-fd21808edbea5ac2.yaml
 releasenotes/notes/no-link-local-2e861978c5c7bf30.yaml
 releasenotes/notes/no-mac-54616606ee6b844d.yaml
@@ -388,14 +394,15 @@
 releasenotes/notes/use-latest-coreos-87f826d26b46548d.yaml
 releasenotes/notes/use-system-random-00b0721c8ebd0c5a.yaml
 releasenotes/notes/vmedia-copy-6a58f3183b166c42.yaml
 releasenotes/notes/wait-for-interfaces-before-lookup-9bf38852b2f176a1.yaml
 releasenotes/notes/wait-root-device-504b517c3aec73e2.yaml
 releasenotes/notes/whole-disk-grub-0b1b8b9c44e31d28.yaml
 releasenotes/notes/zero-size-78d3be2ac8fd59c2.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/liberty.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
```

### Comparing `ironic-python-agent-9.4.0/ironic_python_agent.egg-info/entry_points.txt` & `ironic-python-agent-9.5.0/ironic_python_agent.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 generic = ironic_python_agent.hardware:GenericHardwareManager
 mlnx = ironic_python_agent.hardware_managers.mlnx:MellanoxDeviceHardwareManager
 
 [ironic_python_agent.inspector.collectors]
 default = ironic_python_agent.inspector:collect_default
 dmi-decode = ironic_python_agent.dmi_inspector:collect_dmidecode_info
 extra-hardware = ironic_python_agent.inspector:collect_extra_hardware
+lldp = ironic_python_agent.inspector:collect_lldp
 logs = ironic_python_agent.inspector:collect_logs
 numa-topology = ironic_python_agent.numa_inspector:collect_numa_topology_info
 pci-devices = ironic_python_agent.inspector:collect_pci_devices_info
 
 [oslo.config.opts]
 ironic-python-agent = ironic_python_agent.config:list_opts
```

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/Collect_NIC_name_given_by_BIOS-657c68c0ae16365b.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/add-vlan-interfaces-cdfeb39d0f3d444d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/add_burnin_dynamic_network_pairing-33e398255050eb98.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/adds-smartctl-ata-check-to-secure-erase-caebba4f25821575.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/allows-bootloader-install-failure-to-be-ignored-b99667b13afa9759.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/ataraid_does_not_appear_as_disk-8a260e66b3496bf6.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/attempts-ata-disk-unlock-897d76c494ec2976.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/check-virtual-media-devices-a9b1f54c3fe7884d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/configdrive-partuuid-3259cfb7428c1483.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/deprecate-coreos-8b01bcf796c0dc54.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/enable-cleaning-fallback-57e8c9aa2f24e63d.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/fix-iscsi-teardown-handling-0df2345318d3c843.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/fixes-centos-fedora-grub2-mkconfig-hang-fe22cde231994044.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/handle-partuuid-for-fstab-e0aadea20a056982.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/handle-ssl-063a91fb7bdcf9b9.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/ignore-grub-efi-fail-dcf7eb07f61f4388.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/jitter-for-inspection-command-5a226927757a0308.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/lshw-for-memory-and-system-info-35c69da067c72b36.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/manual-introspection-b04b5c25f5e004ac.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/multipath-handling-00a5b412d2cf2e4e.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/prevent-deletion-of-shared-disk-filesystems-4c17c7666d2fe3bc.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/softraid-bootable-with-uefi-aa22e6cbaf1ea747.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/softraid-partitioning-refactor-104b817c3bdc73e3.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/stream-raw-images-d2e245aaed991d86.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/support-bootloader-csv-file-use-c815b520c600cd98.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml` & `ironic-python-agent-9.5.0/releasenotes/notes/support-lldp-in-inventory-4ab6e45ccd35dace.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/releasenotes/source/conf.py` & `ironic-python-agent-9.5.0/releasenotes/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'openstackdocs'
 
 # openstackdocstheme options
 openstackdocs_repo_name = 'openstack/ironic-python-agent'
 openstackdocs_auto_name = False
-openstackdocs_use_storyboard = True
+openstackdocs_use_storyboard = False
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
```

### Comparing `ironic-python-agent-9.4.0/requirements.txt` & `ironic-python-agent-9.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/setup.cfg` & `ironic-python-agent-9.5.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 ironic_python_agent.inspector.collectors = 
 	default = ironic_python_agent.inspector:collect_default
 	logs = ironic_python_agent.inspector:collect_logs
 	extra-hardware = ironic_python_agent.inspector:collect_extra_hardware
 	pci-devices = ironic_python_agent.inspector:collect_pci_devices_info
 	numa-topology = ironic_python_agent.numa_inspector:collect_numa_topology_info
 	dmi-decode = ironic_python_agent.dmi_inspector:collect_dmidecode_info
+	lldp = ironic_python_agent.inspector:collect_lldp
 
 [pbr]
 autodoc_index_modules = True
 api_doc_dir = contributor/api
 
 [egg_info]
 tag_build =
```

### Comparing `ironic-python-agent-9.4.0/setup.py` & `ironic-python-agent-9.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/tools/bandit.yml` & `ironic-python-agent-9.5.0/tools/bandit.yml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/tools/config/check_uptodate.sh` & `ironic-python-agent-9.5.0/tools/config/check_uptodate.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/tools/run_bashate.sh` & `ironic-python-agent-9.5.0/tools/run_bashate.sh`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/tox.ini` & `ironic-python-agent-9.5.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
   OS_TEST_PATH=./ironic_python_agent/tests/functional
   TEST_PORT=9999
   IPA_WAIT_TRIES=100
 commands = stestr run {posargs}
 
 [testenv:pep8]
 deps =
-    hacking>=4.1.0,<5.0.0 # Apache-2.0
+    hacking~=6.0.0 # Apache-2.0
     bashate>=0.5.1 # Apache-2.0
     flake8-import-order>=0.17.1 # LGPLv3
     pycodestyle>=2.0.0,<3.0.0 # MIT
     doc8>=0.8.1 # Apache-2.0
 allowlist_externals = bash
                       {toxinidir}/tools/run_bashate.sh
 commands =
```

### Comparing `ironic-python-agent-9.4.0/zuul.d/ironic-python-agent-jobs.yaml` & `ironic-python-agent-9.5.0/zuul.d/ironic-python-agent-jobs.yaml`

 * *Files identical despite different names*

### Comparing `ironic-python-agent-9.4.0/zuul.d/project.yaml` & `ironic-python-agent-9.5.0/zuul.d/project.yaml`

 * *Files identical despite different names*

