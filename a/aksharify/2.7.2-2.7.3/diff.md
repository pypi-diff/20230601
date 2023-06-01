# Comparing `tmp/aksharify-2.7.2.tar.gz` & `tmp/aksharify-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.7.2.tar", max compression
+gzip compressed data, was "aksharify-2.7.3.tar", max compression
```

## Comparing `aksharify-2.7.2.tar` & `aksharify-2.7.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.7.2/aksharify/__init__.py
--rw-r--r--   0        0        0     7234 2023-05-30 14:05:22.226629 aksharify-2.7.2/aksharify/aksharify.py
--rw-r--r--   0        0        0      901 2023-05-30 14:33:38.944602 aksharify-2.7.2/pyproject.toml
--rw-r--r--   0        0        0     5864 2023-05-30 14:27:02.119233 aksharify-2.7.2/README.md
--rw-r--r--   0        0        0     6619 1970-01-01 00:00:00.000000 aksharify-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.7.3/aksharify/__init__.py
+-rw-r--r--   0        0        0     7763 2023-06-01 02:42:15.057908 aksharify-2.7.3/aksharify/aksharify.py
+-rw-r--r--   0        0        0      923 2023-06-01 02:46:42.208155 aksharify-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5864 2023-05-30 14:27:02.119233 aksharify-2.7.3/README.md
+-rw-r--r--   0        0        0     6661 1970-01-01 00:00:00.000000 aksharify-2.7.3/PKG-INFO
```

### Comparing `aksharify-2.7.2/aksharify/aksharify.py` & `aksharify-2.7.3/aksharify/aksharify.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,21 @@
 class AksharArt:
     
     def __init__(self, image, chars="01") -> None:
         self.image = Image.open(image)
         self.w, self.h = self.image.size
         self.chars = list(set(chars))
         self.CH_CONSTANT = 2.143
-        self.H_dis, self.V_dis = 11.1, 20
-        self.font_size = 20
+        self.H_dis, self.V_dis = 5.55, 10
+        self.font_size = 10
+    
+    def set_font_size(self, size):
+        self.H_dis = (size*555)/1000
+        self.V_dis = size
+        self.font_size = size
 
     def set_dim(self, width=None, height=None):
         if width != None and height == None:
             self.w, self.h = width, int(
                 (self.h/self.w * width)/self.CH_CONSTANT)
         elif width == None and height != None:
             self.w, self.h = int((self.w/self.h * height)
@@ -77,29 +82,36 @@
             
     def span(self, integer, integer_colour):
         return f"<span style='color: rgb{integer_colour};'><b>{integer}</b></span>"
 
     def tspan(self, char, char_color, x):
         return f'<tspan x="{x}" fill="{char_color}">{char}</tspan>'
     
+    def btspan(self, char, char_color, x):
+        return f'<tspan x="{x}" fill="{char_color}" font-weight="bold">{char}</tspan>'
+    
     def rgb2hex(self, rgba):
         return '#{:02x}{:02x}{:02x}'.format(rgba[0], rgba[1], rgba[2])
 
-    def svgify(self, bg_color="None"):
+    def svgify(self, bg_color="None", bold=False):
         file = SVG_HEADER.format(
             int(self.w*self.H_dis)+41, 
             int(self.h*self.V_dis)+41,
             "monospace", self.font_size, bg_color
             )
         file += f'<a href="https://primepatel.github.io/aksharify-docs/">'
         x, y = 20, 30
+        if bold == False:
+            char_func = self.tspan
+        else:
+            char_func = self.btspan
         for line_no in range(self.h):
             file += f'<text x="{x}" y="{y}">'
             for char_no in range(self.w):
-                file += self.tspan(
+                file += char_func(
                     self.matrix[line_no][char_no],
                     self.rgb2hex(self.image.getpixel((char_no, line_no))), x
                     )
                 x += self.H_dis
             file += '</text>'
             x = 20
             y += self.V_dis
@@ -139,14 +151,19 @@
             svg2png(bytestring=self.ascii_svg,write_to=fname+'.png',output_height=height,output_width=width)
 
 
 class EmojiArt(AksharArt):
     def __init__(self, image, chars="🙂😅") -> None:
         super().__init__(image, chars)
         self.H_dis = 20
+    
+    def set_font_size(self, size):
+        self.H_dis = size
+        self.V_dis = size
+        self.font_size = size
 
 class TextArt(AksharArt):
     
     def __init__(self, image, chars=SORTEDCHARS, ordered=False) -> None:
         super().__init__(image)
         self.chars = list(set(chars))
         if not ordered:
```

### Comparing `aksharify-2.7.2/pyproject.toml` & `aksharify-2.7.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2261 6b73 6861 7269 6679  ame = "aksharify
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 322e  "..version = "2.
-00000030: 372e 3222 0d0a 6465 7363 7269 7074 696f  7.2"..descriptio
+00000030: 372e 3322 0d0a 6465 7363 7269 7074 696f  7.3"..descriptio
 00000040: 6e20 3d20 2250 7974 686f 6e20 4173 6369  n = "Python Asci
 00000050: 6920 2b20 456d 6f6a 6920 4172 7420 4d6f  i + Emoji Art Mo
 00000060: 6475 6c65 220d 0a61 7574 686f 7273 203d  dule"..authors =
 00000070: 205b 2250 7269 6d65 2050 6174 656c 203c   ["Prime Patel <
 00000080: 7072 696d 6573 7061 7465 6c40 676d 6169  primespatel@gmai
 00000090: 6c2e 636f 6d3e 225d 0d0a 6c69 6365 6e73  l.com>"]..licens
 000000a0: 6520 3d20 224d 4954 220d 0a72 6561 646d  e = "MIT"..readm
@@ -44,14 +44,15 @@
 000002b0: 0a20 2020 2020 2020 2022 4f70 6572 6174  .        "Operat
 000002c0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
 000002d0: 2049 6e64 6570 656e 6465 6e74 222c 0d0a   Independent",..
 000002e0: 2020 2020 5d0d 0a0d 0a5b 746f 6f6c 2e70      ]....[tool.p
 000002f0: 6f65 7472 792e 6465 7065 6e64 656e 6369  oetry.dependenci
 00000300: 6573 5d0d 0a70 7974 686f 6e20 3d20 225e  es]..python = "^
 00000310: 332e 3130 220d 0a70 696c 6c6f 7720 3d20  3.10"..pillow = 
-00000320: 225e 392e 352e 3022 0d0a 0d0a 0d0a 5b62  "^9.5.0"......[b
-00000330: 7569 6c64 2d73 7973 7465 6d5d 0d0a 7265  uild-system]..re
-00000340: 7175 6972 6573 203d 205b 2270 6f65 7472  quires = ["poetr
-00000350: 792d 636f 7265 225d 0d0a 6275 696c 642d  y-core"]..build-
-00000360: 6261 636b 656e 6420 3d20 2270 6f65 7472  backend = "poetr
-00000370: 792e 636f 7265 2e6d 6173 6f6e 7279 2e61  y.core.masonry.a
-00000380: 7069 220d 0a                             pi"..
+00000320: 225e 392e 352e 3022 0d0a 7265 7175 6573  "^9.5.0"..reques
+00000330: 7473 203d 2022 5e32 2e33 312e 3022 0d0a  ts = "^2.31.0"..
+00000340: 0d0a 0d0a 5b62 7569 6c64 2d73 7973 7465  ....[build-syste
+00000350: 6d5d 0d0a 7265 7175 6972 6573 203d 205b  m]..requires = [
+00000360: 2270 6f65 7472 792d 636f 7265 225d 0d0a  "poetry-core"]..
+00000370: 6275 696c 642d 6261 636b 656e 6420 3d20  build-backend = 
+00000380: 2270 6f65 7472 792e 636f 7265 2e6d 6173  "poetry.core.mas
+00000390: 6f6e 7279 2e61 7069 220d 0a              onry.api"..
```

### Comparing `aksharify-2.7.2/README.md` & `aksharify-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-2.7.2/PKG-INFO` & `aksharify-2.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 2.7.2
+Version: 2.7.3
 Summary: Python Ascii + Emoji Art Module
 Home-page: https://primepatel.github.io/aksharify-docs/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/primepatel/aksharify
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
 
 # __Aksharify__
```

