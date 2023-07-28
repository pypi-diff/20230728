# Comparing `tmp/crimson-1.1.0.tar.gz` & `tmp/crimson-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crimson-1.1.0.tar", max compression
+gzip compressed data, was "crimson-1.1.1.tar", max compression
```

## Comparing `crimson-1.1.0.tar` & `crimson-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2325 2022-04-11 16:07:50.180711 crimson-1.1.0/CHANGELOG.adoc
--rw-r--r--   0        0        0     1512 2021-07-06 19:43:02.314200 crimson-1.1.0/LICENSE
--rw-r--r--   0        0        0     4138 2021-07-04 20:20:27.751950 crimson-1.1.0/README.md
--rw-r--r--   0        0        0      395 2021-07-06 19:43:02.314200 crimson-1.1.0/crimson/__init__.py
--rw-r--r--   0        0        0     5268 2021-07-06 19:43:02.314200 crimson-1.1.0/crimson/cli.py
--rw-r--r--   0        0        0     8727 2021-07-06 19:43:02.314200 crimson-1.1.0/crimson/fastqc.py
--rw-r--r--   0        0        0     2938 2021-07-06 19:43:02.314200 crimson-1.1.0/crimson/flagstat.py
--rw-r--r--   0        0        0     6375 2021-07-06 19:43:02.314200 crimson-1.1.0/crimson/fusioncatcher.py
--rw-r--r--   0        0        0     3480 2021-10-31 10:36:02.582669 crimson-1.1.0/crimson/picard.py
--rw-r--r--   0        0        0     3822 2021-07-06 19:43:02.314200 crimson-1.1.0/crimson/star.py
--rw-r--r--   0        0        0    12454 2022-04-11 04:33:23.738319 crimson-1.1.0/crimson/star_fusion.py
--rw-r--r--   0        0        0     3350 2022-04-11 10:38:31.620395 crimson-1.1.0/crimson/utils.py
--rw-r--r--   0        0        0     3405 2021-10-11 22:28:24.631166 crimson-1.1.0/crimson/vep.py
--rw-r--r--   0        0        0     1669 2022-04-11 16:26:14.502373 crimson-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5098 2022-04-11 16:26:15.005735 crimson-1.1.0/setup.py
--rw-r--r--   0        0        0     5305 2022-04-11 16:26:15.006063 crimson-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2632 2023-07-28 21:15:34.281514 crimson-1.1.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1566 2022-12-04 05:53:19.619351 crimson-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4639 2022-12-04 05:53:19.622684 crimson-1.1.1/README.md
+-rw-r--r--   0        0        0      445 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/__init__.py
+-rw-r--r--   0        0        0     5341 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/cli.py
+-rw-r--r--   0        0        0     8777 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/fastqc.py
+-rw-r--r--   0        0        0     2988 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/flagstat.py
+-rw-r--r--   0        0        0     6425 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/fusioncatcher.py
+-rw-r--r--   0        0        0     3530 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/picard.py
+-rw-r--r--   0        0        0     3872 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/star.py
+-rw-r--r--   0        0        0    12504 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/star_fusion.py
+-rw-r--r--   0        0        0     3400 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/utils.py
+-rw-r--r--   0        0        0     3455 2022-12-04 05:53:19.622684 crimson-1.1.1/crimson/vep.py
+-rw-r--r--   0        0        0     2444 2023-07-28 21:16:50.506777 crimson-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5641 1970-01-01 00:00:00.000000 crimson-1.1.1/setup.py
+-rw-r--r--   0        0        0     6051 1970-01-01 00:00:00.000000 crimson-1.1.1/PKG-INFO
```

### Comparing `crimson-1.1.0/LICENSE` & `crimson-1.1.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Copyright (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
 
 All rights reserved.
 
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
+    1. Redistributions of source code must retain the above copyright notice,
+       this list of conditions and the following disclaimer.
 
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of crimson nor the names of its contributors may be used to
-  endorse or promote products derived from this software without specific prior
-  written permission.
+    2. Redistributions in binary form must reproduce the above copyright notice,
+       this list of conditions and the following disclaimer in the documentation
+       and/or other materials provided with the distribution.
+
+    3. Neither the name of the copyright holder nor the names of its
+       contributors may be used to endorse or promote products derived from this
+       software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+ LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `crimson-1.1.0/README.md` & `crimson-1.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,103 @@
-# `crimson`
+# Crimson
 
 [![pypi](https://img.shields.io/pypi/v/crimson)](https://pypi.org/project/crimson)
-[![sourcehut](https://builds.sr.ht/~bow/crimson.svg)](https://builds.sr.ht/~bow/crimson?)
+[![ci](https://github.com/bow/crimson/actions/workflows/ci.yml/badge.svg)](https://github.com/bow/crimson/actions?query=branch%3Amaster)
+[![coverage](https://api.codeclimate.com/v1/badges/7904a5424f60f09ebbd7/test_coverage)](https://codeclimate.com/github/bow/crimson/test_coverage)
 
 
-``crimson`` converts non-standard bioinformatics tool outputs to JSON or YAML.
+Crimson converts non-standard bioinformatics tool outputs to JSON or YAML.
 
 Currently it can convert outputs of the following tools:
 
   * [FastQC](http://www.bioinformatics.babraham.ac.uk/projects/fastqc/>) (``fastqc``)
   * [FusionCatcher](https://github.com/ndaniel/fusioncatcher) (``fusioncatcher``)
   * [samtools](http://www.htslib.org/doc/samtools.html) flagstat (``flagstat``)
   * [Picard](https://broadinstitute.github.io/picard/) metrics tools (``picard``)
   * [STAR](https://github.com/alexdobin/STAR) log file (``star``)
   * [STAR-Fusion](https://github.com/STAR-Fusion/STAR-Fusion) hits table (``star-fusion``)
   * [Variant Effect Predictor](http://www.ensembl.org/info/docs/tools/vep/index.html)
     plain text output (``vep``)
 
-The conversion can be done using the command line interface or by calling the
-tool-specificparser functions in your Python script.
+For each conversion, there are two execution options: as command line tool or as a Python
+library function. The first alternative uses `crimson` as a command-line tool. The second one
+requires importing the `crimson` library in your program.
 
 
 ## Installation
 
-``crimson`` is available on the [Python Package Index](https://pypi.org/project/crimson/)
+Crimson is available on the [Python Package Index](https://pypi.org/project/crimson/)
 and you can install it via ``pip``:
 
 ```shell
 $ pip install crimson
 ```
 
 It is also available on
 [BioConda](https://bioconda.github.io/recipes/crimson/README.html), both through the
 `conda` package manager or as a
 [Docker container](https://quay.io/repository/biocontainers/crimson?tab=tags).
 
+For Docker execution, you may also use
+[the GitHub Docker registry](https://github.com/bow/crimson/pkgs/container/crimson). This
+registry hosts the latest version, but does not host versions 1.1.0 or earlier.
+
+```shell
+docker pull ghcr.io/bow/crimson
+```
+
 
 ## Usage
 
 ### As a command line tool
 
-The general command is `crimson {program_name}` and by default the output is written to
+The general command is `crimson {tool_name}`. By default, the output is written to
 `stdout`. For example, to use the `picard` parser, you would execute:
 
 ```shell
 $ crimson picard /path/to/a/picard.metrics
 ```
 
-You can also specify a file name directly to write to a file. The following command will
-write the output to a file named ``converted.json``:
+You can also write the output to a file by specifying a file name. The following
+command writes the output to a file named `converted.json`:
 
 ```shell
 $ crimson picard /path/to/a/picard.metrics converted.json
 ```
 
-Some parsers may also accept additional input format. The FastQC parser, for example, also
-works if you specify a path to a FastQC output directory:
+Some parsers may accept additional input formats. The FastQC parser, for example, also
+accepts a path to a FastQC output directory as its input:
 
 
 ```shell
 $ crimson fastqc /path/to/a/fastqc/dir
 ```
 
-or path to a zipped result:
+It also accepts a path to a zipped result:
 
 ```shell
 $ crimson fastqc /path/to/a/fastqc_result.zip
 ```
 
 When in doubt, use the ``--help`` flag:
 
 ```shell
 $ crimson --help            # for the general help
-$ crimson fastqc --help     # for parser-specific (FastQC) help
+$ crimson fastqc --help     # for the parser-specific help, in this case FastQC
 ```
 
 ### As a Python library function
 
-Generally, the function to import is located at `crimson.{program_name}.parser`. For
-example, to use the `picard` parser in your script, you can do:
+The specific function to import is generally located at `crimson.{tool_name}.parser`. So to
+use the `picard` parser in your program, you can do:
 
 ```python
 from crimson import picard
 
-# You can specify the input file name as a string ...
+# You can specify the input file name as a string or path-like object...
 parsed = picard.parse("/path/to/a/picard.metrics")
 
 # ... or a file handle
 with open("/path/to/a/picard.metrics") as src:
     parsed = picard.parse(src)
 ```
 
@@ -97,43 +107,41 @@
   * Writing and re-writing the same parsers across different scripts is not a productive
     way to spend the day.
 
 
 ## Local Development
 
 Setting up a local development requires that you set up all of the supported Python
-versions. We recommend using [pyenv](https://github.com/pyenv/pyenv) for this.
-
-The following steps can be your guide for your local development setup:
+versions. We use [pyenv](https://github.com/pyenv/pyenv) for this.
 
 ```shell
 # Clone the repository and cd into it.
-$ git clone https://git.sr.ht/~bow/crimson
+$ git clone https://github.com/bow/crimson
 $ cd crimson
 
-# Create your virtualenv.
-# If you already have pyenv installed, you may use the Makefile rule below.
-$ make dev-pyenv
-
-# Install the package along with its development dependencies.
-$ make dev
+# Create your local development environment. This command also installs
+# all supported Python versions using `pyenv`.
+$ make env
 
 # Run the test and linter suite to verify the setup.
 $ make lint test
+
+# When in doubt, just run `make` without any arguments.
+$ make
 ```
 
 
 ## Contributing
 
-If you are interested, `crimson` accepts the following types contribution:
+If you are interested, Crimson accepts the following types contribution:
 
-  * Documentation additions (if anything seems unclear, feel free to open an issue)
+  * Documentation updates / tweaks (if anything seems unclear, feel free to open an issue)
   * Bug reports
-  * Support for tools' outputs which can be converted to JSON or YAML.
+  * Support for tools' outputs which can be converted to JSON or YAML
 
 For any of these, feel free to open an issue in the [issue
 tracker](https://github.com/bow/crimson/issues>) or submit a pull request.
 
 
 ## License
 
-``crimson`` is BSD-licensed. Refer to the ``LICENSE`` file for the full license.
+Crimson is BSD-licensed. Refer to the ``LICENSE`` file for the full license.
```

### Comparing `crimson-1.1.0/crimson/cli.py` & `crimson-1.1.1/crimson/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Main entry point for command line invocation"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 from pathlib import Path
 from typing import Optional, TextIO, cast
 
 import click
 
 from . import __version__
@@ -14,15 +15,15 @@
 from . import star as m_star
 from . import star_fusion as m_star_fusion
 from . import vep as m_vep
 from .utils import write_output
 
 
 @click.group()
-@click.version_option(__version__)
+@click.version_option(__version__, message="%(version)s")
 @click.option(
     "--fmt",
     default="json",
     type=click.Choice(["json", "yaml"]),
     help="Output file format. Default: json.",
 )
 @click.option(
```

### Comparing `crimson-1.1.0/crimson/fastqc.py` & `crimson-1.1.1/crimson/fastqc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parser for FastQC output"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 from io import StringIO
 from os import PathLike, walk
 from pathlib import Path
 from typing import IO, Any, Dict, List, TextIO, Union, cast
 from zipfile import ZipFile, is_zipfile
```

### Comparing `crimson-1.1.0/crimson/flagstat.py` & `crimson-1.1.1/crimson/flagstat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parser for samtools flagstat output"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 import re
 from functools import partial
 from os import PathLike
 from typing import List, Optional, Pattern, TextIO, Union
 
 import click
```

### Comparing `crimson-1.1.0/crimson/fusioncatcher.py` & `crimson-1.1.1/crimson/fusioncatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parser for FusionCatcher"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 from os import PathLike
 from typing import Dict, List, TextIO, Union
 
 import click
 
 from .utils import get_handle
```

### Comparing `crimson-1.1.0/crimson/picard.py` & `crimson-1.1.1/crimson/picard.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parser for Picard metrics files"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import re
 from typing import Any, Dict, Optional, TextIO, Union
 
 import click
```

### Comparing `crimson-1.1.0/crimson/star.py` & `crimson-1.1.1/crimson/star.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parser for STAR Log.final.out file"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 import os
 from typing import Any, Callable, Dict, Optional, TextIO, Tuple, Union
 
 import click
 
 from .utils import convert, get_handle, get_linesep
```

### Comparing `crimson-1.1.0/crimson/star_fusion.py` & `crimson-1.1.1/crimson/star_fusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parser for STAR-Fusion output"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 from os import PathLike
 from typing import Any, Dict, List, TextIO, Tuple, Union
 
 import click
 
 from .utils import get_handle
```

### Comparing `crimson-1.1.0/crimson/utils.py` & `crimson-1.1.1/crimson/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """General utilities"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 import json
 import os
 import re
 from contextlib import contextmanager
 from os import PathLike, linesep
 from pathlib import Path
```

### Comparing `crimson-1.1.0/crimson/vep.py` & `crimson-1.1.1/crimson/vep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Parser for VEP plain text statistics file"""
-# (c) 2015-2021 Wibowo Arindrarto <contact@arindrarto.dev>
+# Copyright (c) 2015-2022 Wibowo Arindrarto <contact@arindrarto.dev>
+# SPDX-License-Identifier: BSD-3-Clause
 
 import collections
 from os import PathLike
 from typing import Dict, List, Optional, TextIO, Tuple, Union
 
 import click
```

### Comparing `crimson-1.1.0/setup.py` & `crimson-1.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 packages = \
 ['crimson']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=5.2,<6.0', 'click>=8.0,<9.0', 'single-source>=0.2.0,<0.3.0']
+['PyYAML>=6.0,<7.0',
+ 'click>=8.0,<9.0',
+ 'single-source>=0.2.0,<0.3.0',
+ 'urllib3>=1.26.16,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['crimson = crimson.cli:main']}
 
 setup_kwargs = {
     'name': 'crimson',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'Bioinformatics tool outputs converter to JSON or YAML',
-    'long_description': '# `crimson`\n\n[![pypi](https://img.shields.io/pypi/v/crimson)](https://pypi.org/project/crimson)\n[![sourcehut](https://builds.sr.ht/~bow/crimson.svg)](https://builds.sr.ht/~bow/crimson?)\n\n\n``crimson`` converts non-standard bioinformatics tool outputs to JSON or YAML.\n\nCurrently it can convert outputs of the following tools:\n\n  * [FastQC](http://www.bioinformatics.babraham.ac.uk/projects/fastqc/>) (``fastqc``)\n  * [FusionCatcher](https://github.com/ndaniel/fusioncatcher) (``fusioncatcher``)\n  * [samtools](http://www.htslib.org/doc/samtools.html) flagstat (``flagstat``)\n  * [Picard](https://broadinstitute.github.io/picard/) metrics tools (``picard``)\n  * [STAR](https://github.com/alexdobin/STAR) log file (``star``)\n  * [STAR-Fusion](https://github.com/STAR-Fusion/STAR-Fusion) hits table (``star-fusion``)\n  * [Variant Effect Predictor](http://www.ensembl.org/info/docs/tools/vep/index.html)\n    plain text output (``vep``)\n\nThe conversion can be done using the command line interface or by calling the\ntool-specificparser functions in your Python script.\n\n\n## Installation\n\n``crimson`` is available on the [Python Package Index](https://pypi.org/project/crimson/)\nand you can install it via ``pip``:\n\n```shell\n$ pip install crimson\n```\n\nIt is also available on\n[BioConda](https://bioconda.github.io/recipes/crimson/README.html), both through the\n`conda` package manager or as a\n[Docker container](https://quay.io/repository/biocontainers/crimson?tab=tags).\n\n\n## Usage\n\n### As a command line tool\n\nThe general command is `crimson {program_name}` and by default the output is written to\n`stdout`. For example, to use the `picard` parser, you would execute:\n\n```shell\n$ crimson picard /path/to/a/picard.metrics\n```\n\nYou can also specify a file name directly to write to a file. The following command will\nwrite the output to a file named ``converted.json``:\n\n```shell\n$ crimson picard /path/to/a/picard.metrics converted.json\n```\n\nSome parsers may also accept additional input format. The FastQC parser, for example, also\nworks if you specify a path to a FastQC output directory:\n\n\n```shell\n$ crimson fastqc /path/to/a/fastqc/dir\n```\n\nor path to a zipped result:\n\n```shell\n$ crimson fastqc /path/to/a/fastqc_result.zip\n```\n\nWhen in doubt, use the ``--help`` flag:\n\n```shell\n$ crimson --help            # for the general help\n$ crimson fastqc --help     # for parser-specific (FastQC) help\n```\n\n### As a Python library function\n\nGenerally, the function to import is located at `crimson.{program_name}.parser`. For\nexample, to use the `picard` parser in your script, you can do:\n\n```python\nfrom crimson import picard\n\n# You can specify the input file name as a string ...\nparsed = picard.parse("/path/to/a/picard.metrics")\n\n# ... or a file handle\nwith open("/path/to/a/picard.metrics") as src:\n    parsed = picard.parse(src)\n```\n\n## Why?\n\n  * Not enough tools use standard output formats.\n  * Writing and re-writing the same parsers across different scripts is not a productive\n    way to spend the day.\n\n\n## Local Development\n\nSetting up a local development requires that you set up all of the supported Python\nversions. We recommend using [pyenv](https://github.com/pyenv/pyenv) for this.\n\nThe following steps can be your guide for your local development setup:\n\n```shell\n# Clone the repository and cd into it.\n$ git clone https://git.sr.ht/~bow/crimson\n$ cd crimson\n\n# Create your virtualenv.\n# If you already have pyenv installed, you may use the Makefile rule below.\n$ make dev-pyenv\n\n# Install the package along with its development dependencies.\n$ make dev\n\n# Run the test and linter suite to verify the setup.\n$ make lint test\n```\n\n\n## Contributing\n\nIf you are interested, `crimson` accepts the following types contribution:\n\n  * Documentation additions (if anything seems unclear, feel free to open an issue)\n  * Bug reports\n  * Support for tools\' outputs which can be converted to JSON or YAML.\n\nFor any of these, feel free to open an issue in the [issue\ntracker](https://github.com/bow/crimson/issues>) or submit a pull request.\n\n\n## License\n\n``crimson`` is BSD-licensed. Refer to the ``LICENSE`` file for the full license.\n',
+    'long_description': '# Crimson\n\n[![pypi](https://img.shields.io/pypi/v/crimson)](https://pypi.org/project/crimson)\n[![ci](https://github.com/bow/crimson/actions/workflows/ci.yml/badge.svg)](https://github.com/bow/crimson/actions?query=branch%3Amaster)\n[![coverage](https://api.codeclimate.com/v1/badges/7904a5424f60f09ebbd7/test_coverage)](https://codeclimate.com/github/bow/crimson/test_coverage)\n\n\nCrimson converts non-standard bioinformatics tool outputs to JSON or YAML.\n\nCurrently it can convert outputs of the following tools:\n\n  * [FastQC](http://www.bioinformatics.babraham.ac.uk/projects/fastqc/>) (``fastqc``)\n  * [FusionCatcher](https://github.com/ndaniel/fusioncatcher) (``fusioncatcher``)\n  * [samtools](http://www.htslib.org/doc/samtools.html) flagstat (``flagstat``)\n  * [Picard](https://broadinstitute.github.io/picard/) metrics tools (``picard``)\n  * [STAR](https://github.com/alexdobin/STAR) log file (``star``)\n  * [STAR-Fusion](https://github.com/STAR-Fusion/STAR-Fusion) hits table (``star-fusion``)\n  * [Variant Effect Predictor](http://www.ensembl.org/info/docs/tools/vep/index.html)\n    plain text output (``vep``)\n\nFor each conversion, there are two execution options: as command line tool or as a Python\nlibrary function. The first alternative uses `crimson` as a command-line tool. The second one\nrequires importing the `crimson` library in your program.\n\n\n## Installation\n\nCrimson is available on the [Python Package Index](https://pypi.org/project/crimson/)\nand you can install it via ``pip``:\n\n```shell\n$ pip install crimson\n```\n\nIt is also available on\n[BioConda](https://bioconda.github.io/recipes/crimson/README.html), both through the\n`conda` package manager or as a\n[Docker container](https://quay.io/repository/biocontainers/crimson?tab=tags).\n\nFor Docker execution, you may also use\n[the GitHub Docker registry](https://github.com/bow/crimson/pkgs/container/crimson). This\nregistry hosts the latest version, but does not host versions 1.1.0 or earlier.\n\n```shell\ndocker pull ghcr.io/bow/crimson\n```\n\n\n## Usage\n\n### As a command line tool\n\nThe general command is `crimson {tool_name}`. By default, the output is written to\n`stdout`. For example, to use the `picard` parser, you would execute:\n\n```shell\n$ crimson picard /path/to/a/picard.metrics\n```\n\nYou can also write the output to a file by specifying a file name. The following\ncommand writes the output to a file named `converted.json`:\n\n```shell\n$ crimson picard /path/to/a/picard.metrics converted.json\n```\n\nSome parsers may accept additional input formats. The FastQC parser, for example, also\naccepts a path to a FastQC output directory as its input:\n\n\n```shell\n$ crimson fastqc /path/to/a/fastqc/dir\n```\n\nIt also accepts a path to a zipped result:\n\n```shell\n$ crimson fastqc /path/to/a/fastqc_result.zip\n```\n\nWhen in doubt, use the ``--help`` flag:\n\n```shell\n$ crimson --help            # for the general help\n$ crimson fastqc --help     # for the parser-specific help, in this case FastQC\n```\n\n### As a Python library function\n\nThe specific function to import is generally located at `crimson.{tool_name}.parser`. So to\nuse the `picard` parser in your program, you can do:\n\n```python\nfrom crimson import picard\n\n# You can specify the input file name as a string or path-like object...\nparsed = picard.parse("/path/to/a/picard.metrics")\n\n# ... or a file handle\nwith open("/path/to/a/picard.metrics") as src:\n    parsed = picard.parse(src)\n```\n\n## Why?\n\n  * Not enough tools use standard output formats.\n  * Writing and re-writing the same parsers across different scripts is not a productive\n    way to spend the day.\n\n\n## Local Development\n\nSetting up a local development requires that you set up all of the supported Python\nversions. We use [pyenv](https://github.com/pyenv/pyenv) for this.\n\n```shell\n# Clone the repository and cd into it.\n$ git clone https://github.com/bow/crimson\n$ cd crimson\n\n# Create your local development environment. This command also installs\n# all supported Python versions using `pyenv`.\n$ make env\n\n# Run the test and linter suite to verify the setup.\n$ make lint test\n\n# When in doubt, just run `make` without any arguments.\n$ make\n```\n\n\n## Contributing\n\nIf you are interested, Crimson accepts the following types contribution:\n\n  * Documentation updates / tweaks (if anything seems unclear, feel free to open an issue)\n  * Bug reports\n  * Support for tools\' outputs which can be converted to JSON or YAML\n\nFor any of these, feel free to open an issue in the [issue\ntracker](https://github.com/bow/crimson/issues>) or submit a pull request.\n\n\n## License\n\nCrimson is BSD-licensed. Refer to the ``LICENSE`` file for the full license.\n',
     'author': 'Wibowo Arindrarto',
     'author_email': 'contact@arindrarto.dev',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://git.sr.ht/~bow/crimson',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/bow/crimson',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `crimson-1.1.0/PKG-INFO` & `crimson-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,138 @@
 Metadata-Version: 2.1
 Name: crimson
-Version: 1.1.0
+Version: 1.1.1
 Summary: Bioinformatics tool outputs converter to JSON or YAML
-Home-page: https://git.sr.ht/~bow/crimson
+Home-page: https://github.com/bow/crimson
 License: BSD-3-Clause
 Keywords: bioinformatics,json,yaml
 Author: Wibowo Arindrarto
 Author-email: contact@arindrarto.dev
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Dist: PyYAML (>=5.2,<6.0)
+Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: single-source (>=0.2.0,<0.3.0)
-Project-URL: Repository, https://git.sr.ht/~bow/crimson
+Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
+Project-URL: Repository, https://github.com/bow/crimson
 Description-Content-Type: text/markdown
 
-# `crimson`
+# Crimson
 
 [![pypi](https://img.shields.io/pypi/v/crimson)](https://pypi.org/project/crimson)
-[![sourcehut](https://builds.sr.ht/~bow/crimson.svg)](https://builds.sr.ht/~bow/crimson?)
+[![ci](https://github.com/bow/crimson/actions/workflows/ci.yml/badge.svg)](https://github.com/bow/crimson/actions?query=branch%3Amaster)
+[![coverage](https://api.codeclimate.com/v1/badges/7904a5424f60f09ebbd7/test_coverage)](https://codeclimate.com/github/bow/crimson/test_coverage)
 
 
-``crimson`` converts non-standard bioinformatics tool outputs to JSON or YAML.
+Crimson converts non-standard bioinformatics tool outputs to JSON or YAML.
 
 Currently it can convert outputs of the following tools:
 
   * [FastQC](http://www.bioinformatics.babraham.ac.uk/projects/fastqc/>) (``fastqc``)
   * [FusionCatcher](https://github.com/ndaniel/fusioncatcher) (``fusioncatcher``)
   * [samtools](http://www.htslib.org/doc/samtools.html) flagstat (``flagstat``)
   * [Picard](https://broadinstitute.github.io/picard/) metrics tools (``picard``)
   * [STAR](https://github.com/alexdobin/STAR) log file (``star``)
   * [STAR-Fusion](https://github.com/STAR-Fusion/STAR-Fusion) hits table (``star-fusion``)
   * [Variant Effect Predictor](http://www.ensembl.org/info/docs/tools/vep/index.html)
     plain text output (``vep``)
 
-The conversion can be done using the command line interface or by calling the
-tool-specificparser functions in your Python script.
+For each conversion, there are two execution options: as command line tool or as a Python
+library function. The first alternative uses `crimson` as a command-line tool. The second one
+requires importing the `crimson` library in your program.
 
 
 ## Installation
 
-``crimson`` is available on the [Python Package Index](https://pypi.org/project/crimson/)
+Crimson is available on the [Python Package Index](https://pypi.org/project/crimson/)
 and you can install it via ``pip``:
 
 ```shell
 $ pip install crimson
 ```
 
 It is also available on
 [BioConda](https://bioconda.github.io/recipes/crimson/README.html), both through the
 `conda` package manager or as a
 [Docker container](https://quay.io/repository/biocontainers/crimson?tab=tags).
 
+For Docker execution, you may also use
+[the GitHub Docker registry](https://github.com/bow/crimson/pkgs/container/crimson). This
+registry hosts the latest version, but does not host versions 1.1.0 or earlier.
+
+```shell
+docker pull ghcr.io/bow/crimson
+```
+
 
 ## Usage
 
 ### As a command line tool
 
-The general command is `crimson {program_name}` and by default the output is written to
+The general command is `crimson {tool_name}`. By default, the output is written to
 `stdout`. For example, to use the `picard` parser, you would execute:
 
 ```shell
 $ crimson picard /path/to/a/picard.metrics
 ```
 
-You can also specify a file name directly to write to a file. The following command will
-write the output to a file named ``converted.json``:
+You can also write the output to a file by specifying a file name. The following
+command writes the output to a file named `converted.json`:
 
 ```shell
 $ crimson picard /path/to/a/picard.metrics converted.json
 ```
 
-Some parsers may also accept additional input format. The FastQC parser, for example, also
-works if you specify a path to a FastQC output directory:
+Some parsers may accept additional input formats. The FastQC parser, for example, also
+accepts a path to a FastQC output directory as its input:
 
 
 ```shell
 $ crimson fastqc /path/to/a/fastqc/dir
 ```
 
-or path to a zipped result:
+It also accepts a path to a zipped result:
 
 ```shell
 $ crimson fastqc /path/to/a/fastqc_result.zip
 ```
 
 When in doubt, use the ``--help`` flag:
 
 ```shell
 $ crimson --help            # for the general help
-$ crimson fastqc --help     # for parser-specific (FastQC) help
+$ crimson fastqc --help     # for the parser-specific help, in this case FastQC
 ```
 
 ### As a Python library function
 
-Generally, the function to import is located at `crimson.{program_name}.parser`. For
-example, to use the `picard` parser in your script, you can do:
+The specific function to import is generally located at `crimson.{tool_name}.parser`. So to
+use the `picard` parser in your program, you can do:
 
 ```python
 from crimson import picard
 
-# You can specify the input file name as a string ...
+# You can specify the input file name as a string or path-like object...
 parsed = picard.parse("/path/to/a/picard.metrics")
 
 # ... or a file handle
 with open("/path/to/a/picard.metrics") as src:
     parsed = picard.parse(src)
 ```
 
@@ -127,44 +142,42 @@
   * Writing and re-writing the same parsers across different scripts is not a productive
     way to spend the day.
 
 
 ## Local Development
 
 Setting up a local development requires that you set up all of the supported Python
-versions. We recommend using [pyenv](https://github.com/pyenv/pyenv) for this.
-
-The following steps can be your guide for your local development setup:
+versions. We use [pyenv](https://github.com/pyenv/pyenv) for this.
 
 ```shell
 # Clone the repository and cd into it.
-$ git clone https://git.sr.ht/~bow/crimson
+$ git clone https://github.com/bow/crimson
 $ cd crimson
 
-# Create your virtualenv.
-# If you already have pyenv installed, you may use the Makefile rule below.
-$ make dev-pyenv
-
-# Install the package along with its development dependencies.
-$ make dev
+# Create your local development environment. This command also installs
+# all supported Python versions using `pyenv`.
+$ make env
 
 # Run the test and linter suite to verify the setup.
 $ make lint test
+
+# When in doubt, just run `make` without any arguments.
+$ make
 ```
 
 
 ## Contributing
 
-If you are interested, `crimson` accepts the following types contribution:
+If you are interested, Crimson accepts the following types contribution:
 
-  * Documentation additions (if anything seems unclear, feel free to open an issue)
+  * Documentation updates / tweaks (if anything seems unclear, feel free to open an issue)
   * Bug reports
-  * Support for tools' outputs which can be converted to JSON or YAML.
+  * Support for tools' outputs which can be converted to JSON or YAML
 
 For any of these, feel free to open an issue in the [issue
 tracker](https://github.com/bow/crimson/issues>) or submit a pull request.
 
 
 ## License
 
-``crimson`` is BSD-licensed. Refer to the ``LICENSE`` file for the full license.
+Crimson is BSD-licensed. Refer to the ``LICENSE`` file for the full license.
```

