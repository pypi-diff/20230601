# Comparing `tmp/atom_access-2.1.1.tar.gz` & `tmp/atom_access-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atom_access-2.1.1.tar", last modified: Tue Feb 28 13:38:47 2023, max compression
+gzip compressed data, was "atom_access-2.2.0.tar", last modified: Thu Jun  1 10:11:43 2023, max compression
```

## Comparing `atom_access-2.1.1.tar` & `atom_access-2.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 13:38:47.967232 atom_access-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    35079 2023-02-28 13:38:02.000000 atom_access-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3867 2023-02-28 13:38:47.966232 atom_access-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3171 2023-02-28 13:38:02.000000 atom_access-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 13:38:47.959231 atom_access-2.1.1/atom_access/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-28 13:38:02.000000 atom_access-2.1.1/atom_access/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-02-28 13:38:02.000000 atom_access-2.1.1/atom_access/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11728 2023-02-28 13:38:02.000000 atom_access-2.1.1/atom_access/core.py
--rw-rw-rw-   0 root         (0) root         (0)     4481 2023-02-28 13:38:02.000000 atom_access-2.1.1/atom_access/objects.py
--rwxrwxrwx   0 root         (0) root         (0)     4787 2023-02-28 13:38:02.000000 atom_access-2.1.1/atom_access/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-02-28 13:38:44.000000 atom_access-2.1.1/atom_access/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 13:38:47.963232 atom_access-2.1.1/atom_access.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3867 2023-02-28 13:38:47.000000 atom_access-2.1.1/atom_access.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2023-02-28 13:38:47.000000 atom_access-2.1.1/atom_access.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 13:38:47.000000 atom_access-2.1.1/atom_access.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-02-28 13:38:47.000000 atom_access-2.1.1/atom_access.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-28 13:38:47.000000 atom_access-2.1.1/atom_access.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-02-28 13:38:47.000000 atom_access-2.1.1/atom_access.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 13:38:47.966232 atom_access-2.1.1/old/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-28 13:38:02.000000 atom_access-2.1.1/old/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3599 2023-02-28 13:38:02.000000 atom_access-2.1.1/old/atom_access.py
--rw-rw-rw-   0 root         (0) root         (0)    17284 2023-02-28 13:38:02.000000 atom_access-2.1.1/old/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-02-28 13:38:02.000000 atom_access-2.1.1/old/version.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-02-28 13:38:02.000000 atom_access-2.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 13:38:47.967232 atom_access-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-02-28 13:38:44.000000 atom_access-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:11:43.153767 atom_access-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35079 2023-06-01 10:11:10.000000 atom_access-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-06-01 10:11:43.152767 atom_access-2.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3171 2023-06-01 10:11:10.000000 atom_access-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:11:43.149767 atom_access-2.2.0/atom_access/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-01 10:11:10.000000 atom_access-2.2.0/atom_access/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4724 2023-06-01 10:11:10.000000 atom_access-2.2.0/atom_access/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    12496 2023-06-01 10:11:10.000000 atom_access-2.2.0/atom_access/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     4581 2023-06-01 10:11:10.000000 atom_access-2.2.0/atom_access/objects.py
+-rwxrwxrwx   0 root         (0) root         (0)     4921 2023-06-01 10:11:10.000000 atom_access-2.2.0/atom_access/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-01 10:11:40.000000 atom_access-2.2.0/atom_access/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:11:43.151767 atom_access-2.2.0/atom_access.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-06-01 10:11:43.000000 atom_access-2.2.0/atom_access.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-06-01 10:11:43.000000 atom_access-2.2.0/atom_access.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 10:11:43.000000 atom_access-2.2.0/atom_access.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-01 10:11:43.000000 atom_access-2.2.0/atom_access.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-01 10:11:43.000000 atom_access-2.2.0/atom_access.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 10:11:43.000000 atom_access-2.2.0/atom_access.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:11:43.152767 atom_access-2.2.0/old/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-06-01 10:11:10.000000 atom_access-2.2.0/old/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3599 2023-06-01 10:11:10.000000 atom_access-2.2.0/old/atom_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    17284 2023-06-01 10:11:10.000000 atom_access-2.2.0/old/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-01 10:11:10.000000 atom_access-2.2.0/old/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-06-01 10:11:10.000000 atom_access-2.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 10:11:43.153767 atom_access-2.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2023-06-01 10:11:40.000000 atom_access-2.2.0/setup.py
```

### Comparing `atom_access-2.1.1/LICENSE` & `atom_access-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atom_access-2.1.1/PKG-INFO` & `atom_access-2.2.0/atom_access.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: atom_access
-Version: 2.1.1
+Name: atom-access
+Version: 2.2.0
 Summary: atom_access is a ray tracing package for addressing the steric          hindrance of molecules
 Home-page: https://gitlab.com/chilton-group/atom_access
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/atom_access/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/atom_access/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 `atom_access` is a python package for assessing the steric hindrance at any atom in a molecule or molecular fragment.
 
 We request that any results obtained through the use of `atom_access` are accompanied by the following reference:
 > Gransbury, G. K.; Corner, S. C.; Kragskow, J. G. C., Evans, P.; Yeung, H. M.; Blackmore, W. J. A.; Whitehead, G. F. S.; Vitorica-Yrezabal, I. J.; Chilton, N. F.; Mills, D. P. *AtomAccess*: A predictive tool for molecular design and its application to the targeted synthesis of dysprosium single-molecule magnets. *ChemRxiv* **2023**, DOI: 10.26434/chemrxiv-2023-28z84.
```

### Comparing `atom_access-2.1.1/README.md` & `atom_access-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `atom_access-2.1.1/atom_access/cli.py` & `atom_access-2.2.0/atom_access/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,191 +1,194 @@
-"""
+'''
 This module contains the command line interface to atom_access
-"""
+'''
 
 import argparse
 from textwrap import dedent
 import numpy as np
 import xyz_py as xyzp
 from . import utils as ut
 from .core import trace_rays, cluster_rays, cluster_size, generate_output
 import pickle
 
 
 def tracing_func(args):
-    """
+    '''
 
     Wrapper function for ray tracing program
 
     Parameters
     ----------
     args : argparser object
         User arguments
 
     Returns
     -------
     None
-
-    """
+    '''
 
     # Check requested density
     if args.density < 0:
-        exit("ZCW Densities must be >=0")
+        exit('ZCW Densities must be >=0')
     elif args.density > 16:
-        exit("ZCW Densities higher than 16 are not supported")
+        exit('ZCW Densities higher than 16 are not supported')
 
     # Load xyz file
     labels, coords = xyzp.load_xyz(args.xyz_f_name)
     labels_nn = xyzp.remove_label_indices(labels)
 
     blocked, unblocked, n_cut = trace_rays(
         labels_nn,
         coords,
-        args.atom-1,
+        args.atom - 1,
         args.cutoff,
         args.density
     )
 
     total_rays = len(blocked) + len(unblocked)
-    pc_unblocked = len(unblocked)/(total_rays) * 100.
+    pc_unblocked = len(unblocked) / (total_rays) * 100.
 
     if not args.quiet:
-        print("\nUsing {:d} rays".format(total_rays))
+        print('\nUsing {:d} rays'.format(total_rays))
         print(
-            "Cutoff of {:f} Angstroms has been enforced, ".format(args.cutoff),
-            "{:d} atoms are completely excluded".format(n_cut)
+            'Cutoff of {:f} Angstroms has been enforced, '.format(args.cutoff),
+            '{:d} atoms are completely excluded'.format(n_cut)
         )
 
-        print("{:.2f} % solid angle is visible".format(pc_unblocked))
+        print('{:.2f} % solid angle is visible'.format(pc_unblocked))
 
     # Cluster rays
     cluster_id = cluster_rays(unblocked, args.density)
 
     if not cluster_id.size and args.quiet:
-        exit("All rays are blocked")
+        exit('All rays are blocked')
     elif not cluster_id.size:
         exit()
 
     # Calculate size of clusters
     clust_percent, _ = cluster_size(cluster_id, total_rays)
 
     if not args.quiet:
-        print("\nThere are {:d} clusters".format(clust_percent.size))
+        print('\nThere are {:d} clusters'.format(clust_percent.size))
 
         for idx, x in enumerate(clust_percent):
             print(
-              "Cluster {:d} contains {:.2f} % solid angle".format(idx+1, x)
+                'Cluster {:d} contains {:.2f} % solid angle'.format(idx + 1, x)
             )
 
     # Get head of xyz file name (i.e. without extension)
-    f_head = args.xyz_f_name.split(".", 1)[0]
+    f_head = args.xyz_f_name.split('.', 1)[0]
 
     # Print output file
     generate_output(
         f_head, args.density, pc_unblocked, clust_percent, args.cutoff,
         no_header=args.quiet
     )
 
+    # Save rays, and xyz file shifted such that
+    # atom of interest is at origin.
     if args.save_rays:
-        _coords = coords - coords[args.atom-1]
-        xyzp.save_xyz("{}_shift.xyz".format(f_head), labels, _coords)
-        with open("rays.pickle", 'wb') as f:
+        print()
+        _coords = coords - coords[args.atom - 1]
+        xyzp.save_xyz('{}_shift.xyz'.format(f_head), labels, _coords)
+        with open('rays.pickle', 'wb') as f:
             pickle.dump(unblocked, f)
+        print('Rays pickled to rays.pickle')
 
     if args.plot:
         cart_vecs = np.array([ray.cart for ray in unblocked])
         ut.plot_rays(cart_vecs, cluster_id, clust_percent.size, show=True)
 
     return
 
 
 def read_args(arg_list=None):
-    """
+    '''
 
     Creates parser and subparsers for command line arguments
 
     Parameters
     ----------
     arg_list : list
         User arguments
 
     Returns
     -------
     None
 
-    """
+    '''
 
-    description = """
+    description = '''
     A program for assessing steric hinderance using ray tracing
-    """
+    '''
 
     parser = argparse.ArgumentParser(
         description=description,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
 
     parser.set_defaults(func=tracing_func) # noqa
 
     parser.add_argument(
-        "xyz_f_name",
-        help="Name of .xyz file containing atomic coordinates"
+        'xyz_f_name',
+        help='Name of .xyz file containing atomic coordinates'
     )
 
     parser.add_argument(
-        "-a",
-        "--atom",
-        help="Index of atom for which %% visible rays is calculated.",
+        '-a',
+        '--atom',
+        help='Index of atom for which %% visible rays is calculated.',
         type=int,
         default=1
     )
 
     parser.add_argument(
-        "-d",
-        "--density",
+        '-d',
+        '--density',
         help=dedent(
-            "ZCW integration density.Integer between 0 and 16,"
-            " note - number of points does not increase linearly.\n"
+            'ZCW integration density.Integer between 0 and 16,'
+            ' note - number of points does not increase linearly.\n'
         ),
         type=int,
         default=10
     )
 
     parser.add_argument(
-        "-c",
-        "--cutoff",
+        '-c',
+        '--cutoff',
         help=dedent(
-            "Cutoff for intersection distance in Angstroms"
+            'Cutoff for intersection distance in Angstroms'
         ),
         default=5.,
         type=float,
     )
 
     parser.add_argument(
-        "-p",
-        "--plot",
+        '-p',
+        '--plot',
         help=dedent(
-            "Plot unblocked points in browser using Plotly"
+            'Plot unblocked points in browser using Plotly'
         ),
         action='store_true'
     )
 
     parser.add_argument(
-        "-sr",
-        "--save_rays",
+        '-sr',
+        '--save_rays',
         help=dedent(
-            "Pickle unblocked rays and save xyz file"
+            'Pickle unblocked rays and save xyz file'
         ),
         action='store_true'
     )
 
     parser.add_argument(
-        "-q",
-        "--quiet",
+        '-q',
+        '--quiet',
         help=dedent(
-            "Suppress print to terminal and output file header"
+            'Suppress print to terminal and output file header'
         ),
         action='store_true'
     )
 
     # If argument list is none, then call function func
     # which is assigned to help function
     args = parser.parse_args(arg_list)
```

### Comparing `atom_access-2.1.1/atom_access/core.py` & `atom_access-2.2.0/atom_access/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-"""
+'''
 This submodule contains the core atom_access functionality
-"""
+'''
 
 import numpy as np
+import numpy.typing as npt
 import xyz_py.atomic as atomic
 import numpy.linalg as la
-from .objects import Sphere
+from .objects import Sphere, Ray
 from . import utils as ut
 from sklearn.cluster import AgglomerativeClustering
 import datetime
 
 
-def trace_rays(labels, coords, centre, radial_cutoff, zcw_density):
-    """
+def trace_rays(labels: list[str], coords: npt.NDArray, centre: int,
+               radial_cutoff: float,
+               zcw_density: int) -> tuple[list[Ray], list[Ray], int]:
+    '''
     Performs ray tracing calculation on set of atomic coordinates to find
     blocked and unblocked rays.
     Atoms within `radial_cutoff` distance from the centre are represented by
     spheres with van der Waals atomic radii. Rays emanate from `centre` and are
     blocked by intersection with an atom.
 
     For van der Waals radii see:
         CRC Handbook of Chemistry and Physics, 97th Ed.; W. H. Haynes Ed. CRC
         Press/Taylor and Francis: Boca Raton, 2016 (accessed 2020-10-01).
 
     Parameters
     ----------
-    labels : list[str]
+    labels: list[str]
         atomic labels
-    coords : np.ndarray[float]
+    coords: np.ndarray[float]
         (n_atoms,3) array containing xyz coordinates of each atom
-    centre : int
+    centre: int
         Index of central atom from which rays emanate
-    radial_cutoff : float
+    radial_cutoff: float
         Cutoff after which atoms will not be considered in raytracing
-    zcw_density : int
+    zcw_density: int
         Value indicating density of rays generated using
         Zaremba-Conroy-Wolfsberg algorithm.
 
     Returns
     -------
     list[Ray]
         Blocked rays as atom_access.objects.ray objects
     list[Ray]
         Unblocked rays as atom_access.objects.ray objects
     n_cut
         Number of atoms excluded by `radial_cutoff`
-    """
+    '''
 
     # Shift chosen center to origin
     coords -= coords[centre]
 
     # Set radius of each atom in full molecule
     radii = [atomic.atomic_radii[lab] for lab in labels]
 
@@ -61,15 +64,15 @@
     labels = [labels[ord] for ord in ordering]
     dists = dists[ordering]
     radii = [radii[ord] for ord in ordering]
 
     # Remove any atoms which are further than distance cutoff
     if any(dist > radial_cutoff for dist in dists):
         cut = np.argmax(dists > radial_cutoff)
-        n_cut = len(dists)-cut
+        n_cut = len(dists) - cut
     else:
         cut = len(dists) + 1
         n_cut = 0
     coords = coords[1:cut]
     labels = labels[1:cut]
     radii = radii[1:cut]
 
@@ -92,34 +95,34 @@
 
     for ray in blocked:
         ray.calc_cart_i()
 
     return blocked, unblocked, n_cut
 
 
-def cluster_rays(rays, zcw_density):
-    """
+def cluster_rays(rays: list[Ray], zcw_density: int):
+    '''
     Clusters rays based on adjacency/connectivity to neighbour. ZCW Density
     defines distance between nearest neighbour rays generated
     in ZCW algorithm - similar to the use of atomic radii in molecular
     connectivity graphs.
 
     Parameters
     ----------
-    rays : list[Ray]
+    rays: list[Ray]
         Rays to cluster as atom_access.objects.ray objects
-    zcw_density : int
+    zcw_density: int
         Value indicating density of rays generated using
         Zaremba-Conroy-Wolfsberg algorithm.
 
     Returns
     -------
     np.ndarray[int]
         Integers specifying which cluster each ray belongs to
-    """
+    '''
 
     cart_vecs = np.array([ray.cart for ray in rays])
 
     # Neighbour threshold distances calculated using neighbours function,
     # rounded up at 8th decimal place
     neighbour_threshold = [
         1.36809116,
@@ -137,45 +140,48 @@
         0.08132305,
         0.06399453,
         0.05033967,
         0.03958930,
         0.03112650
     ]
 
+    if zcw_density >= len(neighbour_threshold):
+        raise ValueError('Clustering unsupported for density > 16')
+
     clstr = AgglomerativeClustering(
         n_clusters=None,
         compute_full_tree=True,
         linkage='single',
         distance_threshold=neighbour_threshold[zcw_density]
     )
     clstr.fit_predict(cart_vecs)
 
     # List of integers indicating which cluster each unblocked ray belongs to
     cluster_id = clstr.labels_
 
     return cluster_id
 
 
-def cluster_size(cluster_id, total_rays):
+def cluster_size(cluster_id: npt.ArrayLike, total_rays: int):
     '''
     Calculate the size of each cluster in terms of % solid angle.
 
     Parameters
     ----------
-    cluster_id : np.ndarray[int]
+    cluster_id: np.ndarray[int]
         Integers specifying which cluster each ray belongs to
-    total_rays : int
+    total_rays: int
         Total number of rays generated using
         Zaremba-Conroy-Wolfsberg algorithm.
 
     Returns
     -------
     list[float]
         % solid angle of each cluster, ordered from largest to smallest
-        cluster.
+        cluster
     list[int]
         Integers specifying ordering of cluster percentages relative to
         initial `cluster_id` order
     '''
 
     _, counts = np.unique(cluster_id, return_counts=True)
 
@@ -184,112 +190,116 @@
     # Order clusters based on size
     ordering = np.argsort(clust_percent)[::-1]
     clust_percent = clust_percent[ordering]
 
     return clust_percent, ordering
 
 
-def generate_output(f_head, zcw_density, pc_unblocked, clust_percent,
-                    radial_cutoff, no_header=False):
+def generate_output(f_head: str, zcw_density: int, pc_unblocked: float,
+                    clust_percent: list[float], radial_cutoff: float,
+                    no_header: bool = False) -> None:
     '''
     Generate an output file with molecule name, settings and cluster sizes.
 
     Parameters
     ----------
-    f_head : str
+    f_head: str
         Input .xyz file name without .xyz extension
-    zcw_density : int
+    zcw_density: int
         Value indicating density of rays generated using
         Zaremba-Conroy-Wolfsberg algorithm.
-    pc_unblocked : float
+    pc_unblocked: float
         Total % of unblocked rays
-    clust_percent : list[float]
+    clust_percent: list[float]
         Size of each cluster given as % solid angle, ordered from largest to
         smallest cluster.
-    radial_cutoff : float
+    radial_cutoff: float
         Cutoff after which atoms will not be considered in raytracing
-    no_header : bool
+    no_header: bool
         True if header suppressed in output file
 
     Returns
     -------
     None
     '''
 
     # Output file name
-    out_f_name = "{}.out".format(f_head)
+    out_f_name = f'{f_head}.out'
 
     # Print results to output
-    with open(out_f_name, "w") as f:
+    with open(out_f_name, 'w') as f:
         if no_header:
-            f.write("                                          Atom Access") # noqa
+            f.write('                                          Atom Access') # noqa
         else:
-            f.write(":5PPPPPPPPPPPPPPPPPPPPPPPPPPPPPPPPP:                                     !GPPPPPPPPPPPPPPPPPPPPPPP5:\n") # noqa
-            f.write("^@B?JJJJJJJJJJ????????JJJJJ????????^7YYYYYYYYYYYYYYY5555YYYYYYYYYYYYYYYJ~~??JJ???????JJJJJJJJJJJ?#@^\n") # noqa
-            f.write("^@Y           :!!!!!!~     .!!!!!!!!?5#&@@@@@@@@@@&BGGGB#@@@@@@@@@@@@#BJ7!!!  :!!!!!!            P@^\n") # noqa
-            f.write("^@Y           5@@@@@@@^    7@@@@@@@@@@P !5#@@@@G7^.      :!Y#@@@@&P7.7@@@@@@? 5@@@@@@^           P@^\n") # noqa
-            f.write("^@Y          .#@@@@@@@J    :??5@@@@B??!   .!PP^             .J#5!.   7@@@@@@P #@@@@@@^           P@^\n") # noqa
-            f.write("^@Y          ~@@@&5@@@B       !@@@@P                 ..       .      7@@@@@@&!@@@@@@@^           P@^\n") # noqa
-            f.write("^@Y          J@@@#~@@@@^      7@@@@P              .Y#&#G^            7@@@&B@@B@@G@@@@^           P@^\n") # noqa
-            f.write("^@Y          G@@@5 #@@@?      7@@@@P              ~@@@@@5            7@@@#J@@@@@?@@@@^           P@^\n") # noqa
-            f.write("^@Y         :&@@@B5&@@@G      7@@@@P               7PBGJ:            7@@@&~&@@@B!@@@@^           P@^\n") # noqa
-            f.write("^@Y         7@@@@@&&@@@@^     7@@@@P      .^7^                !^.    7@@@&.G@@@Y~@@@@^           P@^\n") # noqa
-            f.write("^@Y         P@@@@J Y@@@@J     7@@@@P  .~?P#@@&J:            !G@@#57^ 7@@@@.?@@@~~@@@@^           P@^\n") # noqa
-            f.write("^@Y         ?YJJY^ ^YJJY7     ^JJYPPYG&@@@@@@@@&P?~^:.::^7Y#@@@@@@@@BB#PJ? :JJJ.:YJJJ:           P@^\n") # noqa
-            f.write("^@Y                          .^75B&@@@@@@@@@@@@@@@@@&&&&@@@@@@@@@@@@@@@&GJ!.                     P@^\n") # noqa
-            f.write("^@Y                      :!YG&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&GJ~.                 P@^\n") # noqa
-            f.write("^@Y                 .^?5B&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&G?~.             P@^\n") # noqa
-            f.write("^@Y            .^!YG#@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&P?^.         P@^\n") # noqa
-            f.write("^@Y        .^?!^7???#@@@@@@@P?!~!75&@@@@@@#Y7~~!?G@@@@@@P7??77J@@@@@&57!~!?P@@@@@@&Y?!~^..:      P@^\n") # noqa
-            f.write("^@Y    :~JP#@@~     Y@@@@@@7   J:  ^&@@@@#:  ^?   J@@@@@?   :^7@@@@@!  :J   J@@@@@~  :J   Y#5!:  G@^\n") # noqa
-            f.write("^@Y:7YB&@@@@@#.  ~  ~@@@@@@:  :@7   G@@@@P   ?@.  ^@@@@@?   P@@@@@@@^  :PJYYP@@@@@:  ^PJYYG@@@&BY5P:\n") # noqa
-            f.write(" :?@@@@@@@@@@5  :P   #@@@@@:  :&BPPP&@@@@P   ?@PPPG@@@@@?   ..7@@@@@B!.  :!P@@@@@@B!.  :7P@@@@@@@!  \n") # noqa
-            f.write("  7@@@@@@@@@@7  ^P.  Y@@@@@:  :@PJJJ#@@@@P   ?@YJJ5@@@@@?   JPG@@@@@BG5?!   7@@@@@BG5?!   ?@@@@@@!  \n") # noqa
-            f.write("  7@@@@@@@@@&:   :   ~@@@@@^  :&!   B@@@@G   ?#   ~@@@@@?   Y#B@@@@@~  ^@~  :&@@@@^  ~@^  ^@@@@@@!  \n") # noqa
-            f.write("  7@@@@@@@@@G   !@~  .#@@@@P:  :  .J@@@@@@?.  :  ^G@@@@@?      #@@@@G:  :  .J@@@@@P:  :  .Y@@@@@@!  \n") # noqa
-            f.write("  7@@@@@@@@@&BBB&@#BBB&@@@@@@BGPPB&@@@@@@@@&BPPG#@@@@@@@&BBBBBB@@@@@@@BGPPB&@@@@@@@@BGPGB&@@@@@@@!  \n") # noqa
-            f.write("  !BBBBBBBBBBBBBBBBBBBBBBBBBBB###BBBBBBBBBBBB###BBBBBBBBBBBBBBBBBBBBBBB###BBBBBBBBBBB###BBBBBBBBB~  \n") # noqa
-        f.write("\n                  Gemma K. Gransbury, Jon G. C. Kragskow, Nicholas F. Chilton\n") # noqa
-        f.write("                                           Citation\n\n")
-        f.write("{}\n\n".format(
-            datetime.datetime.now().strftime("%H:%M:%S %d-%m-%Y "))
+            f.write(':5PPPPPPPPPPPPPPPPPPPPPPPPPPPPPPPPP:                                     !GPPPPPPPPPPPPPPPPPPPPPPP5:\n') # noqa
+            f.write('^@B?JJJJJJJJJJ????????JJJJJ????????^7YYYYYYYYYYYYYYY5555YYYYYYYYYYYYYYYJ~~??JJ???????JJJJJJJJJJJ?#@^\n') # noqa
+            f.write('^@Y           :!!!!!!~     .!!!!!!!!?5#&@@@@@@@@@@&BGGGB#@@@@@@@@@@@@#BJ7!!!  :!!!!!!            P@^\n') # noqa
+            f.write('^@Y           5@@@@@@@^    7@@@@@@@@@@P !5#@@@@G7^.      :!Y#@@@@&P7.7@@@@@@? 5@@@@@@^           P@^\n') # noqa
+            f.write('^@Y          .#@@@@@@@J    :??5@@@@B??!   .!PP^             .J#5!.   7@@@@@@P #@@@@@@^           P@^\n') # noqa
+            f.write('^@Y          ~@@@&5@@@B       !@@@@P                 ..       .      7@@@@@@&!@@@@@@@^           P@^\n') # noqa
+            f.write('^@Y          J@@@#~@@@@^      7@@@@P              .Y#&#G^            7@@@&B@@B@@G@@@@^           P@^\n') # noqa
+            f.write('^@Y          G@@@5 #@@@?      7@@@@P              ~@@@@@5            7@@@#J@@@@@?@@@@^           P@^\n') # noqa
+            f.write('^@Y         :&@@@B5&@@@G      7@@@@P               7PBGJ:            7@@@&~&@@@B!@@@@^           P@^\n') # noqa
+            f.write('^@Y         7@@@@@&&@@@@^     7@@@@P      .^7^                !^.    7@@@&.G@@@Y~@@@@^           P@^\n') # noqa
+            f.write('^@Y         P@@@@J Y@@@@J     7@@@@P  .~?P#@@&J:            !G@@#57^ 7@@@@.?@@@~~@@@@^           P@^\n') # noqa
+            f.write('^@Y         ?YJJY^ ^YJJY7     ^JJYPPYG&@@@@@@@@&P?~^:.::^7Y#@@@@@@@@BB#PJ? :JJJ.:YJJJ:           P@^\n') # noqa
+            f.write('^@Y                          .^75B&@@@@@@@@@@@@@@@@@&&&&@@@@@@@@@@@@@@@&GJ!.                     P@^\n') # noqa
+            f.write('^@Y                      :!YG&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&GJ~.                 P@^\n') # noqa
+            f.write('^@Y                 .^?5B&@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&G?~.             P@^\n') # noqa
+            f.write('^@Y            .^!YG#@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@&P?^.         P@^\n') # noqa
+            f.write('^@Y        .^?!^7???#@@@@@@@P?!~!75&@@@@@@#Y7~~!?G@@@@@@P7??77J@@@@@&57!~!?P@@@@@@&Y?!~^..:      P@^\n') # noqa
+            f.write('^@Y    :~JP#@@~     Y@@@@@@7   J:  ^&@@@@#:  ^?   J@@@@@?   :^7@@@@@!  :J   J@@@@@~  :J   Y#5!:  G@^\n') # noqa
+            f.write('^@Y:7YB&@@@@@#.  ~  ~@@@@@@:  :@7   G@@@@P   ?@.  ^@@@@@?   P@@@@@@@^  :PJYYP@@@@@:  ^PJYYG@@@&BY5P:\n') # noqa
+            f.write(' :?@@@@@@@@@@5  :P   #@@@@@:  :&BPPP&@@@@P   ?@PPPG@@@@@?   ..7@@@@@B!.  :!P@@@@@@B!.  :7P@@@@@@@!  \n') # noqa
+            f.write('  7@@@@@@@@@@7  ^P.  Y@@@@@:  :@PJJJ#@@@@P   ?@YJJ5@@@@@?   JPG@@@@@BG5?!   7@@@@@BG5?!   ?@@@@@@!  \n') # noqa
+            f.write('  7@@@@@@@@@&:   :   ~@@@@@^  :&!   B@@@@G   ?#   ~@@@@@?   Y#B@@@@@~  ^@~  :&@@@@^  ~@^  ^@@@@@@!  \n') # noqa
+            f.write('  7@@@@@@@@@G   !@~  .#@@@@P:  :  .J@@@@@@?.  :  ^G@@@@@?      #@@@@G:  :  .J@@@@@P:  :  .Y@@@@@@!  \n') # noqa
+            f.write('  7@@@@@@@@@&BBB&@#BBB&@@@@@@BGPPB&@@@@@@@@&BPPG#@@@@@@@&BBBBBB@@@@@@@BGPPB&@@@@@@@@BGPGB&@@@@@@@!  \n') # noqa
+            f.write('  !BBBBBBBBBBBBBBBBBBBBBBBBBBB###BBBBBBBBBBBB###BBBBBBBBBBBBBBBBBBBBBBB###BBBBBBBBBBB###BBBBBBBBB~  \n') # noqa
+        f.write('\n                  Gemma K. Gransbury, Jon G. C. Kragskow, Nicholas F. Chilton\n') # noqa
+        f.write('\nGransbury, G. K.; Corner, S. C.; Kragskow, J. G. C.; Evans, P.; Yeung, H. M.; Blackmore, W. J. A.;') # noqa
+        f.write('\n     Whitehead, G. F. S.; Vitorica-Yrezabal, I. J.; Chilton, N. F.; Mills, D. P. AtomAccess:')       # noqa
+        f.write('\nA predictive tool for molecular design and its application to the targeted synthesis of dysprosium') # noqa
+        f.write('\n           single-molecule magnets. ChemRxiv, 2023, DOI: 10.26434/chemrxiv-2023-28z84.\n\n')         # noqa
+        f.write('{}\n\n'.format(
+            datetime.datetime.now().strftime('%H:%M:%S %d-%m-%Y '))
         )
 
-        f.write("Output file for {}\n".format(f_head))
+        f.write(f'Output file for {f_head}\n')
 
-        f.write("Integration density: {:d}\n".format(zcw_density))
-        f.write("Radial cutoff: {:f} Angstrom\n\n".format(radial_cutoff))
-        f.write("Total visible solid angle is {:.6f}\n\n".format(pc_unblocked))
-        f.write("There are {:d} clusters of visible points:\n".format(
+        f.write(f'Integration density: {zcw_density:d}\n')
+        f.write(f'Radial cutoff: {radial_cutoff:f} Angstrom\n\n')
+        f.write(f'Total visible solid angle is {pc_unblocked:.6f}\n\n')
+        f.write('There are {:d} clusters of visible points:\n'.format(
             clust_percent.size
         ))
 
         for idx, x in enumerate(clust_percent):
             f.write(
-                "Cluster {:d} contains {:.6f} % solid angle\n".format(
-                    idx+1, x
+                'Cluster {:d} contains {:.6f} % solid angle\n'.format(
+                    idx + 1, x
                 )
             )
     return
 
 
-def neighbours(rays, n):
+def neighbours(rays: list[Ray], n: int) -> float:
     '''
     Define maximum nth-nearest neighbour distance for a group of rays.
 
     Parameters
     ----------
-    rays : list[Ray]
+    rays: list[Ray]
         List of atom_access.objects.rays generated using ZCW algorithm
-    n : int
+    n: int
         Index of requested (nth) nearest neighbour
 
     Returns
     -------
-    float:
+    float
         maximum distance between any ray and its nth nearest neighbour
     '''
 
     # Extract ray vectors from rays
     cart_vecs = np.array([ray.cart for ray in rays])
 
     # Pairwise difference of all ray vectors
```

### Comparing `atom_access-2.1.1/atom_access/objects.py` & `atom_access-2.2.0/atom_access/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-"""
+'''
 This submodule contains ray and sphere objects and methods used for raytracing
-"""
+'''
 
 import numpy as np
+import numpy.typing as npt
 import numpy.linalg as la
 
 
 class Sphere:
-    """
+    '''
     Contains all information required to define a sphere and to calculate
     its intersection with a ray
 
     Parameters
     ----------
-    radius : float
+    radius: float
         Radius of sphere
-    center : np.ndarray[float]
+    center: np.ndarray[float]
         x,y,z coordinates of sphere center
 
     Attributes
     ----------
-    radius : float
+    radius: float
         Radius of sphere
-    radius2 : float
+    radius2: float
         Squared radius of sphere
-    center : np.ndarray[float]
+    center: np.ndarray[float]
         x,y,z coordinates of sphere center
-    center_dist : np.ndarray[float]
+    center_dist: np.ndarray[float]
         Distance to center from origin
-    """
+    '''
     __slots__ = 'radius', 'radius2', 'center', 'center_dist'
 
-    def __init__(self, radius, center):
+    def __init__(self, radius: float, center: npt.NDArray):
 
         self.radius = radius
         self.radius2 = radius**2
         self.center = center
         self.center_dist = la.norm(self.center)
 
         return
 
-    def intersect(self, ray):
-        """
+    def intersect(self, ray: 'Ray') -> tuple[bool, float, float]:
+        '''
         Calculate intersection points of normalised ray vector with
         sphere if they exist.
 
         Parameters
         ----------
-        ray : Ray
+        ray: Ray
             Ray object
 
         Returns
         -------
-        bool :
+        bool
             True if intersection, else False
-        float :
+        float
             First intersection point, 0 if no intersection
-        float :
+        float
             Second intersection point, 0 if no intersection
-        """
+        '''
 
         # Find projection of ray onto sphere centre-origin vector
         p = np.dot(self.center, ray.cart)
 
         if p < 0.:
             return False, 0., 0.
         # Find minimum sphere centre to ray distance (squared)
         d2 = self.center_dist**2 - p**2
         if d2 > self.radius2:
             return False, 0., 0.
-        t = np.sqrt(self.radius2-d2)
+        t = np.sqrt(self.radius2 - d2)
 
         # Find ray-sphere intersection points
         # These are scalars used in the vector equation of line
         # P1 = O + (p-t)*uhat
         # P2 = O + (p+t)*uhat
         # where P1 is intersection point on the ray, uhat is the
         # normalised ray vector, and O is a point in space,
@@ -81,106 +82,106 @@
         p1 = p - t
         p2 = p + t
 
         return True, p1, p2
 
 
 class Ray:
-    """
+    '''
     Contains all information required to define a ray of light and its
     intersection with an object
 
 
     Parameters
     ----------
-    theta : float
+    theta: float
         Polar angle 0 <= theta <= pi
-    phi : float
+    phi: float
         Azimuthal angle 0 <= phi <= 2pi
 
 
     Attributes
     ----------
-    theta : float
+    theta: float
         Polar angle 0 <= theta <= pi
-    phi : float
+    phi: float
         Azimuthal angle 0 <= phi <= 2pi
-    r : float
+    r: float
         Length of ray, assumed unity (ray is normalised)
-    x : float
+    x: float
         x component of ray vector in cartesian coordinates
-    y : float
+    y: float
         y component of ray vector in cartesian coordinates
-    z : float
+    z: float
         z component of ray vector in cartesian coordinates
-    cart : np.ndarray[float]
+    cart: np.ndarray[float]
         Direction vector of ray as (3,) np.array
-    intersection : bool
+    intersection: bool
         True if ray intersects with object
-    r_i : float
+    r_i: float
         Distance to intersection point from origin
-    cart_i : np.ndarray[float]
+    cart_i: np.ndarray[float]
         Position vector of intersection point as (3,) np.array
 
-    """
+    '''
     __slots__ = [
         'theta', 'phi', 'x', 'y', 'z', 'intersection', 'r', 'r_i', 'cart',
         'cart_i'
     ]
 
-    def __init__(self, theta, phi):
+    def __init__(self, theta: float, phi: float):
 
         # Spherical coordinates
         self.theta = theta
         self.phi = phi
         self.r = 1.
 
         # Cartesian coordinates
         st = np.sin(self.theta)
-        self.x = self.r*st*np.cos(self.phi)
-        self.y = self.r*st*np.sin(self.phi)
-        self.z = self.r*np.cos(self.theta)
+        self.x = self.r * st * np.cos(self.phi)
+        self.y = self.r * st * np.sin(self.phi)
+        self.z = self.r * np.cos(self.theta)
         self.cart = np.array([self.x, self.y, self.z])
 
         # Intersection point
         self.intersection = False
         self.r_i = np.inf
         self.cart_i = np.array([0., 0., 0.])
 
         return
 
-    def reset_intersection(self):
-        """
+    def reset_intersection(self) -> None:
+        '''
         Resets intersection attributes of ray
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
-        """
+        '''
 
         self.intersection = False
         self.r_i = 0.
         self.cart_i = [0., 0., 0.]
 
         return
 
-    def calc_cart_i(self):
-        """
+    def calc_cart_i(self) -> None:
+        '''
         Calculates position vector of intersection point using intersection
         distance
 
         Parameters
         ----------
         None
 
         Returns
         -------
         None
-        """
+        '''
 
         self.cart_i = self.cart * self.r_i
 
         return
```

### Comparing `atom_access-2.1.1/atom_access/utils.py` & `atom_access-2.2.0/atom_access/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,194 +1,197 @@
-"""
+'''
 This submodule contains utility functions
-"""
+'''
 
 import numpy as np
+import numpy.typing as npt
 from .objects import Ray
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 
-def create_zcw_rays(density):
-    """
+def create_zcw_rays(density: int) -> list[Ray]:
+    '''
     Generate a set of rays emanating from a single point using the ZCW
     algorithm
 
     See Appendix I in
-        Eden, M.; Levitt, M. H. J. Magn. Res., 1998, 132, 220-239.
+    Eden, M.; Levitt, M. H. J. Magn. Res., 1998, 132, 220-239.
 
     Parameters
     ----------
     density : int
         Density number for ZCW algorithm
 
     Returns
     -------
     list[Ray]
         List of ray objects
-    """
+    '''
 
-    g = [recursive_g(m) for m in range(density+3)]
-    N = g[density+2]
+    g = [recursive_g(m) for m in range(density + 3)]
+    N = g[density + 2]
 
     c = [1, 2, 1]
 
     rays = [
         Ray(
-            np.arccos(c[0]*(c[1] * np.fmod(j/N, 1)-1)),
-            2*np.pi/c[2] * np.fmod(j*g[density]/N, 1)
+            np.arccos(c[0] * (c[1] * np.fmod(j / N, 1) - 1)),
+            2 * np.pi / c[2] * np.fmod(j * g[density] / N, 1)
         ) for j in range(N)
     ]
 
     return rays
 
 
-def recursive_g(m):
-    """
+def recursive_g(m: int) -> int:
+    '''
     Recursively calculates numbers g_m required by ZCW integration scheme
 
     Parameters
     ----------
     m : int
         m index
 
     Returns
     -------
     int
         g_m value for given m
 
-    """
+    '''
 
     if m == 0:
         g = 8
     elif m == 1:
         g = 13
     else:
-        g = recursive_g(m-2) + recursive_g(m-1)
+        g = recursive_g(m - 2) + recursive_g(m - 1)
 
     return g
 
 
-def plot_rays(vecs, clusters, n_clust, show=True, fig=None, colours=None):
-    """
+def plot_rays(vecs: npt.NDArray, clusters: npt.NDArray, n_clust: int,
+              show: bool = True, fig: go.Figure = None,
+              colours: list[str] = None) -> None:
+    '''
     Create a plot of unblocked rays for web browser using plotly
 
     Parameters
     ----------
     vecs : np.ndarray[float]
         (3,n_unblocked_rays) array containing xyz vectors of unblocked rays
     clusters : np.ndarray[int]
         Integers specifying which cluster each ray belongs to
     n_clust : int
         Number of clusters
     show : bool
         If true, displays figure in browser
-    fig : plotly graph objects figure object
+    fig : go.Figure
         If provided, rays are added to this figure
     colours : list[str]
-        List of colours, one per cluster formatted as
-        [
-            "rgb(VAL, VAL, VAL)",
-            "rgb(VAL, VAL, VAL)",
-            ...
-        ]
+        List of colours, one per cluster formatted as\n
+        [\n
+            'rgb(VAL, VAL, VAL)',\n
+            'rgb(VAL, VAL, VAL)',\n
+            ...\n
+        ]\n
         where VAL is Red, Green, Blue in range(0, 255)
 
     Returns
     -------
-    plotly graph objects figure object
+    go.Figure
         Figure of unblocked rays as points
-    """
+    '''
 
     if not colours:
         colours = [
-            "rgb(51 , 34 , 136)",
-            "rgb(17 , 119, 51)",
-            "rgb(68 , 170, 153)",
-            "rgb(136, 204, 238)",
-            "rgb(221, 204, 119)",
-            "rgb(204, 102, 119)",
-            "rgb(170, 68 , 153)",
-            "rgb(136, 34 , 85)",
-            "rgb(0  , 0  , 0)",
-            "rgb(230, 159, 0)",
-            "rgb(86 , 180, 233)",
-            "rgb(0  , 158, 115)",
-            "rgb(240, 228, 66)",
-            "rgb(0  , 114, 178)",
-            "rgb(213, 94 , 0)",
-            "rgb(204, 121, 167)",
+            'rgb(51 , 34 , 136)',
+            'rgb(17 , 119, 51)',
+            'rgb(68 , 170, 153)',
+            'rgb(136, 204, 238)',
+            'rgb(221, 204, 119)',
+            'rgb(204, 102, 119)',
+            'rgb(170, 68 , 153)',
+            'rgb(136, 34 , 85)',
+            'rgb(0  , 0  , 0)',
+            'rgb(230, 159, 0)',
+            'rgb(86 , 180, 233)',
+            'rgb(0  , 158, 115)',
+            'rgb(240, 228, 66)',
+            'rgb(0  , 114, 178)',
+            'rgb(213, 94 , 0)',
+            'rgb(204, 121, 167)',
         ]
 
     if fig is None:
         fig = make_subplots()
     for cl in range(n_clust):
         # Unblocked rays
         fig.add_trace(
             go.Scatter3d(
                 x=vecs[clusters == cl, 0],
                 y=vecs[clusters == cl, 1],
                 z=vecs[clusters == cl, 2],
-                mode="markers",
-                marker={"color": colours[cl]},
+                mode='markers',
+                marker={'color': colours[cl]},
                 showlegend=False
             )
         )
 
     # Turn off plotly gubbins
     layout = go.Layout(
         hovermode=False,
-        dragmode="orbit",
-        scene_aspectmode="cube",
+        dragmode='orbit',
+        scene_aspectmode='cube',
         scene=dict(
             xaxis=dict(
-                gridcolor="rgb(255, 255, 255)",
-                zerolinecolor="rgb(255, 255, 255)",
+                gridcolor='rgb(255, 255, 255)',
+                zerolinecolor='rgb(255, 255, 255)',
                 showbackground=False,
                 showgrid=False,
                 zeroline=False,
-                title="",
+                title='',
                 showline=False,
-                ticks="",
+                ticks='',
                 showticklabels=False,
-                backgroundcolor="rgb(255, 255,255)",
+                backgroundcolor='rgb(255, 255,255)',
             ),
             yaxis=dict(
-                gridcolor="rgb(255, 255, 255)",
-                zerolinecolor="rgb(255, 255, 255)",
+                gridcolor='rgb(255, 255, 255)',
+                zerolinecolor='rgb(255, 255, 255)',
                 showgrid=False,
                 zeroline=False,
-                title="",
+                title='',
                 showline=False,
-                ticks="",
+                ticks='',
                 showticklabels=False,
-                backgroundcolor="rgb(255, 255,255)",
-                ),
+                backgroundcolor='rgb(255, 255,255)',
+            ),
             zaxis=dict(
-                gridcolor="rgb(255, 255, 255)",
-                zerolinecolor="rgb(255, 255, 255)",
+                gridcolor='rgb(255, 255, 255)',
+                zerolinecolor='rgb(255, 255, 255)',
                 showgrid=False,
-                title="",
+                title='',
                 zeroline=False,
                 showline=False,
-                ticks="",
+                ticks='',
                 showticklabels=False,
-                backgroundcolor="rgb(255, 255,255)",
+                backgroundcolor='rgb(255, 255,255)',
             ),
             aspectratio=dict(
                 x=1,
                 y=1,
                 z=1
             ),
         ),
         margin={
-            "l": 20,
-            "r": 30,
-            "t": 30,
-            "b": 20
+            'l': 20,
+            'r': 30,
+            't': 30,
+            'b': 20
         }
     )
 
     fig.update_layout(layout)
 
     if show:
         fig.show()
```

### Comparing `atom_access-2.1.1/atom_access.egg-info/PKG-INFO` & `atom_access-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: atom-access
-Version: 2.1.1
+Name: atom_access
+Version: 2.2.0
 Summary: atom_access is a ray tracing package for addressing the steric          hindrance of molecules
 Home-page: https://gitlab.com/chilton-group/atom_access
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/atom_access/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/atom_access/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 `atom_access` is a python package for assessing the steric hindrance at any atom in a molecule or molecular fragment.
 
 We request that any results obtained through the use of `atom_access` are accompanied by the following reference:
 > Gransbury, G. K.; Corner, S. C.; Kragskow, J. G. C., Evans, P.; Yeung, H. M.; Blackmore, W. J. A.; Whitehead, G. F. S.; Vitorica-Yrezabal, I. J.; Chilton, N. F.; Mills, D. P. *AtomAccess*: A predictive tool for molecular design and its application to the targeted synthesis of dysprosium single-molecule magnets. *ChemRxiv* **2023**, DOI: 10.26434/chemrxiv-2023-28z84.
```

### Comparing `atom_access-2.1.1/old/atom_access.py` & `atom_access-2.2.0/old/atom_access.py`

 * *Files identical despite different names*

### Comparing `atom_access-2.1.1/old/cli.py` & `atom_access-2.2.0/old/cli.py`

 * *Files identical despite different names*

### Comparing `atom_access-2.1.1/setup.py` & `atom_access-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from textwrap import dedent
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "2.1.1"
+__version__ = "2.2.0"
 
 setuptools.setup(
     name='atom_access',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description=dedent(
@@ -27,23 +27,23 @@
         "Bug Tracker": "https://gitlab.com/chilton-group/atom_access/-/issues",
         "Documentation": "https://chilton-group.gitlab.io/atom_access/"
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent'
-        ],
+    ],
     packages=setuptools.find_packages(),
-    python_requires='>=3.6',
+    python_requires='>=3.9',
     install_requires=[
-        'numpy',
-        'xyz_py>=5.1.0',
-        'plotly',
-        'scikit-learn'
-        ],
+        'numpy>=1.24.3',
+        'xyz_py>=5.6.1',
+        'plotly>=5.14.1',
+        'scikit-learn>=1.2.2'
+    ],
     entry_points={
         'console_scripts': [
             'atom_access = atom_access.cli:main',
             'atomaccess = atom_access.cli:main'
-            ]
-        }
-    )
+        ]
+    }
+)
```

