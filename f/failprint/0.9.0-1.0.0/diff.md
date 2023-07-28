# Comparing `tmp/failprint-0.9.0.tar.gz` & `tmp/failprint-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "failprint-0.9.0.tar", last modified: Fri Feb 10 13:35:51 2023, max compression
+gzip compressed data, was "failprint-1.0.0.tar", last modified: Fri Jul 28 18:51:31 2023, max compression
```

## Comparing `failprint-0.9.0.tar` & `failprint-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      754 2023-02-10 13:22:27.696958 failprint-0.9.0/LICENSE
--rw-r--r--   0        0        0     4818 2023-02-10 13:22:27.850288 failprint-0.9.0/README.md
--rw-r--r--   0        0        0     3230 2023-02-10 13:22:27.850288 failprint-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      269 2023-02-10 13:22:27.850288 failprint-0.9.0/src/failprint/__init__.py
--rw-r--r--   0        0        0      344 2023-02-10 13:22:27.540294 failprint-0.9.0/src/failprint/__main__.py
--rw-r--r--   0        0        0     2926 2023-02-10 13:10:24.550141 failprint-0.9.0/src/failprint/capture.py
--rw-r--r--   0        0        0     6197 2023-02-10 13:29:32.616214 failprint-0.9.0/src/failprint/cli.py
--rw-r--r--   0        0        0     4880 2023-02-10 13:10:24.560140 failprint-0.9.0/src/failprint/formats.py
--rw-r--r--   0        0        0     2875 2023-02-10 13:10:24.563474 failprint-0.9.0/src/failprint/process.py
--rw-r--r--   0        0        0        0 2023-02-10 13:22:27.533627 failprint-0.9.0/src/failprint/py.typed
--rw-r--r--   0        0        0     7449 2023-02-10 13:10:24.563474 failprint-0.9.0/src/failprint/runners.py
--rw-r--r--   0        0        0      338 2023-02-10 13:10:24.566807 failprint-0.9.0/src/failprint/types.py
--rw-r--r--   0        0        0      162 2023-02-10 13:22:27.533627 failprint-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-02-10 13:22:27.530294 failprint-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0      817 2020-10-11 17:22:45.809295 failprint-0.9.0/tests/test_capture.py
--rw-r--r--   0        0        0      891 2023-02-10 13:22:27.850288 failprint-0.9.0/tests/test_cli.py
--rw-r--r--   0        0        0     3358 2020-10-10 23:14:46.307266 failprint-0.9.0/tests/test_formats.py
--rw-r--r--   0        0        0     2159 2021-07-31 10:36:47.600135 failprint-0.9.0/tests/test_process.py
--rw-r--r--   0        0        0     9094 2021-07-31 10:36:47.600135 failprint-0.9.0/tests/test_runners.py
--rw-r--r--   0        0        0     6290 1970-01-01 00:00:00.000000 failprint-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-07-23 09:32:34.916242 failprint-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4818 2023-07-23 09:32:37.209566 failprint-1.0.0/README.md
+-rw-r--r--   0        0        0     2740 2023-07-28 18:51:31.162042 failprint-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      525 2023-07-27 15:16:34.103795 failprint-1.0.0/src/failprint/__init__.py
+-rw-r--r--   0        0        0      343 2023-07-23 09:32:34.719576 failprint-1.0.0/src/failprint/__main__.py
+-rw-r--r--   0        0        0     6008 2023-07-27 15:02:19.138784 failprint-1.0.0/src/failprint/capture.py
+-rw-r--r--   0        0        0     6157 2023-07-27 15:02:56.211686 failprint-1.0.0/src/failprint/cli.py
+-rw-r--r--   0        0        0     5777 2023-07-27 15:04:10.100820 failprint-1.0.0/src/failprint/formats.py
+-rw-r--r--   0        0        0     3061 2023-07-27 15:07:47.014907 failprint-1.0.0/src/failprint/lazy.py
+-rw-r--r--   0        0        0     2942 2023-07-27 15:16:34.100461 failprint-1.0.0/src/failprint/process.py
+-rw-r--r--   0        0        0        0 2023-07-23 09:32:34.722909 failprint-1.0.0/src/failprint/py.typed
+-rw-r--r--   0        0        0     7301 2023-07-28 18:50:05.019854 failprint-1.0.0/src/failprint/runners.py
+-rw-r--r--   0        0        0      360 2023-07-27 15:09:15.600507 failprint-1.0.0/src/failprint/types.py
+-rw-r--r--   0        0        0      162 2023-07-23 09:32:34.692909 failprint-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-23 09:32:34.692909 failprint-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      873 2023-07-25 17:05:37.815840 failprint-1.0.0/tests/test_capture.py
+-rw-r--r--   0        0        0     1000 2023-07-23 09:37:38.267685 failprint-1.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0     4242 2023-04-10 14:08:12.815777 failprint-1.0.0/tests/test_formats.py
+-rw-r--r--   0        0        0      978 2023-04-10 14:08:12.815777 failprint-1.0.0/tests/test_lazy.py
+-rw-r--r--   0        0        0     2213 2023-07-27 15:16:34.103795 failprint-1.0.0/tests/test_process.py
+-rw-r--r--   0        0        0    10476 2023-07-27 15:16:34.103795 failprint-1.0.0/tests/test_runners.py
+-rw-r--r--   0        0        0     6412 1970-01-01 00:00:00.000000 failprint-1.0.0/PKG-INFO
```

### Comparing `failprint-0.9.0/LICENSE` & `failprint-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `failprint-0.9.0/README.md` & `failprint-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 With `pip`:
 ```bash
 pip install failprint
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install failprint
 ```
 
 ## Usage
 
 ```console
 % poetry run failprint -h
```

#### html2text {}

```diff
@@ -19,15 +19,15 @@
 above.  To install Python 3.6, I recommend using pyenv. ```bash # install pyenv
 git clone https://github.com/pyenv/pyenv ~/.pyenv # setup pyenv (you should
 also put these three lines in .bashrc or similar) export PATH="${HOME}/.pyenv/
 bin:${PATH}" export PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" #
 install Python 3.6 pyenv install 3.6.12 # make it available globally pyenv
 global system 3.6.12 ```  ## Installation With `pip`: ```bash pip install
 failprint ``` With [`pipx`](https://github.com/pipxproject/pipx): ```bash
-python3.7 -m pip install --user pipx pipx install failprint ``` ## Usage
+python3.8 -m pip install --user pipx pipx install failprint ``` ## Usage
 ```console % poetry run failprint -h usage: failprint [-h] [-c
 {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p | -P] [-q | -Q] [-
 s | -S] [-z | -Z] [-n NUMBER] [-t TITLE] COMMAND [COMMAND ...] positional
 arguments: COMMAND optional arguments: -h, --help show this help message and
 exit -c {stdout,stderr,both,none}, --capture {stdout,stderr,both,none} Which
 output to capture. Colors are supported with 'both' only, unless the command
 has a 'force color' option. -f {pretty,tap}, --format {pretty,tap} Output
```

### Comparing `failprint-0.9.0/pyproject.toml` & `failprint-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,136 +1,121 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "failprint"
 description = "Run a command, print its output only if it fails."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
-license = "ISC"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = [
     "cli",
     "failure",
     "output",
     "runner",
 ]
 dynamic = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Documentation",
     "Topic :: Software Development",
-    "Topic :: Software Development :: Documentation",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "ansimarkup~=1.4",
     "jinja2>=2.11, <4",
     "ptyprocess~=0.6; sys_platform != 'win32'",
+    "typing-extensions>=4.1; python_version < '3.10'",
 ]
-version = "0.9.0"
+version = "1.0.0"
+
+[project.license]
+text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/failprint"
 Documentation = "https://pawamoy.github.io/failprint"
 Changelog = "https://pawamoy.github.io/failprint/changelog"
 Repository = "https://github.com/pawamoy/failprint"
 Issues = "https://github.com/pawamoy/failprint/issues"
 Discussions = "https://github.com/pawamoy/failprint/discussions"
 Gitter = "https://gitter.im/failprint/community"
 Funding = "https://github.com/sponsors/pawamoy"
 
 [project.scripts]
 failprint = "failprint.cli:main"
 
+[tool.pdm]
+plugins = [
+    "pdm-multirun",
+]
+
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 duty = [
-    "duty>=0.7",
+    "duty>=0.10",
+]
+ci-quality = [
+    "failprint[duty,docs,quality,typing,security]",
+]
+ci-tests = [
+    "failprint[duty,tests]",
 ]
 docs = [
+    "black>=23.1",
+    "markdown-callouts>=0.2",
+    "markdown-exec>=0.5",
     "mkdocs>=1.3",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
+    "mkdocs-git-committers-plugin-2>=1.1",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
-    "mkdocs-section-index>=0.3",
+    "mkdocs-minify-plugin>=0.6.4",
     "mkdocstrings[python]>=0.18",
-    "markdown-callouts>=0.2",
-    "markdown-exec>=0.5",
     "toml>=0.10",
 ]
-format = [
-    "autoflake>=1.4",
-    "black>=23.1",
-    "isort>=5.10",
-]
 maintain = [
+    "black>=23.1",
+    "blacken-docs>=1.13",
     "git-changelog>=1.0",
 ]
 quality = [
-    "importlib-metadata<5; python_version < '3.8'",
-    "flake8>=4; python_version >= '3.8'",
-    "darglint>=1.8",
-    "flake8-bandit>=2.1",
-    "flake8-black>=0.2",
-    "flake8-bugbear>=21.9",
-    "flake8-builtins>=1.5",
-    "flake8-comprehensions>=3.7",
-    "flake8-docstrings>=1.6",
-    "flake8-pytest-style>=1.5",
-    "flake8-string-format>=0.3",
-    "flake8-tidy-imports>=4.5",
-    "flake8-variables-names>=0.0",
-    "pep8-naming>=0.12",
-    "wps-light>=0.15",
+    "ruff>=0.0.246",
 ]
 tests = [
     "pytest>=6.2",
     "pytest-cov>=3.0",
     "pytest-randomly>=3.10",
     "pytest-xdist>=2.4",
     "hypothesis>=6.13",
 ]
 typing = [
     "mypy>=0.910",
     "types-markdown>=3.3",
+    "types-pyyaml>=6.0",
     "types-toml>=0.10",
 ]
 security = [
     "safety>=2",
 ]
-
-[tool.black]
-line-length = 120
-exclude = "tests/fixtures"
-
-[tool.isort]
-line_length = 120
-not_skip = "__init__.py"
-multi_line_output = 3
-force_single_line = false
-balanced_wrapping = true
-default_section = "THIRDPARTY"
-known_first_party = "failprint"
-include_trailing_comma = true
```

### Comparing `failprint-0.9.0/src/failprint/cli.py` & `failprint-1.0.0/src/failprint/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+"""Module that contains the command line application."""
+
 # Why does this file exist, and why not put this in `__main__`?
 #
 # You might be tempted to import things from `__main__` later,
 # but that will cause problems: the code will get executed twice:
 #
 # - When you run `python -m failprint` python will execute
 #   `__main__.py` as a script. That means there won't be any
 #   `failprint.__main__` in `sys.modules`.
 # - When you import `__main__` it will get executed again (as a module) because
 #   there's no `failprint.__main__` in `sys.modules`.
 
-"""Module that contains the command line application."""
-
 from __future__ import annotations
 
 import argparse
 from typing import Any, Sequence
 
 from failprint.capture import Capture
 from failprint.formats import accept_custom_format, formats
@@ -28,35 +28,33 @@
         self,
         truthy: Sequence[str],
         falsy: Sequence[str],
         truthy_help: str = "",
         falsy_help: str = "",
         **kwargs: Any,
     ) -> None:
-        """
-        Add a boolean flag/argument to the parser.
+        """Add a boolean flag/argument to the parser.
 
         Arguments:
             truthy: Values that will store true in the destination.
             falsy: Values that will store false in the destination.
             truthy_help: Help for the truthy arguments.
             falsy_help: Help for the falsy arguments.
             **kwargs: Remaining keyword arguments passed to `argparse.ArgumentParser.add_argument`.
         """
         truthy_kwargs = {**kwargs, "help": truthy_help, "action": "store_true"}
         falsy_kwargs = {**kwargs, "help": falsy_help, "action": "store_false"}
 
         mxg = self.add_mutually_exclusive_group()
-        mxg.add_argument(*truthy, **truthy_kwargs)  # type: ignore  # mypy is confused by arguments position
-        mxg.add_argument(*falsy, **falsy_kwargs)  # type: ignore
+        mxg.add_argument(*truthy, **truthy_kwargs)
+        mxg.add_argument(*falsy, **falsy_kwargs)
 
 
-def add_flags(parser: ArgParser, set_defaults: bool = True) -> ArgParser:
-    """
-    Add some boolean flags to the parser.
+def add_flags(parser: ArgParser, *, set_defaults: bool = True) -> ArgParser:
+    """Add some boolean flags to the parser.
 
     We made this method separate and public
     for its use in [duty](https://github.com/pawamoy/duty).
 
     Arguments:
         parser: The parser to add flags to.
         set_defaults: Whether to set default values on arguments.
@@ -159,9 +157,12 @@
     Parameters:
         args: Arguments passed from the command line.
 
     Returns:
         An exit code.
     """
     parser = get_parser()
-    opts = parser.parse_args(args).__dict__.items()  # noqa: WPS609
+    opts = parser.parse_args(args).__dict__.items()
     return run(**{_: value for _, value in opts if value is not None}).code
+
+
+__all__ = ["ArgParser", "add_flags", "get_parser", "main"]
```

### Comparing `failprint-0.9.0/src/failprint/formats.py` & `failprint-1.0.0/src/failprint/formats.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """Output-printing formats."""
 
 from __future__ import annotations
 
 import inspect
-from typing import Callable, Sequence
+from typing import TYPE_CHECKING, Callable, Sequence
 
-from failprint.types import CmdFuncType
+from failprint.lazy import LazyCallable
+
+if TYPE_CHECKING:
+    from types import FrameType
+
+    from failprint.types import CmdFuncType
 
 DEFAULT_FORMAT = "pretty"
+DEFAULT_CALLABLE_NAME = "callable"
 
 
 class Format:
     """Class to define a display format."""
 
-    def __init__(self, template: str, progress_template: str | None = None, accept_ansi: bool = True) -> None:
-        """
-        Initialize the object.
+    def __init__(self, template: str, *, progress_template: str | None = None, accept_ansi: bool = True) -> None:
+        """Initialize the object.
 
         Arguments:
             template: The main template.
             progress_template: The template to show progress.
             accept_ansi: Whether to accept ANSI sequences.
         """
         self.template = template
@@ -46,32 +51,30 @@
         "output: |\n{{ output|indent(4 * ' ') }}\n  ...{% endif %}",
         accept_ansi=False,
     ),
 }
 
 
 def accept_custom_format(string: str) -> str:
-    """
-    Store the value in `formats` if it starts with custom.
+    """Store the value in `formats` if it starts with custom.
 
     Arguments:
         string: A format name.
 
     Returns:
         The format name, or `custom` if it started with `custom=`.
     """
     if string.startswith("custom="):
         formats["custom"] = Format(string[7:])
         return "custom"
     return string
 
 
 def printable_command(cmd: CmdFuncType, args: Sequence | None = None, kwargs: dict | None = None) -> str:
-    """
-    Transform a command or function into a string.
+    """Transform a command or function into a string.
 
     Arguments:
         cmd: The command or function to transform.
         args: Positional arguments passed to the function.
         kwargs: Keyword arguments passed to the function.
 
     Returns:
@@ -80,17 +83,16 @@
     if isinstance(cmd, str):
         return cmd
     if callable(cmd):
         return as_python_statement(cmd, args, kwargs)
     return as_shell_command(cmd)
 
 
-def as_shell_command(cmd: list[str]) -> str:  # noqa: WPS231 (not that complex)
-    """
-    Rebuild a command line from system arguments.
+def as_shell_command(cmd: list[str]) -> str:
+    """Rebuild a command line from system arguments.
 
     Arguments:
         cmd: The command as a list of strings.
 
     Returns:
         A printable and shell-runnable command.
     """
@@ -101,47 +103,76 @@
             continue
         has_spaces = " " in part
         has_double_quotes = '"' in part
         has_single_quotes = "'" in part
         if has_double_quotes and not has_single_quotes:
             # double quotes, no single quotes
             # -> wrap in single quotes
-            part = f"'{part}'"
+            part = f"'{part}'"  # noqa: PLW2901
         elif has_single_quotes and has_double_quotes:
             # double and single quotes
             # -> escape double quotes, wrap in double quotes
-            part = part.replace('"', r"\"")
-            part = f'"{part}"'
+            part = part.replace('"', r"\"")  # noqa: PLW2901
+            part = f'"{part}"'  # noqa: PLW2901
         elif has_single_quotes or has_spaces:
             # spaces or single quotes
             # -> wrap in double quotes
-            part = f'"{part}"'
+            part = f'"{part}"'  # noqa: PLW2901
         parts.append(part)
     return " ".join(parts)
 
 
-def as_python_statement(func: Callable, args: Sequence | None = None, kwargs: dict | None = None) -> str:
-    """
-    Transform a callable and its arguments into a Python statement string.
+def as_python_statement(func: Callable | LazyCallable, args: Sequence | None = None, kwargs: dict | None = None) -> str:
+    """Transform a callable and its arguments into a Python statement string.
 
     Arguments:
         func: The callable to transform.
         args: Positional arguments passed to the function.
         kwargs: Keyword arguments passed to the function.
 
     Returns:
         A Python statement.
     """
-    func_name = getattr(func, "__name__", None)
-    try:  # noqa: WPS229
-        # climb back up to the frame above the call to run(),
-        # to get the name passed from the external caller (user)
-        ctx_run_call = inspect.currentframe().f_back.f_back.f_back.f_back  # type: ignore[union-attr]
-        call_vars = ctx_run_call.f_locals.items()  # type: ignore[union-attr]
-        func_name = next(var_name for var_name, var_val in call_vars if var_val is func)
-    except (AttributeError, StopIteration):
-        func_name = getattr(func, "__name__", "callable")
-
+    if isinstance(func, LazyCallable):
+        callable_name = func.name or _get_callable_name(func.call)
+        args = args or func.args
+        kwargs = kwargs or func.kwargs
+    else:
+        callable_name = _get_callable_name(func)
     args_str = [repr(arg) for arg in args] if args else []
-    kwargs_str = [f"{k}={v!r}" for k, v in kwargs.items()] if kwargs else []  # noqa: WPS111,WPS221
+    kwargs_str = [f"{k}={v!r}" for k, v in kwargs.items()] if kwargs else []
     arguments = ", ".join(args_str + kwargs_str)
-    return f"{func_name}({arguments})"
+    return f"{callable_name}({arguments})"
+
+
+def _get_callable_name(callee: Callable) -> str:
+    callable_name = getattr(callee, "__name__", None)
+    if callable_name:
+        return callable_name
+
+    # Climb back up the frames to search the callable in the locals
+    callable_name = None
+    caller_frame: FrameType = inspect.currentframe()  # type: ignore[assignment]
+    while callable_name is None and caller_frame.f_back:
+        caller_frame = caller_frame.f_back
+        callable_name = _find_callable_name_in_frame_locals(caller_frame, callee)
+
+    return callable_name or DEFAULT_CALLABLE_NAME
+
+
+def _find_callable_name_in_frame_locals(caller_frame: FrameType, callee: Callable) -> str | None:
+    call_vars = caller_frame.f_locals.items()
+    try:
+        # ignore @py_assert variables from pytest
+        return next(var_name for var_name, var_val in call_vars if var_val is callee and not var_name.startswith("@"))
+    except StopIteration:
+        return None
+
+
+__all__ = [
+    "accept_custom_format",
+    "as_python_statement",
+    "as_shell_command",
+    "Format",
+    "formats",
+    "printable_command",
+]
```

### Comparing `failprint-0.9.0/src/failprint/process.py` & `failprint-1.0.0/src/failprint/process.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 """Functions related to subprocesses."""
 
 from __future__ import annotations
 
 import contextlib
-import subprocess  # noqa: S404 (we don't mind the security implication)
+import os
+import subprocess
+import sys
+from typing import TYPE_CHECKING
 
-from failprint import WINDOWS
 from failprint.capture import Capture
 from failprint.formats import printable_command
-from failprint.types import CmdType
+
+if TYPE_CHECKING:
+    from failprint.types import CmdType
+
+
+WINDOWS = sys.platform.startswith("win") or os.name == "nt"
 
 if not WINDOWS:
     from ptyprocess import PtyProcessUnicode
 
 
 def run_subprocess(
     cmd: CmdType,
+    *,
     capture: Capture = Capture.BOTH,
     shell: bool = False,
     stdin: str | None = None,
 ) -> tuple[int, str]:
-    """
-    Run a command in a subprocess.
+    """Run a command in a subprocess.
 
     Arguments:
         cmd: The command to run.
         capture: The output to capture.
         shell: Whether to run the command in a shell.
         stdin: String to use as standard input.
 
@@ -33,30 +40,26 @@
         The exit code and the command raw output.
     """
     if capture == Capture.NONE:
         stdout_opt = None
         stderr_opt = None
     else:
         stdout_opt = subprocess.PIPE
-
-        if capture == Capture.BOTH:
-            stderr_opt = subprocess.STDOUT
-        else:
-            stderr_opt = subprocess.PIPE
+        stderr_opt = subprocess.STDOUT if capture == Capture.BOTH else subprocess.PIPE
 
     if shell and not isinstance(cmd, str):
         cmd = printable_command(cmd)
 
-    process = subprocess.run(  # noqa: S603,W1510 (we trust the input, and don't want to "check")
+    process = subprocess.run(
         cmd,
         input=stdin,
         stdout=stdout_opt,
         stderr=stderr_opt,
-        shell=shell,  # noqa: S602 (shell=True)
-        universal_newlines=True,
+        shell=shell,  # noqa: S603
+        text=True,
         encoding="utf8",
     )
 
     if capture == Capture.NONE:
         output = ""
     elif capture == Capture.STDERR:
         output = process.stderr
@@ -64,46 +67,51 @@
         output = process.stdout
 
     return process.returncode, output
 
 
 def run_pty_subprocess(
     cmd: list[str],
+    *,
     capture: Capture = Capture.BOTH,
     stdin: str | None = None,
-) -> tuple[int, str] | None:
-    """
-    Run a command in a PTY subprocess.
+) -> tuple[int, str]:
+    """Run a command in a PTY subprocess.
 
     Arguments:
         cmd: The command to run.
         capture: The output to capture.
         stdin: String to use as standard input.
 
     Returns:
         The exit code and the command output.
     """
     process = PtyProcessUnicode.spawn(cmd)
+    process.delayafterclose = 0.01  # default to 0.1
+    process.delayafterterminate = 0.01  # default to 0.1
     pty_output: list[str] = []
 
     if stdin is not None:
-        process.setecho(False)
+        process.setecho(state=False)
         process.waitnoecho()
         process.write(stdin)
         process.sendeof()
         # not sure why but sending only one eof is not always enough,
         # so we send a second one and ignore any IO error
         with contextlib.suppress(OSError):
             process.sendeof()
 
     while True:
         try:
             output_data = process.read()
         except EOFError:
             break
         if capture == Capture.NONE:
-            print(output_data, end="", flush=True)  # noqa: WPS421 (print)
+            print(output_data, end="", flush=True)  # noqa: T201
         else:
             pty_output.append(output_data)
 
     output = "".join(pty_output).replace("\r\n", "\n")
     return process.wait(), output
+
+
+__all__ = ["run_subprocess", "run_pty_subprocess"]
```

### Comparing `failprint-0.9.0/src/failprint/runners.py` & `failprint-1.0.0/src/failprint/runners.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,63 +3,64 @@
 from __future__ import annotations
 
 import os
 import shutil
 import sys
 import textwrap
 import traceback
-from typing import Callable, Sequence, TextIO
+from typing import TYPE_CHECKING, Callable, Sequence
 
 import colorama
 from ansimarkup import ansiprint
 from jinja2 import Environment
 
-from failprint import WINDOWS
-from failprint.capture import Capture, cast_capture, stdbuffer
+from failprint.capture import Capture
 from failprint.formats import DEFAULT_FORMAT, accept_custom_format, formats, printable_command
-from failprint.process import run_pty_subprocess, run_subprocess
-from failprint.types import CmdFuncType, CmdType
+from failprint.lazy import LazyCallable
+from failprint.process import WINDOWS, run_pty_subprocess, run_subprocess
+
+if TYPE_CHECKING:
+    from failprint.types import CmdFuncType, CmdType
 
 if WINDOWS:
     colorama.init()
 
 
 class RunResult:
     """Placeholder for a run result."""
 
     def __init__(self, code: int, output: str) -> None:
-        """
-        Initialize the object.
+        """Initialize the object.
 
         Arguments:
             code: The exit code of the command.
             output: The output of the command.
         """
         self.code = code
         self.output = output
 
 
-def run(  # noqa: WPS231 (high complexity)
+def run(
     cmd: CmdFuncType,
+    *,
     args: Sequence | None = None,
     kwargs: dict | None = None,
     number: int = 1,
     capture: str | bool | Capture | None = None,
     title: str | None = None,
     fmt: str | None = None,
     pty: bool = False,
     progress: bool = True,
     nofail: bool = False,
     quiet: bool = False,
     silent: bool = False,
     stdin: str | None = None,
     command: str | None = None,
 ) -> RunResult:
-    """
-    Run a command in a subprocess or a Python function, and print its output if it fails.
+    """Run a command in a subprocess or a Python function, and print its output if it fails.
 
     Arguments:
         cmd: The command to run.
         args: Arguments to pass to the callable.
         kwargs: Keyword arguments to pass to the callable.
         number: The command number.
         capture: The output to capture.
@@ -72,33 +73,33 @@
         silent: Don't print anything.
         stdin: String to use as standard input.
         command: The command to display.
 
     Returns:
         The command exit code, or 0 if `nofail` is True.
     """
-    format_name: str = fmt or os.environ.get("FAILPRINT_FORMAT", DEFAULT_FORMAT)  # type: ignore
+    format_name: str = fmt or os.environ.get("FAILPRINT_FORMAT", DEFAULT_FORMAT)  # type: ignore[assignment]
     format_name = accept_custom_format(format_name)
     format_obj = formats.get(format_name, formats[DEFAULT_FORMAT])
 
     env = Environment(autoescape=False)  # noqa: S701 (no HTML: no need to escape)
     env.filters["indent"] = textwrap.indent
 
     command = command if command is not None else printable_command(cmd, args, kwargs)
 
     if not silent and progress and format_obj.progress_template:
         progress_template = env.from_string(format_obj.progress_template)
         ansiprint(progress_template.render({"title": title, "command": command}), end="\r")
 
-    capture = cast_capture(capture)
+    capture = Capture.cast(capture)
 
     if callable(cmd):
-        code, output = run_function(cmd, args, kwargs, capture, stdin)
+        code, output = run_function(cmd, args=args, kwargs=kwargs, capture=capture, stdin=stdin)
     else:
-        code, output = run_command(cmd, capture, format_obj.accept_ansi, pty, stdin)
+        code, output = run_command(cmd, capture=capture, ansi=format_obj.accept_ansi, pty=pty, stdin=stdin)
 
     if not silent:
         template = env.from_string(format_obj.template)
         ansiprint(
             template.render(
                 {
                     "title": title,
@@ -116,21 +117,21 @@
         )
 
     return RunResult(0 if nofail else code, output)
 
 
 def run_command(
     cmd: CmdType,
+    *,
     capture: Capture = Capture.BOTH,
     ansi: bool = False,
     pty: bool = False,
     stdin: str | None = None,
 ) -> tuple[int, str]:
-    """
-    Run a command.
+    """Run a command.
 
     Arguments:
         cmd: The command to run.
         capture: The output to capture.
         ansi: Whether to accept ANSI sequences.
         pty: Whether to run in a PTY.
         stdin: String to use as standard input.
@@ -143,36 +144,36 @@
     # if chosen format doesn't accept ansi, or on Windows, don't use pty
     if pty and (not ansi or WINDOWS):
         pty = False
 
     # pty can only combine, so only use pty when combining
     if pty and capture in {Capture.BOTH, Capture.NONE}:
         if shell:
-            cmd = ["sh", "-c", cmd]  # type: ignore  # we know cmd is str
-        return run_pty_subprocess(cmd, capture, stdin)  # type: ignore  # we made sure cmd is a list
+            cmd = ["sh", "-c", cmd]  # type: ignore[list-item]  # we know cmd is str
+        return run_pty_subprocess(cmd, capture=capture, stdin=stdin)  # type: ignore[arg-type]  # we made sure cmd is a list
 
     # we are on Windows
     if WINDOWS:
         # make sure the process can find the executable
         if not shell:
-            cmd[0] = shutil.which(cmd[0]) or cmd[0]  # type: ignore  # we know cmd is a list
-        return run_subprocess(cmd, capture, shell=shell, stdin=stdin)  # noqa: S604 (shell=True)
+            cmd[0] = shutil.which(cmd[0]) or cmd[0]  # type: ignore[index]  # we know cmd is a list
+        return run_subprocess(cmd, capture=capture, shell=shell, stdin=stdin)
 
-    return run_subprocess(cmd, capture, shell=shell, stdin=stdin)  # noqa: S604 (shell=True)
+    return run_subprocess(cmd, capture=capture, shell=shell, stdin=stdin)
 
 
 def run_function(
     func: Callable,
+    *,
     args: Sequence | None = None,
     kwargs: dict | None = None,
     capture: Capture = Capture.BOTH,
     stdin: str | None = None,
 ) -> tuple[int, str]:
-    """
-    Run a function.
+    """Run a function.
 
     Arguments:
         func: The function to run.
         args: Positional arguments passed to the function.
         kwargs: Keyword arguments passed to the function.
         capture: The output to capture.
         stdin: String to use as standard input.
@@ -180,69 +181,69 @@
     Returns:
         The exit code and the function output.
     """
     args = args or []
     kwargs = kwargs or {}
 
     if capture == Capture.NONE:
-        return run_function_get_code(func, sys.stderr, args, kwargs), ""
-
-    with stdbuffer(stdin) as buffer:
-        if capture == Capture.BOTH:
-            # combining stdout and stderr
-            # -> redirect stderr to stdout
-            buffer.stderr = buffer.stdout
-            sys.stderr = buffer.stdout
+        return run_function_get_code(func, args=args, kwargs=kwargs), ""
 
-        code = run_function_get_code(func, buffer.stderr, args, kwargs)
+    with capture.here(stdin=stdin) as captured:
+        code = run_function_get_code(func, args=args, kwargs=kwargs)
 
-        if capture == Capture.STDERR:
-            output = buffer.stderr.getvalue()
-        else:
-            output = buffer.stdout.getvalue()
+    return code, str(captured)
 
-    return code, output
 
-
-def run_function_get_code(  # noqa: WPS212,WPS231
+def run_function_get_code(
     func: Callable,
-    stderr: TextIO,
+    *,
     args: Sequence,
     kwargs: dict,
 ) -> int:
-    """
-    Run a function and return a exit code.
+    """Run a function and return a exit code.
 
     Arguments:
         func: The function to run.
-        stderr: A file descriptor to write potential tracebacks.
         args: Positional arguments passed to the function.
         kwargs: Keyword arguments passed to the function.
 
     Returns:
         An exit code.
     """
     try:
         result = func(*args, **kwargs)
     except SystemExit as exit:
         if exit.code is None:
             return 0
         if isinstance(exit.code, int):
             return exit.code
-        stderr.write(str(exit.code))
+        sys.stderr.write(str(exit.code))
         return 1
-    except Exception:  # noqa: W0703 (catching Exception on purpose)
-        stderr.write(traceback.format_exc() + "\n")
+    except Exception:  # noqa: BLE001
+        sys.stderr.write(traceback.format_exc() + "\n")
         return 1
 
+    # if func was a lazy callable, recurse
+    if isinstance(result, LazyCallable):
+        return run_function_get_code(result, args=(), kwargs={})
+
     # first check True and False
     # because int(True) == 1 and int(False) == 0
     if result is True:
         return 0
     if result is False:
         return 1
     try:
         return int(result)
     except (ValueError, TypeError):
         if result is None or bool(result):
             return 0
         return 1
+
+
+__all__ = [
+    "run",
+    "run_command",
+    "run_function",
+    "run_function_get_code",
+    "RunResult",
+]
```

### Comparing `failprint-0.9.0/tests/test_capture.py` & `failprint-1.0.0/tests/test_capture.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Tests for the `capture` module."""
 
+from __future__ import annotations
+
 import pytest
 
-from failprint.capture import Capture, cast_capture
+from failprint.capture import Capture
 
 
 @pytest.mark.parametrize(
     ("value", "expected"),
     [
         ("stdout", Capture.STDOUT),
         ("stderr", Capture.STDERR),
@@ -17,16 +19,15 @@
         (Capture.STDOUT, Capture.STDOUT),
         (Capture.STDERR, Capture.STDERR),
         (Capture.BOTH, Capture.BOTH),
         (Capture.NONE, Capture.NONE),
         (None, Capture.BOTH),  # default
     ],
 )
-def test_cast_string(value, expected):
-    """
-    Cast various values in a Capture enumeration value.
+def test_cast_string(value: str | bool | Capture, expected: Capture) -> None:
+    """Cast various values in a Capture enumeration value.
 
     Arguments:
         value: The value to cast.
         expected: The value to expect.
     """
-    assert cast_capture(value) == expected
+    assert Capture.cast(value) == expected
```

### Comparing `failprint-0.9.0/tests/test_cli.py` & `failprint-1.0.0/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Tests for the `cli` module."""
 
+from __future__ import annotations
+
 import pytest
 
 from failprint import cli
 
 
-def test_fail_without_arguments():
+def test_fail_without_arguments() -> None:
     """Fails without arguments."""
     with pytest.raises(SystemExit):
         cli.main([])
 
 
-def test_show_help(capsys):
+def test_show_help(capsys: pytest.CaptureFixture) -> None:
     """Show help.
 
     Parameters:
         capsys: Pytest fixture to capture output.
     """
     with pytest.raises(SystemExit):
         cli.main(["-h"])
     captured = capsys.readouterr()
     assert "failprint" in captured.out
 
 
-def test_run_command():
+def test_run_command() -> None:
     """Run a simple command."""
     assert cli.main(["echo", "hello"]) == 0
 
 
-def test_accept_custom_format(capsys):
-    """
-    Run a command with a custom output format.
+def test_accept_custom_format(capsys: pytest.CaptureFixture) -> None:
+    """Run a command with a custom output format.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     assert cli.main(["--no-progress", "-f", "custom={{output}}", "echo", "custom"]) == 0
     outerr = capsys.readouterr()
     assert "custom" in outerr.out
```

### Comparing `failprint-0.9.0/tests/test_formats.py` & `failprint-1.0.0/tests/test_formats.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Tests for the `formats` module."""
 
+from __future__ import annotations
+
+from typing import Callable, Sequence
+
 import pytest
 from hypothesis import given
 from hypothesis.strategies import text
 
-from failprint.formats import printable_command
+from failprint.formats import DEFAULT_CALLABLE_NAME, _get_callable_name, printable_command
 from failprint.runners import run
 
 
 @pytest.mark.parametrize(
     ("cmd", "expected"),
     [
         # empty arg
@@ -18,87 +22,116 @@
         # spaces
         (["a", "command", "with", " "], 'a command with " "'),
         # single quotes
         (["a", "command", "with", "'"], 'a command with "\'"'),
         # double quotes
         (["a", "command", "with", '"'], "a command with '\"'"),
         # both quotes
-        (["a", "command", "with", "\"'"], 'a command with "\\"\'"'),  # noqa: WPS342 (raw string)
+        (["a", "command", "with", "\"'"], 'a command with "\\"\'"'),
         # both quotes and spaces
-        (["a", "command", "with", "\" '"], 'a command with "\\" \'"'),  # noqa: WPS342 (raw string)
+        (["a", "command", "with", "\" '"], 'a command with "\\" \'"'),
     ],
 )
-def test_printable_command_with_list(cmd, expected) -> None:
-    """
-    Correctly transform a list of arguments into a runnable shell command.
+def test_printable_command_with_list(cmd: list[str], expected: str) -> None:
+    """Correctly transform a list of arguments into a runnable shell command.
 
     Arguments:
         cmd: The command as a list of arguments.
         expected: The expected result after transformation.
     """
     assert printable_command(cmd) == expected
 
 
 @given(text())
-def test_printable_command_with_string(cmd):
-    """
-    Correctly transform a string into a runnable shell command.
+def test_printable_command_with_string(cmd: str) -> None:
+    """Correctly transform a string into a runnable shell command.
 
     Arguments:
         cmd: The command as a string.
     """
     assert printable_command(cmd) == cmd
 
 
-class Repr:  # noqa: D101,C0115 (missing docstring)
-    def __init__(self, value):  # noqa: D107 (missing docstring)
+class Repr:  # noqa: D101 (missing docstring)
+    def __init__(self, value: str | int):  # noqa: D107 (missing docstring)
         self.value = value
 
     def __repr__(self):
         return f"Repr(value={self.value!r})"
 
 
 @pytest.mark.parametrize(
     ("cmd", "args", "kwargs", "expected"),
     [
-        (lambda: 0, None, None, "<lambda>()"),  # noqa: WPS522 (implicit primitive/lambda)
+        (lambda: 0, None, None, "<lambda>()"),
         (lambda _: _, None, None, "<lambda>()"),
-        (lambda: 0, [6], None, "<lambda>(6)"),  # noqa: WPS522
+        (lambda: 0, [6], None, "<lambda>(6)"),
         (lambda _: _, [6], None, "<lambda>(6)"),
-        (lambda: 0, None, {"kwarg": "hello"}, "<lambda>(kwarg='hello')"),  # noqa: WPS522
+        (lambda: 0, None, {"kwarg": "hello"}, "<lambda>(kwarg='hello')"),
         (lambda _: _, None, {"kwarg": 6}, "<lambda>(kwarg=6)"),
-        (lambda: 0, [6, 7], {"kwarg": 3.2}, "<lambda>(6, 7, kwarg=3.2)"),  # noqa: WPS522
+        (lambda: 0, [6, 7], {"kwarg": 3.2}, "<lambda>(6, 7, kwarg=3.2)"),
         (lambda _: _, [True, None, 5.5], {"kwarg": True}, "<lambda>(True, None, 5.5, kwarg=True)"),
         (
             printable_command,
             [Repr(0)],
             {"repr": Repr("marvin")},
             "printable_command(Repr(value=0), repr=Repr(value='marvin'))",
         ),
     ],
 )
-def test_printable_command_with_callable(cmd, args, kwargs, expected):
-    """
-    Correctly transform a callable into a runnable shell command.
+def test_printable_command_with_callable(
+    cmd: Callable,
+    args: Sequence | None,
+    kwargs: dict | None,
+    expected: str,
+) -> None:
+    """Correctly transform a callable into a runnable shell command.
 
     Arguments:
         cmd: The command as a string.
         args: Arguments passed to `printable_command`.
         kwargs: Keyword arguments passed to `printable_command`.
         expected: The expected result after transformation.
     """
     assert printable_command(cmd, args, kwargs) == expected
 
 
-def test_tap_format(capsys):
-    """
-    Check the tap output format.
+def test_tap_format(capsys: pytest.CaptureFixture) -> None:
+    """Check the tap output format.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     run(["true"], fmt="tap")
     outerr = capsys.readouterr()
     assert "ok" in outerr.out
     run(["false"], fmt="tap")
     outerr = capsys.readouterr()
     assert "not ok" in outerr.out
+
+
+def test_getting_callable_name_from_stack() -> None:
+    """Check that we're able to get a callable's name from the stack."""
+
+    def greet() -> None:
+        pass  # pragma: no cover
+
+    assert _get_callable_name(greet) == "greet"
+    greet.__name__ = "changed"
+    assert _get_callable_name(greet) == "changed"
+    greet.__name__ = ""
+    assert _get_callable_name(greet) == "greet"
+    hello = greet
+    del greet
+    assert _get_callable_name(hello) == "hello"
+
+
+def test_failing_to_get_callable_name_from_stack() -> None:
+    """Check case where we're unable to get a callable's name from the stack."""
+
+    class A:
+        def greet(self) -> None:
+            pass  # pragma: no cover
+
+    A.greet.__name__ = ""
+    a = A()
+    assert _get_callable_name(a.greet) == DEFAULT_CALLABLE_NAME
```

### Comparing `failprint-0.9.0/tests/test_process.py` & `failprint-1.0.0/tests/test_process.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 """Tests for the `process` module."""
 
+from __future__ import annotations
 
 import pytest
 from hypothesis import given, settings
 from hypothesis.strategies import characters, text
 
-from failprint import WINDOWS
 from failprint.capture import Capture
-from failprint.process import run_pty_subprocess, run_subprocess
+from failprint.process import WINDOWS, run_pty_subprocess, run_subprocess
 
 
-def test_run_list_of_args_as_shell():
+def test_run_list_of_args_as_shell() -> None:
     """Test that a list of arguments is stringified."""
-    code, output = run_subprocess(["python", "-V"], shell=True)  # noqa: S604 (shell=True)
+    code, output = run_subprocess(["python", "-V"], shell=True)  # noqa: S604
     assert code == 0
     assert "Python" in output
 
 
-def test_run_unknown_shell_command():
+def test_run_unknown_shell_command() -> None:
     """Run an unknown command in a shell."""
-    code, output = run_subprocess("mlemlemlemlemle", shell=True)  # noqa: S604 (shell=True)
+    code, output = run_subprocess("mlemlemlemlemle", shell=True)  # noqa: S604
     assert code > 0
     assert output
 
 
-def test_run_unknown_command():
+def test_run_unknown_command() -> None:
     """Run an unknown command without a shell."""
     # maybe this exception should be caught in the code?
     with pytest.raises(FileNotFoundError):
         run_subprocess("mlemlemlemlemle")
 
 
 @pytest.mark.skipif(WINDOWS, reason="no PTY support on Windows")
-def test_run_pty_subprocess_capture_none(capsys):
-    """
-    Run a PTY subprocess without capturing output.
+def test_run_pty_subprocess_capture_none(capsys: pytest.CaptureFixture) -> None:
+    """Run a PTY subprocess without capturing output.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     code, output = run_pty_subprocess(["bash", "-c", "echo PTY"], capture=Capture.NONE)
     assert code == 0
     assert not output
     outerr = capsys.readouterr()
     assert "PTY" in outerr.out
 
 
 @given(text(alphabet=characters(blacklist_categories="C")))
-def test_pass_stdin_to_subprocess(stdin):
-    """
-    Pass input to a normal subprocess.
+def test_pass_stdin_to_subprocess(stdin: str) -> None:
+    """Pass input to a normal subprocess.
 
     Arguments:
         stdin: Text sample generated by Hypothesis.
     """
     code, output = run_subprocess(["cat"], stdin=stdin)
     assert code == 0
     assert output == stdin
 
 
 @pytest.mark.skipif(WINDOWS, reason="no PTY support on Windows")
 @given(text(alphabet=characters(blacklist_categories="C")))
 @settings(deadline=None)
-def test_pass_stdin_to_pty_subprocess(stdin):
-    """
-    Pass input to a PTY subprocess.
+def test_pass_stdin_to_pty_subprocess(stdin: str) -> None:
+    """Pass input to a PTY subprocess.
 
     Arguments:
         stdin: Text sample generated by Hypothesis.
     """
     code, output = run_pty_subprocess(["cat"], stdin=stdin)
     assert code == 0
     assert output == stdin
```

### Comparing `failprint-0.9.0/tests/test_runners.py` & `failprint-1.0.0/tests/test_runners.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,341 +1,357 @@
 """Tests for the `runners` module."""
 
+import os
+import subprocess
 import sys
 from unittest.mock import MagicMock, patch
 
 import pytest
 from hypothesis import given
 from hypothesis.strategies import characters, integers, text
 
-from failprint import WINDOWS
+from failprint.capture import Capture
+from failprint.lazy import lazy
+from failprint.process import WINDOWS
 from failprint.runners import run, run_function
 
 
-def test_run_silent_command_silently(capsys):
-    """
-    Run a silent command, silently.
+def test_run_silent_command_silently(capsys: pytest.CaptureFixture) -> None:
+    """Run a silent command, silently.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     run(["true"], silent=True)
     outerr = capsys.readouterr()
     assert not outerr.out
-    assert not outerr.err  # noqa: WPS204 (overuse)
+    assert not outerr.err
 
 
-def test_run_verbose_command_silently(capsys):
-    """
-    Run a verbose command, silently.
+def test_run_verbose_command_silently(capsys: pytest.CaptureFixture) -> None:
+    """Run a verbose command, silently.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     run("echo VERBS", silent=True)
     outerr = capsys.readouterr()
     assert not outerr.out
     assert not outerr.err
 
 
-def test_run_silent_command_verbosely(capsys):
-    """
-    Run a silent command, verbosely.
+def test_run_silent_command_verbosely(capsys: pytest.CaptureFixture) -> None:
+    """Run a silent command, verbosely.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     run(["true"])
     outerr = capsys.readouterr()
     assert "true" in outerr.out
     assert not outerr.err
 
 
-def test_run_failing_silent_command_verbosely(capsys):
-    """
-    Run a failing silent command, verbosely.
+def test_run_failing_silent_command_verbosely(capsys: pytest.CaptureFixture) -> None:
+    """Run a failing silent command, verbosely.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     run(["false"])
     outerr = capsys.readouterr()
     assert "false" in outerr.out
     assert not outerr.err
 
 
-def test_run_verbose_command_verbosely(capsys):
-    """
-    Run a verbose command, verbosely.
+def test_run_verbose_command_verbosely(capsys: pytest.CaptureFixture) -> None:
+    """Run a verbose command, verbosely.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     assert run("echo VERBS").code == 0
     outerr = capsys.readouterr()
     assert "VERBS" in outerr.out
     assert not outerr.err
 
 
-def return_success_code():
+def test_return_success_code() -> None:
     """Check the return code of a successful command."""
     assert run(["true"]).code == 0
 
 
-def return_failure_code():
+def test_return_failure_code() -> None:
     """Check the return code of a failing command."""
     assert run(["false"]).code == 1
 
 
-def return_shell_custom_code():
+def test_return_shell_custom_code() -> None:
     """Check the return code of a shell exit."""
-    assert run("exit 15").code == 15  # noqa: WPS432 (magic number)
+    assert run("exit 15").code == 15
 
 
 @pytest.mark.skipif(WINDOWS, reason="runs on Linux only")
-def run_linux_shell_command(capsys):
-    """
-    Run a Linux shell command.
+def test_run_linux_shell_command() -> None:
+    """Run a Linux shell command.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
-    assert run("echo herbert | grep -o er", capture=False, silent=True).code == 0
-    outerr = capsys.readouterr()
-    assert outerr.out.split("\n") == ["er", "er"]
-    assert not outerr.err
+    result = run("echo herbert | grep -o er", capture=True, silent=True)
+    assert result.code == 0
+    assert result.output.split("\n").count("er") == 2
 
 
 @pytest.mark.skipif(WINDOWS, reason="runs on Linux only")
-def test_run_linux_program():
+def test_run_linux_program() -> None:
     """Run a GNU/Linux program."""
     marker = "THIS VERY LINE"
     assert run(["grep", "-q", marker, __file__]).code == 0
     assert run(["grep", "-q", r"NOT\s*THIS\s*LINE", __file__]).code == 1
 
 
 @given(integers())
-def test_callable_exit_codes(code):
-    """
-    Check the return codes of Python callables.
+def test_callable_exit_codes(code: int) -> None:
+    """Check the return codes of Python callables.
 
     Arguments:
         code: Hypothesis fixture to provide various integers.
     """
     assert run(lambda: code).code == code
 
 
-def test_succeed_with_none_result():
+def test_handling_system_exit() -> None:
+    """Check that we handle system exit."""
+    assert run(lambda: sys.exit()).code == 0
+    assert run(lambda: sys.exit(0)).code == 0
+    assert run(lambda: sys.exit(1)).code == 1
+    assert run(lambda: sys.exit("bye")).code == 1
+
+
+def test_succeed_with_none_result() -> None:
     """Check the return code when a callable returns `None`."""
     assert run(lambda: None).code == 0
 
 
-def test_succeed_with_truthy_object():
+def test_succeed_with_truthy_object() -> None:
     """Check the return code when a callable returns a truthy object."""
     assert run(object).code == 0
 
 
-def test_fails_with_falsy_object():
+def test_fails_with_falsy_object() -> None:
     """Check the return code when a callable returns a falsy object."""
 
-    class Meh:  # noqa: C0115,WPS431 (missing docstring, nested class)
+    class Meh:
         def __bool__(self):
             return False
 
     assert run(Meh).code == 1
 
 
-def test_run_callable_return_boolean():
+def test_run_callable_return_boolean() -> None:
     """Check the return code when a callable returns a boolean."""
     assert run(lambda: True).code == 0
-    assert run(lambda: False).code == 1  # noqa: WPS522 (implicit primitive/lambda)
+    assert run(lambda: False).code == 1
 
 
-def test_callable_capture_none(capsys):
-    """
-    Check that nothing is captured while running a callable.
+def test_callable_capture_none(capsys: pytest.CaptureFixture) -> None:
+    """Check that nothing is captured while running a callable.
 
     Arguments:
         capsys: Pytest fixture to capture output.
     """
     msg = "out"
-    assert run(lambda: print(msg), capture=False, silent=True).code == 0  # noqa: WPS421 (print)
+    assert run(lambda: print(msg), capture=False, silent=True).code == 0
     outerr = capsys.readouterr()
     assert msg in outerr.out
 
 
-def test_callable_capture_both(capsys):
-    """
-    Check that all is captured while running a callable.
-
-    Arguments:
-        capsys: Pytest fixture to capture output.
-    """
+def test_callable_capture_both() -> None:
+    """Check that all is captured while running a callable."""
     msg_stdout = "out\n"
     msg_stderr = "err\n"
-    run(
+    result = run(
         lambda: sys.stdout.write(msg_stdout) and sys.stderr.write(msg_stderr),
         capture=True,
         fmt="custom={{output}}",
     )
-    outerr = capsys.readouterr()
-    assert msg_stdout in outerr.out
-    assert msg_stderr in outerr.out
-    assert not outerr.err
+    assert msg_stdout in result.output
+    assert msg_stderr in result.output
 
 
-def test_callable_capture_stdout(capsys):
-    """
-    Check that stdout is captured while running a callable.
-
-    Arguments:
-        capsys: Pytest fixture to capture output.
-    """
+def test_callable_capture_stdout() -> None:
+    """Check that stdout is captured while running a callable."""
     msg_stdout = "out"
     msg_stderr = "err"
-    run(
+    result = run(
         lambda: sys.stdout.write(msg_stdout) and sys.stderr.write(msg_stderr),
         capture="stdout",
         fmt="custom={{output}}",
     )
-    outerr = capsys.readouterr()
-    assert msg_stdout in outerr.out
-    assert msg_stderr not in outerr.out
-    assert not outerr.err
-
+    assert msg_stdout in result.output
+    assert msg_stderr not in result.output
 
-def test_callable_capture_stderr(capsys):
-    """
-    Check that stderr is captured while running a callable.
 
-    Arguments:
-        capsys: Pytest fixture to capture output.
-    """
+def test_callable_capture_stderr() -> None:
+    """Check that stderr is captured while running a callable."""
     msg_stdout = "out"
     msg_stderr = "err"
-    run(
+    result = run(
         lambda: sys.stdout.write(msg_stdout) and sys.stderr.write(msg_stderr),
         capture="stderr",
         fmt="custom={{output}}",
     )
-    outerr = capsys.readouterr()
-    assert msg_stdout not in outerr.out
-    assert msg_stderr in outerr.out
-    assert not outerr.err
+    assert msg_stdout not in result.output
+    assert msg_stderr in result.output
 
 
-def test_process_capture_none(capfd):
-    """
-    Check that nothing is captured while running a process.
+def test_process_capture_none(capfd: pytest.CaptureFixture) -> None:
+    """Check that nothing is captured while running a process.
 
     Arguments:
         capfd: Pytest fixture to capture output.
     """
     assert run([sys.executable, "-V"], capture=False, silent=True).code == 0
     outerr = capfd.readouterr()
     assert "Python" in outerr.out
 
 
-def test_process_capture_both(capsys):
-    """
-    Check that all is captured while running a process.
-
-    Arguments:
-        capsys: Pytest fixture to capture output.
-    """
+def test_process_capture_both() -> None:
+    """Check that all is captured while running a process."""
     msg_stdout = "out"
     msg_stderr = "err"
-    run(
+    result = run(
         ["bash", "-c", f"echo {msg_stdout}; echo {msg_stderr} >&2"],
         capture=True,
         fmt="custom={{output}}",
     )
-    outerr = capsys.readouterr()
-    assert msg_stdout in outerr.out
-    assert msg_stderr in outerr.out
-    assert not outerr.err
+    assert msg_stdout in result.output
+    assert msg_stderr in result.output
 
 
-def test_process_capture_stdout(capsys):
-    """
-    Check that stdout is captured while running a process.
-
-    Arguments:
-        capsys: Pytest fixture to capture output.
-    """
+def test_process_capture_stdout() -> None:
+    """Check that stdout is captured while running a process."""
     msg_stdout = "out"
     msg_stderr = "err"
-    run(
+    result = run(
         ["bash", "-c", f"echo {msg_stdout}; echo {msg_stderr} >&2"],
         capture="stdout",
         fmt="custom={{output}}",
     )
-    outerr = capsys.readouterr()
-    assert msg_stdout in outerr.out
-    assert msg_stderr not in outerr.out
-    assert not outerr.err
-
+    assert msg_stdout in result.output
+    assert msg_stderr not in result.output
 
-def test_process_capture_stderr(capsys):
-    """
-    Check that stderr is captured while running a process.
 
-    Arguments:
-        capsys: Pytest fixture to capture output.
-    """
+def test_process_capture_stderr() -> None:
+    """Check that stderr is captured while running a process."""
     msg_stdout = "out"
     msg_stderr = "err"
-    run(
+    result = run(
         ["bash", "-c", f"echo {msg_stdout}; echo {msg_stderr} >&2"],
         capture="stderr",
         fmt="custom={{output}}",
     )
-    outerr = capsys.readouterr()
-    assert msg_stdout not in outerr.out
-    assert msg_stderr in outerr.out
-    assert not outerr.err
+    assert msg_stdout not in result.output
+    assert msg_stderr in result.output
 
 
-def test_cancel_pty():
+def test_cancel_pty() -> None:
     """Test that using PTY is canceled if the format does not support it."""
-    with patch("failprint.runners.run_subprocess", new=MagicMock(return_value=(0, ""))) as run_sub:
+    with patch("failprint.runners.run_subprocess", new=MagicMock(return_value=(0, ""))) as run_sub:  # noqa: SIM117
         with patch("failprint.runners.run_pty_subprocess", new=MagicMock(return_value=(0, ""))) as run_pty_sub:
             run("true", pty=True, fmt="tap")
             assert not run_pty_sub.called
             assert run_sub.called
 
 
 @pytest.mark.skipif(WINDOWS, reason="no PTY support on Windows")
-def test_run_pty_shell():
+def test_run_pty_shell() -> None:
     """Test running a shell command in a PTY."""
     with patch("failprint.runners.run_pty_subprocess", new=MagicMock(return_value=(0, ""))) as run_pty_sub:
         run("true", pty=True)
         assert run_pty_sub.called
 
 
-def test_run_callable_raising_exception(capsys):
-    """
-    Test running a callable raising an exception.
+def test_run_callable_raising_exception(capfd: pytest.CaptureFixture) -> None:
+    """Test running a callable raising an exception.
 
     Arguments:
-        capsys: Pytest fixture to capture output.
+        capfd: Pytest fixture to capture output.
     """
-    assert run(lambda: 1 / 0).code == 1  # noqa: WPS344 (zero division)
-    outerr = capsys.readouterr()
+    assert run(lambda: 1 / 0).code == 1
+    outerr = capfd.readouterr()
     assert "ZeroDivisionError:" in outerr.out
 
 
 @given(text(alphabet=characters(blacklist_categories="C")))
-def test_pass_stdin_to_function(stdin):
-    """
-    Pass input to a normal subprocess.
+def test_pass_stdin_to_function(stdin: str) -> None:
+    """Pass input to a normal subprocess.
 
     Arguments:
         stdin: Text sample generated by Hypothesis.
     """
 
-    def print_stdin():  # noqa: WPS430
+    def print_stdin() -> None:
         print(sys.stdin.read(), end="")
 
     code, output = run_function(print_stdin, stdin=stdin)
     assert code == 0
     assert output == stdin
+
+
+def test_run_lazy_callable(capfd: pytest.CaptureFixture) -> None:
+    """Assert we can run a lazy callable and stringify it.
+
+    Arguments:
+        capfd: Pytest fixture to capture output.
+    """
+
+    @lazy
+    def greet(name: str) -> int:
+        print(f"hello {name}")
+        return 1
+
+    result = run(greet("tim"))
+    outerr = capfd.readouterr()
+    assert result.code == 1
+    assert result.output == "hello tim\n"
+    assert "greet('tim')" in outerr.out
+
+
+def test_run_lazy_callable_without_calling_it(capfd: pytest.CaptureFixture) -> None:
+    """Assert we can run a lazy callable without actually calling it.
+
+    Arguments:
+        capfd: Pytest fixture to capture output.
+    """
+
+    @lazy
+    def greet(name: str) -> int:
+        print(f"hello {name}")
+        return 1
+
+    result = run(greet, args=["tim"])
+    outerr = capfd.readouterr()
+    assert result.code == 1
+    assert result.output == "hello tim\n"
+    assert "greet('tim')" in outerr.out
+
+
+def test_capture_function_and_subprocess_output(capsys: pytest.CaptureFixture) -> None:
+    """Assert we capture everything when running a function.
+
+    Arguments:
+        capsys: Pytest fixture to capture output.
+    """
+
+    def function() -> None:
+        print("print")
+        sys.stdout.write("sys stdout write\n")
+        os.system("echo os system")  # noqa: S605,S607
+        subprocess.run(["sh", "-c", "echo sh -c echo"])  # noqa: S603,S607
+
+    with capsys.disabled(), Capture.BOTH.here() as captured:
+        function()
+
+    lines = str(captured).rstrip("\n").split("\n")
+    assert lines == ["print", "sys stdout write", "os system", "sh -c echo"]
```

### Comparing `failprint-0.9.0/PKG-INFO` & `failprint-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: failprint
-Version: 0.9.0
+Version: 1.0.0
 Summary: Run a command, print its output only if it fails.
+Keywords: cli failure output runner
+Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
-Keywords: cli,failure,output,runner
-Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Project-URL: Homepage, https://pawamoy.github.io/failprint
+Project-URL: Documentation, https://pawamoy.github.io/failprint
 Project-URL: Changelog, https://pawamoy.github.io/failprint/changelog
+Project-URL: Repository, https://github.com/pawamoy/failprint
+Project-URL: Issues, https://github.com/pawamoy/failprint/issues
 Project-URL: Discussions, https://github.com/pawamoy/failprint/discussions
-Project-URL: Documentation, https://pawamoy.github.io/failprint
-Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/failprint/community
-Project-URL: Homepage, https://pawamoy.github.io/failprint
-Project-URL: Issues, https://github.com/pawamoy/failprint/issues
-Project-URL: Repository, https://github.com/pawamoy/failprint
+Project-URL: Funding, https://github.com/sponsors/pawamoy
+Requires-Python: >=3.8
+Requires-Dist: ansimarkup~=1.4
+Requires-Dist: jinja2<4,>=2.11
+Requires-Dist: ptyprocess~=0.6; sys_platform != "win32"
+Requires-Dist: typing-extensions>=4.1; python_version < "3.10"
 Description-Content-Type: text/markdown
 
 # failprint
 
 [![ci](https://github.com/pawamoy/failprint/workflows/ci/badge.svg)](https://github.com/pawamoy/failprint/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/failprint/)
 [![pypi version](https://img.shields.io/pypi/v/failprint.svg)](https://pypi.org/project/failprint/)
@@ -91,15 +94,15 @@
 With `pip`:
 ```bash
 pip install failprint
 ```
 
 With [`pipx`](https://github.com/pipxproject/pipx):
 ```bash
-python3.7 -m pip install --user pipx
+python3.8 -m pip install --user pipx
 pipx install failprint
 ```
 
 ## Usage
 
 ```console
 % poetry run failprint -h
@@ -153,8 +156,7 @@
     pty=False,      # use a PTY
     progress=True,  # print the "progress" template before running the command
     nofail=False,   # always return zero
     quiet=False,    # don't print output when the command fails
     silent=False,   # don't print anything
 )
 ```
-
```

#### html2text {}

```diff
@@ -1,32 +1,34 @@
-Metadata-Version: 2.1 Name: failprint Version: 0.9.0 Summary: Run a command,
-print its output only if it fails. License: ISC Keywords:
-cli,failure,output,runner Author-email: TimothÃ©e Mazzucotelli
-pm.me> Requires-Python: >=3.7 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Metadata-Version: 2.1 Name: failprint Version: 1.0.0 Summary: Run a command,
+print its output only if it fails. Keywords: cli failure output runner Author-
+Email: TimothÃ©e Mazzucotelli
+pm.me> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
+3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Documentation Classifier: Topic :: Software Development Classifier: Topic ::
-Software Development :: Documentation Classifier: Topic :: Utilities
-Classifier: Typing :: Typed Project-URL: Changelog, https://pawamoy.github.io/
-failprint/changelog Project-URL: Discussions, https://github.com/pawamoy/
-failprint/discussions Project-URL: Documentation, https://pawamoy.github.io/
-failprint Project-URL: Funding, https://github.com/sponsors/pawamoy Project-
-URL: Gitter, https://gitter.im/failprint/community Project-URL: Homepage,
-https://pawamoy.github.io/failprint Project-URL: Issues, https://github.com/
-pawamoy/failprint/issues Project-URL: Repository, https://github.com/pawamoy/
-failprint Description-Content-Type: text/markdown # failprint [![ci](https://
-github.com/pawamoy/failprint/workflows/ci/badge.svg)](https://github.com/
-pawamoy/failprint/actions?query=workflow%3Aci) [![documentation](https://
-img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://
-pawamoy.github.io/failprint/) [![pypi version](https://img.shields.io/pypi/v/
-failprint.svg)](https://pypi.org/project/failprint/) [![gitpod](https://
+Utilities Classifier: Typing :: Typed Project-URL: Homepage, https://
+pawamoy.github.io/failprint Project-URL: Documentation, https://
+pawamoy.github.io/failprint Project-URL: Changelog, https://pawamoy.github.io/
+failprint/changelog Project-URL: Repository, https://github.com/pawamoy/
+failprint Project-URL: Issues, https://github.com/pawamoy/failprint/issues
+Project-URL: Discussions, https://github.com/pawamoy/failprint/discussions
+Project-URL: Gitter, https://gitter.im/failprint/community Project-URL:
+Funding, https://github.com/sponsors/pawamoy Requires-Python: >=3.8 Requires-
+Dist: ansimarkup~=1.4 Requires-Dist: jinja2<4,>=2.11 Requires-Dist:
+ptyprocess~=0.6; sys_platform != "win32" Requires-Dist: typing-extensions>=4.1;
+python_version < "3.10" Description-Content-Type: text/markdown # failprint [!
+[ci](https://github.com/pawamoy/failprint/workflows/ci/badge.svg)](https://
+github.com/pawamoy/failprint/actions?query=workflow%3Aci) [![documentation]
+(https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)]
+(https://pawamoy.github.io/failprint/) [![pypi version](https://img.shields.io/
+pypi/v/failprint.svg)](https://pypi.org/project/failprint/) [![gitpod](https://
 img.shields.io/badge/gitpod-workspace-blue.svg?style=flat)](https://gitpod.io/
 #https://github.com/pawamoy/failprint) [![gitter](https://badges.gitter.im/
 join%20chat.svg)](https://gitter.im/failprint/community) Run a command, print
 its output only if it fails. Tired of searching the `quiet` options of your
 programs to lighten up the output of your `make check` or `make lint` commands?
 Tired of finding out that standard output and error are mixed up in some of
 them? Simply run your command through `failprint`. If it succeeds, nothing is
@@ -38,15 +40,15 @@
 Requirements failprint requires Python 3.6 or above.  To install Python 3.6, I
 recommend using pyenv. ```bash # install pyenv git clone https://github.com/
 pyenv/pyenv ~/.pyenv # setup pyenv (you should also put these three lines in
 .bashrc or similar) export PATH="${HOME}/.pyenv/bin:${PATH}" export
 PYENV_ROOT="${HOME}/.pyenv" eval "$(pyenv init -)" # install Python 3.6 pyenv
 install 3.6.12 # make it available globally pyenv global system 3.6.12 ```  ##
 Installation With `pip`: ```bash pip install failprint ``` With [`pipx`](https:
-//github.com/pipxproject/pipx): ```bash python3.7 -m pip install --user pipx
+//github.com/pipxproject/pipx): ```bash python3.8 -m pip install --user pipx
 pipx install failprint ``` ## Usage ```console % poetry run failprint -h usage:
 failprint [-h] [-c {stdout,stderr,both,none}] [-f {pretty,tap}] [-y | -Y] [-p |
 -P] [-q | -Q] [-s | -S] [-z | -Z] [-n NUMBER] [-t TITLE] COMMAND [COMMAND ...]
 positional arguments: COMMAND optional arguments: -h, --help show this help
 message and exit -c {stdout,stderr,both,none}, --capture
 {stdout,stderr,both,none} Which output to capture. Colors are supported with
 'both' only, unless the command has a 'force color' option. -f {pretty,tap}, --
```

