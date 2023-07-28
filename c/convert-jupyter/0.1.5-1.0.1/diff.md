# Comparing `tmp/convert_jupyter-0.1.5.tar.gz` & `tmp/convert_jupyter-1.0.1.tar.gz`

## Comparing `convert_jupyter-0.1.5.tar` & `convert_jupyter-1.0.1.tar`

### file list

```diff
@@ -1,800 +1,29 @@
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.pylintrc
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/Makefile
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/lint.sh
--rw-r--r--   0        0        0    22675 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/poetry.lock
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/upload.sh
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/@plugins_snapshot.json
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/__future__.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/__future__.meta.json
--rw-r--r--   0        0        0   113330 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_ast.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_ast.meta.json
--rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_bisect.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_bisect.meta.json
--rw-r--r--   0        0        0    50980 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_codecs.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_codecs.meta.json
--rw-r--r--   0        0        0    10028 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_collections_abc.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_collections_abc.meta.json
--rw-r--r--   0        0        0   166299 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_decimal.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_decimal.meta.json
--rw-r--r--   0        0        0   110535 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_operator.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_operator.meta.json
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_random.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_random.meta.json
--rw-r--r--   0        0        0   135728 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_socket.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_socket.meta.json
--rw-r--r--   0        0        0    20534 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_stat.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_stat.meta.json
--rw-r--r--   0        0        0    23593 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_thread.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_thread.meta.json
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_tracemalloc.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_tracemalloc.meta.json
--rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_warnings.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_warnings.meta.json
--rw-r--r--   0        0        0    26629 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_weakref.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_weakref.meta.json
--rw-r--r--   0        0        0    46032 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_weakrefset.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_weakrefset.meta.json
--rw-r--r--   0        0        0    19399 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/abc.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/abc.meta.json
--rw-r--r--   0        0        0   148628 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/argparse.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/argparse.meta.json
--rw-r--r--   0        0        0    63508 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/array.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/array.meta.json
--rw-r--r--   0        0        0   119539 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/ast.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/ast.meta.json
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/atexit.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/atexit.meta.json
--rw-r--r--   0        0        0    50413 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/bdb.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/bdb.meta.json
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/bisect.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/bisect.meta.json
--rw-r--r--   0        0        0   960702 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/builtins.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/builtins.meta.json
--rw-r--r--   0        0        0    20588 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/cmd.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/cmd.meta.json
--rw-r--r--   0        0        0   119849 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/codecs.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/codecs.meta.json
--rw-r--r--   0        0        0    86397 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/contextlib.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/contextlib.meta.json
--rw-r--r--   0        0        0    36734 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/contextvars.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/contextvars.meta.json
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert.meta.json
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/copy.data.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/copy.meta.json
--rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/copyreg.data.json
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/copyreg.meta.json
--rw-r--r--   0        0        0    48110 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/dataclasses.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/dataclasses.meta.json
--rw-r--r--   0        0        0   126737 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/datetime.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/datetime.meta.json
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/decimal.data.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/decimal.meta.json
--rw-r--r--   0        0        0    58050 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/difflib.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/difflib.meta.json
--rw-r--r--   0        0        0    42024 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/dis.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/dis.meta.json
--rw-r--r--   0        0        0    78210 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/doctest.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/doctest.meta.json
--rw-r--r--   0        0        0    61118 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/enum.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/enum.meta.json
--rw-r--r--   0        0        0    29754 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/errno.data.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/errno.meta.json
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/fnmatch.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/fnmatch.meta.json
--rw-r--r--   0        0        0    91152 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/fractions.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/fractions.meta.json
--rw-r--r--   0        0        0   125793 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/functools.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/functools.meta.json
--rw-r--r--   0        0        0    15373 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/gc.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/gc.meta.json
--rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/genericpath.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/genericpath.meta.json
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/getpass.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/getpass.meta.json
--rw-r--r--   0        0        0    52298 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/gettext.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/gettext.meta.json
--rw-r--r--   0        0        0     9220 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/glob.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/glob.meta.json
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/hashlib.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/hashlib.meta.json
--rw-r--r--   0        0        0   303266 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/inspect.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/inspect.meta.json
--rw-r--r--   0        0        0    86134 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/io.data.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/io.meta.json
--rw-r--r--   0        0        0   254143 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/itertools.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/itertools.meta.json
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/keyword.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/keyword.meta.json
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/marshal.data.json
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/marshal.meta.json
--rw-r--r--   0        0        0    37325 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/math.data.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/math.meta.json
--rw-r--r--   0        0        0    28029 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/mmap.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/mmap.meta.json
--rw-r--r--   0        0        0    78458 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numbers.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numbers.meta.json
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/opcode.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/opcode.meta.json
--rw-r--r--   0        0        0    50001 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/operator.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/operator.meta.json
--rw-r--r--   0        0        0    83871 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pathlib.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pathlib.meta.json
--rw-r--r--   0        0        0    93929 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pdb.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pdb.meta.json
--rw-r--r--   0        0        0    47454 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pickle.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pickle.meta.json
--rw-r--r--   0        0        0    31602 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pkgutil.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pkgutil.meta.json
--rw-r--r--   0        0        0    34351 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/platform.data.json
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/platform.meta.json
--rw-r--r--   0        0        0    77460 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/posixpath.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/posixpath.meta.json
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pprint.data.json
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pprint.meta.json
--rw-r--r--   0        0        0    28857 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/queue.data.json
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/queue.meta.json
--rw-r--r--   0        0        0    41558 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/random.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/random.meta.json
--rw-r--r--   0        0        0    54778 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/re.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/re.meta.json
--rw-r--r--   0        0        0    17273 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/reprlib.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/reprlib.meta.json
--rw-r--r--   0        0        0    68434 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/selectors.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/selectors.meta.json
--rw-r--r--   0        0        0    16338 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/shlex.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/shlex.meta.json
--rw-r--r--   0        0        0    70263 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/shutil.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/shutil.meta.json
--rw-r--r--   0        0        0    48665 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/signal.data.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/signal.meta.json
--rw-r--r--   0        0        0   108997 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/socket.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/socket.meta.json
--rw-r--r--   0        0        0    14947 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sre_compile.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sre_compile.meta.json
--rw-r--r--   0        0        0    29612 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sre_constants.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sre_constants.meta.json
--rw-r--r--   0        0        0    51529 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sre_parse.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sre_parse.meta.json
--rw-r--r--   0        0        0   184743 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/ssl.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/ssl.meta.json
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/stat.data.json
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/stat.meta.json
--rw-r--r--   0        0        0    17861 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/string.data.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/string.meta.json
--rw-r--r--   0        0        0    13620 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/struct.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/struct.meta.json
--rw-r--r--   0        0        0   146151 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/subprocess.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/subprocess.meta.json
--rw-r--r--   0        0        0   137539 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sys.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sys.meta.json
--rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sysconfig.data.json
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/sysconfig.meta.json
--rw-r--r--   0        0        0   112058 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tempfile.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tempfile.meta.json
--rw-r--r--   0        0        0    19924 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/textwrap.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/textwrap.meta.json
--rw-r--r--   0        0        0    67700 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/threading.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/threading.meta.json
--rw-r--r--   0        0        0    42510 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/time.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/time.meta.json
--rw-r--r--   0        0        0    15863 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/token.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/token.meta.json
--rw-r--r--   0        0        0    52181 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tokenize.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tokenize.meta.json
--rw-r--r--   0        0        0    46048 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/traceback.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/traceback.meta.json
--rw-r--r--   0        0        0    47219 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tracemalloc.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tracemalloc.meta.json
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/try2.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/try2.meta.json
--rw-r--r--   0        0        0   228259 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/types.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/types.meta.json
--rw-r--r--   0        0        0   491732 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/typing.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/typing.meta.json
--rw-r--r--   0        0        0    59648 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/typing_extensions.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/typing_extensions.meta.json
--rw-r--r--   0        0        0    23245 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unicodedata.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unicodedata.meta.json
--rw-r--r--   0        0        0    33144 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/uuid.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/uuid.meta.json
--rw-r--r--   0        0        0    23407 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/warnings.data.json
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/warnings.meta.json
--rw-r--r--   0        0        0   102725 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/weakref.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/weakref.meta.json
--rw-r--r--   0        0        0    68595 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/zipfile.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/zipfile.meta.json
--rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/zipimport.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/zipimport.meta.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/__init__.data.json
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/__init__.meta.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_argcomplete.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_argcomplete.meta.json
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_version.data.json
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_version.meta.json
--rw-r--r--   0        0        0    45151 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/cacheprovider.data.json
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/cacheprovider.meta.json
--rw-r--r--   0        0        0   115600 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/capture.data.json
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/capture.meta.json
--rw-r--r--   0        0        0    28039 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/compat.data.json
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/compat.meta.json
--rw-r--r--   0        0        0    30467 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/debugging.data.json
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/debugging.meta.json
--rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/deprecated.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/deprecated.meta.json
--rw-r--r--   0        0        0   160482 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/fixtures.data.json
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/fixtures.meta.json
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/freeze_support.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/freeze_support.meta.json
--rw-r--r--   0        0        0     8779 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/helpconfig.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/helpconfig.meta.json
--rw-r--r--   0        0        0    55642 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/hookspec.data.json
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/hookspec.meta.json
--rw-r--r--   0        0        0    61764 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/legacypath.data.json
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/legacypath.meta.json
--rw-r--r--   0        0        0    71777 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/logging.data.json
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/logging.meta.json
--rw-r--r--   0        0        0    48380 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/main.data.json
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/main.meta.json
--rw-r--r--   0        0        0    25127 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/monkeypatch.data.json
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/monkeypatch.meta.json
--rw-r--r--   0        0        0    55452 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/nodes.data.json
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/nodes.meta.json
--rw-r--r--   0        0        0    29821 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/outcomes.data.json
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/outcomes.meta.json
--rw-r--r--   0        0        0    32109 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/pathlib.data.json
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/pathlib.meta.json
--rw-r--r--   0        0        0   127493 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/pytester.data.json
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/pytester.meta.json
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/pytester_assertions.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/pytester_assertions.meta.json
--rw-r--r--   0        0        0   120557 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/python.data.json
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/python.meta.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/python_api.data.json
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/python_api.meta.json
--rw-r--r--   0        0        0    29913 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/recwarn.data.json
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/recwarn.meta.json
--rw-r--r--   0        0        0    48022 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/reports.data.json
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/reports.meta.json
--rw-r--r--   0        0        0    42739 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/runner.data.json
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/runner.meta.json
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/scope.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/scope.meta.json
--rw-r--r--   0        0        0    14267 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/stash.data.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/stash.meta.json
--rw-r--r--   0        0        0    93383 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/terminal.data.json
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/terminal.meta.json
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/timing.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/timing.meta.json
--rw-r--r--   0        0        0    18976 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/tmpdir.data.json
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/tmpdir.meta.json
--rw-r--r--   0        0        0    28053 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/warning_types.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/warning_types.meta.json
--rw-r--r--   0        0        0    12285 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/warnings.data.json
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/warnings.meta.json
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_code/__init__.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_code/__init__.meta.json
--rw-r--r--   0        0        0   156659 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_code/code.data.json
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_code/code.meta.json
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_code/source.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_code/source.meta.json
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/__init__.meta.json
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/saferepr.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/saferepr.meta.json
--rw-r--r--   0        0        0    15648 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/terminalwriter.data.json
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/terminalwriter.meta.json
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/wcwidth.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/_io/wcwidth.meta.json
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/__init__.data.json
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/__init__.meta.json
--rw-r--r--   0        0        0    57796 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/rewrite.data.json
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/rewrite.meta.json
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/truncate.data.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/truncate.meta.json
--rw-r--r--   0        0        0    22198 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/util.data.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/assertion/util.meta.json
--rw-r--r--   0        0        0    98624 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/__init__.data.json
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/__init__.meta.json
--rw-r--r--   0        0        0    40173 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/argparsing.data.json
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/argparsing.meta.json
--rw-r--r--   0        0        0     4519 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/compat.data.json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/compat.meta.json
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/exceptions.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/exceptions.meta.json
--rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/findpaths.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/config/findpaths.meta.json
--rw-r--r--   0        0        0    30207 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/mark/__init__.data.json
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/mark/__init__.meta.json
--rw-r--r--   0        0        0    32898 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/mark/expression.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/mark/expression.meta.json
--rw-r--r--   0        0        0   125991 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/mark/structures.data.json
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_pytest/mark/structures.meta.json
--rw-r--r--   0        0        0    83683 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11223 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/__init__.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   103295 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/base_events.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/base_events.meta.json
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   193926 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/events.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/events.meta.json
--rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    33231 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/futures.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/futures.meta.json
--rw-r--r--   0        0        0    32184 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/locks.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/locks.meta.json
--rw-r--r--   0        0        0    17213 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    22405 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/queues.data.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/queues.meta.json
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/runners.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/runners.meta.json
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    37906 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/streams.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/streams.meta.json
--rw-r--r--   0        0        0    26122 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0   114482 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/tasks.meta.json
--rw-r--r--   0        0        0    29784 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/transports.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/transports.meta.json
--rw-r--r--   0        0        0    52671 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0   272323 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/__init__.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/__init__.meta.json
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/_version_info.data.json
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/_version_info.meta.json
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/converters.data.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/converters.meta.json
--rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/exceptions.data.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/exceptions.meta.json
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/filters.data.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/filters.meta.json
--rw-r--r--   0        0        0     8030 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/setters.data.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/setters.meta.json
--rw-r--r--   0        0        0    42485 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/validators.data.json
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/attr/validators.meta.json
--rw-r--r--   0        0        0   328600 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/collections/__init__.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/collections/__init__.meta.json
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/collections/abc.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/collections/abc.meta.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    73338 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    49160 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    21604 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert_jupyter/__init__.data.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert_jupyter/__init__.meta.json
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert_jupyter/code.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert_jupyter/code.meta.json
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert_jupyter/constans.data.json
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/convert_jupyter/constans.meta.json
--rw-r--r--   0        0        0   128612 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7771 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/__init__.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/__init__.meta.json
--rw-r--r--   0        0        0    12285 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/charset.data.json
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/charset.meta.json
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/contentmanager.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24056 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/errors.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/errors.meta.json
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/header.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/header.meta.json
--rw-r--r--   0        0        0    55948 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/message.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/message.meta.json
--rw-r--r--   0        0        0    31211 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/policy.data.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/email/policy.meta.json
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/html/__init__.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/html/__init__.meta.json
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/html/entities.data.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/html/entities.meta.json
--rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/__init__.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/__init__.meta.json
--rw-r--r--   0        0        0    44393 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/abc.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/abc.meta.json
--rw-r--r--   0        0        0    66414 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/machinery.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/machinery.meta.json
--rw-r--r--   0        0        0    22581 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/util.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/util.meta.json
--rw-r--r--   0        0        0    65166 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    17232 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/iniconfig/__init__.data.json
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/iniconfig/__init__.meta.json
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/__init__.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/__init__.meta.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/_identifier.data.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/_identifier.meta.json
--rw-r--r--   0        0        0     7488 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/async_utils.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/async_utils.meta.json
--rw-r--r--   0        0        0    25821 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/bccache.data.json
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/bccache.meta.json
--rw-r--r--   0        0        0   159096 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/compiler.data.json
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/compiler.meta.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/constants.data.json
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/constants.meta.json
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/debug.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/debug.meta.json
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/defaults.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/defaults.meta.json
--rw-r--r--   0        0        0   117491 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/environment.data.json
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/environment.meta.json
--rw-r--r--   0        0        0    17666 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/exceptions.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/exceptions.meta.json
--rw-r--r--   0        0        0    50117 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/ext.data.json
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/ext.meta.json
--rw-r--r--   0        0        0   155116 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/filters.data.json
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/filters.meta.json
--rw-r--r--   0        0        0    42209 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/idtracking.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/idtracking.meta.json
--rw-r--r--   0        0        0    92324 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/lexer.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/lexer.meta.json
--rw-r--r--   0        0        0    47987 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/loaders.data.json
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/loaders.meta.json
--rw-r--r--   0        0        0   149485 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/nodes.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/nodes.meta.json
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/optimizer.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/optimizer.meta.json
--rw-r--r--   0        0        0    46788 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/parser.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/parser.meta.json
--rw-r--r--   0        0        0   149733 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/runtime.data.json
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/runtime.meta.json
--rw-r--r--   0        0        0    32977 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/sandbox.data.json
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/sandbox.meta.json
--rw-r--r--   0        0        0    18093 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/tests.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/tests.meta.json
--rw-r--r--   0        0        0    62046 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/utils.data.json
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/utils.meta.json
--rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/visitor.data.json
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/jinja2/visitor.meta.json
--rw-r--r--   0        0        0    16015 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/json/__init__.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/json/__init__.meta.json
--rw-r--r--   0        0        0    15057 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/json/decoder.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/json/decoder.meta.json
--rw-r--r--   0        0        0    11196 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/json/encoder.data.json
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/json/encoder.meta.json
--rw-r--r--   0        0        0   144599 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/logging/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/logging/__init__.meta.json
--rw-r--r--   0        0        0    34453 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/markupsafe/__init__.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/markupsafe/__init__.meta.json
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/markupsafe/_native.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/markupsafe/_native.meta.json
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/markupsafe/_speedups.data.json
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/markupsafe/_speedups.meta.json
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/__init__.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/__init__.meta.json
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/clean.data.json
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/clean.meta.json
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/code.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/code.meta.json
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/constans.data.json
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/menage_jupyter/constans.meta.json
--rw-r--r--   0        0        0    42808 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    29655 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    93585 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/context.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   141324 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    50446 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    22242 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    27747 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    26570 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    69348 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0     9856 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    25959 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0  2214583 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/__init__.data.json
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/_version.data.json
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/_version.meta.json
--rw-r--r--   0        0        0   116318 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/version.data.json
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/version.meta.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    22832 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     6949 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    72420 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   170442 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0   167325 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0    83238 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    15236 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   315905 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   194107 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    49470 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    54880 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/records.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/records.meta.json
--rw-r--r--   0        0        0    43630 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    19427 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    25918 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    20330 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   163337 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    27456 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   237819 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0     9809 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    65717 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    17124 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    41881 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    85476 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0    98137 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    90440 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    25448 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    82333 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0    99688 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    26852 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   110410 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29972 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   134395 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    22426 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14380 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    23983 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16270 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   292229 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    13311 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    17328 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    72995 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   389675 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   106200 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0    25009 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    19038 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_array_like.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_array_like.meta.json
--rw-r--r--   0        0        0   258623 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_callable.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_callable.meta.json
--rw-r--r--   0        0        0    45267 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_char_codes.data.json
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_char_codes.meta.json
--rw-r--r--   0        0        0    31334 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    27148 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_nbit.data.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_nbit.meta.json
--rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_scalars.data.json
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_scalars.meta.json
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_shape.data.json
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_shape.meta.json
--rw-r--r--   0        0        0   253879 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_ufunc.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/numpy/typing/_ufunc.meta.json
--rw-r--r--   0        0        0   332061 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/os/__init__.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/os/__init__.meta.json
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/os/path.data.json
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/os/path.meta.json
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/__about__.data.json
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/__about__.meta.json
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/__init__.data.json
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/__init__.meta.json
--rw-r--r--   0        0        0    34819 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/_manylinux.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/_manylinux.meta.json
--rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/_musllinux.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/_musllinux.meta.json
--rw-r--r--   0        0        0    13639 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/_structures.data.json
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/_structures.meta.json
--rw-r--r--   0        0        0    28426 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/markers.data.json
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/markers.meta.json
--rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/requirements.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/requirements.meta.json
--rw-r--r--   0        0        0    76266 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/specifiers.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/specifiers.meta.json
--rw-r--r--   0        0        0    27718 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/tags.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/tags.meta.json
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/utils.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/utils.meta.json
--rw-r--r--   0        0        0    85548 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/version.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/packaging/version.meta.json
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/__init__.data.json
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/__init__.meta.json
--rw-r--r--   0        0        0    91329 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/error.data.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/error.meta.json
--rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/iniconfig.data.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/iniconfig.meta.json
--rw-r--r--   0        0        0    47841 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/io.data.json
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/io.meta.json
--rw-r--r--   0        0        0    75515 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/path.data.json
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/path.meta.json
--rw-r--r--   0        0        0    12290 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/xml.data.json
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/py/xml.meta.json
--rw-r--r--   0        0        0    44798 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/__init__.data.json
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/__init__.meta.json
--rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/actions.data.json
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/actions.meta.json
--rw-r--r--   0        0        0    40364 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/common.data.json
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/common.meta.json
--rw-r--r--   0        0        0   354500 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/core.data.json
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/core.meta.json
--rw-r--r--   0        0        0    21997 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/exceptions.data.json
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/exceptions.meta.json
--rw-r--r--   0        0        0    49128 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/helpers.data.json
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/helpers.meta.json
--rw-r--r--   0        0        0    29831 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/results.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/results.meta.json
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/testing.data.json
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/testing.meta.json
--rw-r--r--   0        0        0    29221 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/unicode.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/unicode.meta.json
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/util.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/util.meta.json
--rw-r--r--   0        0        0    59045 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/diagram/__init__.data.json
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pyparsing/diagram/__init__.meta.json
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pytest/__init__.data.json
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/pytest/__init__.meta.json
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tests/__init__.data.json
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tests/__init__.meta.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tests/test_clean.data.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tests/test_clean.meta.json
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tests/test_code.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tests/test_code.meta.json
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/__init__.data.json
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/__init__.meta.json
--rw-r--r--   0        0        0    52540 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/_parser.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/_parser.meta.json
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/_re.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/_re.meta.json
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/_types.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/tomli/_types.meta.json
--rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/__init__.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/__init__.meta.json
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/async_case.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/async_case.meta.json
--rw-r--r--   0        0        0   223979 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/case.data.json
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/case.meta.json
--rw-r--r--   0        0        0    14335 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/loader.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/loader.meta.json
--rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/main.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/main.meta.json
--rw-r--r--   0        0        0    20934 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/result.data.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/result.meta.json
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/runner.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/runner.meta.json
--rw-r--r--   0        0        0    11681 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/signals.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/signals.meta.json
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/suite.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/unittest/suite.meta.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/urllib/__init__.data.json
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/urllib/__init__.meta.json
--rw-r--r--   0        0        0   141406 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/urllib/parse.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.mypy_cache/3.8/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.pytest_cache/README.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/menage_jupyter/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/menage_jupyter/clean.py
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/menage_jupyter/code.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/menage_jupyter/constans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/test_clean.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/test_code.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/convert.py
--rw-r--r--   0        0        0    84335 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/test_jupyter.ipynb
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/test_jupyter_clean.ipynb
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/tmp.ipynb
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/try.ipynb
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/try.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/try3.ipynb
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/tests/code/try3.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/LICENSE.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/README.md
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 convert_jupyter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/.flake8
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/.pylintrc
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/Makefile
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/lint.sh
+-rw-r--r--   0        0        0    46737 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/poetry.lock
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/upload.sh
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/__init__.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/__main__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/clean.py
+-rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/code.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/convert_jupyter/constans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/test_clean.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/test_code.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/test_main.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/convert.py
+-rw-r--r--   0        0        0    84335 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/test_jupyter.ipynb
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/test_jupyter_clean.ipynb
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/tmp.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/tmp.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try3.ipynb
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/tests/code/try3.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/README.md
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 convert_jupyter-1.0.1/PKG-INFO
```

### Comparing `convert_jupyter-0.1.5/.pylintrc` & `convert_jupyter-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `convert_jupyter-0.1.5/menage_jupyter/clean.py` & `convert_jupyter-1.0.1/convert_jupyter/clean.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import json
 import os
-from typing import Any, Dict
+from typing import Any, Dict, List
 
 
-def get_files_ext(path: str, ext: str = "ipynb"):
+def get_files_ext(path: str, ext: str = "ipynb") -> List[str]:
+    """
+    Function looks for files with the specified
+    extension in the path and children's folders.
+
+    Args:
+        path (str): root
+        ext (str, optional): extension searched for. Defaults to "ipynb".
+
+    Returns:
+        List[str]: list of files
+    """
     ext_files = []
     for (root, _, files) in os.walk(path):
         for f in files:
             if f.split(".")[-1] == ext:
                 ext_files.append(os.sep.join([root, f]))
     return ext_files
 
@@ -15,38 +26,38 @@
 def clean_all(path: str) -> None:
     """The function recursively finds all jupyter files
         and clears their output.
 
     Args:
         path (str): path with files to clean
     """
-    file_to_clear = get_files_ext(path, ext="ipynb")
-    for f in file_to_clear:
+    files_to_clear = get_files_ext(path, ext="ipynb")
+    for f in files_to_clear:
         clean(f)
 
 
 def clean(path: str) -> None:
     """Function clean jupyter file output.
 
     Args:
         path (str): file to cleancells
     """
-    with open(path, "r") as f:
+    with open(path, "r", encoding="utf-8") as f:
         my_file = json.load(f)
     new_cells = []
     for cell in my_file["cells"]:
         new_cell: Dict[str, Any] = {}
         if cell["cell_type"] == "code":
             new_cell["outputs"] = []
             new_cell["execution_count"] = None
         for key in ("cell_type", "metadata", "source"):
             new_cell[key] = cell[key]
         new_cells.append(new_cell)
     my_file["cells"] = new_cells
-    with open(path, "w") as f:
+    with open(path, "w", encoding="utf-8") as f:
         print(json.dumps(my_file, indent=1, sort_keys=True), file=f)
 
 
 if __name__ == "__main__":
     file_to_clear = get_files_ext(os.getcwd())[0]
     print(file_to_clear)
     clean(file_to_clear)
```

### Comparing `convert_jupyter-0.1.5/menage_jupyter/code.py` & `convert_jupyter-1.0.1/convert_jupyter/code.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 from os.path import exists
-from typing import Any, Dict
+from typing import Any, Dict, Union
 
 from .constans import CELL_SEPARATOR, MARKDOWN_BEGIN, MARKDOWN_END
 
 
-def jupyter2py(f_in_name: str, f_out_name: str = None, force=False) -> None:
+def jupyter2py(
+    f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False
+) -> None:
     """Function convert .ipynb to .py file.
 
     Function convert .ipynb to .py file.
     All cells after convert are separate to possible is revert convert.
     Markdown cells are commented.
 
     Args:
@@ -25,36 +27,37 @@
     """
     if f_out_name is None:
         f_out_name = f_in_name.replace(".ipynb", ".py")
     if force is False and exists(f_out_name):
         raise FileExistsError(
             f"{f_out_name} exist, use force=True to overwrite",
         )
-    f_in = open(f_in_name, "r")
-    f_out = open(f_out_name, "w")
-
-    my_file = json.load(f_in)
-
-    for i, cell in enumerate(my_file["cells"]):
-        if i > 0:
-            print(CELL_SEPARATOR, file=f_out, end="")
-        if cell["cell_type"] == "code":
-            print(*cell["source"], sep="", file=f_out, end="")
-        elif cell["cell_type"] == "markdown":
-            print(
-                MARKDOWN_BEGIN,
-                *cell["source"],
-                MARKDOWN_END,
-                sep="",
-                file=f_out,
-                end="",
-            )
-
-
-def py2jupyter(f_in_name: str, f_out_name: str = None, force=False) -> None:
+    with open(f_in_name, "r", encoding="utf-8") as f_in, open(
+        f_out_name, "w", encoding="utf-8"
+    ) as f_out:
+        my_file = json.load(f_in)
+        for i, cell in enumerate(my_file["cells"]):
+            if i > 0:
+                print(CELL_SEPARATOR, file=f_out, end="")
+            if cell["cell_type"] == "code":
+                print(*cell["source"], sep="", file=f_out, end="")
+            elif cell["cell_type"] == "markdown":
+                print(
+                    MARKDOWN_BEGIN,
+                    *cell["source"],
+                    MARKDOWN_END,
+                    sep="",
+                    file=f_out,
+                    end="",
+                )
+
+
+def py2jupyter(
+    f_in_name: str, f_out_name: Union[str, None] = None, force: bool = False
+) -> None:
     """Function convert .py to .ipynb file.
 
     Function convert .py to .ipynb file.
     Cells separator is {CELL_SEPARATOR}.
     Markdown cells starts by {MARKDOWN_BEGIN} end end by {MARKDOWN_END}
 
     Args:
@@ -70,55 +73,60 @@
     """
     if f_out_name is None:
         f_out_name = f_in_name.replace(".py", ".ipynb")
     if force is False and exists(f_out_name):
         raise FileExistsError(
             f"{f_out_name} exist, use force=True to overwrite",
         )
-    f_in = open(f_in_name, "r")
-    f_out = open(f_out_name, "w")
-    ret: Dict[str, Any] = {}
-    text = f_in.read()
-    cells_text = text.split(CELL_SEPARATOR)
-    cells = []
-    for cell in cells_text:
-        cell = cell
-        if cell[: len(MARKDOWN_BEGIN)] == MARKDOWN_BEGIN:
-            cells.append(_get_markdown(cell))
-        else:
-            cells.append(_get_code(cell))
-    ret["cells"] = cells
-
-    ret["metadata"] = (
-        {
-            "kernelspec": {
-                "display_name": "Python 3.8.10 64-bit",
-                "language": "python",
-                "name": "python3",
-            },
-            "language_info": {
-                "codemirror_mode": {"name": "ipython", "version": 3},
-                "file_extension": ".py",
-                "mimetype": "text/x-python",
-                "name": "python",
-                "nbconvert_exporter": "python",
-                "pygments_lexer": "ipython3",
-                "version": "3.8.10",
-            },
-            "orig_nbformat": 4,
-            "vscode": {
-                "interpreter": {
-                    "hash": "916dbcbb3f70747c44a77c7bcd40155683ae19c65e1c03b4aa3499c5328201f1"  # noqa
-                }
+
+    with open(f_in_name, "r", encoding="utf-8") as f_in, open(
+        f_out_name, "w", encoding="utf-8"
+    ) as f_out:
+
+        ret: Dict[str, Any] = {}
+        text = f_in.read()
+        cells_text = text.split(CELL_SEPARATOR)
+        cells = []
+        for cell in cells_text:
+            if cell[: len(MARKDOWN_BEGIN)] == MARKDOWN_BEGIN:
+                cells.append(_get_markdown(cell))
+            else:
+                cells.append(_get_code(cell))
+        ret["cells"] = cells
+
+        ret["metadata"] = (
+            {
+                "kernelspec": {
+                    "display_name": "Python 3.8.10 64-bit",
+                    "language": "python",
+                    "name": "python3",
+                },
+                "language_info": {
+                    "codemirror_mode": {"name": "ipython", "version": 3},
+                    "file_extension": ".py",
+                    "mimetype": "text/x-python",
+                    "name": "python",
+                    "nbconvert_exporter": "python",
+                    "pygments_lexer": "ipython3",
+                    "version": "3.8.10",
+                },
+                "orig_nbformat": 4,
+                "vscode": {
+                    "interpreter": {
+                        "hash": (
+                            "916dbcbb3f70747c44a77c7bcd40155683"
+                            "ae19c65e1c03b4aa3499c5328201f1"
+                        )
+                    }
+                },
             },
-        },
-    )
-    ret["nbformat"] = (4,)
-    ret["nbformat_minor"] = 2
-    print(json.dumps(ret, indent=4), file=f_out, end="")
+        )
+        ret["nbformat"] = (4,)
+        ret["nbformat_minor"] = 2
+        print(json.dumps(ret, indent=4), file=f_out, end="")
 
 
 def _get_markdown(value: str):
     cell = {
         "cell_type": "markdown",
         "source": value[len(MARKDOWN_BEGIN) : -len(MARKDOWN_END)],  # noqa
         "metadata": {},
```

### Comparing `convert_jupyter-0.1.5/tests/test_code.py` & `convert_jupyter-1.0.1/tests/test_code.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 import pytest
 
-from menage_jupyter.code import jupyter2py, py2jupyter
+from convert_jupyter.code import jupyter2py, py2jupyter
 
 
 def test_decode():
-    jupyter2py("tests/code/try.ipynb", "tests/code/try3.py", force=True)
-    with open("tests/code/try.py", "r") as expected, open(
-        "tests/code/try3.py", "r"
+    jupyter2py("tests/code/try.ipynb", "tests/code/tmp.py", force=True)
+    with open("tests/code/tmp.py", "r") as expected, open(
+        "tests/code/try3.py", "r", encoding="utf-8"
+    ) as actual:
+        assert expected.read() == actual.read()
+
+
+def test_encode():
+    py2jupyter("tests/code/try.py", "tests/code/tmp.ipynb", force=True)
+    with open("tests/code/tmp.ipynb", "r") as expected, open(
+        "tests/code/try3.ipynb", "r", encoding="utf-8"
     ) as actual:
         assert expected.read() == actual.read()
 
 
 def test_reverse_code():
-    py2jupyter("tests/code/try.py", "tests/code/try3.ipynb", force=True)
-    jupyter2py("tests/code/try3.ipynb", "tests/code/try3.py", force=True)
-    with open("tests/code/try.py") as begin, open("tests/code/try3.py") as end:
+    py2jupyter("tests/code/try.py", "tests/code/tmp.ipynb", force=True)
+    jupyter2py("tests/code/tmp.ipynb", "tests/code/try3.py", force=True)
+    with open("tests/code/try.py", encoding="utf-8") as begin, open(
+        "tests/code/try3.py", encoding="utf-8"
+    ) as end:
         assert begin.read() == end.read()
 
 
 def test_errors():
     with pytest.raises(FileExistsError):
         py2jupyter("tests/code/try.py", "tests/code/try3.ipynb")
```

### Comparing `convert_jupyter-0.1.5/tests/code/convert.py` & `convert_jupyter-1.0.1/tests/code/convert.py`

 * *Files identical despite different names*

### Comparing `convert_jupyter-0.1.5/tests/code/test_jupyter.ipynb` & `convert_jupyter-1.0.1/tests/code/test_jupyter.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-0.1.5/tests/code/test_jupyter_clean.ipynb` & `convert_jupyter-1.0.1/tests/code/test_jupyter_clean.ipynb`

 * *Files identical despite different names*

### Comparing `convert_jupyter-0.1.5/tests/code/try.ipynb` & `convert_jupyter-1.0.1/tests/code/try.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974206349206349%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, '\\n')]}}, 2: {'source': {insert: [(1, '\\n'), (2, "*

 * *            "'\\n')]}}}"}*

```diff
@@ -14,22 +14,25 @@
                 "vscode": {
                     "languageId": "python"
                 }
             },
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n"
+                "import numpy as np\n",
+                "\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## initialize\n"
+                "## initialize\n",
+                "\n",
+                "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "vscode": {
```

### Comparing `convert_jupyter-0.1.5/tests/code/try3.ipynb` & `convert_jupyter-1.0.1/tests/code/tmp.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666667%*

 * *Differences: {"'cells'": "{1: {'source': 'import matplotlib.pyplot as plt\\nimport numpy as np\\n\\n'}, 2: "*

 * *            "{'source': '## initialize\\n\\n\\n'}}"}*

```diff
@@ -5,20 +5,20 @@
             "metadata": {},
             "source": "## imports\n"
         },
         {
             "cell_type": "code",
             "metadata": {},
             "outputs": [],
-            "source": "import matplotlib.pyplot as plt\nimport numpy as np\n"
+            "source": "import matplotlib.pyplot as plt\nimport numpy as np\n\n"
         },
         {
             "cell_type": "markdown",
             "metadata": {},
-            "source": "## initialize\n"
+            "source": "## initialize\n\n\n"
         },
         {
             "cell_type": "code",
             "metadata": {},
             "outputs": [],
             "source": "X = np.arange(0, 100)\n"
         },
```

### Comparing `convert_jupyter-0.1.5/LICENSE.md` & `convert_jupyter-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_jupyter-0.1.5/README.md` & `convert_jupyter-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-# Menage jupyter 
-This project help menage jupyter flie.
+# Convert jupyter 
+This project help convert jupyter flie.
 It let:
     - convert .ipynb to .py file
     - convert .py to .ipynb file
     - clean output jupyter
 
 
 ## autors
 Bartłomiej Chwiłkowski (github: chwilko)
 
 
 # Structure
-menage_jupyter:
+convert_jupyter:
     - file with functions
 
 
 ## Functions 
 
 jupyter2py(f_in_name: str, f_out_name: str = None)
+
 py2jupyter(f_in_name: str, f_out_name: str = None)
+
 clean(path: str)
     Function clean jupyter file output.
+
 clean_all(path: str)
     The function recursively finds all jupyter files and clears their output.
 
 
 ## Licence
 MIT
```

### Comparing `convert_jupyter-0.1.5/pyproject.toml` & `convert_jupyter-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 [tool.poetry]
 name = "convert-jupyter"
-version = "0.1.5"
-description = "Package help menage jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
+version = "1.0.1"
+description = "Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
 
 authors = ["Bartłomiej Chwiłkowski <bartekchwilkowski@gmail.com>"]
-packages = [{include = "menage_jupyter"}]
+packages = [{include = "convert_jupyter"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 black = {extras = ["jupyter"], version = "^22.10.0"}
+pylint = "^2.17.5"
+isort = "^5.12.0"
+mypy = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "convert-jupyter"
-version = "0.1.5"
+version = "1.0.1"
 authors = [    
   { name="Bartłomiej Chwiłkowski", email="bartekchwilkowski@gmail.com" },
   ]
-description = "Package help menage jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
+description = "Package help convert jupyter files. It let convert py to jupyter file and vice versa, and clean jupyter output. Useful to exclude git conflicts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/chwilko/menage_jupyter"
+"Homepage" = "https://github.com/chwilko/convert_jupyter"
 
+
+
+[tool.black]
+target_version = ["py310"]
```

