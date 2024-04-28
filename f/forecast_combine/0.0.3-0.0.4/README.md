# Comparing `tmp/forecast_combine-0.0.3.tar.gz` & `tmp/forecast_combine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecast_combine-0.0.3.tar", max compression
+gzip compressed data, was "forecast_combine-0.0.4.tar", max compression
```

## Comparing `forecast_combine-0.0.3.tar` & `forecast_combine-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-08-09 11:13:58.574534 forecast_combine-0.0.3/LICENSE
--rw-r--r--   0        0        0     3791 2024-04-18 10:16:14.517329 forecast_combine-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-19 11:40:31.366849 forecast_combine-0.0.3/forecast_combine/__init__.py
--rwxr-xr-x   0        0        0    47676 2024-04-19 11:32:34.647494 forecast_combine-0.0.3/forecast_combine/forecast.py
--rwxr-xr-x   0        0        0    49040 2024-04-19 11:36:03.211712 forecast_combine-0.0.3/forecast_combine/model_select.py
--rw-r--r--   0        0        0    17317 2024-04-19 11:32:37.711438 forecast_combine-0.0.3/forecast_combine/reconcile.py
--rw-r--r--   0        0        0     5534 2024-04-12 15:21:42.963039 forecast_combine-0.0.3/forecast_combine/utils/explore.py
--rw-r--r--   0        0        0     3194 2024-04-17 09:26:53.214931 forecast_combine-0.0.3/forecast_combine/utils/metrics.py
--rwxr-xr-x   0        0        0     9434 2024-04-15 11:32:24.768704 forecast_combine-0.0.3/forecast_combine/utils/plotting.py
--rw-r--r--   0        0        0     1329 2024-04-19 11:58:09.803691 forecast_combine-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 forecast_combine-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-09 11:13:58.574534 forecast_combine-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3791 2024-04-18 10:16:14.517329 forecast_combine-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 11:40:31.366849 forecast_combine-0.0.4/forecast_combine/__init__.py
+-rwxr-xr-x   0        0        0    47676 2024-04-19 11:32:34.647494 forecast_combine-0.0.4/forecast_combine/forecast.py
+-rwxr-xr-x   0        0        0    49442 2024-04-28 19:10:49.484229 forecast_combine-0.0.4/forecast_combine/model_select.py
+-rw-r--r--   0        0        0    17317 2024-04-19 11:32:37.711438 forecast_combine-0.0.4/forecast_combine/reconcile.py
+-rw-r--r--   0        0        0        0 2024-04-19 12:02:46.642685 forecast_combine-0.0.4/forecast_combine/utils/__init__.py
+-rw-r--r--   0        0        0     8839 2024-04-19 12:10:24.326406 forecast_combine-0.0.4/forecast_combine/utils/explore.py
+-rw-r--r--   0        0        0     3433 2024-04-19 12:12:37.491998 forecast_combine-0.0.4/forecast_combine/utils/metrics.py
+-rwxr-xr-x   0        0        0     9971 2024-04-28 17:47:46.285138 forecast_combine-0.0.4/forecast_combine/utils/plotting.py
+-rw-r--r--   0        0        0     1328 2024-04-28 20:24:57.089680 forecast_combine-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4917 1970-01-01 00:00:00.000000 forecast_combine-0.0.4/PKG-INFO
```

### Comparing `forecast_combine-0.0.3/LICENSE` & `forecast_combine-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.3/README.md` & `forecast_combine-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.3/forecast_combine/forecast.py` & `forecast_combine-0.0.4/forecast_combine/forecast.py`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.3/forecast_combine/model_select.py` & `forecast_combine-0.0.4/forecast_combine/model_select.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,19 @@
                 A tuple containing the aggregated prediction and prediction intervals.
         """
         if mode is None:
             mode = self._mode
         if mode == 'model':
             assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
             _lf_X = self.__stage_X(self.LF_d[model_name], X)
-            return self.LF_d[model_name].predict(X=_lf_X, fh=fh, coverage=coverage)
+            pred, pred_int = self.LF_d[model_name].predict(X=_lf_X, fh=fh, coverage=coverage)
+            if ret_underlying:
+                return pred, pred_int, None, None
+            else: 
+                return pred, pred_int
         else:
             preds = {}; pred_ints = {}
             for _fname, _lf in self.LF_d.items():
                 _lf_X = self.__stage_X(self.LF_d[_fname], X)                
                 _y_pred, _y_pred_ints = _lf.predict(X=_lf_X, fh=fh, coverage=coverage)
                 preds[_fname] = _y_pred
                 pred_ints[_fname] =_y_pred_ints
@@ -557,15 +561,19 @@
         """
         if mode is None:
             mode = self._mode
 
         if mode == 'model':
             assert model_name in self.LF_d.keys(), 'Model name not in the list of models'
             _lf_X = self.__stage_X(self.LF_d[model_name], new_X)
-            return self.LF_d[model_name].update(new_y=new_y, new_X=_lf_X, fh=fh, coverage=coverage, refit=refit)
+            pred, pred_int =  self.LF_d[model_name].update(new_y=new_y, new_X=_lf_X, fh=fh, coverage=coverage, refit=refit)
+            if ret_underlying:
+                return pred, pred_int, None, None
+            else: 
+                return pred, pred_int
         else:
             if reevaluate == False:            
                 preds = {}; pred_ints = {}
                 for _lf in self.LF_d.values():
                     _lf_X = self.__stage_X(_lf, new_X)
                     try:
                         _y_pred, _y_pred_ints = _lf.update(new_y=new_y, new_X=_lf_X, 
@@ -912,25 +920,14 @@
             y_pred = preds[_best_model]            
             if _best_model in pred_ints.columns:
                 y_pred_int = pred_ints[_best_model]
             else:
                 print(f'Prediction intervals for {_best_model} are not available')
                 y_pred_int = pd.DataFrame()
 
-        elif mode =='best_horizon':
-            # returns the prediction of the best model for each forecast horizon
-            best_horizon = self.model_rank_perhorizon[score].loc['Best_1'].to_dict()
-            y_pred = pd.Series([preds[v].iloc[k-1] for k, v in best_horizon.items()], 
-                   index=preds.index)
-            if all([v in pred_ints.columns for v in best_horizon.values()]):
-                y_pred_int = pd.concat([pred_ints[v].iloc[k-1].to_frame().T for k, v in best_horizon.items()])
-            else:
-                print('One or several model that are best in their respective horizon are not available')
-                y_pred_int = pd.DataFrame() 
-
         elif mode == 'average':
             # returns the average prediction of all models
             y_pred = preds.mean(axis=1)
             y_pred_int = pred_ints.unstack().unstack(0).mean(axis=1).unstack().T
 
         elif mode == 'inverse_score':
             # returns the Average models proportionals to performance score
@@ -955,23 +952,35 @@
             y_pred = preds[self._best_x_overall[score]].mean(axis=1)
             if all([v in pred_ints.columns for v in self._best_x_overall[score]]):
                 y_pred_int = pred_ints[self._best_x_overall[score]]\
             .unstack().unstack(0).mean(axis=1).unstack().T
             else:
                 print(f'Prediction intervals for {nbest} best models are not available')
                 y_pred_int = None
+        
+        elif mode =='best_horizon':
+            # returns the prediction of the best model for each forecast horizon
+            best_horizon = self.model_rank_perhorizon[score].loc['Best_1'].to_dict()
+            y_pred = pd.Series([preds[v].iloc[k-1] for k, v in best_horizon.items()], 
+                   index=preds.index)
+            if all([v in pred_ints.columns for v in best_horizon.values()]):
+                y_pred_int = pd.concat([pred_ints[v].iloc[k-1].to_frame().T for k, v in best_horizon.items()])
+            else:
+                print('One or several model that are best in their respective horizon are not available')
+                y_pred_int = pd.DataFrame() 
 
         elif mode == 'nbest_average_horizon':
             # return the average prediction on the nbest models per horizon
-            best_horizon = self.model_rank_perhorizon[score].iloc[:nbest].T
+            best_horizon = self.model_rank_perhorizon['RMSE'].iloc[:2].T
+            _uniq_best_model = self.model_rank_perhorizon['RMSE'].iloc[:2].T.unstack().unique()
             best_horizon = best_horizon.apply(lambda x: x.values, axis=1).to_dict()
 
             y_pred = pd.Series([preds[v].iloc[k-1].mean() for k, v in best_horizon.items()], 
                                index=preds.index)
-            if all([v in pred_ints.columns for v in best_horizon.values()]):
+            if all([v in pred_ints.columns for v in _uniq_best_model]):
                 y_pred_int = pd.concat([pred_ints[v].iloc[k-1].unstack(0).mean(axis=1).to_frame().T for k, v in best_horizon.items()])
                 y_pred_int.index = y_pred.index        
             else:
                 print(f'Prediction intervals for {nbest} best models are not available')
                 y_pred_int = None
                 
         else:
```

### Comparing `forecast_combine-0.0.3/forecast_combine/reconcile.py` & `forecast_combine-0.0.4/forecast_combine/reconcile.py`

 * *Files identical despite different names*

### Comparing `forecast_combine-0.0.3/forecast_combine/utils/metrics.py` & `forecast_combine-0.0.4/forecast_combine/utils/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,21 +6,31 @@
     mean_absolute_error,
     r2_score,
     median_absolute_error
 )
 
 def evaluate_metrics(y_true, y_pred):
     """
-    Computes performance metrics for the fitted curve.
-    The performance metrics include 
-        RMSE: Root Mean Squared Error
-        MAE: Mean Absolute Error
-        MAPE: Mean Absolute Percentage Error
-        R2: R-squared
-        MedianAE: Median Absolute Error
+    Computes performance metrics for the fitted curve. The currently covered performance metrics include 
+    - RMSE: Root Mean Squared Error
+    - MAE: Mean Absolute Error
+    - MAPE: Mean Absolute Percentage Error
+    - R2: R-squared
+    - MedianAE: Median Absolute Error
+
+    Parameters:
+    -----------
+        y_true (array-like): 
+            The true values.
+        y_pred (array-like): 
+            The predicted values.
+
+    Returns:
+    --------
+        Series: A series containing the performance metrics.
     """
     metrics = {
         'RMSE': np.sqrt(mean_squared_error(y_true, y_pred)),
         'MAE': mean_absolute_error(y_true, y_pred),
         'MAPE': np.mean(np.abs((y_true - y_pred) / y_true)),
         'R2': r2_score(y_true, y_pred),
         'MedianAE': median_absolute_error(y_true, y_pred)
@@ -30,19 +40,20 @@
 def summary_perf(insample_result_df, 
 			 grouper, 
 			 y_true_col = 'y_true',
 			 y_pred_col = 'y_pred',
 			):
     """
 	Compute summary performance metrics for a given forecast.
-        RMSE: Root Mean Squared Error
-        MAE: Mean Absolute Error
-        MAPE: Mean Absolute Percentage Error
-        R2: R-squared
-        MedianAE: Median Absolute Error
+    - RMSE: Root Mean Squared Error
+    - MAE: Mean Absolute Error
+    - MAPE: Mean Absolute Percentage Error
+    - R2: R-squared
+    - MedianAE: Median Absolute Error
+
 
 	Parameters:
     -----------
 	    insample_result_df (DataFrame): 
             A DataFrame containing the forecast results.
 		grouper (str): 
             The column name to group the forecast results for computing summary metrics.
```

### Comparing `forecast_combine-0.0.3/forecast_combine/utils/plotting.py` & `forecast_combine-0.0.4/forecast_combine/utils/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,32 @@
     
     if _ax_kwarg_is_none:
         return fig, ax
     else:
         return ax
 
 def plot_interval(ax, interval_df, legend_label ='prediction interval'):
+    """
+    Plot the confidence interval within a plot.
+
+    Parameters:
+    -----------
+        ax : plt.Axes
+            The Axes object for the plot.
+        interval_df : pd.DataFrame
+            Output of `forecaster.predict_interval()`. Contains columns for lower
+            and upper boundaries of confidence interval.
+        legend_label : str, default = 'prediction interval'
+            The label for the legend.
+
+    Returns:
+    --------
+        ax : plt.Axes
+            Axes containing the plot
+    """
     cov = interval_df.columns.levels[1][0]
     var_name = interval_df.columns.levels[0][0]
     ax.fill_between(
         ax.get_lines()[-1].get_xdata(),
         interval_df[var_name][cov]["lower"].astype("float64"),
         interval_df[var_name][cov]["upper"].astype("float64"),
         alpha=0.2,
```

### Comparing `forecast_combine-0.0.3/pyproject.toml` & `forecast_combine-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forecast_combine"
-version = "0.0.3"
+version = "0.0.4"
 description = "Automation of forecast models testing, combining and predicting"
 authors = ["amineraboun <amineraboun@gmail.com>"]
 repository ="https://github.com/amineraboun/forecast"
 homepage  ="https://github.com/amineraboun/forecast"
 
 readme = "README.md"
 keywords = ["arima", "ets", "theta", "tbats", "prophet"]
@@ -23,27 +23,26 @@
 tbats = "^1.1.3"
 prophet = "^1.1.4"
 arch = "^6.3.0"
 statsmodels = "^0.14.0"
 tqdm = "^4.66.0"
 matplotlib = "^3.7.2"
 seaborn = "^0.12.2"
+openpyxl = "^3.1.2"
+
+[tool.poetry.dev-dependencies]
+pytest = "^7.1.3"
+pytest-cov = "^3.0"
 sphinx = "^7.1.2"
 nbsphinx = "^0.9.2"
 sphinx-mdinclude = "^0.5.3"
 pandoc = "^2.3"
-openpyxl = "^3.1.2"
 pdoc = "^14.4.0"
 typing-extensions = "^4.11.0"
 
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
-pytest-cov = "^3.0"
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = [
     "tests",
 ]
 
 [tool.pylint]
```

### Comparing `forecast_combine-0.0.3/PKG-INFO` & `forecast_combine-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 Metadata-Version: 2.1
 Name: forecast_combine
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automation of forecast models testing, combining and predicting
 Home-page: https://github.com/amineraboun/forecast
 Keywords: arima,ets,theta,tbats,prophet
 Author: amineraboun
 Author-email: amineraboun@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arch (>=6.3.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
-Requires-Dist: nbsphinx (>=0.9.2,<0.10.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandoc (>=2.3,<3.0)
-Requires-Dist: pdoc (>=14.4.0,<15.0.0)
 Requires-Dist: prophet (>=1.1.4,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: sktime (>=0.28.0,<0.29.0)
-Requires-Dist: sphinx (>=7.1.2,<8.0.0)
-Requires-Dist: sphinx-mdinclude (>=0.5.3,<0.6.0)
 Requires-Dist: statsforecast (>=1.7.4,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: tbats (>=1.1.3,<2.0.0)
 Requires-Dist: tqdm (>=4.66.0,<5.0.0)
-Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Project-URL: Repository, https://github.com/amineraboun/forecast
 Description-Content-Type: text/markdown
 
 # forecast_combine
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
```

