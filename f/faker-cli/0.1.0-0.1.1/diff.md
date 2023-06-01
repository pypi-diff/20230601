# Comparing `tmp/faker_cli-0.1.0.tar.gz` & `tmp/faker_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker_cli-0.1.0.tar", max compression
+gzip compressed data, was "faker_cli-0.1.1.tar", max compression
```

## Comparing `faker_cli-0.1.0.tar` & `faker_cli-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-26 07:16:29.115396 faker_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     2829 2023-05-26 07:16:29.115396 faker_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-26 07:16:29.115396 faker_cli-0.1.0/faker_cli/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-26 07:16:29.119396 faker_cli-0.1.0/faker_cli/cli.py
--rw-r--r--   0        0        0    26455 2023-05-26 07:16:29.119396 faker_cli-0.1.0/faker_cli/templates.py
--rw-r--r--   0        0        0      809 2023-05-26 07:16:29.119396 faker_cli-0.1.0/faker_cli/writer.py
--rw-r--r--   0        0        0      461 2023-05-26 07:16:53.423462 faker_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3302 1970-01-01 00:00:00.000000 faker_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-01 06:00:07.671393 faker_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2916 2023-06-01 06:00:07.671393 faker_cli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/__init__.py
+-rw-r--r--   0        0        0     2799 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/cli.py
+-rw-r--r--   0        0        0    27694 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/templates.py
+-rw-r--r--   0        0        0      809 2023-06-01 06:00:07.671393 faker_cli-0.1.1/faker_cli/writer.py
+-rw-r--r--   0        0        0      461 2023-06-01 06:00:12.147436 faker_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 faker_cli-0.1.1/PKG-INFO
```

### Comparing `faker_cli-0.1.0/LICENSE` & `faker_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `faker_cli-0.1.0/README.md` & `faker_cli-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 {"id": 6986, "awesome_name": "ballen", "last_attention_at": "2023-01-08"}
 {"id": 6892, "awesome_name": "jennifer61", "last_attention_at": "2023-01-03"}
 {"id": 1967, "awesome_name": "jmendoza", "last_attention_at": "2023-01-23"}
 ```
 
 ## Templates
 
-As of now,the only amazing best template supported ever is `s3access`.
-
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
 fake -t s3access -n 10
-```
+```
+
+How about CloudFront? Go ahead.
+
+```bash
+fake -t cloudfront -n 10
+```
+
+> **Warning**: Both of these templates are still being validated - please be cautious!
```

### Comparing `faker_cli-0.1.0/faker_cli/cli.py` & `faker_cli-0.1.1/faker_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,24 +24,38 @@
 TEMPLATE_MAPPER = {
     "s3access": [S3AccessWriter, "s3_access_log"],
     "cloudfront": [CloudFrontWriter, "cloudfront_log"],
 }
 
 fake = Faker()
 fake.add_provider(S3AccessLogs)
-fake.add_provider(CloudTrailLogs)
 fake.add_provider(CloudFrontLogs)
 
 @click.command()
 @click.option("--num-rows", "-n", default=1, help="Number of rows")
 @click.option("--format", "-f", type=click.Choice(["csv", "json"]), default="csv", help="Format of the output")
 @click.option("--columns", "-c", help="Column names", default=None, required=False)
 @click.option("--template", "-t", help="Template to use", type=click.Choice(["s3access", "cloudfront"]), default=None)
 @click.argument("column_types", required=False)
 def main(num_rows, format, columns, template, column_types):
+    """
+    Generate fake data, easily.
+
+    COLUMN_TYPES is a comma-seperated list of Faker property names, like
+    pyint,username,date_this_year
+
+    You can also use --template for real-world synthetic data.
+    """
+    if not template and not column_types:
+        ctx = click.get_current_context()
+        click.echo(ctx.get_help())
+        ctx.exit()
+        raise click.BadArgumentUsage(
+            "either --template or a list of Faker property names must be provided."
+        )
     if template:
         writer = TEMPLATE_MAPPER[template][0](sys.stdout, None)
         log_entry = TEMPLATE_MAPPER[template][1]
         for i in range(num_rows):
             row = fake.format(log_entry)
             writer.write(row)
         return
```

### Comparing `faker_cli-0.1.0/faker_cli/templates.py` & `faker_cli-0.1.1/faker_cli/templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -213,14 +213,18 @@
         partition: Optional[str] = "aws",
         service: Optional[str] = None,
         region: Optional[str] = None,
         account_id: Optional[str] = None,
         resource_id: Optional[str] = None,
         resource_type: Optional[str] = None,
     ) -> str:
+        """
+        Build an ARN for either a random service or provided.
+        Reference: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference-arns.html
+        """
         if not partition:
             partition = self.generator.random_element(elements=["aws", "aws-cn", "aws-us-gov"])
         if not service:
             service = self.generator.random_element(elements=["s3", "ec2", "iam", "sts"])
         if not region and service not in ["iam"]:
             region = self.generator.random_element(elements=AWSConstants._regions)
         if not account_id:
@@ -237,14 +241,17 @@
         resource_part = resource_id
         if resource_type:
             resource_part = f"{resource_type}/{resource_id}"
 
         return f"arn:{partition}:{service}:{region or ''}:{account_id}:{resource_part}"
 
     def aws_iam_arn(self, service: Optional[str] = None, resource: Optional[str] = None) -> str:
+        """
+        Generate an IAM or STS ARN
+        """
         if service is None:
             service = self.generator.random_element(elements=["iam", "sts"])
         if resource is None:
             if service == "iam":
                 resource = self.generator.random_element(elements=["root", f"user/{self.generator.user_name()}"])
             if service == "sts":
                 resource = self.generator.random_element(
@@ -324,14 +331,15 @@
         ]
 
     def s3_bucket_owner(self) -> str:
         return self._random_alnum(64)
 
     def s3_bucket(self) -> str:
         # return self.generator.random_element(elements=self.bucket_names)
+        # TODO: S3 Buckets should be globally unique
         return self.generator.domain_word()
 
     def s3_bucket_owner_tuple(self) -> str:
         return self.generator.random_element(elements=self.bucket_owner_tuples)
 
     def s3a_time(self) -> str:
         return self.generator.date_time(tzinfo=dt.timezone.utc).strftime("[%d/%b/%Y:%H:%M:%S %z]")
@@ -510,18 +518,28 @@
         return self.aws_arn(service="s3", resource_type="accesspoint")
 
     def acl_required(self) -> str:
         return self.generator.random_element(elements=("Yes", "-"))
 
 
 class CloudTrailLogs(AWSProvider):
+    """
+    There are CloudTrail management events and CloudTrail data events.
+    There is a page [here](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-management-events-with-cloudtrail.html)
+    that has more detail about what each of those are, but in short management events are control plane operations and 
+    data events are operations on specific resources. 
+    Alas, there's no easy way to generate realistic fake versions of these without serious time-consuming work.
+    - CloudTrail list of service topics for each AWS service: https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-aws-service-specific-topics.html
+    - Table of data events: https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-data-events-with-cloudtrail.html
+    - Example of S3 data event: https://docs.aws.amazon.com/AmazonS3/latest/userguide/cloudtrail-logging-s3-info.html#cloudtrail-object-level-tracking
+    """
     __use_weighting__ = True
 
     def event_version(self) -> str:
-        return "1.0"
+        return "1.08"
 
     def event_time(self) -> str:
         return self.generator.iso8601()
 
     def event_source(self) -> str:
         return self.generator.random_element(AWSConstants._services) + ".amazonaws.com"
```

### Comparing `faker_cli-0.1.0/faker_cli/writer.py` & `faker_cli-0.1.1/faker_cli/writer.py`

 * *Files identical despite different names*

### Comparing `faker_cli-0.1.0/PKG-INFO` & `faker_cli-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Damon P. Cortesi
 Author-email: d.lifehacker@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -83,14 +83,20 @@
 {"id": 6986, "awesome_name": "ballen", "last_attention_at": "2023-01-08"}
 {"id": 6892, "awesome_name": "jennifer61", "last_attention_at": "2023-01-03"}
 {"id": 1967, "awesome_name": "jmendoza", "last_attention_at": "2023-01-23"}
 ```
 
 ## Templates
 
-As of now,the only amazing best template supported ever is `s3access`.
-
 Want to generate 1 MILLION S3 Access logs in ~2 minutes? Now you can.
 
 ```bash
 fake -t s3access -n 10
 ```
+
+How about CloudFront? Go ahead.
+
+```bash
+fake -t cloudfront -n 10
+```
+
+> **Warning**: Both of these templates are still being validated - please be cautious!
```

