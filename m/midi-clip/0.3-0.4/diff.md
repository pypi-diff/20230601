# Comparing `tmp/midi-clip-0.3.tar.gz` & `tmp/midi-clip-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi-clip-0.3.tar", last modified: Thu Jun  1 06:09:56 2023, max compression
+gzip compressed data, was "midi-clip-0.4.tar", last modified: Thu Jun  1 10:35:01 2023, max compression
```

## Comparing `midi-clip-0.3.tar` & `midi-clip-0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:09:56.320728 midi-clip-0.3/
--rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.3/LICENSE.md
--rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 06:09:56.320470 midi-clip-0.3/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)       46 2023-06-01 05:50:17.000000 midi-clip-0.3/README.md
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:09:56.318485 midi-clip-0.3/midi_clip/
--rw-r--r--   0 hyunshin   (501) staff       (20)       33 2023-06-01 06:08:52.000000 midi-clip-0.3/midi_clip/__init__.py
--rw-r--r--   0 hyunshin   (501) staff       (20)    17649 2023-06-01 05:58:06.000000 midi-clip-0.3/midi_clip/midi_clip.py
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 06:09:56.320074 midi-clip-0.3/midi_clip.egg-info/
--rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 06:09:56.000000 midi-clip-0.3/midi_clip.egg-info/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)      238 2023-06-01 06:09:56.000000 midi-clip-0.3/midi_clip.egg-info/SOURCES.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-01 06:09:56.000000 midi-clip-0.3/midi_clip.egg-info/dependency_links.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-01 06:09:56.000000 midi-clip-0.3/midi_clip.egg-info/requires.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-01 06:09:56.000000 midi-clip-0.3/midi_clip.egg-info/top_level.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-01 06:09:56.320826 midi-clip-0.3/setup.cfg
--rw-r--r--   0 hyunshin   (501) staff       (20)      336 2023-06-01 06:09:39.000000 midi-clip-0.3/setup.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 10:35:01.192280 midi-clip-0.4/
+-rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.4/LICENSE.md
+-rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 10:35:01.191824 midi-clip-0.4/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)     1576 2023-06-01 09:33:07.000000 midi-clip-0.4/README.md
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 10:35:01.187669 midi-clip-0.4/midi_clip/
+-rw-r--r--   0 hyunshin   (501) staff       (20)       74 2023-06-01 09:19:37.000000 midi-clip-0.4/midi_clip/__init__.py
+-rw-r--r--   0 hyunshin   (501) staff       (20)    17959 2023-06-01 10:33:40.000000 midi-clip-0.4/midi_clip/midi_clip.py
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2838 2023-06-01 09:19:09.000000 midi-clip-0.4/midi_clip/midi_duration.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 10:35:01.190937 midi-clip-0.4/midi_clip.egg-info/
+-rw-r--r--   0 hyunshin   (501) staff       (20)      219 2023-06-01 10:35:00.000000 midi-clip-0.4/midi_clip.egg-info/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)      265 2023-06-01 10:35:01.000000 midi-clip-0.4/midi_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-01 10:35:00.000000 midi-clip-0.4/midi_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-01 10:35:00.000000 midi-clip-0.4/midi_clip.egg-info/requires.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-01 10:35:00.000000 midi-clip-0.4/midi_clip.egg-info/top_level.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-01 10:35:01.192447 midi-clip-0.4/setup.cfg
+-rw-r--r--   0 hyunshin   (501) staff       (20)      336 2023-06-01 10:34:24.000000 midi-clip-0.4/setup.py
```

### Comparing `midi-clip-0.3/LICENSE.md` & `midi-clip-0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `midi-clip-0.3/midi_clip/midi_clip.py` & `midi-clip-0.4/midi_clip/midi_clip.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,20 @@
                     settings['time_signature_before_start'] = msg
                 elif msg.type == 'end_of_track':
                     settings["end_of_track"] = True
                     break
                 if msg.type in ["note_on", "note_off"]:
                     settings["has_tempo_track"] = False
                     break
+                prev_elapsed_seconds = settings["elapsed_seconds"]
                 settings["elapsed_seconds"] += mido.tick2second(msg.time, mid.ticks_per_beat, settings["tempo"])
+                if settings["elapsed_seconds"] >= end:
+                    settings["last_note_time"] = int(
+                        mido.second2tick(end - prev_elapsed_seconds, mid.ticks_per_beat, settings["tempo"]))
+                    break
                 if settings["is_start"] is True:
                     if settings["tick_delay"] > 0:
                         msg.time += settings["tick_delay"]
                         settings["tick_delay"] = 0
                     new_track.append(msg)
                 elif msg.type == "track_name":
                     # 곡이 시작되지 않았을 때 나온 track_name은 시간 0으로써, "가장 먼저 추가된다"
@@ -288,8 +293,7 @@
                     new_track.append(
                         mido.Message(type="note_off", channel=channel, note=note, time=settings["last_note_time"]))
                     # 두 번째 부터는 무조건 0초
                     settings["last_note_time"] = 0
         new_track.append(mido.MetaMessage('end_of_track', time=settings["last_note_time"]))
         output_mid.tracks.append(new_track)
     return output_mid
-
```

