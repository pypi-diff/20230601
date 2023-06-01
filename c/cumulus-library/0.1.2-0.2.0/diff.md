# Comparing `tmp/cumulus_library-0.1.2.tar.gz` & `tmp/cumulus_library-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.1.2.tar` & `cumulus_library-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,45 @@
--rw-r--r--   0        0        0      421 2023-05-10 17:46:11.727831 cumulus_library-0.1.2/README.md
--rw-r--r--   0        0        0     6148 2023-04-26 20:28:05.487741 cumulus_library-0.1.2/cumulus_library/.DS_Store
--rw-r--r--   0        0        0       37 2023-04-24 13:09:43.021887 cumulus_library-0.1.2/cumulus_library/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-04-24 13:09:43.021298 cumulus_library-0.1.2/cumulus_library/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-04-24 13:09:43.021615 cumulus_library-0.1.2/cumulus_library/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-04-24 13:09:43.022444 cumulus_library-0.1.2/cumulus_library/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-04-24 13:09:43.022626 cumulus_library-0.1.2/cumulus_library/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      654 2023-05-16 20:32:14.957654 cumulus_library-0.1.2/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0        0 2023-05-03 14:13:54.864994 cumulus_library-0.1.2/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-05-03 14:13:55.000740 cumulus_library-0.1.2/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    11454 2023-05-16 20:32:45.691586 cumulus_library-0.1.2/cumulus_library/cli.py
--rw-r--r--   0        0        0      190 2023-05-03 14:13:54.867961 cumulus_library-0.1.2/cumulus_library/errors.py
--rw-r--r--   0        0        0     1502 2023-05-03 14:13:55.001322 cumulus_library-0.1.2/cumulus_library/helper.py
--rw-r--r--   0        0        0        0 2023-05-03 14:13:54.868178 cumulus_library-0.1.2/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4843 2023-05-03 14:13:55.001612 cumulus_library-0.1.2/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3322 2023-05-03 14:13:55.001778 cumulus_library-0.1.2/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-05-03 14:13:55.001942 cumulus_library-0.1.2/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     5868 2023-05-03 14:13:55.002108 cumulus_library-0.1.2/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     6148 2023-05-06 20:43:18.328180 cumulus_library-0.1.2/cumulus_library/studies/.DS_Store
--rw-r--r--   0        0        0     6148 2023-04-24 13:09:42.998797 cumulus_library-0.1.2/cumulus_library/studies/core/.DS_Store
--rw-r--r--   0        0        0     2982 2023-05-03 14:13:55.002432 cumulus_library-0.1.2/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2867 2023-05-03 14:13:55.002644 cumulus_library-0.1.2/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     3263 2023-05-03 14:13:55.002823 cumulus_library-0.1.2/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     4146 2023-05-03 14:13:55.002993 cumulus_library-0.1.2/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      484 2023-05-03 14:13:55.003203 cumulus_library-0.1.2/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     2884 2023-05-03 14:13:55.003374 cumulus_library-0.1.2/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1499 2023-05-03 14:13:55.003625 cumulus_library-0.1.2/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     1436 2023-05-03 14:13:55.061560 cumulus_library-0.1.2/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1458 2023-05-03 14:13:55.003874 cumulus_library-0.1.2/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      834 2023-05-03 14:13:55.061676 cumulus_library-0.1.2/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-05-03 14:13:55.061738 cumulus_library-0.1.2/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-05-03 14:13:55.061855 cumulus_library-0.1.2/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-05-11 15:38:11.190624 cumulus_library-0.1.2/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1152 2023-05-03 14:13:54.946012 cumulus_library-0.1.2/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 26867633 2023-05-03 14:13:55.047134 cumulus_library-0.1.2/cumulus_library/studies/vocab/ICD10.bsv
--rw-r--r--   0        0        0  2988766 2023-05-03 14:13:55.053775 cumulus_library-0.1.2/cumulus_library/studies/vocab/ICD9.bsv
--rw-r--r--   0        0        0      404 2023-05-03 14:13:55.062071 cumulus_library-0.1.2/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-05-10 20:27:46.158537 cumulus_library-0.1.2/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4834 2023-05-03 14:13:55.055203 cumulus_library-0.1.2/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16003 2023-05-11 16:08:07.728842 cumulus_library-0.1.2/cumulus_library/study_parser.py
--rw-r--r--   0        0        0      610 2023-05-03 14:13:54.869125 cumulus_library-0.1.2/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-05-03 14:13:54.946534 cumulus_library-0.1.2/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0      370 2023-05-03 14:13:54.869469 cumulus_library-0.1.2/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-05-03 14:13:54.946863 cumulus_library-0.1.2/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-05-03 14:13:54.947071 cumulus_library-0.1.2/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     3652 2023-05-03 14:13:54.947262 cumulus_library-0.1.2/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     1561 2023-05-16 20:48:25.434997 cumulus_library-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 cumulus_library-0.1.2/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      421 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/README.md
+-rw-r--r--   0        0        0      822 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0        0 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    12415 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/cli.py
+-rw-r--r--   0        0        0      190 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1502 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0        0 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4843 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3322 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     5868 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2982 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2867 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     3402 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     4146 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      615 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1241 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     2884 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1601 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     2241 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/patient_extensions.py
+-rw-r--r--   0        0        0     1436 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      834 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-06-01 17:48:52.279573 cumulus_library-0.2.0/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-06-01 17:48:52.283573 cumulus_library-0.2.0/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1152 2023-06-01 17:48:52.283573 cumulus_library-0.2.0/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 26867633 2023-06-01 17:48:52.359577 cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD10.bsv
+-rw-r--r--   0        0        0  2988766 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD9.bsv
+-rw-r--r--   0        0        0      404 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4834 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16000 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0      610 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1800 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     5866 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     1566 2023-06-01 17:48:52.371577 cumulus_library-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 cumulus_library-0.2.0/PKG-INFO
```

### Comparing `cumulus_library-0.1.2/cumulus_library/base_runner.py` & `cumulus_library-0.2.0/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/cli.py` & `cumulus_library-0.2.0/cumulus_library/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 #!/usr/bin/env python3
 """Utility for building/retrieving data views in AWS Athena"""
 
 import argparse
+import json
 import os
 import sys
+import sysconfig
 
 from pathlib import Path, PosixPath
 from typing import Dict, List, Optional
 
 import pyathena
 
 from pyathena.pandas.cursor import PandasCursor
 
 from cumulus_library.study_parser import StudyManifestParser
 
 
+# ** Don't delete! **
+# This class isn't used in the rest of the code,
+# but it is used manually as a quick & dirty alternative to the CLI.
 class CumulusEnv:  # pylint: disable=too-few-public-methods
     """
     Wrapper for Cumulus Environment vars.
     Simplifies connections to StudyBuilder without requiring CLI parsing.
     """
 
     def __init__(self):
-        self.bucket = os.environ.get("CUMULUS_LIBRARY_S3")
         self.region = os.environ.get("CUMULUS_LIBRARY_REGION", "us-east-1")
         self.workgroup = os.environ.get("CUMULUS_LIBRARY_WORKGROUP", "cumulus")
         self.profile = os.environ.get("CUMULUS_LIBRARY_PROFILE")
-        self.schema_name = os.environ.get("CUMULUS_LIBRARY_SCHEMA")
+        self.schema_name = os.environ.get("CUMULUS_LIBRARY_DATABASE")
 
     def get_study_builder(self):
-        """Convinience method for getting athena args from environment"""
-        return StudyBuilder(
-            self.bucket, self.region, self.workgroup, self.profile, self.schema_name
-        )
+        """Convenience method for getting athena args from environment"""
+        return StudyBuilder(self.region, self.workgroup, self.profile, self.schema_name)
 
 
 class StudyBuilder:
     """Class for managing Athena cursors and executing Cumulus queries"""
 
     verbose = False
     schema_name = None
 
     def __init__(  # pylint: disable=too-many-arguments
-        self, bucket: str, region: str, workgroup: str, profile: str, schema: str
+        self, region: str, workgroup: str, profile: str, schema: str
     ):
         self.cursor = pyathena.connect(
-            s3_staging_dir=bucket,
             region_name=region,
             work_group=workgroup,
             profile_name=profile,
             schema_name=schema,
         ).cursor()
         self.pandas_cursor = pyathena.connect(
-            s3_staging_dir=bucket,
             region_name=region,
             work_group=workgroup,
             profile_name=profile,
             schema_name=schema,
             cursor_class=PandasCursor,
         ).cursor()
         self.schema_name = schema
@@ -136,20 +136,35 @@
     for source, dest in copy_lists:
         source_path = Path(Path(__file__).resolve().parents[0], source)
         dest_path = Path(abs_path, dest)
         dest_path.write_bytes(source_path.read_bytes())
 
 
 def get_study_dict(alt_dir_paths: List) -> Optional[Dict[str, PosixPath]]:
-    """Convenience function for getting directories in ./studies/
+    """Gets valid study targets from ./studies/, and any pip installed studies
 
     :returns: A list of pathlib.PosixPath objects
     """
     manifest_studies = {}
-    paths = [Path(Path(__file__).resolve().parents[0], "studies")]
+    cli_path = Path(__file__).resolve().parents[0]
+
+    # first, we'll get any installed public studies
+    with open(
+        Path(cli_path, "./module_allowlist.json"), "r", encoding="utf-8"
+    ) as study_allowlist_json:
+        study_allowlist = json.load(study_allowlist_json)["allowlist"]
+    site_packages_dir = sysconfig.get_path("purelib")
+    for study, subdir in study_allowlist.items():
+        study_path = Path(site_packages_dir, subdir)
+        if study_path.exists():
+            manifest_studies[study] = study_path
+
+    # then we'll get all studies inside the project directory, followed by
+    # any user supplied paths last. These take precedence.
+    paths = [Path(cli_path, "studies")]
     if alt_dir_paths is not None:
         paths = paths + alt_dir_paths
     for parent_path in paths:
         for child_path in parent_path.iterdir():
             if child_path.is_dir():
                 manifest_studies[child_path.name] = child_path
             elif child_path.name == "manifest.toml":
@@ -166,36 +181,43 @@
                 "See `cumulus-library --help` for more information"
             )
         )
 
     if args["create"]:
         create_template(args["path"])
 
-    if args["build"] or args["export"]:
+    elif args["build"] or args["export"]:
         builder = StudyBuilder(
-            args["s3_bucket"],
             args["region"],
             args["workgroup"],
             args["profile"],
-            args["database"],
+            args["schema_name"],
         )
         if args["verbose"]:
             builder.verbose = True
 
         study_dict = get_study_dict(args["study_dir"])
+        if args["target"]:
+            for target in args["target"]:
+                if target not in study_dict:
+                    sys.exit(
+                        f"{target} was not found in available studies: "
+                        f"{list(study_dict.keys())}.\n\n"
+                        "If you are trying to run a custom study, make sure "
+                        "you include `-s path/to/study/dir` as an arugment."
+                    )
         # here we invoke the cursor once to confirm valid connections
         builder.cursor.execute("show tables")
 
         if args["build"]:
             if "all" in args["target"]:
                 builder.clean_and_build_all(study_dict)
             else:
                 for target in args["target"]:
-                    if target in study_dict:
-                        builder.clean_and_build_study(study_dict[target])
+                    builder.clean_and_build_study(study_dict[target])
 
         if args["export"]:
             if "all" in args["target"]:
                 builder.export_all(study_dict)
             else:
                 for target in args["target"]:
                     builder.export_study(study_dict[target])
@@ -210,15 +232,15 @@
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""Generates study tables and views from post-Cumulus ETL data.
 
 cumulus_library will attempt to create a connection to AWS athena. The
 following order of preference is used to select credentials:
   - explict command line arguments
   - cumulus environment variables (CUMULUS_LIBRARY_PROFILE, 
-    CUMULUS_LIBRARY_SCHEMA, CUMULUS_LIBRARY_S3, CUMULUS_LIBRARY_REGION)
+    CUMULUS_LIBRARY_DATABASE, CUMULUS_LIBRARY_REGION)
   - Normal boto profile order (AWS env vars, ~/.aws/credentials, ~/.aws/config)""",
     )
 
     studygen = parser.add_argument_group("Creating study templates")
     studygen.add_argument(
         "-c",
         "--create",
@@ -244,22 +266,22 @@
         help=(
             "Specify one or more studies to create views form. Default is to "
             "build all studies."
         ),
     )
     db.add_argument(
         "-s",
-        "--study_dir",
+        "--study-dir",
         action="append",
         help=(
             "Optionally add one or more directories to look for study definitions in. "
             "Default is in project directory and CUMULUS_LIBRARY_PATH, if present, "
             "followed by any supplied paths. Target, and all its subdirectories, "
             "are checked for manifests. Overriding studies with the same namespace "
-            "supercede eariler ones."
+            "supersede earlier ones."
         ),
     )
     db.add_argument(
         "-b",
         "--build",
         default=False,
         action="store_true",
@@ -278,27 +300,26 @@
         default=False,
         action="store_true",
         help=("Prints detailed SQL query info"),
     )
 
     aws = parser.add_argument_group("AWS config")
     aws.add_argument("--profile", help="AWS profile", default="default")
-    aws.add_argument("--database", help="Cumulus ETL Athena DB/schema")
+    aws.add_argument(
+        "--database",
+        # internally, we use PyAthena's terminology for this but the UX term is "database"
+        dest="schema_name",
+        help="Cumulus Athena database name",
+    )
     aws.add_argument(
         "--workgroup",
         default="cumulus",
         help="Cumulus Athena workgroup (default: cumulus)",
     )
     aws.add_argument(
-        "--s3_bucket",
-        help=(
-            "S3 location to store athena metadata. " "(will contain some query outputs)"
-        ),
-    )
-    aws.add_argument(
         "--region",
         help="AWS region data of Athena instance (default: us-east-1)",
         default="us-east-1",
     )
 
     return parser
 
@@ -320,23 +341,25 @@
         posix_paths = []
         for path in args["study_dir"]:
             posix_paths.append(get_abs_posix_path(path))
         args["study_dir"] = posix_paths
 
     if profile_env := os.environ.get("CUMULUS_LIBRARY_PROFILE"):
         args["profile"] = profile_env
-    if database_env := os.environ.get("CUMULUS_LIBRARY_SCHEMA"):
-        args["database"] = database_env
+    if database_env := os.environ.get("CUMULUS_LIBRARY_DATABASE"):
+        args["schema_name"] = database_env
     if workgroup_env := os.environ.get("CUMULUS_LIBRARY_WORKGROUP"):
         args["workgroup"] = workgroup_env
-    if bucket_env := os.environ.get("CUMULUS_LIBRARY_S3"):
-        args["s3_bucket"] = bucket_env
     if region_env := os.environ.get("CUMULUS_LIBRARY_REGION"):
         args["region"] = region_env
     if path_dir := os.environ.get("CUMULUS_LIBRARY_PATH"):
         args["path"] = [path_dir] + args["path"]
 
     return run_cli(args)
 
 
+def main_cli():  # called by the generated wrapper scripts
+    main()
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `cumulus_library-0.1.2/cumulus_library/helper.py` & `cumulus_library-0.2.0/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/schema/columns.py` & `cumulus_library-0.2.0/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/schema/counts.py` & `cumulus_library-0.2.0/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/schema/typesystem.py` & `cumulus_library-0.2.0/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/schema/valueset.py` & `cumulus_library-0.2.0/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.2.0/cumulus_library/studies/core/condition.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.2.0/cumulus_library/studies/core/documentreference.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/core/encounter.sql` & `cumulus_library-0.2.0/cumulus_library/studies/core/encounter.sql`

 * *Files 5% similar despite different names*

```diff
@@ -47,51 +47,55 @@
     ce.start_month,
     ce.start_year,
     ce.subject_ref,
     ce.encounter_ref,
     ce.encounter_id,
     ce.enc_class.code AS enc_class_code,
     cp.gender,
-    cp.race,
+    cp.race_display,
+    cp.ethnicity_display,
     cp.postalcode3
 FROM core__encounter AS ce, core__patient AS cp
 WHERE ce.subject_ref = cp.subject_ref;
 
 
 CREATE OR REPLACE VIEW core__count_encounter_month AS
 WITH powerset AS (
     SELECT
         count(DISTINCT ce.subject_ref) AS cnt_subject,
         count(DISTINCT ce.encounter_id) AS cnt_encounter,
         ce.enc_class.code AS enc_class_code,
         ce.start_month,
         ce.age_at_visit,
         cp.gender,
-        cp.race,
+        cp.race_display,
+        cp.ethnicity_display,
         cp.postalcode3
     FROM core__encounter AS ce, core__patient AS cp
     WHERE ce.subject_ref = cp.subject_ref
     GROUP BY
         cube(
             ce.enc_class,
             ce.start_month,
             ce.age_at_visit,
             cp.gender,
-            cp.race,
+            cp.race_display,
+            cp.ethnicity_display,
             cp.postalcode3
         )
 )
 
 SELECT DISTINCT
     powerset.cnt_encounter AS cnt,
     powerset.enc_class_code,
     powerset.start_month,
     powerset.age_at_visit,
     powerset.gender,
-    race.display AS race_display,
+    powerset.race_display,
+    powerset.ethnicity_display,
     powerset.postalcode3
 FROM powerset
 WHERE powerset.cnt_subject >= 10
 ORDER BY
     powerset.start_month ASC, powerset.enc_class_code ASC, powerset.age_at_visit ASC;
 
 CREATE OR REPLACE VIEW core__count_encounter_day AS
```

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.2.0/cumulus_library/studies/core/fhir_define.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.2.0/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.2.0/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.2.0/cumulus_library/studies/core/study_period.sql`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
         ce.end_date,
         ce.age_at_visit,
         cd.author_date,
         cd.author_week,
         cd.author_month,
         cd.author_year,
         cp.gender,
-        cp.race.display AS race_display,
+        cp.race_display,
+        cp.ethnicity_display,
         cp.subject_ref,
         ce.encounter_ref,
         cd.doc_ref,
         date_diff('day', ce.start_date, cd.author_date) AS diff_enc_note_days,
         coalesce(ce.enc_class.code, '?') AS enc_class_code,
         coalesce(cd.doc_type.code, '?') AS doc_type_code,
         coalesce(cd.doc_type.display, cd.doc_type.code) AS doc_type_display
```

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.2.0/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.2.0/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.2.0/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.2.0/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/vocab/ICD10.bsv` & `cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD10.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/vocab/ICD9.bsv` & `cumulus_library-0.2.0/cumulus_library/studies/vocab/ICD9.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.2.0/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/cumulus_library/study_parser.py` & `cumulus_library-0.2.0/cumulus_library/study_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         :verbose: toggle from progress bar to query output, optional
         :returns: list of dropped tables (for unit testing only)
 
         TODO: If we need to support additional databases, we may need to investigate
         additional ways to get a list of table prefixes
         """
         if not schema_name:
-            raise ValueError("No schema name provided")
+            raise ValueError("No database provided")
         prefix = self.get_study_prefix()
         view_sql = get_show_views(schema_name, prefix)
         table_sql = get_show_tables(schema_name, prefix)
         view_table_list = []
         for query_and_type in [[view_sql, "VIEW"], [table_sql, "TABLE"]]:
             cursor.execute(query_and_type[0])
             for db_row_tuple in cursor:
```

### Comparing `cumulus_library-0.1.2/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.2.0/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.1.2/pyproject.toml` & `cumulus_library-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cumulus-library"
-version = "0.1.2"
+version = "0.2.0"
 # In order to support 3.12, we wil need to refactor out load_module, which is
 # targeted for deprecation in that version.
 requires-python = ">= 3.9, <3.12"
 dependencies = [
     "ctakesclient >= 1.3",
     "fhirclient >= 4.1",
     "Jinja2 > 3",
@@ -40,15 +40,15 @@
 [project.urls]
 Home = "https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/"
 Documentation = "https://docs.smarthealthit.org/cumulus/"
 Source = "https://github.com/smart-on-fhir/cumulus-library-core"
 
 
 [project.scripts]
-cumulus-library = "cumulus_library.cli:main"
+cumulus-library = "cumulus_library.cli:main_cli"
 
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.sdist]
-include = [".sqlfluff"]
+include = [".sqlfluff"]
```

### Comparing `cumulus_library-0.1.2/PKG-INFO` & `cumulus_library-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.1.2
+Version: 0.2.0
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

