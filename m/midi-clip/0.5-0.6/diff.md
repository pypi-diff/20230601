# Comparing `tmp/midi-clip-0.5.tar.gz` & `tmp/midi-clip-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi-clip-0.5.tar", last modified: Thu Jun  1 11:32:49 2023, max compression
+gzip compressed data, was "midi-clip-0.6.tar", last modified: Thu Jun  1 11:37:21 2023, max compression
```

## Comparing `midi-clip-0.5.tar` & `midi-clip-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 11:32:49.778828 midi-clip-0.5/
--rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.5/LICENSE.md
--rw-r--r--   0 hyunshin   (501) staff       (20)     1836 2023-06-01 11:32:49.778468 midi-clip-0.5/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)     1575 2023-06-01 11:31:35.000000 midi-clip-0.5/README.md
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 11:32:49.775431 midi-clip-0.5/midi_clip/
--rw-r--r--   0 hyunshin   (501) staff       (20)       74 2023-06-01 09:19:37.000000 midi-clip-0.5/midi_clip/__init__.py
--rw-r--r--   0 hyunshin   (501) staff       (20)    17959 2023-06-01 10:33:40.000000 midi-clip-0.5/midi_clip/midi_clip.py
--rw-r--r--   0 hyunshin   (501) staff       (20)     2838 2023-06-01 09:19:09.000000 midi-clip-0.5/midi_clip/midi_duration.py
-drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 11:32:49.778073 midi-clip-0.5/midi_clip.egg-info/
--rw-r--r--   0 hyunshin   (501) staff       (20)     1836 2023-06-01 11:32:49.000000 midi-clip-0.5/midi_clip.egg-info/PKG-INFO
--rw-r--r--   0 hyunshin   (501) staff       (20)      265 2023-06-01 11:32:49.000000 midi-clip-0.5/midi_clip.egg-info/SOURCES.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-01 11:32:49.000000 midi-clip-0.5/midi_clip.egg-info/dependency_links.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-01 11:32:49.000000 midi-clip-0.5/midi_clip.egg-info/requires.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-01 11:32:49.000000 midi-clip-0.5/midi_clip.egg-info/top_level.txt
--rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-01 11:32:49.778945 midi-clip-0.5/setup.cfg
--rw-r--r--   0 hyunshin   (501) staff       (20)      553 2023-06-01 11:32:17.000000 midi-clip-0.5/setup.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 11:37:21.712450 midi-clip-0.6/
+-rw-r--r--   0 hyunshin   (501) staff       (20)      758 2023-06-01 05:50:44.000000 midi-clip-0.6/LICENSE.md
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2045 2023-06-01 11:37:21.712147 midi-clip-0.6/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)     1784 2023-06-01 11:37:09.000000 midi-clip-0.6/README.md
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 11:37:21.709412 midi-clip-0.6/midi_clip/
+-rw-r--r--   0 hyunshin   (501) staff       (20)       74 2023-06-01 09:19:37.000000 midi-clip-0.6/midi_clip/__init__.py
+-rw-r--r--   0 hyunshin   (501) staff       (20)    17959 2023-06-01 10:33:40.000000 midi-clip-0.6/midi_clip/midi_clip.py
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2838 2023-06-01 09:19:09.000000 midi-clip-0.6/midi_clip/midi_duration.py
+drwxr-xr-x   0 hyunshin   (501) staff       (20)        0 2023-06-01 11:37:21.711694 midi-clip-0.6/midi_clip.egg-info/
+-rw-r--r--   0 hyunshin   (501) staff       (20)     2045 2023-06-01 11:37:21.000000 midi-clip-0.6/midi_clip.egg-info/PKG-INFO
+-rw-r--r--   0 hyunshin   (501) staff       (20)      265 2023-06-01 11:37:21.000000 midi-clip-0.6/midi_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        1 2023-06-01 11:37:21.000000 midi-clip-0.6/midi_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)        5 2023-06-01 11:37:21.000000 midi-clip-0.6/midi_clip.egg-info/requires.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       10 2023-06-01 11:37:21.000000 midi-clip-0.6/midi_clip.egg-info/top_level.txt
+-rw-r--r--   0 hyunshin   (501) staff       (20)       38 2023-06-01 11:37:21.712573 midi-clip-0.6/setup.cfg
+-rw-r--r--   0 hyunshin   (501) staff       (20)      553 2023-06-01 11:36:12.000000 midi-clip-0.6/setup.py
```

### Comparing `midi-clip-0.5/LICENSE.md` & `midi-clip-0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `midi-clip-0.5/PKG-INFO` & `midi-clip-0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,13 @@
-Metadata-Version: 2.1
-Name: midi-clip
-Version: 0.5
-Summary: A python package for midi clip.
-Home-page: https://github.com/kyaryunha/midi-clip
-Author: kyaryunha
-Author-email: kyaryunha@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # midi-clip
+[![PyPI](https://img.shields.io/pypi/v/midi-clip.svg)](https://pypi.python.org/pypi/midi-clip)
+
+A python package for midi clip (and midi duration) based on mido. ([github](https://github.com/kyaryunha/midi-clip))
 
-A python package for midi clip (and midi duration) based on mido.
+Author: Hyun Shin ([kyaryunha](https://github.com/kyaryunha))
 
 ### Introduce
 
 This library considers a lot of things for detailing midi clips: followings:
 
 - Supports both multi-track MIDI
 - Supports both tempo track & non-tempo track
@@ -60,8 +53,8 @@
 <td>./example/ocean_5_15.wav</td>
 </tr>
 </table>
 
 ** Used GarageBand to obtain piano roll images and Cubase to obtain audio.
 GarageBand fills in the measure regardless of the actual end of track time in the MIDI, resulting in slightly longer audio. MIDI file's time clip is precisely.
 
-** Data used for result was allowed by an anonymous artist.
+** Data used for result was allowed by an anonymous artist.
```

#### html2text {}

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1 Name: midi-clip Version: 0.5 Summary: A python package
-for midi clip. Home-page: https://github.com/kyaryunha/midi-clip Author:
-kyaryunha Author-email: kyaryunha@gmail.com Description-Content-Type: text/
-markdown License-File: LICENSE.md # midi-clip A python package for midi clip
-(and midi duration) based on mido. ### Introduce This library considers a lot
-of things for detailing midi clips: followings: - Supports both multi-track
-MIDI - Supports both tempo track & non-tempo track - Consider controllers that
-appear before start time or note_on that were not closed - Consider empty space
-before the midi - All note_on and note_off pairs are validate. (Number of
-note_on and note_off is the same, and all note_on are closed by note_off) ###
-Usage ```python import mido import midi_clip # load midi use mido mid =
-mido.MidiFile('resources/hosu.mid') # clip midi output_mid =
-midi_clip.midi_clip(mid, 5., 15.) # you can get total duration(second) of midi
-duration = midi_clip.midi_duration(output_mid) # if you see by print print
+# midi-clip [![PyPI](https://img.shields.io/pypi/v/midi-clip.svg)](https://
+pypi.python.org/pypi/midi-clip) A python package for midi clip (and midi
+duration) based on mido. ([github](https://github.com/kyaryunha/midi-clip))
+Author: Hyun Shin ([kyaryunha](https://github.com/kyaryunha)) ### Introduce
+This library considers a lot of things for detailing midi clips: followings: -
+Supports both multi-track MIDI - Supports both tempo track & non-tempo track -
+Consider controllers that appear before start time or note_on that were not
+closed - Consider empty space before the midi - All note_on and note_off pairs
+are validate. (Number of note_on and note_off is the same, and all note_on are
+closed by note_off) ### Usage ```python import mido import midi_clip # load
+midi use mido mid = mido.MidiFile('resources/hosu.mid') # clip midi output_mid
+= midi_clip.midi_clip(mid, 5., 15.) # you can get total duration(second) of
+midi duration = midi_clip.midi_duration(output_mid) # if you see by print print
 (output_mid, duration) # if you save midi clip output_mid.save('output.mid')
 ``` ### Result Result of clip "A Town With An Ocean View" MIDI from 0 to 30
 seconds and from 5 to 15 seconds.
        Piano Roll                 Audio
 0s-30s [./example/ocean_0_30.png] ./example/ocean_0_30.wav
 5s-15s [./example/ocean_5_15.png] ./example/ocean_5_15.wav
 ** Used GarageBand to obtain piano roll images and Cubase to obtain audio.
```

### Comparing `midi-clip-0.5/midi_clip/midi_clip.py` & `midi-clip-0.6/midi_clip/midi_clip.py`

 * *Files identical despite different names*

### Comparing `midi-clip-0.5/midi_clip/midi_duration.py` & `midi-clip-0.6/midi_clip/midi_duration.py`

 * *Files identical despite different names*

### Comparing `midi-clip-0.5/midi_clip.egg-info/PKG-INFO` & `midi-clip-0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: midi-clip
-Version: 0.5
+Version: 0.6
 Summary: A python package for midi clip.
 Home-page: https://github.com/kyaryunha/midi-clip
 Author: kyaryunha
 Author-email: kyaryunha@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # midi-clip
+[![PyPI](https://img.shields.io/pypi/v/midi-clip.svg)](https://pypi.python.org/pypi/midi-clip)
 
-A python package for midi clip (and midi duration) based on mido.
+A python package for midi clip (and midi duration) based on mido. ([github](https://github.com/kyaryunha/midi-clip))
+
+Author: Hyun Shin ([kyaryunha](https://github.com/kyaryunha))
 
 ### Introduce
 
 This library considers a lot of things for detailing midi clips: followings:
 
 - Supports both multi-track MIDI
 - Supports both tempo track & non-tempo track
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: midi-clip Version: 0.5 Summary: A python package
+Metadata-Version: 2.1 Name: midi-clip Version: 0.6 Summary: A python package
 for midi clip. Home-page: https://github.com/kyaryunha/midi-clip Author:
 kyaryunha Author-email: kyaryunha@gmail.com Description-Content-Type: text/
-markdown License-File: LICENSE.md # midi-clip A python package for midi clip
-(and midi duration) based on mido. ### Introduce This library considers a lot
-of things for detailing midi clips: followings: - Supports both multi-track
-MIDI - Supports both tempo track & non-tempo track - Consider controllers that
-appear before start time or note_on that were not closed - Consider empty space
-before the midi - All note_on and note_off pairs are validate. (Number of
-note_on and note_off is the same, and all note_on are closed by note_off) ###
-Usage ```python import mido import midi_clip # load midi use mido mid =
-mido.MidiFile('resources/hosu.mid') # clip midi output_mid =
-midi_clip.midi_clip(mid, 5., 15.) # you can get total duration(second) of midi
-duration = midi_clip.midi_duration(output_mid) # if you see by print print
-(output_mid, duration) # if you save midi clip output_mid.save('output.mid')
-``` ### Result Result of clip "A Town With An Ocean View" MIDI from 0 to 30
-seconds and from 5 to 15 seconds.
+markdown License-File: LICENSE.md # midi-clip [![PyPI](https://img.shields.io/
+pypi/v/midi-clip.svg)](https://pypi.python.org/pypi/midi-clip) A python package
+for midi clip (and midi duration) based on mido. ([github](https://github.com/
+kyaryunha/midi-clip)) Author: Hyun Shin ([kyaryunha](https://github.com/
+kyaryunha)) ### Introduce This library considers a lot of things for detailing
+midi clips: followings: - Supports both multi-track MIDI - Supports both tempo
+track & non-tempo track - Consider controllers that appear before start time or
+note_on that were not closed - Consider empty space before the midi - All
+note_on and note_off pairs are validate. (Number of note_on and note_off is the
+same, and all note_on are closed by note_off) ### Usage ```python import mido
+import midi_clip # load midi use mido mid = mido.MidiFile('resources/hosu.mid')
+# clip midi output_mid = midi_clip.midi_clip(mid, 5., 15.) # you can get total
+duration(second) of midi duration = midi_clip.midi_duration(output_mid) # if
+you see by print print(output_mid, duration) # if you save midi clip
+output_mid.save('output.mid') ``` ### Result Result of clip "A Town With An
+Ocean View" MIDI from 0 to 30 seconds and from 5 to 15 seconds.
        Piano Roll                 Audio
 0s-30s [./example/ocean_0_30.png] ./example/ocean_0_30.wav
 5s-15s [./example/ocean_5_15.png] ./example/ocean_5_15.wav
 ** Used GarageBand to obtain piano roll images and Cubase to obtain audio.
 GarageBand fills in the measure regardless of the actual end of track time in
 the MIDI, resulting in slightly longer audio. MIDI file's time clip is
 precisely. ** Data used for result was allowed by an anonymous artist.
```

### Comparing `midi-clip-0.5/setup.py` & `midi-clip-0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="midi-clip",
-    version="0.5",
+    version="0.6",
     packages=find_packages(),
     description="A python package for midi clip.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="kyaryunha",
     author_email="kyaryunha@gmail.com",
     url="https://github.com/kyaryunha/midi-clip",
```

