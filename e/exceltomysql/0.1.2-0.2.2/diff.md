# Comparing `tmp/exceltomysql-0.1.2.tar.gz` & `tmp/exceltomysql-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\exceltomysql-0.1.2.tar", last modified: Tue Dec 29 21:56:08 2020, max compression
+gzip compressed data, was "exceltomysql-0.2.2.tar", last modified: Thu Jun  1 21:41:12 2023, max compression
```

## Comparing `exceltomysql-0.1.2.tar` & `exceltomysql-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/
--rw-rw-rw-   0        0        0     2976 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1849 2020-12-29 21:46:06.000000 exceltomysql-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/exceltomysql/
--rw-rw-rw-   0        0        0      301 2020-12-29 21:34:31.000000 exceltomysql-0.1.2/exceltomysql/__init__.py
--rw-rw-rw-   0        0        0      396 2020-12-29 21:34:17.000000 exceltomysql-0.1.2/exceltomysql/_api.py
--rw-rw-rw-   0        0        0     2763 2020-12-29 21:54:45.000000 exceltomysql-0.1.2/exceltomysql/exceltomysql.py
-drwxrwxrwx   0        0        0        0 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/exceltomysql.egg-info/
--rw-rw-rw-   0        0        0     2976 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/exceltomysql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/exceltomysql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/exceltomysql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/exceltomysql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-29 21:56:08.000000 exceltomysql-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1464 2020-12-29 21:55:39.000000 exceltomysql-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:41:12.083690 exceltomysql-0.2.2/
+-rw-rw-rw-   0        0        0     1082 2020-12-28 22:31:19.000000 exceltomysql-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2346 2023-06-01 21:41:12.081694 exceltomysql-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1849 2023-06-01 21:37:26.000000 exceltomysql-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 21:41:12.045711 exceltomysql-0.2.2/exceltomysql/
+-rw-rw-rw-   0        0        0      328 2023-06-01 21:37:55.000000 exceltomysql-0.2.2/exceltomysql/__init__.py
+-rw-rw-rw-   0        0        0      396 2020-12-29 21:34:17.000000 exceltomysql-0.2.2/exceltomysql/_api.py
+-rw-rw-rw-   0        0        0     2662 2023-06-01 21:40:05.000000 exceltomysql-0.2.2/exceltomysql/exceltomysql.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:41:12.078691 exceltomysql-0.2.2/exceltomysql.egg-info/
+-rw-rw-rw-   0        0        0     2346 2023-06-01 21:41:11.000000 exceltomysql-0.2.2/exceltomysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-01 21:41:11.000000 exceltomysql-0.2.2/exceltomysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 21:41:11.000000 exceltomysql-0.2.2/exceltomysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 21:41:11.000000 exceltomysql-0.2.2/exceltomysql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 21:41:12.083690 exceltomysql-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-06-01 21:32:12.000000 exceltomysql-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `exceltomysql-0.1.2/README.md` & `exceltomysql-0.2.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -19,57 +19,57 @@
 👍   [pymysql](http://www.pymssql.org/)
 
 👍   [sqlalchemy](https://www.sqlalchemy.org/)
 
 # QuickStart
 
 ```python
-import exceltomysq as em
+import exceltomysql as em
 # generate the class instance
 
 # STEP One, prepare your input pareameters
 
 yourFile  = "test01.xls"  # available for xlsx, xls,csv
 yourUsrID = ""
 yourPWD   = ""
 yourDBname= ""
-save2tableName = False  # save your file name table name onto MySQL Server or A string like: "test"
+save2tableName = ""  # Use your filename as tablename to MySQL Server or user define their prefered table name. e.g. : "test"
 
 # get your local host name
 # this will return your local computer name for your MySQL server database
-host_name = em.hostname   
+host_name = em.hostname
 
-# get your local ip address 
+# get your local ip address
 # this will return your local ip address (if your sql server can be accessed by DNS)
-ip = em.local_ip  
+ip = em.local_ip
 
 yourHostORip  = "localhost"   # you need to change your host if needed, dns: local ip address
 
 
-# STEP Two  convert your data to sql server
-em.exceltoDBtable(yourFile,yourHoseORip,yourUsrID,yourPWD,yourDBname,save2tableName)
+# STEP Two  convert your data to MySQL
+em.exceltoDBtable(yourFile, yourHoseORip, yourUsrID, yourPWD, yourDBname, rename_table)
 
 
 ```
 
 ```python
 output:
 Successfully load excel data...
 Secessfully connected to MySQL Server...
-Secessfully saved 'yourtable' into SQL Server...
+Secessfully saved 'yourtable' to MySQL Server...
 ```
 
 # API Reference
 
-exceltosqlserver.exceltoDBtable(`filePath,hostORip=False,usrID =False,pwd=False,database=False,save2tableName`)
+exceltosqlserver.exceltoDBtable(`filePath, hostORip ="", usrID = "", pwd = "", database = "", rename_table = ""`)
 
 filePath: str
 
-hostORip: str  default :False
+hostORip: str  default :""
 
-usrID: str  default: False
+usrID: str  default: ""
 
-pwd: str   default: False
+pwd: str   default: ""
 
-database: str  default:False
+database: str  default: ""
 
-save2tableName: str   default:False, will auto save your file name as table name  into mysql database. If assignmed value, will change table name from your file name to the assigned value.
+rename_table: str   default: "",  will auto save your filename as tablename to MySQL Database. If assignmed value, will change tablename from your filename to the assigned value.
```

### Comparing `exceltomysql-0.1.2/exceltomysql/exceltomysql.py` & `exceltomysql-0.2.2/exceltomysql/exceltomysql.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,74 +2,73 @@
 ##############################################################
 # Created Date: Monday, December 28th 2020
 # Contact Info: luoxiangyong01@gmail.com
 # Author/Copyright: Mr. Xiangyong Luo
 ##############################################################
 
 
+import socket
+
 import pandas as pd
 import pymysql
 import pyodbc
 from sqlalchemy import create_engine
 
-import socket
-
 hostname = socket.gethostname()
 local_ip = socket.gethostbyname(hostname)
 
 
-# Pandas to sql need to use sqlalcemy to create engine
-
-
 class exceltoDBtable:
     #  Available for sql server and mysql now
-    def __init__(self,filePath,server=False,usrID =False,pwd=False,database=False,save2tableName=False):
-        if not any([server,database,usrID,pwd]):
+    def __init__(self,
+                 filePath: str,
+                 server: str = "",
+                 usrID: str = "",
+                 pwd: str = "",
+                 database: str = "",
+                 rename_table: str = ""):
+
+        if not any([server, database, usrID, pwd]):
             raise Exception("Partially inputs, please check your inputs...")
-        else:
-            self.filePath = filePath
-            self.server = server
-            self.database=database
-            self.usrID = usrID
-            self.pwd = pwd
-            self.save2tableName = save2tableName
-        self.dbType = ["mysql","sqlserver"]
+
+        self.filePath = filePath
+        self.server = server
+        self.database = database
+        self.usrID = usrID
+        self.pwd = pwd
+        self.rename_table = rename_table
         self.readData()
         self.connect2DB()
         self.save2database()
 
-    def connect2DB(self) -> "Connect to Database Server":
-    
+    def connect2DB(self) -> None:
+
         try:
             # self.conn = pymysql.connect(host=self.server,user=self.usrID,password=self.pwd,db=self.database,charset="utf8",cursorclass=pymysql.cursors.DictCursor)
-            
-            self.engine = create_engine('mysql+pymysql://%s:%s@%s:3306/%s'%(self.usrID,self.pwd,self.server,self.database))
+            self.engine = create_engine('mysql+pymysql://%s:%s@%s:3306/%s' % (self.usrID, self.pwd, self.server, self.database))
             print("Successfully connected to MySQL...")
-        except:
-            raise Exception("Can not connect to %s, please check your input info."%self.dbType)
+        except Exception:
+            raise Exception("Can not connect to MySQL, please check your input info.")
 
-    def readData(self) -> "DataFrame":
-        if self.filePath.split(".")[-1] in ["xlsx","xls"]:
+    def readData(self) -> None:
+        if self.filePath.split(".")[-1] in ["xlsx", "xls"]:
             self.file_data = pd.read_excel(self.filePath)
             print("Successfully load excel data...")
         elif self.filePath.split(".")[-1] in ["csv"]:
             self.file_data = pd.read_csv(self.filePath)
             print("Successfully load csv data...")
         else:
             raise Exception("Unable to load input file...")
 
-    def save2database(self) ->"DataFrame to database":
-        if self.save2tableName:
-            tableName = self.save2tableName
+    def save2database(self) -> None:
+        if self.rename_table:
+            tableName = self.rename_table
+        elif "/" in self.filePath:
+            tableName = self.filePath.split("/")[-1].split(".")[0]
         else:
-            if "/" in self.filePath:
-                tableName = self.filePath.split("/")[-1].split(".")[0]
-            else:
-                tableName = self.filePath.split(".")[0]
+            tableName = self.filePath.split(".")[0]
+
         try:
-            self.file_data.to_sql(tableName,con=self.engine)
-            print("Successfully save %s into database..."%tableName)
+            self.file_data.to_sql(tableName, con=self.engine)
+            print("Successfully save %s into database..." % tableName)
         except Exception as e:
             raise Exception(e)
-
-
-
```

### Comparing `exceltomysql-0.1.2/setup.py` & `exceltomysql-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 ##############################################################
 
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
-    
+
 try:
     # if have requirements.txt file inside the folder
     with open("requirements.txt", "r", encoding="utf-8") as f:
-        modules_needed = [i.strip() for i in fh.readlines()]   
+        modules_needed = [i.strip() for i in fh.readlines()]
 except:
     modules_needed = []
 
 setuptools.setup(
     name="exceltomysql", # Replace with your own username
-    version="0.1.2",
+    version="0.2.2",
     author="Xiangyong Luo",
     author_email="rochemay@163.com",
-    description="This package help to convert your excel files (xlsx,xls,csv) to MySQL database.",
+    description="This package help convert your excel files (xlsx,xls,csv) to MySQL Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xiangyongluo/exceltomysql",
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=modules_needed,
-    
+
     packages=setuptools.find_packages(),
     include_package_data=True,
-    package_data= {'':['*.txt','*.xls','*.xlsx','*.csv'],
-                   "test_data":['*.xls']}
+    package_data={'': ['*.txt', '*.xls', '*.xlsx', '*.csv'],
+                  "test_data": ['*.xls']}
 )
```

