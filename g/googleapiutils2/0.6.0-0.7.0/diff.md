# Comparing `tmp/googleapiutils2-0.6.0.tar.gz` & `tmp/googleapiutils2-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.6.0.tar", max compression
+gzip compressed data, was "googleapiutils2-0.7.0.tar", max compression
```

## Comparing `googleapiutils2-0.6.0.tar` & `googleapiutils2-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.6.0/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.6.0/README.md
--rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.6.0/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.6.0/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.6.0/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.6.0/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.6.0/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1040 2023-05-25 17:49:07.456779 googleapiutils2-0.6.0/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.6.0/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.6.0/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.6.0/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    20550 2023-05-30 20:16:51.953461 googleapiutils2-0.6.0/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     4966 2023-05-25 18:06:02.584876 googleapiutils2-0.6.0/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     7471 2023-05-30 19:56:34.731914 googleapiutils2-0.6.0/googleapiutils2/utils.py
--rw-r--r--   0        0        0      846 2023-05-30 20:18:18.198374 googleapiutils2-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.7.0/README.md
+-rw-r--r--   0        0        0       96 2023-06-01 17:02:06.802855 googleapiutils2-0.7.0/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.7.0/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.7.0/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.7.0/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.7.0/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1040 2023-05-25 17:49:07.456779 googleapiutils2-0.7.0/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.7.0/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.7.0/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     7443 2023-06-01 17:26:02.003498 googleapiutils2-0.7.0/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    24151 2023-06-01 20:48:26.565632 googleapiutils2-0.7.0/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5310 2023-06-01 18:17:35.266727 googleapiutils2-0.7.0/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     7497 2023-06-01 20:46:27.789563 googleapiutils2-0.7.0/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1067 2023-06-01 20:55:40.347638 googleapiutils2-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.7.0/PKG-INFO
```

### Comparing `googleapiutils2-0.6.0/LICENSE` & `googleapiutils2-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.6.0/README.md` & `googleapiutils2-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.6.0/googleapiutils2/drive/drive.py` & `googleapiutils2-0.7.0/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.6.0/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.7.0/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.6.0/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.7.0/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.6.0/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.7.0/googleapiutils2/sheets/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,41 +4,60 @@
 from dataclasses import dataclass
 from enum import Enum
 from types import EllipsisType
 from typing import *
 
 from ..utils import to_base
 
+
 VERSION = "v4"
 
 DEFAULT_SHEET_NAME = "Sheet1"
 
 DEFAULT_SHEET_SHAPE = (1000, 26)
 
+SheetsValues = list[list[Any]] | list[dict[str | Any, Any]]
+
 
 class ValueInputOption(Enum):
+    """How the input data should be interpreted."""
+
+    # The values the user has entered will not be parsed and will be stored as-is.
     unspecified = "INPUT_VALUE_OPTION_UNSPECIFIED"
+    # The values will be parsed as if the user typed them into the UI. Numbers will stay as
     raw = "RAW"
+    # The values will be parsed as if the user typed them into the UI, but numbers will be
     user_entered = "USER_ENTERED"
 
 
 class ValueRenderOption(Enum):
+    """How values should be represented in the output."""
+
+    # The values will be represented as they are formatted in the sheet.
     formatted = "FORMATTED_VALUE"
+    # The values will be represented as they are in the sheet, without formatting.
     unformatted = "UNFORMATTED_VALUE"
+    # The values will be represented as the formula (e.g. "=A1+B1") that is stored in the sheet.
     formula = "FORMULA"
 
 
 class InsertDataOption(Enum):
+    """How the input data should be inserted."""
+
+    # Rows are inserted for the new data.
     insert = "INSERT_ROWS"
+    # Rows are overwritten with the new data.
     overwrite = "OVERWRITE"
 
 
 def format_range_name(
     sheet_name: str | None = None, range_name: str | None = None
 ) -> str:
+    """Format a range name for use in a Google Sheets API request."""
+
     if sheet_name is not None and range_name is not None:
         if not (sheet_name.startswith("'") and sheet_name.endswith("'")):
             sheet_name = f"'{sheet_name}'"
         return f"{sheet_name}!{range_name}"
     elif range_name is not None:
         return range_name
     elif sheet_name is not None:
@@ -70,16 +89,16 @@
         return a1, None
 
     a1 = a1.lower()
     if ":" in a1:
         row, col = a1.split(":")
         return finder(row), finder(col)
     else:
-        row = finder(a1)
-        return row, row
+        new_row = finder(a1)
+        return new_row, new_row
 
 
 def slices_to_A1(row_ix: slice, col_ix: slice) -> tuple[str, str]:
     return (
         rc_to_A1(row_ix.start, col_ix.start),
         rc_to_A1(row_ix.stop, col_ix.stop),
     )
@@ -129,14 +148,15 @@
 
 def expand_slices(
     row_ix: slice | int, col_ix: slice | int, shape: tuple[int, int] | None
 ) -> list[str | None]:
     row_ix, col_ix = to_slice(row_ix, col_ix, shape=shape)
     row_ix, col_ix = slices_to_A1(row_ix, col_ix)
     range_name = f"{row_ix}:{col_ix}" if row_ix != "" and col_ix != "" else None
+
     return range_name
 
 
 def parse_sheets_ixs(
     ixs: str | tuple[Any, ...], shape: tuple[int, int] | None
 ) -> tuple[str | None, str | None]:
     match ixs:
@@ -148,15 +168,17 @@
             return sheet_name, expand_slices(row_ix, col_ix, shape=shape)
         case row_ix, col_ix:
             return None, expand_slices(row_ix, col_ix, shape=shape)
         case _:
             raise IndexError(f"Invalid index: {ixs}")
 
 
-def reverse_sheet_range(range_name: str) -> tuple[str, str]:
+def reverse_sheet_range(range_name: Any) -> tuple[str, str]:
+    range_name = str(range_name)
+
     if "!" in range_name:
         sheet_name, range_name = range_name.split("!")
         return sheet_name, range_name
 
     if ":" in range_name:
         return DEFAULT_SHEET_NAME, range_name
     else:
```

### Comparing `googleapiutils2-0.6.0/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.7.0/googleapiutils2/sheets/sheets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
+from collections import defaultdict
 
 import logging
 import operator
+import time
 from typing import *
 
 import pandas as pd
 from cachetools import TTLCache, cachedmethod
 from google.oauth2.credentials import Credentials
 from googleapiclient import discovery
 
-from ..utils import nested_defaultdict, parse_file_id
+from ..utils import THROTTLE_TIME, nested_defaultdict, parse_file_id
 from .misc import (
     DEFAULT_SHEET_NAME,
     VERSION,
     InsertDataOption,
     SheetSlice,
     SheetSliceT,
+    SheetsValues,
     ValueInputOption,
     ValueRenderOption,
     reverse_sheet_range,
 )
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
@@ -37,25 +40,33 @@
         SpreadsheetProperties,
         UpdateValuesResponse,
         ValueRange,
     )
 
 logger = logging.getLogger(__name__)
 
+SheetsRange = str | SheetSliceT | Any
+
 
 class Sheets:
-    def __init__(self, creds: Credentials):
+    def __init__(self, creds: Credentials, throttle_time: float = THROTTLE_TIME):
         self.creds = creds
         self.service: SheetsResource = discovery.build(  # type: ignore
             "sheets", VERSION, credentials=self.creds
         )
         self.sheets: SheetsResource.SpreadsheetsResource = self.service.spreadsheets()
+        self.throttle_time = throttle_time
 
         self._cache: TTLCache = TTLCache(maxsize=128, ttl=80)
 
+        self._batched_data: DefaultDict[
+            str, dict[str | Any, SheetsValues]
+        ] = defaultdict(dict)
+        self._prev_time: Optional[float] = None
+
     def create(
         self,
         title: str,
         sheet_names: list[str] | None = None,
         body: Spreadsheet | None = None,  # type: ignore
     ):
         body: Spreadsheet = nested_defaultdict(body if body else {})  # type: ignore
@@ -63,15 +74,15 @@
 
         body["properties"]["title"] = title  # type: ignore
         for n, sheet_name in enumerate(sheet_names):
             body["sheets"][n]["properties"]["title"] = sheet_name  # type: ignore
 
         body["sheets"] = list(body["sheets"].values())  # type: ignore
 
-        return self.sheets.create(body=body).execute()
+        return self.sheets.create(body=body).execute()  # type: ignore
 
     def copy_to(
         self,
         from_spreadsheet_id: str,
         from_sheet_id: int,
         to_spreadsheet_id: str,
     ):
@@ -88,54 +99,54 @@
         )
         body: CopySheetToAnotherSpreadsheetRequest = {
             "destinationSpreadsheetId": to_spreadsheet_id
         }
 
         return (
             self.sheets.sheets()
-            .copyTo(
+            .copyTo(  # type: ignore
                 spreadsheetId=from_spreadsheet_id,
                 sheetId=from_sheet_id,
                 body=body,
             )
             .execute()
         )
 
-    def get(
+    def get_spreadsheet(
         self,
         spreadsheet_id: str,
     ) -> Spreadsheet:
         spreadsheet_id = parse_file_id(spreadsheet_id)
         return self.sheets.get(spreadsheetId=spreadsheet_id).execute()
 
-    def get_sheet(
+    def get(
         self,
         spreadsheet_id: str,
         name: str | None = None,
         sheet_id: int | None = None,
     ) -> Sheet | None:
         """Get a sheet from a spreadsheet. Either the name or the ID of the sheet must be provided.
 
         Args:
             spreadsheet_id (str): The ID of the spreadsheet containing the sheet to get.
             name (str, optional): The name of the sheet to get. Defaults to None.
             sheet_id (int, optional): The ID of the sheet to get. Defaults to None.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
-        spreadsheet = self.get(spreadsheet_id)
+        spreadsheet = self.get_spreadsheet(spreadsheet_id)
 
         for sheet in spreadsheet["sheets"]:
             if sheet_id is not None and sheet["properties"]["sheetId"] == sheet_id:
                 return sheet
             if name is not None and sheet["properties"]["title"] == name:
                 return sheet
 
         return None
 
-    def rename_sheet(
+    def rename(
         self,
         spreadsheet_id: str,
         sheet_id: int,
         new_name: str,
     ):
         """Rename a sheet in a spreadsheet.
 
@@ -155,15 +166,15 @@
                 }
             ]
         }
         return self.sheets.batchUpdate(
             spreadsheetId=spreadsheet_id, body=body
         ).execute()
 
-    def add_sheet(
+    def add(
         self,
         spreadsheet_id: str,
         names: str | list[str],
         rows: int = 1000,
         cols: int = 26,
         index: int | None = None,
         **kwargs: Any,
@@ -206,15 +217,15 @@
 
         return self.sheets.batchUpdate(
             spreadsheetId=spreadsheet_id,
             body=body,
             **kwargs,
         ).execute()
 
-    def delete_sheet(
+    def delete(
         self,
         spreadsheet_id: str,
         sheet_id: int,
         **kwargs: Any,
     ):
         """Deletes a sheet from a spreadsheet.
 
@@ -238,23 +249,23 @@
             body=body,
             **kwargs,
         ).execute()
 
     def values(
         self,
         spreadsheet_id: str,
-        range_name: str | Any = DEFAULT_SHEET_NAME,
+        range_name: SheetsRange = DEFAULT_SHEET_NAME,
         value_render_option: ValueRenderOption = ValueRenderOption.unformatted,
         **kwargs: Any,
     ):
         """Get values from a spreadsheet within a range.
 
         Args:
             spreadsheet_id (str): The spreadsheet ID.
-            range_name (str | Any, optional): The range to get values from. Defaults to DEFAULT_SHEET_NAME.
+            range_name (SheetsRange, optional): The range to get values from. Defaults to DEFAULT_SHEET_NAME.
             value_render_option (ValueRenderOption, optional): The value render option. Defaults to ValueRenderOption.unformatted.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
         return (
             self.sheets.values()
             .get(
@@ -264,216 +275,293 @@
                 **kwargs,
             )
             .execute()
         )
 
     @cachedmethod(operator.attrgetter("_cache"))
     def _header(self, spreadsheet_id: str, sheet_name: str = DEFAULT_SHEET_NAME):
-        """Get the header of a sheet; cache the result"""
+        """Get the header of a sheet; cache the result."""
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(SheetSlice[sheet_name, 1, ...])
         return self.values(spreadsheet_id=spreadsheet_id, range_name=range_name).get(
             "values", [[]]
         )[0]
 
     def _dict_to_values_align_columns(
         self,
         spreadsheet_id: str,
-        range_name: str,
-        rows: list[dict],
+        range_name: SheetsRange,
+        rows: list[dict[SheetsRange, Any]],
         align_columns: bool = True,
     ):
-        if align_columns:
-            sheet_name, _ = reverse_sheet_range(range_name)
-            header = self._header(spreadsheet_id, sheet_name)
-            header = pd.Index(header).astype(str)
+        """Transforms a list of dictionaries into a list of lists, aligning the columns with the header.
+        If new columns were added, the header is appended to the right; the header of the sheet is updated.
 
-            frame = pd.DataFrame(rows)
-            frame = frame.reindex(
-                list(rows[0].keys()), axis=1
-            )  # preserve the insertion order
-            frame.index = frame.index.astype(str)
-
-            if len(diff := frame.columns.difference(header)):
-                # only align columns if there are new columns
-                header = header.append(diff)
-                sheet_name, _ = reverse_sheet_range(range_name)
-                self.update(
-                    spreadsheet_id,
-                    SheetSlice[sheet_name, 1, ...],
-                    [header.tolist()],
-                )
-                self._cache[(spreadsheet_id, sheet_name)] = list(header)
-
-            other = pd.DataFrame(columns=header)
-            frame = pd.concat([other, frame], ignore_index=True).fillna("")
-            return frame.values.tolist()
-        else:
+        Args:
+            spreadsheet_id (str): The spreadsheet ID.
+            range_name (SheetsRange): The range to update.
+            rows (list[dict[SheetsRange, Any]]): The rows to update.
+            align_columns (bool, optional): Whether to align the columns with the header. Defaults to True.
+        """
+        if not align_columns:
             logger.debug("align_columns is False, skipping column alignment")
             return [list(row.values()) for row in rows]
 
-    def _process_values(
+        sheet_name, _ = reverse_sheet_range(range_name)
+        header = self._header(spreadsheet_id, sheet_name)
+        header = pd.Index(header).astype(str)
+
+        frame = pd.DataFrame(rows)
+        frame = frame.reindex(
+            list(rows[0].keys()), axis=1
+        )  # preserve the insertion order
+        frame.index = frame.index.astype(str)
+
+        if len(diff := frame.columns.difference(header)):
+            header = header.append(diff)
+            sheet_name, _ = reverse_sheet_range(range_name)
+            self.update(
+                spreadsheet_id,
+                SheetSlice[sheet_name, 1, ...],
+                [header.tolist()],
+            )
+            self._cache[(spreadsheet_id, sheet_name)] = list(header)
+
+        frame = frame.reindex(columns=header)
+        return frame.fillna("").values.tolist()  # fill null values with an empty string
+
+    def _process_sheets_values(
         self,
         spreadsheet_id: str,
-        range_name: str,
-        values: list[list[Any]] | list[dict],
+        range_name: SheetsRange,
+        values: SheetsValues,
         align_columns: bool = True,
-    ) -> list[list[Any]] | list[dict]:
+    ) -> list[list[Any]]:
         if all(isinstance(value, dict) for value in values):
             return self._dict_to_values_align_columns(
                 spreadsheet_id=spreadsheet_id,
                 range_name=range_name,
                 rows=values,  # type: ignore
                 align_columns=align_columns,
             )
         else:
-            return values
+            return values  # type: ignore
 
     def update(
         self,
         spreadsheet_id: str,
-        range_name: str | Any,
-        values: list[list[Any]] | list[dict] | list[Any],
+        range_name: SheetsRange,
+        values: SheetsValues,
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
         align_columns: bool = True,
     ):
         """Updates a range of values in a spreadsheet.
 
         If `values` is a list of dicts, the keys of the first dict will be used as the header row.
         Further, if the input is a list of dicts and `align_columns` is True, the columns of the spreadsheet
         will be aligned with the keys of the first dict.
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
-            range_name (str | Any): The range to update. Can be a string or a SheetSlice.
-            values (list[list[Any]] | list[dict]): The values to update.
+            range_name (SheetsRange): The range to update.
+            values (SheetsValues): The values to update.
             value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
             align_columns (bool, optional): Whether to align the columns of the spreadsheet with the keys of the first row of the values. Defaults to True.
-
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
-        values = self._process_values(spreadsheet_id, range_name, values, align_columns)
+        values = self._process_sheets_values(
+            spreadsheet_id, range_name, values, align_columns
+        )
 
         return (
             self.sheets.values()
             .update(
                 spreadsheetId=spreadsheet_id,
                 range=range_name,
                 body={"values": values},  # type: ignore
                 valueInputOption=value_input_option.value,
             )
             .execute()
         )
 
-    def batch_update(
+    def _batch_update(
         self,
         spreadsheet_id: str,
-        data: dict[str | Any, list[list[Any]] | list[dict]],
+        data: dict[SheetsRange, SheetsValues],
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
         align_columns: bool = True,
     ):
-        """Updates a series of range values in a spreadsheet. Much faster version of calling `update` multiple times.
-        See `update` for more details.
-
-        Args:
-            spreadsheet_id (str): The spreadsheet to update.
-            data (dict): A dict of {range_name: values} to update;
-                        values: list[list[Any]] | list[dict].
-            value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
-            align_columns (bool, optional): Whether to align the columns of the spreadsheet with the keys of the first row of the values. Defaults to True.
-        """
-        spreadsheet_id = parse_file_id(spreadsheet_id)
-
-        batch: list[ValueRange] = [
+        """Internal method for batch updating values. Use `batch_update` instead."""
+        new_data: list[ValueRange] = [
             {
                 "range": (str_range_name := str(range_name)),
-                "values": self._process_values(
+                "values": self._process_sheets_values(
                     spreadsheet_id=spreadsheet_id,
                     range_name=str_range_name,
                     values=values,
                     align_columns=align_columns,
                 ),
             }
             for range_name, values in data.items()
-        ]  # type: ignore
+        ]
 
         body: BatchUpdateValuesRequest = {
             "valueInputOption": value_input_option.value,
-            "data": batch,
+            "data": new_data,
         }
         return (
             self.sheets.values()
             .batchUpdate(
                 spreadsheetId=spreadsheet_id,
                 body=body,
             )
             .execute()
         )
 
+    def batch_update(
+        self,
+        spreadsheet_id: str,
+        data: dict[SheetsRange, SheetsValues],
+        value_input_option: ValueInputOption = ValueInputOption.user_entered,
+        align_columns: bool = True,
+        batch_size: int | None = None,
+    ):
+        """Updates a series of range values in a spreadsheet. Much faster version of calling `update` multiple times.
+        See `update` for more details.
+
+        If the `batch_size` is None, all updates will be batched together. Otherwise, the updates will be batched by the following
+        rules:
+        -   If the number of updates is greater than `batch_size` AND
+        -   If the time between the first update and the last update is greater than `THROTTLE_TIME` OR
+
+        Args:
+            spreadsheet_id (str): The spreadsheet to update.
+            data (dict[SheetsRange, SheetsValues]): The data to update.
+            value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
+            align_columns (bool, optional): Whether to align the columns of the spreadsheet with the keys of the first row of the values. Defaults to True.
+            batch_size (int | None, optional): The number of updates to batch together. If None, all updates will be batched together. Defaults to None.
+        """
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+
+        if batch_size is None:
+            return self._batch_update(
+                spreadsheet_id=spreadsheet_id,
+                data=data,
+                value_input_option=value_input_option,
+                align_columns=align_columns,
+            )
+
+        batched_data = self._batched_data[spreadsheet_id]
+
+        if data is not None:
+            self._batched_data[spreadsheet_id] |= data
+
+        curr_time = time.perf_counter()
+        dt = (
+            curr_time - self._prev_time
+            if self._prev_time is not None
+            else self.throttle_time
+        )
+
+        # If the conditions for a batch update are not met, simply return
+        if not (dt >= self.throttle_time and len(batched_data) >= batch_size):
+            return None
+
+        self._prev_time = curr_time
+        res = self._batch_update(
+            spreadsheet_id=spreadsheet_id,
+            data=batched_data,
+            value_input_option=value_input_option,
+            align_columns=align_columns,
+        )
+        self._batched_data[spreadsheet_id].clear()
+
+        return res
+
+    def batched_update_remaining(self, spreadsheet_id: str):
+        """Updates any remaining batched data that's been left over from previous calls to `batch_update`."""
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+        batched_data = self._batched_data[spreadsheet_id]
+
+        res = self._batch_update(
+            spreadsheet_id=spreadsheet_id,
+            data=batched_data,
+        )
+        self._batched_data[spreadsheet_id].clear()
+        return res
+
     def append(
         self,
         spreadsheet_id: str,
-        range_name: str | Any,
-        values: list[list[Any]],
+        range_name: SheetsRange,
+        values: SheetsValues,
         insert_data_option: InsertDataOption = InsertDataOption.overwrite,
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
         align_columns: bool = True,
     ):
-        """Appends values to a spreadsheet. Like `update`, but appends instead of overwrites.
+        """Appends values to a spreadsheet. Like `update`, but searches for the next available row to append to.
         This means rows will be added to the spreadsheet if the input values are longer than the
-        number of existing rows.
+        number of existing rows. See: https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/append
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
-            range_name (str | Any): The range to update. Can be a string or a SheetSlice.
+            range_name (SheetsRange): The range to update.
             values (list[list[Any]]): The values to append.
             insert_data_option (InsertDataOption, optional): How the input data should be inserted. Defaults to InsertDataOption.overwrite.
             value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
             align_columns (bool, optional): Whether to align the columns of the spreadsheet with the keys of the first row of the values. Defaults to True.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
         body: ValueRange = {
-            "values": self._process_values(
-                spreadsheet_id, range_name, values, align_columns
-            )  # type: ignore
+            "values": self._process_sheets_values(
+                spreadsheet_id=spreadsheet_id,
+                range_name=range_name,
+                values=values,
+                align_columns=align_columns,
+            )
         }
 
         return (
             self.sheets.values()
             .append(
                 spreadsheetId=spreadsheet_id,
                 range=range_name,
                 body=body,
                 insertDataOption=insert_data_option.value,
                 valueInputOption=value_input_option.value,
             )
             .execute()
         )
 
-    def clear(self, spreadsheet_id: str, range_name: str | Any):
+    def clear(
+        self,
+        spreadsheet_id: str,
+        range_name: SheetsRange,
+    ):
         """Clears a range of values in a spreadsheet.
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
-            range_name (str | Any): The range to update. Can be a string or a SheetSlice.
+            range_name (SheetsRange): The range to clear.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
 
         return (
             self.sheets.values()
             .clear(spreadsheetId=spreadsheet_id, range=range_name)
             .execute()
         )
 
     @staticmethod
     def to_frame(values: ValueRange, **kwargs: Any) -> pd.DataFrame | None:
         """Converts a ValueRange to a DataFrame.
+
         Useful for working with the data in Pandas after a call to sheets.values().
         If one of the keyword arguments to the dataframe is "columns",
         the first row of the values will be used as the column names, aligned to the data.
 
         All string values that are empty will be converted to pd.NA,
         and the data types of the columns will be inferred.
 
@@ -536,45 +624,57 @@
                 {
                     "autoResizeDimensions": {
                         "dimensions": make_range(i),
                     }
                 }
                 for i in range(num_columns)
             ]
-        else:
-            if isinstance(widths, int):
-                widths = [widths] * num_columns
 
-            return [
-                {
-                    "updateDimensionProperties": {
-                        "range": make_range(i),
-                        "properties": {"pixelSize": widths[i]},
-                        "fields": "pixelSize",
-                    }
+        if isinstance(widths, int):
+            widths = [widths] * num_columns
+        return [
+            {
+                "updateDimensionProperties": {
+                    "range": make_range(i),
+                    "properties": {"pixelSize": widths[i]},
+                    "fields": "pixelSize",
                 }
-                for i in range(num_columns)
-            ]
+            }
+            for i in range(num_columns)
+        ]
 
     def resize_columns(
         self, spreadsheet_id: str, sheet_name: str, width: int | None = 100
     ):
         """Resizes the columns of a sheet.
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
             sheet_name (str): The name of the sheet to update.
             width (int, optional): The width to set the columns to. Defaults to 100. If None, will auto-resize.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
-        sheet = self.get_sheet(spreadsheet_id, name=sheet_name)
-        if not sheet:
+        sheet = self.get(spreadsheet_id, name=sheet_name)
+        if sheet is None:
             raise ValueError(f"Sheet '{sheet_name}' not found in the given spreadsheet")
 
-        body: BatchUpdateSpreadsheetRequest = {
-            "requests": self._resize_columns(sheet, width)
-        }
-        return (
-            self.service.spreadsheets()
-            .batchUpdate(spreadsheetId=spreadsheet_id, body=body)
-            .execute()
-        )
+        def resize():
+            body: BatchUpdateSpreadsheetRequest = {
+                "requests": self._resize_columns(sheet, width)  # type: ignore
+            }
+            return (
+                self.service.spreadsheets()
+                .batchUpdate(spreadsheetId=spreadsheet_id, body=body)
+                .execute()
+            )
+
+        if width is None:
+            header = self._header(spreadsheet_id, sheet_name)
+            res = self.append(spreadsheet_id, sheet_name, [header])
+            updated_range = res["updates"]["updatedRange"]
+
+            res = resize()
+
+            self.clear(spreadsheet_id, updated_range)
+            return res
+        else:
+            return resize()
```

### Comparing `googleapiutils2-0.6.0/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.7.0/googleapiutils2/sheets/sheets_value_range.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,24 +68,32 @@
     def header(self) -> list[str]:
         return self.sheets._header(
             spreadsheet_id=self.spreadsheet_id, sheet_name=self.sheet_name
         )
 
     @cachedmethod(operator.attrgetter("_cache"))
     def shape(self) -> tuple[int, int]:
-        for sheet in self.sheets.get(self.spreadsheet_id).get("sheets", []):
+        for sheet in self.sheets.get_spreadsheet(self.spreadsheet_id).get("sheets", []):
             properties = sheet.get("properties", {})
             if properties.get("title") == self.sheet_name:
                 grid_properties = properties.get("gridProperties", {})
                 return (
                     grid_properties.get("rowCount", 0),
                     grid_properties.get("columnCount", 0),
                 )
         return DEFAULT_SHEET_SHAPE
 
+    @cachedmethod(operator.attrgetter("_cache"))
+    def sheet_id(self) -> int:
+        for sheet in self.sheets.get_spreadsheet(self.spreadsheet_id).get("sheets", []):
+            properties = sheet.get("properties", {})
+            if properties.get("title") == self.sheet_name:
+                return properties.get("sheetId", 0)
+        return 0
+
     def values(
         self,
         value_render_option: ValueRenderOption = ValueRenderOption.unformatted,
     ):
         return self.sheets.values(
             spreadsheet_id=self.spreadsheet_id,
             range_name=str(self),
@@ -102,19 +110,19 @@
             spreadsheet_id=self.spreadsheet_id,
             range_name=str(self),
             values=values,
             value_input_option=value_input_option,
             align_columns=align_columns,
         )
 
-    def rename(self, new_sheet_name: str):
-        return self.sheets.rename_sheet(
+    def rename(self, new_name: str):
+        return self.sheets.rename(
             spreadsheet_id=self.spreadsheet_id,
-            curr_name=self.sheet_name,
-            new_name=new_sheet_name,
+            sheet_id=self.sheet_id(),
+            new_name=new_name,
         )
 
     def append(
         self,
         values: list[list[Any]],
         insert_data_option: InsertDataOption = InsertDataOption.overwrite,
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
```

### Comparing `googleapiutils2-0.6.0/googleapiutils2/utils.py` & `googleapiutils2-0.7.0/googleapiutils2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from enum import Enum
 from functools import cache
 from pathlib import Path
 from typing import *
 
 import googleapiclient.http
 import requests
+
 from google.auth.transport.requests import Request
 from google.oauth2 import service_account
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 
 FilePath = str | Path
 
-
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
     from googleapiclient._apis.sheets.v4.resources import Spreadsheet
 
 
+THROTTLE_TIME = 30
+
 SCOPES = [
     "https://www.googleapis.com/auth/spreadsheets",
     "https://www.googleapis.com/auth/drive.file",
     "https://www.googleapis.com/auth/drive",
 ]
 
 
@@ -232,15 +234,17 @@
         y.append(x % base)
         if (x := (x // base) - 1) < 0:
             break
 
     return y[::-1]
 
 
-def nested_defaultdict(existing: dict | Any | None = None, **kwargs: Any) -> dict[Any, Any]:
+def nested_defaultdict(
+    existing: dict | Any | None = None, **kwargs: Any
+) -> dict[Any, Any]:
     if existing is None:
         existing = {}
     elif not isinstance(existing, dict):
         return existing
     existing = {key: nested_defaultdict(val) for key, val in existing.items()}
     return defaultdict(nested_defaultdict, existing, **kwargs)
```

### Comparing `googleapiutils2-0.6.0/pyproject.toml` & `googleapiutils2-0.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.6.0"
+version = "0.7.0"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
@@ -24,10 +24,22 @@
 [tool.poetry.group.dev.dependencies]
 types-requests = "^2.31.0.1"
 types-cachetools = "^5.3.0.5"
 pytest = "^7.3.1"
 pandas-stubs = "^2.0.1.230501"
 black = "^23.3.0"
 
+[tool.mypy]
+python_version = "3.10"
+warn_return_any = false
+warn_unused_configs = false
+disallow_untyped_defs = false
+check_untyped_defs = true
+
+
+[[tool.mypy.overrides]]
+module = "google.*"
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `googleapiutils2-0.6.0/PKG-INFO` & `googleapiutils2-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.6.0
+Version: 0.7.0
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

