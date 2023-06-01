# Comparing `tmp/mfrc522_i2c-0.0.4.tar.gz` & `tmp/mfrc522_i2c-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522_i2c-0.0.4.tar", last modified: Wed Sep 21 11:46:13 2022, max compression
+gzip compressed data, was "/home/cpranzl/Projects/mfrc522_i2c/dist/.tmp-15mt0yof/mfrc522_i2c-0.0.5.tar", last modified: Thu Jun  1 08:31:03 2023, max compression
```

## Comparing `mfrc522_i2c-0.0.4.tar` & `mfrc522_i2c-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cpranzl   (1000) cpranzl   (1000)        0 2022-09-21 11:46:12.997846 mfrc522_i2c-0.0.4/
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)    35149 2022-09-20 07:46:28.000000 mfrc522_i2c-0.0.4/LICENSE
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)     1021 2022-09-21 11:46:12.997846 mfrc522_i2c-0.0.4/PKG-INFO
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)      343 2022-09-20 07:46:28.000000 mfrc522_i2c-0.0.4/README.md
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)      104 2022-09-20 07:46:28.000000 mfrc522_i2c-0.0.4/pyproject.toml
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)      739 2022-09-21 11:46:12.997846 mfrc522_i2c-0.0.4/setup.cfg
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)     1128 2022-09-21 08:46:37.000000 mfrc522_i2c-0.0.4/setup.py
-drwxr-xr-x   0 cpranzl   (1000) cpranzl   (1000)        0 2022-09-21 11:46:12.993846 mfrc522_i2c-0.0.4/src/
-drwxr-xr-x   0 cpranzl   (1000) cpranzl   (1000)        0 2022-09-21 11:46:12.993846 mfrc522_i2c-0.0.4/src/mfrc522_i2c/
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)       79 2022-09-20 07:46:28.000000 mfrc522_i2c-0.0.4/src/mfrc522_i2c/__init__.py
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)    22366 2022-09-21 08:46:09.000000 mfrc522_i2c-0.0.4/src/mfrc522_i2c/mfrc522_i2c.py
-drwxr-xr-x   0 cpranzl   (1000) cpranzl   (1000)        0 2022-09-21 11:46:12.997846 mfrc522_i2c-0.0.4/src/mfrc522_i2c.egg-info/
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)     1021 2022-09-21 11:46:12.000000 mfrc522_i2c-0.0.4/src/mfrc522_i2c.egg-info/PKG-INFO
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)      304 2022-09-21 11:46:12.000000 mfrc522_i2c-0.0.4/src/mfrc522_i2c.egg-info/SOURCES.txt
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)        1 2022-09-21 11:46:12.000000 mfrc522_i2c-0.0.4/src/mfrc522_i2c.egg-info/dependency_links.txt
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)       17 2022-09-21 11:46:12.000000 mfrc522_i2c-0.0.4/src/mfrc522_i2c.egg-info/requires.txt
--rw-r--r--   0 cpranzl   (1000) cpranzl   (1000)       12 2022-09-21 11:46:12.000000 mfrc522_i2c-0.0.4/src/mfrc522_i2c.egg-info/top_level.txt
+drwxr-xr-x   0 cpranzl   (1001) cpranzl   (1001)        0 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)    35149 2021-07-19 13:23:51.000000 mfrc522_i2c-0.0.5/LICENSE
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)     1021 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/PKG-INFO
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)      343 2021-07-19 13:23:51.000000 mfrc522_i2c-0.0.5/README.md
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)      104 2021-07-19 13:23:51.000000 mfrc522_i2c-0.0.5/pyproject.toml
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)      739 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/setup.cfg
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)     1128 2023-05-25 16:53:13.000000 mfrc522_i2c-0.0.5/setup.py
+drwxr-xr-x   0 cpranzl   (1001) cpranzl   (1001)        0 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/
+drwxr-xr-x   0 cpranzl   (1001) cpranzl   (1001)        0 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c/
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)       79 2022-09-21 09:48:01.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c/__init__.py
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)    22547 2023-05-31 12:35:11.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c/mfrc522_i2c.py
+drwxr-xr-x   0 cpranzl   (1001) cpranzl   (1001)        0 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c.egg-info/
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)     1021 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c.egg-info/PKG-INFO
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)      304 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c.egg-info/SOURCES.txt
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)        1 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c.egg-info/dependency_links.txt
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)       17 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c.egg-info/requires.txt
+-rw-r--r--   0 cpranzl   (1001) cpranzl   (1001)       12 2023-06-01 08:31:03.000000 mfrc522_i2c-0.0.5/src/mfrc522_i2c.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mfrc522_i2c-0.0.4/LICENSE` & `mfrc522_i2c-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522_i2c-0.0.4/PKG-INFO` & `mfrc522_i2c-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522_i2c
-Version: 0.0.4
+Version: 0.0.5
 Summary: MFRC522 RFID reader/writer I2C driver in Python 3
 Home-page: https://github.com/cpranzl/mfrc522_i2c
 Author: Christoph Pranzl
 Author-email: christoph.pranzl@pranzl.net
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/cpranzl/mfrc522_i2c/issues
 Keywords: i2c rfid mfrc522
```

### Comparing `mfrc522_i2c-0.0.4/setup.cfg` & `mfrc522_i2c-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `mfrc522_i2c-0.0.4/setup.py` & `mfrc522_i2c-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="mfrc522_i2c",
-    version="0.0.4",
+    version="0.0.5",
     author="Christoph Pranzl",
     author_email="christoph.pranzl@pranzl.net",
     description=("MFRC522 RFID reader/writer I2C driver in Python 3"),
     license="GPLv3",
     keywords="i2c rfid mfrc522",
     url="https://github.com/cpranzl/mfrc522_i2c",
     packages=['mfrc522_i2c'],
```

### Comparing `mfrc522_i2c-0.0.4/src/mfrc522_i2c/mfrc522_i2c.py` & `mfrc522_i2c-0.0.5/src/mfrc522_i2c/mfrc522_i2c.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf8 -*-
 """
 MFRC522 RFID reader/writer I2C driver in Python 3
 """
 
 __author__ = "Christoph Pranzl"
-__version__ = "0.0.4444"
+__version__ = "0.0.5"
 __license__ = "GPLv3"
 
 from smbus import SMBus
 
 
 class MFRC522:
     # Define register values from datasheet
@@ -64,39 +64,39 @@
 
     # Mifare 1K EEPROM is arranged of 16 sectors. Each sector has 4 blocks and
     # each block has 16-byte. Block 0 is a special read-only data block that
     # keeps the manufacturer data and the UID of the tag. The sector trailer
     # block, the last block of the sector, holds the access conditions and two
     # of the authentication keys for that particular sector
     MIFARE_1K_MANUFAKTURERBLOCK = [0]
-    MIFARE_1K_SECTORTRAILER = [  3,   7,  11,  15,  19,  23,  27,  31,  35,
-                                39,  43,  47,  51,  55,  59,  63]
-    MIFARE_1K_DATABLOCK = [  1,   2,   4,   5,   6,   8,   9,  10,  12,  13,
-                            14,  16,  17,  18,  20,  21,  22,  24,  25,  26,
-                            28,  29,  30,  32,  33,  34,  36,  37,  38,  40,
-                            41,  42,  44,  45,  46,  48,  49,  50,  52,  53,
-                            54,  56,  57,  58,  60,  61,  62]
-
+    MIFARE_1K_SECTORTRAILER = [3, 7, 11, 15, 19, 23, 27, 31, 35,
+                               39, 43, 47, 51, 55, 59, 63]
+    MIFARE_1K_DATABLOCK = [1, 2, 4, 5, 6, 8, 9, 10, 12, 13,
+                           14, 16, 17, 18, 20, 21, 22,  24,  25,  26,
+                           28, 29, 30, 32, 33, 34, 36,  37,  38,  40,
+                           41, 42, 44, 45, 46, 48, 49,  50,  52,  53,
+                           54, 56, 57, 58, 60, 61, 62]
 
     # Mifare 4K EEPROM is arranged of 40 sectors. From sector 0 to 31, memory
     # organization is similar to Mifare 1K, each sector has 4 blocks. From
     # sector 32 to 39, each sector has 16 blocks
     MIFARE_4K_MANUFAKTURERBLOCK = [0]
-    MIFARE_4K_SECTORTRAILER = [  3,   7,  11,  15,  19,  23,  27,  31,  35,  39,
-                                43,  47,  51,  55,  59,  63,  67,  71,  75,  79,
-                                83,  87,  91,  95,  99, 103, 107, 111, 115, 119,
-                               123, 127, 143, 159, 175, 191, 207, 223, 239, 255]
-    MIFARE_4K_DATABLOCK = [  1,   2,   4,   5,   6,   8,   9,  10,  12,  13,
-                            14,  16,  17,  18,  20,  21,  22,  24,  25,  26,
-                            28,  29,  30,  32,  33,  34,  36,  37,  38,  40,
-                            41,  42,  44,  45,  46,  48,  49,  50,  52,  53,
-                            54,  56,  57,  58,  60,  61,  62,  64,  65,  66,
-                            68,  69,  70,  72,  73,  74,  76,  77,  78,  80,
-                            81,  82,  84,  85,  86,  88,  89,  90,  92,  93,
-                            94,  96,  97,  98, 100, 101, 102, 104, 105, 106,
+    MIFARE_4K_SECTORTRAILER = [3, 7, 11, 15, 19, 23, 27, 31, 35, 39,
+                               43, 47, 51, 55, 59, 63, 67, 71, 75, 79,
+                               83, 87, 91, 95, 99, 103, 107, 111, 115, 119,
+                               123, 127, 143, 159, 175, 191, 207, 223, 239,
+                               255]
+    MIFARE_4K_DATABLOCK = [1,  2, 4, 5, 6, 8, 9, 10, 12, 13,
+                           14, 16, 17, 18, 20, 21, 22, 24, 25, 26,
+                           28, 29, 30, 32, 33, 34, 36, 37, 38, 40,
+                           41, 42, 44, 45, 46, 48, 49, 50, 52, 53,
+                           54, 56, 57, 58, 60, 61, 62, 64, 65, 66,
+                           68, 69, 70, 72, 73, 74, 76, 77, 78, 80,
+                           81, 82, 84, 85, 86, 88, 89, 90, 92, 93,
+                           94, 96, 97, 98, 100, 101, 102, 104, 105, 106,
                            108, 109, 110, 112, 113, 114, 116, 117, 118, 120,
                            121, 122, 124, 125, 126, 128, 129, 130, 131, 132,
                            133, 134, 135, 136, 137, 138, 139, 140, 141, 142,
                            144, 145, 146, 147, 148, 149, 150, 151, 152, 153,
                            154, 155, 156, 157, 158, 160, 161, 162, 163, 164,
                            165, 166, 167, 168, 169, 170, 171, 172, 173, 174,
                            176, 177, 178, 179, 180, 181, 182, 183, 184, 185,
@@ -197,38 +197,36 @@
         TxIEn = 0x40  # Allow the transmitter to interrupt requests
         RxIEn = 0x20  # Allow the receiver to interrupt requests
         IdleIEn = 0x10  # Allow the idle interrupt request
         LoAlertIEn = 0x04  # Allow the low Alert interrupt request
         ErrIEn = 0x02  # Allow the error interrupt request
         TimerIEn = 0x01  # Allow the timer interrupt request
         self.__MFRC522_write(self.COMIENREG, (IRqInv |
-                                            TxIEn |
-                                            RxIEn |
-                                            IdleIEn |
-                                            LoAlertIEn |
-                                            ErrIEn |
-                                            TimerIEn))
+                                              TxIEn |
+                                              RxIEn |
+                                              IdleIEn |
+                                              LoAlertIEn |
+                                              ErrIEn |
+                                              TimerIEn))
 
         # Indicates that the bits in the ComIrqReg register are set
         Set1 = 0x80
         self.__MFRC522_clearBitMask(self.COMIRQREG, Set1)
 
         # Immediatly clears the internal FIFO buffer's read and write pointer
         # and ErrorReg register's BufferOvfl bit
         FlushBuffer = 0x80
         self.__MFRC522_setBitMask(self.FIFOLEVELREG, FlushBuffer)
 
         # Cancel running commands
         self.__MFRC522_write(self.COMMANDREG, self.MFRC522_IDLE)
 
         # Write data in FIFO register
-        i = 0
-        while (i < len(data)):
+        for i in range(0, len(data)):
             self.__MFRC522_write(self.FIFODATAREG, data[i])
-            i = i + 1
 
         # Countinously repeat the transmission of data from the FIFO buffer and
         # the reception of data from the RF field.
         self.__MFRC522_write(self.COMMANDREG, self.MFRC522_TRANSCEIVE)
 
         # Starts the transmission of data, only valid in combination with the
         # Transceive command
@@ -254,15 +252,15 @@
                 break
             if (comIRqReg & IdleIRq):
                 # Command terminate
                 break
             if (i == 0):
                 # Watchdog expired
                 break
-            i = i - 1
+            i -= 1
 
         # Clear the StartSend bit in BitFramingReg register
         self.__MFRC522_clearBitMask(self.BITFRAMINGREG, StartSend)
 
         # Retrieve data from FIFODATAREG
         if (i != 0):
             # The host or a MFRC522's internal state machine tries to write
@@ -303,18 +301,17 @@
                 lastBits = self.__MFRC522_read(self.CONTROLREG) & RxLastBits
 
                 if (lastBits != 0):
                     backBits = (fifoLevelReg - 1) * 8 + lastBits
                 else:
                     backBits = fifoLevelReg * 8
 
-                i = 0
-                while (i < fifoLevelReg):
+                # Read data from FIFO register
+                for i in range(0, fifoLevelReg):
                     backData.append(self.__MFRC522_read(self.FIFODATAREG))
-                    i = i + 1
 
             else:
                 status.MIFARE_ERR
 
         return (status, backData, backBits)
 
     def __calculateCRC(self, data):
@@ -456,14 +453,15 @@
                 break
             if (comIRqReg & IdleIRq):
                 # Command terminate
                 break
             if (i == 0):
                 # Watchdog expired
                 break
+            i -= 1
 
         # Clear the StartSend bit in BitFramingReg register
         StartSend = 0x80
         self.__MFRC522_clearBitMask(self.BITFRAMINGREG, StartSend)
 
         # Retrieve data from FIFODATAREG
         if (i != 0):
@@ -574,22 +572,30 @@
         TReloadVal_Lo = 0x00
         self.__MFRC522_write(self.TRELOADREGH, TReloadVal_Hi)
         self.__MFRC522_write(self.TRELOADREGL, TReloadVal_Lo)
 
         Force100ASK = 0x40  # Forces a 100% ASK modulation
         self.__MFRC522_write(self.TXASKREG, Force100ASK)
 
+        # Moderegister reset value
+        ResetVal = 0x3F
+        # Moderegister feature mask
+        FeatureMask = 0x14
         # Transmitter can only be started if RF field is generated
-        TxWaitRF = 0x32
+        TxWaitRF = 0x20
         # Defines polarity of pin MFIN, polarity of pin is active HIGH
         PolMFin = 0x08
         # Defines the preset value for the CRC coprocessor for the CalcCRC
         # command
-        CRCPreset0 = 0x01
-        self.__MFRC522_write(self.MODEREG, ( TxWaitRF | PolMFin | CRCPreset0))
+        CRCPreset = 0x01
+        self.__MFRC522_write(self.MODEREG, ((ResetVal &
+                                             FeatureMask) |
+                                            TxWaitRF |
+                                            PolMFin |
+                                            CRCPreset))
 
         # Activate antenna
         self.__MFRC522_antennaOn()
 
     def __MFRC522_read(self, address):
         """ Read data from an address on the i2c bus """
         value = self.i2cBus.read_byte_data(self.i2cAddress, address)
```

### Comparing `mfrc522_i2c-0.0.4/src/mfrc522_i2c.egg-info/PKG-INFO` & `mfrc522_i2c-0.0.5/src/mfrc522_i2c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-i2c
-Version: 0.0.4
+Version: 0.0.5
 Summary: MFRC522 RFID reader/writer I2C driver in Python 3
 Home-page: https://github.com/cpranzl/mfrc522_i2c
 Author: Christoph Pranzl
 Author-email: christoph.pranzl@pranzl.net
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/cpranzl/mfrc522_i2c/issues
 Keywords: i2c rfid mfrc522
```

