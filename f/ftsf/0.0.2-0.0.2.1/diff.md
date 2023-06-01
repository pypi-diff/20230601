# Comparing `tmp/ftsf-0.0.2.tar.gz` & `tmp/ftsf-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftsf-0.0.2.tar", last modified: Wed May 31 21:25:54 2023, max compression
+gzip compressed data, was "ftsf-0.0.2.1.tar", last modified: Thu Jun  1 20:02:18 2023, max compression
```

## Comparing `ftsf-0.0.2.tar` & `ftsf-0.0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.684793 ftsf-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.657826 ftsf-0.0.2/FTSF.egg-info/
--rw-rw-rw-   0        0        0     1185 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1100 2023-05-26 02:11:38.000000 ftsf-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1185 2023-05-31 21:25:54.683795 ftsf-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-05-29 03:05:15.000000 ftsf-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.675587 ftsf-0.0.2/ftsf/
--rw-rw-rw-   0        0        0      587 2023-05-31 21:20:54.000000 ftsf-0.0.2/ftsf/__init__.py
--rw-rw-rw-   0        0        0     3533 2023-05-31 21:20:02.000000 ftsf-0.0.2/ftsf/backtest.py
--rw-rw-rw-   0        0        0     7399 2023-05-31 21:22:08.000000 ftsf-0.0.2/ftsf/evaluation.py
--rw-rw-rw-   0        0        0     8687 2023-05-31 21:18:58.000000 ftsf-0.0.2/ftsf/model.py
--rw-rw-rw-   0        0        0     4601 2023-05-31 21:15:23.000000 ftsf-0.0.2/ftsf/preprocessing.py
--rw-rw-rw-   0        0        0     2178 2023-05-31 21:19:24.000000 ftsf-0.0.2/ftsf/scaler.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.681781 ftsf-0.0.2/ftsf/tests/
--rw-rw-rw-   0        0        0     5000 2023-05-31 21:02:22.000000 ftsf-0.0.2/ftsf/tests/test_evaluation.py
--rw-rw-rw-   0        0        0      643 2023-05-31 21:02:22.000000 ftsf-0.0.2/ftsf/tests/test_preprocessing.py
--rw-rw-rw-   0        0        0      440 2023-05-31 21:02:22.000000 ftsf-0.0.2/ftsf/tests/test_scaler.py
--rw-rw-rw-   0        0        0     6197 2023-05-31 21:18:24.000000 ftsf-0.0.2/ftsf/utils.py
--rw-rw-rw-   0        0        0      810 2023-05-31 21:25:28.000000 ftsf-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 21:25:54.684793 ftsf-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.500089 ftsf-0.0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-01 20:02:18.500089 ftsf-0.0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.496089 ftsf-0.0.2.1/ftsf/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.496089 ftsf-0.0.2.1/ftsf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/tests/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.496089 ftsf-0.0.2.1/ftsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:02:18.500089 ftsf-0.0.2.1/setup.cfg
```

### Comparing `ftsf-0.0.2/FTSF.egg-info/PKG-INFO` & `ftsf-0.0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: ftsf
-Version: 0.0.2
-Summary: Package for financial time series forecasting.
-Author-email: Nikita Safonov <sixxio@yandex.ru>
-Project-URL: Homepage, https://github.com/sixxio/ftsf
-Project-URL: Documentation, https://sixxio.github.io/ftsf/
-Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ftsf
-This package provides high-level interface to work with financial time series forecasting models.
-### Installation
-To install this package run command:
-> pip install ftsf
-### Usage
-The usage of package is simple:
-> from ftsf.model import Model  
-> from ftsf.preprocessing import get_data  
-> x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
-> model = Model('LSTM x2', lag = 15)  
-> model.fit(x_train, y_train)
-> model.evaluate(x_test, y_test, scaler)  
-{'mse' : 0.679, 'mae' : 0.8291, 'mape' : 0.00783, 'r2' : 0.98778}
+Metadata-Version: 2.1
+Name: ftsf
+Version: 0.0.2.1
+Summary: Package for financial time series forecasting.
+Author-email: Nikita Safonov <sixxio@yandex.ru>
+Project-URL: Homepage, https://github.com/sixxio/ftsf
+Project-URL: Documentation, https://sixxio.github.io/ftsf/
+Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ftsf
+This package provides high-level interface to work with financial time series forecasting models.
+### Installation
+To install this package run command:
+> pip install ftsf
+### Usage
+The usage of package is simple:
+> from ftsf.model import Model  
+> from ftsf.preprocessing import get_data  
+> x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
+> model = Model('LSTM x2', lag = 15)  
+> model.fit(x_train, y_train)
+> model.evaluate(x_test, y_test, scaler)  
+{'mse' : 0.679, 'mae' : 0.8291, 'mape' : 0.00783, 'r2' : 0.98778}
```

### Comparing `ftsf-0.0.2/PKG-INFO` & `ftsf-0.0.2.1/ftsf.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1
-Name: ftsf
-Version: 0.0.2
-Summary: Package for financial time series forecasting.
-Author-email: Nikita Safonov <sixxio@yandex.ru>
-Project-URL: Homepage, https://github.com/sixxio/ftsf
-Project-URL: Documentation, https://sixxio.github.io/ftsf/
-Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ftsf
-This package provides high-level interface to work with financial time series forecasting models.
-### Installation
-To install this package run command:
-> pip install ftsf
-### Usage
-The usage of package is simple:
-> from ftsf.model import Model  
-> from ftsf.preprocessing import get_data  
-> x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
-> model = Model('LSTM x2', lag = 15)  
-> model.fit(x_train, y_train)
-> model.evaluate(x_test, y_test, scaler)  
-{'mse' : 0.679, 'mae' : 0.8291, 'mape' : 0.00783, 'r2' : 0.98778}
+Metadata-Version: 2.1
+Name: ftsf
+Version: 0.0.2.1
+Summary: Package for financial time series forecasting.
+Author-email: Nikita Safonov <sixxio@yandex.ru>
+Project-URL: Homepage, https://github.com/sixxio/ftsf
+Project-URL: Documentation, https://sixxio.github.io/ftsf/
+Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ftsf
+This package provides high-level interface to work with financial time series forecasting models.
+### Installation
+To install this package run command:
+> pip install ftsf
+### Usage
+The usage of package is simple:
+> from ftsf.model import Model  
+> from ftsf.preprocessing import get_data  
+> x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
+> model = Model('LSTM x2', lag = 15)  
+> model.fit(x_train, y_train)
+> model.evaluate(x_test, y_test, scaler)  
+{'mse' : 0.679, 'mae' : 0.8291, 'mape' : 0.00783, 'r2' : 0.98778}
```

### Comparing `ftsf-0.0.2/README.md` & `ftsf-0.0.2.1/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# ftsf
-This package provides high-level interface to work with financial time series forecasting models.
-### Installation
-To install this package run command:
-> pip install ftsf
-### Usage
-The usage of package is simple:
-> from ftsf.model import Model  
-> from ftsf.preprocessing import get_data  
-> x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
-> model = Model('LSTM x2', lag = 15)  
-> model.fit(x_train, y_train)
-> model.evaluate(x_test, y_test, scaler)  
+# ftsf
+This package provides high-level interface to work with financial time series forecasting models.
+### Installation
+To install this package run command:
+> pip install ftsf
+### Usage
+The usage of package is simple:
+> from ftsf.model import Model  
+> from ftsf.preprocessing import get_data  
+> x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
+> model = Model('LSTM x2', lag = 15)  
+> model.fit(x_train, y_train)
+> model.evaluate(x_test, y_test, scaler)  
 {'mse' : 0.679, 'mae' : 0.8291, 'mape' : 0.00783, 'r2' : 0.98778}
```

### Comparing `ftsf-0.0.2/ftsf/backtest.py` & `ftsf-0.0.2.1/ftsf/backtest.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-'''This submodule contains instrument to test trading strategy based on model on historical data.'''
-
-import numpy as np
-
-from .model import Model
-from .scaler import Scaler
-
-
-class BackTesting:
-    '''
-    Models trading strategy and backtests it.
-
-    Attributes:
-
-        initial_money: Initial amount of money to work with.
-
-        money: Current amount of money.
-
-        stocks: Current amount of stocks.
-
-        model: Instance of model used for forecasting.
-    '''
-    __initial_money = 0
-    __money = 0
-    __stocks = 0
-    __model = None
-
-    def __init__(self, model : Model, initial_money : float):
-        '''
-        Initializes money and model.
-        '''
-        self.__model = model
-        self.__initial_money = initial_money
-
-    def __sell(self, price : float):
-        '''
-        Internal method to model stocks selling.
-        '''
-        volume = self.__stocks
-        self.__money += volume*price
-        self.__stocks -= volume
-
-    def __buy(self, price : float):
-        '''
-        Internal method to model stocks buying.
-        '''
-        volume = int(self.__money / price)
-        self.__money -= volume*price
-        self.__stocks += volume
-
-    def __predict_steps(self, current_state : list, depth = 15, steps_forward = 1) -> float:
-        '''
-        Internal method to forecast for a few steps forward.
-        '''
-        current_state = current_state.copy()
-        scaler = Scaler().fit(current_state)
-        for i in range(steps_forward):
-            current_state += self.__model.predict(scaler.scale(np.array(current_state[-depth:]).reshape((1,depth,1))), scaler).reshape(-1).tolist()
-        return current_state[-1]
-
-    def test(self, states, depth = 15, steps_forward = 5):
-        '''
-        Implements strategy based on model forecasts, then backtests it.
-
-        Args:
-
-            states: Array of historic values.
-
-            depth: Number of values to forecast on.
-
-            steps_forward: Number of steps to forecast.
-
-        Example:
-        >>> str = Backtesting(model, 10e4)
-        >>> str.test(states, 15, 1)
-        Successfully tested: 12532
-        +2532 or 25.32% in 50 days.
-        2 trades, avg profit 1266 $ per trade.
-        '''
-        self.__money = self.__initial_money
-        trades_no = 0
-        for i in range(len(states)-depth):
-            current_state = states[i:i+depth]
-            if (self.__predict_steps(current_state, depth, steps_forward) > current_state[-1]):
-                if self.__money > current_state[-1]:
-                    self.__buy(current_state[-1])
-                    print(f'Bought {self.__stocks} stocks.')
-                    bought = current_state[-1]
-                    trades_no +=1
-            else:
-                if self.__stocks > 0:
-                    print(f'Sold {self.__stocks} stocks.')
-                    print(f'Delta = {current_state[-1] - bought}/stock')
-                    self.__sell(current_state[-1])
-        self.__sell(current_state[-1])
-        print(f'Successfully tested: \n{self.__money }$')
-        print(f'{"+" if self.__money - self.__initial_money > 0 else ""}{round(self.__money - self.__initial_money)}$ or \
-        {"+" if self.__money - self.__initial_money>0 else ""}{round((self.__money - self.__initial_money)/self.__initial_money*100)}% in {len(states)} days.')
-        print(f'{trades_no}, avg profit {(self.__money - self.__initial_money)/trades_no}$ per trade.')
+'''This submodule contains instrument to test trading strategy based on model on historical data.'''
+
+import numpy as np
+
+from .model import Model
+from .scaler import Scaler
+
+
+class BackTesting:
+    '''
+    Models trading strategy and backtests it.
+
+    Attributes:
+
+        initial_money: Initial amount of money to work with.
+
+        money: Current amount of money.
+
+        stocks: Current amount of stocks.
+
+        model: Instance of model used for forecasting.
+    '''
+    __initial_money = 0
+    __money = 0
+    __stocks = 0
+    __model = None
+
+    def __init__(self, model : Model, initial_money : float):
+        '''
+        Initializes money and model.
+        '''
+        self.__model = model
+        self.__initial_money = initial_money
+
+    def __sell(self, price : float):
+        '''
+        Internal method to model stocks selling.
+        '''
+        volume = self.__stocks
+        self.__money += volume*price
+        self.__stocks -= volume
+
+    def __buy(self, price : float):
+        '''
+        Internal method to model stocks buying.
+        '''
+        volume = int(self.__money / price)
+        self.__money -= volume*price
+        self.__stocks += volume
+
+    def __predict_steps(self, current_state : list, depth = 15, steps_forward = 1) -> float:
+        '''
+        Internal method to forecast for a few steps forward.
+        '''
+        current_state = current_state.copy()
+        scaler = Scaler().fit(current_state)
+        for i in range(steps_forward):
+            current_state += self.__model.predict(scaler.scale(np.array(current_state[-depth:]).reshape((1,depth,1))), scaler).reshape(-1).tolist()
+        return current_state[-1]
+
+    def test(self, states, depth = 15, steps_forward = 5):
+        '''
+        Implements strategy based on model forecasts, then backtests it.
+
+        Args:
+
+            states: Array of historic values.
+
+            depth: Number of values to forecast on.
+
+            steps_forward: Number of steps to forecast.
+
+        Example:
+        >>> str = Backtesting(model, 10e4)
+        >>> str.test(states, 15, 1)
+        Successfully tested: 12532
+        +2532 or 25.32% in 50 days.
+        2 trades, avg profit 1266 $ per trade.
+        '''
+        self.__money = self.__initial_money
+        trades_no = 0
+        for i in range(len(states)-depth):
+            current_state = states[i:i+depth]
+            if (self.__predict_steps(current_state, depth, steps_forward) > current_state[-1]):
+                if self.__money > current_state[-1]:
+                    self.__buy(current_state[-1])
+                    print(f'Bought {self.__stocks} stocks.')
+                    bought = current_state[-1]
+                    trades_no +=1
+            else:
+                if self.__stocks > 0:
+                    print(f'Sold {self.__stocks} stocks.')
+                    print(f'Delta = {current_state[-1] - bought}/stock')
+                    self.__sell(current_state[-1])
+        self.__sell(current_state[-1])
+        print(f'Successfully tested: \n{self.__money }$')
+        print(f'{"+" if self.__money - self.__initial_money > 0 else ""}{round(self.__money - self.__initial_money)}$ or \
+        {"+" if self.__money - self.__initial_money>0 else ""}{round((self.__money - self.__initial_money)/self.__initial_money*100)}% in {len(states)} days.')
+        print(f'{trades_no}, avg profit {(self.__money - self.__initial_money)/trades_no}$ per trade.')
```

### Comparing `ftsf-0.0.2/ftsf/evaluation.py` & `ftsf-0.0.2.1/ftsf/evaluation.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-'''This submodule contains methods to evaluate models.'''
-
-import time
-import warnings
-
-import pandas as pd
-from sklearn.metrics import (mean_absolute_error,
-                             mean_absolute_percentage_error,
-                             mean_squared_error, r2_score)
-
-warnings.filterwarnings("ignore")
-
-from .model import Model
-from .utils import get_models
-
-
-def evaluate_ml_models(x_train, x_test, y_train, y_test, scaler, out_type = 'list'):
-    '''
-    Evaluates machine learning models on data.
-
-    Args:
-
-        x_train: Input values to fit model.
-
-        x_test: Input values to evaluate model.
-
-        y_train: Target values to fit model.
-
-        y_test: Target values to fit model.
-
-        scaler: Scaler to scale/unscale values during evaluation.
-
-        out_type: Format to return data.
-
-    Returns:
-
-        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
-
-        or pd.DataFrame: dataframe with the same data.
-
-    Example:
-    >>> evaluate_ml_models(x_train, x_test, y_train, y_test, scaler)
-    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LR'}, ...]
-    '''
-    statistics = []
-    for i in get_models('ml'):
-        current_model = Model(i)
-        start_time = time.time()
-        current_model.fit(x_train, y_train)
-        utilized = time.time() - start_time
-        pred = current_model.predict(x_test, scaler)
-        true = scaler.unscale(y_test)
-        statistics.append({ 'time': utilized,
-                    'mse': mean_squared_error(true, pred),
-                    'mae': mean_absolute_error(true, pred),
-                    'mape': mean_absolute_percentage_error(true, pred),
-                    'r2':  r2_score(true, pred),
-                    'model': i})
-
-    if out_type == 'df':
-        return pd.DataFrame(statistics).sort_values(by='mape')
-    elif out_type == 'list':
-        return statistics
-
-def evaluate_ar_models(x_train, x_test, y_train, y_test, scaler, out_type = 'list'):
-    '''
-    Evaluates autoregressive models on data.
-
-    Args:
-
-        x_train: Input values to fit model.
-
-        x_test: Input values to evaluate model.
-
-        y_train: Target values to fit model.
-
-        y_test: Target values to fit model.
-
-        scaler: Scaler to scale/unscale values during evaluation.
-
-        out_type: Format to return data.
-
-    Returns:
-
-        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
-
-        or pd.DataFrame : dataframe with the same data.
-
-    Example:
-    >>> evaluate_ar_models(x_train, x_test, y_train, y_test, scaler)
-    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'ARMA(2,1)'}, ...]
-    '''
-    statistics = []
-    for i in get_models('ar'):
-        pred = []
-        for j in range(len(y_test)):
-            start_time = time.time()
-            current_model = Model(i).fit(x_test[j], y_test[j])
-            utilized = time.time() - start_time
-            pred.append(current_model.predict(x_test[j], scaler))
-        true = scaler.unscale(y_test)
-        statistics.append({ 'time': utilized,
-                    'mse': mean_squared_error(true, pred),
-                    'mae': mean_absolute_error(true, pred),
-                    'mape': mean_absolute_percentage_error(true, pred),
-                    'r2':  r2_score(true, pred),
-                    'model': i})
-
-    if out_type == 'df':
-        return pd.DataFrame(statistics).sort_values(by='mape')
-    elif out_type == 'list':
-        return statistics
-
-def evaluate_nn_models(x_train, x_test, y_train, y_test, scaler, optimizer = 'nadam', loss = 'mse', epochs = 10, batch_size = 256, out_type = 'list'):
-    '''
-    Evaluates neural network based models on data.
-
-    Args:
-
-        x_train: Input values to fit model.
-
-        x_test: Input values to evaluate model.
-
-        y_train: Target values to fit model.
-
-        y_test: Target values to fit model.
-
-        scaler: Scaler to scale/unscale values during evaluation.
-
-        optimizer: tf.Keras optimizer name (optional: only for neural networks).
-
-        loss: tf.Keras loss name (optional: only for neural networks).
-
-        epochs: Number of epochs during fitting (optional: only for neural networks).
-
-        batch_size: Size of batch during fitting (optional: only for neural networks).
-
-        out_type: Format to return data.
-
-    Returns:
-
-        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
-
-        or pd.DataFrame: dataframe with the same data.
-
-    Example:
-    >>> evaluate_nn_models(x_train, x_test, y_train, y_test, scaler)
-    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LSTM x1'}, ...]
-    '''
-
-    statistics = []
-    for i in get_models('nn'):
-        current_model = Model(i, lag = x_train.shape[1]+1, optimizer=optimizer, loss=loss)
-        start_time = time.time()
-        current_model.fit(x_train, y_train, epochs, batch_size)
-        utilized = time.time() - start_time
-        pred = current_model.predict(x_test, scaler)
-        true = scaler.unscale(y_test)
-        statistics.append({ 'time': utilized,
-                    'mse': mean_squared_error(true, pred),
-                    'mae': mean_absolute_error(true, pred),
-                    'mape': mean_absolute_percentage_error(true, pred),
-                    'r2':  r2_score(true, pred),
-                    'model': i})
-
-    if out_type == 'df':
-        return pd.DataFrame(statistics).sort_values(by='mape')
-    elif out_type == 'list':
-        return statistics
-
-
-def evaluate_all_models(x_train, x_test, y_train, y_test, scaler, optimizer = 'nadam', loss = 'mse', epochs = 10, batch_size = 256, out_type = 'df'):
-    '''
-    Evaluates all models on data.
-
-    Args:
-
-        x_train: Input values to fit model.
-
-        x_test: Input values to evaluate model.
-
-        y_train: Target values to fit model.
-
-        y_test: Target values to fit model.
-
-        scaler: Scaler to scale/unscale values during evaluation.
-
-        optimizer: tf.Keras optimizer name (optional: only for neural networks).
-
-        loss: tf.Keras loss name (optional: only for neural networks).
-
-        epochs: Number of epochs during fitting (optional: only for neural networks).
-
-        batch_size: Size of batch during fitting (optional: only for neural networks).
-
-        out_type: Format to return data.
-
-    Returns:
-
-        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
-
-        or pd.DataFrame: dataframe with the same data.
-
-    Example:
-    >>> evaluate_all_models(x_train, x_test, y_train, y_test, scaler)
-    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LR'}, ...]
-    '''
-
-    statistics = evaluate_ml_models(x_train, x_test, y_train, y_test, scaler)
-    statistics += evaluate_ar_models(x_train, x_test, y_train, y_test, scaler)
-    statistics += evaluate_nn_models(x_train, x_test, y_train, y_test, scaler, optimizer, loss, epochs, batch_size)
-
-    if out_type == 'df':
-        return pd.DataFrame(statistics).sort_values(by='mape')
-    elif out_type == 'list':
-        return statistics
+'''This submodule contains methods to evaluate models.'''
+
+import time
+import warnings
+
+import pandas as pd
+from sklearn.metrics import (mean_absolute_error,
+                             mean_absolute_percentage_error,
+                             mean_squared_error, r2_score)
+
+warnings.filterwarnings("ignore")
+
+from .model import Model
+from .utils import get_models
+
+
+def evaluate_ml_models(x_train, x_test, y_train, y_test, scaler, out_type = 'list'):
+    '''
+    Evaluates machine learning models on data.
+
+    Args:
+
+        x_train: Input values to fit model.
+
+        x_test: Input values to evaluate model.
+
+        y_train: Target values to fit model.
+
+        y_test: Target values to fit model.
+
+        scaler: Scaler to scale/unscale values during evaluation.
+
+        out_type: Format to return data.
+
+    Returns:
+
+        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
+
+        or pd.DataFrame: dataframe with the same data.
+
+    Example:
+    >>> evaluate_ml_models(x_train, x_test, y_train, y_test, scaler)
+    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LR'}, ...]
+    '''
+    statistics = []
+    for i in get_models('ml'):
+        current_model = Model(i)
+        start_time = time.time()
+        current_model.fit(x_train, y_train)
+        utilized = time.time() - start_time
+        pred = current_model.predict(x_test, scaler)
+        true = scaler.unscale(y_test)
+        statistics.append({ 'time': utilized,
+                    'mse': mean_squared_error(true, pred),
+                    'mae': mean_absolute_error(true, pred),
+                    'mape': mean_absolute_percentage_error(true, pred),
+                    'r2':  r2_score(true, pred),
+                    'model': i})
+
+    if out_type == 'df':
+        return pd.DataFrame(statistics).sort_values(by='mape')
+    elif out_type == 'list':
+        return statistics
+
+def evaluate_ar_models(x_train, x_test, y_train, y_test, scaler, out_type = 'list'):
+    '''
+    Evaluates autoregressive models on data.
+
+    Args:
+
+        x_train: Input values to fit model.
+
+        x_test: Input values to evaluate model.
+
+        y_train: Target values to fit model.
+
+        y_test: Target values to fit model.
+
+        scaler: Scaler to scale/unscale values during evaluation.
+
+        out_type: Format to return data.
+
+    Returns:
+
+        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
+
+        or pd.DataFrame : dataframe with the same data.
+
+    Example:
+    >>> evaluate_ar_models(x_train, x_test, y_train, y_test, scaler)
+    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'ARMA(2,1)'}, ...]
+    '''
+    statistics = []
+    for i in get_models('ar'):
+        pred = []
+        for j in range(len(y_test)):
+            start_time = time.time()
+            current_model = Model(i).fit(x_test[j], y_test[j])
+            utilized = time.time() - start_time
+            pred.append(current_model.predict(x_test[j], scaler))
+        true = scaler.unscale(y_test)
+        statistics.append({ 'time': utilized,
+                    'mse': mean_squared_error(true, pred),
+                    'mae': mean_absolute_error(true, pred),
+                    'mape': mean_absolute_percentage_error(true, pred),
+                    'r2':  r2_score(true, pred),
+                    'model': i})
+
+    if out_type == 'df':
+        return pd.DataFrame(statistics).sort_values(by='mape')
+    elif out_type == 'list':
+        return statistics
+
+def evaluate_nn_models(x_train, x_test, y_train, y_test, scaler, optimizer = 'nadam', loss = 'mse', epochs = 10, batch_size = 256, out_type = 'list'):
+    '''
+    Evaluates neural network based models on data.
+
+    Args:
+
+        x_train: Input values to fit model.
+
+        x_test: Input values to evaluate model.
+
+        y_train: Target values to fit model.
+
+        y_test: Target values to fit model.
+
+        scaler: Scaler to scale/unscale values during evaluation.
+
+        optimizer: tf.Keras optimizer name (optional: only for neural networks).
+
+        loss: tf.Keras loss name (optional: only for neural networks).
+
+        epochs: Number of epochs during fitting (optional: only for neural networks).
+
+        batch_size: Size of batch during fitting (optional: only for neural networks).
+
+        out_type: Format to return data.
+
+    Returns:
+
+        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
+
+        or pd.DataFrame: dataframe with the same data.
+
+    Example:
+    >>> evaluate_nn_models(x_train, x_test, y_train, y_test, scaler)
+    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LSTM x1'}, ...]
+    '''
+
+    statistics = []
+    for i in get_models('nn'):
+        current_model = Model(i, lag = x_train.shape[1]+1, optimizer=optimizer, loss=loss)
+        start_time = time.time()
+        current_model.fit(x_train, y_train, epochs, batch_size)
+        utilized = time.time() - start_time
+        pred = current_model.predict(x_test, scaler)
+        true = scaler.unscale(y_test)
+        statistics.append({ 'time': utilized,
+                    'mse': mean_squared_error(true, pred),
+                    'mae': mean_absolute_error(true, pred),
+                    'mape': mean_absolute_percentage_error(true, pred),
+                    'r2':  r2_score(true, pred),
+                    'model': i})
+
+    if out_type == 'df':
+        return pd.DataFrame(statistics).sort_values(by='mape')
+    elif out_type == 'list':
+        return statistics
+
+
+def evaluate_all_models(x_train, x_test, y_train, y_test, scaler, optimizer = 'nadam', loss = 'mse', epochs = 10, batch_size = 256, out_type = 'df'):
+    '''
+    Evaluates all models on data.
+
+    Args:
+
+        x_train: Input values to fit model.
+
+        x_test: Input values to evaluate model.
+
+        y_train: Target values to fit model.
+
+        y_test: Target values to fit model.
+
+        scaler: Scaler to scale/unscale values during evaluation.
+
+        optimizer: tf.Keras optimizer name (optional: only for neural networks).
+
+        loss: tf.Keras loss name (optional: only for neural networks).
+
+        epochs: Number of epochs during fitting (optional: only for neural networks).
+
+        batch_size: Size of batch during fitting (optional: only for neural networks).
+
+        out_type: Format to return data.
+
+    Returns:
+
+        list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
+
+        or pd.DataFrame: dataframe with the same data.
+
+    Example:
+    >>> evaluate_all_models(x_train, x_test, y_train, y_test, scaler)
+    [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LR'}, ...]
+    '''
+
+    statistics = evaluate_ml_models(x_train, x_test, y_train, y_test, scaler)
+    statistics += evaluate_ar_models(x_train, x_test, y_train, y_test, scaler)
+    statistics += evaluate_nn_models(x_train, x_test, y_train, y_test, scaler, optimizer, loss, epochs, batch_size)
+
+    if out_type == 'df':
+        return pd.DataFrame(statistics).sort_values(by='mape')
+    elif out_type == 'list':
+        return statistics
```

### Comparing `ftsf-0.0.2/ftsf/model.py` & `ftsf-0.0.2.1/ftsf/model.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,245 +1,245 @@
-'''This submodule contains generic model class.'''
-
-import numpy as np
-from catboost import CatBoostRegressor
-from joblib import dump, load
-from sklearn.ensemble import GradientBoostingRegressor, RandomForestRegressor
-from sklearn.linear_model import LinearRegression
-from sklearn.metrics import (mean_absolute_error,
-                             mean_absolute_percentage_error,
-                             mean_squared_error, r2_score)
-from sklearn.svm import SVR
-from sklearn.tree import DecisionTreeRegressor
-from statsmodels.tsa.arima.model import ARIMA
-from tensorflow.keras import Sequential
-from tensorflow.keras.models import load_model, save_model
-from xgboost import XGBRegressor, XGBRFRegressor
-
-from .utils import get_topologies, parse_name
-
-
-class Model:
-    '''
-    Generic ML/AR/NN based model with unified interface.
-
-
-    Models:
-
-        ML: LinearRegression, DecisionTreeRegressor, RandomForestRegressor, GradientBoostingRegressor, SVR, CatBoostRegressor, XGBoostRegressor, XGBoostRandomForestRegressor.
-
-        AR: ARMA, ARIMA.
-
-        NN: CNN + SimpleRNN/LSTM/GRU, LSTM x1-3, GRU x1-3, SimpleRNN x1-3, CNN, MLP(1-3).
-
-    Attributes:
-
-        type: Type of model.
-
-        backend: Type of backend used to work with model.
-
-        name: Model name.
-
-        model: Model object.
-    '''
-
-    __type = ''
-    __backend = ''
-    __name = ''
-    __model = None
-
-    def __init__(self, name, lag = 15, optimizer = 'nadam', loss = 'mse'):
-        '''
-        Initializes the instance of model based on defined type.
-
-        Args:
-
-            name: Defines exact model.
-
-            lag: An integer indicating number of values to base prediction on.
-
-            data: Data to use on autoregressive model fit.
-
-            optimizer: Optimizer to use on compiling neural network based models.
-
-            loss: Loss function to use on compiling neural network based models.
-
-        Example:
-        >>> Model('LSTM x2', 15)
-        '''
-        models = {'ml': ['LR', 'DTR', 'RFR', 'GBR', 'SVR', 'CBR', 'XGBR', 'XGBRFR'],
-                  'ar': ['ARMA(2,1)', 'ARIMA(2,1,1)'],
-                  'nn': ['CNN + LSTM', 'LSTM x3', 'LSTM x2', 'LSTM x1', 'CNN + GRU', 'GRU x3', 'GRU x2', 'GRU x1', \
-                         'CNN + SimpleRNN', 'SimpleRNN x3', 'SimpleRNN x2', 'SimpleRNN x1', 'CNN', 'MLP(3)', 'MLP(2)', 'MLP(1)']}
-
-        self.__type = [key for key, value in models.items() if name in value][0]
-        self.__name = name
-
-        if self.__type == 'ml':
-            if name == 'CBR':
-                self.__backend = 'Catboost'
-            elif name[:2] == 'XG':
-                self.__backend = 'XGBoost'
-            else:
-                self.__backend = 'Scikit-learn'
-
-            self.__model = {  'LR' :  LinearRegression(),
-                            'DTR' : DecisionTreeRegressor(min_samples_leaf=5),
-                            'RFR' : RandomForestRegressor(),
-                            'GBR' : GradientBoostingRegressor(),
-                            'SVR' : SVR(kernel='linear', epsilon=1e-3),
-                            'CBR' : CatBoostRegressor(loss_function='MAPE'),
-                            'XGBR': XGBRegressor(objective='reg:squarederror'),
-                            'XGBRFR': XGBRFRegressor(objective = 'reg:squarederror')}[name]
-
-        elif self.__type == 'ar':
-            self.__backend = 'Statsmodels'
-
-        elif self.__type == 'nn':
-            self.__backend = 'TensorFlow.Keras'
-            self.__model = Sequential(get_topologies(lag)[name])
-            self.__model.compile(optimizer = optimizer, loss = loss,  metrics = ['mse', 'mae', 'mape'])
-
-    def fit(self, x_train, y_train, epochs = 25, batch_size = 32):
-        '''
-        Fits model using x_train and y_train.
-
-        Note that autoregressive models differ from other and can be fitted only on one sample of data.
-
-        Args:
-
-            x_train: Array with previous price values.
-
-            y_train: Array with target price values.
-
-            epochs: Number of epochs in case of using neural network.
-
-            batch_size: Number of objects in one fit batch in case of using neural network.
-
-        Example:
-        >>> model.fit(x_train, y_train)
-        '''
-
-        if self.__type == 'nn':
-            x_train = x_train.reshape((x_train.shape[0], x_train.shape[1], 1))
-            self.__model.fit(x_train, y_train, epochs = epochs, batch_size = batch_size, verbose = 0)
-        elif self.__name == 'CBR':
-            x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
-            self.__model.fit(x_train, y_train, silent = True)
-        elif self.__backend != 'Statsmodels':
-            x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
-            self.__model.fit(x_train, y_train)
-        elif self.__backend == 'Statsmodels':
-            self.__model = ARIMA(x_train, order = parse_name(self.__name), enforce_stationarity = False)
-
-        return self
-
-    def predict(self, x_test, scaler):
-        '''
-        Predicts and scales values using x_test and scaler.
-
-        Args:
-
-            x_test - previous price values;
-
-            scaler - scaler will be used to scale values back.
-
-        Returns:
-
-            Array of predicted and scaled price values.
-
-        Example:
-        >>> model.predict(x_test, scaler)
-        [123, 124, 123, 128]
-        '''
-
-        if self.__type == 'ar':
-            x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
-            return scaler.unscale(self.__model.fit().forecast(steps = 1)[0])
-        elif self.__type == 'nn':
-            x_test = x_test.reshape((x_test.shape[0], x_test.shape[1], 1))
-            return scaler.unscale(self.__model.predict(x_test, verbose = 0).reshape(-1))
-        else:
-            x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
-            return scaler.unscale(self.__model.predict(x_test))
-
-    def evaluate(self, x_test, y_test, scaler):
-        '''
-        Predicts and scales values using x_test and scaler, then measures MSE, MAE, MAPE and R2.
-
-        Args:
-
-            x_test: Array with previous price values.
-
-            y_test: Array with target price values.
-
-            scaler: Scaler to be used to scale values back.
-
-        Returns:
-
-            Dict with errors values.
-
-        Example:
-        >>> model.evaluate(x_test, y_test, scaler)
-        {'mse': 123.123, 'mae': 123.123, 'mape': 123.123, 'r2': 123.123}
-        '''
-
-        true = scaler.unscale(y_test)
-        prediction = self.predict(x_test, scaler)
-        return {'mse': mean_squared_error(np.array(true), np.array(prediction)),
-                'mae': mean_absolute_error(np.array(true), np.array(prediction)),
-                'mape': mean_absolute_percentage_error(np.array(true), np.array(prediction)),
-                'r2':  r2_score(np.array(true), np.array(prediction))}
-
-    def summary(self):
-        '''
-        Shows short summary about model, its type and backend.
-
-        Returns:
-
-            String with short model description.
-
-        Example:
-        >>> model.summary()
-        ML model XGBRegressor, backend is based on XGBoost.
-        '''
-
-        print(f'{self.__type.upper()} model {self.__name}, backend is based on {self.__backend}.')
-
-    def save(self, filename):
-        '''
-        Saves the trained model to a file.
-
-        Args:
-
-            filename: Path to save model file.
-
-        Example:
-        >>> model.save('saved_model.h5')
-        Model has been saved to saved_model.h5
-        '''
-        if self.__type == 'ml':
-            dump(self.__model, f'{filename}.joblib')
-            print(f'Model has been saved to {filename}.joblib.')
-        elif self.__type == 'nn':
-            save_model(self.__model, f'{filename}.h5')
-            print(f'Model has been saved to {filename}.h5.')
-        elif self.__type == 'ar':
-            print('Saving and loading AutoRegressive models is still developing.')
-
-    def load(self, filename):
-        '''
-        Loads a trained model from a file.
-
-        Args:
-            filename: Path to saved model file.
-
-        Example:
-        >>> model.load('saved_model.h5')
-        '''
-        if self.__type == 'ml':
-            self.__model = load(f'{filename}')
-        elif self.__type == 'nn':
-            self.__model = load_model(f'{filename}')
-        elif self.__type == 'ar':
-            print('Saving and loading AutoRegressive models is still developing.')
-        return self
+'''This submodule contains generic model class.'''
+
+import numpy as np
+from catboost import CatBoostRegressor
+from joblib import dump, load
+from sklearn.ensemble import GradientBoostingRegressor, RandomForestRegressor
+from sklearn.linear_model import LinearRegression
+from sklearn.metrics import (mean_absolute_error,
+                             mean_absolute_percentage_error,
+                             mean_squared_error, r2_score)
+from sklearn.svm import SVR
+from sklearn.tree import DecisionTreeRegressor
+from statsmodels.tsa.arima.model import ARIMA
+from tensorflow.keras import Sequential
+from tensorflow.keras.models import load_model, save_model
+from xgboost import XGBRegressor, XGBRFRegressor
+
+from .utils import get_topologies, parse_name
+
+
+class Model:
+    '''
+    Generic ML/AR/NN based model with unified interface.
+
+
+    Models:
+
+        ML: LinearRegression, DecisionTreeRegressor, RandomForestRegressor, GradientBoostingRegressor, SVR, CatBoostRegressor, XGBoostRegressor, XGBoostRandomForestRegressor.
+
+        AR: ARMA, ARIMA.
+
+        NN: CNN + SimpleRNN/LSTM/GRU, LSTM x1-3, GRU x1-3, SimpleRNN x1-3, CNN, MLP(1-3).
+
+    Attributes:
+
+        type: Type of model.
+
+        backend: Type of backend used to work with model.
+
+        name: Model name.
+
+        model: Model object.
+    '''
+
+    __type = ''
+    __backend = ''
+    __name = ''
+    __model = None
+
+    def __init__(self, name, lag = 15, optimizer = 'nadam', loss = 'mse'):
+        '''
+        Initializes the instance of model based on defined type.
+
+        Args:
+
+            name: Defines exact model.
+
+            lag: An integer indicating number of values to base prediction on.
+
+            data: Data to use on autoregressive model fit.
+
+            optimizer: Optimizer to use on compiling neural network based models.
+
+            loss: Loss function to use on compiling neural network based models.
+
+        Example:
+        >>> Model('LSTM x2', 15)
+        '''
+        models = {'ml': ['LR', 'DTR', 'RFR', 'GBR', 'SVR', 'CBR', 'XGBR', 'XGBRFR'],
+                  'ar': ['ARMA(2,1)', 'ARIMA(2,1,1)'],
+                  'nn': ['CNN + LSTM', 'LSTM x3', 'LSTM x2', 'LSTM x1', 'CNN + GRU', 'GRU x3', 'GRU x2', 'GRU x1', \
+                         'CNN + SimpleRNN', 'SimpleRNN x3', 'SimpleRNN x2', 'SimpleRNN x1', 'CNN', 'MLP(3)', 'MLP(2)', 'MLP(1)']}
+
+        self.__type = [key for key, value in models.items() if name in value][0]
+        self.__name = name
+
+        if self.__type == 'ml':
+            if name == 'CBR':
+                self.__backend = 'Catboost'
+            elif name[:2] == 'XG':
+                self.__backend = 'XGBoost'
+            else:
+                self.__backend = 'Scikit-learn'
+
+            self.__model = {  'LR' :  LinearRegression(),
+                            'DTR' : DecisionTreeRegressor(min_samples_leaf=5),
+                            'RFR' : RandomForestRegressor(),
+                            'GBR' : GradientBoostingRegressor(),
+                            'SVR' : SVR(kernel='linear', epsilon=1e-3),
+                            'CBR' : CatBoostRegressor(loss_function='MAPE'),
+                            'XGBR': XGBRegressor(objective='reg:squarederror'),
+                            'XGBRFR': XGBRFRegressor(objective = 'reg:squarederror')}[name]
+
+        elif self.__type == 'ar':
+            self.__backend = 'Statsmodels'
+
+        elif self.__type == 'nn':
+            self.__backend = 'TensorFlow.Keras'
+            self.__model = Sequential(get_topologies(lag)[name])
+            self.__model.compile(optimizer = optimizer, loss = loss,  metrics = ['mse', 'mae', 'mape'])
+
+    def fit(self, x_train, y_train, epochs = 25, batch_size = 32):
+        '''
+        Fits model using x_train and y_train.
+
+        Note that autoregressive models differ from other and can be fitted only on one sample of data.
+
+        Args:
+
+            x_train: Array with previous price values.
+
+            y_train: Array with target price values.
+
+            epochs: Number of epochs in case of using neural network.
+
+            batch_size: Number of objects in one fit batch in case of using neural network.
+
+        Example:
+        >>> model.fit(x_train, y_train)
+        '''
+
+        if self.__type == 'nn':
+            x_train = x_train.reshape((x_train.shape[0], x_train.shape[1], 1))
+            self.__model.fit(x_train, y_train, epochs = epochs, batch_size = batch_size, verbose = 0)
+        elif self.__name == 'CBR':
+            x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
+            self.__model.fit(x_train, y_train, silent = True)
+        elif self.__backend != 'Statsmodels':
+            x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
+            self.__model.fit(x_train, y_train)
+        elif self.__backend == 'Statsmodels':
+            self.__model = ARIMA(x_train, order = parse_name(self.__name), enforce_stationarity = False)
+
+        return self
+
+    def predict(self, x_test, scaler):
+        '''
+        Predicts and scales values using x_test and scaler.
+
+        Args:
+
+            x_test - previous price values;
+
+            scaler - scaler will be used to scale values back.
+
+        Returns:
+
+            Array of predicted and scaled price values.
+
+        Example:
+        >>> model.predict(x_test, scaler)
+        [123, 124, 123, 128]
+        '''
+
+        if self.__type == 'ar':
+            x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
+            return scaler.unscale(self.__model.fit().forecast(steps = 1)[0])
+        elif self.__type == 'nn':
+            x_test = x_test.reshape((x_test.shape[0], x_test.shape[1], 1))
+            return scaler.unscale(self.__model.predict(x_test, verbose = 0).reshape(-1))
+        else:
+            x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
+            return scaler.unscale(self.__model.predict(x_test))
+
+    def evaluate(self, x_test, y_test, scaler):
+        '''
+        Predicts and scales values using x_test and scaler, then measures MSE, MAE, MAPE and R2.
+
+        Args:
+
+            x_test: Array with previous price values.
+
+            y_test: Array with target price values.
+
+            scaler: Scaler to be used to scale values back.
+
+        Returns:
+
+            Dict with errors values.
+
+        Example:
+        >>> model.evaluate(x_test, y_test, scaler)
+        {'mse': 123.123, 'mae': 123.123, 'mape': 123.123, 'r2': 123.123}
+        '''
+
+        true = scaler.unscale(y_test)
+        prediction = self.predict(x_test, scaler)
+        return {'mse': mean_squared_error(np.array(true), np.array(prediction)),
+                'mae': mean_absolute_error(np.array(true), np.array(prediction)),
+                'mape': mean_absolute_percentage_error(np.array(true), np.array(prediction)),
+                'r2':  r2_score(np.array(true), np.array(prediction))}
+
+    def summary(self):
+        '''
+        Shows short summary about model, its type and backend.
+
+        Returns:
+
+            String with short model description.
+
+        Example:
+        >>> model.summary()
+        ML model XGBRegressor, backend is based on XGBoost.
+        '''
+
+        print(f'{self.__type.upper()} model {self.__name}, backend is based on {self.__backend}.')
+
+    def save(self, filename):
+        '''
+        Saves the trained model to a file.
+
+        Args:
+
+            filename: Path to save model file.
+
+        Example:
+        >>> model.save('saved_model.h5')
+        Model has been saved to saved_model.h5
+        '''
+        if self.__type == 'ml':
+            dump(self.__model, f'{filename}.joblib')
+            print(f'Model has been saved to {filename}.joblib.')
+        elif self.__type == 'nn':
+            save_model(self.__model, f'{filename}.h5')
+            print(f'Model has been saved to {filename}.h5.')
+        elif self.__type == 'ar':
+            print('Saving and loading AutoRegressive models is still developing.')
+
+    def load(self, filename):
+        '''
+        Loads a trained model from a file.
+
+        Args:
+            filename: Path to saved model file.
+
+        Example:
+        >>> model.load('saved_model.h5')
+        '''
+        if self.__type == 'ml':
+            self.__model = load(f'{filename}')
+        elif self.__type == 'nn':
+            self.__model = load_model(f'{filename}')
+        elif self.__type == 'ar':
+            print('Saving and loading AutoRegressive models is still developing.')
+        return self
```

### Comparing `ftsf-0.0.2/ftsf/preprocessing.py` & `ftsf-0.0.2.1/ftsf/preprocessing.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-'''This submodule contains functions to preprocess and update data.'''
-
-import datetime
-import json
-import re
-from pathlib import Path
-
-import numpy as np
-import pandas as pd
-import requests as rq
-
-from .scaler import Scaler
-
-PACKAGEDIR = Path(__file__).parent.absolute()
-
-
-def get_data(ticker = 'AAPL', column = 'close', length = 15, step = 1, start_date = '01-01-2013', split_date = '01-01-2022', end_date = '01-01-2023', flatten = False, validate = False):
-    '''
-    Prepares data for training and evaluating.
-
-    Args:
-
-        ticker: Ticker to get data for.
-
-        column: Column from HLOCV to work with.
-
-        length: Length of arrays, length-1 values are for fitting, 1 value is for evaluating.
-
-        step: Step to cut data using sliding window.
-
-        start_date: Date to start cutting data from.
-
-        split_date: Date to split into train/test.
-
-        end_date: Date to end cutting data.
-
-        flatten: Shape format:  (cuts, length-1) or (cuts, length-1, 1).
-
-        validate: To make validation split or not.
-
-    Returns:
-        x_train, x_test, y_train, y_test, scaler: train and test data with scaler to work with.
-
-    Example:
-    >>> get_data('AAPL', 'close', 10)
-    [[0.122, 0.12, 0.125, ..], ..]
-    [0.12, ..]
-    [[0.132, 0.13, 0.135, ..], ..]
-    [0.13, ..]
-    Scaler()
-    '''
-    data = pd.read_parquet(f'{PACKAGEDIR}/data.parquet.gz')
-    data = data[(data.dateTime >= start_date) & (data.ticker == ticker)]
-
-    train_data = data[(data.dateTime < split_date)][column].values.reshape(-1, 1)
-    test_data =  data[(data.dateTime >= split_date) & (data.dateTime < end_date)][column].values.reshape(-1, 1)
-
-    train_set = [train_data[j:j+length,0] for j in range(0, len(train_data)-length, step)]
-    test_set =  [test_data[j:j+length,0] for j in range(0, len(test_data)-length, step)]
-
-    scaler = Scaler().fit(train_set)
-    scaled_train_set = scaler.scale(train_set)
-    scaled_test_set = scaler.scale(test_set)
-
-    scaled_x_train, scaled_x_test = scaled_train_set[:,:length-1], scaled_test_set[:,:length-1]
-    scaled_y_train, scaled_y_test = scaled_train_set[:,length-1],  scaled_test_set[:,length-1]
-
-    if not flatten:
-        scaled_x_train = np.reshape(scaled_x_train, (scaled_x_train.shape[0], length - 1,1))
-        scaled_x_test = np.reshape(scaled_x_test, (scaled_x_test.shape[0], length - 1,1))
-
-    if validate:
-        val_data = data[(data.dateTime >= end_date) & (data.ticker == ticker)][column].values.reshape(-1, 1)
-        val_set = [val_data[j:j+length,0] for j in range(0, len(val_data)-length, step)]
-        scaled_val_set = scaler.scale(val_set)
-        scaled_x_val, scaled_y_val = scaled_val_set[:,:length-1], scaled_val_set[:,length-1]
-        return scaled_x_train, scaled_x_test, scaled_x_val, scaled_y_train, scaled_y_test, scaled_y_val, scaler
-    else:
-        return scaled_x_train, scaled_x_test, scaled_y_train, scaled_y_test, scaler
-
-def update_data(tickers = []):
-    '''
-    Updates stored data for defined tickers.
-
-    Args:
-
-        tickers (list): Tickers list to update data for.
-
-    Example:
-    >>> get_data(['AMZN', 'TSLA', 'NVDA']])
-    Info about 3 tickers successfully uploaded.
-    '''
-    all_tickers_df = pd.read_parquet(f'{PACKAGEDIR}/data.parquet.gz')
-    for i in tickers:
-        headers = {"Accept":"text/html", "Accept-Language":"en-US", "Referer":"https://www.nasdaq.com/", "User-Agent":"Chrome/64.0.3282.119"}
-        resp = rq.get(f'https://api.nasdaq.com/api/quote/{i}/chart?assetclass=stocks&fromdate=2023-04-29&todate={datetime.datetime.now().strftime("%Y-%m-%d")}', headers=headers, verify=True)
-        if resp.status_code == 200:
-            try:
-                smth = json.loads(re.search('\[.*\]', resp.text).group())
-                cur_tick_data = pd.DataFrame([smth[k]['z'] for k in range(len(smth))])
-                cur_tick_data['ticker'] = i
-                for col_name in ['high','low','open','close','volume','value']:
-                    cur_tick_data[col_name] = pd.to_numeric(cur_tick_data[col_name].str.replace(',',''))
-                cur_tick_data['dateTime'] = pd.to_datetime(cur_tick_data['dateTime'])
-                all_tickers_df = pd.concat([all_tickers_df, cur_tick_data])
-            except KeyError:
-                pass
-        else:
-            print(f'ERROR: smth is wrong with {i}')
-    all_tickers_df.to_parquet(f'{PACKAGEDIR}/data.parquet.gz', compression='gzip')
-    print(f'Info about {len(tickers)} tickers successfully uploaded.')
+'''This submodule contains functions to preprocess and update data.'''
+
+import datetime
+import json
+import re
+from pathlib import Path
+
+import numpy as np
+import pandas as pd
+import requests as rq
+
+from .scaler import Scaler
+
+PACKAGEDIR = Path(__file__).parent.absolute()
+
+
+def get_data(ticker = 'AAPL', column = 'close', length = 15, step = 1, start_date = '01-01-2013', split_date = '01-01-2022', end_date = '01-01-2023', flatten = False, validate = False):
+    '''
+    Prepares data for training and evaluating.
+
+    Args:
+
+        ticker: Ticker to get data for.
+
+        column: Column from HLOCV to work with.
+
+        length: Length of arrays, length-1 values are for fitting, 1 value is for evaluating.
+
+        step: Step to cut data using sliding window.
+
+        start_date: Date to start cutting data from.
+
+        split_date: Date to split into train/test.
+
+        end_date: Date to end cutting data.
+
+        flatten: Shape format:  (cuts, length-1) or (cuts, length-1, 1).
+
+        validate: To make validation split or not.
+
+    Returns:
+        x_train, x_test, y_train, y_test, scaler: train and test data with scaler to work with.
+
+    Example:
+    >>> get_data('AAPL', 'close', 10)
+    [[0.122, 0.12, 0.125, ..], ..]
+    [0.12, ..]
+    [[0.132, 0.13, 0.135, ..], ..]
+    [0.13, ..]
+    Scaler()
+    '''
+    data = pd.read_parquet(f'{PACKAGEDIR}/data.parquet.gz')
+    data = data[(data.dateTime >= start_date) & (data.ticker == ticker)]
+
+    train_data = data[(data.dateTime < split_date)][column].values.reshape(-1, 1)
+    test_data =  data[(data.dateTime >= split_date) & (data.dateTime < end_date)][column].values.reshape(-1, 1)
+
+    train_set = [train_data[j:j+length,0] for j in range(0, len(train_data)-length, step)]
+    test_set =  [test_data[j:j+length,0] for j in range(0, len(test_data)-length, step)]
+
+    scaler = Scaler().fit(train_set)
+    scaled_train_set = scaler.scale(train_set)
+    scaled_test_set = scaler.scale(test_set)
+
+    scaled_x_train, scaled_x_test = scaled_train_set[:,:length-1], scaled_test_set[:,:length-1]
+    scaled_y_train, scaled_y_test = scaled_train_set[:,length-1],  scaled_test_set[:,length-1]
+
+    if not flatten:
+        scaled_x_train = np.reshape(scaled_x_train, (scaled_x_train.shape[0], length - 1,1))
+        scaled_x_test = np.reshape(scaled_x_test, (scaled_x_test.shape[0], length - 1,1))
+
+    if validate:
+        val_data = data[(data.dateTime >= end_date) & (data.ticker == ticker)][column].values.reshape(-1, 1)
+        val_set = [val_data[j:j+length,0] for j in range(0, len(val_data)-length, step)]
+        scaled_val_set = scaler.scale(val_set)
+        scaled_x_val, scaled_y_val = scaled_val_set[:,:length-1], scaled_val_set[:,length-1]
+        return scaled_x_train, scaled_x_test, scaled_x_val, scaled_y_train, scaled_y_test, scaled_y_val, scaler
+    else:
+        return scaled_x_train, scaled_x_test, scaled_y_train, scaled_y_test, scaler
+
+def update_data(tickers = []):
+    '''
+    Updates stored data for defined tickers.
+
+    Args:
+
+        tickers (list): Tickers list to update data for.
+
+    Example:
+    >>> get_data(['AMZN', 'TSLA', 'NVDA']])
+    Info about 3 tickers successfully uploaded.
+    '''
+    all_tickers_df = pd.read_parquet(f'{PACKAGEDIR}/data.parquet.gz')
+    for i in tickers:
+        headers = {"Accept":"text/html", "Accept-Language":"en-US", "Referer":"https://www.nasdaq.com/", "User-Agent":"Chrome/64.0.3282.119"}
+        resp = rq.get(f'https://api.nasdaq.com/api/quote/{i}/chart?assetclass=stocks&fromdate=2023-04-29&todate={datetime.datetime.now().strftime("%Y-%m-%d")}', headers=headers, verify=True)
+        if resp.status_code == 200:
+            try:
+                smth = json.loads(re.search('\[.*\]', resp.text).group())
+                cur_tick_data = pd.DataFrame([smth[k]['z'] for k in range(len(smth))])
+                cur_tick_data['ticker'] = i
+                for col_name in ['high','low','open','close','volume','value']:
+                    cur_tick_data[col_name] = pd.to_numeric(cur_tick_data[col_name].str.replace(',',''))
+                cur_tick_data['dateTime'] = pd.to_datetime(cur_tick_data['dateTime'])
+                all_tickers_df = pd.concat([all_tickers_df, cur_tick_data])
+            except KeyError:
+                pass
+        else:
+            print(f'ERROR: smth is wrong with {i}')
+    all_tickers_df.to_parquet(f'{PACKAGEDIR}/data.parquet.gz', compression='gzip')
+    print(f'Info about {len(tickers)} tickers successfully uploaded.')
```

### Comparing `ftsf-0.0.2/ftsf/scaler.py` & `ftsf-0.0.2.1/ftsf/scaler.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-'''This submodule contains scaler class.'''
-
-import numpy as np
-
-
-class Scaler:
-    '''
-    Instance of default minmax scaler adapted for price scaling.
-
-    Attributes:
-
-        minimum: Minimum value seen during fit.
-
-        maximum: Maximum value seen during fit.
-
-    '''
-
-    __minimum = 0
-    __maximum = 0
-
-    def __init__(self, params = None):
-        '''
-        Initializes instance of scaler.
-
-        Args:
-
-            params: List of min and max values.
-
-        Example:
-        >>> Scaler([0.2, 2.3])
-        '''
-        if params is not None:
-            self.__minimum, self.__maximum = params[0], params[1]
-
-    def fit(self, array):
-        '''
-        Fits scaler on array.
-
-        Args:
-
-            array: Array to fit scaler on.
-
-        Returns:
-
-            Scaler fitted on array.
-
-        Example:
-        >>> scaler.fit([[0.2, 2.3], [0.3,0.2], ..])
-        '''
-        self.__minimum = np.min(array)
-        self.__maximum = np.max(array)
-        return self
-
-    def scale(self, array) -> np.array:
-        '''
-        Scales array using min and max found on fit.
-
-        Args:
-
-            array: Array to scale.
-
-        Returns:
-
-            Scaled array.
-
-        Example:
-        >>> scaler.scale([[2, 3], [0.3,0.2], ...])
-        [[0.6666, 1], [0.11, 0.066], ..]
-        '''
-        return (array-self.__minimum)/(self.__maximum - self.__minimum)
-
-    def unscale(self, array) -> np.array:
-        '''
-        Scales back array using min and max found on fit.
-
-        Args:
-
-            array: Array to scale back.
-
-        Returns:
-
-            Scaled back array.
-
-        Example:
-        >>> scaler.scale([[0.6666, 1], [0.11, 0.066], ..])
-        [[2, 3], [0.3,0.2], ..]
-        '''
-        return array*(self.__maximum - self.__minimum) + self.__minimum
-
-    def params(self) -> list:
-        '''
-        Shows min and max values, used to scale.
-
-        Returns:
-
-            min and max parameters of scaler.
-
-        Example:
-        >>> scaler.params()
-        (2, 29)
-        '''
-        return self.__minimum, self.__maximum
+'''This submodule contains scaler class.'''
+
+import numpy as np
+
+
+class Scaler:
+    '''
+    Instance of default minmax scaler adapted for price scaling.
+
+    Attributes:
+
+        minimum: Minimum value seen during fit.
+
+        maximum: Maximum value seen during fit.
+
+    '''
+
+    __minimum = 0
+    __maximum = 0
+
+    def __init__(self, params = None):
+        '''
+        Initializes instance of scaler.
+
+        Args:
+
+            params: List of min and max values.
+
+        Example:
+        >>> Scaler([0.2, 2.3])
+        '''
+        if params is not None:
+            self.__minimum, self.__maximum = params[0], params[1]
+
+    def fit(self, array):
+        '''
+        Fits scaler on array.
+
+        Args:
+
+            array: Array to fit scaler on.
+
+        Returns:
+
+            Scaler fitted on array.
+
+        Example:
+        >>> scaler.fit([[0.2, 2.3], [0.3,0.2], ..])
+        '''
+        self.__minimum = np.min(array)
+        self.__maximum = np.max(array)
+        return self
+
+    def scale(self, array) -> np.array:
+        '''
+        Scales array using min and max found on fit.
+
+        Args:
+
+            array: Array to scale.
+
+        Returns:
+
+            Scaled array.
+
+        Example:
+        >>> scaler.scale([[2, 3], [0.3,0.2], ...])
+        [[0.6666, 1], [0.11, 0.066], ..]
+        '''
+        return (array-self.__minimum)/(self.__maximum - self.__minimum)
+
+    def unscale(self, array) -> np.array:
+        '''
+        Scales back array using min and max found on fit.
+
+        Args:
+
+            array: Array to scale back.
+
+        Returns:
+
+            Scaled back array.
+
+        Example:
+        >>> scaler.scale([[0.6666, 1], [0.11, 0.066], ..])
+        [[2, 3], [0.3,0.2], ..]
+        '''
+        return array*(self.__maximum - self.__minimum) + self.__minimum
+
+    def params(self) -> list:
+        '''
+        Shows min and max values, used to scale.
+
+        Returns:
+
+            min and max parameters of scaler.
+
+        Example:
+        >>> scaler.params()
+        (2, 29)
+        '''
+        return self.__minimum, self.__maximum
```

### Comparing `ftsf-0.0.2/ftsf/tests/test_evaluation.py` & `ftsf-0.0.2.1/ftsf/tests/test_evaluation.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-import sys
-
-sys.path.insert(0, '../ftsf')
-
-from ftsf import evaluation as ev
-from ftsf import preprocessing as pr
-
-
-def test_eval_ml_len():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert len(ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)) == 8
-
-def test_eval_ar_len():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert len(ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)) == 2
-
-def test_eval_nn_len():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
-    assert len(ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512)) == 16
-
-def test_eval_all_len():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
-    assert len(ev.evaluate_all_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='list')) == 26
-
-
-def test_eval_ml_keys():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert list(ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
-
-def test_eval_ar_keys():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert list(ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
-
-def test_eval_nn_keys():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
-    assert list(ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512)[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
-
-def test_eval_all_keys():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
-    assert list(ev.evaluate_all_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='list')[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
-
-
-def test_eval_ml_df():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').shape == (8,6)
-
-def test_eval_ar_df():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').shape == (2,6)
-
-def test_eval_nn_df():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
-    assert ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='df').shape == (16,6)
-
-def test_eval_all_df():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
-    assert ev.evaluate_all_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='df').shape == (26,6)
-
-
-def test_eval_ml_df_cols():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').columns.to_list() == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
-
-def test_eval_ar_df_cols():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
-    assert ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').columns.to_list() == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
-
-def test_eval_nn_df_cols():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
-    assert ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='df').columns.to_list() == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
-
-def test_eval_all_df_cols():
-    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+import sys
+
+sys.path.insert(0, '../ftsf')
+
+from ftsf import evaluation as ev
+from ftsf import preprocessing as pr
+
+
+def test_eval_ml_len():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert len(ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)) == 8
+
+def test_eval_ar_len():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert len(ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)) == 2
+
+def test_eval_nn_len():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+    assert len(ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512)) == 16
+
+def test_eval_all_len():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+    assert len(ev.evaluate_all_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='list')) == 26
+
+
+def test_eval_ml_keys():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert list(ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
+
+def test_eval_ar_keys():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert list(ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler)[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
+
+def test_eval_nn_keys():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+    assert list(ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512)[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
+
+def test_eval_all_keys():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+    assert list(ev.evaluate_all_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='list')[0].keys()) == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
+
+
+def test_eval_ml_df():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').shape == (8,6)
+
+def test_eval_ar_df():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').shape == (2,6)
+
+def test_eval_nn_df():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+    assert ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='df').shape == (16,6)
+
+def test_eval_all_df():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+    assert ev.evaluate_all_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='df').shape == (26,6)
+
+
+def test_eval_ml_df_cols():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert ev.evaluate_ml_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').columns.to_list() == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
+
+def test_eval_ar_df_cols():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=5)
+    assert ev.evaluate_ar_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, out_type='df').columns.to_list() == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
+
+def test_eval_nn_df_cols():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
+    assert ev.evaluate_nn_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='df').columns.to_list() == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
+
+def test_eval_all_df_cols():
+    test_xtr, test_xt, test_ytr, test_yt, test_scaler = pr.get_data(start_date='11-11-2021', end_date='03-03-2022', length=7)
     assert ev.evaluate_all_models(test_xtr, test_xt, test_ytr, test_yt, test_scaler, epochs = 2, batch_size = 512, out_type='df').columns.to_list() == ['time', 'mse', 'mae', 'mape', 'r2', 'model']
```

