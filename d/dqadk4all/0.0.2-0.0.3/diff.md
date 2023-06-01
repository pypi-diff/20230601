# Comparing `tmp/dqadk4all-0.0.2.tar.gz` & `tmp/dqadk4all-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqadk4all-0.0.2.tar", last modified: Thu Jun  1 08:40:55 2023, max compression
+gzip compressed data, was "dqadk4all-0.0.3.tar", last modified: Thu Jun  1 10:27:51 2023, max compression
```

## Comparing `dqadk4all-0.0.2.tar` & `dqadk4all-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:40:55.899712 dqadk4all-0.0.2/
--rw-rw-rw-   0        0        0      355 2023-06-01 08:40:55.898713 dqadk4all-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       38 2023-05-31 10:46:38.000000 dqadk4all-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:40:55.877713 dqadk4all-0.0.2/dqadk4all/
--rw-rw-rw-   0        0        0      599 2023-05-31 17:23:59.000000 dqadk4all-0.0.2/dqadk4all/__init__.py
--rw-rw-rw-   0        0        0    25069 2023-05-31 17:28:14.000000 dqadk4all-0.0.2/dqadk4all/ge_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:40:55.897712 dqadk4all-0.0.2/dqadk4all.egg-info/
--rw-rw-rw-   0        0        0      355 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 08:40:55.000000 dqadk4all-0.0.2/dqadk4all.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:40:55.899712 dqadk4all-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-06-01 08:40:28.000000 dqadk4all-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:27:51.064443 dqadk4all-0.0.3/
+-rw-rw-rw-   0        0        0      355 2023-06-01 10:27:51.063490 dqadk4all-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2023-05-31 10:46:38.000000 dqadk4all-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 10:27:51.050132 dqadk4all-0.0.3/dqadk4all/
+-rw-rw-rw-   0        0        0      558 2023-06-01 10:09:34.000000 dqadk4all-0.0.3/dqadk4all/__init__.py
+-rw-rw-rw-   0        0        0    26327 2023-06-01 10:27:11.000000 dqadk4all-0.0.3/dqadk4all/ge_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:27:51.062534 dqadk4all-0.0.3/dqadk4all.egg-info/
+-rw-rw-rw-   0        0        0      355 2023-06-01 10:27:50.000000 dqadk4all-0.0.3/dqadk4all.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-01 10:27:50.000000 dqadk4all-0.0.3/dqadk4all.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 10:27:50.000000 dqadk4all-0.0.3/dqadk4all.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 10:27:50.000000 dqadk4all-0.0.3/dqadk4all.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 10:27:51.064443 dqadk4all-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-06-01 10:27:40.000000 dqadk4all-0.0.3/setup.py
```

### Comparing `dqadk4all-0.0.2/dqadk4all/__init__.py` & `dqadk4all-0.0.3/dqadk4all/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 from .ge_lib import result_default, result_error_exception, check_column_value_lengths_to_be_between, \
-    check_orphan_values_in_column_table, check_table_row_count_with_source_table, normalize_json, \
+    check_orphan_values_in_column_table, normalize_json, \
     table_columns_check_duplicates, table_columns_check_nulls, table_columns_correct_nomenclature, \
     table_columns_match, validate_if_startdate_after_enddate, validate_key_value_connections, \
     validate_list_of_values_in_column, validate_percentage_of_values_in_columns, \
     table_columns_static_dimension_default_values_existence, execute_tc, set_time_now, FormatResult, AddResult
```

### Comparing `dqadk4all-0.0.2/dqadk4all/ge_lib.py` & `dqadk4all-0.0.3/dqadk4all/ge_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 import json as J
 from datetime import datetime
+# from pyspark.sql.types import *
+# from pyspark.sql.functions import *
+from pyspark.sql import SparkSession
+from pyspark.context import SparkContext
+
+sc = SparkContext.getOrCreate()
+spark = SparkSession(sc)
 
 result_default_pre =  {
   "success" : True,
   "result" : {
       "partial_unexpected_list" : [],
       "unexpected_count" : 0,
       "unexpected_percent" : 0,
@@ -425,35 +432,35 @@
 
 # COMMAND ----------
 
 # MAGIC %md ### Check table row count with source table
 
 # COMMAND ----------
 
-def check_table_row_count_with_source_table(Table, SourcePath, Parameters):
-  tc_Parameters = Parameters
-  tc_table = SourcePath + '.' + Table
-  check_table_row_count_with_table_result = result_default()
-  try:
-    sql_count = "SELECT COUNT(*) as table_a_count FROM " + tc_table
-    table_a_count = spark.sql(sql_count)
-    a_count = table_a_count.first().table_a_count
-    sql_count_raw = "SELECT COUNT(*) as table_b_count FROM " + tc_Parameters
-    table_b_count = readSql(sql_count_raw)
-    b_count = table_b_count.first().table_b_count
-    if a_count != b_count:
-        check_table_row_count_with_table_result["success"] = False
-        check_table_row_count_with_table_result["result"]["partial_unexpected_list"] =[]
-        check_table_row_count_with_table_result["result"]["partial_unexpected_list"].append(tc_table + ": " + str(a_count) + " - " + tc_Parameters + ": " + str(b_count))
-        check_table_row_count_with_table_result["result"]["unexpected_count"]= 1
-        check_table_row_count_with_table_result["result"]["unexpected_percent"]= 1
-  except Exception as e:
-    result_error = result_error_exception(check_table_row_count_with_table_result,e)
-    return result_error  
-  return check_table_row_count_with_table_result
+# def check_table_row_count_with_source_table(Table, SourcePath, Parameters):
+#   tc_Parameters = Parameters
+#   tc_table = SourcePath + '.' + Table
+#   check_table_row_count_with_table_result = result_default()
+#   try:
+#     sql_count = "SELECT COUNT(*) as table_a_count FROM " + tc_table
+#     table_a_count = spark.sql(sql_count)
+#     a_count = table_a_count.first().table_a_count
+#     sql_count_raw = "SELECT COUNT(*) as table_b_count FROM " + tc_Parameters
+#     table_b_count = readSql(sql_count_raw)
+#     b_count = table_b_count.first().table_b_count
+#     if a_count != b_count:
+#         check_table_row_count_with_table_result["success"] = False
+#         check_table_row_count_with_table_result["result"]["partial_unexpected_list"] =[]
+#         check_table_row_count_with_table_result["result"]["partial_unexpected_list"].append(tc_table + ": " + str(a_count) + " - " + tc_Parameters + ": " + str(b_count))
+#         check_table_row_count_with_table_result["result"]["unexpected_count"]= 1
+#         check_table_row_count_with_table_result["result"]["unexpected_percent"]= 1
+#   except Exception as e:
+#     result_error = result_error_exception(check_table_row_count_with_table_result,e)
+#     return result_error  
+#   return check_table_row_count_with_table_result
 
 def execute_tc(TestSuiteCode, TestCaseCode, Model, TestCase, Table, Filter, Parameters, Sets, geDF, Sourcepath, source_df):
   test_start_time = set_time_now()
   tc_TestSuiteCode = TestSuiteCode
   tc_TestCaseCode = TestCaseCode
   tc_Table = Table
   tc_Sets = Sets 
@@ -477,16 +484,16 @@
     ResultData = validate_percentage_of_values_in_columns(geDF,tc_Parameters,tc_Sets)
   elif tc_TestCase == 'Validate Key Value Connection':
     ResultData = validate_key_value_connections(source_df, tc_Sets, tc_Parameters, tc_sourcepath)
   elif tc_TestCase == 'Validate if start date after end date':
     ResultData = validate_if_startdate_after_enddate(geDF, tc_Sets)
   elif tc_TestCase == 'Check orphan values in column table':
     ResultData = check_orphan_values_in_column_table(source_df,Sets,Filter,Parameters)  
-  elif tc_TestCase == 'Check table row count with source table':
-    ResultData = check_table_row_count_with_source_table(Table,Sourcepath,Parameters)
+  # elif tc_TestCase == 'Check table row count with source table':
+  #   ResultData = check_table_row_count_with_source_table(Table,Sourcepath,Parameters)
   elif tc_TestCase == 'Validate list of values in column':    
     ResultData = validate_list_of_values_in_column(geDF,tc_Parameters,tc_Sets)
   elif tc_TestCase == 'Check column value lengths to be between':      
     ResultData = check_column_value_lengths_to_be_between(geDF,tc_Parameters,tc_Sets)
 #   elif tc_TestCase == 'Validate views in datamart':
 #     ResultData = Validate_views_in_datamart(source_df)  
   else:
@@ -515,7 +522,28 @@
   f_result['test_start_time'] = start_time
   f_result['test_end_time'] = end_time
   return f_result
 
 def AddResult(j_testrun,j_testcase_result):
   j_testrun['run_result'].append(j_testcase_result)
   return j_testrun
+
+# def readSql(query,url,user,password,database):
+#   DF = spark.read\
+#           .format("jdbc")\
+#           .option("url", url)\
+#           .option("user", user)\
+#           .option("password", password)\
+#           .option("database", database)\
+#           .option("forwardSparkAzureStorageCredentials", "true") \
+#           .option("query", query)\
+#           .load()
+#   # DF = spark.read\
+#   #           .format("jdbc")\
+#   #           .option("url", dbutils.secrets.get(scope = vault_scope, key = sqldw_conn))\
+#   #           .option("user", dbutils.secrets.get(scope = vault_scope, key = sqldw_user))\
+#   #           .option("password", dbutils.secrets.get(scope = vault_scope, key = sqldw_pwd))\
+#   #           .option("database", dbutils.secrets.get(scope = vault_scope, key = "SQL-SDW-DatabaseName"))\
+#   #           .option("forwardSparkAzureStorageCredentials", "true") \
+#   #           .option("query", query)\
+#   #           .load()
+#   return DF
```

