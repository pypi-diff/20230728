# Comparing `tmp/hi-ml-azure-0.3.2.tar.gz` & `tmp/hi-ml-azure-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hi-ml-azure-0.3.2.tar", last modified: Thu Jul 20 05:23:40 2023, max compression
+gzip compressed data, was "dist/hi-ml-azure-0.3.4.tar", last modified: Fri Jul 28 09:33:38 2023, max compression
```

## Comparing `hi-ml-azure-0.3.2.tar` & `hi-ml-azure-0.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/package_description.md
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/run_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/src/health_azure/
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/amulet.py
--rw-r--r--   0 runner    (1001) docker     (122)    20546 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/argparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)    28663 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/src/health_azure/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/examples/elevate_this.py
--rw-r--r--   0 runner    (1001) docker     (122)    60858 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/himl.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1939 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/himl_download.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5570 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/himl_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     5486 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/mlflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/package_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2884 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)    11400 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/traverse.py
--rw-r--r--   0 runner    (1001) docker     (122)    96986 2023-07-20 05:23:23.000000 hi-ml-azure-0.3.2/src/health_azure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-07-20 05:23:39.000000 hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-20 05:23:40.000000 hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 05:23:39.000000 hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-20 05:23:39.000000 hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-20 05:23:39.000000 hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-20 05:23:39.000000 hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/package_description.md
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/run_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/health_azure/
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/amulet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20546 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28663 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/health_azure/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/examples/elevate_this.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61699 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/himl.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1939 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/himl_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5570 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/himl_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5486 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/mlflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2884 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11400 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    96986 2023-07-28 09:33:23.000000 hi-ml-azure-0.3.4/src/health_azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-28 09:33:38.000000 hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/top_level.txt
```

### Comparing `hi-ml-azure-0.3.2/LICENSE` & `hi-ml-azure-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/PKG-INFO` & `hi-ml-azure-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.3.2
+Version: 0.3.4
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Azure Toolbox
```

### Comparing `hi-ml-azure-0.3.2/package_description.md` & `hi-ml-azure-0.3.4/package_description.md`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/setup.py` & `hi-ml-azure-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/__init__.py` & `hi-ml-azure-0.3.4/src/health_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/amulet.py` & `hi-ml-azure-0.3.4/src/health_azure/amulet.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/argparsing.py` & `hi-ml-azure-0.3.4/src/health_azure/argparsing.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/datasets.py` & `hi-ml-azure-0.3.4/src/health_azure/datasets.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/examples/elevate_this.py` & `hi-ml-azure-0.3.4/src/health_azure/examples/elevate_this.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/himl.py` & `hi-ml-azure-0.3.4/src/health_azure/himl.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
 from azure.ai.ml import Input, MLClient, Output, command
 from azure.ai.ml.constants import InputOutputModes
 from azure.ai.ml.entities import Command, Data
 from azure.ai.ml.entities import Environment as EnvironmentV2
 from azure.ai.ml.entities import Job, Sweep, UserIdentityConfiguration
-from azure.ai.ml.entities._job.distribution import MpiDistribution, PyTorchDistribution
+from azure.ai.ml.entities._job.distribution import DistributionConfiguration, MpiDistribution, PyTorchDistribution
 from azure.ai.ml.sweep import Choice
 from azureml._base_sdk_common import user_agent
 from azureml.core import ComputeTarget, Environment, Experiment, Run, RunConfiguration, ScriptRunConfig, Workspace
 from azureml.core.runconfig import DockerConfiguration, MpiConfiguration
 from azureml.data import OutputFileDatasetConfig
 from azureml.data.dataset_consumption_config import DatasetConsumptionConfig
 from azureml.dataprep.fuse.daemon import MountContext
@@ -423,14 +423,15 @@
     tags: Optional[Dict[str, str]] = None,
     docker_shm_size: str = "",
     wait_for_completion: bool = False,
     identity_based_auth: bool = False,
     hyperparam_args: Optional[Dict[str, Any]] = None,
     num_nodes: int = 1,
     pytorch_processes_per_node: Optional[int] = None,
+    use_mpi_run_for_single_node_jobs: bool = True,
     display_name: Optional[str] = None,
 ) -> Job:
     """
     Starts a v2 AML Job on a given workspace by submitting a command
 
     :param ml_client: An Azure MLClient object for interacting with Azure resources.
     :param environment: An AML v2 Environment object.
@@ -450,14 +451,16 @@
     :param wait_for_completion: If False (the default) return after the run is submitted to AzureML, otherwise wait for
         the completion of this run (if True).
     :param hyperparam_args: A dictionary of hyperparameter search args to pass into a sweep job.
     :param num_nodes: The number of nodes to use for the job in AzureML. The value must be 1 or greater.
     :param pytorch_processes_per_node: For plain PyTorch multi-GPU processing: The number of processes per node.
         If supplied, it will run a command job with the "pytorch" framework (rather than "Python"), and using "nccl"
         as the communication backend.
+    :param use_mpi_run_for_single_node_jobs: If True, even single node jobs will be run as distributed MPI jobs.
+        This is required for Kubernetes compute. If False, single node jobs will not be run as distributed jobs.
     :param display_name: The name for the run that will be displayed in the AML UI. If not provided, a random
         display name will be generated by AzureML.
     :return: An AzureML Run object.
     """
     snapshot_root_directory = snapshot_root_directory or Path.cwd()
     root_dir = Path(snapshot_root_directory)
 
@@ -480,19 +483,21 @@
         raise ValueError("num_nodes must be >= 1")
     num_nodes = num_nodes if num_nodes >= 1 else 1
     if pytorch_processes_per_node is not None:
         if pytorch_processes_per_node < 1:
             raise ValueError("pytorch_processes_per_node must be >= 1")
 
     def create_command_job(cmd: str) -> Command:
+        distribution: Optional[DistributionConfiguration] = None
         if pytorch_processes_per_node is None:
             # On AML managed compute, we can set distribution to None for single node jobs.
             # However, on Kubernetes compute, single node jobs don't see any GPUs. GPUs are visible for MpiDistribution
             # jobs, so we set MpiDistribution even for single node jobs.
-            distribution: Union[MpiDistribution, PyTorchDistribution] = MpiDistribution(process_count_per_instance=1)
+            if use_mpi_run_for_single_node_jobs:
+                distribution = MpiDistribution(process_count_per_instance=1)
         else:
             distribution = PyTorchDistribution(process_count_per_instance=pytorch_processes_per_node)
         return command(
             code=str(snapshot_root_directory),
             command=cmd,
             inputs=input_datasets_v2,
             outputs=output_datasets_v2,
@@ -741,14 +746,15 @@
     tags: Optional[Dict[str, str]] = None,
     after_submission: Optional[Union[Callable[[Run], None], Callable[[Job, MLClient], None]]] = None,
     hyperdrive_config: Optional[HyperDriveConfig] = None,
     hyperparam_args: Optional[Dict[str, Any]] = None,
     strictly_aml_v1: bool = False,
     identity_based_auth: bool = False,
     pytorch_processes_per_node_v2: Optional[int] = None,
+    use_mpi_run_for_single_node_jobs: bool = True,
     display_name: Optional[str] = None,
 ) -> AzureRunInfo:  # pragma: no cover
     """
     Submit a folder to Azure, if needed and run it.
     Use the commandline flag --azureml to submit to AzureML, and leave it out to run locally.
 
     :param after_submission: A function that will be called directly after submitting the job to AzureML.
@@ -809,14 +815,17 @@
         for local execution (i.e., return immediately) will be executed. If not provided (None), submission to AzureML
         will be triggered if the commandline flag '--azureml' is present in sys.argv
     :param hyperdrive_config: A configuration object for Hyperdrive (hyperparameter search).
     :param strictly_aml_v1: If True, use Azure ML SDK v1. Otherwise, attempt to use Azure ML SDK v2.
     :param pytorch_processes_per_node_v2: For plain PyTorch multi-GPU processing: The number of processes per node. This
         is only supported with AML SDK v2, and ignored in v1. If supplied, the job will be submitted as using the
         "pytorch" framework (rather than "Python"), and using "nccl" as the communication backend.
+    :param use_mpi_run_for_single_node_jobs: If True, even single node jobs with SDK v2 will be run as distributed MPI
+        jobs. This is required for Kubernetes compute. If False, single node jobs will not be run as distributed jobs.
+        This setting only affects jobs submitted with SDK v2 (when `strictly_aml_v1=False`)
     :param display_name: The name for the run that will be displayed in the AML UI. If not provided, a random
         display name will be generated by AzureML.
     :return: If the script is submitted to AzureML then we terminate python as the script should be executed in AzureML,
         otherwise we return a AzureRunInfo object.
     """
     health_azure_package_setup()
     workspace_config_path = _str_to_path(workspace_config_file)
@@ -977,14 +986,15 @@
                 display_name=display_name,
                 docker_shm_size=docker_shm_size,
                 wait_for_completion=wait_for_completion,
                 identity_based_auth=identity_based_auth,
                 hyperparam_args=hyperparam_args,
                 num_nodes=num_nodes,
                 pytorch_processes_per_node=pytorch_processes_per_node_v2,
+                use_mpi_run_for_single_node_jobs=use_mpi_run_for_single_node_jobs,
             )
 
             if after_submission is not None:
                 after_submission(job, ml_client)  # type: ignore
 
     exit(0)
```

### Comparing `hi-ml-azure-0.3.2/src/health_azure/himl_download.py` & `hi-ml-azure-0.3.4/src/health_azure/himl_download.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/himl_tensorboard.py` & `hi-ml-azure-0.3.4/src/health_azure/himl_tensorboard.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/logging.py` & `hi-ml-azure-0.3.4/src/health_azure/logging.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/mlflow_utils.py` & `hi-ml-azure-0.3.4/src/health_azure/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/package_setup.py` & `hi-ml-azure-0.3.4/src/health_azure/package_setup.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/paths.py` & `hi-ml-azure-0.3.4/src/health_azure/paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/traverse.py` & `hi-ml-azure-0.3.4/src/health_azure/traverse.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/health_azure/utils.py` & `hi-ml-azure-0.3.4/src/health_azure/utils.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/PKG-INFO` & `hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.3.2
+Version: 0.3.4
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Azure Toolbox
```

### Comparing `hi-ml-azure-0.3.2/src/hi_ml_azure.egg-info/SOURCES.txt` & `hi-ml-azure-0.3.4/src/hi_ml_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

