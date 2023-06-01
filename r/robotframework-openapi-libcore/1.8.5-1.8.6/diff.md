# Comparing `tmp/robotframework_openapi_libcore-1.8.5.tar.gz` & `tmp/robotframework_openapi_libcore-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapi_libcore-1.8.5.tar", max compression
+gzip compressed data, was "robotframework_openapi_libcore-1.8.6.tar", max compression
```

## Comparing `robotframework_openapi_libcore-1.8.5.tar` & `robotframework_openapi_libcore-1.8.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4693 2023-04-20 08:42:44.492938 robotframework_openapi_libcore-1.8.5/docs/README.md
--rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.8.5/LICENSE
--rw-r--r--   0        0        0     2345 2023-04-20 08:33:33.956737 robotframework_openapi_libcore-1.8.5/pyproject.toml
--rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/__init__.py
--rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_base.py
--rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_utils.py
--rw-r--r--   0        0        0      163 2023-04-20 07:55:08.986947 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/oas_cache.py
--rw-r--r--   0        0        0    24298 2023-04-20 08:42:44.415026 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.libspec
--rw-r--r--   0        0        0    59158 2023-04-20 08:42:16.575425 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.py
--rw-r--r--   0        0        0    14713 2023-02-17 14:58:53.548382 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/value_utils.py
--rw-r--r--   0        0        0     5656 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.5/setup.py
--rw-r--r--   0        0        0     5867 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     4693 2023-06-01 13:47:36.261686 robotframework_openapi_libcore-1.8.6/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.8.6/LICENSE
+-rw-r--r--   0        0        0     2372 2023-06-01 13:27:50.821095 robotframework_openapi_libcore-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/__init__.py
+-rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_base.py
+-rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_utils.py
+-rw-r--r--   0        0        0      163 2023-04-20 07:55:08.986947 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/oas_cache.py
+-rw-r--r--   0        0        0    26880 2023-06-01 13:47:36.184561 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.libspec
+-rw-r--r--   0        0        0    59161 2023-06-01 13:47:32.907232 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.py
+-rw-r--r--   0        0        0    14791 2023-06-01 13:47:32.926184 robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/value_utils.py
+-rw-r--r--   0        0        0     5656 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.6/setup.py
+-rw-r--r--   0        0        0     5867 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.6/PKG-INFO
```

### Comparing `robotframework_openapi_libcore-1.8.5/docs/README.md` & `robotframework_openapi_libcore-1.8.6/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.5/LICENSE` & `robotframework_openapi_libcore-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.5/pyproject.toml` & `robotframework_openapi_libcore-1.8.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapi-libcore"
-version = "1.8.5"
+version = "1.8.6"
 description = "A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs."
 license = "Apache-2.0"
 authors = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 maintainers = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 readme =  "./docs/README.md"
 homepage = "https://github.com/MarketSquare/robotframework-openapi-libcore"
 classifiers = [
@@ -57,14 +57,15 @@
 exclude_lines = [
     "pragma: no cover",
     "@abstract"
 ]
 
 [tool.mypy]
 show_error_codes = true
+check_untyped_defs = true
 plugins = "pydantic.mypy"
 
 [[tool.mypy.overrides]]
 module = [
     "prance.*",
     "robot.*",
     "openapi_core.*",
```

### Comparing `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/__init__.py` & `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_base.py` & `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_base.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 4% similar despite different names*

#### Comparing `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-04-20T08:42:44+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="380">
-  <version>1.8.5</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-06-01T13:47:36+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="379">
+  <version>1.8.6</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
-    <init name="__init__" lineno="388">
+    <init name="__init__" lineno="387">
       <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, extra_headers: Dict[str, str] | None = None, invalid_property_default_response: int = 422, recursion_limit: int = 1, recursion_default: Any = {}, faker_locale: str | List[str] | None = None, default_id_property_name: str = id">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
           <name>source</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="origin: str = ">
           <name>origin</name>
@@ -120,16 +120,16 @@
 &lt;h4&gt;default_id_property_name&lt;/h4&gt;
 &lt;p&gt;The default name for the property that identifies a resource (i.e. a unique entiry) within the API. The default value for this property name is &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt;. If the target API uses a different name for all the resources within the API, you can configure it globally using this property.&lt;/p&gt;
 &lt;p&gt;If different property names are used for the unique identifier for different types of resources, an &lt;span class=&quot;name&quot;&gt;ID_MAPPING&lt;/span&gt; can be implemented in the &lt;span class=&quot;name&quot;&gt;mappings_path&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>=== source === An absolute path to an openapi.json or openapi.yaml file or an url to such a file.</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1360">
-      <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Any] | None = None">
+    <kw name="Authorized Request" lineno="1359">
+      <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
@@ -142,50 +142,55 @@
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="headers: Dict[str, str] | None = None">
           <name>headers</name>
           <type typedoc="dictionary">Dict[str, str]</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
-        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="json_data: Dict[str, Any] | None = None">
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
           <name>json_data</name>
-          <type typedoc="dictionary">Dict[str, Any]</type>
+          <type typedoc="dictionary">Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None]</type>
+          <type typedoc="list">List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None]</type>
+          <type typedoc="string">str</type>
+          <type typedoc="integer">int</type>
+          <type typedoc="float">float</type>
+          <type typedoc="boolean">bool</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1264">
+    <kw name="Ensure In Use" lineno="1263">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type>IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="699">
+    <kw name="Get Ids From Url" lineno="698">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1043">
+    <kw name="Get Invalid Json Data" lineno="1042">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -200,40 +205,40 @@
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1091">
+    <kw name="Get Invalidated Parameters" lineno="1090">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1009">
+    <kw name="Get Invalidated Url" lineno="1008">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="919">
+    <kw name="Get Json Data For Dto Class" lineno="918">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type typedoc="dictionary">Dict[str, Any]</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="dto_class: Dto | Type[Dto]">
           <name>dto_class</name>
@@ -245,15 +250,15 @@
           <type typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1308">
+    <kw name="Get Json Data With Conflict" lineno="1307">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -267,54 +272,54 @@
           <name>conflict_status_code</name>
           <type typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1031">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1030">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="739">
+    <kw name="Get Request Data" lineno="738">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an object with valid request data for body, headers and query params.&lt;/p&gt;</doc>
       <shortdoc>Return an object with valid request data for body, headers and query params.</shortdoc>
     </kw>
-    <kw name="Get Valid Id For Endpoint" lineno="611">
+    <kw name="Get Valid Id For Endpoint" lineno="610">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Support keyword that returns the &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; for an existing resource at &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;To prevent resource conflicts with other test cases, a new resource is created (POST) if possible.&lt;/p&gt;</doc>
       <shortdoc>Support keyword that returns the `id` for an existing resource at `endpoint`.</shortdoc>
     </kw>
-    <kw name="Get Valid Url" lineno="571">
+    <kw name="Get Valid Url" lineno="570">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -325,39 +330,65 @@
 &lt;p&gt;If the &lt;span class=&quot;name&quot;&gt;endpoint&lt;/span&gt; contains path parameters the Get Valid Id For Endpoint keyword will be executed to retrieve valid ids for the path parameters.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: if valid ids cannot be retrieved within the scope of the API, the &lt;span class=&quot;name&quot;&gt;PathPropertiesConstraint&lt;/span&gt; Relation can be used. More information can be found &lt;a href=&quot;https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html&quot;&gt;here&lt;/a&gt;.&lt;/p&gt;</doc>
       <shortdoc>This keyword returns a valid url for the given `endpoint` and `method`.</shortdoc>
     </kw>
   </keywords>
   <datatypes/>
   <typedocs>
+    <type name="boolean" type="Standard">
+      <doc>&lt;p&gt;Strings &lt;code&gt;TRUE&lt;/code&gt;, &lt;code&gt;YES&lt;/code&gt;, &lt;code&gt;ON&lt;/code&gt; and &lt;code&gt;1&lt;/code&gt; are converted to Boolean &lt;code&gt;True&lt;/code&gt;, the empty string as well as strings &lt;code&gt;FALSE&lt;/code&gt;, &lt;code&gt;NO&lt;/code&gt;, &lt;code&gt;OFF&lt;/code&gt; and &lt;code&gt;0&lt;/code&gt; are converted to Boolean &lt;code&gt;False&lt;/code&gt;, and the string &lt;code&gt;NONE&lt;/code&gt; is converted to the Python &lt;code&gt;None&lt;/code&gt; object. Other strings and other accepted values are passed as-is, allowing keywords to handle them specially if needed. All string comparisons are case-insensitive.&lt;/p&gt;
+&lt;p&gt;Examples: &lt;code&gt;TRUE&lt;/code&gt; (converted to &lt;code&gt;True&lt;/code&gt;), &lt;code&gt;off&lt;/code&gt; (converted to &lt;code&gt;False&lt;/code&gt;), &lt;code&gt;example&lt;/code&gt; (used as-is)&lt;/p&gt;</doc>
+      <accepts>
+        <type>string</type>
+        <type>integer</type>
+        <type>float</type>
+        <type>None</type>
+      </accepts>
+      <usages>
+        <usage>Authorized Request</usage>
+      </usages>
+    </type>
     <type name="dictionary" type="Standard">
       <doc>&lt;p&gt;Strings must be Python &lt;a href=&quot;https://docs.python.org/library/stdtypes.html#dict&quot;&gt;dictionary&lt;/a&gt; literals. They are converted to actual dictionaries using the &lt;a href=&quot;https://docs.python.org/library/ast.html#ast.literal_eval&quot;&gt;ast.literal_eval&lt;/a&gt; function. They can contain any values &lt;code&gt;ast.literal_eval&lt;/code&gt; supports, including dictionaries and other containers.&lt;/p&gt;
 &lt;p&gt;If the type has nested types like &lt;code&gt;dict[str, int]&lt;/code&gt;, items are converted to those types automatically. This in new in Robot Framework 6.0.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;{'a': 1, 'b': 2}&lt;/code&gt;, &lt;code&gt;{'key': 1, 'nested': {'key': 2}}&lt;/code&gt;&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
         <type>Mapping</type>
       </accepts>
       <usages>
         <usage>__init__</usage>
         <usage>Authorized Request</usage>
         <usage>Get Json Data For Dto Class</usage>
       </usages>
     </type>
+    <type name="float" type="Standard">
+      <doc>&lt;p&gt;Conversion is done using Python's &lt;a href=&quot;https://docs.python.org/library/functions.html#float&quot;&gt;float&lt;/a&gt; built-in function.&lt;/p&gt;
+&lt;p&gt;Starting from RF 4.1, spaces and underscores can be used as visual separators for digit grouping purposes.&lt;/p&gt;
+&lt;p&gt;Examples: &lt;code&gt;3.14&lt;/code&gt;, &lt;code&gt;2.9979e8&lt;/code&gt;, &lt;code&gt;10 000.000 01&lt;/code&gt;&lt;/p&gt;</doc>
+      <accepts>
+        <type>string</type>
+        <type>Real</type>
+      </accepts>
+      <usages>
+        <usage>Authorized Request</usage>
+      </usages>
+    </type>
     <type name="integer" type="Standard">
       <doc>&lt;p&gt;Conversion is done using Python's &lt;a href=&quot;https://docs.python.org/library/functions.html#int&quot;&gt;int&lt;/a&gt; built-in function. Floating point numbers are accepted only if they can be represented as integers exactly. For example, &lt;code&gt;1.0&lt;/code&gt; is accepted and &lt;code&gt;1.1&lt;/code&gt; is not.&lt;/p&gt;
 &lt;p&gt;Starting from RF 4.1, it is possible to use hexadecimal, octal and binary numbers by prefixing values with &lt;code&gt;0x&lt;/code&gt;, &lt;code&gt;0o&lt;/code&gt; and &lt;code&gt;0b&lt;/code&gt;, respectively.&lt;/p&gt;
 &lt;p&gt;Starting from RF 4.1, spaces and underscores can be used as visual separators for digit grouping purposes.&lt;/p&gt;
 &lt;p&gt;Examples: &lt;code&gt;42&lt;/code&gt;, &lt;code&gt;-1&lt;/code&gt;, &lt;code&gt;0b1010&lt;/code&gt;, &lt;code&gt;10 000 000&lt;/code&gt;, &lt;code&gt;0xBAD_C0FFEE&lt;/code&gt;&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
         <type>float</type>
       </accepts>
       <usages>
         <usage>__init__</usage>
+        <usage>Authorized Request</usage>
         <usage>Get Invalid Json Data</usage>
         <usage>Get Invalidated Parameters</usage>
         <usage>Get Json Data With Conflict</usage>
       </usages>
     </type>
     <type name="list" type="Standard">
       <doc>&lt;p&gt;Strings must be Python &lt;a href=&quot;https://docs.python.org/library/stdtypes.html#list&quot;&gt;list&lt;/a&gt; literals. They are converted to actual lists using the &lt;a href=&quot;https://docs.python.org/library/ast.html#ast.literal_eval&quot;&gt;ast.literal_eval&lt;/a&gt; function. They can contain any values &lt;code&gt;ast.literal_eval&lt;/code&gt; supports, including lists and other containers.&lt;/p&gt;
@@ -365,14 +396,15 @@
 &lt;p&gt;Examples: &lt;code&gt;['one', 'two']&lt;/code&gt;, &lt;code&gt;[('one', 1), ('two', 2)]&lt;/code&gt;&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
         <type>Sequence</type>
       </accepts>
       <usages>
         <usage>__init__</usage>
+        <usage>Authorized Request</usage>
       </usages>
     </type>
     <type name="None" type="Standard">
       <doc>&lt;p&gt;String &lt;code&gt;NONE&lt;/code&gt; (case-insensitive) is converted to Python &lt;code&gt;None&lt;/code&gt; object. Other values cause an error.&lt;/p&gt;</doc>
       <accepts>
         <type>string</type>
       </accepts>
```

### Comparing `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,19 +157,18 @@
 from OpenApiLibCore.dto_utils import (
     DEFAULT_ID_PROPERTY_NAME,
     DefaultDto,
     get_dto_class,
     get_id_property_name,
 )
 from OpenApiLibCore.oas_cache import PARSER_CACHE
-from OpenApiLibCore.value_utils import FAKE, IGNORE
+from OpenApiLibCore.value_utils import FAKE, IGNORE, JSON
 
 run_keyword = BuiltIn().run_keyword
 
-
 logger = getLogger(__name__)
 
 
 def resolve_schema(schema: Dict[str, Any]) -> Dict[str, Any]:
     """Helper method to resolve allOf, anyOf and oneOf instances in a schema."""
     # schema is mutable, so deepcopy to prevent mutation of original schema argument
     resolved_schema: Dict[str, Any] = deepcopy(schema)
@@ -706,15 +705,15 @@
         response = run_keyword(
             "authorized_request",
             url,
             "get",
             request_data.get_required_params(),
             request_data.get_required_headers(),
         )
-        assert response.ok
+        response.raise_for_status()
         response_data: Union[Dict[str, Any], List[Dict[str, Any]]] = response.json()
 
         # determine the property name to use
         mapping = self.get_id_property_name(endpoint=endpoint)
         if isinstance(mapping, str):
             id_property = mapping
         else:
@@ -1359,15 +1358,15 @@
     @keyword
     def authorized_request(  # pylint: disable=too-many-arguments
         self,
         url: str,
         method: str,
         params: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
-        json_data: Optional[Dict[str, Any]] = None,
+        json_data: Optional[JSON] = None,
     ) -> Response:
         """
         Perform a request using the security token or authentication set in the library.
 
         > Note: provided username / password or auth objects take precedence over token
             based security
         """
```

### Comparing `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/value_utils.py` & `robotframework_openapi_libcore-1.8.6/src/OpenApiLibCore/value_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from logging import getLogger
 from random import choice, randint, uniform
 from typing import Any, Dict, List, Optional, Union
 
 import faker
 import rstr
 
+JSON = Union[Dict[str, "JSON"], List["JSON"], str, int, float, bool, None]
+
 logger = getLogger(__name__)
 
 IGNORE = object()
 
 
 class LocalizedFaker:
     """Class to support setting a locale post-init."""
```

### Comparing `robotframework_openapi_libcore-1.8.5/setup.py` & `robotframework_openapi_libcore-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prance[cli]>=0.22,<0.23',
  'requests>=2.27,<3.0',
  'robotframework>=4',
  'rstr>=3,<4']
 
 setup_kwargs = {
     'name': 'robotframework-openapi-libcore',
-    'version': '1.8.5',
+    'version': '1.8.6',
     'description': 'A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.',
     'long_description': '---\n---\n\n# OpenApiLibCore for Robot Framework\n\nThe OpenApiLibCore library is a utility library that is meant to simplify creation\nof other Robot Framework libraries for API testing based on the information in\nan OpenAPI document (also known as Swagger document).\nThis document explains how to use the OpenApiLibCore library.\n\nMy RoboCon 2022 talk about OpenApiDriver and OpenApiLibCore can be found\n[here](https://www.youtube.com/watch?v=7YWZEHxk9Ps)\n\nFor more information about Robot Framework, see http://robotframework.org.\n\n---\n\n> Note: OpenApiLibCore is still being developed so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapi-libcore`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiLibCore implements a number of Robot Framework keywords that make it\neasy to interact with an OpenAPI implementation by using the information in the\nopenapi document (Swagger file), for examply by automatic generation of valid values\nfor requests based on the schema information in the document.\n\n> Note: OpenApiLibCore is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use the keywords exposed by OpenApiLibCore on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiLibCore.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the API to not use recursion is recommended.\nAt present OpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source`, `origin` and \'endpoint\' altered to\nfit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiLibCore\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\n\n*** Test Cases ***\nGetting Started\n    ${url}=    Get Valid Url    endpoint=/employees/{employee_id}   method=get\n\n```\n\nRunning the above suite for the first time may result in an error / failed test.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiLibCore library parameters and keywords that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/openapi_libcore.html).\n\nThe OpenApiLibCore also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-endpoint authorization levels.\n- Parsing of OAS 3.1 documents is supported by the parsing tools, but runtime behavior is untested.\n\n',
     'author': 'Robin Mackaij',
     'author_email': 'r.a.mackaij@gmail.com',
     'maintainer': 'Robin Mackaij',
     'maintainer_email': 'r.a.mackaij@gmail.com',
     'url': 'https://github.com/MarketSquare/robotframework-openapi-libcore',
```

### Comparing `robotframework_openapi_libcore-1.8.5/PKG-INFO` & `robotframework_openapi_libcore-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapi-libcore
-Version: 1.8.5
+Version: 1.8.6
 Summary: A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.
 Home-page: https://github.com/MarketSquare/robotframework-openapi-libcore
 License: Apache-2.0
 Author: Robin Mackaij
 Author-email: r.a.mackaij@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
```

