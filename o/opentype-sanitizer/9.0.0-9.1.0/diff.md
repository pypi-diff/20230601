# Comparing `tmp/opentype-sanitizer-9.0.0.tar.gz` & `tmp/opentype-sanitizer-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentype-sanitizer-9.0.0.tar", last modified: Thu Sep 15 14:32:44 2022, max compression
+gzip compressed data, was "opentype-sanitizer-9.1.0.tar", last modified: Wed May 31 23:18:16 2023, max compression
```

## Comparing `opentype-sanitizer-9.0.0.tar` & `opentype-sanitizer-9.1.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     5025 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/config.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/cross-files/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/cross-files/darwin/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/cross-files/darwin/arm64
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/cross-files/darwin/x86_64
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     9371 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/src/c/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.299998 opentype-sanitizer-9.0.0/src/c/ots/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/src/c/ots/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.299998 opentype-sanitizer-9.0.0/src/c/ots/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (121)     2894 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/.github/workflows/ci.yml
--rw-rw-r--   0 runner    (1001) docker     (121)       12 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (121)     1485 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/LICENSE
--rw-rw-r--   0 runner    (1001) docker     (121)     1653 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.299998 opentype-sanitizer-9.0.0/src/c/ots/docs/
--rw-rw-r--   0 runner    (1001) docker     (121)     6883 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/DesignDoc.md
--rw-rw-r--   0 runner    (1001) docker     (121)     1693 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/HowToFix.md
--rw-rw-r--   0 runner    (1001) docker     (121)     7157 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/HowToTest.md
--rw-rw-r--   0 runner    (1001) docker     (121)     1026 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/ots-idempotent.1
--rw-rw-r--   0 runner    (1001) docker     (121)      780 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/ots-perf.1
--rw-rw-r--   0 runner    (1001) docker     (121)     1218 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/ots-sanitize.1
--rw-rw-r--   0 runner    (1001) docker     (121)     4013 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/ots-side-by-side.1
--rw-rw-r--   0 runner    (1001) docker     (121)     1519 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/docs/ots-validator-checker.1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.299998 opentype-sanitizer-9.0.0/src/c/ots/include/
--rw-rw-r--   0 runner    (1001) docker     (121)     5859 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/include/opentype-sanitiser.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2542 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/include/ots-memory-stream.h
--rw-rw-r--   0 runner    (1001) docker     (121)     6106 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/meson.build
--rw-rw-r--   0 runner    (1001) docker     (121)      205 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/meson_options.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/c/ots/src/
--rw-rw-r--   0 runner    (1001) docker     (121)     3511 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/avar.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      958 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/avar.h
--rw-rw-r--   0 runner    (1001) docker     (121)    38813 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cff.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     2231 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cff.h
--rw-rw-r--   0 runner    (1001) docker     (121)    29940 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cff_charstring.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     3143 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cff_charstring.h
--rw-rw-r--   0 runner    (1001) docker     (121)    39062 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cmap.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     2580 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cmap.h
--rw-rw-r--   0 runner    (1001) docker     (121)    36232 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/colr.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      604 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/colr.h
--rw-rw-r--   0 runner    (1001) docker     (121)     9123 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cpal.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      883 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cpal.h
--rw-rw-r--   0 runner    (1001) docker     (121)     1402 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cvar.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      747 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cvar.h
--rw-rw-r--   0 runner    (1001) docker     (121)     1091 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cvt.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      582 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/cvt.h
--rw-rw-r--   0 runner    (1001) docker     (121)     6287 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/feat.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1724 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/feat.h
--rw-rw-r--   0 runner    (1001) docker     (121)     1011 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/fpgm.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      587 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/fpgm.h
--rw-rw-r--   0 runner    (1001) docker     (121)     5523 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/fvar.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1482 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/fvar.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2430 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gasp.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      700 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gasp.h
--rw-rw-r--   0 runner    (1001) docker     (121)    12548 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gdef.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      912 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gdef.h
--rw-rw-r--   0 runner    (1001) docker     (121)    15190 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/glat.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     5548 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/glat.h
--rw-rw-r--   0 runner    (1001) docker     (121)     3440 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gloc.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      824 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gloc.h
--rw-rw-r--   0 runner    (1001) docker     (121)    16722 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/glyf.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1633 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/glyf.h
--rw-rw-r--   0 runner    (1001) docker     (121)    31300 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gpos.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      679 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gpos.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2063 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/graphite.h
--rw-rw-r--   0 runner    (1001) docker     (121)    23772 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gsub.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      698 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gsub.h
--rw-rw-r--   0 runner    (1001) docker     (121)     5154 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gvar.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      747 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/gvar.h
--rw-rw-r--   0 runner    (1001) docker     (121)     3740 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/hdmx.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      778 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/hdmx.h
--rw-rw-r--   0 runner    (1001) docker     (121)     3526 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/head.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      726 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/head.h
--rw-rw-r--   0 runner    (1001) docker     (121)      701 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/hhea.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      527 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/hhea.h
--rw-rw-r--   0 runner    (1001) docker     (121)      506 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/hmtx.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2502 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/hvar.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      747 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/hvar.h
--rw-rw-r--   0 runner    (1001) docker     (121)     5924 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/kern.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1119 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/kern.h
--rw-rw-r--   0 runner    (1001) docker     (121)    64693 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/layout.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     3629 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/layout.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2834 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/loca.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      561 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/loca.h
--rw-rw-r--   0 runner    (1001) docker     (121)     1841 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/ltsh.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      614 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/ltsh.h
--rw-rw-r--   0 runner    (1001) docker     (121)    18398 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/math.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     2813 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/math_.h
--rw-rw-r--   0 runner    (1001) docker     (121)     3029 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/maxp.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      882 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/maxp.h
--rw-rw-r--   0 runner    (1001) docker     (121)     5342 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/metrics.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1319 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/metrics.h
--rw-rw-r--   0 runner    (1001) docker     (121)     3346 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/mvar.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      747 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/mvar.h
--rw-rw-r--   0 runner    (1001) docker     (121)    11385 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/name.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1581 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/name.h
--rw-rw-r--   0 runner    (1001) docker     (121)    11105 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/os2.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1577 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/os2.h
--rw-rw-r--   0 runner    (1001) docker     (121)    37195 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/ots.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     9967 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/ots.h
--rw-rw-r--   0 runner    (1001) docker     (121)     5605 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/post.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      771 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/post.h
--rw-rw-r--   0 runner    (1001) docker     (121)     1064 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/prep.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      591 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/prep.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2246 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/sile.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      775 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/sile.h
--rw-rw-r--   0 runner    (1001) docker     (121)    35559 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/silf.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     6351 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/silf.h
--rw-rw-r--   0 runner    (1001) docker     (121)     5229 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/sill.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1382 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/sill.h
--rw-rw-r--   0 runner    (1001) docker     (121)    11730 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/stat.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     3596 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/stat.h
--rw-rw-r--   0 runner    (1001) docker     (121)     8508 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/variations.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      828 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/variations.h
--rw-rw-r--   0 runner    (1001) docker     (121)     4811 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vdmx.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1094 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vdmx.h
--rw-rw-r--   0 runner    (1001) docker     (121)      736 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vhea.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      528 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vhea.h
--rw-rw-r--   0 runner    (1001) docker     (121)      508 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vmtx.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2358 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vorg.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      775 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vorg.h
--rw-rw-r--   0 runner    (1001) docker     (121)     2849 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vvar.cc
--rw-rw-r--   0 runner    (1001) docker     (121)      747 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/src/vvar.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/c/ots/subprojects/
--rw-rw-r--   0 runner    (1001) docker     (121)       27 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (121)      311 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/freetype2.wrap
--rw-rw-r--   0 runner    (1001) docker     (121)      536 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/google-brotli.wrap
--rw-rw-r--   0 runner    (1001) docker     (121)      588 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/google-woff2.wrap
--rw-rw-r--   0 runner    (1001) docker     (121)      541 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/gtest.wrap
--rw-rw-r--   0 runner    (1001) docker     (121)      447 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/lz4.wrap
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/brotli/
--rw-rw-r--   0 runner    (1001) docker     (121)     1070 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/brotli/LICENSE.build
--rw-rw-r--   0 runner    (1001) docker     (121)     3321 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/brotli/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/woff2/
--rw-rw-r--   0 runner    (1001) docker     (121)     1105 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/woff2/LICENSE.build
--rw-rw-r--   0 runner    (1001) docker     (121)     3875 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/woff2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (121)      162 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/woff2/meson_options.txt
--rw-rw-r--   0 runner    (1001) docker     (121)      424 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/subprojects/zlib.wrap
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/c/ots/tests/
--rw-rw-r--   0 runner    (1001) docker     (121)    45037 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/tests/cff_charstring_test.cc
--rw-rw-r--   0 runner    (1001) docker     (121)    22362 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/tests/layout_common_table_test.cc
--rw-rw-r--   0 runner    (1001) docker     (121)    26145 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/tests/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/c/ots/util/
--rw-rw-r--   0 runner    (1001) docker     (121)     1579 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/util/ots-fuzzer.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     5100 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/util/ots-idempotent.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     2036 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/util/ots-perf.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     2844 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/util/ots-sanitize.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     7684 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/util/ots-side-by-side.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     4646 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/util/ots-validator-checker.cc
--rw-rw-r--   0 runner    (1001) docker     (121)     1108 2022-09-15 13:24:32.000000 opentype-sanitizer-9.0.0/src/c/ots/util/test-context.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.295998 opentype-sanitizer-9.0.0/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-09-15 14:32:44.000000 opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2022-09-15 14:32:44.000000 opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 14:32:44.000000 opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 14:32:44.000000 opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-09-15 14:32:44.000000 opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-15 14:32:44.000000 opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/src/python/ots/
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/src/python/ots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/src/python/ots/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-15 14:32:38.000000 opentype-sanitizer-9.0.0/src/python/ots/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 14:32:44.307998 opentype-sanitizer-9.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/tests/test_ots.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-09-15 14:32:27.000000 opentype-sanitizer-9.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.327554 opentype-sanitizer-9.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.291554 opentype-sanitizer-9.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.295554 opentype-sanitizer-9.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-31 23:18:16.327554 opentype-sanitizer-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5025 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/config.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.291554 opentype-sanitizer-9.1.0/cross-files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.295554 opentype-sanitizer-9.1.0/cross-files/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/cross-files/darwin/arm64
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/cross-files/darwin/x86_64
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-31 23:18:16.327554 opentype-sanitizer-9.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9371 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.291554 opentype-sanitizer-9.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.291554 opentype-sanitizer-9.1.0/src/c/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.295554 opentype-sanitizer-9.1.0/src/c/ots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.291554 opentype-sanitizer-9.1.0/src/c/ots/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.295554 opentype-sanitizer-9.1.0/src/c/ots/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2894 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/.github/workflows/ci.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      691 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/.github/workflows/cifuzz.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)       12 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)     1485 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (123)     1653 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.299554 opentype-sanitizer-9.1.0/src/c/ots/docs/
+-rw-rw-r--   0 runner    (1001) docker     (123)     6883 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/DesignDoc.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1693 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/HowToFix.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     7157 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/HowToTest.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1026 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/ots-idempotent.1
+-rw-rw-r--   0 runner    (1001) docker     (123)      780 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/ots-perf.1
+-rw-rw-r--   0 runner    (1001) docker     (123)     1218 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/ots-sanitize.1
+-rw-rw-r--   0 runner    (1001) docker     (123)     4013 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/ots-side-by-side.1
+-rw-rw-r--   0 runner    (1001) docker     (123)     1519 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/docs/ots-validator-checker.1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.299554 opentype-sanitizer-9.1.0/src/c/ots/include/
+-rw-rw-r--   0 runner    (1001) docker     (123)     5859 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/include/opentype-sanitiser.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2542 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/include/ots-memory-stream.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     5911 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)      324 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/meson_options.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.319554 opentype-sanitizer-9.1.0/src/c/ots/src/
+-rw-rw-r--   0 runner    (1001) docker     (123)     5054 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/avar.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1036 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/avar.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    38813 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cff.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     2231 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cff.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    29942 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cff_charstring.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     3143 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cff_charstring.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    39062 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cmap.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     2580 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cmap.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    36232 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/colr.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      604 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/colr.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     9145 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cpal.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      883 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cpal.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     1402 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cvar.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      747 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cvar.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     1091 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cvt.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      582 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/cvt.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     6287 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/feat.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1724 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/feat.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     1011 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/fpgm.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      587 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/fpgm.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     5523 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/fvar.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1482 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/fvar.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2430 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gasp.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      700 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gasp.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    12548 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gdef.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      912 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gdef.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    15190 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/glat.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     5548 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/glat.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     3440 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gloc.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      824 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gloc.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    16722 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/glyf.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1633 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/glyf.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    26036 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gpos.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1161 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gpos.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2063 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/graphite.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    18219 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gsub.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1122 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gsub.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     6796 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gvar.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      933 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/gvar.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     3740 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/hdmx.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      778 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/hdmx.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     3526 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/head.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      726 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/head.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      701 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/hhea.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      527 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/hhea.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      506 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/hmtx.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2502 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/hvar.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      747 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/hvar.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     5924 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/kern.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1119 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/kern.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    65312 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/layout.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     2345 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/layout.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2834 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/loca.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      561 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/loca.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     1841 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/ltsh.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      614 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/ltsh.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    18398 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/math.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     2813 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/math_.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     3029 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/maxp.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      882 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/maxp.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     5342 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/metrics.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1319 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/metrics.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     3346 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/mvar.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      747 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/mvar.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    11385 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/name.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1581 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/name.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    11105 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/os2.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1577 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/os2.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    38356 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/ots.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)    10193 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/ots.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     5605 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/post.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      771 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/post.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     1064 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/prep.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      591 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/prep.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2246 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/sile.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      775 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/sile.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    35559 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/silf.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     6351 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/silf.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     5229 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/sill.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1382 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/sill.h
+-rw-rw-r--   0 runner    (1001) docker     (123)    11730 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/stat.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     3596 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/stat.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     8508 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/variations.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      828 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/variations.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     5403 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vdmx.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1094 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vdmx.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      736 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vhea.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      528 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vhea.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      508 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vmtx.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2358 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vorg.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      775 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vorg.h
+-rw-rw-r--   0 runner    (1001) docker     (123)     2849 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vvar.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)      747 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/src/vvar.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.319554 opentype-sanitizer-9.1.0/src/c/ots/subprojects/
+-rw-rw-r--   0 runner    (1001) docker     (123)       27 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)      311 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/freetype2.wrap
+-rw-rw-r--   0 runner    (1001) docker     (123)      536 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/google-brotli.wrap
+-rw-rw-r--   0 runner    (1001) docker     (123)      588 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/google-woff2.wrap
+-rw-rw-r--   0 runner    (1001) docker     (123)      541 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/gtest.wrap
+-rw-rw-r--   0 runner    (1001) docker     (123)      447 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/lz4.wrap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.291554 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.323554 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/brotli/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1070 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/brotli/LICENSE.build
+-rw-rw-r--   0 runner    (1001) docker     (123)     3321 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/brotli/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.323554 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/woff2/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1105 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/woff2/LICENSE.build
+-rw-rw-r--   0 runner    (1001) docker     (123)     3875 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/woff2/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)      162 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/woff2/meson_options.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      424 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/subprojects/zlib.wrap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.323554 opentype-sanitizer-9.1.0/src/c/ots/tests/
+-rw-rw-r--   0 runner    (1001) docker     (123)    45037 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/tests/cff_charstring_test.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)    26267 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/tests/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.323554 opentype-sanitizer-9.1.0/src/c/ots/util/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1579 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/util/ots-fuzzer.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     5100 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/util/ots-idempotent.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     2036 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/util/ots-perf.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     2844 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/util/ots-sanitize.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     7684 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/util/ots-side-by-side.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     4646 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/util/ots-validator-checker.cc
+-rw-rw-r--   0 runner    (1001) docker     (123)     1108 2023-05-29 21:44:20.000000 opentype-sanitizer-9.1.0/src/c/ots/util/test-context.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.291554 opentype-sanitizer-9.1.0/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.323554 opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-31 23:18:16.000000 opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-31 23:18:16.000000 opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:18:16.000000 opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:18:16.000000 opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 23:18:16.000000 opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 23:18:16.000000 opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.327554 opentype-sanitizer-9.1.0/src/python/ots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/src/python/ots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/src/python/ots/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 23:18:08.000000 opentype-sanitizer-9.1.0/src/python/ots/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:18:16.327554 opentype-sanitizer-9.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/tests/test_ots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-31 23:17:56.000000 opentype-sanitizer-9.1.0/tox.ini
```

### Comparing `opentype-sanitizer-9.0.0/.github/workflows/ci.yml` & `opentype-sanitizer-9.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/.gitignore` & `opentype-sanitizer-9.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/LICENSE` & `opentype-sanitizer-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/PKG-INFO` & `opentype-sanitizer-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentype-sanitizer
-Version: 9.0.0
+Version: 9.1.0
 Summary: Python wrapper for the OpenType Sanitizer
 Home-page: https://github.com/googlefonts/ots-python
 Author: Cosimo Lupo
 Author-email: cosimo@anthrotype.com
 License: OpenSource, BSD-style
 Platform: posix
 Platform: nt
```

### Comparing `opentype-sanitizer-9.0.0/build.py` & `opentype-sanitizer-9.1.0/build.py`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/config.sh` & `opentype-sanitizer-9.1.0/config.sh`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/setup.py` & `opentype-sanitizer-9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/.github/workflows/ci.yml` & `opentype-sanitizer-9.1.0/src/c/ots/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/LICENSE` & `opentype-sanitizer-9.1.0/src/c/ots/LICENSE`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/README.md` & `opentype-sanitizer-9.1.0/src/c/ots/README.md`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/DesignDoc.md` & `opentype-sanitizer-9.1.0/src/c/ots/docs/DesignDoc.md`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/HowToFix.md` & `opentype-sanitizer-9.1.0/src/c/ots/docs/HowToFix.md`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/HowToTest.md` & `opentype-sanitizer-9.1.0/src/c/ots/docs/HowToTest.md`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/ots-idempotent.1` & `opentype-sanitizer-9.1.0/src/c/ots/docs/ots-idempotent.1`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/ots-perf.1` & `opentype-sanitizer-9.1.0/src/c/ots/docs/ots-perf.1`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/ots-sanitize.1` & `opentype-sanitizer-9.1.0/src/c/ots/docs/ots-sanitize.1`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/ots-side-by-side.1` & `opentype-sanitizer-9.1.0/src/c/ots/docs/ots-side-by-side.1`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/docs/ots-validator-checker.1` & `opentype-sanitizer-9.1.0/src/c/ots/docs/ots-validator-checker.1`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/include/opentype-sanitiser.h` & `opentype-sanitizer-9.1.0/src/c/ots/include/opentype-sanitiser.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/include/ots-memory-stream.h` & `opentype-sanitizer-9.1.0/src/c/ots/include/ots-memory-stream.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/meson.build` & `opentype-sanitizer-9.1.0/src/c/ots/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('ots', 'c', 'cpp',
-  version: '9.0.0',
+  version: '9.1.0',
   default_options : ['cpp_std=c++11', 'default_library=static', 'warning_level=2'],
   meson_version : '>= 0.55.2',
 )
 
 subdir('tests')
 
 cxx = meson.get_compiler('cpp')
@@ -16,14 +16,18 @@
   conf.set('OTS_DEBUG', 1)
 endif
 
 if get_option('graphite')
   conf.set('OTS_GRAPHITE', 1)
 endif
 
+if get_option('synthesize-gvar')
+  conf.set('OTS_SYNTHESIZE_MISSING_GVAR', 1)
+endif
+
 freetype = dependency('freetype2', required: false)
 if freetype.found()
   conf.set('HAVE_FREETYPE', 1)
 endif
 
 coretext = dependency('appleframeworks', modules: 'applicationservices',
                       required: false)
@@ -256,26 +260,14 @@
   link_with: libots,
   dependencies: gtest,
 )
 
 test('cff_charstring', cff_charstring)
 
 
-layout_common_table = executable('layout_common_table',
-  'tests/layout_common_table_test.cc',
-  include_directories: include_directories(['include', 'src']),
-  link_with: libots,
-  dependencies: gtest,
-)
-
-test('layout_common_table', layout_common_table,
-  protocol: 'gtest',
-)
-
-
 foreach file_name : bad_fonts
   test(file_name, ots_sanitize,
     args: meson.current_source_dir() / 'tests' / file_name,
     suite: 'bad',
     should_fail: true,
   )
 endforeach
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/avar.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/avar.cc`

 * *Files 27% similar despite different names*

```diff
@@ -2,39 +2,52 @@
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
 #include "avar.h"
 
 #include "fvar.h"
 
+#include "variations.h"
+
 namespace ots {
 
 // -----------------------------------------------------------------------------
 // OpenTypeAVAR
 // -----------------------------------------------------------------------------
 
 bool OpenTypeAVAR::Parse(const uint8_t* data, size_t length) {
   Buffer table(data, length);
   if (!table.ReadU16(&this->majorVersion) ||
       !table.ReadU16(&this->minorVersion) ||
       !table.ReadU16(&this->reserved) ||
       !table.ReadU16(&this->axisCount)) {
     return Drop("Failed to read table header");
   }
-  if (this->majorVersion != 1) {
+  if (this->majorVersion > 2) {
     return Drop("Unknown table version");
   }
-  if (this->minorVersion > 0) {
-    // we only know how to serialize version 1.0
-    Warning("Downgrading minor version to 0");
-    this->minorVersion = 0;
-  }
-  if (this->reserved != 0) {
-    Warning("Expected reserved=0");
-    this->reserved = 0;
+  if (this->majorVersion == 1) {
+    // We can fix table
+    if (this->minorVersion > 0) {
+      // we only know how to serialize version 1.0
+      Warning("Downgrading minor version to 0");
+      this->minorVersion = 0;
+    }
+    if (this->reserved != 0) {
+      Warning("Expected reserved=0");
+      this->reserved = 0;
+    }
+  } else {
+    // We serialize data unchanged, so drop even for minor errors
+    if (this->minorVersion > 0) {
+      return Drop("Unknown minor table version");
+    }
+    if (this->reserved != 0) {
+      return Drop("Expected reserved=0");
+    }
   }
 
   OpenTypeFVAR* fvar = static_cast<OpenTypeFVAR*>(
       GetFont()->GetTypedTable(OTS_TAG_FVAR));
   if (!fvar) {
     return DropVariations("Required fvar table is missing");
   }
@@ -75,18 +88,60 @@
       this->axisSegmentMaps[i].push_back(map);
     }
     if (positionMapCount > 0 && foundRequiredMappings != 3) {
       return Drop("A required mapping (for -1, 0 or 1) is missing");
     }
   }
 
+  if (this->majorVersion < 2)
+    return true;
+
+  uint32_t axisIndexMapOffset;
+  uint32_t varStoreOffset;
+
+  if (!table.ReadU32(&axisIndexMapOffset) ||
+      !table.ReadU32(&varStoreOffset)) {
+    return Drop("Failed to read version 2 offsets");
+  }
+
+  Font *font = GetFont();
+  uint32_t headerSize = table.offset();
+
+  if (axisIndexMapOffset) {
+    if (axisIndexMapOffset < headerSize || axisIndexMapOffset >= length) {
+      return Drop("Bad delta set index offset in table header");
+    }
+    if (!ParseDeltaSetIndexMap(font, data + axisIndexMapOffset, length - axisIndexMapOffset)) {
+      return Drop("Failed to parse delta set index map");
+    }
+  }
+
+  if (varStoreOffset) {
+    if (varStoreOffset < headerSize || varStoreOffset >= length) {
+      return Drop("Bad item variation store offset in table header");
+    }
+    if (!ParseItemVariationStore(font, data + varStoreOffset, length - varStoreOffset)) {
+      return Drop("Failed to parse item variation store");
+    }
+  }
+
+  this->m_data = data;
+  this->m_length = length;
+
   return true;
 }
 
 bool OpenTypeAVAR::Serialize(OTSStream* out) {
+  if (this->majorVersion >= 2) {
+    if (!out->Write(this->m_data, this->m_length)) {
+      return Error("Failed to write table");
+    }
+    return true;
+  }
+
   if (!out->WriteU16(this->majorVersion) ||
       !out->WriteU16(this->minorVersion) ||
       !out->WriteU16(this->reserved) ||
       !out->WriteU16(this->axisCount)) {
     return Error("Failed to write table");
   }
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/avar.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/avar.h`

 * *Files 26% similar despite different names*

```diff
@@ -31,12 +31,16 @@
 
   struct AxisValueMap {
     int16_t fromCoordinate;
     int16_t toCoordinate;
   };
 
   std::vector<std::vector<AxisValueMap>> axisSegmentMaps;
+
+  // Only used for versions >= 2
+  const uint8_t *m_data;
+  size_t m_length;
 };
 
 }  // namespace ots
 
 #endif  // OTS_AVAR_H_
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cff.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/cff.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cff.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/cff.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cff_charstring.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/cff_charstring.cc`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
       return OTS_FAILURE();
     }
     if (cs_ctx.vsindex >= (int32_t)cff.region_index_count.size()) {
       return OTS_FAILURE();
     }
     uint16_t k = cff.region_index_count.at(cs_ctx.vsindex);
     uint16_t n = argument_stack->top();
-    if (stack_size < n * (k + 1) + 1) {
+    if (stack_size < n * (k + 1u) + 1u) {
       return OTS_FAILURE();
     }
 
     // Keep the 1st n operands on the stack for the next operator to use and
     // pop the rest. There can be multiple consecutive blend operators, so this
     // makes sure the operands of all of them are kept on the stack.
     while (argument_stack->size() > stack_size - ((n * k) + 1))
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cff_charstring.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/cff_charstring.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cmap.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/cmap.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cmap.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/cmap.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/colr.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/colr.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/colr.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/colr.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cpal.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/cpal.cc`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,17 @@
   return true;
 }
 
 bool OpenTypeCPAL::Serialize(OTSStream *out) {
   uint16_t numPalettes = this->colorRecordIndices.size();
   uint16_t numColorRecords = this->colorRecords.size();
 
+#ifndef NDEBUG
   off_t start = out->Tell();
+#endif
 
   size_t colorRecordsArrayOffset = 4 * sizeof(uint16_t) + sizeof(uint32_t) +
       numPalettes * sizeof(uint16_t);
   if (this->version == 1) {
     colorRecordsArrayOffset += 3 * sizeof(uint32_t);
   }
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cpal.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/cpal.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cvar.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/cvar.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cvar.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/cvar.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cvt.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/cvt.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/cvt.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/cvt.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/feat.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/feat.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/feat.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/feat.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/fpgm.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/fpgm.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/fpgm.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/fpgm.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/fvar.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/fvar.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/fvar.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/fvar.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gasp.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/gasp.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gasp.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/gasp.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gdef.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/gdef.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gdef.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/gdef.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/glat.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/glat.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/glat.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/glat.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gloc.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/gloc.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gloc.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/gloc.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/glyf.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/glyf.cc`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -108,17 +108,17 @@
   uint16_t bytecode_length = 0;
   if (!glyph.ReadU16(&bytecode_length)) {
     return Error("Can't read bytecode length");
   }
 
   if (this->maxp->version_1 &&
       this->maxp->max_size_glyf_instructions < bytecode_length) {
-    this->maxp->max_size_glyf_instructions = bytecode_length;
     Warning("Bytecode length is bigger than maxp.maxSizeOfInstructions %d: %d",
             this->maxp->max_size_glyf_instructions, bytecode_length);
+    this->maxp->max_size_glyf_instructions = bytecode_length;
   }
 
   if (!glyph.Skip(bytecode_length)) {
     return Error("Can't read bytecode of length %d", bytecode_length);
   }
 
   uint32_t coordinates_length = 0;
@@ -211,18 +211,18 @@
     uint16_t bytecode_length;
     if (!glyph.ReadU16(&bytecode_length)) {
       return Error("Can't read instructions size");
     }
 
     if (this->maxp->version_1 &&
         this->maxp->max_size_glyf_instructions < bytecode_length) {
-      this->maxp->max_size_glyf_instructions = bytecode_length;
       Warning("Bytecode length is bigger than maxp.maxSizeOfInstructions "
               "%d: %d",
               this->maxp->max_size_glyf_instructions, bytecode_length);
+      this->maxp->max_size_glyf_instructions = bytecode_length;
     }
 
     if (!glyph.Skip(bytecode_length)) {
       return Error("Can't read bytecode of length %d", bytecode_length);
     }
   }
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/glyf.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/glyf.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gpos.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/gpos.cc`

 * *Files 20% similar despite different names*

```diff
@@ -26,58 +26,17 @@
   GPOS_TYPE_MARK_TO_MARK_ATTACHMENT = 6,
   GPOS_TYPE_CONTEXT_POSITIONING = 7,
   GPOS_TYPE_CHAINED_CONTEXT_POSITIONING = 8,
   GPOS_TYPE_EXTENSION_POSITIONING = 9,
   GPOS_TYPE_RESERVED = 10
 };
 
-// The size of gpos header, version 1.0.
-const unsigned kGposHeaderSize_1_0 = 10;
-// The size of gpos header, version 1.1.
-const unsigned kGposHeaderSize_1_1 = 14;
 // The maximum format number for anchor tables.
 const uint16_t kMaxAnchorFormat = 3;
 
-// Lookup type parsers.
-bool ParseSingleAdjustment(const ots::Font *font,
-                           const uint8_t *data, const size_t length);
-bool ParsePairAdjustment(const ots::Font *font,
-                         const uint8_t *data, const size_t length);
-bool ParseCursiveAttachment(const ots::Font *font,
-                            const uint8_t *data, const size_t length);
-bool ParseMarkToBaseAttachment(const ots::Font *font,
-                               const uint8_t *data, const size_t length);
-bool ParseMarkToLigatureAttachment(const ots::Font *font,
-                                   const uint8_t *data, const size_t length);
-bool ParseMarkToMarkAttachment(const ots::Font *font,
-                               const uint8_t *data, const size_t length);
-bool ParseContextPositioning(const ots::Font *font,
-                             const uint8_t *data, const size_t length);
-bool ParseChainedContextPositioning(const ots::Font *font,
-                                    const uint8_t *data, const size_t length);
-bool ParseExtensionPositioning(const ots::Font *font,
-                               const uint8_t *data, const size_t length);
-
-const ots::LookupSubtableParser::TypeParser kGposTypeParsers[] = {
-  {GPOS_TYPE_SINGLE_ADJUSTMENT, ParseSingleAdjustment},
-  {GPOS_TYPE_PAIR_ADJUSTMENT, ParsePairAdjustment},
-  {GPOS_TYPE_CURSIVE_ATTACHMENT, ParseCursiveAttachment},
-  {GPOS_TYPE_MARK_TO_BASE_ATTACHMENT, ParseMarkToBaseAttachment},
-  {GPOS_TYPE_MARK_TO_LIGATURE_ATTACHMENT, ParseMarkToLigatureAttachment},
-  {GPOS_TYPE_MARK_TO_MARK_ATTACHMENT, ParseMarkToMarkAttachment},
-  {GPOS_TYPE_CONTEXT_POSITIONING, ParseContextPositioning},
-  {GPOS_TYPE_CHAINED_CONTEXT_POSITIONING, ParseChainedContextPositioning},
-  {GPOS_TYPE_EXTENSION_POSITIONING, ParseExtensionPositioning}
-};
-
-const ots::LookupSubtableParser kGposLookupSubtableParser = {
-  arraysize(kGposTypeParsers),
-  GPOS_TYPE_EXTENSION_POSITIONING, kGposTypeParsers
-};
-
 // Shared Tables: ValueRecord, Anchor Table, and MarkArray
 
 size_t CalcValueRecordSize(const uint16_t value_format) {
   size_t size = 0;
   for (unsigned i = 0; i < 8; ++i) {
     if ((value_format >> i) & 0x1) {
       size += 2;
@@ -210,67 +169,14 @@
       return OTS_FAILURE_MSG("Faled to parse anchor table for mark table %d", i);
     }
   }
 
   return true;
 }
 
-// Lookup Type 1:
-// Single Adjustment Positioning Subtable
-bool ParseSingleAdjustment(const ots::Font *font, const uint8_t *data,
-                           const size_t length) {
-  ots::Buffer subtable(data, length);
-
-  ots::OpenTypeMAXP *maxp = static_cast<ots::OpenTypeMAXP*>(
-      font->GetTypedTable(OTS_TAG_MAXP));
-  if (!maxp) {
-    return OTS_FAILURE_MSG("Required maxp table missing");
-  }
-
-  uint16_t format = 0;
-  uint16_t offset_coverage = 0;
-  uint16_t value_format = 0;
-  if (!subtable.ReadU16(&format) ||
-      !subtable.ReadU16(&offset_coverage) ||
-      !subtable.ReadU16(&value_format)) {
-    return OTS_FAILURE_MSG("Can't read single adjustment information");
-  }
-
-  if (format == 1) {
-    // Format 1 exactly one value record.
-    if (!ParseValueRecord(font, &subtable, value_format)) {
-      return OTS_FAILURE_MSG("Failed to parse format 1 single adjustment table");
-    }
-  } else if (format == 2) {
-    uint16_t value_count = 0;
-    if (!subtable.ReadU16(&value_count)) {
-      return OTS_FAILURE_MSG("Failed to parse format 2 single adjustment table");
-    }
-    for (unsigned i = 0; i < value_count; ++i) {
-      if (!ParseValueRecord(font, &subtable, value_format)) {
-        return OTS_FAILURE_MSG("Failed to parse value record %d in format 2 single adjustment table", i);
-      }
-    }
-  } else {
-    return OTS_FAILURE_MSG("Bad format %d in single adjustment table", format);
-  }
-
-  if (offset_coverage < subtable.offset() || offset_coverage >= length) {
-    return OTS_FAILURE_MSG("Bad coverage offset %d in single adjustment table", offset_coverage);
-  }
-
-  if (!ots::ParseCoverageTable(font, data + offset_coverage,
-                               length - offset_coverage,
-                               maxp->num_glyphs)) {
-    return OTS_FAILURE_MSG("Failed to parse coverage table in single adjustment table");
-  }
-
-  return true;
-}
-
 bool ParsePairSetTable(const ots::Font *font,
                        const uint8_t *data, const size_t length,
                        const uint16_t value_format1,
                        const uint16_t value_format2,
                        const uint16_t num_glyphs) {
   ots::Buffer subtable(data, length);
 
@@ -400,136 +306,14 @@
                                num_glyphs, ots::kMaxClassDefValue)) {
     return OTS_FAILURE_MSG("Failed to parse class definition table 2");
   }
 
   return true;
 }
 
-// Lookup Type 2:
-// Pair Adjustment Positioning Subtable
-bool ParsePairAdjustment(const ots::Font *font, const uint8_t *data,
-                         const size_t length) {
-  ots::Buffer subtable(data, length);
-
-  ots::OpenTypeMAXP *maxp = static_cast<ots::OpenTypeMAXP*>(
-      font->GetTypedTable(OTS_TAG_MAXP));
-  if (!maxp) {
-    return OTS_FAILURE_MSG("Required maxp table missing");
-  }
-
-  uint16_t format = 0;
-  uint16_t offset_coverage = 0;
-  uint16_t value_format1 = 0;
-  uint16_t value_format2 = 0;
-  if (!subtable.ReadU16(&format) ||
-      !subtable.ReadU16(&offset_coverage) ||
-      !subtable.ReadU16(&value_format1) ||
-      !subtable.ReadU16(&value_format2)) {
-    return OTS_FAILURE_MSG("Failed to read pair adjustment structure");
-  }
-
-  if (format == 1) {
-    if (!ParsePairPosFormat1(font, data, length, value_format1, value_format2,
-                             maxp->num_glyphs)) {
-      return OTS_FAILURE_MSG("Failed to parse pair pos format 1");
-    }
-  } else if (format == 2) {
-    if (!ParsePairPosFormat2(font, data, length, value_format1, value_format2,
-                             maxp->num_glyphs)) {
-      return OTS_FAILURE_MSG("Failed to parse pair format 2");
-    }
-  } else {
-    return OTS_FAILURE_MSG("Bad pos pair format %d", format);
-  }
-
-  if (offset_coverage < subtable.offset() || offset_coverage >= length) {
-    return OTS_FAILURE_MSG("Bad pair pos offset coverage %d", offset_coverage);
-  }
-  if (!ots::ParseCoverageTable(font, data + offset_coverage,
-                               length - offset_coverage,
-                               maxp->num_glyphs)) {
-    return OTS_FAILURE_MSG("Failed to parse coverage table");
-  }
-
-  return true;
-}
-
-// Lookup Type 3
-// Cursive Attachment Positioning Subtable
-bool ParseCursiveAttachment(const ots::Font *font, const uint8_t *data,
-                            const size_t length) {
-  ots::Buffer subtable(data, length);
-
-  ots::OpenTypeMAXP *maxp = static_cast<ots::OpenTypeMAXP*>(
-      font->GetTypedTable(OTS_TAG_MAXP));
-  if (!maxp) {
-    return OTS_FAILURE_MSG("Required maxp table missing");
-  }
-
-  uint16_t format = 0;
-  uint16_t offset_coverage = 0;
-  uint16_t entry_exit_count = 0;
-  if (!subtable.ReadU16(&format) ||
-      !subtable.ReadU16(&offset_coverage) ||
-      !subtable.ReadU16(&entry_exit_count)) {
-    return OTS_FAILURE_MSG("Failed to read cursive attachment structure");
-  }
-
-  if (format != 1) {
-    return OTS_FAILURE_MSG("Bad cursive attachment format %d", format);
-  }
-
-  // Check entry exit records.
-  const unsigned entry_exit_records_end =
-      2 * static_cast<unsigned>(entry_exit_count) + 6;
-  if (entry_exit_records_end > std::numeric_limits<uint16_t>::max()) {
-    return OTS_FAILURE_MSG("Bad entry exit record end %d", entry_exit_records_end);
-  }
-  for (unsigned i = 0; i < entry_exit_count; ++i) {
-    uint16_t offset_entry_anchor = 0;
-    uint16_t offset_exit_anchor = 0;
-    if (!subtable.ReadU16(&offset_entry_anchor) ||
-        !subtable.ReadU16(&offset_exit_anchor)) {
-      return OTS_FAILURE_MSG("Can't read entry exit record %d", i);
-    }
-    // These offsets could be NULL.
-    if (offset_entry_anchor) {
-      if (offset_entry_anchor < entry_exit_records_end ||
-          offset_entry_anchor >= length) {
-        return OTS_FAILURE_MSG("Bad entry anchor offset %d in entry exit record %d", offset_entry_anchor, i);
-      }
-      if (!ParseAnchorTable(font, data + offset_entry_anchor,
-                            length - offset_entry_anchor)) {
-        return OTS_FAILURE_MSG("Failed to parse entry anchor table in entry exit record %d", i);
-      }
-    }
-    if (offset_exit_anchor) {
-      if (offset_exit_anchor < entry_exit_records_end ||
-         offset_exit_anchor >= length) {
-        return OTS_FAILURE_MSG("Bad exit anchor offset %d in entry exit record %d", offset_exit_anchor, i);
-      }
-      if (!ParseAnchorTable(font, data + offset_exit_anchor,
-                            length - offset_exit_anchor)) {
-        return OTS_FAILURE_MSG("Failed to parse exit anchor table in entry exit record %d", i);
-      }
-    }
-  }
-
-  if (offset_coverage < subtable.offset() || offset_coverage >= length) {
-    return OTS_FAILURE_MSG("Bad coverage offset in cursive attachment %d", offset_coverage);
-  }
-  if (!ots::ParseCoverageTable(font, data + offset_coverage,
-                               length - offset_coverage,
-                               maxp->num_glyphs)) {
-    return OTS_FAILURE_MSG("Failed to parse coverage table in cursive attachment");
-  }
-
-  return true;
-}
-
 bool ParseAnchorArrayTable(const ots::Font *font,
                            const uint8_t *data, const size_t length,
                            const uint16_t class_count) {
   ots::Buffer subtable(data, length);
 
   uint16_t record_count = 0;
   if (!subtable.ReadU16(&record_count)) {
@@ -667,175 +451,261 @@
   } else {
     return OTS_FAILURE_MSG("Bad attachment type %d", type);
   }
 
   return true;
 }
 
-// Lookup Type 4:
-// MarkToBase Attachment Positioning Subtable
-bool ParseMarkToBaseAttachment(const ots::Font *font,
-                               const uint8_t *data, const size_t length) {
-  return ParseMarkToAttachmentSubtables(font, data, length,
-                                        GPOS_TYPE_MARK_TO_BASE_ATTACHMENT);
-}
+}  // namespace
 
-// Lookup Type 5:
-// MarkToLigature Attachment Positioning Subtable
-bool ParseMarkToLigatureAttachment(const ots::Font *font,
-                                   const uint8_t *data, const size_t length) {
-  return ParseMarkToAttachmentSubtables(font, data, length,
-                                        GPOS_TYPE_MARK_TO_LIGATURE_ATTACHMENT);
-}
+namespace ots {
 
-// Lookup Type 6:
-// MarkToMark Attachment Positioning Subtable
-bool ParseMarkToMarkAttachment(const ots::Font *font,
-                               const uint8_t *data, const size_t length) {
-  return ParseMarkToAttachmentSubtables(font, data, length,
-                                        GPOS_TYPE_MARK_TO_MARK_ATTACHMENT);
-}
+// Lookup Type 1:
+// Single Adjustment Positioning Subtable
+bool OpenTypeGPOS::ParseSingleAdjustment(const uint8_t *data,
+                                         const size_t length) {
+  Font* font = GetFont();
+  Buffer subtable(data, length);
 
-// Lookup Type 7:
-// Contextual Positioning Subtables
-bool ParseContextPositioning(const ots::Font *font,
-                             const uint8_t *data, const size_t length) {
-  ots::OpenTypeMAXP *maxp = static_cast<ots::OpenTypeMAXP*>(
+  OpenTypeMAXP *maxp = static_cast<OpenTypeMAXP*>(
       font->GetTypedTable(OTS_TAG_MAXP));
   if (!maxp) {
-    return OTS_FAILURE_MSG("Required maxp table missing");
+    return Error("Required maxp table missing");
   }
-  ots::OpenTypeGPOS *gpos = static_cast<ots::OpenTypeGPOS*>(
-      font->GetTypedTable(OTS_TAG_GPOS));
-  if (!gpos) {
-    return OTS_FAILURE_MSG("Internal error!");
+
+  uint16_t format = 0;
+  uint16_t offset_coverage = 0;
+  uint16_t value_format = 0;
+  if (!subtable.ReadU16(&format) ||
+      !subtable.ReadU16(&offset_coverage) ||
+      !subtable.ReadU16(&value_format)) {
+    return Error("Can't read single adjustment information");
   }
-  return ots::ParseContextSubtable(font, data, length, maxp->num_glyphs,
-                                   gpos->num_lookups);
-}
 
-// Lookup Type 8:
-// Chaining Contexual Positioning Subtable
-bool ParseChainedContextPositioning(const ots::Font *font,
-                                    const uint8_t *data, const size_t length) {
-  ots::OpenTypeMAXP *maxp = static_cast<ots::OpenTypeMAXP*>(
-      font->GetTypedTable(OTS_TAG_MAXP));
-  if (!maxp) {
-    return OTS_FAILURE_MSG("Required maxp table missing");
+  if (format == 1) {
+    // Format 1 exactly one value record.
+    if (!ParseValueRecord(font, &subtable, value_format)) {
+      return Error("Failed to parse format 1 single adjustment table");
+    }
+  } else if (format == 2) {
+    uint16_t value_count = 0;
+    if (!subtable.ReadU16(&value_count)) {
+      return Error("Failed to parse format 2 single adjustment table");
+    }
+    for (unsigned i = 0; i < value_count; ++i) {
+      if (!ParseValueRecord(font, &subtable, value_format)) {
+        return Error("Failed to parse value record %d in format 2 single adjustment table", i);
+      }
+    }
+  } else {
+    return Error("Bad format %d in single adjustment table", format);
   }
-  ots::OpenTypeGPOS *gpos = static_cast<ots::OpenTypeGPOS*>(
-      font->GetTypedTable(OTS_TAG_GPOS));
-  if (!gpos) {
-    return OTS_FAILURE_MSG("Internal error!");
-  }
-  return ots::ParseChainingContextSubtable(font, data, length,
-                                           maxp->num_glyphs,
-                                           gpos->num_lookups);
-}
 
-// Lookup Type 9:
-// Extension Positioning
-bool ParseExtensionPositioning(const ots::Font *font,
-                               const uint8_t *data, const size_t length) {
-  return ots::ParseExtensionSubtable(font, data, length,
-                                     &kGposLookupSubtableParser);
-}
+  if (offset_coverage < subtable.offset() || offset_coverage >= length) {
+    return Error("Bad coverage offset %d in single adjustment table", offset_coverage);
+  }
 
-}  // namespace
+  if (!ots::ParseCoverageTable(font, data + offset_coverage,
+                               length - offset_coverage,
+                               maxp->num_glyphs)) {
+    return Error("Failed to parse coverage table in single adjustment table");
+  }
 
-namespace ots {
+  return true;
+}
 
-bool OpenTypeGPOS::Parse(const uint8_t *data, size_t length) {
-  Font *font = GetFont();
-  Buffer table(data, length);
+// Lookup Type 2:
+// Pair Adjustment Positioning Subtable
+bool OpenTypeGPOS::ParsePairAdjustment(const uint8_t *data,
+                                       const size_t length) {
+  Font* font = GetFont();
+  Buffer subtable(data, length);
 
-  uint16_t version_major = 0, version_minor = 0;
-  uint16_t offset_script_list = 0;
-  uint16_t offset_feature_list = 0;
-  uint16_t offset_lookup_list = 0;
-  uint32_t offset_feature_variations = 0;
-  if (!table.ReadU16(&version_major) ||
-      !table.ReadU16(&version_minor) ||
-      !table.ReadU16(&offset_script_list) ||
-      !table.ReadU16(&offset_feature_list) ||
-      !table.ReadU16(&offset_lookup_list)) {
-    return Error("Incomplete table");
+  OpenTypeMAXP *maxp = static_cast<OpenTypeMAXP*>(
+      font->GetTypedTable(OTS_TAG_MAXP));
+  if (!maxp) {
+    return Error("Required maxp table missing");
   }
 
-  if (version_major != 1 || version_minor > 1) {
-    return Error("Bad version");
+  uint16_t format = 0;
+  uint16_t offset_coverage = 0;
+  uint16_t value_format1 = 0;
+  uint16_t value_format2 = 0;
+  if (!subtable.ReadU16(&format) ||
+      !subtable.ReadU16(&offset_coverage) ||
+      !subtable.ReadU16(&value_format1) ||
+      !subtable.ReadU16(&value_format2)) {
+    return Error("Failed to read pair adjustment structure");
   }
 
-  if (version_minor > 0) {
-    if (!table.ReadU32(&offset_feature_variations)) {
-      return Error("Incomplete table");
+  if (format == 1) {
+    if (!ParsePairPosFormat1(font, data, length, value_format1, value_format2,
+                             maxp->num_glyphs)) {
+      return Error("Failed to parse pair pos format 1");
+    }
+  } else if (format == 2) {
+    if (!ParsePairPosFormat2(font, data, length, value_format1, value_format2,
+                             maxp->num_glyphs)) {
+      return Error("Failed to parse pair format 2");
     }
+  } else {
+    return Error("Bad pos pair format %d", format);
   }
 
-  const size_t header_size =
-    (version_minor == 0) ? kGposHeaderSize_1_0 : kGposHeaderSize_1_1;
+  if (offset_coverage < subtable.offset() || offset_coverage >= length) {
+    return Error("Bad pair pos offset coverage %d", offset_coverage);
+  }
+  if (!ots::ParseCoverageTable(font, data + offset_coverage,
+                               length - offset_coverage,
+                               maxp->num_glyphs)) {
+    return Error("Failed to parse coverage table");
+  }
 
-  if (offset_lookup_list) {
-    if (offset_lookup_list < header_size || offset_lookup_list >= length) {
-      return Error("Bad lookup list offset in table header");
-    }
+  return true;
+}
 
-    if (!ParseLookupListTable(font, data + offset_lookup_list,
-                              length - offset_lookup_list,
-                              &kGposLookupSubtableParser,
-                              &this->num_lookups)) {
-      return Error("Failed to parse lookup list table");
-    }
+// Lookup Type 3
+// Cursive Attachment Positioning Subtable
+bool OpenTypeGPOS::ParseCursiveAttachment(const uint8_t *data,
+                                          const size_t length) {
+  Font* font = GetFont();
+  Buffer subtable(data, length);
+
+  OpenTypeMAXP *maxp = static_cast<OpenTypeMAXP*>(
+      font->GetTypedTable(OTS_TAG_MAXP));
+  if (!maxp) {
+    return Error("Required maxp table missing");
   }
 
-  uint16_t num_features = 0;
-  if (offset_feature_list) {
-    if (offset_feature_list < header_size || offset_feature_list >= length) {
-      return Error("Bad feature list offset in table header");
-    }
+  uint16_t format = 0;
+  uint16_t offset_coverage = 0;
+  uint16_t entry_exit_count = 0;
+  if (!subtable.ReadU16(&format) ||
+      !subtable.ReadU16(&offset_coverage) ||
+      !subtable.ReadU16(&entry_exit_count)) {
+    return Error("Failed to read cursive attachment structure");
+  }
 
-    if (!ParseFeatureListTable(font, data + offset_feature_list,
-                               length - offset_feature_list, this->num_lookups,
-                               &num_features)) {
-      return Error("Failed to parse feature list table");
-    }
+  if (format != 1) {
+    return Error("Bad cursive attachment format %d", format);
   }
 
-  if (offset_script_list) {
-    if (offset_script_list < header_size || offset_script_list >= length) {
-      return Error("Bad script list offset in table header");
+  // Check entry exit records.
+  const unsigned entry_exit_records_end =
+      2 * static_cast<unsigned>(entry_exit_count) + 6;
+  if (entry_exit_records_end > std::numeric_limits<uint16_t>::max()) {
+    return Error("Bad entry exit record end %d", entry_exit_records_end);
+  }
+  for (unsigned i = 0; i < entry_exit_count; ++i) {
+    uint16_t offset_entry_anchor = 0;
+    uint16_t offset_exit_anchor = 0;
+    if (!subtable.ReadU16(&offset_entry_anchor) ||
+        !subtable.ReadU16(&offset_exit_anchor)) {
+      return Error("Can't read entry exit record %d", i);
     }
-
-    if (!ParseScriptListTable(font, data + offset_script_list,
-                              length - offset_script_list, num_features)) {
-      return Error("Failed to parse script list table");
+    // These offsets could be NULL.
+    if (offset_entry_anchor) {
+      if (offset_entry_anchor < entry_exit_records_end ||
+          offset_entry_anchor >= length) {
+        return Error("Bad entry anchor offset %d in entry exit record %d", offset_entry_anchor, i);
+      }
+      if (!ParseAnchorTable(font, data + offset_entry_anchor,
+                            length - offset_entry_anchor)) {
+        return Error("Failed to parse entry anchor table in entry exit record %d", i);
+      }
     }
-  }
-
-  if (offset_feature_variations) {
-    if (offset_feature_variations < header_size || offset_feature_variations >= length) {
-      return Error("Bad feature variations offset in table header");
+    if (offset_exit_anchor) {
+      if (offset_exit_anchor < entry_exit_records_end ||
+         offset_exit_anchor >= length) {
+        return Error("Bad exit anchor offset %d in entry exit record %d", offset_exit_anchor, i);
+      }
+      if (!ParseAnchorTable(font, data + offset_exit_anchor,
+                            length - offset_exit_anchor)) {
+        return Error("Failed to parse exit anchor table in entry exit record %d", i);
+      }
     }
+  }
 
-    if (!ParseFeatureVariationsTable(font, data + offset_feature_variations,
-                                     length - offset_feature_variations,
-                                     this->num_lookups)) {
-      return Error("Failed to parse feature variations table");
-    }
+  if (offset_coverage < subtable.offset() || offset_coverage >= length) {
+    return Error("Bad coverage offset in cursive attachment %d", offset_coverage);
+  }
+  if (!ots::ParseCoverageTable(font, data + offset_coverage,
+                               length - offset_coverage,
+                               maxp->num_glyphs)) {
+    return Error("Failed to parse coverage table in cursive attachment");
   }
 
-  this->m_data = data;
-  this->m_length = length;
   return true;
 }
 
-bool OpenTypeGPOS::Serialize(OTSStream *out) {
-  if (!out->Write(this->m_data, this->m_length)) {
-    return Error("Failed to write GPOS table");
-  }
+// Lookup Type 4:
+// MarkToBase Attachment Positioning Subtable
+bool OpenTypeGPOS::ParseMarkToBaseAttachment(const uint8_t *data,
+                                             const size_t length) {
+  return ParseMarkToAttachmentSubtables(GetFont(), data, length,
+                                        GPOS_TYPE_MARK_TO_BASE_ATTACHMENT);
+}
 
-  return true;
+// Lookup Type 5:
+// MarkToLigature Attachment Positioning Subtable
+bool OpenTypeGPOS::ParseMarkToLigatureAttachment(const uint8_t *data,
+                                                 const size_t length) {
+  return ParseMarkToAttachmentSubtables(GetFont(), data, length,
+                                        GPOS_TYPE_MARK_TO_LIGATURE_ATTACHMENT);
+}
+
+// Lookup Type 6:
+// MarkToMark Attachment Positioning Subtable
+bool OpenTypeGPOS::ParseMarkToMarkAttachment(const uint8_t *data,
+                                             const size_t length) {
+  return ParseMarkToAttachmentSubtables(GetFont(), data, length,
+                                        GPOS_TYPE_MARK_TO_MARK_ATTACHMENT);
+}
+
+// Lookup Type 7:
+// Contextual Positioning Subtables
+// OpenTypeLayoutTable::ParseContextSubtable()
+
+// Lookup Type 8:
+// Chaining Contexual Positioning Subtable
+// OpenTypeLayoutTable::ParseChainingContextSubtable()
+
+// Lookup Type 9:
+// Extension Positioning
+// OpenTypeLayoutTable::ParseExtensionSubtable
+
+
+bool OpenTypeGPOS::ValidLookupSubtableType(const uint16_t lookup_type,
+                                           bool extension) const {
+  if (extension && lookup_type == GPOS_TYPE_EXTENSION_POSITIONING)
+    return false;
+  return lookup_type >= GPOS_TYPE_SINGLE_ADJUSTMENT && lookup_type < GPOS_TYPE_RESERVED;
+}
+
+bool OpenTypeGPOS::ParseLookupSubtable(const uint8_t *data, const size_t length,
+                                       const uint16_t lookup_type) {
+  switch (lookup_type) {
+    case GPOS_TYPE_SINGLE_ADJUSTMENT:
+      return ParseSingleAdjustment(data, length);
+    case GPOS_TYPE_PAIR_ADJUSTMENT:
+      return ParsePairAdjustment(data, length);
+    case GPOS_TYPE_CURSIVE_ATTACHMENT:
+      return ParseCursiveAttachment(data, length);
+    case GPOS_TYPE_MARK_TO_BASE_ATTACHMENT:
+      return ParseMarkToBaseAttachment(data, length);
+    case GPOS_TYPE_MARK_TO_LIGATURE_ATTACHMENT:
+      return ParseMarkToLigatureAttachment(data, length);
+    case GPOS_TYPE_MARK_TO_MARK_ATTACHMENT:
+      return ParseMarkToMarkAttachment(data, length);
+    case GPOS_TYPE_CONTEXT_POSITIONING:
+      return ParseContextSubtable(data, length);
+    case GPOS_TYPE_CHAINED_CONTEXT_POSITIONING:
+      return ParseChainingContextSubtable(data, length);
+    case GPOS_TYPE_EXTENSION_POSITIONING:
+      return ParseExtensionSubtable(data, length);
+  }
+  return false;
 }
 
 }  // namespace ots
 
 #undef TABLE_NAME
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gpos.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/prep.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-// Copyright (c) 2011-2017 The OTS Authors. All rights reserved.
+// Copyright (c) 2009-2017 The OTS Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
-#ifndef OTS_GPOS_H_
-#define OTS_GPOS_H_
+#ifndef OTS_PREP_H_
+#define OTS_PREP_H_
 
 #include "ots.h"
 
 namespace ots {
 
-class OpenTypeGPOS : public Table {
+class OpenTypePREP : public Table {
  public:
-  explicit OpenTypeGPOS(Font *font, uint32_t tag)
-      : Table(font, tag, tag),
-        num_lookups(0),
-        m_data(NULL),
-        m_length(0) {
-  }
+  explicit OpenTypePREP(Font *font, uint32_t tag)
+      : Table(font, tag, tag) { }
 
   bool Parse(const uint8_t *data, size_t length);
   bool Serialize(OTSStream *out);
-
-  // Number of lookups in GPOS table
-  uint16_t num_lookups;
+  bool ShouldSerialize();
 
  private:
   const uint8_t *m_data;
-  size_t m_length;
+  uint32_t m_length;
 };
 
 }  // namespace ots
 
-#endif
-
+#endif  // OTS_PREP_H_
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/graphite.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/graphite.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gsub.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/gvar.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-// Copyright (c) 2011-2017 The OTS Authors. All rights reserved.
+// Copyright (c) 2018 The OTS Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
-#ifndef OTS_GSUB_H_
-#define OTS_GSUB_H_
+#ifndef OTS_GVAR_H_
+#define OTS_GVAR_H_
 
 #include "ots.h"
 
 namespace ots {
 
-class OpenTypeGSUB : public Table {
+// -----------------------------------------------------------------------------
+// OpenTypeGVAR Interface
+// -----------------------------------------------------------------------------
+
+class OpenTypeGVAR : public Table {
  public:
-  explicit OpenTypeGSUB(Font *font, uint32_t tag)
-      : Table(font, tag, tag),
-        num_lookups(0),
-        m_data(NULL),
-        m_length(0) {
+  explicit OpenTypeGVAR(Font* font, uint32_t tag)
+      : Table(font, tag, tag), m_ownsData(false) { }
+
+  virtual ~OpenTypeGVAR() {
+    if (m_ownsData) {
+      delete[] m_data;
+    }
   }
 
-  bool Parse(const uint8_t *data, size_t length);
-  bool Serialize(OTSStream *out);
+  bool Parse(const uint8_t* data, size_t length);
+  bool Serialize(OTSStream* out);
 
-  // Number of lookups in GPSUB table
-  uint16_t num_lookups;
+#ifdef OTS_SYNTHESIZE_MISSING_GVAR
+  bool InitEmpty();
+#endif
 
- //private:
+ private:
   const uint8_t *m_data;
   size_t m_length;
+
+  bool m_ownsData;
 };
 
 }  // namespace ots
 
-#endif  // OTS_GSUB_H_
-
+#endif  // OTS_GVAR_H_
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gvar.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/gvar.cc`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 // found in the LICENSE file.
 
 #include "gvar.h"
 
 #include "fvar.h"
 #include "maxp.h"
 #include "variations.h"
+#include "ots-memory-stream.h"
 
 #define TABLE_NAME "gvar"
 
 namespace ots {
 
 // -----------------------------------------------------------------------------
 // OpenTypeGVAR
@@ -141,14 +142,64 @@
 
   this->m_data = data;
   this->m_length = length;
 
   return true;
 }
 
+#ifdef OTS_SYNTHESIZE_MISSING_GVAR
+bool OpenTypeGVAR::InitEmpty() {
+  // Generate an empty but well-formed 'gvar' table for the font.
+  const ots::Font* font = GetFont();
+
+  OpenTypeFVAR* fvar = static_cast<OpenTypeFVAR*>(font->GetTypedTable(OTS_TAG_FVAR));
+  if (!fvar) {
+    return DropVariations("Required fvar table missing");
+  }
+
+  OpenTypeMAXP* maxp = static_cast<OpenTypeMAXP*>(font->GetTypedTable(OTS_TAG_MAXP));
+  if (!maxp) {
+    return DropVariations("Required maxp table missing");
+  }
+
+  uint16_t majorVersion = 1;
+  uint16_t minorVersion = 0;
+  uint16_t axisCount = fvar->AxisCount();
+  uint16_t sharedTupleCount = 0;
+  uint32_t sharedTuplesOffset = 0;
+  uint16_t glyphCount = maxp->num_glyphs;
+  uint16_t flags = 0;
+  uint32_t glyphVariationDataArrayOffset = 0;
+
+  size_t length = 6 * sizeof(uint16_t) + 2 * sizeof(uint32_t)  // basic header fields
+      + (glyphCount + 1) * sizeof(uint16_t);  // glyphVariationDataOffsets[] array
+
+  uint8_t* data = new uint8_t[length];
+  MemoryStream stream(data, length);
+  if (!stream.WriteU16(majorVersion) ||
+      !stream.WriteU16(minorVersion) ||
+      !stream.WriteU16(axisCount) ||
+      !stream.WriteU16(sharedTupleCount) ||
+      !stream.WriteU32(sharedTuplesOffset) ||
+      !stream.WriteU16(glyphCount) ||
+      !stream.WriteU16(flags) ||
+      !stream.WriteU32(glyphVariationDataArrayOffset) ||
+      !stream.Pad((glyphCount + 1) * sizeof(uint16_t))) {
+    delete[] data;
+    return DropVariations("Failed to generate dummy gvar table");
+  }
+
+  this->m_data = data;
+  this->m_length = length;
+  this->m_ownsData = true;
+
+  return true;
+}
+#endif
+
 bool OpenTypeGVAR::Serialize(OTSStream* out) {
   if (!out->Write(this->m_data, this->m_length)) {
     return Error("Failed to write gvar table");
   }
 
   return true;
 }
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/gvar.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/mvar.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 // Copyright (c) 2018 The OTS Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
-#ifndef OTS_GVAR_H_
-#define OTS_GVAR_H_
+#ifndef OTS_MVAR_H_
+#define OTS_MVAR_H_
 
 #include "ots.h"
 
 namespace ots {
 
 // -----------------------------------------------------------------------------
-// OpenTypeGVAR Interface
+// OpenTypeMVAR Interface
 // -----------------------------------------------------------------------------
 
-class OpenTypeGVAR : public Table {
+class OpenTypeMVAR : public Table {
  public:
-  explicit OpenTypeGVAR(Font* font, uint32_t tag)
+  explicit OpenTypeMVAR(Font* font, uint32_t tag)
       : Table(font, tag, tag) { }
 
   bool Parse(const uint8_t* data, size_t length);
   bool Serialize(OTSStream* out);
 
  private:
   const uint8_t *m_data;
   size_t m_length;
 };
 
 }  // namespace ots
 
-#endif  // OTS_GVAR_H_
+#endif  // OTS_MVAR_H_
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/hdmx.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/hdmx.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/hdmx.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/hdmx.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/head.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/head.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/head.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/head.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/hhea.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/hhea.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/hhea.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/hhea.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/hvar.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/hvar.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/hvar.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/hvar.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/kern.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/kern.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/kern.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/kern.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/layout.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/layout.cc`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #include "layout.h"
 
 #include <limits>
 #include <vector>
 
 #include "fvar.h"
 #include "gdef.h"
+#include "maxp.h"
 
 // OpenType Layout Common Table Formats
 // http://www.microsoft.com/typography/otspec/chapter2.htm
 
 #define TABLE_NAME "Layout" // XXX: use individual table names
 
 namespace {
@@ -170,83 +171,14 @@
     if (lookup_index >= num_lookups) {
       return OTS_FAILURE_MSG("Bad lookup index %d for lookup %d", lookup_index, i);
     }
   }
   return true;
 }
 
-bool ParseLookupTable(ots::Font *font, const uint8_t *data,
-                      const size_t length,
-                      const ots::LookupSubtableParser* parser) {
-  ots::Buffer subtable(data, length);
-
-  uint16_t lookup_type = 0;
-  uint16_t lookup_flag = 0;
-  uint16_t subtable_count = 0;
-  if (!subtable.ReadU16(&lookup_type) ||
-      !subtable.ReadU16(&lookup_flag) ||
-      !subtable.ReadU16(&subtable_count)) {
-    return OTS_FAILURE_MSG("Failed to read lookup table header");
-  }
-
-  if (lookup_type == 0 || lookup_type > parser->num_types) {
-    return OTS_FAILURE_MSG("Bad lookup type %d", lookup_type);
-  }
-
-  bool use_mark_filtering_set = lookup_flag & kUseMarkFilteringSetBit;
-
-  std::vector<uint16_t> subtables;
-  subtables.reserve(subtable_count);
-  // If the |kUseMarkFilteringSetBit| of |lookup_flag| is set,
-  // extra 2 bytes will follow after subtable offset array.
-  const unsigned lookup_table_end = 2 * static_cast<unsigned>(subtable_count) +
-      (use_mark_filtering_set ? 8 : 6);
-  if (lookup_table_end > std::numeric_limits<uint16_t>::max()) {
-    return OTS_FAILURE_MSG("Bad end of lookup %d", lookup_table_end);
-  }
-  for (unsigned i = 0; i < subtable_count; ++i) {
-    uint16_t offset_subtable = 0;
-    if (!subtable.ReadU16(&offset_subtable)) {
-      return OTS_FAILURE_MSG("Failed to read subtable offset %d", i);
-    }
-    if (offset_subtable < lookup_table_end ||
-        offset_subtable >= length) {
-      return OTS_FAILURE_MSG("Bad subtable offset %d for subtable %d", offset_subtable, i);
-    }
-    subtables.push_back(offset_subtable);
-  }
-  if (subtables.size() != subtable_count) {
-    return OTS_FAILURE_MSG("Bad subtable size %ld", subtables.size());
-  }
-
-  if (use_mark_filtering_set) {
-    uint16_t mark_filtering_set = 0;
-    if (!subtable.ReadU16(&mark_filtering_set)) {
-      return OTS_FAILURE_MSG("Failed to read mark filtering set");
-    }
-
-    ots::OpenTypeGDEF *gdef = static_cast<ots::OpenTypeGDEF*>(
-        font->GetTypedTable(OTS_TAG_GDEF));
-
-    if (gdef && (gdef->num_mark_glyph_sets == 0 ||
-        mark_filtering_set >= gdef->num_mark_glyph_sets)) {
-      return OTS_FAILURE_MSG("Bad mark filtering set %d", mark_filtering_set);
-    }
-  }
-
-  // Parse lookup subtables for this lookup type.
-  for (unsigned i = 0; i < subtable_count; ++i) {
-    if (!parser->Parse(font, data + subtables[i], length - subtables[i],
-                       lookup_type)) {
-      return OTS_FAILURE_MSG("Failed to parse subtable %d", i);
-    }
-  }
-  return true;
-}
-
 bool ParseClassDefFormat1(const ots::Font *font,
                           const uint8_t *data, size_t length,
                           const uint16_t num_glyphs,
                           const uint16_t num_classes) {
   ots::Buffer subtable(data, length);
 
   // Skip format field.
@@ -442,15 +374,15 @@
   uint16_t glyph_count = 0;
   uint16_t lookup_count = 0;
   if (!subtable.ReadU16(&glyph_count) ||
       !subtable.ReadU16(&lookup_count)) {
     return OTS_FAILURE_MSG("Failed to read rule subtable header");
   }
 
-  if (glyph_count == 0 || glyph_count >= num_glyphs) {
+  if (glyph_count == 0) {
     return OTS_FAILURE_MSG("Bad glyph count %d in rule subtable", glyph_count);
   }
   for (unsigned i = 0; i < glyph_count - static_cast<unsigned>(1); ++i) {
     uint16_t glyph_id = 0;
     if (!subtable.ReadU16(&glyph_id)) {
       return OTS_FAILURE_MSG("Failed to read glyph %d", i);
     }
@@ -721,32 +653,29 @@
                             const uint16_t num_lookups) {
   ots::Buffer subtable(data, length);
 
   uint16_t backtrack_count = 0;
   if (!subtable.ReadU16(&backtrack_count)) {
     return OTS_FAILURE_MSG("Failed to read backtrack count in chain rule subtable");
   }
-  if (backtrack_count >= num_glyphs) {
-    return OTS_FAILURE_MSG("Bad backtrack count %d in chain rule subtable", backtrack_count);
-  }
   for (unsigned i = 0; i < backtrack_count; ++i) {
     uint16_t glyph_id = 0;
     if (!subtable.ReadU16(&glyph_id)) {
       return OTS_FAILURE_MSG("Failed to read backtrack glyph %d in chain rule subtable", i);
     }
     if (glyph_id > num_glyphs) {
       return OTS_FAILURE_MSG("Bad glyph id %d for bactrack glyph %d in chain rule subtable", glyph_id, i);
     }
   }
 
   uint16_t input_count = 0;
   if (!subtable.ReadU16(&input_count)) {
     return OTS_FAILURE_MSG("Failed to read input count in chain rule subtable");
   }
-  if (input_count == 0 || input_count >= num_glyphs) {
+  if (input_count == 0) {
     return OTS_FAILURE_MSG("Bad input count %d in chain rule subtable", input_count);
   }
   for (unsigned i = 0; i < input_count - static_cast<unsigned>(1); ++i) {
     uint16_t glyph_id = 0;
     if (!subtable.ReadU16(&glyph_id)) {
       return OTS_FAILURE_MSG("Failed to read input glyph %d in chain rule subtable", i);
     }
@@ -755,17 +684,14 @@
     }
   }
 
   uint16_t lookahead_count = 0;
   if (!subtable.ReadU16(&lookahead_count)) {
     return OTS_FAILURE_MSG("Failed to read lookahead count in chain rule subtable");
   }
-  if (lookahead_count >= num_glyphs) {
-    return OTS_FAILURE_MSG("Bad lookahead count %d in chain rule subtable", lookahead_count);
-  }
   for (unsigned i = 0; i < lookahead_count; ++i) {
     uint16_t glyph_id = 0;
     if (!subtable.ReadU16(&glyph_id)) {
       return OTS_FAILURE_MSG("Failed to read lookahead glyph %d in chain rule subtable", i);
     }
     if (glyph_id > num_glyphs) {
       return OTS_FAILURE_MSG("Bad glyph id %d for lookadhead glyph %d in chain rule subtable", glyph_id, i);
@@ -874,39 +800,33 @@
   // In this subtable, we don't check the value of classes for now since
   // these could take arbitrary values.
 
   uint16_t backtrack_count = 0;
   if (!subtable.ReadU16(&backtrack_count)) {
     return OTS_FAILURE_MSG("Failed to read backtrack count in chain class rule subtable");
   }
-  if (backtrack_count >= num_glyphs) {
-    return OTS_FAILURE_MSG("Bad backtrack count %d in chain class rule subtable", backtrack_count);
-  }
   if (!subtable.Skip(2 * backtrack_count)) {
     return OTS_FAILURE_MSG("Failed to skip backtrack offsets in chain class rule subtable");
   }
 
   uint16_t input_count = 0;
   if (!subtable.ReadU16(&input_count)) {
     return OTS_FAILURE_MSG("Failed to read input count in chain class rule subtable");
   }
-  if (input_count == 0 || input_count >= num_glyphs) {
+  if (input_count == 0) {
     return OTS_FAILURE_MSG("Bad input count %d in chain class rule subtable", input_count);
   }
   if (!subtable.Skip(2 * (input_count - 1))) {
     return OTS_FAILURE_MSG("Failed to skip input offsets in chain class rule subtable");
   }
 
   uint16_t lookahead_count = 0;
   if (!subtable.ReadU16(&lookahead_count)) {
     return OTS_FAILURE_MSG("Failed to read lookahead count in chain class rule subtable");
   }
-  if (lookahead_count >= num_glyphs) {
-    return OTS_FAILURE_MSG("Bad lookahead count %d in chain class rule subtable", lookahead_count);
-  }
   if (!subtable.Skip(2 * lookahead_count)) {
     return OTS_FAILURE_MSG("Failed to skip lookahead offsets in chain class rule subtable");
   }
 
   uint16_t lookup_count = 0;
   if (!subtable.ReadU16(&lookup_count)) {
     return OTS_FAILURE_MSG("Failed to read lookup count in chain class rule subtable");
@@ -1054,17 +974,14 @@
   uint16_t backtrack_count = 0;
   // Skip format field.
   if (!subtable.Skip(2) ||
       !subtable.ReadU16(&backtrack_count)) {
     return OTS_FAILURE_MSG("Failed to read backtrack count in chain context format 3");
   }
 
-  if (backtrack_count >= num_glyphs) {
-    return OTS_FAILURE_MSG("Bad backtrack count %d in chain context format 3", backtrack_count);
-  }
   std::vector<uint16_t> offsets_backtrack;
   offsets_backtrack.reserve(backtrack_count);
   for (unsigned i = 0; i < backtrack_count; ++i) {
     uint16_t offset = 0;
     if (!subtable.ReadU16(&offset)) {
       return OTS_FAILURE_MSG("Failed to read backtrack offset %d in chain context format 3", i);
     }
@@ -1074,17 +991,14 @@
     return OTS_FAILURE_MSG("Bad backtrack offsets size %ld in chain context format 3", offsets_backtrack.size());
   }
 
   uint16_t input_count = 0;
   if (!subtable.ReadU16(&input_count)) {
     return OTS_FAILURE_MSG("Failed to read input count in chain context format 3");
   }
-  if (input_count >= num_glyphs) {
-    return OTS_FAILURE_MSG("Bad input count %d in chain context format 3", input_count);
-  }
   std::vector<uint16_t> offsets_input;
   offsets_input.reserve(input_count);
   for (unsigned i = 0; i < input_count; ++i) {
     uint16_t offset = 0;
     if (!subtable.ReadU16(&offset)) {
       return OTS_FAILURE_MSG("Failed to read input offset %d in chain context format 3", i);
     }
@@ -1094,17 +1008,14 @@
     return OTS_FAILURE_MSG("Bad input offsets size %ld in chain context format 3", offsets_input.size());
   }
 
   uint16_t lookahead_count = 0;
   if (!subtable.ReadU16(&lookahead_count)) {
     return OTS_FAILURE_MSG("Failed ot read lookahead count in chain context format 3");
   }
-  if (lookahead_count >= num_glyphs) {
-    return OTS_FAILURE_MSG("Bad lookahead count %d in chain context format 3", lookahead_count);
-  }
   std::vector<uint16_t> offsets_lookahead;
   offsets_lookahead.reserve(lookahead_count);
   for (unsigned i = 0; i < lookahead_count; ++i) {
     uint16_t offset = 0;
     if (!subtable.ReadU16(&offset)) {
       return OTS_FAILURE_MSG("Failed to read lookahead offset %d in chain context format 3", i);
     }
@@ -1161,175 +1072,330 @@
       return OTS_FAILURE_MSG("Failed to parse lookahead coverage table %d in chain context format 3", i);
     }
   }
 
   return true;
 }
 
-}  // namespace
+bool ParseFeatureTableSubstitutionTable(const ots::Font *font,
+                                        const uint8_t *data, const size_t length,
+                                        const uint16_t num_lookups) {
+  ots::Buffer subtable(data, length);
 
-namespace ots {
+  uint16_t version_major = 0;
+  uint16_t version_minor = 0;
+  uint16_t substitution_count = 0;
+  const size_t kFeatureTableSubstitutionHeaderSize = 3 * sizeof(uint16_t);
 
-bool LookupSubtableParser::Parse(const Font *font, const uint8_t *data,
-                                 const size_t length,
-                                 const uint16_t lookup_type) const {
-  for (unsigned i = 0; i < num_types; ++i) {
-    if (parsers[i].type == lookup_type && parsers[i].parse) {
-      if (!parsers[i].parse(font, data, length)) {
-        return OTS_FAILURE_MSG("Failed to parse lookup subtable %d", i);
-      }
-      return true;
+  if (!subtable.ReadU16(&version_major) ||
+      !subtable.ReadU16(&version_minor) ||
+      !subtable.ReadU16(&substitution_count)) {
+    return OTS_FAILURE_MSG("Failed to read feature table substitution table header");
+  }
+
+  for (uint16_t i = 0; i < substitution_count; i++) {
+    uint16_t feature_index = 0;
+    uint32_t alternate_feature_table_offset = 0;
+    const size_t kFeatureTableSubstitutionRecordSize = sizeof(uint16_t) + sizeof(uint32_t);
+
+    if (!subtable.ReadU16(&feature_index) ||
+        !subtable.ReadU32(&alternate_feature_table_offset)) {
+      return OTS_FAILURE_MSG("Failed to read feature table substitution record");
+    }
+
+    if (alternate_feature_table_offset < kFeatureTableSubstitutionHeaderSize +
+                                         kFeatureTableSubstitutionRecordSize * substitution_count ||
+        alternate_feature_table_offset >= length) {
+      return OTS_FAILURE_MSG("Invalid alternate feature table offset");
+    }
+
+    if (!ParseFeatureTable(font, data + alternate_feature_table_offset,
+                           length - alternate_feature_table_offset, num_lookups)) {
+      return OTS_FAILURE_MSG("Failed to parse alternate feature table");
+    }
+  }
+
+  return true;
+}
+
+bool ParseConditionTable(const ots::Font *font,
+                         const uint8_t *data, const size_t length,
+                         const uint16_t axis_count) {
+  ots::Buffer subtable(data, length);
+
+  uint16_t format = 0;
+  if (!subtable.ReadU16(&format)) {
+    return OTS_FAILURE_MSG("Failed to read condition table format");
+  }
+
+  if (format != 1) {
+    // An unknown format is not an error, but should be ignored per spec.
+    return true;
+  }
+
+  uint16_t axis_index = 0;
+  int16_t filter_range_min_value = 0;
+  int16_t filter_range_max_value = 0;
+  if (!subtable.ReadU16(&axis_index) ||
+      !subtable.ReadS16(&filter_range_min_value) ||
+      !subtable.ReadS16(&filter_range_max_value)) {
+    return OTS_FAILURE_MSG("Failed to read condition table (format 1)");
+  }
+
+  if (axis_index >= axis_count) {
+    return OTS_FAILURE_MSG("Axis index out of range in condition");
+  }
+
+  // Check min/max values are within range -1.0 .. 1.0 and properly ordered
+  if (filter_range_min_value < -0x4000 || // -1.0 in F2DOT14 format
+      filter_range_max_value > 0x4000 || // +1.0 in F2DOT14 format
+      filter_range_min_value > filter_range_max_value) {
+    return OTS_FAILURE_MSG("Invalid filter range in condition");
+  }
+
+  return true;
+}
+
+bool ParseConditionSetTable(const ots::Font *font,
+                            const uint8_t *data, const size_t length,
+                            const uint16_t axis_count) {
+  ots::Buffer subtable(data, length);
+
+  uint16_t condition_count = 0;
+  if (!subtable.ReadU16(&condition_count)) {
+    return OTS_FAILURE_MSG("Failed to read condition count");
+  }
+
+  for (uint16_t i = 0; i < condition_count; i++) {
+    uint32_t condition_offset = 0;
+    if (!subtable.ReadU32(&condition_offset)) {
+      return OTS_FAILURE_MSG("Failed to read condition offset");
+    }
+    if (condition_offset < subtable.offset() || condition_offset >= length) {
+      return OTS_FAILURE_MSG("Offset out of range");
+    }
+    if (!ParseConditionTable(font, data + condition_offset, length - condition_offset,
+                             axis_count)) {
+      return OTS_FAILURE_MSG("Failed to parse condition table");
     }
   }
-  return OTS_FAILURE_MSG("No lookup subtables to parse");
+
+  return true;
 }
 
+}  // namespace
+
+namespace ots {
+
 // Parsing ScriptListTable requires number of features so we need to
 // parse FeatureListTable before calling this function.
-bool ParseScriptListTable(const ots::Font *font,
-                          const uint8_t *data, const size_t length,
-                          const uint16_t num_features) {
+bool OpenTypeLayoutTable::ParseScriptListTable(const uint8_t *data, const size_t length) {
+  Font* font = GetFont();
   Buffer subtable(data, length);
 
   uint16_t script_count = 0;
   if (!subtable.ReadU16(&script_count)) {
-    return OTS_FAILURE_MSG("Failed to read script count in script list table");
+    return Error("Failed to read script count in script list table");
   }
 
   const unsigned script_record_end =
       6 * static_cast<unsigned>(script_count) + 2;
   if (script_record_end > std::numeric_limits<uint16_t>::max()) {
-    return OTS_FAILURE_MSG("Bad end of script record %d in script list table", script_record_end);
+    return Error("Bad end of script record %d in script list table", script_record_end);
   }
   std::vector<ScriptRecord> script_list;
   script_list.reserve(script_count);
   uint32_t last_tag = 0;
   for (unsigned i = 0; i < script_count; ++i) {
     ScriptRecord record;
     if (!subtable.ReadU32(&record.tag) ||
         !subtable.ReadU16(&record.offset)) {
-      return OTS_FAILURE_MSG("Failed to read script record %d in script list table", i);
+      return Error("Failed to read script record %d in script list table", i);
     }
     // Script tags should be arranged alphabetically by tag
     if (last_tag != 0 && last_tag > record.tag) {
       // Several fonts don't arrange tags alphabetically.
       // It seems that the order of tags might not be a security issue
       // so we just warn it.
       OTS_WARNING("tags aren't arranged alphabetically.");
     }
     last_tag = record.tag;
     if (record.offset < script_record_end || record.offset >= length) {
-      return OTS_FAILURE_MSG("Bad record offset %d for script %c%c%c%c entry %d in script list table", record.offset, OTS_UNTAG(record.tag), i);
+      return Error("Bad record offset %d for script %c%c%c%c entry %d in script list table", record.offset, OTS_UNTAG(record.tag), i);
     }
     script_list.push_back(record);
   }
   if (script_list.size() != script_count) {
-    return OTS_FAILURE_MSG("Bad script list size %ld in script list table", script_list.size());
+    return Error("Bad script list size %ld in script list table", script_list.size());
   }
 
   // Check script records.
   for (unsigned i = 0; i < script_count; ++i) {
     if (!ParseScriptTable(font, data + script_list[i].offset,
                           length - script_list[i].offset,
-                          script_list[i].tag, num_features)) {
-      return OTS_FAILURE_MSG("Failed to parse script table %d", i);
+                          script_list[i].tag, m_num_features)) {
+      return Error("Failed to parse script table %d", i);
     }
   }
 
   return true;
 }
 
 // Parsing FeatureListTable requires number of lookups so we need to parse
 // LookupListTable before calling this function.
-bool ParseFeatureListTable(const ots::Font *font,
-                           const uint8_t *data, const size_t length,
-                           const uint16_t num_lookups,
-                           uint16_t* num_features) {
+bool OpenTypeLayoutTable::ParseFeatureListTable(const uint8_t *data, const size_t length) {
+  Font *font = GetFont();
   Buffer subtable(data, length);
 
   uint16_t feature_count = 0;
   if (!subtable.ReadU16(&feature_count)) {
-    return OTS_FAILURE_MSG("Failed to read feature count");
+    return Error("Failed to read feature count");
   }
 
   std::vector<FeatureRecord> feature_records;
   feature_records.resize(feature_count);
   const unsigned feature_record_end =
       6 * static_cast<unsigned>(feature_count) + 2;
   if (feature_record_end > std::numeric_limits<uint16_t>::max()) {
-    return OTS_FAILURE_MSG("Bad end of feature record %d", feature_record_end);
+    return Error("Bad end of feature record %d", feature_record_end);
   }
   uint32_t last_tag = 0;
   for (unsigned i = 0; i < feature_count; ++i) {
     if (!subtable.ReadU32(&feature_records[i].tag) ||
         !subtable.ReadU16(&feature_records[i].offset)) {
-      return OTS_FAILURE_MSG("Failed to read feature header %d", i);
+      return Error("Failed to read feature header %d", i);
     }
     // Feature record array should be arranged alphabetically by tag
     if (last_tag != 0 && last_tag > feature_records[i].tag) {
       // Several fonts don't arrange tags alphabetically.
       // It seems that the order of tags might not be a security issue
       // so we just warn it.
       OTS_WARNING("tags aren't arranged alphabetically.");
     }
     last_tag = feature_records[i].tag;
     if (feature_records[i].offset < feature_record_end ||
         feature_records[i].offset >= length) {
-      return OTS_FAILURE_MSG("Bad feature offset %d for feature %d %c%c%c%c", feature_records[i].offset, i, OTS_UNTAG(feature_records[i].tag));
+      return Error("Bad feature offset %d for feature %d %c%c%c%c", feature_records[i].offset, i, OTS_UNTAG(feature_records[i].tag));
     }
   }
 
   for (unsigned i = 0; i < feature_count; ++i) {
     if (!ParseFeatureTable(font, data + feature_records[i].offset,
-                           length - feature_records[i].offset, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse feature table %d", i);
+                           length - feature_records[i].offset, m_num_lookups)) {
+      return Error("Failed to parse feature table %d", i);
+    }
+  }
+  m_num_features = feature_count;
+  return true;
+}
+
+bool OpenTypeLayoutTable::ParseLookupTable(const uint8_t *data,
+                                           const size_t length) {
+  Font* font = GetFont(); 
+  Buffer subtable(data, length);
+
+  uint16_t lookup_type = 0;
+  uint16_t lookup_flag = 0;
+  uint16_t subtable_count = 0;
+  if (!subtable.ReadU16(&lookup_type) ||
+      !subtable.ReadU16(&lookup_flag) ||
+      !subtable.ReadU16(&subtable_count)) {
+    return Error("Failed to read lookup table header");
+  }
+
+  if (!ValidLookupSubtableType(lookup_type)) {
+    return Error("Bad lookup type %d", lookup_type);
+  }
+
+  bool use_mark_filtering_set = lookup_flag & kUseMarkFilteringSetBit;
+
+  std::vector<uint16_t> subtables;
+  subtables.reserve(subtable_count);
+  // If the |kUseMarkFilteringSetBit| of |lookup_flag| is set,
+  // extra 2 bytes will follow after subtable offset array.
+  const unsigned lookup_table_end = 2 * static_cast<unsigned>(subtable_count) +
+      (use_mark_filtering_set ? 8 : 6);
+  if (lookup_table_end > std::numeric_limits<uint16_t>::max()) {
+    return Error("Bad end of lookup %d", lookup_table_end);
+  }
+  for (unsigned i = 0; i < subtable_count; ++i) {
+    uint16_t offset_subtable = 0;
+    if (!subtable.ReadU16(&offset_subtable)) {
+      return Error("Failed to read subtable offset %d", i);
+    }
+    if (offset_subtable < lookup_table_end ||
+        offset_subtable >= length) {
+      return Error("Bad subtable offset %d for subtable %d", offset_subtable, i);
+    }
+    subtables.push_back(offset_subtable);
+  }
+  if (subtables.size() != subtable_count) {
+    return Error("Bad subtable size %ld", subtables.size());
+  }
+
+  if (use_mark_filtering_set) {
+    uint16_t mark_filtering_set = 0;
+    if (!subtable.ReadU16(&mark_filtering_set)) {
+      return Error("Failed to read mark filtering set");
+    }
+
+    OpenTypeGDEF *gdef = static_cast<OpenTypeGDEF*>(
+        font->GetTypedTable(OTS_TAG_GDEF));
+
+    if (gdef && (gdef->num_mark_glyph_sets == 0 ||
+        mark_filtering_set >= gdef->num_mark_glyph_sets)) {
+      return Error("Bad mark filtering set %d", mark_filtering_set);
+    }
+  }
+
+  // Parse lookup subtables for this lookup type.
+  for (unsigned i = 0; i < subtable_count; ++i) {
+    if (!ParseLookupSubtable(data + subtables[i], length - subtables[i],
+                             lookup_type)) {
+      return Error("Failed to parse subtable %d", i);
     }
   }
-  *num_features = feature_count;
   return true;
 }
 
 // For parsing GPOS/GSUB tables, this function should be called at first to
 // obtain the number of lookups because parsing FeatureTableList requires
 // the number.
-bool ParseLookupListTable(Font *font, const uint8_t *data,
-                          const size_t length,
-                          const LookupSubtableParser* parser,
-                          uint16_t *num_lookups) {
+bool OpenTypeLayoutTable::ParseLookupListTable(const uint8_t *data,
+                                               const size_t length) {
   Buffer subtable(data, length);
 
-  if (!subtable.ReadU16(num_lookups)) {
-    return OTS_FAILURE_MSG("Failed to read number of lookups");
+  if (!subtable.ReadU16(&m_num_lookups)) {
+    return Error("Failed to read number of lookups");
   }
 
   std::vector<uint16_t> lookups;
-  lookups.reserve(*num_lookups);
+  lookups.reserve(m_num_lookups);
   const unsigned lookup_end =
-      2 * static_cast<unsigned>(*num_lookups) + 2;
+      2 * static_cast<unsigned>(m_num_lookups) + 2;
   if (lookup_end > std::numeric_limits<uint16_t>::max()) {
-    return OTS_FAILURE_MSG("Bad end of lookups %d", lookup_end);
+    return Error("Bad end of lookups %d", lookup_end);
   }
-  for (unsigned i = 0; i < *num_lookups; ++i) {
+  for (unsigned i = 0; i < m_num_lookups; ++i) {
     uint16_t offset = 0;
     if (!subtable.ReadU16(&offset)) {
-      return OTS_FAILURE_MSG("Failed to read lookup offset %d", i);
+      return Error("Failed to read lookup offset %d", i);
     }
     if (offset < lookup_end || offset >= length) {
-      return OTS_FAILURE_MSG("Bad lookup offset %d for lookup %d", offset, i);
+      return Error("Bad lookup offset %d for lookup %d", offset, i);
     }
     lookups.push_back(offset);
   }
-  if (lookups.size() != *num_lookups) {
-    return OTS_FAILURE_MSG("Bad lookup offsets list size %ld", lookups.size());
+  if (lookups.size() != m_num_lookups) {
+    return Error("Bad lookup offsets list size %ld", lookups.size());
   }
 
-  for (unsigned i = 0; i < *num_lookups; ++i) {
-    if (!ParseLookupTable(font, data + lookups[i], length - lookups[i],
-                          parser)) {
-      return OTS_FAILURE_MSG("Failed to parse lookup %d", i);
+  for (unsigned i = 0; i < m_num_lookups; ++i) {
+    if (!ParseLookupTable(data + lookups[i], length - lookups[i])) {
+      return Error("Failed to parse lookup %d", i);
     }
   }
 
   return true;
 }
 
 bool ParseClassDefTable(const ots::Font *font,
@@ -1402,275 +1468,268 @@
   // arbitrary values.
   if (!subtable.Skip(num_units * 2)) {
     return OTS_FAILURE_MSG("Failed to skip data in device table");
   }
   return true;
 }
 
-bool ParseContextSubtable(const ots::Font *font,
-                          const uint8_t *data, const size_t length,
-                          const uint16_t num_glyphs,
-                          const uint16_t num_lookups) {
+bool OpenTypeLayoutTable::ParseContextSubtable(const uint8_t *data,
+                                               const size_t length) {
+  Font *font = GetFont();
   Buffer subtable(data, length);
 
   uint16_t format = 0;
   if (!subtable.ReadU16(&format)) {
-    return OTS_FAILURE_MSG("Failed to read context subtable format");
+    return Error("Failed to read context subtable format");
+  }
+
+  OpenTypeMAXP *maxp = static_cast<OpenTypeMAXP*>(
+      font->GetTypedTable(OTS_TAG_MAXP));
+  if (!maxp) {
+    return Error("Required maxp table missing");
   }
 
   if (format == 1) {
-    if (!ParseContextFormat1(font, data, length, num_glyphs, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse context format 1 subtable");
+    if (!ParseContextFormat1(font, data, length, maxp->num_glyphs, m_num_lookups)) {
+      return Error("Failed to parse context format 1 subtable");
     }
   } else if (format == 2) {
-    if (!ParseContextFormat2(font, data, length, num_glyphs, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse context format 2 subtable");
+    if (!ParseContextFormat2(font, data, length, maxp->num_glyphs, m_num_lookups)) {
+      return Error("Failed to parse context format 2 subtable");
     }
   } else if (format == 3) {
-    if (!ParseContextFormat3(font, data, length, num_glyphs, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse context format 3 subtable");
+    if (!ParseContextFormat3(font, data, length, maxp->num_glyphs, m_num_lookups)) {
+      return Error("Failed to parse context format 3 subtable");
     }
   } else {
-    return OTS_FAILURE_MSG("Bad context subtable format %d", format);
+    return Error("Bad context subtable format %d", format);
   }
 
   return true;
 }
 
-bool ParseChainingContextSubtable(const ots::Font *font,
-                                  const uint8_t *data, const size_t length,
-                                  const uint16_t num_glyphs,
-                                  const uint16_t num_lookups) {
+bool OpenTypeLayoutTable::ParseChainingContextSubtable(const uint8_t *data,
+                                                       const size_t length) {
+  Font *font = GetFont();
   Buffer subtable(data, length);
 
   uint16_t format = 0;
   if (!subtable.ReadU16(&format)) {
-    return OTS_FAILURE_MSG("Failed to read chaining context subtable format");
+    return Error("Failed to read chaining context subtable format");
+  }
+
+  OpenTypeMAXP *maxp = static_cast<OpenTypeMAXP*>(
+      font->GetTypedTable(OTS_TAG_MAXP));
+  if (!maxp) {
+    return Error("Required maxp table missing");
   }
 
   if (format == 1) {
-    if (!ParseChainContextFormat1(font, data, length, num_glyphs, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse chaining context format 1 subtable");
+    if (!ParseChainContextFormat1(font, data, length, maxp->num_glyphs, m_num_lookups)) {
+      return Error("Failed to parse chaining context format 1 subtable");
     }
   } else if (format == 2) {
-    if (!ParseChainContextFormat2(font, data, length, num_glyphs, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse chaining context format 2 subtable");
+    if (!ParseChainContextFormat2(font, data, length, maxp->num_glyphs, m_num_lookups)) {
+      return Error("Failed to parse chaining context format 2 subtable");
     }
   } else if (format == 3) {
-    if (!ParseChainContextFormat3(font, data, length, num_glyphs, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse chaining context format 3 subtable");
+    if (!ParseChainContextFormat3(font, data, length, maxp->num_glyphs, m_num_lookups)) {
+      return Error("Failed to parse chaining context format 3 subtable");
     }
   } else {
-    return OTS_FAILURE_MSG("Bad chaining context subtable format %d", format);
+    return Error("Bad chaining context subtable format %d", format);
   }
 
   return true;
 }
 
-bool ParseExtensionSubtable(const Font *font,
-                            const uint8_t *data, const size_t length,
-                            const LookupSubtableParser* parser) {
+bool OpenTypeLayoutTable::ParseExtensionSubtable(const uint8_t *data,
+                                                 const size_t length) {
   Buffer subtable(data, length);
 
   uint16_t format = 0;
   uint16_t lookup_type = 0;
   uint32_t offset_extension = 0;
   if (!subtable.ReadU16(&format) ||
       !subtable.ReadU16(&lookup_type) ||
       !subtable.ReadU32(&offset_extension)) {
-    return OTS_FAILURE_MSG("Failed to read extension table header");
+    return Error("Failed to read extension table header");
   }
 
   if (format != 1) {
-    return OTS_FAILURE_MSG("Bad extension table format %d", format);
+    return Error("Bad extension table format %d", format);
   }
   // |lookup_type| should be other than |parser->extension_type|.
-  if (lookup_type < 1 || lookup_type > parser->num_types ||
-      lookup_type == parser->extension_type) {
-    return OTS_FAILURE_MSG("Bad lookup type %d in extension table", lookup_type);
+  if (!ValidLookupSubtableType(lookup_type, true)) {
+    return Error("Bad lookup type %d in extension table", lookup_type);
   }
 
   const unsigned format_end = static_cast<unsigned>(8);
   if (offset_extension < format_end ||
       offset_extension >= length) {
-    return OTS_FAILURE_MSG("Bad extension offset %d", offset_extension);
+    return Error("Bad extension offset %d", offset_extension);
   }
 
   // Parse the extension subtable of |lookup_type|.
-  if (!parser->Parse(font, data + offset_extension, length - offset_extension,
-                     lookup_type)) {
-    return OTS_FAILURE_MSG("Failed to parse lookup from extension lookup");
-  }
-
-  return true;
-}
-
-bool ParseConditionTable(const Font *font,
-                         const uint8_t *data, const size_t length,
-                         const uint16_t axis_count) {
-  Buffer subtable(data, length);
-
-  uint16_t format = 0;
-  if (!subtable.ReadU16(&format)) {
-    return OTS_FAILURE_MSG("Failed to read condition table format");
-  }
-
-  if (format != 1) {
-    // An unknown format is not an error, but should be ignored per spec.
-    return true;
-  }
-
-  uint16_t axis_index = 0;
-  int16_t filter_range_min_value = 0;
-  int16_t filter_range_max_value = 0;
-  if (!subtable.ReadU16(&axis_index) ||
-      !subtable.ReadS16(&filter_range_min_value) ||
-      !subtable.ReadS16(&filter_range_max_value)) {
-    return OTS_FAILURE_MSG("Failed to read condition table (format 1)");
-  }
-
-  if (axis_index >= axis_count) {
-    return OTS_FAILURE_MSG("Axis index out of range in condition");
-  }
-
-  // Check min/max values are within range -1.0 .. 1.0 and properly ordered
-  if (filter_range_min_value < -0x4000 || // -1.0 in F2DOT14 format
-      filter_range_max_value > 0x4000 || // +1.0 in F2DOT14 format
-      filter_range_min_value > filter_range_max_value) {
-    return OTS_FAILURE_MSG("Invalid filter range in condition");
+  if (!ParseLookupSubtable(data + offset_extension, length - offset_extension,
+                           lookup_type)) {
+    return Error("Failed to parse lookup from extension lookup");
   }
 
   return true;
 }
 
-bool ParseConditionSetTable(const Font *font,
-                            const uint8_t *data, const size_t length,
-                            const uint16_t axis_count) {
-  Buffer subtable(data, length);
-
-  uint16_t condition_count = 0;
-  if (!subtable.ReadU16(&condition_count)) {
-    return OTS_FAILURE_MSG("Failed to read condition count");
-  }
-
-  for (uint16_t i = 0; i < condition_count; i++) {
-    uint32_t condition_offset = 0;
-    if (!subtable.ReadU32(&condition_offset)) {
-      return OTS_FAILURE_MSG("Failed to read condition offset");
-    }
-    if (condition_offset < subtable.offset() || condition_offset >= length) {
-      return OTS_FAILURE_MSG("Offset out of range");
-    }
-    if (!ParseConditionTable(font, data + condition_offset, length - condition_offset,
-                             axis_count)) {
-      return OTS_FAILURE_MSG("Failed to parse condition table");
-    }
-  }
-
-  return true;
-}
-
-bool ParseFeatureTableSubstitutionTable(const Font *font,
-                                        const uint8_t *data, const size_t length,
-                                        const uint16_t num_lookups) {
-  Buffer subtable(data, length);
-
-  uint16_t version_major = 0;
-  uint16_t version_minor = 0;
-  uint16_t substitution_count = 0;
-  const size_t kFeatureTableSubstitutionHeaderSize = 3 * sizeof(uint16_t);
-
-  if (!subtable.ReadU16(&version_major) ||
-      !subtable.ReadU16(&version_minor) ||
-      !subtable.ReadU16(&substitution_count)) {
-    return OTS_FAILURE_MSG("Failed to read feature table substitution table header");
-  }
-
-  for (uint16_t i = 0; i < substitution_count; i++) {
-    uint16_t feature_index = 0;
-    uint32_t alternate_feature_table_offset = 0;
-    const size_t kFeatureTableSubstitutionRecordSize = sizeof(uint16_t) + sizeof(uint32_t);
-
-    if (!subtable.ReadU16(&feature_index) ||
-        !subtable.ReadU32(&alternate_feature_table_offset)) {
-      return OTS_FAILURE_MSG("Failed to read feature table substitution record");
-    }
-
-    if (alternate_feature_table_offset < kFeatureTableSubstitutionHeaderSize +
-                                         kFeatureTableSubstitutionRecordSize * substitution_count ||
-        alternate_feature_table_offset >= length) {
-      return OTS_FAILURE_MSG("Invalid alternate feature table offset");
-    }
-
-    if (!ParseFeatureTable(font, data + alternate_feature_table_offset,
-                           length - alternate_feature_table_offset, num_lookups)) {
-      return OTS_FAILURE_MSG("Failed to parse alternate feature table");
-    }
-  }
-
-  return true;
-}
-
-bool ParseFeatureVariationsTable(const Font *font,
-                                 const uint8_t *data, const size_t length,
-                                 const uint16_t num_lookups) {
+// Parsing feature variations table (in GSUB/GPOS v1.1)
+bool OpenTypeLayoutTable::ParseFeatureVariationsTable(const uint8_t *data, const size_t length) {
+  Font *font = GetFont();
   Buffer subtable(data, length);
 
   uint16_t version_major = 0;
   uint16_t version_minor = 0;
   uint32_t feature_variation_record_count = 0;
 
   if (!subtable.ReadU16(&version_major) ||
       !subtable.ReadU16(&version_minor) ||
       !subtable.ReadU32(&feature_variation_record_count)) {
-    return OTS_FAILURE_MSG("Failed to read feature variations table header");
+    return Error("Failed to read feature variations table header");
   }
 
   OpenTypeFVAR* fvar = static_cast<OpenTypeFVAR*>(font->GetTypedTable(OTS_TAG_FVAR));
   if (!fvar) {
-    return OTS_FAILURE_MSG("Not a variation font");
+    return Error("Not a variation font");
   }
   const uint16_t axis_count = fvar->AxisCount();
 
   const size_t kEndOfFeatureVariationRecords =
     2 * sizeof(uint16_t) + sizeof(uint32_t) +
     feature_variation_record_count * 2 * sizeof(uint32_t);
 
   for (uint32_t i = 0; i < feature_variation_record_count; i++) {
     uint32_t condition_set_offset = 0;
     uint32_t feature_table_substitution_offset = 0;
     if (!subtable.ReadU32(&condition_set_offset) ||
         !subtable.ReadU32(&feature_table_substitution_offset)) {
-      return OTS_FAILURE_MSG("Failed to read feature variation record");
+      return Error("Failed to read feature variation record");
     }
 
     if (condition_set_offset) {
       if (condition_set_offset < kEndOfFeatureVariationRecords ||
           condition_set_offset >= length) {
-        return OTS_FAILURE_MSG("Condition set offset out of range");
+        return Error("Condition set offset out of range");
       }
       if (!ParseConditionSetTable(font, data + condition_set_offset,
                                   length - condition_set_offset,
                                   axis_count)) {
-        return OTS_FAILURE_MSG("Failed to parse condition set table");
+        return Error("Failed to parse condition set table");
       }
     }
 
     if (feature_table_substitution_offset) {
       if (feature_table_substitution_offset < kEndOfFeatureVariationRecords ||
           feature_table_substitution_offset >= length) {
-        return OTS_FAILURE_MSG("Feature table substitution offset out of range");
+        return Error("Feature table substitution offset out of range");
       }
       if (!ParseFeatureTableSubstitutionTable(font, data + feature_table_substitution_offset,
                                               length - feature_table_substitution_offset,
-                                              num_lookups)) {
-        return OTS_FAILURE_MSG("Failed to parse feature table substitution table");
+                                              m_num_lookups)) {
+        return Error("Failed to parse feature table substitution table");
       }
     }
   }
 
   return true;
 }
 
+// GSUB/GPOS header size for table version 1.0
+const size_t kHeaderSize_1_0 = 4 + 3 * 2;
+// GSUB/GPOS header size for table versio 1.1
+const size_t kHeaderSize_1_1 = 4 + 3 * 2 + 4;
+
+bool OpenTypeLayoutTable::Parse(const uint8_t *data, size_t length) {
+  Buffer table(data, length);
+
+  uint16_t version_major = 0, version_minor = 0;
+  uint16_t offset_script_list = 0;
+  uint16_t offset_feature_list = 0;
+  uint16_t offset_lookup_list = 0;
+  uint32_t offset_feature_variations = 0;
+  if (!table.ReadU16(&version_major) ||
+      !table.ReadU16(&version_minor) ||
+      !table.ReadU16(&offset_script_list) ||
+      !table.ReadU16(&offset_feature_list) ||
+      !table.ReadU16(&offset_lookup_list)) {
+    return Error("Incomplete table");
+  }
+
+  if (version_major != 1 || version_minor > 1) {
+    return Error("Bad version");
+  }
+
+  if (version_minor > 0) {
+    if (!table.ReadU32(&offset_feature_variations)) {
+      return Error("Incomplete table");
+    }
+  }
+
+  const size_t header_size =
+    (version_minor == 0) ? kHeaderSize_1_0 : kHeaderSize_1_1;
+
+  if (offset_lookup_list) {
+    if (offset_lookup_list < header_size || offset_lookup_list >= length) {
+      return Error("Bad lookup list offset in table header");
+    }
+
+    if (!ParseLookupListTable(data + offset_lookup_list,
+                              length - offset_lookup_list)) {
+      return Error("Failed to parse lookup list table");
+    }
+  }
+
+  if (offset_feature_list) {
+    if (offset_feature_list < header_size || offset_feature_list >= length) {
+      return Error("Bad feature list offset in table header");
+    }
+
+    if (!ParseFeatureListTable(data + offset_feature_list,
+                               length - offset_feature_list)) {
+      return Error("Failed to parse feature list table");
+    }
+  }
+
+  if (offset_script_list) {
+    if (offset_script_list < header_size || offset_script_list >= length) {
+      return Error("Bad script list offset in table header");
+    }
+
+    if (!ParseScriptListTable(data + offset_script_list,
+                              length - offset_script_list)) {
+      return Error("Failed to parse script list table");
+    }
+  }
+
+  if (offset_feature_variations) {
+    if (offset_feature_variations < header_size || offset_feature_variations >= length) {
+      return Error("Bad feature variations offset in table header");
+    }
+
+    if (!ParseFeatureVariationsTable(data + offset_feature_variations,
+                                     length - offset_feature_variations)) {
+      return Error("Failed to parse feature variations table");
+    }
+  }
+
+  this->m_data = data;
+  this->m_length = length;
+  return true;
+}
+
+bool OpenTypeLayoutTable::Serialize(OTSStream *out) {
+  if (!out->Write(this->m_data, this->m_length)) {
+    return Error("Failed to write table");
+  }
+
+  return true;
+}
+
 }  // namespace ots
 
 #undef TABLE_NAME
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/loca.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/loca.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/loca.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/loca.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/ltsh.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/ltsh.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/ltsh.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/ltsh.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/math.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/math.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/math_.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/math_.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/maxp.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/maxp.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/maxp.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/maxp.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/metrics.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/metrics.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/metrics.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/metrics.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/mvar.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/mvar.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/mvar.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/vvar.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 // Copyright (c) 2018 The OTS Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
-#ifndef OTS_MVAR_H_
-#define OTS_MVAR_H_
+#ifndef OTS_VVAR_H_
+#define OTS_VVAR_H_
 
 #include "ots.h"
 
 namespace ots {
 
 // -----------------------------------------------------------------------------
-// OpenTypeMVAR Interface
+// OpenTypeVVAR Interface
 // -----------------------------------------------------------------------------
 
-class OpenTypeMVAR : public Table {
+class OpenTypeVVAR : public Table {
  public:
-  explicit OpenTypeMVAR(Font* font, uint32_t tag)
+  explicit OpenTypeVVAR(Font* font, uint32_t tag)
       : Table(font, tag, tag) { }
 
   bool Parse(const uint8_t* data, size_t length);
   bool Serialize(OTSStream* out);
 
  private:
   const uint8_t *m_data;
   size_t m_length;
 };
 
 }  // namespace ots
 
-#endif  // OTS_MVAR_H_
+#endif  // OTS_VVAR_H_
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/name.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/name.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/name.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/name.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/os2.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/os2.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/os2.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/os2.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/ots.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/ots.cc`

 * *Files 3% similar despite different names*

```diff
@@ -733,14 +733,35 @@
     if (!font->GetTable(table_entry.tag)) {
       if (!font->ParseTable(table_entry, data, arena)) {
         return OTS_FAILURE_MSG_TAG("Failed to parse table", table_entry.tag);
       }
     }
   }
 
+#ifdef OTS_SYNTHESIZE_MISSING_GVAR
+  // If there was an fvar table but no gvar, synthesize an empty gvar to avoid
+  // issues with rasterizers (e.g. Core Text) that assume it must be present.
+  if (font->GetTable(OTS_TAG_FVAR) && !font->GetTable(OTS_TAG_GVAR)) {
+    ots::TableEntry table_entry{ OTS_TAG_GVAR, 0, 0, 0, 0 };
+    const auto &it = font->file->tables.find(table_entry);
+    if (it != font->file->tables.end()) {
+      table_map[OTS_TAG_GVAR] = table_entry;
+      font->AddTable(table_entry, it->second);
+    } else {
+      ots::OpenTypeGVAR *gvar = new ots::OpenTypeGVAR(font, OTS_TAG_GVAR);
+      if (gvar->InitEmpty()) {
+        table_map[OTS_TAG_GVAR] = table_entry;
+        font->AddTable(table_entry, gvar);
+      } else {
+        delete gvar;
+      }
+    }
+  }
+#endif
+
   ots::Table *glyf = font->GetTable(OTS_TAG_GLYF);
   ots::Table *loca = font->GetTable(OTS_TAG_LOCA);
   ots::Table *cff  = font->GetTable(OTS_TAG_CFF);
   ots::Table *cff2 = font->GetTable(OTS_TAG_CFF2);
 
   if (glyf && loca) {
     if (font->version != 0x000010000) {
@@ -885,14 +906,40 @@
   if (!output->Seek(end_of_file)) {
     return OTS_FAILURE_MSG_HDR("error writing output");
   }
 
   return true;
 }
 
+bool IsGraphiteTag(uint32_t tag) {
+  if (tag == OTS_TAG_FEAT ||
+      tag == OTS_TAG_GLAT ||
+      tag == OTS_TAG_GLOC ||
+      tag == OTS_TAG_SILE ||
+      tag == OTS_TAG_SILF ||
+      tag == OTS_TAG_SILL) {
+    return true;
+  }
+  return false;
+}
+
+bool IsVariationsTag(uint32_t tag) {
+  if (tag == OTS_TAG_AVAR ||
+      tag == OTS_TAG_CVAR ||
+      tag == OTS_TAG_FVAR ||
+      tag == OTS_TAG_GVAR ||
+      tag == OTS_TAG_HVAR ||
+      tag == OTS_TAG_MVAR ||
+      tag == OTS_TAG_STAT ||
+      tag == OTS_TAG_VVAR) {
+    return true;
+  }
+  return false;
+}
+
 }  // namespace
 
 namespace ots {
 
 FontFile::~FontFile() {
   for (const auto& it : tables) {
     delete it.second;
@@ -973,22 +1020,17 @@
 
   if (table) {
     const uint8_t* table_data;
     size_t table_length;
 
     ret = GetTableData(data, table_entry, arena, &table_length, &table_data);
     if (ret) {
-      // FIXME: Parsing some tables will fail if the table is not added to
-      // m_tables first.
-      m_tables[tag] = table;
       ret = table->Parse(table_data, table_length);
       if (ret)
-        file->tables[table_entry] = table;
-      else
-        m_tables.erase(tag);
+        AddTable(table_entry, table);
     }
   }
 
   if (!ret)
     delete table;
 
   return ret;
@@ -1004,39 +1046,35 @@
 Table* Font::GetTypedTable(uint32_t tag) const {
   Table* t = GetTable(tag);
   if (t && t->Type() == tag)
     return t;
   return NULL;
 }
 
+void Font::AddTable(TableEntry entry, Table* table) {
+  // Attempting to add a duplicate table would be an error; this should only
+  // be used to add a table that does not already exist.
+  assert(m_tables.find(table->Tag()) == m_tables.end());
+  m_tables[table->Tag()] = table;
+  file->tables[entry] = table;
+}
+
 void Font::DropGraphite() {
   file->context->Message(0, "Dropping all Graphite tables");
   for (const std::pair<uint32_t, Table*> entry : m_tables) {
-    if (entry.first == OTS_TAG_FEAT ||
-        entry.first == OTS_TAG_GLAT ||
-        entry.first == OTS_TAG_GLOC ||
-        entry.first == OTS_TAG_SILE ||
-        entry.first == OTS_TAG_SILF ||
-        entry.first == OTS_TAG_SILL) {
+    if (IsGraphiteTag(entry.first)) {
       entry.second->Drop("Discarding Graphite table");
     }
   }
 }
 
 void Font::DropVariations() {
   file->context->Message(0, "Dropping all Variation tables");
   for (const std::pair<uint32_t, Table*> entry : m_tables) {
-    if (entry.first == OTS_TAG_AVAR ||
-        entry.first == OTS_TAG_CVAR ||
-        entry.first == OTS_TAG_FVAR ||
-        entry.first == OTS_TAG_GVAR ||
-        entry.first == OTS_TAG_HVAR ||
-        entry.first == OTS_TAG_MVAR ||
-        entry.first == OTS_TAG_STAT ||
-        entry.first == OTS_TAG_VVAR) {
+    if (IsVariationsTag(entry.first)) {
       entry.second->Drop("Discarding Variations table");
     }
   }
 }
 
 bool Table::ShouldSerialize() {
   return m_shouldSerialize;
@@ -1081,24 +1119,30 @@
 bool Table::DropGraphite(const char *format, ...) {
   va_list va;
   va_start(va, format);
   Message(0, format, va);
   va_end(va);
 
   m_font->DropGraphite();
+  if (IsGraphiteTag(m_tag))
+      Drop("Discarding Graphite table");
+
   return true;
 }
 
 bool Table::DropVariations(const char *format, ...) {
   va_list va;
   va_start(va, format);
   Message(0, format, va);
   va_end(va);
 
   m_font->DropVariations();
+  if (IsVariationsTag(m_tag))
+      Drop("Discarding Variations table");
+
   return true;
 }
 
 bool TablePassthru::Parse(const uint8_t *data, size_t length) {
   m_data = data;
   m_length = length;
   return true;
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/ots.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/ots.h`

 * *Files 6% similar despite different names*

```diff
@@ -259,14 +259,17 @@
   // Return the tag (table type) this Table was parsed as, to support
   // "poor man's RTTI" so that we know if we can safely down-cast to
   // a specific Table subclass. The m_type field is initialized to the
   // appropriate tag when a subclass is constructed, or to zero for
   // TablePassthru (indicating unparsed data).
   uint32_t Type() { return m_type; }
 
+  // Return the tag assigned when this table was constructed.
+  uint32_t Tag() { return m_tag; }
+
   Font* GetFont() { return m_font; }
 
   bool Error(const char *format, ...);
   bool Warning(const char *format, ...);
   bool Drop(const char *format, ...);
   bool DropGraphite(const char *format, ...);
   bool DropVariations(const char *format, ...);
@@ -311,14 +314,17 @@
   Table* GetTable(uint32_t tag) const;
 
   // This checks that the returned Table is actually of the correct subclass
   // for |tag|, so it can safely be downcast to the corresponding OpenTypeXXXX;
   // if not (i.e. if the table was treated as Passthru), it will return NULL.
   Table* GetTypedTable(uint32_t tag) const;
 
+  // Insert a new table. Asserts if a table with the same tag already exists.
+  void AddTable(TableEntry entry, Table* table);
+
   // Drop all Graphite tables and don't parse new ones.
   void DropGraphite();
 
   // Drop all Variations tables and don't parse new ones.
   void DropVariations();
 
   FontFile *file;
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/post.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/post.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/post.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/post.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/prep.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/prep.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/prep.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/sile.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 // Copyright (c) 2009-2017 The OTS Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
-#ifndef OTS_PREP_H_
-#define OTS_PREP_H_
+#ifndef OTS_SILE_H_
+#define OTS_SILE_H_
 
 #include "ots.h"
+#include "graphite.h"
+
+#include <vector>
 
 namespace ots {
 
-class OpenTypePREP : public Table {
+class OpenTypeSILE : public Table {
  public:
-  explicit OpenTypePREP(Font *font, uint32_t tag)
+  explicit OpenTypeSILE(Font* font, uint32_t tag)
       : Table(font, tag, tag) { }
 
-  bool Parse(const uint8_t *data, size_t length);
-  bool Serialize(OTSStream *out);
-  bool ShouldSerialize();
+  bool Parse(const uint8_t* data, size_t length);
+  bool Serialize(OTSStream* out);
 
  private:
-  const uint8_t *m_data;
-  uint32_t m_length;
+  uint32_t version;
+  uint32_t checksum;
+  uint32_t createTime[2];
+  uint32_t modifyTime[2];
+  uint16_t fontNameLength;
+  std::vector<uint16_t> fontName;
+  uint16_t fontFileLength;
+  std::vector<uint16_t> baseFile;
 };
 
 }  // namespace ots
 
-#endif  // OTS_PREP_H_
+#endif  // OTS_SILE_H_
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/sile.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/sile.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/sile.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/vorg.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 // Copyright (c) 2009-2017 The OTS Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
-#ifndef OTS_SILE_H_
-#define OTS_SILE_H_
-
-#include "ots.h"
-#include "graphite.h"
+#ifndef OTS_VORG_H_
+#define OTS_VORG_H_
 
 #include <vector>
 
+#include "ots.h"
+
 namespace ots {
 
-class OpenTypeSILE : public Table {
+struct OpenTypeVORGMetrics {
+  uint16_t glyph_index;
+  int16_t vert_origin_y;
+};
+
+class OpenTypeVORG : public Table {
  public:
-  explicit OpenTypeSILE(Font* font, uint32_t tag)
+  explicit OpenTypeVORG(Font *font, uint32_t tag)
       : Table(font, tag, tag) { }
 
-  bool Parse(const uint8_t* data, size_t length);
-  bool Serialize(OTSStream* out);
+  bool Parse(const uint8_t *data, size_t length);
+  bool Serialize(OTSStream *out);
+  bool ShouldSerialize();
 
  private:
-  uint32_t version;
-  uint32_t checksum;
-  uint32_t createTime[2];
-  uint32_t modifyTime[2];
-  uint16_t fontNameLength;
-  std::vector<uint16_t> fontName;
-  uint16_t fontFileLength;
-  std::vector<uint16_t> baseFile;
+  uint16_t major_version;
+  uint16_t minor_version;
+  int16_t default_vert_origin_y;
+  std::vector<OpenTypeVORGMetrics> metrics;
 };
 
 }  // namespace ots
 
-#endif  // OTS_SILE_H_
+#endif  // OTS_VORG_H_
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/silf.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/silf.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/silf.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/silf.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/sill.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/sill.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/sill.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/sill.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/stat.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/stat.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/stat.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/stat.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/variations.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/variations.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/variations.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/variations.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/vdmx.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/vdmx.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 // Copyright (c) 2009-2017 The OTS Authors. All rights reserved.
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
 #include "vdmx.h"
 
+#include <set>
+
 // VDMX - Vertical Device Metrics
 // http://www.microsoft.com/typography/otspec/vdmx.htm
 
 namespace ots {
 
+#define TABLE_NAME "VDMX"
+
 bool OpenTypeVDMX::Parse(const uint8_t *data, size_t length) {
   Buffer table(data, length);
+  ots::Font* font = this->GetFont();
 
   if (!table.ReadU16(&this->version) ||
       !table.ReadU16(&this->num_recs) ||
       !table.ReadU16(&this->num_ratios)) {
-    return Error("Failed to read table header");
+    return Drop("Failed to read table header");
   }
 
   if (this->version > 1) {
     return Drop("Unsupported table version: %u", this->version);
   }
 
   this->rat_ranges.reserve(this->num_ratios);
   for (unsigned i = 0; i < this->num_ratios; ++i) {
     OpenTypeVDMXRatioRecord rec;
 
     if (!table.ReadU8(&rec.charset) ||
         !table.ReadU8(&rec.x_ratio) ||
         !table.ReadU8(&rec.y_start_ratio) ||
         !table.ReadU8(&rec.y_end_ratio)) {
-      return Error("Failed to read RatioRange record %d", i);
+      return Drop("Failed to read RatioRange record %d", i);
     }
 
     if (rec.charset > 1) {
       return Drop("Unsupported character set: %u", rec.charset);
     }
 
     if (rec.y_start_ratio > rec.y_end_ratio) {
@@ -52,42 +57,53 @@
     }
 
     this->rat_ranges.push_back(rec);
   }
 
   this->offsets.reserve(this->num_ratios);
   const size_t current_offset = table.offset();
+  std::set<uint16_t> unique_offsets;
   // current_offset is less than (2 bytes * 3) + (4 bytes * USHRT_MAX) = 256k.
   for (unsigned i = 0; i < this->num_ratios; ++i) {
     uint16_t offset;
     if (!table.ReadU16(&offset)) {
-      return Error("Failed to read ratio offset %d", i);
+      return Drop("Failed to read ratio offset %d", i);
     }
     if (current_offset + offset >= length) {  // thus doesn't overflow.
-      return Error("Bad ratio offset %d for ration %d", offset, i);
+      return Drop("Bad ratio offset %d for ration %d", offset, i);
     }
 
     this->offsets.push_back(offset);
+    unique_offsets.insert(offset);
+  }
+
+  // Check that num_recs is sufficient to provide as many VDMXGroup records
+  // as there are unique offsets; if not, update it (we'll return an error
+  // below if they're not actually present).
+  if (unique_offsets.size() > this->num_recs) {
+    OTS_WARNING("increasing num_recs (%u is too small for %u unique offsets)",
+                this->num_recs, unique_offsets.size());
+    this->num_recs = unique_offsets.size();
   }
 
   this->groups.reserve(this->num_recs);
   for (unsigned i = 0; i < this->num_recs; ++i) {
     OpenTypeVDMXGroup group;
     if (!table.ReadU16(&group.recs) ||
         !table.ReadU8(&group.startsz) ||
         !table.ReadU8(&group.endsz)) {
-      return Error("Failed to read record header %d", i);
+      return Drop("Failed to read record header %d", i);
     }
     group.entries.reserve(group.recs);
     for (unsigned j = 0; j < group.recs; ++j) {
       OpenTypeVDMXVTable vt;
       if (!table.ReadU16(&vt.y_pel_height) ||
           !table.ReadS16(&vt.y_max) ||
           !table.ReadS16(&vt.y_min)) {
-        return Error("Failed to read reacord %d group %d", i, j);
+        return Drop("Failed to read record %d group %d", i, j);
       }
       if (vt.y_max < vt.y_min) {
         return Drop("bad y min/max");
       }
 
       // This table must appear in sorted order (sorted by yPelHeight),
       // but need not be continuous.
@@ -148,8 +164,10 @@
       }
     }
   }
 
   return true;
 }
 
+#undef TABLE_NAME
+
 }  // namespace ots
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/vdmx.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/vdmx.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/vhea.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/vhea.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/vhea.h` & `opentype-sanitizer-9.1.0/src/c/ots/src/vhea.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/vorg.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/vorg.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/src/vvar.cc` & `opentype-sanitizer-9.1.0/src/c/ots/src/vvar.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/subprojects/google-brotli.wrap` & `opentype-sanitizer-9.1.0/src/c/ots/subprojects/google-brotli.wrap`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/subprojects/google-woff2.wrap` & `opentype-sanitizer-9.1.0/src/c/ots/subprojects/google-woff2.wrap`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/subprojects/gtest.wrap` & `opentype-sanitizer-9.1.0/src/c/ots/subprojects/gtest.wrap`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/brotli/LICENSE.build` & `opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/brotli/LICENSE.build`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/brotli/meson.build` & `opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/brotli/meson.build`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/woff2/LICENSE.build` & `opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/woff2/LICENSE.build`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/subprojects/packagefiles/woff2/meson.build` & `opentype-sanitizer-9.1.0/src/c/ots/subprojects/packagefiles/woff2/meson.build`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/tests/cff_charstring_test.cc` & `opentype-sanitizer-9.1.0/src/c/ots/tests/cff_charstring_test.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/tests/meson.build` & `opentype-sanitizer-9.1.0/src/c/ots/tests/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,116 +1,118 @@
 good_fonts = [
   'fonts/good/00ae3c2b1b7718361fc76ee31da97253057b15b7.ttf',
   'fonts/good/01ae09f3a2ca8f33035e6261d09e9fe06b919174.ttf',
   'fonts/good/029c6e2623f5b255ba10e2e3b0f17711ad8aa966.ttf',
   'fonts/good/02d99e81593bcabce56b6a589254e8bc77e00208.otf',
+  'fonts/good/068aaf44acba22aa769fc7023b9b575fdf72c530.otf',
   'fonts/good/0c4afb23b983bbab65c39869b81ca1dfb90c0258.ttf',
   'fonts/good/0e16ec5ab94d3992bba42a9177b159113ede1485.ttf',
   'fonts/good/0fc088827bbe36bfb3fb6c3d8b59f66cb234dfb3.ttf',
   'fonts/good/1232d0423fe3bb731faa3da008281ca030d3fe0a.woff',
   'fonts/good/126e13890b4c36319166a07bb5f4301132e6dcee.ttf',
+  'fonts/good/14b84df95987d7ba699d058686e9163eb4ca5e75.ttf',
+  'fonts/good/1554deaab977f26747d651fa983988429bc0ebc5.ttf',
   'fonts/good/15e79042604b100fa6f93d817112b8f4921f6a4b.ttf',
   'fonts/good/164f99832db39451f53858175d6c2d251feb028c.ttf',
   'fonts/good/171ec9ef597e59a0f33cdeae1d4cf43af1d255ce.otf',
   'fonts/good/19d60aa144bb703f0c7535e3b34e926e0cae954d.ttf',
   'fonts/good/224f3a28601603e869da5ab0650148ae8cbadd2d.ttf',
   'fonts/good/24834cb0e118b8a80c05209d996963cf05121f43.ttf',
+  'fonts/good/27312d3d8d62bf7f3d2dec4afd90ac5549c05958.otf',
   'fonts/good/27f2cd91ff43713d977b2b253e82b8fcb781e674.otf',
   'fonts/good/2eba8164a0811c8422ecde8900bf476bb4a05ca3.otf',
   'fonts/good/2f806821ba44e69a532fbcc9d5f46a5aa20fa905.ttf',
   'fonts/good/322aa2ac0a3916d3a5cb1e7789ca355de0a6bc76.ttf',
+  'fonts/good/39b02c925a67188e7dd1fb9e78e7799976d8b6f6.otf',
   'fonts/good/3b4a0f922a35acba59502ba042f35cafbff1865f.ttf',
   'fonts/good/3eb899fa22c7a7e1294f50204804869fddfda8c9.ttf',
   'fonts/good/3ee1ab163f0029bdd8f90b79f2c0e798bc26957b.ttf',
+  'fonts/good/40acdfaee3c5f4fac5348001d8c54a9085623a24.ttf',
   'fonts/good/49331b1dd031e95ca803d632f69404d09ee6f592.ttf',
   'fonts/good/49a9db4b6c08dadd1e8aeff4cee63dc454c5cb7c.ttf',
   'fonts/good/4c471c403831e131c7887e9e0b9a547495749579.otf',
+  'fonts/good/4e5ac04a7e4638302443a8d9e3258772ccb60744.ttf',
+  'fonts/good/4e7747c985aa4f1b89f5f6c09f4ec4094bf1b20b.otf',
   'fonts/good/4fa1f484ba76ad1951727d8e4a80d57d9b08204b.ttf',
+  'fonts/good/54819458b3920c39db79d6e4cc8594e47654ca5f.otf',
   'fonts/good/56e62c1aa63b75291bd6c3bd04f29ee36590341f.ttf',
+  'fonts/good/5b376d5ec538bc3c86749e13a815661c7f5d9528.ttf',
+  'fonts/good/611dc1a20537abb29791dfdbf12ecb48afd94f53.otf',
   'fonts/good/6a20e627475700e4b889926fcc423420d6df3033.ttf',
   'fonts/good/6a46e85c50dce18db3a5739456933f29442e410e.ttf',
   'fonts/good/6ae5423c8ca52f5e20fc4be14d10ae0cd3857be5.ttf',
   'fonts/good/6bed910d67d00b0e705b657747af2b83f2edc1c5.ttf',
   'fonts/good/6c26e8ccc29afe595364bf649455d10dc0e39861.ttf',
+  'fonts/good/6d7ceee66a8d288d96ea235b1d642b75d96cafd5.otf',
   'fonts/good/759f24b9ab9a97980c5bb5649d9f5032fb9e41b0.ttf',
   'fonts/good/7cbb117642ab9715b476160b09b3e2fac33a91cb.ttf',
+  'fonts/good/7ef289b55de3392d9fca03735ea0a1c8498fdf0a.ttf',
   'fonts/good/81cee6e061d37a83f12c007c89b89e4b81951eb5.ttf',
   'fonts/good/83de2fc102dbe5e1738710655787d736e51f5b56.ttf',
   'fonts/good/84df123947f7f5f9a5456e755f91bef963b1dd7c.otf',
   'fonts/good/877ba38762b32f50468250d8bb659a2af252f44f.ttf',
+  'fonts/good/88ffc07c893a8e7d1f9622eaebd572d588fee7ea.otf',
   'fonts/good/89166e0ffdfdac0309d31012d1d5c1de8fe65a52.otf',
   'fonts/good/8df517d0db2e2e3b65fe3f8e93cf5c0cffaff3d9.ttf',
   'fonts/good/9227eefacd215fee911b7c4f935e0bad9bde5772.ttf',
   'fonts/good/923963eece37a2b494c7f2b75db4ac24635784bf.ttf',
   'fonts/good/942fab6918c0dc9bf59f62ab15e3fd38736bbe8d.ttf',
   'fonts/good/94eec826e16eb8d695b13690bb1e704948b98bf9.ttf',
+  'fonts/good/960799635ff99168566f5475bb9d37facf8629fd.ttf',
   'fonts/good/965fe4ee4b2f4d090ea4cb90507c3eddcf597e1c.ttf',
+  'fonts/good/983fcc3c7f3bc7bf2063104d72d1b5d7589378d2.otf',
   'fonts/good/9a614250473dd0f051d808ff05e5bcb5988d44f4.ttf',
   'fonts/good/9dc7e9523203d97914edf64aff494a1a18762782.ttf',
+  'fonts/good/9ed41be8b32ab179d63c91df0585e8cc070e21ec.ttf',
   'fonts/good/a29b6af1965f9cac3b4ada03258bcce6a155b168.ttf',
   'fonts/good/a64a622a50d6400592a9590c003afb02e9e4436d.otf',
   'fonts/good/a69c0298f6d3e29903a492ce1f175932dabf800e.otf',
   'fonts/good/ad455c8c531334cf470a98901cbe86a378895c14.ttf',
   'fonts/good/b258998a804fe4780216ebd43248436e2d015f03.ttf',
+  'fonts/good/b2fc7c776ddbc942ae72bf4060a8c1412b715cf3.otf',
   'fonts/good/b3590210e2baa7fb6c58af1ce98d383d8bf47683.ttf',
   'fonts/good/b4a99e4fdd041256e354d4ada89bb2900908e78b.ttf',
   'fonts/good/b8a18a5eec94d4ab749fbd825e6fa198607704a2.ttf',
   'fonts/good/b98ec6ce1630f86eb34d18666002676498618717.ttf',
   'fonts/good/baaef388d8b2a70bec6024534974f417119304be.ttf',
+  'fonts/good/bb4d6e4c25c01847c88db33066bf85e97ea27cd0.otf',
   'fonts/good/bd4c6cd00c8b7de49831f2153414c49902da973c.ttf',
   'fonts/good/bdc581002a733b039b57b0c56d187ad228bf4a1f.ttf',
   'fonts/good/bf5c8e9f890bfbf757589943b18534e6097eeaad.ttf',
   'fonts/good/c026cbcefd9e0c9995208ef613c27b48b548ba6f.ttf',
   'fonts/good/c1fd802800359304594785d0ea5fb1eadb14666c.ttf',
   'fonts/good/c3886b3124a97b9b9212c426c50366773e9ef10c.otf',
   'fonts/good/c39e763ce6fb900b07f219ca252524ea37e6d1ad.ttf',
+  'fonts/good/c58d4e63655652bc74153333cd91f190a6e6671e.ttf',
   'fonts/good/c7999e53cde30047922a2f6adb5eb64f4aac2d54.ttf',
+  'fonts/good/c7c0abafe42cda85913730dd6813223cbb5d57ae.otf',
   'fonts/good/c7d76de613012ce941785c387eb6570d905bc6a7.ttf',
   'fonts/good/c8af7209f1c5c9a2e541214c9bc31bb2bb676c0e.otf',
+  'fonts/good/ce6ada335d2950f6893926d3fbec2b648a4014cb.ttf',
   'fonts/good/d0ff0af970457d3a599c5f82f375ceb1faaade3c.ttf',
   'fonts/good/d391cf982a114ea43871890da047df4a7b5a087b.ttf',
   'fonts/good/d3ae20d9f21e321f0813094dd6970468f187b669.ttf',
   'fonts/good/d427ef152e9e6a8b1865ae00c22b9a282d008073.ttf',
   'fonts/good/d8ab8092b46ae0e06c310bdd063b9fd65d04fe93.ttf',
   'fonts/good/da1c5e82a0257f9998ff45185ffc153fde98fb12.ttf',
   'fonts/good/db4b768546934de921667761967706f4f527a75a.ttf',
   'fonts/good/dc884ba7e1d0f85620c586423782e8e65a16be44.ttf',
   'fonts/good/e1d157dc9799a686992e5f6c150949fcf3d20ce0.otf',
+  'fonts/good/e502b70bfa49d3f497b2a15093a3765e29ccfdcc.ttf',
   'fonts/good/e6e8ab2987f8c1f9bf6a8a3f9e58dbd62195c4e6.ttf',
+  'fonts/good/e9b02051de5a2b3a3ae1e044e2c459421511a77f.otf',
   'fonts/good/e9e065f23e8c5c1559cdb76a7a350b857ce2713e.ttf',
   'fonts/good/ec0f5f1cccb6c5675b4f396b462eedf1acce7d95.ttf',
   'fonts/good/ef7da53aaff13acd3e6dedda380a2ac0ef746cab.ttf',
   'fonts/good/f172aa07083478097b7ba62e485c9ffefcd0d623.ttf',
   'fonts/good/f60191da5f12f78d23ec32c6fdf51314ce3bb8c0.ttf',
+  'fonts/good/f681955b5a5f59517c3b66a9efa202ced7f99ae1.otf',
   'fonts/good/fc6af2540969ab193e421276a18ad3cca6c68501.ttf',
   'fonts/good/fd2f7ce86f14f554ebd65bd9ba04f2d8f13943ec.ttf',
   'fonts/good/fd62f786684b29020b46c40ae4cacfbd044fc7ab.ttf',
-  'fonts/good/068aaf44acba22aa769fc7023b9b575fdf72c530.otf',
-  'fonts/good/14b84df95987d7ba699d058686e9163eb4ca5e75.ttf',
-  'fonts/good/1554deaab977f26747d651fa983988429bc0ebc5.ttf',
-  'fonts/good/27312d3d8d62bf7f3d2dec4afd90ac5549c05958.otf',
-  'fonts/good/39b02c925a67188e7dd1fb9e78e7799976d8b6f6.otf',
-  'fonts/good/4e5ac04a7e4638302443a8d9e3258772ccb60744.ttf',
-  'fonts/good/4e7747c985aa4f1b89f5f6c09f4ec4094bf1b20b.otf',
-  'fonts/good/54819458b3920c39db79d6e4cc8594e47654ca5f.otf',
-  'fonts/good/5b376d5ec538bc3c86749e13a815661c7f5d9528.ttf',
-  'fonts/good/611dc1a20537abb29791dfdbf12ecb48afd94f53.otf',
-  'fonts/good/6d7ceee66a8d288d96ea235b1d642b75d96cafd5.otf',
-  'fonts/good/7ef289b55de3392d9fca03735ea0a1c8498fdf0a.ttf',
-  'fonts/good/88ffc07c893a8e7d1f9622eaebd572d588fee7ea.otf',
-  'fonts/good/960799635ff99168566f5475bb9d37facf8629fd.ttf',
-  'fonts/good/983fcc3c7f3bc7bf2063104d72d1b5d7589378d2.otf',
-  'fonts/good/9ed41be8b32ab179d63c91df0585e8cc070e21ec.ttf',
-  'fonts/good/b2fc7c776ddbc942ae72bf4060a8c1412b715cf3.otf',
-  'fonts/good/bb4d6e4c25c01847c88db33066bf85e97ea27cd0.otf',
-  'fonts/good/c58d4e63655652bc74153333cd91f190a6e6671e.ttf',
-  'fonts/good/c7c0abafe42cda85913730dd6813223cbb5d57ae.otf',
-  'fonts/good/ce6ada335d2950f6893926d3fbec2b648a4014cb.ttf',
-  'fonts/good/e9b02051de5a2b3a3ae1e044e2c459421511a77f.otf',
-  'fonts/good/f681955b5a5f59517c3b66a9efa202ced7f99ae1.otf',
 ]
 
 bad_fonts = [
   'fonts/bad/0014256514b220c525e98840b0d6ba736a85acbd.ttf',
   'fonts/bad/003a9baf5665abc42fae0d7027718294601385b9.ttf',
   'fonts/bad/00ac7a910785ea3a30655fe386d4cb02b39719aa.otf',
   'fonts/bad/013d9956e40d1ea194c4d7817fbf220d6be9c33b.ttf',
@@ -137,14 +139,15 @@
   'fonts/bad/173c4c23291c983fead3d734afd8a4de504f508e.otf',
   'fonts/bad/17cbd36aad32fe96dfb6dc49ceaaed54553c9189.ttf',
   'fonts/bad/1ccbe1de6cfd3c183f067d4a2549f81405740a1d.ttf',
   'fonts/bad/1de19636832bb7ebb45680fb09b44227f19a96ce.ttf',
   'fonts/bad/1ef2c4e95428d382ed8653c6657bdb66eb0f415d.ttf',
   'fonts/bad/23b2a3316b3797bf9a61acdf36cf63d10ab3342e.woff',
   'fonts/bad/251a4ffb5418b336217a9e7958941192b5a20137.otf',
+  'fonts/bad/257a9ccbda162eec44796987d8e20fca32288029.otf',
   'fonts/bad/28ce9a4dc67328856213bb1da09d55e4cf561c68.ttf',
   'fonts/bad/2d0bf4e52a64aa8bda2fdd9597e1bb4fbf33eb2b.woff2',
   'fonts/bad/2d80771036e065b9cd582b769d0388a0de90f84f.ttf',
   'fonts/bad/2edb1d50d2b8f4ccf8b7d56e7f354dd86be081f9.ttf',
   'fonts/bad/2f74c3cb404c60d9a46e883c88d6c10dc3562fad.otf',
   'fonts/bad/335e7e5a354010624679dfb52609652c4a7f6fc8.ttf',
   'fonts/bad/33df9c8b531928c90a3afebf6b15828dd0cad929.otf',
@@ -216,15 +219,14 @@
   'fonts/bad/e071a5082117ad5a64dc3db1bfcd0a31d6db93ae.ttf',
   'fonts/bad/ea8c4b1d5178ae184ffd0346f12fd426850729cc.otf',
   'fonts/bad/eaeb6d903b14ee184f887aa8a0a81b917e252da9.otf',
   'fonts/bad/eb44137aa49ccb9ea7aad127a8fdc6e155f20565.ttf',
   'fonts/bad/ed550c912a8c5febfdad9ca2500b3284ecfac0d7.ttf',
   'fonts/bad/edaf09c932e0582b1473384f66d5571da752a4d2.otf',
   'fonts/bad/f1dba4340ce94f5359fa4434debc7efcfd1b521f.ttf',
-  'fonts/bad/257a9ccbda162eec44796987d8e20fca32288029.otf',
 ]
 
 fuzzing_fonts = good_fonts + bad_fonts + [
   'fonts/fuzzing/011facefb10ee4f813117eae60bb5940a280ae30.woff2',
   'fonts/fuzzing/0509e80afb379d16560e9e47bdd7d888bebdebc6.ttf',
   'fonts/fuzzing/051d92f8bc6ff724511b296c27623f824de256e9.ttf',
   'fonts/fuzzing/05a7abc8e4c954ef105d056bd6249c6fda96d4a8.otf',
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/util/ots-fuzzer.cc` & `opentype-sanitizer-9.1.0/src/c/ots/util/ots-fuzzer.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/util/ots-idempotent.cc` & `opentype-sanitizer-9.1.0/src/c/ots/util/ots-idempotent.cc`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 // Use of this source code is governed by a BSD-style license that can be
 // found in the LICENSE file.
 
 #include "config.h"
 
 #if defined(HAVE_CORETEXT)
 #include <ApplicationServices/ApplicationServices.h>
+#elif defined(HAVE_WIN32)
+#define NOMINMAX
+#include <Windows.h>
 #elif defined(HAVE_FREETYPE)
 #include <ft2build.h>
 #include FT_FREETYPE_H
 #include FT_OUTLINE_H
-#elif defined(HAVE_WIN32)
-#define NOMINMAX
-#include <Windows.h>
 #endif
 
 #include <fstream>
 #include <iostream>
 #include <vector>
 
 #include "test-context.h"
@@ -66,14 +66,26 @@
   CGFontRelease(cgFontRef);
   if (!numGlyphs) {
     return false;
   }
   return true;
 }
 
+#elif defined(HAVE_WIN32)
+// Windows
+bool VerifyTranscodedFont(uint8_t *result, const size_t len) {
+  DWORD num_fonts = 0;
+  HANDLE handle = AddFontMemResourceEx(result, len, 0, &num_fonts);
+  if (!handle) {
+    return false;
+  }
+  RemoveFontMemResourceEx(handle);
+  return true;
+}
+
 #elif defined(HAVE_FREETYPE)
 bool VerifyTranscodedFont(uint8_t *result, const size_t len) {
   FT_Library library;
   FT_Error error = ::FT_Init_FreeType(&library);
   if (error) {
     return false;
   }
@@ -83,26 +95,14 @@
     return false;
   }
   ::FT_Done_Face(dummy);
   ::FT_Done_FreeType(library);
   return true;
 }
 
-#elif defined(HAVE_WIN32)
-// Windows
-bool VerifyTranscodedFont(uint8_t *result, const size_t len) {
-  DWORD num_fonts = 0;
-  HANDLE handle = AddFontMemResourceEx(result, len, 0, &num_fonts);
-  if (!handle) {
-    return false;
-  }
-  RemoveFontMemResourceEx(handle);
-  return true;
-}
-
 #else
 bool VerifyTranscodedFont(uint8_t *result, const size_t len) {
   std::fprintf(stderr, "Can't verify the transcoded font on this platform.\n");
   return false;
 }
 
 #endif
```

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/util/ots-perf.cc` & `opentype-sanitizer-9.1.0/src/c/ots/util/ots-perf.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/util/ots-sanitize.cc` & `opentype-sanitizer-9.1.0/src/c/ots/util/ots-sanitize.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/util/ots-side-by-side.cc` & `opentype-sanitizer-9.1.0/src/c/ots/util/ots-side-by-side.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/util/ots-validator-checker.cc` & `opentype-sanitizer-9.1.0/src/c/ots/util/ots-validator-checker.cc`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/c/ots/util/test-context.h` & `opentype-sanitizer-9.1.0/src/c/ots/util/test-context.h`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/PKG-INFO` & `opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentype-sanitizer
-Version: 9.0.0
+Version: 9.1.0
 Summary: Python wrapper for the OpenType Sanitizer
 Home-page: https://github.com/googlefonts/ots-python
 Author: Cosimo Lupo
 Author-email: cosimo@anthrotype.com
 License: OpenSource, BSD-style
 Platform: posix
 Platform: nt
```

### Comparing `opentype-sanitizer-9.0.0/src/python/opentype_sanitizer.egg-info/SOURCES.txt` & `opentype-sanitizer-9.1.0/src/python/opentype_sanitizer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 cross-files/darwin/x86_64
 src/c/ots/.gitignore
 src/c/ots/LICENSE
 src/c/ots/README.md
 src/c/ots/meson.build
 src/c/ots/meson_options.txt
 src/c/ots/.github/workflows/ci.yml
+src/c/ots/.github/workflows/cifuzz.yml
 src/c/ots/docs/DesignDoc.md
 src/c/ots/docs/HowToFix.md
 src/c/ots/docs/HowToTest.md
 src/c/ots/docs/ots-idempotent.1
 src/c/ots/docs/ots-perf.1
 src/c/ots/docs/ots-sanitize.1
 src/c/ots/docs/ots-side-by-side.1
@@ -130,15 +131,14 @@
 src/c/ots/subprojects/zlib.wrap
 src/c/ots/subprojects/packagefiles/brotli/LICENSE.build
 src/c/ots/subprojects/packagefiles/brotli/meson.build
 src/c/ots/subprojects/packagefiles/woff2/LICENSE.build
 src/c/ots/subprojects/packagefiles/woff2/meson.build
 src/c/ots/subprojects/packagefiles/woff2/meson_options.txt
 src/c/ots/tests/cff_charstring_test.cc
-src/c/ots/tests/layout_common_table_test.cc
 src/c/ots/tests/meson.build
 src/c/ots/util/ots-fuzzer.cc
 src/c/ots/util/ots-idempotent.cc
 src/c/ots/util/ots-perf.cc
 src/c/ots/util/ots-sanitize.cc
 src/c/ots/util/ots-side-by-side.cc
 src/c/ots/util/ots-validator-checker.cc
```

### Comparing `opentype-sanitizer-9.0.0/src/python/ots/__init__.py` & `opentype-sanitizer-9.1.0/src/python/ots/__init__.py`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/tests/test_ots.py` & `opentype-sanitizer-9.1.0/tests/test_ots.py`

 * *Files identical despite different names*

### Comparing `opentype-sanitizer-9.0.0/tox.ini` & `opentype-sanitizer-9.1.0/tox.ini`

 * *Files identical despite different names*

