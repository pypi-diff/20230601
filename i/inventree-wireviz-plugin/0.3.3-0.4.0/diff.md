# Comparing `tmp/inventree-wireviz-plugin-0.3.3.tar.gz` & `tmp/inventree-wireviz-plugin-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inventree-wireviz-plugin-0.3.3.tar", last modified: Fri May 26 06:36:34 2023, max compression
+gzip compressed data, was "dist/inventree-wireviz-plugin-0.4.0.tar", last modified: Thu Jun  1 13:59:14 2023, max compression
```

## Comparing `inventree-wireviz-plugin-0.3.3.tar` & `inventree-wireviz-plugin-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/wireviz/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/wireviz/harness_panel.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/templates/wireviz/harness_panel.js
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz/wireviz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 06:36:33.000000 inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 06:36:34.000000 inventree-wireviz-plugin-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 06:36:25.000000 inventree-wireviz-plugin-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/wireviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/wireviz/harness_panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/templates/wireviz/harness_panel.js
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz/wireviz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-01 13:59:14.000000 inventree-wireviz-plugin-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 13:59:06.000000 inventree-wireviz-plugin-0.4.0/setup.py
```

### Comparing `inventree-wireviz-plugin-0.3.3/LICENSE` & `inventree-wireviz-plugin-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.3/inventree_wireviz/wireviz.py` & `inventree-wireviz-plugin-0.4.0/inventree_wireviz/wireviz.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,58 +4,61 @@
 
 - Render wireviz diagrams in the browser
 - Extract and integrate bills of materials from wireviz diagrams
 """
 
 import logging
 import os
-import tempfile
 
 from wireviz.Harness import Harness
 from wireviz.wireviz import parse as parse_wireviz
-from wireviz.wv_bom import bom_list
-from wireviz.wv_html import generate_html_output
 
 from django.conf import settings
 from django.core.files.base import ContentFile
 from django.db import transaction
 
 from plugin import InvenTreePlugin
-from plugin.mixins import EventMixin, PanelMixin, SettingsMixin
+from plugin.mixins import EventMixin, PanelMixin, ReportMixin, SettingsMixin
 
+from build.views import BuildDetail
 from company.models import ManufacturerPart, SupplierPart
 from InvenTree.api_version import INVENTREE_API_VERSION
 from part.models import BomItem, Part, PartAttachment
 from part.views import PartDetail
 
 from .version import PLUGIN_VERSION
 
 
 logger = logging.getLogger('inventree')
 
 
-class WirevizPlugin(EventMixin, PanelMixin, SettingsMixin, InvenTreePlugin):
+class WirevizPlugin(EventMixin, PanelMixin, ReportMixin, SettingsMixin, InvenTreePlugin):
     """"Wireviz plugin for InvenTree
     
     - Provides a custom panel for rendering wireviz diagrams
     - Automatically renders wireviz diagrams when a .wireviz file is uploaded
     - Extract BOM information from the wireviz diagram
     """
 
     AUTHOR = "Oliver Walters"
     DESCRIPTION = "Wireviz plugin for InvenTree"
     VERSION = PLUGIN_VERSION
 
+    MIN_VERSION = '0.12.0'
+
     NAME = "Wireviz"
     SLUG = "wireviz"
     TITLE = "Wireviz Plugin"
 
-    HARNESS_HTML_FILE = "wireviz_harness.html"
-    ERROR_MSG_FILE = 'wireviz_errors.txt'
-    WARNING_MSG_FILE = "wireviz_warnings.txt"
+    # Filenames and key constants
+    HARNESS_SVG_FILE = "wireviz_harness.svg"
+
+    HARNESS_SRC_KEY = "source_file"
+    HARNESS_SVG_KEY = "svg_file"
+    HARNESS_BOM_KEY = "bom_data"
 
     SETTINGS = {
         "WIREVIZ_PATH": {
             'name': 'Wireviz Upload Path',
             'description': 'Path to store uploaded wireviz template files (relative to media root)',
             'default': 'wireviz',
         },
@@ -81,70 +84,109 @@
             'name': 'Add Part Images',
             'description': 'Include part images in the wireviz diagram (not yet implemeted)',
             'default': True,
             'validator': bool,
         },
     }
 
-    def get_harness_data(self, part: Part):
-        """Return the harness html data for the part."""
-            
-        for attachment in part.attachments.all():
-            fn = attachment.attachment.name
-            if os.path.basename(fn) == self.HARNESS_HTML_FILE:
-                return attachment.attachment.read().decode()
+    def get_part_from_instance(self, instance):
+        """Return a Part object from the given instance."""
+
+        if not instance:
+            return None
+
+        if isinstance(instance, Part):
+            return instance
     
+        if hasattr(instance, 'part') and isinstance(instance.part, Part):
+            return instance.part
+        
+        # No match
         return None
 
+    def add_report_context(self, report_instance, model_instance, request, context):
+        """Inject wireviz data into the report context."""
+
+        # Extract a Part model from the model instance
+        part = self.get_part_from_instance(model_instance)
+
+        if isinstance(part, Part):
+            metadata = part.get_metadata('wireviz')
+
+            if metadata:
+                if svg_file := metadata.get(self.HARNESS_SVG_KEY, None):
+                    context['wireviz_svg_file'] = svg_file
+
+                if bom_data := metadata.get(self.HARNESS_BOM_KEY, None):
+                    context['wireviz_bom_data'] = bom_data
+
     def get_panel_context(self, view, request, context):
         """Return context information for the Wireviz panel."""
 
         try:
-            part = view.get_object()
+            instance = view.get_object()
         except AttributeError:
             return context
-        
-        if isinstance(view, PartDetail) and isinstance(part, Part):
-            # Extract any wireviz errors from the part attachments
-            for attachment in part.attachments.all():
-                fn = attachment.attachment.name
 
-                if harness_html := self.get_harness_data(part):
-                    context['wireviz_harness_html'] = harness_html
+        part = self.get_part_from_instance(instance)
+
+        if part and isinstance(part, Part):
 
-                if os.path.basename(fn) == self.ERROR_MSG_FILE:
-                    context['wireviz_errors'] = attachment.attachment.read().decode().split("\n")
+            # Get wireviz file information from part metadata
+            wireviz_metadata = part.get_metadata('wireviz')
 
-                if os.path.basename(fn) == self.WARNING_MSG_FILE:
-                    context['wireviz_warnings'] = attachment.attachment.read().decode().split("\n")
+            if wireviz_metadata:
+                svg_file = wireviz_metadata.get(self.HARNESS_SVG_KEY, None)
+                bom_data = wireviz_metadata.get(self.HARNESS_BOM_KEY, None)
+                src_file = wireviz_metadata.get(self.HARNESS_SRC_KEY, None)
+
+                if svg_file:
+                    context['wireviz_svg_file'] = os.path.join(settings.MEDIA_URL, svg_file)
+
+                if src_file:
+                    context['wireviz_source_file'] = os.path.join(settings.MEDIA_URL, src_file)
+
+                if bom_data:
+                    context['wireviz_bom_data'] = bom_data
+                
+                # Add warnings and errors
+                context['wireviz_warnings'] = wireviz_metadata.get('warnings', None)
+                context['wireviz_errors'] = wireviz_metadata.get('errors', None)
 
         return context
 
     def get_custom_panels(self, view, request):
         """Determine if custom panels should be displayed in the UI."""
 
         panels = []
 
         try:
             instance = view.get_object()
         except AttributeError:
             return panels
+        
+        part = self.get_part_from_instance(instance)
+
+        # A valid part object has been found
+        if part and isinstance(part, Part):
     
-        if isinstance(view, PartDetail):
-            part = instance
+            # We are on the PartDetail or BuildDetail page
+            if isinstance(view, PartDetail) or isinstance(view, BuildDetail):
+
+                logger.debug(f"Checking for wireviz file for part {part}")
 
-            logger.debug(f"Checking for wireviz file for part {part}")
+                metadata = part.get_metadata('wireviz')
 
-            if self.get_harness_data(part):
-                panels.append({
-                    'title': 'WireViz Harness',
-                    'icon': 'fas fa-plug',
-                    'content_template': 'wireviz/harness_panel.html',
-                    'javascript_template': 'wireviz/harness_panel.js',
-                })
+                if metadata:
+                    panels.append({
+                        'title': 'Harness Diagram',
+                        'icon': 'fas fa-project-diagram',
+                        'content_template': 'wireviz/harness_panel.html',
+                        'javascript_template': 'wireviz/harness_panel.js',
+                    })
         
         return panels
 
     def process_event(self, event, *args, **kwargs):
         """Callback for event processing.
         
         We are interested in the following events:
@@ -160,32 +202,55 @@
                 filename = attachment.attachment.name
 
                 # Store a reference to the parent Part
                 self.part = attachment.part
 
                 # Check if the attachment is a .wireviz file
                 if filename.endswith(".wireviz"):
-                    self.process_wireviz_file(filename)
-
-                    # Delete *old* wireviz files
-                    if self.get_setting('DELETE_OLD_FILES'):
-                        for attach in PartAttachment.objects.filter(part=self.part):
-                            # Don't delete this one!
-                            if attach.pk == attachment.pk:
-                                continue
-
-                            fn = attach.attachment.name
-
-                            # Delete old wireviz files
-                            if fn.endswith(".wireviz"):
-                                attach.delete()
+                    self.cleanup_old_files(filename, self.part)
+                    self.process_wireviz_file(filename, part=self.part)
 
             except PartAttachment.DoesNotExist:
                 pass
     
+    def cleanup_old_files(self, filename: str, part: Part):
+        """Remove any old wireviz files from the part."""
+
+        if not self.get_setting('DELETE_OLD_FILES'):
+            # Don't delete old files
+            return
+        
+        file_keys = [
+            self.HARNESS_SRC_KEY,
+            self.HARNESS_SVG_KEY,
+        ]
+
+        metadata = part.get_metadata('wireviz')
+
+        if not metadata:
+            # No metadata to check
+            return
+
+        filenames = []
+
+        for key in file_keys:
+            if key in metadata:
+                filenames.append(metadata[key])
+
+        for attachment in part.attachments.all():
+            fn = attachment.attachment.name
+
+            if fn == filename or os.path.basename(fn) == filename:
+                # Don't delete the newly uploaded file!
+                continue
+
+            if fn in filenames or os.path.basename(fn) in filenames:
+                logger.info(f"Deleting old wireviz file: {fn}")
+                attachment.delete()
+
     def process_wireviz_file(self, wv_file: str, part: Part = None):
         """Process a wireviz file, and extract the relevant information."""
 
         logger.info(f"WirevizPlugin: Processing wireviz file: {wv_file}")
 
         # Get a unit registry for conversion
         if INVENTREE_API_VERSION >= 117:
@@ -222,27 +287,43 @@
             )
         except Exception as exc:
             logger.error(f"WirevizPlugin: Failed to parse wireviz file: {exc}")
 
             from InvenTree.exceptions import log_error
             log_error("Wireviz Import")
             return
-
+        
         # Extract BOM data from the harness
         self.extract_bom_data(harness)
 
         if self.get_setting("ADD_IMAGES"):
             self.add_part_images(harness)
 
-        self.save_bom_data()
-        self.generate_html_output(harness)
+        wz_filename = os.path.basename(wv_file)
+
+        # Generate SVG output
+
+        try:
+            svg_file = self.generate_svg_output(harness, wz_filename)
+            svg_file = svg_file.attachment.name
+        except Exception as exc:
+            self.add_error(f"Failed to generate SVG output for wireviz file: {wv_file}")
+            self.add_error(f"Exception: {exc}")
+            svg_file = None
+
+        # Update the part metadata
+        wireviz_data = {
+            self.HARNESS_SRC_KEY: wv_file,
+            self.HARNESS_SVG_KEY: svg_file,
+            self.HARNESS_BOM_KEY: self.bom_lines,
+            'errors': self.errors,
+            'warnings': self.warnings,
+        }
 
-        # Save any error messages to a file
-        self.save_error_file()
-        self.save_warning_file()
+        part.set_metadata('wireviz', wireviz_data, overwrite=True)
 
     def prepend_wireviz_data(self):
         """Load (and prepend) any custom wireviz templates.
         
         - Any '.wireviz' files found in the WIREVIZ_PATH directory will be loaded
         - The contents of these files will be prepended to the wireviz data
         """
@@ -272,42 +353,14 @@
 
     def add_part_images(self, harness: Harness):
         """Add part images to the wireviz harness"""
         
         logger.warning("WirevizPlugin: Adding part images is not yet supported")
         
         # TODO: Implement native image support
-
-        """
-        # Path to part images directory
-        img_path = pathlib.Path(settings.MEDIA_ROOT)
-
-        for designator, part in self.part_map.items():
-
-            logger.debug(f"Checking image for {designator} - {part}")
-
-            # Check if the part has an image
-            if not part.image:
-                continue
-
-            # Check if the image exists
-            img_filename = pathlib.Path(img_path, part.image.name)
-
-            if not img_filename.exists():
-                continue
-
-            # Construct a new image object associated with the part
-            img = WirevizImage(img_filename, src=part.image.name, width=100)
-
-            # Add the image to the harness
-            if designator in harness.connectors:
-                harness.connectors[designator].image = img
-            if designator in harness.cables:
-                harness.cables[designator].image = img
-        """
                 
     @transaction.atomic
     def extract_bom_data(self, harness: Harness):
         """Extract Bill of Materials data from a wireviz harness.
         
         Arguments:
             harness: A wireviz Harness instance
@@ -315,36 +368,60 @@
         logger.info("WirevizPlugin: Extracting BOM data from wireviz harness")
 
         bom = harness.bom()
 
         # A list of BomItem objects to be created
         self.bom_items = []
 
+        # A list of BOM lines to be exported to csv
+        self.bom_lines = []
+
         for line in bom:
             designators = line.get('designators', [])
             description = line.get('description', None)
+            pn = line.get('pn', None)
+            mpn = line.get('mpn', None)
+            spn = line.get('spn', None)
             quantity = line.get('qty', None)
             unit = line.get('unit', None)
 
             try:
                 quantity = float(quantity)
             except (TypeError, ValueError):
                 self.add_error(f"Invalid quantity for line: {line}")
                 continue
 
             sub_part = self.match_part(line)
 
+            # Add line to internally stored BOM data
+            self.bom_lines.append({
+                'idx': len(self.bom_lines) + 1,
+                'description': description,
+                'designators': ', '.join(designators),
+                'quantity': quantity,
+                'unit': unit,
+                'sub_part': sub_part.pk if sub_part else None,
+                'pn': pn,
+                'mpn': mpn,
+                'spn': spn,
+            })
+
             if not sub_part:
-                self.add_warning(f"No matching part for line: {description}")
+                # No matching part can be found
                 continue
 
             if sub_part == self.part:
                 self.add_error(f"Part {sub_part} is the same as the parent part")
                 continue
 
+            # Check that it is a *valid* option for the BOM
+            if not sub_part.check_add_to_bom(self.part):
+                self.add_error(f"Part {sub_part} is not a valid option for the BOM")
+                continue
+
             # Associate the internal part with the designators
             for designator in designators:
                 self.part_map[designator] = sub_part
 
             if unit or sub_part.units:
                 quantity = self.convert_quantity(quantity, unit, sub_part.units)
 
@@ -356,14 +433,17 @@
             self.bom_items.append(BomItem(
                 part=self.part,
                 sub_part=sub_part,
                 quantity=quantity,
                 reference=' '.join(designators),
                 note="Wireviz BOM item"
             ))
+        
+        # Write BOM data to database
+        self.save_bom_data()
 
     def save_bom_data(self):
         """Write the extracted BOM data to the database."""
 
         if not self.get_setting('EXTRACT_BOM'):
             return
         
@@ -444,101 +524,45 @@
             if results.count() == 1:
                 return results.first()
         
             # Match wire_pn -> part.name
             results = Part.objects.filter(name=wire_pn)
             if results.count() == 1:
                 return results.first()
-    
-    def create_or_overwrite_attachment(self, fn, data, comment='Wireviz attachment'):
-        """Create a new attachment, or overwrite an existing attachment.
-        
-        - Check for an existing attachment with the same filename
-        - If it exists, overwrite the data
-        - If it does not exist, create a new attachment
-        """
 
-        for attachment in self.part.attachments.all():
-            if os.path.basename(attachment.attachment.name) == fn:
-                logger.info(f"WirevizPlugin: Overwriting existing attachment {fn}")
-
-                if len(data) == 0:
-                    attachment.delete()
-                    return
+    def generate_svg_output(self, harness: Harness, filename: str):
+        """Generate SVG output from a wireviz harness."""
 
-                filename = os.path.join(settings.MEDIA_ROOT, attachment.attachment.name)
+        logger.info("WirevizPlugin: Generating SVG output for wireviz harness")
 
-                with open(filename, 'wb') as fo:
-                    fo.write(data)
-                
-                return
-
-        if len(data) == 0:
-            # Ignore empty file data
-            return
+        graph = harness.create_graph()
+        svg_data = graph.pipe(format='svg')
 
-        # No existing attachment found, create a new one
-        PartAttachment.objects.create(
+        return PartAttachment.objects.create(
             part=self.part,
             attachment=ContentFile(
-                data,
-                name=fn,
+                svg_data.decode('utf-8'),
+                name='wireviz_harness.svg',
             ),
-            comment=comment,
+            comment=f"Wireviz Harness (autogenerated from {filename})",
             user=None
         )
 
-    def generate_html_output(self, harness: Harness):
-        """Generate HTML output from a wireviz harness."""
-
-        logger.info("WirevizPlugin: Generating HTML output for wireviz harness")
-
-        bomlist = bom_list(harness.bom())
-
-        # For now, we must write to a tempfile
-        # In the future, work out how to write to an in-memory file object
-        out_file = os.path.join(tempfile.gettempdir(), 'harness_out')
-        
-        harness.output(filename=out_file, fmt=('svg',), view=False)
-        generate_html_output(out_file, bomlist, harness.metadata, harness.options)
-
-        # Read the data back in
-        with open(out_file + '.html', 'r') as f:
-            html_data = f.read()
-        
-        self.create_or_overwrite_attachment(
-            self.HARNESS_HTML_FILE,
-            html_data.encode(),
-            comment='Wireviz Harness (autogenerated from .wireviz file)'
-        )
-
     def add_error(self, msg: str):
         """Add an error message to the list of errors."""
 
         self.errors.append(msg)
         logger.error(f"WireViz: {msg}")
 
     def add_warning(self, msg: str):
         """Add a warning message to the list of errors."""
 
         self.warnings.append(msg)
         logger.warning(f"WireViz: {msg}")
 
-    def save_error_file(self):
-        """Save an error file containing all error messages"""
-
-        data = '\n'.join(self.errors).encode()
-        self.create_or_overwrite_attachment(self.ERROR_MSG_FILE, data, comment='Wireviz error messages')
-    
-    def save_warning_file(self):
-        """Save a warning file containing all warning messages"""
-
-        data = '\n'.join(self.warnings).encode()
-        self.create_or_overwrite_attachment(self.WARNING_MSG_FILE, data, comment='Wireviz warning messages')
-
     def convert_quantity(self, quantity, unit, base_unit):
         """Convert a provided physical quantity into the "base units" of the part.
         
         Args:
             quantity: The quantity to convert
             unit: The unit of the quantity
             base_unit: The base unit of the part
```

### Comparing `inventree-wireviz-plugin-0.3.3/inventree_wireviz_plugin.egg-info/SOURCES.txt` & `inventree-wireviz-plugin-0.4.0/inventree_wireviz_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inventree-wireviz-plugin-0.3.3/setup.py` & `inventree-wireviz-plugin-0.4.0/setup.py`

 * *Files identical despite different names*

