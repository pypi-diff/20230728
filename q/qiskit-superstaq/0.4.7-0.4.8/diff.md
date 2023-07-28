# Comparing `tmp/qiskit-superstaq-0.4.7.tar.gz` & `tmp/qiskit-superstaq-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-superstaq-0.4.7.tar", last modified: Wed Jul 26 21:52:38 2023, max compression
+gzip compressed data, was "qiskit-superstaq-0.4.8.tar", last modified: Fri Jul 28 17:44:28 2023, max compression
```

## Comparing `qiskit-superstaq-0.4.7.tar` & `qiskit-superstaq-0.4.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:38.480159 qiskit-superstaq-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-26 21:52:38.480159 qiskit-superstaq-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/example-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:38.480159 qiskit-superstaq-0.4.7/qiskit_superstaq/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/compiler_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/compiler_output_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/custom_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/custom_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/daily_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16248 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_job_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16310 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/qiskit_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:38.480159 qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-26 21:52:38.000000 qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-26 21:52:38.000000 qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:52:38.000000 qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 21:52:38.000000 qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 21:52:38.000000 qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 21:51:58.000000 qiskit-superstaq-0.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:52:38.480159 qiskit-superstaq-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/example-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/qiskit_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/daily_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20716 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/qiskit_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 17:44:28.000000 qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 17:43:49.000000 qiskit-superstaq-0.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:44:28.480668 qiskit-superstaq-0.4.8/setup.cfg
```

### Comparing `qiskit-superstaq-0.4.7/PKG-INFO` & `qiskit-superstaq-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-superstaq
-Version: 0.4.7
+Version: 0.4.8
 Summary: The Qiskit module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `qiskit-superstaq-0.4.7/README.md` & `qiskit-superstaq-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/pyproject.toml` & `qiskit-superstaq-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/__init__.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/compiler_output.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/compiler_output_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/compiler_output_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/custom_gates.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/custom_gates_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/custom_gates_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/daily_integration_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/daily_integration_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,20 +212,35 @@
     num_qubits = 3
     depth = 1
     circuits, fidelities = provider.supercheq(files, num_qubits, depth)
     assert len(circuits) == 32
     assert fidelities.shape == (32, 32)
 
 
-def test_submit_to_provider_simulators(provider: qss.superstaq_provider.SuperstaqProvider) -> None:
+def test_dfe(provider: qss.superstaq_provider.SuperstaqProvider) -> None:
+    qc = qiskit.QuantumCircuit(1)
+    qc.h(0)
+    target = "ss_unconstrained_simulator"
+    ids = provider.submit_dfe(
+        rho_1=(qc, target),
+        rho_2=(qc, target),
+        num_random_bases=5,
+        shots=1000,
+    )
+    assert len(ids) == 2
 
+    result = provider.process_dfe(ids)
+    assert isinstance(result, float)
+
+
+@pytest.mark.parametrize(
+    "target", ["cq_hilbert_simulator", "aws_sv1_simulator", "ibmq_qasm_simulator"]
+)
+def test_submit_to_provider_simulators(target: str, provider: qss.SuperstaqProvider) -> None:
     qc = qiskit.QuantumCircuit(2, 2)
     qc.x(0)
     qc.cx(0, 1)
     qc.measure(0, 0)
     qc.measure(1, 1)
 
-    backends = ["cq_hilbert_simulator", "aws_sv1_simulator", "ibmq_qasm_simulator"]
-
-    for backend in backends:
-        job = provider.get_backend(backend).run(qc, shots=1)
-        assert job.result().get_counts() == {"11": 1}
+    job = provider.get_backend(target).run(qc, shots=1)
+    assert job.result().get_counts() == {"11": 1}
```

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/serialization.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/serialization_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/serialization_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_backend.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -291,16 +291,18 @@
             final_logical_to_physicals,
             pulse_sequences=pulses,
         )
 
     def qscout_compile(
         self,
         circuits: Union[qiskit.QuantumCircuit, Sequence[qiskit.QuantumCircuit]],
-        mirror_swaps: bool = True,
+        *,
+        mirror_swaps: bool = False,
         base_entangling_gate: str = "xx",
+        num_qubits: Optional[int] = None,
         **kwargs: Any,
     ) -> qss.compiler_output.CompilerOutput:
         """Compiles and optimizes the given circuit(s) for the QSCOUT trapped-ion testbed at Sandia
         National Laboratories [1].
 
         Compiled circuits are returned as both `qiskit.QuantumCircuit` objects and corresponding
         Jaqal [2] programs (strings).
@@ -313,14 +315,16 @@
                 International Conference on Quantum Computing and Engineering (QCE), 402-408 (2020).
                 https://arxiv.org/abs/2008.08042.
 
         Args:
             circuits: The circuit(s) to compile.
             mirror_swaps: Whether to use mirror swapping to reduce two-qubit gate overhead.
             base_entangling_gate: The base entangling gate to use (either "xx" or "zz").
+            num_qubits: An optional number of qubits that should be present in the compiled
+                circuit(s) and Jaqal program(s) (otherwise this will be determined from the input).
             kwargs: Other desired qscout_compile options.
 
         Returns:
             Object whose .circuit(s) attribute contains optimized `qiskit QuantumCircuit`(s), and
             `.jaqal_program(s)` attribute contains the corresponding Jaqal program(s).
 
         Raises:
@@ -334,14 +338,19 @@
             raise ValueError("base_entangling_gate must be either 'xx' or 'zz'")
 
         options = {
             **kwargs,
             "mirror_swaps": mirror_swaps,
             "base_entangling_gate": base_entangling_gate,
         }
+
+        if num_qubits is not None:
+            gss.validation.validate_integer_param(num_qubits)
+            options["num_qubits"] = num_qubits
+
         request_json = self._get_compile_request_json(circuits, **options)
         circuits_is_list = not isinstance(circuits, qiskit.QuantumCircuit)
         json_dict = self._provider._client.qscout_compile(request_json)
         return qss.compiler_output.read_json_qscout(json_dict, circuits_is_list)
 
     def cq_compile(
         self,
```

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_backend_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_backend_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_job.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,7 +192,22 @@
     def submit(self) -> None:
         """Unsupported submission call.
 
         Raises:
             NotImplementedError: If a job is submitted via SuperstaqJob.
         """
         raise NotImplementedError("Submit through SuperstaqBackend, not through SuperstaqJob")
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Refreshes and returns job information.
+
+        Note:
+            The contents of this dictionary are not guaranteed to be consistent over time. Whenever
+            possible, users should use the specific `SuperstaqJob` methods to retrieve the desired
+            job information instead of relying on particular entries in the output of this method.
+
+        Returns:
+            A dictionary containing updated job information.
+        """
+        if self._overall_status not in self.TERMINAL_STATES:
+            self._refresh_job()
+        return self._job_info
```

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_job_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_job_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,7 +228,22 @@
     assert job != "super.tech"
 
     job2 = qss.SuperstaqJob(backend=backend, job_id="123456")
     assert job != job2
 
     job3 = qss.SuperstaqJob(backend=backend, job_id="12345")
     assert job == job3
+
+
+def test_to_dict(backend: qss.SuperstaqBackend) -> None:
+    job = qss.SuperstaqJob(backend=backend, job_id="12345")
+    with mock.patch(
+        "general_superstaq.superstaq_client._SuperstaqClient.get_job",
+        return_value=mock_response("Done"),
+    ):
+        assert job.to_dict() == {
+            "12345": {
+                "status": "Done",
+                "samples": {"10": 100},
+                "shots": 100,
+            }
+        }
```

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_provider.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -268,17 +268,19 @@
             raise ValueError(f"{target!r} is not a valid IBMQ target.")
 
         return self.get_backend(target).compile(circuits, **kwargs)
 
     def qscout_compile(
         self,
         circuits: Union[qiskit.QuantumCircuit, Sequence[qiskit.QuantumCircuit]],
+        target: str = "sandia_qscout_qpu",
+        *,
         mirror_swaps: bool = False,
         base_entangling_gate: str = "xx",
-        target: str = "sandia_qscout_qpu",
+        num_qubits: Optional[int] = None,
         **kwargs: Any,
     ) -> qss.compiler_output.CompilerOutput:
         """Compiles and optimizes the given circuit(s) for the QSCOUT trapped-ion testbed at
         Sandia National Laboratories [1].
 
         Compiled circuits are returned as both `qiskit.QuantumCircuit` objects and corresponding
         Jaqal [2] programs (strings).
@@ -292,29 +294,35 @@
                 https://arxiv.org/abs/2008.08042.
 
         Args:
             circuits: The circuit(s) to compile.
             target: A string containing the name of a target backend.
             mirror_swaps: Whether to use mirror swapping to reduce two-qubit gate overhead.
             base_entangling_gate: The base entangling gate to use (either "xx" or "zz").
+            num_qubits: An optional number of qubits that should be present in the compiled
+                circuit(s) and Jaqal program(s) (otherwise this will be determined from the input).
             kwargs: Other desired qscout_compile options.
 
         Returns:
             Object whose .circuit(s) attribute contains optimized `qiskit QuantumCircuit`(s), and
             `.jaqal_program(s)` attribute contains the corresponding Jaqal program(s).
 
         Raises:
             ValueError: If `target` is not a valid Sandia target.
             ValueError: If `base_entangling_gate` is not a valid gate option.
         """
         if not target.startswith("sandia_"):
             raise ValueError(f"{target!r} is not a valid Sandia target.")
 
         return self.get_backend(target).compile(
-            circuits, mirror_swaps=mirror_swaps, base_entangling_gate=base_entangling_gate, **kwargs
+            circuits,
+            mirror_swaps=mirror_swaps,
+            base_entangling_gate=base_entangling_gate,
+            num_qubits=num_qubits,
+            **kwargs,
         )
 
     def cq_compile(
         self,
         circuits: Union[qiskit.QuantumCircuit, Sequence[qiskit.QuantumCircuit]],
         target: str = "cq_hilbert_qpu",
         **kwargs: Any,
@@ -357,14 +365,107 @@
                 fidelity matrices.
         """
         json_dict = self._client.supercheq(files, num_qubits, depth, "qiskit_circuits")
         circuits = qss.serialization.deserialize_circuits(json_dict["qiskit_circuits"])
         fidelities = gss.serialization.deserialize(json_dict["fidelities"])
         return circuits, fidelities
 
+    def submit_dfe(
+        self,
+        rho_1: Tuple[qiskit.QuantumCircuit, str],
+        rho_2: Tuple[qiskit.QuantumCircuit, str],
+        num_random_bases: int,
+        shots: int,
+        **kwargs: Any,
+    ) -> List[str]:
+        """Executes the circuits neccessary for the DFE protocol.
+
+        The circuits used to prepare the desired states should not contain final measurements, but
+        can contain mid-circuit measurements (as long as the intended target supports them). For
+        example, to prepare a Bell state to be ran in `ss_unconstrained_simulator`, you should pass
+        `qc = qiskit.QuantumCircuit(2); qc.h(0); qc.cx(0, 1)` as the first element of some `rho_i`
+        (note there are no final measurements).
+
+        The fidelity between states is calculated following the random measurement protocol
+        outlined in [1].
+
+        References:
+            [1] Elben, Andreas, Benoît Vermersch, Rick van Bijnen, Christian Kokail, Tiff Brydges,
+                Christine Maier, Manoj K. Joshi, Rainer Blatt, Christian F. Roos, and Peter Zoller.
+                "Cross-platform verification of intermediate scale quantum devices." Physical
+                review letters 124, no. 1 (2020): 010504.
+
+        Args:
+            rho_1: Tuple containing the information to prepare the first state. It contains a
+                `qiskit.QuantumCircuit` at index 0 and a target name at index 1.
+            rho_2: Tuple containing the information to prepare the second state. It contains a
+                `qiskit.QuantumCircuit` at index 0 and a target name at index 1.
+            num_random_bases: Number of random bases to measure each state in.
+            shots: Number of shots to use per random basis.
+            kwargs: Other execution parameters.
+                - tag: Tag for all jobs submitted for this protocol.
+                - lifespan: How long to store the jobs submitted for in days (only works with right
+                permissions).
+                - method: Which type of method to execute the circuits with.
+
+        Returns:
+            A list with two strings, which are the job ids that need to be passed to `process_dfe`
+            to post-process the measurement results and return the fidelity.
+
+        Raises:
+            ValueError: If `circuit` is not a valid `qiskit.QuantumCircuit`.
+            SuperstaqServerException: If there was an error accessing the API.
+        """
+        circuit_1 = rho_1[0]
+        circuit_2 = rho_2[0]
+        target_1 = rho_1[1]
+        target_2 = rho_2[1]
+
+        qss.validation.validate_qiskit_circuits(circuit_1)
+        qss.validation.validate_qiskit_circuits(circuit_2)
+        gss.validation.validate_target(target_1)
+        gss.validation.validate_target(target_2)
+
+        if not (
+            isinstance(circuit_1, qiskit.QuantumCircuit)
+            and isinstance(circuit_2, qiskit.QuantumCircuit)
+        ):
+            raise ValueError("Each state `rho_i` should contain a single circuit.")
+
+        serialized_circuit_1 = qss.serialization.serialize_circuits(circuit_1)
+        serialized_circuit_2 = qss.serialization.serialize_circuits(circuit_2)
+
+        ids = self._client.submit_dfe(
+            circuit_1={"qiskit_circuits": serialized_circuit_1},
+            target_1=target_1,
+            circuit_2={"qiskit_circuits": serialized_circuit_2},
+            target_2=target_2,
+            num_random_bases=num_random_bases,
+            shots=shots,
+            **kwargs,
+        )
+
+        return ids
+
+    def process_dfe(self, ids: List[str]) -> float:
+        """Process the results of a DFE protocol.
+
+        Args:
+            ids: A list (size two) of ids returned by a call to `submit_dfe`.
+
+        Returns:
+            The estimated fidelity between the two states as a float.
+
+        Raises:
+            ValueError: If `ids` is not of size two.
+            SuperstaqServerException: If there was an error accesing the API or the jobs submitted
+                through `submit_dfe` have not finished running.
+        """
+        return self._client.process_dfe(ids)
+
     def target_info(self, target: str) -> Dict[str, Any]:
         """Returns information about the device specified by `target`.
 
         Args:
             target: A string containing the name of a target backend.
 
         Returns:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/superstaq_provider_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/superstaq_provider_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -280,20 +280,27 @@
     qc = qiskit.QuantumCircuit()
 
     mock_post.return_value.json = lambda: {
         "qiskit_circuits": qss.serialization.serialize_circuits(qc),
         "final_logical_to_physicals": json.dumps([[(0, 13)]]),
         "jaqal_programs": [""],
     }
+
     _ = provider.qscout_compile(qc, mirror_swaps=mirror_swaps)
     mock_post.assert_called_once()
-    _, kwargs = mock_post.call_args
-    assert json.loads(kwargs["json"]["options"]) == {
+    assert json.loads(mock_post.call_args.kwargs["json"]["options"]) == {
+        "mirror_swaps": mirror_swaps,
+        "base_entangling_gate": "xx",
+    }
+
+    _ = provider.qscout_compile(qc, mirror_swaps=mirror_swaps, num_qubits=3)
+    assert json.loads(mock_post.call_args.kwargs["json"]["options"]) == {
         "mirror_swaps": mirror_swaps,
         "base_entangling_gate": "xx",
+        "num_qubits": 3,
     }
 
 
 @patch("requests.post")
 @pytest.mark.parametrize("base_entangling_gate", ("xx", "zz"))
 def test_qscout_compile_change_entangler(mock_post: MagicMock, base_entangling_gate: str) -> None:
     provider = qss.SuperstaqProvider(api_key="MY_TOKEN")
@@ -301,22 +308,29 @@
     qc = qiskit.QuantumCircuit()
 
     mock_post.return_value.json = lambda: {
         "qiskit_circuits": qss.serialization.serialize_circuits(qc),
         "final_logical_to_physicals": "[[]]",
         "jaqal_programs": [""],
     }
+
     _ = provider.qscout_compile(qc, base_entangling_gate=base_entangling_gate)
     mock_post.assert_called_once()
-    _, kwargs = mock_post.call_args
-    assert json.loads(kwargs["json"]["options"]) == {
+    assert json.loads(mock_post.call_args.kwargs["json"]["options"]) == {
         "mirror_swaps": False,
         "base_entangling_gate": base_entangling_gate,
     }
 
+    _ = provider.qscout_compile(qc, base_entangling_gate=base_entangling_gate, num_qubits=4)
+    assert json.loads(mock_post.call_args.kwargs["json"]["options"]) == {
+        "mirror_swaps": False,
+        "base_entangling_gate": base_entangling_gate,
+        "num_qubits": 4,
+    }
+
 
 @patch("requests.post")
 def test_qscout_compile_wrong_entangler(mock_post: MagicMock) -> None:
     provider = qss.SuperstaqProvider(api_key="MY_TOKEN")
 
     qc = qiskit.QuantumCircuit()
 
@@ -370,14 +384,39 @@
         "final_logical_to_physicals": "[[]]",
         "fidelities": gss.serialization.serialize(fidelities),
     }
     assert provider.supercheq([[0]], 1, 1) == (circuits, fidelities)
 
 
 @patch("requests.post")
+def test_dfe(mock_post: MagicMock) -> None:
+    provider = qss.SuperstaqProvider(api_key="key")
+    qc = qiskit.QuantumCircuit(1)
+    qc.h(0)
+    mock_post.return_value.json = lambda: ["id1", "id2"]
+    assert provider.submit_dfe(
+        rho_1=(qc, "ss_example_qpu"),
+        rho_2=(qc, "ss_example_qpu"),
+        num_random_bases=5,
+        shots=100,
+    ) == ["id1", "id2"]
+
+    with pytest.raises(ValueError, match="should contain a single circuit"):
+        provider.submit_dfe(
+            rho_1=([qc, qc], "ss_example_qpu"),
+            rho_2=(qc, "ss_example_qpu"),
+            num_random_bases=5,
+            shots=100,
+        )
+
+    mock_post.return_value.json = lambda: 1
+    assert provider.process_dfe(["1", "2"]) == 1
+
+
+@patch("requests.post")
 def test_target_info(mock_post: MagicMock) -> None:
     provider = qss.SuperstaqProvider(api_key="key")
     fake_data = {"target_info": {"backend_name": "ss_example_qpu", "max_experiments": 1234}}
     mock_post.return_value.json = lambda: fake_data
     assert provider.target_info("ss_example_qpu") == fake_data["target_info"]
```

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/validation.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq/validation_test.py` & `qiskit-superstaq-0.4.8/qiskit_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/PKG-INFO` & `qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-superstaq
-Version: 0.4.7
+Version: 0.4.8
 Summary: The Qiskit module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `qiskit-superstaq-0.4.7/qiskit_superstaq.egg-info/SOURCES.txt` & `qiskit-superstaq-0.4.8/qiskit_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

