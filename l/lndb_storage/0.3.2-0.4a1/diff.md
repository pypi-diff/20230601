# Comparing `tmp/lndb_storage-0.3.2.tar.gz` & `tmp/lndb_storage-0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.3.2.tar", last modified: Sun May 28 14:43:27 2023, max compression
+gzip compressed data, was "lndb_storage-0.4a1.tar", last modified: Thu Jun  1 12:13:50 2023, max compression
```

## Comparing `lndb_storage-0.3.2.tar` & `lndb_storage-0.4a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3285 2023-05-28 10:46:30.904356 lndb_storage-0.3.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      135 2022-11-13 16:42:34.073467 lndb_storage-0.3.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      622 2022-11-13 16:42:34.079466 lndb_storage-0.3.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1307 2022-11-13 16:42:34.087464 lndb_storage-0.3.2/.gitignore
--rw-r--r--   0        0        0     1829 2023-04-27 12:28:45.977838 lndb_storage-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11525 2022-11-13 16:42:34.107465 lndb_storage-0.3.2/LICENSE
--rw-r--r--   0        0        0      127 2023-04-04 17:37:51.923635 lndb_storage-0.3.2/README.md
--rw-r--r--   0        0        0     3759 2023-05-28 14:42:45.235025 lndb_storage-0.3.2/docs/changelog.md
--rw-r--r--   0        0        0    10222 2023-04-23 18:25:59.426479 lndb_storage-0.3.2/docs/guide/add-replace-stage.ipynb
--rw-r--r--   0        0        0       98 2023-04-10 13:07:42.667859 lndb_storage-0.3.2/docs/guide/index.md
--rw-r--r--   0        0        0     4127 2023-04-04 17:37:51.986149 lndb_storage-0.3.2/docs/guide/iris.csv
--rw-r--r--   0        0        0     4700 2023-04-04 17:37:52.017398 lndb_storage-0.3.2/docs/guide/iris.data
--rw-r--r--   0        0        0     4500 2023-04-23 18:25:59.447479 lndb_storage-0.3.2/docs/guide/new_iris.csv
--rw-r--r--   0        0        0     4853 2023-04-10 13:07:42.667859 lndb_storage-0.3.2/docs/guide/serialize-cache.ipynb
--rw-r--r--   0        0        0     5889 2023-05-27 13:51:12.723290 lndb_storage-0.3.2/docs/guide/stream.ipynb
--rw-r--r--   0        0        0     9234 2023-05-28 14:38:51.236000 lndb_storage-0.3.2/docs/guide/upload.ipynb
--rw-r--r--   0        0        0      134 2023-04-10 13:07:42.721318 lndb_storage-0.3.2/docs/index.md
--rw-r--r--   0        0        0       65 2023-04-10 13:07:42.721318 lndb_storage-0.3.2/docs/reference.md
--rw-r--r--   0        0        0      165 2022-11-13 16:42:34.193462 lndb_storage-0.3.2/lamin-project.yaml
--rw-r--r--   0        0        0      579 2023-05-28 14:42:45.955147 lndb_storage-0.3.2/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3450 2023-04-18 13:49:41.034991 lndb_storage-0.3.2/lndb_storage/_file.py
--rw-r--r--   0        0        0      509 2023-04-16 14:26:59.906685 lndb_storage-0.3.2/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      212 2023-03-13 18:04:48.685214 lndb_storage-0.3.2/lndb_storage/_images.py
--rw-r--r--   0        0        0     2374 2023-03-26 12:52:12.411859 lndb_storage-0.3.2/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2851 2023-04-10 13:07:42.783828 lndb_storage-0.3.2/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      332 2023-03-26 12:52:12.411859 lndb_storage-0.3.2/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      972 2023-04-16 14:26:59.906685 lndb_storage-0.3.2/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0    12088 2023-05-27 13:51:12.746289 lndb_storage-0.3.2/lndb_storage/object/_anndata_accessor.py
--rw-r--r--   0        0        0      761 2023-03-13 18:04:48.716390 lndb_storage-0.3.2/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      931 2023-03-14 18:15:14.187412 lndb_storage-0.3.2/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4274 2023-03-13 18:04:48.716390 lndb_storage-0.3.2/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     4100 2023-05-27 13:51:12.758291 lndb_storage-0.3.2/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      959 2023-05-27 13:51:12.769318 lndb_storage-0.3.2/noxfile.py
--rw-r--r--   0        0        0     1140 2023-05-28 14:38:51.251649 lndb_storage-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      500 2023-05-07 12:55:11.415073 lndb_storage-0.3.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 lndb_storage-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3186 2023-05-28 10:01:53.664520 lndb_storage-0.4a1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.4a1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.4a1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.4a1/.gitignore
+-rw-r--r--   0        0        0     1765 2023-04-24 16:53:24.500304 lndb_storage-0.4a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.4a1/LICENSE
+-rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.4a1/README.md
+-rw-r--r--   0        0        0     3921 2023-06-01 12:13:32.783503 lndb_storage-0.4a1/docs/changelog.md
+-rw-r--r--   0        0        0     9693 2023-06-01 12:13:23.602348 lndb_storage-0.4a1/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.4a1/docs/guide/index.md
+-rw-r--r--   0        0        0     3976 2023-05-28 10:02:04.898719 lndb_storage-0.4a1/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4550 2023-05-28 10:02:04.898995 lndb_storage-0.4a1/docs/guide/iris.data
+-rw-r--r--   0        0        0     4349 2023-05-28 10:02:04.899279 lndb_storage-0.4a1/docs/guide/new_iris.csv
+-rw-r--r--   0        0        0     4624 2023-06-01 12:13:23.602530 lndb_storage-0.4a1/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     5600 2023-05-28 16:19:45.635177 lndb_storage-0.4a1/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     8813 2023-05-28 16:19:45.636193 lndb_storage-0.4a1/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.4a1/docs/index.md
+-rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.4a1/docs/reference.md
+-rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.4a1/lamin-project.yaml
+-rw-r--r--   0        0        0      597 2023-06-01 12:13:27.648873 lndb_storage-0.4a1/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3355 2023-06-01 12:13:23.602870 lndb_storage-0.4a1/lndb_storage/_file.py
+-rw-r--r--   0        0        0      510 2023-06-01 12:13:23.603125 lndb_storage-0.4a1/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.4a1/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.4a1/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2773 2023-06-01 12:13:23.603355 lndb_storage-0.4a1/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.4a1/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      954 2023-06-01 12:13:23.603603 lndb_storage-0.4a1/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0    11739 2023-06-01 12:13:23.603824 lndb_storage-0.4a1/lndb_storage/object/_anndata_accessor.py
+-rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.4a1/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.4a1/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.4a1/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     4000 2023-06-01 12:13:23.603991 lndb_storage-0.4a1/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      921 2023-06-01 12:13:23.604224 lndb_storage-0.4a1/noxfile.py
+-rw-r--r--   0        0        0     1087 2023-06-01 12:13:23.604554 lndb_storage-0.4a1/pyproject.toml
+-rw-r--r--   0        0        0      484 2023-05-23 14:40:16.493813 lndb_storage-0.4a1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 lndb_storage-0.4a1/PKG-INFO
```

### Comparing `lndb_storage-0.3.2/LICENSE` & `lndb_storage-0.4a1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
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
-   Copyright [yyyy] [name of copyright owner]
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
+Apache License
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
+   Copyright [yyyy] [name of copyright owner]
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

### Comparing `lndb_storage-0.3.2/docs/changelog.md` & `lndb_storage-0.4a1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+:truck: Rename lndb to lamindb-storage | [40](https://github.com/laminlabs/lndb-storage/pull/40) | [falexwolf](https://github.com/falexwolf) | 2023-06-01 | 0.4a1
 ➖ Update fsspec and move s3 and gs dependencies to extras  | [38](https://github.com/laminlabs/lndb-storage/pull/38) | [Koncopd](https://github.com/Koncopd) | 2023-05-28 | 0.3.2
 :memo: Add content from lamindb | [36](https://github.com/laminlabs/lndb-storage/pull/36) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 |
 ✨ `AnnDataAccessor` for access to cloud AnnData attributes | [32](https://github.com/laminlabs/lndb-storage/pull/32) | [Koncopd](https://github.com/Koncopd) | 2023-05-27 | 0.3.1
 ✅ Use nbproject-test directly in test_notebooks.py | [31](https://github.com/laminlabs/lndb-storage/pull/31) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 | 0.3.0
 ♻️ Refactor CloudAnnData | [29](https://github.com/laminlabs/lndb-storage/pull/29) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 🦺 Check that obs and var are dataframes in subset | [28](https://github.com/laminlabs/lndb-storage/pull/28) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 ✨ Add `CloudAnnData` | [26](https://github.com/laminlabs/lndb-storage/pull/26) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.2rc6
```

### Comparing `lndb_storage-0.3.2/docs/guide/iris.data` & `lndb_storage-0.4a1/docs/guide/iris.data`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-5.1,3.5,1.4,0.2,Iris-setosa
-4.9,3.0,1.4,0.2,Iris-setosa
-4.7,3.2,1.3,0.2,Iris-setosa
-4.6,3.1,1.5,0.2,Iris-setosa
-5.0,3.6,1.4,0.2,Iris-setosa
-5.4,3.9,1.7,0.4,Iris-setosa
-4.6,3.4,1.4,0.3,Iris-setosa
-5.0,3.4,1.5,0.2,Iris-setosa
-4.4,2.9,1.4,0.2,Iris-setosa
-4.9,3.1,1.5,0.1,Iris-setosa
-5.4,3.7,1.5,0.2,Iris-setosa
-4.8,3.4,1.6,0.2,Iris-setosa
-4.8,3.0,1.4,0.1,Iris-setosa
-4.3,3.0,1.1,0.1,Iris-setosa
-5.8,4.0,1.2,0.2,Iris-setosa
-5.7,4.4,1.5,0.4,Iris-setosa
-5.4,3.9,1.3,0.4,Iris-setosa
-5.1,3.5,1.4,0.3,Iris-setosa
-5.7,3.8,1.7,0.3,Iris-setosa
-5.1,3.8,1.5,0.3,Iris-setosa
-5.4,3.4,1.7,0.2,Iris-setosa
-5.1,3.7,1.5,0.4,Iris-setosa
-4.6,3.6,1.0,0.2,Iris-setosa
-5.1,3.3,1.7,0.5,Iris-setosa
-4.8,3.4,1.9,0.2,Iris-setosa
-5.0,3.0,1.6,0.2,Iris-setosa
-5.0,3.4,1.6,0.4,Iris-setosa
-5.2,3.5,1.5,0.2,Iris-setosa
-5.2,3.4,1.4,0.2,Iris-setosa
-4.7,3.2,1.6,0.2,Iris-setosa
-4.8,3.1,1.6,0.2,Iris-setosa
-5.4,3.4,1.5,0.4,Iris-setosa
-5.2,4.1,1.5,0.1,Iris-setosa
-5.5,4.2,1.4,0.2,Iris-setosa
-4.9,3.1,1.5,0.1,Iris-setosa
-5.0,3.2,1.2,0.2,Iris-setosa
-5.5,3.5,1.3,0.2,Iris-setosa
-4.9,3.1,1.5,0.1,Iris-setosa
-4.4,3.0,1.3,0.2,Iris-setosa
-5.1,3.4,1.5,0.2,Iris-setosa
-5.0,3.5,1.3,0.3,Iris-setosa
-4.5,2.3,1.3,0.3,Iris-setosa
-4.4,3.2,1.3,0.2,Iris-setosa
-5.0,3.5,1.6,0.6,Iris-setosa
-5.1,3.8,1.9,0.4,Iris-setosa
-4.8,3.0,1.4,0.3,Iris-setosa
-5.1,3.8,1.6,0.2,Iris-setosa
-4.6,3.2,1.4,0.2,Iris-setosa
-5.3,3.7,1.5,0.2,Iris-setosa
-5.0,3.3,1.4,0.2,Iris-setosa
-7.0,3.2,4.7,1.4,Iris-versicolor
-6.4,3.2,4.5,1.5,Iris-versicolor
-6.9,3.1,4.9,1.5,Iris-versicolor
-5.5,2.3,4.0,1.3,Iris-versicolor
-6.5,2.8,4.6,1.5,Iris-versicolor
-5.7,2.8,4.5,1.3,Iris-versicolor
-6.3,3.3,4.7,1.6,Iris-versicolor
-4.9,2.4,3.3,1.0,Iris-versicolor
-6.6,2.9,4.6,1.3,Iris-versicolor
-5.2,2.7,3.9,1.4,Iris-versicolor
-5.0,2.0,3.5,1.0,Iris-versicolor
-5.9,3.0,4.2,1.5,Iris-versicolor
-6.0,2.2,4.0,1.0,Iris-versicolor
-6.1,2.9,4.7,1.4,Iris-versicolor
-5.6,2.9,3.6,1.3,Iris-versicolor
-6.7,3.1,4.4,1.4,Iris-versicolor
-5.6,3.0,4.5,1.5,Iris-versicolor
-5.8,2.7,4.1,1.0,Iris-versicolor
-6.2,2.2,4.5,1.5,Iris-versicolor
-5.6,2.5,3.9,1.1,Iris-versicolor
-5.9,3.2,4.8,1.8,Iris-versicolor
-6.1,2.8,4.0,1.3,Iris-versicolor
-6.3,2.5,4.9,1.5,Iris-versicolor
-6.1,2.8,4.7,1.2,Iris-versicolor
-6.4,2.9,4.3,1.3,Iris-versicolor
-6.6,3.0,4.4,1.4,Iris-versicolor
-6.8,2.8,4.8,1.4,Iris-versicolor
-6.7,3.0,5.0,1.7,Iris-versicolor
-6.0,2.9,4.5,1.5,Iris-versicolor
-5.7,2.6,3.5,1.0,Iris-versicolor
-5.5,2.4,3.8,1.1,Iris-versicolor
-5.5,2.4,3.7,1.0,Iris-versicolor
-5.8,2.7,3.9,1.2,Iris-versicolor
-6.0,2.7,5.1,1.6,Iris-versicolor
-5.4,3.0,4.5,1.5,Iris-versicolor
-6.0,3.4,4.5,1.6,Iris-versicolor
-6.7,3.1,4.7,1.5,Iris-versicolor
-6.3,2.3,4.4,1.3,Iris-versicolor
-5.6,3.0,4.1,1.3,Iris-versicolor
-5.5,2.5,4.0,1.3,Iris-versicolor
-5.5,2.6,4.4,1.2,Iris-versicolor
-6.1,3.0,4.6,1.4,Iris-versicolor
-5.8,2.6,4.0,1.2,Iris-versicolor
-5.0,2.3,3.3,1.0,Iris-versicolor
-5.6,2.7,4.2,1.3,Iris-versicolor
-5.7,3.0,4.2,1.2,Iris-versicolor
-5.7,2.9,4.2,1.3,Iris-versicolor
-6.2,2.9,4.3,1.3,Iris-versicolor
-5.1,2.5,3.0,1.1,Iris-versicolor
-5.7,2.8,4.1,1.3,Iris-versicolor
-6.3,3.3,6.0,2.5,Iris-virginica
-5.8,2.7,5.1,1.9,Iris-virginica
-7.1,3.0,5.9,2.1,Iris-virginica
-6.3,2.9,5.6,1.8,Iris-virginica
-6.5,3.0,5.8,2.2,Iris-virginica
-7.6,3.0,6.6,2.1,Iris-virginica
-4.9,2.5,4.5,1.7,Iris-virginica
-7.3,2.9,6.3,1.8,Iris-virginica
-6.7,2.5,5.8,1.8,Iris-virginica
-7.2,3.6,6.1,2.5,Iris-virginica
-6.5,3.2,5.1,2.0,Iris-virginica
-6.4,2.7,5.3,1.9,Iris-virginica
-6.8,3.0,5.5,2.1,Iris-virginica
-5.7,2.5,5.0,2.0,Iris-virginica
-5.8,2.8,5.1,2.4,Iris-virginica
-6.4,3.2,5.3,2.3,Iris-virginica
-6.5,3.0,5.5,1.8,Iris-virginica
-7.7,3.8,6.7,2.2,Iris-virginica
-7.7,2.6,6.9,2.3,Iris-virginica
-6.0,2.2,5.0,1.5,Iris-virginica
-6.9,3.2,5.7,2.3,Iris-virginica
-5.6,2.8,4.9,2.0,Iris-virginica
-7.7,2.8,6.7,2.0,Iris-virginica
-6.3,2.7,4.9,1.8,Iris-virginica
-6.7,3.3,5.7,2.1,Iris-virginica
-7.2,3.2,6.0,1.8,Iris-virginica
-6.2,2.8,4.8,1.8,Iris-virginica
-6.1,3.0,4.9,1.8,Iris-virginica
-6.4,2.8,5.6,2.1,Iris-virginica
-7.2,3.0,5.8,1.6,Iris-virginica
-7.4,2.8,6.1,1.9,Iris-virginica
-7.9,3.8,6.4,2.0,Iris-virginica
-6.4,2.8,5.6,2.2,Iris-virginica
-6.3,2.8,5.1,1.5,Iris-virginica
-6.1,2.6,5.6,1.4,Iris-virginica
-7.7,3.0,6.1,2.3,Iris-virginica
-6.3,3.4,5.6,2.4,Iris-virginica
-6.4,3.1,5.5,1.8,Iris-virginica
-6.0,3.0,4.8,1.8,Iris-virginica
-6.9,3.1,5.4,2.1,Iris-virginica
-6.7,3.1,5.6,2.4,Iris-virginica
-6.9,3.1,5.1,2.3,Iris-virginica
-5.8,2.7,5.1,1.9,Iris-virginica
-6.8,3.2,5.9,2.3,Iris-virginica
-6.7,3.3,5.7,2.5,Iris-virginica
-6.7,3.0,5.2,2.3,Iris-virginica
-6.3,2.5,5.0,1.9,Iris-virginica
-6.5,3.0,5.2,2.0,Iris-virginica
-6.2,3.4,5.4,2.3,Iris-virginica
-5.9,3.0,5.1,1.8,Iris-virginica
+5.1,3.5,1.4,0.2,Iris-setosa
+4.9,3.0,1.4,0.2,Iris-setosa
+4.7,3.2,1.3,0.2,Iris-setosa
+4.6,3.1,1.5,0.2,Iris-setosa
+5.0,3.6,1.4,0.2,Iris-setosa
+5.4,3.9,1.7,0.4,Iris-setosa
+4.6,3.4,1.4,0.3,Iris-setosa
+5.0,3.4,1.5,0.2,Iris-setosa
+4.4,2.9,1.4,0.2,Iris-setosa
+4.9,3.1,1.5,0.1,Iris-setosa
+5.4,3.7,1.5,0.2,Iris-setosa
+4.8,3.4,1.6,0.2,Iris-setosa
+4.8,3.0,1.4,0.1,Iris-setosa
+4.3,3.0,1.1,0.1,Iris-setosa
+5.8,4.0,1.2,0.2,Iris-setosa
+5.7,4.4,1.5,0.4,Iris-setosa
+5.4,3.9,1.3,0.4,Iris-setosa
+5.1,3.5,1.4,0.3,Iris-setosa
+5.7,3.8,1.7,0.3,Iris-setosa
+5.1,3.8,1.5,0.3,Iris-setosa
+5.4,3.4,1.7,0.2,Iris-setosa
+5.1,3.7,1.5,0.4,Iris-setosa
+4.6,3.6,1.0,0.2,Iris-setosa
+5.1,3.3,1.7,0.5,Iris-setosa
+4.8,3.4,1.9,0.2,Iris-setosa
+5.0,3.0,1.6,0.2,Iris-setosa
+5.0,3.4,1.6,0.4,Iris-setosa
+5.2,3.5,1.5,0.2,Iris-setosa
+5.2,3.4,1.4,0.2,Iris-setosa
+4.7,3.2,1.6,0.2,Iris-setosa
+4.8,3.1,1.6,0.2,Iris-setosa
+5.4,3.4,1.5,0.4,Iris-setosa
+5.2,4.1,1.5,0.1,Iris-setosa
+5.5,4.2,1.4,0.2,Iris-setosa
+4.9,3.1,1.5,0.1,Iris-setosa
+5.0,3.2,1.2,0.2,Iris-setosa
+5.5,3.5,1.3,0.2,Iris-setosa
+4.9,3.1,1.5,0.1,Iris-setosa
+4.4,3.0,1.3,0.2,Iris-setosa
+5.1,3.4,1.5,0.2,Iris-setosa
+5.0,3.5,1.3,0.3,Iris-setosa
+4.5,2.3,1.3,0.3,Iris-setosa
+4.4,3.2,1.3,0.2,Iris-setosa
+5.0,3.5,1.6,0.6,Iris-setosa
+5.1,3.8,1.9,0.4,Iris-setosa
+4.8,3.0,1.4,0.3,Iris-setosa
+5.1,3.8,1.6,0.2,Iris-setosa
+4.6,3.2,1.4,0.2,Iris-setosa
+5.3,3.7,1.5,0.2,Iris-setosa
+5.0,3.3,1.4,0.2,Iris-setosa
+7.0,3.2,4.7,1.4,Iris-versicolor
+6.4,3.2,4.5,1.5,Iris-versicolor
+6.9,3.1,4.9,1.5,Iris-versicolor
+5.5,2.3,4.0,1.3,Iris-versicolor
+6.5,2.8,4.6,1.5,Iris-versicolor
+5.7,2.8,4.5,1.3,Iris-versicolor
+6.3,3.3,4.7,1.6,Iris-versicolor
+4.9,2.4,3.3,1.0,Iris-versicolor
+6.6,2.9,4.6,1.3,Iris-versicolor
+5.2,2.7,3.9,1.4,Iris-versicolor
+5.0,2.0,3.5,1.0,Iris-versicolor
+5.9,3.0,4.2,1.5,Iris-versicolor
+6.0,2.2,4.0,1.0,Iris-versicolor
+6.1,2.9,4.7,1.4,Iris-versicolor
+5.6,2.9,3.6,1.3,Iris-versicolor
+6.7,3.1,4.4,1.4,Iris-versicolor
+5.6,3.0,4.5,1.5,Iris-versicolor
+5.8,2.7,4.1,1.0,Iris-versicolor
+6.2,2.2,4.5,1.5,Iris-versicolor
+5.6,2.5,3.9,1.1,Iris-versicolor
+5.9,3.2,4.8,1.8,Iris-versicolor
+6.1,2.8,4.0,1.3,Iris-versicolor
+6.3,2.5,4.9,1.5,Iris-versicolor
+6.1,2.8,4.7,1.2,Iris-versicolor
+6.4,2.9,4.3,1.3,Iris-versicolor
+6.6,3.0,4.4,1.4,Iris-versicolor
+6.8,2.8,4.8,1.4,Iris-versicolor
+6.7,3.0,5.0,1.7,Iris-versicolor
+6.0,2.9,4.5,1.5,Iris-versicolor
+5.7,2.6,3.5,1.0,Iris-versicolor
+5.5,2.4,3.8,1.1,Iris-versicolor
+5.5,2.4,3.7,1.0,Iris-versicolor
+5.8,2.7,3.9,1.2,Iris-versicolor
+6.0,2.7,5.1,1.6,Iris-versicolor
+5.4,3.0,4.5,1.5,Iris-versicolor
+6.0,3.4,4.5,1.6,Iris-versicolor
+6.7,3.1,4.7,1.5,Iris-versicolor
+6.3,2.3,4.4,1.3,Iris-versicolor
+5.6,3.0,4.1,1.3,Iris-versicolor
+5.5,2.5,4.0,1.3,Iris-versicolor
+5.5,2.6,4.4,1.2,Iris-versicolor
+6.1,3.0,4.6,1.4,Iris-versicolor
+5.8,2.6,4.0,1.2,Iris-versicolor
+5.0,2.3,3.3,1.0,Iris-versicolor
+5.6,2.7,4.2,1.3,Iris-versicolor
+5.7,3.0,4.2,1.2,Iris-versicolor
+5.7,2.9,4.2,1.3,Iris-versicolor
+6.2,2.9,4.3,1.3,Iris-versicolor
+5.1,2.5,3.0,1.1,Iris-versicolor
+5.7,2.8,4.1,1.3,Iris-versicolor
+6.3,3.3,6.0,2.5,Iris-virginica
+5.8,2.7,5.1,1.9,Iris-virginica
+7.1,3.0,5.9,2.1,Iris-virginica
+6.3,2.9,5.6,1.8,Iris-virginica
+6.5,3.0,5.8,2.2,Iris-virginica
+7.6,3.0,6.6,2.1,Iris-virginica
+4.9,2.5,4.5,1.7,Iris-virginica
+7.3,2.9,6.3,1.8,Iris-virginica
+6.7,2.5,5.8,1.8,Iris-virginica
+7.2,3.6,6.1,2.5,Iris-virginica
+6.5,3.2,5.1,2.0,Iris-virginica
+6.4,2.7,5.3,1.9,Iris-virginica
+6.8,3.0,5.5,2.1,Iris-virginica
+5.7,2.5,5.0,2.0,Iris-virginica
+5.8,2.8,5.1,2.4,Iris-virginica
+6.4,3.2,5.3,2.3,Iris-virginica
+6.5,3.0,5.5,1.8,Iris-virginica
+7.7,3.8,6.7,2.2,Iris-virginica
+7.7,2.6,6.9,2.3,Iris-virginica
+6.0,2.2,5.0,1.5,Iris-virginica
+6.9,3.2,5.7,2.3,Iris-virginica
+5.6,2.8,4.9,2.0,Iris-virginica
+7.7,2.8,6.7,2.0,Iris-virginica
+6.3,2.7,4.9,1.8,Iris-virginica
+6.7,3.3,5.7,2.1,Iris-virginica
+7.2,3.2,6.0,1.8,Iris-virginica
+6.2,2.8,4.8,1.8,Iris-virginica
+6.1,3.0,4.9,1.8,Iris-virginica
+6.4,2.8,5.6,2.1,Iris-virginica
+7.2,3.0,5.8,1.6,Iris-virginica
+7.4,2.8,6.1,1.9,Iris-virginica
+7.9,3.8,6.4,2.0,Iris-virginica
+6.4,2.8,5.6,2.2,Iris-virginica
+6.3,2.8,5.1,1.5,Iris-virginica
+6.1,2.6,5.6,1.4,Iris-virginica
+7.7,3.0,6.1,2.3,Iris-virginica
+6.3,3.4,5.6,2.4,Iris-virginica
+6.4,3.1,5.5,1.8,Iris-virginica
+6.0,3.0,4.8,1.8,Iris-virginica
+6.9,3.1,5.4,2.1,Iris-virginica
+6.7,3.1,5.6,2.4,Iris-virginica
+6.9,3.1,5.1,2.3,Iris-virginica
+5.8,2.7,5.1,1.9,Iris-virginica
+6.8,3.2,5.9,2.3,Iris-virginica
+6.7,3.3,5.7,2.5,Iris-virginica
+6.7,3.0,5.2,2.3,Iris-virginica
+6.3,2.5,5.0,1.9,Iris-virginica
+6.5,3.0,5.2,2.0,Iris-virginica
+6.2,3.4,5.4,2.3,Iris-virginica
+5.9,3.0,5.1,1.8,Iris-virginica
```

### Comparing `lndb_storage-0.3.2/docs/guide/new_iris.csv` & `lndb_storage-0.4a1/docs/guide/new_iris.csv`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-;sepal.length;sepal.width;petal.length;petal.width;variety
-0;5.1;3.5;1.4;0.2;Setosa
-1;4.9;3.0;1.4;0.2;Setosa
-2;4.7;3.2;1.3;0.2;Setosa
-3;4.6;3.1;1.5;0.2;Setosa
-4;5.0;3.6;1.4;0.2;Setosa
-5;5.4;3.9;1.7;0.4;Setosa
-6;4.6;3.4;1.4;0.3;Setosa
-7;5.0;3.4;1.5;0.2;Setosa
-8;4.4;2.9;1.4;0.2;Setosa
-9;4.9;3.1;1.5;0.1;Setosa
-10;5.4;3.7;1.5;0.2;Setosa
-11;4.8;3.4;1.6;0.2;Setosa
-12;4.8;3.0;1.4;0.1;Setosa
-13;4.3;3.0;1.1;0.1;Setosa
-14;5.8;4.0;1.2;0.2;Setosa
-15;5.7;4.4;1.5;0.4;Setosa
-16;5.4;3.9;1.3;0.4;Setosa
-17;5.1;3.5;1.4;0.3;Setosa
-18;5.7;3.8;1.7;0.3;Setosa
-19;5.1;3.8;1.5;0.3;Setosa
-20;5.4;3.4;1.7;0.2;Setosa
-21;5.1;3.7;1.5;0.4;Setosa
-22;4.6;3.6;1.0;0.2;Setosa
-23;5.1;3.3;1.7;0.5;Setosa
-24;4.8;3.4;1.9;0.2;Setosa
-25;5.0;3.0;1.6;0.2;Setosa
-26;5.0;3.4;1.6;0.4;Setosa
-27;5.2;3.5;1.5;0.2;Setosa
-28;5.2;3.4;1.4;0.2;Setosa
-29;4.7;3.2;1.6;0.2;Setosa
-30;4.8;3.1;1.6;0.2;Setosa
-31;5.4;3.4;1.5;0.4;Setosa
-32;5.2;4.1;1.5;0.1;Setosa
-33;5.5;4.2;1.4;0.2;Setosa
-34;4.9;3.1;1.5;0.2;Setosa
-35;5.0;3.2;1.2;0.2;Setosa
-36;5.5;3.5;1.3;0.2;Setosa
-37;4.9;3.6;1.4;0.1;Setosa
-38;4.4;3.0;1.3;0.2;Setosa
-39;5.1;3.4;1.5;0.2;Setosa
-40;5.0;3.5;1.3;0.3;Setosa
-41;4.5;2.3;1.3;0.3;Setosa
-42;4.4;3.2;1.3;0.2;Setosa
-43;5.0;3.5;1.6;0.6;Setosa
-44;5.1;3.8;1.9;0.4;Setosa
-45;4.8;3.0;1.4;0.3;Setosa
-46;5.1;3.8;1.6;0.2;Setosa
-47;4.6;3.2;1.4;0.2;Setosa
-48;5.3;3.7;1.5;0.2;Setosa
-49;5.0;3.3;1.4;0.2;Setosa
-50;7.0;3.2;4.7;1.4;Versicolor
-51;6.4;3.2;4.5;1.5;Versicolor
-52;6.9;3.1;4.9;1.5;Versicolor
-53;5.5;2.3;4.0;1.3;Versicolor
-54;6.5;2.8;4.6;1.5;Versicolor
-55;5.7;2.8;4.5;1.3;Versicolor
-56;6.3;3.3;4.7;1.6;Versicolor
-57;4.9;2.4;3.3;1.0;Versicolor
-58;6.6;2.9;4.6;1.3;Versicolor
-59;5.2;2.7;3.9;1.4;Versicolor
-60;5.0;2.0;3.5;1.0;Versicolor
-61;5.9;3.0;4.2;1.5;Versicolor
-62;6.0;2.2;4.0;1.0;Versicolor
-63;6.1;2.9;4.7;1.4;Versicolor
-64;5.6;2.9;3.6;1.3;Versicolor
-65;6.7;3.1;4.4;1.4;Versicolor
-66;5.6;3.0;4.5;1.5;Versicolor
-67;5.8;2.7;4.1;1.0;Versicolor
-68;6.2;2.2;4.5;1.5;Versicolor
-69;5.6;2.5;3.9;1.1;Versicolor
-70;5.9;3.2;4.8;1.8;Versicolor
-71;6.1;2.8;4.0;1.3;Versicolor
-72;6.3;2.5;4.9;1.5;Versicolor
-73;6.1;2.8;4.7;1.2;Versicolor
-74;6.4;2.9;4.3;1.3;Versicolor
-75;6.6;3.0;4.4;1.4;Versicolor
-76;6.8;2.8;4.8;1.4;Versicolor
-77;6.7;3.0;5.0;1.7;Versicolor
-78;6.0;2.9;4.5;1.5;Versicolor
-79;5.7;2.6;3.5;1.0;Versicolor
-80;5.5;2.4;3.8;1.1;Versicolor
-81;5.5;2.4;3.7;1.0;Versicolor
-82;5.8;2.7;3.9;1.2;Versicolor
-83;6.0;2.7;5.1;1.6;Versicolor
-84;5.4;3.0;4.5;1.5;Versicolor
-85;6.0;3.4;4.5;1.6;Versicolor
-86;6.7;3.1;4.7;1.5;Versicolor
-87;6.3;2.3;4.4;1.3;Versicolor
-88;5.6;3.0;4.1;1.3;Versicolor
-89;5.5;2.5;4.0;1.3;Versicolor
-90;5.5;2.6;4.4;1.2;Versicolor
-91;6.1;3.0;4.6;1.4;Versicolor
-92;5.8;2.6;4.0;1.2;Versicolor
-93;5.0;2.3;3.3;1.0;Versicolor
-94;5.6;2.7;4.2;1.3;Versicolor
-95;5.7;3.0;4.2;1.2;Versicolor
-96;5.7;2.9;4.2;1.3;Versicolor
-97;6.2;2.9;4.3;1.3;Versicolor
-98;5.1;2.5;3.0;1.1;Versicolor
-99;5.7;2.8;4.1;1.3;Versicolor
-100;6.3;3.3;6.0;2.5;Virginica
-101;5.8;2.7;5.1;1.9;Virginica
-102;7.1;3.0;5.9;2.1;Virginica
-103;6.3;2.9;5.6;1.8;Virginica
-104;6.5;3.0;5.8;2.2;Virginica
-105;7.6;3.0;6.6;2.1;Virginica
-106;4.9;2.5;4.5;1.7;Virginica
-107;7.3;2.9;6.3;1.8;Virginica
-108;6.7;2.5;5.8;1.8;Virginica
-109;7.2;3.6;6.1;2.5;Virginica
-110;6.5;3.2;5.1;2.0;Virginica
-111;6.4;2.7;5.3;1.9;Virginica
-112;6.8;3.0;5.5;2.1;Virginica
-113;5.7;2.5;5.0;2.0;Virginica
-114;5.8;2.8;5.1;2.4;Virginica
-115;6.4;3.2;5.3;2.3;Virginica
-116;6.5;3.0;5.5;1.8;Virginica
-117;7.7;3.8;6.7;2.2;Virginica
-118;7.7;2.6;6.9;2.3;Virginica
-119;6.0;2.2;5.0;1.5;Virginica
-120;6.9;3.2;5.7;2.3;Virginica
-121;5.6;2.8;4.9;2.0;Virginica
-122;7.7;2.8;6.7;2.0;Virginica
-123;6.3;2.7;4.9;1.8;Virginica
-124;6.7;3.3;5.7;2.1;Virginica
-125;7.2;3.2;6.0;1.8;Virginica
-126;6.2;2.8;4.8;1.8;Virginica
-127;6.1;3.0;4.9;1.8;Virginica
-128;6.4;2.8;5.6;2.1;Virginica
-129;7.2;3.0;5.8;1.6;Virginica
-130;7.4;2.8;6.1;1.9;Virginica
-131;7.9;3.8;6.4;2.0;Virginica
-132;6.4;2.8;5.6;2.2;Virginica
-133;6.3;2.8;5.1;1.5;Virginica
-134;6.1;2.6;5.6;1.4;Virginica
-135;7.7;3.0;6.1;2.3;Virginica
-136;6.3;3.4;5.6;2.4;Virginica
-137;6.4;3.1;5.5;1.8;Virginica
-138;6.0;3.0;4.8;1.8;Virginica
-139;6.9;3.1;5.4;2.1;Virginica
-140;6.7;3.1;5.6;2.4;Virginica
-141;6.9;3.1;5.1;2.3;Virginica
-142;5.8;2.7;5.1;1.9;Virginica
-143;6.8;3.2;5.9;2.3;Virginica
-144;6.7;3.3;5.7;2.5;Virginica
-145;6.7;3.0;5.2;2.3;Virginica
-146;6.3;2.5;5.0;1.9;Virginica
-147;6.5;3.0;5.2;2.0;Virginica
-148;6.2;3.4;5.4;2.3;Virginica
-149;5.9;3.0;5.1;1.8;Virginica
+;sepal.length;sepal.width;petal.length;petal.width;variety
+0;5.1;3.5;1.4;0.2;Setosa
+1;4.9;3.0;1.4;0.2;Setosa
+2;4.7;3.2;1.3;0.2;Setosa
+3;4.6;3.1;1.5;0.2;Setosa
+4;5.0;3.6;1.4;0.2;Setosa
+5;5.4;3.9;1.7;0.4;Setosa
+6;4.6;3.4;1.4;0.3;Setosa
+7;5.0;3.4;1.5;0.2;Setosa
+8;4.4;2.9;1.4;0.2;Setosa
+9;4.9;3.1;1.5;0.1;Setosa
+10;5.4;3.7;1.5;0.2;Setosa
+11;4.8;3.4;1.6;0.2;Setosa
+12;4.8;3.0;1.4;0.1;Setosa
+13;4.3;3.0;1.1;0.1;Setosa
+14;5.8;4.0;1.2;0.2;Setosa
+15;5.7;4.4;1.5;0.4;Setosa
+16;5.4;3.9;1.3;0.4;Setosa
+17;5.1;3.5;1.4;0.3;Setosa
+18;5.7;3.8;1.7;0.3;Setosa
+19;5.1;3.8;1.5;0.3;Setosa
+20;5.4;3.4;1.7;0.2;Setosa
+21;5.1;3.7;1.5;0.4;Setosa
+22;4.6;3.6;1.0;0.2;Setosa
+23;5.1;3.3;1.7;0.5;Setosa
+24;4.8;3.4;1.9;0.2;Setosa
+25;5.0;3.0;1.6;0.2;Setosa
+26;5.0;3.4;1.6;0.4;Setosa
+27;5.2;3.5;1.5;0.2;Setosa
+28;5.2;3.4;1.4;0.2;Setosa
+29;4.7;3.2;1.6;0.2;Setosa
+30;4.8;3.1;1.6;0.2;Setosa
+31;5.4;3.4;1.5;0.4;Setosa
+32;5.2;4.1;1.5;0.1;Setosa
+33;5.5;4.2;1.4;0.2;Setosa
+34;4.9;3.1;1.5;0.2;Setosa
+35;5.0;3.2;1.2;0.2;Setosa
+36;5.5;3.5;1.3;0.2;Setosa
+37;4.9;3.6;1.4;0.1;Setosa
+38;4.4;3.0;1.3;0.2;Setosa
+39;5.1;3.4;1.5;0.2;Setosa
+40;5.0;3.5;1.3;0.3;Setosa
+41;4.5;2.3;1.3;0.3;Setosa
+42;4.4;3.2;1.3;0.2;Setosa
+43;5.0;3.5;1.6;0.6;Setosa
+44;5.1;3.8;1.9;0.4;Setosa
+45;4.8;3.0;1.4;0.3;Setosa
+46;5.1;3.8;1.6;0.2;Setosa
+47;4.6;3.2;1.4;0.2;Setosa
+48;5.3;3.7;1.5;0.2;Setosa
+49;5.0;3.3;1.4;0.2;Setosa
+50;7.0;3.2;4.7;1.4;Versicolor
+51;6.4;3.2;4.5;1.5;Versicolor
+52;6.9;3.1;4.9;1.5;Versicolor
+53;5.5;2.3;4.0;1.3;Versicolor
+54;6.5;2.8;4.6;1.5;Versicolor
+55;5.7;2.8;4.5;1.3;Versicolor
+56;6.3;3.3;4.7;1.6;Versicolor
+57;4.9;2.4;3.3;1.0;Versicolor
+58;6.6;2.9;4.6;1.3;Versicolor
+59;5.2;2.7;3.9;1.4;Versicolor
+60;5.0;2.0;3.5;1.0;Versicolor
+61;5.9;3.0;4.2;1.5;Versicolor
+62;6.0;2.2;4.0;1.0;Versicolor
+63;6.1;2.9;4.7;1.4;Versicolor
+64;5.6;2.9;3.6;1.3;Versicolor
+65;6.7;3.1;4.4;1.4;Versicolor
+66;5.6;3.0;4.5;1.5;Versicolor
+67;5.8;2.7;4.1;1.0;Versicolor
+68;6.2;2.2;4.5;1.5;Versicolor
+69;5.6;2.5;3.9;1.1;Versicolor
+70;5.9;3.2;4.8;1.8;Versicolor
+71;6.1;2.8;4.0;1.3;Versicolor
+72;6.3;2.5;4.9;1.5;Versicolor
+73;6.1;2.8;4.7;1.2;Versicolor
+74;6.4;2.9;4.3;1.3;Versicolor
+75;6.6;3.0;4.4;1.4;Versicolor
+76;6.8;2.8;4.8;1.4;Versicolor
+77;6.7;3.0;5.0;1.7;Versicolor
+78;6.0;2.9;4.5;1.5;Versicolor
+79;5.7;2.6;3.5;1.0;Versicolor
+80;5.5;2.4;3.8;1.1;Versicolor
+81;5.5;2.4;3.7;1.0;Versicolor
+82;5.8;2.7;3.9;1.2;Versicolor
+83;6.0;2.7;5.1;1.6;Versicolor
+84;5.4;3.0;4.5;1.5;Versicolor
+85;6.0;3.4;4.5;1.6;Versicolor
+86;6.7;3.1;4.7;1.5;Versicolor
+87;6.3;2.3;4.4;1.3;Versicolor
+88;5.6;3.0;4.1;1.3;Versicolor
+89;5.5;2.5;4.0;1.3;Versicolor
+90;5.5;2.6;4.4;1.2;Versicolor
+91;6.1;3.0;4.6;1.4;Versicolor
+92;5.8;2.6;4.0;1.2;Versicolor
+93;5.0;2.3;3.3;1.0;Versicolor
+94;5.6;2.7;4.2;1.3;Versicolor
+95;5.7;3.0;4.2;1.2;Versicolor
+96;5.7;2.9;4.2;1.3;Versicolor
+97;6.2;2.9;4.3;1.3;Versicolor
+98;5.1;2.5;3.0;1.1;Versicolor
+99;5.7;2.8;4.1;1.3;Versicolor
+100;6.3;3.3;6.0;2.5;Virginica
+101;5.8;2.7;5.1;1.9;Virginica
+102;7.1;3.0;5.9;2.1;Virginica
+103;6.3;2.9;5.6;1.8;Virginica
+104;6.5;3.0;5.8;2.2;Virginica
+105;7.6;3.0;6.6;2.1;Virginica
+106;4.9;2.5;4.5;1.7;Virginica
+107;7.3;2.9;6.3;1.8;Virginica
+108;6.7;2.5;5.8;1.8;Virginica
+109;7.2;3.6;6.1;2.5;Virginica
+110;6.5;3.2;5.1;2.0;Virginica
+111;6.4;2.7;5.3;1.9;Virginica
+112;6.8;3.0;5.5;2.1;Virginica
+113;5.7;2.5;5.0;2.0;Virginica
+114;5.8;2.8;5.1;2.4;Virginica
+115;6.4;3.2;5.3;2.3;Virginica
+116;6.5;3.0;5.5;1.8;Virginica
+117;7.7;3.8;6.7;2.2;Virginica
+118;7.7;2.6;6.9;2.3;Virginica
+119;6.0;2.2;5.0;1.5;Virginica
+120;6.9;3.2;5.7;2.3;Virginica
+121;5.6;2.8;4.9;2.0;Virginica
+122;7.7;2.8;6.7;2.0;Virginica
+123;6.3;2.7;4.9;1.8;Virginica
+124;6.7;3.3;5.7;2.1;Virginica
+125;7.2;3.2;6.0;1.8;Virginica
+126;6.2;2.8;4.8;1.8;Virginica
+127;6.1;3.0;4.9;1.8;Virginica
+128;6.4;2.8;5.6;2.1;Virginica
+129;7.2;3.0;5.8;1.6;Virginica
+130;7.4;2.8;6.1;1.9;Virginica
+131;7.9;3.8;6.4;2.0;Virginica
+132;6.4;2.8;5.6;2.2;Virginica
+133;6.3;2.8;5.1;1.5;Virginica
+134;6.1;2.6;5.6;1.4;Virginica
+135;7.7;3.0;6.1;2.3;Virginica
+136;6.3;3.4;5.6;2.4;Virginica
+137;6.4;3.1;5.5;1.8;Virginica
+138;6.0;3.0;4.8;1.8;Virginica
+139;6.9;3.1;5.4;2.1;Virginica
+140;6.7;3.1;5.6;2.4;Virginica
+141;6.9;3.1;5.1;2.3;Virginica
+142;5.8;2.7;5.1;1.9;Virginica
+143;6.8;3.2;5.9;2.3;Virginica
+144;6.7;3.3;5.7;2.5;Virginica
+145;6.7;3.0;5.2;2.3;Virginica
+146;6.3;2.5;5.0;1.9;Virginica
+147;6.5;3.0;5.2;2.0;Virginica
+148;6.2;3.4;5.4;2.3;Virginica
+149;5.9;3.0;5.1;1.8;Virginica
```

### Comparing `lndb_storage-0.3.2/docs/guide/upload.ipynb` & `lndb_storage-0.4a1/docs/guide/upload.ipynb`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 23% similar despite different names*

```diff
@@ -1,578 +1,551 @@
-00000000: 7b0d 0a20 2263 656c 6c73 223a 205b 0d0a  {.. "cells": [..
-00000010: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-00000020: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
-00000030: 0d0a 2020 2022 6964 223a 2022 6464 3662  ..   "id": "dd6b
-00000040: 6638 6431 2d62 6134 302d 3430 3534 2d39  f8d1-ba40-4054-9
-00000050: 6636 322d 6134 3032 3538 3866 3761 3935  f62-a402588f7a95
-00000060: 222c 0d0a 2020 2022 6d65 7461 6461 7461  ",..   "metadata
-00000070: 223a 207b 7d2c 0d0a 2020 2022 736f 7572  ": {},..   "sour
-00000080: 6365 223a 205b 0d0a 2020 2020 2223 2054  ce": [..    "# T
-00000090: 7261 636b 2066 696c 6573 2c20 696e 2d6d  rack files, in-m
-000000a0: 656d 6f72 7920 6f62 6a65 6374 7320 2620  emory objects & 
-000000b0: 666f 6c64 6572 7320 5b53 3320 7374 6f72  folders [S3 stor
-000000c0: 6167 655d 220d 0a20 2020 5d0d 0a20 207d  age]"..   ]..  }
-000000d0: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
-000000e0: 5f74 7970 6522 3a20 2263 6f64 6522 2c0d  _type": "code",.
-000000f0: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-00000100: 6f75 6e74 223a 206e 756c 6c2c 0d0a 2020  ount": null,..  
-00000110: 2022 6964 223a 2022 3863 3231 6432 3065   "id": "8c21d20e
-00000120: 2d30 6634 652d 3430 3937 2d61 3337 612d  -0f4e-4097-a37a-
-00000130: 6261 3738 3461 6464 6334 3132 222c 0d0a  ba784addc412",..
-00000140: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00000150: 0d0a 2020 2020 2274 6167 7322 3a20 5b0d  ..    "tags": [.
-00000160: 0a20 2020 2020 2268 6964 652d 6365 6c6c  .     "hide-cell
-00000170: 220d 0a20 2020 205d 0d0a 2020 207d 2c0d  "..    ]..   },.
-00000180: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
-00000190: 5d2c 0d0a 2020 2022 736f 7572 6365 223a  ],..   "source":
-000001a0: 205b 0d0a 2020 2020 2221 6c61 6d69 6e20   [..    "!lamin 
-000001b0: 6c6f 6769 6e20 7465 7374 7573 6572 315c  login testuser1\
-000001c0: 6e22 2c0d 0a20 2020 2022 216c 616d 696e  n",..    "!lamin
-000001d0: 206c 6f61 6420 7465 7374 7573 6572 312f   load testuser1/
-000001e0: 6c6e 6462 2d73 746f 7261 6765 5c6e 222c  lndb-storage\n",
-000001f0: 0d0a 2020 2020 2221 6c61 6d69 6e20 6465  ..    "!lamin de
-00000200: 6c65 7465 206c 6e64 622d 7374 6f72 6167  lete lndb-storag
-00000210: 655c 6e22 2c0d 0a20 2020 2022 216c 616d  e\n",..    "!lam
-00000220: 696e 2069 6e69 7420 2d2d 7374 6f72 6167  in init --storag
-00000230: 6520 7333 3a2f 2f6c 616d 696e 6462 2d63  e s3://lamindb-c
-00000240: 6920 2d2d 6e61 6d65 206c 6e64 622d 7374  i --name lndb-st
-00000250: 6f72 6167 6522 0d0a 2020 205d 0d0a 2020  orage"..   ]..  
-00000260: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
-00000270: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
-00000280: 0d0a 2020 2022 6578 6563 7574 696f 6e5f  ..   "execution_
-00000290: 636f 756e 7422 3a20 6e75 6c6c 2c0d 0a20  count": null,.. 
-000002a0: 2020 2269 6422 3a20 2238 6562 3039 3766    "id": "8eb097f
-000002b0: 342d 3431 3134 2d34 6133 352d 3837 3634  4-4114-4a35-8764
-000002c0: 2d65 6263 6665 3165 3835 6264 6322 2c0d  -ebcfe1e85bdc",.
-000002d0: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-000002e0: 7b7d 2c0d 0a20 2020 226f 7574 7075 7473  {},..   "outputs
-000002f0: 223a 205b 5d2c 0d0a 2020 2022 736f 7572  ": [],..   "sour
-00000300: 6365 223a 205b 0d0a 2020 2020 2269 6d70  ce": [..    "imp
-00000310: 6f72 7420 6c61 6d69 6e64 6220 6173 206c  ort lamindb as l
-00000320: 6e5c 6e22 2c0d 0a20 2020 2022 696d 706f  n\n",..    "impo
-00000330: 7274 2070 7974 6573 745c 6e22 2c0d 0a20  rt pytest\n",.. 
-00000340: 2020 2022 5c6e 222c 0d0a 2020 2020 226c     "\n",..    "l
-00000350: 6e2e 7472 6163 6b28 2922 0d0a 2020 205d  n.track()"..   ]
-00000360: 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20 2020  ..  },..  {..   
-00000370: 2263 656c 6c5f 7479 7065 223a 2022 6d61  "cell_type": "ma
-00000380: 726b 646f 776e 222c 0d0a 2020 2022 6964  rkdown",..   "id
-00000390: 223a 2022 6262 3935 6162 6537 222c 0d0a  ": "bb95abe7",..
-000003a0: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-000003b0: 7d2c 0d0a 2020 2022 736f 7572 6365 223a  },..   "source":
-000003c0: 205b 0d0a 2020 2020 2223 2320 4c6f 6361   [..    "## Loca
-000003d0: 6c20 6669 6c65 7322 0d0a 2020 205d 0d0a  l files"..   ]..
-000003e0: 2020 7d2c 0d0a 2020 7b0d 0a20 2020 2263    },..  {..   "c
-000003f0: 656c 6c5f 7479 7065 223a 2022 6d61 726b  ell_type": "mark
-00000400: 646f 776e 222c 0d0a 2020 2022 6964 223a  down",..   "id":
-00000410: 2022 6231 3132 3135 6166 2d62 6237 662d   "b11215af-bb7f-
-00000420: 3439 3332 2d38 3365 652d 3866 3436 6635  4932-83ee-8f46f5
-00000430: 3538 3365 6438 222c 0d0a 2020 2022 6d65  583ed8",..   "me
-00000440: 7461 6461 7461 223a 207b 7d2c 0d0a 2020  tadata": {},..  
-00000450: 2022 736f 7572 6365 223a 205b 0d0a 2020   "source": [..  
-00000460: 2020 2253 6f6d 6520 7465 7374 2064 6174    "Some test dat
-00000470: 612e 220d 0a20 2020 5d0d 0a20 207d 2c0d  a."..   ]..  },.
-00000480: 0a20 207b 0d0a 2020 2022 6365 6c6c 5f74  .  {..   "cell_t
-00000490: 7970 6522 3a20 2263 6f64 6522 2c0d 0a20  ype": "code",.. 
-000004a0: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
-000004b0: 6e74 223a 206e 756c 6c2c 0d0a 2020 2022  nt": null,..   "
-000004c0: 6964 223a 2022 3037 3733 3434 6132 2d34  id": "077344a2-4
-000004d0: 6631 382d 3437 6339 2d62 3861 352d 6333  f18-47c9-b8a5-c3
-000004e0: 6336 3431 3135 3131 6462 222c 0d0a 2020  c6411511db",..  
-000004f0: 2022 6d65 7461 6461 7461 223a 207b 7d2c   "metadata": {},
-00000500: 0d0a 2020 2022 6f75 7470 7574 7322 3a20  ..   "outputs": 
-00000510: 5b5d 2c0d 0a20 2020 2273 6f75 7263 6522  [],..   "source"
-00000520: 3a20 5b0d 0a20 2020 2022 7062 6d63 3638  : [..    "pbmc68
-00000530: 6b20 3d20 6c6e 2e64 6576 2e64 6174 6173  k = ln.dev.datas
-00000540: 6574 732e 616e 6e64 6174 615f 7062 6d63  ets.anndata_pbmc
-00000550: 3638 6b5f 7265 6475 6365 6428 2922 0d0a  68k_reduced()"..
-00000560: 2020 205d 0d0a 2020 7d2c 0d0a 2020 7b0d     ]..  },..  {.
-00000570: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00000580: 2022 6d61 726b 646f 776e 222c 0d0a 2020   "markdown",..  
-00000590: 2022 6964 223a 2022 3761 6633 6430 3564   "id": "7af3d05d
-000005a0: 2d38 6463 332d 3435 3564 2d62 6531 622d  -8dc3-455d-be1b-
-000005b0: 3833 6537 3938 3632 3130 3531 222c 0d0a  83e798621051",..
-000005c0: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-000005d0: 7d2c 0d0a 2020 2022 736f 7572 6365 223a  },..   "source":
-000005e0: 205b 0d0a 2020 2020 2253 7562 7365 7420   [..    "Subset 
-000005f0: 746f 2061 206d 696e 6920 6669 6c65 2074  to a mini file t
-00000600: 6f20 7370 6565 6420 7570 2074 6865 2072  o speed up the r
-00000610: 756e 2074 696d 6520 6f66 2074 6869 7320  un time of this 
-00000620: 6e6f 7465 626f 6f6b 3a22 0d0a 2020 205d  notebook:"..   ]
-00000630: 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20 2020  ..  },..  {..   
-00000640: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
-00000650: 6465 222c 0d0a 2020 2022 6578 6563 7574  de",..   "execut
-00000660: 696f 6e5f 636f 756e 7422 3a20 6e75 6c6c  ion_count": null
-00000670: 2c0d 0a20 2020 2269 6422 3a20 2236 3134  ,..   "id": "614
-00000680: 6138 3736 362d 6235 3934 2d34 3537 382d  a8766-b594-4578-
-00000690: 6131 3633 2d32 3439 3738 3335 6363 3962  a163-2497835cc9b
-000006a0: 3422 2c0d 0a20 2020 226d 6574 6164 6174  4",..   "metadat
-000006b0: 6122 3a20 7b7d 2c0d 0a20 2020 226f 7574  a": {},..   "out
-000006c0: 7075 7473 223a 205b 5d2c 0d0a 2020 2022  puts": [],..   "
-000006d0: 736f 7572 6365 223a 205b 0d0a 2020 2020  source": [..    
-000006e0: 2270 626d 6336 386b 203d 2070 626d 6336  "pbmc68k = pbmc6
-000006f0: 386b 5b3a 352c 203a 355d 2e63 6f70 7928  8k[:5, :5].copy(
-00000700: 2922 0d0a 2020 205d 0d0a 2020 7d2c 0d0a  )"..   ]..  },..
-00000710: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-00000720: 7065 223a 2022 636f 6465 222c 0d0a 2020  pe": "code",..  
-00000730: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
-00000740: 7422 3a20 6e75 6c6c 2c0d 0a20 2020 2269  t": null,..   "i
-00000750: 6422 3a20 2234 3233 3462 6234 322d 3033  d": "4234bb42-03
-00000760: 6532 2d34 3637 362d 6136 3734 2d39 3238  e2-4676-a674-928
-00000770: 3165 6232 3935 6466 3722 2c0d 0a20 2020  1eb295df7",..   
-00000780: 226d 6574 6164 6174 6122 3a20 7b7d 2c0d  "metadata": {},.
-00000790: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
-000007a0: 5d2c 0d0a 2020 2022 736f 7572 6365 223a  ],..   "source":
-000007b0: 205b 0d0a 2020 2020 2270 626d 6336 386b   [..    "pbmc68k
-000007c0: 220d 0a20 2020 5d0d 0a20 207d 2c0d 0a20  "..   ]..  },.. 
-000007d0: 207b 0d0a 2020 2022 6365 6c6c 5f74 7970   {..   "cell_typ
-000007e0: 6522 3a20 226d 6172 6b64 6f77 6e22 2c0d  e": "markdown",.
-000007f0: 0a20 2020 2269 6422 3a20 2236 3232 6238  .   "id": "622b8
-00000800: 3031 322d 3661 3934 2d34 6134 312d 3861  012-6a94-4a41-8a
-00000810: 3662 2d34 6331 3738 6564 3463 6661 3622  6b-4c178ed4cfa6"
-00000820: 2c0d 0a20 2020 226d 6574 6164 6174 6122  ,..   "metadata"
-00000830: 3a20 7b7d 2c0d 0a20 2020 2273 6f75 7263  : {},..   "sourc
-00000840: 6522 3a20 5b0d 0a20 2020 2022 2323 2320  e": [..    "### 
-00000850: 2055 706c 6f61 6420 6672 6f6d 206d 656d   Upload from mem
-00000860: 6f72 7920 7573 696e 6720 6578 706c 6963  ory using explic
-00000870: 6974 2073 656d 616e 7469 6320 606b 6579  it semantic `key
-00000880: 6022 0d0a 2020 205d 0d0a 2020 7d2c 0d0a  `"..   ]..  },..
-00000890: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-000008a0: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
-000008b0: 0d0a 2020 2022 6964 223a 2022 3831 3338  ..   "id": "8138
-000008c0: 6138 3837 2d32 6465 382d 3461 6439 2d61  a887-2de8-4ad9-a
-000008d0: 6438 622d 3633 3332 3432 3633 6662 3764  d8b-63324263fb7d
-000008e0: 222c 0d0a 2020 2022 6d65 7461 6461 7461  ",..   "metadata
-000008f0: 223a 207b 7d2c 0d0a 2020 2022 736f 7572  ": {},..   "sour
-00000900: 6365 223a 205b 0d0a 2020 2020 2223 2323  ce": [..    "###
-00000910: 2320 5570 6c6f 6164 2068 3561 6422 0d0a  # Upload h5ad"..
-00000920: 2020 205d 0d0a 2020 7d2c 0d0a 2020 7b0d     ]..  },..  {.
-00000930: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00000940: 2022 636f 6465 222c 0d0a 2020 2022 6578   "code",..   "ex
-00000950: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-00000960: 6e75 6c6c 2c0d 0a20 2020 2269 6422 3a20  null,..   "id": 
-00000970: 2266 6366 6637 3237 322d 3133 6466 2d34  "fcff7272-13df-4
-00000980: 3666 392d 6162 3633 2d32 3539 3231 6135  6f9-ab63-25921a5
-00000990: 3037 6639 3822 2c0d 0a20 2020 226d 6574  07f98",..   "met
-000009a0: 6164 6174 6122 3a20 7b7d 2c0d 0a20 2020  adata": {},..   
-000009b0: 226f 7574 7075 7473 223a 205b 5d2c 0d0a  "outputs": [],..
-000009c0: 2020 2022 736f 7572 6365 223a 205b 0d0a     "source": [..
-000009d0: 2020 2020 2270 626d 6336 386b 5f68 3561      "pbmc68k_h5a
-000009e0: 6420 3d20 6c6e 2e46 696c 6528 7062 6d63  d = ln.File(pbmc
-000009f0: 3638 6b2c 206b 6579 3d5c 2274 6573 742d  68k, key=\"test-
-00000a00: 7570 6c6f 6164 2f70 626d 6336 386b 2e68  upload/pbmc68k.h
-00000a10: 3561 645c 2229 220d 0a20 2020 5d0d 0a20  5ad\")"..   ].. 
-00000a20: 207d 2c0d 0a20 207b 0d0a 2020 2022 6365   },..  {..   "ce
-00000a30: 6c6c 5f74 7970 6522 3a20 2263 6f64 6522  ll_type": "code"
-00000a40: 2c0d 0a20 2020 2265 7865 6375 7469 6f6e  ,..   "execution
-00000a50: 5f63 6f75 6e74 223a 206e 756c 6c2c 0d0a  _count": null,..
-00000a60: 2020 2022 6964 223a 2022 6139 3736 3137     "id": "a97617
-00000a70: 6664 2d30 6634 312d 3433 6631 2d39 3931  fd-0f41-43f1-991
-00000a80: 392d 3235 6163 6162 3364 6630 6335 222c  9-25acab3df0c5",
-00000a90: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
-00000aa0: 207b 7d2c 0d0a 2020 2022 6f75 7470 7574   {},..   "output
-00000ab0: 7322 3a20 5b5d 2c0d 0a20 2020 2273 6f75  s": [],..   "sou
-00000ac0: 7263 6522 3a20 5b0d 0a20 2020 2022 7062  rce": [..    "pb
-00000ad0: 6d63 3638 6b5f 6835 6164 203d 206c 6e2e  mc68k_h5ad = ln.
-00000ae0: 6164 6428 7062 6d63 3638 6b5f 6835 6164  add(pbmc68k_h5ad
-00000af0: 2922 0d0a 2020 205d 0d0a 2020 7d2c 0d0a  )"..   ]..  },..
-00000b00: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-00000b10: 7065 223a 2022 636f 6465 222c 0d0a 2020  pe": "code",..  
-00000b20: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
-00000b30: 7422 3a20 6e75 6c6c 2c0d 0a20 2020 2269  t": null,..   "i
-00000b40: 6422 3a20 2231 3462 3133 3963 332d 6662  d": "14b139c3-fb
-00000b50: 3165 2d34 6363 612d 6137 3561 2d38 6564  1e-4cca-a75a-8ed
-00000b60: 3739 3863 3138 3961 3822 2c0d 0a20 2020  798c189a8",..   
-00000b70: 226d 6574 6164 6174 6122 3a20 7b7d 2c0d  "metadata": {},.
-00000b80: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
-00000b90: 5d2c 0d0a 2020 2022 736f 7572 6365 223a  ],..   "source":
-00000ba0: 205b 0d0a 2020 2020 226c 6e2e 6465 6c65   [..    "ln.dele
-00000bb0: 7465 2870 626d 6336 386b 5f68 3561 642c  te(pbmc68k_h5ad,
-00000bc0: 2064 656c 6574 655f 6461 7461 5f66 726f   delete_data_fro
-00000bd0: 6d5f 7374 6f72 6167 653d 5472 7565 2922  m_storage=True)"
-00000be0: 0d0a 2020 205d 0d0a 2020 7d2c 0d0a 2020  ..   ]..  },..  
-00000bf0: 7b0d 0a20 2020 2263 656c 6c5f 7479 7065  {..   "cell_type
-00000c00: 223a 2022 6d61 726b 646f 776e 222c 0d0a  ": "markdown",..
-00000c10: 2020 2022 6964 223a 2022 6666 3065 3334     "id": "ff0e34
-00000c20: 6364 2d38 6562 642d 3431 3936 2d61 3762  cd-8ebd-4196-a7b
-00000c30: 642d 6136 3637 6232 6133 3630 6131 222c  d-a667b2a360a1",
-00000c40: 0d0a 2020 2022 6d65 7461 6461 7461 223a  ..   "metadata":
-00000c50: 207b 7d2c 0d0a 2020 2022 736f 7572 6365   {},..   "source
-00000c60: 223a 205b 0d0a 2020 2020 2223 2323 2320  ": [..    "#### 
-00000c70: 5570 6c6f 6164 207a 6172 7222 0d0a 2020  Upload zarr"..  
-00000c80: 205d 0d0a 2020 7d2c 0d0a 2020 7b0d 0a20   ]..  },..  {.. 
-00000c90: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
-00000ca0: 636f 6465 222c 0d0a 2020 2022 6578 6563  code",..   "exec
-00000cb0: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
-00000cc0: 6c6c 2c0d 0a20 2020 2269 6422 3a20 2262  ll,..   "id": "b
-00000cd0: 3636 6563 3061 662d 3963 3933 2d34 3338  66ec0af-9c93-438
-00000ce0: 612d 3832 3830 2d64 3933 6665 3635 3762  a-8280-d93fe657b
-00000cf0: 6266 6222 2c0d 0a20 2020 226d 6574 6164  bfb",..   "metad
-00000d00: 6174 6122 3a20 7b7d 2c0d 0a20 2020 226f  ata": {},..   "o
-00000d10: 7574 7075 7473 223a 205b 5d2c 0d0a 2020  utputs": [],..  
-00000d20: 2022 736f 7572 6365 223a 205b 0d0a 2020   "source": [..  
-00000d30: 2020 2223 2052 756e 7320 746f 6f20 6c6f    "# Runs too lo
-00000d40: 6e67 2c20 7368 6f75 6c64 2062 6520 7465  ng, should be te
-00000d50: 7374 6564 2065 6c73 6577 6865 7265 5c6e  sted elsewhere\n
-00000d60: 222c 0d0a 2020 2020 2223 2070 626d 6336  ",..    "# pbmc6
-00000d70: 386b 5f7a 6172 7220 3d20 6c6e 2e46 696c  8k_zarr = ln.Fil
-00000d80: 6528 7062 6d63 3638 6b2c 206b 6579 3d5c  e(pbmc68k, key=\
-00000d90: 2274 6573 742d 7570 6c6f 6164 2f70 626d  "test-upload/pbm
-00000da0: 6336 386b 2e7a 6172 725c 222c 2066 6f72  c68k.zarr\", for
-00000db0: 6d61 743d 5c22 7a61 7272 5c22 295c 6e22  mat=\"zarr\")\n"
-00000dc0: 2c0d 0a20 2020 2022 2320 7062 6d63 3638  ,..    "# pbmc68
-00000dd0: 6b5f 7a61 7272 203d 206c 6e2e 6164 6428  k_zarr = ln.add(
-00000de0: 7062 6d63 3638 6b5f 7a61 7272 295c 6e22  pbmc68k_zarr)\n"
-00000df0: 2c0d 0a20 2020 2022 2320 6c6e 2e64 656c  ,..    "# ln.del
-00000e00: 6574 6528 7062 6d63 3638 6b5f 7a61 7272  ete(pbmc68k_zarr
-00000e10: 2c20 6465 6c65 7465 5f64 6174 615f 6672  , delete_data_fr
-00000e20: 6f6d 5f73 746f 7261 6765 3d54 7275 6529  om_storage=True)
-00000e30: 220d 0a20 2020 5d0d 0a20 207d 2c0d 0a20  "..   ]..  },.. 
-00000e40: 207b 0d0a 2020 2022 6365 6c6c 5f74 7970   {..   "cell_typ
-00000e50: 6522 3a20 226d 6172 6b64 6f77 6e22 2c0d  e": "markdown",.
-00000e60: 0a20 2020 2269 6422 3a20 2263 3535 3261  .   "id": "c552a
-00000e70: 6639 302d 6234 6233 2d34 3436 352d 6161  f90-b4b3-4465-aa
-00000e80: 6563 2d36 3632 3934 3964 3438 3062 3322  ec-662949d480b3"
-00000e90: 2c0d 0a20 2020 226d 6574 6164 6174 6122  ,..   "metadata"
-00000ea0: 3a20 7b7d 2c0d 0a20 2020 2273 6f75 7263  : {},..   "sourc
-00000eb0: 6522 3a20 5b0d 0a20 2020 2022 2323 2320  e": [..    "### 
-00000ec0: 5570 6c6f 6164 2075 7369 6e67 2060 6964  Upload using `id
-00000ed0: 6020 7769 7468 2069 6d70 6c69 6369 7420  ` with implicit 
-00000ee0: 606b 6579 6022 0d0a 2020 205d 0d0a 2020  `key`"..   ]..  
-00000ef0: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
-00000f00: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
-00000f10: 776e 222c 0d0a 2020 2022 6964 223a 2022  wn",..   "id": "
-00000f20: 3661 6331 3666 3862 2d33 3935 322d 3436  6ac16f8b-3952-46
-00000f30: 3962 2d39 6236 632d 3361 3738 6330 3936  9b-9b6c-3a78c096
-00000f40: 3436 3763 222c 0d0a 2020 2022 6d65 7461  467c",..   "meta
-00000f50: 6461 7461 223a 207b 7d2c 0d0a 2020 2022  data": {},..   "
-00000f60: 736f 7572 6365 223a 205b 0d0a 2020 2020  source": [..    
-00000f70: 2223 2323 2320 5570 6c6f 6164 2068 3561  "#### Upload h5a
-00000f80: 6422 0d0a 2020 205d 0d0a 2020 7d2c 0d0a  d"..   ]..  },..
-00000f90: 2020 7b0d 0a20 2020 2263 656c 6c5f 7479    {..   "cell_ty
-00000fa0: 7065 223a 2022 636f 6465 222c 0d0a 2020  pe": "code",..  
-00000fb0: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
-00000fc0: 7422 3a20 6e75 6c6c 2c0d 0a20 2020 2269  t": null,..   "i
-00000fd0: 6422 3a20 2232 3536 3735 6565 622d 6233  d": "25675eeb-b3
-00000fe0: 3339 2d34 3463 372d 3931 3138 2d36 3137  39-44c7-9118-617
-00000ff0: 3862 3333 3531 3130 3022 2c0d 0a20 2020  8b3351100",..   
-00001000: 226d 6574 6164 6174 6122 3a20 7b7d 2c0d  "metadata": {},.
-00001010: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
-00001020: 5d2c 0d0a 2020 2022 736f 7572 6365 223a  ],..   "source":
-00001030: 205b 0d0a 2020 2020 2270 626d 6336 386b   [..    "pbmc68k
-00001040: 5f68 3561 6420 3d20 6c6e 2e46 696c 6528  _h5ad = ln.File(
-00001050: 7062 6d63 3638 6b2c 206e 616d 653d 5c22  pbmc68k, name=\"
-00001060: 7062 6d63 3638 6b2e 6835 6164 5c22 2922  pbmc68k.h5ad\")"
-00001070: 0d0a 2020 205d 0d0a 2020 7d2c 0d0a 2020  ..   ]..  },..  
-00001080: 7b0d 0a20 2020 2263 656c 6c5f 7479 7065  {..   "cell_type
-00001090: 223a 2022 636f 6465 222c 0d0a 2020 2022  ": "code",..   "
-000010a0: 6578 6563 7574 696f 6e5f 636f 756e 7422  execution_count"
-000010b0: 3a20 6e75 6c6c 2c0d 0a20 2020 2269 6422  : null,..   "id"
-000010c0: 3a20 2236 3331 3465 3862 312d 6363 6633  : "6314e8b1-ccf3
-000010d0: 2d34 3637 662d 6136 6530 2d34 3638 3766  -467f-a6e0-4687f
-000010e0: 3532 6431 3033 3322 2c0d 0a20 2020 226d  52d1033",..   "m
-000010f0: 6574 6164 6174 6122 3a20 7b7d 2c0d 0a20  etadata": {},.. 
-00001100: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
-00001110: 0d0a 2020 2022 736f 7572 6365 223a 205b  ..   "source": [
-00001120: 0d0a 2020 2020 2270 626d 6336 386b 5f68  ..    "pbmc68k_h
-00001130: 3561 6420 3d20 6c6e 2e61 6464 2870 626d  5ad = ln.add(pbm
-00001140: 6336 386b 5f68 3561 6429 220d 0a20 2020  c68k_h5ad)"..   
-00001150: 5d0d 0a20 207d 2c0d 0a20 207b 0d0a 2020  ]..  },..  {..  
-00001160: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
-00001170: 6f64 6522 2c0d 0a20 2020 2265 7865 6375  ode",..   "execu
-00001180: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
-00001190: 6c2c 0d0a 2020 2022 6964 223a 2022 3037  l,..   "id": "07
-000011a0: 6538 6536 3136 2d38 3964 662d 3433 3364  e8e616-89df-433d
-000011b0: 2d38 3961 372d 6139 6338 6165 6438 3930  -89a7-a9c8aed890
-000011c0: 6365 222c 0d0a 2020 2022 6d65 7461 6461  ce",..   "metada
-000011d0: 7461 223a 207b 7d2c 0d0a 2020 2022 6f75  ta": {},..   "ou
-000011e0: 7470 7574 7322 3a20 5b5d 2c0d 0a20 2020  tputs": [],..   
-000011f0: 2273 6f75 7263 6522 3a20 5b0d 0a20 2020  "source": [..   
-00001200: 2022 6c6e 2e64 656c 6574 6528 7062 6d63   "ln.delete(pbmc
-00001210: 3638 6b5f 6835 6164 2c20 6465 6c65 7465  68k_h5ad, delete
-00001220: 5f64 6174 615f 6672 6f6d 5f73 746f 7261  _data_from_stora
-00001230: 6765 3d54 7275 6529 220d 0a20 2020 5d0d  ge=True)"..   ].
-00001240: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-00001250: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-00001260: 6b64 6f77 6e22 2c0d 0a20 2020 2269 6422  kdown",..   "id"
-00001270: 3a20 2238 6264 3564 6135 392d 6336 3136  : "8bd5da59-c616
-00001280: 2d34 6534 392d 3966 3032 2d66 3438 3134  -4e49-9f02-f4814
-00001290: 6331 3930 3332 6622 2c0d 0a20 2020 226d  c19032f",..   "m
-000012a0: 6574 6164 6174 6122 3a20 7b7d 2c0d 0a20  etadata": {},.. 
-000012b0: 2020 2273 6f75 7263 6522 3a20 5b0d 0a20    "source": [.. 
-000012c0: 2020 2022 2323 2323 2055 706c 6f61 6420     "#### Upload 
-000012d0: 7a61 7272 220d 0a20 2020 5d0d 0a20 207d  zarr"..   ]..  }
-000012e0: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
-000012f0: 5f74 7970 6522 3a20 2263 6f64 6522 2c0d  _type": "code",.
-00001300: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-00001310: 6f75 6e74 223a 206e 756c 6c2c 0d0a 2020  ount": null,..  
-00001320: 2022 6964 223a 2022 3265 3665 3361 6530   "id": "2e6e3ae0
-00001330: 2d35 6261 392d 3433 3132 2d61 3930 322d  -5ba9-4312-a902-
-00001340: 6630 3237 3864 3165 6664 6663 222c 0d0a  f0278d1efdfc",..
-00001350: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00001360: 7d2c 0d0a 2020 2022 6f75 7470 7574 7322  },..   "outputs"
-00001370: 3a20 5b5d 2c0d 0a20 2020 2273 6f75 7263  : [],..   "sourc
-00001380: 6522 3a20 5b0d 0a20 2020 2022 2320 5275  e": [..    "# Ru
-00001390: 6e73 2074 6f6f 206c 6f6e 672c 2073 686f  ns too long, sho
-000013a0: 756c 6420 6265 2074 6573 7465 6420 656c  uld be tested el
-000013b0: 7365 7768 6572 655c 6e22 2c0d 0a20 2020  sewhere\n",..   
-000013c0: 2022 2320 7062 6d63 3638 6b5f 7a61 7272   "# pbmc68k_zarr
-000013d0: 203d 206c 6e2e 4669 6c65 2870 626d 6336   = ln.File(pbmc6
-000013e0: 386b 2c20 6e61 6d65 3d5c 2270 626d 6336  8k, name=\"pbmc6
-000013f0: 386b 2e7a 6172 725c 222c 2066 6f72 6d61  8k.zarr\", forma
-00001400: 743d 5c22 7a61 7272 5c22 295c 6e22 2c0d  t=\"zarr\")\n",.
-00001410: 0a20 2020 2022 2320 7062 6d63 3638 6b5f  .    "# pbmc68k_
-00001420: 7a61 7272 203d 206c 6e2e 6164 6428 7062  zarr = ln.add(pb
-00001430: 6d63 3638 6b5f 7a61 7272 295c 6e22 2c0d  mc68k_zarr)\n",.
-00001440: 0a20 2020 2022 2320 6c6e 2e64 656c 6574  .    "# ln.delet
-00001450: 6528 7062 6d63 3638 6b5f 7a61 7272 2c20  e(pbmc68k_zarr, 
-00001460: 6465 6c65 7465 5f64 6174 615f 6672 6f6d  delete_data_from
-00001470: 5f73 746f 7261 6765 3d54 7275 6529 220d  _storage=True)".
-00001480: 0a20 2020 5d0d 0a20 207d 2c0d 0a20 207b  .   ]..  },..  {
-00001490: 0d0a 2020 2022 6365 6c6c 5f74 7970 6522  ..   "cell_type"
-000014a0: 3a20 226d 6172 6b64 6f77 6e22 2c0d 0a20  : "markdown",.. 
-000014b0: 2020 2269 6422 3a20 2230 3661 3931 6439    "id": "06a91d9
-000014c0: 392d 6432 3034 2d34 6563 322d 6235 3637  9-d204-4ec2-b567
-000014d0: 2d39 3630 6132 6161 6164 3338 6422 2c0d  -960a2aaad38d",.
-000014e0: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-000014f0: 7b0d 0a20 2020 2022 7461 6773 223a 205b  {..    "tags": [
-00001500: 5d0d 0a20 2020 7d2c 0d0a 2020 2022 736f  ]..   },..   "so
-00001510: 7572 6365 223a 205b 0d0a 2020 2020 2223  urce": [..    "#
-00001520: 2323 2045 7272 6f72 2062 6568 6176 696f  ## Error behavio
-00001530: 7273 220d 0a20 2020 5d0d 0a20 207d 2c0d  rs"..   ]..  },.
-00001540: 0a20 207b 0d0a 2020 2022 6365 6c6c 5f74  .  {..   "cell_t
-00001550: 7970 6522 3a20 226d 6172 6b64 6f77 6e22  ype": "markdown"
-00001560: 2c0d 0a20 2020 2269 6422 3a20 2266 3736  ,..   "id": "f76
-00001570: 3063 6261 302d 3338 6130 2d34 6265 322d  0cba0-38a0-4be2-
-00001580: 3838 3534 2d64 3166 3137 3638 3964 6530  8854-d1f17689de0
-00001590: 3522 2c0d 0a20 2020 226d 6574 6164 6174  5",..   "metadat
-000015a0: 6122 3a20 7b7d 2c0d 0a20 2020 2273 6f75  a": {},..   "sou
-000015b0: 7263 6522 3a20 5b0d 0a20 2020 2022 5370  rce": [..    "Sp
-000015c0: 6563 6966 6965 6420 6275 636b 6574 2064  ecified bucket d
-000015d0: 6f65 7320 6e6f 7420 6578 6973 742e 220d  oes not exist.".
-000015e0: 0a20 2020 5d0d 0a20 207d 2c0d 0a20 207b  .   ]..  },..  {
-000015f0: 0d0a 2020 2022 6365 6c6c 5f74 7970 6522  ..   "cell_type"
-00001600: 3a20 2263 6f64 6522 2c0d 0a20 2020 2265  : "code",..   "e
-00001610: 7865 6375 7469 6f6e 5f63 6f75 6e74 223a  xecution_count":
-00001620: 206e 756c 6c2c 0d0a 2020 2022 6964 223a   null,..   "id":
-00001630: 2022 6465 3266 3963 3762 2d39 3934 632d   "de2f9c7b-994c-
-00001640: 3431 3761 2d61 3730 302d 6635 3137 6132  417a-a700-f517a2
-00001650: 3964 6637 3865 222c 0d0a 2020 2022 6d65  9df78e",..   "me
-00001660: 7461 6461 7461 223a 207b 7d2c 0d0a 2020  tadata": {},..  
-00001670: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0d   "outputs": [],.
-00001680: 0a20 2020 2273 6f75 7263 6522 3a20 5b0d  .   "source": [.
-00001690: 0a20 2020 2022 7769 7468 2070 7974 6573  .    "with pytes
-000016a0: 742e 7261 6973 6573 2846 696c 654e 6f74  t.raises(FileNot
-000016b0: 466f 756e 6445 7272 6f72 293a 5c6e 222c  FoundError):\n",
-000016c0: 0d0a 2020 2020 2220 2020 2070 626d 6336  ..    "    pbmc6
-000016d0: 386b 5f68 3561 6420 3d20 6c6e 2e46 696c  8k_h5ad = ln.Fil
-000016e0: 6528 5c22 7333 3a2f 2f69 6e65 7869 7374  e(\"s3://inexist
-000016f0: 656e 742d 6275 636b 6574 2d32 3339 3830  ent-bucket-23980
-00001700: 3938 3334 2f70 626d 6336 386b 2e68 3561  9834/pbmc68k.h5a
-00001710: 645c 2229 220d 0a20 2020 5d0d 0a20 207d  d\")"..   ]..  }
-00001720: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
-00001730: 5f74 7970 6522 3a20 2263 6f64 6522 2c0d  _type": "code",.
-00001740: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-00001750: 6f75 6e74 223a 206e 756c 6c2c 0d0a 2020  ount": null,..  
-00001760: 2022 6964 223a 2022 3133 3835 3063 3863   "id": "13850c8c
-00001770: 2d36 3534 332d 3463 6634 2d62 3861 652d  -6543-4cf4-b8ae-
-00001780: 6463 3061 3030 3330 3065 3266 222c 0d0a  dc0a00300e2f",..
+00000000: 7b0a 2022 6365 6c6c 7322 3a20 5b0a 2020  {. "cells": [.  
+00000010: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00000020: 3a20 226d 6172 6b64 6f77 6e22 2c0a 2020  : "markdown",.  
+00000030: 2022 6964 223a 2022 6464 3662 6638 6431   "id": "dd6bf8d1
+00000040: 2d62 6134 302d 3430 3534 2d39 6636 322d  -ba40-4054-9f62-
+00000050: 6134 3032 3538 3866 3761 3935 222c 0a20  a402588f7a95",. 
+00000060: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
+00000070: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
+00000080: 0a20 2020 2022 2320 5472 6163 6b20 6669  .    "# Track fi
+00000090: 6c65 732c 2069 6e2d 6d65 6d6f 7279 206f  les, in-memory o
+000000a0: 626a 6563 7473 2026 2066 6f6c 6465 7273  bjects & folders
+000000b0: 205b 5333 2073 746f 7261 6765 5d22 0a20   [S3 storage]". 
+000000c0: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+000000d0: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
+000000e0: 6465 222c 0a20 2020 2265 7865 6375 7469  de",.   "executi
+000000f0: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
+00000100: 0a20 2020 2269 6422 3a20 2238 6332 3164  .   "id": "8c21d
+00000110: 3230 652d 3066 3465 2d34 3039 372d 6133  20e-0f4e-4097-a3
+00000120: 3761 2d62 6137 3834 6164 6463 3431 3222  7a-ba784addc412"
+00000130: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+00000140: 207b 0a20 2020 2022 7461 6773 223a 205b   {.    "tags": [
+00000150: 0a20 2020 2020 2268 6964 652d 6365 6c6c  .     "hide-cell
+00000160: 220a 2020 2020 5d0a 2020 207d 2c0a 2020  ".    ].   },.  
+00000170: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
+00000180: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
+00000190: 2020 2022 216c 616d 696e 206c 6f67 696e     "!lamin login
+000001a0: 2074 6573 7475 7365 7231 5c6e 222c 0a20   testuser1\n",. 
+000001b0: 2020 2022 216c 616d 696e 206c 6f61 6420     "!lamin load 
+000001c0: 7465 7374 7573 6572 312f 6c6e 6462 2d73  testuser1/lndb-s
+000001d0: 746f 7261 6765 5c6e 222c 0a20 2020 2022  torage\n",.    "
+000001e0: 216c 616d 696e 2064 656c 6574 6520 6c6e  !lamin delete ln
+000001f0: 6462 2d73 746f 7261 6765 5c6e 222c 0a20  db-storage\n",. 
+00000200: 2020 2022 216c 616d 696e 2069 6e69 7420     "!lamin init 
+00000210: 2d2d 7374 6f72 6167 6520 7333 3a2f 2f6c  --storage s3://l
+00000220: 616d 696e 6462 2d63 6920 2d2d 6e61 6d65  amindb-ci --name
+00000230: 206c 6e64 622d 7374 6f72 6167 6522 0a20   lndb-storage". 
+00000240: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+00000250: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
+00000260: 6465 222c 0a20 2020 2265 7865 6375 7469  de",.   "executi
+00000270: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
+00000280: 0a20 2020 2269 6422 3a20 2238 6562 3039  .   "id": "8eb09
+00000290: 3766 342d 3431 3134 2d34 6133 352d 3837  7f4-4114-4a35-87
+000002a0: 3634 2d65 6263 6665 3165 3835 6264 6322  64-ebcfe1e85bdc"
+000002b0: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+000002c0: 207b 7d2c 0a20 2020 226f 7574 7075 7473   {},.   "outputs
+000002d0: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
+000002e0: 6522 3a20 5b0a 2020 2020 2269 6d70 6f72  e": [.    "impor
+000002f0: 7420 6c61 6d69 6e64 6220 6173 206c 6e5c  t lamindb as ln\
+00000300: 6e22 2c0a 2020 2020 2269 6d70 6f72 7420  n",.    "import 
+00000310: 7079 7465 7374 5c6e 222c 0a20 2020 2022  pytest\n",.    "
+00000320: 5c6e 222c 0a20 2020 2022 6c6e 2e74 7261  \n",.    "ln.tra
+00000330: 636b 2829 220a 2020 205d 0a20 207d 2c0a  ck()".   ].  },.
+00000340: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
+00000350: 6522 3a20 226d 6172 6b64 6f77 6e22 2c0a  e": "markdown",.
+00000360: 2020 2022 6964 223a 2022 6262 3935 6162     "id": "bb95ab
+00000370: 6537 222c 0a20 2020 226d 6574 6164 6174  e7",.   "metadat
+00000380: 6122 3a20 7b7d 2c0a 2020 2022 736f 7572  a": {},.   "sour
+00000390: 6365 223a 205b 0a20 2020 2022 2323 204c  ce": [.    "## L
+000003a0: 6f63 616c 2066 696c 6573 220a 2020 205d  ocal files".   ]
+000003b0: 0a20 207d 2c0a 2020 7b0a 2020 2022 6365  .  },.  {.   "ce
+000003c0: 6c6c 5f74 7970 6522 3a20 226d 6172 6b64  ll_type": "markd
+000003d0: 6f77 6e22 2c0a 2020 2022 6964 223a 2022  own",.   "id": "
+000003e0: 6231 3132 3135 6166 2d62 6237 662d 3439  b11215af-bb7f-49
+000003f0: 3332 2d38 3365 652d 3866 3436 6635 3538  32-83ee-8f46f558
+00000400: 3365 6438 222c 0a20 2020 226d 6574 6164  3ed8",.   "metad
+00000410: 6174 6122 3a20 7b7d 2c0a 2020 2022 736f  ata": {},.   "so
+00000420: 7572 6365 223a 205b 0a20 2020 2022 536f  urce": [.    "So
+00000430: 6d65 2074 6573 7420 6461 7461 2e22 0a20  me test data.". 
+00000440: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+00000450: 2263 656c 6c5f 7479 7065 223a 2022 636f  "cell_type": "co
+00000460: 6465 222c 0a20 2020 2265 7865 6375 7469  de",.   "executi
+00000470: 6f6e 5f63 6f75 6e74 223a 206e 756c 6c2c  on_count": null,
+00000480: 0a20 2020 2269 6422 3a20 2230 3737 3334  .   "id": "07734
+00000490: 3461 322d 3466 3138 2d34 3763 392d 6238  4a2-4f18-47c9-b8
+000004a0: 6135 2d63 3363 3634 3131 3531 3164 6222  a5-c3c6411511db"
+000004b0: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+000004c0: 207b 7d2c 0a20 2020 226f 7574 7075 7473   {},.   "outputs
+000004d0: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
+000004e0: 6522 3a20 5b0a 2020 2020 2270 626d 6336  e": [.    "pbmc6
+000004f0: 386b 203d 206c 6e2e 6465 762e 6461 7461  8k = ln.dev.data
+00000500: 7365 7473 2e61 6e6e 6461 7461 5f70 626d  sets.anndata_pbm
+00000510: 6336 386b 5f72 6564 7563 6564 2829 220a  c68k_reduced()".
+00000520: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00000530: 2022 6365 6c6c 5f74 7970 6522 3a20 226d   "cell_type": "m
+00000540: 6172 6b64 6f77 6e22 2c0a 2020 2022 6964  arkdown",.   "id
+00000550: 223a 2022 3761 6633 6430 3564 2d38 6463  ": "7af3d05d-8dc
+00000560: 332d 3435 3564 2d62 6531 622d 3833 6537  3-455d-be1b-83e7
+00000570: 3938 3632 3130 3531 222c 0a20 2020 226d  98621051",.   "m
+00000580: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+00000590: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+000005a0: 2022 5375 6273 6574 2074 6f20 6120 6d69   "Subset to a mi
+000005b0: 6e69 2066 696c 6520 746f 2073 7065 6564  ni file to speed
+000005c0: 2075 7020 7468 6520 7275 6e20 7469 6d65   up the run time
+000005d0: 206f 6620 7468 6973 206e 6f74 6562 6f6f   of this noteboo
+000005e0: 6b3a 220a 2020 205d 0a20 207d 2c0a 2020  k:".   ].  },.  
+000005f0: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00000600: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
+00000610: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
+00000620: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
+00000630: 3631 3461 3837 3636 2d62 3539 342d 3435  614a8766-b594-45
+00000640: 3738 2d61 3136 332d 3234 3937 3833 3563  78-a163-2497835c
+00000650: 6339 6234 222c 0a20 2020 226d 6574 6164  c9b4",.   "metad
+00000660: 6174 6122 3a20 7b7d 2c0a 2020 2022 6f75  ata": {},.   "ou
+00000670: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
+00000680: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+00000690: 7062 6d63 3638 6b20 3d20 7062 6d63 3638  pbmc68k = pbmc68
+000006a0: 6b5b 3a35 2c20 3a35 5d2e 636f 7079 2829  k[:5, :5].copy()
+000006b0: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+000006c0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+000006d0: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
+000006e0: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+000006f0: 6c6c 2c0a 2020 2022 6964 223a 2022 3432  ll,.   "id": "42
+00000700: 3334 6262 3432 2d30 3365 322d 3436 3736  34bb42-03e2-4676
+00000710: 2d61 3637 342d 3932 3831 6562 3239 3564  -a674-9281eb295d
+00000720: 6637 222c 0a20 2020 226d 6574 6164 6174  f7",.   "metadat
+00000730: 6122 3a20 7b7d 2c0a 2020 2022 6f75 7470  a": {},.   "outp
+00000740: 7574 7322 3a20 5b5d 2c0a 2020 2022 736f  uts": [],.   "so
+00000750: 7572 6365 223a 205b 0a20 2020 2022 7062  urce": [.    "pb
+00000760: 6d63 3638 6b22 0a20 2020 5d0a 2020 7d2c  mc68k".   ].  },
+00000770: 0a20 207b 0a20 2020 2263 656c 6c5f 7479  .  {.   "cell_ty
+00000780: 7065 223a 2022 6d61 726b 646f 776e 222c  pe": "markdown",
+00000790: 0a20 2020 2269 6422 3a20 2236 3232 6238  .   "id": "622b8
+000007a0: 3031 322d 3661 3934 2d34 6134 312d 3861  012-6a94-4a41-8a
+000007b0: 3662 2d34 6331 3738 6564 3463 6661 3622  6b-4c178ed4cfa6"
+000007c0: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+000007d0: 207b 7d2c 0a20 2020 2273 6f75 7263 6522   {},.   "source"
+000007e0: 3a20 5b0a 2020 2020 2223 2323 2020 5570  : [.    "###  Up
+000007f0: 6c6f 6164 2066 726f 6d20 6d65 6d6f 7279  load from memory
+00000800: 2075 7369 6e67 2065 7870 6c69 6369 7420   using explicit 
+00000810: 7365 6d61 6e74 6963 2060 6b65 7960 220a  semantic `key`".
+00000820: 2020 205d 0a20 207d 2c0a 2020 7b0a 2020     ].  },.  {.  
+00000830: 2022 6365 6c6c 5f74 7970 6522 3a20 226d   "cell_type": "m
+00000840: 6172 6b64 6f77 6e22 2c0a 2020 2022 6964  arkdown",.   "id
+00000850: 223a 2022 3831 3338 6138 3837 2d32 6465  ": "8138a887-2de
+00000860: 382d 3461 6439 2d61 6438 622d 3633 3332  8-4ad9-ad8b-6332
+00000870: 3432 3633 6662 3764 222c 0a20 2020 226d  4263fb7d",.   "m
+00000880: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+00000890: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+000008a0: 2022 2323 2323 2055 706c 6f61 6420 6835   "#### Upload h5
+000008b0: 6164 220a 2020 205d 0a20 207d 2c0a 2020  ad".   ].  },.  
+000008c0: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+000008d0: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
+000008e0: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
+000008f0: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
+00000900: 6663 6666 3732 3732 2d31 3364 662d 3436  fcff7272-13df-46
+00000910: 6639 2d61 6236 332d 3235 3932 3161 3530  f9-ab63-25921a50
+00000920: 3766 3938 222c 0a20 2020 226d 6574 6164  7f98",.   "metad
+00000930: 6174 6122 3a20 7b7d 2c0a 2020 2022 6f75  ata": {},.   "ou
+00000940: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
+00000950: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+00000960: 7062 6d63 3638 6b5f 6835 6164 203d 206c  pbmc68k_h5ad = l
+00000970: 6e2e 4669 6c65 2870 626d 6336 386b 2c20  n.File(pbmc68k, 
+00000980: 6b65 793d 5c22 7465 7374 2d75 706c 6f61  key=\"test-uploa
+00000990: 642f 7062 6d63 3638 6b2e 6835 6164 5c22  d/pbmc68k.h5ad\"
+000009a0: 2922 0a20 2020 5d0a 2020 7d2c 0a20 207b  )".   ].  },.  {
+000009b0: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
+000009c0: 2022 636f 6465 222c 0a20 2020 2265 7865   "code",.   "exe
+000009d0: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
+000009e0: 756c 6c2c 0a20 2020 2269 6422 3a20 2261  ull,.   "id": "a
+000009f0: 3937 3631 3766 642d 3066 3431 2d34 3366  97617fd-0f41-43f
+00000a00: 312d 3939 3139 2d32 3561 6361 6233 6466  1-9919-25acab3df
+00000a10: 3063 3522 2c0a 2020 2022 6d65 7461 6461  0c5",.   "metada
+00000a20: 7461 223a 207b 7d2c 0a20 2020 226f 7574  ta": {},.   "out
+00000a30: 7075 7473 223a 205b 5d2c 0a20 2020 2273  puts": [],.   "s
+00000a40: 6f75 7263 6522 3a20 5b0a 2020 2020 2270  ource": [.    "p
+00000a50: 626d 6336 386b 5f68 3561 6420 3d20 6c6e  bmc68k_h5ad = ln
+00000a60: 2e61 6464 2870 626d 6336 386b 5f68 3561  .add(pbmc68k_h5a
+00000a70: 6429 220a 2020 205d 0a20 207d 2c0a 2020  d)".   ].  },.  
+00000a80: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00000a90: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
+00000aa0: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
+00000ab0: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
+00000ac0: 3134 6231 3339 6333 2d66 6231 652d 3463  14b139c3-fb1e-4c
+00000ad0: 6361 2d61 3735 612d 3865 6437 3938 6331  ca-a75a-8ed798c1
+00000ae0: 3839 6138 222c 0a20 2020 226d 6574 6164  89a8",.   "metad
+00000af0: 6174 6122 3a20 7b7d 2c0a 2020 2022 6f75  ata": {},.   "ou
+00000b00: 7470 7574 7322 3a20 5b5d 2c0a 2020 2022  tputs": [],.   "
+00000b10: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+00000b20: 6c6e 2e64 656c 6574 6528 7062 6d63 3638  ln.delete(pbmc68
+00000b30: 6b5f 6835 6164 2c20 6465 6c65 7465 5f64  k_h5ad, delete_d
+00000b40: 6174 615f 6672 6f6d 5f73 746f 7261 6765  ata_from_storage
+00000b50: 3d54 7275 6529 220a 2020 205d 0a20 207d  =True)".   ].  }
+00000b60: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
+00000b70: 7970 6522 3a20 226d 6172 6b64 6f77 6e22  ype": "markdown"
+00000b80: 2c0a 2020 2022 6964 223a 2022 6666 3065  ,.   "id": "ff0e
+00000b90: 3334 6364 2d38 6562 642d 3431 3936 2d61  34cd-8ebd-4196-a
+00000ba0: 3762 642d 6136 3637 6232 6133 3630 6131  7bd-a667b2a360a1
+00000bb0: 222c 0a20 2020 226d 6574 6164 6174 6122  ",.   "metadata"
+00000bc0: 3a20 7b7d 2c0a 2020 2022 736f 7572 6365  : {},.   "source
+00000bd0: 223a 205b 0a20 2020 2022 2323 2323 2055  ": [.    "#### U
+00000be0: 706c 6f61 6420 7a61 7272 220a 2020 205d  pload zarr".   ]
+00000bf0: 0a20 207d 2c0a 2020 7b0a 2020 2022 6365  .  },.  {.   "ce
+00000c00: 6c6c 5f74 7970 6522 3a20 2263 6f64 6522  ll_type": "code"
+00000c10: 2c0a 2020 2022 6578 6563 7574 696f 6e5f  ,.   "execution_
+00000c20: 636f 756e 7422 3a20 6e75 6c6c 2c0a 2020  count": null,.  
+00000c30: 2022 6964 223a 2022 6236 3665 6330 6166   "id": "b66ec0af
+00000c40: 2d39 6339 332d 3433 3861 2d38 3238 302d  -9c93-438a-8280-
+00000c50: 6439 3366 6536 3537 6262 6662 222c 0a20  d93fe657bbfb",. 
+00000c60: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
+00000c70: 2c0a 2020 2022 6f75 7470 7574 7322 3a20  ,.   "outputs": 
+00000c80: 5b5d 2c0a 2020 2022 736f 7572 6365 223a  [],.   "source":
+00000c90: 205b 0a20 2020 2022 2320 5275 6e73 2074   [.    "# Runs t
+00000ca0: 6f6f 206c 6f6e 672c 2073 686f 756c 6420  oo long, should 
+00000cb0: 6265 2074 6573 7465 6420 656c 7365 7768  be tested elsewh
+00000cc0: 6572 655c 6e22 2c0a 2020 2020 2223 2070  ere\n",.    "# p
+00000cd0: 626d 6336 386b 5f7a 6172 7220 3d20 6c6e  bmc68k_zarr = ln
+00000ce0: 2e46 696c 6528 7062 6d63 3638 6b2c 206b  .File(pbmc68k, k
+00000cf0: 6579 3d5c 2274 6573 742d 7570 6c6f 6164  ey=\"test-upload
+00000d00: 2f70 626d 6336 386b 2e7a 6172 725c 222c  /pbmc68k.zarr\",
+00000d10: 2066 6f72 6d61 743d 5c22 7a61 7272 5c22   format=\"zarr\"
+00000d20: 295c 6e22 2c0a 2020 2020 2223 2070 626d  )\n",.    "# pbm
+00000d30: 6336 386b 5f7a 6172 7220 3d20 6c6e 2e61  c68k_zarr = ln.a
+00000d40: 6464 2870 626d 6336 386b 5f7a 6172 7229  dd(pbmc68k_zarr)
+00000d50: 5c6e 222c 0a20 2020 2022 2320 6c6e 2e64  \n",.    "# ln.d
+00000d60: 656c 6574 6528 7062 6d63 3638 6b5f 7a61  elete(pbmc68k_za
+00000d70: 7272 2c20 6465 6c65 7465 5f64 6174 615f  rr, delete_data_
+00000d80: 6672 6f6d 5f73 746f 7261 6765 3d54 7275  from_storage=Tru
+00000d90: 6529 220a 2020 205d 0a20 207d 2c0a 2020  e)".   ].  },.  
+00000da0: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00000db0: 3a20 226d 6172 6b64 6f77 6e22 2c0a 2020  : "markdown",.  
+00000dc0: 2022 6964 223a 2022 6335 3532 6166 3930   "id": "c552af90
+00000dd0: 2d62 3462 332d 3434 3635 2d61 6165 632d  -b4b3-4465-aaec-
+00000de0: 3636 3239 3439 6434 3830 6233 222c 0a20  662949d480b3",. 
+00000df0: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
+00000e00: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
+00000e10: 0a20 2020 2022 2323 2320 5570 6c6f 6164  .    "### Upload
+00000e20: 2075 7369 6e67 2060 6964 6020 7769 7468   using `id` with
+00000e30: 2069 6d70 6c69 6369 7420 606b 6579 6022   implicit `key`"
+00000e40: 0a20 2020 5d0a 2020 7d2c 0a20 207b 0a20  .   ].  },.  {. 
+00000e50: 2020 2263 656c 6c5f 7479 7065 223a 2022    "cell_type": "
+00000e60: 6d61 726b 646f 776e 222c 0a20 2020 2269  markdown",.   "i
+00000e70: 6422 3a20 2236 6163 3136 6638 622d 3339  d": "6ac16f8b-39
+00000e80: 3532 2d34 3639 622d 3962 3663 2d33 6137  52-469b-9b6c-3a7
+00000e90: 3863 3039 3634 3637 6322 2c0a 2020 2022  8c096467c",.   "
+00000ea0: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
+00000eb0: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
+00000ec0: 2020 2223 2323 2320 5570 6c6f 6164 2068    "#### Upload h
+00000ed0: 3561 6422 0a20 2020 5d0a 2020 7d2c 0a20  5ad".   ].  },. 
+00000ee0: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
+00000ef0: 223a 2022 636f 6465 222c 0a20 2020 2265  ": "code",.   "e
+00000f00: 7865 6375 7469 6f6e 5f63 6f75 6e74 223a  xecution_count":
+00000f10: 206e 756c 6c2c 0a20 2020 2269 6422 3a20   null,.   "id": 
+00000f20: 2232 3536 3735 6565 622d 6233 3339 2d34  "25675eeb-b339-4
+00000f30: 3463 372d 3931 3138 2d36 3137 3862 3333  4c7-9118-6178b33
+00000f40: 3531 3130 3022 2c0a 2020 2022 6d65 7461  51100",.   "meta
+00000f50: 6461 7461 223a 207b 7d2c 0a20 2020 226f  data": {},.   "o
+00000f60: 7574 7075 7473 223a 205b 5d2c 0a20 2020  utputs": [],.   
+00000f70: 2273 6f75 7263 6522 3a20 5b0a 2020 2020  "source": [.    
+00000f80: 2270 626d 6336 386b 5f68 3561 6420 3d20  "pbmc68k_h5ad = 
+00000f90: 6c6e 2e46 696c 6528 7062 6d63 3638 6b2c  ln.File(pbmc68k,
+00000fa0: 206e 616d 653d 5c22 7062 6d63 3638 6b2e   name=\"pbmc68k.
+00000fb0: 6835 6164 5c22 2922 0a20 2020 5d0a 2020  h5ad\")".   ].  
+00000fc0: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
+00000fd0: 7479 7065 223a 2022 636f 6465 222c 0a20  type": "code",. 
+00000fe0: 2020 2265 7865 6375 7469 6f6e 5f63 6f75    "execution_cou
+00000ff0: 6e74 223a 206e 756c 6c2c 0a20 2020 2269  nt": null,.   "i
+00001000: 6422 3a20 2236 3331 3465 3862 312d 6363  d": "6314e8b1-cc
+00001010: 6633 2d34 3637 662d 6136 6530 2d34 3638  f3-467f-a6e0-468
+00001020: 3766 3532 6431 3033 3322 2c0a 2020 2022  7f52d1033",.   "
+00001030: 6d65 7461 6461 7461 223a 207b 7d2c 0a20  metadata": {},. 
+00001040: 2020 226f 7574 7075 7473 223a 205b 5d2c    "outputs": [],
+00001050: 0a20 2020 2273 6f75 7263 6522 3a20 5b0a  .   "source": [.
+00001060: 2020 2020 2270 626d 6336 386b 5f68 3561      "pbmc68k_h5a
+00001070: 6420 3d20 6c6e 2e61 6464 2870 626d 6336  d = ln.add(pbmc6
+00001080: 386b 5f68 3561 6429 220a 2020 205d 0a20  8k_h5ad)".   ]. 
+00001090: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
+000010a0: 5f74 7970 6522 3a20 2263 6f64 6522 2c0a  _type": "code",.
+000010b0: 2020 2022 6578 6563 7574 696f 6e5f 636f     "execution_co
+000010c0: 756e 7422 3a20 6e75 6c6c 2c0a 2020 2022  unt": null,.   "
+000010d0: 6964 223a 2022 3037 6538 6536 3136 2d38  id": "07e8e616-8
+000010e0: 3964 662d 3433 3364 2d38 3961 372d 6139  9df-433d-89a7-a9
+000010f0: 6338 6165 6438 3930 6365 222c 0a20 2020  c8aed890ce",.   
+00001100: 226d 6574 6164 6174 6122 3a20 7b7d 2c0a  "metadata": {},.
+00001110: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
+00001120: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
+00001130: 0a20 2020 2022 6c6e 2e64 656c 6574 6528  .    "ln.delete(
+00001140: 7062 6d63 3638 6b5f 6835 6164 2c20 6465  pbmc68k_h5ad, de
+00001150: 6c65 7465 5f64 6174 615f 6672 6f6d 5f73  lete_data_from_s
+00001160: 746f 7261 6765 3d54 7275 6529 220a 2020  torage=True)".  
+00001170: 205d 0a20 207d 2c0a 2020 7b0a 2020 2022   ].  },.  {.   "
+00001180: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
+00001190: 6b64 6f77 6e22 2c0a 2020 2022 6964 223a  kdown",.   "id":
+000011a0: 2022 3862 6435 6461 3539 2d63 3631 362d   "8bd5da59-c616-
+000011b0: 3465 3439 2d39 6630 322d 6634 3831 3463  4e49-9f02-f4814c
+000011c0: 3139 3033 3266 222c 0a20 2020 226d 6574  19032f",.   "met
+000011d0: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+000011e0: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+000011f0: 2323 2323 2055 706c 6f61 6420 7a61 7272  #### Upload zarr
+00001200: 220a 2020 205d 0a20 207d 2c0a 2020 7b0a  ".   ].  },.  {.
+00001210: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
+00001220: 2263 6f64 6522 2c0a 2020 2022 6578 6563  "code",.   "exec
+00001230: 7574 696f 6e5f 636f 756e 7422 3a20 6e75  ution_count": nu
+00001240: 6c6c 2c0a 2020 2022 6964 223a 2022 3265  ll,.   "id": "2e
+00001250: 3665 3361 6530 2d35 6261 392d 3433 3132  6e3ae0-5ba9-4312
+00001260: 2d61 3930 322d 6630 3237 3864 3165 6664  -a902-f0278d1efd
+00001270: 6663 222c 0a20 2020 226d 6574 6164 6174  fc",.   "metadat
+00001280: 6122 3a20 7b7d 2c0a 2020 2022 6f75 7470  a": {},.   "outp
+00001290: 7574 7322 3a20 5b5d 2c0a 2020 2022 736f  uts": [],.   "so
+000012a0: 7572 6365 223a 205b 0a20 2020 2022 2320  urce": [.    "# 
+000012b0: 5275 6e73 2074 6f6f 206c 6f6e 672c 2073  Runs too long, s
+000012c0: 686f 756c 6420 6265 2074 6573 7465 6420  hould be tested 
+000012d0: 656c 7365 7768 6572 655c 6e22 2c0a 2020  elsewhere\n",.  
+000012e0: 2020 2223 2070 626d 6336 386b 5f7a 6172    "# pbmc68k_zar
+000012f0: 7220 3d20 6c6e 2e46 696c 6528 7062 6d63  r = ln.File(pbmc
+00001300: 3638 6b2c 206e 616d 653d 5c22 7062 6d63  68k, name=\"pbmc
+00001310: 3638 6b2e 7a61 7272 5c22 2c20 666f 726d  68k.zarr\", form
+00001320: 6174 3d5c 227a 6172 725c 2229 5c6e 222c  at=\"zarr\")\n",
+00001330: 0a20 2020 2022 2320 7062 6d63 3638 6b5f  .    "# pbmc68k_
+00001340: 7a61 7272 203d 206c 6e2e 6164 6428 7062  zarr = ln.add(pb
+00001350: 6d63 3638 6b5f 7a61 7272 295c 6e22 2c0a  mc68k_zarr)\n",.
+00001360: 2020 2020 2223 206c 6e2e 6465 6c65 7465      "# ln.delete
+00001370: 2870 626d 6336 386b 5f7a 6172 722c 2064  (pbmc68k_zarr, d
+00001380: 656c 6574 655f 6461 7461 5f66 726f 6d5f  elete_data_from_
+00001390: 7374 6f72 6167 653d 5472 7565 2922 0a20  storage=True)". 
+000013a0: 2020 5d0a 2020 7d2c 0a20 207b 0a20 2020    ].  },.  {.   
+000013b0: 2263 656c 6c5f 7479 7065 223a 2022 6d61  "cell_type": "ma
+000013c0: 726b 646f 776e 222c 0a20 2020 2269 6422  rkdown",.   "id"
+000013d0: 3a20 2230 3661 3931 6439 392d 6432 3034  : "06a91d99-d204
+000013e0: 2d34 6563 322d 6235 3637 2d39 3630 6132  -4ec2-b567-960a2
+000013f0: 6161 6164 3338 6422 2c0a 2020 2022 6d65  aaad38d",.   "me
+00001400: 7461 6461 7461 223a 207b 0a20 2020 2022  tadata": {.    "
+00001410: 7461 6773 223a 205b 5d0a 2020 207d 2c0a  tags": [].   },.
+00001420: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
+00001430: 2020 2022 2323 2320 4572 726f 7220 6265     "### Error be
+00001440: 6861 7669 6f72 7322 0a20 2020 5d0a 2020  haviors".   ].  
+00001450: 7d2c 0a20 207b 0a20 2020 2263 656c 6c5f  },.  {.   "cell_
+00001460: 7479 7065 223a 2022 6d61 726b 646f 776e  type": "markdown
+00001470: 222c 0a20 2020 2269 6422 3a20 2266 3736  ",.   "id": "f76
+00001480: 3063 6261 302d 3338 6130 2d34 6265 322d  0cba0-38a0-4be2-
+00001490: 3838 3534 2d64 3166 3137 3638 3964 6530  8854-d1f17689de0
+000014a0: 3522 2c0a 2020 2022 6d65 7461 6461 7461  5",.   "metadata
+000014b0: 223a 207b 7d2c 0a20 2020 2273 6f75 7263  ": {},.   "sourc
+000014c0: 6522 3a20 5b0a 2020 2020 2253 7065 6369  e": [.    "Speci
+000014d0: 6669 6564 2062 7563 6b65 7420 646f 6573  fied bucket does
+000014e0: 206e 6f74 2065 7869 7374 2e22 0a20 2020   not exist.".   
+000014f0: 5d0a 2020 7d2c 0a20 207b 0a20 2020 2263  ].  },.  {.   "c
+00001500: 656c 6c5f 7479 7065 223a 2022 636f 6465  ell_type": "code
+00001510: 222c 0a20 2020 2265 7865 6375 7469 6f6e  ",.   "execution
+00001520: 5f63 6f75 6e74 223a 206e 756c 6c2c 0a20  _count": null,. 
+00001530: 2020 2269 6422 3a20 2264 6532 6639 6337    "id": "de2f9c7
+00001540: 622d 3939 3463 2d34 3137 612d 6137 3030  b-994c-417a-a700
+00001550: 2d66 3531 3761 3239 6466 3738 6522 2c0a  -f517a29df78e",.
+00001560: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
+00001570: 7d2c 0a20 2020 226f 7574 7075 7473 223a  },.   "outputs":
+00001580: 205b 5d2c 0a20 2020 2273 6f75 7263 6522   [],.   "source"
+00001590: 3a20 5b0a 2020 2020 2277 6974 6820 7079  : [.    "with py
+000015a0: 7465 7374 2e72 6169 7365 7328 4669 6c65  test.raises(File
+000015b0: 4e6f 7446 6f75 6e64 4572 726f 7229 3a5c  NotFoundError):\
+000015c0: 6e22 2c0a 2020 2020 2220 2020 2070 626d  n",.    "    pbm
+000015d0: 6336 386b 5f68 3561 6420 3d20 6c6e 2e46  c68k_h5ad = ln.F
+000015e0: 696c 6528 5c22 7333 3a2f 2f69 6e65 7869  ile(\"s3://inexi
+000015f0: 7374 656e 742d 6275 636b 6574 2d32 3339  stent-bucket-239
+00001600: 3830 3938 3334 2f70 626d 6336 386b 2e68  809834/pbmc68k.h
+00001610: 3561 645c 2229 220a 2020 205d 0a20 207d  5ad\")".   ].  }
+00001620: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
+00001630: 7970 6522 3a20 2263 6f64 6522 2c0a 2020  ype": "code",.  
+00001640: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
+00001650: 7422 3a20 6e75 6c6c 2c0a 2020 2022 6964  t": null,.   "id
+00001660: 223a 2022 3133 3835 3063 3863 2d36 3534  ": "13850c8c-654
+00001670: 332d 3463 6634 2d62 3861 652d 6463 3061  3-4cf4-b8ae-dc0a
+00001680: 3030 3330 3065 3266 222c 0a20 2020 226d  00300e2f",.   "m
+00001690: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+000016a0: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
+000016b0: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
+000016c0: 2020 2022 7769 7468 2070 7974 6573 742e     "with pytest.
+000016d0: 7261 6973 6573 2846 696c 654e 6f74 466f  raises(FileNotFo
+000016e0: 756e 6445 7272 6f72 293a 5c6e 222c 0a20  undError):\n",. 
+000016f0: 2020 2022 2020 2020 7062 6d63 3638 6b5f     "    pbmc68k_
+00001700: 6835 6164 203d 206c 6e2e 4669 6c65 285c  h5ad = ln.File(\
+00001710: 2273 333a 2f2f 6c6e 6462 2d73 6574 7570  "s3://lndb-setup
+00001720: 2d63 692f 7062 6d63 3638 6b2e 6835 6164  -ci/pbmc68k.h5ad
+00001730: 5c22 2922 0a20 2020 5d0a 2020 7d2c 0a20  \")".   ].  },. 
+00001740: 207b 0a20 2020 2263 656c 6c5f 7479 7065   {.   "cell_type
+00001750: 223a 2022 6d61 726b 646f 776e 222c 0a20  ": "markdown",. 
+00001760: 2020 2269 6422 3a20 2262 6362 3339 3962    "id": "bcb399b
+00001770: 642d 3863 3133 2d34 3234 612d 6262 6237  d-8c13-424a-bbb7
+00001780: 2d64 3662 6237 6362 3166 3565 3722 2c0a  -d6bb7cb1f5e7",.
 00001790: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-000017a0: 7d2c 0d0a 2020 2022 6f75 7470 7574 7322  },..   "outputs"
-000017b0: 3a20 5b5d 2c0d 0a20 2020 2273 6f75 7263  : [],..   "sourc
-000017c0: 6522 3a20 5b0d 0a20 2020 2022 7769 7468  e": [..    "with
-000017d0: 2070 7974 6573 742e 7261 6973 6573 2846   pytest.raises(F
-000017e0: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
-000017f0: 293a 5c6e 222c 0d0a 2020 2020 2220 2020  ):\n",..    "   
-00001800: 2070 626d 6336 386b 5f68 3561 6420 3d20   pbmc68k_h5ad = 
-00001810: 6c6e 2e46 696c 6528 5c22 7333 3a2f 2f6c  ln.File(\"s3://l
-00001820: 6e64 622d 7365 7475 702d 6369 2f70 626d  ndb-setup-ci/pbm
-00001830: 6336 386b 2e68 3561 645c 2229 220d 0a20  c68k.h5ad\")".. 
-00001840: 2020 5d0d 0a20 207d 2c0d 0a20 207b 0d0a    ]..  },..  {..
-00001850: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-00001860: 226d 6172 6b64 6f77 6e22 2c0d 0a20 2020  "markdown",..   
-00001870: 2269 6422 3a20 2262 6362 3339 3962 642d  "id": "bcb399bd-
-00001880: 3863 3133 2d34 3234 612d 6262 6237 2d64  8c13-424a-bbb7-d
-00001890: 3662 6237 6362 3166 3565 3722 2c0d 0a20  6bb7cb1f5e7",.. 
-000018a0: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
-000018b0: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
-000018c0: 5b0d 0a20 2020 2022 4372 6f73 7320 6275  [..    "Cross bu
-000018d0: 636b 6574 206d 6f76 696e 6720 6f66 2066  cket moving of f
-000018e0: 696c 6573 2e22 0d0a 2020 205d 0d0a 2020  iles."..   ]..  
-000018f0: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
-00001900: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
-00001910: 0d0a 2020 2022 6578 6563 7574 696f 6e5f  ..   "execution_
-00001920: 636f 756e 7422 3a20 6e75 6c6c 2c0d 0a20  count": null,.. 
-00001930: 2020 2269 6422 3a20 2261 6637 3435 3233    "id": "af74523
-00001940: 632d 3535 3362 2d34 6132 352d 3930 6462  c-553b-4a25-90db
-00001950: 2d39 6438 3230 3030 3664 6663 3122 2c0d  -9d820006dfc1",.
-00001960: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
-00001970: 7b7d 2c0d 0a20 2020 226f 7574 7075 7473  {},..   "outputs
-00001980: 223a 205b 5d2c 0d0a 2020 2022 736f 7572  ": [],..   "sour
-00001990: 6365 223a 205b 0d0a 2020 2020 2277 6974  ce": [..    "wit
-000019a0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-000019b0: 5661 6c75 6545 7272 6f72 293a 5c6e 222c  ValueError):\n",
-000019c0: 0d0a 2020 2020 2220 2020 2070 626d 6336  ..    "    pbmc6
-000019d0: 386b 5f68 3561 6420 3d20 6c6e 2e46 696c  8k_h5ad = ln.Fil
-000019e0: 6528 5c22 7333 3a2f 2f62 696f 6e74 792d  e(\"s3://bionty-
-000019f0: 6173 7365 7473 2f53 7065 6369 6573 2e63  assets/Species.c
-00001a00: 7376 5c22 2922 0d0a 2020 205d 0d0a 2020  sv\")"..   ]..  
-00001a10: 7d2c 0d0a 2020 7b0d 0a20 2020 2263 656c  },..  {..   "cel
-00001a20: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
-00001a30: 776e 222c 0d0a 2020 2022 6964 223a 2022  wn",..   "id": "
-00001a40: 3634 3535 3063 3366 222c 0d0a 2020 2022  64550c3f",..   "
-00001a50: 6d65 7461 6461 7461 223a 207b 7d2c 0d0a  metadata": {},..
-00001a60: 2020 2022 736f 7572 6365 223a 205b 0d0a     "source": [..
-00001a70: 2020 2020 2223 2320 5472 6163 6b20 6578      "## Track ex
-00001a80: 6973 7469 6e67 2066 696c 6573 220d 0a20  isting files".. 
-00001a90: 2020 5d0d 0a20 207d 2c0d 0a20 207b 0d0a    ]..  },..  {..
-00001aa0: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-00001ab0: 226d 6172 6b64 6f77 6e22 2c0d 0a20 2020  "markdown",..   
-00001ac0: 2269 6422 3a20 2236 3234 3836 6435 6622  "id": "62486d5f"
-00001ad0: 2c0d 0a20 2020 226d 6574 6164 6174 6122  ,..   "metadata"
-00001ae0: 3a20 7b7d 2c0d 0a20 2020 2273 6f75 7263  : {},..   "sourc
-00001af0: 6522 3a20 5b0d 0a20 2020 2022 4e6f 7720  e": [..    "Now 
-00001b00: 7765 2764 206c 696b 6520 746f 2069 6e67  we'd like to ing
-00001b10: 6573 7420 6120 6373 7620 6669 6c65 2074  est a csv file t
-00001b20: 6861 7420 6973 206c 6f63 6174 6564 2069  hat is located i
-00001b30: 6e20 7468 6973 2062 7563 6b65 743a 220d  n this bucket:".
-00001b40: 0a20 2020 5d0d 0a20 207d 2c0d 0a20 207b  .   ]..  },..  {
-00001b50: 0d0a 2020 2022 6365 6c6c 5f74 7970 6522  ..   "cell_type"
-00001b60: 3a20 2263 6f64 6522 2c0d 0a20 2020 2265  : "code",..   "e
-00001b70: 7865 6375 7469 6f6e 5f63 6f75 6e74 223a  xecution_count":
-00001b80: 206e 756c 6c2c 0d0a 2020 2022 6964 223a   null,..   "id":
-00001b90: 2022 3061 3434 3939 3265 222c 0d0a 2020   "0a44992e",..  
-00001ba0: 2022 6d65 7461 6461 7461 223a 207b 7d2c   "metadata": {},
-00001bb0: 0d0a 2020 2022 6f75 7470 7574 7322 3a20  ..   "outputs": 
-00001bc0: 5b5d 2c0d 0a20 2020 2273 6f75 7263 6522  [],..   "source"
-00001bd0: 3a20 5b0d 0a20 2020 2022 6669 6c65 203d  : [..    "file =
-00001be0: 206c 6e2e 4669 6c65 285c 2273 333a 2f2f   ln.File(\"s3://
-00001bf0: 6c61 6d69 6e64 622d 6369 2f74 6573 742d  lamindb-ci/test-
-00001c00: 6461 7461 2f74 6573 742e 6373 765c 2229  data/test.csv\")
-00001c10: 220d 0a20 2020 5d0d 0a20 207d 2c0d 0a20  "..   ]..  },.. 
-00001c20: 207b 0d0a 2020 2022 6365 6c6c 5f74 7970   {..   "cell_typ
-00001c30: 6522 3a20 2263 6f64 6522 2c0d 0a20 2020  e": "code",..   
-00001c40: 2265 7865 6375 7469 6f6e 5f63 6f75 6e74  "execution_count
-00001c50: 223a 206e 756c 6c2c 0d0a 2020 2022 6964  ": null,..   "id
-00001c60: 223a 2022 6235 3263 3937 3131 222c 0d0a  ": "b52c9711",..
-00001c70: 2020 2022 6d65 7461 6461 7461 223a 207b     "metadata": {
-00001c80: 7d2c 0d0a 2020 2022 6f75 7470 7574 7322  },..   "outputs"
-00001c90: 3a20 5b5d 2c0d 0a20 2020 2273 6f75 7263  : [],..   "sourc
-00001ca0: 6522 3a20 5b0d 0a20 2020 2022 6c6e 2e61  e": [..    "ln.a
-00001cb0: 6464 2866 696c 6529 220d 0a20 2020 5d0d  dd(file)"..   ].
-00001cc0: 0a20 207d 2c0d 0a20 207b 0d0a 2020 2022  .  },..  {..   "
-00001cd0: 6365 6c6c 5f74 7970 6522 3a20 226d 6172  cell_type": "mar
-00001ce0: 6b64 6f77 6e22 2c0d 0a20 2020 2269 6422  kdown",..   "id"
-00001cf0: 3a20 2266 6366 3835 3235 3122 2c0d 0a20  : "fcf85251",.. 
-00001d00: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
-00001d10: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
-00001d20: 5b0d 0a20 2020 2022 5175 6572 7920 616e  [..    "Query an
-00001d30: 6420 6c6f 6164 2064 6174 613a 220d 0a20  d load data:".. 
-00001d40: 2020 5d0d 0a20 207d 2c0d 0a20 207b 0d0a    ]..  },..  {..
-00001d50: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-00001d60: 2263 6f64 6522 2c0d 0a20 2020 2265 7865  "code",..   "exe
-00001d70: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
-00001d80: 756c 6c2c 0d0a 2020 2022 6964 223a 2022  ull,..   "id": "
-00001d90: 6261 3933 6131 6232 222c 0d0a 2020 2022  ba93a1b2",..   "
-00001da0: 6d65 7461 6461 7461 223a 207b 7d2c 0d0a  metadata": {},..
-00001db0: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
-00001dc0: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
-00001dd0: 5b0d 0a20 2020 2022 6669 6c65 203d 206c  [..    "file = l
-00001de0: 6e2e 7365 6c65 6374 286c 6e2e 4669 6c65  n.select(ln.File
-00001df0: 2c20 6964 3d66 696c 652e 6964 292e 6f6e  , id=file.id).on
-00001e00: 6528 295c 6e22 2c0d 0a20 2020 2022 5c6e  e()\n",..    "\n
-00001e10: 222c 0d0a 2020 2020 2266 696c 6522 0d0a  ",..    "file"..
-00001e20: 2020 205d 0d0a 2020 7d2c 0d0a 2020 7b0d     ]..  },..  {.
-00001e30: 0a20 2020 2263 656c 6c5f 7479 7065 223a  .   "cell_type":
-00001e40: 2022 636f 6465 222c 0d0a 2020 2022 6578   "code",..   "ex
-00001e50: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
-00001e60: 6e75 6c6c 2c0d 0a20 2020 2269 6422 3a20  null,..   "id": 
-00001e70: 2264 3932 6435 6363 6422 2c0d 0a20 2020  "d92d5ccd",..   
-00001e80: 226d 6574 6164 6174 6122 3a20 7b7d 2c0d  "metadata": {},.
-00001e90: 0a20 2020 226f 7574 7075 7473 223a 205b  .   "outputs": [
-00001ea0: 5d2c 0d0a 2020 2022 736f 7572 6365 223a  ],..   "source":
-00001eb0: 205b 0d0a 2020 2020 2266 696c 652e 7061   [..    "file.pa
-00001ec0: 7468 2829 220d 0a20 2020 5d0d 0a20 207d  th()"..   ]..  }
-00001ed0: 2c0d 0a20 207b 0d0a 2020 2022 6365 6c6c  ,..  {..   "cell
-00001ee0: 5f74 7970 6522 3a20 2263 6f64 6522 2c0d  _type": "code",.
-00001ef0: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
-00001f00: 6f75 6e74 223a 206e 756c 6c2c 0d0a 2020  ount": null,..  
-00001f10: 2022 6964 223a 2022 3861 6437 3237 3437   "id": "8ad72747
-00001f20: 222c 0d0a 2020 2022 6d65 7461 6461 7461  ",..   "metadata
-00001f30: 223a 207b 7d2c 0d0a 2020 2022 6f75 7470  ": {},..   "outp
-00001f40: 7574 7322 3a20 5b5d 2c0d 0a20 2020 2273  uts": [],..   "s
-00001f50: 6f75 7263 6522 3a20 5b0d 0a20 2020 2022  ource": [..    "
-00001f60: 6669 6c65 2e73 7461 6765 2829 220d 0a20  file.stage()".. 
-00001f70: 2020 5d0d 0a20 207d 2c0d 0a20 207b 0d0a    ]..  },..  {..
-00001f80: 2020 2022 6365 6c6c 5f74 7970 6522 3a20     "cell_type": 
-00001f90: 2263 6f64 6522 2c0d 0a20 2020 2265 7865  "code",..   "exe
-00001fa0: 6375 7469 6f6e 5f63 6f75 6e74 223a 206e  cution_count": n
-00001fb0: 756c 6c2c 0d0a 2020 2022 6964 223a 2022  ull,..   "id": "
-00001fc0: 3738 6664 6238 6532 222c 0d0a 2020 2022  78fdb8e2",..   "
-00001fd0: 6d65 7461 6461 7461 223a 207b 7d2c 0d0a  metadata": {},..
-00001fe0: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
-00001ff0: 2c0d 0a20 2020 2273 6f75 7263 6522 3a20  ,..   "source": 
-00002000: 5b0d 0a20 2020 2022 6669 6c65 2e6c 6f61  [..    "file.loa
-00002010: 6428 292e 6865 6164 2829 220d 0a20 2020  d().head()"..   
-00002020: 5d0d 0a20 207d 2c0d 0a20 207b 0d0a 2020  ]..  },..  {..  
-00002030: 2022 6365 6c6c 5f74 7970 6522 3a20 2263   "cell_type": "c
-00002040: 6f64 6522 2c0d 0a20 2020 2265 7865 6375  ode",..   "execu
-00002050: 7469 6f6e 5f63 6f75 6e74 223a 206e 756c  tion_count": nul
-00002060: 6c2c 0d0a 2020 2022 6964 223a 2022 6138  l,..   "id": "a8
-00002070: 6564 6631 3237 222c 0d0a 2020 2022 6d65  edf127",..   "me
-00002080: 7461 6461 7461 223a 207b 0d0a 2020 2020  tadata": {..    
-00002090: 2274 6167 7322 3a20 5b0d 0a20 2020 2020  "tags": [..     
-000020a0: 2268 6964 652d 6365 6c6c 220d 0a20 2020  "hide-cell"..   
-000020b0: 205d 0d0a 2020 207d 2c0d 0a20 2020 226f   ]..   },..   "o
-000020c0: 7574 7075 7473 223a 205b 5d2c 0d0a 2020  utputs": [],..  
-000020d0: 2022 736f 7572 6365 223a 205b 0d0a 2020   "source": [..  
-000020e0: 2020 2223 2044 656c 6574 6520 7468 6520    "# Delete the 
-000020f0: 6669 6c65 2072 6563 6f72 645c 6e22 2c0d  file record\n",.
-00002100: 0a20 2020 2022 6c6e 2e64 656c 6574 6528  .    "ln.delete(
-00002110: 6669 6c65 2c20 6465 6c65 7465 5f64 6174  file, delete_dat
-00002120: 615f 6672 6f6d 5f73 746f 7261 6765 3d46  a_from_storage=F
-00002130: 616c 7365 2922 0d0a 2020 205d 0d0a 2020  alse)"..   ]..  
-00002140: 7d0d 0a20 5d2c 0d0a 2022 6d65 7461 6461  }.. ],.. "metada
-00002150: 7461 223a 207b 0d0a 2020 226b 6572 6e65  ta": {..  "kerne
-00002160: 6c73 7065 6322 3a20 7b0d 0a20 2020 2264  lspec": {..   "d
-00002170: 6973 706c 6179 5f6e 616d 6522 3a20 2250  isplay_name": "P
-00002180: 7974 686f 6e20 3320 2869 7079 6b65 726e  ython 3 (ipykern
-00002190: 656c 2922 2c0d 0a20 2020 226c 616e 6775  el)",..   "langu
-000021a0: 6167 6522 3a20 2270 7974 686f 6e22 2c0d  age": "python",.
-000021b0: 0a20 2020 226e 616d 6522 3a20 2270 7974  .   "name": "pyt
-000021c0: 686f 6e33 220d 0a20 207d 2c0d 0a20 2022  hon3"..  },..  "
-000021d0: 6c61 6e67 7561 6765 5f69 6e66 6f22 3a20  language_info": 
-000021e0: 7b0d 0a20 2020 2263 6f64 656d 6972 726f  {..   "codemirro
-000021f0: 725f 6d6f 6465 223a 207b 0d0a 2020 2020  r_mode": {..    
-00002200: 226e 616d 6522 3a20 2269 7079 7468 6f6e  "name": "ipython
-00002210: 222c 0d0a 2020 2020 2276 6572 7369 6f6e  ",..    "version
-00002220: 223a 2033 0d0a 2020 207d 2c0d 0a20 2020  ": 3..   },..   
-00002230: 2266 696c 655f 6578 7465 6e73 696f 6e22  "file_extension"
-00002240: 3a20 222e 7079 222c 0d0a 2020 2022 6d69  : ".py",..   "mi
-00002250: 6d65 7479 7065 223a 2022 7465 7874 2f78  metype": "text/x
-00002260: 2d70 7974 686f 6e22 2c0d 0a20 2020 226e  -python",..   "n
-00002270: 616d 6522 3a20 2270 7974 686f 6e22 2c0d  ame": "python",.
-00002280: 0a20 2020 226e 6263 6f6e 7665 7274 5f65  .   "nbconvert_e
-00002290: 7870 6f72 7465 7222 3a20 2270 7974 686f  xporter": "pytho
-000022a0: 6e22 2c0d 0a20 2020 2270 7967 6d65 6e74  n",..   "pygment
-000022b0: 735f 6c65 7865 7222 3a20 2269 7079 7468  s_lexer": "ipyth
-000022c0: 6f6e 3322 2c0d 0a20 2020 2276 6572 7369  on3",..   "versi
-000022d0: 6f6e 223a 2022 332e 392e 3132 220d 0a20  on": "3.9.12".. 
-000022e0: 207d 2c0d 0a20 2022 6e62 7072 6f6a 6563   },..  "nbprojec
-000022f0: 7422 3a20 7b0d 0a20 2020 2269 6422 3a20  t": {..   "id": 
-00002300: 2270 735a 6775 6234 464f 6d7a 5322 2c0d  "psZgub4FOmzS",.
-00002310: 0a20 2020 2270 6172 656e 7422 3a20 6e75  .   "parent": nu
-00002320: 6c6c 2c0d 0a20 2020 2270 7970 6163 6b61  ll,..   "pypacka
-00002330: 6765 223a 206e 756c 6c2c 0d0a 2020 2022  ge": null,..   "
-00002340: 7469 6d65 5f69 6e69 7422 3a20 2232 3032  time_init": "202
-00002350: 332d 3034 2d30 3954 3230 3a30 313a 3537  3-04-09T20:01:57
-00002360: 2e37 3830 3035 332b 3030 3a30 3022 2c0d  .780053+00:00",.
-00002370: 0a20 2020 2275 7365 725f 6861 6e64 6c65  .   "user_handle
-00002380: 223a 2022 7465 7374 7573 6572 3122 2c0d  ": "testuser1",.
-00002390: 0a20 2020 2275 7365 725f 6964 223a 2022  .   "user_id": "
-000023a0: 447a 546a 6b4b 7365 222c 0d0a 2020 2022  DzTjkKse",..   "
-000023b0: 7573 6572 5f6e 616d 6522 3a20 2254 6573  user_name": "Tes
-000023c0: 7420 5573 6572 3122 2c0d 0a20 2020 2276  t User1",..   "v
-000023d0: 6572 7369 6f6e 223a 2022 3022 0d0a 2020  ersion": "0"..  
-000023e0: 7d0d 0a20 7d2c 0d0a 2022 6e62 666f 726d  }.. },.. "nbform
-000023f0: 6174 223a 2034 2c0d 0a20 226e 6266 6f72  at": 4,.. "nbfor
-00002400: 6d61 745f 6d69 6e6f 7222 3a20 350d 0a7d  mat_minor": 5..}
-00002410: 0d0a                                     ..
+000017a0: 7d2c 0a20 2020 2273 6f75 7263 6522 3a20  },.   "source": 
+000017b0: 5b0a 2020 2020 2243 726f 7373 2062 7563  [.    "Cross buc
+000017c0: 6b65 7420 6d6f 7669 6e67 206f 6620 6669  ket moving of fi
+000017d0: 6c65 732e 220a 2020 205d 0a20 207d 2c0a  les.".   ].  },.
+000017e0: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
+000017f0: 6522 3a20 2263 6f64 6522 2c0a 2020 2022  e": "code",.   "
+00001800: 6578 6563 7574 696f 6e5f 636f 756e 7422  execution_count"
+00001810: 3a20 6e75 6c6c 2c0a 2020 2022 6964 223a  : null,.   "id":
+00001820: 2022 6166 3734 3532 3363 2d35 3533 622d   "af74523c-553b-
+00001830: 3461 3235 2d39 3064 622d 3964 3832 3030  4a25-90db-9d8200
+00001840: 3036 6466 6331 222c 0a20 2020 226d 6574  06dfc1",.   "met
+00001850: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00001860: 6f75 7470 7574 7322 3a20 5b5d 2c0a 2020  outputs": [],.  
+00001870: 2022 736f 7572 6365 223a 205b 0a20 2020   "source": [.   
+00001880: 2022 7769 7468 2070 7974 6573 742e 7261   "with pytest.ra
+00001890: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+000018a0: 3a5c 6e22 2c0a 2020 2020 2220 2020 2070  :\n",.    "    p
+000018b0: 626d 6336 386b 5f68 3561 6420 3d20 6c6e  bmc68k_h5ad = ln
+000018c0: 2e46 696c 6528 5c22 7333 3a2f 2f62 696f  .File(\"s3://bio
+000018d0: 6e74 792d 6173 7365 7473 2f53 7065 6369  nty-assets/Speci
+000018e0: 6573 2e63 7376 5c22 2922 0a20 2020 5d0a  es.csv\")".   ].
+000018f0: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
+00001900: 6c5f 7479 7065 223a 2022 6d61 726b 646f  l_type": "markdo
+00001910: 776e 222c 0a20 2020 2269 6422 3a20 2236  wn",.   "id": "6
+00001920: 3435 3530 6333 6622 2c0a 2020 2022 6d65  4550c3f",.   "me
+00001930: 7461 6461 7461 223a 207b 7d2c 0a20 2020  tadata": {},.   
+00001940: 2273 6f75 7263 6522 3a20 5b0a 2020 2020  "source": [.    
+00001950: 2223 2320 5472 6163 6b20 6578 6973 7469  "## Track existi
+00001960: 6e67 2066 696c 6573 220a 2020 205d 0a20  ng files".   ]. 
+00001970: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
+00001980: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
+00001990: 6e22 2c0a 2020 2022 6964 223a 2022 3632  n",.   "id": "62
+000019a0: 3438 3664 3566 222c 0a20 2020 226d 6574  486d5f",.   "met
+000019b0: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+000019c0: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+000019d0: 4e6f 7720 7765 2764 206c 696b 6520 746f  Now we'd like to
+000019e0: 2069 6e67 6573 7420 6120 6373 7620 6669   ingest a csv fi
+000019f0: 6c65 2074 6861 7420 6973 206c 6f63 6174  le that is locat
+00001a00: 6564 2069 6e20 7468 6973 2062 7563 6b65  ed in this bucke
+00001a10: 743a 220a 2020 205d 0a20 207d 2c0a 2020  t:".   ].  },.  
+00001a20: 7b0a 2020 2022 6365 6c6c 5f74 7970 6522  {.   "cell_type"
+00001a30: 3a20 2263 6f64 6522 2c0a 2020 2022 6578  : "code",.   "ex
+00001a40: 6563 7574 696f 6e5f 636f 756e 7422 3a20  ecution_count": 
+00001a50: 6e75 6c6c 2c0a 2020 2022 6964 223a 2022  null,.   "id": "
+00001a60: 3061 3434 3939 3265 222c 0a20 2020 226d  0a44992e",.   "m
+00001a70: 6574 6164 6174 6122 3a20 7b7d 2c0a 2020  etadata": {},.  
+00001a80: 2022 6f75 7470 7574 7322 3a20 5b5d 2c0a   "outputs": [],.
+00001a90: 2020 2022 736f 7572 6365 223a 205b 0a20     "source": [. 
+00001aa0: 2020 2022 6669 6c65 203d 206c 6e2e 4669     "file = ln.Fi
+00001ab0: 6c65 285c 2273 333a 2f2f 6c61 6d69 6e64  le(\"s3://lamind
+00001ac0: 622d 6369 2f74 6573 742d 6461 7461 2f74  b-ci/test-data/t
+00001ad0: 6573 742e 6373 765c 2229 220a 2020 205d  est.csv\")".   ]
+00001ae0: 0a20 207d 2c0a 2020 7b0a 2020 2022 6365  .  },.  {.   "ce
+00001af0: 6c6c 5f74 7970 6522 3a20 2263 6f64 6522  ll_type": "code"
+00001b00: 2c0a 2020 2022 6578 6563 7574 696f 6e5f  ,.   "execution_
+00001b10: 636f 756e 7422 3a20 6e75 6c6c 2c0a 2020  count": null,.  
+00001b20: 2022 6964 223a 2022 6235 3263 3937 3131   "id": "b52c9711
+00001b30: 222c 0a20 2020 226d 6574 6164 6174 6122  ",.   "metadata"
+00001b40: 3a20 7b7d 2c0a 2020 2022 6f75 7470 7574  : {},.   "output
+00001b50: 7322 3a20 5b5d 2c0a 2020 2022 736f 7572  s": [],.   "sour
+00001b60: 6365 223a 205b 0a20 2020 2022 6c6e 2e61  ce": [.    "ln.a
+00001b70: 6464 2866 696c 6529 220a 2020 205d 0a20  dd(file)".   ]. 
+00001b80: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
+00001b90: 5f74 7970 6522 3a20 226d 6172 6b64 6f77  _type": "markdow
+00001ba0: 6e22 2c0a 2020 2022 6964 223a 2022 6663  n",.   "id": "fc
+00001bb0: 6638 3532 3531 222c 0a20 2020 226d 6574  f85251",.   "met
+00001bc0: 6164 6174 6122 3a20 7b7d 2c0a 2020 2022  adata": {},.   "
+00001bd0: 736f 7572 6365 223a 205b 0a20 2020 2022  source": [.    "
+00001be0: 5175 6572 7920 616e 6420 6c6f 6164 2064  Query and load d
+00001bf0: 6174 613a 220a 2020 205d 0a20 207d 2c0a  ata:".   ].  },.
+00001c00: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
+00001c10: 6522 3a20 2263 6f64 6522 2c0a 2020 2022  e": "code",.   "
+00001c20: 6578 6563 7574 696f 6e5f 636f 756e 7422  execution_count"
+00001c30: 3a20 6e75 6c6c 2c0a 2020 2022 6964 223a  : null,.   "id":
+00001c40: 2022 6261 3933 6131 6232 222c 0a20 2020   "ba93a1b2",.   
+00001c50: 226d 6574 6164 6174 6122 3a20 7b7d 2c0a  "metadata": {},.
+00001c60: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
+00001c70: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
+00001c80: 0a20 2020 2022 6669 6c65 203d 206c 6e2e  .    "file = ln.
+00001c90: 7365 6c65 6374 286c 6e2e 4669 6c65 2c20  select(ln.File, 
+00001ca0: 6964 3d66 696c 652e 6964 292e 6f6e 6528  id=file.id).one(
+00001cb0: 295c 6e22 2c0a 2020 2020 225c 6e22 2c0a  )\n",.    "\n",.
+00001cc0: 2020 2020 2266 696c 6522 0a20 2020 5d0a      "file".   ].
+00001cd0: 2020 7d2c 0a20 207b 0a20 2020 2263 656c    },.  {.   "cel
+00001ce0: 6c5f 7479 7065 223a 2022 636f 6465 222c  l_type": "code",
+00001cf0: 0a20 2020 2265 7865 6375 7469 6f6e 5f63  .   "execution_c
+00001d00: 6f75 6e74 223a 206e 756c 6c2c 0a20 2020  ount": null,.   
+00001d10: 2269 6422 3a20 2264 3932 6435 6363 6422  "id": "d92d5ccd"
+00001d20: 2c0a 2020 2022 6d65 7461 6461 7461 223a  ,.   "metadata":
+00001d30: 207b 7d2c 0a20 2020 226f 7574 7075 7473   {},.   "outputs
+00001d40: 223a 205b 5d2c 0a20 2020 2273 6f75 7263  ": [],.   "sourc
+00001d50: 6522 3a20 5b0a 2020 2020 2266 696c 652e  e": [.    "file.
+00001d60: 7061 7468 2829 220a 2020 205d 0a20 207d  path()".   ].  }
+00001d70: 2c0a 2020 7b0a 2020 2022 6365 6c6c 5f74  ,.  {.   "cell_t
+00001d80: 7970 6522 3a20 2263 6f64 6522 2c0a 2020  ype": "code",.  
+00001d90: 2022 6578 6563 7574 696f 6e5f 636f 756e   "execution_coun
+00001da0: 7422 3a20 6e75 6c6c 2c0a 2020 2022 6964  t": null,.   "id
+00001db0: 223a 2022 3861 6437 3237 3437 222c 0a20  ": "8ad72747",. 
+00001dc0: 2020 226d 6574 6164 6174 6122 3a20 7b7d    "metadata": {}
+00001dd0: 2c0a 2020 2022 6f75 7470 7574 7322 3a20  ,.   "outputs": 
+00001de0: 5b5d 2c0a 2020 2022 736f 7572 6365 223a  [],.   "source":
+00001df0: 205b 0a20 2020 2022 6669 6c65 2e73 7461   [.    "file.sta
+00001e00: 6765 2829 220a 2020 205d 0a20 207d 2c0a  ge()".   ].  },.
+00001e10: 2020 7b0a 2020 2022 6365 6c6c 5f74 7970    {.   "cell_typ
+00001e20: 6522 3a20 2263 6f64 6522 2c0a 2020 2022  e": "code",.   "
+00001e30: 6578 6563 7574 696f 6e5f 636f 756e 7422  execution_count"
+00001e40: 3a20 6e75 6c6c 2c0a 2020 2022 6964 223a  : null,.   "id":
+00001e50: 2022 3738 6664 6238 6532 222c 0a20 2020   "78fdb8e2",.   
+00001e60: 226d 6574 6164 6174 6122 3a20 7b7d 2c0a  "metadata": {},.
+00001e70: 2020 2022 6f75 7470 7574 7322 3a20 5b5d     "outputs": []
+00001e80: 2c0a 2020 2022 736f 7572 6365 223a 205b  ,.   "source": [
+00001e90: 0a20 2020 2022 6669 6c65 2e6c 6f61 6428  .    "file.load(
+00001ea0: 292e 6865 6164 2829 220a 2020 205d 0a20  ).head()".   ]. 
+00001eb0: 207d 2c0a 2020 7b0a 2020 2022 6365 6c6c   },.  {.   "cell
+00001ec0: 5f74 7970 6522 3a20 2263 6f64 6522 2c0a  _type": "code",.
+00001ed0: 2020 2022 6578 6563 7574 696f 6e5f 636f     "execution_co
+00001ee0: 756e 7422 3a20 6e75 6c6c 2c0a 2020 2022  unt": null,.   "
+00001ef0: 6964 223a 2022 6138 6564 6631 3237 222c  id": "a8edf127",
+00001f00: 0a20 2020 226d 6574 6164 6174 6122 3a20  .   "metadata": 
+00001f10: 7b0a 2020 2020 2274 6167 7322 3a20 5b0a  {.    "tags": [.
+00001f20: 2020 2020 2022 6869 6465 2d63 656c 6c22       "hide-cell"
+00001f30: 0a20 2020 205d 0a20 2020 7d2c 0a20 2020  .    ].   },.   
+00001f40: 226f 7574 7075 7473 223a 205b 5d2c 0a20  "outputs": [],. 
+00001f50: 2020 2273 6f75 7263 6522 3a20 5b0a 2020    "source": [.  
+00001f60: 2020 2223 2044 656c 6574 6520 7468 6520    "# Delete the 
+00001f70: 6669 6c65 2072 6563 6f72 645c 6e22 2c0a  file record\n",.
+00001f80: 2020 2020 226c 6e2e 6465 6c65 7465 2866      "ln.delete(f
+00001f90: 696c 652c 2064 656c 6574 655f 6461 7461  ile, delete_data
+00001fa0: 5f66 726f 6d5f 7374 6f72 6167 653d 4661  _from_storage=Fa
+00001fb0: 6c73 6529 220a 2020 205d 0a20 207d 0a20  lse)".   ].  }. 
+00001fc0: 5d2c 0a20 226d 6574 6164 6174 6122 3a20  ],. "metadata": 
+00001fd0: 7b0a 2020 226b 6572 6e65 6c73 7065 6322  {.  "kernelspec"
+00001fe0: 3a20 7b0a 2020 2022 6469 7370 6c61 795f  : {.   "display_
+00001ff0: 6e61 6d65 223a 2022 5079 7468 6f6e 2033  name": "Python 3
+00002000: 2028 6970 796b 6572 6e65 6c29 222c 0a20   (ipykernel)",. 
+00002010: 2020 226c 616e 6775 6167 6522 3a20 2270    "language": "p
+00002020: 7974 686f 6e22 2c0a 2020 2022 6e61 6d65  ython",.   "name
+00002030: 223a 2022 7079 7468 6f6e 3322 0a20 207d  ": "python3".  }
+00002040: 2c0a 2020 226c 616e 6775 6167 655f 696e  ,.  "language_in
+00002050: 666f 223a 207b 0a20 2020 2263 6f64 656d  fo": {.   "codem
+00002060: 6972 726f 725f 6d6f 6465 223a 207b 0a20  irror_mode": {. 
+00002070: 2020 2022 6e61 6d65 223a 2022 6970 7974     "name": "ipyt
+00002080: 686f 6e22 2c0a 2020 2020 2276 6572 7369  hon",.    "versi
+00002090: 6f6e 223a 2033 0a20 2020 7d2c 0a20 2020  on": 3.   },.   
+000020a0: 2266 696c 655f 6578 7465 6e73 696f 6e22  "file_extension"
+000020b0: 3a20 222e 7079 222c 0a20 2020 226d 696d  : ".py",.   "mim
+000020c0: 6574 7970 6522 3a20 2274 6578 742f 782d  etype": "text/x-
+000020d0: 7079 7468 6f6e 222c 0a20 2020 226e 616d  python",.   "nam
+000020e0: 6522 3a20 2270 7974 686f 6e22 2c0a 2020  e": "python",.  
+000020f0: 2022 6e62 636f 6e76 6572 745f 6578 706f   "nbconvert_expo
+00002100: 7274 6572 223a 2022 7079 7468 6f6e 222c  rter": "python",
+00002110: 0a20 2020 2270 7967 6d65 6e74 735f 6c65  .   "pygments_le
+00002120: 7865 7222 3a20 2269 7079 7468 6f6e 3322  xer": "ipython3"
+00002130: 2c0a 2020 2022 7665 7273 696f 6e22 3a20  ,.   "version": 
+00002140: 2233 2e39 2e31 3222 0a20 207d 2c0a 2020  "3.9.12".  },.  
+00002150: 226e 6270 726f 6a65 6374 223a 207b 0a20  "nbproject": {. 
+00002160: 2020 2269 6422 3a20 2270 735a 6775 6234    "id": "psZgub4
+00002170: 464f 6d7a 5322 2c0a 2020 2022 7061 7265  FOmzS",.   "pare
+00002180: 6e74 223a 206e 756c 6c2c 0a20 2020 2270  nt": null,.   "p
+00002190: 7970 6163 6b61 6765 223a 206e 756c 6c2c  ypackage": null,
+000021a0: 0a20 2020 2274 696d 655f 696e 6974 223a  .   "time_init":
+000021b0: 2022 3230 3233 2d30 342d 3039 5432 303a   "2023-04-09T20:
+000021c0: 3031 3a35 372e 3738 3030 3533 2b30 303a  01:57.780053+00:
+000021d0: 3030 222c 0a20 2020 2275 7365 725f 6861  00",.   "user_ha
+000021e0: 6e64 6c65 223a 2022 7465 7374 7573 6572  ndle": "testuser
+000021f0: 3122 2c0a 2020 2022 7573 6572 5f69 6422  1",.   "user_id"
+00002200: 3a20 2244 7a54 6a6b 4b73 6522 2c0a 2020  : "DzTjkKse",.  
+00002210: 2022 7573 6572 5f6e 616d 6522 3a20 2254   "user_name": "T
+00002220: 6573 7420 5573 6572 3122 2c0a 2020 2022  est User1",.   "
+00002230: 7665 7273 696f 6e22 3a20 2230 220a 2020  version": "0".  
+00002240: 7d0a 207d 2c0a 2022 6e62 666f 726d 6174  }. },. "nbformat
+00002250: 223a 2034 2c0a 2022 6e62 666f 726d 6174  ": 4,. "nbformat
+00002260: 5f6d 696e 6f72 223a 2035 0a7d 0a         _minor": 5.}.
```

### Comparing `lndb_storage-0.3.2/lndb_storage/_file.py` & `lndb_storage-0.4a1/lndb_storage/_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import os
-import shutil
-from pathlib import Path
-from typing import Union
-
-import fsspec
-import pandas as pd
-import readfcs
-from lndb import settings
-from lndb.dev.upath import UPath
-
-from ._h5ad import read_adata_h5ad
-from ._zarr import read_adata_zarr
-
-READER_FUNCS = {
-    ".csv": pd.read_csv,
-    ".h5ad": read_adata_h5ad,
-    ".parquet": pd.read_parquet,
-    ".fcs": readfcs.read,
-    ".zarr": read_adata_zarr,
-}
-
-
-def print_hook(size, value, **kwargs):
-    progress = value / size
-    out = f"... uploading {Path(kwargs['filepath']).name}: {min(progress, 1.):4.2f}"
-    if progress >= 1:
-        out += "\n"
-    if "NBPRJ_TEST_NBPATH" not in os.environ:
-        print(out, end="\r")
-
-
-class ProgressCallback(fsspec.callbacks.Callback):
-    def branch(self, path_1, path_2, kwargs):
-        kwargs["callback"] = fsspec.callbacks.Callback(
-            hooks=dict(print_hook=print_hook), filepath=path_1
-        )
-
-    def call(self, *args, **kwargs):
-        return None
-
-
-def store_object(localpath: Union[str, Path], storagekey: str) -> float:
-    """Store arbitrary file to configured storage location.
-
-    Returns size in bytes.
-    """
-    storagepath = settings.instance.storage.key_to_filepath(storagekey)
-    localpath = Path(localpath)
-
-    if localpath.is_file():
-        size = localpath.stat().st_size
-    else:
-        size = sum(f.stat().st_size for f in localpath.rglob("*") if f.is_file())
-
-    if isinstance(storagepath, UPath):
-        if localpath.suffix != ".zarr":
-            cb = ProgressCallback()
-        else:
-            # todo: make proper progress bar for zarr
-            cb = fsspec.callbacks.NoOpCallback()
-        storagepath.upload_from(localpath, recursive=True, callback=cb)
-    else:  # storage path is local
-        storagepath.parent.mkdir(parents=True, exist_ok=True)
-        if localpath.is_file():
-            try:
-                shutil.copyfile(localpath, storagepath)
-            except shutil.SameFileError:
-                pass
-        else:
-            if storagepath.exists():
-                shutil.rmtree(storagepath)
-            shutil.copytree(localpath, storagepath)
-    return float(size)  # because this is how we store in the db
-
-
-def delete_storage(storagekey: str):
-    """Delete arbitrary file."""
-    storagepath = settings.instance.storage.key_to_filepath(storagekey)
-    if storagepath.is_file():
-        storagepath.unlink()
-    elif storagepath.is_dir():
-        if isinstance(storagepath, UPath):
-            storagepath.rmdir()
-        else:
-            shutil.rmtree(storagepath)
-    else:
-        raise FileNotFoundError(f"{storagepath} is not an existing path!")
-
-
-def load_to_memory(filepath: Union[str, Path, UPath], stream: bool = False):
-    """Load a file into memory.
-
-    Returns the filepath if no in-memory form is found.
-    """
-    if isinstance(filepath, str):
-        filepath = Path(filepath)
-
-    if filepath.suffix == ".zarr":
-        stream = True
-    elif filepath.suffix != ".h5ad":
-        stream = False
-
-    if not stream:
-        # caching happens here if filename is a UPath
-        # todo: make it safe when filepath is just Path
-        filepath = settings.instance.storage.cloud_to_local(filepath)
-
-    reader = READER_FUNCS.get(filepath.suffix)
-    if reader is None:
-        return filepath
-    else:
-        return reader(filepath)
+import os
+import shutil
+from pathlib import Path
+from typing import Union
+
+import fsspec
+import pandas as pd
+import readfcs
+from lamindb_setup import settings
+from lamindb_setup.dev.upath import UPath
+
+from ._h5ad import read_adata_h5ad
+from ._zarr import read_adata_zarr
+
+READER_FUNCS = {
+    ".csv": pd.read_csv,
+    ".h5ad": read_adata_h5ad,
+    ".parquet": pd.read_parquet,
+    ".fcs": readfcs.read,
+    ".zarr": read_adata_zarr,
+}
+
+
+def print_hook(size, value, **kwargs):
+    progress = value / size
+    out = f"... uploading {Path(kwargs['filepath']).name}: {min(progress, 1.):4.2f}"
+    if progress >= 1:
+        out += "\n"
+    if "NBPRJ_TEST_NBPATH" not in os.environ:
+        print(out, end="\r")
+
+
+class ProgressCallback(fsspec.callbacks.Callback):
+    def branch(self, path_1, path_2, kwargs):
+        kwargs["callback"] = fsspec.callbacks.Callback(
+            hooks=dict(print_hook=print_hook), filepath=path_1
+        )
+
+    def call(self, *args, **kwargs):
+        return None
+
+
+def store_object(localpath: Union[str, Path], storagekey: str) -> float:
+    """Store arbitrary file to configured storage location.
+
+    Returns size in bytes.
+    """
+    storagepath = settings.instance.storage.key_to_filepath(storagekey)
+    localpath = Path(localpath)
+
+    if localpath.is_file():
+        size = localpath.stat().st_size
+    else:
+        size = sum(f.stat().st_size for f in localpath.rglob("*") if f.is_file())
+
+    if isinstance(storagepath, UPath):
+        if localpath.suffix != ".zarr":
+            cb = ProgressCallback()
+        else:
+            # todo: make proper progress bar for zarr
+            cb = fsspec.callbacks.NoOpCallback()
+        storagepath.upload_from(localpath, recursive=True, callback=cb)
+    else:  # storage path is local
+        storagepath.parent.mkdir(parents=True, exist_ok=True)
+        if localpath.is_file():
+            try:
+                shutil.copyfile(localpath, storagepath)
+            except shutil.SameFileError:
+                pass
+        else:
+            if storagepath.exists():
+                shutil.rmtree(storagepath)
+            shutil.copytree(localpath, storagepath)
+    return float(size)  # because this is how we store in the db
+
+
+def delete_storage(storagekey: str):
+    """Delete arbitrary file."""
+    storagepath = settings.instance.storage.key_to_filepath(storagekey)
+    if storagepath.is_file():
+        storagepath.unlink()
+    elif storagepath.is_dir():
+        if isinstance(storagepath, UPath):
+            storagepath.rmdir()
+        else:
+            shutil.rmtree(storagepath)
+    else:
+        raise FileNotFoundError(f"{storagepath} is not an existing path!")
+
+
+def load_to_memory(filepath: Union[str, Path, UPath], stream: bool = False):
+    """Load a file into memory.
+
+    Returns the filepath if no in-memory form is found.
+    """
+    if isinstance(filepath, str):
+        filepath = Path(filepath)
+
+    if filepath.suffix == ".zarr":
+        stream = True
+    elif filepath.suffix != ".h5ad":
+        stream = False
+
+    if not stream:
+        # caching happens here if filename is a UPath
+        # todo: make it safe when filepath is just Path
+        filepath = settings.instance.storage.cloud_to_local(filepath)
+
+    reader = READER_FUNCS.get(filepath.suffix)
+    if reader is None:
+        return filepath
+    else:
+        return reader(filepath)
```

### Comparing `lndb_storage-0.3.2/lndb_storage/_subset.py` & `lndb_storage-0.4a1/lndb_storage/_subset.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from typing import List, Optional, Union
-
-from anndata import AnnData, concat
-from lamin_logger import logger
-from lnschema_core import File
-
-from .object import LazySelector, _subset_anndata_file
-
-SUFFIXES = (".h5ad", ".zarr")
-
-
-def subset(
-    files: Union[List[File], File],
-    query_obs: Optional[Union[List[str], str, LazySelector]] = None,
-    query_var: Optional[Union[List[str], str, LazySelector]] = None,
-    use_concat: bool = False,
-    concat_args: Optional[dict] = None,
-) -> Union[List[AnnData], AnnData, None]:
-    """Subset AnnData files and stream results into memory.
-
-    Args:
-        files: A `File` or a list of `Files` containing `AnnData` objects
-        to subset and load into memory.
-        query_obs: The pandas query string to evaluate on `.obs` of each
-        underlying `AnnData` object.
-        query_var: The pandas query string to evaluate on `.var` of each
-        underlying `AnnData` object.
-        use_concat: If `True`, applies `anndata.concat` on
-        the returned `AnnData` objects.
-        concat_args: Arguments for concatenation.
-    """
-    if isinstance(files, File):
-        files = [files]
-
-    n_files = len(files)
-    if isinstance(query_obs, list):
-        if len(query_obs) != n_files:
-            raise ValueError("query_obs list should be the same length as files.")
-    else:
-        query_obs = [query_obs] * n_files  # type: ignore
-    if isinstance(query_var, list):
-        if len(query_var) != n_files:
-            raise ValueError("query_var list should be the same length as files.")
-    else:
-        query_var = [query_var] * n_files  # type: ignore
-
-    adatas = []
-    # todo: implement parallel processing
-    for i, file in enumerate(files):
-        if file.suffix not in SUFFIXES:
-            logger.warning(f"File {file.id} is not an AnnData object, ignoring.")
-            continue
-        result = _subset_anndata_file(file, query_obs[i], query_var[i])
-        if result is not None:
-            adatas.append(result)
-
-    if not use_concat:
-        return adatas
-    # concat branch here
-    n_adatas = len(adatas)
-    if n_adatas == 0:
-        return None
-    elif n_adatas == 1:
-        return adatas[0]
-    else:
-        concat_args = {} if concat_args is None else concat_args
-        return concat(adatas, **concat_args)
+from typing import List, Optional, Union
+
+from anndata import AnnData, concat
+from lamin_logger import logger
+from lnschema_core import File
+
+from .object import LazySelector, _subset_anndata_file
+
+SUFFIXES = (".h5ad", ".zarr")
+
+
+def subset(
+    files: Union[List[File], File],
+    query_obs: Optional[Union[List[str], str, LazySelector]] = None,
+    query_var: Optional[Union[List[str], str, LazySelector]] = None,
+    use_concat: bool = False,
+    concat_args: Optional[dict] = None,
+) -> Union[List[AnnData], AnnData, None]:
+    """Subset AnnData files and stream results into memory.
+
+    Args:
+        files: A `File` or a list of `Files` containing `AnnData` objects
+        to subset and load into memory.
+        query_obs: The pandas query string to evaluate on `.obs` of each
+        underlying `AnnData` object.
+        query_var: The pandas query string to evaluate on `.var` of each
+        underlying `AnnData` object.
+        use_concat: If `True`, applies `anndata.concat` on
+        the returned `AnnData` objects.
+        concat_args: Arguments for concatenation.
+    """
+    if isinstance(files, File):
+        files = [files]
+
+    n_files = len(files)
+    if isinstance(query_obs, list):
+        if len(query_obs) != n_files:
+            raise ValueError("query_obs list should be the same length as files.")
+    else:
+        query_obs = [query_obs] * n_files  # type: ignore
+    if isinstance(query_var, list):
+        if len(query_var) != n_files:
+            raise ValueError("query_var list should be the same length as files.")
+    else:
+        query_var = [query_var] * n_files  # type: ignore
+
+    adatas = []
+    # todo: implement parallel processing
+    for i, file in enumerate(files):
+        if file.suffix not in SUFFIXES:
+            logger.warning(f"File {file.id} is not an AnnData object, ignoring.")
+            continue
+        result = _subset_anndata_file(file, query_obs[i], query_var[i])
+        if result is not None:
+            adatas.append(result)
+
+    if not use_concat:
+        return adatas
+    # concat branch here
+    n_adatas = len(adatas)
+    if n_adatas == 0:
+        return None
+    elif n_adatas == 1:
+        return adatas[0]
+    else:
+        concat_args = {} if concat_args is None else concat_args
+        return concat(adatas, **concat_args)
```

### Comparing `lndb_storage-0.3.2/lndb_storage/_zarr.py` & `lndb_storage-0.4a1/lndb_storage/_zarr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import warnings
-from typing import Optional
-
-import scipy.sparse as sparse
-import zarr
-from anndata import AnnData
-from anndata._io import read_zarr
-from anndata._io.specs import write_elem
-from lndb.dev.upath import infer_filesystem
-
-from .object._anndata_sizes import _size_elem, _size_raw, size_adata
-
-
-def read_adata_zarr(storepath) -> AnnData:
-    fs, storepath = infer_filesystem(storepath)
-
-    store = fs.get_mapper(storepath, check=True)
-    adata = read_zarr(store)
-
-    return adata
-
-
-def write_adata_zarr(
-    adata: AnnData, storepath, callback=None, chunks=None, **dataset_kwargs
-):
-    fs, storepath = infer_filesystem(storepath)
-
-    store = fs.get_mapper(storepath, create=True)
-    f = zarr.open(store, mode="w")
-
-    adata.strings_to_categoricals()
-    if adata.raw is not None:
-        adata.strings_to_categoricals(adata.raw.var)
-
-    f.attrs.setdefault("encoding-type", "anndata")
-    f.attrs.setdefault("encoding-version", "0.1.0")
-
-    adata_size = None
-    cumulative_val = 0
-
-    def _cb(key_write: Optional[str] = None):
-        nonlocal adata_size
-        nonlocal cumulative_val
-
-        if callback is None:
-            return None
-        if adata_size is None:
-            adata_size = size_adata(adata)
-        if key_write is None:
-            # begin or finish
-            if cumulative_val < adata_size:
-                callback(adata_size, adata_size if cumulative_val > 0 else 0)
-            return None
-
-        elem = getattr(adata, key_write, None)
-        if elem is None:
-            return None
-        elem_size = _size_raw(elem) if key_write == "raw" else _size_elem(elem)
-        if elem_size == 0:
-            return None
-
-        cumulative_val += elem_size
-        callback(adata_size, cumulative_val)
-
-    def _write_elem_cb(f, k, elem, dataset_kwargs):
-        write_elem(f, k, elem, dataset_kwargs=dataset_kwargs)
-        _cb(k)
-
-    _cb(None)
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=UserWarning, module="zarr")
-
-        if chunks is not None and not isinstance(adata.X, sparse.spmatrix):
-            _write_elem_cb(
-                f, "X", adata.X, dataset_kwargs=dict(chunks=chunks, **dataset_kwargs)
-            )
-        else:
-            _write_elem_cb(f, "X", adata.X, dataset_kwargs=dataset_kwargs)
-        for elem in ("obs", "var"):
-            _write_elem_cb(f, elem, getattr(adata, elem), dataset_kwargs=dataset_kwargs)
-        for elem in ("obsm", "varm", "obsp", "varp", "layers", "uns"):
-            _write_elem_cb(
-                f, elem, dict(getattr(adata, elem)), dataset_kwargs=dataset_kwargs
-            )
-        _write_elem_cb(f, "raw", adata.raw, dataset_kwargs=dataset_kwargs)
-    # todo: fix size less than total at the end
-    _cb(None)
+import warnings
+from typing import Optional
+
+import scipy.sparse as sparse
+import zarr
+from anndata import AnnData
+from anndata._io import read_zarr
+from anndata._io.specs import write_elem
+from lamindb_setup.dev.upath import infer_filesystem
+
+from .object._anndata_sizes import _size_elem, _size_raw, size_adata
+
+
+def read_adata_zarr(storepath) -> AnnData:
+    fs, storepath = infer_filesystem(storepath)
+
+    store = fs.get_mapper(storepath, check=True)
+    adata = read_zarr(store)
+
+    return adata
+
+
+def write_adata_zarr(
+    adata: AnnData, storepath, callback=None, chunks=None, **dataset_kwargs
+):
+    fs, storepath = infer_filesystem(storepath)
+
+    store = fs.get_mapper(storepath, create=True)
+    f = zarr.open(store, mode="w")
+
+    adata.strings_to_categoricals()
+    if adata.raw is not None:
+        adata.strings_to_categoricals(adata.raw.var)
+
+    f.attrs.setdefault("encoding-type", "anndata")
+    f.attrs.setdefault("encoding-version", "0.1.0")
+
+    adata_size = None
+    cumulative_val = 0
+
+    def _cb(key_write: Optional[str] = None):
+        nonlocal adata_size
+        nonlocal cumulative_val
+
+        if callback is None:
+            return None
+        if adata_size is None:
+            adata_size = size_adata(adata)
+        if key_write is None:
+            # begin or finish
+            if cumulative_val < adata_size:
+                callback(adata_size, adata_size if cumulative_val > 0 else 0)
+            return None
+
+        elem = getattr(adata, key_write, None)
+        if elem is None:
+            return None
+        elem_size = _size_raw(elem) if key_write == "raw" else _size_elem(elem)
+        if elem_size == 0:
+            return None
+
+        cumulative_val += elem_size
+        callback(adata_size, cumulative_val)
+
+    def _write_elem_cb(f, k, elem, dataset_kwargs):
+        write_elem(f, k, elem, dataset_kwargs=dataset_kwargs)
+        _cb(k)
+
+    _cb(None)
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=UserWarning, module="zarr")
+
+        if chunks is not None and not isinstance(adata.X, sparse.spmatrix):
+            _write_elem_cb(
+                f, "X", adata.X, dataset_kwargs=dict(chunks=chunks, **dataset_kwargs)
+            )
+        else:
+            _write_elem_cb(f, "X", adata.X, dataset_kwargs=dataset_kwargs)
+        for elem in ("obs", "var"):
+            _write_elem_cb(f, elem, getattr(adata, elem), dataset_kwargs=dataset_kwargs)
+        for elem in ("obsm", "varm", "obsp", "varp", "layers", "uns"):
+            _write_elem_cb(
+                f, elem, dict(getattr(adata, elem)), dataset_kwargs=dataset_kwargs
+            )
+        _write_elem_cb(f, "raw", adata.raw, dataset_kwargs=dataset_kwargs)
+    # todo: fix size less than total at the end
+    _cb(None)
```

### Comparing `lndb_storage-0.3.2/lndb_storage/object/_anndata_accessor.py` & `lndb_storage-0.4a1/lndb_storage/object/_anndata_accessor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,358 +1,358 @@
-from functools import cached_property
-from typing import Dict, Mapping, Union
-
-import h5py
-import pandas as pd
-import zarr
-from anndata._core.index import Index, _normalize_indices
-from anndata._core.sparse_dataset import SparseDataset
-from anndata._core.views import _resolve_idx
-from anndata._io.specs.methods import read_indices
-from anndata._io.specs.registry import get_spec, read_elem, read_elem_partial
-from anndata.compat import _read_attr
-from lndb.dev.upath import infer_filesystem as _infer_filesystem
-from lnschema_core import File
-from lnschema_core._core import filepath_from_file_or_folder
-
-from ._subset_anndata import _read_dataframe
-
-
-def _try_backed_full(elem):
-    # think what to do for compatibility with old var and obs
-    if isinstance(elem, (h5py.Dataset, zarr.Array)):
-        return elem
-
-    if isinstance(elem, (h5py.Group, zarr.Group)):
-        encoding_type = get_spec(elem)
-        if encoding_type in ("csr_matrix", "csc_matrix"):
-            return SparseDataset(elem)
-        if "h5sparse_format" in elem.attrs:
-            return SparseDataset(elem)
-
-    return read_elem(elem)
-
-
-class _MapAccessor:
-    def __init__(self, elem, name, indices=None):
-        self.elem = elem
-        self.indices = indices
-        self.name = name
-
-    def __getitem__(self, key):
-        if self.indices is None:
-            return _try_backed_full(self.elem[key])
-        else:
-            return read_elem_partial(self.elem[key], indices=self.indices)
-
-    def keys(self):
-        return list(self.elem.keys())
-
-    def __repr__(self):
-        """Description of the _MapAccessor object."""
-        descr = f"Accessor for the AnnData attribute {self.name}"
-        descr += f"\n  with keys: {self.keys()}"
-        return descr
-
-
-class _AnnDataAttrsMixin:
-    storage: Union[h5py.File, zarr.Group]
-    _attrs_keys: Mapping[str, list]
-
-    @cached_property
-    def obs(self) -> pd.DataFrame:
-        if "obs" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[0], slice(None))
-            return read_elem_partial(self.storage["obs"], indices=indices)
-        else:
-            return _read_dataframe(self.storage["obs"])
-
-    @cached_property
-    def var(self) -> pd.DataFrame:
-        if "var" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[1], slice(None))
-            return read_elem_partial(self.storage["var"], indices=indices)
-        else:
-            return _read_dataframe(self.storage["var"])
-
-    @cached_property
-    def uns(self):
-        if "uns" not in self._attrs_keys:
-            return None
-        return read_elem(self.storage["uns"])
-
-    @cached_property
-    def X(self):
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            return read_elem_partial(self.storage["X"], indices=indices)
-        else:
-            return _try_backed_full(self.storage["X"])
-
-    @cached_property
-    def obsm(self):
-        if "obsm" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[0], slice(None))
-        return _MapAccessor(self.storage["obsm"], "obsm", indices)
-
-    @cached_property
-    def varm(self):
-        if "varm" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[1], slice(None))
-        return _MapAccessor(self.storage["varm"], "varm", indices)
-
-    @cached_property
-    def obsp(self):
-        if "obsp" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[0], indices[0])
-        return _MapAccessor(self.storage["obsp"], "obsp", indices)
-
-    @cached_property
-    def varp(self):
-        if "varp" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[1], indices[1])
-        return _MapAccessor(self.storage["varp"], "varp", indices)
-
-    @cached_property
-    def layers(self):
-        if "layers" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        return _MapAccessor(self.storage["layers"], "layers", indices)
-
-    @property
-    def obs_names(self):
-        return self._obs_names
-
-    @property
-    def var_names(self):
-        return self._var_names
-
-    @cached_property
-    def shape(self):
-        return len(self._obs_names), len(self._var_names)
-
-
-class AnnDataAccessorSubset(_AnnDataAttrsMixin):
-    def __init__(self, storage, indices, attrs_keys, obs_names, var_names, ref_shape):
-        self.storage = storage
-        self.indices = indices
-
-        self._attrs_keys = attrs_keys
-        self._obs_names, self._var_names = obs_names, var_names
-
-        self._ref_shape = ref_shape
-
-    def __getitem__(self, index: Index):
-        """Access a subset of the underlying AnnData object."""
-        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
-        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
-        if self.indices is not None:
-            oidx = _resolve_idx(self.indices[0], oidx, self._ref_shape[0])
-            vidx = _resolve_idx(self.indices[1], vidx, self._ref_shape[1])
-        return type(self)(
-            self.storage,
-            (oidx, vidx),
-            self._attrs_keys,
-            new_obs_names,
-            new_var_names,
-            self._ref_shape,
-        )
-
-    def __repr__(self):
-        """Description of the object."""
-        n_obs, n_vars = self.shape
-        descr = f"{type(self).__name__} object with n_obs × n_vars = {n_obs} × {n_vars}"
-        for attr, keys in self._attrs_keys.items():
-            descr += f"\n  {attr}: {keys}"
-        return descr
-
-    @cached_property
-    def raw(self):
-        if "raw" not in self._attrs_keys:
-            return None
-        prepare_indices = None
-        if self.indices is not None:
-            oidx = self.indices[0]
-            if oidx != slice(None):
-                prepare_indices = oidx, slice(None)
-        return AnnDataRawAccessor(
-            self.storage["raw"],
-            prepare_indices,
-            None,
-            self._obs_names,
-            None,
-            self._ref_shape[0],
-        )
-
-
-class AnnDataRawAccessor(AnnDataAccessorSubset):
-    def __init__(
-        self, storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
-    ):
-        var_raw = storage_raw["var"]
-
-        if var_names is None:
-            var_names = read_elem(var_raw[_read_attr(var_raw.attrs, "_index")])
-
-        if isinstance(ref_shape, int):
-            ref_shape = ref_shape, len(var_names)
-        elif isinstance(ref_shape, tuple) and len(ref_shape) < 2:
-            ref_shape = ref_shape[0], len(var_names)
-
-        if attrs_keys is None:
-            attrs_keys = {}
-            if isinstance(var_raw, (h5py.Dataset, zarr.Array)):
-                attrs_keys["var"] = list(var_raw.dtype.fields.keys())
-            else:
-                # for some reason list(var_raw.keys()) is very slow for zarr
-                # maybe also directly get keys from the underlying mapper
-                attrs_keys["var"] = [key for key in var_raw]
-            if "varm" in storage_raw:
-                varm_keys_raw = [key for key in storage_raw["varm"]]
-                if len(varm_keys_raw) > 0:
-                    attrs_keys["varm"] = varm_keys_raw
-
-        super().__init__(
-            storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
-        )
-
-    @property
-    def raw(self):
-        raise AttributeError
-
-
-class AnnDataAccessor(_AnnDataAttrsMixin):
-    def __init__(self, file: File):
-        fs, file_path_str = _infer_filesystem(filepath_from_file_or_folder(file))
-
-        if file.suffix == ".h5ad":
-            self._conn = fs.open(file_path_str, mode="rb")
-            try:
-                self.storage = h5py.File(self._conn, mode="r")
-            except Exception as e:
-                self._conn.close()
-                raise e
-            self._attrs_keys = _keys_h5(self.storage)
-        elif file.suffix in (".zarr", ".zrad"):
-            self._conn = None
-            mapper = fs.get_mapper(file_path_str, check=True)
-            self.storage = zarr.open(mapper, mode="r")
-            self._attrs_keys = _keys_zarr(self.storage)
-        else:
-            raise ValueError(
-                f"file should have .h5ad, .zarr or .zrad suffix, not {file.suffix}."
-            )
-
-        self._name = file.name
-
-        self._obs_names, self._var_names = read_indices(self.storage)
-
-    def __del__(self):
-        """Closes the connection."""
-        if self._conn is not None:
-            self.storage.close()
-            self._conn.close()
-
-    def __getitem__(self, index: Index) -> AnnDataAccessorSubset:
-        """Access a subset of the underlying AnnData object."""
-        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
-        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
-        return AnnDataAccessorSubset(
-            self.storage,
-            (oidx, vidx),
-            self._attrs_keys,
-            new_obs_names,
-            new_var_names,
-            self.shape,
-        )
-
-    def __repr__(self):
-        """Description of the AnnDataAccessor object."""
-        n_obs, n_vars = self.shape
-        descr = f"AnnDataAccessor object with n_obs × n_vars = {n_obs} × {n_vars}"
-        descr += f"\n  constructed for the AnnData object {self._name}"
-        for attr, keys in self._attrs_keys.items():
-            descr += f"\n    {attr}: {keys}"
-        return descr
-
-    @cached_property
-    def raw(self):
-        if "raw" not in self._attrs_keys:
-            return None
-        return AnnDataRawAccessor(
-            self.storage["raw"], None, None, self._obs_names, None, self.shape[0]
-        )
-
-
-# this is needed because accessing zarr.Group.keys() directly is very slow
-def _keys_zarr(storage: zarr.Group):
-    paths = storage._store.keys()
-
-    attrs_keys: Dict[str, list] = {}
-    obs_var_arrays = []
-
-    for path in paths:
-        if path in (".zattrs", ".zgroup"):
-            continue
-        parts = path.split("/")
-        if len(parts) < 2:
-            continue
-        attr = parts[0]
-        key = parts[1]
-
-        if attr == "X":
-            continue
-
-        if attr in ("obs", "var"):
-            if attr in obs_var_arrays:
-                continue
-            if key == ".zarray":
-                attrs_keys.pop(attr, None)
-                obs_var_arrays.append(attr)
-
-        if attr not in attrs_keys:
-            attrs_keys[attr] = []
-
-        if key in (".zattrs", ".zgroup", ".zarray"):
-            continue
-        attr_keys = attrs_keys[attr]
-        if key not in attr_keys:
-            attr_keys.append(key)
-
-    for attr in obs_var_arrays:
-        attrs_keys[attr] = list(storage[attr].dtype.fields.keys())
-
-    return {attr: keys for attr, keys in attrs_keys.items() if len(keys) > 0}
-
-
-def _keys_h5(storage: h5py.File):
-    attrs_keys: Dict[str, list] = {}
-    for attr in storage.keys():
-        if attr == "X":
-            continue
-        attr_obj = storage[attr]
-        if attr in ("obs", "var") and isinstance(attr_obj, h5py.Dataset):
-            keys = list(attr_obj.dtype.fields.keys())
-        else:
-            keys = list(attr_obj.keys())
-        if len(keys) > 0:
-            attrs_keys[attr] = keys
-    return attrs_keys
+from functools import cached_property
+from typing import Dict, Mapping, Union
+
+import h5py
+import pandas as pd
+import zarr
+from anndata._core.index import Index, _normalize_indices
+from anndata._core.sparse_dataset import SparseDataset
+from anndata._core.views import _resolve_idx
+from anndata._io.specs.methods import read_indices
+from anndata._io.specs.registry import get_spec, read_elem, read_elem_partial
+from anndata.compat import _read_attr
+from lamindb_setup.dev.upath import infer_filesystem as _infer_filesystem
+from lnschema_core import File
+from lnschema_core._core import filepath_from_file_or_folder
+
+from ._subset_anndata import _read_dataframe
+
+
+def _try_backed_full(elem):
+    # think what to do for compatibility with old var and obs
+    if isinstance(elem, (h5py.Dataset, zarr.Array)):
+        return elem
+
+    if isinstance(elem, (h5py.Group, zarr.Group)):
+        encoding_type = get_spec(elem)
+        if encoding_type in ("csr_matrix", "csc_matrix"):
+            return SparseDataset(elem)
+        if "h5sparse_format" in elem.attrs:
+            return SparseDataset(elem)
+
+    return read_elem(elem)
+
+
+class _MapAccessor:
+    def __init__(self, elem, name, indices=None):
+        self.elem = elem
+        self.indices = indices
+        self.name = name
+
+    def __getitem__(self, key):
+        if self.indices is None:
+            return _try_backed_full(self.elem[key])
+        else:
+            return read_elem_partial(self.elem[key], indices=self.indices)
+
+    def keys(self):
+        return list(self.elem.keys())
+
+    def __repr__(self):
+        """Description of the _MapAccessor object."""
+        descr = f"Accessor for the AnnData attribute {self.name}"
+        descr += f"\n  with keys: {self.keys()}"
+        return descr
+
+
+class _AnnDataAttrsMixin:
+    storage: Union[h5py.File, zarr.Group]
+    _attrs_keys: Mapping[str, list]
+
+    @cached_property
+    def obs(self) -> pd.DataFrame:
+        if "obs" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[0], slice(None))
+            return read_elem_partial(self.storage["obs"], indices=indices)
+        else:
+            return _read_dataframe(self.storage["obs"])
+
+    @cached_property
+    def var(self) -> pd.DataFrame:
+        if "var" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[1], slice(None))
+            return read_elem_partial(self.storage["var"], indices=indices)
+        else:
+            return _read_dataframe(self.storage["var"])
+
+    @cached_property
+    def uns(self):
+        if "uns" not in self._attrs_keys:
+            return None
+        return read_elem(self.storage["uns"])
+
+    @cached_property
+    def X(self):
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            return read_elem_partial(self.storage["X"], indices=indices)
+        else:
+            return _try_backed_full(self.storage["X"])
+
+    @cached_property
+    def obsm(self):
+        if "obsm" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[0], slice(None))
+        return _MapAccessor(self.storage["obsm"], "obsm", indices)
+
+    @cached_property
+    def varm(self):
+        if "varm" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[1], slice(None))
+        return _MapAccessor(self.storage["varm"], "varm", indices)
+
+    @cached_property
+    def obsp(self):
+        if "obsp" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[0], indices[0])
+        return _MapAccessor(self.storage["obsp"], "obsp", indices)
+
+    @cached_property
+    def varp(self):
+        if "varp" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[1], indices[1])
+        return _MapAccessor(self.storage["varp"], "varp", indices)
+
+    @cached_property
+    def layers(self):
+        if "layers" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        return _MapAccessor(self.storage["layers"], "layers", indices)
+
+    @property
+    def obs_names(self):
+        return self._obs_names
+
+    @property
+    def var_names(self):
+        return self._var_names
+
+    @cached_property
+    def shape(self):
+        return len(self._obs_names), len(self._var_names)
+
+
+class AnnDataAccessorSubset(_AnnDataAttrsMixin):
+    def __init__(self, storage, indices, attrs_keys, obs_names, var_names, ref_shape):
+        self.storage = storage
+        self.indices = indices
+
+        self._attrs_keys = attrs_keys
+        self._obs_names, self._var_names = obs_names, var_names
+
+        self._ref_shape = ref_shape
+
+    def __getitem__(self, index: Index):
+        """Access a subset of the underlying AnnData object."""
+        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
+        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
+        if self.indices is not None:
+            oidx = _resolve_idx(self.indices[0], oidx, self._ref_shape[0])
+            vidx = _resolve_idx(self.indices[1], vidx, self._ref_shape[1])
+        return type(self)(
+            self.storage,
+            (oidx, vidx),
+            self._attrs_keys,
+            new_obs_names,
+            new_var_names,
+            self._ref_shape,
+        )
+
+    def __repr__(self):
+        """Description of the object."""
+        n_obs, n_vars = self.shape
+        descr = f"{type(self).__name__} object with n_obs × n_vars = {n_obs} × {n_vars}"
+        for attr, keys in self._attrs_keys.items():
+            descr += f"\n  {attr}: {keys}"
+        return descr
+
+    @cached_property
+    def raw(self):
+        if "raw" not in self._attrs_keys:
+            return None
+        prepare_indices = None
+        if self.indices is not None:
+            oidx = self.indices[0]
+            if oidx != slice(None):
+                prepare_indices = oidx, slice(None)
+        return AnnDataRawAccessor(
+            self.storage["raw"],
+            prepare_indices,
+            None,
+            self._obs_names,
+            None,
+            self._ref_shape[0],
+        )
+
+
+class AnnDataRawAccessor(AnnDataAccessorSubset):
+    def __init__(
+        self, storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
+    ):
+        var_raw = storage_raw["var"]
+
+        if var_names is None:
+            var_names = read_elem(var_raw[_read_attr(var_raw.attrs, "_index")])
+
+        if isinstance(ref_shape, int):
+            ref_shape = ref_shape, len(var_names)
+        elif isinstance(ref_shape, tuple) and len(ref_shape) < 2:
+            ref_shape = ref_shape[0], len(var_names)
+
+        if attrs_keys is None:
+            attrs_keys = {}
+            if isinstance(var_raw, (h5py.Dataset, zarr.Array)):
+                attrs_keys["var"] = list(var_raw.dtype.fields.keys())
+            else:
+                # for some reason list(var_raw.keys()) is very slow for zarr
+                # maybe also directly get keys from the underlying mapper
+                attrs_keys["var"] = [key for key in var_raw]
+            if "varm" in storage_raw:
+                varm_keys_raw = [key for key in storage_raw["varm"]]
+                if len(varm_keys_raw) > 0:
+                    attrs_keys["varm"] = varm_keys_raw
+
+        super().__init__(
+            storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
+        )
+
+    @property
+    def raw(self):
+        raise AttributeError
+
+
+class AnnDataAccessor(_AnnDataAttrsMixin):
+    def __init__(self, file: File):
+        fs, file_path_str = _infer_filesystem(filepath_from_file_or_folder(file))
+
+        if file.suffix == ".h5ad":
+            self._conn = fs.open(file_path_str, mode="rb")
+            try:
+                self.storage = h5py.File(self._conn, mode="r")
+            except Exception as e:
+                self._conn.close()
+                raise e
+            self._attrs_keys = _keys_h5(self.storage)
+        elif file.suffix in (".zarr", ".zrad"):
+            self._conn = None
+            mapper = fs.get_mapper(file_path_str, check=True)
+            self.storage = zarr.open(mapper, mode="r")
+            self._attrs_keys = _keys_zarr(self.storage)
+        else:
+            raise ValueError(
+                f"file should have .h5ad, .zarr or .zrad suffix, not {file.suffix}."
+            )
+
+        self._name = file.name
+
+        self._obs_names, self._var_names = read_indices(self.storage)
+
+    def __del__(self):
+        """Closes the connection."""
+        if self._conn is not None:
+            self.storage.close()
+            self._conn.close()
+
+    def __getitem__(self, index: Index) -> AnnDataAccessorSubset:
+        """Access a subset of the underlying AnnData object."""
+        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
+        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
+        return AnnDataAccessorSubset(
+            self.storage,
+            (oidx, vidx),
+            self._attrs_keys,
+            new_obs_names,
+            new_var_names,
+            self.shape,
+        )
+
+    def __repr__(self):
+        """Description of the AnnDataAccessor object."""
+        n_obs, n_vars = self.shape
+        descr = f"AnnDataAccessor object with n_obs × n_vars = {n_obs} × {n_vars}"
+        descr += f"\n  constructed for the AnnData object {self._name}"
+        for attr, keys in self._attrs_keys.items():
+            descr += f"\n    {attr}: {keys}"
+        return descr
+
+    @cached_property
+    def raw(self):
+        if "raw" not in self._attrs_keys:
+            return None
+        return AnnDataRawAccessor(
+            self.storage["raw"], None, None, self._obs_names, None, self.shape[0]
+        )
+
+
+# this is needed because accessing zarr.Group.keys() directly is very slow
+def _keys_zarr(storage: zarr.Group):
+    paths = storage._store.keys()
+
+    attrs_keys: Dict[str, list] = {}
+    obs_var_arrays = []
+
+    for path in paths:
+        if path in (".zattrs", ".zgroup"):
+            continue
+        parts = path.split("/")
+        if len(parts) < 2:
+            continue
+        attr = parts[0]
+        key = parts[1]
+
+        if attr == "X":
+            continue
+
+        if attr in ("obs", "var"):
+            if attr in obs_var_arrays:
+                continue
+            if key == ".zarray":
+                attrs_keys.pop(attr, None)
+                obs_var_arrays.append(attr)
+
+        if attr not in attrs_keys:
+            attrs_keys[attr] = []
+
+        if key in (".zattrs", ".zgroup", ".zarray"):
+            continue
+        attr_keys = attrs_keys[attr]
+        if key not in attr_keys:
+            attr_keys.append(key)
+
+    for attr in obs_var_arrays:
+        attrs_keys[attr] = list(storage[attr].dtype.fields.keys())
+
+    return {attr: keys for attr, keys in attrs_keys.items() if len(keys) > 0}
+
+
+def _keys_h5(storage: h5py.File):
+    attrs_keys: Dict[str, list] = {}
+    for attr in storage.keys():
+        if attr == "X":
+            continue
+        attr_obj = storage[attr]
+        if attr in ("obs", "var") and isinstance(attr_obj, h5py.Dataset):
+            keys = list(attr_obj.dtype.fields.keys())
+        else:
+            keys = list(attr_obj.keys())
+        if len(keys) > 0:
+            attrs_keys[attr] = keys
+    return attrs_keys
```

### Comparing `lndb_storage-0.3.2/lndb_storage/object/_subset_anndata.py` & `lndb_storage-0.4a1/lndb_storage/object/_subset_anndata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from typing import Optional, Union
-
-import h5py
-import zarr
-from anndata import AnnData
-from anndata._io.h5ad import read_dataframe_legacy as read_dataframe_legacy_h5
-from anndata._io.specs.methods import _read_partial
-from anndata._io.specs.registry import read_elem, read_elem_partial
-from anndata._io.zarr import read_dataframe_legacy as read_dataframe_legacy_zarr
-from lndb.dev.upath import infer_filesystem as _infer_filesystem
-from lnschema_core import File
-from lnschema_core._core import filepath_from_file_or_folder
-
-from ._lazy_field import LazySelector
-
-
-def _read_dataframe(elem: Union[zarr.Array, h5py.Dataset, zarr.Group, h5py.Group]):
-    if isinstance(elem, zarr.Array):
-        return read_dataframe_legacy_zarr(elem)
-    elif isinstance(elem, h5py.Dataset):
-        return read_dataframe_legacy_h5(elem)
-    else:
-        return read_elem(elem)
-
-
-def _indices(base_indices, select_indices):
-    if len(base_indices) == len(select_indices):
-        return slice(None)
-    else:
-        return list(base_indices.get_indexer(select_indices))
-
-
-def _subset_adata_storage(
-    storage: Union[zarr.Group, h5py.File],
-    query_obs: Optional[Union[str, LazySelector]] = None,
-    query_var: Optional[Union[str, LazySelector]] = None,
-) -> Union[AnnData, None]:
-    with storage as access:
-        obs = _read_dataframe(access["obs"])
-        var = _read_dataframe(access["var"])
-
-        if query_obs is not None:
-            if hasattr(query_obs, "evaluate"):
-                obs_result = obs[query_obs.evaluate(obj=obs)]  # type: ignore
-            else:
-                obs_result = obs.query(query_obs)
-        else:
-            obs_result = obs
-
-        if query_var is not None:
-            if hasattr(query_var, "evaluate"):
-                var_result = var[query_var.evaluate(obj=var)]  # type: ignore
-            else:
-                var_result = var.query(query_var)
-        else:
-            var_result = var
-
-        if obs_result.index.empty or var_result.index.empty:
-            return None
-
-        obs_idx = _indices(obs.index, obs_result.index)
-        var_idx = _indices(var.index, var_result.index)
-
-        prepare_adata = {}
-        prepare_adata["obs"] = obs_result
-        prepare_adata["var"] = var_result
-        X = read_elem_partial(access["X"], indices=(obs_idx, var_idx))
-        prepare_adata["X"] = X
-        if "obsm" in access:
-            obsm = _read_partial(access["obsm"], indices=(obs_idx, slice(None)))
-            prepare_adata["obsm"] = obsm
-        if "varm" in access:
-            varm = _read_partial(access["varm"], indices=(var_idx, slice(None)))
-            prepare_adata["varm"] = varm
-        if "obsp" in access:
-            obsp = _read_partial(access["obsp"], indices=(obs_idx, obs_idx))
-            prepare_adata["obsp"] = obsp
-        if "varp" in access:
-            varp = _read_partial(access["varp"], indices=(var_idx, var_idx))
-            prepare_adata["varp"] = varp
-        if "layers" in access:
-            layers = _read_partial(access["layers"], indices=(obs_idx, var_idx))
-            prepare_adata["layers"] = layers
-        if "uns" in access:
-            prepare_adata["uns"] = read_elem(access["uns"])
-
-        return AnnData(**prepare_adata)
-
-
-def _subset_anndata_file(
-    file: File,
-    query_obs: Optional[Union[str, LazySelector]] = None,
-    query_var: Optional[Union[str, LazySelector]] = None,
-) -> Union[AnnData, None]:
-    file_path = filepath_from_file_or_folder(file)
-    fs, file_path_str = _infer_filesystem(file_path)
-
-    adata: Union[AnnData, None] = None
-
-    if file.suffix == ".h5ad":
-        with fs.open(file_path_str, mode="rb") as file:
-            storage = h5py.File(file, mode="r")
-            adata = _subset_adata_storage(storage, query_obs, query_var)
-    elif file.suffix == ".zarr":
-        mapper = fs.get_mapper(file_path_str, check=True)
-        storage = zarr.open(mapper, mode="r")
-        adata = _subset_adata_storage(storage, query_obs, query_var)
-
-    return adata
+from typing import Optional, Union
+
+import h5py
+import zarr
+from anndata import AnnData
+from anndata._io.h5ad import read_dataframe_legacy as read_dataframe_legacy_h5
+from anndata._io.specs.methods import _read_partial
+from anndata._io.specs.registry import read_elem, read_elem_partial
+from anndata._io.zarr import read_dataframe_legacy as read_dataframe_legacy_zarr
+from lamindb_setup.dev.upath import infer_filesystem as _infer_filesystem
+from lnschema_core import File
+from lnschema_core._core import filepath_from_file_or_folder
+
+from ._lazy_field import LazySelector
+
+
+def _read_dataframe(elem: Union[zarr.Array, h5py.Dataset, zarr.Group, h5py.Group]):
+    if isinstance(elem, zarr.Array):
+        return read_dataframe_legacy_zarr(elem)
+    elif isinstance(elem, h5py.Dataset):
+        return read_dataframe_legacy_h5(elem)
+    else:
+        return read_elem(elem)
+
+
+def _indices(base_indices, select_indices):
+    if len(base_indices) == len(select_indices):
+        return slice(None)
+    else:
+        return list(base_indices.get_indexer(select_indices))
+
+
+def _subset_adata_storage(
+    storage: Union[zarr.Group, h5py.File],
+    query_obs: Optional[Union[str, LazySelector]] = None,
+    query_var: Optional[Union[str, LazySelector]] = None,
+) -> Union[AnnData, None]:
+    with storage as access:
+        obs = _read_dataframe(access["obs"])
+        var = _read_dataframe(access["var"])
+
+        if query_obs is not None:
+            if hasattr(query_obs, "evaluate"):
+                obs_result = obs[query_obs.evaluate(obj=obs)]  # type: ignore
+            else:
+                obs_result = obs.query(query_obs)
+        else:
+            obs_result = obs
+
+        if query_var is not None:
+            if hasattr(query_var, "evaluate"):
+                var_result = var[query_var.evaluate(obj=var)]  # type: ignore
+            else:
+                var_result = var.query(query_var)
+        else:
+            var_result = var
+
+        if obs_result.index.empty or var_result.index.empty:
+            return None
+
+        obs_idx = _indices(obs.index, obs_result.index)
+        var_idx = _indices(var.index, var_result.index)
+
+        prepare_adata = {}
+        prepare_adata["obs"] = obs_result
+        prepare_adata["var"] = var_result
+        X = read_elem_partial(access["X"], indices=(obs_idx, var_idx))
+        prepare_adata["X"] = X
+        if "obsm" in access:
+            obsm = _read_partial(access["obsm"], indices=(obs_idx, slice(None)))
+            prepare_adata["obsm"] = obsm
+        if "varm" in access:
+            varm = _read_partial(access["varm"], indices=(var_idx, slice(None)))
+            prepare_adata["varm"] = varm
+        if "obsp" in access:
+            obsp = _read_partial(access["obsp"], indices=(obs_idx, obs_idx))
+            prepare_adata["obsp"] = obsp
+        if "varp" in access:
+            varp = _read_partial(access["varp"], indices=(var_idx, var_idx))
+            prepare_adata["varp"] = varp
+        if "layers" in access:
+            layers = _read_partial(access["layers"], indices=(obs_idx, var_idx))
+            prepare_adata["layers"] = layers
+        if "uns" in access:
+            prepare_adata["uns"] = read_elem(access["uns"])
+
+        return AnnData(**prepare_adata)
+
+
+def _subset_anndata_file(
+    file: File,
+    query_obs: Optional[Union[str, LazySelector]] = None,
+    query_var: Optional[Union[str, LazySelector]] = None,
+) -> Union[AnnData, None]:
+    file_path = filepath_from_file_or_folder(file)
+    fs, file_path_str = _infer_filesystem(file_path)
+
+    adata: Union[AnnData, None] = None
+
+    if file.suffix == ".h5ad":
+        with fs.open(file_path_str, mode="rb") as file:
+            storage = h5py.File(file, mode="r")
+            adata = _subset_adata_storage(storage, query_obs, query_var)
+    elif file.suffix == ".zarr":
+        mapper = fs.get_mapper(file_path_str, check=True)
+        storage = zarr.open(mapper, mode="r")
+        adata = _subset_adata_storage(storage, query_obs, query_var)
+
+    return adata
```

### Comparing `lndb_storage-0.3.2/noxfile.py` & `lndb_storage-0.4a1/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import nox
-import requests  # type: ignore
-from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_artifact
-from laminci.nox import build_docs, login_testuser1, run_pre_commit, run_pytest
-
-nox.options.reuse_existing_virtualenvs = True
-
-
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
-def lint(session: nox.Session) -> None:
-    run_pre_commit(session)
-
-
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
-def build(session):
-    login_testuser1(session)
-    session.install(".[dev,test]")
-    response = requests.get("https://github.com/laminlabs/lamindb/tree/adata_access")
-    if response.status_code < 400:
-        session.install("git+https://github.com/laminlabs/lamindb@adata_access")
-    else:
-        session.install("git+https://github.com/laminlabs/lamindb")
-    run_pytest(session)
-    build_docs(session)
-    upload_docs_artifact()
-    move_built_docs_to_docs_slash_project_slug()
+import nox
+import requests  # type: ignore
+from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_artifact
+from laminci.nox import build_docs, login_testuser1, run_pre_commit, run_pytest
+
+nox.options.reuse_existing_virtualenvs = True
+
+
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
+def lint(session: nox.Session) -> None:
+    run_pre_commit(session)
+
+
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
+def build(session):
+    login_testuser1(session)
+    session.install(".[dev,test]")
+    response = requests.get("https://github.com/laminlabs/lamindb/tree/rename")
+    if response.status_code < 400:
+        session.install("git+https://github.com/laminlabs/lamindb@rename")
+    else:
+        session.install("git+https://github.com/laminlabs/lamindb")
+    run_pytest(session)
+    build_docs(session)
+    upload_docs_artifact()
+    move_built_docs_to_docs_slash_project_slug()
```

### Comparing `lndb_storage-0.3.2/PKG-INFO` & `lndb_storage-0.4a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lndb_storage
-Version: 0.3.2
+Version: 0.4a1
 Summary: Storage → object.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core
-Requires-Dist: lndb>=0.45a4
+Requires-Dist: lamindb_setup>=0.46a2
 Requires-Dist: lamin_logger>=0.3.0
 Requires-Dist: nbproject
 Requires-Dist: readfcs
 Requires-Dist: python-dateutil
 Requires-Dist: zarr
 Requires-Dist: anndata>=0.9.1
 Requires-Dist: fsspec
```

