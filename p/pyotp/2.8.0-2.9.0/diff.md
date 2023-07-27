# Comparing `tmp/pyotp-2.8.0.tar.gz` & `tmp/pyotp-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyotp-2.8.0.tar", last modified: Wed Dec 14 03:54:21 2022, max compression
+gzip compressed data, was "pyotp-2.9.0.tar", last modified: Thu Jul 27 23:40:52 2023, max compression
```

## Comparing `pyotp-2.8.0.tar` & `pyotp-2.9.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2022-12-14 03:54:21.049550 pyotp-2.8.0/
--rw-r--r--   0 kislyuk    (501) staff       (20)     1174 2022-09-11 18:31:53.000000 pyotp-2.8.0/LICENSE
--rw-r--r--   0 kislyuk    (501) staff       (20)       51 2022-09-11 18:31:53.000000 pyotp-2.8.0/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)     8758 2022-12-14 03:54:21.049833 pyotp-2.8.0/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     7868 2022-12-14 03:34:30.000000 pyotp-2.8.0/README.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)       80 2022-09-11 18:53:33.000000 pyotp-2.8.0/pyproject.toml
--rw-r--r--   0 kislyuk    (501) staff       (20)       91 2022-12-14 03:54:21.051077 pyotp-2.8.0/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1196 2022-12-14 03:53:16.000000 pyotp-2.8.0/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2022-12-14 03:54:21.044831 pyotp-2.8.0/src/
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2022-12-14 03:54:21.047445 pyotp-2.8.0/src/pyotp/
--rw-r--r--   0 kislyuk    (501) staff       (20)     3492 2022-12-14 03:51:41.000000 pyotp-2.8.0/src/pyotp/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      209 2022-09-11 18:31:53.000000 pyotp-2.8.0/src/pyotp/compat.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2022-12-14 03:54:21.049278 pyotp-2.8.0/src/pyotp/contrib/
--rw-r--r--   0 kislyuk    (501) staff       (20)       38 2022-09-11 18:53:29.000000 pyotp-2.8.0/src/pyotp/contrib/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     1339 2022-09-11 18:53:33.000000 pyotp-2.8.0/src/pyotp/contrib/steam.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2672 2022-12-14 03:34:30.000000 pyotp-2.8.0/src/pyotp/hotp.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2222 2022-12-14 03:51:41.000000 pyotp-2.8.0/src/pyotp/otp.py
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-09-11 18:31:53.000000 pyotp-2.8.0/src/pyotp/py.typed
--rw-r--r--   0 kislyuk    (501) staff       (20)     4096 2022-12-14 03:34:30.000000 pyotp-2.8.0/src/pyotp/totp.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     3120 2022-12-14 03:51:41.000000 pyotp-2.8.0/src/pyotp/utils.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2022-12-14 03:54:21.048404 pyotp-2.8.0/src/pyotp.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)     8758 2022-12-14 03:54:21.000000 pyotp-2.8.0/src/pyotp.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)      426 2022-12-14 03:54:21.000000 pyotp-2.8.0/src/pyotp.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2022-12-14 03:54:21.000000 pyotp-2.8.0/src/pyotp.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2016-06-14 14:22:47.000000 pyotp-2.8.0/src/pyotp.egg-info/not-zip-safe
--rw-r--r--   0 kislyuk    (501) staff       (20)        6 2022-12-14 03:54:21.000000 pyotp-2.8.0/src/pyotp.egg-info/top_level.txt
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    19287 2022-09-11 18:53:33.000000 pyotp-2.8.0/test.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-07-27 23:40:52.159931 pyotp-2.9.0/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1174 2021-12-09 09:28:01.000000 pyotp-2.9.0/LICENSE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       51 2021-12-09 09:29:43.000000 pyotp-2.9.0/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9684 2023-07-27 23:40:52.158836 pyotp-2.9.0/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8507 2023-06-16 00:22:25.000000 pyotp-2.9.0/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      112 2023-06-16 00:22:25.000000 pyotp-2.9.0/pyproject.toml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2023-07-27 23:40:52.160089 pyotp-2.9.0/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1571 2023-07-27 23:38:36.000000 pyotp-2.9.0/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-07-27 23:40:52.146624 pyotp-2.9.0/src/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-07-27 23:40:52.154266 pyotp-2.9.0/src/pyotp/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3792 2023-07-27 23:37:40.000000 pyotp-2.9.0/src/pyotp/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      209 2021-12-09 09:28:01.000000 pyotp-2.9.0/src/pyotp/compat.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-07-27 23:40:52.158217 pyotp-2.9.0/src/pyotp/contrib/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2022-09-12 14:53:34.000000 pyotp-2.9.0/src/pyotp/contrib/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1410 2023-07-27 23:37:40.000000 pyotp-2.9.0/src/pyotp/contrib/steam.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2672 2023-03-04 20:03:14.000000 pyotp-2.9.0/src/pyotp/hotp.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2222 2023-07-27 23:37:37.000000 pyotp-2.9.0/src/pyotp/otp.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2021-12-09 09:28:01.000000 pyotp-2.9.0/src/pyotp/py.typed
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4096 2023-03-04 20:03:14.000000 pyotp-2.9.0/src/pyotp/totp.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3120 2023-03-04 20:03:14.000000 pyotp-2.9.0/src/pyotp/utils.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-07-27 23:40:52.157473 pyotp-2.9.0/src/pyotp.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9684 2023-07-27 23:40:52.000000 pyotp-2.9.0/src/pyotp.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      448 2023-07-27 23:40:52.000000 pyotp-2.9.0/src/pyotp.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-07-27 23:40:52.000000 pyotp-2.9.0/src/pyotp.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2021-12-09 09:32:05.000000 pyotp-2.9.0/src/pyotp.egg-info/not-zip-safe
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       33 2023-07-27 23:40:52.000000 pyotp-2.9.0/src/pyotp.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        6 2023-07-27 23:40:52.000000 pyotp-2.9.0/src/pyotp.egg-info/top_level.txt
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    20368 2023-07-27 23:37:40.000000 pyotp-2.9.0/test.py
```

### Comparing `pyotp-2.8.0/LICENSE` & `pyotp-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyotp-2.8.0/PKG-INFO` & `pyotp-2.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: pyotp
-Version: 2.8.0
-Summary: Python One Time Password Library
-Home-page: https://github.com/pyotp/pyotp
-Author: PyOTP contributors
-Author-email: kislyuk@gmail.com
-License: MIT License
-Platform: MacOS X
-Platform: Posix
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
-License-File: LICENSE
-
 PyOTP - The Python One-Time Password Library
 ============================================
 
 PyOTP is a Python library for generating and verifying one-time passwords. It can be used to implement two-factor (2FA)
 or multi-factor (MFA) authentication methods in web applications and in other systems that require users to log in.
 
 Open MFA standards are defined in `RFC 4226 <https://tools.ietf.org/html/rfc4226>`_ (HOTP: An HMAC-Based One-Time
@@ -39,37 +14,41 @@
 
 Implementers should read and follow the `HOTP security requirements <https://tools.ietf.org/html/rfc4226#section-7>`_
 and `TOTP security considerations <https://tools.ietf.org/html/rfc6238#section-5>`_ sections of the relevant RFCs. At
 minimum, application implementers should follow this checklist:
 
 - Ensure transport confidentiality by using HTTPS
 - Ensure HOTP/TOTP secret confidentiality by storing secrets in a controlled access database
-- Deny replay attacks by rejecting one-time passwords that have been used by the client (this requires storing the most 
-  recently authenticated timestamp, OTP, or hash of the OTP in your database, and rejecting the OTP when a match is seen)
+- Deny replay attacks by rejecting one-time passwords that have been used by the client (this requires storing the most
+  recently authenticated timestamp, OTP, or hash of the OTP in your database, and rejecting the OTP when a match is
+  seen)
 - Throttle (rate limit) brute-force attacks against your application's login functionality (see RFC 4226, section 7.3)
 - When implementing a "greenfield" application, consider supporting
   `FIDO U2F <https://en.wikipedia.org/wiki/Universal_2nd_Factor>`_/`WebAuthn <https://www.w3.org/TR/webauthn/>`_ in
   addition to HOTP/TOTP. U2F uses asymmetric cryptography to avoid using a shared secret design, which strengthens your
   MFA solution against server-side attacks. Hardware U2F also sequesters the client secret in a dedicated single-purpose
   device, which strengthens your clients against client-side attacks. And by automating scoping of credentials to
-  relying party IDs (application origin/domain names), U2F adds protection against phishing attacks. One implementation of
-  FIDO U2F/WebAuthn is PyOTP's sister project, `PyWARP <https://github.com/pyauth/pywarp>`_.
+  relying party IDs (application origin/domain names), U2F adds protection against phishing attacks. One implementation
+  of FIDO U2F/WebAuthn is PyOTP's sister project, `PyWARP <https://github.com/pyauth/pywarp>`_.
 
 We also recommend that implementers read the
-`OWASP Authentication Cheat Sheet <https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Authentication_Cheat_Sheet.md>`_ and
+`OWASP Authentication Cheat Sheet
+<https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Authentication_Cheat_Sheet.md>`_ and
 `NIST SP 800-63-3: Digital Authentication Guideline <https://pages.nist.gov/800-63-3/>`_ for a high level overview of
 authentication best practices.
 
 Quick overview of using One Time Passwords on your phone
 --------------------------------------------------------
 
 * OTPs involve a shared secret, stored both on the phone and the server
 * OTPs can be generated on a phone without internet connectivity
-* OTPs should always be used as a second factor of authentication (if your phone is lost, you account is still secured with a password)
-* Google Authenticator and other OTP client apps allow you to store multiple OTP secrets and provision those using a QR Code
+* OTPs should always be used as a second factor of authentication (if your phone is lost, you account is still secured
+  with a password)
+* Google Authenticator and other OTP client apps allow you to store multiple OTP secrets and provision those using a QR
+  Code
 
 Installation
 ------------
 ::
 
     pip install pyotp
 
@@ -104,38 +83,39 @@
 
     # OTP verified with a counter
     hotp.verify('316439', 1401) # => True
     hotp.verify('316439', 1402) # => False
 
 Generating a Secret Key
 ~~~~~~~~~~~~~~~~~~~~~~~
-A helper function is provided to generate a 32-character base32 secret, compatible with Google Authenticator and other OTP apps::
+A helper function is provided to generate a 32-character base32 secret, compatible with Google Authenticator and other
+OTP apps::
 
     pyotp.random_base32()
 
 Some applications want the secret key to be formatted as a hex-encoded string::
 
     pyotp.random_hex()  # returns a 40-character hex-encoded secret
 
 Google Authenticator Compatible
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-PyOTP works with the Google Authenticator iPhone and Android app, as well as other OTP apps like Authy. PyOTP includes the
-ability to generate provisioning URIs for use with the QR Code scanner built into these MFA client apps::
+PyOTP works with the Google Authenticator iPhone and Android app, as well as other OTP apps like Authy. PyOTP includes
+the ability to generate provisioning URIs for use with the QR Code scanner built into these MFA client apps::
 
     pyotp.totp.TOTP('JBSWY3DPEHPK3PXP').provisioning_uri(name='alice@google.com', issuer_name='Secure App')
 
     >>> 'otpauth://totp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App'
 
     pyotp.hotp.HOTP('JBSWY3DPEHPK3PXP').provisioning_uri(name="alice@google.com", issuer_name="Secure App", initial_count=0)
 
     >>> 'otpauth://hotp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App&counter=0'
 
-This URL can then be rendered as a QR Code (for example, using https://github.com/soldair/node-qrcode) which can then be scanned
-and added to the users list of OTP credentials.
+This URL can then be rendered as a QR Code (for example, using https://github.com/soldair/node-qrcode) which can then be
+scanned and added to the users list of OTP credentials.
 
 Parsing these URLs is also supported::
 
     pyotp.parse_uri('otpauth://totp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App')
 
     >>> <pyotp.totp.TOTP object at 0xFFFFFFFF>
 
@@ -152,14 +132,21 @@
 
 Now run the following and compare the output::
 
     import pyotp
     totp = pyotp.TOTP("JBSWY3DPEHPK3PXP")
     print("Current OTP:", totp.now())
 
+Third-party contributions
+~~~~~~~~~~~~~~~~~~~~~~~~~
+The following third-party contributions are not described by a standard, not officially supported, and provided for
+reference only:
+
+* ``pyotp.contrib.Steam()``: An implementation of Steam TOTP. Uses the same API as `pyotp.TOTP()`.
+
 Links
 ~~~~~
 
 * `Project home page (GitHub) <https://github.com/pyauth/pyotp>`_
 * `Documentation <https://pyauth.github.io/pyotp/>`_
 * `Package distribution (PyPI) <https://pypi.python.org/pypi/pyotp>`_
 * `Change log <https://github.com/pyauth/pyotp/blob/master/Changes.rst>`_
@@ -171,14 +158,21 @@
 * `NIST SP 800-63-3: Digital Authentication Guideline <https://pages.nist.gov/800-63-3/>`_
 
 For new applications:
 
 * `WebAuthn <https://www.w3.org/TR/webauthn/>`_
 * `PyWARP <https://github.com/pyauth/pywarp>`_
 
+Versioning
+~~~~~~~~~~
+This package follows the `Semantic Versioning 2.0.0 <http://semver.org/>`_ standard. To control changes, it is
+recommended that application developers pin the package version and manage it using `pip-tools
+<https://github.com/jazzband/pip-tools>`_ or similar. For library developers, pinning the major version is
+recommended.
+
 .. image:: https://github.com/pyauth/pyotp/workflows/Python%20package/badge.svg
         :target: https://github.com/pyauth/pyotp/actions
 .. image:: https://img.shields.io/codecov/c/github/pyauth/pyotp/master.svg
         :target: https://codecov.io/github/pyauth/pyotp?branch=master
 .. image:: https://img.shields.io/pypi/v/pyotp.svg
         :target: https://pypi.python.org/pypi/pyotp
 .. image:: https://img.shields.io/pypi/l/pyotp.svg
```

### Comparing `pyotp-2.8.0/README.rst` & `pyotp-2.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: pyotp
+Version: 2.9.0
+Summary: Python One Time Password Library
+Home-page: https://github.com/pyotp/pyotp
+Author: PyOTP contributors
+Author-email: kislyuk@gmail.com
+License: MIT License
+Project-URL: Documentation, https://pyauth.github.io/pyotp
+Project-URL: Source Code, https://github.com/pyauth/pyotp
+Project-URL: Issue Tracker, https://github.com/pyauth/pyotp/issues
+Project-URL: Change Log, https://github.com/pyauth/pyotp/blob/master/Changes.rst
+Platform: MacOS X
+Platform: Posix
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
+Provides-Extra: test
+License-File: LICENSE
+
 PyOTP - The Python One-Time Password Library
 ============================================
 
 PyOTP is a Python library for generating and verifying one-time passwords. It can be used to implement two-factor (2FA)
 or multi-factor (MFA) authentication methods in web applications and in other systems that require users to log in.
 
 Open MFA standards are defined in `RFC 4226 <https://tools.ietf.org/html/rfc4226>`_ (HOTP: An HMAC-Based One-Time
@@ -14,37 +44,41 @@
 
 Implementers should read and follow the `HOTP security requirements <https://tools.ietf.org/html/rfc4226#section-7>`_
 and `TOTP security considerations <https://tools.ietf.org/html/rfc6238#section-5>`_ sections of the relevant RFCs. At
 minimum, application implementers should follow this checklist:
 
 - Ensure transport confidentiality by using HTTPS
 - Ensure HOTP/TOTP secret confidentiality by storing secrets in a controlled access database
-- Deny replay attacks by rejecting one-time passwords that have been used by the client (this requires storing the most 
-  recently authenticated timestamp, OTP, or hash of the OTP in your database, and rejecting the OTP when a match is seen)
+- Deny replay attacks by rejecting one-time passwords that have been used by the client (this requires storing the most
+  recently authenticated timestamp, OTP, or hash of the OTP in your database, and rejecting the OTP when a match is
+  seen)
 - Throttle (rate limit) brute-force attacks against your application's login functionality (see RFC 4226, section 7.3)
 - When implementing a "greenfield" application, consider supporting
   `FIDO U2F <https://en.wikipedia.org/wiki/Universal_2nd_Factor>`_/`WebAuthn <https://www.w3.org/TR/webauthn/>`_ in
   addition to HOTP/TOTP. U2F uses asymmetric cryptography to avoid using a shared secret design, which strengthens your
   MFA solution against server-side attacks. Hardware U2F also sequesters the client secret in a dedicated single-purpose
   device, which strengthens your clients against client-side attacks. And by automating scoping of credentials to
-  relying party IDs (application origin/domain names), U2F adds protection against phishing attacks. One implementation of
-  FIDO U2F/WebAuthn is PyOTP's sister project, `PyWARP <https://github.com/pyauth/pywarp>`_.
+  relying party IDs (application origin/domain names), U2F adds protection against phishing attacks. One implementation
+  of FIDO U2F/WebAuthn is PyOTP's sister project, `PyWARP <https://github.com/pyauth/pywarp>`_.
 
 We also recommend that implementers read the
-`OWASP Authentication Cheat Sheet <https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Authentication_Cheat_Sheet.md>`_ and
+`OWASP Authentication Cheat Sheet
+<https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Authentication_Cheat_Sheet.md>`_ and
 `NIST SP 800-63-3: Digital Authentication Guideline <https://pages.nist.gov/800-63-3/>`_ for a high level overview of
 authentication best practices.
 
 Quick overview of using One Time Passwords on your phone
 --------------------------------------------------------
 
 * OTPs involve a shared secret, stored both on the phone and the server
 * OTPs can be generated on a phone without internet connectivity
-* OTPs should always be used as a second factor of authentication (if your phone is lost, you account is still secured with a password)
-* Google Authenticator and other OTP client apps allow you to store multiple OTP secrets and provision those using a QR Code
+* OTPs should always be used as a second factor of authentication (if your phone is lost, you account is still secured
+  with a password)
+* Google Authenticator and other OTP client apps allow you to store multiple OTP secrets and provision those using a QR
+  Code
 
 Installation
 ------------
 ::
 
     pip install pyotp
 
@@ -79,38 +113,39 @@
 
     # OTP verified with a counter
     hotp.verify('316439', 1401) # => True
     hotp.verify('316439', 1402) # => False
 
 Generating a Secret Key
 ~~~~~~~~~~~~~~~~~~~~~~~
-A helper function is provided to generate a 32-character base32 secret, compatible with Google Authenticator and other OTP apps::
+A helper function is provided to generate a 32-character base32 secret, compatible with Google Authenticator and other
+OTP apps::
 
     pyotp.random_base32()
 
 Some applications want the secret key to be formatted as a hex-encoded string::
 
     pyotp.random_hex()  # returns a 40-character hex-encoded secret
 
 Google Authenticator Compatible
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-PyOTP works with the Google Authenticator iPhone and Android app, as well as other OTP apps like Authy. PyOTP includes the
-ability to generate provisioning URIs for use with the QR Code scanner built into these MFA client apps::
+PyOTP works with the Google Authenticator iPhone and Android app, as well as other OTP apps like Authy. PyOTP includes
+the ability to generate provisioning URIs for use with the QR Code scanner built into these MFA client apps::
 
     pyotp.totp.TOTP('JBSWY3DPEHPK3PXP').provisioning_uri(name='alice@google.com', issuer_name='Secure App')
 
     >>> 'otpauth://totp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App'
 
     pyotp.hotp.HOTP('JBSWY3DPEHPK3PXP').provisioning_uri(name="alice@google.com", issuer_name="Secure App", initial_count=0)
 
     >>> 'otpauth://hotp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App&counter=0'
 
-This URL can then be rendered as a QR Code (for example, using https://github.com/soldair/node-qrcode) which can then be scanned
-and added to the users list of OTP credentials.
+This URL can then be rendered as a QR Code (for example, using https://github.com/soldair/node-qrcode) which can then be
+scanned and added to the users list of OTP credentials.
 
 Parsing these URLs is also supported::
 
     pyotp.parse_uri('otpauth://totp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App')
 
     >>> <pyotp.totp.TOTP object at 0xFFFFFFFF>
 
@@ -127,14 +162,21 @@
 
 Now run the following and compare the output::
 
     import pyotp
     totp = pyotp.TOTP("JBSWY3DPEHPK3PXP")
     print("Current OTP:", totp.now())
 
+Third-party contributions
+~~~~~~~~~~~~~~~~~~~~~~~~~
+The following third-party contributions are not described by a standard, not officially supported, and provided for
+reference only:
+
+* ``pyotp.contrib.Steam()``: An implementation of Steam TOTP. Uses the same API as `pyotp.TOTP()`.
+
 Links
 ~~~~~
 
 * `Project home page (GitHub) <https://github.com/pyauth/pyotp>`_
 * `Documentation <https://pyauth.github.io/pyotp/>`_
 * `Package distribution (PyPI) <https://pypi.python.org/pypi/pyotp>`_
 * `Change log <https://github.com/pyauth/pyotp/blob/master/Changes.rst>`_
@@ -146,14 +188,21 @@
 * `NIST SP 800-63-3: Digital Authentication Guideline <https://pages.nist.gov/800-63-3/>`_
 
 For new applications:
 
 * `WebAuthn <https://www.w3.org/TR/webauthn/>`_
 * `PyWARP <https://github.com/pyauth/pywarp>`_
 
+Versioning
+~~~~~~~~~~
+This package follows the `Semantic Versioning 2.0.0 <http://semver.org/>`_ standard. To control changes, it is
+recommended that application developers pin the package version and manage it using `pip-tools
+<https://github.com/jazzband/pip-tools>`_ or similar. For library developers, pinning the major version is
+recommended.
+
 .. image:: https://github.com/pyauth/pyotp/workflows/Python%20package/badge.svg
         :target: https://github.com/pyauth/pyotp/actions
 .. image:: https://img.shields.io/codecov/c/github/pyauth/pyotp/master.svg
         :target: https://codecov.io/github/pyauth/pyotp?branch=master
 .. image:: https://img.shields.io/pypi/v/pyotp.svg
         :target: https://pypi.python.org/pypi/pyotp
 .. image:: https://img.shields.io/pypi/l/pyotp.svg
```

### Comparing `pyotp-2.8.0/src/pyotp/__init__.py` & `pyotp-2.9.0/src/pyotp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,20 @@
     :param uri: the hotp/totp URI to parse
     :returns: OTP object
     """
 
     # Secret (to be filled in later)
     secret = None
 
+    # Encoder (to be filled in later)
+    encoder = None
+
+    # Digits (to be filled in later)
+    digits = None
+
     # Data we'll parse to the correct constructor
     otp_data: Dict[str, Any] = {}
 
     # Parse with URLlib
     parsed_uri = urlparse(unquote(uri))
 
     if parsed_uri.scheme != "otpauth":
@@ -70,29 +76,35 @@
                 otp_data["digest"] = hashlib.sha1
             elif value == "SHA256":
                 otp_data["digest"] = hashlib.sha256
             elif value == "SHA512":
                 otp_data["digest"] = hashlib.sha512
             else:
                 raise ValueError("Invalid value for algorithm, must be SHA1, SHA256 or SHA512")
+        elif key == "encoder":
+            encoder = value
         elif key == "digits":
             digits = int(value)
-            if digits not in [6, 7, 8]:
-                raise ValueError("Digits may only be 6, 7, or 8")
             otp_data["digits"] = digits
         elif key == "period":
             otp_data["interval"] = int(value)
         elif key == "counter":
             otp_data["initial_count"] = int(value)
         elif key != "image":
             raise ValueError("{} is not a valid parameter".format(key))
-
+    
+    if encoder != "steam":
+        if digits is not None and digits not in [6, 7, 8]:
+            raise ValueError("Digits may only be 6, 7, or 8")
+    
     if not secret:
         raise ValueError("No secret found in URI")
 
     # Create objects
+    if encoder == "steam":
+        return contrib.Steam(secret, **otp_data)
     if parsed_uri.netloc == "totp":
         return TOTP(secret, **otp_data)
     elif parsed_uri.netloc == "hotp":
         return HOTP(secret, **otp_data)
 
     raise ValueError("Not a supported OTP type")
```

### Comparing `pyotp-2.8.0/src/pyotp/contrib/steam.py` & `pyotp-2.9.0/src/pyotp/contrib/steam.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 
 
 class Steam(TOTP):
     """
     Steam's custom TOTP. Subclass of `pyotp.totp.TOTP`.
     """
 
-    def __init__(self, s: str, name: Optional[str] = None, issuer: Optional[str] = None, interval: int = 30) -> None:
+    def __init__(
+        self,
+        s: str,
+        name: Optional[str] = None,
+        issuer: Optional[str] = None,
+        interval: int = 30,
+        digits: int = 5
+    ) -> None:
         """
         :param s: secret in base32 format
         :param interval: the time interval in seconds for OTP. This defaults to 30.
         :param name: account name
         :param issuer: issuer
         """
         self.interval = interval
```

### Comparing `pyotp-2.8.0/src/pyotp/hotp.py` & `pyotp-2.9.0/src/pyotp/hotp.py`

 * *Files identical despite different names*

### Comparing `pyotp-2.8.0/src/pyotp/otp.py` & `pyotp-2.9.0/src/pyotp/otp.py`

 * *Files identical despite different names*

### Comparing `pyotp-2.8.0/src/pyotp/totp.py` & `pyotp-2.9.0/src/pyotp/totp.py`

 * *Files identical despite different names*

### Comparing `pyotp-2.8.0/src/pyotp/utils.py` & `pyotp-2.9.0/src/pyotp/utils.py`

 * *Files identical despite different names*

### Comparing `pyotp-2.8.0/src/pyotp.egg-info/PKG-INFO` & `pyotp-2.9.0/src/pyotp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: pyotp
-Version: 2.8.0
+Version: 2.9.0
 Summary: Python One Time Password Library
 Home-page: https://github.com/pyotp/pyotp
 Author: PyOTP contributors
 Author-email: kislyuk@gmail.com
 License: MIT License
+Project-URL: Documentation, https://pyauth.github.io/pyotp
+Project-URL: Source Code, https://github.com/pyauth/pyotp
+Project-URL: Issue Tracker, https://github.com/pyauth/pyotp/issues
+Project-URL: Change Log, https://github.com/pyauth/pyotp/blob/master/Changes.rst
 Platform: MacOS X
 Platform: Posix
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+Provides-Extra: test
 License-File: LICENSE
 
 PyOTP - The Python One-Time Password Library
 ============================================
 
 PyOTP is a Python library for generating and verifying one-time passwords. It can be used to implement two-factor (2FA)
 or multi-factor (MFA) authentication methods in web applications and in other systems that require users to log in.
@@ -39,37 +44,41 @@
 
 Implementers should read and follow the `HOTP security requirements <https://tools.ietf.org/html/rfc4226#section-7>`_
 and `TOTP security considerations <https://tools.ietf.org/html/rfc6238#section-5>`_ sections of the relevant RFCs. At
 minimum, application implementers should follow this checklist:
 
 - Ensure transport confidentiality by using HTTPS
 - Ensure HOTP/TOTP secret confidentiality by storing secrets in a controlled access database
-- Deny replay attacks by rejecting one-time passwords that have been used by the client (this requires storing the most 
-  recently authenticated timestamp, OTP, or hash of the OTP in your database, and rejecting the OTP when a match is seen)
+- Deny replay attacks by rejecting one-time passwords that have been used by the client (this requires storing the most
+  recently authenticated timestamp, OTP, or hash of the OTP in your database, and rejecting the OTP when a match is
+  seen)
 - Throttle (rate limit) brute-force attacks against your application's login functionality (see RFC 4226, section 7.3)
 - When implementing a "greenfield" application, consider supporting
   `FIDO U2F <https://en.wikipedia.org/wiki/Universal_2nd_Factor>`_/`WebAuthn <https://www.w3.org/TR/webauthn/>`_ in
   addition to HOTP/TOTP. U2F uses asymmetric cryptography to avoid using a shared secret design, which strengthens your
   MFA solution against server-side attacks. Hardware U2F also sequesters the client secret in a dedicated single-purpose
   device, which strengthens your clients against client-side attacks. And by automating scoping of credentials to
-  relying party IDs (application origin/domain names), U2F adds protection against phishing attacks. One implementation of
-  FIDO U2F/WebAuthn is PyOTP's sister project, `PyWARP <https://github.com/pyauth/pywarp>`_.
+  relying party IDs (application origin/domain names), U2F adds protection against phishing attacks. One implementation
+  of FIDO U2F/WebAuthn is PyOTP's sister project, `PyWARP <https://github.com/pyauth/pywarp>`_.
 
 We also recommend that implementers read the
-`OWASP Authentication Cheat Sheet <https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Authentication_Cheat_Sheet.md>`_ and
+`OWASP Authentication Cheat Sheet
+<https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Authentication_Cheat_Sheet.md>`_ and
 `NIST SP 800-63-3: Digital Authentication Guideline <https://pages.nist.gov/800-63-3/>`_ for a high level overview of
 authentication best practices.
 
 Quick overview of using One Time Passwords on your phone
 --------------------------------------------------------
 
 * OTPs involve a shared secret, stored both on the phone and the server
 * OTPs can be generated on a phone without internet connectivity
-* OTPs should always be used as a second factor of authentication (if your phone is lost, you account is still secured with a password)
-* Google Authenticator and other OTP client apps allow you to store multiple OTP secrets and provision those using a QR Code
+* OTPs should always be used as a second factor of authentication (if your phone is lost, you account is still secured
+  with a password)
+* Google Authenticator and other OTP client apps allow you to store multiple OTP secrets and provision those using a QR
+  Code
 
 Installation
 ------------
 ::
 
     pip install pyotp
 
@@ -104,38 +113,39 @@
 
     # OTP verified with a counter
     hotp.verify('316439', 1401) # => True
     hotp.verify('316439', 1402) # => False
 
 Generating a Secret Key
 ~~~~~~~~~~~~~~~~~~~~~~~
-A helper function is provided to generate a 32-character base32 secret, compatible with Google Authenticator and other OTP apps::
+A helper function is provided to generate a 32-character base32 secret, compatible with Google Authenticator and other
+OTP apps::
 
     pyotp.random_base32()
 
 Some applications want the secret key to be formatted as a hex-encoded string::
 
     pyotp.random_hex()  # returns a 40-character hex-encoded secret
 
 Google Authenticator Compatible
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-PyOTP works with the Google Authenticator iPhone and Android app, as well as other OTP apps like Authy. PyOTP includes the
-ability to generate provisioning URIs for use with the QR Code scanner built into these MFA client apps::
+PyOTP works with the Google Authenticator iPhone and Android app, as well as other OTP apps like Authy. PyOTP includes
+the ability to generate provisioning URIs for use with the QR Code scanner built into these MFA client apps::
 
     pyotp.totp.TOTP('JBSWY3DPEHPK3PXP').provisioning_uri(name='alice@google.com', issuer_name='Secure App')
 
     >>> 'otpauth://totp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App'
 
     pyotp.hotp.HOTP('JBSWY3DPEHPK3PXP').provisioning_uri(name="alice@google.com", issuer_name="Secure App", initial_count=0)
 
     >>> 'otpauth://hotp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App&counter=0'
 
-This URL can then be rendered as a QR Code (for example, using https://github.com/soldair/node-qrcode) which can then be scanned
-and added to the users list of OTP credentials.
+This URL can then be rendered as a QR Code (for example, using https://github.com/soldair/node-qrcode) which can then be
+scanned and added to the users list of OTP credentials.
 
 Parsing these URLs is also supported::
 
     pyotp.parse_uri('otpauth://totp/Secure%20App:alice%40google.com?secret=JBSWY3DPEHPK3PXP&issuer=Secure%20App')
 
     >>> <pyotp.totp.TOTP object at 0xFFFFFFFF>
 
@@ -152,14 +162,21 @@
 
 Now run the following and compare the output::
 
     import pyotp
     totp = pyotp.TOTP("JBSWY3DPEHPK3PXP")
     print("Current OTP:", totp.now())
 
+Third-party contributions
+~~~~~~~~~~~~~~~~~~~~~~~~~
+The following third-party contributions are not described by a standard, not officially supported, and provided for
+reference only:
+
+* ``pyotp.contrib.Steam()``: An implementation of Steam TOTP. Uses the same API as `pyotp.TOTP()`.
+
 Links
 ~~~~~
 
 * `Project home page (GitHub) <https://github.com/pyauth/pyotp>`_
 * `Documentation <https://pyauth.github.io/pyotp/>`_
 * `Package distribution (PyPI) <https://pypi.python.org/pypi/pyotp>`_
 * `Change log <https://github.com/pyauth/pyotp/blob/master/Changes.rst>`_
@@ -171,14 +188,21 @@
 * `NIST SP 800-63-3: Digital Authentication Guideline <https://pages.nist.gov/800-63-3/>`_
 
 For new applications:
 
 * `WebAuthn <https://www.w3.org/TR/webauthn/>`_
 * `PyWARP <https://github.com/pyauth/pywarp>`_
 
+Versioning
+~~~~~~~~~~
+This package follows the `Semantic Versioning 2.0.0 <http://semver.org/>`_ standard. To control changes, it is
+recommended that application developers pin the package version and manage it using `pip-tools
+<https://github.com/jazzband/pip-tools>`_ or similar. For library developers, pinning the major version is
+recommended.
+
 .. image:: https://github.com/pyauth/pyotp/workflows/Python%20package/badge.svg
         :target: https://github.com/pyauth/pyotp/actions
 .. image:: https://img.shields.io/codecov/c/github/pyauth/pyotp/master.svg
         :target: https://codecov.io/github/pyauth/pyotp?branch=master
 .. image:: https://img.shields.io/pypi/v/pyotp.svg
         :target: https://pypi.python.org/pypi/pyotp
 .. image:: https://img.shields.io/pypi/l/pyotp.svg
```

### Comparing `pyotp-2.8.0/test.py` & `pyotp-2.9.0/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,21 @@
         with self.assertRaises(ValueError) as cm:
             pyotp.parse_uri("otpauth://totp/SomeIssuer:?issuer=AnotherIssuer")
         self.assertEqual("If issuer is specified in both label and parameters, it should be equal.", str(cm.exception))
 
         with self.assertRaises(ValueError) as cm:
             pyotp.parse_uri("otpauth://totp?algorithm=aes")
         self.assertEqual("Invalid value for algorithm, must be SHA1, SHA256 or SHA512", str(cm.exception))
+    
+    def test_parse_steam(self):
+        otp = pyotp.parse_uri("otpauth://totp/Steam:?secret=SOME_SECRET&encoder=steam")
+        self.assertEqual(type(otp), pyotp.contrib.Steam)
+
+        otp = pyotp.parse_uri("otpauth://totp/Steam:?secret=SOME_SECRET")
+        self.assertNotEqual(type(otp), pyotp.contrib.Steam)
 
     @unittest.skipIf(sys.version_info < (3, 6), "Skipping test that requires deterministic dict key enumeration")
     def test_algorithms(self):
         otp = pyotp.parse_uri("otpauth://totp?algorithm=SHA1&secret=GEZDGNBV&algorithm=SHA1")
         self.assertEqual(hashlib.sha1, otp.digest)
         self.assertEqual(otp.at(0), "734055")
         self.assertEqual(otp.at(30), "662488")
@@ -416,14 +423,28 @@
         )
         with self.assertRaises(ValueError):
             otp.provisioning_uri(name="n", issuer_name="i", image="nourl")
 
         otp = pyotp.parse_uri(otp.provisioning_uri(name="n", issuer_name="i", image="https://test.net/test.png"))
         self.assertEqual(hashlib.sha512, otp.digest)
 
+        otp = pyotp.parse_uri("otpauth://totp/Steam:?secret=FMXNK4QEGKVPULRTADY6JIDK5VHUBGZW&encoder=steam")
+        self.assertEqual(type(otp), pyotp.contrib.Steam)
+        self.assertEqual(otp.at(0), "C5V56")
+        self.assertEqual(otp.at(30), "QJY8Y")
+        self.assertEqual(otp.at(60), "R3WQY")
+        self.assertEqual(otp.at(90), "JG3T3")
+
+        # period and digits should be ignored
+        otp = pyotp.parse_uri("otpauth://totp/Steam:?secret=FMXNK4QEGKVPULRTADY6JIDK5VHUBGZW&period=15&digits=7&encoder=steam")
+        self.assertEqual(type(otp), pyotp.contrib.Steam)
+        self.assertEqual(otp.at(0), "C5V56")
+        self.assertEqual(otp.at(30), "QJY8Y")
+        self.assertEqual(otp.at(60), "R3WQY")
+        self.assertEqual(otp.at(90), "JG3T3")
 
 class Timecop(object):
     """
     Half-assed clone of timecop.rb, just enough to pass our tests.
     """
 
     def __init__(self, freeze_timestamp):
```

