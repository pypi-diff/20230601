# Comparing `tmp/xt_st_common-0.5.2.tar.gz` & `tmp/xt_st_common-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xt_st_common-0.5.2.tar", max compression
+gzip compressed data, was "xt_st_common-0.5.3.tar", max compression
```

## Comparing `xt_st_common-0.5.2.tar` & `xt_st_common-0.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      720 2023-06-01 08:25:47.344884 xt_st_common-0.5.2/README.md
--rw-r--r--   0        0        0     2603 2023-06-01 08:25:47.344884 xt_st_common-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     6128 2023-06-01 08:25:13.036578 xt_st_common-0.5.2/src/streamlit_plotly_events/__init__.py
--rw-r--r--   0        0        0      180 2023-06-01 08:25:13.036578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/.env
--rw-r--r--   0        0        0       67 2023-06-01 08:25:13.036578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/.prettierrc
--rw-r--r--   0        0        0      859 2023-06-01 08:25:13.040578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/asset-manifest.json
--rw-r--r--   0        0        0     2052 2023-06-01 08:25:13.040578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/index.html
--rw-r--r--   0        0        0      564 2023-06-01 08:25:13.040578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
--rw-r--r--   0        0        0     1183 2023-06-01 08:25:13.040578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/service-worker.js
--rw-r--r--   0        0        0  4138182 2023-06-01 08:25:13.060578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
--rw-r--r--   0        0        0     3326 2023-06-01 08:25:13.060578 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
--rw-r--r--   0        0        0 16152785 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
--rw-r--r--   0        0        0     1442 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
--rw-r--r--   0        0        0     3848 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
--rw-r--r--   0        0        0     1598 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0        0        0     8317 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
--rw-r--r--   0        0        0     1141 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/package.json
--rw-r--r--   0        0        0      839 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/public/index.html
--rw-r--r--   0        0        0     1922 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
--rw-r--r--   0        0        0      274 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      459 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/tsconfig.json
--rw-r--r--   0        0        0       22 2023-06-01 08:25:47.344884 xt_st_common-0.5.2/src/xt_st_common/__init__.py
--rw-r--r--   0        0        0     5010 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/components.py
--rw-r--r--   0        0        0     2371 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/config.py
--rw-r--r--   0        0        0     3177 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/database.py
--rw-r--r--   0        0        0     6303 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/fs_upload_page.py
--rw-r--r--   0        0        0    21217 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/project_components.py
--rw-r--r--   0        0        0     6518 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/project_models.py
--rw-r--r--   0        0        0     5976 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/session.py
--rw-r--r--   0        0        0     6251 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/storage.py
--rw-r--r--   0        0        0     1957 2023-06-01 08:25:13.144579 xt_st_common-0.5.2/src/xt_st_common/utils.py
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      720 2023-06-01 11:30:34.282081 xt_st_common-0.5.3/README.md
+-rw-r--r--   0        0        0     2603 2023-06-01 11:30:34.282081 xt_st_common-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6128 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/.env
+-rw-r--r--   0        0        0       67 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/.prettierrc
+-rw-r--r--   0        0        0      859 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0     2052 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/index.html
+-rw-r--r--   0        0        0      564 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js
+-rw-r--r--   0        0        0     1183 2023-06-01 11:29:58.898501 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/service-worker.js
+-rw-r--r--   0        0        0  4138182 2023-06-01 11:29:58.926504 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js
+-rw-r--r--   0        0        0     3326 2023-06-01 11:29:58.926504 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0 16152785 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map
+-rw-r--r--   0        0        0     1442 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js
+-rw-r--r--   0        0        0     3848 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map
+-rw-r--r--   0        0        0     1598 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0        0        0     8317 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map
+-rw-r--r--   0        0        0     1141 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/package.json
+-rw-r--r--   0        0        0      839 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/public/index.html
+-rw-r--r--   0        0        0     1922 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx
+-rw-r--r--   0        0        0      274 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/tsconfig.json
+-rw-r--r--   0        0        0       22 2023-06-01 11:30:34.282081 xt_st_common-0.5.3/src/xt_st_common/__init__.py
+-rw-r--r--   0        0        0     5010 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/components.py
+-rw-r--r--   0        0        0     2371 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/config.py
+-rw-r--r--   0        0        0     3177 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/database.py
+-rw-r--r--   0        0        0     6303 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/fs_upload_page.py
+-rw-r--r--   0        0        0    21814 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/project_components.py
+-rw-r--r--   0        0        0     6518 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/project_models.py
+-rw-r--r--   0        0        0     5976 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/session.py
+-rw-r--r--   0        0        0     6251 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/storage.py
+-rw-r--r--   0        0        0     1957 2023-06-01 11:29:59.018513 xt_st_common-0.5.3/src/xt_st_common/utils.py
+-rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 xt_st_common-0.5.3/PKG-INFO
```

### Comparing `xt_st_common-0.5.2/README.md` & `xt_st_common-0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# XT-STREAMLIT - 0.5.2
+# XT-STREAMLIT - 0.5.3
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

### Comparing `xt_st_common-0.5.2/pyproject.toml` & `xt_st_common-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xt-st-common"
-version = "0.5.2"
+version = "0.5.3"
 description = "Common Streamlit framework used by Exploration Toolkit"
 authors = ["Alex Hunt <alex.hunt@csiro.au>", "Sam Bradley <sam.bradley@csiro.au>", "John Hille <john.hille@csiro.au>"]
 readme = "README.md"
 packages = [{include = "xt_st_common", from= "src"}, {include = "streamlit_plotly_events", from= "src"}]
 
 [tool.poe.tasks]
 test = { cmd="pytest --cov=src/xt_st_common", help="Run unit tests"}
```

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/__init__.py` & `xt_st_common-0.5.3/src/streamlit_plotly_events/__init__.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/asset-manifest.json` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/index.html` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/precache-manifest.e3df0e84b856a278b39da3a085481f45.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/service-worker.js` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/2.a9de1b85.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/main.2ba31fb4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/package.json` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/package.json`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/public/index.html` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx` & `xt_st_common-0.5.3/src/streamlit_plotly_events/frontend/src/StreamlitPlotlyEventsComponent.tsx`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/xt_st_common/components.py` & `xt_st_common-0.5.3/src/xt_st_common/components.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/xt_st_common/config.py` & `xt_st_common-0.5.3/src/xt_st_common/config.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/xt_st_common/database.py` & `xt_st_common-0.5.3/src/xt_st_common/database.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/xt_st_common/fs_upload_page.py` & `xt_st_common-0.5.3/src/xt_st_common/fs_upload_page.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/xt_st_common/project_components.py` & `xt_st_common-0.5.3/src/xt_st_common/project_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 from xt_st_common.project_models import ProjectState
 from xt_st_common.session import get_user_email
 from xt_st_common.storage import FileRef, storage_client
 from xt_st_common.utils import get_encoding_and_dialect, get_state, seperate_users, set_state
 
 # from bson.objectid import ObjectId
 
+# mapping for language options for streamlit code formatter. For other available options
+# see: https://github.com/react-syntax-highlighter/react-syntax-highlighter/blob/master/AVAILABLE_LANGUAGES_PRISM.MD
+CODE_FORMAT_MAPPING = {"json": "json", "yaml": "yaml", "yml": "yaml", "toml": "toml", "md": "markfown"}
+
 REPLACE_FILE_HELP_TXT = (
     "The new file can have a different name but must have the same extension."
     "Warning: Uploading a new file that is significantly different to the original "
     "can have catastrophic results."
 )
 
 
@@ -393,17 +397,16 @@
     st_context=st.sidebar,
     help_text: Optional[str] = None,
     allow_upload=True,
     allow_delete=True,
     allow_replace=True,
     key_prefix: str = "",
     expand_file_actions=False,
-    folder_select_text = "Select Borehole/Run",
-    auto_parse_csv = True
-
+    folder_select_text="Select Borehole/Run",
+    auto_parse_csv=True,
 ):
     file_delete_confirm = get_state(ProjectState.FILE_DELETE_CONFIRM)
     file_to_delete = get_state(ProjectState.FILE_TO_DELETE)
     file_success_message = get_state(ProjectState.FILE_SUCCESS_MESSAGE)
     file_warning_message = get_state(ProjectState.FILE_WARNING_MESSAGE)
 
     st_context.subheader(f"Files: {project.name}")
@@ -524,22 +527,26 @@
                     preview_frame = row.button(
                         "Preview Frame",
                         key=f"{key_prefix}file_manager_preview_frame",
                     )
                     if preview_frame:
                         with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
                             st.dataframe(get_df_preview(selected_file.path, selected_file.get_ext()))
-                if selected_key.lower().endswith((".json", ".yml", ".yaml", ".txt")) and (
+                if selected_key.lower().endswith((".json", ".yml", ".yaml", ".toml", ".md", ".txt")) and (
                     preview_frame := row.button(
                         "Preview File",
                         key=f"{key_prefix}file_manager_preview_file",
                     )
                 ):
                     with st.expander(f"**Frame Viewer:** {selected_file.name}", expanded=True):
-                        st.write(get_string_preview(selected_file))
+                        code_format = CODE_FORMAT_MAPPING.get(selected_key.lower().split(".")[-1])
+                        if code_format is None:
+                            st.write(get_string_preview(selected_file))
+                        else:
+                            st.code(get_string_preview(selected_file), language=code_format)
                 if row.checkbox(
                     "Prepare Download",
                     key=f"{key_prefix}file_manager_download_chbx",
                 ):
                     file_data = storage_client().get_file(selected_file.path)
 
                     row.download_button(
```

### Comparing `xt_st_common-0.5.2/src/xt_st_common/project_models.py` & `xt_st_common-0.5.3/src/xt_st_common/project_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     def get_files_in_folder(self, folder: str, include_subfolders=True, extensions=None, null_option=None):
         _files: Dict[str, Union[None, FileRef]] = {} if null_option is None else {null_option: None}
 
         path = self.get_folder_path(folder)
         for file in self.files:
             if path in file.path:
                 file_path = file.path.removeprefix(path).strip("/")
-                if (include_subfolders or file_path.find("/") == 0) and (
+                if (include_subfolders or file_path.find("/") <= 0) and (
                     extensions is None or str(Path(file.name).suffix.lower()) in extensions
                 ):
                     _files[file_path] = file
 
         return _files
 
     def populate_node(self, _dict, part, parts):
```

### Comparing `xt_st_common-0.5.2/src/xt_st_common/session.py` & `xt_st_common-0.5.3/src/xt_st_common/session.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/xt_st_common/storage.py` & `xt_st_common-0.5.3/src/xt_st_common/storage.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/src/xt_st_common/utils.py` & `xt_st_common-0.5.3/src/xt_st_common/utils.py`

 * *Files identical despite different names*

### Comparing `xt_st_common-0.5.2/PKG-INFO` & `xt_st_common-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xt-st-common
-Version: 0.5.2
+Version: 0.5.3
 Summary: Common Streamlit framework used by Exploration Toolkit
 Author: Alex Hunt
 Author-email: alex.hunt@csiro.au
 Requires-Python: >3.9.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 Requires-Dist: pymongo (>=4.3.3) ; extra == "databases"
 Requires-Dist: pymongo-auth-aws (>=1.1.0) ; extra == "databases"
 Requires-Dist: streamlit (>=1.22.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
 Description-Content-Type: text/markdown
 
-# XT-STREAMLIT - 0.5.2
+# XT-STREAMLIT - 0.5.3
 
 This repo contains all of the common Streamlit code used by the Exploration Toolkit and CMR's Discovery Program.
 
 ## `xt-st-common` - Common Framework for XT's Streamlit apps
 
 ## Getting Started User
 TODO: Installation guide and pointer to API docs
```

