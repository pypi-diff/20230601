# Comparing `tmp/daemonflux-0.6.1.tar.gz` & `tmp/daemonflux-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daemonflux-0.6.1.tar", last modified: Mon May  8 08:50:04 2023, max compression
+gzip compressed data, was "daemonflux-0.7.0.tar", last modified: Thu Jun  1 12:50:51 2023, max compression
```

## Comparing `daemonflux-0.6.1.tar` & `daemonflux-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-08 08:49:33.000000 daemonflux-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-08 08:50:04.333390 daemonflux-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-05-08 08:49:33.000000 daemonflux-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 08:49:33.000000 daemonflux-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 08:50:04.333390 daemonflux-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.329390 daemonflux-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/src/daemonflux/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-08 08:49:33.000000 daemonflux-0.6.1/src/daemonflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21769 2023-05-08 08:49:33.000000 daemonflux-0.6.1/src/daemonflux/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-08 08:49:33.000000 daemonflux-0.6.1/src/daemonflux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/src/daemonflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-08 08:50:04.000000 daemonflux-0.6.1/src/daemonflux.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 08:50:04.333390 daemonflux-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-08 08:49:34.000000 daemonflux-0.6.1/tests/test_daemonflux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-01 12:50:26.000000 daemonflux-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 12:50:51.821183 daemonflux-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-01 12:50:26.000000 daemonflux-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-01 12:50:26.000000 daemonflux-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-01 12:50:51.821183 daemonflux-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.817183 daemonflux-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/src/daemonflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 12:50:26.000000 daemonflux-0.7.0/src/daemonflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26884 2023-06-01 12:50:26.000000 daemonflux-0.7.0/src/daemonflux/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-01 12:50:26.000000 daemonflux-0.7.0/src/daemonflux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/src/daemonflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 12:50:51.000000 daemonflux-0.7.0/src/daemonflux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:50:51.821183 daemonflux-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-06-01 12:50:26.000000 daemonflux-0.7.0/tests/test_daemonflux.py
```

### Comparing `daemonflux-0.6.1/LICENSE` & `daemonflux-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daemonflux-0.6.1/PKG-INFO` & `daemonflux-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.6.1
+Version: 0.7.0
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `daemonflux-0.6.1/README.md` & `daemonflux-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `daemonflux-0.6.1/setup.cfg` & `daemonflux-0.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = daemonflux
-version = 0.6.1
+version = 0.7.0
 author = Anatoli Fedynitch
 maintainer_email = afedynitch@gmail.com
 description = Tabulated representation of a muon-calibrated muon and neutrino flux model
 license = BSD 3-Clause License
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mceq-project/daemonflux
```

### Comparing `daemonflux-0.6.1/src/daemonflux/__init__.py` & `daemonflux-0.7.0/src/daemonflux/__init__.py`

 * *Files identical despite different names*

### Comparing `daemonflux-0.6.1/src/daemonflux/flux.py` & `daemonflux-0.7.0/src/daemonflux/flux.py`

 * *Files 14% similar despite different names*

```diff
@@ -84,66 +84,124 @@
             Parameter value.
         """
         for p, pv in zip(self.known_parameters, self.values):
             yield p, pv
 
 
 class Flux:
+    """
+    This class encapsulates the behavior of a Flux.
+
+    Attributes
+    ----------
+    exclude : list
+        A list of items to be excluded.
+    _debug : int
+        Debug level.
+    supported_fluxes : list
+        A list of fluxes supported.
+
+    """
+
     _default_url = (
         "https://github.com/mceq-project/daemonflux/releases/download/prerelease/"
     )
     _default_spl_file = "daemonsplines_{location}_{rev}.pkl"
-    _default_cal_file = "daemonsplines_calibration_{rev}.pkl"
+    _default_cal_file = "daemonsplines_calibration_{cset}_{rev}.pkl"
     _revision = "202303_1"
 
     def __init__(
         self,
         location="generic",
         spl_file=None,
         cal_file=None,
+        calibration_set="default",
         use_calibration=True,
         exclude=[],
         keep_old_revisions=False,
         debug=1,
     ) -> None:
+        """
+        Initialize the Flux instance.
+
+        Parameters
+        ----------
+        location : str, optional
+            Location to be used, default is "generic".
+        spl_file : str, optional
+            Path to the spline file.
+        cal_file : str, optional
+            Path to the calibration file.
+        use_calibration : bool, optional
+            Flag indicating whether to use calibration, default is True.
+        calibration_set : str, optional
+            Calibration set to be used. Default is "default". Optional is "with_deis".
+        exclude : list, optional
+            A list of parameters to be excluded, default is an empty list.
+        keep_old_revisions : bool, optional
+            Flag indicating whether to keep old spline file revisions, default is False.
+        debug : int, optional
+            Debug level, default is 1.
+        """
         self.exclude = exclude
         self._debug = debug
         spl_file = (
             spl_file
             if spl_file
             else _cached_data_dir(
                 self._default_url
                 + self._default_spl_file.format(location=location, rev=self._revision)
             )
         )
-        if not use_calibration:
+        if not use_calibration or not calibration_set:
             cal_file = None
         elif use_calibration and cal_file is None:
             cal_file = _cached_data_dir(
-                self._default_url + self._default_cal_file.format(rev=self._revision)
+                self._default_url
+                + self._default_cal_file.format(
+                    cset=calibration_set, rev=self._revision
+                )
             )
 
         self._load_splines(spl_file, cal_file)
         if not keep_old_revisions:
             self._cleanup_old_revisions()
 
     def _cleanup_old_revisions(self):
+        """
+        Clean up old revisions of the data.
+        """
         import pathlib
 
         for f in pathlib.Path(base_path / "data").glob("daemonsplines*"):
             if self._revision not in str(f):
                 print("Removing old version", f)
                 f.unlink()
 
     def _load_splines(self, spl_file, cal_file):
+        """
+        Load splines from given files.
+
+        Parameters
+        ----------
+        spl_file : str
+            Path to the spline file.
+        cal_file : str
+            Path to the calibration file.
+        """
         from .utils import rearrange_covariance
         from copy import deepcopy
 
         assert pathlib.Path(spl_file).is_file(), f"Spline file {spl_file} not found."
-        (known_pars, self._fl_spl, self._jac_spl, cov,) = pickle.load(
+        (
+            known_pars,
+            self._fl_spl,
+            self._jac_spl,
+            cov,
+        ) = pickle.load(
             open(spl_file, "rb")
         )[:4]
 
         known_parameters = []
         for k in known_pars:
             if k in self.exclude:
                 continue
@@ -160,15 +218,14 @@
                 cov,
             )
             assert params.cov.shape == (len(known_parameters),) * 2, (
                 f"covariance shape {params.cov.shape} is not consistent"
                 + f" with the number of parameters {len(known_parameters)}"
             )
         else:
-
             assert pathlib.Path(
                 cal_file
             ).is_file(), f"Calibration file {cal_file} not found."
 
             calibration_d = pickle.load(open(str(cal_file), "rb"), encoding="latin1")
 
             param_values = []
@@ -213,14 +270,15 @@
                         + " "
                         + str(pj)
                         + " incorrectly sorted."
                     )
 
             params = Parameters(known_parameters, np.asarray(param_values), cov)
 
+        # If multiple locations inside the spline file, create a FluxEntry for each
         self.supported_fluxes = []
         for exp in self._fl_spl:
             subflux = _FluxEntry(
                 exp,
                 self._fl_spl[exp],
                 self._jac_spl[exp],
                 deepcopy(params),
@@ -231,47 +289,145 @@
 
     def __repr__(self):
         s = ""
         for exp in self._fl_spl:
             s += "{0}: [{1}]\n".format(exp, ", ".join(self._fl_spl[exp].keys()))
         return s
 
-    def print_experiments(self):
+    def print_locations(self):
+        """
+        Print the locations contained within the spline file.
+        """
         print(self.__repr__())
 
     @property
     def zenith_angles(self, exp=""):
+        """
+        Retrieve zenith angles of splines for the specified location/experiment.
+
+        Parameters
+        ----------
+        exp : str, optional
+            Experiment name, default is an empty string.
+        """
         if not exp and len(self.supported_fluxes) > 1:
             raise Exception("'exp' argument needs to be one of", self.supported_fluxes)
         if len(self.supported_fluxes) == 1:
             return self.__getattribute__(self.supported_fluxes[0]).zenith_angles
         else:
             return self.__getattribute__(exp).zenith_angles
 
     def _get_flux_instance(self, exp):
+        """
+        Retrieve the _FluxEntry indexed by an experiment or location.
+
+        Parameters
+        ----------
+        exp : str
+            Experiment name.
+        """
         if not exp and len(self.supported_fluxes) > 1:
             raise Exception("'exp' argument needs to be one of", self.supported_fluxes)
 
         if len(self.supported_fluxes) == 1:
             return self.__getattribute__(self.supported_fluxes[0])
         else:
             return self.__getattribute__(exp)
 
     @property
     def quantities(self, exp=""):
+        """
+        Retrieve the quantities supported by the spline file.
+
+        The default quantities are 'muflux', 'muratio', 'numuflux', 'numuratio',
+        'nueflux', 'nueratio', 'flavorratio', 'mu+', 'mu-', 'numu', 'antinumu',
+        'nue', 'antinue'. The quantities are the same for all locations. Those with
+        'flux' in the names sums over conventional 'mu+' and 'mu-', and neutrino and
+        antineutrino, respectively. Those with 'ratio' in the names are the ratios of
+        the fluxes. A second set of quantities is available with the 'total_' prefix,
+        which includes is a sum of the conventional and prompt fluxes. The latter are
+        calculated with the SIBYLL2.3d hadronic interaction model.
+
+        Parameters
+        ----------
+        exp : str, optional
+            Experiment name, default is an empty string.
+        """
         return self._get_flux_instance(exp)._quantities
 
     @property
     def params(self, exp=""):
+        """
+        Retrieve a list of the daemonflux parameters.
+
+        Parameters
+        ----------
+        exp : str, optional
+            Experiment name, default is an empty string.
+        """
         return self._get_flux_instance(exp)._params
 
     def flux(self, grid, zenith_deg, quantity, params={}, exp=""):
+        """
+        The flux of a given quantity for the specified energy grid and zenith angles.
+
+        The flux is multiplied by E^3 in units of GeV^2/(cm^2 s sr).
+
+        Parameters
+        ----------
+        grid : np.ndarray
+            The energy grid in units of GeV.
+        zenith_deg : float or str or list of float
+            The zenith angle in degrees. If "average", the average flux over all
+            zenith angles will be returned.
+        quantity : str
+            The type of flux to be returned.
+        params : Dict[str, float], optional
+            A dictionary of parameter values to shift daemonflux off the baseline.
+
+        Returns
+        -------
+        np.ndarray
+            The flux multiplied by E^3 in units of GeV^2/(cm^2 s sr).
+
+        Raises
+        ------
+        Exception
+            If `zenith_deg` is "average" but splines do not contain average flux.
+        """
         return self._get_flux_instance(exp).flux(grid, zenith_deg, quantity, params)
 
     def error(self, grid, zenith_deg, quantity, only_hadronic=False, exp=""):
+        """
+        The flux of a given quantity for the specified energy grid and zenith angles.
+
+        The error is multiplied by E^3 in units of GeV^2/(cm^2 s sr).
+
+        Parameters
+        ----------
+        grid : np.ndarray
+            The energy grid for which to compute the error.
+        zenith_deg : float or str or list of float
+            The zenith angle in degrees, or a list of zenith angles.
+        quantity : str
+            The quantity to compute the error for.
+        only_hadronic : bool, optional
+            Whether to only include the hadronic error, excluding the cosmic ray flux
+            error, by default False.
+
+        Returns
+        -------
+        np.ndarray
+            The error of the flux estimation.
+
+        Raises
+        ------
+        Exception
+            If `zenith_deg` is "average" but splines do not contain average flux.
+        """
         return self._get_flux_instance(exp).error(
             grid,
             zenith_deg,
             quantity,
             only_hadronic,
         )
 
@@ -366,15 +522,14 @@
         else:
             prev = deepcopy(self._params)
             pars = self._params
             new_kp = []
             new_values = []
             keep_cov = []
             for ik, k in enumerate(pars.known_parameters):
-
                 if exclude_str in k:
                     continue
                 new_kp.append(k)
                 new_values.append(pars.values[ik])
                 keep_cov.append(ik)
 
             pars.cov = np.take(np.take(pars.cov, keep_cov, axis=0), keep_cov, axis=1)
@@ -471,15 +626,14 @@
         if self._debug > 2:
             print(
                 f"Return {quantity} flux for {zenith_deg}, only_hadronic=",
                 only_hadronic,
             )
 
         with self._temporary_exclude_parameters("GSF" if only_hadronic else None):
-
             jac = self._jac_spl[zenith_deg]
 
             jacfl = np.vstack(
                 [
                     jac[par][quantity](np.log(grid))
                     for par in self._params.known_parameters
                 ]
@@ -560,21 +714,21 @@
         """
         Compute the flux at the given energy grid, zenith angle, and quantity.
 
         Parameters
         ----------
         grid : np.ndarray
             The energy grid in units of GeV.
-        zenith_deg : float or str
+        zenith_deg : float or str or list of float
             The zenith angle in degrees. If "average", the average flux over all
             zenith angles will be returned.
         quantity : str
             The type of flux to be returned.
         params : Dict[str, float], optional
-            A dictionary of parameter values to use for the calculation.
+            A dictionary of parameter values to shift daemonflux off the baseline.
 
         Returns
         -------
         np.ndarray
             The flux multiplied by E^3 in units of GeV^2/(cm^2 s sr).
 
         Raises
```

### Comparing `daemonflux-0.6.1/src/daemonflux/utils.py` & `daemonflux-0.7.0/src/daemonflux/utils.py`

 * *Files identical despite different names*

### Comparing `daemonflux-0.6.1/src/daemonflux.egg-info/PKG-INFO` & `daemonflux-0.7.0/src/daemonflux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daemonflux
-Version: 0.6.1
+Version: 0.7.0
 Summary: Tabulated representation of a muon-calibrated muon and neutrino flux model
 Home-page: https://github.com/mceq-project/daemonflux
 Download-URL: https://pypi.python.org/pypi/daemonflux
 Author: Anatoli Fedynitch
 Maintainer-email: afedynitch@gmail.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `daemonflux-0.6.1/tests/test_daemonflux.py` & `daemonflux-0.7.0/tests/test_daemonflux.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,29 +138,29 @@
 def test_flux_calibrated():
     import pathlib
 
     basep = pathlib.Path(__file__).parent.absolute()
     return Flux(
         "",
         spl_file=basep / "test_daemonsplines_generic_202303_1.pkl",
-        cal_file=basep / "test_calibration_202303_1.pkl",
+        cal_file=basep / "test_calibration_default_202303_1.pkl",
         use_calibration=True,
         debug=1,
     )
 
 
 @pytest.fixture(scope="session")
 def test_flux_not_calibrated():
     import pathlib
 
     basep = pathlib.Path(__file__).parent.absolute()
     return Flux(
         "",
         spl_file=basep / "test_daemonsplines_generic_202303_1.pkl",
-        cal_file=basep / "test_calibration_202303_1.pkl",
+        cal_file=basep / "test_calibration_default_202303_1.pkl",
         use_calibration=False,
         debug=1,
     )
 
 
 # Generate updated numbers for this test by running the following:
 def test_Flux(test_flux_calibrated, test_flux_not_calibrated):
@@ -351,16 +351,18 @@
     url_generic_spl = (
         test_flux_calibrated._default_url
         + test_flux_calibrated._default_spl_file.format(
             location="generic", rev=test_flux_calibrated._revision
         )
         + ".zip"
     )
-    url_cal = (
-        test_flux_calibrated._default_url
-        + test_flux_calibrated._default_cal_file.format(
-            rev=test_flux_calibrated._revision
-        )
-        + ".zip"
-    )
     assert request.urlopen(url_generic_spl).status in [200, 302]
-    assert request.urlopen(url_cal).status in [200, 302]
+    
+    for cal_set in ["default", "with_deis"]:
+        url_cal = (
+            test_flux_calibrated._default_url
+            + test_flux_calibrated._default_cal_file.format(
+                cset=cal_set, rev=test_flux_calibrated._revision
+            )
+            + ".zip"
+        )
+        assert request.urlopen(url_cal).status in [200, 302]
```

