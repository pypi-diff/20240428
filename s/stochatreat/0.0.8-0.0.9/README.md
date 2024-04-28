# Comparing `tmp/stochatreat-0.0.8.tar.gz` & `tmp/stochatreat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\stochatreat-0.0.8.tar", last modified: Wed Jul 24 13:24:54 2019, max compression
+gzip compressed data, was "stochatreat-0.0.9.tar", last modified: Fri Jul  9 01:05:36 2021, max compression
```

## Comparing `stochatreat-0.0.8.tar` & `stochatreat-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2019-07-24 13:24:54.000000 stochatreat-0.0.8/
--rw-rw-rw-   0        0        0     1093 2018-12-08 16:12:49.000000 stochatreat-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       17 2019-07-16 14:08:23.000000 stochatreat-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4410 2019-07-24 13:24:54.000000 stochatreat-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3201 2019-07-15 20:23:28.000000 stochatreat-0.0.8/README.md
--rw-rw-rw-   0        0        0       81 2019-07-24 13:24:54.000000 stochatreat-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1379 2019-07-17 13:36:26.000000 stochatreat-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2019-07-24 13:24:54.000000 stochatreat-0.0.8/stochatreat/
--rw-rw-rw-   0        0        0      409 2019-07-24 13:24:09.000000 stochatreat-0.0.8/stochatreat/__init__.py
--rw-rw-rw-   0        0        0    10089 2019-07-24 13:23:51.000000 stochatreat-0.0.8/stochatreat/stochatreat.py
--rw-rw-rw-   0        0        0      573 2019-07-19 14:43:05.000000 stochatreat-0.0.8/stochatreat/utils.py
-drwxrwxrwx   0        0        0        0 2019-07-24 13:24:54.000000 stochatreat-0.0.8/stochatreat.egg-info/
--rw-rw-rw-   0        0        0     4410 2019-07-24 13:24:54.000000 stochatreat-0.0.8/stochatreat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2019-07-24 13:24:54.000000 stochatreat-0.0.8/stochatreat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-07-24 13:24:54.000000 stochatreat-0.0.8/stochatreat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2019-07-24 13:24:54.000000 stochatreat-0.0.8/stochatreat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2019-07-24 13:24:54.000000 stochatreat-0.0.8/stochatreat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-07-09 01:05:36.641057 stochatreat-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2018-12-08 16:12:49.000000 stochatreat-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       17 2019-07-16 14:08:23.000000 stochatreat-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4646 2021-07-09 01:05:36.641057 stochatreat-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3282 2021-07-09 01:01:56.000000 stochatreat-0.0.9/README.md
+-rw-rw-rw-   0        0        0      123 2021-07-09 01:05:36.643059 stochatreat-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1721 2021-07-09 01:04:56.000000 stochatreat-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-07-09 01:05:36.631059 stochatreat-0.0.9/stochatreat/
+-rw-rw-rw-   0        0        0      347 2021-07-09 01:01:56.000000 stochatreat-0.0.9/stochatreat/__init__.py
+-rw-rw-rw-   0        0        0    10102 2021-07-09 01:01:56.000000 stochatreat-0.0.9/stochatreat/stochatreat.py
+-rw-rw-rw-   0        0        0      658 2021-07-09 01:01:56.000000 stochatreat-0.0.9/stochatreat/utils.py
+drwxrwxrwx   0        0        0        0 2021-07-09 01:05:36.640061 stochatreat-0.0.9/stochatreat.egg-info/
+-rw-rw-rw-   0        0        0     4646 2021-07-09 01:05:36.000000 stochatreat-0.0.9/stochatreat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2021-07-09 01:05:36.000000 stochatreat-0.0.9/stochatreat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-07-09 01:05:36.000000 stochatreat-0.0.9/stochatreat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2021-07-09 01:05:36.000000 stochatreat-0.0.9/stochatreat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2021-07-09 01:05:36.000000 stochatreat-0.0.9/stochatreat.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `stochatreat-0.0.8/LICENSE` & `stochatreat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stochatreat-0.0.8/PKG-INFO` & `stochatreat-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,102 +1,114 @@
 Metadata-Version: 2.1
 Name: stochatreat
-Version: 0.0.8
-Summary: Randomized block assignment using pandas
+Version: 0.0.9
+Summary: Stratified random assignment using pandas
 Home-page: https://github.com/manmartgarc/stochatreat
 Author: Manuel Martinez
 Author-email: manmartgarc@gmail.com
 License: UNKNOWN
 Description: # Stochatreat
+        
         ## Introduction
+        
         This is a Python module to employ block randomization using pandas. Mainly thought with RCTs in mind, it also works for any other scenario in where you would like to randomly allocate treatment within *blocks* or *strata*.
         
         ## Installation
-        ```
-        pip install stochatreat
+        
+        ```bash
+        pip install stochatreat$$
         ```
         
         ## Usage
+        
         Single cluster:
+        
         ```python
         from stochatreat import stochatreat
         import numpy as np
         import pandas as pd
         
         # make 1000 households in 5 different neighborhoods.
         np.random.seed(42)
-        df = pd.DataFrame(data={'id': list(range(1000)),
-                                'nhood': np.random.randint(1, 6, size=1000)})
+        df = pd.DataFrame(
+              data={'id': list(range(1000)),
+              'nhood': np.random.randint(1, 6, size=1000)})
         
         # randomly assign treatments by neighborhoods.
-        treats = stochatreat(data=df,              # your dataframe
-                             block_cols='nhood',   # the blocking variable
-                             treats=2,             # including control
-                             idx_col='id',         # the unique id column
-                             random_state=42)
+        treats = stochatreat(
+              data=df,                      # your dataframe
+              stratum_cols='nhood',         # the blocking variable
+              treats=2,                     # including control
+              idx_col='id',                 # the unique id column
+              random_state=42,              # random seed
+              misfit_strategy='stratum')    # the misfit strategy to use
         # merge back with original data
         df = df.merge(treats, how='left', on='id')
         
         # check for allocations
         df.groupby('nhood')['treat'].value_counts().unstack()
         
         # previous code should return this
-        treat  0.0  1.0
-        nhood          
+        treat    0    1
+        nhood
         1      105  105
         2       95   95
         3       95   95
         4      103  103
         5      102  102
         ```
         
         Multiple clusters and treatment probabilities:
+        
         ```python
         from stochatreat import stochatreat
         import numpy as np
         import pandas as pd
         
         # make 1000 households in 5 different neighborhoods, with a dummy indicator
         np.random.seed(42)
         df = pd.DataFrame(data={'id': list(range(1000)),
                                 'nhood': np.random.randint(1, 6, size=1000),
                                 'dummy': np.random.randint(0, 2, size=1000)})
         
         # randomly assign treatments by neighborhoods and dummy status.
         treats = stochatreat(data=df,
-                             block_cols=['nhood', 'dummy'],
+                             stratum_cols=['nhood', 'dummy'],
                              treats=2,
                              probs=[1/3, 2/3],
                              idx_col='id',
-                             random_state=42)
+                             random_state=42,
+                             misfit_strategy='global')
         # merge back with original data
         df = df.merge(treats, how='left', on='id')
         
         # check for allocations
         df.groupby(['nhood', 'dummy'])['treat'].value_counts().unstack()
         
         # previous code should return this
-        treat        0.0  1.0
-        nhood dummy          
-        1     0       38   74
-              1       33   65
-        2     0       35   69
-              1       29   57
-        3     0       30   58
-              1       34   68
-        4     0       36   72
-              1       33   65
-        5     0       34   67
-              1       35   68
+        treat         0   1
+        nhood dummy
+        1     0      37  75
+              1      33  65
+        2     0      35  69
+              1      29  57
+        3     0      30  58
+              1      34  68
+        4     0      36  72
+              1      32  66
+        5     0      33  68
+              1      35  68
         ```
         
         ## Acknowledgments
-        - `stochatreat` is totally inspired by [Alvaro Carril's](https://acarril.github.io/) fantastic Stata package: [`randtreat`](https://acarril.github.io/posts/randtreat), which was published in [The Stata Journal](https://www.stata-journal.com/article.html?article=st0490) :trumpet:.
+        
+        - `stochatreat` is totally inspired by [Alvaro Carril's](https://acarril.github.io/) fantastic Stata package: [`randtreat`](https://acarril.github.io/posts/randtreat), which was published in [The Stata Journal](https://www.stata-journal.com/article.html?article=st0490).
         - [David McKenzie's](http://blogs.worldbank.org/impactevaluations/tools-of-the-trade-doing-stratified-randomization-with-uneven-numbers-in-some-strata) fantastic post (and blog) about running RCTs for the World Bank.
         - [*In Pursuit of Balance: Randomization in Practice in Development Field Experiments.* Bruhn, McKenzie, 2009](https://www.aeaweb.org/articles?id=10.1257/app.1.4.200)
         
-Keywords: randomization,block randomization
+Keywords: randomization,block randomization,stratified randomizationstratified,strata
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stochatreat-0.0.8/README.md` & `stochatreat-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,98 @@
 # Stochatreat
+
 ## Introduction
+
 This is a Python module to employ block randomization using pandas. Mainly thought with RCTs in mind, it also works for any other scenario in where you would like to randomly allocate treatment within *blocks* or *strata*.
 
 ## Installation
-```
-pip install stochatreat
+
+```bash
+pip install stochatreat$$
 ```
 
 ## Usage
+
 Single cluster:
+
 ```python
 from stochatreat import stochatreat
 import numpy as np
 import pandas as pd
 
 # make 1000 households in 5 different neighborhoods.
 np.random.seed(42)
-df = pd.DataFrame(data={'id': list(range(1000)),
-                        'nhood': np.random.randint(1, 6, size=1000)})
+df = pd.DataFrame(
+      data={'id': list(range(1000)),
+      'nhood': np.random.randint(1, 6, size=1000)})
 
 # randomly assign treatments by neighborhoods.
-treats = stochatreat(data=df,              # your dataframe
-                     block_cols='nhood',   # the blocking variable
-                     treats=2,             # including control
-                     idx_col='id',         # the unique id column
-                     random_state=42)
+treats = stochatreat(
+      data=df,                      # your dataframe
+      stratum_cols='nhood',         # the blocking variable
+      treats=2,                     # including control
+      idx_col='id',                 # the unique id column
+      random_state=42,              # random seed
+      misfit_strategy='stratum')    # the misfit strategy to use
 # merge back with original data
 df = df.merge(treats, how='left', on='id')
 
 # check for allocations
 df.groupby('nhood')['treat'].value_counts().unstack()
 
 # previous code should return this
-treat  0.0  1.0
-nhood          
+treat    0    1
+nhood
 1      105  105
 2       95   95
 3       95   95
 4      103  103
 5      102  102
 ```
 
 Multiple clusters and treatment probabilities:
+
 ```python
 from stochatreat import stochatreat
 import numpy as np
 import pandas as pd
 
 # make 1000 households in 5 different neighborhoods, with a dummy indicator
 np.random.seed(42)
 df = pd.DataFrame(data={'id': list(range(1000)),
                         'nhood': np.random.randint(1, 6, size=1000),
                         'dummy': np.random.randint(0, 2, size=1000)})
 
 # randomly assign treatments by neighborhoods and dummy status.
 treats = stochatreat(data=df,
-                     block_cols=['nhood', 'dummy'],
+                     stratum_cols=['nhood', 'dummy'],
                      treats=2,
                      probs=[1/3, 2/3],
                      idx_col='id',
-                     random_state=42)
+                     random_state=42,
+                     misfit_strategy='global')
 # merge back with original data
 df = df.merge(treats, how='left', on='id')
 
 # check for allocations
 df.groupby(['nhood', 'dummy'])['treat'].value_counts().unstack()
 
 # previous code should return this
-treat        0.0  1.0
-nhood dummy          
-1     0       38   74
-      1       33   65
-2     0       35   69
-      1       29   57
-3     0       30   58
-      1       34   68
-4     0       36   72
-      1       33   65
-5     0       34   67
-      1       35   68
+treat         0   1
+nhood dummy
+1     0      37  75
+      1      33  65
+2     0      35  69
+      1      29  57
+3     0      30  58
+      1      34  68
+4     0      36  72
+      1      32  66
+5     0      33  68
+      1      35  68
 ```
 
 ## Acknowledgments
-- `stochatreat` is totally inspired by [Alvaro Carril's](https://acarril.github.io/) fantastic Stata package: [`randtreat`](https://acarril.github.io/posts/randtreat), which was published in [The Stata Journal](https://www.stata-journal.com/article.html?article=st0490) :trumpet:.
+
+- `stochatreat` is totally inspired by [Alvaro Carril's](https://acarril.github.io/) fantastic Stata package: [`randtreat`](https://acarril.github.io/posts/randtreat), which was published in [The Stata Journal](https://www.stata-journal.com/article.html?article=st0490).
 - [David McKenzie's](http://blogs.worldbank.org/impactevaluations/tools-of-the-trade-doing-stratified-randomization-with-uneven-numbers-in-some-strata) fantastic post (and blog) about running RCTs for the World Bank.
 - [*In Pursuit of Balance: Randomization in Practice in Development Field Experiments.* Bruhn, McKenzie, 2009](https://www.aeaweb.org/articles?id=10.1257/app.1.4.200)
```

### Comparing `stochatreat-0.0.8/stochatreat/stochatreat.py` & `stochatreat-0.0.9/stochatreat/stochatreat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # -*- coding: utf-8 -*-
 """
-Created on Thu Nov  8 14:34:47 2018
-
+Created on Thursday, 8th November 2018 2:34:47 pm
 ===============================================================================
-@author:    Manuel Martinez
+@filename:  stochatreat.py
+@author:    Manuel Martinez (manmartgarc@gmail.com)
 @project:   stochatreat
 @purpose:   Define a function that assign treatments over an arbitrary
             number of strata.
 ===============================================================================
 """
-from typing import List
+from typing import List, Optional
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 
 from .utils import get_lcm_prob_denominators
 
-# %%===========================================================================
-# Main
-# =============================================================================
-
 
 def stochatreat(data: pd.DataFrame,
                 stratum_cols: List[str],
                 treats: int,
-                probs: List[float] = [None],
+                probs: Optional[List[float]] = None,
                 random_state: int = 42,
                 idx_col: str = None,
                 size: int = None,
                 misfit_strategy: str = "stratum"
                 ) -> pd.DataFrame:
     """
     Takes a dataframe and an arbitrary number of treatments over an
@@ -41,32 +37,32 @@
     Parameters
     ----------
     data            :   The data that contains unique ids and the
                         stratification columns.
     stratum_cols    :   The columns in 'data' that you want to stratify over.
     treats          :   The number of treatments you would like to
                         implement, including control.
-    probs           :   The assignment probabilities for each of the 
+    probs           :   The assignment probabilities for each of the
                         treatments.
     random_state    :   The seed for the rng instance.
     idx_col         :   The column name that indicates the ids for your data.
     size            :   The size of the sample if you would like to sample
                         from your data.
-    misfit_strategy :   The strategy used to assign misfits. Can be one of 
+    misfit_strategy :   The strategy used to assign misfits. Can be one of
                         'stratum' or 'global'.
                         If 'stratum', will assign misfits randomly and
                         independently within each stratum using probs.
-                        If 'global', will group all misfits into one stratum 
-                        and do a full assignment procedure in this new stratum 
-                        with local random assignments of the misfits in this 
+                        If 'global', will group all misfits into one stratum
+                        and do a full assignment procedure in this new stratum
+                        with local random assignments of the misfits in this
                         stratum
 
     Returns
     -------
-    pandas.DataFrame with idx_col, treat (treatment assignments) and 
+    pandas.DataFrame with idx_col, treat (treatment assignments) and
     stratum_id (the id of the stratum within which the assignment procedure
     was carried out) columns
 
     Usage
     -----
     Single stratum:
         >>> treats = stochatreat(data=data,               # your dataframe
@@ -81,86 +77,86 @@
                                  stratum_cols=['stratum1', 'stratum2'],
                                  treats=2,
                                  probs=[1/3, 2/3],
                                  idx_col='myid',
                                  random_state=42)
         >>> data = data.merge(treats, how='left', on='myid')
     """
+    # pylint: disable=invalid-name
     R = np.random.RandomState(random_state)
 
     # =========================================================================
     # do checks
     # =========================================================================
     data = data.copy()
 
     # create treatment array and probability array
     treatment_ids = list(range(treats))
     # if no probabilities stated
-    if probs == [None]:
+    if probs is None:
         frac = 1 / len(treatment_ids)
-        probs = np.array([frac] * len(treatment_ids))
-    elif probs != [None]:
-        probs = np.array(probs)
-        if probs.sum() != 1:
+        probs_np = np.array([frac] * len(treatment_ids))
+    elif probs is not None:
+        probs_np = np.array(probs)
+        if probs_np.sum() != 1:
             raise ValueError('The probabilities must add up to 1')
 
     assertmsg = 'length of treatments and probs must be the same'
-    assert len(treatment_ids) == len(probs), assertmsg
+    assert len(treatment_ids) == len(probs_np), assertmsg
 
     # check if dataframe is empty
     if data.empty:
         raise ValueError('Make sure that your dataframe is not empty.')
 
     # check length of data
-    if len(data) < 1:
+    if len(data) < 2:
         raise ValueError('Make sure your data has enough observations.')
 
     # if idx_col parameter was not defined.
     if idx_col is None:
         data = data.rename_axis('index', axis='index').reset_index()
         idx_col = 'index'
-    elif type(idx_col) is not str:
+    elif not isinstance(idx_col, str):
         raise TypeError('idx_col has to be a string.')
-    
+
     # retrieve type to check and re-assign in the end
     idx_col_type = data[idx_col].dtype
 
     # check for unique identifiers
     if data[idx_col].duplicated(keep=False).sum() > 0:
         raise ValueError('Values in idx_col are not unique.')
 
     # if size is larger than sample universe
     if size is not None and size > len(data):
         raise ValueError('Size argument is larger than the sample universe.')
 
     # deal with multiple strata
-    if type(stratum_cols) is str:
+    if isinstance(stratum_cols, str):
         stratum_cols = [stratum_cols]
 
     if misfit_strategy not in ('stratum', 'global'):
         raise ValueError("the strategy must be one of 'stratum' or 'global'")
 
     # sort data - useful to preserve correspondence between `idx_col` and
     # assignments
     data = data.sort_values(by=idx_col)
 
     # combine strata cells - by assigning stratum ids
     data['stratum_id'] = data.groupby(stratum_cols).ngroup()
 
     # keep only ids and concatenated strata
     data = data[[idx_col] + ['stratum_id']].copy()
-    
+
     # apply weights to each stratum if sampling is wanted
     if size is not None:
         size = int(size)
         # get sampling weights
         strata_fracs = (data['stratum_id']
-            .value_counts(normalize=True)
-            .sort_index()
-        )
+                        .value_counts(normalize=True)
+                        .sort_index())
         reduced_sizes = (strata_fracs * size).round().astype(int)
         # draw sample
         data = data.groupby('stratum_id').apply(
             lambda x: x.sample(
                 n=reduced_sizes[x.name],
                 random_state=random_state
             )
@@ -172,22 +168,22 @@
     # 1. In as far as units can be neatly divided in the proportions given by
     #    prob they are so divided.
     # 2. Any leftovers ("misfits") are dealt with using either of the methods
     #    described in the docstring
 
     # 1. determine how to divide cleanly as much as possible
 
-    # convert all probs to fractions and get the lowest common multiple of 
+    # convert all probs to fractions and get the lowest common multiple of
     # their denominators
-    lcm_prob_denominators = get_lcm_prob_denominators(probs)
+    lcm_prob_denominators = get_lcm_prob_denominators(probs_np)
 
-    # produce the assignment mask that we will use to achieve perfect 
+    # produce the assignment mask that we will use to achieve perfect
     # proportions
     treat_mask = np.repeat(
-        treatment_ids, (lcm_prob_denominators*probs).astype(int)
+        treatment_ids, (lcm_prob_denominators*probs_np).astype(int)
     )
 
     # =========================================================================
     # re-arrange strata
     # =========================================================================
 
     if misfit_strategy == 'global':
@@ -204,53 +200,46 @@
         # assign the misfits their own stratum and concatenate
         misfit_data.loc[:, 'stratum_id'] = np.Inf
         data = pd.concat([good_form_data, misfit_data])
 
     # =========================================================================
     # assign treatments
     # =========================================================================
-    
+
     # sort by strata first, and assign a long list of permuted `treat_mask` to
     # deal with misfits, we add fake rows to each stratum so that its length is
-    # divisible by `lcm_prob_denominators` and toss them later 
+    # divisible by `lcm_prob_denominators` and toss them later
     # -> no costly apply inside the strata
 
     # add fake rows for each stratum so the total number can be divided by
     # `lcm_prob_denominators`
-    fake = pd.DataFrame(
-        {'fake': data.groupby('stratum_id').size()}
-    ).reset_index()  
-    fake.loc[:, 'fake'] = (
-        (lcm_prob_denominators - fake['fake'] % lcm_prob_denominators) % 
-            lcm_prob_denominators
-    )
-    fake_rep = pd.DataFrame(
-        fake.values.repeat(fake['fake'], axis=0), 
-        columns=fake.columns
-    )
+    fake = pd.DataFrame({'fake': data.groupby('stratum_id').size()})
+    fake = fake.reset_index()
+    fake.loc[:, 'fake'] = ((lcm_prob_denominators
+                            - fake['fake'] % lcm_prob_denominators)
+                           % lcm_prob_denominators)
+    fake_rep = pd.DataFrame(fake.values.repeat(fake['fake'], axis=0),
+                            columns=fake.columns)
 
     data.loc[:, 'fake'] = False
     fake_rep.loc[:, 'fake'] = True
 
-    data = (pd.concat([data, fake_rep], sort=False)
-        .sort_values(['stratum_id'])
-    )
+    data = pd.concat([data, fake_rep], sort=False).sort_values(by='stratum_id')
 
     # generate random permutations without loop by generating large number of
     # random values and sorting row (meaning one permutation) wise
-    permutations = np.argsort(
-        R.rand(len(data) // lcm_prob_denominators, lcm_prob_denominators),
-        axis=1
-    )
+    permutations = np.argsort(R.rand(len(data) // lcm_prob_denominators,
+                                     lcm_prob_denominators),
+                              axis=1)
     # lookup treatment name for permutations. This works because we flatten
     # row-major style, i.e. one row after another.
     data.loc[:, 'treat'] = treat_mask[permutations].flatten(order='C')
     data = data[~data['fake']].drop(columns=['fake'])
 
     # re-assign type - as it might have changed with the addition of fake data
     data.loc[:, idx_col] = data[idx_col].astype(idx_col_type)
-    
+
     data.loc[:, 'treat'] = data['treat'].astype(np.int64)
 
     assert data['treat'].isnull().sum() == 0
-    
+
     return data
```

### Comparing `stochatreat-0.0.8/stochatreat/utils.py` & `stochatreat-0.0.9/stochatreat/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-from math import gcd
 from fractions import Fraction
 from functools import reduce
+from math import gcd
+from typing import Iterable
 
-def lcm(ints):
-    """Helper function to compute the Lowest Common Multiple of a list of integers"""
+
+def lcm(ints: Iterable[int]):
+    """
+    Helper function to compute the Lowest Common Multiple of a list of integers
+    """
     return reduce(lambda a, b: a * b // gcd(a, b), ints)
 
 
-def get_lcm_prob_denominators(probs):
-    """Helper function to compute the LCM of the denominators of the probabilities"""
+def get_lcm_prob_denominators(probs: Iterable[float]):
+    """
+    Helper function to compute the LCM of the denominators of the probabilities
+    """
     prob_denominators = [
         Fraction(prob).limit_denominator().denominator for prob in probs
     ]
     lcm_prob_denominators = lcm(prob_denominators)
     return lcm_prob_denominators
-
```

### Comparing `stochatreat-0.0.8/stochatreat.egg-info/PKG-INFO` & `stochatreat-0.0.9/stochatreat.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,102 +1,114 @@
 Metadata-Version: 2.1
 Name: stochatreat
-Version: 0.0.8
-Summary: Randomized block assignment using pandas
+Version: 0.0.9
+Summary: Stratified random assignment using pandas
 Home-page: https://github.com/manmartgarc/stochatreat
 Author: Manuel Martinez
 Author-email: manmartgarc@gmail.com
 License: UNKNOWN
 Description: # Stochatreat
+        
         ## Introduction
+        
         This is a Python module to employ block randomization using pandas. Mainly thought with RCTs in mind, it also works for any other scenario in where you would like to randomly allocate treatment within *blocks* or *strata*.
         
         ## Installation
-        ```
-        pip install stochatreat
+        
+        ```bash
+        pip install stochatreat$$
         ```
         
         ## Usage
+        
         Single cluster:
+        
         ```python
         from stochatreat import stochatreat
         import numpy as np
         import pandas as pd
         
         # make 1000 households in 5 different neighborhoods.
         np.random.seed(42)
-        df = pd.DataFrame(data={'id': list(range(1000)),
-                                'nhood': np.random.randint(1, 6, size=1000)})
+        df = pd.DataFrame(
+              data={'id': list(range(1000)),
+              'nhood': np.random.randint(1, 6, size=1000)})
         
         # randomly assign treatments by neighborhoods.
-        treats = stochatreat(data=df,              # your dataframe
-                             block_cols='nhood',   # the blocking variable
-                             treats=2,             # including control
-                             idx_col='id',         # the unique id column
-                             random_state=42)
+        treats = stochatreat(
+              data=df,                      # your dataframe
+              stratum_cols='nhood',         # the blocking variable
+              treats=2,                     # including control
+              idx_col='id',                 # the unique id column
+              random_state=42,              # random seed
+              misfit_strategy='stratum')    # the misfit strategy to use
         # merge back with original data
         df = df.merge(treats, how='left', on='id')
         
         # check for allocations
         df.groupby('nhood')['treat'].value_counts().unstack()
         
         # previous code should return this
-        treat  0.0  1.0
-        nhood          
+        treat    0    1
+        nhood
         1      105  105
         2       95   95
         3       95   95
         4      103  103
         5      102  102
         ```
         
         Multiple clusters and treatment probabilities:
+        
         ```python
         from stochatreat import stochatreat
         import numpy as np
         import pandas as pd
         
         # make 1000 households in 5 different neighborhoods, with a dummy indicator
         np.random.seed(42)
         df = pd.DataFrame(data={'id': list(range(1000)),
                                 'nhood': np.random.randint(1, 6, size=1000),
                                 'dummy': np.random.randint(0, 2, size=1000)})
         
         # randomly assign treatments by neighborhoods and dummy status.
         treats = stochatreat(data=df,
-                             block_cols=['nhood', 'dummy'],
+                             stratum_cols=['nhood', 'dummy'],
                              treats=2,
                              probs=[1/3, 2/3],
                              idx_col='id',
-                             random_state=42)
+                             random_state=42,
+                             misfit_strategy='global')
         # merge back with original data
         df = df.merge(treats, how='left', on='id')
         
         # check for allocations
         df.groupby(['nhood', 'dummy'])['treat'].value_counts().unstack()
         
         # previous code should return this
-        treat        0.0  1.0
-        nhood dummy          
-        1     0       38   74
-              1       33   65
-        2     0       35   69
-              1       29   57
-        3     0       30   58
-              1       34   68
-        4     0       36   72
-              1       33   65
-        5     0       34   67
-              1       35   68
+        treat         0   1
+        nhood dummy
+        1     0      37  75
+              1      33  65
+        2     0      35  69
+              1      29  57
+        3     0      30  58
+              1      34  68
+        4     0      36  72
+              1      32  66
+        5     0      33  68
+              1      35  68
         ```
         
         ## Acknowledgments
-        - `stochatreat` is totally inspired by [Alvaro Carril's](https://acarril.github.io/) fantastic Stata package: [`randtreat`](https://acarril.github.io/posts/randtreat), which was published in [The Stata Journal](https://www.stata-journal.com/article.html?article=st0490) :trumpet:.
+        
+        - `stochatreat` is totally inspired by [Alvaro Carril's](https://acarril.github.io/) fantastic Stata package: [`randtreat`](https://acarril.github.io/posts/randtreat), which was published in [The Stata Journal](https://www.stata-journal.com/article.html?article=st0490).
         - [David McKenzie's](http://blogs.worldbank.org/impactevaluations/tools-of-the-trade-doing-stratified-randomization-with-uneven-numbers-in-some-strata) fantastic post (and blog) about running RCTs for the World Bank.
         - [*In Pursuit of Balance: Randomization in Practice in Development Field Experiments.* Bruhn, McKenzie, 2009](https://www.aeaweb.org/articles?id=10.1257/app.1.4.200)
         
-Keywords: randomization,block randomization
+Keywords: randomization,block randomization,stratified randomizationstratified,strata
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

