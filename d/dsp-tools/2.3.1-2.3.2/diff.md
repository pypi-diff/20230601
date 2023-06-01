# Comparing `tmp/dsp_tools-2.3.1.tar.gz` & `tmp/dsp_tools-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.3.1.tar", max compression
+gzip compressed data, was "dsp_tools-2.3.2.tar", max compression
```

## Comparing `dsp_tools-2.3.1.tar` & `dsp_tools-2.3.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-05-24 07:58:06.593740 dsp_tools-2.3.1/LICENSE
--rw-r--r--   0        0        0     4373 2023-05-24 07:58:06.609734 dsp_tools-2.3.1/docs/index.md
--rw-r--r--   0        0        0     4916 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    19989 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    82048 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/__init__.py
--rw-r--r--   0        0        0    29477 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/process_files.py
--rw-r--r--   0        0        0    14393 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_files.py
--rw-r--r--   0        0        0     4148 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_xml.py
--rw-r--r--   0        0        0        0 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      962 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     9760 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0     3197 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     9538 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16915 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     9810 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    23066 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      506 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    19744 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2972 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    19128 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1930 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    21129 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1896 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    22134 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    34527 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      419 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0      890 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    27302 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    34725 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     2153 2023-05-24 07:58:06.613732 dsp_tools-2.3.1/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      747 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0      254 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlerror.py
--rw-r--r--   0        0        0     1841 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2371 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8874 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2614 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0     1488 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23543 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0     2867 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0        0 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15096 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4828 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     7818 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0    10202 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3174 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0    40875 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     8032 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4617 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    18724 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4242 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    12829 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0     6830 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    51407 2023-05-24 07:58:06.617731 dsp_tools-2.3.1/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 dsp_tools-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-01 06:56:39.377437 dsp_tools-2.3.2/LICENSE
+-rw-r--r--   0        0        0     4373 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/docs/index.md
+-rw-r--r--   0        0        0     4836 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    20257 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    88414 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/__init__.py
+-rw-r--r--   0        0        0    29382 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/process_files.py
+-rw-r--r--   0        0        0    14418 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_files.py
+-rw-r--r--   0        0        0     4173 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      962 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     9760 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0     3197 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     9538 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16915 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     9810 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    23066 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      506 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    19744 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2972 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    19128 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1930 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    21129 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1896 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    22134 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    34527 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      419 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0      890 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    27302 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    34725 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     2153 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      747 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0      254 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlerror.py
+-rw-r--r--   0        0        0     1841 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2371 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8874 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2614 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0     1488 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23543 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42584 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32171 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0     2867 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0        0 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15096 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4828 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     7818 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0    10202 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3174 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0     1157 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/logging.py
+-rw-r--r--   0        0        0    40900 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8057 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4617 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18724 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4242 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    12854 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0     6830 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    51156 2023-06-01 06:56:39.401439 dsp_tools-2.3.2/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 dsp_tools-2.3.2/PKG-INFO
```

### Comparing `dsp_tools-2.3.1/LICENSE` & `dsp_tools-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/docs/index.md` & `dsp_tools-2.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/pyproject.toml` & `dsp_tools-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.3.1"
+version = "2.3.2"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -35,15 +35,14 @@
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.11"
 mkdocs-include-markdown-plugin = "^4.0.4"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
-autopep8 = "^2.0.2"
 pytest = "^7.3.1"
 types-requests = "^2.30.0.0"
 types-lxml = "^2023.3.28"
 types-jsonschema = "^4.17.0.8"
 types-openpyxl = "^3.1.0.7"
 types-regex = "^2023.5.5.0"
 
@@ -66,19 +65,14 @@
 
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 # see https://docs.pytest.org/en/latest/explanation/goodpractices.html#tests-outside-application-code
 
 
-[tool.autopep8]
-max_line_length = 150
-experimental = true
-
-
 [tool.mypy]
 ignore_missing_imports = true              # TODO: deactivate this
 show_column_numbers = true
 strict = true
 exclude = [
     "src/dsp_tools/models",                # TODO: activate this
     "src/dsp_tools/import_scripts",        # TODO: activate this
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/dsp_tools.py` & `dsp_tools-2.3.2/src/dsp_tools/dsp_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
 The code in this file handles the arguments passed by the user from the command line and calls the requested actions.
 """
 import argparse
 import datetime
-import logging
-import logging.handlers
 import sys
 from importlib.metadata import version
-from pathlib import Path
 
 from dsp_tools.excel2xml import excel2xml
 from dsp_tools.fast_xmlupload.process_files import process_files
 from dsp_tools.fast_xmlupload.upload_files import upload_files
 from dsp_tools.fast_xmlupload.upload_xml import fast_xmlupload
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.excel_to_json_lists import (
@@ -19,23 +16,26 @@
     validate_lists_section_with_schema
 )
 from dsp_tools.utils.excel_to_json_project import excel2json
 from dsp_tools.utils.excel_to_json_properties import excel2properties
 from dsp_tools.utils.excel_to_json_resources import excel2resources
 from dsp_tools.utils.generate_templates import generate_template_repo
 from dsp_tools.utils.id_to_iri import id_to_iri
+from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.project_create import create_project
 from dsp_tools.utils.project_create_lists import create_lists
 from dsp_tools.utils.project_get import get_project
 from dsp_tools.utils.project_validate import validate_project
 from dsp_tools.utils.rosetta import upload_rosetta
 from dsp_tools.utils.shared import validate_xml_against_schema
 from dsp_tools.utils.stack_handling import start_stack, stop_stack
 from dsp_tools.utils.xml_upload import xml_upload
 
+logger = get_logger(__name__)
+
 
 def make_parser() -> argparse.ArgumentParser:
     """
     Create a parser for the command line arguments
 
     Returns:
         parser
@@ -224,43 +224,68 @@
         help="Clone the most up to data rosetta repository, create the data model and upload the data"
     )
     parser_rosetta.set_defaults(action="rosetta")
 
     return parser
 
 
+def _log_cli_arguments(parsed_args: argparse.Namespace) -> None:
+    """
+    Log the CLI arguments passed by the user from the command line.
+
+    Args:
+        parsed_args: parsed arguments
+    """
+    msg = f"*** Called the DSP-TOOLS action '{parsed_args.action}' from the command line with these parameters:"
+    parameters_to_log = {key: value for key, value in vars(parsed_args).items() if key != "action"}
+    longest_key_length = max(len(key) for key in parameters_to_log) if parameters_to_log else 0
+    lines = list()
+    for key, value in parameters_to_log.items():
+        if key == "password":
+            lines.append(f"***   {key:<{longest_key_length}} = {'*' * len(value)}")
+        else:
+            lines.append(f"***   {key:<{longest_key_length}} = {value}")
+    if not lines:
+        lines.append("***   (no parameters)")
+    asterisk_count = max(
+        len(msg), 
+        max(len(line) for line in lines)
+    )
+    logger.info("*" * asterisk_count)
+    logger.info(msg)
+    for line in lines:
+        logger.info(line)
+    logger.info("*" * asterisk_count)
+
+
 def call_requested_action(
     user_args: list[str],
-    parser: argparse.ArgumentParser,
-    logger: logging.Logger
+    parser: argparse.ArgumentParser
 ) -> bool:
     """
     With the help of the parser, parse the user arguments and call the appropriate method of DSP-TOOLS.
 
     Args:
         user_args: list of arguments passed by the user from the command line
         parser: parser to parse the user arguments
-        logger: the logger for this module
 
     Raises:
         BaseError from the called methods
         UserError from the called methods
         unexpected errors from the called methods and underlying libraries
 
     Returns:
         success status
     """
     args = parser.parse_args(user_args)
     if not hasattr(args, "action"):
         parser.print_help(sys.stderr)
         sys.exit(1)
 
-    logger.info("*****************************************************************************************")
-    logger.info(f"***Called DSP-TOOLS action '{args.action}' from command line with these parameters: {args}")
-    logger.info("*****************************************************************************************")
+    _log_cli_arguments(args)
 
     if args.action == "create":
         if args.lists_only:
             if args.validate_only:
                 success = validate_lists_section_with_schema(path_to_json_project_file=args.project_definition)
                 print("'Lists' section of the JSON project file is syntactically correct and passed validation.")
             else:
@@ -388,34 +413,19 @@
         logger.error(f"Unknown action '{args.action}'")
 
     return success
 
 
 def main() -> None:
     """Main entry point of the program as referenced in pyproject.toml"""
-    logging.basicConfig(
-        format="{asctime}   {filename: <20} {levelname: <8} {message}",
-        style="{",
-        level=logging.INFO,
-        handlers=[
-            logging.handlers.RotatingFileHandler(
-                filename=Path.home() / Path(".dsp-tools") / "logging.log",
-                maxBytes=3*1024*1024,
-                backupCount=1
-            )
-        ]
-    )
-    logger = logging.getLogger(__name__)
-
     parser = make_parser()
     try:
         success = call_requested_action(
             user_args=sys.argv[1:],
-            parser=parser,
-            logger=logger
+            parser=parser
         )
     except UserError as err:
         print(err.message)
         sys.exit(1)
     # let BaseError and all unexpected errors escalate, so that a stack trace is printed
 
     if not success:
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/excel2xml.py` & `dsp_tools-2.3.2/src/dsp_tools/excel2xml.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import datetime
 import difflib
 import json
 import os
 import re
 import uuid
 import warnings
-from operator import xor
-from typing import Any, Iterable, Optional, Union
+from typing import Any, Callable, Iterable, Optional, Union
 
 import pandas as pd
 import regex
 from lxml import etree
 from lxml.builder import E  # pylint: disable=no-name-in-module
 
 from dsp_tools.models.exceptions import BaseError
@@ -69,45 +68,14 @@
     # add uuid
     _uuid = uuid.uuid4()
     res = f"{res}_{_uuid}"
 
     return res
 
 
-def _derandomize_xsd_id(string: str, multiple_occurrences: bool = False) -> str:
-    """
-    In some contexts, the random component of the output of make_xsd_id_compatible() is a hindrance, especially for
-    testing. This method removes the random part, but leaves the other modifications introduced by
-    make_xsd_id_compatible() in place. This method's behaviour is defined by the example in the "Examples" section.
-
-    Args:
-        string: the output of make_xsd_id_compatible()
-        multiple_occurrences: If true, string can be an entire XML document, and all occurrences will be removed
-
-    Raises:
-        BaseError: if the input cannot be derandomized
-
-    Returns:
-        the derandomized string
-
-    Examples:
-        >>> id_1 = make_xsd_id_compatible("Hello!")
-        >>> id_2 = make_xsd_id_compatible("Hello!")
-        >>> assert _derandomize_xsd_id(id_1) == _derandomize_xsd_id(id_2)
-    """
-    if not isinstance(string, str) or not check_notna(string):
-        raise BaseError(f"The input '{string}' cannot be derandomized.")
-
-    uuid4_regex = r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}"
-    if multiple_occurrences:
-        return re.subn(uuid4_regex, "", string, flags=re.IGNORECASE)[0]
-    else:
-        return re.sub(uuid4_regex, "", string, re.IGNORECASE)
-
-
 def find_date_in_string(string: str) -> Optional[str]:
     """
     Checks if a string contains a date value (single date, or date range), and returns the first found date as
     DSP-formatted string. Returns None if no date was found.
 
     Notes:
         - All dates are interpreted in the Christian era and the Gregorian calendar. There is no support for BC dates or
@@ -1793,200 +1761,487 @@
     try:
         validate_xml_against_schema(input_file=filepath)
         print(f"The XML file was successfully saved to {filepath}")
     except BaseError as err:
         warnings.warn(f"The XML file was successfully saved to {filepath}, but the following Schema validation error(s) occurred: {err.message}")
 
 
-def excel2xml(datafile: str, shortcode: str, default_ontology: str) -> bool:
+def _read_cli_input_file(datafile: str) -> pd.DataFrame:
+    """
+    Parse the input file from the CLI (in either CSV or Excel format)
+
+    Args:
+        datafile: path to the input file
+
+    Raises:
+        BaseError: if the input file is neither .csv, .xls nor .xlsx
+
+    Returns:
+        a pandas DataFrame with the input data
     """
-    This is a method that is called from the command line. It isn't intended to be used in a Python script. It takes a
-    tabular data source in CSV/XLS(X) format that is formatted according to the specifications, and transforms it to DSP-
-    conforming XML file that can be uploaded to a DSP server with the xmlupload command. The output file is saved in the
-    same directory as the input file, with the name [default_ontology]-data.xml.
+    if re.search(r"\.csv$", datafile):
+        dataframe = pd.read_csv(
+            filepath_or_buffer=datafile, 
+            encoding="utf_8_sig",           # utf_8_sig is the default encoding of Excel
+            dtype="str", 
+            sep=None, 
+            engine="python"                 # let the "python" engine detect the separator
+        )
+    elif re.search(r"(\.xls|\.xlsx)$", datafile):
+        dataframe = pd.read_excel(
+            io=datafile, 
+            dtype="str"
+        )
+    else:
+        raise BaseError(f"Cannot open file '{datafile}': Invalid extension. Allowed extensions: 'csv', 'xls', 'xlsx'")
+    return dataframe
 
-    Please note that this method doesn't do any data cleaning or data transformation tasks. The input and the output of
-    this method are semantically exactly equivalent.
+
+def _validate_and_prepare_cli_input_file(dataframe: pd.DataFrame) -> pd.DataFrame:
+    """
+    Make sure that the required columns are present,
+    replace NA-like cells by NA,
+    remove empty columns, so that the max_num_of_props can be calculated without errors,
+    and remove empty rows, to prevent them from being processed and raising an error.
 
     Args:
-        datafile: path to the data file (CSV or XLS(X))
-        shortcode: shortcode of the project that this data belongs to
-        default_ontology: name of the ontology that this data belongs to
+        dataframe: pandas dataframe with the input data
 
     Raises:
-        BaseError if something went wrong
+        BaseError: if one of the required columns is missing
 
     Returns:
-        True if everything went well, False otherwise
+        the prepared pandas DataFrame
     """
+    # make sure that the required columns are present
+    required_columns = ["id", "label", "restype", "permissions", "prop name", "prop type", "1_value"]
+    if any(req not in dataframe for req in required_columns):
+        raise BaseError(f"Some columns in your input file are missing. The following columns are required: {required_columns}")
 
-    # general preparation
-    # -------------------
-    success = True
-    proptype_2_function = {
+    # replace NA-like cells by NA
+    dataframe = dataframe.applymap(
+        lambda x: x if pd.notna(x) and regex.search(r"[\p{L}\d_!?\-]", str(x), flags=regex.U) else pd.NA
+    )
+
+    # remove empty columns/rows
+    dataframe.dropna(axis="columns", how="all", inplace=True)
+    dataframe.dropna(axis="index", how="all", inplace=True)
+
+    return dataframe
+
+
+def _convert_rows_to_xml(
+    dataframe: pd.DataFrame,
+    max_num_of_props: int
+) -> list[etree._Element]:
+    """
+    Iterate through the rows of the CSV/Excel input file, 
+    convert every row to either a XML resource or an XML property,
+    and return a list of XML resources.
+
+    Args:
+        dataframe: pandas dataframe with the input data
+        max_num_of_props: highest number of properties that a resource in this file has
+    
+    Raises:
+        BaseError: if one of the rows is neither a resource-row nor a property-row, or if the file starts with a property-row
+
+    Returns:
+        a list of XML resources (with their respective properties)
+    """
+    resources: list[etree._Element] = []
+
+    # to start, there is no previous resource
+    resource: Optional[etree._Element] = None
+
+    for index, row in dataframe.iterrows():
+        row_number = int(str(index)) + 2
+        # either the row is a resource-row or a property-row, but not both
+        if check_notna(row["id"]) == check_notna(row["prop name"]):
+            raise BaseError(
+                f"Exactly 1 of the 2 columns 'id' and 'prop name' must be filled. "
+                f"Excel row {row_number} has too many/too less entries:\n"
+                f"id:        '{row['id']}'\n"
+                f"prop name: '{row['prop name']}'"
+            )
+        
+        # this is a resource-row
+        elif check_notna(row["id"]):
+            # the previous resource is finished, a new resource begins: append the previous to the resulting list
+            # in all cases (except for the very first iteration), a previous resource exists
+            if resource is not None:
+                resources.append(resource)
+            resource = _convert_resource_row_to_xml(
+                row_number=row_number,
+                row=row
+            )
+
+        # this is a property-row
+        else:  
+            assert check_notna(row["prop name"])
+            if resource is None:
+                raise BaseError("The first row of your Excel/CSV is invalid. The first row must define a resource, not a property.")
+            prop = _convert_property_row_to_xml(
+                row_number=row_number,
+                row=row,
+                max_num_of_props=max_num_of_props,
+                resource_id=resource.attrib["id"]
+            )
+            resource.append(prop)
+
+    # append the resource of the very last iteration of the for loop
+    if resource is not None:
+        resources.append(resource)
+
+    return resources
+
+
+def _append_bitstream_to_resource(
+    resource: etree._Element,
+    row: pd.Series,
+    row_number: int
+) -> etree._Element:
+    """
+    Create a bitstream-prop element, and append it to the resource.
+    If the file permissions are missing, try to deduce them from the resource permissions.
+
+    Args:
+        resource: the resource element to which the bitstream-prop element should be appended
+        row: the row of the CSV/Excel file from where all information comes from
+        row_number: row number of the CSV/Excel sheet
+
+    Raises:
+        BaseError: if the file permissions are missing and cannot be deduced from the resource permissions
+
+    Returns:
+        the resource element with the appended bitstream-prop element
+    """
+    file_permissions = row.get("file permissions")
+    if not check_notna(file_permissions):
+        resource_permissions = row.get("permissions")
+        if resource_permissions == "res-default":
+            file_permissions = "prop-default"
+        elif resource_permissions == "res-restricted":
+            file_permissions = "prop-restricted"
+        else:
+            raise BaseError(
+                f"Missing file permissions for file '{row['file']}' (Resource ID '{row['id']}', Excel row {row_number}). "
+                f"An attempt to deduce them from the resource permissions failed."
+            )
+    resource.append(
+        make_bitstream_prop(
+            path=str(row["file"]),
+            permissions=str(file_permissions),
+            calling_resource=row["id"]
+        )
+    )
+    return resource
+
+
+def _convert_resource_row_to_xml(
+    row_number: int,
+    row: pd.Series
+) -> etree._Element:
+    """
+    Convert a resource-row to an XML resource element.
+    First, check if the mandatory cells are present.
+    Then, call the appropriate function, depending on the restype (Resource, LinkObj, Annotation, Region).
+
+    Args:
+        row_number: row number of the CSV/Excel sheet
+        row: the pandas series representing the current row
+
+    Raises:
+        BaseError: if a mandatory cell is missing
+
+    Returns:
+        the resource element created from the row
+    """
+    # read and check the mandatory columns
+    resource_id = row["id"]
+    resource_label = row.get("label")
+    if pd.isna([resource_label]):
+        raise BaseError(f"Missing label for resource '{resource_id}' (Excel row {row_number})")
+    if not check_notna(resource_label):
+        warnings.warn(f"The label of resource '{resource_id}' looks suspicious: '{resource_label}' (Excel row {row_number})")
+    resource_restype = row.get("restype")
+    if not check_notna(resource_restype):
+        raise BaseError(f"Missing restype for resource '{resource_id}' (Excel row {row_number})")
+    resource_permissions = row.get("permissions")
+    if not check_notna(resource_permissions):
+        raise BaseError(f"Missing permissions for resource '{resource_id}' (Excel row {row_number})")
+
+    # construct the kwargs for the method call
+    kwargs_resource = {
+        "label": resource_label,
+        "permissions": resource_permissions,
+        "id": resource_id
+    }
+    if check_notna(row.get("ark")):
+        kwargs_resource["ark"] = row["ark"]
+    if check_notna(row.get("iri")):
+        kwargs_resource["iri"] = row["iri"]
+    if check_notna(row.get("ark")) and check_notna(row.get("iri")):
+        warnings.warn(f"Both ARK and IRI were provided for resource '{resource_label}' ({resource_id}). The ARK will override the IRI.")
+    if check_notna(row.get("created")):
+        kwargs_resource["creation_date"] = row["created"]
+    
+    # call the appropriate method
+    if resource_restype == "Region":
+        resource = make_region(**kwargs_resource)
+    elif resource_restype == "Annotation":
+        resource = make_annotation(**kwargs_resource)
+    elif resource_restype == "LinkObj":
+        resource = make_link(**kwargs_resource)
+    else:
+        kwargs_resource["restype"] = resource_restype
+        resource = make_resource(**kwargs_resource)
+        if check_notna(row.get("file")):
+            resource = _append_bitstream_to_resource(
+                resource=resource,
+                row=row,
+                row_number=row_number
+            )
+
+    return resource
+
+
+def _get_prop_function(
+    row: pd.Series,
+    resource_id: str
+) -> Callable[..., etree._Element]:
+    """
+    Return the function that creates the appropriate property, depending on the proptype.
+
+    Args:
+        row: row of the CSV/Excel sheet that defines the property
+        resource_id: resource ID of the resource to which the property belongs
+
+    Raises:
+        BaseError: if the proptype is invalid
+
+    Returns:
+        the function that creates the appropriate property
+    """
+    proptype_2_function: dict[str, Callable[..., etree._Element]] = {
         "bitstream": make_bitstream_prop,
         "boolean-prop": make_boolean_prop,
         "color-prop": make_color_prop,
         "date-prop": make_date_prop,
         "decimal-prop": make_decimal_prop,
         "geometry-prop": make_geometry_prop,
         "geoname-prop": make_geoname_prop,
         "integer-prop": make_integer_prop,
         "interval-prop": make_interval_prop,
         "list-prop": make_list_prop,
         "resptr-prop": make_resptr_prop,
         "text-prop": make_text_prop,
         "uri-prop": make_uri_prop
     }
-    if re.search(r"\.csv$", datafile):
-        # "utf_8_sig": an optional BOM at the start of the file will be skipped
-        # let the "python" engine detect the separator
-        main_df = pd.read_csv(datafile, encoding="utf_8_sig", dtype="str", sep=None, engine="python")
-    elif re.search(r"(\.xls|\.xlsx)$", datafile):
-        main_df = pd.read_excel(datafile, dtype="str")
-    else:
-        raise BaseError("The argument 'datafile' must have one of the extensions 'csv', 'xls', 'xlsx'")
-    # replace NA-like cells by NA
-    main_df = main_df.applymap(
-        lambda x: x if pd.notna(x) and regex.search(r"[\p{L}\d_!?\-]", str(x), flags=regex.U) else pd.NA
+    if row.get("prop type") not in proptype_2_function:
+        raise BaseError(f"Invalid prop type for property {row.get('prop name')} in resource {resource_id}")
+    make_prop_function = proptype_2_function[row["prop type"]]
+    return make_prop_function
+
+
+def _convert_row_to_property_elements(
+    row: pd.Series,
+    max_num_of_props: int,
+    row_number: int,
+    resource_id: str
+) -> list[PropertyElement]:
+    """
+    Every property contains i elements, 
+    which are represented in the Excel as groups of columns named 
+    {i_value, i_encoding, i_permissions, i_comment}. 
+    Depending on the property type, some of these cells are empty.
+    This method converts a row to a list of PropertyElement objects.
+
+    Args:
+        row: the pandas series representing the current row
+        max_num_of_props: highest number of properties that a resource in this file has
+        row_number: row number of the CSV/Excel sheet
+        resource_id: id of resource to which this property belongs to
+
+    Raises:
+        BaseError: if a mandatory cell is missing, or if there are too many/too few values per property
+
+    Returns:
+        list of PropertyElement objects
+    """
+    property_elements: list[PropertyElement] = []
+    for i in range(1, max_num_of_props + 1):
+        value = row[f"{i}_value"]
+        if pd.isna(value):
+            # raise error if other cells of this property element are not empty
+            # if all other cells are empty, continue with next property element
+            other_cell_headers = [f"{i}_{x}" for x in ["encoding", "permissions", "comment"]]
+            notna_cell_headers = [x for x in other_cell_headers if check_notna(row.get(x))]
+            notna_cell_headers_str = ", ".join([f"'{x}'" for x in notna_cell_headers])
+            if notna_cell_headers_str:
+                raise BaseError(
+                    f"Error in resource '{resource_id}': Excel row {row_number} has an entry in column(s) {notna_cell_headers_str}, "
+                    f"but not in '{i}_value'. "
+                    r"Please note that cell contents that don't meet the requirements of the regex [\p{L}\d_!?\-] are considered inexistent."
+                )
+            continue
+        
+        # construct a PropertyElement from this property element
+        kwargs_propelem = {
+            "value": value,
+            "permissions": str(row.get(f"{i}_permissions"))
+        }
+        if not check_notna(row.get(f"{i}_permissions")):
+            raise BaseError(f"Missing permissions in column '{i}_permissions' of property '{row['prop name']}' in resource with id '{resource_id}'")
+        if check_notna(row.get(f"{i}_comment")):
+            kwargs_propelem["comment"] = str(row[f"{i}_comment"])
+        if check_notna(row.get(f"{i}_encoding")):
+            kwargs_propelem["encoding"] = str(row[f"{i}_encoding"])
+        property_elements.append(PropertyElement(**kwargs_propelem))
+
+    # validate the end result before returning it
+    if len(property_elements) == 0:
+        raise BaseError(f"At least one value per property is required, "
+                        f"but resource '{resource_id}' (Excel row {row_number}) doesn't contain any values.")
+    if row.get("prop type") == "boolean-prop" and len(property_elements) != 1:
+        raise BaseError(f"A <boolean-prop> can only have a single value, "
+                        f"but resource '{resource_id}' (Excel row {row_number}) contains more than one value.")
+    
+    return property_elements
+
+
+def _convert_property_row_to_xml(
+    row_number: int,
+    row: pd.Series,
+    max_num_of_props: int,
+    resource_id: str
+) -> etree._Element:
+    """
+    Convert a property-row of the CSV/Excel sheet to an XML element.
+
+    Args:
+        row_number: row number of the CSV/Excel sheet
+        row: the pandas series representing the current row
+        max_num_of_props: highest number of properties that a resource in this file has
+        resource_id: id of the resource to which the property will be appended
+
+    Raises:
+        BaseError: if there is inconsistent data in the row / if a validation fails
+
+    Returns:
+        the resource element with the appended property
+    """
+    # based on the property type, the right function has to be chosen
+    make_prop_function = _get_prop_function(
+        row=row, 
+        resource_id=resource_id
     )
-    # remove empty columns, so that the max_prop_count can be calculated without errors
-    main_df.dropna(axis="columns", how="all", inplace=True)
-    # remove empty rows, to prevent them from being processed and raising an error
-    main_df.dropna(axis="index", how="all", inplace=True)
-    max_prop_count = int(str(list(main_df)[-1]).split("_")[0])
-    root = make_root(shortcode=shortcode, default_ontology=default_ontology)
-    root = append_permissions(root)
-    resource_id: str = ""
 
-    # create all resources
-    # --------------------
-    resource = None
-    for index, row in main_df.iterrows():
-
-        # there are two cases: either the row is a resource-row or a property-row.
-        if not xor(check_notna(row.get("id")), check_notna(row.get("prop name"))):
-            raise BaseError(f"Exactly 1 of the 2 columns 'id' and 'prop name' must have an entry. "
-                            f"Excel row no. {int(str(index)) + 2} has too many/too less entries:\n"
-                            f"id:        '{row.get('id')}'\n"
-                            f"prop name: '{row.get('prop name')}'")
-
-        ########### case resource-row ###########
-        if check_notna(row.get("id")):
-            resource_id = row["id"]
-            resource_permissions = row.get("permissions")
-            if not check_notna(resource_permissions):
-                raise BaseError(f"Missing permissions for resource {resource_id}")
-            resource_label = row.get("label")
-            if not check_notna(resource_label):
-                raise BaseError(f"Missing label for resource {resource_id}")
-            resource_restype = row.get("restype")
-            if not check_notna(resource_restype):
-                raise BaseError(f"Missing restype for resource {resource_id}")
-            if check_notna(row.get("ark")) and check_notna(row.get("iri")):
-                raise BaseError(f"Both ARK and IRI were provided for resource '{resource_label}' ({resource_id}). The ARK will override the IRI.")
-            # previous resource is finished, now a new resource begins. in all cases (except for
-            # the very first iteration), a previous resource exists. if it exists, append it to root.
-            if resource is not None:
-                root.append(resource)
-            kwargs_resource = {
-                "label": resource_label,
-                "permissions": resource_permissions,
-                "id": resource_id
-            }
-            if check_notna(row.get("ark")):
-                kwargs_resource["ark"] = row["ark"]
-            if check_notna(row.get("iri")):
-                kwargs_resource["iri"] = row["iri"]
-            if check_notna(row.get("created")):
-                kwargs_resource["creation_date"] = row["created"]
-            if resource_restype not in ["Annotation", "Region", "LinkObj"]:
-                kwargs_resource["restype"] = resource_restype
-                resource = make_resource(**kwargs_resource)
-                if check_notna(row.get("file")):
-                    file_permissions = row.get("file permissions")
-                    if not check_notna(file_permissions):
-                        if resource_permissions == "res-default":
-                            file_permissions = "prop-default"
-                        elif resource_permissions == "res-restricted":
-                            file_permissions = "prop-restricted"
-                        else:
-                            raise BaseError(f"'file permissions' missing for file '{row['file']}' (Excel row {int(str(index)) + 2}). "
-                                            f"An attempt to deduce them from the resource permissions failed.")
-                    resource.append(make_bitstream_prop(
-                        path=str(row["file"]),
-                        permissions=str(file_permissions),
-                        calling_resource=resource_id
-                    ))
-            elif resource_restype == "Region":
-                resource = make_region(**kwargs_resource)
-            elif resource_restype == "Annotation":
-                resource = make_annotation(**kwargs_resource)
-            elif resource_restype == "LinkObj":
-                resource = make_link(**kwargs_resource)
-
-        ########### case property-row ###########
-        else:  # check_notna(row["prop name"]):
-            # based on the property type, the right function has to be chosen
-            if row.get("prop type") not in proptype_2_function:
-                raise BaseError(f"Invalid prop type for property {row.get('prop name')} in resource {resource_id}")
-            make_prop_function = proptype_2_function[row["prop type"]]
-
-            # every property contains i elements, which are represented in the Excel as groups of
-            # columns named {i_value, i_encoding, i_res ref, i_permissions, i_comment}. Depending
-            # on the property type, some of these items are NA.
-            # Thus, prepare list of PropertyElement objects, with each PropertyElement containing only
-            # the existing items.
-            property_elements: list[PropertyElement] = []
-            for i in range(1, max_prop_count + 1):
-                value = row[f"{i}_value"]
-                if pd.notna(value):
-                    kwargs_propelem = {
-                        "value": value,
-                        "permissions": str(row.get(f"{i}_permissions"))
-                    }
-                    if not check_notna(row.get(f"{i}_permissions")):
-                        raise BaseError(f"Missing permissions for value {value} of property {row['prop name']} in resource {resource_id}")
-                    if check_notna(row.get(f"{i}_comment")):
-                        kwargs_propelem["comment"] = str(row[f"{i}_comment"])
-                    if check_notna(row.get(f"{i}_encoding")):
-                        kwargs_propelem["encoding"] = str(row[f"{i}_encoding"])
-                    property_elements.append(PropertyElement(**kwargs_propelem))
-                elif check_notna(str(row.get(f"{i}_permissions"))):
-                    raise BaseError(
-                        f"Excel row {int(str(index)) + 2} has an entry in column {i}_permissions, but not in {i}_value. "
-                        r"Please note that cell contents that don't meet the requirements of the regex [\p{L}\d_!?\-] are considered inexistent."
-                    )
-
-            # validate property_elements
-            if len(property_elements) == 0:
-                raise BaseError(f"At least one value per property is required, but Excel row {int(str(index)) + 2} doesn't contain any values.")
-            if make_prop_function == make_boolean_prop and len(property_elements) != 1:     # pylint: disable=comparison-with-callable
-                raise BaseError(f"A <boolean-prop> can only have a single value, but Excel row {int(str(index)) + 2} contains more than one value.")
-
-            # create the property and append it to resource
-            kwargs_propfunc: dict[str, Union[str, PropertyElement, list[PropertyElement]]] = {
-                "name": row["prop name"],
-                "calling_resource": resource_id
-            }
-            if make_prop_function == make_boolean_prop:                                     # pylint: disable=comparison-with-callable
-                kwargs_propfunc["value"] = property_elements[0]
-            else:
-                kwargs_propfunc["value"] = property_elements
-            if check_notna(row.get("prop list")):
-                kwargs_propfunc["list_name"] = str(row["prop list"])
+    # convert the row to a list of PropertyElement objects
+    property_elements = _convert_row_to_property_elements(
+        row=row,
+        max_num_of_props=max_num_of_props,
+        row_number=row_number,
+        resource_id=resource_id
+    )
 
-            resource.append(make_prop_function(**kwargs_propfunc))  # type: ignore
+    # create the property
+    prop = _create_property(
+        make_prop_function=make_prop_function,
+        row=row,
+        property_elements=property_elements,
+        resource_id=resource_id
+    )
+    return prop
 
-    # append the resource of the very last iteration of the for loop
-    if resource:
+
+def _create_property(
+    make_prop_function: Callable[..., etree._Element],
+    row: pd.Series,
+    property_elements: list[PropertyElement],
+    resource_id: str
+) -> etree._Element:
+    """
+    Create a property based on the appropriate function and the property elements.
+
+    Args:
+        make_prop_function: the function to create the property
+        row: the pandas series representing the current row of the Excel/CSV
+        property_elements: the list of PropertyElement objects
+        resource_id: id of resource to which this property belongs to
+
+    Returns:
+        the resource with the properties appended
+    """
+    kwargs_propfunc: dict[str, Union[str, PropertyElement, list[PropertyElement]]] = {
+        "name": row["prop name"],
+        "calling_resource": resource_id
+    }
+
+    if row.get("prop type") == "boolean-prop":
+        kwargs_propfunc["value"] = property_elements[0]
+    else:
+        kwargs_propfunc["value"] = property_elements
+    
+    if check_notna(row.get("prop list")):
+        kwargs_propfunc["list_name"] = str(row["prop list"])
+
+    prop = make_prop_function(**kwargs_propfunc)
+
+    return prop
+
+
+def excel2xml(
+    datafile: str, 
+    shortcode: str, 
+    default_ontology: str
+) -> bool:
+    """
+    This is a method that is called from the command line. 
+    It isn't intended to be used in a Python script. 
+    It takes a tabular data source in CSV/XLS(X) format that is formatted according to the specifications, 
+    and transforms it into a DSP-conforming XML file 
+    that can be uploaded to a DSP server with the xmlupload command. 
+    The output file is saved in the same directory as the input file, 
+    with the name [default_ontology]-data.xml.
+
+    Please note that this method doesn't do any data cleaning or data transformation tasks. 
+    The input and the output of this method are semantically exactly equivalent.
+
+    Args:
+        datafile: path to the data file (CSV or XLS(X))
+        shortcode: shortcode of the project that this data belongs to
+        default_ontology: name of the ontology that this data belongs to
+
+    Raises:
+        BaseError if something went wrong
+
+    Returns:
+        True if everything went well, False otherwise
+    """
+    # read and prepare the input file
+    success = True
+    dataframe = _read_cli_input_file(datafile)
+    dataframe = _validate_and_prepare_cli_input_file(dataframe)
+    last_column_title = str(list(dataframe)[-1])    # last column title, in the format "i_comment"
+    max_num_of_props = int(last_column_title.split("_")[0])
+
+    # create the XML root element
+    root = make_root(shortcode=shortcode, default_ontology=default_ontology)
+    root = append_permissions(root)
+
+    # parse the input file row by row
+    resources = _convert_rows_to_xml(
+        dataframe=dataframe,
+        max_num_of_props=max_num_of_props
+    )
+    for resource in resources:
         root.append(resource)
 
     # write file
-    # ----------
     with warnings.catch_warnings(record=True) as w:
         write_xml(root, f"{default_ontology}-data.xml")
         if len(w) > 0:
             success = False
     print(f"XML file successfully created at {default_ontology}-data.xml")
 
     return success
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/process_files.py` & `dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/process_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """This module handles processing of files referenced in the bitstream tags of an XML file."""
 
 import hashlib
 import json
-import logging
 import pickle
 import shutil
 import subprocess
 import uuid
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from pathlib import Path, PurePath
@@ -14,16 +13,17 @@
 
 import docker
 import requests
 from docker.models.containers import Container
 from lxml import etree
 
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.utils.logging import get_logger
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 sipi_container: Optional[Container] = None
 export_moving_image_frames_script: Optional[Path] = None
 
 
 def _get_export_moving_image_frames_script() -> None:
     """
     Downloads the shell script that is used to extract the preview image from a video.
@@ -731,15 +731,14 @@
         output_dir: path to the directory where the transformed / created files should be written to
         xml_file: path to xml file containing the resources
         nthreads: number of threads to use for processing
 
     Returns:
         success status
     """
-    logger.info(f"***Call to process_files(input_dir='{input_dir}', out_dir='{output_dir}', xml_file='{xml_file}')***")
     # check the input parameters
     param_check_result = _check_params(
         input_dir=input_dir,
         out_dir=output_dir,
         xml_file=xml_file
     )
     if param_check_result:
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_files.py` & `dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import glob
-import logging
 import pickle
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 import requests
 from regex import regex
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.shared import login
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 def _get_upload_candidates(
     dir_with_processed_files: Path,
     internal_filename_of_processed_file: Path
 ) -> list[Path]:
     """
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/fast_xmlupload/upload_xml.py` & `dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import logging
 import pickle
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 from lxml import etree
 
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.xml_upload import xml_upload
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 def _get_paths_from_pkl_file(pkl_file: Path) -> dict[str, str]:
     """
     Read the pickle file returned by the processing step.
 
     Args:
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/bitstream.py` & `dsp_tools-2.3.2/src/dsp_tools/models/bitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/connection.py` & `dsp_tools-2.3.2/src/dsp_tools/models/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/exceptions.py` & `dsp_tools-2.3.2/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/group.py` & `dsp_tools-2.3.2/src/dsp_tools/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/helpers.py` & `dsp_tools-2.3.2/src/dsp_tools/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/langstring.py` & `dsp_tools-2.3.2/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/listnode.py` & `dsp_tools-2.3.2/src/dsp_tools/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/ontology.py` & `dsp_tools-2.3.2/src/dsp_tools/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/permission.py` & `dsp_tools-2.3.2/src/dsp_tools/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/project.py` & `dsp_tools-2.3.2/src/dsp_tools/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/projectContext.py` & `dsp_tools-2.3.2/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/propertyclass.py` & `dsp_tools-2.3.2/src/dsp_tools/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/propertyelement.py` & `dsp_tools-2.3.2/src/dsp_tools/models/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/resource.py` & `dsp_tools-2.3.2/src/dsp_tools/models/resource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/resourceclass.py` & `dsp_tools-2.3.2/src/dsp_tools/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/sipi.py` & `dsp_tools-2.3.2/src/dsp_tools/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/user.py` & `dsp_tools-2.3.2/src/dsp_tools/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/value.py` & `dsp_tools-2.3.2/src/dsp_tools/models/value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/xmlallow.py` & `dsp_tools-2.3.2/src/dsp_tools/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-2.3.2/src/dsp_tools/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-2.3.2/src/dsp_tools/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-2.3.2/src/dsp_tools/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/xmlresource.py` & `dsp_tools-2.3.2/src/dsp_tools/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-2.3.2/src/dsp_tools/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.3.2/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-2.3.2/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/schema/project.json` & `dsp_tools-2.3.2/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-2.3.2/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-2.3.2/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-2.3.2/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 
 version: '3.7'
 
 services:
 
   app:
-    image: daschswiss/dsp-app:v10.19.1  # on the verge of every deployment (fortnightly),
+    image: daschswiss/dsp-app:v10.20.1  # on the verge of every deployment (fortnightly),
                                         # take the tag of https://hub.docker.com/r/daschswiss/dsp-app/tags
                                         # that corresponds to the version on https://admin.staging.dasch.swiss/help
                                         # (see also https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json)
     ports:
       - "4200:4200"
     networks:
       - knora-net
@@ -23,15 +23,15 @@
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   sipi:
-    image: daschswiss/knora-sipi:28.2.0  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
+    image: daschswiss/knora-sipi:28.3.0  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
     ports:
       - "1024:1024"
     volumes:
       - .:/docker
     networks:
       - knora-net
     environment:
@@ -42,15 +42,15 @@
       - SIPI_WEBAPI_HOSTNAME=api
       - SIPI_WEBAPI_PORT=3333
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/docker/sipi.docker-config.lua
 
   api:
-    image: daschswiss/knora-api:28.2.0  # on the verge of every deployment (fortnightly),
+    image: daschswiss/knora-api:28.3.0  # on the verge of every deployment (fortnightly),
                                         # take the tag of https://hub.docker.com/r/daschswiss/knora-api/tags
                                         # that corresponds to the version on https://admin.staging.dasch.swiss/help
                                         # (see also https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json)
     depends_on:
       - sipi
       - db
     ports:
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/id_to_iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/project_create.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/project_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """This module handles the ontology creation, update and upload to a DSP server. This includes the creation and update
 of the project, the creation of groups, users, lists, resource classes, properties and cardinalities."""
-import logging
 import re
 from pathlib import Path
 from typing import Any, Union, cast
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.group import Group
@@ -12,19 +11,20 @@
 from dsp_tools.models.langstring import LangString
 from dsp_tools.models.ontology import Ontology
 from dsp_tools.models.project import Project
 from dsp_tools.models.propertyclass import PropertyClass
 from dsp_tools.models.resourceclass import ResourceClass
 from dsp_tools.models.user import User
 from dsp_tools.utils.excel_to_json_lists import expand_lists_from_excel
+from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.project_create_lists import create_lists_on_server
 from dsp_tools.utils.project_validate import validate_project
 from dsp_tools.utils.shared import login, parse_json_input, try_network_action
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 def _create_project_on_server(
     project_definition: dict[str, Any],
     con: Connection,
     verbose: bool
 ) -> tuple[Project, bool]:
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/project_create_lists.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import logging
 from typing import Any, Optional, Union
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.project import Project
 from dsp_tools.utils.excel_to_json_lists import expand_lists_from_excel
+from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.project_validate import validate_project
 from dsp_tools.utils.shared import login, parse_json_input, try_network_action
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 def _create_list_node(
     con: Connection,
     project: Project,
     node: dict[str, Any],
     parent_node: Optional[ListNode] = None
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/project_get.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/project_get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/project_validate.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/rosetta.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/shared.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import copy
 import importlib.resources
 import json
-import logging
 import time
 import unicodedata
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Callable, Optional, Union
 
 import pandas as pd
 import regex
 from lxml import etree
 from requests import RequestException
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.propertyelement import PropertyElement
+from dsp_tools.utils.logging import get_logger
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 def login(server: str, user: str, password: str) -> Connection:
     """
     Creates a connection, 
     makes a login (handling temporary network interruptions),
     and returns the active connection.
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/stack_handling.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/stack_handling.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     docker_path_of_distribution = importlib.resources.files("dsp_tools").joinpath("resources/start-stack")
     for file in docker_path_of_distribution.iterdir():
         with importlib.resources.as_file(file) as f:
             file_path = Path(f)
         shutil.copy(file_path, docker_path_of_user / file.name)
 
     # get sipi.docker-config.lua
-    commit_of_used_api_version = "d6bae7ff5e6b6a635982c14f21ca4e69e298a312"      # gitleaks:allow
+    commit_of_used_api_version = "783428ebc84d974b82452e3d7358b946ae40588c"      # gitleaks:allow
     url_prefix = f"https://github.com/dasch-swiss/dsp-api/raw/{commit_of_used_api_version}/"
     docker_config_lua_text = requests.get(f"{url_prefix}sipi/config/sipi.docker-config.lua", timeout=5).text
     if max_file_size:
         max_post_size_regex = r"max_post_size ?= ?[\'\"]\d+M[\'\"]"
         if not re.search(max_post_size_regex, docker_config_lua_text):
             raise BaseError("Unable to set max_file_size. Please try again without this flag.")
         docker_config_lua_text = re.sub(max_post_size_regex, f"max_post_size = '{max_file_size}M'", docker_config_lua_text)
```

### Comparing `dsp_tools-2.3.1/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-2.3.2/src/dsp_tools/utils/xml_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module handles the import of XML data into the DSP platform.
 """
 from __future__ import annotations
 
 import base64
 import copy
 import json
-import logging
 import os
 import re
 import sys
 import uuid
 from collections import namedtuple
 from datetime import datetime
 from pathlib import Path
@@ -30,23 +29,24 @@
     ResourceInstanceFactory
 )
 from dsp_tools.models.sipi import Sipi
 from dsp_tools.models.value import KnoraStandoffXml
 from dsp_tools.models.xmlpermission import XmlPermission
 from dsp_tools.models.xmlproperty import XMLProperty
 from dsp_tools.models.xmlresource import XMLResource
+from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.shared import (
     login,
     try_network_action,
     validate_xml_against_schema
 )
 
 MetricRecord = namedtuple("MetricRecord", ["res_id", "filetype", "filesize_mb", "event", "duration_ms", "mb_per_sec"])
 
-logger = logging.getLogger(__name__)
+logger = get_logger(__name__)
 
 
 def _transform_server_url_to_foldername(server: str) -> str:
     """
     Take the server URL and transform it so that it can be used as foldername.
 
     Args:
@@ -470,18 +470,14 @@
         BaseError or UserError in case of permanent network or software failure
         UserError if the XML file is invalid
 
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
-
-    logger.info(f"Method call xml_upload(input_file='{input_file}', server='{server}', user='{user}', imgdir='{imgdir}', sipi='{sipi}', "
-                f"verbose={verbose}, incremental={incremental}, save_metrics={save_metrics}, preprocessing_done={preprocessing_done})")
-
     # parse the XML file
     validate_xml_against_schema(input_file=input_file)
     root = _parse_xml_file(input_file=input_file)
     shortcode = root.attrib['shortcode']
     default_ontology = root.attrib['default-ontology']
     logger.info(f"Validated and parsed the XML file. Shortcode='{shortcode}' and default_ontology='{default_ontology}'")
```

### Comparing `dsp_tools-2.3.1/PKG-INFO` & `dsp_tools-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.3.1
+Version: 2.3.2
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

