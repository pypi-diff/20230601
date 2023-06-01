# Comparing `tmp/optimtool-2.4.3.tar.gz` & `tmp/optimtool-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimtool-2.4.3.tar", last modified: Thu Jun  1 09:48:18 2023, max compression
+gzip compressed data, was "optimtool-2.4.4.tar", last modified: Thu Jun  1 11:29:25 2023, max compression
```

## Comparing `optimtool-2.4.3.tar` & `optimtool-2.4.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.903978 optimtool-2.4.3/
--rw-rw-rw-   0        0        0     1089 2023-06-01 09:36:40.000000 optimtool-2.4.3/LICENSE
--rw-rw-rw-   0        0        0    17700 2023-06-01 09:48:18.901977 optimtool-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0    16392 2023-06-01 09:36:40.000000 optimtool-2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.833979 optimtool-2.4.3/optimtool/
--rw-rw-rw-   0        0        0     1401 2023-06-01 09:42:38.000000 optimtool-2.4.3/optimtool/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-06-01 09:38:12.000000 optimtool-2.4.3/optimtool/_convert.py
--rw-rw-rw-   0        0        0    10976 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_drive.py
--rw-rw-rw-   0        0        0     1804 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_kernel.py
--rw-rw-rw-   0        0        0     8878 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_search.py
--rw-rw-rw-   0        0        0     1832 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_typing.py
--rw-rw-rw-   0        0        0     2535 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/_utils.py
--rw-rw-rw-   0        0        0     1132 2023-06-01 09:37:20.000000 optimtool-2.4.3/optimtool/_version.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.870977 optimtool-2.4.3/optimtool/constrain/
--rw-rw-rw-   0        0        0     1177 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/__init__.py
--rw-rw-rw-   0        0        0     5357 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/equal.py
--rw-rw-rw-   0        0        0     9429 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/mixequal.py
--rw-rw-rw-   0        0        0     8216 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/constrain/unequal.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.880986 optimtool-2.4.3/optimtool/example/
--rw-rw-rw-   0        0        0     8263 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/example/Lasso.py
--rw-rw-rw-   0        0        0    10603 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/example/WanYuan.py
--rw-rw-rw-   0        0        0     1153 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.884978 optimtool-2.4.3/optimtool/hybrid/
--rw-rw-rw-   0        0        0     1172 2023-06-01 09:47:08.000000 optimtool-2.4.3/optimtool/hybrid/__init__.py
--rw-rw-rw-   0        0        0     1104 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/hybrid/approximate_point_gradient.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.900097 optimtool-2.4.3/optimtool/unconstrain/
--rw-rw-rw-   0        0        0     1257 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/__init__.py
--rw-rw-rw-   0        0        0     6456 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/gradient_descent.py
--rw-rw-rw-   0        0        0     6034 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/newton.py
--rw-rw-rw-   0        0        0     7656 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/newton_quasi.py
--rw-rw-rw-   0        0        0     5858 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/nonlinear_least_square.py
--rw-rw-rw-   0        0        0     3821 2023-06-01 09:36:40.000000 optimtool-2.4.3/optimtool/unconstrain/trust_region.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:48:18.861981 optimtool-2.4.3/optimtool.egg-info/
--rw-rw-rw-   0        0        0    17700 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      909 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-01 09:48:18.000000 optimtool-2.4.3/optimtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:48:18.903978 optimtool-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0     3048 2023-06-01 09:40:55.000000 optimtool-2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:29:25.598907 optimtool-2.4.4/
+-rw-rw-rw-   0        0        0     1089 2023-06-01 10:20:40.000000 optimtool-2.4.4/LICENSE
+-rw-rw-rw-   0        0        0    17769 2023-06-01 11:29:25.597400 optimtool-2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0    16461 2023-06-01 11:20:13.000000 optimtool-2.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 11:29:25.511377 optimtool-2.4.4/optimtool/
+-rw-rw-rw-   0        0        0     1401 2023-06-01 10:47:27.000000 optimtool-2.4.4/optimtool/__init__.py
+-rw-rw-rw-   0        0        0     2717 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/_convert.py
+-rw-rw-rw-   0        0        0    10976 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/_drive.py
+-rw-rw-rw-   0        0        0     3231 2023-06-01 11:16:08.000000 optimtool-2.4.4/optimtool/_kernel.py
+-rw-rw-rw-   0        0        0     8878 2023-06-01 10:26:33.000000 optimtool-2.4.4/optimtool/_search.py
+-rw-rw-rw-   0        0        0     1832 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/_typing.py
+-rw-rw-rw-   0        0        0     2535 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/_utils.py
+-rw-rw-rw-   0        0        0     1132 2023-06-01 10:47:21.000000 optimtool-2.4.4/optimtool/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:29:25.567438 optimtool-2.4.4/optimtool/constrain/
+-rw-rw-rw-   0        0        0     1177 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/constrain/__init__.py
+-rw-rw-rw-   0        0        0     5324 2023-06-01 11:17:40.000000 optimtool-2.4.4/optimtool/constrain/equal.py
+-rw-rw-rw-   0        0        0     9416 2023-06-01 11:18:10.000000 optimtool-2.4.4/optimtool/constrain/mixequal.py
+-rw-rw-rw-   0        0        0     8240 2023-06-01 11:18:26.000000 optimtool-2.4.4/optimtool/constrain/unequal.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:29:25.574373 optimtool-2.4.4/optimtool/example/
+-rw-rw-rw-   0        0        0     8263 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/example/Lasso.py
+-rw-rw-rw-   0        0        0    10603 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/example/WanYuan.py
+-rw-rw-rw-   0        0        0     1153 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:29:25.580378 optimtool-2.4.4/optimtool/hybrid/
+-rw-rw-rw-   0        0        0     1172 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/hybrid/__init__.py
+-rw-rw-rw-   0        0        0     1104 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/hybrid/approximate_point_gradient.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:29:25.595373 optimtool-2.4.4/optimtool/unconstrain/
+-rw-rw-rw-   0        0        0     1257 2023-06-01 10:20:40.000000 optimtool-2.4.4/optimtool/unconstrain/__init__.py
+-rw-rw-rw-   0        0        0     6797 2023-06-01 11:08:02.000000 optimtool-2.4.4/optimtool/unconstrain/gradient_descent.py
+-rw-rw-rw-   0        0        0     6300 2023-06-01 10:36:11.000000 optimtool-2.4.4/optimtool/unconstrain/newton.py
+-rw-rw-rw-   0        0        0     7842 2023-06-01 10:40:29.000000 optimtool-2.4.4/optimtool/unconstrain/newton_quasi.py
+-rw-rw-rw-   0        0        0     5836 2023-06-01 10:42:09.000000 optimtool-2.4.4/optimtool/unconstrain/nonlinear_least_square.py
+-rw-rw-rw-   0        0        0     3885 2023-06-01 10:42:48.000000 optimtool-2.4.4/optimtool/unconstrain/trust_region.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:29:25.557078 optimtool-2.4.4/optimtool.egg-info/
+-rw-rw-rw-   0        0        0    17769 2023-06-01 11:29:25.000000 optimtool-2.4.4/optimtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      909 2023-06-01 11:29:25.000000 optimtool-2.4.4/optimtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:29:25.000000 optimtool-2.4.4/optimtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 11:29:25.000000 optimtool-2.4.4/optimtool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2023-06-01 11:29:25.000000 optimtool-2.4.4/optimtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-01 11:29:25.000000 optimtool-2.4.4/optimtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 11:29:25.598907 optimtool-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     3048 2023-06-01 10:47:08.000000 optimtool-2.4.4/setup.py
```

### Comparing `optimtool-2.4.3/LICENSE` & `optimtool-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/PKG-INFO` & `optimtool-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimtool
-Version: 2.4.3
+Version: 2.4.4
 Summary: The fundamental package for scientific research in optimization.
 Home-page: https://github.com/linjing-lab/optimtool
 Download-URL: https://github.com/linjing-lab/optimtool/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
@@ -125,15 +125,15 @@
 ou.gradient_descent.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                 | 解释                                   |
 | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                                                             | 通过解方程的方式来求解精确步长                      |
 | steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                           | 使用线搜索方法求解非精确步长（默认使用wolfe线搜索）         |
-| barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
+| barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, M: int=20, eta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
 
 #### 牛顿法（newton）
 
 ```python
 ou.newton.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
@@ -187,40 +187,40 @@
 
 ```python
 oc.equal.[函数名]([目标函数], [参数表], [等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                   | 解释        |
 | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=2, epsk: float=1e-4, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 不等式约束（unequal）
 
 ```python
 oc.unequal.[函数名]([目标函数], [参数表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                      | 解释        |
 | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------- |
-| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
-| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
-| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.4, epsk: float=1e-4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
+| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=12, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
+| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 混合等式约束（mixequal）
 
 ```python
 oc.mixequal.[函数名]([目标函数], [参数表], [等式约束表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                                                  | 解释        |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
-| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
-| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
+| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=1, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
+| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 ### 方法的应用（example）
 
 ```python
 import optimtool.example as oe
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optimtool Version: 2.4.3 Summary: The fundamental
+Metadata-Version: 2.1 Name: optimtool Version: 2.4.4 Summary: The fundamental
 package for scientific research in optimization. Home-page: https://github.com/
 linjing-lab/optimtool Download-URL: https://github.com/linjing-lab/optimtool/
 tags Author: ææ¯ Author-email: linjing010729@163.com License: MIT Project-
 URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
 Project-URL: Tracker, https://github.com/linjing-lab/optimtool/issues
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
@@ -60,15 +60,16 @@
 bool=False, epsilon: float=1e-10, k: int=0) -> OutputType |
 éè¿è§£æ¹ç¨çæ¹å¼æ¥æ±è§£ç²¾ç¡®æ­¥é¿ | | steepest(funcs: FuncArray,
 args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
 str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨çº¿æç´¢æ¹æ³æ±è§£éç²¾ç¡®æ­¥é¿ï¼é»è®¤ä½¿ç¨wolfeçº¿æç´¢ï¼ | |
 barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta:
-float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType |
+float=0.6, M: int=20, eta: float=0.6, alpha: float=1, epsilon: float=1e-10, k:
+int=0) -> OutputType |
 ä½¿ç¨Grippoä¸ZhangHangeræåºçéåè°çº¿æç´¢æ¹æ³æ´æ°æ­¥é¿ | ####
 çé¡¿æ³ï¼newtonï¼ ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------------------
 ----------------------------------------------------------------------------- |
 --------------------------------- | | classic(funcs: FuncArray, args: ArgArray,
 x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10,
 k: int=0) -> OutputType |
@@ -119,64 +120,65 @@
 oc.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [ä¸ç­å¼çº¦æ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### ç­å¼çº¦æï¼equalï¼
 ```python oc.equal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------- | --------- | | penalty_quadratice
 (funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
-p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region",
-lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon:
-float=1e-6, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
-ä¸ç­å¼çº¦æï¼unequalï¼ ```python oc.unequal.[å½æ°å]([ç®æ å½æ°],
-[åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
-| | ---------------------------------------------------------------------------
+bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p:
+float=2, epsk: float=1e-4, epsilon: float=1e-4, k: int=0) -> OutputType |
+å¢å äºæ¬¡ç½é¡¹ | | lagrange_augmentede(funcs: FuncArray, args: ArgArray,
+cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
+method: str="newton", lamk: float=6, sigma: float=10, p: float=2, etak:
+float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType |
+å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | #### ä¸ç­å¼çº¦æï¼unequalï¼ ```python
+oc.unequal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨],
+[åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
--------------- | --------- | | penalty_quadraticu(funcs: FuncArray, args:
-ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon:
-float=1e-10, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | |
-penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray,
-x_0: PointArray, draw: bool=True, output_f: bool=False, method:
-str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k:
-int=0) -> OutputType | å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs:
+---------------------------------------------------------- | --------- | |
+penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
+PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma:
+float=10, p: float=0.4, epsk: float=1e-4, epsilon: float=1e-10, k: int=0) -
+> OutputType | å¢å äºæ¬¡ç½é¡¹ | | penalty_interior_fraction(funcs:
 FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
-output_f: bool=False, method: str="trust_region", muk: float=10, sigma:
-float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1,
-epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
-#### æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
+output_f: bool=False, method: str="newton", sigma: float=12, p: float=0.6,
+epsk: float=1e-6, epsilon: float=1e-6, k: int=0) -> OutputType |
+å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs: FuncArray, args:
+ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
+bool=False, method: str="newton", muk: float=10, sigma: float=8, alpha:
+float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4,
+k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
+æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨], [ä¸ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------- | --------- | | penalty_quadraticm(funcs: FuncArray, args: ArgArray,
 cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
-p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p:
+float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType |
 å¢å äºæ¬¡ç½é¡¹ | | penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal:
 FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon:
-float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
+bool=False, method: str="newton", sigma: float=1, p: float=0.6, epsk: float=1e-
+6, epsilon: float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
 lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray,
 cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma:
-float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
-epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
-### æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ```
-#### Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA],
-[ç©éµb], [å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
-| | ---------------------------------------------------------------------------
----------------------------- | ---------------- | | gradient(A: NDArray, b:
-NDArray, mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, delta: float=10, alp: float=1e-3, epsilon: float=1e-2, k: int=0) -
-> OutputType | åæ»åLassoå½æ°æ³ | | subgradient(A: NDArray, b: NDArray,
-mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, alphak: float=2e-2, epsilon: float=1e-3, k: int=0) -> OutputType |
+bool=False, method: str="newton", lamk: float=6, muk: float=10, sigma: float=8,
+alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon:
+float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ###
+æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ``` ####
+Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA], [ç©éµb],
+[å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------
+-------------------------------------------------------------------------------
+------------------ | ---------------- | | gradient(A: NDArray, b: NDArray, mu:
+float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
+delta: float=10, alp: float=1e-3, epsilon: float=1e-2, k: int=0) -> OutputType
+| åæ»åLassoå½æ°æ³ | | subgradient(A: NDArray, b: NDArray, mu: float,
+args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, alphak:
+float=2e-2, epsilon: float=1e-3, k: int=0) -> OutputType |
 æ¬¡æ¢¯åº¦æ³Lassoé¿åä¸é¶ä¸å¯å¯¼ | | penalty(A: NDArray, b: NDArray, mu:
 float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
 gamma: float=0.01, epsilon: float=1e-6, k: int=0) -> OutputType | ç½å½æ°æ³
 | | approximate_point(A: NDArray, b: NDArray, mu: float, args: ArgArray, x_0:
 PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-4, k:
 int=0) -> OutputType | é»è¿ç®å­æ´æ° | ####
 æ²çº¿ç¸åé®é¢ï¼WanYuanï¼ ```python oe.WanYuan.[å½æ°å](
```

### Comparing `optimtool-2.4.3/README.md` & `optimtool-2.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 ou.gradient_descent.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                 | 解释                                   |
 | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                                                             | 通过解方程的方式来求解精确步长                      |
 | steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                           | 使用线搜索方法求解非精确步长（默认使用wolfe线搜索）         |
-| barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
+| barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, M: int=20, eta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
 
 #### 牛顿法（newton）
 
 ```python
 ou.newton.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
@@ -158,40 +158,40 @@
 
 ```python
 oc.equal.[函数名]([目标函数], [参数表], [等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                   | 解释        |
 | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=2, epsk: float=1e-4, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 不等式约束（unequal）
 
 ```python
 oc.unequal.[函数名]([目标函数], [参数表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                      | 解释        |
 | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------- |
-| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
-| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
-| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.4, epsk: float=1e-4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
+| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=12, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
+| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 混合等式约束（mixequal）
 
 ```python
 oc.mixequal.[函数名]([目标函数], [参数表], [等式约束表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                                                  | 解释        |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
-| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
-| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
+| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=1, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
+| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 ### 方法的应用（example）
 
 ```python
 import optimtool.example as oe
 ```
```

#### html2text {}

```diff
@@ -43,15 +43,16 @@
 bool=False, epsilon: float=1e-10, k: int=0) -> OutputType |
 éè¿è§£æ¹ç¨çæ¹å¼æ¥æ±è§£ç²¾ç¡®æ­¥é¿ | | steepest(funcs: FuncArray,
 args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
 str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨çº¿æç´¢æ¹æ³æ±è§£éç²¾ç¡®æ­¥é¿ï¼é»è®¤ä½¿ç¨wolfeçº¿æç´¢ï¼ | |
 barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta:
-float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType |
+float=0.6, M: int=20, eta: float=0.6, alpha: float=1, epsilon: float=1e-10, k:
+int=0) -> OutputType |
 ä½¿ç¨Grippoä¸ZhangHangeræåºçéåè°çº¿æç´¢æ¹æ³æ´æ°æ­¥é¿ | ####
 çé¡¿æ³ï¼newtonï¼ ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------------------
 ----------------------------------------------------------------------------- |
 --------------------------------- | | classic(funcs: FuncArray, args: ArgArray,
 x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10,
 k: int=0) -> OutputType |
@@ -102,64 +103,65 @@
 oc.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [ä¸ç­å¼çº¦æ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### ç­å¼çº¦æï¼equalï¼
 ```python oc.equal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------- | --------- | | penalty_quadratice
 (funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
-p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region",
-lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon:
-float=1e-6, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
-ä¸ç­å¼çº¦æï¼unequalï¼ ```python oc.unequal.[å½æ°å]([ç®æ å½æ°],
-[åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
-| | ---------------------------------------------------------------------------
+bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p:
+float=2, epsk: float=1e-4, epsilon: float=1e-4, k: int=0) -> OutputType |
+å¢å äºæ¬¡ç½é¡¹ | | lagrange_augmentede(funcs: FuncArray, args: ArgArray,
+cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
+method: str="newton", lamk: float=6, sigma: float=10, p: float=2, etak:
+float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType |
+å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | #### ä¸ç­å¼çº¦æï¼unequalï¼ ```python
+oc.unequal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨],
+[åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
--------------- | --------- | | penalty_quadraticu(funcs: FuncArray, args:
-ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon:
-float=1e-10, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | |
-penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray,
-x_0: PointArray, draw: bool=True, output_f: bool=False, method:
-str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k:
-int=0) -> OutputType | å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs:
+---------------------------------------------------------- | --------- | |
+penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
+PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma:
+float=10, p: float=0.4, epsk: float=1e-4, epsilon: float=1e-10, k: int=0) -
+> OutputType | å¢å äºæ¬¡ç½é¡¹ | | penalty_interior_fraction(funcs:
 FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
-output_f: bool=False, method: str="trust_region", muk: float=10, sigma:
-float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1,
-epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
-#### æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
+output_f: bool=False, method: str="newton", sigma: float=12, p: float=0.6,
+epsk: float=1e-6, epsilon: float=1e-6, k: int=0) -> OutputType |
+å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs: FuncArray, args:
+ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
+bool=False, method: str="newton", muk: float=10, sigma: float=8, alpha:
+float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4,
+k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
+æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨], [ä¸ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------- | --------- | | penalty_quadraticm(funcs: FuncArray, args: ArgArray,
 cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
-p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p:
+float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType |
 å¢å äºæ¬¡ç½é¡¹ | | penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal:
 FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon:
-float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
+bool=False, method: str="newton", sigma: float=1, p: float=0.6, epsk: float=1e-
+6, epsilon: float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
 lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray,
 cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma:
-float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
-epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
-### æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ```
-#### Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA],
-[ç©éµb], [å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
-| | ---------------------------------------------------------------------------
----------------------------- | ---------------- | | gradient(A: NDArray, b:
-NDArray, mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, delta: float=10, alp: float=1e-3, epsilon: float=1e-2, k: int=0) -
-> OutputType | åæ»åLassoå½æ°æ³ | | subgradient(A: NDArray, b: NDArray,
-mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, alphak: float=2e-2, epsilon: float=1e-3, k: int=0) -> OutputType |
+bool=False, method: str="newton", lamk: float=6, muk: float=10, sigma: float=8,
+alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon:
+float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ###
+æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ``` ####
+Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA], [ç©éµb],
+[å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------
+-------------------------------------------------------------------------------
+------------------ | ---------------- | | gradient(A: NDArray, b: NDArray, mu:
+float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
+delta: float=10, alp: float=1e-3, epsilon: float=1e-2, k: int=0) -> OutputType
+| åæ»åLassoå½æ°æ³ | | subgradient(A: NDArray, b: NDArray, mu: float,
+args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, alphak:
+float=2e-2, epsilon: float=1e-3, k: int=0) -> OutputType |
 æ¬¡æ¢¯åº¦æ³Lassoé¿åä¸é¶ä¸å¯å¯¼ | | penalty(A: NDArray, b: NDArray, mu:
 float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
 gamma: float=0.01, epsilon: float=1e-6, k: int=0) -> OutputType | ç½å½æ°æ³
 | | approximate_point(A: NDArray, b: NDArray, mu: float, args: ArgArray, x_0:
 PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-4, k:
 int=0) -> OutputType | é»è¿ç®å­æ´æ° | ####
 æ²çº¿ç¸åé®é¢ï¼WanYuanï¼ ```python oe.WanYuan.[å½æ°å](
```

### Comparing `optimtool-2.4.3/optimtool/__init__.py` & `optimtool-2.4.4/optimtool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 from . import unconstrain
 from . import example
 from . import hybrid # appear in v2.5.0
 
 from ._version import __version__
 
 if sys.version_info < (3, 7, 0):
-    raise OSError(f'optimtool-2.4.3 requires Python >=3.7, but yours is {sys.version}')
+    raise OSError(f'optimtool-2.4.4 requires Python >=3.7, but yours is {sys.version}')
```

### Comparing `optimtool-2.4.3/optimtool/_convert.py` & `optimtool-2.4.4/optimtool/_convert.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/_drive.py` & `optimtool-2.4.4/optimtool/_drive.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/_search.py` & `optimtool-2.4.4/optimtool/_search.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/_typing.py` & `optimtool-2.4.4/optimtool/_typing.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/_utils.py` & `optimtool-2.4.4/optimtool/_utils.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/_version.py` & `optimtool-2.4.4/optimtool/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '2.4.3'
+__version__ = '2.4.4'
```

### Comparing `optimtool-2.4.3/optimtool/constrain/__init__.py` & `optimtool-2.4.4/optimtool/constrain/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/constrain/equal.py` & `optimtool-2.4.4/optimtool/constrain/equal.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy as np
 import sympy as sp
 from .._utils import get_value, plot_iteration
 from .._convert import f2m, a2m, p2t
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-def penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10.0, p: float=2.0, epsilon: float=1e-4, k: int=0) -> OutputType:
+def penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10.0, p: float=2.0, epsk: float=1e-4, epsilon: float=1e-4, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -51,14 +51,17 @@
         无约束优化方法内核
         
     sigma : float
         罚函数因子
         
     p : float
         修正参数
+    
+    epsk: float
+        无约束内核的精度
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
@@ -67,34 +70,34 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 1
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    from .._kernel import kernel
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search, point, f = eval(kernel(method)), [], []
+    search, point, f = kernel(method), [], []
     sig = sp.symbols("sig")
     pen = funcs + (sig / 2) * cons.T * cons
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         pe = pen.subs(sig, sigma)
-        x_0, _ = search(pe, args, tuple(x_0), draw=False)
+        x_0, _ = search(pe, args, tuple(x_0), draw=False, epsilon=epsk)
         k = k + 1
         if np.linalg.norm(x_0 - point[k - 1]) < epsilon:
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_quadratic_equal")     
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-def lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType:
+def lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -138,18 +141,18 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 1
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
-    search, f = eval(kernel(method)), []
+    from .._kernel import kernel
+    search, f = kernel(method), []
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    lamk = np.array([lamk for i in range(cons.shape[0])]).reshape(cons.shape[0], 1)
+    lamk = np.array([lamk for _ in range(cons.shape[0])]).reshape(cons.shape[0], 1)
     while 1:
         L = sp.Matrix([funcs + (sigma / 2) * cons.T * cons + cons.T * lamk])
         f.append(get_value(funcs, args, x_0))
         x_0, _ = search(L, args, tuple(x_0), draw=False, epsilon=etak)
         k = k + 1
         reps = dict(zip(args, x_0))
         consv = np.array(cons.subs(reps)).astype(DataType)
```

### Comparing `optimtool-2.4.3/optimtool/constrain/mixequal.py` & `optimtool-2.4.4/optimtool/constrain/mixequal.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import numpy as np
 import sympy as sp
 from .._utils import get_value, plot_iteration
 from .._convert import f2m, a2m, p2t
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-def penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType:
+def penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -54,14 +54,17 @@
         无约束优化方法内核
         
     sigma : float
         罚函数因子
         
     p : float
         修正参数
+
+    epsk: float
+        无约束内核的精度
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
@@ -70,36 +73,36 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    from .._kernel import kernel
     funcs, args, cons_equal, cons_unequal, x_0 = f2m(funcs), a2m(args), f2m(cons_equal), f2m(cons_unequal), p2t(x_0)
-    search, point, f = eval(kernel(method)), [], []
+    search, point, f = kernel(method), [], []
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         reps = dict(zip(args, x_0))
         consv = np.array(cons_unequal.subs(reps)).astype(DataType)
         consv = np.where(consv <= 0, consv, 1)
         consv = np.where(consv > 0, consv, 0)
         pe = sp.Matrix([funcs + (sigma / 2) * cons_unequal.T * consv + (sigma / 2) * cons_equal.T * cons_equal])
-        x_0, _ = search(pe, args, tuple(x_0), draw=False)
+        x_0, _ = search(pe, args, tuple(x_0), draw=False, epsilon=epsk)
         k = k + 1
         if np.linalg.norm(x_0 - point[k - 1]) < epsilon:
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_quadratic_mixequal")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-def penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType:
+def penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=1, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -124,14 +127,17 @@
         无约束优化方法内核
         
     sigma : float
         罚函数因子
         
     p : float
         修正参数
+
+    epsk: float
+        无约束内核的精度
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
@@ -140,39 +146,39 @@
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    from .._kernel import kernel
     funcs, args, cons_equal, cons_unequal, x_0 = f2m(funcs), a2m(args), f2m(cons_equal), f2m(cons_unequal), p2t(x_0)
-    search, point, f = eval(kernel(method)), [], []
+    search, point, f = kernel(method), [], []
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         reps = dict(zip(args, x_0))
         consv_unequal = np.array(cons_unequal.subs(reps)).astype(DataType)
         consv_unequal = np.where(consv_unequal <= 0, consv_unequal, 1)
         consv_unequal = np.where(consv_unequal > 0, consv_unequal, 0)
         consv_equal = np.array(cons_equal.subs(reps)).astype(DataType)
         consv_equal = np.where(consv_equal <= 0, consv_equal, 1)
         consv_equal = np.where(consv_equal > 0, consv_equal, -1)
         pe = sp.Matrix([funcs + sigma * cons_unequal.T * consv_unequal + sigma * cons_equal.T * consv_equal])
-        x_0, _ = search(pe, args, tuple(x_0), draw=False)
+        x_0, _ = search(pe, args, tuple(x_0), draw=False, epsilon=epsk)
         k = k + 1
         if np.linalg.norm(x_0 - point[k - 1]) < epsilon:
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_L1")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-def lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType:
+def lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -231,20 +237,20 @@
         
     '''
     assert sigma > 0
     assert p > 1
     assert alpha > 0 
     assert alpha <= beta
     assert beta < 1
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    from .._kernel import kernel
     from .._drive import cons_unequal_L, v_k, renew_mu_k
     funcs, args, cons_equal, cons_unequal, x_0 = f2m(funcs), a2m(args), f2m(cons_equal), f2m(cons_unequal), p2t(x_0)
-    search, f = eval(kernel(method)), []
-    lamk = np.array([lamk for i in range(cons_equal.shape[0])]).reshape(cons_equal.shape[0], 1)
-    muk = np.array([muk for i in range(cons_unequal.shape[0])]).reshape(cons_unequal.shape[0], 1)
+    search, f = kernel(method), []
+    lamk = np.array([lamk for _ in range(cons_equal.shape[0])]).reshape(cons_equal.shape[0], 1)
+    muk = np.array([muk for _ in range(cons_unequal.shape[0])]).reshape(cons_unequal.shape[0], 1)
     while 1:
         etak = 1 / sigma
         epsilonk = 1 / sigma**alpha
         cons_uneuqal_modifyed = cons_unequal_L(cons_unequal, args, muk, sigma, x_0)
         L = sp.Matrix([funcs + (sigma / 2) * (cons_equal.T * cons_equal + cons_uneuqal_modifyed) + cons_equal.T * lamk])
         f.append(get_value(funcs, args, x_0))
         x_0, _ = search(L, args, tuple(x_0), draw=False, epsilon=epsilonk)
```

### Comparing `optimtool-2.4.3/optimtool/constrain/unequal.py` & `optimtool-2.4.4/optimtool/constrain/unequal.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import sympy as sp
 import numpy as np
 from .._utils import get_value, plot_iteration
 from .._convert import f2m, a2m, p2t
 
 from .._typing import FuncArray, ArgArray, PointArray, OutputType, DataType
 
-def penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType:
+def penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.4, epsk: float=1e-4, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -51,14 +51,17 @@
         无约束优化方法内核
         
     sigma : float
         罚函数因子
         
     p : float
         修正参数
+
+    epsk: float
+        无约束内核的精度
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
@@ -68,39 +71,40 @@
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
     assert p < 1
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    from .._kernel import kernel
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search, point, f = eval(kernel(method)), [], []
+    search, point, f = kernel(method), [], []
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         reps = dict(zip(args, x_0))
         consv = np.array(cons.subs(reps)).astype(DataType)
         consv = np.where(consv <= 0, consv, 1)
         consv = np.where(consv > 0, consv, 0)
         pe = sp.Matrix([funcs + (sigma / 2) * cons.T * consv])
-        x_0, _ = search(pe, args, tuple(x_0), draw=False)
+        x_0, _ = search(pe, args, tuple(x_0), draw=False, epsilon=epsk)
         k = k + 1
         if np.linalg.norm(x_0 - point[k - 1]) < epsilon:
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
         sigma = p * sigma
     plot_iteration(f, draw, "penalty_quadratic_unequal") 
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 '''
 保证点在定义域内
 '''
-def penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType:
+# 后续版本会弃用这个方法
+def penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=12, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-6, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -122,14 +126,17 @@
         无约束优化方法内核
         
     sigma : float
         罚函数因子
         
     p : float
         修正参数
+
+    epsk: float
+        无约束内核的精度
         
     epsilon : float
         迭代停机准则
         
     k : int
         迭代次数
         
@@ -139,36 +146,36 @@
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     assert sigma > 0
     assert p > 0
     assert p < 1
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    from .._kernel import kernel
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search, point, f = eval(kernel(method)), [], []
+    search, point, f = kernel(method), [], []
     sub_pe = 0
     for i in cons:
         sub_pe += 1 / i
     sub_pe = sp.Matrix([sub_pe])
     while 1:
         point.append(np.array(x_0))
         f.append(get_value(funcs, args, x_0))
         pe = sp.Matrix([funcs - sigma * sub_pe])
-        x_0, _ = search(pe, args, tuple(x_0), draw=False)
+        x_0, _ = search(pe, args, tuple(x_0), draw=False, epsilon=epsk)
         k = k + 1
         sigma = p * sigma
         if np.linalg.norm(x_0 - point[k - 1]) < epsilon:
             point.append(np.array(x_0))
             f.append(get_value(funcs, args, x_0))
             break
     plot_iteration(f, draw, "penalty_interior_fraction")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
-def lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType:
+def lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -221,18 +228,18 @@
         
     '''
     assert sigma > 0
     assert p > 1
     assert alpha > 0 
     assert alpha <= beta
     assert beta < 1
-    from .._kernel import kernel, barzilar_borwein, modified, L_BFGS, steihaug_CG
+    from .._kernel import kernel
     from .._drive import cons_unequal_L, renew_mu_k, v_k
     funcs, args, x_0, cons = f2m(funcs), a2m(args), p2t(x_0), f2m(cons)
-    search, f = eval(kernel(method)), []
+    search, f = kernel(method), []
     muk = np.array([muk for _ in range(cons.shape[0])]).reshape(cons.shape[0], 1)
     while 1:
         etak = 1 / sigma
         epsilonk = 1 / sigma**alpha
         cons_uneuqal_modifyed = cons_unequal_L(cons, args, muk, sigma, x_0)
         L = sp.Matrix([funcs + (sigma / 2) * cons_uneuqal_modifyed])
         f.append(get_value(funcs, args, x_0))
```

### Comparing `optimtool-2.4.3/optimtool/example/Lasso.py` & `optimtool-2.4.4/optimtool/example/Lasso.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/example/WanYuan.py` & `optimtool-2.4.4/optimtool/example/WanYuan.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/example/__init__.py` & `optimtool-2.4.4/optimtool/example/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/hybrid/__init__.py` & `optimtool-2.4.4/optimtool/hybrid/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/hybrid/approximate_point_gradient.py` & `optimtool-2.4.4/optimtool/hybrid/approximate_point_gradient.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/unconstrain/__init__.py` & `optimtool-2.4.4/optimtool/unconstrain/__init__.py`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/optimtool/unconstrain/gradient_descent.py` & `optimtool-2.4.4/optimtool/unconstrain/gradient_descent.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,28 +54,28 @@
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    res = funcs.jacobian(args)
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    res = funcs.jacobian(args) # gradient
     m = sp.symbols("m")
-    arg = sp.Matrix([m])
-    f = []
+    arg, f = sp.Matrix([m]), []
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
         dk = -np.array(res.subs(reps)).astype(DataType)
         if np.linalg.norm(dk) >= epsilon:
             xt = x_0 + m * dk[0]
             h = funcs.subs(dict(zip(args, xt))).jacobian(arg)
             mt = sp.solve(h)
-            x_0 = (x_0 + mt[m] * dk[0]).astype(DataType)
-            k = k + 1
+            x_0 += (mt[m] * dk[0]).astype(DataType)
+            k += 1
         else:
             break
     plot_iteration(f, draw, "gradient_descent_solve")
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 def steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
@@ -108,33 +108,34 @@
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    from .._search import armijo, goldstein, wolfe
-    search, f = eval(method), []
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    res = funcs.jacobian(args)
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    from .._kernel import linear_search
+    search, f = linear_search(method), []
+    res = funcs.jacobian(args) # gradient
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
         dk = -np.array(res.subs(reps)).astype(DataType)
         if np.linalg.norm(dk) >= epsilon:
             alpha = search(funcs, args, x_0, dk)
-            x_0 = x_0 + alpha * dk[0]
-            k = k + 1
+            x_0 += alpha * dk[0]
+            k += 1
         else:
             break
     plot_iteration(f, draw, "gradient_descent_steepest")
     return (x_0, k, f) if output_f is True else (x_0, k)
     
 # Barzilar Borwein梯度下降法
-def barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType:
+def barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, M: int=20, eta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
     Parameters
     ----------
     funcs : FuncArray
         当前目标方程
         
     args : ArgArray
@@ -148,22 +149,25 @@
         
     output_f : bool
         输出迭代函数值列表
         
     method : str
         非单调线搜索方法："Grippo"与"ZhangHanger"
         
-    M : int
-        阈值
-        
     c1 : float
         常数
         
     beta : float
         常数
+
+    M : int
+        阈值
+
+    eta: float
+        阈值
         
     alpha : float
         初始步长
         
     epsilon : float
         迭代停机准则
         
@@ -178,32 +182,36 @@
         
     '''
     assert alpha > 0
     assert c1 > 0
     assert c1 < 1
     assert beta > 0
     assert beta < 1
-    from .._search import Grippo, ZhangHanger
-    search, point, f = eval(method), [], []
+    assert M > 0
+    assert eta > 0
+    assert eta < 1
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    res = funcs.jacobian(args)
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    from .._kernel import nonmonotonic_search
+    search, constant = nonmonotonic_search(method, M, eta)
+    res, point, f = funcs.jacobian(args), [], []
     while 1:
         point.append(x_0)
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
-        dk = - np.array(res.subs(reps)).astype(DataType)
+        dk = -np.array(res.subs(reps)).astype(DataType)
         if np.linalg.norm(dk) >= epsilon:
-            alpha = search(funcs, args, x_0, dk, k, point, c1, beta, alpha)
+            alpha = search(funcs, args, x_0, dk, k, point, c1, beta, alpha, constant)
             delta = alpha * dk[0]
             x_0 = x_0 + delta
             yk = np.array(res.subs(dict(zip(args, x_0)))).astype(DataType) + dk
             alpha_up = delta.dot(delta.T)
             alpha_down = delta.dot(yk.T)
             if alpha_down != 0:
                 alpha = alpha_up / alpha_down
-            k = k + 1
+            k += 1
         else:
             break
     plot_iteration(f, draw, "gradient_descent_barzilar_borwein_" + method)
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 __all__ = [solve, steepest, barzilar_borwein]
```

### Comparing `optimtool-2.4.3/optimtool/unconstrain/newton.py` & `optimtool-2.4.4/optimtool/unconstrain/newton.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,26 +53,26 @@
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    res = funcs.jacobian(args)
-    hes = res.jacobian(args)
-    f = []
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    res = funcs.jacobian(args) # gradient
+    hes, f = res.jacobian(args), []
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
-        hessian = np.array(hes.subs(reps)).astype(DataType)
         gradient = np.array(res.subs(reps)).astype(DataType)
-        dk = - np.linalg.inv(hessian).dot(gradient.T).reshape(1, -1)
+        hessian = np.array(hes.subs(reps)).astype(DataType)
+        dk = -np.linalg.inv(hessian).dot(gradient.T).reshape(1, -1)
         if np.linalg.norm(dk) >= epsilon:
-            x_0 = x_0 + dk[0]
-            k = k + 1
+            x_0 += dk[0]
+            k += 1
         else:
             break
     plot_iteration(f, draw, "newton_classic")        
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 def modified(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", m: int=20, epsilon: float=1e-10, k: int=0) -> OutputType:
     '''
@@ -105,30 +105,31 @@
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    from .._search import armijo, goldstein, wolfe
+    from .._kernel import linear_search
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search, f = eval(method), []
-    res = funcs.jacobian(args)
-    hes = res.jacobian(args)
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    search, f = linear_search(method), []
+    res = funcs.jacobian(args) # graident
+    hes = res.jacobian(args) # hessian
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
         gradient = np.array(res.subs(reps)).astype(DataType)
-        hessian = np.array(hes.subs(reps)).astype(DataType)
+        hessian = np.array(hes.subs(reps)).astype(DataType) # hessian: from `object` to `float`
         hessian = h2h(hessian)
         dk = -np.linalg.inv(hessian).dot(gradient.T).reshape(1, -1)
         if np.linalg.norm(dk) >= epsilon:
             alpha = search(funcs, args, x_0, dk)
-            x_0 = x_0 + alpha * dk[0]
-            k = k + 1
+            x_0 += alpha * dk[0]
+            k += 1
         else:
             break
     plot_iteration(f, draw, "newton_modified_" + method)
     return (x_0, k, f) if output_f is True else (x_0, k)
 
 def CG(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-6, k: int=0) -> OutputType:
     '''
@@ -159,23 +160,23 @@
         迭代次数
         
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
-        
+        f
     '''
-    from .._search import armijo, goldstein, wolfe
     from .._drive import CG_gradient
+    from .._kernel import linear_search
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search, f = eval(method), []
-    res = funcs.jacobian(args)
-    hes = res.jacobian(args)
-    dk0 = np.zeros((args.shape[0], 1))
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    search, f = linear_search(method), []
+    res = funcs.jacobian(args) # gradient
+    hes, dk0 = res.jacobian(args), np.zeros((args.shape[0], 1)) # hessian and initial dk
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
         gradient = np.array(res.subs(reps)).astype(DataType)
         hess = np.array(hes.subs(reps)).astype(DataType)
         dk, _ = CG_gradient(hess, -gradient, dk0)
         if np.linalg.norm(dk) >= epsilon:
```

### Comparing `optimtool-2.4.3/optimtool/unconstrain/newton_quasi.py` & `optimtool-2.4.4/optimtool/unconstrain/newton_quasi.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,17 +56,18 @@
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    from .._search import armijo, goldstein, wolfe
+    from .._kernel import linear_search
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search, f = eval(method), []
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    search, f = linear_search(method), []
     res = funcs.jacobian(args)
     hes = res.jacobian(args)
     hess = np.array(hes.subs(dict(zip(args, x_0)))).astype(DataType)
     hess = h2h(hess)
     while 1:
         reps = dict(zip(args, x_0))
         f.append(get_value(funcs, args, x_0))
@@ -119,17 +120,18 @@
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    from .._search import armijo, goldstein, wolfe
+    from .._kernel import linear_search
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search, f = eval(method), []
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    search, f = linear_search(method), []
     res = funcs.jacobian(args)
     hes = res.jacobian(args)
     hess = np.array(hes.subs(dict(zip(args, x_0)))).astype(DataType)
     hess = h2h(hess)
     hessi = np.linalg.inv(hess)
     while 1:
         reps = dict(zip(args, x_0))
@@ -186,18 +188,19 @@
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    from .._search import armijo, goldstein, wolfe
     from .._drive import L_BFGS_double_loop
+    from .._kernel import linear_search
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
-    search = eval(method)
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
+    search = linear_search(method)
     res = funcs.jacobian(args)
     hes = res.jacobian(args)
     l = hes.shape[0]
     f, s, y, p = [], [], [], []
     gamma = []
     gamma.append(1)
     while 1:
```

### Comparing `optimtool-2.4.3/optimtool/unconstrain/nonlinear_least_square.py` & `optimtool-2.4.4/optimtool/unconstrain/nonlinear_least_square.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,20 +56,19 @@
 
     Returns
     -------
     OutputType
         最终收敛点, 迭代次数, (迭代函数值列表)
         
     '''
-    from .._search import armijo, goldstein, wolfe
+    from .._kernel import linear_search
     funcr, args, x_0 = f2m(funcr), a2m(args), p2t(x_0)
     assert funcr.shape[0] > 1 and funcr.shape[1] ==1 and args.shape[0] == len(x_0)
-    search, f = eval(method), []
-    res = funcr.jacobian(args)
-    funcs = sp.Matrix([(1/2)*funcr.T*funcr])
+    search, f = linear_search(method), []
+    res, funcs = funcr.jacobian(args), sp.Matrix([(1/2)*funcr.T*funcr])
     while 1:
         reps = dict(zip(args, x_0))
         rk = np.array(funcr.subs(reps)).astype(DataType)
         f.append(get_value(funcs, args, x_0))
         jk = np.array(res.subs(reps)).astype(DataType)
         q, r = np.linalg.qr(jk)
         dk = np.linalg.inv(r).dot(-(q.T).dot(rk)).reshape(1,-1)
@@ -137,20 +136,17 @@
     assert p1 < p2
     assert p2 < 1
     assert gamma1 < 1
     assert gamma2 > 1
     from .._drive import CG_gradient
     funcr, args, x_0 = f2m(funcr), a2m(args), p2t(x_0)
     assert funcr.shape[0] > 1 and funcr.shape[1] ==1 and args.shape[0] == len(x_0)
-    res = funcr.jacobian(args)
-    funcs = sp.Matrix([(1/2)*funcr.T*funcr])
+    res, funcs = funcr.jacobian(args), sp.Matrix([(1/2)*funcr.T*funcr])
     resf = funcs.jacobian(args)
-    hess = resf.jacobian(args)
-    dk0 = np.zeros((args.shape[0], 1))
-    f = []
+    hess, dk0, f = resf.jacobian(args), np.zeros((args.shape[0], 1)), []
     while 1:
         reps = dict(zip(args, x_0))
         rk = np.array(funcr.subs(reps)).astype(DataType)
         f.append(get_value(funcs, args, x_0))
         jk = np.array(res.subs(reps)).astype(DataType)
         dk, _ = CG_gradient((jk.T).dot(jk) + lamk, -((jk.T).dot(rk)).reshape(1, -1), dk0)
         pk_up = np.array(funcs.subs(reps)).astype(DataType) - np.array(funcs.subs(dict(zip(args, x_0 + dk[0])))).astype(DataType)
```

### Comparing `optimtool-2.4.3/optimtool/unconstrain/trust_region.py` & `optimtool-2.4.4/optimtool/unconstrain/trust_region.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     assert eta < p1
     assert p1 < p2
     assert p2 < 1
     assert gamma1 < 1
     assert gamma2 > 1
     from .._drive import steihaug
     funcs, args, x_0 = f2m(funcs), a2m(args), p2t(x_0)
+    assert all(funcs.shape) == 1 and args.shape[0] == len(x_0)
     res = funcs.jacobian(args)
     hes = res.jacobian(args)
     s0, f = [0 for _ in range(args.shape[0])], []
     while 1:
         reps = dict(zip(args, x_0))
         funv = np.array(funcs.subs(reps)).astype(DataType)
         f.append(funv[0][0])
```

### Comparing `optimtool-2.4.3/optimtool.egg-info/PKG-INFO` & `optimtool-2.4.4/optimtool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimtool
-Version: 2.4.3
+Version: 2.4.4
 Summary: The fundamental package for scientific research in optimization.
 Home-page: https://github.com/linjing-lab/optimtool
 Download-URL: https://github.com/linjing-lab/optimtool/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MIT
 Project-URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
@@ -125,15 +125,15 @@
 ou.gradient_descent.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                 | 解释                                   |
 | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
 | solve(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10, k: int=0) -> OutputType                                                             | 通过解方程的方式来求解精确步长                      |
 | steepest(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType                                           | 使用线搜索方法求解非精确步长（默认使用wolfe线搜索）         |
-| barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
+| barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta: float=0.6, M: int=20, eta: float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType | 使用Grippo与ZhangHanger提出的非单调线搜索方法更新步长 |
 
 #### 牛顿法（newton）
 
 ```python
 ou.newton.[函数名]([目标函数], [参数表], [初始迭代点])
 ```
 
@@ -187,40 +187,40 @@
 
 ```python
 oc.equal.[函数名]([目标函数], [参数表], [等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                   | 解释        |
 | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadratice(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=2, epsk: float=1e-4, epsilon: float=1e-4, k: int=0) -> OutputType                     | 增加二次罚项    |
+| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 不等式约束（unequal）
 
 ```python
 oc.unequal.[函数名]([目标函数], [参数表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                      | 解释        |
 | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------- |
-| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
-| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
-| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.4, epsk: float=1e-4, epsilon: float=1e-10, k: int=0) -> OutputType                                     | 增加二次罚项    |
+| penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=12, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-6, k: int=0) -> OutputType                              | 增加分式函数罚项  |
+| lagrange_augmentedu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", muk: float=10, sigma: float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 #### 混合等式约束（mixequal）
 
 ```python
 oc.mixequal.[函数名]([目标函数], [参数表], [等式约束表], [不等式约束表], [初始迭代点])
 ```
 
 | 方法头                                                                                                                                                                                                  | 解释        |
 | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
-| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
-| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
-| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
+| penalty_quadraticm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType                                             | 增加二次罚项    |
+| penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma: float=1, p: float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType                                                     | L1精确罚函数法  |
+| lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method: str="newton", lamk: float=6, muk: float=10, sigma: float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon: float=1e-4, k: int=0) -> OutputType | 增广拉格朗日乘子法 |
 
 ### 方法的应用（example）
 
 ```python
 import optimtool.example as oe
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optimtool Version: 2.4.3 Summary: The fundamental
+Metadata-Version: 2.1 Name: optimtool Version: 2.4.4 Summary: The fundamental
 package for scientific research in optimization. Home-page: https://github.com/
 linjing-lab/optimtool Download-URL: https://github.com/linjing-lab/optimtool/
 tags Author: ææ¯ Author-email: linjing010729@163.com License: MIT Project-
 URL: Source, https://github.com/linjing-lab/optimtool/tree/master/optimtool/
 Project-URL: Tracker, https://github.com/linjing-lab/optimtool/issues
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
@@ -60,15 +60,16 @@
 bool=False, epsilon: float=1e-10, k: int=0) -> OutputType |
 éè¿è§£æ¹ç¨çæ¹å¼æ¥æ±è§£ç²¾ç¡®æ­¥é¿ | | steepest(funcs: FuncArray,
 args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, method:
 str="wolfe", epsilon: float=1e-10, k: int=0) -> OutputType |
 ä½¿ç¨çº¿æç´¢æ¹æ³æ±è§£éç²¾ç¡®æ­¥é¿ï¼é»è®¤ä½¿ç¨wolfeçº¿æç´¢ï¼ | |
 barzilar_borwein(funcs: FuncArray, args: ArgArray, x_0: PointArray, draw:
 bool=True, output_f: bool=False, method: str="Grippo", c1: float=0.6, beta:
-float=0.6, alpha: float=1, epsilon: float=1e-10, k: int=0) -> OutputType |
+float=0.6, M: int=20, eta: float=0.6, alpha: float=1, epsilon: float=1e-10, k:
+int=0) -> OutputType |
 ä½¿ç¨Grippoä¸ZhangHangeræåºçéåè°çº¿æç´¢æ¹æ³æ´æ°æ­¥é¿ | ####
 çé¡¿æ³ï¼newtonï¼ ```python ou.newton.[å½æ°å]([ç®æ å½æ°],
 [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------------------
 ----------------------------------------------------------------------------- |
 --------------------------------- | | classic(funcs: FuncArray, args: ArgArray,
 x_0: PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-10,
 k: int=0) -> OutputType |
@@ -119,64 +120,65 @@
 oc.[æ¹æ³å].[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [ä¸ç­å¼çº¦æ°è¡¨], [åå§è¿­ä»£ç¹]) ``` #### ç­å¼çº¦æï¼equalï¼
 ```python oc.equal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 --------------------------------------- | --------- | | penalty_quadratice
 (funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
-p: float=2, epsilon: float=1e-4, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ |
-| lagrange_augmentede(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
-PointArray, draw: bool=True, output_f: bool=False, method: str="trust_region",
-lamk: float=6, sigma: float=10, p: float=2, etak: float=1e-4, epsilon:
-float=1e-6, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
-ä¸ç­å¼çº¦æï¼unequalï¼ ```python oc.unequal.[å½æ°å]([ç®æ å½æ°],
-[åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
-| | ---------------------------------------------------------------------------
+bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p:
+float=2, epsk: float=1e-4, epsilon: float=1e-4, k: int=0) -> OutputType |
+å¢å äºæ¬¡ç½é¡¹ | | lagrange_augmentede(funcs: FuncArray, args: ArgArray,
+cons: FuncArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
+method: str="newton", lamk: float=6, sigma: float=10, p: float=2, etak:
+float=1e-4, epsilon: float=1e-6, k: int=0) -> OutputType |
+å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | #### ä¸ç­å¼çº¦æï¼unequalï¼ ```python
+oc.unequal.[å½æ°å]([ç®æ å½æ°], [åæ°è¡¨], [ä¸ç­å¼çº¦æè¡¨],
+[åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
--------------- | --------- | | penalty_quadraticu(funcs: FuncArray, args:
-ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", sigma: float=10, p: float=0.4, epsilon:
-float=1e-10, k: int=0) -> OutputType | å¢å äºæ¬¡ç½é¡¹ | |
-penalty_interior_fraction(funcs: FuncArray, args: ArgArray, cons: FuncArray,
-x_0: PointArray, draw: bool=True, output_f: bool=False, method:
-str="trust_region", sigma: float=12, p: float=0.6, epsilon: float=1e-6, k:
-int=0) -> OutputType | å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs:
+---------------------------------------------------------- | --------- | |
+penalty_quadraticu(funcs: FuncArray, args: ArgArray, cons: FuncArray, x_0:
+PointArray, draw: bool=True, output_f: bool=False, method: str="newton", sigma:
+float=10, p: float=0.4, epsk: float=1e-4, epsilon: float=1e-10, k: int=0) -
+> OutputType | å¢å äºæ¬¡ç½é¡¹ | | penalty_interior_fraction(funcs:
 FuncArray, args: ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True,
-output_f: bool=False, method: str="trust_region", muk: float=10, sigma:
-float=8, alpha: float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1,
-epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
-#### æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
+output_f: bool=False, method: str="newton", sigma: float=12, p: float=0.6,
+epsk: float=1e-6, epsilon: float=1e-6, k: int=0) -> OutputType |
+å¢å åå¼å½æ°ç½é¡¹ | | lagrange_augmentedu(funcs: FuncArray, args:
+ArgArray, cons: FuncArray, x_0: PointArray, draw: bool=True, output_f:
+bool=False, method: str="newton", muk: float=10, sigma: float=8, alpha:
+float=0.2, beta: float=0.7, p: float=2, eta: float=1e-1, epsilon: float=1e-4,
+k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ####
+æ··åç­å¼çº¦æï¼mixequalï¼ ```python oc.mixequal.[å½æ°å](
 [ç®æ å½æ°], [åæ°è¡¨], [ç­å¼çº¦æè¡¨], [ä¸ç­å¼çº¦æè¡¨],
 [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | -------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 ------- | --------- | | penalty_quadraticm(funcs: FuncArray, args: ArgArray,
 cons_equal: FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw:
-bool=True, output_f: bool=False, method: str="trust_region", sigma: float=10,
-p: float=0.6, epsilon: float=1e-10, k: int=0) -> OutputType |
+bool=True, output_f: bool=False, method: str="newton", sigma: float=10, p:
+float=0.6, epsk: float=1e-6, epsilon: float=1e-10, k: int=0) -> OutputType |
 å¢å äºæ¬¡ç½é¡¹ | | penalty_L1(funcs: FuncArray, args: ArgArray, cons_equal:
 FuncArray, cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", sigma: float=1, p: float=0.6, epsilon:
-float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
+bool=False, method: str="newton", sigma: float=1, p: float=0.6, epsk: float=1e-
+6, epsilon: float=1e-10, k: int=0) -> OutputType | L1ç²¾ç¡®ç½å½æ°æ³ | |
 lagrange_augmentedm(funcs: FuncArray, args: ArgArray, cons_equal: FuncArray,
 cons_unequal: FuncArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, method: str="trust_region", lamk: float=6, muk: float=10, sigma:
-float=8, alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3,
-epsilon: float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ |
-### æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ```
-#### Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA],
-[ç©éµb], [å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é
-| | ---------------------------------------------------------------------------
----------------------------- | ---------------- | | gradient(A: NDArray, b:
-NDArray, mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, delta: float=10, alp: float=1e-3, epsilon: float=1e-2, k: int=0) -
-> OutputType | åæ»åLassoå½æ°æ³ | | subgradient(A: NDArray, b: NDArray,
-mu: float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f:
-bool=False, alphak: float=2e-2, epsilon: float=1e-3, k: int=0) -> OutputType |
+bool=False, method: str="newton", lamk: float=6, muk: float=10, sigma: float=8,
+alpha: float=0.5, beta: float=0.7, p: float=2, eta: float=1e-3, epsilon:
+float=1e-4, k: int=0) -> OutputType | å¢å¹¿ææ ¼ææ¥ä¹å­æ³ | ###
+æ¹æ³çåºç¨ï¼exampleï¼ ```python import optimtool.example as oe ``` ####
+Lassoé®é¢ï¼Lassoï¼ ```python oe.Lasso.[å½æ°å]([ç©éµA], [ç©éµb],
+[å å­mu], [åæ°è¡¨], [åå§è¿­ä»£ç¹]) ``` | æ¹æ³å¤´ | è§£é | | ------
+-------------------------------------------------------------------------------
+------------------ | ---------------- | | gradient(A: NDArray, b: NDArray, mu:
+float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
+delta: float=10, alp: float=1e-3, epsilon: float=1e-2, k: int=0) -> OutputType
+| åæ»åLassoå½æ°æ³ | | subgradient(A: NDArray, b: NDArray, mu: float,
+args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False, alphak:
+float=2e-2, epsilon: float=1e-3, k: int=0) -> OutputType |
 æ¬¡æ¢¯åº¦æ³Lassoé¿åä¸é¶ä¸å¯å¯¼ | | penalty(A: NDArray, b: NDArray, mu:
 float, args: ArgArray, x_0: PointArray, draw: bool=True, output_f: bool=False,
 gamma: float=0.01, epsilon: float=1e-6, k: int=0) -> OutputType | ç½å½æ°æ³
 | | approximate_point(A: NDArray, b: NDArray, mu: float, args: ArgArray, x_0:
 PointArray, draw: bool=True, output_f: bool=False, epsilon: float=1e-4, k:
 int=0) -> OutputType | é»è¿ç®å­æ´æ° | ####
 æ²çº¿ç¸åé®é¢ï¼WanYuanï¼ ```python oe.WanYuan.[å½æ°å](
```

### Comparing `optimtool-2.4.3/optimtool.egg-info/SOURCES.txt` & `optimtool-2.4.4/optimtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimtool-2.4.3/setup.py` & `optimtool-2.4.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import sys
 
 from setuptools import setup
 
 if sys.version_info < (3, 7, 0):
-    raise OSError(f'optimtool-2.4.3 requires Python >=3.7, but yours is {sys.version}')
+    raise OSError(f'optimtool-2.4.4 requires Python >=3.7, but yours is {sys.version}')
 
 if (3, 7, 0) <= sys.version_info < (3, 8, 0):
     # https://github.com/pypa/setuptools/issues/926#issuecomment-294369342
     try:
         import fastentrypoints
     except ImportError:
         try:
```

