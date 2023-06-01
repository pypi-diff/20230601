# Comparing `tmp/spectrum_io-0.1.0.tar.gz` & `tmp/spectrum_io-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_io-0.1.0.tar", max compression
+gzip compressed data, was "spectrum_io-0.2.0.tar", max compression
```

## Comparing `spectrum_io-0.1.0.tar` & `spectrum_io-0.2.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1072 2023-03-09 12:47:14.755679 spectrum_io-0.1.0/LICENSE
--rw-r--r--   0        0        0     2411 2023-03-09 12:47:14.755679 spectrum_io-0.1.0/README.rst
--rw-r--r--   0        0        0     2338 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1048 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/__init__.py
--rw-r--r--   0        0        0      351 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/__main__.py
--rw-r--r--   0        0        0      103 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/file/__init__.py
--rw-r--r--   0        0        0      479 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/file/csv.py
--rw-r--r--   0        0        0     5874 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/file/hdf5.py
--rw-r--r--   0        0        0        0 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/py.typed
--rw-r--r--   0        0        0      104 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/__init__.py
--rw-r--r--   0        0        0     6349 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/msraw.py
--rw-r--r--   0        0        0     3742 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/thermo_raw.py
--rwxr-xr-x   0        0        0    33200 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll
--rwxr-xr-x   0        0        0     5384 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb
--rwxr-xr-x   0        0        0    17827 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml
--rwxr-xr-x   0        0        0   136192 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll
--rwxr-xr-x   0        0        0    73260 2023-03-09 12:47:14.759679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb
--rwxr-xr-x   0        0        0   607957 2023-03-09 12:47:14.763679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml
--rwxr-xr-x   0        0        0   904704 2023-03-09 12:47:14.767679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll
--rwxr-xr-x   0        0        0   245016 2023-03-09 12:47:14.767679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb
--rwxr-xr-x   0        0        0   726825 2023-03-09 12:47:14.771679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml
--rwxr-xr-x   0        0        0   636928 2023-03-09 12:47:14.775679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll
--rwxr-xr-x   0        0        0   281820 2023-03-09 12:47:14.775679 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb
--rwxr-xr-x   0        0        0  1215406 2023-03-09 12:47:14.779680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml
--rwxr-xr-x   0        0        0    15360 2023-03-09 12:47:14.779680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll
--rw-r--r--   0        0        0    11324 2023-03-09 12:47:14.779680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE
--rwxr-xr-x   0        0        0  1689600 2023-03-09 12:47:14.791680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll
--rwxr-xr-x   0        0        0  3688730 2023-03-09 12:47:14.799680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml
--rwxr-xr-x   0        0        0    45168 2023-03-09 12:47:14.799680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll
--rwxr-xr-x   0        0        0   229376 2023-03-09 12:47:14.799680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll
--rwxr-xr-x   0        0        0   181640 2023-03-09 12:47:14.803680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml
--rwxr-xr-x   0        0        0    52224 2023-03-09 12:47:14.803680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll
--rwxr-xr-x   0        0        0    40909 2023-03-09 12:47:14.803680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml
--rwxr-xr-x   0        0        0   701992 2023-03-09 12:47:14.807680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll
--rwxr-xr-x   0        0        0   698888 2023-03-09 12:47:14.807680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml
--rwxr-xr-x   0        0        0    34304 2023-03-09 12:47:14.807680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll
--rwxr-xr-x   0        0        0    61952 2023-03-09 12:47:14.807680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll
--rwxr-xr-x   0        0        0    50343 2023-03-09 12:47:14.807680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml
--rwxr-xr-x   0        0        0   159232 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll
--rwxr-xr-x   0        0        0    91970 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml
--rwxr-xr-x   0        0        0    20856 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll
--rwxr-xr-x   0        0        0     3445 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml
--rwxr-xr-x   0        0        0    28552 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll
--rwxr-xr-x   0        0        0    64416 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml
--rwxr-xr-x   0        0        0   141184 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll
--rwxr-xr-x   0        0        0    13585 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml
--rwxr-xr-x   0        0        0   115856 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll
--rwxr-xr-x   0        0        0   180815 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml
--rwxr-xr-x   0        0        0    16768 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll
--rwxr-xr-x   0        0        0    17733 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml
--rwxr-xr-x   0        0        0    33672 2023-03-09 12:47:14.811680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll
--rwxr-xr-x   0        0        0   218987 2023-03-09 12:47:14.815680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml
--rwxr-xr-x   0        0        0    18312 2023-03-09 12:47:14.815680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll
--rwxr-xr-x   0        0        0    89643 2023-03-09 12:47:14.815680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml
--rwxr-xr-x   0        0        0   758664 2023-03-09 12:47:14.819680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll
--rwxr-xr-x   0        0        0     2048 2023-03-09 12:47:14.819680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml
--rwxr-xr-x   0        0        0    25232 2023-03-09 12:47:14.819680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll
--rwxr-xr-x   0        0        0      134 2023-03-09 12:47:14.819680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.xml
--rw-r--r--   0        0        0     6509 2023-03-09 12:47:14.819680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE
--rw-r--r--   0        0        0   404480 2023-03-09 12:47:14.819680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll
--rw-r--r--   0        0        0  1433139 2023-03-09 12:47:14.827680 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml
--rw-r--r--   0        0        0   639488 2023-03-09 12:47:14.831681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll
--rw-r--r--   0        0        0  1547413 2023-03-09 12:47:14.835681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml
--rw-r--r--   0        0        0   174592 2023-03-09 12:47:14.835681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe
--rw-r--r--   0        0        0     3096 2023-03-09 12:47:14.835681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config
--rw-r--r--   0        0        0    56512 2023-03-09 12:47:14.835681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb
--rw-r--r--   0        0        0  4630427 2023-03-09 12:47:14.851681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip
--rw-r--r--   0        0        0      920 2023-03-09 12:47:14.851681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config
--rwxr-xr-x   0        0        0   270336 2023-03-09 12:47:14.855681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll
--rwxr-xr-x   0        0        0  1513051 2023-03-09 12:47:14.859681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml
--rwxr-xr-x   0        0        0   480768 2023-03-09 12:47:14.859681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll
--rwxr-xr-x   0        0        0  1086558 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml
--rwxr-xr-x   0        0        0    69632 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll
--rw-r--r--   0        0        0      122 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/search_result/__init__.py
--rw-r--r--   0        0        0     4892 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/search_result/mascot.py
--rw-r--r--   0        0        0     5511 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/search_result/maxquant.py
--rw-r--r--   0        0        0     3760 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/search_result/msfragger.py
--rw-r--r--   0        0        0     1506 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/search_result/search_results.py
--rw-r--r--   0        0        0      191 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/__init__.py
--rw-r--r--   0        0        0    22116 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/digest.py
--rw-r--r--   0        0        0    45056 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib
--rw-r--r--   0        0        0     7867 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/dlib.py
--rw-r--r--   0        0        0    98385 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/msp/myPrositLib.msp
--rw-r--r--   0        0        0     3997 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/msp.py
--rw-r--r--   0        0        0     1212 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/spectral_library.py
--rw-r--r--   0        0        0   565091 2023-03-09 12:47:14.867681 spectrum_io-0.1.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
--rw-r--r--   0        0        0     4999 2023-03-09 12:47:14.863681 spectrum_io-0.1.0/spectrum_io/spectral_library/spectronaut.py
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 spectrum_io-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2411 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/README.rst
+-rw-r--r--   0        0        0     2338 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1048 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/__init__.py
+-rw-r--r--   0        0        0      351 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/__main__.py
+-rw-r--r--   0        0        0      103 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/file/__init__.py
+-rw-r--r--   0        0        0      556 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/file/csv.py
+-rw-r--r--   0        0        0     5912 2023-06-01 16:20:57.401868 spectrum_io-0.2.0/spectrum_io/file/hdf5.py
+-rw-r--r--   0        0        0        0 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/py.typed
+-rw-r--r--   0        0        0      104 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/__init__.py
+-rw-r--r--   0        0        0     9611 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/msraw.py
+-rw-r--r--   0        0        0     3742 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/thermo_raw.py
+-rwxr-xr-x   0        0        0    33200 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll
+-rwxr-xr-x   0        0        0     5384 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb
+-rwxr-xr-x   0        0        0    17827 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml
+-rwxr-xr-x   0        0        0   136192 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll
+-rwxr-xr-x   0        0        0    73260 2023-06-01 16:20:57.405868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb
+-rwxr-xr-x   0        0        0   607957 2023-06-01 16:20:57.409868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml
+-rwxr-xr-x   0        0        0   904704 2023-06-01 16:20:57.413868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll
+-rwxr-xr-x   0        0        0   245016 2023-06-01 16:20:57.413868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb
+-rwxr-xr-x   0        0        0   726825 2023-06-01 16:20:57.417868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml
+-rwxr-xr-x   0        0        0   636928 2023-06-01 16:20:57.421868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll
+-rwxr-xr-x   0        0        0   281820 2023-06-01 16:20:57.421868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb
+-rwxr-xr-x   0        0        0  1215406 2023-06-01 16:20:57.429868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml
+-rwxr-xr-x   0        0        0    15360 2023-06-01 16:20:57.429868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll
+-rw-r--r--   0        0        0    11324 2023-06-01 16:20:57.429868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE
+-rwxr-xr-x   0        0        0  1689600 2023-06-01 16:20:57.437868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll
+-rwxr-xr-x   0        0        0  3688730 2023-06-01 16:20:57.449868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml
+-rwxr-xr-x   0        0        0    45168 2023-06-01 16:20:57.449868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll
+-rwxr-xr-x   0        0        0   229376 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll
+-rwxr-xr-x   0        0        0   181640 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml
+-rwxr-xr-x   0        0        0    52224 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll
+-rwxr-xr-x   0        0        0    40909 2023-06-01 16:20:57.453868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml
+-rwxr-xr-x   0        0        0   701992 2023-06-01 16:20:57.457868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll
+-rwxr-xr-x   0        0        0   698888 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml
+-rwxr-xr-x   0        0        0    34304 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll
+-rwxr-xr-x   0        0        0    61952 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll
+-rwxr-xr-x   0        0        0    50343 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml
+-rwxr-xr-x   0        0        0   159232 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll
+-rwxr-xr-x   0        0        0    91970 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml
+-rwxr-xr-x   0        0        0    20856 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll
+-rwxr-xr-x   0        0        0     3445 2023-06-01 16:20:57.461868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml
+-rwxr-xr-x   0        0        0    28552 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll
+-rwxr-xr-x   0        0        0    64416 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml
+-rwxr-xr-x   0        0        0   141184 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll
+-rwxr-xr-x   0        0        0    13585 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml
+-rwxr-xr-x   0        0        0   115856 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll
+-rwxr-xr-x   0        0        0   180815 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml
+-rwxr-xr-x   0        0        0    16768 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll
+-rwxr-xr-x   0        0        0    17733 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml
+-rwxr-xr-x   0        0        0    33672 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll
+-rwxr-xr-x   0        0        0   218987 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml
+-rwxr-xr-x   0        0        0    18312 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll
+-rwxr-xr-x   0        0        0    89643 2023-06-01 16:20:57.465868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml
+-rwxr-xr-x   0        0        0   758664 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll
+-rwxr-xr-x   0        0        0     2048 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml
+-rwxr-xr-x   0        0        0    25232 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll
+-rwxr-xr-x   0        0        0      134 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.xml
+-rw-r--r--   0        0        0     6509 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE
+-rw-r--r--   0        0        0   404480 2023-06-01 16:20:57.473868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll
+-rw-r--r--   0        0        0  1433139 2023-06-01 16:20:57.485869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml
+-rw-r--r--   0        0        0   639488 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll
+-rw-r--r--   0        0        0  1547413 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml
+-rw-r--r--   0        0        0   174592 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe
+-rw-r--r--   0        0        0     3096 2023-06-01 16:20:57.489868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config
+-rw-r--r--   0        0        0    56512 2023-06-01 16:20:57.493868 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb
+-rw-r--r--   0        0        0  4630427 2023-06-01 16:20:57.509869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip
+-rw-r--r--   0        0        0      920 2023-06-01 16:20:57.509869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config
+-rwxr-xr-x   0        0        0   270336 2023-06-01 16:20:57.513869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll
+-rwxr-xr-x   0        0        0  1513051 2023-06-01 16:20:57.517869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml
+-rwxr-xr-x   0        0        0   480768 2023-06-01 16:20:57.521869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll
+-rwxr-xr-x   0        0        0  1086558 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml
+-rwxr-xr-x   0        0        0    69632 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll
+-rw-r--r--   0        0        0      122 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/__init__.py
+-rw-r--r--   0        0        0     4410 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/mascot.py
+-rw-r--r--   0        0        0     4507 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/maxquant.py
+-rw-r--r--   0        0        0     3634 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/msfragger.py
+-rw-r--r--   0        0        0     2685 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/search_result/search_results.py
+-rw-r--r--   0        0        0      191 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/__init__.py
+-rw-r--r--   0        0        0    22116 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/digest.py
+-rw-r--r--   0        0        0    45056 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib
+-rw-r--r--   0        0        0     7918 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/dlib.py
+-rw-r--r--   0        0        0    98385 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/msp/myPrositLib.msp
+-rw-r--r--   0        0        0     3997 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/msp.py
+-rw-r--r--   0        0        0     1148 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/spectral_library.py
+-rw-r--r--   0        0        0   565091 2023-06-01 16:20:57.529869 spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv
+-rw-r--r--   0        0        0     4999 2023-06-01 16:20:57.525869 spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut.py
+-rw-r--r--   0        0        0     3618 1970-01-01 00:00:00.000000 spectrum_io-0.2.0/PKG-INFO
```

### Comparing `spectrum_io-0.1.0/LICENSE` & `spectrum_io-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/README.rst` & `spectrum_io-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/pyproject.toml` & `spectrum_io-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_io"
-version = "0.1.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.2.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "IO related functionalities for oktoberfest."
 authors = ["Mario Picciani <mario.picciani@tum.de>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_io"
 repository = "https://github.com/wilhelm-lab/spectrum_io"
 documentation = "https://spectrum_io.readthedocs.io"
@@ -27,15 +27,15 @@
 numpy = "^1.18.1"
 pandas = "^1.3.0"
 h5py = "^3.1.0"
 pymzml = "^2.5.0"
 pyteomics = "^4.3.3"
 lxml= '^4.5.2'
 tables = "^3.6.1"
-spectrum-fundamentals = "^0.3.0"
+spectrum-fundamentals = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.3"
 coverage = {extras = ["toml"], version = ">=5.3"}
 safety = ">=1.9.0"
 typeguard = ">=2.12.0"
 xdoctest = {extras = ["colors"], version = ">=0.15.0"}
```

### Comparing `spectrum_io-0.1.0/spectrum_io/__init__.py` & `spectrum_io-0.2.0/spectrum_io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for spectrum_io."""
 
 __author__ = "Mario Picciani"
 __email__ = "mario.picciani@tum.de"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 from . import file, raw
```

### Comparing `spectrum_io-0.1.0/spectrum_io/file/hdf5.py` & `spectrum_io-0.2.0/spectrum_io/file/hdf5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import threading
+from pathlib import Path
 from typing import List, Optional, Union
 
 import h5py
 import pandas as pd
 import scipy
 from scipy.sparse import coo_matrix
 
@@ -11,15 +12,15 @@
 
 META_DATA_KEY = "meta_data"
 INTENSITY_RAW_KEY = "raw_intensity"
 INTENSITY_PRED_KEY = "pred_intensity"
 MZ_RAW_KEY = "raw_mz"
 
 
-def read_file(path: str, key: str) -> pd.DataFrame:
+def read_file(path: Union[str, Path], key: str) -> pd.DataFrame:
     """
     Read hdf5 file and return dataframe with contents.
 
     With possibility to partial load for memory issues.
     :param path: The path to the hdf5 file to read
     :param key: The key of the dataset/group of interest
     :return: a pandas DataFrame with contents
```

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/msraw.py` & `spectrum_io-0.2.0/spectrum_io/raw/msraw.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,78 @@
 import logging
-import os
 import warnings
 from abc import abstractmethod
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
+from xml.etree import ElementTree
 
 import pandas as pd
 import pymzml
 from pyteomics import mzml
 from spectrum_fundamentals.constants import MZML_DATA_COLUMNS
 
 logger = logging.getLogger(__name__)
 
 
+def get_mass_analyzer(file_path: Path) -> str:
+    """
+    Retrieve mass analyzer information from mzml file.
+
+    This is using the description of the mzml format to check for specific accessions in the mzml file
+    that are not covered by pyteomics or pymzml. The documentation can be found here:
+    https://raw.githubusercontent.com/HUPO-PSI/psi-ms-CV/master/psi-ms.obo
+
+    :param file_path: The path to the mzml file to parse
+    :raises AssertionError: if the mass analyzer metadata cannot be found in the file or the search
+        was conducted with an unsupported mass analyzer.
+    :return: A string that is either FTMS or ITMS to represent the respective mass analyzer category.
+    """
+    tree = ElementTree.parse(file_path)
+    root = tree.getroot()
+    namespace = {"ns0": "http://psi.hupo.org/ms/mzml"}
+    analyzer = root.find(
+        ".//ns0:instrumentConfigurationList/ns0:instrumentConfiguration/ns0:componentList/ns0:analyzer/ns0:cvParam",
+        namespace,
+    )
+    if analyzer is None:
+        raise AssertionError("The mass analyzer information can not be retrieved from the mzml file!")
+
+    acc = analyzer.get("accession")
+    if acc in ["MS:1000079", "MS:1000484"]:  # fourier transform ion cyclotron, orbitrap
+        mass_analyzer = "FTMS"
+    elif acc in ["MS:1000082", "MS:1000264"]:  # quadrupole ion-trap, io-trap
+        mass_analyzer = "ITMS"
+    elif acc in ["MS:1000084"]:  # TOF
+        mass_analyzer = "TOF"
+    else:
+        raise AssertionError(f"The mass analyzer with accession {acc} ({analyzer.get('name')}) is not supported.")
+
+    return mass_analyzer
+
+
 class MSRaw:
     """Main to read mzml file and generate dataframe containing intensities and m/z values."""
 
-    path: Optional[str]
-    output_path: Optional[str]
-
-    def __init__(self, path: Optional[str] = None, output_path: Optional[str] = None):
+    def __init__(self, path: Optional[Union[str, Path]] = None, output_path: Optional[Union[str, Path]] = None):
         """
         Initialize a MSRaw object.
 
         :param path: path to mzml file
         :param output_path: path to save the output file
         """
+        if isinstance(path, str):
+            path = Path(path)
+        if isinstance(output_path, str):
+            output_path = Path(output_path)
         self.path = path
         self.output_path = output_path
 
     @staticmethod
     def read_mzml(
-        source: Union[str, List[str]],
+        source: Union[str, Path, List[Union[str, Path]]],
         ext: str = "mzml",
         package: str = "pyteomics",
         search_type: str = "Maxquant",
         scanidx: Optional[List] = None,
         *args,
         **kwargs,
     ) -> pd.DataFrame:
@@ -47,101 +85,135 @@
         :param scanidx: optional list of scan numbers to extract. if not specified, all scans will be extracted
         :param search_type: type of the search (Maxquant, Mascot, Msfragger)
         :param args: additional positional arguments
         :param kwargs: additional keyword arguments
         :raises AssertionError: if package has an unexpected type
         :return: pd.DataFrame with intensities and m/z values
         """
-        if isinstance(source, str):
-            file_list = MSRaw.get_file_list(source, ext)
-            source = file_list
+        file_list = MSRaw.get_file_list(source, ext)
         data = {}  # type: Dict[str, Any]
         if package == "pymzml":
             with warnings.catch_warnings():
                 warnings.filterwarnings("ignore", category=ImportWarning)
-                for file_path in source:
+                for file_path in file_list:
                     logger.info(f"Reading mzML file: {file_path}")
                     MSRaw._get_scans_pymzml(file_path, data, scanidx, *args, **kwargs)
         elif package == "pyteomics":
-            for file_path in source:
+            for file_path in file_list:
+                mass_analyzer = get_mass_analyzer(file_path)
                 logger.info(f"Reading mzML file: {file_path}")
-                data_iter = mzml.read(source=file_path, *args, **kwargs)
-                file_name = os.path.splitext(os.path.basename(file_path))[0]
+                data_iter = mzml.read(source=str(file_path), *args, **kwargs)
+                file_name = file_path.stem
                 for spec in data_iter:
-                    id = spec["id"].split("scan=")[-1]
-                    mass_analyzer = spec["scanList"]["scan"][0]["filter string"].split()[0]
-                    fragmentation = spec["scanList"]["scan"][0]["filter string"].split("@")[1][:3]
-                    mz_range = spec["scanList"]["scan"][0]["filter string"].split("[")[1][:-1]
-                    key = f"{file_name}_{id}"
-                    if search_type == "maxquant":
-                        data[key] = [file_name, id, spec["intensity array"], spec["m/z array"], mz_range]
-                    else:
+                    if spec["ms level"] != 1:  # filter out ms1 spectra if there are any
+                        spec_id = spec["id"].split("scan=")[-1]
+                        fragmentation = spec["scanList"]["scan"][0]["filter string"].split("@")[1][:3].upper()
+                        mz_range = spec["scanList"]["scan"][0]["filter string"].split("[")[1][:-1]
+                        rt = spec["scanList"]["scan"][0]["scan start time"]
+                        key = f"{file_name}_{spec_id}"
                         data[key] = [
                             file_name,
-                            id,
+                            spec_id,
                             spec["intensity array"],
                             spec["m/z array"],
                             mz_range,
+                            rt,
                             mass_analyzer,
                             fragmentation,
                         ]
                 data_iter.close()
         else:
             raise AssertionError("Choose either 'pymzml' or 'pyteomics'")
-        if search_type == "maxquant":
-            data = pd.DataFrame.from_dict(data, orient="index", columns=MZML_DATA_COLUMNS)
-        else:
-            data = pd.DataFrame.from_dict(
-                data, orient="index", columns=MZML_DATA_COLUMNS + ["MASS_ANALYZER", "FRAGMENTATION"]
-            )
+
+        data = pd.DataFrame.from_dict(data, orient="index", columns=MZML_DATA_COLUMNS)
         data["SCAN_NUMBER"] = pd.to_numeric(data["SCAN_NUMBER"])
         return data
 
     @staticmethod
-    def get_file_list(source: Union[str, List[str]], ext: str = "mzml"):
+    def get_file_list(source: Union[str, Path, List[Union[str, Path]]], ext: str = "mzml") -> List[Path]:
         """
         Get list of files from source.
 
         :param source: a directory containing mzml files, a list of files or a single file
         :param ext: file extension for searching a specified directory
+        :raises FileNotFoundError: if one of the files given by source does not exist
+        :raises TypeError: if source is not given as a str, Path or list object
         :return: list of files
         """
         file_list = []
-        if isinstance(source, str) and os.path.isdir(source):
-            # if string is provided and is a directory, search all mzml files with provided extension
-            for file in os.listdir(source):
-                if file.lower().endswith(ext.lower()):
-                    file_list.append(file)
-
-        else:
-            if isinstance(source, list):
-                file_list.extend(source)
+        if isinstance(source, str):
+            source = Path(source)
+        if isinstance(source, Path):
+            if source.is_file():
+                file_list = [source]
+            elif source.is_dir():
+                file_list = list(source.glob("*[mM][zZ][mM][lL]"))
             else:
-                file_list.append(source)
+                raise FileNotFoundError(f"{source} does not exist.")
+        elif isinstance(source, list):
+            for elem in source:
+                if isinstance(elem, str):
+                    elem = Path(elem)
+                if elem.is_file():
+                    file_list.append(elem)
+                else:
+                    raise FileNotFoundError(f"{elem} does not exist,")
+        else:
+            raise TypeError("source can only be a single str or Path or a list of files.")
         return file_list
 
     @staticmethod
-    def _get_scans_pymzml(file_path: str, data: Dict, scanidx: Optional[List] = None, *args, **kwargs) -> None:
+    def _get_scans_pymzml(
+        file_path: Union[str, Path], data: Dict, scanidx: Optional[List] = None, *args, **kwargs
+    ) -> None:
         """
         Reads mzml and generates a dataframe containing intensities and m/z values.
 
         :param file_path: path to a single mzml file.
         :param data: dictionary to be added to by this function
         :param scanidx: optional list of scan numbers to extract. if not specified, all scans will be extracted
         :param args: additional positional arguments
         :param kwargs: additional keyword arguments
         """
+        if isinstance(file_path, str):
+            file_path = Path(file_path)
         data_iter = pymzml.run.Reader(file_path, args=args, kwargs=kwargs)
-        file_name = os.path.splitext(os.path.basename(file_path))[0]
+        file_name = file_path.stem
+        mass_analyzer = get_mass_analyzer(file_path)
         if scanidx is None:
             for spec in data_iter:
-                key = f"{file_name}_{spec.ID}"
-                data[key] = [file_name, spec.ID, spec.i, spec.mz]
+                if spec.ms_level != 1:  # filter out ms1 spectra if there are any
+                    key = f"{file_name}_{spec.ID}"
+                    filter_string = str(spec.element.find(".//*[@accession='MS:1000512']").get("value"))
+                    fragmentation = filter_string.split("@")[1][:3].upper()
+                    mz_range = filter_string.split("[")[1][:-1]
+                    data[key] = [
+                        file_name,
+                        spec.ID,
+                        spec.i,
+                        spec.mz,
+                        mz_range,
+                        spec.scan_time_in_minutes(),
+                        mass_analyzer,
+                        fragmentation,
+                    ]
         else:
             for idx in scanidx:
                 spec = data_iter[idx]
                 # this does not work if some spectra are filtered out, e.g. mzML files with only MS2 spectra, see:
                 # https://github.com/pymzml/pymzML/blob/a883ff0e61fd97465b0a74667233ff594238e335/pymzml/file_classes
                 # /standardMzml.py#L81-L84
                 key = f"{file_name}_{spec.ID}"
-                data[key] = [file_name, spec.ID, spec.i, spec.mz]
+                filter_string = str(spec.element.find(".//*[@accession='MS:1000512']").get("value"))
+                fragmentation = filter_string.split("@")[1][:3].upper()
+                mz_range = filter_string.split("[")[1][:-1]
+                data[key] = [
+                    file_name,
+                    spec.ID,
+                    spec.i,
+                    spec.mz,
+                    mz_range,
+                    spec.scan_time_in_minutes(),
+                    mass_analyzer,
+                    fragmentation,
+                ]
         data_iter.close()
```

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/thermo_raw.py` & `spectrum_io-0.2.0/spectrum_io/raw/thermo_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 import subprocess
 from pathlib import Path
 from sys import platform
 from typing import Any, List, Optional, Tuple, Union
 
 from .msraw import MSRaw
 
@@ -30,15 +29,15 @@
         "-i",
         input_path,
         "-b",
         output_path,
     ]
     if gzip:
         exec_arg_list.append("-g")
-    if "linux" in platform:
+    if "linux" in platform or platform == "darwin":
         exec_arg_list.insert(0, "mono")
 
     return exec_arg_list
 
 
 class ThermoRaw(MSRaw):
     """Main to convert a ThermoRaw file into mzml file."""
@@ -73,29 +72,29 @@
         if isinstance(ms_level, int):
             ms_level = [ms_level]
         for level in ms_level:
             _type_check(level, "all ms_levels in list", int)
             if not 1 <= level <= 3:
                 raise ValueError(f"Value of all ms_levels must be within [1,3]. Got {level}")
 
-        if os.path.isfile(output_path):
+        if output_path.is_file():
             logger.info(f"Found converted file at {output_path}, skipping conversion")
             return output_path
 
         exec_arg_list = _assemble_arg_list(input_path, output_path, ms_level, gzip)
 
         logger.info(
             f"Converting thermo rawfile to mzml with the command: {' '.join([str(arg) for arg in exec_arg_list])}"
         )
 
         try:
             subprocess.run(exec_arg_list, shell=False, check=True)
         except subprocess.CalledProcessError:
-            if os.path.isfile(output_path):
-                os.remove(output_path)
+            if output_path.is_file():
+                output_path.unlink()
             raise  # reraise only after removing a corrupted file
 
         return output_path
 
 
 if __name__ == "__main__":
     from sys import argv
```

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWS.Logger.Core.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.CloudWatchLogs.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.Core.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/AWSSDK.S3.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/IronSnappy.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/MathNet.Numerics.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Mono.Options.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/NJsonSchema.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Namotion.Reflection.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.Extensions.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/OpenMcdf.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/Parquet.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Buffers.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.IO.FileSystem.AccessControl.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Memory.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Numerics.Vectors.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Runtime.CompilerServices.Unsafe.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.AccessControl.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Security.Principal.Windows.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.Text.Encoding.CodePages.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/System.ValueTuple.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/THERMO_LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.Data.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoFisher.CommonCore.RawFileReader.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.exe.config`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.pdb`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/ThermoRawFileParser.zip`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.config`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/log4net.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/nunit.framework.xml`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll` & `spectrum_io-0.2.0/spectrum_io/raw/utils/ThermoRawFileParser/zlib.net.dll`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/search_result/mascot.py` & `spectrum_io-0.2.0/spectrum_io/search_result/mascot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 import sqlite3
-from typing import Optional
+from pathlib import Path
+from typing import Optional, Union
 
 import pandas as pd
 import spectrum_fundamentals.constants as c
 from spectrum_fundamentals.mod_string import internal_without_mods
 
-from .search_results import SearchResults
+from .search_results import SearchResults, filter_valid_prosit_sequences
 
 logger = logging.getLogger(__name__)
 
 
 class Mascot(SearchResults):
     """Handle search results from Mascot."""
 
     @staticmethod
-    def read_result(path: str, tmt_labeled: str) -> pd.DataFrame:
+    def read_result(path: Union[str, Path], tmt_labeled: str) -> pd.DataFrame:
         """
         Function to read a mascot msf file and perform some basic formatting.
 
         :param path: path to msms.txt to read
         :param tmt_labeled: tmt label as str
         :return: pd.DataFrame with the formatted data
         """
@@ -51,15 +52,14 @@
 
         df.rename(
             columns={
                 "SpectrumID": "SCAN NUMBER",
                 "ModifiedSequence": "MODIFIED SEQUENCE",
                 "Charge": "PRECURSOR CHARGE",
                 "XCorr": "SCORE",
-                "RetentionTime": "RETENTION TIME",
                 "SpectrumFileName": "RAW FILE",
             },
             inplace=True,
         )
 
         # Standardize column names
         df.columns = df.columns.str.upper()
@@ -69,15 +69,15 @@
         logger.info("Converting MSFragger  peptide sequence to internal format")
         df["RAW_FILE"] = df["RAW_FILE"].str.replace(".raw", "")
         df["MODIFICATIONS"] = (
             (df["POSITION"].astype(int) - 1).astype(str) + "$" + df["DELTAMONOISOTOPICMASS"].astype(str)
         )
         df = df.groupby("SCAN_NUMBER", as_index=False).apply(lambda x: x.sort_values("POSITION"))
         df = df.groupby(
-            ["SCAN_NUMBER", "PRECURSOR_CHARGE", "SCORE", "RETENTION_TIME", "RAW_FILE", "SEQUENCE", "REVERSE"],
+            ["SCAN_NUMBER", "PRECURSOR_CHARGE", "SCORE", "RAW_FILE", "SEQUENCE", "REVERSE"],
             as_index=False,
         ).agg({"MODIFICATIONS": "|".join})
         mod_masses_reverse = {round(float(v), 3): k for k, v in c.MOD_MASSES.items()}
 
         sequences = []
         for _, row in df.iterrows():
             modifications = row["MODIFICATIONS"].split("|")
@@ -96,16 +96,9 @@
                     skip = skip + len(mod_masses_reverse[round(float(mass), 3)])
                 sequences.append(sequence)
 
         df["MODIFIED_SEQUENCE"] = sequences
 
         df["SEQUENCE"] = internal_without_mods(df["MODIFIED_SEQUENCE"])
         df["PEPTIDE_LENGTH"] = df["SEQUENCE"].apply(lambda x: len(x))
-        logger.info(f"No of sequences before Filtering is {len(df['PEPTIDE_LENGTH'])}")
-        df = df[(df["PEPTIDE_LENGTH"] <= 30)]
-        df = df[(~df["MODIFIED_SEQUENCE"].str.contains(r"\(ac\)"))]
-        df = df[(~df["MODIFIED_SEQUENCE"].str.contains(r"\(Acetyl \(Protein N-term\)\)"))]
-        df = df[(~df["SEQUENCE"].str.contains("U"))]
-        df = df[df["PRECURSOR_CHARGE"] <= 6]
-        df = df[df["PEPTIDE_LENGTH"] >= 7]
-        logger.info(f"No of sequences after Filtering is {len(df['PEPTIDE_LENGTH'])}")
-        return df
+
+        return filter_valid_prosit_sequences(df)
```

### Comparing `spectrum_io-0.1.0/spectrum_io/search_result/maxquant.py` & `spectrum_io-0.2.0/spectrum_io/search_result/maxquant.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
+from pathlib import Path
+from typing import Union
 
 import pandas as pd
 import spectrum_fundamentals.constants as c
 from spectrum_fundamentals.mod_string import internal_without_mods, maxquant_to_internal
 
-from .search_results import SearchResults
+from .search_results import SearchResults, filter_valid_prosit_sequences
 
 logger = logging.getLogger(__name__)
 
 
 class MaxQuant(SearchResults):
     """Handle search results from MaxQuant."""
 
@@ -23,15 +25,15 @@
         :return: mass as float
         """
         num_of_tmt = seq.count(unimod_tag)
         mass += num_of_tmt * c.MOD_MASSES[f"{unimod_tag}"]
         return mass
 
     @staticmethod
-    def read_result(path: str, tmt_labeled: str) -> pd.DataFrame:
+    def read_result(path: Union[str, Path], tmt_labeled: str) -> pd.DataFrame:
         """
         Function to read a msms txt and perform some basic formatting.
 
         :param path: path to msms.txt to read
         :param tmt_labeled: tmt label as str
         :return: pd.DataFrame with the formatted data
         """
@@ -40,51 +42,42 @@
             path,
             usecols=lambda x: x.upper()
             in [
                 "RAW FILE",
                 "SCAN NUMBER",
                 "MODIFIED SEQUENCE",
                 "CHARGE",
-                "FRAGMENTATION",
-                "MASS ANALYZER",
                 "SCAN EVENT NUMBER",
                 "LABELING STATE",
                 "MASS",  # = Calculated Precursor mass; TODO get column with experimental Precursor mass instead
                 "SCORE",
                 "REVERSE",
-                "RETENTION TIME",
             ],
             sep="\t",
         )
         logger.info("Finished reading msms.txt file")
 
         # Standardize column names
         df.columns = df.columns.str.upper()
         df.columns = df.columns.str.replace(" ", "_")
 
         df = MaxQuant.update_columns_for_prosit(df, tmt_labeled)
-        df = MaxQuant.filter_valid_prosit_sequences(df)
-
-        return df
+        return filter_valid_prosit_sequences(df)
 
     @staticmethod
     def update_columns_for_prosit(df: pd.DataFrame, tmt_labeled: str) -> pd.DataFrame:
         """
         Update columns of df to work with Prosit.
 
         :param df: df to modify
         :param tmt_labeled: True if tmt labeled
         :return: modified df as pd.DataFrame
         """
         df.rename(columns={"CHARGE": "PRECURSOR_CHARGE"}, inplace=True)
 
-        if "MASS_ANALYZER" not in df.columns:
-            df["MASS_ANALYZER"] = "FTMS"
-        if "FRAGMENTATION" not in df.columns:
-            df["FRAGMENTATION"] = "HCD"
         df["REVERSE"].fillna(False, inplace=True)
         df["REVERSE"].replace("+", True, inplace=True)
         logger.info("Converting MaxQuant peptide sequence to internal format")
         if tmt_labeled != "":
             unimod_tag = c.TMT_MODS[tmt_labeled]
             logger.info("Adding TMT fixed modifications")
             df["MODIFIED_SEQUENCE"] = maxquant_to_internal(
@@ -111,26 +104,7 @@
             df.drop(columns=["LABELING_STATE"], inplace=True)
         else:
             df["MODIFIED_SEQUENCE"] = maxquant_to_internal(df["MODIFIED_SEQUENCE"].to_numpy())
         df["SEQUENCE"] = internal_without_mods(df["MODIFIED_SEQUENCE"])
         df["PEPTIDE_LENGTH"] = df["SEQUENCE"].apply(lambda x: len(x))
 
         return df
-
-    @staticmethod
-    def filter_valid_prosit_sequences(df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Filter valid Prosit sequences.
-
-        :param df: df to filter
-        :return: df after filtration
-        """
-        logger.info(f"#sequences before filtering for valid prosit sequences: {len(df.index)}")
-        df = df[(df["PEPTIDE_LENGTH"] <= 30)]
-        df = df[(~df["MODIFIED_SEQUENCE"].str.contains("(ac)", regex=False))]
-        df = df[(~df["MODIFIED_SEQUENCE"].str.contains("(Acetyl (Protein N-term))", regex=False))]
-        df = df[(~df["SEQUENCE"].str.contains("U"))]
-        df = df[df["PRECURSOR_CHARGE"] <= 6]
-        df = df[df["PEPTIDE_LENGTH"] >= 7]
-        logger.info(f"#sequences after filtering for valid prosit sequences: {len(df.index)}")
-
-        return df
```

### Comparing `spectrum_io-0.1.0/spectrum_io/search_result/msfragger.py` & `spectrum_io-0.2.0/spectrum_io/search_result/msfragger.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
+from pathlib import Path
+from typing import Union
 
 import pandas as pd
 import spectrum_fundamentals.constants as c
 from spectrum_fundamentals.mod_string import internal_without_mods
 
-from .search_results import SearchResults
+from .search_results import SearchResults, filter_valid_prosit_sequences
 
 logger = logging.getLogger(__name__)
 
 
 class MSFragger(SearchResults):
     """Handle search results from MSFragger."""
 
     @staticmethod
-    def read_result(path: str, tmt_labeled: str) -> pd.DataFrame:
+    def read_result(path: Union[str, Path], tmt_labeled: str) -> pd.DataFrame:
         """
         Function to read a msms txt and perform some basic formatting.
 
         :param path: path to msms.txt to read
         :param tmt_labeled: tmt label as str
         :return: pd.DataFrame with the formatted data
         """
@@ -28,36 +30,46 @@
             in [
                 "SCANID",
                 "PEPTIDE SEQUENCE",
                 "PRECURSOR CHARGE",
                 "PRECURSOR NEUTRAL MASS (DA)",
                 "HYPERSCORE",
                 "PROTEIN",
-                "RETENTION TIME (MINUTES)",
                 "VARIABLE MODIFICATIONS DETECTED (STARTS WITH M, SEPARATED BY |, FORMATED AS POSITION,MASS)",
             ],
         )
         logger.info("Finished reading msfragger xlsx file")
 
         df.rename(
             columns={
                 "ScanID": "SCAN NUMBER",
                 "Peptide Sequence": "MODIFIED SEQUENCE",
                 "Precursor neutral mass (Da)": "MASS",
                 "Hyperscore": "SCORE",
-                "Retention time (minutes)": "RETENTION TIME",
                 "Variable modifications detected (starts with M, separated by |, formated as position,mass)": "MODIFICATIONS",
             },
             inplace=True,
         )
 
         # Standardize column names
         df.columns = df.columns.str.upper()
         df.columns = df.columns.str.replace(" ", "_")
 
+        df = MSFragger.update_columns_for_prosit(df, tmt_labeled)
+        return filter_valid_prosit_sequences(df)
+
+    @staticmethod
+    def update_columns_for_prosit(df, tmt_labeled: str) -> pd.DataFrame:
+        """
+        Update columns of df to work with Prosit.
+
+        :param df: df to modify
+        :param tmt_labeled: True if tmt labeled
+        :return: modified df as pd.DataFrame
+        """
         df.rename(columns={"CHARGE": "PRECURSOR_CHARGE"}, inplace=True)
 
         df["REVERSE"] = df["PROTEIN"].str.contains("Reverse")
         # df["RAW_FILE"] = df.iloc[0]["PROTEIN"]
         df["RAW_FILE"] = "01625b_GA6-TUM_first_pool_41_01_01-DDA-1h-R2"
         logger.info("Converting MSFragger  peptide sequence to internal format")
 
@@ -81,16 +93,8 @@
                 sequences.append(sequence)
 
         df["MODIFIED_SEQUENCE"] = sequences
 
         df["SEQUENCE"] = internal_without_mods(df["MODIFIED_SEQUENCE"])
         df["PEPTIDE_LENGTH"] = df["SEQUENCE"].apply(lambda x: len(x))
 
-        logger.info(f"No of sequences before Filtering is {len(df['PEPTIDE_LENGTH'])}")
-        df = df[(df["PEPTIDE_LENGTH"] <= 30)]
-        df = df[(~df["MODIFIED_SEQUENCE"].str.contains(r"\(ac\)"))]
-        df = df[(~df["MODIFIED_SEQUENCE"].str.contains(r"\(Acetyl \(Protein N-term\)\)"))]
-        df = df[(~df["SEQUENCE"].str.contains("U"))]
-        df = df[df["PRECURSOR_CHARGE"] <= 6]
-        df = df[df["PEPTIDE_LENGTH"] >= 7]
-        logger.info(f"No of sequences after Filtering is {len(df['PEPTIDE_LENGTH'])}")
         return df
```

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/digest.py` & `spectrum_io-0.2.0/spectrum_io/spectral_library/digest.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib` & `spectrum_io-0.2.0/spectrum_io/spectral_library/dlib/myPrositLib.dlib`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/dlib.py` & `spectrum_io-0.2.0/spectrum_io/spectral_library/dlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sqlite3
 import zlib
+from pathlib import Path
 from typing import List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from spectrum_fundamentals.mod_string import internal_to_mod_mass, internal_without_mods
 
 from .spectral_library import SpectralLibrary
@@ -28,15 +29,15 @@
         self,
         precursor_mz: Union[List[float], np.ndarray],
         precursor_charges: Union[List[int], np.ndarray],
         modified_sequences: List[str],
         retention_times: Union[List[float], np.ndarray],
         fragmentmz: List[np.ndarray],
         intensities: List[np.ndarray],
-        path: str,
+        path: Union[str, Path],
         min_intensity_threshold: Optional[float] = 0.05,
     ):
         """
         Initializer for the DLib class.
 
         :param precursor_mz: precursor mass to charge ratios
         :param precursor_charges: precurosr charges
@@ -114,15 +115,15 @@
             mz_bytes_list.append(zlib.compress(bytes_mz))
             i_bytes_list.append(zlib.compress(bytes(bytes_i)))
             mz_lengths.append(len(bytes_mz))
             i_lengths.append(len(bytes_i))
         return mz_bytes_list, i_bytes_list, mz_lengths, i_lengths
 
     @staticmethod
-    def create_database(path: str):
+    def create_database(path: Union[str, Path]):
         """
         Creates the database file with prefab tables entries, peptidetoprotein (p2p) and metadata, according to the \
         dlib specification.
 
         :param path: specifies the path of the created database file
         """
         sql_create_entries = """
```

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/msp/myPrositLib.msp` & `spectrum_io-0.2.0/spectrum_io/spectral_library/msp/myPrositLib.msp`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/msp.py` & `spectrum_io-0.2.0/spectrum_io/spectral_library/msp.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/spectral_library.py` & `spectrum_io-0.2.0/spectrum_io/spectral_library/spectral_library.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from abc import abstractmethod
+from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 
 
 class SpectralLibrary:
     """Main to initialze a SpectralLibrary obj."""
 
-    # Check https://gitlab.lrz.de/proteomics/prosit_tools/converter for old code
-    spectra_input: pd.DataFrame
-    grpc_output: dict
-    spectra_output: pd.DataFrame
-    out_path: str
-
-    def __init__(self, input_dataframe: pd.DataFrame, grpc_dict: dict, output_path: str):
+    def __init__(self, input_dataframe: pd.DataFrame, grpc_dict: dict, output_path: Union[str, Path]):
         """
         Initialize a SpectralLibrary obj.
 
         :param input_dataframe: dataframe of sequences, charges, and masses of all library peptides
         :param grpc_dict: GRPC client output dictionary with spectrum, irt, and proteotypicity prediction
         :param output_path: path to output file including file name
         """
+        if isinstance(output_path, str):
+            output_path = Path(output_path)
         self.spectra_input = input_dataframe
         self.grpc_output = grpc_dict
         self.out_path = output_path
 
     def load(self):
         """Load predictions from hdf5 file."""
```

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv` & `spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut/myPrositLib.csv`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/spectrum_io/spectral_library/spectronaut.py` & `spectrum_io-0.2.0/spectrum_io/spectral_library/spectronaut.py`

 * *Files identical despite different names*

### Comparing `spectrum_io-0.1.0/PKG-INFO` & `spectrum_io-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: spectrum-io
-Version: 0.1.0
+Version: 0.2.0
 Summary: IO related functionalities for oktoberfest.
 Home-page: https://github.com/wilhelm-lab/spectrum_io
 License: MIT
 Author: Mario Picciani
 Author-email: mario.picciani@tum.de
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: h5py (>=3.1.0,<4.0.0)
 Requires-Dist: lxml (>=4.5.2,<5.0.0)
 Requires-Dist: numpy (>=1.18.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pymzml (>=2.5.0,<3.0.0)
 Requires-Dist: pyteomics (>=4.3.3,<5.0.0)
 Requires-Dist: rich (>=10.3.0)
-Requires-Dist: spectrum-fundamentals (>=0.3.0,<0.4.0)
+Requires-Dist: spectrum-fundamentals (>=0.4.0,<0.5.0)
 Requires-Dist: tables (>=3.6.1,<4.0.0)
 Project-URL: Documentation, https://spectrum_io.readthedocs.io
 Project-URL: Repository, https://github.com/wilhelm-lab/spectrum_io
 Description-Content-Type: text/x-rst
 
 spectrum_io
 ===========================
```

