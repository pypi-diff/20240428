# Comparing `tmp/cfpack-0.1.6.tar.gz` & `tmp/cfpack-0.1.7.tar.gz`

## Comparing `cfpack-0.1.6.tar` & `cfpack-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.6/pyproject.toml.new
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.6/pyproject.toml.old
--rw-r--r--   0        0        0    47144 2020-02-02 00:00:00.000000 cfpack-0.1.6/cfpack/__init__.py
--rwxr-xr-x   0        0        0     6551 2020-02-02 00:00:00.000000 cfpack-0.1.6/cfpack/automator.py
--rwxr-xr-x   0        0        0     5236 2020-02-02 00:00:00.000000 cfpack-0.1.6/cfpack/browser_control.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.1.6/cfpack/constants.py
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.1.6/cfpack/hdfio.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 cfpack-0.1.6/cfpack/matplotlibrc.py
--rwxr-xr-x   0        0        0     2772 2020-02-02 00:00:00.000000 cfpack-0.1.6/cfpack/tests.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.1.6/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.1.6/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cfpack-0.1.6/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 cfpack-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack.browser_control.html
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack.html
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.7/pyproject.toml.new
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.7/pyproject.toml.old
+-rw-r--r--   0        0        0    49822 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/__init__.py
+-rwxr-xr-x   0        0        0     6551 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/automator.py
+-rwxr-xr-x   0        0        0     5236 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/browser_control.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/constants.py
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/hdfio.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/matplotlibrc.py
+-rwxr-xr-x   0        0        0     2772 2020-02-02 00:00:00.000000 cfpack-0.1.7/cfpack/tests.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cfpack-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cfpack-0.1.7/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 cfpack-0.1.7/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cfpack-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 cfpack-0.1.7/PKG-INFO
```

### Comparing `cfpack-0.1.6/pyproject.toml.new` & `cfpack-0.1.7/pyproject.toml.new`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.0"
+version = "0.1.5"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.6/pyproject.toml.old` & `cfpack-0.1.7/pyproject.toml.old`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.6/cfpack/__init__.py` & `cfpack-0.1.7/cfpack/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,17 @@
                 return stop()
         exit() # exit on error
     return # return if everything is normal
 # === END print ===
 
 # === START plot ===
 def plot(y=None, x=None, yerr=None, xerr=None, type=None, xlabel='x', ylabel='y', label=None, marker=None, linestyle=None, linewidth=None, aspect=None,
-         show=False, pause=None, xlog=False, ylog=False, xlim=None, ylim=None, save=None, legend_loc='upper left', text=None, shaded_err=None, bin_width=0.5, *args, **kwargs):
+         show=False, pause=None, xlog=False, ylog=False, xlim=None, ylim=None, axes_format=[None,None], save=None, legend_loc='upper left', text=None, shaded_err=None, bin_width=0.5, *args, **kwargs):
     import matplotlib.pyplot as plt
+    import matplotlib as mpl
     if linestyle == 'long dashed': linestyle = (0,(5,5))
     if y is not None:
         if x is None: x = np.arange(len(y)) # in this case, we just use the array indices as the x axis values
         if text is not None:
             plt.text(x, y, text, *args, **kwargs)
         else:
             if type == 'pdf' or type == 'histogram' or type == 'hist':
@@ -89,40 +90,41 @@
                     print("x must contain bin edges for type='"+type+"'", error=True)
                 width = (x[1:]-x[:-1]) * bin_width # bin widths
                 x = (x[1:]+x[:-1]) / 2.0 # bin mid points
                 plt.bar(x, height=y, width=width, *args, **kwargs)
             if type == 'scatter':
                 linestyle = "None"
                 if marker is None: marker = 'o'
-            if shaded_err is not None: # switch off error bars if shaded error region is requested
-                xerr_bars = None; yerr_bars = None
-            else:
-                xerr_bars = xerr; yerr_bars = yerr
+            xerr_bars = None; yerr_bars = None
+            if shaded_err is None: # only plot error bars, if shaded error region is not requested
+                if xerr is not None: xerr_bars = np.abs(xerr)
+                if yerr is not None: yerr_bars = np.abs(yerr)
             if type == 'scatter':
                 plt.scatter(x, y, marker=marker, linestyle=linestyle, linewidth=linewidth, label=label, *args, **kwargs)
             else:
                 plt.errorbar(x, y, xerr=xerr_bars, yerr=yerr_bars, marker=marker, linestyle=linestyle, linewidth=linewidth, label=label, *args, **kwargs)
             if shaded_err is not None: # yerr must have shape (2,N), containing the lower and upper errors for each of the N data points
                 if isinstance(shaded_err, list): # user provided a list with [color, alpha]
                     color_err = shaded_err[1]
                     alpha_err = shaded_err[0]
                 else:
                     color_err = plt.gca().lines[-1].get_color()
                     alpha_err = 0.5
-                plt.fill_between(x, y-yerr[0], y+yerr[1], color=color_err, alpha=alpha_err, linewidth=0.0)
+                plt.fill_between(x, y-np.abs(yerr[0]), y+np.abs(yerr[1]), color=color_err, alpha=alpha_err, linewidth=0.0)
     if show or save:
         ax = plt.gca()
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
         if xlim is not None: plt.xlim(xlim)
         if ylim is not None: plt.ylim(ylim)
         if xlog: ax.set_xscale('log')
         if ylog: ax.set_yscale('log')
-        if aspect is not None:
-            ax.set_aspect(aspect)
+        if axes_format[0] is not None: ax.xaxis.set_major_formatter(mpl.ticker.StrMethodFormatter(axes_format[0]))
+        if axes_format[1] is not None: ax.yaxis.set_major_formatter(mpl.ticker.StrMethodFormatter(axes_format[1]))
+        if aspect is not None: ax.set_aspect(aspect)
         legend_handles, legend_labels = ax.get_legend_handles_labels()
         if legend_labels or legend_handles: plt.legend(loc=legend_loc, *args, **kwargs)
         if save:
             plt.savefig(save, bbox_inches='tight')
             print(save+' written.', color='magenta')
         if show:
             block = None
@@ -202,16 +204,20 @@
     values = values[::-1]
     # Finally, scale output values to cmap range.
     values = cmap_vmin + values * (cmap_vmax - cmap_vmin)
     return values
 # === END rgba2data ===
 
 # === START fit ===
-# params should be a dict with the parameter name(s) and a list specifying [min, start, max]
-def fit(func, xdat, ydat, xerr=None, yerr=None, n_random_draws=1000, weights=None, scale_covar=True, params=None, verbose=1, *args, **kwargs):
+# - params can be a dict with the parameter name(s) and a list specifying [min, start, max]
+# - Method for parameter error estimate (based on random sampling with n_random_draws=1000):
+#     perr_method='statistical': statistical error estimate based on sampling from data errors provided (xerr and/or yerr)
+#     perr_method='systematic' : systematic error estimate based on sampling dat_frac_for_systematic_perr=0.5 of the original data
+def fit(func, xdat, ydat, xerr=None, yerr=None, perr_method='statistical', n_random_draws=1000, dat_frac_for_systematic_perr=0.3,
+        weights=None, scale_covar=True, params=None, verbose=1, *args, **kwargs):
     from lmfit import Model as lmfit_model
     model = lmfit_model(func) # get lmfit model object
     # set up parameters
     lmfit_params = model.make_params() # make lmfit default params
     if params is not None: # user previded parameter bounds and initial values
         for pname in params:
             if pname not in model.param_names: print("parameter key error: '"+pname+"'", error=True)
@@ -251,49 +257,73 @@
     ret_pstd = [] # parameter standard deviation
     ret_perr = [] # parameter error range (lower and upper)
     ret_psamples = [] # parameter sampling list (only if xerr or yerr is used)
     ret_lmfit_result = None # lmfit result
     # dealing with weights or errors (1-sigma data errors in x and/or y)
     if weights is not None and ((xerr is not None) or (yerr is not None)):
         print("cannot use weights when either xerr or yerr is present", error=True)
-    if xerr is not None or yerr is not None:
-        print("Performing a total of "+str(n_random_draws)+" sampling fits...")
-        # draw from Gaussian random distribution
-        if xerr is not None:
-            xtry = np.array([generate_random_gaussian_numbers(n=n_random_draws, mu=xdat[i], sigma=xerr[i], seed=None) for i in range(len(xdat))])
-        if yerr is not None:
-            ytry = np.array([generate_random_gaussian_numbers(n=n_random_draws, mu=ydat[i], sigma=yerr[i], seed=None) for i in range(len(ydat))])
-        # for each random sample, fit and record the best-fit parameter(s) in popts
-        popts = []
-        for i in range(n_random_draws):
+    if xerr is not None or yerr is not None or perr_method == "systematic":
+        popts = [] # list of parameter samples
+        if perr_method == "statistical":
+            print("Performing statistical error estimate with "+str(n_random_draws)+" sampling fits, based on data errors provided...", highlight=True)
+            # draw from Gaussian random distribution
             if xerr is not None:
-                x = xtry[:,i]
-            else:
-                x = xdat
+                xtry = np.array([generate_random_gaussian_numbers(n=n_random_draws, mu=xdat[i], sigma=xerr[i], seed=None) for i in range(len(xdat))])
             if yerr is not None:
-                y = ytry[:,i]
-            else:
-                y = ydat
-            independent_vars_dict = {model.independent_vars[0]:x} # set independent variable
-            fit_result = model.fit(data=y, params=lmfit_params, weights=None, *args, **kwargs, **independent_vars_dict)
-            popt = []
-            for pname in fit_result.params:
-                popt.append(fit_result.params[pname].value)
-            popts.append(popt)
-        popts = np.array(popts)
+                ytry = np.array([generate_random_gaussian_numbers(n=n_random_draws, mu=ydat[i], sigma=yerr[i], seed=None) for i in range(len(ydat))])
+            # for each random sample, fit and record the best-fit parameter(s) in popts
+            for i in range(n_random_draws):
+                if xerr is not None:
+                    x = xtry[:,i]
+                else:
+                    x = xdat
+                if yerr is not None:
+                    y = ytry[:,i]
+                else:
+                    y = ydat
+                independent_vars_dict = {model.independent_vars[0]:x} # set independent variable
+                fit_result = model.fit(data=y, params=lmfit_params, weights=None, *args, **kwargs, **independent_vars_dict)
+                popt = []
+                for pname in fit_result.params:
+                    popt.append(fit_result.params[pname].value)
+                popts.append(popt)
+        if perr_method == "systematic":
+            print("Performing systematic error estimate with "+str(n_random_draws)+" sampling fits, based on random subsets of "+str(dat_frac_for_systematic_perr*100)+"% of the original data...", highlight=True)
+            from random import seed, randrange
+            n_dat_frac = max([len(lmfit_params)+1, int(np.ceil(dat_frac_for_systematic_perr*len(xdat)))]) # take only a fraction of the original data size (minimally, the number of parameters + 1)
+            n_dat_toss = len(xdat) - n_dat_frac # number of data elements to drop
+            for i in range(n_random_draws):
+                x = np.copy(xdat) # copy original x data
+                y = np.copy(ydat) # copy original y data
+                for i in range(n_dat_toss): # now randomly remove indices
+                    seed(None) # set the random seed; if None, random uses the system time
+                    ind = randrange(len(x))
+                    x = np.delete(x, ind)
+                    y = np.delete(y, ind)
+                independent_vars_dict = {model.independent_vars[0]:x} # set independent variable
+                fit_result = model.fit(data=y, params=lmfit_params, weights=None, *args, **kwargs, **independent_vars_dict)
+                popt = []
+                for pname in fit_result.params:
+                    popt.append(fit_result.params[pname].value)
+                popts.append(popt)
         # prepare return values (median, standard deviation, 16th to 84th percentile, and complete list of popts)
-        for ip, pname in enumerate(fit_result.params):
-            median = np.percentile(popts[:,ip], 50)
-            percentile_16 = np.percentile(popts[:,ip], 16)
-            percentile_84 = np.percentile(popts[:,ip], 84)
-            ret_popt.append(median)
-            ret_pstd.append(np.std(popts[:,ip]))
-            ret_perr.append(np.array([-(median-percentile_16), (percentile_84-median)]))
-            ret_psamples.append(popts)
+        if len(popts) > 0:
+            popts = np.array(popts)
+            for ip, pname in enumerate(fit_result.params):
+                median = np.percentile(popts[:,ip], 50)
+                percentile_16 = np.percentile(popts[:,ip], 16)
+                percentile_84 = np.percentile(popts[:,ip], 84)
+                ret_popt.append(median)
+                ret_pstd.append(np.std(popts[:,ip]))
+                ret_perr.append(np.array([-(median-percentile_16), (percentile_84-median)]))
+                ret_psamples.append(popts)
     else: # do a normal weighted or unweighted fit
+        weights_info_str = "without"
+        if weights is not None: weights_info_str = "with"
+        print("Performing normal fit "+weights_info_str+" weights...", highlight=True)
         if weights is not None and scale_covar:
             print("Assuming good fit for reporting parameter errors. "+
                     "Consider setting 'scale_covar=False' if you believe the fit is not of good quality.", warn=True)
         # do the fit
         independent_vars_dict = {model.independent_vars[0]:xdat} # set independent variable
         fit_result = model.fit(data=ydat, params=lmfit_params, weights=weights, scale_covar=scale_covar, *args, **kwargs, **independent_vars_dict)
         ret_lmfit_result = fit_result # for return class below
```

### Comparing `cfpack-0.1.6/cfpack/automator.py` & `cfpack-0.1.7/cfpack/automator.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.6/cfpack/browser_control.py` & `cfpack-0.1.7/cfpack/browser_control.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.6/cfpack/constants.py` & `cfpack-0.1.7/cfpack/constants.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.6/cfpack/hdfio.py` & `cfpack-0.1.7/cfpack/hdfio.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.6/cfpack/matplotlibrc.py` & `cfpack-0.1.7/cfpack/matplotlibrc.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,11 +32,13 @@
 rcParams['ytick.minor.pad'] = 5
 # legend
 rcParams['legend.fontsize'] = rcParams['font.size']
 rcParams['legend.labelspacing'] = 0.2
 rcParams['legend.loc'] = 'upper left'
 rcParams['legend.frameon'] = False
 # figure
-rcParams['figure.figsize'] = (8.0, 5.0)
+rcParams['figure.figsize'] = (7.0, 4.5)
 rcParams['figure.dpi'] = 150
 rcParams['savefig.dpi'] = 200
 rcParams['savefig.bbox'] = 'tight'
+# errorbars
+rcParams['errorbar.capsize'] = 1.5
```

### Comparing `cfpack-0.1.6/cfpack/tests.py` & `cfpack-0.1.7/cfpack/tests.py`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.6/LICENSE` & `cfpack-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cfpack-0.1.6/pyproject.toml` & `cfpack-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfpack"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Christoph Federrath", email="christoph.federrath@anu.edu.au" },
 ]
 description = "Christoph Federrath (CF) python package (cfpack)"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3"
```

### Comparing `cfpack-0.1.6/PKG-INFO` & `cfpack-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cfpack
-Version: 0.1.6
+Version: 0.1.7
 Summary: Christoph Federrath (CF) python package (cfpack)
 Project-URL: Homepage, https://www.mso.anu.edu.au/~chfeder/codes/cfpack/cfpack.html
 Author-email: Christoph Federrath <christoph.federrath@anu.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Christoph Federrath
```

