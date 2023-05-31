# Comparing `tmp/tpds_schema-1.0.1-py3-none-any.whl.zip` & `tmp/tpds_schema-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,37 @@
-Zip file size: 96079 bytes, number of entries: 14
--rw-r--r--  2.0 unx       65 b- defN 23-Mar-14 22:00 tpds/__init__.py
--rw-r--r--  2.0 unx      191 b- defN 23-Mar-14 22:00 tpds/schema/__init__.py
--rw-r--r--  2.0 unx    82303 b- defN 23-Mar-14 22:00 tpds/schema/data/cryptoauth/ECC204_TA010_Config_1.0.xsd
--rw-r--r--  2.0 unx    47350 b- defN 23-Mar-14 22:00 tpds/schema/data/generic/Provisioning_Config_1.0.xsd
--rw-r--r--  2.0 unx   153562 b- defN 23-Mar-14 22:00 tpds/schema/data/trustanchor/TA100_Config_1.0.xsd
--rw-r--r--  2.0 unx   154890 b- defN 23-Mar-14 22:00 tpds/schema/data/trustanchor/TA100_Config_1.1.xsd
--rw-r--r--  2.0 unx     7200 b- defN 23-Mar-14 22:00 tpds/schema/models/__init__.py
--rw-r--r--  2.0 unx   113750 b- defN 23-Mar-14 22:00 tpds/schema/models/ecc204_ta010_config_1_0.py
--rw-r--r--  2.0 unx   199850 b- defN 23-Mar-14 22:00 tpds/schema/models/ta100_config_1_1.py
--rw-r--r--  2.0 unx     1322 b- defN 23-Mar-14 22:02 tpds_schema-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2351 b- defN 23-Mar-14 22:02 tpds_schema-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-14 22:02 tpds_schema-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-14 22:02 tpds_schema-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1282 b- defN 23-Mar-14 22:02 tpds_schema-1.0.1.dist-info/RECORD
-14 files, 764213 bytes uncompressed, 93921 bytes compressed:  87.7%
+Zip file size: 136265 bytes, number of entries: 35
+-rw-r--r--  2.0 unx       65 b- defN 23-May-31 23:17 tpds/__init__.py
+-rw-r--r--  2.0 unx      523 b- defN 23-May-31 23:17 tpds/schema/__init__.py
+-rw-r--r--  2.0 unx    82303 b- defN 23-May-31 23:17 tpds/schema/data/cryptoauth/ECC204_TA010_Config_1.0.xsd
+-rw-r--r--  2.0 unx    90307 b- defN 23-May-31 23:17 tpds/schema/data/cryptoauth/ECC204_TA010_Config_1.1.xsd
+-rw-r--r--  2.0 unx    47350 b- defN 23-May-31 23:17 tpds/schema/data/generic/Provisioning_Config_1.0.xsd
+-rw-r--r--  2.0 unx   153562 b- defN 23-May-31 23:17 tpds/schema/data/trustanchor/TA100_Config_1.0.xsd
+-rw-r--r--  2.0 unx   154890 b- defN 23-May-31 23:17 tpds/schema/data/trustanchor/TA100_Config_1.1.xsd
+-rw-r--r--  2.0 unx       15 b- defN 23-May-31 23:17 tpds/schema/models/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 23:17 tpds/schema/models/common/__init__.py
+-rw-r--r--  2.0 unx       97 b- defN 23-May-31 23:17 tpds/schema/models/common/algo_1_0.py
+-rw-r--r--  2.0 unx     5962 b- defN 23-May-31 23:17 tpds/schema/models/common/cert_def_1_0.py
+-rw-r--r--  2.0 unx     5299 b- defN 23-May-31 23:17 tpds/schema/models/common/config_1_0.py
+-rw-r--r--  2.0 unx     6954 b- defN 23-May-31 23:17 tpds/schema/models/common/data_1_0.py
+-rw-r--r--  2.0 unx     1628 b- defN 23-May-31 23:17 tpds/schema/models/common/extension_1_0.py
+-rw-r--r--  2.0 unx     1238 b- defN 23-May-31 23:17 tpds/schema/models/common/otp_1_0.py
+-rw-r--r--  2.0 unx     1866 b- defN 23-May-31 23:17 tpds/schema/models/common/types.py
+-rw-r--r--  2.0 unx       72 b- defN 23-May-31 23:17 tpds/schema/models/ecc108_1_0/__init__.py
+-rw-r--r--  2.0 unx     6409 b- defN 23-May-31 23:17 tpds/schema/models/ecc108_1_0/ecc108_config_1_0.py
+-rw-r--r--  2.0 unx     7394 b- defN 23-May-31 23:17 tpds/schema/models/ecc204_1_0/__init__.py
+-rw-r--r--  2.0 unx   113683 b- defN 23-May-31 23:17 tpds/schema/models/ecc204_1_0/ecc204_ta010_config_1_0.py
+-rw-r--r--  2.0 unx     8390 b- defN 23-May-31 23:17 tpds/schema/models/ecc204_1_1/__init__.py
+-rw-r--r--  2.0 unx   124161 b- defN 23-May-31 23:17 tpds/schema/models/ecc204_1_1/ecc204_ta010_config_1_1.py
+-rw-r--r--  2.0 unx       72 b- defN 23-May-31 23:17 tpds/schema/models/ecc508_1_0/__init__.py
+-rw-r--r--  2.0 unx     5380 b- defN 23-May-31 23:17 tpds/schema/models/ecc508_1_0/ecc508_config_1_0.py
+-rw-r--r--  2.0 unx      267 b- defN 23-May-31 23:17 tpds/schema/models/ecc608_1_0/__init__.py
+-rw-r--r--  2.0 unx     9509 b- defN 23-May-31 23:17 tpds/schema/models/ecc608_1_0/ecc608_config_1_0.py
+-rw-r--r--  2.0 unx       72 b- defN 23-May-31 23:17 tpds/schema/models/sha204_1_0/__init__.py
+-rw-r--r--  2.0 unx     7129 b- defN 23-May-31 23:17 tpds/schema/models/sha204_1_0/sha204_config_1_0.py
+-rw-r--r--  2.0 unx     4062 b- defN 23-May-31 23:17 tpds/schema/models/ta100_1_1/__init__.py
+-rw-r--r--  2.0 unx   199847 b- defN 23-May-31 23:17 tpds/schema/models/ta100_1_1/ta100_config_1_1.py
+-rw-r--r--  2.0 unx     1322 b- defN 23-May-31 23:18 tpds_schema-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2903 b- defN 23-May-31 23:18 tpds_schema-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 23:18 tpds_schema-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-31 23:18 tpds_schema-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3389 b- defN 23-May-31 23:18 tpds_schema-1.1.0.dist-info/RECORD
+35 files, 1046217 bytes uncompressed, 130669 bytes compressed:  87.5%
```

## zipnote {}

```diff
@@ -3,41 +3,104 @@
 
 Filename: tpds/schema/__init__.py
 Comment: 
 
 Filename: tpds/schema/data/cryptoauth/ECC204_TA010_Config_1.0.xsd
 Comment: 
 
+Filename: tpds/schema/data/cryptoauth/ECC204_TA010_Config_1.1.xsd
+Comment: 
+
 Filename: tpds/schema/data/generic/Provisioning_Config_1.0.xsd
 Comment: 
 
 Filename: tpds/schema/data/trustanchor/TA100_Config_1.0.xsd
 Comment: 
 
 Filename: tpds/schema/data/trustanchor/TA100_Config_1.1.xsd
 Comment: 
 
 Filename: tpds/schema/models/__init__.py
 Comment: 
 
-Filename: tpds/schema/models/ecc204_ta010_config_1_0.py
+Filename: tpds/schema/models/common/__init__.py
+Comment: 
+
+Filename: tpds/schema/models/common/algo_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/common/cert_def_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/common/config_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/common/data_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/common/extension_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/common/otp_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/common/types.py
+Comment: 
+
+Filename: tpds/schema/models/ecc108_1_0/__init__.py
+Comment: 
+
+Filename: tpds/schema/models/ecc108_1_0/ecc108_config_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/ecc204_1_0/__init__.py
+Comment: 
+
+Filename: tpds/schema/models/ecc204_1_0/ecc204_ta010_config_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/ecc204_1_1/__init__.py
+Comment: 
+
+Filename: tpds/schema/models/ecc204_1_1/ecc204_ta010_config_1_1.py
+Comment: 
+
+Filename: tpds/schema/models/ecc508_1_0/__init__.py
+Comment: 
+
+Filename: tpds/schema/models/ecc508_1_0/ecc508_config_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/ecc608_1_0/__init__.py
+Comment: 
+
+Filename: tpds/schema/models/ecc608_1_0/ecc608_config_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/sha204_1_0/__init__.py
+Comment: 
+
+Filename: tpds/schema/models/sha204_1_0/sha204_config_1_0.py
+Comment: 
+
+Filename: tpds/schema/models/ta100_1_1/__init__.py
 Comment: 
 
-Filename: tpds/schema/models/ta100_config_1_1.py
+Filename: tpds/schema/models/ta100_1_1/ta100_config_1_1.py
 Comment: 
 
-Filename: tpds_schema-1.0.1.dist-info/LICENSE
+Filename: tpds_schema-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: tpds_schema-1.0.1.dist-info/METADATA
+Filename: tpds_schema-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: tpds_schema-1.0.1.dist-info/WHEEL
+Filename: tpds_schema-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: tpds_schema-1.0.1.dist-info/top_level.txt
+Filename: tpds_schema-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tpds_schema-1.0.1.dist-info/RECORD
+Filename: tpds_schema-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpds/schema/__init__.py

```diff
@@ -1,8 +1,18 @@
 import os
 
+# This import is required in order to use the datamodels properly as
+# it adds additional validators to the pydantic system
+import xsdata_pydantic.bindings  # noqa F401
+
 
 def get_ecc204_ta010_xsd_path():
-    return os.path.join(os.path.dirname(__file__), "data", "cryptoauth", "ECC204_TA010_Config_1.0.xsd")
+    return os.path.join(
+        os.path.dirname(__file__), "data", "cryptoauth", "ECC204_TA010_Config_1.1.xsd"
+    )
+
+
+def get_ta100_xsd_path():
+    return os.path.join(os.path.dirname(__file__), "data", "trustanchor", "TA100_Config_1.1.xsd")
 
 
-__all__ = ['get_ecc204_ta010_xsd_path']
+__all__ = ["get_ecc204_ta010_xsd_path", "get_ta100_xsd_path"]
```

## tpds/schema/models/__init__.py

```diff
@@ -1,263 +1 @@
-from tpds.schema.models.ecc204_ta010_config_1_0 import (
-    BooleanType,
-    ByteOrderType,
-    BytesEncodeHexType,
-    BytesEncodeType,
-    BytesPadType,
-    ChipModeCmosEn,
-    ChipModeClockDivider,
-    ClientDataItemType,
-    ClientDataType,
-    ClientDeviceDataType,
-    ConfigurationSubzone0Type,
-    ConfigurationSubzone0TypeValue,
-    ConfigurationSubzone1Type,
-    ConfigurationSubzone2Type,
-    ConfigurationSubzone3Type,
-    CounterType,
-    DerbinaryDataOrFromSourceType,
-    DataBase64,
-    DataHex10Bytes,
-    DataHex10BytesEncoding,
-    DataHex11Bytes,
-    DataHex11BytesEncoding,
-    DataHex12Bytes,
-    DataHex12BytesEncoding,
-    DataHex13Bytes,
-    DataHex13BytesEncoding,
-    DataHex14Bytes,
-    DataHex14BytesEncoding,
-    DataHex15Bytes,
-    DataHex15BytesEncoding,
-    DataHex16Bytes,
-    DataHex16BytesEncoding,
-    DataHex1Byte,
-    DataHex1ByteEncoding,
-    DataHex2Bytes,
-    DataHex2BytesEncoding,
-    DataHex3Bytes,
-    DataHex3BytesEncoding,
-    DataHex4Bytes,
-    DataHex4BytesEncoding,
-    DataHex5Bytes,
-    DataHex5BytesEncoding,
-    DataHex6Bytes,
-    DataHex6BytesEncoding,
-    DataHex7Bytes,
-    DataHex7BytesEncoding,
-    DataHex8Bytes,
-    DataHex8BytesEncoding,
-    DataHex9Bytes,
-    DataHex9BytesEncoding,
-    DataSourceType,
-    DataSourcesType,
-    DataSourcesWrappedKeyType,
-    DataSourcesWriterType,
-    DataTypeEnum,
-    DatabaseDataFieldType,
-    DatabaseDataType,
-    DateTimeModifyType,
-    DefinitionEncoding,
-    DeviceGenerateKeyType,
-    Ecc204Config,
-    Ecc204Ta010ConfigType,
-    EccFormat,
-    EncryptionAlgorithmEnum,
-    FixedSizeAlignment,
-    GenerateKeyEcctype,
-    GenerateKeyRsatype,
-    HsmgenerateKeyType,
-    HsmrandomType,
-    HashAlgorithmAndNoneEnum,
-    HashAlgorithmEnum,
-    IdMethodIssuerAndSerialNumber,
-    IoOptionsInterface,
-    KeyIdentifierCalculatedEnum,
-    KeyIdentifierCalculatedType,
-    PublicBinaryDataType,
-    PublicBinaryEncodingEnum,
-    ReferenceMappingsType,
-    SecretBinaryDataType,
-    SecretBinaryEncodingEnum,
-    SignatureAlgorithmEcdsatype,
-    SignatureAlgorithmRsa15Type,
-    SignatureAlgorithmRsapsstype,
-    SignatureAlgorithmRsapsstypeTrailerField,
-    SignatureAlgorithmType,
-    SlotConfig3WriteMode,
-    SlotLocksType,
-    StaticBytesType,
-    StaticPrivateKeyPublicType,
-    StaticPrivateKeySecretType,
-    StaticPrivateKeyType,
-    StaticPublicKeyPublicType,
-    StaticPublicKeySecretType,
-    StaticPublicKeyType,
-    StringCaseType,
-    StringOrDataOrFromSourceType,
-    Ta010Config,
-    TemplateType,
-    ValueType,
-    X509AuthorityKeyIdentifierType,
-    X509BasicConstraintsType,
-    X509BasicConstraintsTypeValue,
-    X509CacertificateChainType,
-    X509CertificateOrFromSource,
-    X509CertificateType,
-    X509ExtendedKeyUsageType,
-    X509ExtensionType,
-    X509ExtensionsType,
-    X509IssuerUniqueIdtype,
-    X509KeyUsageType,
-    X509NameType,
-    X509SerialNumberType,
-    X509SignatureAlgorithmEcdsatype,
-    X509SignatureAlgorithmRsa15Type,
-    X509SignatureAlgorithmRsapsstype,
-    X509SignatureAlgorithmRsapsstypeTrailerField,
-    X509SignatureAlgorithmType,
-    X509SubjectKeyIdentifierType,
-    X509SubjectPublicKeyInfoType,
-    X509SubjectUniqueIdtype,
-    X509TimeType,
-    X509TimeTypeType,
-    X509VersionType,
-    X520DirectoryStringOrFromSourceType,
-    X520DirectoryStringOrFromSourceTypeType,
-    X520Ia5StringOrFromSourceType,
-    X520Ia5StringOrFromSourceTypeType,
-    X520PrintableStringOrFromSourceType,
-    X520PrintableStringOrFromSourceTypeType,
-)
-
-__all__ = [
-    "BooleanType",
-    "ByteOrderType",
-    "BytesEncodeHexType",
-    "BytesEncodeType",
-    "BytesPadType",
-    "ChipModeCmosEn",
-    "ChipModeClockDivider",
-    "ClientDataItemType",
-    "ClientDataType",
-    "ClientDeviceDataType",
-    "ConfigurationSubzone0Type",
-    "ConfigurationSubzone0TypeValue",
-    "ConfigurationSubzone1Type",
-    "ConfigurationSubzone2Type",
-    "ConfigurationSubzone3Type",
-    "CounterType",
-    "DerbinaryDataOrFromSourceType",
-    "DataBase64",
-    "DataHex10Bytes",
-    "DataHex10BytesEncoding",
-    "DataHex11Bytes",
-    "DataHex11BytesEncoding",
-    "DataHex12Bytes",
-    "DataHex12BytesEncoding",
-    "DataHex13Bytes",
-    "DataHex13BytesEncoding",
-    "DataHex14Bytes",
-    "DataHex14BytesEncoding",
-    "DataHex15Bytes",
-    "DataHex15BytesEncoding",
-    "DataHex16Bytes",
-    "DataHex16BytesEncoding",
-    "DataHex1Byte",
-    "DataHex1ByteEncoding",
-    "DataHex2Bytes",
-    "DataHex2BytesEncoding",
-    "DataHex3Bytes",
-    "DataHex3BytesEncoding",
-    "DataHex4Bytes",
-    "DataHex4BytesEncoding",
-    "DataHex5Bytes",
-    "DataHex5BytesEncoding",
-    "DataHex6Bytes",
-    "DataHex6BytesEncoding",
-    "DataHex7Bytes",
-    "DataHex7BytesEncoding",
-    "DataHex8Bytes",
-    "DataHex8BytesEncoding",
-    "DataHex9Bytes",
-    "DataHex9BytesEncoding",
-    "DataSourceType",
-    "DataSourcesType",
-    "DataSourcesWrappedKeyType",
-    "DataSourcesWriterType",
-    "DataTypeEnum",
-    "DatabaseDataFieldType",
-    "DatabaseDataType",
-    "DateTimeModifyType",
-    "DefinitionEncoding",
-    "DeviceGenerateKeyType",
-    "Ecc204Config",
-    "Ecc204Ta010ConfigType",
-    "EccFormat",
-    "EncryptionAlgorithmEnum",
-    "FixedSizeAlignment",
-    "GenerateKeyEcctype",
-    "GenerateKeyRsatype",
-    "HsmgenerateKeyType",
-    "HsmrandomType",
-    "HashAlgorithmAndNoneEnum",
-    "HashAlgorithmEnum",
-    "IdMethodIssuerAndSerialNumber",
-    "IoOptionsInterface",
-    "KeyIdentifierCalculatedEnum",
-    "KeyIdentifierCalculatedType",
-    "PublicBinaryDataType",
-    "PublicBinaryEncodingEnum",
-    "ReferenceMappingsType",
-    "SecretBinaryDataType",
-    "SecretBinaryEncodingEnum",
-    "SignatureAlgorithmEcdsatype",
-    "SignatureAlgorithmRsa15Type",
-    "SignatureAlgorithmRsapsstype",
-    "SignatureAlgorithmRsapsstypeTrailerField",
-    "SignatureAlgorithmType",
-    "SlotConfig3WriteMode",
-    "SlotLocksType",
-    "StaticBytesType",
-    "StaticPrivateKeyPublicType",
-    "StaticPrivateKeySecretType",
-    "StaticPrivateKeyType",
-    "StaticPublicKeyPublicType",
-    "StaticPublicKeySecretType",
-    "StaticPublicKeyType",
-    "StringCaseType",
-    "StringOrDataOrFromSourceType",
-    "Ta010Config",
-    "TemplateType",
-    "ValueType",
-    "X509AuthorityKeyIdentifierType",
-    "X509BasicConstraintsType",
-    "X509BasicConstraintsTypeValue",
-    "X509CacertificateChainType",
-    "X509CertificateOrFromSource",
-    "X509CertificateType",
-    "X509ExtendedKeyUsageType",
-    "X509ExtensionType",
-    "X509ExtensionsType",
-    "X509IssuerUniqueIdtype",
-    "X509KeyUsageType",
-    "X509NameType",
-    "X509SerialNumberType",
-    "X509SignatureAlgorithmEcdsatype",
-    "X509SignatureAlgorithmRsa15Type",
-    "X509SignatureAlgorithmRsapsstype",
-    "X509SignatureAlgorithmRsapsstypeTrailerField",
-    "X509SignatureAlgorithmType",
-    "X509SubjectKeyIdentifierType",
-    "X509SubjectPublicKeyInfoType",
-    "X509SubjectUniqueIdtype",
-    "X509TimeType",
-    "X509TimeTypeType",
-    "X509VersionType",
-    "X520DirectoryStringOrFromSourceType",
-    "X520DirectoryStringOrFromSourceTypeType",
-    "X520Ia5StringOrFromSourceType",
-    "X520Ia5StringOrFromSourceTypeType",
-    "X520PrintableStringOrFromSourceType",
-    "X520PrintableStringOrFromSourceTypeType",
-]
+# nothing here
```

## Comparing `tpds/schema/models/ecc204_ta010_config_1_0.py` & `tpds/schema/models/ecc204_1_0/ecc204_ta010_config_1_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import field
 from enum import Enum
-from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
+
+from pydantic.dataclasses import dataclass
 from xsdata.models.datatype import XmlDateTime, XmlDuration
 
 __NAMESPACE__ = "https://www.microchip.com/schema/ECC204_TA010_Config_1.0"
 
 
 class AsymmetricSecretBinaryEncodingEnum(Enum):
     HEX = "Hex"
@@ -337,24 +338,22 @@
     """
     database_record_set_name: List["ReferenceMappingsType.DatabaseRecordSetName"] = field(
         default_factory=list,
         metadata={
             "name": "Database_Record_Set_Name",
             "type": "Element",
             "namespace": "https://www.microchip.com/schema/ECC204_TA010_Config_1.0",
-            "sequential": True,
         }
     )
     counter_name: List["ReferenceMappingsType.CounterName"] = field(
         default_factory=list,
         metadata={
             "name": "Counter_Name",
             "type": "Element",
             "namespace": "https://www.microchip.com/schema/ECC204_TA010_Config_1.0",
-            "sequential": True,
         }
     )
 
     @dataclass
     class DatabaseRecordSetName:
         external: Optional[str] = field(
             default=None,
@@ -2943,16 +2942,15 @@
             "required": True,
         }
     )
 
 
 @dataclass
 class X520Ia5StringOrFromSourceType(StringOrDataOrFromSourceType):
-    """Express a string using the IA5String type directly or from a data
-    source.
+    """Express a string using the IA5String type directly or from a data source.
 
     The Raw type allows one to specify the raw ASN.1 data for the value
     must include properly formed tag, length, and value in DER encoding.
     encoding attribute must be Hex or Base64 for this type.
     """
     class Meta:
         name = "X520IA5StringOrFromSourceType"
```

## Comparing `tpds/schema/models/ta100_config_1_1.py` & `tpds/schema/models/ta100_1_1/ta100_config_1_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import field
 from enum import Enum
-from pydantic.dataclasses import dataclass
 from typing import List, Optional, Union
+
+from pydantic.dataclasses import dataclass
 from xsdata.models.datatype import XmlDateTime, XmlDuration
 
 __NAMESPACE__ = "https://www.microchip.com/schema/TA100_Config_1.1"
 
 
 class BasicConstraintsValue(Enum):
     NO_LIMIT = "No_Limit"
@@ -1464,16 +1465,16 @@
                 "required": True,
                 "pattern": r"0b[01]{3}",
             }
         )
 
     @dataclass
     class GpioSecureBoot:
-        """GPIO will be configured to drive this pin to match the complement of
-        the Secure_Boot VCC latch.
+        """GPIO will be configured to drive this pin to match the complement of the
+        Secure_Boot VCC latch.
 
         On power-up, brownout, RESET pin assertion, or other boot
         events, this pin will be driven high. When a successful secure
         boot completes, this pin will be driven low.
 
         :ivar reserved: Reserved, must be 0b00000
         """
@@ -1486,16 +1487,16 @@
                 "required": True,
                 "pattern": r"0b[01]{5}",
             }
         )
 
     @dataclass
     class GpioPulse:
-        """GPIO_1 can effectively be configured to operate as an output
-        following the Reset state of the device.
+        """GPIO_1 can effectively be configured to operate as an output following the
+        Reset state of the device.
 
         When configured to be in this mode with Command_Complete,
         Init_Complete, Secure_Boot_Warn, and Secure_Boot_Clear set to
         False, the GPIO_1 output will be driven low during a POR, RESET
         pin assertion, brown-out, soft reboot, or any internal fault. It
         will then be driven high after a short delay (~1.5 ms) after the
         device reset source is released, as the device reboots. GPIO_1
@@ -2027,16 +2028,15 @@
             "required": True,
         }
     )
 
 
 @dataclass
 class Ia5StringOrFromSource(StringOrDataOrFromSource):
-    """Express a string using the IA5String type directly or from a data
-    source.
+    """Express a string using the IA5String type directly or from a data source.
 
     The Raw type allows one to specify the raw ASN.1 data for the value
     must include properly formed tag, length, and value in DER encoding.
     encoding attribute must be Hex or Base64 for this type.
     """
     class Meta:
         name = "IA5StringOrFromSource"
@@ -4465,17 +4465,17 @@
                     "required": True,
                     "pattern": r"0b[01]",
                 }
             )
 
         @dataclass
         class Idle:
-            """The idle time delay should be set such that the host is sure to
-            issue each command in a sequence before the timer expires, which
-            causes the internal state of the TA100 device to be reset.
+            """The idle time delay should be set such that the host is sure to issue each
+            command in a sequence before the timer expires, which causes the internal state
+            of the TA100 device to be reset.
 
             Setting the idle timer to a low value will optimize the
             power consumption by ensuring that the device goes into
             Sleep mode at the earliest possible time.
 
             :ivar enable: False: Idle timer is disabled. True: Idle
                 timer is enabled.
```

## Comparing `tpds_schema-1.0.1.dist-info/LICENSE` & `tpds_schema-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tpds_schema-1.0.1.dist-info/METADATA` & `tpds_schema-1.1.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpds-schema
-Version: 1.0.1
+Version: 1.1.0
 Summary: Microchip(SPG) Trust Platform Schemas
 Maintainer-email: Microchip Technology <SPG.Tools@microchip.com>
 License: (c) 2015-2023 Microchip Technology Inc. and its subsidiaries.
         
         Subject to your compliance with these terms, you may use the Microchip Software
         and any derivatives exclusively with Microchip products. It is your
         responsibility to comply with third party license terms applicable to your
@@ -32,19 +32,34 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: xsdata
 Requires-Dist: pydantic
 Requires-Dist: xsdata-pydantic
+Provides-Extra: dev
+Requires-Dist: flake8 ; extra == 'dev'
+Requires-Dist: black ; extra == 'dev'
+Requires-Dist: isort ; extra == 'dev'
+Requires-Dist: mypy ; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: pytest-cov ; extra == 'test'
+Requires-Dist: pytest-mock ; extra == 'test'
+Requires-Dist: pytest-integration ; extra == 'test'
+Requires-Dist: xmldiff ; extra == 'test'
 
 Trust Platform Design Suite - Schemas
 ==============================================================================
 
 This repo contains the package generation for the secure exchange process
 schemas
 
 To generate the models from the schemas:
 
 ```
-python -m xsdata --output pydantic --package tpds/schema/models <path_to_xsd>
+./scripts/generate_model.sh <model_package_name> <path_to_xsd>
+```
+
+For example to generate tpds.models.ecc204_1_0 model one would run (from the repo base)
+```
+./scripts/generate_model.sh ecc204_1_0 tpds/schema/data/cryptoauth/ECC204_TA010_Config_1.0.xsd
 ```
```

