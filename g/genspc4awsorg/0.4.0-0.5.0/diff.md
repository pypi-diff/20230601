# Comparing `tmp/genspc4awsorg-0.4.0.tar.gz` & `tmp/genspc4awsorg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/H/SynologyDrive/Drive/wslhome/py/steampipe-conn-generator-for-aws-organization/dist/tmp1h5job4z/genspc4awsorg-0.4.", last modified: Tue Jun 14 09:19:21 2022, max compression
+gzip compressed data, was "genspc4awsorg-0.5.0.tar", last modified: Thu Jun  1 05:16:09 2023, max compression
```

## Comparing `genspc4awsorg-0.4.0.tar` & `genspc4awsorg-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 hal       (1000) hal       (1000)        0 2022-06-14 09:19:21.000000 genspc4awsorg-0.4.0/
--rwxrwxrwx   0 hal       (1000) hal       (1000)    35149 2022-04-22 14:21:12.000000 genspc4awsorg-0.4.0/LICENSE
--rwxrwxrwx   0 hal       (1000) hal       (1000)     4555 2022-06-14 09:19:21.000000 genspc4awsorg-0.4.0/PKG-INFO
--rwxrwxrwx   0 hal       (1000) hal       (1000)     3680 2022-04-27 13:29:31.000000 genspc4awsorg-0.4.0/README.md
--rwxrwxrwx   0 hal       (1000) hal       (1000)       80 2022-04-23 09:31:41.000000 genspc4awsorg-0.4.0/pyproject.toml
--rwxrwxrwx   0 hal       (1000) hal       (1000)     1123 2022-06-14 09:19:21.000000 genspc4awsorg-0.4.0/setup.cfg
-drwxrwxrwx   0 hal       (1000) hal       (1000)        0 2022-06-14 09:19:21.000000 genspc4awsorg-0.4.0/src/
-drwxrwxrwx   0 hal       (1000) hal       (1000)        0 2022-06-14 09:19:21.000000 genspc4awsorg-0.4.0/src/genspc4awsorg/
--rwxrwxrwx   0 hal       (1000) hal       (1000)        0 2022-04-22 06:42:24.000000 genspc4awsorg-0.4.0/src/genspc4awsorg/__init__.py
--rwxrwxrwx   0 hal       (1000) hal       (1000)    10545 2022-06-14 09:18:17.000000 genspc4awsorg-0.4.0/src/genspc4awsorg/__main__.py
-drwxrwxrwx   0 hal       (1000) hal       (1000)        0 2022-06-14 09:19:21.000000 genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/
--rwxrwxrwx   0 hal       (1000) hal       (1000)     4555 2022-06-14 09:19:20.000000 genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/PKG-INFO
--rwxrwxrwx   0 hal       (1000) hal       (1000)      350 2022-06-14 09:19:21.000000 genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/SOURCES.txt
--rwxrwxrwx   0 hal       (1000) hal       (1000)        1 2022-06-14 09:19:20.000000 genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/dependency_links.txt
--rwxrwxrwx   0 hal       (1000) hal       (1000)       62 2022-06-14 09:19:20.000000 genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/entry_points.txt
--rwxrwxrwx   0 hal       (1000) hal       (1000)       14 2022-06-14 09:19:20.000000 genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/requires.txt
--rwxrwxrwx   0 hal       (1000) hal       (1000)       14 2022-06-14 09:19:20.000000 genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:16:09.979403 genspc4awsorg-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 05:16:01.000000 genspc4awsorg-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-01 05:16:09.979403 genspc4awsorg-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-01 05:16:01.000000 genspc4awsorg-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 05:16:01.000000 genspc4awsorg-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-01 05:16:09.979403 genspc4awsorg-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:16:09.975403 genspc4awsorg-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:16:09.975403 genspc4awsorg-0.5.0/src/genspc4awsorg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 05:16:01.000000 genspc4awsorg-0.5.0/src/genspc4awsorg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-06-01 05:16:01.000000 genspc4awsorg-0.5.0/src/genspc4awsorg/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 05:16:09.979403 genspc4awsorg-0.5.0/src/genspc4awsorg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-01 05:16:09.000000 genspc4awsorg-0.5.0/src/genspc4awsorg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-01 05:16:09.000000 genspc4awsorg-0.5.0/src/genspc4awsorg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 05:16:09.000000 genspc4awsorg-0.5.0/src/genspc4awsorg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 05:16:09.000000 genspc4awsorg-0.5.0/src/genspc4awsorg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 05:16:09.000000 genspc4awsorg-0.5.0/src/genspc4awsorg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 05:16:09.000000 genspc4awsorg-0.5.0/src/genspc4awsorg.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `genspc4awsorg-0.4.0/LICENSE` & `genspc4awsorg-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `genspc4awsorg-0.4.0/PKG-INFO` & `genspc4awsorg-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: genspc4awsorg
-Version: 0.4.0
-Summary: Generate steampipe connection file(.spc) for accounts and OUs in specified AWS organization. Before run this script, please make sure correct AWS credential in envs(using aws-vault is recommend), and base credential profile which can AssumeRole to accounts accross organization has been configured.
-Home-page: https://github.com/happy240/steampipe-conn-generator-for-aws-organization
-Author: Henry Huo
-Author-email: happy78@live.com
-Project-URL: Bug Tracker, https://github.com/happy240/steampipe-conn-generator-for-aws-organization/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Steampipe connection configuration file generator for AWS accounts accross organization
 
 [Steampipe](https://github.com/turbot/steampipe) is an excellent utility which users can use SQL to instantly query your cloud services (AWS, Azure, GCP and more).
 
 When use steampipe for AWS organization accounts at scale, [build connection configuration file](https://steampipe.io/docs/managing/connections) can be a complex and time consuming task. This python script generate steampipe connection file(.spc) for accounts and OUs in specified AWS organization.
 
 ## Prerequisites:
@@ -62,46 +47,42 @@
 ## How genspc4awsorg works
 This script will travers accounts and OUs accross AWS organization and generate an .spc file in ~/.steampipe/config/.
 There will be a connection for every account with name rule '<PREFIX_ACCOUNT ID>', and a aggregator connection with name rule '<PREFIX_OU NAME>'.
 genspc4awsorg will create profiles in ~/.aws/config for every accounts by default, which can be used with awscli and other tools, this action can be ignored with -nc switch.
 
 ## Usage
 ```
-genspc4awsorg \[-h\] \[-sp SOURCEPROFILE\] \[-mfa MFASERIAL\]
-
-                        \[-r ROLENAME\] \[-nc\]
+usage: genspc4awsorg [-h] [-sp SOURCEPROFILE] [-mfa MFASERIAL] [-ir] [-r ROLENAME] [-nc] [-si SOURCE_IDENTITY]
+                     [-st SESSION_TAGS] [-tst TRANSITIVE_SESSION_TAGS] [-ttl CACHE_TTL] [-p PROFILE]
+                     orgprefix
+
+Generate steampipe connection file(.spc) for accounts and OUs in specified AWS organization.Before run this script, please   
+make sure correct AWS credential in envs(using aws-vault is recommend), and base credential profile which can AssumeRole to  
+accounts accross organization has been configured.
 
-                        orgprefix
-```
 positional arguments:
-
-  orgprefix             Prefix for AWS organization, used in steampipe
-
-                        connection names.
+  orgprefix             Prefix for AWS organization, used in steampipe connection names.
 
 optional arguments:
-
-  -h, --help            show this help message and exit
-
-  -sp SOURCEPROFILE, --sourceprofile SOURCEPROFILE
-
-                        AWS credential profile(in ~/.aws/credentials) which
-
-                        can AssumeRole to accounts accross organization.if not
-
-                        provided, default to same value of $orgprefix
-
-  -mfa MFASERIAL, --mfaserial MFASERIAL
-
-                        Mfa serial arn used to access target account.
-
-  -r ROLENAME, --rolename ROLENAME
-
-                        Role name used to access target account. Default to
-
-                        "OrganizationAccountAccessRole"
-
-  -nc, --ignoreconfigprofile
-
-                        Create steampipe connection config only, NO
-
-                        ~/.aws/config profiles.
+  -h, --help            show this help message and exit
+  -sp SOURCEPROFILE, --sourceprofile SOURCEPROFILE
+                        AWS credential profile(in ~/.aws/credentials) which can AssumeRole to accounts accross
+                        organization.if not provided, default to same value of $orgprefix.Ignored when use "--useec2role"    
+                        option.
+  -mfa MFASERIAL, --mfaserial MFASERIAL
+                        Mfa serial arn used to access target account.
+  -ir, --useec2role     Use EC2 Instance Role credential instead of source profile.
+  -r ROLENAME, --rolename ROLENAME
+                        Role name used to access target account. Default to "OrganizationAccountAccessRole"
+  -nc, --ignoreconfigprofile
+                        Create steampipe connection config only, NO ~/.aws/config profiles.
+  -si SOURCE_IDENTITY, --source_identity SOURCE_IDENTITY
+                        "source_identity" in ~/.aws/config profile.
+  -st SESSION_TAGS, --session_tags SESSION_TAGS
+                        "session_tags" in ~/.aws/config profile.
+  -tst TRANSITIVE_SESSION_TAGS, --transitive_session_tags TRANSITIVE_SESSION_TAGS
+                        "transit_session_tags" in ~/.aws/config profile.
+  -ttl CACHE_TTL, --cache_ttl CACHE_TTL
+                        Cache TTL in seconds. Default to 300.
+  -p PROFILE, --profile PROFILE
+                        Base profile used to get organization info.
+```
```

### Comparing `genspc4awsorg-0.4.0/setup.cfg` & `genspc4awsorg-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = genspc4awsorg
-version = 0.4.0
+version = 0.5.0
 author = Henry Huo
 author_email = happy78@live.com
 description = Generate steampipe connection file(.spc) for accounts and OUs in specified AWS organization. Before run this script, please make sure correct AWS credential in envs(using aws-vault is recommend), and base credential profile which can AssumeRole to accounts accross organization has been configured.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/happy240/steampipe-conn-generator-for-aws-organization
 project_urls =
```

### Comparing `genspc4awsorg-0.4.0/src/genspc4awsorg.egg-info/PKG-INFO` & `genspc4awsorg-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genspc4awsorg
-Version: 0.4.0
+Version: 0.5.0
 Summary: Generate steampipe connection file(.spc) for accounts and OUs in specified AWS organization. Before run this script, please make sure correct AWS credential in envs(using aws-vault is recommend), and base credential profile which can AssumeRole to accounts accross organization has been configured.
 Home-page: https://github.com/happy240/steampipe-conn-generator-for-aws-organization
 Author: Henry Huo
 Author-email: happy78@live.com
 Project-URL: Bug Tracker, https://github.com/happy240/steampipe-conn-generator-for-aws-organization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -62,46 +62,42 @@
 ## How genspc4awsorg works
 This script will travers accounts and OUs accross AWS organization and generate an .spc file in ~/.steampipe/config/.
 There will be a connection for every account with name rule '<PREFIX_ACCOUNT ID>', and a aggregator connection with name rule '<PREFIX_OU NAME>'.
 genspc4awsorg will create profiles in ~/.aws/config for every accounts by default, which can be used with awscli and other tools, this action can be ignored with -nc switch.
 
 ## Usage
 ```
-genspc4awsorg \[-h\] \[-sp SOURCEPROFILE\] \[-mfa MFASERIAL\]
+usage: genspc4awsorg [-h] [-sp SOURCEPROFILE] [-mfa MFASERIAL] [-ir] [-r ROLENAME] [-nc] [-si SOURCE_IDENTITY]
+                     [-st SESSION_TAGS] [-tst TRANSITIVE_SESSION_TAGS] [-ttl CACHE_TTL] [-p PROFILE]
+                     orgprefix
+
+Generate steampipe connection file(.spc) for accounts and OUs in specified AWS organization.Before run this script, please   
+make sure correct AWS credential in envs(using aws-vault is recommend), and base credential profile which can AssumeRole to  
+accounts accross organization has been configured.
 
-                        \[-r ROLENAME\] \[-nc\]
-
-                        orgprefix
-```
 positional arguments:
-
-  orgprefix             Prefix for AWS organization, used in steampipe
-
-                        connection names.
+  orgprefix             Prefix for AWS organization, used in steampipe connection names.
 
 optional arguments:
-
-  -h, --help            show this help message and exit
-
-  -sp SOURCEPROFILE, --sourceprofile SOURCEPROFILE
-
-                        AWS credential profile(in ~/.aws/credentials) which
-
-                        can AssumeRole to accounts accross organization.if not
-
-                        provided, default to same value of $orgprefix
-
-  -mfa MFASERIAL, --mfaserial MFASERIAL
-
-                        Mfa serial arn used to access target account.
-
-  -r ROLENAME, --rolename ROLENAME
-
-                        Role name used to access target account. Default to
-
-                        "OrganizationAccountAccessRole"
-
-  -nc, --ignoreconfigprofile
-
-                        Create steampipe connection config only, NO
-
-                        ~/.aws/config profiles.
+  -h, --help            show this help message and exit
+  -sp SOURCEPROFILE, --sourceprofile SOURCEPROFILE
+                        AWS credential profile(in ~/.aws/credentials) which can AssumeRole to accounts accross
+                        organization.if not provided, default to same value of $orgprefix.Ignored when use "--useec2role"    
+                        option.
+  -mfa MFASERIAL, --mfaserial MFASERIAL
+                        Mfa serial arn used to access target account.
+  -ir, --useec2role     Use EC2 Instance Role credential instead of source profile.
+  -r ROLENAME, --rolename ROLENAME
+                        Role name used to access target account. Default to "OrganizationAccountAccessRole"
+  -nc, --ignoreconfigprofile
+                        Create steampipe connection config only, NO ~/.aws/config profiles.
+  -si SOURCE_IDENTITY, --source_identity SOURCE_IDENTITY
+                        "source_identity" in ~/.aws/config profile.
+  -st SESSION_TAGS, --session_tags SESSION_TAGS
+                        "session_tags" in ~/.aws/config profile.
+  -tst TRANSITIVE_SESSION_TAGS, --transitive_session_tags TRANSITIVE_SESSION_TAGS
+                        "transit_session_tags" in ~/.aws/config profile.
+  -ttl CACHE_TTL, --cache_ttl CACHE_TTL
+                        Cache TTL in seconds. Default to 300.
+  -p PROFILE, --profile PROFILE
+                        Base profile used to get organization info.
+```
```

