# Comparing `tmp/pysiml-0.2.9.dev202307040514-py3-none-any.whl.zip` & `tmp/pysiml-0.2.9.dev202307281731-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 178872 bytes, number of entries: 147
+Zip file size: 179413 bytes, number of entries: 147
 -rw-r--r--  2.0 unx     1520 b- defN 80-Jan-01 00:00 pyproject.toml
 -rw-r--r--  2.0 unx      638 b- defN 80-Jan-01 00:00 siml/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 siml/__main__/__init__.py
 -rw-r--r--  2.0 unx      900 b- defN 80-Jan-01 00:00 siml/__main__/convert_interim_data.py
 -rw-r--r--  2.0 unx     1400 b- defN 80-Jan-01 00:00 siml/__main__/convert_raw_data.py
 -rw-r--r--  2.0 unx     1742 b- defN 80-Jan-01 00:00 siml/__main__/optimize.py
 -rw-r--r--  2.0 unx     8663 b- defN 80-Jan-01 00:00 siml/__main__/plot_losses.py
@@ -12,15 +12,15 @@
 -rw-r--r--  2.0 unx     3961 b- defN 80-Jan-01 00:00 siml/__main__/visualize_graph.py
 -rw-r--r--  2.0 unx      139 b- defN 80-Jan-01 00:00 siml/base/siml_const.py
 -rw-r--r--  2.0 unx      579 b- defN 80-Jan-01 00:00 siml/base/siml_enums.py
 -rw-r--r--  2.0 unx      228 b- defN 80-Jan-01 00:00 siml/base/siml_typing.py
 -rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 siml/config.py
 -rw-r--r--  2.0 unx     3520 b- defN 80-Jan-01 00:00 siml/data_parallel.py
 -rw-r--r--  2.0 unx    26513 b- defN 80-Jan-01 00:00 siml/datasets.py
--rw-r--r--  2.0 unx    28758 b- defN 80-Jan-01 00:00 siml/inferer.py
+-rw-r--r--  2.0 unx    29033 b- defN 80-Jan-01 00:00 siml/inferer.py
 -rw-r--r--  2.0 unx       84 b- defN 80-Jan-01 00:00 siml/loss_operations/__init__.py
 -rw-r--r--  2.0 unx     1463 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_assignment.py
 -rw-r--r--  2.0 unx     4057 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_calculator.py
 -rw-r--r--  2.0 unx     1960 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_calculator_builder.py
 -rw-r--r--  2.0 unx     2045 b- defN 80-Jan-01 00:00 siml/loss_operations/loss_selector.py
 -rw-r--r--  2.0 unx     1364 b- defN 80-Jan-01 00:00 siml/mains.py
 -rw-r--r--  2.0 unx     2724 b- defN 80-Jan-01 00:00 siml/networks/__init__.py
@@ -96,54 +96,54 @@
 -rw-r--r--  2.0 unx      570 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/standard_scaler.py
 -rw-r--r--  2.0 unx      865 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scale_functions/user_defined_scaler.py
 -rw-r--r--  2.0 unx     1012 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_result_save.py
 -rw-r--r--  2.0 unx     4367 b- defN 80-Jan-01 00:00 siml/preprocessing/siml_scalers/scaler_wrapper.py
 -rw-r--r--  2.0 unx      154 b- defN 80-Jan-01 00:00 siml/services/__init__.py
 -rw-r--r--  2.0 unx     2342 b- defN 80-Jan-01 00:00 siml/services/environment.py
 -rw-r--r--  2.0 unx      279 b- defN 80-Jan-01 00:00 siml/services/inference/__init__.py
--rw-r--r--  2.0 unx     2587 b- defN 80-Jan-01 00:00 siml/services/inference/core_inferer.py
+-rw-r--r--  2.0 unx     2600 b- defN 80-Jan-01 00:00 siml/services/inference/core_inferer.py
 -rw-r--r--  2.0 unx     1818 b- defN 80-Jan-01 00:00 siml/services/inference/data_loader_builder.py
--rw-r--r--  2.0 unx     2619 b- defN 80-Jan-01 00:00 siml/services/inference/engine_builder.py
+-rw-r--r--  2.0 unx     2632 b- defN 80-Jan-01 00:00 siml/services/inference/engine_builder.py
 -rw-r--r--  2.0 unx     5750 b- defN 80-Jan-01 00:00 siml/services/inference/inner_setting.py
 -rw-r--r--  2.0 unx     4710 b- defN 80-Jan-01 00:00 siml/services/inference/metrics_builder.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/__init__.py
 -rw-r--r--  2.0 unx     5603 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/post_fem_data.py
 -rw-r--r--  2.0 unx     4979 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/postprocessor.py
 -rw-r--r--  2.0 unx     7052 b- defN 80-Jan-01 00:00 siml/services/inference/postprocessing/save_processor.py
 -rw-r--r--  2.0 unx     1082 b- defN 80-Jan-01 00:00 siml/services/inference/record_object.py
 -rw-r--r--  2.0 unx     3161 b- defN 80-Jan-01 00:00 siml/services/model_builder.py
 -rw-r--r--  2.0 unx     4978 b- defN 80-Jan-01 00:00 siml/services/model_selector.py
 -rw-r--r--  2.0 unx     7124 b- defN 80-Jan-01 00:00 siml/services/path_rules.py
 -rw-r--r--  2.0 unx      200 b- defN 80-Jan-01 00:00 siml/services/training/__init__.py
--rw-r--r--  2.0 unx     7389 b- defN 80-Jan-01 00:00 siml/services/training/data_loader_builder.py
--rw-r--r--  2.0 unx     7993 b- defN 80-Jan-01 00:00 siml/services/training/engine_builder.py
--rw-r--r--  2.0 unx     7134 b- defN 80-Jan-01 00:00 siml/services/training/events_assigners.py
--rw-r--r--  2.0 unx     3084 b- defN 80-Jan-01 00:00 siml/services/training/inner_settings.py
+-rw-r--r--  2.0 unx     7425 b- defN 80-Jan-01 00:00 siml/services/training/data_loader_builder.py
+-rw-r--r--  2.0 unx     8310 b- defN 80-Jan-01 00:00 siml/services/training/engine_builder.py
+-rw-r--r--  2.0 unx     7443 b- defN 80-Jan-01 00:00 siml/services/training/events_assigners.py
+-rw-r--r--  2.0 unx     3215 b- defN 80-Jan-01 00:00 siml/services/training/inner_settings.py
 -rw-r--r--  2.0 unx      775 b- defN 80-Jan-01 00:00 siml/services/training/logging_items/__init__.py
 -rw-r--r--  2.0 unx     4198 b- defN 80-Jan-01 00:00 siml/services/training/logging_items/logging_items.py
 -rw-r--r--  2.0 unx     2729 b- defN 80-Jan-01 00:00 siml/services/training/tensor_spliter.py
--rw-r--r--  2.0 unx     9217 b- defN 80-Jan-01 00:00 siml/services/training/trainers_builder.py
--rw-r--r--  2.0 unx     6633 b- defN 80-Jan-01 00:00 siml/services/training/training_logger.py
--rw-r--r--  2.0 unx    52787 b- defN 80-Jan-01 00:00 siml/setting.py
+-rw-r--r--  2.0 unx     9402 b- defN 80-Jan-01 00:00 siml/services/training/trainers_builder.py
+-rw-r--r--  2.0 unx     7429 b- defN 80-Jan-01 00:00 siml/services/training/training_logger.py
+-rw-r--r--  2.0 unx    52855 b- defN 80-Jan-01 00:00 siml/setting.py
 -rw-r--r--  2.0 unx      163 b- defN 80-Jan-01 00:00 siml/siml_variables/__init__.py
 -rw-r--r--  2.0 unx      594 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/__init__.py
 -rw-r--r--  2.0 unx     1573 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/interface_wrapper.py
 -rw-r--r--  2.0 unx     1398 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/ndarray_wrapper.py
 -rw-r--r--  2.0 unx     1809 b- defN 80-Jan-01 00:00 siml/siml_variables/array_variables/sparce_array_wrapper.py
 -rw-r--r--  2.0 unx     4156 b- defN 80-Jan-01 00:00 siml/siml_variables/tensor_variables/tensor_variables.py
 -rw-r--r--  2.0 unx    12967 b- defN 80-Jan-01 00:00 siml/study.py
--rw-r--r--  2.0 unx    10653 b- defN 80-Jan-01 00:00 siml/trainer.py
+-rw-r--r--  2.0 unx    11300 b- defN 80-Jan-01 00:00 siml/trainer.py
 -rw-r--r--  2.0 unx      211 b- defN 80-Jan-01 00:00 siml/update_functions/__init__.py
 -rw-r--r--  2.0 unx     1774 b- defN 80-Jan-01 00:00 siml/update_functions/element_batch_update.py
 -rw-r--r--  2.0 unx     3623 b- defN 80-Jan-01 00:00 siml/update_functions/pseudo_batch_update.py
 -rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 siml/update_functions/standard_update.py
 -rw-r--r--  2.0 unx      429 b- defN 80-Jan-01 00:00 siml/update_functions/update_interface.py
 -rw-r--r--  2.0 unx    23027 b- defN 80-Jan-01 00:00 siml/util.py
 -rw-r--r--  2.0 unx       37 b- defN 80-Jan-01 00:00 siml/utils/__init__.py
 -rw-r--r--  2.0 unx     7682 b- defN 80-Jan-01 00:00 siml/utils/fem_data_utils.py
 -rw-r--r--  2.0 unx     1247 b- defN 80-Jan-01 00:00 siml/utils/timer.py
--rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/LICENSE
--rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/WHEEL
--rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx    13463 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202307040514.dist-info/RECORD
-147 files, 627155 bytes uncompressed, 157342 bytes compressed:  74.9%
+-rw-r--r--  2.0 unx    11431 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307281731.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1638 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307281731.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307281731.dist-info/WHEEL
+-rw-r--r--  2.0 unx      388 b- defN 80-Jan-01 00:00 pysiml-0.2.9.dev202307281731.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx    13463 b- defN 16-Jan-01 00:00 pysiml-0.2.9.dev202307281731.dist-info/RECORD
+147 files, 629945 bytes uncompressed, 157883 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -420,23 +420,23 @@
 
 Filename: siml/utils/fem_data_utils.py
 Comment: 
 
 Filename: siml/utils/timer.py
 Comment: 
 
-Filename: pysiml-0.2.9.dev202307040514.dist-info/LICENSE
+Filename: pysiml-0.2.9.dev202307281731.dist-info/LICENSE
 Comment: 
 
-Filename: pysiml-0.2.9.dev202307040514.dist-info/METADATA
+Filename: pysiml-0.2.9.dev202307281731.dist-info/METADATA
 Comment: 
 
-Filename: pysiml-0.2.9.dev202307040514.dist-info/WHEEL
+Filename: pysiml-0.2.9.dev202307281731.dist-info/WHEEL
 Comment: 
 
-Filename: pysiml-0.2.9.dev202307040514.dist-info/entry_points.txt
+Filename: pysiml-0.2.9.dev202307281731.dist-info/entry_points.txt
 Comment: 
 
-Filename: pysiml-0.2.9.dev202307040514.dist-info/RECORD
+Filename: pysiml-0.2.9.dev202307281731.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyproject.toml

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysiml"
-version = "0.2.9.dev202307040514"
+version = "0.2.9.dev202307281731"
 description = "SiML - a Simulation ML library"
 license = "Apache-2.0"
 authors = ["RICOS Co. Ltd."]
 readme = "README.md"
 repository = "https://github.com/ricosjp/pysiml"
 documentation = "https://ricosjp.github.io/pysiml/"
 packages = [
```

## siml/inferer.py

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
+
 import pathlib
 from typing import Callable, Optional, Union
 
+import femio
 import numpy as np
+from ignite.engine import State
 from torch import Tensor
 from torch.utils.data import DataLoader
-import femio
-from ignite.engine import State
 
 from siml import datasets, setting
 from siml.base.siml_const import SimlConstItems
 from siml.loss_operations import LossCalculatorBuilder
 from siml.path_like_objects import SimlDirectory, SimlFileBuilder
 from siml.preprocessing import ScalersComposition
-from siml.preprocessing.converter import (
-    ILoadFunction, IConvertFunction, RawConverter)
-from siml.services import ModelEnvironmentSetting, ModelSelectorBuilder
-from siml.services.inference import (
-    CoreInferer, InferenceDataLoaderBuilder, InnerInfererSetting,
-    PredictionRecord, PostPredictionRecord
-)
-from siml.services.inference.postprocessing import (
-    IInfererSaveFunction, SaveProcessor, PostProcessor,
-    PostFEMDataConverter, IFEMDataAdditionFunction
-)
+from siml.preprocessing.converter import (IConvertFunction, ILoadFunction,
+                                          RawConverter)
+from siml.services import ModelSelectorBuilder
+from siml.services.inference import (CoreInferer, InferenceDataLoaderBuilder,
+                                     InnerInfererSetting, PostPredictionRecord,
+                                     PredictionRecord)
+from siml.services.inference.postprocessing import (IFEMDataAdditionFunction,
+                                                    IInfererSaveFunction,
+                                                    PostFEMDataConverter,
+                                                    PostProcessor,
+                                                    SaveProcessor)
 
 
 class WholeInferProcessor:
     def __init__(
         self,
         main_setting: setting.MainSetting,
         model_path: Optional[pathlib.Path] = None,
```

## siml/services/inference/core_inferer.py

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Optional
 import pathlib
 
 from ignite.engine import Engine, State
 from torch.utils.data import DataLoader
 
 from siml import networks, setting
-from siml.inferer import ModelEnvironmentSetting
+from siml.services.environment import ModelEnvironmentSetting
 from siml.loss_operations import ILossCalculator
 from siml.services.model_builder import ModelBuilder
 
 from .engine_builder import InferenceEngineBuilder
 from .metrics_builder import MetricsBuilder
 from .postprocessing import PostProcessor
```

## siml/services/inference/engine_builder.py

```diff
@@ -2,15 +2,15 @@
 import time
 
 import torch
 from ignite.engine import Engine
 
 from siml import networks, util
 from siml.siml_variables import siml_tensor_variables
-from siml.inferer import ModelEnvironmentSetting
+from siml.services.environment import ModelEnvironmentSetting
 
 from .record_object import RawPredictionRecord
 from .postprocessing import PostProcessor
 
 
 class InferenceEngineBuilder:
     def __init__(
```

## siml/services/training/data_loader_builder.py

```diff
@@ -129,15 +129,15 @@
         random_generator.manual_seed(self._trainer_setting.seed)
 
         print(f"num_workers for data_loader: {num_workers}")
         train_loader = DataLoader(
             train_dataset,
             collate_fn=self._collate_fn,
             batch_size=batch_size,
-            shuffle=True,
+            shuffle=self._trainer_setting.train_data_shuffle,
             num_workers=num_workers,
             worker_init_fn=self._seed_worker,
             generator=random_generator
         )
         validation_loader = DataLoader(
             validation_dataset,
             collate_fn=self._collate_fn,
@@ -161,16 +161,16 @@
             train_loader,
             self._trainer_setting.input_names_list
         )
 
         self._check_data_dimension(
             train_loader,
             self._trainer_setting.output_names_list
-
         )
+
         return train_loader, validation_loader, test_loader
 
     def _seed_worker(worker_id) -> None:
         worker_seed = torch.initial_seed() % 2**32
         np.random.seed(worker_seed)
         random.seed(worker_seed)
```

## siml/services/training/engine_builder.py

```diff
@@ -1,35 +1,38 @@
-from typing import Callable, Union
+from typing import Callable, Optional, Union
 
 import ignite
-from ignite.engine import Engine
 import numpy as np
 import torch
 import yaml
+from ignite.engine import Engine
 
 from siml import util
 from siml.loss_operations import ILossCalculator
 from siml.networks import Network
 from siml.services.environment import ModelEnvironmentSetting
+from siml.services.training.tensor_spliter import TensorSpliter
+from siml.services.training.training_logger import TrainDataDebugLogger
 from siml.setting import TrainerSetting
 from siml.siml_variables import siml_tensor_variables
 from siml.update_functions import IStepUpdateFunction
-from siml.services.training.tensor_spliter import TensorSpliter
 
 
 class TrainerEngineBuilder:
     def __init__(
         self,
         env_setting: ModelEnvironmentSetting,
         prepare_batch_function: Callable,
-        trainer_setting: TrainerSetting
+        trainer_setting: TrainerSetting,
+        debug_logger: Optional[TrainDataDebugLogger] = None
     ) -> None:
         self._env_setting = env_setting
         self._prepare_batch_func = prepare_batch_function
         self._trainer_setting = trainer_setting
+        self._debug_logger = debug_logger
 
     def create_supervised_trainer(
         self,
         model: Network,
         optimizer: torch.optim.Optimizer,
         update_function: IStepUpdateFunction
     ) -> Engine:
@@ -65,14 +68,18 @@
                 output_device=output_device,
                 support_device=support_device,
                 non_blocking=self._trainer_setting.non_blocking
             )
             loss = update_function(x, y, model, optimizer)
             if self._trainer_setting.output_stats:
                 self.output_stats(model, engine)
+
+            if self._trainer_setting.debug_dataset:
+                self._debug_logger.write(batch.get("data_directories", None))
+
             return loss
 
         return Engine(update_model)
 
     def output_stats(
         self,
         model: Network,
```

## siml/services/training/events_assigners.py

```diff
@@ -1,20 +1,22 @@
 import enum
+from typing import Optional
 
 import numpy as np
 import optuna
 from ignite.engine import Engine, Events
 from ignite.handlers import EarlyStopping
 from torch.utils.data import DataLoader
 from torch.optim import Optimizer
 from tqdm import tqdm
 
 from siml.networks import Network
 from siml.services.training import (LogRecordItems, SimlTrainingConsoleLogger,
                                     SimlTrainingFileLogger)
+from siml.services.training.training_logger import TrainDataDebugLogger
 from siml.setting import TrainerSetting
 from siml.utils.timer import SimlStopWatch
 
 
 # Add early stopping
 class StopTriggerEvents(enum.Enum):
     EVALUATED = 'evaluated'
@@ -27,25 +29,27 @@
         file_logger: SimlTrainingFileLogger,
         console_logger: SimlTrainingConsoleLogger,
         train_loader: DataLoader,
         validation_loader: DataLoader,
         evaluator: Engine,
         model: Network,
         optimizer: Optimizer,
-        timer: SimlStopWatch
+        timer: SimlStopWatch,
+        debug_logger: Optional[TrainDataDebugLogger] = None
     ) -> None:
         self._file_logger = file_logger
         self._console_logger = console_logger
         self._evaluator = evaluator
         self._train_loader = train_loader
         self._validation_loader = validation_loader
         self._model = model
         self._trainer_setting = trainer_setting
         self._timer = timer
         self._optimizer = optimizer
+        self._debug_logger = debug_logger
 
         self._desc: str = "loss: {:.5e}"
         self._trick = 1
         self._evaluator_tick = 1
 
         total = len(train_loader) + self._trainer_setting.log_trigger_epoch
         self._pbar = _create_pbar(total, self._desc.format(0))
@@ -111,14 +115,16 @@
             epoch=engine.state.epoch,
             model=self._model,
             optimizer=self._optimizer,
             validation_loss=validation_loss,
             trainer_setting=self._trainer_setting
         )
 
+        if self._debug_logger is not None:
+            self._debug_logger.write_epoch(engine.state.epoch)
         # Write log
         self._file_logger.write(log_record)
 
         # Plot
         self._file_logger.save_figure()
         return
```

## siml/services/training/inner_settings.py

```diff
@@ -32,14 +32,18 @@
         return self.main_setting.trainer
 
     @property
     def log_file_path(self):
         return self.trainer_setting.output_directory / 'log.csv'
 
     @property
+    def log_dataset_file_path(self):
+        return self.trainer_setting.output_directory / 'log_debug_dataset.txt'
+
+    @property
     def loss_figure_path(self):
         return self.trainer_setting.output_directory \
             / f"plot.{self.trainer_setting.figure_format}"
 
     def __post_init_post_parse__(self):
         self._check_restart_and_pretrain()
         if self.trainer_setting.restart_directory is not None:
```

## siml/services/training/trainers_builder.py

```diff
@@ -4,21 +4,22 @@
 from ignite.engine import Engine
 import torch
 from torch.optim import Optimizer
 
 from .tensor_spliter import TensorSpliter
 from siml import networks, setting
 from siml import update_functions
-from siml.inferer import ModelEnvironmentSetting
+from siml.services.environment import ModelEnvironmentSetting
 from siml.services.model_selector import ModelSelectorBuilder
 from siml.loss_operations import ILossCalculator
 from siml.services.model_builder import ModelBuilder
 from siml.services.training.engine_builder import (
     TrainerEngineBuilder, EvaluatorEngineBuilder
 )
+from siml.services.training.training_logger import TrainDataDebugLogger
 
 
 class UpdateFunctionSelector:
     def __init__(
         self,
         trainer_setting: setting.TrainerSetting,
         env_setting: ModelEnvironmentSetting,
@@ -92,15 +93,16 @@
     def __init__(
         self,
         trainer_setting: setting.TrainerSetting,
         model_setting: setting.ModelSetting,
         env_setting: ModelEnvironmentSetting,
         prepare_batch_function: Callable,
         loss_function: ILossCalculator,
-        decrypt_key: Optional[bytes] = None
+        decrypt_key: Optional[bytes] = None,
+        debug_logger: Optional[TrainDataDebugLogger] = None
     ) -> None:
 
         self._trainer_setting = trainer_setting
         self._model_setting = model_setting
         self._env_setting = env_setting
         self._prepare_batch_function = prepare_batch_function
         self._loss_function = loss_function
@@ -116,15 +118,16 @@
             loss_function=self._loss_function,
             spliter=self._spliter
         )
 
         self._trainer_builder = TrainerEngineBuilder(
             env_setting=self._env_setting,
             prepare_batch_function=self._prepare_batch_function,
-            trainer_setting=self._trainer_setting
+            trainer_setting=self._trainer_setting,
+            debug_logger=debug_logger
         )
         self._evaluator_builder = EvaluatorEngineBuilder(
             env_setting=self._env_setting,
             prepare_batch_function=self._prepare_batch_function,
             trainer_setting=self._trainer_setting,
             loss_function=self._loss_function,
             spliter=self._spliter
```

## siml/services/training/training_logger.py

```diff
@@ -1,8 +1,9 @@
 import pathlib
+from typing import Union
 
 import matplotlib.pyplot as plt
 import pandas as pd
 from torch.optim import Optimizer
 
 from siml.networks import Network
 from siml.path_like_objects import SimlFileBuilder
@@ -56,21 +57,25 @@
             'validation_loss',
             *[f"validation/{k}" for k in self._loss_keys],
             'elapsed_time'
         ]
         headers = [create_logitems(v) for v in headers]
         return headers
 
-    def output_header(self) -> str:
+    def get_header(self) -> str:
         strings = [
             v.format(padding_margin=self._display_margin)
             for v in self._headers
         ]
         return "\n" + "".join(strings)
 
+    def output_header(self) -> None:
+        header = self.get_header()
+        print(header)
+
     def output(self, log_record: LogRecordItems) -> str:
         strings = [
             log_record.epoch.format(padding_margin=self._display_margin),
             log_record.train_loss.format(
                 formatter=".5e", padding_margin=self._display_margin
             ),
             log_record.train_other_losses.format(
@@ -199,7 +204,30 @@
             'model_state_dict': model.state_dict(),
             'optimizer_state_dict': optimizer.state_dict()
         }
         siml_file.save(
             data,
             encrypt_key=trainer_setting.model_key
         )
+
+
+class TrainDataDebugLogger:
+    def __init__(self, file_path: pathlib.Path) -> None:
+        self._file_path = file_path
+
+    def _header_strings(self) -> list[str]:
+        return ["data_directory"]
+
+    def write_epoch(self, epoch: int):
+        with open(self._file_path, 'a') as fw:
+            fw.write(f"epoch: {epoch} finished ---------- \n")
+
+    def write(
+        self, data_directories: Union[list[pathlib.Path], None]
+    ) -> None:
+        if data_directories is None:
+            values = []
+        else:
+            values = [str(path) for path in data_directories]
+
+        with open(self._file_path, 'a') as fw:
+            fw.write(", ".join(values) + '\n')
```

## siml/setting.py

```diff
@@ -573,22 +573,24 @@
     clip_grad_value: float = dc.field(
         default=None, metadata={'allow_none': True})
     clip_grad_norm: float = dc.field(
         default=None, metadata={'allow_none': True})
     recursive: bool = True
     state_dict_strict: bool = True
 
+    train_data_shuffle: bool = True
     data_parallel: bool = False
     model_parallel: bool = False
     draw_network: bool = True
     output_stats: bool = False
     split_ratio: dict = dc.field(default_factory=dict)
     figure_format: str = 'pdf'
 
     pseudo_batch_size: int = 0
+    debug_dataset: bool = False
     time_series_split: list[int] = dc.field(
         default=None, metadata={'allow_none': True})
     time_series_split_evaluation: list[int] = dc.field(
         default=None, metadata={'allow_none': True})
     loss_slice: slice = dc.field(default_factory=lambda: slice(None))
 
     def __post_init__(self):
```

## siml/trainer.py

```diff
@@ -1,21 +1,22 @@
-from typing import Callable, Union
+from typing import Callable, Union, Optional
 
 import numpy as np
 from ignite.engine import Engine, State
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 
 from siml.loss_operations import LossCalculatorBuilder, ILossCalculator
 from siml.networks import Network
 from siml.services.environment import ModelEnvironmentSetting
 from siml.services.training import (InnerTrainingSetting,
                                     SimlTrainingConsoleLogger,
                                     SimlTrainingFileLogger)
+from siml.services.training.training_logger import TrainDataDebugLogger
 from siml.services.training.data_loader_builder import DataLoaderBuilder
 from siml.services.training.events_assigners import (TrainerEventsAssigner,
                                                      ValidationEventsAssigner)
 from siml.services.training.trainers_builder import TrainersBuilder
 from siml.utils.timer import SimlStopWatch
 
 from . import datasets, setting, util
@@ -63,17 +64,19 @@
             collate_fn=self._collate_fn,
             decrypt_key=self.setting.get_crypt_key()
         )
         self._loss_calculator = LossCalculatorBuilder.create(
             trainer_setting=self.setting.trainer,
             user_loss_function_dic=self.user_loss_function_dic
         )
+        self._debug_logger = self._setup_debug_logger()
         self._trainers_builder = self._create_trainers_builder(
             prepare_batch=self._collate_fn.prepare_batch,
-            loss_calculator=self._loss_calculator
+            loss_calculator=self._loss_calculator,
+            debug_logger=self._debug_logger
         )
 
         # SET IN _initialize_state()
         self.train_loader: DataLoader = None
         self.validation_loader: DataLoader = None
         self.test_loader: DataLoader = None
         self._model: Network = None
@@ -118,15 +121,15 @@
             If True, evaluation by test dataset is performed, by default False
         load_best_model : bool, optional
             If True, best model is used to evaluate, by default False
 
         Returns
         -------
         tuple[State, Union[State, None], Union[State, None]]
-            ignite State objects for train, validation and test dataset 
+            ignite State objects for train, validation and test dataset
         """
 
         if load_best_model:
             self.setting.trainer.pretrain_directory \
                 = self.setting.trainer.output_directory
             self._initialize_state()
         train_state = self._evaluator.run(self.train_loader)
@@ -144,17 +147,16 @@
     def _initialize_state(self):
         # Initialize state
         self.train_loader, self.validation_loader, self.test_loader = \
             self._data_loader_builder.create()
         self._trainer, self._evaluator, self._model, self._optimizer =\
             self._trainers_builder.create(epoch_length=len(self.train_loader))
 
-        self._console_logger, self._file_logger = self._setup_loggers(
-            self._model
-        )
+        self._console_logger, self._file_logger \
+            = self._setup_loggers(self._model)
         self._stop_watch = self._setup_stopwatch(self._file_logger)
 
         # HACK: NEED to be called last
         self._assign_trainer_events(self._trainer)
         self._assign_evaluator_events(self._evaluator)
 
     def _prepare_files_and_dirs(self, draw_model: bool = True):
@@ -174,15 +176,15 @@
             self.setting,
             self.setting.trainer.output_directory / yaml_file_name,
             key=self.setting.trainer.model_key
         )
 
     def _run_training(self):
         # start logging
-        print(self._console_logger.output_header())
+        self._console_logger.output_header()
         self._file_logger.write_header_if_needed()
         self._stop_watch.start()
 
         self._trainer.run(
             self.train_loader,
             max_epochs=self.setting.trainer.n_epoch
         )
@@ -200,16 +202,25 @@
         )
         file_logger = SimlTrainingFileLogger(
             file_path=self._inner_setting.log_file_path,
             loss_figure_path=self._inner_setting.loss_figure_path,
             loss_keys=model.get_loss_keys(),
             continue_mode=self.setting.trainer.overwrite_restart_mode
         )
+
         return console_logger, file_logger
 
+    def _setup_debug_logger(self) -> Union[TrainDataDebugLogger, None]:
+        if self._inner_setting.trainer_setting.debug_dataset:
+            file_path = self._inner_setting.log_dataset_file_path
+            debug_logger = TrainDataDebugLogger(file_path)
+        else:
+            debug_logger = None
+        return debug_logger
+
     def _setup_stopwatch(self, file_logger: SimlTrainingFileLogger):
         time_offset = file_logger.read_offset_start_time()
         stop_watch = SimlStopWatch(offset=time_offset)
         return stop_watch
 
     def _assign_trainer_events(self, trainer: Engine) -> None:
         train_events = TrainerEventsAssigner(
@@ -217,15 +228,16 @@
             file_logger=self._file_logger,
             console_logger=self._console_logger,
             train_loader=self.train_loader,
             validation_loader=self.validation_loader,
             evaluator=self._evaluator,
             model=self._model,
             optimizer=self._optimizer,
-            timer=self._stop_watch
+            timer=self._stop_watch,
+            debug_logger=self._debug_logger
         )
         train_events.assign_handlers(trainer)
 
     def _assign_evaluator_events(self, evaluator: Engine) -> None:
         evaluator_events = ValidationEventsAssigner(
             file_logger=self._file_logger,
             console_logger=self._console_logger,
@@ -268,18 +280,20 @@
             output_time_slices=tr_setting.outputs.time_slice
         )
         return collate_fn
 
     def _create_trainers_builder(
         self,
         prepare_batch: Callable,
-        loss_calculator: ILossCalculator
+        loss_calculator: ILossCalculator,
+        debug_logger: Optional[TrainDataDebugLogger] = None
     ):
         trainers_builder = TrainersBuilder(
             trainer_setting=self.setting.trainer,
             model_setting=self.setting.model,
             env_setting=self._env_setting,
             prepare_batch_function=prepare_batch,
             loss_function=loss_calculator,
-            decrypt_key=self.setting.get_crypt_key()
+            decrypt_key=self.setting.get_crypt_key(),
+            debug_logger=debug_logger
         )
         return trainers_builder
```

## Comparing `pysiml-0.2.9.dev202307040514.dist-info/LICENSE` & `pysiml-0.2.9.dev202307281731.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pysiml-0.2.9.dev202307040514.dist-info/METADATA` & `pysiml-0.2.9.dev202307281731.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysiml
-Version: 0.2.9.dev202307040514
+Version: 0.2.9.dev202307281731
 Summary: SiML - a Simulation ML library
 Home-page: https://github.com/ricosjp/pysiml
 License: Apache-2.0
 Author: RICOS Co. Ltd.
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pysiml-0.2.9.dev202307040514.dist-info/RECORD` & `pysiml-0.2.9.dev202307281731.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyproject.toml,sha256=bUwTI0ASk1HRlyK_veOxzfJbzdgi9q8OonWAv7-BcD4,1520
+pyproject.toml,sha256=BFkhubvoWkQ54Ptjjfuw9rcE7FaRDYl1sHQX4ZtrZvw,1520
 siml/__init__.py,sha256=mC61oSLHO5F6zXHhOrzH51R-vkH0mL4MShhSBiRRe6s,638
 siml/__main__/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 siml/__main__/convert_interim_data.py,sha256=jA6GD7BlnsEjARcln3UBwXlFj64BeFALAmgD1ohBkqo,900
 siml/__main__/convert_raw_data.py,sha256=VNVOyx9lChopF2Q-9OXtN_-MtfBsyjS_JvFwCjdkv0c,1400
 siml/__main__/optimize.py,sha256=6HALn60Mxh4GUiPbSXjvrdpkoQ4NgYSzCHCBRbli4W0,1742
 siml/__main__/plot_losses.py,sha256=0uMsoPN-xR0JhPg0WzSQL5GbD80ovuFO12eVpc0x6Xc,8663
 siml/__main__/prepare_preprocess_converters.py,sha256=w_rzic--RUyISagQOJw_5-oEkOFEKXUN7G1TkTOxd8g,927
@@ -11,15 +11,15 @@
 siml/__main__/visualize_graph.py,sha256=xyPqVZHA0p3xnB41w4PsKCfy7feicBRMXZveQdo_lpM,3961
 siml/base/siml_const.py,sha256=XHUALl1xhy7YVorWj_weZ0FTfsoitJdFcfKGm-9C1L8,139
 siml/base/siml_enums.py,sha256=aR3INV-U399qmFQBrjnYvB2JRyQmkaqA9cETbsx4A2I,579
 siml/base/siml_typing.py,sha256=A0pQGeRPNQmS3Dd6qNq3umZkbHRrn1YwDb0Owlurweo,228
 siml/config.py,sha256=_Cc2w65g05Y5QDuh8b8UIY_XFZbwKmXx_Z40ATxVw_I,57
 siml/data_parallel.py,sha256=b4DU0QCVVbFWB02QdvtMLuLuTIz57npYSlbmKfJVjVo,3520
 siml/datasets.py,sha256=v1eVzPCWgCtsR-l5xqzL1ozlGOInYXgef6FoGXk218w,26513
-siml/inferer.py,sha256=0-EDtpc_pUS1yXhsSz6Zqts0Twd1ZJn4GNcEi-jadFI,28758
+siml/inferer.py,sha256=OA1AuJXE0laKqhUWaZuKP_ok4un0dK3PJ6RxZk5nXHo,29033
 siml/loss_operations/__init__.py,sha256=N1Hz-fJTL3e1MCeJt2QP99TDvbO9s6AlP_XzpdiBOpA,84
 siml/loss_operations/loss_assignment.py,sha256=Eyf7riWlLm4fMWFuqpmKJIAbd-fwIWdIK0sDgTCtcLQ,1463
 siml/loss_operations/loss_calculator.py,sha256=mac4Bo4Kb2B6pGDUBamTKEPk_cxo8xPtkG9ydwE4gqM,4057
 siml/loss_operations/loss_calculator_builder.py,sha256=VOXTFCPqIOAIbq37UNsc4N6OlWWs6IECXlLxl-hsCYU,1960
 siml/loss_operations/loss_selector.py,sha256=d-sTYDF6yIyNbwQwuwpEOoUaX45Wk-7f1vs4x_q7tH0,2045
 siml/mains.py,sha256=2Bah9LWn8YPmmXfianE-_nhl9581nUlgwDtA0xUy30o,1364
 siml/networks/__init__.py,sha256=8lF58NgkEeR1cl_h5fELLyIOMeYZUS-L4wWChGSMCH8,2724
@@ -95,53 +95,53 @@
 siml/preprocessing/siml_scalers/scale_functions/standard_scaler.py,sha256=qvyUGXXw4j60xGw0RwXUaHaYlnVZHR9XB_DFkayySBg,570
 siml/preprocessing/siml_scalers/scale_functions/user_defined_scaler.py,sha256=GFwX9UyJ6z9iTy8XiiJgvlv65W6dBRZ8bDLV2sECdTs,865
 siml/preprocessing/siml_scalers/scaler_result_save.py,sha256=9ZD7dibMlteAZvpePfsK5sEAhf4VMadAMclKJpypz54,1012
 siml/preprocessing/siml_scalers/scaler_wrapper.py,sha256=_YoFh6KXCS093l-CjMw8hxvy3pO0GxdMcwCj9uZwJ0o,4367
 siml/services/__init__.py,sha256=UfdYF0fGhc34bu7gPjTSCQgkD0Hnlaavx4AI5yc9iaA,154
 siml/services/environment.py,sha256=oi0GhoCxvI6HtIYPYa0D6JAh2RdD9Ao0jeeV2pVUykQ,2342
 siml/services/inference/__init__.py,sha256=bCltATxDFTamdw_d4jpVP68ZfKUpguExJsDqLUbzVgk,279
-siml/services/inference/core_inferer.py,sha256=EkfbyqjFwOL9G2jH-UMZuruDDFBeDgmtHa4R9Ae3GUk,2587
+siml/services/inference/core_inferer.py,sha256=bHSCJhQb01oReORPvY9dot37ksVYhfE_rpet5366rJA,2600
 siml/services/inference/data_loader_builder.py,sha256=5FhUabZ39P1yEODpM3pPduFLAyriyexB_qUHmPuJ7NU,1818
-siml/services/inference/engine_builder.py,sha256=y6K7J_nhK1-3f2Cj3vNQiNh4yzda79ury12RaCFBovE,2619
+siml/services/inference/engine_builder.py,sha256=BpEtMBQZYOdGFyAjeXWAdX2bpUsdkY9ZKy6EaOdm1Pw,2632
 siml/services/inference/inner_setting.py,sha256=sw3_Priovxo87tcfgBObvm6MY--1QAahM-KG4qz244M,5750
 siml/services/inference/metrics_builder.py,sha256=I8ORAOZO4Mf5b0AaPCfpdu0ieqx1peuKkW9Z9H8RaAY,4710
 siml/services/inference/postprocessing/__init__.py,sha256=txubVxvNDftzgw3M05LP2GPmwvvJZCZKJcU02q4iiqs,203
 siml/services/inference/postprocessing/post_fem_data.py,sha256=8apB2-cUyssum_6BOx9uVUhmNNvBjoXRnSWn4w4aJ-A,5603
 siml/services/inference/postprocessing/postprocessor.py,sha256=lnHod9-Wa87QLb4ZMq7cOOeRxFjKQYq4NeuPaTHD6Nk,4979
 siml/services/inference/postprocessing/save_processor.py,sha256=oJVxJJplyH8dLiYIpG1GJWD_Y58RwrnAwlqNt_dLuA0,7052
 siml/services/inference/record_object.py,sha256=9cSmtHyNuVwtQbAxkMoUOhCg7TQ6fgyFFwWqyBJ3Gw4,1082
 siml/services/model_builder.py,sha256=N1TH7yARLchn4ZuXQA9-hoGmqVUkHcPUU0D77Gc0kt0,3161
 siml/services/model_selector.py,sha256=q2oXdJcujaOa6Y_HFHZ1emxkNaRN00BAGi_kc0zXmvE,4978
 siml/services/path_rules.py,sha256=fPNdpXcf8GZtI6ZfMrEkKcdo0JkxxPNmnvohbY1evI8,7124
 siml/services/training/__init__.py,sha256=nuxgfAYieJxucFOKJXwdICJuyvUhHdKjup0okMU8ULk,200
-siml/services/training/data_loader_builder.py,sha256=pV5j63xz1zyss9HsGKQf20i_dE_t2-QecGDVaRc2gh4,7389
-siml/services/training/engine_builder.py,sha256=3zsc_B5Uk8BZOnDtOK3VEb9MmlS5S6PdTX3Qd-7IXH8,7993
-siml/services/training/events_assigners.py,sha256=bWyGoqWiyVkHXbRf3BNL0LQnbVexjUpcJDRq6BvqAGA,7134
-siml/services/training/inner_settings.py,sha256=bexDtmR5EECIXXjaYdR7NZ7phs-UYC6QL-wgu5epGDw,3084
+siml/services/training/data_loader_builder.py,sha256=2ALPbrVuYGLiF9NBCjVlCUlyrciOCKOTV731Z-gMzhQ,7425
+siml/services/training/engine_builder.py,sha256=M9BijQYVXbceA3ZDy52wRA8EIjrN0Gg5fQQXqo_cFAs,8310
+siml/services/training/events_assigners.py,sha256=MWuZNFeGa3ANn--dd5lIB3p2qGBOyVlHpgLMPbyDdW8,7443
+siml/services/training/inner_settings.py,sha256=LdRlYvE2J2OQAM72-XBXGfF2wsDPJcudzYVbjEQrCRM,3215
 siml/services/training/logging_items/__init__.py,sha256=1Njqc0eCpuwo6mzxDv2iRhhvslHG3yfH3oHnCgc3FMc,775
 siml/services/training/logging_items/logging_items.py,sha256=hQMvAImDg2YpHFY8qIj72ICZRW6pgNZ4qdZi4hll2kE,4198
 siml/services/training/tensor_spliter.py,sha256=pezCbe50ODgef-jjOYTVH-DERN3muv1OZuBq39fzbB4,2729
-siml/services/training/trainers_builder.py,sha256=4bcE_npNBCGzCQAq3K0a_MOgklnIOr59eqZtk0Oe4cA,9217
-siml/services/training/training_logger.py,sha256=C7hz_xCGzV9ms-kv3M67TnPK-wx-AQ8DcKVituJ5LwE,6633
-siml/setting.py,sha256=L3WsnrAo-Te420XxTpHSkVTEvTKv6C0WXXWO3dorJHM,52787
+siml/services/training/trainers_builder.py,sha256=_6tszYKDi1GCeSjeFZktNp6DTvs9XMRzjdeCYZiBA94,9402
+siml/services/training/training_logger.py,sha256=DverZ-3h1PdZRfZUSkT7UmNEXTUAuYJ1g3GbQkaHhRg,7429
+siml/setting.py,sha256=ifTwh7HFtrHe36nF7JjaljIvtoiTa34Ns3yMwYlQu04,52855
 siml/siml_variables/__init__.py,sha256=Nt8iJ0yLPBJpg1o6K_b5Qr-go5iurvC9FnHxI4lD6eg,163
 siml/siml_variables/array_variables/__init__.py,sha256=Y2syJXtd98L-Z3kRTCOlCEVZffc-xBbuMIS1uv3ekQU,594
 siml/siml_variables/array_variables/interface_wrapper.py,sha256=Wi0GcuEexwx6sqTqVcBCtWo2K7kw_LQN6LOdoXnNFYw,1573
 siml/siml_variables/array_variables/ndarray_wrapper.py,sha256=oNOfbQu_5twQZq9AM_NEWcbswnCzASAEGzCPpUXcujM,1398
 siml/siml_variables/array_variables/sparce_array_wrapper.py,sha256=yyWwfuKHn686-aQemDMIgcig4K9a6XC-HCTYETJS0O8,1809
 siml/siml_variables/tensor_variables/tensor_variables.py,sha256=Nh3W1ft6FbGID7cp88lw2VyVVxTkrx_1ovI_I2DFSX0,4156
 siml/study.py,sha256=Sc8DBdT3ni3mcHICtURUmjDslCkSf7T6lCqADogoRs4,12967
-siml/trainer.py,sha256=5GBxNYpDDfmxG_p6MkZxbZvFSDRMjSFo1EYqGF-kl6E,10653
+siml/trainer.py,sha256=C-NRHJGrDIUXFPNntsJEwWnh2LmsdDJ6ZVuCbi2ZoY4,11300
 siml/update_functions/__init__.py,sha256=fQY19xMEhZv7k6flZPBmhIgLl3uHuBWkay-YCFfaY64,211
 siml/update_functions/element_batch_update.py,sha256=93_L9jl4D9lFQXmEX1Lo8l4n3rDf1wdZljPJIQd9rUs,1774
 siml/update_functions/pseudo_batch_update.py,sha256=7PS6SEXOMB57uaJQhZ8VrtEiIkDF59JE1c6yyrKL3YY,3623
 siml/update_functions/standard_update.py,sha256=jIgeQ_c9R1dgcxDQWzx-w5TkJ7naDKmNi_WUFFchxc4,2702
 siml/update_functions/update_interface.py,sha256=O1fGrE21iXckz7NTOTDNlyQ4rll1SQDehdc_Kk5we0Q,429
 siml/util.py,sha256=AzvnYN1svE28ioHGPgMjkpiK35hCA5m5qwFEDb3agHA,23027
 siml/utils/__init__.py,sha256=DVdxWEBXfapWAWNM0jUouKJzru4RyK2ru2QheBmrm_s,37
 siml/utils/fem_data_utils.py,sha256=LDB_MxYPg_WELl6D_az9ikMZxAF5Ml5qKUXR2CnuxvE,7682
 siml/utils/timer.py,sha256=DEDtrmFpFqiGRykErkLMnwZ3tWUsOsarubnN40kwb6I,1247
-pysiml-0.2.9.dev202307040514.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
-pysiml-0.2.9.dev202307040514.dist-info/METADATA,sha256=f1L-eWRQgVtMOnG-7cShn_mR1rB3tH4b3OZYGrINIZ0,1638
-pysiml-0.2.9.dev202307040514.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-pysiml-0.2.9.dev202307040514.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
-pysiml-0.2.9.dev202307040514.dist-info/RECORD,,
+pysiml-0.2.9.dev202307281731.dist-info/LICENSE,sha256=Ok4O8jxCIpLhGZjTNzgBW8V8xITF_SUVEp1juLijZpA,11431
+pysiml-0.2.9.dev202307281731.dist-info/METADATA,sha256=vLGZlZCxNK1OqFeulJSWmIOs1aryjQ9RWx_SxMjwATE,1638
+pysiml-0.2.9.dev202307281731.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+pysiml-0.2.9.dev202307281731.dist-info/entry_points.txt,sha256=zXU0Gd56XeUfgaeG-CGXcYaTpORSU6kVeQ_vVvjIFPs,388
+pysiml-0.2.9.dev202307281731.dist-info/RECORD,,
```

