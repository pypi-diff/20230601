# Comparing `tmp/looqbox_components-1.3.2-py3-none-any.whl.zip` & `tmp/looqbox_components-1.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 8694 bytes, number of entries: 14
+Zip file size: 9918 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      231 b- defN 23-May-03 16:35 looqbox_components/__init__.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 18:07 looqbox_components/templates/__init__.py
--rw-r--r--  2.0 unx     6858 b- defN 23-Apr-28 18:07 looqbox_components/templates/container.py
--rw-r--r--  2.0 unx     2350 b- defN 23-Apr-28 18:07 looqbox_components/templates/simple_card.py
+-rw-r--r--  2.0 unx     7156 b- defN 23-May-16 13:35 looqbox_components/templates/container.py
+-rw-r--r--  2.0 unx     2688 b- defN 23-May-16 13:35 looqbox_components/templates/simple_card.py
 -rw-r--r--  2.0 unx     5683 b- defN 23-Apr-28 18:07 looqbox_components/templates/tag.py
 -rw-r--r--  2.0 unx     2840 b- defN 23-Apr-28 18:07 looqbox_components/templates/toplist.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/templates/tests/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 23-May-16 13:35 looqbox_components/templates/tests/test_simple_card.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/tests/__init__.py
 -rw-r--r--  2.0 unx      233 b- defN 23-Apr-28 18:07 looqbox_components/tests/test_looqbox_components.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 18:07 looqbox_components/utils/__init__.py
--rw-r--r--  2.0 unx      989 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1294 b- defN 23-May-03 16:36 looqbox_components-1.3.2.dist-info/RECORD
-14 files, 20590 bytes uncompressed, 6470 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx      775 b- defN 23-May-16 13:35 looqbox_components/utils/parent_parameters.py
+-rw-r--r--  2.0 unx      989 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1505 b- defN 23-Jun-01 18:09 looqbox_components-1.3.4.dist-info/RECORD
+16 files, 22803 bytes uncompressed, 7344 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -15,29 +15,35 @@
 
 Filename: looqbox_components/templates/toplist.py
 Comment: 
 
 Filename: looqbox_components/templates/tests/__init__.py
 Comment: 
 
+Filename: looqbox_components/templates/tests/test_simple_card.py
+Comment: 
+
 Filename: looqbox_components/tests/__init__.py
 Comment: 
 
 Filename: looqbox_components/tests/test_looqbox_components.py
 Comment: 
 
 Filename: looqbox_components/utils/__init__.py
 Comment: 
 
-Filename: looqbox_components-1.3.2.dist-info/METADATA
+Filename: looqbox_components/utils/parent_parameters.py
+Comment: 
+
+Filename: looqbox_components-1.3.4.dist-info/METADATA
 Comment: 
 
-Filename: looqbox_components-1.3.2.dist-info/WHEEL
+Filename: looqbox_components-1.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: looqbox_components-1.3.2.dist-info/top_level.txt
+Filename: looqbox_components-1.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: looqbox_components-1.3.2.dist-info/RECORD
+Filename: looqbox_components-1.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## looqbox_components/templates/container.py

```diff
@@ -79,19 +79,28 @@
         ]
         self._tooltip_style = [
             Css.Position("absolute"),
             Css.Right(self.properties.get("tooltip-spacing", "5px")),
             Css.Width(self.properties.get("tooltip-size", "15px")),
             Css.Height(self.properties.get("tooltip-size", "15px"))
         ]
+        self.parent_properties = self._get_parent_properties(self.properties)
+        vars(self).update(self.parent_properties)
+
+    def _get_parent_properties(self, properties):
+        return {property_name: property_value for property_name, property_value in properties.items()
+                if property_name not in self.obj_container_args}
 
     def _get_container(self) -> ObjRow:
         content = self._get_content()
-        extra_properties = {looq_object_property: property_value for looq_object_property, property_value in
-                            vars(self).items() if looq_object_property in self.abs_container_args}
+        extra_properties = {
+            prop: value
+            for prop, value in vars(self).items()
+            if prop in self.abs_container_args
+        }
         return ObjRow(content, css_options=[Css.Padding("5px")], **extra_properties)
 
     def _get_content(self) -> ObjRow:
 
         _header = self._get_header()
         _is_single_container = self.is_single_switch(self.content)
```

## looqbox_components/templates/simple_card.py

```diff
@@ -1,64 +1,70 @@
 from typing import Union
 
 from looqbox import ObjText, ObjRow, ObjColumn
-from looqbox.objects.looq_object import LooqObject
+from looqbox.objects.container.positional.abstract_positional_container import AbstractPositionalContainer
 from looqbox.render.abstract_render import BaseRender
 
 from looqbox_components.templates.container import Container
 from looqbox_components.templates.tag import Tag
+from looqbox_components.utils.parent_parameters import include_extra_parent_params
 
 
-class SimpleCard(LooqObject):
+class SimpleCard(AbstractPositionalContainer):
     """
     Create and render a simple card template.
 
     :return: A JSON string.
 
     """
 
     def __init__(self, title: Union[ObjText, str], value: Union[ObjText, float, int],
                  tag_value: Union[int, float] = None, tooltip: str = None, line: bool = False,
-                 line_color: str = "#40db62", **tag_properties) -> None:
+                 line_color: str = "#40db62", tag_properties=None, children=None, **parent_params) -> None:
         """
         Default template for simple card
         :param title: str or lq.ObjText - title of the card
         :param value: lq.ObjText or int or float - value of the card
         :param tag_value: int or float - value of the tag in card
         :param tooltip: str - text to display in tooltip
         :param line: boolean - add a line on the left side of the card
         :param line_color: str - set color of the line
         :param tag_properties: properties for tag customization
         """
         super().__init__(value)
+
         self.title = title
         self.value = value
         self.tag_value = tag_value
         self.tooltip = tooltip
         self.line = line
         self.line_color = line_color
-        self.tag_properties = tag_properties
+        self.tag_properties = tag_properties or {}
+        self.parent_params = parent_params
+        self.children = children or self.get_children()
 
+    @include_extra_parent_params
     def _build_card(self):
-        self.card = Container(
-            ObjRow(
-                *[ObjColumn(
-                    self.value,
-                    render_condition=self.value
-                ).set_main_alignment_center],
-                ObjRow(Tag(self.tag_value, tag_format="percent:1", **self.tag_properties),
-                       render_condition=self.tag_value).set_main_alignment_end
-            ).set_main_alignment_space_between.set_cross_alignment_center,
+        return Container(
+            self.children,
             title=self.title,
             tooltip=self.tooltip,
             line=self.line,
-            line_color=self.line_color
+            line_color=self.line_color,
+            **self.parent_params
         )
 
+    def get_children(self):
+        return ObjRow(
+            [ObjColumn(self.value, render_condition=self.value).set_main_alignment_center],
+            ObjRow(
+                Tag(self.tag_value, tag_format="percent:1", **self.tag_properties),
+                render_condition=self.tag_value).set_main_alignment_end
+        ).set_main_alignment_space_between.set_cross_alignment_center
+
     def _set_value_as_text(self):
         if not isinstance(self.value, ObjText):
             self.value = ObjText(self.value)
 
     def to_json_structure(self, visitor: BaseRender):
         self._set_value_as_text()
-        self._build_card()
-        return self.card.to_json_structure(visitor)
+        return self._build_card().to_json_structure(visitor)
```

## Comparing `looqbox_components-1.3.2.dist-info/METADATA` & `looqbox_components-1.3.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looqbox-components
-Version: 1.3.2
+Version: 1.3.4
 Summary: A looqbox package with most used visual components templates
 Home-page: https://github.com/looqbox/python-visual-components
 Author: Looqbox
 Author-email: admin@looqbox.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `looqbox_components-1.3.2.dist-info/RECORD` & `looqbox_components-1.3.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 looqbox_components/__init__.py,sha256=t-xfKsHcJ7n8NfeWb6JLRJeBgdPD86Aqm_nQid_fZxw,231
 looqbox_components/templates/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-looqbox_components/templates/container.py,sha256=vsjreTp40yse1YmdrT3LCO_g2waadDY-dQ7m08HYLh4,6858
-looqbox_components/templates/simple_card.py,sha256=wfL-cG3hWQqDb4ETg_I9tl5PglDJE9hcBajKiqd8590,2350
+looqbox_components/templates/container.py,sha256=QFClUUkX2GtwiT8MmIPJQmSrfZBg3PRnWM01BQodMfw,7156
+looqbox_components/templates/simple_card.py,sha256=yqYXcZMaNt1BwtPOGvulOwgMLH2ox-5nqr0roa6kH7o,2688
 looqbox_components/templates/tag.py,sha256=EciZ3VRCIdloOUTC68hF7FHL-_9xtQ2TVi1K60oAKDw,5683
 looqbox_components/templates/toplist.py,sha256=mAlFkUBYXMMqSSIz5MogMascE1OfzVoT5sfGfFiuC5Y,2840
 looqbox_components/templates/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+looqbox_components/templates/tests/test_simple_card.py,sha256=p7axi8j3Fqs5Ka_GSSDM7JImPZaH-xpDc4ZmBYCdupU,591
 looqbox_components/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 looqbox_components/tests/test_looqbox_components.py,sha256=8fVRfEvqcxlJDuNp6RlucKwH13JMCrXkeGgSmkdxonU,233
 looqbox_components/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-looqbox_components-1.3.2.dist-info/METADATA,sha256=go2xZEdxyqwkaE9EfDqB2z_LBvmk-xxzix1LlpHtlkQ,989
-looqbox_components-1.3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-looqbox_components-1.3.2.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
-looqbox_components-1.3.2.dist-info/RECORD,,
+looqbox_components/utils/parent_parameters.py,sha256=SEgVvejN3PqjcSkKJztrYykjo-m626BY0s1WvpGEmOs,775
+looqbox_components-1.3.4.dist-info/METADATA,sha256=K6_Y_Sr6Y0o8PsXWpdDE_w2VyEjM4OiS80Ru0Els9f0,989
+looqbox_components-1.3.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+looqbox_components-1.3.4.dist-info/top_level.txt,sha256=Zb_QlF8DlA-rP1wb-5-vbk_U_exlVnC4IXl1bBro5kQ,19
+looqbox_components-1.3.4.dist-info/RECORD,,
```

