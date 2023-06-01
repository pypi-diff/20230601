# Comparing `tmp/imgmisc-0.2.1.tar.gz` & `tmp/imgmisc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgmisc-0.2.1.tar", last modified: Fri Feb 17 12:54:11 2023, max compression
+gzip compressed data, was "imgmisc-0.2.2.tar", last modified: Thu Jun  1 08:55:25 2023, max compression
```

## Comparing `imgmisc-0.2.1.tar` & `imgmisc-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-02-17 12:54:11.095127 imgmisc-0.2.1/
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      152 2020-05-13 19:31:22.000000 imgmisc-0.2.1/AUTHORS.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     3547 2020-05-13 19:31:22.000000 imgmisc-0.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       89 2020-05-13 19:31:22.000000 imgmisc-0.2.1/HISTORY.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1521 2020-05-13 19:31:22.000000 imgmisc-0.2.1/LICENSE
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      262 2020-05-13 19:31:22.000000 imgmisc-0.2.1/MANIFEST.in
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1739 2023-02-17 12:54:11.095127 imgmisc-0.2.1/PKG-INFO
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      853 2020-05-13 19:31:22.000000 imgmisc-0.2.1/README.rst
-drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-02-17 12:54:11.095127 imgmisc-0.2.1/docs/
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      608 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/Makefile
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       28 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/authors.rst
--rwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)     4806 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/conf.py
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       33 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/contributing.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       28 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/history.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      304 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/index.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1138 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/installation.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      769 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/make.bat
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       27 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/readme.rst
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       69 2020-05-13 19:31:22.000000 imgmisc-0.2.1/docs/usage.rst
-drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-02-17 12:54:11.095127 imgmisc-0.2.1/imgmisc/
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      186 2023-02-17 12:53:49.000000 imgmisc-0.2.1/imgmisc/__init__.py
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)    65835 2023-02-16 21:42:29.000000 imgmisc-0.2.1/imgmisc/imgmisc.py
-drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-02-17 12:54:11.095127 imgmisc-0.2.1/imgmisc.egg-info/
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1739 2023-02-17 12:54:11.000000 imgmisc-0.2.1/imgmisc.egg-info/PKG-INFO
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      518 2023-02-17 12:54:11.000000 imgmisc-0.2.1/imgmisc.egg-info/SOURCES.txt
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)        1 2023-02-17 12:54:11.000000 imgmisc-0.2.1/imgmisc.egg-info/dependency_links.txt
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)        1 2023-02-17 12:54:11.000000 imgmisc-0.2.1/imgmisc.egg-info/not-zip-safe
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       11 2023-02-17 12:54:11.000000 imgmisc-0.2.1/imgmisc.egg-info/requires.txt
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)        8 2023-02-17 12:54:11.000000 imgmisc-0.2.1/imgmisc.egg-info/top_level.txt
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      390 2023-02-17 12:54:11.095127 imgmisc-0.2.1/setup.cfg
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1649 2023-02-17 12:53:49.000000 imgmisc-0.2.1/setup.py
-drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-02-17 12:54:11.095127 imgmisc-0.2.1/tests/
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       62 2020-05-13 19:31:22.000000 imgmisc-0.2.1/tests/__init__.py
--rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      876 2020-05-13 19:31:22.000000 imgmisc-0.2.1/tests/test_imgmisc.py
+drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-06-01 08:55:25.589605 imgmisc-0.2.2/
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      152 2020-05-13 19:31:22.000000 imgmisc-0.2.2/AUTHORS.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     3547 2020-05-13 19:31:22.000000 imgmisc-0.2.2/CONTRIBUTING.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       89 2020-05-13 19:31:22.000000 imgmisc-0.2.2/HISTORY.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1521 2020-05-13 19:31:22.000000 imgmisc-0.2.2/LICENSE
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      262 2020-05-13 19:31:22.000000 imgmisc-0.2.2/MANIFEST.in
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1739 2023-06-01 08:55:25.589605 imgmisc-0.2.2/PKG-INFO
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      853 2020-05-13 19:31:22.000000 imgmisc-0.2.2/README.rst
+drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-06-01 08:55:25.581601 imgmisc-0.2.2/docs/
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      608 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/Makefile
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       28 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/authors.rst
+-rwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)     4806 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/conf.py
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       33 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/contributing.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       28 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/history.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      304 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/index.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1138 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/installation.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      769 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/make.bat
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       27 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/readme.rst
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       69 2020-05-13 19:31:22.000000 imgmisc-0.2.2/docs/usage.rst
+drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-06-01 08:55:25.585603 imgmisc-0.2.2/imgmisc/
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      186 2023-06-01 08:50:32.000000 imgmisc-0.2.2/imgmisc/__init__.py
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)    69367 2023-05-25 15:31:47.000000 imgmisc-0.2.2/imgmisc/imgmisc.py
+drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-06-01 08:55:25.589605 imgmisc-0.2.2/imgmisc.egg-info/
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1739 2023-06-01 08:55:25.000000 imgmisc-0.2.2/imgmisc.egg-info/PKG-INFO
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      518 2023-06-01 08:55:25.000000 imgmisc-0.2.2/imgmisc.egg-info/SOURCES.txt
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)        1 2023-06-01 08:55:25.000000 imgmisc-0.2.2/imgmisc.egg-info/dependency_links.txt
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)        1 2023-06-01 08:55:25.000000 imgmisc-0.2.2/imgmisc.egg-info/not-zip-safe
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       11 2023-06-01 08:55:25.000000 imgmisc-0.2.2/imgmisc.egg-info/requires.txt
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)        8 2023-06-01 08:55:25.000000 imgmisc-0.2.2/imgmisc.egg-info/top_level.txt
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      390 2023-06-01 08:55:25.589605 imgmisc-0.2.2/setup.cfg
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)     1649 2023-06-01 08:50:32.000000 imgmisc-0.2.2/setup.py
+drwxrwxr-x   0 henrikahl  (1001) henrikahl  (1001)        0 2023-06-01 08:55:25.589605 imgmisc-0.2.2/tests/
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)       62 2020-05-13 19:31:22.000000 imgmisc-0.2.2/tests/__init__.py
+-rw-rw-r--   0 henrikahl  (1001) henrikahl  (1001)      876 2020-05-13 19:31:22.000000 imgmisc-0.2.2/tests/test_imgmisc.py
```

### Comparing `imgmisc-0.2.1/CONTRIBUTING.rst` & `imgmisc-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/LICENSE` & `imgmisc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/PKG-INFO` & `imgmisc-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgmisc
-Version: 0.2.1
+Version: 0.2.2
 Summary: imgmisc
 Home-page: https://github.com/supersubscript/imgmisc
 Author: Henrik Åhl
 Author-email: hpa22@cam.ac.uk
 License: GNU General Public License v3
 Keywords: imgmisc
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `imgmisc-0.2.1/README.rst` & `imgmisc-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/docs/Makefile` & `imgmisc-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/docs/conf.py` & `imgmisc-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/docs/installation.rst` & `imgmisc-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/docs/make.bat` & `imgmisc-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/imgmisc/imgmisc.py` & `imgmisc-0.2.2/imgmisc/imgmisc.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     mesh_surface_area,
     regionprops,
     regionprops_table,
 )
 from skimage.morphology import binary_dilation
 from skimage.transform import warp
 from sklearn.decomposition import PCA
+from scipy.ndimage import find_objects
 
+from tqdm import tqdm
 from loguru import logger
 
 def bname(x):
     """Return the basename of a string"""
     return os.path.basename(os.path.splitext(x)[0])
 
 
@@ -62,15 +64,27 @@
         img = tiff.imread(fname)
     except:
         try:
             import czifile as cz
 
             img = cz.czifile(fname)
         except:
-            raise Exception(f"Input file type for {fname} not supported.")
+            try:
+                import read_lif as lif
+                reader = lif.Reader(fname)
+                series = reader.getSeries()
+                chosen = series[0]
+                data = []
+                for nchan in range(len(chosen.getChannels())):
+                    image = chosen.getFrame(T=0, channel=nchan)
+                    data.append(image)
+                data = np.stack(data, axis=1)
+            except:
+                raise Exception(f'Input file type for {fname} not supported.')
+
     img = np.squeeze(img)
     if img.ndim < 3:
         raise Exception("Too few channels")
     if img.ndim == 4 and channel is not None:
         img = img[:, channel]
 
     return img
@@ -171,14 +185,87 @@
                 )
             ] = True
         return mask
 
     bordering = np.unique(seg_img[mask_borders(seg_img)])
     return bordering
 
+def lowmap(img, background=0, sort=True):
+    """
+    Generate a low-valued mapping of object labels such that two adjacent objects
+    will not have the same label. This simplifies visualisation.
+
+    Parameters
+    ----------
+    img : np.array
+        The input, segmented image.
+    background : int, optional
+        The background label. The default is 0.
+    sort : bool, optional
+        Whether to initiate labelling with the objects with the most neighbours.
+        Doing this may decrease the output range. The default is True.
+
+    Returns
+    -------
+    mapping : dict of {old_label:new_id} of type int/int.
+        The output mapping.
+
+    """
+    
+    # Get the cell neighbours
+    neighs = find_neighbors(img, background=0)
+    
+    # Sort based of neighbours
+    if sort:
+        neighs = sorted(neighs.items(), key=lambda x: len(x[1]), reverse=True)
+
+    # Compute mappings    
+    mapping = np.full(len(neighs), -1)#
+    for cell_id, cell_neighs in neighs:
+        arr = np.append(cell_id, cell_neighs)
+        labelled = mapping[arr-1] != -1
+        label = 1
+        while True:
+            if label not in mapping[arr[labelled] - 1]:
+                mapping[cell_id - 1] = label
+                break
+            label += 1
+    mapping = dict(zip([nn[0] for nn in neighs], mapping))
+    
+    return mapping
+
+def lowmap_img(img, background=0, sort=True):
+    """
+    Generate a low-valued mapping of object labels such that two adjacent objects
+    will not have the same label. This simplifies visualisation. 
+    
+    Return the transformed image.
+
+    Parameters
+    ----------
+    img : np.array
+        The input, segmented image.
+    background : int, optional
+        The background label. The default is 0.
+    sort : bool, optional
+        Whether to initiate labelling with the objects with the most neighbours.
+        Doing this may decrease the output range. The default is True.
+
+    Returns
+    -------
+    output : np.array
+        The input image with its labels mapped to the lower values.
+
+    """
+    
+    mapping = lowmap(img, background, sort)
+    output = map_replace(img, mapping)
+    
+    return output
+
 
 def get_bottom(seg_img, background=0, width=1):
     bottom = np.unique(seg_img[:width, :, :])
     bottom = bottom[bottom != background]
     return bottom
 
 
@@ -224,15 +311,14 @@
     elif weights.lower() in ["quad", "quadric", "quadratic"]:
         fct = lambda x: 1.0 / (1 + x) ** 2
     else:
         fct = lambda x: 1.0
 
     points = points.copy()
     for iter_ in range(iters):
-        # print(f'iter {ii}')
         tree = cKDTree(points)
         pts = tree.query_ball_tree(tree, r)
         pts = [pp for pp in pts]
         pts_coords = [points[pts[ii]] for ii in range(len(pts))]
         dists = [
             [((points[ii] - pc) ** 2).sum() ** 0.5 / r for pc in pts_coords[ii]]
             for ii in range(len(pts))
@@ -843,15 +929,15 @@
             flatness = []
         if "fractional_anisotropy" in properties:
             fractional_anisotropy = []
         if "ellipsoidity" in properties:
             ellipsoidity = []
 
         for iter_, rr in enumerate(rp_all):
-            print(iter_)
+            # print(iter_)
             mask = rr.image
             mask_padded = np.pad(np.atleast_3d(mask), pad_width=1, mode="constant")
             temp = distance_transform_edt(mask_padded, sampling=resolution)
             dt = extract_subsection(temp, shape=mask.shape)
 
             if "max_inscribed_sphere_radius" in properties:
                 max_inscribed_sphere_radius.append(dt.max())
@@ -937,16 +1023,16 @@
         regprops["flatness"] = flatness
     if "obbox_sides" in properties:
         regprops["obbox_side-0"] = obb_side_0
         regprops["obbox_side-1"] = obb_side_1
         regprops["obbox_side-2"] = obb_side_2
     if "ellipsoidity" in properties:
         regprops["ellipsoidity"] = ellipsoidity
-    if "fractional_anisitropy" in properties:
-        regprops["fractional_anisitropy"] = fractional_anisotropy
+    if "fractional_anisotropy" in properties:
+        regprops["fractional_anisotropy"] = fractional_anisotropy
     if "obbox_area" in properties:
         regprops["obbox_area"] = obbox_area
     if "obbox_volume" in properties:
         regprops["obbox_volume"] = obbox_area
     if "cuboidness" in properties:
         regprops["cuboidness"] = cuboidness
 
@@ -1029,17 +1115,15 @@
 def l1_cell_surface_areas(seg_img, resolution=[1, 1, 1], verbose=True):
     mesh = contour2mesh(seg_img, resolution=resolution, labeled=True)
     labels = np.unique(mesh["labels"])
     faces = mesh.faces.reshape((-1, 4))[:, 1:]
     faces_labels = mesh["labels"][faces]
 
     areas = []
-    for ii, label in enumerate(labels):
-        if verbose:
-            print(f"{ii} / {len(labels)} done...")
+    for ii, label in enumerate(tqdm(labels, disable=(not verbose))):
         subset = np.all(faces_labels == label, axis=1)
         area = mesh_surface_area(mesh.points, faces[subset])
         areas.append(area)
     return labels, areas
 
 
 def sphericity(bw, resolution=[1, 1, 1]):
@@ -1051,46 +1135,75 @@
     verts, faces, norms, vals = marching_cubes(volume=tmp, level=0, spacing=resolution)
 
     a_region = mesh_surface_area(verts, faces)
     sphericity = a_equiv / a_region
     return sphericity
 
 
-def create_cellular_mesh(seg_img, resolution=[1, 1, 1], verbose=True):
-    cells = []
-    n_cells = len(np.unique(seg_img)) - 1
-    for c_idx, cell_id in enumerate(np.unique(seg_img)[1:]):
-        if verbose:
-            print(f"Now meshing cell {c_idx} (label: {cell_id}) out of {n_cells}")
-        cell_img, cell_cuts = autocrop(
-            seg_img == cell_id,
-            threshold=0,
-            n=1,
-            return_cuts=True,
-            offset=[[2, 2], [2, 2], [2, 2]],
-        )
-        cell_volume = np.sum(cell_img > 0) * np.product(resolution)
+def create_cellular_mesh(seg_img, resolution=[1, 1, 1], background=0, verbose=True):
+    """
+    Create a cellular mesh from a segmented image.
+
+    Parameters
+    ----------
+    seg_img : np.array
+        The segmented image.
+    resolution : 3-tuple, optional
+        The spational resolution. The default is [1, 1, 1].
+    background : int, optional
+        The background label. The default is 0.
+    verbose : bool, optional
+        Whether to print the progress. The default is True.
+
+    Returns
+    -------
+    poly : pyvista.PolyData
+        The output cellular mesh.
+
+    """
+    
+    if background != 0:
+        raise NotImplementedError(
+            f'The background label is set as {background}. Currently, the background label has to be 0.')
+
+    labels = np.unique(seg_img)
+    labels = labels[labels != background]
+    
+    # poly = pv.PolyData()
+    all_v, all_f, all_cid, all_vols = [], [], [], []
+    slices = find_objects(seg_img)
+    for c_idx, cell_id in enumerate(tqdm(labels, disable=(not verbose))):
+            
+        # Extract the cell of interest and compute its faces and vertices
+        cell_slices = slices[c_idx]
+        cell_img = seg_img[cell_slices]
+        cell_img = np.pad(cell_img, 2)
+        cell_mask = cell_img == cell_id
 
         v, f, _, _ = marching_cubes(
-            cell_img, 0, allow_degenerate=False, step_size=1, spacing=resolution
+            cell_mask, .5, allow_degenerate=False, step_size=1, spacing=resolution
         )
-        v[:, 0] += cell_cuts[0, 0] * resolution[0]
-        v[:, 1] += cell_cuts[1, 0] * resolution[1]
-        v[:, 2] += cell_cuts[2, 0] * resolution[2]
-
-        cell_mesh = pv.PolyData(v, np.ravel(np.c_[[[3]] * len(f), f]))
-        cell_mesh["cell_id"] = np.full(fill_value=cell_id, shape=cell_mesh.n_points)
-        cell_mesh["volume"] = np.full(fill_value=cell_volume, shape=cell_mesh.n_points)
-
-        cells.append(cell_mesh)
-
-    multi = pv.MultiBlock(cells)
-    poly = pv.PolyData()
-    for ii in range(multi.n_blocks):
-        poly += multi.get(ii)
+        
+        # Set correct coordinates in global space and create cell mesh
+        for dim in range(3):
+            v[:, dim] += (cell_slices[dim].start - 2) * resolution[dim]
+        f = np.ravel(np.c_[[[3]] * len(f), f + len(all_v)]) 
+        all_v.extend(list(v))
+        all_f.extend(list(f))
+    
+        # Add volume and cell info
+        cell_volume = np.sum(cell_mask) * np.product(resolution)
+        all_cid.extend([cell_id] * len(v))
+        all_vols.extend([cell_volume] * len(v))
+
+    # Create final mesh
+    poly = pv.PolyData(np.array(all_v), np.array(all_f))        
+    poly['cell_id'] = all_cid
+    poly['volume'] = all_vols
+
     return poly
 
 
 def get_l1(seg_img, background=0, selem=None):
     # TODO: Include option to remove cells bordering the image limits?
     bg_dilated = np.logical_and(
         binary_dilation(seg_img == background, selem=selem), seg_img
@@ -1543,15 +1656,15 @@
 
 
 def listdir(
     path,
     include=None,
     exclude=None,
     full=True,
-    sorting=None,
+    sorting='natural',
     recursive=False,
     exclude_directories=True,
 ):
     if isinstance(path, (list, np.ndarray)):
         files = flatten(
             [listdir(ff, include, exclude, full, sorting, recursive) for ff in path]
         )
@@ -1591,15 +1704,17 @@
     if exclude_directories:
         files = [ff for ff in files if not os.path.isdir(ff)]
 
     if sorting == "natural":
         files = np.array(natural_sort(files))
     elif sorting == "alphabetical":
         files = np.sort(files)
-    elif sorting == True:
+    elif sorting == 'size':
+        files = np.array(sorted(files, key = lambda x: os.stat(x).st_size))
+    elif sorting == True or sorting == 'ascii':
         files = np.sort(files)
 
     return files
 
 
 def natural_sort(l):
     """
@@ -1802,19 +1917,19 @@
     :return: colormap for matplotlib
     """
     import colorsys
 
     from matplotlib.colors import LinearSegmentedColormap
 
     if type not in ("bright", "soft"):
-        print('Please choose "bright" or "soft" for type')
+        logger.warning('Please choose "bright" or "soft" for type')
         return
 
     if verbose:
-        print("Number of labels: " + str(nlabels))
+        logger.info("Number of labels: " + str(nlabels))
 
     # Generate color map for bright colors, based on hsv
     if type == "bright":
         randHSVcolors = [
             (
                 np.random.uniform(low=0.0, high=1),
                 np.random.uniform(low=0.2, high=1),
```

### Comparing `imgmisc-0.2.1/imgmisc.egg-info/PKG-INFO` & `imgmisc-0.2.2/imgmisc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgmisc
-Version: 0.2.1
+Version: 0.2.2
 Summary: imgmisc
 Home-page: https://github.com/supersubscript/imgmisc
 Author: Henrik Åhl
 Author-email: hpa22@cam.ac.uk
 License: GNU General Public License v3
 Keywords: imgmisc
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `imgmisc-0.2.1/imgmisc.egg-info/SOURCES.txt` & `imgmisc-0.2.2/imgmisc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgmisc-0.2.1/setup.py` & `imgmisc-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     keywords='imgmisc',
     name='imgmisc',
     packages=find_packages(include=['imgmisc', 'imgmisc.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/supersubscript/imgmisc',
-    version='0.2.1',
+    version='0.2.2',
     zip_safe=False,
 )
```

### Comparing `imgmisc-0.2.1/tests/test_imgmisc.py` & `imgmisc-0.2.2/tests/test_imgmisc.py`

 * *Files identical despite different names*

