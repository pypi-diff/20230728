# Comparing `tmp/gridworks_cert-0.2.0.tar.gz` & `tmp/gridworks_cert-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_cert-0.2.0.tar", max compression
+gzip compressed data, was "gridworks_cert-0.3.0.tar", max compression
```

## Comparing `gridworks_cert-0.2.0.tar` & `gridworks_cert-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-21 15:12:20.887634 gridworks_cert-0.2.0/LICENSE
--rw-r--r--   0        0        0     3822 2023-07-21 15:12:20.887634 gridworks_cert-0.2.0/README.md
--rw-r--r--   0        0        0     2081 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/__init__.py
--rw-r--r--   0        0        0      455 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/__main__.py
--rw-r--r--   0        0        0       99 2023-07-21 15:12:20.891634 gridworks_cert-0.2.0/src/gwcert/ca/__init__.py
--rw-r--r--   0        0        0     7319 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/ca/__main__.py
--rw-r--r--   0        0        0      101 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/key/__init__.py
--rw-r--r--   0        0        0    19855 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/key/__main__.py
--rw-r--r--   0        0        0      196 2023-07-21 15:12:37.475856 gridworks_cert-0.2.0/src/gwcert/paths.py
--rw-r--r--   0        0        0        0 2023-07-21 15:12:20.891634 gridworks_cert-0.2.0/src/gwcert/py.typed
--rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 gridworks_cert-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3837 2023-07-27 23:18:42.450132 gridworks_cert-0.3.0/README.md
+-rw-r--r--   0        0        0     2081 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/__init__.py
+-rw-r--r--   0        0        0      455 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/ca/__init__.py
+-rw-r--r--   0        0        0     7416 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/src/gwcert/ca/__main__.py
+-rw-r--r--   0        0        0      172 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/src/gwcert/key/__init__.py
+-rw-r--r--   0        0        0    21478 2023-07-27 23:18:42.454132 gridworks_cert-0.3.0/src/gwcert/key/__main__.py
+-rw-r--r--   0        0        0      196 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/paths.py
+-rw-r--r--   0        0        0        0 2023-07-27 23:18:23.041003 gridworks_cert-0.3.0/src/gwcert/py.typed
+-rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 gridworks_cert-0.3.0/PKG-INFO
```

### Comparing `gridworks_cert-0.2.0/LICENSE` & `gridworks_cert-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.2.0/README.md` & `gridworks_cert-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [![PyPI](https://img.shields.io/pypi/v/gridworks-cert.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/gridworks-cert.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/gridworks-cert)][python version]
 [![License](https://img.shields.io/pypi/l/gridworks-cert)][license]
 
 [![Read the documentation at https://gridworks-cert.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-cert/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/anschweitzer/gridworks-cert/workflows/Tests/badge.svg)][tests]
-[![Codecov](https://codecov.io/gh/anschweitzer/gridworks-cert/branch/main/graph/badge.svg)][codecov]
+[![Tests](https://github.com/thegridelectric/gridworks-cert/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-cert/branch/main/graph/badge.svg)][codecov]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 Tools for creating TLS certificates for use with, e.g. MQTT and RabbitMQ.
 
 **NOTE**: these are temporary tools for _non-production_ deployments. This library is more or less equivalent to a README
@@ -82,15 +82,15 @@
 ## Credits
 
 This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
 
 [@cjolowicz]: https://github.com/cjolowicz
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
-[file an issue]: https://github.com/anschweitzer/gridworks-cert/issues
+[file an issue]: https://github.com/thegridelectric/gridworks-cert/issues
 [pip]: https://pip.pypa.io/
 [pypi_]: https://pypi.org/project/gridworks-cert/
 [status]: https://pypi.org/project/gridworks-cert/
 [python version]: https://pypi.org/project/gridworks-cert
 [read the docs]: https://gridworks-cert.readthedocs.io/
 [tests]: https://github.com/thegridelectric/gridworks-cert/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-cert
@@ -100,10 +100,10 @@
 [ownca]: https://ownca.readthedocs.io/en/latest/
 [pyca/cryptography]: https://cryptography.io/en/latest/
 [openssl]: https://www.openssl.org/
 [rabbitmq]: https://rabbitmq.com/ssl.html#automated-certificate-generation-transcript
 
 <!-- github-only -->
 
-[license]: https://github.com/anschweitzer/gridworks-cert/blob/main/LICENSE
-[contributor guide]: https://github.com/anschweitzer/gridworks-cert/blob/main/CONTRIBUTING.md
+[license]: https://github.com/thegridelectric/gridworks-cert/blob/main/LICENSE
+[contributor guide]: https://github.com/thegridelectric/gridworks-cert/blob/main/CONTRIBUTING.md
 [command-line reference]: https://gridworks-cert.readthedocs.io/en/latest/usage.html
```

### Comparing `gridworks_cert-0.2.0/pyproject.toml` & `gridworks_cert-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-cert"
-version = "0.2.0"
+version = "0.3.0"
 description = "gwcert"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/anschweitzer/gridworks-cert"
 repository = "https://github.com/anschweitzer/gridworks-cert"
 documentation = "https://gridworks-cert.readthedocs.io"
```

### Comparing `gridworks_cert-0.2.0/src/gwcert/ca/__main__.py` & `gridworks_cert-0.3.0/src/gwcert/ca/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
             f"  {description:30s}    Exists:{str(file_path.exists()):5s}  {str(file_path)}"
         )
     named_keys = ca.certificates
     named_key_dir = ca_dir / CA_CERTS_DIR
     print(f" Named keys in {named_key_dir}: {len(named_keys)} ")
     for named_key in named_keys:
         print(f"  {named_key}")
+        for path in (named_key_dir / named_key).iterdir():
+            print(f"    {str(path)}")
 
 
 @app.command()
 def create(
     common_name: Annotated[
         str, typer.Argument(help="Certificate Authority Common Name when issuing cert.")
     ],
```

### Comparing `gridworks_cert-0.2.0/src/gwcert/key/__main__.py` & `gridworks_cert-0.3.0/src/gwcert/key/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Commands for gwcert.ca package."""
 import datetime
+import subprocess
 import uuid
 from pathlib import Path
 from typing import Annotated
 from typing import List
 from typing import Optional
 
+import rich
 import typer
 from cryptography import x509
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa as crypto_rsa
 from cryptography.x509.oid import NameOID
-from rich import print
 
 from gwcert import DEFAULT_CA_DIR
 from gwcert.paths import DEFAULT_CERTS_DIR
 
 
 app = typer.Typer(
     no_args_is_help=True,
@@ -46,15 +47,15 @@
     """,
 )
 
 _INVALID_PATHS = [Path("."), Path("..")]
 CWD = Path(".")
 
 
-def _get_output_path(
+def get_output_path(
     name_or_output_path: str, output_suffix: str, certs_dir: Path = CWD
 ) -> Path:
     """
     Return an output of the form certs_dir/name_or_output_path/name_or_output_path.suffix, unless name_or_output_path
     contains parent directories, in which case the return value is Path(name_or_output_path).
 
     Output path construction, when performed, is:
@@ -149,44 +150,44 @@
     Writes public and private key files, by default named:
 
         $HOME/.local/share/gridworks/ca/certs/name/name.pub
         $HOME/.local/share/gridworks/ca/certs/name/name.pem
 
     Output files can be explicitly named by passing a path-like string for a ".pem" file to the name parameter.
     """
-    private_key_path = _get_output_path(
+    private_key_path = get_output_path(
         name_or_output_path=name, output_suffix=".pem", certs_dir=certs_dir
     )
     public_key_path = private_key_path.with_suffix(".pub")
     if not force and (private_key_path.exists() or public_key_path.exists()):
-        print(
+        rich.print(
             "One or more output files [yellow][bold]already exist. Doing nothing.[/yellow][/bold]"
         )
-        print(
+        rich.print(
             f"  private key file  exists:{str(private_key_path.exists()):5s}  {private_key_path}"
         )
-        print(
+        rich.print(
             f"  public key file   exists:{str(private_key_path.exists()):5s}  {private_key_path}"
         )
-        print("\nUse --force to overwrite keys")
+        rich.print("\nUse --force to overwrite keys")
         return
     key = crypto_rsa.generate_private_key(
         public_exponent=public_exponent, key_size=key_size
     )
-    print(f"Writing private key file: {private_key_path}")
+    rich.print(f"Writing private key file: {private_key_path}")
     _store_file(
         private_key_path,
         key.private_bytes(
             serialization.Encoding.PEM,
             serialization.PrivateFormat.PKCS8,
             serialization.NoEncryption(),
         ),
         0o600,
     )
-    print(f"Writing public key file:  {public_key_path}")
+    rich.print(f"Writing public key file:  {public_key_path}")
     _store_file(
         public_key_path,
         key.public_key().public_bytes(
             serialization.Encoding.OpenSSH,
             serialization.PublicFormat.OpenSSH,
         ),
     )
@@ -242,36 +243,39 @@
 
         $HOME/.local/share/gridworks/ca/certs/name/name.csr
 
     Input file can be explicitly named with the --private-key-path paramter.
     Output file can be explicitly named by passing a path-like string for a ".csr" file to the name parameter.
 
     """
-    csr_path = _get_output_path(
+    csr_path = get_output_path(
         name_or_output_path=name, output_suffix=".csr", certs_dir=certs_dir
     )
     if not force and csr_path.exists():
-        print(
+        rich.print(
             f"CSR file {csr_path} [yellow][bold]already exists. Doing nothing.[/yellow][/bold]"
         )
-        print("\nUse --force to overwrite csr file")
+        rich.print("\nUse --force to overwrite csr file")
         return
     if private_key_path is None:
         private_key_path = csr_path.with_suffix(".pem")
 
     if not private_key_path.exists():
         raise ValueError(f"Private key path {private_key_path} does not exist")
 
     with private_key_path.open("rb") as f:
         key = serialization.load_pem_private_key(f.read(), password=None)
 
+    if not common_name:
+        common_name = csr_path.stem
+
     if not dns_names:
         dns_names = [common_name]
 
-    print(f"Writing CSR file:         {csr_path}")
+    rich.print(f"Writing CSR file:         {csr_path}")
     _store_file(
         csr_path,
         x509.CertificateSigningRequestBuilder()  # type: ignore
         .subject_name(x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, common_name)]))  # type: ignore
         .add_extension(
             x509.SubjectAlternativeName(
                 [x509.DNSName(dns_name) for dns_name in dns_names]
@@ -349,55 +353,55 @@
     Writes a certificate file, by default named:
 
         $HOME/.local/share/gridworks/ca/certs/name/name.crt
 
     Input file can be explicitly named with the --csr-path, --ca-certificate-path and --ca-private-key-path parameters.
     Output file can be explicitly named by passing a path-like string for a ".crt" file to the name parameter.
     """
-    certificate_path = _get_output_path(name, ".crt", certs_dir)
+    certificate_path = get_output_path(name, ".crt", certs_dir)
     if csr_path is None:
         csr_path = certificate_path.with_suffix(".csr")
     if ca_certificate_path is None:
         ca_certificate_path = ca_dir / "ca.crt"
     if ca_private_key_path is None:
         ca_private_key_path = ca_dir / "private" / "ca_key.pem"
 
     if not force and certificate_path.exists():
-        print(
+        rich.print(
             f"Ceritifcate file {certificate_path} [yellow][bold]already exists. Doing nothing.[/yellow][/bold]"
         )
-        print("\nUse --force to overwrite certificate file")
+        rich.print("\nUse --force to overwrite certificate file")
         return
     if not csr_path.exists():
         raise ValueError(f"CSR path {csr_path} does not exist")
     if not ca_certificate_path.exists():
         raise ValueError(f"CA certificate path {ca_certificate_path} does not exist")
     if not ca_private_key_path.exists():
         raise ValueError(f"CA private key path {ca_private_key_path} does not exist")
 
     with csr_path.open("rb") as f:
-        csr = x509.load_pem_x509_csr(f.read())
+        csr_ = x509.load_pem_x509_csr(f.read())
     with ca_certificate_path.open("rb") as f:
         ca_certificate = x509.load_pem_x509_certificate(f.read())
     with ca_private_key_path.open("rb") as f:
         ca_key = serialization.load_pem_private_key(f.read(), password=None)
 
-    certificate_builder: x509.CertificateBuilder = x509.CertificateBuilder().subject_name(csr.subject)  # type: ignore
-    for extension in csr.extensions:
+    certificate_builder: x509.CertificateBuilder = x509.CertificateBuilder().subject_name(csr_.subject)  # type: ignore
+    for extension in csr_.extensions:
         if extension.value.oid._name != "subjectAltName":  # noqa
             continue
         certificate_builder = certificate_builder.add_extension(
             extension.value, critical=extension.critical
         )
 
-    print(f"Writing certificate file: {certificate_path}")
+    rich.print(f"Writing certificate file: {certificate_path}")
     _store_file(
         certificate_path,
         certificate_builder.issuer_name(ca_certificate.subject)
-        .public_key(csr.public_key())
+        .public_key(csr_.public_key())
         .serial_number(uuid.uuid4().int)
         .not_valid_before(datetime.datetime.today() - datetime.timedelta(1, 0, 0))
         .not_valid_after(
             datetime.datetime.today() + (datetime.timedelta(1, 0, 0) * valid_days)
         )
         .add_extension(
             x509.KeyUsage(
@@ -426,14 +430,59 @@
             algorithm=hashes.SHA256(),
         )
         .public_bytes(encoding=serialization.Encoding.PEM),
     )
 
 
 @app.command()
+def info(
+    name: Annotated[
+        str,
+        typer.Argument(
+            help="'name' of generated certificate, or explict path to generated crt file."
+        ),
+    ],
+    certs_dir: Annotated[
+        Path, typer.Option(help="Base storage directory for named certs")
+    ] = DEFAULT_CERTS_DIR,
+    show_files: Annotated[
+        bool,
+        typer.Option(
+            "--files", help="Show paths of files in directory of certificate."
+        ),
+    ] = False,
+) -> None:
+    """Show information about a certificate using '[cyan]openssl x509 -in CERTIFICATE_PATH -text -noout[/cyan]'."""
+    certificate_path = get_output_path(
+        name_or_output_path=name, output_suffix=".crt", certs_dir=certs_dir
+    )
+    rich.print(f"Showing information for certificate {certificate_path}")
+    if show_files:
+        cert_dir = certificate_path.parent
+        rich.print(f"Files for certificate {certificate_path.stem}")
+        for path in cert_dir.iterdir():
+            rich.print(f" {path}")
+    cmd = [
+        "openssl",
+        "x509",
+        "-in",
+        str(certificate_path),
+        "-text",
+        "-noout",
+    ]
+    rich.print(f"Running command:\n\n\t{' '.join(cmd)}\n")
+    result = subprocess.run(cmd, capture_output=True)
+    print(result.stdout.decode("utf-8"))
+    if result.returncode != 0:
+        raise RuntimeError(
+            f"ERROR. Command <{' '.join(cmd)}> failed with returncode:{result.returncode}"
+        )
+
+
+@app.command()
 def add(
     ctx: typer.Context,
     name: Annotated[
         str,
         typer.Argument(
             help="'name' of generated identity, or explict path to generated private key file."
         ),
@@ -522,44 +571,44 @@
         $HOME/.local/share/gridworks/ca/certs/name/name.csr
         $HOME/.local/share/gridworks/ca/certs/name/name.crt
 
     Input file can be explicitly named with the --ca-certificate-path and --ca-private-key-path parameters.
     Output file can be explicitly named by passing a path-like string for a ".pem" file to the name parameter and/or
     with --csr-path and --certificate-path parameters.
     """
-    private_key_path = _get_output_path(
+    private_key_path = get_output_path(
         name_or_output_path=name, output_suffix=".pem", certs_dir=certs_dir
     )
     public_key_path = private_key_path.with_suffix(".pub")
     if csr_path is None:
         csr_path = private_key_path.with_suffix(".csr")
     if certificate_path is None:
         certificate_path = private_key_path.with_suffix(".crt")
     if not force and (
         private_key_path.exists()
         or public_key_path.exists()
         or csr_path.exists()
         or certificate_path.exists()
     ):
-        print(
+        rich.print(
             "One or more output files [yellow][bold]already exist. Doing nothing.[/yellow][/bold]"
         )
-        print(
+        rich.print(
             f"  private key file  exists:{str(private_key_path.exists()):5s}  {private_key_path}"
         )
-        print(
+        rich.print(
             f"  public key file   exists:{str(private_key_path.exists()):5s}  {private_key_path}"
         )
-        print(
+        rich.print(
             f"  CSR file          exists:{str(csr_path.exists()):5s}  {private_key_path}"
         )
-        print(
+        rich.print(
             f"  Certificate file  exists:{str(certificate_path.exists()):5s}  {private_key_path}"
         )
-        print("\nUse --force to overwrite keys")
+        rich.print("\nUse --force to overwrite keys")
         return
     ctx.invoke(
         rsa,
         name=name,
         certs_dir=certs_dir,
         public_exponent=public_exponent,
         key_size=key_size,
```

### Comparing `gridworks_cert-0.2.0/PKG-INFO` & `gridworks_cert-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-cert
-Version: 0.2.0
+Version: 0.3.0
 Summary: gwcert
 Home-page: https://github.com/anschweitzer/gridworks-cert
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -26,16 +26,16 @@
 
 [![PyPI](https://img.shields.io/pypi/v/gridworks-cert.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/gridworks-cert.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/gridworks-cert)][python version]
 [![License](https://img.shields.io/pypi/l/gridworks-cert)][license]
 
 [![Read the documentation at https://gridworks-cert.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-cert/latest.svg?label=Read%20the%20Docs)][read the docs]
-[![Tests](https://github.com/anschweitzer/gridworks-cert/workflows/Tests/badge.svg)][tests]
-[![Codecov](https://codecov.io/gh/anschweitzer/gridworks-cert/branch/main/graph/badge.svg)][codecov]
+[![Tests](https://github.com/thegridelectric/gridworks-cert/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-cert/branch/main/graph/badge.svg)][codecov]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 Tools for creating TLS certificates for use with, e.g. MQTT and RabbitMQ.
 
 **NOTE**: these are temporary tools for _non-production_ deployments. This library is more or less equivalent to a README
@@ -106,15 +106,15 @@
 ## Credits
 
 This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
 
 [@cjolowicz]: https://github.com/cjolowicz
 [pypi]: https://pypi.org/
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
-[file an issue]: https://github.com/anschweitzer/gridworks-cert/issues
+[file an issue]: https://github.com/thegridelectric/gridworks-cert/issues
 [pip]: https://pip.pypa.io/
 [pypi_]: https://pypi.org/project/gridworks-cert/
 [status]: https://pypi.org/project/gridworks-cert/
 [python version]: https://pypi.org/project/gridworks-cert
 [read the docs]: https://gridworks-cert.readthedocs.io/
 [tests]: https://github.com/thegridelectric/gridworks-cert/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-cert
@@ -124,11 +124,11 @@
 [ownca]: https://ownca.readthedocs.io/en/latest/
 [pyca/cryptography]: https://cryptography.io/en/latest/
 [openssl]: https://www.openssl.org/
 [rabbitmq]: https://rabbitmq.com/ssl.html#automated-certificate-generation-transcript
 
 <!-- github-only -->
 
-[license]: https://github.com/anschweitzer/gridworks-cert/blob/main/LICENSE
-[contributor guide]: https://github.com/anschweitzer/gridworks-cert/blob/main/CONTRIBUTING.md
+[license]: https://github.com/thegridelectric/gridworks-cert/blob/main/LICENSE
+[contributor guide]: https://github.com/thegridelectric/gridworks-cert/blob/main/CONTRIBUTING.md
 [command-line reference]: https://gridworks-cert.readthedocs.io/en/latest/usage.html
```

