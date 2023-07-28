# Comparing `tmp/dnacauldron-2.0.8.tar.gz` & `tmp/dnacauldron-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnacauldron-2.0.8.tar", last modified: Thu May 25 21:39:39 2023, max compression
+gzip compressed data, was "dnacauldron-2.0.9.tar", last modified: Fri Jul 28 17:04:47 2023, max compression
```

## Comparing `dnacauldron-2.0.8.tar` & `dnacauldron-2.0.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.698314 dnacauldron-2.0.8/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1081 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/LICENCE.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      142 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     7501 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/README.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.686314 dnacauldron-2.0.8/dnacauldron/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4949 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/Assembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1063 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyFlaw.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1148 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1843 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8123 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      175 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2324 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4992 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblySimulation.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      922 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/
--rw-rw-r--   0 peter     (1000) peter     (1000)     6114 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6816 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7816 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8788 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3311 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8859 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      521 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyMix/
--rw-rw-r--   0 peter     (1000) peter     (1000)      984 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/AssemblyMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      254 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/AssemblyMixError.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2372 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/HomologousAssemblyMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4859 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3768 2022-06-10 21:42:51.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/RestrictionLigationMix.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/
--rw-rw-r--   0 peter     (1000) peter     (1000)     5787 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3423 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2348 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)       54 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      509 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3607 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    11176 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1733 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3938 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/GraphsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2150 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/PlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      204 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/
--rw-rw-r--   0 peter     (1000) peter     (1000)    10277 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlan.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    12568 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      168 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4111 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/plot_leveled_graph.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3236 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Filter.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Fragment/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2146 2022-12-18 17:38:32.000000 dnacauldron-2.0.8/dnacauldron/Fragment/Fragment.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5698 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/Fragment/FragmentChain.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/
--rw-rw-r--   0 peter     (1000) peter     (1000)     6008 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3418 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      148 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1676 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6665 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     9470 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      316 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      314 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7104 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/SequenceRepository.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1233 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/biotools/
--rw-rw-r--   0 peter     (1000) peter     (1000)      342 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/biotools/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      921 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/biotools/autoselect_enzyme.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4516 2022-12-18 17:38:32.000000 dnacauldron-2.0.8/dnacauldron/biotools/record_operations.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8602 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/biotools/sequence_io.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/report_assets/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/report_assets/imgs/
--rw-rw-r--   0 peter     (1000) peter     (1000)    19541 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/report_assets/imgs/logo.png
--rw-rw-r--   0 peter     (1000) peter     (1000)      303 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/report_assets/report_style.css
--rw-rw-r--   0 peter     (1000) peter     (1000)      973 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/report_assets/simulation_report.pug
--rw-rw-r--   0 peter     (1000) peter     (1000)     1989 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/reports.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      562 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/tools.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/utils/
--rw-rw-r--   0 peter     (1000) peter     (1000)      512 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/utils/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    11627 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/utils/insert_parts_on_backbones.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4918 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/utils/utils.py
--rw-rw-r--   0 peter     (1000) peter     (1000)       22 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/version.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.686314 dnacauldron-2.0.8/dnacauldron.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     3745 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      175 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/top_level.txt
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.686314 dnacauldron-2.0.8/examples/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/BASIC_assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)      330 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/BASIC_assembly/BASIC_assembly.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/autoselect_connectors/
--rw-rw-r--   0 peter     (1000) peter     (1000)      795 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/autoselect_connectors/autoselect_connectors.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/combinatorial_golden_gate/
--rw-rw-r--   0 peter     (1000) peter     (1000)      661 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/combinatorial_golden_gate/combinatorial_golden_gate.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      640 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/gibson_assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)      634 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/gibson_assembly/gibson_assembly.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/hierarchical_biobrick/
--rw-rw-r--   0 peter     (1000) peter     (1000)      454 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/hierarchical_biobrick/hierarchical_biobrick.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/hierarchical_golden_gate/
--rw-rw-r--   0 peter     (1000) peter     (1000)      523 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/hierarchical_golden_gate/hierarchical_golden_gate.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/lcr_assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)      329 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/lcr_assembly/README.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      384 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/lcr_assembly/example_with_assembly_plan.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/multi_assemby_plan/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1511 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/multi_assemby_plan/multi_assembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8512 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/ez_setup.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1275 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/pypi-readme.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/scripts/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2213 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/scripts/dnacauldron
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-05-25 21:39:39.698314 dnacauldron-2.0.8/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1056 2022-06-10 21:42:51.000000 dnacauldron-2.0.8/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1081 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/LICENCE.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      142 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7501 2023-05-25 21:39:26.000000 dnacauldron-2.0.9/README.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.965986 dnacauldron-2.0.9/dnacauldron/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/Assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4949 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/Assembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1063 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyFlaw.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1148 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1843 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8157 2023-07-28 17:04:35.000000 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      175 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2324 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4992 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/AssemblySimulation.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      922 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6114 2023-05-25 21:39:26.000000 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6816 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7816 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8788 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3311 2023-05-25 21:39:26.000000 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8859 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      521 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/AssemblyMix/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      984 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/AssemblyMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      254 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/AssemblyMixError.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2372 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/HomologousAssemblyMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4859 2022-12-18 16:46:46.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3768 2022-06-10 21:42:51.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/RestrictionLigationMix.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5787 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3423 2022-12-18 16:46:46.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2348 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       54 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      509 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3607 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11176 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1733 2022-12-18 16:46:46.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3938 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/GraphsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2150 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/PlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      204 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/AssemblyPlan/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10277 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyPlan/AssemblyPlan.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    12568 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      168 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyPlan/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4111 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/AssemblyPlan/plot_leveled_graph.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3236 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Filter.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron/Fragment/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2146 2022-12-18 17:38:32.000000 dnacauldron-2.0.9/dnacauldron/Fragment/Fragment.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5698 2022-12-18 16:46:46.000000 dnacauldron-2.0.9/dnacauldron/Fragment/FragmentChain.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/dnacauldron/Fragment/HomologousFragment/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6008 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3418 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      148 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Fragment/HomologousFragment/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1676 2023-05-25 21:39:26.000000 dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6724 2023-07-28 17:04:35.000000 dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9470 2023-05-25 21:39:26.000000 dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      316 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      314 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/Fragment/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7104 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/SequenceRepository.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1233 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/dnacauldron/biotools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      342 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/biotools/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      921 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/biotools/autoselect_enzyme.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4516 2022-12-18 17:38:32.000000 dnacauldron-2.0.9/dnacauldron/biotools/record_operations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8602 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/biotools/sequence_io.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/dnacauldron/report_assets/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/dnacauldron/report_assets/imgs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    19541 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/report_assets/imgs/logo.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)      303 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/report_assets/report_style.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)      973 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/report_assets/simulation_report.pug
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1989 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/reports.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      562 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/tools.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/dnacauldron/utils/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      512 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/dnacauldron/utils/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11627 2022-12-18 16:46:46.000000 dnacauldron-2.0.9/dnacauldron/utils/insert_parts_on_backbones.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4918 2022-12-18 16:46:46.000000 dnacauldron-2.0.9/dnacauldron/utils/utils.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       22 2023-07-28 17:04:35.000000 dnacauldron-2.0.9/dnacauldron/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.969986 dnacauldron-2.0.9/dnacauldron.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2023-07-28 17:04:47.000000 dnacauldron-2.0.9/dnacauldron.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3745 2023-07-28 17:04:47.000000 dnacauldron-2.0.9/dnacauldron.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-28 17:04:47.000000 dnacauldron-2.0.9/dnacauldron.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      175 2023-07-28 17:04:47.000000 dnacauldron-2.0.9/dnacauldron.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-07-28 17:04:47.000000 dnacauldron-2.0.9/dnacauldron.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.965986 dnacauldron-2.0.9/examples/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/BASIC_assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      330 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/BASIC_assembly/BASIC_assembly.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/autoselect_connectors/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      795 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/autoselect_connectors/autoselect_connectors.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/combinatorial_golden_gate/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      661 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/combinatorial_golden_gate/combinatorial_golden_gate.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      640 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/gibson_assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      634 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/gibson_assembly/gibson_assembly.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/hierarchical_biobrick/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      454 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/hierarchical_biobrick/hierarchical_biobrick.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/hierarchical_golden_gate/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      523 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/hierarchical_golden_gate/hierarchical_golden_gate.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/lcr_assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      329 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/lcr_assembly/README.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      384 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/lcr_assembly/example_with_assembly_plan.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/examples/multi_assemby_plan/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1511 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/examples/multi_assemby_plan/multi_assembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8512 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/ez_setup.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1275 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/pypi-readme.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/scripts/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2213 2021-11-25 11:15:52.000000 dnacauldron-2.0.9/scripts/dnacauldron
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-28 17:04:47.973986 dnacauldron-2.0.9/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1056 2022-06-10 21:42:51.000000 dnacauldron-2.0.9/setup.py
```

### Comparing `dnacauldron-2.0.8/LICENCE.txt` & `dnacauldron-2.0.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/PKG-INFO` & `dnacauldron-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnacauldron
-Version: 2.0.8
+Version: 2.0.9
 Summary: Cloning simulation for DNA assembly (Golden Gate, Gibson...)
 Home-page: https://github.com/Edinburgh-Genome-Foundry/DnaCauldron
 Author: Zulko
 License: MIT
 Keywords: DNA assembly cloning simulator synthetic biology
 Platform: UNKNOWN
 Provides-Extra: reports
```

### Comparing `dnacauldron-2.0.8/README.rst` & `dnacauldron-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/Assembly.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/Assembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyFlaw.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyFlaw.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,9 +178,9 @@
                 assembly_simulation, report_root, error_type="error"
             )
         if self.include_warnings_spreadsheet:
             self._write_errors_spreadsheet(
                 assembly_simulation, report_root, error_type="warnings"
             )
 
-        if target == "@memory":
+        if (target == "@memory") or str(target).endswith(".zip"):
             return report_root._close()
```

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblySimulation.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/AssemblySimulation.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/__init__.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/__init__.py` & `dnacauldron-2.0.9/dnacauldron/Assembly/builtin_assembly_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/AssemblyMix.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/AssemblyMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/HomologousAssemblyMix.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/HomologousAssemblyMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/RestrictionLigationMix.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/RestrictionLigationMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/GraphsMixin.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/GraphsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/PlotsMixin.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyMix/mixins/PlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlan.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyPlan/AssemblyPlan.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/AssemblyPlan/plot_leveled_graph.py` & `dnacauldron-2.0.9/dnacauldron/AssemblyPlan/plot_leveled_graph.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Filter.py` & `dnacauldron-2.0.9/dnacauldron/Filter.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Fragment/Fragment.py` & `dnacauldron-2.0.9/dnacauldron/Fragment/Fragment.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Fragment/FragmentChain.py` & `dnacauldron-2.0.9/dnacauldron/Fragment/FragmentChain.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py` & `dnacauldron-2.0.9/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py` & `dnacauldron-2.0.9/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py` & `dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py` & `dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         the other record's left sticky end."""
         right_end = self.seq.right_end
         return (right_end is not None) and right_end.will_clip_directly_with(
             other.seq.left_end
         )
 
     def circularized(
-        self, annotate_homology=False, annotation_type="homology", qualifiers=None,
+        self,
+        annotate_homology=False,
+        annotation_type="homology",
+        qualifiers=None,
     ):
         """Return the Biopython record obtained by cirularizing the result.
 
         Only works if the left and right sticky ends are compatible. The
         return is a simple Biopython record where the sticky end has been
         integrated in the sequence.
         """
@@ -57,15 +60,18 @@
     def annotate_connector(self, connector, annotation_type="homology"):
         """Annotate a connector to indicate it used to be a sticky end."""
         if len(connector) > 8:
             label = "homology"
         else:
             label = str(connector.seq)
         feature = self.create_homology_annotation(
-            start=0, end=len(connector), annotation_type=annotation_type, label=label,
+            start=0,
+            end=len(connector),
+            annotation_type=annotation_type,
+            label=label,
         )
         connector.features = [feature]
 
     @staticmethod
     def assemble(fragments, circularize=False, annotate_homologies=False):
         """Return the (sticky end) record obtained by assembling the fragments.
 
@@ -135,15 +141,15 @@
             )
             return record_fragments[1 : n_cuts + 1]
         fragments = StickyEndSeq.list_from_sequence_digestion(
             record.seq, enzyme, linear=linear
         )
         record_fragments = []
         for fragment in fragments:
-            index = record.seq.find(fragment)
+            index = record.seq.upper().find(fragment)
             if index == -1:
                 continue
 
             def only_parts_indicators(feature):
                 return feature.qualifiers.get("indicates_part", False)
 
             subrecord = crop_record_with_saddling_features(
@@ -163,16 +169,15 @@
 
     def to_standard_string(self):
         """Return a string representation of the fragment, used for quick
         comparison of fragments and fragments chains."""
         return "%s%s%s" % (self.seq.left_end, self.seq, self.seq.right_end)
 
     def text_representation_in_plots(self):
-        """Plot a fragment as left//PART_NAME//right (where // is a new line)
-        """
+        """Plot a fragment as left//PART_NAME//right (where // is a new line)"""
         lines = [
             str(self.seq.left_end),
             r"$\bf{%s}$" % self.original_part.id,
             str(self.seq.right_end),
         ]
         return "\n".join(lines)
```

### Comparing `dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py` & `dnacauldron-2.0.9/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/SequenceRepository.py` & `dnacauldron-2.0.9/dnacauldron/SequenceRepository.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/__init__.py` & `dnacauldron-2.0.9/dnacauldron/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/biotools/autoselect_enzyme.py` & `dnacauldron-2.0.9/dnacauldron/biotools/autoselect_enzyme.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/biotools/record_operations.py` & `dnacauldron-2.0.9/dnacauldron/biotools/record_operations.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/biotools/sequence_io.py` & `dnacauldron-2.0.9/dnacauldron/biotools/sequence_io.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/report_assets/imgs/logo.png` & `dnacauldron-2.0.9/dnacauldron/report_assets/imgs/logo.png`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/report_assets/simulation_report.pug` & `dnacauldron-2.0.9/dnacauldron/report_assets/simulation_report.pug`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/reports.py` & `dnacauldron-2.0.9/dnacauldron/reports.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/tools.py` & `dnacauldron-2.0.9/dnacauldron/tools.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/utils/__init__.py` & `dnacauldron-2.0.9/dnacauldron/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/utils/insert_parts_on_backbones.py` & `dnacauldron-2.0.9/dnacauldron/utils/insert_parts_on_backbones.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron/utils/utils.py` & `dnacauldron-2.0.9/dnacauldron/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/dnacauldron.egg-info/PKG-INFO` & `dnacauldron-2.0.9/dnacauldron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnacauldron
-Version: 2.0.8
+Version: 2.0.9
 Summary: Cloning simulation for DNA assembly (Golden Gate, Gibson...)
 Home-page: https://github.com/Edinburgh-Genome-Foundry/DnaCauldron
 Author: Zulko
 License: MIT
 Keywords: DNA assembly cloning simulator synthetic biology
 Platform: UNKNOWN
 Provides-Extra: reports
```

### Comparing `dnacauldron-2.0.8/dnacauldron.egg-info/SOURCES.txt` & `dnacauldron-2.0.9/dnacauldron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/examples/autoselect_connectors/autoselect_connectors.py` & `dnacauldron-2.0.9/examples/autoselect_connectors/autoselect_connectors.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/examples/combinatorial_golden_gate/combinatorial_golden_gate.py` & `dnacauldron-2.0.9/examples/combinatorial_golden_gate/combinatorial_golden_gate.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py` & `dnacauldron-2.0.9/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/examples/gibson_assembly/gibson_assembly.py` & `dnacauldron-2.0.9/examples/gibson_assembly/gibson_assembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/examples/hierarchical_golden_gate/hierarchical_golden_gate.py` & `dnacauldron-2.0.9/examples/hierarchical_golden_gate/hierarchical_golden_gate.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/examples/multi_assemby_plan/multi_assembly.py` & `dnacauldron-2.0.9/examples/multi_assemby_plan/multi_assembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/ez_setup.py` & `dnacauldron-2.0.9/ez_setup.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/pypi-readme.rst` & `dnacauldron-2.0.9/pypi-readme.rst`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/scripts/dnacauldron` & `dnacauldron-2.0.9/scripts/dnacauldron`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.8/setup.py` & `dnacauldron-2.0.9/setup.py`

 * *Files identical despite different names*

