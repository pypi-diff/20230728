# Comparing `tmp/pysui_fastcrypto-0.1.2.tar.gz` & `tmp/pysui_fastcrypto-0.1.3.tar.gz`

## Comparing `pysui_fastcrypto-0.1.2.tar` & `pysui_fastcrypto-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.2/Cargo.toml
--rw-r--r--   0      501       20       38 2023-07-18 11:56:07.000000 pysui_fastcrypto-0.1.2/.gitignore
--rw-r--r--   0      501       20      463 2023-07-25 12:15:55.000000 pysui_fastcrypto-0.1.2/CHANGELOG.md
--rw-r--r--   0      501       20    11357 2023-07-23 20:18:01.000000 pysui_fastcrypto-0.1.2/LICENSE
--rw-r--r--   0      501       20      115 2023-07-23 20:17:48.000000 pysui_fastcrypto-0.1.2/README.rst
--rw-r--r--   0      501       20      720 2023-07-25 11:41:22.000000 pysui_fastcrypto-0.1.2/pyproject.toml
--rw-r--r--   0      501       20       15 2023-07-23 20:45:50.000000 pysui_fastcrypto-0.1.2/requirements.txt
--rw-r--r--   0      501       20    18008 2023-07-25 12:12:46.000000 pysui_fastcrypto-0.1.2/src/lib.rs
--rw-r--r--   0      501       20    54346 2023-07-25 11:42:02.000000 pysui_fastcrypto-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20       38 2023-07-18 11:56:07.000000 pysui_fastcrypto-0.1.3/.gitignore
+-rw-r--r--   0      501       20      839 2023-07-26 19:01:11.000000 pysui_fastcrypto-0.1.3/CHANGELOG.md
+-rw-r--r--   0      501       20    11357 2023-07-23 20:18:01.000000 pysui_fastcrypto-0.1.3/LICENSE
+-rw-r--r--   0      501       20      143 2023-07-25 20:14:51.000000 pysui_fastcrypto-0.1.3/README.rst
+-rw-r--r--   0      501       20      720 2023-07-25 11:41:22.000000 pysui_fastcrypto-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20       15 2023-07-23 20:45:50.000000 pysui_fastcrypto-0.1.3/requirements.txt
+-rw-r--r--   0      501       20    18016 2023-07-26 19:07:58.000000 pysui_fastcrypto-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20    54330 2023-07-25 19:44:38.000000 pysui_fastcrypto-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.1.3/PKG-INFO
```

### Comparing `pysui_fastcrypto-0.1.2/Cargo.toml` & `pysui_fastcrypto-0.1.3/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [package]
 name = "pysui-fastcrypto"
-version = "0.1.2"
+version = "0.1.3"
 license = "Apache-2.0"
 edition = "2021"
 
 [lib]
 name = "pysui_fastcrypto"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "1.0.71"
 base64ct = "1.6.0"
 bip32 = "0.5.1"
 fastcrypto = "0.1.5"
-lazy_static = "1.4.0"
 slip10_ed25519 = "0.1.3"
 tiny-bip39 = "1.0.0"
 
 [dependencies.pyo3]
 version = "0.19.0"
 # "abi3-py37" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.10
 features = ["abi3-py310"]
```

### Comparing `pysui_fastcrypto-0.1.2/LICENSE` & `pysui_fastcrypto-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysui_fastcrypto-0.1.2/pyproject.toml` & `pysui_fastcrypto-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysui_fastcrypto-0.1.2/src/lib.rs` & `pysui_fastcrypto-0.1.3/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -7,19 +7,15 @@
     ed25519::{Ed25519KeyPair, Ed25519PrivateKey, Ed25519PublicKey},
     hash::{Blake2b256, HashFunction},
     secp256k1::{Secp256k1KeyPair, Secp256k1PrivateKey, Secp256k1PublicKey},
     secp256r1::{Secp256r1KeyPair, Secp256r1PrivateKey, Secp256r1PublicKey},
     traits::{KeyPair, Signer, ToFromBytes},
 };
 use slip10_ed25519::derive_ed25519_private_key;
-use std::{
-    collections::{BTreeMap, VecDeque},
-    str::FromStr,
-    sync::Mutex,
-};
+use std::{collections::VecDeque, str::FromStr};
 
 use pyo3::prelude::*;
 
 type LibError = anyhow::Error;
 pub type DefaultHash = Blake2b256;
 const DERIVATION_PATH_COIN_TYPE: u32 = 784;
 const DERVIATION_PATH_PURPOSE_ED25519: u32 = 44;
@@ -66,15 +62,15 @@
 
     fn encode<T: AsRef<[u8]>>(data: T) -> String {
         base64ct::Base64::encode_string(data.as_ref())
     }
 }
 
 /// Signature Schemes supported by Sui
-#[derive(Debug, PartialEq, Eq)]
+#[derive(Clone, Debug, PartialEq, Eq)]
 pub enum SignatureScheme {
     ED25519,
     Secp256k1,
     Secp256r1,
     BLS12381, // This is currently not supported for user Sui Address.
     MultiSig,
     ZkLoginAuthenticator,
@@ -165,53 +161,54 @@
     fn scheme(&self) -> SignatureScheme {
         match self {
             SuiKeyPair::Ed25519(_) => SignatureScheme::ED25519,
             SuiKeyPair::Secp256k1(_) => SignatureScheme::Secp256k1,
             SuiKeyPair::Secp256r1(_) => SignatureScheme::Secp256r1,
         }
     }
-    fn duplicate(&self) -> SuiKeyPair {
+
+    /// Get the private key bytes
+    fn as_bytes(&self) -> Vec<u8> {
         match self {
-            SuiKeyPair::Ed25519(kp) => {
-                SuiKeyPair::Ed25519(Ed25519KeyPair::from_bytes(kp.as_bytes()).unwrap())
-            }
-            SuiKeyPair::Secp256k1(kp) => {
-                SuiKeyPair::Secp256k1(Secp256k1KeyPair::from_bytes(kp.as_bytes()).unwrap())
-            }
-            SuiKeyPair::Secp256r1(kp) => {
-                SuiKeyPair::Secp256r1(Secp256r1KeyPair::from_bytes(kp.as_bytes()).unwrap())
-            }
+            SuiKeyPair::Ed25519(kp) => kp.as_bytes().to_vec(),
+            SuiKeyPair::Secp256k1(kp) => kp.as_bytes().to_vec(),
+            SuiKeyPair::Secp256r1(kp) => kp.as_bytes().to_vec(),
         }
     }
 }
 
-/// Given a keystring, produce a keypair
-fn keypair_from_keystring(keystring: String) -> Result<SuiKeyPair, LibError> {
-    let b64b = &mut VecDeque::from(Base64::decode(&keystring).unwrap());
-    let kscheme = SignatureScheme::from_flag_byte(&b64b.pop_front().unwrap()).unwrap();
-    let rembytes = b64b.make_contiguous();
+/// Construct a SuiKeyPair from seed
+fn kp_from_bytes(kscheme: SignatureScheme, seed: &[u8]) -> Result<SuiKeyPair, LibError> {
     match kscheme {
         SignatureScheme::ED25519 => Ok(SuiKeyPair::Ed25519(
-            Ed25519KeyPair::from_bytes(rembytes).unwrap(),
+            Ed25519KeyPair::from_bytes(seed).unwrap(),
         )),
         SignatureScheme::Secp256k1 => Ok(SuiKeyPair::Secp256k1(
-            Secp256k1KeyPair::from_bytes(rembytes).unwrap(),
+            Secp256k1KeyPair::from_bytes(seed).unwrap(),
         )),
         SignatureScheme::Secp256r1 => Ok(SuiKeyPair::Secp256r1(
-            Secp256r1KeyPair::from_bytes(rembytes).unwrap(),
+            Secp256r1KeyPair::from_bytes(seed).unwrap(),
         )),
         SignatureScheme::BLS12381
         | SignatureScheme::MultiSig
         | SignatureScheme::ZkLoginAuthenticator => Err(anyhow!(format!(
             "key derivation not supported {:?}",
             kscheme
         ))),
     }
 }
 
+/// Given a keystring, produce a keypair
+fn keypair_from_keystring(keystring: String) -> Result<(SignatureScheme, SuiKeyPair), LibError> {
+    let b64b = &mut VecDeque::from(Base64::decode(&keystring)?);
+    let kscheme = SignatureScheme::from_flag_byte(&b64b.pop_front().unwrap())?;
+    let rembytes = b64b.make_contiguous();
+    Ok((kscheme.clone(), kp_from_bytes(kscheme, &rembytes)?))
+}
+
 pub fn validate_path(
     key_scheme: &SignatureScheme,
     path: Option<DerivationPath>,
 ) -> Result<DerivationPath, LibError> {
     match key_scheme {
         SignatureScheme::ED25519 => {
             match path.clone() {
@@ -352,28 +349,44 @@
 }
 
 /// Generate a new keypair with derivation path and optional mnemonic word lengths for phrase
 fn new_keypair(
     scheme: u8,
     derivation_path: Option<String>,
     word_length: Option<String>,
-) -> Result<(SignatureScheme, String, SuiKeyPair)> {
+) -> Result<(String, SuiKeyPair)> {
     let scheme = SignatureScheme::from_flag_byte(&scheme).unwrap();
     let dvpath = match derivation_path {
         Some(s) => Some(DerivationPath::from_str(&s).unwrap()),
         None => None,
     };
     let mnemonic = Mnemonic::new(parse_word_length(word_length).unwrap(), Language::English);
     let seed = Seed::new(&mnemonic, "");
     match derive_key_pair_from_path(seed.as_bytes(), dvpath, &scheme) {
-        Ok(kp) => Ok((scheme, mnemonic.phrase().to_string(), kp)),
+        Ok(kp) => Ok((mnemonic.phrase().to_string(), kp)),
         Err(e) => Err(anyhow!("Failed to generate keypair: {:?}", e)),
     }
 }
 
+/// Generate a new keypair with derivation path and mnemonic phrase
+fn recover_keypair(scheme: u8, derivation_path: String, phrase: String) -> Result<SuiKeyPair> {
+    let scheme = SignatureScheme::from_flag_byte(&scheme).unwrap();
+    let dvpath = Some(DerivationPath::from_str(&derivation_path).unwrap());
+    // let mnemonic = Mnemonic::from_phrase(&phrase, Language::English);
+    match Mnemonic::from_phrase(&phrase, Language::English) {
+        Ok(mnemonic) => {
+            let seed = Seed::new(&mnemonic, "");
+            match derive_key_pair_from_path(seed.as_bytes(), dvpath, &scheme) {
+                Ok(kp) => Ok(kp),
+                Err(e) => Err(anyhow!("Failed to recover keypair: {:?}", e)),
+            }
+        }
+        Err(e) => Err(anyhow!("Recovery phrash failed: {:?}", e)),
+    }
+}
 /// Find the word length for the mnemonic phrase
 fn parse_word_length(s: Option<String>) -> Result<MnemonicType, anyhow::Error> {
     match s {
         None => Ok(MnemonicType::Words12),
         Some(s) => match s.as_str() {
             "12" => Ok(MnemonicType::Words12),
             "15" => Ok(MnemonicType::Words15),
@@ -381,73 +394,55 @@
             "21" => Ok(MnemonicType::Words21),
             "24" => Ok(MnemonicType::Words24),
             _ => anyhow::bail!("Invalid word length"),
         },
     }
 }
 
-static GLOBAL_DATA: Mutex<BTreeMap<String, SuiKeyPair>> =
-    Mutex::new(BTreeMap::<String, SuiKeyPair>::new());
-
-/// Store a keypair associated to the hashed public key.
-///
-/// Throws error if key/token already exists
-fn store_key(key_pair: SuiKeyPair) -> Result<(Vec<u8>, String), LibError> {
-    // Hash the public key bytes
-    let key_bytes = key_pair.pubkey().as_bytes();
-    let mut hasher = DefaultHash::default();
-    hasher.update(key_bytes.clone());
-    // Stringify the token and use as key to keypair
-    let mut map = GLOBAL_DATA.lock().unwrap();
-    let token = Base64::encode(hasher.finalize().digest);
-    if map.contains_key(&token) {
-        return Err(anyhow!(format!("Failed to generate keypair: {:?}", token)));
-    }
-    map.insert(token.clone(), key_pair);
-    Ok((key_bytes, token))
-}
-
-/// Get a duplicate of the keypair from token
-fn keypair_from_token(token: &String) -> Result<SuiKeyPair, LibError> {
-    let map = GLOBAL_DATA.lock().unwrap();
-    if let Some(kp) = map.get(token) {
-        return Ok(kp.duplicate());
-    }
-    Err(anyhow!(format!("Token {} not found", token)))
-}
-
 /// Returns a keystrings scheme, public key bytes and a token from a Sui keystring.
 /// Assumes that the inbound keystring is valid (e.g. `flag | private_key bytes`)
 #[pyfunction]
-fn keys_from_keystring(in_str: String) -> (u8, Vec<u8>, String) {
+fn keys_from_keystring(in_str: String) -> (u8, Vec<u8>, Vec<u8>) {
     assert!(in_str.len() != 0, "Requires valid keystring");
-    let kp = keypair_from_keystring(in_str).unwrap();
-    let scheme = kp.scheme().flag();
-    let (pub_key, token) = store_key(kp).unwrap();
-    (scheme, pub_key, token)
+    let (scheme, kp) = keypair_from_keystring(in_str).unwrap();
+    (scheme.flag(), kp.pubkey().as_bytes(), kp.as_bytes())
 }
 
-/// Returns a new keystrings scheme, public key bytes and a token./// Assumes that the inbound keystring is valid (e.g. `flag | private_key bytes`)
+/// Returns a new keystrings scheme, public and private key bytes and a token.
+/// Assumes that the inbound keystring is valid (e.g. `flag | private_key bytes`)
 #[pyfunction]
 fn generate_new_keypair(
     in_scheme: u8,
     derv_path: Option<String>,
     word_count: Option<String>,
-) -> (u8, String, Vec<u8>, String) {
-    let (scheme, phrase, kp) = new_keypair(in_scheme, derv_path, word_count).unwrap();
-    // Hash the public key
-    let (pub_key, token) = store_key(kp).unwrap();
-    (scheme.flag(), phrase, pub_key, token)
+) -> (String, Vec<u8>, Vec<u8>) {
+    let (phrase, kp) = new_keypair(in_scheme, derv_path, word_count).unwrap();
+    (phrase, kp.pubkey().as_bytes(), kp.as_bytes())
 }
 
+/// Returns keystrings scheme, public and private key bytes from mnemonic phrase and derivation path
+#[pyfunction]
+fn keys_from_mnemonics(scheme: u8, derivation_path: String, phrase: String) -> (Vec<u8>, Vec<u8>) {
+    let kp = recover_keypair(scheme, derivation_path, phrase).unwrap();
+    (kp.pubkey().as_bytes(), kp.as_bytes())
+}
 /// Signs a message with optional intent, otherwise default is used
 /// The in_data string is the tx_bytes string
 #[pyfunction]
-fn sign_digest(token: String, in_data: String, intent: Option<Vec<u8>>) -> Vec<u8> {
-    let kp = keypair_from_token(&token).unwrap();
+fn sign_digest(
+    in_scheme: u8,
+    prv_bytes: Vec<u8>,
+    in_data: String,
+    intent: Option<Vec<u8>>,
+) -> Vec<u8> {
+    let kp = kp_from_bytes(
+        SignatureScheme::from_flag_byte(&in_scheme).unwrap(),
+        &prv_bytes,
+    )
+    .unwrap();
     let intent_msg = match intent {
         Some(inv) => inv,
         None => vec![0, 0, 0],
     };
     let mut hasher = DefaultHash::default();
     hasher.update(intent_msg);
     hasher.update(Base64::decode(&in_data).unwrap());
@@ -459,12 +454,13 @@
 }
 
 /// The pysui_fastcrypto module implemented in Rust.  In order
 /// to import the function name must match the Cargo.toml name
 #[pymodule]
 fn pysui_fastcrypto(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(keys_from_keystring, m)?)?;
+    m.add_function(wrap_pyfunction!(keys_from_mnemonics, m)?)?;
     m.add_function(wrap_pyfunction!(generate_new_keypair, m)?)?;
     m.add_function(wrap_pyfunction!(sign_digest, m)?)?;
 
     Ok(())
 }
```

### Comparing `pysui_fastcrypto-0.1.2/Cargo.lock` & `pysui_fastcrypto-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1407,21 +1407,20 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pysui-fastcrypto"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "base64ct",
  "bip32",
  "fastcrypto",
- "lazy_static",
  "pyo3",
  "slip10_ed25519",
  "tiny-bip39",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pysui_fastcrypto-0.1.2/PKG-INFO` & `pysui_fastcrypto-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pysui-fastcrypto
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 License-File: LICENSE
 Summary: Python wrapper for MystenLab/fastcrypto Rust crate
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
 Project-URL: homepage, https://github.com/FrankC01/pysui-fastcrypto
 Project-URL: repository, https://github.com/FrankC01/pysui-fastcrypto
 Project-URL: changelog, https://github.com/FrankC01/pysui-fastcrypto/blob/main/CHANGELOG.md
 
 pysui-fastcrypto
 ================
 
-pysui-fastcrypto is a wrapper around MytenLab/fastcrypto. It is used by `pysui`
+pysui-fastcrypto is a Python wrapper for `MytenLab/fastcrypto <https://github.com/MystenLabs/fastcrypto>`_.
```

