# Comparing `tmp/cipher_parse-0.5.0a3.tar.gz` & `tmp/cipher_parse-0.5.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipher_parse-0.5.0a3.tar", max compression
+gzip compressed data, was "cipher_parse-0.5.1a0.tar", max compression
```

## Comparing `cipher_parse-0.5.0a3.tar` & `cipher_parse-0.5.1a0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1066 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/LICENSE
--rw-r--r--   0        0        0      807 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/README.md
--rw-r--r--   0        0        0      280 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/__init__.py
--rw-r--r--   0        0        0       24 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/_version.py
--rw-r--r--   0        0        0    28011 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/cipher_input.py
--rw-r--r--   0        0        0    35818 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/cipher_output.py
--rw-r--r--   0        0        0      384 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/derived_outputs.py
--rw-r--r--   0        0        0    11603 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/discrete_voronoi.py
--rw-r--r--   0        0        0      603 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/errors.py
--rw-r--r--   0        0        0        0 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/example_data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 13:00:57.311619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/__init__.py
--rw-r--r--   0        0        0   807612 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d
--rw-r--r--   0        0        0    19811 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json
--rw-r--r--   0        0        0     2154 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf
--rw-r--r--   0        0        0        0 2023-05-15 13:00:57.315619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/__init__.py
--rw-r--r--   0        0        0 10104120 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d
--rw-r--r--   0        0        0    19811 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json
--rw-r--r--   0        0        0     2160 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf
--rw-r--r--   0        0        0    47897 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/geometry.py
--rw-r--r--   0        0        0     5726 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/interface.py
--rw-r--r--   0        0        0     9770 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/material.py
--rw-r--r--   0        0        0     7286 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/quats.py
--rw-r--r--   0        0        0    20946 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/utilities.py
--rw-r--r--   0        0        0    12404 2023-05-15 13:00:57.339619 cipher_parse-0.5.0a3/cipher_parse/voxel_map.py
--rw-r--r--   0        0        0     1612 2023-05-15 13:00:57.343619 cipher_parse-0.5.0a3/pyproject.toml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 cipher_parse-0.5.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/LICENSE
+-rw-r--r--   0        0        0      807 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/README.md
+-rw-r--r--   0        0        0      280 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/_version.py
+-rw-r--r--   0        0        0    28011 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/cipher_input.py
+-rw-r--r--   0        0        0    36114 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/cipher_output.py
+-rw-r--r--   0        0        0      384 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/derived_outputs.py
+-rw-r--r--   0        0        0    11603 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/discrete_voronoi.py
+-rw-r--r--   0        0        0      603 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/errors.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/example_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/__init__.py
+-rw-r--r--   0        0        0   807612 2023-06-01 12:37:35.722376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d
+-rw-r--r--   0        0        0    19811 2023-06-01 12:37:35.726376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json
+-rw-r--r--   0        0        0     2154 2023-06-01 12:37:35.726376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf
+-rw-r--r--   0        0        0        0 2023-06-01 12:37:35.726376 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/__init__.py
+-rw-r--r--   0        0        0 10104120 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d
+-rw-r--r--   0        0        0    19811 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json
+-rw-r--r--   0        0        0     2160 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf
+-rw-r--r--   0        0        0    47897 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/geometry.py
+-rw-r--r--   0        0        0     5726 2023-06-01 12:37:35.750377 cipher_parse-0.5.1a0/cipher_parse/interface.py
+-rw-r--r--   0        0        0     9770 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/material.py
+-rw-r--r--   0        0        0     7286 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/quats.py
+-rw-r--r--   0        0        0    20955 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/utilities.py
+-rw-r--r--   0        0        0    12404 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/cipher_parse/voxel_map.py
+-rw-r--r--   0        0        0     1612 2023-06-01 12:37:35.754377 cipher_parse-0.5.1a0/pyproject.toml
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 cipher_parse-0.5.1a0/PKG-INFO
```

### Comparing `cipher_parse-0.5.0a3/LICENSE` & `cipher_parse-0.5.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/README.md` & `cipher_parse-0.5.1a0/README.md`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/cipher_input.py` & `cipher_parse-0.5.1a0/cipher_parse/cipher_input.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/cipher_output.py` & `cipher_parse-0.5.1a0/cipher_parse/cipher_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,23 +273,30 @@
         )
         vti_file_list = sorted(
             list(self.directory.glob(f"{outfile_base}_*.vti")),
             key=lambda x: int(re.search(r"\d+", x.name).group()),
         )
 
         # Move all VTU files to a sub-directory:
-        viz_dir = Path("original_viz")
-        viz_dir.mkdir()
+        viz_dir = self.directory / "original_viz"
+        
         vtu_orig_file_list = []
-        for viz_file_i in vtu_file_list:
-            dst_i = viz_dir.joinpath(viz_file_i.name).with_suffix(
-                ".viz" + viz_file_i.suffix
-            )
-            shutil.move(viz_file_i, dst_i)
-            vtu_orig_file_list.append(dst_i)
+        if not viz_dir.is_dir():
+            viz_dir.mkdir()
+            for viz_file_i in vtu_file_list:
+                dst_i = viz_dir.joinpath(viz_file_i.name).with_suffix(
+                    ".viz" + viz_file_i.suffix
+                )
+                shutil.move(viz_file_i, dst_i)
+                vtu_orig_file_list.append(dst_i)
+        else:
+            vtu_orig_file_list = sorted(
+            list(viz_dir.glob("*")),
+            key=lambda x: int(re.search(r"\d+", x.name).group()),
+        )
 
         # Copy back to the root directory VTU files that we want to keep:
         if self.options["num_VTU_files"]:
             viz_files_keep_idx = get_subset_indices(
                 len(vti_file_list),
                 self.options["num_VTU_files"],
             )
@@ -298,15 +305,15 @@
                 time_interval=self.options["VTU_files_time_interval"]
             )
         else:
             viz_files_keep_idx = []
 
         for i in viz_files_keep_idx:
             viz_file_i = vtu_orig_file_list[i]
-            dst_i = Path("").joinpath(viz_file_i.name).with_suffix("").with_suffix(".vtu")
+            dst_i = self.directory.joinpath(viz_file_i.name).with_suffix("").with_suffix(".vtu")
             shutil.copy(viz_file_i, dst_i)
 
         if self.options["delete_VTUs"]:
             print(f"Deleting original VTU files in directory: {viz_dir}")
             shutil.rmtree(viz_dir)
 
         # get which files to include for each output/derived output
@@ -338,15 +345,15 @@
 
             standard_outputs = {}
             for name in output_lookup:
                 arr_flat = mesh.get_array(output_lookup[name])
                 arr = arr_flat.reshape(mesh.dimensions, order="F")
                 if name in STANDARD_OUTPUTS_TYPES:
                     arr = arr.astype(STANDARD_OUTPUTS_TYPES[name])
-                standard_outputs[name] = arr
+                standard_outputs[name] = np.array(arr) # convert from pyvista_ndarray
 
             derived_outputs = {}
             for derive_out_i in self.options["derive_outputs"]:
                 name_i = derive_out_i["name"]
                 func = DERIVED_OUTPUTS_FUNCS[name_i]
                 func_args = {"cipher_input": cipher_input}
                 func_args.update(
```

### Comparing `cipher_parse-0.5.0a3/cipher_parse/discrete_voronoi.py` & `cipher_parse-0.5.1a0/cipher_parse/discrete_voronoi.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/errors.py` & `cipher_parse-0.5.1a0/cipher_parse/errors.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d` & `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json` & `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.json`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf` & `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/2D/synthetic_d3d.xdmf`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d` & `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json` & `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.json`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf` & `cipher_parse-0.5.1a0/cipher_parse/example_data/dream3d/3D/synthetic_d3d.xdmf`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/geometry.py` & `cipher_parse-0.5.1a0/cipher_parse/geometry.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/interface.py` & `cipher_parse-0.5.1a0/cipher_parse/interface.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/material.py` & `cipher_parse-0.5.1a0/cipher_parse/material.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/quats.py` & `cipher_parse-0.5.1a0/cipher_parse/quats.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/cipher_parse/utilities.py` & `cipher_parse-0.5.1a0/cipher_parse/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,15 +534,15 @@
 def get_time_linear_subset_indices(time_interval, max_time, times):
     intervals = np.linspace(
         0,
         max_time,
         num=int(((max_time + time_interval) / time_interval)),
         endpoint=True,
     )
-    return list(set(np.argmin(np.abs(times - intervals[:, None]), axis=1)))
+    return list(set(np.argmin(np.abs(times - intervals[:, None]), axis=1).tolist()))
 
 
 def sample_from_orientations_gradient(phase_centroids, max_misorientation_deg):
     """Generate an orientation gradient where orientations rotate uniformly according to a
     phase_centroids coordinate."""
 
     coords = phase_centroids[:, 0]
```

### Comparing `cipher_parse-0.5.0a3/cipher_parse/voxel_map.py` & `cipher_parse-0.5.1a0/cipher_parse/voxel_map.py`

 * *Files identical despite different names*

### Comparing `cipher_parse-0.5.0a3/pyproject.toml` & `cipher_parse-0.5.1a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cipher-parse"
-version = "0.5.0a3"
+version = "0.5.1a0"
 description = "Pre- and post-processing for the phase-field code CIPHER."
 authors = ["aplowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "cipher_parse/example_data/dream3d/2D/synthetic_d3d.dream3d",
     "cipher_parse/example_data/dream3d/3D/synthetic_d3d.dream3d",
@@ -45,15 +45,15 @@
 [tool.poetry.extras]
 hickle = ["hickle"]
 matflow = ["hickle", "matflow", "sqlalchemy"]
 notebook = ["notebook"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0a3"
+version = "0.5.1a0"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "cipher_parse/_version.py"
 ]
 bump_message = "bump: $current_version → $new_version [skip ci]"
```

### Comparing `cipher_parse-0.5.0a3/PKG-INFO` & `cipher_parse-0.5.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipher-parse
-Version: 0.5.0a3
+Version: 0.5.1a0
 Summary: Pre- and post-processing for the phase-field code CIPHER.
 License: MIT
 Author: aplowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

