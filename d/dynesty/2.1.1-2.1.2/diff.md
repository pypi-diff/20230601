# Comparing `tmp/dynesty-2.1.1.tar.gz` & `tmp/dynesty-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynesty-2.1.1.tar", last modified: Sun Apr 16 02:01:46 2023, max compression
+gzip compressed data, was "dynesty-2.1.2.tar", last modified: Thu Jun  1 15:18:48 2023, max compression
```

## Comparing `dynesty-2.1.1.tar` & `dynesty-2.1.2.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.530282 dynesty-2.1.1/
--rw-rw-r--   0 koposov   (1000) koposov   (1000)      850 2022-12-02 00:57:09.000000 dynesty-2.1.1/AUTHORS.md
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1166 2022-12-02 00:56:46.000000 dynesty-2.1.1/LICENSE
--rw-rw-r--   0 koposov   (1000) koposov   (1000)       37 2022-12-02 00:56:46.000000 dynesty-2.1.1/MANIFEST.in
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     2954 2023-04-16 02:01:46.530282 dynesty-2.1.1/PKG-INFO
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     2176 2023-02-28 22:18:22.000000 dynesty-2.1.1/README.md
-drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.526282 dynesty-2.1.1/py/
-drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.526282 dynesty-2.1.1/py/dynesty/
--rw-rw-r--   0 koposov   (1000) koposov   (1000)      361 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/__init__.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)       22 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/_version.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    53481 2022-12-26 20:42:45.000000 dynesty-2.1.1/py/dynesty/bounding.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    95151 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/dynamicsampler.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    34682 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/dynesty.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    37294 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/nestedsamplers.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    90800 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/plotting.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     4846 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/pool.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)      160 2022-12-02 00:56:47.000000 dynesty-2.1.1/py/dynesty/results.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    43989 2023-04-15 23:00:14.000000 dynesty-2.1.1/py/dynesty/sampler.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    40647 2023-03-19 23:04:45.000000 dynesty-2.1.1/py/dynesty/sampling.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    80191 2023-04-15 16:30:55.000000 dynesty-2.1.1/py/dynesty/utils.py
-drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.526282 dynesty-2.1.1/py/dynesty.egg-info/
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     2954 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/PKG-INFO
--rw-rw-r--   0 koposov   (1000) koposov   (1000)      939 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/SOURCES.txt
--rw-rw-r--   0 koposov   (1000) koposov   (1000)        1 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/dependency_links.txt
--rw-rw-r--   0 koposov   (1000) koposov   (1000)        8 2023-04-16 02:01:46.000000 dynesty-2.1.1/py/dynesty.egg-info/top_level.txt
--rw-rw-r--   0 koposov   (1000) koposov   (1000)       67 2023-04-16 02:01:46.530282 dynesty-2.1.1/setup.cfg
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1841 2022-12-02 00:57:09.000000 dynesty-2.1.1/setup.py
-drwxrwxr-x   0 koposov   (1000) koposov   (1000)        0 2023-04-16 02:01:46.530282 dynesty-2.1.1/tests/
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     5309 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_blob.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1112 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_dyn.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1875 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_egg.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     8684 2022-12-02 00:57:09.000000 dynesty-2.1.1/tests/test_ellipsoid.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    13016 2023-03-16 20:38:54.000000 dynesty-2.1.1/tests/test_gau.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     4205 2023-04-16 00:32:09.000000 dynesty-2.1.1/tests/test_highdim.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)    24687 2023-04-15 23:00:14.000000 dynesty-2.1.1/tests/test_misc.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     5644 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_ncdim.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)      944 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_notebooks.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1520 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_pathology.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     2709 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_periodic.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     9343 2023-04-15 23:00:08.000000 dynesty-2.1.1/tests/test_plateau.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     6161 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_plot.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     6382 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_pool.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1872 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_printing.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1967 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_reflect.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     6629 2023-04-15 23:00:14.000000 dynesty-2.1.1/tests/test_resume.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     3503 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_rosenbrock.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     3633 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_sampling.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     1570 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_saver.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     6187 2022-12-02 00:56:47.000000 dynesty-2.1.1/tests/test_volume.py
--rw-rw-r--   0 koposov   (1000) koposov   (1000)     2420 2022-12-14 13:10:24.000000 dynesty-2.1.1/tests/test_wedding.py
+drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-06-01 15:18:48.106120 dynesty-2.1.2/
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      850 2023-03-21 14:57:34.000000 dynesty-2.1.2/AUTHORS.md
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1166 2023-03-20 15:21:48.000000 dynesty-2.1.2/LICENSE
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       37 2023-03-20 15:21:48.000000 dynesty-2.1.2/MANIFEST.in
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     2954 2023-06-01 15:18:48.106120 dynesty-2.1.2/PKG-INFO
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     2176 2023-03-21 14:57:34.000000 dynesty-2.1.2/README.md
+drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-06-01 15:18:48.102120 dynesty-2.1.2/py/
+drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-06-01 15:18:48.106120 dynesty-2.1.2/py/dynesty/
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      361 2023-03-21 14:57:34.000000 dynesty-2.1.2/py/dynesty/__init__.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       22 2023-06-01 10:58:32.000000 dynesty-2.1.2/py/dynesty/_version.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    53481 2023-06-01 15:06:31.000000 dynesty-2.1.2/py/dynesty/bounding.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    95926 2023-05-19 10:34:52.000000 dynesty-2.1.2/py/dynesty/dynamicsampler.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    34682 2023-04-06 18:39:44.000000 dynesty-2.1.2/py/dynesty/dynesty.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    37294 2023-04-06 18:39:44.000000 dynesty-2.1.2/py/dynesty/nestedsamplers.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    90800 2023-03-21 14:57:34.000000 dynesty-2.1.2/py/dynesty/plotting.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     4846 2023-03-21 14:57:34.000000 dynesty-2.1.2/py/dynesty/pool.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      160 2023-03-21 14:57:34.000000 dynesty-2.1.2/py/dynesty/results.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    43943 2023-05-10 10:34:28.000000 dynesty-2.1.2/py/dynesty/sampler.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    40647 2023-03-21 14:57:34.000000 dynesty-2.1.2/py/dynesty/sampling.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    80766 2023-05-10 09:24:14.000000 dynesty-2.1.2/py/dynesty/utils.py
+drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-06-01 15:18:48.106120 dynesty-2.1.2/py/dynesty.egg-info/
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     2954 2023-06-01 15:18:48.000000 dynesty-2.1.2/py/dynesty.egg-info/PKG-INFO
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      917 2023-06-01 15:18:48.000000 dynesty-2.1.2/py/dynesty.egg-info/SOURCES.txt
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)        1 2023-06-01 15:18:48.000000 dynesty-2.1.2/py/dynesty.egg-info/dependency_links.txt
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)        8 2023-06-01 15:18:48.000000 dynesty-2.1.2/py/dynesty.egg-info/top_level.txt
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)       67 2023-06-01 15:18:48.106120 dynesty-2.1.2/setup.cfg
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1841 2023-03-21 14:57:34.000000 dynesty-2.1.2/setup.py
+drwxrwxr-x   0 skoposov  (1000) skoposov  (1000)        0 2023-06-01 15:18:48.106120 dynesty-2.1.2/tests/
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     5309 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_blob.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1112 2023-03-21 07:55:04.000000 dynesty-2.1.2/tests/test_dyn.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1875 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_egg.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     8865 2023-06-01 10:52:38.000000 dynesty-2.1.2/tests/test_ellipsoid.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    13016 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_gau.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     4205 2023-04-17 10:29:22.000000 dynesty-2.1.2/tests/test_highdim.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)    24691 2023-05-05 08:34:44.000000 dynesty-2.1.2/tests/test_misc.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     5644 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_ncdim.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)      944 2023-03-21 07:55:04.000000 dynesty-2.1.2/tests/test_notebooks.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1520 2023-03-21 07:55:04.000000 dynesty-2.1.2/tests/test_pathology.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     2709 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_periodic.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     9343 2023-05-18 20:20:52.000000 dynesty-2.1.2/tests/test_plateau.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     6161 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_plot.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     6439 2023-05-10 09:24:14.000000 dynesty-2.1.2/tests/test_pool.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1872 2023-03-21 07:55:04.000000 dynesty-2.1.2/tests/test_printing.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1967 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_reflect.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     7607 2023-05-10 12:32:45.000000 dynesty-2.1.2/tests/test_resume.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     3503 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_rosenbrock.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     3633 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_sampling.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     1570 2023-03-21 14:57:34.000000 dynesty-2.1.2/tests/test_saver.py
+-rw-rw-r--   0 skoposov  (1000) skoposov  (1000)     6187 2023-03-21 07:55:04.000000 dynesty-2.1.2/tests/test_volume.py
```

### Comparing `dynesty-2.1.1/AUTHORS.md` & `dynesty-2.1.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/LICENSE` & `dynesty-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/PKG-INFO` & `dynesty-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynesty
-Version: 2.1.1
+Version: 2.1.2
 Summary: A dynamic nested sampling package for computing Bayesian posteriors and evidences.
 Home-page: https://github.com/joshspeagle/dynesty
 Author: Joshua S Speagle, Sergey E Koposov
 Author-email: j.speagle@utoronto.ca
 License: MIT
 Keywords: nested sampling,dynamic,monte carlo,bayesian,inference,modeling
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dynesty-2.1.1/README.md` & `dynesty-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/py/dynesty/bounding.py` & `dynesty-2.1.2/py/dynesty/bounding.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/py/dynesty/dynamicsampler.py` & `dynesty-2.1.2/py/dynesty/dynamicsampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -977,15 +977,17 @@
         self.live_v = None
         self.live_it = None
         self.live_bound = None
         self.live_logl = None
         self.live_init = None
         self.nlive_init = None
         self.batch_sampler = None
-
+        self.checkpoint_timer = None
+        # the reason why we need a global object is to
+        # preserve the timer betweeen batch calls
         self.live_blobs = None
 
     def __setstate__(self, state):
         self.__dict__ = state
         self.pool = None
         self.M = map
 
@@ -1659,14 +1661,15 @@
                                       loglstar=results.loglstar,
                                       nc=results.nc,
                                       worst_it=results.worst_it + it0,
                                       boundidx=results.boundidx,
                                       bounditer=results.bounditer,
                                       eff=self.eff)
         del self.batch_sampler
+        self.batch_sampler = None
 
     def combine_runs(self):
         """ Merge the most recent run into the previous (combined) run by
         "stepping through" both runs simultaneously."""
 
         # Make sure we have a run to add.
         if len(self.new_run['id']) == 0:
@@ -2030,15 +2033,15 @@
         if resume and self.internal_state == DynamicSamplerStatesEnum.RUN_DONE:
             warnings.warn(
                 """You tried to resume the run that has ended successfully.
 This is not supported. No sampling was performed""", RuntimeWarning)
             return
         # Baseline run.
         pbar, print_func = get_print_func(print_func, print_progress)
-        timer = DelayTimer(checkpoint_every)
+        self.checkpoint_timer = DelayTimer(checkpoint_every)
         try:
             if not self.base:
                 for results in self.sample_initial(
                         nlive=nlive_init,
                         dlogz=dlogz_init,
                         maxcall=maxcall_init,
                         maxiter=maxiter_init,
@@ -2049,15 +2052,15 @@
                         save_samples=True):
                     if resume:
                         resume = False
                     ncall += results.nc
                     niter += 1
                     if (checkpoint_file is not None and self.internal_state !=
                             DynamicSamplerStatesEnum.INBASEADDLIVE
-                            and timer.is_time()):
+                            and self.checkpoint_timer.is_time()):
                         self.save(checkpoint_file)
                     # Print progress.
                     if print_progress:
                         print_func(results,
                                    niter,
                                    ncall,
                                    nbatch=0,
@@ -2084,27 +2087,25 @@
                     stop_val = np.nan
 
                 # If we have likelihood calls remaining, iterations remaining,
                 # and we have failed to hit the minimum ESS, run our batch.
                 if mcall > 0 and miter > 0 and not stop:
                     # Compute our sampling bounds using the provided
                     # weight function.
-                    passback = self.add_batch(
-                        nlive=nlive_batch,
-                        wt_function=wt_function,
-                        wt_kwargs=wt_kwargs,
-                        maxiter=miter,
-                        maxcall=mcall,
-                        save_bounds=save_bounds,
-                        print_progress=print_progress,
-                        print_func=print_func,
-                        stop_val=stop_val,
-                        resume=resume,
-                        checkpoint_file=checkpoint_file,
-                        checkpoint_every=checkpoint_every)
+                    passback = self.add_batch(nlive=nlive_batch,
+                                              wt_function=wt_function,
+                                              wt_kwargs=wt_kwargs,
+                                              maxiter=miter,
+                                              maxcall=mcall,
+                                              save_bounds=save_bounds,
+                                              print_progress=print_progress,
+                                              print_func=print_func,
+                                              stop_val=stop_val,
+                                              resume=resume,
+                                              checkpoint_file=checkpoint_file)
                     if resume:
                         # The assumption here is after the first resume
                         # iteration we will proceed as normal
                         resume = False
                     ncall, niter, logl_bounds, results = passback
                 elif logl_bounds[1] != np.inf:
                     # We ran at least one batch and now we're done!
@@ -2141,15 +2142,15 @@
                   logl_bounds=None,
                   save_bounds=True,
                   print_progress=True,
                   print_func=None,
                   stop_val=None,
                   resume=False,
                   checkpoint_file=None,
-                  checkpoint_every=60):
+                  checkpoint_every=None):
         """
         Allocate an additional batch of (nested) samples based on
         the combined set of previous samples using the specified
         weight function.
 
         Parameters
         ----------
@@ -2213,16 +2214,16 @@
             If resume is set to true, we will try to resume a previously
             interrupted run
         checkpoint_file: string, optional
             if not None The state of the sampler will be saved into this
             file every checkpoint_every seconds
         checkpoint_every: float, optional
             The number of seconds between checkpoints that will save
-            the internal state of the sampler. The sampler will also be
-            saved in the end of the run irrespective of checkpoint_every.
+            the internal state of the sampler. If this is None, we
+            we will use the timer created in run_nested()
         """
 
         # Initialize values.
         maxcall = maxcall or sys.maxsize
         maxiter = maxiter or sys.maxsize
         wt_function = wt_function or weight_function
         wt_kwargs = wt_kwargs or {}
@@ -2246,16 +2247,23 @@
         # For printing as well, we just display old logz,logzerr here
         logz, logzvar = res['logz'][-1], res['logzerr'][-1]**2
 
         # If we have either likelihood calls or iterations remaining,
         # add our new batch of live points.
         ncall, niter, n = self.ncall, self.it - 1, self.batch
         if checkpoint_file is not None:
-            timer = DelayTimer(checkpoint_every)
-
+            # if checkpoint_every is provided we are assuming we are
+            # running externally otherwise we are being run from run_nested
+            # and in that case we use a global timer
+            # We have to care about this because if our batches take
+            # shorter than checkpoint_every we still would like to save
+            if checkpoint_every is not None:
+                timer = DelayTimer(checkpoint_every)
+            else:
+                timer = self.checkpoint_timer
         if maxcall > 0 and maxiter > 0:
             pbar, print_func = get_print_func(print_func, print_progress)
             try:
                 results = None  # to silence pylint as
                 # sample_batch() should return something given maxiter/maxcall
                 for cur_results in self.sample_batch(nlive_new=nlive,
                                                      dlogz=dlogz,
```

### Comparing `dynesty-2.1.1/py/dynesty/dynesty.py` & `dynesty-2.1.2/py/dynesty/dynesty.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/py/dynesty/nestedsamplers.py` & `dynesty-2.1.2/py/dynesty/nestedsamplers.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/py/dynesty/plotting.py` & `dynesty-2.1.2/py/dynesty/plotting.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/py/dynesty/pool.py` & `dynesty-2.1.2/py/dynesty/pool.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/py/dynesty/sampler.py` & `dynesty-2.1.2/py/dynesty/sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,16 +297,16 @@
         The arguments are the loglstar and number of calls
         if force is true we update the bound no matter what
         """
 
         if ncall is None:
             ncall = self.ncall
         call_check_first = (ncall >= self.first_bound_update_ncall)
-        call_check = (ncall >=
-                      self.bound_update_interval + self.ncall_at_last_update)
+        call_check = (ncall >= self.bound_update_interval +
+                      self.ncall_at_last_update)
         efficiency_check = (self.eff < self.first_bound_update_eff)
         # there are three cases when we update the bound
         # * if we are still using uniform cube sampling and both efficiency is
         # lower than the threshold and the number of calls is larger than the
         # threshold
         # * if we are sampling from uniform cube and loglstar is larger than
         # the previously saved logl_first_update
@@ -728,19 +728,18 @@
 
         else:
             # Remove live points (if added) from previous run.
             if self.added_live and not resume:
                 self._remove_live_points()
 
             # Get final state from previous run.
-            h, logz, logzvar, logvol = [
+            h, logz, logzvar, logvol, loglstar = [
                 self.saved_run[_][-1]
-                for _ in ['h', 'logz', 'logzvar', 'logvol']
+                for _ in ['h', 'logz', 'logzvar', 'logvol', 'logl']
             ]
-            loglstar = np.min(self.live_logl)  # ln(likelihood)
             delta_logz = np.logaddexp(0,
                                       np.max(self.live_logl) + logvol - logz)
 
         nplateau = 0
         stop_iterations = False
         # The main nested sampling loop.
         for it in range(sys.maxsize):
```

### Comparing `dynesty-2.1.1/py/dynesty/sampling.py` & `dynesty-2.1.2/py/dynesty/sampling.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/py/dynesty/utils.py` & `dynesty-2.1.2/py/dynesty/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,39 +308,39 @@
         return self.D.keys()
 
 
 class DelayTimer:
     """ Utility class that allows us to detect a certain
     time has passed"""
 
-    def __init__(self, dt):
+    def __init__(self, delay):
         """ Initialise the time with delay of dt seconds
 
         Parameters
         ----------
 
-        dt: float
+        delay: float
             The number of seconds in the timer
         """
-        self.dt = dt
+        self.delay = delay
         self.last_time = time.time()
 
     def is_time(self):
         """
         Returns true if more than self.dt seconds has passed
         since the initialization or last call of successful is_time()
 
         Returns
         -------
         ret: bool
              True if specified amout of time has passed since the
              initialization or last successful is_time() call
         """
         curt = time.time()
-        if curt - self.last_time > self.dt:
+        if curt - self.last_time > self.delay:
             self.last_time = curt
             return True
         return False
 
 
 PrintFnArgs = namedtuple('PrintFnArgs',
                          ['niter', 'short_str', 'mid_str', 'long_str'])
@@ -2270,21 +2270,36 @@
         raise RuntimeError('Incorrect format version')
     if save_ver != DYNESTY_VERSION:
         warnings.warn(
             f'The dynesty version in the checkpoint file ({save_ver})'
             f'does not match the current dynesty version'
             '({DYNESTY_VERSION}). That is *NOT* guaranteed to work')
     if pool is not None:
-        sampler.M = pool.map
-        sampler.pool = pool
-        sampler.loglikelihood.pool = pool
-    else:
-        sampler.loglikelihood.pool = None
-        sampler.pool = None
-        sampler.M = map
+        mapper = pool.map
+    else:
+        mapper = map
+    if hasattr(sampler, 'sampler'):
+        # This is the case of th dynamic sampler
+        # this is better be written as isinstanceof()
+        # but I couldn't do it due to circular imports
+        # TODO
+
+        # Here we are dealing with the special case of dynamic sampler
+        # where it has internal samplers that also need their pool configured
+        # this is the initial sampler
+        samplers = [sampler, sampler.sampler]
+        if sampler.batch_sampler is not None:
+            samplers.append(sampler.batch_sampler)
+    else:
+        samplers = [sampler]
+
+    for cursamp in samplers:
+        cursamp.M = mapper
+        cursamp.pool = pool
+        cursamp.loglikelihood.pool = pool
     return sampler
 
 
 def save_sampler(sampler, fname):
     """
     Save the state of the dynamic sampler in a file
```

### Comparing `dynesty-2.1.1/py/dynesty.egg-info/PKG-INFO` & `dynesty-2.1.2/py/dynesty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynesty
-Version: 2.1.1
+Version: 2.1.2
 Summary: A dynamic nested sampling package for computing Bayesian posteriors and evidences.
 Home-page: https://github.com/joshspeagle/dynesty
 Author: Joshua S Speagle, Sergey E Koposov
 Author-email: j.speagle@utoronto.ca
 License: MIT
 Keywords: nested sampling,dynamic,monte carlo,bayesian,inference,modeling
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dynesty-2.1.1/py/dynesty.egg-info/SOURCES.txt` & `dynesty-2.1.2/py/dynesty.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,9 +36,8 @@
 tests/test_pool.py
 tests/test_printing.py
 tests/test_reflect.py
 tests/test_resume.py
 tests/test_rosenbrock.py
 tests/test_sampling.py
 tests/test_saver.py
-tests/test_volume.py
-tests/test_wedding.py
+tests/test_volume.py
```

### Comparing `dynesty-2.1.1/setup.py` & `dynesty-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_blob.py` & `dynesty-2.1.2/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_dyn.py` & `dynesty-2.1.2/tests/test_dyn.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_egg.py` & `dynesty-2.1.2/tests/test_egg.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_ellipsoid.py` & `dynesty-2.1.2/tests/test_ellipsoid.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,16 +226,19 @@
         lv = rf.monte_carlo_logvol(np.array([cen1, cen2]),
                                    nsamp,
                                    rstate=rstate)[0]
         if D > 2 * r1:
             lvtrue = np.log(2 * r1) * ndim + np.log(2)
         else:
             lvtrue = np.log(2 * r1) * (ndim - 1) + np.log(D + 2 * r1)
-
-        assert (np.abs(lvtrue - lv) < 1e-2)
+        exp_frac = np.exp(lvtrue - (np.log(2 * r1) * ndim + np.log(2)))
+        nexp = exp_frac * nsamp
+        rel_error = 1. / np.sqrt(nexp)
+        threshold = 4
+        assert (np.abs(lvtrue - lv) < threshold * rel_error)
 
 
 def test_bounds():
     rstate = get_rstate()
     Ndim = 20
     Ngood = 10
     eigv = np.abs(rstate.normal(size=Ngood))
```

### Comparing `dynesty-2.1.1/tests/test_gau.py` & `dynesty-2.1.2/tests/test_gau.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_highdim.py` & `dynesty-2.1.2/tests/test_highdim.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_misc.py` & `dynesty-2.1.2/tests/test_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,21 +398,21 @@
             assert np.allclose(val0, val1)
 
 
 @pytest.mark.parametrize('dyn', [False, True])
 def test_update_interval(dyn):
     # test that we can set update_interval
     ndim = 2
-    rstate = get_rstate()
     bigres = {}
     if dyn:
         CL = dynesty.DynamicNestedSampler
     else:
         CL = dynesty.NestedSampler
     for i in range(3):
+        rstate = get_rstate()
         if i == 0:
             update_interval = None
         elif i == 1:
             update_interval = int(.5 * nlive)
         elif i == 2:
             update_interval = .5
         sampler = CL(loglike,
```

### Comparing `dynesty-2.1.1/tests/test_ncdim.py` & `dynesty-2.1.2/tests/test_ncdim.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_notebooks.py` & `dynesty-2.1.2/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_pathology.py` & `dynesty-2.1.2/tests/test_pathology.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_periodic.py` & `dynesty-2.1.2/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_plateau.py` & `dynesty-2.1.2/tests/test_plateau.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_plot.py` & `dynesty-2.1.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_pool.py` & `dynesty-2.1.2/tests/test_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,34 +59,35 @@
                                         ndim,
                                         nlive=nlive,
                                         pool=pool,
                                         queue_size=100,
                                         rstate=rstate)
         sampler.run_nested(dlogz=0.1, print_progress=printing)
 
-        assert (abs(LOGZ_TRUTH_EGG - sampler.results['logz'][-1]) <
-                5. * sampler.results['logzerr'][-1])
+        assert (abs(LOGZ_TRUTH_EGG - sampler.results['logz'][-1])
+                < 5. * sampler.results['logzerr'][-1])
         terminator(pool)
 
 
 def test_pool_x():
     # check without specifying queue_size
     rstate = get_rstate()
 
     with dypool.Pool(2, loglike_egg, prior_transform_egg) as pool:
         sampler = dynesty.NestedSampler(pool.loglike,
                                         pool.prior_transform,
                                         ndim,
                                         nlive=50,
                                         pool=pool,
+                                        queue_size=100,
                                         rstate=rstate)
         sampler.run_nested(print_progress=printing, maxiter=100)
 
-        assert (abs(LOGZ_TRUTH_EGG - sampler.results['logz'][-1]) <
-                5. * sampler.results['logzerr'][-1])
+        assert (abs(LOGZ_TRUTH_EGG - sampler.results['logz'][-1])
+                < 5. * sampler.results['logzerr'][-1])
         terminator(pool)
 
 
 def test_pool_dynamic():
     # test pool on gau problem
     # i specify large queue_size here, otherwise it is too slow
     rstate = get_rstate()
@@ -97,16 +98,16 @@
                                                ndim,
                                                nlive=nlive,
                                                pool=pool,
                                                queue_size=100,
                                                rstate=rstate)
         sampler.run_nested(dlogz_init=1, print_progress=printing)
 
-        assert (abs(LOGZ_TRUTH_GAU - sampler.results['logz'][-1]) <
-                5. * sampler.results['logzerr'][-1])
+        assert (abs(LOGZ_TRUTH_GAU - sampler.results['logz'][-1])
+                < 5. * sampler.results['logzerr'][-1])
         terminator(pool)
 
 
 def loglike_gau_args(x, y, z=None):
     return (-0.5 * np.log(2 * np.pi) * ndim - np.log(gau_s) * ndim -
             0.5 * np.sum((x - 0.5)**2) / gau_s**2) + y + z
 
@@ -132,16 +133,16 @@
                                                ndim,
                                                nlive=nlive,
                                                pool=pool,
                                                queue_size=100,
                                                rstate=rstate)
         sampler.run_nested(maxiter=300, print_progress=printing)
 
-        assert (abs(LOGZ_TRUTH_GAU - sampler.results['logz'][-1]) <
-                5. * sampler.results['logzerr'][-1])
+        assert (abs(LOGZ_TRUTH_GAU - sampler.results['logz'][-1])
+                < 5. * sampler.results['logzerr'][-1])
 
         # to ensure we get coverage
         terminator(pool)
 
 
 @pytest.mark.parametrize('sample', ['slice', 'rwalk', 'rslice'])
 def test_pool_samplers(sample):
@@ -151,19 +152,19 @@
     with mp.Pool(2) as pool:
         sampler = dynesty.NestedSampler(loglike_gau,
                                         prior_transform_gau,
                                         ndim,
                                         nlive=nlive,
                                         sample=sample,
                                         pool=pool,
-                                        queue_size=10,
+                                        queue_size=100,
                                         rstate=rstate)
         sampler.run_nested(print_progress=printing)
-        assert (abs(LOGZ_TRUTH_GAU - sampler.results['logz'][-1]) <
-                5. * sampler.results['logzerr'][-1])
+        assert (abs(LOGZ_TRUTH_GAU - sampler.results['logz'][-1])
+                < 5. * sampler.results['logzerr'][-1])
         terminator(pool)
 
 
 POOL_KW = ['prior_transform', 'loglikelihood', 'propose_point', 'update_bound']
 
 
 @pytest.mark.parametrize('func', POOL_KW)
```

### Comparing `dynesty-2.1.1/tests/test_printing.py` & `dynesty-2.1.2/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_reflect.py` & `dynesty-2.1.2/tests/test_reflect.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_rosenbrock.py` & `dynesty-2.1.2/tests/test_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_sampling.py` & `dynesty-2.1.2/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_saver.py` & `dynesty-2.1.2/tests/test_saver.py`

 * *Files identical despite different names*

### Comparing `dynesty-2.1.1/tests/test_volume.py` & `dynesty-2.1.2/tests/test_volume.py`

 * *Files identical despite different names*

