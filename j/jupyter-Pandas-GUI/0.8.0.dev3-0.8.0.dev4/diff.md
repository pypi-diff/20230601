# Comparing `tmp/jupyter_Pandas_GUI-0.8.0.dev3.tar.gz` & `tmp/jupyter_Pandas_GUI-0.8.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev3.tar", last modified: Tue May 23 17:55:40 2023, max compression
+gzip compressed data, was "jupyter_Pandas_GUI-0.8.0.dev4.tar", last modified: Wed May 31 22:03:24 2023, max compression
```

## Comparing `jupyter_Pandas_GUI-0.8.0.dev3.tar` & `jupyter_Pandas_GUI-0.8.0.dev4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 17:55:40.516985 jupyter_Pandas_GUI-0.8.0.dev3/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev3/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 17:55:40.516985 jupyter_Pandas_GUI-0.8.0.dev3/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8312 2023-05-22 02:01:29.000000 jupyter_Pandas_GUI-0.8.0.dev3/README.md
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 17:55:40.512985 jupyter_Pandas_GUI-0.8.0.dev3/jupyter_Pandas_GUI.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9058 2023-05-23 17:55:40.000000 jupyter_Pandas_GUI-0.8.0.dev3/jupyter_Pandas_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-23 17:55:40.000000 jupyter_Pandas_GUI-0.8.0.dev3/jupyter_Pandas_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-23 17:55:40.000000 jupyter_Pandas_GUI-0.8.0.dev3/jupyter_Pandas_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-23 17:55:40.000000 jupyter_Pandas_GUI-0.8.0.dev3/jupyter_Pandas_GUI.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-23 17:55:40.000000 jupyter_Pandas_GUI-0.8.0.dev3/jupyter_Pandas_GUI.egg-info/top_level.txt
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-23 17:55:40.516985 jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49923 2023-05-23 14:11:00.000000 jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/fit_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/new_pandas_column_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/plot_Pandas_GUI.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14252 2023-05-23 17:50:14.000000 jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-23 17:55:40.516985 jupyter_Pandas_GUI-0.8.0.dev3/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1325 2023-05-23 17:55:34.000000 jupyter_Pandas_GUI-0.8.0.dev3/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    35149 2020-05-31 15:03:56.000000 jupyter_Pandas_GUI-0.8.0.dev4/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9816 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9070 2023-05-31 21:59:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/README.md
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-31 22:03:24.258275 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     9816 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      373 2023-05-31 22:03:24.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      156 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       11 2023-05-31 22:03:23.000000 jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      568 2022-12-18 21:05:47.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    49800 2023-05-24 21:34:46.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/fit_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    12021 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/new_pandas_column_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    29470 2023-05-21 02:08:14.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/plot_Pandas_GUI.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14252 2023-05-23 17:50:14.000000 jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-31 22:03:24.262275 jupyter_Pandas_GUI-0.8.0.dev4/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1325 2023-05-31 21:48:40.000000 jupyter_Pandas_GUI-0.8.0.dev4/setup.py
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/LICENSE` & `jupyter_Pandas_GUI-0.8.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev4/jupyter_Pandas_GUI.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyter_Pandas_GUI
-Version: 0.8.0.dev3
+Name: jupyter-Pandas-GUI
+Version: 0.8.0.dev4
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 
 The user can pass the GUI tools a list of Pandas 
 DataFrames to work with. If nothing is passed, the GUI will look for 
 Pandas DataFrames in the interactive session. In classic Jupyter the whole GUI 
 and the Jupyter cell that created it are deleted when done. This leaves 
 only the code that was generated by the GUI and the results of running the
 generated code. In Colab and Lab the code is generated in an editable text 
-box. In Colab it can be run by clicking a button. In Lab it is best to copy 
+box. In Lab it can be run by clicking a button. In Colab it is best to copy 
 the code into a new cell before running it.
 
 The generated code contains comments meant to help new users 
 understand the code.
 
 *Currently defined GUIs:*
 
@@ -154,14 +154,22 @@
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
 * 0.8.0dev (2023-5-)
   * In Jupyter Lab results of running code now replace the GUI rather than 
     appearing in the Console.
+  * Colab behavior has been inconsistent. To avoid problems for the time being 
+    the user is required to copy the code from the textbox it is created in 
+    and paste it into an empty code cell to run it.
+  * BUG FIX: collapsed "code that was run" box in Lab now keeps raw html 
+    codes, so when copied and pasted output formatting is maintained.
+  * Changes to avoid warnings caused by JSON having no representation for 
+    floating point infinity and not-a-number.
+  * Documentation updates to reflect changes.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
     does not yet work in Google Colab.
@@ -190,14 +198,20 @@
   * Readme updates.
 * 0.5.0 Initial beta release.
 
 ## Issues or comments
 
 [JupyterPhysSciLab/jupyter_Pandas_GUI/issues](https://github.com/JupyterPhysSciLab/jupyter_Pandas_GUI/issues)
 
+### Known issues
+* In Google Colabratory images in point styles buttons do not show up. This 
+  is a related to a known [issue with
+  Colab](https://github.com/googlecolab/colabtools/issues/1302). Fix will 
+  depend on updates to Colab.
+
 ## [This software is distributed under the GNU V3 license](https://gnu.org/licenses)
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/README.md` & `jupyter_Pandas_GUI-0.8.0.dev4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 The user can pass the GUI tools a list of Pandas 
 DataFrames to work with. If nothing is passed, the GUI will look for 
 Pandas DataFrames in the interactive session. In classic Jupyter the whole GUI 
 and the Jupyter cell that created it are deleted when done. This leaves 
 only the code that was generated by the GUI and the results of running the
 generated code. In Colab and Lab the code is generated in an editable text 
-box. In Colab it can be run by clicking a button. In Lab it is best to copy 
+box. In Lab it can be run by clicking a button. In Colab it is best to copy 
 the code into a new cell before running it.
 
 The generated code contains comments meant to help new users 
 understand the code.
 
 *Currently defined GUIs:*
 
@@ -135,14 +135,22 @@
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
 * 0.8.0dev (2023-5-)
   * In Jupyter Lab results of running code now replace the GUI rather than 
     appearing in the Console.
+  * Colab behavior has been inconsistent. To avoid problems for the time being 
+    the user is required to copy the code from the textbox it is created in 
+    and paste it into an empty code cell to run it.
+  * BUG FIX: collapsed "code that was run" box in Lab now keeps raw html 
+    codes, so when copied and pasted output formatting is maintained.
+  * Changes to avoid warnings caused by JSON having no representation for 
+    floating point infinity and not-a-number.
+  * Documentation updates to reflect changes.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
     does not yet work in Google Colab.
@@ -171,14 +179,20 @@
   * Readme updates.
 * 0.5.0 Initial beta release.
 
 ## Issues or comments
 
 [JupyterPhysSciLab/jupyter_Pandas_GUI/issues](https://github.com/JupyterPhysSciLab/jupyter_Pandas_GUI/issues)
 
+### Known issues
+* In Google Colabratory images in point styles buttons do not show up. This 
+  is a related to a known [issue with
+  Colab](https://github.com/googlecolab/colabtools/issues/1302). Fix will 
+  depend on updates to Colab.
+
 ## [This software is distributed under the GNU V3 license](https://gnu.org/licenses)
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/jupyter_Pandas_GUI.egg-info/PKG-INFO` & `jupyter_Pandas_GUI-0.8.0.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyter-Pandas-GUI
-Version: 0.8.0.dev3
+Name: jupyter_Pandas_GUI
+Version: 0.8.0.dev4
 Summary: Pandas expression composers using Jupyter widgets.
 Home-page: https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Keywords: fitting,data-analysis,plotting,learning to code
 Classifier: Development Status :: 4 - Beta
@@ -47,15 +47,15 @@
 
 The user can pass the GUI tools a list of Pandas 
 DataFrames to work with. If nothing is passed, the GUI will look for 
 Pandas DataFrames in the interactive session. In classic Jupyter the whole GUI 
 and the Jupyter cell that created it are deleted when done. This leaves 
 only the code that was generated by the GUI and the results of running the
 generated code. In Colab and Lab the code is generated in an editable text 
-box. In Colab it can be run by clicking a button. In Lab it is best to copy 
+box. In Lab it can be run by clicking a button. In Colab it is best to copy 
 the code into a new cell before running it.
 
 The generated code contains comments meant to help new users 
 understand the code.
 
 *Currently defined GUIs:*
 
@@ -154,14 +154,22 @@
 install -e ../jupyter_Pandas_GUI` in the _Production_
 instructions.
 
 ## Change Log
 * 0.8.0dev (2023-5-)
   * In Jupyter Lab results of running code now replace the GUI rather than 
     appearing in the Console.
+  * Colab behavior has been inconsistent. To avoid problems for the time being 
+    the user is required to copy the code from the textbox it is created in 
+    and paste it into an empty code cell to run it.
+  * BUG FIX: collapsed "code that was run" box in Lab now keeps raw html 
+    codes, so when copied and pasted output formatting is maintained.
+  * Changes to avoid warnings caused by JSON having no representation for 
+    floating point infinity and not-a-number.
+  * Documentation updates to reflect changes.
 * 0.7.1 (2022-12-18)
   * Documentation fixes and link updates for mybinder.org launches.
   * Updates to requirements.
 * 0.7.0
   * GUIs now also work in Jupyter Lab and Google Colab, although less 
     elegently than in classic Jupyter. Only the fit range selection tab 
     does not yet work in Google Colab.
@@ -190,14 +198,20 @@
   * Readme updates.
 * 0.5.0 Initial beta release.
 
 ## Issues or comments
 
 [JupyterPhysSciLab/jupyter_Pandas_GUI/issues](https://github.com/JupyterPhysSciLab/jupyter_Pandas_GUI/issues)
 
+### Known issues
+* In Google Colabratory images in point styles buttons do not show up. This 
+  is a related to a known [issue with
+  Colab](https://github.com/googlecolab/colabtools/issues/1302). Fix will 
+  depend on updates to Colab.
+
 ## [This software is distributed under the GNU V3 license](https://gnu.org/licenses)
 This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/__init__.py` & `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/fit_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/fit_Pandas_GUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+
 import numpy as np
 
 def calcresid(result):
     '''
     lmfit has empty values for residuals where the weighting is infinite or not defined.
     This calculates all the residuals based on the actual data and fit results.
 
@@ -519,36 +521,28 @@
             guesses and constraints.
         :return VBox: params_set with fields reset and those available visible.
         '''
         currmodel = getattr(models,modelname)()
         currmodel_param = []
         labeltext = ''
         fix = False
-        value = np.nan
-        min = -np.inf
-        max = np.inf
+        value = 0
+        min = -sys.float_info.max
+        max = sys.float_info.max
         expr = None  # Not used, maybe for arbitrary functions.
         for i in range(0,8):
             fix = False
-            if modelname == 'PolynomialModel':
-                # PolynomialModel requires that the initial value be a number
-                value = 0
-            else:
-                value = np.nan
-            min = -np.inf
-            max = np.inf
-            expr = None  # Not used, maybe for arbitrary functions.
             if i < len(currmodel.param_names):
                 labeltext = str(currmodel.param_names[i])
                 hints = currmodel.param_hints.get(labeltext,None)
                 if isinstance(hints,dict):
                     fix = not(hints.get('vary',True))
-                    value = hints.get('value',np.nan)
-                    min = hints.get('min',-np.inf)
-                    max = hints.get('max',np.inf)
+                    value = hints.get('value', 0)
+                    min = hints.get('min', -sys.float_info.max)
+                    max = hints.get('max', sys.float_info.max)
                     expr = hints.get('expr',None)
                 params_set.children[i].layout.display=''
                 if modelname == 'ExponentialModel':
                     df = friendly_to_object[whichframe.value]
                     xvals = df[Xcoord.value]
                     yvals = df[Ycoord.value]
                     if labeltext == 'amplitude':
@@ -571,29 +565,30 @@
         1. fixcheck (checkbox for fixing the value)
         2. valuefield (floatText for setting the value)
         3. minfield (floatText for setting the minimum allowed value)
         4. maxfield (floatText for setting the maximum allowed value)
         By default the all VBox components have their `layout.display=none`.
         :return: VBox
         '''
+        import sys
         currmodel_param=[]
         for i in range (0,8):
             fixcheck = Checkbox(value=False,
                                 description='Fix (hold)',
                                 disabled=False,
                                 style=longdesc)
-            valuefield = FloatText(value=np.nan,
+            valuefield = FloatText(value=0,
                                    description='Value: ',
                                    disabled=False,
                                    style=longdesc)
-            minfield = FloatText(value=-np.inf,
+            minfield = FloatText(value=-sys.float_info.max,
                                  description='Min: ',
                                  disabled=False,
                                  style=longdesc)
-            maxfield = FloatText(value=np.inf,
+            maxfield = FloatText(value=sys.float_info.max,
                                  description='Max: ',
                                  disabled=False,
                                  style=longdesc)
             paramlabel = Label(value = str(i)+':',style=longdesc)
             parambox =  VBox(children=[paramlabel, HBox(children=[fixcheck,valuefield,minfield,
                                     maxfield])])
             parambox.layout.display = 'none'
@@ -805,28 +800,30 @@
                     yerrvalue.value) + '\n\n'
             if yerrtype.value == 'data':
                 step2str += 'Yerr = ' + dfname +'[\"'
                 step2str += str(yerrdata.value)+'\"]\n\n'
             pass
         if change['old']== 2:
             # update step 3 string
-            step3str = '# Define the fit model, initial guesses, and contraints\n'
+            step3str = '# Define the fit model, initial guesses, ' \
+                       'and constraints\n'
             step3str += 'fitmod = lmfit.models.'+str(modeldrop.value)+'()\n'
             currmodel = getattr(models, str(modeldrop.value))()
             for k in params_set.children:
                 param_name = str(k.children[0].value.split(':')[0])
                 if param_name in currmodel.param_names:
                     step3str += 'fitmod.set_param_hint(\"'+param_name+'\",'
                     step3str += ' vary = '+str(not(k.children[1].children[
                         0].value))
                     temp_val = k.children[1].children[1].value
                     def tst_temp_val(temp_val):
                         if (temp_val != np.nan) and (temp_val != np.inf) and\
-                                (temp_val != -np.inf) and (str(temp_val) != \
-                                'nan'):
+                                (temp_val != -np.inf) and (temp_val != \
+                                -sys.float_info.max) and (temp_val != \
+                                sys.float_info.max):
                             return True
                         else:
                             return False
                     if tst_temp_val(temp_val):
                         step3str += ', value = ' + str(temp_val)
                     temp_val = k.children[1].children[2].value
                     if tst_temp_val(temp_val):
@@ -906,17 +903,17 @@
                     xstr = 'Xfitdata'
                     if not(extend_fit.value):
                         step5str += '# Delete residuals in ranges not fit\n'
                         step5str += '# and fit values that are not ' \
                                     'displayed.\n'
                         step5str += 'for i in range(len(resid)):\n'
                         step5str += '    if np.isnan(Xfitdata[i]):\n'
-                        step5str += '        resid[i] = np.nan\n'
+                        step5str += '        resid[i] = None\n'
                         step5str += '        '+str(fitname)+'.best_fit[i] = ' \
-                                                   'np.nan\n\n'
+                                                   'None\n\n'
                 else:
                     xstr = 'Xvals'
                 errbarstr = ''
                 if yerrtype.value!='none':
                     errbarstr = ', error_y_type=\"data\", error_y_array=Yerr'
                 xresidstr = xstr
                 if extend_fit.value:
```

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/new_pandas_column_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/new_pandas_column_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/plot_Pandas_GUI.py` & `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/plot_Pandas_GUI.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/pandas_GUI/utils.py` & `jupyter_Pandas_GUI-0.8.0.dev4/pandas_GUI/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_Pandas_GUI-0.8.0.dev3/setup.py` & `jupyter_Pandas_GUI-0.8.0.dev4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="jupyter_Pandas_GUI",
-    version="0.8.0dev3",
+    version="0.8.0dev4",
     description="Pandas expression composers using Jupyter widgets.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://jupyterphysscilab.github.io/jupyter_Pandas_GUI/",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="fitting, data-analysis, plotting, learning to code",
```

