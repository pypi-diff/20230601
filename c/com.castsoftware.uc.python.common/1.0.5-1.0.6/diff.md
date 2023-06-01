# Comparing `tmp/com.castsoftware.uc.python.common-1.0.5.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.0.5.tar", last modified: Tue May 23 17:45:07 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.6.tar", last modified: Thu Jun  1 18:19:38 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.0.5.tar` & `com.castsoftware.uc.python.common-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 17:45:07.472983 com.castsoftware.uc.python.common-1.0.5/
--rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      714 2023-05-23 17:45:07.464557 com.castsoftware.uc.python.common-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 17:45:07.356525 com.castsoftware.uc.python.common-1.0.5/cast_common/
--rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    11918 2023-05-23 14:56:31.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0     7524 2023-05-23 17:44:36.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/highlight.py
--rw-rw-rw-   0        0        0     5478 2023-05-18 15:25:57.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/logger.py
--rw-rw-rw-   0        0        0     5264 2023-05-21 20:59:32.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     6930 2023-05-18 15:27:50.000000 com.castsoftware.uc.python.common-1.0.5/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 17:45:07.449864 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      714 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-23 17:45:07.000000 com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      643 2023-05-23 17:43:34.000000 com.castsoftware.uc.python.common-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 17:45:07.472983 com.castsoftware.uc.python.common-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 18:19:38.006461 com.castsoftware.uc.python.common-1.0.6/
+-rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-06-01 18:19:37.996746 com.castsoftware.uc.python.common-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 18:19:37.883353 com.castsoftware.uc.python.common-1.0.6/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    12884 2023-06-01 16:17:16.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0    10826 2023-05-25 20:32:57.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/highlight.py
+-rw-rw-rw-   0        0        0     5478 2023-05-18 15:25:57.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/logger.py
+-rw-rw-rw-   0        0        0     5264 2023-05-21 20:59:32.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     6953 2023-06-01 18:18:30.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:19:37.981840 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      643 2023-05-31 20:37:12.000000 com.castsoftware.uc.python.common-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:19:38.006461 com.castsoftware.uc.python.common-1.0.6/setup.cfg
```

### Comparing `com.castsoftware.uc.python.common-1.0.5/LICENSE` & `com.castsoftware.uc.python.common-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.5/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.5
+Version: 1.0.6
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.5/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.0.6/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.5/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.0.6/cast_common/aipRestCall.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,35 +66,55 @@
         url = f'{domain_id}/applications/3/results?quality-indicators={key}'
         (status,json) = self.get(url)
         if status == codes.ok and len(json) > 0:
             return json[0]['applicationResults']
         else:
             return None
 
+    def _get_snapshot(self,domain_id):
+        self.debug(f'retrieving latest snapshot information for {domain_id}')
+        (status,json) = self.get(f'{domain_id}/applications/3/snapshots')
+        return status,json
+
+
     def get_latest_snapshot(self,domain_id):
         self.debug(f'retrieving latest snapshot information for {domain_id}')
         snapshot = {}
-        (status,json) = self.get(f'{domain_id}/applications/3/snapshots')
+        (status,json) = self._get_snapshot(domain_id)
         if status == codes.ok and len(json) > 0:
             snapshot['id'] = json[0]['href'].split('/')[-1]  
             snapshot['name'] = json[0]['name']
             snapshot['technology'] = json[0]['technologies']
             snapshot['module_href'] = json[0]['moduleSnapshots']['href']
             snapshot['result_href'] = json[0]['results']['href'] 
         return snapshot 
 
+    def get_prev_snapshot(self,domain_id):
+        self.debug(f'retrieving latest snapshot information for {domain_id}')
+        snapshot = {}
+        (status,json) = self._get_snapshot(domain_id)
+        if status == codes.ok and len(json) > 1:
+            snapshot['id'] = json[1]['href'].split('/')[-1]  
+            snapshot['name'] = json[1]['name']
+            snapshot['technology'] = json[1]['technologies']
+            snapshot['module_href'] = json[1]['moduleSnapshots']['href']
+            snapshot['result_href'] = json[1]['results']['href'] 
+        return snapshot 
+
     def get_grades_by_technology(self,domain_id,snapshot):
         self.debug(f'retrieving grades by technology for domain {domain_id} and snapshot {snapshot}')
         first_tech=True
         grade = DataFrame(columns=list(self._measures.values()))
+        snapshot_id=snapshot['id']
         for tech in snapshot['technology']:
             t={}
             a={}
             for key in self._measures: 
-                url = f'{domain_id}/applications/3/results?quality-indicators={key}&technologies={tech}'
+#                url = f'{domain_id}/applications/3/results?quality-indicators={key}&technologies={tech}'
+                url = f'{domain_id}/applications/3/snapshots/{snapshot_id}/results?quality-indicators={key}&technologies={tech}'
                 (status,json) = self.get(url)
                 if status == codes.ok and len(json) > 0:
                     try:
                         t[self._measures[key]]=json[0]['applicationResults'][0]['technologyResults'][0]['result']['grade']
                     except IndexError:
                         self.warning(f'{domain_id} no grade available for {key} {tech} setting it to 4')
                         t[self._measures[key]]=4
```

### Comparing `com.castsoftware.uc.python.common-1.0.5/cast_common/highlight.py` & `com.castsoftware.uc.python.common-1.0.6/cast_common/highlight.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from cast_common.restAPI import RestCall
 from cast_common.logger import INFO
 from cast_common.util import format_table
 
 from requests import codes
-from pandas import ExcelWriter,DataFrame,json_normalize
-
+from pandas import ExcelWriter,DataFrame,json_normalize,concat
+from typing import List
+from json import loads
 
 class Highlight(RestCall):
 
     _data = {}
     _apps = []
     _tags = []
     _cloud = []
@@ -36,47 +37,66 @@
         self._apps.dropna(subset=['metrics'],inplace=True)
         self.info(f'Found {len(self._apps)} analyzed applications')
         if len(hl_apps) > 0:
             self._apps = self._apps[self._apps['name'].isin(hl_apps)]
         self.info(f'{len(self._apps)} applications selected')
 
         self._data = {}
-        for idx,app in self._apps.iterrows():
-            try:
-                app_name = app['name']
+        # for idx,app in self._apps.iterrows():
+        #     try:
+        #         app_name = app['name']
                 
-                self.info(f'Loading Highlight data for {app_name}')
-                self._data[app_name]= self._get_application_data(app_name)
+        #         self.info(f'Loading Highlight data for {app_name}')
+        #         self._data[app_name]= self._get_application_data(app_name)
 
 
                 # domains = app_data[app_name]['domains']
                 # metrics = app_data[app_name]['metrics'][0]
                 # green_detail = json_normalize(metrics['greenDetail'],['greenIndexDetails'],meta=['technology','greenIndexScan'])
                 # cloud_detail = metrics['cloudReadyDetail'][0]
                 # technology_detail = metrics['technologies'][0]
                 # vulnerability_detail = metrics['vulnerabilities'][0]
                 # components_detail = metrics['components'][0]
 
                 # app_data[app]={'domains':domains}
 
-                pass
-            except KeyError as ke:
-                pass
-        pass
+        #         pass
+        #     except KeyError as ke:
+        #         pass
+        #     except Exception as ex:
+        #         self.error(str(ex))
+        # pass
 
 
         # file_name = r'e:/work/wellsfargo/tags.xlsx'
         # writer = ExcelWriter(file_name, engine='xlsxwriter')
         # summary_tab = format_table(writer,DataFrame(self._tags),'Tags')
         # writer.close()
 
         pass
 
+    def _get_all_application_data(self):
+        self.info('Retrieving all HL application specific data')
+        self._data = {}
+        for idx,app in self._apps.iterrows():
+            try:
+                app_name = app['name']
+                self.info(f'Loading Highlight data for {app_name}')
+                self._data[app_name]= self._get_application_data(app_name)
+            except KeyError as ke:
+                self.warning(str(ke))
+                pass
+            except Exception as ex:
+                self.error(str(ex))
+        pass
+
     def _get_metrics(self,app_name):
         try:
+            if len(self._data)==0:
+                self._get_all_application_data()
             data = self._data[app_name]
             metrics = data['metrics'][0]
             return metrics
         except KeyError as ke:
             self.error(f'{app_name} has no Metric Data')
             raise ke
 
@@ -133,15 +153,15 @@
             int: highlight tag id
         """
         if len(self._tags)==0:
             self._tags = self._get_tags()
 
         series = self._tags[self._tags['label']==tag_name]
         if series.empty:
-            raise KeyError (f'Highlight application not found: {tag_name}')
+            raise KeyError (f'Highlight tag not found: {tag_name}')
         else:
             return int(series.iloc[0]['id'])
             
     def add_tag(self,app_name,tag_name) -> bool:
         """Add tag for application 
 
         Args:
@@ -155,14 +175,45 @@
 
         url = f'domains/{self._hl_instance}/applications/{app_id}/tags/{tag_id}'
         (status,json) = self.post(url)
         if status == codes.ok or status == codes.no_content:
             return True
         else:
             return False 
+    
+    def get_tech_debt_advisor(self,order:List[str],tag:str=None) -> DataFrame:
+        #https://rpa.casthighlight.com/WS2/domains/1271/technicalDebt/aggregated?tagIds=685&activePagination=false&pageOffset=0&maxEntryPerPage=9999&maxPage=999&order=healthFactor&order=alert
+        tag_part = ""
+        if tag is not None:
+            tag_part = f'tagIds={self.get_tag_id(tag)}&'
+        url = f'domains/{self._hl_instance}/technicalDebt/aggregated?{tag_part}&activePagination=false&pageOffset=0&maxEntryPerPage=9999&maxPage=999'
+        for o in order:
+            url=f'{url}&order={o}'
+        
+        (status, json) = self.get(url)
+        if status == codes.ok:
+            d1 = json_normalize(json,['subLevel'], max_level=1)
+            d1.rename(columns={'id':'Health Factor'},inplace=True)
+            d1.drop(columns=['levelType'], inplace=True)
+
+            d2=d1.explode('subLevel')
+            d2=json_normalize(d2.to_dict('records'), max_level=1)
+            d2=d2.rename(columns={'subLevel.id':'Alert','subLevel.detail':'detail'})
+            d2=d2.drop(columns=['subLevel.levelType'])
+
+            d3=json_normalize(d2.to_dict('records'),['detail'],meta=['Health Factor','Alert'])
+            d3=d3.rename(columns={'application_id':'App Id','effort':'Effort'})
+            d3=d3.drop(columns=['counter'])
+
+            return d3
+
+        else:
+            raise KeyError (f'Server returned a {status} while accessing {url}')
+
+
 
     def get_cloud_detail(self,app_name:str)->DataFrame:
         """Highlight cloud ready data
 
         Args:
             app_name (str): name of the application
 
@@ -210,9 +261,32 @@
 
 
 
 # hl = Highlight('n.kaplan+MerckMSD@castsoftware.com','vadKpBFAZ8KIKb2f2y',4711,hl_base_url='https://cloud.casthighlight.com/')
 # green_data = hl.get_green_details('TPS-2')
 # pass
 
-# hl.add_tag('1AXM:axmweb-sqlcode','EFT')
+
+# hl = Highlight('n.kaplan+WellsFargo@castsoftware.com','mdSi20ty@02',1271,hl_base_url='https://rpa.casthighlight.com/')
+
+# df = hl.get_tech_debt_advisor(['healthFactor','alert'],tag='Hamilton, Cliona')
+# df['Effort']=df['Effort']/60/8
+# df=df.rename(columns={'application_name':'Component'})
+# #df['Technology']=''
+# df['Technology']=df['Alert'].str.split('__').str[0]
+# df['Rule']=df['Alert'].str.split('__').str[1]
+# df['Rule']=df['Rule'].str.replace('_','').str.replace(r"(\w)([A-Z])", r"\1 \2",regex=True)
+
+# df['Application']=df['Component'].str.split(':').str[0]
+# df['Component']=df['Component'].str.split(':').str[-1]
+
+# df.drop(columns=['Alert'],inplace=True)
+# df = df[['Health Factor','Application','Component','Effort','Technology','Rule']]
+
+# from os.path import abspath
+
+# apps_df = df['Application'].drop_duplicates().to_frame()
+# file_name = abspath(f'E:/work/WellsFargo/tech-debt-HamiltonCliona.xlsx')
+# writer = ExcelWriter(file_name, engine='xlsxwriter')
+# app_tab = format_table(writer,apps_df,'applications')
+# writer.close
```

### Comparing `com.castsoftware.uc.python.common-1.0.5/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.0.6/cast_common/hlRestCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.5/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.0.6/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.5/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-1.0.6/cast_common/restAPI.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.5/cast_common/util.py` & `com.castsoftware.uc.python.common-1.0.6/cast_common/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         ret.append(line)
     stdout, stderr = process.communicate()
     return process.returncode,ret
     
 
 def format_table(writer, data, sheet_name,width=None):
     
-    data.to_excel(writer, index=False, sheet_name=sheet_name, startrow=1,header=False)
+    data.to_excel(writer, index=False, sheet_name=sheet_name, startrow=1,header=False,float_format = "%0.2f")
 
     workbook = writer.book
     worksheet = writer.sheets[sheet_name]
     rows = len(data)
     cols = len(data.columns)-1
     columns=[]
     for col_num, value in enumerate(data.columns.values):
```

### Comparing `com.castsoftware.uc.python.common-1.0.5/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.5
+Version: 1.0.6
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.5/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.0.5' #prod version
+version='1.0.6' #prod version
 
 dependencies = ['pandas','requests','XlsxWriter']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

