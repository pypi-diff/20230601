# Comparing `tmp/portage-3.0.47.tar.gz` & `tmp/portage-3.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portage-3.0.47.tar", last modified: Sun Apr 30 04:11:56 2023, max compression
+gzip compressed data, was "portage-3.0.48.tar", last modified: Thu Jun  1 01:26:11 2023, max compression
```

## Comparing `portage-3.0.47.tar` & `portage-3.0.48.tar`

### file list

```diff
@@ -1,942 +1,944 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:35.927469 portage-3.0.47/.portage_not_installed
--rw-r--r--   0 root         (0) root         (0)     6944 2023-03-21 03:50:18.057424 portage-3.0.47/DEVELOPING
--rw-r--r--   0 root         (0) root         (0)    18092 2021-11-12 08:15:35.927469 portage-3.0.47/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4474 2023-04-30 04:11:56.749078 portage-3.0.47/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1864 2021-11-12 08:15:35.927469 portage-3.0.47/TEST-NOTES
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.722411 portage-3.0.47/bin/
--rwxr-xr-x   0 root         (0) root         (0)     3262 2023-03-21 23:52:40.754842 portage-3.0.47/bin/archive-conf
--rwxr-xr-x   0 root         (0) root         (0)     1443 2023-04-07 10:38:37.709109 portage-3.0.47/bin/bashrc-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)     4457 2023-03-21 23:52:40.598174 portage-3.0.47/bin/binhost-snapshot
--rwxr-xr-x   0 root         (0) root         (0)       51 2021-11-12 08:15:35.934136 portage-3.0.47/bin/cgroup-release-agent
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.934136 portage-3.0.47/bin/chmod-lite -> ebuild-pyhelper
--rwxr-xr-x   0 root         (0) root         (0)      951 2023-03-21 03:35:23.553538 portage-3.0.47/bin/chmod-lite.py
--rwxr-xr-x   0 root         (0) root         (0)     5891 2023-03-21 03:35:23.553538 portage-3.0.47/bin/chpathtool.py
--rwxr-xr-x   0 root         (0) root         (0)     1421 2023-03-21 03:35:23.553538 portage-3.0.47/bin/clean_locks
--rwxr-xr-x   0 root         (0) root         (0)    19951 2023-04-29 04:41:18.541267 portage-3.0.47/bin/dispatch-conf
--rwxr-xr-x   0 root         (0) root         (0)     8895 2023-04-29 04:41:16.537917 portage-3.0.47/bin/dohtml.py
--rwxr-xr-x   0 root         (0) root         (0)    20007 2023-04-07 10:38:37.709109 portage-3.0.47/bin/doins.py
--rwxr-xr-x   0 root         (0) root         (0)     6078 2023-04-07 10:38:37.709109 portage-3.0.47/bin/eapi.sh
--rwxr-xr-x   0 root         (0) root         (0)     4310 2023-04-07 10:38:37.709109 portage-3.0.47/bin/eapi7-ver-funcs.sh
--rwxr-xr-x   0 root         (0) root         (0)    15468 2023-03-21 23:52:40.598174 portage-3.0.47/bin/ebuild
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/bsd/
--rwxr-xr-x   0 root         (0) root         (0)      639 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/bsd/sed
--rwxr-xr-x   0 root         (0) root         (0)      200 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/die
--rwxr-xr-x   0 root         (0) root         (0)     1049 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dobin
--rwxr-xr-x   0 root         (0) root         (0)      515 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doconfd
--rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-helpers/dodir
--rwxr-xr-x   0 root         (0) root         (0)      885 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dodoc
--rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doenvd
--rwxr-xr-x   0 root         (0) root         (0)      952 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doexe
--rwxr-xr-x   0 root         (0) root         (0)      531 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/dohard
--rwxr-xr-x   0 root         (0) root         (0)      632 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doheader
--rwxr-xr-x   0 root         (0) root         (0)      782 2022-09-10 09:45:01.063717 portage-3.0.47/bin/ebuild-helpers/dohtml
--rwxr-xr-x   0 root         (0) root         (0)      722 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/doinfo
--rwxr-xr-x   0 root         (0) root         (0)      485 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doinitd
--rwxr-xr-x   0 root         (0) root         (0)     3034 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/doins
--rwxr-xr-x   0 root         (0) root         (0)     1438 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dolib
--rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/dolib.a
--rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/dolib.so
--rwxr-xr-x   0 root         (0) root         (0)     1553 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/doman
--rwxr-xr-x   0 root         (0) root         (0)     1216 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/domo
--rwxr-xr-x   0 root         (0) root         (0)     1053 2023-04-29 04:41:16.537917 portage-3.0.47/bin/ebuild-helpers/dosbin
--rwxr-xr-x   0 root         (0) root         (0)      818 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/dosed
--rwxr-xr-x   0 root         (0) root         (0)     2366 2022-09-10 09:45:01.063717 portage-3.0.47/bin/ebuild-helpers/dosym
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/eerror -> elog
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/einfo -> elog
--rwxr-xr-x   0 root         (0) root         (0)      204 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/elog
--rwxr-xr-x   0 root         (0) root         (0)      894 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/emake
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/eqawarn -> elog
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.47/bin/ebuild-helpers/ewarn -> elog
--rwxr-xr-x   0 root         (0) root         (0)      792 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-helpers/fowners
--rwxr-xr-x   0 root         (0) root         (0)      850 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/fperms
--rwxr-xr-x   0 root         (0) root         (0)      490 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/keepdir
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newbin -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newconfd -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newdoc -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newenvd -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newexe -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newheader -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newinitd -> newins
--rwxr-xr-x   0 root         (0) root         (0)     1201 2023-02-03 18:03:13.730194 portage-3.0.47/bin/ebuild-helpers/newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newlib.a -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newlib.so -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newman -> newins
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/newsbin -> newins
--rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/nonfatal
--rwxr-xr-x   0 root         (0) root         (0)      739 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/portageq
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/prepall
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/prepalldocs
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/prepallinfo
--rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.47/bin/ebuild-helpers/prepallman
--rwxr-xr-x   0 root         (0) root         (0)      383 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-helpers/prepallstrip
--rwxr-xr-x   0 root         (0) root         (0)      843 2023-04-09 06:49:46.512769 portage-3.0.47/bin/ebuild-helpers/prepinfo
--rwxr-xr-x   0 root         (0) root         (0)      364 2023-04-09 06:49:46.512769 portage-3.0.47/bin/ebuild-helpers/prepman
--rwxr-xr-x   0 root         (0) root         (0)      375 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/prepstrip
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/unprivileged/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-helpers/unprivileged/chgrp -> chown
--rwxr-xr-x   0 root         (0) root         (0)     1178 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/unprivileged/chown
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/ebuild-helpers/xattr/
--rwxr-xr-x   0 root         (0) root         (0)     1369 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ebuild-helpers/xattr/install
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.47/bin/ebuild-ipc -> ebuild-pyhelper
--rwxr-xr-x   0 root         (0) root         (0)    10684 2023-03-21 23:52:40.598174 portage-3.0.47/bin/ebuild-ipc.py
--rwxr-xr-x   0 root         (0) root         (0)      616 2022-09-10 09:45:01.057050 portage-3.0.47/bin/ebuild-pyhelper
--rwxr-xr-x   0 root         (0) root         (0)    26114 2023-03-21 03:35:23.556871 portage-3.0.47/bin/ebuild.sh
--rwxr-xr-x   0 root         (0) root         (0)     6481 2022-12-24 02:35:49.845990 portage-3.0.47/bin/ecompress
--rwxr-xr-x   0 root         (0) root         (0)     1746 2022-09-10 09:45:01.060384 portage-3.0.47/bin/ecompress-file
--rwxr-xr-x   0 root         (0) root         (0)    53990 2023-03-21 23:52:40.598174 portage-3.0.47/bin/egencache
--rwxr-xr-x   0 root         (0) root         (0)     1857 2023-03-21 03:35:23.556871 portage-3.0.47/bin/emaint
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-03-21 23:52:40.598174 portage-3.0.47/bin/emerge
--rwxr-xr-x   0 root         (0) root         (0)    18798 2023-04-09 07:25:51.408246 portage-3.0.47/bin/emerge-webrsync
--rwxr-xr-x   0 root         (0) root         (0)      634 2022-09-10 09:45:01.053717 portage-3.0.47/bin/emirrordist
--rwxr-xr-x   0 root         (0) root         (0)     1048 2023-03-21 03:35:23.556871 portage-3.0.47/bin/env-update
--rwxr-xr-x   0 root         (0) root         (0)    17296 2023-03-21 03:35:23.556871 portage-3.0.47/bin/estrip
--rwxr-xr-x   0 root         (0) root         (0)    23454 2023-03-21 03:50:18.057424 portage-3.0.47/bin/etc-update
--rwxr-xr-x   0 root         (0) root         (0)     6045 2023-03-21 03:35:23.556871 portage-3.0.47/bin/filter-bash-environment.py
--rwxr-xr-x   0 root         (0) root         (0)     1601 2023-03-21 03:35:23.556871 portage-3.0.47/bin/fixpackages
--rwxr-xr-x   0 root         (0) root         (0)    15636 2023-03-21 23:52:40.601508 portage-3.0.47/bin/glsa-check
--rwxr-xr-x   0 root         (0) root         (0)     2166 2023-03-21 03:35:23.556871 portage-3.0.47/bin/gpkg-helper.py
--rwxr-xr-x   0 root         (0) root         (0)     2476 2022-12-24 02:35:49.845990 portage-3.0.47/bin/gpkg-sign
--rwxr-xr-x   0 root         (0) root         (0)     2918 2023-04-07 10:38:37.709109 portage-3.0.47/bin/helper-functions.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/install-qa-check.d/
--rwxr-xr-x   0 root         (0) root         (0)      444 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/05double-D
--rwxr-xr-x   0 root         (0) root         (0)     4302 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/05prefix
--rwxr-xr-x   0 root         (0) root         (0)     5559 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/10executable-issues
--rwxr-xr-x   0 root         (0) root         (0)     3591 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/10ignored-flags
--rwxr-xr-x   0 root         (0) root         (0)      406 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/20deprecated-directories
--rwxr-xr-x   0 root         (0) root         (0)      835 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/20runtime-directories
--rwxr-xr-x   0 root         (0) root         (0)     3306 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60bash-completion
--rwxr-xr-x   0 root         (0) root         (0)     1443 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60openrc
--rwxr-xr-x   0 root         (0) root         (0)     5508 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60pkgconfig
--rwxr-xr-x   0 root         (0) root         (0)      668 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60pngfix
--rwxr-xr-x   0 root         (0) root         (0)      687 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60systemd
--rwxr-xr-x   0 root         (0) root         (0)      442 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/60udev
--rwxr-xr-x   0 root         (0) root         (0)     5556 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/80libraries
--rwxr-xr-x   0 root         (0) root         (0)     1417 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/80multilib-strict
--rwxr-xr-x   0 root         (0) root         (0)     1918 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90bad-bin-group-write
--rwxr-xr-x   0 root         (0) root         (0)     1566 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90bad-bin-owner
--rwxr-xr-x   0 root         (0) root         (0)      654 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90cmake-warnings
--rwxr-xr-x   0 root         (0) root         (0)     3333 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90config-impl-decl
--rwxr-xr-x   0 root         (0) root         (0)     1277 2023-04-23 20:49:21.036042 portage-3.0.47/bin/install-qa-check.d/90cython-dep
--rwxr-xr-x   0 root         (0) root         (0)     8300 2023-04-09 06:49:46.512769 portage-3.0.47/bin/install-qa-check.d/90gcc-warnings
--rwxr-xr-x   0 root         (0) root         (0)     1042 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/90world-writable
--rwxr-xr-x   0 root         (0) root         (0)     1518 2023-04-07 10:38:37.709109 portage-3.0.47/bin/install-qa-check.d/95empty-dirs
--rwxr-xr-x   0 root         (0) root         (0)     6314 2023-03-21 23:52:40.601508 portage-3.0.47/bin/install.py
--rwxr-xr-x   0 root         (0) root         (0)    18552 2023-04-07 10:38:37.712442 portage-3.0.47/bin/isolated-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)      903 2023-03-21 03:35:23.553538 portage-3.0.47/bin/lock-helper.py
--rwxr-xr-x   0 root         (0) root         (0)    20244 2023-04-09 06:49:46.512769 portage-3.0.47/bin/misc-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)    34584 2023-04-29 04:41:16.537917 portage-3.0.47/bin/phase-functions.sh
--rwxr-xr-x   0 root         (0) root         (0)    33858 2023-04-29 04:41:16.537917 portage-3.0.47/bin/phase-helpers.sh
--rwxr-xr-x   0 root         (0) root         (0)     5723 2023-04-07 10:38:37.712442 portage-3.0.47/bin/pid-ns-init
--rwxr-xr-x   0 root         (0) root         (0)    51197 2023-03-21 23:52:40.601508 portage-3.0.47/bin/portageq
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/postinst-qa-check.d/
--rwxr-xr-x   0 root         (0) root         (0)     5236 2023-04-07 10:38:37.712442 portage-3.0.47/bin/postinst-qa-check.d/50xdg-utils
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/bin/preinst-qa-check.d/
-lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.947469 portage-3.0.47/bin/preinst-qa-check.d/50xdg-utils -> ../postinst-qa-check.d/50xdg-utils
--rwxr-xr-x   0 root         (0) root         (0)    16731 2023-03-21 23:52:40.601508 portage-3.0.47/bin/quickpkg
--rwxr-xr-x   0 root         (0) root         (0)     4992 2023-03-21 03:35:23.556871 portage-3.0.47/bin/regenworld
--rwxr-xr-x   0 root         (0) root         (0)     4535 2023-04-29 04:41:16.541251 portage-3.0.47/bin/save-ebuild-env.sh
--rwxr-xr-x   0 root         (0) root         (0)     1339 2022-09-10 09:45:01.060384 portage-3.0.47/bin/shelve-utils
--rwxr-xr-x   0 root         (0) root         (0)     8140 2023-04-07 10:38:37.712442 portage-3.0.47/bin/socks5-server.py
--rwxr-xr-x   0 root         (0) root         (0)     4784 2023-03-21 23:52:40.601508 portage-3.0.47/bin/xattr-helper.py
--rwxr-xr-x   0 root         (0) root         (0)     1825 2023-03-21 03:35:23.550205 portage-3.0.47/bin/xpak-helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/cnf/
--rw-r--r--   0 root         (0) root         (0)     1718 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.alpha.diff
--rw-r--r--   0 root         (0) root         (0)     2319 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.amd64-fbsd.diff
--rw-r--r--   0 root         (0) root         (0)     2309 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.amd64.diff
--rw-r--r--   0 root         (0) root         (0)     1592 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.arm.diff
--rw-r--r--   0 root         (0) root         (0)     1580 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.arm64.diff
--rw-r--r--   0 root         (0) root         (0)     2465 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.hppa.diff
--rw-r--r--   0 root         (0) root         (0)      663 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.ia64.diff
--rw-r--r--   0 root         (0) root         (0)     2192 2023-03-21 03:35:23.550205 portage-3.0.47/cnf/make.conf.example.loong.diff
--rw-r--r--   0 root         (0) root         (0)      900 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.m68k.diff
--rw-r--r--   0 root         (0) root         (0)     1383 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.mips.diff
--rw-r--r--   0 root         (0) root         (0)     3541 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.ppc.diff
--rw-r--r--   0 root         (0) root         (0)     2361 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.ppc64.diff
--rw-r--r--   0 root         (0) root         (0)     2332 2022-09-10 09:44:56.963689 portage-3.0.47/cnf/make.conf.example.riscv.diff
--rw-r--r--   0 root         (0) root         (0)      656 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.s390.diff
--rw-r--r--   0 root         (0) root         (0)     1257 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.sh.diff
--rw-r--r--   0 root         (0) root         (0)      728 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.sparc-fbsd.diff
--rw-r--r--   0 root         (0) root         (0)     2129 2021-12-09 09:19:33.760140 portage-3.0.47/cnf/make.conf.example.sparc.diff
--rw-r--r--   0 root         (0) root         (0)     2507 2021-12-09 09:19:33.763473 portage-3.0.47/cnf/make.conf.example.x86-fbsd.diff
--rw-r--r--   0 root         (0) root         (0)     3759 2021-12-09 09:19:33.763473 portage-3.0.47/cnf/make.conf.example.x86.diff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/api/
--rw-r--r--   0 root         (0) root         (0)     1141 2021-11-12 08:15:35.954135 portage-3.0.47/doc/api/Makefile
--rw-r--r--   0 root         (0) root         (0)     2372 2023-03-21 03:35:23.550205 portage-3.0.47/doc/api/conf.py
--rw-r--r--   0 root         (0) root         (0)      217 2021-11-12 08:15:35.954135 portage-3.0.47/doc/api/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/config/
--rw-r--r--   0 root         (0) root         (0)     1900 2021-11-12 08:15:35.954135 portage-3.0.47/doc/config/bashrc.docbook
--rw-r--r--   0 root         (0) root         (0)    26214 2021-11-12 08:15:35.954135 portage-3.0.47/doc/config/sets.docbook
--rw-r--r--   0 root         (0) root         (0)       85 2021-11-12 08:15:35.954135 portage-3.0.47/doc/config.docbook
--rw-r--r--   0 root         (0) root         (0)      257 2021-11-12 08:15:35.954135 portage-3.0.47/doc/custom.xsl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/dependency_resolution/
--rw-r--r--   0 root         (0) root         (0)     3281 2021-11-12 08:15:35.957468 portage-3.0.47/doc/dependency_resolution/decision_making.docbook
--rw-r--r--   0 root         (0) root         (0)     4154 2021-11-12 08:15:35.957468 portage-3.0.47/doc/dependency_resolution/package_modeling.docbook
--rw-r--r--   0 root         (0) root         (0)     3451 2021-11-12 08:15:35.957468 portage-3.0.47/doc/dependency_resolution/task_scheduling.docbook
--rw-r--r--   0 root         (0) root         (0)      200 2021-11-12 08:15:35.954135 portage-3.0.47/doc/dependency_resolution.docbook
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/package/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.725745 portage-3.0.47/doc/package/ebuild/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.729078 portage-3.0.47/doc/package/ebuild/eapi/
--rw-r--r--   0 root         (0) root         (0)      487 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/0.docbook
--rw-r--r--   0 root         (0) root         (0)     1598 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/1.docbook
--rw-r--r--   0 root         (0) root         (0)     8299 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/2.docbook
--rw-r--r--   0 root         (0) root         (0)     2938 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/3.docbook
--rw-r--r--   0 root         (0) root         (0)     3112 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/4-slot-abi.docbook
--rw-r--r--   0 root         (0) root         (0)    14690 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/4.docbook
--rw-r--r--   0 root         (0) root         (0)     8044 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/eapi/5.docbook
--rw-r--r--   0 root         (0) root         (0)     1725 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/helper_functions.docbook
--rw-r--r--   0 root         (0) root         (0)     2780 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package/ebuild/phases.docbook
--rw-r--r--   0 root         (0) root         (0)      364 2022-09-10 09:45:01.060384 portage-3.0.47/doc/package/ebuild.docbook
--rw-r--r--   0 root         (0) root         (0)       76 2021-11-12 08:15:35.957468 portage-3.0.47/doc/package.docbook
--rw-r--r--   0 root         (0) root         (0)     2194 2022-09-10 09:45:01.060384 portage-3.0.47/doc/portage.docbook
--rw-r--r--   0 root         (0) root         (0)    19579 2021-11-12 08:15:35.960802 portage-3.0.47/doc/qa.docbook
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.712411 portage-3.0.47/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.729078 portage-3.0.47/lib/_emerge/
--rw-r--r--   0 root         (0) root         (0)      816 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/AbstractDepPriority.py
--rw-r--r--   0 root         (0) root         (0)    18460 2023-03-21 03:50:18.057424 portage-3.0.47/lib/_emerge/AbstractEbuildProcess.py
--rw-r--r--   0 root         (0) root         (0)     3723 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/AbstractPollTask.py
--rw-r--r--   0 root         (0) root         (0)    10471 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/AsynchronousLock.py
--rw-r--r--   0 root         (0) root         (0)     7090 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/AsynchronousTask.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/AtomArg.py
--rw-r--r--   0 root         (0) root         (0)    21241 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/Binpkg.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgEnvExtractor.py
--rw-r--r--   0 root         (0) root         (0)     5494 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgExtractorAsync.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgFetcher.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgPrefetcher.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/BinpkgVerifier.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/Blocker.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/BlockerCache.py
--rw-r--r--   0 root         (0) root         (0)     5325 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/BlockerDB.py
--rw-r--r--   0 root         (0) root         (0)      355 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/BlockerDepPriority.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/CompositeTask.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/DepPriority.py
--rw-r--r--   0 root         (0) root         (0)     1564 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/DepPriorityNormalRange.py
--rw-r--r--   0 root         (0) root         (0)     3647 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/DepPrioritySatisfiedRange.py
--rw-r--r--   0 root         (0) root         (0)      878 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/Dependency.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/DependencyArg.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildBinpkg.py
--rw-r--r--   0 root         (0) root         (0)    23204 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildBuild.py
--rw-r--r--   0 root         (0) root         (0)     5749 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildBuildDir.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildExecuter.py
--rw-r--r--   0 root         (0) root         (0)    14395 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildFetcher.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildFetchonly.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/EbuildIpcDaemon.py
--rw-r--r--   0 root         (0) root         (0)     3258 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/EbuildMerge.py
--rw-r--r--   0 root         (0) root         (0)     7597 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/EbuildMetadataPhase.py
--rw-r--r--   0 root         (0) root         (0)    22622 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildPhase.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildProcess.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/EbuildSpawnProcess.py
--rw-r--r--   0 root         (0) root         (0)    12786 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/FakeVartree.py
--rw-r--r--   0 root         (0) root         (0)     1774 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/FifoIpcDaemon.py
--rw-r--r--   0 root         (0) root         (0)     9113 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/JobStatusDisplay.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/MergeListItem.py
--rw-r--r--   0 root         (0) root         (0)     6121 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/MetadataRegen.py
--rw-r--r--   0 root         (0) root         (0)     2424 2022-09-10 09:45:01.063717 portage-3.0.47/lib/_emerge/MiscFunctionsProcess.py
--rw-r--r--   0 root         (0) root         (0)    31019 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/Package.py
--rw-r--r--   0 root         (0) root         (0)      735 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/PackageArg.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PackageMerge.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PackagePhase.py
--rw-r--r--   0 root         (0) root         (0)     5870 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PackageUninstall.py
--rw-r--r--   0 root         (0) root         (0)     4651 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/PackageVirtualDbapi.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PipeReader.py
--rw-r--r--   0 root         (0) root         (0)     6630 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/PollScheduler.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/ProgressHandler.py
--rw-r--r--   0 root         (0) root         (0)     1227 2022-09-10 09:44:56.967023 portage-3.0.47/lib/_emerge/RootConfig.py
--rw-r--r--   0 root         (0) root         (0)    85615 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/Scheduler.py
--rw-r--r--   0 root         (0) root         (0)     2648 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SequentialTaskQueue.py
--rw-r--r--   0 root         (0) root         (0)      421 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SetArg.py
--rw-r--r--   0 root         (0) root         (0)    10190 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SpawnProcess.py
--rw-r--r--   0 root         (0) root         (0)     3167 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/SubProcess.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/Task.py
--rw-r--r--   0 root         (0) root         (0)     1538 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/TaskSequence.py
--rw-r--r--   0 root         (0) root         (0)      455 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/UninstallFailure.py
--rw-r--r--   0 root         (0) root         (0)     1326 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/UnmergeDepPriority.py
--rw-r--r--   0 root         (0) root         (0)     3555 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/UseFlagDisplay.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/UserQuery.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.977468 portage-3.0.47/lib/_emerge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1165 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/_find_deep_system_runtime_deps.py
--rw-r--r--   0 root         (0) root         (0)      442 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/_flush_elog_mod_echo.py
--rw-r--r--   0 root         (0) root         (0)   149373 2023-03-21 03:50:18.060757 portage-3.0.47/lib/_emerge/actions.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/chk_updated_cfg_files.py
--rw-r--r--   0 root         (0) root         (0)      498 2022-09-10 09:44:56.963689 portage-3.0.47/lib/_emerge/clear_caches.py
--rw-r--r--   0 root         (0) root         (0)      586 2023-02-03 18:03:13.733528 portage-3.0.47/lib/_emerge/countdown.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/create_depgraph_params.py
--rw-r--r--   0 root         (0) root         (0)     5191 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/create_world_atom.py
--rw-r--r--   0 root         (0) root         (0)   499558 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/depgraph.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/emergelog.py
--rw-r--r--   0 root         (0) root         (0)      958 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/getloadavg.py
--rw-r--r--   0 root         (0) root         (0)     3425 2022-09-10 09:44:56.970356 portage-3.0.47/lib/_emerge/help.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/is_valid_package_atom.py
--rw-r--r--   0 root         (0) root         (0)    42164 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/main.py
--rw-r--r--   0 root         (0) root         (0)     5614 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/post_emerge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.729078 portage-3.0.47/lib/_emerge/resolver/
--rw-r--r--   0 root         (0) root         (0)     3198 2022-09-10 09:44:56.970356 portage-3.0.47/lib/_emerge/resolver/DbapiProvidesIndex.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.980801 portage-3.0.47/lib/_emerge/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11328 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/backtracking.py
--rw-r--r--   0 root         (0) root         (0)    11932 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/circular_dependency.py
--rw-r--r--   0 root         (0) root         (0)    39548 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/output.py
--rw-r--r--   0 root         (0) root         (0)    20756 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/output_helpers.py
--rw-r--r--   0 root         (0) root         (0)    15636 2023-03-21 03:35:23.550205 portage-3.0.47/lib/_emerge/resolver/package_tracker.py
--rw-r--r--   0 root         (0) root         (0)    59893 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/resolver/slot_collision.py
--rw-r--r--   0 root         (0) root         (0)    20976 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/search.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/show_invalid_depstring_notice.py
--rw-r--r--   0 root         (0) root         (0)     3196 2023-03-21 03:35:23.553538 portage-3.0.47/lib/_emerge/stdout_spinner.py
--rw-r--r--   0 root         (0) root         (0)    26564 2023-03-21 03:35:23.556871 portage-3.0.47/lib/_emerge/unmerge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/
--rw-r--r--   0 root         (0) root         (0)    25908 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/_compat_upgrade/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.007468 portage-3.0.47/lib/portage/_compat_upgrade/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/_compat_upgrade/binpkg_compression.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_compat_upgrade/binpkg_multi_instance.py
--rw-r--r--   0 root         (0) root         (0)     4288 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_compat_upgrade/default_locations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/_emirrordist/
--rw-r--r--   0 root         (0) root         (0)     5376 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/Config.py
--rw-r--r--   0 root         (0) root         (0)     7223 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/ContentDB.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/DeletionIterator.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_emirrordist/DeletionTask.py
--rw-r--r--   0 root         (0) root         (0)    11176 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_emirrordist/FetchIterator.py
--rw-r--r--   0 root         (0) root         (0)    25443 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_emirrordist/FetchTask.py
--rw-r--r--   0 root         (0) root         (0)     9145 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_emirrordist/MirrorDistTask.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.007468 portage-3.0.47/lib/portage/_emirrordist/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16082 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/_emirrordist/main.py
--rw-r--r--   0 root         (0) root         (0)    10222 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_global_updates.py
--rw-r--r--   0 root         (0) root         (0)     2550 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/_legacy_globals.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_selinux.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/_sets/
--rw-r--r--   0 root         (0) root         (0)     1719 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/ProfilePackageSet.py
--rw-r--r--   0 root         (0) root         (0)    14268 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/_sets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8205 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/base.py
--rw-r--r--   0 root         (0) root         (0)    22035 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/dbapi.py
--rw-r--r--   0 root         (0) root         (0)    15573 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/files.py
--rw-r--r--   0 root         (0) root         (0)     3603 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/_sets/libs.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/profiles.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/security.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/_sets/shell.py
--rw-r--r--   0 root         (0) root         (0)     2576 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/binpkg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/binrepo/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.014134 portage-3.0.47/lib/portage/binrepo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4554 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/binrepo/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/cache/
--rw-r--r--   0 root         (0) root         (0)      101 2021-11-12 08:15:36.014134 portage-3.0.47/lib/portage/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3167 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/anydbm.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/cache_errors.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/ebuild_xattr.py
--rw-r--r--   0 root         (0) root         (0)     5286 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/flat_hash.py
--rw-r--r--   0 root         (0) root         (0)     3197 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/fs_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/cache/index/
--rw-r--r--   0 root         (0) root         (0)      562 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/index/IndexStreamIterator.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.017468 portage-3.0.47/lib/portage/cache/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/index/pkg_desc_index.py
--rw-r--r--   0 root         (0) root         (0)    11957 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/mappings.py
--rw-r--r--   0 root         (0) root         (0)     5844 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/metadata.py
--rw-r--r--   0 root         (0) root         (0)    11820 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/sql_template.py
--rw-r--r--   0 root         (0) root         (0)    13390 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/cache/sqlite.py
--rw-r--r--   0 root         (0) root         (0)    13272 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/template.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/cache/volatile.py
--rw-r--r--   0 root         (0) root         (0)    16566 2023-04-07 09:45:44.114534 portage-3.0.47/lib/portage/checksum.py
--rw-r--r--   0 root         (0) root         (0)     8879 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/const.py
--rw-r--r--   0 root         (0) root         (0)    11470 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/cvstree.py
--rw-r--r--   0 root         (0) root         (0)    11537 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/dbapi/
--rw-r--r--   0 root         (0) root         (0)      643 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/dbapi/DummyTree.py
--rw-r--r--   0 root         (0) root         (0)     5690 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dbapi/IndexedPortdb.py
--rw-r--r--   0 root         (0) root         (0)     3743 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/dbapi/IndexedVardb.py
--rw-r--r--   0 root         (0) root         (0)     2991 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dbapi/_ContentsCaseSensitivityManager.py
--rw-r--r--   0 root         (0) root         (0)    10128 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/dbapi/_MergeProcess.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dbapi/_SyncfsProcess.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dbapi/_VdbMetadataDelta.py
--rw-r--r--   0 root         (0) root         (0)    16769 2023-04-09 06:49:46.516103 portage-3.0.47/lib/portage/dbapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2545 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/dbapi/_expand_new_virt.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dbapi/_similar_name_search.py
--rw-r--r--   0 root         (0) root         (0)    90388 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/bintree.py
--rw-r--r--   0 root         (0) root         (0)     4184 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/dbapi/cpv_expand.py
--rw-r--r--   0 root         (0) root         (0)     1889 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/dbapi/dep_expand.py
--rw-r--r--   0 root         (0) root         (0)    64264 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/porttree.py
--rw-r--r--   0 root         (0) root         (0)   252193 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/vartree.py
--rw-r--r--   0 root         (0) root         (0)     7587 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dbapi/virtual.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/dep/
--rw-r--r--   0 root         (0) root         (0)   107693 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/_dnf.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/_slot_operator.py
--rw-r--r--   0 root         (0) root         (0)    42498 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/dep_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/dep/soname/
--rw-r--r--   0 root         (0) root         (0)     1925 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/dep/soname/SonameAtom.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.030801 portage-3.0.47/lib/portage/dep/soname/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5080 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/dep/soname/multilib_category.py
--rw-r--r--   0 root         (0) root         (0)     1491 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/dep/soname/parse.py
--rw-r--r--   0 root         (0) root         (0)    14093 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/dispatch_conf.py
--rw-r--r--   0 root         (0) root         (0)     8092 2023-01-10 15:35:29.386865 portage-3.0.47/lib/portage/eapi.py
--rw-r--r--   0 root         (0) root         (0)     6757 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/eclass_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/elog/
--rw-r--r--   0 root         (0) root         (0)     6879 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/elog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      613 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/elog/filtering.py
--rw-r--r--   0 root         (0) root         (0)     6065 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/elog/messages.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-02-03 18:03:13.736861 portage-3.0.47/lib/portage/elog/mod_custom.py
--rw-r--r--   0 root         (0) root         (0)     2204 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/elog/mod_echo.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/elog/mod_mail.py
--rw-r--r--   0 root         (0) root         (0)     3183 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_mail_summary.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_save.py
--rw-r--r--   0 root         (0) root         (0)     3580 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_save_summary.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/elog/mod_syslog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/
--rw-r--r--   0 root         (0) root         (0)      163 2021-11-12 08:15:36.037467 portage-3.0.47/lib/portage/emaint/__init__.py
--rw-r--r--   0 root         (0) root         (0)      762 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/defaults.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/
--rw-r--r--   0 root         (0) root         (0)      173 2021-11-12 08:15:36.037467 portage-3.0.47/lib/portage/emaint/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/binhost/
--rw-r--r--   0 root         (0) root         (0)      524 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/binhost/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6358 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/binhost/binhost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/config/
--rw-r--r--   0 root         (0) root         (0)      534 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/config/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/logs/
--rw-r--r--   0 root         (0) root         (0)     1629 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/logs/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.732411 portage-3.0.47/lib/portage/emaint/modules/merges/
--rw-r--r--   0 root         (0) root         (0)     1417 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/merges/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9834 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/emaint/modules/merges/merges.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/move/
--rw-r--r--   0 root         (0) root         (0)      851 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/move/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7693 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/move/move.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/resume/
--rw-r--r--   0 root         (0) root         (0)      566 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/resume/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/resume/resume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/sync/
--rw-r--r--   0 root         (0) root         (0)     2145 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18469 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/sync/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/emaint/modules/world/
--rw-r--r--   0 root         (0) root         (0)      502 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/emaint/modules/world/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/emaint/modules/world/world.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/env/
--rw-r--r--   0 root         (0) root         (0)       52 2021-11-12 08:15:36.044134 portage-3.0.47/lib/portage/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/env/config.py
--rw-r--r--   0 root         (0) root         (0)    10311 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/env/loaders.py
--rw-r--r--   0 root         (0) root         (0)      578 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/env/validators.py
--rw-r--r--   0 root         (0) root         (0)     6616 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/exception.py
--rw-r--r--   0 root         (0) root         (0)    31465 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/getbinpkg.py
--rw-r--r--   0 root         (0) root         (0)    31099 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/glsa.py
--rw-r--r--   0 root         (0) root         (0)     3637 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/gpg.py
--rw-r--r--   0 root         (0) root         (0)    80663 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/gpkg.py
--rw-r--r--   0 root         (0) root         (0)     1550 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/localization.py
--rw-r--r--   0 root         (0) root         (0)    28153 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/locks.py
--rw-r--r--   0 root         (0) root         (0)     6187 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/mail.py
--rw-r--r--   0 root         (0) root         (0)    31108 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/manifest.py
--rw-r--r--   0 root         (0) root         (0)     8221 2023-02-03 18:03:13.736861 portage-3.0.47/lib/portage/metadata.py
--rw-r--r--   0 root         (0) root         (0)     8568 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/module.py
--rw-r--r--   0 root         (0) root         (0)    18485 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/news.py
--rw-r--r--   0 root         (0) root         (0)    29784 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.047467 portage-3.0.47/lib/portage/package/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.47/lib/portage/package/ebuild/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/_config/
--rw-r--r--   0 root         (0) root         (0)    13005 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/package/ebuild/_config/KeywordsManager.py
--rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_config/LicenseManager.py
--rw-r--r--   0 root         (0) root         (0)    16684 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_config/LocationsManager.py
--rw-r--r--   0 root         (0) root         (0)    13915 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/MaskManager.py
--rw-r--r--   0 root         (0) root         (0)    21565 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/package/ebuild/_config/UseManager.py
--rw-r--r--   0 root         (0) root         (0)     8443 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/VirtualsManager.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.47/lib/portage/package/ebuild/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      770 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/env_var_validation.py
--rw-r--r--   0 root         (0) root         (0)     4694 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/features_set.py
--rw-r--r--   0 root         (0) root         (0)     2272 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_config/helper.py
--rw-r--r--   0 root         (0) root         (0)     9457 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/package/ebuild/_config/special_env_vars.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/_ipc/
--rw-r--r--   0 root         (0) root         (0)      829 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_ipc/ExitCommand.py
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_ipc/IpcCommand.py
--rw-r--r--   0 root         (0) root         (0)     5193 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/package/ebuild/_ipc/QueryCommand.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.054134 portage-3.0.47/lib/portage/package/ebuild/_ipc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_metadata_invalid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py
--rw-r--r--   0 root         (0) root         (0)     7859 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.057467 portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4987 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/package/ebuild/_spawn_nofetch.py
--rw-r--r--   0 root         (0) root         (0)   133992 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/config.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/package/ebuild/deprecated_profile_check.py
--rw-r--r--   0 root         (0) root         (0)     6732 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/package/ebuild/digestcheck.py
--rw-r--r--   0 root         (0) root         (0)     9424 2023-03-21 03:35:23.550205 portage-3.0.47/lib/portage/package/ebuild/digestgen.py
--rw-r--r--   0 root         (0) root         (0)   111579 2023-04-29 04:41:37.948089 portage-3.0.47/lib/portage/package/ebuild/doebuild.py
--rw-r--r--   0 root         (0) root         (0)    79658 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/package/ebuild/fetch.py
--rw-r--r--   0 root         (0) root         (0)     4689 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/package/ebuild/getmaskingreason.py
--rw-r--r--   0 root         (0) root         (0)     6556 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/package/ebuild/getmaskingstatus.py
--rw-r--r--   0 root         (0) root         (0)    19287 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/package/ebuild/prepare_build_dirs.py
--rw-r--r--   0 root         (0) root         (0)     1004 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/package/ebuild/profile_iuse.py
--rw-r--r--   0 root         (0) root         (0)    41702 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/process.py
--rw-r--r--   0 root         (0) root         (0)     1573 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/proxy/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.060800 portage-3.0.47/lib/portage/proxy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7832 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/proxy/lazyimport.py
--rw-r--r--   0 root         (0) root         (0)     2857 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/proxy/objectproxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/repository/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.47/lib/portage/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62136 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/repository/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/repository/storage/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.47/lib/portage/repository/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3951 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/repository/storage/hardlink_quarantine.py
--rw-r--r--   0 root         (0) root         (0)    10940 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/repository/storage/hardlink_rcu.py
--rw-r--r--   0 root         (0) root         (0)     1153 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/repository/storage/inplace.py
--rw-r--r--   0 root         (0) root         (0)     2675 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/repository/storage/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/
--rw-r--r--   0 root         (0) root         (0)     1589 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3015 2023-02-03 18:03:13.733528 portage-3.0.47/lib/portage/sync/config_checks.py
--rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/sync/controller.py
--rw-r--r--   0 root         (0) root         (0)      696 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/getaddrinfo_validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.067467 portage-3.0.47/lib/portage/sync/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/cvs/
--rw-r--r--   0 root         (0) root         (0)     1650 2023-02-03 18:03:13.733528 portage-3.0.47/lib/portage/sync/modules/cvs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/sync/modules/cvs/cvs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/git/
--rw-r--r--   0 root         (0) root         (0)     2722 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/sync/modules/git/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20049 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/sync/modules/git/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/mercurial/
--rw-r--r--   0 root         (0) root         (0)     1403 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/modules/mercurial/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6125 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/sync/modules/mercurial/mercurial.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/rsync/
--rw-r--r--   0 root         (0) root         (0)     1287 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/modules/rsync/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33953 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/modules/rsync/rsync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/svn/
--rw-r--r--   0 root         (0) root         (0)     1037 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/sync/modules/svn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2759 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/modules/svn/svn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/sync/modules/webrsync/
--rw-r--r--   0 root         (0) root         (0)     1650 2023-04-09 06:51:34.556710 portage-3.0.47/lib/portage/sync/modules/webrsync/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-04-09 06:51:34.716710 portage-3.0.47/lib/portage/sync/modules/webrsync/webrsync.py
--rw-r--r--   0 root         (0) root         (0)     2485 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/old_tree_timestamp.py
--rw-r--r--   0 root         (0) root         (0)    13139 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/sync/syncbase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/.gnupg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/
--rw-r--r--   0 root         (0) root         (0)     1850 2022-09-10 09:45:01.063717 portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev
--rw-r--r--   0 root         (0) root         (0)     1852 2022-09-10 09:45:01.063717 portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/
--rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key
--rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key
--rw-r--r--   0 root         (0) root         (0)     2774 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/.gnupg/pubring.kbx
--rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/.gnupg/trustdb.gpg
--rw-r--r--   0 root         (0) root         (0)    11871 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/bin/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/bin/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/bin/setup_env.py
--rw-r--r--   0 root         (0) root         (0)      547 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/bin/test_dobin.py
--rw-r--r--   0 root         (0) root         (0)      565 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/bin/test_dodir.py
--rw-r--r--   0 root         (0) root         (0)    13013 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/bin/test_doins.py
--rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/bin/test_eapi7_ver_funcs.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/bin/test_filter_bash_env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.735745 portage-3.0.47/lib/portage/tests/dbapi/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/dbapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.47/lib/portage/tests/dbapi/__test__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dbapi/test_auxdb.py
--rw-r--r--   0 root         (0) root         (0)     6521 2023-02-03 18:03:13.730194 portage-3.0.47/lib/portage/tests/dbapi/test_bintree.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dbapi/test_fakedbapi.py
--rw-r--r--   0 root         (0) root         (0)     9409 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dbapi/test_portdb_cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/dep/
--rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.077467 portage-3.0.47/lib/portage/tests/dep/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.077467 portage-3.0.47/lib/portage/tests/dep/__test__.py
--rw-r--r--   0 root         (0) root         (0)    24520 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dep/testAtom.py
--rw-r--r--   0 root         (0) root         (0)     9752 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/testCheckRequiredUse.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/testExtendedAtomDict.py
--rw-r--r--   0 root         (0) root         (0)     3769 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/testExtractAffectingUSE.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dep/testStandalone.py
--rw-r--r--   0 root         (0) root         (0)     4452 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/dep/test_best_match_to_list.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getcpv.py
--rw-r--r--   0 root         (0) root         (0)      988 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getrepo.py
--rw-r--r--   0 root         (0) root         (0)      934 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getslot.py
--rw-r--r--   0 root         (0) root         (0)     1402 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dep_getusedeps.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_dnf_convert.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_get_operator.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_get_required_use_flags.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_isjustname.py
--rw-r--r--   0 root         (0) root         (0)    11660 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_isvalidatom.py
--rw-r--r--   0 root         (0) root         (0)    11132 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_match_from_list.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_overlap_dnf.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_paren_reduce.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/dep/test_soname_atom_pickle.py
--rw-r--r--   0 root         (0) root         (0)    27656 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/dep/test_use_reduce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/ebuild/
--rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/ebuild/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/ebuild/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_array_fromfile_eof.py
--rw-r--r--   0 root         (0) root         (0)    14001 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_config.py
--rw-r--r--   0 root         (0) root         (0)     5947 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py
--rw-r--r--   0 root         (0) root         (0)     5167 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_spawn.py
--rw-r--r--   0 root         (0) root         (0)    35283 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_fetch.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_ipc_daemon.py
--rw-r--r--   0 root         (0) root         (0)     5211 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/ebuild/test_shell_quote.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/ebuild/test_spawn.py
--rw-r--r--   0 root         (0) root         (0)     4479 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/ebuild/test_use_expand_incremental.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/emerge/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/emerge/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.47/lib/portage/tests/emerge/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1877 2022-12-24 02:35:49.845990 portage-3.0.47/lib/portage/tests/emerge/test_actions.py
--rw-r--r--   0 root         (0) root         (0)    10290 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_config_protect.py
--rw-r--r--   0 root         (0) root         (0)     6335 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py
--rw-r--r--   0 root         (0) root         (0)     6615 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_emerge_slot_abi.py
--rw-r--r--   0 root         (0) root         (0)     1320 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/emerge/test_global_updates.py
--rw-r--r--   0 root         (0) root         (0)    26423 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/emerge/test_simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/env/
--rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/env/config/
--rw-r--r--   0 root         (0) root         (0)      176 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/env/config/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/env/config/test_PackageKeywordsFile.py
--rw-r--r--   0 root         (0) root         (0)      818 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/env/config/test_PackageMaskFile.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/env/config/test_PackageUseFile.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/env/config/test_PortageModulesFile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/glsa/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/glsa/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/glsa/__test__.py
--rw-r--r--   0 root         (0) root         (0)     7173 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/glsa/test_security_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/gpkg/
--rw-r--r--   0 root         (0) root         (0)      102 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/gpkg/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/gpkg/__test__.py
--rw-r--r--   0 root         (0) root         (0)    13833 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_checksum.py
--rw-r--r--   0 root         (0) root         (0)    15728 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_gpg.py
--rw-r--r--   0 root         (0) root         (0)     1899 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_update.py
--rw-r--r--   0 root         (0) root         (0)     5288 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_url.py
--rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_path.py
--rw-r--r--   0 root         (0) root         (0)     1868 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_size.py
--rw-r--r--   0 root         (0) root         (0)     3305 2022-09-20 03:21:13.396002 portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/lafilefixer/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lafilefixer/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lafilefixer/__test__.py
--rw-r--r--   0 root         (0) root         (0)     6338 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lafilefixer/test_lafilefixer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/lazyimport/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lazyimport/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.47/lib/portage/tests/lazyimport/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py
--rw-r--r--   0 root         (0) root         (0)      596 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lazyimport/test_preload_portage_submodules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/lint/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/lint/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/lint/__test__.py
--rw-r--r--   0 root         (0) root         (0)      214 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lint/metadata.py
--rw-r--r--   0 root         (0) root         (0)     2345 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/lint/test_bash_syntax.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/lint/test_compile_modules.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/lint/test_import_modules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/locks/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/locks/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/locks/__test__.py
--rw-r--r--   0 root         (0) root         (0)     7850 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/locks/test_asynchronous_lock.py
--rw-r--r--   0 root         (0) root         (0)     2763 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/locks/test_lock_nonblock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/news/
--rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/news/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/news/__test__.py
--rw-r--r--   0 root         (0) root         (0)    14363 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/news/test_NewsItem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.739078 portage-3.0.47/lib/portage/tests/process/
--rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.47/lib/portage/tests/process/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2016 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/process/test_AsyncFunction.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_PipeLogger.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_PopenProcess.py
--rw-r--r--   0 root         (0) root         (0)     2366 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_PopenProcessBlockingIO.py
--rw-r--r--   0 root         (0) root         (0)     3737 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_poll.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_spawn_fail_e2big.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-03-21 03:50:18.060757 portage-3.0.47/lib/portage/tests/process/test_spawn_warn_large_env.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/process/test_unshare_net.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/resolver/
--rw-r--r--   0 root         (0) root         (0)    42502 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/tests/resolver/ResolverPlayground.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/__test__.py
--rw-r--r--   0 root         (0) root         (0)     5585 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py
--rw-r--r--   0 root         (0) root         (0)     3747 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/resolver/soname/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/resolver/soname/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/resolver/soname/__test__.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_autounmask.py
--rw-r--r--   0 root         (0) root         (0)     1755 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_depclean.py
--rw-r--r--   0 root         (0) root         (0)     8528 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_downgrade.py
--rw-r--r--   0 root         (0) root         (0)     3840 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_or_choices.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_reinstall.py
--rw-r--r--   0 root         (0) root         (0)     3338 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_skip_update.py
--rw-r--r--   0 root         (0) root         (0)    12877 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_update.py
--rw-r--r--   0 root         (0) root         (0)     2944 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_soname_provided.py
--rw-r--r--   0 root         (0) root         (0)     2778 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfiable.py
--rw-r--r--   0 root         (0) root         (0)     3354 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfied.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py
--rw-r--r--   0 root         (0) root         (0)    28432 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_binpkg_use.py
--rw-r--r--   0 root         (0) root         (0)     2176 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_keep_keywords.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_multilib_use.py
--rw-r--r--   0 root         (0) root         (0)     1279 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_parent.py
--rw-r--r--   0 root         (0) root         (0)     2573 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_backtrack.py
--rw-r--r--   0 root         (0) root         (0)     3743 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_breakage.py
--rw-r--r--   0 root         (0) root         (0)     1830 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py
--rw-r--r--   0 root         (0) root         (0)     5786 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_backtracking.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_bdeps.py
--rw-r--r--   0 root         (0) root         (0)     4927 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py
--rw-r--r--   0 root         (0) root         (0)     4231 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_blocker.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_changed_deps.py
--rw-r--r--   0 root         (0) root         (0)     7899 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_circular_choices.py
--rw-r--r--   0 root         (0) root         (0)     3341 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_circular_choices_rust.py
--rw-r--r--   0 root         (0) root         (0)     4832 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_circular_dependencies.py
--rw-r--r--   0 root         (0) root         (0)     4948 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_complete_graph.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py
--rw-r--r--   0 root         (0) root         (0)     9959 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_depclean.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_depclean_order.py
--rw-r--r--   0 root         (0) root         (0)     2443 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_depclean_slot_unavailable.py
--rw-r--r--   0 root         (0) root         (0)    13128 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_depth.py
--rw-r--r--   0 root         (0) root         (0)     3329 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_disjunctive_depend_order.py
--rw-r--r--   0 root         (0) root         (0)     9983 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_eapi.py
--rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_features_test_use.py
--rw-r--r--   0 root         (0) root         (0)     3379 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py
--rw-r--r--   0 root         (0) root         (0)     3457 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/resolver/test_installkernel.py
--rw-r--r--   0 root         (0) root         (0)    11063 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_keywords.py
--rw-r--r--   0 root         (0) root         (0)    31088 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_merge_order.py
--rw-r--r--   0 root         (0) root         (0)     1234 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_multirepo.py
--rw-r--r--   0 root         (0) root         (0)     1772 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_multislot.py
--rw-r--r--   0 root         (0) root         (0)     1554 2022-09-10 09:44:56.963689 portage-3.0.47/lib/portage/tests/resolver/test_old_dep_chain_display.py
--rw-r--r--   0 root         (0) root         (0)     1142 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps.py
--rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_circular.py
--rw-r--r--   0 root         (0) root         (0)     5933 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_ideps.py
--rw-r--r--   0 root         (0) root         (0)     2552 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_minimal.py
--rw-r--r--   0 root         (0) root         (0)    25072 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_or_choices.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_or_downgrade_installed.py
--rw-r--r--   0 root         (0) root         (0)     6850 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_or_upgrade_installed.py
--rw-r--r--   0 root         (0) root         (0)     3911 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_output.py
--rw-r--r--   0 root         (0) root         (0)     9049 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_package_tracker.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_profile_default_eapi.py
--rw-r--r--   0 root         (0) root         (0)     3353 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_profile_package_set.py
--rw-r--r--   0 root         (0) root         (0)     6911 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     2409 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py
--rw-r--r--   0 root         (0) root         (0)    11792 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_required_use.py
--rw-r--r--   0 root         (0) root         (0)     2640 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_simple.py
--rw-r--r--   0 root         (0) root         (0)    18128 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_abi.py
--rw-r--r--   0 root         (0) root         (0)     8790 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_abi_downgrade.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_change_without_revbump.py
--rw-r--r--   0 root         (0) root         (0)    13393 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_collisions.py
--rw-r--r--   0 root         (0) root         (0)     1990 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     1432 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_mask_update.py
--rw-r--r--   0 root         (0) root         (0)    14826 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     7910 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py
--rw-r--r--   0 root         (0) root         (0)     2579 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update.py
--rw-r--r--   0 root         (0) root         (0)     2491 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update_virt.py
--rw-r--r--   0 root         (0) root         (0)     5024 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_autounmask.py
--rw-r--r--   0 root         (0) root         (0)     7642 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_bdeps.py
--rw-r--r--   0 root         (0) root         (0)     4350 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_complete_graph.py
--rw-r--r--   0 root         (0) root         (0)     4694 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py
--rw-r--r--   0 root         (0) root         (0)     4366 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_missed_update.py
--rw-r--r--   0 root         (0) root         (0)     3719 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_required_use.py
--rw-r--r--   0 root         (0) root         (0)     9190 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py
--rw-r--r--   0 root         (0) root         (0)     3974 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsolved.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py
--rw-r--r--   0 root         (0) root         (0)     3584 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/resolver/test_targetroot.py
--rw-r--r--   0 root         (0) root         (0)     1571 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py
--rw-r--r--   0 root         (0) root         (0)    11321 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/resolver/test_unmerge_order.py
--rw-r--r--   0 root         (0) root         (0)     3843 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_update.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_use_dep_defaults.py
--rw-r--r--   0 root         (0) root         (0)     5326 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_useflags.py
--rw-r--r--   0 root         (0) root         (0)     9976 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_virtual_minimize_children.py
--rw-r--r--   0 root         (0) root         (0)     9326 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/resolver/test_virtual_slot.py
--rw-r--r--   0 root         (0) root         (0)     2910 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/resolver/test_with_test_deps.py
--rwxr-xr-x   0 root         (0) root         (0)     2100 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/tests/runTests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/base/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/base/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sets/base/testInternalPackageSet.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sets/base/testVariableSet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/files/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/files/__test__.py
--rw-r--r--   0 root         (0) root         (0)      992 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/sets/files/testConfigFileSet.py
--rw-r--r--   0 root         (0) root         (0)      829 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/sets/files/testStaticFileSet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sets/shell/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sets/shell/__test__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sets/shell/testShell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.742411 portage-3.0.47/lib/portage/tests/sync/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sync/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/sync/__test__.py
--rw-r--r--   0 root         (0) root         (0)    16481 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/sync/test_sync_local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/unicode/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/unicode/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.47/lib/portage/tests/unicode/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2294 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/unicode/test_string_format.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/update/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.110799 portage-3.0.47/lib/portage/tests/update/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.110799 portage-3.0.47/lib/portage/tests/update/__test__.py
--rw-r--r--   0 root         (0) root         (0)     4462 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/update/test_move_ent.py
--rw-r--r--   0 root         (0) root         (0)     5444 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/update/test_move_slot_ent.py
--rw-r--r--   0 root         (0) root         (0)    11460 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/update/test_update_dbentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/
--rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/dyn_libs/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/dyn_libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/dyn_libs/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1389 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/dyn_libs/test_soname_deps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/eventloop/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/eventloop/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/eventloop/__test__.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/eventloop/test_call_soon_fifo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/file_copy/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/file_copy/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/file_copy/__test__.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/file_copy/test_copyfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/futures/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/futures/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.47/lib/portage/tests/util/futures/__test__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/util/futures/asyncio/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/util/futures/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/util/futures/asyncio/__test__.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_child_watcher.py
--rw-r--r--   0 root         (0) root         (0)     2025 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py
--rw-r--r--   0 root         (0) root         (0)     5394 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py
--rw-r--r--   0 root         (0) root         (0)      795 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py
--rw-r--r--   0 root         (0) root         (0)     1394 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py
--rw-r--r--   0 root         (0) root         (0)     6912 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py
--rw-r--r--   0 root         (0) root         (0)     7135 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_compat_coroutine.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_done_callback.py
--rw-r--r--   0 root         (0) root         (0)     1565 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/futures/test_done_callback_after_exit.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_iter_completed.py
--rw-r--r--   0 root         (0) root         (0)    10828 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/futures/test_retry.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/tests/util/test_checksum.py
--rw-r--r--   0 root         (0) root         (0)    11345 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_digraph.py
--rw-r--r--   0 root         (0) root         (0)     1824 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_file_copier.py
--rw-r--r--   0 root         (0) root         (0)     3534 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_getconfig.py
--rw-r--r--   0 root         (0) root         (0)      315 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/test_grabdict.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_install_mask.py
--rw-r--r--   0 root         (0) root         (0)     1120 2022-12-24 02:35:49.845990 portage-3.0.47/lib/portage/tests/util/test_manifest.py
--rw-r--r--   0 root         (0) root         (0)    10489 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/tests/util/test_mtimedb.py
--rw-r--r--   0 root         (0) root         (0)      440 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_normalizedPath.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-09 06:49:46.516103 portage-3.0.47/lib/portage/tests/util/test_shelve.py
--rw-r--r--   0 root         (0) root         (0)     6638 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_socks5.py
--rw-r--r--   0 root         (0) root         (0)      832 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/test_stackDictList.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/tests/util/test_stackDicts.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_stackLists.py
--rw-r--r--   0 root         (0) root         (0)      897 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/tests/util/test_uniqueArray.py
--rw-r--r--   0 root         (0) root         (0)     3347 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_varExpand.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_whirlpool.py
--rw-r--r--   0 root         (0) root         (0)     6243 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/util/test_xattr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/versions/
--rw-r--r--   0 root         (0) root         (0)      174 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/versions/__test__.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/versions/test_cpv_sort_key.py
--rw-r--r--   0 root         (0) root         (0)     3026 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/versions/test_vercmp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/tests/xpak/
--rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/xpak/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.47/lib/portage/tests/xpak/__test__.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/tests/xpak/test_decodeint.py
--rw-r--r--   0 root         (0) root         (0)    17014 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.745745 portage-3.0.47/lib/portage/util/
--rw-r--r--   0 root         (0) root         (0)     3063 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/ExtractKernelVersion.py
--rw-r--r--   0 root         (0) root         (0)     2141 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/SlotObject.py
--rw-r--r--   0 root         (0) root         (0)    68707 2023-03-21 03:50:18.064091 portage-3.0.47/lib/portage/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/_async/
--rw-r--r--   0 root         (0) root         (0)     2609 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_async/AsyncFunction.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/AsyncScheduler.py
--rw-r--r--   0 root         (0) root         (0)      963 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_async/AsyncTaskFuture.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/BuildLogger.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/FileCopier.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_async/FileDigester.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/ForkProcess.py
--rw-r--r--   0 root         (0) root         (0)     7527 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/PipeLogger.py
--rw-r--r--   0 root         (0) root         (0)     2676 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/PipeReaderBlockingIO.py
--rw-r--r--   0 root         (0) root         (0)     1076 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/PopenProcess.py
--rw-r--r--   0 root         (0) root         (0)     4501 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_async/SchedulerInterface.py
--rw-r--r--   0 root         (0) root         (0)      644 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_async/TaskScheduler.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.127466 portage-3.0.47/lib/portage/util/_async/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_async/run_main_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     4347 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_compare_files.py
--rw-r--r--   0 root         (0) root         (0)     1219 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_ctypes.py
--rw-r--r--   0 root         (0) root         (0)     2654 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_desktop_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/_dyn_libs/
--rw-r--r--   0 root         (0) root         (0)    41425 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/LinkageMapELF.py
--rw-r--r--   0 root         (0) root         (0)     2877 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/_dyn_libs/NeededEntry.py
--rw-r--r--   0 root         (0) root         (0)     9385 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.130799 portage-3.0.47/lib/portage/util/_dyn_libs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/display_preserved_libs.py
--rw-r--r--   0 root         (0) root         (0)     1070 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_dyn_libs/dyn_libs.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps.py
--rw-r--r--   0 root         (0) root         (0)     3722 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps_qa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/_eventloop/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.134132 portage-3.0.47/lib/portage/util/_eventloop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5849 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_eventloop/asyncio_event_loop.py
--rw-r--r--   0 root         (0) root         (0)      213 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/_eventloop/global_event_loop.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_get_vm_info.py
--rw-r--r--   0 root         (0) root         (0)     5956 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_info_files.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_path.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/_pty.py
--rw-r--r--   0 root         (0) root         (0)     4032 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/util/_urlopen.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/_xattr.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/backoff.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/bin_entry_point.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3464 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/compression_probe.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/configparser.py
--rw-r--r--   0 root         (0) root         (0)     2180 2022-12-24 02:35:49.845990 portage-3.0.47/lib/portage/util/cpuinfo.py
--rw-r--r--   0 root         (0) root         (0)    12975 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/digraph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/elf/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.47/lib/portage/util/elf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/elf/constants.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/elf/header.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/endian/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.47/lib/portage/util/endian/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1303 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/endian/decode.py
--rw-r--r--   0 root         (0) root         (0)    15592 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/env_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/file_copy/
--rw-r--r--   0 root         (0) root         (0)      909 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/file_copy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2118 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/formatter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/futures/
--rw-r--r--   0 root         (0) root         (0)      180 2022-09-10 09:44:56.967023 portage-3.0.47/lib/portage/util/futures/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/futures/_asyncio/
--rw-r--r--   0 root         (0) root         (0)     9758 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/futures/_asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/futures/_asyncio/streams.py
--rw-r--r--   0 root         (0) root         (0)     1854 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/futures/_sync_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/compat_coroutine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/futures/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.140799 portage-3.0.47/lib/portage/util/futures/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4306 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/executor/fork.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/extendedfutures.py
--rw-r--r--   0 root         (0) root         (0)      516 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/futures/futures.py
--rw-r--r--   0 root         (0) root         (0)     6868 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/iter_completed.py
--rw-r--r--   0 root         (0) root         (0)     6297 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/futures/retry.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/futures/unix_events.py
--rw-r--r--   0 root         (0) root         (0)     1584 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/hooks.py
--rw-r--r--   0 root         (0) root         (0)     6549 2022-09-10 09:45:01.060384 portage-3.0.47/lib/portage/util/install_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/util/iterators/
--rw-r--r--   0 root         (0) root         (0)     2996 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/iterators/MultiIterGroupBy.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.144132 portage-3.0.47/lib/portage/util/iterators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7349 2022-09-10 09:45:01.063717 portage-3.0.47/lib/portage/util/lafilefixer.py
--rw-r--r--   0 root         (0) root         (0)     4814 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/listdir.py
--rw-r--r--   0 root         (0) root         (0)     4339 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/locale.py
--rw-r--r--   0 root         (0) root         (0)    13909 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/movefile.py
--rw-r--r--   0 root         (0) root         (0)     4258 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/mtimedb.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/netlink.py
--rw-r--r--   0 root         (0) root         (0)     1336 2022-09-10 09:44:56.970356 portage-3.0.47/lib/portage/util/path.py
--rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:45:01.057050 portage-3.0.47/lib/portage/util/shelve.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/socks5.py
--rw-r--r--   0 root         (0) root         (0)    58416 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/util/whirlpool.py
--rw-r--r--   0 root         (0) root         (0)     4506 2023-03-21 03:35:23.553538 portage-3.0.47/lib/portage/util/writeable_check.py
--rw-r--r--   0 root         (0) root         (0)    19275 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/lib/portage/xml/
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.147466 portage-3.0.47/lib/portage/xml/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16789 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/xml/metadata.py
--rw-r--r--   0 root         (0) root         (0)    19413 2023-03-21 03:35:23.556871 portage-3.0.47/lib/portage/xpak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/misc/
--rwxr-xr-x   0 root         (0) root         (0)    24116 2023-02-03 18:03:13.736861 portage-3.0.47/misc/emerge-delta-webrsync
--rwxr-xr-x   0 root         (0) root         (0)    29953 2023-04-30 04:10:22.598516 portage-3.0.47/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 04:11:56.749078 portage-3.0.47/src/
--rw-r--r--   0 root         (0) root         (0)    71291 2023-03-21 03:35:23.556871 portage-3.0.47/src/portage_util__whirlpool.c
--rw-r--r--   0 root         (0) root         (0)    13384 2023-03-21 03:35:23.556871 portage-3.0.47/src/portage_util_file_copy_reflink_linux.c
--rw-r--r--   0 root         (0) root         (0)     1276 2023-03-21 03:35:23.556871 portage-3.0.47/src/portage_util_libc.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:35.927469 portage-3.0.48/.portage_not_installed
+-rw-r--r--   0 root         (0) root         (0)     6944 2023-03-21 03:50:18.057424 portage-3.0.48/DEVELOPING
+-rw-r--r--   0 root         (0) root         (0)    18092 2021-11-12 08:15:35.927469 portage-3.0.48/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4474 2023-06-01 01:26:11.262328 portage-3.0.48/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1864 2021-11-12 08:15:35.927469 portage-3.0.48/TEST-NOTES
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.235661 portage-3.0.48/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     3262 2023-03-21 23:52:40.754842 portage-3.0.48/bin/archive-conf
+-rwxr-xr-x   0 root         (0) root         (0)     1443 2023-04-30 23:29:06.349730 portage-3.0.48/bin/bashrc-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4457 2023-03-21 23:52:40.598174 portage-3.0.48/bin/binhost-snapshot
+-rwxr-xr-x   0 root         (0) root         (0)       51 2021-11-12 08:15:35.934136 portage-3.0.48/bin/cgroup-release-agent
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.934136 portage-3.0.48/bin/chmod-lite -> ebuild-pyhelper
+-rwxr-xr-x   0 root         (0) root         (0)      951 2023-03-21 03:35:23.553538 portage-3.0.48/bin/chmod-lite.py
+-rwxr-xr-x   0 root         (0) root         (0)     5891 2023-03-21 03:35:23.553538 portage-3.0.48/bin/chpathtool.py
+-rwxr-xr-x   0 root         (0) root         (0)     1421 2023-03-21 03:35:23.553538 portage-3.0.48/bin/clean_locks
+-rwxr-xr-x   0 root         (0) root         (0)    19951 2023-04-29 04:41:18.541267 portage-3.0.48/bin/dispatch-conf
+-rwxr-xr-x   0 root         (0) root         (0)     8895 2023-04-29 04:41:16.537917 portage-3.0.48/bin/dohtml.py
+-rwxr-xr-x   0 root         (0) root         (0)    20007 2023-04-30 23:29:06.349730 portage-3.0.48/bin/doins.py
+-rwxr-xr-x   0 root         (0) root         (0)     6078 2023-04-30 23:29:06.349730 portage-3.0.48/bin/eapi.sh
+-rwxr-xr-x   0 root         (0) root         (0)     4310 2023-04-30 23:29:06.349730 portage-3.0.48/bin/eapi7-ver-funcs.sh
+-rwxr-xr-x   0 root         (0) root         (0)    15468 2023-03-21 23:52:40.598174 portage-3.0.48/bin/ebuild
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/bin/ebuild-helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/bin/ebuild-helpers/bsd/
+-rwxr-xr-x   0 root         (0) root         (0)      639 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/bsd/sed
+-rwxr-xr-x   0 root         (0) root         (0)      200 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/die
+-rwxr-xr-x   0 root         (0) root         (0)     1049 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/dobin
+-rwxr-xr-x   0 root         (0) root         (0)      515 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/doconfd
+-rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.057050 portage-3.0.48/bin/ebuild-helpers/dodir
+-rwxr-xr-x   0 root         (0) root         (0)      885 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/dodoc
+-rwxr-xr-x   0 root         (0) root         (0)      513 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/doenvd
+-rwxr-xr-x   0 root         (0) root         (0)      952 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/doexe
+-rwxr-xr-x   0 root         (0) root         (0)      531 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/dohard
+-rwxr-xr-x   0 root         (0) root         (0)      632 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/doheader
+-rwxr-xr-x   0 root         (0) root         (0)      782 2022-09-10 09:45:01.063717 portage-3.0.48/bin/ebuild-helpers/dohtml
+-rwxr-xr-x   0 root         (0) root         (0)      722 2023-02-03 18:03:13.730194 portage-3.0.48/bin/ebuild-helpers/doinfo
+-rwxr-xr-x   0 root         (0) root         (0)      485 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/doinitd
+-rwxr-xr-x   0 root         (0) root         (0)     3034 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/doins
+-rwxr-xr-x   0 root         (0) root         (0)     1333 2023-05-10 01:03:08.508755 portage-3.0.48/bin/ebuild-helpers/dolib
+-rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/dolib.a
+-rwxr-xr-x   0 root         (0) root         (0)      189 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/dolib.so
+-rwxr-xr-x   0 root         (0) root         (0)     1553 2023-02-03 18:03:13.730194 portage-3.0.48/bin/ebuild-helpers/doman
+-rwxr-xr-x   0 root         (0) root         (0)     1216 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/domo
+-rwxr-xr-x   0 root         (0) root         (0)     1053 2023-04-29 04:41:16.537917 portage-3.0.48/bin/ebuild-helpers/dosbin
+-rwxr-xr-x   0 root         (0) root         (0)      818 2023-02-03 18:03:13.730194 portage-3.0.48/bin/ebuild-helpers/dosed
+-rwxr-xr-x   0 root         (0) root         (0)     2366 2022-09-10 09:45:01.063717 portage-3.0.48/bin/ebuild-helpers/dosym
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.48/bin/ebuild-helpers/eerror -> elog
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.48/bin/ebuild-helpers/einfo -> elog
+-rwxr-xr-x   0 root         (0) root         (0)      204 2022-09-10 09:45:01.053717 portage-3.0.48/bin/ebuild-helpers/elog
+-rwxr-xr-x   0 root         (0) root         (0)      894 2022-09-10 09:45:01.053717 portage-3.0.48/bin/ebuild-helpers/emake
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.48/bin/ebuild-helpers/eqawarn -> elog
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.937469 portage-3.0.48/bin/ebuild-helpers/ewarn -> elog
+-rwxr-xr-x   0 root         (0) root         (0)      871 2023-04-30 23:29:11.103090 portage-3.0.48/bin/ebuild-helpers/fowners
+-rwxr-xr-x   0 root         (0) root         (0)      938 2023-04-30 23:29:11.103090 portage-3.0.48/bin/ebuild-helpers/fperms
+-rwxr-xr-x   0 root         (0) root         (0)      490 2023-02-03 18:03:13.730194 portage-3.0.48/bin/ebuild-helpers/keepdir
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newbin -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newconfd -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newdoc -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newenvd -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newexe -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newheader -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newinitd -> newins
+-rwxr-xr-x   0 root         (0) root         (0)     1201 2023-02-03 18:03:13.730194 portage-3.0.48/bin/ebuild-helpers/newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newlib.a -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newlib.so -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newman -> newins
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/newsbin -> newins
+-rwxr-xr-x   0 root         (0) root         (0)      359 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/nonfatal
+-rwxr-xr-x   0 root         (0) root         (0)      299 2023-05-15 02:02:30.372073 portage-3.0.48/bin/ebuild-helpers/portageq
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/prepall
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.48/bin/ebuild-helpers/prepalldocs
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.48/bin/ebuild-helpers/prepallinfo
+-rwxr-xr-x   0 root         (0) root         (0)      245 2022-09-10 09:45:01.053717 portage-3.0.48/bin/ebuild-helpers/prepallman
+-rwxr-xr-x   0 root         (0) root         (0)      444 2023-05-11 20:15:47.085992 portage-3.0.48/bin/ebuild-helpers/prepallstrip
+-rwxr-xr-x   0 root         (0) root         (0)      843 2023-04-09 06:49:46.512769 portage-3.0.48/bin/ebuild-helpers/prepinfo
+-rwxr-xr-x   0 root         (0) root         (0)      364 2023-04-09 06:49:46.512769 portage-3.0.48/bin/ebuild-helpers/prepman
+-rwxr-xr-x   0 root         (0) root         (0)      436 2023-05-11 20:15:47.085992 portage-3.0.48/bin/ebuild-helpers/prepstrip
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/bin/ebuild-helpers/unprivileged/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-helpers/unprivileged/chgrp -> chown
+-rwxr-xr-x   0 root         (0) root         (0)     1178 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/unprivileged/chown
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/bin/ebuild-helpers/xattr/
+-rwxr-xr-x   0 root         (0) root         (0)     1369 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ebuild-helpers/xattr/install
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.940802 portage-3.0.48/bin/ebuild-ipc -> ebuild-pyhelper
+-rwxr-xr-x   0 root         (0) root         (0)    10684 2023-03-21 23:52:40.598174 portage-3.0.48/bin/ebuild-ipc.py
+-rwxr-xr-x   0 root         (0) root         (0)      618 2023-05-23 00:21:31.539461 portage-3.0.48/bin/ebuild-pyhelper
+-rwxr-xr-x   0 root         (0) root         (0)    26114 2023-03-21 03:35:23.556871 portage-3.0.48/bin/ebuild.sh
+-rwxr-xr-x   0 root         (0) root         (0)     6481 2022-12-24 02:35:49.845990 portage-3.0.48/bin/ecompress
+-rwxr-xr-x   0 root         (0) root         (0)     1746 2022-09-10 09:45:01.060384 portage-3.0.48/bin/ecompress-file
+-rwxr-xr-x   0 root         (0) root         (0)    53990 2023-03-21 23:52:40.598174 portage-3.0.48/bin/egencache
+-rwxr-xr-x   0 root         (0) root         (0)     1857 2023-03-21 03:35:23.556871 portage-3.0.48/bin/emaint
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-03-21 23:52:40.598174 portage-3.0.48/bin/emerge
+-rwxr-xr-x   0 root         (0) root         (0)    20498 2023-05-26 01:33:03.449635 portage-3.0.48/bin/emerge-webrsync
+-rwxr-xr-x   0 root         (0) root         (0)      634 2022-09-10 09:45:01.053717 portage-3.0.48/bin/emirrordist
+-rwxr-xr-x   0 root         (0) root         (0)     1048 2023-03-21 03:35:23.556871 portage-3.0.48/bin/env-update
+-rwxr-xr-x   0 root         (0) root         (0)    17406 2023-05-17 06:19:53.321081 portage-3.0.48/bin/estrip
+-rwxr-xr-x   0 root         (0) root         (0)    23454 2023-03-21 03:50:18.057424 portage-3.0.48/bin/etc-update
+-rwxr-xr-x   0 root         (0) root         (0)     6045 2023-03-21 03:35:23.556871 portage-3.0.48/bin/filter-bash-environment.py
+-rwxr-xr-x   0 root         (0) root         (0)     1601 2023-03-21 03:35:23.556871 portage-3.0.48/bin/fixpackages
+-rwxr-xr-x   0 root         (0) root         (0)    15636 2023-03-21 23:52:40.601508 portage-3.0.48/bin/glsa-check
+-rwxr-xr-x   0 root         (0) root         (0)     2166 2023-03-21 03:35:23.556871 portage-3.0.48/bin/gpkg-helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     2476 2022-12-24 02:35:49.845990 portage-3.0.48/bin/gpkg-sign
+-rwxr-xr-x   0 root         (0) root         (0)     2918 2023-04-30 23:29:06.349730 portage-3.0.48/bin/helper-functions.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/bin/install-qa-check.d/
+-rwxr-xr-x   0 root         (0) root         (0)      444 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/05double-D
+-rwxr-xr-x   0 root         (0) root         (0)     4302 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/05prefix
+-rwxr-xr-x   0 root         (0) root         (0)     5559 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/10executable-issues
+-rwxr-xr-x   0 root         (0) root         (0)     3591 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/10ignored-flags
+-rwxr-xr-x   0 root         (0) root         (0)      406 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/20deprecated-directories
+-rwxr-xr-x   0 root         (0) root         (0)      835 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/20runtime-directories
+-rwxr-xr-x   0 root         (0) root         (0)     3306 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/60bash-completion
+-rwxr-xr-x   0 root         (0) root         (0)     1443 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/60openrc
+-rwxr-xr-x   0 root         (0) root         (0)     5508 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/60pkgconfig
+-rwxr-xr-x   0 root         (0) root         (0)      668 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/60pngfix
+-rwxr-xr-x   0 root         (0) root         (0)      687 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/60systemd
+-rwxr-xr-x   0 root         (0) root         (0)      442 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/60udev
+-rwxr-xr-x   0 root         (0) root         (0)     5556 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/80libraries
+-rwxr-xr-x   0 root         (0) root         (0)     1417 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/80multilib-strict
+-rwxr-xr-x   0 root         (0) root         (0)     1918 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/90bad-bin-group-write
+-rwxr-xr-x   0 root         (0) root         (0)     1566 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/90bad-bin-owner
+-rwxr-xr-x   0 root         (0) root         (0)      654 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/90cmake-warnings
+-rwxr-xr-x   0 root         (0) root         (0)     3995 2023-05-11 01:24:42.440571 portage-3.0.48/bin/install-qa-check.d/90config-impl-decl
+-rwxr-xr-x   0 root         (0) root         (0)     1277 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/90cython-dep
+-rwxr-xr-x   0 root         (0) root         (0)     8300 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/90gcc-warnings
+-rwxr-xr-x   0 root         (0) root         (0)     1042 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/90world-writable
+-rwxr-xr-x   0 root         (0) root         (0)     1518 2023-04-30 23:29:06.349730 portage-3.0.48/bin/install-qa-check.d/95empty-dirs
+-rwxr-xr-x   0 root         (0) root         (0)     6314 2023-03-21 23:52:40.601508 portage-3.0.48/bin/install.py
+-rwxr-xr-x   0 root         (0) root         (0)    18552 2023-04-30 23:29:06.349730 portage-3.0.48/bin/isolated-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)      903 2023-03-21 03:35:23.553538 portage-3.0.48/bin/lock-helper.py
+-rwxr-xr-x   0 root         (0) root         (0)    20306 2023-05-15 02:02:30.372073 portage-3.0.48/bin/misc-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)    34584 2023-04-30 23:29:06.349730 portage-3.0.48/bin/phase-functions.sh
+-rwxr-xr-x   0 root         (0) root         (0)    33763 2023-05-15 02:02:30.372073 portage-3.0.48/bin/phase-helpers.sh
+-rwxr-xr-x   0 root         (0) root         (0)     5723 2023-04-30 23:29:06.349730 portage-3.0.48/bin/pid-ns-init
+-rwxr-xr-x   0 root         (0) root         (0)    51197 2023-03-21 23:52:40.601508 portage-3.0.48/bin/portageq
+-rwxr-xr-x   0 root         (0) root         (0)      608 2023-05-15 02:02:30.372073 portage-3.0.48/bin/portageq-wrapper
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/bin/postinst-qa-check.d/
+-rwxr-xr-x   0 root         (0) root         (0)     5236 2023-04-30 23:29:06.349730 portage-3.0.48/bin/postinst-qa-check.d/50xdg-utils
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/bin/preinst-qa-check.d/
+lrwxrwxrwx   0 root         (0) root         (0)        0 2021-11-12 08:15:35.947469 portage-3.0.48/bin/preinst-qa-check.d/50xdg-utils -> ../postinst-qa-check.d/50xdg-utils
+-rwxr-xr-x   0 root         (0) root         (0)    16731 2023-03-21 23:52:40.601508 portage-3.0.48/bin/quickpkg
+-rwxr-xr-x   0 root         (0) root         (0)     4992 2023-03-21 03:35:23.556871 portage-3.0.48/bin/regenworld
+-rwxr-xr-x   0 root         (0) root         (0)     4535 2023-04-30 23:29:06.349730 portage-3.0.48/bin/save-ebuild-env.sh
+-rwxr-xr-x   0 root         (0) root         (0)     1339 2022-09-10 09:45:01.060384 portage-3.0.48/bin/shelve-utils
+-rwxr-xr-x   0 root         (0) root         (0)     8140 2023-04-30 23:29:06.349730 portage-3.0.48/bin/socks5-server.py
+-rwxr-xr-x   0 root         (0) root         (0)     4784 2023-03-21 23:52:40.601508 portage-3.0.48/bin/xattr-helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     1825 2023-03-21 03:35:23.550205 portage-3.0.48/bin/xpak-helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/cnf/
+-rw-r--r--   0 root         (0) root         (0)     1718 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.alpha.diff
+-rw-r--r--   0 root         (0) root         (0)     2319 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.amd64-fbsd.diff
+-rw-r--r--   0 root         (0) root         (0)     2309 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.amd64.diff
+-rw-r--r--   0 root         (0) root         (0)     1592 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.arm.diff
+-rw-r--r--   0 root         (0) root         (0)     1580 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.arm64.diff
+-rw-r--r--   0 root         (0) root         (0)     2465 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.hppa.diff
+-rw-r--r--   0 root         (0) root         (0)      663 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.ia64.diff
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-03-21 03:35:23.550205 portage-3.0.48/cnf/make.conf.example.loong.diff
+-rw-r--r--   0 root         (0) root         (0)      900 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.m68k.diff
+-rw-r--r--   0 root         (0) root         (0)     1383 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.mips.diff
+-rw-r--r--   0 root         (0) root         (0)     3541 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.ppc.diff
+-rw-r--r--   0 root         (0) root         (0)     2361 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.ppc64.diff
+-rw-r--r--   0 root         (0) root         (0)     2332 2022-09-10 09:44:56.963689 portage-3.0.48/cnf/make.conf.example.riscv.diff
+-rw-r--r--   0 root         (0) root         (0)      656 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.s390.diff
+-rw-r--r--   0 root         (0) root         (0)     1257 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.sh.diff
+-rw-r--r--   0 root         (0) root         (0)      728 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.sparc-fbsd.diff
+-rw-r--r--   0 root         (0) root         (0)     2129 2021-12-09 09:19:33.760140 portage-3.0.48/cnf/make.conf.example.sparc.diff
+-rw-r--r--   0 root         (0) root         (0)     2507 2021-12-09 09:19:33.763473 portage-3.0.48/cnf/make.conf.example.x86-fbsd.diff
+-rw-r--r--   0 root         (0) root         (0)     3759 2021-12-09 09:19:33.763473 portage-3.0.48/cnf/make.conf.example.x86.diff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/doc/api/
+-rw-r--r--   0 root         (0) root         (0)     1141 2021-11-12 08:15:35.954135 portage-3.0.48/doc/api/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-03-21 03:35:23.550205 portage-3.0.48/doc/api/conf.py
+-rw-r--r--   0 root         (0) root         (0)      217 2021-11-12 08:15:35.954135 portage-3.0.48/doc/api/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/doc/config/
+-rw-r--r--   0 root         (0) root         (0)     1900 2021-11-12 08:15:35.954135 portage-3.0.48/doc/config/bashrc.docbook
+-rw-r--r--   0 root         (0) root         (0)    26214 2021-11-12 08:15:35.954135 portage-3.0.48/doc/config/sets.docbook
+-rw-r--r--   0 root         (0) root         (0)       85 2021-11-12 08:15:35.954135 portage-3.0.48/doc/config.docbook
+-rw-r--r--   0 root         (0) root         (0)      257 2021-11-12 08:15:35.954135 portage-3.0.48/doc/custom.xsl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/doc/dependency_resolution/
+-rw-r--r--   0 root         (0) root         (0)     3281 2021-11-12 08:15:35.957468 portage-3.0.48/doc/dependency_resolution/decision_making.docbook
+-rw-r--r--   0 root         (0) root         (0)     4154 2021-11-12 08:15:35.957468 portage-3.0.48/doc/dependency_resolution/package_modeling.docbook
+-rw-r--r--   0 root         (0) root         (0)     3451 2021-11-12 08:15:35.957468 portage-3.0.48/doc/dependency_resolution/task_scheduling.docbook
+-rw-r--r--   0 root         (0) root         (0)      200 2021-11-12 08:15:35.954135 portage-3.0.48/doc/dependency_resolution.docbook
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/doc/package/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/doc/package/ebuild/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.238995 portage-3.0.48/doc/package/ebuild/eapi/
+-rw-r--r--   0 root         (0) root         (0)      487 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/eapi/0.docbook
+-rw-r--r--   0 root         (0) root         (0)     1598 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/eapi/1.docbook
+-rw-r--r--   0 root         (0) root         (0)     8299 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/eapi/2.docbook
+-rw-r--r--   0 root         (0) root         (0)     2938 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/eapi/3.docbook
+-rw-r--r--   0 root         (0) root         (0)     3112 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/eapi/4-slot-abi.docbook
+-rw-r--r--   0 root         (0) root         (0)    14690 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/eapi/4.docbook
+-rw-r--r--   0 root         (0) root         (0)     8044 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/eapi/5.docbook
+-rw-r--r--   0 root         (0) root         (0)     1725 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/helper_functions.docbook
+-rw-r--r--   0 root         (0) root         (0)     2780 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package/ebuild/phases.docbook
+-rw-r--r--   0 root         (0) root         (0)      364 2022-09-10 09:45:01.060384 portage-3.0.48/doc/package/ebuild.docbook
+-rw-r--r--   0 root         (0) root         (0)       76 2021-11-12 08:15:35.957468 portage-3.0.48/doc/package.docbook
+-rw-r--r--   0 root         (0) root         (0)     2194 2022-09-10 09:45:01.060384 portage-3.0.48/doc/portage.docbook
+-rw-r--r--   0 root         (0) root         (0)    19579 2021-11-12 08:15:35.960802 portage-3.0.48/doc/qa.docbook
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.228995 portage-3.0.48/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.242328 portage-3.0.48/lib/_emerge/
+-rw-r--r--   0 root         (0) root         (0)      816 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/AbstractDepPriority.py
+-rw-r--r--   0 root         (0) root         (0)    18231 2023-04-30 23:30:07.143407 portage-3.0.48/lib/_emerge/AbstractEbuildProcess.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/AbstractPollTask.py
+-rw-r--r--   0 root         (0) root         (0)    10372 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/AsynchronousLock.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/AsynchronousTask.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/AtomArg.py
+-rw-r--r--   0 root         (0) root         (0)    21241 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/Binpkg.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/BinpkgEnvExtractor.py
+-rw-r--r--   0 root         (0) root         (0)     5399 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/BinpkgExtractorAsync.py
+-rw-r--r--   0 root         (0) root         (0)     9555 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/BinpkgFetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/BinpkgPrefetcher.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/BinpkgVerifier.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/Blocker.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/BlockerCache.py
+-rw-r--r--   0 root         (0) root         (0)     5325 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/BlockerDB.py
+-rw-r--r--   0 root         (0) root         (0)      355 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/BlockerDepPriority.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/CompositeTask.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/DepPriority.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/DepPriorityNormalRange.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/DepPrioritySatisfiedRange.py
+-rw-r--r--   0 root         (0) root         (0)      878 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/Dependency.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/DependencyArg.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/EbuildBinpkg.py
+-rw-r--r--   0 root         (0) root         (0)    23204 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/EbuildBuild.py
+-rw-r--r--   0 root         (0) root         (0)     5749 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/EbuildBuildDir.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/EbuildExecuter.py
+-rw-r--r--   0 root         (0) root         (0)    14395 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/EbuildFetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/EbuildFetchonly.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/EbuildIpcDaemon.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/EbuildMerge.py
+-rw-r--r--   0 root         (0) root         (0)     7597 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/EbuildMetadataPhase.py
+-rw-r--r--   0 root         (0) root         (0)    22622 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/EbuildPhase.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/EbuildProcess.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/EbuildSpawnProcess.py
+-rw-r--r--   0 root         (0) root         (0)    12786 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/FakeVartree.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/FifoIpcDaemon.py
+-rw-r--r--   0 root         (0) root         (0)     9142 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/JobStatusDisplay.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/MergeListItem.py
+-rw-r--r--   0 root         (0) root         (0)     6121 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/MetadataRegen.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2022-09-10 09:45:01.063717 portage-3.0.48/lib/_emerge/MiscFunctionsProcess.py
+-rw-r--r--   0 root         (0) root         (0)    30870 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/Package.py
+-rw-r--r--   0 root         (0) root         (0)      735 2022-09-10 09:44:56.967023 portage-3.0.48/lib/_emerge/PackageArg.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/PackageMerge.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/PackagePhase.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/PackageUninstall.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2022-09-10 09:44:56.967023 portage-3.0.48/lib/_emerge/PackageVirtualDbapi.py
+-rw-r--r--   0 root         (0) root         (0)     2681 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/PipeReader.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/PollScheduler.py
+-rw-r--r--   0 root         (0) root         (0)      603 2022-09-10 09:44:56.967023 portage-3.0.48/lib/_emerge/ProgressHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2022-09-10 09:44:56.967023 portage-3.0.48/lib/_emerge/RootConfig.py
+-rw-r--r--   0 root         (0) root         (0)    85602 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/Scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/SequentialTaskQueue.py
+-rw-r--r--   0 root         (0) root         (0)      421 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/SetArg.py
+-rw-r--r--   0 root         (0) root         (0)    10067 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/SpawnProcess.py
+-rw-r--r--   0 root         (0) root         (0)     3162 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/SubProcess.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/Task.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/TaskSequence.py
+-rw-r--r--   0 root         (0) root         (0)      455 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/UninstallFailure.py
+-rw-r--r--   0 root         (0) root         (0)     1326 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/UnmergeDepPriority.py
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/UseFlagDisplay.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-04-30 23:30:07.146741 portage-3.0.48/lib/_emerge/UserQuery.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.977468 portage-3.0.48/lib/_emerge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/_find_deep_system_runtime_deps.py
+-rw-r--r--   0 root         (0) root         (0)      442 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/_flush_elog_mod_echo.py
+-rw-r--r--   0 root         (0) root         (0)   148632 2023-05-23 02:59:13.685038 portage-3.0.48/lib/_emerge/actions.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-04-30 23:30:07.150074 portage-3.0.48/lib/_emerge/chk_updated_cfg_files.py
+-rw-r--r--   0 root         (0) root         (0)      498 2022-09-10 09:44:56.963689 portage-3.0.48/lib/_emerge/clear_caches.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-30 23:30:07.150074 portage-3.0.48/lib/_emerge/countdown.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/create_depgraph_params.py
+-rw-r--r--   0 root         (0) root         (0)     5191 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/create_world_atom.py
+-rw-r--r--   0 root         (0) root         (0)   497595 2023-05-11 20:19:00.830630 portage-3.0.48/lib/_emerge/depgraph.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/emergelog.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/getloadavg.py
+-rw-r--r--   0 root         (0) root         (0)     3425 2022-09-10 09:44:56.970356 portage-3.0.48/lib/_emerge/help.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-03-21 03:35:23.556871 portage-3.0.48/lib/_emerge/is_valid_package_atom.py
+-rw-r--r--   0 root         (0) root         (0)    42164 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/main.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/post_emerge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.242328 portage-3.0.48/lib/_emerge/resolver/
+-rw-r--r--   0 root         (0) root         (0)     3198 2022-09-10 09:44:56.970356 portage-3.0.48/lib/_emerge/resolver/DbapiProvidesIndex.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:35.980801 portage-3.0.48/lib/_emerge/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11328 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/resolver/backtracking.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/resolver/circular_dependency.py
+-rw-r--r--   0 root         (0) root         (0)    39524 2023-04-30 23:30:07.153407 portage-3.0.48/lib/_emerge/resolver/output.py
+-rw-r--r--   0 root         (0) root         (0)    20748 2023-04-30 23:30:07.156741 portage-3.0.48/lib/_emerge/resolver/output_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    15636 2023-03-21 03:35:23.550205 portage-3.0.48/lib/_emerge/resolver/package_tracker.py
+-rw-r--r--   0 root         (0) root         (0)    58871 2023-04-30 23:30:07.156741 portage-3.0.48/lib/_emerge/resolver/slot_collision.py
+-rw-r--r--   0 root         (0) root         (0)    20942 2023-04-30 23:30:07.156741 portage-3.0.48/lib/_emerge/search.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/show_invalid_depstring_notice.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-03-21 03:35:23.553538 portage-3.0.48/lib/_emerge/stdout_spinner.py
+-rw-r--r--   0 root         (0) root         (0)    26360 2023-04-30 23:30:07.160074 portage-3.0.48/lib/_emerge/unmerge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.242328 portage-3.0.48/lib/portage/
+-rw-r--r--   0 root         (0) root         (0)    25908 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.242328 portage-3.0.48/lib/portage/_compat_upgrade/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.007468 portage-3.0.48/lib/portage/_compat_upgrade/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/_compat_upgrade/binpkg_compression.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_compat_upgrade/binpkg_multi_instance.py
+-rw-r--r--   0 root         (0) root         (0)     4288 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_compat_upgrade/default_locations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.242328 portage-3.0.48/lib/portage/_emirrordist/
+-rw-r--r--   0 root         (0) root         (0)     5376 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_emirrordist/Config.py
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_emirrordist/ContentDB.py
+-rw-r--r--   0 root         (0) root         (0)     4631 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_emirrordist/DeletionIterator.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_emirrordist/DeletionTask.py
+-rw-r--r--   0 root         (0) root         (0)    11176 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_emirrordist/FetchIterator.py
+-rw-r--r--   0 root         (0) root         (0)    25443 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_emirrordist/FetchTask.py
+-rw-r--r--   0 root         (0) root         (0)     9145 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_emirrordist/MirrorDistTask.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.007468 portage-3.0.48/lib/portage/_emirrordist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16082 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/_emirrordist/main.py
+-rw-r--r--   0 root         (0) root         (0)    10222 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_global_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/_legacy_globals.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_selinux.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/_sets/
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_sets/ProfilePackageSet.py
+-rw-r--r--   0 root         (0) root         (0)    14268 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/_sets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_sets/base.py
+-rw-r--r--   0 root         (0) root         (0)    22035 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_sets/dbapi.py
+-rw-r--r--   0 root         (0) root         (0)    15573 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_sets/files.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/_sets/libs.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_sets/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_sets/security.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/_sets/shell.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/binpkg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/binrepo/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.014134 portage-3.0.48/lib/portage/binrepo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4554 2023-02-03 18:03:13.730194 portage-3.0.48/lib/portage/binrepo/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/cache/
+-rw-r--r--   0 root         (0) root         (0)      101 2021-11-12 08:15:36.014134 portage-3.0.48/lib/portage/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3167 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/anydbm.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/cache_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/ebuild_xattr.py
+-rw-r--r--   0 root         (0) root         (0)     5286 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/flat_hash.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/fs_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/cache/index/
+-rw-r--r--   0 root         (0) root         (0)      562 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/index/IndexStreamIterator.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.017468 portage-3.0.48/lib/portage/cache/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/cache/index/pkg_desc_index.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/cache/mappings.py
+-rw-r--r--   0 root         (0) root         (0)     5844 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/cache/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    11820 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/cache/sql_template.py
+-rw-r--r--   0 root         (0) root         (0)    13390 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/cache/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)    13272 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/template.py
+-rw-r--r--   0 root         (0) root         (0)      789 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/cache/volatile.py
+-rw-r--r--   0 root         (0) root         (0)    16566 2023-04-07 09:45:44.114534 portage-3.0.48/lib/portage/checksum.py
+-rw-r--r--   0 root         (0) root         (0)     8879 2023-05-26 01:33:06.126329 portage-3.0.48/lib/portage/const.py
+-rw-r--r--   0 root         (0) root         (0)    11470 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/cvstree.py
+-rw-r--r--   0 root         (0) root         (0)    11537 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/dbapi/
+-rw-r--r--   0 root         (0) root         (0)      643 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/dbapi/DummyTree.py
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/dbapi/IndexedPortdb.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/dbapi/IndexedVardb.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/dbapi/_ContentsCaseSensitivityManager.py
+-rw-r--r--   0 root         (0) root         (0)    10128 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/dbapi/_MergeProcess.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/dbapi/_SyncfsProcess.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/dbapi/_VdbMetadataDelta.py
+-rw-r--r--   0 root         (0) root         (0)    16769 2023-04-09 06:49:46.516103 portage-3.0.48/lib/portage/dbapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/dbapi/_expand_new_virt.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/dbapi/_similar_name_search.py
+-rw-r--r--   0 root         (0) root         (0)    90388 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/dbapi/bintree.py
+-rw-r--r--   0 root         (0) root         (0)     4184 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/dbapi/cpv_expand.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/dbapi/dep_expand.py
+-rw-r--r--   0 root         (0) root         (0)    64264 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/dbapi/porttree.py
+-rw-r--r--   0 root         (0) root         (0)   253670 2023-05-26 01:33:06.126329 portage-3.0.48/lib/portage/dbapi/vartree.py
+-rw-r--r--   0 root         (0) root         (0)     7587 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/dbapi/virtual.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/dep/
+-rw-r--r--   0 root         (0) root         (0)   107693 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/dep/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/dep/_dnf.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/dep/_slot_operator.py
+-rw-r--r--   0 root         (0) root         (0)    42498 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/dep/dep_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/dep/soname/
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/dep/soname/SonameAtom.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.030801 portage-3.0.48/lib/portage/dep/soname/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/dep/soname/multilib_category.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/dep/soname/parse.py
+-rw-r--r--   0 root         (0) root         (0)    14093 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/dispatch_conf.py
+-rw-r--r--   0 root         (0) root         (0)     8092 2023-01-10 15:35:29.386865 portage-3.0.48/lib/portage/eapi.py
+-rw-r--r--   0 root         (0) root         (0)     6757 2022-09-10 09:45:01.057050 portage-3.0.48/lib/portage/eclass_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/elog/
+-rw-r--r--   0 root         (0) root         (0)     6879 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/elog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      613 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/elog/filtering.py
+-rw-r--r--   0 root         (0) root         (0)     6065 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/elog/messages.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-02-03 18:03:13.736861 portage-3.0.48/lib/portage/elog/mod_custom.py
+-rw-r--r--   0 root         (0) root         (0)     2204 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/elog/mod_echo.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/elog/mod_mail.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/elog/mod_mail_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/elog/mod_save.py
+-rw-r--r--   0 root         (0) root         (0)     3580 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/elog/mod_save_summary.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/elog/mod_syslog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/
+-rw-r--r--   0 root         (0) root         (0)      163 2021-11-12 08:15:36.037467 portage-3.0.48/lib/portage/emaint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      762 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     8691 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/emaint/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/
+-rw-r--r--   0 root         (0) root         (0)      173 2021-11-12 08:15:36.037467 portage-3.0.48/lib/portage/emaint/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/binhost/
+-rw-r--r--   0 root         (0) root         (0)      524 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/binhost/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/emaint/modules/binhost/binhost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/config/
+-rw-r--r--   0 root         (0) root         (0)      534 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2520 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/emaint/modules/config/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/logs/
+-rw-r--r--   0 root         (0) root         (0)     1629 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/emaint/modules/logs/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/merges/
+-rw-r--r--   0 root         (0) root         (0)     1417 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/merges/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/emaint/modules/merges/merges.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/move/
+-rw-r--r--   0 root         (0) root         (0)      851 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/move/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7693 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/emaint/modules/move/move.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/resume/
+-rw-r--r--   0 root         (0) root         (0)      566 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/resume/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/emaint/modules/resume/resume.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/sync/
+-rw-r--r--   0 root         (0) root         (0)     2145 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18469 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/emaint/modules/sync/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/emaint/modules/world/
+-rw-r--r--   0 root         (0) root         (0)      502 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/emaint/modules/world/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/emaint/modules/world/world.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/env/
+-rw-r--r--   0 root         (0) root         (0)       52 2021-11-12 08:15:36.044134 portage-3.0.48/lib/portage/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/env/config.py
+-rw-r--r--   0 root         (0) root         (0)    10311 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/env/loaders.py
+-rw-r--r--   0 root         (0) root         (0)      578 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/env/validators.py
+-rw-r--r--   0 root         (0) root         (0)     6616 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/exception.py
+-rw-r--r--   0 root         (0) root         (0)    31465 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/getbinpkg.py
+-rw-r--r--   0 root         (0) root         (0)    31099 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/glsa.py
+-rw-r--r--   0 root         (0) root         (0)     3637 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/gpg.py
+-rw-r--r--   0 root         (0) root         (0)    80663 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/gpkg.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/localization.py
+-rw-r--r--   0 root         (0) root         (0)    28153 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/locks.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/mail.py
+-rw-r--r--   0 root         (0) root         (0)    31108 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/manifest.py
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-02-03 18:03:13.736861 portage-3.0.48/lib/portage/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     8568 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/module.py
+-rw-r--r--   0 root         (0) root         (0)    18485 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/news.py
+-rw-r--r--   0 root         (0) root         (0)    29784 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/package/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.047467 portage-3.0.48/lib/portage/package/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/package/ebuild/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.48/lib/portage/package/ebuild/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.245661 portage-3.0.48/lib/portage/package/ebuild/_config/
+-rw-r--r--   0 root         (0) root         (0)    13005 2023-02-03 18:03:13.730194 portage-3.0.48/lib/portage/package/ebuild/_config/KeywordsManager.py
+-rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_config/LicenseManager.py
+-rw-r--r--   0 root         (0) root         (0)    16684 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_config/LocationsManager.py
+-rw-r--r--   0 root         (0) root         (0)    13915 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/package/ebuild/_config/MaskManager.py
+-rw-r--r--   0 root         (0) root         (0)    21565 2023-02-03 18:03:13.730194 portage-3.0.48/lib/portage/package/ebuild/_config/UseManager.py
+-rw-r--r--   0 root         (0) root         (0)     8443 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/package/ebuild/_config/VirtualsManager.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.050800 portage-3.0.48/lib/portage/package/ebuild/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      770 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/package/ebuild/_config/env_var_validation.py
+-rw-r--r--   0 root         (0) root         (0)     4694 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/package/ebuild/_config/features_set.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/package/ebuild/_config/helper.py
+-rw-r--r--   0 root         (0) root         (0)     9457 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/package/ebuild/_config/special_env_vars.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/package/ebuild/_ipc/
+-rw-r--r--   0 root         (0) root         (0)      829 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_ipc/ExitCommand.py
+-rw-r--r--   0 root         (0) root         (0)      212 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_ipc/IpcCommand.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/package/ebuild/_ipc/QueryCommand.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.054134 portage-3.0.48/lib/portage/package/ebuild/_ipc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_metadata_invalid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.057467 portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4987 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/package/ebuild/_spawn_nofetch.py
+-rw-r--r--   0 root         (0) root         (0)   133992 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/config.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/package/ebuild/deprecated_profile_check.py
+-rw-r--r--   0 root         (0) root         (0)     6732 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/package/ebuild/digestcheck.py
+-rw-r--r--   0 root         (0) root         (0)     9424 2023-03-21 03:35:23.550205 portage-3.0.48/lib/portage/package/ebuild/digestgen.py
+-rw-r--r--   0 root         (0) root         (0)   111579 2023-04-29 04:41:37.948089 portage-3.0.48/lib/portage/package/ebuild/doebuild.py
+-rw-r--r--   0 root         (0) root         (0)    79658 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/package/ebuild/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     4689 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/package/ebuild/getmaskingreason.py
+-rw-r--r--   0 root         (0) root         (0)     6556 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/package/ebuild/getmaskingstatus.py
+-rw-r--r--   0 root         (0) root         (0)    19287 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/package/ebuild/prepare_build_dirs.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/package/ebuild/profile_iuse.py
+-rw-r--r--   0 root         (0) root         (0)    41702 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/process.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/proxy/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.060800 portage-3.0.48/lib/portage/proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7832 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/proxy/lazyimport.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/proxy/objectproxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/repository/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.48/lib/portage/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62136 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/repository/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/repository/storage/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.064134 portage-3.0.48/lib/portage/repository/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3951 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/repository/storage/hardlink_quarantine.py
+-rw-r--r--   0 root         (0) root         (0)    10940 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/repository/storage/hardlink_rcu.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/repository/storage/inplace.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/repository/storage/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/
+-rw-r--r--   0 root         (0) root         (0)     1589 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3015 2023-02-03 18:03:13.733528 portage-3.0.48/lib/portage/sync/config_checks.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/sync/controller.py
+-rw-r--r--   0 root         (0) root         (0)      696 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/sync/getaddrinfo_validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.067467 portage-3.0.48/lib/portage/sync/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/modules/cvs/
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-02-03 18:03:13.733528 portage-3.0.48/lib/portage/sync/modules/cvs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-02-03 18:03:13.730194 portage-3.0.48/lib/portage/sync/modules/cvs/cvs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/modules/git/
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-02-03 18:03:13.730194 portage-3.0.48/lib/portage/sync/modules/git/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20049 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/sync/modules/git/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/modules/mercurial/
+-rw-r--r--   0 root         (0) root         (0)     1403 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/sync/modules/mercurial/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6125 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/sync/modules/mercurial/mercurial.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/modules/rsync/
+-rw-r--r--   0 root         (0) root         (0)     1287 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/sync/modules/rsync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33953 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/sync/modules/rsync/rsync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/modules/svn/
+-rw-r--r--   0 root         (0) root         (0)     1037 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/sync/modules/svn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/sync/modules/svn/svn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/sync/modules/webrsync/
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-04-09 06:51:34.556710 portage-3.0.48/lib/portage/sync/modules/webrsync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-05-01 07:21:54.891482 portage-3.0.48/lib/portage/sync/modules/webrsync/webrsync.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/sync/old_tree_timestamp.py
+-rw-r--r--   0 root         (0) root         (0)    13139 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/sync/syncbase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/.gnupg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/.gnupg/openpgp-revocs.d/
+-rw-r--r--   0 root         (0) root         (0)     1850 2022-09-10 09:45:01.063717 portage-3.0.48/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev
+-rw-r--r--   0 root         (0) root         (0)     1852 2022-09-10 09:45:01.063717 portage-3.0.48/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/.gnupg/private-keys-v1.d/
+-rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.057050 portage-3.0.48/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key
+-rw-r--r--   0 root         (0) root         (0)     2055 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key
+-rw-r--r--   0 root         (0) root         (0)     2774 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/tests/.gnupg/pubring.kbx
+-rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/tests/.gnupg/trustdb.gpg
+-rw-r--r--   0 root         (0) root         (0)    11871 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/bin/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.48/lib/portage/tests/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.48/lib/portage/tests/bin/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/bin/setup_env.py
+-rw-r--r--   0 root         (0) root         (0)      547 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/bin/test_dobin.py
+-rw-r--r--   0 root         (0) root         (0)      565 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/bin/test_dodir.py
+-rw-r--r--   0 root         (0) root         (0)    13013 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/bin/test_doins.py
+-rw-r--r--   0 root         (0) root         (0)     9192 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/bin/test_eapi7_ver_funcs.py
+-rw-r--r--   0 root         (0) root         (0)     3083 2023-05-10 01:03:08.508755 portage-3.0.48/lib/portage/tests/bin/test_filter_bash_env.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-05-26 15:44:35.713957 portage-3.0.48/lib/portage/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/dbapi/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.074133 portage-3.0.48/lib/portage/tests/dbapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.074133 portage-3.0.48/lib/portage/tests/dbapi/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dbapi/test_auxdb.py
+-rw-r--r--   0 root         (0) root         (0)     6521 2023-02-03 18:03:13.730194 portage-3.0.48/lib/portage/tests/dbapi/test_bintree.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/dbapi/test_fakedbapi.py
+-rw-r--r--   0 root         (0) root         (0)     9409 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/dbapi/test_portdb_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/dep/
+-rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.077467 portage-3.0.48/lib/portage/tests/dep/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.077467 portage-3.0.48/lib/portage/tests/dep/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    24520 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/dep/testAtom.py
+-rw-r--r--   0 root         (0) root         (0)     9752 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/dep/testCheckRequiredUse.py
+-rw-r--r--   0 root         (0) root         (0)      779 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/dep/testExtendedAtomDict.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/dep/testExtractAffectingUSE.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/dep/testStandalone.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/dep/test_best_match_to_list.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_dep_getcpv.py
+-rw-r--r--   0 root         (0) root         (0)      988 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_dep_getrepo.py
+-rw-r--r--   0 root         (0) root         (0)      934 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_dep_getslot.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_dep_getusedeps.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_dnf_convert.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_get_operator.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_get_required_use_flags.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_isjustname.py
+-rw-r--r--   0 root         (0) root         (0)    11660 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_isvalidatom.py
+-rw-r--r--   0 root         (0) root         (0)    11132 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_match_from_list.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_overlap_dnf.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_paren_reduce.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/dep/test_soname_atom_pickle.py
+-rw-r--r--   0 root         (0) root         (0)    27656 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/dep/test_use_reduce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/ebuild/
+-rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.080800 portage-3.0.48/lib/portage/tests/ebuild/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.48/lib/portage/tests/ebuild/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/ebuild/test_array_fromfile_eof.py
+-rw-r--r--   0 root         (0) root         (0)    14001 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/ebuild/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     5947 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py
+-rw-r--r--   0 root         (0) root         (0)     5167 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/ebuild/test_doebuild_spawn.py
+-rw-r--r--   0 root         (0) root         (0)    35283 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/ebuild/test_fetch.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/ebuild/test_ipc_daemon.py
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/ebuild/test_shell_quote.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/ebuild/test_spawn.py
+-rw-r--r--   0 root         (0) root         (0)     4479 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/ebuild/test_use_expand_incremental.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/emerge/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.080800 portage-3.0.48/lib/portage/tests/emerge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.080800 portage-3.0.48/lib/portage/tests/emerge/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2022-12-24 02:35:49.845990 portage-3.0.48/lib/portage/tests/emerge/test_actions.py
+-rw-r--r--   0 root         (0) root         (0)    10338 2023-05-26 15:44:38.047315 portage-3.0.48/lib/portage/tests/emerge/test_config_protect.py
+-rw-r--r--   0 root         (0) root         (0)     6441 2023-05-26 15:44:38.047315 portage-3.0.48/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py
+-rw-r--r--   0 root         (0) root         (0)     6721 2023-05-26 15:44:38.047315 portage-3.0.48/lib/portage/tests/emerge/test_emerge_slot_abi.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/emerge/test_global_updates.py
+-rw-r--r--   0 root         (0) root         (0)    26471 2023-05-26 15:44:38.047315 portage-3.0.48/lib/portage/tests/emerge/test_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.248995 portage-3.0.48/lib/portage/tests/env/
+-rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/env/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/env/config/
+-rw-r--r--   0 root         (0) root         (0)      176 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/env/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/env/config/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/env/config/test_PackageKeywordsFile.py
+-rw-r--r--   0 root         (0) root         (0)      818 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/env/config/test_PackageMaskFile.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/env/config/test_PackageUseFile.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/env/config/test_PortageModulesFile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/glsa/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/glsa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/glsa/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/glsa/test_security_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/gpkg/
+-rw-r--r--   0 root         (0) root         (0)      102 2022-09-10 09:45:01.057050 portage-3.0.48/lib/portage/tests/gpkg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-09-10 09:45:01.057050 portage-3.0.48/lib/portage/tests/gpkg/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    13833 2022-09-20 03:21:13.396002 portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_checksum.py
+-rw-r--r--   0 root         (0) root         (0)    15728 2022-09-20 03:21:13.396002 portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_gpg.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2022-09-20 03:21:13.396002 portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_metadata_update.py
+-rw-r--r--   0 root         (0) root         (0)     5288 2022-09-20 03:21:13.396002 portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_metadata_url.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_path.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2022-09-20 03:21:13.396002 portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_size.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2022-09-20 03:21:13.396002 portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/lafilefixer/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/lafilefixer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/lafilefixer/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     6338 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/lafilefixer/test_lafilefixer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/lazyimport/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/lazyimport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.084133 portage-3.0.48/lib/portage/tests/lazyimport/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py
+-rw-r--r--   0 root         (0) root         (0)      596 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/lazyimport/test_preload_portage_submodules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/lint/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/lint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/lint/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      214 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/lint/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/lint/test_bash_syntax.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/lint/test_compile_modules.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/lint/test_import_modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/locks/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/locks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/locks/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     7850 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/locks/test_asynchronous_lock.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/locks/test_lock_nonblock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/news/
+-rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/news/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/news/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    14363 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/news/test_NewsItem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.252328 portage-3.0.48/lib/portage/tests/process/
+-rw-r--r--   0 root         (0) root         (0)      107 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.087467 portage-3.0.48/lib/portage/tests/process/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/process/test_AsyncFunction.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/process/test_PipeLogger.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/process/test_PopenProcess.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/process/test_PopenProcessBlockingIO.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2023-05-26 15:44:37.533976 portage-3.0.48/lib/portage/tests/process/test_poll.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-05-26 15:44:37.077305 portage-3.0.48/lib/portage/tests/process/test_spawn_fail_e2big.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-03-21 03:50:18.060757 portage-3.0.48/lib/portage/tests/process/test_spawn_warn_large_env.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2023-05-26 15:44:37.740645 portage-3.0.48/lib/portage/tests/process/test_unshare_net.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/resolver/
+-rw-r--r--   0 root         (0) root         (0)    42502 2023-03-21 03:50:18.064091 portage-3.0.48/lib/portage/tests/resolver/ResolverPlayground.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.48/lib/portage/tests/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.104133 portage-3.0.48/lib/portage/tests/resolver/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/resolver/binpkg_multi_instance/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.48/lib/portage/tests/resolver/binpkg_multi_instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.104133 portage-3.0.48/lib/portage/tests/resolver/binpkg_multi_instance/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     5585 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py
+-rw-r--r--   0 root         (0) root         (0)     3747 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/resolver/soname/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/resolver/soname/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/resolver/soname/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_autounmask.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_depclean.py
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3840 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_or_choices.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_reinstall.py
+-rw-r--r--   0 root         (0) root         (0)     3338 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_skip_update.py
+-rw-r--r--   0 root         (0) root         (0)    12877 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_slot_conflict_update.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_soname_provided.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/soname/test_unsatisfiable.py
+-rw-r--r--   0 root         (0) root         (0)     3354 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/soname/test_unsatisfied.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)    28432 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_autounmask.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_autounmask_binpkg_use.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_autounmask_keep_keywords.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-05-26 15:44:37.740645 portage-3.0.48/lib/portage/tests/resolver/test_autounmask_multilib_use.py
+-rw-r--r--   0 root         (0) root         (0)     1279 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_autounmask_parent.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_autounmask_use_backtrack.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_autounmask_use_breakage.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-05-26 15:44:36.773968 portage-3.0.48/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/resolver/test_backtracking.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_bdeps.py
+-rw-r--r--   0 root         (0) root         (0)     4927 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/resolver/test_blocker.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_changed_deps.py
+-rw-r--r--   0 root         (0) root         (0)     7899 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_circular_choices.py
+-rw-r--r--   0 root         (0) root         (0)     3341 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_circular_choices_rust.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_circular_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)     4948 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_complete_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py
+-rw-r--r--   0 root         (0) root         (0)     9959 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_depclean.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_depclean_order.py
+-rw-r--r--   0 root         (0) root         (0)     2443 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_depclean_slot_unavailable.py
+-rw-r--r--   0 root         (0) root         (0)    13128 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_depth.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_disjunctive_depend_order.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_eapi.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_features_test_use.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2022-09-10 09:45:01.057050 portage-3.0.48/lib/portage/tests/resolver/test_installkernel.py
+-rw-r--r--   0 root         (0) root         (0)    11063 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_keywords.py
+-rw-r--r--   0 root         (0) root         (0)    31088 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_merge_order.py
+-rw-r--r--   0 root         (0) root         (0)     1234 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_multirepo.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/resolver/test_multislot.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2022-09-10 09:44:56.963689 portage-3.0.48/lib/portage/tests/resolver/test_old_dep_chain_display.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_onlydeps.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_onlydeps_circular.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_onlydeps_ideps.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_onlydeps_minimal.py
+-rw-r--r--   0 root         (0) root         (0)    25154 2023-05-26 15:44:37.740645 portage-3.0.48/lib/portage/tests/resolver/test_or_choices.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_or_downgrade_installed.py
+-rw-r--r--   0 root         (0) root         (0)     6850 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_or_upgrade_installed.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_output.py
+-rw-r--r--   0 root         (0) root         (0)     9049 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_package_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_profile_default_eapi.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_profile_package_set.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py
+-rw-r--r--   0 root         (0) root         (0)    11792 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_required_use.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_simple.py
+-rw-r--r--   0 root         (0) root         (0)    18128 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_abi.py
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_abi_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_change_without_revbump.py
+-rw-r--r--   0 root         (0) root         (0)    13393 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_collisions.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_mask_update.py
+-rw-r--r--   0 root         (0) root         (0)    14826 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     7910 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py
+-rw-r--r--   0 root         (0) root         (0)     2579 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_update.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_update_virt.py
+-rw-r--r--   0 root         (0) root         (0)     5024 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_autounmask.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_bdeps.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_complete_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4694 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py
+-rw-r--r--   0 root         (0) root         (0)     4366 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_missed_update.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_required_use.py
+-rw-r--r--   0 root         (0) root         (0)     9190 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_unsolved.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/tests/resolver/test_targetroot.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py
+-rw-r--r--   0 root         (0) root         (0)    11321 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/tests/resolver/test_unmerge_order.py
+-rw-r--r--   0 root         (0) root         (0)     3843 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_update.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_use_dep_defaults.py
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_useflags.py
+-rw-r--r--   0 root         (0) root         (0)     9976 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_virtual_minimize_children.py
+-rw-r--r--   0 root         (0) root         (0)     9326 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/resolver/test_virtual_slot.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/resolver/test_with_test_deps.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-05-26 15:44:35.863958 portage-3.0.48/lib/portage/tests/runTests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/sets/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/sets/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/base/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/sets/base/testInternalPackageSet.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/sets/base/testVariableSet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/sets/files/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/files/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/sets/files/testConfigFileSet.py
+-rw-r--r--   0 root         (0) root         (0)      829 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/sets/files/testStaticFileSet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/sets/shell/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sets/shell/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/sets/shell/testShell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/sync/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sync/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/sync/__test__.py
+-rw-r--r--   0 root         (0) root         (0)    16481 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/sync/test_sync_local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/unicode/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/unicode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.107466 portage-3.0.48/lib/portage/tests/unicode/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/unicode/test_string_format.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/update/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.110799 portage-3.0.48/lib/portage/tests/update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.110799 portage-3.0.48/lib/portage/tests/update/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/update/test_move_ent.py
+-rw-r--r--   0 root         (0) root         (0)     5444 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/update/test_move_slot_ent.py
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/update/test_update_dbentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/util/
+-rw-r--r--   0 root         (0) root         (0)      170 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/util/dyn_libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/dyn_libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/dyn_libs/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/util/dyn_libs/test_soname_deps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/util/eventloop/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/eventloop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/eventloop/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      826 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/eventloop/test_call_soon_fifo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/util/file_copy/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/file_copy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/file_copy/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-05-26 15:44:37.383975 portage-3.0.48/lib/portage/tests/util/file_copy/test_copyfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.255662 portage-3.0.48/lib/portage/tests/util/futures/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/futures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.114133 portage-3.0.48/lib/portage/tests/util/futures/__test__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/tests/util/futures/asyncio/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.48/lib/portage/tests/util/futures/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.48/lib/portage/tests/util/futures/asyncio/__test__.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_child_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py
+-rw-r--r--   0 root         (0) root         (0)     5394 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py
+-rw-r--r--   0 root         (0) root         (0)      795 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py
+-rw-r--r--   0 root         (0) root         (0)     7135 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/futures/test_compat_coroutine.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/futures/test_done_callback.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/util/futures/test_done_callback_after_exit.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/futures/test_iter_completed.py
+-rw-r--r--   0 root         (0) root         (0)    10828 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/futures/test_retry.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:50:18.064091 portage-3.0.48/lib/portage/tests/util/test_checksum.py
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/test_digraph.py
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/test_file_copier.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/test_getconfig.py
+-rw-r--r--   0 root         (0) root         (0)      315 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/util/test_grabdict.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/test_install_mask.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2022-12-24 02:35:49.845990 portage-3.0.48/lib/portage/tests/util/test_manifest.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2022-09-10 09:45:01.057050 portage-3.0.48/lib/portage/tests/util/test_mtimedb.py
+-rw-r--r--   0 root         (0) root         (0)      440 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/test_normalizedPath.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-09 06:49:46.516103 portage-3.0.48/lib/portage/tests/util/test_shelve.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/test_socks5.py
+-rw-r--r--   0 root         (0) root         (0)      832 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/util/test_stackDictList.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/tests/util/test_stackDicts.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/test_stackLists.py
+-rw-r--r--   0 root         (0) root         (0)      897 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/tests/util/test_uniqueArray.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/test_varExpand.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-05-26 15:44:37.383975 portage-3.0.48/lib/portage/tests/util/test_whirlpool.py
+-rw-r--r--   0 root         (0) root         (0)     6243 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/util/test_xattr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/tests/versions/
+-rw-r--r--   0 root         (0) root         (0)      174 2021-11-12 08:15:36.117466 portage-3.0.48/lib/portage/tests/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.48/lib/portage/tests/versions/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/versions/test_cpv_sort_key.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/versions/test_vercmp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/tests/xpak/
+-rw-r--r--   0 root         (0) root         (0)      169 2021-11-12 08:15:36.117466 portage-3.0.48/lib/portage/tests/xpak/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.117466 portage-3.0.48/lib/portage/tests/xpak/__test__.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/tests/xpak/test_decodeint.py
+-rw-r--r--   0 root         (0) root         (0)    17014 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/ExtractKernelVersion.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/SlotObject.py
+-rw-r--r--   0 root         (0) root         (0)    68707 2023-03-21 03:50:18.064091 portage-3.0.48/lib/portage/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/_async/
+-rw-r--r--   0 root         (0) root         (0)     2609 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/_async/AsyncFunction.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/_async/AsyncScheduler.py
+-rw-r--r--   0 root         (0) root         (0)      963 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/_async/AsyncTaskFuture.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/_async/BuildLogger.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/_async/FileCopier.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/_async/FileDigester.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_async/ForkProcess.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_async/PipeLogger.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_async/PipeReaderBlockingIO.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_async/PopenProcess.py
+-rw-r--r--   0 root         (0) root         (0)     4501 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_async/SchedulerInterface.py
+-rw-r--r--   0 root         (0) root         (0)      644 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/_async/TaskScheduler.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.127466 portage-3.0.48/lib/portage/util/_async/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/_async/run_main_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/_compare_files.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/_ctypes.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/_desktop_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/_dyn_libs/
+-rw-r--r--   0 root         (0) root         (0)    41425 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_dyn_libs/LinkageMapELF.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/_dyn_libs/NeededEntry.py
+-rw-r--r--   0 root         (0) root         (0)     9385 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.130799 portage-3.0.48/lib/portage/util/_dyn_libs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_dyn_libs/display_preserved_libs.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/_dyn_libs/dyn_libs.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_dyn_libs/soname_deps.py
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_dyn_libs/soname_deps_qa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/_eventloop/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.134132 portage-3.0.48/lib/portage/util/_eventloop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5849 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/_eventloop/asyncio_event_loop.py
+-rw-r--r--   0 root         (0) root         (0)      213 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/_eventloop/global_event_loop.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_get_vm_info.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/_info_files.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/_path.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/_pty.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/util/_urlopen.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/_xattr.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/bin_entry_point.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/compression_probe.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/configparser.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2022-12-24 02:35:49.845990 portage-3.0.48/lib/portage/util/cpuinfo.py
+-rw-r--r--   0 root         (0) root         (0)    12975 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/digraph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/elf/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.48/lib/portage/util/elf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/elf/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/elf/header.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/endian/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.137466 portage-3.0.48/lib/portage/util/endian/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1303 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/endian/decode.py
+-rw-r--r--   0 root         (0) root         (0)    15592 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/env_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/file_copy/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/file_copy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/formatter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/futures/
+-rw-r--r--   0 root         (0) root         (0)      180 2022-09-10 09:44:56.967023 portage-3.0.48/lib/portage/util/futures/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/futures/_asyncio/
+-rw-r--r--   0 root         (0) root         (0)     9758 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/futures/_asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/futures/_asyncio/streams.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/futures/_sync_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/futures/compat_coroutine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/futures/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-12 08:15:36.140799 portage-3.0.48/lib/portage/util/futures/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/futures/executor/fork.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/futures/extendedfutures.py
+-rw-r--r--   0 root         (0) root         (0)      516 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/futures/futures.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/futures/iter_completed.py
+-rw-r--r--   0 root         (0) root         (0)     6297 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/futures/retry.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/futures/unix_events.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     6549 2022-09-10 09:45:01.060384 portage-3.0.48/lib/portage/util/install_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/util/iterators/
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/iterators/MultiIterGroupBy.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.144132 portage-3.0.48/lib/portage/util/iterators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7349 2022-09-10 09:45:01.063717 portage-3.0.48/lib/portage/util/lafilefixer.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/listdir.py
+-rw-r--r--   0 root         (0) root         (0)     4339 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/locale.py
+-rw-r--r--   0 root         (0) root         (0)    14806 2023-05-23 00:22:09.516487 portage-3.0.48/lib/portage/util/movefile.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/mtimedb.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/netlink.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2022-09-10 09:44:56.970356 portage-3.0.48/lib/portage/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2022-09-10 09:45:01.057050 portage-3.0.48/lib/portage/util/shelve.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/socks5.py
+-rw-r--r--   0 root         (0) root         (0)    58416 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/util/whirlpool.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-03-21 03:35:23.553538 portage-3.0.48/lib/portage/util/writeable_check.py
+-rw-r--r--   0 root         (0) root         (0)    19275 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/lib/portage/xml/
+-rw-r--r--   0 root         (0) root         (0)      102 2021-11-12 08:15:36.147466 portage-3.0.48/lib/portage/xml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16789 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/xml/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    19413 2023-03-21 03:35:23.556871 portage-3.0.48/lib/portage/xpak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/misc/
+-rwxr-xr-x   0 root         (0) root         (0)    24116 2023-02-03 18:03:13.736861 portage-3.0.48/misc/emerge-delta-webrsync
+-rwxr-xr-x   0 root         (0) root         (0)    29844 2023-06-01 01:20:09.289416 portage-3.0.48/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 01:26:11.258995 portage-3.0.48/src/
+-rw-r--r--   0 root         (0) root         (0)    71291 2023-03-21 03:35:23.556871 portage-3.0.48/src/portage_util__whirlpool.c
+-rw-r--r--   0 root         (0) root         (0)    13384 2023-03-21 03:35:23.556871 portage-3.0.48/src/portage_util_file_copy_reflink_linux.c
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-03-21 03:35:23.556871 portage-3.0.48/src/portage_util_libc.c
```

### Comparing `portage-3.0.47/DEVELOPING` & `portage-3.0.48/DEVELOPING`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/LICENSE` & `portage-3.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/PKG-INFO` & `portage-3.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portage
-Version: 3.0.47
+Version: 3.0.48
 Summary: Portage is the package management and distribution system for Gentoo
 Home-page: https://wiki.gentoo.org/wiki/Project:Portage
 Author: Gentoo Portage Development Team
 Author-email: dev-portage@gentoo.org
 License: GPLV2
 Project-URL: Release Notes, https://gitweb.gentoo.org/proj/portage.git/plain/NEWS
 Project-URL: Documentation, https://wiki.gentoo.org/wiki/Handbook:AMD64/Working/Portage
```

### Comparing `portage-3.0.47/TEST-NOTES` & `portage-3.0.48/TEST-NOTES`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/archive-conf` & `portage-3.0.48/bin/archive-conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/bashrc-functions.sh` & `portage-3.0.48/bin/bashrc-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/binhost-snapshot` & `portage-3.0.48/bin/binhost-snapshot`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/chmod-lite.py` & `portage-3.0.48/bin/chmod-lite.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/chpathtool.py` & `portage-3.0.48/bin/chpathtool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/clean_locks` & `portage-3.0.48/bin/clean_locks`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/dispatch-conf` & `portage-3.0.48/bin/dispatch-conf`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/dohtml.py` & `portage-3.0.48/bin/dohtml.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/doins.py` & `portage-3.0.48/bin/doins.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/eapi.sh` & `portage-3.0.48/bin/eapi.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/eapi7-ver-funcs.sh` & `portage-3.0.48/bin/eapi7-ver-funcs.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild` & `portage-3.0.48/bin/ebuild`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/bsd/sed` & `portage-3.0.48/bin/ebuild-helpers/bsd/sed`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dobin` & `portage-3.0.48/bin/ebuild-helpers/dobin`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/doconfd` & `portage-3.0.48/bin/ebuild-helpers/doconfd`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dodoc` & `portage-3.0.48/bin/ebuild-helpers/dodoc`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/doenvd` & `portage-3.0.48/bin/ebuild-helpers/doenvd`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/doexe` & `portage-3.0.48/bin/ebuild-helpers/doexe`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dohard` & `portage-3.0.48/bin/ebuild-helpers/dohard`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/doheader` & `portage-3.0.48/bin/ebuild-helpers/doheader`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dohtml` & `portage-3.0.48/bin/ebuild-helpers/dohtml`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/doinfo` & `portage-3.0.48/bin/ebuild-helpers/doinfo`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/doins` & `portage-3.0.48/bin/ebuild-helpers/doins`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dolib` & `portage-3.0.48/bin/ebuild-helpers/dolib`

 * *Files 17% similar despite different names*

```diff
@@ -18,23 +18,21 @@
 		die "${0##*/}: \${DESTTREE} has been banned for EAPI '${EAPI}'; use 'into' instead"
 else
 	# backwards compatibility
 	__E_DESTTREE=${DESTTREE}
 fi
 
 # Setup ABI cruft
-LIBDIR_VAR="LIBDIR_${ABI}"
-if [[ -n ${ABI} && -n ${!LIBDIR_VAR} ]] ; then
-	CONF_LIBDIR=${!LIBDIR_VAR}
+libdir="lib"
+libdir_var="LIBDIR_${ABI}"
+if [[ -n ${ABI} && -n ${!libdir_var} ]] ; then
+	libdir=${!libdir_var}
 fi
-unset LIBDIR_VAR
 
-# We need this to default to lib so that things dont break
-CONF_LIBDIR=${CONF_LIBDIR:-lib}
-libdir="${ED%/}/${__E_DESTTREE#/}/${CONF_LIBDIR}"
+libdir="${ED%/}/${__E_DESTTREE#/}/${libdir}"
 
 if [[ $# -lt 1 ]] ; then
 	__helpers_die "${0##*/}: at least one argument needed"
 	exit 1
 fi
 if [[ ! -d ${libdir} ]] ; then
 	install -d "${libdir}" || { __helpers_die "${0##*/}: failed to install ${libdir}"; exit 1; }
```

### Comparing `portage-3.0.47/bin/ebuild-helpers/doman` & `portage-3.0.48/bin/ebuild-helpers/doman`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/domo` & `portage-3.0.48/bin/ebuild-helpers/domo`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dosbin` & `portage-3.0.48/bin/ebuild-helpers/dosbin`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dosed` & `portage-3.0.48/bin/ebuild-helpers/dosed`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/dosym` & `portage-3.0.48/bin/ebuild-helpers/dosym`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/emake` & `portage-3.0.48/bin/ebuild-helpers/emake`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/fperms` & `portage-3.0.48/bin/ebuild-helpers/fperms`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/env bash
-# Copyright 1999-2018 Gentoo Foundation
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/isolated-functions.sh || exit 1
 
 if ! ___eapi_has_prefix_variables; then
 	ED=${D}
 fi
 
+args=()
 got_mode=
 for arg; do
 	# - can either be an option or a mode string
-	[[ ${arg} == -* && ${arg} != -[ugorwxXst] ]] && continue
-
-	if [[ ! ${got_mode} ]]; then
+	if [[ ${arg} == -* && ${arg} != -[ugorwxXst] ]]; then
+		args+=( "${arg}" )
+	elif [[ ! ${got_mode} ]]; then
+		# the first non-option is the mode and must not be prefixed
 		got_mode=1
-		continue
-	fi
-
-	if [[ ${arg} != /* ]]; then
-		eqawarn "Relative path passed to '${0##*/}': ${arg}"
-		eqawarn "This is unsupported. Please use 'chmod' when you need to work on files"
-		eqawarn "outside the installation image (\${ED})."
+		args+=( "${arg}" )
+	else
+		args+=( "${ED%/}/${arg#/}" )
+		# remove the QA warning after 2024-12-31
+		if [[ ${arg:0:1} != / ]]; then
+			eqawarn "${0##*/}: Path '${arg}' does not start with '/'."
+			eqawarn "This is unsupported. Add a slash for a path in \${ED},"
+			eqawarn "or use 'chmod' for a path relative to the working dir."
+		fi
 	fi
 done
 
-# we can't prefix all arguments because
-# chmod takes random options
-slash="/"
-chmod "${@/#${slash}/${ED%/}${slash}}"
+chmod "${args[@]}"
 ret=$?
 [[ ${ret} -ne 0 ]] && __helpers_die "${0##*/} failed"
 exit ${ret}
```

### Comparing `portage-3.0.47/bin/ebuild-helpers/newins` & `portage-3.0.48/bin/ebuild-helpers/newins`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/prepinfo` & `portage-3.0.48/bin/ebuild-helpers/prepinfo`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/unprivileged/chown` & `portage-3.0.48/bin/ebuild-helpers/unprivileged/chown`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-helpers/xattr/install` & `portage-3.0.48/bin/ebuild-helpers/xattr/install`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-ipc.py` & `portage-3.0.48/bin/ebuild-ipc.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ebuild-pyhelper` & `portage-3.0.48/bin/ebuild-pyhelper`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 2010-2021 Gentoo Authors
+# Copyright 2010-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 export __PORTAGE_HELPER_CWD=${PWD}
 
 if [[ ${0##*/} == "ebuild-pyhelper" ]]; then
 	echo "ebuild-pyhelper: must be called via symlink" &>2
 	exit 1
@@ -14,8 +14,8 @@
 for path in "${PORTAGE_BIN_PATH}/${0##*/}"{.py,}; do
 	if [[ -x "${path}" ]]; then
 		PYTHONPATH=${PORTAGE_PYTHONPATH:-${PORTAGE_PYM_PATH}} \
 			exec "${PORTAGE_PYTHON:-/usr/bin/python}" "${path}" "$@"
 	fi
 done
 echo "File not found: ${path}" >&2
-exit 1
+exit 127
```

### Comparing `portage-3.0.47/bin/ebuild.sh` & `portage-3.0.48/bin/ebuild.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ecompress` & `portage-3.0.48/bin/ecompress`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/ecompress-file` & `portage-3.0.48/bin/ecompress-file`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/egencache` & `portage-3.0.48/bin/egencache`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/emaint` & `portage-3.0.48/bin/emaint`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/emerge` & `portage-3.0.48/bin/emerge`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/emerge-webrsync` & `portage-3.0.48/bin/emerge-webrsync`

 * *Files 4% similar despite different names*

```diff
@@ -105,54 +105,59 @@
 	renice "${PORTAGE_NICENESS}" $$ > /dev/null
 fi
 
 do_debug=0
 keep=false
 
 handle_pgp_setup() {
-	has webrsync-gpg ${FEATURES} && webrsync_gpg=1 || webrsync_gpg=0
+	# WEBRSYNC_VERIFY_SIGNATURE=0: disable PGP verification
+	# WEBRSYNC_VERIFY_SIGNATURE=1: use gemato for verification, fallback to regular gpg
+	# WEBRSYNC_VERIFY_SIGNATURE=2: use legacy FEATURES="webrsync-gpg"
+	WEBRSYNC_VERIFY_SIGNATURE=1
 
-	if [[ ${webrsync_gpg} -eq 1 ]]; then
-		ewarn "FEATURES=webrsync-gpg is deprecated, see the make.conf(5) man page."
-	fi
+	has webrsync-gpg ${FEATURES} && webrsync_gpg=1 || webrsync_gpg=0
 
 	repo_has_webrsync_verify=$(
 		has $(__repo_attr "${repo_name}" sync-webrsync-verify-signature	| LC_ALL=C tr '[:upper:]' '[:lower:]') true yes
 	)
 
-	# WEBRSYNC_VERIFY_SIGNATURE=0: disable PGP verification
-	# WEBRSYNC_VERIFY_SIGNATURE=1: use gemato for verification, fallback to regular gpg
-	# WEBRSYNC_VERIFY_SIGNATURE=2: use legacy FEATURES="webrsync-gpg"
-	WEBRSYNC_VERIFY_SIGNATURE=1
-
 	if [[ -n ${PORTAGE_TEMP_GPG_DIR} ]] || [[ ${repo_has_webrsync_verify} -eq 1 ]]; then
 		# If FEATURES=webrsync-gpg is enabled then allow direct emerge-webrsync
 		# calls for backward compatibility (this triggers a deprecation warning
 		# above). Since direct emerge-webrsync calls do not use gemato for secure
 		# key refresh, this behavior will not be supported in a future release.
 		if [[ ! ( -d ${PORTAGE_GPG_DIR} && ${webrsync_gpg} -eq 1 ) && -z ${PORTAGE_TEMP_GPG_DIR} ]]; then
 			die "Do not call ${argv0##*/} directly, instead call emerge --sync or emaint sync."
 		fi
 
-		WEBRSYNC_VERIFY_SIGNATURE=2
-	elif has webrsync-gpg ${FEATURES}; then
+		# Use gemato for the standard Portage-calling-us case w/ sync-type='webrsync'.
+		WEBRSYNC_VERIFY_SIGNATURE=1
+	elif [[ ${webrsync_gpg} -eq 1 ]]; then
+		# We only warn if FEATURES="webrsync-gpg" is in make.conf, not if
+		# Portage is calling us for 'sync-type=webrsync' with verification, because
+		# that path uses gemato now (plus the user can't help it, obviously).
+		ewarn "FEATURES=webrsync-gpg is deprecated, see the make.conf(5) man page."
 		WEBRSYNC_VERIFY_SIGNATURE=2
 	elif [[ -n ${no_pgp_verify} ]]; then
 		WEBRSYNC_VERIFY_SIGNATURE=0
+	else
+		# The default at the beginning of handle_pgp_setup is WEBRSYNC_VERIFY_SIGNATURE=1
+		# i.e. gemato.
+		:;
 	fi
 
 	case "${WEBRSYNC_VERIFY_SIGNATURE}" in
 		0)
 			[[ ${PORTAGE_QUIET} -eq 1 ]] || ewarn "PGP verification method: disabled"
 			;;
 		1)
 			[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "PGP verification method: gemato"
 			;;
 		2)
-			ewarn "PGP verification method: legacy FEATURES=webrsync-gpg"
+			ewarn "PGP verification method: legacy gpg path"
 			;;
 		*)
 			die "Unknown WEBRSYNC_VERIFY_SIGNATURE state: \${WEBRSYNC_VERIFY_SIGNATURE}=${WEBRSYNC_VERIFY_SIGNATURE}"
 			;;
 	esac
 
 	if [[ -n ${PORTAGE_TEMP_GPG_DIR} ]]; then
@@ -264,42 +269,75 @@
 
 check_file_signature_gemato() {
 	local signature="$1"
 	local file="$2"
 	local r=1
 
 	if type -P gemato > /dev/null; then
+		if [[ -n ${PORTAGE_GPG_KEY} ]] ; then
+			local key="${PORTAGE_GPG_KEY}"
+		else
+			local key="${EPREFIX:-/}"/usr/share/openpgp-keys/gentoo-release.asc
+		fi
+
+		local keyserver
+		if [[ -n ${PORTAGE_GPG_KEY_SERVER} ]] ; then
+			keyserver="--keyserver ${PORTAGE_GPG_KEY_SERVER}"
+		fi
+
 		local gemato_args=(
 			openpgp-verify-detached
-			-K /usr/share/openpgp-keys/gentoo-release.asc
+			-K "${key}"
 		)
 
+		[[ -n ${PORTAGE_GPG_KEY_SERVER} ]] && gemato_args+=( --keyserver "${PORTAGE_GPG_KEY_SERVER}" )
 		[[ ${PORTAGE_QUIET} == 1 ]] && gemato_args+=( --quiet )
 		[[ ${do_debug} == 1 ]] && gemato_args+=( --debug )
 
-		gemato "${gemato_args[@]}" "${signature}" "${file}"
+		gemato "${gemato_args[@]}" -- "${signature}" "${file}"
 		r=$?
 
 		if [[ ${r} -ne 0 ]]; then
 			# Exit early since it's typically inappropriate to
 			# try other mirrors in this case (it may indicate
 			# a keyring problem).
 			die "signature verification failed"
 		fi
+	else
+		return 127
 	fi
 
 	return "${r}"
 }
 
 check_file_signature_gpg_unwrapped() {
 	local signature="$1"
 	local file="$2"
 
 	if type -P gpg > /dev/null; then
-		if gnupg_status=$(gpg --homedir "${PORTAGE_GPG_DIR}" --batch \
+		if [[ -n ${PORTAGE_GPG_KEY} ]] ; then
+			local key="${PORTAGE_GPG_KEY}"
+		else
+			local key="${EPREFIX:-/}"/usr/share/openpgp-keys/gentoo-release.asc
+		fi
+
+		local gpgdir="${PORTAGE_GPG_DIR}"
+		if [[ -z ${gpgdir} ]] ; then
+			gpgdir=$(mktemp -d "${PORTAGE_TMPDIR}/portage/webrsync-XXXXXX")
+			if [[ ! -w ${gpgdir} ]] ; then
+				die "gpgdir is not writable: ${gpgdir}"
+			fi
+
+			# If we're created our own temporary directory, it's okay for us
+			# to import the keyring by ourselves. But we'll avoid doing it
+			# if the user has set PORTAGE_GPG_DIR by themselves.
+			gpg --no-default-keyring --homedir "${gpgdir}" --batch --import "${key}"
+		fi
+
+		if gnupg_status=$(gpg --no-default-keyring --homedir "${gpgdir}" --batch \
 			--status-fd 1 --verify "${signature}" "${file}"); then
 			while read -r line; do
 				if [[ ${line} == "[GNUPG:] GOODSIG"* ]]; then
 					r=0
 					break
 				fi
 			done <<< "${gnupg_status}"
@@ -325,20 +363,32 @@
 	if [[ ${WEBRSYNC_VERIFY_SIGNATURE} != 0 ]]; then
 		[[ ${PORTAGE_QUIET} -eq 1 ]] || einfo "Checking signature ..."
 
 		case ${WEBRSYNC_VERIFY_SIGNATURE} in
 			1)
 				check_file_signature_gemato "${signature}" "${file}"
 				r=$?
+
+				if [[ ${r} -eq 127 ]] ; then
+					ewarn "Falling back to gpg as gemato is not installed"
+					check_file_signature_gpg_unwrapped "${signature}" "${file}"
+					r=$?
+				fi
+
 				;;
 			2)
 				check_file_signature_gpg_unwrapped "${signature}" "${file}"
 				r=$?
 				;;
 		esac
+
+		if [[ ${r} != 0 ]] ; then
+			eerror "Error occurred in check_file_signature: ${r}. Aborting."
+			die "Verification error occured."
+		fi
 	else
 		r=0
 	fi
 
 	return "${r}"
 }
 
@@ -539,15 +589,15 @@
 	existing_timestamp=$(get_repository_timestamp)
 	start_time=$(get_utc_date_in_seconds)
 	start_hour=$(get_date_part "${start_time}" "%H")
 
 	# Daily snapshots are created at 00:45 and are not
 	# available until after 01:00. Don't waste time trying
 	# to fetch a snapshot before it's been created.
-	if [[ ${start_hour} -lt 1 ]] ; then
+	if [[ ${start_hour#0} -lt 1 ]] ; then
 		(( start_time -= 86400 ))
 	fi
 
 	snapshot_date=$(get_date_part "${start_time}" "%Y%m%d")
 	snapshot_date_seconds=$(get_utc_second_from_string "${snapshot_date}")
 
 	while (( ${attempts} < 40 )) ; do
```

### Comparing `portage-3.0.47/bin/emirrordist` & `portage-3.0.48/bin/emirrordist`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/env-update` & `portage-3.0.48/bin/env-update`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/estrip` & `portage-3.0.48/bin/estrip`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env bash
-# Copyright 1999-2019 Gentoo Authors
+# Copyright 1999-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 source "${PORTAGE_BIN_PATH}"/helper-functions.sh || exit 1
 
 # avoid multiple calls to `has`.  this creates things like:
 #   FEATURES_foo=false
 # if "foo" is not in ${FEATURES}
@@ -110,15 +110,20 @@
 
 			unset scanelf_results needed_entry needed_entry_file find_path
 		fi
 
 		exit 0
 		;;
 	--dequeue)
-		[[ -n ${2} ]] && die "${0##*/}: --dequeue takes no additional arguments"
+		[[ $# -eq 1 ]] || die "${0##*/}: $1 takes no additional arguments"
+		break
+		;;
+	--prepallstrip)
+		[[ $# -eq 1 ]] || die "${0##*/}: $1 takes no additional arguments"
+		prepstrip=true
 		break
 		;;
 	*)
 		die "${0##*/}: unknown arguments '$*'"
 		exit 1
 		;;
 	esac
```

### Comparing `portage-3.0.47/bin/etc-update` & `portage-3.0.48/bin/etc-update`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/filter-bash-environment.py` & `portage-3.0.48/bin/filter-bash-environment.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/fixpackages` & `portage-3.0.48/bin/fixpackages`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/glsa-check` & `portage-3.0.48/bin/glsa-check`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/gpkg-helper.py` & `portage-3.0.48/bin/gpkg-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/gpkg-sign` & `portage-3.0.48/bin/gpkg-sign`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/helper-functions.sh` & `portage-3.0.48/bin/helper-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/05prefix` & `portage-3.0.48/bin/install-qa-check.d/05prefix`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/10executable-issues` & `portage-3.0.48/bin/install-qa-check.d/10executable-issues`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/10ignored-flags` & `portage-3.0.48/bin/install-qa-check.d/10ignored-flags`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/20runtime-directories` & `portage-3.0.48/bin/install-qa-check.d/20runtime-directories`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/60bash-completion` & `portage-3.0.48/bin/install-qa-check.d/60bash-completion`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/60openrc` & `portage-3.0.48/bin/install-qa-check.d/60openrc`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/60pkgconfig` & `portage-3.0.48/bin/install-qa-check.d/60pkgconfig`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/60pngfix` & `portage-3.0.48/bin/install-qa-check.d/60pngfix`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/60systemd` & `portage-3.0.48/bin/install-qa-check.d/60systemd`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/80libraries` & `portage-3.0.48/bin/install-qa-check.d/80libraries`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/80multilib-strict` & `portage-3.0.48/bin/install-qa-check.d/80multilib-strict`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/90bad-bin-group-write` & `portage-3.0.48/bin/install-qa-check.d/90bad-bin-group-write`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/90bad-bin-owner` & `portage-3.0.48/bin/install-qa-check.d/90bad-bin-owner`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/90cmake-warnings` & `portage-3.0.48/bin/install-qa-check.d/90cmake-warnings`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/90config-impl-decl` & `portage-3.0.48/bin/install-qa-check.d/90config-impl-decl`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,46 @@
 # systemd-utils: work/systemd-stable-251.10-abi_x86_64.amd64/meson-logs/meson-log.txt
 #                ^---  can be non-autotools
 #
 # Adapted from macports portconfigure.tcl with love.
 #
 # See also: bug 892651
 
+# Same as the "has" function, but allows wildcards in the array
+is_in() {
+	local needle=$1
+	shift
+
+	local x
+	for x in "$@"; do
+		[[ "${needle}" = ${x} ]] && return 0
+	done
+	return 1
+}
+
+add_default_skips() {
+	# Skip built-in functions provided by the compiler
+	QA_CONFIG_IMPL_DECL_SKIP+=(
+		"__builtin_*"
+		# https://gcc.gnu.org/onlinedocs/gcc/_005f_005fsync-Builtins.html
+		"__sync_*"
+		# https://gcc.gnu.org/onlinedocs/gcc/_005f_005fatomic-Builtins.html
+		"__atomic_*"
+	)
+
+	# Functions not available on Linux
+	[[ ${CHOST} == *linux* ]] && QA_CONFIG_IMPL_DECL_SKIP+=(
+		acl
+		acl_get_perm_np
+		res_getservers
+		res_ndestroy
+		statacl
+	)
+}
+
 find_log_targets() {
 	local log_targets=(
 		'config.log'
 		'CMakeError.log'
 		'meson-log.txt'
 	)
 	local find_args=()
@@ -52,14 +84,16 @@
 	local entry
 	local line
 	local func
 	local re_uni
 	local re_asc
 	local is_utf8
 
+	add_default_skips
+
 	# Given the UTF-8 character type, both gcc and clang may enclose the
 	# function name between the LEFT SINGLE QUOTATION MARK and RIGHT SINGLE
 	# QUOTATION MARK codepoints.
 	re_uni=$' function \u2018([^\u2019]+)\u2019'
 
 	# This variant matches ASCII single quotes.
 	re_asc=$' function \x27([^\x27]+)\x27'
@@ -76,15 +110,15 @@
 			line="${entry%%:*}"
 			if [[ ${is_utf8} -eq 1 && ${entry} =~ ${re_uni} ]] || [[ ${entry} =~ ${re_asc} ]]; then
 				func="${BASH_REMATCH[1]}"
 			else
 				continue
 			fi
 
-			has "${func}" "${QA_CONFIG_IMPL_DECL_SKIP[@]}" && continue
+			is_in "${func}" "${QA_CONFIG_IMPL_DECL_SKIP[@]}" && continue
 
 			files+=( "${l}" )
 			lines+=( "${line}" )
 			funcs+=( "${func}" )
 		# Using -I to ignore binary files is a GNU extension for grep
 		done 3< <(grep -nEI -e '-W(error=)?implicit-function-declaration' "${l}")
 	done < <(find_log_targets)
```

### Comparing `portage-3.0.47/bin/install-qa-check.d/90cython-dep` & `portage-3.0.48/bin/install-qa-check.d/90cython-dep`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/90gcc-warnings` & `portage-3.0.48/bin/install-qa-check.d/90gcc-warnings`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/90world-writable` & `portage-3.0.48/bin/install-qa-check.d/90world-writable`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install-qa-check.d/95empty-dirs` & `portage-3.0.48/bin/install-qa-check.d/95empty-dirs`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/install.py` & `portage-3.0.48/bin/install.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/isolated-functions.sh` & `portage-3.0.48/bin/isolated-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/lock-helper.py` & `portage-3.0.48/bin/lock-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/misc-functions.sh` & `portage-3.0.48/bin/misc-functions.sh`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 	if has binpkg-dostrip ${FEATURES}; then
 		export STRIP_MASK
 		if ___eapi_has_dostrip; then
 			"${PORTAGE_BIN_PATH}"/estrip --queue "${PORTAGE_DOSTRIP[@]}"
 			"${PORTAGE_BIN_PATH}"/estrip --ignore "${PORTAGE_DOSTRIP_SKIP[@]}"
 			"${PORTAGE_BIN_PATH}"/estrip --dequeue
 		else
-			prepallstrip
+			"${PORTAGE_BIN_PATH}"/estrip --prepallstrip
 		fi
 	fi
 }
 
 __dyn_instprep() {
 	if [[ -e ${PORTAGE_BUILDDIR}/.instprepped ]] ; then
 		__vecho ">>> It appears that '${PF}' is already instprepped; skipping."
@@ -298,15 +298,15 @@
 	if ! has binpkg-dostrip ${FEATURES}; then
 		export STRIP_MASK
 		if ___eapi_has_dostrip; then
 			"${PORTAGE_BIN_PATH}"/estrip --queue "${PORTAGE_DOSTRIP[@]}"
 			"${PORTAGE_BIN_PATH}"/estrip --ignore "${PORTAGE_DOSTRIP_SKIP[@]}"
 			"${PORTAGE_BIN_PATH}"/estrip --dequeue
 		else
-			prepallstrip
+			"${PORTAGE_BIN_PATH}"/estrip --prepallstrip
 		fi
 	fi
 
 	if has chflags ${FEATURES}; then
 		# Restore all the file flags that were saved earlier on.
 		mtree -U -e -p "${ED}" -k flags < "${T}/bsdflags.mtree" &> /dev/null
 	fi
```

### Comparing `portage-3.0.47/bin/phase-functions.sh` & `portage-3.0.48/bin/phase-functions.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/phase-helpers.sh` & `portage-3.0.48/bin/phase-helpers.sh`

 * *Files 4% similar despite different names*

```diff
@@ -677,32 +677,32 @@
 				if [[ ${conf_help} == *--with-sysroot[^A-Za-z0-9+_.-]* ]]; then
 					conf_args+=( --with-sysroot="${ESYSROOT:-/}" )
 				fi
 			fi
 		fi
 
 		# If the profile defines a location to install libs to aside from default, pass it on.
-		# If the ebuild passes in --libdir, they're responsible for the conf_libdir fun.
-		local CONF_LIBDIR LIBDIR_VAR="LIBDIR_${ABI}"
-		if [[ -n ${ABI} && -n ${!LIBDIR_VAR} ]] ; then
-			CONF_LIBDIR=${!LIBDIR_VAR}
+		# If the ebuild passes in --libdir, they're responsible for the libdir fun.
+		local libdir libdir_var="LIBDIR_${ABI}"
+		if [[ -n ${ABI} && -n ${!libdir_var} ]] ; then
+			libdir=${!libdir_var}
 		fi
 
-		if [[ -n ${CONF_LIBDIR} ]] && ! __hasgq --libdir=\* "$@" ; then
+		if [[ -n ${libdir} ]] && ! __hasgq --libdir=\* "$@" ; then
 			export CONF_PREFIX=$(__hasg --exec-prefix=\* "$@")
 			[[ -z ${CONF_PREFIX} ]] && CONF_PREFIX=$(__hasg --prefix=\* "$@")
 
 			: ${CONF_PREFIX:=${EPREFIX}/usr}
 			CONF_PREFIX=${CONF_PREFIX#*=}
 
 			[[ ${CONF_PREFIX} != /* ]] && CONF_PREFIX="/${CONF_PREFIX}"
-			[[ ${CONF_LIBDIR} != /* ]] && CONF_LIBDIR="/${CONF_LIBDIR}"
+			[[ ${libdir} != /* ]] && libdir="/${libdir}"
 
 			conf_args+=(
-				--libdir="$(__strip_duplicate_slashes "${CONF_PREFIX}${CONF_LIBDIR}")"
+				--libdir="$(__strip_duplicate_slashes "${CONF_PREFIX}${libdir}")"
 			)
 		fi
 
 		# Handle arguments containing quoted whitespace (see bug #457136).
 		eval "local -a EXTRA_ECONF=(${EXTRA_ECONF})"
 
 		set -- \
@@ -747,25 +747,23 @@
 
 	# CONF_PREFIX is only set if they didn't pass in libdir above.
 	local LOCAL_EXTRA_EINSTALL="${EXTRA_EINSTALL}"
 	if ! ___eapi_has_prefix_variables; then
 		local ED=${D}
 	fi
 
-	LIBDIR_VAR="LIBDIR_${ABI}"
-	if [[ -n "${ABI}" && -n "${!LIBDIR_VAR}" ]]; then
-		CONF_LIBDIR="${!LIBDIR_VAR}"
-	fi
-	unset LIBDIR_VAR
-
-	if [[ -n "${CONF_LIBDIR}" && "${CONF_PREFIX:+set}" = set ]]; then
-		EI_DESTLIBDIR="${D%/}/${CONF_PREFIX}/${CONF_LIBDIR}"
-		EI_DESTLIBDIR="$(__strip_duplicate_slashes "${EI_DESTLIBDIR}")"
-		LOCAL_EXTRA_EINSTALL="libdir=${EI_DESTLIBDIR} ${LOCAL_EXTRA_EINSTALL}"
-		unset EI_DESTLIBDIR
+	local libdir libdir_var="LIBDIR_${ABI}"
+	if [[ -n "${ABI}" && -n "${!libdir_var}" ]]; then
+		libdir="${!libdir_var}"
+	fi
+
+	if [[ -n "${libdir}" && "${CONF_PREFIX:+set}" = set ]]; then
+		local destlibdir="${D%/}/${CONF_PREFIX}/${libdir}"
+		destlibdir="$(__strip_duplicate_slashes "${destlibdir}")"
+		LOCAL_EXTRA_EINSTALL="libdir=${destlibdir} ${LOCAL_EXTRA_EINSTALL}"
 	fi
 
 	if [[ -f Makefile || -f GNUmakefile || -f makefile ]] ; then
 		if [[ "${PORTAGE_DEBUG}" == "1" ]]; then
 			${MAKE:-make} -n prefix="${ED%/}/usr" \
 				datadir="${ED%/}/usr/share" \
 				infodir="${ED%/}/usr/share/info" \
@@ -961,15 +959,15 @@
 				esac
 			fi ;;
 	esac
 
 	if [[ -n ${PORTAGE_IPC_DAEMON} ]] ; then
 		cmd+=("${PORTAGE_BIN_PATH}"/ebuild-ipc "${FUNCNAME[1]}" "${root}" "${atom}")
 	else
-		cmd+=("${PORTAGE_BIN_PATH}"/ebuild-helpers/portageq "${FUNCNAME[1]}" "${root}" "${atom}")
+		cmd+=("${PORTAGE_BIN_PATH}"/portageq-wrapper "${FUNCNAME[1]}" "${root}" "${atom}")
 	fi
 
 	"${cmd[@]}"
 	local retval=$?
 
 	case "${retval}" in
 		0|1)
```

### Comparing `portage-3.0.47/bin/pid-ns-init` & `portage-3.0.48/bin/pid-ns-init`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/portageq` & `portage-3.0.48/bin/portageq`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/postinst-qa-check.d/50xdg-utils` & `portage-3.0.48/bin/postinst-qa-check.d/50xdg-utils`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/quickpkg` & `portage-3.0.48/bin/quickpkg`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/regenworld` & `portage-3.0.48/bin/regenworld`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/save-ebuild-env.sh` & `portage-3.0.48/bin/save-ebuild-env.sh`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/shelve-utils` & `portage-3.0.48/bin/shelve-utils`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/socks5-server.py` & `portage-3.0.48/bin/socks5-server.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/xattr-helper.py` & `portage-3.0.48/bin/xattr-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/bin/xpak-helper.py` & `portage-3.0.48/bin/xpak-helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.alpha.diff` & `portage-3.0.48/cnf/make.conf.example.alpha.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.amd64-fbsd.diff` & `portage-3.0.48/cnf/make.conf.example.amd64-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.amd64.diff` & `portage-3.0.48/cnf/make.conf.example.amd64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.arm.diff` & `portage-3.0.48/cnf/make.conf.example.arm.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.arm64.diff` & `portage-3.0.48/cnf/make.conf.example.arm64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.hppa.diff` & `portage-3.0.48/cnf/make.conf.example.hppa.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.ia64.diff` & `portage-3.0.48/cnf/make.conf.example.ia64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.loong.diff` & `portage-3.0.48/cnf/make.conf.example.loong.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.m68k.diff` & `portage-3.0.48/cnf/make.conf.example.m68k.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.mips.diff` & `portage-3.0.48/cnf/make.conf.example.mips.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.ppc.diff` & `portage-3.0.48/cnf/make.conf.example.ppc.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.ppc64.diff` & `portage-3.0.48/cnf/make.conf.example.ppc64.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.riscv.diff` & `portage-3.0.48/cnf/make.conf.example.riscv.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.s390.diff` & `portage-3.0.48/cnf/make.conf.example.s390.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.sh.diff` & `portage-3.0.48/cnf/make.conf.example.sh.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.sparc-fbsd.diff` & `portage-3.0.48/cnf/make.conf.example.sparc-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.sparc.diff` & `portage-3.0.48/cnf/make.conf.example.sparc.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.x86-fbsd.diff` & `portage-3.0.48/cnf/make.conf.example.x86-fbsd.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/cnf/make.conf.example.x86.diff` & `portage-3.0.48/cnf/make.conf.example.x86.diff`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/api/Makefile` & `portage-3.0.48/doc/api/Makefile`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/api/conf.py` & `portage-3.0.48/doc/api/conf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/config/bashrc.docbook` & `portage-3.0.48/doc/config/bashrc.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/config/sets.docbook` & `portage-3.0.48/doc/config/sets.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/dependency_resolution/decision_making.docbook` & `portage-3.0.48/doc/dependency_resolution/decision_making.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/dependency_resolution/package_modeling.docbook` & `portage-3.0.48/doc/dependency_resolution/package_modeling.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/dependency_resolution/task_scheduling.docbook` & `portage-3.0.48/doc/dependency_resolution/task_scheduling.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/eapi/1.docbook` & `portage-3.0.48/doc/package/ebuild/eapi/1.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/eapi/2.docbook` & `portage-3.0.48/doc/package/ebuild/eapi/2.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/eapi/3.docbook` & `portage-3.0.48/doc/package/ebuild/eapi/3.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/eapi/4-slot-abi.docbook` & `portage-3.0.48/doc/package/ebuild/eapi/4-slot-abi.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/eapi/4.docbook` & `portage-3.0.48/doc/package/ebuild/eapi/4.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/eapi/5.docbook` & `portage-3.0.48/doc/package/ebuild/eapi/5.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/helper_functions.docbook` & `portage-3.0.48/doc/package/ebuild/helper_functions.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/package/ebuild/phases.docbook` & `portage-3.0.48/doc/package/ebuild/phases.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/portage.docbook` & `portage-3.0.48/doc/portage.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/doc/qa.docbook` & `portage-3.0.48/doc/qa.docbook`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/AbstractDepPriority.py` & `portage-3.0.48/lib/_emerge/AbstractDepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/AbstractEbuildProcess.py` & `portage-3.0.48/lib/_emerge/AbstractEbuildProcess.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import tempfile
 import textwrap
 from _emerge.SpawnProcess import SpawnProcess
 from _emerge.EbuildBuildDir import EbuildBuildDir
 from _emerge.EbuildIpcDaemon import EbuildIpcDaemon
 import portage
 from portage.elog import messages as elog_messages
-from portage.localization import _
 from portage.package.ebuild._ipc.ExitCommand import ExitCommand
 from portage.package.ebuild._ipc.QueryCommand import QueryCommand
 from portage import os
 from portage.util.futures import asyncio
 from portage.util import apply_secpass_permissions, no_color
 
 portage.proxy.lazyimport.lazyimport(
@@ -68,18 +67,18 @@
     def _start(self):
         need_builddir = self.phase not in self._phases_without_builddir
 
         # This can happen if the pre-clean phase triggers
         # die_hooks for some reason, and PORTAGE_BUILDDIR
         # doesn't exist yet.
         if need_builddir and not os.path.isdir(self.settings["PORTAGE_BUILDDIR"]):
-            msg = _(
-                "The ebuild phase '%s' has been aborted "
-                "since PORTAGE_BUILDDIR does not exist: '%s'"
-            ) % (self.phase, self.settings["PORTAGE_BUILDDIR"])
+            msg = (
+                f"The ebuild phase '{self.phase}' has been aborted since "
+                f"PORTAGE_BUILDDIR does not exist: '{self.settings['PORTAGE_BUILDDIR']}'"
+            )
             self._eerror(textwrap.wrap(msg, 72))
             self.returncode = 1
             self._async_wait()
             return
 
         # Check if the cgroup hierarchy is in place. If it's not, mount it.
         if (
@@ -322,19 +321,18 @@
     def _cancel_timeout_cb(self):
         self._exit_timeout_id = None
         self._async_waitpid()
 
     def _orphan_process_warn(self):
         phase = self.phase
 
-        msg = _(
-            "The ebuild phase '%s' with pid %s appears "
-            "to have left an orphan process running in the "
-            "background."
-        ) % (phase, self.pid)
+        msg = (
+            f"The ebuild phase '{phase}' with pid {self.pid} appears "
+            "to have left an orphan process running in the background."
+        )
 
         self._eerror(textwrap.wrap(msg, 72))
 
     def _can_log(self, slave_fd):
         # With sesandbox, logging works through a pty but not through a
         # normal pipe. So, disable logging if ptys are broken.
         # See Bug #162404.
@@ -342,46 +340,40 @@
         # sesandbox, since EbuildIpcDaemon uses a fifo and it's known
         # to be compatible with sesandbox.
         return not (
             "sesandbox" in self.settings.features and self.settings.selinux_enabled()
         ) or os.isatty(slave_fd)
 
     def _killed_by_signal(self, signum):
-        msg = _("The ebuild phase '%s' has been " "killed by signal %s.") % (
-            self.phase,
-            signum,
-        )
+        msg = f"The ebuild phase '{self.phase}' has been killed by signal {signum}."
         self._eerror(textwrap.wrap(msg, 72))
 
     def _unexpected_exit(self):
         phase = self.phase
 
         msg = (
-            _(
-                "The ebuild phase '%s' has exited "
-                "unexpectedly. This type of behavior "
-                "is known to be triggered "
-                "by things such as failed variable "
-                "assignments (bug #190128) or bad substitution "
-                "errors (bug #200313). Normally, before exiting, bash should "
-                "have displayed an error message above. If bash did not "
-                "produce an error message above, it's possible "
-                "that the ebuild has called `exit` when it "
-                "should have called `die` instead. This behavior may also "
-                "be triggered by a corrupt bash binary or a hardware "
-                "problem such as memory or cpu malfunction. If the problem is not "
-                "reproducible or it appears to occur randomly, then it is likely "
-                "to be triggered by a hardware problem. "
-                "If you suspect a hardware problem then you should "
-                "try some basic hardware diagnostics such as memtest. "
-                "Please do not report this as a bug unless it is consistently "
-                "reproducible and you are sure that your bash binary and hardware "
-                "are functioning properly."
-            )
-            % phase
+            f"The ebuild phase '{phase}' has exited "
+            "unexpectedly. This type of behavior "
+            "is known to be triggered "
+            "by things such as failed variable "
+            "assignments (bug #190128) or bad substitution "
+            "errors (bug #200313). Normally, before exiting, bash should "
+            "have displayed an error message above. If bash did not "
+            "produce an error message above, it's possible "
+            "that the ebuild has called `exit` when it "
+            "should have called `die` instead. This behavior may also "
+            "be triggered by a corrupt bash binary or a hardware "
+            "problem such as memory or cpu malfunction. If the problem is not "
+            "reproducible or it appears to occur randomly, then it is likely "
+            "to be triggered by a hardware problem. "
+            "If you suspect a hardware problem then you should "
+            "try some basic hardware diagnostics such as memtest. "
+            "Please do not report this as a bug unless it is consistently "
+            "reproducible and you are sure that your bash binary and hardware "
+            "are functioning properly."
         )
 
         self._eerror(textwrap.wrap(msg, 72))
 
     def _eerror(self, lines):
         self._elog("eerror", lines)
```

### Comparing `portage-3.0.47/lib/_emerge/AbstractPollTask.py` & `portage-3.0.48/lib/_emerge/AbstractPollTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/AsynchronousLock.py` & `portage-3.0.48/lib/_emerge/AsynchronousLock.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     import threading
 except ImportError:
     threading = dummy_threading
 
 import portage
 from portage import os
 from portage.exception import TryAgain
-from portage.localization import _
 from portage.locks import lockfile, unlockfile
 from portage.util import writemsg_level
 from _emerge.AbstractPollTask import AbstractPollTask
 from _emerge.AsynchronousTask import AsynchronousTask
 from _emerge.SpawnProcess import SpawnProcess
 
 
@@ -240,17 +239,15 @@
 
             if not self._acquired:
                 # If the lock hasn't been aquired yet, the
                 # caller can check the returncode and handle
                 # this failure appropriately.
                 if not (self.cancelled or self._kill_test):
                     writemsg_level(
-                        "_LockProcess: %s\n"
-                        % _("failed to acquire lock on '%s'")
-                        % (self.path,),
+                        "_LockProcess: failed to acquire lock on '{self.path}'\n",
                         level=logging.ERROR,
                         noiselevel=-1,
                     )
                 self._unregister()
                 self.returncode = proc.returncode
                 self._async_wait()
                 return
```

### Comparing `portage-3.0.47/lib/_emerge/AsynchronousTask.py` & `portage-3.0.48/lib/_emerge/AsynchronousTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/Binpkg.py` & `portage-3.0.48/lib/_emerge/Binpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/BinpkgEnvExtractor.py` & `portage-3.0.48/lib/_emerge/BinpkgEnvExtractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,18 +27,15 @@
 
     def _get_dest_env_path(self):
         return os.path.join(self.settings["T"], "environment")
 
     def _start(self):
         saved_env_path = self._get_saved_env_path()
         dest_env_path = self._get_dest_env_path()
-        shell_cmd = (
-            "${PORTAGE_BUNZIP2_COMMAND:-${PORTAGE_BZIP2_COMMAND} -d} -c -- %s > %s"
-            % (_shell_quote(saved_env_path), _shell_quote(dest_env_path))
-        )
+        shell_cmd = f"${{PORTAGE_BUNZIP2_COMMAND:-${{PORTAGE_BZIP2_COMMAND}} -d}} -c -- {_shell_quote(saved_env_path)} > {_shell_quote(dest_env_path)}"
 
         logfile = None
         if self.settings.get("PORTAGE_BACKGROUND") != "subprocess":
             logfile = self.settings.get("PORTAGE_LOG_FILE")
 
         extractor_proc = SpawnProcess(
             args=[BASH_BINARY, "-c", shell_cmd],
```

### Comparing `portage-3.0.47/lib/_emerge/BinpkgExtractorAsync.py` & `portage-3.0.48/lib/_emerge/BinpkgExtractorAsync.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 1999-2013 Gentoo Foundation
 # Distributed under the terms of the GNU General Public License v2
 
 import logging
 
 from _emerge.SpawnProcess import SpawnProcess
 import portage
-from portage.localization import _
 from portage.util.compression_probe import (
     compression_probe,
     _compressors,
 )
 from portage.util.cpuinfo import makeopts_to_job_count
 from portage.process import find_binary
 from portage.util import (
@@ -17,14 +16,15 @@
     varexpand,
 )
 from portage.exception import InvalidBinaryPackageFormat
 from portage.binpkg import get_binpkg_format
 import signal
 import subprocess
 import tarfile
+import textwrap
 
 
 class BinpkgExtractorAsync(SpawnProcess):
     __slots__ = ("features", "image_dir", "pkg", "pkg_path")
 
     _shell_binary = portage.const.BASH_BINARY
 
@@ -68,17 +68,15 @@
                 "compress": "cat",
                 "package": "sys-apps/coreutils",
             }
         else:
             decomp_cmd = None
         if decomp_cmd is None:
             self.scheduler.output(
-                "!!! %s\n"
-                % _("File compression header unrecognized: %s")
-                % self.pkg_path,
+                f"!!! File compression header unrecognized: {self.pkg_path}\n",
                 log_path=self.logfile,
                 background=self.background,
                 level=logging.ERROR,
             )
             self.returncode = 1
             self._async_wait()
             return
@@ -100,23 +98,17 @@
                 )[0]
             except IndexError:
                 decompression_binary = ""
 
             if find_binary(decompression_binary) is None:
                 missing_package = decomp.get("package")
                 self.scheduler.output(
-                    "!!! %s\n"
-                    % _(
-                        "File compression unsupported %s.\n Command was: %s.\n Maybe missing package: %s"
-                    )
-                    % (
-                        self.pkg_path,
-                        varexpand(decomp_cmd, mydict=self.env),
-                        missing_package,
-                    ),
+                    f"!!! File compression unsupported {self.pkg_path}.\n"
+                    f" Command was: {varexpand(decomp_cmd, mydict=self.env)}.\n"
+                    f" Missing package: {missing_package}\n",
                     log_path=self.logfile,
                     background=self.background,
                     level=logging.ERROR,
                 )
                 self.returncode = 1
                 self._async_wait()
                 return
@@ -125,30 +117,34 @@
         pkg_xpak.scan()
 
         # SIGPIPE handling (128 + SIGPIPE) should be compatible with
         # assert_sigpipe_ok() that's used by the ebuild unpack() helper.
         self.args = [
             self._shell_binary,
             "-c",
-            (
-                "cmd0=(head -c %d -- %s) cmd1=(%s) cmd2=(tar -xp %s -C %s -f -); "
-                + '"${cmd0[@]}" | "${cmd1[@]}" | "${cmd2[@]}"; '
-                + "p=(${PIPESTATUS[@]}) ; for i in {0..2}; do "
-                + "if [[ ${p[$i]} != 0 && ${p[$i]} != %d ]] ; then "
-                + 'echo command $(eval "echo \\"\'\\${cmd$i[*]}\'\\"") '
-                + "failed with status ${p[$i]} ; exit ${p[$i]} ; fi ; done; "
-                + "if [ ${p[$i]} != 0 ] ; then "
-                + 'echo command $(eval "echo \\"\'\\${cmd$i[*]}\'\\"") '
-                + "failed with status ${p[$i]} ; exit ${p[$i]} ; fi ; "
-                + "exit 0 ;"
-            )
-            % (
-                pkg_xpak.filestat.st_size - pkg_xpak.xpaksize,
-                portage._shell_quote(self.pkg_path),
-                decomp_cmd,
-                tar_options,
-                portage._shell_quote(self.image_dir),
-                128 + signal.SIGPIPE,
-            ),
+            textwrap.dedent(
+                f"""
+                    cmd0=(head -c {pkg_xpak.filestat.st_size - pkg_xpak.xpaksize} -- {portage._shell_quote(self.pkg_path)})
+                    cmd1=({decomp_cmd})
+                    cmd2=(tar -xp {tar_options} -C {portage._shell_quote(self.image_dir)} -f -);
+                """
+                """
+                    "${cmd0[@]}" | "${cmd1[@]}" | "${cmd2[@]}";
+                    p=(${PIPESTATUS[@]}) ; for i in {0..2}; do
+                """
+                f"""
+                    if [[ ${{p[$i]}} != 0 && ${{p[$i]}} != {128 + signal.SIGPIPE} ]] ; then
+                """
+                """
+                    echo command $(eval "echo \\"'\\${cmd$i[*]}'\\"") failed with status ${p[$i]} ;
+                    exit ${p[$i]} ; fi ; done;
+                    if [ ${p[$i]} != 0 ] ; then
+                    echo command $(eval "echo \\"'\\${cmd$i[*]}'\\"") failed with status ${p[$i]} ;
+                    exit ${p[$i]} ; fi ;
+                    exit 0 ;
+                """
+            )
+            .replace("\n", " ")
+            .strip(),
         ]
 
         SpawnProcess._start(self)
```

### Comparing `portage-3.0.47/lib/_emerge/BinpkgFetcher.py` & `portage-3.0.48/lib/_emerge/BinpkgFetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,16 +240,15 @@
         def acquired_lock(async_lock):
             if async_lock.wait() == os.EX_OK:
                 self.locked = True
                 result.set_result(None)
             else:
                 result.set_exception(
                     AssertionError(
-                        "AsynchronousLock failed with returncode %s"
-                        % (async_lock.returncode,)
+                        f"AsynchronousLock failed with returncode {async_lock.returncode}"
                     )
                 )
 
         self._lock_obj = AsynchronousLock(path=self.pkg_path, scheduler=self.scheduler)
         self._lock_obj.addExitListener(acquired_lock)
         self._lock_obj.start()
         return result
```

### Comparing `portage-3.0.47/lib/_emerge/BinpkgPrefetcher.py` & `portage-3.0.48/lib/_emerge/BinpkgPrefetcher.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/BinpkgVerifier.py` & `portage-3.0.48/lib/_emerge/BinpkgVerifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         try:
             size = os.stat(self._pkg_path).st_size
         except OSError as e:
             if e.errno not in (errno.ENOENT, errno.ESTALE):
                 raise
             self.scheduler.output(
-                ("!!! Fetching Binary failed " "for '%s'\n") % self.pkg.cpv,
+                f"!!! Fetching Binary failed for '{self.pkg.cpv}'\n",
                 log_path=self.logfile,
                 background=self.background,
             )
             self.returncode = 1
             self._async_wait()
             return
         else:
@@ -119,19 +119,16 @@
     def _digest_exception(self, name, value, expected):
         head, tail = os.path.split(self._pkg_path)
         temp_filename = _checksum_failure_temp_file(
             self.pkg.root_config.settings, head, tail
         )
 
         self.scheduler.output(
-            (
-                "\n!!! Digest verification failed:\n"
-                "!!! %s\n"
-                "!!! Reason: Failed on %s verification\n"
-                "!!! Got: %s\n"
-                "!!! Expected: %s\n"
-                "File renamed to '%s'\n"
-            )
-            % (self._pkg_path, name, value, expected, temp_filename),
+            "\n!!! Digest verification failed:\n"
+            f"!!! {self._pkg_path}\n"
+            f"!!! Reason: Failed on {name} verification\n"
+            f"!!! Got: {value}\n"
+            f"!!! Expected: {expected}\n"
+            f"File renamed to '{temp_filename}'\n",
             log_path=self.logfile,
             background=self.background,
         )
```

### Comparing `portage-3.0.47/lib/_emerge/BlockerCache.py` & `portage-3.0.48/lib/_emerge/BlockerCache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/BlockerDB.py` & `portage-3.0.48/lib/_emerge/BlockerDB.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/CompositeTask.py` & `portage-3.0.48/lib/_emerge/CompositeTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/DepPriority.py` & `portage-3.0.48/lib/_emerge/DepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/DepPriorityNormalRange.py` & `portage-3.0.48/lib/_emerge/DepPriorityNormalRange.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/DepPrioritySatisfiedRange.py` & `portage-3.0.48/lib/_emerge/DepPrioritySatisfiedRange.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/Dependency.py` & `portage-3.0.48/lib/_emerge/Dependency.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/DependencyArg.py` & `portage-3.0.48/lib/_emerge/DependencyArg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildBinpkg.py` & `portage-3.0.48/lib/_emerge/EbuildBinpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildBuild.py` & `portage-3.0.48/lib/_emerge/EbuildBuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildBuildDir.py` & `portage-3.0.48/lib/_emerge/EbuildBuildDir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildExecuter.py` & `portage-3.0.48/lib/_emerge/EbuildExecuter.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildFetcher.py` & `portage-3.0.48/lib/_emerge/EbuildFetcher.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildFetchonly.py` & `portage-3.0.48/lib/_emerge/EbuildFetchonly.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildIpcDaemon.py` & `portage-3.0.48/lib/_emerge/EbuildIpcDaemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildMerge.py` & `portage-3.0.48/lib/_emerge/EbuildMerge.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,21 +71,21 @@
         if "noclean" not in self.settings.features:
             short_msg = "emerge: ({} of {}) {} Clean Post".format(
                 pkg_count.curval,
                 pkg_count.maxval,
                 pkg.cpv,
             )
             logger.log(
-                (" === (%s of %s) " + "Post-Build Cleaning (%s::%s)")
-                % (pkg_count.curval, pkg_count.maxval, pkg.cpv, pkg_path),
+                f" === ({pkg_count.curval} of {pkg_count.maxval}) "
+                f"Post-Build Cleaning ({pkg.cpv}::{pkg_path})",
                 short_msg=short_msg,
             )
         logger.log(
-            " ::: completed emerge (%s of %s) %s to %s"
-            % (pkg_count.curval, pkg_count.maxval, pkg.cpv, pkg.root)
+            f" ::: completed emerge ({pkg_count.curval} of {pkg_count.maxval}) "
+            f"{pkg.cpv} to {pkg.root}"
         )
 
         self._start_exit_hook(self.returncode)
 
     def _start_exit_hook(self, returncode):
         """
         Start the exit hook, and set returncode after it completes.
```

### Comparing `portage-3.0.47/lib/_emerge/EbuildMetadataPhase.py` & `portage-3.0.48/lib/_emerge/EbuildMetadataPhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildPhase.py` & `portage-3.0.48/lib/_emerge/EbuildPhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildProcess.py` & `portage-3.0.48/lib/_emerge/EbuildProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/EbuildSpawnProcess.py` & `portage-3.0.48/lib/_emerge/EbuildSpawnProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/FakeVartree.py` & `portage-3.0.48/lib/_emerge/FakeVartree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/FifoIpcDaemon.py` & `portage-3.0.48/lib/_emerge/FifoIpcDaemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/JobStatusDisplay.py` & `portage-3.0.48/lib/_emerge/JobStatusDisplay.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,21 +187,19 @@
             avg = getloadavg()
         except OSError:
             return "unknown"
 
         max_avg = max(avg)
 
         if max_avg < 10:
-            digits = 2
+            return ", ".join(f"{x:.2f}" for x in avg)
         elif max_avg < 100:
-            digits = 1
+            return ", ".join(f"{x:.1f}" for x in avg)
         else:
-            digits = 0
-
-        return ", ".join(("%%.%df" % digits) % x for x in avg)
+            return ", ".join(f"{x:.0f}" for x in avg)
 
     def display(self):
         """
         Display status on stdout, but only if something has
         changed since the last call. This always returns True,
         for continuous scheduling via timeout_add.
         """
```

### Comparing `portage-3.0.47/lib/_emerge/MergeListItem.py` & `portage-3.0.48/lib/_emerge/MergeListItem.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,16 +76,16 @@
 
         if pkg.root_config.settings["ROOT"] != "/":
             msg += f" {preposition} {pkg.root}"
 
         if not build_opts.pretend:
             self.statusMessage(msg)
             logger.log(
-                " >>> emerge (%s of %s) %s to %s"
-                % (pkg_count.curval, pkg_count.maxval, pkg.cpv, pkg.root)
+                f" >>> emerge ({pkg_count.curval} of {pkg_count.maxval}) "
+                f"{pkg.cpv} to {pkg.root}"
             )
 
         if pkg.type_name == "ebuild":
             build = EbuildBuild(
                 args_set=args_set,
                 background=self.background,
                 config_pool=self.config_pool,
```

### Comparing `portage-3.0.47/lib/_emerge/MetadataRegen.py` & `portage-3.0.48/lib/_emerge/MetadataRegen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/MiscFunctionsProcess.py` & `portage-3.0.48/lib/_emerge/MiscFunctionsProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/Package.py` & `portage-3.0.48/lib/_emerge/Package.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     _slot_separator,
     _repo_separator,
 )
 from portage.dep.soname.parse import parse_soname_deps
 from portage.versions import _pkg_str, _unknown_repo
 from portage.eapi import _get_eapi_attrs
 from portage.exception import InvalidData, InvalidDependString
-from portage.localization import _
 from _emerge.Task import Task
 
 
 class Package(Task):
     __hash__ = Task.__hash__
     __slots__ = (
         "built",
@@ -340,19 +339,16 @@
                 validated_atoms.extend(atoms)
                 if not self.built:
                     for atom in atoms:
                         if not isinstance(atom, Atom):
                             continue
                         if atom.slot_operator_built:
                             e = InvalidDependString(
-                                _(
-                                    "Improper context for slot-operator "
-                                    '"built" atom syntax: %s'
-                                )
-                                % (atom.unevaluated_atom,)
+                                'Improper context for slot-operator "built" '
+                                f"atom syntax: {atom.unevaluated_atom}"
                             )
                             self._metadata_exception(k, e)
 
         self._validated_atoms = tuple(
             {atom for atom in validated_atoms if isinstance(atom, Atom)}
         )
```

### Comparing `portage-3.0.47/lib/_emerge/PackageArg.py` & `portage-3.0.48/lib/_emerge/PackageArg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/PackageMerge.py` & `portage-3.0.48/lib/_emerge/PackageMerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/PackagePhase.py` & `portage-3.0.48/lib/_emerge/PackagePhase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/PackageUninstall.py` & `portage-3.0.48/lib/_emerge/PackageUninstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/PackageVirtualDbapi.py` & `portage-3.0.48/lib/_emerge/PackageVirtualDbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/PipeReader.py` & `portage-3.0.48/lib/_emerge/PipeReader.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/PollScheduler.py` & `portage-3.0.48/lib/_emerge/PollScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/ProgressHandler.py` & `portage-3.0.48/lib/_emerge/ProgressHandler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/RootConfig.py` & `portage-3.0.48/lib/_emerge/RootConfig.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/Scheduler.py` & `portage-3.0.48/lib/_emerge/Scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -2214,19 +2214,19 @@
                 if hasattr(world_set, "remove"):
                     for s in pkg.root_config.setconfig.active:
                         world_set.remove(SETPREFIX + s)
             else:
                 if atom is not None:
                     if hasattr(world_set, "add"):
                         self._status_msg(
-                            ('Recording %s in "world" ' + "favorites file...") % atom
+                            f'Recording {atom} in "world" favorites file...'
                         )
                         logger.log(
-                            " === (%s of %s) Updating world file (%s)"
-                            % (pkg_count.curval, pkg_count.maxval, pkg.cpv)
+                            f" === ({pkg_count.curval} of {pkg_count.maxval}) "
+                            f"Updating world file ({pkg.cpv})"
                         )
                         world_set.add(atom)
                     else:
                         writemsg_level(
                             f'\n!!! Unable to record {atom} in "world"\n',
                             level=logging.WARN,
                             noiselevel=-1,
```

### Comparing `portage-3.0.47/lib/_emerge/SequentialTaskQueue.py` & `portage-3.0.48/lib/_emerge/SequentialTaskQueue.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/SpawnProcess.py` & `portage-3.0.48/lib/_emerge/SpawnProcess.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import signal
 import sys
 
 from _emerge.SubProcess import SubProcess
 import portage
 from portage import os
 from portage.const import BASH_BINARY
-from portage.localization import _
 from portage.output import EOutput
 from portage.util import writemsg_level
 from portage.util._async.BuildLogger import BuildLogger
 from portage.util._async.PipeLogger import PipeLogger
 from portage.util._pty import _create_pty_or_pipe
 from portage.util.futures import asyncio
 
@@ -267,15 +266,15 @@
                 for p in pids:
                     try:
                         os.kill(p, sig)
                     except OSError as e:
                         if e.errno == errno.EPERM:
                             # Reported with hardened kernel (bug #358211).
                             writemsg_level(
-                                "!!! kill: (%i) - Operation not permitted\n" % (p,),
+                                f"!!! kill: ({p}) - Operation not permitted\n",
                                 level=logging.ERROR,
                                 noiselevel=-1,
                             )
                         elif e.errno != errno.ESRCH:
                             raise
 
             # step 1: kill all orphans (loop in case of new forks)
@@ -287,19 +286,17 @@
                     kill_all(pids, signal.SIGKILL)
                 else:
                     break
 
             if pids:
                 msg = []
                 msg.append(
-                    _("Failed to kill pid(s) in '%(cgroup)s': %(pids)s")
-                    % dict(
-                        cgroup=os.path.join(self.cgroup, "cgroup.procs"),
-                        pids=" ".join(str(pid) for pid in pids),
-                    )
+                    "Failed to kill pid(s) in "
+                    f"'{os.path.join(self.cgroup, 'cgroup.procs')}': "
+                    f"{' '.join(str(pid) for pid in pids)}"
                 )
 
                 self._elog("eerror", msg)
 
             # step 2: remove the cgroup
             try:
                 os.rmdir(self.cgroup)
```

### Comparing `portage-3.0.47/lib/_emerge/SubProcess.py` & `portage-3.0.48/lib/_emerge/SubProcess.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         if self.isAlive() and self.pid is not None:
             try:
                 os.kill(self.pid, signal.SIGTERM)
             except OSError as e:
                 if e.errno == errno.EPERM:
                     # Reported with hardened kernel (bug #358211).
                     writemsg_level(
-                        "!!! kill: (%i) - Operation not permitted\n" % (self.pid,),
+                        f"!!! kill: ({self.pid}) - Operation not permitted\n",
                         level=logging.ERROR,
                         noiselevel=-1,
                     )
                 elif e.errno != errno.ESRCH:
                     raise
 
     def _async_wait(self):
```

### Comparing `portage-3.0.47/lib/_emerge/Task.py` & `portage-3.0.48/lib/_emerge/Task.py`

 * *Files 25% similar despite different names*

```diff
@@ -37,17 +37,18 @@
         return key in self._hash_key
 
     def __str__(self):
         """
         Emulate tuple.__repr__, but don't show 'foo' as u'foo' for unicode
         strings.
         """
-        return "(%s)" % ", ".join("'%s'" % x for x in self._hash_key)
+        strings = (f"'{x}'" for x in self._hash_key)
+        return f"({', '.join(strings)})"
 
     def __repr__(self):
         if self._hash_key is None:
             # triggered by python-trace
             return SlotObject.__repr__(self)
         return "<{} ({})>".format(
             self.__class__.__name__,
-            ", ".join("'%s'" % x for x in self._hash_key),
+            ", ".join(f"'{x}'" for x in self._hash_key),
         )
```

### Comparing `portage-3.0.47/lib/_emerge/TaskSequence.py` & `portage-3.0.48/lib/_emerge/TaskSequence.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/UnmergeDepPriority.py` & `portage-3.0.48/lib/_emerge/UnmergeDepPriority.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/UseFlagDisplay.py` & `portage-3.0.48/lib/_emerge/UseFlagDisplay.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/UserQuery.py` & `portage-3.0.48/lib/_emerge/UserQuery.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,18 +50,15 @@
         if "--alert" in self.myopts:
             prompt = "\a" + prompt
         print(bold(prompt), end=" ")
         try:
             while True:
                 try:
                     response = input(
-                        "[%s] "
-                        % "/".join(
-                            [colours[i](responses[i]) for i in range(len(responses))]
-                        )
+                        f"[{'/'.join([colours[i](responses[i]) for i in range(len(responses))])}] "
                     )
                 except UnicodeDecodeError as e:
                     response = _unicode_decode(e.object).rstrip("\n")
                 if response or not enter_invalid:
                     for key in responses:
                         # An empty response will match the
                         # first value in responses.
```

### Comparing `portage-3.0.47/lib/_emerge/_find_deep_system_runtime_deps.py` & `portage-3.0.48/lib/_emerge/_find_deep_system_runtime_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/actions.py` & `portage-3.0.48/lib/_emerge/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,17 +578,15 @@
                     eroots.add(x.root)
                     if x.type_name == "ebuild":
                         ebuild_eroots.add(x.root)
 
             for eroot in eroots:
                 if need_write_vardb and not trees[eroot]["vartree"].dbapi.writable:
                     writemsg_level(
-                        "!!! %s\n"
-                        % _("Read-only file system: %s")
-                        % trees[eroot]["vartree"].dbapi._dbroot,
+                        f"!!! Read-only file system: {trees[eroot]['vartree'].dbapi._dbroot}\n",
                         level=logging.ERROR,
                         noiselevel=-1,
                     )
                     return 1
 
                 if (
                     need_write_bindb
@@ -597,17 +595,15 @@
                         "buildpkg" in trees[eroot]["root_config"].settings.features
                         or "buildsyspkg"
                         in trees[eroot]["root_config"].settings.features
                     )
                     and not trees[eroot]["bintree"].dbapi.writable
                 ):
                     writemsg_level(
-                        "!!! %s\n"
-                        % _("Read-only file system: %s")
-                        % trees[eroot]["bintree"].pkgdir,
+                        f"!!! Read-only file system: {trees[eroot]['bintree'].pkgdir}\n",
                         level=logging.ERROR,
                         noiselevel=-1,
                     )
                     return 1
 
                 # unlock GPG if needed
                 if (
@@ -939,16 +935,15 @@
     for k in ("profile", "system", "selected"):
         try:
             set_atoms[k] = root_config.setconfig.getSetAtoms(k)
         except portage.exception.PackageSetNotFound as e:
             # A nested set could not be resolved, so ignore nested sets.
             set_atoms[k] = root_config.sets[k].getAtoms()
             writemsg_level(
-                _("!!! The set '%s' " "contains a non-existent set named '%s'.\n")
-                % (k, e),
+                f"!!! The set '{k}' contains a non-existent set named '{e}'.\n",
                 level=logging.ERROR,
                 noiselevel=-1,
             )
             set_error = True
 
     # Support @profile as an alternative to @system.
     if not (set_atoms["system"] or set_atoms["profile"]):
@@ -963,16 +958,15 @@
 
     # Suppress world file warnings unless @world is completely empty,
     # since having an empty world file can be a valid state.
     try:
         world_atoms = bool(root_config.setconfig.getSetAtoms("world"))
     except portage.exception.PackageSetNotFound as e:
         writemsg_level(
-            _("!!! The set '%s' " "contains a non-existent set named '%s'.\n")
-            % ("world", e),
+            f"!!! The set 'world' contains a non-existent set named '{e}'.\n",
             level=logging.ERROR,
             noiselevel=-1,
         )
         set_error = True
     else:
         if not world_atoms:
             writemsg_level(
@@ -1048,29 +1042,29 @@
         for pkg in vardb:
             if spinner is not None:
                 spinner.update()
             pkgs_for_cp = vardb.match_pkgs(Atom(pkg.cp))
             if not pkgs_for_cp or pkg not in pkgs_for_cp:
                 raise AssertionError(
                     "package expected in matches: "
-                    + "cp = %s, cpv = %s matches = %s"
-                    % (pkg.cp, pkg.cpv, [str(x) for x in pkgs_for_cp])
+                    f"cp = {pkg.cp}, cpv = {pkg.cpv}, "
+                    f"matches = {[str(x) for x in pkgs_for_cp]}"
                 )
 
             highest_version = pkgs_for_cp[-1]
             if pkg == highest_version:
                 # pkg is the highest version
                 protected_set.add("=" + pkg.cpv)
                 continue
 
             if len(pkgs_for_cp) <= 1:
                 raise AssertionError(
                     "more packages expected: "
-                    + "cp = %s, cpv = %s matches = %s"
-                    % (pkg.cp, pkg.cpv, [str(x) for x in pkgs_for_cp])
+                    f"cp = {pkg.cp}, cpv = {pkg.cpv}, "
+                    f"matches = {[str(x) for x in pkgs_for_cp]}"
                 )
 
             try:
                 if args_set.findAtomForPackage(pkg) is None:
                     protected_set.add("=" + pkg.cpv)
                     continue
             except portage.exception.InvalidDependString as e:
@@ -1252,19 +1246,16 @@
 
         parent_strs = []
         for parent, atoms in parent_atom_dict.items():
             # Display package atoms and soname
             # atoms in separate groups.
             atoms = sorted(atoms, reverse=True, key=operator.attrgetter("package"))
             parent_strs.append(
-                "%s requires %s"
-                % (
-                    getattr(parent, "cpv", parent),
-                    ", ".join(str(atom) for atom in atoms),
-                )
+                f"{getattr(parent, 'cpv', parent)} requires "
+                f"{', '.join(str(atom) for atom in atoms)}"
             )
         parent_strs.sort()
         msg = []
         msg.append(f"  {child_node.cpv} pulled in by:\n")
         for parent_str in parent_strs:
             msg.append(f"    {parent_str}\n")
         msg.append("\n")
@@ -1773,16 +1764,16 @@
 
                 if atom.startswith(SETPREFIX):
                     filename = "world_sets"
                 else:
                     filename = "world"
 
                 writemsg_stdout(
-                    '>>> %s %s from "%s" favorites file...\n'
-                    % (action_desc, colorize("INFORM", str(atom)), filename),
+                    f">>> {action_desc} {colorize('INFORM', str(atom))} "
+                    f'from "{filename}" favorites file...\n',
                     noiselevel=-1,
                 )
 
             if "--ask" in opts:
                 prompt = (
                     "Would you like to remove these "
                     + "packages from your world favorites?"
@@ -1870,16 +1861,15 @@
         if not cp_exists:
             xinfo = f'"{x.unevaluated_atom}"'
             # Discard null/ from failed cpv_expand category expansion.
             xinfo = xinfo.replace("null/", "")
             if settings["ROOT"] != "/":
                 xinfo = f"{xinfo} for {eroot}"
             writemsg(
-                "\nemerge: there are no ebuilds to satisfy %s.\n"
-                % colorize("INFORM", xinfo),
+                f"\nemerge: there are no ebuilds to satisfy {colorize('INFORM', xinfo)}.\n",
                 noiselevel=-1,
             )
 
             if myopts.get("--misspell-suggestions", "y") != "n":
                 writemsg("\nemerge: searching for similar names...", noiselevel=-1)
 
                 search_index = myopts.get("--search-index", "y") != "n"
@@ -1893,16 +1883,15 @@
 
                 if len(matches) == 1:
                     writemsg(
                         "\nemerge: Maybe you meant " + matches[0] + "?\n", noiselevel=-1
                     )
                 elif len(matches) > 1:
                     writemsg(
-                        "\nemerge: Maybe you meant any of these: %s?\n"
-                        % (", ".join(matches),),
+                        f"\nemerge: Maybe you meant any of these: {', '.join(matches)}?\n",
                         noiselevel=-1,
                     )
                 else:
                     # Generally, this would only happen if
                     # all dbapis are empty.
                     writemsg(" nothing similar found.\n", noiselevel=-1)
 
@@ -1929,22 +1918,22 @@
         append(header_width * "=")
         append(header_title.rjust(int(header_width / 2 + len(header_title) / 2)))
     append(header_width * "=")
     append(f"System uname: {platform.platform(aliased=1)}")
 
     vm_info = get_vm_info()
     if "ram.total" in vm_info:
-        line = "%-9s %10d total" % ("KiB Mem:", vm_info["ram.total"] // 1024)
+        line = f"KiB Mem:  {vm_info['ram.total'] // 1024:10d} total"
         if "ram.free" in vm_info:
-            line += ",%10d free" % (vm_info["ram.free"] // 1024,)
+            line += f",{vm_info['ram.free'] // 1024:10d} free"
         append(line)
     if "swap.total" in vm_info:
-        line = "%-9s %10d total" % ("KiB Swap:", vm_info["swap.total"] // 1024)
+        line = f"KiB Swap: {vm_info['swap.total'] // 1024:10d} total"
         if "swap.free" in vm_info:
-            line += ",%10d free" % (vm_info["swap.free"] // 1024,)
+            line += f",{vm_info['swap.free'] // 1024:10d} free"
         append(line)
 
     for repo in repos:
         last_sync = portage.grabfile(
             os.path.join(repo.location, "metadata", "timestamp.chk")
         )
         head_commit = None
@@ -2064,15 +2053,15 @@
     ]
     myvars += portage.util.grabfile(settings["PORTDIR"] + "/profiles/info_pkgs")
     atoms = []
     for x in myvars:
         try:
             x = Atom(x)
         except InvalidAtom:
-            append("%-20s %s" % (x + ":", "[NOT VALID]"))
+            append(f"{x + ':':<20s} [NOT VALID]")
         else:
             for atom in expand_new_virt(vardb, x):
                 if not atom.blocker:
                     atoms.append((x, atom))
 
     myvars = sorted(set(atoms))
 
@@ -2258,26 +2247,26 @@
                 ),
                 root_config=root_config,
                 type_name=pkg_type,
             )
 
             if pkg_type == "installed":
                 append(
-                    "\n%s was built with the following:"
-                    % colorize("INFORM", str(pkg.cpv + _repo_separator + pkg.repo))
+                    f"\n{colorize('INFORM', str(pkg.cpv + _repo_separator + pkg.repo))} "
+                    "was built with the following:"
                 )
             elif pkg_type == "ebuild":
                 append(
-                    "\n%s would be built with the following:"
-                    % colorize("INFORM", str(pkg.cpv + _repo_separator + pkg.repo))
+                    f"\n{colorize('INFORM', str(pkg.cpv + _repo_separator + pkg.repo))} "
+                    "would be built with the following:"
                 )
             elif pkg_type == "binary":
                 append(
-                    "\n%s (non-installed binary) was built with the following:"
-                    % colorize("INFORM", str(pkg.cpv + _repo_separator + pkg.repo))
+                    f"\n{colorize('INFORM', str(pkg.cpv + _repo_separator + pkg.repo))} "
+                    "(non-installed binary) was built with the following:"
                 )
 
             append(f"{pkg_use_display(pkg, myopts)}")
             if pkg_type == "installed":
                 for myvar in mydesiredvars:
                     if metadata[myvar].split() != settings.get(myvar, "").split():
                         append(f'{myvar}="{metadata[myvar]}"')
@@ -2470,33 +2459,29 @@
                         noiselevel=-1,
                     )
                 writemsg_level("\n", level=logging.ERROR, noiselevel=-1)
                 return 1
             else:
                 if atom.use and atom.use.conditional:
                     writemsg_level(
-                        (
-                            "\n\n!!! '%s' contains a conditional "
-                            + "which is not allowed.\n"
-                        )
-                        % (x,),
+                        f"\n\n!!! '{x}' contains a conditional which is not allowed.\n",
                         level=logging.ERROR,
                         noiselevel=-1,
                     )
                     writemsg_level(
                         "!!! Please check ebuild(5) for full details.\n",
                         level=logging.ERROR,
                     )
                     return 1
                 valid_atoms.append(atom)
 
         elif x.startswith(os.sep):
             if not x.startswith(eroot):
                 writemsg_level(
-                    ("!!! '%s' does not start with" + " $EROOT.\n") % x,
+                    f"!!! '{x}' does not start with $EROOT.\n",
                     level=logging.ERROR,
                     noiselevel=-1,
                 )
                 return 1
             # Queue these up since it's most efficient to handle
             # multiple files in a single iter_owners() call.
             lookup_owners.append(x)
@@ -2573,15 +2558,15 @@
         if owners:
             for cpv in owners:
                 pkg = vardb._pkg_str(cpv, None)
                 atom = f"{pkg.cp}:{pkg.slot}"
                 valid_atoms.append(portage.dep.Atom(atom))
         else:
             writemsg_level(
-                ("!!! '%s' is not claimed " + "by any package.\n") % lookup_owners[0],
+                f"!!! '{lookup_owners[0]}' is not claimed by any package.\n",
                 level=logging.WARNING,
                 noiselevel=-1,
             )
 
     if files and not valid_atoms:
         return 1
 
@@ -2704,16 +2689,16 @@
     try:
         EMERGE_WARNING_DELAY = int(
             settings.get("EMERGE_WARNING_DELAY", str(EMERGE_WARNING_DELAY))
         )
     except ValueError as e:
         portage.writemsg(f"!!! {str(e)}\n", noiselevel=-1)
         portage.writemsg(
-            "!!! Unable to parse integer: EMERGE_WARNING_DELAY='%s'\n"
-            % settings["EMERGE_WARNING_DELAY"],
+            "!!! Unable to parse integer: "
+            f"EMERGE_WARNING_DELAY='{settings['EMERGE_WARNING_DELAY']}'\n",
             noiselevel=-1,
         )
     settings["EMERGE_WARNING_DELAY"] = str(EMERGE_WARNING_DELAY)
     settings.backup_changes("EMERGE_WARNING_DELAY")
 
     buildpkg = myopts.get("--buildpkg")
     if buildpkg is True:
@@ -2736,23 +2721,23 @@
 
     # Set various debug markers... They should be merged somehow.
     PORTAGE_DEBUG = 0
     try:
         PORTAGE_DEBUG = int(settings.get("PORTAGE_DEBUG", str(PORTAGE_DEBUG)))
         if PORTAGE_DEBUG not in (0, 1):
             portage.writemsg(
-                "!!! Invalid value: PORTAGE_DEBUG='%i'\n" % PORTAGE_DEBUG, noiselevel=-1
+                f"!!! Invalid value: PORTAGE_DEBUG='{PORTAGE_DEBUG}'\n",
+                noiselevel=-1,
             )
             portage.writemsg("!!! PORTAGE_DEBUG must be either 0 or 1\n", noiselevel=-1)
             PORTAGE_DEBUG = 0
     except ValueError as e:
         portage.writemsg(f"!!! {str(e)}\n", noiselevel=-1)
         portage.writemsg(
-            "!!! Unable to parse integer: PORTAGE_DEBUG='%s'\n"
-            % settings["PORTAGE_DEBUG"],
+            f"!!! Unable to parse integer: PORTAGE_DEBUG='{settings['PORTAGE_DEBUG']}'\n",
             noiselevel=-1,
         )
         del e
     if "--debug" in myopts:
         PORTAGE_DEBUG = 1
     settings["PORTAGE_DEBUG"] = str(PORTAGE_DEBUG)
     settings.backup_changes("PORTAGE_DEBUG")
@@ -2779,16 +2764,16 @@
         settings["PORTAGE_BINPKG_FORMAT"] = myopts["--pkg-format"]
         settings.backup_changes("PORTAGE_BINPKG_FORMAT")
 
 
 def display_missing_pkg_set(root_config, set_name):
     msg = []
     msg.append(
-        ("emerge: There are no sets to satisfy '%s'. " + "The following sets exist:")
-        % colorize("INFORM", set_name)
+        f"emerge: There are no sets to satisfy '{colorize('INFORM', set_name)}'. "
+        "The following sets exist:"
     )
     msg.append("")
 
     for s in sorted(root_config.sets):
         msg.append(f"    {s}")
     msg.append("")
 
@@ -2802,15 +2787,22 @@
         profilever = realpath[1 + len(basepath) :]
     else:
         profilever = None
     return profilever
 
 
 def getportageversion(portdir, _unused, profile, chost, vardb):
-    pythonver = "python %d.%d.%d-%s-%d" % sys.version_info[:]
+    pythonver = (
+        "python"
+        f" {sys.version_info[0]}"
+        f".{sys.version_info[1]}"
+        f".{sys.version_info[2]}"
+        f"-{sys.version_info[3]}"
+        f"-{sys.version_info[4]}"
+    )
     profilever = None
     repositories = vardb.settings.repositories
     if profile:
         profilever = relative_profile_path(portdir, profile)
         if profilever is None:
             try:
                 for parent in portage.grabfile(os.path.join(profile, "parent")):
@@ -3074,15 +3066,15 @@
     except portage.exception.CommandNotFound:
         # The OS kernel probably doesn't support ionice,
         # so return silently.
         return
 
     if rval != os.EX_OK:
         out = portage.output.EOutput()
-        out.eerror("PORTAGE_IONICE_COMMAND returned %d" % (rval,))
+        out.eerror(f"PORTAGE_IONICE_COMMAND returned {rval}")
         out.eerror(
             "See the make.conf(5) man page for PORTAGE_IONICE_COMMAND usage instructions."
         )
 
 
 def set_scheduling_policy(settings):
     scheduling_policy = settings.get("PORTAGE_SCHEDULING_POLICY")
@@ -3153,30 +3145,30 @@
 
 
 def missing_sets_warning(root_config, missing_sets):
     if len(missing_sets) > 2:
         missing_sets_str = ", ".join(f'"{s}"' for s in missing_sets[:-1])
         missing_sets_str += f', and "{missing_sets[-1]}"'
     elif len(missing_sets) == 2:
-        missing_sets_str = '"%s" and "%s"' % tuple(missing_sets)
+        missing_sets_str = f'"{missing_sets[0]}" and "{missing_sets[1]}"'
     else:
         missing_sets_str = f'"{missing_sets[-1]}"'
     msg = [
         "emerge: incomplete set configuration, " + f"missing set(s): {missing_sets_str}"
     ]
     if root_config.sets:
         msg.append(f"        sets defined: {', '.join(root_config.sets)}")
     global_config_path = portage.const.GLOBAL_CONFIG_PATH
     if portage.const.EPREFIX:
         global_config_path = os.path.join(
             portage.const.EPREFIX, portage.const.GLOBAL_CONFIG_PATH.lstrip(os.sep)
         )
     msg.append(
-        "        This usually means that '%s'"
-        % (os.path.join(global_config_path, "sets/portage.conf"),)
+        "        This usually means that "
+        f"'{os.path.join(global_config_path, 'sets/portage.conf')}'"
     )
     msg.append("        is missing or corrupt.")
     msg.append("        Falling back to default world and system set configuration!!!")
     for line in msg:
         writemsg_level(line + "\n", level=logging.ERROR, noiselevel=-1)
 
 
@@ -3279,34 +3271,26 @@
                 newargs.append(a)
                 continue
 
             try:
                 set_atoms = setconfig.getSetAtoms(s)
             except portage.exception.PackageSetNotFound as e:
                 writemsg_level(
-                    (
-                        "emerge: the given set '%s' "
-                        + "contains a non-existent set named '%s'.\n"
-                    )
-                    % (s, e),
+                    f"emerge: the given set '{s}' contains a non-existent set named '{e}'.\n",
                     level=logging.ERROR,
                     noiselevel=-1,
                 )
                 if (
                     s in ("world", "selected")
                     and SETPREFIX + e.value in sets["selected"]
                 ):
                     writemsg_level(
                         (
-                            "Use `emerge --deselect %s%s` to "
+                            f"Use `emerge --deselect {SETPREFIX}{e}` to "
                             "remove this set from world_sets.\n"
-                        )
-                        % (
-                            SETPREFIX,
-                            e,
                         ),
                         level=logging.ERROR,
                         noiselevel=-1,
                     )
                 return (None, 1)
             if myaction in unmerge_actions and not sets[s].supportsOperation("unmerge"):
                 writemsg_level(
@@ -3515,19 +3499,15 @@
         if not fmt in portage.const.SUPPORTED_BINPKG_FORMATS:
             if "--pkg-format" in emerge_config.opts:
                 problematic = "--pkg-format"
             else:
                 problematic = "PORTAGE_BINPKG_FORMAT"
 
             writemsg_level(
-                (
-                    "emerge: %s is not set correctly. Format "
-                    + "'%s' is not supported.\n"
-                )
-                % (problematic, fmt),
+                f"emerge: {problematic} is not set correctly. Format '{fmt}' is not supported.\n",
                 level=logging.ERROR,
                 noiselevel=-1,
             )
             return 1
 
     if emerge_config.action == "version":
         writemsg_stdout(
@@ -3538,17 +3518,14 @@
                 emerge_config.target_config.settings.get("CHOST"),
                 emerge_config.target_config.trees["vartree"].dbapi,
             )
             + "\n",
             noiselevel=-1,
         )
         return 0
-    if emerge_config.action == "help":
-        emerge_help()
-        return 0
 
     spinner = stdout_spinner()
     if "candy" in emerge_config.target_config.settings.features:
         spinner.update = spinner.update_scroll
 
     if "--quiet" not in emerge_config.opts:
         portage.deprecated_profile_check(settings=emerge_config.target_config.settings)
@@ -3594,16 +3571,15 @@
 
     if (
         emerge_config.action is None
         and "--resume" in emerge_config.opts
         and emerge_config.args
     ):
         writemsg(
-            "emerge: unexpected argument(s) for --resume: %s\n"
-            % " ".join(emerge_config.args),
+            f"emerge: unexpected argument(s) for --resume: {' '.join(emerge_config.args)}\n",
             noiselevel=-1,
         )
         return 1
 
     # only expand sets for actions taking package arguments
     oldargs = emerge_config.args[:]
     if emerge_config.action in (
@@ -3737,15 +3713,15 @@
                         )
                         == "No"
                     ):
                         return 128 + signal.SIGINT
                     emerge_config.opts["--pretend"] = True
                     emerge_config.opts.pop("--ask")
                 else:
-                    sys.stderr.write(("emerge: %s access is required\n") % access_desc)
+                    sys.stderr.write(f"emerge: {access_desc} access is required\n")
                     if portage.data.secpass < 1 and not need_superuser:
                         portage.data.portage_group_warning()
                     return 1
 
     # Disable emergelog for everything except build or unmerge operations.
     # This helps minimize parallel emerge.log entries that can confuse log
     # parsers like genlop.
@@ -3849,16 +3825,15 @@
             xtermTitleReset()
 
     portage.atexit_register(emergeexit)
 
     if emerge_config.action in ("config", "metadata", "regen", "sync"):
         if "--pretend" in emerge_config.opts:
             sys.stderr.write(
-                ("emerge: The '%s' action does " + "not support '--pretend'.\n")
-                % emerge_config.action
+                f"emerge: The '{emerge_config.action}' action does not support '--pretend'.\n"
             )
             return 1
 
     if "sync" == emerge_config.action:
         return action_sync(emerge_config)
     if "metadata" == emerge_config.action:
         action_metadata(
```

### Comparing `portage-3.0.47/lib/_emerge/chk_updated_cfg_files.py` & `portage-3.0.48/lib/_emerge/chk_updated_cfg_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,31 +18,31 @@
         writemsg_level(
             f"\n {colorize('WARN', '* ' + _('IMPORTANT:'))} ",
             level=logging.INFO,
             noiselevel=-1,
         )
         if not x[1]:  # it's a protected file
             writemsg_level(
-                _("config file '%s' needs updating.\n") % x[0],
+                f"config file '{x[0]}' needs updating.\n",
                 level=logging.INFO,
                 noiselevel=-1,
             )
         else:  # it's a protected dir
             if len(x[1]) == 1:
                 head, tail = os.path.split(x[1][0])
                 tail = tail[len("._cfg0000_") :]
                 fpath = os.path.join(head, tail)
                 writemsg_level(
-                    _("config file '%s' needs updating.\n") % fpath,
+                    f"config file '{fpath}' needs updating.\n",
                     level=logging.INFO,
                     noiselevel=-1,
                 )
             else:
                 writemsg_level(
-                    _("%d config files in '%s' need updating.\n") % (len(x[1]), x[0]),
+                    f"{len(x[1])} config files in '{x[0]}' need updating.\n",
                     level=logging.INFO,
                     noiselevel=-1,
                 )
 
     if result:
         print(
             " "
```

### Comparing `portage-3.0.47/lib/_emerge/create_depgraph_params.py` & `portage-3.0.48/lib/_emerge/create_depgraph_params.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/create_world_atom.py` & `portage-3.0.48/lib/_emerge/create_world_atom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/depgraph.py` & `portage-3.0.48/lib/_emerge/depgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     InvalidAtom,
     InvalidBinaryPackageFormat,
     InvalidData,
     InvalidDependString,
     PackageNotFound,
     PortageException,
 )
-from portage.localization import _
 from portage.output import colorize, create_color_func, darkgreen, green
 
 bad = create_color_func("BAD")
 from portage.package.ebuild.config import _get_feature_flags
 from portage.package.ebuild.getmaskingstatus import _getmaskingstatus, _MaskReason
 from portage._sets import SETPREFIX
 from portage._sets.base import InternalPackageSet
@@ -1127,19 +1126,15 @@
         # graph, so it's safe to silently ignore them. This suppresses
         # noise for the unaffected user, even though some of the changed
         # dependencies might be worthy of revision bumps.
         if not in_graph:
             return
 
         writemsg(
-            "\n%s\n\n"
-            % colorize(
-                "WARN",
-                "!!! Detected ebuild dependency change(s) without revision bump:",
-            ),
+            f"\n{colorize('WARN','!!! Detected ebuild dependency change(s) without revision bump:')}\n\n",
             noiselevel=-1,
         )
 
         for pkg, ebuild in report_pkgs:
             writemsg(f"    {pkg.cpv}::{pkg.repo}", noiselevel=-1)
             if pkg.root_config.settings["ROOT"] != "/":
                 writemsg(f" for {pkg.root}", noiselevel=-1)
@@ -1407,22 +1402,21 @@
             msg.append(str(pkg.slot_atom))
             if pkg.root_config.settings["ROOT"] != "/":
                 msg.append(f" for {pkg.root}")
             msg.append("\n\n")
 
             msg.append(indent)
             msg.append(
-                "%s %s"
-                % (
-                    pkg,
+                f"{pkg} "
+                + str(
                     pkg_use_display(
                         pkg,
                         self._frozen_config.myopts,
                         modified_use=self._pkg_use_enabled(pkg),
-                    ),
+                    )
                 )
             )
             msg.append(" conflicts with\n")
 
             for parent, atom in parent_atoms:
                 if isinstance(parent, (PackageArg, AtomArg)):
                     # For PackageArg and AtomArg types, it's
@@ -1642,16 +1636,15 @@
                 if debug:
                     writemsg_level(
                         f"      parent: {parent}\n",
                         level=logging.DEBUG,
                         noiselevel=-1,
                     )
                     writemsg_level(
-                        "      arg, non-conflict: %s, %s\n"
-                        % (is_arg_parent, is_non_conflict_parent),
+                        f"      arg, non-conflict: {is_arg_parent}, {is_non_conflict_parent}\n",
                         level=logging.DEBUG,
                         noiselevel=-1,
                     )
                     writemsg_level(
                         f"         atom: {atom}\n", level=logging.DEBUG, noiselevel=-1
                     )
 
@@ -1902,16 +1895,16 @@
         for pkg in slot_nodes:
             if (
                 self._dynamic_config._allow_backtracking
                 and pkg in self._dynamic_config._runtime_pkg_mask
             ):
                 if debug:
                     writemsg_level(
-                        "!!! backtracking loop detected: %s %s\n"
-                        % (pkg, self._dynamic_config._runtime_pkg_mask[pkg]),
+                        f"!!! backtracking loop detected: {pkg} "
+                        f"{self._dynamic_config._runtime_pkg_mask[pkg]}\n",
                         level=logging.DEBUG,
                         noiselevel=-1,
                     )
 
             parent_atoms = self._dynamic_config._parent_atoms.get(pkg)
             if parent_atoms is None:
                 parent_atoms = set()
@@ -2306,16 +2299,15 @@
                     ) in self._dynamic_config._parent_atoms.get(existing_pkg, []):
                         if other_parent is parent:
                             parent_atoms.append(other_atom)
                     msg = (
                         "",
                         "",
                         "_slot_operator_check_reverse_dependencies:",
-                        "   candidate package does not match atom '%s': %s"
-                        % (atom, candidate_pkg),
+                        f"   candidate package does not match atom '{atom}': {candidate_pkg}",
                         f"   parent: {parent}",
                         f"   parent atoms: {' '.join(parent_atoms)}",
                         "",
                     )
                     writemsg_level("\n".join(msg), noiselevel=-1, level=logging.DEBUG)
                 return False
         return True
@@ -2549,16 +2541,16 @@
         if debug:
             msg = (
                 "",
                 "",
                 "slot_operator_update_probe:",
                 f"   existing child package:  {dep.child}",
                 f"   existing parent package: {dep.parent}",
-                "   new child package:  %s" % None,
-                "   new parent package: %s" % None,
+                "   new child package:  None",
+                "   new parent package: None",
                 "",
             )
             writemsg_level("\n".join(msg), noiselevel=-1, level=logging.DEBUG)
 
         return None
 
     def _slot_operator_unsatisfied_probe(self, dep):
@@ -2613,16 +2605,16 @@
         if debug:
             msg = (
                 "",
                 "",
                 "slot_operator_unsatisfied_probe:",
                 f"   existing parent package: {dep.parent}",
                 f"   existing parent atom: {dep.atom}",
-                "   new parent package: %s" % None,
-                "   new child package:  %s" % None,
+                "   new parent package: None",
+                "   new child package:  None",
                 "",
             )
             writemsg_level("\n".join(msg), noiselevel=-1, level=logging.DEBUG)
 
         return False
 
     def _slot_operator_unsatisfied_backtrack(self, dep):
@@ -3287,24 +3279,23 @@
             priority = dep.priority
             depth = dep.depth
         if priority is None:
             priority = DepPriority()
 
         if debug:
             writemsg_level(
-                "\n%s%s %s\n"
-                % (
-                    "Child:".ljust(15),
-                    pkg,
+                f"\n{'Child:':15}{pkg} "
+                + str(
                     pkg_use_display(
                         pkg,
                         self._frozen_config.myopts,
                         modified_use=self._pkg_use_enabled(pkg),
-                    ),
-                ),
+                    )
+                )
+                + "\n",
                 level=logging.DEBUG,
                 noiselevel=-1,
             )
             if isinstance(myparent, (PackageArg, AtomArg)):
                 # For PackageArg and AtomArg types, it's
                 # redundant to display the atom attribute.
                 writemsg_level(
@@ -3319,16 +3310,15 @@
                 if (
                     dep.atom
                     and dep.atom.package
                     and dep.atom is not dep.atom.unevaluated_atom
                 ):
                     uneval = f" ({dep.atom.unevaluated_atom})"
                 writemsg_level(
-                    "%s%s%s required by %s\n"
-                    % ("Parent Dep:".ljust(15), dep.atom, uneval, myparent),
+                    f"{'Parent Dep:':15}{dep.atom}{uneval} required by {myparent}\n",
                     level=logging.DEBUG,
                     noiselevel=-1,
                 )
 
         # Ensure that the dependencies of the same package
         # are never processed more than once.
         previously_added = pkg in self._dynamic_config.digraph
@@ -3399,24 +3389,23 @@
                             if not pkg.installed:
                                 # should have been masked before
                                 # it was selected
                                 raise
 
                         if debug:
                             writemsg_level(
-                                "%s%s %s\n"
-                                % (
-                                    "Re-used Child:".ljust(15),
-                                    pkg,
+                                f"{'Re-used Child:':15}{pkg} "
+                                + str(
                                     pkg_use_display(
                                         pkg,
                                         self._frozen_config.myopts,
                                         modified_use=self._pkg_use_enabled(pkg),
-                                    ),
-                                ),
+                                    )
+                                )
+                                + "\n",
                                 level=logging.DEBUG,
                                 noiselevel=-1,
                             )
                 elif (
                     pkg.installed
                     and isinstance(myparent, Package)
                     and pkg.root == myparent.root
@@ -3425,42 +3414,40 @@
                     # If the parent package is replacing the child package then
                     # there's no slot conflict. Since the child will be replaced,
                     # do not add it to the graph. No attempt will be made to
                     # satisfy its dependencies, which is unsafe if it has any
                     # missing dependencies, as discussed in bug 199856.
                     if debug:
                         writemsg_level(
-                            "%s%s %s\n"
-                            % (
-                                "Replace Child:".ljust(15),
-                                pkg,
+                            f"{'Replace Child:':15}{pkg} "
+                            + str(
                                 pkg_use_display(
                                     pkg,
                                     self._frozen_config.myopts,
                                     modified_use=self._pkg_use_enabled(pkg),
-                                ),
-                            ),
+                                )
+                            )
+                            + "\n",
                             level=logging.DEBUG,
                             noiselevel=-1,
                         )
                     return 1
 
                 else:
                     if debug:
                         writemsg_level(
-                            "%s%s %s\n"
-                            % (
-                                "Slot Conflict:".ljust(15),
-                                existing_node,
+                            f"{'Slot Conflict:':15}{existing_node} "
+                            + str(
                                 pkg_use_display(
                                     existing_node,
                                     self._frozen_config.myopts,
                                     modified_use=self._pkg_use_enabled(existing_node),
-                                ),
-                            ),
+                                )
+                            )
+                            + "\n",
                             level=logging.DEBUG,
                             noiselevel=-1,
                         )
 
             if not previously_added:
                 self._dynamic_config._package_tracker.add_pkg(pkg)
                 self._dynamic_config._filtered_trees[pkg.root][
@@ -4538,15 +4525,15 @@
 
                 try:
                     binpkg_format = get_binpkg_format(x)
                 except InvalidBinaryPackageFormat as e:
                     writemsg(
                         colorize(
                             "BAD",
-                            "\n{e}\n" % x,
+                            f"\n{e}\n",
                         ),
                         noiselevel=-1,
                     )
                     continue
 
                 if binpkg_format == "xpak":
                     mytbz2 = portage.xpak.tbz2(x)
@@ -4585,39 +4572,35 @@
                 for pkg in self._iter_match_pkgs(
                     root_config, "binary", Atom(f"={mykey}")
                 ):
                     if x == os.path.realpath(bindb.bintree.getname(pkg.cpv)):
                         break
                 else:
                     writemsg(
-                        "\n%s\n\n"
-                        % colorize(
+                        "\n"
+                        + colorize(
                             "BAD",
-                            "*** "
-                            + _(
-                                "You need to adjust PKGDIR to emerge "
-                                "this package: %s"
-                            )
-                            % x,
-                        ),
+                            f"*** You need to adjust PKGDIR to emerge this package: {x}",
+                        )
+                        + "\n\n",
                         noiselevel=-1,
                     )
                     self._dynamic_config._skip_restart = True
                     return 0, myfavorites
 
                 args.append(PackageArg(arg=x, package=pkg, root_config=root_config))
             elif x.endswith(".ebuild"):
                 ebuild_path = portage.util.normalize_path(os.path.abspath(x))
                 pkgdir = os.path.dirname(ebuild_path)
                 tree_root = os.path.dirname(os.path.dirname(pkgdir))
                 cp = pkgdir[len(tree_root) + 1 :]
                 error_msg = (
-                    "\n\n!!! '%s' is not in a valid ebuild repository "
+                    f"\n\n!!! '{x}' is not in a valid ebuild repository "
                     "hierarchy or does not exist\n"
-                ) % x
+                )
                 if not portage.isvalidatom(cp):
                     writemsg(error_msg, noiselevel=-1)
                     return 0, myfavorites
                 cat = portage.catsplit(cp)[0]
                 mykey = cat + "/" + os.path.basename(ebuild_path[:-7])
                 if not portage.isvalidatom("=" + mykey):
                     writemsg(error_msg, noiselevel=-1)
@@ -4672,31 +4655,27 @@
                         os.path.dirname(os.path.dirname(os.path.dirname(ebuild_path)))
                     ),
                 )
                 args.append(PackageArg(arg=x, package=pkg, root_config=root_config))
             elif x.startswith(os.path.sep):
                 if not x.startswith(eroot):
                     portage.writemsg(
-                        ("\n\n!!! '%s' does not start with" + " $EROOT.\n") % x,
+                        f"\n\n!!! '{x}' does not start with $EROOT.\n",
                         noiselevel=-1,
                     )
                     self._dynamic_config._skip_restart = True
                     return 0, []
                 # Queue these up since it's most efficient to handle
                 # multiple files in a single iter_owners() call.
                 lookup_owners.append(x)
             elif x.startswith("." + os.sep) or x.startswith(".." + os.sep):
                 f = os.path.abspath(x)
                 if not f.startswith(eroot):
                     portage.writemsg(
-                        (
-                            "\n\n!!! '%s' (resolved from '%s') does not start with"
-                            + " $EROOT.\n"
-                        )
-                        % (f, x),
+                        f"\n\n!!! '{f}' (resolved from '{x}') does not start with $EROOT.\n",
                         noiselevel=-1,
                     )
                     self._dynamic_config._skip_restart = True
                     return 0, []
                 lookup_owners.append(f)
             else:
                 if x in ("system", "world"):
@@ -4717,35 +4696,26 @@
                                 writemsg_level(
                                     f"{error_msg}\n",
                                     level=logging.ERROR,
                                     noiselevel=-1,
                                 )
 
                         writemsg_level(
-                            (
-                                "emerge: the given set '%s' "
-                                "contains a non-existent set named '%s'.\n"
-                            )
-                            % (s, e),
+                            f"emerge: the given set '{s}' contains a non-existent set named "
+                            f"'{e}'.\n",
                             level=logging.ERROR,
                             noiselevel=-1,
                         )
                         if (
                             s in ("world", "selected")
                             and SETPREFIX + e.value in sets["selected"]
                         ):
                             writemsg_level(
-                                (
-                                    "Use `emerge --deselect %s%s` to "
-                                    "remove this set from world_sets.\n"
-                                )
-                                % (
-                                    SETPREFIX,
-                                    e,
-                                ),
+                                f"Use `emerge --deselect {SETPREFIX}{e}` to remove this set from "
+                                "world_sets.\n",
                                 level=logging.ERROR,
                                 noiselevel=-1,
                             )
                         writemsg_level("\n", level=logging.ERROR, noiselevel=-1)
                         return False, myfavorites
 
                     pset = sets[s]
@@ -4831,19 +4801,15 @@
                             null_atom.replace("null/", "virtual/", 1), allow_repo=True
                         )
                     else:
                         atom = null_atom
 
                 if atom.use and atom.use.conditional:
                     writemsg(
-                        (
-                            "\n\n!!! '%s' contains a conditional "
-                            + "which is not allowed.\n"
-                        )
-                        % (x,),
+                        f"\n\n!!! '{x}' contains a conditional which is not allowed.\n",
                         noiselevel=-1,
                     )
                     writemsg("!!! Please check ebuild(5) for full details.\n")
                     self._dynamic_config._skip_restart = True
                     return (0, [])
 
                 args.append(AtomArg(arg=x, atom=atom, root_config=root_config))
@@ -4863,16 +4829,15 @@
             for pkg, relative_path in real_vardb._owners.iter_owners(relative_paths):
                 owners.add(pkg.mycpv)
                 if not search_for_multiple:
                     break
 
             if not owners:
                 portage.writemsg(
-                    ("\n\n!!! '%s' is not claimed " + "by any package.\n")
-                    % lookup_owners[0],
+                    f"\n\n!!! '{lookup_owners[0]}' is not claimed by any package.\n",
                     noiselevel=-1,
                 )
                 self._dynamic_config._skip_restart = True
                 return 0, []
 
             for cpv in owners:
                 pkg = vardb._pkg_str(cpv, None)
@@ -4997,19 +4962,15 @@
                     if isinstance(arg, PackageArg):
                         if (
                             not self._add_pkg(arg.package, dep)
                             or not self._create_graph()
                         ):
                             if not self.need_restart():
                                 writemsg(
-                                    (
-                                        "\n\n!!! Problem "
-                                        + "resolving dependencies for %s\n"
-                                    )
-                                    % arg.arg,
+                                    f"\n\n!!! Problem resolving dependencies for {arg.arg}\n",
                                     noiselevel=-1,
                                 )
                             return 0, myfavorites
                         continue
                     if debug:
                         writemsg_level(
                             f"\n      Arg: {arg}\n     Atom: {atom}\n",
@@ -5113,25 +5074,21 @@
                     # so that later dep_check() calls can use it as feedback
                     # for making more consistent atom selections.
                     if not self._add_pkg(pkg, dep):
                         if self.need_restart():
                             pass
                         elif isinstance(arg, SetArg):
                             writemsg(
-                                (
-                                    "\n\n!!! Problem resolving "
-                                    + "dependencies for %s from %s\n"
-                                )
-                                % (atom, arg.arg),
+                                f"\n\n!!! Problem resolving dependencies for {atom} from "
+                                f"{arg.arg}\n",
                                 noiselevel=-1,
                             )
                         else:
                             writemsg(
-                                ("\n\n!!! Problem resolving " + "dependencies for %s\n")
-                                % (atom,),
+                                f"\n\n!!! Problem resolving dependencies for {atom}\n",
                                 noiselevel=-1,
                             )
                         return 0, myfavorites
 
                 except SystemExit as e:
                     raise  # Needed else can't exit
                 except Exception as e:
@@ -6205,16 +6162,16 @@
                     if check_required_use(
                         required_use, old_use, pkg.iuse.is_valid_flag, eapi=pkg.eapi
                     ) and not check_required_use(
                         required_use, new_use, pkg.iuse.is_valid_flag, eapi=pkg.eapi
                     ):
                         required_use_warning = (
                             ", this change violates use flag constraints "
-                            + "defined by %s: '%s'"
-                            % (pkg.cpv, human_readable_required_use(required_use))
+                            f"defined by {pkg.cpv}: "
+                            f"'{human_readable_required_use(required_use)}'"
                         )
 
                 if need_enable or need_disable:
                     changes = []
                     changes.extend(colorize("red", "+" + x) for x in need_enable)
                     changes.extend(colorize("blue", "-" + x) for x in need_disable)
                     mreasons.append(
@@ -6276,19 +6233,16 @@
                             required_use,
                             new_use,
                             myparent.iuse.is_valid_flag,
                             eapi=myparent.eapi,
                         ):
                             required_use_warning = (
                                 ", this change violates use flag constraints "
-                                + "defined by %s: '%s'"
-                                % (
-                                    myparent.cpv,
-                                    human_readable_required_use(required_use),
-                                )
+                                f"defined by {myparent.cpv}: "
+                                f"'{human_readable_required_use(required_use)}'"
                             )
 
                     target_use = {}
                     for flag in involved_flags:
                         if flag in self._pkg_use_enabled(myparent):
                             target_use[flag] = False
                             changes.append(colorize("blue", "-" + flag))
@@ -6463,39 +6417,38 @@
                 noiselevel=-1,
             )
             have_eapi_mask = show_masked_packages(masked_packages)
             if have_eapi_mask:
                 writemsg("\n", noiselevel=-1)
                 msg = (
                     "The current version of portage supports "
-                    + "EAPI '%s'. You must upgrade to a newer version"
-                    + " of portage before EAPI masked packages can"
-                    + " be installed."
-                ) % portage.const.EAPI
+                    f"EAPI '{portage.const.EAPI}'. You must upgrade to a newer version"
+                    " of portage before EAPI masked packages can"
+                    " be installed."
+                )
                 writemsg("\n".join(textwrap.wrap(msg, 75)), noiselevel=-1)
             writemsg("\n", noiselevel=-1)
             mask_docs = True
         else:
             cp_exists = False
             if atom.package and not atom.cp.startswith("null/"):
                 for pkg in self._iter_match_pkgs_any(root_config, Atom(atom.cp)):
                     cp_exists = True
                     break
 
-            writemsg(
-                "\nemerge: there are no %s to satisfy "
-                % (
-                    "binary packages"
-                    if self._frozen_config.myopts.get("--usepkgonly", "y") == True
-                    else "ebuilds"
+            if self._frozen_config.myopts.get("--usepkgonly", "y"):
+                writemsg(
+                    f"\nemerge: there are no binary packages to satisfy {green(xinfo)}.\n",
+                    noiselevel=-1,
+                )
+            else:
+                writemsg(
+                    f"\nemerge: there are no ebuilds to satisfy {green(xinfo)}.\n",
+                    noiselevel=-1,
                 )
-                + green(xinfo)
-                + ".\n",
-                noiselevel=-1,
-            )
             if (
                 isinstance(myparent, AtomArg)
                 and not cp_exists
                 and self._frozen_config.myopts.get("--misspell-suggestions", "y") != "n"
             ):
                 writemsg("\nemerge: searching for similar names...", noiselevel=-1)
 
@@ -6514,31 +6467,29 @@
 
                 if len(matches) == 1:
                     writemsg(
                         "\nemerge: Maybe you meant " + matches[0] + "?\n", noiselevel=-1
                     )
                 elif len(matches) > 1:
                     writemsg(
-                        "\nemerge: Maybe you meant any of these: %s?\n"
-                        % (", ".join(matches),),
+                        f"\nemerge: Maybe you meant any of these: {', '.join(matches)}?\n",
                         noiselevel=-1,
                     )
                 else:
                     # Generally, this would only happen if
                     # all dbapis are empty.
                     writemsg(" nothing similar found.\n", noiselevel=-1)
         msg = []
         if not isinstance(myparent, AtomArg):
             # It's redundant to show parent for AtomArg since
             # it's the same as 'xinfo' displayed above.
             dep_chain = self._get_dep_chain(myparent, atom)
             for node, node_type in dep_chain:
                 msg.append(
-                    '(dependency required by "%s" [%s])'
-                    % (colorize("INFORM", "%s" % (node)), node_type)
+                    f'(dependency required by "{colorize("INFORM", str(node))}" [{node_type}])'
                 )
 
         if msg:
             writemsg("\n".join(msg), noiselevel=-1)
             writemsg("\n", noiselevel=-1)
 
         if mask_docs:
@@ -7746,21 +7697,15 @@
 
         if not matched_packages:
             return None, None
 
         if "--debug" in self._frozen_config.myopts:
             for pkg in matched_packages:
                 portage.writemsg(
-                    "%s %s%s%s\n"
-                    % (
-                        (pkg.type_name + ":").rjust(10),
-                        pkg.cpv,
-                        _repo_separator,
-                        pkg.repo,
-                    ),
+                    f"{pkg.type_name + ':':>10} {pkg.cpv}{_repo_separator}{pkg.repo}\n",
                     noiselevel=-1,
                 )
 
         # Filter out any old-style virtual matches if they are
         # mixed with new-style virtual matches.
         cp = atom_cp
         if (
@@ -8958,16 +8903,15 @@
                     myuse=self._pkg_use_enabled(running_portage),
                     parent=running_portage,
                     strict=False,
                 )
             except portage.exception.InvalidDependString as e:
                 portage.writemsg(
                     "!!! Invalid RDEPEND in "
-                    + "'%svar/db/pkg/%s/RDEPEND': %s\n"
-                    % (running_root, running_portage.cpv, e),
+                    f"'{running_root}var/db/pkg/{running_portage.cpv}/RDEPEND': {e}\n",
                     noiselevel=-1,
                 )
                 del e
                 portage_rdepend = {running_portage: []}
             for atoms in portage_rdepend.values():
                 runtime_deps.update(atom for atom in atoms if not atom.blocker)
 
@@ -9243,16 +9187,15 @@
                         # that we have intentionally ignored, select
                         # only one node here, so that merge order
                         # accounts for as many dependencies as possible.
                         selected_nodes = [leaves[0]]
 
                     if debug:
                         writemsg(
-                            "\nruntime cycle digraph (%s nodes):\n\n"
-                            % (len(selected_nodes),),
+                            f"\nruntime cycle digraph ({len(selected_nodes)} nodes):\n\n",
                             noiselevel=-1,
                         )
                         cycle_digraph.debug_print()
                         writemsg("\n", noiselevel=-1)
 
                         if leaves:
                             writemsg(
@@ -9691,16 +9634,17 @@
                 msg = [
                     "enabling 'complete' depgraph mode " "due to uninstall task(s):",
                     "",
                 ]
                 for node in retlist:
                     if isinstance(node, Package) and node.operation == "uninstall":
                         msg.append(f"\t{node}")
+                temp_joined = "".join(f"{line}\n" for line in msg)
                 writemsg_level(
-                    "\n%s\n" % "".join("%s\n" % line for line in msg),
+                    f"\n{temp_joined}\n",
                     level=logging.DEBUG,
                     noiselevel=-1,
                 )
             raise self._serialize_tasks_retry("")
 
         # Set satisfied state on blockers, but not before the
         # above retry path, since we don't want to modify the
@@ -9908,16 +9852,16 @@
                         else:
                             use_display = ""
                         if atom.package and atom != atom.unevaluated_atom:
                             # Show the unevaluated atom, since it can reveal
                             # issues with conditional use-flags missing
                             # from IUSE.
                             msg.append(
-                                "%s (%s) required by %s %s"
-                                % (atom.unevaluated_atom, atom, parent, use_display)
+                                f"{atom.unevaluated_atom} ({atom}) "
+                                f"required by {parent} {use_display}"
                             )
                         else:
                             msg.append(f"{atom} required by {parent} {use_display}")
                     msg.append("\n")
 
                 msg.append("\n")
 
@@ -10243,16 +10187,15 @@
                     file_to_write_to[
                         (abs_user_config, "package.license")
                     ] = find_config_file(abs_user_config, "package.license")
 
             for (abs_user_config, f), path in file_to_write_to.items():
                 if path is None:
                     problems.append(
-                        "!!! No file to write for '%s'\n"
-                        % os.path.join(abs_user_config, f)
+                        f"!!! No file to write for '{os.path.join(abs_user_config, f)}'\n"
                     )
 
             write_to_file = not problems
 
         def format_msg(lines):
             lines = lines[:]
             for i, line in enumerate(lines):
@@ -10268,19 +10211,16 @@
             )
 
             if len(roots) > 1:
                 writemsg(f"\nFor {abs_user_config}:\n", noiselevel=-1)
 
             def _writemsg(reason, file):
                 writemsg(
-                    (
-                        "\nThe following %s are necessary to proceed:\n"
-                        ' (see "%s" in the portage(5) man page for more details)\n'
-                    )
-                    % (colorize("BAD", reason), file),
+                    f"\nThe following {colorize('BAD', reason)} are necessary to proceed:\n"
+                    f' (see "{file}" in the portage(5) man page for more details)\n',
                     noiselevel=-1,
                 )
 
             if root in unstable_keyword_msg:
                 _writemsg("keyword changes", "package.accept_keywords")
                 writemsg(format_msg(unstable_keyword_msg[root]), noiselevel=-1)
 
@@ -10670,16 +10610,15 @@
                     added_favorites.add(myfavkey)
             except portage.exception.InvalidDependString as e:
                 writemsg(
                     f"\n\n!!! '{x.cpv}' has invalid PROVIDE: {e}\n",
                     noiselevel=-1,
                 )
                 writemsg(
-                    "!!! see '%s'\n\n"
-                    % os.path.join(x.root, portage.VDB_PATH, x.cpv, "PROVIDE"),
+                    f"!!! see '{os.path.join(x.root, portage.VDB_PATH, x.cpv, 'PROVIDE')}'\n\n",
                     noiselevel=-1,
                 )
                 del e
         all_added = []
         for arg in self._dynamic_config._initial_arg_list:
             if not isinstance(arg, SetArg):
                 continue
@@ -10714,16 +10653,16 @@
             if not skip:
                 for a in all_added:
                     if a.startswith(SETPREFIX):
                         filename = "world_sets"
                     else:
                         filename = "world"
                     writemsg_stdout(
-                        '>>> Recording %s in "%s" favorites file...\n'
-                        % (colorize("INFORM", str(a)), filename),
+                        f">>> Recording {colorize('INFORM', str(a))} "
+                        f'in "{filename}" favorites file...\n',
                         noiselevel=-1,
                     )
                 world_set.update(all_added)
 
         if world_locked:
             world_set.unlock()
 
@@ -11758,18 +11697,15 @@
         portdb = root_config.trees["porttree"].dbapi
         for l in missing_licenses:
             if l in shown_licenses:
                 continue
             l_path = portdb.findLicensePath(l)
             if l_path is None:
                 continue
-            msg = ("A copy of the '%s' license" + " is located at '%s'.\n\n") % (
-                l,
-                l_path,
-            )
+            msg = f"A copy of the '{l}' license is located at '{l_path}'.\n\n"
             writemsg(msg, noiselevel=-1)
             shown_licenses.add(l)
     return have_eapi_mask
 
 
 def show_mask_docs():
     writemsg(
```

### Comparing `portage-3.0.47/lib/_emerge/emergelog.py` & `portage-3.0.48/lib/_emerge/emergelog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/getloadavg.py` & `portage-3.0.48/lib/_emerge/getloadavg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/help.py` & `portage-3.0.48/lib/_emerge/help.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/is_valid_package_atom.py` & `portage-3.0.48/lib/_emerge/is_valid_package_atom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/main.py` & `portage-3.0.48/lib/_emerge/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/post_emerge.py` & `portage-3.0.48/lib/_emerge/post_emerge.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/resolver/DbapiProvidesIndex.py` & `portage-3.0.48/lib/_emerge/resolver/DbapiProvidesIndex.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/resolver/backtracking.py` & `portage-3.0.48/lib/_emerge/resolver/backtracking.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/resolver/circular_dependency.py` & `portage-3.0.48/lib/_emerge/resolver/circular_dependency.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/resolver/output.py` & `portage-3.0.48/lib/_emerge/resolver/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,15 @@
         if blocker.atom.blocker.overlap.forbid:
             blocking_desc = "hard blocking"
         else:
             blocking_desc = "soft blocking"
         if self.resolved != blocker.atom:
             addl += colorize(
                 self.blocker_style,
-                ' ("%s" is %s %s)'
-                % (str(blocker.atom).lstrip("!"), blocking_desc, block_parents),
+                f' ("{str(blocker.atom).lstrip("!")}" is {blocking_desc} {block_parents})',
             )
         else:
             addl += colorize(
                 self.blocker_style, f" (is {blocking_desc} {block_parents})"
             )
         if blocker.satisfied:
             if not self.conf.columns:
```

### Comparing `portage-3.0.47/lib/_emerge/resolver/output_helpers.py` & `portage-3.0.48/lib/_emerge/resolver/output_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,24 +146,25 @@
         myoutput.append(f", Size of downloads: {localized_size(self.totalsize)}")
         if self.restrict_fetch:
             myoutput.append(f"\nFetch Restriction: {self.restrict_fetch} package")
             if self.restrict_fetch > 1:
                 myoutput.append("s")
         if self.restrict_fetch_satisfied < self.restrict_fetch:
             myoutput.append(
-                bad(" (%s unsatisfied)")
-                % (self.restrict_fetch - self.restrict_fetch_satisfied)
+                bad(
+                    f" ({self.restrict_fetch - self.restrict_fetch_satisfied} unsatisfied)"
+                )
             )
         if self.blocks > 0:
             myoutput.append(f"\nConflict: {self.blocks} block")
             if self.blocks > 1:
                 myoutput.append("s")
             if self.blocks_satisfied < self.blocks:
                 myoutput.append(
-                    bad(" (%s unsatisfied)") % (self.blocks - self.blocks_satisfied)
+                    bad(f" ({self.blocks - self.blocks_satisfied} unsatisfied)")
                 )
             else:
                 myoutput.append(" (all satisfied)")
         return "".join(myoutput)
 
 
 class _DisplayConfig:
@@ -201,16 +202,15 @@
         mywidth = 130
         if "COLUMNWIDTH" in frozen_config.settings:
             try:
                 mywidth = int(frozen_config.settings["COLUMNWIDTH"])
             except ValueError as e:
                 writemsg(f"!!! {str(e)}\n", noiselevel=-1)
                 writemsg(
-                    "!!! Unable to parse COLUMNWIDTH='%s'\n"
-                    % frozen_config.settings["COLUMNWIDTH"],
+                    f"!!! Unable to parse COLUMNWIDTH='{frozen_config.settings['COLUMNWIDTH']}'\n",
                     noiselevel=-1,
                 )
                 del e
         self.columnwidth = mywidth
 
         if "--quiet-repo-display" in frozen_config.myopts:
             self.repo_display = _RepoDisplay(frozen_config.roots)
```

### Comparing `portage-3.0.47/lib/_emerge/resolver/package_tracker.py` & `portage-3.0.48/lib/_emerge/resolver/package_tracker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/resolver/slot_collision.py` & `portage-3.0.48/lib/_emerge/resolver/slot_collision.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,22 +262,21 @@
             if root != self.depgraph._frozen_config._running_root.root:
                 msg.append(f" for {root}")
             msg.append("\n\n")
 
             for pkg in pkgs:
                 msg.append(indent)
                 msg.append(
-                    "%s %s"
-                    % (
-                        pkg,
+                    f"{pkg} "
+                    + str(
                         pkg_use_display(
                             pkg,
                             self.depgraph._frozen_config.myopts,
                             modified_use=self.depgraph._pkg_use_enabled(pkg),
-                        ),
+                        )
                     )
                 )
                 parent_atoms = self.all_parents.get(pkg)
                 if parent_atoms:
                     # Create a list of collision reasons and map them to sets
                     # of atoms.
                     # Possible reasons:
@@ -364,27 +363,20 @@
                                     if violated_atom.use is None:
                                         # Something like bug #453400 caused the
                                         # above findAtomForPackage call to
                                         # return None unexpectedly.
                                         msg = (
                                             "\n\n!!! BUG: Detected "
                                             "USE dep match inconsistency:\n"
-                                            "\tppkg: %s\n"
-                                            "\tviolated_atom: %s\n"
-                                            "\tatom: %s unevaluated: %s\n"
-                                            "\tother_pkg: %s IUSE: %s USE: %s\n"
-                                            % (
-                                                ppkg,
-                                                violated_atom,
-                                                atom,
-                                                atom.unevaluated_atom,
-                                                other_pkg,
-                                                sorted(other_pkg.iuse.all),
-                                                sorted(_pkg_use_enabled(other_pkg)),
-                                            )
+                                            f"\tppkg: {ppkg}\n"
+                                            f"\tviolated_atom: {violated_atom}\n"
+                                            f"\tatom: {atom} unevaluated: {atom.unevaluated_atom}\n"
+                                            f"\tother_pkg: {other_pkg} "
+                                            f"IUSE: {sorted(other_pkg.iuse.all)} "
+                                            f"USE: {sorted(_pkg_use_enabled(other_pkg))}\n"
                                         )
                                         writemsg(msg, noiselevel=-2)
                                         raise AssertionError(
                                             "BUG: USE dep match inconsistency"
                                         )
                                     for flag in violated_atom.use.enabled.union(
                                         violated_atom.use.disabled
@@ -699,21 +691,19 @@
 
                     omitted_parents = num_all_specific_atoms - len(selected_for_display)
                     if omitted_parents:
                         any_omitted_parents = True
                         msg.append(2 * indent)
                         if len(selected_for_display) > 1:
                             msg.append(
-                                "(and %d more with the same problems)\n"
-                                % omitted_parents
+                                f"(and {omitted_parents} more with the same problems)\n"
                             )
                         else:
                             msg.append(
-                                "(and %d more with the same problem)\n"
-                                % omitted_parents
+                                f"(and {omitted_parents} more with the same problem)\n"
                             )
                 else:
                     msg.append(" (no parents)\n")
                 msg.append("\n")
 
         if any_omitted_parents:
             msg.append(
@@ -820,19 +810,15 @@
                     if pkg.iuse.all.symmetric_difference(
                         other_pkg.iuse.all
                     ) or _pkg_use_enabled(pkg).symmetric_difference(
                         _pkg_use_enabled(other_pkg)
                     ):
                         if self.debug:
                             writemsg(
-                                (
-                                    "%s has pending USE changes. "
-                                    "Rejecting configuration.\n"
-                                )
-                                % (pkg,),
+                                f"{pkg} has pending USE changes. Rejecting configuration.\n",
                                 noiselevel=-1,
                             )
                         return False
 
         # A list of dicts. Keeps one dict per slot conflict. [ { flag1: "enabled" }, { flag2: "disabled" } ]
         all_involved_flags = []
 
@@ -853,33 +839,26 @@
                     continue
 
                 i = InternalPackageSet(initial_atoms=(atom.without_use,))
                 if not i.findAtomForPackage(pkg, modified_use=_pkg_use_enabled(pkg)):
                     # Version range does not match.
                     if self.debug:
                         writemsg(
-                            (
-                                "%s does not satify all version "
-                                "requirements. Rejecting configuration.\n"
-                            )
-                            % (pkg,),
+                            f"{pkg} does not satify all version "
+                            "requirements. Rejecting configuration.\n",
                             noiselevel=-1,
                         )
                     return False
 
                 if not pkg.iuse.is_valid_flag(atom.unevaluated_atom.use.required):
                     # Missing IUSE.
                     # FIXME: This needs to support use dep defaults.
                     if self.debug:
                         writemsg(
-                            (
-                                "%s misses needed flags from IUSE."
-                                " Rejecting configuration.\n"
-                            )
-                            % (pkg,),
+                            f"{pkg} misses needed flags from IUSE. Rejecting configuration.\n",
                             noiselevel=-1,
                         )
                     return False
 
                 if not isinstance(ppkg, Package) or ppkg.installed:
                     # We cannot assume that it's possible to reinstall the package. Do not
                     # check if some of its atom has use.conditional
@@ -905,19 +884,16 @@
                 if pkg.installed and (
                     violated_atom.use.enabled or violated_atom.use.disabled
                 ):
                     # We can't change USE of an installed package (only of an ebuild, but that is already
                     # part of the conflict, isn't it?)
                     if self.debug:
                         writemsg(
-                            (
-                                "%s: installed package would need USE"
-                                " changes. Rejecting configuration.\n"
-                            )
-                            % (pkg,),
+                            f"{pkg}: installed package would need USE changes. "
+                            "Rejecting configuration.\n",
                             noiselevel=-1,
                         )
                     return False
 
                 # Compute the required USE changes. A flag can be forced to "enabled" or "disabled",
                 # it can be in the conditional state "cond" that allows both values or in the
                 # "contradiction" state, which means that some atoms insist on different values
@@ -1181,19 +1157,16 @@
                 new_atom = atom.unevaluated_atom.evaluate_conditionals(ppkg_new_use)
                 i = InternalPackageSet(initial_atoms=(new_atom,))
                 if not i.findAtomForPackage(pkg, new_use):
                     # We managed to create a new problem with our changes.
                     is_valid_solution = False
                     if self.debug:
                         writemsg(
-                            (
-                                "new conflict introduced: %s"
-                                " does not match %s from %s\n"
-                            )
-                            % (pkg, new_atom, ppkg),
+                            f"new conflict introduced: {pkg} does not match "
+                            f"{new_atom} from {ppkg}\n",
                             noiselevel=-1,
                         )
                     break
 
             if not is_valid_solution:
                 break
```

### Comparing `portage-3.0.47/lib/_emerge/search.py` & `portage-3.0.48/lib/_emerge/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,16 +498,15 @@
 
                 if myebuild and file_size_str is None:
                     file_size_str = localized_size(mysum[0])
 
                 if self.verbose:
                     if available:
                         msg.append(
-                            "      %s %s\n"
-                            % (darkgreen("Latest version available:"), myversion)
+                            f"      {darkgreen('Latest version available:')} {myversion}\n"
                         )
                     msg.append(
                         f"      {self.getInstallationStatus(mycat + '/' + mypkg)}\n"
                     )
                     if myebuild:
                         msg.append(
                             f"      {darkgreen('Size of files:')} {file_size_str}\n"
```

### Comparing `portage-3.0.47/lib/_emerge/show_invalid_depstring_notice.py` & `portage-3.0.48/lib/_emerge/show_invalid_depstring_notice.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/stdout_spinner.py` & `portage-3.0.48/lib/_emerge/stdout_spinner.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/_emerge/unmerge.py` & `portage-3.0.48/lib/_emerge/unmerge.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import logging
 import signal
 import sys
 import textwrap
 import portage
 from portage import os
 from portage.dbapi._expand_new_virt import expand_new_virt
-from portage.localization import _
 from portage.output import bold, colorize, darkgreen, green
 from portage._sets import SETPREFIX
 from portage._sets.base import EditablePackageSet
 from portage.versions import cpv_sort_key, _pkg_str
 
 from _emerge.emergelog import emergelog
 from _emerge.Package import Package
@@ -224,16 +223,15 @@
                 print()
                 sys.exit(1)
 
             if not mymatch and x[0] not in "<>=~":
                 mymatch = vartree.dep_match(x)
             if not mymatch:
                 portage.writemsg(
-                    "\n--- Couldn't find '%s' to %s.\n"
-                    % (x.replace("null/", ""), unmerge_action),
+                    f"\n--- Couldn't find '{x.replace('null/', '')}' to {unmerge_action}.\n",
                     noiselevel=-1,
                 )
                 continue
 
             pkgmap.append({"protected": set(), "selected": set(), "omitted": set()})
             mykey = len(pkgmap) - 1
             if unmerge_action in ["rage-clean", "unmerge"]:
@@ -365,25 +363,25 @@
                 # by a concurrent process.
                 continue
 
             if unmerge_action != "clean" and root_config.root == "/":
                 skip_pkg = False
                 if portage.match_from_list(portage.const.PORTAGE_PACKAGE_ATOM, [pkg]):
                     msg = (
-                        "Not unmerging package %s "
+                        f"Not unmerging package {pkg.cpv} "
                         "since there is no valid reason for Portage to "
-                        "%s itself."
-                    ) % (pkg.cpv, unmerge_action)
+                        f"{unmerge_action} itself."
+                    )
                     skip_pkg = True
                 elif vartree.dbapi._dblink(cpv).isowner(portage._python_interpreter):
                     msg = (
-                        "Not unmerging package %s since there is no valid "
-                        "reason for Portage to %s currently used Python "
+                        f"Not unmerging package {pkg.cpv} since there is no valid "
+                        f"reason for Portage to {unmerge_action} currently used Python "
                         "interpreter."
-                    ) % (pkg.cpv, unmerge_action)
+                    )
                     skip_pkg = True
                 if skip_pkg:
                     for line in textwrap.wrap(msg, 75):
                         out.eerror(line)
                     # adjust pkgmap so the display output is correct
                     pkgmap[cp]["selected"].remove(cpv)
                     all_selected.remove(cpv)
@@ -400,20 +398,16 @@
 
                 if s not in sets:
                     if s in unknown_sets:
                         continue
                     unknown_sets.add(s)
                     out = portage.output.EOutput()
                     out.eerror(
-                        ("Unknown set '@%s' in %s%s")
-                        % (
-                            s,
-                            root_config.settings["EROOT"],
-                            portage.const.WORLD_SETS_FILE,
-                        )
+                        f"Unknown set '@{s}' in "
+                        f"{root_config.settings['EROOT']}{portage.const.WORLD_SETS_FILE}"
                     )
                     continue
 
                 # only check instances of EditablePackageSet as other classes are generally used for
                 # special purposes and can be ignored here (and are usually generated dynamically, so the
                 # user can't do much about them anyway)
                 if isinstance(sets[s], EditablePackageSet):
@@ -551,15 +545,15 @@
                 writemsg_level("none ", noiselevel=-1)
             if not quiet:
                 writemsg_level("\n", noiselevel=-1)
         if quiet:
             writemsg_level("\n", noiselevel=-1)
 
     writemsg_level(
-        "\nAll selected packages: %s\n" % " ".join("=%s" % x for x in all_selected),
+        f"\nAll selected packages: {' '.join(f'={x}' for x in all_selected)}\n",
         noiselevel=-1,
     )
 
     writemsg_level(
         "\n>>> "
         + colorize("UNMERGE_WARN", "'Selected'")
         + " packages are slated for removal.\n"
@@ -628,15 +622,15 @@
             print()
             print("Quitting.")
             print()
             return 128 + signal.SIGINT
 
     if not vartree.dbapi.writable:
         writemsg_level(
-            "!!! %s\n" % _("Read-only file system: %s") % vartree.dbapi._dbroot,
+            f"!!! Read-only file system: {vartree.dbapi._dbroot}\n",
             level=logging.ERROR,
             noiselevel=-1,
         )
         return 1
 
     # the real unmerging begins, after a short delay unless we're raging....
     if not unmerge_action == "rage-clean" and clean_delay and not autoclean:
```

### Comparing `portage-3.0.47/lib/portage/__init__.py` & `portage-3.0.48/lib/portage/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_compat_upgrade/binpkg_compression.py` & `portage-3.0.48/lib/portage/_compat_upgrade/binpkg_compression.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_compat_upgrade/binpkg_multi_instance.py` & `portage-3.0.48/lib/portage/_compat_upgrade/binpkg_multi_instance.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_compat_upgrade/default_locations.py` & `portage-3.0.48/lib/portage/_compat_upgrade/default_locations.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/Config.py` & `portage-3.0.48/lib/portage/_emirrordist/Config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/ContentDB.py` & `portage-3.0.48/lib/portage/_emirrordist/ContentDB.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/DeletionIterator.py` & `portage-3.0.48/lib/portage/_emirrordist/DeletionIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/DeletionTask.py` & `portage-3.0.48/lib/portage/_emirrordist/DeletionTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/FetchIterator.py` & `portage-3.0.48/lib/portage/_emirrordist/FetchIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/FetchTask.py` & `portage-3.0.48/lib/portage/_emirrordist/FetchTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/MirrorDistTask.py` & `portage-3.0.48/lib/portage/_emirrordist/MirrorDistTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_emirrordist/main.py` & `portage-3.0.48/lib/portage/_emirrordist/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_global_updates.py` & `portage-3.0.48/lib/portage/_global_updates.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_legacy_globals.py` & `portage-3.0.48/lib/portage/_legacy_globals.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_selinux.py` & `portage-3.0.48/lib/portage/_selinux.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/ProfilePackageSet.py` & `portage-3.0.48/lib/portage/_sets/ProfilePackageSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/__init__.py` & `portage-3.0.48/lib/portage/_sets/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/base.py` & `portage-3.0.48/lib/portage/_sets/base.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/dbapi.py` & `portage-3.0.48/lib/portage/_sets/dbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/files.py` & `portage-3.0.48/lib/portage/_sets/files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/libs.py` & `portage-3.0.48/lib/portage/_sets/libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/profiles.py` & `portage-3.0.48/lib/portage/_sets/profiles.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/security.py` & `portage-3.0.48/lib/portage/_sets/security.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/_sets/shell.py` & `portage-3.0.48/lib/portage/_sets/shell.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/binpkg.py` & `portage-3.0.48/lib/portage/binpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/binrepo/config.py` & `portage-3.0.48/lib/portage/binrepo/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/anydbm.py` & `portage-3.0.48/lib/portage/cache/anydbm.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/cache_errors.py` & `portage-3.0.48/lib/portage/cache/cache_errors.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/ebuild_xattr.py` & `portage-3.0.48/lib/portage/cache/ebuild_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/flat_hash.py` & `portage-3.0.48/lib/portage/cache/flat_hash.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/fs_template.py` & `portage-3.0.48/lib/portage/cache/fs_template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/index/IndexStreamIterator.py` & `portage-3.0.48/lib/portage/cache/index/IndexStreamIterator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/index/pkg_desc_index.py` & `portage-3.0.48/lib/portage/cache/index/pkg_desc_index.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/mappings.py` & `portage-3.0.48/lib/portage/cache/mappings.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/metadata.py` & `portage-3.0.48/lib/portage/cache/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/sql_template.py` & `portage-3.0.48/lib/portage/cache/sql_template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/sqlite.py` & `portage-3.0.48/lib/portage/cache/sqlite.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/template.py` & `portage-3.0.48/lib/portage/cache/template.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cache/volatile.py` & `portage-3.0.48/lib/portage/cache/volatile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/checksum.py` & `portage-3.0.48/lib/portage/checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/const.py` & `portage-3.0.48/lib/portage/const.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/cvstree.py` & `portage-3.0.48/lib/portage/cvstree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/data.py` & `portage-3.0.48/lib/portage/data.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/DummyTree.py` & `portage-3.0.48/lib/portage/dbapi/DummyTree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/IndexedPortdb.py` & `portage-3.0.48/lib/portage/dbapi/IndexedPortdb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/IndexedVardb.py` & `portage-3.0.48/lib/portage/dbapi/IndexedVardb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/_ContentsCaseSensitivityManager.py` & `portage-3.0.48/lib/portage/dbapi/_ContentsCaseSensitivityManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/_MergeProcess.py` & `portage-3.0.48/lib/portage/dbapi/_MergeProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/_SyncfsProcess.py` & `portage-3.0.48/lib/portage/dbapi/_SyncfsProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/_VdbMetadataDelta.py` & `portage-3.0.48/lib/portage/dbapi/_VdbMetadataDelta.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/__init__.py` & `portage-3.0.48/lib/portage/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/_expand_new_virt.py` & `portage-3.0.48/lib/portage/dbapi/_expand_new_virt.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/_similar_name_search.py` & `portage-3.0.48/lib/portage/dbapi/_similar_name_search.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/bintree.py` & `portage-3.0.48/lib/portage/dbapi/bintree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/cpv_expand.py` & `portage-3.0.48/lib/portage/dbapi/cpv_expand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/dep_expand.py` & `portage-3.0.48/lib/portage/dbapi/dep_expand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/porttree.py` & `portage-3.0.48/lib/portage/dbapi/porttree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dbapi/vartree.py` & `portage-3.0.48/lib/portage/dbapi/vartree.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     + "writemsg,writemsg_level,write_atomic,atomic_ofstream,writedict,"
     + "grabdict,normalize_path,new_protect_filename",
     "portage.util._compare_files:compare_files",
     "portage.util.digraph:digraph",
     "portage.util.env_update:env_update",
     "portage.util.install_mask:install_mask_dir,InstallMask,_raise_exc",
     "portage.util.listdir:dircache,listdir",
-    "portage.util.movefile:movefile",
+    "portage.util.movefile:movefile,_cmpxattr",
     "portage.util.path:first_existing,iter_parents",
     "portage.util.writeable_check:get_ro_checker",
     "portage.util._xattr:xattr",
     "portage.util._dyn_libs.PreservedLibsRegistry:PreservedLibsRegistry",
     "portage.util._dyn_libs.LinkageMapELF:LinkageMapELF@LinkageMap",
     "portage.util._dyn_libs.NeededEntry:NeededEntry",
     "portage.util._async.SchedulerInterface:SchedulerInterface",
@@ -89,14 +89,15 @@
 from _emerge.emergelog import emergelog
 from _emerge.MiscFunctionsProcess import MiscFunctionsProcess
 from _emerge.SpawnProcess import SpawnProcess
 from ._ContentsCaseSensitivityManager import ContentsCaseSensitivityManager
 
 import argparse
 import errno
+import filecmp
 import fnmatch
 import functools
 import gc
 import grp
 import io
 from itertools import chain
 import logging
@@ -5539,14 +5540,16 @@
                     myto,
                     mydest,
                     myrealdest,
                     mydmode,
                     destmd5,
                     mydest_link,
                 )
+                if protected and moveme:
+                    mydmode = None
 
             zing = "!!!"
             if not moveme:
                 # confmem rejected this update
                 zing = "---"
 
             if stat.S_ISLNK(mymode):
@@ -5579,14 +5582,15 @@
                         msg.append(
                             _("This symlink will be merged with a different name:")
                         )
                         msg.append(f"  '{newdest}'")
                         msg.append("")
                         self._eerror("preinst", msg)
                         mydest = newdest
+                        mydmode = None
 
                 # if secondhand is None it means we're operating in "force" mode and should not create a second hand.
                 if (secondhand is not None) and (not os.path.exists(myrealto)):
                     # either the target directory doesn't exist yet or the target file doesn't exist -- or
                     # the target is a broken symlink.  We will add this file to our "second hand" and merge
                     # it later.
                     secondhand.append(mysrc[len(srcroot) :])
@@ -5792,40 +5796,51 @@
                     )
                     msg.append(f"  '{mydest}'")
                     msg.append(_("This file will be merged with a different name:"))
                     msg.append(f"  '{newdest}'")
                     msg.append("")
                     self._eerror("preinst", msg)
                     mydest = newdest
+                    mydmode = None
 
                 # whether config protection or not, we merge the new file the
                 # same way.  Unless moveme=0 (blocking directory)
                 if moveme:
-                    # Create hardlinks only for source files that already exist
-                    # as hardlinks (having identical st_dev and st_ino).
-                    hardlink_key = (mystat.st_dev, mystat.st_ino)
-
-                    hardlink_candidates = self._hardlink_merge_map.get(hardlink_key)
-                    if hardlink_candidates is None:
-                        hardlink_candidates = []
-                        self._hardlink_merge_map[hardlink_key] = hardlink_candidates
+                    # only replace the existing file if it differs, see #722270
+                    if self._needs_move(mysrc, mydest, mymode, mydmode):
+                        # Create hardlinks only for source files that already exist
+                        # as hardlinks (having identical st_dev and st_ino).
+                        hardlink_key = (mystat.st_dev, mystat.st_ino)
+
+                        hardlink_candidates = self._hardlink_merge_map.get(hardlink_key)
+                        if hardlink_candidates is None:
+                            hardlink_candidates = []
+                            self._hardlink_merge_map[hardlink_key] = hardlink_candidates
 
-                    mymtime = movefile(
-                        mysrc,
-                        mydest,
-                        newmtime=thismtime,
-                        sstat=mystat,
-                        mysettings=self.settings,
-                        hardlink_candidates=hardlink_candidates,
-                        encoding=_encodings["merge"],
-                    )
-                    if mymtime is None:
-                        return 1
-                    hardlink_candidates.append(mydest)
-                    zing = ">>>"
+                        mymtime = movefile(
+                            mysrc,
+                            mydest,
+                            newmtime=thismtime,
+                            sstat=mystat,
+                            mysettings=self.settings,
+                            hardlink_candidates=hardlink_candidates,
+                            encoding=_encodings["merge"],
+                        )
+                        if mymtime is None:
+                            return 1
+                        hardlink_candidates.append(mydest)
+                        zing = ">>>"
+                    else:
+                        mymtime = thismtime if thismtime is not None else mymtime
+                        try:
+                            os.utime(mydest, ns=(mymtime, mymtime))
+                        except OSError:
+                            # utime can fail here with EPERM
+                            pass
+                        zing = "==="
 
                     try:
                         self._merged_path(mydest, os.lstat(mydest))
                     except OSError:
                         pass
 
                 if mymtime is not None:
@@ -6243,14 +6258,32 @@
             quickpkg_proc.start()
 
             return quickpkg_proc.wait()
 
         finally:
             self.unlockdb()
 
+    def _needs_move(self, mysrc, mydest, mymode, mydmode):
+        """
+        Checks whether the given file at |mysrc| needs to be moved to |mydest| or if
+        they are identical.
+
+        Takes file mode and extended attributes into account.
+        Should only be used for regular files.
+        """
+        if mydmode is None or not stat.S_ISREG(mydmode) or mymode != mydmode:
+            return True
+
+        if "xattr" in self.settings.features:
+            excluded_xattrs = self.settings.get("PORTAGE_XATTR_EXCLUDE", "")
+            if not _cmpxattr(mysrc, mydest, exclude=excluded_xattrs):
+                return True
+
+        return not filecmp.cmp(mysrc, mydest, shallow=False)
+
 
 def merge(
     mycat,
     mypkg,
     pkgloc,
     infloc,
     myroot=None,
```

### Comparing `portage-3.0.47/lib/portage/dbapi/virtual.py` & `portage-3.0.48/lib/portage/dbapi/virtual.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/debug.py` & `portage-3.0.48/lib/portage/debug.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dep/__init__.py` & `portage-3.0.48/lib/portage/dep/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dep/_dnf.py` & `portage-3.0.48/lib/portage/dep/_dnf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dep/_slot_operator.py` & `portage-3.0.48/lib/portage/dep/_slot_operator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dep/dep_check.py` & `portage-3.0.48/lib/portage/dep/dep_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dep/soname/SonameAtom.py` & `portage-3.0.48/lib/portage/dep/soname/SonameAtom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dep/soname/multilib_category.py` & `portage-3.0.48/lib/portage/dep/soname/multilib_category.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dep/soname/parse.py` & `portage-3.0.48/lib/portage/dep/soname/parse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/dispatch_conf.py` & `portage-3.0.48/lib/portage/dispatch_conf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/eapi.py` & `portage-3.0.48/lib/portage/eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/eclass_cache.py` & `portage-3.0.48/lib/portage/eclass_cache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/__init__.py` & `portage-3.0.48/lib/portage/elog/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/filtering.py` & `portage-3.0.48/lib/portage/elog/filtering.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/messages.py` & `portage-3.0.48/lib/portage/elog/messages.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/mod_custom.py` & `portage-3.0.48/lib/portage/elog/mod_custom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/mod_echo.py` & `portage-3.0.48/lib/portage/elog/mod_echo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/mod_mail.py` & `portage-3.0.48/lib/portage/elog/mod_mail.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/mod_mail_summary.py` & `portage-3.0.48/lib/portage/elog/mod_mail_summary.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/mod_save.py` & `portage-3.0.48/lib/portage/elog/mod_save.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/mod_save_summary.py` & `portage-3.0.48/lib/portage/elog/mod_save_summary.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/elog/mod_syslog.py` & `portage-3.0.48/lib/portage/elog/mod_syslog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/defaults.py` & `portage-3.0.48/lib/portage/emaint/defaults.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/main.py` & `portage-3.0.48/lib/portage/emaint/main.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/binhost/__init__.py` & `portage-3.0.48/lib/portage/emaint/modules/binhost/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/binhost/binhost.py` & `portage-3.0.48/lib/portage/emaint/modules/binhost/binhost.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/config/__init__.py` & `portage-3.0.48/lib/portage/emaint/modules/config/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/config/config.py` & `portage-3.0.48/lib/portage/emaint/modules/config/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/logs/__init__.py` & `portage-3.0.48/lib/portage/emaint/modules/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/logs/logs.py` & `portage-3.0.48/lib/portage/emaint/modules/logs/logs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/merges/__init__.py` & `portage-3.0.48/lib/portage/emaint/modules/merges/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/merges/merges.py` & `portage-3.0.48/lib/portage/emaint/modules/merges/merges.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/move/__init__.py` & `portage-3.0.48/lib/portage/emaint/modules/move/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/move/move.py` & `portage-3.0.48/lib/portage/emaint/modules/move/move.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/resume/__init__.py` & `portage-3.0.48/lib/portage/emaint/modules/resume/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/resume/resume.py` & `portage-3.0.48/lib/portage/emaint/modules/resume/resume.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/sync/__init__.py` & `portage-3.0.48/lib/portage/emaint/modules/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/sync/sync.py` & `portage-3.0.48/lib/portage/emaint/modules/sync/sync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/emaint/modules/world/world.py` & `portage-3.0.48/lib/portage/emaint/modules/world/world.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/env/config.py` & `portage-3.0.48/lib/portage/env/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/env/loaders.py` & `portage-3.0.48/lib/portage/env/loaders.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/env/validators.py` & `portage-3.0.48/lib/portage/env/validators.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/exception.py` & `portage-3.0.48/lib/portage/exception.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/getbinpkg.py` & `portage-3.0.48/lib/portage/getbinpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/glsa.py` & `portage-3.0.48/lib/portage/glsa.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/gpg.py` & `portage-3.0.48/lib/portage/gpg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/gpkg.py` & `portage-3.0.48/lib/portage/gpkg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/localization.py` & `portage-3.0.48/lib/portage/localization.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/locks.py` & `portage-3.0.48/lib/portage/locks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/mail.py` & `portage-3.0.48/lib/portage/mail.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/manifest.py` & `portage-3.0.48/lib/portage/manifest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/metadata.py` & `portage-3.0.48/lib/portage/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/module.py` & `portage-3.0.48/lib/portage/module.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/news.py` & `portage-3.0.48/lib/portage/news.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/output.py` & `portage-3.0.48/lib/portage/output.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/KeywordsManager.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/KeywordsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/LicenseManager.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/LicenseManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/LocationsManager.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/LocationsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/MaskManager.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/MaskManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/UseManager.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/UseManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/VirtualsManager.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/VirtualsManager.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/env_var_validation.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/env_var_validation.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/features_set.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/features_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/helper.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/helper.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_config/special_env_vars.py` & `portage-3.0.48/lib/portage/package/ebuild/_config/special_env_vars.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_ipc/ExitCommand.py` & `portage-3.0.48/lib/portage/package/ebuild/_ipc/ExitCommand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_ipc/QueryCommand.py` & `portage-3.0.48/lib/portage/package/ebuild/_ipc/QueryCommand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_metadata_invalid.py` & `portage-3.0.48/lib/portage/package/ebuild/_metadata_invalid.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py` & `portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/ManifestProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py` & `portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/ManifestScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py` & `portage-3.0.48/lib/portage/package/ebuild/_parallel_manifest/ManifestTask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/_spawn_nofetch.py` & `portage-3.0.48/lib/portage/package/ebuild/_spawn_nofetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/config.py` & `portage-3.0.48/lib/portage/package/ebuild/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/deprecated_profile_check.py` & `portage-3.0.48/lib/portage/package/ebuild/deprecated_profile_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/digestcheck.py` & `portage-3.0.48/lib/portage/package/ebuild/digestcheck.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/digestgen.py` & `portage-3.0.48/lib/portage/package/ebuild/digestgen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/doebuild.py` & `portage-3.0.48/lib/portage/package/ebuild/doebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/fetch.py` & `portage-3.0.48/lib/portage/package/ebuild/fetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/getmaskingreason.py` & `portage-3.0.48/lib/portage/package/ebuild/getmaskingreason.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/getmaskingstatus.py` & `portage-3.0.48/lib/portage/package/ebuild/getmaskingstatus.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/prepare_build_dirs.py` & `portage-3.0.48/lib/portage/package/ebuild/prepare_build_dirs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/package/ebuild/profile_iuse.py` & `portage-3.0.48/lib/portage/package/ebuild/profile_iuse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/process.py` & `portage-3.0.48/lib/portage/process.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/progress.py` & `portage-3.0.48/lib/portage/progress.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/proxy/lazyimport.py` & `portage-3.0.48/lib/portage/proxy/lazyimport.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/proxy/objectproxy.py` & `portage-3.0.48/lib/portage/proxy/objectproxy.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/repository/config.py` & `portage-3.0.48/lib/portage/repository/config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/repository/storage/hardlink_quarantine.py` & `portage-3.0.48/lib/portage/repository/storage/hardlink_quarantine.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/repository/storage/hardlink_rcu.py` & `portage-3.0.48/lib/portage/repository/storage/hardlink_rcu.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/repository/storage/inplace.py` & `portage-3.0.48/lib/portage/repository/storage/inplace.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/repository/storage/interface.py` & `portage-3.0.48/lib/portage/repository/storage/interface.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/__init__.py` & `portage-3.0.48/lib/portage/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/config_checks.py` & `portage-3.0.48/lib/portage/sync/config_checks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/controller.py` & `portage-3.0.48/lib/portage/sync/controller.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/getaddrinfo_validate.py` & `portage-3.0.48/lib/portage/sync/getaddrinfo_validate.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/cvs/__init__.py` & `portage-3.0.48/lib/portage/sync/modules/cvs/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/cvs/cvs.py` & `portage-3.0.48/lib/portage/sync/modules/cvs/cvs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/git/__init__.py` & `portage-3.0.48/lib/portage/sync/modules/git/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/git/git.py` & `portage-3.0.48/lib/portage/sync/modules/git/git.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/mercurial/__init__.py` & `portage-3.0.48/lib/portage/sync/modules/mercurial/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/mercurial/mercurial.py` & `portage-3.0.48/lib/portage/sync/modules/mercurial/mercurial.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/rsync/__init__.py` & `portage-3.0.48/lib/portage/sync/modules/rsync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/rsync/rsync.py` & `portage-3.0.48/lib/portage/sync/modules/rsync/rsync.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/svn/__init__.py` & `portage-3.0.48/lib/portage/sync/modules/svn/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/svn/svn.py` & `portage-3.0.48/lib/portage/sync/modules/svn/svn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/modules/webrsync/__init__.py` & `portage-3.0.48/lib/portage/sync/modules/webrsync/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/old_tree_timestamp.py` & `portage-3.0.48/lib/portage/sync/old_tree_timestamp.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/sync/syncbase.py` & `portage-3.0.48/lib/portage/sync/syncbase.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev` & `portage-3.0.48/lib/portage/tests/.gnupg/openpgp-revocs.d/06B3A311BD775C280D22A9305D90EA06352177F6.rev`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev` & `portage-3.0.48/lib/portage/tests/.gnupg/openpgp-revocs.d/8DEDA2CDED49C8809287B89D8812797DDF1DD192.rev`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key` & `portage-3.0.48/lib/portage/tests/.gnupg/private-keys-v1.d/273B030399E7BEA66A9AD42216DE7CA17BA5D42E.key`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key` & `portage-3.0.48/lib/portage/tests/.gnupg/private-keys-v1.d/C99796FB85B0C3DF03314A11B5850C51167D6282.key`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/.gnupg/pubring.kbx` & `portage-3.0.48/lib/portage/tests/.gnupg/pubring.kbx`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/.gnupg/trustdb.gpg` & `portage-3.0.48/lib/portage/tests/.gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/__init__.py` & `portage-3.0.48/lib/portage/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/bin/setup_env.py` & `portage-3.0.48/lib/portage/tests/bin/setup_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/bin/test_dobin.py` & `portage-3.0.48/lib/portage/tests/bin/test_dobin.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/bin/test_dodir.py` & `portage-3.0.48/lib/portage/tests/bin/test_dodir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/bin/test_doins.py` & `portage-3.0.48/lib/portage/tests/bin/test_doins.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/bin/test_eapi7_ver_funcs.py` & `portage-3.0.48/lib/portage/tests/bin/test_eapi7_ver_funcs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/bin/test_filter_bash_env.py` & `portage-3.0.48/lib/portage/tests/bin/test_filter_bash_env.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Gentoo Foundation
+# Copyright 2018-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import difflib
 import os
 import subprocess
 
 import portage
@@ -29,20 +29,18 @@
 declare -x PF="portage-2.3.24"
 declare -a PYTHON_COMPAT=([0]="pypy" [1]="python3_4" [2]="python3_5" [3]="python3_6" [4]="python2_7")
 declare -- _EPATCH_ECLASS="1"
 declare -- _EUTILS_ECLASS="1"
 declare -- f
 get_libdir ()
 {
-    local CONF_LIBDIR;
-    if [ -n "${CONF_LIBDIR_OVERRIDE}" ]; then
-        echo ${CONF_LIBDIR_OVERRIDE};
-    else
-        get_abi_LIBDIR;
-    fi
+    local libdir_var="LIBDIR_${ABI}";
+    local libdir="lib";
+    [[ -n ${ABI} && -n ${!libdir_var} ]] && libdir=${!libdir_var};
+    echo "${libdir}"
 }
 make_wrapper ()
 {
     cat  <<-EOF
 export ${var}="\${${var}}:${EPREFIX}${libdir}"
 EOF
 }
@@ -61,20 +59,18 @@
         ) "
 declare -x PF="portage-2.3.24"
 declare -a PYTHON_COMPAT=([0]="pypy" [1]="python3_4" [2]="python3_5" [3]="python3_6" [4]="python2_7")
 declare -- _EUTILS_ECLASS="1"
 declare -- f
 get_libdir ()
 {
-    local CONF_LIBDIR;
-    if [ -n "${CONF_LIBDIR_OVERRIDE}" ]; then
-        echo ${CONF_LIBDIR_OVERRIDE};
-    else
-        get_abi_LIBDIR;
-    fi
+    local libdir_var="LIBDIR_${ABI}";
+    local libdir="lib";
+    [[ -n ${ABI} && -n ${!libdir_var} ]] && libdir=${!libdir_var};
+    echo "${libdir}"
 }
 make_wrapper ()
 {
     cat  <<-EOF
 export ${var}="\${${var}}:${EPREFIX}${libdir}"
 EOF
 }
```

### Comparing `portage-3.0.47/lib/portage/tests/dbapi/test_auxdb.py` & `portage-3.0.48/lib/portage/tests/dbapi/test_auxdb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dbapi/test_bintree.py` & `portage-3.0.48/lib/portage/tests/dbapi/test_bintree.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dbapi/test_fakedbapi.py` & `portage-3.0.48/lib/portage/tests/dbapi/test_fakedbapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dbapi/test_portdb_cache.py` & `portage-3.0.48/lib/portage/tests/dbapi/test_portdb_cache.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/testAtom.py` & `portage-3.0.48/lib/portage/tests/dep/testAtom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/testCheckRequiredUse.py` & `portage-3.0.48/lib/portage/tests/dep/testCheckRequiredUse.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/testExtendedAtomDict.py` & `portage-3.0.48/lib/portage/tests/dep/testExtendedAtomDict.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/testExtractAffectingUSE.py` & `portage-3.0.48/lib/portage/tests/dep/testExtractAffectingUSE.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/testStandalone.py` & `portage-3.0.48/lib/portage/tests/dep/testStandalone.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_best_match_to_list.py` & `portage-3.0.48/lib/portage/tests/dep/test_best_match_to_list.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_dep_getcpv.py` & `portage-3.0.48/lib/portage/tests/dep/test_dep_getcpv.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_dep_getrepo.py` & `portage-3.0.48/lib/portage/tests/dep/test_dep_getrepo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_dep_getslot.py` & `portage-3.0.48/lib/portage/tests/dep/test_dep_getslot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_dep_getusedeps.py` & `portage-3.0.48/lib/portage/tests/dep/test_dep_getusedeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_dnf_convert.py` & `portage-3.0.48/lib/portage/tests/dep/test_dnf_convert.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_get_operator.py` & `portage-3.0.48/lib/portage/tests/dep/test_get_operator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_get_required_use_flags.py` & `portage-3.0.48/lib/portage/tests/dep/test_get_required_use_flags.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_isjustname.py` & `portage-3.0.48/lib/portage/tests/dep/test_isjustname.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_isvalidatom.py` & `portage-3.0.48/lib/portage/tests/dep/test_isvalidatom.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_match_from_list.py` & `portage-3.0.48/lib/portage/tests/dep/test_match_from_list.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_overlap_dnf.py` & `portage-3.0.48/lib/portage/tests/dep/test_overlap_dnf.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_paren_reduce.py` & `portage-3.0.48/lib/portage/tests/dep/test_paren_reduce.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_soname_atom_pickle.py` & `portage-3.0.48/lib/portage/tests/dep/test_soname_atom_pickle.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/dep/test_use_reduce.py` & `portage-3.0.48/lib/portage/tests/dep/test_use_reduce.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_array_fromfile_eof.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_array_fromfile_eof.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_config.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_config.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_doebuild_fd_pipes.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_doebuild_spawn.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_doebuild_spawn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_fetch.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_fetch.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_ipc_daemon.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_ipc_daemon.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_shell_quote.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_shell_quote.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_spawn.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_spawn.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/ebuild/test_use_expand_incremental.py` & `portage-3.0.48/lib/portage/tests/ebuild/test_use_expand_incremental.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/emerge/test_actions.py` & `portage-3.0.48/lib/portage/tests/emerge/test_actions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/emerge/test_config_protect.py` & `portage-3.0.48/lib/portage/tests/emerge/test_config_protect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014-2015 Gentoo Foundation
+# Copyright 2014-2015, 2023 Gentoo Foundation
 # Distributed under the terms of the GNU General Public License v2
 
 from functools import partial
 import shutil
 import stat
 import subprocess
 import sys
@@ -213,16 +213,16 @@
             "CONFIG_PROTECT": config_protect,
             "DISTDIR": distdir,
             "EMERGE_DEFAULT_OPTS": "-v",
             "EMERGE_WARNING_DELAY": "0",
             "INFODIR": "",
             "INFOPATH": "",
             "PATH": path,
-            "PORTAGE_INST_GID": str(portage.data.portage_gid),
-            "PORTAGE_INST_UID": str(portage.data.portage_uid),
+            "PORTAGE_INST_GID": str(os.getgid()),  # str(portage.data.portage_gid),
+            "PORTAGE_INST_UID": str(os.getuid()),  # str(portage.data.portage_uid),
             "PORTAGE_PYTHON": portage_python,
             "PORTAGE_REPOSITORIES": settings.repositories.config_string(),
             "PORTAGE_TMPDIR": portage_tmpdir,
             "PYTHONDONTWRITEBYTECODE": os.environ.get("PYTHONDONTWRITEBYTECODE", ""),
             "PYTHONPATH": pythonpath,
             "__PORTAGE_TEST_PATH_OVERRIDE": fake_bin,
         }
```

### Comparing `portage-3.0.47/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py` & `portage-3.0.48/lib/portage/tests/emerge/test_emerge_blocker_file_collision.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2016 Gentoo Foundation
+# Copyright 2016, 2023 Gentoo Foundation
 # Distributed under the terms of the GNU General Public License v2
 
 import subprocess
 import sys
 
 import portage
 from portage import os
@@ -117,14 +117,16 @@
         env = {
             "PORTAGE_OVERRIDE_EPREFIX": eprefix,
             "PATH": path,
             "PORTAGE_PYTHON": portage_python,
             "PORTAGE_REPOSITORIES": settings.repositories.config_string(),
             "PYTHONDONTWRITEBYTECODE": os.environ.get("PYTHONDONTWRITEBYTECODE", ""),
             "PYTHONPATH": pythonpath,
+            "PORTAGE_INST_GID": str(os.getgid()),
+            "PORTAGE_INST_UID": str(os.getuid()),
         }
 
         if "__PORTAGE_TEST_HARDLINK_LOCKS" in os.environ:
             env["__PORTAGE_TEST_HARDLINK_LOCKS"] = os.environ[
                 "__PORTAGE_TEST_HARDLINK_LOCKS"
             ]
```

### Comparing `portage-3.0.47/lib/portage/tests/emerge/test_emerge_slot_abi.py` & `portage-3.0.48/lib/portage/tests/emerge/test_emerge_slot_abi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2012-2019 Gentoo Authors
+# Copyright 2012-2019, 2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import subprocess
 import sys
 
 import portage
 from portage import os
@@ -125,14 +125,16 @@
         env = {
             "PORTAGE_OVERRIDE_EPREFIX": eprefix,
             "PATH": path,
             "PORTAGE_PYTHON": portage_python,
             "PORTAGE_REPOSITORIES": settings.repositories.config_string(),
             "PYTHONDONTWRITEBYTECODE": os.environ.get("PYTHONDONTWRITEBYTECODE", ""),
             "PYTHONPATH": pythonpath,
+            "PORTAGE_INST_GID": str(os.getgid()),
+            "PORTAGE_INST_UID": str(os.getuid()),
         }
 
         if "__PORTAGE_TEST_HARDLINK_LOCKS" in os.environ:
             env["__PORTAGE_TEST_HARDLINK_LOCKS"] = os.environ[
                 "__PORTAGE_TEST_HARDLINK_LOCKS"
             ]
```

### Comparing `portage-3.0.47/lib/portage/tests/emerge/test_global_updates.py` & `portage-3.0.48/lib/portage/tests/emerge/test_global_updates.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/emerge/test_simple.py` & `portage-3.0.48/lib/portage/tests/emerge/test_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2011-2021 Gentoo Authors
+# Copyright 2011-2021, 2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import argparse
 import subprocess
 import sys
 
 import portage
@@ -616,16 +616,16 @@
             "CLEAN_DELAY": "0",
             "DISTDIR": distdir,
             "EMERGE_WARNING_DELAY": "0",
             "INFODIR": "",
             "INFOPATH": "",
             "PATH": path,
             "PKGDIR": pkgdir,
-            "PORTAGE_INST_GID": str(portage.data.portage_gid),
-            "PORTAGE_INST_UID": str(portage.data.portage_uid),
+            "PORTAGE_INST_GID": str(os.getgid()),  # str(portage.data.portage_gid),
+            "PORTAGE_INST_UID": str(os.getuid()),  # str(portage.data.portage_uid),
             "PORTAGE_PYTHON": portage_python,
             "PORTAGE_REPOSITORIES": settings.repositories.config_string(),
             "PORTAGE_TMPDIR": portage_tmpdir,
             "PORTAGE_LOGDIR": portage_tmpdir,
             "PYTHONDONTWRITEBYTECODE": os.environ.get("PYTHONDONTWRITEBYTECODE", ""),
             "PYTHONPATH": pythonpath,
             "__PORTAGE_TEST_PATH_OVERRIDE": fake_bin,
```

### Comparing `portage-3.0.47/lib/portage/tests/env/config/test_PackageKeywordsFile.py` & `portage-3.0.48/lib/portage/tests/env/config/test_PackageKeywordsFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/env/config/test_PackageMaskFile.py` & `portage-3.0.48/lib/portage/tests/env/config/test_PackageMaskFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/env/config/test_PackageUseFile.py` & `portage-3.0.48/lib/portage/tests/env/config/test_PackageUseFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/env/config/test_PortageModulesFile.py` & `portage-3.0.48/lib/portage/tests/env/config/test_PortageModulesFile.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/glsa/test_security_set.py` & `portage-3.0.48/lib/portage/tests/glsa/test_security_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_checksum.py` & `portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_gpg.py` & `portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_gpg.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_update.py` & `portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_metadata_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_metadata_url.py` & `portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_metadata_url.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_path.py` & `portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_size.py` & `portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_size.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/gpkg/test_gpkg_stream.py` & `portage-3.0.48/lib/portage/tests/gpkg/test_gpkg_stream.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/lafilefixer/test_lafilefixer.py` & `portage-3.0.48/lib/portage/tests/lafilefixer/test_lafilefixer.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py` & `portage-3.0.48/lib/portage/tests/lazyimport/test_lazy_import_portage_baseline.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/lazyimport/test_preload_portage_submodules.py` & `portage-3.0.48/lib/portage/tests/lazyimport/test_preload_portage_submodules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/lint/test_bash_syntax.py` & `portage-3.0.48/lib/portage/tests/lint/test_bash_syntax.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/lint/test_compile_modules.py` & `portage-3.0.48/lib/portage/tests/lint/test_compile_modules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/lint/test_import_modules.py` & `portage-3.0.48/lib/portage/tests/lint/test_import_modules.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/locks/test_asynchronous_lock.py` & `portage-3.0.48/lib/portage/tests/locks/test_asynchronous_lock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/locks/test_lock_nonblock.py` & `portage-3.0.48/lib/portage/tests/locks/test_lock_nonblock.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/news/test_NewsItem.py` & `portage-3.0.48/lib/portage/tests/news/test_NewsItem.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/process/test_AsyncFunction.py` & `portage-3.0.48/lib/portage/tests/process/test_AsyncFunction.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/process/test_PipeLogger.py` & `portage-3.0.48/lib/portage/tests/process/test_PipeLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/process/test_PopenProcess.py` & `portage-3.0.48/lib/portage/tests/process/test_PopenProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/process/test_PopenProcessBlockingIO.py` & `portage-3.0.48/lib/portage/tests/process/test_PopenProcessBlockingIO.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/process/test_poll.py` & `portage-3.0.48/lib/portage/tests/process/test_poll.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# Copyright 1998-2020 Gentoo Authors
+# Copyright 1998-2020, 2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import functools
 import pty
 import shutil
 import socket
 import tempfile
 
+import pytest
+
 from portage import os
 from portage.tests import TestCase
 from portage.util._eventloop.global_event_loop import global_event_loop
 from portage.util.futures import asyncio
 from _emerge.PipeReader import PipeReader
 
 
@@ -105,14 +107,15 @@
                     f"x = {x}, len(output) = {len(output)}",
                 )
             finally:
                 if cleanup is not None:
                     cleanup()
 
 
+@pytest.mark.xfail()  # This fails sometimes, that's the reason of xfail here
 class PipeReaderArrayTestCase(PipeReaderTestCase):
     _use_array = True
     # sleep allows reliable triggering of the failure mode on fast computers
     _echo_cmd = "sleep 0.1 ; echo -n '%s'"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `portage-3.0.47/lib/portage/tests/process/test_spawn_warn_large_env.py` & `portage-3.0.48/lib/portage/tests/process/test_spawn_warn_large_env.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/ResolverPlayground.py` & `portage-3.0.48/lib/portage/tests/resolver/ResolverPlayground.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py` & `portage-3.0.48/lib/portage/tests/resolver/binpkg_multi_instance/test_build_id_profile_format.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py` & `portage-3.0.48/lib/portage/tests/resolver/binpkg_multi_instance/test_rebuilt_binaries.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_autounmask.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_depclean.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_depclean.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_downgrade.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_or_choices.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_or_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_reinstall.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_reinstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_skip_update.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_skip_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_slot_conflict_reinstall.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_slot_conflict_update.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_slot_conflict_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_soname_provided.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_soname_provided.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfiable.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_unsatisfiable.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/soname/test_unsatisfied.py` & `portage-3.0.48/lib/portage/tests/resolver/soname/test_unsatisfied.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py` & `portage-3.0.48/lib/portage/tests/resolver/test_aggressive_backtrack_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_binpkg_use.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask_binpkg_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_keep_keywords.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask_keep_keywords.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_multilib_use.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask_multilib_use.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Copyright 2013 Gentoo Foundation
+# Copyright 2013, 2023 Gentoo Foundation
 # Distributed under the terms of the GNU General Public License v2
 
+import pytest
+
 from portage.tests import TestCase
 from portage.tests.resolver.ResolverPlayground import (
     ResolverPlayground,
     ResolverPlaygroundTestCase,
 )
 
 
 class AutounmaskMultilibUseTestCase(TestCase):
+    @pytest.mark.xfail()
     def testAutounmaskMultilibUse(self):
         self.todo = True
 
         ebuilds = {
             "x11-proto/xextproto-7.2.1-r1": {
                 "EAPI": "5",
                 "IUSE": "abi_x86_32 abi_x86_64",
```

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_parent.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask_parent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_backtrack.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask_use_backtrack.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_breakage.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask_use_breakage.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py` & `portage-3.0.48/lib/portage/tests/resolver/test_autounmask_use_slot_conflict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# Copyright 2017-2021 Gentoo Authors
+# Copyright 2017-2021, 2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
+import pytest
+
 from portage.tests import TestCase
 from portage.tests.resolver.ResolverPlayground import (
     ResolverPlayground,
     ResolverPlaygroundTestCase,
 )
 
 
 class AutounmaskUseSlotConflictTestCase(TestCase):
+    @pytest.mark.xfail()
     def testAutounmaskUseSlotConflict(self):
         self.todo = True
 
         ebuilds = {
             "sci-libs/K-1": {"IUSE": "+foo", "EAPI": 1},
             "sci-libs/L-1": {"DEPEND": "sci-libs/K[-foo]", "EAPI": 2},
             "sci-libs/M-1": {"DEPEND": "sci-libs/K[foo=]", "IUSE": "+foo", "EAPI": 2},
```

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_backtracking.py` & `portage-3.0.48/lib/portage/tests/resolver/test_backtracking.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_bdeps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_bdeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py` & `portage-3.0.48/lib/portage/tests/resolver/test_binary_pkg_ebuild_visibility.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_blocker.py` & `portage-3.0.48/lib/portage/tests/resolver/test_blocker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_changed_deps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_changed_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_circular_choices.py` & `portage-3.0.48/lib/portage/tests/resolver/test_circular_choices.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_circular_choices_rust.py` & `portage-3.0.48/lib/portage/tests/resolver/test_circular_choices_rust.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_circular_dependencies.py` & `portage-3.0.48/lib/portage/tests/resolver/test_circular_dependencies.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_complete_graph.py` & `portage-3.0.48/lib/portage/tests/resolver/test_complete_graph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py` & `portage-3.0.48/lib/portage/tests/resolver/test_complete_if_new_subslot_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_depclean.py` & `portage-3.0.48/lib/portage/tests/resolver/test_depclean.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_depclean_order.py` & `portage-3.0.48/lib/portage/tests/resolver/test_depclean_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_depclean_slot_unavailable.py` & `portage-3.0.48/lib/portage/tests/resolver/test_depclean_slot_unavailable.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_depth.py` & `portage-3.0.48/lib/portage/tests/resolver/test_depth.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_disjunctive_depend_order.py` & `portage-3.0.48/lib/portage/tests/resolver/test_disjunctive_depend_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_eapi.py` & `portage-3.0.48/lib/portage/tests/resolver/test_eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_features_test_use.py` & `portage-3.0.48/lib/portage/tests/resolver/test_features_test_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py` & `portage-3.0.48/lib/portage/tests/resolver/test_imagemagick_graphicsmagick.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_installkernel.py` & `portage-3.0.48/lib/portage/tests/resolver/test_installkernel.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_keywords.py` & `portage-3.0.48/lib/portage/tests/resolver/test_keywords.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_merge_order.py` & `portage-3.0.48/lib/portage/tests/resolver/test_merge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py` & `portage-3.0.48/lib/portage/tests/resolver/test_missing_iuse_and_evaluated_atoms.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_multirepo.py` & `portage-3.0.48/lib/portage/tests/resolver/test_multirepo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_multislot.py` & `portage-3.0.48/lib/portage/tests/resolver/test_multislot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_old_dep_chain_display.py` & `portage-3.0.48/lib/portage/tests/resolver/test_old_dep_chain_display.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_onlydeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_circular.py` & `portage-3.0.48/lib/portage/tests/resolver/test_onlydeps_circular.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_ideps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_onlydeps_ideps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_onlydeps_minimal.py` & `portage-3.0.48/lib/portage/tests/resolver/test_onlydeps_minimal.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_or_choices.py` & `portage-3.0.48/lib/portage/tests/resolver/test_or_choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# Copyright 2013-2020 Gentoo Authors
+# Copyright 2013-2020, 2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
 import itertools
 
+import pytest
+
 from portage.tests import TestCase
 from portage.tests.resolver.ResolverPlayground import (
     ResolverPlayground,
     ResolverPlaygroundTestCase,
 )
 
 
@@ -633,14 +635,15 @@
                 self.assertEqual(test_case.test_success, True, test_case.fail_msg)
         finally:
             playground.debug = False
             playground.cleanup()
 
 
 class OrChoicesLibpostprocTestCase(TestCase):
+    @pytest.mark.xfail(reason="Irrelevant blocker conflict")
     def testOrChoicesLibpostproc(self):
         # This test case is expected to fail after the fix for bug 706278,
         # since the "undesirable" slot upgrade which triggers a blocker conflict
         # in this test case is practically indistinguishable from a desirable
         # slot upgrade. This particular blocker conflict is no longer relevant,
         # since current versions of media-libs/libpostproc are no longer
         # compatible with any available media-video/ffmpeg slot. In order to
```

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_or_downgrade_installed.py` & `portage-3.0.48/lib/portage/tests/resolver/test_or_downgrade_installed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_or_upgrade_installed.py` & `portage-3.0.48/lib/portage/tests/resolver/test_or_upgrade_installed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_output.py` & `portage-3.0.48/lib/portage/tests/resolver/test_output.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_package_tracker.py` & `portage-3.0.48/lib/portage/tests/resolver/test_package_tracker.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_profile_default_eapi.py` & `portage-3.0.48/lib/portage/tests/resolver/test_profile_default_eapi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_profile_package_set.py` & `portage-3.0.48/lib/portage/tests/resolver/test_profile_package_set.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_rebuild.py` & `portage-3.0.48/lib/portage/tests/resolver/test_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py` & `portage-3.0.48/lib/portage/tests/resolver/test_regular_slot_change_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_required_use.py` & `portage-3.0.48/lib/portage/tests/resolver/test_required_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py` & `portage-3.0.48/lib/portage/tests/resolver/test_runtime_cycle_merge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_simple.py` & `portage-3.0.48/lib/portage/tests/resolver/test_simple.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_abi.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_abi.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_abi_downgrade.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_abi_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_change_without_revbump.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_change_without_revbump.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_collisions.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_collisions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_force_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_mask_update.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_mask_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_rebuild.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_unsatisfied_deep_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_conflict_update_virt.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_conflict_update_virt.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_autounmask.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_autounmask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_bdeps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_bdeps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_complete_graph.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_complete_graph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_exclusive_slots.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_missed_update.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_missed_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_rebuild.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_rebuild.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_required_use.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_required_use.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_reverse_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_runtime_pkg_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_unsatisfied.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_unsolved.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_unsolved.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py` & `portage-3.0.48/lib/portage/tests/resolver/test_slot_operator_update_probe_parent_downgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py` & `portage-3.0.48/lib/portage/tests/resolver/test_solve_non_slot_operator_slot_conflicts.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_targetroot.py` & `portage-3.0.48/lib/portage/tests/resolver/test_targetroot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py` & `portage-3.0.48/lib/portage/tests/resolver/test_unecessary_slot_upgrade.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_unmerge_order.py` & `portage-3.0.48/lib/portage/tests/resolver/test_unmerge_order.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_update.py` & `portage-3.0.48/lib/portage/tests/resolver/test_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_use_dep_defaults.py` & `portage-3.0.48/lib/portage/tests/resolver/test_use_dep_defaults.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_useflags.py` & `portage-3.0.48/lib/portage/tests/resolver/test_useflags.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_virtual_minimize_children.py` & `portage-3.0.48/lib/portage/tests/resolver/test_virtual_minimize_children.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_virtual_slot.py` & `portage-3.0.48/lib/portage/tests/resolver/test_virtual_slot.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/resolver/test_with_test_deps.py` & `portage-3.0.48/lib/portage/tests/resolver/test_with_test_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/runTests.py` & `portage-3.0.48/lib/portage/tests/runTests.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/sets/base/testInternalPackageSet.py` & `portage-3.0.48/lib/portage/tests/sets/base/testInternalPackageSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/sets/base/testVariableSet.py` & `portage-3.0.48/lib/portage/tests/sets/base/testVariableSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/sets/files/testConfigFileSet.py` & `portage-3.0.48/lib/portage/tests/sets/files/testConfigFileSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/sets/files/testStaticFileSet.py` & `portage-3.0.48/lib/portage/tests/sets/files/testStaticFileSet.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/sets/shell/testShell.py` & `portage-3.0.48/lib/portage/tests/sets/shell/testShell.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/sync/test_sync_local.py` & `portage-3.0.48/lib/portage/tests/sync/test_sync_local.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/unicode/test_string_format.py` & `portage-3.0.48/lib/portage/tests/unicode/test_string_format.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/update/test_move_ent.py` & `portage-3.0.48/lib/portage/tests/update/test_move_ent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/update/test_move_slot_ent.py` & `portage-3.0.48/lib/portage/tests/update/test_move_slot_ent.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/update/test_update_dbentry.py` & `portage-3.0.48/lib/portage/tests/update/test_update_dbentry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/dyn_libs/test_soname_deps.py` & `portage-3.0.48/lib/portage/tests/util/dyn_libs/test_soname_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/eventloop/test_call_soon_fifo.py` & `portage-3.0.48/lib/portage/tests/util/eventloop/test_call_soon_fifo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/file_copy/test_copyfile.py` & `portage-3.0.48/lib/portage/tests/util/file_copy/test_copyfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# Copyright 2017 Gentoo Foundation
+# Copyright 2017, 2023 Gentoo Foundation
 # Distributed under the terms of the GNU General Public License v2
 
 import shutil
 import tempfile
 
+import pytest
+
 from portage import os
 from portage.tests import TestCase
 from portage.checksum import perform_md5
 from portage.util.file_copy import copyfile
 
 
 class CopyFileTestCase(TestCase):
@@ -51,15 +53,21 @@
 
             copyfile(src_path, dest_path)
 
             self.assertEqual(perform_md5(src_path), perform_md5(dest_path))
 
             # This last part of the test is expected to fail when sparse
             # copy is not implemented, so set the todo flag in order
-            # to tolerate failures.
-            self.todo = True
+            # to tolerate failures. Or mark it xfail:
+
+            AM_I_UNDER_PYTEST = "PYTEST_CURRENT_TEST" in os.environ
+
+            if AM_I_UNDER_PYTEST:
+                pytest.xfail(reason="sparse copy is not implemented")
+            else:
+                self.todo = True
 
             # If sparse blocks were preserved, then both files should
             # consume the same number of blocks.
             self.assertEqual(os.stat(src_path).st_blocks, os.stat(dest_path).st_blocks)
         finally:
             shutil.rmtree(tempdir)
```

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_child_watcher.py` & `portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_child_watcher.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py` & `portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_event_loop_in_fork.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py` & `portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_pipe_closed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py` & `portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_policy_wrapper_recursion.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py` & `portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_run_until_complete.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py` & `portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_subprocess_exec.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py` & `portage-3.0.48/lib/portage/tests/util/futures/asyncio/test_wakeup_fd_sigchld.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/test_compat_coroutine.py` & `portage-3.0.48/lib/portage/tests/util/futures/test_compat_coroutine.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/test_done_callback.py` & `portage-3.0.48/lib/portage/tests/util/futures/test_done_callback.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/test_done_callback_after_exit.py` & `portage-3.0.48/lib/portage/tests/util/futures/test_done_callback_after_exit.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/test_iter_completed.py` & `portage-3.0.48/lib/portage/tests/util/futures/test_iter_completed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/futures/test_retry.py` & `portage-3.0.48/lib/portage/tests/util/futures/test_retry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_checksum.py` & `portage-3.0.48/lib/portage/tests/util/test_checksum.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_digraph.py` & `portage-3.0.48/lib/portage/tests/util/test_digraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_file_copier.py` & `portage-3.0.48/lib/portage/tests/util/test_file_copier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_getconfig.py` & `portage-3.0.48/lib/portage/tests/util/test_getconfig.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_install_mask.py` & `portage-3.0.48/lib/portage/tests/util/test_install_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_manifest.py` & `portage-3.0.48/lib/portage/tests/util/test_manifest.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_mtimedb.py` & `portage-3.0.48/lib/portage/tests/util/test_mtimedb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_shelve.py` & `portage-3.0.48/lib/portage/tests/util/test_shelve.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_socks5.py` & `portage-3.0.48/lib/portage/tests/util/test_socks5.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_stackDictList.py` & `portage-3.0.48/lib/portage/tests/util/test_stackDictList.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_stackDicts.py` & `portage-3.0.48/lib/portage/tests/util/test_stackDicts.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_stackLists.py` & `portage-3.0.48/lib/portage/tests/util/test_stackLists.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_uniqueArray.py` & `portage-3.0.48/lib/portage/tests/util/test_uniqueArray.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_varExpand.py` & `portage-3.0.48/lib/portage/tests/util/test_varExpand.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/util/test_whirlpool.py` & `portage-3.0.48/lib/portage/tests/util/test_whirlpool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-# Copyright 2011-2022 Gentoo Authors
+# Copyright 2011-2023 Gentoo Authors
 # Distributed under the terms of the GNU General Public License v2
 
+import pytest
+
 from portage.tests import TestCase
 from portage.util.whirlpool import CWhirlpool, PyWhirlpool
 
 
+CWHIRLPOOL_AVAILABLE = CWhirlpool.is_available
+CWHIRLPOOL_NOT_AVAILABLE_MSG = "C Whirlpool extension is not importable"
+
+
 class WhirlpoolTestCase(TestCase):
     def testBundledWhirlpool(self, cls=PyWhirlpool):
         self.assertEqual(
             cls(b"The quick brown fox jumps over the lazy dog").hexdigest(),
             "b97de512e91e3828b40d2b0fdce9ceb3c4a71f9bea8d88e75c4fa854df36725fd2b52eb6544edcacd6f8beddfea403cb55ae31f03ad62a5ef54e42ee82c3fb35",
         )
         self.assertEqual(
@@ -22,11 +28,15 @@
         w = cls()
         w.update(b"")
         self.assertEqual(
             w.hexdigest(),
             "19fa61d75522a4669b44e39c1d2e1726c530232130d407f89afee0964997f7a73e83be698b288febcf88e3e03c4f0757ea8964e59b63d93708b138cc42a66eb3",
         )
 
+    @pytest.mark.skipif(
+        not CWHIRLPOOL_AVAILABLE,
+        reason=CWHIRLPOOL_NOT_AVAILABLE_MSG,
+    )
     def testCWhirlpool(self):
-        if not CWhirlpool.is_available:
-            self.skipTest("C Whirlpool extension is not importable")
+        if not CWHIRLPOOL_AVAILABLE:
+            self.skipTest(CWHIRLPOOL_NOT_AVAILABLE_MSG)
         self.testBundledWhirlpool(CWhirlpool)
```

### Comparing `portage-3.0.47/lib/portage/tests/util/test_xattr.py` & `portage-3.0.48/lib/portage/tests/util/test_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/versions/test_cpv_sort_key.py` & `portage-3.0.48/lib/portage/tests/versions/test_cpv_sort_key.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/tests/versions/test_vercmp.py` & `portage-3.0.48/lib/portage/tests/versions/test_vercmp.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/update.py` & `portage-3.0.48/lib/portage/update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/ExtractKernelVersion.py` & `portage-3.0.48/lib/portage/util/ExtractKernelVersion.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/SlotObject.py` & `portage-3.0.48/lib/portage/util/SlotObject.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/__init__.py` & `portage-3.0.48/lib/portage/util/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/AsyncFunction.py` & `portage-3.0.48/lib/portage/util/_async/AsyncFunction.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/AsyncScheduler.py` & `portage-3.0.48/lib/portage/util/_async/AsyncScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/AsyncTaskFuture.py` & `portage-3.0.48/lib/portage/util/_async/AsyncTaskFuture.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/BuildLogger.py` & `portage-3.0.48/lib/portage/util/_async/BuildLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/FileCopier.py` & `portage-3.0.48/lib/portage/util/_async/FileCopier.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/FileDigester.py` & `portage-3.0.48/lib/portage/util/_async/FileDigester.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/ForkProcess.py` & `portage-3.0.48/lib/portage/util/_async/ForkProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/PipeLogger.py` & `portage-3.0.48/lib/portage/util/_async/PipeLogger.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/PipeReaderBlockingIO.py` & `portage-3.0.48/lib/portage/util/_async/PipeReaderBlockingIO.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/PopenProcess.py` & `portage-3.0.48/lib/portage/util/_async/PopenProcess.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/SchedulerInterface.py` & `portage-3.0.48/lib/portage/util/_async/SchedulerInterface.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/TaskScheduler.py` & `portage-3.0.48/lib/portage/util/_async/TaskScheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_async/run_main_scheduler.py` & `portage-3.0.48/lib/portage/util/_async/run_main_scheduler.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_compare_files.py` & `portage-3.0.48/lib/portage/util/_compare_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_ctypes.py` & `portage-3.0.48/lib/portage/util/_ctypes.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_desktop_entry.py` & `portage-3.0.48/lib/portage/util/_desktop_entry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_dyn_libs/LinkageMapELF.py` & `portage-3.0.48/lib/portage/util/_dyn_libs/LinkageMapELF.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_dyn_libs/NeededEntry.py` & `portage-3.0.48/lib/portage/util/_dyn_libs/NeededEntry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py` & `portage-3.0.48/lib/portage/util/_dyn_libs/PreservedLibsRegistry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_dyn_libs/display_preserved_libs.py` & `portage-3.0.48/lib/portage/util/_dyn_libs/display_preserved_libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_dyn_libs/dyn_libs.py` & `portage-3.0.48/lib/portage/util/_dyn_libs/dyn_libs.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps.py` & `portage-3.0.48/lib/portage/util/_dyn_libs/soname_deps.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_dyn_libs/soname_deps_qa.py` & `portage-3.0.48/lib/portage/util/_dyn_libs/soname_deps_qa.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_eventloop/asyncio_event_loop.py` & `portage-3.0.48/lib/portage/util/_eventloop/asyncio_event_loop.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_get_vm_info.py` & `portage-3.0.48/lib/portage/util/_get_vm_info.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_info_files.py` & `portage-3.0.48/lib/portage/util/_info_files.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_path.py` & `portage-3.0.48/lib/portage/util/_path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_pty.py` & `portage-3.0.48/lib/portage/util/_pty.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_urlopen.py` & `portage-3.0.48/lib/portage/util/_urlopen.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/_xattr.py` & `portage-3.0.48/lib/portage/util/_xattr.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/backoff.py` & `portage-3.0.48/lib/portage/util/backoff.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/bin_entry_point.py` & `portage-3.0.48/lib/portage/util/bin_entry_point.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/changelog.py` & `portage-3.0.48/lib/portage/util/changelog.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/compression_probe.py` & `portage-3.0.48/lib/portage/util/compression_probe.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/configparser.py` & `portage-3.0.48/lib/portage/util/configparser.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/cpuinfo.py` & `portage-3.0.48/lib/portage/util/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/digraph.py` & `portage-3.0.48/lib/portage/util/digraph.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/elf/constants.py` & `portage-3.0.48/lib/portage/util/elf/constants.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/elf/header.py` & `portage-3.0.48/lib/portage/util/elf/header.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/endian/decode.py` & `portage-3.0.48/lib/portage/util/endian/decode.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/env_update.py` & `portage-3.0.48/lib/portage/util/env_update.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/file_copy/__init__.py` & `portage-3.0.48/lib/portage/util/file_copy/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/formatter.py` & `portage-3.0.48/lib/portage/util/formatter.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/_asyncio/__init__.py` & `portage-3.0.48/lib/portage/util/futures/_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/_asyncio/streams.py` & `portage-3.0.48/lib/portage/util/futures/_asyncio/streams.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/_sync_decorator.py` & `portage-3.0.48/lib/portage/util/futures/_sync_decorator.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/compat_coroutine.py` & `portage-3.0.48/lib/portage/util/futures/compat_coroutine.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/executor/fork.py` & `portage-3.0.48/lib/portage/util/futures/executor/fork.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/extendedfutures.py` & `portage-3.0.48/lib/portage/util/futures/extendedfutures.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/futures.py` & `portage-3.0.48/lib/portage/util/futures/futures.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/iter_completed.py` & `portage-3.0.48/lib/portage/util/futures/iter_completed.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/retry.py` & `portage-3.0.48/lib/portage/util/futures/retry.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/futures/unix_events.py` & `portage-3.0.48/lib/portage/util/futures/unix_events.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/hooks.py` & `portage-3.0.48/lib/portage/util/hooks.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/install_mask.py` & `portage-3.0.48/lib/portage/util/install_mask.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/iterators/MultiIterGroupBy.py` & `portage-3.0.48/lib/portage/util/iterators/MultiIterGroupBy.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/lafilefixer.py` & `portage-3.0.48/lib/portage/util/lafilefixer.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/listdir.py` & `portage-3.0.48/lib/portage/util/listdir.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/locale.py` & `portage-3.0.48/lib/portage/util/locale.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/movefile.py` & `portage-3.0.48/lib/portage/util/movefile.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,43 @@
                     "Filesystem containing file '%s' "
                     "does not support extended attribute '%s'"
                 )
                 % (_unicode_decode(dest), _unicode_decode(attr))
             )
 
 
+def _cmpxattr(src, dest, exclude=None):
+    """
+    Compares extended attributes between |src| and |dest| and returns True
+    if they are equal or xattrs are not supported, False otherwise
+    """
+    try:
+        src_attrs = xattr.list(src)
+        dest_attrs = xattr.list(dest)
+    except OSError as e:
+        if e.errno != OperationNotSupported.errno:
+            raise
+        return True
+
+    if src_attrs:
+        if exclude is not None and isinstance(src_attrs[0], bytes):
+            exclude = exclude.encode(_encodings["fs"])
+    exclude = _get_xattr_excluder(exclude)
+
+    src_attrs = {attr for attr in src_attrs if not exclude(attr)}
+    dest_attrs = {attr for attr in dest_attrs if not exclude(attr)}
+    if src_attrs != dest_attrs:
+        return False
+
+    for attr in src_attrs:
+        if xattr.get(src, attr) != xattr.get(dest, attr):
+            return False
+    return True
+
+
 def movefile(
     src,
     dest,
     newmtime=None,
     sstat=None,
     mysettings=None,
     hardlink_candidates=None,
```

### Comparing `portage-3.0.47/lib/portage/util/mtimedb.py` & `portage-3.0.48/lib/portage/util/mtimedb.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/netlink.py` & `portage-3.0.48/lib/portage/util/netlink.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/path.py` & `portage-3.0.48/lib/portage/util/path.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/shelve.py` & `portage-3.0.48/lib/portage/util/shelve.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/socks5.py` & `portage-3.0.48/lib/portage/util/socks5.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/whirlpool.py` & `portage-3.0.48/lib/portage/util/whirlpool.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/util/writeable_check.py` & `portage-3.0.48/lib/portage/util/writeable_check.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/versions.py` & `portage-3.0.48/lib/portage/versions.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/xml/metadata.py` & `portage-3.0.48/lib/portage/xml/metadata.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/lib/portage/xpak.py` & `portage-3.0.48/lib/portage/xpak.py`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/misc/emerge-delta-webrsync` & `portage-3.0.48/misc/emerge-delta-webrsync`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/setup.py` & `portage-3.0.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -727,16 +727,15 @@
         if "__init__.py" in filenames:
             yield os.path.relpath(dirpath, "lib")
 
 
 def find_scripts():
     for dirpath, _dirnames, filenames in os.walk("bin"):
         for f in filenames:
-            if f not in ["deprecated-path"]:
-                yield os.path.join(dirpath, f)
+            yield os.path.join(dirpath, f)
 
 
 def get_manpages():
     linguas = os.environ.get("LINGUAS")
     if linguas is not None:
         linguas = linguas.split()
 
@@ -813,15 +812,15 @@
         return list(venv_data_files(venv_files))
 
     return regular_files
 
 
 setup(
     name="portage",
-    version="3.0.47",
+    version="3.0.48",
     url="https://wiki.gentoo.org/wiki/Project:Portage",
     project_urls={
         "Release Notes": "https://gitweb.gentoo.org/proj/portage.git/plain/NEWS",
         "Documentation": "https://wiki.gentoo.org/wiki/Handbook:AMD64/Working/Portage",
     },
     author="Gentoo Portage Development Team",
     author_email="dev-portage@gentoo.org",
@@ -840,15 +839,14 @@
             ["$logrotatedir", ["cnf/logrotate.d/elog-save-summary"]],
             [
                 "$portage_confdir",
                 ["cnf/make.conf.example", "cnf/make.globals", "cnf/repos.conf"],
             ],
             ["$portage_setsdir", ["cnf/sets/portage.conf"]],
             ["$docdir", ["NEWS", "RELEASE-NOTES"]],
-            ["$portage_base/bin", ["bin/deprecated-path"]],
             ["$portage_confdir/repo.postsync.d", ["cnf/repo.postsync.d/example"]],
         ],
         [
             ("etc", "cnf", ("etc-update.conf", "dispatch-conf.conf")),
             ("etc/logrotate.d", "cnf/logrotate.d", ("elog-save-summary",)),
             (
                 "share/portage/config/repo.postsync.d",
```

### Comparing `portage-3.0.47/src/portage_util__whirlpool.c` & `portage-3.0.48/src/portage_util__whirlpool.c`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/src/portage_util_file_copy_reflink_linux.c` & `portage-3.0.48/src/portage_util_file_copy_reflink_linux.c`

 * *Files identical despite different names*

### Comparing `portage-3.0.47/src/portage_util_libc.c` & `portage-3.0.48/src/portage_util_libc.c`

 * *Files identical despite different names*

