# Comparing `tmp/exceltosqlserver-0.1.3.tar.gz` & `tmp/exceltosqlserver-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\exceltosqlserver-0.1.3.tar", last modified: Wed Dec 30 02:08:32 2020, max compression
+gzip compressed data, was "exceltosqlserver-0.2.1.tar", last modified: Thu Jun  1 21:14:54 2023, max compression
```

## Comparing `exceltosqlserver-0.1.3.tar` & `exceltosqlserver-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/
--rw-rw-rw-   0        0        0     3051 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1903 2020-12-29 22:06:06.000000 exceltosqlserver-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver/
--rw-rw-rw-   0        0        0       23 2020-12-29 20:38:16.000000 exceltosqlserver-0.1.3/exceltosqlserver/__init__.py
--rw-rw-rw-   0        0        0      493 2020-12-29 21:05:25.000000 exceltosqlserver-0.1.3/exceltosqlserver/_api.py
--rw-rw-rw-   0        0        0     3364 2020-12-30 02:07:29.000000 exceltosqlserver-0.1.3/exceltosqlserver/exceltosqlserver.py
-drwxrwxrwx   0        0        0        0 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver/tesanother/
--rw-rw-rw-   0        0        0      305 2020-12-29 20:35:15.000000 exceltosqlserver-0.1.3/exceltosqlserver/tesanother/__init__.py
--rw-rw-rw-   0        0        0      339 2020-12-29 20:35:26.000000 exceltosqlserver-0.1.3/exceltosqlserver/tesanother/writeMSG.py
-drwxrwxrwx   0        0        0        0 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver/test_data/
--rw-rw-rw-   0        0        0      307 2020-12-29 20:37:07.000000 exceltosqlserver-0.1.3/exceltosqlserver/test_data/__init__.py
--rw-rw-rw-   0        0        0      361 2020-12-29 18:29:06.000000 exceltosqlserver-0.1.3/exceltosqlserver/test_data/writeINtes.py
-drwxrwxrwx   0        0        0        0 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver.egg-info/
--rw-rw-rw-   0        0        0     3051 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/exceltosqlserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-30 02:08:32.000000 exceltosqlserver-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1214 2020-12-30 02:08:14.000000 exceltosqlserver-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:14:54.469389 exceltosqlserver-0.2.1/
+-rw-rw-rw-   0        0        0     1082 2020-12-29 01:16:08.000000 exceltosqlserver-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2399 2023-06-01 21:14:54.467388 exceltosqlserver-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1889 2023-06-01 21:05:08.000000 exceltosqlserver-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 21:14:54.443387 exceltosqlserver-0.2.1/exceltosqlserver/
+-rw-rw-rw-   0        0        0       50 2023-06-01 20:23:39.000000 exceltosqlserver-0.2.1/exceltosqlserver/__init__.py
+-rw-rw-rw-   0        0        0      408 2023-06-01 21:01:31.000000 exceltosqlserver-0.2.1/exceltosqlserver/_api.py
+-rw-rw-rw-   0        0        0     3427 2023-06-01 21:10:58.000000 exceltosqlserver-0.2.1/exceltosqlserver/exceltosqlserver.py
+drwxrwxrwx   0        0        0        0 2023-06-01 21:14:54.464396 exceltosqlserver-0.2.1/exceltosqlserver/test_data/
+-rw-rw-rw-   0        0        0      278 2023-06-01 20:48:13.000000 exceltosqlserver-0.2.1/exceltosqlserver/test_data/__init__.py
+-rw-rw-rw-   0        0        0     8869 2020-12-28 19:44:36.000000 exceltosqlserver-0.2.1/exceltosqlserver/test_data/test01.xls
+drwxrwxrwx   0        0        0        0 2023-06-01 21:14:54.459392 exceltosqlserver-0.2.1/exceltosqlserver.egg-info/
+-rw-rw-rw-   0        0        0     2399 2023-06-01 21:14:54.000000 exceltosqlserver-0.2.1/exceltosqlserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-01 21:14:54.000000 exceltosqlserver-0.2.1/exceltosqlserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 21:14:54.000000 exceltosqlserver-0.2.1/exceltosqlserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-01 21:14:54.000000 exceltosqlserver-0.2.1/exceltosqlserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 21:14:54.469389 exceltosqlserver-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-06-01 21:12:39.000000 exceltosqlserver-0.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `exceltosqlserver-0.1.3/PKG-INFO` & `exceltosqlserver-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 Metadata-Version: 2.1
 Name: exceltosqlserver
-Version: 0.1.3
-Summary: This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.
+Version: 0.2.1
+Summary: This package help convert your excel files (xlsx,xls,csv) to SQL Server Database.
 Home-page: https://github.com/Xiangyongluo/exceltosqlserver
 Author: Xiangyong Luo
 Author-email: rochemay@163.com
-License: UNKNOWN
-Description: # Introduction
-        
-        This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.
-        
-        # Installation
-        
-        exceltomysql can be installed as:
-        
-        ```python
-        pip install exceltosqlserver
-        ```
-        
-        # Dependency
-        
-        👍   [pandas](https://pandas.pydata.org/)
-        
-        👍   [pyodbc](https://github.com/mkleehammer/pyodbc)
-        
-        👍   [sqlalchemy](https://www.sqlalchemy.org/)
-        
-        # QuickStart
-        
-        ```python
-        import exceltosqlserver as es
-        # generate the class instance
-        
-        # STEP One, prepare your input pareameters
-        
-        yourFile  = "test01.xls"  # available for xlsx, xls,csv
-        yourUsrID = ""
-        yourPWD   = ""
-        yourDBname= ""
-        save2tableName = False  # save your file name table name onto SQL Server or A string like: "test"
-        
-        # get your local host name
-        # this will return your local computer name for your sql server database
-        host_name = es.hostname   
-        
-        # get your local ip address 
-        # this will return your local ip address (if your sql server can be accessed by DNS)
-        ip = es.local_ip  
-        
-        # you need to change your host if needed, dns: local ip address
-        #yourHostORip  = "localhost"   
-        # yourHostORip  = host_name
-        yourHostORip  = ip
-        
-        
-        # STEP Two  convert your data to sql server
-        es.exceltoDBtable(yourFile,yourHostORip,yourUsrID,yourPWD,yourDBname,save2tableName)
-        
-        
-        ```
-        
-        ```python
-        output:
-        Successfully load excel data...
-        Secessfully connected to SQL Server...
-        Secessfully saved 'yourtable' into SQL Server...
-        ```
-        
-        # API Reference
-        
-        exceltosqlserver.exceltoDBtable(`filePath,hostORip=False,usrID =False,pwd=False,database=False,save2tableName`)
-        
-        filePath: str
-        
-        hostORip: str  default :False
-        
-        usrID: str  default: False
-        
-        pwd: str   default: False
-        
-        database: str  default:False
-        
-        save2tableName: str   default:False, will auto save your file name as table name  into mysql database. If assignmed value, will change table name from your file name to the assigned value.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Introduction
+
+This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.
+
+# Installation
+
+exceltomysql can be installed as:
+
+```python
+pip install exceltosqlserver
+```
+
+# Dependency
+
+👍   [pandas](https://pandas.pydata.org/)
+
+👍   [pyodbc](https://github.com/mkleehammer/pyodbc)
+
+👍   [sqlalchemy](https://www.sqlalchemy.org/)
+
+# QuickStart
+
+```python
+import exceltosqlserver as es
+# generate the class instance
+
+# STEP One, prepare your input pareameters
+
+yourFile  = "test01.xls"  # available for xlsx, xls,csv
+yourUsrID = ""
+yourPWD   = ""
+yourDBname= ""
+rename_table = ""  # Use your filename as tablename onto SQL Server or user define the table name, e.g. :"test"
+
+# get your local host name
+# this will return your local computer name for your sql server database
+host_name = es.hostname
+
+# get your local ip address
+# this will return your local ip address (if your sql server can be accessed by DNS)
+ip = es.local_ip
+
+# you need to change your host if needed, dns: local ip address
+#yourHostORip  = "localhost"
+# yourHostORip  = host_name
+yourHostORip  = ip
+
+
+# STEP Two add your data to sql server
+es.exceltoDBtable(yourFile, yourHostORip, yourUsrID, yourPWD, yourDBname, rename_table)
+
+
+```
+
+```python
+output:
+Successfully load excel data...
+Sucessfully connected to SQL Server...
+Sucessfully saved 'yourtable' to SQL Server...
+```
+
+# API Reference
+
+exceltosqlserver.exceltoDBtable(`filePath,hostORip=False,usrID =False,pwd=False,database=False,rename_table`)
+
+filePath: str
+
+hostORip: str  default: ""
+
+usrID: str  default: ""
+
+pwd: str   default: ""
+
+database: str  default: ""
+
+rename_table: str   default: "", will auto save your filename as table name  to sql  server database. If assignmed value, will change table name from your filename to the assigned value.
```

### Comparing `exceltosqlserver-0.1.3/README.md` & `exceltosqlserver-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,51 +26,51 @@
 
 # STEP One, prepare your input pareameters
 
 yourFile  = "test01.xls"  # available for xlsx, xls,csv
 yourUsrID = ""
 yourPWD   = ""
 yourDBname= ""
-save2tableName = False  # save your file name table name onto SQL Server or A string like: "test"
+rename_table = ""  # Use your filename as tablename onto SQL Server or user define the table name, e.g. :"test"
 
 # get your local host name
 # this will return your local computer name for your sql server database
-host_name = es.hostname   
+host_name = es.hostname
 
-# get your local ip address 
+# get your local ip address
 # this will return your local ip address (if your sql server can be accessed by DNS)
-ip = es.local_ip  
+ip = es.local_ip
 
 # you need to change your host if needed, dns: local ip address
-#yourHostORip  = "localhost"   
+#yourHostORip  = "localhost"
 # yourHostORip  = host_name
 yourHostORip  = ip
 
 
-# STEP Two  convert your data to sql server
-es.exceltoDBtable(yourFile,yourHostORip,yourUsrID,yourPWD,yourDBname,save2tableName)
+# STEP Two add your data to sql server
+es.exceltoDBtable(yourFile, yourHostORip, yourUsrID, yourPWD, yourDBname, rename_table)
 
 
 ```
 
 ```python
 output:
 Successfully load excel data...
-Secessfully connected to SQL Server...
-Secessfully saved 'yourtable' into SQL Server...
+Sucessfully connected to SQL Server...
+Sucessfully saved 'yourtable' to SQL Server...
 ```
 
 # API Reference
 
-exceltosqlserver.exceltoDBtable(`filePath,hostORip=False,usrID =False,pwd=False,database=False,save2tableName`)
+exceltosqlserver.exceltoDBtable(`filePath,hostORip=False,usrID =False,pwd=False,database=False,rename_table`)
 
 filePath: str
 
-hostORip: str  default :False
+hostORip: str  default: ""
 
-usrID: str  default: False
+usrID: str  default: ""
 
-pwd: str   default: False
+pwd: str   default: ""
 
-database: str  default:False
+database: str  default: ""
 
-save2tableName: str   default:False, will auto save your file name as table name  into mysql database. If assignmed value, will change table name from your file name to the assigned value.
+rename_table: str   default: "", will auto save your filename as table name  to sql  server database. If assignmed value, will change table name from your filename to the assigned value.
```

### Comparing `exceltosqlserver-0.1.3/exceltosqlserver/exceltosqlserver.py` & `exceltosqlserver-0.2.1/exceltosqlserver/exceltosqlserver.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,73 +10,81 @@
 import pyodbc
 from sqlalchemy import create_engine
 import socket
 
 hostname = socket.gethostname()
 local_ip = socket.gethostbyname(hostname)
 
-# Pandas to sql need to use sqlalcemy to create engine
 
 class exceltoDBtable:
     #  Available for sql server and mysql now
-    def __init__(self,filePath,hostORip=False,usrID =False,pwd=False,database=False,save2tableName=False):
-        if not any([hostORip,database,usrID,pwd]):
+    def __init__(self,
+                 filePath: str,
+                 hostORip: str = "",
+                 usrID: str = "",
+                 pwd: str = "",
+                 database: str = "",
+                 rename_table: str = ""):
+
+        if not any([hostORip, database, usrID, pwd]):
             raise Exception("Partially inputs, please check your inputs...")
-        else:
-            self.filePath = filePath
-            self.hostORip = hostORip
-            self.database=database
-            self.usrID = usrID
-            self.pwd = pwd
-            self.save2tableName = save2tableName
-            
+
+        self.filePath = filePath
+        self.hostORip = hostORip
+        self.database = database
+        self.usrID = usrID
+        self.pwd = pwd
+        self.rename_table = rename_table
+
         self.dbType = ["sqlserver"]
         self.readData()
         self.connect2DB()
-        
-    def connect2DB(self) -> "Connect to Database Server":
+
+    def connect2DB(self) -> None:  # sourcery skip: assign-if-exp, extract-method
         # This will test whether a sql server database or a mysql database
-        sqlserverDriver=["{SQL Server}",
-                         "{SQL Native Client}",
-                         "{SQL Server Native Client 10.0}",
-                         "{SQL Server Native Client 11.0}",
-                         "{ODBC Driver 11 for SQL Server}",
-                         "{ODBC Driver 13 for SQL Server}",
-                         "{ODBC Driver 13.1 for SQL Server}",
-                         "{ODBC Driver 17 for SQL Server}"]
+        sqlserverDriver = ["{SQL Server}",
+                           "{SQL Native Client}",
+                           "{SQL Server Native Client 10.0}",
+                           "{SQL Server Native Client 11.0}",
+                           "{ODBC Driver 11 for SQL Server}",
+                           "{ODBC Driver 13 for SQL Server}",
+                           "{ODBC Driver 13.1 for SQL Server}",
+                           "{ODBC Driver 17 for SQL Server}",
+                           "{ODBC Driver 18 for SQL Server}"]
+
         for i in sqlserverDriver:
-            driveString = i.replace(" ","+").replace("{","").replace("}","")
-            # print(driveString)
-            
-            
+            driveString = i.replace(" ", "+").replace("{", "").replace("}", "")
+
             try:
-                self.engine = create_engine("mssql+pyodbc://%s:%s@%s/%s?driver=%s?"%(self.usrID,self.pwd,self.hostORip,self.database,driveString))
-                print("Seccessfully connected to SQL Server...")
-                
-                if self.save2tableName:
-                    tableName = self.save2tableName
+                # connect to sql server
+                self.engine = create_engine(
+                    f"mssql+pyodbc://{self.usrID}:{self.pwd}@{self.hostORip}/{self.database}?driver={driveString}?")
+
+                print("Successfully connected to SQL Server...")
+
+                if self.rename_table:
+                    table_name = self.rename_table
+                elif "/" in self.filePath:
+                    table_name = self.filePath.split("/")[-1].split(".")[0]
                 else:
-                    if "/" in self.filePath:
-                        tableName = self.filePath.split("/")[-1].split(".")[0]
-                    else:
-                        tableName = self.filePath.split(".")[0]
-                
-                self.file_data.to_sql(tableName,con=self.engine)
-                print("Successfully saved %s into SQL Server..."%tableName)
-                return None 
-            except:
+                    table_name = self.filePath.split(".")[0]
+
+                self.file_data.to_sql(table_name, con=self.engine)
+                print("Successfully saved %s into SQL Server..." % table_name)
+                return None
+
+            except Exception:
                 self.engine = False
                 continue
-            
-        raise Exception("Can not save table to sql server, please check your inputs.")
-        
-    def readData(self) -> "DataFrame":
-        if self.filePath.split(".")[-1] in ["xlsx","xls"]:
+
+        raise Exception(
+            "Can not save table to sql server, please check your inputs.")
+
+    def readData(self) -> None:
+        if self.filePath.split(".")[-1] in ["xlsx", "xls"]:
             self.file_data = pd.read_excel(self.filePath)
             print("Successfully load excel data...")
         elif self.filePath.split(".")[-1] in ["csv"]:
             self.file_data = pd.read_csv(self.filePath)
             print("Successfully load csv data...")
         else:
             raise Exception("Unable to load input file...")
-
-
```

### Comparing `exceltosqlserver-0.1.3/exceltosqlserver.egg-info/PKG-INFO` & `exceltosqlserver-0.2.1/exceltosqlserver.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 Metadata-Version: 2.1
 Name: exceltosqlserver
-Version: 0.1.3
-Summary: This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.
+Version: 0.2.1
+Summary: This package help convert your excel files (xlsx,xls,csv) to SQL Server Database.
 Home-page: https://github.com/Xiangyongluo/exceltosqlserver
 Author: Xiangyong Luo
 Author-email: rochemay@163.com
-License: UNKNOWN
-Description: # Introduction
-        
-        This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.
-        
-        # Installation
-        
-        exceltomysql can be installed as:
-        
-        ```python
-        pip install exceltosqlserver
-        ```
-        
-        # Dependency
-        
-        👍   [pandas](https://pandas.pydata.org/)
-        
-        👍   [pyodbc](https://github.com/mkleehammer/pyodbc)
-        
-        👍   [sqlalchemy](https://www.sqlalchemy.org/)
-        
-        # QuickStart
-        
-        ```python
-        import exceltosqlserver as es
-        # generate the class instance
-        
-        # STEP One, prepare your input pareameters
-        
-        yourFile  = "test01.xls"  # available for xlsx, xls,csv
-        yourUsrID = ""
-        yourPWD   = ""
-        yourDBname= ""
-        save2tableName = False  # save your file name table name onto SQL Server or A string like: "test"
-        
-        # get your local host name
-        # this will return your local computer name for your sql server database
-        host_name = es.hostname   
-        
-        # get your local ip address 
-        # this will return your local ip address (if your sql server can be accessed by DNS)
-        ip = es.local_ip  
-        
-        # you need to change your host if needed, dns: local ip address
-        #yourHostORip  = "localhost"   
-        # yourHostORip  = host_name
-        yourHostORip  = ip
-        
-        
-        # STEP Two  convert your data to sql server
-        es.exceltoDBtable(yourFile,yourHostORip,yourUsrID,yourPWD,yourDBname,save2tableName)
-        
-        
-        ```
-        
-        ```python
-        output:
-        Successfully load excel data...
-        Secessfully connected to SQL Server...
-        Secessfully saved 'yourtable' into SQL Server...
-        ```
-        
-        # API Reference
-        
-        exceltosqlserver.exceltoDBtable(`filePath,hostORip=False,usrID =False,pwd=False,database=False,save2tableName`)
-        
-        filePath: str
-        
-        hostORip: str  default :False
-        
-        usrID: str  default: False
-        
-        pwd: str   default: False
-        
-        database: str  default:False
-        
-        save2tableName: str   default:False, will auto save your file name as table name  into mysql database. If assignmed value, will change table name from your file name to the assigned value.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Introduction
+
+This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.
+
+# Installation
+
+exceltomysql can be installed as:
+
+```python
+pip install exceltosqlserver
+```
+
+# Dependency
+
+👍   [pandas](https://pandas.pydata.org/)
+
+👍   [pyodbc](https://github.com/mkleehammer/pyodbc)
+
+👍   [sqlalchemy](https://www.sqlalchemy.org/)
+
+# QuickStart
+
+```python
+import exceltosqlserver as es
+# generate the class instance
+
+# STEP One, prepare your input pareameters
+
+yourFile  = "test01.xls"  # available for xlsx, xls,csv
+yourUsrID = ""
+yourPWD   = ""
+yourDBname= ""
+rename_table = ""  # Use your filename as tablename onto SQL Server or user define the table name, e.g. :"test"
+
+# get your local host name
+# this will return your local computer name for your sql server database
+host_name = es.hostname
+
+# get your local ip address
+# this will return your local ip address (if your sql server can be accessed by DNS)
+ip = es.local_ip
+
+# you need to change your host if needed, dns: local ip address
+#yourHostORip  = "localhost"
+# yourHostORip  = host_name
+yourHostORip  = ip
+
+
+# STEP Two add your data to sql server
+es.exceltoDBtable(yourFile, yourHostORip, yourUsrID, yourPWD, yourDBname, rename_table)
+
+
+```
+
+```python
+output:
+Successfully load excel data...
+Sucessfully connected to SQL Server...
+Sucessfully saved 'yourtable' to SQL Server...
+```
+
+# API Reference
+
+exceltosqlserver.exceltoDBtable(`filePath,hostORip=False,usrID =False,pwd=False,database=False,rename_table`)
+
+filePath: str
+
+hostORip: str  default: ""
+
+usrID: str  default: ""
+
+pwd: str   default: ""
+
+database: str  default: ""
+
+rename_table: str   default: "", will auto save your filename as table name  to sql  server database. If assignmed value, will change table name from your filename to the assigned value.
```

### Comparing `exceltosqlserver-0.1.3/setup.py` & `exceltosqlserver-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
-    
+
 try:
     # if have requirements.txt file inside the folder
     with open("requirements.txt", "r", encoding="utf-8") as f:
-        modules_needed = [i.strip() for i in fh.readlines()]   
-except:
+        modules_needed = [i.strip() for i in fh.readlines()]
+except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="exceltosqlserver", # Replace with your own username
-    version="0.1.3",
+    version="0.2.1",
     author="Xiangyong Luo",
     author_email="rochemay@163.com",
-    description="This package help to convert your excel files (xlsx,xls,csv) to SQL Server database.",
+    description="This package help convert your excel files (xlsx,xls,csv) to SQL Server Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xiangyongluo/exceltosqlserver",
-    
-    
+
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    
+
     install_requires=modules_needed,
     packages=setuptools.find_packages(),
     include_package_data=True,
 
-    package_data= {'':['*.txt','*.xls','*.xlsx','*.csv'],
-                   "test_data":['*.txt']}
+    package_data={'': ['*.txt', '*.xls', '*.xlsx', '*.csv'],
+                  "test_data": ['*.txt']}
 )
 
-
```

