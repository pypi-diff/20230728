# Comparing `tmp/argdeco-josugoar-1.4.0.tar.gz` & `tmp/argdeco-josugoar-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argdeco-josugoar-1.4.0.tar", last modified: Mon Mar 29 15:13:08 2021, max compression
+gzip compressed data, was "argdeco-josugoar-1.6.0.tar", last modified: Fri Jul 28 09:48:06 2023, max compression
```

## Comparing `argdeco-josugoar-1.4.0.tar` & `argdeco-josugoar-1.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-03-29 15:13:08.051389 argdeco-josugoar-1.4.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14504 2021-03-29 15:13:08.050389 argdeco-josugoar-1.4.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11264 2021-02-15 13:16:19.000000 argdeco-josugoar-1.4.0/README.md
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3160 2021-03-24 16:49:13.000000 argdeco-josugoar-1.4.0/argdeco.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2021-03-29 15:13:08.050389 argdeco-josugoar-1.4.0/argdeco_josugoar.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14504 2021-03-29 15:13:06.000000 argdeco-josugoar-1.4.0/argdeco_josugoar.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      228 2021-03-29 15:13:07.000000 argdeco-josugoar-1.4.0/argdeco_josugoar.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2021-03-29 15:13:06.000000 argdeco-josugoar-1.4.0/argdeco_josugoar.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2021-03-29 15:13:06.000000 argdeco-josugoar-1.4.0/argdeco_josugoar.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2021-03-29 15:13:06.000000 argdeco-josugoar-1.4.0/argdeco_josugoar.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2021-03-29 15:13:08.051389 argdeco-josugoar-1.4.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1100 2021-03-29 15:08:43.000000 argdeco-josugoar-1.4.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 09:48:06.377918 argdeco-josugoar-1.6.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1065 2023-07-27 13:09:39.000000 argdeco-josugoar-1.6.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12457 2023-07-28 09:48:06.377918 argdeco-josugoar-1.6.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11564 2023-07-28 09:46:36.000000 argdeco-josugoar-1.6.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6377 2023-07-28 09:46:45.000000 argdeco-josugoar-1.6.0/argdeco.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-28 09:48:06.376918 argdeco-josugoar-1.6.0/argdeco_josugoar.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12457 2023-07-28 09:48:06.000000 argdeco-josugoar-1.6.0/argdeco_josugoar.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      197 2023-07-28 09:48:06.000000 argdeco-josugoar-1.6.0/argdeco_josugoar.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-28 09:48:06.000000 argdeco-josugoar-1.6.0/argdeco_josugoar.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-07-28 09:48:06.000000 argdeco-josugoar-1.6.0/argdeco_josugoar.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-28 09:48:06.377918 argdeco-josugoar-1.6.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1205 2023-07-28 09:46:58.000000 argdeco-josugoar-1.6.0/setup.py
```

### Comparing `argdeco-josugoar-1.4.0/PKG-INFO` & `argdeco-josugoar-1.6.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,325 +1,350 @@
 Metadata-Version: 2.1
 Name: argdeco-josugoar
-Version: 1.4.0
-Summary: Unopinionated argparse wrapper
+Version: 1.6.0
+Summary: Opinionated argparse wrapper
 Home-page: https://github.com/josugoar/argdeco
+Download-URL: https://github.com/josugoar/argdeco/archive/v1.6.0.tar.gz
 Author: josugoar
 License: MIT
-Download-URL: https://github.com/josugoar/argdeco/archive/v1.4.0.tar.gz
 Project-URL: Source, https://github.com/josugoar/argdeco
-Description: <p align="center">
-          <img src="assets/argdeco.png" alt="argdeco" width="640" height="320" />
-        </p>
-        
-        <h1></h1>
-        
-        > Unopinionated **argparse** wrapper
-        
-        * The EXACT same decorating order as regular **argparse** MUST be respected
-        
-        * It is recommended to install the development version directly from the repository
-        
-        # Why argdeco?
-        
-        There are so many libraries out there for writing command line utilities; why does **argdeco** exist?
-        
-        This question is easy to answer: because there is not a single command line utility for Python out there which ticks the following boxes: ([sound familiar?](https://click.palletsprojects.com/en/7.x/why/))
-        
-        * supports class callback method decoration and method instance binding with class instance forwarding (thank you [Graham Dumpleton](https://github.com/GrahamDumpleton) for [wrapt](https://github.com/GrahamDumpleton/wrapt)!)
-        
-        * supports callback callable instance binding with **argparse** context or parser instance forwarding
-        
-        * shares the EXACT same API as **argparse** using decorators
-        
-        # Installation
-        
-        You can get the library directly from PyPI:
-        
-        ```sh
-        $ pip install argdeco-JoshGoA
-        ```
-        
-        The installation into a [virtualenv](https://github.com/pypa/virtualenv) (or [pipenv](https://github.com/pypa/pipenv)) is heavily recommended.
-        
-        # API reference
-        
-        * **argdeco.argument_parser**(wrapped=None, parser_class=argparse.ArgumentParser, ctx=False, prog=None, usage=None, description=None, epilog=None, parents=[], formatter_class=argparse.HelpFormatter, prefix_chars="-", fromfile_prefix_chars=None, argument_default=None, conflict_handler="error", add_help=True, allow_abbrev=True)
-        
-          * Create a new ArgumentParser object. All parameters should be passed as keyword arguments. Each parameter has its own more detailed description below, but in short they are:
-        
-              * wrapped - The callback callable (default: None)
-        
-              * parser_class - The class to instantiate the parser (default: argparse.ArgumentParser)
-        
-              * ctx - Pass the **argparse** context or parser instance to the callback callable (default: False)
-        
-              * prog - The name of the program (default: sys.argv[0])
-        
-              * usage - The string describing the program usage (default: generated from arguments added to parser)
-        
-              * description - Text to display before the argument help (default: __doc__)
-        
-              * epilog - Text to display after the argument help (default: none)
-        
-              * parents - A list of ArgumentParser objects whose arguments should also be included
-        
-              * formatter_class - A class for customizing the help output
-        
-              * prefix_chars - The set of characters that prefix optional arguments (default: "-")
-        
-              * fromfile_prefix_chars - The set of characters that prefix files from which additional arguments should be read (default: None)
-        
-              * argument_default - The global default value for arguments (default: None)
-        
-              * conflict_handler - The strategy for resolving conflicting optionals (usually unnecessary)
-        
-              * add_help - Add a -h/--help option to the parser (default: True)
-        
-              * allow_abbrev - Allows long options to be abbreviated if the abbreviation is unambiguous. (default: True)
-        
-        ```py
-        >>> import argdeco
-        >>> @argdeco.add_argument("--foo", help="foo help")
-        ... @argdeco.argument_parser
-        ... def parser(foo):
-        ...     pass
-        ...
-        ```
-        
-        ```py
-        >>> parser(["--help"])
-        usage: myprogram.py [-h] [--foo FOO]
-        
-        optional arguments:
-         -h, --help  show this help message and exit
-         --foo FOO   foo help
-        ```
-        
-        * **argdeco.add_argument**(name or flags..., group=None, [, action][, nargs][, const][, default][, type][, choices][, required][, help][, metavar][, dest])
-        
-          * Define how a single command-line argument should be parsed. Each parameter has its own more detailed description below, but in short they are:
-        
-            * name or flags - Either a name or a list of option strings, e.g. foo or -f, --foo.
-        
-            * group - The group to add the argument. (default: None)
-        
-            * action - The basic type of action to be taken when this argument is encountered at the command line.
-        
-            * nargs - The number of command-line arguments that should be consumed.
-        
-            * const - A constant value required by some action and nargs selections.
-        
-            * default - The value produced if the argument is absent from the command line.
-        
-            * type - The type to which the command-line argument should be converted.
-        
-            * choices - A container of the allowable values for the argument.
-        
-            * required - Whether or not the command-line option may be omitted (optionals only).
-        
-            * help - A brief description of what the argument does.
-        
-            * metavar - A name for the argument in usage messages.
-        
-            * dest - The name of the attribute to be added to the object returned by parse_args().
-        
-        * **argdeco.add_subparsers**(wrapped=None, [title][, description][, prog][, parser_class][, action][, option_string][, dest][, required][, help][, metavar])
-        
-          * Many programs split up their functionality into a number of sub-commands, for example, the svn program can invoke sub-commands like svn checkout, svn update, and svn commit. Splitting up functionality this way can be a particularly good idea when a program performs several different functions which require different kinds of command-line arguments. ArgumentParser supports the creation of such sub-commands with the add_subparsers() method. The add_subparsers() method is normally called with no arguments and returns a special action object. This object has a single method, add_parser(), which takes a command name and any ArgumentParser constructor arguments, and returns an ArgumentParser object that can be modified as usual.
-        
-          * Description of parameters:
-        
-            * wrapped - The callback callable (default: None)
-        
-            * title - title for the sub-parser group in help output; by default “subcommands” if description is provided, otherwise uses title for positional arguments
-        
-            * description - description for the sub-parser group in help output, by default None
-        
-            * prog - usage information that will be displayed with sub-command help, by default the name of the program and any positional arguments before the subparser argument
-        
-            * parser_class - class which will be used to create sub-parser instances, by default the class of the current parser (e.g. ArgumentParser)
-        
-            * action - the basic type of action to be taken when this argument is encountered at the command line
-        
-            * dest - name of the attribute under which sub-command name will be stored; by default None and no value is stored
-        
-            * required - Whether or not a subcommand must be provided, by default False (added in 3.7)
-        
-            * help - help for sub-parser group in help output, by default None
-        
-            * metavar - string presenting available sub-commands in help; by default it is None and presents sub-commands in form {cmd1, cmd2, ..}
-        
-        ```py
-        >>> # create the top-level parser
-        >>> @argdeco.add_subparsers(help="sub-command help")
-        ... @argdeco.add_argument("--foo", action="store_true", help="foo help")
-        ... @argdeco.argument_parser(prog="PROG")
-        ... def parser(**kwargs):
-        ...     print("parser")
-        ...     print(kwargs)
-        ...
-        ```
-        
-        ```py
-        >>> # create the parser for the "a" command
-        >>> @argdeco.add_argument("bar", type=int, help="bar help")
-        ... @argdeco.add_parser(parser, "a", help="a help")
-        ... def parser_a(**kwargs):
-        ...     print("parser_a")
-        ...     print(kwargs)
-        ...
-        ```
-        
-        ```py
-        >>> # create the parser for the "a" command
-        >>> @argdeco.add_argument("--baz", choices="XYZ", help="baz help")
-        ... @argdeco.add_parser(parser, "b", help="b help")
-        ... def parser_b(**kwargs):
-        ...     print("parser_b")
-        ...     print(kwargs)
-        ...
-        ```
-        
-        ```py
-        >>> # parse some argument lists
-        >>> parser(["a", "12"])
-        parser_a
-        {"foo": False, "bar": 12}
-        >>> parser(["--foo", "b", "--baz", "Z"])
-        parser_b
-        {"foo": True, "baz": "Z"}
-        ```
-        
-        * **argdeco.add_argument_group**(title=None, description=None)
-        
-          * By default, ArgumentParser groups command-line arguments into “positional arguments” and “optional arguments” when displaying help messages. When there is a better conceptual grouping of arguments than this default one, appropriate groups can be created using the add_argument_group() method:
-        
-        ```py
-        >>> @argdeco.add_argument("bar", group="group", help="bar help")
-        ... @argdeco.add_argument("--foo", group="group", help="foo help")
-        ... @argdeco.add_argument_group("group")
-        ... @argdeco.argument_parser(prog="PROG", add_help=False)
-        ... def parser(**kwargs):
-        ...     pass
-        ...
-        >>> parser.print_help()
-        usage: PROG [--foo FOO] bar
-        
-        group:
-          bar    bar help
-          --foo FOO  foo help
-        ```
-        
-        * **ardeco.add_mutually_exclusive_group**(required=False)
-        
-        ```py
-        >>> @argdeco.add_argument("--bar", group="group", action="store_false")
-        ... @argdeco.add_argument("--foo", group="group", action="store_true")
-        ... @argdeco.add_mutually_exclusive_group("group")
-        ... @argdeco.argument_parser(prog="PROG")
-        ... def parser(**kwargs):
-        ...     print(kwargs)
-        ...
-        >>> parser(["--foo"])
-        {"foo": True, "bar": True}
-        >>> parser(["--bar"])
-        {"foo": False, "bar": False}
-        >>> parser(["--foo", "--bar"])
-        usage: PROG [-h] [--foo | --bar]
-        PROG: error: argument --bar: not allowed with argument --foo
-        ```
-        
-        # Advanced usage
-        
-        ## Accessing attributes
-        
-        **argdeco** does NOT override decorated functions so that they can be accessed by the user easily if needed. In order to access the **argparse** context or parser instance, it is recommended to use context forwarding.
-        
-        ```py
-        >>> @argdeco.argument_parser
-        ... def prog(self):
-        ...     pass
-        ...
-        >>> prog.__wrapped__
-        <function prog at 0x0000029BCBFABF70>
-        >>> prog.parser
-        ArgumentParser(prog="argdeco.py", usage=None, description=None, formatter_class=<class "argparse.HelpFormatter">, conflict_handler="error", add_help=True)
-        ```
-        
-        ## Class method decoration
-        
-        **argdeco** supports class callback method decoration, unlike the big majority of CLI decorator libraries, without any difference as regular callback callable decoration.
-        
-        ```py
-        >>> class Prog:
-        ...
-        ...     @argdeco.argument_parser
-        ...     def parser(self):
-        ...         pass
-        ...
-        ```
-        
-        Decorating a class will forward the arguments to the *\_\_init__* method (usually not the desired behaviour), as decorated callbacks will ALWAYS be treated as callables.
-        
-        ```py
-        >>> @argdeco.argument_parser
-        ... class Prog:
-        ...     pass
-        ...
-        ```
-        
-        Decorating the *\_\_call__* method will forward the arguments to the class itself, following standard decorator usage as specified by [wrapt](https://wrapt.readthedocs.io/en/latest/decorators.html#decorating-class-methods).
-        
-        ```py
-        >>> class Prog:
-        ...
-        ...     @argdeco.argument_parser
-        ...     def __call__(self):
-        ...         pass
-        ...
-        ```
-        
-        ## Context forwarding
-        
-        Decorated callback callables can get access to the **argparse** context or parser instance.
-        
-        ```py
-        >>> @argdeco.argument_parser(ctx=True, prog="PROG")
-        ... def parser(ctx):
-        ...     ctx.print_help()
-        ...
-        >>> parser([])
-        usage: PROG [-h]
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-        Class callback method context or parser instance forwarding is still respected on decorated class methods.
-        
-        ```py
-        >>> class Prog:
-        ...
-        ...     @argdeco.argument_parser(ctx=True, prog="PROG")
-        ...     def __call__(self, ctx):
-        ...         ctx.print_help()
-        ...
-        >>> prog = Prog()
-        >>> prog([])
-        usage: PROG [-h]
-        
-        optional arguments:
-          -h, --help  show this help message and exit
-        ```
-        
-Keywords: argparse cli library pipenv python wrapt
-Platform: UNKNOWN
+Keywords: argparse cli docker library python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <img src="assets/argdeco.png" alt="argdeco" width="640" height="320" />
+</p>
+
+<h1></h1>
+
+> Opinionated **argparse** wrapper
+
+* API breaking change in later versions due to major refactor!!
+
+* Follows the same decorating order as regular **argparse**
+
+* Recommended to install the development version directly from the repository
+
+# Why argdeco?
+
+There are so many libraries out there for writing command line utilities; why does **argdeco** exist?
+
+This question is easy to answer: because there is not a single command line utility for Python out there which ticks the following boxes: ([sound familiar?](https://click.palletsprojects.com/en/7.x/why/))
+
+* is fully typed using official **typeshed** **argparse** stubs
+
+* supports class callback method decoration and method instance binding with class instance forwarding
+
+* supports callback callable instance binding with **argparse** context or parser instance forwarding
+
+* shares the EXACT same API as **argparse** using decorators
+
+# Installation
+
+You can get the library directly from PyPI:
+
+```sh
+$ python -m pip install argdeco-josugoar
+```
+
+The installation into a [virtualenv](https://github.com/pypa/virtualenv) (or [pipenv](https://github.com/pypa/pipenv)) is heavily recommended.
+
+# API reference
+
+* **argdeco.argument_parser**(prog=None, usage=None, description=None, epilog=None, parents=[], formatter_class=argparse.HelpFormatter, prefix_chars="-", fromfile_prefix_chars=None, argument_default=None, conflict_handler="error", add_help=True, allow_abbrev=True, exit_on_error=True)
+
+  * Create a new ArgumentParser object. All parameters should be passed as keyword arguments. Each parameter has its own more detailed description below, but in short they are:
+
+      * prog - The name of the program (default: sys.argv[0])
+
+      * usage - The string describing the program usage (default: generated from arguments added to parser)
+
+      * description - Text to display before the argument help (default: __doc__)
+
+      * epilog - Text to display after the argument help (default: none)
+
+      * parents - A list of ArgumentParser objects whose arguments should also be included
+
+      * formatter_class - A class for customizing the help output
+
+      * prefix_chars - The set of characters that prefix optional arguments (default: "-")
+
+      * fromfile_prefix_chars - The set of characters that prefix files from which additional arguments should be read (default: None)
+
+      * argument_default - The global default value for arguments (default: None)
+
+      * conflict_handler - The strategy for resolving conflicting optionals (usually unnecessary)
+
+      * add_help - Add a -h/--help option to the parser (default: True)
+
+      * allow_abbrev - Allows long options to be abbreviated if the abbreviation is unambiguous. (default: True)
+
+      * exit_on_error - Determines whether or not ArgumentParser exits with error info when an error occurs. (default: True)
+
+```py
+>>> import argdeco
+>>> @argdeco.add_argument("--foo", help="foo help")
+... @argdeco.argument_parser()
+... def parser(foo):
+...     pass
+...
+```
+
+```py
+>>> parser(["--help"])
+usage: myprogram.py [-h] [--foo FOO]
+
+optional arguments:
+ -h, --help  show this help message and exit
+ --foo FOO   foo help
+```
+
+* **argdeco.add_argument**(name or flags..., group=None, [, action][, nargs][, const][, default][, type][, choices][, required][, help][, metavar][, dest])
+
+  * Define how a single command-line argument should be parsed. Each parameter has its own more detailed description below, but in short they are:
+
+    * name or flags - Either a name or a list of option strings, e.g. foo or -f, --foo.
+
+    * group - The group to add the argument. (default: None)
+
+    * action - The basic type of action to be taken when this argument is encountered at the command line.
+
+    * nargs - The number of command-line arguments that should be consumed.
+
+    * const - A constant value required by some action and nargs selections.
+
+    * default - The value produced if the argument is absent from the command line.
+
+    * type - The type to which the command-line argument should be converted.
+
+    * choices - A container of the allowable values for the argument.
+
+    * required - Whether or not the command-line option may be omitted (optionals only).
+
+    * help - A brief description of what the argument does.
+
+    * metavar - A name for the argument in usage messages.
+
+    * dest - The name of the attribute to be added to the object returned by parse_args().
+
+* **argdeco.add_subparsers**([title][, description][, prog][, parser_class][, action][, option_string][, dest][, required][, help][, metavar])
+
+  * Many programs split up their functionality into a number of sub-commands, for example, the svn program can invoke sub-commands like svn checkout, svn update, and svn commit. Splitting up functionality this way can be a particularly good idea when a program performs several different functions which require different kinds of command-line arguments. ArgumentParser supports the creation of such sub-commands with the add_subparsers() method. The add_subparsers() method is normally called with no arguments and returns a special action object. This object has a single method, add_parser(), which takes a command name and any ArgumentParser constructor arguments, and returns an ArgumentParser object that can be modified as usual.
+
+  * Description of parameters:
+
+    * title - title for the sub-parser group in help output; by default “subcommands” if description is provided, otherwise uses title for positional arguments
+
+    * description - description for the sub-parser group in help output, by default None
+
+    * prog - usage information that will be displayed with sub-command help, by default the name of the program and any positional arguments before the subparser argument
+
+    * parser_class - class which will be used to create sub-parser instances, by default the class of the current parser (e.g. ArgumentParser)
+
+    * action - the basic type of action to be taken when this argument is encountered at the command line
+
+    * dest - name of the attribute under which sub-command name will be stored; by default None and no value is stored
+
+    * required - Whether or not a subcommand must be provided, by default False (added in 3.7)
+
+    * help - help for sub-parser group in help output, by default None
+
+    * metavar - string presenting available sub-commands in help; by default it is None and presents sub-commands in form {cmd1, cmd2, ..}
+
+```py
+>>> # create the top-level parser
+>>> @argdeco.add_subparsers(help="sub-command help")
+... @argdeco.add_argument("--foo", action="store_true", help="foo help")
+... @argdeco.argument_parser(prog="PROG")
+... def parser(**kwargs):
+...     print("parser")
+...     print(kwargs)
+...
+```
+
+```py
+>>> # create the parser for the "a" command
+>>> @argdeco.add_argument("bar", type=int, help="bar help")
+... @argdeco.add_parser(parser, "a", help="a help")
+... def parser_a(**kwargs):
+...     print("parser_a")
+...     print(kwargs)
+...
+```
+
+```py
+>>> # create the parser for the "b" command
+>>> @argdeco.add_argument("--baz", choices="XYZ", help="baz help")
+... @argdeco.add_parser(parser, "b", help="b help")
+... def parser_b(**kwargs):
+...     print("parser_b")
+...     print(kwargs)
+...
+```
+
+```py
+>>> # parse some argument lists
+>>> parser(["a", "12"])
+parser_a
+{"foo": False, "bar": 12}
+>>> parser(["--foo", "b", "--baz", "Z"])
+parser_b
+{"foo": True, "baz": "Z"}
+```
+
+* **argdeco.add_argument_group**(title=None, description=None)
+
+  * By default, ArgumentParser groups command-line arguments into “positional arguments” and “optional arguments” when displaying help messages. When there is a better conceptual grouping of arguments than this default one, appropriate groups can be created using the add_argument_group() method. The last added argument group in the decorator chain will be the one receiving the subsequently added arguments.
+
+```py
+>>> @argdeco.add_argument("bar", help="bar help")
+... @argdeco.add_argument("--foo", help="foo help")
+... @argdeco.add_argument_group(title="group")
+... @argdeco.argument_parser(prog="PROG", add_help=False)
+... def parser(**kwargs):
+...     pass
+...
+>>> parser.print_help()
+usage: PROG [--foo FOO] bar
+
+group:
+  bar    bar help
+  --foo FOO  foo help
+```
+
+  * Group are defined in order and arguments are added to the last group in the chain.
+
+```py
+>>> @argdeco.add_argument("bar2", help="bar help")
+... @argdeco.add_argument("--foo2", help="foo help")
+... @argdeco.add_argument_group(title="group2")
+... @argdeco.add_argument("bar1", help="bar help")
+... @argdeco.add_argument("--foo1", help="foo help")
+... @argdeco.add_argument_group(title="group1")
+... @argdeco.argument_parser(prog="PROG", add_help=False)
+... def parser(**kwargs):
+...     pass
+...
+>>> parser.print_help()
+usage: PROG [--foo1 FOO1] [--foo2 FOO2] bar1 bar2
+
+group1:
+  --foo1 FOO1  foo help
+  bar1         bar help
+
+group2:
+  --foo2 FOO2  foo help
+  bar2         bar help
+```
+
+* **ardeco.add_mutually_exclusive_group**(required=False)
+
+```py
+>>> @argdeco.add_argument("--bar", action="store_false")
+... @argdeco.add_argument("--foo", action="store_true")
+... @argdeco.add_mutually_exclusive_group()
+... @argdeco.argument_parser(prog="PROG")
+... def parser(**kwargs):
+...     print(kwargs)
+...
+>>> parser(["--foo"])
+{"foo": True, "bar": True}
+>>> parser(["--bar"])
+{"foo": False, "bar": False}
+>>> parser(["--foo", "--bar"])
+usage: PROG [-h] [--foo | --bar]
+PROG: error: argument --bar: not allowed with argument --foo
+```
+
+# Advanced usage
+
+## Accessing attributes
+
+**argdeco** makes it so that each decorated function is converted to an **argparse** parser, so that further customization can be achieved by calling the proper original methods.
+
+```py
+>>> @argdeco.argument_parser()
+... def prog(self):
+...     pass
+...
+>>> prog.__wrapped__
+<function prog at 0x0000029BCBFABF70>
+>>> prog
+_ArgumentParser(prog="argdeco.py", usage=None, description=None, formatter_class=<class "argparse.HelpFormatter">, conflict_handler="error", add_help=True)
+```
+
+## Class method decoration
+
+argdeco supports class callback method decoration, unlike the big majority of CLI decorator libraries, without any difference as regular callback callable decoration.
+
+```py
+>>> class Prog:
+...
+...     @argdeco.argument_parser()
+...     def parser(self):
+...         pass
+...
+```
+
+Decorating a class will forward the arguments to the *\_\_init__* method (usually not the desired behaviour), as decorated callbacks will ALWAYS be treated as callables.
+
+```py
+>>> @argdeco.argument_parser()
+... class Prog:
+...     pass
+...
+```
+
+Decorating the *\_\_call__* method will forward the arguments to the class itself.
+
+```py
+>>> class Prog:
+...
+...     @argdeco.argument_parser()
+...     def __call__(self):
+...         pass
+...
+```
+
+## Context forwarding
+
+Decorated callback callables can get access to the **argparse** context or parser instance.
+
+```py
+>>> @argdeco.argument_parser(prog="PROG")
+... def parser():
+...     parser.print_help()
+...
+>>> parser([])
+usage: PROG [-h]
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
+
+Class callback method context or parser instance forwarding is still respected on decorated class methods.
+
+```py
+>>> class Prog:
+...
+...     @argdeco.argument_parser(prog="PROG")
+...     def __call__(self):
+...         Prog.__call__.print_help()
+...
+>>> prog = Prog()
+>>> prog([])
+usage: PROG [-h]
+
+optional arguments:
+  -h, --help  show this help message and exit
+```
```

### Comparing `argdeco-josugoar-1.4.0/README.md` & `argdeco-josugoar-1.6.0/argdeco_josugoar.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,74 @@
+Metadata-Version: 2.1
+Name: argdeco-josugoar
+Version: 1.6.0
+Summary: Opinionated argparse wrapper
+Home-page: https://github.com/josugoar/argdeco
+Download-URL: https://github.com/josugoar/argdeco/archive/v1.6.0.tar.gz
+Author: josugoar
+License: MIT
+Project-URL: Source, https://github.com/josugoar/argdeco
+Keywords: argparse cli docker library python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="assets/argdeco.png" alt="argdeco" width="640" height="320" />
 </p>
 
 <h1></h1>
 
-> Unopinionated **argparse** wrapper
+> Opinionated **argparse** wrapper
+
+* API breaking change in later versions due to major refactor!!
 
-* The EXACT same decorating order as regular **argparse** MUST be respected
+* Follows the same decorating order as regular **argparse**
 
-* It is recommended to install the development version directly from the repository
+* Recommended to install the development version directly from the repository
 
 # Why argdeco?
 
 There are so many libraries out there for writing command line utilities; why does **argdeco** exist?
 
 This question is easy to answer: because there is not a single command line utility for Python out there which ticks the following boxes: ([sound familiar?](https://click.palletsprojects.com/en/7.x/why/))
 
-* supports class callback method decoration and method instance binding with class instance forwarding (thank you [Graham Dumpleton](https://github.com/GrahamDumpleton) for [wrapt](https://github.com/GrahamDumpleton/wrapt)!)
+* is fully typed using official **typeshed** **argparse** stubs
+
+* supports class callback method decoration and method instance binding with class instance forwarding
 
 * supports callback callable instance binding with **argparse** context or parser instance forwarding
 
 * shares the EXACT same API as **argparse** using decorators
 
 # Installation
 
 You can get the library directly from PyPI:
 
 ```sh
-$ pip install argdeco-JoshGoA
+$ python -m pip install argdeco-josugoar
 ```
 
 The installation into a [virtualenv](https://github.com/pypa/virtualenv) (or [pipenv](https://github.com/pypa/pipenv)) is heavily recommended.
 
 # API reference
 
-* **argdeco.argument_parser**(wrapped=None, parser_class=argparse.ArgumentParser, ctx=False, prog=None, usage=None, description=None, epilog=None, parents=[], formatter_class=argparse.HelpFormatter, prefix_chars="-", fromfile_prefix_chars=None, argument_default=None, conflict_handler="error", add_help=True, allow_abbrev=True)
+* **argdeco.argument_parser**(prog=None, usage=None, description=None, epilog=None, parents=[], formatter_class=argparse.HelpFormatter, prefix_chars="-", fromfile_prefix_chars=None, argument_default=None, conflict_handler="error", add_help=True, allow_abbrev=True, exit_on_error=True)
 
   * Create a new ArgumentParser object. All parameters should be passed as keyword arguments. Each parameter has its own more detailed description below, but in short they are:
 
-      * wrapped - The callback callable (default: None)
-
-      * parser_class - The class to instantiate the parser (default: argparse.ArgumentParser)
-
-      * ctx - Pass the **argparse** context or parser instance to the callback callable (default: False)
-
       * prog - The name of the program (default: sys.argv[0])
 
       * usage - The string describing the program usage (default: generated from arguments added to parser)
 
       * description - Text to display before the argument help (default: __doc__)
 
       * epilog - Text to display after the argument help (default: none)
@@ -64,18 +85,20 @@
 
       * conflict_handler - The strategy for resolving conflicting optionals (usually unnecessary)
 
       * add_help - Add a -h/--help option to the parser (default: True)
 
       * allow_abbrev - Allows long options to be abbreviated if the abbreviation is unambiguous. (default: True)
 
+      * exit_on_error - Determines whether or not ArgumentParser exits with error info when an error occurs. (default: True)
+
 ```py
 >>> import argdeco
 >>> @argdeco.add_argument("--foo", help="foo help")
-... @argdeco.argument_parser
+... @argdeco.argument_parser()
 ... def parser(foo):
 ...     pass
 ...
 ```
 
 ```py
 >>> parser(["--help"])
@@ -110,22 +133,20 @@
 
     * help - A brief description of what the argument does.
 
     * metavar - A name for the argument in usage messages.
 
     * dest - The name of the attribute to be added to the object returned by parse_args().
 
-* **argdeco.add_subparsers**(wrapped=None, [title][, description][, prog][, parser_class][, action][, option_string][, dest][, required][, help][, metavar])
+* **argdeco.add_subparsers**([title][, description][, prog][, parser_class][, action][, option_string][, dest][, required][, help][, metavar])
 
   * Many programs split up their functionality into a number of sub-commands, for example, the svn program can invoke sub-commands like svn checkout, svn update, and svn commit. Splitting up functionality this way can be a particularly good idea when a program performs several different functions which require different kinds of command-line arguments. ArgumentParser supports the creation of such sub-commands with the add_subparsers() method. The add_subparsers() method is normally called with no arguments and returns a special action object. This object has a single method, add_parser(), which takes a command name and any ArgumentParser constructor arguments, and returns an ArgumentParser object that can be modified as usual.
 
   * Description of parameters:
 
-    * wrapped - The callback callable (default: None)
-
     * title - title for the sub-parser group in help output; by default “subcommands” if description is provided, otherwise uses title for positional arguments
 
     * description - description for the sub-parser group in help output, by default None
 
     * prog - usage information that will be displayed with sub-command help, by default the name of the program and any positional arguments before the subparser argument
 
     * parser_class - class which will be used to create sub-parser instances, by default the class of the current parser (e.g. ArgumentParser)
@@ -158,15 +179,15 @@
 ... def parser_a(**kwargs):
 ...     print("parser_a")
 ...     print(kwargs)
 ...
 ```
 
 ```py
->>> # create the parser for the "a" command
+>>> # create the parser for the "b" command
 >>> @argdeco.add_argument("--baz", choices="XYZ", help="baz help")
 ... @argdeco.add_parser(parser, "b", help="b help")
 ... def parser_b(**kwargs):
 ...     print("parser_b")
 ...     print(kwargs)
 ...
 ```
@@ -179,38 +200,63 @@
 >>> parser(["--foo", "b", "--baz", "Z"])
 parser_b
 {"foo": True, "baz": "Z"}
 ```
 
 * **argdeco.add_argument_group**(title=None, description=None)
 
-  * By default, ArgumentParser groups command-line arguments into “positional arguments” and “optional arguments” when displaying help messages. When there is a better conceptual grouping of arguments than this default one, appropriate groups can be created using the add_argument_group() method:
+  * By default, ArgumentParser groups command-line arguments into “positional arguments” and “optional arguments” when displaying help messages. When there is a better conceptual grouping of arguments than this default one, appropriate groups can be created using the add_argument_group() method. The last added argument group in the decorator chain will be the one receiving the subsequently added arguments.
 
 ```py
->>> @argdeco.add_argument("bar", group="group", help="bar help")
-... @argdeco.add_argument("--foo", group="group", help="foo help")
-... @argdeco.add_argument_group("group")
+>>> @argdeco.add_argument("bar", help="bar help")
+... @argdeco.add_argument("--foo", help="foo help")
+... @argdeco.add_argument_group(title="group")
 ... @argdeco.argument_parser(prog="PROG", add_help=False)
 ... def parser(**kwargs):
 ...     pass
 ...
 >>> parser.print_help()
 usage: PROG [--foo FOO] bar
 
 group:
   bar    bar help
   --foo FOO  foo help
 ```
 
+  * Group are defined in order and arguments are added to the last group in the chain.
+
+```py
+>>> @argdeco.add_argument("bar2", help="bar help")
+... @argdeco.add_argument("--foo2", help="foo help")
+... @argdeco.add_argument_group(title="group2")
+... @argdeco.add_argument("bar1", help="bar help")
+... @argdeco.add_argument("--foo1", help="foo help")
+... @argdeco.add_argument_group(title="group1")
+... @argdeco.argument_parser(prog="PROG", add_help=False)
+... def parser(**kwargs):
+...     pass
+...
+>>> parser.print_help()
+usage: PROG [--foo1 FOO1] [--foo2 FOO2] bar1 bar2
+
+group1:
+  --foo1 FOO1  foo help
+  bar1         bar help
+
+group2:
+  --foo2 FOO2  foo help
+  bar2         bar help
+```
+
 * **ardeco.add_mutually_exclusive_group**(required=False)
 
 ```py
->>> @argdeco.add_argument("--bar", group="group", action="store_false")
-... @argdeco.add_argument("--foo", group="group", action="store_true")
-... @argdeco.add_mutually_exclusive_group("group")
+>>> @argdeco.add_argument("--bar", action="store_false")
+... @argdeco.add_argument("--foo", action="store_true")
+... @argdeco.add_mutually_exclusive_group()
 ... @argdeco.argument_parser(prog="PROG")
 ... def parser(**kwargs):
 ...     print(kwargs)
 ...
 >>> parser(["--foo"])
 {"foo": True, "bar": True}
 >>> parser(["--bar"])
@@ -220,84 +266,84 @@
 PROG: error: argument --bar: not allowed with argument --foo
 ```
 
 # Advanced usage
 
 ## Accessing attributes
 
-**argdeco** does NOT override decorated functions so that they can be accessed by the user easily if needed. In order to access the **argparse** context or parser instance, it is recommended to use context forwarding.
+**argdeco** makes it so that each decorated function is converted to an **argparse** parser, so that further customization can be achieved by calling the proper original methods.
 
 ```py
->>> @argdeco.argument_parser
+>>> @argdeco.argument_parser()
 ... def prog(self):
 ...     pass
 ...
 >>> prog.__wrapped__
 <function prog at 0x0000029BCBFABF70>
->>> prog.parser
-ArgumentParser(prog="argdeco.py", usage=None, description=None, formatter_class=<class "argparse.HelpFormatter">, conflict_handler="error", add_help=True)
+>>> prog
+_ArgumentParser(prog="argdeco.py", usage=None, description=None, formatter_class=<class "argparse.HelpFormatter">, conflict_handler="error", add_help=True)
 ```
 
 ## Class method decoration
 
-**argdeco** supports class callback method decoration, unlike the big majority of CLI decorator libraries, without any difference as regular callback callable decoration.
+argdeco supports class callback method decoration, unlike the big majority of CLI decorator libraries, without any difference as regular callback callable decoration.
 
 ```py
 >>> class Prog:
 ...
-...     @argdeco.argument_parser
+...     @argdeco.argument_parser()
 ...     def parser(self):
 ...         pass
 ...
 ```
 
 Decorating a class will forward the arguments to the *\_\_init__* method (usually not the desired behaviour), as decorated callbacks will ALWAYS be treated as callables.
 
 ```py
->>> @argdeco.argument_parser
+>>> @argdeco.argument_parser()
 ... class Prog:
 ...     pass
 ...
 ```
 
-Decorating the *\_\_call__* method will forward the arguments to the class itself, following standard decorator usage as specified by [wrapt](https://wrapt.readthedocs.io/en/latest/decorators.html#decorating-class-methods).
+Decorating the *\_\_call__* method will forward the arguments to the class itself.
 
 ```py
 >>> class Prog:
 ...
-...     @argdeco.argument_parser
+...     @argdeco.argument_parser()
 ...     def __call__(self):
 ...         pass
 ...
 ```
 
 ## Context forwarding
 
 Decorated callback callables can get access to the **argparse** context or parser instance.
 
 ```py
->>> @argdeco.argument_parser(ctx=True, prog="PROG")
-... def parser(ctx):
-...     ctx.print_help()
+>>> @argdeco.argument_parser(prog="PROG")
+... def parser():
+...     parser.print_help()
 ...
 >>> parser([])
 usage: PROG [-h]
 
 optional arguments:
   -h, --help  show this help message and exit
 ```
 
 Class callback method context or parser instance forwarding is still respected on decorated class methods.
 
 ```py
 >>> class Prog:
 ...
-...     @argdeco.argument_parser(ctx=True, prog="PROG")
-...     def __call__(self, ctx):
-...         ctx.print_help()
+...     @argdeco.argument_parser(prog="PROG")
+...     def __call__(self):
+...         Prog.__call__.print_help()
 ...
 >>> prog = Prog()
 >>> prog([])
 usage: PROG [-h]
 
 optional arguments:
   -h, --help  show this help message and exit
```

### Comparing `argdeco-josugoar-1.4.0/setup.py` & `argdeco-josugoar-1.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import setuptools
 
-with open("README.md") as f:
+with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="argdeco-josugoar",
-    version="1.4.0",
-    description="Unopinionated argparse wrapper",
+    version="1.6.0",
+    description="Opinionated argparse wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="josugoar",
     url="https://github.com/josugoar/argdeco",
-    download_url="https://github.com/josugoar/argdeco/archive/v1.4.0.tar.gz",
+    download_url="https://github.com/josugoar/argdeco/archive/v1.6.0.tar.gz",
     py_modules=["argdeco"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
-    package_data={"argdeco": ["LICENSE", "README.md"]},
+    package_data={"argdeco": ["LICENSE", "README.md", "py.typed", "argdeco.pyi"]},
     license="MIT",
-    keywords="argparse cli library pipenv python wrapt",
+    keywords="argparse cli docker library python",
     project_urls={"Source": "https://github.com/josugoar/argdeco"},
-    install_requires=["wrapt"],
-    python_requires=">=3.8"
+    python_requires=">=3.9"
 )
```

