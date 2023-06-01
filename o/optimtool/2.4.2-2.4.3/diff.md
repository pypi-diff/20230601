# Comparing `tmp/optimtool-2.4.2.tar.gz` & `tmp/optimtool-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimtool-2.4.2.tar", last modified: Mon Apr 17 14:54:10 2023, max compression
+gzip compressed data, was "optimtool-2.4.3.tar", last modified: Thu Jun  1 09:48:18 2023, max compression
```

## Comparing `optimtool-2.4.2.tar` & `optimtool-2.4.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.919752 optimtool-2.4.2/
--rw-rw-rw-   0        0        0     1089 2023-04-17 13:50:21.000000 optimtool-2.4.2/LICENSE
--rw-rw-rw-   0        0        0    17700 2023-04-17 14:54:10.903757 optimtool-2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    16392 2023-04-17 14:53:03.000000 optimtool-2.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.723751 optimtool-2.4.2/optimtool/
--rw-rw-rw-   0        0        0     1404 2023-04-17 13:59:09.000000 optimtool-2.4.2/optimtool/__init__.py
--rw-rw-rw-   0        0        0     2802 2023-04-17 14:01:20.000000 optimtool-2.4.2/optimtool/_convert.py
--rw-rw-rw-   0        0        0    10976 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/_drive.py
--rw-rw-rw-   0        0        0     1804 2023-04-17 14:14:24.000000 optimtool-2.4.2/optimtool/_kernel.py
--rw-rw-rw-   0        0        0     8878 2023-04-17 14:42:57.000000 optimtool-2.4.2/optimtool/_search.py
--rw-rw-rw-   0        0        0     1832 2023-04-17 13:55:26.000000 optimtool-2.4.2/optimtool/_typing.py
--rw-rw-rw-   0        0        0     2535 2023-04-17 13:54:24.000000 optimtool-2.4.2/optimtool/_utils.py
--rw-rw-rw-   0        0        0     1132 2023-04-17 13:52:58.000000 optimtool-2.4.2/optimtool/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.820754 optimtool-2.4.2/optimtool/constrain/
--rw-rw-rw-   0        0        0     1177 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/constrain/__init__.py
--rw-rw-rw-   0        0        0     5357 2023-04-17 14:14:47.000000 optimtool-2.4.2/optimtool/constrain/equal.py
--rw-rw-rw-   0        0        0     9429 2023-04-17 14:15:14.000000 optimtool-2.4.2/optimtool/constrain/mixequal.py
--rw-rw-rw-   0        0        0     8216 2023-04-17 14:18:23.000000 optimtool-2.4.2/optimtool/constrain/unequal.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.831758 optimtool-2.4.2/optimtool/example/
--rw-rw-rw-   0        0        0     8263 2023-04-17 14:18:57.000000 optimtool-2.4.2/optimtool/example/Lasso.py
--rw-rw-rw-   0        0        0    10603 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/example/WanYuan.py
--rw-rw-rw-   0        0        0     1153 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.853753 optimtool-2.4.2/optimtool/hybrid/
--rw-rw-rw-   0        0        0     1185 2023-04-17 14:12:40.000000 optimtool-2.4.2/optimtool/hybrid/__init__.py
--rw-rw-rw-   0        0        0     1104 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/hybrid/approximate_point_gradient.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.887751 optimtool-2.4.2/optimtool/unconstrain/
--rw-rw-rw-   0        0        0     1257 2023-04-17 13:50:21.000000 optimtool-2.4.2/optimtool/unconstrain/__init__.py
--rw-rw-rw-   0        0        0     6456 2023-04-17 14:09:25.000000 optimtool-2.4.2/optimtool/unconstrain/gradient_descent.py
--rw-rw-rw-   0        0        0     6034 2023-04-17 14:11:11.000000 optimtool-2.4.2/optimtool/unconstrain/newton.py
--rw-rw-rw-   0        0        0     7656 2023-04-17 14:10:40.000000 optimtool-2.4.2/optimtool/unconstrain/newton_quasi.py
--rw-rw-rw-   0        0        0     5858 2023-04-17 14:28:17.000000 optimtool-2.4.2/optimtool/unconstrain/nonlinear_least_square.py
--rw-rw-rw-   0        0        0     3821 2023-04-17 14:12:08.000000 optimtool-2.4.2/optimtool/unconstrain/trust_region.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:54:10.806333 optimtool-2.4.2/optimtool.egg-info/
--rw-rw-rw-   0        0        0    17700 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      909 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 14:54:10.000000 optimtool-2.4.2/optimtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 14:54:10.920752 optimtool-2.4.2/setup.cfg
--rw-rw-rw-   0        0        0     3048 2023-04-17 14:53:49.000000 optimtool-2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.903978 optimtool-2.4.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-01 09:36:40.000000 optimtool-2.4.3/LICENSE
+-rw-rw-rw-   0        0        0    17700 2023-06-01 09:48:18.901977 optimtool-2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    16392 2023-06-01 09:36:40.000000 optimtool-2.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.833979 optimtool-2.4.3/optimtool/
+-rw-rw-rw-   0        0        0     1401 2023-06-01 09:42:38.000000 optimtool-2.4.3/optimtool/__init__.py
+-rw-rw-rw-   0        0        0     2717 2023-06-01 09:38:12.000000 optimtool-2.4.3/optimtool/_convert.py
+-rw-rw-rw-   0        0        0    10976 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_drive.py
+-rw-rw-rw-   0        0        0     1804 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_kernel.py
+-rw-rw-rw-   0        0        0     8878 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_search.py
+-rw-rw-rw-   0        0        0     1832 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_typing.py
+-rw-rw-rw-   0        0        0     2535 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_utils.py
+-rw-rw-rw-   0        0        0     1132 2023-06-01 09:37:20.000000 optimtool-2.4.3/optimtool/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.870977 optimtool-2.4.3/optimtool/constrain/
+-rw-rw-rw-   0        0        0     1177 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/__init__.py
+-rw-rw-rw-   0        0        0     5357 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/equal.py
+-rw-rw-rw-   0        0        0     9429 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/mixequal.py
+-rw-rw-rw-   0        0        0     8216 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/unequal.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.880986 optimtool-2.4.3/optimtool/example/
+-rw-rw-rw-   0        0        0     8263 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/example/Lasso.py
+-rw-rw-rw-   0        0        0    10603 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/example/WanYuan.py
+-rw-rw-rw-   0        0        0     1153 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.884978 optimtool-2.4.3/optimtool/hybrid/
+-rw-rw-rw-   0        0        0     1172 2023-06-01 09:47:08.000000 optimtool-2.4.3/optimtool/hybrid/__init__.py
+-rw-rw-rw-   0        0        0     1104 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/hybrid/approximate_point_gradient.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.900097 optimtool-2.4.3/optimtool/unconstrain/
+-rw-rw-rw-   0        0        0     1257 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/gradient_descent.py
+-rw-rw-rw-   0        0        0     6034 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/newton.py
+-rw-rw-rw-   0        0        0     7656 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/newton_quasi.py
+-rw-rw-rw-   0        0        0     5858 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/nonlinear_least_square.py
+-rw-rw-rw-   0        0        0     3821 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/trust_region.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.861981 optimtool-2.4.3/optimtool.egg-info/
+-rw-rw-rw-   0        0        0    17700 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      909 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 09:48:18.903978 optimtool-2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     3048 2023-06-01 09:40:55.000000 optimtool-2.4.3/setup.py
```

### Comparing `optimtool-2.4.2/LICENSE` & `optimtool-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/PKG-INFO` & `optimtool-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimtool
-Version: 2.4.2
+Version: 2.4.3
 Summary: The fundamental package for scientific research in optimization.
 Home-page: https://github.com/linjing-lab/optimtool
 Download-URL: https://github.com/linjing-lab/optimtool/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optimtool Version: 2.4.2 Summary: The fundamental
+Metadata-Version: 2.1 Name: optimtool Version: 2.4.3 Summary: The fundamental
 package for scientific research in optimization. Home-page: https://github.com/
 linjing-lab/optimtool Download-URL: https://github.com/linjing-lab/optimtool/
 tags Author: ææ¯ Author-email: linjing010729@163.com License: MIT Project-
 URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
 Project-URL: Tracker, https://github.com/linjing-lab/optimtool/issues
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
```

### Comparing `optimtool-2.4.2/README.md` & `optimtool-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/__init__.py` & `optimtool-2.4.3/optimtool/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 # SOFTWARE.
 
 import sys
 
 from . import constrain
 from . import unconstrain
 from . import example
-from . import hybrid # not implemented yet
+from . import hybrid # appear in v2.5.0
 
 from ._version import __version__
 
 if sys.version_info < (3, 7, 0):
-    raise OSError(f'optimtool-2.4.2 requires Python >=3.7, but yours is {sys.version}')
+    raise OSError(f'optimtool-2.4.3 requires Python >=3.7, but yours is {sys.version}')
```

### Comparing `optimtool-2.4.2/optimtool/_convert.py` & `optimtool-2.4.3/optimtool/_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,34 +66,30 @@
     x_0 : PointArray
         参数
 
     '''
     # convert x_0
     return (x_0,) if not isinstance(x_0, (list, tuple)) else x_0
 
-def h2h(hessian: NDArray, pk: int=1) -> NDArray:
+def h2h(hessian: NDArray) -> NDArray:
     '''
     Parameters
     ----------
     hessian : numpy.array
         未修正的海瑟矩阵值
-        
-    pk : int
-        常数
-        
+
 
     Returns
     -------
     numpy.array
         修正后的海瑟矩阵
         
     '''
     l = hessian.shape[0] # hessian.shape = (l, l)
     while 1:
         rank = np.linalg.matrix_rank(hessian)
         if rank == l:
             break
         else:
-            hessian = hessian + pk * np.identity(l)
-            pk += 1
+            hessian = hessian + np.identity(l)
     return hessian
 __all__ = [f2m, a2m, p2t, h2h]
```

### Comparing `optimtool-2.4.2/optimtool/_drive.py` & `optimtool-2.4.3/optimtool/_drive.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/_kernel.py` & `optimtool-2.4.3/optimtool/_kernel.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/_search.py` & `optimtool-2.4.3/optimtool/_search.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/_typing.py` & `optimtool-2.4.3/optimtool/_typing.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/_utils.py` & `optimtool-2.4.3/optimtool/_utils.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/_version.py` & `optimtool-2.4.3/optimtool/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '2.4.2'
+__version__ = '2.4.3'
```

### Comparing `optimtool-2.4.2/optimtool/constrain/__init__.py` & `optimtool-2.4.3/optimtool/constrain/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/constrain/equal.py` & `optimtool-2.4.3/optimtool/constrain/equal.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/constrain/mixequal.py` & `optimtool-2.4.3/optimtool/constrain/mixequal.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/constrain/unequal.py` & `optimtool-2.4.3/optimtool/constrain/unequal.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/example/Lasso.py` & `optimtool-2.4.3/optimtool/example/Lasso.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/example/WanYuan.py` & `optimtool-2.4.3/optimtool/example/WanYuan.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/example/__init__.py` & `optimtool-2.4.3/optimtool/example/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/hybrid/__init__.py` & `optimtool-2.4.3/optimtool/unconstrain/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,9 +14,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from . import approximate_point_gradient 
-# will be updated in the future
+from . import gradient_descent
+from . import newton
+from . import newton_quasi
+from . import nonlinear_least_square
+from . import trust_region
```

### Comparing `optimtool-2.4.2/optimtool/hybrid/approximate_point_gradient.py` & `optimtool-2.4.3/optimtool/hybrid/approximate_point_gradient.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/unconstrain/__init__.py` & `optimtool-2.4.3/optimtool/hybrid/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,12 +14,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from . import gradient_descent
-from . import newton
-from . import newton_quasi
-from . import nonlinear_least_square
-from . import trust_region
+from . import approximate_point_gradient 
+# appear in v2.5.0
```

### Comparing `optimtool-2.4.2/optimtool/unconstrain/gradient_descent.py` & `optimtool-2.4.3/optimtool/unconstrain/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/unconstrain/newton.py` & `optimtool-2.4.3/optimtool/unconstrain/newton.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/unconstrain/newton_quasi.py` & `optimtool-2.4.3/optimtool/unconstrain/newton_quasi.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/unconstrain/nonlinear_least_square.py` & `optimtool-2.4.3/optimtool/unconstrain/nonlinear_least_square.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool/unconstrain/trust_region.py` & `optimtool-2.4.3/optimtool/unconstrain/trust_region.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/optimtool.egg-info/PKG-INFO` & `optimtool-2.4.3/optimtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimtool
-Version: 2.4.2
+Version: 2.4.3
 Summary: The fundamental package for scientific research in optimization.
 Home-page: https://github.com/linjing-lab/optimtool
 Download-URL: https://github.com/linjing-lab/optimtool/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optimtool Version: 2.4.2 Summary: The fundamental
+Metadata-Version: 2.1 Name: optimtool Version: 2.4.3 Summary: The fundamental
 package for scientific research in optimization. Home-page: https://github.com/
 linjing-lab/optimtool Download-URL: https://github.com/linjing-lab/optimtool/
 tags Author: ææ¯ Author-email: linjing010729@163.com License: MIT Project-
 URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
 Project-URL: Tracker, https://github.com/linjing-lab/optimtool/issues
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
```

### Comparing `optimtool-2.4.2/optimtool.egg-info/SOURCES.txt` & `optimtool-2.4.3/optimtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.2/setup.py` & `optimtool-2.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import sys
 
 from setuptools import setup
 
 if sys.version_info < (3, 7, 0):
-    raise OSError(f'optimtool-2.4.1 requires Python >=3.7, but yours is {sys.version}')
+    raise OSError(f'optimtool-2.4.3 requires Python >=3.7, but yours is {sys.version}')
 
 if (3, 7, 0) <= sys.version_info < (3, 8, 0):
     # https://github.com/pypa/setuptools/issues/926#issuecomment-294369342
     try:
         import fastentrypoints
     except ImportError:
         try:
```

