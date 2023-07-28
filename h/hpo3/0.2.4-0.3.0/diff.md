# Comparing `tmp/hpo3-0.2.4.tar.gz` & `tmp/hpo3-0.3.0.tar.gz`

## Comparing `hpo3-0.2.4.tar` & `hpo3-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 hpo3-0.2.4/Cargo.toml
--rw-r--r--   0     1001      123     2014 2023-05-08 19:17:53.000000 hpo3-0.2.4/.github/check_version.py
--rw-r--r--   0     1001      123     3163 2023-05-08 19:17:53.000000 hpo3-0.2.4/.github/workflows/release.yml
--rw-r--r--   0     1001      123      713 2023-05-08 19:17:53.000000 hpo3-0.2.4/.gitignore
--rw-r--r--   0     1001      123      637 2023-05-08 19:17:53.000000 hpo3-0.2.4/Makefile
--rw-r--r--   0     1001      123    13785 2023-05-08 19:17:53.000000 hpo3-0.2.4/README.md
--rw-r--r--   0     1001      123  4801046 2023-05-08 19:17:53.000000 hpo3-0.2.4/data/ontology.hpo
--rw-r--r--   0     1001      123      150 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/annotations.rst
--rw-r--r--   0     1001      123     1068 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/conf.py
--rw-r--r--   0     1001      123      112 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/enrichment.rst
--rw-r--r--   0     1001      123     1482 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/getting_started.rst
--rw-r--r--   0     1001      123       79 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/hposet.rst
--rw-r--r--   0     1001      123       82 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/hpoterm.rst
--rw-r--r--   0     1001      123     5515 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/index.rst
--rw-r--r--   0     1001      123     1756 2023-05-08 19:17:53.000000 hpo3-0.2.4/docs/ontology.rst
--rw-r--r--   0     1001      123        0 2023-05-08 19:17:53.000000 hpo3-0.2.4/pyhpo.pyi
--rw-r--r--   0     1001      123     1178 2023-05-08 19:17:53.000000 hpo3-0.2.4/pyproject.toml
--rw-r--r--   0     1001      123     6994 2023-05-08 19:17:53.000000 hpo3-0.2.4/src/annotations.rs
--rw-r--r--   0     1001      123     5096 2023-05-08 19:17:53.000000 hpo3-0.2.4/src/enrichment.rs
--rw-r--r--   0     1001      123     1927 2023-05-08 19:17:53.000000 hpo3-0.2.4/src/information_content.rs
--rw-r--r--   0     1001      123    10179 2023-05-08 19:17:53.000000 hpo3-0.2.4/src/lib.rs
--rw-r--r--   0     1001      123     8771 2023-05-08 19:17:53.000000 hpo3-0.2.4/src/ontology.rs
--rw-r--r--   0     1001      123    13630 2023-05-08 19:17:53.000000 hpo3-0.2.4/src/set.rs
--rw-r--r--   0     1001      123    17096 2023-05-08 19:17:53.000000 hpo3-0.2.4/src/term.rs
--rw-r--r--   0     1001      123      946 2023-05-08 19:17:53.000000 hpo3-0.2.4/tests/benchmarking.py
--rw-r--r--   0     1001      123     4997 2023-05-08 19:17:53.000000 hpo3-0.2.4/tests/test_integration.py
--rw-r--r--   0     1001      123    18983 2023-05-08 19:19:03.000000 hpo3-0.2.4/Cargo.lock
--rw-r--r--   0        0        0    14904 1970-01-01 00:00:00.000000 hpo3-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 hpo3-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     2014 2023-07-28 20:02:53.000000 hpo3-0.3.0/.github/check_version.py
+-rw-r--r--   0     1001      123     3163 2023-07-28 20:02:53.000000 hpo3-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      713 2023-07-28 20:02:53.000000 hpo3-0.3.0/.gitignore
+-rw-r--r--   0     1001      123      637 2023-07-28 20:02:53.000000 hpo3-0.3.0/Makefile
+-rw-r--r--   0     1001      123    13785 2023-07-28 20:02:53.000000 hpo3-0.3.0/README.md
+-rw-r--r--   0     1001      123  4801046 2023-07-28 20:02:53.000000 hpo3-0.3.0/data/ontology.hpo
+-rw-r--r--   0     1001      123      150 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/annotations.rst
+-rw-r--r--   0     1001      123     1068 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/conf.py
+-rw-r--r--   0     1001      123      112 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/enrichment.rst
+-rw-r--r--   0     1001      123     1482 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/getting_started.rst
+-rw-r--r--   0     1001      123       79 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/hposet.rst
+-rw-r--r--   0     1001      123       82 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/hpoterm.rst
+-rw-r--r--   0     1001      123     5515 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/index.rst
+-rw-r--r--   0     1001      123     1756 2023-07-28 20:02:53.000000 hpo3-0.3.0/docs/ontology.rst
+-rw-r--r--   0     1001      123        0 2023-07-28 20:02:53.000000 hpo3-0.3.0/pyhpo.pyi
+-rw-r--r--   0     1001      123     1178 2023-07-28 20:02:53.000000 hpo3-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     8263 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/annotations.rs
+-rw-r--r--   0     1001      123     5114 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/enrichment.rs
+-rw-r--r--   0     1001      123     1927 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/information_content.rs
+-rw-r--r--   0     1001      123    10848 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123     5213 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/linkage.rs
+-rw-r--r--   0     1001      123     8968 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/ontology.rs
+-rw-r--r--   0     1001      123    15889 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/set.rs
+-rw-r--r--   0     1001      123    17159 2023-07-28 20:02:53.000000 hpo3-0.3.0/src/term.rs
+-rw-r--r--   0     1001      123      946 2023-07-28 20:02:53.000000 hpo3-0.3.0/tests/benchmarking.py
+-rw-r--r--   0     1001      123     4997 2023-07-28 20:02:53.000000 hpo3-0.3.0/tests/test_integration.py
+-rw-r--r--   0     1001      123    18965 2023-07-28 20:02:58.000000 hpo3-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0    14904 1970-01-01 00:00:00.000000 hpo3-0.3.0/PKG-INFO
```

### Comparing `hpo3-0.2.4/.github/check_version.py` & `hpo3-0.3.0/.github/check_version.py`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/.github/workflows/release.yml` & `hpo3-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/.gitignore` & `hpo3-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/Makefile` & `hpo3-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/README.md` & `hpo3-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/data/ontology.hpo` & `hpo3-0.3.0/data/ontology.hpo`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/docs/conf.py` & `hpo3-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/docs/getting_started.rst` & `hpo3-0.3.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/docs/index.rst` & `hpo3-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/docs/ontology.rst` & `hpo3-0.3.0/docs/ontology.rst`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/pyproject.toml` & `hpo3-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/src/annotations.rs` & `hpo3-0.3.0/src/annotations.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use std::collections::HashSet;
 use std::hash::Hash;
 
 use pyo3::class::basic::CompareOp;
-use pyo3::exceptions::PyTypeError;
+use pyo3::exceptions::{PyTypeError, PyKeyError};
+use pyo3::types::PyDict;
 use pyo3::{prelude::*, types::PyType};
 
 use hpo::annotations::AnnotationId;
 use hpo::annotations::{GeneId, OmimDiseaseId};
 
 use crate::{get_ontology, set::PyHpoSet, PyQuery};
 
@@ -78,26 +79,44 @@
     }
 
     fn hpo_set(&self) -> PyResult<PyHpoSet> {
         PyHpoSet::try_from(self)
     }
 
     #[classmethod]
-    fn get(_cls: &PyType, query: PyQuery) -> PyResult<Option<PyGene>> {
+    fn get(_cls: &PyType, query: PyQuery) -> PyResult<PyGene> {
         let ont = get_ontology()?;
         match query {
-            PyQuery::Str(symbol) => Ok(ont
+            PyQuery::Str(symbol) => ont
                 .gene_by_name(&symbol)
-                .map(|g| PyGene::new(*g.id(), g.name().into()))),
-            PyQuery::Id(gene_id) => Ok(ont
+                .ok_or(PyKeyError::new_err("No gene found for query"))
+                .map(|g| PyGene::new(*g.id(), g.name().into())),
+            PyQuery::Id(gene_id) => ont
                 .gene(&gene_id.into())
-                .map(|g| PyGene::new(*g.id(), g.name().into()))),
+                .ok_or(PyKeyError::new_err("No gene found for query"))
+                .map(|g| PyGene::new(*g.id(), g.name().into())),
         }
     }
 
+    #[pyo3(signature = (verbose = false))]
+    #[pyo3(text_signature = "($self, verbose)")]
+    #[allow(non_snake_case)]
+    pub fn toJSON<'a>(&'a self, py: Python<'a>, verbose: bool) -> PyResult<&PyDict> {
+        let dict = PyDict::new(py);
+        dict.set_item("name", self.name())?;
+        dict.set_item("id", self.id())?;
+        dict.set_item("symbol", self.name())?;
+
+        if verbose {
+            let hpos: Vec<u32> = self.hpo()?.iter().copied().collect();
+            dict.set_item("hpo", hpos)?;
+        }
+        Ok(dict)
+    }
+
     fn __str__(&self) -> String {
         format!("{} | {}", self.id(), self.name())
     }
 
     fn __repr__(&self) -> String {
         format!("<Gene ({})>", self.name())
     }
@@ -215,19 +234,36 @@
     }
 
     fn hpo_set(&self) -> PyResult<PyHpoSet> {
         PyHpoSet::try_from(self)
     }
 
     #[classmethod]
-    fn get(_cls: &PyType, id: u32) -> PyResult<Option<PyOmimDisease>> {
+    fn get(_cls: &PyType, id: u32) -> PyResult<PyOmimDisease> {
         let ont = get_ontology()?;
-        Ok(ont
+        ont
             .omim_disease(&id.into())
-            .map(|d| PyOmimDisease::new(*d.id(), d.name().into())))
+            .ok_or(PyKeyError::new_err("'No disease found for query'"))
+            .map(|d| PyOmimDisease::new(*d.id(), d.name().into()))
+    }
+
+    #[pyo3(signature = (verbose = false))]
+    #[pyo3(text_signature = "($self, verbose)")]
+    #[allow(non_snake_case)]
+    pub fn toJSON<'a>(&'a self, py: Python<'a>, verbose: bool) -> PyResult<&PyDict> {
+        let dict = PyDict::new(py);
+        dict.set_item("name", self.name())?;
+        dict.set_item("id", self.id())?;
+
+        if verbose {
+            let hpos: Vec<u32> = self.hpo()?.iter().copied().collect();
+            dict.set_item("hpo", hpos)?;
+        }
+
+        Ok(dict)
     }
 
     fn __str__(&self) -> String {
         format!("{} | {}", self.id(), self.name())
     }
 
     fn __repr__(&self) -> String {
```

### Comparing `hpo3-0.2.4/src/enrichment.rs` & `hpo3-0.3.0/src/enrichment.rs`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,16 @@
     enrichment: &hpo::stats::Enrichment<T>,
 ) -> PyResult<&'a PyDict>
 where
     T: std::fmt::Display + hpo::annotations::AnnotationId,
 {
     let disease = get_ontology()?
         .omim_disease(&OmimDiseaseId::from(enrichment.id().as_u32()))
-        .map(|d| PyOmimDisease::new(*d.id(), d.name().into())).unwrap();
+        .map(|d| PyOmimDisease::new(*d.id(), d.name().into()))
+        .unwrap();
     let dict = PyDict::new(py);
     dict.set_item("enrichment", enrichment.pvalue())?;
     dict.set_item("fold", enrichment.enrichment())?;
     dict.set_item("count", enrichment.count())?;
     dict.set_item("item", disease.into_py(py))?;
     Ok(dict)
 }
@@ -147,15 +148,16 @@
     enrichment: &hpo::stats::Enrichment<T>,
 ) -> PyResult<&'a PyDict>
 where
     T: std::fmt::Display + hpo::annotations::AnnotationId,
 {
     let gene = get_ontology()?
         .gene(&GeneId::from(enrichment.id().as_u32()))
-        .map(|g| PyGene::new(*g.id(), g.name().into())).unwrap();
+        .map(|g| PyGene::new(*g.id(), g.name().into()))
+        .unwrap();
     let dict = PyDict::new(py);
     dict.set_item("enrichment", enrichment.pvalue())?;
     dict.set_item("fold", enrichment.enrichment())?;
     dict.set_item("count", enrichment.count())?;
     dict.set_item("item", gene.into_py(py))?;
     Ok(dict)
 }
```

### Comparing `hpo3-0.2.4/src/information_content.rs` & `hpo3-0.3.0/src/information_content.rs`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/src/lib.rs` & `hpo3-0.3.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 use hpo::stats::hypergeom::{disease_enrichment, gene_enrichment};
 use hpo::term::HpoTermId;
 use hpo::{HpoTerm, Ontology as ActualOntology};
 
 mod annotations;
 mod enrichment;
 mod information_content;
+mod linkage;
 mod ontology;
 mod set;
 mod term;
 
 use crate::annotations::{PyGene, PyOmimDisease};
 use crate::enrichment::PyEnrichmentModel;
 use crate::information_content::{PyInformationContent, PyInformationContentKind};
@@ -51,42 +52,56 @@
 
 /// Returns a reference to the Ontology
 ///
 /// This method only works **after** building the ontology
 fn get_ontology() -> PyResult<&'static ActualOntology> {
     ONTOLOGY.get().ok_or_else(|| {
         pyo3::exceptions::PyNameError::new_err(
-            "You must build the ontology first: `ont = pyhpo.Ontology()`",
+            "You must build the ontology first: `>> pyhpo.Ontology()`",
         )
     })
 }
 
 /// Returns a [`PyHpoTerm`] from a `u32` ID
 fn pyterm_from_id(id: u32) -> PyResult<PyHpoTerm> {
     let term = term_from_id(id)?;
     Ok(PyHpoTerm::new(term.id(), term.name().to_string()))
 }
 
 /// Returns an [`HpoTerm`] from a `u32` ID
+///
+/// # Errors
+///
+/// PyKeyError: No term with that ID present in Ontology
 fn term_from_id(id: u32) -> PyResult<hpo::HpoTerm<'static>> {
     let ont = get_ontology()?;
     match ont.hpo(id) {
         Some(term) => Ok(term),
         None => Err(PyKeyError::new_err(format!("No HPOTerm for index {}", id))),
     }
 }
 
 /// Returns an [`HpoTerm`] from a `str` or `u32` query
+///
+/// # Errors
+///
+/// PyValueError: query cannot be converted to HpoTermId
+/// PyRuntimeError: query is a name and does not have a match in the Ontology
 fn term_from_query(query: PyQuery) -> PyResult<HpoTerm<'static>> {
     match query {
-        PyQuery::Id(id) => return term_from_id(id),
+        PyQuery::Id(id) => {
+            return term_from_id(id).map_err(|_| PyRuntimeError::new_err("Unknown HPO term"))
+        }
         PyQuery::Str(term_name) => {
             if term_name.starts_with("HP:") {
                 match HpoTermId::try_from(term_name.as_str()) {
-                    Ok(termid) => return term_from_id(termid.as_u32()),
+                    Ok(termid) => {
+                        return term_from_id(termid.as_u32())
+                            .map_err(|_| PyRuntimeError::new_err("Unknown HPO term"))
+                    }
                     Err(_) => {
                         return Err(PyValueError::new_err(format!("Invalid id: {}", term_name)))
                     }
                 }
             } else {
                 let ont = get_ontology()?;
                 for term in ont {
@@ -102,14 +117,20 @@
 
 #[derive(FromPyObject)]
 pub enum PyQuery {
     Id(u32),
     Str(String),
 }
 
+#[derive(FromPyObject)]
+pub enum TermOrId {
+    Term(PyHpoTerm),
+    Id(u32),
+}
+
 /// Python bindings for the Rust hpo crate
 ///
 /// This library aims to be a drop-in replacement for
 /// `pyhpo <https://pypi.org/project/pyhpo/>`_
 #[pymodule]
 fn pyhpo(py: Python, m: &PyModule) -> PyResult<()> {
     let ont = PyOntology::blank();
@@ -141,14 +162,15 @@
     Ok(())
 }
 
 fn register_set_module(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
     let child_module = PyModule::new(py, "set")?;
     child_module.add_class::<set::BasicPyHpoSet>()?;
     child_module.add_class::<set::PyHpoSet>()?;
+    child_module.add_class::<set::PhenoSet>()?;
     parent_module.add_submodule(child_module)?;
 
     py.import("sys")?
         .getattr("modules")?
         .set_item("pyhpo.set", child_module)?;
 
     Ok(())
@@ -167,14 +189,15 @@
         .set_item("pyhpo.helper", child_module)?;
     Ok(())
 }
 
 fn register_stats_module(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
     let child_module = PyModule::new(py, "stats")?;
     child_module.add_class::<PyEnrichmentModel>()?;
+    child_module.add_function(wrap_pyfunction!(linkage::linkage, child_module)?)?;
     parent_module.add_submodule(child_module)?;
 
     py.import("sys")?
         .getattr("modules")?
         .set_item("pyhpo.stats", child_module)?;
 
     Ok(())
```

### Comparing `hpo3-0.2.4/src/ontology.rs` & `hpo3-0.3.0/src/ontology.rs`

 * *Files 6% similar despite different names*

```diff
@@ -234,26 +234,30 @@
 
     /// Constructs the ontology based on provided ontology files
     ///
     /// The ontology files can be in the standard format as provided
     /// by Jax or as a binary file as generated by `hpo`
     ///
     /// Arguments
-    /// path: str
+    /// data_folder: str
     ///     Path to the source files (default: `./ontology.hpo`)
     /// binary: bool
     ///     Whether the input format is binary (default true)
-    #[pyo3(signature = (path = "", binary = true))]
-    fn __call__(&self, path: &str, binary: bool) {
-        if path.is_empty() {
+    #[pyo3(signature = (data_folder = "", from_obo_file = true))]
+    fn __call__(&self, data_folder: &str, from_obo_file: bool) {
+        if get_ontology().is_ok() {
+            println!("The Ontology has been built before already");
+            return;
+        }
+        if data_folder.is_empty() {
             from_builtin();
-        } else if binary {
-            from_binary(path);
+        } else if from_obo_file {
+            from_obo(data_folder);
         } else {
-            from_obo(path);
+            from_binary(data_folder);
         }
     }
 
     /// Returns the number of HPO-Terms in the Ontology
     ///
     /// Returns
     /// -------
```

### Comparing `hpo3-0.2.4/src/set.rs` & `hpo3-0.3.0/src/set.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 use std::collections::{HashSet, VecDeque};
 use std::num::ParseIntError;
 
 use rayon::prelude::*;
 
-use pyo3::exceptions::PyRuntimeError;
+use pyo3::exceptions::{PyAttributeError, PyRuntimeError};
 use pyo3::types::PyDict;
 use pyo3::{prelude::*, types::PyType};
 
 use hpo::annotations::AnnotationId;
 use hpo::similarity::{GroupSimilarity, StandardCombiner};
 use hpo::Ontology;
 use hpo::{term::HpoGroup, HpoSet, HpoTermId};
 
 use crate::term::PyHpoTerm;
 use crate::{
     annotations::{PyGene, PyOmimDisease},
     get_ontology,
     information_content::PyInformationContentKind,
 };
-use crate::{pyterm_from_id, term_from_query, PyQuery, term_from_id};
+use crate::{pyterm_from_id, term_from_id, term_from_query, PyQuery, TermOrId};
 
 #[pyclass(name = "HPOSet")]
 #[derive(Clone)]
 pub(crate) struct PyHpoSet {
     ids: HpoGroup,
 }
 
@@ -51,22 +51,32 @@
 ///     s = HPOSet([1, 118])
 ///     len(s)  
 ///     # >> 2
 ///
 #[pymethods]
 impl PyHpoSet {
     #[new]
-    fn new(terms: Vec<u32>) -> Self {
+    fn new(terms: Vec<TermOrId>) -> Self {
         let mut ids = HpoGroup::new();
         for id in terms {
-            ids.insert(id);
+            match id {
+                TermOrId::Id(x) => ids.insert(x),
+                TermOrId::Term(x) => ids.insert(x.hpo_term_id().as_u32()),
+            };
         }
         Self { ids }
     }
 
+    fn add(&mut self, term: TermOrId) {
+        match term {
+            TermOrId::Id(x) => self.ids.insert(x),
+            TermOrId::Term(x) => self.ids.insert(x.hpo_term_id().as_u32()),
+        };
+    }
+
     fn child_nodes(&self) -> PyResult<Self> {
         let ont = get_ontology()?;
         Ok(HpoSet::new(ont, self.ids.clone()).child_nodes().into())
     }
 
     fn remove_modifier(&self) -> PyResult<Self> {
         let ont = get_ontology()?;
@@ -174,15 +184,16 @@
         method: &str,
         combine: &str,
     ) -> PyResult<f32> {
         let ont = get_ontology()?;
         let set_a = HpoSet::new(ont, self.ids.clone());
         let set_b = HpoSet::new(ont, other.ids.clone());
 
-        let kind = PyInformationContentKind::try_from(kind)?;
+        let kind = PyInformationContentKind::try_from(kind)
+            .map_err(|_| PyAttributeError::new_err("Invalid Information content"))?;
 
         let similarity = hpo::similarity::Builtins::new(method, kind.into())
             .map_err(|_| PyRuntimeError::new_err("Unknown method to calculate similarity"))?;
         let combiner = StandardCombiner::try_from(combine)
             .map_err(|_| PyRuntimeError::new_err("Invalid combine method specified"))?;
 
         let g_sim = GroupSimilarity::new(combiner, similarity);
@@ -231,38 +242,43 @@
             .map(|sb| {
                 let set_b = HpoSet::new(ont, sb.ids.clone());
                 g_sim.calculate(&set_a, &set_b)
             })
             .collect())
     }
 
+    #[pyo3(signature = (verbose = false))]
+    #[pyo3(text_signature = "($self, verbose)")]
     #[allow(non_snake_case)]
     fn toJSON<'a>(&'a self, py: Python<'a>, verbose: bool) -> PyResult<Vec<&PyDict>> {
-        self.ids.iter().map(|id|{
-            let dict = PyDict::new(py);
-            let term = term_from_id(id.as_u32())?;
-            dict.set_item("name", term.name())?;
-            dict.set_item("id", term.id().to_string())?;
-            dict.set_item("int", term.id().as_u32())?;
-
-            if verbose {
-                let ic = PyDict::new(py);
-                ic.set_item("gene", term.information_content().gene())?;
-                ic.set_item("omim", term.information_content().omim_disease())?;
-                ic.set_item("orpha", f32::NAN)?;
-                ic.set_item("decipher", f32::NAN)?;
-                dict.set_item::<&str, Vec<&str>>("synonym", vec![])?;
-                dict.set_item("comment", "")?;
-                dict.set_item("def", "")?;
-                dict.set_item::<&str, Vec<&str>>("xref", vec![])?;
-                dict.set_item::<&str, Vec<&str>>("is_a", vec![])?;
-                dict.set_item("ic", ic)?;
-            }
-            Ok(dict)
-        }).collect()
+        self.ids
+            .iter()
+            .map(|id| {
+                let dict = PyDict::new(py);
+                let term = term_from_id(id.as_u32())?;
+                dict.set_item("name", term.name())?;
+                dict.set_item("id", term.id().to_string())?;
+                dict.set_item("int", term.id().as_u32())?;
+
+                if verbose {
+                    let ic = PyDict::new(py);
+                    ic.set_item("gene", term.information_content().gene())?;
+                    ic.set_item("omim", term.information_content().omim_disease())?;
+                    ic.set_item("orpha", 0.0)?;
+                    ic.set_item("decipher", 0.0)?;
+                    dict.set_item::<&str, Vec<&str>>("synonym", vec![])?;
+                    dict.set_item("comment", "")?;
+                    dict.set_item("definition", "")?;
+                    dict.set_item::<&str, Vec<&str>>("xref", vec![])?;
+                    dict.set_item::<&str, Vec<&str>>("is_a", vec![])?;
+                    dict.set_item("ic", ic)?;
+                }
+                Ok(dict)
+            })
+            .collect()
     }
 
     fn serialize(&self) -> String {
         let mut ids = self
             .ids
             .iter()
             .map(|tid| tid.as_u32())
@@ -273,16 +289,15 @@
         id_strings.join("+")
     }
 
     /// Returns the HPOTerms in the set
     ///
     /// TODO: Convert this to an iterator
     fn terms(&self) -> PyResult<Vec<PyHpoTerm>> {
-        self
-            .ids
+        self.ids
             .iter()
             .map(|id| pyterm_from_id(id.as_u32()))
             .collect()
     }
 
     #[classmethod]
     fn from_queries(_cls: &PyType, queries: Vec<PyQuery>) -> PyResult<Self> {
@@ -381,57 +396,62 @@
             .omim_disease(&disease.id().into())
             .expect("ontology must. be present and gene must be included")
             .to_hpo_set(ont)
             .into())
     }
 }
 
-
 #[pyclass(name = "SetIterator")]
 struct Iter {
-    ids: VecDeque<HpoTermId>
+    ids: VecDeque<HpoTermId>,
 }
 
 impl Iter {
     fn new(ids: &HpoGroup) -> Self {
-        Self { ids: ids.iter().collect() }
+        Self {
+            ids: ids.iter().collect(),
+        }
     }
 }
 
 #[pymethods]
 impl Iter {
     #[allow(clippy::self_named_constructors)]
     fn __iter__(slf: PyRef<Self>) -> PyRef<Self> {
         slf
     }
 
     fn __next__(mut slf: PyRefMut<Self>) -> Option<PyHpoTerm> {
-        slf.ids.pop_front().map(|id| pyterm_from_id(id.as_u32()).unwrap())
+        slf.ids
+            .pop_front()
+            .map(|id| pyterm_from_id(id.as_u32()).unwrap())
     }
 }
 
-
-
 #[pyclass(name = "BasicHPOSet")]
 #[derive(Clone, Default, Debug)]
 pub(crate) struct BasicPyHpoSet;
 
 impl BasicPyHpoSet {
     fn build<I: IntoIterator<Item = HpoTermId>>(ids: I) -> PyHpoSet {
         let ont = get_ontology().expect("Ontology must be initialized");
         let mut group = HpoGroup::new();
         for id in ids {
             group.insert(id);
         }
-        let mut set = HpoSet::new(ont, group);
+        let set = HpoSet::new(ont, group);
         let mut set = set.child_nodes();
         set.replace_obsolete();
         set.remove_obsolete();
         set.remove_modifier();
-        PyHpoSet::new(set.iter().map(|term| term.id().as_u32()).collect())
+        PyHpoSet::new(
+            set.iter()
+                .map(|term| TermOrId::Id(term.id().as_u32()))
+                .collect(),
+        )
     }
 }
 
 #[pymethods]
 impl BasicPyHpoSet {
     fn __call__(&self, terms: Vec<u32>) -> PyHpoSet {
         BasicPyHpoSet::build(terms.iter().map(|id| HpoTermId::from_u32(*id)))
@@ -452,9 +472,60 @@
             pickle
                 .split('+')
                 .map(|id| id.parse::<u32>())
                 .collect::<Result<Vec<u32>, ParseIntError>>()?
                 .iter()
                 .map(|id| HpoTermId::from_u32(*id)),
         ))
+    }
+}
+
+#[pyclass(name = "HPOPhenoSet")]
+#[derive(Clone, Default, Debug)]
+pub(crate) struct PhenoSet;
+
+impl PhenoSet {
+    fn build<I: IntoIterator<Item = HpoTermId>>(ids: I) -> PyHpoSet {
+        let ont = get_ontology().expect("Ontology must be initialized");
+        let mut group = HpoGroup::new();
+        for id in ids {
+            group.insert(id);
+        }
+        let mut set = HpoSet::new(ont, group);
+        set.replace_obsolete();
+        set.remove_obsolete();
+        set.remove_modifier();
+        PyHpoSet::new(
+            set.iter()
+                .map(|term| TermOrId::Id(term.id().as_u32()))
+                .collect(),
+        )
+    }
+}
+
+#[pymethods]
+impl PhenoSet {
+    fn __call__(&self, terms: Vec<u32>) -> PyHpoSet {
+        PhenoSet::build(terms.iter().map(|id| HpoTermId::from_u32(*id)))
+    }
+
+    #[classmethod]
+    fn from_queries(_cls: &PyType, queries: Vec<PyQuery>) -> PyResult<PyHpoSet> {
+        let mut ids: Vec<HpoTermId> = Vec::with_capacity(queries.len());
+        for q in queries {
+            ids.push(term_from_query(q)?.id());
+        }
+        Ok(PhenoSet::build(ids))
+    }
+
+    #[classmethod]
+    fn from_serialized(_cls: &PyType, pickle: &str) -> PyResult<PyHpoSet> {
+        Ok(PhenoSet::build(
+            pickle
+                .split('+')
+                .map(|id| id.parse::<u32>())
+                .collect::<Result<Vec<u32>, ParseIntError>>()?
+                .iter()
+                .map(|id| HpoTermId::from_u32(*id)),
+        ))
     }
 }
```

### Comparing `hpo3-0.2.4/src/term.rs` & `hpo3-0.3.0/src/term.rs`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,14 @@
             .omim_diseases()
             .fold(HashSet::new(), |mut set, disease| {
                 set.insert(PyOmimDisease::from(disease));
                 set
             })
     }
 
-
     /// A list of the phenotypical categories the term belongs to
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
@@ -474,29 +473,34 @@
     ///     term = Ontology[11968]
     ///
     ///     term.similarity_scores(list(Ontology))
     ///
     ///
     #[pyo3(signature = (others, kind = "omim", method = "graphic"))]
     #[pyo3(text_signature = "($self, others, kind, method)")]
-    fn similarity_scores(&self, others: Vec<PyHpoTerm>, kind: &str, method: &str) -> PyResult<Vec<f32>> {
+    fn similarity_scores(
+        &self,
+        others: Vec<PyHpoTerm>,
+        kind: &str,
+        method: &str,
+    ) -> PyResult<Vec<f32>> {
         let kind = PyInformationContentKind::try_from(kind)?;
 
         let term_a = self.hpo();
 
         let similarity = hpo::similarity::Builtins::new(method, kind.into())
             .map_err(|_| PyRuntimeError::new_err("Unknown method to calculate similarity"))?;
 
-    Ok(others
-        .par_iter()
-        .map(|term_b| {
-            let t2: hpo::HpoTerm = term_b.into();
-            similarity.calculate(&term_a, &t2)
-        })
-        .collect())
+        Ok(others
+            .par_iter()
+            .map(|term_b| {
+                let t2: hpo::HpoTerm = term_b.into();
+                similarity.calculate(&term_a, &t2)
+            })
+            .collect())
     }
 
     #[pyo3(signature = (verbose = false))]
     #[pyo3(text_signature = "($self, verbose)")]
     #[allow(non_snake_case)]
     pub fn toJSON<'a>(&'a self, py: Python<'a>, verbose: bool) -> PyResult<&PyDict> {
         let term = self.hpo();
@@ -505,19 +509,19 @@
         dict.set_item("id", term.id().to_string())?;
         dict.set_item("int", term.id().as_u32())?;
 
         if verbose {
             let ic = PyDict::new(py);
             ic.set_item("gene", term.information_content().gene())?;
             ic.set_item("omim", term.information_content().omim_disease())?;
-            ic.set_item("orpha", f32::NAN)?;
-            ic.set_item("decipher", f32::NAN)?;
+            ic.set_item("orpha", 0.0)?;
+            ic.set_item("decipher", 0.0)?;
             dict.set_item::<&str, Vec<&str>>("synonym", vec![])?;
             dict.set_item("comment", "")?;
-            dict.set_item("def", "")?;
+            dict.set_item("definition", "")?;
             dict.set_item::<&str, Vec<&str>>("xref", vec![])?;
             dict.set_item::<&str, Vec<&str>>("is_a", vec![])?;
             dict.set_item("ic", ic)?;
         }
         Ok(dict)
     }
```

### Comparing `hpo3-0.2.4/tests/benchmarking.py` & `hpo3-0.3.0/tests/benchmarking.py`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/tests/test_integration.py` & `hpo3-0.3.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `hpo3-0.2.4/Cargo.lock` & `hpo3-0.3.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -67,76 +67,73 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "hpo"
-version = "0.7.1"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0be120a2e5d3ff528a67320508f5bcedbe6ee92efdcef553a1cc4f631f8767cd"
+checksum = "b1ff6300a69364cd64636a5076291f56812f87923d01ef764655cb6ab79546fa"
 dependencies = [
  "aquamarine",
  "smallvec",
  "statrs",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "hpo3"
-version = "0.2.4"
+version = "0.3.0"
 dependencies = [
  "hpo",
  "once_cell",
  "pyo3",
  "rayon",
 ]
 
@@ -159,29 +156,29 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "matrixmultiply"
@@ -199,14 +196,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "memoffset"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
 name = "nalgebra"
 version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d506eb7e08d6329505faa8a3a00a5dcc6de9f76e0c77e4b75763ae3c770831ff"
 dependencies = [
  "approx",
  "matrixmultiply",
@@ -259,72 +265,72 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
+checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
@@ -350,31 +356,31 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -419,17 +425,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -496,35 +502,35 @@
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "safe_arch"
-version = "0.6.0"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
+checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "simba"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0b7840f121a46d63066ee7a99fc81dcabbc6105e437cae43528cea199b5a05f"
 dependencies = [
@@ -533,17 +539,17 @@
  "num-traits",
  "paste",
  "wide",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "statrs"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d08e5e1748192713cc281da8b16924fb46be7b0c2431854eadc785823e5696e"
 dependencies = [
@@ -563,47 +569,47 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
@@ -612,43 +618,43 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.24"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -662,80 +668,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wide"
-version = "0.7.8"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b689b6c49d6549434bf944e6b0f39238cf63693cb7a147e9d887507fffa3b223"
+checksum = "aa469ffa65ef7e0ba0f164183697b89b854253fd31aeb92358b7b6155177d62f"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
-
-[[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `hpo3-0.2.4/PKG-INFO` & `hpo3-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo3
-Version: 0.2.4
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,17 @@
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Summary: A drop-in replacement for PyHPO using a Rust backend for faster performance
 Author-email: Jonas Marcello <jonas.marcello@esbme.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Bug Tracker, https://github.com/anergictcell/hpo3/issues
 Project-URL: homepage, https://github.com/anergictcell/hpo3
 Project-URL: repository, https://github.com/anergictcell/hpo3
-Project-URL: Bug Tracker, https://github.com/anergictcell/hpo3/issues
 
 # HPO3
 
 `HPO3` is a Rust based drop-in replacement of [`PyHPO`](https://pypi.org/project/pyhpo/). It is based on the [`hpo`](https://crates.io/crates/hpo) Rust library which is a performance optimzied implementation of `PyHPO`.
 
 Using the Rust-based `hpo` library increases performance easily 100 fold for many operations. It enables developers to utilize multithreading, further improving performance greatly.
```

