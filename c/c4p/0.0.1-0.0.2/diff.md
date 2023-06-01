# Comparing `tmp/c4p-0.0.1.tar.gz` & `tmp/c4p-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4p-0.0.1.tar", last modified: Thu Jun  1 04:50:02 2023, max compression
+gzip compressed data, was "c4p-0.0.2.tar", last modified: Thu Jun  1 05:25:59 2023, max compression
```

## Comparing `c4p-0.0.1.tar` & `c4p-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 04:50:02.917358 c4p-0.0.1/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-0.0.1/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      510 2023-06-01 04:50:02.916880 c4p-0.0.1/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       66 2023-05-31 23:29:16.000000 c4p-0.0.1/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 04:50:02.912774 c4p-0.0.1/c4p/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-0.0.1/c4p/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5198 2023-06-01 04:47:25.000000 c4p-0.0.1/c4p/case.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1576 2023-06-01 04:11:06.000000 c4p-0.0.1/c4p/utils.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 04:50:02.916265 c4p-0.0.1/c4p.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      510 2023-06-01 04:50:02.913458 c4p-0.0.1/c4p.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      227 2023-06-01 04:50:02.913966 c4p-0.0.1/c4p.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:50:02.914480 c4p-0.0.1/c4p.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-0.0.1/c4p.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-06-01 04:50:02.915679 c4p-0.0.1/c4p.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-06-01 04:50:02.916381 c4p-0.0.1/c4p.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-06-01 04:50:02.917490 c4p-0.0.1/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      877 2023-06-01 04:12:41.000000 c4p-0.0.1/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 05:25:59.121749 c4p-0.0.2/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-0.0.2/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      510 2023-06-01 05:25:59.121309 c4p-0.0.2/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       66 2023-05-31 23:29:16.000000 c4p-0.0.2/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 05:25:59.117048 c4p-0.0.2/c4p/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-0.0.2/c4p/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5920 2023-06-01 05:24:39.000000 c4p-0.0.2/c4p/case.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1576 2023-06-01 04:11:06.000000 c4p-0.0.2/c4p/utils.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 05:25:59.120715 c4p-0.0.2/c4p.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      510 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      227 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-0.0.2/c4p.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-06-01 05:25:59.121878 c4p-0.0.2/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      877 2023-06-01 05:16:11.000000 c4p-0.0.2/setup.py
```

### Comparing `c4p-0.0.1/LICENSE` & `c4p-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c4p-0.0.1/c4p/case.py` & `c4p-0.0.2/c4p/case.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,27 @@
                   url_plotrdirc_ncl='https://github.com/CESM-Development/paleoToolkit/trunk/cesm1_2/rof/plot_rdirc.ncl',
                   url_rtm_ncdf_pro='https://github.com/CESM-Development/paleoToolkit/trunk/cesm1_2/rof/rtm_ncdf.pro',
                   url_runoff_map='https://github.com/CESM-Development/paleoToolkit/trunk/cesm1_2/rof/runoff_map_1deg',
                   url_runoff_map_template_nml='https://github.com/CESM-Development/paleoToolkit/trunk/cesm1_2/rof/runoff_map.1x1.template.nml',
                   url_create_ESMF_map_sh='https://github.com/CESM-Development/paleoToolkit/trunk/cesm1_2/rof/create_ESMF_map.sh',
                   ):
         # Step 19
+        utils.p_header('>>> Prep topo file at proper resolution ...')
         fpath = utils.svn_export(url_create_topo_ncl)
         utils.replace_str(
             fpath,
             {
                 '<casename>': self.casename,
                 '<input_topo-bath_filename>': topo_path,
             },
         )
-        utils.run_shell(f'ncl {fpath}', timeout=3)
+        utils.run_shell(f'source /glade/u/apps/ch/opt/lmod/8.7.13/lmod/lmod/init/zsh && module load ncl && ncl {fpath}', timeout=3)
         
         # Step 20
+        utils.p_header('>>> Generate runoff data from topo inputs ...')
         fpath_new = utils.svn_export(url_rdirc_template_csh, f'./rdirc_{self.casename}.csh')
         utils.replace_str(
             fpath_new,
             {
                 '<casename>': self.casename,
                 '<path/topography-bathymetry_file>': f'topo.1x1deg.{self.casename}.nc',
             },
@@ -53,20 +55,22 @@
             },
         )
 
         utils.svn_export(url_Makefile)
         utils.exec_script(fpath_new)
 
         # Step 21
+        utils.p_header('>>> Plot runoff ...')
         fpath = utils.svn_export(url_plotrdirc_csh)
         utils.replace_str(
             fpath,
             {
                 '<casename>': self.casename,
                 '<topography-bathymetry_file>': os.path.basename(topo_path),
+                'ncl < plot_rdirc.ncl': '/glade/u/apps/ch/opt/ncl/6.6.2/intel/19.1.1/bin/ncl < plot_rdirc.ncl',
             },
         )
         fpath_ncl = utils.svn_export(url_plotrdirc_ncl)
 
         # output png instead of ps
         utils.replace_str(
             fpath_ncl,
@@ -74,14 +78,15 @@
                 'PSName= "ps"': 'PSName= "png"',
             },
         )
 
         utils.exec_script(fpath)
 
         # Step 24
+        utils.p_header('>>> Convert runoff file to netcdf ...')
         fpath = utils.svn_export(url_rtm_ncdf_pro)
         
         utils.replace_str(
             fpath,
             {
                 '<casename>': self.casename,
                 '<user>': 'Feng Zhu',
@@ -90,14 +95,15 @@
             },
         )
 
         # run IDL
         utils.run_shell('source /glade/u/apps/ch/opt/lmod/8.7.13/lmod/lmod/init/zsh && module load idl && printf ".rn rtm_ncdf\nrtm\nexit\n" | idl')
 
         # Step 25
+        utils.p_header('>>> Create runoff to ocean mapping file (part 1) ...')
         fpath = utils.svn_export(url_runoff_map)
         fpath_new = utils.svn_export(url_runoff_map_template_nml,  f'./runoff_map.1x1.{self.casename}.nml')
         utils.replace_str(
             fpath_new,
             {
                 '<casename>': self.casename,
                 './<SCRIP_mapping_file>': ocn_scrp_path,
@@ -105,21 +111,23 @@
                 '<date>': '20230514',
             },
         )
         utils.run_shell(f'ln -s {fpath_new} ./runoff_map.nml')
         utils.exec_script(fpath)
 
         # Step 26
+        utils.p_header('>>> Create runoff to ocean mapping file (part 2) ...')
         fpath = utils.svn_export(url_create_ESMF_map_sh)
         ocnres = f'gx1{self.casename}'
         fsrc = os.path.join(grids_dirpath, '1x1d.nc')
         fdst = ocn_scrp_path
         utils.exec_script(fpath, args=f'-fsrc {fsrc} -nsrc r1_nomask -fdst {fdst} -ndst {ocnres} -map aave')
 
         # Step 27
+        utils.p_header('>>> Create runoff to/from land mapping files - needed if rof at 1deg rather than 0.5 deg ...')
         fsrc = os.path.join(grids_dirpath, 'fv1.9x2.5_141008.nc')
         fdst = os.path.join(grids_dirpath, '1x1d_lonshift.nc')
         utils.exec_script(fpath, args=f'-fsrc {fsrc} -nsrc r19_nomask -fdst {fdst} -ndst r1x1 -map aave')
 
         fsrc = os.path.join(grids_dirpath, '1x1d_lonshift.nc')
         fdst = os.path.join(grids_dirpath, 'fv1.9x2.5_141008.nc')
         utils.exec_script(fpath, args=f' -fsrc {fsrc} -nsrc r1x1 -fdst {fdst} -ndst r19 -map aave')
```

### Comparing `c4p-0.0.1/c4p/utils.py` & `c4p-0.0.2/c4p/utils.py`

 * *Files identical despite different names*

### Comparing `c4p-0.0.1/setup.py` & `c4p-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='c4p',  # required
-    version='0.0.1',
+    version='0.0.2',
     description='c4p: CESM for Paleo',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Jiang Zhu',
     author_email='fengzhu@ucar.edu, jiangzhu@ucar.edu',
     url='https://github.com/fzhu2e/cesm4paleo',
     packages=find_packages(),
```

