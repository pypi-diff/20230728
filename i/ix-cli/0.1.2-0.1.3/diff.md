# Comparing `tmp/ix_cli-0.1.2.tar.gz` & `tmp/ix_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ix_cli-0.1.2.tar", max compression
+gzip compressed data, was "ix_cli-0.1.3.tar", max compression
```

## Comparing `ix_cli-0.1.2.tar` & `ix_cli-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      101 2023-03-10 01:37:38.985439 ix_cli-0.1.2/ix_cli/__init__.py
--rw-r--r--   0        0        0     5255 2023-03-10 01:52:21.424206 ix_cli-0.1.2/ix_cli/cli.py
--rw-r--r--   0        0        0     4811 2023-03-10 02:39:55.778414 ix_cli-0.1.2/ix_cli/utils.py
--rw-r--r--   0        0        0     1068 2023-03-10 02:00:49.732923 ix_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0      458 2023-03-10 02:41:36.124777 ix_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2509 2023-03-10 02:18:33.098490 ix_cli-0.1.2/README.md
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 ix_cli-0.1.2/setup.py
--rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 ix_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-28 00:52:46.524534 ix_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2632 2023-07-28 00:52:46.524534 ix_cli-0.1.3/README.md
+-rw-r--r--   0        0        0       95 2023-07-28 00:52:46.525534 ix_cli-0.1.3/ix_cli/__init__.py
+-rw-r--r--   0        0        0     5084 2023-07-28 00:52:46.525534 ix_cli-0.1.3/ix_cli/cli.py
+-rw-r--r--   0        0        0     4661 2023-07-28 00:52:46.525534 ix_cli-0.1.3/ix_cli/utils.py
+-rw-r--r--   0        0        0      692 2023-07-28 00:59:48.539424 ix_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3298 1970-01-01 00:00:00.000000 ix_cli-0.1.3/PKG-INFO
```

### Comparing `ix_cli-0.1.2/ix_cli/cli.py` & `ix_cli-0.1.3/ix_cli/cli.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-import typer
-import rich
-import json
-import sys
-import re
-
-from pathlib import Path
-from rich.table import Table
-
-from .utils import (
-    uploadFromFile,
-    uploadFromStdin,
-    download,
-    initHistory,
-    resetHistory,
-    console,
-    windowsDictRepair,
-    HISTORY_PATH,
-    PROVIDER_URL
-)
-
-PROVIDER_NAME = PROVIDER_URL.split("//")[-1]
-
-app = typer.Typer(
-    name="ix",
-    help=f"A CLI for interacting with the {PROVIDER_NAME} pastebin service.",
-    no_args_is_help=True,
-    rich_help_panel="rich",
-    rich_markup_mode="rich",
-)
-
-@app.command(
-    "f",
-    help=f"Upload a file to {PROVIDER_NAME}",
-    no_args_is_help=True,
-)
-def from_file(
-    filepath: Path = typer.Argument(
-        ...,
-        help="The path to the file to upload.", 
-        exists=True,
-        file_okay=True,
-        dir_okay=False,
-        readable=True
-        ),
-    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode.")
-    ):
-    initHistory(silent = not debug)
-    console.print(uploadFromFile(filepath))
-    
-@app.command(
-    "s",
-    help=f"Upload stdin to {PROVIDER_NAME}",
-    no_args_is_help=False,
-)
-def from_stdin(
-    param: str = typer.Argument(None, help=f"sdtin input to upload to {PROVIDER_NAME}, defaults to sys.argv"),
-    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
-):
-    param = ' '.join(sys.argv[2:])
-    param = param if param.strip() else None
-    initHistory(silent = not debug)
-    if response := uploadFromStdin(param):
-        console.print(response)
-    
-@app.command("h", help="Show the history of uploaded files.")
-def history():
-    if not HISTORY_PATH.exists():
-        console.print("No history found.", style="bold red")
-        return
-    jhistory = json.loads(HISTORY_PATH.read_text())
-    table = Table(show_header=True, header_style="bold magenta")
-    
-    table.add_column("ID", style="bold red", width=12)
-    table.add_column("Content-Start", style="bold yellow", justify="center")
-    table.add_column("Url", style="bold cyan", justify="center")
-    
-    for x in jhistory:
-        table.add_row(x["id"], x["name"], x["url"])
-        
-    console.print(table)
-    
-    
-@app.command(
-    "g",
-    help=f"Download a file from {PROVIDER_NAME}",
-    no_args_is_help=True,
-)
-def get(
-    param: str = typer.Argument(
-        ...,
-        help="The URL/ID/Name of the file to download.",
-    ),
-    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
-    ):
-    initHistory(silent = not debug)
-    if param.startswith("http"):
-        url = param
-    elif re.match(r"^[a-zA-Z0-9]+$", param):
-        url = f"http://{PROVIDER_NAME}/{param}"
-    else:
-        jhistory = json.loads(history.read_text())
-        url = next((x["url"] for x in jhistory if x["id"] == param or x["name"] == param), None)
-        if not url:
-            console.print(f"Could not find {param} in history", style="bold red")
-            return
-        
-    console.print(download(url))
-    
-@app.command("rmh", help="Clear the history of uploaded files.")
-def rm_history():
-    resetHistory()
-    console.print("History cleared.", style="bold green")
-
-@app.command("x", help="Export the history of uploaded files.")
-def export_history(
-    nlines: int = typer.Option(None, "--num-lines", "-n", help="Number of past lines to export."),
-    ):
-    if not HISTORY_PATH.exists():
-        console.print("No history found.", style="bold red")
-        return
-    jhistory = json.loads(HISTORY_PATH.read_text())
-    export = jhistory[-nlines:] if nlines else jhistory
-    console.print(json.dumps(windowsDictRepair(jhistory), indent=4))
-
-@app.command("xl", help="Export last line of the history of uploaded files.")
-def export_last_history():
-    if not HISTORY_PATH.exists():
-        console.print("No history found.", style="bold red")
-        return
-    jhistory = json.loads(HISTORY_PATH.read_text())
-    console.print(json.dumps(windowsDictRepair(jhistory[-1]), indent=4))
-
-    
-############################################
-##### Aliases for the commands above #######
-############################################
-
-@app.command("file", hidden=True)
-def file_alias(
-    filepath: Path = typer.Argument(
-        ...,
-        help="The path to the file to upload.", 
-        exists=True,
-        file_okay=True,
-        dir_okay=False,
-        readable=True
-        ),
-    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode.")
-):
-    from_file(filepath, debug)
-
-@app.command("stdin", hidden=True)
-def stdin_alias(
-    param: str = typer.Argument(None, help=f"sdtin input to upload to {PROVIDER_NAME}, defaults to sys.argv"),
-    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
-):
-    from_stdin(param, debug)
-
-@app.command("hist", hidden=True)
-def hist_alias():
-    history()
-
-@app.command("get", hidden=True)
-def get_alias(
-    param: str = typer.Argument(
-        ...,
-        help="The URL/ID/Name of the file to download.",
-    ),
-    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
-):
+import typer
+import rich
+import json
+import sys
+import re
+
+from pathlib import Path
+from rich.table import Table
+
+from .utils import (
+    uploadFromFile,
+    uploadFromStdin,
+    download,
+    initHistory,
+    resetHistory,
+    console,
+    windowsDictRepair,
+    HISTORY_PATH,
+    PROVIDER_URL
+)
+
+PROVIDER_NAME = PROVIDER_URL.split("//")[-1]
+
+app = typer.Typer(
+    name="ix",
+    help=f"A CLI for interacting with the {PROVIDER_NAME} pastebin service.",
+    no_args_is_help=True,
+    rich_help_panel="rich",
+    rich_markup_mode="rich",
+)
+
+@app.command(
+    "f",
+    help=f"Upload a file to {PROVIDER_NAME}",
+    no_args_is_help=True,
+)
+def from_file(
+    filepath: Path = typer.Argument(
+        ...,
+        help="The path to the file to upload.", 
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True
+        ),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode.")
+    ):
+    initHistory(silent = not debug)
+    console.print(uploadFromFile(filepath))
+    
+@app.command(
+    "s",
+    help=f"Upload stdin to {PROVIDER_NAME}",
+    no_args_is_help=False,
+)
+def from_stdin(
+    param: str = typer.Argument(None, help=f"sdtin input to upload to {PROVIDER_NAME}, defaults to sys.argv"),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
+):
+    param = ' '.join(sys.argv[2:])
+    param = param if param.strip() else None
+    initHistory(silent = not debug)
+    if response := uploadFromStdin(param):
+        console.print(response)
+    
+@app.command("h", help="Show the history of uploaded files.")
+def history():
+    if not HISTORY_PATH.exists():
+        console.print("No history found.", style="bold red")
+        return
+    jhistory = json.loads(HISTORY_PATH.read_text())
+    table = Table(show_header=True, header_style="bold magenta")
+    
+    table.add_column("ID", style="bold red", width=12)
+    table.add_column("Content-Start", style="bold yellow", justify="center")
+    table.add_column("Url", style="bold cyan", justify="center")
+    
+    for x in jhistory:
+        table.add_row(x["id"], x["name"], x["url"])
+        
+    console.print(table)
+    
+    
+@app.command(
+    "g",
+    help=f"Download a file from {PROVIDER_NAME}",
+    no_args_is_help=True,
+)
+def get(
+    param: str = typer.Argument(
+        ...,
+        help="The URL/ID/Name of the file to download.",
+    ),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
+    ):
+    initHistory(silent = not debug)
+    if param.startswith("http"):
+        url = param
+    elif re.match(r"^[a-zA-Z0-9]+$", param):
+        url = f"http://{PROVIDER_NAME}/{param}"
+    else:
+        jhistory = json.loads(history.read_text())
+        url = next((x["url"] for x in jhistory if x["id"] == param or x["name"] == param), None)
+        if not url:
+            console.print(f"Could not find {param} in history", style="bold red")
+            return
+        
+    console.print(download(url))
+    
+@app.command("rmh", help="Clear the history of uploaded files.")
+def rm_history():
+    resetHistory()
+    console.print("History cleared.", style="bold green")
+
+@app.command("x", help="Export the history of uploaded files.")
+def export_history(
+    nlines: int = typer.Option(None, "--num-lines", "-n", help="Number of past lines to export."),
+    ):
+    if not HISTORY_PATH.exists():
+        console.print("No history found.", style="bold red")
+        return
+    jhistory = json.loads(HISTORY_PATH.read_text())
+    export = jhistory[-nlines:] if nlines else jhistory
+    console.print(json.dumps(windowsDictRepair(jhistory), indent=4))
+
+@app.command("xl", help="Export last line of the history of uploaded files.")
+def export_last_history():
+    if not HISTORY_PATH.exists():
+        console.print("No history found.", style="bold red")
+        return
+    jhistory = json.loads(HISTORY_PATH.read_text())
+    console.print(json.dumps(windowsDictRepair(jhistory[-1]), indent=4))
+
+    
+############################################
+##### Aliases for the commands above #######
+############################################
+
+@app.command("file", hidden=True)
+def file_alias(
+    filepath: Path = typer.Argument(
+        ...,
+        help="The path to the file to upload.", 
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True
+        ),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode.")
+):
+    from_file(filepath, debug)
+
+@app.command("stdin", hidden=True)
+def stdin_alias(
+    param: str = typer.Argument(None, help=f"sdtin input to upload to {PROVIDER_NAME}, defaults to sys.argv"),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
+):
+    from_stdin(param, debug)
+
+@app.command("hist", hidden=True)
+def hist_alias():
+    history()
+
+@app.command("get", hidden=True)
+def get_alias(
+    param: str = typer.Argument(
+        ...,
+        help="The URL/ID/Name of the file to download.",
+    ),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug mode."),
+):
     get(param, debug)
```

### Comparing `ix_cli-0.1.2/ix_cli/utils.py` & `ix_cli-0.1.3/ix_cli/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import os
-import re
-import sys
-import json
-import rich
-import requests
-from pathlib import Path
-from rich.console import Console
-from rich.progress import (
-    Progress, SpinnerColumn, TextColumn, TimeElapsedColumn
-    )
-from copy import deepcopy
-from typing import Union
-
-__all__ = [
-    "uploadFromFile",
-    "uploadFromStdin",
-    "download",
-    "initHistory",
-    "HISTORY_PATH",
-    "resetHistory",
-    "PROVIDER_URL",
-    "console",
-    "sanitize",
-    ]
-
-Pbar = Progress(
-    SpinnerColumn(),
-    "●",
-    TextColumn("[bold cyan]Sanitizing data[/bold cyan] [bold magenta](Windows only)[/bold magenta]", justify="right"),
-    "●",
-    TimeElapsedColumn(),
-)
-
-console = Console()
-
-PROVIDER_URL = "http://ix.io"
-
-HISTORY_PATH = Path().home() / ".ix" / "history.json"
-
-def initHistory(silent: bool = True):
-    try:
-        HISTORY_PATH.parent.mkdir(parents=True, exist_ok=True)
-        if not HISTORY_PATH.exists():
-            HISTORY_PATH.write_text("[]")
-    except OSError:
-        if not silent:
-            console.print(f"Could not create history file at {HISTORY_PATH}", style="bold red")
-
-def resetHistory():
-    HISTORY_PATH.unlink()
-    initHistory()
-
-def updateHistory(response, src: Union[Path,str], nlines: int = 100):
-    if not HISTORY_PATH.exists():
-        return
-    jhistory = json.loads(HISTORY_PATH.read_text())
-    jhistory.append({
-        "url": response.text,
-        "id": response.text.split("/")[-1],
-        "name": src.name if isinstance(src, Path) else src[:min(15, src.find(" "))],
-        })
-    if len(jhistory) > nlines:
-        jhistory = jhistory[-nlines:]
-    HISTORY_PATH.write_text(json.dumps(jhistory, indent=4))
-
-def uploadFromFile(filepath: Path) -> str:
-    """Uploads a file to ix.io and returns the URL."""
-    files = {"f:1": open(filepath, "rb")}
-    response = requests.post(PROVIDER_URL, files=files)
-    if response.status_code == 200:
-        updateHistory(response, filepath.name)
-    return response.text
-
-def pipeInput() -> str:
-    """Returns the piped input if any."""
-    return "".join(sys.argv[1:]).replace("s", "") if sys.stdin.isatty() else sys.stdin.buffer.read().decode("utf-8")
-
-def uploadFromStdin(param: str = None) -> str:
-    """Uploads stdin to ix.io and returns the URL."""
-    data = param or pipeInput()
-    sys.stdin.close()
-    if '{' in data and sys.platform == 'win32':
-        with Pbar as pbar:
-            task = pbar.add_task("Data Sanitization", total=1)
-            data = sanitize(data)
-            pbar.update(task, description="[bold green]Done[/bold green]", completed=True)
-        
-    if not data:
-        console.print("[bold red]No data found in stdin.[/bold red]")
-        console.print("[bold yellow]Usage:[/bold yellow]")
-        console.print(" -  ix s <data>")
-        console.print(" -  echo <data> | ix s")
-        console.print(" -  cat <file>  | ix s")
-        return
-    response = requests.post(PROVIDER_URL, data={"f:1": data})
-    if response.status_code == 200:
-        updateHistory(response, f"stdin:{data[:5]}")
-    return response.text
-
-def download(url: str) -> str:
-    """Downloads a file from ix.io and returns the contents."""
-    url = url.strip()
-    response = requests.get(url)
-    return response.text
-
-def winIterKeys(subparam: str):
-    for item in subparam.split(","):
-        key, value = item.split(":")
-        key = key.lstrip()
-        if '[' in value:
-            for lv in value[1:-1].split("@lsep@"):
-                new_value = value.replace(lv, f'"{lv}"')
-        else:
-            new_value = value
-        kvstr = f'"{key}":"{new_value}"'
-        subparam = subparam.replace(item, kvstr)
-    return subparam
-
-def subDictFix(subparam: str):
-    
-    nextdict = subparam.find("{")
-    subparam = subparam[:nextdict]
-    return winIterKeys(subparam)
-
-def sanitize(param: str):
-    try:
-        return windowsDictRepair(param)
-    except Exception as e:
-        return param
-
-def windowsDictRepair(param: str):
-    if not param:
-        return param
-    chars = ['{', '}', ":"]
-    if any(x not in param for x in chars):
-        return param
-    param = param[1:-1]
-    for listvar in re.findall(r'\[(.*)\]', param):
-        param = param.replace(listvar, listvar.replace(",", "@lsep@"))
-
-    non_nested = deepcopy(param)
-    for dictvar in re.findall(r'\{(.*)\}', param):
-        param = param.replace(dictvar, subDictFix(dictvar))
-        non_nested = non_nested.replace(dictvar, '')
-    non_nested = non_nested.replace("{", "").replace("}", "")
-    param = param.replace(non_nested, winIterKeys(non_nested))
-    param = param.replace(':""', ':')
-    param = param.replace("@lsep@", ",")
-    return '{' + param + '}'
+import os
+import re
+import sys
+import json
+import rich
+import requests
+from pathlib import Path
+from rich.console import Console
+from rich.progress import (
+    Progress, SpinnerColumn, TextColumn, TimeElapsedColumn
+    )
+from copy import deepcopy
+from typing import Union
+
+__all__ = [
+    "uploadFromFile",
+    "uploadFromStdin",
+    "download",
+    "initHistory",
+    "HISTORY_PATH",
+    "resetHistory",
+    "PROVIDER_URL",
+    "console",
+    "sanitize",
+    ]
+
+Pbar = Progress(
+    SpinnerColumn(),
+    "●",
+    TextColumn("[bold cyan]Sanitizing data[/bold cyan] [bold magenta](Windows only)[/bold magenta]", justify="right"),
+    "●",
+    TimeElapsedColumn(),
+)
+
+console = Console()
+
+PROVIDER_URL = "http://ix.io"
+
+HISTORY_PATH = Path().home() / ".ix" / "history.json"
+
+def initHistory(silent: bool = True):
+    try:
+        HISTORY_PATH.parent.mkdir(parents=True, exist_ok=True)
+        if not HISTORY_PATH.exists():
+            HISTORY_PATH.write_text("[]")
+    except OSError:
+        if not silent:
+            console.print(f"Could not create history file at {HISTORY_PATH}", style="bold red")
+
+def resetHistory():
+    HISTORY_PATH.unlink()
+    initHistory()
+
+def updateHistory(response, src: Union[Path,str], nlines: int = 100):
+    if not HISTORY_PATH.exists():
+        return
+    jhistory = json.loads(HISTORY_PATH.read_text())
+    jhistory.append({
+        "url": response.text,
+        "id": response.text.split("/")[-1],
+        "name": src.name if isinstance(src, Path) else src[:min(15, src.find(" "))],
+        })
+    if len(jhistory) > nlines:
+        jhistory = jhistory[-nlines:]
+    HISTORY_PATH.write_text(json.dumps(jhistory, indent=4))
+
+def uploadFromFile(filepath: Path) -> str:
+    """Uploads a file to ix.io and returns the URL."""
+    files = {"f:1": open(filepath, "rb")}
+    response = requests.post(PROVIDER_URL, files=files)
+    if response.status_code == 200:
+        updateHistory(response, filepath.name)
+    return response.text
+
+def pipeInput() -> str:
+    """Returns the piped input if any."""
+    return "".join(sys.argv[1:]).replace("s", "") if sys.stdin.isatty() else sys.stdin.buffer.read().decode("utf-8")
+
+def uploadFromStdin(param: str = None) -> str:
+    """Uploads stdin to ix.io and returns the URL."""
+    data = param or pipeInput()
+    sys.stdin.close()
+    if '{' in data and sys.platform == 'win32':
+        with Pbar as pbar:
+            task = pbar.add_task("Data Sanitization", total=1)
+            data = sanitize(data)
+            pbar.update(task, description="[bold green]Done[/bold green]", completed=True)
+        
+    if not data:
+        console.print("[bold red]No data found in stdin.[/bold red]")
+        console.print("[bold yellow]Usage:[/bold yellow]")
+        console.print(" -  ix s <data>")
+        console.print(" -  echo <data> | ix s")
+        console.print(" -  cat <file>  | ix s")
+        return
+    response = requests.post(PROVIDER_URL, data={"f:1": data})
+    if response.status_code == 200:
+        updateHistory(response, f"stdin:{data[:5]}")
+    return response.text
+
+def download(url: str) -> str:
+    """Downloads a file from ix.io and returns the contents."""
+    url = url.strip()
+    response = requests.get(url)
+    return response.text
+
+def winIterKeys(subparam: str):
+    for item in subparam.split(","):
+        key, value = item.split(":")
+        key = key.lstrip()
+        if '[' in value:
+            for lv in value[1:-1].split("@lsep@"):
+                new_value = value.replace(lv, f'"{lv}"')
+        else:
+            new_value = value
+        kvstr = f'"{key}":"{new_value}"'
+        subparam = subparam.replace(item, kvstr)
+    return subparam
+
+def subDictFix(subparam: str):
+    
+    nextdict = subparam.find("{")
+    subparam = subparam[:nextdict]
+    return winIterKeys(subparam)
+
+def sanitize(param: str):
+    try:
+        return windowsDictRepair(param)
+    except Exception as e:
+        return param
+
+def windowsDictRepair(param: str):
+    if not param:
+        return param
+    chars = ['{', '}', ":"]
+    if any(x not in param for x in chars):
+        return param
+    param = param[1:-1]
+    for listvar in re.findall(r'\[(.*)\]', param):
+        param = param.replace(listvar, listvar.replace(",", "@lsep@"))
+
+    non_nested = deepcopy(param)
+    for dictvar in re.findall(r'\{(.*)\}', param):
+        param = param.replace(dictvar, subDictFix(dictvar))
+        non_nested = non_nested.replace(dictvar, '')
+    non_nested = non_nested.replace("{", "").replace("}", "")
+    param = param.replace(non_nested, winIterKeys(non_nested))
+    param = param.replace(':""', ':')
+    param = param.replace("@lsep@", ",")
+    return '{' + param + '}'
```

### Comparing `ix_cli-0.1.2/LICENSE` & `ix_cli-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 Arno Veletanlic
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2023 Arno Veletanlic
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `ix_cli-0.1.2/README.md` & `ix_cli-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,99 +1,107 @@
-# A rich CLI template for pastebin CLI tools
-
-ix is a command line interface for [ix.io](https://ix.io), a pastebin service.
-
-I tried to make this CLI as "reusable" as possible, so that you can clone this repository and use it as a template for your own pastebin CLI tool.
-
-## How to use this template
-
-1. Clone this repository
-2. Rename the `ix_cli` directory to the name of your pastebin service
-3. Replace the variable `PROVIDER_URL` in `ix_cli/utils.py` with the URL of your pastebin service (e.g. `https://paste.example.com`)
-4. Replace the name of the app in `pyproject.toml` with the name of your pastebin service in both the `name` and `[tool.poetry.scripts]` sections
-5. Install [poetry](https://python-poetry.org) and run `poetry install` to install the dependencies
-6. Run a basic command to make sure everything works: `<new-app-name> s "Hello, world!"`
-7. Edit the README to your liking
-8. Commit your changes and push them to your repository
-9. Publish your app to [PyPI](https://pypi.org) using `poetry build` and `poetry publish`
-
-## Installation
-
-### Using pip
-
-```bash
-pip install ix-cli
-```
-
-### Cloning the repository
-
-```bash
-git clone https://github.com/arnos-stuff/ix.git
-```
-
-## Basic usage
-
-### As a Python module
-
-```python
-from ix_cli import uploadFromFile, uploadFromStdin, download, getHistory
-
-# Upload from stdin
-url = uploadFromStdin("Hello, world!")
-print(url)
-
-# Upload from file
-url = uploadFromFile("README.md")
-print(url)
-
-# Download
-data = download(url)
-print(data)
-```
-
-### As a CLI tool
-
-Using ix is simple. Just pipe some text into it:
-
-```bash
-echo "Hello, world!" | ix s
-```
-
-This will print the URL of the paste to stdout. You can also use ix to upload files:
-
-```bash
-ix f README.md
-```
-
-This CLI has an extra feature: it stores the past 100 URLs in a local cache. You can use this to quickly access your pastes:
-
-```bash
-ix h
-```
-
-This will print a list of your pastes, with the most recent at the top. You also have the option to limit the number of pastes shown:
-
-```bash
-ix h -n 3
-```
-
-This will print the 3 most recent pastes.
-
-## Getting the data back
-
-You can use ix to retrieve the data from a paste by using the `g` command:
-
-```bash
-ix g https://ix.io/1QZp
-```
-
-or simply
-
-```bash
-ix g 1QZp
-```
-
-This will print the contents of the paste to stdout.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+---
+title: xi-cli
+description: A rich CLI template for pastebin CLI tools
+pypi_url: https://pypi.org/project/ix-cli/#files
+tar_url: https://pypi.org/project/ix-cli/#files
+github_url: https://github.com/arnos-stuff/ix
+---
+
+# A rich CLI template for pastebin CLI tools
+
+ix is a command line interface for [ix.io](https://ix.io), a pastebin service.
+
+I tried to make this CLI as "reusable" as possible, so that you can clone this repository and use it as a template for your own pastebin CLI tool.
+
+## How to use this template
+
+1. Clone this repository
+2. Rename the `ix_cli` directory to the name of your pastebin service
+3. Replace the variable `PROVIDER_URL` in `ix_cli/utils.py` with the URL of your pastebin service (e.g. `https://paste.example.com`)
+4. Replace the name of the app in `pyproject.toml` with the name of your pastebin service in both the `name` and `[tool.poetry.scripts]` sections
+5. Install [poetry](https://python-poetry.org) and run `poetry install` to install the dependencies
+6. Run a basic command to make sure everything works: `<new-app-name> s "Hello, world!"`
+7. Edit the README to your liking
+8. Commit your changes and push them to your repository
+9. Publish your app to [PyPI](https://pypi.org) using `poetry build` and `poetry publish`
+
+## Installation
+
+### Using pip
+
+```bash
+pip install ix-cli
+```
+
+### Cloning the repository
+
+```bash
+git clone https://github.com/arnos-stuff/ix.git
+```
+
+## Basic usage
+
+### As a Python module
+
+```python
+from ix_cli import uploadFromFile, uploadFromStdin, download, getHistory
+
+# Upload from stdin
+url = uploadFromStdin("Hello, world!")
+print(url)
+
+# Upload from file
+url = uploadFromFile("README.md")
+print(url)
+
+# Download
+data = download(url)
+print(data)
+```
+
+### As a CLI tool
+
+Using ix is simple. Just pipe some text into it:
+
+```bash
+echo "Hello, world!" | ix s
+```
+
+This will print the URL of the paste to stdout. You can also use ix to upload files:
+
+```bash
+ix f README.md
+```
+
+This CLI has an extra feature: it stores the past 100 URLs in a local cache. You can use this to quickly access your pastes:
+
+```bash
+ix h
+```
+
+This will print a list of your pastes, with the most recent at the top. You also have the option to limit the number of pastes shown:
+
+```bash
+ix h -n 3
+```
+
+This will print the 3 most recent pastes.
+
+## Getting the data back
+
+You can use ix to retrieve the data from a paste by using the `g` command:
+
+```bash
+ix g https://ix.io/1QZp
+```
+
+or simply
+
+```bash
+ix g 1QZp
+```
+
+This will print the contents of the paste to stdout.
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
```

### Comparing `ix_cli-0.1.2/PKG-INFO` & `ix_cli-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: ix-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/arnos-stuff/ix
 License: MIT
 Author: arnos-stuff
 Author-email: bcda0276@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0) ; python_version < "3.11"
+Requires-Dist: typer[all] (>=0.9.0) ; python_version >= "3.11"
 Description-Content-Type: text/markdown
 
+---
+title: xi-cli
+description: A rich CLI template for pastebin CLI tools
+pypi_url: https://pypi.org/project/ix-cli/#files
+tar_url: https://pypi.org/project/ix-cli/#files
+github_url: https://github.com/arnos-stuff/ix
+---
+
 # A rich CLI template for pastebin CLI tools
 
 ix is a command line interface for [ix.io](https://ix.io), a pastebin service.
 
 I tried to make this CLI as "reusable" as possible, so that you can clone this repository and use it as a template for your own pastebin CLI tool.
 
 ## How to use this template
```

