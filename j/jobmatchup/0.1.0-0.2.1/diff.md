# Comparing `tmp/jobmatchup-0.1.0.tar.gz` & `tmp/jobmatchup-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobmatchup-0.1.0.tar", max compression
+gzip compressed data, was "jobmatchup-0.2.1.tar", max compression
```

## Comparing `jobmatchup-0.1.0.tar` & `jobmatchup-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1063 2023-05-24 23:26:16.257962 jobmatchup-0.1.0/LICENSE
--rw-r--r--   0        0        0      420 2023-05-29 18:53:23.244415 jobmatchup-0.1.0/README.md
--rw-r--r--   0        0        0       49 2023-05-29 13:13:58.937195 jobmatchup-0.1.0/jobmatchup/__init__.py
--rw-r--r--   0        0        0       21 2023-05-27 22:39:41.000000 jobmatchup-0.1.0/jobmatchup/api/__init__.py
--rw-r--r--   0        0        0     3387 2023-05-29 13:43:27.829493 jobmatchup-0.1.0/jobmatchup/api/hh_api.py
--rw-r--r--   0        0        0     2341 2023-05-29 13:13:58.980195 jobmatchup-0.1.0/jobmatchup/api/query.py
--rw-r--r--   0        0        0     3980 2023-05-29 13:13:58.967195 jobmatchup-0.1.0/jobmatchup/api/superjob_api.py
--rw-r--r--   0        0        0      321 2023-05-29 13:13:58.941195 jobmatchup-0.1.0/jobmatchup/api/vacancy_service.py
--rw-r--r--   0        0        0       46 2023-05-27 22:39:41.000000 jobmatchup-0.1.0/jobmatchup/configs/__init__.py
--rw-r--r--   0        0        0     2998 2023-05-29 19:57:14.122835 jobmatchup-0.1.0/jobmatchup/configs/app_cfg.py
--rw-r--r--   0        0        0      443 2023-05-29 19:57:14.131836 jobmatchup-0.1.0/jobmatchup/configs/storage.py
--rw-r--r--   0        0        0       41 2023-05-27 22:39:41.000000 jobmatchup-0.1.0/jobmatchup/entity/__init__.py
--rw-r--r--   0        0        0     1038 2023-05-29 13:13:58.959195 jobmatchup-0.1.0/jobmatchup/entity/api.py
--rw-r--r--   0        0        0      108 2023-05-29 13:13:58.942196 jobmatchup-0.1.0/jobmatchup/entity/db.py
--rw-r--r--   0        0        0     2387 2023-05-29 13:13:58.963195 jobmatchup-0.1.0/jobmatchup/entity/hh.py
--rw-r--r--   0        0        0     2864 2023-05-29 13:49:13.911856 jobmatchup-0.1.0/jobmatchup/entity/super_job.py
--rw-r--r--   0        0        0     2886 2023-05-29 13:22:04.458285 jobmatchup-0.1.0/jobmatchup/entity/vacancy.py
--rw-r--r--   0        0        0       18 2023-05-27 22:39:41.000000 jobmatchup-0.1.0/jobmatchup/storage/__init__.py
--rw-r--r--   0        0        0     1043 2023-05-29 13:13:58.957195 jobmatchup-0.1.0/jobmatchup/storage/db.py
--rw-r--r--   0        0        0     1481 2023-05-29 13:13:58.964195 jobmatchup-0.1.0/jobmatchup/storage/file_db.py
--rw-r--r--   0        0        0       20 2023-05-28 14:30:42.557907 jobmatchup-0.1.0/jobmatchup/tools/__init__.py
--rw-r--r--   0        0        0      900 2023-05-29 13:13:58.952195 jobmatchup-0.1.0/jobmatchup/tools/filter_vacancy.py
--rw-r--r--   0        0        0      864 2023-05-29 13:13:58.957195 jobmatchup-0.1.0/jobmatchup/tools/show.py
--rw-r--r--   0        0        0      620 2023-05-29 13:13:58.947195 jobmatchup-0.1.0/jobmatchup/tools/sort_vacancy.py
--rw-r--r--   0        0        0      621 2023-05-29 20:06:46.152886 jobmatchup-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 jobmatchup-0.1.0/setup.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 jobmatchup-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-24 23:26:16.257962 jobmatchup-0.2.1/LICENSE
+-rw-r--r--   0        0        0      463 2023-05-29 20:23:04.753892 jobmatchup-0.2.1/README.md
+-rw-r--r--   0        0        0       49 2023-05-29 13:13:58.937195 jobmatchup-0.2.1/jobmatchup/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-27 22:39:41.000000 jobmatchup-0.2.1/jobmatchup/api/__init__.py
+-rw-r--r--   0        0        0     3415 2023-05-31 23:27:05.799597 jobmatchup-0.2.1/jobmatchup/api/hh_api.py
+-rw-r--r--   0        0        0     2341 2023-05-29 13:13:58.980195 jobmatchup-0.2.1/jobmatchup/api/query.py
+-rw-r--r--   0        0        0     3980 2023-05-29 13:13:58.967195 jobmatchup-0.2.1/jobmatchup/api/superjob_api.py
+-rw-r--r--   0        0        0      321 2023-05-29 13:13:58.941195 jobmatchup-0.2.1/jobmatchup/api/vacancy_service.py
+-rw-r--r--   0        0        0       46 2023-05-27 22:39:41.000000 jobmatchup-0.2.1/jobmatchup/configs/__init__.py
+-rw-r--r--   0        0        0     3019 2023-05-31 23:16:56.281492 jobmatchup-0.2.1/jobmatchup/configs/app_cfg.py
+-rw-r--r--   0        0        0      443 2023-05-29 19:57:14.131836 jobmatchup-0.2.1/jobmatchup/configs/storage.py
+-rw-r--r--   0        0        0       41 2023-05-27 22:39:41.000000 jobmatchup-0.2.1/jobmatchup/entity/__init__.py
+-rw-r--r--   0        0        0     1038 2023-05-29 13:13:58.959195 jobmatchup-0.2.1/jobmatchup/entity/api.py
+-rw-r--r--   0        0        0      108 2023-05-29 13:13:58.942196 jobmatchup-0.2.1/jobmatchup/entity/db.py
+-rw-r--r--   0        0        0     2401 2023-05-31 23:27:05.795597 jobmatchup-0.2.1/jobmatchup/entity/hh.py
+-rw-r--r--   0        0        0     3051 2023-05-31 23:27:05.797597 jobmatchup-0.2.1/jobmatchup/entity/super_job.py
+-rw-r--r--   0        0        0     3209 2023-05-31 23:14:13.982061 jobmatchup-0.2.1/jobmatchup/entity/vacancy.py
+-rw-r--r--   0        0        0       18 2023-05-27 22:39:41.000000 jobmatchup-0.2.1/jobmatchup/storage/__init__.py
+-rw-r--r--   0        0        0     1043 2023-05-29 13:13:58.957195 jobmatchup-0.2.1/jobmatchup/storage/db.py
+-rw-r--r--   0        0        0     1507 2023-05-31 23:19:29.305012 jobmatchup-0.2.1/jobmatchup/storage/file_db.py
+-rw-r--r--   0        0        0       78 2023-06-01 13:43:24.022934 jobmatchup-0.2.1/jobmatchup/tools/__init__.py
+-rw-r--r--   0        0        0      900 2023-05-29 13:13:58.952195 jobmatchup-0.2.1/jobmatchup/tools/filter_vacancy.py
+-rw-r--r--   0        0        0      864 2023-05-29 13:13:58.957195 jobmatchup-0.2.1/jobmatchup/tools/show.py
+-rw-r--r--   0        0        0      620 2023-05-29 13:13:58.947195 jobmatchup-0.2.1/jobmatchup/tools/sort_vacancy.py
+-rw-r--r--   0        0        0      640 2023-06-01 00:25:22.196064 jobmatchup-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 jobmatchup-0.2.1/setup.py
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 jobmatchup-0.2.1/PKG-INFO
```

### Comparing `jobmatchup-0.1.0/LICENSE` & `jobmatchup-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/jobmatchup/api/hh_api.py` & `jobmatchup-0.2.1/jobmatchup/api/hh_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,19 +35,19 @@
                 url=item.alternate_url,
                 date_published_timestamp=self._date_to_timestamp(item.published_at),
                 city="не указан"
                 if not item.address or not item.address.city
                 else item.address.city,
                 requirements=self._requirements_formatter(item),
                 salary_min=0
-                if not item.salary or not item.salary.minimal
-                else item.salary.minimal,
+                if not item.salary or not item.salary.salary_minimal
+                else item.salary.salary_minimal,
                 salary_max=0
-                if not item.salary or not item.salary.maximum
-                else item.salary.maximum,
+                if not item.salary or not item.salary.salary_maximum
+                else item.salary.salary_maximum,
                 currency="RUB"
                 if not item.salary
                 else self._currency_mapping(item.salary.currency),
             )
             for item in vacancies_items
         ]
```

### Comparing `jobmatchup-0.1.0/jobmatchup/api/query.py` & `jobmatchup-0.2.1/jobmatchup/api/query.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/jobmatchup/api/superjob_api.py` & `jobmatchup-0.2.1/jobmatchup/api/superjob_api.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/jobmatchup/configs/app_cfg.py` & `jobmatchup-0.2.1/jobmatchup/configs/app_cfg.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,29 +47,29 @@
                 else:
                     self._set_new_token()
             except ValidationError:
                 logging.fatal("! ENV's not found !")
 
     def _load_token(self):
         self.token_info = TokenInfo(
-            token=getenv("TOKEN"),
-            refresh_token=getenv("REFRESH_TOKEN"),
-            expires_in=getenv("EXPIRES_IN"),
+            token=getenv("SJ_TOKEN"),
+            refresh_token=getenv("SJ_REFRESH_TOKEN"),
+            expires_in=getenv("SJ_EXPIRES_IN"),
         )
 
     def _load_app_info(self):
         self.app_info = AppInfo(
-            app_id=getenv("APP_ID"),
-            secret_key=getenv("SECRET_KEY"),
+            app_id=getenv("SJ_APP_ID"),
+            secret_key=getenv("SJ_SECRET_KEY"),
         )
 
     def _load_auth_info(self) -> None:
         self.auth_info = AuthInfo(
-            login=getenv("LOGIN"),
-            password=getenv("PASSWORD"),
+            login=getenv("SJ_LOGIN"),
+            password=getenv("SJ_PASSWORD"),
         )
 
     def _load_cfg_from_toml(self) -> dict[str, Any]:
         from tomllib import load as load_toml
 
         # Read .toml file
         with open(self.cfg_file_path, "rb") as f:
```

### Comparing `jobmatchup-0.1.0/jobmatchup/entity/api.py` & `jobmatchup-0.2.1/jobmatchup/entity/api.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/jobmatchup/entity/hh.py` & `jobmatchup-0.2.1/jobmatchup/entity/hh.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     name: str
 
 
 class HeadHunterVacancySalary(BaseModel):
     currency: Literal[
         "UZS", "USD", "UAH", "RUR", "KZT", "KGS", "GEL", "EUR", "BYR", "AZN"
     ]
-    minimal: Optional[NonNegativeInt] = Field(alias="from")
+    salary_minimal: Optional[NonNegativeInt] = Field(alias="from")
     gross: bool
-    maximum: Optional[NonNegativeInt] = Field(alias="to")
+    salary_maximum: Optional[NonNegativeInt] = Field(alias="to")
 
 
 class HeadHunterVacancySnippet(BaseModel):
     requirement: str | None
     responsibility: str | None
```

### Comparing `jobmatchup-0.1.0/jobmatchup/entity/super_job.py` & `jobmatchup-0.2.1/jobmatchup/entity/super_job.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     positions: list[ObjectsCataloguesPositions]
     title: str
 
 
 class ObjectsTown(BaseModel):
     declension: str
     genitive: str
-    hasMetro: bool
+    has_metro: bool = Field(alias="hasMetro")
     id: PositiveInt
     title: str
 
 
 class ObjectsPhones(BaseModel):
-    additionalNumber: str | None
+    additional_number: str | None = Field(alias="additionalNumber")
     number: str | None
 
 
 class ObjectsClient(BaseModel):
     address: str | None
     addresses: list | None
     client_logo: AnyUrl | None
@@ -59,15 +59,15 @@
     address: str | None
     age_from: NonNegativeInt
     age_to: NonNegativeInt
     agency: FieldsIDTitle
     agreement: bool
     already_sent_on_vacancy: bool
     anonymous: bool
-    canEdit: bool
+    can_edit: bool = Field(alias="canEdit")
     candidat: str
     catalogues: list[ObjectsCatalogues]
     children: FieldsIDTitle
     client: ObjectsClient
     client_logo: AnyUrl | None
     compensation: None
     contact: str | None
@@ -85,36 +85,36 @@
     faxes: None
     firm_activity: str | None
     firm_name: str
     gender: FieldsIDTitle
     highlight: bool
     id: PositiveInt
     id_client: NonNegativeInt
-    isBlacklisted: bool
+    is_blacklisted: bool = Field(alias="isBlacklisted")
     is_archive: bool
     is_closed: bool
     is_storage: bool
     languages: list
     latitude: float | None
     link: AnyUrl
     longitude: float | None
-    maritalstatus: FieldsIDTitle
+    marital_status: FieldsIDTitle = Field(alias="maritalstatus")
     metro: list
     moveable: bool
     salary_minimal: NonNegativeInt = Field(alias="payment_from")
     salary_maximum: NonNegativeInt = Field(alias="payment_to")
     phone: str | None
     phones: list[ObjectsPhones] | None
     place_of_work: FieldsIDTitle
     profession: str
     rejected: bool
     response_info: list
     town: ObjectsTown
     type_of_work: FieldsIDTitle
-    vacancyRichText: str
+    vacancy_rich_text: str = Field(alias="vacancyRichText")
     work: None
 
 
 class SuperJobAPIVacancies(BaseModel):
     more: bool
     objects: list[SuperJobAPIVacanciesObject]
     subscription_active: bool
```

### Comparing `jobmatchup-0.1.0/jobmatchup/entity/vacancy.py` & `jobmatchup-0.2.1/jobmatchup/entity/vacancy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import logging
 from datetime import datetime, timezone, date
 from json import loads as json_loads
 from typing import Any, LiteralString
 from urllib import request, error
 
+from orjson import dumps, loads
 from pydantic import BaseModel, AnyHttpUrl, PositiveInt, NonNegativeInt, Field
 
 __all__ = ["VacancyDefault"]
 
 
+def orjson_dumps(v, *, default):
+    # orjson.dumps returns bytes, to match standard json.dumps we need to decode
+    return dumps(v, default=default).decode()
+
+
 class VacancyDefault(BaseModel):
     """
     Class Vacancy
     """
 
     title: str | None
     url: AnyHttpUrl | None
@@ -20,14 +26,22 @@
     city: str | None
     requirements: str | None
     salary_min: NonNegativeInt = Field(default=0)
     salary_max: NonNegativeInt = Field(default=0)
     currency: str = "RUB"
     _default_currency: str = "RUB"
 
+    class Config:
+        """
+        Fast serialize.
+        """
+
+        json_loads = loads
+        json_dumps = orjson_dumps
+
     @property
     def default_currency(self):
         return self._default_currency
 
     @default_currency.setter
     def default_currency(self, currency: LiteralString):
         self._default_currency = currency
```

### Comparing `jobmatchup-0.1.0/jobmatchup/storage/db.py` & `jobmatchup-0.2.1/jobmatchup/storage/db.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/jobmatchup/storage/file_db.py` & `jobmatchup-0.2.1/jobmatchup/storage/file_db.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,17 @@
         Save vacancy in DB.
         :param vacancy: Vacancy object
         """
         with open(self.file_path, "a+") as f:
             try:
                 data = load(f)
             except JSONDecodeError:
-                dump([vacancy.json()], f)
+                dump([vacancy.json(by_alias=True)], f)
             else:
-                data.append(vacancy.json())
+                data.append(vacancy.json(by_alias=True))
                 dump(data, f)
 
     def get_vacancies_by_salary(self, salary_min: int) -> list:
         """
         Select vacancies by salary.
         :param salary_min: salary
         :return: vacancies objects
```

### Comparing `jobmatchup-0.1.0/jobmatchup/tools/filter_vacancy.py` & `jobmatchup-0.2.1/jobmatchup/tools/filter_vacancy.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/jobmatchup/tools/show.py` & `jobmatchup-0.2.1/jobmatchup/tools/show.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/jobmatchup/tools/sort_vacancy.py` & `jobmatchup-0.2.1/jobmatchup/tools/sort_vacancy.py`

 * *Files identical despite different names*

### Comparing `jobmatchup-0.1.0/pyproject.toml` & `jobmatchup-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "jobmatchup"
-version = "0.1.0"
+version = "0.2.1"
 description = "Personal Vacancies Parse"
 authors = ["bbt-t <zlukcss@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/bbt-t/jobmatchup"
 repository = "https://github.com/bbt-t/jobmatchup"
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.8"
 python-dateutil = "^2.8.2"
+orjson = "^3.8.14"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 flake8 = "^6.0.0"
 black = "^23.3.0"
 pep8-naming = "^0.13.3"
```

### Comparing `jobmatchup-0.1.0/setup.py` & `jobmatchup-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,23 @@
  'jobmatchup.storage',
  'jobmatchup.tools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pydantic>=1.10.8,<2.0.0', 'python-dateutil>=2.8.2,<3.0.0']
+['orjson>=3.8.14,<4.0.0',
+ 'pydantic>=1.10.8,<2.0.0',
+ 'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'jobmatchup',
-    'version': '0.1.0',
+    'version': '0.2.1',
     'description': 'Personal Vacancies Parse',
-    'long_description': '<p align="center">\n  <img alt="" src="https://i.ibb.co/6XWd58N/python-applications-removebg.png" width="500px">\n</p>\t\n\n***\n### about\n\n> Personal vacancies Parser\n\n<details>\n <summary>What sites can you parse from?</summary>\n<ul>\n  <li>hh.ru :heavy_check_mark:</li>\n  <li>superjob.ru :heavy_check_mark:</li>\n</ul>\n</details>\n\n***\n\n### usage\n\n`see examples` [> Examples <](https://github.com/bbt-t/pvp/tree/main/examples)\n',
+    'long_description': '<p align="center">\n  <img alt="" src="https://i.ibb.co/6XWd58N/python-applications-removebg.png" width="500px">\n</p>\t\n\n***\n### about\n\n> Personal vacancies Parser\n\n<details>\n <summary>What sites can you parse from?</summary>\n<ul>\n  <li>hh.ru :heavy_check_mark:</li>\n  <li>superjob.ru :heavy_check_mark:</li>\n</ul>\n</details>\n\n***\n\n## install\n\n`pip install jobmatchup`\n\n***\n\n### usage\n\n`see examples` [> Examples <](https://github.com/bbt-t/pvp/tree/main/examples)\n',
     'author': 'bbt-t',
     'author_email': 'zlukcss@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bbt-t/jobmatchup',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `jobmatchup-0.1.0/PKG-INFO` & `jobmatchup-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: jobmatchup
-Version: 0.1.0
+Version: 0.2.1
 Summary: Personal Vacancies Parse
 Home-page: https://github.com/bbt-t/jobmatchup
 License: MIT
 Author: bbt-t
 Author-email: zlukcss@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: orjson (>=3.8.14,<4.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/bbt-t/jobmatchup
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img alt="" src="https://i.ibb.co/6XWd58N/python-applications-removebg.png" width="500px">
@@ -30,11 +31,17 @@
   <li>hh.ru :heavy_check_mark:</li>
   <li>superjob.ru :heavy_check_mark:</li>
 </ul>
 </details>
 
 ***
 
+## install
+
+`pip install jobmatchup`
+
+***
+
 ### usage
 
 `see examples` [> Examples <](https://github.com/bbt-t/pvp/tree/main/examples)
```

