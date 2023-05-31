# Comparing `tmp/ftsf-0.0.1.4.tar.gz` & `tmp/ftsf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftsf-0.0.1.4.tar", last modified: Sat May 27 02:33:04 2023, max compression
+gzip compressed data, was "ftsf-0.0.2.tar", last modified: Wed May 31 21:25:54 2023, max compression
```

## Comparing `ftsf-0.0.1.4.tar` & `ftsf-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.814004 ftsf-0.0.1.4/
-drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.794993 ftsf-0.0.1.4/FTSF.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-27 02:33:04.000000 ftsf-0.0.1.4/FTSF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1100 2023-05-26 02:11:38.000000 ftsf-0.0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-05-27 02:33:04.812494 ftsf-0.0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-05-26 23:32:26.000000 ftsf-0.0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.807492 ftsf-0.0.1.4/ftsf/
--rw-rw-rw-   0        0        0        0 2023-05-25 02:03:02.000000 ftsf-0.0.1.4/ftsf/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-05-27 01:28:45.000000 ftsf-0.0.1.4/ftsf/backtest.py
--rw-rw-rw-   0        0        0     7484 2023-05-27 02:13:28.000000 ftsf-0.0.1.4/ftsf/evaluation.py
--rw-rw-rw-   0        0        0     7962 2023-05-27 02:00:08.000000 ftsf-0.0.1.4/ftsf/model.py
--rw-rw-rw-   0        0        0     4486 2023-05-26 04:29:45.000000 ftsf-0.0.1.4/ftsf/preprocessing.py
--rw-rw-rw-   0        0        0     1646 2023-05-27 01:35:41.000000 ftsf-0.0.1.4/ftsf/scaler.py
-drwxrwxrwx   0        0        0        0 2023-05-27 02:33:04.810508 ftsf-0.0.1.4/ftsf/tests/
--rw-rw-rw-   0        0        0      629 2023-05-25 02:40:23.000000 ftsf-0.0.1.4/ftsf/tests/test_scaler.py
--rw-rw-rw-   0        0        0     5321 2023-05-27 02:11:47.000000 ftsf-0.0.1.4/ftsf/utils.py
--rw-rw-rw-   0        0        0      812 2023-05-27 02:32:39.000000 ftsf-0.0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 02:33:04.815520 ftsf-0.0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.684793 ftsf-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.657826 ftsf-0.0.2/FTSF.egg-info/
+-rw-rw-rw-   0        0        0     1185 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-31 21:25:54.000000 ftsf-0.0.2/FTSF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1100 2023-05-26 02:11:38.000000 ftsf-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1185 2023-05-31 21:25:54.683795 ftsf-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-05-29 03:05:15.000000 ftsf-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.675587 ftsf-0.0.2/ftsf/
+-rw-rw-rw-   0        0        0      587 2023-05-31 21:20:54.000000 ftsf-0.0.2/ftsf/__init__.py
+-rw-rw-rw-   0        0        0     3533 2023-05-31 21:20:02.000000 ftsf-0.0.2/ftsf/backtest.py
+-rw-rw-rw-   0        0        0     7399 2023-05-31 21:22:08.000000 ftsf-0.0.2/ftsf/evaluation.py
+-rw-rw-rw-   0        0        0     8687 2023-05-31 21:18:58.000000 ftsf-0.0.2/ftsf/model.py
+-rw-rw-rw-   0        0        0     4601 2023-05-31 21:15:23.000000 ftsf-0.0.2/ftsf/preprocessing.py
+-rw-rw-rw-   0        0        0     2178 2023-05-31 21:19:24.000000 ftsf-0.0.2/ftsf/scaler.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:25:54.681781 ftsf-0.0.2/ftsf/tests/
+-rw-rw-rw-   0        0        0     5000 2023-05-31 21:02:22.000000 ftsf-0.0.2/ftsf/tests/test_evaluation.py
+-rw-rw-rw-   0        0        0      643 2023-05-31 21:02:22.000000 ftsf-0.0.2/ftsf/tests/test_preprocessing.py
+-rw-rw-rw-   0        0        0      440 2023-05-31 21:02:22.000000 ftsf-0.0.2/ftsf/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     6197 2023-05-31 21:18:24.000000 ftsf-0.0.2/ftsf/utils.py
+-rw-rw-rw-   0        0        0      810 2023-05-31 21:25:28.000000 ftsf-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 21:25:54.684793 ftsf-0.0.2/setup.cfg
```

### Comparing `ftsf-0.0.1.4/FTSF.egg-info/PKG-INFO` & `ftsf-0.0.2/FTSF.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftsf
-Version: 0.0.1.4
+Version: 0.0.2
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -23,7 +23,8 @@
 The usage of package is simple:
 > from ftsf.model import Model  
 > from ftsf.preprocessing import get_data  
 > x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
 > model = Model('LSTM x2', lag = 15)  
 > model.fit(x_train, y_train)
 > model.evaluate(x_test, y_test, scaler)  
+{'mse' : 0.679, 'mae' : 0.8291, 'mape' : 0.00783, 'r2' : 0.98778}
```

### Comparing `ftsf-0.0.1.4/LICENSE` & `ftsf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.1.4/PKG-INFO` & `ftsf-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftsf
-Version: 0.0.1.4
+Version: 0.0.2
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -23,7 +23,8 @@
 The usage of package is simple:
 > from ftsf.model import Model  
 > from ftsf.preprocessing import get_data  
 > x_train, x_test, y_train, y_test, scaler = get_data('AAPL', length=15)  
 > model = Model('LSTM x2', lag = 15)  
 > model.fit(x_train, y_train)
 > model.evaluate(x_test, y_test, scaler)  
+{'mse' : 0.679, 'mae' : 0.8291, 'mape' : 0.00783, 'r2' : 0.98778}
```

### Comparing `ftsf-0.0.1.4/ftsf/backtest.py` & `ftsf-0.0.2/ftsf/backtest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from .scaler import Scaler
-from .model import Model
+'''This submodule contains instrument to test trading strategy based on model on historical data.'''
+
 import numpy as np
 
+from .model import Model
+from .scaler import Scaler
+
+
 class BackTesting:
     '''
     Models trading strategy and backtests it.
 
     Attributes:
-        
+
         initial_money: Initial amount of money to work with.
-        
+
         money: Current amount of money.
-        
+
         stocks: Current amount of stocks.
 
         model: Instance of model used for forecasting.
     '''
     __initial_money = 0
     __money = 0
     __stocks = 0
@@ -45,34 +49,37 @@
         self.__stocks += volume
 
     def __predict_steps(self, current_state : list, depth = 15, steps_forward = 1) -> float:
         '''
         Internal method to forecast for a few steps forward.
         '''
         current_state = current_state.copy()
-        cs = Scaler().fit(current_state)
+        scaler = Scaler().fit(current_state)
         for i in range(steps_forward):
-            current_state += self.__model.predict(cs.scale(np.array(current_state[-depth:]).reshape((1,depth,1))), cs).reshape(-1).tolist()
-        return current_state[-1]  
+            current_state += self.__model.predict(scaler.scale(np.array(current_state[-depth:]).reshape((1,depth,1))), scaler).reshape(-1).tolist()
+        return current_state[-1]
 
     def test(self, states, depth = 15, steps_forward = 5):
         '''
-        Implement strategy based on model forecasts, then backtests it.
+        Implements strategy based on model forecasts, then backtests it.
 
         Args:
-            states (list): Array of historic values.
-            depth (int): Number of values to forecast on.
-            steps_forward (int): Number of steps to forecast.
+
+            states: Array of historic values.
+
+            depth: Number of values to forecast on.
+
+            steps_forward: Number of steps to forecast.
 
         Example:
         >>> str = Backtesting(model, 10e4)
         >>> str.test(states, 15, 1)
         Successfully tested: 12532
         +2532 or 25.32% in 50 days.
-        2 trades, avg profit 1266 $ per trade. 
+        2 trades, avg profit 1266 $ per trade.
         '''
         self.__money = self.__initial_money
         trades_no = 0
         for i in range(len(states)-depth):
             current_state = states[i:i+depth]
             if (self.__predict_steps(current_state, depth, steps_forward) > current_state[-1]):
                 if self.__money > current_state[-1]:
@@ -85,8 +92,8 @@
                     print(f'Sold {self.__stocks} stocks.')
                     print(f'Delta = {current_state[-1] - bought}/stock')
                     self.__sell(current_state[-1])
         self.__sell(current_state[-1])
         print(f'Successfully tested: \n{self.__money }$')
         print(f'{"+" if self.__money - self.__initial_money > 0 else ""}{round(self.__money - self.__initial_money)}$ or \
         {"+" if self.__money - self.__initial_money>0 else ""}{round((self.__money - self.__initial_money)/self.__initial_money*100)}% in {len(states)} days.')
-        print(f'{trades_no}, avg profit {(self.__money - self.__initial_money)/trades_no}$ per trade.')
+        print(f'{trades_no}, avg profit {(self.__money - self.__initial_money)/trades_no}$ per trade.')
```

### Comparing `ftsf-0.0.1.4/ftsf/evaluation.py` & `ftsf-0.0.2/ftsf/evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,66 @@
-import pandas as pd, time
-import plotly.express as px
-from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score,  mean_absolute_percentage_error
+'''This submodule contains methods to evaluate models.'''
 
+import time
 import warnings
+
+import pandas as pd
+from sklearn.metrics import (mean_absolute_error,
+                             mean_absolute_percentage_error,
+                             mean_squared_error, r2_score)
+
 warnings.filterwarnings("ignore")
 
 from .model import Model
 from .utils import get_models
 
+
 def evaluate_ml_models(x_train, x_test, y_train, y_test, scaler, out_type = 'list'):
     '''
     Evaluates machine learning models on data.
 
     Args:
 
         x_train: Input values to fit model.
-        
+
         x_test: Input values to evaluate model.
-        
+
         y_train: Target values to fit model.
-        
+
         y_test: Target values to fit model.
-        
+
         scaler: Scaler to scale/unscale values during evaluation.
-        
-        out_type: Format to return data. 
-    
+
+        out_type: Format to return data.
+
     Returns:
-        
+
         list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
-        
+
         or pd.DataFrame: dataframe with the same data.
 
     Example:
     >>> evaluate_ml_models(x_train, x_test, y_train, y_test, scaler)
     [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LR'}, ...]
     '''
     statistics = []
     for i in get_models('ml'):
         current_model = Model(i)
         start_time = time.time()
         current_model.fit(x_train, y_train)
         utilized = time.time() - start_time
         pred = current_model.predict(x_test, scaler)
         true = scaler.unscale(y_test)
-        statistics.append({ 'time': utilized, 
+        statistics.append({ 'time': utilized,
                     'mse': mean_squared_error(true, pred),
                     'mae': mean_absolute_error(true, pred),
                     'mape': mean_absolute_percentage_error(true, pred),
                     'r2':  r2_score(true, pred),
                     'model': i})
-        
+
     if out_type == 'df':
         return pd.DataFrame(statistics).sort_values(by='mape')
     elif out_type == 'list':
         return statistics
 
 def evaluate_ar_models(x_train, x_test, y_train, y_test, scaler, out_type = 'list'):
     '''
@@ -68,16 +74,16 @@
 
         y_train: Target values to fit model.
 
         y_test: Target values to fit model.
 
         scaler: Scaler to scale/unscale values during evaluation.
 
-        out_type: Format to return data. 
-    
+        out_type: Format to return data.
+
     Returns:
 
         list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
 
         or pd.DataFrame : dataframe with the same data.
 
     Example:
@@ -85,60 +91,60 @@
     [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'ARMA(2,1)'}, ...]
     '''
     statistics = []
     for i in get_models('ar'):
         pred = []
         for j in range(len(y_test)):
             start_time = time.time()
-            current_model = Model(i, data=x_test[j])            
+            current_model = Model(i).fit(x_test[j], y_test[j])
             utilized = time.time() - start_time
             pred.append(current_model.predict(x_test[j], scaler))
         true = scaler.unscale(y_test)
-        statistics.append({ 'time': utilized, 
+        statistics.append({ 'time': utilized,
                     'mse': mean_squared_error(true, pred),
                     'mae': mean_absolute_error(true, pred),
                     'mape': mean_absolute_percentage_error(true, pred),
                     'r2':  r2_score(true, pred),
                     'model': i})
-        
+
     if out_type == 'df':
         return pd.DataFrame(statistics).sort_values(by='mape')
     elif out_type == 'list':
-        return statistics  
+        return statistics
 
 def evaluate_nn_models(x_train, x_test, y_train, y_test, scaler, optimizer = 'nadam', loss = 'mse', epochs = 10, batch_size = 256, out_type = 'list'):
     '''
     Evaluates neural network based models on data.
 
     Args:
 
         x_train: Input values to fit model.
-    
+
         x_test: Input values to evaluate model.
-        
+
         y_train: Target values to fit model.
-        
+
         y_test: Target values to fit model.
-        
+
         scaler: Scaler to scale/unscale values during evaluation.
-        
+
         optimizer: tf.Keras optimizer name (optional: only for neural networks).
-        
+
         loss: tf.Keras loss name (optional: only for neural networks).
-        
+
         epochs: Number of epochs during fitting (optional: only for neural networks).
-        
+
         batch_size: Size of batch during fitting (optional: only for neural networks).
-        
-        out_type: Format to return data. 
-    
+
+        out_type: Format to return data.
+
     Returns:
-        
+
         list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
-        
+
         or pd.DataFrame: dataframe with the same data.
 
     Example:
     >>> evaluate_nn_models(x_train, x_test, y_train, y_test, scaler)
     [{'time' : 0.12, 'mse' : 0.04, 'mae' : 0.2, 'mape' : 0.01, 'model' : 'LSTM x1'}, ...]
     '''
 
@@ -146,36 +152,36 @@
     for i in get_models('nn'):
         current_model = Model(i, lag = x_train.shape[1]+1, optimizer=optimizer, loss=loss)
         start_time = time.time()
         current_model.fit(x_train, y_train, epochs, batch_size)
         utilized = time.time() - start_time
         pred = current_model.predict(x_test, scaler)
         true = scaler.unscale(y_test)
-        statistics.append({ 'time': utilized, 
+        statistics.append({ 'time': utilized,
                     'mse': mean_squared_error(true, pred),
                     'mae': mean_absolute_error(true, pred),
                     'mape': mean_absolute_percentage_error(true, pred),
                     'r2':  r2_score(true, pred),
                     'model': i})
-    
+
     if out_type == 'df':
         return pd.DataFrame(statistics).sort_values(by='mape')
     elif out_type == 'list':
         return statistics
 
 
 def evaluate_all_models(x_train, x_test, y_train, y_test, scaler, optimizer = 'nadam', loss = 'mse', epochs = 10, batch_size = 256, out_type = 'df'):
     '''
     Evaluates all models on data.
 
     Args:
 
-        x_train: Input values to fit model.  
+        x_train: Input values to fit model.
 
-        x_test: Input values to evaluate model.  
+        x_test: Input values to evaluate model.
 
         y_train: Target values to fit model.
 
         y_test: Target values to fit model.
 
         scaler: Scaler to scale/unscale values during evaluation.
 
@@ -183,16 +189,16 @@
 
         loss: tf.Keras loss name (optional: only for neural networks).
 
         epochs: Number of epochs during fitting (optional: only for neural networks).
 
         batch_size: Size of batch during fitting (optional: only for neural networks).
 
-        out_type: Format to return data. 
-    
+        out_type: Format to return data.
+
     Returns:
 
         list: List of dictionaries with time, MSE, MAE, MAPE, R2 values and model name for each model.
 
         or pd.DataFrame: dataframe with the same data.
 
     Example:
@@ -203,8 +209,8 @@
     statistics = evaluate_ml_models(x_train, x_test, y_train, y_test, scaler)
     statistics += evaluate_ar_models(x_train, x_test, y_train, y_test, scaler)
     statistics += evaluate_nn_models(x_train, x_test, y_train, y_test, scaler, optimizer, loss, epochs, batch_size)
 
     if out_type == 'df':
         return pd.DataFrame(statistics).sort_values(by='mape')
     elif out_type == 'list':
-        return statistics
+        return statistics
```

### Comparing `ftsf-0.0.1.4/ftsf/model.py` & `ftsf-0.0.2/ftsf/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# ML methods
+'''This submodule contains generic model class.'''
+
+import numpy as np
+from catboost import CatBoostRegressor
+from joblib import dump, load
+from sklearn.ensemble import GradientBoostingRegressor, RandomForestRegressor
 from sklearn.linear_model import LinearRegression
-from sklearn.ensemble import RandomForestRegressor, GradientBoostingRegressor
-from sklearn.tree import DecisionTreeRegressor
+from sklearn.metrics import (mean_absolute_error,
+                             mean_absolute_percentage_error,
+                             mean_squared_error, r2_score)
 from sklearn.svm import SVR
-from catboost import CatBoostRegressor
-from xgboost import XGBRegressor, XGBRFRegressor
-
-# Autoregressive methods
+from sklearn.tree import DecisionTreeRegressor
 from statsmodels.tsa.arima.model import ARIMA
-
-# NN methods
 from tensorflow.keras import Sequential
+from tensorflow.keras.models import load_model, save_model
+from xgboost import XGBRegressor, XGBRFRegressor
 
-# Metrics
-from sklearn.metrics import mean_squared_error, mean_absolute_error, mean_absolute_percentage_error, r2_score
-import numpy as np
+from .utils import get_topologies, parse_name
 
-from .utils import get_topologies
 
 class Model:
     '''
     Generic ML/AR/NN based model with unified interface.
 
 
     Models:
@@ -46,69 +46,69 @@
     __backend = ''
     __name = ''
     __model = None
 
     def __init__(self, name, lag = 15, optimizer = 'nadam', loss = 'mse'):
         '''
         Initializes the instance of model based on defined type.
-        
+
         Args:
 
             name: Defines exact model.
 
             lag: An integer indicating number of values to base prediction on.
 
             data: Data to use on autoregressive model fit.
 
             optimizer: Optimizer to use on compiling neural network based models.
 
             loss: Loss function to use on compiling neural network based models.
-        
+
         Example:
         >>> Model('LSTM x2', 15)
         '''
         models = {'ml': ['LR', 'DTR', 'RFR', 'GBR', 'SVR', 'CBR', 'XGBR', 'XGBRFR'],
-                  'ar': ['ARMA(2,1)', 'ARIMA(2,1,1)'], 
+                  'ar': ['ARMA(2,1)', 'ARIMA(2,1,1)'],
                   'nn': ['CNN + LSTM', 'LSTM x3', 'LSTM x2', 'LSTM x1', 'CNN + GRU', 'GRU x3', 'GRU x2', 'GRU x1', \
                          'CNN + SimpleRNN', 'SimpleRNN x3', 'SimpleRNN x2', 'SimpleRNN x1', 'CNN', 'MLP(3)', 'MLP(2)', 'MLP(1)']}
-        
+
         self.__type = [key for key, value in models.items() if name in value][0]
         self.__name = name
 
         if self.__type == 'ml':
             if name == 'CBR':
                 self.__backend = 'Catboost'
             elif name[:2] == 'XG':
                 self.__backend = 'XGBoost'
             else:
                 self.__backend = 'Scikit-learn'
-    
+
             self.__model = {  'LR' :  LinearRegression(),
                             'DTR' : DecisionTreeRegressor(min_samples_leaf=5),
                             'RFR' : RandomForestRegressor(),
                             'GBR' : GradientBoostingRegressor(),
                             'SVR' : SVR(kernel='linear', epsilon=1e-3),
                             'CBR' : CatBoostRegressor(loss_function='MAPE'),
                             'XGBR': XGBRegressor(objective='reg:squarederror'),
                             'XGBRFR': XGBRFRegressor(objective = 'reg:squarederror')}[name]
-        
+
         elif self.__type == 'ar':
             self.__backend = 'Statsmodels'
-        
+
         elif self.__type == 'nn':
             self.__backend = 'TensorFlow.Keras'
             self.__model = Sequential(get_topologies(lag)[name])
             self.__model.compile(optimizer = optimizer, loss = loss,  metrics = ['mse', 'mae', 'mape'])
 
     def fit(self, x_train, y_train, epochs = 25, batch_size = 32):
         '''
         Fits model using x_train and y_train.
 
         Note that autoregressive models differ from other and can be fitted only on one sample of data.
-        
+
         Args:
 
             x_train: Array with previous price values.
 
             y_train: Array with target price values.
 
             epochs: Number of epochs in case of using neural network.
@@ -121,34 +121,26 @@
 
         if self.__type == 'nn':
             x_train = x_train.reshape((x_train.shape[0], x_train.shape[1], 1))
             self.__model.fit(x_train, y_train, epochs = epochs, batch_size = batch_size, verbose = 0)
         elif self.__name == 'CBR':
             x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
             self.__model.fit(x_train, y_train, silent = True)
-        elif self.__backend != 'statsmodels':
+        elif self.__backend != 'Statsmodels':
             x_train = x_train.reshape((x_train.shape[0], x_train.shape[1]))
             self.__model.fit(x_train, y_train)
         elif self.__backend == 'Statsmodels':
-            if self.__name.find('I') != -1:
-                p = float(self.__name[self.__name.find('(') + 1 : self.__name.find(',')])
-                d = float(self.__name[self.__name.find(',') + 1 : self.__name.find(',', self.__name.find(',') + 1)])
-                q = float(self.__name[self.__name.find(',', self.__name.find(',') + 1) + 1 : self.__name.find(')')])
-            else:
-                p = float(self.__name[self.__name.find('(') + 1 : self.__name.find(',')])
-                d = 0
-                q = float(self.__name[self.__name.find(',') + 1 : self.__name.find(')')])
-            self.__model = ARIMA(x_train, order = (p, d, q), enforce_stationarity = False).fit()
-        
+            self.__model = ARIMA(x_train, order = parse_name(self.__name), enforce_stationarity = False)
+
         return self
 
     def predict(self, x_test, scaler):
         '''
         Predicts and scales values using x_test and scaler.
-        
+
         Args:
 
             x_test - previous price values;
 
             scaler - scaler will be used to scale values back.
 
         Returns:
@@ -158,26 +150,26 @@
         Example:
         >>> model.predict(x_test, scaler)
         [123, 124, 123, 128]
         '''
 
         if self.__type == 'ar':
             x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
-            return scaler.unscale(self.__model.forecast(steps = 1)[0])
+            return scaler.unscale(self.__model.fit().forecast(steps = 1)[0])
         elif self.__type == 'nn':
             x_test = x_test.reshape((x_test.shape[0], x_test.shape[1], 1))
             return scaler.unscale(self.__model.predict(x_test, verbose = 0).reshape(-1))
         else:
             x_test = x_test.reshape((x_test.shape[0], x_test.shape[1]))
             return scaler.unscale(self.__model.predict(x_test))
 
     def evaluate(self, x_test, y_test, scaler):
         '''
         Predicts and scales values using x_test and scaler, then measures MSE, MAE, MAPE and R2.
-        
+
         Args:
 
             x_test: Array with previous price values.
 
             y_test: Array with target price values.
 
             scaler: Scaler to be used to scale values back.
@@ -199,15 +191,55 @@
                 'r2':  r2_score(np.array(true), np.array(prediction))}
 
     def summary(self):
         '''
         Shows short summary about model, its type and backend.
 
         Returns:
+
             String with short model description.
-        
+
         Example:
         >>> model.summary()
         ML model XGBRegressor, backend is based on XGBoost.
         '''
-        
-        print(f'{self.__type.upper()} model {self.__name}, backend is based on {self.__backend}.')
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

### Comparing `ftsf-0.0.1.4/ftsf/preprocessing.py` & `ftsf-0.0.2/ftsf/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,47 @@
-import pandas as pd, re, json, requests as rq, numpy as np, datetime
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
 
 from .scaler import Scaler
 
-from pathlib import Path
 PACKAGEDIR = Path(__file__).parent.absolute()
 
 
 def get_data(ticker = 'AAPL', column = 'close', length = 15, step = 1, start_date = '01-01-2013', split_date = '01-01-2022', end_date = '01-01-2023', flatten = False, validate = False):
     '''
     Prepares data for training and evaluating.
 
     Args:
-    ticker (str): Ticker to get data for.
-    column (str): Column from HLOCV to work with.
-    length (int): Length of arrays, length-1 values are for fitting, 1 value is for evaluating.
-    step (int): Step to cut data using sliding window.
-    start_date (str): Date to start cutting data from.
-    split_date (str): Date to split into train/test.
-    end_date (str): Date to end cutting data.
-    flatten (bool): Shape format:  (cuts, length-1) or (cuts, length-1, 1).
-    validate (bool): To make validation split or not.
-    
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
     Returns:
         x_train, x_test, y_train, y_test, scaler: train and test data with scaler to work with.
 
     Example:
     >>> get_data('AAPL', 'close', 10)
     [[0.122, 0.12, 0.125, ..], ..]
     [0.12, ..]
@@ -49,36 +66,37 @@
     scaled_y_train, scaled_y_test = scaled_train_set[:,length-1],  scaled_test_set[:,length-1]
 
     if not flatten:
         scaled_x_train = np.reshape(scaled_x_train, (scaled_x_train.shape[0], length - 1,1))
         scaled_x_test = np.reshape(scaled_x_test, (scaled_x_test.shape[0], length - 1,1))
 
     if validate:
-        val_data = data[(data.date >= end_date) & (data.ticker == ticker)]['price'].values.reshape(-1, 1)
+        val_data = data[(data.dateTime >= end_date) & (data.ticker == ticker)][column].values.reshape(-1, 1)
         val_set = [val_data[j:j+length,0] for j in range(0, len(val_data)-length, step)]
         scaled_val_set = scaler.scale(val_set)
         scaled_x_val, scaled_y_val = scaled_val_set[:,:length-1], scaled_val_set[:,length-1]
         return scaled_x_train, scaled_x_test, scaled_x_val, scaled_y_train, scaled_y_test, scaled_y_val, scaler
     else:
         return scaled_x_train, scaled_x_test, scaled_y_train, scaled_y_test, scaler
 
 def update_data(tickers = []):
     '''
     Updates stored data for defined tickers.
 
     Args:
-    tickers (list): Tickers list to update data for.
+
+        tickers (list): Tickers list to update data for.
 
     Example:
     >>> get_data(['AMZN', 'TSLA', 'NVDA']])
     Info about 3 tickers successfully uploaded.
     '''
     all_tickers_df = pd.read_parquet(f'{PACKAGEDIR}/data.parquet.gz')
     for i in tickers:
-        headers = {"Accept":"text/html", "Accept-Language":"en-US", "Referer":"https://www.nasdaq.com/", "User-Agent":"Chrome/64.0.3282.119"} 
+        headers = {"Accept":"text/html", "Accept-Language":"en-US", "Referer":"https://www.nasdaq.com/", "User-Agent":"Chrome/64.0.3282.119"}
         resp = rq.get(f'https://api.nasdaq.com/api/quote/{i}/chart?assetclass=stocks&fromdate=2023-04-29&todate={datetime.datetime.now().strftime("%Y-%m-%d")}', headers=headers, verify=True)
         if resp.status_code == 200:
             try:
                 smth = json.loads(re.search('\[.*\]', resp.text).group())
                 cur_tick_data = pd.DataFrame([smth[k]['z'] for k in range(len(smth))])
                 cur_tick_data['ticker'] = i
                 for col_name in ['high','low','open','close','volume','value']:
@@ -86,8 +104,8 @@
                 cur_tick_data['dateTime'] = pd.to_datetime(cur_tick_data['dateTime'])
                 all_tickers_df = pd.concat([all_tickers_df, cur_tick_data])
             except KeyError:
                 pass
         else:
             print(f'ERROR: smth is wrong with {i}')
     all_tickers_df.to_parquet(f'{PACKAGEDIR}/data.parquet.gz', compression='gzip')
-    print(f'Info about {len(tickers)} tickers successfully uploaded.')
+    print(f'Info about {len(tickers)} tickers successfully uploaded.')
```

### Comparing `ftsf-0.0.1.4/ftsf/utils.py` & `ftsf-0.0.2/ftsf/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from tensorflow.keras.layers import LSTM, Dense, GRU, SimpleRNN, Conv1D, Flatten
+'''This submodule contains utils to get nn topologies and models list, parse model names.'''
+
+from tensorflow.keras.layers import (GRU, LSTM, Conv1D, Dense, Flatten,
+                                     SimpleRNN)
+
 
 def get_topologies(lag = 30):
     '''
-    Generating neural network topologies adapted to defined lag. 
+    Generating neural network topologies adapted to defined lag.
 
     Args:
 
         lag: Number of previous values will be used to forecast on.
 
     Returns:
 
@@ -19,72 +23,72 @@
 
     neurons_per_layer = lag-1
     input_shape = (neurons_per_layer, 1)
 
     return {'CNN + LSTM': [Conv1D(filters = 128, kernel_size = 3, activation = 'relu', input_shape = input_shape),
                                 LSTM(units = neurons_per_layer),
                                 Dense(units = 1)],
-            'LSTM x3': [LSTM(units = neurons_per_layer, 
-                            return_sequences = True, 
+            'LSTM x3': [LSTM(units = neurons_per_layer,
+                            return_sequences = True,
                             input_shape = input_shape),
-                        LSTM(units = neurons_per_layer, 
+                        LSTM(units = neurons_per_layer,
                             return_sequences = True),
                         LSTM(units = neurons_per_layer),
                         Dense(units = 1)],
-            'LSTM x2': [LSTM(units = neurons_per_layer, 
-                            return_sequences = True, 
+            'LSTM x2': [LSTM(units = neurons_per_layer,
+                            return_sequences = True,
                             input_shape = input_shape),
                         LSTM(units = neurons_per_layer),
                         Dense(units = 1)],
-            'LSTM x1': [LSTM(units = neurons_per_layer, 
+            'LSTM x1': [LSTM(units = neurons_per_layer,
                             input_shape = input_shape),
                         Dense(units = 1)],
             'CNN + GRU': [Conv1D(filters = 128, kernel_size = 3, activation = 'relu', input_shape = input_shape),
                         GRU(units = neurons_per_layer),
                         Dense(units = 1)],
-            'GRU x3' : [GRU(units = neurons_per_layer, 
-                            return_sequences = True, 
+            'GRU x3' : [GRU(units = neurons_per_layer,
+                            return_sequences = True,
                             input_shape = input_shape),
-                        GRU(units = neurons_per_layer, 
+                        GRU(units = neurons_per_layer,
                             return_sequences = True),
                         GRU(units = neurons_per_layer),
                         Dense(units = 1)],
-            'GRU x2' : [GRU(units = neurons_per_layer, 
-                            return_sequences = True, 
+            'GRU x2' : [GRU(units = neurons_per_layer,
+                            return_sequences = True,
                             input_shape = input_shape),
                         GRU(units = neurons_per_layer),
                         Dense(units = 1)],
-            'GRU x1' : [GRU(units = neurons_per_layer, 
+            'GRU x1' : [GRU(units = neurons_per_layer,
                             input_shape = input_shape),
                         Dense(units = 1)],
             'CNN + SimpleRNN': [Conv1D(filters = 128, kernel_size = 3, activation = 'relu', input_shape = input_shape),
                                 SimpleRNN(units = neurons_per_layer),
                                 Dense(units = 1)],
-            'SimpleRNN x3':[SimpleRNN(units = neurons_per_layer, 
-                                    return_sequences = True, 
+            'SimpleRNN x3':[SimpleRNN(units = neurons_per_layer,
+                                    return_sequences = True,
                                     input_shape = input_shape),
-                            SimpleRNN(units = neurons_per_layer, 
+                            SimpleRNN(units = neurons_per_layer,
                                     return_sequences = True),
                             SimpleRNN(units = neurons_per_layer),
                             Dense(units = 1)],
-            'SimpleRNN x2':[SimpleRNN(units = neurons_per_layer, 
-                                    return_sequences = True, 
+            'SimpleRNN x2':[SimpleRNN(units = neurons_per_layer,
+                                    return_sequences = True,
                                     input_shape = input_shape),
                             SimpleRNN(units = neurons_per_layer),
                             Dense(units = 1)],
-            'SimpleRNN x1':[SimpleRNN(units = neurons_per_layer, 
+            'SimpleRNN x1':[SimpleRNN(units = neurons_per_layer,
                                     input_shape = input_shape),
                             Dense(units = 1)],
             'CNN': [Conv1D(filters = 32, kernel_size = 5, input_shape = input_shape, activation = 'relu'),
                     Flatten(),
                     Dense(units = 1)],
             'MLP(3)': [Dense(units = neurons_per_layer, input_shape = (neurons_per_layer,)),
                     Dense(units = neurons_per_layer*2),
                     Dense(units = neurons_per_layer),
-                    Dense(units = 1)],        
+                    Dense(units = 1)],
             'MLP(2)': [Dense(units = neurons_per_layer, input_shape = (neurons_per_layer,)),
                     Dense(units = neurons_per_layer),
                     Dense(units = 1)],
             'MLP(1)': [Dense(units = neurons_per_layer, input_shape = (neurons_per_layer,)),
                     Dense(units = 1)]}
 
 def get_models(type):
@@ -101,12 +105,38 @@
 
     Example:
     >>> get_models('ml')
     ['LR', 'DTR', 'RFR', 'GBR', 'SVR', 'CBR', 'XGBR', 'XGBRFR']
     '''
 
     models = {'ml': ['LR', 'DTR', 'RFR', 'GBR', 'SVR', 'CBR', 'XGBR', 'XGBRFR'],
-            'ar': ['ARMA(2,1)', 'ARIMA(2,1,1)'], 
+            'ar': ['ARMA(2,1)', 'ARIMA(2,1,1)'],
             'nn': ['CNN + LSTM', 'LSTM x3', 'LSTM x2', 'LSTM x1', 'CNN + GRU', 'GRU x3', 'GRU x2', 'GRU x1', \
                 'CNN + SimpleRNN', 'SimpleRNN x3', 'SimpleRNN x2', 'SimpleRNN x1', 'CNN', 'MLP(3)', 'MLP(2)', 'MLP(1)']}
-    
-    return models[type.lower()] if type != 'all' else models
+
+    return models[type.lower()] if type != 'all' else models
+
+def parse_name(name):
+    '''
+    Parsing p, d and q parameters from autoregressive model name.
+
+    Args:
+
+        name: Name of autoregressive model.
+
+    Returns:
+
+        List of parameters p, d and q.
+
+    Example:
+    >>> parse_name('ARIMA(2,1,1)')
+    (2, 1, 1)
+    '''
+    if name.find('I') != -1:
+        coef_p = float(name[name.find('(') + 1 : name.find(',')])
+        coef_d = float(name[name.find(',') + 1 : name.find(',', name.find(',') + 1)])
+        coef_q = float(name[name.find(',', name.find(',') + 1) + 1 : name.find(')')])
+    else:
+        coef_p = float(name[name.find('(') + 1 : name.find(',')])
+        coef_d = 0
+        coef_q = float(name[name.find(',') + 1 : name.find(')')])
+    return (coef_p, coef_d, coef_q)
```

### Comparing `ftsf-0.0.1.4/pyproject.toml` & `ftsf-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ftsf"
-version = "0.0.1.4"
+version = "0.0.2"
 authors = [{ name="Nikita Safonov", email="sixxio@yandex.ru" }]
 description = "Package for financial time series forecasting."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
```

