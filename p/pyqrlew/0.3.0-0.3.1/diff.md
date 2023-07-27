# Comparing `tmp/pyqrlew-0.3.0.tar.gz` & `tmp/pyqrlew-0.3.1.tar.gz`

## Comparing `pyqrlew-0.3.0.tar` & `pyqrlew-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,32 @@
--rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.3.0/Cargo.toml
--rw-r--r--   0     1001      123     4542 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3539 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/.gitignore
--rw-r--r--   0     1001      123      818 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/.readthedocs.yaml
--rw-r--r--   0     1001      123      719 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/CHANGELOG.md
--rw-r--r--   0     1001      123    11357 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/LICENSE
--rw-r--r--   0     1001      123     1466 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/README.md
--rw-r--r--   0     1001      123      634 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/Makefile
--rw-r--r--   0     1001      123     1212 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/conf.py
--rw-r--r--   0     1001      123      224 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/contributing.md
--rw-r--r--   0     1001      123     1786 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/index.md
--rw-r--r--   0     1001      123      800 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/make.bat
--rw-r--r--   0     1001      123       61 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/docs/requirements.txt
--rw-r--r--   0     1001      123    49678 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/PyQrlew.ipynb
--rw-r--r--   0     1001      123   146621 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/demo.ipynb
--rw-r--r--   0     1001      123      431 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/dataset.json
--rw-r--r--   0     1001      123     1032 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/install_db.sql
--rw-r--r--   0     1001      123      234 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/install_db_on_docker.sh
--rw-r--r--   0     1001      123    84990 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/schema.json
--rw-r--r--   0     1001      123    11484 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/demo/retail_data/size.json
--rw-r--r--   0     1001      123      133 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/requirements.txt
--rw-r--r--   0     1001      123      317 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/examples/simple.py
--rw-r--r--   0     1001      123     1139 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/pyproject.toml
--rw-r--r--   0     1001      123      112 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/__init__.py
--rw-r--r--   0     1001      123       45 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/io/__init__.py
--rw-r--r--   0     1001      123    10178 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/io/database.py
--rw-r--r--   0     1001      123     2612 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/python/pyqrlew/io/postgresql.py
--rw-r--r--   0     1001      123    13493 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/src/lib.rs
--rw-r--r--   0     1001      123      136 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/conftest.py
--rw-r--r--   0     1001      123     2481 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/queries/sql_unlimited_queries.sql
--rw-r--r--   0     1001      123     7054 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/queries/valid_queries.sql
--rw-r--r--   0     1001      123      178 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/requirements.txt
--rw-r--r--   0     1001      123     1399 2023-07-22 10:42:56.000000 pyqrlew-0.3.0/tests/test_financial_dataset.py
--rw-r--r--   0     1001      123    48628 2023-07-22 10:43:08.000000 pyqrlew-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      123     4542 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3539 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/.gitignore
+-rw-r--r--   0     1001      123      818 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/.readthedocs.yaml
+-rw-r--r--   0     1001      123      719 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/CHANGELOG.md
+-rw-r--r--   0     1001      123    11357 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/LICENSE
+-rw-r--r--   0     1001      123     1466 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/README.md
+-rw-r--r--   0     1001      123      634 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/Makefile
+-rw-r--r--   0     1001      123     1212 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/conf.py
+-rw-r--r--   0     1001      123      224 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/contributing.md
+-rw-r--r--   0     1001      123     1786 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/index.md
+-rw-r--r--   0     1001      123      800 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/make.bat
+-rw-r--r--   0     1001      123       61 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/requirements.txt
+-rw-r--r--   0     1001      123   146621 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/deprecated_demo.ipynb
+-rw-r--r--   0     1001      123      189 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/expose_protobufs.py
+-rw-r--r--   0     1001      123    45574 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/pyqrlew_display_relations.ipynb
+-rw-r--r--   0     1001      123    39156 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/pyqrlew_retail_demo.ipynb
+-rw-r--r--   0     1001      123      133 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/requirements.txt
+-rw-r--r--   0     1001      123      380 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/simple.py
+-rw-r--r--   0     1001      123     1139 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/pyproject.toml
+-rw-r--r--   0     1001      123      112 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/__init__.py
+-rw-r--r--   0     1001      123       45 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/io/__init__.py
+-rw-r--r--   0     1001      123    12628 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/io/database.py
+-rw-r--r--   0     1001      123     2333 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/io/postgresql.py
+-rw-r--r--   0     1001      123    10104 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      123      136 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/conftest.py
+-rw-r--r--   0     1001      123     2481 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/queries/sql_unlimited_queries.sql
+-rw-r--r--   0     1001      123     7054 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/queries/valid_queries.sql
+-rw-r--r--   0     1001      123      178 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/requirements.txt
+-rw-r--r--   0     1001      123     1431 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/test_extract_dataset.py
+-rw-r--r--   0     1001      123    48628 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.3.1/PKG-INFO
```

### Comparing `pyqrlew-0.3.0/.github/workflows/CI.yml` & `pyqrlew-0.3.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/.gitignore` & `pyqrlew-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/.readthedocs.yaml` & `pyqrlew-0.3.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/CHANGELOG.md` & `pyqrlew-0.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/LICENSE` & `pyqrlew-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/README.md` & `pyqrlew-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/docs/Makefile` & `pyqrlew-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/docs/conf.py` & `pyqrlew-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/docs/index.md` & `pyqrlew-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/docs/make.bat` & `pyqrlew-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/examples/PyQrlew.ipynb` & `pyqrlew-0.3.1/examples/pyqrlew_display_relations.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.739979297563933%*

 * *Differences: {"'cells'": "{0: {'execution_count': None, 'metadata': {replace: OrderedDict([('id', "*

 * *            "'AyS1ZNijGQAG')])}, 'source': ['%%shell\\n', '# Inspred by "*

 * *            "https://colab.research.google.com/github/tensorflow/io/blob/master/docs/tutorials/postgresql.ipynb#scrollTo=YUj0878jPyz7\\n', "*

 * *            "'sudo apt-get -y -qq update\\n', 'sudo apt-get -y -qq install postgresql-14\\n', '# "*

 * *            'Start postgresql server\\n\', \'sudo sed -i "s/port = 5432/port = 5433/g" '*

 * *            "/etc/post […]*

```diff
@@ -1,644 +1,286 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 3,
-            "id": "8beccd5c",
-            "metadata": {},
+            "execution_count": null,
+            "metadata": {
+                "id": "AyS1ZNijGQAG"
+            },
+            "outputs": [],
+            "source": [
+                "%%shell\n",
+                "# Inspred by https://colab.research.google.com/github/tensorflow/io/blob/master/docs/tutorials/postgresql.ipynb#scrollTo=YUj0878jPyz7\n",
+                "sudo apt-get -y -qq update\n",
+                "sudo apt-get -y -qq install postgresql-14\n",
+                "# Start postgresql server\n",
+                "sudo sed -i \"s/port = 5432/port = 5433/g\" /etc/postgresql/14/main/postgresql.conf\n",
+                "sudo service postgresql start\n",
+                "# Set password\n",
+                "sudo -u postgres psql -U postgres -c \"ALTER USER postgres PASSWORD 'pyqrlew-db'\"\n",
+                "# Install python packages\n",
+                "pip install -U pyqrlew graphviz"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {
+                "id": "F4qDGkdTCbKZ"
+            },
             "outputs": [],
             "source": [
                 "import pyqrlew as qrl\n",
                 "from pyqrlew.io import PostgreSQL"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "id": "b5bddda2",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Error response from daemon: network with name qrlew-net already exists\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "/var/run/postgresql:5432 - accepting connections\n",
-                        "/var/run/postgresql:5432 - accepting connections\n",
-                        "/var/run/postgresql:5432 - accepting connections\n"
-                    ]
-                }
-            ],
+            "execution_count": 3,
+            "metadata": {
+                "id": "pjAPehPpCWl8"
+            },
+            "outputs": [],
             "source": [
                 "# Read data\n",
                 "db = PostgreSQL()\n",
                 "dataset = db.financial()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "57f50658",
-            "metadata": {},
+            "execution_count": 4,
+            "metadata": {
+                "colab": {
+                    "base_uri": "https://localhost:8080/"
+                },
+                "id": "GSSZZONiqObY",
+                "outputId": "99155ba4-701b-4e1f-8e1e-afd7c9e8ae68"
+            },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[(['account'], <Relation at 0x10d3d6ed0>),\n",
-                            " (['card'], <Relation at 0x10d3d6c90>),\n",
-                            " (['client'], <Relation at 0x10d3d6fc0>),\n",
-                            " (['disp'], <Relation at 0x10d3d6cc0>),\n",
-                            " (['district'], <Relation at 0x10d3d6b40>),\n",
-                            " (['loan'], <Relation at 0x10d3d6e10>),\n",
-                            " (['order'], <Relation at 0x10d3d6d50>),\n",
-                            " (['trans'], <Relation at 0x10d3d6de0>)]"
+                            "[(['account'], <Relation at 0x7c1c7cbf79c0>),\n",
+                            " (['card'], <Relation at 0x7c1c7cfeed00>),\n",
+                            " (['client'], <Relation at 0x7c1c7cfee9d0>),\n",
+                            " (['disp'], <Relation at 0x7c1c7cb61740>),\n",
+                            " (['district'], <Relation at 0x7c1c7cb616b0>),\n",
+                            " (['loan'], <Relation at 0x7c1c7cb615f0>),\n",
+                            " (['order'], <Relation at 0x7c1c7cb62820>),\n",
+                            " (['trans'], <Relation at 0x7c1c7c722d90>)]"
                         ]
                     },
-                    "execution_count": 5,
+                    "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dataset.relations()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "id": "cfafa037",
-            "metadata": {},
+            "execution_count": 9,
+            "metadata": {
+                "colab": {
+                    "base_uri": "https://localhost:8080/",
+                    "height": 1000
+                },
+                "id": "JV3ATSsvVNLl",
+                "outputId": "f74fede3-02d0-43ef-a421-1f5c48aad9a7"
+            },
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "'digraph graph_agay {\\n\\n        rankdir=\"TB\";\\n        splines=true;\\n        overlap=false;\\n        nodesep=\"0.2\";\\n        ranksep=\"0.4\";\\n        labelloc=\"t\";\\n        fontname=\"Ovo,Red Hat Text\";\\n        fontsize=\"11pt\"\\n        bgcolor=\"#00000000\"\\n\\n            node [ shape=\"box\" style=\"filled,rounded\" margin=0.2, fontname=\"Red Hat Display,sans-serif\", fontsize=\"11pt\", color=\"#00000055\" ]\\n            edge [ fontname=\"Red Hat Text\" color=\"#2B303A\" ]\\n            \\n    graph_agay[label=<<b>ACCOUNT size \u2208 int{0}</b><br/>account_id = account_id \u2208 int<br/>district_id = district_id \u2208 int<br/>frequency = frequency \u2208 str<br/>date = date \u2208 datetime[0001-01-01 00:00:00 9999-12-31 00:00:00]>][fillcolor=\"#ff1744\"][fontcolor=\"#ffffffbb\"];\\n}\\n'"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "dataset.relations()[0][1].dot()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 15,
-            "id": "73b1bf25",
-            "metadata": {},
-            "outputs": [
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Traceback (most recent call last):\n",
+                        "  File \"/usr/local/lib/python3.10/dist-packages/google/colab/_variable_inspector.py\", line 27, in run\n",
+                        "RuntimeError: pyqrlew::Relation is unsendbale, but is dropped on another thread!\n"
+                    ]
+                },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_agay Pages: 1 -->\n",
-                            "<svg width=\"366pt\" height=\"92pt\"\n",
-                            " viewBox=\"0.00 0.00 366.05 91.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87.8)\">\n",
-                            "<title>graph_agay</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-87.8 362.05,-87.8 362.05,4 -4,4\"/>\n",
-                            "<!-- graph_agay -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_agay</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M346.05,-83.8C346.05,-83.8 12,-83.8 12,-83.8 6,-83.8 0,-77.8 0,-71.8 0,-71.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 346.05,0 346.05,0 352.05,0 358.05,-6 358.05,-12 358.05,-12 358.05,-71.8 358.05,-71.8 358.05,-77.8 352.05,-83.8 346.05,-83.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"119.77\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">ACCOUNT size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"110.77\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"116.02\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"114.9\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">frequency = frequency \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_agay Pages: 1 -->\n<svg width=\"463pt\" height=\"91pt\"\n viewBox=\"0.00 0.00 463.00 91.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87)\">\n<title>graph_agay</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-87 459,-87 459,4 -4,4\"/>\n<!-- graph_agay -->\n<g id=\"node1\" class=\"node\">\n<title>graph_agay</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M443,-83C443,-83 12,-83 12,-83 6,-83 0,-77 0,-71 0,-71 0,-12 0,-12 0,-6 6,0 12,0 12,0 443,0 443,0 449,0 455,-6 455,-12 455,-12 455,-71 455,-71 455,-77 449,-83 443,-83\"/>\n<text text-anchor=\"start\" x=\"155.5\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">ACCOUNT size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"129\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"122\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"135.5\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">frequency = frequency \u2208 str</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d4652e0>"
+                            "<graphviz.sources.Source at 0x7c1c7c7cace0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_xo23 Pages: 1 -->\n",
-                            "<svg width=\"383pt\" height=\"92pt\"\n",
-                            " viewBox=\"0.00 0.00 382.55 91.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87.8)\">\n",
-                            "<title>graph_xo23</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-87.8 378.55,-87.8 378.55,4 -4,4\"/>\n",
-                            "<!-- graph_xo23 -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_xo23</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M362.55,-83.8C362.55,-83.8 12,-83.8 12,-83.8 6,-83.8 0,-77.8 0,-71.8 0,-71.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 362.55,0 362.55,0 368.55,0 374.55,-6 374.55,-12 374.55,-12 374.55,-71.8 374.55,-71.8 374.55,-77.8 368.55,-83.8 362.55,-83.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"139.65\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">CARD size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"137.78\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">card_id = card_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"138.53\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">disp_id = disp_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"149.4\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">type = type \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">issued = issued \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_xo23 Pages: 1 -->\n<svg width=\"490pt\" height=\"91pt\"\n viewBox=\"0.00 0.00 490.00 91.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87)\">\n<title>graph_xo23</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-87 486,-87 486,4 -4,4\"/>\n<!-- graph_xo23 -->\n<g id=\"node1\" class=\"node\">\n<title>graph_xo23</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M470,-83C470,-83 12,-83 12,-83 6,-83 0,-77 0,-71 0,-71 0,-12 0,-12 0,-6 6,0 12,0 12,0 470,0 470,0 476,0 482,-6 482,-12 482,-12 482,-71 482,-71 482,-77 476,-83 470,-83\"/>\n<text text-anchor=\"start\" x=\"179\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">CARD size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"162.5\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">card_id = card_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"162.5\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">disp_id = disp_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"183\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">type = type \u2208 str</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">issued = issued \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d0eef10>"
+                            "<graphviz.sources.Source at 0x7c1c7c7cace0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_5y73 Pages: 1 -->\n",
-                            "<svg width=\"420pt\" height=\"92pt\"\n",
-                            " viewBox=\"0.00 0.00 420.05 91.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87.8)\">\n",
-                            "<title>graph_5y73</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-87.8 416.05,-87.8 416.05,4 -4,4\"/>\n",
-                            "<!-- graph_5y73 -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_5y73</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M400.05,-83.8C400.05,-83.8 12,-83.8 12,-83.8 6,-83.8 0,-77.8 0,-71.8 0,-71.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 400.05,0 400.05,0 406.05,0 412.05,-6 412.05,-12 412.05,-12 412.05,-71.8 412.05,-71.8 412.05,-77.8 406.05,-83.8 400.05,-83.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"154.27\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">CLIENT size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"150.52\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">client_id = client_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"155.4\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">gender = gender \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">birth_date = birth_date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "<text text-anchor=\"start\" x=\"143.02\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_5y73 Pages: 1 -->\n<svg width=\"544pt\" height=\"91pt\"\n viewBox=\"0.00 0.00 544.00 91.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87)\">\n<title>graph_5y73</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-87 540,-87 540,4 -4,4\"/>\n<!-- graph_5y73 -->\n<g id=\"node1\" class=\"node\">\n<title>graph_5y73</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M524,-83C524,-83 12,-83 12,-83 6,-83 0,-77 0,-71 0,-71 0,-12 0,-12 0,-6 6,0 12,0 12,0 524,0 524,0 530,0 536,-6 536,-12 536,-12 536,-71 536,-71 536,-77 530,-83 524,-83\"/>\n<text text-anchor=\"start\" x=\"199.5\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">CLIENT size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"176\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">client_id = client_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"196.5\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">gender = gender \u2208 str</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">birth_date = birth_date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n<text text-anchor=\"start\" x=\"162.5\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d0eef10>"
+                            "<graphviz.sources.Source at 0x7c1c9bb229b0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_how1 Pages: 1 -->\n",
-                            "<svg width=\"173pt\" height=\"92pt\"\n",
-                            " viewBox=\"0.00 0.00 173.30 91.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87.8)\">\n",
-                            "<title>graph_how1</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-87.8 169.3,-87.8 169.3,4 -4,4\"/>\n",
-                            "<!-- graph_how1 -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_how1</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M153.3,-83.8C153.3,-83.8 12,-83.8 12,-83.8 6,-83.8 0,-77.8 0,-71.8 0,-71.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 153.3,0 153.3,0 159.3,0 165.3,-6 165.3,-12 165.3,-12 165.3,-71.8 165.3,-71.8 165.3,-77.8 159.3,-83.8 153.3,-83.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"38.4\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">DISP size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"33.9\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">disp_id = disp_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"27.15\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">client_id = client_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"44.78\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">type = type \u2208 str</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_how1 Pages: 1 -->\n<svg width=\"233pt\" height=\"91pt\"\n viewBox=\"0.00 0.00 233.00 91.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 87)\">\n<title>graph_how1</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-87 229,-87 229,4 -4,4\"/>\n<!-- graph_how1 -->\n<g id=\"node1\" class=\"node\">\n<title>graph_how1</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M213,-83C213,-83 12,-83 12,-83 6,-83 0,-77 0,-71 0,-71 0,-12 0,-12 0,-6 6,0 12,0 12,0 213,0 213,0 219,0 225,-6 225,-12 225,-12 225,-71 225,-71 225,-77 219,-83 213,-83\"/>\n<text text-anchor=\"start\" x=\"50.5\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">DISP size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"34\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">disp_id = disp_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"20.5\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">client_id = client_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"54.5\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">type = type \u2208 str</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d0eef10>"
+                            "<graphviz.sources.Source at 0x7c1c9bb229b0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_dsly Pages: 1 -->\n",
-                            "<svg width=\"163pt\" height=\"224pt\"\n",
-                            " viewBox=\"0.00 0.00 162.80 223.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 219.8)\">\n",
-                            "<title>graph_dsly</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-219.8 158.8,-219.8 158.8,4 -4,4\"/>\n",
-                            "<!-- graph_dsly -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_dsly</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M142.8,-215.8C142.8,-215.8 12,-215.8 12,-215.8 6,-215.8 0,-209.8 0,-203.8 0,-203.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 142.8,0 142.8,0 148.8,0 154.8,-6 154.8,-12 154.8,-12 154.8,-203.8 154.8,-203.8 154.8,-209.8 148.8,-215.8 142.8,-215.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"20.03\" y=\"-191.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">DISTRICT size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-180.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"49.28\" y=\"-169.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a2 = a2 \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"49.28\" y=\"-158.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a3 = a3 \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"48.9\" y=\"-147.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a4 = a4 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"49.65\" y=\"-136.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a5 = a5 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"48.9\" y=\"-125.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a6 = a6 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"49.65\" y=\"-114.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a7 = a7 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"48.9\" y=\"-103.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a8 = a8 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"48.9\" y=\"-92.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a9 = a9 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"39.9\" y=\"-81.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a10 = a10 \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"49.65\" y=\"-70.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a11 = a11 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"41.4\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a12 = a12 \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"41.4\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a13 = a13 \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"45.9\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a14 = a14 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"46.65\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a15 = a15 \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"45.9\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a16 = a16 \u2208 int</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_dsly Pages: 1 -->\n<svg width=\"247pt\" height=\"223pt\"\n viewBox=\"0.00 0.00 247.00 223.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 219)\">\n<title>graph_dsly</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-219 243,-219 243,4 -4,4\"/>\n<!-- graph_dsly -->\n<g id=\"node1\" class=\"node\">\n<title>graph_dsly</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M227,-215C227,-215 12,-215 12,-215 6,-215 0,-209 0,-203 0,-203 0,-12 0,-12 0,-6 6,0 12,0 12,0 227,0 227,0 233,0 239,-6 239,-12 239,-12 239,-203 239,-203 239,-209 233,-215 227,-215\"/>\n<text text-anchor=\"start\" x=\"44\" y=\"-193.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">DISTRICT size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-182.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-171.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a2 = a2 \u2208 str</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-160.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a3 = a3 \u2208 str</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-149.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a4 = a4 \u2208 int</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-138.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a5 = a5 \u2208 int</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-127.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a6 = a6 \u2208 int</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-116.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a7 = a7 \u2208 int</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-105.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a8 = a8 \u2208 int</text>\n<text text-anchor=\"start\" x=\"75\" y=\"-94.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a9 = a9 \u2208 int</text>\n<text text-anchor=\"start\" x=\"61.5\" y=\"-83.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a10 = a10 \u2208 float</text>\n<text text-anchor=\"start\" x=\"68\" y=\"-72.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a11 = a11 \u2208 int</text>\n<text text-anchor=\"start\" x=\"61.5\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a12 = a12 \u2208 float</text>\n<text text-anchor=\"start\" x=\"61.5\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a13 = a13 \u2208 float</text>\n<text text-anchor=\"start\" x=\"68\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a14 = a14 \u2208 int</text>\n<text text-anchor=\"start\" x=\"68\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a15 = a15 \u2208 int</text>\n<text text-anchor=\"start\" x=\"68\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">a16 = a16 \u2208 int</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d0eef10>"
+                            "<graphviz.sources.Source at 0x7c1c9aec7bb0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_z_qz Pages: 1 -->\n",
-                            "<svg width=\"366pt\" height=\"125pt\"\n",
-                            " viewBox=\"0.00 0.00 366.05 124.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 120.8)\">\n",
-                            "<title>graph_z_qz</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-120.8 362.05,-120.8 362.05,4 -4,4\"/>\n",
-                            "<!-- graph_z_qz -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_z_qz</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M346.05,-116.8C346.05,-116.8 12,-116.8 12,-116.8 6,-116.8 0,-110.8 0,-104.8 0,-104.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 346.05,0 346.05,0 352.05,0 358.05,-6 358.05,-12 358.05,-12 358.05,-104.8 358.05,-104.8 358.05,-110.8 352.05,-116.8 346.05,-116.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"132.15\" y=\"-92.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">LOAN size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"128.77\" y=\"-81.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">loan_id = loan_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"110.77\" y=\"-70.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "<text text-anchor=\"start\" x=\"126.52\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"123.52\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">duration = duration \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"112.27\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">payments = payments \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"134.4\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">status = status \u2208 str</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_z_qz Pages: 1 -->\n<svg width=\"463pt\" height=\"124pt\"\n viewBox=\"0.00 0.00 463.00 124.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 120)\">\n<title>graph_z_qz</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-120 459,-120 459,4 -4,4\"/>\n<!-- graph_z_qz -->\n<g id=\"node1\" class=\"node\">\n<title>graph_z_qz</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M443,-116C443,-116 12,-116 12,-116 6,-116 0,-110 0,-104 0,-104 0,-12 0,-12 0,-6 6,0 12,0 12,0 443,0 443,0 449,0 455,-6 455,-12 455,-12 455,-104 455,-104 455,-110 449,-116 443,-116\"/>\n<text text-anchor=\"start\" x=\"165.5\" y=\"-94.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">LOAN size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"149\" y=\"-83.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">loan_id = loan_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"129\" y=\"-72.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n<text text-anchor=\"start\" x=\"156\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n<text text-anchor=\"start\" x=\"142.5\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">duration = duration \u2208 int</text>\n<text text-anchor=\"start\" x=\"135.5\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">payments = payments \u2208 float</text>\n<text text-anchor=\"start\" x=\"156\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">status = status \u2208 str</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d0eef10>"
+                            "<graphviz.sources.Source at 0x7c1c9bb229b0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_2ab8 Pages: 1 -->\n",
-                            "<svg width=\"176pt\" height=\"114pt\"\n",
-                            " viewBox=\"0.00 0.00 176.30 113.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 109.8)\">\n",
-                            "<title>graph_2ab8</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-109.8 172.3,-109.8 172.3,4 -4,4\"/>\n",
-                            "<!-- graph_2ab8 -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_2ab8</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M156.3,-105.8C156.3,-105.8 12,-105.8 12,-105.8 6,-105.8 0,-99.8 0,-93.8 0,-93.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 156.3,0 156.3,0 162.3,0 168.3,-6 168.3,-12 168.3,-12 168.3,-93.8 168.3,-93.8 168.3,-99.8 162.3,-105.8 156.3,-105.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"33.15\" y=\"-81.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">ORDER size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"28.65\" y=\"-70.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">order_id = order_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"15.9\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"29.78\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">bank_to = bank_to \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_to = account_to \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"26.4\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"23.03\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">k_symbol = k_symbol \u2208 str</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_2ab8 Pages: 1 -->\n<svg width=\"233pt\" height=\"113pt\"\n viewBox=\"0.00 0.00 233.00 113.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 109)\">\n<title>graph_2ab8</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-109 229,-109 229,4 -4,4\"/>\n<!-- graph_2ab8 -->\n<g id=\"node1\" class=\"node\">\n<title>graph_2ab8</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M213,-105C213,-105 12,-105 12,-105 6,-105 0,-99 0,-93 0,-93 0,-12 0,-12 0,-6 6,0 12,0 12,0 213,0 213,0 219,0 225,-6 225,-12 225,-12 225,-93 225,-93 225,-99 219,-105 213,-105\"/>\n<text text-anchor=\"start\" x=\"47.5\" y=\"-83.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">ORDER size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"27.5\" y=\"-72.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">order_id = order_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"34\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">bank_to = bank_to \u2208 str</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_to = account_to \u2208 int</text>\n<text text-anchor=\"start\" x=\"34\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 float</text>\n<text text-anchor=\"start\" x=\"27.5\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">k_symbol = k_symbol \u2208 str</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d0eef10>"
+                            "<graphviz.sources.Source at 0x7c1c9aec7bb0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_mpiu Pages: 1 -->\n",
-                            "<svg width=\"366pt\" height=\"158pt\"\n",
-                            " viewBox=\"0.00 0.00 366.05 157.80\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 153.8)\">\n",
-                            "<title>graph_mpiu</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-153.8 362.05,-153.8 362.05,4 -4,4\"/>\n",
-                            "<!-- graph_mpiu -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_mpiu</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M346.05,-149.8C346.05,-149.8 12,-149.8 12,-149.8 6,-149.8 0,-143.8 0,-137.8 0,-137.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 346.05,0 346.05,0 352.05,0 358.05,-6 358.05,-12 358.05,-12 358.05,-137.8 358.05,-137.8 358.05,-143.8 352.05,-149.8 346.05,-149.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"128.4\" y=\"-125.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">TRANS size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"126.52\" y=\"-114.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">trans_id = trans_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"110.77\" y=\"-103.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-92.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "<text text-anchor=\"start\" x=\"141.15\" y=\"-81.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">type = type \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"116.4\" y=\"-70.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">operation = operation \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"126.52\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"126.52\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">balance = balance \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"117.9\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">k_symbol = k_symbol \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"139.65\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">bank = bank \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"125.02\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account = account \u2208 int</text>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_mpiu Pages: 1 -->\n<svg width=\"463pt\" height=\"157pt\"\n viewBox=\"0.00 0.00 463.00 157.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 153)\">\n<title>graph_mpiu</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-153 459,-153 459,4 -4,4\"/>\n<!-- graph_mpiu -->\n<g id=\"node1\" class=\"node\">\n<title>graph_mpiu</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M443,-149C443,-149 12,-149 12,-149 6,-149 0,-143 0,-137 0,-137 0,-12 0,-12 0,-6 6,0 12,0 12,0 443,0 443,0 449,0 455,-6 455,-12 455,-12 455,-137 455,-137 455,-143 449,-149 443,-149\"/>\n<text text-anchor=\"start\" x=\"162.5\" y=\"-127.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">TRANS size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"142.5\" y=\"-116.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">trans_id = trans_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"129\" y=\"-105.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-94.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n<text text-anchor=\"start\" x=\"169.5\" y=\"-83.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">type = type \u2208 str</text>\n<text text-anchor=\"start\" x=\"135.5\" y=\"-72.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">operation = operation \u2208 str</text>\n<text text-anchor=\"start\" x=\"156\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n<text text-anchor=\"start\" x=\"149\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">balance = balance \u2208 int</text>\n<text text-anchor=\"start\" x=\"142.5\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">k_symbol = k_symbol \u2208 str</text>\n<text text-anchor=\"start\" x=\"169.5\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">bank = bank \u2208 str</text>\n<text text-anchor=\"start\" x=\"149\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account = account \u2208 int</text>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d0eef10>"
+                            "<graphviz.sources.Source at 0x7c1c9aec7bb0>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "import graphviz\n",
+                "from graphviz import Source\n",
                 "from IPython.display import display\n",
                 "\n",
                 "for path, relation in dataset.relations():\n",
-                "    display(graphviz.Source(relation.dot()))"
+                "    display(Source(relation.dot()))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "id": "309aa2b9",
-            "metadata": {},
+            "execution_count": 10,
+            "metadata": {
+                "colab": {
+                    "base_uri": "https://localhost:8080/",
+                    "height": 494
+                },
+                "id": "CZuSB9RkqTC9",
+                "outputId": "c3cf44ba-d7d6-4bbf-cb8c-04ebb152512a"
+            },
             "outputs": [
                 {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_ipd3 Pages: 1 -->\n",
-                            "<svg width=\"366pt\" height=\"317pt\"\n",
-                            " viewBox=\"0.00 0.00 366.05 317.40\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 313.4)\">\n",
-                            "<title>graph_ipd3</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-313.4 362.05,-313.4 362.05,4 -4,4\"/>\n",
-                            "<!-- graph_z_qz -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_z_qz</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M346.05,-116.8C346.05,-116.8 12,-116.8 12,-116.8 6,-116.8 0,-110.8 0,-104.8 0,-104.8 0,-12 0,-12 0,-6 6,0 12,0 12,0 346.05,0 346.05,0 352.05,0 358.05,-6 358.05,-12 358.05,-12 358.05,-104.8 358.05,-104.8 358.05,-110.8 352.05,-116.8 346.05,-116.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"132.15\" y=\"-92.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">LOAN size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"128.77\" y=\"-81.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">loan_id = loan_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"110.77\" y=\"-70.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "<text text-anchor=\"start\" x=\"126.52\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"123.52\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">duration = duration \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"112.27\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">payments = payments \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"134.4\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">status = status \u2208 str</text>\n",
-                            "</g>\n",
-                            "<!-- graph_x2u7 -->\n",
-                            "<g id=\"node2\" class=\"node\">\n",
-                            "<title>graph_x2u7</title>\n",
-                            "<path fill=\"#428e92\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M260.55,-207.6C260.55,-207.6 97.5,-207.6 97.5,-207.6 91.5,-207.6 85.5,-201.6 85.5,-195.6 85.5,-195.6 85.5,-157.8 85.5,-157.8 85.5,-151.8 91.5,-145.8 97.5,-145.8 97.5,-145.8 260.55,-145.8 260.55,-145.8 266.55,-145.8 272.55,-151.8 272.55,-157.8 272.55,-157.8 272.55,-195.6 272.55,-195.6 272.55,-201.6 266.55,-207.6 260.55,-207.6\"/>\n",
-                            "<text text-anchor=\"start\" x=\"117.52\" y=\"-183.75\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">MAP_4SGL size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"99.9\" y=\"-172.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_u1zo = (2 * payments) \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"113.02\" y=\"-161.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_kr4u = account_id \u2208 int</text>\n",
-                            "</g>\n",
-                            "<!-- graph_x2u7&#45;&gt;graph_z_qz -->\n",
-                            "<g id=\"edge1\" class=\"edge\">\n",
-                            "<title>graph_x2u7&#45;&gt;graph_z_qz</title>\n",
-                            "<path fill=\"none\" stroke=\"#2b303a\" d=\"M179.02,-145.45C179.02,-139.84 179.02,-133.78 179.02,-127.57\"/>\n",
-                            "<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"182.53,-128.01 179.02,-118.01 175.53,-128.01 182.53,-128.01\"/>\n",
-                            "</g>\n",
-                            "<!-- graph_ipd3 -->\n",
-                            "<g id=\"node3\" class=\"node\">\n",
-                            "<title>graph_ipd3</title>\n",
-                            "<path fill=\"#00363a\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M271.42,-309.4C271.42,-309.4 86.62,-309.4 86.62,-309.4 80.62,-309.4 74.62,-303.4 74.62,-297.4 74.62,-297.4 74.62,-248.6 74.62,-248.6 74.62,-242.6 80.62,-236.6 86.62,-236.6 86.62,-236.6 271.42,-236.6 271.42,-236.6 277.42,-236.6 283.42,-242.6 283.42,-248.6 283.42,-248.6 283.42,-297.4 283.42,-297.4 283.42,-303.4 277.42,-309.4 271.42,-309.4\"/>\n",
-                            "<text text-anchor=\"start\" x=\"106.65\" y=\"-285.55\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">REDUCE_HU6P size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"89.02\" y=\"-274.55\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">field_rif0 = sum(field_u1zo) \u2208 float{&#45;0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"90.52\" y=\"-263.55\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">field_sxga = count(field_kr4u) \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"122.77\" y=\"-252.55\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">GROUP BY (field_kr4u)</text>\n",
-                            "</g>\n",
-                            "<!-- graph_ipd3&#45;&gt;graph_x2u7 -->\n",
-                            "<g id=\"edge2\" class=\"edge\">\n",
-                            "<title>graph_ipd3&#45;&gt;graph_x2u7</title>\n",
-                            "<path fill=\"none\" stroke=\"#2b303a\" d=\"M179.02,-236.35C179.02,-230.63 179.02,-224.67 179.02,-218.83\"/>\n",
-                            "<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"182.53,-218.86 179.02,-208.86 175.53,-218.86 182.53,-218.86\"/>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_ipd3 Pages: 1 -->\n<svg width=\"463pt\" height=\"315pt\"\n viewBox=\"0.00 0.00 463.00 315.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 311)\">\n<title>graph_ipd3</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-311 459,-311 459,4 -4,4\"/>\n<!-- graph_z_qz -->\n<g id=\"node1\" class=\"node\">\n<title>graph_z_qz</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M443,-116C443,-116 12,-116 12,-116 6,-116 0,-110 0,-104 0,-104 0,-12 0,-12 0,-6 6,0 12,0 12,0 443,0 443,0 449,0 455,-6 455,-12 455,-12 455,-104 455,-104 455,-110 449,-116 443,-116\"/>\n<text text-anchor=\"start\" x=\"165.5\" y=\"-94.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">LOAN size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"149\" y=\"-83.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">loan_id = loan_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"129\" y=\"-72.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n<text text-anchor=\"start\" x=\"156\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n<text text-anchor=\"start\" x=\"142.5\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">duration = duration \u2208 int</text>\n<text text-anchor=\"start\" x=\"135.5\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">payments = payments \u2208 float</text>\n<text text-anchor=\"start\" x=\"156\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">status = status \u2208 str</text>\n</g>\n<!-- graph_x2u7 -->\n<g id=\"node2\" class=\"node\">\n<title>graph_x2u7</title>\n<path fill=\"#428e92\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M348.5,-206C348.5,-206 106.5,-206 106.5,-206 100.5,-206 94.5,-200 94.5,-194 94.5,-194 94.5,-157 94.5,-157 94.5,-151 100.5,-145 106.5,-145 106.5,-145 348.5,-145 348.5,-145 354.5,-145 360.5,-151 360.5,-157 360.5,-157 360.5,-194 360.5,-194 360.5,-200 354.5,-206 348.5,-206\"/>\n<text text-anchor=\"start\" x=\"152\" y=\"-184.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">MAP_4SGL size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"108.5\" y=\"-173.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_u1zo = (2 * payments) \u2208 float</text>\n<text text-anchor=\"start\" x=\"129\" y=\"-162.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_kr4u = account_id \u2208 int</text>\n</g>\n<!-- graph_x2u7&#45;&gt;graph_z_qz -->\n<g id=\"edge1\" class=\"edge\">\n<title>graph_x2u7&#45;&gt;graph_z_qz</title>\n<path fill=\"none\" stroke=\"#2b303a\" d=\"M227.5,-144.76C227.5,-138.97 227.5,-132.68 227.5,-126.23\"/>\n<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"231,-126.02 227.5,-116.02 224,-126.02 231,-126.02\"/>\n</g>\n<!-- graph_ipd3 -->\n<g id=\"node3\" class=\"node\">\n<title>graph_ipd3</title>\n<path fill=\"#00363a\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M365,-307C365,-307 90,-307 90,-307 84,-307 78,-301 78,-295 78,-295 78,-247 78,-247 78,-241 84,-235 90,-235 90,-235 365,-235 365,-235 371,-235 377,-241 377,-247 377,-247 377,-295 377,-295 377,-301 371,-307 365,-307\"/>\n<text text-anchor=\"start\" x=\"142\" y=\"-285.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">REDUCE_HU6P size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"92\" y=\"-274.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">field_rif0 = sum(field_u1zo) \u2208 float{&#45;0}</text>\n<text text-anchor=\"start\" x=\"95\" y=\"-263.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">field_sxga = count(field_kr4u) \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"156.5\" y=\"-252.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">GROUP BY (field_kr4u)</text>\n</g>\n<!-- graph_ipd3&#45;&gt;graph_x2u7 -->\n<g id=\"edge2\" class=\"edge\">\n<title>graph_ipd3&#45;&gt;graph_x2u7</title>\n<path fill=\"none\" stroke=\"#2b303a\" d=\"M227.5,-234.92C227.5,-228.88 227.5,-222.56 227.5,-216.4\"/>\n<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"231,-216.27 227.5,-206.27 224,-216.27 231,-216.27\"/>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d3f08e0>"
+                            "<graphviz.sources.Source at 0x7c1c7c7c8f10>"
                         ]
                     },
+                    "execution_count": 10,
                     "metadata": {},
-                    "output_type": "display_data"
+                    "output_type": "execute_result"
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Traceback (most recent call last):\n",
+                        "  File \"/usr/local/lib/python3.10/dist-packages/google/colab/_variable_inspector.py\", line 27, in run\n",
+                        "RuntimeError: pyqrlew::Relation is unsendbale, but is dropped on another thread!\n"
+                    ]
                 }
             ],
             "source": [
-                "result = dataset.sql('select sum(2*payments), count(account_id) from loan group by account_id')\n",
+                "result = dataset.sql('SELECT sum(2*payments), count(account_id) FROM loan GROUP BY account_id')\n",
                 "\n",
-                "display(graphviz.Source(result.dot()))"
+                "Source(result.dot())"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
-            "id": "e15b4384",
-            "metadata": {},
+            "execution_count": 11,
+            "metadata": {
+                "colab": {
+                    "base_uri": "https://localhost:8080/",
+                    "height": 852
+                },
+                "id": "878bVgORVinw",
+                "outputId": "248b3c74-8356-4203-8605-1ef20cdd30c2"
+            },
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Traceback (most recent call last):\n",
+                        "  File \"/usr/local/lib/python3.10/dist-packages/google/colab/_variable_inspector.py\", line 27, in run\n",
+                        "RuntimeError: pyqrlew::Relation is unsendbale, but is dropped on another thread!\n"
+                    ]
+                },
+                {
                     "data": {
-                        "image/svg+xml": [
-                            "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n",
-                            "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
-                            " \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
-                            "<!-- Generated by graphviz version 8.1.0 (20230707.0739)\n",
-                            " -->\n",
-                            "<!-- Title: graph_dxao Pages: 1 -->\n",
-                            "<svg width=\"738pt\" height=\"587pt\"\n",
-                            " viewBox=\"0.00 0.00 738.05 587.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n",
-                            "<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 583)\">\n",
-                            "<title>graph_dxao</title>\n",
-                            "<polygon fill=\"none\" stroke=\"none\" points=\"-4,4 -4,-583 734.05,-583 734.05,4 -4,4\"/>\n",
-                            "<!-- graph_agay -->\n",
-                            "<g id=\"node1\" class=\"node\">\n",
-                            "<title>graph_agay</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M346.05,-100.3C346.05,-100.3 12,-100.3 12,-100.3 6,-100.3 0,-94.3 0,-88.3 0,-88.3 0,-28.5 0,-28.5 0,-22.5 6,-16.5 12,-16.5 12,-16.5 346.05,-16.5 346.05,-16.5 352.05,-16.5 358.05,-22.5 358.05,-28.5 358.05,-28.5 358.05,-88.3 358.05,-88.3 358.05,-94.3 352.05,-100.3 346.05,-100.3\"/>\n",
-                            "<text text-anchor=\"start\" x=\"119.77\" y=\"-76.45\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">ACCOUNT size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"110.77\" y=\"-65.45\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"116.02\" y=\"-54.45\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"114.9\" y=\"-43.45\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">frequency = frequency \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"14.4\" y=\"-32.45\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "</g>\n",
-                            "<!-- graph_z_qz -->\n",
-                            "<g id=\"node2\" class=\"node\">\n",
-                            "<title>graph_z_qz</title>\n",
-                            "<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M718.05,-116.8C718.05,-116.8 384,-116.8 384,-116.8 378,-116.8 372,-110.8 372,-104.8 372,-104.8 372,-12 372,-12 372,-6 378,0 384,0 384,0 718.05,0 718.05,0 724.05,0 730.05,-6 730.05,-12 730.05,-12 730.05,-104.8 730.05,-104.8 730.05,-110.8 724.05,-116.8 718.05,-116.8\"/>\n",
-                            "<text text-anchor=\"start\" x=\"504.15\" y=\"-92.95\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">LOAN size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"500.77\" y=\"-81.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">loan_id = loan_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"482.77\" y=\"-70.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"386.4\" y=\"-59.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "<text text-anchor=\"start\" x=\"498.52\" y=\"-48.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"495.52\" y=\"-37.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">duration = duration \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"484.27\" y=\"-26.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">payments = payments \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"506.4\" y=\"-15.95\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">status = status \u2208 str</text>\n",
-                            "</g>\n",
-                            "<!-- graph_rrcy -->\n",
-                            "<g id=\"node3\" class=\"node\">\n",
-                            "<title>graph_rrcy</title>\n",
-                            "<path fill=\"#ff616f\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M563.92,-317.6C563.92,-317.6 166.12,-317.6 166.12,-317.6 160.12,-317.6 154.12,-311.6 154.12,-305.6 154.12,-305.6 154.12,-157.8 154.12,-157.8 154.12,-151.8 160.12,-145.8 166.12,-145.8 166.12,-145.8 563.92,-145.8 563.92,-145.8 569.92,-145.8 575.92,-151.8 575.92,-157.8 575.92,-157.8 575.92,-305.6 575.92,-305.6 575.92,-311.6 569.92,-317.6 563.92,-317.6\"/>\n",
-                            "<text text-anchor=\"start\" x=\"303.52\" y=\"-293.75\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">JOIN_PA9E size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"297.15\" y=\"-282.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_cybr = loan.loan_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"287.4\" y=\"-271.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_ubyc = loan.account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"179.4\" y=\"-260.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_i1ks = loan.date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "<text text-anchor=\"start\" x=\"293.77\" y=\"-249.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_0d45 = loan.amount \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"294.9\" y=\"-238.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_kni6 = loan.duration \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"287.02\" y=\"-227.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_yqki = loan.payments \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"299.4\" y=\"-216.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_vq3v = loan.status \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"279.52\" y=\"-205.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_e6qj = account.account_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"281.02\" y=\"-194.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_e_4y = account.district_id \u2208 int</text>\n",
-                            "<text text-anchor=\"start\" x=\"280.65\" y=\"-183.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_xxn6 = account.frequency \u2208 str</text>\n",
-                            "<text text-anchor=\"start\" x=\"168.52\" y=\"-172.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_t6ct = account.date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n",
-                            "<text text-anchor=\"start\" x=\"246.15\" y=\"-161.75\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">INNER ON (loan.account_id = account.account_id)</text>\n",
-                            "</g>\n",
-                            "<!-- graph_rrcy&#45;&gt;graph_agay -->\n",
-                            "<g id=\"edge2\" class=\"edge\">\n",
-                            "<title>graph_rrcy&#45;&gt;graph_agay</title>\n",
-                            "<path fill=\"none\" stroke=\"#2b303a\" d=\"M272.3,-145.3C258.28,-132.39 244.26,-119.48 231.5,-107.72\"/>\n",
-                            "<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"234.45,-105.77 224.73,-101.57 229.71,-110.92 234.45,-105.77\"/>\n",
-                            "</g>\n",
-                            "<!-- graph_rrcy&#45;&gt;graph_z_qz -->\n",
-                            "<g id=\"edge1\" class=\"edge\">\n",
-                            "<title>graph_rrcy&#45;&gt;graph_z_qz</title>\n",
-                            "<path fill=\"none\" stroke=\"#2b303a\" d=\"M457.75,-145.3C465.37,-138.28 472.99,-131.27 480.41,-124.43\"/>\n",
-                            "<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"482.39,-127.45 487.37,-118.1 477.64,-122.3 482.39,-127.45\"/>\n",
-                            "</g>\n",
-                            "<!-- graph_eprp -->\n",
-                            "<g id=\"node4\" class=\"node\">\n",
-                            "<title>graph_eprp</title>\n",
-                            "<path fill=\"#428e92\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M437.17,-408.4C437.17,-408.4 292.88,-408.4 292.88,-408.4 286.88,-408.4 280.88,-402.4 280.88,-396.4 280.88,-396.4 280.88,-358.6 280.88,-358.6 280.88,-352.6 286.88,-346.6 292.88,-346.6 292.88,-346.6 437.17,-346.6 437.17,-346.6 443.17,-346.6 449.17,-352.6 449.17,-358.6 449.17,-358.6 449.17,-396.4 449.17,-396.4 449.17,-402.4 443.17,-408.4 437.17,-408.4\"/>\n",
-                            "<text text-anchor=\"start\" x=\"303.52\" y=\"-384.55\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">MAP_M5F9 size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"295.27\" y=\"-373.55\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_weho = field_yqki \u2208 float</text>\n",
-                            "<text text-anchor=\"start\" x=\"297.52\" y=\"-362.55\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_w8w7 = field_e_4y \u2208 int</text>\n",
-                            "</g>\n",
-                            "<!-- graph_eprp&#45;&gt;graph_rrcy -->\n",
-                            "<g id=\"edge3\" class=\"edge\">\n",
-                            "<title>graph_eprp&#45;&gt;graph_rrcy</title>\n",
-                            "<path fill=\"none\" stroke=\"#2b303a\" d=\"M365.02,-346.35C365.02,-340.87 365.02,-334.88 365.02,-328.63\"/>\n",
-                            "<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"368.53,-328.87 365.02,-318.87 361.53,-328.87 368.53,-328.87\"/>\n",
-                            "</g>\n",
-                            "<!-- graph_e7j9 -->\n",
-                            "<g id=\"node5\" class=\"node\">\n",
-                            "<title>graph_e7j9</title>\n",
-                            "<path fill=\"#00363a\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M462.3,-499.2C462.3,-499.2 267.75,-499.2 267.75,-499.2 261.75,-499.2 255.75,-493.2 255.75,-487.2 255.75,-487.2 255.75,-449.4 255.75,-449.4 255.75,-443.4 261.75,-437.4 267.75,-437.4 267.75,-437.4 462.3,-437.4 462.3,-437.4 468.3,-437.4 474.3,-443.4 474.3,-449.4 474.3,-449.4 474.3,-487.2 474.3,-487.2 474.3,-493.2 468.3,-499.2 462.3,-499.2\"/>\n",
-                            "<text text-anchor=\"start\" x=\"292.27\" y=\"-475.35\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">REDUCE_4ADB size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"270.15\" y=\"-464.35\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">field_jkgw = sum(field_weho) \u2208 float{&#45;0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"305.77\" y=\"-453.35\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">GROUP BY (field_w8w7)</text>\n",
-                            "</g>\n",
-                            "<!-- graph_e7j9&#45;&gt;graph_eprp -->\n",
-                            "<g id=\"edge4\" class=\"edge\">\n",
-                            "<title>graph_e7j9&#45;&gt;graph_eprp</title>\n",
-                            "<path fill=\"none\" stroke=\"#2b303a\" d=\"M365.02,-437.24C365.02,-431.51 365.02,-425.43 365.02,-419.44\"/>\n",
-                            "<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"368.53,-419.83 365.02,-409.83 361.53,-419.83 368.53,-419.83\"/>\n",
-                            "</g>\n",
-                            "<!-- graph_dxao -->\n",
-                            "<g id=\"node6\" class=\"node\">\n",
-                            "<title>graph_dxao</title>\n",
-                            "<path fill=\"#428e92\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M457.8,-579C457.8,-579 272.25,-579 272.25,-579 266.25,-579 260.25,-573 260.25,-567 260.25,-567 260.25,-540.2 260.25,-540.2 260.25,-534.2 266.25,-528.2 272.25,-528.2 272.25,-528.2 457.8,-528.2 457.8,-528.2 463.8,-528.2 469.8,-534.2 469.8,-540.2 469.8,-540.2 469.8,-567 469.8,-567 469.8,-573 463.8,-579 457.8,-579\"/>\n",
-                            "<text text-anchor=\"start\" x=\"303.9\" y=\"-555.15\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">MAP_3SBU size \u2208 int{0}</text>\n",
-                            "<text text-anchor=\"start\" x=\"274.65\" y=\"-544.15\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_d37f = (2 * field_jkgw) \u2208 float{&#45;0}</text>\n",
-                            "</g>\n",
-                            "<!-- graph_dxao&#45;&gt;graph_e7j9 -->\n",
-                            "<g id=\"edge5\" class=\"edge\">\n",
-                            "<title>graph_dxao&#45;&gt;graph_e7j9</title>\n",
-                            "<path fill=\"none\" stroke=\"#2b303a\" d=\"M365.02,-528.06C365.02,-522.48 365.02,-516.4 365.02,-510.35\"/>\n",
-                            "<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"368.53,-510.57 365.02,-500.57 361.53,-510.57 368.53,-510.57\"/>\n",
-                            "</g>\n",
-                            "</g>\n",
-                            "</svg>\n"
-                        ],
+                        "image/svg+xml": "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>\n<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n<!-- Generated by graphviz version 2.43.0 (0)\n -->\n<!-- Title: graph_dxao Pages: 1 -->\n<svg width=\"932pt\" height=\"583pt\"\n viewBox=\"0.00 0.00 932.00 583.00\" xmlns=\"http://www.w3.org/2000/svg\" xmlns:xlink=\"http://www.w3.org/1999/xlink\">\n<g id=\"graph0\" class=\"graph\" transform=\"scale(1 1) rotate(0) translate(4 579)\">\n<title>graph_dxao</title>\n<polygon fill=\"transparent\" stroke=\"transparent\" points=\"-4,4 -4,-579 928,-579 928,4 -4,4\"/>\n<!-- graph_agay -->\n<g id=\"node1\" class=\"node\">\n<title>graph_agay</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M443,-99.5C443,-99.5 12,-99.5 12,-99.5 6,-99.5 0,-93.5 0,-87.5 0,-87.5 0,-28.5 0,-28.5 0,-22.5 6,-16.5 12,-16.5 12,-16.5 443,-16.5 443,-16.5 449,-16.5 455,-22.5 455,-28.5 455,-28.5 455,-87.5 455,-87.5 455,-93.5 449,-99.5 443,-99.5\"/>\n<text text-anchor=\"start\" x=\"155.5\" y=\"-77.7\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">ACCOUNT size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"129\" y=\"-66.7\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"122\" y=\"-55.7\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">district_id = district_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"135.5\" y=\"-44.7\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">frequency = frequency \u2208 str</text>\n<text text-anchor=\"start\" x=\"14\" y=\"-33.7\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n</g>\n<!-- graph_z_qz -->\n<g id=\"node2\" class=\"node\">\n<title>graph_z_qz</title>\n<path fill=\"#ff1744\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M912,-116C912,-116 481,-116 481,-116 475,-116 469,-110 469,-104 469,-104 469,-12 469,-12 469,-6 475,0 481,0 481,0 912,0 912,0 918,0 924,-6 924,-12 924,-12 924,-104 924,-104 924,-110 918,-116 912,-116\"/>\n<text text-anchor=\"start\" x=\"634.5\" y=\"-94.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">LOAN size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"618\" y=\"-83.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">loan_id = loan_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"598\" y=\"-72.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">account_id = account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"483\" y=\"-61.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">date = date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n<text text-anchor=\"start\" x=\"625\" y=\"-50.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">amount = amount \u2208 int</text>\n<text text-anchor=\"start\" x=\"611.5\" y=\"-39.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">duration = duration \u2208 int</text>\n<text text-anchor=\"start\" x=\"604.5\" y=\"-28.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">payments = payments \u2208 float</text>\n<text text-anchor=\"start\" x=\"625\" y=\"-17.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">status = status \u2208 str</text>\n</g>\n<!-- graph_rrcy -->\n<g id=\"node3\" class=\"node\">\n<title>graph_rrcy</title>\n<path fill=\"#ff616f\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M724,-316C724,-316 199,-316 199,-316 193,-316 187,-310 187,-304 187,-304 187,-157 187,-157 187,-151 193,-145 199,-145 199,-145 724,-145 724,-145 730,-145 736,-151 736,-157 736,-157 736,-304 736,-304 736,-310 730,-316 724,-316\"/>\n<text text-anchor=\"start\" x=\"383\" y=\"-294.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">JOIN_PA9E size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"356\" y=\"-283.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_cybr = loan.loan_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"346\" y=\"-272.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_ubyc = loan.account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"211\" y=\"-261.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_i1ks = loan.date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n<text text-anchor=\"start\" x=\"359.5\" y=\"-250.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_0d45 = loan.amount \u2208 int</text>\n<text text-anchor=\"start\" x=\"353\" y=\"-239.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_kni6 = loan.duration \u2208 int</text>\n<text text-anchor=\"start\" x=\"346\" y=\"-228.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_yqki = loan.payments \u2208 float</text>\n<text text-anchor=\"start\" x=\"359.5\" y=\"-217.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_vq3v = loan.status \u2208 str</text>\n<text text-anchor=\"start\" x=\"336\" y=\"-206.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_e6qj = account.account_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"332.5\" y=\"-195.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_e_4y = account.district_id \u2208 int</text>\n<text text-anchor=\"start\" x=\"339.5\" y=\"-184.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_xxn6 = account.frequency \u2208 str</text>\n<text text-anchor=\"start\" x=\"201\" y=\"-173.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_t6ct = account.date \u2208 datetime[0001&#45;01&#45;01 00:00:00 9999&#45;12&#45;31 00:00:00]</text>\n<text text-anchor=\"start\" x=\"302.5\" y=\"-162.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">INNER ON (loan.account_id = account.account_id)</text>\n</g>\n<!-- graph_rrcy&#45;&gt;graph_agay -->\n<g id=\"edge2\" class=\"edge\">\n<title>graph_rrcy&#45;&gt;graph_agay</title>\n<path fill=\"none\" stroke=\"#2b303a\" d=\"M345.53,-145C326.86,-131.4 308.16,-117.77 291.33,-105.51\"/>\n<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"293.36,-102.66 283.22,-99.6 289.24,-108.32 293.36,-102.66\"/>\n</g>\n<!-- graph_rrcy&#45;&gt;graph_z_qz -->\n<g id=\"edge1\" class=\"edge\">\n<title>graph_rrcy&#45;&gt;graph_z_qz</title>\n<path fill=\"none\" stroke=\"#2b303a\" d=\"M577.97,-145C588.62,-137.27 599.29,-129.53 609.62,-122.04\"/>\n<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"611.78,-124.79 617.82,-116.09 607.67,-119.13 611.78,-124.79\"/>\n</g>\n<!-- graph_eprp -->\n<g id=\"node4\" class=\"node\">\n<title>graph_eprp</title>\n<path fill=\"#428e92\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M569,-406C569,-406 354,-406 354,-406 348,-406 342,-400 342,-394 342,-394 342,-357 342,-357 342,-351 348,-345 354,-345 354,-345 569,-345 569,-345 575,-345 581,-351 581,-357 581,-357 581,-394 581,-394 581,-400 575,-406 569,-406\"/>\n<text text-anchor=\"start\" x=\"386\" y=\"-384.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">MAP_M5F9 size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"356\" y=\"-373.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_weho = field_yqki \u2208 float</text>\n<text text-anchor=\"start\" x=\"363\" y=\"-362.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_w8w7 = field_e_4y \u2208 int</text>\n</g>\n<!-- graph_eprp&#45;&gt;graph_rrcy -->\n<g id=\"edge3\" class=\"edge\">\n<title>graph_eprp&#45;&gt;graph_rrcy</title>\n<path fill=\"none\" stroke=\"#2b303a\" d=\"M461.5,-344.87C461.5,-339.23 461.5,-333.06 461.5,-326.6\"/>\n<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"465,-326.24 461.5,-316.24 458,-326.24 465,-326.24\"/>\n</g>\n<!-- graph_e7j9 -->\n<g id=\"node5\" class=\"node\">\n<title>graph_e7j9</title>\n<path fill=\"#00363a\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M599,-496C599,-496 324,-496 324,-496 318,-496 312,-490 312,-484 312,-484 312,-447 312,-447 312,-441 318,-435 324,-435 324,-435 599,-435 599,-435 605,-435 611,-441 611,-447 611,-447 611,-484 611,-484 611,-490 605,-496 599,-496\"/>\n<text text-anchor=\"start\" x=\"376\" y=\"-474.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">REDUCE_4ADB size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"326\" y=\"-463.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">field_jkgw = sum(field_weho) \u2208 float{&#45;0}</text>\n<text text-anchor=\"start\" x=\"390.5\" y=\"-452.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#ffffff\" fill-opacity=\"0.733333\">GROUP BY (field_w8w7)</text>\n</g>\n<!-- graph_e7j9&#45;&gt;graph_eprp -->\n<g id=\"edge4\" class=\"edge\">\n<title>graph_e7j9&#45;&gt;graph_eprp</title>\n<path fill=\"none\" stroke=\"#2b303a\" d=\"M461.5,-434.71C461.5,-428.83 461.5,-422.57 461.5,-416.42\"/>\n<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"465,-416.26 461.5,-406.26 458,-416.26 465,-416.26\"/>\n</g>\n<!-- graph_dxao -->\n<g id=\"node6\" class=\"node\">\n<title>graph_dxao</title>\n<path fill=\"#428e92\" stroke=\"#000000\" stroke-opacity=\"0.333333\" d=\"M602.5,-575C602.5,-575 320.5,-575 320.5,-575 314.5,-575 308.5,-569 308.5,-563 308.5,-563 308.5,-537 308.5,-537 308.5,-531 314.5,-525 320.5,-525 320.5,-525 602.5,-525 602.5,-525 608.5,-525 614.5,-531 614.5,-537 614.5,-537 614.5,-563 614.5,-563 614.5,-569 608.5,-575 602.5,-575\"/>\n<text text-anchor=\"start\" x=\"386\" y=\"-553.2\" font-family=\"Red Hat Display,sans-serif\" font-weight=\"bold\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">MAP_3SBU size \u2208 int{0}</text>\n<text text-anchor=\"start\" x=\"322.5\" y=\"-542.2\" font-family=\"Red Hat Display,sans-serif\" font-size=\"11.00\" fill=\"#000000\" fill-opacity=\"0.733333\">field_d37f = (2 * field_jkgw) \u2208 float{&#45;0}</text>\n</g>\n<!-- graph_dxao&#45;&gt;graph_e7j9 -->\n<g id=\"edge5\" class=\"edge\">\n<title>graph_dxao&#45;&gt;graph_e7j9</title>\n<path fill=\"none\" stroke=\"#2b303a\" d=\"M461.5,-524.69C461.5,-518.97 461.5,-512.72 461.5,-506.5\"/>\n<polygon fill=\"#2b303a\" stroke=\"#2b303a\" points=\"465,-506.18 461.5,-496.18 458,-506.18 465,-506.18\"/>\n</g>\n</g>\n</svg>\n",
                         "text/plain": [
-                            "<graphviz.sources.Source at 0x10d3f06d0>"
+                            "<graphviz.sources.Source at 0x7c1c7c7c8a60>"
                         ]
                     },
+                    "execution_count": 11,
                     "metadata": {},
-                    "output_type": "display_data"
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
-                "result = dataset.sql('select 2*sum(payments) from loan join account on loan.account_id=account.account_id group by district_id')\n",
+                "result = dataset.sql('SELECT 2*sum(payments) FROM loan join account ON loan.account_id=account.account_id GROUP BY district_id')\n",
                 "\n",
-                "display(graphviz.Source(result.dot()))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "cfeea0e5",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                " "
+                "Source(result.dot())"
             ]
         }
     ],
     "metadata": {
+        "colab": {
+            "gpuType": "T4",
+            "provenance": []
+        },
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
-            "language": "python",
+            "display_name": "Python 3",
             "name": "python3"
         },
         "language_info": {
-            "codemirror_mode": {
-                "name": "ipython",
-                "version": 3
-            },
-            "file_extension": ".py",
-            "mimetype": "text/x-python",
-            "name": "python",
-            "nbconvert_exporter": "python",
-            "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "name": "python"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 0
 }
```

### Comparing `pyqrlew-0.3.0/examples/demo/demo.ipynb` & `pyqrlew-0.3.1/examples/deprecated_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/pyproject.toml` & `pyqrlew-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/python/pyqrlew/io/database.py` & `pyqrlew-0.3.1/python/pyqrlew/io/database.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,307 +1,342 @@
+import logging
 from uuid import uuid4 as generate_uuid
 from typing import Optional
+import json
 from sqlalchemy import Engine, MetaData, Table, Column
 from sqlalchemy import types, select, func
+import pyqrlew as qrl
 
-def dataset_schema_size(name: str, engine: Engine, schema_name: Optional[str]=None) -> tuple[dict, dict, Optional[dict]]:
-    """Return a (dataset, schema) pair or (dataset, schema, size) triplet """
-    md = MetaData()
-    md.reflect(engine, schema=schema_name or name)
-    ds = dataset(name, md)
-    return (
-        ds,
-        schema(name, md, ds),
-        size(name, engine, ds, schema_name)
-    )
+def dataset(name: str, engine: Engine, schema_name: Optional[str]=None) -> qrl.Dataset:
+    metadata = MetaData()
+    schema = schema_name or name
+    metadata.reflect(engine, schema=schema)
 
-def dataset(name: str, metadata: MetaData) -> dict:
-    """Return a (dataset, schema) pair or (dataset, schema, size) triplet """
-    return {
-        '@type': 'sarus_data_spec/sarus_data_spec.Dataset',
-        'uuid': generate_uuid().hex,
-        'name': 'Transformed',
-        'spec': {
-            'transformed': {
-                'transform': generate_uuid().hex,
-                'arguments': [],
-                'named_arguments': {},
-            }
-        },
-        'properties': {},
-        'doc': 'This ia a demo dataset for testing purpose',
-    }
+    def _dataset_schema_size() -> tuple[dict, dict, Optional[dict]]:
+        """Return a (dataset, schema) pair or (dataset, schema, size) triplet """
+        ds = _dataset()
+        return (
+            ds,
+            _schema(ds),
+            _size(ds),
+        )
 
-def schema(name: str, metadata: MetaData, dataset: dict) -> dict:
-    return {
-        '@type': 'sarus_data_spec/sarus_data_spec.Schema',
-        'uuid': generate_uuid().hex,
-        'dataset': dataset['uuid'],
-        'name': name,
-        'type': {
-            # Slugname
-            'name': name.lower(),
-            'struct': {
-                'fields': [
-                    {
-                        'name': 'sarus_data',
-                        'type': {
-                            'name': 'Union',
-                            'union': {
-                                "fields": [table(metadata.tables[name]) for name in metadata.tables]
-                            },
-                            'properties': {
-                                'public_fields': '[]'
-                            },
-                        }
-                    },
-                    {
-                        'name': 'sarus_weights',
-                        'type': {
-                            'name': 'Integer',
-                            'integer': {
-                                'min': '-9223372036854775808',
-                                'max': '9223372036854775807',
-                                'base': 'INT64',
-                                'possible_values': []
-                            },
-                            'properties': {}
-                        }
-                    },
-                    {
-                        'name': 'sarus_is_public',
-                        'type': {
-                            'name': 'Boolean',
-                            'boolean': {},
-                            'properties': {}
-                        }
-                    },
-                    {
-                        'name': 'sarus_protected_entity',
-                        'type': {
-                            'name': 'Id',
-                            'id': {
-                                'base': 'STRING',
-                                'unique': False
-                            },
-                            'properties': {}
-                        }
-                    },
-                ],
-            },
-            'properties': {}
-        },
-        'protected': {
-            'label': 'data',
-            'paths': [],
-            'properties': {}
-        },
-        'properties': {
-            'max_max_multiplicity': '1',
-            'foreign_keys': '',
-            'primary_keys': '',
-        }
-    }
-
-def table(tab: Table) -> dict:
-    return {
-        'name': tab.name,
-        'type': {
-            'name': 'Struct',
-            'struct': {
-                'fields': [column(col) for col in tab.columns]
+    def _dataset() -> dict:
+        """Return a (dataset, schema) pair or (dataset, schema, size) triplet """
+        return {
+            '@type': 'sarus_data_spec/sarus_data_spec.Dataset',
+            'uuid': generate_uuid().hex,
+            'name': 'Transformed',
+            'spec': {
+                'transformed': {
+                    'transform': generate_uuid().hex,
+                    'arguments': [],
+                    'named_arguments': {},
+                },
             },
             'properties': {},
+            'doc': 'This ia a demo dataset for testing purpose',
         }
-    }
 
-def column(col: Column) -> dict:
-    if isinstance(col.type, types.Integer) or isinstance(col.type, types.BigInteger):
+    def _schema(dataset: dict) -> dict:
         return {
-            'name': col.name,
+            '@type': 'sarus_data_spec/sarus_data_spec.Schema',
+            'uuid': generate_uuid().hex,
+            'dataset': dataset['uuid'],
+            'name': name,
             'type': {
-                'name': 'Integer',
-                'integer': {
-                    'base': 'INT64',
-                    'min': '-9223372036854775808',
-                    'max': '9223372036854775807',
-                    'possible_values': []
+                # Slugname
+                'name': name.lower(),
+                'struct': {
+                    'fields': [
+                        {
+                            'name': 'sarus_data',
+                            'type': {
+                                'name': 'Union',
+                                'union': {
+                                    "fields": [{
+                                        'name': schema,
+                                        'type': {
+                                            'name': 'Union',
+                                            'union': {
+                                                "fields": [_table(metadata.tables[name]) for name in metadata.tables]
+                                            },
+                                            'properties': {
+                                                'public_fields': '[]'
+                                            },
+                                        }
+                                    }],
+                                },
+                                'properties': {
+                                    'public_fields': '[]',
+                                },
+                            },
+                        },
+                        {
+                            'name': 'sarus_weights',
+                            'type': {
+                                'name': 'Integer',
+                                'integer': {
+                                    'min': '-9223372036854775808',
+                                    'max': '9223372036854775807',
+                                    'base': 'INT64',
+                                    'possible_values': []
+                                },
+                                'properties': {}
+                            },
+                        },
+                        {
+                            'name': 'sarus_is_public',
+                            'type': {
+                                'name': 'Boolean',
+                                'boolean': {},
+                                'properties': {},
+                            },
+                        },
+                        {
+                            'name': 'sarus_protected_entity',
+                            'type': {
+                                'name': 'Id',
+                                'id': {
+                                    'base': 'STRING',
+                                    'unique': False,
+                                },
+                                'properties': {},
+                            },
+                        },
+                    ],
                 },
+                'properties': {}
+            },
+            'protected': {
+                'label': 'data',
+                'paths': [],
                 'properties': {},
+            },
+            'properties': {
+                'max_max_multiplicity': '1',
+                'foreign_keys': '',
+                'primary_keys': '',
             }
         }
-    elif isinstance(col.type, types.Float) or isinstance(col.type, types.Numeric):
+
+    def _table(tab: Table) -> dict:
         return {
-            'name': col.name,
+            'name': tab.name,
             'type': {
-                'name': 'Float64',
-                'float': {
-                    'base': 'FLOAT64',
-                    'min': '-1.7976931348623157e+308',
-                    'max': '1.7976931348623157e+308',
-                    'possible_values': []
+                'name': 'Struct',
+                'struct': {
+                    'fields': [_column(col) for col in tab.columns],
                 },
                 'properties': {},
             }
         }
-    elif isinstance(col.type, types.String) or isinstance(col.type, types.Text) or isinstance(col.type, types.Unicode) or isinstance(col.type, types.UnicodeText):
-        return {
-            'name': col.name,
-            'type': {
-                'name': 'Text UTF-8',
-                'text': {
-                    'encoding': 'UTF-8'
+
+    def _column(col: Column) -> dict:
+        if isinstance(col.type, types.Integer) or isinstance(col.type, types.BigInteger):
+            return {
+                'name': col.name,
+                'type': {
+                    'name': 'Integer',
+                    'integer': {
+                        'base': 'INT64',
+                        'min': '-9223372036854775808',
+                        'max': '9223372036854775807',
+                        'possible_values': [],
+                    },
+                    'properties': {},
                 },
-                'properties': {},
             }
-        }
-    elif isinstance(col.type, types.Boolean):
-        return {
-            'name': col.name,
-            'type': {
-                'name': 'Boolean',
-                'boolean': {},
-                'properties': {},
+        elif isinstance(col.type, types.Float) or isinstance(col.type, types.Numeric):
+            return {
+                'name': col.name,
+                'type': {
+                    'name': 'Float64',
+                    'float': {
+                        'base': 'FLOAT64',
+                        'min': '-1.7976931348623157e+308',
+                        'max': '1.7976931348623157e+308',
+                        'possible_values': [],
+                    },
+                    'properties': {},
+                },
             }
-        }
-    elif isinstance(col.type, types.Date) or isinstance(col.type, types.DateTime) or isinstance(col.type, types.Time):
-        return {
-            'name': col.name,
-            'type': {
-                'name': 'Datetime',
-                'datetime': {
-                    'format': '%Y-%m-%d %H:%M:%S',
-                    'min': '01-01-01 00:00:00',
-                    'max': '9999-12-31 00:00:00',
+        elif isinstance(col.type, types.String) or isinstance(col.type, types.Text) or isinstance(col.type, types.Unicode) or isinstance(col.type, types.UnicodeText):
+            return {
+                'name': col.name,
+                'type': {
+                    'name': 'Text UTF-8',
+                    'text': {
+                        'encoding': 'UTF-8'
+                    },
+                    'properties': {},
                 },
-                'properties': {},
             }
-        }
-    else:
-        return {
-            'name': col.name,
-            'type': {
-                'name': 'Type',
-                'type': {},
-                'properties': {},
+        elif isinstance(col.type, types.Boolean):
+            return {
+                'name': col.name,
+                'type': {
+                    'name': 'Boolean',
+                    'boolean': {},
+                    'properties': {},
+                },
+            }
+        elif isinstance(col.type, types.Date) or isinstance(col.type, types.DateTime) or isinstance(col.type, types.Time):
+            return {
+                'name': col.name,
+                'type': {
+                    'name': 'Datetime',
+                    'datetime': {
+                        'format': '%Y-%m-%d %H:%M:%S',
+                        'min': '01-01-01 00:00:00',
+                        'max': '9999-12-31 00:00:00',
+                    },
+                    'properties': {},
+                },
+            }
+        else:
+            return {
+                'name': col.name,
+                'type': {
+                    'name': 'Type',
+                    'type': {},
+                    'properties': {},
+                },
             }
-        }
-
-def size(name: str, engine: Engine, dataset: dict, schema_name: Optional[str]=None) -> dict:
-    md = MetaData()
-    md.reflect(engine, schema=schema_name or name)
-    return {
-        '@type': 'sarus_data_spec/sarus_data_spec.Size',
-        'uuid': generate_uuid().hex,
-        'dataset': dataset['uuid'],
-        'name': f'{name}_sizes',
-        'statistics': {
-            'name': 'Union',
-            'union': {
-                "fields": [table_size(engine, md.tables[name]) for name in md.tables]
-            },
-            'properties': {}
-        },
-        'properties': {}
-    }
 
-def table_size(engine: Engine, tab: Table) -> dict:
-    with engine.connect() as conn:
-        result = conn.execute(select(func.count()).select_from(tab))
-        size = result.scalar()
-    multiplicity = 1.0
-    return {
-        'name': tab.name,
-        'statistics': {
-            'name': 'Struct',
-            'size': str(size),
-            'multiplicity': multiplicity,
-            'struct': {
-                'fields': [column_size(col, size, multiplicity) for col in tab.columns]
+    def _size(dataset: dict) -> dict:
+        return {
+            '@type': 'sarus_data_spec/sarus_data_spec.Size',
+            'uuid': generate_uuid().hex,
+            'dataset': dataset['uuid'],
+            'name': f'{name}_sizes',
+            'statistics': {
+                'name': 'Union',
+                'union': {
+                    'fields': [
+                        {
+                            'name': schema,
+                            'statistics': {
+                                'name': 'Union',
+                                'union': {
+                                    'fields': [_table_size(metadata.tables[name]) for name in metadata.tables]
+                                },
+                                'properties': {},
+                            },
+                            'properties': {},
+                        },
+                    ],
+                },
+                'properties': {},
             },
             'properties': {},
         }
-    }
 
-def column_size(col: Column, size: int, multiplicity: float) -> dict:
-    if isinstance(col.type, types.Integer) or isinstance(col.type, types.BigInteger):
+    def _table_size(tab: Table) -> dict:
+        with engine.connect() as conn:
+            result = conn.execute(select(func.count()).select_from(tab))
+            size = result.scalar()
+        multiplicity = 1.0
         return {
-            'name': col.name,
+            'name': tab.name,
             'statistics': {
-                'name': 'Integer',
+                'name': 'Struct',
                 'size': str(size),
                 'multiplicity': multiplicity,
-                'integer': {
-                    'base': 'INT64',
-                    'min': '-9223372036854775808',
-                    'max': '9223372036854775807',
-                    'possible_values': []
+                'struct': {
+                    'fields': [_column_size(col, size, multiplicity) for col in tab.columns],
                 },
                 'properties': {},
             }
         }
-    elif isinstance(col.type, types.Float) or isinstance(col.type, types.Numeric):
-        return {
-            'name': col.name,
-            'statistics': {
-                'name': 'Float64',
-                'size': str(size),
-                'multiplicity': multiplicity,
-                'float': {
-                    'base': 'FLOAT64',
-                    'min': '-1.7976931348623157e+308',
-                    'max': '1.7976931348623157e+308',
-                    'possible_values': []
+
+    def _column_size(col: Column, size: int, multiplicity: float) -> dict:
+        if isinstance(col.type, types.Integer) or isinstance(col.type, types.BigInteger):
+            return {
+                'name': col.name,
+                'statistics': {
+                    'name': 'Integer',
+                    'size': str(size),
+                    'multiplicity': multiplicity,
+                    'integer': {
+                        'base': 'INT64',
+                        'min': '-9223372036854775808',
+                        'max': '9223372036854775807',
+                        'possible_values': []
+                    },
+                    'properties': {},
                 },
-                'properties': {},
             }
-        }
-    elif isinstance(col.type, types.String) or isinstance(col.type, types.Text) or isinstance(col.type, types.Unicode) or isinstance(col.type, types.UnicodeText):
-        return {
-            'name': col.name,
-            'statistics': {
-                'name': 'Text UTF-8',
-                'size': str(size),
-                'multiplicity': multiplicity,
-                'text': {
-                    'encoding': 'UTF-8'
+        elif isinstance(col.type, types.Float) or isinstance(col.type, types.Numeric):
+            return {
+                'name': col.name,
+                'statistics': {
+                    'name': 'Float64',
+                    'size': str(size),
+                    'multiplicity': multiplicity,
+                    'float': {
+                        'base': 'FLOAT64',
+                        'min': '-1.7976931348623157e+308',
+                        'max': '1.7976931348623157e+308',
+                        'possible_values': [],
+                    },
+                    'properties': {},
+                }
+            }
+        elif isinstance(col.type, types.String) or isinstance(col.type, types.Text) or isinstance(col.type, types.Unicode) or isinstance(col.type, types.UnicodeText):
+            return {
+                'name': col.name,
+                'statistics': {
+                    'name': 'Text UTF-8',
+                    'size': str(size),
+                    'multiplicity': multiplicity,
+                    'text': {
+                        'encoding': 'UTF-8',
+                    },
+                    'properties': {},
                 },
-                'properties': {},
             }
-        }
-    elif isinstance(col.type, types.Boolean):
-        return {
-            'name': col.name,
-            'statistics': {
-                'name': 'Boolean',
-                'size': str(size),
-                'multiplicity': multiplicity,
-                'boolean': {},
-                'properties': {},
+        elif isinstance(col.type, types.Boolean):
+            return {
+                'name': col.name,
+                'statistics': {
+                    'name': 'Boolean',
+                    'size': str(size),
+                    'multiplicity': multiplicity,
+                    'boolean': {},
+                    'properties': {},
+                },
             }
-        }
-    elif isinstance(col.type, types.Date) or isinstance(col.type, types.DateTime) or isinstance(col.type, types.Time):
-        return {
-            'name': col.name,
-            'statistics': {
-                'name': 'Datetime',
-                'size': str(size),
-                'multiplicity': multiplicity,
-                'datetime': {
-                    'format': '%Y-%m-%d %H:%M:%S',
-                    'min': '01-01-01 00:00:00',
-                    'max': '9999-12-31 00:00:00',
+        elif isinstance(col.type, types.Date) or isinstance(col.type, types.DateTime) or isinstance(col.type, types.Time):
+            return {
+                'name': col.name,
+                'statistics': {
+                    'name': 'Datetime',
+                    'size': str(size),
+                    'multiplicity': multiplicity,
+                    'datetime': {
+                        'format': '%Y-%m-%d %H:%M:%S',
+                        'min': '01-01-01 00:00:00',
+                        'max': '9999-12-31 00:00:00',
+                    },
+                    'properties': {},
                 },
-                'properties': {},
             }
-        }
-    else:
-        return {
-            'name': col.name,
-            'statistics': {
-                'name': 'Type',
-                'size': str(size),
-                'multiplicity': multiplicity,
-                'type': {},
-                'properties': {},
+        else:
+            return {
+                'name': col.name,
+                'statistics': {
+                    'name': 'Type',
+                    'size': str(size),
+                    'multiplicity': multiplicity,
+                    'type': {},
+                    'properties': {},
+                },
             }
-        }
+    # Gather protobufs
+    dataset, schema, size = _dataset_schema_size()
+    # Display when debugging
+    logging.debug(json.dumps(dataset))
+    logging.debug(json.dumps(schema))
+    logging.debug(json.dumps(size))
+    # Return the result
+    return qrl.Dataset(json.dumps(dataset), json.dumps(schema), json.dumps(size))
```

### Comparing `pyqrlew-0.3.0/python/pyqrlew/io/postgresql.py` & `pyqrlew-0.3.1/python/pyqrlew/io/postgresql.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import shutil
 from pathlib import Path
 import importlib.resources as pkg_resources
 import json
 import logging
-from sqlalchemy import MetaData, Engine, exists, select, column, table, text
+from sqlalchemy import MetaData, Engine, exists, select, column, table, text, Result
 from datasets import sources
 from datasets.databases import PostgreSQL as EmptyPostgreSQL
-from pyqrlew.io.database import dataset_schema_size
+from pyqrlew.io.database import dataset
 import pyqrlew as qrl
 
 NAME: str = 'pyqrlew-db'
 USER: str = 'postgres'
 PASSWORD: str = 'pyqrlew-db'
 PORT: str = 5433
 
@@ -38,24 +38,25 @@
         return self.load_resource('hepatitis_std', pkg_resources.files(sources) / 'hepatitis' / 'Hepatitis_std.sql')
 
     def load_imdb(self) -> 'PostgreSQL':
         return self.load_resource('imdb_ijs', pkg_resources.files(sources) / 'imdb' / 'imdb_ijs.sql')
     
     def extract(self) -> qrl.Dataset:
         self.load_extract()
-        dataset, schema, size = dataset_schema_size('extract', self.engine())
-        return qrl.Dataset(json.dumps(dataset), json.dumps(schema), json.dumps(size))
+        return dataset('extract', self.engine())
     
     def financial(self) -> qrl.Dataset:
         self.load_financial()
-        dataset, schema, size = dataset_schema_size('financial', self.engine())
-        return qrl.Dataset(json.dumps(dataset), json.dumps(schema), json.dumps(size))
+        return dataset('financial', self.engine())
     
     def hepatitis(self) -> qrl.Dataset:
         self.load_hepatitis()
-        dataset, schema, size = dataset_schema_size('hepatitis_std', self.engine())
-        return qrl.Dataset(json.dumps(dataset), json.dumps(schema), json.dumps(size))
+        return dataset('hepatitis_std', self.engine())
 
     def imdb(self) -> qrl.Dataset:
         self.load_imdb()
-        dataset, schema, size = dataset_schema_size('imdb_ijs', self.engine())
-        return qrl.Dataset(json.dumps(dataset), json.dumps(schema), json.dumps(size))
+        return dataset('imdb_ijs', self.engine())
+
+    def eval(self, relation: qrl.Relation) -> list:
+        with self.engine().connect() as conn:
+            result = conn.execute(text(relation.render())).all()
+        return result
```

### Comparing `pyqrlew-0.3.0/tests/queries/sql_unlimited_queries.sql` & `pyqrlew-0.3.1/tests/queries/sql_unlimited_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/tests/queries/valid_queries.sql` & `pyqrlew-0.3.1/tests/queries/valid_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.0/tests/test_financial_dataset.py` & `pyqrlew-0.3.1/tests/test_extract_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     dataset: qrl.Dataset,
     connection: Connection,
     query: str
 ) -> None:
     result = execute_query(connection, query)
     rel = dataset.sql(query)
     new_query = rel.render()
+    print(f'DEBUG {new_query}')
     print(f"{query}->{new_query}")
     try:
         result2 = execute_query(connection, new_query)
     except TypeError as e:
         print(
             f"Sending {new_query} \nfailed with error:\n{e}"
         )
```

### Comparing `pyqrlew-0.3.0/Cargo.lock` & `pyqrlew-0.3.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1018,27 +1018,27 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyqrlew"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "pyo3",
  "qrlew",
  "qrlew-sarus",
  "serde_json",
 ]
 
 [[package]]
 name = "qrlew"
-version = "0.1.9"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b4449f36c9565aa300af891c90997d5440eafe4a00c93d8d6870e585cbc832a"
+checksum = "0726d200fbf67a1a954924d5feb613847a3fc317b9e1552a08e312752940a484"
 dependencies = [
  "base64",
  "chrono",
  "colored",
  "dot",
  "env_logger",
  "itertools",
@@ -1051,17 +1051,17 @@
  "serde_json",
  "sqlparser",
  "statrs",
 ]
 
 [[package]]
 name = "qrlew-sarus"
-version = "0.2.2"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53055cfd1efb7aeeb2ad31ddefe40d661cf778fa44b92e8ddaa8b55930b38e52"
+checksum = "c2fc630e36f960672eb517862ae58ef5c881808505cc7b087814f61ecf587b12"
 dependencies = [
  "anyhow",
  "chrono",
  "colored",
  "env_logger",
  "glob",
  "itertools",
@@ -1369,17 +1369,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "sqlparser"
-version = "0.35.0"
+version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca597d77c98894be1f965f2e4e2d2a61575d4998088e655476c73715c54b2b43"
+checksum = "2eaa1e88e78d2c2460d78b7dc3f0c08dbb606ab4222f9aff36f420d36e307d87"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "statrs"
 version = "0.16.0"
```

### Comparing `pyqrlew-0.3.0/PKG-INFO` & `pyqrlew-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqrlew
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: SQLAlchemy ~= 2.0
 Requires-Dist: psycopg[binary, pool] ~= 3.0
 Requires-Dist: pymysql ~= 1.0
 Requires-Dist: qrlew-datasets ~= 0.3.0
@@ -13,18 +13,18 @@
 Provides-Extra: test
 License-File: LICENSE
 Summary: A library to manipulate SQL queries, designed with privacy application in mind.
 Keywords: SQL,Privecy,Differential Privacy,AST,Intermediate Representation,Rust
 Author-email: Nicolas Grislain <ng@sarus.tech>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/Qrlew/pyqrlew
-Project-URL: homepage, https://qrlew.github.io
 Project-URL: documentation, https://pyqrlew.readthedocs.io
 Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
+Project-URL: homepage, https://qrlew.github.io
+Project-URL: repository, https://github.com/Qrlew/pyqrlew
 
 # [Qrlew](https://qrlew.github.io/) framework (by [Sarus](https://www.sarus.tech/))
 Open source SQL manipulation framework written in Rust
 
 ## What is [Qrlew](https://qrlew.github.io/)?
 [Qrlew](https://qrlew.github.io/) is an open source library that aims to parse and compile SQL queries into an Intermediate Representation (IR) that is well-suited for various rewriting tasks. Although it was originally designed for privacy-focused applications, it can be utilized for a wide range of purposes.
```

