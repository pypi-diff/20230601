# Comparing `tmp/pydra_petpvc-0.0.2.tar.gz` & `tmp/pydra_petpvc-0.0.3.tar.gz`

## Comparing `pydra_petpvc-0.0.2.tar` & `pydra_petpvc-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/.editorconfig
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/.github/dependabot.yaml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/src/pydra/tasks/petpvc/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/src/pydra/tasks/petpvc/petpvc.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/src/pydra/tasks/petpvc/utils.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/LICENSE
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/README.md
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/hatch.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/.editorconfig
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/.github/dependabot.yaml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/src/pydra/tasks/petpvc/__init__.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/src/pydra/tasks/petpvc/petpvc.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/src/pydra/tasks/petpvc/specs.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/src/pydra/tasks/petpvc/utils.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/README.md
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/hatch.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pydra_petpvc-0.0.3/PKG-INFO
```

### Comparing `pydra_petpvc-0.0.2/.github/workflows/publish.yaml` & `pydra_petpvc-0.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pydra_petpvc-0.0.2/.github/workflows/test.yaml` & `pydra_petpvc-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pydra_petpvc-0.0.2/src/pydra/tasks/petpvc/petpvc.py` & `pydra_petpvc-0.0.3/src/pydra/tasks/petpvc/petpvc.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,32 @@
 
 Iterative Yang with a 6-millimeter PSF:
 
 >>> task = PETPVC(
 ...     input_image="input.nii",
 ...     input_mask="mask.nii",
 ...     pvc_method="IY",
-...     fwhm=(6.0, 6.0, 6.0),
+...     fwhm_x=6.0,
+...     fwhm_y=6.0,
+...     fwhm_z=6.0,
 ... )
 >>> task.cmdline    # doctest: +ELLIPSIS
-'petpvc --input input.nii --mask mask.nii --output ...input_pvc.nii --pvc IY -x 6.0 -y 6.0 -z 6.0 ...'
+'petpvc --input input.nii --mask mask.nii --output ...input_pvc.nii --pvc IY ... -x 6.0 -y 6.0 -z 6.0'
 """
 
 __all__ = ["PETPVC"]
 
 from os import PathLike
-from typing import Tuple
 
 from attrs import define, field
 from pydra.engine.specs import ShellSpec, SpecInfo
 from pydra.engine.task import ShellCommandTask
 
+from .specs import FWHMSpec
+
 
 @define(kw_only=True)
 class PETPVCSpec(ShellSpec):
     """Specifications for petpvc."""
 
     input_image: PathLike = field(metadata={"help_string": "input image", "mandatory": True, "argstr": "--input"})
 
@@ -68,22 +71,14 @@
                 "MG",
                 "MG+VC",
                 "MG+RL",
             },
         }
     )
 
-    fwhm: Tuple[float, float, float] = field(
-        metadata={
-            "help_string": "FWHM of the PSF along x, y and z",
-            "mandatory": True,
-            "formatter": lambda fwhm: f"-x {str(fwhm[0])} -y {str(fwhm[1])} -z {str(fwhm[2])}",
-        }
-    )
-
     debug: bool = field(metadata={"help_string": "print debug information", "argstr": "-d"})
 
     num_iterations_for_iterative_yang: int = field(
         default=10,
         metadata={
             "help_string": "number of iterations for the iterative Yang method",
             "formatter": lambda num_iterations_for_iterative_yang, pvc_method: (
@@ -112,8 +107,8 @@
 
 
 class PETPVC(ShellCommandTask):
     """Task definition for petpvc."""
 
     executable = "petpvc"
 
-    input_spec = SpecInfo(name="Inputs", bases=(PETPVCSpec,))
+    input_spec = SpecInfo(name="Inputs", bases=(PETPVCSpec, FWHMSpec))
```

### Comparing `pydra_petpvc-0.0.2/src/pydra/tasks/petpvc/utils.py` & `pydra_petpvc-0.0.3/src/pydra/tasks/petpvc/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,54 +2,55 @@
 Utilities
 =========
 
 Produce a 4-D mask file from 3-D labels:
 
 >>> task = PVCMake4D(input_image="mask.nii")
 >>> task.cmdline    # doctest: +ELLIPSIS
-'pvc_make4d -i mask.nii -o ...mask_4D.nii'
+'pvc_make4d -i mask.nii -o ...mask_pvcmake4d.nii'
 
 Relabel an image:
 
 >>> task = PVCRelabel(
 ...     input_image="input.nii",
 ...     parcellation_file="parc.csv",
 ...     parcellation_type="DST",
 ... )
 >>> task.cmdline    # doctest: +ELLIPSIS
-'pvc_relabel -i input.nii -o ...input_relabeled.nii --parc parc.csv --type DST'
+'pvc_relabel -i input.nii -o ...input_pvcrelabel.nii --parc parc.csv --type DST'
 
 Simulate partial volume effect with blurring:
 
->>> task = PVCSimulate(input_image="input.nii", fwhm=(4.0, 4.0, 4.0))
+>>> task = PVCSimulate(input_image="input.nii", fwhm_x=4.0, fwhm_y=4.0, fwhm_z=4.0)
 >>> task.cmdline    # doctest: +ELLIPSIS
-'pvc_simulate input.nii ...input_pvcsim.nii -x 4.0 -y 4.0 -z 4.0'
+'pvc_simulate input.nii ...input_pvcsimulate.nii -x 4.0 -y 4.0 -z 4.0'
 """
 
 __all__ = ["PVCMake4D", "PVCRelabel", "PVCSimulate"]
 
 from os import PathLike
-from typing import Tuple
 
 from attrs import define, field
 from pydra.engine.specs import ShellSpec, SpecInfo
 from pydra.engine.task import ShellCommandTask
 
+from .specs import FWHMSpec
+
 
 @define(kw_only=True)
 class PVCMake4DSpec(ShellSpec):
     """Specifications for pvc_make4d."""
 
     input_image: PathLike = field(metadata={"help_string": "input 3-D mask image", "mandatory": True, "argstr": "-i"})
 
     output_image: str = field(
         metadata={
             "help_string": "output 4-D region mask image",
             "argstr": "-o",
-            "output_file_template": "{input_image}_4D",
+            "output_file_template": "{input_image}_pvcmake4d",
         }
     )
 
 
 class PVCMake4D(ShellCommandTask):
     """Task definition for pvc_make4d."""
 
@@ -61,15 +62,15 @@
 @define(kw_only=True)
 class PVCRelabelSpec(ShellSpec):
     """Specifications for pvc_relabel."""
 
     input_image: PathLike = field(metadata={"help_string": "input image", "mandatory": True, "argstr": "-i"})
 
     output_image: str = field(
-        metadata={"help_string": "output image", "argstr": "-o", "output_file_template": "{input_image}_relabeled"}
+        metadata={"help_string": "output image", "argstr": "-o", "output_file_template": "{input_image}_pvcrelabel"}
     )
 
     parcellation_file: PathLike = field(
         metadata={"help_string": "parcellation file", "mandatory": True, "argstr": "--parc"}
     )
 
     parcellation_type: str = field(metadata={"help_string": "parcellation type", "mandatory": True, "argstr": "--type"})
@@ -83,28 +84,27 @@
     input_spec = SpecInfo(name="Inputs", bases=(PVCRelabelSpec,))
 
 
 @define(kw_only=True)
 class PVCSimulateSpec(ShellSpec):
     """Specifications for pvc_simulate."""
 
-    input_image: PathLike = field(metadata={"help_string": "input image", "mandatory": True, "argstr": ""})
-
-    output_image: str = field(
-        metadata={"help_string": "output image", "argstr": "", "output_file_template": "{input_image}_pvcsim"}
+    input_image: PathLike = field(
+        metadata={"help_string": "input image", "mandatory": True, "argstr": "", "position": 0}
     )
 
-    fwhm: Tuple[float, float, float] = field(
+    output_image: str = field(
         metadata={
-            "help_string": "FWHM of the PSF along x, y and z",
-            "mandatory": True,
-            "formatter": lambda fwhm: f"-x {str(fwhm[0])} -y {str(fwhm[1])} -z {str(fwhm[2])}",
+            "help_string": "output image",
+            "argstr": "",
+            "position": 1,
+            "output_file_template": "{input_image}_pvcsimulate",
         }
     )
 
 
 class PVCSimulate(ShellCommandTask):
     """Task definition for pvc_simulate."""
 
     executable = "pvc_simulate"
 
-    input_spec = SpecInfo(name="Inputs", bases=(PVCSimulateSpec,))
+    input_spec = SpecInfo(name="Inputs", bases=(PVCSimulateSpec, FWHMSpec))
```

### Comparing `pydra_petpvc-0.0.2/.gitignore` & `pydra_petpvc-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pydra_petpvc-0.0.2/LICENSE` & `pydra_petpvc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_petpvc-0.0.2/README.md` & `pydra_petpvc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydra_petpvc-0.0.2/pyproject.toml` & `pydra_petpvc-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydra-petpvc"
-version = "0.0.2"
+version = "0.0.3"
 description = 'Pydra tasks for PETPVC'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "Apache-2.0"
 keywords = ["pydra", "pet", "petpvc", "pvc"]
 authors = [
   { name = "Ghislain Vaillant", email = "ghislain.vaillant@icm-institute.org" },
```

### Comparing `pydra_petpvc-0.0.2/PKG-INFO` & `pydra_petpvc-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydra-petpvc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pydra tasks for PETPVC
 Project-URL: Documentation, https://github.com/ghisvail/pydra-petpvc#readme
 Project-URL: Issues, https://github.com/ghisvail/pydra-petpvc/issues
 Project-URL: Source, https://github.com/ghisvail/pydra-petpvc
 Author-email: Ghislain Vaillant <ghislain.vaillant@icm-institute.org>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

