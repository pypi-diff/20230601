# Comparing `tmp/cumulus_library-0.2.0.tar.gz` & `tmp/cumulus_library-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.2.0.tar` & `cumulus_library-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-lrwxr-xr-x   0        0        0        0 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      421 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/README.md
--rw-r--r--   0        0        0      822 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0        0 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    12415 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/cli.py
--rw-r--r--   0        0        0      190 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/errors.py
--rw-r--r--   0        0        0     1502 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0        0 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4843 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3322 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     5868 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2982 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2867 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     3402 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     4146 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      615 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1241 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     2884 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1601 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     2241 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/patient_extensions.py
--rw-r--r--   0        0        0     1436 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1472 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      834 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-06-01 17:48:52.283573 cumulus_library-0.2.0/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1152 2023-06-01 17:48:52.283573 cumulus_library-0.2.0/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 26867633 2023-06-01 17:48:52.359577 cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD10.bsv
--rw-r--r--   0        0        0  2988766 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD9.bsv
--rw-r--r--   0        0        0      404 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4834 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16000 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/study_parser.py
--rw-r--r--   0        0        0      610 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1800 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     5866 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     1566 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 cumulus_library-0.2.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      421 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/README.md
+-rw-r--r--   0        0        0      822 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0        0 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    12415 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/cli.py
+-rw-r--r--   0        0        0      190 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1502 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-06-01 19:47:52.196538 cumulus_library-0.2.1/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0        0 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4843 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3322 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     5868 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2982 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2867 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     3402 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     4146 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      615 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1241 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     2884 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1701 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     2241 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/patient_extensions.py
+-rw-r--r--   0        0        0     1436 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      834 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1152 2023-06-01 19:47:52.200538 cumulus_library-0.2.1/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 26867633 2023-06-01 19:47:52.284538 cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD10.bsv
+-rw-r--r--   0        0        0  2988766 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD9.bsv
+-rw-r--r--   0        0        0      404 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4834 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16000 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0      610 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1800 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     5866 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     1566 2023-06-01 19:47:52.296537 cumulus_library-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 cumulus_library-0.2.1/PKG-INFO
```

### Comparing `cumulus_library-0.2.0/cumulus_library/.sqlfluff` & `cumulus_library-0.2.1/cumulus_library/.sqlfluff`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/base_runner.py` & `cumulus_library-0.2.1/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/cli.py` & `cumulus_library-0.2.1/cumulus_library/cli.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/helper.py` & `cumulus_library-0.2.1/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/schema/columns.py` & `cumulus_library-0.2.1/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/schema/counts.py` & `cumulus_library-0.2.1/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/schema/typesystem.py` & `cumulus_library-0.2.1/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/schema/valueset.py` & `cumulus_library-0.2.1/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/condition.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/documentreference.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/encounter.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/encounter.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/fhir_define.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/manifest.toml` & `cumulus_library-0.2.1/cumulus_library/studies/core/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/medication_request.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/medication_request.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/patient.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/patient.sql`

 * *Files 18% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         WHEN
             t_address.addr_row.postalcode IS NOT NULL
             THEN substr(t_address.addr_row.postalcode, 1, 3)
         ELSE '?'
     END AS postalcode3,
     tp.subject_id,
     tp.subject_ref,
-    tp.race_display,
-    tp.ethnicity_display
+    coalesce(tp.race_display, ARRAY['unknown']) AS race_display,
+    coalesce(tp.ethnicity_display, ARRAY['unknown']) AS ethnicity_display
 FROM
     temp_patient AS tp,
-    unnest(tp.address) AS t_address(addr_row) --noqa
+    unnest(tp.address) AS t_address (addr_row) --noqa: AL05
 
 WHERE
     tp.birthdate IS NOT NULL
     AND tp.gender IS NOT NULL;
 
 
 CREATE OR REPLACE VIEW core__count_patient AS
```

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/patient_extensions.py` & `cumulus_library-0.2.1/cumulus_library/studies/core/patient_extensions.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.2.1/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.2.1/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.2.1/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.2.1/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.2.1/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD10.bsv` & `cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD10.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD9.bsv` & `cumulus_library-0.2.1/cumulus_library/studies/vocab/ICD9.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.2.1/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/study_parser.py` & `cumulus_library-0.2.1/cumulus_library/study_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.2.1/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-0.2.1/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/cumulus_library/template_sql/templates.py` & `cumulus_library-0.2.1/cumulus_library/template_sql/templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.2.0/pyproject.toml` & `cumulus_library-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cumulus-library"
-version = "0.2.0"
+version = "0.2.1"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
     "ctakesclient >= 1.3",
     "fhirclient >= 4.1",
     "Jinja2 > 3",
```

### Comparing `cumulus_library-0.2.0/PKG-INFO` & `cumulus_library-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.2.0
+Version: 0.2.1
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

