# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230531174947.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230601153606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230531174947.tar", last modified: Wed May 31 17:50:29 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230601153606.tar", last modified: Thu Jun  1 15:36:46 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:50:29.548801 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-31 17:49:40.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:50:29.548801 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-31 17:49:40.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 17:50:29.548801 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 17:50:26.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:50:29.548801 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:50:29.548801 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 17:49:40.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10281 2023-05-31 17:49:40.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-05-31 17:49:40.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 17:50:29.548801 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-31 17:50:29.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-31 17:50:29.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 17:50:29.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-31 17:50:29.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 17:50:29.000000 echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-01 15:36:44.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11349 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-06-01 15:36:00.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:36:46.859203 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 15:36:46.000000 echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230531174947
+Version: 1.0.0.dev20230601153606
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230531174947",
+  version="1.0.0.dev20230601153606",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,14 +135,43 @@
             #      [2] Calibrated w/o calibration data
             #      [3] uncalibrated
             calibration_status['CAL_STATE'] = calibration_status['CAL_STATE'].apply(lambda x: x.find('Calibrated') >= 0)
         else:
             print(f"Unsuccessful S3 get_object response. Status - {status}")
         return calibration_status
 
+
+    def __truncateTable(self, dynamo, tableName):
+        table = dynamo.Table(tableName)
+
+        #get the table keys
+        tableKeyNames = [key.get("AttributeName") for key in table.key_schema]
+
+        #Only retrieve the keys for each item in the table (minimize data transfer)
+        projectionExpression = ", ".join('#' + key for key in tableKeyNames)
+        expressionAttrNames = {'#'+key: key for key in tableKeyNames}
+
+        counter = 0
+        page = table.scan(ProjectionExpression=projectionExpression, ExpressionAttributeNames=expressionAttrNames)
+        with table.batch_writer() as batch:
+            while page["Count"] > 0:
+                counter += page["Count"]
+                # Delete items in batches
+                for itemKeys in page["Items"]:
+                    batch.delete_item(Key=itemKeys)
+                # Fetch the next page
+                if 'LastEvaluatedKey' in page:
+                    page = table.scan(
+                        ProjectionExpression=projectionExpression, ExpressionAttributeNames=expressionAttrNames,
+                        ExclusiveStartKey=page['LastEvaluatedKey'])
+                else:
+                    break
+        print(f"Deleted {counter}")
+
+
     def execute(self, message):
         session = boto3.Session()
         dynamodb = session.client(service_name='dynamodb')
         s3 = session.client(service_name='s3', config=botocore.config.Config(max_pool_connections=self.max_pool_connections))
 
 
 
@@ -152,19 +181,16 @@
         #
         subset_ek60_by_prefix = self.__get_subset_ek60_prefix(
             df=all_objects[all_objects['Key'].str.contains('EK60')][['Key', 'Size']]
         )
         subset_datagrams = self.__get_subset_datagrams(df=subset_ek60_by_prefix)
         ek60_objects = self.__get_ek60_objects(subset_ek60_by_prefix, subset_datagrams)
         print(start)  # 1:26:57 to 1:39:??
-        #
-        # current_tables = self.dynamodb.list_tables()
-        # if self.index_ek60_table_name in current_tables['TableNames']:
-        #     print('deleting existing table')
-        #     self.__delete_table()
+
+        self.__truncateTable(dynamodb, self.index_ek60_table_name)
 
         calibration_status = self.__get_calibration_information(s3)
         #
         # TODO: melt calibration_status with
         # ek60_objects['CALIBRATED'] = np.repeat(False, ek60_objects.shape[0])
         # cruises = list(set(ek60_objects['CRUISE']))
         # for i in cruises:
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230531174947/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230601153606/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230531174947
+Version: 1.0.0.dev20230601153606
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

