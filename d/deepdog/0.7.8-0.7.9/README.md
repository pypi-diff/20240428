# Comparing `tmp/deepdog-0.7.8.tar.gz` & `tmp/deepdog-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.7.8.tar", max compression
+gzip compressed data, was "deepdog-0.7.9.tar", max compression
```

## Comparing `deepdog-0.7.8.tar` & `deepdog-0.7.9.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      605 2024-02-29 00:42:10.812082 deepdog-0.7.8/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2024-02-29 00:42:10.812082 deepdog-0.7.8/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2024-02-29 00:42:10.812082 deepdog-0.7.8/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0     7661 2024-02-29 00:42:10.812082 deepdog-0.7.8/deepdog/bayes_run_with_ss.py
--rw-r--r--   0        0        0      161 2024-02-29 00:42:10.812082 deepdog-0.7.8/deepdog/direct_monte_carlo/__init__.py
--rw-r--r--   0        0        0     4615 2024-02-29 00:42:10.816082 deepdog-0.7.8/deepdog/direct_monte_carlo/direct_mc.py
--rw-r--r--   0        0        0       73 2024-02-29 00:42:10.816082 deepdog-0.7.8/deepdog/meta.py
--rw-r--r--   0        0        0    10940 2024-02-29 00:42:10.816082 deepdog-0.7.8/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0      110 2024-02-29 00:42:10.824083 deepdog-0.7.8/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0    11428 2024-02-29 00:42:10.824083 deepdog-0.7.8/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2024-02-29 00:42:10.832083 deepdog-0.7.8/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      916 2024-02-29 00:42:10.840083 deepdog-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      692 2024-02-29 00:43:27.107091 deepdog-0.7.8/setup.py
--rw-r--r--   0        0        0      361 2024-02-29 00:43:27.107461 deepdog-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      605 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0     7661 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/bayes_run_with_ss.py
+-rw-r--r--   0        0        0      161 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/direct_monte_carlo/__init__.py
+-rw-r--r--   0        0        0      461 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/direct_monte_carlo/compose_filter.py
+-rw-r--r--   0        0        0     5103 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/direct_monte_carlo/direct_mc.py
+-rw-r--r--   0        0        0     3920 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/direct_monte_carlo/dmc_filters.py
+-rw-r--r--   0        0        0       73 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/meta.py
+-rw-r--r--   0        0        0    13688 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0      110 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-21 16:24:23.080795 deepdog-0.7.9/deepdog/subset_simulation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9024 2024-04-21 16:24:23.084795 deepdog-0.7.9/deepdog/subset_simulation/__pycache__/subset_simulation_impl.cpython-39.pyc
+-rw-r--r--   0        0        0    11428 2024-04-21 16:24:04.447878 deepdog-0.7.9/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2024-04-21 16:24:04.451878 deepdog-0.7.9/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      916 2024-04-21 16:24:04.451878 deepdog-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 deepdog-0.7.9/PKG-INFO
```

### Comparing `deepdog-0.7.8/deepdog/__init__.py` & `deepdog-0.7.9/deepdog/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.8/deepdog/bayes_run.py` & `deepdog-0.7.9/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.8/deepdog/bayes_run_simulpairs.py` & `deepdog-0.7.9/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.8/deepdog/bayes_run_with_ss.py` & `deepdog-0.7.9/deepdog/bayes_run_with_ss.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.8/deepdog/direct_monte_carlo/direct_mc.py` & `deepdog-0.7.9/deepdog/direct_monte_carlo/direct_mc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pdme.model
 import pdme.measurement
 import pdme.measurement.input_types
 import pdme.subspace_simulation
-from typing import Tuple, Sequence
+from typing import Tuple, Dict, NewType, Any
 from dataclasses import dataclass
 import logging
 import numpy
 import numpy.random
 import pdme.util.fast_v_calc
 
 _logger = logging.getLogger(__name__)
@@ -26,14 +26,28 @@
 	target_success: int = 100
 	max_monte_carlo_cycles_steps: int = 10
 	monte_carlo_seed: int = 1234
 	write_successes_to_file: bool = False
 	tag: str = ""
 
 
+# Aliasing dict as a generic data container
+DirectMonteCarloData = NewType("DirectMonteCarloData", Dict[str, Any])
+
+
+class DirectMonteCarloFilter:
+	"""
+	Abstract class for filtering out samples matching some criteria. Initialise with data as needed,
+	then filter out samples as needed.
+	"""
+
+	def filter_samples(self, samples: numpy.ndarray) -> numpy.ndarray:
+		raise NotImplementedError
+
+
 class DirectMonteCarloRun:
 	"""
 	A single model Direct Monte Carlo run, currently implemented only using single threading.
 	An encapsulation of the steps needed for a Bayes run.
 
 	Parameters
 	----------
@@ -61,54 +75,57 @@
 	monte_carlo_seed: int
 	The seed to use for the RNG.
 	"""
 
 	def __init__(
 		self,
 		model_name_pair: Tuple[str, pdme.model.DipoleModel],
-		measurements: Sequence[pdme.measurement.DotRangeMeasurement],
+		filter: DirectMonteCarloFilter,
 		config: DirectMonteCarloConfig,
 	):
 		self.model_name, self.model = model_name_pair
 
-		self.measurements = measurements
-		self.dot_inputs = [(measure.r, measure.f) for measure in self.measurements]
+		# self.measurements = measurements
+		# self.dot_inputs = [(measure.r, measure.f) for measure in self.measurements]
 
-		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
-			self.dot_inputs
-		)
+		# self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
+		# 	self.dot_inputs
+		# )
 
 		self.config = config
-		(
-			self.lows,
-			self.highs,
-		) = pdme.measurement.input_types.dot_range_measurements_low_high_arrays(
-			self.measurements
-		)
+		self.filter = filter
+		# (
+		# 	self.lows,
+		# 	self.highs,
+		# ) = pdme.measurement.input_types.dot_range_measurements_low_high_arrays(
+		# 	self.measurements
+		# )
 
 	def _single_run(self, seed) -> numpy.ndarray:
 		rng = numpy.random.default_rng(seed)
 
 		sample_dipoles = self.model.get_monte_carlo_dipole_inputs(
 			self.config.monte_carlo_count_per_cycle, -1, rng
 		)
 
 		current_sample = sample_dipoles
-		for di, low, high in zip(self.dot_inputs_array, self.lows, self.highs):
 
-			if len(current_sample) < 1:
-				break
-			vals = pdme.util.fast_v_calc.fast_vs_for_dipoleses(
-				numpy.array([di]), current_sample
-			)
-
-			current_sample = current_sample[
-				numpy.all((vals > low) & (vals < high), axis=1)
-			]
-		return current_sample
+		return self.filter.filter_samples(current_sample)
+		# for di, low, high in zip(self.dot_inputs_array, self.lows, self.highs):
+
+		# 	if len(current_sample) < 1:
+		# 		break
+		# 	vals = pdme.util.fast_v_calc.fast_vs_for_dipoleses(
+		# 		numpy.array([di]), current_sample
+		# 	)
+
+		# 	current_sample = current_sample[
+		# 		numpy.all((vals > low) & (vals < high), axis=1)
+		# 	]
+		# return current_sample
 
 	def execute(self) -> DirectMonteCarloResult:
 		step_count = 0
 		total_success = 0
 		total_count = 0
 
 		count_per_step = (
```

### Comparing `deepdog-0.7.8/deepdog/real_spectrum_run.py` & `deepdog-0.7.9/deepdog/real_spectrum_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
 				axis=1,
 			)
 		]
 	return len(current_sample)
 
 
-def get_a_result_fast_filter_pair_phase_only(input) -> int:
+def get_a_result_fast_filter_potential_pair_phase_only(input) -> int:
 	(
 		model,
 		pair_inputs,
 		pair_phase_lows,
 		pair_phase_highs,
 		monte_carlo_count,
 		seed,
@@ -98,14 +98,111 @@
 				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
 				axis=1,
 			)
 		]
 	return len(current_sample)
 
 
+def get_a_result_fast_filter_tarucha_spin_qubit_pair_phase_only(input) -> int:
+	(
+		model,
+		pair_inputs,
+		pair_phase_lows,
+		pair_phase_highs,
+		monte_carlo_count,
+		seed,
+	) = input
+
+	def fast_s_spin_qubit_tarucha_nonlocal_dipoleses(
+		dot_pair_inputs: numpy.ndarray, dipoleses: numpy.ndarray
+	) -> numpy.ndarray:
+		"""
+		No error correction here baby.
+		"""
+		ps = dipoleses[:, :, 0:3]
+		ss = dipoleses[:, :, 3:6]
+		ws = dipoleses[:, :, 6]
+
+		r1s = dot_pair_inputs[:, 0, 0:3]
+		r2s = dot_pair_inputs[:, 1, 0:3]
+		f1s = dot_pair_inputs[:, 0, 3]
+		# don't actually need, because we're assuming they're the same frequencies across the pair
+		# f2s = dot_pair_inputs[:, 1, 3]
+
+		diffses1 = r1s[:, None] - ss[:, None, :]
+		diffses2 = r2s[:, None] - ss[:, None, :]
+
+		norms1 = numpy.linalg.norm(diffses1, axis=3)
+		norms2 = numpy.linalg.norm(diffses2, axis=3)
+
+		alphses1 = (
+			(
+				3
+				* numpy.transpose(
+					numpy.transpose(
+						numpy.einsum("abcd,acd->abc", diffses1, ps) / (norms1**2)
+					)
+					* numpy.transpose(diffses1)
+				)[:, :, :, 0]
+			)
+			- ps[:, :, 0, numpy.newaxis]
+		) / (norms1**3)
+		alphses2 = (
+			(
+				3
+				* numpy.transpose(
+					numpy.transpose(
+						numpy.einsum("abcd,acd->abc", diffses2, ps) / (norms2**2)
+					)
+					* numpy.transpose(diffses2)
+				)[:, :, :, 0]
+			)
+			- ps[:, :, 0, numpy.newaxis]
+		) / (norms2**3)
+
+		bses = (1 / numpy.pi) * (
+			ws[:, None, :] / (f1s[:, None] ** 2 + ws[:, None, :] ** 2)
+		)
+
+		return numpy.einsum("...j->...", alphses1 * alphses2 * bses)
+
+	rng = numpy.random.default_rng(seed)
+	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
+	sample_dipoles = model.get_monte_carlo_dipole_inputs(
+		monte_carlo_count, None, rng_to_use=rng
+	)
+
+	current_sample = sample_dipoles
+
+	for pi, plow, phigh in zip(pair_inputs, pair_phase_lows, pair_phase_highs):
+		if len(current_sample) < 1:
+			break
+
+		###
+		# This should be  abstracted out, but we're going to dump it here for time pressure's sake
+		###
+		# vals = pdme.util.fast_nonlocal_spectrum.signarg(
+		# 	pdme.util.fast_nonlocal_spectrum.fast_s_nonlocal_dipoleses(
+		# 		numpy.array([pi]), current_sample
+		# 	)
+		#
+		vals = pdme.util.fast_nonlocal_spectrum.signarg(
+			fast_s_spin_qubit_tarucha_nonlocal_dipoleses(
+				numpy.array([pi]), current_sample
+			)
+		)
+		current_sample = current_sample[
+			numpy.all(
+				((vals > plow) & (vals < phigh)) | ((vals < plow) & (vals > phigh)),
+				axis=1,
+			)
+		]
+	return len(current_sample)
+
+
 def get_a_result_fast_filter(input) -> int:
 	model, dot_inputs, lows, highs, monte_carlo_count, seed = input
 
 	rng = numpy.random.default_rng(seed)
 	# TODO: A long term refactor is to pull the frequency stuff out from here. The None stands for max_frequency, which is unneeded in the actually useful models.
 	sample_dipoles = model.get_monte_carlo_dipole_inputs(
 		monte_carlo_count, None, rng_to_use=rng
@@ -295,14 +392,15 @@
 
 					# generate a seed from the sequence for each core.
 					# note this needs to be inside the loop for monte carlo cycle steps!
 					# that way we get more stuff.
 					seeds = seed_sequence.spawn(self.monte_carlo_cycles)
 
 					if self.use_pair_measurements:
+						_logger.debug("using pair measurements")
 						current_success = sum(
 							pool.imap_unordered(
 								get_a_result_fast_filter_pairs,
 								[
 									(
 										model,
 										self.dot_inputs_array,
@@ -316,17 +414,19 @@
 									)
 									for seed in seeds
 								],
 								self.chunksize,
 							)
 						)
 					elif self.use_pair_phase_measurements:
+						_logger.debug("using pair phase measurements")
+						_logger.debug("specifically using tarucha")
 						current_success = sum(
 							pool.imap_unordered(
-								get_a_result_fast_filter_pairs,
+								get_a_result_fast_filter_tarucha_spin_qubit_pair_phase_only,
 								[
 									(
 										model,
 										self.dot_pair_inputs_array,
 										pair_phase_lows,
 										pair_phase_highs,
 										self.monte_carlo_count,
```

### Comparing `deepdog-0.7.8/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-0.7.9/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.8/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.7.9/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.8/pyproject.toml` & `deepdog-0.7.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.7.8"
+version = "0.7.9"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 pdme = "^0.9.3"
 numpy = "1.22.3"
```

