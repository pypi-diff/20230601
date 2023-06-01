# Comparing `tmp/logiclayer_complexity-0.2.0.tar.gz` & `tmp/logiclayer_complexity-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logiclayer_complexity-0.2.0.tar", max compression
+gzip compressed data, was "logiclayer_complexity-0.2.1.tar", max compression
```

## Comparing `logiclayer_complexity-0.2.0.tar` & `logiclayer_complexity-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1093 2022-08-10 00:34:08.071136 logiclayer_complexity-0.2.0/LICENSE
--rw-r--r--   0        0        0      225 2023-03-24 16:22:43.492174 logiclayer_complexity-0.2.0/logiclayer_complexity/__init__.py
--rw-r--r--   0        0        0      201 2023-03-30 19:44:18.693799 logiclayer_complexity-0.2.0/logiclayer_complexity/__version__.py
--rw-r--r--   0        0        0     2893 2023-03-24 16:29:25.668819 logiclayer_complexity-0.2.0/logiclayer_complexity/complexity.py
--rw-r--r--   0        0        0     6662 2023-03-24 16:19:10.751757 logiclayer_complexity-0.2.0/logiclayer_complexity/dependencies.py
--rw-r--r--   0        0        0     5523 2023-03-24 18:34:31.243084 logiclayer_complexity-0.2.0/logiclayer_complexity/module.py
--rw-r--r--   0        0        0     4162 2022-10-27 18:32:32.255267 logiclayer_complexity-0.2.0/logiclayer_complexity/rca.py
--rw-r--r--   0        0        0     2372 2023-03-30 19:51:42.438109 logiclayer_complexity-0.2.0/logiclayer_complexity/wdi.py
--rw-r--r--   0        0        0     1658 2022-08-10 00:46:00.273578 logiclayer_complexity-0.2.0/PACKAGE.md
--rw-r--r--   0        0        0      813 2023-03-30 19:43:21.749830 logiclayer_complexity-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 logiclayer_complexity-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2022-08-10 00:34:08.071136 logiclayer_complexity-0.2.1/LICENSE
+-rw-r--r--   0        0        0      225 2023-03-24 16:22:43.492174 logiclayer_complexity-0.2.1/logiclayer_complexity/__init__.py
+-rw-r--r--   0        0        0      201 2023-06-01 20:37:25.601431 logiclayer_complexity-0.2.1/logiclayer_complexity/__version__.py
+-rw-r--r--   0        0        0     2893 2023-03-24 16:29:25.668819 logiclayer_complexity-0.2.1/logiclayer_complexity/complexity.py
+-rw-r--r--   0        0        0     9173 2023-06-01 20:37:25.602408 logiclayer_complexity-0.2.1/logiclayer_complexity/dependencies.py
+-rw-r--r--   0        0        0     7074 2023-06-01 20:37:25.604401 logiclayer_complexity-0.2.1/logiclayer_complexity/module.py
+-rw-r--r--   0        0        0     2518 2023-06-01 20:37:25.610389 logiclayer_complexity-0.2.1/logiclayer_complexity/opportunity_gain.py
+-rw-r--r--   0        0        0     4193 2023-04-25 20:50:56.613422 logiclayer_complexity-0.2.1/logiclayer_complexity/rca.py
+-rw-r--r--   0        0        0     2921 2023-05-25 23:53:02.057525 logiclayer_complexity-0.2.1/logiclayer_complexity/relatedness.py
+-rw-r--r--   0        0        0     2313 2023-05-25 23:52:38.097041 logiclayer_complexity-0.2.1/logiclayer_complexity/wdi.py
+-rw-r--r--   0        0        0     1658 2022-08-10 00:46:00.273578 logiclayer_complexity-0.2.1/PACKAGE.md
+-rw-r--r--   0        0        0      885 2023-06-01 20:37:25.617392 logiclayer_complexity-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 logiclayer_complexity-0.2.1/PKG-INFO
```

### Comparing `logiclayer_complexity-0.2.0/LICENSE` & `logiclayer_complexity-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.2.0/logiclayer_complexity/complexity.py` & `logiclayer_complexity-0.2.1/logiclayer_complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.2.0/logiclayer_complexity/module.py` & `logiclayer_complexity-0.2.1/logiclayer_complexity/module.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 from logiclayer import LogicLayerModule, route
 from tesseract_olap import DataRequest, OlapServer
 from tesseract_olap.backend.exceptions import BackendError
 from tesseract_olap.query.exceptions import QueryError
 
 from .__version__ import __title__, __version__
 from .complexity import ComplexityParameters
-from .dependencies import parse_filter, prepare_complexity_params, prepare_rca_params
+from .dependencies import parse_filter, prepare_complexity_params, prepare_rca_params, prepare_relatedness_params, prepare_opportunity_gain_params
 from .rca import RcaParameters
 from .wdi import WdiParameters, WdiReference, WdiReferenceSchema, parse_wdi
+from .relatedness import RelatednessParameters
+from .opportunity_gain import OpportunityGainParameters
 
 
 class EconomicComplexityModule(LogicLayerModule):
     """Economic Complexity calculations module class for LogicLayer."""
 
     server: "OlapServer"
     wdi: Optional["WdiReference"]
@@ -34,18 +36,18 @@
         """Setups the server for this instance."""
         super().__init__()
 
         if server is None:
             raise ValueError(
                 "EconomicComplexityModule requires a tesseract_olap.OlapServer instance"
             )
+
         self.server = server
+        self.wdi = None if wdi is None else WdiReference(**wdi)
 
-        if wdi is not None:
-            self.wdi = WdiReference(**wdi)
 
     async def fetch_data(self, query: DataRequest):
         """Retrieves the data from the backend, and handles related errors."""
         try:
             res = await self.server.execute(query)
         except QueryError as exc:
             raise HTTPException(status_code=400, detail=exc.message) from None
@@ -147,14 +149,54 @@
         apply_filters(pci, filters)
         apply_aliases(pci, cmplx.aliases)
 
         return {
             "data": pci.to_dict("records"),
         }
 
+    @route("GET", "/relatedness")
+    async def route_relatedness(
+        self,
+        relatedness: RelatednessParameters = Depends(prepare_relatedness_params),
+        filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
+    ):
+        """Relatedness calculation endpoint."""
+        df = await self.fetch_data(relatedness.query)
+
+        relatedness.apply_threshold(df)
+
+        relatedness_df = relatedness.calculate(df, unpivot=True)
+
+        apply_filters(relatedness_df, filters)
+        apply_aliases(relatedness_df, relatedness.aliases)
+
+        return {
+            "data": relatedness_df.to_dict("records"),
+        }
+    
+    @route("GET", "/opportunity_gain")
+    async def route_opportunity_gain(
+        self,
+        opportunity_gain: OpportunityGainParameters = Depends(prepare_opportunity_gain_params),
+        filters: Dict[str, Tuple[str, ...]] = Depends(parse_filter),
+    ):
+        """Opportunity Gain calculation endpoint."""
+        df = await self.fetch_data(opportunity_gain.query)
+
+        opportunity_gain.apply_threshold(df)
+
+        opportunity_gain_df = opportunity_gain.calculate(df, unpivot=True)
+
+        apply_filters(opportunity_gain_df, filters)
+        apply_aliases(opportunity_gain_df, opportunity_gain.aliases)
+
+        return {
+            "data": opportunity_gain_df.to_dict("records"),
+        }
+
 
 def apply_filters(df: pd.DataFrame, filters: Dict[str, Tuple[str, ...]]):
     # filter which members will be sent in the response
     for key, values in filters.items():
         column_id = f"{key} ID"
         dropping = df.loc[~df[column_id].isin(values)].index
         df.drop(dropping, inplace=True)
```

### Comparing `logiclayer_complexity-0.2.0/logiclayer_complexity/rca.py` & `logiclayer_complexity-0.2.1/logiclayer_complexity/rca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from dataclasses import dataclass
-from typing import Dict, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import economic_complexity
 import pandas as pd
 from tesseract_olap import DataRequest, DataRequestParams
 
 
 @dataclass
 class RcaParameters:
     cube: str
     activity: str
     location: str
     measure: str
-    year: int
+    years: List[int]
     locale: Optional[str]
     threshold: Dict[str, Tuple[str, int]]
     aliases: Dict[str, str]
 
     @property
     def query(self) -> DataRequest:
         params: DataRequestParams = {
             "drilldowns": [self.location, self.activity],
             "measures": [self.measure],
             "cuts_include": {
-                "Year": [str(self.year)],
+                "Year": [str(year) for year in self.years],
             },
         }
 
         if self.locale is not None:
             params["locale"] = self.locale
 
         return DataRequest.new(self.cube, params)
```

### Comparing `logiclayer_complexity-0.2.0/logiclayer_complexity/wdi.py` & `logiclayer_complexity-0.2.1/logiclayer_complexity/wdi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from dataclasses import dataclass, field
 from typing import Dict, List
-from typing_extensions import TypedDict
+from typing_extensions import TypedDict, Required
 
 from fastapi import HTTPException, Query
 from tesseract_olap import DataRequest
 
 
 @dataclass
 class WdiParameters:
     indicator: str
     year: List[int]
     comparison: str
     value: int
 
 
-class RequiredWdiReferenceSchema(TypedDict, total=True):
-    cube: str
-
-
-class WdiReferenceSchema(RequiredWdiReferenceSchema, total=False):
+class WdiReferenceSchema(TypedDict, total=False):
+    cube: Required[str]
     measure: str
     level_mapper: Dict[str, str]
 
 
 @dataclass
 class WdiReference:
     cube: str
```

### Comparing `logiclayer_complexity-0.2.0/PACKAGE.md` & `logiclayer_complexity-0.2.1/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `logiclayer_complexity-0.2.0/pyproject.toml` & `logiclayer_complexity-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [tool.poetry]
 name = "logiclayer-complexity"
-version = "0.2.0"
+version = "0.2.1"
 description = "LogicLayer module to enable Economic Complexity calculations, using data from a tesseract-olap server."
 authors = [
   "Francisco Abarzua <francisco@datawheel.us>",
+  "Jelmy Hermosilla <jelmy@datawheel.us>",
   "Miguel Castillo <miguel@datawheel.us>",
 ]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/logiclayer-complexity"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 economic-complexity = "^0.1.0"
 logiclayer = "^0.2.0"
-tesseract-olap = "^0.6.0"
+tesseract-olap = ">=0.7.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 ipykernel = "^6.0.0"
 pytest = "^7.2.0"
 pytest-asyncio = "^0.20.0"
 ruff = "^0.0.259"
-tesseract-olap = {version = "^0.6.0", extras = ["clickhouse"]}
+tesseract-olap = {version = "^0.7.0", extras = ["clickhouse"]}
+uvicorn = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `logiclayer_complexity-0.2.0/PKG-INFO` & `logiclayer_complexity-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logiclayer-complexity
-Version: 0.2.0
+Version: 0.2.1
 Summary: LogicLayer module to enable Economic Complexity calculations, using data from a tesseract-olap server.
 Home-page: https://github.com/Datawheel/logiclayer-complexity
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: economic-complexity (>=0.1.0,<0.2.0)
 Requires-Dist: logiclayer (>=0.2.0,<0.3.0)
-Requires-Dist: tesseract-olap (>=0.6.0,<0.7.0)
+Requires-Dist: tesseract-olap (>=0.7.0)
 Project-URL: Repository, https://github.com/Datawheel/logiclayer-complexity
 Description-Content-Type: text/markdown
 
 <p>
 <a href="https://github.com/Datawheel/logiclayer-complexity/releases"><img src="https://flat.badgen.net/github/release/Datawheel/logiclayer-complexity" /></a>
 <a href="https://github.com/Datawheel/logiclayer-complexity/blob/master/LICENSE"><img src="https://flat.badgen.net/github/license/Datawheel/logiclayer-complexity" /></a>
 <a href="https://github.com/Datawheel/logiclayer-complexity/"><img src="https://flat.badgen.net/github/checks/Datawheel/logiclayer-complexity" /></a>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: logiclayer-complexity Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: logiclayer-complexity Version: 0.2.1 Summary:
 LogicLayer module to enable Economic Complexity calculations, using data from a
 tesseract-olap server. Home-page: https://github.com/Datawheel/logiclayer-
 complexity License: MIT Author: Francisco Abarzua Author-email:
 francisco@datawheel.us Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: economic-complexity (>=0.1.0,<0.2.0)
 Requires-Dist: logiclayer (>=0.2.0,<0.3.0) Requires-Dist: tesseract-olap
-(>=0.6.0,<0.7.0) Project-URL: Repository, https://github.com/Datawheel/
-logiclayer-complexity Description-Content-Type: text/markdown
+(>=0.7.0) Project-URL: Repository, https://github.com/Datawheel/logiclayer-
+complexity Description-Content-Type: text/markdown
 [https://flat.badgen.net/github/release/Datawheel/logiclayer-complexity]
 [https://flat.badgen.net/github/license/Datawheel/logiclayer-complexity]
 [https://flat.badgen.net/github/checks/Datawheel/logiclayer-complexity] [https:
 //flat.badgen.net/github/issues/Datawheel/logiclayer-complexity]
 ## Getting started This module must be used with LogicLayer. An instance of
 `OlapServer` from the `tesseract_olap` package is also required to retrieve the
 data. ```python # app.py from logiclayer import LogicLayer from
```

