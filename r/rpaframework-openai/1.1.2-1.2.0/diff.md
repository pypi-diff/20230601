# Comparing `tmp/rpaframework_openai-1.1.2.tar.gz` & `tmp/rpaframework_openai-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_openai-1.1.2.tar", max compression
+gzip compressed data, was "rpaframework_openai-1.2.0.tar", max compression
```

## Comparing `rpaframework_openai-1.1.2.tar` & `rpaframework_openai-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2023-02-07 05:36:00.877190 rpaframework_openai-1.1.2/LICENSE
--rw-r--r--   0        0        0      155 2023-02-07 05:36:00.877389 rpaframework_openai-1.1.2/README.rst
--rw-r--r--   0        0        0    15680 2023-03-14 10:43:57.530769 rpaframework_openai-1.1.2/RPA_OpenAI.libspec
--rw-r--r--   0        0        0     1830 2023-03-14 10:18:53.156313 rpaframework_openai-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    11718 2023-03-08 07:24:21.296490 rpaframework_openai-1.1.2/src/RPA/OpenAI.py
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 rpaframework_openai-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11560 2023-03-06 14:03:56.127418 rpaframework_openai-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1898 2023-06-01 16:44:30.466236 rpaframework_openai-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-03-06 14:03:56.127418 rpaframework_openai-1.2.0/README.rst
+-rw-r--r--   0        0        0    18717 2023-06-01 16:46:59.196696 rpaframework_openai-1.2.0/RPA_OpenAI.libspec
+-rw-r--r--   0        0        0    14920 2023-06-01 16:44:30.467236 rpaframework_openai-1.2.0/src/RPA/OpenAI.py
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 rpaframework_openai-1.2.0/PKG-INFO
```

### Comparing `rpaframework_openai-1.1.2/LICENSE` & `rpaframework_openai-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2020 Robocorp Technologies, Inc.
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2020 Robocorp Technologies, Inc.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `rpaframework_openai-1.1.2/RPA_OpenAI.libspec` & `rpaframework_openai-1.2.0/RPA_OpenAI.libspec`

 * *Files 23% similar despite different names*

#### Comparing `rpaframework_openai-1.1.2/RPA_OpenAI.libspec` & `rpaframework_openai-1.2.0/RPA_OpenAI.libspec`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="RPA.OpenAI" type="LIBRARY" format="REST" scope="GLOBAL" generated="2023-03-14T10:43:57Z" specversion="4" source="./RPA/OpenAI.py" lineno="7">
+<keywordspec name="RPA.OpenAI" type="LIBRARY" format="REST" scope="GLOBAL" generated="2023-06-01T16:46:59Z" specversion="4" source="./RPA/OpenAI.py" lineno="7">
   <version/>
-  <doc>Library to support `OpenAI &lt;https://openai.com&gt;`_ service.
+  <doc>Library to support `OpenAI &lt;https://openai.com&gt;`_ and `Azure OpenAI &lt;https://learn.microsoft.com/en-us/azure/cognitive-services/openai/overview&gt;`_ services.
 
 Library is **not** included in the `rpaframework` package, so in order to use it
 you have to add `rpaframework-openai` with the desired version in your
 *conda.yaml* file.
 
 **Robot Framework example usage**
 
@@ -39,15 +39,70 @@
         Create a tagline for icecream shop',
         temperature=0.6,
     )
     print(result)</doc>
   <tags/>
   <inits/>
   <keywords>
-    <kw name="Authorize To Openai" lineno="56">
+    <kw name="Authorize To Azure Openai" lineno="57">
+      <arguments repr="api_key: str, api_base: str, api_type: str | None = azure, api_version: str | None = 2023-05-15">
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="api_key: str">
+          <name>api_key</name>
+          <type typedoc="string">str</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="true" repr="api_base: str">
+          <name>api_base</name>
+          <type typedoc="string">str</type>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="api_type: str | None = azure">
+          <name>api_type</name>
+          <type typedoc="string">str</type>
+          <type typedoc="None">None</type>
+          <default>azure</default>
+        </arg>
+        <arg kind="POSITIONAL_OR_NAMED" required="false" repr="api_version: str | None = 2023-05-15">
+          <name>api_version</name>
+          <type typedoc="string">str</type>
+          <type typedoc="None">None</type>
+          <default>2023-05-15</default>
+        </arg>
+      </arguments>
+      <doc>Keyword for authorize to Azure OpenAI.
+
+:param api_key: Your Azure OpenAI API key
+:param api_base: Your Endpoint URL. Example: https://docs-test-001.openai.azure.com/
+:param api_type: &quot;azure&quot;
+:param api_version: &quot;2023-05-15&quot;
+
+Robot Framework example:
+
+.. code-block:: robotframework
+
+    ${secrets}   Get Secret   secret_name=AzureOpenAI
+    Authorize To Azure Openai
+    ...    api_key=${secrets}[api_key]
+    ...    api_base=${secrets}[api_base]
+    ...    api_type=azure
+    ...    api_version=2023-05-15
+
+Python example:
+
+.. code-block:: python
+
+    secrets = Vault().get_secret(&quot;AzureOpenAI&quot;)
+    baselib = OpenAI()
+    baselib.authorize_to_azure_openai(
+        secrets[&quot;api_key&quot;],
+        secrets[&quot;api_base&quot;],
+        &quot;azure&quot;,
+        &quot;2023-05-15&quot;
+    )</doc>
+      <shortdoc>Keyword for authorize to Azure OpenAI.</shortdoc>
+    </kw>
+    <kw name="Authorize To Openai" lineno="103">
       <arguments repr="api_key: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="api_key: str">
           <name>api_key</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>Keyword for authorize to OpenAI with your API key obtained from your account.
@@ -66,15 +121,15 @@
 .. code-block:: python
 
     secrets = Vault().get_secret(&quot;OpenAI&quot;)
     baselib = OpenAI()
     baselib.authorize_to_openai(secrets[&quot;key&quot;])</doc>
       <shortdoc>Keyword for authorize to OpenAI with your API key obtained from your account.</shortdoc>
     </kw>
-    <kw name="Chat Completion Create" lineno="147">
+    <kw name="Chat Completion Create" lineno="202">
       <arguments repr="user_content: str | None = None, conversation: List | None = None, model: str | None = gpt-3.5-turbo, system_content: str | None = None, temperature: int | None = 1, top_probability: int | None = 1, frequency_penalty: int | None = 0, presence_penalty: int | None = 0">
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="user_content: str | None = None">
           <name>user_content</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>None</default>
         </arg>
@@ -117,22 +172,26 @@
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="presence_penalty: int | None = 0">
           <name>presence_penalty</name>
           <type typedoc="integer">int</type>
           <type typedoc="None">None</type>
           <default>0</default>
         </arg>
       </arguments>
-      <doc>Keyword for creating ChatGPT text completions in OpenAI. Keyword returns a
-list containing the response as a string and the message history as a list.
+      <doc>Keyword for creating ChatGPT text completions using OpenAI or Azure OpenAI.
+Keyword returns the response as a string and the message history as a list.
+
+**Note**. When using ``Azure OpenAI`` you must provide the ``deployment_name``
+as the ``model`` parameter instead of the model ID used with ``OpenAI``.
 
 :param user_content: Text submitted to ChatGPT to generate completions.
 :param conversation: List containing the conversation to be continued. Leave
  empty for a new conversation.
-:param model: ID of the model to use. Currently, only gpt-3.5-turbo and
- gpt-3.5-turbo-0301 are supported.
+:param model: For ``OpenAI`` the ID of the model to use, e.g. ``gpt-4``
+ or ``gpt-3.5-turbo``. For ``Azure OpenAI`` the Deployment name,
+ e.g. ``myGPT4deployment``.
 :param system_content: The system message helps set the behavior of
  the assistant.
 :param temperature: What sampling temperature to use between 0 to 2. Higher
  values means the model will take more risks.
 :param top_probability: An alternative to sampling with temperature, called
  nucleus sampling, where the model considers the results of the tokens with
  top_p probability mass.
@@ -141,27 +200,27 @@
 :param presence_penalty: Number between -2.0 and 2.0. Positive values penalize
  new tokens based on whether they appear in the text so far.
 
 Robot Framework example:
 
 .. code-block:: robotframework
 
-    # Create a new conversation without conversation history.
+    # Get response without conversation history.
     ${response}   @{chatgpt_conversation}=     Chat Completion Create
     ...    user_content=What is the biggest mammal?
     Log    ${response}
 
     # Continue the conversation by using the &quot;conversation&quot; argument.
     ${response}   @{chatgpt_conversation}=     Chat Completion Create
     ...    conversation=${chatgpt_conversation}
     ...    user_content=How old can it live?
     Log    ${response}</doc>
-      <shortdoc>Keyword for creating ChatGPT text completions in OpenAI. Keyword returns a list containing the response as a string and the message history as a list.</shortdoc>
+      <shortdoc>Keyword for creating ChatGPT text completions using OpenAI or Azure OpenAI. Keyword returns the response as a string and the message history as a list.</shortdoc>
     </kw>
-    <kw name="Completion Create" lineno="80">
+    <kw name="Completion Create" lineno="127">
       <arguments repr="prompt: str, model: str | None = text-davinci-003, temperature: int | None = 0.7, max_tokens: int | None = 256, top_probability: int | None = 1, frequency_penalty: int | None = 0, presence_penalty: int | None = 0, result_format: str | None = string">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="prompt: str">
           <name>prompt</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="model: str | None = text-davinci-003">
           <name>model</name>
@@ -202,19 +261,23 @@
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="result_format: str | None = string">
           <name>result_format</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>string</default>
         </arg>
       </arguments>
-      <doc>Keyword for creating text completions in OpenAI.
+      <doc>Keyword for creating text completions in OpenAI and Azure OpenAI.
 Keyword returns a text string.
 
+**Note**. When using ``Azure OpenAI`` you must provide the ``deployment_name``
+as the ``model`` parameter instead of the model ID used with ``OpenAI``.
+
 :param prompt: Text submitted to OpenAI for creating natural language.
-:param model: OpenAI's model to use in the completion.
+:param model: For ``OpenAI`` the ID of the model to use, e.g. ``text-davinci-003``.
+ For ``Azure OpenAI`` the Deployment name, e.g. ``myDavinci3deployment``.
 :param temperature: What sampling temperature to use.
     Higher values means the model will take more risks..
 :param max_tokens: The maximum number of tokens to generate in the completion..
 :param top_probability: Controls diversity via nucleus sampling. 0.5 means half
     of all likelihood-weighted options are considered.
 :param frequency_penalty: Number between -2.0 and 2.0. Positive values penalize
     new tokens based on their existing frequency in the text so far.
@@ -237,17 +300,17 @@
 .. code-block:: python
 
     result = baselib.completion_create(
         'Create a tagline for icecream shop',
         temperature=0.6,
     )
     print(result)</doc>
-      <shortdoc>Keyword for creating text completions in OpenAI. Keyword returns a text string.</shortdoc>
+      <shortdoc>Keyword for creating text completions in OpenAI and Azure OpenAI. Keyword returns a text string.</shortdoc>
     </kw>
-    <kw name="Image Create" lineno="227">
+    <kw name="Image Create" lineno="289">
       <arguments repr="prompt: str, size: str | None = 512x512, num_images: int | None = 1, result_format: str | None = list">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="prompt: str">
           <name>prompt</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="size: str | None = 512x512">
           <name>size</name>
@@ -264,17 +327,19 @@
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="result_format: str | None = list">
           <name>result_format</name>
           <type typedoc="string">str</type>
           <type typedoc="None">None</type>
           <default>list</default>
         </arg>
       </arguments>
-      <doc>Keyword for creating one or more images in OpenAI.
+      <doc>Keyword for creating one or more images using OpenAI.
 Keyword returns a list of urls for the images created.
 
+**Note**. Keyword not supported in the ``Azure OpenAI`` service.
+
 :param prompt: A text description of the desired image(s).
     The maximum length is 1000 characters.
 :param size: Size of the files to be created. 256x256, 512x512, 1024x1024
 :param num_images: The number of images to generate. Must be between 1 and 10.
 :param result_format: Result format (list / json).
 
 Robot Framework example:
@@ -296,17 +361,17 @@
     images = baselib.image_create(
         'Cartoon style picture of a cute monkey skateboarding',
         size='256x256',
         num_images=2,
     )
     for url in images:
         print(url)</doc>
-      <shortdoc>Keyword for creating one or more images in OpenAI. Keyword returns a list of urls for the images created.</shortdoc>
+      <shortdoc>Keyword for creating one or more images using OpenAI. Keyword returns a list of urls for the images created.</shortdoc>
     </kw>
-    <kw name="Image Create Variation" lineno="282">
+    <kw name="Image Create Variation" lineno="350">
       <arguments repr="src_image: str, size: str | None = 512x512, num_images: int | None = 1, result_format: str | None = list">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="src_image: str">
           <name>src_image</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="false" repr="size: str | None = 512x512">
           <name>size</name>
@@ -327,14 +392,16 @@
           <default>list</default>
         </arg>
       </arguments>
       <doc>Keyword for creating one or more variations of a image. Keyword
 returns a list of urls for the images created.
 Source file must be a valid PNG file, less than 4MB, and square.
 
+**Note**. Keyword not supported in the ``Azure OpenAI`` service.
+
 :param src_image: The image to use as the basis for the variation(s).
     Must be a valid PNG file, less than 4MB, and square.
 :param size: The size of the generated images.
     Must be one of 256x256, 512x512, or 1024x1024.
 :param num_images: The number of images to generate. Must be between 1 and 10
 :param result_format: Result format (list / json).
 
@@ -409,26 +476,28 @@
     <type name="None" type="Standard">
       <doc>String ``NONE`` (case-insensitive) is converted to Python ``None`` object.
 Other values cause an error.</doc>
       <accepts>
         <type>string</type>
       </accepts>
       <usages>
+        <usage>Authorize To Azure Openai</usage>
         <usage>Chat Completion Create</usage>
         <usage>Completion Create</usage>
         <usage>Image Create</usage>
         <usage>Image Create Variation</usage>
       </usages>
     </type>
     <type name="string" type="Standard">
       <doc>All arguments are converted to Unicode strings.</doc>
       <accepts>
         <type>Any</type>
       </accepts>
       <usages>
+        <usage>Authorize To Azure Openai</usage>
         <usage>Authorize To Openai</usage>
         <usage>Chat Completion Create</usage>
         <usage>Completion Create</usage>
         <usage>Image Create</usage>
         <usage>Image Create Variation</usage>
       </usages>
     </type>
```

### Comparing `rpaframework_openai-1.1.2/pyproject.toml` & `rpaframework_openai-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-[tool.poetry]
-name = "rpaframework-openai"
-version = "1.1.2"
-description = "OpenAI library for RPA Framework"
-authors = ["RPA Framework <rpafw@robocorp.com>"]
-license = "Apache-2.0"
-readme = "README.rst"
-
-homepage = "https://rpaframework.org/"
-documentation = "https://rpaframework.org/"
-repository = "https://github.com/robocorp/rpaframework"
-
-keywords = ["robotframework", "rpa", "automation", "openai"]
-classifiers = [
-	"License :: OSI Approved :: Apache Software License",
-	"Development Status :: 5 - Production/Stable",
-	"Operating System :: OS Independent",
-	"Intended Audience :: Developers",
-	"Topic :: Software Development :: Libraries :: Python Modules",
-	"Topic :: Software Development :: Libraries",
-	"Framework :: Robot Framework :: Library",
-	"Framework :: Robot Framework",
-	"Programming Language :: Python :: 3.7",
-	"Programming Language :: Python :: 3.8",
-	"Programming Language :: Python :: 3.9",
-]
-
-include = ["*.libspec"]
-
-packages = [{ include = "RPA", from = "src" }]
-
-[tool.poetry.dependencies]
-python = "^3.7.1"
-openai = "^0.27.0"
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-flake8 = "^3.7.9"
-pylint = "^2.4.4, <2.13"
-pytest = "^7.2.0"
-mock = "^5.0.0"
-pytest-cov = "^4.0.0"
-invoke = "^1.6.0"
-sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.1.1"
-toml = "^0.10.2"
-sphinx-markdown-builder = "^0.5.4"
-robotframework-docgen = "^0.15.0"
-sphinx-issues = "^3.0.1"
-docutils = "0.16"
-moto = "3.1.8"
-colorama = "^0.4.5"
-keyring = "^23.9.0"
-PyYAML = "^5.4.1"
-importlib-metadata = "^4.13.0"
-flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.7"
-
-[tool.black]
-target-version = ["py37", "py38", "py39"]
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-addopts = "-v --cov=src --cov-report term-missing --cov-branch"
-testpaths = ["tests"]
+[tool.poetry]
+name = "rpaframework-openai"
+version = "1.2.0"
+description = "OpenAI library for RPA Framework"
+authors = ["RPA Framework <rpafw@robocorp.com>"]
+license = "Apache-2.0"
+readme = "README.rst"
+
+homepage = "https://rpaframework.org/"
+documentation = "https://rpaframework.org/"
+repository = "https://github.com/robocorp/rpaframework"
+
+keywords = ["robotframework", "rpa", "automation", "openai"]
+classifiers = [
+	"License :: OSI Approved :: Apache Software License",
+	"Development Status :: 5 - Production/Stable",
+	"Operating System :: OS Independent",
+	"Intended Audience :: Developers",
+	"Topic :: Software Development :: Libraries :: Python Modules",
+	"Topic :: Software Development :: Libraries",
+	"Framework :: Robot Framework :: Library",
+	"Framework :: Robot Framework",
+	"Programming Language :: Python :: 3.7",
+	"Programming Language :: Python :: 3.8",
+	"Programming Language :: Python :: 3.9",
+]
+
+include = ["*.libspec"]
+
+packages = [{ include = "RPA", from = "src" }]
+
+[tool.poetry.dependencies]
+python = "^3.7.1"
+openai = "^0.27.7"
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.3.0"
+flake8 = "^3.7.9"
+pylint = "^2.4.4, <2.13"
+pytest = "^7.2.0"
+mock = "^5.0.0"
+pytest-cov = "^4.0.0"
+invoke = "^1.6.0"
+sphinx = "^5.3.0"
+sphinx-rtd-theme = "^1.1.1"
+toml = "^0.10.2"
+sphinx-markdown-builder = "^0.5.4"
+robotframework-docgen = "^0.15.0"
+sphinx-issues = "^3.0.1"
+docutils = "0.16"
+moto = "3.1.8"
+colorama = "^0.4.5"
+keyring = "^23.9.0"
+PyYAML = "^5.4.1"
+importlib-metadata = "^4.13.0"
+flake8-docstrings = "^1.6.0"
+flake8-rst-docstrings = "^0.2.7"
+
+[tool.black]
+target-version = ["py37", "py38", "py39"]
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+addopts = "-v --cov=src --cov-report term-missing --cov-branch"
+testpaths = ["tests"]
```

### Comparing `rpaframework_openai-1.1.2/PKG-INFO` & `rpaframework_openai-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-openai
-Version: 1.1.2
+Version: 1.2.0
 Summary: OpenAI library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,openai
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: openai (>=0.27.0,<0.28.0)
+Requires-Dist: openai (>=0.27.7,<0.28.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
 
 rpaframework-openai
 ===================
```

