# Comparing `tmp/pycmx-1.2.0.tar.gz` & `tmp/pycmx-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmx-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pycmx-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pycmx-1.2.0.tar` & `pycmx-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2803 2023-05-18 00:06:45.586033 pycmx-1.2.0/README.md
--rw-r--r--   0        0        0      444 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/__init__.py
--rw-r--r--   0        0        0     3116 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/channel_map.py
--rw-r--r--   0        0        0     3624 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/edit.py
--rw-r--r--   0        0        0     2993 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/edit_list.py
--rw-r--r--   0        0        0     3156 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/event.py
--rw-r--r--   0        0        0      463 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/parse_cmx_events.py
--rw-r--r--   0        0        0     6668 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/parse_cmx_statements.py
--rw-r--r--   0        0        0     2258 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/transition.py
--rw-r--r--   0        0        0      801 2023-05-18 00:06:45.586033 pycmx-1.2.0/pycmx/util.py
--rw-r--r--   0        0        0     1465 2023-05-18 00:06:45.586033 pycmx-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 pycmx-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2803 2023-06-01 02:00:40.751563 pycmx-1.2.1/README.md
+-rw-r--r--   0        0        0      388 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/__init__.py
+-rw-r--r--   0        0        0     3248 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/channel_map.py
+-rw-r--r--   0        0        0     3775 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/edit.py
+-rw-r--r--   0        0        0     3172 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/edit_list.py
+-rw-r--r--   0        0        0     3781 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/event.py
+-rw-r--r--   0        0        0      472 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/parse_cmx_events.py
+-rw-r--r--   0        0        0     6755 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/parse_cmx_statements.py
+-rw-r--r--   0        0        0     2378 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/transition.py
+-rw-r--r--   0        0        0      801 2023-06-01 02:00:40.751563 pycmx-1.2.1/pycmx/util.py
+-rw-r--r--   0        0        0     1465 2023-06-01 02:00:40.751563 pycmx-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3877 1970-01-01 00:00:00.000000 pycmx-1.2.1/PKG-INFO
```

### Comparing `pycmx-1.2.0/README.md` & `pycmx-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pycmx-1.2.0/pycmx/channel_map.py` & `pycmx-1.2.1/pycmx/channel_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pycmx
 # (c) 2018 Jamie Hardt
 
 from re import (compile, match)
-from typing import Dict, Tuple
+from typing import Dict, Tuple, Generator
 
 class ChannelMap:
     """
     Represents a set of all the channels to which an event applies.
     """
 
     _chan_map : Dict[str, Tuple] = {     
@@ -20,70 +20,70 @@
         }
 
     def __init__(self, v=False, audio_channels=set()):
         self._audio_channel_set = audio_channels 
         self.v = v
 
     @property
-    def video(self):
+    def video(self) -> bool:
         'True if video is included'
         return self.v
 
     @property
-    def audio(self):
+    def audio(self) -> bool:
         'True if an audio channel is included'
         return len(self._audio_channel_set) > 0
 
     @property
-    def channels(self):
+    def channels(self) -> Generator[int, None, None]:
         'A generator for each audio channel'
         for c in self._audio_channel_set:
             yield c
 
     @property
-    def a1(self):
+    def a1(self) -> bool:
         """True if A1 is included"""
         return self.get_audio_channel(1)
 
     @a1.setter
-    def a1(self,val):
+    def a1(self, val: bool):
         self.set_audio_channel(1,val)
 
     @property
-    def a2(self):
+    def a2(self) -> bool:
         """True if A2 is included"""
         return self.get_audio_channel(2)
 
     @a2.setter
-    def a2(self,val):
+    def a2(self, val: bool):
         self.set_audio_channel(2,val)
 
     @property
-    def a3(self):
+    def a3(self) -> bool:
         """True if A3 is included"""
         return self.get_audio_channel(3)
 
     @a3.setter
-    def a3(self,val):
+    def a3(self, val: bool):
         self.set_audio_channel(3,val)
     
     @property
-    def a4(self):
+    def a4(self) -> bool:
         """True if A4 is included"""
         return self.get_audio_channel(4)
 
     @a4.setter
-    def a4(self,val):
+    def a4(self,val: bool):
         self.set_audio_channel(4,val)
 
-    def get_audio_channel(self,chan_num):
+    def get_audio_channel(self, chan_num) -> bool:
         """True if chan_num is included"""
         return (chan_num in self._audio_channel_set)
 
-    def set_audio_channel(self,chan_num,enabled):
+    def set_audio_channel(self,chan_num, enabled: bool):
         """If enabled is true, chan_num will be included"""
         if enabled:
             self._audio_channel_set.add(chan_num)
         elif self.get_audio_channel(chan_num):
             self._audio_channel_set.remove(chan_num)
     
     def _append_event(self, event_str):
```

### Comparing `pycmx-1.2.0/pycmx/edit.py` & `pycmx-1.2.1/pycmx/edit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,124 @@
 # pycmx
 # (c) 2018 Jamie Hardt
 
 from .transition import Transition
 from .channel_map import ChannelMap
-from .parse_cmx_statements import StmtEffectsName
+# from .parse_cmx_statements import StmtEffectsName
+
+from typing import Optional
 
 class Edit:
     """
     An individual source-to-record operation, with a source roll, source and 
     recorder timecode in and out, a transition and channels.
     """
     def __init__(self, edit_statement, audio_ext_statement, clip_name_statement, source_file_statement, trans_name_statement = None):
         self.edit_statement = edit_statement
         self.audio_ext = audio_ext_statement
         self.clip_name_statement = clip_name_statement
         self.source_file_statement = source_file_statement
         self.trans_name_statement = trans_name_statement 
 
     @property
-    def line_number(self):
+    def line_number(self) -> int:
         """
         Get the line number for the "standard form" statement associated with
         this edit. Line numbers a zero-indexed, such that the 
         "TITLE:" record is line zero.
         """
         return self.edit_statement.line_number
 
     @property
-    def channels(self):
+    def channels(self) -> ChannelMap:
         """
         Get the :obj:`ChannelMap` object associated with this Edit.
         """
         cm = ChannelMap()
         cm._append_event(self.edit_statement.channels)
         if self.audio_ext != None:
             cm._append_ext(self.audio_ext)
         return cm
 
     @property
-    def transition(self):
+    def transition(self) -> Transition:
         """
         Get the :obj:`Transition` object associated with this edit.
         """
         if self.trans_name_statement:
             return Transition(self.edit_statement.trans, self.edit_statement.trans_op, self.trans_name_statement.name)
         else:
             return Transition(self.edit_statement.trans, self.edit_statement.trans_op, None)
     
     @property
-    def source_in(self):
+    def source_in(self) -> str:
         """
         Get the source in timecode.
         """
         return self.edit_statement.source_in
 
     @property
-    def source_out(self):
+    def source_out(self) -> str:
         """
         Get the source out timecode.
         """
 
         return self.edit_statement.source_out
 
     @property
-    def record_in(self):
+    def record_in(self) -> str:
         """
         Get the record in timecode.
         """
 
         return self.edit_statement.record_in
 
     @property
-    def record_out(self):
+    def record_out(self) -> str:
         """
         Get the record out timecode.
         """
 
         return self.edit_statement.record_out
 
     @property
-    def source(self):
+    def source(self) -> str:
         """
         Get the source column. This is the 8, 32 or 128-character string on the
         event record line, this usually references the tape name of the source.
         """
         return self.edit_statement.source
 
     @property
-    def black(self):
+    def black(self) -> bool:
         """
         Black video or silence should be used as the source for this event.
         """
         return self.source == "BL"
 
     @property
-    def aux_source(self):
+    def aux_source(self) -> bool:
         """
         An auxiliary source is the source of this event.
         """
         return self.source == "AX"
 
     @property
-    def source_file(self):
+    def source_file(self) -> Optional[str]:
         """
         Get the source file, as attested by a "* SOURCE FILE" remark on the
         EDL. This will return None if the information is not present.
         """
         if self.source_file_statement is None:
             return None
         else:
             return self.source_file_statement.filename
 
     @property
-    def clip_name(self):
+    def clip_name(self) -> Optional[str]:
         """
         Get the clip name, as attested by a "* FROM CLIP NAME" or "* TO CLIP 
         NAME" remark on the EDL. This will return None if the information is
         not present.
         """
         if self.clip_name_statement is None:
             return None
```

### Comparing `pycmx-1.2.0/pycmx/edit_list.py` & `pycmx-1.2.1/pycmx/edit_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # pycmx
 # (c) 2018 Jamie Hardt
 
 from .parse_cmx_statements import (StmtUnrecognized, StmtFCM, StmtEvent, StmtSourceUMID)
 from .event import Event
 from .channel_map import ChannelMap
 
+from typing import Generator
+
 class EditList:
     """
-    Represents an entire edit decision list as returned by `parse_cmx3600()`.
-    
+    Represents an entire edit decision list as returned by :func:`~pycmx.parse_cmx3600()`.
     """
     def __init__(self, statements):
         self.title_statement = statements[0]
         self.event_statements = statements[1:]
 
-    
     @property
-    def format(self):
+    def format(self) -> str:
         """
-        The detected format of the EDL. Possible values are: `3600`,`File32`,
-        `File128`, and `unknown`
+        The detected format of the EDL. Possible values are: "3600", "File32",
+        "File128", and "unknown".
         """
         first_event = next( (s for s in self.event_statements if type(s) is StmtEvent), None)
 
         if first_event:
             if first_event.format == 8:
                 return '3600'
             elif first_event.format == 32:
@@ -33,47 +33,47 @@
             else:
                 return 'unknown'
         else:
             return 'unknown'
         
 
     @property
-    def channels(self):
+    def channels(self) -> ChannelMap:
         """
         Return the union of every channel channel.
         """
 
         retval = ChannelMap()
         for event in self.events:
             for edit in event.edits:
                 retval = retval | edit.channels
 
         return retval
         
 
     @property
-    def title(self):
+    def title(self) -> str:
         """
         The title of this edit list.
         """
         return self.title_statement.title
 
     
     @property
-    def unrecognized_statements(self):
+    def unrecognized_statements(self) -> Generator[StmtUnrecognized, None, None]:
         """
         A generator for all the unrecognized statements in the list.
         """
         for s in self.event_statements:
             if type(s) is StmtUnrecognized:
                 yield s
         
 
     @property
-    def events(self):
+    def events(self) -> Generator[Event, None, None]:
         'A generator for all the events in the edit list'
         is_drop = None
         current_event_num = None
         event_statements = []
         for stmt in self.event_statements:
             if type(stmt) is StmtFCM:
                 is_drop = stmt.drop
@@ -93,15 +93,15 @@
                 break
             else:
                 event_statements.append(stmt)
 
         yield Event(statements=event_statements)
 
     @property
-    def sources(self):
+    def sources(self) -> Generator[StmtSourceUMID, None, None]:
         """
         A generator for all of the sources in the list
         """
         
         for stmt in self.event_statements:
             if type(stmt) is StmtSourceUMID:
                 yield stmt
```

### Comparing `pycmx-1.2.0/pycmx/event.py` & `pycmx-1.2.1/pycmx/event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 # pycmx
-# (c) 2018 Jamie Hardt
+# (c) 2023 Jamie Hardt
 
 from .parse_cmx_statements import (StmtEvent, StmtClipName, StmtSourceFile, StmtAudioExt, StmtUnrecognized, StmtEffectsName)
-from .edit import Edit
+from .edit import Edit 
+
+from typing import List, Generator, Optional, Tuple, Any
 
 class Event:
     """
-    Represents a collection of :class:`Edit`s, all with the same event number.
+    Represents a collection of :class:`~pycmx.edit.Edit` s, all with the same event number.
     """
 
     def __init__(self, statements):
         self.statements = statements
     
     @property
-    def number(self):
+    def number(self) -> int:
         """
         Return the event number.
         """
         return int(self._edit_statements()[0].event)
 
     @property
-    def edits(self):
+    def edits(self) -> List[Edit]:
         """
         Returns the edits. Most events will have a single edit, a single event
         will have multiple edits when a dissolve, wipe or key transition needs
         to be performed.
         """
         edits_audio = list( self._statements_with_audio_ext() )
         clip_names  = self._clip_name_statements()
         source_files= self._source_file_statements()
          
-        the_zip = [edits_audio]
+        the_zip: List[List[Any]] = [edits_audio]
 
         if len(edits_audio) == 2:
-            cn = [None, None]
+            start_name: Optional[StmtClipName] = None
+            end_name: Optional[StmtClipName] = None
+
             for clip_name in clip_names:
                 if clip_name.affect == 'from':
-                    cn[0] = clip_name
+                    start_name = clip_name
                 elif clip_name.affect == 'to':
-                    cn[1] = clip_name
+                    end_name = clip_name
 
-            the_zip.append(cn)
+            the_zip.append([start_name, end_name])
         else:    
             if len(edits_audio) == len(clip_names):
                 the_zip.append(clip_names)
             else:
                 the_zip.append([None] * len(edits_audio) )
 
         if len(edits_audio) == len(source_files):
@@ -53,45 +57,48 @@
             the_zip.append( source_files * len(edits_audio) )
         else:
             the_zip.append([None] * len(edits_audio) )
         
         # attach trans name to last event
         try:
             trans_statement = self._trans_name_statements()[0]
-            trans_names = [None] * (len(edits_audio) - 1)
+            trans_names: List[Optional[Any]] = [None] * (len(edits_audio) - 1)
             trans_names.append(trans_statement)
             the_zip.append(trans_names)
         except IndexError:
             the_zip.append([None] * len(edits_audio) )
 
-
-        return [ Edit(e1[0],e1[1],n1,s1,u1) for (e1,n1,s1,u1) in zip(*the_zip) ]
+        return [ Edit(edit_statement=e1[0],
+                      audio_ext_statement=e1[1],
+                      clip_name_statement=n1,
+                      source_file_statement=s1,
+                      trans_name_statement=u1) for (e1,n1,s1,u1) in zip(*the_zip) ]
             
     @property
-    def unrecognized_statements(self):
+    def unrecognized_statements(self) -> Generator[StmtUnrecognized, None, None]:
         """
         A generator for all the unrecognized statements in the event.
         """
         for s in self.statements:
             if type(s) is StmtUnrecognized:
                 yield s
     
-    def _trans_name_statements(self):
+    def _trans_name_statements(self) -> List[StmtEffectsName]:
         return [s for s in self.statements if type(s) is StmtEffectsName]
 
-    def _edit_statements(self):
+    def _edit_statements(self) -> List[StmtEvent]:
         return [s for s in self.statements if type(s) is StmtEvent]
 
-    def _clip_name_statements(self):
+    def _clip_name_statements(self) -> List[StmtClipName]:
         return [s for s in self.statements if type(s) is StmtClipName]
     
-    def _source_file_statements(self):
+    def _source_file_statements(self) -> List[StmtSourceFile]:
         return [s for s in self.statements if type(s) is StmtSourceFile]
     
-    def _statements_with_audio_ext(self):
+    def _statements_with_audio_ext(self) -> Generator[Tuple[StmtEvent, Optional[StmtAudioExt]], None, None]:
         for (s1, s2) in zip(self.statements, self.statements[1:]):
             if type(s1) is StmtEvent and type(s2) is StmtAudioExt:
                 yield (s1,s2)
             elif type(s1) is StmtEvent:
                 yield (s1, None)
```

### Comparing `pycmx-1.2.0/pycmx/parse_cmx_statements.py` & `pycmx-1.2.1/pycmx/parse_cmx_statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # pycmx
 # (c) 2018 Jamie Hardt
 
 import re
 import sys
 from collections import namedtuple
 from itertools import count
+from typing import TextIO, List
+
 
 from .util import collimate
 
 StmtTitle =     namedtuple("Title",["title","line_number"])
 StmtFCM =       namedtuple("FCM",["drop","line_number"])
 StmtEvent =     namedtuple("Event",["event","source","channels","trans",\
         "trans_op","source_in","source_out","record_in","record_out","format","line_number"])
 StmtAudioExt =  namedtuple("AudioExt",["audio3","audio4","line_number"])
 StmtClipName =  namedtuple("ClipName",["name","affect","line_number"])
 StmtSourceFile = namedtuple("SourceFile",["filename","line_number"])
 StmtRemark =    namedtuple("Remark",["text","line_number"])
 StmtEffectsName = namedtuple("EffectsName",["name","line_number"])
 StmtSourceUMID =   namedtuple("Source",["name","umid","line_number"])
-StmtSplitEdit = namedtuple("SplitEdit",["video","magnitue", "line_number"])
+StmtSplitEdit = namedtuple("SplitEdit",["video","magnitude", "line_number"])
 StmtMotionMemory = namedtuple("MotionMemory",["source","fps"]) # FIXME needs more fields
 StmtUnrecognized = namedtuple("Unrecognized",["content","line_number"])
 
 
-def parse_cmx3600_statements(file):
+def parse_cmx3600_statements(file: TextIO) -> List[object]:
     """
     Return a list of every statement in the file argument.
     """
     lines = file.readlines()
     line_numbers = count() 
     return [_parse_cmx3600_line(line.strip(), line_number) \
             for (line, line_number) in zip(lines,line_numbers)]
@@ -105,25 +107,25 @@
     elif content == "AUD   4":
         return StmtAudioExt(audio3=False, audio4=True, line_number=line_number)
     elif content == "AUD   3     4":
         return StmtAudioExt(audio3=True, audio4=True, line_number=line_number)
     else:
         return StmtUnrecognized(content=line, line_number=line_number)
     
-def _parse_remark(line, line_number):
+def _parse_remark(line, line_number) -> object:
     if line.startswith("FROM CLIP NAME:"):
         return StmtClipName(name=line[15:].strip() , affect="from", line_number=line_number)
     elif line.startswith("TO CLIP NAME:"):
         return StmtClipName(name=line[13:].strip(), affect="to", line_number=line_number)
     elif line.startswith("SOURCE FILE:"):
         return StmtSourceFile(filename=line[12:].strip() , line_number=line_number)
     else:
         return StmtRemark(text=line, line_number=line_number)
 
-def _parse_effects_name(line, line_number):
+def _parse_effects_name(line, line_number) -> StmtEffectsName:
     name = line[16:].strip()
     return StmtEffectsName(name=name, line_number=line_number)
 
 def _parse_split(line, line_number):
     split_type = line[10:21]
     is_video = False
     if split_type.startswith("VIDEO"):
```

### Comparing `pycmx-1.2.0/pycmx/transition.py` & `pycmx-1.2.1/pycmx/transition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # pycmx
-# (c) 2018 Jamie Hardt
+# (c) 2023 Jamie Hardt
+
+from typing import Optional
 
 class Transition:
     """
     A CMX transition: a wipe, dissolve or cut.
     """
     
     Cut = "C"
@@ -15,15 +17,15 @@
 
     def __init__(self, transition, operand, name=None):
         self.transition = transition
         self.operand = operand
         self.name = name
 
     @property
-    def kind(self):
+    def kind(self) -> Optional[str]:
         """
         Return the kind of transition: Cut, Wipe, etc
         """
         if self.cut:
             return Transition.Cut
         elif self.dissolve:
             return Transition.Dissolve
@@ -33,54 +35,56 @@
             return Transition.KeyBackground
         elif self.key_foreground:
             return Transition.Key
         elif self.key_out:
             return Transition.KeyOut
 
     @property
-    def cut(self):
+    def cut(self) -> bool:
         "`True` if this transition is a cut."
         return self.transition == 'C' 
 
     @property
-    def dissolve(self):
+    def dissolve(self) -> bool:
         "`True` if this traansition is a dissolve."
         return self.transition == 'D'
 
     @property
-    def wipe(self):
+    def wipe(self) -> bool:
         "`True` if this transition is a wipe."
         return self.transition.startswith('W')
 
     @property
-    def effect_duration(self):
+    def effect_duration(self) -> int:
         """The duration of this transition, in frames of the record target.
         
         In the event of a key event, this is the duration of the fade in.
         """
         return int(self.operand)
 
     @property
-    def wipe_number(self):
+    def wipe_number(self) -> Optional[int]:
         "Wipes are identified by a particular number."
         if self.wipe:
             return int(self.transition[1:])
         else:
             return None
 
     @property
-    def key_background(self):
+    def key_background(self) -> bool:
         "`True` if this edit is a key background."
         return self.transition == Transition.KeyBackground
 
     @property
-    def key_foreground(self):
+    def key_foreground(self) -> bool:
         "`True` if this edit is a key foreground."
         return self.transition == Transition.Key
 
     @property
-    def key_out(self):
+    def key_out(self) -> bool:
         """
         `True` if this edit is a key out. This material will removed from
         the key foreground and replaced with the key background.
         """
         return self.transition == Transition.KeyOut
+
+
```

### Comparing `pycmx-1.2.0/pycmx/util.py` & `pycmx-1.2.1/pycmx/util.py`

 * *Files identical despite different names*

### Comparing `pycmx-1.2.0/pyproject.toml` & `pycmx-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycmx-1.2.0/PKG-INFO` & `pycmx-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pycmx
-Version: 1.2.0
-Summary: pycmx is a module for parsing CMX 3600-style EDLs. For more information and
+Version: 1.2.1
+Summary: pycmx is a parser for CMX 3600-style EDLs.
 Keywords: parser,film,broadcast
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia
```

