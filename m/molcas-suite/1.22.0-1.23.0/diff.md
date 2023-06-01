# Comparing `tmp/molcas_suite-1.22.0.tar.gz` & `tmp/molcas_suite-1.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molcas_suite-1.22.0.tar", last modified: Sun May 28 14:32:12 2023, max compression
+gzip compressed data, was "molcas_suite-1.23.0.tar", last modified: Thu Jun  1 10:32:07 2023, max compression
```

## Comparing `molcas_suite-1.22.0.tar` & `molcas_suite-1.23.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:32:12.020009 molcas_suite-1.22.0/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3618 2023-05-28 14:32:12.020009 molcas_suite-1.22.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:32:12.018009 molcas_suite-1.22.0/molcas_suite/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-28 14:32:09.000000 molcas_suite-1.22.0/molcas_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/barrier.py
--rw-rw-rw-   0 root         (0) root         (0)     2188 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/cfp.py
--rw-rw-rw-   0 root         (0) root         (0)    28028 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    31919 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    18391 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/generate_input.py
--rw-rw-rw-   0 root         (0) root         (0)    25262 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/generate_job.py
--rw-rw-rw-   0 root         (0) root         (0)     6356 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/h5tools.py
--rw-rw-rw-   0 root         (0) root         (0)    21698 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/molcas_suite/orbs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 14:32:12.019009 molcas_suite-1.22.0/molcas_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3618 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-28 14:32:11.000000 molcas_suite-1.22.0/molcas_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-05-28 14:31:52.000000 molcas_suite-1.22.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 14:32:12.020009 molcas_suite-1.22.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1458 2023-05-28 14:32:09.000000 molcas_suite-1.22.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:32:07.767176 molcas_suite-1.23.0/molcas_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-01 10:32:05.000000 molcas_suite-1.23.0/molcas_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/barrier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2188 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/cfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    28336 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    31919 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    18799 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/generate_input.py
+-rw-rw-rw-   0 root         (0) root         (0)    25262 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/generate_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     6356 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/h5tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21698 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/molcas_suite/orbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/molcas_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3618 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 10:32:07.000000 molcas_suite-1.23.0/molcas_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-01 10:31:53.000000 molcas_suite-1.23.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 10:32:07.769176 molcas_suite-1.23.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2023-06-01 10:32:05.000000 molcas_suite-1.23.0/setup.py
```

### Comparing `molcas_suite-1.22.0/LICENSE` & `molcas_suite-1.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/PKG-INFO` & `molcas_suite-1.23.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas_suite
-Version: 1.22.0
+Version: 1.23.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.22.0/README.md` & `molcas_suite-1.23.0/README.md`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/molcas_suite/barrier.py` & `molcas_suite-1.23.0/molcas_suite/barrier.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/molcas_suite/cfp.py` & `molcas_suite-1.23.0/molcas_suite/cfp.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/molcas_suite/cli.py` & `molcas_suite-1.23.0/molcas_suite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         args.central_atom,
         args.charge,
         args.n_active_elec,
         args.n_active_orb,
         args.n_coord_atoms,
         name,
         xfield=xfield,
+        kirkwood=args.kirkwood,
         decomp=args.decomp,
         gateway_extra=args.gateway_extra,
         basis_set_central=args.basis_set_central,
         basis_set_coord=args.basis_set_coord,
         basis_set_remaining=args.basis_set_remaining,
         rasscf_extra=args.rasscf_extra,
         high_S_only=args.high_S_only,
@@ -598,14 +599,22 @@
     gen_inp.add_argument(
         '--skip_magneto',
         action=argparse.BooleanOptionalAction,
         default=False,
         help='Skip calculation of magnetic data.'
     )
 
+    gen_inp.add_argument(
+        '--kirkwood',
+        nargs=3,
+        metavar=("eps", "radius", "order"),
+        help=('Request Kirkwood reaction field with parameters: dielectric '
+              'constant, cavitiy radius in Å, order of multipole expansion.')
+        )
+
     # Generate Jobscript
 
     job = subparsers.add_parser(
         'generate_job',
         description="""
         Creates shell script for running molcas calculation
         """,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `molcas_suite-1.22.0/molcas_suite/extractor.py` & `molcas_suite-1.23.0/molcas_suite/extractor.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/molcas_suite/generate_input.py` & `molcas_suite-1.23.0/molcas_suite/generate_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 import numpy.linalg as la
 import xyz_py as xyzp
 from xyz_py import atomic
 import scipy.special as sps
 import copy
 
+ANG2BOHR = 1.88973
 
 class MolcasInput:
 
     def __init__(self, *sections, title=None):
         self.sections = sections
         self.title = title
 
@@ -71,15 +72,20 @@
              if isinstance(val, list) else (
                  "\n".join(map(str_indent, (f"{key}",) + val))
                  if isinstance(val, tuple) else str_indent(f"{key}= {val}"))
              for key, val in keywords_vals.items() if val is not None])
 
 
 class Gateway(MolcasProg):
-    def __init__(self, *args, group="NoSym", **kwargs):
+    def __init__(self, *args, group="NoSym", kirkwood=None, **kwargs):
+
+        if kirkwood is not None:  # make me pretty
+            rf_params = f"{kirkwood[0]} {float(kirkwood[1]) * ANG2BOHR} {kirkwood[2]}"
+            kwargs["rf-input"] = ("reaction field", rf_params, "end of rf-input")
+
         super().__init__('Gateway', *args, **kwargs, group="NoSym")
 
 
 class Seward(MolcasProg):
     def __init__(self, *args, **kwargs):
         super().__init__('Seward', *args, **kwargs)
 
@@ -229,15 +235,15 @@
         for line in xfield:
             # x, y, z, charge (, dipolex, dipoley, dipolez)
             f.write(fmt.format(*line))
 
 
 def generate_input(labels, coords, central_atom, charge, n_active_elec,
                    n_active_orb, n_coord_atoms, f_name,
-                   xfield=None, coord_hydrogens=False,
+                   xfield=None, kirkwood=None, coord_hydrogens=False,
                    decomp="High Cholesky", gateway_extra=((), {}),
                    basis_set_central="ANO-RCC-VTZP",
                    basis_set_coord="ANO-RCC-VDZP",
                    basis_set_remaining="ANO-RCC-VDZ",
                    rasscf_extra=((), {}), high_S_only=False, initial_orb=None,
                    max_orb=None, extract_orbs=True,
                    caspt2=False, caspt2_extra=((), {}),
@@ -264,14 +270,16 @@
         Number of active orbitals
     n_coord_atoms : int
         Number of atoms coordinates to central atom
     f_name : str
         Filename of final input file including extension
     xfield : list, optional
         list of lists of x, y, z, charge, dipole
+    kirkwood: tuple, optional
+        Tuple of dielectric constant, cavitiy radius in Å, order of multipoles
     coord_hydrogens : bool, default False
         If True, hydrogens will be treated as coordinating atoms
     decomp : str, default "High Cholesky"
         Keyword(s) to use for SEWARD 2 electron integral decompositon
     gateway_extra : list, optional
         Extra keywords/commands for GATEWAY section
     basis_set_central : str, default ANO-RCC-VTZP
@@ -348,14 +356,15 @@
     sections.append(Gateway(
         "AMFI",
         *gateway_extra[0],
         "RICD" if decomp == 'RICD_acCD' else None,
         "acCD" if decomp == 'RICD_acCD' else None,
         Coord=f"${{CurrDir}}/{rel_stem}_basis.xyz",
         XField=f"${{CurrDir}}/{rel_stem}.xfield" if xfield else None,
+        kirkwood=kirkwood,
         Angmom=' '.join(map(str, coords[ctr_idx])) + " ANGSTROM",
         **gateway_extra[1]))
 
     sections.append(Seward(decomp if decomp != 'RICD_acCD' else None))
 
     # Get information on electronic states
     spin_list, root_list, trunc_root_list = get_spin_and_roots(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `molcas_suite-1.22.0/molcas_suite/generate_job.py` & `molcas_suite-1.23.0/molcas_suite/generate_job.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/molcas_suite/h5tools.py` & `molcas_suite-1.23.0/molcas_suite/h5tools.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/molcas_suite/orbs.py` & `molcas_suite-1.23.0/molcas_suite/orbs.py`

 * *Files identical despite different names*

### Comparing `molcas_suite-1.22.0/molcas_suite.egg-info/PKG-INFO` & `molcas_suite-1.23.0/molcas_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molcas-suite
-Version: 1.22.0
+Version: 1.23.0
 Summary: A package for dealing with OpenMOLCAS input and output files
 Home-page: https://gitlab.com/chilton-group/molcas_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/molcas_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/molcas_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molcas_suite-1.22.0/setup.py` & `molcas_suite-1.23.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.22.0"
+__version__ = "1.23.0"
 
 setuptools.setup(
     name='molcas_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for dealing with OpenMOLCAS input and output files',
@@ -30,15 +30,15 @@
         'Operating System :: OS Independent'
         ],
     python_requires='>=3.9',
     install_requires=[
         'numpy',
         'scipy',
         'h5py',
-        'xyz_py>=5.1.0',
+        'xyz_py>=5.6.1',
         'angmom_suite>=1.11.1',
         'hpc_suite>=1.8.0',
         'matplotlib'
         ],
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
```

