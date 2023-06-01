# Comparing `tmp/pyatem-0.8.0.tar.gz` & `tmp/pyatem-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatem-0.8.0.tar", last modified: Fri Sep 16 12:03:46 2022, max compression
+gzip compressed data, was "pyatem-0.9.0.tar", last modified: Thu Jun  1 17:04:01 2023, max compression
```

## Comparing `pyatem-0.8.0.tar` & `pyatem-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,233 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 12:03:46.734415 pyatem-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     7652 2017-09-30 07:16:26.000000 pyatem-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3577 2022-09-16 12:03:46.734415 pyatem-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2994 2022-05-23 16:02:11.000000 pyatem-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 12:03:46.734415 pyatem-0.8.0/pyatem/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-30 01:10:34.000000 pyatem-0.8.0/pyatem/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10698 2022-04-16 00:23:49.000000 pyatem-0.8.0/pyatem/cameracontrol.py
--rw-r--r--   0 root         (0) root         (0)    88194 2022-08-09 22:06:41.000000 pyatem-0.8.0/pyatem/command.py
--rw-r--r--   0 root         (0) root         (0)   108948 2022-08-09 22:06:41.000000 pyatem-0.8.0/pyatem/field.py
--rw-r--r--   0 root         (0) root         (0)    15178 2022-04-16 00:23:49.000000 pyatem-0.8.0/pyatem/hexdump.py
--rw-r--r--   0 root         (0) root         (0)     2063 2022-05-20 11:17:47.000000 pyatem-0.8.0/pyatem/locate.py
--rw-r--r--   0 root         (0) root         (0)     2232 2022-04-16 00:23:49.000000 pyatem-0.8.0/pyatem/macro.py
--rw-r--r--   0 root         (0) root         (0)     5038 2022-04-16 00:23:49.000000 pyatem-0.8.0/pyatem/macrocommand.py
--rw-r--r--   0 root         (0) root         (0)     3417 2022-05-23 18:14:25.000000 pyatem-0.8.0/pyatem/media.py
--rw-r--r--   0 root         (0) root         (0)     7730 2022-06-08 11:24:54.000000 pyatem-0.8.0/pyatem/mediaconvertmodule.c
--rw-r--r--   0 root         (0) root         (0)    22200 2022-08-14 17:38:03.000000 pyatem-0.8.0/pyatem/protocol.py
--rw-r--r--   0 root         (0) root         (0)     1061 2022-05-29 16:55:34.000000 pyatem-0.8.0/pyatem/socketqueue.py
--rw-r--r--   0 root         (0) root         (0)     3514 2022-06-08 11:41:09.000000 pyatem-0.8.0/pyatem/test_colorspace.py
--rw-r--r--   0 root         (0) root         (0)     1781 2022-05-29 16:55:34.000000 pyatem-0.8.0/pyatem/test_media.py
--rw-r--r--   0 root         (0) root         (0)     2698 2022-05-29 16:55:34.000000 pyatem-0.8.0/pyatem/test_rle.py
--rw-r--r--   0 root         (0) root         (0)     2260 2022-06-05 14:07:43.000000 pyatem-0.8.0/pyatem/transfer.py
--rw-r--r--   0 root         (0) root         (0)    20543 2022-09-16 11:59:33.000000 pyatem-0.8.0/pyatem/transport.py
--rw-r--r--   0 root         (0) root         (0)     5778 2022-05-20 11:17:47.000000 pyatem-0.8.0/pyatem/videohub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-16 12:03:46.734415 pyatem-0.8.0/pyatem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3577 2022-09-16 12:03:46.000000 pyatem-0.8.0/pyatem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      506 2022-09-16 12:03:46.000000 pyatem-0.8.0/pyatem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-16 12:03:46.000000 pyatem-0.8.0/pyatem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-09-16 12:03:46.000000 pyatem-0.8.0/pyatem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-16 12:03:46.734415 pyatem-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      784 2022-09-16 12:00:45.000000 pyatem-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.414320 pyatem-0.9.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.365320 pyatem-0.9.0/.builds/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-03-23 15:17:49.000000 pyatem-0.9.0/.builds/site.yml
+-rw-r--r--   0 root         (0) root         (0)     2218 2022-10-14 20:50:18.000000 pyatem-0.9.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      655 2022-10-14 20:50:18.000000 pyatem-0.9.0/100-blackmagicdesign.rules
+-rw-r--r--   0 root         (0) root         (0)      288 2022-10-15 21:25:30.000000 pyatem-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    35149 2022-10-15 21:25:30.000000 pyatem-0.9.0/LICENSE-gpl3.txt
+-rw-r--r--   0 root         (0) root         (0)     7652 2022-10-15 21:25:30.000000 pyatem-0.9.0/LICENSE-lgpl3.txt
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-06-01 17:04:01.414320 pyatem-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2994 2023-01-29 18:52:55.000000 pyatem-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.367320 pyatem-0.9.0/bmd_setup/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-10-14 20:50:18.000000 pyatem-0.9.0/bmd_setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      825 2022-10-15 21:25:29.000000 pyatem-0.9.0/bmd_setup/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      544 2022-10-15 21:50:44.000000 pyatem-0.9.0/bmd_setup/bmd-setup.1.scd
+-rwxr-xr-x   0 root         (0) root         (0)      439 2022-10-15 21:25:29.000000 pyatem-0.9.0/bmd_setup/bmd-setup.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.368320 pyatem-0.9.0/bmd_setup/data/
+-rw-r--r--   0 root         (0) root         (0)      341 2022-10-14 20:50:18.000000 pyatem-0.9.0/bmd_setup/data/meson.build
+-rw-r--r--   0 root         (0) root         (0)     1939 2022-10-17 23:40:19.000000 pyatem-0.9.0/bmd_setup/data/nl.brixit.Setup.appdata.xml
+-rw-r--r--   0 root         (0) root         (0)      231 2022-10-15 21:27:06.000000 pyatem-0.9.0/bmd_setup/data/nl.brixit.Setup.desktop
+-rw-r--r--   0 root         (0) root         (0)    16365 2022-10-14 20:50:18.000000 pyatem-0.9.0/bmd_setup/data/nl.brixit.Setup.svg
+-rw-r--r--   0 root         (0) root         (0)     1528 2022-10-17 12:33:21.000000 pyatem-0.9.0/bmd_setup/meson.build
+-rw-r--r--   0 root         (0) root         (0)    13829 2022-12-31 15:38:09.000000 pyatem-0.9.0/bmd_setup/window.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.368320 pyatem-0.9.0/build-aux/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.368320 pyatem-0.9.0/build-aux/meson/
+-rw-r--r--   0 root         (0) root         (0)      595 2021-02-02 20:42:38.000000 pyatem-0.9.0/build-aux/meson/postinstall.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2022-10-14 20:50:18.000000 pyatem-0.9.0/build-aux/nl.brixit.Setup.json
+-rw-r--r--   0 root         (0) root         (0)     1649 2022-10-14 20:50:18.000000 pyatem-0.9.0/build-aux/nl.brixit.Switcher.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.369320 pyatem-0.9.0/data/
+-rw-r--r--   0 root         (0) root         (0)      471 2021-02-09 15:02:01.000000 pyatem-0.9.0/data/meson.build
+-rw-r--r--   0 root         (0) root         (0)     7816 2023-06-01 16:52:18.000000 pyatem-0.9.0/data/nl.brixit.Switcher.appdata.xml
+-rw-r--r--   0 root         (0) root         (0)      280 2022-10-14 21:10:22.000000 pyatem-0.9.0/data/nl.brixit.Switcher.desktop
+-rw-r--r--   0 root         (0) root         (0)      820 2022-10-14 20:50:18.000000 pyatem-0.9.0/data/nl.brixit.Switcher.gschema.xml
+-rw-r--r--   0 root         (0) root         (0)    13693 2021-02-08 01:15:04.000000 pyatem-0.9.0/data/nl.brixit.Switcher.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.372320 pyatem-0.9.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2021-01-30 01:14:18.000000 pyatem-0.9.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.374320 pyatem-0.9.0/docs/commands/
+-rw-r--r--   0 root         (0) root         (0)      559 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands/audiomixer.rst
+-rw-r--r--   0 root         (0) root         (0)      530 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands/camera.rst
+-rw-r--r--   0 root         (0) root         (0)      634 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands/encoder.rst
+-rw-r--r--   0 root         (0) root         (0)      562 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands/fairlightmixer.rst
+-rw-r--r--   0 root         (0) root         (0)      773 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands/filetransfer.rst
+-rw-r--r--   0 root         (0) root         (0)      374 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands/hardware.rst
+-rw-r--r--   0 root         (0) root         (0)     3271 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands/switcher.rst
+-rw-r--r--   0 root         (0) root         (0)      320 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)     1981 2021-02-11 00:30:02.000000 pyatem-0.9.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     8296 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/converters.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.375320 pyatem-0.9.0/docs/fields/
+-rw-r--r--   0 root         (0) root         (0)      605 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/fields/audiomixer.rst
+-rw-r--r--   0 root         (0) root         (0)     1010 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/fields/encoder.rst
+-rw-r--r--   0 root         (0) root         (0)      981 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/fields/fairlightmixer.rst
+-rw-r--r--   0 root         (0) root         (0)      808 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/fields/filetransfer.rst
+-rw-r--r--   0 root         (0) root         (0)      912 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/fields/hardware.rst
+-rw-r--r--   0 root         (0) root         (0)     2167 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/fields/switcher.rst
+-rw-r--r--   0 root         (0) root         (0)      283 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/fields.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.375320 pyatem-0.9.0/docs/images/
+-rw-r--r--   0 root         (0) root         (0)    32377 2022-04-16 00:23:49.000000 pyatem-0.9.0/docs/images/proxy-status.png
+-rw-r--r--   0 root         (0) root         (0)      573 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2021-01-30 01:14:18.000000 pyatem-0.9.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     7062 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/media.rst
+-rw-r--r--   0 root         (0) root         (0)     6926 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/proxy.rst
+-rw-r--r--   0 root         (0) root         (0)     3229 2021-02-11 18:07:33.000000 pyatem-0.9.0/docs/python.rst
+-rw-r--r--   0 root         (0) root         (0)     4384 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/tcptransport.rst
+-rw-r--r--   0 root         (0) root         (0)     5729 2023-02-11 13:31:59.000000 pyatem-0.9.0/docs/udptransport.rst
+-rw-r--r--   0 root         (0) root         (0)     3241 2022-10-14 20:50:18.000000 pyatem-0.9.0/docs/usbtransport.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.376320 pyatem-0.9.0/examples/
+-rw-r--r--   0 root         (0) root         (0)     2955 2021-08-04 17:04:46.000000 pyatem-0.9.0/examples/apiserver.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2021-08-04 16:48:19.000000 pyatem-0.9.0/examples/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2022-10-14 20:50:18.000000 pyatem-0.9.0/examples/stills.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.383320 pyatem-0.9.0/gtk_switcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-31 14:58:21.000000 pyatem-0.9.0/gtk_switcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2022-10-15 21:20:39.000000 pyatem-0.9.0/gtk_switcher/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2022-10-15 21:20:48.000000 pyatem-0.9.0/gtk_switcher/adjustmententry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.384320 pyatem-0.9.0/gtk_switcher/asset/
+-rw-r--r--   0 root         (0) root         (0)    79673 2021-03-05 21:00:21.000000 pyatem-0.9.0/gtk_switcher/asset/rainbow.png
+-rw-r--r--   0 root         (0) root         (0)     1685 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/atem.gresource.xml
+-rw-r--r--   0 root         (0) root         (0)    26337 2023-02-23 12:32:18.000000 pyatem-0.9.0/gtk_switcher/atemwindow.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2022-10-15 21:20:55.000000 pyatem-0.9.0/gtk_switcher/audio.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2022-10-15 21:20:59.000000 pyatem-0.9.0/gtk_switcher/camera.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2022-10-15 21:21:01.000000 pyatem-0.9.0/gtk_switcher/colorwheel.py
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-01-28 16:47:19.000000 pyatem-0.9.0/gtk_switcher/connectionwindow.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2022-10-15 21:21:07.000000 pyatem-0.9.0/gtk_switcher/debugger.py
+-rw-r--r--   0 root         (0) root         (0)      504 2022-10-15 21:21:11.000000 pyatem-0.9.0/gtk_switcher/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2022-10-15 21:21:14.000000 pyatem-0.9.0/gtk_switcher/dial.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2022-10-15 21:21:18.000000 pyatem-0.9.0/gtk_switcher/downstreamkey.py
+-rw-r--r--   0 root         (0) root         (0)    10732 2022-10-15 21:21:21.000000 pyatem-0.9.0/gtk_switcher/eqcurve.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2022-10-15 21:21:24.000000 pyatem-0.9.0/gtk_switcher/eqwindow.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2022-10-15 21:21:26.000000 pyatem-0.9.0/gtk_switcher/gtklogadjustment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.389320 pyatem-0.9.0/gtk_switcher/icons/
+-rw-r--r--   0 root         (0) root         (0)     4352 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/multiview-bl.svg
+-rw-r--r--   0 root         (0) root         (0)     4352 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/multiview-br.svg
+-rw-r--r--   0 root         (0) root         (0)     2320 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/multiview-safearea.svg
+-rw-r--r--   0 root         (0) root         (0)     2255 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/multiview-swap.svg
+-rw-r--r--   0 root         (0) root         (0)     4309 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/multiview-tl.svg
+-rw-r--r--   0 root         (0) root         (0)     4351 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/multiview-tr.svg
+-rw-r--r--   0 root         (0) root         (0)     4174 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/multiview-vu.svg
+-rw-r--r--   0 root         (0) root         (0)    13693 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/icons/openswitcher.svg
+-rw-r--r--   0 root         (0) root         (0)     1846 2021-02-04 18:30:19.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-bl.svg
+-rw-r--r--   0 root         (0) root         (0)     1855 2021-02-04 18:34:07.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-bottom.svg
+-rw-r--r--   0 root         (0) root         (0)     1850 2021-02-04 18:30:03.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-br.svg
+-rw-r--r--   0 root         (0) root         (0)     1848 2021-02-04 18:34:24.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-left.svg
+-rw-r--r--   0 root         (0) root         (0)     1853 2021-02-04 18:34:37.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-right.svg
+-rw-r--r--   0 root         (0) root         (0)     1842 2021-02-04 18:29:16.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-tl.svg
+-rw-r--r--   0 root         (0) root         (0)     1848 2021-02-04 18:33:52.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-top.svg
+-rw-r--r--   0 root         (0) root         (0)     1846 2021-02-04 18:29:53.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box-tr.svg
+-rw-r--r--   0 root         (0) root         (0)     1848 2021-02-04 18:29:38.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-box.svg
+-rw-r--r--   0 root         (0) root         (0)     2654 2021-02-04 18:19:56.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-cross.svg
+-rw-r--r--   0 root         (0) root         (0)     1851 2021-02-04 18:36:05.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-diag1.svg
+-rw-r--r--   0 root         (0) root         (0)     1851 2021-02-04 18:36:21.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-diag2.svg
+-rw-r--r--   0 root         (0) root         (0)     1863 2021-02-04 18:27:33.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-diamond.svg
+-rw-r--r--   0 root         (0) root         (0)     1798 2021-02-04 18:14:38.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-h.svg
+-rw-r--r--   0 root         (0) root         (0)     2010 2021-02-04 18:28:42.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-iris.svg
+-rw-r--r--   0 root         (0) root         (0)     2040 2021-02-04 18:19:01.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-mh.svg
+-rw-r--r--   0 root         (0) root         (0)     2127 2021-02-04 18:19:17.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-mv.svg
+-rw-r--r--   0 root         (0) root         (0)     1807 2021-02-04 18:15:03.000000 pyatem-0.9.0/gtk_switcher/icons/wipe-v.svg
+-rw-r--r--   0 root         (0) root         (0)    18234 2022-10-15 21:21:29.000000 pyatem-0.9.0/gtk_switcher/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2022-10-15 21:21:31.000000 pyatem-0.9.0/gtk_switcher/macroeditor.py
+-rw-r--r--   0 root         (0) root         (0)    14849 2022-11-19 15:14:00.000000 pyatem-0.9.0/gtk_switcher/media.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2022-10-17 12:30:13.000000 pyatem-0.9.0/gtk_switcher/meson.build
+-rw-r--r--   0 root         (0) root         (0)    28327 2023-02-22 23:58:07.000000 pyatem-0.9.0/gtk_switcher/mixeffect.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2022-10-15 21:21:53.000000 pyatem-0.9.0/gtk_switcher/mixeffect_aux.py
+-rw-r--r--   0 root         (0) root         (0)    16258 2022-10-15 21:21:59.000000 pyatem-0.9.0/gtk_switcher/preferences.py
+-rw-r--r--   0 root         (0) root         (0)     1786 2022-10-15 21:21:56.000000 pyatem-0.9.0/gtk_switcher/stream_data.py
+-rw-r--r--   0 root         (0) root         (0)      949 2022-10-15 21:40:59.000000 pyatem-0.9.0/gtk_switcher/switcher-control.1.scd
+-rwxr-xr-x   0 root         (0) root         (0)      897 2022-10-18 11:20:40.000000 pyatem-0.9.0/gtk_switcher/switcher-control.in
+-rw-r--r--   0 root         (0) root         (0)    53864 2023-02-23 00:39:49.000000 pyatem-0.9.0/gtk_switcher/switcher.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2022-10-15 21:22:13.000000 pyatem-0.9.0/gtk_switcher/template_i18n.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.394320 pyatem-0.9.0/gtk_switcher/ui/
+-rw-r--r--   0 root         (0) root         (0)    33180 2023-01-28 16:47:15.000000 pyatem-0.9.0/gtk_switcher/ui/connection.glade
+-rw-r--r--   0 root         (0) root         (0)     8334 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/debugger.glade
+-rw-r--r--   0 root         (0) root         (0)    19719 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/downstream-keyer.glade
+-rw-r--r--   0 root         (0) root         (0)    20129 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/eq.glade
+-rw-r--r--   0 root         (0) root         (0)     9934 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/macro-editor.glade
+-rw-r--r--   0 root         (0) root         (0)     6586 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/mixeffect-aux.glade
+-rw-r--r--   0 root         (0) root         (0)    58343 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/mixeffect.glade
+-rw-r--r--   0 root         (0) root         (0)   254926 2023-02-27 16:55:38.000000 pyatem-0.9.0/gtk_switcher/ui/mixer.glade
+-rw-r--r--   0 root         (0) root         (0)    63993 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/preferences.glade
+-rw-r--r--   0 root         (0) root         (0)     2579 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/shortcuts.ui
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-01-28 16:50:32.000000 pyatem-0.9.0/gtk_switcher/ui/style.css
+-rw-r--r--   0 root         (0) root         (0)    94554 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/upstream-keyer.glade
+-rw-r--r--   0 root         (0) root         (0)     6580 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/videohub-bus.glade
+-rw-r--r--   0 root         (0) root         (0)     5200 2022-10-14 20:50:18.000000 pyatem-0.9.0/gtk_switcher/ui/videohub.glade
+-rw-r--r--   0 root         (0) root         (0)    21302 2023-02-23 00:30:42.000000 pyatem-0.9.0/gtk_switcher/upstreamkey.py
+-rw-r--r--   0 root         (0) root         (0)     5900 2022-10-15 21:22:18.000000 pyatem-0.9.0/gtk_switcher/videohub.py
+-rw-r--r--   0 root         (0) root         (0)     3734 2022-10-15 21:22:21.000000 pyatem-0.9.0/gtk_switcher/videohubbus.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2022-10-15 21:22:23.000000 pyatem-0.9.0/gtk_switcher/videohubconnection.py
+-rw-r--r--   0 root         (0) root         (0)      586 2023-06-01 16:46:08.000000 pyatem-0.9.0/meson.build
+-rw-r--r--   0 root         (0) root         (0)      263 2022-10-15 21:42:40.000000 pyatem-0.9.0/meson_options.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.394320 pyatem-0.9.0/notebooks/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-03-16 01:59:35.000000 pyatem-0.9.0/notebooks/clip-upload-notes.txt
+-rw-r--r--   0 root         (0) root         (0)    65946 2023-03-20 01:46:46.000000 pyatem-0.9.0/notebooks/constellation-fields.txt
+-rw-r--r--   0 root         (0) root         (0)    40420 2022-10-14 20:50:18.000000 pyatem-0.9.0/notebooks/eqcurve.ipynb
+-rwxr-xr-x   0 root         (0) root         (0)      726 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher-develop.sh
+-rwxr-xr-x   0 root         (0) root         (0)      633 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher-install.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.397320 pyatem-0.9.0/openswitcher_proxy/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-16 00:23:49.000000 pyatem-0.9.0/openswitcher_proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2758 2023-02-27 00:50:57.000000 pyatem-0.9.0/openswitcher_proxy/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2022-10-16 22:05:42.000000 pyatem-0.9.0/openswitcher_proxy/atemswitch.1.scd
+-rw-r--r--   0 root         (0) root         (0)     1637 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher_proxy/cli-switch.py
+-rw-r--r--   0 root         (0) root         (0)      151 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher_proxy/error.py
+-rw-r--r--   0 root         (0) root         (0)      852 2022-04-16 00:23:49.000000 pyatem-0.9.0/openswitcher_proxy/frontend.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2022-04-16 00:23:49.000000 pyatem-0.9.0/openswitcher_proxy/frontend_httpapi.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher_proxy/frontend_mqtt.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2022-04-16 00:23:49.000000 pyatem-0.9.0/openswitcher_proxy/frontend_status.py
+-rw-r--r--   0 root         (0) root         (0)     8934 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher_proxy/frontend_tcp.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher_proxy/hardware.py
+-rw-r--r--   0 root         (0) root         (0)     1720 2022-10-17 12:32:14.000000 pyatem-0.9.0/openswitcher_proxy/meson.build
+-rw-r--r--   0 root         (0) root         (0)      933 2022-10-15 21:47:44.000000 pyatem-0.9.0/openswitcher_proxy/openswitcher-proxy.1.scd
+-rwxr-xr-x   0 root         (0) root         (0)      318 2022-10-14 20:50:18.000000 pyatem-0.9.0/openswitcher_proxy/openswitcher-proxy.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.400320 pyatem-0.9.0/po/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-02-01 14:17:09.000000 pyatem-0.9.0/po/LINGUAS
+-rw-r--r--   0 root         (0) root         (0)      454 2022-10-14 20:50:18.000000 pyatem-0.9.0/po/POTFILES
+-rw-r--r--   0 root         (0) root         (0)    16343 2023-02-01 14:17:09.000000 pyatem-0.9.0/po/cs.po
+-rw-r--r--   0 root         (0) root         (0)    17673 2022-10-14 20:50:18.000000 pyatem-0.9.0/po/da.po
+-rw-r--r--   0 root         (0) root         (0)    20267 2023-02-01 14:17:09.000000 pyatem-0.9.0/po/de.po
+-rw-r--r--   0 root         (0) root         (0)    17769 2022-10-14 20:50:18.000000 pyatem-0.9.0/po/en.po
+-rw-r--r--   0 root         (0) root         (0)    20874 2023-02-01 14:17:09.000000 pyatem-0.9.0/po/es.po
+-rw-r--r--   0 root         (0) root         (0)       44 2022-10-14 20:50:18.000000 pyatem-0.9.0/po/meson.build
+-rw-r--r--   0 root         (0) root         (0)    18566 2022-10-14 20:50:18.000000 pyatem-0.9.0/po/nb_NO.po
+-rw-r--r--   0 root         (0) root         (0)    20841 2023-02-01 14:17:09.000000 pyatem-0.9.0/po/nl.po
+-rw-r--r--   0 root         (0) root         (0)    17700 2022-10-14 20:50:18.000000 pyatem-0.9.0/po/openswitcher.pot
+-rw-r--r--   0 root         (0) root         (0)    19103 2022-10-14 20:50:18.000000 pyatem-0.9.0/po/sv.po
+-rw-r--r--   0 root         (0) root         (0)    23215 2023-02-01 14:17:09.000000 pyatem-0.9.0/po/tr.po
+-rw-r--r--   0 root         (0) root         (0)      487 2022-04-16 00:23:49.000000 pyatem-0.9.0/proxy-full.toml
+-rw-r--r--   0 root         (0) root         (0)      583 2023-02-27 00:51:11.000000 pyatem-0.9.0/proxy.toml
+-rwxr-xr-x   0 root         (0) root         (0)       66 2022-10-14 20:50:18.000000 pyatem-0.9.0/publish-pypi.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.405320 pyatem-0.9.0/pyatem/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-30 01:10:34.000000 pyatem-0.9.0/pyatem/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/cameracontrol.py
+-rw-r--r--   0 root         (0) root         (0)    90687 2023-03-23 15:46:14.000000 pyatem-0.9.0/pyatem/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.406320 pyatem-0.9.0/pyatem/converters/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-10-14 20:50:18.000000 pyatem-0.9.0/pyatem/converters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2022-12-31 15:12:51.000000 pyatem-0.9.0/pyatem/converters/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     3625 2022-12-31 15:14:12.000000 pyatem-0.9.0/pyatem/converters/converter.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2022-10-16 21:55:15.000000 pyatem-0.9.0/pyatem/converters/lut.py
+-rw-r--r--   0 root         (0) root         (0)     9527 2023-01-20 14:17:05.000000 pyatem-0.9.0/pyatem/converters/protocol.py
+-rw-r--r--   0 root         (0) root         (0)      785 2022-10-17 15:40:01.000000 pyatem-0.9.0/pyatem/converters/test_lut.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.407320 pyatem-0.9.0/pyatem/dissector/
+-rw-r--r--   0 root         (0) root         (0)    13148 2023-01-15 17:29:42.000000 pyatem-0.9.0/pyatem/dissector/atem_dissector.tpl
+-rw-r--r--   0 root         (0) root         (0)     3677 2023-01-15 18:14:14.000000 pyatem-0.9.0/pyatem/dissector/generator.py
+-rw-r--r--   0 root         (0) root         (0)   111560 2023-06-01 16:47:23.000000 pyatem-0.9.0/pyatem/field.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.411320 pyatem-0.9.0/pyatem/fixtures/
+-rw-r--r--   0 root         (0) root         (0)    19652 2022-10-14 20:50:18.000000 pyatem-0.9.0/pyatem/fixtures/linear-17.bin
+-rwxr-xr-x   0 root         (0) root         (0)   124607 2022-10-14 20:50:18.000000 pyatem-0.9.0/pyatem/fixtures/linear-17.cube
+-rw-r--r--   0 root         (0) root         (0)  2500072 2022-10-14 20:50:18.000000 pyatem-0.9.0/pyatem/fixtures/ramps-atemsc.data.gz
+-rwxr-xr-x   0 root         (0) root         (0)  1127569 2022-10-14 20:50:18.000000 pyatem-0.9.0/pyatem/fixtures/ramps.png
+-rw-r--r--   0 root         (0) root         (0)    15178 2022-10-14 20:50:18.000000 pyatem-0.9.0/pyatem/hexdump.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/locate.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/macro.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/macrocommand.py
+-rw-r--r--   0 root         (0) root         (0)     3559 2022-11-19 15:11:00.000000 pyatem-0.9.0/pyatem/media.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-06-01 16:47:23.000000 pyatem-0.9.0/pyatem/mediaconvertmodule.c
+-rw-r--r--   0 root         (0) root         (0)    23483 2023-03-19 14:37:28.000000 pyatem-0.9.0/pyatem/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/socketqueue.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/test_colorspace.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/test_media.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/test_rle.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/transfer.py
+-rw-r--r--   0 root         (0) root         (0)    20690 2023-02-11 13:31:59.000000 pyatem-0.9.0/pyatem/transport.py
+-rw-r--r--   0 root         (0) root         (0)     5888 2022-10-16 21:54:35.000000 pyatem-0.9.0/pyatem/videohub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.405320 pyatem-0.9.0/pyatem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-06-01 17:04:01.000000 pyatem-0.9.0/pyatem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5377 2023-06-01 17:04:01.000000 pyatem-0.9.0/pyatem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 17:04:01.000000 pyatem-0.9.0/pyatem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 17:04:01.000000 pyatem-0.9.0/pyatem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2021-02-02 11:47:59.000000 pyatem-0.9.0/pyhyperdeckemu.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 17:04:01.414320 pyatem-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-06-01 16:46:08.000000 pyatem-0.9.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2022-10-14 20:50:18.000000 pyatem-0.9.0/test-against-hardware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.413320 pyatem-0.9.0/testset/
+-rw-r--r--   0 root         (0) root         (0)     1650 2022-10-14 20:50:18.000000 pyatem-0.9.0/testset/ATEM Mini Pro.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 17:04:01.413320 pyatem-0.9.0/utils/
+-rw-r--r--   0 root         (0) root         (0)     2871 2022-10-14 20:50:18.000000 pyatem-0.9.0/utils/atem-to-rgb.c
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-03-19 14:35:23.000000 pyatem-0.9.0/utils/dump-unknown.py
```

### Comparing `pyatem-0.8.0/LICENSE` & `pyatem-0.9.0/LICENSE-lgpl3.txt`

 * *Files identical despite different names*

### Comparing `pyatem-0.8.0/PKG-INFO` & `pyatem-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: pyatem
-Version: 0.8.0
+Version: 0.9.0
 Summary: Library implementing the Blackmagic Design Atem switcher protocol
 Home-page: https://git.sr.ht/~martijnbraam/pyatem
 Author: Martijn Braam
 Author-email: martijn@brixit.nl
 License: LGPL3
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
+License-File: LICENSE-gpl3.txt
+License-File: LICENSE-lgpl3.txt
 
 PyATEM
 ======
 
 Library implementing the ATEM video switcher protocol and a GTK3.0 application
 
 ![Screenshot of the control application](https://brixitcdn.net/metainfo/openswitcher.png)
@@ -76,15 +82,15 @@
 
     python3 -m openswitcher_proxy --config /etc/myconfigfile.toml
 
 Or if the software installed it can be started using the launcher script::
 
     openswitcher-proxy --config /etc/myconfigfile.toml
 
-The default config location is /etc/openswitcher/proxy.conf if not specified. Here's an example config:
+The default config location is /etc/openswitcher/proxy.toml if not specified. Here's an example config:
 
     [[hardware]]
     id = "mini"
     label = "Atem Mini"
     address = "192.168.2.84"
 
     [[hardware]]
@@ -113,8 +119,7 @@
 
 
 Translations
 ------------
 
 The main language for the software is english, the translation for the project happens on
 https://hosted.weblate.org/projects/openswitcher
-
```

### Comparing `pyatem-0.8.0/README.md` & `pyatem-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     python3 -m openswitcher_proxy --config /etc/myconfigfile.toml
 
 Or if the software installed it can be started using the launcher script::
 
     openswitcher-proxy --config /etc/myconfigfile.toml
 
-The default config location is /etc/openswitcher/proxy.conf if not specified. Here's an example config:
+The default config location is /etc/openswitcher/proxy.toml if not specified. Here's an example config:
 
     [[hardware]]
     id = "mini"
     label = "Atem Mini"
     address = "192.168.2.84"
 
     [[hardware]]
```

### Comparing `pyatem-0.8.0/pyatem/cameracontrol.py` & `pyatem-0.9.0/pyatem/cameracontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import math
 import sys
 import inspect
 
 from pyatem.command import CameraControlCommand
 
 _cache = {}
```

### Comparing `pyatem-0.8.0/pyatem/command.py` & `pyatem-0.9.0/pyatem/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import colorsys
+import datetime
 import struct
 
 
 class Command:
     def get_command(self):
         pass
 
@@ -1222,15 +1225,19 @@
     === ==========
 
 
     """
 
     def __init__(self, eq_gain=None, dynamics_gain=None, volume=None, afv=None, eq_enable=None):
         """
-        :param index: 0-indexed M/E number to control the preview bus of
+        :param eq_gain: Make-up gain for the master EQ dialog
+        :param eq_enable: Enable the EQ on the master bus
+        :param dynamics_gain: Make-up gain for the master Dynamics dialog
+        :param volume: Master volume fader value
+        :param afv: Make the master volume follow the fade-to-black function
         """
 
         self.eq_gain = eq_gain
         self.dynamics_gain = dynamics_gain
         self.volume = volume
         self.afv = afv
         self.eq_enable = eq_enable
@@ -1258,14 +1265,19 @@
         return self._make_command('CFMP', data)
 
 
 class FairlightStripPropertiesCommand(Command):
     """
     Implementation of the `CFSP` command. This sets the settings of a channel strip in fairlight audio.
 
+    The source index is the same as the video source index from the InputProperties fields.
+
+    For normal channel strips the channel index should be -1. If the channel is split (two mono channels instead of a
+    stereo input) the channel numbers are 0 and 1.
+
     ====== ==== ====== ===========
     Offset Size Type   Description
     ====== ==== ====== ===========
     0      2    u16    Mask, see table below
     2      2    u16    Source index
     15     1    u8     Channel number
     16     1    u8     Delay in frames
@@ -1294,15 +1306,24 @@
 
 
     """
 
     def __init__(self, source, channel, delay=None, gain=None, eq_gain=None, eq_enable=None, dynamics_gain=None,
                  balance=None, volume=None, state=None):
         """
-        :param index: 0-indexed M/E number to control the preview bus of
+        :param source: The source index
+        :param channel: The channel index inside the source, -1 for the normal stereo channels and 0 and 1 for split
+        :param delay: Delay in frames
+        :param gain: Input gain
+        :param eq_gain: Make-up gain from the EQ dialog
+        :param eq_enable: Enable the EQ block
+        :param dynamics_gain: Make-up gain from the dynamics dialog
+        :param balance: Channel balance or pan
+        :param volume: The volume fader level
+        :param state: Bitfield for the mute and AFV state. 1=off, 2=on, 4=afv
         """
         self.source = source
         self.channel = channel
         self.delay = delay
         self.gain = gain
         self.eq_gain = eq_gain
         self.eq_enable = eq_enable
@@ -1338,15 +1359,15 @@
         balance = 0 if self.balance is None else self.balance
         volume = 0 if self.volume is None else self.volume
         state = 0 if self.state is None else self.state
 
         split = 0xff if self.channel > -1 else 0x01
         self.channel = 0x00 if self.channel == -1 else self.channel
         pad = b'\xff\xff\xff\xff\xff\xff\xff'
-        data = struct.pack('>H H4x6sBb B 3x i ? 5x h 2x Hh 2x iB 3x', mask, self.source, pad, split, self.channel,
+        data = struct.pack('>H H4x6sBb B 3x i xx? 1x h 2x H 2x h 2x iB 3x', mask, self.source, pad, split, self.channel,
                            delay,
                            gain, eq_enable, eq_gain,
                            dynamics_gain, balance, volume, state)
         return self._make_command('CFSP', data)
 
 
 class KeyOnAirCommand(Command):
@@ -1912,15 +1933,16 @@
         brightness = 0 if self.brightness is None else self.brightness
         contrast = 0 if self.contrast is None else self.contrast
         saturation = 0 if self.saturation is None else self.saturation
         red = 0 if self.red is None else self.red
         green = 0 if self.green is None else self.green
         blue = 0 if self.blue is None else self.blue
 
-        data = struct.pack('>HBB HHH HH hhHhhh xx', mask, self.index, self.keyer, foreground, background, key_edge, spill,
+        data = struct.pack('>HBB HHH HH hhHhhh xx', mask, self.index, self.keyer, foreground, background, key_edge,
+                           spill,
                            flare, brightness, contrast, saturation, red, green, blue)
 
         return self._make_command('CACK', data)
 
 
 class KeyPropertiesLumaCommand(Command):
     """
@@ -2192,14 +2214,40 @@
         key = self.key.encode() if self.key is not None else b''
 
         data = struct.pack('>B 64s 512s 512s 3x II', mask, name, url, key,
                            self.bitrate_min or 0, self.bitrate_max or 0)
         return self._make_command('CRSS', data)
 
 
+class StreamingAudioBitrateCommand(Command):
+    """
+    Implementation of the `STAB` command. This sets the audio bitrate parameters for the stream and recording.
+    In practice this is always set to 128k min/max bitrate.
+
+    ====== ==== ====== ===========
+    Offset Size Type   Description
+    ====== ==== ====== ===========
+    0      4    u32    Minimum bitrate (Bps)
+    4      4    u32    Maximum bitrate (Bps)
+    ====== ==== ====== ===========
+    """
+
+    def __init__(self, bitrate_min, bitrate_max):
+        """
+        :param bitrate_min: Minimum bitrate
+        :param bitrate_max: Maximum bitrate
+        """
+        self.bitrate_min = bitrate_min
+        self.bitrate_max = bitrate_max
+
+    def get_command(self):
+        data = struct.pack('>II', self.bitrate_min, self.bitrate_max)
+        return self._make_command('STAB', data)
+
+
 class StreamingStatusSetCommand(Command):
     """
     Implementation of the `StrR` command. This starts and stops the live stream
 
     ====== ==== ====== ===========
     Offset Size Type   Description
     ====== ==== ====== ===========
@@ -2751,14 +2799,30 @@
     This command has no arguments
     """
 
     def get_command(self):
         return self._make_command('TiRq', b'')
 
 
+class SetTimeOfDayCommand(Command):
+    """
+    Set the time of day on the hardware. Used my ATEMSC at startup to set the atem to the system clock of the computer.
+    """
+
+    def __init__(self, time):
+        if not isinstance(time, datetime.datetime):
+            raise ValueError()
+        self.time = time
+
+    def get_command(self):
+        timestamp = self.time.timestamp()
+        data = struct.pack('>I4x', timestamp)
+        return self._make_command('SToD', data)
+
+
 class TransferCompleteCommand(Command):
     """
     Implementation of the `*XFC` command. This is an command that's part of OpenSwitcher for the TCP protocol and not part
     of the actual ATEM protocol.
 
     ====== ==== ====== ===========
     Offset Size Type   Description
```

### Comparing `pyatem-0.8.0/pyatem/field.py` & `pyatem-0.9.0/pyatem/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import colorsys
 import struct
 import math
 
 from pyatem.hexdump import hexdump
 
 
@@ -109,30 +111,33 @@
 class ProductNameField(FieldBase):
     """
     Data from the `_pin` field. This stores the product name of the mixer
 
     ====== ==== ====== ===========
     Offset Size Type   Description
     ====== ==== ====== ===========
-    0      44   char[] Product name
+    0      40   char[] Product name
+    40     1    u8     Model number
+    41     3    ?      unknown
     ====== ==== ====== ===========
 
     After parsing:
 
     :ivar name: User friendly product name
     """
 
     CODE = "_pin"
 
     def __init__(self, raw):
         self.raw = raw
-        self.name = self._get_string(raw)
+        name, self.model = struct.unpack('>40s B 3x', raw)
+        self.name = self._get_string(name)
 
     def __repr__(self):
-        return '<product-name {}>'.format(self.name)
+        return '<product-name {} (model 0x{:02X})>'.format(self.name, self.model)
 
 
 class MixerEffectConfigField(FieldBase):
     """
     Data from the `_MeC` field. This stores basic info about the M/E units.
 
     The mixer will send multiple fields, one for each M/E unit.
@@ -260,14 +265,16 @@
     21  8k24
     22  8k25
     23  8k29.97
     24  8k50
     25  8k59.94
     26  1080p30
     27  1080p60
+    28  720p60
+    29  1080i60
     === ==========
 
     After parsing:
 
     :ivar mode: mode number
     :ivar resolution: vertical resolution of the mode
     :ivar interlaced: the current mode is interlaced
@@ -306,21 +313,25 @@
             21: (4320, False, 24, True),
             22: (4320, False, 25, True),
             23: (4320, False, 29.97, True),
             24: (4320, False, 50, True),
             25: (4320, False, 59.94, True),
             26: (1080, False, 30, True),
             27: (1080, False, 60, True),
+            28: (720, False, 60, True),
+            29: (1080, True, 60, True),
         }
 
         if self.mode in modes:
             self.resolution = modes[self.mode][0]
             self.interlaced = modes[self.mode][1]
             self.rate = modes[self.mode][2]
             self.widescreen = modes[self.mode][3]
+        else:
+            raise ValueError(f"Unknown resolution code {self.mode}, cannot continue")
 
     def get_label(self):
         if self.resolution is None:
             return 'unknown [{}]'.format(self.mode)
 
         pi = 'p'
         if self.interlaced:
@@ -401,14 +412,16 @@
     21  8k24
     22  8k25
     23  8k29.97
     24  8k50
     25  8k59.94
     26  1080p30
     27  1080p60
+    28  720p60
+    29  1080i60
     === ==========
 
     The multiview and downconvert bitfields are the same values as the resultion numbers but the
     key is the bit instead.
 
     After parsing:
 
@@ -1021,46 +1034,46 @@
     dve                 1         1       1
     stinger             0         1       0
     supersources        0         0       0
     multiview           0         1       1
     rs485               0         1       1
     =================== ========= ======= ======
 
-    ====== ==== ====== ========= ========= ======= ======= ====== ===========
-    Offset Size Type   Atem Mini Mini Pro  1M/E 4k Prod 4k TVS HD Description
-    ====== ==== ====== ========= ========= ======= ======= ====== ===========
-    0      1    u8     1         1         1       1       1      Number of M/E units
-    1      1    u8     14        15        31      24      24     Sources
-    2      1    u8     1         1         2       2       2      Downstream keyers
-    3      1    u8     1         1         3       1       1      AUX busses
-    4      1    u8     0         0         0       0       4      MixMinus Outputs
-    5      1    u8     1         1         2       2       2      Media players
-    6      1    u8     0         1         1       1       1      Multiviewers
-    7      1    u8     0         0         1       0       1      rs485
-    8      1    u8     4         4         4       4       4      Hyperdecks
-    9      1    u8     1         1         1       0       1      DVE
-    10     1    u8     0         0         1       0       0      Stingers
-    11     1    u8     0         0         0       0       0      supersources
-    12     1    u8     0         0         1       1       1      ? Multiview routable?
-    13     1    u8     0         0         0       0       1      Talkback channels
-    14     1    u8     0         0         0       0       4      ?
-    15     1    u8     1         1         0       0       0      ?
-    16     1    u8     0         0         0       0       0      ?
-    17     1    u8     0         0         1       1       0      ?
-    18     1    u8     1         1         1       1       1      Camera Control
-    19     1    u8     0         0         1       0       1      ?
-    20     1    u8     0         0         1       0       1      ?
-    21     1    u8     0         0         1       1       1      ? Multiview routable?
-    22     1    u8     1         1         0       0       0      Advanced chroma keyers
-    23     1    u8     1         1         0       0       0      Only configurable outputs
-    24     1    u8     1         1         0       0       0      ?
-    25     1    u8     0x20      0x2f      0x20    0       0x10   ?
-    26     1    u8     3         108       0       0       0      ?
-    27     1    u8     0xe8      0x69      0x00    0       0x0    ?
-    ====== ==== ====== ========= ========= ======= ======= ====== ===========
+    ====== ==== ====== ========= ========= ======= ======= ====== ======= ===========
+    Offset Size Type   Atem Mini Mini Pro  1M/E 4k Prod 4k TVS HD CHD 2ME Description
+    ====== ==== ====== ========= ========= ======= ======= ====== ======= ===========
+    0      1    u8     1         1         1       1       1      2       Number of M/E units
+    1      1    u8     14        15        31      24      24     57      Sources
+    2      1    u8     1         1         2       2       2      2       Downstream keyers
+    3      1    u8     1         1         3       1       1      12      AUX busses
+    4      1    u8     0         0         0       0       4      12      MixMinus Outputs
+    5      1    u8     1         1         2       2       2      2       Media players
+    6      1    u8     0         1         1       1       1      2       Multiviewers
+    7      1    u8     0         0         1       0       1      0       rs485
+    8      1    u8     4         4         4       4       4      4       Hyperdecks
+    9      1    u8     1         1         1       0       1      1       DVE
+    10     1    u8     0         0         1       0       0      1       Stingers
+    11     1    u8     0         0         0       0       0      1       supersources
+    12     1    u8     0         0         1       1       1      0       ?
+    13     1    u8     0         0         0       0       1      2       Talkback channels
+    14     1    u8     0         0         0       0       4      20      SDI inputs ?
+    15     1    u8     1         1         0       0       0      1       Scalers on input?
+    16     1    u8     0         0         0       0       0      0       ?
+    17     1    u8     0         0         1       1       0      0       ?
+    18     1    u8     1         1         1       1       1      1       Camera Control
+    19     1    u8     0         0         1       0       1      0       ?
+    20     1    u8     0         0         1       0       1      0       ?
+    21     1    u8     0         0         1       1       1      1       Multiview routable
+    22     1    u8     1         1         0       0       0      1       Advanced chroma keyers
+    23     1    u8     1         1         0       0       0      1       Only configurable outputs
+    24     1    u8     1         1         0       0       0      0       ?
+    25     1    u8     0x20      0x2f      0x20    0       0x10   0       ?
+    26     1    u8     3         108       0       0       0      0       ?
+    27     1    u8     0xe8      0x69      0x00    0       0x0    0       ?
+    ====== ==== ====== ========= ========= ======= ======= ====== ======= ===========
 
 
     After parsing:
 
     :ivar me_units: Number of M/E units in the mixer
     :ivar sources: Number of internal and external sources
     :ivar downstream_keyers: Number of downstream keyers
@@ -1416,14 +1429,70 @@
         self.reverse = field[10]
         self.flipflop = field[11]
 
     def __repr__(self):
         return '<transition-dve: me={}, rate={} style={}>'.format(self.index, self.rate, self.style)
 
 
+class TransitionStingerField(FieldBase):
+    """
+    Data from the `TStP`. Settings for the Stinger transition.
+
+    ====== ==== ====== ===========
+    Offset Size Type   Descriptions
+    ====== ==== ====== ===========
+    0      1    u8     M/E index
+    1      1    u8     Stinger mediaplayer index
+    2      1    bool   Source key is premultiplied
+    3      1    ?      padding
+    4      2    u16    Key clip [0-1000]
+    6      2    u16    Key gain [0-1000]
+    8      1    bool   Key invert
+    9      1    ?      padding
+    10     2    u16    Preroll frames
+    12     2    u16    Clip duration frames
+    14     2    u16    Trigger point frame
+    16     2    u16    Mix Rate
+    18     2    ?      unknown
+    ====== ==== ====== ===========
+
+    After parsing:
+
+    :ivar index: M/E index in the mixer
+    :ivar mediaplayer: Mediaplayer number for the stinger source
+    :ivar key_premultiplied: Key is premultiplied alpha
+    :ivar key_clip: Key clipping point
+    :ivar key_gain: Key Gain
+    :ivar key_invert: Invert key source
+    :ivar preroll: Number of preroll frames
+    :ivar triggerpoint: Triggerpoint frame offset
+    :ivar duration: Clip duration in frames
+    :ivar rate: Clip rate
+    """
+
+    CODE = "TStP"
+
+    def __init__(self, raw):
+        self.raw = raw
+        field = struct.unpack('>BB?x HH?x 4H2x', raw)
+        self.index = field[0]
+        self.mediaplayer = field[1]
+        self.key_premultiplied = field[2]
+        self.key_clip = field[3]
+        self.key_gain = field[4]
+        self.key_invert = field[5]
+        self.preroll = field[6]
+        self.duration = field[7]
+        self.triggerpoint = field[8]
+        self.rate = field[9]
+
+    def __repr__(self):
+        return '<transition-stinger: me={}, mediaplayer={}>'.format(self.index, self.mediaplayer)
+
+
 class AudioMixerMasterPropertiesField(FieldBase):
     """
     Data from the `AMMO`. Settings for the master bus on legacy audio units.
 
     ====== ==== ====== ===========
     Offset Size Type   Descriptions
     ====== ==== ====== ===========
@@ -1783,14 +1852,16 @@
     5      4    ?      Unknown
     8      1    bool   Muted (0) / Umuted (1)
     9      1    u8     Last soloed channel (just the main part)
     10     22   ?      Unknown
 
     """
 
+    CODE = "FMHP"
+
     def __init__(self, raw):
         self.raw = raw
         self.volume, self.unmuted = struct.unpack('> i 4x ? 23x', raw)
 
     def __repr__(self):
         return '<fairlight-headphones volume={} unmuted={}>'.format(self.volume, self.unmuted)
 
@@ -1808,14 +1879,16 @@
     9      1    u8     Soloed channel (main)
     10     12   ?      Unknown
     22     1    u8     No subchannels (0x01), split into L/R (0xff)
     23     1    u8     Soloed channel (subchannel)
 
     """
 
+    CODE = "FAMS"
+
     def __init__(self, raw):
         self.raw = raw
         self.solo, self.channel, self.is_split_lr, self.subchannel = struct.unpack('> ? 8x B 12x BB', raw)
 
     def __repr__(self):
         return '<fairlight-solo active={} source={}>'.format(
             self.solo,
```

### Comparing `pyatem-0.8.0/pyatem/hexdump.py` & `pyatem-0.9.0/pyatem/hexdump.py`

 * *Files identical despite different names*

### Comparing `pyatem-0.8.0/pyatem/locate.py` & `pyatem-0.9.0/pyatem/locate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import ipaddress
 import logging
 import sys
 
 try:
     from zeroconf import ServiceBrowser, Zeroconf
```

### Comparing `pyatem-0.8.0/pyatem/macro.py` & `pyatem-0.9.0/pyatem/macro.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 from pyatem.macrocommand import *
 import pyatem.macrocommand as macromodule
 
 macro_command_map = {
     0x0002: ProgramInputMacroCommand,
     0x0003: PreviewInputMacroCommand,
     0x0007: SleepMacroCommand,
```

### Comparing `pyatem-0.8.0/pyatem/macrocommand.py` & `pyatem-0.9.0/pyatem/macrocommand.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import shlex
 import struct
 
 
 class BaseMacroCommand:
     NAME = "Unknown action"
     TAG = "unknown-action"
```

### Comparing `pyatem-0.8.0/pyatem/media.py` & `pyatem-0.9.0/pyatem/media.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import struct
 import pyatem.mediaconvert as mc
 
 
 def atem_to_image(data, width, height):
     """Decompress and decode an atem frame to RGBA8888"""
     data = rle_decode(data)
@@ -16,17 +18,17 @@
 
 
 def atem_to_rgb(data, width, height):
     """Wrapper for the native function"""
     return mc.atem_to_rgb(data, width, height)
 
 
-def rgb_to_atem(data, width, height):
+def rgb_to_atem(data, width, height, premultiply=False):
     """Wrapper for the native function"""
-    return mc.rgb_to_atem(data, width, height)
+    return mc.rgb_to_atem(data, width, height, premultiply)
 
 
 def rle_encode_slow(data):
     """
     See rle_decode for format description
     :param data:
     :return:
```

### Comparing `pyatem-0.8.0/pyatem/mediaconvertmodule.c` & `pyatem-0.9.0/pyatem/mediaconvertmodule.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+/*
+Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+SPDX-License-Identifier: LGPL-3.0-only
+*/
 #define PY_SSIZE_T_CLEAN
 #define RLE_HEADER 0xFEFEFEFEFEFEFEFE
 
 #include <Python.h>
 
 const double bt709_coeff_r = 0.2126;
 const double bt709_coeff_g = 0.7152;
@@ -99,19 +103,19 @@
 }
 
 static PyObject *
 method_rgb_to_atem(PyObject *self, PyObject *args)
 {
     Py_buffer input_buffer;
     Py_ssize_t data_length;
-    unsigned int width, height;
+    unsigned int width, height, premultiply;
     PyObject *res;
 
     /* Parse arguments */
-    if (!PyArg_ParseTuple(args, "y*II", &input_buffer, &width, &height)) {
+    if (!PyArg_ParseTuple(args, "y*IIp", &input_buffer, &width, &height, &premultiply)) {
         return NULL;
     }
 
     data_length = input_buffer.len;
     unsigned char *buffer;
     buffer = input_buffer.buf;
 
@@ -128,14 +132,26 @@
         float r1 = (float)buffer[0] / 255;
         float g1 = (float)buffer[1] / 255;
         float b1 = (float)buffer[2] / 255;
         float r2 = (float)buffer[4] / 255;
         float g2 = (float)buffer[5] / 255;
         float b2 = (float)buffer[6] / 255;
 
+        if (premultiply) {
+            // PNG files have straight alpha, for BMD switchers premultipled alpha is easier
+            float a1 = (float)buffer[3] / 255;
+            float a2 = (float)buffer[7] / 255;
+            r1 = r1 * a1;
+            g1 = g1 * a1;
+            b1 = b1 * a1;
+            r2 = r2 * a2;
+            g2 = g2 * a2;
+            b2 = b2 * a2;
+        }
+
         float y1 = (0.2126 * r1) + (0.7152 * g1) + (0.0722 * b1);
         float y2 = (0.2126 * r2) + (0.7152 * g2) + (0.0722 * b2);
         float cb = (b2 - y2) / 1.8556;
         float cr = (r2 - y2) /  1.5748;
 
         unsigned short a10a = ((buffer[3] << 2) * 219 / 255) + (15 << 2) + 1;
         unsigned short a10b = ((buffer[7] << 2) * 219 / 255) + (15 << 2) + 1;
```

### Comparing `pyatem-0.8.0/pyatem/protocol.py` & `pyatem-0.9.0/pyatem/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import logging
 import struct
 
 from pyatem.transfer import TransferTask, TransferQueueFlushed
 from pyatem.transport import UdpProtocol, Packet, UsbProtocol, TcpProtocol, ConnectionReady
 from pyatem.command import LockCommand, TransferDownloadRequestCommand, TransferAckCommand, \
     TransferUploadRequestCommand, TransferDataCommand, TransferFileDataCommand, PartialLockCommand, TimeRequestCommand
@@ -54,26 +56,42 @@
         'DskS': 'dkey-state',
         'FtbP': 'fade-to-black',
         'FtbS': 'fade-to-black-state',
         'ColV': 'color-generator',
         'AuxS': 'aux-output-source',
         'MPfe': 'mediaplayer-file-info',
         'MPCE': 'mediaplayer-selected',
+        'MPSp': 'mediaplayer-space',
+        'MPCS': 'mediaplayer-clip-source',
+        'MPAS': 'mediaplayer-audio-source',
+        'RCPS': 'mediaplayer-clip-status',
         'AMMO': 'audio-mixer-master-properties',
         'AMmO': 'audio-mixer-monitor-properties',
         'AMTl': 'audio-mixer-tally',
         'FASP': 'fairlight-strip-properties',
         'FAMP': 'fairlight-master-properties',
+        'FMPP': 'fairlight-properties',
         'FMHP': 'fairlight-headphones',
         'FAMS': 'fairlight-solo',
+        'AIXP': 'fairlight-expander-properties',
+        'AICP': 'fairlight-compressor-properties',
+        'AILP': 'fairlight-limiter-properties',
+        'MOCP': 'fairlight-master-compressor-properties',
+        'AMLP': 'fairlight-master-limiter-properties',
+        'ATMP': 'talkback-mixer-properties',
+        'TMIP': 'talkback-mixer-input-properties',
+        'MMOP': 'mix-minus-output-properties',
         '_TlC': 'tally-config',
         'TlIn': 'tally-index',
         'TlSr': 'tally-source',
         'FMTl': 'fairlight-tally',
         'MPrp': 'macro-properties',
+        'MRPr': 'macro-play-status',
+        'MRcS': 'macro-record-status',
+        'CCst': 'camera-control-settings',
         'AiVM': 'auto-input-video-mode',
         'FASD': 'fairlight-strip-delete',
         'FAIP': 'fairlight-audio-input',
         'AMIP': 'audio-input',
         'RTMR': 'recording-duration',
         'RTMD': 'recording-disk',
         'RTMS': 'recording-status',
@@ -81,14 +99,15 @@
         'SRSU': 'streaming-service',
         'STAB': 'streaming-audio-bitrate',
         'StRS': 'streaming-status',
         'SRST': 'streaming-time',
         'SRSS': 'streaming-stats',
         'SAth': 'streaming-authentication',
         'AEBP': 'atem-eq-band-properties',
+        'AMBP': 'atem-master-eq-band-properties',
         'MvPr': 'multiviewer-properties',
         'MvIn': 'multiviewer-input',
         'VuMC': 'multiviewer-vu',
         'VuMo': 'multiviewer-vu-opacity',
         'SaMw': 'multiviewer-safe-area',
         'LKOB': 'lock-obtained',
         'FTDa': 'file-transfer-data',
@@ -97,14 +116,24 @@
         'FTDC': 'file-transfer-data-complete',
         'FTCD': 'file-transfer-continue-data',
         'AMLv': 'audio-meter-levels',
         'FMLv': 'fairlight-meter-levels',
         'FDLv': 'fairlight-master-levels',
         'CCdP': 'camera-control-data-packet',
         '*XFC': 'transfer-complete',
+        '_SSC': 'supersource-config',
+        'SSrc': 'supersource-properties',
+        'SSBP': 'supersource-box-properties',
+        'V3sl': 'sdi-3g-level',
+        'RXMS': 'hyperdeck-settings',
+        'RXCP': 'hyperdeck-status',
+        'RXSS': 'hyperdeck-storage',
+        'RXCC': 'hyperdeck-clip-count',
+        'DCPV': 'displayclock-properties',
+        'DSTV': 'displayclock-set-time',
     }
 
     FIELDNAME_UNIQUE = {
         'mixer-effect-config': struct.Struct('>B'),
         'input-properties': struct.Struct('>H'),
         'program-bus-input': struct.Struct('>B'),
         'preview-bus-input': struct.Struct('>B'),
```

### Comparing `pyatem-0.8.0/pyatem/socketqueue.py` & `pyatem-0.9.0/pyatem/socketqueue.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import queue
 import socket
 import os
 
 
 class SocketQueue(queue.Queue):
     """
```

### Comparing `pyatem-0.8.0/pyatem/test_colorspace.py` & `pyatem-0.9.0/pyatem/test_colorspace.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
+import os
 from unittest import TestCase
 import gzip
 
 import pyatem.media
 from PIL import Image
 
 
 class Test(TestCase):
 
     def setUp(self):
-        fixture = self._encode_test('fixtures/ramps.png')
+        fixtures_dir = os.environ.get('TEST_FIXTURES', os.path.join(os.path.dirname(__file__), 'fixtures'))
+        fixture = self._encode_test(os.path.join(fixtures_dir, 'ramps.png'))
         self.encoded = pyatem.media.rgb_to_atem(fixture, 1920, 1080)
 
-        with gzip.open('fixtures/ramps-atemsc.data.gz', 'rb') as handle:
+        with gzip.open(os.path.join(fixtures_dir, 'ramps-atemsc.data.gz'), 'rb') as handle:
             self.reference = handle.read()
 
     def _encode_test(self, path):
         """
         Load a test fixture image with pillow and run through the atem frame encoder without compression
         """
         im = Image.open(path)
```

### Comparing `pyatem-0.8.0/pyatem/test_media.py` & `pyatem-0.9.0/pyatem/test_media.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 from unittest import TestCase
 
 from pyatem.hexdump import hexdump
 from pyatem.media import rle_decode, rle_encode, atem_to_image, image_to_atem, rgb_to_atem
 from pyatem.mediaconvert import atem_to_rgb
```

### Comparing `pyatem-0.8.0/pyatem/test_rle.py` & `pyatem-0.9.0/pyatem/test_rle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 from unittest import TestCase
 
 from pyatem.hexdump import hexdump
 from pyatem.media import rle_decode, rle_encode
 
 
 class Test(TestCase):
```

### Comparing `pyatem-0.8.0/pyatem/transfer.py` & `pyatem-0.9.0/pyatem/transfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import hashlib
 import struct
 
 from pyatem.media import rle_encode
 
 
 class TransferTask:
```

### Comparing `pyatem-0.8.0/pyatem/transport.py` & `pyatem-0.9.0/pyatem/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import select
 import socket
 import struct
 import logging
 import time
 from queue import Queue, Empty
 import collections
@@ -403,14 +405,15 @@
 
 class UsbProtocol(BaseProtocol):
     STATE_INIT = 0
 
     PRODUCTS = {
         0xbe49: "Atem Mini",
         0xbe55: "Atem Mini Pro",
+        0xbe7c: "Atem Mini Extreme",
     }
 
     def __init__(self, port=None):
         super().__init__()
         port = port or "auto"
         self.port = port
         self.queue = Queue()
```

### Comparing `pyatem-0.8.0/pyatem/videohub.py` & `pyatem-0.9.0/pyatem/videohub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2021 - 2022, Martijn Braam and the OpenAtem contributors
+# SPDX-License-Identifier: LGPL-3.0-only
 import socket
 
 
 class VideoHub:
     _SECTION_UNKNOWN = 0
     _SECTION_PREAMBLE = 1
     _SECTION_DEVICE = 2
```

### Comparing `pyatem-0.8.0/pyatem.egg-info/PKG-INFO` & `pyatem-0.9.0/pyatem.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: pyatem
-Version: 0.8.0
+Version: 0.9.0
 Summary: Library implementing the Blackmagic Design Atem switcher protocol
 Home-page: https://git.sr.ht/~martijnbraam/pyatem
 Author: Martijn Braam
 Author-email: martijn@brixit.nl
 License: LGPL3
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
+License-File: LICENSE-gpl3.txt
+License-File: LICENSE-lgpl3.txt
 
 PyATEM
 ======
 
 Library implementing the ATEM video switcher protocol and a GTK3.0 application
 
 ![Screenshot of the control application](https://brixitcdn.net/metainfo/openswitcher.png)
@@ -76,15 +82,15 @@
 
     python3 -m openswitcher_proxy --config /etc/myconfigfile.toml
 
 Or if the software installed it can be started using the launcher script::
 
     openswitcher-proxy --config /etc/myconfigfile.toml
 
-The default config location is /etc/openswitcher/proxy.conf if not specified. Here's an example config:
+The default config location is /etc/openswitcher/proxy.toml if not specified. Here's an example config:
 
     [[hardware]]
     id = "mini"
     label = "Atem Mini"
     address = "192.168.2.84"
 
     [[hardware]]
@@ -113,8 +119,7 @@
 
 
 Translations
 ------------
 
 The main language for the software is english, the translation for the project happens on
 https://hosted.weblate.org/projects/openswitcher
-
```

