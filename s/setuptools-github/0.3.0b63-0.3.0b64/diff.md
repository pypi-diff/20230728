# Comparing `tmp/setuptools-github-0.3.0b63.tar.gz` & `tmp/setuptools-github-0.3.0b64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.0b63.tar", last modified: Tue Jul 25 22:13:35 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.0b64.tar", last modified: Fri Jul 28 19:05:01 2023, max compression
```

## Comparing `setuptools-github-0.3.0b63.tar` & `setuptools-github-0.3.0b64.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.588287 setuptools-github-0.3.0b63/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.588287 setuptools-github-0.3.0b63/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.689865 setuptools-github-0.3.0b64/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 19:05:01.000000 setuptools-github-0.3.0b64/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 19:05:01.693865 setuptools-github-0.3.0b64/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-28 19:04:32.000000 setuptools-github-0.3.0b64/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.0b63/LICENSE` & `setuptools-github-0.3.0b64/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b63/setup.py` & `setuptools-github-0.3.0b64/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: BSD License",
     ],
 )
```

### Comparing `setuptools-github-0.3.0b63/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.0b64/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b63/src/setuptools_github/checks.py` & `setuptools-github-0.3.0b64/src/setuptools_github/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from pathlib import Path
-from typing import List, Callable, Dict, TypeVar
+from typing import Callable, Dict, List, TypeVar
 
 from mypy_extensions import Arg, DefaultArg
 
 from . import tools
 
 BETAEXPR = re.compile(r"beta/(?P<ver>\d+([.]\d+)*)")
 
@@ -18,15 +18,15 @@
         ],
         None,
     ],
 )
 
 
 def check_repo_mods(error: ErrorFunctionType, workdir: Path, initfile: Path):
-    from pygit2 import Repository, GIT_STATUS_WT_NEW, GIT_STATUS_IGNORED  # type: ignore
+    from pygit2 import GIT_STATUS_IGNORED, GIT_STATUS_WT_NEW, Repository  # type: ignore
 
     repo = Repository(workdir)
 
     rel_initfile = str(initfile.absolute().relative_to(workdir.absolute())).replace(
         "\\", "/"
     )
     unstracked = {p for p, f in repo.status().items() if f & GIT_STATUS_WT_NEW}
```

### Comparing `setuptools-github-0.3.0b63/src/setuptools_github/cli.py` & `setuptools-github-0.3.0b64/src/setuptools_github/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
+
 import argparse
-import logging
 import functools
+import logging
 import sys
 from typing import Any, Callable, Protocol
+
 from . import tools
 
 
 class ErrorFn(Protocol):
     def __call__(self, message: str, explain: str | None, hint: str | None) -> None:
         ...
 
 
-class AbortExecution(Exception):
+class AbortExecutionError(Exception):
     @staticmethod
     def _strip(txt):
         txt = txt or ""
         txt = txt[1:] if txt.startswith("\n") else txt
         txt = tools.indent(txt, pre="")
         return txt[:-1] if txt.endswith("\n") else txt
 
@@ -109,26 +111,26 @@
 
                 def error(
                     message: str,
                     explain: str = "",
                     hint: str = "",
                     usage: str | None = None,
                 ):
-                    raise AbortExecution(message, explain, hint, usage)
+                    raise AbortExecutionError(message, explain, hint, usage)
 
                 errorfn: ErrorFn = functools.partial(error, usage=parser.format_usage())
                 options.error = errorfn
 
                 options = _process_options(options, errorfn) or options
                 if process_options:
                     options = process_options(options, errorfn) or options
 
                 return main(options)
-            except AbortExecution as exc:
-                print(str(exc), file=sys.stderr)
-                raise SystemExit(2)
+            except AbortExecutionError as err:
+                print(str(err), file=sys.stderr)  # noqa: T201
+                raise SystemExit(2) from None
             except Exception:
                 raise
 
         return _fn1
 
     return _fn
```

### Comparing `setuptools-github-0.3.0b63/src/setuptools_github/scm.py` & `setuptools-github-0.3.0b64/src/setuptools_github/scm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 from __future__ import annotations
+
+import dataclasses as dc
 import io
 import re
-import dataclasses as dc
 import subprocess
 from pathlib import Path
-
+from typing import Any, List, Union
 
 from typing_extensions import TypeAlias
-from typing import Union, List, Any
-
 
 ListOfArgs: TypeAlias = Union[str, Path, List[Union[str, Path]]]
 
 
 def to_list_of_paths(paths: ListOfArgs) -> list[Path]:
     return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
 
+def indent(txt: str, pre: str = " " * 2) -> str:
+    "simple text indentation"
+
+    from textwrap import dedent
+
+    txt = dedent(txt)
+    if txt.endswith("\n"):
+        last_eol = "\n"
+        txt = txt[:-1]
+    else:
+        last_eol = ""
+
+    result = pre + txt.replace("\n", "\n" + pre) + last_eol
+    return result if result.strip() else result.strip()
+
+
 def shorthand(txt: str) -> str:
     tag = "refs/heads/"
     return txt[len(tag) :] if txt.startswith(tag) else txt
 
 
 class NA:
     pass
 
 
 class GitError(Exception):
     pass
 
 
+class InvalidGitRepoError(GitError):
+    pass
+
+
 @dc.dataclass
 class GitRepoBranches:
     local: list[str]
     remote: list[str]
 
 
 @dc.dataclass
 class GitRepoHead:
     @dc.dataclass
     class GitRepoHeadHex:
-        hex: str
+        hex: str  # noqa: A003
 
     name: str
     target: GitRepoHeadHex
 
     @property
     def shorthand(self):
         return shorthand(self.name)
@@ -66,22 +85,20 @@
                     "--work-tree",
                     str(self.workdir),
                     "--git-dir",
                     str(self.gitdir),
                 ]
             )
         arguments.extend(str(c) for c in cmds)
-        return subprocess.check_output(arguments, encoding="utf-8")
+        return subprocess.check_output(arguments, encoding="utf-8")  # noqa: S603
 
     def __truediv__(self, other):
         return (self.workdir / other).absolute()
 
-    def dumps(self, mask=False) -> str:
-        from setuptools_github.tools import indent
-
+    def dumps(self, mask: bool = False) -> str:
         lines = f"REPO: {self.workdir}"
         lines += "\n [status]\n" + indent(self(["status"]))
         branches = self(["branch", "-avv"])
         if mask:
             branches = re.sub(r"(..\w\s+)\w{7}(\s+.*)", r"\1ABCDEFG\2", branches)
         lines += "\n [branch]\n" + indent(branches)
         lines += "\n [tags]\n" + indent(self(["tag", "-l"]))
@@ -126,20 +143,25 @@
         try:
             txt = self(["rev-parse", name]).strip()
         except subprocess.CalledProcessError as exc:
             raise GitError(f"no branch '{name}'") from exc
         return GitRepoHead(name=name, target=GitRepoHead.GitRepoHeadHex(txt))
 
     def status(
-        self, untracked_files: str = "all", ignored: bool = False
+        self,
+        untracked_files: str = "all",
+        ignored: bool = False,
     ) -> dict[str, int]:
+        # to update the mapping:
+        # pygit2.Repository(self.workdir).status()
         mapper = {
             "??": 128 if untracked_files == "all" else None,
             " D": 512,
             " M": 256,
+            "A ": 1,
         }
         result = {}
         try:
             txt = self(["status", "--porcelain"])
         except subprocess.CalledProcessError as exc:
             raise GitError("invalid repo") from exc
         for line in txt.split("\n"):
@@ -160,15 +182,16 @@
         self(["add", *all_paths])
         self(["commit", "-m", message, *all_paths])
 
     def branch(self, name: str | None = None, origin: str = "master") -> str:
         if not name:
             name = self.head.name or ""
             return name[11:] if name.startswith("refs/heads/") else name
-        assert origin or origin is None
+        if not (origin or origin is None):
+            raise RuntimeError(f"invalid {origin=}")
         old = self.branch()
         self(["checkout", "-b", name, "--track", origin])
         return old[11:] if old.startswith("refs/heads/") else old
 
     @property
     def branches(self) -> GitRepoBranches:
         result = GitRepoBranches([], [])
@@ -190,15 +213,15 @@
             for line in self(["tag", "-l"]).split("\n")
             if line.strip()
         ]
 
     def clone(
         self,
         dest: str | Path,
-        force=False,
+        force: bool = False,
         branch: str | None = None,
     ) -> GitRepo:
         from shutil import rmtree
 
         workdir = Path(dest).absolute()
         if force:
             rmtree(workdir, ignore_errors=True)
```

### Comparing `setuptools-github-0.3.0b63/src/setuptools_github/script.py` & `setuptools-github-0.3.0b64/src/setuptools_github/script.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 
 Or will release the beta branch and will move inot the next minor
 
     setuptools-github {major|minor|micro} ./src/setuptools_github/__init__.py
 
 """
 from __future__ import annotations
+
+import argparse
 import logging
 import re
 import sys
 from pathlib import Path
-import argparse
-from . import cli, tools, scm
 
+from . import cli, scm, tools
 
 log = logging.getLogger(__name__)
 
 
 def add_arguments(parser: argparse.ArgumentParser):
     parser.add_argument("--master", help="the 'master' branch")
     parser.add_argument(
@@ -74,16 +75,17 @@
 
     if options.repo.status(untracked_files="no", ignored=False):
         options.error(f"modified files in {options.repo.workdir}")
     if not options.initfile.exists():
         options.error(f"cannot find version file {options.initfile}")
 
     version = tools.get_module_var(options.initfile, "__version__")
-    assert version
     log.info("got version %s for branch '%s'", version, options.repo.head.shorthand)
+    if not version:
+        raise tools.InvalidVersionError(f"cannot find a version in {options.initfile}")
 
     # fetching all remotes
     options.repo(["fetch", "--all"])
 
     if options.mode == "make-beta":
         if options.repo.head.name != f"refs/heads/{master}":
             options.error(
@@ -122,15 +124,15 @@
         tools.set_module_var(options.initfile, "__version__", new_version)
 
         # commit
         options.repo.commit(
             options.initfile, f"version bump {version} -> {new_version}"
         )
 
-        print(
+        print(  # noqa: T201
             tools.indent(
                 f"""
         The release is almost complete.
 
         To proceed:
             git push origin release/{version}
```

### Comparing `setuptools-github-0.3.0b63/src/setuptools_github/tools.py` & `setuptools-github-0.3.0b64/src/setuptools_github/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from __future__ import annotations
 
-import re
 import ast
 import json
-
+import re
 from pathlib import Path
-from typing import Any, Union, Tuple, Optional
+from typing import Any
 
 from . import scm
 
 
-class GithubError(Exception):
+class ToolsError(Exception):
     pass
 
 
-class MissingVariable(GithubError):
+class ValidationError(ToolsError):
     pass
 
 
-class InvalidGithubReference(GithubError):
+class InvalidVersionError(ToolsError):
     pass
 
 
-class AbortExecution(Exception):
+class MissingVariableError(ToolsError):
+    pass
+
+
+class AbortExecutionError(Exception):
     @staticmethod
     def _strip(txt):
         txt = txt or ""
         txt = txt[1:] if txt.startswith("\n") else txt
         txt = indent(txt, pre="")
         return txt[:-1] if txt.endswith("\n") else txt
 
     def __init__(
-        self, message: str, explain: Optional[str] = None, hint: Optional[str] = None
+        self, message: str, explain: str | None = None, hint: str | None = None
     ):
         self.message = message.strip()
         self._explain = explain
         self._hint = hint
 
     @property
     def explain(self):
@@ -60,15 +63,16 @@
     from shutil import rmtree
     from stat import S_IWUSR
 
     if name == "nt":
         for p in path.rglob("*"):
             p.chmod(S_IWUSR)
     rmtree(path, ignore_errors=True)
-    assert not path.exists()
+    if path.exists():
+        raise RuntimeError(f"cannot remove {path=}")
 
 
 def indent(txt: str, pre: str = " " * 2) -> str:
     "simple text indentation"
 
     from textwrap import dedent
 
@@ -84,16 +88,16 @@
 
 
 def list_of_paths(paths: str | Path | list[str | Path]) -> list[Path]:
     return [Path(s) for s in ([paths] if isinstance(paths, (str, Path)) else paths)]
 
 
 def get_module_var(
-    path: Union[Path, str], var: str = "__version__", abort=True
-) -> Optional[str]:
+    path: Path | str, var: str = "__version__", abort=True
+) -> str | None:
     """extract from a python module in path the module level <var> variable
 
     Args:
         path (str,Path): python module file to parse using ast (no code-execution)
         var (str): module level variable name to extract
         abort (bool): raise MissingVariable if var is not present
 
@@ -108,28 +112,27 @@
     """
 
     class V(ast.NodeVisitor):
         def __init__(self, keys):
             self.keys = keys
             self.result = {}
 
-        def visit_Module(self, node):
+        def visit_Module(self, node):  # noqa: N802
             # we extract the module level variables
             for subnode in ast.iter_child_nodes(node):
                 if not isinstance(subnode, ast.Assign):
                     continue
                 for target in subnode.targets:
                     if target.id not in self.keys:
                         continue
-                    assert isinstance(
-                        subnode.value, (ast.Num, ast.Str, ast.Constant)
-                    ), (
-                        f"cannot extract non Constant variable "
-                        f"{target.id} ({type(subnode.value)})"
-                    )
+                    if not isinstance(subnode.value, (ast.Num, ast.Str, ast.Constant)):
+                        raise ValidationError(
+                            f"cannot extract non Constant variable "
+                            f"{target.id} ({type(subnode.value)})"
+                        )
                     if isinstance(subnode.value, ast.Str):
                         value = subnode.value.s
                     elif isinstance(subnode.value, ast.Num):
                         value = subnode.value.n
                     else:
                         value = subnode.value.value
                     self.result[target.id] = value
@@ -137,21 +140,21 @@
 
     v = V({var})
     path = Path(path)
     if path.exists():
         tree = ast.parse(Path(path).read_text())
         v.visit(tree)
     if var not in v.result and abort:
-        raise MissingVariable(f"cannot find {var} in {path}", path, var)
+        raise MissingVariableError(f"cannot find {var} in {path}", path, var)
     return v.result.get(var, None)
 
 
 def set_module_var(
-    path: Union[str, Path], var: str, value: Any, create: bool = True
-) -> Tuple[Any, str]:
+    path: str | Path, var: str, value: Any, create: bool = True
+) -> tuple[Any, str]:
     """replace var in path with value
 
     Args:
         path (str,Path): python module file to parse
         var (str): module level variable name to extract
         value (None or Any): if not None replace var in initfile
         create (bool): create path if not present
@@ -218,15 +221,15 @@
     elif mode == "micro":
         newver[-1] += 1
     return ".".join(str(v) for v in newver)
 
 
 def update_version(
     initfile: str | Path, github_dump: str | None = None, abort: bool = True
-) -> Optional[str]:
+) -> str | None:
     """extracts version information from github_dump and updates initfile in-place
 
     Args:
         initfile (str, Path): path to the __init__.py file with a __version__ variable
         github_dump (str): the os.getenv("GITHUB_DUMP") value
 
     Returns:
@@ -234,15 +237,15 @@
     """
 
     path = Path(initfile)
     repo = scm.lookup(path)
 
     if not (repo or github_dump):
         if abort:
-            raise GithubError(f"cannot find a valid git repo for {path}")
+            raise scm.InvalidGitRepoError(f"cannot find a valid git repo for {path}")
         return get_module_var(path, "__version__")
 
     if not github_dump and repo:
         gdata = {
             "ref": repo.head.name,
             "sha": repo.head.target.hex[:7],
             "run_number": 0,
@@ -258,17 +261,17 @@
     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
 
     if match := expr.search(gdata["ref"]):
         # setuptools double calls the update_version,
         # this fixes the issue
         match1 = expr1.search(current or "")
         if not match1:
-            raise InvalidGithubReference(f"cannot parse current version '{current}'")
+            raise InvalidVersionError(f"cannot parse current version '{current}'")
         if match1.group("version") != match.group("version"):
-            raise InvalidGithubReference(
+            raise InvalidVersionError(
                 f"building package for {current} from '{gdata['ref']}' "
                 f"branch ({match.groupdict()} mismatch {match1.groupdict()})"
             )
         if match.group("what") == "beta":
             version = f"{match1.group('version')}b{gdata['run_number']}"
 
     short = gdata["sha"] + ("*" if dirty else "")
```

### Comparing `setuptools-github-0.3.0b63/tests/conftest.py` & `setuptools-github-0.3.0b64/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b63/tests/test_checks.py` & `setuptools-github-0.3.0b64/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b63/tests/test_cli.py` & `setuptools-github-0.3.0b64/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools_github import cli
 
 
 def test_exception():
-    obj = cli.AbortExecution(
+    obj = cli.AbortExecutionError(
         message="this is a short one-liner",
         explain="""
           It looks the repository doesn't have any branch,
           you should:
             git checkout --orphan <branch-name>
           """,
         hint="create a git branch",
```

### Comparing `setuptools-github-0.3.0b63/tests/test_conftest.py` & `setuptools-github-0.3.0b64/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b63/tests/test_scm.py` & `setuptools-github-0.3.0b64/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b63/tests/test_script.py` & `setuptools-github-0.3.0b64/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b63/tests/test_tools.py` & `setuptools-github-0.3.0b64/tests/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
         "ref": "refs/heads/master",
         "sha": "2169f90c",
         "run_number": "20",
     },
 }
 
 
-def T(txt):
+def T(txt):  # noqa: N802
     from textwrap import dedent
 
     txt = dedent(txt)
     if txt.startswith("\n"):
         txt = txt[1:]
     return txt
 
 
-def T1(txt):
+def T1(txt):  # noqa: N802
     return T(txt).rstrip("\n")
 
 
 def test_abort_exception():
     "test the AbortExecution exception"
-    a = tools.AbortExecution(
+    a = tools.AbortExecutionError(
         "a one-line error message",
         """
         A multi line
           explaination of
            what happened
          with some detail
     """,
@@ -66,28 +66,28 @@
         == """
 Another multiline hint how
   to fix the issue
 """
     )
 
     assert (
-        f"\n{str(a)}\n"
+        f"\n{a!s}\n"
         == """
 a one-line error message
   A multi line
     explaination of
      what happened
    with some detail
 hint:
   Another multiline hint how
     to fix the issue
 """
     )
 
-    a = tools.AbortExecution("hello world")
+    a = tools.AbortExecutionError("hello world")
     assert a.message == "hello world"
     assert a.explain == ""
     assert a.hint == ""
     assert str(a) == "hello world"
 
 
 def test_urmtree(tmp_path):
@@ -139,16 +139,16 @@
 B = 3+5
 C = "hello"
 # end of test
 """
     )
     assert 12 == tools.get_module_var(path, "A")
     assert "hello" == tools.get_module_var(path, "C")
-    pytest.raises(AssertionError, tools.get_module_var, path, "B")
-    pytest.raises(tools.MissingVariable, tools.get_module_var, path, "X1")
+    pytest.raises(tools.ValidationError, tools.get_module_var, path, "B")
+    pytest.raises(tools.MissingVariableError, tools.get_module_var, path, "X1")
 
 
 def test_set_module_var(tmp_path):
     "handles set_module_var cases"
     path = tmp_path / "in2.txt"
 
     path.write_text(
@@ -270,21 +270,21 @@
     assert tools.get_module_var(repo.initfile, "__hash__") == "2169f90c22e"
     repo.revert(repo.initfile)
 
     # wrong branch
     repo.branch("beta/0.0.2", "master")
     assert repo.branch() == "beta/0.0.2"
     pytest.raises(
-        tools.InvalidGithubReference, tools.update_version, repo.initfile, abort=False
+        tools.InvalidVersionError, tools.update_version, repo.initfile, abort=False
     )
 
     github_dump = GITHUB["beta"].copy()
     github_dump["ref"] = "refs/heads/beta/0.0.2"
     pytest.raises(
-        tools.InvalidGithubReference,
+        tools.InvalidVersionError,
         tools.update_version,
         repo.initfile,
         github_dump,
         abort=False,
     )
```

