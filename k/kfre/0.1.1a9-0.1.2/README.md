# Comparing `tmp/kfre-0.1.1a9.tar.gz` & `tmp/kfre-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kfre-0.1.1a9.tar", last modified: Fri Apr 26 19:24:08 2024, max compression
+gzip compressed data, was "dist\kfre-0.1.2.tar", last modified: Sun Apr 28 01:16:20 2024, max compression
```

## Comparing `kfre-0.1.1a9.tar` & `kfre-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 19:24:08.715963 kfre-0.1.1a9/
--rw-rw-rw-   0        0        0     5070 2024-04-26 19:24:08.715963 kfre-0.1.1a9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-26 19:24:08.716962 kfre-0.1.1a9/setup.cfg
--rw-rw-rw-   0        0        0     1380 2024-04-26 19:23:45.000000 kfre-0.1.1a9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:24:08.683394 kfre-0.1.1a9/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 19:24:08.693979 kfre-0.1.1a9/src/kfre/
--rw-rw-rw-   0        0        0       55 2024-04-26 04:56:44.000000 kfre-0.1.1a9/src/kfre/__init__.py
--rw-rw-rw-   0        0        0    17849 2024-04-26 19:21:47.000000 kfre-0.1.1a9/src/kfre/main.py
-drwxrwxrwx   0        0        0        0 2024-04-26 19:24:08.714981 kfre-0.1.1a9/src/kfre.egg-info/
--rw-rw-rw-   0        0        0     5070 2024-04-26 19:24:08.000000 kfre-0.1.1a9/src/kfre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-04-26 19:24:08.000000 kfre-0.1.1a9/src/kfre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 19:24:08.000000 kfre-0.1.1a9/src/kfre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-04-26 19:24:08.000000 kfre-0.1.1a9/src/kfre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 19:24:08.000000 kfre-0.1.1a9/src/kfre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.129324 kfre-0.1.2/
+-rw-rw-rw-   0        0        0    28206 2024-04-28 01:16:20.128262 kfre-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    24261 2024-04-28 01:16:09.000000 kfre-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-28 01:16:20.129324 kfre-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2024-04-28 01:08:27.000000 kfre-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.088129 kfre-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.090130 kfre-0.1.2/src/kfre/
+-rw-rw-rw-   0        0        0     1872 2024-04-28 00:46:44.000000 kfre-0.1.2/src/kfre/__init__.py
+-rw-rw-rw-   0        0        0    26880 2024-04-28 00:46:36.000000 kfre-0.1.2/src/kfre/main.py
+drwxrwxrwx   0        0        0        0 2024-04-28 01:16:20.127135 kfre-0.1.2/src/kfre.egg-info/
+-rw-rw-rw-   0        0        0    28206 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-28 01:16:20.000000 kfre-0.1.2/src/kfre.egg-info/top_level.txt
```

### Comparing `kfre-0.1.1a9/setup.py` & `kfre-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="kfre",
-    version="0.1.1-alpha9",
+    version="0.1.2",
     author="Leonid Shpaner",
     author_email="Lshpaner@ucla.edu",
     description="A Python library for kidney failure risk estimation using Tangri's KFRE model",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",  # Type of the long description
-    url="https://github.com/lshpaner/kfre",  # URL to the repository or documentation
     package_dir={"": "src"},  # Directory where your package files are located
     # Automatically find packages in the specified directory
     packages=find_packages(where="src"),
     project_urls={  # Optional
         "Author Website": "https://www.leonshpaner.com",
         # "Documentation": "https://example.com/project-documentation",
         "Source Code": "https://github.com/lshpaner/kfre",
```

### Comparing `kfre-0.1.1a9/src/kfre/main.py` & `kfre-0.1.2/src/kfre/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 ################################################################################
 
 
 class RiskPredictor:
     """
     A class to represent a risk predictor for chronic kidney disease (CKD).
 
+    This class implements the Tangri risk prediction model, which is based on the
+    multinational assessments described in Tangri N, Grams ME, Levey AS, et al.
+    "Multinational assessment of accuracy of equations for predicting risk of kidney
+    failure: A meta-analysis." JAMA, 315(2), 164–174, doi: 10.1001/jama.2015.18202.
+
     This class uses the Tangri risk prediction model, which calculates risk
     based on various patient parameters. Results are accurate for both males
     and females, but the original paper calculated risk specifically for males.
 
     Attributes:
     data (DataFrame): The patient data.
     columns (dict): Dictionary to map expected parameter names to actual column
@@ -22,15 +27,15 @@
     Methods:
     predict(years, use_extra_vars): Predicts the risk of CKD for the given
     number of years, optionally using extra variables for the prediction.
     """
 
     def __init__(
         self,
-        data=None,
+        df=None,
         columns=None,
     ):
         """
         Constructs the necessary attributes for the RiskPredictor object.
 
         Parameters:
         data (DataFrame): The patient data.
@@ -38,58 +43,17 @@
         that correspond to the required parameters.
         Example: {'age': 'Age', 'sex': 'Gender', 'eGFR': 'eGFR',
         'uACR': 'Albumin_Ratio', 'region': 'Region', 'dm': 'Diabetes',
         'htn': 'Hypertension'}
         apply_conversions (bool, optional): Flag to apply unit conversions.
         Default is False.
         """
-        self.data = data
+        self.df = df
         self.columns = columns
 
-    def perform_conversions(self, reverse=False):
-        """
-        Applies or reverses unit conversions to the biochemical markers in the dataset.
-
-        Parameters:
-        - reverse (bool): If True, perform reverse conversions. Defaults to False.
-
-        Converts:
-        - uPCR from mmol to mg/g or vice versa
-        - Calcium from mmol to mg/dL or vice versa
-        - Phosphate from mmol to mg/dL or vice versa
-        - Albumin from g/L to g/dL or vice versa
-        """
-        if not reverse:
-            # Conversions from units in the dataset to standard units
-            # 0.11312 g creatinine/1 mg protein = 8.84
-            conversion_factor = 1 / 0.11312
-            self.data["uPCR (mg/g)"] = (
-                self.data[self.columns["uPCR_mmol"]] * conversion_factor
-            )
-            self.data["Calcium (mg/dL)"] = self.data[self.columns["calcium_mmol"]] * 4
-            self.data["Phosphate (mg/dL)"] = (
-                self.data[self.columns["phosphate_mmol"]] * 3.1
-            )
-            self.data["Albumin (g/dL)"] = (
-                self.data[self.columns["albumin_g_per_l"]] / 10
-            )
-        else:
-            # Reverse conversions from standard units back to units in the dataset
-            # 0.11312 g creatinine/1 mg protein = 8.84
-            self.data[self.columns["uPCR_mmol"]] = (
-                self.data["uPCR (mg/g)"] / conversion_factor
-            )
-            self.data[self.columns["calcium_mmol"]] = self.data["Calcium (mg/dL)"] / 4
-            self.data[self.columns["phosphate_mmol"]] = (
-                self.data["Phosphate (mg/dL)"] / 3.1
-            )
-            self.data[self.columns["albumin_g_per_l"]] = (
-                self.data["Albumin (g/dL)"] * 10
-            )
-
     def predict_kfre(
         self,
         years,
         is_north_american,
         use_extra_vars=False,
         num_vars=4,
     ):
@@ -133,52 +97,52 @@
             self.columns["age"],
             self.columns["sex"],
             self.columns["eGFR"],
             self.columns["uACR"],
         ]
 
         # Retrieve data only once
-        data = self.data[necessary_cols].copy()
+        df = self.df[necessary_cols].copy()
 
         # Convert sex to numeric in a vectorized way
-        data[self.columns["sex"]] = (
-            data[self.columns["sex"]].str.lower() == "male"
+        df[self.columns["sex"]] = (
+            df[self.columns["sex"]].str.lower() == "male"
         ).astype(int)
 
         # Extract basic parameters from the DataFrame
-        age = data[self.columns["age"]]
-        sex = data[self.columns["sex"]]
-        eGFR = data[self.columns["eGFR"]]
-        uACR = data[self.columns["uACR"]]
+        age = df[self.columns["age"]]
+        sex = df[self.columns["sex"]]
+        eGFR = df[self.columns["eGFR"]]
+        uACR = df[self.columns["uACR"]]
 
         if use_extra_vars:
             if num_vars == 6:
                 # Extend columns for 6-variable model
                 necessary_cols.extend([self.columns["dm"], self.columns["htn"]])
-                data = self.data[necessary_cols].copy()
-                dm = data[self.columns["dm"]]
-                htn = data[self.columns["htn"]]
+                df = self.df[necessary_cols].copy()
+                dm = df[self.columns["dm"]]
+                htn = df[self.columns["htn"]]
                 return risk_pred(
                     age, sex, eGFR, uACR, is_north_american, dm, htn, years=years
                 )
             elif num_vars == 8:
                 # Extend columns for 8-variable model
                 necessary_cols.extend(
                     [
                         self.columns["albumin"],
                         self.columns["phosphorous"],
                         self.columns["bicarbonate"],
                         self.columns["calcium"],
                     ]
                 )
-                data = self.data[necessary_cols].copy()
-                albumin = data[self.columns["albumin"]]
-                phosphorous = data[self.columns["phosphorous"]]
-                bicarbonate = data[self.columns["bicarbonate"]]
-                calcium = data[self.columns["calcium"]]
+                df = self.df[necessary_cols].copy()
+                albumin = df[self.columns["albumin"]]
+                phosphorous = df[self.columns["phosphorous"]]
+                bicarbonate = df[self.columns["bicarbonate"]]
+                calcium = df[self.columns["calcium"]]
                 return risk_pred(
                     age,
                     sex,
                     eGFR,
                     uACR,
                     is_north_american,
                     None,
@@ -250,67 +214,309 @@
 
 
 ################################################################################
 ################################ uPCR to uACR ##################################
 ################################################################################
 
 
-def upcr_uacr(
-    row,
-    sex_col,
-    diabetes_col,
-    hypertension_col,
-    upcr_col,
-    female_str,
-):
+def upcr_uacr(df, sex_col, diabetes_col, hypertension_col, upcr_col, female_str):
     """
     Converts urinary protein-creatinine ratio (uPCR) to urinary
-    albumin-creatinine ratio (uACR) using a specified formula that considers
-    patient demographics and conditions.
+    albumin-creatinine ratio (uACR) for an entire DataFrame using vectorized
+    operations to enhance performance. This function is designed to handle large
+    datasets efficiently by applying the conversion formula across columns,
+    rather than row-by-row.
+
+    The conversion uses patient-specific factors such as sex, presence of
+    diabetes, and presence of hypertension to adjust the uACR calculation
+    according to a specified logarithmic and exponential formula. This approach
+    is critical in clinical settings where accurate adjustments based on
+    demographic factors are essential for proper diagnosis and treatment planning.
 
     Parameters:
-    - row (pd.Series): A single row from a pandas DataFrame representing one
-      patient's data.
-    - sex_col (str): Column name containing the patient's gender.
-    - diabetes_col (str): Column name indicating whether the patient has
-      diabetes (1 for yes, 0 for no).
-    - hypertension_col (str): Column name indicating whether the patient has
-      hypertension (1 for yes, 0 for no).
-    - upcr_col (str): Column name containing the urinary protein-creatinine ratio.
-    - female_str (str): The exact string used in the dataset to identify a
-      patient as female, critical for accurate calculations.
+    - df (pd.DataFrame): The DataFrame containing the patient data.
+    - sex_col (str): Column name in 'df' that contains the patient's gender.
+    - diabetes_col (str): Column name in 'df' that indicates whether the
+      patient has diabetes (1=yes; 0=no).
+    - hypertension_col (str): Column name in 'df' that indicates whether the
+      patient has hypertension (1=yes; 0=no).
+    - upcr_col (str): Column name in 'df' that contains the urinary
+      protein-creatinine ratio.
+    - female_str (str): The string used in the dataset to identify female patients.
 
     Returns:
-    - float: The computed urinary albumin-creatinine ratio (uACR).
+    - pd.Series: A pandas Series object containing the computed urinary
+      albumin-creatinine ratio (uACR) for each patient in the DataFrame.
 
-    This function applies a complex logarithmic and exponential calculation to
-    derive the uACR from the uPCR, adjusting for factors such as gender,
-    diabetes, and hypertension status. The accuracy of the function relies on
-    the exact match of the 'female_str' with the dataset's representation of
-    female gender.
+    This function ensures that all calculations respect the integrity of the
+    original data by not modifying any existing columns and only adding the
+    resulting uACR as a new column. It handles NaN values by excluding them
+    from the calculation, thus retaining them in the resulting uACR values to
+    reflect the lack of information for certain patients.
 
     Notes: Conversion from uPCR to uACR can be independently verified using the
     calculator on `https://ckdpcrisk.org/pcr2acr/`
+
+    This function converts urine protein-creatinine ratio or urine dipstick
+    protein to urine albumin-creatinine ratio, based on the method outlined in
+    Sumida K, Nadkarni GN, Grams ME, et al. "Conversion of urine protein-creatinine
+    ratio or urine dipstick protein to urine albumin-creatinine ratio for use in
+    chronic kidney disease screening and prognosis."
+    Ann Intern Med, 173(6), 426-435, doi: 10.7326/M20-0529.
+
     """
-    upcr = row[upcr_col]
-    female = 1 if row[sex_col] == female_str else 0
-    diabetic = row[diabetes_col]
-    hypertensive = row[hypertension_col]
+    # Convert to float and get the female mask
+    upcr = df[upcr_col].astype(float)
+    female = (df[sex_col] == female_str).astype(int)
+
+    # Masks to identify valid data for diabetes and hypertension
+    diabetic_mask = ~df[diabetes_col].isna()
+    hypertensive_mask = ~df[hypertension_col].isna()
+
+    # Only calculate uACR where we have complete information
+    valid_mask = diabetic_mask & hypertensive_mask
 
-    # Applying the provided formula
-    uacr = np.exp(
+    # Initialize uACR with NaNs
+    uacr = np.full(df.shape[0], np.nan)
+
+    # Calculate uACR only for valid data
+    uacr[valid_mask] = np.exp(
         5.2659
-        + 0.2934 * np.log(np.minimum(upcr / 50, 1))
-        + 1.5643 * np.log(np.maximum(np.minimum(upcr / 500, 1), 0.1))
-        + 1.1109 * np.log(np.maximum(upcr / 500, 1))
-        - 0.0773 * female
-        + 0.0797 * diabetic
-        + 0.1265 * hypertensive
+        + 0.2934 * np.log(np.minimum(upcr[valid_mask] / 50, 1))
+        + 1.5643 * np.log(np.maximum(np.minimum(upcr[valid_mask] / 500, 1), 0.1))
+        + 1.1109 * np.log(np.maximum(upcr[valid_mask] / 500, 1))
+        - 0.0773 * female[valid_mask]
+        + 0.0797 * df[diabetes_col][valid_mask].astype(int)
+        + 0.1265 * df[hypertension_col][valid_mask].astype(int)
+    )
+
+    return pd.Series(uacr, index=df.index)
+
+
+################################################################################
+#################################  Wrappers  ###################################
+################################################################################
+
+
+# convenience function as wrapper for method with the same name
+def predict_kfre(
+    df, columns, years, is_north_american, use_extra_vars=False, num_vars=4
+):
+    """
+    A convenience function to predict CKD risk using the Tangri risk prediction
+    model without directly creating an instance of the RiskPredictor class.
+
+    Parameters:
+    - df (DataFrame): The DataFrame containing patient data.
+    - columns (dict): Maps clinical parameter names to DataFrame column names.
+    - years (int): Number of years for the risk prediction.
+    - is_north_american (bool): True if the data is from North America.
+    - use_extra_vars (bool): If True, use additional clinical variables for the
+      prediction.
+    - num_vars (int): Number of variables used in the model (4, 6, or 8).
+
+    Returns:
+    - Series: CKD risk probabilities for each patient.
+    """
+
+    predictor = RiskPredictor(df=df, columns=columns)
+    return predictor.predict_kfre(
+        years=years,
+        is_north_american=is_north_american,
+        use_extra_vars=use_extra_vars,
+        num_vars=num_vars,
+    )
+
+
+def add_kfre_risk_col(
+    df,
+    age_col=None,
+    sex_col=None,
+    eGFR_col=None,
+    uACR_col=None,
+    dm_col=None,
+    htn_col=None,
+    albumin_col=None,
+    phosphorous_col=None,
+    bicarbonate_col=None,
+    calcium_col=None,
+    num_vars=8,
+    years=(2, 5),
+    is_north_american=False,
+    copy=True,
+):
+    """
+    Calculate CKD risks for specified variable num_vars and time frames or for
+    all num_vars and years, grouping the results by model first and then by time
+    frame in the output DataFrame. Optionally creates a copy of the DataFrame to
+    avoid modifying the original data.
+
+    Parameters:
+    - df (DataFrame): The patient data.
+    - age_col, sex_col, ..., calcium_col (str): Column names for the patient
+      parameters.
+    - num_vars (int or list): Specifies the number of variables to use (4, 6, 8).
+    - years (tuple or list): Time frames to calculate risk for.
+    - is_north_american (bool): True if the calculation is for the North
+      American region.
+    - copy (bool): If True, operates on a copy of the DataFrame. If False,
+      modifies the DataFrame in place.
+
+    Returns:
+    - DataFrame: The modified or new DataFrame with added risk prediction columns.
+    """
+    # Use a copy if requested for safety
+    df_used = df.copy() if copy else df
+
+    column_map = {
+        "age": age_col,
+        "sex": sex_col,
+        "eGFR": eGFR_col,
+        "uACR": uACR_col,
+        "dm": dm_col,
+        "htn": htn_col,
+        "albumin": albumin_col,
+        "phosphorous": phosphorous_col,
+        "bicarbonate": bicarbonate_col,
+        "calcium": calcium_col,
+    }
+
+    model_requirements = {
+        4: ["age", "sex", "eGFR", "uACR"],
+        6: ["age", "sex", "eGFR", "uACR", "dm", "htn"],
+        8: [
+            "age",
+            "sex",
+            "eGFR",
+            "uACR",
+            "albumin",
+            "phosphorous",
+            "bicarbonate",
+            "calcium",
+        ],
+    }
+
+    # Adjust 'num_vars' and 'years' handling to accept 'all', integer, or iterable
+    num_vars = (
+        [4, 6, 8]
+        if num_vars == "all"
+        else ([num_vars] if isinstance(num_vars, int) else num_vars)
+    )
+    years = (
+        [2, 5]
+        if years == "all"
+        else ([years] if isinstance(years, int) else list(years))
     )
-    return uacr
+
+    for model in num_vars:
+        missing = [req for req in model_requirements[model] if column_map[req] is None]
+        if missing:
+            required_cols = ", ".join(missing)
+            raise ValueError(
+                f"{required_cols} needed to complete calculation for {model}var model"
+            )
+
+    # Initialize the predictor with the data and columns
+    predictor = RiskPredictor(
+        df_used, {k: v for k, v in column_map.items() if v is not None}
+    )
+
+    # Calculate risks for each model and time frame
+    for model_vars in num_vars:
+        if all(column_map[req] is not None for req in model_requirements[model_vars]):
+            for time_frame in years:
+                risk_column = f"kfre_{model_vars}var_{time_frame}year"
+                df_used[risk_column] = predictor.predict_kfre(
+                    years=time_frame,
+                    is_north_american=is_north_american,
+                    use_extra_vars=(model_vars > 4),
+                    num_vars=model_vars,
+                )
+
+    return df_used
+
+
+def perform_conversions(
+    df,
+    reverse=False,
+    convert_all=False,
+    upcr_col=None,
+    calcium_col=None,
+    phosphate_col=None,
+    albumin_col=None,
+):
+    """
+    Convert specified units of columns in a dataframe and create new columns
+    for the results, with specific suffixes based on the conversion direction.
+    Original columns are preserved.
+
+    Parameters:
+    - df (DataFrame): The dataframe containing the data.
+    - reverse (bool): If True, revert to original units by dividing; if False,
+      perform the standard conversion by multiplying.
+    - convert_all (bool): If True, automatically convert all recognized columns.
+    - upcr_col (str, optional): Column name for urine protein-creatinine ratio.
+    - calcium_col (str, optional): Column name for calcium.
+    - phosphate_col (str, optional): Column name for phosphate.
+    - albumin_col (str, optional): Column name for albumin.
+    """
+    # Define the conversion factors and the suffixes for the converted units
+    conversion_factors = {
+        "uPCR": 1 / 0.11312,  # From mg/g to mmol/L
+        "Calcium": 4,  # From mg/dL to mmol/L
+        "Phosphate": 3.1,  # From mg/dL to mmol/L
+        "Albumin": 1 / 10,  # From g/dL to g/L
+    }
+
+    # Define the suffixes for new column names based on conversion direction
+    conversion_suffix = {
+        "uPCR": "mg_g" if not reverse else "mmol_L",
+        "Calcium": "mg_dl" if not reverse else "mmol_L",
+        "Phosphate": "mg_dl" if not reverse else "mmol_L",
+        "Albumin": "g_dl" if not reverse else "g_L",
+    }
+
+    # Initialize columns_to_convert with provided column names or defaults
+    columns_to_convert = {
+        "uPCR": upcr_col,
+        "Calcium": calcium_col,
+        "Phosphate": phosphate_col,
+        "Albumin": albumin_col,
+    }
+
+    # If convert_all is True, automatically identify columns for conversion
+    if convert_all:
+        columns_to_convert = {
+            key: next((col for col in df.columns if key.lower() in col.lower()), None)
+            for key in conversion_factors
+        }
+
+    # Perform conversions
+    for key, orig_col in columns_to_convert.items():
+        if orig_col and orig_col in df.columns:
+            factor = conversion_factors[key]
+            suffix = conversion_suffix[key]
+            # Calculate the converted values
+            converted_values = (
+                df[orig_col] / factor if reverse else df[orig_col] * factor
+            )
+            # Create the new column name
+            new_col = f"{key}_{suffix}"
+            # Add the converted values as a new column to the dataframe
+            df[new_col] = converted_values
+            print(
+                f"Converted '{orig_col}' to new column '{new_col}' with factor {factor}"
+            )
+        else:
+            print(
+                f"Warning: Column '{orig_col}' not found in DataFrame. "
+                f"No conversion performed for this column."
+            )
+
+    return df
 
 
 ################################################################################
 ############################## KFRE Risk Predictor #############################
 ################################################################################
 
 
@@ -457,7 +663,28 @@
 
     # Select alpha based on region and years
     alpha = alpha_values[(is_north_american, years)]
 
     # Compute the risk prediction
     risk_prediction = 1 - alpha ** np.exp(risk_score)
     return risk_prediction
+
+
+################################################################################
+# References
+# ------------------------------------------------------------------------------
+#
+# Tangri N, Grams ME, Levey AS, Coresh J, et al. (2016). Multinational assessment
+# of accuracy of equations for predicting risk of kidney failure: A meta-analysis.
+# JAMA, 315(2), 164–174. doi: 10.1001/jama.2015.18202.
+#
+# Tangri, N., Stevens, L. A., Griffith, J., Tighiouart, H., Djurdjev, O.,
+# Naimark, D., Levin, A., & Levey, A. S. (2011). A predictive model for
+# progression of chronic kidney disease to kidney failure. JAMA, 305(15),
+# 1553-1559. doi: 10.1001/jama.2011.451.
+#
+# Sumida K, Nadkarni GN, Grams ME, Sang Y, et al. (2020). Conversion of urine
+# protein-creatinine ratio or urine dipstick protein to urine albumin-creatinine
+# ratio for use in chronic kidney disease screening and prognosis. Ann Intern Med,
+# 173(6), 426-435. doi: 10.7326/M20-0529.
+# ------------------------------------------------------------------------------
+################################################################################
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

