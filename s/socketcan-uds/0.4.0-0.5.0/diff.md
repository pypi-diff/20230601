# Comparing `tmp/socketcan-uds-0.4.0.tar.gz` & `tmp/socketcan-uds-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketcan-uds-0.4.0.tar", last modified: Thu Nov 10 17:49:58 2022, max compression
+gzip compressed data, was "socketcan-uds-0.5.0.tar", last modified: Thu Jun  1 19:29:35 2023, max compression
```

## Comparing `socketcan-uds-0.4.0.tar` & `socketcan-uds-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2022-11-10 17:49:58.246108 socketcan-uds-0.4.0/
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    35147 2018-06-01 10:17:25.000000 socketcan-uds-0.4.0/LICENSE
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     2263 2022-11-10 17:49:58.246108 socketcan-uds-0.4.0/PKG-INFO
--rw-r--r--   0 zeero     (1000) zeero     (1000)     1447 2022-08-13 05:11:20.000000 socketcan-uds-0.4.0/README.md
--rw-rw-r--   0 zeero     (1000) zeero     (1000)       38 2022-11-10 17:49:58.246108 socketcan-uds-0.4.0/setup.cfg
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     1072 2022-11-08 21:14:06.000000 socketcan-uds-0.4.0/setup.py
-drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2022-11-10 17:49:58.242108 socketcan-uds-0.4.0/socketcan_uds.egg-info/
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     2263 2022-11-10 17:49:58.000000 socketcan-uds-0.4.0/socketcan_uds.egg-info/PKG-INFO
--rw-rw-r--   0 zeero     (1000) zeero     (1000)      321 2022-11-10 17:49:58.000000 socketcan-uds-0.4.0/socketcan_uds.egg-info/SOURCES.txt
--rw-rw-r--   0 zeero     (1000) zeero     (1000)        1 2022-11-10 17:49:58.000000 socketcan-uds-0.4.0/socketcan_uds.egg-info/dependency_links.txt
--rw-rw-r--   0 zeero     (1000) zeero     (1000)        4 2022-11-10 17:49:58.000000 socketcan-uds-0.4.0/socketcan_uds.egg-info/top_level.txt
-drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2022-11-10 17:49:58.246108 socketcan-uds-0.4.0/uds/
--rw-rw-r--   0 zeero     (1000) zeero     (1000)      350 2022-03-12 12:21:06.000000 socketcan-uds-0.4.0/uds/__init__.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    23489 2022-11-08 21:14:06.000000 socketcan-uds-0.4.0/uds/client.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    72855 2022-11-08 21:14:06.000000 socketcan-uds-0.4.0/uds/common.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    18182 2022-11-08 21:14:06.000000 socketcan-uds-0.4.0/uds/odx_elements.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     6410 2022-11-08 21:14:06.000000 socketcan-uds-0.4.0/uds/odx_file_utils.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    15856 2022-11-08 21:14:06.000000 socketcan-uds-0.4.0/uds/program_file.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)    27382 2022-10-13 19:57:06.000000 socketcan-uds-0.4.0/uds/programmer.py
--rw-rw-r--   0 zeero     (1000) zeero     (1000)     1951 2022-01-29 08:17:19.000000 socketcan-uds-0.4.0/uds/security_access.py
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-06-01 19:29:35.794586 socketcan-uds-0.5.0/
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    35908 2023-05-30 19:16:22.000000 socketcan-uds-0.5.0/LICENSE
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     2301 2023-06-01 19:29:35.794586 socketcan-uds-0.5.0/PKG-INFO
+-rw-r--r--   0 zeero     (1000) zeero     (1000)     1447 2022-08-13 05:11:20.000000 socketcan-uds-0.5.0/README.md
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)      988 2023-06-01 19:26:16.000000 socketcan-uds-0.5.0/pyproject.toml
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)       38 2023-06-01 19:29:35.794586 socketcan-uds-0.5.0/setup.cfg
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-06-01 19:29:35.790585 socketcan-uds-0.5.0/socketcan_uds.egg-info/
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     2301 2023-06-01 19:29:35.000000 socketcan-uds-0.5.0/socketcan_uds.egg-info/PKG-INFO
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)      543 2023-06-01 19:29:35.000000 socketcan-uds-0.5.0/socketcan_uds.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)        1 2023-06-01 19:29:35.000000 socketcan-uds-0.5.0/socketcan_uds.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)       10 2023-06-01 19:29:35.000000 socketcan-uds-0.5.0/socketcan_uds.egg-info/requires.txt
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)        4 2023-06-01 19:29:35.000000 socketcan-uds-0.5.0/socketcan_uds.egg-info/top_level.txt
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-06-01 19:29:35.790585 socketcan-uds-0.5.0/tests/
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    15519 2022-08-13 08:41:30.000000 socketcan-uds-0.5.0/tests/test_client.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    23060 2022-08-12 15:36:03.000000 socketcan-uds-0.5.0/tests/test_common.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    11883 2023-06-01 16:51:10.000000 socketcan-uds-0.5.0/tests/test_odx_elements.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     2995 2023-05-30 20:17:12.000000 socketcan-uds-0.5.0/tests/test_odx_file_utils.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     2473 2023-06-01 15:35:15.000000 socketcan-uds-0.5.0/tests/test_program_file.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     8429 2023-06-01 19:02:42.000000 socketcan-uds-0.5.0/tests/test_programmer.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     3255 2022-01-29 08:13:40.000000 socketcan-uds-0.5.0/tests/test_security_access.py
+drwxrwxr-x   0 zeero     (1000) zeero     (1000)        0 2023-06-01 19:29:35.794586 socketcan-uds-0.5.0/uds/
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)      284 2023-05-31 19:43:18.000000 socketcan-uds-0.5.0/uds/__init__.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    23489 2022-11-10 18:01:51.000000 socketcan-uds-0.5.0/uds/client.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    72855 2023-05-30 19:16:22.000000 socketcan-uds-0.5.0/uds/common.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    21746 2023-06-01 16:51:10.000000 socketcan-uds-0.5.0/uds/odx_elements.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     7210 2023-06-01 16:51:10.000000 socketcan-uds-0.5.0/uds/odx_file_utils.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    18381 2023-06-01 16:51:10.000000 socketcan-uds-0.5.0/uds/program_file.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)    31021 2023-06-01 18:39:54.000000 socketcan-uds-0.5.0/uds/programmer.py
+-rw-rw-r--   0 zeero     (1000) zeero     (1000)     1951 2023-06-01 18:39:54.000000 socketcan-uds-0.5.0/uds/security_access.py
```

### Comparing `socketcan-uds-0.4.0/LICENSE` & `socketcan-uds-0.5.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+NON COMMERCIAL USE LICENSE based on GPL v3
+
+This software is distributed under GPLv3 with some extension because GPLv3
+did not manage to deny criminal misuse by organizations.
+This software is intended for usage by community and private individuals who
+are interested in car hacking. It is explicitly denied that any company or
+organization monetizes on this software. Monetize does not only mean money,
+it means gaining a competitive advantage of any kind by using this software.
+The author explicitly denies the usage for people associated with military,
+government agencies of any kind to whatever degree, same for car manufacturers
+and associates.
+
+GPL v3 Reference for completeness
+8<------------8<------------8<------------8<------------8<------------8<
+
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
```

### Comparing `socketcan-uds-0.4.0/PKG-INFO` & `socketcan-uds-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: socketcan-uds
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python 3 interface to Unified Diagnostic Services (UDS) Protocol
-Home-page: https://gitlab.com/menschel/socketcan-uds
-Author: Patrick Menschel
-Author-email: menschel.p@posteo.de
-Keywords: socketcan can uds
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
+Author-email: Patrick Menschel <menschel.p@posteo.de>
+Project-URL: Homepage, https://gitlab.com/menschel/socketcan-uds
+Project-URL: Bug Tracker, https://gitlab.com/menschel/socketcan-uds/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires: socketcan
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # socketcan-uds
 
 ![coverage](https://gitlab.com/Menschel/socketcan-uds/badges/master/coverage.svg)
```

### Comparing `socketcan-uds-0.4.0/README.md` & `socketcan-uds-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `socketcan-uds-0.4.0/socketcan_uds.egg-info/PKG-INFO` & `socketcan-uds-0.5.0/socketcan_uds.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: socketcan-uds
-Version: 0.4.0
+Version: 0.5.0
 Summary: A python 3 interface to Unified Diagnostic Services (UDS) Protocol
-Home-page: https://gitlab.com/menschel/socketcan-uds
-Author: Patrick Menschel
-Author-email: menschel.p@posteo.de
-Keywords: socketcan can uds
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
+Author-email: Patrick Menschel <menschel.p@posteo.de>
+Project-URL: Homepage, https://gitlab.com/menschel/socketcan-uds
+Project-URL: Bug Tracker, https://gitlab.com/menschel/socketcan-uds/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires: socketcan
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # socketcan-uds
 
 ![coverage](https://gitlab.com/Menschel/socketcan-uds/badges/master/coverage.svg)
```

### Comparing `socketcan-uds-0.4.0/uds/client.py` & `socketcan-uds-0.5.0/uds/client.py`

 * *Files identical despite different names*

### Comparing `socketcan-uds-0.4.0/uds/common.py` & `socketcan-uds-0.5.0/uds/common.py`

 * *Files identical despite different names*

### Comparing `socketcan-uds-0.4.0/uds/odx_elements.py` & `socketcan-uds-0.5.0/uds/odx_elements.py`

 * *Files 12% similar despite different names*

```diff
@@ -245,52 +245,93 @@
         if self.fw_checksum is not None:
             ET.SubElement(root_node, "FW-CHECKSUM", {"TYPE": "A_BYTEFIELD"}).text = self.fw_checksum.hex()
         if self.validity_for is not None:
             ET.SubElement(root_node, "VALIDITY-FOR", {"TYPE": "A_ASCIISTRING"}).text = self.validity_for
         return root_node
 
 
+class OwnIdentElement(OdxElement):
+    __TAG__ = "OWN-IDENT"
+    __NAME_PREFIX__ = "OI"
+
+    def __init__(self,
+                 long_name: str,
+                 value: str,
+                 id_: Optional[str] = None,
+                 short_name: Optional[str] = None,
+                 ):
+        super().__init__(id_=id_,
+                         short_name=short_name,
+                         long_name=long_name)
+        self.value = value
+
+    @classmethod
+    def from_element(cls, tree: ET.Element):
+        assert tree.tag == cls.__TAG__
+        id_ = tree.attrib.get("ID")
+        short_name = tree.find("./SHORT-NAME").text
+        long_name = tree.find("./LONG-NAME").text
+        value = tree.find("./IDENT-VALUE").text
+
+        return cls(id_=id_,
+                   short_name=short_name,
+                   long_name=long_name,
+                   value=value
+                   )
+
+    def to_element(self) -> ET.Element:
+        root_node = super(OwnIdentElement, self).to_element()
+        ET.SubElement(root_node, "IDENT-VALUE", {"TYPE": "A_ASCIISTRING"}).text = self.value
+        return root_node
+
+
 class DataBlockElement(OdxElement):
     __TAG__ = "DATABLOCK"
     __NAME_PREFIX__ = "DB"
 
     def __init__(self,
                  long_name: str,
                  flashdata_ref: str,
                  block_type: str,
                  segments: Optional[Sequence[SegmentElement]] = None,
+                 own_idents: Optional[Sequence[OwnIdentElement]] = None,
                  securitys: Optional[Sequence[SecurityElement]] = None,
                  id_: Optional[str] = None,
                  short_name: Optional[str] = None,
                  ):
         super().__init__(id_=id_,
                          short_name=short_name,
                          long_name=long_name)
         self.flashdata_ref = flashdata_ref
         self.segments = segments
+        self.own_idents = list()
+        if own_idents is not None:
+            self.own_idents = own_idents
         self.block_type = block_type
         self.securitys = list()
         if securitys is not None:
             self.securitys = securitys
 
     @classmethod
     def from_element(cls, tree: ET.Element):
         assert tree.tag == cls.__TAG__
         id_ = tree.attrib.get("ID")
         block_type = tree.attrib.get("TYPE")
         short_name = tree.find("./SHORT-NAME").text
         long_name = tree.find("./LONG-NAME").text
         flashdata_ref = tree.find("./FLASHDATA-REF").get("ID-REF")
         segments = [SegmentElement.from_element(elem) for elem in tree.findall("./SEGMENTS/SEGMENT")]
+        own_idents = [OwnIdentElement.from_element(elem) for elem in tree.findall("./OWN-IDENTS/OWN-IDENT")]
         securitys = [SecurityElement.from_element(elem) for elem in tree.findall("./SECURITYS/SECURITY")]
         return cls(id_=id_,
                    short_name=short_name,
                    long_name=long_name,
                    flashdata_ref=flashdata_ref,
                    segments=segments,
+                   own_idents=own_idents,
                    block_type=block_type,
                    securitys=securitys,
                    )
 
     def to_element(self) -> ET.Element:
         root_node = super(DataBlockElement, self).to_element()
         root_node.set("TYPE", self.block_type)
@@ -299,54 +340,107 @@
         for security in self.securitys:
             securitys_node.append(security.to_element())
         root_node.append(securitys_node)
         segments_node = ET.Element("SEGMENTS")
         for segment in self.segments:
             segments_node.append(segment.to_element())
         root_node.append(segments_node)
+        own_idents_node = ET.Element("OWN-IDENTS")
+        for own_ident in self.own_idents:
+            own_idents_node.append(own_ident.to_element())
+        root_node.append(own_idents_node)
+        return root_node
+
+
+class ExpectedIdentElement(OdxElement):
+    __TAG__ = "EXPECTED-IDENT"
+    __NAME_PREFIX__ = "EI"
+
+    def __init__(self,
+                 long_name: str,
+                 values: Sequence[str],
+                 id_: Optional[str] = None,
+                 short_name: Optional[str] = None,
+                 ):
+        super().__init__(id_=id_,
+                         short_name=short_name,
+                         long_name=long_name)
+        self.values = values
+
+    @classmethod
+    def from_element(cls, tree: ET.Element):
+        assert tree.tag == cls.__TAG__
+        id_ = tree.attrib.get("ID")
+        short_name = tree.find("./SHORT-NAME").text
+        long_name = tree.find("./LONG-NAME").text
+        values = [ident_values_node.text
+                  for ident_values_node in tree.findall("./IDENT-VALUES/IDENT-VALUE")]
+
+        return cls(id_=id_,
+                   short_name=short_name,
+                   long_name=long_name,
+                   values=values
+                   )
+
+    def to_element(self) -> ET.Element:
+        root_node = super(ExpectedIdentElement, self).to_element()
+        ident_values_node = ET.Element("IDENT-VALUES")
+        for value in self.values:
+            ET.SubElement(ident_values_node, "IDENT-VALUE", {"TYPE": "A_ASCIISTRING"}).text = value
+        root_node.append(ident_values_node)
         return root_node
 
 
 class SessionElement(OdxElement):
     __TAG__ = "SESSION"
     __NAME_PREFIX__ = "SES"
 
     def __init__(self,
                  long_name: str,
+                 expected_idents: Sequence[ExpectedIdentElement],
                  securitys: Sequence[SecurityElement],
                  datablockrefs: Sequence[str],
                  id_: Optional[str] = None,
                  short_name: Optional[str] = None,
                  ):
         super().__init__(id_=id_,
                          short_name=short_name,
                          long_name=long_name)
+        self.expected_idents = expected_idents
         self.securitys = securitys
         self.datablockrefs = datablockrefs
 
     @classmethod
     def from_element(cls, tree: ET.Element):
         assert tree.tag == cls.__TAG__
         id_ = tree.attrib.get("ID")
         short_name = tree.find("./SHORT-NAME").text
         long_name = tree.find("./LONG-NAME").text
         securitys = [SecurityElement.from_element(elem) for elem in tree.findall("./SECURITYS/SECURITY")]
+        expected_idents = [ExpectedIdentElement.from_element(elem) for elem in
+                           tree.findall("./EXPECTED-IDENTS/EXPECTED-IDENT")]
 
         datablockrefs = [datablockref_node.get("ID-REF")
                          for datablockref_node in tree.findall("./DATABLOCK-REFS/DATABLOCK-REF")]
 
         return cls(id_=id_,
                    short_name=short_name,
                    long_name=long_name,
+                   expected_idents=expected_idents,
                    securitys=securitys,
                    datablockrefs=datablockrefs
                    )
 
     def to_element(self) -> ET.Element:
         root_node = super(SessionElement, self).to_element()
+        expected_idents_node = ET.Element("EXPECTED-IDENTS")
+        for expected_ident in self.expected_idents:
+            expected_idents_node.append(expected_ident.to_element())
+        root_node.append(expected_idents_node)
+
         securitys_node = ET.Element("SECURITYS")
         for security in self.securitys:
             securitys_node.append(security.to_element())
         root_node.append(securitys_node)
 
         datablockrefs_node = ET.Element("DATABLOCK-REFS")
         for datablockref in self.datablockrefs:
```

### Comparing `socketcan-uds-0.4.0/uds/odx_file_utils.py` & `socketcan-uds-0.5.0/uds/odx_file_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -96,14 +96,24 @@
     tree = ET.ElementTree(element=root)
     tree.write(file_or_filename=odx_file,
                encoding="UTF-8",
                xml_declaration=True,
                )
 
 
+def find_security_methods(ecu_mem: EcuMemElement) -> dict:
+    return {sec.security_method: dict(fw_signature=sec.fw_signature, valid_for=sec.validity_for) for sec in
+            ecu_mem.mem.session.securitys}
+
+
+def find_block_security_methods(data_block: DataBlockElement) -> dict:
+    return {sec.security_method: dict(fw_signature=sec.fw_signature, valid_for=sec.validity_for) for sec in
+            data_block.securitys}
+
+
 def find_uds_address_length_format_identifier(ecu_mem: EcuMemElement) -> dict:
     uds_address_length_format_identifier = None
     for sec in ecu_mem.mem.session.securitys:
         if sec.security_method == "ALFID":
             alfid_bytes = sec.fw_signature
             uds_address_length_format_identifier = {
                 "routine_control": ((alfid_bytes[0] & 0xF), (alfid_bytes[0] >> 4)),
@@ -140,15 +150,15 @@
             break
     return sa2
 
 
 def find_checksum_for_block(datablock: DataBlockElement, session: SessionElement) -> Optional[bytes]:
     checksum = None
     if datablock.securitys:
-        checksum = datablock.securitys[0].fw_signature
+        checksum = datablock.securitys[0].fw_checksum
     elif (session_securitys := [sec for sec in session.securitys if
                                 (sec.validity_for is not None and datablock.id.endswith(
                                     sec.validity_for))]):
         checksum = session_securitys[0].fw_checksum
     return checksum
 
 
@@ -157,7 +167,18 @@
     if datablock.securitys:
         signature = datablock.securitys[0].fw_signature
     elif (session_securitys := [sec for sec in session.securitys if
                                 (sec.validity_for is not None and datablock.id.endswith(
                                     sec.validity_for))]):
         signature = session_securitys[0].fw_signature
     return signature
+
+
+def find_expected_idents(ecu_mem: EcuMemElement) -> dict:
+    session = ecu_mem.mem.session
+    expected_idents = {ei.short_name: ei.values for ei in session.expected_idents}
+    return expected_idents
+
+
+def find_own_idents_for_datablock(datablock: DataBlockElement) -> dict:
+    own_idents = {oi.short_name: oi.value for oi in datablock.own_idents}
+    return own_idents
```

### Comparing `socketcan-uds-0.4.0/uds/program_file.py` & `socketcan-uds-0.5.0/uds/program_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,28 @@
     :platform: Posix
     :synopsis: A class file for a program file / flash container
     moduleauthor:: Patrick Menschel (menschel.p@posteo.de)
     license:: GPL v3
 """
 import logging
 import pickle
+import zipfile
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from hashlib import sha256
 from pathlib import Path
-import zipfile
-from typing import Optional
+from typing import Optional, Dict
 
 from uds import EncryptionMethod, CompressionMethod
 from uds.odx_elements import EcuMemElement, SessionElement, FlashDataElement, SegmentElement, DataBlockElement, \
-    SecurityElement, MemElement, FlashElement
-from uds.odx_file_utils import parse_odx, find_uds_address_length_format_identifier, find_sa2, \
-    find_checksum_for_block, find_signature_for_block, parse_index_xml, write_odx, alfid_dict_to_alfid_bytes, \
-    create_index_xml
+    SecurityElement, MemElement, FlashElement, ExpectedIdentElement, OwnIdentElement
+from uds.odx_file_utils import parse_odx, find_uds_address_length_format_identifier, find_checksum_for_block, \
+    find_signature_for_block, parse_index_xml, write_odx, create_index_xml, find_expected_idents, \
+    find_own_idents_for_datablock, find_security_methods, \
+    find_block_security_methods
 
 
 class ProgrammingFileABC(ABC):
 
     def __init__(self, filepath: Optional[Path] = None):
         self._filepath = None
         self._dictionary = None
@@ -85,15 +86,16 @@
             odx = parse_odx(odx_file=fp)
 
         flash_elem: FlashElement = odx.get("flash")
         ecu_mem = flash_elem.ecu_mem
         self._dictionary = {}
 
         uds_address_length_format_identifier = find_uds_address_length_format_identifier(ecu_mem)
-        sa2 = find_sa2(ecu_mem)
+        security_methods = find_security_methods(ecu_mem)
+        expected_idents = find_expected_idents(ecu_mem)
 
         blocks = OrderedDict()
         for datablockref in ecu_mem.mem.session.datablockrefs:
             datablock = [x for x in ecu_mem.mem.datablocks if x.id == datablockref][0]
 
             assert len(datablock.segments), "Datablocks with more then one segment are not handled yet."
             segment = datablock.segments[0]
@@ -111,30 +113,33 @@
 
             erase_block = (datablock.block_type in ["FLASH_DATA", ])
 
             checksum = find_checksum_for_block(datablock=datablock,
                                                session=ecu_mem.mem.session)
             signature = find_signature_for_block(datablock=datablock,
                                                  session=ecu_mem.mem.session)
+            own_idents = find_own_idents_for_datablock(datablock=datablock)
 
             blocks.update({datablock.long_name: {"addr": addr,
                                                  "data": data,
                                                  "datafile": datafile,
+                                                 "own_idents": own_idents,
                                                  "erase_block": erase_block,
                                                  "compression_method": compression_method,
                                                  "encryption_method": encryption_method,
                                                  "transfer_request_parameters": transfer_request_parameters,
                                                  "uncompressed_size": uncompressed_size,
                                                  "compressed_size": compressed_size,
-                                                 "checksum": checksum,
-                                                 "signature": signature,
+                                                 "security_methods": find_block_security_methods(datablock),
+                                                 "checksum": checksum,  # obsolete
+                                                 "signature": signature,  # obsolete
                                                  }})
-
         self._dictionary.update({"uds_address_and_length_format_identifier": uds_address_length_format_identifier,
-                                 "sa2": sa2,
+                                 "security_methods": security_methods,
+                                 "expected_idents": expected_idents,
                                  "blocks": blocks})
         # emem name can be extracted from datablock_id left most string of "."
         self._container_name = flash_elem.long_name
         self._filepath = filepath
 
     def _write_file(self, filepath: Path, format_flash_pdx: bool = False):
         """
@@ -161,29 +166,33 @@
         flash.ecu_mem = ecu_mem
 
         mem = MemElement(datablocks=datablocks,
                          flashdatas=flashdatas,
                          )
         ecu_mem.mem = mem
 
+        expected_idents = [ExpectedIdentElement(long_name=long_name, values=values) for
+                           long_name, values in self.get_expected_idents().items()]
+        # print(expected_idents)
         session = SessionElement(securitys=session_securitys,
                                  long_name=ecu_mem.long_name,
                                  datablockrefs=datablockrefs,
+                                 expected_idents=expected_idents,
                                  )
         session.id = ".".join([ecu_mem.short_name, session.short_name])
         mem.session = session
 
-        session_securitys.extend([SecurityElement(security_method="SA2", fw_signature=self._dictionary.get("sa2")),
-                                  SecurityElement(security_method="ALFID",
-                                                  fw_signature=alfid_dict_to_alfid_bytes(
-                                                      self.get_address_and_length_format_identifier())),
-                                  ])
+        session_securitys.extend([SecurityElement(security_method=security_method_name,
+                                                  fw_signature=security_method_data.get("fw_signature"),
+                                                  validity_for=security_method_data.get("valid_for"))
+                                  for security_method_name, security_method_data in self.security_methods.items()])
+
         for index, (datablock_name, block_data) in enumerate(self.get_blocks().items()):
             if not datablock_name.split()[0].isnumeric():
-                datablock_long_name = "{0:02X} {1}".format(index+1, datablock_name)
+                datablock_long_name = "{0:02X} {1}".format(index + 1, datablock_name)
             else:
                 datablock_long_name = datablock_name
 
             self._logger.info("Using {0}".format(datablock_long_name))
 
             encrypt_compress_method = bytes(
                 ((block_data.get("compression_method") << 4) | block_data.get("encryption_method"),))
@@ -193,35 +202,32 @@
                                           data=block_data.get("data"),
                                           encrypt_compress_method=encrypt_compress_method,
                                           dataformat="BINARY",
                                           )
             flash_data.id = ".".join([ecu_mem.short_name, flash_data.short_name])
             flashdatas.append(flash_data)
 
-            block_securitys = []
-            if format_flash_pdx:
-                security_method_name = "SECURITY_METHOD_NAME"
-                session_securitys.append(SecurityElement(security_method=security_method_name,
-                                                         fw_signature=block_data.get("signature"),
-                                                         fw_checksum=block_data.get("checksum"),
-                                                         validity_for=datablock_long_name,
-                                                         ))
-            else:
-                security_method_name = "SECURITY_METHOD_NAME"
-                block_securitys.append(SecurityElement(security_method=security_method_name,
-                                                       fw_signature=block_data.get("signature"),
-                                                       fw_checksum=block_data.get("checksum"),
-                                                       ))
+            block_securitys = [SecurityElement(security_method=security_method_name,
+                                               fw_signature=security_method_data.get("fw_signature"),
+                                               validity_for=security_method_data.get("valid_for"))
+                               for security_method_name, security_method_data in
+                               block_data.get("security_methods").items()]
 
+            own_idents = [OwnIdentElement(long_name=long_name, value=value) for
+                          long_name, value in block_data.get("own_idents").items()]
             datablock = DataBlockElement(long_name=datablock_long_name,
                                          securitys=block_securitys,
                                          block_type="FLASH-DATA",
                                          flashdata_ref=flash_data.id,
+                                         own_idents=own_idents,
                                          )
+
             datablock.id = ".".join([ecu_mem.short_name, datablock.short_name])
+            for own_ident in datablock.own_idents:
+                own_ident.id = ".".join([datablock.id, own_ident.short_name])
 
             segment_long_name = "{0:X}".format(block_data.get("addr"))
             segment = SegmentElement(
                 long_name=segment_long_name,
                 compressed_size=block_data.get("compressed_size"),
                 uncompressed_size=block_data.get("uncompressed_size"),
                 source_start_address=block_data.get("addr"),
@@ -232,20 +238,43 @@
             datablocks.append(datablock)
             datablockrefs.append(datablock.id)
 
         with filepath.open("wb") as fp:  # Note: The filename defaults to the id of the flash block
             write_odx(odx_file=fp,
                       flash=flash)
 
+    def get_expected_idents(self) -> Dict[str, str]:
+        """
+        Get the EXPECTED-IDENT fields
+        :return: A Dictionary of expected identifications
+        """
+        return self._dictionary.get("expected_idents")
+
+    def get_own_idents(self) -> Dict[str, dict]:
+        """
+        Get the OWN-IDENT fields
+        :return: A collection of Key,Value Tuples, tbd.
+        """
+        return {block_data.get("addr"): block_data.get("own_idents") for block_name, block_data in
+                self.get_blocks().items()}
+
+    @property
+    def security_methods(self) -> Optional[dict]:
+        """
+        Get the SECURITY-METHODS
+        :return: A collection of Security Methods
+        """
+        return self._dictionary.get("security_methods")
+
 
 class PackedUpdateContainer(UpdateContainerOdxFile):
     """
     A packed Update Container aka packed Odx or Pdx
 
-    In essence it is a Zip file, that contains an
+    In essence, it is a Zip file, that contains an
     index.xml file catalog,
     an Odx Update Container,
     a number of .bin files.
     """
 
     def _load_file(self, filepath: Path):
         """
@@ -330,29 +359,54 @@
                 )
             create_index_xml(zipfile.Path(zfp, index_file_name),
                              short_name=self._container_name,
                              data_files=data_files
                              )
 
 
-FILE_EXT_TO_PROGRAMMING_FILE_MAPPING = {".pkl": ExampleProgrammingFile,
-                                        ".odx": UpdateContainerOdxFile,
-                                        ".pdx": PackedUpdateContainer,
-                                        }
-
-
 def read_programming_file(filepath: Path) -> ProgrammingFileABC:
     """
     Read a programming file and return a suitable class object.
+    This function is mainly for testing purposes.
 
     :param filepath: The Path to the file.
     :type filepath: Path
     :return: A programming file object.
     :rtype: ProgrammingFileABC
     :raise ValueError: If not successful.
     """
+
+    FILE_EXT_TO_PROGRAMMING_FILE_MAPPING = {".pkl": ExampleProgrammingFile,
+                                            ".odx": UpdateContainerOdxFile,
+                                            ".pdx": PackedUpdateContainer,
+                                            }
+
+    if not filepath.exists():
+        raise ValueError("Filepath does not exist. {0}".format(filepath))
+    if filepath.suffix not in FILE_EXT_TO_PROGRAMMING_FILE_MAPPING:
+        raise ValueError("No suitable programming file class for extention {0}".format(filepath.suffix))
+    programming_file_class = FILE_EXT_TO_PROGRAMMING_FILE_MAPPING.get(filepath.suffix)
+    return programming_file_class(filepath=filepath)
+
+
+def read_odx_update_container(filepath: Path) -> UpdateContainerOdxFile:
+    """
+    Read an odx-based programming file and return a suitable class object.
+    This is the actual function to be used when loading a file into the programmer.
+
+    :param filepath: The Path to the file.
+    :type filepath: Path
+    :return: A programming file object.
+    :rtype: ProgrammingFileABC
+    :raise ValueError: If not successful.
+    """
+
+    FILE_EXT_TO_PROGRAMMING_FILE_MAPPING = {".odx": UpdateContainerOdxFile,
+                                            ".pdx": PackedUpdateContainer,
+                                            }
+
     if not filepath.exists():
         raise ValueError("Filepath does not exist. {0}".format(filepath))
     if filepath.suffix not in FILE_EXT_TO_PROGRAMMING_FILE_MAPPING:
         raise ValueError("No suitable programming file class for extention {0}".format(filepath.suffix))
     programming_file_class = FILE_EXT_TO_PROGRAMMING_FILE_MAPPING.get(filepath.suffix)
     return programming_file_class(filepath=filepath)
```

### Comparing `socketcan-uds-0.4.0/uds/programmer.py` & `socketcan-uds-0.5.0/uds/programmer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """ module:: uds.programmer
     :platform: Posix
-    :synopsis: A class file for a uds programmer
+    :synopsis: A class file for an uds programmer
     moduleauthor:: Patrick Menschel (menschel.p@posteo.de)
     license:: GPL v3
 """
+import logging
+import struct
 import threading
 import time
 from abc import ABC, abstractmethod
 from collections import OrderedDict
+from enum import IntEnum, auto
 from pathlib import Path
 from typing import Optional, Tuple, Callable, Union
-from enum import IntEnum, auto
-import struct
 
+from uds.client import UdsClient
 from uds.common import CompressionMethod, EncryptionMethod, RoutineControlType, DiagnosticSession, UdsTimeoutError, \
     UdsProtocolException, ConditionsNotCorrect, ExceededNumberOfAttempts, RequiredTimeDelayNotExpired
-
-from uds.client import UdsClient
-
-import logging
-
-from uds.program_file import read_programming_file
+from uds.program_file import read_programming_file, read_odx_update_container
 
 EXAMPLE_BLOCK_DICT = OrderedDict(
     {"example_block": {"addr": 0x1234,
                        "checksum": bytes(range(15)),
                        "signature": bytes(range(15)),
                        "data": bytes.fromhex("11 22 33 44 55 66 77 88"),
                        "uncompressed_size": 8,
@@ -71,17 +68,23 @@
 class StageException(ProgrammingException):
     """
     The Programming State Job did fail.
     """
     pass
 
 
+class WrongDeviceConntectedException(ProgrammingException):
+    """
+    The expected identifications did not match the device.
+    """
+
+
 class UdsProgrammerABC(ABC):
     """
-    Abstract Base Class for an UDS Programmer class
+    Abstract Base Class for a UDS Programmer
     """
 
     def __init__(self,
                  client: Optional[UdsClient] = None,
                  programming_filepath: Optional[Path] = None,
                  force_programming: bool = False,
                  ):
@@ -119,41 +122,41 @@
         self._current_block_progress = None
         self._worker = None
 
         if programming_filepath is not None:
             self.load_programming_file(filepath=programming_filepath)
 
     @property
-    def current_programming_block(self) -> Optional[Tuple[str, int, int]]:
+    def current_programming_block(self) -> Optional[dict]:
         """
         current_programming_block Getter
+
         :return: A tuple of (block_name, block_number, total_block_number) or None.
         """
         return self._current_programming_block
 
     @current_programming_block.setter
-    def current_programming_block(self, val: Tuple[str, int, int]) -> None:
+    def current_programming_block(self, block_dict: dict) -> None:
         """
         current_programming_block Setter
-        :param val: A tuple of (block_name, block_number, total_block_number)
+
+        :param block_dict: A tuple of (block_name, block_number, total_block_number)
         :return: Nothing.
         """
-        block_name, block_number, total_block_number = val
         for hook in self._hooks:
             hook({"type": "new_programming_block",
-                  "block_name": block_name,
-                  "block_number": block_number,
-                  "total_block_number": total_block_number
+                  "block_dict": block_dict,
                   })
-        self._current_programming_block = val
+        self._current_programming_block = block_dict
 
     @property
     def current_block_progress(self) -> Tuple[int, int]:
         """
         current_block_progress Getter
+
         :return: A tuple of (current_byte, total_bytes)
         """
         return self._current_block_progress
 
     @current_block_progress.setter
     def current_block_progress(self, val: Tuple[int, int]) -> None:
         current_byte, total_bytes = val
@@ -164,22 +167,24 @@
                   })
         self._current_block_progress = val
 
     @property
     def state(self) -> ProgrammerState:
         """
         State Getter
+
         :return: The Value.
         """
         return self._state
 
     @state.setter
     def state(self, val: ProgrammerState) -> None:
         """
         State Setter
+
         :param val: The Value.
         :return: Nothing.
         """
         assert isinstance(val, ProgrammerState)
         if val != self._state:
             for hook in self._hooks:
                 hook({"type": "state_transition",
@@ -190,88 +195,116 @@
         self._previous_state = self._state
         self._state = val
 
     @property
     def previous_state(self) -> ProgrammerState:
         """
         Previous State Getter
+
         :return: The Value.
         """
         return self._previous_state
 
     def register_hook(self,
                       hook_function: Callable,
                       ):
         if hook_function not in self._hooks:
             self._hooks.append(hook_function)
 
+    def get_uds_server_identification(self) -> Optional[dict]:
+        """
+        An abstract function to retrieve the identification from
+        the connected UDS server.
+        This is necessary for a download target check.
+
+        :return: A dictionary or None.
+        """
+        return None
+
+    def get_uds_server_block_versions(self) -> Optional[dict]:
+        """
+        An abstract function to retrieve the block versions from
+        the connected UDS server.
+        This is necessary for a download content check.
+
+        :return: A dictionary or None.
+        """
+        return None
+
     def start_programming(self) -> None:
         """
         This function starts the programming job, e.g. the worker that traverses the state machine.
+
         :return: Nothing
         """
         assert self._client is not None
         assert self._programming_file is not None
         assert self._worker is None or not self._worker.is_alive()
 
         self._state = ProgrammerState.Init
         self._worker = threading.Thread(target=self.handle_state_machine)
         self._worker.daemon = True
         self._worker.start()
 
     def is_finished(self) -> bool:
         """
         Function to check if the programmer has finished the programming job.
+
         :return: True if finished / False is not.
         """
         return self.state in [ProgrammerState.ProgrammingFinished, ProgrammerState.ProgrammingError, None]
 
     def handle_state_machine(self):
         """
         The actual worker daemon of this class.
         The state machine uses a Last-In-First-Out-Queue to store the states to be traversed.
         (Note: The names stage, step or state have more or less the same meaning in this context.)
-        Using this method, additional / intermediary steps can by dynamically added by the currently handled state, e.g.
+        Using this method, additional / intermediary steps can be dynamically added by the currently handled state, e.g.
         if the UnlockDeviceForProgramming step encounters an error pointing towards a non elapsed barricade timer, it
         can route back to the PreProgramming State by just putting that state and itself back to the queue.
         (Note: This method is Work-in-Progress and has to be perfected while testing.)
+
         :return: None
         """
 
         while not self.is_finished():
             job_for_this_state = self.state_to_function_dict.get(self.state)
             if job_for_this_state is not None and callable(job_for_this_state):
-                self.state = job_for_this_state()
+                try:
+                    self.state = job_for_this_state()
+                except UdsTimeoutError:
+                    self._logger.error("Lost connection - Restarting")
+                    self.state = ProgrammerState.NotConnected
             else:
-                self._logger.error("No job for this state")
+                self._logger.error("No job for this state {0}".format(self.state))
                 self.state = ProgrammerState.ProgrammingError
 
     def load_programming_file(self, filepath: Path) -> None:
         """
         1st phase of programming. Loading a programming file.
         Although uds has been standardized, the programming sequences have not and basically every EOM has
         their own flavor. Since ODX based formats have emerged, namely PDX, a programming ODX format,
         a programming file provides
 
         * binary data: the actual binaries to be programmed
         * means of communication with the target device: typically CAN IDs for an ISOTP channel
         * device compatibility checks based on what identification the device provides,
           e.g. a part number is provided by read data by id
         * device unlock and signature methods, e.g. used crypto functions and keys
-        * meta data for each binary data:
+        * metadata for each binary data:
 
           * where the binary goes, e.g. address or index of a binary block and
             subsequently if the location has to be erased in case of flash memory
           * precalculated hashes and signatures for binary blocks
           * binary data may be encrypted or compressed and the programming
              application must know this to populate the corresponding uds services
 
         This abstracted programmer must obtain all necessary information from the programming file.
-        A OrderedDict of blocks has to be provided, ordered because because it matters in which sequence
-        blocks are programmed. An item must provide meta data on the block, the definition is
+        A OrderedDict of blocks has to be provided, ordered because it matters in which sequence
+        blocks are programmed. An item must provide metadata on the block, the definition is
 
         .. code-block:: python
 
             {
                 "blocks":{
                     "example_block": {
                         "addr": 0x1234,
@@ -288,28 +321,29 @@
                 "uds_address_and_length_format_identifier": {"request_download": (2, 4),
                                                              "routine_control": (2, 4),
                                                              },
                 }
             }
 
         There can be general information on communication parameters as well.
-        For example, some devices can't handle address items or size items other then 4bytes. In that case the item
+        For example, some devices can't handle address items or size items other than 4bytes. In that case the item
         "uds_address_and_length_format_identifier": int, # parameter of request download
         has to be filled. To be continued...
         """
         self._programming_file = read_programming_file(filepath=filepath)
 
     ####################################
     # Tasks / Jobs for specific states #
     ####################################
 
     def try_to_connect(self) -> ProgrammerState:
         """
         A function to check if the programmer which
         by itself is a client, is connected to a server.
+
         :return: The next state, it can be this state again.
         """
         next_state = self.state
         try:
             self._client.tester_present()
             next_state = ProgrammerState.PreProgramming
         except UdsTimeoutError:
@@ -323,30 +357,36 @@
         2nd phase of programming
         Pre_programming:
         It consists of a couple of steps that occur linear.
 
         * Identification Check (Application / Optional)
           In case the programming file provides information or identification patterns on the target device,
           this should be checked against the connected device.
+        * Download Content Check (Application)
+          Typically, a programming file contains different blocks to be flashed and each block has some
+          sort of unique identification or version. It would be wasteful to program something that is
+          already programmed, so the task is to "filter" was needs to be programmed.
         * Preconditions Check (Application)
           An ECU must perform some task, so it must be asked if it is safe to purge regular operation,
           reboot and stay in bootloader without starting application.
         * Preparations Step (Application)
           Any necessary preparation, e.g. disable the settings of DTCs and stop all unnecessary communication.
           This is not actually plausible because when a programming session is started, the scope of operation
           of the ecu typically is very small, so it would not do anything other than handle diagnostic requests.
-          It may even happen that an ECU does tell it's communication partners that it is not available for a limited
+          It may even happen that an ECU does tell its communication partners that it is not available for a limited
           time, i.e. like you tell your neighbors that your on holiday for the weekend, so they don't miss you
           and hopefully water your plants.
         * Transition to Programming Session (Application -> Bootloader)
           The most obvious step last but not least, the start of the programming session, which typically involves
           a reboot to bootloader, and setting some flags before, so bootloader waits for programming instead
           of starting application.
           This phase should also contain a sanity check if the programming session has been reached.
 
+        IMPORTANT NOTICE: This function may stop to be abstract in the future because the Download Content Check part
+                          can be unified / modeled in an abstract way.
         :return: The next state, typically ProgrammerState.SwitchToProgrammingMode.
         """
 
     # 3rd phase of programming - the programming in programming session
     # this requires a state machine which is not yet written, however tasks during programming can be
     # abstracted into separate functions.
 
@@ -392,22 +432,26 @@
 
         :return: The next state, typically ProgrammerState.UnlockDeviceForProgramming.
         """
 
     def block_programming(self) -> ProgrammerState:
         """
         A universal function for the state block programming.
+
         :return: The next state, typically ProgrammerState.PostProgramming.
         """
         next_step = ProgrammerState.ProgrammingError
         number_of_programming_blocks = len(self._programming_file.get_blocks())
         addr_size_len = self._programming_file.get_address_and_length_format_identifier().get("request_download")
         try:
             for block_idx, (block_name, block_data) in enumerate(self._programming_file.get_blocks().items()):
-                self.current_programming_block = (block_name, block_idx, number_of_programming_blocks)
+                self.current_programming_block = {"block_name": block_name,
+                                                  "block_data": block_data,
+                                                  "block_idx": block_idx,
+                                                  "number_of_programming_blocks": number_of_programming_blocks}
                 self._logger.debug("Programming Block {0}".format(block_name))
                 addr = block_data.get("addr")
                 data = block_data.get("data")
                 erase_block = block_data.get("erase_block")
                 compression_method = block_data.get("compression_method")
                 encryption_method = block_data.get("encryption_method")
                 transfer_request_parameters = block_data.get("transfer_request_parameters")
@@ -438,38 +482,39 @@
 
     @abstractmethod
     def pre_block_download(self,
                            addr: int,
                            erase_block: bool,
                            ) -> None:
         """
-        Prepare a block download. Subfunction to BlockProgramming State.
+        Prepare a block download. Sub-function to BlockProgramming State.
         This function intended for block specific tasks before the block is downloaded.
         In general there are multiple things to do when programming a block.
         At first there are hardware constraints. A non-volatile flash memory block needs to be erased
-        before it can be programmed again. Therefore the uds client commands the uds server to erase
+        before it can be programmed again. Therefore, the uds client commands the uds server to erase
         that block, typically be routine control uds service.
         Another task may be the use of a journal for a block, e.g. a programming entry, who?, what?, when?,
-        how often has the block been programmed, when does it starts to wear out?
+        how often has the block been programmed, when does it start to wear out?
 
         :return: Nothing.
         """
 
     def download_block(self,
                        addr: int,
                        data: bytes,
                        size: int,
                        addr_size_len: Union[str, Tuple[int, int]] = "auto",
                        compression_method: CompressionMethod = CompressionMethod.NO_COMPRESSION,
                        encryption_method: EncryptionMethod = EncryptionMethod.NO_ENCRYPTION,
                        transfer_request_parameters: bytes = bytes(),
                        ) -> None:
         """
-        Download a block, subfunction to Block Programming State.
+        Download a block, subf-unction to Block Programming State.
         This function is universal due to the defined set of uds services for this purpose.
+
         :param addr: The address of the download.
         :param data: The data to be transferred.
         :param compression_method: The method of compression.
         :param encryption_method: The method of encryption.
         :param transfer_request_parameters: A never used manufacturer specific value.
         :param size: The uncompressed size of the block.
         :param addr_size_len: A tuple of fixed address and size or "auto".
@@ -503,60 +548,63 @@
     @abstractmethod
     def post_block_download(self,
                             addr: int,
                             checksum: bytes,
                             signature: bytes,
                             ) -> None:
         """
-        Check a block after download. Subfunction to Block Programming State
+        Check a block after download. Sub-function to Block Programming State
         This function is intended for block specific tasks after a block was downloaded.
         Typical task is a check for data integrity, e.g. the uds client starts a checksum routine
         on the uds server and either provides the expected checksum for check or the uds server sends
         the checksum back, so the client can compare and decide what to do.
         There may also be crypto involved, e.g. a signature check.
 
         :return: Nothing.
         """
 
     @abstractmethod
     def post_programming(self) -> ProgrammerState:
         """
         Post programming.
         This function is intended for the big cleanup after the block programming has happened.
-        The goal is to have the freshly programmed device resume it's tasks by starting application again.
+        The goal is to have the freshly programmed device resume its tasks by starting application again.
         This is usually done by switching back to default session or calling ecu reset.
         After the device is running application again, it may also be needed to re-enable services that have
-        been disabled in pre programming step.
+        been disabled in pre-programming step.
+
         :return: The next state, typically ProgrammerState.ProgrammingFinished.
         """
 
 
 class ExampleUdsProgrammer(UdsProgrammerABC):
+    """
+    This class is for testing purposes only.
+    """
 
     def pre_programming(self) -> ProgrammerState:
         """
         Check if the logical preconditions for programming are fulfilled.
         You won't flash an engine ecu while the engine is running, would you?
         Well it can be done in some rare cases.
+
         :return: The next state.
         """
         next_state = ProgrammerState.ProgrammingError
-        try:
-            check_programming_did = 0xBEEF
-            data = self._client.read_data_by_id(did=check_programming_did).get("data")
-            status = bool.from_bytes(data, "big")
-            if status:
-                next_state = ProgrammerState.SwitchToProgrammingMode
-        except UdsProtocolException:
-            pass
+        check_programming_did = 0xBEEF
+        data = self._client.read_data_by_id(did=check_programming_did).get("data")
+        status = bool.from_bytes(data, "big")
+        if status:
+            next_state = ProgrammerState.SwitchToProgrammingMode
         return next_state
 
     def unlock_device(self) -> ProgrammerState:
         """
         Execute seed and key routine to unlock the device.
+
         :return: The next state.
         """
         next_state = ProgrammerState.ProgrammingError
         try:
             security_level = 1
             seed = self._client.security_access(security_level=security_level).get("seed")
             key = struct.pack(">I", struct.unpack(">I", seed)[0] + 1)
@@ -569,45 +617,125 @@
     def pre_block_download(self,
                            addr: int,
                            erase_block: bool,
                            ) -> None:
         """
         Write the workshop name into the device for
         an easy example.
+
         :param addr: The address of the block.
         :param erase_block: The erase flag.
         :return: Nothing
         """
         workshop_did = 0xCAFE
         self._client.write_data_by_id(did=workshop_did, data="1234".encode())
 
     def post_block_download(self,
                             addr: int,
                             checksum: bytes,
                             signature: bytes,
                             ) -> None:
         """
         Execute a check routine in device.
+
         :param addr: The address of the block.
         :param checksum: The block checksum.
         :param signature: The block signature.
         :return: Nothing.
         """
         self._client.routine_control(routine_control_type=RoutineControlType.StartRoutine,
                                      routine_id=0x1234,
                                      data=bytes.fromhex("11 22 33 44 55 66 77 88"))
 
     def post_programming(self) -> ProgrammerState:
         """
         Write the programming date for an easy example.
+
         :return: The next programming state.
         """
         programming_date_did = 0x4242
         self._client.write_data_by_id(did=programming_date_did, data=bytes.fromhex("11 22 33 44"))
         return ProgrammerState.ProgrammingFinished
 
     def access_unblock_wait(self) -> ProgrammerState:
         """
         Dummy Implementation. Return the previous state.
+
         :return: The previous state.
         """
         return self.previous_state
+
+
+class OdxFileProgrammerBase(UdsProgrammerABC):
+    """
+    This class is the Base class for all ODX-file based programmers.
+    It should aggregate functions common to this type and be used as test
+    class.
+    """
+
+    def load_programming_file(self, filepath: Path) -> None:
+        """
+        Load the programming file. In this case a pdx file.
+        :param filepath: The filepath to the pdx file.
+        :return: None
+        """
+        self._programming_file = read_odx_update_container(filepath=filepath)
+
+    def unlock_device(self) -> ProgrammerState:
+        """
+        Proceed to Block Programming.
+
+        :return: Next State.
+        """
+        return ProgrammerState.BlockProgramming
+
+    def pre_programming(self) -> ProgrammerState:
+        """
+        Proceed to SwitchToProgrammingMode.
+
+        :return: Next State.
+        """
+        return ProgrammerState.SwitchToProgrammingMode
+
+    def access_unblock_wait(self) -> ProgrammerState:
+        """
+        Proceed to previous State.
+
+        :return: Next State.
+        """
+        return self.previous_state
+
+    def pre_block_download(self,
+                           addr: int,
+                           erase_block: bool,
+                           ) -> None:
+        """
+        Execute some procedure pre block download.
+
+        :param addr: The address of the block.
+        :param erase_block: The erase flag.
+        :return: Nothing
+        """
+        pass
+
+    def post_block_download(self,
+                            addr: int,
+                            checksum: bytes,
+                            signature: bytes):
+        """
+        Execute some procedure post block download.
+
+        :param addr: The address of the block.
+        :param checksum: The block checksum.
+        :param signature: The block signature.
+        :return: Nothing.
+        """
+        pass
+
+    def post_programming(self) -> ProgrammerState:
+        """
+        Proceed to Programming Finished.
+
+        :return: The next programming state.
+        """
+
+        return ProgrammerState.ProgrammingFinished
```

### Comparing `socketcan-uds-0.4.0/uds/security_access.py` & `socketcan-uds-0.5.0/uds/security_access.py`

 * *Files identical despite different names*

