# Comparing `tmp/biocartograph-0.5.3.tar.gz` & `tmp/biocartograph-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.5.3.tar", last modified: Fri May 19 09:24:42 2023, max compression
+gzip compressed data, was "biocartograph-0.6.0.tar", last modified: Thu Jun  1 15:38:04 2023, max compression
```

## Comparing `biocartograph-0.5.3.tar` & `biocartograph-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.262913 biocartograph-0.5.3/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-01-03 14:01:46.000000 biocartograph-0.5.3/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-19 09:24:42.262913 biocartograph-0.5.3/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-04-04 06:38:15.000000 biocartograph-0.5.3/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.260913 biocartograph-0.5.3/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-19 09:24:42.000000 biocartograph-0.5.3/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-19 09:24:42.262913 biocartograph-0.5.3/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-19 09:14:57.000000 biocartograph-0.5.3/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.259913 biocartograph-0.5.3/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-19 09:24:42.261913 biocartograph-0.5.3/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-03-26 08:32:40.000000 biocartograph-0.5.3/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-03-26 10:38:54.000000 biocartograph-0.5.3/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    20536 2023-05-19 09:17:35.000000 biocartograph-0.5.3/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    27027 2023-05-16 13:50:30.000000 biocartograph-0.5.3/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.872826 biocartograph-0.6.0/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-06-01 15:35:36.000000 biocartograph-0.6.0/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-01 15:38:04.872826 biocartograph-0.6.0/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-06-01 15:35:36.000000 biocartograph-0.6.0/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.872826 biocartograph-0.6.0/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      334 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-06-01 15:38:04.000000 biocartograph-0.6.0/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-06-01 15:38:04.872826 biocartograph-0.6.0/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      955 2023-06-01 15:35:36.000000 biocartograph-0.6.0/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.871826 biocartograph-0.6.0/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-06-01 15:38:04.872826 biocartograph-0.6.0/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)     3334 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/composition.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    22401 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    26154 2023-06-01 15:35:36.000000 biocartograph-0.6.0/src/biocartograph/special.py
```

### Comparing `biocartograph-0.5.3/LICENSE` & `biocartograph-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.3/PKG-INFO` & `biocartograph-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.5.3
+Version: 0.6.0
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.5.3/README.md` & `biocartograph-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.3/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.6.0/biocartograph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.5.3
+Version: 0.6.0
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `biocartograph-0.5.3/setup.py` & `biocartograph-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.5.3",
+    version      = "0.6.0",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
-    package_dir = {'biocartograph':'src/biocartograph','quantification':'src/quantification','special':'src/special','enrichment':'src/enrichment'},
+    package_dir = {	'biocartograph':'src/biocartograph' , 'quantification':'src/quantification' ,
+			'composition':'src/composition' , 'special':'src/special' , 'enrichment':'src/enrichment' },
     classifiers = [
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `biocartograph-0.5.3/src/biocartograph/enrichment.py` & `biocartograph-0.6.0/src/biocartograph/enrichment.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.5.3/src/biocartograph/quantification.py` & `biocartograph-0.6.0/src/biocartograph/quantification.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,77 +117,79 @@
 
 def full_mapping ( adf:pd.DataFrame , jdf:pd.DataFrame ,
         bVerbose:bool = True , bExtreme:bool = True , n_clusters:list[int] = None ,
         n_components:int = None , bUseUmap:bool = False , bPreCompute:bool=True ,
         distance_type:str  = 'covariation' ,
         umap_dimension:int = 2 , umap_n_neighbors:int = 20 , umap_local_connectivity:float = 20. ,
         umap_seed:int = 42 , hierarchy_cmd:str = 'ward' , divergence = lambda r : np.exp(r) ,
-        add_labels:list[str] = None , sample_label:str = None , alignment_label:str = None , bRemoveCurse:bool=False ,
+        add_labels:list[str] = None , sample_label:str = None , alignment_label:str = None ,
+	bRemoveCurse:bool = False , bAuxConsensusPCA:bool=True ,
         n_projections:int = 2 , directory:str = './' , bQN:int = None ,
         nNeighborFilter:list[int] = None , heal_symmetry_break_method:str = 'average' ,
         epls_ownership:str = 'angle' , bNonEuclideanBackprojection:bool = False ,
         Sfunc = lambda x:np.mean(x,0) , bAddPies:bool=False , bUseTDA:bool = False ,
         consensus_function = lambda x:np.sum(x) , consensus_labels:list[str] = None ,
-        bUseGeometricallyCenteredZvalues:bool = False ,
+        bUseGeometricallyCenteredZvalues:bool = False , EPLSformula:str=None ,
         contraction_quantile:float = None   ,
         contraction_depth:float    = None   ) -> tuple[pd.DataFrame] :
     #
-    import biocartograph.special as biox
+    import biocartograph.special	as biox
+    import biocartograph.composition	as bioc
     #
     if bVerbose :
         print ( "TO DISABLE WRITING OF RESULTS TO", directory )
         print ( "SET THE directory=None " )
         print ( "TO MAKE BIOCARTOGRAPH QUIET SET bVerbose=False" )
         import time
         header_str = 'YMDHMS_' + '_'.join( list( str(t) for t in time.gmtime())[:-3] )+'_'
         header_str = 'DMHMSY_' + time.ctime().replace(':','_').replace(' ','_') + '_'
         if not directory is None :
             if not directory[-1] == '/' :
                 directory = directory + '/'
             header_str = directory + header_str
             #
             # HERE WE INCLUDE ALL THE RUN PARAMETERS THAT ARE ACCESIBLE AS INPUTS
-            # AND FROM THE ENVIRONMENT AT THE START OF THE RUN
+            # OR ACCESSIBLE FROM THE ENVIRONMENT AT THE START OF THE RUN
             #
             runinfo_file = 'params.txt'
             run_dict = { 'bVerbose:bool':bVerbose , 'bExtreme:bool':bExtreme , 'n_clusters:list[int]':n_clusters ,
         'n_components:int':n_components , 'bUseUmap:bool':bUseUmap , 'bPreCompute:bool':bPreCompute , 'distance_type:str':distance_type ,
         'umap_dimension:int':umap_dimension , 'umap_n_neighbors:int':umap_n_neighbors , 'umap_local_connectivity:float':umap_local_connectivity ,
         'umap_seed:int':umap_seed , 'hierarchy_cmd:str':hierarchy_cmd , 'divergence:lambda function': divergence ,
         'add_labels:list[str]':add_labels , 'sample_label:str':sample_label , 'alignment_label:str':alignment_label ,
         'bRemoveCurse:bool':bRemoveCurse , 'n_projections:int':n_projections , 'directory:str':directory , 'bQN:int':bQN ,
         'nNeighborFilter:list[int]':nNeighborFilter , 'heal_symmetry_break_method:str':heal_symmetry_break_method ,
         'epls_ownership:str':epls_ownership , 'bNonEuclideanBackprojection:bool':bNonEuclideanBackprojection ,
-        'Sfunc':Sfunc , 'bAddPies:bool':bAddPies , 'bUseTDA':bUseTDA ,
-        'consensus_function':consensus_function , 'consensus_labels:list[str]':consensus_labels ,
-        'bUseGeometricallyCenteredZvalues:bool' : bUseGeometricallyCenteredZvalues ,
+        'Sfunc':Sfunc , 'bAddPies:bool':bAddPies , 'bUseTDA:bool':bUseTDA , 'bAuxConsensusPCA:bool':bAuxConsensusPCA ,
+        'consensus_function':consensus_function , 'consensus_labels:list[str]' : consensus_labels ,
+        'bUseGeometricallyCenteredZvalues:bool' : bUseGeometricallyCenteredZvalues , 'EPLSformula:str':EPLSformula ,
 	'contraction_quantile:float': contraction_quantile , ' contraction_depth:float': contraction_depth }
             ofile = open ( header_str + runinfo_file , 'w' )
             for item in run_dict.items():
                 if 'list' in str(type(item[1])):
                     print ( item[0],'\t=\t [', ','.join([str(i) for i in item[1]]) ,']', file=ofile )
                 else :
                     print ( item[0],'\t=\t [', str(item[1]) ,']', file=ofile )
             print ( 'PYTHON GLOBALS:\n ',
 			'\n'.join([ '\t=\t '.join([str(i) for i in item if not i is None]) for item in globals().items() if not item is None ] ),
 			file = ofile )
     #
-    if bVerbose:
+    if bVerbose :
         print ( "INFORMATION : \t WARNINGS ISSUED AFTER THIS MESSAGE MEANS THAT SOME ITEMS WITH ZERO STANDARD DEVIATION WERE DROPPED\nBEGIN")
     adf = adf.iloc[ np.inf != np.abs( 1.0/np.std(adf.values,1) ) ,
                     np.inf != np.abs( 1.0/np.std(adf.values,0) ) ].copy().apply(pd.to_numeric)
     if bVerbose :
         print ( "END")
     #
     comp_df = None
     if not jdf is None :
         if not ( alignment_label is None ) :
             if bVerbose :
                 print ( "CONDUCTING COMPOSITIONAL ANALYSIS" )
-            comp_df = biox.calculate_compositions ( adf , jdf, label = alignment_label , bAddPies=bAddPies )
+            comp_df = bioc.calculate_compositions ( adf , jdf, label = alignment_label , bAddPies=bAddPies )
             comp_df.columns = [ alignment_label +'.'+ c for c in comp_df.columns.values ]
             if bVerbose :
                 print (  'FINISHED RESULTS > ' , 'composition.tsv' )
             if not directory is None:
                 comp_df .to_csv (  header_str + 'composition.tsv' , sep='\t' )
     #
     if not bQN is None :
@@ -320,40 +322,68 @@
         soldf_s .to_csv( header_str + 'soldf_s.tsv',sep='\t' )
         hierarch_s_df.to_csv( header_str + 'hierarch_s.tsv' , sep='\t' )
     #
     pcas_df , pcaw_df = None , None
     if not jdf is None :
         if not ( alignment_label is None ) :
             if bVerbose :
-                print ( "MULTIVAR ALIGNED PCA" )
+                print ( "MULTIVAR ALIGNED PCA", alignment_label ) # ALWAYS ON ALIGNMENT LABEL
             from impetuous.quantification import multivariate_aligned_pca
             if sample_label is None :
                 jdf.loc['samplenames'] = jdf.columns.values
                 sample_label = 'samplenames'
             pcas_df , pcaw_df = multivariate_aligned_pca ( adf , jdf ,
                     sample_label = sample_label , align_to = alignment_label ,
                     n_components = n_components , add_labels = add_labels )
+            print ( 'DONE' )
+            aux_labels = list( set( consensus_labels ) - set([alignment_label]) )
+            if bAuxConsensusPCA :
+                print ( 'MUTLIVAR AUX ALIGNED PCA: ' , aux_labels  )
+                for a_label in aux_labels :
+                    tmp_pcas_df , tmp_pcaw_df = multivariate_aligned_pca ( adf , jdf ,
+                        sample_label = sample_label , align_to = a_label ,
+                        n_components = n_components , add_labels = add_labels )
+                    tpsdf = tmp_pcas_df.loc[ : , [ c for c in tmp_pcas_df.columns if not 'PCA' in c ] ]
+                    tpsdf .columns = [ 'AUX.'+a_label+'.'+c for c in tpsdf.columns ]
+                    tpwdf = tmp_pcaw_df.loc[ : , [ c for c in tmp_pcaw_df.columns if not 'PCA' in c ] ]
+                    tpwdf.columns = [ 'AUX.'+a_label+'.'+c for c in tpwdf.columns ]
+                    pcas_df = pd.concat([ pcas_df.T, tpsdf.T ]).T
+                    pcaw_df = pd.concat([ pcaw_df.T, tpwdf.T ]).T
+            #
             if bVerbose :
                 print ( "ENCODED PLS REGRESSION" )
             from impetuous.quantification import run_rpls_regression as epls
-            jdf = jdf.rename(index={alignment_label:'AL0xXx'})
-            res = epls ( analyte_df=adf, journal_df=jdf, formula = 'Expression~C(AL0xXx)' , owner_by = epls_ownership )
-            jdf = jdf.rename(index={'AL0xXx':alignment_label})
-            res[0].columns = [ 'EPLS.' + v for v in res[0].columns.values ]
-            res[1].columns = [ 'EPLS.' + v for v in res[1].columns.values ]
+            #
+            L_ = 'abcdefghijklmnopqrstuvwxyz'.upper()
+            idx_rename = None # CREATES AN ACRONYM
+            if EPLSformula is None :
+                formula = "Expression~"
+                epls_labels = [ alignment_label ]
+                idx_rename = { epls_labels[i_] : L_[i_] + "L0xXx" for i_ in range(len( epls_labels )) }
+                for c in idx_rename.values() :
+                    formula +='C('+c+')+'
+                formula = formula[:-1]
+            else :
+                formula = EPLSformula
+            jdf = jdf.rename( index = idx_rename )
+            print ( 'EPLS:', formula )
+            res = epls ( analyte_df=adf, journal_df=jdf , formula = formula , owner_by = epls_ownership )
+            if not idx_rename is None :
+                jdf = jdf.rename( index = {v:k for (k,v) in idx_rename.items() } )
+            res[0] .columns = [ 'EPLS.' + v for v in res[0].columns.values ]
+            res[1] .columns = [ 'EPLS.' + v for v in res[1].columns.values ]
             if bVerbose :
                 print ( 'FINISHED RESULTS > ', 'pcas_df.tsv', 'pcaw_df.tsv', 'epls_f.tsv' , 'epls_s.tsv' )
             if not directory is None:
                 pcas_df .to_csv ( header_str + 'pcas_df.tsv', sep='\t' )
                 pcaw_df .to_csv ( header_str + 'pcaw_df.tsv', sep='\t' )
                 res[ 0 ].to_csv ( header_str + 'epls_f.tsv' , sep='\t' )
                 res[ 1 ].to_csv ( header_str + 'epls_s.tsv' , sep='\t' )
             resdf_f = pd.concat( [resdf_f.T, pcas_df.T , res[0].T , comp_df.T ] ).T
             resdf_s = pd.concat( [resdf_s.T, pcaw_df.T , res[1].T ] ).T
-    #
     if bVerbose :
         print ( 'RETURNING: ')
         print ( 'FEATURE MAP, SAMPLE MAP, FULL FEATURE HIERARCHY, FULL SAMPLE HIERARCHY' )
     if not header_str is None :
         resdf_f .index .name = header_str
     return ( resdf_f , resdf_s , hierarch_f_df, hierarch_s_df , soldf_f , soldf_s )
```

### Comparing `biocartograph-0.5.3/src/biocartograph/special.py` & `biocartograph-0.6.0/src/biocartograph/special.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,28 +106,14 @@
         u_ , s_ , vt_ = np.linalg.svd( b_distm )
         a_distm = distance_calculation ( u_*s_ , 'euclidean' , False , None )
     if a_distm is None :
         a_distm = np.mean(np.array([b_distm,b_distm.T]),0)
     a_distm *= ( 1-np.eye(len(b_distm))>0 )
     return ( a_distm )
 
-def calculate_compositions( adf:pd.DataFrame , jdf:pd.DataFrame , label:str, bAddPies:bool=True ) -> pd.DataFrame :
-    from impetuous.quantification import compositional_analysis
-    from impetuous.quantification import composition_absolute
-    cdf			= composition_absolute ( adf=adf , jdf=jdf , label=label )
-    composition_df      = cdf.T.apply(compositional_analysis).T
-    composition_df .columns = ['Beta','Tau','Gini','Geni','TSI','FILLING']
-    max_quant_df        = cdf.T.apply(lambda x: x.index.values[np.argmax(x)] )
-    composition_df .loc[ max_quant_df.index.values , 'Leading Quantification Label' ] = max_quant_df.values
-    if bAddPies :
-        from impetuous.quantification import composition_piechart
-        fractions_df    = composition_piechart( cdf )
-        return ( pd.concat( [composition_df.T, fractions_df]).T )
-    return ( composition_df )
-
 def pivot_data ( mdf:pd.DataFrame , index:str ='index' , column:str = 'sample', values:str = 'value' ) -> pd.DataFrame :
     pdf = mdf.pivot( index = index , columns = [column] , values = values )
     return ( pdf )
 
 def check_directory ( dir_string:str ,
                       use_exclusion:str = 'pruned' ) -> list :
     check_set  = {'tsv','csv','xlsx'}
@@ -427,30 +413,28 @@
     nn_df = generate_neighbor_distance_df ( df=df , lab=lab , iex=iex , nNN=nNN )
     file_info = sep.join([ str(c) for c in nn_df.columns.values.tolist() ]) + '\n'
     for v in nn_df.values :
         file_info += sep.join( [ str(w) for w in v ] ) + '\n'
     return ( file_info )
 
 
-
 def cluster_center_information ( all_convex_hulls:dict , sep:str = '\t' ) -> str :
     # results/Clustering_results/brain_HPA23v4/UMAP/cluster_centers.tsv
     N           = len( list(all_convex_hulls.items())[0][1]['center'] )
     crdn        = 'xyzuvwabcdefghijklmnopqrst'
     file_info   = ""
     if len( crdn ) < N :
         print ( 'WARNING : THERE IS PROBABLY AN ERROR IN THE HULL CALCULATION ', N , len(crdn) )
     #
     file_info += sep.join( [ 'cluster' , *[ crdn[i] for i in range(N) ] ] ) + '\n'
     for item in all_convex_hulls.items() :
         file_info += str(item[0]) + sep + sep.join([str(v) for v in item[1]['center']] ) + '\n'
     return ( file_info )
 
 
-
 def create_cluster_polygon_information ( all_convex_hulls:dict , sep:str = '\t' ) -> str :
     # results/Clustering_results/brain_HPA23v4/UMAP/UMAP_polygons.tsv
     DIM         = len( list(all_convex_hulls.items())[0][1]['center'] )
     crdn        = 'xyzuvwabcdefghijklmnopqrst'.upper()
     file_info   = ""
     if len( crdn ) < DIM :
         print ( 'WARNING : THERE IS PROBABLY AN ERROR IN THE HULL CALCULATION ', DIM , len(crdn) )
@@ -464,14 +448,15 @@
         M    = len(crds[0])
         crds = np.array(crds).reshape(-1)
         crds = [ [ crds[k*M+i] for k in range(DIM) ] for i in range(M) ]
         for crd in crds :
             file_info += sep.join([ str(item[0]) , '1' , '1' ,'primary' , *[str(c) for c in crd] , '1' , '1' ,   str(item[0])+'_1_1' ]) + '\n'
     return ( file_info )
 
+
 def create_directory ( directory_path:str ) :
     import os
     drsp = directory_path.split('/')
     for i in range( len(drsp) ) :
         if drsp[i] == '.' or drsp[i] == '..' :
             continue
         if len(drsp[:i+1])>0 :
```

