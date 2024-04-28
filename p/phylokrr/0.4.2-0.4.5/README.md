# Comparing `tmp/phylokrr-0.4.2.tar.gz` & `tmp/phylokrr-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phylokrr-0.4.2.tar", last modified: Sun Feb 25 07:50:02 2024, max compression
+gzip compressed data, was "dist/phylokrr-0.4.5.tar", last modified: Sun Apr 28 01:28:40 2024, max compression
```

## Comparing `phylokrr-0.4.2.tar` & `phylokrr-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-02-25 07:50:02.000000 phylokrr-0.4.2/
--rw-r--r--   0 ulises     (502) staff       (20)     3818 2024-02-25 07:50:02.000000 phylokrr-0.4.2/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)     3581 2024-02-25 07:49:25.000000 phylokrr-0.4.2/README.md
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-02-25 07:50:02.000000 phylokrr-0.4.2/phylokrr.egg-info/
--rw-r--r--   0 ulises     (502) staff       (20)     3818 2024-02-25 07:50:01.000000 phylokrr-0.4.2/phylokrr.egg-info/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)      295 2024-02-25 07:50:01.000000 phylokrr-0.4.2/phylokrr.egg-info/SOURCES.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-02-25 07:50:01.000000 phylokrr-0.4.2/phylokrr.egg-info/dependency_links.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-02-25 07:01:05.000000 phylokrr-0.4.2/phylokrr.egg-info/not-zip-safe
--rw-r--r--   0 ulises     (502) staff       (20)        6 2024-02-25 07:50:01.000000 phylokrr-0.4.2/phylokrr.egg-info/requires.txt
--rw-r--r--   0 ulises     (502) staff       (20)        9 2024-02-25 07:50:01.000000 phylokrr-0.4.2/phylokrr.egg-info/top_level.txt
--rw-r--r--   0 ulises     (502) staff       (20)       38 2024-02-25 07:50:02.000000 phylokrr-0.4.2/setup.cfg
--rw-r--r--   0 ulises     (502) staff       (20)      570 2024-02-25 07:49:55.000000 phylokrr-0.4.2/setup.py
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-02-25 07:50:02.000000 phylokrr-0.4.2/src/
--rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.4.2/src/__init__.py
--rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.4.2/src/core.py
--rw-r--r--   0 ulises     (502) staff       (20)    10353 2024-02-25 07:45:07.000000 phylokrr-0.4.2/src/kernels.py
--rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.4.2/src/metrics.py
--rw-r--r--   0 ulises     (502) staff       (20)      234 2024-02-25 06:45:59.000000 phylokrr-0.4.2/src/phylosig.py
--rw-r--r--   0 ulises     (502) staff       (20)     4501 2024-02-22 06:24:07.000000 phylokrr-0.4.2/src/utils.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 01:28:40.000000 phylokrr-0.4.5/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 01:28:40.000000 phylokrr-0.4.5/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)     3579 2024-04-27 21:04:58.000000 phylokrr-0.4.5/README.md
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)      313 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/SOURCES.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        1 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/dependency_links.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        1 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/not-zip-safe
+-rw-r--r--   0 ulises     (502) staff       (20)        6 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/requires.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        9 2024-04-28 01:28:40.000000 phylokrr-0.4.5/phylokrr.egg-info/top_level.txt
+-rw-r--r--   0 ulises     (502) staff       (20)       38 2024-04-28 01:28:40.000000 phylokrr-0.4.5/setup.cfg
+-rw-r--r--   0 ulises     (502) staff       (20)      574 2024-04-28 01:28:20.000000 phylokrr-0.4.5/setup.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-04-28 01:28:40.000000 phylokrr-0.4.5/src/
+-rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.4.5/src/__init__.py
+-rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.4.5/src/core.py
+-rw-r--r--   0 ulises     (502) staff       (20)     2650 2024-04-23 23:57:46.000000 phylokrr-0.4.5/src/inspection.py
+-rw-r--r--   0 ulises     (502) staff       (20)     7245 2024-04-23 23:30:12.000000 phylokrr-0.4.5/src/kernels.py
+-rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.4.5/src/metrics.py
+-rw-r--r--   0 ulises     (502) staff       (20)    20652 2024-04-23 23:32:36.000000 phylokrr-0.4.5/src/phylosig.py
+-rw-r--r--   0 ulises     (502) staff       (20)    15326 2024-04-28 01:15:05.000000 phylokrr-0.4.5/src/utils.py
```

### Comparing `phylokrr-0.4.2/PKG-INFO` & `phylokrr-0.4.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: phylokrr
-Version: 0.4.2
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
 # Non-linear Phylogenetic regression using regularized kernels
 
 
 # Installation
 
 ```
 pip install phylokrr
@@ -38,15 +27,15 @@
 vcv = np.loadtxt("./data/test_cov2.csv", delimiter=',') 
 
 # Trait simulation under Brownian motion
 n = vcv.shape[0]
 mean = np.zeros(n)
 X = np.random.multivariate_normal(cov=vcv, mean=mean).reshape(-1,1)
 # Non-linear response variable (sine curve)
-y = np.sin(X*2.1).ravel() + 5 
+y = np.sin(X*2).ravel() + 5 
 
 # Add noise to the response variable
 y[::10] += 4 * (0.5 - np.random.rand(X.shape[0] // 10)) 
 ```
 We then split data into training and testing sets, including their covariances
 
 ```python
@@ -133,9 +122,7 @@
 <img src="https://github.com/Ulises-Rosas/phylokrr/blob/main/data/imgs/phyloKRR_vs_PGLS_cv.png" alt="drawing" width="600px"/>
 </p>
 
 
 # Reference
 
 Rosas-Puchuri, U., Santaquiteria, A., Khanmohammadi, S., Solis-Lemus, C., & Betancur-R, R. (2023). [Non-linear phylogenetic regression using regularized kernels](https://www.biorxiv.org/content/10.1101/2023.10.04.560983v1.abstract). bioRxiv, 2023-10.
-
-
```

### Comparing `phylokrr-0.4.2/setup.py` & `phylokrr-0.4.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     "numpy"
 ]
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(name = "phylokrr",
-      version = '0.4.2',
-      long_description = readme,
-      long_description_content_type = 'text/markdown',
+      version = '0.4.5',
+    #   long_description = readme,
+    #   long_description_content_type = 'text/markdown',
       packages = ['phylokrr'],
       package_dir = {'phylokrr': 'src'},
       python_requires='>=3.5',
       install_requires = dependencies,
       zip_safe = False,
       classifiers = [
           'Programming Language :: Python :: 3',
```

### Comparing `phylokrr-0.4.2/src/core.py` & `phylokrr-0.4.5/src/core.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.2/src/kernels.py` & `phylokrr-0.4.5/src/kernels.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,298 +21,163 @@
     """
     XXt = a.dot(b.T)
     C = c * np.ones(XXt.shape)
 
     return XXt + C
 
 
-
-class KRR:
-
-    def __init__(self, kernel = 'rbf', fit_intercept = True, check_cov = False) -> None:
-        """
-        Weighted Kernel Ridge Regression
-
-        kernel: str, default = 'rbf'
-            kernel type
-
-        fit_intercept: bool, default = True
-            fit intercept term
-
-        check_cov: bool, default = False
-            Check covariance matrix, i.e., P.T @ P == vcv^-1
-        """
-
+class WKRR:
+    def __init__(self, kernel='rbf', fit_intercept=True, check_cov=False) -> None:
         self.kernel = kernel
 
         if self.kernel == 'rbf':
             self.params = {'gamma': 0.1, 'lambda': 0.1}
 
         else:
             self.params = {'c': 0.1, 'lambda': 0.1}
 
         self.fit_intercept = fit_intercept
         self.check_cov = check_cov
-        
-        # internal
         self.intercept = 0
         self.alpha = np.array([])
         self.X = np.array([])
-
         self.chol = False
 
     def set_params(self, **params):
-
         if self.kernel == 'rbf':
             self.params['gamma'] = params['gamma']
 
         else:
             self.params['c'] = params['c']
 
         self.params['lambda'] = params['lambda']
 
     def get_params(self):
         return self.params
-    
+
     def P_mat(self, vcv):
-        """
-        get the square root of the inverse of the
-        covariance matrix.
-
-        vcv: np.array, default = None
-            covariance matrix
-        """
-        
         if isinstance(vcv, type(None)):
             return None
-        
+
         if self.check_cov:
             self.assert_COV_sym(vcv)
 
         if self.chol:
-            C = np.linalg.cholesky( vcv )
-            P = np.linalg.inv( C )
+            C = np.linalg.cholesky(vcv)
+            P = np.linalg.inv(C)
 
         else:
-            L,Q  = np.linalg.eig( vcv )
-            P  = Q @ np.diag( L**(-1/2) ) @ Q.T 
+            L, Q = np.linalg.eig(vcv)
+            P = Q @ np.diag(L ** (-1 / 2)) @ Q.T
 
         if self.check_cov:
             self.assert_COV_decom(P, vcv)
 
         return P
-    
+
     def assert_COV_sym(self, vcv, tol=1e-8):
-        assert np.all(np.abs(vcv-vcv.T) < tol), 'not symmetric matrix'
+        assert np.all(np.abs(vcv - vcv.T) < tol), 'not symmetric matrix'
 
     def assert_COV_decom(self, P, vcv):
-        """
-        check if P.T @ P == vcv^-1
-        expensive calculation for large matrices
-        """
         assert np.all(np.round(P.T @ P, 2) == np.round(np.linalg.inv(vcv), 2)), "P.T @ P != vcv^-1"
 
-    def fit(self, X, y, vcv = None):
-        """
-        Fit the model
-
-        vcv: np.array, default = None
-            covariance matrix
-
-        """
-        # X = X_train
-        # y = y_train
-        # vcv = vcv_train
-        
+    def fit(self, X, y, vcv=None):
         self.X = X
-        # self.y = y
         P = self.P_mat(vcv)
 
         if self.kernel == 'rbf':
             K_train = RBF_kernel(self.X, self.X, self.params['gamma'])
-
         else:
             K_train = linear_kernel(self.X, self.X, self.params['c'])
 
         self.alpha = self.opt_alpha(K_train, y, self.params['lambda'], P)
-        
-        # intercept term 
+
         if self.fit_intercept:
             self.intercept = np.mean(y - K_train @ self.alpha)
 
     def predict(self, X_test):
-
         assert len(self.alpha) > 0, "The model needs to be fitted first"
 
         if self.kernel == 'rbf':
             K_test = RBF_kernel(X_test, self.X, self.params['gamma'])
-
         else:
             K_test = linear_kernel(X_test, self.X, self.params['c'])
-        
-        return K_test @ self.alpha + self.intercept
-    
-    def score(self, X_test, y_test, vcv_test, metric = 'rmse'):
-        """
-        
-        Calculates score considerint the covariance matrix
-        This error is the same as the in objective function
 
-        X_test: np.array
-            testing data
-        
-        y_test: np.array
-            testing targets
-        
-        vcv_test: np.array
-            testing covariance matrix. If None, then it
-            will return the standard RMSE and R^2
-
-        metric: str, default = 'rmse'
-            weighted root mean squared error (the same 
-            that was used to construct the objective function).
-            if metric = 'r2', then it returns the R^2 which
-            also considers the covariance matrix, see Willett & Singer (1988)
-
-        Returns:
-        --------
-        float
-            score
-
-        Reference:
-        ---------
-        Willett, J. B., & Singer, J. D. (1988). 
-        Another cautionary note about R 2: Its use 
-        in weighted least-squares regression analysis. 
-        The American Statistician, 42(3), 236-238.
-        """
+        return K_test @ self.alpha + self.intercept
 
+    def score(self, X_test, y_test, vcv_test, metric='rmse'):
         y_pred = self.predict(X_test)
-        r = y_pred - y_test
-        
+
         if isinstance(vcv_test, type(None)):
             P = np.eye(X_test.shape[0])
-
         else:
             P = self.P_mat(vcv_test)
 
-        werr = P @ r # weighted residuals
-        Py   = P @ y_test # weighted targets
+        werr = P @ (y_pred - y_test)  # weighted residuals
 
         if metric == 'rmse':
             return rmse(werr)
-        
         else:
+            Py = P @ y_test  # weighted targets
             return R2(Py, werr)
-            
-        # if metric == 'rmse':
-        #     return np.sqrt( np.mean( r**2 ) )
-        
-        # else:
-        #     u = r.T @ r
-        #     v = y_test.T @ y_test - n * np.mean(y_test)**2
-        #     return 1 - (u/v)
-    
-    def opt_alpha(self, K, y, reg_lam = None, P = None):
-        # Y = y
-        # X = X
-        # m = None
-        n,_ = self.X.shape
-        
+
+    def opt_alpha(self, K, y, reg_lam=None, P=None):
+
+        n, _ = self.X.shape
         I = np.eye(K.shape[0])
         nlI = n * reg_lam * I
 
         if isinstance(P, type(None)):
             return np.linalg.solve(K + nlI, y)
         
         else:
-            return P @ np.linalg.solve(P @ K @ P + nlI,  P @ y)
-            # return np.linalg.solve(P.T @ P @ K + nlI,  P.T @ P @ y)
+            return P @ np.linalg.solve(P @ K @ P + nlI, P @ y)
 
+class KRR(WKRR):
 
-class LKRR:
-
-    def __init__(self, kernel = 'rbf') -> None:
-
-        self.kernel = kernel
-
-        if self.kernel == 'rbf':
-            self.params = {'gamma': 0.1, 'lambda': 0.1}
-
-        else:
-            self.params = {'c': 0.1, 'lambda': 0.1}
-
-        # internal
-        self.alpha = []
-        self.X = []
-        self.y = []
-
-    def p1(self, X, beta):
-        return 1/(1 + np.exp(X.dot(beta)))
-
-    def p0(self, X, beta):
-        EX = np.exp(X.dot(beta))
-        return EX/(1 + EX)
-
-    def set_params(self, params):
-        self.params = params
+    def __init__(self, kernel='rbf', fit_intercept=True) -> None:
+        super().__init__(kernel, fit_intercept)
+        self.intercept = 0
+        self.alpha = np.array([])
+        self.X = np.array([])
 
-    def get_params(self):
-        return self.params
-    
     def fit(self, X, y):
-        
         self.X = X
         self.y = y
 
         if self.kernel == 'rbf':
             K_train = RBF_kernel(self.X, self.X, self.params['gamma'])
-
+            
         else:
             K_train = linear_kernel(self.X, self.X, self.params['c'])
 
         self.alpha = self.opt_alpha(K_train, self.y, self.params['lambda'])
 
-    def predict(self, X_test):
-
-        assert len(self.alpha) > 0, "The model needs to be fitted first"
+        if self.fit_intercept:
+            self.intercept = np.mean(y - K_train @ self.alpha)
 
-        if self.kernel == 'rbf':
-            K_test = RBF_kernel(X_test, self.X, self.params['gamma'])
+    def opt_alpha(self, K, y, reg_lam=None):
+        
+        n, _ = self.X.shape
+        I = np.eye(K.shape[0])
+        nlI = n * reg_lam * I
 
-        else:
-            K_test = linear_kernel(X_test, self.X, self.params['c'])
+        return np.linalg.solve(K + nlI, y)
         
-        return K_test @ self.alpha
-    
-    def score(self, X_test, y_test, metric = 'rmse'):
 
+    def score(self, X_test, y_test, metric='rmse'):
         y_pred = self.predict(X_test)
 
         if metric == 'rmse':
-            return np.sqrt( np.mean( (y_pred - y_test)**2 ) )
-    
+            return np.sqrt(np.mean((y_pred - y_test) ** 2))
         else:
-            # r2
-            u = ((y_test - y_pred)**2).sum()
-            v = ((y_test - y_test.mean())** 2).sum()
-
-            return 1 - (u/v)
-    
-    def rmse(self, K, alpha, Y):
-
-        return np.sqrt( np.mean( (K.dot(alpha) - Y)**2 ) )
-    
-    def opt_alpha(self, K, y, reg_lam = None):
-        # Y = y
-        # X = X
-        # m = None
-        K_Idx = K + reg_lam * np.diag( np.ones( K.shape[0] ) )
-        return np.linalg.inv( K_Idx ).dot( y )
+            u = ((y_test - y_pred) ** 2).sum()
+            v = ((y_test - y_test.mean()) ** 2).sum()
 
+            return 1 - (u / v)
 
 # def P_mat(vcv, chol = False, corr = False):
     
 #     if corr:
 #         Kr = np.diag(1/np.sqrt(np.diag(vcv)))
 #         vcv = Kr @ vcv @ Kr
```

