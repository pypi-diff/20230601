# Comparing `tmp/spin_phonon_suite-0.9.1.tar.gz` & `tmp/spin_phonon_suite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin_phonon_suite-0.9.1.tar", last modified: Thu Sep 22 16:44:44 2022, max compression
+gzip compressed data, was "spin_phonon_suite-1.0.0.tar", last modified: Thu Jun  1 13:19:24 2023, max compression
```

## Comparing `spin_phonon_suite-0.9.1.tar` & `spin_phonon_suite-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3750 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3031 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1648 2022-09-22 16:44:41.000000 spin_phonon_suite-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 16:44:44.620681 spin_phonon_suite-0.9.1/spin_phonon_suite/
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2022-09-22 16:44:41.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    26274 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/cells.py
--rw-rw-rw-   0 root         (0) root         (0)    34571 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    10565 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/derivative.py
--rw-rw-rw-   0 root         (0) root         (0)     8653 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/distortion.py
--rw-rw-rw-   0 root         (0) root         (0)     2906 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/func.py
--rw-rw-rw-   0 root         (0) root         (0)    12030 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/lvc.py
--rw-rw-rw-   0 root         (0) root         (0)    10800 2022-09-22 16:44:02.000000 spin_phonon_suite-0.9.1/spin_phonon_suite/vibrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 16:44:44.623681 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3750 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      138 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-09-22 16:44:44.000000 spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:19:24.963726 spin_phonon_suite-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35085 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-06-01 13:19:24.963726 spin_phonon_suite-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 13:19:24.963726 spin_phonon_suite-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1660 2023-06-01 13:19:22.000000 spin_phonon_suite-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:19:24.961727 spin_phonon_suite-1.0.0/spin_phonon_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-01 13:19:22.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10655 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/cells.py
+-rw-rw-rw-   0 root         (0) root         (0)    35667 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)    22303 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/lvc.py
+-rw-rw-rw-   0 root         (0) root         (0)    18786 2023-06-01 13:18:48.000000 spin_phonon_suite-1.0.0/spin_phonon_suite/vibrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:19:24.962726 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3750 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      526 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 13:19:24.000000 spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/top_level.txt
```

### Comparing `spin_phonon_suite-0.9.1/LICENSE` & `spin_phonon_suite-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.1/PKG-INFO` & `spin_phonon_suite-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin_phonon_suite
-Version: 0.9.1
+Version: 1.0.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-0.9.1/README.md` & `spin_phonon_suite-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-0.9.1/setup.py` & `spin_phonon_suite-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "0.9.1"
+__version__ = "1.0.0"
 
 setuptools.setup(
     name='spin_phonon_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian', # noqa
@@ -31,22 +31,22 @@
         ],
     python_requires='>=3.9',
     install_requires=[
         'numpy',
         'scipy',
         'h5py',
         'xyz_py>=5.1.0',
-        'angmom_suite>=1.10.0',
-        'hpc_suite',
+        'angmom_suite>=1.11.1',
+        'hpc_suite>=1.8.0',
         'matplotlib',
-        'findiff',
-        'gaussian_suite>=1.8.0',
+        'gaussian_suite>=1.11.0',
         'phonopy',
         'molvis>=0.3.0',
-        'molcas_suite'
+        'molcas_suite>=1.21.0',
+        'ase'
         ],
     packages=setuptools.find_packages(),
     entry_points={
         'console_scripts': [
             'spin_phonon_suite = spin_phonon_suite.cli:main'
             ]
         }
```

### Comparing `spin_phonon_suite-0.9.1/spin_phonon_suite/cli.py` & `spin_phonon_suite-1.0.0/spin_phonon_suite/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,473 +1,458 @@
 #!/usr/bin/env python3
 
 from argparse import ArgumentParser, ArgumentTypeError, \
-                     RawDescriptionHelpFormatter
+                     RawDescriptionHelpFormatter, BooleanOptionalAction
 import sys
 import os
 import re
-import numpy as np
 import pickle
+from operator import add
+from functools import reduce
+from itertools import product
+import h5py
+import numpy as np
 import matplotlib.pyplot as plt
 
 import gaussian_suite.gen_input as gsgi
 import xyz_py as xyzp
-import xyz_py.atomic as atomic
-from molcas_suite.extractor import make_extractor as make_molcas_extractor
-from gaussian_suite.extractor import make_extractor as make_gaussian_extractor
+from xyz_py import atomic
+from molcas_suite.cli import ParseExtra
 import gaussian_suite.cd_extractor as gscd
-from hpc_suite.action import ParseKwargs, BooleanOptionalAction
-from hpc_suite import parse_dict_key_only, parse_dict, SecondaryHelp
+import hpc_suite as hpc
+from hpc_suite.action import ParseKwargs, OrderedSelectionAction
+from hpc_suite import make_parse_dict, SecondaryHelp
 import angmom_suite
-import angmom_suite.crystal as crystal
+from angmom_suite import crystal
+from angmom_suite.basis import Level
+from angmom_suite.multi_electron import Ion
 import molvis.core as mvis
+from pymatgen.core.structure import Molecule, Structure
+from pymatgen.transformations.site_transformations import TranslateSitesTransformation
 
-from .distortion import Distortion, Dx, DistortionInfo
-from .derivative import Finite, print_tau_style, read_tau_style
-from .func import make_func
-from .lvc import LVC, generate_lvc_input
+from .coordinates import CoordinateInfo
+from .derivative import print_tau_style, read_tau_style
+from .lvc import LVC, generate_lvc_input, make_lvc_evaluator, ANG2BOHR, \
+    LVCModelHamiltonian, LVCAdiabaticEnergies, LVCDiabaticHamiltonian
 from .vibrations import Harmonic
 from . import cells
 
 plt.rcParams['font.family'] = "Arial"
 
+HARTREE2INVCM = 219474.63 
+
 
 # Action for secondary function help message
 class FunctionHelp(SecondaryHelp):
     def __call__(self, parser, namespace, values, option_string=None):
 
         if namespace.function == 'cfp':
             angmom_suite.read_args(['cfp', '--help'])
         else:
             raise ValueError("Supply valid option to function argument.")
 
 
-def generate_distortion_func(args):
-
-    labels, coords = xyzp.load_xyz(args.input)
-
-    sp_data = DistortionInfo.from_file(args.distortion_info)
-
-    coords += sp_data.make_distortion(args.distortion.axes).evaluate()
-
-    if args.origin:
-        origin = [lab.split('.')[0] for lab in labels].index(args.origin)
-        coords -= coords[origin]
-
-    xyzp.save_xyz(args.output, labels, coords)
-
-    return
+def str_int(x):
+    try:
+        return int(x)
+    except ValueError:
+        return str(x)
 
 
-def init_func(args):
-    sp_data = DistortionInfo.from_args(args)
+def coords_func(args):
+    sp_data = CoordinateInfo.from_args(args)
     sp_data.to_file(args.distortion_info)
 
     return
 
 
 def lvc_func(args):
 
-    sp_data = DistortionInfo.from_file(args.distortion_info)
+    if args.add is not None:
+        def join(a, b):
+            return a.join(b, xyzp.load_xyz(args.reference_xyz)[1] * ANG2BOHR)
+        lvc = reduce(join, (LVC.from_file(f_lvc) for f_lvc in args.add))
+
+    elif args.efld is not None:
+        charge_list = [np.loadtxt(f_chrg) for f_chrg in args.charge]
+        xyz_list = [xyzp.load_xyz(f_xyz)[1] * ANG2BOHR for f_xyz in args.xyz]
+        lvc = LVC.from_molcas_frozen_density(
+            args.rassi, args.efld, charge_list, xyz_list)
 
-    V0th = {}
-    W1st = {}
+    elif args.grad is not None:
+        lvc = LVC.from_molcas(args.rassi, args.grad)
 
-    sf_smult = make_molcas_extractor(args.rassi, ("rassi", "spin_mult"))[()]
-    ener = make_molcas_extractor(args.rassi, ("rassi", "SFS_energies"))[()]
+    else:
+        raise ValueError("LVC gradient information supplied!")
 
-    for smult, nroots in zip(*np.unique(sf_smult, return_counts=True)):
-        V0th[smult] = ener[smult == sf_smult]
-        W1st[smult] = np.zeros((nroots, nroots, sp_data.natoms, 3))
+    if args.active_atoms is not None:
+        idc = [idx - 1 for idc in args.active_atoms for idx in idc]
+        lvc = lvc.subset_atoms(active_atom_idc=idc)
 
-    for grad_file in args.grad:
+    elif args.ref_coordinates is not None:
+        _, coords = xyzp.load_xyz(args.ref_coordinates)
+        lvc = lvc.subset_atoms(ref_coords=coords * ANG2BOHR)
 
-        grad = make_molcas_extractor(grad_file, ("gradients", None))
+    lvc.to_file(args.lvc_data, verbose=args.verbose)
 
-        for lab, val in iter(grad):
-            smult, root = lab
-            W1st[smult][root-1, root-1] = val
+    return
 
-        nacs = make_molcas_extractor(grad_file, ("nacs", "CI"))
 
-        for lab, val in iter(nacs):
-            smult, root1, root2 = lab
-            W1st[smult][root1-1, root2-1] = W1st[smult][root2-1, root1-1] = val
+def eval_func(args, unknown_args):
 
-    sf_amfi = make_molcas_extractor(args.rassi, ("rassi", "SFS_AMFIint"))[()]
-    sf_angm = make_molcas_extractor(args.rassi, ("rassi", "SFS_angmom"))[()]
-    coords = make_molcas_extractor(
-        args.rassi, ("rassi", "center_coordinates"))[()]
+    try:
+        selected = args._selection
+    except AttributeError:
+        sys.exit("No quantity selected for evaluation!")
 
-    lvc = LVC(V0th, W1st, sf_smult=sf_smult, sf_amfi=sf_amfi, sf_angm=sf_angm,
-              coords=coords, verbose=True)
+    # Resolve coordinates
+    if args.vibration_info is not None:
+        ho = Harmonic.from_file(args.vibration_info)
+        coords = ho.mass_freq_weighted_coordinates * ANG2BOHR
+    else:
+        coords = None
 
-    lvc.to_file(args.lvc_data)
+    store_args = hpc.read_args(['store'] + unknown_args)
 
-    return
+    eval_args = (store_args, make_lvc_evaluator, selected)
+    eval_kwargs = {"order": args.order, "coords": coords,
+                   "truncate": args.truncate, "align": args.align}
+
+    if args.geom is None:
+        hpc.store_func(*eval_args, geom=None, **eval_kwargs)
+    else:
+        for geom in map(lambda file: xyzp.load_xyz(file)[1], args.geom):
+            hpc.store_func(*eval_args, geom=geom * ANG2BOHR, **eval_kwargs)
 
 
 def vib_func(args):
 
     if args.gaussian_log:
-        ho = Harmonic.from_gaussian_log(args.gaussian_log)
+
         if args.mass:
             raise ValueError("The --mass argument is not available with freq "
-                             "data read from Gaussian text output.")
+                             "data read from Gaussian text output use *.fchk!")
+
+        ho = Harmonic.from_gaussian_log(args.gaussian_log)
 
     elif args.gaussian_fchk:
         ho = Harmonic.from_gaussian_fchk(
-            args.gaussian_fchk, ext_masses=args.mass)
+            args.gaussian_fchk,
+            ext_masses=args.mass,
+            rot=args.rot,
+            trans=args.trans
+        )
 
     elif args.force_sets:
+
         ho = Harmonic.from_vasp_phonopy(
             args.poscar,
             args.force_sets,
-            supercell=args.distortion_expansion,
+            ext_masses=args.mass,
+            trans=args.trans,
+            distortion_expansion=args.distortion_expansion,
+            distortion_expansion_old=args.distortion_expansion_old,
+            distortion_cutoff=args.distortion_cutoff,
+            central_index=args.central_index,
             force_expansion=args.force_expansion,
-            ext_masses=args.mass
+            q_mesh=args.q_mesh
         )
 
-    subset = None if args.active_atoms is None else \
-        [idx - 1 for idc in args.active_atoms for idx in idc]
-
-    ho.subset_atoms(subset).to_file(args.vibration_info)
-
-    return
-
+    elif args.phonopy_hdf5:
 
-def summary_func(args):
-
-    # read spin-phonon data
-    sp_data = DistortionInfo.from_file(args.distortion_info)
+        if args.mass:
+            raise ValueError("The --mass argument is not available with phonon"
+                             " data read from phonopy hdf5 database, use "
+                             "FORCE_SETS instead!")
 
-    distortion_list = sp_data.generate_distortion_list()
-    distortion_str = ' '.join([str(d) for d in distortion_list])
+        ho = Harmonic.from_phonopy_hdf5(
+            args.poscar,
+            args.phonopy_hdf5,
+            trans=args.trans,
+            distortion_expansion=args.distortion_expansion,
+            distortion_expansion_old=args.distortion_expansion_old,
+            distortion_cutoff=args.distortion_cutoff,
+            central_index=args.central_index
+        )
 
-    distortion_count = len(distortion_list)
+    if args.active_atoms is not None:
+        idc = [idx - 1 for idc in args.active_atoms for idx in idc]
+        ho = ho.subset_atoms(active_atom_idc=idc)
+
+    elif args.ref_coordinates is not None:
+        _, coords = xyzp.load_xyz(args.ref_coordinates)
+        ho = ho.subset_atoms(ref_coords=coords)
 
-    if args.count:
-        print(distortion_count)
+    ho.to_file(args.vibration_info, store_vecs=args.store_vecs)
 
-    elif args.distortions:
-        print(distortion_str)
-
-    else:
-        print("Number of distortion calculations: {}".format(distortion_count))
-        print("Distortion list: {}".format(distortion_str))
+    if args.save_pyvibms is not None:
+        ho.to_pyvibms(args.save_pyvibms)
 
     return
 
 
-def prepare_func(args, unknown_args):
+def prepare_func(args):
 
     if args.program == 'tau':
         # CFP args
-        if args.lvc_data:
-            cfp_args = angmom_suite.read_args(['cfp'] + unknown_args)
-            cfp_args.theta = True
-            cfp_args.space = cfp_args.space or cfp_args.ion.casscf_terms('s')
-            cfp_args.symbol = cfp_args.symbol or {
-                'l': cfp_args.ion.ground_term,
-                'j': cfp_args.ion.ground_level
-                }[cfp_args.basis]
-            func_kwargs = vars(cfp_args)
+        proj_kwargs = {
+            'model_space': args.ground_level,
+            'quax': args.quax,
+            'terms': {"cf": [('J',)]},
+            'k_max': args.k_max,
+            'theta': True,
+            'ion': args.ion
+        }
 
-        else:
-            func_kwargs = {}
+        # EQ_CFPs.dat
+        cfp_eq = LVCModelHamiltonian(LVC.from_file(args.lvc_data), 0,
+                                     **proj_kwargs)[("cf", "J")]
 
-        # derivative args
-        setattr(args, 'function', 'CFPs')
-        setattr(args, 'zpd_unit', True)
-        setattr(args, 'order', 1)
-        setattr(args, 'max_analytic_order', None)
-        setattr(args, 'format', 'tau')
+        cfp_data = np.column_stack(
+            (np.ones(27), list(cfp_eq.keys()), list(cfp_eq.values())))
 
-        # EQ_CFPs.dat
-        kq_idc = angmom_suite.crystal.stevens_kq_indices[:27]
-        cfp_vals = make_func(args, **func_kwargs)(Distortion(), Dx())
-        cfp_data = np.column_stack((np.ones(27), kq_idc, cfp_vals))
         np.savetxt('EQ_CFPs.dat', cfp_data,
                    fmt=['%2d', '%2d', '% 2d', '%16.8f'])
 
-        # CFP_derivatives.dat
-        derivatives_func(args, **func_kwargs)
-
         # mode_energies.dat
         ho = Harmonic.from_file(args.vibration_info)
         np.savetxt('mode_energies.dat', ho.freqs, fmt='%16.8f',
                    header="Frequency (cm-1)", comments='')
 
+        cfp_dq = LVCModelHamiltonian(
+            LVC.from_file(args.lvc_data), 1,
+            coords=ho.mass_freq_weighted_coordinates * ANG2BOHR,
+            **proj_kwargs
+        )
+
+        print_tau_style(filter(lambda pars: pars[0][1] == 'cf', iter(cfp_dq)),
+                        ho.freqs, 'CFP_polynomials.dat')
+
+    elif args.program == 'tau_direct':
+
+        ho = Harmonic.from_file(args.vibration_info)
+        np.savetxt('mode_energies.dat', ho.freqs, fmt='%16.8f',
+                   header="Frequency (cm-1)", comments='')
+
+        lvc = LVC.from_file(args.lvc_data)
+
+        ener = LVCAdiabaticEnergies(lvc, 0, soc=True,
+                                    truncate=args.truncate)[()]
+
+        nstates = args.truncate or ener.size
+
+        couplings = LVCDiabaticHamiltonian(lvc, 1, 
+            coords=ho.mass_freq_weighted_coordinates * ANG2BOHR,
+            soc=True, truncate=nstates)
+
+        with h5py.File('tau.hdf5', 'w') as h, open('coupling_strength.dat', 'w') as f:
+
+            h.create_dataset('energies', data=(ener - ener[0]) * HARTREE2INVCM)
+
+            grp = h.create_group("couplings")
+
+            for modes, lin in iter(couplings):
+
+                cplg = lin * HARTREE2INVCM
+
+                if args.trace_less:
+                    cplg -= np.identity(nstates) * np.trace(cplg) / nstates
+
+                grp.create_dataset('_'.join(map(str, modes)), data=cplg)
+                strength = np.sum((cplg * cplg.conj()).real)
+                f.write(f'{strength}\n')
+
+            angm_grp = h.create_group('angmom')
+            spin_grp = h.create_group('spin')
+
+            for idx, comp in enumerate(["x", "y", "z"]):
+                idc = np.ix_(range(nstates), range(nstates))
+                angm_grp.create_dataset(comp, data=lvc.sos_angm[idx][idc])
+                spin_grp.create_dataset(comp, data=lvc.sos_spin[idx][idc])
+
     return
 
 
-def gen_charges_func(args):
+def charges_func(args):
     """
-    Wrapper function for cli call to gen_charges
+    Wrapper function for cli call to charges
     """
 
-    scell = cells.SuperCell.from_poscar(args.poscar, args.distortion_expansion)
+    structure = Structure.from_file(args.poscar)
+    equivalent_positions, elements, mappings, entities = \
+        cells.get_unique_entities(structure)
+
+    if args.gen:
+        gen_charges_func(entities)
+    elif args.parse:
+        parse_charges_func(equivalent_positions, elements, mappings, entities)
+    else:
+        ValueError(f"{args.mode} mode not supported!")
+
+
+def format_formula(formula):
+    return formula.replace(" ", "")
 
-    xyzp.save_xyz(
-        "supercell.xyz", scell.atom_labels, scell.cart_coords, verbose=False
-    )
-    print()
-    print("Supercell written to supercell.xyz")
+
+def gen_charges_func(entities):
+    """
+    Wrapper function for cli call to charges gen
+    """
 
     print("******************************")
     print("The unique entities are")
-    for formula, indices in scell.asu_entities.items():
-        print(formula)
+    for mol in entities:
+        print(mol.formula)
+        mol.to(f"{format_formula(mol.formula)}.xyz")
     print("******************************")
 
-    asu_indices = np.unique(scell.symmetry["equivalent_atoms"])
-
-    xyzp.save_xyz(
-        "unique_entities.xyz",
-        scell.atom_labels[asu_indices],
-        (scell.cart_coords + scell.repair_shifts)[asu_indices],
-        verbose=False
-    )
-    print("Unique entities written to unique_entities.xyz\n")
-
-    if len(asu_indices) < len(cells.flatten(scell.asu_entities.values())):
-        print("\033[31m             ****Warning****") # noqa
-        print("      High symmetry entity detected")
-        print("Check calculated CHELPG charges obey symmetry \033[0m\n")
-
     # Create gaussian inputs for CHELPG calculation, one for each
     # member of the ASU
 
     # All electron aug-cc-pvtz
     ae_pvtz = [
         'H', 'Li', 'Be', 'Na', 'Mg', 'B', 'C', 'N', 'O', 'F', 'He', 'Ne', 'Al',
         'Si', 'P', 'S', 'Cl', 'Ar', 'Ga', 'Ge', 'As', 'Se', 'Br', 'Kr'
     ]
-    ae_basis = {
-        "{}".format(atoms): "aug-cc-pvtz"
-        for atoms in ae_pvtz
-    }
+    ae_basis = {atom: "aug-cc-pvtz" for atom in ae_pvtz}
 
     unsupported = [
         "K", "Ca", "Rb", "Sr", "Cs", "Ba", "Ac", "Th", "Pa", "U", "Np",
         "Pu", "Am", "Cm"
     ]
-    unsupported_basis = {
-        "{}".format(atoms): "????"
-        for atoms in unsupported
-    }
+    unsupported_basis = {atom: "????" for atom in unsupported}
 
-    for lab in scell.atom_labels[cells.flatten(scell.asu_entities.values())]:
+    for lab in (site.specie.symbol for mol in entities for site in mol.sites):
         if lab in unsupported:
-            print("\033[31m Warning, add basis for {} to .com file\033[0m \n".format(lab)) # noqa
+            print(f"\033[31m Warning, add basis for {lab} to .com file\033[0m \n")
+
     ae_basis = ae_basis | unsupported_basis
 
     # ECP
     pp_pvtz = [
         'In', 'Sn', 'Sb', 'Te', 'I', 'Xe', 'Tl', 'Pb', 'Bi', 'Po', 'At', 'Rn'
     ]
-    small_pp_basis = {
-        "{}".format(atoms): "aug-cc-pvtz-pp"
-        for atoms in pp_pvtz
-    }
-
-    stuttgart = {
-        "{}".format(metals): "stuttgart rsc 1997"
-        for metals in atomic.lanthanides + atomic.transition_metals
-    }
+    small_pp_basis = {atom: "aug-cc-pvtz-pp" for atom in pp_pvtz}
+
+    stuttgart = {metal: "stuttgart rsc 1997"
+                 for metal in atomic.lanthanides + atomic.transition_metals}
 
     psuedo = small_pp_basis | stuttgart
 
     try:
         os.mkdir("gaussian")
     except OSError:
         pass
 
-    for formula, indices in scell.asu_entities.items():
+    for idx, mol in enumerate(entities, start=1):
         gsgi.gen_input(
-            "gaussian/{}.com".format(formula),
-            scell.atom_labels[indices],
-            (scell.cart_coords+scell.repair_shifts)[indices],
+            f"gaussian/{format_formula(mol.formula)}_{idx}.com",
+            list(map(lambda site: site.specie.symbol, mol.sites)),
+            list(map(lambda site: (site.x, site.y, site.z), mol.sites)),
             99,
             99,
             method="PBE",
             bs_spec=ae_basis,
             ecp_spec=psuedo,
             opt=False,
             freq=False,
-            extra_title="{}".format(formula),
+            extra_title=f"{format_formula(mol.formula)} (molecule #{idx})",
             chelpg="charge"
         )
         print()
 
     print("\033[93mCharge and multiplicity set to 99 in all .com files")
     print("Please replace with actual values before submitting \033[0m \n")
 
-    # Store supercell object in pickle for next step
-    with open("supercell.pickle", 'wb') as _file:
-        pickle.dump(scell, _file)
-
-    print(
-        "\033[0;32mSupercell object pickled in supercell.pickle \033[0m"
-    )
     return
 
 
-def parse_charges_func(args):
+def parse_charges_func(equivalent_positions, elements, mappings, entities):
     """
-    Wrapper function for cli call to parse_charges
+    Wrapper function for cli call to charges parse
     """
 
-    # Load cell object from gen_charges
-    with open(args.supercell_pickle, 'rb') as _file:
-        scell: cells.Cell = pickle.load(_file)
+    def read_charges(mol, idx):
+        file = f"gaussian/{format_formula(mol.formula)}_{idx}.log"
+        return np.array(gscd.get_chelpg_charges(file))
+
+    def symmetrize(mapping, charges):
+        for val in np.unique(mapping):
+            for idc in np.flatnonzero(mapping == val):
+                yield val, np.mean(charges[idc])
+
+    def neutralize(charges):
+        return np.array(charges) - np.mean(charges)
+
+    mol_mappings = enumerate(zip(mappings, entities), start=1)
+    atomic_charges = {idx: chrg for mol_idx, (mapping, mol) in mol_mappings
+                      for idx, chrg in symmetrize(mapping, read_charges(mol, mol_idx))}
 
-    if args.calc_dir.lower() != 'cwd':
-        calc_dir = "{}/".format(args.calc_dir)
-    else:
-        calc_dir = ""
+    unitcell_charges = neutralize([
+        atomic_charges[pos] for pos in equivalent_positions])
 
-    asu_charges = {
-        head: gscd.get_chelpg_charges("{}/{}.log".format(calc_dir, head))
-        for head in scell.asu_entities.keys()
-    }
-
-    index_to_charge = {
-        index: charge
-        for head in scell.asu_entities.keys()
-        for index, charge in zip(scell.asu_entities[head], asu_charges[head])
-    }
+    np.savetxt("charges.dat", unitcell_charges)
 
-    supercell_charges = [
-        index_to_charge[index] for index in scell.symmetry['equivalent_atoms']
-    ]
-    _min_charge = np.min(supercell_charges)
-    _max_charge = np.max(supercell_charges)
-    _charge_spread = _max_charge - _min_charge
-
-    if args.vis_charges in ["entities", "all"]:
-
-        viewers = []
-
-        for it, indices in enumerate(scell.asu_entities.values()):
-            # Get charge of current entity
-            _charges = [supercell_charges[ind] for ind in indices]
-            # Get labels and coords, and shift centre of mass to origin
-            # so that interactive plot can be manipulated easily by user
-            _labels = scell.atom_labels[indices]
-            _coords = (scell.cart_coords+scell.repair_shifts)[indices]
-            _coords -= xyzp.calculate_com(_labels, _coords)
-
-            # Create Viewer object for current entity
-            _tmp = cells.vis_charges_viewer(
-                coords=_coords,
-                labels=_labels,
-                norm_charges=(_charges - _min_charge)/_charge_spread,
-                viewer_style_args={
-                    "height": "{}vh".format(95/len(asu_charges.keys())),
-                    "width": "95vw"
-                },
-                viewer_div_args={
-                    "div_id": "viewer_{:d}".format(it+1)
-                }
-            )
-            viewers.append(_tmp)
-        
-        # Create webpage containing one viewer per entity with 
-        # headers specifiying charge and colours
-        body = [
-            "<P> Maximum negative charge is {:f} e (Blue) </P>".format(
-                _min_charge
-            ),
-            "<P> Maximum positive charge is {:f} e (Red) </P>".format(
-                _max_charge
-            ),
-            "<P> Right click image to save </P>"
-        ]
-        body += [viewer.div for viewer in viewers]
-        page = mvis.HtmlPage(
-            scripts=[viewer.script for viewer in viewers],
-            body=body
-        )
-        page.save("entities.html")
-        print("\n\033[0;32mEntity charges can be visualised in entities.html\033[0m\n")
+    # Make molcas basis file for environment charges
+    cells.write_molcas_basis(
+        elements, dict(enumerate(unitcell_charges, start=1)), "ENV")
 
-    central_atom = args.central_atom
-    central_formula = args.central_formula
+    print("\033[93m")
+    print("Molcas basis set file for environment written to:")
+    print("     ENV (basis set specification)\033[0m")
 
-    # Pick user defined entity and move to centre of cell
-    central_indices, without_central_indices = scell.find_centre_indices(
-        central_formula=central_formula
-    )
 
-    catind = np.where(scell.atom_labels[central_indices] == central_atom)[0][0]
-    catind = central_indices[catind]
+def cluster_func(args):
 
-    # Periodically recentre coordinates at central_formula
-    scell.shift_centre_to(scell.frac_coords[catind])
+    structure = Structure.from_file(args.poscar)
+    central_index = args.central_index
+    central_index_unit = (central_index - 1) % structure.num_sites
+
+    if args.from_central:
+        molecular_graph = cells.generate_molecular_graph(structure)
+        connected_graphs = cells.split_molecular_graph(molecular_graph, filter_unique=False)
+        central_graph = next(filter(lambda nodes: central_index_unit in nodes, connected_graphs))
+        _, qm_region = cells.extract_molecule(structure, central_graph, central_index=central_index_unit)
+    elif args.qm_region is not None:
+        _, qm_region = Molecule.from_file(args.qm_region)
+    else:
+        raise NotImplementedError()
 
-    xyzp.save_xyz(
-        "central_o_shifted.xyz",
-        scell.atom_labels[central_indices],
-        scell.cart_coords[central_indices]
-    )
+    central_site = structure.sites[central_index_unit]
+    shift = np.array([central_site.x, central_site.y, central_site.z])
 
-    xyzp.save_xyz(
-        "environment_o_shifted.xyz",
-        scell.atom_labels[without_central_indices],
-        scell.cart_coords[without_central_indices]
-    )
+    cluster = cells.build_cluster(args.poscar, central_index=central_index,
+                                  distortion_expansion=args.distortion_expansion,
+                                  distortion_expansion_old=args.distortion_expansion_old,
+                                  distortion_cutoff=args.distortion_cutoff)
 
-    # Make molcas basis file for environment charges
-    _charges = [
-        supercell_charges[wci] for wci in without_central_indices
-    ]
-    _coords = scell.cart_coords[without_central_indices]
-    _labels = scell.atom_labels[without_central_indices]
+    def format_label(args):
+        idx, specie = args
+        return f"{specie.symbol}.ENV.{idx}"
 
-    cells.make_molcas_basis_and_xyz(_labels, _coords, _charges)
-    print("\033[93m")
-    print("Molcas files for environment written to:")
-    print("     ENV (basis set specification)")
-    print("     molcas_environment.xyz (environment coordinates, use with molcas_suite generate_input --basis_xyz) \033[0m") # noqa
-
-    np.savetxt(
-        "environment_charges.dat",
-        _charges
-    )
-
-    if args.vis_charges in ["supercell", "all"]:
-
-        viewer = cells.vis_charges_viewer(
-            coords=_coords,
-            labels=_labels,
-            norm_charges=(_charges - _min_charge)/_charge_spread,
-            extra_coords=scell.cart_coords[central_indices],
-            extra_labels=scell.atom_labels[central_indices],
-            extra_color='#000000',
-            viewer_style_args={
-                "width":"95vw"
-            },
-            main_kwargs={"atom_opacities":0.5}
-        )
-        body = [
-            "<P> Maximum negative charge is {:f} e (Blue) </P>".format(_min_charge),
-            "<P> Maximum positive charge is {:f} e (Red) </P>".format(_max_charge),
-            "<P> Right click image to save </P>",
-            viewer.div
-        ]
-        page = mvis.HtmlPage(
-            scripts=[viewer.script],
-            body=body
-        )
+    labels = list(map(format_label, enumerate(structure.species, start=1))) * cluster.n_cell
 
-        page.save("supercell.html")
-        print("\n\033[0;32mSupercell charges can be visualised in supercell.html\033[0m") #noqa
+    def generate_mapping(ref_coords):
 
-    return
+        for idx, site in enumerate(qm_region.sites):
+
+            coord = np.array([site.x, site.y, site.z]) - shift
+            idc = np.flatnonzero(np.isclose(ref_coords, coord).all(axis=1))
+
+            if len(idc) == 0:
+                continue
+            elif len(idc) == 1:
+                yield idc[0]
+            else:
+                raise ValueError(f"Multiple instances of atom {coord}!")
+
+    for idx in generate_mapping(cluster.cart_coords):
+        labels[idx] = labels[idx].split('.')[0]
+
+    xyzp.save_xyz("cluster.xyz", labels, cluster.cart_coords)
 
 
 def derivatives_func(args, unknown_args=None, **func_kwargs):
 
     if args.method == "findiff":
         dx = Finite.from_file(args.distortion_info)
 
@@ -517,40 +502,35 @@
     # parse_range and a custom action which flattens, check also other uses of
     # parse_range if flattened
 
     # todo: replace dict by global definition
     roots_dict = {'dy': [18]}
 
     if args.num_roots:
-        num_roots = [int(n) for n in args.num_roots]
+        num_roots = map(int, args.num_roots)
     elif args.ion:
         num_roots = roots_dict[args.ion.lower()]
     else:
         sys.exit("Invalid specification of the number of roots.")
 
-    iph_idc = range(1, len(num_roots) + 1) \
-        if args.jobiph is None else [int(i) for i in args.jobiph]
+    for iph_idx, num_root in enumerate(num_roots, start=1):
 
-    for num_root, iph_idx in zip(num_roots, iph_idc):
-        if args.dry:
-            input_name = r"lvc_root{:0" + str(len(str(num_root))) + r"}"
-            print(
-                ' '.join(
-                    [input_name.format(i) for i in range(1, num_root + 1)]
-                )
-            )
-        else:
-            generate_lvc_input(
-                args.old_path,
-                args.old_project,
-                num_root,
-                iph_idx,
-                mclr_kwargs=args.mclr,
-                alaska_kwargs=args.alaska
-            )
+        if num_root == 0:
+            continue
+
+        generate_lvc_input(
+            args.old_path,
+            args.old_project,
+            num_root,
+            iph_idx,
+            mclr_extra=args.mclr_extra,
+            alaska_extra=args.alaska_extra,
+            two_step=args.two_step,
+            dry=args.dry
+        )
 
     return
 
 
 def parse_range(string):
     """
     adapted from https://stackoverflow.com/questions/6512280/accept-a-range-of-
@@ -636,229 +616,200 @@
         plt.savefig("strengths.png")
         print("Strength plots saved to strengths.svg and strengths.png")
         plt.show()
 
     return
 
 
+cluster = ArgumentParser(
+        formatter_class=RawDescriptionHelpFormatter,
+        add_help=False
+)
+
+morph = cluster.add_mutually_exclusive_group()
+
+morph.add_argument(
+    '--distortion_expansion',
+    nargs=3,
+    metavar=('N_x', 'N_y', 'N_z'),
+    type=int,
+    help='Supercell expansion.'
+)
+
+morph.add_argument(
+    '--distortion_expansion_old',
+    nargs=3,
+    metavar=('N_x', 'N_y', 'N_z'),
+    type=int,
+    help='Supercell expansion in the old convention.'
+)
+
+morph.add_argument(
+    '--distortion_cutoff',
+    type=float,
+    help='Cut-off distance for unit cell cluster.'
+)
+
+cluster.add_argument(
+    '--central_index',
+    type=int,
+    help='Index of the central spin center.'
+)
+
+
 def read_args(arg_list=None):
     description = '''
     A package for performing Spin-Phonon coupling calculations.
     '''
 
     parser = ArgumentParser(
             description=description,
             formatter_class=RawDescriptionHelpFormatter
             )
 
     subparsers = parser.add_subparsers(dest='prog')
 
-    distort = subparsers.add_parser('generate_distortion')
-    distort.set_defaults(func=generate_distortion_func)
-
-    distort.add_argument(
-        'input',
-        type=str,
-        help='Input file containing the xyz-coordinates of the equilibrium structure.' # noqa
-    )
-
-    distort.add_argument(
-        'output',
-        type=str,
-        help='Output file containing the xyz-coordinates of the distorted structure.' # noqa
-    )
-
-    distort.add_argument(
-        '-D',
-        '--distortion_info',
-        type=str,
-        help='HDF5 database file containing the normal mode displacement vectors.' # noqa
-    )
-
-    distort.add_argument(
-        '--origin',
-        type=str,
-        help='Label of atom which stays fixed at the origin during distortion.'
-    )
-
-    distort.add_argument(
-        '-d',
-        '--distortion',
-        required=True,
-        type=Distortion.parse,
-        help='Tuple consisting of <direction> (pos|neg) / <step_num> / <mode_index> ...' # noqa
-    )
+    coords = subparsers.add_parser('coords')
+    coords.set_defaults(func=coords_func)
 
-    init = subparsers.add_parser('init')
-    init.set_defaults(func=init_func)
-
-    init.add_argument(
+    coords.add_argument(
         '-D',
         '--distortion_info',
         type=str,
         help='HDF5 database containing information about the distortion.'
     )
 
-    init.add_argument(
+    coords.add_argument(
         '--num_atoms',
         type=int,
         default=1,
         help='Number of atoms.'
     )
 
-    init.add_argument(
-        '--freq_gaussian',
-        type=str,
-        help='Gaussian output containing the normal mode information.'
-    )
-
-    init.add_argument(
+    coords.add_argument(
         '--mode_wise',
         nargs='*',
         default=None,
         type=parse_range,
         help='Mode indices to be included in distortions calculations ' +
              '- activates mode-wise distortions.'
         )
 
-    init.add_argument(
+    coords.add_argument(
         '--atomic',
         nargs='*',
         default=None,
         type=parse_range,
         help='Atomic indices to be included in distortion calculations ' +
              '- activates atomic distortions.'
         )
 
-    init.add_argument(
+    coords.add_argument(
         '--num_steps',
         type=int,
         default=0,
         help='Number of distortion steps.'
     )
 
-    init.add_argument(
+    coords.add_argument(
         '--order',
         type=int,
         default=1,
         help='Order of distortion.'
     )
 
-    init.add_argument(
+    coords.add_argument(
         '--constant_step',
         type=float,
         help='Step size factor for constant displacement.'
     )
 
-    info = subparsers.add_parser('summary')
-    info.set_defaults(func=summary_func)
-
-    info.add_argument(
-        '-D',
-        '--distortion_info',
-        help='HDF5 database containing the spin-phonon information.'
-    )
-
-    select = info.add_mutually_exclusive_group(required=True)
-
-    select.add_argument(
-        '--distortions',
-        default=False,
-        action='store_true',
-        help='Print list of distortions.'
-    )
-
-    select.add_argument(
-        '--count',
-        default=False,
-        action='store_true',
-        help='Print number of distortions.'
-    )
-
-    derive = subparsers.add_parser('derivatives')
-    derive.set_defaults(func=derivatives_func)
+    evaluate = subparsers.add_parser('eval')
+    evaluate.set_defaults(func=eval_func)
 
-    derive.add_argument(
+    evaluate.add_argument(
         '-H',
         '--Help',
         action=FunctionHelp,
         help='show help message for additional arguments and exit'
     )
 
-    derive.add_argument(
-        'function',
-        type=str,
-        help='Function to derive.'
-    )
-
-    derive.add_argument(
-        '--method',
-        type=str,
-        default="findiff",
-        choices=["findiff", "polynomial"],
-        help='Differentiation method'
-    )
-
-    evaluation = derive.add_mutually_exclusive_group(required=True)
-
-    evaluation.add_argument(
-        '-G',
-        '--grid_data',
-        type=str,
-        help='HDF5 database containing the function values at distorted geometries.' # noqa
-    )
-
-    evaluation.add_argument(
+    evaluate.add_argument(
         '-L',
         '--lvc_data',
         type=str,
         help='HDF5 database containing the LVC parameters.'
     )
 
-    derive.add_argument(
+    coords = evaluate.add_mutually_exclusive_group()
+
+    coords.add_argument(
         '-V',
         '--vibration_info',
         type=str,
-        help='HDF5 database containing information about the vibrations.'
+        help=('HDF5 database containing information about the vibrations.'
+              'Derivatives are evaluated in the basis of dimension-less'
+              'mass-frequency weighted normal mode coordinates.')
     )
 
-    derive.add_argument(
-        '-D',
-        '--distortion_info',
-        type=str,
-        help='HDF5 database containing the distortion information.'
+    evaluate.add_argument(
+        '--geom',
+        nargs='+',
+        help='*.xyz coordinates at which properties will be evaluated.'
     )
 
-    derive.add_argument(
+    evaluate.add_argument(
         '--order',
         type=int,
-        default=1,
+        default=0,
         help='Order of derivative.'
     )
 
-    derive.add_argument(
-        '--max_analytic_order',
+    evaluate.add_argument(
+        '--truncate',
         type=int,
-        help=(
-            'Maximum analytic derivative order available for function.'
-            'Defaults to 0 for grid data and 1 for LVC function data.'
-        )
+        metavar="max_state",
+        help='Truncate matrix elements at max_state'
     )
 
-    derive.add_argument(
-        '--format',
-        choices=['tau', 'points'],
-        help='Output in <CFP_polynomials.dat> style.'
+    evaluate.add_argument(
+        '--align',
+        action=BooleanOptionalAction,
+        default=True,
+        help='Align LVC model reference to input geometry by minimising RMSD.'
     )
 
-    derive.add_argument(
-        '--zpd_unit',
-        default=False,
-        action='store_true',
-        help='Convert to units of zero point displacement.'
+    evaluate.add_argument(
+        '--adiabatic_energies',
+        nargs='+',
+        action=OrderedSelectionAction,
+        choices=['mch', 'soc'],
+        help='Energies of the MCH or SOC eigenstates.'
+    )
+
+    evaluate.add_argument(
+        '--diabatic_hamiltonian',
+        nargs='+',
+        action=OrderedSelectionAction,
+        choices=['mch', 'soc'],
+        help='Diabatic potential energy matrix between MCH or SOC states.'
+    )
+
+    evaluate.add_argument(
+        '--proj',
+        nargs='+',
+        action=OrderedSelectionAction,
+        help='Model Hamiltonian projection'
+    )
+
+    evaluate.add_argument(
+        '--sus',
+        nargs='+',
+        action=OrderedSelectionAction,
+        help='Magnetic susceptibility'
     )
 
     inp = subparsers.add_parser('generate_input')
     inp.set_defaults(func=generate_lvc_input_func)
 
     inp.add_argument(
         'old_project',
@@ -890,68 +841,157 @@
     inp.add_argument(
         '--jobiph',
         nargs='+',
         help='Indices of Molcas JOBIPH wavefunction files *_IPH.'
     )
 
     inp.add_argument(
-        '--mclr',
+        '--mclr_extra',
         nargs='+',
-        default=None,
-        type=parse_dict_key_only,
-        action=ParseKwargs,
+        default=((), {}),
+        type=make_parse_dict(str, str, key_only=True),
+        action=ParseExtra,
         help='Manually run mclr with custom options, e.g. thre=1e-8',
         metavar='name=value')
 
     inp.add_argument(
-        '--alaska',
+        '--alaska_extra',
         nargs='+',
-        default=None,
-        type=parse_dict_key_only,
-        action=ParseKwargs,
+        default=((), {}),
+        type=make_parse_dict(str, str, key_only=True),
+        action=ParseExtra,
         help='Run alaska with custom options, e.g. cuto=1e-8',
         metavar='name=value')
 
     inp.add_argument(
+        '--two_step',
+        action=BooleanOptionalAction,
+        default=True,
+        help='Utilize two-step procedure for MCLR runs'
+    )
+
+    inp.add_argument(
         '--dry',
         default=False,
         action='store_true',
         help='Dry-run which prints files to be created'
     )
 
     lvc = subparsers.add_parser('lvc')
     lvc.set_defaults(func=lvc_func)
 
     lvc.add_argument(
-        '-D', '--distortion_info',
-        type=str,
-        help='HDF5 database containing information about the distortion.'
-    )
-
-    lvc.add_argument(
         '-L', '--lvc_data',
         type=str,
         help='HDF5 database output containing the LVC data.'
     )
 
-    lvc.add_argument(
+    grad = lvc.add_mutually_exclusive_group()
+
+    grad.add_argument(
         '--grad',
         type=str,
         nargs='+',
         help='Molcas output file(s) containing gradients and NACs.'
     )
 
+    grad.add_argument(
+        '--efld',
+        type=str,
+        nargs='+',
+        help='Molcas output file(s) containing electric field values.'
+    )
+
+    grad.add_argument(
+        '--add',
+        type=str,
+        nargs='+',
+        help='LVC HDF5 data bases to be added.'
+    )
+
+    frozen = lvc.add_argument_group('Frozen density gradient arguments')
+
+    frozen.add_argument(
+        '--charge',
+        type=str,
+        nargs='+',
+        help='Text file(s) containing point charge values.'
+    )
+
+    frozen.add_argument(
+        '--xyz',
+        type=str,
+        nargs='+',
+        help='xyz file(s) containing point charge coordinates.'
+    )
+
+    add = lvc.add_argument_group('LVC addition arguments')
+
+    add.add_argument(
+        '--reference_xyz',
+        type=str,
+        help='xyz file containing the reference coordinates.'
+    )
+
     lvc.add_argument(
         '--rassi',
         type=str,
         help=('Molcas *.rassi.h5 output file containing AMFI integrals, '
               'SF_ANGMOM operators and the spin multiplicities.')
     )
 
-    vibrate = subparsers.add_parser('vib')
+    subset = lvc.add_mutually_exclusive_group()
+
+    subset.add_argument(
+        '--active_atoms',
+        nargs='+',
+        type=parse_range,
+        help=(
+            'Atomic indices active during spin-phonon coupling. Effectively '
+            'effectively setting the coupling of all other atoms to zero. '
+            'Useful to suppress coupling of specific atoms.'
+        )
+    )
+
+    subset.add_argument(
+        '--ref_coordinates',
+        help='xyz coordinates containing the atomic positions of active atoms.'
+    )
+
+    lvc.add_argument(
+        '--verbose',
+        action='store_true',
+        help='Plot gradient norm and invariance measures.'
+    )
+
+    build = subparsers.add_parser('cluster', parents=[cluster])
+    build.set_defaults(func=cluster_func)
+
+    build.add_argument(
+        '--poscar',
+        type=str,
+        help='Unit cell POSCAR.'
+    )
+
+    qm = vib_calc_excl = build.add_mutually_exclusive_group(required=True)
+
+    qm.add_argument(
+        '--from_central',
+        action='store_true',
+        help=('QM region is built by completing the molecule around the '
+              'central index.')
+    )
+
+    qm.add_argument(
+        '--qm_region',
+        type=str,
+        help='Coordinates of the QM-region.'
+    )
+
+    vibrate = subparsers.add_parser('vib', parents=[cluster])
     vibrate.set_defaults(func=vib_func)
 
     vibrate.add_argument(
         '-V', '--vibration_info',
         type=str,
         help='HDF5 database containing information about the vibrations.'
     )
@@ -972,45 +1012,53 @@
 
     vib_calc_excl.add_argument(
         '--force_sets',
         type=str,
         help='FORCE_SETS file from VASP-phonopy pre-process.'
     )
 
+    vib_calc_excl.add_argument(
+        '--phonopy_hdf5',
+        type=str,
+        help='Phonon database from phono3py calculation.'
+    )
+
     vibrate.add_argument(
         '--poscar',
         type=str,
         help='Unit cell POSCAR from VASP-phonopy pre-process.'
     )
 
     vibrate.add_argument(
-        '--distortion_expansion',
+        '--force_expansion',
         nargs=3,
         metavar=('N_x', 'N_y', 'N_z'),
+        default=(1, 1, 1),
         type=int,
-        help='Supercell expansion.'
+        help='Supercell expansion used in phonon calculation'
     )
 
-    vibrate.add_argument(
-        '--force_expansion',
+    qpoints = vibrate.add_mutually_exclusive_group()
+
+    qpoints.add_argument(
+        '--q_mesh',
         nargs=3,
         metavar=('N_x', 'N_y', 'N_z'),
-        default=(1, 1, 1),
         type=int,
-        help='Supercell expansion used in phonon calculation'
+        help='Mesh in q-space for phonon evaluation.'
     )
 
     vibrate.add_argument(
         '--mass',
-        type=parse_dict,
+        type=make_parse_dict(str_int, float),
         default={},
         nargs='+',
         action=ParseKwargs,
-        help='Modify atomic masses for isotopic substitiution.',
-        metavar='atom_index=mass'
+        help='Modify atomic masses for isotopic substitution.',
+        metavar='atom_index=mass or element_symbol=mass'
     )
 
     vibrate.add_argument(
         '--trans',
         action=BooleanOptionalAction,
         default=True,
         help='Project out three rigid body translations.'
@@ -1019,135 +1067,132 @@
     vibrate.add_argument(
         '--rot',
         action=BooleanOptionalAction,
         default=True,
         help='Project out three rigid body rotations.'
     )
 
-    vibrate.add_argument(
+    subset = vibrate.add_mutually_exclusive_group()
+
+    subset.add_argument(
         '--active_atoms',
-        nargs='*',
+        nargs='+',
         type=parse_range,
         help=(
             'Atomic indices active during spin-phonon coupling. Effectively'
             ' subsets the displacement vectors. Useful if coupling is '
             'evaluated with a subset of the atoms present in the vibrational'
             ' calculation.'
         )
     )
 
+    subset.add_argument(
+        '--ref_coordinates',
+        help='xyz coordinates containing the atomic positions of active atoms.'
+    )
+
+    vibrate.add_argument(
+        '--save_pyvibms',
+        type=str,
+        help='optional pyvibms output for visualisation in PyMol.'
+    )
+
+    vibrate.add_argument(
+        '--store_vecs',
+        action=BooleanOptionalAction,
+        default=True,
+        help='Flag to disable expensive storage of normal mode displacements.'
+    )
+
     prepare = subparsers.add_parser('prep')
     prepare.set_defaults(func=prepare_func)
 
     prepare.add_argument(
         'program',
-        choices=['tau'],
+        choices=['tau', 'tau_direct'],
         help='Program for which to prepare inputs.'
     )
 
     data = prepare.add_argument_group('database files')
 
     data.add_argument(
-        '-G', '--grid_data',
-        help=('HDF5 database containing the function values at distorted '
-              'geometries.')
-    )
-
-    data.add_argument(
         '-L', '--lvc_data',
         help='HDF5 database containing the LVC parameters.')
 
     data.add_argument(
         '-V', '--vibration_info',
         help='HDF5 database containing information about the vibrations.')
 
-    data.add_argument(
-        '-D', '--distortion_info',
-        help='HDF5 database containing the distortion information.')
-
     prepare.add_argument(
-        '--method',
-        type=str,
-        default="findiff",
-        choices=["findiff", "polynomial"],
-        help='Differentiation method'
+        '--ground_level',
+        type=Level.parse,
+        help='Symbol of the model space.'
     )
 
-    gen_charges = subparsers.add_parser(
-        "gen_charges",
-        description="""
-        Creates inputs for Gaussian CHELPG charge calculations of each
-        entity in the asymmetric unit of a VASP optimised structure
-        """)
-    gen_charges.set_defaults(func=gen_charges_func)
-
-    gen_charges.add_argument(
-        "poscar",
-        type=str,
-        help='Poscar containing optimised geometry'
+    prepare.add_argument(
+        '--ion',
+        type=Ion.parse,
+        help='Central ion.'
     )
 
-    gen_charges.add_argument(
-        "distortion_expansion",
+    prepare.add_argument(
+        '--k_max',
         type=int,
-        nargs=3,
-        help=(
-            "Expansion used to generate supercell for spin phonon coupling"
-            "calculations"
-        )
+        default=6,
+        help='Maximum Stevens operator rank.'
     )
 
-    parse_charges = subparsers.add_parser(
-        "parse_charges",
-        description=(
-            "Collects result of Gaussian CHELPG charge calculations and maps"
-            "charges back onto supercell coordinates."
-        )
+    prepare.add_argument(
+        '--quax',
+        action=angmom_suite.QuaxAction,
+        help='Quantisation axes.'
     )
-    parse_charges.set_defaults(func=parse_charges_func)
 
-    parse_charges.add_argument(
-        "central_formula",
-        type=str,
-        help=(
-            "Formula of central SMM or entity"
-            "must match one of those given by gen_charges"
-        )
+    prepare.add_argument(
+        '--truncate',
+        type=int,
+        metavar="max_state",
+        help='Truncate matrix elements at max_state'
     )
 
-    parse_charges.add_argument(
-        "central_atom",
-        type=str,
-        help='Central of central_formula, e.g. Dy'
+    prepare.add_argument(
+        '--trace_less',
+        action=BooleanOptionalAction,
+        default=True,
+        help='Substract out trace from bare coupling elements.'
     )
 
-    parse_charges.add_argument(
-        "--supercell_pickle",
+    charges = subparsers.add_parser(
+        "charges",
+        description="""
+        Creates inputs for Gaussian CHELPG charge calculations of each
+        entity in the unit cell of a VASP optimised structure and
+        collects the resulting charges
+        """)
+
+    charges.set_defaults(func=charges_func)
+
+    charges.add_argument(
+        "poscar",
         type=str,
-        default='supercell.pickle',
-        help='Supercell object pickle file'
+        help='Poscar containing optimised geometry'
     )
 
-    parse_charges.add_argument(
-        "--calc_dir",
-        type=str,
-        default='gaussian',
-        help=(
-            'Directory containing Gaussian .log file(s) with CHELPG charges'
-            ' set to CWD for current directory'
-        )
+    mode = charges.add_mutually_exclusive_group(required=True)
+
+    mode.add_argument(
+        "--gen",
+        action='store_true',
+        help='Generate Gaussian ChelpG inputs.'
     )
 
-    parse_charges.add_argument(
-        "--vis_charges",
-        type=str,
-        help=(
-            'Creates html file to visualise charges for entities and supercell'
-        ),
-        choices=("none", "all","supercell","entities")
+    mode.add_argument(
+        "--parse",
+        action='store_true',
+        help='Parse Gaussian ChelpG outputs.'
     )
 
     strength = subparsers.add_parser('strength')
     strength.set_defaults(func=strength_func)
 
     strength.add_argument(
         "cfp_file",
@@ -1217,15 +1262,15 @@
     # back end.
 
     # read sub-parser
     parser.set_defaults(func=lambda args: parser.print_help())
     _args, _ = parser.parse_known_args(arg_list)
 
     # select parsing option based on sub-parser
-    if _args.prog in ['derivatives', 'prep']:
+    if _args.prog in ['derivatives', 'eval']:
         args, hpc_args = parser.parse_known_args(arg_list)
         args.func(args, hpc_args)
     else:
         args = parser.parse_args(arg_list)
         args.func(args)
```

### Comparing `spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/PKG-INFO` & `spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-phonon-suite
-Version: 0.9.1
+Version: 1.0.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-0.9.1/spin_phonon_suite.egg-info/SOURCES.txt` & `spin_phonon_suite-1.0.0/spin_phonon_suite.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 README.md
 pyproject.toml
 setup.py
 spin_phonon_suite/__init__.py
 spin_phonon_suite/__version__.py
 spin_phonon_suite/cells.py
 spin_phonon_suite/cli.py
+spin_phonon_suite/coordinates.py
 spin_phonon_suite/derivative.py
-spin_phonon_suite/distortion.py
-spin_phonon_suite/func.py
 spin_phonon_suite/lvc.py
 spin_phonon_suite/vibrations.py
 spin_phonon_suite.egg-info/PKG-INFO
 spin_phonon_suite.egg-info/SOURCES.txt
 spin_phonon_suite.egg-info/dependency_links.txt
 spin_phonon_suite.egg-info/entry_points.txt
 spin_phonon_suite.egg-info/requires.txt
```

