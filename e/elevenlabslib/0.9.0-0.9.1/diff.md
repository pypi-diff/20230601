# Comparing `tmp/elevenlabslib-0.9.0.tar.gz` & `tmp/elevenlabslib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.9.0.tar", last modified: Thu Jun  1 12:06:38 2023, max compression
+gzip compressed data, was "elevenlabslib-0.9.1.tar", last modified: Thu Jun  1 12:13:03 2023, max compression
```

## Comparing `elevenlabslib-0.9.0.tar` & `elevenlabslib-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 12:06:38.283165 elevenlabslib-0.9.0/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     3375 2023-06-01 12:06:38.282166 elevenlabslib-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2720 2023-05-31 21:41:09.000000 elevenlabslib-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 12:06:38.274166 elevenlabslib-0.9.0/elevenlabslib/
--rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.0/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.0/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.0/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    40774 2023-06-01 12:00:13.000000 elevenlabslib-0.9.0/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.0/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     8403 2023-05-31 21:35:21.000000 elevenlabslib-0.9.0/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:06:38.281166 elevenlabslib-0.9.0/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     3375 2023-06-01 12:06:38.000000 elevenlabslib-0.9.0/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-01 12:06:38.000000 elevenlabslib-0.9.0/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 12:06:38.000000 elevenlabslib-0.9.0/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-01 12:06:38.000000 elevenlabslib-0.9.0/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 12:06:38.000000 elevenlabslib-0.9.0/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-06-01 12:00:29.000000 elevenlabslib-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 12:06:38.283165 elevenlabslib-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 12:13:03.599790 elevenlabslib-0.9.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     3379 2023-06-01 12:13:03.599790 elevenlabslib-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2023-06-01 12:12:53.000000 elevenlabslib-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 12:13:03.592790 elevenlabslib-0.9.1/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    40774 2023-06-01 12:00:13.000000 elevenlabslib-0.9.1/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.1/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     8403 2023-05-31 21:35:21.000000 elevenlabslib-0.9.1/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:13:03.597790 elevenlabslib-0.9.1/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     3379 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 12:13:03.000000 elevenlabslib-0.9.1/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-06-01 12:12:34.000000 elevenlabslib-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 12:13:03.599790 elevenlabslib-0.9.1/setup.cfg
```

### Comparing `elevenlabslib-0.9.0/LICENSE` & `elevenlabslib-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.0/PKG-INFO` & `elevenlabslib-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.0
+Version: 0.9.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # elevenlabslib
-<a href='https://ko-fi.com/lugia19' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />
+<a href='https://ko-fi.com/lugia19' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)
 ![GitHub last commit](https://img.shields.io/github/last-commit/lugia19/elevenlabslib?style=for-the-badge)
 
 Python wrapper for the full elevenlabs API.
 
 ### NOTE: There's now an official wrapper, but this project will continue to be maintained.
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.0 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.1 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE # elevenlabslib [Buy_Me_a_Coffee_at_ko-fi.com]_!
-[PyPI_-_Downloads](https://img.shields.io/pypi/dm/
-elevenlabslib?color=%23009FFFFF&style=for-the-badge)_![PyPI](https://
-img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)_!
-[GitHub_last_commit](https://img.shields.io/github/last-commit/lugia19/
-elevenlabslib?style=for-the-badge)_Python_wrapper_for_the_full_elevenlabs_API.
-###_NOTE:_There's_now_an_official_wrapper,_but_this_project_will_continue_to_be
-maintained._The_main_reason_is_the_different_approach_to_playback._By_doing
-playback_purely_within_python_instead_of_piping_to_an_external_process,_there
-are_a_couple_of_important_extra_things_that_can_be_done,_such_as:_-_Playback_on
-a_specific_output_device_-_Running_functions_exactly_when_the_playback_begins
-and_ends_-_Controlling_the_playback_from_within_python_###_**Documentation_now
-available_at_https://elevenlabslib.readthedocs.io/en/latest/**_#_Installation
-Just_run_`pip_install_elevenlabslib`,_it's_on_[pypi](https://pypi.org/project/
-elevenlabslib/)._Note:_On_Linux,_you_may_need_to_install_portaudio._On_debian
-and_derivatives,_it's_`sudo_apt-get_install_libportaudio2`,_and_possibly_also
-`sudo_apt-get_install_python3-pyaudio`._**IMPORTANT**:_The_library_requires
-libsndfile_`v1.1.0`_or_newer,_as_that_is_when_mp3_support_was_introduced._This
-won't_be_an_issue_on_Windows,_but_may_be_relevant_on_other_platforms._Check_the
-[soundfile](https://github.com/bastibe/python-soundfile#installation)_repo_for
-more_information._#_Usage_For_a_far_more_comprehensive_example,_check_
+markdown License-File: LICENSE # elevenlabslib [Buy_Me_a_Coffee_at_ko-fi.com] !
+[PyPI - Downloads](https://img.shields.io/pypi/dm/
+elevenlabslib?color=%23009FFFFF&style=for-the-badge) ![PyPI](https://
+img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge) !
+[GitHub last commit](https://img.shields.io/github/last-commit/lugia19/
+elevenlabslib?style=for-the-badge) Python wrapper for the full elevenlabs API.
+### NOTE: There's now an official wrapper, but this project will continue to be
+maintained. The main reason is the different approach to playback. By doing
+playback purely within python instead of piping to an external process, there
+are a couple of important extra things that can be done, such as: - Playback on
+a specific output device - Running functions exactly when the playback begins
+and ends - Controlling the playback from within python ### **Documentation now
+available at https://elevenlabslib.readthedocs.io/en/latest/** # Installation
+Just run `pip install elevenlabslib`, it's on [pypi](https://pypi.org/project/
+elevenlabslib/). Note: On Linux, you may need to install portaudio. On debian
+and derivatives, it's `sudo apt-get install libportaudio2`, and possibly also
+`sudo apt-get install python3-pyaudio`. **IMPORTANT**: The library requires
+libsndfile `v1.1.0` or newer, as that is when mp3 support was introduced. This
+won't be an issue on Windows, but may be relevant on other platforms. Check the
+[soundfile](https://github.com/bastibe/python-soundfile#installation) repo for
+more information. # Usage For a far more comprehensive example, check
 [example.py](https://github.com/lugia19/elevenlabslib/blob/master/example.py)
-or_[the_docs](https://elevenlabslib.readthedocs.io/en/latest/)._Here_is_a_very
-simple_usage_sample._-_Retrieves_a_voice_based_on_the_name_-_Plays_back_(using
-the_included_playback_functions_that_use_sounddevice)_all_its_samples_(and_the
-preview)_-_Generates_and_plays_back_a_new_audio_-_Deletes_the_newly_created
-audio_from_the_user_history_```py_from_elevenlabslib_import_*_user_=
-ElevenLabsUser("API_KEY")_voice_=_user.get_voices_by_name("Rachel")[0]_#_This
-is_a_list_because_multiple_voices_can_have_the_same_name_voice.play_preview
-(playInBackground=False)_voice.generate_play_audio("Test.",
-playInBackground=False)_for_historyItem_in_user.get_history_items_paginated():
-if_historyItem.text_==_"Test.":_#_The_first_items_are_the_newest,_so_we_can
-stop_as_soon_as_we_find_one._historyItem.delete()_break_```_
+or [the docs](https://elevenlabslib.readthedocs.io/en/latest/). Here is a very
+simple usage sample. - Retrieves a voice based on the name - Plays back (using
+the included playback functions that use sounddevice) all its samples (and the
+preview) - Generates and plays back a new audio - Deletes the newly created
+audio from the user history ```py from elevenlabslib import * user =
+ElevenLabsUser("API_KEY") voice = user.get_voices_by_name("Rachel")[0] # This
+is a list because multiple voices can have the same name voice.play_preview
+(playInBackground=False) voice.generate_play_audio("Test.",
+playInBackground=False) for historyItem in user.get_history_items_paginated():
+if historyItem.text == "Test.": # The first items are the newest, so we can
+stop as soon as we find one. historyItem.delete() break ```
```

### Comparing `elevenlabslib-0.9.0/README.md` & `elevenlabslib-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # elevenlabslib
-<a href='https://ko-fi.com/lugia19' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />
+<a href='https://ko-fi.com/lugia19' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)
 ![GitHub last commit](https://img.shields.io/github/last-commit/lugia19/elevenlabslib?style=for-the-badge)
 
 Python wrapper for the full elevenlabs API.
 
 ### NOTE: There's now an official wrapper, but this project will continue to be maintained.
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-# elevenlabslib [Buy_Me_a_Coffee_at_ko-fi.com]_![PyPI_-_Downloads](https://
-img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)_!
+# elevenlabslib [Buy_Me_a_Coffee_at_ko-fi.com] ![PyPI - Downloads](https://
+img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge) !
 [PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-
-the-badge)_![GitHub_last_commit](https://img.shields.io/github/last-commit/
-lugia19/elevenlabslib?style=for-the-badge)_Python_wrapper_for_the_full
-elevenlabs_API._###_NOTE:_There's_now_an_official_wrapper,_but_this_project
-will_continue_to_be_maintained._The_main_reason_is_the_different_approach_to
-playback._By_doing_playback_purely_within_python_instead_of_piping_to_an
-external_process,_there_are_a_couple_of_important_extra_things_that_can_be
-done,_such_as:_-_Playback_on_a_specific_output_device_-_Running_functions
-exactly_when_the_playback_begins_and_ends_-_Controlling_the_playback_from
-within_python_###_**Documentation_now_available_at_https://
-elevenlabslib.readthedocs.io/en/latest/**_#_Installation_Just_run_`pip_install
-elevenlabslib`,_it's_on_[pypi](https://pypi.org/project/elevenlabslib/)._Note:
-On_Linux,_you_may_need_to_install_portaudio._On_debian_and_derivatives,_it's
-`sudo_apt-get_install_libportaudio2`,_and_possibly_also_`sudo_apt-get_install
-python3-pyaudio`._**IMPORTANT**:_The_library_requires_libsndfile_`v1.1.0`_or
-newer,_as_that_is_when_mp3_support_was_introduced._This_won't_be_an_issue_on
-Windows,_but_may_be_relevant_on_other_platforms._Check_the_[soundfile](https://
-github.com/bastibe/python-soundfile#installation)_repo_for_more_information._#
-Usage_For_a_far_more_comprehensive_example,_check_[example.py](https://
-github.com/lugia19/elevenlabslib/blob/master/example.py)_or_[the_docs](https://
-elevenlabslib.readthedocs.io/en/latest/)._Here_is_a_very_simple_usage_sample._-
-Retrieves_a_voice_based_on_the_name_-_Plays_back_(using_the_included_playback
-functions_that_use_sounddevice)_all_its_samples_(and_the_preview)_-_Generates
-and_plays_back_a_new_audio_-_Deletes_the_newly_created_audio_from_the_user
-history_```py_from_elevenlabslib_import_*_user_=_ElevenLabsUser("API_KEY")
-voice_=_user.get_voices_by_name("Rachel")[0]_#_This_is_a_list_because_multiple
-voices_can_have_the_same_name_voice.play_preview(playInBackground=False)
-voice.generate_play_audio("Test.",_playInBackground=False)_for_historyItem_in
-user.get_history_items_paginated():_if_historyItem.text_==_"Test.":_#_The_first
-items_are_the_newest,_so_we_can_stop_as_soon_as_we_find_one._historyItem.delete
-()_break_```_
+the-badge) ![GitHub last commit](https://img.shields.io/github/last-commit/
+lugia19/elevenlabslib?style=for-the-badge) Python wrapper for the full
+elevenlabs API. ### NOTE: There's now an official wrapper, but this project
+will continue to be maintained. The main reason is the different approach to
+playback. By doing playback purely within python instead of piping to an
+external process, there are a couple of important extra things that can be
+done, such as: - Playback on a specific output device - Running functions
+exactly when the playback begins and ends - Controlling the playback from
+within python ### **Documentation now available at https://
+elevenlabslib.readthedocs.io/en/latest/** # Installation Just run `pip install
+elevenlabslib`, it's on [pypi](https://pypi.org/project/elevenlabslib/). Note:
+On Linux, you may need to install portaudio. On debian and derivatives, it's
+`sudo apt-get install libportaudio2`, and possibly also `sudo apt-get install
+python3-pyaudio`. **IMPORTANT**: The library requires libsndfile `v1.1.0` or
+newer, as that is when mp3 support was introduced. This won't be an issue on
+Windows, but may be relevant on other platforms. Check the [soundfile](https://
+github.com/bastibe/python-soundfile#installation) repo for more information. #
+Usage For a far more comprehensive example, check [example.py](https://
+github.com/lugia19/elevenlabslib/blob/master/example.py) or [the docs](https://
+elevenlabslib.readthedocs.io/en/latest/). Here is a very simple usage sample. -
+Retrieves a voice based on the name - Plays back (using the included playback
+functions that use sounddevice) all its samples (and the preview) - Generates
+and plays back a new audio - Deletes the newly created audio from the user
+history ```py from elevenlabslib import * user = ElevenLabsUser("API_KEY")
+voice = user.get_voices_by_name("Rachel")[0] # This is a list because multiple
+voices can have the same name voice.play_preview(playInBackground=False)
+voice.generate_play_audio("Test.", playInBackground=False) for historyItem in
+user.get_history_items_paginated(): if historyItem.text == "Test.": # The first
+items are the newest, so we can stop as soon as we find one. historyItem.delete
+() break ```
```

### Comparing `elevenlabslib-0.9.0/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.0/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.0/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.0/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.9.1/elevenlabslib/ElevenLabsVoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.0/elevenlabslib/__init__.py` & `elevenlabslib-0.9.1/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.0/elevenlabslib/helpers.py` & `elevenlabslib-0.9.1/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.0/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.9.1/elevenlabslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.0
+Version: 0.9.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # elevenlabslib
-<a href='https://ko-fi.com/lugia19' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' />
+<a href='https://ko-fi.com/lugia19' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/elevenlabslib?color=%23009FFFFF&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)
 ![GitHub last commit](https://img.shields.io/github/last-commit/lugia19/elevenlabslib?style=for-the-badge)
 
 Python wrapper for the full elevenlabs API.
 
 ### NOTE: There's now an official wrapper, but this project will continue to be maintained.
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.0 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.1 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE # elevenlabslib [Buy_Me_a_Coffee_at_ko-fi.com]_!
-[PyPI_-_Downloads](https://img.shields.io/pypi/dm/
-elevenlabslib?color=%23009FFFFF&style=for-the-badge)_![PyPI](https://
-img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge)_!
-[GitHub_last_commit](https://img.shields.io/github/last-commit/lugia19/
-elevenlabslib?style=for-the-badge)_Python_wrapper_for_the_full_elevenlabs_API.
-###_NOTE:_There's_now_an_official_wrapper,_but_this_project_will_continue_to_be
-maintained._The_main_reason_is_the_different_approach_to_playback._By_doing
-playback_purely_within_python_instead_of_piping_to_an_external_process,_there
-are_a_couple_of_important_extra_things_that_can_be_done,_such_as:_-_Playback_on
-a_specific_output_device_-_Running_functions_exactly_when_the_playback_begins
-and_ends_-_Controlling_the_playback_from_within_python_###_**Documentation_now
-available_at_https://elevenlabslib.readthedocs.io/en/latest/**_#_Installation
-Just_run_`pip_install_elevenlabslib`,_it's_on_[pypi](https://pypi.org/project/
-elevenlabslib/)._Note:_On_Linux,_you_may_need_to_install_portaudio._On_debian
-and_derivatives,_it's_`sudo_apt-get_install_libportaudio2`,_and_possibly_also
-`sudo_apt-get_install_python3-pyaudio`._**IMPORTANT**:_The_library_requires
-libsndfile_`v1.1.0`_or_newer,_as_that_is_when_mp3_support_was_introduced._This
-won't_be_an_issue_on_Windows,_but_may_be_relevant_on_other_platforms._Check_the
-[soundfile](https://github.com/bastibe/python-soundfile#installation)_repo_for
-more_information._#_Usage_For_a_far_more_comprehensive_example,_check_
+markdown License-File: LICENSE # elevenlabslib [Buy_Me_a_Coffee_at_ko-fi.com] !
+[PyPI - Downloads](https://img.shields.io/pypi/dm/
+elevenlabslib?color=%23009FFFFF&style=for-the-badge) ![PyPI](https://
+img.shields.io/pypi/v/elevenlabslib?color=%23FE6137&style=for-the-badge) !
+[GitHub last commit](https://img.shields.io/github/last-commit/lugia19/
+elevenlabslib?style=for-the-badge) Python wrapper for the full elevenlabs API.
+### NOTE: There's now an official wrapper, but this project will continue to be
+maintained. The main reason is the different approach to playback. By doing
+playback purely within python instead of piping to an external process, there
+are a couple of important extra things that can be done, such as: - Playback on
+a specific output device - Running functions exactly when the playback begins
+and ends - Controlling the playback from within python ### **Documentation now
+available at https://elevenlabslib.readthedocs.io/en/latest/** # Installation
+Just run `pip install elevenlabslib`, it's on [pypi](https://pypi.org/project/
+elevenlabslib/). Note: On Linux, you may need to install portaudio. On debian
+and derivatives, it's `sudo apt-get install libportaudio2`, and possibly also
+`sudo apt-get install python3-pyaudio`. **IMPORTANT**: The library requires
+libsndfile `v1.1.0` or newer, as that is when mp3 support was introduced. This
+won't be an issue on Windows, but may be relevant on other platforms. Check the
+[soundfile](https://github.com/bastibe/python-soundfile#installation) repo for
+more information. # Usage For a far more comprehensive example, check
 [example.py](https://github.com/lugia19/elevenlabslib/blob/master/example.py)
-or_[the_docs](https://elevenlabslib.readthedocs.io/en/latest/)._Here_is_a_very
-simple_usage_sample._-_Retrieves_a_voice_based_on_the_name_-_Plays_back_(using
-the_included_playback_functions_that_use_sounddevice)_all_its_samples_(and_the
-preview)_-_Generates_and_plays_back_a_new_audio_-_Deletes_the_newly_created
-audio_from_the_user_history_```py_from_elevenlabslib_import_*_user_=
-ElevenLabsUser("API_KEY")_voice_=_user.get_voices_by_name("Rachel")[0]_#_This
-is_a_list_because_multiple_voices_can_have_the_same_name_voice.play_preview
-(playInBackground=False)_voice.generate_play_audio("Test.",
-playInBackground=False)_for_historyItem_in_user.get_history_items_paginated():
-if_historyItem.text_==_"Test.":_#_The_first_items_are_the_newest,_so_we_can
-stop_as_soon_as_we_find_one._historyItem.delete()_break_```_
+or [the docs](https://elevenlabslib.readthedocs.io/en/latest/). Here is a very
+simple usage sample. - Retrieves a voice based on the name - Plays back (using
+the included playback functions that use sounddevice) all its samples (and the
+preview) - Generates and plays back a new audio - Deletes the newly created
+audio from the user history ```py from elevenlabslib import * user =
+ElevenLabsUser("API_KEY") voice = user.get_voices_by_name("Rachel")[0] # This
+is a list because multiple voices can have the same name voice.play_preview
+(playInBackground=False) voice.generate_play_audio("Test.",
+playInBackground=False) for historyItem in user.get_history_items_paginated():
+if historyItem.text == "Test.": # The first items are the newest, so we can
+stop as soon as we find one. historyItem.delete() break ```
```

### Comparing `elevenlabslib-0.9.0/pyproject.toml` & `elevenlabslib-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

