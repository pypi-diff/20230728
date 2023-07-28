# Comparing `tmp/typetest-cli-1.2.1.tar.gz` & `tmp/typetest-cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typetest-cli-1.2.1.tar", last modified: Fri Jul 14 15:57:42 2023, max compression
+gzip compressed data, was "typetest-cli-1.2.2.tar", last modified: Fri Jul 28 00:19:50 2023, max compression
```

## Comparing `typetest-cli-1.2.1.tar` & `typetest-cli-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-14 15:57:42.007283 typetest-cli-1.2.1/
--rw-r--r--   0 senyc     (1000) senyc     (1000)     1062 2023-07-07 01:09:21.000000 typetest-cli-1.2.1/LICENSE
--rw-r--r--   0 senyc     (1000) senyc     (1000)       29 2023-07-10 21:11:04.000000 typetest-cli-1.2.1/MANIFEST.in
--rw-r--r--   0 senyc     (1000) senyc     (1000)     1631 2023-07-14 15:57:42.007283 typetest-cli-1.2.1/PKG-INFO
--rw-r--r--   0 senyc     (1000) senyc     (1000)     1021 2023-07-10 23:35:08.000000 typetest-cli-1.2.1/README.rst
--rw-r--r--   0 senyc     (1000) senyc     (1000)      957 2023-07-14 15:51:48.000000 typetest-cli-1.2.1/pyproject.toml
--rw-r--r--   0 senyc     (1000) senyc     (1000)       38 2023-07-14 15:57:42.007283 typetest-cli-1.2.1/setup.cfg
--rw-r--r--   0 senyc     (1000) senyc     (1000)      328 2023-07-08 22:22:54.000000 typetest-cli-1.2.1/setup.py
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-14 15:57:42.003950 typetest-cli-1.2.1/src/
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-14 15:57:42.007283 typetest-cli-1.2.1/src/typetest_cli/
--rw-r--r--   0 senyc     (1000) senyc     (1000)        0 2023-07-07 21:44:48.000000 typetest-cli-1.2.1/src/typetest_cli/__init__.py
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-14 15:57:42.007283 typetest-cli-1.2.1/src/typetest_cli/text/
--rw-r--r--   0 senyc     (1000) senyc     (1000)       81 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/eight.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       57 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/five.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       83 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/four.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      117 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/nine.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      114 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/one.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       97 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/seven.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       88 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/six.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      169 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/ten.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       93 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/three.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)      115 2023-07-07 21:35:59.000000 typetest-cli-1.2.1/src/typetest_cli/text/two.txt
--rwxr-xr-x   0 senyc     (1000) senyc     (1000)     4992 2023-07-14 15:49:31.000000 typetest-cli-1.2.1/src/typetest_cli/typetest.py
-drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-14 15:57:42.007283 typetest-cli-1.2.1/src/typetest_cli.egg-info/
--rw-r--r--   0 senyc     (1000) senyc     (1000)     1631 2023-07-14 15:57:42.000000 typetest-cli-1.2.1/src/typetest_cli.egg-info/PKG-INFO
--rw-r--r--   0 senyc     (1000) senyc     (1000)      663 2023-07-14 15:57:42.000000 typetest-cli-1.2.1/src/typetest_cli.egg-info/SOURCES.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)        1 2023-07-14 15:57:42.000000 typetest-cli-1.2.1/src/typetest_cli.egg-info/dependency_links.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       98 2023-07-14 15:57:42.000000 typetest-cli-1.2.1/src/typetest_cli.egg-info/entry_points.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)        5 2023-07-14 15:57:42.000000 typetest-cli-1.2.1/src/typetest_cli.egg-info/requires.txt
--rw-r--r--   0 senyc     (1000) senyc     (1000)       13 2023-07-14 15:57:42.000000 typetest-cli-1.2.1/src/typetest_cli.egg-info/top_level.txt
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-28 00:19:50.128046 typetest-cli-1.2.2/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)     1062 2023-07-07 01:09:21.000000 typetest-cli-1.2.2/LICENSE
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       29 2023-07-10 21:11:04.000000 typetest-cli-1.2.2/MANIFEST.in
+-rw-r--r--   0 senyc     (1000) senyc     (1000)     1730 2023-07-28 00:19:50.128046 typetest-cli-1.2.2/PKG-INFO
+-rw-r--r--   0 senyc     (1000) senyc     (1000)     1120 2023-07-15 16:04:57.000000 typetest-cli-1.2.2/README.rst
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      991 2023-07-28 00:09:36.000000 typetest-cli-1.2.2/pyproject.toml
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       38 2023-07-28 00:19:50.128046 typetest-cli-1.2.2/setup.cfg
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      328 2023-07-08 22:22:54.000000 typetest-cli-1.2.2/setup.py
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-28 00:19:50.124713 typetest-cli-1.2.2/src/
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-28 00:19:50.124713 typetest-cli-1.2.2/src/typetest_cli/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)        0 2023-07-27 23:49:40.000000 typetest-cli-1.2.2/src/typetest_cli/__init__.py
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-28 00:19:50.128046 typetest-cli-1.2.2/src/typetest_cli/text/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       81 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/eight.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       57 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/five.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       83 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/four.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      117 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/nine.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      114 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/one.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       97 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/seven.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       88 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/six.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      169 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/ten.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       93 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/three.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      115 2023-07-07 21:35:59.000000 typetest-cli-1.2.2/src/typetest_cli/text/two.txt
+-rwxr-xr-x   0 senyc     (1000) senyc     (1000)     5383 2023-07-27 23:48:12.000000 typetest-cli-1.2.2/src/typetest_cli/typetest.py
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-28 00:19:50.124713 typetest-cli-1.2.2/src/typetest_cli.egg-info/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)     1730 2023-07-28 00:19:50.000000 typetest-cli-1.2.2/src/typetest_cli.egg-info/PKG-INFO
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      725 2023-07-28 00:19:50.000000 typetest-cli-1.2.2/src/typetest_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)        1 2023-07-28 00:19:50.000000 typetest-cli-1.2.2/src/typetest_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       98 2023-07-28 00:19:50.000000 typetest-cli-1.2.2/src/typetest_cli.egg-info/entry_points.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)        5 2023-07-28 00:19:50.000000 typetest-cli-1.2.2/src/typetest_cli.egg-info/requires.txt
+-rw-r--r--   0 senyc     (1000) senyc     (1000)       13 2023-07-28 00:19:50.000000 typetest-cli-1.2.2/src/typetest_cli.egg-info/top_level.txt
+drwxr-xr-x   0 senyc     (1000) senyc     (1000)        0 2023-07-28 00:19:50.128046 typetest-cli-1.2.2/tests/
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      770 2023-07-28 00:00:30.000000 typetest-cli-1.2.2/tests/test_calculations.py
+-rw-r--r--   0 senyc     (1000) senyc     (1000)      479 2023-07-27 23:56:59.000000 typetest-cli-1.2.2/tests/test_character_validation.py
```

### Comparing `typetest-cli-1.2.1/LICENSE` & `typetest-cli-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `typetest-cli-1.2.1/PKG-INFO` & `typetest-cli-1.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetest-cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Lightweight typing speed commandline tool
 Author: Kyler
 Project-URL: repository, https://github.com/senyc/typetest-cli
 Keywords: speed,test,typing,typetest,typetest-cli,terminal
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.8
@@ -49,20 +49,22 @@
 ========================
 
 After install you should be able to run the program with ``typetest`` or ``typetest-cli``
 
 Usage
 --------
 
-.. code-block:: bash
-
-    usage: typetest [-h] [--hide-acc] [--hide-wpm] [--only-base]
+.. code-block::
 
+    usage: typetest [-h] [--hide-acc] [--hide-wpm] [--only-base] [--no-blocking]
+    
     Lightweight typing speed commandline tool. Can be exited with Ctrl-c or return.
-
+    
     options:
-      -h, --help       show this help message and exit
-      --hide-acc, -a   hides the accuracy statistic
-      --hide-wpm, -w   hides the word per minute statistic
-      --only-base, -b  Only uses the base text
-
+      -h, --help         show this help message and exit
+      --hide-acc, -a     hides the accuracy statistic
+      --hide-wpm, -w     hides the word per minute statistic
+      --only-base, -b    Only uses the base text
+      --no-blocking, -n  Do not block input after 3 failed attmpts
+    
     Will only disply typing speed and accuracy upon completion of the line
+
```

### Comparing `typetest-cli-1.2.1/README.rst` & `typetest-cli-1.2.2/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -32,20 +32,22 @@
 ========================
 
 After install you should be able to run the program with ``typetest`` or ``typetest-cli``
 
 Usage
 --------
 
-.. code-block:: bash
-
-    usage: typetest [-h] [--hide-acc] [--hide-wpm] [--only-base]
+.. code-block::
 
+    usage: typetest [-h] [--hide-acc] [--hide-wpm] [--only-base] [--no-blocking]
+    
     Lightweight typing speed commandline tool. Can be exited with Ctrl-c or return.
-
+    
     options:
-      -h, --help       show this help message and exit
-      --hide-acc, -a   hides the accuracy statistic
-      --hide-wpm, -w   hides the word per minute statistic
-      --only-base, -b  Only uses the base text
-
+      -h, --help         show this help message and exit
+      --hide-acc, -a     hides the accuracy statistic
+      --hide-wpm, -w     hides the word per minute statistic
+      --only-base, -b    Only uses the base text
+      --no-blocking, -n  Do not block input after 3 failed attmpts
+    
     Will only disply typing speed and accuracy upon completion of the line
+
```

### Comparing `typetest-cli-1.2.1/pyproject.toml` & `typetest-cli-1.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+[tool.black]
+line-length = 100
+
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "typetest-cli"
-version = "1.2.1"
+version = "1.2.2"
 authors = [{ name = 'Kyler' }]
 description = "Lightweight typing speed commandline tool"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = ["rich"]
 keywords = ["speed", "test", "typing", "typetest", "typetest-cli", "terminal"]
 classifiers = [
@@ -30,8 +33,9 @@
 license-files = ["LICENSE"]
 
 [tool.setuptools.package-data]
 "typetest_cli.text" = ["*.txt"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
-exclude = ["tests*"]
+exclude = ["*tests*"]
+
```

### Comparing `typetest-cli-1.2.1/src/typetest_cli/typetest.py` & `typetest-cli-1.2.2/src/typetest_cli/typetest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,156 @@
 #!/usr/bin/env python3
 
+from contextlib import contextmanager
+from itertools import zip_longest
+from typing import Final
 import argparse
 import glob
 import os
 import random
 import sys
 import termios
 import time
 import tty
-from contextlib import contextmanager
-from typing import Final
 
 from rich.console import Console
 from rich.live import Live
 
-user_dir = os.path.expanduser('~')
+user_dir = os.path.expanduser("~")
 here = os.path.abspath(os.path.dirname(__file__))
 
-SOURCE_DIR: Final[str] = f'{here}/text'
-EXTERN_DIR: Final[str] = f'{user_dir}/.local/share/typetest-cli/text'
+SOURCE_DIR: Final[str] = f"{here}/text"
+EXTERN_DIR: Final[str] = f"{user_dir}/.local/share/typetest-cli/text"
 MAX_SUBSEUQENT_ERRORS: Final[int] = 3
+LETTERS_PER_WORD: Final[int] = 5
+
 
 @contextmanager
 def raw_mode(file):
     """Puts the terminal into raw mode, allowing for full reading of user input.
     On exit, restores the terminal to previous settings."""
     old_settings = termios.tcgetattr(file.fileno())
     try:
         tty.setraw(file.fileno())
         yield
     finally:
         termios.tcsetattr(file.fileno(), termios.TCSADRAIN, old_settings)
 
+
 def get_char() -> str:
     """Gets the next character input from the user"""
     with raw_mode(sys.stdin):
         char = sys.stdin.read(1)
     return char
 
+
 def format_text(source: str, user_input: str) -> str:
-    final_text = ''
+    final_text = ""
     for source_char, input_char in zip(source, user_input):
         if source_char == input_char:
-            final_text += f'[green]{source_char}[/]'
+            final_text += f"[green]{source_char}[/]"
         else:
             final_text += f"[red]{source_char if source_char != ' ' else '_'}[/]"
     if len(user_input) < len(source):
         return final_text + f"[blue]{source[len(user_input)]}[/]{source[len(user_input) + 1:]}"
     return final_text
 
-def calc_wpm(time_seconds: float, letters: int) -> int:
-    words = letters / 5
+
+def calc_wpm(time_seconds: float, letters: int, letters_per_word: int) -> int:
+    words = letters / letters_per_word
     minutes = time_seconds / 60
     return int(words // minutes)
 
-def get_accuracy(failures: int, letters: int) -> int:
+
+def get_accuracy_percent(failures: int, letters: int) -> int:
     return int(((letters - failures) / letters) * 100)
 
+
 def count_failures(source: str, user_input: str) -> int:
     failures = 0
-    for source_letter, user_input_letter in zip(source, user_input):
+    for source_letter, user_input_letter in zip_longest(source, user_input):
         if user_input_letter != source_letter:
             failures += 1
     return failures
 
+
 def get_random_file(*args) -> str:
     options = []
     for directory in args:
-        files = glob.glob(f'{directory}/*')
+        files = glob.glob(f"{directory}/*")
         options.extend(files)
     return random.choice(options)
 
+
 def not_quit(char: str) -> bool:
-    """Checks for SIGINT or return"""
-    return not (char != '' and ord(char) == 3) or (char == '\n' or char == '\r')
+    """Checks for SIGINT"""
+    return ord(str(char)) != 3
+
 
 def is_backspace(char: str) -> bool:
-    return char == '\x7f'
+    return char == "\x7f"
+
 
 def add_to(current_input: str, new_char: str) -> str:
     if is_backspace(new_char):
         if len(current_input) > 0:
             return current_input[:-1]
         else:
             return current_input
     return current_input + new_char
 
+
 def is_input_error(char: str, DATA: str, input_index: int) -> bool:
     if is_backspace(char):
         return False
     return char != DATA[input_index]
 
+
 def main() -> None:
     parser = argparse.ArgumentParser(
-        prog='typetest',
-        description='Lightweight typing speed commandline tool. Can be exited with Ctrl-c or return.',
-        epilog='Will only disply typing speed and accuracy upon completion of the line'
+        prog="typetest",
+        description="Lightweight typing speed commandline tool. Can be exited with ctrl-c",
+        epilog="Will only disply typing speed and accuracy upon completion of the text.",
     )
 
-    parser.add_argument('--hide-acc', '-a', action='store_true', help='hides the accuracy statistic')
-    parser.add_argument('--hide-wpm', '-w', action='store_true', help='hides the word per minute statistic')
-    parser.add_argument('--only-base', '-b', action='store_false', help='Only uses the base text')
-    parser.add_argument('--no-blocking', '-n', action='store_false', help='Do not block input after 3 failed attmpts')
+    parser.add_argument(
+        "file_path", metavar="file_path", type=str, nargs="?", help="path to read file"
+    )
+    parser.add_argument(
+        "--hide-acc", "-a", action="store_true", help="hides the accuracy statistic"
+    )
+    parser.add_argument(
+        "--hide-wpm",
+        "-w",
+        action="store_true",
+        help="hides the word per minute statistic",
+    )
+    parser.add_argument("--only-base", "-b", action="store_false", help="Only uses the base text")
+    parser.add_argument(
+        "--no-blocking",
+        "-n",
+        action="store_false",
+        help="Do not block input after 3 failed attmpts",
+    )
 
     args = parser.parse_args()
-    if args.only_base:
+
+    if args.file_path and os.path.exists(args.file_path):
+        file = args.file_path
+    elif args.only_base:
         file = get_random_file(SOURCE_DIR)
     else:
         file = get_random_file(SOURCE_DIR, EXTERN_DIR)
 
-    with open(file, encoding='utf-8', mode='r') as file:
-        DATA = file.read().strip('\n').strip(' ')
+    with open(file, encoding="utf-8", mode="r") as file:
+        DATA = file.read().strip("\n").strip(" ")
 
     console = Console(soft_wrap=False, no_color=False)
     start = end = None
-    user_input = ''
+    user_input = ""
     subsequent_errors: int = 0
 
     with Live(console=console, auto_refresh=False) as display:
         display.update(DATA, refresh=True)
         while not_quit(char := get_char()):
             if start is None:
                 start = time.time()
@@ -138,16 +170,15 @@
         end = time.time()
         display.update(format_text(DATA, user_input), refresh=True)
 
     if len(user_input) != len(DATA):
         return
 
     if not args.hide_acc:
-        print(get_accuracy(count_failures(DATA, user_input), len(DATA)), "percent correct")
+        print(get_accuracy_percent(count_failures(DATA, user_input), len(DATA)), "percent correct")
 
     if not args.hide_wpm:
-        print(calc_wpm(end - start, len(DATA)), "words per minute")
+        print(calc_wpm(end - start, len(DATA), LETTERS_PER_WORD), "words per minute")
 
 
 if __name__ == '__main__':
     main()
-
```

### Comparing `typetest-cli-1.2.1/src/typetest_cli.egg-info/PKG-INFO` & `typetest-cli-1.2.2/src/typetest_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typetest-cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Lightweight typing speed commandline tool
 Author: Kyler
 Project-URL: repository, https://github.com/senyc/typetest-cli
 Keywords: speed,test,typing,typetest,typetest-cli,terminal
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.8
@@ -49,20 +49,22 @@
 ========================
 
 After install you should be able to run the program with ``typetest`` or ``typetest-cli``
 
 Usage
 --------
 
-.. code-block:: bash
-
-    usage: typetest [-h] [--hide-acc] [--hide-wpm] [--only-base]
+.. code-block::
 
+    usage: typetest [-h] [--hide-acc] [--hide-wpm] [--only-base] [--no-blocking]
+    
     Lightweight typing speed commandline tool. Can be exited with Ctrl-c or return.
-
+    
     options:
-      -h, --help       show this help message and exit
-      --hide-acc, -a   hides the accuracy statistic
-      --hide-wpm, -w   hides the word per minute statistic
-      --only-base, -b  Only uses the base text
-
+      -h, --help         show this help message and exit
+      --hide-acc, -a     hides the accuracy statistic
+      --hide-wpm, -w     hides the word per minute statistic
+      --only-base, -b    Only uses the base text
+      --no-blocking, -n  Do not block input after 3 failed attmpts
+    
     Will only disply typing speed and accuracy upon completion of the line
+
```

