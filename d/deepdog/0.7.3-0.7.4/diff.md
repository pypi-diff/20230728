# Comparing `tmp/deepdog-0.7.3.tar.gz` & `tmp/deepdog-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.7.3.tar", max compression
+gzip compressed data, was "deepdog-0.7.4.tar", max compression
```

## Comparing `deepdog-0.7.3.tar` & `deepdog-0.7.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      605 2023-07-27 01:28:09.712641 deepdog-0.7.3/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0     6973 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/bayes_run_with_ss.py
--rw-r--r--   0        0        0       73 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/meta.py
--rw-r--r--   0        0        0     8471 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0      110 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0     9657 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      898 2023-07-27 01:28:09.716642 deepdog-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      662 2023-07-27 01:29:16.137585 deepdog-0.7.3/setup.py
--rw-r--r--   0        0        0      361 2023-07-27 01:29:16.137938 deepdog-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      605 2023-07-27 22:41:43.464893 deepdog-0.7.4/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-07-27 22:41:43.464893 deepdog-0.7.4/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-07-27 22:41:43.464893 deepdog-0.7.4/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0     7530 2023-07-27 22:41:43.464893 deepdog-0.7.4/deepdog/bayes_run_with_ss.py
+-rw-r--r--   0        0        0       73 2023-07-27 22:41:43.464893 deepdog-0.7.4/deepdog/meta.py
+-rw-r--r--   0        0        0     8471 2023-07-27 22:41:43.464893 deepdog-0.7.4/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0      110 2023-07-27 22:41:43.468893 deepdog-0.7.4/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0    10287 2023-07-27 22:41:43.468893 deepdog-0.7.4/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2023-07-27 22:41:43.468893 deepdog-0.7.4/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      916 2023-07-27 22:41:43.468893 deepdog-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      662 2023-07-27 22:43:21.256860 deepdog-0.7.4/setup.py
+-rw-r--r--   0        0        0      361 2023-07-27 22:43:21.257464 deepdog-0.7.4/PKG-INFO
```

### Comparing `deepdog-0.7.3/deepdog/__init__.py` & `deepdog-0.7.4/deepdog/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.3/deepdog/bayes_run.py` & `deepdog-0.7.4/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.3/deepdog/bayes_run_simulpairs.py` & `deepdog-0.7.4/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.3/deepdog/bayes_run_with_ss.py` & `deepdog-0.7.4/deepdog/bayes_run_with_ss.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 		ss_use_adaptive_steps=True,
 		ss_default_phi_step=0.01,
 		ss_default_theta_step=0.01,
 		ss_default_r_step=0.01,
 		ss_default_w_log_step=0.01,
 		ss_default_upper_w_log_step=4,
 		ss_dump_last_generation=False,
+		ss_initial_costs_chunk_size=100,
+		write_output_to_bayesruncsv=True,
 	) -> None:
 		self.dot_inputs = pdme.inputs.inputs_with_frequency_range(
 			dot_positions, frequency_range
 		)
 		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
 			self.dot_inputs
 		)
@@ -131,21 +133,29 @@
 		self.ss_use_adaptive_steps = ss_use_adaptive_steps
 		self.ss_default_phi_step = ss_default_phi_step
 		self.ss_default_theta_step = ss_default_theta_step
 		self.ss_default_r_step = ss_default_r_step
 		self.ss_default_w_log_step = ss_default_w_log_step
 		self.ss_default_upper_w_log_step = ss_default_upper_w_log_step
 		self.ss_dump_last_generation = ss_dump_last_generation
-
+		self.ss_initial_costs_chunk_size = ss_initial_costs_chunk_size
 		self.run_count = run_count
 
-	def go(self) -> None:
-		with open(self.filename, "a", newline="") as outfile:
-			writer = csv.DictWriter(outfile, fieldnames=self.csv_fields, dialect="unix")
-			writer.writeheader()
+		self.write_output_to_csv = write_output_to_bayesruncsv
+
+	def go(self) -> Sequence:
+
+		if self.write_output_to_csv:
+			with open(self.filename, "a", newline="") as outfile:
+				writer = csv.DictWriter(
+					outfile, fieldnames=self.csv_fields, dialect="unix"
+				)
+				writer.writeheader()
+
+		return_result = []
 
 		for run in range(1, self.run_count + 1):
 
 			# Generate the actual dipoles
 			actual_dipoles = self.actual_model.get_dipoles(self.max_frequency)
 
 			measurements = actual_dipoles.get_dot_measurements(self.dot_inputs)
@@ -170,14 +180,15 @@
 					self.ss_mcmc_seed,
 					self.ss_use_adaptive_steps,
 					self.ss_default_phi_step,
 					self.ss_default_theta_step,
 					self.ss_default_r_step,
 					self.ss_default_w_log_step,
 					self.ss_default_upper_w_log_step,
+					initial_cost_chunk_size=self.ss_initial_costs_chunk_size,
 					keep_probs_list=False,
 					dump_last_generation_to_file=self.ss_dump_last_generation,
 				)
 				results.append(subset_run.execute())
 
 			_logger.debug("Done, constructing output now")
 			row = {
@@ -195,15 +206,19 @@
 					_logger.info(f"Not writing anymore, saw end after {i}")
 					break
 
 			likelihoods: List[float] = []
 
 			for (name, result) in zip(self.model_names, results):
 				if result.over_target_likelihood is None:
-					clamped_likelihood = result.probs_list[-1][0] / CLAMPING_FACTOR
+					if result.lowest_likelihood is None:
+						_logger.error(f"result {result} looks bad")
+						clamped_likelihood = 10**-15
+					else:
+						clamped_likelihood = result.lowest_likelihood / CLAMPING_FACTOR
 					_logger.warning(
 						f"got a none result, clamping to {clamped_likelihood}"
 					)
 				else:
 					clamped_likelihood = result.over_target_likelihood
 				likelihoods.append(clamped_likelihood)
 				row[f"{name}_likelihood"] = clamped_likelihood
@@ -218,21 +233,25 @@
 				likelihood * old_prob / success_weight
 				for likelihood, old_prob in zip(likelihoods, self.probabilities)
 			]
 			self.probabilities = new_probabilities
 			for name, probability in zip(self.model_names, self.probabilities):
 				row[f"{name}_prob"] = probability
 			_logger.info(row)
+			return_result.append(row)
 
-			with open(self.filename, "a", newline="") as outfile:
-				writer = csv.DictWriter(
-					outfile, fieldnames=self.csv_fields, dialect="unix"
-				)
-				writer.writerow(row)
+			if self.write_output_to_csv:
+				with open(self.filename, "a", newline="") as outfile:
+					writer = csv.DictWriter(
+						outfile, fieldnames=self.csv_fields, dialect="unix"
+					)
+					writer.writerow(row)
 
 			if self.use_end_threshold:
 				max_prob = max(self.probabilities)
 				if max_prob > self.end_threshold:
 					_logger.info(
 						f"Aborting early, because {max_prob} is greater than {self.end_threshold}"
 					)
 					break
+
+		return return_result
```

### Comparing `deepdog-0.7.3/deepdog/real_spectrum_run.py` & `deepdog-0.7.4/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.3/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-0.7.4/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 		default_phi_step=0.01,
 		default_theta_step=0.01,
 		default_r_step=0.01,
 		default_w_log_step=0.01,
 		default_upper_w_log_step=4,
 		keep_probs_list=True,
 		dump_last_generation_to_file=False,
+		initial_cost_chunk_size=100,
 	):
 		name, model = model_name_pair
 		self.model_name = name
 		self.model = model
 		_logger.info(f"got model {self.model_name}")
 
 		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
@@ -81,26 +82,35 @@
 
 		self.target_cost = target_cost
 		_logger.info(f"will stop at target cost {target_cost}")
 
 		self.keep_probs_list = keep_probs_list
 		self.dump_last_generations = dump_last_generation_to_file
 
+		self.initial_cost_chunk_size = initial_cost_chunk_size
+
 	def execute(self) -> SubsetSimulationResult:
 
 		probs_list = []
 
 		sample_dipoles = self.model.get_monte_carlo_dipole_inputs(
 			self.n_c * self.n_s,
 			-1,
 			rng_to_use=numpy.random.default_rng(self.level_0_seed),
 		)
 		# _logger.debug(sample_dipoles)
 		# _logger.debug(sample_dipoles.shape)
-		costs = self.cost_function_to_use(sample_dipoles)
+
+		raw_costs = []
+		_logger.debug(f"Using iterated cost function thing with chunk size {self.initial_cost_chunk_size}")
+
+		for x in range(0, len(sample_dipoles), self.initial_cost_chunk_size):
+			_logger.debug(f"doing chunk {x}")
+			raw_costs.extend(self.cost_function_to_use(sample_dipoles[x: x + self.initial_cost_chunk_size]))
+		costs = numpy.array(raw_costs)
 
 		_logger.debug(f"costs: {costs}")
 		sorted_indexes = costs.argsort()[::-1]
 
 		_logger.debug(costs[sorted_indexes])
 		_logger.debug(sample_dipoles[sorted_indexes])
 
@@ -116,15 +126,15 @@
 			]
 		)
 		all_chains = list(zip(sorted_costs, all_dipoles))
 
 		mcmc_rng = numpy.random.default_rng(self.mcmc_seed)
 
 		for i in range(self.m_max):
-			next_seeds = all_chains[-self.n_c:]
+			next_seeds = all_chains[-self.n_c :]
 
 			if self.dump_last_generations:
 				_logger.info("writing out csv file")
 				next_dipoles_seed_dipoles = numpy.array([n[1] for n in next_seeds])
 				for n in range(self.model.n):
 					_logger.info(f"{next_dipoles_seed_dipoles[:, n].shape}")
 					numpy.savetxt(
@@ -144,19 +154,22 @@
 						)
 					)
 
 			next_seeds_as_array = numpy.array([s for _, s in next_seeds])
 
 			stdevs = self.get_stdevs_from_arrays(next_seeds_as_array)
 			_logger.info(f"got stdevs: {stdevs.stdevs}")
-
+			_logger.debug("Starting the MCMC")
 			all_chains = []
-			for c, s in next_seeds:
+			for seed_index, (c, s) in enumerate(next_seeds):
 				# chain = mcmc(s, threshold_cost, n_s, model, dot_inputs_array, actual_measurement_array, mcmc_rng, curr_cost=c, stdevs=stdevs)
 				# until new version gotta do
+				_logger.debug(
+					f"\t{seed_index}: getting another chain from the next seed"
+				)
 				chain = self.model.get_mcmc_chain(
 					s,
 					self.cost_function_to_use,
 					self.n_s,
 					threshold_cost,
 					stdevs,
 					initial_cost=c,
@@ -164,18 +177,19 @@
 				)
 				for cost, chained in chain:
 					try:
 						filtered_cost = cost[0]
 					except IndexError:
 						filtered_cost = cost
 					all_chains.append((filtered_cost, chained))
-
+			_logger.debug("finished mcmc")
 			# _logger.debug(all_chains)
 
 			all_chains.sort(key=lambda c: c[0], reverse=True)
+			_logger.debug("finished sorting all_chains")
 
 			threshold_cost = all_chains[-self.n_c][0]
 			_logger.info(
 				f"current threshold cost: {threshold_cost}, at P = (1 / {self.n_s})^{i + 1}"
 			)
 			if (self.target_cost is not None) and (threshold_cost < self.target_cost):
 				_logger.info(
@@ -236,15 +250,15 @@
 		)
 		for a in all_chains[-10:]:
 			_logger.info(a)
 		# for prob, prob_cost in probs_list:
 		# 	_logger.info(f"\t{prob}: {prob_cost}")
 		probs_list.sort(key=lambda c: c[0], reverse=True)
 
-		min_likelihood = ((1) / (self.n_c * self.n_s)) / (self.n_s ** (self.m_max + 1))
+		min_likelihood = ((1) / (self.n_c * self.n_s)) / (self.n_s ** (self.m_max))
 
 		result = SubsetSimulationResult(
 			probs_list=probs_list,
 			over_target_cost=None,
 			over_target_likelihood=None,
 			under_target_cost=None,
 			under_target_likelihood=None,
```

### Comparing `deepdog-0.7.3/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.7.4/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.3/pyproject.toml` & `deepdog-0.7.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.7.3"
+version = "0.7.4"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 pdme = "^0.9.1"
 numpy = "1.22.3"
@@ -13,14 +13,15 @@
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.1"
 pytest-cov = "^4.1.0"
 mypy = "^0.971"
 python-semantic-release = "^7.24.0"
 black = "^22.3.0"
+syrupy = "^4.0.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `deepdog-0.7.3/setup.py` & `deepdog-0.7.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy==1.22.3', 'pdme>=0.9.1,<0.10.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.7.3',
+    'version': '0.7.4',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

