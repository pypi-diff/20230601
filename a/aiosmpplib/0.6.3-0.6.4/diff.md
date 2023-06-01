# Comparing `tmp/aiosmpplib-0.6.3.tar.gz` & `tmp/aiosmpplib-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosmpplib-0.6.3.tar", last modified: Sat Nov 26 17:19:57 2022, max compression
+gzip compressed data, was "aiosmpplib-0.6.4.tar", last modified: Thu Jun  1 11:26:28 2023, max compression
```

## Comparing `aiosmpplib-0.6.3.tar` & `aiosmpplib-0.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2022-11-26 17:19:57.689822 aiosmpplib-0.6.3/
--rw-r--r--   0 nik       (1000) nik       (1000)     1080 2022-10-22 18:21:47.000000 aiosmpplib-0.6.3/LICENSE.txt
--rw-r--r--   0 nik       (1000) nik       (1000)    11097 2022-11-26 17:19:57.689822 aiosmpplib-0.6.3/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)    10256 2022-11-26 17:04:16.000000 aiosmpplib-0.6.3/README.rst
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2022-11-26 17:19:57.686489 aiosmpplib-0.6.3/aiosmpplib/
--rw-r--r--   0 nik       (1000) nik       (1000)     1792 2022-11-13 12:09:23.000000 aiosmpplib-0.6.3/aiosmpplib/__init__.py
--rw-r--r--   0 nik       (1000) nik       (1000)      304 2022-11-26 17:04:30.000000 aiosmpplib-0.6.3/aiosmpplib/__version__.py
--rw-r--r--   0 nik       (1000) nik       (1000)     2658 2022-11-13 12:07:21.000000 aiosmpplib-0.6.3/aiosmpplib/broker.py
--rw-r--r--   0 nik       (1000) nik       (1000)    16291 2022-11-13 18:48:28.000000 aiosmpplib-0.6.3/aiosmpplib/codec.py
--rw-r--r--   0 nik       (1000) nik       (1000)     7320 2022-11-13 12:05:57.000000 aiosmpplib-0.6.3/aiosmpplib/correlator.py
--rw-r--r--   0 nik       (1000) nik       (1000)    38579 2022-11-26 17:15:58.000000 aiosmpplib-0.6.3/aiosmpplib/esme.py
--rw-r--r--   0 nik       (1000) nik       (1000)     3202 2022-11-13 12:05:02.000000 aiosmpplib-0.6.3/aiosmpplib/hook.py
--rw-r--r--   0 nik       (1000) nik       (1000)     1650 2022-11-26 11:38:03.000000 aiosmpplib-0.6.3/aiosmpplib/jsonutils.py
--rw-r--r--   0 nik       (1000) nik       (1000)    11415 2022-11-26 12:26:28.000000 aiosmpplib-0.6.3/aiosmpplib/log.py
--rw-r--r--   0 nik       (1000) nik       (1000)    38685 2022-11-26 11:39:26.000000 aiosmpplib-0.6.3/aiosmpplib/protocol.py
--rw-r--r--   0 nik       (1000) nik       (1000)     3067 2022-11-13 12:04:08.000000 aiosmpplib-0.6.3/aiosmpplib/ratelimiter.py
--rw-r--r--   0 nik       (1000) nik       (1000)     2481 2022-11-21 08:30:25.000000 aiosmpplib-0.6.3/aiosmpplib/retrytimer.py
--rw-r--r--   0 nik       (1000) nik       (1000)     1665 2022-11-13 12:03:18.000000 aiosmpplib-0.6.3/aiosmpplib/sequence.py
--rw-r--r--   0 nik       (1000) nik       (1000)    29102 2022-11-25 21:53:37.000000 aiosmpplib-0.6.3/aiosmpplib/state.py
--rw-r--r--   0 nik       (1000) nik       (1000)     6874 2022-11-13 12:02:12.000000 aiosmpplib-0.6.3/aiosmpplib/throttle.py
--rw-r--r--   0 nik       (1000) nik       (1000)     2509 2022-11-22 12:24:47.000000 aiosmpplib-0.6.3/aiosmpplib/utils.py
-drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2022-11-26 17:19:57.689822 aiosmpplib-0.6.3/aiosmpplib.egg-info/
--rw-r--r--   0 nik       (1000) nik       (1000)    11097 2022-11-26 17:19:57.000000 aiosmpplib-0.6.3/aiosmpplib.egg-info/PKG-INFO
--rw-r--r--   0 nik       (1000) nik       (1000)      555 2022-11-26 17:19:57.000000 aiosmpplib-0.6.3/aiosmpplib.egg-info/SOURCES.txt
--rw-r--r--   0 nik       (1000) nik       (1000)        1 2022-11-26 17:19:57.000000 aiosmpplib-0.6.3/aiosmpplib.egg-info/dependency_links.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       43 2022-11-26 17:19:57.000000 aiosmpplib-0.6.3/aiosmpplib.egg-info/requires.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       11 2022-11-26 17:19:57.000000 aiosmpplib-0.6.3/aiosmpplib.egg-info/top_level.txt
--rw-r--r--   0 nik       (1000) nik       (1000)       38 2022-11-26 17:19:57.689822 aiosmpplib-0.6.3/setup.cfg
--rw-r--r--   0 nik       (1000) nik       (1000)     5477 2022-11-09 19:19:56.000000 aiosmpplib-0.6.3/setup.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-01 11:26:28.565899 aiosmpplib-0.6.4/
+-rw-r--r--   0 nik       (1000) nik       (1000)     1080 2022-10-22 18:21:47.000000 aiosmpplib-0.6.4/LICENSE.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)    11097 2023-06-01 11:26:28.562566 aiosmpplib-0.6.4/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)    10256 2022-11-26 17:04:16.000000 aiosmpplib-0.6.4/README.rst
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-01 11:26:28.562566 aiosmpplib-0.6.4/aiosmpplib/
+-rw-r--r--   0 nik       (1000) nik       (1000)     1760 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/__init__.py
+-rw-r--r--   0 nik       (1000) nik       (1000)      304 2023-06-01 11:21:57.000000 aiosmpplib-0.6.4/aiosmpplib/__version__.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     2660 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/broker.py
+-rw-r--r--   0 nik       (1000) nik       (1000)    16365 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/codec.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     7331 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/correlator.py
+-rw-r--r--   0 nik       (1000) nik       (1000)    37843 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/esme.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     3156 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/hook.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     1625 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/jsonutils.py
+-rw-r--r--   0 nik       (1000) nik       (1000)    11591 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/log.py
+-rw-r--r--   0 nik       (1000) nik       (1000)    38918 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/protocol.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     3086 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/ratelimiter.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     2485 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/retrytimer.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     1665 2022-11-13 12:03:18.000000 aiosmpplib-0.6.4/aiosmpplib/sequence.py
+-rw-r--r--   0 nik       (1000) nik       (1000)    28385 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/state.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     6958 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/throttle.py
+-rw-r--r--   0 nik       (1000) nik       (1000)     2561 2023-06-01 11:19:59.000000 aiosmpplib-0.6.4/aiosmpplib/utils.py
+drwxr-xr-x   0 nik       (1000) nik       (1000)        0 2023-06-01 11:26:28.562566 aiosmpplib-0.6.4/aiosmpplib.egg-info/
+-rw-r--r--   0 nik       (1000) nik       (1000)    11097 2023-06-01 11:26:28.000000 aiosmpplib-0.6.4/aiosmpplib.egg-info/PKG-INFO
+-rw-r--r--   0 nik       (1000) nik       (1000)      555 2023-06-01 11:26:28.000000 aiosmpplib-0.6.4/aiosmpplib.egg-info/SOURCES.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)        1 2023-06-01 11:26:28.000000 aiosmpplib-0.6.4/aiosmpplib.egg-info/dependency_links.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       43 2023-06-01 11:26:28.000000 aiosmpplib-0.6.4/aiosmpplib.egg-info/requires.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       11 2023-06-01 11:26:28.000000 aiosmpplib-0.6.4/aiosmpplib.egg-info/top_level.txt
+-rw-r--r--   0 nik       (1000) nik       (1000)       38 2023-06-01 11:26:28.565899 aiosmpplib-0.6.4/setup.cfg
+-rw-r--r--   0 nik       (1000) nik       (1000)     5477 2022-11-09 19:19:56.000000 aiosmpplib-0.6.4/setup.py
```

### Comparing `aiosmpplib-0.6.3/LICENSE.txt` & `aiosmpplib-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiosmpplib-0.6.3/PKG-INFO` & `aiosmpplib-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosmpplib
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python asyncio SMPP client library.
 Home-page: https://github.com/niksabaldun/aiosmpplib
 Author: Nikša Baldun
 Author-email: niksa.baldun@gmail.com
 License: MIT
 Keywords: aiosmpplib,smpp,smpp-client,smpp-protocol,smpp-library,esme,smsc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aiosmpplib-0.6.3/README.rst` & `aiosmpplib-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `aiosmpplib-0.6.3/aiosmpplib/__init__.py` & `aiosmpplib-0.6.4/aiosmpplib/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 from .broker import AbstractBroker
 from .correlator import AbstractCorrelator
 from .hook import AbstractHook
 from .ratelimiter import AbstractRateLimiter
 from .retrytimer import AbstractRetryTimer
 from .sequence import AbstractSequenceGenerator
 from .throttle import AbstractThrottleHandler
-from .state import (OptionalTag, OptionalParam, SmppCommand, SmppCommandStatus, SmppDataCoding,
-                    SmppSessionState, BindMode, TON, NPI, PhoneNumber, SmppError)
-from .protocol import (SubmitSm, SubmitSmResp, DeliverSm, DeliverSmResp, Unbind, UnbindResp,
-                       BindTransceiver, BindTransceiverResp, BindReceiver, BindReceiverResp,
-                       BindTransmitter, BindTransmitterResp, EnquireLink, EnquireLinkResp,
-                       GenericNack, SmppMessage, Trackable, PduHeader, SMPP_VERSION_3_4)
+from .state import (OptionalTag, OptionalParam, SmppCommand, SmppCommandStatus, SmppDataCoding, SmppSessionState,
+                    BindMode, TON, NPI, PhoneNumber, SmppError)
+from .protocol import (SubmitSm, SubmitSmResp, DeliverSm, DeliverSmResp, Unbind, UnbindResp, BindTransceiver,
+                       BindTransceiverResp, BindReceiver, BindReceiverResp, BindTransmitter, BindTransmitterResp,
+                       EnquireLink, EnquireLinkResp, GenericNack, SmppMessage, Trackable, PduHeader, SMPP_VERSION_3_4)
 from .jsonutils import json_decode, json_encode
 
 __all__ = [
-    'SMPP_VERSION_3_4', 'GSM7BitCodec', 'GSM7BitPackedCodec', 'UCS2Codec', 'StructuredLogger',
-    'ESME', 'AbstractBroker', 'AbstractCorrelator', 'AbstractHook', 'AbstractRateLimiter',
-    'AbstractRetryTimer', 'AbstractSequenceGenerator', 'AbstractThrottleHandler', 'OptionalTag',
-    'OptionalParam', 'SmppCommand', 'SmppCommandStatus', 'SmppDataCoding', 'SmppSessionState',
-    'BindMode', 'TON', 'NPI', 'PhoneNumber', 'SmppError', 'SubmitSm', 'SubmitSmResp', 'DeliverSm',
-    'DeliverSmResp', 'Unbind', 'UnbindResp', 'BindTransceiver', 'BindTransceiverResp',
-    'BindReceiver', 'BindReceiverResp', 'BindTransmitter', 'BindTransmitterResp',
-    'EnquireLink', 'EnquireLinkResp' , 'GenericNack', 'SmppMessage', 'Trackable', 'PduHeader',
-    'json_decode', 'json_encode'
+    'SMPP_VERSION_3_4', 'GSM7BitCodec', 'GSM7BitPackedCodec', 'UCS2Codec', 'StructuredLogger', 'ESME',
+    'AbstractBroker', 'AbstractCorrelator', 'AbstractHook', 'AbstractRateLimiter', 'AbstractRetryTimer',
+    'AbstractSequenceGenerator', 'AbstractThrottleHandler', 'OptionalTag', 'OptionalParam', 'SmppCommand',
+    'SmppCommandStatus', 'SmppDataCoding', 'SmppSessionState', 'BindMode', 'TON', 'NPI', 'PhoneNumber', 'SmppError',
+    'SubmitSm', 'SubmitSmResp', 'DeliverSm', 'DeliverSmResp', 'Unbind', 'UnbindResp', 'BindTransceiver',
+    'BindTransceiverResp', 'BindReceiver', 'BindReceiverResp', 'BindTransmitter', 'BindTransmitterResp', 'EnquireLink',
+    'EnquireLinkResp', 'GenericNack', 'SmppMessage', 'Trackable', 'PduHeader', 'json_decode', 'json_encode'
 ]
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/broker.py` & `aiosmpplib-0.6.4/aiosmpplib/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 class SimpleBroker(AbstractBroker):
     '''
     This is an in-memory implementation of AbstractBroker.
 
     WARNING: It should only be used for tests and demo purposes.
     '''
 
-    def __init__(self, maxsize: int=2500) -> None:
+    def __init__(self, maxsize: int = 2500) -> None:
         '''
         Parameters:
             maxsize: the maximum number of items that can be put in the queue.
         '''
         check_param(maxsize, 'maxsize', int)
         self.queue: asyncio.Queue = asyncio.Queue(maxsize=maxsize)
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/codec.py` & `aiosmpplib-0.6.4/aiosmpplib/codec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,189 +1,189 @@
 from codecs import (Codec, CodecInfo, lookup, utf_16_be_decode, utf_16_be_encode)
 from abc import abstractmethod
 from struct import pack
 from typing import Dict, List, Optional, Tuple
 
 # GSM 03.38 -> unicode
 GSM_BASIC_DECODE_MAP: Dict[int, str] = {
-    0x00: '\u0040', # COMMERCIAL AT
-    0x01: '\u00A3', # POUND SIGN
-    0x02: '\u0024', # DOLLAR SIGN
-    0x03: '\u00A5', # YEN SIGN
-    0x04: '\u00E8', # LATIN SMALL LETTER E WITH GRAVE
-    0x05: '\u00E9', # LATIN SMALL LETTER E WITH ACUTE
-    0x06: '\u00F9', # LATIN SMALL LETTER U WITH GRAVE
-    0x07: '\u00EC', # LATIN SMALL LETTER I WITH GRAVE
-    0x08: '\u00F2', # LATIN SMALL LETTER O WITH GRAVE
-    0x09: '\u00C7', # LATIN CAPITAL LETTER C WITH CEDILLA
-    0x0A: '\u000A', # LINE FEED
-    0x0B: '\u00D8', # LATIN CAPITAL LETTER O WITH STROKE
-    0x0C: '\u00F8', # LATIN SMALL LETTER O WITH STROKE
-    0x0D: '\u000D', # CARRIAGE RETURN
-    0x0E: '\u00C5', # LATIN CAPITAL LETTER A WITH RING ABOVE
-    0x0F: '\u00E5', # LATIN SMALL LETTER A WITH RING ABOVE
-    0x10: '\u0394', # GREEK CAPITAL LETTER DELTA
-    0x11: '\u005F', # LOW LINE
-    0x12: '\u03A6', # GREEK CAPITAL LETTER PHI
-    0x13: '\u0393', # GREEK CAPITAL LETTER GAMMA
-    0x14: '\u039B', # GREEK CAPITAL LETTER LAMDA
-    0x15: '\u03A9', # GREEK CAPITAL LETTER OMEGA
-    0x16: '\u03A0', # GREEK CAPITAL LETTER PI
-    0x17: '\u03A8', # GREEK CAPITAL LETTER PSI
-    0x18: '\u03A3', # GREEK CAPITAL LETTER SIGMA
-    0x19: '\u0398', # GREEK CAPITAL LETTER THETA
-    0x1A: '\u039E', # GREEK CAPITAL LETTER XI
-    0x1C: '\u00C6', # LATIN CAPITAL LETTER AE
-    0x1D: '\u00E6', # LATIN SMALL LETTER AE
-    0x1E: '\u00DF', # LATIN SMALL LETTER SHARP S (German)
-    0x1F: '\u00C9', # LATIN CAPITAL LETTER E WITH ACUTE
-    0x20: '\u0020', # SPACE
-    0x21: '\u0021', # EXCLAMATION MARK
-    0x22: '\u0022', # QUOTATION MARK
-    0x23: '\u0023', # NUMBER SIGN
-    0x24: '\u00A4', # CURRENCY SIGN
-    0x25: '\u0025', # PERCENT SIGN
-    0x26: '\u0026', # AMPERSAND
-    0x27: '\u0027', # APOSTROPHE
-    0x28: '\u0028', # LEFT PARENTHESIS
-    0x29: '\u0029', # RIGHT PARENTHESIS
-    0x2A: '\u002A', # ASTERISK
-    0x2B: '\u002B', # PLUS SIGN
-    0x2C: '\u002C', # COMMA
-    0x2D: '\u002D', # HYPHEN-MINUS
-    0x2E: '\u002E', # FULL STOP
-    0x2F: '\u002F', # SOLIDUS
-    0x30: '\u0030', # DIGIT ZERO
-    0x31: '\u0031', # DIGIT ONE
-    0x32: '\u0032', # DIGIT TWO
-    0x33: '\u0033', # DIGIT THREE
-    0x34: '\u0034', # DIGIT FOUR
-    0x35: '\u0035', # DIGIT FIVE
-    0x36: '\u0036', # DIGIT SIX
-    0x37: '\u0037', # DIGIT SEVEN
-    0x38: '\u0038', # DIGIT EIGHT
-    0x39: '\u0039', # DIGIT NINE
-    0x3A: '\u003A', # COLON
-    0x3B: '\u003B', # SEMICOLON
-    0x3C: '\u003C', # LESS-THAN SIGN
-    0x3D: '\u003D', # EQUALS SIGN
-    0x3E: '\u003E', # GREATER-THAN SIGN
-    0x3F: '\u003F', # QUESTION MARK
-    0x40: '\u00A1', # INVERTED EXCLAMATION MARK
-    0x41: '\u0041', # LATIN CAPITAL LETTER A
-    0x42: '\u0042', # LATIN CAPITAL LETTER B
-    0x43: '\u0043', # LATIN CAPITAL LETTER C
-    0x44: '\u0044', # LATIN CAPITAL LETTER D
-    0x45: '\u0045', # LATIN CAPITAL LETTER E
-    0x46: '\u0046', # LATIN CAPITAL LETTER F
-    0x47: '\u0047', # LATIN CAPITAL LETTER G
-    0x48: '\u0048', # LATIN CAPITAL LETTER H
-    0x49: '\u0049', # LATIN CAPITAL LETTER I
-    0x4A: '\u004A', # LATIN CAPITAL LETTER J
-    0x4B: '\u004B', # LATIN CAPITAL LETTER K
-    0x4C: '\u004C', # LATIN CAPITAL LETTER L
-    0x4D: '\u004D', # LATIN CAPITAL LETTER M
-    0x4E: '\u004E', # LATIN CAPITAL LETTER N
-    0x4F: '\u004F', # LATIN CAPITAL LETTER O
-    0x50: '\u0050', # LATIN CAPITAL LETTER P
-    0x51: '\u0051', # LATIN CAPITAL LETTER Q
-    0x52: '\u0052', # LATIN CAPITAL LETTER R
-    0x53: '\u0053', # LATIN CAPITAL LETTER S
-    0x54: '\u0054', # LATIN CAPITAL LETTER T
-    0x55: '\u0055', # LATIN CAPITAL LETTER U
-    0x56: '\u0056', # LATIN CAPITAL LETTER V
-    0x57: '\u0057', # LATIN CAPITAL LETTER W
-    0x58: '\u0058', # LATIN CAPITAL LETTER X
-    0x59: '\u0059', # LATIN CAPITAL LETTER Y
-    0x5A: '\u005A', # LATIN CAPITAL LETTER Z
-    0x5B: '\u00C4', # LATIN CAPITAL LETTER A WITH DIAERESIS
-    0x5C: '\u00D6', # LATIN CAPITAL LETTER O WITH DIAERESIS
-    0x5D: '\u00D1', # LATIN CAPITAL LETTER N WITH TILDE
-    0x5E: '\u00DC', # LATIN CAPITAL LETTER U WITH DIAERESIS
-    0x5F: '\u00A7', # SECTION SIGN
-    0x60: '\u00BF', # INVERTED QUESTION MARK
-    0x61: '\u0061', # LATIN SMALL LETTER A
-    0x62: '\u0062', # LATIN SMALL LETTER B
-    0x63: '\u0063', # LATIN SMALL LETTER C
-    0x64: '\u0064', # LATIN SMALL LETTER D
-    0x65: '\u0065', # LATIN SMALL LETTER E
-    0x66: '\u0066', # LATIN SMALL LETTER F
-    0x67: '\u0067', # LATIN SMALL LETTER G
-    0x68: '\u0068', # LATIN SMALL LETTER H
-    0x69: '\u0069', # LATIN SMALL LETTER I
-    0x6A: '\u006A', # LATIN SMALL LETTER J
-    0x6B: '\u006B', # LATIN SMALL LETTER K
-    0x6C: '\u006C', # LATIN SMALL LETTER L
-    0x6D: '\u006D', # LATIN SMALL LETTER M
-    0x6E: '\u006E', # LATIN SMALL LETTER N
-    0x6F: '\u006F', # LATIN SMALL LETTER O
-    0x70: '\u0070', # LATIN SMALL LETTER P
-    0x71: '\u0071', # LATIN SMALL LETTER Q
-    0x72: '\u0072', # LATIN SMALL LETTER R
-    0x73: '\u0073', # LATIN SMALL LETTER S
-    0x74: '\u0074', # LATIN SMALL LETTER T
-    0x75: '\u0075', # LATIN SMALL LETTER U
-    0x76: '\u0076', # LATIN SMALL LETTER V
-    0x77: '\u0077', # LATIN SMALL LETTER W
-    0x78: '\u0078', # LATIN SMALL LETTER X
-    0x79: '\u0079', # LATIN SMALL LETTER Y
-    0x7A: '\u007A', # LATIN SMALL LETTER Z
-    0x7B: '\u00E4', # LATIN SMALL LETTER A WITH DIAERESIS
-    0x7C: '\u00F6', # LATIN SMALL LETTER O WITH DIAERESIS
-    0x7D: '\u00F1', # LATIN SMALL LETTER N WITH TILDE
-    0x7E: '\u00FC', # LATIN SMALL LETTER U WITH DIAERESIS
-    0x7F: '\u00E0', # LATIN SMALL LETTER A WITH GRAVE
+    0x00: '\u0040',  # COMMERCIAL AT
+    0x01: '\u00A3',  # POUND SIGN
+    0x02: '\u0024',  # DOLLAR SIGN
+    0x03: '\u00A5',  # YEN SIGN
+    0x04: '\u00E8',  # LATIN SMALL LETTER E WITH GRAVE
+    0x05: '\u00E9',  # LATIN SMALL LETTER E WITH ACUTE
+    0x06: '\u00F9',  # LATIN SMALL LETTER U WITH GRAVE
+    0x07: '\u00EC',  # LATIN SMALL LETTER I WITH GRAVE
+    0x08: '\u00F2',  # LATIN SMALL LETTER O WITH GRAVE
+    0x09: '\u00C7',  # LATIN CAPITAL LETTER C WITH CEDILLA
+    0x0A: '\u000A',  # LINE FEED
+    0x0B: '\u00D8',  # LATIN CAPITAL LETTER O WITH STROKE
+    0x0C: '\u00F8',  # LATIN SMALL LETTER O WITH STROKE
+    0x0D: '\u000D',  # CARRIAGE RETURN
+    0x0E: '\u00C5',  # LATIN CAPITAL LETTER A WITH RING ABOVE
+    0x0F: '\u00E5',  # LATIN SMALL LETTER A WITH RING ABOVE
+    0x10: '\u0394',  # GREEK CAPITAL LETTER DELTA
+    0x11: '\u005F',  # LOW LINE
+    0x12: '\u03A6',  # GREEK CAPITAL LETTER PHI
+    0x13: '\u0393',  # GREEK CAPITAL LETTER GAMMA
+    0x14: '\u039B',  # GREEK CAPITAL LETTER LAMDA
+    0x15: '\u03A9',  # GREEK CAPITAL LETTER OMEGA
+    0x16: '\u03A0',  # GREEK CAPITAL LETTER PI
+    0x17: '\u03A8',  # GREEK CAPITAL LETTER PSI
+    0x18: '\u03A3',  # GREEK CAPITAL LETTER SIGMA
+    0x19: '\u0398',  # GREEK CAPITAL LETTER THETA
+    0x1A: '\u039E',  # GREEK CAPITAL LETTER XI
+    0x1C: '\u00C6',  # LATIN CAPITAL LETTER AE
+    0x1D: '\u00E6',  # LATIN SMALL LETTER AE
+    0x1E: '\u00DF',  # LATIN SMALL LETTER SHARP S (German)
+    0x1F: '\u00C9',  # LATIN CAPITAL LETTER E WITH ACUTE
+    0x20: '\u0020',  # SPACE
+    0x21: '\u0021',  # EXCLAMATION MARK
+    0x22: '\u0022',  # QUOTATION MARK
+    0x23: '\u0023',  # NUMBER SIGN
+    0x24: '\u00A4',  # CURRENCY SIGN
+    0x25: '\u0025',  # PERCENT SIGN
+    0x26: '\u0026',  # AMPERSAND
+    0x27: '\u0027',  # APOSTROPHE
+    0x28: '\u0028',  # LEFT PARENTHESIS
+    0x29: '\u0029',  # RIGHT PARENTHESIS
+    0x2A: '\u002A',  # ASTERISK
+    0x2B: '\u002B',  # PLUS SIGN
+    0x2C: '\u002C',  # COMMA
+    0x2D: '\u002D',  # HYPHEN-MINUS
+    0x2E: '\u002E',  # FULL STOP
+    0x2F: '\u002F',  # SOLIDUS
+    0x30: '\u0030',  # DIGIT ZERO
+    0x31: '\u0031',  # DIGIT ONE
+    0x32: '\u0032',  # DIGIT TWO
+    0x33: '\u0033',  # DIGIT THREE
+    0x34: '\u0034',  # DIGIT FOUR
+    0x35: '\u0035',  # DIGIT FIVE
+    0x36: '\u0036',  # DIGIT SIX
+    0x37: '\u0037',  # DIGIT SEVEN
+    0x38: '\u0038',  # DIGIT EIGHT
+    0x39: '\u0039',  # DIGIT NINE
+    0x3A: '\u003A',  # COLON
+    0x3B: '\u003B',  # SEMICOLON
+    0x3C: '\u003C',  # LESS-THAN SIGN
+    0x3D: '\u003D',  # EQUALS SIGN
+    0x3E: '\u003E',  # GREATER-THAN SIGN
+    0x3F: '\u003F',  # QUESTION MARK
+    0x40: '\u00A1',  # INVERTED EXCLAMATION MARK
+    0x41: '\u0041',  # LATIN CAPITAL LETTER A
+    0x42: '\u0042',  # LATIN CAPITAL LETTER B
+    0x43: '\u0043',  # LATIN CAPITAL LETTER C
+    0x44: '\u0044',  # LATIN CAPITAL LETTER D
+    0x45: '\u0045',  # LATIN CAPITAL LETTER E
+    0x46: '\u0046',  # LATIN CAPITAL LETTER F
+    0x47: '\u0047',  # LATIN CAPITAL LETTER G
+    0x48: '\u0048',  # LATIN CAPITAL LETTER H
+    0x49: '\u0049',  # LATIN CAPITAL LETTER I
+    0x4A: '\u004A',  # LATIN CAPITAL LETTER J
+    0x4B: '\u004B',  # LATIN CAPITAL LETTER K
+    0x4C: '\u004C',  # LATIN CAPITAL LETTER L
+    0x4D: '\u004D',  # LATIN CAPITAL LETTER M
+    0x4E: '\u004E',  # LATIN CAPITAL LETTER N
+    0x4F: '\u004F',  # LATIN CAPITAL LETTER O
+    0x50: '\u0050',  # LATIN CAPITAL LETTER P
+    0x51: '\u0051',  # LATIN CAPITAL LETTER Q
+    0x52: '\u0052',  # LATIN CAPITAL LETTER R
+    0x53: '\u0053',  # LATIN CAPITAL LETTER S
+    0x54: '\u0054',  # LATIN CAPITAL LETTER T
+    0x55: '\u0055',  # LATIN CAPITAL LETTER U
+    0x56: '\u0056',  # LATIN CAPITAL LETTER V
+    0x57: '\u0057',  # LATIN CAPITAL LETTER W
+    0x58: '\u0058',  # LATIN CAPITAL LETTER X
+    0x59: '\u0059',  # LATIN CAPITAL LETTER Y
+    0x5A: '\u005A',  # LATIN CAPITAL LETTER Z
+    0x5B: '\u00C4',  # LATIN CAPITAL LETTER A WITH DIAERESIS
+    0x5C: '\u00D6',  # LATIN CAPITAL LETTER O WITH DIAERESIS
+    0x5D: '\u00D1',  # LATIN CAPITAL LETTER N WITH TILDE
+    0x5E: '\u00DC',  # LATIN CAPITAL LETTER U WITH DIAERESIS
+    0x5F: '\u00A7',  # SECTION SIGN
+    0x60: '\u00BF',  # INVERTED QUESTION MARK
+    0x61: '\u0061',  # LATIN SMALL LETTER A
+    0x62: '\u0062',  # LATIN SMALL LETTER B
+    0x63: '\u0063',  # LATIN SMALL LETTER C
+    0x64: '\u0064',  # LATIN SMALL LETTER D
+    0x65: '\u0065',  # LATIN SMALL LETTER E
+    0x66: '\u0066',  # LATIN SMALL LETTER F
+    0x67: '\u0067',  # LATIN SMALL LETTER G
+    0x68: '\u0068',  # LATIN SMALL LETTER H
+    0x69: '\u0069',  # LATIN SMALL LETTER I
+    0x6A: '\u006A',  # LATIN SMALL LETTER J
+    0x6B: '\u006B',  # LATIN SMALL LETTER K
+    0x6C: '\u006C',  # LATIN SMALL LETTER L
+    0x6D: '\u006D',  # LATIN SMALL LETTER M
+    0x6E: '\u006E',  # LATIN SMALL LETTER N
+    0x6F: '\u006F',  # LATIN SMALL LETTER O
+    0x70: '\u0070',  # LATIN SMALL LETTER P
+    0x71: '\u0071',  # LATIN SMALL LETTER Q
+    0x72: '\u0072',  # LATIN SMALL LETTER R
+    0x73: '\u0073',  # LATIN SMALL LETTER S
+    0x74: '\u0074',  # LATIN SMALL LETTER T
+    0x75: '\u0075',  # LATIN SMALL LETTER U
+    0x76: '\u0076',  # LATIN SMALL LETTER V
+    0x77: '\u0077',  # LATIN SMALL LETTER W
+    0x78: '\u0078',  # LATIN SMALL LETTER X
+    0x79: '\u0079',  # LATIN SMALL LETTER Y
+    0x7A: '\u007A',  # LATIN SMALL LETTER Z
+    0x7B: '\u00E4',  # LATIN SMALL LETTER A WITH DIAERESIS
+    0x7C: '\u00F6',  # LATIN SMALL LETTER O WITH DIAERESIS
+    0x7D: '\u00F1',  # LATIN SMALL LETTER N WITH TILDE
+    0x7E: '\u00FC',  # LATIN SMALL LETTER U WITH DIAERESIS
+    0x7F: '\u00E0',  # LATIN SMALL LETTER A WITH GRAVE
 }
 
 # GSM 03.38 escaped characters -> unicode
 GSM_EXTENDED_DECODE_MAP: Dict[int, str] = {
-    0x0A: '\u000C', # FORM FEED
-    0x14: '\u005E', # CIRCUMFLEX ACCENT
-    0x28: '\u007B', # LEFT CURLY BRACKET
-    0x29: '\u007D', # RIGHT CURLY BRACKET
-    0x2F: '\u005C', # REVERSE SOLIDUS
-    0x3C: '\u005B', # LEFT SQUARE BRACKET
-    0x3D: '\u007E', # TILDE
-    0x3E: '\u005D', # RIGHT SQUARE BRACKET
-    0x40: '\u007C', # VERTICAL LINE
-    0x65: '\u20AC', # EURO SIGN
+    0x0A: '\u000C',  # FORM FEED
+    0x14: '\u005E',  # CIRCUMFLEX ACCENT
+    0x28: '\u007B',  # LEFT CURLY BRACKET
+    0x29: '\u007D',  # RIGHT CURLY BRACKET
+    0x2F: '\u005C',  # REVERSE SOLIDUS
+    0x3C: '\u005B',  # LEFT SQUARE BRACKET
+    0x3D: '\u007E',  # TILDE
+    0x3E: '\u005D',  # RIGHT SQUARE BRACKET
+    0x40: '\u007C',  # VERTICAL LINE
+    0x65: '\u20AC',  # EURO SIGN
 }
 
 # Replacement characters, default is question mark. Used when it is not too
 # important to ensure exact UTF-8 -> GSM -> UTF-8 equivalence, such as when
 # humans read and write SMS. But for USSD and other M2M applications it's
 # important to ensure the conversion is exact.
 GSM_REPLACE_ENCODE_MAP: Dict[str, int] = {
-    '\u00E7': 0x09, # LATIN SMALL LETTER C WITH CEDILLA
-    '\u0391': 0x41, # GREEK CAPITAL LETTER ALPHA
-    '\u0392': 0x42, # GREEK CAPITAL LETTER BETA
-    '\u0395': 0x45, # GREEK CAPITAL LETTER EPSILON
-    '\u0397': 0x48, # GREEK CAPITAL LETTER ETA
-    '\u0399': 0x49, # GREEK CAPITAL LETTER IOTA
-    '\u039A': 0x4B, # GREEK CAPITAL LETTER KAPPA
-    '\u039C': 0x4D, # GREEK CAPITAL LETTER MU
-    '\u039D': 0x4E, # GREEK CAPITAL LETTER NU
-    '\u039F': 0x4F, # GREEK CAPITAL LETTER OMICRON
-    '\u03A1': 0x50, # GREEK CAPITAL LETTER RHO
-    '\u03A4': 0x54, # GREEK CAPITAL LETTER TAU
-    '\u03A7': 0x58, # GREEK CAPITAL LETTER CHI
-    '\u03A5': 0x59, # GREEK CAPITAL LETTER UPSILON
-    '\u0396': 0x5A, # GREEK CAPITAL LETTER ZETA
+    '\u00E7': 0x09,  # LATIN SMALL LETTER C WITH CEDILLA
+    '\u0391': 0x41,  # GREEK CAPITAL LETTER ALPHA
+    '\u0392': 0x42,  # GREEK CAPITAL LETTER BETA
+    '\u0395': 0x45,  # GREEK CAPITAL LETTER EPSILON
+    '\u0397': 0x48,  # GREEK CAPITAL LETTER ETA
+    '\u0399': 0x49,  # GREEK CAPITAL LETTER IOTA
+    '\u039A': 0x4B,  # GREEK CAPITAL LETTER KAPPA
+    '\u039C': 0x4D,  # GREEK CAPITAL LETTER MU
+    '\u039D': 0x4E,  # GREEK CAPITAL LETTER NU
+    '\u039F': 0x4F,  # GREEK CAPITAL LETTER OMICRON
+    '\u03A1': 0x50,  # GREEK CAPITAL LETTER RHO
+    '\u03A4': 0x54,  # GREEK CAPITAL LETTER TAU
+    '\u03A7': 0x58,  # GREEK CAPITAL LETTER CHI
+    '\u03A5': 0x59,  # GREEK CAPITAL LETTER UPSILON
+    '\u0396': 0x5A,  # GREEK CAPITAL LETTER ZETA
 }
 
 GSM_BASIC_ENCODE_MAP: Dict[str, int] = {char: code for code, char in GSM_BASIC_DECODE_MAP.items()}
-GSM_EXTENDED_ENCODE_MAP: Dict[str, int] = {char: code
-                                           for code, char in GSM_EXTENDED_DECODE_MAP.items()}
+GSM_EXTENDED_ENCODE_MAP: Dict[str, int] = {char: code for code, char in GSM_EXTENDED_DECODE_MAP.items()}
 
 ESCAPE: int = 0x1B
 QUESTION_MARK: int = 0x3F
 NO_BREAK_SPACE: int = 0xA0
 
 
 class SmsCodec(Codec):
+
     @classmethod
     @abstractmethod
     def get_name(cls) -> str:
         raise NotImplementedError()
 
     # encodings module API
     @classmethod
@@ -211,25 +211,24 @@
     '''
 
     @classmethod
     def get_name(cls) -> str:
         return 'gsm0338'
 
     # pylint: disable=redefined-builtin; wrongly named in superclass
-    def encode(self, input: str, errors: str='strict') -> Tuple[bytes, int]:
+    def encode(self, input: str, errors: str = 'strict') -> Tuple[bytes, int]:
         if not isinstance(input, str):
             raise TypeError('Expected str input')
         if errors not in ('strict', 'replace', 'ignore'):
             raise ValueError(f'Unknown error handling {errors}.')
 
         gsm_codes: List[int] = self.to_gsm_codes(input, errors)
         return pack('!' + 'B' * len(gsm_codes), *gsm_codes), len(input)
 
-
-    def decode(self, input: bytes, errors: str='strict') -> Tuple[str, int]:
+    def decode(self, input: bytes, errors: str = 'strict') -> Tuple[str, int]:
         if not isinstance(input, bytes):
             raise TypeError('Expected bytes input')
         if errors not in ('strict', 'replace', 'ignore'):
             raise ValueError(f'Unknown error handling {errors}.')
 
         result: str = ''
         escaped: bool = False
@@ -254,39 +253,36 @@
                 raise UnicodeDecodeError(self.get_name(), bytes(ESCAPE), consumed - 1, consumed,
                                          'Sequence ends with escape')
             if errors == 'replace':
                 result += chr(NO_BREAK_SPACE)
 
         return result, consumed
 
-
     def _decode_char(self, char_code: int, escaped: bool) -> Tuple[str, bool]:
         if char_code == ESCAPE:
             return '', True
         if escaped:
             return GSM_EXTENDED_DECODE_MAP.get(char_code, chr(NO_BREAK_SPACE)), False
         return GSM_BASIC_DECODE_MAP.get(char_code, ''), False
 
-
-    def to_gsm_codes(self, text: str, errors: str='strict') -> List[int]:
+    def to_gsm_codes(self, text: str, errors: str = 'strict') -> List[int]:
         gsm_codes: List[int] = []
         for pos, char in enumerate(text):
             char_code: Optional[int] = GSM_BASIC_ENCODE_MAP.get(char)
             if char_code is not None:
                 gsm_codes.append(char_code)
             else:
                 char_code = GSM_EXTENDED_ENCODE_MAP.get(char)
                 if char_code is not None:
                     # Encode it as an escaped character
                     gsm_codes.append(ESCAPE)
                     gsm_codes.append(char_code)
                 else:
                     if errors == 'strict':
-                        raise UnicodeEncodeError(self.get_name(), char, pos, pos + 1,
-                                                 'Unsupported char')
+                        raise UnicodeEncodeError(self.get_name(), char, pos, pos + 1, 'Unsupported char')
                     if errors == 'replace':
                         gsm_codes.append(GSM_REPLACE_ENCODE_MAP.get(char, QUESTION_MARK))
                     # Otherwise, ignore
         return gsm_codes
 
     @staticmethod
     def is_gsm_text(text: str) -> bool:
@@ -305,26 +301,26 @@
     '''
 
     @classmethod
     def get_name(cls) -> str:
         return 'gsm0338-packed'
 
     # pylint: disable=redefined-builtin; wrongly named in superclass
-    def encode(self, input: str, errors: str='strict') -> Tuple[bytes, int]:
+    def encode(self, input: str, errors: str = 'strict') -> Tuple[bytes, int]:
         if not isinstance(input, str):
             raise TypeError('Expected str input')
         if errors not in ('strict', 'replace', 'ignore'):
             raise ValueError(f'Unknown error handling {errors}.')
 
         gsm_codes: List[int] = self.to_gsm_codes(input, errors)
 
         # Pack septets to octets
-        msg_len: int = len(gsm_codes) * 7 # Required bits
-        msg_len = int(msg_len / 8) + int(msg_len % 8 > 0) # Required bytes
-        gsm_codes.append(0x00) # Add 0x00 char for easier loop handling
+        msg_len: int = len(gsm_codes) * 7  # Required bits
+        msg_len = int(msg_len / 8) + int(msg_len % 8 > 0)  # Required bytes
+        gsm_codes.append(0x00)  # Add 0x00 char for easier loop handling
         result: bytearray = bytearray(msg_len)
         count: int = 0
         index: int
         for index in range(msg_len):
             shift: int = index % 7
             lb: int = gsm_codes[count] >> shift
             hb: int = gsm_codes[count + 1] << (7 - shift) & 0xFF
@@ -332,16 +328,15 @@
             if shift == 6:
                 count += 2
             else:
                 count += 1
 
         return bytes(result), len(input)
 
-
-    def decode(self, input: bytes, errors: str='strict') -> Tuple[str, int]:
+    def decode(self, input: bytes, errors: str = 'strict') -> Tuple[str, int]:
         if not isinstance(input, bytes):
             raise TypeError('Expected bytes input')
         if errors not in ('strict', 'replace', 'ignore'):
             raise ValueError(f'Unknown error handling {errors}.')
 
         # Unpack septets from octets before lookup
         result: str = ''
@@ -398,19 +393,20 @@
 
 INBUILT_CODECS: Dict[str, CodecInfo] = {
     GSM7BitCodec.get_name(): GSM7BitCodec.get_codec_info(),
     GSM7BitPackedCodec.get_name(): GSM7BitPackedCodec.get_codec_info(),
     UCS2Codec.get_name(): UCS2Codec.get_codec_info(),
 }
 
+
 # We don't register codecs with Python registry to avoid conflict with other libraries
 # which may register the same codecs. Instead, we provide our own encode and decode methods.
 # We also get the ability to have per-client custom codecs.
-def find_codec_info(encoding: str, custom_codecs: Optional[Dict[str, CodecInfo]]=None) -> CodecInfo:
+def find_codec_info(encoding: str, custom_codecs: Optional[Dict[str, CodecInfo]] = None) -> CodecInfo:
     codec_info: Optional[CodecInfo] = None
     if custom_codecs:
         codec_info = custom_codecs.get(encoding)
     if not codec_info:
         codec_info = INBUILT_CODECS.get(encoding)
     if not codec_info:
-        codec_info = lookup(encoding) # Will raise LookupError if not found
+        codec_info = lookup(encoding)  # Will raise LookupError if not found
     return codec_info
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/correlator.py` & `aiosmpplib-0.6.4/aiosmpplib/correlator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Optional, Tuple
 from .hook import AbstractHook
 from .protocol import SmppMessage, SubmitSm
 from .state import SmppCommand
 from .utils import check_param
 
-
 _EXPIRED_ERROR: TimeoutError = TimeoutError('No response to command received within timeout')
 
 
 class AbstractCorrelator(ABC):
     '''
     Interface that must be implemented to satisfy aiosmpplib Correlator.
     User implementations should inherit this class and
@@ -123,15 +122,15 @@
        {
             'smsc_message_id1': (681.109023565, 'log_id1', 'hook_metadata1'),
             'smsc_message_id2': (682.109023565, 'log_id2', 'hook_metadata2'),
             ...
        }
     '''
 
-    def __init__(self, max_ttl: float=15.00) -> None:
+    def __init__(self, max_ttl: float = 15.00) -> None:
         '''
         Parameters:
             max_ttl: The time in seconds that an item is going to be stored.
                      After the expiration of max_ttl seconds, that item will be deleted.
         '''
         check_param(max_ttl, 'max_ttl', float)
         if max_ttl < 1.00:
@@ -175,9 +174,11 @@
             message: SmppMessage
             stored_at, message = self._store[sequence_num]
             if now - stored_at > self.max_ttl:
                 del self._store[sequence_num]
                 await self.expired(message)
 
         if any(now - value[0] > self.max_ttl for value in self._delivery_store.values()):
-            self._delivery_store = {key: value for key, value in self._delivery_store.items()
-                                    if now - value[0] > self.max_ttl}
+            self._delivery_store = {
+                key: value
+                for key, value in self._delivery_store.items() if now - value[0] > self.max_ttl
+            }
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/esme.py` & `aiosmpplib-0.6.4/aiosmpplib/esme.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,30 @@
 from codecs import CodecInfo
 from string import ascii_lowercase, digits
 from typing import Any, Awaitable, Callable, Dict, Optional, Set, Tuple, Type, TypeVar, Union
 from .broker import AbstractBroker, SimpleBroker
 from .correlator import AbstractCorrelator, SimpleCorrelator
 from .hook import AbstractHook, SimpleHook
 from .log import ERROR, WARNING, INFO, StructuredLogger, Handler
-from .protocol import (DEFAULT_ENCODING, MESSAGE_TYPE_MAP, PDU_HEADER_LENGTH, SMPP_VERSION_3_4,
-                       SmppMessage, GenericNack, SubmitSm, SubmitSmResp, DeliverSm,
-                       BindReceiver, BindTransmitter, BindTransceiver, EnquireLink, Unbind)
+from .protocol import (DEFAULT_ENCODING, MESSAGE_TYPE_MAP, PDU_HEADER_LENGTH, SMPP_VERSION_3_4, SmppMessage,
+                       GenericNack, SubmitSm, SubmitSmResp, DeliverSm, BindReceiver, BindTransmitter, BindTransceiver,
+                       EnquireLink, Unbind)
 from .ratelimiter import AbstractRateLimiter
 from .retrytimer import AbstractRetryTimer, SimpleExponentialBackoff
 from .sequence import AbstractSequenceGenerator, SimpleSequenceGenerator, assert_valid_sequence
 from .throttle import AbstractThrottleHandler, SimpleThrottleHandler
-from .state import (COMMAND_RESPONSE_MAP, RESPONSE_COMMAND_MAP, NPI, TON, PduHeader, BindMode,
-                    SmppCommand, SmppDataCoding, SmppError, SmppSessionState, SmppCommandStatus)
+from .state import (COMMAND_RESPONSE_MAP, RESPONSE_COMMAND_MAP, NPI, TON, PduHeader, BindMode, SmppCommand,
+                    SmppDataCoding, SmppError, SmppSessionState, SmppCommandStatus)
 from .utils import check_param
 
-
-T = TypeVar('T') # For generic type hints
+T = TypeVar('T')  # For generic type hints
 # Maximum size of inbound network buffer.
 # The message_payload parameter can hold up to 64k data, and we add a little more to that
 # to guard against an unlikely possibility of LimitOverrunError.
-_NETWORK_BUFFER_LIMIT = 2 ** 16 + 1024
+_NETWORK_BUFFER_LIMIT = 2**16 + 1024
 
 
 class ESME:
     '''
     The External Short Message Entities implementation that will interact with SMSC server.
 
     Example declaration:
@@ -45,42 +44,43 @@
             smsc_port=2775,
             system_id='esme1',
             password=os.getenv('password', 'password'),
         )
         await esme.start()
     '''
 
-    def __init__(self,
-                 smsc_host: str,
-                 smsc_port: int,
-                 system_id: str,
-                 password: str,
-                 system_type: str='',
-                 addr_ton: TON=TON.UNKNOWN,
-                 addr_npi: NPI=NPI.UNKNOWN,
-                 address_range: str='',
-                 bind_mode: BindMode=BindMode.TRANSCEIVER,
-                 ### NON-SMPP ATTRIBUTES ###
-                 client_id: Optional[str]=None,
-                 enquire_link_interval: float=55.00,
-                 log_level: Union[str, int]=INFO,
-                 log_metadata: Optional[Dict[str, Any]]=None,
-                 log_handler: Optional[Handler]=None,
-                 log_include_timestamp: bool=True,
-                 hook: Optional[AbstractHook]=None,
-                 broker: Optional[AbstractBroker]=None,
-                 rate_limiter: Optional[AbstractRateLimiter]=None,
-                 sequence_generator: Optional[AbstractSequenceGenerator]=None,
-                 throttle_handler: Optional[AbstractThrottleHandler]=None,
-                 correlator: Optional[AbstractCorrelator]=None,
-                 retry_timer: Optional[AbstractRetryTimer]=None,
-                 socket_timeout: float=30.0,
-                 custom_codecs: Optional[Dict[str, CodecInfo]]=None,
-                 default_encoding: str=DEFAULT_ENCODING,
-                 testing: bool=False) -> None:
+    def __init__(
+            self,
+            smsc_host: str,
+            smsc_port: int,
+            system_id: str,
+            password: str,
+            system_type: str = '',
+            addr_ton: TON = TON.UNKNOWN,
+            addr_npi: NPI = NPI.UNKNOWN,
+            address_range: str = '',
+            bind_mode: BindMode = BindMode.TRANSCEIVER,
+            # NON-SMPP ATTRIBUTES
+            client_id: Optional[str] = None,
+            enquire_link_interval: float = 55.00,
+            log_level: Union[str, int] = INFO,
+            log_metadata: Optional[Dict[str, Any]] = None,
+            log_handler: Optional[Handler] = None,
+            log_include_timestamp: bool = True,
+            hook: Optional[AbstractHook] = None,
+            broker: Optional[AbstractBroker] = None,
+            rate_limiter: Optional[AbstractRateLimiter] = None,
+            sequence_generator: Optional[AbstractSequenceGenerator] = None,
+            throttle_handler: Optional[AbstractThrottleHandler] = None,
+            correlator: Optional[AbstractCorrelator] = None,
+            retry_timer: Optional[AbstractRetryTimer] = None,
+            socket_timeout: float = 30.0,
+            custom_codecs: Optional[Dict[str, CodecInfo]] = None,
+            default_encoding: str = DEFAULT_ENCODING,
+            testing: bool = False) -> None:
         '''
         Parameters:
             smsc_host: The IP address(or domain name) of the SMSC gateway/server
             smsc_port: The port at which SMSC is listening on
             system_id: Identifies the ESME system requesting to bind as
                        a transceiver with the SMSC.
             password: The password to be used by the SMSC to authenticate
@@ -137,16 +137,15 @@
         check_param(log_level, 'log_level', (int, str))
         check_param(log_metadata, 'log_metadata', dict, optional=True)
         check_param(log_handler, 'log_handler', Handler, optional=True)
         check_param(log_include_timestamp, 'log_include_timestamp', bool)
         check_param(hook, 'hook', AbstractHook, optional=True)
         check_param(broker, 'broker', AbstractBroker, optional=True)
         check_param(rate_limiter, 'rate_limiter', AbstractRateLimiter, optional=True)
-        check_param(sequence_generator, 'sequence_generator', AbstractSequenceGenerator,
-                    optional=True)
+        check_param(sequence_generator, 'sequence_generator', AbstractSequenceGenerator, optional=True)
         check_param(throttle_handler, 'throttle_handler', AbstractThrottleHandler, optional=True)
         check_param(correlator, 'correlator', AbstractCorrelator, optional=True)
         check_param(retry_timer, 'retry_timer', AbstractRetryTimer, optional=True)
         check_param(socket_timeout, 'socket_timeout', float)
         check_param(custom_codecs, 'custom_codecs', dict, optional=True)
         check_param(default_encoding, 'default_encoding', str)
         check_param(testing, 'testing', bool)
@@ -180,24 +179,22 @@
         if log_metadata is None:
             log_metadata = {
                 'smsc_host': smsc_host,
                 'system_id': system_id,
                 'client_id': self.client_id,
                 'pid': os.getpid(),
             }
-        self._logger: StructuredLogger = StructuredLogger('esme' + self.client_id, log_level,
-                                                          log_metadata, log_handler,
-                                                          log_include_timestamp)
+        self._logger: StructuredLogger = StructuredLogger('esme' + self.client_id, log_level, log_metadata,
+                                                          log_handler, log_include_timestamp)
         self.hook: AbstractHook = hook or SimpleHook(logger=self._logger)
         self.broker: AbstractBroker = broker or SimpleBroker()
         self.rate_limiter: Optional[AbstractRateLimiter] = rate_limiter
-        self.sequence_generator: AbstractSequenceGenerator = (sequence_generator or
-                                                          SimpleSequenceGenerator())
-        self.throttle_handler: AbstractThrottleHandler = (throttle_handler or
-                                                      SimpleThrottleHandler(logger=self._logger))
+        self.sequence_generator: AbstractSequenceGenerator = (sequence_generator or SimpleSequenceGenerator())
+        self.throttle_handler: AbstractThrottleHandler = (throttle_handler
+                                                          or SimpleThrottleHandler(logger=self._logger))
         self.correlator: AbstractCorrelator = correlator or SimpleCorrelator()
         self.correlator.hook = self.hook
         self.correlator.client_id = self.client_id
         self.retry_timer: AbstractRetryTimer = retry_timer or SimpleExponentialBackoff()
         self.socket_timeout: float = socket_timeout
         self.interface_version: int = SMPP_VERSION_3_4
         self._session_state: SmppSessionState = SmppSessionState.CLOSED
@@ -212,15 +209,15 @@
     async def _end_task(self, task: Task) -> None:
         '''
         Ends a top-level task after error or shutdown
         '''
         task_name: str = task.get_name()
         self._logger.debug('Ending task', task=task_name)
         try:
-            await asyncio.wait_for(task, 0.5) # Give task a chance to end gracefully
+            await asyncio.wait_for(task, 0.5)  # Give task a chance to end gracefully
         except asyncio.TimeoutError:
             await self._cancel_task(task, task_name)
             return
         except (ConnectionError, TimeoutError, IncompleteReadError, OSError, ValueError):
             # We are ending a task so we don't care about errors
             pass
         self._logger.debug('Ended task', task=task_name)
@@ -232,36 +229,36 @@
         if not task:
             task = next((t for t in asyncio.all_tasks() if t.get_name() == task_name), None)
         if not task or task.done():
             return False
 
         task.cancel()
         try:
-            await task # Will raise CancelledError
+            await task  # Will raise CancelledError
         except CancelledError:
             pass
         except RuntimeError:
             # If the coroutine sleeps, Runtime error "await wasn't used with future" will be raised
             pass
-        except Exception: # pylint: disable=broad-except
+        except Exception:  # pylint: disable=broad-except
             self._logger.exception('Error while cancelling task.', task=task_name)
 
         return True
 
     async def _socket_operation(self, coro: Awaitable[T]) -> T:
         '''
         Performs network socket operation with timeout
         '''
         return await asyncio.wait_for(coro, self.socket_timeout)
 
     async def _get_pdu(self) -> Tuple[bytes, PduHeader]:
         '''
         Retrieves next PDU from SMSC
         '''
-        assert isinstance(self._reader, StreamReader) # For type checkers
+        assert isinstance(self._reader, StreamReader)  # For type checkers
         header_data: bytes = await self._reader.readexactly(PDU_HEADER_LENGTH)
         try:
             header: PduHeader = SmppMessage.parse_header(header_data)
         except ValueError:
             self._logger.exception('PDU header parse error', header=header_data.hex())
             raise
         body_data: bytes = await self._reader.readexactly(header.pdu_length - PDU_HEADER_LENGTH)
@@ -276,17 +273,16 @@
         try:
             while True:
                 # Wait for interval to expire or data event to be triggered, whichever comes first.
                 # Receiver function will trigger the event after data is received.
                 sleep_task = asyncio.create_task(asyncio.sleep(self.enquire_link_interval))
                 event_task = asyncio.create_task(self._data_received.wait())
                 done: Set[Task]
-                done, _pending = await asyncio.wait({sleep_task, event_task},
-                                                    return_when=asyncio.FIRST_COMPLETED)
-                await next(iter(done)) # There must be only one element
+                done, _pending = await asyncio.wait({sleep_task, event_task}, return_when=asyncio.FIRST_COMPLETED)
+                await next(iter(done))  # There must be only one element
 
                 if self._is_shutting_down or self._session_state != self.bind_mode.session_state:
                     break
 
                 if sleep_task in done:
                     # Interval expired, send keep-alive message
                     asyncio.create_task(self._send_data(EnquireLink()))
@@ -318,55 +314,56 @@
 
         Parameters:
             smpp_message: Message to be sent
         '''
         # TODO: Look at `set_write_buffer_limits` and `get_write_buffer_limits` methods
         # print('get_write_buffer_limits:', writer.transport.get_write_buffer_limits())
 
-        self._logger.debug('Requested sending SMPP message',
-                           smpp_command=smpp_message.smpp_command.name)
+        self._logger.debug('Requested sending SMPP message', smpp_command=smpp_message.smpp_command.name)
 
         # Only bind-type commands can be sent in open state.
         # Otherwise, wait until we are in bound state.
         if not isinstance(smpp_message, (BindTransmitter, BindReceiver, BindTransceiver)):
             await self._bound.wait()
 
         if smpp_message.smpp_command in COMMAND_RESPONSE_MAP:
             # This is a request. A new sequence number must be generated,
             # and message saved for correlation with a response.
             sequence_num: int = self.sequence_generator.next_sequence()
             assert_valid_sequence(sequence_num)
             smpp_message.sequence_num = sequence_num
 
-        self._logger.debug('Sending SMPP message', smpp_command=smpp_message.smpp_command.name,
+        self._logger.debug('Sending SMPP message',
+                           smpp_command=smpp_message.smpp_command.name,
                            sequence_num=smpp_message.sequence_num)
 
         pdu: bytes = smpp_message.pdu()
-        await self.hook.sending(smpp_message, pdu, self.client_id) # Call user's hook
+        await self.hook.sending(smpp_message, pdu, self.client_id)  # Call user's hook
 
         # We use writer.drain() which is a flow control method that interacts with the
         # IO write buffer. When the size of the buffer reaches the high watermark,
         # drain blocks until the size of the buffer is drained down to the low watermark
         # and writing can be resumed.
         # When there is nothing to wait for, the drain() returns immediately.
         # ref: https://docs.python.org/3/library/asyncio-stream.html#asyncio.StreamWriter.drain
-        assert isinstance(self._writer, StreamWriter) # For type checkers
+        assert isinstance(self._writer, StreamWriter)  # For type checkers
         self._writer.write(pdu)
         async with self._drain_lock:
             # see: https://github.com/komuw/naz/issues/114
             await self._writer.drain()
 
-        self._logger.debug('Sent SMPP message', smpp_command=smpp_message.smpp_command.name,
+        self._logger.debug('Sent SMPP message',
+                           smpp_command=smpp_message.smpp_command.name,
                            sequence_num=smpp_message.sequence_num)
 
         if smpp_message.smpp_command in COMMAND_RESPONSE_MAP:
             # If no error occured, save correlation data
             self._logger.debug('Saving request correlation data',
-                                smpp_command=smpp_message.smpp_command,
-                                sequence_num=smpp_message.sequence_num)
+                               smpp_command=smpp_message.smpp_command,
+                               sequence_num=smpp_message.sequence_num)
             await self.correlator.put(smpp_message)
 
     async def _dequeue_messages(self) -> Dict:
         '''
         In a loop; dequeues items from the :attr:`broker <ESME.broker>` and sends them to SMSC.
         '''
         try:
@@ -384,26 +381,24 @@
                     if self.rate_limiter:
                         await self.rate_limiter.limit()
                     # Broker must never raise exception when dequeueing.
                     # It must handle exceptions internally and implement retry mechanism.
                     smpp_message: SmppMessage = await self.broker.dequeue()
                     if self.bind_mode == BindMode.RECEIVER:
                         if self._logger.isEnabledFor(WARNING):
-                            self._logger.warning('ESME bound as receiver. Message discarded.',
-                                                 message=smpp_message)
+                            self._logger.warning('ESME bound as receiver. Message discarded.', message=smpp_message)
                         continue
                     if isinstance(smpp_message, SubmitSm):
                         smpp_message.set_encoding_info(self.default_encoding, self.custom_codecs)
                     try:
                         await self._send_data(smpp_message)
-                    except Exception as err: # pylint: disable=broad-except
+                    except Exception as err:  # pylint: disable=broad-except
                         # We must intercept this exception to inform user application about failure
                         if self._logger.isEnabledFor(ERROR):
-                            self._logger.exception('SMPP message could not be sent',
-                                                   message=smpp_message)
+                            self._logger.exception('SMPP message could not be sent', message=smpp_message)
                         if isinstance(smpp_message, SubmitSm):
                             await self.hook.send_error(smpp_message, err, self.client_id)
                         # ValueError indicates problem with building the PDU, which is likely the
                         # result of invalid parameters passed by user application.
                         # Otherwise, it is a transport error and we must stop.
                         if not isinstance(err, ValueError):
                             raise
@@ -435,15 +430,15 @@
                     return None
 
                 self._logger.debug('Receive data cycle start')
 
                 pdu: bytes
                 header: PduHeader
                 pdu, header = await self._get_pdu()
-                self._data_received.set() # Inform connection keeper that data was received
+                self._data_received.set()  # Inform connection keeper that data was received
                 pdu_handler: Callable[[bytes, PduHeader], Awaitable[Optional[SmppMessage]]]
                 if header.smpp_command in COMMAND_RESPONSE_MAP:
                     pdu_handler = self._handle_request
                 else:
                     pdu_handler = self._handle_response
                 smpp_message: Optional[SmppMessage] = await pdu_handler(pdu, header)
 
@@ -474,64 +469,60 @@
 
         Parameters:
             pdu: PDU in bytes that have been read from network
             header: PduHeader instance containing data parsed from PDU header
         '''
         self._logger.debug('Handling SMPP response', header=header)
 
-        if header.smpp_command not in (SmppCommand.BIND_TRANSMITTER_RESP,
-                                       SmppCommand.BIND_RECEIVER_RESP,
-                                       SmppCommand.BIND_TRANSCEIVER_RESP,
-                                       SmppCommand.UNBIND_RESP, SmppCommand.SUBMIT_SM_RESP,
-                                       SmppCommand.ENQUIRE_LINK_RESP, SmppCommand.GENERIC_NACK):
+        if header.smpp_command not in (SmppCommand.BIND_TRANSMITTER_RESP, SmppCommand.BIND_RECEIVER_RESP,
+                                       SmppCommand.BIND_TRANSCEIVER_RESP, SmppCommand.UNBIND_RESP,
+                                       SmppCommand.SUBMIT_SM_RESP, SmppCommand.ENQUIRE_LINK_RESP,
+                                       SmppCommand.GENERIC_NACK):
             # This should not happen; we don't send any other requests
             self._logger.warning('Received unexpected SMPP response', header=header)
             return None
 
         original_command: Optional[SmppCommand] = RESPONSE_COMMAND_MAP[header.smpp_command]
-        original_message: Optional[SmppMessage] = await self.correlator.get(original_command,
-                                                                            header.sequence_num)
+        original_message: Optional[SmppMessage] = await self.correlator.get(original_command, header.sequence_num)
         if not original_message:
             # This should not happen
             self._logger.error('Could not correlate SMPP response', header=header)
-        elif (header.smpp_command != SmppCommand.GENERIC_NACK
-              and original_message.smpp_command != original_command):
+        elif (header.smpp_command != SmppCommand.GENERIC_NACK and original_message.smpp_command != original_command):
             # This should DEFINITELY not happen
             if self._logger.isEnabledFor(ERROR):
                 self._logger.error('SMPP response correlated to unrelated request',
-                                   header=header, request=original_message.__dict__)
+                                   header=header,
+                                   request=original_message.__dict__)
             return None
 
         message_class: Type[SmppMessage] = MESSAGE_TYPE_MAP[header.smpp_command]
         try:
             smpp_message: SmppMessage = message_class.from_pdu(pdu, header)
         except ValueError:
             if self._logger.isEnabledFor(ERROR):
                 self._logger.exception('Unable to parse PDU', header=header, pdu=pdu.hex())
             return None
         self._logger.debug('SMPP response parsed successfully', header=header)
 
         if isinstance(smpp_message, SubmitSmResp) and isinstance(original_message, SubmitSm):
             # Call throttling handler
-            if header.command_status in (SmppCommandStatus.ESME_RTHROTTLED,
-                                         SmppCommandStatus.ESME_RMSGQFUL):
+            if header.command_status in (SmppCommandStatus.ESME_RTHROTTLED, SmppCommandStatus.ESME_RMSGQFUL):
                 await self.throttle_handler.throttled()
             else:
                 await self.throttle_handler.not_throttled()
 
             # Response may be SubmitSmResp or GenericNack
             smpp_message.log_id = original_message.log_id
             smpp_message.extra_data = original_message.extra_data
-            if (isinstance(smpp_message, SubmitSmResp)
-                and header.command_status == SmppCommandStatus.ESME_ROK):
+            if (isinstance(smpp_message, SubmitSmResp) and header.command_status == SmppCommandStatus.ESME_ROK):
                 # The body of this only has `message_id` which is a C-Octet String
                 # of variable length up to 65 octets.  It may be used at a later stage
                 # to query the status of a message, cancel or replace the message.
                 # Take the full message body minus terminating NULL char
-                message_id_data: bytes = pdu[PDU_HEADER_LENGTH:header.pdu_length-1]
+                message_id_data: bytes = pdu[PDU_HEADER_LENGTH:header.pdu_length - 1]
                 smsc_message_id: str = message_id_data.decode('ascii')
                 self._logger.debug('Saving delivery receipt correlation data',
                                    smsc_message_id=smsc_message_id,
                                    log_id=original_message.log_id,
                                    extra_data=original_message.extra_data)
                 await self.correlator.put_delivery(
                     smsc_message_id=smsc_message_id,
@@ -549,25 +540,23 @@
 
         Parameters:
             pdu: PDU in bytes that have been read from network
             header: PduHeader instance containing data parsed from PDU header
         '''
         self._logger.debug('Handling SMPP request', header=header)
 
-        if header.smpp_command not in (SmppCommand.UNBIND, SmppCommand.ENQUIRE_LINK,
-                                       SmppCommand.DELIVER_SM):
+        if header.smpp_command not in (SmppCommand.UNBIND, SmppCommand.ENQUIRE_LINK, SmppCommand.DELIVER_SM):
             # This should not happen; we can't handle any other requests
             self._logger.warning('Received unexpected SMPP request', header=header)
             await self._send_data(GenericNack(header.sequence_num))
             return None
 
         message_class: Type[SmppMessage] = MESSAGE_TYPE_MAP[header.smpp_command]
         try:
-            smpp_message: SmppMessage = message_class.from_pdu(pdu, header, self.default_encoding,
-                                                               self.custom_codecs)
+            smpp_message: SmppMessage = message_class.from_pdu(pdu, header, self.default_encoding, self.custom_codecs)
         except ValueError:
             if self._logger.isEnabledFor(ERROR):
                 self._logger.exception('Unable to parse PDU', header=header, pdu=pdu.hex())
             await self._send_data(GenericNack(header.sequence_num))
             return None
         if isinstance(smpp_message, DeliverSm) and smpp_message.is_receipt():
             receipt: Dict[str, Any] = smpp_message.parse_receipt()
@@ -580,29 +569,29 @@
                 smpp_message.extra_data = extra_data
                 if log_id:
                     self._logger.debug('Correlated delivery receipt to SubmitSm',
                                        smsc_message_id=msg_id,
                                        log_id=log_id,
                                        extra_data=extra_data)
                 else:
-                    self._logger.warning('Could not correlate delivery receipt to SubmitSm',
-                                         smsc_message_id=msg_id)
+                    self._logger.warning('Could not correlate delivery receipt to SubmitSm', smsc_message_id=msg_id)
             else:
                 self._logger.warning('Could not get receipted message ID from delivery receipt',
-                                     header=header, receipt=receipt)
+                                     header=header,
+                                     receipt=receipt)
 
         self._logger.debug('Handled SMPP request', header=header)
         return smpp_message
 
     async def _disconnect(self) -> None:
         '''
         Drop connection to SMSC.
         '''
         if self._writer is None:
-            return # Already disconnected
+            return  # Already disconnected
         self._logger.debug('Closing network connection to SMSC')
         try:
             # 1. Set buffers to 0
             # 2. Unbind
             # 3. Drain
             # 4. Close connection
             # `start` function will await all tasks and set state to closed before it exits
@@ -622,16 +611,15 @@
         '''
         Open connection to SMSC and bind as a transceiver.
         '''
         if self._session_state == self.bind_mode.session_state:
             return
         self._logger.info('Initiating connection to SMSC')
         self._writer = None
-        conn_func = asyncio.open_connection(self.smsc_host, self.smsc_port,
-                                            limit=_NETWORK_BUFFER_LIMIT)
+        conn_func = asyncio.open_connection(self.smsc_host, self.smsc_port, limit=_NETWORK_BUFFER_LIMIT)
         self._reader, self._writer = await self._socket_operation(conn_func)
         self._session_state = SmppSessionState.OPEN
         self._logger.info('Connected to SMSC, trying to bind as a %s', self.bind_mode.description)
         bind_command: SmppCommand = self.bind_mode.smpp_command
         bind_request_cls: Type[SmppMessage] = MESSAGE_TYPE_MAP[bind_command]
         assert bind_request_cls in (BindTransmitter, BindReceiver, BindTransceiver)
         bind_request: SmppMessage = bind_request_cls(
@@ -653,16 +641,15 @@
         expected_response_command = COMMAND_RESPONSE_MAP[bind_command]
         if header.smpp_command != expected_response_command:
             raise SmppError(header.smpp_command, header.command_status)
         bind_response_cls: Type[SmppMessage] = MESSAGE_TYPE_MAP[expected_response_command]
         await self.hook.received(bind_response_cls.from_pdu(pdu, header), pdu, self.client_id)
         # ESME_RALYBND means that we are already bound.
         # This should not happen, but we cover it just in case.
-        if header.command_status not in (SmppCommandStatus.ESME_ROK,
-                                         SmppCommandStatus.ESME_RALYBND):
+        if header.command_status not in (SmppCommandStatus.ESME_ROK, SmppCommandStatus.ESME_RALYBND):
             self._session_state = SmppSessionState.CLOSED
             raise SmppError(header.smpp_command, header.command_status)
         self._session_state = self.bind_mode.session_state
         self._logger.info('Bound to SMSC as a %s', self.bind_mode.description)
 
     async def start(self) -> None:
         '''
@@ -673,27 +660,26 @@
         conn_error: Optional[Exception]
         all_tasks: Set[Task] = set()
         while True:
             try:
                 all_tasks.clear()
                 self._logger.debug('SMSC connect cycle start')
                 conn_error = None
-                await self.connect() # Will raise error if not successful
+                await self.connect()  # Will raise error if not successful
                 self.retry_timer.reset()
-                self._bound.set() # Tell _send_data it can proceed
+                self._bound.set()  # Tell _send_data it can proceed
                 # Wait until any task fails
                 all_tasks: Set[Task] = {
                     asyncio.create_task(self._receive_data(), name='Receiver'),
                     asyncio.create_task(self._dequeue_messages(), name='Sender'),
                     asyncio.create_task(self._connection_keeper(), name='Connection keeper'),
                 }
                 done_tasks: Set[Task] = set()
                 pending_tasks: Set[Task] = set()
-                done_tasks, pending_tasks = await asyncio.wait(all_tasks,
-                                                               return_when=asyncio.FIRST_COMPLETED)
+                done_tasks, pending_tasks = await asyncio.wait(all_tasks, return_when=asyncio.FIRST_COMPLETED)
                 self._session_state = SmppSessionState.CLOSED
                 task: Task
                 for task in done_tasks:
                     await self._end_task(task)
                 for task in pending_tasks:
                     await self._end_task(task)
             except SmppError as err:
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/hook.py` & `aiosmpplib-0.6.4/aiosmpplib/hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,15 @@
             smpp_message: Protocol message that is being sent
             pdu: The full PDU as sent to SMPP peer
             client_id: Client ID
         '''
         raise NotImplementedError()
 
     @abstractmethod
-    async def received(self, smpp_message: Optional[SmppMessage], pdu: bytes,
-                       client_id: str) -> None:
+    async def received(self, smpp_message: Optional[SmppMessage], pdu: bytes, client_id: str) -> None:
         '''
         Called after receiving data from SMPP peer.
 
         Parameters:
             smpp_message: Protocol message that was received, or None if PDU couldn't be parsed
             pdu: Full PDU as received from SMPP peer
             client_id: Client ID
@@ -66,15 +65,14 @@
         check_param(logger, 'logger', StructuredLogger)
         self.logger: StructuredLogger = logger
 
     async def sending(self, smpp_message: SmppMessage, pdu: bytes, client_id: str) -> None:
         if self.logger.isEnabledFor(TRACE):
             self.logger.trace(TRACE, 'Sending message', pdu=pdu.hex())
 
-    async def received(self, smpp_message: Optional[SmppMessage], pdu: bytes,
-                       client_id: str) -> None:
+    async def received(self, smpp_message: Optional[SmppMessage], pdu: bytes, client_id: str) -> None:
         if self.logger.isEnabledFor(TRACE):
             self.logger.trace('Received message', pdu=pdu.hex())
 
     async def send_error(self, smpp_message: SmppMessage, error: Exception, client_id: str) -> None:
         if self.logger.isEnabledFor(TRACE):
             self.logger.trace('Send error occured', exc_info=error)
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/jsonutils.py` & `aiosmpplib-0.6.4/aiosmpplib/jsonutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from datetime import datetime, timedelta
 from typing import Any, Dict, Type, Union
 from .protocol import SmppMessage, MESSAGE_TYPE_MAP
 from .state import SmppCommand
 try:
     import orjson
     from orjson import loads as json_loads
+
     def json_encode(obj: Any) -> str:
-        return orjson.dumps(obj, default=_json_default,
-                            option=orjson.OPT_PASSTHROUGH_DATACLASS).decode('utf-8')
+        return orjson.dumps(obj, default=_json_default, option=orjson.OPT_PASSTHROUGH_DATACLASS).decode('utf-8')
 except ImportError:
     import json
     from json import loads as json_loads
+
     def json_encode(obj: Any) -> str:
         return json.dumps(obj, default=_json_default)
 
 
 def _json_default(o: Any) -> Any:
     if isinstance(o, timedelta):
         return o.total_seconds()
@@ -35,9 +36,9 @@
     json_object: Dict[str, Any] = json_loads(json_data)
     if not isinstance(json_object, dict):
         raise ValueError('Invalid JSON string')
     smpp_command_str = json_object.get('__smpp_command__', '')
     if not smpp_command_str:
         raise ValueError('Invalid JSON object: not a SMPP message')
     smpp_command: SmppCommand = SmppCommand[smpp_command_str]
-    message_class: Type[SmppMessage]= MESSAGE_TYPE_MAP[smpp_command]
+    message_class: Type[SmppMessage] = MESSAGE_TYPE_MAP[smpp_command]
     return message_class.from_json(json_object)
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/log.py` & `aiosmpplib-0.6.4/aiosmpplib/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import datetime
 import time
 import logging
-from logging import (CRITICAL, DEBUG, ERROR, INFO, WARNING, Formatter, Handler, LogRecord, Logger,
-                     StreamHandler, handlers)
+from logging import (CRITICAL, DEBUG, ERROR, INFO, WARNING, Formatter, Handler, LogRecord, Logger, StreamHandler,
+                     handlers)
 from typing import Any, Deque, Dict, Optional, Union
 from collections import deque
 from .jsonutils import json_encode
 from .utils import check_param
 
-
-#def trace_to_root(message, *args, **kwargs):
-#    logging.log(TRACE, message, *args, **kwargs)
+# def trace_to_root(message, *args, **kwargs):
+#     logging.log(TRACE, message, *args, **kwargs)
 
 TRACE: int = logging.DEBUG - 5
 # Add TRACE level to logging module
 logging.addLevelName(TRACE, 'TRACE')
 setattr(logging, 'TRACE', TRACE)
-#setattr(logging, 'trace', trace_to_root)
+# setattr(logging, 'trace', trace_to_root)
 
 
 class StructuredLogger(Logger):
     '''
     It implements a structured logger that renders logs as JSON.
 
     example usage:
@@ -28,17 +27,21 @@
     .. highlight:: python
     .. code-block:: python
 
         logger = StructuredLogger('myLogger')
         logger.log(logging.INFO, event='web_request', url='https://www.google.com/')
     '''
 
-    def __init__(self, logger_name: str, level: Union[str, int]=INFO,
-                 log_metadata: Optional[Dict[str, Any]]=None, handler: Optional[Handler]=None,
-                 include_timestamp: bool=True, include_level: bool=True) -> None:
+    def __init__(self,
+                 logger_name: str,
+                 level: Union[str, int] = INFO,
+                 log_metadata: Optional[Dict[str, Any]] = None,
+                 handler: Optional[Handler] = None,
+                 include_timestamp: bool = True,
+                 include_level: bool = True) -> None:
         '''
         Parameters:
             logger_name: Name of the logger. It should be unique per logger.
             level: The level at which to log
             log_metadata: Metadata that will be included in all log statements
             handler: Python logging
                     `handler <https://docs.python.org/3/library/logging.html#logging.Handler>`_
@@ -80,31 +83,35 @@
         if self.isEnabledFor(WARNING):
             self._log(WARNING, msg, args, **kwargs)
 
     def error(self, msg: Any, *args, **kwargs):
         if self.isEnabledFor(ERROR):
             self._log(ERROR, msg, args, **kwargs)
 
-    def exception(self, msg: Any, *args, exc_info: bool=True, **kwargs):
+    def exception(self, msg: Any, *args, exc_info: bool = True, **kwargs):
         self.error(msg, *args, exc_info=exc_info, **kwargs)
 
     def critical(self, msg: Any, *args, **kwargs):
         if self.isEnabledFor(CRITICAL):
             self._log(CRITICAL, msg, args, **kwargs)
 
     def log(self, level: int, msg: Any, *args, **kwargs):
         assert isinstance(level, int)
         if self.isEnabledFor(level):
             self._log(level, msg, args, **kwargs)
 
     def _log(self, level: int, msg: Any, *args, **kwargs):
-        user_args: Dict = {key: value for key, value in kwargs.items()
-                           if key not in ('exc_info', 'extra', 'stack_info', 'stacklevel')}
-        logger_args: Dict = {key: value for key, value in kwargs.items()
-                             if key in ('exc_info', 'extra', 'stack_info', 'stacklevel')}
+        user_args: Dict = {
+            key: value
+            for key, value in kwargs.items() if key not in ('exc_info', 'extra', 'stack_info', 'stacklevel')
+        }
+        logger_args: Dict = {
+            key: value
+            for key, value in kwargs.items() if key in ('exc_info', 'extra', 'stack_info', 'stacklevel')
+        }
         if self.include_timestamp:
             user_args['timestamp'] = datetime.datetime.now().isoformat()
         if self.include_level:
             user_args['log_level'] = logging.getLevelName(level)
         new_msg: str = self._process_msg(msg, **user_args)
         return super()._log(level, new_msg, *args, **logger_args)
 
@@ -126,15 +133,15 @@
     def _to_json(self, input_msg: Dict) -> str:
         '''
         Tries to convert the input message to JSON and returns it.
         If it fails, it returns the error in string (not JSON) format.
         '''
         try:
             return json_encode(input_msg)
-        except Exception as err: # pylint: disable=broad-except
+        except Exception as err:  # pylint: disable=broad-except
             return f'aiosmpplib.StructuredLogger error: {repr(err)}'
 
 
 class BreachHandler(handlers.MemoryHandler):
     '''
     This is an implementation of `logging.Handler` that puts logs in an in-memory ring buffer.
     When a trigger condition(eg a certain log level) is met;
@@ -173,17 +180,21 @@
             logger.addHandler(handler)
         logger.setLevel('DEBUG')
 
         logger.info('I did records for Tweet before y'all could even tweet - Dr. Missy Elliot')
         logger.error('damn')
     '''
 
-    def __init__(self, flushLevel: int=WARNING, capacity: int=1000, target: Optional[Handler]=None,
-                 flushOnClose: bool=False, heartbeatInterval: Optional[float]=None,
-                 targetLevel: str='DEBUG') -> None:
+    def __init__(self,
+                 flushLevel: int = WARNING,
+                 capacity: int = 1000,
+                 target: Optional[Handler] = None,
+                 flushOnClose: bool = False,
+                 heartbeatInterval: Optional[float] = None,
+                 targetLevel: str = 'DEBUG') -> None:
         '''
         Parameters:
             flushLevel: the log level that will trigger this handler to
                         flush logs to :py:attr:`~target`
             capacity: the maximum number of log records to store in the ring buffer
             target: `log handler <https://docs.python.org/3/library/logging.html#logging.Handler>`_
                     that will be used.
@@ -219,15 +230,15 @@
 
         self.heartbeatInterval = heartbeatInterval
         if self.heartbeatInterval:
             self.heartbeatInterval = heartbeatInterval  # seconds
             self._s_time = time.monotonic()
 
         self.targetLevel: int = StructuredLogger._check_level(targetLevel)
-        assert self.target is not None # For type checkers
+        assert self.target is not None  # For type checkers
         self.target.setLevel(self.targetLevel)
 
     def shouldFlush(self, record: LogRecord) -> bool:
         '''
         Check for record at the flushLevel or higher.
         Implementation is mostly taken from `logging.handlers.MemoryHandler`
         '''
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/protocol.py` & `aiosmpplib-0.6.4/aiosmpplib/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from codecs import CodecInfo
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from math import floor
 from struct import pack, unpack_from
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from .codec import find_codec_info
-from .state import (NPI, TON, OptionalParam, OptionalTag, PhoneNumber, SmppCommand,
-                    SmppCommandStatus, SmppDataCoding, PduHeader)
+from .state import (NPI, TON, OptionalParam, OptionalTag, PhoneNumber, SmppCommand, SmppCommandStatus, SmppDataCoding,
+                    PduHeader)
 from .utils import check_param, FixedOffset
 
-
 NULL = b'\x00'
 PDU_HEADER_LENGTH: int = 16
 SMPP_VERSION_3_4: int = 0x34
 DEFAULT_ENCODING: str = 'gsm0338'
 
 
 class Base(ABC):
+
     def __post_init__(self):
         # Intercept the __post_init__ calls so they aren't relayed to `object`
         pass
 
 
 @dataclass
 class Trackable(Base):
@@ -81,31 +81,32 @@
         '''
         # First 16 bytes always contain:
         # PDU length, command ID, status, and sequence number, 4 bytes each
         pdu_length: int = unpack_from('!I', header_data)[0]
         command_id: int = unpack_from('!I', header_data, 4)[0]
         command_status_id: int = unpack_from('!I', header_data, 8)[0]
         sequence_num: int = unpack_from('!I', header_data, 12)[0]
-        return PduHeader(
-            pdu_length=pdu_length,
-            smpp_command=SmppCommand(command_id),
-            command_status=SmppCommandStatus(command_status_id),
-            sequence_num=sequence_num
-        )
+        return PduHeader(pdu_length=pdu_length,
+                         smpp_command=SmppCommand(command_id),
+                         command_status=SmppCommandStatus(command_status_id),
+                         sequence_num=sequence_num)
 
     def pdu(self) -> bytes:
         '''
         Returns message representation as SMPP PDU (encoded to binary data)
         '''
         # Many messages have empty body, so this is a default
         return self.pack_header(PDU_HEADER_LENGTH)
 
     @classmethod
-    def from_pdu(cls, pdu: bytes, header: PduHeader, default_encoding: str='',
-                 custom_codecs: Optional[Dict[str, CodecInfo]]=None) -> SmppMessage:
+    def from_pdu(cls,
+                 pdu: bytes,
+                 header: PduHeader,
+                 default_encoding: str = '',
+                 custom_codecs: Optional[Dict[str, CodecInfo]] = None) -> SmppMessage:
         '''
         Creates SmppMessage object from data parsed from byte sequence.
         PDU header needs to be pre-parsed because it contains PDU length and command type.
 
         Parameters:
             pdu: PDU in bytes that have been read from network
             header: PduHeader instance containing data parsed from PDU header
@@ -159,20 +160,20 @@
         auto_message_payload: Automatically use message_payload if message
                               does not fit in short_message
         error_handling: same meaning as the `errors` argument to Python's
                         `encode <https://docs.python.org/3/library/codecs.html#codecs.encode>`_
                         method
     '''
     short_message: str = ''
-    source: PhoneNumber = PhoneNumber('')
-    destination: PhoneNumber = PhoneNumber('')
+    source: PhoneNumber = field(default_factory=lambda: PhoneNumber(''))
+    destination: PhoneNumber = field(default_factory=lambda: PhoneNumber(''))
     service_type: str = ''
     esm_class: int = 0x00000000
     protocol_id: int = 0x00000000
-    priority_flag:int = 0x00000000
+    priority_flag: int = 0x00000000
     schedule_delivery_time: Optional[Union[datetime, timedelta]] = None
     validity_period: Optional[Union[datetime, timedelta]] = None
     registered_delivery: int = 0b00000001
     replace_if_present_flag: int = 0x00000000
     encoding: Optional[str] = None
     sm_default_msg_id: int = 0x00000000
     message_payload: str = ''
@@ -184,16 +185,15 @@
         check_param(self.short_message, 'short_message', str)
         check_param(self.source, 'source', PhoneNumber)
         check_param(self.destination, 'destination', PhoneNumber)
         check_param(self.service_type, 'service_type', str, maxlen=5)
         check_param(self.esm_class, 'esm_class', int)
         check_param(self.protocol_id, 'protocol_id', int)
         check_param(self.priority_flag, 'priority_flag', int)
-        check_param(self.schedule_delivery_time, 'schedule_delivery_time', (datetime, timedelta),
-                    optional=True)
+        check_param(self.schedule_delivery_time, 'schedule_delivery_time', (datetime, timedelta), optional=True)
         check_param(self.validity_period, 'validity_period', (datetime, timedelta), optional=True)
         check_param(self.registered_delivery, 'registered_delivery', int)
         check_param(self.replace_if_present_flag, 'replace_if_present_flag', int)
         check_param(self.encoding, 'encoding', str, optional=True)
         check_param(self.sm_default_msg_id, 'sm_default_msg_id', int)
         check_param(self.message_payload, 'message_payload', str)
         check_param(self.optional_params, 'optional_params', list, optional=True)
@@ -232,16 +232,15 @@
             time_object: A datetime or timedelta instance.
         '''
         if time_object is None:
             return ''
         if isinstance(time_object, datetime):
             # datetime is converted to absolute validity
             tenth_second: str = str(time_object.microsecond // 100000)
-            offset: Optional[timedelta] = (time_object.tzinfo.utcoffset(time_object)
-                                           if time_object.tzinfo else None)
+            offset: Optional[timedelta] = (time_object.tzinfo.utcoffset(time_object) if time_object.tzinfo else None)
             offset_str: str
             prefix: str
             if not offset:
                 offset_str = '00'
                 prefix = '+'
             else:
                 # Unit is quarter-hour (15 minutes)
@@ -299,16 +298,15 @@
             hour=hour,
             minute=minute,
             second=second,
             microsecond=tenth_second * 1000000,
             tzinfo=offset,
         )
 
-    def set_encoding_info(self, default_encoding: str,
-                          custom_codecs: Optional[Dict[str, CodecInfo]]) -> None:
+    def set_encoding_info(self, default_encoding: str, custom_codecs: Optional[Dict[str, CodecInfo]]) -> None:
         '''
         Sets info neccessary for encoding message text.
 
         Parameters:
             default_encoding: SMSC default encoding.
             custom_codecs: User-provided codecs, if any.
         '''
@@ -340,75 +338,75 @@
         # If encoding is set to auto, smpp_encode will set encoding param of the message
         # to ucs2 if default encoding cannot be used
         encoded_short_message: bytes = self.smpp_encode(self.short_message or self.message_payload)
         encoded_message_payload: bytes = b''
         if self.encoding:
             data_coding: int = SmppDataCoding[self.encoding].value
         else:
-            data_coding: int = 0 # SMSC default
+            data_coding: int = 0  # SMSC default
         sm_length: int = len(encoded_short_message)
         if sm_length > 254 and self.short_message and not self.auto_message_payload:
             # short_message supports up to 254 bytes, so this does not fit,
             # but automatic moving to message_payload was deactivated
             raise ValueError(f'Message is too long ({sm_length} bytes, maximum is 254)')
         if sm_length > 254 or self.message_payload:
             tag: int = OptionalTag.MESSAGE_PAYLOAD.value
             encoded_message_payload = pack('!HH', tag, sm_length) + encoded_short_message
             encoded_short_message = b''
             sm_length = 0
 
         body: bytes = (
-            self.service_type.encode('ascii') + NULL
-            + pack('!BB', self.source.ton, self.source.npi)
-            + self.source.number.encode('ascii') + NULL
-            + pack('!BB', self.destination.ton, self.destination.npi)
-            + self.destination.number.encode('ascii') + NULL
-            + pack('!BBB', self.esm_class, self.protocol_id, self.priority_flag)
-            + self.datetime_to_smpp_time(self.schedule_delivery_time).encode('ascii') + NULL
-            + self.datetime_to_smpp_time(self.validity_period).encode('ascii') + NULL
-            + pack('!BB', self.registered_delivery, self.replace_if_present_flag)
-            + pack('!BBB', data_coding, self.sm_default_msg_id, sm_length)
-            + encoded_short_message
-            + encoded_message_payload
-            + b''.join(opt_param.tlv for opt_param in self.optional_params or [])
+            self.service_type.encode('ascii') + NULL + pack('!BB', self.source.ton, self.source.npi) +
+            self.source.number.encode('ascii') + NULL + pack('!BB', self.destination.ton, self.destination.npi) +
+            self.destination.number.encode('ascii') + NULL +
+            pack('!BBB', self.esm_class, self.protocol_id, self.priority_flag) +
+            self.datetime_to_smpp_time(self.schedule_delivery_time).encode('ascii') + NULL +
+            self.datetime_to_smpp_time(self.validity_period).encode('ascii') + NULL +
+            pack('!BB', self.registered_delivery, self.replace_if_present_flag) +
+            pack('!BBB', data_coding, self.sm_default_msg_id, sm_length) + encoded_short_message +
+            encoded_message_payload + b''.join(opt_param.tlv for opt_param in self.optional_params or [])
             # optional params may be included in ANY ORDER within
             # the `Optional Parameters` section of the SMPP PDU.
         )
         return self.pack_header(PDU_HEADER_LENGTH + len(body)) + body
 
     @classmethod
-    def from_pdu(cls, pdu: bytes, header: PduHeader, default_encoding: str='',
-                 custom_codecs: Optional[Dict[str, CodecInfo]]=None) -> SmppMessage:
+    def from_pdu(cls,
+                 pdu: bytes,
+                 header: PduHeader,
+                 default_encoding: str = '',
+                 custom_codecs: Optional[Dict[str, CodecInfo]] = None) -> SmppMessage:
+
         def get_c_octet_string() -> str:
             nonlocal index
             str_end: int = pdu.index(NULL, index)
             octet_string: str = pdu[index:str_end].decode('ascii')
             index = str_end + 1
             return octet_string
 
         def get_octet_string(count: int) -> str:
             nonlocal index
-            octet_string: str = pdu[index:index+count].decode('ascii')
-            if octet_string.endswith(chr(0)): # String may be null-terminated
+            octet_string: str = pdu[index:index + count].decode('ascii')
+            if octet_string.endswith(chr(0)):  # String may be null-terminated
                 octet_string = octet_string[:-1]
             index += count
             return octet_string
 
         def get_integer(count: int) -> int:
             nonlocal index
             int_format: Dict[int, str] = {
-                1: '!B', # unsigned char
-                2: '!H', # unsigned short
-                4: '!I', # unsigned int
+                1: '!B',  # unsigned char
+                2: '!H',  # unsigned short
+                4: '!I',  # unsigned int
             }
             integer: int = unpack_from(int_format[count], pdu, index)[0]
             index += count
             return integer
 
-        index: int = PDU_HEADER_LENGTH # Only body is parsed here, header is pre-parsed
+        index: int = PDU_HEADER_LENGTH  # Only body is parsed here, header is pre-parsed
         service_type: str = get_c_octet_string()
         source_ton: TON = TON(get_integer(1))
         source_npi: NPI = NPI(get_integer(1))
         source: PhoneNumber = PhoneNumber(get_c_octet_string(), source_ton, source_npi)
         dest_ton: TON = TON(get_integer(1))
         dest_npi: NPI = NPI(get_integer(1))
         destination: PhoneNumber = PhoneNumber(get_c_octet_string(), dest_ton, dest_npi)
@@ -423,26 +421,26 @@
         if data_coding:
             encoding: str = SmppDataCoding(data_coding).name
         else:
             encoding: str = default_encoding
         codec_info: CodecInfo = find_codec_info(encoding, custom_codecs)
         sm_default_msg_id: int = get_integer(1)
         sm_length: int = get_integer(1)
-        short_message: str = codec_info.decode(pdu[index:index+sm_length])[0]
+        short_message: str = codec_info.decode(pdu[index:index + sm_length])[0]
         index += sm_length
 
         message_payload: str = ''
         # Read optional parameters, if any
         optional_params: List[OptionalParam] = []
         while index < header.pdu_length:
             tag: OptionalTag = OptionalTag(get_integer(2))
             length: int = get_integer(2)
             if tag == OptionalTag.MESSAGE_PAYLOAD:
                 # message_payload is a special case, it is an alternative to short_message
-                message_payload = codec_info.decode(pdu[index:index+length])[0]
+                message_payload = codec_info.decode(pdu[index:index + length])[0]
                 index += length
             elif tag.data_type == int:
                 int_value: int = get_integer(length)
                 optional_params.append(OptionalParam(tag, int_value))
             elif tag.data_type == bool:
                 # alert_on_message_delivery doesn't have an actual value (it is zero-length),
                 # but is a bool param, so we set it to True
@@ -470,21 +468,18 @@
             message_payload=message_payload,
             optional_params=optional_params,
         )
 
     @classmethod
     def from_json(cls, json_object: Dict[str, Any]) -> SmppMessage:
         source_dict: Dict[str, Any] = json_object['source']
-        source: PhoneNumber = PhoneNumber(
-            source_dict['number'], TON(source_dict['ton']), NPI(source_dict['npi'])
-        )
+        source: PhoneNumber = PhoneNumber(source_dict['number'], TON(source_dict['ton']), NPI(source_dict['npi']))
         destination_dict: Dict[str, Any] = json_object['destination']
-        destination: PhoneNumber = PhoneNumber(
-            destination_dict['number'], TON(destination_dict['ton']), NPI(destination_dict['npi'])
-        )
+        destination: PhoneNumber = PhoneNumber(destination_dict['number'], TON(destination_dict['ton']),
+                                               NPI(destination_dict['npi']))
         schedule_delivery_time: Optional[Union[datetime, timedelta]]
         if isinstance(json_object['schedule_delivery_time'], str):
             schedule_delivery_time = datetime.fromisoformat(json_object['schedule_delivery_time'])
         elif isinstance(json_object['schedule_delivery_time'], float):
             schedule_delivery_time = timedelta(seconds=json_object['schedule_delivery_time'])
         else:
             schedule_delivery_time = None
@@ -544,19 +539,22 @@
         return SmppCommand.SUBMIT_SM_RESP
 
     def pdu(self) -> bytes:
         body: bytes = self.message_id.encode('ascii') + NULL
         return self.pack_header(PDU_HEADER_LENGTH + len(body)) + body
 
     @classmethod
-    def from_pdu(cls, pdu: bytes, header: PduHeader, default_encoding: str='',
-                 custom_codecs: Optional[Dict[str, CodecInfo]]=None) -> SmppMessage:
+    def from_pdu(cls,
+                 pdu: bytes,
+                 header: PduHeader,
+                 default_encoding: str = '',
+                 custom_codecs: Optional[Dict[str, CodecInfo]] = None) -> SmppMessage:
         # pylint: disable=unused-argument
         # Decode the full body of the PDU, minus terminating NULL char
-        message_id: str = pdu[PDU_HEADER_LENGTH:header.pdu_length-1].decode('ascii')
+        message_id: str = pdu[PDU_HEADER_LENGTH:header.pdu_length - 1].decode('ascii')
         return cls(
             sequence_num=header.sequence_num,
             command_status=header.command_status,
             message_id=message_id,
         )
 
     @classmethod
@@ -569,14 +567,15 @@
 
 
 @dataclass
 class DeliverSm(SubmitSm):
     '''
     Represents the deliver_sm SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.DELIVER_SM
 
     def is_receipt(self) -> bool:
         '''
         Checks if this DeliverSm is a delivery receipt.
@@ -595,15 +594,15 @@
             nonlocal index
             str_end: int = self.short_message.find(':', index)
             if str_end == -1:
                 return None, None
             param: str = self.short_message[index:str_end].lower()
             index = str_end + 1
             str_end = self.short_message.find(' ', index)
-            if str_end == -1 or param == 'text': # Text must be last
+            if str_end == -1 or param == 'text':  # Text must be last
                 str_end = len(self.short_message)
             value: str = self.short_message[index:str_end]
             index = str_end + 1
             return param, value
 
         rcpt_data: Dict[str, Any] = {}
         index: int = 0
@@ -618,67 +617,67 @@
             elif rcpt_param in ('submit date', 'done date'):
                 rcpt_data[rcpt_param] = datetime.strptime(rcpt_value, '%y%m%d%H%M')
             elif rcpt_param in ('id', 'stat', 'err', 'text'):
                 rcpt_data[rcpt_param] = rcpt_value
             else:
                 rcpt_data[rcpt_param] = rcpt_value
 
-        smsc_message_id: Optional[str] = rcpt_data.get('id') # Get message ID from report data
+        smsc_message_id: Optional[str] = rcpt_data.get('id')  # Get message ID from report data
         if not smsc_message_id and self.optional_params:
             # Message ID not found, check if receipted_message_id param exists
-            id_param: Optional[OptionalParam] = next((
-                param for param in self.optional_params
-                if param.tag == OptionalTag.RECEIPTED_MESSAGE_ID
-            ), None)
+            id_param: Optional[OptionalParam] = next(
+                (param for param in self.optional_params if param.tag == OptionalTag.RECEIPTED_MESSAGE_ID), None)
             if id_param:
                 rcpt_data['id'] = id_param.value
 
         return rcpt_data
 
     @staticmethod
     def encode_receipt(rcpt_data: Dict[str, Any]) -> str:
         '''
         Encodes receipt dictionary in text.
 
         Parameters:
             rcpt_data: A dictionary containing receipt data.
         '''
         # Receipt format is SMSC-specific, but it usually follows the following pattern
-        msg_id: str = rcpt_data.get('id', '') # Message ID allocated by the SMSC when submitted.
-        sub: int = rcpt_data.get('sub', 0) # Number of short messages originally submitted.
-        dlvrd: int = rcpt_data.get('dlvrd', 0) # Number of short messages delivered.
+        msg_id: str = rcpt_data.get('id', '')  # Message ID allocated by the SMSC when submitted.
+        sub: int = rcpt_data.get('sub', 0)  # Number of short messages originally submitted.
+        dlvrd: int = rcpt_data.get('dlvrd', 0)  # Number of short messages delivered.
         # The time and date at which the message was submitted.
         submit_date: Optional[datetime] = rcpt_data.get('submit date')
         submit_date_str: str = submit_date.strftime('%y%m%d%H%M') if submit_date else ''
         # The time and date at which the message reached its final state.
         done_date: Optional[datetime] = rcpt_data.get('done date')
         done_date_str: str = done_date.strftime('%y%m%d%H%M') if done_date else ''
-        stat: str = rcpt_data.get('stat', '') # The final status of the message.
-        err: str = rcpt_data.get('err', '') # Network specific error code or an SMSC error code.
-        text: str = rcpt_data.get('text', '') # The first 20 characters of the short message.
+        stat: str = rcpt_data.get('stat', '')  # The final status of the message.
+        err: str = rcpt_data.get('err', '')  # Network specific error code or an SMSC error code.
+        text: str = rcpt_data.get('text', '')  # The first 20 characters of the short message.
         return (f'id:{msg_id} sub:{sub:03d} dlvrd:{dlvrd:03d}'
                 f' submit date:{submit_date_str} done date:{done_date_str}'
                 f' stat:{stat} err:{err} Text:{text:20}')
 
 
 @dataclass
 class DeliverSmResp(SubmitSmResp):
     '''
     Represents the deliver_sm_resp SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.DELIVER_SM_RESP
 
 
 @dataclass
 class GenericNack(Trackable, SmppMessage):
     '''
     Represents the generic_nack SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.GENERIC_NACK
 
 
 @dataclass
 class BindTransceiver(SmppMessage):
@@ -713,41 +712,41 @@
         check_param(self.address_range, 'address_range', str, maxlen=40)
 
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.BIND_TRANSCEIVER
 
     def pdu(self) -> bytes:
-        body: bytes = (
-            self.system_id.encode('ascii') + NULL
-            + self.password.encode('ascii') + NULL
-            + self.system_type.encode('ascii') + NULL
-            + pack('!BBB', self.interface_version, self.addr_ton, self.addr_npi)
-            + self.address_range.encode('ascii') + NULL
-        )
+        body: bytes = (self.system_id.encode('ascii') + NULL + self.password.encode('ascii') + NULL +
+                       self.system_type.encode('ascii') + NULL +
+                       pack('!BBB', self.interface_version, self.addr_ton, self.addr_npi) +
+                       self.address_range.encode('ascii') + NULL)
         return self.pack_header(PDU_HEADER_LENGTH + len(body)) + body
 
     @classmethod
-    def from_pdu(cls, pdu: bytes, header: PduHeader, default_encoding: str='',
-                 custom_codecs: Optional[Dict[str, CodecInfo]]=None) -> SmppMessage:
+    def from_pdu(cls,
+                 pdu: bytes,
+                 header: PduHeader,
+                 default_encoding: str = '',
+                 custom_codecs: Optional[Dict[str, CodecInfo]] = None) -> SmppMessage:
         # pylint: disable=unused-argument
         def get_c_octet_string() -> str:
             nonlocal index
             str_end: int = pdu.index(NULL, index)
             octet_string: str = pdu[index:str_end].decode('ascii')
             index = str_end + 1
             return octet_string
 
         def get_char() -> int:
             nonlocal index
             integer: int = unpack_from('!B', pdu, index)[0]
             index += 1
             return integer
 
-        index: int = PDU_HEADER_LENGTH # Only body is parsed here, header is pre-parsed
+        index: int = PDU_HEADER_LENGTH  # Only body is parsed here, header is pre-parsed
         system_id: str = get_c_octet_string()
         password: str = get_c_octet_string()
         system_type: str = get_c_octet_string()
         interface_version: int = get_char()
         addr_ton: TON = TON(get_char())
         addr_npi: NPI = NPI(get_char())
         address_range: str = get_c_octet_string()
@@ -800,16 +799,19 @@
     def pdu(self) -> bytes:
         body: bytes = self.system_id.encode('ascii') + NULL
         if self.sc_interface_version is not None:
             body += OptionalParam(OptionalTag.SC_INTERFACE_VERSION, self.sc_interface_version).tlv
         return self.pack_header(PDU_HEADER_LENGTH + len(body)) + body
 
     @classmethod
-    def from_pdu(cls, pdu: bytes, header: PduHeader, default_encoding: str='',
-                 custom_codecs: Optional[Dict[str, CodecInfo]]=None) -> SmppMessage:
+    def from_pdu(cls,
+                 pdu: bytes,
+                 header: PduHeader,
+                 default_encoding: str = '',
+                 custom_codecs: Optional[Dict[str, CodecInfo]] = None) -> SmppMessage:
         # pylint: disable=unused-argument
         index: int = pdu.index(NULL, PDU_HEADER_LENGTH)
         system_id: str = pdu[PDU_HEADER_LENGTH:index].decode('ascii')
         index += 1
         sc_interface_version: Optional[int] = None
         if index < header.pdu_length:
             # Optional param sc_interface_version. It must have a total of 5 bytes in length.
@@ -834,84 +836,92 @@
 
 
 @dataclass
 class BindTransmitter(BindTransceiver):
     '''
     Represents the bind_transmitter SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.BIND_TRANSMITTER
 
 
 @dataclass
 class BindTransmitterResp(BindTransceiverResp):
     '''
     Represents the bind_transmitter_resp SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.BIND_TRANSMITTER_RESP
 
 
 @dataclass
 class BindReceiver(BindTransceiver):
     '''
     Represents the bind_receiver SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.BIND_RECEIVER
 
 
 @dataclass
 class BindReceiverResp(BindTransceiverResp):
     '''
     Represents the bind_receiver_resp SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.BIND_RECEIVER_RESP
 
 
 @dataclass
 class EnquireLink(SmppMessage):
     '''
     Represents the enquire_link SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.ENQUIRE_LINK
 
 
 @dataclass
 class EnquireLinkResp(SmppMessage):
     '''
     Represents the enquire_link_resp SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.ENQUIRE_LINK_RESP
 
 
 @dataclass
 class Unbind(SmppMessage):
     '''
     Represents the unbind SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.UNBIND
 
 
 @dataclass
 class UnbindResp(SmppMessage):
     '''
     Represents the unbind_resp SMPP message type.
     '''
+
     @property
     def smpp_command(self) -> SmppCommand:
         return SmppCommand.UNBIND_RESP
 
 
 MESSAGE_TYPE_MAP: Dict[SmppCommand, Type[SmppMessage]] = {
     SmppCommand.GENERIC_NACK: GenericNack,
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/ratelimiter.py` & `aiosmpplib-0.6.4/aiosmpplib/ratelimiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     .. code-block:: python
 
         rate_limiter = SimpleRateLimiter(send_rate=10)
         await rate_limiter.limit()
         send_messages()
     '''
 
-    def __init__(self, logger: StructuredLogger, send_rate: float=100000.00) -> None:
+    def __init__(self, logger: StructuredLogger, send_rate: float = 100000.00) -> None:
         '''
         Parameters:
             logger: A python `logger <https://docs.python.org/3/library/html#Logger>`_
                     instance to be used for logging
             send_rate: The maximum rate, in messages/second, at which messages can be sent to SMSC.
         '''
         check_param(logger, 'logger', StructuredLogger)
@@ -60,15 +60,16 @@
         self.messages_delivered: int = 0
         self.effective_send_rate: float = 0.00
 
     async def limit(self) -> None:
         self.logger.debug('Rate limiter checking if request should be delayed.')
         while self.tokens < 1:
             self._add_new_tokens()
-            self.logger.debug('Rate limiter delayed the request.',
+            self.logger.debug(
+                'Rate limiter delayed the request.',
                 delay=self.delay_for_tokens,
                 send_rate=self.send_rate,
                 effective_send_rate=self.effective_send_rate,
             )
             # todo: sleep in an exponential manner up to a maximum then wrap around.
             await asyncio.sleep(self.delay_for_tokens)
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/retrytimer.py` & `aiosmpplib-0.6.4/aiosmpplib/retrytimer.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 class SimpleExponentialBackoff(AbstractRetryTimer):
     '''
     This is an implementation of AbstractRetryTimer using simple truncated exponential backoff.
     Retry delay starts at the minimum and is doubled up to the maximum.
     '''
 
-    def __init__(self, min_delay: int=1000, max_increases: int=5) -> None:
+    def __init__(self, min_delay: int = 1000, max_increases: int = 5) -> None:
         '''
         Parameters:
             min_delay: Minimum (starting) delay in milliseconds.
             max_increases: Maximum times to double the initial (minimum) delay.
         '''
         check_param(min_delay, 'min_delay', int)
         check_param(max_increases, 'max_increases', int)
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/sequence.py` & `aiosmpplib-0.6.4/aiosmpplib/sequence.py`

 * *Files identical despite different names*

### Comparing `aiosmpplib-0.6.3/aiosmpplib/state.py` & `aiosmpplib-0.6.4/aiosmpplib/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,30 +32,31 @@
     SUBMIT_MULTI = 0x00000021
     SUBMIT_MULTI_RESP = 0x80000021
     OUTBIND = 0x0000000B
     ALERT_NOTIFICATION = 0x00000102
     DATA_SM = 0x00000103
     DATA_SM_RESP = 0x80000103
 
+
 COMMAND_RESPONSE_MAP: Dict[SmppCommand, SmppCommand] = {
     SmppCommand.BIND_RECEIVER: SmppCommand.BIND_RECEIVER_RESP,
     SmppCommand.BIND_TRANSMITTER: SmppCommand.BIND_TRANSMITTER_RESP,
     SmppCommand.BIND_TRANSCEIVER: SmppCommand.BIND_TRANSCEIVER_RESP,
     SmppCommand.UNBIND: SmppCommand.UNBIND_RESP,
     SmppCommand.SUBMIT_SM: SmppCommand.SUBMIT_SM_RESP,
     SmppCommand.DELIVER_SM: SmppCommand.DELIVER_SM_RESP,
     SmppCommand.ENQUIRE_LINK: SmppCommand.ENQUIRE_LINK_RESP,
     SmppCommand.QUERY_SM: SmppCommand.QUERY_SM_RESP,
     SmppCommand.REPLACE_SM: SmppCommand.REPLACE_SM_RESP,
     SmppCommand.CANCEL_SM: SmppCommand.CANCEL_SM_RESP,
     SmppCommand.SUBMIT_MULTI: SmppCommand.SUBMIT_MULTI_RESP,
     SmppCommand.DATA_SM: SmppCommand.DATA_SM_RESP,
 }
-RESPONSE_COMMAND_MAP: Dict[SmppCommand, SmppCommand] = {resp: comm for comm, resp
-                                                        in COMMAND_RESPONSE_MAP.items()}
+RESPONSE_COMMAND_MAP: Dict[SmppCommand, SmppCommand] = {resp: comm for comm, resp in COMMAND_RESPONSE_MAP.items()}
+
 
 class SmppCommandStatus(IntEnum):
     '''
     Represents the various SMPP commands statuses.
     '''
 
     # See section 5.1.3 of SMPP ver 3.4 spec document
@@ -201,15 +202,15 @@
             return 'Invalid Parameter Length.'
         if self.value == 0x000000C3:
             return 'Expected Optional Parameter missing'
         if self.value == 0x000000C4:
             return 'Invalid Optional Parameter Value'
         if self.value == 0x000000FE:
             return 'Delivery Failure (used for data_sm_resp)'
-        return 'Unknown Error' # self.value == 0x000000FF
+        return 'Unknown Error'  # self.value == 0x000000FF
 
 
 class SmppSessionState(IntEnum):
     '''
     Represensts the states in which an SMPP session can be in.
     '''
     # See section 2.2 of SMPP spec document v3.4
@@ -315,15 +316,15 @@
             return 'UCS2(ISO / IEC - 10646)'
         if self.value == 0b00001000:
             return 'UCS2(ISO / IEC - 10646)'
         if self.value == 0b00001001:
             return 'Pictogram Encoding'
         if self.value == 0b00001010:
             return 'ISO - 2022 - JP(Music Codes)'
-        return 'KS C 5601' # self.value == 0b00001110
+        return 'KS C 5601'  # self.value == 0b00001110
 
 
 class OptionalTag(IntEnum):
     '''
     Represents SMPP optional tag.
 
     see section 5.3.2 of SMPP ver 3.4 spec document.
@@ -459,21 +460,19 @@
     # its_session_info: It contains control information for the interactive session
     #                   between an MS and an ESME. It is a required parameter for the CDMA
     #                   Interactive Teleservice as defined by the Korean PCS carriers [KORITS].
     ITS_SESSION_INFO = 0x1383
 
     @property
     def data_type(self) -> Type:
-        if self.value in (0x001D, 0x001E, 0x0202, 0x0203, 0x0303,
-                          0x0381, 0x0423, 0x0424, 0x0501, 0x1383):
+        if self.value in (0x001D, 0x001E, 0x0202, 0x0203, 0x0303, 0x0381, 0x0423, 0x0424, 0x0501, 0x1383):
             return str
-        if self.value in (0x0005, 0x0006, 0x0007, 0x0008, 0x000D, 0x000E, 0x000F, 0x0010, 0x0017,
-                          0x0019, 0x0030, 0x0201, 0x0204, 0x0205, 0x020A, 0x020B, 0x020C, 0x020D,
-                          0x020E, 0x020F, 0x0210, 0x0302, 0x0304, 0x0420, 0x0421, 0x0422, 0x0425,
-                          0x0426, 0x0427, 0x1201, 0x1203, 0x1204, 0x1380):
+        if self.value in (0x0005, 0x0006, 0x0007, 0x0008, 0x000D, 0x000E, 0x000F, 0x0010, 0x0017, 0x0019, 0x0030,
+                          0x0201, 0x0204, 0x0205, 0x020A, 0x020B, 0x020C, 0x020D, 0x020E, 0x020F, 0x0210, 0x0302,
+                          0x0304, 0x0420, 0x0421, 0x0422, 0x0425, 0x0426, 0x0427, 0x1201, 0x1203, 0x1204, 0x1380):
             return int
         if self.value == 0x130C:
             # ALERT_ON_MESSAGE_DELIVERY doesn't actually have any value.
             # We use bool to indicate whether the parameter should be set.
             return bool
 
 
@@ -523,89 +522,63 @@
 
     @property
     def length(self) -> int:
         '''
         Returns the Value field of an optional SMPP parameter.
         The Length field indicates the length of the Value field in octets(integer).
         '''
-        if self.tag in (OptionalTag.DEST_ADDR_SUBUNIT,
-                        OptionalTag.DEST_NETWORK_TYPE,
-                        OptionalTag.DEST_BEARER_TYPE,
-                        OptionalTag.SOURCE_ADDR_SUBUNIT,
-                        OptionalTag.SOURCE_NETWORK_TYPE,
-                        OptionalTag.SOURCE_BEARER_TYPE,
-                        OptionalTag.SOURCE_TELEMATICS_ID,
-                        OptionalTag.PAYLOAD_TYPE,
-                        OptionalTag.MS_MSG_WAIT_FACILITIES,
-                        OptionalTag.PRIVACY_INDICATOR,
-                        OptionalTag.USER_RESPONSE_CODE,
-                        OptionalTag.LANGUAGE_INDICATOR,
-                        OptionalTag.SAR_TOTAL_SEGMENTS,
-                        OptionalTag.SAR_SEGMENT_SEQNUM,
-                        OptionalTag.SC_INTERFACE_VERSION,
-                        OptionalTag.CALLBACK_NUM_PRES_IND,
-                        OptionalTag.NUMBER_OF_MESSAGES,
-                        OptionalTag.DPF_RESULT,
-                        OptionalTag.SET_DPF,
-                        OptionalTag.MS_AVAILABILITY_STATUS,
-                        OptionalTag.DELIVERY_FAILURE_REASON,
-                        OptionalTag.MORE_MESSAGES_TO_SEND,
-                        OptionalTag.MESSAGE_STATE,
-                        OptionalTag.DISPLAY_TIME,
-                        OptionalTag.MS_VALIDITY,
-                        OptionalTag.ITS_REPLY_TYPE):
+        if self.tag in (OptionalTag.DEST_ADDR_SUBUNIT, OptionalTag.DEST_NETWORK_TYPE, OptionalTag.DEST_BEARER_TYPE,
+                        OptionalTag.SOURCE_ADDR_SUBUNIT, OptionalTag.SOURCE_NETWORK_TYPE,
+                        OptionalTag.SOURCE_BEARER_TYPE, OptionalTag.SOURCE_TELEMATICS_ID, OptionalTag.PAYLOAD_TYPE,
+                        OptionalTag.MS_MSG_WAIT_FACILITIES, OptionalTag.PRIVACY_INDICATOR,
+                        OptionalTag.USER_RESPONSE_CODE, OptionalTag.LANGUAGE_INDICATOR, OptionalTag.SAR_TOTAL_SEGMENTS,
+                        OptionalTag.SAR_SEGMENT_SEQNUM, OptionalTag.SC_INTERFACE_VERSION,
+                        OptionalTag.CALLBACK_NUM_PRES_IND, OptionalTag.NUMBER_OF_MESSAGES, OptionalTag.DPF_RESULT,
+                        OptionalTag.SET_DPF, OptionalTag.MS_AVAILABILITY_STATUS, OptionalTag.DELIVERY_FAILURE_REASON,
+                        OptionalTag.MORE_MESSAGES_TO_SEND, OptionalTag.MESSAGE_STATE, OptionalTag.DISPLAY_TIME,
+                        OptionalTag.MS_VALIDITY, OptionalTag.ITS_REPLY_TYPE):
             # This is for unsigned ints size 1
             # SMPP doc says: 'Length of value part in octets'.
             return 1
-        if self.tag in (OptionalTag.DEST_TELEMATICS_ID,
-                        OptionalTag.USER_MESSAGE_REFERENCE,
-                        OptionalTag.SOURCE_PORT,
-                        OptionalTag.DESTINATION_PORT,
-                        OptionalTag.SAR_MSG_REF_NUM,
-                        OptionalTag.SMS_SIGNAL):
+        if self.tag in (OptionalTag.DEST_TELEMATICS_ID, OptionalTag.USER_MESSAGE_REFERENCE, OptionalTag.SOURCE_PORT,
+                        OptionalTag.DESTINATION_PORT, OptionalTag.SAR_MSG_REF_NUM, OptionalTag.SMS_SIGNAL):
             return 2
         if self.tag == OptionalTag.QOS_TIME_TO_LIVE:
             # This is for unsigned ints size 4
             return 4
-        if self.tag in (OptionalTag.ADDITIONAL_STATUS_INFO_TEXT,
-                        OptionalTag.RECEIPTED_MESSAGE_ID):
-            assert isinstance(self.value, str) # For linters
-            return len(self.value) + 1 # C Octet String (+1 for null termination)
-        if self.tag in (OptionalTag.SOURCE_SUBADDRESS,
-                        OptionalTag.DEST_SUBADDRESS,
-                        OptionalTag.CALLBACK_NUM_ATAG,
-                        OptionalTag.CALLBACK_NUM,
-                        OptionalTag.NETWORK_ERROR_CODE,
-                        OptionalTag.USSD_SERVICE_OP,
+        if self.tag in (OptionalTag.ADDITIONAL_STATUS_INFO_TEXT, OptionalTag.RECEIPTED_MESSAGE_ID):
+            assert isinstance(self.value, str)  # For linters
+            return len(self.value) + 1  # C Octet String (+1 for null termination)
+        if self.tag in (OptionalTag.SOURCE_SUBADDRESS, OptionalTag.DEST_SUBADDRESS, OptionalTag.CALLBACK_NUM_ATAG,
+                        OptionalTag.CALLBACK_NUM, OptionalTag.NETWORK_ERROR_CODE, OptionalTag.USSD_SERVICE_OP,
                         OptionalTag.ITS_SESSION_INFO):
-            assert isinstance(self.value, str) # For linters
-            return len(self.value) # Octet String (no null termination)
+            assert isinstance(self.value, str)  # For linters
+            return len(self.value)  # Octet String (no null termination)
         # Only remaining option is alert_on_message_delivery; see section 5.3.2.41 of SMPP document
         return 0
 
     @property
     def tlv(self) -> bytes:
         '''
         Returns the bytes representation of an optional SMPP parameter.
         '''
 
         length: int = self.length
         if self.tag.data_type == int:
             int_format: Dict[int, str] = {
-                1: '!HHB', # unsigned char
-                2: '!HHH', # unsigned short
-                4: '!HHI', # unsigned int
+                1: '!HHB',  # unsigned char
+                2: '!HHH',  # unsigned short
+                4: '!HHI',  # unsigned int
             }
             return pack(int_format[length], self.tag.value, length, self.value)
         if self.tag.data_type == str:
-            assert isinstance(self.value, str) # For linters
-            val: bytes = self.value.encode('ascii') # Octet String
-            if self.tag in (OptionalTag.ADDITIONAL_STATUS_INFO_TEXT,
-                            OptionalTag.RECEIPTED_MESSAGE_ID):
-                val += chr(0).encode('ascii') # C Octet String, terminate with NULL
+            assert isinstance(self.value, str)  # For linters
+            val: bytes = self.value.encode('ascii')  # Octet String
+            if self.tag in (OptionalTag.ADDITIONAL_STATUS_INFO_TEXT, OptionalTag.RECEIPTED_MESSAGE_ID):
+                val += chr(0).encode('ascii')  # C Octet String, terminate with NULL
             return pack('!HH', self.tag, length) + val
         # Only remaining option is alert_on_message_delivery; see section 5.3.2.41 of SMPP document
         if self.value:
             # TLV has no value field
             return pack('!HH', self.tag, self.length)
         return b''
 
@@ -659,18 +632,19 @@
 
 
 @dataclass
 class PduHeader():
     '''
     PDU header representation
     '''
-    pdu_length: int # Total PDU length
-    smpp_command: SmppCommand # SMPP command
-    command_status: SmppCommandStatus # SMPP response status (only relevant for responses)
-    sequence_num: int # SMPP sequence number
+    pdu_length: int  # Total PDU length
+    smpp_command: SmppCommand  # SMPP command
+    command_status: SmppCommandStatus  # SMPP response status (only relevant for responses)
+    sequence_num: int  # SMPP sequence number
 
 
 class SmppError(Exception):
+
     def __init__(self, smpp_command: SmppCommand, command_status: SmppCommandStatus) -> None:
         super().__init__()
         self.smpp_command: SmppCommand = smpp_command
         self.command_status: SmppCommandStatus = command_status
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/throttle.py` & `aiosmpplib-0.6.4/aiosmpplib/throttle.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,19 @@
       percent AND total number of responses from SMSC is greater than \
       :attr:`sample_size <SimpleThrottleHandler.sample_size>` over \
       :attr:`sampling_period <SimpleThrottleHandler.sampling_period>` seconds
     - then deny making anymore requests to SMSC
 
     '''
 
-    def __init__(self, logger: StructuredLogger, sampling_period: float = 180.00,
-                 sample_size: float = 50.00, deny_request_at: float = 1.00,
+    def __init__(self,
+                 logger: StructuredLogger,
+                 sampling_period: float = 180.00,
+                 sample_size: float = 50.00,
+                 deny_request_at: float = 1.00,
                  throttle_wait: float = 3.00) -> None:
         '''
         Parameters:
             logger: A StructuredLogger instance to be used for logging
             sampling_period: The duration in seconds over which we will calculate
                              the percentage of throttled responses.
             sample_size: The minimum number of responses we should have got from SMSC over
@@ -126,15 +129,17 @@
             # seconds, so reset values after self.sampling_period seconds.
             self.non_throttle_responses = 0
             self.throttle_responses = 0
             self.updated_at = now
         allowed: bool = current_percent_throttles <= self.deny_request_at
         log_level: int = DEBUG if allowed else WARNING
         if self.logger.isEnabledFor(log_level):
-            self.logger.log(log_level, 'Throttle handler result:',
+            self.logger.log(
+                log_level,
+                'Throttle handler result:',
                 result='allowed' if allowed else 'denied',
                 percent_throttles=current_percent_throttles,
                 throttle_responses=_throttle_responses,
                 non_throttle_responses=_non_throttle_responses,
                 sampling_period=self.sampling_period,
                 sample_size=self.sample_size,
                 deny_request_at=self.deny_request_at,
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib/utils.py` & `aiosmpplib-0.6.4/aiosmpplib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from datetime import datetime, timedelta, tzinfo
 from typing import Any, Optional, Tuple, Type, Union
 
 
-def check_param(param: Any, param_name: str, param_type: Union[Type, Tuple[Type]],
-                optional: bool=False, maxlen: int = 0) -> None:
+def check_param(param: Any,
+                param_name: str,
+                param_type: Union[Type, Tuple[Type]],
+                optional: bool = False,
+                maxlen: int = 0) -> None:
     if param is None:
         if not optional:
             raise ValueError(f'Non-optional parameter `{param_name}` was set to None.')
         return
     if not isinstance(param, param_type):
         if isinstance(param_type, Type):
             type_names: str = f'`{param_type.__name__}`'
@@ -39,15 +42,15 @@
         return self.offset
 
     def dst(self, dt: Optional[datetime]) -> timedelta:
         # pylint: disable=unused-argument
         return timedelta(0)
 
     @classmethod
-    def from_timezone(cls, offset_str: str, name: str='') -> 'FixedOffset':
+    def from_timezone(cls, offset_str: str, name: str = '') -> 'FixedOffset':
         '''
         Parameters:
             offset_str: Timezone part of datetime in ISO8601 format, e.g. '+0100' or '-0300'
             name: Timezone name
         '''
         if not offset_str:
             return cls(timedelta(0), name)
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib.egg-info/PKG-INFO` & `aiosmpplib-0.6.4/aiosmpplib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosmpplib
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python asyncio SMPP client library.
 Home-page: https://github.com/niksabaldun/aiosmpplib
 Author: Nikša Baldun
 Author-email: niksa.baldun@gmail.com
 License: MIT
 Keywords: aiosmpplib,smpp,smpp-client,smpp-protocol,smpp-library,esme,smsc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aiosmpplib-0.6.3/aiosmpplib.egg-info/SOURCES.txt` & `aiosmpplib-0.6.4/aiosmpplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiosmpplib-0.6.3/setup.py` & `aiosmpplib-0.6.4/setup.py`

 * *Files identical despite different names*

