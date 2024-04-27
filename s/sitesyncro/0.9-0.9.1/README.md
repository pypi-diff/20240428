# Comparing `tmp/sitesyncro-0.9.tar.gz` & `tmp/sitesyncro-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesyncro-0.9.tar", last modified: Sun Apr 21 22:23:49 2024, max compression
+gzip compressed data, was "sitesyncro-0.9.1.tar", last modified: Sat Apr 27 09:03:44 2024, max compression
```

## Comparing `sitesyncro-0.9.tar` & `sitesyncro-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 22:23:49.235634 sitesyncro-0.9/
--rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9/LICENSE
--rw-rw-rw-   0        0        0    17806 2024-04-21 22:23:49.235634 sitesyncro-0.9/PKG-INFO
--rw-rw-rw-   0        0        0    16874 2024-04-21 21:46:02.000000 sitesyncro-0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 22:23:49.235634 sitesyncro-0.9/setup.cfg
--rw-rw-rw-   0        0        0     1710 2024-04-21 22:02:41.000000 sitesyncro-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:23:49.197885 sitesyncro-0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-21 22:23:49.197885 sitesyncro-0.9/src/sitesyncro/
--rw-rw-rw-   0        0        0     8319 2024-04-21 21:48:37.000000 sitesyncro-0.9/src/sitesyncro/SiteSyncro.py
--rw-rw-rw-   0        0        0      172 2024-04-21 21:49:10.000000 sitesyncro-0.9/src/sitesyncro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:23:49.235634 sitesyncro-0.9/src/sitesyncro/lib/
--rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9/src/sitesyncro/lib/__init__.py
--rw-rw-rw-   0        0        0     8539 2024-04-21 21:47:04.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_cluster.py
--rw-rw-rw-   0        0        0    12238 2024-04-21 16:38:02.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_data.py
--rw-rw-rw-   0        0        0     4217 2024-04-21 14:18:10.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_load.py
--rw-rw-rw-   0        0        0     1568 2022-05-26 16:44:35.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_mp.py
--rw-rw-rw-   0        0        0     7534 2024-04-21 21:47:14.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_oxcal.py
--rw-rw-rw-   0        0        0     6167 2024-04-21 14:37:26.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_phase.py
--rw-rw-rw-   0        0        0     5767 2024-04-21 16:34:31.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_plot.py
--rw-rw-rw-   0        0        0     7635 2024-04-21 21:47:26.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_process.py
--rw-rw-rw-   0        0        0     1464 2024-04-19 17:13:39.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_radiocarbon.py
--rw-rw-rw-   0        0        0     7465 2024-04-21 21:47:35.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_simulate.py
--rw-rw-rw-   0        0        0     3269 2024-04-20 09:08:14.000000 sitesyncro-0.9/src/sitesyncro/lib/fnc_sum.py
--rw-rw-rw-   0        0        0     1958 2024-04-21 21:48:02.000000 sitesyncro-0.9/src/sitesyncro/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 22:23:49.235634 sitesyncro-0.9/src/sitesyncro.egg-info/
--rw-rw-rw-   0        0        0    17806 2024-04-21 22:23:49.000000 sitesyncro-0.9/src/sitesyncro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      682 2024-04-21 22:23:49.000000 sitesyncro-0.9/src/sitesyncro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 22:23:49.000000 sitesyncro-0.9/src/sitesyncro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-04-21 22:23:49.000000 sitesyncro-0.9/src/sitesyncro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-21 22:23:49.000000 sitesyncro-0.9/src/sitesyncro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-27 09:03:44.073151 sitesyncro-0.9.1/
+-rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0    21234 2024-04-27 09:03:44.069893 sitesyncro-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20300 2024-04-27 08:37:27.000000 sitesyncro-0.9.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-27 09:03:44.074369 sitesyncro-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1712 2024-04-26 19:27:47.000000 sitesyncro-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:03:43.988338 sitesyncro-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-27 09:03:44.007340 sitesyncro-0.9.1/src/sitesyncro/
+-rw-rw-rw-   0        0        0    19405 2024-04-27 08:51:16.000000 sitesyncro-0.9.1/src/sitesyncro/Model.py
+-rw-rw-rw-   0        0        0     9768 2024-04-26 17:24:58.000000 sitesyncro-0.9.1/src/sitesyncro/Sample.py
+-rw-rw-rw-   0        0        0      200 2024-04-24 16:19:07.000000 sitesyncro-0.9.1/src/sitesyncro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:03:44.062974 sitesyncro-0.9.1/src/sitesyncro/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.1/src/sitesyncro/utils/__init__.py
+-rw-rw-rw-   0        0        0     9844 2024-04-27 08:10:02.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_cluster.py
+-rw-rw-rw-   0        0        0      961 2024-04-23 15:45:23.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_data.py
+-rw-rw-rw-   0        0        0     4696 2024-04-24 16:42:54.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_load.py
+-rw-rw-rw-   0        0        0     1568 2022-05-26 16:44:35.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_mp.py
+-rw-rw-rw-   0        0        0     8908 2024-04-26 17:15:36.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_oxcal.py
+-rw-rw-rw-   0        0        0     6594 2024-04-27 08:32:52.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_phase.py
+-rw-rw-rw-   0        0        0     4360 2024-04-26 15:27:54.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_plot.py
+-rw-rw-rw-   0        0        0     2173 2024-04-23 17:46:49.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_radiocarbon.py
+-rw-rw-rw-   0        0        0     6780 2024-04-27 07:54:11.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_simulate.py
+-rw-rw-rw-   0        0        0     3959 2024-04-27 08:24:13.000000 sitesyncro-0.9.1/src/sitesyncro/utils/fnc_stat.py
+drwxrwxrwx   0        0        0        0 2024-04-27 09:03:44.066455 sitesyncro-0.9.1/src/sitesyncro.egg-info/
+-rw-rw-rw-   0        0        0    21234 2024-04-27 09:03:43.000000 sitesyncro-0.9.1/src/sitesyncro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      668 2024-04-27 09:03:43.000000 sitesyncro-0.9.1/src/sitesyncro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-27 09:03:43.000000 sitesyncro-0.9.1/src/sitesyncro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-04-27 09:03:43.000000 sitesyncro-0.9.1/src/sitesyncro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-27 09:03:43.000000 sitesyncro-0.9.1/src/sitesyncro.egg-info/top_level.txt
```

### Comparing `sitesyncro-0.9/LICENSE` & `sitesyncro-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9/PKG-INFO` & `sitesyncro-0.9.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,24 @@
-Metadata-Version: 2.1
-Name: sitesyncro
-Version: 0.9
-Summary: SiteSyncro - Site-specific chronological modeling and synchronization
-Home-page: https://github.com/demjanp/SiteSyncro
-Author: Peter Demjan
-Author-email: peter.demjan@gmail.com
-Keywords: archaeology,radiocarbon,chronology,stratigraphy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy<2,>=1.26.4
-Requires-Dist: scipy<2,>=1.13.0
-Requires-Dist: matplotlib<4,>=3.8.4
-Requires-Dist: scikit-learn<2,>=1.4.2
-Requires-Dist: tqdm<5,>=4.66.0
-Requires-Dist: requests<3,>=2.31.0
-Requires-Dist: networkx<4,>=3.3.0
-
 # SiteSyncro
 Site-specific chronological modeling and synchronization
 
 Created on 10.4.2024
 
 <details>
 <summary>Table of Contents</summary>
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
+   * [Input File Format](#input_file)
+   * [Model Class](#model_class)
+   * [Sample Class](#sample_class)
 4. [Developer Notes](#developer)
+	* [Preparing the Virtual Environment](#venv)
+	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
 </details>
 
 ## About SiteSyncro <a name="about"></a>
@@ -52,279 +33,318 @@
 For a detailed overview of the clustering method see:
 
 Demján, P., & Pavúk, P. (2021). CLUSTERING OF CALIBRATED RADIOCARBON DATES: SITE-SPECIFIC CHRONOLOGICAL SEQUENCES IDENTIFIED BY DENSE RADIOCARBON SAMPLING. Radiocarbon, 63(2), 429-438. [doi:10.1017/RDC.2020.129](https://doi.org/10.1017/RDC.2020.129)
 
 
 ## Installation <a name="installation"></a>
 
-SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The OxCal program is used for bayesian modeling of the radiocarbon dates. The OxCal program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
+[Windows executable](https://github.com/demjanp/SiteSyncro/releases/latest) is available for users who do not want to install Python and dependencies.
 
-For Windows users, an executable version of SiteSyncro is available. You can download the `sitesyncro.exe` file from the [latest release on GitHub](https://github.com/demjanp/SiteSyncro/releases/latest). After downloading, you can run SiteSyncro directly without needing to install Python or any dependencies.
+To run SiteSyncro on other platforms, please refer to the [Developer Notes](#developer) section on how to clone SiteSyncro from GitHub and create a virtual environment. See [Usage](#usage) section on how to run the script or import SiteSyncro as a python library.
 
-To run SiteSyncro on other platforms, please refer to the [Developer Notes](#developer) section on how to clone SiteSyncro from GitHub and create a virtual environment. See [Usage](#usage) section on how to run the script.
+To use SiteSyncro in your Python applications, install the latest version from the Python package index, use the following command:
+```
+pip install SiteSyncro
+```
+See [Model Class](#model_class) on usage tips.
+
+SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
 
 ## Usage <a name="usage"></a>
+
+### Running the Script
 To use SiteSyncro, you need to run the [process.py](bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
-```bash
-python process.py data_sample.csv
+```
+python process.py -input data_sample.csv
 ```
 or
-```bash
-sitesyncro.exe data_sample.csv
-```bash
+```
+sitesyncro.exe -input data_sample.csv
+```
 `process.py` & `sitesyncro.exe` accepts the following command-line arguments:
-
-- `input`: The path to the input file in semicolon-separated CSV format (required).
-- `-result`: The directory path to store the results (default is "result").
-- `-existing`: Flag indicating whether to use existing results (default is 0).
-- `-curve`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
-- `-model`: OxCal model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
-- `-n`: Number of clusters to form (-1 = automatic; default is -1).
+- `-h`, `--help`: Show help message and exit.
+- `-directory`: Working directory for model data (default is "model").
+- `-input`: The path to the input file in semicolon-separated CSV format.
+- `-curve_name`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
+- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
+- `-cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
+- `-by_clusters`: Flag indicating whether to update the phasing by clustering sample dates (default is 0).
 - `-uniform`: Flag indicating whether to use a uniform distribution for the calendar ages (default is 0).
 - `-p_value`: P-value for the randomization tests (default is 0.05).
-- `-uncert_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
+- `-uncertainty_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
 - `-npass`: Minimum number of passes for the randomization tests (default is 100).
 - `-convergence`: Convergence threshold for the randomization tests (default is 0.99).
 - `-max_cpus`: Maximum number of CPUs to use for parallel processing (-1 = all available; default is -1).
-- `-max_queue_size`: Maximum queue size for parallel processing (default is 100).
+- `-max_queue_size`: Maximum queue size for parallel processing (default is 100)
 
 For example, if you want to run the script with a specific calibration curve, using uniform distributions for randomization testing and a P-value threshold of 0.01, you can do so like this:
 
 ```bash
-python process.py data_sample.csv -curve intcal20.14c -uniform 1 -p_value 0.01
+python process.py -input data_sample.csv -curve intcal20.14c -uniform 1 -p_value 0.01
 ```
 
 This will run the script with input data from data_sample.csv and use the IntCal20 calibration curve, a uniform distribution for the calendar ages, and a P-value of 0.01 for the randomization tests.
 
+### Input File Format <a name="input_file"></a>
 The input file name must be a semicolon-separated CSV file with the following 8 columns: 
 1. Sample: Sample ID (required, unique identifier)
 2. Context: Context ID (required)
 3. Excavation Area: Excavation area ID (required)
 4. C-14 Age: Radiocarbon age in years BP (required)
 5. Uncertainty: Uncertainty of the radiocarbon age in C-14 years (required)
 6. Phase: Phase of the sample (lower = older) (optional)
 7. Earlier-Than: List of contexts that the sample is earlier (older) than (optional)
 8. Long-Lived / Redeposited: Flag indicating whether the sample is long-lived (e.g. old wood) or redeposited (e.g. from an older context) (required, 1 or 0)
 
 See [data_sample.csv](data_sample.csv) for an example of the input file format.
 
+### Model Class <a name="model_class"></a>
+All functions regarding modeling are encapsulated in the `Model` class. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Model
+
+if __name__ == '__main__':
+	
+    # Initialize the Model object
+    model = Model()
+    
+    # Load the data
+    model.import_csv('data_sample.csv')
+    
+    # Process the model
+    model.process()
+    
+    # Plot the randomization test result
+    model.plot_randomized()
+    
+    # Plot the clustering result
+    model.plot_clusters()
+    
+    # Save the results to a CSV file
+    model.save_csv()
+```
+This will create the default directory `model` and generate the following files:
+`model.json.gz`
+`model.oxcal`
+`model.js`, `model.log`, `model.txt`
+`randomized.pdf`
+`silhouette.pdf`
+`results.csv`
+
+#### Parameters <a name="model_parameters"></a>
+
+The `Model` class constructor accepts the following parameters:
+- `directory`: Working directory for model data (default is "model").
+- `samples`: List of samples as instances of the class [Sample](#sample_class)
+- `curve_name`: The name of the calibration curve to use (default is "intcal20.14c").
+- `phase_model`: OxCal phase model type. Can be 'sequence', 'contiguous', 'overlapping', or 'none' (default is "sequence").
+- `cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
+- `uniform`: Flag indicating whether to use uniform randomization (default is False).
+- `p_value`: The P-value for statistical tests (default is 0.05).
+- `uncertainty_base`: The base uncertainty for randomization (default is 15).
+- `npass`: Minimum number of passes for the randomization tests (default is 100).
+- `convergence`: Convergence threshold for the randomization tests (default is 0.99).
+- `oxcal_url`: Url to download the OxCal program (default is "https://c14.arch.ox.ac.uk/OxCalDistribution.zip").
+
+#### Methods
+
+The `Model` class provides the following methods:
+- `add_sample(sample)` or `add_sample(name, age, uncertainty, **kwargs)`: Add a sample to the model.
+	- For arguments see [Sample parameters](#sample_parameters).
+- `del_sample(name)`: Delete a sample from the model.
+- `reset_model()`: Reset the model to the initial state.
+- `save(zipped = False)`: Save the model to a file.
+	- `zipped`; if True, save the model as a zipped JSON file
+- `copy(directory)`: Copy the model to a new directory.
+	- `directory`: Directory for the new model
+- `import_csv(fname)`: Import sample data from a CSV file. See [Input File Format](#input_file) for details.
+- `plot_randomized(show = False)`: Plot the randomization test results. If `show` is True, the plot is shown, otherwise it is saved as `randomized.pdf`.
+- `plot_clusters(show = False)`: Plot the clustering results. If `show` is True, the plot is shown, otherwise it is saved as `silhouette.pdf`.
+- `save_csv(fcsv = None)`: Save the results to a CSV file.
+	- `fcsv`: File path for the CSV file. If None, `results.csv` is saved in the model directory.
+- `to_oxcal()`: Save the phasing model in OxCal format as `model.oxcal`.
+- `load_oxcal_data()`: Load results of OxCal modeling from `model.js`.
+- `update_params(**kwargs)`: Update model parameters.
+	- For keyword arguments see [Parameters](#model_parameters)
+- `process_phasing(by_clusters = False)`: Update groups and phases of samples based on stratigraphic relations.
+	- `by_clusters`: if True, update the phasing by clustering sample dates
+- `process_dates()`: Calculate posteriors of sample dates based on phasing using bayesian modeling in OxCal.
+- `process_randomization(max_cpus = -1, max_queue_size = 100)`: Test if sample dates represent a uniform / normal (depending on Model.uniform parameter) distribution in time.
+- `process_clustering(max_cpus = -1, max_queue_size = 100)`: Cluster dates and using randomization testing find optimal clustering solution
+- `process(by_clusters = False, max_cpus = -1, max_queue_size = 100)`: Process the complete model
+	- `by_clusters`: if True, update the phasing by clustering sample dates
+	- `max_cpus`: Maximum number of CPUs to use for parallel processing (-1 = all available)
+	- `max_queue_size`: Maximum queue size for parallel processing
+
+#### Attributes
+
+The `Model` class has the following attributes:
+- `directory`: Working directory for model data
+- `samples`: Dictionary of samples in format `{name: Sample, ...}`
+- `curve_name`: The name of the calibration curve
+- `phase_model`: OxCal phase model type
+- `cluster_n`: Number of clusters to form
+- `uniform`: Flag indicating whether to use uniform randomization
+- `p_value`: The P-value threshold for statistical tests
+- `uncertainty_base`: The base uncertainty for randomization
+- `npass`: Minimum number of passes for the randomization tests
+- `convergence`: Convergence threshold for the randomization tests
+- `oxcal_url`: Url to download the OxCal program
+- `years`: Calendar years BP corresponding to the probability distributions in format `np.array([year, ...])`
+- `curve`: Calibration curve in format `np.array([[calendar year BP, C-14 year, uncertainty], ...])`, sorted by calendar years
+- `uncertainties`: List of uncertainties from C-14 dates of samples
+- `oxcal_data`: Results of OxCal modeling from `model.js` in format `{key: data, ...}`
+- `summed`: Summed probability distribution of the dating of all samples in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `random_p`: Calculated p-value for the randomization test
+- `random_lower`: Lower bound of the randomization test in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `random_upper`: Upper bound of the randomization test in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `areas`: List of excavation areas that the samples belong to
+- `contexts`: List of contexts that the samples belong to
+- `groups`: Groups that the samples belong to based on stratigraphic interconnection with other samples in format `{group_name: [sample name, ...], ...}`
+- `clusters`: Clusters of samples based on the similarity of their probability distributions in format `{clusters_n: [cluster: [sample name, ...], ...}, ...}`
+- `cluster_means`: Mean date of the samples in each cluster in calendar years BP in format `{clusters_n: {cluster: year, ...}, ...}`
+- `cluster_sils`: Silhouette score of each clustering solution in format `{clusters_n: silhouette, ...}`
+- `cluster_ps`: P-value of the clustering solutions in format `{clusters_n: p, ...}`
+- `cluster_opt_n`: Optimal number of clusters
+- `has_data`: Boolean indicating if the model has sample data
+- `is_modeled`: Boolean indicating if bayesian modeling of sample dates (process_dates) has been performed
+- `is_randomized`: Boolean indicating if randomization testing of the distribution of samples (process_randomization) has been performed
+- `is_clustered`: Boolean indicating if the model has been clustered (process_clustering)
+
+### Sample Class <a name="sample_class"></a>
+The `Sample` class represents a single radiocarbon sample. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Sample
+
+if __name__ == '__main__':
+	
+	# Initialize the Sample object
+	sample = Sample('Sample1', 1000, 50, phase = 1, earlier_than = ['Sample2'], long_lived = 0)
+	
+	# Print the sample data
+	print(sample)
+```
+
+#### Parameters <a name="sample_parameters"></a>
+
+The 'Sample' class constructor accepts the following parameters:
+- `name`: Sample ID (required, unique identifier)
+- `age`: C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U' (required)
+- `uncertainty`: Uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U' (required)
+- `date_type`: 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution
+- `long_lived`: True if sample is older than the examined deposition event due to e.g. old wood effect or redeposition from older strata
+- `context`: Name of the context where sample was found
+- `area`: Excavation area
+- `area_excavation_phase`: Chronological phase of the context within the excavation area (integer, lower = earlier (older) phase)
+- `earlier_than`: List of names of samples which are stratigraphically later (younger) than this sample
+- `curve`: Radiocarbon calibration curve in format `np.array([[calendar year BP, C-14 year, uncertainty], ...])`
+
+#### Methods
+
+The `Sample` class provides the following methods:
+- `calibrate(curve)`: Calibrate the sample using the provided calibration curve.
+	- `curve = np.array([[calendar year BP, C-14 year, uncertainty], ...])`
+- `set_group(group)`: Set the group number for the sample.
+- `set_phase(phase)`: Set the phase number for the sample.
+- `set_likelihood(distribution, mean = None, rng = None)`: Set the likelihood for the sample.
+	- `distribution = np.array([p, ...])`
+	- `rng = [from, to]`; 2-sigma (95.45%) range in calendar years BP
+- `set_posterior(distribution, mean = None, rng = None, agreement = 0)`: Set the posterior for the sample.
+	- `distribution = np.array([p, ...])`
+	- `rng = [from, to]`; 2-sigma (95.45%) range in calendar years BP
+	- `agreement`: agreement index generated by OxCal modeling
+- `to_oxcal()`: Convert the sample to OxCal model format (str).
+- `to_dict()`: Convert the sample data to a JSON dictionary.
+- `from_dict(data)`: Load the sample data from a JSON dictionary.
+- `copy()`: Create a copy of the sample instance.
+
+#### Attributes
+The `Sample` class has the following attributes:
+
+- `name`: Sample ID (unique identifier)
+- `age`: C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U'
+- `uncertainty`: Uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U'
+- `date_type`: 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution
+- `long_lived`: True if sample is older than the examined deposition event due to e.g. old wood effect or redeposition from older strata
+- `context`: Name of the context where sample was found
+- `area`: Excavation area
+- `area_excavation_phase`: Chronological phase of the context within the excavation area (integer, lower = earlier (older) phase)
+- `earlier_than`: List of names of samples which are stratigraphically later (younger) than this sample
+- `group`: Group that the sample belongs to based on stratigraphic interconnection with other samples
+- `phase`: Stratigraphic phase of the sample within the group (lower = earlier (older) phase)
+- `years`: Calendar years BP corresponding to the probability distributions in format `np.array([year, ...])`
+- `likelihood`: Probability distribution of the dating of the sample before Bayesian modeling in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `posterior`: Probability distribution of the dating of the sample after Bayesian modeling in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `likelihood_range`: 2-sigma (95.45%) range of the dating of the sample in calendar years BP before Bayesian modeling in format `[from, to]`
+- `likelihood_mean`: Mean calendar age of the sample in calendar years BP before Bayesian modeling
+- `posterior_range`: 2-sigma (95.45%) range of the dating of the sample in calendar years BP after Bayesian modeling in format `[from, to]`
+- `posterior_mean`: Mean calendar age of the sample in calendar years BP after Bayesian modeling
+- `posterior_agreement`: Agreement index generated by OxCal modeling
+- `is_calibrated`: Boolean indicating if the sample has been calibrated
+- `is_modeled`: Boolean indicating if posterior has been calculated using Bayesian modeling
+
 ## Developer Notes <a name="developer"></a>
 ### Preparing the Virtual Environment <a name="venv"></a>
 SiteSyncro requires [Python 3.10](https://www.python.org/downloads/).
 
 To prepare a Python virtual environment open a terminal or command prompt window and type the following commands:
 
 ```
 git clone https://github.com/demjanp/SiteSyncro.git
-
 cd sitesyncro
-
 python -m venv .venv
-
 .venv\Scripts\activate.bat
-
 python.exe -m pip install --upgrade pip
-
 pip install -e .
 ```
 
 See [Usage](#usage) on further instructions how to run the script.
 
-### Building a Windows Executable
+### Building a Windows Executable <a name="build"></a>
 To build a Windows executable, open a terminal or command prompt window and change to the `sitesyncro` folder: 
 ```
 cd SiteSyncro\sitesyncro
 ```
 Activate the virtual environment:
 ```
 .venv\Scripts\activate.bat
 ```
 Then type the following commands (this only has to be done once per virtual environment):
 ```
-python.exe -m pip install --upgrade pip
+python -m pip install --upgrade pip
 python -m pip install --upgrade build
 pip install twine
 pip install pyinstaller==6.6.0
 ```
 To build the executable, type:
 ```
 pip install -e .
 python -m build
 pyinstaller sitesyncro.spec
 ```
-You will find the executable `sitesyncro.exe` in the `dist` folder.
-
-### SiteSyncro Class
-All functions of SiteSyncro are encapsulated in the `SiteSyncro` class. Here is a basic example of how to use it:
-
-```python
-from sitesyncro import SiteSyncro
-
-# Initialize the SiteSyncro object
-ssync = SiteSyncro(input='data_sample.csv')
-
-# Load the data
-ssync.load_data()
-
-# Process the model
-ssync.process()
-
-# Plot the randomization test result
-ssync.plot_randomized()
-
-# Plot the clustering result
-ssync.plot_clusters()
-
-# Save the results to a CSV file
-ssync.save_results_csv()
-```
-
-#### Parameters <a name="parameters"></a>
-
-The `SiteSyncro` class accepts the following parameters:
-- `input`: The path to the input file.
-- `result`: The name of the result directory (default is "result").
-- `existing`: Boolean indicating whether to use existing results (default is False).
-- `curve`: The name of the calibration curve to use (default is "intcal20.14c").
-- `model`: The name of the model to use. Can be 'sequence', 'contiguous', 'overlapping', or 'none' (default is "sequence").
-- `n`: The number of clusters (-1 = automatic) (default is -1).
-- `uniform`: Boolean indicating whether to use uniform randomization (default is False).
-- `p_value`: The P-value for statistical tests (default is 0.05).
-- `uncert_base`: The base uncertainty for randomization (default is 15).
-- `npass`: The number of passes for the clustering algorithm (default is 100).
-- `convergence`: The convergence criterion for the clustering algorithm (default is 0.99).
-- `max_cpus`: The maximum number of CPUs to use (default is -1).
-- `max_queue_size`: The maximum size of the queue for parallel processing (default is 100).
-
-#### Methods
-
-The `SiteSyncro` class provides the following methods:
-- `load_data(**kwargs)`: Loads data from the input file and updates the internal data. The input file must be a CSV file with the following columns: Context, Excavation Area, C-14 Age, Uncertainty, Phase (lower = older), Earlier-Than, Long-Lived / Redeposited. For possible keyword arguments see [Parameters](#parameters).
-- `process(**kwargs)`: Processes the data. For possible keyword arguments see [Parameters](#parameters).
-- `plot_randomized(show=False)`: Plots the randomized data. If `show` is True, the plot is shown. If False, the plot is saved to a file.
-- `plot_clusters(show=False)`: Plots the clustering data. If `show` is True, the plot is shown. If False, the plot is saved to a file.
-- `save_results_csv(fcsv=None)`: Saves the results to a CSV file. If `fcsv` is None, a default file path is used.
-
-#### Attributes
-
-The `SiteSyncro` class has the following attributes:
-- `oc_data` (OxCalData): Used to store and manage the data after bayesian modelling of the radiocarbon dates with the OxCal program.
-- `rnd_data` (RandomizeData): Used to store and manage the data related to the randomization testing of the null hypothesis that the observed C-14 dates represent a normal/uniform distribution.
-- `clu_data` (ClusterData): Used to store and manage the data related to the temporal clustering of the modelled C-14 dates.
-- `oc_clu_data` (OxCalData): Used to store and manage the modelled data updated according to the temporal clustering of the C-14 dates.
-
-All variables generated by the OxCal program can be accessed using `oc_data[key]`. Use `print(oc_data)` to see a list of available keys.
-
-`OxCalData` class methods:
-- `__init__(fname=None)`: If a filename of an OxCal .js file is provided, it reads and stores the data.
-- `has_data(self)`: Returns True if the data dictionary is not empty, False otherwise.
-- `set_priors(samples, context_samples, context_area, areas, groups, phases, earlier_than, long_lived, r_dates, dates, model, curve)`: Sets the priors for the bayesian modeling.
-    ```
-    samples = [sample, ...]
-    context_samples = {context: [sample, ...], ...}
-    context_area = {context: area, ...}
-    areas = [area, ...]
-    groups = {group: [sample, ...], ...}
-    phases = {group: {sample: phase, ...}, ...}
-    long_lived = {sample: True/False, ...}
-    r_dates = {sample: (age, uncertainty), ...}
-    dates = {sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}; R = radiocarbon, U = uniform
-    ```
-- `get_likelihoods()`: Returns the likelihood distributions for each sample.
-    Format: `{name: {'prob': [p, ...], 'years': [calendar year CE, ...], 'mean': mean, 'range': [min year CE, max year CE]}}`
-    Ranges are calculated at the 95.45% (2-sigma) level.
-- `get_posteriors()`: Returns the posterior distributions for each sample. 
-    Format: `{name: {'prob': [p, ...], 'years': [calendar year CE, ...], 'mean': mean, 'range': [min year CE, max year CE], 'agreement': agreement index}}`	
-    Ranges are calculated at the 95.45% (2-sigma) level.
-- `get_samples()`: Returns the sample names.
-    Format: `[name, ...]`
-- `get_context_samples()`: Returns the contexts and their contained samples.
-    Format: `{context: [sample, ...], ...}`
-- `get_context_area()`: Returns the contexts and their areas.
-    Format: `{context: area, ...}`
-- `get_areas()`: Returns the areas.
-    Format: `[area, ...]`
-- `get_groups()`: Returns the groups based on stratigraphic links.
-    Format: `{group: [sample, ...], ...}`
-- `get_phases()`: Returns the phases for each group and sample. Lower = earlier (older) phase.
-    Format: `{group: {sample: phase, ...}, ...}`
-- `get_earlier_than()`: Returns the earlier-than relations between samples.
-    Format: `matrix[n_samples x n_samples] = [True/False, ...]`. Sample in row is earlier than sample in column based on stratigraphy.
-- `get_long_lived()`: Returns the long-lived value for each sample.
-    Format: `{sample: True/False, ...}`
-- `get_r_dates()`: Returns the radiocarbon dates for each sample.
-    Format: `{sample: (age, uncertainty), ...}`
-- `get_dates()`: Returns the date for bayesian modeling for each sample. Long-lived or redeposited samples are represented by a uniform distribution where the lower boundary is the lower boundary of the 2-sigma range of the calibrated date and the upper boundary is 1950 CE. 
-    Format: `{sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}`; R = radiocarbon, U = uniform
-- `get_model()`: Returns the model type used for the bayesian modeling.
-    Values: 'sequence', 'contiguous', 'overlapping', 'none'
-- `get_curve()`: Returns the calibration curve used.
-    Format: curve name (see OxCal\bin folder for available curves)
-
-`ClusterData` class methods:
-- `__init__(clusters = {}, means = {}, sils = {}, ps = {}, p_value = None, opt_n = None)`
-    ```
-    means = {n: mean, ...}
-    sils = {sample: sil, ...}
-    ps = {n: p, ...}
-    p_value = p-value threshold for randomization testing
-    opt_n = optimal number of clusters
-	```	
-- `has_data()`: Returns True if the clusters dictionary is not empty, False otherwise.
-- `get_clusters()`: Returns the clusters for each number of clusters.
-    Format: `{n: {sample: cluster, ...}, ...}`
-- `get_means()`: Returns the mean silhouette score for each number of clusters.
-    Format: `{n: mean, ...}`
-- `get_sils()`: Returns the silhouette score for each sample.
-    Format: `{sample: sil, ...}`
-- `get_ps()`: Returns the p-value for each number of clusters.
-    Format: `{n: p, ...}`
-- `get_p_value()`: Returns the p-value threshold for randomization testing.
-- `get_opt_n()`: Returns the optimal number of clusters.
-
-`RandomizeData` class methods:
-- `__init__(years = None, sum_obs = None, uniform = None, p = None, p_value = None, sums_rnd_lower = None, sums_rnd_upper = None)`
-    ```
-    years = [year, ...]. The years are in calendar years BP.
-    sum_obs = [p, ...] in order of the years.
-    uniform = True/False
-    p = calculated p-value
-    p_value = p-value threshold
-    sums_rnd_lower = [p, ...] in order of the years.
-    sums_rnd_upper = [p, ...] in order of the years.
-	```
-- `has_data()`: Returns True if the years attribute is not None, False otherwise.
-- `get_years()`: Returns the years for the randomization test.
-    Format: `[year, ...]`. The years are in calendar years BP.
-- `get_sum_obs()`: Returns the sum of the observed distributions.
-    Format: `[p, ...]` in order of the years.
-- `get_uniform()`: Returns True if the uniform distribution was used.
-- `get_p()`: Returns the calculated p-value for the randomization test.
-- `get_p_value()`: Returns the p-value threshold for the randomization test.
-- `get_sums_rnd_lower()`: Returns the lower boundary of the randomized distributions.
-    Format: `[p, ...]` in order of the years.
-- `get_sums_rnd_upper()`: Returns the upper boundary of the randomized distributions.
-    Format: `[p, ...]` in order of the years.
+The executable `sitesyncro.exe` will be created in the `dist` folder.
 
 ## Contact: <a name="contact"></a>
 Peter Demján (peter.demjan@gmail.com)
 
 Institute of Archaeology of the Czech Academy of Sciences, Prague, v.v.i.
 
 ## Acknowledgements <a name="acknowledgements"></a>
 
 Development of this software was supported by project OP JAC "Ready for the future: understanding long-term resilience of the human culture (RES-HUM)", Reg. No. CZ.02.01.01/00/22_008/0004593 of the Ministry of Education, Youth, and Sports of the Czech Republic and EU.
 
 This software requires the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program for bayesian modeling of the radiocarbon dates.
 
 This software uses the following open source packages:
-* [NumPy](https://www.numpy.org/)
-* [SciPy](https://scipy.org/)
 * [Matplotlib](https://matplotlib.org/)
+* [NetworkX](https://networkx.org/)
+* [NumPy](https://www.numpy.org/)
+* [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
+* [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
-* [Requests](https://requests.readthedocs.io/)
-* [NetworkX](https://networkx.org/)
 
 ## License <a name="license"></a>
 
-This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
+This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
```

### Comparing `sitesyncro-0.9/README.md` & `sitesyncro-0.9.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,48 @@
+Metadata-Version: 2.1
+Name: sitesyncro
+Version: 0.9.1
+Summary: SiteSyncro - Site-specific chronological modeling and synchronization
+Home-page: https://github.com/demjanp/SiteSyncro
+Author: Peter Demjan
+Author-email: peter.demjan@gmail.com
+Keywords: archaeology,radiocarbon,chronology,stratigraphy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy<2,>=1.26.4
+Requires-Dist: scipy<2,>=1.13.0
+Requires-Dist: matplotlib<4,>=3.8.4
+Requires-Dist: scikit-learn<2,>=1.4.2
+Requires-Dist: tqdm<5,>=4.66.0
+Requires-Dist: requests<3,>=2.31.0
+Requires-Dist: networkx<4,>=3.3.0
+
 # SiteSyncro
 Site-specific chronological modeling and synchronization
 
 Created on 10.4.2024
 
 <details>
 <summary>Table of Contents</summary>
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
+   * [Input File Format](#input_file)
+   * [Model Class](#model_class)
+   * [Sample Class](#sample_class)
 4. [Developer Notes](#developer)
+	* [Preparing the Virtual Environment](#venv)
+	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
 </details>
 
 ## About SiteSyncro <a name="about"></a>
@@ -28,279 +57,318 @@
 For a detailed overview of the clustering method see:
 
 Demján, P., & Pavúk, P. (2021). CLUSTERING OF CALIBRATED RADIOCARBON DATES: SITE-SPECIFIC CHRONOLOGICAL SEQUENCES IDENTIFIED BY DENSE RADIOCARBON SAMPLING. Radiocarbon, 63(2), 429-438. [doi:10.1017/RDC.2020.129](https://doi.org/10.1017/RDC.2020.129)
 
 
 ## Installation <a name="installation"></a>
 
-SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The OxCal program is used for bayesian modeling of the radiocarbon dates. The OxCal program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
+[Windows executable](https://github.com/demjanp/SiteSyncro/releases/latest) is available for users who do not want to install Python and dependencies.
 
-For Windows users, an executable version of SiteSyncro is available. You can download the `sitesyncro.exe` file from the [latest release on GitHub](https://github.com/demjanp/SiteSyncro/releases/latest). After downloading, you can run SiteSyncro directly without needing to install Python or any dependencies.
+To run SiteSyncro on other platforms, please refer to the [Developer Notes](#developer) section on how to clone SiteSyncro from GitHub and create a virtual environment. See [Usage](#usage) section on how to run the script or import SiteSyncro as a python library.
 
-To run SiteSyncro on other platforms, please refer to the [Developer Notes](#developer) section on how to clone SiteSyncro from GitHub and create a virtual environment. See [Usage](#usage) section on how to run the script.
+To use SiteSyncro in your Python applications, install the latest version from the Python package index, use the following command:
+```
+pip install SiteSyncro
+```
+See [Model Class](#model_class) on usage tips.
+
+SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
 
 ## Usage <a name="usage"></a>
+
+### Running the Script
 To use SiteSyncro, you need to run the [process.py](bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
-```bash
-python process.py data_sample.csv
+```
+python process.py -input data_sample.csv
 ```
 or
-```bash
-sitesyncro.exe data_sample.csv
-```bash
+```
+sitesyncro.exe -input data_sample.csv
+```
 `process.py` & `sitesyncro.exe` accepts the following command-line arguments:
-
-- `input`: The path to the input file in semicolon-separated CSV format (required).
-- `-result`: The directory path to store the results (default is "result").
-- `-existing`: Flag indicating whether to use existing results (default is 0).
-- `-curve`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
-- `-model`: OxCal model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
-- `-n`: Number of clusters to form (-1 = automatic; default is -1).
+- `-h`, `--help`: Show help message and exit.
+- `-directory`: Working directory for model data (default is "model").
+- `-input`: The path to the input file in semicolon-separated CSV format.
+- `-curve_name`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
+- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
+- `-cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
+- `-by_clusters`: Flag indicating whether to update the phasing by clustering sample dates (default is 0).
 - `-uniform`: Flag indicating whether to use a uniform distribution for the calendar ages (default is 0).
 - `-p_value`: P-value for the randomization tests (default is 0.05).
-- `-uncert_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
+- `-uncertainty_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
 - `-npass`: Minimum number of passes for the randomization tests (default is 100).
 - `-convergence`: Convergence threshold for the randomization tests (default is 0.99).
 - `-max_cpus`: Maximum number of CPUs to use for parallel processing (-1 = all available; default is -1).
-- `-max_queue_size`: Maximum queue size for parallel processing (default is 100).
+- `-max_queue_size`: Maximum queue size for parallel processing (default is 100)
 
 For example, if you want to run the script with a specific calibration curve, using uniform distributions for randomization testing and a P-value threshold of 0.01, you can do so like this:
 
 ```bash
-python process.py data_sample.csv -curve intcal20.14c -uniform 1 -p_value 0.01
+python process.py -input data_sample.csv -curve intcal20.14c -uniform 1 -p_value 0.01
 ```
 
 This will run the script with input data from data_sample.csv and use the IntCal20 calibration curve, a uniform distribution for the calendar ages, and a P-value of 0.01 for the randomization tests.
 
+### Input File Format <a name="input_file"></a>
 The input file name must be a semicolon-separated CSV file with the following 8 columns: 
 1. Sample: Sample ID (required, unique identifier)
 2. Context: Context ID (required)
 3. Excavation Area: Excavation area ID (required)
 4. C-14 Age: Radiocarbon age in years BP (required)
 5. Uncertainty: Uncertainty of the radiocarbon age in C-14 years (required)
 6. Phase: Phase of the sample (lower = older) (optional)
 7. Earlier-Than: List of contexts that the sample is earlier (older) than (optional)
 8. Long-Lived / Redeposited: Flag indicating whether the sample is long-lived (e.g. old wood) or redeposited (e.g. from an older context) (required, 1 or 0)
 
 See [data_sample.csv](data_sample.csv) for an example of the input file format.
 
+### Model Class <a name="model_class"></a>
+All functions regarding modeling are encapsulated in the `Model` class. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Model
+
+if __name__ == '__main__':
+	
+    # Initialize the Model object
+    model = Model()
+    
+    # Load the data
+    model.import_csv('data_sample.csv')
+    
+    # Process the model
+    model.process()
+    
+    # Plot the randomization test result
+    model.plot_randomized()
+    
+    # Plot the clustering result
+    model.plot_clusters()
+    
+    # Save the results to a CSV file
+    model.save_csv()
+```
+This will create the default directory `model` and generate the following files:
+`model.json.gz`
+`model.oxcal`
+`model.js`, `model.log`, `model.txt`
+`randomized.pdf`
+`silhouette.pdf`
+`results.csv`
+
+#### Parameters <a name="model_parameters"></a>
+
+The `Model` class constructor accepts the following parameters:
+- `directory`: Working directory for model data (default is "model").
+- `samples`: List of samples as instances of the class [Sample](#sample_class)
+- `curve_name`: The name of the calibration curve to use (default is "intcal20.14c").
+- `phase_model`: OxCal phase model type. Can be 'sequence', 'contiguous', 'overlapping', or 'none' (default is "sequence").
+- `cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
+- `uniform`: Flag indicating whether to use uniform randomization (default is False).
+- `p_value`: The P-value for statistical tests (default is 0.05).
+- `uncertainty_base`: The base uncertainty for randomization (default is 15).
+- `npass`: Minimum number of passes for the randomization tests (default is 100).
+- `convergence`: Convergence threshold for the randomization tests (default is 0.99).
+- `oxcal_url`: Url to download the OxCal program (default is "https://c14.arch.ox.ac.uk/OxCalDistribution.zip").
+
+#### Methods
+
+The `Model` class provides the following methods:
+- `add_sample(sample)` or `add_sample(name, age, uncertainty, **kwargs)`: Add a sample to the model.
+	- For arguments see [Sample parameters](#sample_parameters).
+- `del_sample(name)`: Delete a sample from the model.
+- `reset_model()`: Reset the model to the initial state.
+- `save(zipped = False)`: Save the model to a file.
+	- `zipped`; if True, save the model as a zipped JSON file
+- `copy(directory)`: Copy the model to a new directory.
+	- `directory`: Directory for the new model
+- `import_csv(fname)`: Import sample data from a CSV file. See [Input File Format](#input_file) for details.
+- `plot_randomized(show = False)`: Plot the randomization test results. If `show` is True, the plot is shown, otherwise it is saved as `randomized.pdf`.
+- `plot_clusters(show = False)`: Plot the clustering results. If `show` is True, the plot is shown, otherwise it is saved as `silhouette.pdf`.
+- `save_csv(fcsv = None)`: Save the results to a CSV file.
+	- `fcsv`: File path for the CSV file. If None, `results.csv` is saved in the model directory.
+- `to_oxcal()`: Save the phasing model in OxCal format as `model.oxcal`.
+- `load_oxcal_data()`: Load results of OxCal modeling from `model.js`.
+- `update_params(**kwargs)`: Update model parameters.
+	- For keyword arguments see [Parameters](#model_parameters)
+- `process_phasing(by_clusters = False)`: Update groups and phases of samples based on stratigraphic relations.
+	- `by_clusters`: if True, update the phasing by clustering sample dates
+- `process_dates()`: Calculate posteriors of sample dates based on phasing using bayesian modeling in OxCal.
+- `process_randomization(max_cpus = -1, max_queue_size = 100)`: Test if sample dates represent a uniform / normal (depending on Model.uniform parameter) distribution in time.
+- `process_clustering(max_cpus = -1, max_queue_size = 100)`: Cluster dates and using randomization testing find optimal clustering solution
+- `process(by_clusters = False, max_cpus = -1, max_queue_size = 100)`: Process the complete model
+	- `by_clusters`: if True, update the phasing by clustering sample dates
+	- `max_cpus`: Maximum number of CPUs to use for parallel processing (-1 = all available)
+	- `max_queue_size`: Maximum queue size for parallel processing
+
+#### Attributes
+
+The `Model` class has the following attributes:
+- `directory`: Working directory for model data
+- `samples`: Dictionary of samples in format `{name: Sample, ...}`
+- `curve_name`: The name of the calibration curve
+- `phase_model`: OxCal phase model type
+- `cluster_n`: Number of clusters to form
+- `uniform`: Flag indicating whether to use uniform randomization
+- `p_value`: The P-value threshold for statistical tests
+- `uncertainty_base`: The base uncertainty for randomization
+- `npass`: Minimum number of passes for the randomization tests
+- `convergence`: Convergence threshold for the randomization tests
+- `oxcal_url`: Url to download the OxCal program
+- `years`: Calendar years BP corresponding to the probability distributions in format `np.array([year, ...])`
+- `curve`: Calibration curve in format `np.array([[calendar year BP, C-14 year, uncertainty], ...])`, sorted by calendar years
+- `uncertainties`: List of uncertainties from C-14 dates of samples
+- `oxcal_data`: Results of OxCal modeling from `model.js` in format `{key: data, ...}`
+- `summed`: Summed probability distribution of the dating of all samples in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `random_p`: Calculated p-value for the randomization test
+- `random_lower`: Lower bound of the randomization test in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `random_upper`: Upper bound of the randomization test in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `areas`: List of excavation areas that the samples belong to
+- `contexts`: List of contexts that the samples belong to
+- `groups`: Groups that the samples belong to based on stratigraphic interconnection with other samples in format `{group_name: [sample name, ...], ...}`
+- `clusters`: Clusters of samples based on the similarity of their probability distributions in format `{clusters_n: [cluster: [sample name, ...], ...}, ...}`
+- `cluster_means`: Mean date of the samples in each cluster in calendar years BP in format `{clusters_n: {cluster: year, ...}, ...}`
+- `cluster_sils`: Silhouette score of each clustering solution in format `{clusters_n: silhouette, ...}`
+- `cluster_ps`: P-value of the clustering solutions in format `{clusters_n: p, ...}`
+- `cluster_opt_n`: Optimal number of clusters
+- `has_data`: Boolean indicating if the model has sample data
+- `is_modeled`: Boolean indicating if bayesian modeling of sample dates (process_dates) has been performed
+- `is_randomized`: Boolean indicating if randomization testing of the distribution of samples (process_randomization) has been performed
+- `is_clustered`: Boolean indicating if the model has been clustered (process_clustering)
+
+### Sample Class <a name="sample_class"></a>
+The `Sample` class represents a single radiocarbon sample. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Sample
+
+if __name__ == '__main__':
+	
+	# Initialize the Sample object
+	sample = Sample('Sample1', 1000, 50, phase = 1, earlier_than = ['Sample2'], long_lived = 0)
+	
+	# Print the sample data
+	print(sample)
+```
+
+#### Parameters <a name="sample_parameters"></a>
+
+The 'Sample' class constructor accepts the following parameters:
+- `name`: Sample ID (required, unique identifier)
+- `age`: C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U' (required)
+- `uncertainty`: Uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U' (required)
+- `date_type`: 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution
+- `long_lived`: True if sample is older than the examined deposition event due to e.g. old wood effect or redeposition from older strata
+- `context`: Name of the context where sample was found
+- `area`: Excavation area
+- `area_excavation_phase`: Chronological phase of the context within the excavation area (integer, lower = earlier (older) phase)
+- `earlier_than`: List of names of samples which are stratigraphically later (younger) than this sample
+- `curve`: Radiocarbon calibration curve in format `np.array([[calendar year BP, C-14 year, uncertainty], ...])`
+
+#### Methods
+
+The `Sample` class provides the following methods:
+- `calibrate(curve)`: Calibrate the sample using the provided calibration curve.
+	- `curve = np.array([[calendar year BP, C-14 year, uncertainty], ...])`
+- `set_group(group)`: Set the group number for the sample.
+- `set_phase(phase)`: Set the phase number for the sample.
+- `set_likelihood(distribution, mean = None, rng = None)`: Set the likelihood for the sample.
+	- `distribution = np.array([p, ...])`
+	- `rng = [from, to]`; 2-sigma (95.45%) range in calendar years BP
+- `set_posterior(distribution, mean = None, rng = None, agreement = 0)`: Set the posterior for the sample.
+	- `distribution = np.array([p, ...])`
+	- `rng = [from, to]`; 2-sigma (95.45%) range in calendar years BP
+	- `agreement`: agreement index generated by OxCal modeling
+- `to_oxcal()`: Convert the sample to OxCal model format (str).
+- `to_dict()`: Convert the sample data to a JSON dictionary.
+- `from_dict(data)`: Load the sample data from a JSON dictionary.
+- `copy()`: Create a copy of the sample instance.
+
+#### Attributes
+The `Sample` class has the following attributes:
+
+- `name`: Sample ID (unique identifier)
+- `age`: C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U'
+- `uncertainty`: Uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U'
+- `date_type`: 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution
+- `long_lived`: True if sample is older than the examined deposition event due to e.g. old wood effect or redeposition from older strata
+- `context`: Name of the context where sample was found
+- `area`: Excavation area
+- `area_excavation_phase`: Chronological phase of the context within the excavation area (integer, lower = earlier (older) phase)
+- `earlier_than`: List of names of samples which are stratigraphically later (younger) than this sample
+- `group`: Group that the sample belongs to based on stratigraphic interconnection with other samples
+- `phase`: Stratigraphic phase of the sample within the group (lower = earlier (older) phase)
+- `years`: Calendar years BP corresponding to the probability distributions in format `np.array([year, ...])`
+- `likelihood`: Probability distribution of the dating of the sample before Bayesian modeling in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `posterior`: Probability distribution of the dating of the sample after Bayesian modeling in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `likelihood_range`: 2-sigma (95.45%) range of the dating of the sample in calendar years BP before Bayesian modeling in format `[from, to]`
+- `likelihood_mean`: Mean calendar age of the sample in calendar years BP before Bayesian modeling
+- `posterior_range`: 2-sigma (95.45%) range of the dating of the sample in calendar years BP after Bayesian modeling in format `[from, to]`
+- `posterior_mean`: Mean calendar age of the sample in calendar years BP after Bayesian modeling
+- `posterior_agreement`: Agreement index generated by OxCal modeling
+- `is_calibrated`: Boolean indicating if the sample has been calibrated
+- `is_modeled`: Boolean indicating if posterior has been calculated using Bayesian modeling
+
 ## Developer Notes <a name="developer"></a>
 ### Preparing the Virtual Environment <a name="venv"></a>
 SiteSyncro requires [Python 3.10](https://www.python.org/downloads/).
 
 To prepare a Python virtual environment open a terminal or command prompt window and type the following commands:
 
 ```
 git clone https://github.com/demjanp/SiteSyncro.git
-
 cd sitesyncro
-
 python -m venv .venv
-
 .venv\Scripts\activate.bat
-
 python.exe -m pip install --upgrade pip
-
 pip install -e .
 ```
 
 See [Usage](#usage) on further instructions how to run the script.
 
-### Building a Windows Executable
+### Building a Windows Executable <a name="build"></a>
 To build a Windows executable, open a terminal or command prompt window and change to the `sitesyncro` folder: 
 ```
 cd SiteSyncro\sitesyncro
 ```
 Activate the virtual environment:
 ```
 .venv\Scripts\activate.bat
 ```
 Then type the following commands (this only has to be done once per virtual environment):
 ```
-python.exe -m pip install --upgrade pip
+python -m pip install --upgrade pip
 python -m pip install --upgrade build
 pip install twine
 pip install pyinstaller==6.6.0
 ```
 To build the executable, type:
 ```
 pip install -e .
 python -m build
 pyinstaller sitesyncro.spec
 ```
-You will find the executable `sitesyncro.exe` in the `dist` folder.
-
-### SiteSyncro Class
-All functions of SiteSyncro are encapsulated in the `SiteSyncro` class. Here is a basic example of how to use it:
-
-```python
-from sitesyncro import SiteSyncro
-
-# Initialize the SiteSyncro object
-ssync = SiteSyncro(input='data_sample.csv')
-
-# Load the data
-ssync.load_data()
-
-# Process the model
-ssync.process()
-
-# Plot the randomization test result
-ssync.plot_randomized()
-
-# Plot the clustering result
-ssync.plot_clusters()
-
-# Save the results to a CSV file
-ssync.save_results_csv()
-```
-
-#### Parameters <a name="parameters"></a>
-
-The `SiteSyncro` class accepts the following parameters:
-- `input`: The path to the input file.
-- `result`: The name of the result directory (default is "result").
-- `existing`: Boolean indicating whether to use existing results (default is False).
-- `curve`: The name of the calibration curve to use (default is "intcal20.14c").
-- `model`: The name of the model to use. Can be 'sequence', 'contiguous', 'overlapping', or 'none' (default is "sequence").
-- `n`: The number of clusters (-1 = automatic) (default is -1).
-- `uniform`: Boolean indicating whether to use uniform randomization (default is False).
-- `p_value`: The P-value for statistical tests (default is 0.05).
-- `uncert_base`: The base uncertainty for randomization (default is 15).
-- `npass`: The number of passes for the clustering algorithm (default is 100).
-- `convergence`: The convergence criterion for the clustering algorithm (default is 0.99).
-- `max_cpus`: The maximum number of CPUs to use (default is -1).
-- `max_queue_size`: The maximum size of the queue for parallel processing (default is 100).
-
-#### Methods
-
-The `SiteSyncro` class provides the following methods:
-- `load_data(**kwargs)`: Loads data from the input file and updates the internal data. The input file must be a CSV file with the following columns: Context, Excavation Area, C-14 Age, Uncertainty, Phase (lower = older), Earlier-Than, Long-Lived / Redeposited. For possible keyword arguments see [Parameters](#parameters).
-- `process(**kwargs)`: Processes the data. For possible keyword arguments see [Parameters](#parameters).
-- `plot_randomized(show=False)`: Plots the randomized data. If `show` is True, the plot is shown. If False, the plot is saved to a file.
-- `plot_clusters(show=False)`: Plots the clustering data. If `show` is True, the plot is shown. If False, the plot is saved to a file.
-- `save_results_csv(fcsv=None)`: Saves the results to a CSV file. If `fcsv` is None, a default file path is used.
-
-#### Attributes
-
-The `SiteSyncro` class has the following attributes:
-- `oc_data` (OxCalData): Used to store and manage the data after bayesian modelling of the radiocarbon dates with the OxCal program.
-- `rnd_data` (RandomizeData): Used to store and manage the data related to the randomization testing of the null hypothesis that the observed C-14 dates represent a normal/uniform distribution.
-- `clu_data` (ClusterData): Used to store and manage the data related to the temporal clustering of the modelled C-14 dates.
-- `oc_clu_data` (OxCalData): Used to store and manage the modelled data updated according to the temporal clustering of the C-14 dates.
-
-All variables generated by the OxCal program can be accessed using `oc_data[key]`. Use `print(oc_data)` to see a list of available keys.
-
-`OxCalData` class methods:
-- `__init__(fname=None)`: If a filename of an OxCal .js file is provided, it reads and stores the data.
-- `has_data(self)`: Returns True if the data dictionary is not empty, False otherwise.
-- `set_priors(samples, context_samples, context_area, areas, groups, phases, earlier_than, long_lived, r_dates, dates, model, curve)`: Sets the priors for the bayesian modeling.
-    ```
-    samples = [sample, ...]
-    context_samples = {context: [sample, ...], ...}
-    context_area = {context: area, ...}
-    areas = [area, ...]
-    groups = {group: [sample, ...], ...}
-    phases = {group: {sample: phase, ...}, ...}
-    long_lived = {sample: True/False, ...}
-    r_dates = {sample: (age, uncertainty), ...}
-    dates = {sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}; R = radiocarbon, U = uniform
-    ```
-- `get_likelihoods()`: Returns the likelihood distributions for each sample.
-    Format: `{name: {'prob': [p, ...], 'years': [calendar year CE, ...], 'mean': mean, 'range': [min year CE, max year CE]}}`
-    Ranges are calculated at the 95.45% (2-sigma) level.
-- `get_posteriors()`: Returns the posterior distributions for each sample. 
-    Format: `{name: {'prob': [p, ...], 'years': [calendar year CE, ...], 'mean': mean, 'range': [min year CE, max year CE], 'agreement': agreement index}}`	
-    Ranges are calculated at the 95.45% (2-sigma) level.
-- `get_samples()`: Returns the sample names.
-    Format: `[name, ...]`
-- `get_context_samples()`: Returns the contexts and their contained samples.
-    Format: `{context: [sample, ...], ...}`
-- `get_context_area()`: Returns the contexts and their areas.
-    Format: `{context: area, ...}`
-- `get_areas()`: Returns the areas.
-    Format: `[area, ...]`
-- `get_groups()`: Returns the groups based on stratigraphic links.
-    Format: `{group: [sample, ...], ...}`
-- `get_phases()`: Returns the phases for each group and sample. Lower = earlier (older) phase.
-    Format: `{group: {sample: phase, ...}, ...}`
-- `get_earlier_than()`: Returns the earlier-than relations between samples.
-    Format: `matrix[n_samples x n_samples] = [True/False, ...]`. Sample in row is earlier than sample in column based on stratigraphy.
-- `get_long_lived()`: Returns the long-lived value for each sample.
-    Format: `{sample: True/False, ...}`
-- `get_r_dates()`: Returns the radiocarbon dates for each sample.
-    Format: `{sample: (age, uncertainty), ...}`
-- `get_dates()`: Returns the date for bayesian modeling for each sample. Long-lived or redeposited samples are represented by a uniform distribution where the lower boundary is the lower boundary of the 2-sigma range of the calibrated date and the upper boundary is 1950 CE. 
-    Format: `{sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}`; R = radiocarbon, U = uniform
-- `get_model()`: Returns the model type used for the bayesian modeling.
-    Values: 'sequence', 'contiguous', 'overlapping', 'none'
-- `get_curve()`: Returns the calibration curve used.
-    Format: curve name (see OxCal\bin folder for available curves)
-
-`ClusterData` class methods:
-- `__init__(clusters = {}, means = {}, sils = {}, ps = {}, p_value = None, opt_n = None)`
-    ```
-    means = {n: mean, ...}
-    sils = {sample: sil, ...}
-    ps = {n: p, ...}
-    p_value = p-value threshold for randomization testing
-    opt_n = optimal number of clusters
-	```	
-- `has_data()`: Returns True if the clusters dictionary is not empty, False otherwise.
-- `get_clusters()`: Returns the clusters for each number of clusters.
-    Format: `{n: {sample: cluster, ...}, ...}`
-- `get_means()`: Returns the mean silhouette score for each number of clusters.
-    Format: `{n: mean, ...}`
-- `get_sils()`: Returns the silhouette score for each sample.
-    Format: `{sample: sil, ...}`
-- `get_ps()`: Returns the p-value for each number of clusters.
-    Format: `{n: p, ...}`
-- `get_p_value()`: Returns the p-value threshold for randomization testing.
-- `get_opt_n()`: Returns the optimal number of clusters.
-
-`RandomizeData` class methods:
-- `__init__(years = None, sum_obs = None, uniform = None, p = None, p_value = None, sums_rnd_lower = None, sums_rnd_upper = None)`
-    ```
-    years = [year, ...]. The years are in calendar years BP.
-    sum_obs = [p, ...] in order of the years.
-    uniform = True/False
-    p = calculated p-value
-    p_value = p-value threshold
-    sums_rnd_lower = [p, ...] in order of the years.
-    sums_rnd_upper = [p, ...] in order of the years.
-	```
-- `has_data()`: Returns True if the years attribute is not None, False otherwise.
-- `get_years()`: Returns the years for the randomization test.
-    Format: `[year, ...]`. The years are in calendar years BP.
-- `get_sum_obs()`: Returns the sum of the observed distributions.
-    Format: `[p, ...]` in order of the years.
-- `get_uniform()`: Returns True if the uniform distribution was used.
-- `get_p()`: Returns the calculated p-value for the randomization test.
-- `get_p_value()`: Returns the p-value threshold for the randomization test.
-- `get_sums_rnd_lower()`: Returns the lower boundary of the randomized distributions.
-    Format: `[p, ...]` in order of the years.
-- `get_sums_rnd_upper()`: Returns the upper boundary of the randomized distributions.
-    Format: `[p, ...]` in order of the years.
+The executable `sitesyncro.exe` will be created in the `dist` folder.
 
 ## Contact: <a name="contact"></a>
 Peter Demján (peter.demjan@gmail.com)
 
 Institute of Archaeology of the Czech Academy of Sciences, Prague, v.v.i.
 
 ## Acknowledgements <a name="acknowledgements"></a>
 
 Development of this software was supported by project OP JAC "Ready for the future: understanding long-term resilience of the human culture (RES-HUM)", Reg. No. CZ.02.01.01/00/22_008/0004593 of the Ministry of Education, Youth, and Sports of the Czech Republic and EU.
 
 This software requires the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program for bayesian modeling of the radiocarbon dates.
 
 This software uses the following open source packages:
-* [NumPy](https://www.numpy.org/)
-* [SciPy](https://scipy.org/)
 * [Matplotlib](https://matplotlib.org/)
+* [NetworkX](https://networkx.org/)
+* [NumPy](https://www.numpy.org/)
+* [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
+* [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
-* [Requests](https://requests.readthedocs.io/)
-* [NetworkX](https://networkx.org/)
 
 ## License <a name="license"></a>
 
-This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
+This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
```

### Comparing `sitesyncro-0.9/setup.py` & `sitesyncro-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="sitesyncro",
-    version="0.9",
+    version="0.9.1",
     description="SiteSyncro - Site-specific chronological modeling and synchronization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/demjanp/SiteSyncro",
     author="Peter Demjan",
     author_email="peter.demjan@gmail.com",
     classifiers=[
```

### Comparing `sitesyncro-0.9/src/sitesyncro/lib/fnc_cluster.py` & `sitesyncro-0.9.1/src/sitesyncro/utils/fnc_cluster.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from sitesyncro.lib.fnc_sum import (sum_distributions, calc_mean_std)
-from sitesyncro.lib.fnc_simulate import (calculate_parameters, generate_random_distributions)
-from sitesyncro.lib.fnc_mp import (process_mp)
+from sitesyncro.utils.fnc_mp import (process_mp)
+from sitesyncro.utils.fnc_stat import (calc_sum, calc_mean_std, samples_to_distributions)
+from sitesyncro.utils.fnc_simulate import (calculate_parameters, generate_random_distributions)
 
 import numpy as np
+from tqdm import tqdm
 from scipy.stats import norm
 from itertools import combinations
 from sklearn.decomposition import PCA
 from sklearn.metrics import silhouette_score
 from scipy.spatial.distance import squareform
 from scipy.cluster.hierarchy import linkage, fcluster
 
@@ -89,126 +90,147 @@
 	
 	clusters_l = np.zeros(D.shape[0], dtype = int)
 	for li, label in enumerate(list(clusters.keys())):
 		clusters_l[clusters[label]] = li + 1
 	
 	return silhouette_score(D, clusters_l, metric = "precomputed")
 
-def cluster_distributions(distributions, years, clusters_n):
+def cluster_distributions(model):
 	# Cluster distributions into n clusters using Hierarchical Cluster Analysis
-	# distributions = {sample: [p, ...], ...}
 	#
 	# Returns clusters, means, silhouette
 	# 	clusters = {label: [sample, ...], ...}
 	#   means = {label: mean, ...}
+	#	silhouette = mean value for all clusters
 	
-	samples = sorted(list(distributions.keys()))
-	distributions = [distributions[sample] for sample in samples]
+	if model.cluster_n < 2:
+		raise Exception("Number of clusters must be >1")
+	
+	samples = []
+	distributions = []
+	for name in model.samples:
+		if model.samples[name].is_modeled:
+			samples.append(name)
+			distributions.append(model.samples[name].posterior)
+	# distributions = [[p, ...], ...]; ordered by samples
+	
+	if not samples:
+		raise Exception("No modeled samples found")
 	
 	D = calc_distance_matrix(distributions)
-	clusters = calc_clusters_hca(D, clusters_n)
+	clusters = calc_clusters_hca(D, model.cluster_n)
 	means = {}
 	for label in clusters:
 		means[label] = np.average(
-			years,
-			weights=sum_distributions([distributions[idx] for idx in clusters[label]])
+			model.years,
+			weights=calc_sum([distributions[idx] for idx in clusters[label]])
 		)
 	sil = calc_silhouette(D, clusters)
 	clusters = dict([(label, [samples[idx] for idx in clusters[label]]) for label in clusters])
 	
 	return clusters, means, sil
 
-def worker_fnc(params, clusters_n, dates_n, t_param1, t_param2, uncert_base, curve, uniform):
+def worker_fnc(params, cluster_n, dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform):
 	
-	distributions = generate_random_distributions(dates_n, t_param1, t_param2, uncert_base, curve, uniform)
+	distributions = generate_random_distributions(dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform)
 	D = calc_distance_matrix(distributions)
-	sil = calc_silhouette(D, calc_clusters_hca(D, clusters_n))
+	sil = calc_silhouette(D, calc_clusters_hca(D, cluster_n))
 	
 	return sil
 
-def collect_fnc(data, results):
+def collect_fnc(data, results, pbar):
 	
 	# data = sil
+	pbar.update(1)
 	results.append(data)
 
-def progress_fnc(done, todo, clusters_n, clu_max, all_done, all_todo, c):
-	
-	print("\rClusters: %d/%d, Iteration: %d/%d, Conv: %0.4f         " % (clusters_n, clu_max, all_done + done, all_todo, c), end = "")
-
-def test_distribution_clustering(distributions, curve, 
-		uncert_base = 15, uniform = False,
-		npass = 100, convergence = 0.99, max_cpus = -1, max_queue_size = 100):
+def test_distribution_clustering(model, max_cpus = -1, max_queue_size = 100):
 	# Test the clustering of distributions for randomness
 	#
-	# distributions = {sample: [p, ...], ...}
-	# curve: [[CalBP, ConvBP, CalSigma], ...]
-	# uncert_base: base uncertainty to simulate the radiocarbon dates
-	# uniform: flag indicating whether to use a uniform distribution for the calendar ages
-	#
 	# returns clusters, means, sils, ps
 	# 	clusters = {n: {label: [sample, ...], ...}, ...}; n = number of clusters
 	#   means = {n: {label: mean, ...}, ...}
 	#	sils = {n: Silhouette, ...}
 	#	ps = {n: p-value, ...}; p-value of the null hypothesis that the 
 	#		Silhouette for n clusters is the product of randomly distributed dates
 	
-	samples = sorted(list(distributions.keys()))
-	distributions = [distributions[sample] for sample in samples]
-	dates_n = len(distributions)
-	
-	years = curve[:, 0]
-	sum_obs = sum_distributions(distributions)
-	t_param1, t_param2 = calculate_parameters(years, sum_obs, uniform)
-	
-	clusters = {}  # {clusters_n: {label: [idx, ...], ...}, ...}; idx = index in samples
-	sils = {} # {clusters_n: silhouette_score, ...}
-	means = {} # {clusters_n: {label: mean, ...}, ...}
+	distributions, samples, joined = samples_to_distributions(model.samples.values())
+	# distributions = [[p, ...], ...]
+	# samples = [sample name, ...] ordered by distributions
+	# joined = {combined_name: [sample name, ...], ...}
+	
+	dates_n = len(samples)
+	
+	if dates_n < 3:
+		raise Exception("Insufficient number samples for testing of clustering.")
+	
+	print("Testing clustering of %d distributions" % dates_n)
+	
+	sum_obs = calc_sum(distributions)
+	t_param1, t_param2 = calculate_parameters(model.years, sum_obs, model.uniform)
+	
+	clusters = {}  # {cluster_n: {label: [idx, ...], ...}, ...}; idx = index in samples
+	sils = {} # {cluster_n: silhouette_score, ...}
+	means = {} # {cluster_n: {label: mean, ...}, ...}
 	D = calc_distance_matrix(distributions)
-	for clusters_n in range(2, dates_n - 1):
-		clusters[clusters_n] = calc_clusters_hca(D, clusters_n)
-		sils[clusters_n] = calc_silhouette(D, clusters[clusters_n])
-		means[clusters_n] = {}
-		for label in clusters[clusters_n]:
-			means[clusters_n][label] = np.average(
-				years,
-				weights=sum_distributions([distributions[idx] for idx in clusters[clusters_n][label]])
+	for cluster_n in range(2, dates_n - 1):
+		clusters[cluster_n] = calc_clusters_hca(D, cluster_n)
+		sils[cluster_n] = calc_silhouette(D, clusters[cluster_n])
+		means[cluster_n] = {}
+		for label in clusters[cluster_n]:
+			means[cluster_n][label] = np.average(
+				model.years,
+				weights=calc_sum([distributions[idx] for idx in clusters[cluster_n][label]])
 			)
-		clusters[clusters_n] = dict([(label, [samples[idx] for idx in clusters[clusters_n][label]]) for label in clusters[clusters_n]])
+		# convert clusters to {cluster_n: {label: [sample name, ...], ...}, ...}
+		clusters[cluster_n] = dict([(label, [samples[idx] for idx in clusters[cluster_n][label]]) for label in clusters[cluster_n]])
 	
 	clu_max = dates_n - 1
 	
 	# Calculate the mean or median and standard deviation or range of the summed distribution
 	ps = {}
-	for clusters_n in clusters:
+	for cluster_n in clusters:
 		sils_rnd = []
 		sils_prev = None
 		c = 0
-		params_list = list(range(npass))
-		todo = npass
-		while True:
-			process_mp(worker_fnc, params_list, [clusters_n, dates_n, t_param1, t_param2, uncert_base, curve, uniform],
-				collect_fnc = collect_fnc, collect_args = [sils_rnd],
-				progress_fnc = progress_fnc, progress_args = [clusters_n, clu_max, len(sils_rnd), npass*2, c],
-				max_cpus = max_cpus, max_queue_size = max_queue_size)
-			if len(sils_rnd) >= todo:
-				sils_m = np.array(sils_rnd).mean()
-				if sils_prev is not None:
-					c = 1 - np.abs(sils_prev - sils_m) / sils_prev
-				sils_prev = sils_m
-				if c >= convergence:
-					print("\nConverged at:", c)
-					break
-				todo *= 2
+		todo = model.npass
+		params_list = list(range(model.npass))
+		with tqdm(total=todo) as pbar:
+			pbar.total = model.npass*2
+			pbar.set_description("Clusters: %d/%d, Conv.: %0.3f" % (cluster_n, clu_max, c))
+			while True:
+				process_mp(worker_fnc, params_list, [cluster_n, dates_n, t_param1, t_param2, model.uncertainties, model.uncertainty_base, model.curve, model.uniform],
+		           collect_fnc = collect_fnc, collect_args = [sils_rnd, pbar],
+		           max_cpus = max_cpus, max_queue_size = max_queue_size)
+				if len(sils_rnd) >= todo:
+					sils_m = np.array(sils_rnd).mean()
+					if sils_prev is not None:
+						c = 1 - np.abs(sils_prev - sils_m) / sils_prev
+						pbar.set_description("Clusters: %d/%d, Conv.: %0.3f" % (cluster_n, clu_max, c))
+					sils_prev = sils_m
+					if c >= model.convergence:
+						break
+					todo *= 2
+					pbar.total = max(todo, model.npass*2)
 		sils_rnd = np.array(sils_rnd)
 		s = sils_rnd.std()
 		if s == 0:
 			p = 0
 		else:
-			p = 1 - float(norm(sils_rnd.mean(), s).cdf(sils[clusters_n]))
-		ps[clusters_n] = p				
+			p = 1 - float(norm(sils_rnd.mean(), s).cdf(sils[cluster_n]))
+		ps[cluster_n] = p
+	
+	# Split joined samples
+	if joined:
+		for cluster_n in clusters:
+			for label in clusters[cluster_n]:
+				for name in joined:
+					if name in clusters[cluster_n][label]:
+						clusters[cluster_n][label].remove(name)
+						clusters[cluster_n][label] += joined[name]
 	
 	return clusters, means, sils, ps
 
 def find_opt_clusters(clusters, ps, sils, p_value = 0.05):
 	# Find optimal number of clusters based on Silhouette scores and p-values of clustering solutions
 	#
 	# clusters = {n: {label: [sample, ...], ...}, ...}; n = number of clusters
@@ -222,7 +244,27 @@
 	sils = np.array([sils[clu_n] for clu_n in clu_ns])
 	idxs = np.where(ps < p_value)[0]
 	if not idxs.size:
 		return None
 	
 	return int(clu_ns[idxs[np.argmax(sils[idxs])]])
 
+def proc_clustering(model, max_cpus = -1, max_queue_size = 100):
+	if model.cluster_n > -1:
+		clusters, means, sil = cluster_distributions(model)
+		clusters = {model.cluster_n: clusters}
+		means = {model.cluster_n: means}
+		sils = {model.cluster_n: sil}
+		ps = {model.cluster_n: 1}
+		opt_n = model.cluster_n
+	else:
+		clusters, means, sils, ps = test_distribution_clustering(model, max_cpus, max_queue_size)
+		opt_n = find_opt_clusters(clusters, ps, sils, model.p_value)
+	if opt_n is None:
+		opt_n = 0
+		clusters[0] = {0: sorted(list(model.samples.keys()))}
+		means[0] = {0: 0}
+		sils[0] = 0
+		ps[0] = 1
+		
+	return clusters, means, sils, ps, opt_n
+
```

### Comparing `sitesyncro-0.9/src/sitesyncro/lib/fnc_load.py` & `sitesyncro-0.9.1/src/sitesyncro/utils/fnc_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict
 import os
 
-def load_input(input_path):
+def load_input(fname):
 	data = []
-	with open(input_path, "r") as file:
+	with open(fname, "r") as file:
 		next(file)  # Skip header
 		for line in file:
 			line = line.strip()
 			if line:
 				elements = line.split(";")
 				if len(elements) != 8:
 					raise Exception(f"Incorrect data format in line: {line}")
@@ -116,25 +116,43 @@
 				pass
 	if n is not None:
 		n += 1
 		result_path = os.path.join(parent_dir, os.path.basename(result_path) + "_" + str(n))
 	os.makedirs(result_path)
 	return result_path
 
-def load_data(input_path):
-	data = load_input(input_path)
+def load_data(fname):
+	data = load_input(fname)
 	samples, context_samples, context_area, areas = get_samples_contexts_and_areas(data)
 	long_lived = get_long_lived(data)
 	r_dates = get_c14_dates(data)
 	context_phase = get_context_phase(data)
 	earlier_than_rel = get_earlier_than_relations(data, context_samples)
 	
 	# samples = [sample, ...]
-	# context_samples = {context: [sample, ...], ...}
+	# contexts = {sample: context, ...}
 	# context_area = {context: area, ...}
-	# areas = [area, ...]
 	# long_lived = {sample: True/False, ...}
 	# r_dates = {sample: (age, uncertainty), ...}
 	# context_phase = {context: phase, ...}
 	# earlier_than_rel = {sample: [sample, ...], ...}
 	
-	return samples, context_samples, context_area, areas, long_lived, r_dates, context_phase, earlier_than_rel
+	contexts = {}
+	for context in context_samples:
+		for sample in context_samples[context]:
+			contexts[sample] = context
+		if context not in context_area:
+			context_area[context] = None
+		if context not in context_phase:
+			context_phase[context] = None
+		
+	for sample in samples:
+		if sample not in contexts:
+			contexts[sample] = None
+		if sample not in long_lived:
+			long_lived[sample] = False
+		if sample not in r_dates:
+			r_dates[sample] = (None, None)
+		if sample not in earlier_than_rel:
+			earlier_than_rel[sample] = {}
+	
+	return samples, contexts, context_area, long_lived, r_dates, context_phase, earlier_than_rel
```

### Comparing `sitesyncro-0.9/src/sitesyncro/lib/fnc_mp.py` & `sitesyncro-0.9.1/src/sitesyncro/utils/fnc_mp.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9/src/sitesyncro/lib/fnc_oxcal.py` & `sitesyncro-0.9.1/src/sitesyncro/utils/fnc_oxcal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from sitesyncro.lib.fnc_data import (OxCalData)
-from sitesyncro.lib.fnc_phase import (update_earlier_than_matrix, get_groups_and_phases)
-
 import os
-import requests
+import re
 import zipfile
+import requests
 import subprocess
+import numpy as np
 from tqdm import tqdm
 from collections import defaultdict
+from scipy.interpolate import interp1d
 
 def download_oxcal(url = None):
 	
 	if os.path.isfile("OxCal\\bin\\OxCalWin.exe"):
 		return True
 	# Download and unzip OxCal from url to the current directory
 	
@@ -44,60 +44,33 @@
 		zip_ref.extractall()
 	
 	# Remove the zip file
 	os.remove(local_zip)
 	
 	return True
 
-def run_oxcal(fmodel, url = None):
-	
-	if not download_oxcal(url):
-		raise Exception("OxCal not found")
-	r = subprocess.call("OxCal\\bin\\OxCalWin.exe %s" % (fmodel))
-
-def gen_dates(dates):
-	
-	txt = ""
-	for lab_code, d1, d2, typ in dates:
-		if typ == "R":
-			txt += '''
-					R_Date("%s", %f, %f);
-			''' % (lab_code, d1, d2)
-		elif typ == "U":
-			txt += '''
-				Date("%s", U(CE(%f), CE(%f)));
-			''' % (lab_code, d1, d2)
-		else:
-			raise Exception("Invalid date type specified: %s (must be 'R' or 'U')" % (typ))
-	return txt
-
-def gen_oxcal_calib(dates, curve_name = 'intcal20.14c'):
-	# Generate OxCal calibration model
-	# dates = [(name, c14age, uncert, 'R'), ...]
-	
-	return '''
-Curve("%s","%s");
-Plot()
-{
-	%s
-};
-	''' % (curve_name, curve_name, gen_dates(dates))
+def oxcal_date(name, age, uncertainty, date_type):
+	if date_type == 'R':
+		return '''R_Date("%s", %f, %f);''' % (name, age, uncertainty)
+	if date_type == 'U':
+		return '''Date("%s", U(CE(%f), CE(%f)));''' % (name, -(age + uncertainty - 1950), -(age - uncertainty - 1950))
+	raise Exception("Invalid date type specified: %s (must be 'R' or 'U')" % (date_type))
 
 def gen_sequence(name, data):
 	
 	txt = ""
 	for phase in sorted(list(data.keys())):
 		txt += '''
 		Boundary("Start %(name)s-%(phase)d");
 		Phase("%(name)s-%(phase)d")
 		{
 			%(dates)s
 		};
 		Boundary("End %(name)s-%(phase)d");
-		''' % dict(name = name, phase = phase, dates = gen_dates(data[phase]))
+		''' % dict(name = name, phase = phase, dates = data[phase])
 	
 	return '''
 	Sequence(%s)
 	{
 		%s
 	};
 	''' % (name, txt)
@@ -116,15 +89,15 @@
 		Boundary("Transition %s-%d/%s-%d");
 			''' % (name, last_phase, name, phase)
 		txt += '''
 		Phase("%s-%d")
 		{
 			%s
 		};
-		''' % (name, phase, gen_dates(data[phase]))
+		''' % (name, phase, data[phase])
 		last_phase = phase
 	txt += '''
 		Boundary("End %s-%d");
 	''' % (name, last_phase)
 	
 	return '''
 	Sequence(%s)
@@ -143,136 +116,226 @@
 			Boundary("Start %(name)s-%(phase)d");
 			Phase("%(name)s-%(phase)d")
 			{
 				%(dates)s
 			};
 			Boundary("End %(name)s-%(phase)d");
 		};
-		''' % dict(name = name, phase = phase, dates = gen_dates(data[phase]))
+		''' % dict(name = name, phase = phase, dates = data[phase])
 	return '''
 	Phase(%s)
 	{
 		%s
 	};
 	''' % (name, txt)
 
 def gen_none(name, data):
 	
 	txt = ""
 	for phase in sorted(list(data.keys())):
 		txt += '''
 		Label("%s-%d");
 		%s
-		''' % (name, phase, gen_dates(data[phase]))
+		''' % (name, phase, data[phase])
 	return txt
 
-def gen_oxcal_model(dates, phases, model, curve_name = 'intcal20.14c'):
-	# dates = {sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}
-	# phases = {group: {sample: phase, ...}, ...}
+def gen_oxcal_model(model):
 	
 	model_fncs = {
 		'sequence': gen_sequence,
 		'contiguous': gen_contiguous,
 		'overlapping': gen_overlapping,
 		'none': gen_none,
 	}
-	if model not in model_fncs:
-		raise Exception("Invalid model specified: %s" % (model))
+	if model.phase_model not in model_fncs:
+		raise Exception("Invalid model specified: %s" % (model.phase_model))
 	
 	txt = ''
-	for group in phases:
+	groups = model.groups
+	for group in groups:
 		data = defaultdict(list)
-		for sample in phases[group]:
-			data[phases[group][sample]].append([sample] + list(dates[sample]))
+		for name in groups[group]:
+			data[model.samples[name].phase].append(model.samples[name])
+		data = dict(data)
+		for phase in data:
+			data[phase] = sorted(data[phase], key = lambda sample: sum(sample.likelihood_range))
+			data[phase] = "\n".join([sample.to_oxcal() for sample in data[phase]])
+			
 		if len(data) > 1:
-			txt += model_fncs[model]("Gr.%d" % (group), data)
+			txt += model_fncs[model.phase_model]("Gr.%d" % (group), data)
 		else:
 			txt += model_fncs['none']("Gr.%d" % (group), data)
 	
 	return '''
 Curve("%s","%s");
 Plot()
 {
 	%s
 };
-	''' % (curve_name, curve_name, txt)
-
+	''' % (model.curve_name, model.curve_name, txt)
 
-def r_dates_to_dates(long_lived, r_dates, curve_name, result_path):
-	# Convert radiocarbon dates to dates for modeling
+def load_oxcal_data(fname):
 	
-	# Calibrate radiocarbon dates of long-lived samples and calculate their 2-sigma ranges
-	ranges_2sig = {}
-	if any(long_lived.values()):
-		txt = gen_oxcal_calib([[sample] + list(r_dates[sample]) + ['R'] for sample in long_lived], curve_name)
-		fcalib = os.path.join(result_path, "calib.oxcal")
-		with open(fcalib, "w") as file:
-			file.write(txt)
-		run_oxcal(fcalib)
-		data = OxCalData(os.path.join(result_path, "calib.js"))
-		likelihoods = data.get_likelihoods()
-		for name in likelihoods:
-			ranges_2sig[name] = likelihoods[name]['range']
-	# ranges_2sig = {sample: (lower, upper), ...}
-	
-	# Generate dates for modeling
-	dates = {}
-	for sample in r_dates:
-		if long_lived[sample]:
-			# If the sample is long-lived, use the oldest date in the 2-sigma range as lower boundary and 1950 CE as upper boundary
-			dates[sample] = (ranges_2sig[sample][0], 1950, 'U')
-		else:
-			dates[sample] = (r_dates[sample][0], r_dates[sample][1], 'R')
-	# dates = {sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}
-	
-	return dates
+	def replace_colons_in_braces(s):
+		# Find the innermost braces
+		inner_braces = re.findall(r'\{[^{}]*\}', s)
+		if not inner_braces:
+			return s
+		
+		for brace in inner_braces:
+			# Replace colons in the innermost braces
+			s = s.replace(brace, "dict(%s)" % brace.replace(':', '=')[1:-1])
+		
+		# Recursively process the modified string
+		return replace_colons_in_braces(s)
+
+	def read_js_file(file_path):
+		
+		data = {}
+		
+		with (open(file_path, 'r') as file):
+			for line in file:
+				if line.startswith('if('):
+					continue
+				
+				# Replace last character of line with a comma
+				line = line[:-2] + ',' + line[-1]
+				
+				# Put everything before "=" in quotes
+				line = line.split('=')
+				line = [line[0], '='.join(line[1:])]
+				
+				key, value = line
+				key = key.strip()
+				value = value.strip().strip(',')
+				
+				value = replace_colons_in_braces(value)
+				
+				# Replace NaN (only if whole word) with None
+				value = re.sub(r'\bNaN\b', 'None', value)
+				
+				# Parse value using python eval
+				value = eval(value)
+				if value == []:
+					value = {}
+				
+				keys = key.split('.')
+				collect = []
+				for key in keys:
+					index1 = None
+					index2 = None
+					if '[' in key:
+						key, index = key.split('[', 1)
+						index1 = int(index.split(']')[0])
+						index2 = None
+						if '[' in index:
+							index2 = int(index.split('[')[1].split(']')[0])
+					if index2 is not None:
+						collect += [key, index1, index2]
+					elif index1 is not None:
+						collect += [key, index1]
+					else:
+						collect.append(key)
+				keys = collect
+				
+				current = data
+				for i, key in enumerate(keys):
+					if i == len(keys) - 1:
+						current[key] = value
+					elif key not in current:
+						current[key] = {}
+					current = current[key]
+		
+		return data
+
+	
+	if not os.path.isfile(fname):
+		raise Exception("Data file %s not found" % (fname))
+	
+	return read_js_file(fname)
+
+def get_distributions(data, curve):
+	# data = OxCal data (from load_oxcal_data)
+	# curve = np.array([[calendar year BP, C-14 year, uncertainty], ...]), sorted by calendar years
+	#
+	# returns likelihoods, posteriors
+	# likelihoods = {name: [distribution, mean, rng], ...}
+	# posteriors = {name: [distribution, mean, rng, agreement], ...}
+	
+	def _get_params(params_data):
+		mean = None
+		if 'mean' in params_data:
+			mean = 1950 - params_data['mean']
+		prob = params_data['prob']
+		start = params_data['start']
+		resolution = params_data['resolution']
+		years = [start + j * resolution for j in range(len(prob))]
+		rng = (None, None)
+		if ('range' in params_data) and (2 in params_data['range']):
+			L = np.inf
+			U = -np.inf
+			for key in params_data['range'][2]:
+				L = min(L, params_data['range'][2][key][0])
+				U = max(U, params_data['range'][2][key][1])
+			rng = (1950 - L, 1950 - U)
+		return mean, rng, prob, years
+	
+	def _unify(dist, years, curve):
+		# years are in CE
+		all_years = curve[:,0]
+		years = 1950 - np.array(years)
+		# Make sure years are in the correct order
+		if np.sign(years[-1] - years[0]) != np.sign(all_years[-1] - all_years[0]):
+			years = years[::-1]
+			dist = dist[::-1]
+		years = np.concatenate(([all_years[0]], years, [all_years[-1]]))
+		dist = np.concatenate(([0], dist, [0]))
+		s = dist.sum()
+		if s > 0:
+			dist /= s
+		new_prob = interp1d(years, dist, kind="linear")(all_years)
+		s = new_prob.sum()
+		if s > 0:
+			new_prob /= s
+		return new_prob
+	
+	def _load_likelihoods(data):
+		result = {}
+		if 'ocd' not in data:
+			return
+		for i in data['ocd']:
+			if i == 0:
+				continue
+			if 'likelihood' not in data['ocd'][i]:
+				continue
+			if 'prob' not in data['ocd'][i]['likelihood']:
+				continue
+			name = data['ocd'][i]['name'].strip()
+			mean, rng, prob, years = _get_params(data['ocd'][i]['likelihood'])
+			result[name] = [_unify(prob, years, curve), mean, rng]
+		return result
+	
+	def _load_posteriors(data):
+		result = {}
+		if 'ocd' not in data:
+			return result
+		for i in data['ocd']:
+			if i == 0:
+				continue
+			if 'posterior' not in data['ocd'][i]:
+				continue
+			if 'prob' not in data['ocd'][i]['posterior']:
+				continue
+			if 0 not in data['ocd'][i]['posterior']['comment']:
+				continue
+			name = data['ocd'][i]['posterior']['comment'][0][:-10].strip()
+			agreement = None
+			if 'agreement' in data['ocd'][i]['posterior']:
+				agreement = data['ocd'][i]['posterior']['agreement']
+			mean, rng, prob, years = _get_params(data['ocd'][i]['posterior'])
+			result[name] = [_unify(prob, years, curve), mean, rng, agreement]
+		return result
+	
+	likelihoods = _load_likelihoods(data)
+	posteriors = _load_posteriors(data)
+	return likelihoods, posteriors
 
-def run_model(dates, phases, model, curve_name, result_path):
-	txt = gen_oxcal_model(dates, phases, model, curve_name)
-	fmodel = os.path.join(result_path, "model.oxcal")
-	with open(fmodel, "w") as file:
-		file.write(txt)
-	run_oxcal(fmodel)
-	data = OxCalData(os.path.join(result_path, "model.js"))
-	return data
-
-def update_model_by_clustering(oc_data, clu_data, result_path):
-	
-	samples = oc_data.get_samples()
-	context_samples = oc_data.get_context_samples()
-	context_area = oc_data.get_context_area()
-	areas = oc_data.get_areas()
-	earlier_than = oc_data.get_earlier_than()
-	long_lived = oc_data.get_long_lived()
-	r_dates = oc_data.get_r_dates()
-	dates = oc_data.get_dates()
-	model = oc_data.get_model()
-	curve_name = oc_data.get_curve()
-	
-	clusters = clu_data.get_clusters()
-	means = clu_data.get_means()
-	opt_n = clu_data.get_opt_n()
-	
-	if opt_n is None:
-		raise ValueError("Optimal number of clusters not found")
-	
-	clusters = clusters[opt_n]  # clusters = {label: [sample, ...], ...}
-	means = means[opt_n]  # means = {label: mean, ...}
-	
-	# Update earlier_than and phasing based on temporal clustering of the samples
-	earlier_than = update_earlier_than_matrix(earlier_than, samples, clusters, means)
-	groups, phases = get_groups_and_phases(earlier_than, samples)
-	
-	# Generate OxCal model
-	txt = gen_oxcal_model(dates, phases, model, curve_name)
-	fmodel = os.path.join(result_path, "clu_model.oxcal")
-	with open(fmodel, "w") as file:
-		file.write(txt)
-
-	# Run OxCal model
-	run_oxcal(fmodel)
-	
-	# Save results
-	data = OxCalData(os.path.join(result_path, "clu_model.js"))
-	data.set_priors(samples, context_samples, context_area, areas, groups, phases, earlier_than, long_lived, r_dates, dates, model, curve_name)
-	
-	return data
```

### Comparing `sitesyncro-0.9/src/sitesyncro/lib/fnc_phase.py` & `sitesyncro-0.9.1/src/sitesyncro/utils/fnc_phase.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 
 def check_circular_relationships(earlier_than, samples):
-	
 	G = nx.convert_matrix.from_numpy_array(earlier_than, create_using=nx.DiGraph)
 	cycles = list(nx.simple_cycles(G))
 	if cycles:
 		print("Circular relationships detected:")
 		for cycle in cycles:
 			cycle_samples = [samples[i] for i in cycle]
 			print(" -> ".join(cycle_samples))
 		return False
-	
-	print("No circular relationships detected.")
 	return True
 
 def visualize_earlier_than(earlier_than, samples):
-	
 	G = nx.convert_matrix.from_numpy_array(earlier_than, create_using=nx.DiGraph)
 	labels = {i: sample for i, sample in enumerate(samples)}
 	pos = nx.spring_layout(G)
 	nx.draw(G, pos, labels=labels, with_labels=True)
 	plt.show()
 
 def extend_earlier_than(earlier_than):
@@ -33,99 +29,53 @@
 
 	# Convert the transitive closure graph back to a matrix
 	extended_earlier_than = nx.convert_matrix.to_numpy_array(transitive_closure)
 
 	return extended_earlier_than.astype(bool)
 
 def find_groups(earlier_than):
-	
 	G = nx.convert_matrix.from_numpy_array(earlier_than, create_using = nx.Graph)
 	groups = []
 	for c in nx.connected_components(G):
 		G_sub = G.subgraph(c)
 		groups.append(list(G_sub.nodes))
 	
 	# groups = {group: [idx, ...], ...}; idx = index in earlier_than
 	return dict(enumerate(sorted(groups, key = lambda group: len(group), reverse = True), start = 1))
 
-def create_earlier_than_matrix(context_phase, earlier_than_rel, samples, context_samples, context_area):
+def create_earlier_than_matrix(model):
+	samples = sorted(list(model.samples.keys()))
 	
 	# Create a matrix of earlier-than relationships
 	earlier_than = np.zeros((len(samples), len(samples)), dtype=bool)
-	for s1 in earlier_than_rel:
-		i = samples.index(s1)
-		for s2 in earlier_than_rel[s1]:
+	for i, s1 in enumerate(samples):
+		for s2 in model.samples[s1].earlier_than:
 			j = samples.index(s2)
 			earlier_than[i][j] = True
 	
 	# Update earlier-than relationships based on phases
-	for c1 in context_samples:
-		a1 = context_area[c1]
-		for c2 in context_samples:
-			a2 = context_area[c2]
-			if (a1 != a2):
-				continue
-			for sample1 in context_samples[c1]:
-				i = samples.index(sample1)
-				for sample2 in context_samples[c2]:
-					j = samples.index(sample2)
-					if (context_phase[c1] < context_phase[c2]):
-						earlier_than[i][j] = True
-					elif (context_phase[c2] < context_phase[c1]):
-						earlier_than[j][i] = True
-	
-	# Check if earlier_than has circular relationships
-	if not check_circular_relationships(earlier_than, samples):
-		# Visualize earlier_than as a DAG
-		visualize_earlier_than(earlier_than, samples)
-		raise Exception("Circular relationships detected")
-		
-	# Extend the earlier_than matrix to include computed relations
-	earlier_than = extend_earlier_than(earlier_than)
-	
-	# earlier_than: matrix[n_samples x n_samples] = [True/False, ...]; sample in row is earlier than sample in column based on stratigraphy
-	
-	return earlier_than
-
-def update_earlier_than_matrix(earlier_than, samples, clusters, means):
-	# Update earlier_than based on temporal clustering of the samples
-	#
-	# clusters = {label: [sample, ...], ...}
-	# means = {label: mean, ...}
-	
-	# Sort clusters from oldest to youngest
-	labels = sorted(clusters.keys(), key=lambda label: means[label], reverse=True)
-	
-	phases_clu = dict((label, idx + 1) for idx, label in enumerate(labels))
-	# phases_clu = {label: phase, ...}; lower phase = earlier
-	
-	phases = {}
-	for label in phases_clu:
-		for sample in clusters[label]:
-			phases[sample] = phases_clu[label]
-	# phases = {sample: phase, ...}
-	
-	# Update earlier-than relationships based on phases derived from clustering
 	for i, s1 in enumerate(samples):
 		for j, s2 in enumerate(samples):
-			if phases[s1] < phases[s2]:
+			if s2 == s1:
+				continue
+			if model.samples[s1].area != model.samples[s2].area:
+				continue
+			if model.samples[s1].area_excavation_phase < model.samples[s2].area_excavation_phase:
 				earlier_than[i][j] = True
-			elif phases[s2] < phases[s1]:
-				earlier_than[j][i] = True
 	
 	# Check if earlier_than has circular relationships
 	if not check_circular_relationships(earlier_than, samples):
 		# Visualize earlier_than as a DAG
 		visualize_earlier_than(earlier_than, samples)
 		raise Exception("Circular relationships detected")
 	
 	# Extend the earlier_than matrix to include computed relations
 	earlier_than = extend_earlier_than(earlier_than)
-	
-	return earlier_than
+	# earlier_than: matrix[n_samples x n_samples] = [True/False, ...]; sample in row is earlier than sample in column based on stratigraphy
+	return earlier_than, samples
 
 def get_phases_gr(earlier_than):
 	n_samples = earlier_than.shape[0]
 	phasing = np.full(n_samples, np.nan)  # phasing[si] = phase; lower = earlier
 	
 	# assign phase to samples latest to earliest
 	mask_todo = earlier_than.copy()
@@ -156,24 +106,77 @@
 	mask = (~np.isnan(phasing))
 	if mask.any():
 		phasing[mask] = phasing[mask].max() - phasing[mask]
 	phasing[~mask] = -1
 	return phasing
 
 def get_groups_and_phases(earlier_than, samples):
+	# returns groups_phases = {sample: [group, phase], ...}
 	
 	groups = find_groups(earlier_than)
 	# groups = {group: [idx, ...], ...}; idx = index in earlier_than
 	
+	groups_phases = dict([(name, [None, None]) for name in samples])
+	for gi in groups:
+		for i in groups[gi]:
+			groups_phases[samples[i]][0] = gi
+	
 	# Calculate phasing for each group
-	phases = {}
 	for gi in groups:
 		earlier_than_gr = earlier_than[np.ix_(groups[gi], groups[gi])]
 		samples_gr = [samples[i] for i in groups[gi]]
 		phases_gr = get_phases_gr(earlier_than_gr)
-		phases[gi] = dict([(samples_gr[i], int(phases_gr[i]) + 1) for i in range(len(groups[gi]))])
-	groups = dict([(gi, [samples[i] for i in groups[gi]]) for gi in groups])
+		for i in range(len(groups[gi])):
+			groups_phases[samples_gr[i]][1] = int(phases_gr[i]) + 1
+	
+	return groups_phases
+
+def update_earlier_than_by_clustering(model, earlier_than, samples):
+	# Update earlier_than based on temporal clustering of the samples
+	
+	if model.cluster_opt_n is None:
+		raise Exception("No clustering found")
+	
+	clusters = model.clusters[model.cluster_opt_n]
+	means = model.cluster_means[model.cluster_opt_n]
+	
+	if len(clusters) < 2:
+		return earlier_than
+	
+	# Sort clusters from oldest to youngest
+	labels = sorted(clusters.keys(), key=lambda label: means[label], reverse=True)
+	
+	phases_clu = dict((label, idx + 1) for idx, label in enumerate(labels))
+	# phases_clu = {label: phase, ...}; lower phase = earlier
+	
+	collect = {}
+	for label in phases_clu:
+		for sample in clusters[label]:
+			collect[sample] = phases_clu[label]
+	phases_clu = collect
+	# phases_clu = {sample: phase, ...}
 	
-	# groups = {group: [sample, ...], ...}
-	# phases = {group: {sample: phase, ...}, ...}
-	return groups, phases
+	# Update earlier-than relationships based on phases derived from clustering
+	errors = []
+	for i, s1 in enumerate(samples):
+		for j, s2 in enumerate(samples):
+			if phases_clu[s1] < phases_clu[s2]:
+				earlier_than[i][j] = True
+				if (model.samples[s1].group == model.samples[s2].group) and (model.samples[s1].phase > model.samples[s2].phase):
+					errors.append([s1, s2, phases_clu[s1], phases_clu[s2], model.samples[s1].phase, model.samples[s2].phase])
+	if errors:
+		print("Warning, collisions detected between stratigraphic phasing and clustering:")
+		for s1, s2, clu1, clu2, ph1, ph2 in errors:
+			print("%s (Strat. phase %s, Clu. phase %s), %s (Strat. phase %s, Clu. phase %s)" % (s1, ph1, clu1, s2, ph2, clu2))
+		print()
+	
+	# Check if earlier_than has circular relationships
+	if not check_circular_relationships(earlier_than, samples):
+		# Visualize earlier_than as a DAG
+		visualize_earlier_than(earlier_than, samples)
+		raise Exception("Circular relationships detected")
+	
+	# Extend the earlier_than matrix to include computed relations
+	earlier_than = extend_earlier_than(earlier_than)
+	
+	return earlier_than
```

### Comparing `sitesyncro-0.9/src/sitesyncro/lib/fnc_simulate.py` & `sitesyncro-0.9.1/src/sitesyncro/utils/fnc_simulate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,67 @@
-from sitesyncro.lib.fnc_radiocarbon import (calibrate)
-from sitesyncro.lib.fnc_sum import (sum_distributions, calc_range, calc_mean_std, calc_percentiles)
-from sitesyncro.lib.fnc_mp import (process_mp)
+from sitesyncro.utils.fnc_radiocarbon import (calibrate)
+from sitesyncro.utils.fnc_stat import (calc_sum, calc_mean_std, calc_percentiles, samples_to_distributions)
+from sitesyncro.utils.fnc_mp import (process_mp)
 
 import numpy as np
+from tqdm import tqdm
 from scipy.stats import norm
 
-def generate_random_distributions(dates_n, t_param1, t_param2, uncert_base, curve, uniform):
+def generate_random_distributions(dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform):
 	# Generate sets of randomized distributions based on observed distributions
 	#
 	# dates_n: number of dates to generate
 	# t_param1: mean or median of the calendar ages
 	# t_param2: standard deviation or range of the calendar ages
-	# uncert_base: base uncertainty to simulate radiocarbon dates
+	# uncertainties: [uncertainty, ...] pool of uncertainties to simulate C-14 dates
+	# uncertainty_base: base uncertainty to calculate uncertainty based on C-14 age if pool is not available
 	# curve: [[CalBP, ConvBP, CalSigma], ...]
 	# uniform: flag indicating whether to use a uniform distribution for the calendar ages
 	
-	dates = []
-	distributions = []
-	for i in range(dates_n):
+	def _sim_age():
 		# Generate a random calendar age
 		if uniform:
 			t = np.random.uniform(t_param1 - t_param2, t_param1 + t_param2)
 		else:
 			t = np.random.normal(t_param1, t_param2)
 		# Find the closest index in the calibration curve
 		idx = np.argmin(np.abs(curve[:, 0] - t))
 		# Get the corresponding radiocarbon age
 		age = curve[idx, 1]
+		return age
+	
+	dates = []
+	distributions = []
+	for i in range(dates_n):
+		# Generate a random calendar age
+		age = _sim_age()
 		# Calculate the standard deviation for the date
-		stdev = uncert_base * np.exp(age / (2 * 8033))
+		if uncertainties:
+			stdev = np.random.choice(uncertainties)
+		else:
+			stdev = uncertainty_base * np.exp(age / (2 * 8033))
 		# Append the date and its standard deviation to the dates list
 		dates.append([age, stdev])
 		# Calibrate the date and append the distribution to the distributions list
-		distribution = calibrate(age, stdev, curve, normalize=True)
+		distribution = calibrate(age, stdev, curve)
 		distributions.append(distribution)
 	
 	# Sum the distributions of the generated dates
-	dist_summed = sum_distributions(distributions)
+	dist_summed = calc_sum(distributions)
 	
 	if uniform:
 		# Calculate weighted median and range
 		median_sum = np.average(curve[:, 0], weights=dist_summed)
 		range_sum = np.sqrt(np.average((curve[:, 0] - median_sum) ** 2, weights=dist_summed))
 	else:
 		# Calculate the mean and standard deviation of the summed distribution
-		mean_sum, std_sum = calc_mean_std([curve[:, 0], dist_summed])
+		mean_sum, std_sum = calc_mean_std(curve[:, 0], dist_summed)
+	
+	curve_min = curve[:,1].min()
+	curve_max = curve[:,1].max()
 	
 	# Adjust the dates until the mean and standard deviation of the summed distribution are close to the desired values
 	iteration = 0
 	scaling_factor = 1.0
 	if uniform:
 		c_threshold = t_param2 * 0.01
 	else:
@@ -62,134 +75,111 @@
 		if c <= c_threshold:
 			break
 		
 		iteration += 1
 		
 		# Randomly select a date to adjust
 		i = np.random.choice(dates_n)
+		age_new = dates[i][0]
 		if uniform:
-			dates[i][0] += 1 * (t_param1 - median_sum)
-			dates[i][0] *= 1 + scaling_factor * ((t_param2 / range_sum) - 1)
+			age_new += 1 * (t_param1 - median_sum)
+			age_new *= 1 + scaling_factor * ((t_param2 / range_sum) - 1)
 		else:
-			dates[i][0] += (t_param1 - mean_sum)
-			dates[i][0] *= 1 + scaling_factor * ((t_param2 / std_sum) - 1)
-		distributions[i] = calibrate(dates[i][0], dates[i][1], curve, normalize=True)
+			age_new += (t_param1 - mean_sum)
+			age_new *= 1 + scaling_factor * ((t_param2 / std_sum) - 1)
+		if (age_new < curve_min) or (age_new > curve_max):
+			age_new = _sim_age()
+		dates[i][0] = age_new
+		distributions[i] = calibrate(dates[i][0], dates[i][1], curve)
 		
 		# Recalculate the sum of the distributions and their mean or median
-		dist_summed = sum_distributions(distributions)
+		dist_summed = calc_sum(distributions)
 		if uniform:
 			median_sum = np.average(curve[:, 0], weights=dist_summed)
 			range_sum = np.sqrt(np.average((curve[:, 0] - median_sum) ** 2, weights=dist_summed))
 		else:
-			mean_sum, std_sum = calc_mean_std([curve[:, 0], dist_summed])
+			mean_sum, std_sum = calc_mean_std(curve[:, 0], dist_summed)
 		# Decrease the scaling factor
 		scaling_factor *= 0.999
 	
 	return distributions
 
-def worker_fnc(params, dates_n, t_param1, t_param2, uncert_base, curve, uniform):
-	
-	return generate_random_distributions(dates_n, t_param1, t_param2, uncert_base, curve, uniform)
-
-def collect_fnc(data, results):
-	
-	# data = distributions
-	# distributions = [[p, ...], ...]
-	
-	results.append(data)
-
-def progress_fnc(done, todo, all_done, all_todo, c):
-	
-	print("\rIteration: %d/%d, Conv: %0.4f         " % (all_done + done, all_todo, c), end = '')
-
 def calculate_parameters(years, distribution, uniform):
 	if uniform:
 		# Calculate weighted median and range of the summed distribution
 		t_median = np.average(years, weights=distribution)
 		t_range = np.sqrt(np.average((years - t_median) ** 2, weights=distribution))
 		t_param1, t_param2 = t_median, t_range
 	else:
 		# Calculate the mean and standard deviation of the summed distribution
-		t_mean, t_std = calc_mean_std([years, distribution])
+		t_mean, t_std = calc_mean_std(years, distribution)
 		t_param1, t_param2 = t_mean, t_std
 
 	return t_param1, t_param2
 
-def test_distributions(distributions, curve, p_value = 0.05, uncert_base = 15, uniform = False,
-                   npass = 100, convergence = 0.99, max_cpus = -1, max_queue_size = 100):
-	# Randomization test of the null hypothesis that the observed distributions
-	# represent a normal / uniform distribution of events
-	#
-	# distributions = {name: [p, ...], ...}
-	# curve: [[CalBP, ConvBP, CalSigma], ...]
-	# uncert_base: base uncertainty to simulate radiocarbon dates
-	# uniform: flag indicating whether to use a uniform distribution for the calendar ages
-	#
-	# returns: [[age, stdev], ...], [distributions, ...]
+
+def worker_fnc(params, dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform):
 	
-	# Number of dates to generate
-	dates_n = len(distributions)
+	return generate_random_distributions(dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve, uniform)
 
-	# Sum the distributions of all samples
-	sum_obs = sum_distributions(list(distributions.values()))
+def collect_fnc(data, results, pbar):
 	
-	years = curve[:, 0]
+	# data = distributions
+	# distributions = [[p, ...], ...]
 	
-	# Calculate the mean or median and standard deviation or range of the summed distribution
-	t_param1, t_param2 = calculate_parameters(years, sum_obs, uniform)
+	pbar.update(1)
+	results.append(data)
+
+def progress_fnc(done, todo, all_done, all_todo, c, pbar):
+	
+	print("\rIteration: %d/%d, Conv: %0.4f         " % (all_done + done, all_todo, c), end = '')
+
+def test_distributions(model, max_cpus = -1, max_queue_size = 100):
+	
+	distributions, _, _ = samples_to_distributions(model.samples.values())
+	
+	dates_n = len(distributions)
+	
+	if dates_n < 3:
+		raise Exception("Insufficient number samples for testing.")
+	
+	print("Testing %d distributions" % dates_n)
+	
+	sum_obs = calc_sum(distributions)
+	years = model.curve[:, 0]
+	t_param1, t_param2 = calculate_parameters(years, sum_obs, model.uniform)
 	
-	# Generate sets of randomized distributions and their sums
 	distributions_rnd = []
 	sums = []
 	sums_prev = None
 	c = 0
-	params_list = list(range(npass))
-	todo = npass
-	while True:
-		process_mp(worker_fnc, params_list, [dates_n, t_param1, t_param2, uncert_base, curve, uniform],
-		           collect_fnc = collect_fnc, collect_args = [distributions_rnd],
-		           progress_fnc = progress_fnc, progress_args = [len(distributions_rnd), npass*2, c],
+	todo = model.npass
+	params_list = list(range(model.npass))
+	with tqdm(total=todo) as pbar:
+		pbar.total = model.npass*2
+		pbar.set_description("Convergence: %0.3f" % (c))
+		while True:
+			process_mp(worker_fnc, params_list, [dates_n, t_param1, t_param2, model.uncertainties, model.uncertainty_base, model.curve, model.uniform],
+		           collect_fnc = collect_fnc, collect_args = [distributions_rnd, pbar],
 		           max_cpus = max_cpus, max_queue_size = max_queue_size)
-		if len(distributions_rnd) >= todo:
-			sums += [sum_distributions(dists) for dists in distributions_rnd[-(len(distributions_rnd) - len(sums)):]]
-			sums_m = np.array(sums).mean(axis = 0)
-			if sums_prev is not None:
-				c = ((sums_prev * sums_m).sum()**2) / ((sums_prev**2).sum() * (sums_m**2).sum())
-			sums_prev = sums_m.copy()
-			if c >= convergence:
-				print("\nConverged at:", c)
-				break
-			todo *= 2
+			if len(distributions_rnd) >= todo:
+				sums += [calc_sum(dists) for dists in distributions_rnd[-(len(distributions_rnd) - len(sums)):]]
+				sums_m = np.array(sums).mean(axis = 0)
+				if sums_prev is not None:
+					c = ((sums_prev * sums_m).sum()**2) / ((sums_prev**2).sum() * (sums_m**2).sum())
+					pbar.set_description("Convergence: %0.3f" % (c))
+				sums_prev = sums_m.copy()
+				if c >= model.convergence:
+					break
+				todo *= 2
+				pbar.total = max(todo, model.npass*2)
 	
 	sums_rnd = np.array(sums)
 	
-	# Calculate p-value
 	mask = (sums_rnd.std(axis = 0) > 0)
 	p = (1 - norm(sums_rnd[:,mask].mean(axis = 0), sums_rnd[:,mask].std(axis = 0)).cdf(sum_obs[mask])).min()
 	
-	# Find the range of years with non-zero probabilities
-	threshold = 0.001 * min(sum_obs.max(), sums_rnd.max())
-	j1 = np.argwhere(sum_obs > threshold).min()
-	j2 = np.argwhere(sum_obs > threshold).max()
-	for i in range(sums_rnd.shape[1]):
-		if sums_rnd[:,i].max() > threshold:
-			j1 = min(j1, i)
-			j2 = max(j2, i)
-	for distrs in distributions_rnd:
-		for i in range(len(distrs)):
-			if distrs[i].max() > threshold:
-				j1 = min(j1, i)
-				j2 = max(j2, i)
-	
-	# Trim the years, observed distribution, and randomized distributions
-	years = years[j1:j2+1]
-	sum_obs = sum_obs[j1:j2+1]
-	sums_rnd = sums_rnd[:,j1:j2+1]
-	for i in range(len(distributions_rnd)):
-		distributions_rnd[i] = [distr[j1:j2+1] for distr in distributions_rnd[i]]
-	
-	perc_lower = (p_value * 100) / 2
+	perc_lower = (model.p_value * 100) / 2
 	perc_upper = 100 - perc_lower
 	sums_rnd_lower, sums_rnd_upper = calc_percentiles(sums_rnd, perc_lower, perc_upper)
 	
-	return years, sum_obs, distributions_rnd, sums_rnd_lower, sums_rnd_upper, p
-
+	return sum_obs, sums_rnd_lower, sums_rnd_upper, p
```

### Comparing `sitesyncro-0.9/src/sitesyncro/lib/fnc_sum.py` & `sitesyncro-0.9.1/src/sitesyncro/utils/fnc_stat.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,34 @@
 import numpy as np
-from scipy.interpolate import interp1d
+from collections import defaultdict
 
-def unify_distributions(distributions, curve):
-	# distributions = {name: [p, ...], ...}
-	# Years are converted from CE to BP
-	
-	# Modify distributions so all lists have the same length
-	all_years = curve[:,0]
-	result = {}
-	for name in distributions:
-		dist, years = distributions[name]['prob'], distributions[name]['years'] # years are CE
-		years = 1950 - np.array(years)
-		
-		# Check if the years are in the correct order
-		if np.sign(years[-1] - years[0]) != np.sign(all_years[-1] - all_years[0]):
-			years = years[::-1]
-			dist = dist[::-1]
-		
-		years = np.concatenate(([all_years[0]], years, [all_years[-1]]))
-		dist = np.concatenate(([0], dist, [0]))
-		s = dist.sum()
-		if s > 0:
-			dist /= s
-		new_prob = interp1d(years, dist, kind="linear")(all_years)
-		s = new_prob.sum()
-		if s > 0:
-			new_prob /= s
-		result[name] = new_prob
-	
-	return result
-
-def sum_distributions(distributions):
+def calc_sum(distributions):
 	# distributions = [[p, ...], ...]
-	
-	# Create a list of all probabilities
-	summed = np.zeros(len(distributions[0]), dtype = float)
-	
-	# Sum probabilities
+	summed = np.zeros(len(distributions[0]), dtype = np.float64)
 	for dist in distributions:
-		summed += np.array(dist, dtype = float)
-	
-	# Normalize probabilities
+		summed += np.array(dist, dtype = np.float64)
 	s = summed.sum()
 	if s != 0:
 		summed /= s
-	
 	return summed
 
-def calc_mean_std(distribution):
-	# distribution = [years, prob]
-	
-	years, prob = distribution
-	
-	mean = np.average(years, weights=prob)
-	std = np.sqrt(np.average((years - mean) ** 2, weights=prob))
-	
+def calc_mean(years, distribution):
+	if not distribution.sum():
+		return None
+	return float(np.average(years, weights=distribution))
+
+def calc_mean_std(years, distribution):
+	mean = calc_mean(years, distribution)
+	if mean is None:
+		return None, None
+	std = np.sqrt(np.average((years - mean) ** 2, weights=distribution))
 	return mean, std
 
-def calc_range(distribution, p = 0.9545, p_threshold = 0.0001, max_multiplier = 32):
-	# distribution = [years, prob]
+def calc_range(years, distribution, p = 0.9545, p_threshold = 0.0001, max_multiplier = 32):
+	# returns [from, to] in calendar years BP
 	
 	def _find_rng(values, weights, v_min, v_max, mul):
 		
 		vs = np.linspace(values.min(), values.max(), values.shape[0] * mul)
 		weights = np.interp(vs, values, weights)
 		values = vs
 		weights /= weights.sum()
@@ -81,36 +47,68 @@
 				p_sum = weights[mask].sum()
 				idxs = np.where(mask)[0]
 				return values[idxs.min()], values[idxs.max()], p - p_sum
 			lvl_prev = lvl
 		idxs = np.where(weights > 0)[0]
 		return values[idxs.min()], values[idxs.max()], 1 - p	
 	
-	years, prob = distribution
 	years = np.array(years)
-	prob = np.array(prob)
+	distribution = np.array(distribution)
+	if not distribution.sum():
+		return [None, None]
 	v_min, v_max = years.min(), years.max()
 	p_diff_opt = np.inf
 	v_opt = [v_min, v_max]
 	mul = 2
 	while True:
-		v_min, v_max, p_diff = _find_rng(years, prob, v_min, v_max, mul)
+		v_min, v_max, p_diff = _find_rng(years, distribution, v_min, v_max, mul)
 		if p_diff >= p_diff_opt:
 			mul *= 2
 		if p_diff < p_diff_opt:
 			p_diff_opt = p_diff
 			v_opt = [v_min, v_max]
 		if p_diff <= p_threshold:
 			break
 		if mul > max_multiplier:
 			break
 	
-	return v_opt
+	return [float(v_opt[1]), float(v_opt[0])]
 
 def calc_percentiles(distributions, perc_lower, perc_upper):
 	# distributions = [[p, ...], ...]
-	
-	combined = np.array(distributions)
-	
+	combined = np.array(distributions, dtype=np.float64)
 	percentiles = np.percentile(combined, [perc_lower, perc_upper], axis=0)
-	
 	return percentiles
+
+def samples_to_distributions(samples):
+	# Get a list of probability distributions from samples
+	# Combine samples from the same context by summation
+	# Use only posterior (modeled) distributions for long-lived samples
+	# samples = [Sample, ...]
+	#
+	# returns distributions, samples_collected, joined
+	#	distributions = [[p, ...], ...]
+	#	samples_collected = [sample name, ...] ordered by distributions
+	#	joined = {combined_name: [sample name, ...], ...}
+	distributions_dict = {}  # {name: np.array([p, ...]), ...}
+	contexts = defaultdict(list)
+	for sample in samples:
+		if sample.is_modeled:
+			distributions_dict[sample.name] = sample.posterior
+			contexts[sample.context].append(sample.name)
+		elif sample.is_calibrated and not sample.long_lived:
+			distributions_dict[sample.name] = sample.likelihood
+			contexts[sample.context].append(sample.name)
+	joined = {}  # {combined_sample: [sample_name, ...], ...}
+	samples_collected = []
+	distributions = []
+	for context, sample_names in contexts.items():
+		if len(sample_names) > 1:
+			combined_sample = '+'.join(sample_names)
+			joined[combined_sample] = sample_names
+			distributions.append(calc_sum([distributions_dict[name] for name in sample_names]))
+			samples_collected.append(combined_sample)
+		else:
+			distributions.append(distributions_dict[sample_names[0]])
+			samples_collected.append(sample_names[0])
+	
+	return distributions, samples_collected, joined
```

### Comparing `sitesyncro-0.9/src/sitesyncro.egg-info/PKG-INFO` & `sitesyncro-0.9.1/src/sitesyncro.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesyncro
-Version: 0.9
+Version: 0.9.1
 Summary: SiteSyncro - Site-specific chronological modeling and synchronization
 Home-page: https://github.com/demjanp/SiteSyncro
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: archaeology,radiocarbon,chronology,stratigraphy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -29,15 +29,20 @@
 
 <details>
 <summary>Table of Contents</summary>
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
+   * [Input File Format](#input_file)
+   * [Model Class](#model_class)
+   * [Sample Class](#sample_class)
 4. [Developer Notes](#developer)
+	* [Preparing the Virtual Environment](#venv)
+	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
 </details>
 
 ## About SiteSyncro <a name="about"></a>
@@ -52,279 +57,318 @@
 For a detailed overview of the clustering method see:
 
 Demján, P., & Pavúk, P. (2021). CLUSTERING OF CALIBRATED RADIOCARBON DATES: SITE-SPECIFIC CHRONOLOGICAL SEQUENCES IDENTIFIED BY DENSE RADIOCARBON SAMPLING. Radiocarbon, 63(2), 429-438. [doi:10.1017/RDC.2020.129](https://doi.org/10.1017/RDC.2020.129)
 
 
 ## Installation <a name="installation"></a>
 
-SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The OxCal program is used for bayesian modeling of the radiocarbon dates. The OxCal program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
+[Windows executable](https://github.com/demjanp/SiteSyncro/releases/latest) is available for users who do not want to install Python and dependencies.
 
-For Windows users, an executable version of SiteSyncro is available. You can download the `sitesyncro.exe` file from the [latest release on GitHub](https://github.com/demjanp/SiteSyncro/releases/latest). After downloading, you can run SiteSyncro directly without needing to install Python or any dependencies.
+To run SiteSyncro on other platforms, please refer to the [Developer Notes](#developer) section on how to clone SiteSyncro from GitHub and create a virtual environment. See [Usage](#usage) section on how to run the script or import SiteSyncro as a python library.
 
-To run SiteSyncro on other platforms, please refer to the [Developer Notes](#developer) section on how to clone SiteSyncro from GitHub and create a virtual environment. See [Usage](#usage) section on how to run the script.
+To use SiteSyncro in your Python applications, install the latest version from the Python package index, use the following command:
+```
+pip install SiteSyncro
+```
+See [Model Class](#model_class) on usage tips.
+
+SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
 
 ## Usage <a name="usage"></a>
+
+### Running the Script
 To use SiteSyncro, you need to run the [process.py](bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
-```bash
-python process.py data_sample.csv
+```
+python process.py -input data_sample.csv
 ```
 or
-```bash
-sitesyncro.exe data_sample.csv
-```bash
+```
+sitesyncro.exe -input data_sample.csv
+```
 `process.py` & `sitesyncro.exe` accepts the following command-line arguments:
-
-- `input`: The path to the input file in semicolon-separated CSV format (required).
-- `-result`: The directory path to store the results (default is "result").
-- `-existing`: Flag indicating whether to use existing results (default is 0).
-- `-curve`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
-- `-model`: OxCal model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
-- `-n`: Number of clusters to form (-1 = automatic; default is -1).
+- `-h`, `--help`: Show help message and exit.
+- `-directory`: Working directory for model data (default is "model").
+- `-input`: The path to the input file in semicolon-separated CSV format.
+- `-curve_name`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
+- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
+- `-cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
+- `-by_clusters`: Flag indicating whether to update the phasing by clustering sample dates (default is 0).
 - `-uniform`: Flag indicating whether to use a uniform distribution for the calendar ages (default is 0).
 - `-p_value`: P-value for the randomization tests (default is 0.05).
-- `-uncert_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
+- `-uncertainty_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
 - `-npass`: Minimum number of passes for the randomization tests (default is 100).
 - `-convergence`: Convergence threshold for the randomization tests (default is 0.99).
 - `-max_cpus`: Maximum number of CPUs to use for parallel processing (-1 = all available; default is -1).
-- `-max_queue_size`: Maximum queue size for parallel processing (default is 100).
+- `-max_queue_size`: Maximum queue size for parallel processing (default is 100)
 
 For example, if you want to run the script with a specific calibration curve, using uniform distributions for randomization testing and a P-value threshold of 0.01, you can do so like this:
 
 ```bash
-python process.py data_sample.csv -curve intcal20.14c -uniform 1 -p_value 0.01
+python process.py -input data_sample.csv -curve intcal20.14c -uniform 1 -p_value 0.01
 ```
 
 This will run the script with input data from data_sample.csv and use the IntCal20 calibration curve, a uniform distribution for the calendar ages, and a P-value of 0.01 for the randomization tests.
 
+### Input File Format <a name="input_file"></a>
 The input file name must be a semicolon-separated CSV file with the following 8 columns: 
 1. Sample: Sample ID (required, unique identifier)
 2. Context: Context ID (required)
 3. Excavation Area: Excavation area ID (required)
 4. C-14 Age: Radiocarbon age in years BP (required)
 5. Uncertainty: Uncertainty of the radiocarbon age in C-14 years (required)
 6. Phase: Phase of the sample (lower = older) (optional)
 7. Earlier-Than: List of contexts that the sample is earlier (older) than (optional)
 8. Long-Lived / Redeposited: Flag indicating whether the sample is long-lived (e.g. old wood) or redeposited (e.g. from an older context) (required, 1 or 0)
 
 See [data_sample.csv](data_sample.csv) for an example of the input file format.
 
+### Model Class <a name="model_class"></a>
+All functions regarding modeling are encapsulated in the `Model` class. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Model
+
+if __name__ == '__main__':
+	
+    # Initialize the Model object
+    model = Model()
+    
+    # Load the data
+    model.import_csv('data_sample.csv')
+    
+    # Process the model
+    model.process()
+    
+    # Plot the randomization test result
+    model.plot_randomized()
+    
+    # Plot the clustering result
+    model.plot_clusters()
+    
+    # Save the results to a CSV file
+    model.save_csv()
+```
+This will create the default directory `model` and generate the following files:
+`model.json.gz`
+`model.oxcal`
+`model.js`, `model.log`, `model.txt`
+`randomized.pdf`
+`silhouette.pdf`
+`results.csv`
+
+#### Parameters <a name="model_parameters"></a>
+
+The `Model` class constructor accepts the following parameters:
+- `directory`: Working directory for model data (default is "model").
+- `samples`: List of samples as instances of the class [Sample](#sample_class)
+- `curve_name`: The name of the calibration curve to use (default is "intcal20.14c").
+- `phase_model`: OxCal phase model type. Can be 'sequence', 'contiguous', 'overlapping', or 'none' (default is "sequence").
+- `cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
+- `uniform`: Flag indicating whether to use uniform randomization (default is False).
+- `p_value`: The P-value for statistical tests (default is 0.05).
+- `uncertainty_base`: The base uncertainty for randomization (default is 15).
+- `npass`: Minimum number of passes for the randomization tests (default is 100).
+- `convergence`: Convergence threshold for the randomization tests (default is 0.99).
+- `oxcal_url`: Url to download the OxCal program (default is "https://c14.arch.ox.ac.uk/OxCalDistribution.zip").
+
+#### Methods
+
+The `Model` class provides the following methods:
+- `add_sample(sample)` or `add_sample(name, age, uncertainty, **kwargs)`: Add a sample to the model.
+	- For arguments see [Sample parameters](#sample_parameters).
+- `del_sample(name)`: Delete a sample from the model.
+- `reset_model()`: Reset the model to the initial state.
+- `save(zipped = False)`: Save the model to a file.
+	- `zipped`; if True, save the model as a zipped JSON file
+- `copy(directory)`: Copy the model to a new directory.
+	- `directory`: Directory for the new model
+- `import_csv(fname)`: Import sample data from a CSV file. See [Input File Format](#input_file) for details.
+- `plot_randomized(show = False)`: Plot the randomization test results. If `show` is True, the plot is shown, otherwise it is saved as `randomized.pdf`.
+- `plot_clusters(show = False)`: Plot the clustering results. If `show` is True, the plot is shown, otherwise it is saved as `silhouette.pdf`.
+- `save_csv(fcsv = None)`: Save the results to a CSV file.
+	- `fcsv`: File path for the CSV file. If None, `results.csv` is saved in the model directory.
+- `to_oxcal()`: Save the phasing model in OxCal format as `model.oxcal`.
+- `load_oxcal_data()`: Load results of OxCal modeling from `model.js`.
+- `update_params(**kwargs)`: Update model parameters.
+	- For keyword arguments see [Parameters](#model_parameters)
+- `process_phasing(by_clusters = False)`: Update groups and phases of samples based on stratigraphic relations.
+	- `by_clusters`: if True, update the phasing by clustering sample dates
+- `process_dates()`: Calculate posteriors of sample dates based on phasing using bayesian modeling in OxCal.
+- `process_randomization(max_cpus = -1, max_queue_size = 100)`: Test if sample dates represent a uniform / normal (depending on Model.uniform parameter) distribution in time.
+- `process_clustering(max_cpus = -1, max_queue_size = 100)`: Cluster dates and using randomization testing find optimal clustering solution
+- `process(by_clusters = False, max_cpus = -1, max_queue_size = 100)`: Process the complete model
+	- `by_clusters`: if True, update the phasing by clustering sample dates
+	- `max_cpus`: Maximum number of CPUs to use for parallel processing (-1 = all available)
+	- `max_queue_size`: Maximum queue size for parallel processing
+
+#### Attributes
+
+The `Model` class has the following attributes:
+- `directory`: Working directory for model data
+- `samples`: Dictionary of samples in format `{name: Sample, ...}`
+- `curve_name`: The name of the calibration curve
+- `phase_model`: OxCal phase model type
+- `cluster_n`: Number of clusters to form
+- `uniform`: Flag indicating whether to use uniform randomization
+- `p_value`: The P-value threshold for statistical tests
+- `uncertainty_base`: The base uncertainty for randomization
+- `npass`: Minimum number of passes for the randomization tests
+- `convergence`: Convergence threshold for the randomization tests
+- `oxcal_url`: Url to download the OxCal program
+- `years`: Calendar years BP corresponding to the probability distributions in format `np.array([year, ...])`
+- `curve`: Calibration curve in format `np.array([[calendar year BP, C-14 year, uncertainty], ...])`, sorted by calendar years
+- `uncertainties`: List of uncertainties from C-14 dates of samples
+- `oxcal_data`: Results of OxCal modeling from `model.js` in format `{key: data, ...}`
+- `summed`: Summed probability distribution of the dating of all samples in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `random_p`: Calculated p-value for the randomization test
+- `random_lower`: Lower bound of the randomization test in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `random_upper`: Upper bound of the randomization test in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `areas`: List of excavation areas that the samples belong to
+- `contexts`: List of contexts that the samples belong to
+- `groups`: Groups that the samples belong to based on stratigraphic interconnection with other samples in format `{group_name: [sample name, ...], ...}`
+- `clusters`: Clusters of samples based on the similarity of their probability distributions in format `{clusters_n: [cluster: [sample name, ...], ...}, ...}`
+- `cluster_means`: Mean date of the samples in each cluster in calendar years BP in format `{clusters_n: {cluster: year, ...}, ...}`
+- `cluster_sils`: Silhouette score of each clustering solution in format `{clusters_n: silhouette, ...}`
+- `cluster_ps`: P-value of the clustering solutions in format `{clusters_n: p, ...}`
+- `cluster_opt_n`: Optimal number of clusters
+- `has_data`: Boolean indicating if the model has sample data
+- `is_modeled`: Boolean indicating if bayesian modeling of sample dates (process_dates) has been performed
+- `is_randomized`: Boolean indicating if randomization testing of the distribution of samples (process_randomization) has been performed
+- `is_clustered`: Boolean indicating if the model has been clustered (process_clustering)
+
+### Sample Class <a name="sample_class"></a>
+The `Sample` class represents a single radiocarbon sample. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Sample
+
+if __name__ == '__main__':
+	
+	# Initialize the Sample object
+	sample = Sample('Sample1', 1000, 50, phase = 1, earlier_than = ['Sample2'], long_lived = 0)
+	
+	# Print the sample data
+	print(sample)
+```
+
+#### Parameters <a name="sample_parameters"></a>
+
+The 'Sample' class constructor accepts the following parameters:
+- `name`: Sample ID (required, unique identifier)
+- `age`: C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U' (required)
+- `uncertainty`: Uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U' (required)
+- `date_type`: 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution
+- `long_lived`: True if sample is older than the examined deposition event due to e.g. old wood effect or redeposition from older strata
+- `context`: Name of the context where sample was found
+- `area`: Excavation area
+- `area_excavation_phase`: Chronological phase of the context within the excavation area (integer, lower = earlier (older) phase)
+- `earlier_than`: List of names of samples which are stratigraphically later (younger) than this sample
+- `curve`: Radiocarbon calibration curve in format `np.array([[calendar year BP, C-14 year, uncertainty], ...])`
+
+#### Methods
+
+The `Sample` class provides the following methods:
+- `calibrate(curve)`: Calibrate the sample using the provided calibration curve.
+	- `curve = np.array([[calendar year BP, C-14 year, uncertainty], ...])`
+- `set_group(group)`: Set the group number for the sample.
+- `set_phase(phase)`: Set the phase number for the sample.
+- `set_likelihood(distribution, mean = None, rng = None)`: Set the likelihood for the sample.
+	- `distribution = np.array([p, ...])`
+	- `rng = [from, to]`; 2-sigma (95.45%) range in calendar years BP
+- `set_posterior(distribution, mean = None, rng = None, agreement = 0)`: Set the posterior for the sample.
+	- `distribution = np.array([p, ...])`
+	- `rng = [from, to]`; 2-sigma (95.45%) range in calendar years BP
+	- `agreement`: agreement index generated by OxCal modeling
+- `to_oxcal()`: Convert the sample to OxCal model format (str).
+- `to_dict()`: Convert the sample data to a JSON dictionary.
+- `from_dict(data)`: Load the sample data from a JSON dictionary.
+- `copy()`: Create a copy of the sample instance.
+
+#### Attributes
+The `Sample` class has the following attributes:
+
+- `name`: Sample ID (unique identifier)
+- `age`: C-14 age (years BP) for date_type 'R'; mean calendar age (years BP) for date_type 'U'
+- `uncertainty`: Uncertainty (years BP) for date_type 'R'; 1/2 range (years BP) for date_type 'U'
+- `date_type`: 'R' for radiocarbon date; 'U' for calendar date as a uniform distribution
+- `long_lived`: True if sample is older than the examined deposition event due to e.g. old wood effect or redeposition from older strata
+- `context`: Name of the context where sample was found
+- `area`: Excavation area
+- `area_excavation_phase`: Chronological phase of the context within the excavation area (integer, lower = earlier (older) phase)
+- `earlier_than`: List of names of samples which are stratigraphically later (younger) than this sample
+- `group`: Group that the sample belongs to based on stratigraphic interconnection with other samples
+- `phase`: Stratigraphic phase of the sample within the group (lower = earlier (older) phase)
+- `years`: Calendar years BP corresponding to the probability distributions in format `np.array([year, ...])`
+- `likelihood`: Probability distribution of the dating of the sample before Bayesian modeling in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `posterior`: Probability distribution of the dating of the sample after Bayesian modeling in format `np.array([p, ...])`, where p is the probability of the calendar year
+- `likelihood_range`: 2-sigma (95.45%) range of the dating of the sample in calendar years BP before Bayesian modeling in format `[from, to]`
+- `likelihood_mean`: Mean calendar age of the sample in calendar years BP before Bayesian modeling
+- `posterior_range`: 2-sigma (95.45%) range of the dating of the sample in calendar years BP after Bayesian modeling in format `[from, to]`
+- `posterior_mean`: Mean calendar age of the sample in calendar years BP after Bayesian modeling
+- `posterior_agreement`: Agreement index generated by OxCal modeling
+- `is_calibrated`: Boolean indicating if the sample has been calibrated
+- `is_modeled`: Boolean indicating if posterior has been calculated using Bayesian modeling
+
 ## Developer Notes <a name="developer"></a>
 ### Preparing the Virtual Environment <a name="venv"></a>
 SiteSyncro requires [Python 3.10](https://www.python.org/downloads/).
 
 To prepare a Python virtual environment open a terminal or command prompt window and type the following commands:
 
 ```
 git clone https://github.com/demjanp/SiteSyncro.git
-
 cd sitesyncro
-
 python -m venv .venv
-
 .venv\Scripts\activate.bat
-
 python.exe -m pip install --upgrade pip
-
 pip install -e .
 ```
 
 See [Usage](#usage) on further instructions how to run the script.
 
-### Building a Windows Executable
+### Building a Windows Executable <a name="build"></a>
 To build a Windows executable, open a terminal or command prompt window and change to the `sitesyncro` folder: 
 ```
 cd SiteSyncro\sitesyncro
 ```
 Activate the virtual environment:
 ```
 .venv\Scripts\activate.bat
 ```
 Then type the following commands (this only has to be done once per virtual environment):
 ```
-python.exe -m pip install --upgrade pip
+python -m pip install --upgrade pip
 python -m pip install --upgrade build
 pip install twine
 pip install pyinstaller==6.6.0
 ```
 To build the executable, type:
 ```
 pip install -e .
 python -m build
 pyinstaller sitesyncro.spec
 ```
-You will find the executable `sitesyncro.exe` in the `dist` folder.
-
-### SiteSyncro Class
-All functions of SiteSyncro are encapsulated in the `SiteSyncro` class. Here is a basic example of how to use it:
-
-```python
-from sitesyncro import SiteSyncro
-
-# Initialize the SiteSyncro object
-ssync = SiteSyncro(input='data_sample.csv')
-
-# Load the data
-ssync.load_data()
-
-# Process the model
-ssync.process()
-
-# Plot the randomization test result
-ssync.plot_randomized()
-
-# Plot the clustering result
-ssync.plot_clusters()
-
-# Save the results to a CSV file
-ssync.save_results_csv()
-```
-
-#### Parameters <a name="parameters"></a>
-
-The `SiteSyncro` class accepts the following parameters:
-- `input`: The path to the input file.
-- `result`: The name of the result directory (default is "result").
-- `existing`: Boolean indicating whether to use existing results (default is False).
-- `curve`: The name of the calibration curve to use (default is "intcal20.14c").
-- `model`: The name of the model to use. Can be 'sequence', 'contiguous', 'overlapping', or 'none' (default is "sequence").
-- `n`: The number of clusters (-1 = automatic) (default is -1).
-- `uniform`: Boolean indicating whether to use uniform randomization (default is False).
-- `p_value`: The P-value for statistical tests (default is 0.05).
-- `uncert_base`: The base uncertainty for randomization (default is 15).
-- `npass`: The number of passes for the clustering algorithm (default is 100).
-- `convergence`: The convergence criterion for the clustering algorithm (default is 0.99).
-- `max_cpus`: The maximum number of CPUs to use (default is -1).
-- `max_queue_size`: The maximum size of the queue for parallel processing (default is 100).
-
-#### Methods
-
-The `SiteSyncro` class provides the following methods:
-- `load_data(**kwargs)`: Loads data from the input file and updates the internal data. The input file must be a CSV file with the following columns: Context, Excavation Area, C-14 Age, Uncertainty, Phase (lower = older), Earlier-Than, Long-Lived / Redeposited. For possible keyword arguments see [Parameters](#parameters).
-- `process(**kwargs)`: Processes the data. For possible keyword arguments see [Parameters](#parameters).
-- `plot_randomized(show=False)`: Plots the randomized data. If `show` is True, the plot is shown. If False, the plot is saved to a file.
-- `plot_clusters(show=False)`: Plots the clustering data. If `show` is True, the plot is shown. If False, the plot is saved to a file.
-- `save_results_csv(fcsv=None)`: Saves the results to a CSV file. If `fcsv` is None, a default file path is used.
-
-#### Attributes
-
-The `SiteSyncro` class has the following attributes:
-- `oc_data` (OxCalData): Used to store and manage the data after bayesian modelling of the radiocarbon dates with the OxCal program.
-- `rnd_data` (RandomizeData): Used to store and manage the data related to the randomization testing of the null hypothesis that the observed C-14 dates represent a normal/uniform distribution.
-- `clu_data` (ClusterData): Used to store and manage the data related to the temporal clustering of the modelled C-14 dates.
-- `oc_clu_data` (OxCalData): Used to store and manage the modelled data updated according to the temporal clustering of the C-14 dates.
-
-All variables generated by the OxCal program can be accessed using `oc_data[key]`. Use `print(oc_data)` to see a list of available keys.
-
-`OxCalData` class methods:
-- `__init__(fname=None)`: If a filename of an OxCal .js file is provided, it reads and stores the data.
-- `has_data(self)`: Returns True if the data dictionary is not empty, False otherwise.
-- `set_priors(samples, context_samples, context_area, areas, groups, phases, earlier_than, long_lived, r_dates, dates, model, curve)`: Sets the priors for the bayesian modeling.
-    ```
-    samples = [sample, ...]
-    context_samples = {context: [sample, ...], ...}
-    context_area = {context: area, ...}
-    areas = [area, ...]
-    groups = {group: [sample, ...], ...}
-    phases = {group: {sample: phase, ...}, ...}
-    long_lived = {sample: True/False, ...}
-    r_dates = {sample: (age, uncertainty), ...}
-    dates = {sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}; R = radiocarbon, U = uniform
-    ```
-- `get_likelihoods()`: Returns the likelihood distributions for each sample.
-    Format: `{name: {'prob': [p, ...], 'years': [calendar year CE, ...], 'mean': mean, 'range': [min year CE, max year CE]}}`
-    Ranges are calculated at the 95.45% (2-sigma) level.
-- `get_posteriors()`: Returns the posterior distributions for each sample. 
-    Format: `{name: {'prob': [p, ...], 'years': [calendar year CE, ...], 'mean': mean, 'range': [min year CE, max year CE], 'agreement': agreement index}}`	
-    Ranges are calculated at the 95.45% (2-sigma) level.
-- `get_samples()`: Returns the sample names.
-    Format: `[name, ...]`
-- `get_context_samples()`: Returns the contexts and their contained samples.
-    Format: `{context: [sample, ...], ...}`
-- `get_context_area()`: Returns the contexts and their areas.
-    Format: `{context: area, ...}`
-- `get_areas()`: Returns the areas.
-    Format: `[area, ...]`
-- `get_groups()`: Returns the groups based on stratigraphic links.
-    Format: `{group: [sample, ...], ...}`
-- `get_phases()`: Returns the phases for each group and sample. Lower = earlier (older) phase.
-    Format: `{group: {sample: phase, ...}, ...}`
-- `get_earlier_than()`: Returns the earlier-than relations between samples.
-    Format: `matrix[n_samples x n_samples] = [True/False, ...]`. Sample in row is earlier than sample in column based on stratigraphy.
-- `get_long_lived()`: Returns the long-lived value for each sample.
-    Format: `{sample: True/False, ...}`
-- `get_r_dates()`: Returns the radiocarbon dates for each sample.
-    Format: `{sample: (age, uncertainty), ...}`
-- `get_dates()`: Returns the date for bayesian modeling for each sample. Long-lived or redeposited samples are represented by a uniform distribution where the lower boundary is the lower boundary of the 2-sigma range of the calibrated date and the upper boundary is 1950 CE. 
-    Format: `{sample: (age, uncertainty, 'R'), sample: (CE from, CE to, 'U'), ...}`; R = radiocarbon, U = uniform
-- `get_model()`: Returns the model type used for the bayesian modeling.
-    Values: 'sequence', 'contiguous', 'overlapping', 'none'
-- `get_curve()`: Returns the calibration curve used.
-    Format: curve name (see OxCal\bin folder for available curves)
-
-`ClusterData` class methods:
-- `__init__(clusters = {}, means = {}, sils = {}, ps = {}, p_value = None, opt_n = None)`
-    ```
-    means = {n: mean, ...}
-    sils = {sample: sil, ...}
-    ps = {n: p, ...}
-    p_value = p-value threshold for randomization testing
-    opt_n = optimal number of clusters
-	```	
-- `has_data()`: Returns True if the clusters dictionary is not empty, False otherwise.
-- `get_clusters()`: Returns the clusters for each number of clusters.
-    Format: `{n: {sample: cluster, ...}, ...}`
-- `get_means()`: Returns the mean silhouette score for each number of clusters.
-    Format: `{n: mean, ...}`
-- `get_sils()`: Returns the silhouette score for each sample.
-    Format: `{sample: sil, ...}`
-- `get_ps()`: Returns the p-value for each number of clusters.
-    Format: `{n: p, ...}`
-- `get_p_value()`: Returns the p-value threshold for randomization testing.
-- `get_opt_n()`: Returns the optimal number of clusters.
-
-`RandomizeData` class methods:
-- `__init__(years = None, sum_obs = None, uniform = None, p = None, p_value = None, sums_rnd_lower = None, sums_rnd_upper = None)`
-    ```
-    years = [year, ...]. The years are in calendar years BP.
-    sum_obs = [p, ...] in order of the years.
-    uniform = True/False
-    p = calculated p-value
-    p_value = p-value threshold
-    sums_rnd_lower = [p, ...] in order of the years.
-    sums_rnd_upper = [p, ...] in order of the years.
-	```
-- `has_data()`: Returns True if the years attribute is not None, False otherwise.
-- `get_years()`: Returns the years for the randomization test.
-    Format: `[year, ...]`. The years are in calendar years BP.
-- `get_sum_obs()`: Returns the sum of the observed distributions.
-    Format: `[p, ...]` in order of the years.
-- `get_uniform()`: Returns True if the uniform distribution was used.
-- `get_p()`: Returns the calculated p-value for the randomization test.
-- `get_p_value()`: Returns the p-value threshold for the randomization test.
-- `get_sums_rnd_lower()`: Returns the lower boundary of the randomized distributions.
-    Format: `[p, ...]` in order of the years.
-- `get_sums_rnd_upper()`: Returns the upper boundary of the randomized distributions.
-    Format: `[p, ...]` in order of the years.
+The executable `sitesyncro.exe` will be created in the `dist` folder.
 
 ## Contact: <a name="contact"></a>
 Peter Demján (peter.demjan@gmail.com)
 
 Institute of Archaeology of the Czech Academy of Sciences, Prague, v.v.i.
 
 ## Acknowledgements <a name="acknowledgements"></a>
 
 Development of this software was supported by project OP JAC "Ready for the future: understanding long-term resilience of the human culture (RES-HUM)", Reg. No. CZ.02.01.01/00/22_008/0004593 of the Ministry of Education, Youth, and Sports of the Czech Republic and EU.
 
 This software requires the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program for bayesian modeling of the radiocarbon dates.
 
 This software uses the following open source packages:
-* [NumPy](https://www.numpy.org/)
-* [SciPy](https://scipy.org/)
 * [Matplotlib](https://matplotlib.org/)
+* [NetworkX](https://networkx.org/)
+* [NumPy](https://www.numpy.org/)
+* [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
+* [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
-* [Requests](https://requests.readthedocs.io/)
-* [NetworkX](https://networkx.org/)
 
 ## License <a name="license"></a>
 
 This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
```

