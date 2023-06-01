# Comparing `tmp/SecuriPy-1.0.7.tar.gz` & `tmp/SecuriPy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.0.7.tar", last modified: Tue May 30 08:04:14 2023, max compression
+gzip compressed data, was "SecuriPy-1.0.8.tar", last modified: Thu Jun  1 16:37:35 2023, max compression
```

## Comparing `SecuriPy-1.0.7.tar` & `SecuriPy-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 08:04:14.599531 SecuriPy-1.0.7/
--rw-rw-rw-   0        0        0     3594 2023-05-30 08:04:14.598202 SecuriPy-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 08:04:14.596208 SecuriPy-1.0.7/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3594 2023-05-30 08:04:14.000000 SecuriPy-1.0.7/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-05-30 08:04:14.000000 SecuriPy-1.0.7/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 08:04:14.000000 SecuriPy-1.0.7/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 08:04:14.000000 SecuriPy-1.0.7/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4685 2023-05-30 08:03:39.000000 SecuriPy-1.0.7/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 08:04:14.599531 SecuriPy-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-05-30 08:03:57.000000 SecuriPy-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:37:35.182075 SecuriPy-1.0.8/
+-rw-rw-rw-   0        0        0     3594 2023-06-01 16:37:35.179055 SecuriPy-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 16:37:35.176100 SecuriPy-1.0.8/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3594 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 16:37:34.000000 SecuriPy-1.0.8/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5163 2023-06-01 16:36:46.000000 SecuriPy-1.0.8/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 16:37:35.182075 SecuriPy-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-06-01 16:37:09.000000 SecuriPy-1.0.8/setup.py
```

### Comparing `SecuriPy-1.0.7/PKG-INFO` & `SecuriPy-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.7/README.md` & `SecuriPy-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.0.7/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.0.8/SecuriPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.0.7
+Version: 1.0.8
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.0.7/SecuriPy.py` & `SecuriPy-1.0.8/SecuriPy.py`

 * *Files 15% similar despite different names*

```diff
@@ -115,7 +115,29 @@
         decrypted_data = decrypt_data(encrypted_data, encryption_key)
 
         # Save the decrypted image as a new image
         # Replace 'path/to/your/decrypted_image.jpg' with the desired path for the decrypted image
         decrypted_image_path = encrypted_image_path
         with open(decrypted_image_path, 'wb') as f:
             f.write(decrypted_data)
+
+    @staticmethod
+    def EncryptAll():
+        import os
+        images = os.listdir()
+
+        for image in images:
+            try:
+                Image.Encrypt(image)
+            except:
+                pass
+
+    @staticmethod
+    def DecryptAll():
+            import os
+            images = os.listdir()
+
+            for image in images:
+                try:
+                    Image.Decrypt(image)
+                except:
+                    pass
```

### Comparing `SecuriPy-1.0.7/setup.py` & `SecuriPy-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.0.7",
+    version="1.0.8",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

