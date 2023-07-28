# Comparing `tmp/q1pulse-0.8.8.tar.gz` & `tmp/q1pulse-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\q1pulse-0.8.8.tar", last modified: Tue Jul 11 15:27:33 2023, max compression
+gzip compressed data, was "dist\q1pulse-0.9.1.tar", last modified: Fri Jul 28 13:45:15 2023, max compression
```

## Comparing `q1pulse-0.8.8.tar` & `q1pulse-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/
--rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.8.8/LICENSE
--rw-rw-rw-   0        0        0      193 2023-07-11 15:27:33.000000 q1pulse-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0    11766 2023-01-23 11:03:43.000000 q1pulse-0.8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/
--rw-rw-rw-   0        0        0      139 2023-07-11 15:27:10.000000 q1pulse-0.8.8/q1pulse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/assembler/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/assembler/__init__.py
--rw-rw-rw-   0        0        0    28695 2023-07-11 13:10:51.000000 q1pulse-0.8.8/q1pulse/assembler/generator.py
--rw-rw-rw-   0        0        0     1813 2023-07-11 13:10:59.000000 q1pulse-0.8.8/q1pulse/assembler/generator_data.py
--rw-rw-rw-   0        0        0     9745 2023-02-08 14:26:47.000000 q1pulse-0.8.8/q1pulse/assembler/instruction_queue.py
--rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.8.8/q1pulse/assembler/registers.py
--rw-rw-rw-   0        0        0    11312 2023-06-30 12:58:43.000000 q1pulse-0.8.8/q1pulse/instrument.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/lang/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/lang/__init__.py
--rw-rw-rw-   0        0        0      148 2021-11-28 16:59:16.000000 q1pulse-0.8.8/q1pulse/lang/base.py
--rw-rw-rw-   0        0        0     1478 2023-02-08 14:26:47.000000 q1pulse-0.8.8/q1pulse/lang/exceptions.py
--rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.8.8/q1pulse/lang/expression.py
--rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.8.8/q1pulse/lang/flow_statements.py
--rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.8.8/q1pulse/lang/generator.py
--rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.8.8/q1pulse/lang/loops.py
--rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.8.8/q1pulse/lang/math_expressions.py
--rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.8.8/q1pulse/lang/register.py
--rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.8.8/q1pulse/lang/register_statements.py
--rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.8.8/q1pulse/lang/registers.py
--rw-rw-rw-   0        0        0     2494 2021-12-14 14:34:49.000000 q1pulse-0.8.8/q1pulse/lang/sequence.py
--rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.8.8/q1pulse/lang/simulator_statements.py
--rw-rw-rw-   0        0        0     4557 2022-12-22 08:51:07.000000 q1pulse-0.8.8/q1pulse/lang/timed_statements.py
--rw-rw-rw-   0        0        0      994 2021-12-13 20:51:09.000000 q1pulse-0.8.8/q1pulse/lang/timeline.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/modules/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/modules/__init__.py
--rw-rw-rw-   0        0        0     8732 2023-06-30 11:37:00.000000 q1pulse-0.8.8/q1pulse/modules/modules.py
--rw-rw-rw-   0        0        0     2924 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/modules/sequencer_states.py
--rw-rw-rw-   0        0        0     5377 2022-12-19 08:32:38.000000 q1pulse-0.8.8/q1pulse/program.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/sequencer/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/sequencer/__init__.py
--rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.8.8/q1pulse/sequencer/builderbase.py
--rw-rw-rw-   0        0        0    14021 2023-06-30 11:37:00.000000 q1pulse-0.8.8/q1pulse/sequencer/control.py
--rw-rw-rw-   0        0        0     6224 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/sequencer/readout.py
--rw-rw-rw-   0        0        0     9429 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/sequencer/sequencer.py
--rw-rw-rw-   0        0        0     3395 2023-07-11 13:19:38.000000 q1pulse-0.8.8/q1pulse/sequencer/sequencer_data.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse/util/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.8/q1pulse/util/__init__.py
--rw-rw-rw-   0        0        0      543 2023-03-13 17:20:01.000000 q1pulse-0.8.8/q1pulse/util/qblox_version.py
-drwxrwxrwx   0        0        0        0 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse.egg-info/
--rw-rw-rw-   0        0        0      193 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-07-11 15:27:33.000000 q1pulse-0.8.8/q1pulse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 15:27:32.000000 q1pulse-0.8.8/q1pulse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-11 15:27:33.000000 q1pulse-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-07-11 15:27:10.000000 q1pulse-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/
+-rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-07-28 13:45:15.000000 q1pulse-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14959 2023-07-24 12:53:33.000000 q1pulse-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/
+-rw-rw-rw-   0        0        0      139 2023-07-28 13:45:07.000000 q1pulse-0.9.1/q1pulse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/assembler/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/assembler/__init__.py
+-rw-rw-rw-   0        0        0    31856 2023-07-26 15:23:50.000000 q1pulse-0.9.1/q1pulse/assembler/generator.py
+-rw-rw-rw-   0        0        0     1813 2023-07-11 13:10:59.000000 q1pulse-0.9.1/q1pulse/assembler/generator_data.py
+-rw-rw-rw-   0        0        0    10258 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/assembler/instruction_queue.py
+-rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.9.1/q1pulse/assembler/registers.py
+-rw-rw-rw-   0        0        0    12183 2023-07-27 12:31:40.000000 q1pulse-0.9.1/q1pulse/instrument.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/lang/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/lang/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-07-20 15:51:39.000000 q1pulse-0.9.1/q1pulse/lang/base.py
+-rw-rw-rw-   0        0        0     6677 2023-07-26 14:18:22.000000 q1pulse-0.9.1/q1pulse/lang/conditions.py
+-rw-rw-rw-   0        0        0     1575 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/exceptions.py
+-rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.9.1/q1pulse/lang/expression.py
+-rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.9.1/q1pulse/lang/flow_statements.py
+-rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.9.1/q1pulse/lang/generator.py
+-rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.9.1/q1pulse/lang/loops.py
+-rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.9.1/q1pulse/lang/math_expressions.py
+-rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.9.1/q1pulse/lang/register.py
+-rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.9.1/q1pulse/lang/register_statements.py
+-rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.9.1/q1pulse/lang/registers.py
+-rw-rw-rw-   0        0        0     2682 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/sequence.py
+-rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.9.1/q1pulse/lang/simulator_statements.py
+-rw-rw-rw-   0        0        0     4697 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/timed_statements.py
+-rw-rw-rw-   0        0        0     1014 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/timeline.py
+-rw-rw-rw-   0        0        0      431 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/lang/triggers.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/modules/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/modules/__init__.py
+-rw-rw-rw-   0        0        0     9514 2023-07-27 12:32:31.000000 q1pulse-0.9.1/q1pulse/modules/modules.py
+-rw-rw-rw-   0        0        0     3028 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/modules/sequencer_states.py
+-rw-rw-rw-   0        0        0     7011 2023-07-27 12:36:42.000000 q1pulse-0.9.1/q1pulse/program.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/sequencer/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/sequencer/__init__.py
+-rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.9.1/q1pulse/sequencer/builderbase.py
+-rw-rw-rw-   0        0        0    14380 2023-07-28 13:37:14.000000 q1pulse-0.9.1/q1pulse/sequencer/control.py
+-rw-rw-rw-   0        0        0     6414 2023-07-27 12:37:02.000000 q1pulse-0.9.1/q1pulse/sequencer/readout.py
+-rw-rw-rw-   0        0        0    12984 2023-07-27 13:36:41.000000 q1pulse-0.9.1/q1pulse/sequencer/sequencer.py
+-rw-rw-rw-   0        0        0     3395 2023-07-11 15:30:18.000000 q1pulse-0.9.1/q1pulse/sequencer/sequencer_data.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse/util/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.9.1/q1pulse/util/__init__.py
+-rw-rw-rw-   0        0        0      690 2023-07-24 12:53:33.000000 q1pulse-0.9.1/q1pulse/util/qblox_version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 13:45:15.000000 q1pulse-0.9.1/q1pulse.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1224 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-28 13:45:14.000000 q1pulse-0.9.1/q1pulse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-28 13:45:15.000000 q1pulse-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      310 2023-07-28 13:45:07.000000 q1pulse-0.9.1/setup.py
```

### Comparing `q1pulse-0.8.8/LICENSE` & `q1pulse-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/assembler/generator.py` & `q1pulse-0.9.1/q1pulse/assembler/generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import logging
 from pprint import pprint
 from numbers import Number
 import numpy as np
 import math
 from functools import wraps
 from contextlib import contextmanager
+from dataclasses import dataclass, field
+from typing import List
 
 from .generator_data import GeneratorData
-from .instruction_queue import InstructionQueue
+from .instruction_queue import InstructionQueue, Instruction
 from .registers import SequencerRegisters
 from ..lang.math_expressions import get_dtype, Expression, Operand
 from ..lang.generator import GeneratorBase
 from ..lang.register import Register
 from ..lang.exceptions import (
         Q1ValueError, Q1TypeError,
         Q1Exception, Q1CompileError
@@ -123,26 +125,35 @@
                 raise Q1CompileError(msg) from ex
 
         return func_wrapper
 
     return decorator_register_args
 
 
+@dataclass
+class ConditionalBlockState:
+    rt_time_start: int = 0
+    n_rt_instruction_start: int = 0
+    last_rt_instructions: List[Instruction] = field(default_factory=list)
+    rt_end_times: List[int] = field(default_factory=list)
+
+
 class Q1asmGenerator(InstructionQueue, GeneratorBase):
     def __init__(self, add_comments=False, list_registers=True,
                  line_numbers=True, comment_arg_conversions=False,
                  optimize=1):
         super().__init__(add_comments=add_comments)
         self._list_registers = list_registers
         self._line_numbers = line_numbers
         self._show_arg_conversions = comment_arg_conversions
         self._optimize = optimize
         self.q1asm = None
         self._repetitions = 1
         self._last_rt_settings = {}
+        self._conditional_block_state = None
         self._data = GeneratorData()
         self._registers = SequencerRegisters(self._add_reg_comment if add_comments else None)
         # counter for signed ASR emulation
         self._asr_jumps = 0
         self.modifies_frequency = False
         self.add_comment('--INIT--', init_section=True)
 
@@ -153,14 +164,15 @@
 
     @repetitions.setter
     def repetitions(self, value):
         self._repetitions = value
 
     def start_main(self):
         self._add_rt_command('wait_sync', time=0)
+        self._wait_till(100)
         self._reset_time()
         self.add_comment('--START-- (t=0)')
         self.set_label('_start')
         self.block_start()
         self.reset_phase(0)
         self._contains_io_instr = False
 
@@ -192,14 +204,65 @@
         # rt_settings may not be overwritten across block boundary
         self._last_rt_settings = {}
 
     def block_end(self):
         # NOTE pending update will move to next block start.
         self._last_rt_settings = {}
 
+    def enter_conditional(self, time):
+        self._flush_pending_update()
+        self._wait_till(time)
+        self.add_comment('Start conditional block')
+        self._conditional_block_state = ConditionalBlockState()
+
+    def set_condition(self, mask, operator):
+        # always use 4 ns for else-wait.
+        self._add_instruction('set_cond', 1, mask, operator, 4)
+        # Store rt state at start to set the time after the block.
+        self._conditional_block_state.n_rt_instruction_start = self._n_rt_instructions
+        self._conditional_block_state.rt_time_start = self._rt_time
+
+    def exit_condition(self):
+        self._flush_pending_update()
+        self._last_rt_settings = {}
+        cbs = self._conditional_block_state
+        # add wait command if there is no pending rt command with wait_after time
+        if self._last_rt_command is None:
+            self._add_rt_command('wait', time=self._rt_time)
+        else_time = 4*(self._n_rt_instructions - cbs.n_rt_instruction_start)
+        self.add_comment(f'End condition. total wait_else {else_time} ns (t_end={self._rt_time})')
+        # update end times of previous branches with time spent in else-wait.
+        for i in range(len(cbs.rt_end_times)):
+            cbs.rt_end_times[i] += else_time
+        # store last rt-statement
+        cbs.last_rt_instructions.append(self._last_rt_command)
+        cbs.rt_end_times.append(self._rt_time)
+        # set time to else time.
+        self._rt_time = cbs.rt_time_start + else_time
+        self._last_rt_command = None
+
+    def exit_conditional(self, time):
+        cbs = self._conditional_block_state
+        max_rt_time_branches = max(cbs.rt_end_times)
+        if max_rt_time_branches > time:
+            self.add_comment(f'End conditional block t={time}, '
+                             f'wait_after {max_rt_time_branches-time} ns, '
+                             f'next at {max_rt_time_branches} ns')
+            time = max_rt_time_branches
+        else:
+            self.add_comment(f'End conditional block t={time}')
+        # update wait after of last instructions
+        for rt_instr, end_time in zip(cbs.last_rt_instructions, cbs.rt_end_times):
+            rt_instr.wait_after += time-end_time
+        # disable condition
+        self._add_instruction('set_cond', 0, 0, 0, 4)
+        self._conditional_block_state = None
+        self._last_rt_command = None
+        self._rt_time = time
+
     @register_args(signature='I')
     def jmp(self, label):
         self._add_instruction('jmp', label)
 
     @register_args(signature='ffI')
     def jlt(self, register, value, label):
         self._add_instruction('jlt', register, value, label)
@@ -389,23 +452,23 @@
         if wave0 is None:
             wave0 = wave1
         elif wave1 is None:
             wave1 = wave0
         wave0 = self._data.translate_wave(wave0)
         wave1 = self._data.translate_wave(wave1)
         self._add_rt_command('play', wave0, wave1,
-                             time=time)
+                             time=time, updating=True)
         self._contains_io_instr = True
 
     @register_args(signature='toI')
     def acquire(self, time, section, bin_index):
         section = self._data.translate_acquisition(section)
         self._add_rt_command('acquire',
                              section, bin_index,
-                             time=time)
+                             time=time, updating=True)
         self._contains_io_instr = True
 
     @register_args(signature='toIoo')
     def acquire_weighed(self, time, bins, bin_index, weight0, weight1):
         bins = self._data.translate_acquisition(bins)
         weight0 = self._data.translate_weight(weight0)
         weight1 = self._data.translate_weight(weight1)
@@ -413,21 +476,28 @@
         # Use acquire_weighed imm,reg,reg,reg,imm instead
         if not isinstance(bin_index, Number):
             with self._registers.temp_regs(2) as (rw0, rw1):
                 self.move(weight0, rw0)
                 self.move(weight1, rw1)
                 self._add_rt_command('acquire_weighed',
                                      bins, bin_index, rw0, rw1,
-                                     time=time)
+                                     time=time, updating=True)
         else:
             self._add_rt_command('acquire_weighed',
                                  bins, bin_index, weight0, weight1,
-                                 time=time)
+                                 time=time, updating=True)
         self._contains_io_instr = True
 
+    @register_args(signature='tI')
+    def set_latch_en(self, time, mask):
+        self._add_rt_command('set_latch_en', mask, time=time)
+
+    def latch_rst(self, time):
+        self._add_rt_command('latch_rst', time=time)
+
     @contextmanager
     def unsigned_registers(self):
         emulate_signed = self.emulate_signed
         self.emulate_signed = False
         yield
         self.emulate_signed = emulate_signed
```

### Comparing `q1pulse-0.8.8/q1pulse/assembler/generator_data.py` & `q1pulse-0.9.1/q1pulse/assembler/generator_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/assembler/instruction_queue.py` & `q1pulse-0.9.1/q1pulse/assembler/instruction_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         self._init_section = []
         self._instructions = []
         self._reg_comment = None
         self._wait_loop_cnt = 0
         self._rt_time = 0
         self._pending_update = None
         self._last_rt_command = None
+        self._n_rt_instructions = 0
         self._finalized = False
         self._updating_reg = None
 
     def add_comment(self, line, init_section=False):
         if not self.add_comments:
             return
         if self._finalized:
@@ -87,27 +88,28 @@
         else:
             comment = None
         instruction = Instruction(mnemonic, args, comment=comment)
         self.__append_instruction(instruction)
         self._schedule_update(time)
         return instruction
 
-    def _add_rt_command(self, mnemonic, *args, time=None, index=None):
-        self._wait_till(time, pending_update='merge')
+    def _add_rt_command(self, mnemonic, *args, time=None, index=None, updating=False):
+        self._wait_till(time, pending_update='merge' if updating else 'flush')
         wait_after = RT_RESOLUTION
         if self.add_comments:
             comment = f't={time}'
         else:
             comment = None
         instruction = Instruction(mnemonic, args, comment=comment, wait_after=wait_after)
         if index is None:
             self.__append_instruction(instruction)
         else:
             self._instructions.insert(index, instruction)
         self._last_rt_command = instruction
+        self._n_rt_instructions += 1
         self._rt_time += wait_after
 
     def _overwrite_rt_setting(self, instruction):
         instruction.overwritten = True
         if self.add_comments:
             instruction.comment += ' = overwritten ='
 
@@ -162,37 +164,45 @@
 
     def _flush_pending_update(self):
         pending_update = self._pending_update
         if pending_update is not None:
             wait_after = RT_RESOLUTION
             instruction = Instruction('upd_param',  wait_after=wait_after, comment=f't={pending_update.time}')
             self._instructions.insert(pending_update.index, instruction)
+            self._n_rt_instructions += 1
             self._pending_update = None
             self._last_rt_command = instruction
             self._rt_time += wait_after
 
     def __add_wait_instruction(self, time):
         if time < 0:
             raise Q1InternalError(f'Illegal wait time {time}')
-        n_max,rem_wait = divmod(time, MAX_WAIT)
-        if n_max <= 2:
-            for _ in range(n_max):
-                self._add_instruction('wait', MAX_WAIT)
+        if time < MAX_WAIT:
+            self._add_instruction('wait', time)
+            self._n_rt_instructions += 1
         else:
-            self._wait_loop_cnt += 1
-            with self.temp_regs(1) as wait_reg:
-                self._add_instruction('move', n_max, wait_reg)
-                label = f'wait{self._wait_loop_cnt}'
-                self.set_label(label)
-                self._add_instruction('wait', MAX_WAIT)
-                self._add_instruction('loop', wait_reg, '@'+label)
-        if rem_wait > 0:
-            self._add_instruction('wait', rem_wait)
+            n_max,rem_wait = divmod(time, MAX_WAIT)
+            if n_max <= 2:
+                for _ in range(n_max):
+                    self._add_instruction('wait', MAX_WAIT)
+            else:
+                self._wait_loop_cnt += 1
+                with self.temp_regs(1) as wait_reg:
+                    self._add_instruction('move', n_max, wait_reg)
+                    label = f'wait{self._wait_loop_cnt}'
+                    self.set_label(label)
+                    self._add_instruction('wait', MAX_WAIT)
+                    self._add_instruction('loop', wait_reg, '@'+label)
+            self._n_rt_instructions += n_max
+            if rem_wait > 0:
+                self._add_instruction('wait', rem_wait)
+                self._n_rt_instructions += 1
 
     def _add_wait_reg(self, time_reg, elapsed=0, less_then_65us=False): # @@@ make use of option less_then_65us
+        self._n_rt_instructions += 1 # this is not correct if > 65 us.
         if less_then_65us and elapsed == 0 and not self._check_time_reg:
             # single instruction for short simple wait
             self._add_instruction('wait', time_reg)
             return
 
         wait_reg = self.allocate_reg('_waittime')
         if elapsed > 0:
```

### Comparing `q1pulse-0.8.8/q1pulse/assembler/registers.py` & `q1pulse-0.9.1/q1pulse/assembler/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/instrument.py` & `q1pulse-0.9.1/q1pulse/instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,43 +113,55 @@
             with DelayedKeyboardInterrupt():
                 module = self.modules[seq.module_name]
 
                 q1asm = program.q1asm(name)
                 self._loaded_q1asm[name] = q1asm
                 if q1asm is None:
                     module.disable_seq(seq)
+                    module.set_awg_offsets(seq.seq_nr, 0.0, 0.0)
                     logger.debug(f'Sequencer {name} no sequence')
                     continue
                 instruments_with_sequence.add(module.pulsar.root_instrument)
                 module.upload(seq.seq_nr, q1asm)
                 t = (time.perf_counter() - t_start) * 1000
                 # logger.debug(f'Sequencer {name} loaded ({t:5.3f} ms)')
 
+                module.invalidate_cache(seq.seq_nr, 'offset_awg_path0')
+                module.invalidate_cache(seq.seq_nr, 'offset_awg_path1')
                 module.enable_seq(seq)
                 prog_seq = program[name]
                 module.set_nco(seq.seq_nr, prog_seq.nco_frequency)
                 if prog_seq.modifies_frequency:
                     module.invalidate_cache(seq.seq_nr, 'nco_freq')
                 if prog_seq.mixer_gain_ratio is not None:
                     module.set_mixer_gain_ratio(seq.seq_nr, prog_seq.mixer_gain_ratio)
                 if prog_seq.mixer_phase_offset_degree is not None:
                     module.set_mixer_phase_offset_degree(seq.seq_nr, prog_seq.mixer_phase_offset_degree)
+                # configure trigger counters
+                for counter in prog_seq.trigger_counters:
+                    module.configure_trigger_counter(seq.seq_nr, counter.trigger.address,
+                                                     counter.threshold, counter.invert)
 
         t = (time.perf_counter() - t_start) * 1000
         # logger.debug(f'Configure QRMs ({t:5.3f} ms)')
         for name,seq in self.readouts.items():
             with DelayedKeyboardInterrupt():
                 readout = program[name]
                 module = self.modules[seq.module_name]
                 if not module.enabled(seq.seq_nr):
                     continue
                 module.thresholded_acq_rotation(seq.seq_nr, readout.thresholded_acq_rotation)
                 module.thresholded_acq_threshold(seq.seq_nr, readout.thresholded_acq_threshold)
                 module.integration_length_acq(seq.seq_nr, int(readout.integration_length_acq))
                 module.delete_acquisition_data(seq.seq_nr)
+                trigger = readout.trigger
+                if trigger is not None:
+                    module.set_trigger(seq.seq_nr, trigger.address, trigger.invert)
+                else:
+                    module.set_trigger(seq.seq_nr, None)
 
         with DelayedKeyboardInterrupt():
             # Note: arm per sequencer. Arm on the cluster still gives red leds on the modules.
             for module in self.modules.values():
                 module.arm_sequencers()
 
             if Q1Instrument._i_feel_lucky:
@@ -176,23 +188,26 @@
                 if not module.enabled(seq.seq_nr):
                     continue
                 state = module.get_sequencer_state(seq.seq_nr, timeout_minutes)
                 logger.log(state.level,
                             f'Status {name} ({module.pulsar.name}:{seq.seq_nr}):'
                              f'{state}')
                 msg_level = max(msg_level, state.level)
+                if state.status != 'STOPPED' or state.level >= logging.WARNING:
+                    errors[name] = str(state)
+                    # reset awg offsets in case of any error.
+                    module.set_awg_offsets(seq.seq_nr, 0.0, 0.0)
                 if state.input_overloaded:
                     if Q1Instrument._exception_on_overload:
                         raise Q1InputOverloaded(
                                 f'INPUT OVERLOAD on {name}.'
                                 '\nException can be suppressed with q1pulse.set_exception_on_overload(False)')
                     else:
                         print(f'WARNING: input overload on {name}')
-                if state.status != 'STOPPED' or state.level >= logging.WARNING:
-                    errors[name] = str(state)
+
         if msg_level == logging.ERROR:
             logger.error('*** Program errors ***')
             for name,state in errors.items():
                 logger.error(f'  {name}: {state}')
             raise Exception(f'Q1 failures (see logger):\n {errors}')
 
         with DelayedKeyboardInterrupt():
@@ -250,8 +265,8 @@
 
 def check_instrument_status(instrument, print_status=False):
     sys_state = instrument.get_system_state()
     if sys_state.status != 'OKAY':
         if getattr(instrument, 'is_dummy', False):
             print(f'Status (Dummy) {instrument.name}:', sys_state)
         else:
-            raise Exception(f'Module {instrument.name} status not OKAY: {sys_state}')
+            raise Exception(f'{instrument.name} status not OKAY: {sys_state}')
```

### Comparing `q1pulse-0.8.8/q1pulse/lang/exceptions.py` & `q1pulse-0.9.1/q1pulse/lang/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     '''
 
 class Q1ValueError(Q1Exception):
     '''
     Raised when invalid value is passed.
     '''
 
+class Q1SyntaxError(Q1Exception):
+    '''
+    Raised when invalid value is passed.
+    '''
+
 class Q1CompileError(Q1Exception):
     '''
     Raised when the error is detected during compilation.
     '''
 
 class Q1SequenceError(Q1Exception):
     '''
```

### Comparing `q1pulse-0.8.8/q1pulse/lang/flow_statements.py` & `q1pulse-0.9.1/q1pulse/lang/flow_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/generator.py` & `q1pulse-0.9.1/q1pulse/lang/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/loops.py` & `q1pulse-0.9.1/q1pulse/lang/loops.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/math_expressions.py` & `q1pulse-0.9.1/q1pulse/lang/math_expressions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/register.py` & `q1pulse-0.9.1/q1pulse/lang/register.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/register_statements.py` & `q1pulse-0.9.1/q1pulse/lang/register_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/registers.py` & `q1pulse-0.9.1/q1pulse/lang/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/sequence.py` & `q1pulse-0.9.1/q1pulse/lang/sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .timed_statements import TimedStatement
+from .timed_statements import TimedStatement, MultiBranchStatement
 from .flow_statements import BranchStatement
 from .exceptions import Q1Exception, Q1SequenceError
 
 class Sequence:
     def __init__(self, timeline):
         self.timeline = timeline
         self._statements = []
@@ -25,14 +25,17 @@
                 time = '#     '
             else:
                 time = ' '*6
             line = f'{time}  {white}{statement}'
             lines.append(line)
             if isinstance(statement, BranchStatement):
                 statement.sequence.describe(lines, indent+1)
+            if isinstance(statement, MultiBranchStatement):
+                for branch in statement.branches:
+                    branch.describe(lines, indent+1)
 
     def compile(self, generator, annotate=False):
         for statement in self._statements:
             if annotate:
                 s = str(statement)
                 if isinstance(statement, TimedStatement):
                     s += f' t={statement.time}'
```

### Comparing `q1pulse-0.8.8/q1pulse/lang/simulator_statements.py` & `q1pulse-0.9.1/q1pulse/lang/simulator_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse/lang/timed_statements.py` & `q1pulse-0.9.1/q1pulse/lang/timed_statements.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from .base import Statement
 
 class TimedStatement(Statement):
     def __init__(self, time):
         self.time = time
 
 
+class MultiBranchStatement(TimedStatement):
+    def __init__(self, time):
+        super().__init__(time)
+        self.branches = []
+
+
 class WaitRegStatement(TimedStatement):
     def __init__(self, time, register):
         super().__init__(time)
         self.register = register
 
     def __repr__(self):
         return f'wait({self.register})'
```

### Comparing `q1pulse-0.8.8/q1pulse/lang/timeline.py` & `q1pulse-0.9.1/q1pulse/lang/timeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,17 +21,18 @@
         return not self._disabled
 
     @property
     def current_time(self):
         return self._current_time
 
     def set_pulse_end(self, value):
+        time = max(value, self._end_time)
         if not self._disabled:
-            self._current_time = value
-        self._end_time = max(value, self._end_time)
+            self._current_time = time
+        self._end_time = time
 
     @property
     def end_time(self):
         return self._end_time
 
     def reset(self):
         self._current_time = 0
```

### Comparing `q1pulse-0.8.8/q1pulse/modules/modules.py` & `q1pulse-0.9.1/q1pulse/modules/modules.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     n_sequencers = 6
 
     def __init__(self, pulsar):
         self.name = pulsar.name
         # check module is present in slot.
         if hasattr(pulsar, 'present'):
             if not pulsar.present():
-                raise Exception('No module in slot {pulsar.slot_idx()}')
+                raise Exception('No module in slot {pulsar.slot_idx}')
         self.pulsar = pulsar
         self._allocated_seq = 0
         self.disable_all_out()
         # disable all sequencers
         for seq_nr in range(0, self.n_sequencers):
             self.enable_sync(seq_nr, False)
 
@@ -99,14 +99,22 @@
 
     def set_mixer_gain_ratio(self, seq_nr, value):
         self._sset(seq_nr, 'mixer_corr_gain_ratio', value)
 
     def set_mixer_phase_offset_degree(self, seq_nr, value):
         self._sset(seq_nr, 'mixer_corr_phase_offset_degree', value)
 
+    def configure_trigger_counter(self, seq_nr, address, threshold, invert):
+        self._sset(seq_nr, f'trigger{address}_count_threshold', threshold)
+        self._sset(seq_nr, f'trigger{address}_threshold_invert', invert)
+
+    def set_awg_offsets(self, seq_nr, offset0, offset1):
+        self._sset(seq_nr, f'offset_awg_path0', offset0)
+        self._sset(seq_nr, f'offset_awg_path1', offset1)
+
     def enabled(self, seq_nr):
         seq = getattr(self.pulsar, f'sequencer{seq_nr}')
         param = seq.parameters['sync_en']
         return param.cache()
 
     def disable_seq(self, sequencer):
         seq_nr = sequencer.seq_nr
@@ -119,15 +127,15 @@
             self.enable_out(seq_nr, ch)
 
     def _sset(self, seq_nr, name, value, cache=True):
         full_name = f'sequencer{seq_nr}.{name}'
         seq = getattr(self.pulsar, f'sequencer{seq_nr}')
         param = seq.parameters[name]
         try:
-            if cache and param.cache() == value:
+            if cache and param.cache.valid and param.cache() == value:
                 if QbloxModule.verbose:
                     logger.debug(f'# {full_name}={value} -- cached')
                 return
         except:
             logger.debug(f'No cache value for {full_name}')
         result = param(value)
         if QbloxModule.verbose:
@@ -239,7 +247,15 @@
 
     def delete_acquisition_data(self, seq_nr):
         self.pulsar.delete_acquisition_data(seq_nr, all=True)
 
     def set_nco(self, seq_nr, nco_frequency):
         super().set_nco(seq_nr, nco_frequency)
         self._sset(seq_nr, 'demod_en_acq', nco_frequency is not None)
+
+    def set_trigger(self, seq_nr, address, invert=False):
+        enabled = address is not None and address > 0
+        self._sset(seq_nr, 'thresholded_acq_trigger_en', enabled)
+        if enabled:
+            self._sset(seq_nr, 'thresholded_acq_trigger_address', address)
+            self._sset(seq_nr, 'thresholded_acq_trigger_invert', invert)
+
```

### Comparing `q1pulse-0.8.8/q1pulse/modules/sequencer_states.py` & `q1pulse-0.9.1/q1pulse/modules/sequencer_states.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     'ACQ BINNING OUT OF RANGE': WARNING,
     'ACQ INDEX INVALID': ERROR,
     'ACQ BIN INDEX INVALID': ERROR,
     'TRIGGER NETWORK CONFLICT': ERROR,
     'TRIGGER NETWORK MISSED INTERNAL TRIGGER': ERROR,
     'OUTPUT OVERFLOW': ERROR,
     'CLOCK INSTABILITY': ERROR,
+    'ACQ INTEGRATOR OUT OF RANGE PATH 0': WARNING,
+    'ACQ INTEGRATOR OUT OF RANGE PATH 1': WARNING,
     }
 
 
 @dataclass
 class SequencerState:
     status: str
     level: int = 10
```

### Comparing `q1pulse-0.8.8/q1pulse/program.py` & `q1pulse-0.9.1/q1pulse/program.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import os
 from contextlib import contextmanager
 from numbers import Number
 
+from .lang.conditions import CounterFlags
+from .lang.exceptions import Q1InternalError, Q1ValueError
+from .lang.triggers import TriggerCounter, Trigger
 from .lang.math_expressions import Expression
 from .lang.timeline import Timeline
 from .lang.registers import Registers
 from .lang.register import Register
 from .lang.register_statements import RegisterAssignment
 from .lang.loops import RangeLoop, LinspaceLoop, ArrayLoop
 from .assembler.generator import Q1asmGenerator
-from .lang.exceptions import Q1InternalError, Q1ValueError
+
 
 class Program:
     def __init__(self, path=None):
         self.sequence_builders = {}
         self.path = path if path is not None else os.path.join('q1','_prog')
         self.R = Registers(self, local=False)
         self.repetitions = 1
         self._q1asm = {}
         self._loop_cnt = 0
+        self._triggers = []
         # shared timeline for all sequencers
         self._timeline = Timeline()
 
     def add_sequence_builder(self, sequence_builder):
         name = sequence_builder.name
         self.sequence_builders[name] = sequence_builder
         setattr(self, name, sequence_builder)
@@ -89,14 +93,52 @@
 
     @contextmanager
     def parallel(self):
         self._timeline.disable_update()
         yield
         self._timeline.enable_update()
 
+    @contextmanager
+    def conditional(self, counters, t_offset=0, evaluation_time=0):
+        for s in self.sequence_builders.values():
+            s.enter_conditional(counters, t_offset=t_offset, evaluation_time=evaluation_time)
+        flags = CounterFlags(self)
+        yield flags
+        for s in self.sequence_builders.values():
+            s.exit_conditional()
+
+    @contextmanager
+    def condition(self, operator):
+        for s in self.sequence_builders.values():
+            s.enter_condition(operator)
+        yield
+        for s in self.sequence_builders.values():
+            s.exit_condition()
+
+    def configure_trigger(self, sequencer_name, invert=False):
+        addr = len(self._triggers)+1
+        trigger = Trigger(sequencer_name, address=addr, invert=invert)
+        self._triggers.append(trigger)
+        self.sequence_builders[sequencer_name].trigger = trigger
+        return trigger
+
+    def add_trigger_counter(self, trigger, threshold=1, invert=False):
+        counter = TriggerCounter(trigger, threshold=threshold, invert=invert)
+        for s in self.sequence_builders.values():
+            s._add_trigger_counter(counter)
+        return counter
+
+    def latch_enable(self, counters, t_offset=0):
+        for s in self.sequence_builders.values():
+            s.latch_enable(counters, t_offset=t_offset)
+
+    def latch_reset(self, t_offset=0):
+        for s in self.sequence_builders.values():
+            s.latch_reset(t_offset=t_offset)
+
     def add_comment(self, comment):
         for s in self.sequence_builders.values():
             s.add_comment(comment)
 
     def wait(self, t):
         if isinstance(t, Number):
             if t < 0:
```

### Comparing `q1pulse-0.8.8/q1pulse/sequencer/control.py` & `q1pulse-0.9.1/q1pulse/sequencer/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,18 @@
             When hires_reg=True this costs ~268 ns.
 
             When `phase` is a constant in q1asm, then the resolution is 1e-9.
             No extra time is needed.
         '''
         t1 = self.current_time + t_offset
         self.set_pulse_end(t1)
+        # WORKAROUND: Qblox sequencer inverts phase delta when frequency is negative
+        # TODO: remove workaround when fixed in firmware
+        if self._nco_frequency and self._nco_frequency < 0:
+            delta = -delta
         self._add_statement(ShiftPhaseStatement(t1, delta, hires_reg))
 
     def set_phase(self, phase, t_offset=0, hires_reg=True):
         '''
         Args:
             hires_reg:
                 Convert register to exactly phase if True, else
@@ -278,17 +282,18 @@
             # TODO: for more precision: add f_step fraction (use 64 bit numbers?)
             f_step = round(f_step)
             w_chirpI, w_chirpQ, delta_phase = self._waves.get_chirp(chirp_loop_time, f_step)
             # divmod, but with rem [1,100], and n > 1
             n, rem = divmod(duration-1, chirp_loop_time)
             rem += 1
 
-            # Note: Qblox sequencer inverts phase delta when frequency is negative
-            if f_start < 0:
-                delta_phase = -delta_phase
+            # TODO: remove workaround when fixed in firmware
+            # Temporarily set NCO frequency for phase shift workaround.
+            nco_freq = self.nco_frequency
+            self.nco_frequency = f_start
 
             self.Rs._freq = int(f_start)
             self.set_gain(amplitude, amplitude)
             if n > 0:
                 with self._seq_repeat(n):
                     self.shift_phase(delta_phase)
                     self.set_frequency(self.Rs._freq)
@@ -296,25 +301,26 @@
                     self.Rs._freq += f_step
                     self.wait(chirp_loop_time)
             self.shift_phase(delta_phase)
             self.set_frequency(self.Rs._freq)
             self.play(w_chirpI, w_chirpQ)
             self.wait(rem)
             self.set_gain(0.0)
+            self.nco_frequency = nco_freq
 
     def _apply_paths(self, arg0, arg1):
         if len(self._enabled_paths) == 0:
             raise Q1ValueError('No output paths enabled')
 
         if len(self._enabled_paths) == 1:
             path = self._enabled_paths[0]
-            if arg1 is not None:
-                raise Q1ValueError('Only 1 output path enabled')
-
-            return (arg0, None) if path == 0 else (None, arg0)
+            if arg1 is None:
+                return (arg0, None) if path == 0 else (None, arg0)
+            else:
+                return (arg0, arg1) if path == 0 else (-arg1, arg0)
 
         # channels could be swapped
         args = (arg0, arg1)
         return (args[i] for i in self._enabled_paths)
 
     def _translate_wave(self, wave):
         if wave is None:
```

### Comparing `q1pulse-0.8.8/q1pulse/sequencer/readout.py` & `q1pulse-0.9.1/q1pulse/sequencer/readout.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
                  nco_frequency=None):
         super().__init__(name, enabled_paths, max_output_voltage, nco_frequency)
         self._acquisitions = AcquisitionBinsCollection()
         self._weights = WeightCollection()
         self._integration_length_acq = 4
         self._thresholded_acq_rotation = 0.0
         self._thresholded_acq_threshold = 0.0
+        self._trigger = None
 
     @property
     def thresholded_acq_rotation(self):
         return self._thresholded_acq_rotation
 
     @thresholded_acq_rotation.setter
     def thresholded_acq_rotation(self, rotation):
@@ -40,14 +41,22 @@
     def integration_length_acq(self):
         return self._integration_length_acq
 
     @integration_length_acq.setter
     def integration_length_acq(self, length):
         self._integration_length_acq = int(length)
 
+    @property
+    def trigger(self):
+        return self._trigger
+
+    @trigger.setter
+    def trigger(self, trigger):
+        self._trigger = trigger
+
     def add_acquisition_bins(self, name, num_bins):
         return self._acquisitions.define_bins(name, num_bins)
 
     def add_weight(self, name, data):
         return self._weights.add_weight(name, data)
 
     def acquire(self, bins, bin_index='increment', t_offset=0):
```

### Comparing `q1pulse-0.8.8/q1pulse/sequencer/sequencer.py` & `q1pulse-0.9.1/q1pulse/sequencer/sequencer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 import sys
 import os
+from copy import copy
 from contextlib import contextmanager
 import traceback
+import logging
 
 from .builderbase import BuilderBase
+from ..lang.triggers import TriggerCounter
 from ..lang.exceptions import (
         Q1StateError, Q1Exception,
         Q1InternalError, Q1SequenceError,
-        Q1TimingError
+        Q1TimingError, Q1SyntaxError,
         )
 from ..lang.sequence import Sequence
 from ..lang.loops import Loop
 from ..lang.registers import Registers
 from ..lang.timed_statements import WaitRegStatement, TimedStatement
 from ..lang.flow_statements import (
         LoopDurationStatement,
         LoopStatement, EndLoopStatement,
         ArrayLoopStatement, EndArrayLoopStatement,
         )
 from ..lang.loops import LinspaceLoop, RangeLoop, ArrayLoop
 from ..lang.simulator_statements import LogStatement
+from ..lang.conditions import (
+        LatchEnableStatement, LatchResetStatement,
+        BranchSequence, ConditionalBlockStatement,
+        CounterFlags,
+        )
+
+logger = logging.getLogger(__name__)
+
 
 class SequenceBuilder(BuilderBase):
     add_traceback_to_instructions = True
     '''
     Adding traceback is convenient to find a problem in your script.
     However, it makes the compiler pretty slow.
     Q1Instrument can suppress the traceback.
@@ -35,14 +46,17 @@
         self.Rs = Registers(self, local=True)
         self._sequence_stack = []
         self._local_time = 0
         self._local_time_active = False
         self._compiled = False
         self._init_sequence = Sequence(None)
         self._last_timed_statement = None
+        self._conditional_block = None
+        self._in_condition = False
+        self._trigger_counters = []
 
     def start_sequence(self, program, timeline):
         self._program = program
         self._timeline = timeline
         self._start_sequence()
 
     def _start_sequence(self):
@@ -60,14 +74,15 @@
             raise Q1StateError('Program cannot be changed after compilation')
         if init_section:
             self._init_sequence.add(statement)
         else:
             self.sequence.add(statement)
 
     def _check_time(self, statement):
+        # TODO: Distinguish parameter operations vs RT IO / RT control instructions.
         if not isinstance(statement, TimedStatement):
             return
         t = statement.time
         if int(t) % 4:
             raise Q1TimingError(f'Time must be multiple of 4 ns:\n'
                                 f'Adding:  t={statement.time}  {statement}')
         last = self._last_timed_statement
@@ -124,36 +139,37 @@
         fp.write(f'Sequence:{self.name}\n')
         for line in init + lines:
             fp.write(line+'\n')
         fp.write('\n')
 
     def compile(self, generator, annotate=False):
         try:
-            if not self._compiled:
-                self._compiled = True
             self._init_sequence.compile(generator, annotate)
             generator.start_main()
             self._sequence_stack[0].compile(generator, annotate)
             generator.end_main(self.end_time)
             self.modifies_frequency = generator.modifies_frequency
+            self._compiled = True
         except Q1Exception as ex:
+            logger.error(f'Compilation error on {self.name}', exc_info=True)
             msgs = [f'Error compiling {self.name}.']
             tb = []
             e = ex
             while e is not None:
                 if isinstance(e, Q1SequenceError):
                     tb = e.traceback
                 msgs.append(f'{type(e).__name__}: {e.args[0]}')
                 e = e.__cause__
             q1_tb = '\n'.join(tb+msgs)
             self._dump_compile_state(generator, q1_tb, ex)
             # Use 'from None' to suppress original context
             # This avoids exposure of and confusion by q1pulse internals.
             raise Q1Exception(q1_tb) from None
         except Exception as ex:
+            logger.error(f'Compilation error on {self.name}', exc_info=True)
             self._dump_compile_state(generator, None, ex)
             raise
 
     def _dump_compile_state(self, generator, q1_tb, exc):
         filename = os.path.join(os.getcwd(), '_q1pulse_dump.txt')
         print(f'**** Exception in {self.name} while compiling. ****')
         print(f'**** For details see: {filename} ****')
@@ -179,14 +195,16 @@
         if self._local_time_active:
             self._local_time += max(0, value - self.current_time)
         else:
             self.sequence.timeline.set_pulse_end(value)
 
     @contextmanager
     def _local_timeline(self, duration=None, t_offset=0):
+        if self._local_time_active:
+            raise Q1InternalError('Local timeline already active')
         end_time = self.current_time + t_offset
         if duration is not None:
             end_time += duration
         self._local_time = t_offset
         self._local_time_active = True
         yield
         self._local_time = 0
@@ -216,15 +234,15 @@
         else:
             raise Q1InternalError('Unknown loop')
         self._add_statement(loop_end_statement)
         self._sequence_stack.pop()
 
     @contextmanager
     def _seq_repeat(self, n):
-        ''' repeat loop not synchronizing with other sequencers. Internal use only ''' # @@@ looks like it can be used normally
+        ''' repeat loop not synchronizing with other sequencers. '''
         if n == 0:
             raise ValueError('n must be > 0')
         if n == 1:
             yield
         else:
             t_start = self.current_time
             loop = Loop(self._local_loop_cnt, n, local=True)
@@ -239,11 +257,83 @@
             loop_end_statement = EndLoopStatement(self.current_time, loop)
             self._add_statement(loop_end_statement)
             t_loop = self.current_time - t_start
             self._add_statement(LoopDurationStatement(n, t_loop))
             self._sequence_stack.pop()
             self.set_pulse_end(t_start + n * t_loop)
 
-
     def _add_reg_wait(self, reg):
-        self._add_statement(WaitRegStatement(self.sequence.timeline.end_time, reg))
+        self._add_statement(WaitRegStatement(self.end_time, reg))
+
+    @property
+    def trigger_counters(self):
+        return self._trigger_counters
+
+    def _add_trigger_counter(self, counter):
+        self._trigger_counters.append(counter)
+
+    def add_trigger_counter(self, trigger, threshold=1, invert=False):
+        counter = TriggerCounter(trigger, threshold=threshold, invert=invert)
+        self._add_trigger_counter(counter)
+        return counter
+
+    def latch_enable(self, counters, t_offset=0):
+        time = self.current_time + t_offset
+        self._add_statement(LatchEnableStatement(time, counters))
+        self.set_pulse_end(time)
+
+    def latch_reset(self, t_offset=0):
+        time = self.current_time + t_offset
+        self._add_statement(LatchResetStatement(time))
+        self.set_pulse_end(time)
+
+    @contextmanager
+    def conditional(self, counters, t_offset=0, evaluation_time=0):
+        self.enter_conditional(counters, t_offset=t_offset, evaluation_time=evaluation_time)
+        flags = CounterFlags(self)
+        yield flags
+        self.exit_conditional()
+
+    def enter_conditional(self, counters, t_offset=0, evaluation_time=0):
+        if self._conditional_block:
+            raise Q1SyntaxError('Nested conditional is not supported')
+        for counter in counters:
+            if counter not in self._trigger_counters:
+                raise Q1SyntaxError('Trigger counter {counter} not registered on sequencer')
+        block = ConditionalBlockStatement(self.current_time+t_offset, counters)
+        self._add_statement(block)
+        self.set_pulse_end(self.current_time + t_offset + evaluation_time)
+        self._conditional_block = block
+
+    def exit_conditional(self):
+        timeline = copy(self._timeline)
+        self._conditional_block.close(timeline)
+        self.set_pulse_end(self._conditional_block.end_time)
+        self._conditional_block = None
+
+    @contextmanager
+    def condition(self, operator):
+        self.enter_condition(operator)
+        yield
+        self.exit_condition()
+
+    def enter_condition(self, operator):
+        if self._conditional_block is None:
+            raise Q1SyntaxError('Conditions must be wrapped in `conditional` section.')
+        if self._in_condition:
+            raise Q1SyntaxError('Conditions cannot be nested')
+        self._in_condition = True
+        timeline = copy(self._timeline)
+        branch = BranchSequence(timeline, operator)
+        self._conditional_block.add_branch(branch)
+        self._sequence_stack.append(branch)
+
+    def exit_condition(self, end_time=None):
+        if end_time is None:
+            end_time = self.end_time
+        self.add_comment(f'Condition end time: {end_time}')
+        self._conditional_block.set_end_time(end_time)
+        self._in_condition = False
+        self._sequence_stack.pop()
+        self._last_timed_statement = self._conditional_block
+
```

### Comparing `q1pulse-0.8.8/q1pulse/sequencer/sequencer_data.py` & `q1pulse-0.9.1/q1pulse/sequencer/sequencer_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.8/q1pulse.egg-info/SOURCES.txt` & `q1pulse-0.9.1/q1pulse.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 q1pulse/assembler/__init__.py
 q1pulse/assembler/generator.py
 q1pulse/assembler/generator_data.py
 q1pulse/assembler/instruction_queue.py
 q1pulse/assembler/registers.py
 q1pulse/lang/__init__.py
 q1pulse/lang/base.py
+q1pulse/lang/conditions.py
 q1pulse/lang/exceptions.py
 q1pulse/lang/expression.py
 q1pulse/lang/flow_statements.py
 q1pulse/lang/generator.py
 q1pulse/lang/loops.py
 q1pulse/lang/math_expressions.py
 q1pulse/lang/register.py
 q1pulse/lang/register_statements.py
 q1pulse/lang/registers.py
 q1pulse/lang/sequence.py
 q1pulse/lang/simulator_statements.py
 q1pulse/lang/timed_statements.py
 q1pulse/lang/timeline.py
+q1pulse/lang/triggers.py
 q1pulse/modules/__init__.py
 q1pulse/modules/modules.py
 q1pulse/modules/sequencer_states.py
 q1pulse/sequencer/__init__.py
 q1pulse/sequencer/builderbase.py
 q1pulse/sequencer/control.py
 q1pulse/sequencer/readout.py
```

