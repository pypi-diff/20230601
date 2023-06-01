# Comparing `tmp/libvirt-python-9.3.0.tar.gz` & `tmp/libvirt-python-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvirt-python-9.3.0.tar", last modified: Tue May  2 12:18:43 2023, max compression
+gzip compressed data, was "libvirt-python-9.4.0.tar", last modified: Thu Jun  1 09:50:26 2023, max compression
```

## Comparing `libvirt-python-9.3.0.tar` & `libvirt-python-9.4.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/
--rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.3.0/.ctags
--rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.3.0/.dir-locals.el
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.075835 libvirt-python-9.3.0/.github/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.079168 libvirt-python-9.3.0/.github/workflows/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.3.0/.github/workflows/lockdown.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/.gitignore
--rw-rw-r--   0 jirka      (500) jirka      (500)     2693 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/.gitlab-ci.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.3.0/.mailmap
--rw-rw-r--   0 jirka      (500) jirka      (500)     3979 2023-05-02 12:18:42.000000 libvirt-python-9.3.0/AUTHORS
--rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.3.0/AUTHORS.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 jirka      (500) jirka      (500)    18092 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/COPYING
--rw-rw-r--   0 jirka      (500) jirka      (500)    26530 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/COPYING.LESSER
--rw-rw-r--   0 jirka      (500) jirka      (500)   405825 2023-05-02 12:18:42.000000 libvirt-python-9.3.0/ChangeLog
--rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/HACKING
--rw-rw-r--   0 jirka      (500) jirka      (500)     1283 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/MANIFEST
--rw-rw-r--   0 jirka      (500) jirka      (500)     1704 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/MANIFEST.in
--rw-rw-r--   0 jirka      (500) jirka      (500)      260 2016-10-04 07:42:23.000000 libvirt-python-9.3.0/Makefile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1162 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/PKG-INFO
--rw-rw-r--   0 jirka      (500) jirka      (500)     1384 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/README
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.075835 libvirt-python-9.3.0/build/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/build/libvirt_python.egg-info/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2328 2023-05-02 12:18:43.000000 libvirt-python-9.3.0/build/libvirt_python.egg-info/SOURCES.txt
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.079168 libvirt-python-9.3.0/ci/
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/ci/buildenv/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1407 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/centos-stream-8.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      965 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/centos-stream-9.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/debian-10.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/debian-sid.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      798 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/fedora-36.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      798 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/ci/buildenv/fedora-37.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      850 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/fedora-rawhide.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      846 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/buildenv/opensuse-leap-154.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)      852 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/opensuse-tumbleweed.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/ubuntu-2004.sh
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/buildenv/ubuntu-2204.sh
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/ci/containers/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1499 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/centos-stream-8.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/centos-stream-9.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1370 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/debian-10.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1371 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/debian-sid.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/fedora-36.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/fedora-37.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1343 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/fedora-rawhide.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      905 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/containers/opensuse-leap-154.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)      919 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/opensuse-tumbleweed.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/ubuntu-2004.Dockerfile
--rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.3.0/ci/containers/ubuntu-2204.Dockerfile
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/ci/gitlab/
--rw-rw-r--   0 jirka      (500) jirka      (500)     6071 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/build-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     5849 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/builds.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/ci/gitlab/container-templates.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1447 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/containers.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)      938 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab/sanity-checks.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     2754 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/gitlab.yml
--rw-rw-r--   0 jirka      (500) jirka      (500)     1475 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/ci/manifest.yml
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/examples/
--rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/README
--rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/consolecallback.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/dhcpleases.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/dominfo.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domipaddrs.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domrestore.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domsave.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/domstart.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/esxlist.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    35898 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/examples/event-test.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.082502 libvirt-python-9.3.0/examples/guest-vcpus/
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu-daemon.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/nodestats.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/sparsestream.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/examples/topology.py
--rwxrwxr-x   0 jirka      (500) jirka      (500)    70037 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/generator.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-lxc-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-lxc-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.3.0/libvirt-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    31114 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virConnect.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.3.0/libvirt-override-virDomain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virDomainCheckpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virDomainSnapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virNetwork.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virStoragePool.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-override-virStream.py
--rw-rw-r--   0 jirka      (500) jirka      (500)   329516 2023-03-01 10:15:08.000000 libvirt-python-9.3.0/libvirt-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.3.0/libvirt-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2759 2023-05-02 12:18:42.000000 libvirt-python-9.3.0/libvirt-python.spec
--rw-rw-r--   0 jirka      (500) jirka      (500)     2766 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/libvirt-python.spec.in
--rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-qemu-override-api.xml
--rw-rw-r--   0 jirka      (500) jirka      (500)    14037 2023-03-01 10:15:08.000000 libvirt-python-9.3.0/libvirt-qemu-override.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.3.0/libvirt-qemu-override.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16182 2022-07-11 21:25:49.000000 libvirt-python-9.3.0/libvirt-utils.c
--rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/libvirt-utils.h
--rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/libvirtaio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/requirements-test.txt
--rw-rw-r--   0 jirka      (500) jirka      (500)       38 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/setup.cfg
--rwxrwxr-x   0 jirka      (500) jirka      (500)    11863 2023-05-02 11:04:38.000000 libvirt-python-9.3.0/setup.py
-drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-05-02 12:18:43.085835 libvirt-python-9.3.0/tests/
--rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/tests/eventmock.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.3.0/tests/test_aio.py
--rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.3.0/tests/test_api_coverage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_conn.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_domain.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_domain_checkpoint.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_domain_snapshot.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_interface.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_network.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_nodedev.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tests/test_storage.py
--rw-rw-r--   0 jirka      (500) jirka      (500)      114 2022-04-01 10:30:02.000000 libvirt-python-9.3.0/tox.ini
--rw-rw-r--   0 jirka      (500) jirka      (500)    10721 2023-03-01 10:15:08.000000 libvirt-python-9.3.0/typewrappers.c
--rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.3.0/typewrappers.h
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.515809 libvirt-python-9.4.0/
+-rw-rw-r--   0 jirka      (500) jirka      (500)       27 2014-06-19 09:18:44.000000 libvirt-python-9.4.0/.ctags
+-rw-rw-r--   0 jirka      (500) jirka      (500)      171 2014-06-19 09:18:44.000000 libvirt-python-9.4.0/.dir-locals.el
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.502476 libvirt-python-9.4.0/.github/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/.github/workflows/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1486 2021-12-01 09:53:22.000000 libvirt-python-9.4.0/.github/workflows/lockdown.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      100 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/.gitignore
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2693 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/.gitlab-ci.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      554 2016-10-04 07:42:23.000000 libvirt-python-9.4.0/.mailmap
+-rw-rw-r--   0 jirka      (500) jirka      (500)     4008 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/AUTHORS
+-rw-rw-r--   0 jirka      (500) jirka      (500)      236 2014-06-19 09:18:44.000000 libvirt-python-9.4.0/AUTHORS.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1023 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 jirka      (500) jirka      (500)    18092 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/COPYING
+-rw-rw-r--   0 jirka      (500) jirka      (500)    26530 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/COPYING.LESSER
+-rw-rw-r--   0 jirka      (500) jirka      (500)   406729 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/ChangeLog
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1491 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/HACKING
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1283 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/MANIFEST
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1704 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/MANIFEST.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)      260 2016-10-04 07:42:23.000000 libvirt-python-9.4.0/Makefile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1162 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/PKG-INFO
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1384 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/README
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.502476 libvirt-python-9.4.0/build/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/build/libvirt_python.egg-info/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2326 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/build/libvirt_python.egg-info/SOURCES.txt
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/ci/
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/ci/buildenv/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1407 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/centos-stream-8.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      965 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/centos-stream-9.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/debian-10.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/debian-sid.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      798 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/ci/buildenv/fedora-37.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      798 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/buildenv/fedora-38.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      850 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/fedora-rawhide.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      846 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/buildenv/opensuse-leap-15.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)      852 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/opensuse-tumbleweed.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/ubuntu-2004.sh
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/buildenv/ubuntu-2204.sh
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.509142 libvirt-python-9.4.0/ci/containers/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1499 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/centos-stream-8.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1058 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/centos-stream-9.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1370 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/debian-10.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1371 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/debian-sid.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/containers/fedora-37.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1281 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/containers/fedora-38.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1343 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/containers/fedora-rawhide.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      905 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/containers/opensuse-leap-15.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)      919 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/opensuse-tumbleweed.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/ubuntu-2004.Dockerfile
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1368 2022-10-03 09:10:28.000000 libvirt-python-9.4.0/ci/containers/ubuntu-2204.Dockerfile
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/ci/gitlab/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6071 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/gitlab/build-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5844 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/gitlab/builds.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1573 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/ci/gitlab/container-templates.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1445 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/gitlab/containers.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)      938 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/gitlab/sanity-checks.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2754 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/ci/gitlab.yml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1474 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/ci/manifest.yml
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/examples/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1592 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/README
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3300 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/consolecallback.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1663 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/dhcpleases.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2107 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/dominfo.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1568 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domipaddrs.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      690 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domrestore.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)      762 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domsave.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1239 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/domstart.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     5066 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/esxlist.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    35898 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/examples/event-test.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/examples/guest-vcpus/
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3880 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu-daemon.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1588 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     2782 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/nodestats.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     3857 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/sparsestream.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)     1235 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/examples/topology.py
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    70037 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/generator.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      737 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-lxc-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3276 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-lxc-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    59229 2022-06-01 07:30:40.000000 libvirt-python-9.4.0/libvirt-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    31114 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virConnect.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     5628 2023-01-16 10:59:44.000000 libvirt-python-9.4.0/libvirt-override-virDomain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      716 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virDomainCheckpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      702 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virDomainSnapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      381 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virNetwork.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      396 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virStoragePool.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    11453 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-override-virStream.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)   329987 2023-06-01 09:50:22.000000 libvirt-python-9.4.0/libvirt-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10085 2022-05-02 11:37:45.000000 libvirt-python-9.4.0/libvirt-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2759 2023-06-01 09:50:26.000000 libvirt-python-9.4.0/libvirt-python.spec
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2766 2023-05-02 11:04:38.000000 libvirt-python-9.4.0/libvirt-python.spec.in
+-rw-rw-r--   0 jirka      (500) jirka      (500)     1135 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-qemu-override-api.xml
+-rw-rw-r--   0 jirka      (500) jirka      (500)    14037 2023-03-01 10:15:08.000000 libvirt-python-9.4.0/libvirt-qemu-override.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     3452 2022-05-02 11:37:45.000000 libvirt-python-9.4.0/libvirt-qemu-override.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16182 2022-07-11 21:25:49.000000 libvirt-python-9.4.0/libvirt-utils.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)    13274 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/libvirt-utils.h
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16957 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/libvirtaio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)       10 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/requirements-test.txt
+-rw-rw-r--   0 jirka      (500) jirka      (500)       38 2023-06-01 09:50:26.515809 libvirt-python-9.4.0/setup.cfg
+-rwxrwxr-x   0 jirka      (500) jirka      (500)    11863 2023-05-17 07:45:20.000000 libvirt-python-9.4.0/setup.py
+drwxrwxr-x   0 jirka      (500) jirka      (500)        0 2023-06-01 09:50:26.512476 libvirt-python-9.4.0/tests/
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2774 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/tests/eventmock.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     6016 2022-07-01 09:27:33.000000 libvirt-python-9.4.0/tests/test_aio.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)    16198 2022-05-02 11:37:45.000000 libvirt-python-9.4.0/tests/test_api_coverage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)     2884 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_conn.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      758 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_domain.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      552 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_domain_checkpoint.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      398 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_domain_snapshot.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      367 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_interface.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      363 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_network.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      380 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_nodedev.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      600 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tests/test_storage.py
+-rw-rw-r--   0 jirka      (500) jirka      (500)      114 2022-04-01 10:30:02.000000 libvirt-python-9.4.0/tox.ini
+-rw-rw-r--   0 jirka      (500) jirka      (500)    10721 2023-03-01 10:15:08.000000 libvirt-python-9.4.0/typewrappers.c
+-rw-rw-r--   0 jirka      (500) jirka      (500)     9234 2022-09-20 16:28:07.000000 libvirt-python-9.4.0/typewrappers.h
```

### Comparing `libvirt-python-9.3.0/.github/workflows/lockdown.yml` & `libvirt-python-9.4.0/.github/workflows/lockdown.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/.gitlab-ci.yml` & `libvirt-python-9.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/.mailmap` & `libvirt-python-9.4.0/.mailmap`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/AUTHORS` & `libvirt-python-9.4.0/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
    Erik Skultety <eskultety@ridgehead.home.lan>
    Federico Simoncelli <fsimonce@redhat.com>
    Giuseppe Scrivano <gscrivan@redhat.com>
    Guan Qiang <hzguanqiang@corp.netease.com>
    Guannan Ren <gren@redhat.com>
    Gui Jianfeng <guijianfeng@cn.fujitsu.com>
    Guido Günther <agx@sigxcpu.org>
+   Han Han <hhan@redhat.com>
    Hu Tao <hutao@cn.fujitsu.com>
    Jason Andryuk <andryuk@aero.org>
    Jim Fehlig <jfehlig@suse.com>
    Jim Meyering <meyering@redhat.com>
    Jiri Denemark <jdenemar@redhat.com>
    John Ferlan <jferlan@redhat.com>
    Jonathon Jongsma <jjongsma@redhat.com>
```

### Comparing `libvirt-python-9.3.0/CONTRIBUTING.rst` & `libvirt-python-9.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/COPYING` & `libvirt-python-9.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/COPYING.LESSER` & `libvirt-python-9.4.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ChangeLog` & `libvirt-python-9.4.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+2023-05-31 Han Han  <hhan@redhat.com>
+    
+    virDomainMigrate3Params: Add missing params
+    Add these missing migrate params:
+    - VIR_MIGRATE_PARAM_DISKS_URI, since libvirt v6.8.0(49186372db)
+    - VIR_MIGRATE_PARAM_TLS_DESTINATION, since libvirt v6.0.0(1b8af37213e)
+    - VIR_MIGRATE_PARAM_COMPRESSION_ZLIB_LEVEL and VIR_MIGRATE_PARAM_COMPRESSION_ZSTD_LEVEL,
+    since libvirt v9.4.0(150ae3e62b9)
+    
+    
+    
+2023-05-03 Erik Skultety  <eskultet@redhat.com>
+    
+    ci: Drop Fedora 36 target
+    
+    
+2023-05-03 Erik Skultety  <eskultet@redhat.com>
+    
+    ci: Add Fedora 38 target
+    
+    
+2023-05-03 Erik Skultety  <eskultet@redhat.com>
+    
+    ci: Replace OpenSUSE Leap 15.4 target with Leap 15 name
+    We now refer to the latest Leap 15.X simply as Leap 15 in lcitool.
+    
+    
+    
+2023-05-02 Jiri Denemark  <jdenemar@redhat.com>
+    
+    Post-release version bump to 9.4.0
+    
+    
 2023-04-26 Daniel P. Berrangé  <berrange@redhat.com>
     
     rpm: convert license to SPDX format
     
     
 2023-04-19 Jiri Denemark  <jdenemar@redhat.com>
```

### Comparing `libvirt-python-9.3.0/HACKING` & `libvirt-python-9.4.0/HACKING`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/MANIFEST` & `libvirt-python-9.4.0/MANIFEST`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/MANIFEST.in` & `libvirt-python-9.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/PKG-INFO` & `libvirt-python-9.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libvirt-python
-Version: 9.3.0
+Version: 9.4.0
 Summary: The libvirt virtualization API python binding
 Home-page: http://www.libvirt.org
 Maintainer: Libvirt Maintainers
 Maintainer-email: libvir-list@redhat.com
 License: LGPLv2+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `libvirt-python-9.3.0/README` & `libvirt-python-9.4.0/README`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/build/libvirt_python.egg-info/SOURCES.txt` & `libvirt-python-9.4.0/build/libvirt_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,29 +43,29 @@
 .github/workflows/lockdown.yml
 ci/gitlab.yml
 ci/manifest.yml
 ci/buildenv/centos-stream-8.sh
 ci/buildenv/centos-stream-9.sh
 ci/buildenv/debian-10.sh
 ci/buildenv/debian-sid.sh
-ci/buildenv/fedora-36.sh
 ci/buildenv/fedora-37.sh
+ci/buildenv/fedora-38.sh
 ci/buildenv/fedora-rawhide.sh
-ci/buildenv/opensuse-leap-154.sh
+ci/buildenv/opensuse-leap-15.sh
 ci/buildenv/opensuse-tumbleweed.sh
 ci/buildenv/ubuntu-2004.sh
 ci/buildenv/ubuntu-2204.sh
 ci/containers/centos-stream-8.Dockerfile
 ci/containers/centos-stream-9.Dockerfile
 ci/containers/debian-10.Dockerfile
 ci/containers/debian-sid.Dockerfile
-ci/containers/fedora-36.Dockerfile
 ci/containers/fedora-37.Dockerfile
+ci/containers/fedora-38.Dockerfile
 ci/containers/fedora-rawhide.Dockerfile
-ci/containers/opensuse-leap-154.Dockerfile
+ci/containers/opensuse-leap-15.Dockerfile
 ci/containers/opensuse-tumbleweed.Dockerfile
 ci/containers/ubuntu-2004.Dockerfile
 ci/containers/ubuntu-2204.Dockerfile
 ci/gitlab/build-templates.yml
 ci/gitlab/builds.yml
 ci/gitlab/container-templates.yml
 ci/gitlab/containers.yml
```

### Comparing `libvirt-python-9.3.0/ci/buildenv/centos-stream-8.sh` & `libvirt-python-9.4.0/ci/buildenv/centos-stream-8.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/centos-stream-9.sh` & `libvirt-python-9.4.0/ci/buildenv/centos-stream-9.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/debian-10.sh` & `libvirt-python-9.4.0/ci/buildenv/debian-10.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/debian-sid.sh` & `libvirt-python-9.4.0/ci/buildenv/debian-sid.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/fedora-36.sh` & `libvirt-python-9.4.0/ci/buildenv/fedora-37.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/fedora-37.sh` & `libvirt-python-9.4.0/ci/buildenv/fedora-38.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/fedora-rawhide.sh` & `libvirt-python-9.4.0/ci/buildenv/fedora-rawhide.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/opensuse-leap-154.sh` & `libvirt-python-9.4.0/ci/buildenv/opensuse-leap-15.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/opensuse-tumbleweed.sh` & `libvirt-python-9.4.0/ci/buildenv/opensuse-tumbleweed.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/ubuntu-2004.sh` & `libvirt-python-9.4.0/ci/buildenv/ubuntu-2004.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/buildenv/ubuntu-2204.sh` & `libvirt-python-9.4.0/ci/buildenv/ubuntu-2204.sh`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/centos-stream-8.Dockerfile` & `libvirt-python-9.4.0/ci/containers/centos-stream-8.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/centos-stream-9.Dockerfile` & `libvirt-python-9.4.0/ci/containers/centos-stream-9.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/debian-10.Dockerfile` & `libvirt-python-9.4.0/ci/containers/debian-10.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/debian-sid.Dockerfile` & `libvirt-python-9.4.0/ci/containers/debian-sid.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/fedora-36.Dockerfile` & `libvirt-python-9.4.0/ci/containers/fedora-38.Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # THIS FILE WAS AUTO-GENERATED
 #
 #  $ lcitool manifest ci/manifest.yml
 #
 # https://gitlab.com/libvirt/libvirt-ci
 
-FROM registry.fedoraproject.org/fedora:36
+FROM registry.fedoraproject.org/fedora:38
 
 RUN dnf install -y nosync && \
     printf '#!/bin/sh\n\
 if test -d /usr/lib64\n\
 then\n\
     export LD_PRELOAD=/usr/lib64/nosync/nosync.so\n\
 else\n\
```

### Comparing `libvirt-python-9.3.0/ci/containers/fedora-37.Dockerfile` & `libvirt-python-9.4.0/ci/containers/fedora-37.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/fedora-rawhide.Dockerfile` & `libvirt-python-9.4.0/ci/containers/fedora-rawhide.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/opensuse-leap-154.Dockerfile` & `libvirt-python-9.4.0/ci/containers/opensuse-leap-15.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/opensuse-tumbleweed.Dockerfile` & `libvirt-python-9.4.0/ci/containers/opensuse-tumbleweed.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/ubuntu-2004.Dockerfile` & `libvirt-python-9.4.0/ci/containers/ubuntu-2004.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/containers/ubuntu-2204.Dockerfile` & `libvirt-python-9.4.0/ci/containers/ubuntu-2204.Dockerfile`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/gitlab/build-templates.yml` & `libvirt-python-9.4.0/ci/gitlab/build-templates.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/gitlab/builds.yml` & `libvirt-python-9.4.0/ci/gitlab/builds.yml`

 * *Files 1% similar despite different names*

```diff
@@ -121,60 +121,60 @@
   allow_failure: true
   variables:
     IMAGE: docker.io/library/debian:sid-slim
     NAME: debian-sid
     PIP_INSTALL: install --break-system-packages
 
 
-x86_64-fedora-36-prebuilt-env:
+x86_64-fedora-37-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
-    - job: x86_64-fedora-36-container
+    - job: x86_64-fedora-37-container
       optional: true
   allow_failure: false
   variables:
-    NAME: fedora-36
+    NAME: fedora-37
   artifacts:
     expire_in: 1 hour
     paths:
       - libvirt-python-rpms
 
-x86_64-fedora-36-local-env:
+x86_64-fedora-37-local-env:
   extends: .native_build_job_local_env
   needs: []
   allow_failure: false
   variables:
-    IMAGE: registry.fedoraproject.org/fedora:36
-    NAME: fedora-36
+    IMAGE: registry.fedoraproject.org/fedora:37
+    NAME: fedora-37
   artifacts:
     expire_in: 1 hour
     paths:
       - libvirt-python-rpms
 
 
-x86_64-fedora-37-prebuilt-env:
+x86_64-fedora-38-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
-    - job: x86_64-fedora-37-container
+    - job: x86_64-fedora-38-container
       optional: true
   allow_failure: false
   variables:
-    NAME: fedora-37
+    NAME: fedora-38
   artifacts:
     expire_in: 1 hour
     paths:
       - libvirt-python-rpms
 
-x86_64-fedora-37-local-env:
+x86_64-fedora-38-local-env:
   extends: .native_build_job_local_env
   needs: []
   allow_failure: false
   variables:
-    IMAGE: registry.fedoraproject.org/fedora:37
-    NAME: fedora-37
+    IMAGE: registry.fedoraproject.org/fedora:38
+    NAME: fedora-38
   artifacts:
     expire_in: 1 hour
     paths:
       - libvirt-python-rpms
 
 
 x86_64-fedora-rawhide-prebuilt-env:
@@ -191,31 +191,31 @@
   needs: []
   allow_failure: true
   variables:
     IMAGE: registry.fedoraproject.org/fedora:rawhide
     NAME: fedora-rawhide
 
 
-x86_64-opensuse-leap-154-prebuilt-env:
+x86_64-opensuse-leap-15-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
-    - job: x86_64-opensuse-leap-154-container
+    - job: x86_64-opensuse-leap-15-container
       optional: true
   allow_failure: false
   variables:
-    NAME: opensuse-leap-154
+    NAME: opensuse-leap-15
     RPM: skip
 
-x86_64-opensuse-leap-154-local-env:
+x86_64-opensuse-leap-15-local-env:
   extends: .native_build_job_local_env
   needs: []
   allow_failure: false
   variables:
     IMAGE: registry.opensuse.org/opensuse/leap:15.4
-    NAME: opensuse-leap-154
+    NAME: opensuse-leap-15
     RPM: skip
 
 
 x86_64-opensuse-tumbleweed-prebuilt-env:
   extends: .native_build_job_prebuilt_env
   needs:
     - job: x86_64-opensuse-tumbleweed-container
```

### Comparing `libvirt-python-9.3.0/ci/gitlab/container-templates.yml` & `libvirt-python-9.4.0/ci/gitlab/container-templates.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/gitlab/containers.yml` & `libvirt-python-9.4.0/ci/gitlab/containers.yml`

 * *Files 3% similar despite different names*

```diff
@@ -31,40 +31,40 @@
 x86_64-debian-sid-container:
   extends: .container_job
   allow_failure: true
   variables:
     NAME: debian-sid
 
 
-x86_64-fedora-36-container:
+x86_64-fedora-37-container:
   extends: .container_job
   allow_failure: false
   variables:
-    NAME: fedora-36
+    NAME: fedora-37
 
 
-x86_64-fedora-37-container:
+x86_64-fedora-38-container:
   extends: .container_job
   allow_failure: false
   variables:
-    NAME: fedora-37
+    NAME: fedora-38
 
 
 x86_64-fedora-rawhide-container:
   extends: .container_job
   allow_failure: true
   variables:
     NAME: fedora-rawhide
 
 
-x86_64-opensuse-leap-154-container:
+x86_64-opensuse-leap-15-container:
   extends: .container_job
   allow_failure: false
   variables:
-    NAME: opensuse-leap-154
+    NAME: opensuse-leap-15
 
 
 x86_64-opensuse-tumbleweed-container:
   extends: .container_job
   allow_failure: true
   variables:
     NAME: opensuse-tumbleweed
```

### Comparing `libvirt-python-9.3.0/ci/gitlab/sanity-checks.yml` & `libvirt-python-9.4.0/ci/gitlab/sanity-checks.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/gitlab.yml` & `libvirt-python-9.4.0/ci/gitlab.yml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/ci/manifest.yml` & `libvirt-python-9.4.0/ci/manifest.yml`

 * *Files 1% similar despite different names*

```diff
@@ -43,36 +43,36 @@
   debian-sid:
     jobs:
       - arch: x86_64
         allow-failure: true
         variables:
           PIP_INSTALL: install --break-system-packages
 
-  fedora-36:
+  fedora-37:
     jobs:
       - arch: x86_64
         artifacts:
           expire_in: 1 hour
           paths:
             - libvirt-python-rpms
 
-  fedora-37:
+  fedora-38:
     jobs:
       - arch: x86_64
         artifacts:
           expire_in: 1 hour
           paths:
             - libvirt-python-rpms
 
   fedora-rawhide:
     jobs:
       - arch: x86_64
         allow-failure: true
 
-  opensuse-leap-154:
+  opensuse-leap-15:
     jobs:
       - arch: x86_64
         variables:
           RPM: skip
 
   opensuse-tumbleweed:
     jobs:
```

### Comparing `libvirt-python-9.3.0/examples/README` & `libvirt-python-9.4.0/examples/README`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/consolecallback.py` & `libvirt-python-9.4.0/examples/consolecallback.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/dhcpleases.py` & `libvirt-python-9.4.0/examples/dhcpleases.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/dominfo.py` & `libvirt-python-9.4.0/examples/dominfo.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/domipaddrs.py` & `libvirt-python-9.4.0/examples/domipaddrs.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/domrestore.py` & `libvirt-python-9.4.0/examples/domrestore.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/domsave.py` & `libvirt-python-9.4.0/examples/domsave.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/domstart.py` & `libvirt-python-9.4.0/examples/domstart.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/esxlist.py` & `libvirt-python-9.4.0/examples/esxlist.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/event-test.py` & `libvirt-python-9.4.0/examples/event-test.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu-daemon.py` & `libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu-daemon.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/guest-vcpus/guest-vcpu.py` & `libvirt-python-9.4.0/examples/guest-vcpus/guest-vcpu.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/nodestats.py` & `libvirt-python-9.4.0/examples/nodestats.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/sparsestream.py` & `libvirt-python-9.4.0/examples/sparsestream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/examples/topology.py` & `libvirt-python-9.4.0/examples/topology.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/generator.py` & `libvirt-python-9.4.0/generator.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-lxc-override-api.xml` & `libvirt-python-9.4.0/libvirt-lxc-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-lxc-override.c` & `libvirt-python-9.4.0/libvirt-lxc-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-override-api.xml` & `libvirt-python-9.4.0/libvirt-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-override-virConnect.py` & `libvirt-python-9.4.0/libvirt-override-virConnect.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-override-virDomain.py` & `libvirt-python-9.4.0/libvirt-override-virDomain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-override-virDomainCheckpoint.py` & `libvirt-python-9.4.0/libvirt-override-virDomainCheckpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-override-virDomainSnapshot.py` & `libvirt-python-9.4.0/libvirt-override-virDomainSnapshot.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-override-virStream.py` & `libvirt-python-9.4.0/libvirt-override-virStream.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-override.c` & `libvirt-python-9.4.0/libvirt-override.c`

 * *Files 0% similar despite different names*

```diff
@@ -8150,14 +8150,26 @@
 # endif
 # ifdef VIR_MIGRATE_PARAM_BANDWIDTH_POSTCOPY
     { VIR_MIGRATE_PARAM_BANDWIDTH_POSTCOPY, VIR_TYPED_PARAM_ULLONG },
 # endif
 # ifdef VIR_MIGRATE_PARAM_PARALLEL_CONNECTIONS
     { VIR_MIGRATE_PARAM_PARALLEL_CONNECTIONS, VIR_TYPED_PARAM_INT },
 # endif
+# ifdef VIR_MIGRATE_PARAM_DISKS_URI
+    { VIR_MIGRATE_PARAM_DISKS_URI, VIR_TYPED_PARAM_STRING },
+#endif
+#ifdef VIR_MIGRATE_PARAM_TLS_DESTINATION
+    { VIR_MIGRATE_PARAM_TLS_DESTINATION, VIR_TYPED_PARAM_STRING },
+#endif
+#ifdef VIR_MIGRATE_PARAM_COMPRESSION_ZLIB_LEVEL
+    { VIR_MIGRATE_PARAM_COMPRESSION_ZLIB_LEVEL, VIR_TYPED_PARAM_INT },
+#endif
+#ifdef VIR_MIGRATE_PARAM_COMPRESSION_ZSTD_LEVEL
+    { VIR_MIGRATE_PARAM_COMPRESSION_ZSTD_LEVEL, VIR_TYPED_PARAM_INT },
+#endif
 };
 
 
 static PyObject *
 libvirt_virDomainMigrate3(PyObject *self ATTRIBUTE_UNUSED,
                           PyObject *args)
 {
```

### Comparing `libvirt-python-9.3.0/libvirt-override.py` & `libvirt-python-9.4.0/libvirt-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-python.spec` & `libvirt-python-9.4.0/libvirt-python.spec`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     %define supported_platform 1
 %else
     %define supported_platform 0
 %endif
 
 Summary: The libvirt virtualization API python3 binding
 Name: libvirt-python
-Version: 9.3.0
+Version: 9.4.0
 Release: 1%{?dist}
 Source0: https://libvirt.org/sources/python/%{name}-%{version}.tar.gz
 Url: https://libvirt.org
 License: LGPL-2.1-or-later
 BuildRequires: libvirt-devel == %{version}
 BuildRequires: python3-devel
 BuildRequires: python3-pytest
```

### Comparing `libvirt-python-9.3.0/libvirt-python.spec.in` & `libvirt-python-9.4.0/libvirt-python.spec.in`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-qemu-override-api.xml` & `libvirt-python-9.4.0/libvirt-qemu-override-api.xml`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-qemu-override.c` & `libvirt-python-9.4.0/libvirt-qemu-override.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-qemu-override.py` & `libvirt-python-9.4.0/libvirt-qemu-override.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-utils.c` & `libvirt-python-9.4.0/libvirt-utils.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirt-utils.h` & `libvirt-python-9.4.0/libvirt-utils.h`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/libvirtaio.py` & `libvirt-python-9.4.0/libvirtaio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/setup.py` & `libvirt-python-9.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
 ##################
 # Invoke setup() #
 ##################
 
 _c_modules, _py_modules = get_module_lists()
 
 setup(name = 'libvirt-python',
-      version = '9.3.0',
+      version = '9.4.0',
       url = 'http://www.libvirt.org',
       maintainer = 'Libvirt Maintainers',
       maintainer_email = 'libvir-list@redhat.com',
       description = 'The libvirt virtualization API python binding',
       long_description =
         '''The libvirt-python package provides a module that permits applications
 written in the Python 3.x programming language to call the interface
```

### Comparing `libvirt-python-9.3.0/tests/eventmock.py` & `libvirt-python-9.4.0/tests/eventmock.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/tests/test_aio.py` & `libvirt-python-9.4.0/tests/test_aio.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/tests/test_api_coverage.py` & `libvirt-python-9.4.0/tests/test_api_coverage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/tests/test_conn.py` & `libvirt-python-9.4.0/tests/test_conn.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/tests/test_domain.py` & `libvirt-python-9.4.0/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/tests/test_domain_checkpoint.py` & `libvirt-python-9.4.0/tests/test_domain_checkpoint.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/tests/test_storage.py` & `libvirt-python-9.4.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/typewrappers.c` & `libvirt-python-9.4.0/typewrappers.c`

 * *Files identical despite different names*

### Comparing `libvirt-python-9.3.0/typewrappers.h` & `libvirt-python-9.4.0/typewrappers.h`

 * *Files identical despite different names*

