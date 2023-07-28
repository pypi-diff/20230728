# Comparing `tmp/cirq-superstaq-0.4.7.tar.gz` & `tmp/cirq-superstaq-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirq-superstaq-0.4.7.tar", last modified: Wed Jul 26 21:52:57 2023, max compression
+gzip compressed data, was "cirq-superstaq-0.4.8.tar", last modified: Fri Jul 28 17:44:46 2023, max compression
```

## Comparing `cirq-superstaq-0.4.7.tar` & `cirq-superstaq-0.4.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:57.976626 cirq-superstaq-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 21:52:57.976626 cirq-superstaq-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:57.972626 cirq-superstaq-0.4.7/cirq_superstaq/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/compiler_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/compiler_output_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/daily_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/job_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:57.976626 cirq-superstaq-0.4.7/cirq_superstaq/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/ops/qubit_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/ops/qubit_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/ops/qudit_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16989 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/ops/qudit_gates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28702 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22661 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/cirq_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:57.976626 cirq-superstaq-0.4.7/cirq_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 21:52:57.000000 cirq-superstaq-0.4.7/cirq_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-26 21:52:57.000000 cirq-superstaq-0.4.7/cirq_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:52:57.000000 cirq-superstaq-0.4.7/cirq_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 21:52:57.000000 cirq-superstaq-0.4.7/cirq_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 21:52:57.000000 cirq-superstaq-0.4.7/cirq_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/example-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 21:51:58.000000 cirq-superstaq-0.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:52:57.976626 cirq-superstaq-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.916900 cirq-superstaq-0.4.8/cirq_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/compiler_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/compiler_output_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/daily_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/job_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/cirq_superstaq/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35310 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38578 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16989 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33059 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24505 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/cirq_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:46.916900 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 17:44:46.000000 cirq-superstaq-0.4.8/cirq_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/example-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 17:43:49.000000 cirq-superstaq-0.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:44:46.920900 cirq-superstaq-0.4.8/setup.cfg
```

### Comparing `cirq-superstaq-0.4.7/PKG-INFO` & `cirq-superstaq-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirq-superstaq
-Version: 0.4.7
+Version: 0.4.8
 Summary: The Cirq module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cirq-superstaq-0.4.7/README.md` & `cirq-superstaq-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/__init__.py` & `cirq-superstaq-0.4.8/cirq_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/compiler_output.py` & `cirq-superstaq-0.4.8/cirq_superstaq/compiler_output.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/compiler_output_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/compiler_output_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/daily_integration_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/daily_integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,29 @@
     num_qubits = 3
     depth = 1
     circuits, fidelities = service.supercheq(files, num_qubits, depth)
     assert len(circuits) == 32
     assert fidelities.shape == (32, 32)
 
 
+def test_dfe(service: css.Service) -> None:
+    circuit = cirq.Circuit(cirq.H(cirq.q(0)))
+    target = "ss_unconstrained_simulator"
+    ids = service.submit_dfe(
+        rho_1=(circuit, target),
+        rho_2=(circuit, target),
+        num_random_bases=5,
+        shots=1000,
+    )
+    assert len(ids) == 2
+
+    result = service.process_dfe(ids)
+    assert isinstance(result, float)
+
+
 def test_job(service: css.Service) -> None:
     circuit = cirq.Circuit(cirq.measure(cirq.q(0)))
     job = service.create_job(circuit, target="ibmq_qasm_simulator", repetitions=10)
 
     job_id = job.job_id()  # To test for https://github.com/Infleqtion/client-superstaq/issues/452
 
     assert job.counts() == {"0": 10}
@@ -255,17 +270,17 @@
 
     # State retrieved from the server should be the same:
     assert job.counts() == {"0": 10}
     assert job.status() == "Done"
     assert job.job_id() == job_id
 
 
-def test_submit_to_provider_simulators(service: css.Service) -> None:
+@pytest.mark.parametrize(
+    "target", ["cq_hilbert_simulator", "aws_sv1_simulator", "ibmq_qasm_simulator"]
+)
+def test_submit_to_provider_simulators(target: str, service: css.Service) -> None:
     q0 = cirq.LineQubit(0)
     q1 = cirq.LineQubit(1)
     circuit = cirq.Circuit(cirq.X(q0), cirq.CNOT(q0, q1), cirq.measure(q0, q1))
 
-    targets = ["cq_hilbert_simulator", "aws_sv1_simulator", "ibmq_qasm_simulator"]
-
-    for target in targets:
-        job = service.create_job(circuit=circuit, repetitions=1, target=target)
-        assert job.counts() == {"11": 1}
+    job = service.create_job(circuit=circuit, repetitions=1, target=target)
+    assert job.counts() == {"11": 1}
```

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/job.py` & `cirq-superstaq-0.4.8/cirq_superstaq/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,14 +188,28 @@
                 )
             time.sleep(polling_seconds)
             time_waited_seconds += polling_seconds
 
         self._check_if_unsuccessful()
         return self._job["samples"]
 
+    def to_dict(self) -> Dict[str, Any]:
+        """Refreshes and returns job information.
+
+        Note:
+            The contents of this dictionary are not guaranteed to be consistent over time. Whenever
+            possible, users should use the specific `Job` methods to retrieve the desired job
+            information instead of relying on particular entries in the output of this method.
+
+        Returns:
+            A dictionary containing updated job information.
+        """
+        self._refresh_job()
+        return self._job
+
     def __str__(self) -> str:
         return f"Job with job_id={self.job_id()}"
 
     def __repr__(self) -> str:
         return f"css.Job(client={self._client!r}, job_id={self.job_id()!r})"
 
     def _value_equality_values_(self) -> Tuple[str, Dict[str, Any]]:
```

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/job_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/job_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,27 @@
     cirq.testing.assert_equivalent_repr(
         job, setup_code="import cirq_superstaq as css\nimport general_superstaq as gss"
     )
 
     assert not job == 1
 
 
+def test_job_to_dict(job: css.job.Job) -> None:
+    job_dict = {
+        "data": {"histogram": {"11": 1}},
+        "num_qubits": 2,
+        "samples": {"11": 1},
+        "shots": 1,
+        "status": "Done",
+        "target": "ss_unconstrained_simulator",
+    }
+    with mocked_get_job_requests(job_dict):
+        assert job.to_dict() == job_dict
+
+
 def test_job_counts(job: css.job.Job) -> None:
     job_dict = {
         "data": {"histogram": {"11": 1}},
         "num_qubits": 2,
         "samples": {"11": 1},
         "shots": 1,
         "status": "Done",
```

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/ops/__init__.py` & `cirq-superstaq-0.4.8/cirq_superstaq/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/ops/qubit_gates.py` & `cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/ops/qubit_gates_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/ops/qubit_gates_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/ops/qudit_gates.py` & `cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/ops/qudit_gates_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/ops/qudit_gates_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/sampler.py` & `cirq-superstaq-0.4.8/cirq_superstaq/sampler.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/serialization.py` & `cirq-superstaq-0.4.8/cirq_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/serialization_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/serialization_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/service.py` & `cirq-superstaq-0.4.8/cirq_superstaq/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -172,16 +172,16 @@
         circuit: cirq.Circuit,
         repetitions: int,
         target: Optional[str] = None,
         param_resolver: cirq.ParamResolverOrSimilarType = cirq.ParamResolver({}),
         method: Optional[str] = None,
         **kwargs: Any,
     ) -> Dict[str, int]:
-        """Runs the given circuit on the Superstaq API and returns the result
-        of the ran circuit as a `collections.Counter`.
+        """Runs the given circuit on the Superstaq API and returns the result of the circuit ran as
+        a `collections.Counter`.
 
         Args:
             circuit: The circuit to run.
             repetitions: The number of times to run the circuit.
             target: Where to run the job.
             param_resolver: A `cirq.ParamResolver` to resolve parameters in  `circuit`.
             method: Optional execution method.
@@ -201,16 +201,16 @@
         circuit: cirq.Circuit,
         repetitions: int,
         target: Optional[str] = None,
         param_resolver: cirq.ParamResolver = cirq.ParamResolver({}),
         method: Optional[str] = None,
         **kwargs: Any,
     ) -> cirq.ResultDict:
-        """Run the given circuit on the Superstaq API and returns the result
-        of the ran circut as a `cirq.ResultDict`.
+        """Runs the given circuit on the Superstaq API and returns the result of the circuit ran as
+        a `cirq.ResultDict`.
 
         Args:
             circuit: The circuit to run.
             repetitions: The number of times to run the circuit.
             target: Where to run the job.
             param_resolver: A `cirq.ParamResolver` to resolve parameters in `circuit`.
             method: Execution method.
@@ -502,17 +502,19 @@
 
         json_dict = self._client.post_request("/aqt_compile", request_json)
         return css.compiler_output.read_json_aqt(json_dict, circuits_is_list, num_eca_circuits)
 
     def qscout_compile(
         self,
         circuits: Union[cirq.Circuit, Sequence[cirq.Circuit]],
+        target: str = "sandia_qscout_qpu",
+        *,
         mirror_swaps: bool = False,
         base_entangling_gate: str = "xx",
-        target: str = "sandia_qscout_qpu",
+        num_qubits: Optional[int] = None,
         **kwargs: Any,
     ) -> css.compiler_output.CompilerOutput:
         """Compiles and optimizes the given circuit(s) for the QSCOUT trapped-ion testbed at
         Sandia National Laboratories [1].
 
         Compiled circuits are returned as both `cirq.Circuit` objects and corresponding Jaqal [2]
         programs (strings).
@@ -526,14 +528,16 @@
                 https://arxiv.org/abs/2008.08042.
 
         Args:
             circuits: The circuit(s) to compile.
             target: String of target representing target device.
             mirror_swaps: Whether to use mirror swapping to reduce two-qubit gate overhead.
             base_entangling_gate: The base entangling gate to use (either "xx" or "zz").
+            num_qubits: An optional number of qubits that should be initialized in the returned
+                Jaqal program(s) (by default this will be determined from the input circuits).
             kwargs: Other desired qscout_compile options.
 
         Returns:
             Object whose .circuit(s) attribute contains optimized `cirq.Circuit`(s), and
             `.jaqal_program(s)` attribute contains the corresponding Jaqal program(s).
 
         Raises:
@@ -553,14 +557,18 @@
 
         options_dict = {
             "mirror_swaps": mirror_swaps,
             "base_entangling_gate": base_entangling_gate,
             **kwargs,
         }
 
+        if num_qubits is not None:
+            gss.validation.validate_integer_param(num_qubits)
+            options_dict["num_qubits"] = num_qubits
+
         json_dict = self._client.qscout_compile(
             {
                 "cirq_circuits": serialized_circuits,
                 "options": cirq.to_json(options_dict),
                 "target": target,
             }
         )
@@ -684,14 +692,102 @@
         """
 
         json_dict = self._client.supercheq(files, num_qubits, depth, "cirq_circuits")
         circuits = css.serialization.deserialize_circuits(json_dict["cirq_circuits"])
         fidelities = gss.serialization.deserialize(json_dict["fidelities"])
         return circuits, fidelities
 
+    def submit_dfe(
+        self,
+        rho_1: Tuple[cirq.AbstractCircuit, str],
+        rho_2: Tuple[cirq.AbstractCircuit, str],
+        num_random_bases: int,
+        shots: int,
+        **kwargs: Any,
+    ) -> List[str]:
+        """Executes the circuits neccessary for the DFE protocol.
+
+        The circuits used to prepare the desired states should not contain final measurements, but
+        can contain mid-circuit measurements (as long as the intended target supports them). For
+        example, to prepare a Bell state to be ran in `ss_unconstrained_simulator`, you should pass
+        `cirq.Circuit(cirq.H(qubits[0]), cirq.CX(qubits[0], qubits[1]))` as the first element of
+        some `rho_i` (note there are no final measurements).
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
+                `cirq.Circuit` at index 0 and a target name at index 1.
+            rho_2: Tuple containing the information to prepare the second state. It contains a
+                `cirq.Circuit` at index 0 and a target name at index 1.
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
+            ValueError: If `circuit` is not a valid `cirq.Circuit`.
+            SuperstaqServerException: If there was an error accessing the API.
+        """
+        circuit_1 = rho_1[0]
+        circuit_2 = rho_2[0]
+        target_1 = self._resolve_target(rho_1[1])
+        target_2 = self._resolve_target(rho_2[1])
+
+        css.validation.validate_cirq_circuits(circuit_1)
+        css.validation.validate_cirq_circuits(circuit_2)
+
+        if not (isinstance(circuit_1, cirq.Circuit) and isinstance(circuit_2, cirq.Circuit)):
+            raise ValueError("Each state `rho_i` should contain a single circuit.")
+
+        serialized_circuits_1 = css.serialization.serialize_circuits(circuit_1)
+        serialized_circuits_2 = css.serialization.serialize_circuits(circuit_2)
+
+        ids = self._client.submit_dfe(
+            circuit_1={"cirq_circuits": serialized_circuits_1},
+            target_1=target_1,
+            circuit_2={"cirq_circuits": serialized_circuits_2},
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
         """Returns information about device specified by `target`.
 
         Args:
             target: A string corresponding to a device.
 
         Returns:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/service_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/service_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -495,14 +495,41 @@
 
     service = css.Service(api_key="key", remote_host="http://example.com")
     with pytest.raises(ValueError):
         _ = service.qscout_compile(circuit, base_entangling_gate="yy")
 
 
 @mock.patch("requests.post")
+def test_qscout_compile_num_qubits(mock_post: mock.MagicMock) -> None:
+    q0 = cirq.LineQubit(0)
+    circuit = cirq.Circuit(cirq.measure(q0))
+    final_logical_to_physical = {q0: q0}
+
+    jaqal_program = ""
+
+    mock_post.return_value.json = lambda: {
+        "cirq_circuits": css.serialization.serialize_circuits(circuit),
+        "final_logical_to_physicals": cirq.to_json([list(final_logical_to_physical.items())]),
+        "jaqal_programs": [jaqal_program],
+    }
+
+    service = css.Service(api_key="key", remote_host="http://example.com")
+    out = service.qscout_compile(circuit, num_qubits=5)
+    assert out.circuit == circuit
+    assert out.final_logical_to_physical == final_logical_to_physical
+    assert out.jaqal_program == jaqal_program
+    mock_post.assert_called_once()
+    assert json.loads(mock_post.call_args.kwargs["json"]["options"]) == {
+        "mirror_swaps": False,
+        "base_entangling_gate": "xx",
+        "num_qubits": 5,
+    }
+
+
+@mock.patch("requests.post")
 def test_service_cq_compile_single(mock_post: mock.MagicMock) -> None:
 
     q0 = cirq.LineQubit(0)
     circuit = cirq.Circuit(cirq.H(q0), cirq.measure(q0))
     final_logical_to_physical = {cirq.q(10): cirq.q(0)}
 
     mock_post.return_value.json = lambda: {
@@ -559,14 +586,38 @@
         "cirq_circuits": css.serialization.serialize_circuits(circuits),
         "fidelities": gss.serialization.serialize(fidelities),
     }
     assert service.supercheq([[0]], 1, 1) == (circuits, fidelities)
 
 
 @mock.patch("requests.post")
+def test_service_dfe(mock_post: mock.MagicMock) -> None:
+    service = css.Service(api_key="key", remote_host="http://example.com")
+    circuit = cirq.Circuit(cirq.X(cirq.q(0)))
+    mock_post.return_value.json = lambda: ["id1", "id2"]
+    assert service.submit_dfe(
+        rho_1=(circuit, "ss_example_qpu"),
+        rho_2=(circuit, "ss_example_qpu"),
+        num_random_bases=5,
+        shots=100,
+    ) == ["id1", "id2"]
+
+    with pytest.raises(ValueError, match="should contain a single circuit"):
+        service.submit_dfe(
+            rho_1=([circuit, circuit], "ss_example_qpu"),  # type: ignore # for testing
+            rho_2=(circuit, "ss_example_qpu"),
+            num_random_bases=5,
+            shots=100,
+        )
+
+    mock_post.return_value.json = lambda: 1
+    assert service.process_dfe(["1", "2"]) == 1
+
+
+@mock.patch("requests.post")
 def test_service_target_info(mock_post: mock.MagicMock) -> None:
     fake_data = {"target_info": {"backend_name": "ss_example_qpu", "max_experiments": 1234}}
     mock_post.return_value.json = lambda: fake_data
     service = css.Service(api_key="key", remote_host="http://example.com")
     assert service.target_info("ss_example_qpu") == fake_data["target_info"]
```

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/validation.py` & `cirq-superstaq-0.4.8/cirq_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq/validation_test.py` & `cirq-superstaq-0.4.8/cirq_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq.egg-info/PKG-INFO` & `cirq-superstaq-0.4.8/cirq_superstaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirq-superstaq
-Version: 0.4.7
+Version: 0.4.8
 Summary: The Cirq module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `cirq-superstaq-0.4.7/cirq_superstaq.egg-info/SOURCES.txt` & `cirq-superstaq-0.4.8/cirq_superstaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cirq-superstaq-0.4.7/pyproject.toml` & `cirq-superstaq-0.4.8/pyproject.toml`

 * *Files identical despite different names*

