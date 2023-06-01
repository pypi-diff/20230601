# Comparing `tmp/midi-clip-0.1.tar.gz` & `tmp/midi-clip-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi-clip-0.1.tar", last modified: Thu Jun  1 06:00:08 2023, max compression
+gzip compressed data, was "midi-clip-0.2.tar", last modified: Thu Jun  1 06:05:54 2023, max compression
```

## Comparing `midi-clip-0.1.tar` & `midi-clip-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:00:08.652259 midi-clip-0.1/
--rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.1/LICENSE.md
--rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 06:00:08.651901 midi-clip-0.1/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)       46 2023-06-01 05:50:17.000000 midi-clip-0.1/README.md
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:00:08.649240 midi-clip-0.1/midi_clip/
--rw-r--r--   0 hyunshin   (501) staff       (20)        0 2023-06-01 05:56:56.000000 midi-clip-0.1/midi_clip/__init__.py
--rw-r--r--   0 hyunshin   (501) staff       (20)    17649 2023-06-01 05:58:06.000000 midi-clip-0.1/midi_clip/midi_clip.py
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:00:08.651464 midi-clip-0.1/midi_clip.egg-info/
--rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 06:00:08.000000 midi-clip-0.1/midi_clip.egg-info/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)      238 2023-06-01 06:00:08.000000 midi-clip-0.1/midi_clip.egg-info/SOURCES.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-01 06:00:08.000000 midi-clip-0.1/midi_clip.egg-info/dependency_links.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-01 06:00:08.000000 midi-clip-0.1/midi_clip.egg-info/requires.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-01 06:00:08.000000 midi-clip-0.1/midi_clip.egg-info/top_level.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-01 06:00:08.652386 midi-clip-0.1/setup.cfg
--rw-r--r--   0 hyunshin   (501) staff       (20)      336 2023-06-01 05:58:16.000000 midi-clip-0.1/setup.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:05:54.094304 midi-clip-0.2/
+-rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.2/LICENSE.md
+-rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 06:05:54.093885 midi-clip-0.2/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)       46 2023-06-01 05:50:17.000000 midi-clip-0.2/README.md
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:05:54.091126 midi-clip-0.2/midi_clip/
+-rw-r--r--   0 hyunshin   (501) staff       (20)       32 2023-06-01 06:02:48.000000 midi-clip-0.2/midi_clip/__init__.py
+-rw-r--r--   0 hyunshin   (501) staff       (20)    17649 2023-06-01 05:58:06.000000 midi-clip-0.2/midi_clip/midi_clip.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:05:54.093438 midi-clip-0.2/midi_clip.egg-info/
+-rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 06:05:53.000000 midi-clip-0.2/midi_clip.egg-info/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)      238 2023-06-01 06:05:54.000000 midi-clip-0.2/midi_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-01 06:05:53.000000 midi-clip-0.2/midi_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-01 06:05:53.000000 midi-clip-0.2/midi_clip.egg-info/requires.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-01 06:05:53.000000 midi-clip-0.2/midi_clip.egg-info/top_level.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-01 06:05:54.094471 midi-clip-0.2/setup.cfg
+-rw-r--r--   0 hyunshin   (501) staff       (20)      336 2023-06-01 06:03:32.000000 midi-clip-0.2/setup.py
```

### Comparing `midi-clip-0.1/LICENSE.md` & `midi-clip-0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `midi-clip-0.1/midi_clip/midi_clip.py` & `midi-clip-0.2/midi_clip/midi_clip.py`

 * *Files identical despite different names*

