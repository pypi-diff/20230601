# Comparing `tmp/glass-2023.2.tar.gz` & `tmp/glass-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glass-2023.2.tar", last modified: Wed Mar  1 11:31:07 2023, max compression
+gzip compressed data, was "glass-2023.5.tar", last modified: Wed May 31 23:39:52 2023, max compression
```

## Comparing `glass-2023.2.tar` & `glass-2023.5.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:31:07.399081 glass-2023.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-01 11:30:59.000000 glass-2023.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-01 11:31:07.403081 glass-2023.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-01 11:30:59.000000 glass-2023.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:31:07.399081 glass-2023.2/glass/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-01 11:30:59.000000 glass-2023.2/glass/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-03-01 11:30:59.000000 glass-2023.2/glass/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-03-01 11:30:59.000000 glass-2023.2/glass/galaxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-03-01 11:30:59.000000 glass-2023.2/glass/lensing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-01 11:30:59.000000 glass-2023.2/glass/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-03-01 11:30:59.000000 glass-2023.2/glass/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-03-01 11:30:59.000000 glass-2023.2/glass/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-03-01 11:30:59.000000 glass-2023.2/glass/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-03-01 11:30:59.000000 glass-2023.2/glass/shells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:31:07.399081 glass-2023.2/glass/test/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-01 11:30:59.000000 glass-2023.2/glass/test/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-03-01 11:30:59.000000 glass-2023.2/glass/test/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-01 11:30:59.000000 glass-2023.2/glass/test/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-01 11:30:59.000000 glass-2023.2/glass/test/test_shells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-01 11:30:59.000000 glass-2023.2/glass/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 11:31:07.399081 glass-2023.2/glass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-03-01 11:31:07.000000 glass-2023.2/glass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-01 11:31:07.000000 glass-2023.2/glass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 11:31:07.000000 glass-2023.2/glass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-01 11:31:07.000000 glass-2023.2/glass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 11:31:07.000000 glass-2023.2/glass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-01 11:31:07.403081 glass-2023.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 11:30:59.000000 glass-2023.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 23:39:43.000000 glass-2023.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-31 23:39:52.298624 glass-2023.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-31 23:39:43.000000 glass-2023.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 23:39:43.000000 glass-2023.5/glass/all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/core/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-31 23:39:43.000000 glass-2023.5/glass/core/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-05-31 23:39:43.000000 glass-2023.5/glass/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-31 23:39:43.000000 glass-2023.5/glass/galaxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-31 23:39:43.000000 glass-2023.5/glass/lensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-31 23:39:43.000000 glass-2023.5/glass/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-31 23:39:43.000000 glass-2023.5/glass/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-31 23:39:43.000000 glass-2023.5/glass/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-31 23:39:43.000000 glass-2023.5/glass/shells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_galaxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-31 23:39:43.000000 glass-2023.5/glass/test/test_shells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-31 23:39:43.000000 glass-2023.5/glass/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:39:52.298624 glass-2023.5/glass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 23:39:52.000000 glass-2023.5/glass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-31 23:39:52.298624 glass-2023.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:39:43.000000 glass-2023.5/setup.py
```

### Comparing `glass-2023.2/LICENSE` & `glass-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glass-2023.2/PKG-INFO` & `glass-2023.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glass
-Version: 2023.2
+Version: 2023.5
 Summary: Generator for Large Scale Structure
 Home-page: https://github.com/glass-dev/glass
 Maintainer: Nicolas Tessore
 Maintainer-email: n.tessore@ucl.ac.uk
 License: MIT
 Project-URL: Documentation, https://glass.readthedocs.io/
 Project-URL: Issues, https://github.com/glass-dev/glass/issues
@@ -20,16 +20,16 @@
 
 **GLASS**: Generator for Large Scale Structure
 ==============================================
 
 [![Documentation](https://readthedocs.org/projects/glass/badge/?version=latest)](https://glass.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/glass)](https://pypi.org/project/glass)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.01942-red)](https://arxiv.org/abs/2302.01942)
-[![adsabs](https://img.shields.io/badge/ads-2023arXiv230201942T-blueviolet)](https://ui.adsabs.harvard.edu/abs/2023arXiv230201942T)
-[![doi](https://img.shields.io/badge/doi-10.48550/arXiv.2302.01942-blue)](https://dx.doi.org/10.48550/arXiv.2302.01942)
+[![adsabs](https://img.shields.io/badge/ads-2023OJAp....6E..11T-blueviolet)](https://ui.adsabs.harvard.edu/abs/2023OJAp....6E..11T)
+[![doi](https://img.shields.io/badge/doi-10.21105/astro.2302.01942-blue)](https://dx.doi.org/10.21105/astro.2302.01942)
 [![Slack](https://img.shields.io/badge/join-Slack-4A154B)](https://glass-dev.github.io/slack)
 
 This is the core library for GLASS, the Generator for Large Scale Structure.
 For more information, see the full [documentation].  There are a number of
 [examples] to get you started.
 
 
@@ -59,12 +59,24 @@
 The best way to get help about the code is currently to get in touch.
 
 If you would like to start a discussion with the wider GLASS community about
 e.g. a design decision or API change, you can use our [Discussions] page.
 
 We also have a public [Slack workspace] for discussions about the project.
 
+To keep up with new GLASS releases, you can receive GitHub release
+notifications from this repository.  Alternatively, you can subscribe to our
+announcement mailing list, which only receives 1 email/release.  To subscribe,
+use the [mailing list page], or send an email to `listserv@jiscmail.ac.uk` with
+any subject and the following message body:
+
+    subscribe glass <Your name>
+
+where `<Your name>` is your full name, or `ANONYMOUS` if you prefer. You will
+be sent a confirmation email in return.
+
 
 [documentation]: https://glass.readthedocs.io/
 [examples]: https://glass.readthedocs.io/projects/examples/
 [Discussions]: https://github.com/orgs/glass-dev/discussions
 [Slack workspace]: https://glass-dev.github.io/slack
+[mailing list page]: https://jiscmail.ac.uk/lists/GLASS.html
```

### Comparing `glass-2023.2/glass/fields.py` & `glass-2023.5/glass/fields.py`

 * *Files identical despite different names*

### Comparing `glass-2023.2/glass/galaxies.py` & `glass-2023.5/glass/galaxies.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,80 +14,83 @@
 
 .. autofunction:: redshifts_from_nz
 .. autofunction:: galaxy_shear
 .. autofunction:: gaussian_phz
 
 '''
 
+from __future__ import annotations
+
 import numpy as np
 import healpix
 
-from typing import Optional, Tuple
+from numpy.typing import ArrayLike
 
-from .math import cumtrapz
+from .core.array import broadcast_leading_axes, cumtrapz
 
 
-def redshifts_from_nz(size: int, z: np.ndarray, nz: np.ndarray, *,
-                      rng: Optional[np.random.Generator] = None
-                      ) -> Tuple[np.ndarray, Optional[np.ndarray]]:
+def redshifts_from_nz(count: int | ArrayLike, z: ArrayLike, nz: ArrayLike, *,
+                      rng: np.random.Generator | None = None
+                      ) -> np.ndarray:
     '''Generate galaxy redshifts from a source distribution.
 
+    The function supports sampling from multiple populations of
+    redshifts if *count* is an array or if there are additional axes in
+    the *z* or *nz* arrays.  In this case, the shape of *count* and the
+    leading dimensions of *z* and *nz* are broadcast to a common shape,
+    and redshifts are sampled independently for each extra dimension.
+    The results are concatenated into a flat array.
+
     Parameters
     ----------
-    size : int
-        Number of redshifts to sample.
+    count : int or array_like
+        Number of redshifts to sample.  If an array is given, its shape
+        is broadcast against the leading axes of *z* and *nz*.
     z, nz : array_like
-        Source distribution.  Leading axes are treated as different
-        galaxy populations.
+        Source distribution.  Leading axes are broadcast against the
+        shape of *count*.
     rng : :class:`~numpy.random.Generator`, optional
-        Random number generator.  If not given, a default RNG will be
-        used.
+        Random number generator.  If not given, a default RNG is used.
 
     Returns
     -------
-    z : array_like
-        Redshifts sampled from the given source distribution.
-    pop : array_like or None
-        Index of the galaxy population from the leading axes of ``nz``;
-        or ``None`` if there are no galaxy populations.
+    redshifts : array_like
+        Redshifts sampled from the given source distribution.  For
+        inputs with extra dimensions, returns a flattened 1-D array of
+        samples from all populations.
 
     '''
 
     # get default RNG if not given
     if rng is None:
         rng = np.random.default_rng()
 
-    # get galaxy populations
-    if np.ndim(nz) > 1:
-        pop = list(np.ndindex(np.shape(nz)[:-1]))
-    else:
-        pop = None
+    # bring inputs' leading axes into common shape
+    dims, count, z, nz = broadcast_leading_axes((count, 0), (z, 1), (nz, 1))
 
-    # compute the as-yet unnormalised CDF of each galaxy population
-    cdf = cumtrapz(nz, z)
+    # list of results for all dimensions
+    redshifts = np.empty(count.sum())
 
-    # compute probability to be in each galaxy population
-    p = cdf[..., -1]/cdf[..., -1].sum(axis=None, keepdims=True)
+    # keep track of the number of sampled redshifts
+    total = 0
 
-    # now normalise the CDFs
-    cdf /= cdf[..., -1:]
-
-    # sample redshifts and populations
-    if pop is not None:
-        x = rng.choice(len(pop), p=p, size=size)
-        gal_z = rng.uniform(0, 1, size=size)
-        for i, j in enumerate(pop):
-            s = (x == i)
-            gal_z[s] = np.interp(gal_z[s], cdf[j], z)
-        gal_pop = np.take(pop, x)
-    else:
-        gal_z = np.interp(rng.uniform(0, 1, size=size), cdf, z)
-        gal_pop = None
+    # go through extra dimensions; also works if dims is empty
+    for k in np.ndindex(dims):
 
-    return gal_z, gal_pop
+        # compute the CDF of each galaxy population
+        cdf = cumtrapz(nz[k], z[k], dtype=float)
+        cdf /= cdf[-1]
+
+        # sample redshifts and store result
+        redshifts[total:total+count[k]] = np.interp(rng.uniform(0, 1, size=count[k]), cdf, z[k])
+        total += count[k]
+
+    assert total == redshifts.size
+
+    return redshifts
 
 
 def galaxy_shear(lon: np.ndarray, lat: np.ndarray, eps: np.ndarray,
                  kappa: np.ndarray, gamma1: np.ndarray, gamma2: np.ndarray, *,
                  reduced_shear: bool = True) -> np.ndarray:
     '''Observed galaxy shears from weak lensing.
 
@@ -138,41 +141,42 @@
     else:
         # simple sum of shears
         g += eps
 
     return g
 
 
-def gaussian_phz(z: np.ndarray, sigma_0: float,
-                 rng: Optional[np.random.Generator] = None) -> np.ndarray:
+def gaussian_phz(z: ArrayLike, sigma_0: float | ArrayLike,
+                 rng: np.random.Generator | None = None) -> np.ndarray:
     r'''Photometric redshifts assuming a Gaussian error.
 
-    A simple toy model of photometric redshift errors that assumes a Gaussian
-    error with redshift-dependent standard deviation :math:`\sigma(z) = (1 + z)
-    \sigma_0` [1]_.
+    A simple toy model of photometric redshift errors that assumes a
+    Gaussian error with redshift-dependent standard deviation
+    :math:`\sigma(z) = (1 + z) \sigma_0` [1]_.
 
     Parameters
     ----------
     z : array_like
         True redshifts.
-    sigma_0 : float
+    sigma_0 : float or array_like
         Redshift error in the tomographic binning at zero redshift.
     rng : :class:`~numpy.random.Generator`, optional
-        Random number generator.  If not given, a default RNG will be used.
+        Random number generator.  If not given, a default RNG is used.
 
     Returns
     -------
     phz : array_like
-        Photometric redshifts assuming Gaussian errors, of the same shape as
-        ``z``.
+        Photometric redshifts assuming Gaussian errors, of the same
+        shape as *z*.
 
     See Also
     --------
     glass.observations.tomo_nz_gausserr :
-        Create tomographic redshift distributions assuming the same model.
+        Create tomographic redshift distributions assuming the same
+        model.
 
     References
     ----------
     .. [1] Amara A., Réfrégier A., 2007, MNRAS, 381, 1018.
            doi:10.1111/j.1365-2966.2007.12271.x
 
     Examples
@@ -181,18 +185,23 @@
 
     '''
 
     # get default RNG if not given
     if rng is None:
         rng = np.random.default_rng()
 
-    size = np.shape(z)
-    z = np.reshape(z, (-1,))
+    sigma = np.add(1, z)*sigma_0
+    dims = np.shape(sigma)
 
-    zphot = rng.normal(z, (1 + z)*sigma_0)
+    zphot = rng.normal(z, sigma)
 
-    trunc = np.where(zphot < 0)[0]
-    while trunc.size:
-        zphot[trunc] = rng.normal(z[trunc], (1 + z[trunc])*sigma_0)
-        trunc = trunc[zphot[trunc] < 0]
+    if not dims:
+        while zphot < 0:
+            zphot = rng.normal(z, sigma)
+    else:
+        z = np.broadcast_to(z, dims)
+        trunc = np.where(zphot < 0)[0]
+        while trunc.size:
+            zphot[trunc] = rng.normal(z[trunc], sigma[trunc])
+            trunc = trunc[zphot[trunc] < 0]
 
-    return zphot.reshape(size)
+    return zphot
```

### Comparing `glass-2023.2/glass/lensing.py` & `glass-2023.5/glass/lensing.py`

 * *Files identical despite different names*

### Comparing `glass-2023.2/glass/observations.py` & `glass-2023.5/glass/observations.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import numpy as np
 import healpy as hp
 import math
 
 from typing import Optional, Tuple, List
 from numpy.typing import ArrayLike
 
-from .math import cumtrapz
+from .core.array import cumtrapz
 
 
 def vmap_galactic_ecliptic(nside: int, galactic: Tuple[float, float] = (30, 90),
                            ecliptic: Tuple[float, float] = (20, 80)
                            ) -> np.ndarray:
     '''visibility map masking galactic and ecliptic plane
```

### Comparing `glass-2023.2/glass/shapes.py` & `glass-2023.5/glass/shapes.py`

 * *Files identical despite different names*

### Comparing `glass-2023.2/glass/shells.py` & `glass-2023.5/glass/shells.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
 '''
 
 import warnings
 from collections import namedtuple
 import numpy as np
 
-from .math import ndinterp
-
+from .core.array import ndinterp
 
 # type checking
 from typing import (Union, Sequence, List, Tuple, Optional, Callable,
                     TYPE_CHECKING)
 from numpy.typing import ArrayLike
 if TYPE_CHECKING:
     from cosmology import Cosmology
```

### Comparing `glass-2023.2/glass/test/test_math.py` & `glass-2023.5/glass/core/test/test_array.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 import numpy as np
 import numpy.testing as npt
 
 
+def test_broadcast_leading_axes():
+    from glass.core.array import broadcast_leading_axes
+
+    a = 0
+    b = np.zeros((4, 10))
+    c = np.zeros((3, 1, 5, 6))
+
+    dims, a, b, c = broadcast_leading_axes((a, 0), (b, 1), (c, 2))
+
+    assert dims == (3, 4)
+    assert a.shape == (3, 4)
+    assert b.shape == (3, 4, 10)
+    assert c.shape == (3, 4, 5, 6)
+
+
 def test_ndinterp():
-    from glass.math import ndinterp
+    from glass.core.array import ndinterp
 
     # test 1d interpolation
 
     xp = [0, 1, 2, 3, 4]
     yp = [1.1, 1.2, 1.3, 1.4, 1.5]
 
     x = 0.5
```

### Comparing `glass-2023.2/glass/test/test_shells.py` & `glass-2023.5/glass/test/test_shells.py`

 * *Files identical despite different names*

### Comparing `glass-2023.2/glass.egg-info/PKG-INFO` & `glass-2023.5/glass.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glass
-Version: 2023.2
+Version: 2023.5
 Summary: Generator for Large Scale Structure
 Home-page: https://github.com/glass-dev/glass
 Maintainer: Nicolas Tessore
 Maintainer-email: n.tessore@ucl.ac.uk
 License: MIT
 Project-URL: Documentation, https://glass.readthedocs.io/
 Project-URL: Issues, https://github.com/glass-dev/glass/issues
@@ -20,16 +20,16 @@
 
 **GLASS**: Generator for Large Scale Structure
 ==============================================
 
 [![Documentation](https://readthedocs.org/projects/glass/badge/?version=latest)](https://glass.readthedocs.io/en/latest/)
 [![PyPI](https://img.shields.io/pypi/v/glass)](https://pypi.org/project/glass)
 [![arXiv](https://img.shields.io/badge/arXiv-2302.01942-red)](https://arxiv.org/abs/2302.01942)
-[![adsabs](https://img.shields.io/badge/ads-2023arXiv230201942T-blueviolet)](https://ui.adsabs.harvard.edu/abs/2023arXiv230201942T)
-[![doi](https://img.shields.io/badge/doi-10.48550/arXiv.2302.01942-blue)](https://dx.doi.org/10.48550/arXiv.2302.01942)
+[![adsabs](https://img.shields.io/badge/ads-2023OJAp....6E..11T-blueviolet)](https://ui.adsabs.harvard.edu/abs/2023OJAp....6E..11T)
+[![doi](https://img.shields.io/badge/doi-10.21105/astro.2302.01942-blue)](https://dx.doi.org/10.21105/astro.2302.01942)
 [![Slack](https://img.shields.io/badge/join-Slack-4A154B)](https://glass-dev.github.io/slack)
 
 This is the core library for GLASS, the Generator for Large Scale Structure.
 For more information, see the full [documentation].  There are a number of
 [examples] to get you started.
 
 
@@ -59,12 +59,24 @@
 The best way to get help about the code is currently to get in touch.
 
 If you would like to start a discussion with the wider GLASS community about
 e.g. a design decision or API change, you can use our [Discussions] page.
 
 We also have a public [Slack workspace] for discussions about the project.
 
+To keep up with new GLASS releases, you can receive GitHub release
+notifications from this repository.  Alternatively, you can subscribe to our
+announcement mailing list, which only receives 1 email/release.  To subscribe,
+use the [mailing list page], or send an email to `listserv@jiscmail.ac.uk` with
+any subject and the following message body:
+
+    subscribe glass <Your name>
+
+where `<Your name>` is your full name, or `ANONYMOUS` if you prefer. You will
+be sent a confirmation email in return.
+
 
 [documentation]: https://glass.readthedocs.io/
 [examples]: https://glass.readthedocs.io/projects/examples/
 [Discussions]: https://github.com/orgs/glass-dev/discussions
 [Slack workspace]: https://glass-dev.github.io/slack
+[mailing list page]: https://jiscmail.ac.uk/lists/GLASS.html
```

### Comparing `glass-2023.2/setup.cfg` & `glass-2023.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = glass
-version = 2023.2
+version = 2023.5
 maintainer = Nicolas Tessore
 maintainer_email = n.tessore@ucl.ac.uk
 description = Generator for Large Scale Structure
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
@@ -16,15 +16,15 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 python_requires = >=3.6
 install_requires = 
-	numpy
+	numpy>=1.20.0
 	healpix>=2022.11.1
 	healpy>=1.15.0
 	cosmology>=2022.10.9
 	gaussiancl>=2022.10.21
 packages = find_namespace:
 
 [options.packages.find]
```

