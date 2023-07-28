# Comparing `tmp/mend_import_sbom-23.3.1-py3-none-any.whl.zip` & `tmp/mend_import_sbom-23.7.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 17344 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-02 14:50 mend_import_sbom/__init__.py
--rw-r--r--  2.0 unx      107 b- defN 23-Mar-02 14:50 mend_import_sbom/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-02 14:50 mend_import_sbom/conftest.py
--rw-r--r--  2.0 unx     3111 b- defN 23-Mar-02 14:50 mend_import_sbom/import_const.py
--rw-r--r--  2.0 unx    23640 b- defN 23-Mar-02 14:50 mend_import_sbom/import_sbom.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-02 14:50 mend_import_sbom-23.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    14205 b- defN 23-Mar-02 14:50 mend_import_sbom-23.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-02 14:50 mend_import_sbom-23.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Mar-02 14:50 mend_import_sbom-23.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-02 14:50 mend_import_sbom-23.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      969 b- defN 23-Mar-02 14:50 mend_import_sbom-23.3.1.dist-info/RECORD
-11 files, 53565 bytes uncompressed, 15674 bytes compressed:  70.7%
+Zip file size: 19621 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 21:30 mend_import_sbom/__init__.py
+-rw-r--r--  2.0 unx      109 b- defN 23-Jul-28 21:30 mend_import_sbom/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-28 21:30 mend_import_sbom/conftest.py
+-rw-r--r--  2.0 unx     3447 b- defN 23-Jul-28 21:30 mend_import_sbom/import_const.py
+-rw-r--r--  2.0 unx    31219 b- defN 23-Jul-28 21:30 mend_import_sbom/import_sbom.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-28 21:30 mend_import_sbom-23.7.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17460 b- defN 23-Jul-28 21:30 mend_import_sbom-23.7.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 21:30 mend_import_sbom-23.7.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-28 21:30 mend_import_sbom-23.7.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-28 21:30 mend_import_sbom-23.7.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      981 b- defN 23-Jul-28 21:30 mend_import_sbom-23.7.2.1.dist-info/RECORD
+11 files, 64748 bytes uncompressed, 17927 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_import_sbom/import_const.py
 Comment: 
 
 Filename: mend_import_sbom/import_sbom.py
 Comment: 
 
-Filename: mend_import_sbom-23.3.1.dist-info/LICENSE
+Filename: mend_import_sbom-23.7.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: mend_import_sbom-23.3.1.dist-info/METADATA
+Filename: mend_import_sbom-23.7.2.1.dist-info/METADATA
 Comment: 
 
-Filename: mend_import_sbom-23.3.1.dist-info/WHEEL
+Filename: mend_import_sbom-23.7.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: mend_import_sbom-23.3.1.dist-info/entry_points.txt
+Filename: mend_import_sbom-23.7.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_import_sbom-23.3.1.dist-info/top_level.txt
+Filename: mend_import_sbom-23.7.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_import_sbom-23.3.1.dist-info/RECORD
+Filename: mend_import_sbom-23.7.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_import_sbom/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.3.1"
+__version__ = "23.7.2.1"
 __tool_name__ = "import_sbom"
 __description__ = "Import SPDX or CSV SBOM into Mend"
```

## mend_import_sbom/import_const.py

```diff
@@ -1,30 +1,32 @@
 from enum import Enum
 import os
 
-class aliases(Enum): # List of aliases for params
+
+class aliases(Enum):  # List of aliases for params
     apikey = ("--apiKey","--api-key","--orgToken")
     userkey = ("--user-key","--userKey")
     projectkey = ("--scope","--projectToken")
     productkey = ("--productToken","--product")
     url = ("--url","--mendUrl")
     output = ("--out","--dir")
     sbom = ("--sbom","--input")
+    version = ("--version","-v")
 
     @classmethod
     def get_aliases_str(cls, key):
         res = list()
         for elem_ in cls.__dict__[key].value:
             res.append(elem_)
             if elem_ != elem_.lower():
                 res.append(elem_.lower())
         return res
 
 
-class varenvs(Enum): # Lit of Env.variables
+class varenvs(Enum):  # Lit of Env.variables
     wsuserkey = ("WS_USERKEY", "MEND_USERKEY")
     wsapikey = ("MEND_APIKEY","WS_APIKEY","WS_TOKEN")
     wsurl = ("WS_WSS_URL","MEND_WSS_URL","WS_URL","MEND_URL")
     wsscope = ("WS_SCOPE","MEND_SCOPE")
     wsproduct = ("WS_PRODUCTTOKEN", "MEND_PRODUCTTOKEN")
 
     @classmethod
@@ -33,39 +35,39 @@
         for el_ in cls.__dict__[key].value:
             res = os.environ.get(el_)
             if res:
                 break
         return res
 
 
+class Templates(Enum):  # Specific patterns of lib name and version
+    # First element is pattern of delimiter in library name.
+    # Second item contains possible specific symbols in version info that should be removed
+    github = (":", "^")
+
+
 class SHA1CalcType(Enum):  # list with supported packages
-    # hackage = ("y","Cabal","cabal") #cabal
-    # gradle = ("y","JAVA","jar") #jar
-    # maven_1 = ("y","JAVA","war") #war
-    # gradle_1 = ("y","JAVA","war") #war
-    # cargo = ("n","Crate","crate") #crate
-    # opam = ("n","Opam","opam") #opam
-    maven = ("y", "JAVA", "jar", "maven")  # jar
-    pypi = ("n", "PYTHON", "whl", "pypi")  # whl
-    npm = ("y", "NPM", "js", "npm", "npm")  # js
-    cdnjs = ("y", "CDNJS", "js", "cdnjs")  # js
-    dotnet = ("y", "NUGET", "exe", ".net")  # exe
-    bower = ("y", "BOWER", "jar", "bower")  # jar
-    ocaml = ("n", "Opam", "ml", "ocaml")  # ml
-    go = ("n", "GO", "go", "go")  # go
-    nuget = ("y", "NUGET", "ng", "nuget")  # ng
-    rpm = ("n", "RPM", "rpm", "rpm")  # rpm
-    composer = ("n", "PHP", "php", "php")  # php
-    cocoapods = ("n", "CocoaPods", "pod", "cocoapods")
-    cran = ("n", "R", "r", "r")  # r
-    gem = ("y", "RUBY", "gem", "ruby")  # gem
-    rust = ("y", "RUST", "rs", "rust")  # rs
-    rlib = ("y", "RUST", "rlib", "rust")  # rlib
-    hex = ("y", "HEX", "hex", "hex", "hex")  # hex, h86
-    alpine = ("n", "Alpine", "apk", "alpine")
+    maven = ("y", "JAVA", "jar", "maven",1)  # jar
+    pypi = ("n", "PYTHON", "whl", "pypi",2)  # whl
+    npm = ("y", "NPM", "js", "npm",3)  # js
+    cdnjs = ("y", "CDNJS", "js", "cdnjs",4)  # js
+    dotnet = ("y", "NUGET", "exe", ".net",5)  # exe
+    bower = ("y", "BOWER", "jar", "bower",6)  # jar
+    ocaml = ("n", "Opam", "ml", "ocaml",7)  # ml
+    go = ("n", "GO", "go", "go",8)  # go
+    nuget = ("y", "NUGET", "ng", "nuget",9)  # ng
+    rpm = ("n", "RPM", "rpm", "rpm",10)  # rpm
+    composer = ("n", "PHP", "php", "php",11)  # php
+    cocoapods = ("n", "CocoaPods", "pod", "cocoapods",12)
+    cran = ("n", "R", "r", "cran",13)  # r
+    gem = ("y", "RUBY", "gem", "ruby",14)  # gem
+    rust = ("y", "RUST", "rs", "rust",15)  # rs
+    rlib = ("y", "RUST", "rlib", "rust",16)  # rlib
+    hex = ("y", "HEX", "hex", "hex",17)  # hex, h86
+    alpine = ("n", "Alpine", "apk", "alpine",18)
 
     @property
     def lower_case(self):
         return self.value[0]
 
     @property
     def language(self):
@@ -75,14 +77,27 @@
     def ext(self):
         return self.value[2]
 
     @property
     def libtype(self):
         return self.value[3]
 
+    @property
+    def order(self):
+        return self.value[4]
+
+    @classmethod
+    def get_el_by_name(cls, name: str):
+        res = None
+        for el_ in cls:
+            if el_.name == name:
+                res = el_
+                break
+        return res
+
     @classmethod
     def get_package_data(cls, lng: str):
         res = ""
         for el_ in cls:
             if el_.language == lng:
                 res = el_.lower_case
                 break
```

## mend_import_sbom/import_sbom.py

```diff
@@ -2,37 +2,40 @@
 import csv
 import datetime
 import inspect
 import json
 import logging
 import os
 import sys
-import http.client
 import re
 import hashlib
-from ws_sdk import web, WS
+import requests
 
 from mend_import_sbom._version import __version__, __tool_name__, __description__
-from mend_import_sbom.import_const import SHA1CalcType, aliases, varenvs
+from mend_import_sbom.import_const import SHA1CalcType, aliases, varenvs, Templates
+from importlib import metadata
 
 logger = logging.getLogger(__tool_name__)
 logger.setLevel(logging.DEBUG)
-is_debug = logging.DEBUG if os.environ.get("DEBUG") in ['True', 'true', "1"] else logging.INFO
+is_debug = logging.DEBUG if os.environ.get("DEBUG") in ['True', 'true', 'TRUE', "1"] else logging.INFO
 
 formatter = logging.Formatter('[%(asctime)s] %(levelname)5s %(message)s', "%Y-%m-%d %H:%M:%S")
 s_handler = logging.StreamHandler()
 s_handler.setFormatter(formatter)
 s_handler.setLevel(is_debug)
 logger.addHandler(s_handler)
 logger.propagate = False
 
 APP_TITLE = "Mend SBOM Importer"
+APP_VERSION = metadata.version(f'mend_{__tool_name__}') if metadata.version(f'mend_{__tool_name__}') else __version__
+API_VERSION = "1.4"
 DFLT_PRD_NAME = "Mend-Imports"
 UPDATE_REQUEST_FILE = "update-request.txt"
 PROJ_URL = '/Wss/WSS.html#!project;id='  # f'{WS_WSS_URL}/Wss/WSS.html#!project;id={PROJECT_ID}'
+AGENT_INFO = {"agent": f"{__tool_name__.replace('_', '-')}", "agentVersion": APP_VERSION}
 
 
 def try_or_error(supplier, msg):
     try:
         return supplier()
     except:
         return msg
@@ -44,48 +47,66 @@
 
 
 def pn():
     pn_stack = inspect.stack()[2]
     return f'{pn_stack.function}:{pn_stack.lineno}'
 
 
+def ex():
+    e_type, e_msg, tb = sys.exc_info()
+    return f'{tb.tb_frame.f_code.co_name}:{tb.tb_lineno}'
+
+
 def log_obj_props(obj, obj_title=""):
     masked_props = ["ws_user_key", "user_key"]
     prop_list = [obj_title] if obj_title else []
     try:
         obj_dict = obj if obj is dict else obj.__dict__
         for k in obj_dict:
             v = "******" if k in masked_props else obj_dict[k]
             prop_list.append(f'{k}={v}')
         logger.debug("\n\t".join(prop_list))
     except Exception as err:
-        logger.error(f'[{fn()}] Failed: {err}')
+        logger.error(f'[{ex()}] Failed: {err}')
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description=__description__)
-    parser.add_argument(*aliases.get_aliases_str("userkey"), help="Mend user key", dest='ws_user_key',
-                        default=varenvs.get_env("wsuserkey"), required=not varenvs.get_env("wsuserkey"))
-    parser.add_argument(*aliases.get_aliases_str("apikey"), help="Mend API key", dest='ws_token',
-                        default=varenvs.get_env("wsapikey"), required=not varenvs.get_env("wsapikey"))
-    parser.add_argument(*aliases.get_aliases_str("projectkey"), help="Mend product/project scope", dest='scope_token',
-                        default=varenvs.get_env("wsscope"))
-    parser.add_argument(*aliases.get_aliases_str("sbom"), help="SBOM Report for upload (*.json|*.csv)", dest='sbom',
-                        required=True, default=os.environ.get("SBOM", ''))
-    parser.add_argument('--updateType', help="Update type", dest='update_type',
-                        default=os.environ.get("WS_UPDATETYPE", 'OVERRIDE'))
-    parser.add_argument(*aliases.get_aliases_str("output"), help="Output directory", dest='out_dir',
-                        default=os.getcwd())
-    parser.add_argument(*aliases.get_aliases_str("url"), help="Mend server URL", dest='ws_url',
-                        default=varenvs.get_env("wsurl"), required=not varenvs.get_env("wsurl"))
-    parser.add_argument('--offline', help="Create update request file without uploading", dest='offline',
-                        default=os.environ.get("WS_OFFLINE", 'false'))
-    arguments = parser.parse_args()
+    got_args = parser.parse_known_args()
+    if len(got_args[1]) == 1 and got_args[1][0] in ["--version", "-v"]:
+        parser.add_argument(*aliases.get_aliases_str("version"), help="Current version", action='store_true')
+    else:
+        parser.add_argument(*aliases.get_aliases_str("userkey"), help="Mend user key", dest='ws_user_key',
+                            default=varenvs.get_env("wsuserkey"), required=not varenvs.get_env("wsuserkey"))
+        parser.add_argument(*aliases.get_aliases_str("apikey"), help="Mend API key", dest='ws_token',
+                            default=varenvs.get_env("wsapikey"), required=not varenvs.get_env("wsapikey"))
+        parser.add_argument(*aliases.get_aliases_str("projectkey"), help="Mend product/project scope",
+                            dest='scope_token',
+                            default=varenvs.get_env("wsscope"))
+        parser.add_argument(*aliases.get_aliases_str("sbom"), help="SBOM Report for upload (*.json|*.csv)", dest='sbom',
+                            required=True, default=os.environ.get("SBOM", ''))
+        parser.add_argument('--updateType', help="Update type", dest='update_type',
+                            default=os.environ.get("WS_UPDATETYPE", 'OVERRIDE'))
+        parser.add_argument(*aliases.get_aliases_str("output"), help="Output directory", dest='out_dir',
+                            default=os.getcwd())
+        parser.add_argument(*aliases.get_aliases_str("url"), help="Mend server URL", dest='ws_url',
+                            default=varenvs.get_env("wsurl"), required=not varenvs.get_env("wsurl"))
+        parser.add_argument('--offline', help="Create update request file without uploading", dest='offline',
+                            default=os.environ.get("WS_OFFLINE", 'false'))
+        parser.add_argument('--multilang', help="Search library in all possible programming languages",
+                            dest='multilang',
+                            default=os.environ.get("WS_MULTILANG", 'true'))
+        parser.add_argument('--proxy', help="Proxy URL", dest='proxy',
+                            default=os.environ.get("HTTP_PROXY", ''))
+        parser.add_argument('--proxyUsername', help="Proxy Username", dest='proxyuser',
+                            default=os.environ.get("HTTP_PROXY_USERNAME", ''))
+        parser.add_argument('--proxyPassword', help="Proxy Password", dest='proxypsw',
+                            default=os.environ.get("HTTP_PROXY_PASSWORD", 'true'))
 
-    return arguments
+    return parser.parse_known_args()[0]
 
 
 def check_el_inlist(name: str) -> bool:  # Don't need to do this check now, might be needed in the future
     res = False
     for rel in relations:
         for key, value in rel.items():
             if 'SPDXRef-PACKAGE-' + name == value:
@@ -164,261 +185,370 @@
                 "originator": json_[el_]["originator"],
                 "homepage": json_[el_]["homepage"],
                 "filesAnalyzed": False,
                 "checksums": [{"algorithm": "SHA1", "checksumValue": json_[el_]["sha1"]}]
             }
             dep.append(pck)
     except Exception as err:
-        logger.error(f'[{fn()}] Failed to convert CSV to JSON: {err}')
+        logger.error(f'[{ex()}] Failed to convert CSV to JSON: {err}')
 
     return dep
 
 
+def call_api(header, data, agent=False, method="POST", agent_info_login=False):
+    res = ""
+    if not agent:
+        data["agentInfo"] = AGENT_INFO
+        if agent_info_login:
+            data["agentInfo"]["agent"] = AGENT_INFO["agent"].replace("ps-", "ps-login-")
+
+    try:
+        proxy = analyze_proxy(args.proxy) if args.proxy else ""
+        proxies = {"https": f"http://{proxy}", "http": f"http://{proxy}"} if proxy else {}
+        res = requests.request(
+            method=method,
+            url=f"{extract_url(args.ws_url)}/agent" if agent else f"{extract_url(args.ws_url)}/api/v{API_VERSION}",
+            data=data,
+            headers=header,
+            proxies=proxies).text
+    except Exception as err:
+        logger.debug(f'[{ex()}] {err}')
+    return res
+
+
 def create_body(args):
-    def create_add_sha1(langtype=""):  # maybe we will need to calculate additional sha1 later
+    def create_add_sha1(langtype: str, lib_name: str,
+                        lib_ver: str):  # maybe we will need to calculate additional sha1 later
         logger.debug(f'[{fn()}] langtype={langtype}')
         pkg_str = ""
         try:
             for ext_ref in package['externalRefs']:
                 if ext_ref['referenceCategory'] == "PACKAGE_MANAGER":
                     pkgname = re.search(r"pkg:(.*?)/", ext_ref['referenceLocator'], flags=re.DOTALL).group(1).strip()
                     lang_type = SHA1CalcType.get_package_type(f_t=pkgname)
-                    if lang_type.lower_case == "y":
-                        pkg_str = f"{package['name'].lower()}_{package['versionInfo'].lower()}_{lang_type.language}"
-                    else:
-                        pkg_str = f"{package['name']}_{package['versionInfo']}_{lang_type.language}"
+                    pkg_str = f"{lib_name.lower()}_{lib_ver.lower()}_{lang_type.language}" if lang_type.lower_case == "y" else f"{lib_name}_{lib_ver}_{lang_type.language} "
                     break
         except Exception as err:
-            if langtype == "":
-                return ""
-            else:
-                if SHA1CalcType.get_package_data(lng=langtype) == "y":
-                    pkg_str = f"{package['name'].lower()}_{package['versionInfo'].lower()}_{langtype}"
-                else:
-                    pkg_str = f"{package['name']}_{package['versionInfo']}_{langtype}"
-        return hashlib.sha1(pkg_str.encode("utf-8")).hexdigest()
+            pkg_str = f"{lib_name.lower()}_{lib_ver.lower()}_{langtype}" if SHA1CalcType.get_package_data(
+                lng=langtype) == "y" else f"{lib_name}_{lib_ver}_{langtype}"
+        return hashlib.sha1(pkg_str.encode("utf-8")).hexdigest() if langtype else ""
 
     def get_pkg_parent(pkg_child: str):  # Will be needed for uploading source files
         logger.debug(f'[{fn()}] pkg_child={pkg_child}')
         res = ""
         try:
             rels = sbom["relationships"]
             for rel_ in rels:
                 if rel_["relationshipType"] == "DYNAMIC_LINK" and rel_["relatedSpdxElement"] == pkg_child:
                     res = rel_["spdxElementId"]
                     break
         except:
             pass
         return res
 
+    def execute_pack_exe_list(package_list : list, exts : list): # Execute whole list of missed packages
+        res = []
+        for pck_ in package_list:
+            for pck_name, pck_ver in pck_.items():
+                logger.info(f'[{fn()}] Mend library search: {f"{pck_name}-{pck_ver}" if pck_ver else pck_name}')
+                res_err_msg = ""
+                br = False
+                for ext_ in exts:
+                    for key, value in ext_.items():
+                        if pkg_ver:
+                            sha1_, lname_, err_, err_msg_ = search_lib_by_name(lib_name=pck_name, lib_ver=pck_ver, lib_type=key)
+                            res_err_msg = err_msg_ if err_ == 3028 else res_err_msg  # Too many libraries were found
+                        else:
+                            sha1_ = ""
+                            lname_ = ""
+                            err_msg_ = ""
+                        # The start parallel running. Keep it for future
+                        #sha1_, lname_, err_, err_msg_, value = generic_thread_pool_search(lib_name=pkg_name,lib_ver=pkg_ver,l_types=lang_types,worker=search_lib_by_name)
+                        if sha1_:
+                            res.append( {
+                                "artifactId": f"{lname_}",
+                                "version": pkg_ver,
+                                "sha1": sha1_,
+                                "systemPath": "",
+                                "optional": False,
+                                "filename": f"{lname_}-{pkg_ver}.{value}",
+                                "checksums": {
+                                    "SHA1": sha1_
+                                },
+                                "dependencyFile": ""
+                            })
+                            br = True
+                    if br:
+                        break
+                if "NOASSERTION" not in pck_name and not sha1_:
+                    logger.info(f"Library not found: {f'{pck_name}-{pck_ver}' if pck_ver else pck_name}. {res_err_msg if res_err_msg else err_msg_}")
+        return res
+
     def search_lib_by_name(lib_name, lib_ver, lib_type):
         logger.debug(f'[{fn()}] Searching library: lib_name={lib_name}, lib_ver={lib_ver}, lib_type={lib_type}')
         sha1 = lname = ""
         error_code = 0
         error_msg = ""
         try:
-            lib_lst = web.WS.call_ws_api(self=args.ws_conn, request_type="getBasicLibraryInfo",
-                                         kv_dict={"libraryName": lib_name, "libraryVersion": lib_ver,
-                                                  "libraryType": lib_type})
-            for lib_ in lib_lst["librariesInformation"]:
-                sha1 = try_or_error(lambda: lib_["sha1"], '')
-                lname = try_or_error(lambda: lib_["artifactId"], '')
-                break
+            header = {"Content-Type": "application/json"}
+            data = json.dumps(
+                {"requestType": "getBasicLibraryInfo",
+                 "userKey": args.ws_user_key,
+                 "orgToken": args.ws_token,
+                 "libraryName": lib_name,
+                 "libraryVersion": lib_ver,
+                 "libraryType": lib_type})
+            lib_lst = json.loads(call_api(header=header, data=data))
+            try:
+                for lib_ in lib_lst["librariesInformation"]:
+                    sha1 = try_or_error(lambda: lib_["sha1"], '')
+                    lname = try_or_error(lambda: lib_["artifactId"], '')
+                    break
+            except:
+                if lib_lst["errorCode"] == 5001:  # User has no permissions. Don't need to continue execution
+                    logger.error(f'[{fn()}] Error Code: {lib_lst["errorCode"]}. Message: {lib_lst["errorMessage"]}')
+                    exit(-1)
+                else:
+                    logger.info(f'[{fn()}] {lib_lst["errorMessage"]}')
+                    error_code = lib_lst["errorCode"]
+                    error_msg = lib_lst["errorMessage"]
         except Exception as err:
-            error_code = json.loads(err.message[err.message.index("Error:")+6:])["errorCode"]  # Getting result as string, need to parse it
-            error_msg = json.loads(err.message[err.message.index("Error:")+6:])["errorMessage"]
-        logger.debug(f'[{fn()}] Result: sha1={sha1}, lname={lname}, error_code={error_code}, error_msg={error_msg}')
+            logger.error(f'[{ex()}] {str(err)}')
+            exit(-1)  # In this case don't need to continue execution
+        logger.debug(f'[{fn()}] Result: sha1={sha1}, libname={lname}, error_code={error_code}, error_msg={error_msg}')
         return sha1, lname, error_code, error_msg
 
+    def update_template_data(creator: str, lib_name: str, lib_ver: str):
+        lname_ = ""
+        lver_ = ""
+        ltype_ = ""
+        for tmpl_ in Templates:
+            if tmpl_.name in creator.lower():
+                lname_ = lib_name[lib_name.find(tmpl_.value[0]) + 1:]
+                ltype_ = lib_name[0:lib_name.find(tmpl_.value[0])]
+                for el_ver_ in tmpl_.value[1].split(","):
+                    lver_ = lver_.replace(el_ver_, "") if lver_ else lib_ver.replace(el_ver_, "")
+                break
+        return lname_.strip() if lname_ else lib_name, lver_.strip() if lver_ else lib_ver, ltype_
+
+    def get_lang_data(creator_):
+        for pkg_type_ in SHA1CalcType:
+            if pkg_type_.libtype in creator_.lower():
+                return pkg_type_
+        return None
+
     ts = round(datetime.datetime.now().timestamp())
     global relations
     global pkgs
     global added_el
     global sbom
     relations = []
     added_el = []
     dep = []
-    PrjID = args.ws_project if (not args.scope_token) else args.scope_token
-    logger.debug(f'[{fn()}] ts={ts}, PrjID={PrjID}')
+    pkg_top = ""
+    prj_id = args.ws_project if (not args.scope_token) else args.scope_token
+    logger.debug(f'[{fn()}] ts={ts}, prj_id={prj_id}')
 
     try:
         if os.path.splitext(args.sbom)[1] == ".csv":
             logger.debug(f'[{fn()}] Parsing CSV file: {args.sbom}')
             sbom = csv_to_json(args.sbom)
         else:
             logger.debug(f'[{fn()}] Parsing JSON file: {args.sbom}')
             with open(args.sbom, "r", encoding="utf-8") as f:
                 sbom = json.load(f)
-            PrjID = try_or_error(lambda: sbom["name"], '') if (not PrjID) else PrjID
-            logger.debug(f'[{fn()}] PrjID: {PrjID}')
+            prj_id = try_or_error(lambda: sbom["name"], '') if (not prj_id) else prj_id
+            logger.debug(f'[{fn()}] prj_id: {prj_id}')
     except Exception as err:
-        logger.error(f'[{fn()}] Unable to parse input file: {err}')
+        logger.error(f'[{ex()}] Unable to parse input file: {err}')
         exit(-1)
 
-    if PrjID == '' or PrjID is None:
+    if not prj_id:
         logger.error(f'[{fn()}] Scope must include either project name or project token')
         exit(-1)
 
     try:
         logger.debug(f'[{fn()}] Resolving dependency relationships')
         for rel_ in sbom["relationships"]:
             if rel_['relationshipType'] == "DEPENDS_ON":
                 relations.append({rel_['spdxElementId']: rel_['relatedSpdxElement']})
-    except AttributeError as err_a:
-        logger.debug(f'[{fn()}] "relationships" block not found, skipping')
+    except Exception as err:
+        logger.debug(f'[{ex()}] "relationships" block not found, skipping')
 
     pkgs = try_or_error(lambda: sbom["packages"], sbom)  # from JSON or from CSV
     logger.debug(f'[{fn()}] Adding dependencies')
+    creator = ""
+    for create_ in try_or_error(lambda: sbom["creationInfo"]["creators"], []):
+        if "Tool:" in create_:
+            creator = create_
     for package in pkgs:
-        sha1 = try_or_error(lambda: f"{package['checksums'][0]['checksumValue']}", '')
+        pkg_type_creator = get_lang_data(creator)  # Get info about possible package type from creator info
+        algorithm = try_or_error(lambda: f"{package['checksums'][0]['algorithm']}", '')
+        sha1 = try_or_error(lambda: f"{package['checksums'][0]['checksumValue']}",
+                            '') if algorithm == "SHA1" or algorithm == "SHA-1" else ""
+
         pkg_name = try_or_error(lambda: package["packageFileName"], package["name"])
         pkg_ver = try_or_error(lambda: package['versionInfo'], '')
+        pkg_name, pkg_ver, pkg_type = update_template_data(creator=creator, lib_name=pkg_name, lib_ver=pkg_ver)
+        # If we know how made library name by creation tool
         pkg_id = f'{pkg_name}-{pkg_ver}' if pkg_ver else pkg_name
+        download_loc = try_or_error(lambda: package["downloadLocation"], '')
+        if algorithm and not sha1:
+            logger.debug(f'[{fn()}] No SHA1 ({algorithm}) algorithm was found for library {pkg_name}')
 
         if sha1:
             pck = {
                 "artifactId": f"{pkg_name}",
                 "version": pkg_ver,
                 "sha1": sha1,
                 "systemPath": "",
                 "optional": False,
                 "filename": f"{pkg_name}",
                 "checksums": {
                     "SHA1": sha1
                 },
                 "dependencyFile": ""
             }
+            if pkg_name not in added_el:
+                added_el.append(pkg_name)  # we add element to list if was not added before
+                dep.append(add_child(pck))
+                logger.debug(f'[{fn()}] Dependency added: {pkg_id}, sha1: {sha1}')
         else:  # SHA1 not found
-            pck = {}
             lang_types = []
             logger.debug(f'[{fn()}] Attempting to resolve library by language type')
             try:
                 pck_ext = package["externalRefs"]  # execute SPDX structure file
                 # like cpe:2.3:a:python:botocore:1.22.12:*:*:*:*:*:*:*
                 for ext_ref in pck_ext:
                     if ext_ref["referenceCategory"] == "PACKAGE_MANAGER" or \
                             ext_ref['referenceCategory'] == "PACKAGE-MANAGER":
                         pkgname = re.search(r"pkg:(.*?)/", ext_ref['referenceLocator'],
                                             flags=re.DOTALL).group(1).strip()
                         pkg_data = SHA1CalcType.get_package_type(f_t=pkgname)
                         if pkg_data:
-                            lang_types.append({pkg_data.libtype: pkg_data.ext})
+                            lang_types.append((0, {pkg_data.libtype: pkg_data.ext}))
                             break
             except:
                 try:
                     if pkg_name != "NOASSERTION":
+                        if not pkg_type_creator and pkg_type:  # If nothing from creator but got package type from library name
+                            pkg_type_creator = try_or_error(lambda: SHA1CalcType.get_el_by_name(name=pkg_type), None)
                         ext_name = os.path.splitext(pkg_name)[1][1:]
-                        if ext_name == "":  # type of extension was not provided. Taken all possible types
-                            for calctype_ in SHA1CalcType:
-                                lang_types.append({calctype_.libtype: calctype_.ext})
+                        ext_name = ext_name if ext_name else os.path.splitext(download_loc)[1][1:]
+                        # Trying to get ext from download link if not found before
+                        type_lst = SHA1CalcType.get_package_type_list_by_ext(ext=ext_name) if ext_name else None
+                        if type_lst:
+                            for type_lst_ in type_lst:
+                                lang_types.append((0, {type_lst_.libtype: type_lst_.ext}))
                         else:
-                            type_lst = SHA1CalcType.get_package_type_list_by_ext(ext=ext_name)
-                            if type_lst == []:
+                            if args.multilang.lower() == "true" or not pkg_type_creator:
                                 for calctype_ in SHA1CalcType:  # Could not identify library extension
                                     # (could be part of the package name)
-                                    lang_types.append({calctype_.libtype: calctype_.ext})
+                                    lang_types.append((0 if calctype_.libtype == pkg_top else calctype_.order,
+                                                       {calctype_.libtype: calctype_.ext}))
                             else:
-                                for type_lst_ in type_lst:
-                                    lang_types.append({type_lst_.libtype: type_lst_.ext})
+                                lang_types.append((0 if pkg_type_creator.libtype == pkg_top else pkg_type_creator.order,
+                                                   {pkg_type_creator.libtype: pkg_type_creator.ext}))
                 except:
                     pass
 
             sha1_ = ""
             res_err_msg = ""
+            logger.info(f'[{fn()}] Mend library search: {pkg_id}')
+            lang_types.sort(key=lambda m: m[0])
             for l_type in lang_types:
-                for key, value in l_type.items():
+                for key, value in l_type[1].items():
                     if pkg_ver:
-                        logger.info(f'[{fn()}] Mend library search: {pkg_id}')
-                        sha1_, lname_, err_, err_msg_ = search_lib_by_name(lib_name=pkg_name, lib_ver=pkg_ver, lib_type=key)
+                        sha1_, lname_, err_, err_msg_ = search_lib_by_name(lib_name=pkg_name, lib_ver=pkg_ver,
+                                                                           lib_type=key)
                         res_err_msg = err_msg_ if err_ == 3028 else res_err_msg  # Too many libraries were found
                     else:
                         sha1_ = ""
                         lname_ = ""
                         err_msg_ = ""
-                if sha1_ != "":
+                if sha1_:
                     pck = {
                         "artifactId": f"{lname_}",
                         "version": pkg_ver,
                         "sha1": sha1_,
                         "systemPath": "",
                         "optional": False,
-                        "filename": f"{lname_}-{pkg_ver}.{value}",
+                        "filename": f"{lname_}-{pkg_ver}.{value}" if pkg_ver not in lname_ else lname_,
                         "checksums": {
                             "SHA1": sha1_
                         },
                         "dependencyFile": ""
                     }
+                    pkg_top = key
                     break
             if sha1_ == "" and pkg_name != "NOASSERTION":
                 logger.info(f"Library not found: {pkg_id}. {res_err_msg if res_err_msg else err_msg_}")
 
-        # if not check_el_inlist(pkg_name) and pck != {}:
         if pck != {}:
             if pkg_name not in added_el:
                 added_el.append(f"{pkg_name}")  # we add element to list if was not added before
                 dep.append(add_child(pck))
                 logger.debug(f'[{fn()}] Dependency added: {pkg_id}, sha1: {sha1}')
 
     logger.debug(f'[{fn()}] Constructing update request')
-    if args.scope_token == '' or args.scope_token is None:
+    if args.scope_token:
         prj = [
             {
-                "coordinates": {
-                    "artifactId": f"{PrjID}"
-                },
+                "projectToken": f"{args.scope_token}",
                 "dependencies": dep
             }
         ]
     else:
         prj = [
             {
-                "projectToken": f"{args.scope_token}",
+                "coordinates": {
+                    "artifactId": f"{prj_id}"
+                },
                 "dependencies": dep
             }
         ]
 
-    out = {
+    return {
         "updateType": f"{args.update_type}",
         "type": "UPDATE",
-        "agent": "fs-agent",
-        "agentVersion": "",
+        "agent": AGENT_INFO["agent"],
+        "agentVersion": AGENT_INFO["agentVersion"],
         "pluginVersion": "",
         "orgToken": f"{args.ws_token}",
         "userKey": f"{args.ws_user_key}",
         "product": f"{args.ws_product}",
         "productVersion": "",
         "timeStamp": ts,
         "projects": prj
     }
-    return out
 
 
-def get_files_from_pck(pck, sbom_f):
+def get_files_from_pck(pck, sbom_f): # Keep for future. Extracting files from Package
     file_lst = []
     try:
         f = pck['hasFiles']
         files = [*set(f)]
     except:
         files = []
     for file_ in files:
-        file_lst.append(get_file_by_spdx(file_,sbom_f))
+        file_lst.append(get_file_by_spdx(file_, sbom_f))
     return file_lst
 
 
 def get_file_by_spdx(spdx, sbom_f):
     file_data = {}
     sbom_f_ = None
     for d in sbom_f:
         if d['SPDXID'] == spdx:
             sbom_f_ = d
             break
 
     if sbom_f_:
-        sha1 = try_or_error(lambda: f"{sbom_f_['checksums'][0]['checksumValue']}","")
-        vers = try_or_error(lambda: f"{sbom_f_['versionInfo']}","")
+        sha1 = try_or_error(lambda: f"{sbom_f_['checksums'][0]['checksumValue']}", "")
+        vers = try_or_error(lambda: f"{sbom_f_['versionInfo']}", "")
         try:
             file_data = {
                 "artifactId": f"{spdx}",
                 "version": vers,
                 "sha1": sha1,
                 "systemPath": "",
                 "optional": False,
@@ -429,42 +559,48 @@
                 "dependencyFile": f"{sbom_f_['fileName']}"
             }
         except:
             pass
     return file_data
 
 
+def analyze_proxy(proxy: str):
+    proxy_ = proxy.replace("https://", "").replace("http://", "")
+    if "@" not in proxy_ and args.proxyuser and args.proxypsw:
+        proxy_ = f"{args.proxyuser}:{args.proxypsw}@" + proxy_
+    return proxy_
+
+
 def upload_to_mend(upload):
     ts = round(datetime.datetime.now().timestamp())
     ret = None
     try:
-        conn = http.client.HTTPSConnection(f"{extract_url(args.ws_url)[8:]}")
         json_prj = json.dumps(upload['projects'])  # API understands just JSON Array type, not simple List
         upload_projects = [proj["coordinates"]["artifactId"] for proj in upload["projects"]]
         if len(upload_projects) > 1:
             proj_txt = "\n  ".join(upload_projects)
             logger.debug(f'[{fn()}] Uploading projects:\n  {proj_txt}')
         else:
             logger.debug(f'[{fn()}] Uploading project:  {upload_projects[0]}')
 
-        payload = f"type=UPDATE&updateType={args.update_type}&agent=fs-agent&agentVersion=1.0&token={args.ws_token}&" \
-                  f"userKey={args.ws_user_key}&product={args.ws_product}&timeStamp={ts}&diff={json_prj}"
-        headers = {'Content-Type': 'application/x-www-form-urlencoded'}
-        conn.request("POST", "/agent", payload, headers)
-        data = json.loads(conn.getresponse().read())
+        data = f"type=UPDATE&updateType={args.update_type}&agent={AGENT_INFO['agent']}&" \
+               f"agentVersion={AGENT_INFO['agentVersion']}&token={args.ws_token}&userKey={args.ws_user_key}&" \
+               f"product={args.ws_product}&timeStamp={ts}&diff={json_prj}"
+        header = {'Content-Type': 'application/x-www-form-urlencoded'}
+        data = json.loads(call_api(header=header, data=data, agent=True))
+
         data_json = json.loads(data["data"])
         data_json["product"] = upload.get("product")
         logger.debug(f'[{fn()}] Response:\n{json.dumps(data_json, indent=2)}')
         if data['status'] == 1:
             ret = data_json
         else:
             logger.error(f"Mend update request failed: {data['message']} ({data['data']})")
-        conn.close()
     except Exception as err:
-        logger.error(f"Upload failed: {err}")
+        logger.error(f"[{ex()}] Upload failed: {err}")
     return ret
 
 
 def extract_url(url: str) -> str:
     url_ = url if url.startswith("https://") else f"https://{url}"
     url_ = url_.replace("http://", "")
     pos = url_.find("/", 8)  # Not using any suffix, just direct url
@@ -487,71 +623,74 @@
 
     args.ws_product = prd_name
     logger.debug(f'[{fn()}] Product name: {prd_name}')
 
     if prj_name:
         logger.debug(f'[{fn()}] Attempting to resolve project scope')
         try:
-            rt = WS.call_ws_api(self=args.ws_conn, request_type="getProjectVitals",
-                                kv_dict={"projectToken": prj_name})
+            header = {"Content-Type": "application/json"}
+            data = json.dumps(
+                {"requestType": "getProjectVitals",
+                 "userKey": args.ws_user_key,
+                 "orgToken": args.ws_token,
+                 "projectToken": prj_name
+                 })
+            rt = json.loads(call_api(header=header, data=data))
             args.scope_token = rt['projectVitals'][0]['token']
             args.ws_product = ""
             logger.debug(f'[{fn()}] Project token: {args.scope_token}')
         except:
             args.scope_token = ""
     args.ws_project = prj_name
     logger.debug(f'[{fn()}] Project name: {args.ws_project}')
 
 
 def main():
-    global output_json
     global args
     output_json = {}
 
-    hdr_title = f'{APP_TITLE} {__version__}'
-    hdr = f'\n{len(hdr_title)*"="}\n{hdr_title}\n{len(hdr_title)*"="}'
-    logger.info(hdr)
-
     try:
         args = parse_args()
-        log_obj_props(args, "Configuration:")
-
-        args.ws_conn = web.WSApp(url=f"{extract_url(args.ws_url)}",
-                                 user_key=args.ws_user_key,
-                                 token=args.ws_token,
-                                 tool_details=(f"ps-{__tool_name__.replace('_', '-')}", __version__))
-        log_obj_props(args.ws_conn, "WSApp connection:")
-
-        if not os.path.isfile(args.sbom):
-            logger.error(f'[{fn()}] Input file does not exist: {args.out_dir}')
-            exit(-1)
-
-        if not os.path.isdir(args.out_dir):
-            logger.info(f'[{fn()}] Creating output directory: {args.out_dir}')
-            try:
-                os.mkdir(args.out_dir)
-            except Exception as err:
-                logger.error(f'[{fn()}] {err}')
+        if try_or_error(lambda: args.version, False):
+            # Just show current version
+            print(f'{AGENT_INFO["agent"]} {AGENT_INFO["agentVersion"]}')
+            exit(0)
+        else:
+            hdr_title = f'{APP_TITLE} {AGENT_INFO["agentVersion"]}'
+            hdr = f'\n{len(hdr_title) * "="}\n{hdr_title}\n{len(hdr_title) * "="}'
+            logger.info(hdr)
+
+            log_obj_props(args, "Configuration:")
+            if not os.path.isfile(args.sbom):
+                logger.error(f'[{fn()}] Input file does not exist: {args.out_dir}')
                 exit(-1)
 
-        logger.info(f'[{fn()}] Generating update request')
-        full_path = os.path.join(args.out_dir, UPDATE_REQUEST_FILE)
-
-        logger.debug(f'[{fn()}] Resolving project scope')
-        analyse_scope(args.scope_token)
-
-        logger.debug(f'[{fn()}] Generating json body')
-        output_json = create_body(args)
-
-        logger.debug(f'[{fn()}] Creating update request file')
-        with open(full_path, 'w') as outfile:
-            json.dump(output_json, outfile, indent=4)
-        logger.info(f'[{fn()}] Update request created successfully: {full_path}')
+            if not os.path.isdir(args.out_dir):
+                logger.info(f'[{fn()}] Creating output directory: {args.out_dir}')
+                try:
+                    os.mkdir(args.out_dir)
+                except Exception as err:
+                    logger.error(f'[{ex()}] {err}')
+                    exit(-1)
+
+            logger.info(f'[{fn()}] Generating update request')
+            full_path = os.path.join(args.out_dir, UPDATE_REQUEST_FILE)
+
+            logger.debug(f'[{fn()}] Resolving project scope')
+            analyse_scope(args.scope_token)
+
+            logger.debug(f'[{fn()}] Generating json body')
+            output_json = create_body(args)
+
+            logger.debug(f'[{fn()}] Creating update request file')
+            with open(full_path, 'w') as outfile:
+                json.dump(output_json, outfile, indent=4)
+            logger.info(f'[{fn()}] Update request created successfully: {full_path}')
     except Exception as err:
-        logger.error(f'[{fn()}] Failed to create update request file: {err}')
+        logger.error(f'[{ex()}] Failed to create update request file: {err}')
         exit(-1)
 
     try:
         if args.offline.lower() == "false":
             logger.info(f'[{fn()}] Uploading data to Mend')
             res_upload = upload_to_mend(output_json)
             if res_upload:
@@ -573,12 +712,13 @@
                         res_txt = f'{res_txt}\n    {pj}'
                 elif len(proj_updated) > 0:
                     res_txt = f'{res_txt}\n  Project updated: {proj_updated[0]}'
                 logger.info(f'[{fn()}] {res_txt}')
                 logger.debug(f'[{fn()}] Request token: {res_upload["requestToken"]}')
 
     except Exception as err:
-        logger.error(f"Upload failed: {err}")
+        logger.error(f"[{ex()}] Upload failed: {err}")
+        exit(-1)
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

## Comparing `mend_import_sbom-23.3.1.dist-info/LICENSE` & `mend_import_sbom-23.7.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_import_sbom-23.3.1.dist-info/METADATA` & `mend_import_sbom-23.7.2.1.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,122 @@
 Metadata-Version: 2.1
 Name: mend-import-sbom
-Version: 23.3.1
+Version: 23.7.2.1
 Summary: Import SPDX or CSV SBOM into Mend
 Home-page: https://github.com/mend-toolkit/import-sbom
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools (~=65.5.1)
+Requires-Dist: DateTime (~=4.9)
+Requires-Dist: requests (~=2.28.2)
 
-[![Logo](https://resources.mend.io/mend-sig/logo/mend-dark-logo-horizontal.png)](https://www.mend.io/)  
+[![Logo](https://resources.mend.io/mend-sig/logo/mend-dark-logo-horizontal.png)](https://www.mend.io/)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
-[![CI](https://github.com/whitesource-ps/mend-import-sbom/actions/workflows/ci.yml/badge.svg)](https://github.com/whitesource-ps/mend-import-sbom/actions/workflows/ci.yml/badge.svg)
-[![GitHub release](https://img.shields.io/github/v/release/whitesource-ps/ws-import-sbom)](https://github.com/whitesource-ps/ws-import-sbom/releases/latest)  
+[![CI](https://github.com/mend-toolkit/import-sbom/actions/workflows/ci.yml/badge.svg)](https://github.com/mend-toolkit/import-sbom/actions/workflows/ci.yml/badge.svg)
+[![GitHub release](https://img.shields.io/github/v/release/mend-toolkit/import-sbom)](https://github.com/mend-toolkit/import-sbom/releases/latest)
 
 # Import SBOM
 
-A CLI tool that imports a project inventory into Mend from a SBOM report in the [SPDX](https://spdx.org) format or CSV format.  
+A CLI tool that imports a project inventory into Mend from a SBOM report in the [SPDX](https://spdx.org) format or CSV format.
 
 The tool can either upload data directly to Mend, or alternatively, create a Mend Offline Request file that can be uploaded separately using one of the following methods:
 - Using the Mend Unified Agent (see [Uploading an Offline Request File](https://docs.mend.io/bundle/unified_agent/page/scanning_with_the_unified_agent_in_offline_mode.html#Uploading-an-Offline-Request-File))
 - Via Mend's UI (**Admin** >> **Upload Update Request**)
 - Using Mend's API (see [Uploading Update Requests via the Mend API](https://docs.mend.io/bundle/wsk/page/uploading_update_requests_via_the_mend_api.html))
 
-The tool supports input files in either **JSON** or **CSV** formats.  
+The tool supports input files in either **JSON** or **CSV** formats.
 <hr>
 
-- [Supported Operating Systems](#supported-operating-systems)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Configuration Parameters](#configuration-parameters)
-- [Importing SPDX SBOM (JSON)](#importing-spdx-sbom-json)
-  - [Imported File Structure](#imported-file-structure)
-  - [Execution Examples](#execution-examples)
-- [Importing CSV SBOM](#importing-csv-sbom)
-  - [Imported File Structure](#imported-file-structure-1)
-  - [Execution Examples](#execution-examples-1)
+- [Import SBOM](#import-sbom)
+  - [Supported Operating Systems](#supported-operating-systems)
+  - [Prerequisites](#prerequisites)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Importing SPDX SBOM (JSON)](#importing-spdx-sbom-json)
+    - [Imported File Structure](#imported-file-structure)
+    - [Execution Examples](#execution-examples)
+  - [Importing CSV SBOM](#importing-csv-sbom)
+    - [Imported File Structure](#imported-file-structure-1)
+    - [Execution Examples](#execution-examples-1)
 
 <hr>
 
 ## Supported Operating Systems
 - **Linux (Bash):**	CentOS, Debian, Ubuntu
 - **Windows (PowerShell):**	10, 2012, 2016
 
 ## Prerequisites
 - Python 3.9+
 - Mend user with admin permissions
 
 ## Installation
-```
-$ pip install mend-import-sbom
+```shell
+pip install mend-import-sbom
 ```
 > **Note:** Depending on whether the package was installed as a root user or not, you need to make sure the package installation location was added to the `$PATH` environment variable.
 
 ## Usage
 **Using command-line arguments only:**
 ```shell
-import_sbom --user-key WS_USERKEY --api-key WS_APIKEY --url $WS_WSS_URL --input $SBOM_FILE_PATH --scope "ProductName//ProjectName" --dir $OUTPUT_DIRECTORY
+import_sbom --user-key $WS_USERKEY --api-key $WS_APIKEY --url $WS_WSS_URL --input $SBOM_FILE_PATH --scope "ProductName//ProjectName" --dir $OUTPUT_DIRECTORY
 ```
 **Using environment variables:**
 ```shell
 export WS_USERKEY=xxxxxxxxxxx
 export WS_APIKEY=xxxxxxxxxxx
 export WS_WSS_URL=https://saas.mend.io
 
 import_sbom --input $SBOM_FILE_PATH --scope "ProductName//ProjectName"
 ```
-> **Note:** Either form is accepted. For the rest of the examples, the latter form would be used  
+> **Note:** Either form is accepted. For the rest of the examples, the latter form would be used
 
 ## Configuration Parameters
->**Note:** Parameters can be specified as either command-line arguments, environment variables, or a combination of both.  
-> 
-> Command-line arguments take precedence over environment variables.  
-
-| CLI argument                   | Env. Variable   |   Type   | Required | Description                                                                              |
-|:-------------------------------|:----------------|:--------:|:--------:|:-----------------------------------------------------------------------------------------|
-| **&#x2011;&#x2011;help**       |                 | `switch` |    No    | Show help and exit                                                                       |
-| **&#x2011;&#x2011;user-key**   | `WS_USERKEY`    | `string` |   Yes    | Mend User Key                                                                            |
-| **&#x2011;&#x2011;api-key**    | `WS_APIKEY`     | `string` |   Yes    | Mend API Key                                                                             |
-| **&#x2011;&#x2011;url**        | `WS_WSS_URL`    | `string` |   Yes    | Mend Server URL                                                                          |
-| **&#x2011;&#x2011;input**      |                 | `string` |   Yes    | SBOM report file to import (`*.json` or `*.csv`)                                         |
-| **&#x2011;&#x2011;scope**      | `WS_SCOPE`      | `string` |   No*    | Product and Project names to create/update. Expected format: `"PRODUCT//PROJECT"`        |
-| **&#x2011;&#x2011;updateType** | `WS_UPDATETYPE` | `string` |    No    | APPEND or OVERRIDE results when importing into an existing project (default: `OVERRIDE`) |
-| **&#x2011;&#x2011;dir**        |                 | `string` |    No    | Output directory for the `update-request.txt` file** in Offline mode (default: `$PWD`)   |
-| **&#x2011;&#x2011;offline**    | `WS_OFFLINE`    |  `bool`  |    No    | Create offline update request file without uploading to Mend (default: `false`)          |
-
-> \* `--scope` specifies the hierarchy (full or partial) for uploading the SBOM report using product and project identifiers.  
-> Both the product and project can be identified by either names (for creating a new one) or token (for updating an existing one).  
->   
-> * `--scope "ProductName//ProjectName"` would specify both the product name and project name to create/update.  
-> * `--scope "ProjectName"` would specify only the project name, and the product name would default to `Mend-Imports`.  
-> * `--scope "ProjectToken"` would specify the token of an existing project, and the product name would default to that project's parent product. When specifying a project token, you cannot specify a product name/token.  
+>**Note:** Parameters can be specified as either command-line arguments, environment variables, or a combination of both.
+>
+> Command-line arguments take precedence over environment variables.
+
+| CLI argument                      | Env. Variable          |   Type   | Required | Description                                                                                                                                                                                       |
+|:----------------------------------|:-----------------------|:--------:|:--------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **&#x2011;&#x2011;help**          |                        | `switch` |    No    | Show help and exit                                                                                                                                                                                |
+| **&#x2011;&#x2011;version**       |                        | `switch` |    No    | Show current version and exit                                                                                                                                                                     |
+| **&#x2011;&#x2011;user-key**      | `WS_USERKEY`           | `string` |   Yes    | Mend User Key                                                                                                                                                                                     |
+| **&#x2011;&#x2011;api-key**       | `WS_APIKEY`            | `string` |   Yes    | Mend API Key                                                                                                                                                                                      |
+| **&#x2011;&#x2011;url**           | `WS_WSS_URL`           | `string` |   Yes    | Mend Server URL                                                                                                                                                                                   |
+| **&#x2011;&#x2011;input**         | `SBOM`                 | `string` |   Yes    | SBOM report file to import (`*.json` or `*.csv`)                                                                                                                                                  |
+| **&#x2011;&#x2011;scope**         | `WS_SCOPE`             | `string` |   No*    | Product and Project names to create/update. Expected format: `"PRODUCT//PROJECT"`                                                                                                                 |
+| **&#x2011;&#x2011;updateType**    | `WS_UPDATETYPE`        | `string` |    No    | APPEND or OVERRIDE results when importing into an existing project (default: `OVERRIDE`)                                                                                                          |
+| **&#x2011;&#x2011;dir**           |                        | `string` |    No    | Output directory for the `update-request.txt` file** in Offline mode (default: `$PWD`)                                                                                                            |
+| **&#x2011;&#x2011;offline**       | `WS_OFFLINE`           |  `bool`  |    No    | Create offline update request file without uploading to Mend (default: `false`)                                                                                                                   |
+| **&#x2011;&#x2011;multilang**     | `WS_MULTILANG`         |  `bool`  |   No**   | In case no SHA1 searching library by All known package types (default: `true`)                                                                                                                    |
+| **&#x2011;&#x2011;proxy**         | `HTTP_PROXY`           | `string` |    No    | Proxy host including port, with or without protocol prefix and optionally credentials. Expected formats:myproxy.host.com:1234,http://myproxy.host.com:1234,http://user:pass@myproxy.host.com:1234 |
+| **&#x2011;&#x2011;proxyUsername** | `HTTP_PROXY_USERNAME`  | `string` |    No    | Proxy username, if needed and if not included in the proxy host.                                                                                                                                  |
+| **&#x2011;&#x2011;proxyPassword** | `HTTP_PROXY_PASSWORD`  | `string` |    No    | Proxy password, if needed and if not included in the proxy host.                                                                                                                                  |
+
+
+> \* `--scope` specifies the hierarchy (full or partial) for uploading the SBOM report using product and project identifiers.
+> Both the product and project can be identified by either names (for creating a new one) or token (for updating an existing one).
+>
+> * `--scope "ProductName//ProjectName"` would specify both the product name and project name to create/update.
+> * `--scope "ProjectName"` would specify only the project name, and the product name would default to `Mend-Imports`.
+> * `--scope "ProjectToken"` would specify the token of an existing project, and the product name would default to that project's parent product. When specifying a project token, you cannot specify a product name/token.
 > * If `--scope` isn't specified, the project name will be taken from the SBOM's `name` property (for `*.json` SPDX) or its parent directory (for `*.csv`).
->  
-> ** See more details about the [update-request.txt](https://docs.mend.io/bundle/wsk/page/does_mend_have_the_ability_to_scan_when_offline_and_then_upload_the_scan_results_when_online_.html) file and [Offline mode](https://docs.mend.io/csh?context=2524153159&topicname=unified_agent_-_advanced_topics.html#Scanning-in-Offline-Mode)  in Mend's documentation.  
+>
+> ** See more details about the [update-request.txt](https://docs.mend.io/bundle/wsk/page/does_mend_have_the_ability_to_scan_when_offline_and_then_upload_the_scan_results_when_online_.html) file and [Offline mode](https://docs.mend.io/csh?context=2524153159&topicname=unified_agent_-_advanced_topics.html#Scanning-in-Offline-Mode)  in Mend's documentation.
 
+> \** If `--multilang` is False script will try to find relevant package name in the Creator field. If such a candidate is found just it will be used for searching libraries.
 
 ## Importing SPDX SBOM (JSON)
 
 ### Imported File Structure
 The SPDX document must correspond to the [Composition of an SPDX document](https://spdx.github.io/spdx-spec/v2.3/composition-of-an-SPDX-document) specification.
 
 The following table describes the set of properties for each imported library:
@@ -123,46 +132,48 @@
 | **versionInfo**          |   Yes*   | [Version Info](https://spdx.github.io/spdx-spec/v2.3/package-information/#73-package-version-field)                      |
 | **packageFileName**      |   Yes*   | [Package Name](https://spdx.github.io/spdx-spec/v2.3/package-information/#74-package-file-name-field)                    |
 | **supplier**             |    No    | [Supplier](https://spdx.github.io/spdx-spec/v2.3/package-information/#75-package-supplier-field)                         |
 | **originator**           |    No    | [Originator](https://spdx.github.io/spdx-spec/v2.3/package-information/#76-package-originator-field)                     |
 | **sha1**                 |   Yes*   | [SHA1](https://spdx.github.io/spdx-spec/v2.3/package-information/#710-package-checksum-field)                            |
 | **homepage**             |    No    | [Home Page](https://spdx.github.io/spdx-spec/v2.3/package-information/#711-package-home-page-field)                      |
 
-> \* Each library requires either **sha1** or the **packageFileName** and **versionInfo** pair. 
+> \* Each library requires either **sha1** or the **packageFileName** and **versionInfo** pair.
+>
+>    **Note:** If **sha1** isn't provided for a particular library, the tool will attempt to search that library by its name and version in Mend's index, which will result in longer execution times.
 
 ### Execution Examples
 
-> **Note:** In the following examples, $WS_USERKEY, $WS_APIKEY and $WS_WSS_URL are assumed to have been exported as environment variables.  
+> **Note:** In the following examples, $WS_USERKEY, $WS_APIKEY and $WS_WSS_URL are assumed to have been exported as environment variables.
 
 Import SPDX SBOM into a new Mend project
 
 ```shell
-$ import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME-sbom.json
+import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME-sbom.json
 ```
 
 Convert SPDX SBOM to an [offline update request](https://docs.mend.io/bundle/wsk/page/understanding_update_requests.html) file for creating a new Mend project under a specific product
 
 ```shell
-$ import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True
+import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True
 ```
 
 Convert SPDX SBOM to an [offline update request](https://docs.mend.io/bundle/wsk/page/understanding_update_requests.html) file for overriding an existing Mend project
 
 ```shell
-$ import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True
+import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True
 
-$ import_sbom --scope $WS_PROJECTTOKEN --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True
+import_sbom --scope $WS_PROJECTTOKEN --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True
 ```
 
 Convert SPDX SBOM to an [offline update request](https://docs.mend.io/bundle/wsk/page/understanding_update_requests.html) file for appending to an existing Mend project
 
 ```shell
-$ import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True --updateType APPEND
+import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True --updateType APPEND
 
-$ import_sbom --scope $WS_PROJECTTOKEN --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True --updateType APPEND
+import_sbom --scope $WS_PROJECTTOKEN --dir $HOME/reports --input $HOME/reports/my-project-sbom.json --offline True --updateType APPEND
 ```
 
 ## Importing CSV SBOM
 
 ### Imported File Structure
 
 [Download CSV Template](./templates/import_template.csv)
@@ -179,27 +190,27 @@
 | packageFileName      | Yes*     | [Package Name](https://spdx.github.io/spdx-spec/v2.3/package-information/#74-package-file-name-field)                    |
 | supplier             | No       | [Supplier](https://spdx.github.io/spdx-spec/v2.3/package-information/#75-package-supplier-field)                         |
 | originator           | No       | [Originator](https://spdx.github.io/spdx-spec/v2.3/package-information/#76-package-originator-field)                     |
 | sha1                 | Yes*     | [SHA1](https://spdx.github.io/spdx-spec/v2.3/package-information/#710-package-checksum-field)                            |
 | homepage             | No       | [Home Page](https://spdx.github.io/spdx-spec/v2.3/package-information/#711-package-home-page-field)                      |
 
 > \* Each library requires either **sha1** or the **packageFileName** and **versionInfo** pair. Other fields can remain empty.
+>
+>    **Note:** If **sha1** isn't provided for a particular library, the tool will attempt to search that library by its name and version in Mend's index, which will result in longer execution times.
 
 ### Execution Examples
 
 > **Note:** In the following examples, $WS_USERKEY, $WS_APIKEY and $WS_WSS_URL are assumed to have been exported as environment variables.
 
 Import CSV SBOM into a new Mend project under the default product (`Mend-Imports`)
 
 ```shell
-$ import_sbom --scope "$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME.csv
+import_sbom --scope "$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME.csv
 ```
 
 Import CSV SBOM, appending to an existing Mend project
 
 ```shell
-$ import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME.csv --updateType APPEND 
+import_sbom --scope "$WS_PRODUCTNAME//$WS_PROJECTNAME" --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME.csv --updateType APPEND
 
-$ import_sbom --scope $WS_PROJECTTOKEN --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME.csv --updateType APPEND
+import_sbom --scope $WS_PROJECTTOKEN --dir $HOME/reports --input $HOME/reports/$WS_PROJECTNAME.csv --updateType APPEND
 ```
-
-
```

## Comparing `mend_import_sbom-23.3.1.dist-info/RECORD` & `mend_import_sbom-23.7.2.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mend_import_sbom/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_import_sbom/_version.py,sha256=Qx0vdx6LPee3cLGkoB2p7_cjeWO3SYG7j0YDW4HEhBo,107
+mend_import_sbom/_version.py,sha256=OYQmEkQ29RTpd_kHS5CdFtNprMsskf9WsI436KKQFcs,109
 mend_import_sbom/conftest.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_import_sbom/import_const.py,sha256=0CX97MZbiHrDPqqFpk4slgfIPeX26S-gS5DZMhOmmP4,3111
-mend_import_sbom/import_sbom.py,sha256=m_U2HEm2Z_OcNeB3tVCqmvC59UKP36TGC9AC7e78vOY,23640
-mend_import_sbom-23.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_import_sbom-23.3.1.dist-info/METADATA,sha256=thGn7ZFHBij-yZDFKUD3FNuaNiYfqFfSvAdqXYNkbnk,14205
-mend_import_sbom-23.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mend_import_sbom-23.3.1.dist-info/entry_points.txt,sha256=TwhF3Td3D_QJA-8HCfANmh23Cz2MezvO_TBWbnXvx2s,67
-mend_import_sbom-23.3.1.dist-info/top_level.txt,sha256=ZouDaDSH2LvREekb4c6gJ223aeSyOSQTgvWoSpBGhYE,17
-mend_import_sbom-23.3.1.dist-info/RECORD,,
+mend_import_sbom/import_const.py,sha256=ZPsQ48tUN2oTCkihPB_0RrLx7R0N_wNRnvPr_IrOTpU,3447
+mend_import_sbom/import_sbom.py,sha256=O2Bi-uoHAinbTwLr-SjONqttW8B16EHJrfXFDo-MJAw,31219
+mend_import_sbom-23.7.2.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_import_sbom-23.7.2.1.dist-info/METADATA,sha256=dFad7XVdBXZEIMftDAjtmJTG9b3KaLlL1bgbw3xEcn4,17460
+mend_import_sbom-23.7.2.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+mend_import_sbom-23.7.2.1.dist-info/entry_points.txt,sha256=n2REmj74MtlyWYzsIU7TDv4JVK65nGHE4pntFX9RJFU,66
+mend_import_sbom-23.7.2.1.dist-info/top_level.txt,sha256=ZouDaDSH2LvREekb4c6gJ223aeSyOSQTgvWoSpBGhYE,17
+mend_import_sbom-23.7.2.1.dist-info/RECORD,,
```

