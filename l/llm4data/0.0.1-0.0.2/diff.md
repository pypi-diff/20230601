# Comparing `tmp/llm4data-0.0.1.tar.gz` & `tmp/llm4data-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm4data-0.0.1.tar", max compression
+gzip compressed data, was "llm4data-0.0.2.tar", max compression
```

## Comparing `llm4data-0.0.1.tar` & `llm4data-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,24 @@
--rw-r--r--   0        0        0    30757 2023-05-26 17:27:00.950549 llm4data-0.0.1/LICENSE
--rw-r--r--   0        0        0     7629 2023-05-27 18:08:36.101699 llm4data-0.0.1/README.md
--rw-r--r--   0        0        0      157 2023-05-27 00:48:13.353628 llm4data-0.0.1/llm4data/__init__.py
--rw-r--r--   0        0        0     1757 2023-05-27 00:15:21.953796 llm4data-0.0.1/llm4data/configs.py
--rw-r--r--   0        0        0     5550 2023-05-27 17:39:27.522862 llm4data-0.0.1/llm4data/llm/indicators/wdi_sql.py
--rw-r--r--   0        0        0        0 2023-05-26 16:41:36.283163 llm4data-0.0.1/llm4data/llm/microdata/.gitkeep
--rw-r--r--   0        0        0     1407 2023-05-27 17:11:44.934021 llm4data-0.0.1/llm4data/prompts/base.py
--rw-r--r--   0        0        0     1663 2023-05-27 17:39:37.424246 llm4data-0.0.1/llm4data/prompts/indicators/templates.py
--rw-r--r--   0        0        0     3945 2023-05-27 17:39:32.427008 llm4data-0.0.1/llm4data/prompts/indicators/wdi.py
--rw-r--r--   0        0        0        0 2023-05-26 16:40:23.801226 llm4data-0.0.1/llm4data/prompts/microdata/.gitkeep
--rw-r--r--   0        0        0      352 2023-05-26 19:58:54.433048 llm4data-0.0.1/llm4data/prompts/utils.py
--rw-r--r--   0        0        0     3146 2023-05-27 00:12:24.551761 llm4data-0.0.1/llm4data/sources/indicators/wdi.py
--rw-r--r--   0        0        0        0 2023-05-26 16:41:22.772734 llm4data-0.0.1/llm4data/sources/microdata/.gitkeep
--rw-r--r--   0        0        0   117888 2023-05-24 15:43:46.011357 llm4data-0.0.1/llm4data/wdi2name.json
--rw-r--r--   0        0        0     1136 2023-05-27 17:09:24.123424 llm4data-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8522 1970-01-01 00:00:00.000000 llm4data-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    30757 2023-05-26 17:27:00.950549 llm4data-0.0.2/LICENSE
+-rw-r--r--   0        0        0     9149 2023-06-01 02:16:59.883937 llm4data-0.0.2/README.md
+-rw-r--r--   0        0        0      289 2023-06-01 02:14:09.993471 llm4data-0.0.2/llm4data/__init__.py
+-rw-r--r--   0        0        0     3005 2023-05-31 23:34:02.046844 llm4data-0.0.2/llm4data/configs.py
+-rw-r--r--   0        0        0      243 2023-05-31 23:34:02.046957 llm4data-0.0.2/llm4data/embeddings/__init__.py
+-rw-r--r--   0        0        0     3155 2023-05-31 23:34:02.047055 llm4data-0.0.2/llm4data/embeddings/base.py
+-rw-r--r--   0        0        0      528 2023-05-31 23:34:02.047157 llm4data-0.0.2/llm4data/embeddings/docs.py
+-rw-r--r--   0        0        0      796 2023-05-31 23:34:02.047256 llm4data-0.0.2/llm4data/embeddings/indicators.py
+-rw-r--r--   0        0        0      803 2023-05-31 23:34:02.047356 llm4data-0.0.2/llm4data/embeddings/microdata.py
+-rw-r--r--   0        0        0      170 2023-05-31 23:34:02.047500 llm4data-0.0.2/llm4data/index/index.py
+-rw-r--r--   0        0        0     2356 2023-05-31 23:34:02.047613 llm4data-0.0.2/llm4data/index/qdrant.py
+-rw-r--r--   0        0        0     5550 2023-05-27 17:39:27.522862 llm4data-0.0.2/llm4data/llm/indicators/wdi_sql.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:41:36.283163 llm4data-0.0.2/llm4data/llm/microdata/.gitkeep
+-rw-r--r--   0        0        0     1407 2023-05-27 17:11:44.934021 llm4data-0.0.2/llm4data/prompts/base.py
+-rw-r--r--   0        0        0     1663 2023-05-27 17:39:37.424246 llm4data-0.0.2/llm4data/prompts/indicators/templates.py
+-rw-r--r--   0        0        0     3945 2023-05-27 17:39:32.427008 llm4data-0.0.2/llm4data/prompts/indicators/wdi.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:40:23.801226 llm4data-0.0.2/llm4data/prompts/microdata/.gitkeep
+-rw-r--r--   0        0        0      352 2023-05-26 19:58:54.433048 llm4data-0.0.2/llm4data/prompts/utils.py
+-rw-r--r--   0        0        0    11208 2023-05-30 17:15:25.960735 llm4data-0.0.2/llm4data/schema/docs/wbdocs.py
+-rw-r--r--   0        0        0     3146 2023-05-27 00:12:24.551761 llm4data-0.0.2/llm4data/sources/indicators/wdi.py
+-rw-r--r--   0        0        0        0 2023-05-26 16:41:22.772734 llm4data-0.0.2/llm4data/sources/microdata/.gitkeep
+-rw-r--r--   0        0        0   117888 2023-05-24 15:43:46.011357 llm4data-0.0.2/llm4data/wdi2name.json
+-rw-r--r--   0        0        0     1290 2023-06-01 02:14:09.985816 llm4data-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10298 1970-01-01 00:00:00.000000 llm4data-0.0.2/PKG-INFO
```

### Comparing `llm4data-0.0.1/LICENSE` & `llm4data-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.1/README.md` & `llm4data-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 # LLM4Data
 
-LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for data and knowledge discovery. It is intended to empower users and organizations to discover and interact with development data in innovative ways through natural language.
+LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery. It is intended to empower users and organizations to discover and interact with development data in innovative ways through natural language.
 
-Built around existing metadata standards and schemas, users and organizations can benefit from LLMs to enhance data-driven applications, enabling natural language processing, text generation, and more with LLM4Data. The library serves as a bridge between LLMs and development data using open-sourced libraries, offering a seamless interface to leverage the capabilities of these powerful language models.
+This library contains a collection of discovery and data augmentation solutions for various data types including documents, indicators, microdata, geospatial data, and more. The current version of the library includes solutions for the WDI indicators. Additional solutions will be added in [future releases](https://worldbank.github.io/llm4data/README.html#upcoming-features).
+
+Built around existing [metadata standards and schemas](https://mah0001.github.io/schema-guide/), users and organizations can benefit from LLMs to enhance data-driven applications, enabling natural language processing, text generation, and more with LLM4Data. The library serves as a bridge between LLMs and development data using open-sourced libraries, offering a seamless interface to leverage the capabilities of these powerful language models.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install LLM4Data.
 
 ```bash
 pip install llm4data
 ```
 
 ## Usage
 
+The following examples demonstrate how to use LLM4Data to generate WDI API URLs and SQL queries from prompts.
+
+Additional examples can be found [here](notebooks/examples/).
 
 ### Generate WDI API URL from a prompt
 
+```{warning}
+This example uses the OpenAI API. Before you proceed, make sure to set your API keys in the `.env` file. See the [setup instructions](https://worldbank.github.io/llm4data/notebooks/examples/getting-started/openai-api.html) for more details.
+```
+
+
 ```python
-from llm4data.promps.indicators import wdi
+from llm4data.prompts.indicators import wdi
 
 # Create a WDI API prompt object
 wdi_api = wdi.WDIAPIPrompt()
 
 # Send a prompt to the LLM to get a WDI API URL relevant to the prompt
 response = wdi_api.send_prompt(
     "What is the gdp and the co2 emissions of the philippines and its neighbors in the last decade?"
@@ -41,14 +51,18 @@
 
 Notice that the URL generated already includes the country codes and indicators relevant to the prompt. It understands which countries are the neighbors of the Philippines. It also understands which indicator codes are likely to provide the relevant data for GDP and CO2 emissions.
 
 The URL also includes the date range, format, and source of the data. The user can then tweak the URL as needed, and use it to query the WDI API.
 
 ### Generate SQL queries on WDI data from a prompt
 
+```{warning}
+Make sure you have set up your environment first. The example below requires a working database engine, e.g., postgresql. If you want to use SQLite, make sure to update the `.env` file and set the environment variables.
+```
+
 While the WDI data can be loaded into a Pandas dataframe, it is not always practical to do so; for example, developing applications that can answer arbitrary data questions.
 
 The LLM4Data library includes an SQL interface to WDI data, allowing users to query the data using SQL.
 
 This interface will allow users to query the data using SQL, and return the results as a Pandas dataframe. The interface also allows users to query the data using SQL, and return the results as a JSON object.
 
 ```python
@@ -116,25 +130,47 @@
 > Finished chain.
 ```
 
 Unfortunately, the answer `The GDP of the Philippines in 2020 was 1.01242392260698 and the military expenditure (% of GDP) was 361751116292.541.` is incorrect because the values have been swapped.
 
 One of the goals of LLM4Data is to develop solutions around the limitations of existing open-source solutions as applied to development data and knowledge discovery.
 
-## Key Features and Roadmap:
+## Key Features and Roadmap
 
 - Text generation: Utilize LLMs to generate coherent and contextually relevant text around development data, enabling the creation of chatbots and content generation systems.
 - Interactive experiences: Create engaging user experiences by integrating LLMs into applications, allowing users to interact with development data in a more intuitive and conversational manner.
 - Metadata augmentation: Enhance existing metadata with LLMs, enabling the creation of new metadata and the improvement of existing metadata.
 - AI-powered insights: Extract valuable insights from datasets using LLMs, empowering data exploration, trend analysis, and knowledge discovery.
 - Dynamic integration: Through the use of metadata standards and schemas, load and utilize your own Python scripts containing LLM functionality on-the-fly, seamlessly incorporating them into your project through plug-ins.
 - Natural language processing: Leverage LLMs to analyze and process textual data, enabling tasks like sentiment analysis, text classification, and language translation.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
-Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more information.
+Please see [CONTRIBUTING.md](.github/CONTRIBUTING.md) for more information.
 
 ## License
 
 LLM4Data is licensed under the [ World Bank Master Community License Agreement](LICENSE).
+
+
+## Upcoming Features
+
+- [ ] Metadata augmentation with LLM
+- [ ] Document and metadata indexing
+- [ ] Semantic search:
+  - [ ] For indicators
+  - [ ] For documents
+  - [ ] For microdata
+  - [ ] For geospatial data
+  - [ ] For voice and videos
+- [ ] Open-source chat UI
+- [ ] Data use framework
+
+
+## TODO
+
+- [ ] Add contributing guidelines
+- [ ] Add more documentations
+- [ ] Add unit tests
+- [ ] Add CI/CD
```

### Comparing `llm4data-0.0.1/llm4data/configs.py` & `llm4data-0.0.2/llm4data/configs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import os
+import warnings
 from pathlib import Path
 from typing import Union, Optional
-from dotenv import load_dotenv
 from dataclasses import dataclass
 
-# Load environment variables from .env file
-load_dotenv()
-
 
 # Define a data class for the database config
 @dataclass
 class WDIDBConfig:
     table_name: Optional[str] = os.getenv("WDI_DB_TABLE_NAME")
     engine: Optional[str] = os.getenv("WDI_DB_ENGINE")
     host: Optional[str] = os.getenv("WDI_DB_HOST")
@@ -32,23 +29,49 @@
             url += f":{self.port}"
 
         return url
 
 
 @dataclass
 class DirsConfig:
+    llm4data_dir: Union[str, Path] = os.getenv("LLM4DATA_DIR", "")
+    llm4data_cache_dir: Union[str, Path] = os.getenv("LLM4DATA_CACHE_DIR", "")
     openai_payload_dir: Union[str, Path] = os.getenv("OPENAI_PAYLOAD_DIR", "")
 
+    _exception_template = "`{dirvar}` environment variable is not set. Consider adding it to your .env file."
+
     def __post_init__(self):
-        if not self.openai_payload_dir:
-            raise ValueError(
-                "`OPENAI_PAYLOAD_DIR` environment variable is not set. Consider adding it to your .env file."
-            )
+        self.llm4data_dir = self._process_dir(self.llm4data_dir, "LLM4DATA_DIR")
+
+        if not isinstance(self.llm4data_cache_dir, str):
+            raise ValueError("`LLM4DATA_CACHE_DIR` environment variable must be a string.")
+
+        if not isinstance(self.openai_payload_dir, str):
+            raise ValueError("`OPENAI_PAYLOAD_DIR` environment variable must be a string.")
+
+        self.llm4data_cache_dir = self.llm4data_dir / self.llm4data_cache_dir
+        self.openai_payload_dir = self.llm4data_dir / self.openai_payload_dir
+
+        self.llm4data_cache_dir = self._process_dir(self.llm4data_cache_dir, "LLM4DATA_CACHE_DIR")
+        self.openai_payload_dir = self._process_dir(self.openai_payload_dir, "OPENAI_PAYLOAD_DIR")
+
+    def _process_dir(self, dirname: Union[str, Path], dirvar: str) -> Path:
+        if not dirname:
+            raise ValueError(self._exception_template.format(dirvar=dirvar))
+
+        dirname = Path(dirname).expanduser().resolve()
+
+        if dirvar != "LLM4DATA_DIR" and self.llm4data_dir == dirname:
+            raise ValueError(f"{dirvar}={dirname} is the same as LLM4DATA_DIR={self.llm4data_dir}")
+
+        if not dirname.exists():
+            warnings.warn(f"{dirvar}={dirname} does not exist. Creating it now...")
+            dirname.mkdir(parents=True)
 
-        self.openai_payload_dir = Path(self.openai_payload_dir)
+        return dirname
 
 
 @dataclass
 class TaskLabelsConfig:
     wdi_sql: str = os.getenv("TASK_LABEL_WDI_SQL", "")
 
     def __post_init__(self):
```

### Comparing `llm4data-0.0.1/llm4data/llm/indicators/wdi_sql.py` & `llm4data-0.0.2/llm4data/llm/indicators/wdi_sql.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.1/llm4data/prompts/base.py` & `llm4data-0.0.2/llm4data/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.1/llm4data/prompts/indicators/templates.py` & `llm4data-0.0.2/llm4data/prompts/indicators/templates.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.1/llm4data/prompts/indicators/wdi.py` & `llm4data-0.0.2/llm4data/prompts/indicators/wdi.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.1/llm4data/sources/indicators/wdi.py` & `llm4data-0.0.2/llm4data/sources/indicators/wdi.py`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.1/llm4data/wdi2name.json` & `llm4data-0.0.2/llm4data/wdi2name.json`

 * *Files identical despite different names*

### Comparing `llm4data-0.0.1/pyproject.toml` & `llm4data-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 name = "llm4data"
-version = "0.0.1"
-description = "LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for data and knowledge discovery."
+version = "0.0.2"
+description = "LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery."
 authors = ["Aivin V. Solatorio <avsolatorio@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.1"
 numpy = "^1.24.3"
 sqlalchemy = "^2.0.15"
 openai-tools = "0.0.0.1.dev3"
 tomli = "^2.0.1"
 langchain = "^0.0.178"
 psycopg2-binary = "^2.9.6"
 python-dotenv = "^1.0.0"
 tiktoken = "^0.4.0"
+fire = "^0.5.0"
+qdrant-client = {version = "^1.2.0", python = ">=3.10,<3.12"}
+sentence-transformers = "^2.2.2"
+instructorembedding = "^1.0.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-dotenv = "^0.5.2"
```

### Comparing `llm4data-0.0.1/PKG-INFO` & `llm4data-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,63 @@
 Metadata-Version: 2.1
 Name: llm4data
-Version: 0.0.1
-Summary: LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for data and knowledge discovery.
+Version: 0.0.2
+Summary: LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery.
 Author: Aivin V. Solatorio
 Author-email: avsolatorio@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: instructorembedding (>=1.0.1,<2.0.0)
 Requires-Dist: langchain (>=0.0.178,<0.0.179)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: openai-tools (==0.0.0.1.dev3)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: qdrant-client (>=1.2.0,<2.0.0) ; python_version >= "3.10" and python_version < "3.12"
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.15,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # LLM4Data
 
-LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for data and knowledge discovery. It is intended to empower users and organizations to discover and interact with development data in innovative ways through natural language.
+LLM4Data is a Python library designed to facilitate the application of large language models (LLMs) and artificial intelligence for development data and knowledge discovery. It is intended to empower users and organizations to discover and interact with development data in innovative ways through natural language.
 
-Built around existing metadata standards and schemas, users and organizations can benefit from LLMs to enhance data-driven applications, enabling natural language processing, text generation, and more with LLM4Data. The library serves as a bridge between LLMs and development data using open-sourced libraries, offering a seamless interface to leverage the capabilities of these powerful language models.
+This library contains a collection of discovery and data augmentation solutions for various data types including documents, indicators, microdata, geospatial data, and more. The current version of the library includes solutions for the WDI indicators. Additional solutions will be added in [future releases](https://worldbank.github.io/llm4data/README.html#upcoming-features).
+
+Built around existing [metadata standards and schemas](https://mah0001.github.io/schema-guide/), users and organizations can benefit from LLMs to enhance data-driven applications, enabling natural language processing, text generation, and more with LLM4Data. The library serves as a bridge between LLMs and development data using open-sourced libraries, offering a seamless interface to leverage the capabilities of these powerful language models.
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install LLM4Data.
 
 ```bash
 pip install llm4data
 ```
 
 ## Usage
 
+The following examples demonstrate how to use LLM4Data to generate WDI API URLs and SQL queries from prompts.
+
+Additional examples can be found [here](notebooks/examples/).
 
 ### Generate WDI API URL from a prompt
 
+```{warning}
+This example uses the OpenAI API. Before you proceed, make sure to set your API keys in the `.env` file. See the [setup instructions](https://worldbank.github.io/llm4data/notebooks/examples/getting-started/openai-api.html) for more details.
+```
+
+
 ```python
-from llm4data.promps.indicators import wdi
+from llm4data.prompts.indicators import wdi
 
 # Create a WDI API prompt object
 wdi_api = wdi.WDIAPIPrompt()
 
 # Send a prompt to the LLM to get a WDI API URL relevant to the prompt
 response = wdi_api.send_prompt(
     "What is the gdp and the co2 emissions of the philippines and its neighbors in the last decade?"
@@ -62,14 +76,18 @@
 
 Notice that the URL generated already includes the country codes and indicators relevant to the prompt. It understands which countries are the neighbors of the Philippines. It also understands which indicator codes are likely to provide the relevant data for GDP and CO2 emissions.
 
 The URL also includes the date range, format, and source of the data. The user can then tweak the URL as needed, and use it to query the WDI API.
 
 ### Generate SQL queries on WDI data from a prompt
 
+```{warning}
+Make sure you have set up your environment first. The example below requires a working database engine, e.g., postgresql. If you want to use SQLite, make sure to update the `.env` file and set the environment variables.
+```
+
 While the WDI data can be loaded into a Pandas dataframe, it is not always practical to do so; for example, developing applications that can answer arbitrary data questions.
 
 The LLM4Data library includes an SQL interface to WDI data, allowing users to query the data using SQL.
 
 This interface will allow users to query the data using SQL, and return the results as a Pandas dataframe. The interface also allows users to query the data using SQL, and return the results as a JSON object.
 
 ```python
@@ -137,26 +155,48 @@
 > Finished chain.
 ```
 
 Unfortunately, the answer `The GDP of the Philippines in 2020 was 1.01242392260698 and the military expenditure (% of GDP) was 361751116292.541.` is incorrect because the values have been swapped.
 
 One of the goals of LLM4Data is to develop solutions around the limitations of existing open-source solutions as applied to development data and knowledge discovery.
 
-## Key Features and Roadmap:
+## Key Features and Roadmap
 
 - Text generation: Utilize LLMs to generate coherent and contextually relevant text around development data, enabling the creation of chatbots and content generation systems.
 - Interactive experiences: Create engaging user experiences by integrating LLMs into applications, allowing users to interact with development data in a more intuitive and conversational manner.
 - Metadata augmentation: Enhance existing metadata with LLMs, enabling the creation of new metadata and the improvement of existing metadata.
 - AI-powered insights: Extract valuable insights from datasets using LLMs, empowering data exploration, trend analysis, and knowledge discovery.
 - Dynamic integration: Through the use of metadata standards and schemas, load and utilize your own Python scripts containing LLM functionality on-the-fly, seamlessly incorporating them into your project through plug-ins.
 - Natural language processing: Leverage LLMs to analyze and process textual data, enabling tasks like sentiment analysis, text classification, and language translation.
 
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
-Please see [CONTRIBUTING.md](CONTRIBUTING.md) for more information.
+Please see [CONTRIBUTING.md](.github/CONTRIBUTING.md) for more information.
 
 ## License
 
 LLM4Data is licensed under the [ World Bank Master Community License Agreement](LICENSE).
 
+
+## Upcoming Features
+
+- [ ] Metadata augmentation with LLM
+- [ ] Document and metadata indexing
+- [ ] Semantic search:
+  - [ ] For indicators
+  - [ ] For documents
+  - [ ] For microdata
+  - [ ] For geospatial data
+  - [ ] For voice and videos
+- [ ] Open-source chat UI
+- [ ] Data use framework
+
+
+## TODO
+
+- [ ] Add contributing guidelines
+- [ ] Add more documentations
+- [ ] Add unit tests
+- [ ] Add CI/CD
+
```

