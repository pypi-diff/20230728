# Comparing `tmp/abstract_gui-0.0.45-py3.11.egg` & `tmp/abstract_gui-0.0.46-py3.11.egg`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 22812 bytes, number of entries: 20
--rw-rw-r--  2.0 unx     3801 b- defN 23-Jul-27 17:10 EGG-INFO/PKG-INFO
--rw-rw-r--  2.0 unx      505 b- defN 23-Jul-27 17:10 EGG-INFO/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-27 17:10 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-27 17:10 EGG-INFO/not-zip-safe
--rw-rw-r--  2.0 unx       31 b- defN 23-Jul-27 17:10 EGG-INFO/requires.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-Jul-27 17:10 EGG-INFO/top_level.txt
+Zip file size: 22859 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx     3800 b- defN 23-Jul-27 17:17 EGG-INFO/PKG-INFO
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jul-27 17:17 EGG-INFO/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-27 17:17 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-27 17:17 EGG-INFO/not-zip-safe
+-rw-rw-r--  2.0 unx       31 b- defN 23-Jul-27 17:17 EGG-INFO/requires.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jul-27 17:17 EGG-INFO/top_level.txt
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 00:17 abstract_gui/__init__.py
 -rw-r--r--  2.0 unx     1294 b- defN 23-May-29 06:40 abstract_gui/main.py
 -rw-r--r--  2.0 unx     2500 b- defN 23-May-26 16:54 abstract_gui/PyQt5/PyQt5_browser_window.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-25 21:06 abstract_gui/PyQt5/__init__.py
--rw-r--r--  2.0 unx     5395 b- defN 23-Jul-27 17:10 abstract_gui/PyQt5/__pycache__/PyQt5_browser_window.cpython-311.pyc
--rw-r--r--  2.0 unx      168 b- defN 23-Jul-27 17:10 abstract_gui/PyQt5/__pycache__/__init__.cpython-311.pyc
--rw-r--r--  2.0 unx      162 b- defN 23-Jul-27 17:10 abstract_gui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--  2.0 unx     2527 b- defN 23-Jul-27 17:10 abstract_gui/__pycache__/main.cpython-311.pyc
+-rw-r--r--  2.0 unx     5395 b- defN 23-Jul-27 17:17 abstract_gui/PyQt5/__pycache__/PyQt5_browser_window.cpython-311.pyc
+-rw-r--r--  2.0 unx      168 b- defN 23-Jul-27 17:17 abstract_gui/PyQt5/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-27 17:17 abstract_gui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx     2527 b- defN 23-Jul-27 17:17 abstract_gui/__pycache__/main.cpython-311.pyc
 -rw-r--r--  2.0 unx      138 b- defN 23-May-30 23:26 abstract_gui/simple_gui/__init__.py
 -rw-r--r--  2.0 unx     3240 b- defN 23-May-31 09:39 abstract_gui/simple_gui/gui_presets.py
--rw-r--r--  2.0 unx    11222 b- defN 23-Jul-27 17:10 abstract_gui/simple_gui/gui_template.py
--rw-r--r--  2.0 unx      396 b- defN 23-Jul-27 17:10 abstract_gui/simple_gui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--  2.0 unx     4542 b- defN 23-Jul-27 17:10 abstract_gui/simple_gui/__pycache__/gui_presets.cpython-311.pyc
--rw-r--r--  2.0 unx    16260 b- defN 23-Jul-27 17:10 abstract_gui/simple_gui/__pycache__/gui_template.cpython-311.pyc
-20 files, 52196 bytes uncompressed, 19748 bytes compressed:  62.2%
+-rw-r--r--  2.0 unx    11278 b- defN 23-Jul-27 17:11 abstract_gui/simple_gui/gui_template.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Jul-27 17:17 abstract_gui/simple_gui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx     4542 b- defN 23-Jul-27 17:17 abstract_gui/simple_gui/__pycache__/gui_presets.cpython-311.pyc
+-rw-r--r--  2.0 unx    16355 b- defN 23-Jul-27 17:17 abstract_gui/simple_gui/__pycache__/gui_template.cpython-311.pyc
+20 files, 52346 bytes uncompressed, 19795 bytes compressed:  62.2%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.45
+Version: 0.0.46
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
-Home-page: https://github.com/abstract_endeavors/abstract_essentials/abstract_gui
+Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

## abstract_gui/simple_gui/gui_template.py

```diff
@@ -217,15 +217,17 @@
     values_all=[]
     if win is None:
         win = get_globes(string='window')
     while verify_window(win):
         event, values = win.read()
         if values != None:
             values_all = values
+        print(values_all)
         if win_closed(event):
+            print(values_all)
             return values_all
             break
     close_window(win)
     return values_all
 
 def single_call(win):
     """
```

## abstract_gui/simple_gui/__pycache__/gui_template.cpython-311.pyc

### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4cebc264 (Thu Jul 27 22:10:20 2023 UTC)
-files sz: 11222
+moddate:  0x9febc264 (Thu Jul 27 22:11:43 2023 UTC)
+files sz: 11278
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -287,33 +287,33 @@
                566 STORE_NAME              37 (while_basic_events)
    
    210         568 LOAD_CONST              64 ((None,))
                570 LOAD_CONST              53 (<code object while_basic, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 210>)
                572 MAKE_FUNCTION            1 (defaults)
                574 STORE_NAME              38 (while_basic)
    
-   230         576 LOAD_CONST              54 (<code object single_call, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 230>)
+   232         576 LOAD_CONST              54 (<code object single_call, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 232>)
                578 MAKE_FUNCTION            0
                580 STORE_NAME              39 (single_call)
    
-   244         582 LOAD_CONST              55 (<code object get_last_window, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 244>)
+   246         582 LOAD_CONST              55 (<code object get_last_window, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 246>)
                584 MAKE_FUNCTION            0
                586 STORE_NAME              40 (get_last_window)
    
-   253         588 LOAD_CONST              69 ((None, 0, 5, None))
+   255         588 LOAD_CONST              69 ((None, 0, 5, None))
                590 LOAD_CONST              57 ('progress')
                592 LOAD_NAME               30 (int)
                594 LOAD_CONST              58 ('step')
                596 LOAD_NAME               30 (int)
                598 BUILD_TUPLE              4
-               600 LOAD_CONST              59 (<code object while_progress, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 253>)
+               600 LOAD_CONST              59 (<code object while_progress, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 255>)
                602 MAKE_FUNCTION            5 (defaults, annotations)
                604 STORE_NAME              41 (while_progress)
    
-   276         606 LOAD_CONST              70 (('last_window', '', ''))
+   278         606 LOAD_CONST              70 (('last_window', '', ''))
                608 LOAD_CONST              44 ('curr_win')
                610 LOAD_NAME               16 (str)
                612 JUMP_IF_TRUE_OR_POP     18 (to 650)
                614 PUSH_NULL
                616 LOAD_NAME               34 (type)
                618 PUSH_NULL
                620 LOAD_NAME               19 (get_window)
@@ -322,53 +322,53 @@
                636 PRECALL                  1
                640 CALL                     1
            >>  650 LOAD_CONST              48 ('st')
                652 LOAD_NAME               16 (str)
                654 LOAD_CONST              18 ('obj')
                656 LOAD_NAME               20 (any)
                658 BUILD_TUPLE              6
-               660 LOAD_CONST              60 (<code object update, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 276>)
+               660 LOAD_CONST              60 (<code object update, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 278>)
                662 MAKE_FUNCTION            5 (defaults, annotations)
                664 STORE_NAME              42 (update)
    
-   291         666 LOAD_CONST              71 (('last_window', ''))
+   293         666 LOAD_CONST              71 (('last_window', ''))
                668 LOAD_CONST              44 ('curr_win')
                670 LOAD_NAME               16 (str)
                672 JUMP_IF_TRUE_OR_POP     18 (to 710)
                674 PUSH_NULL
                676 LOAD_NAME               34 (type)
                678 PUSH_NULL
                680 LOAD_NAME               19 (get_window)
                682 PRECALL                  0
                686 CALL                     0
                696 PRECALL                  1
                700 CALL                     1
            >>  710 LOAD_CONST              48 ('st')
                712 LOAD_NAME               16 (str)
                714 BUILD_TUPLE              4
-               716 LOAD_CONST              61 (<code object get_value, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 291>)
+               716 LOAD_CONST              61 (<code object get_value, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 293>)
                718 MAKE_FUNCTION            5 (defaults, annotations)
                720 STORE_NAME              43 (get_value)
    
-   311         722 LOAD_CONST              71 (('last_window', ''))
+   313         722 LOAD_CONST              71 (('last_window', ''))
                724 LOAD_CONST              44 ('curr_win')
                726 LOAD_NAME               16 (str)
                728 JUMP_IF_TRUE_OR_POP     18 (to 766)
                730 PUSH_NULL
                732 LOAD_NAME               34 (type)
                734 PUSH_NULL
                736 LOAD_NAME               19 (get_window)
                738 PRECALL                  0
                742 CALL                     0
                752 PRECALL                  1
                756 CALL                     1
            >>  766 LOAD_CONST              48 ('st')
                768 LOAD_NAME               16 (str)
                770 BUILD_TUPLE              4
-               772 LOAD_CONST              62 (<code object get_event, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 311>)
+               772 LOAD_CONST              62 (<code object get_event, file "build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py", line 313>)
                774 MAKE_FUNCTION            5 (defaults, annotations)
                776 STORE_NAME              44 (get_event)
                778 LOAD_CONST              24 (None)
                780 RETURN_VALUE
    consts
       0
       ('get_keys',)
@@ -1215,19 +1215,21 @@
          argcount  : 1
          nlocals   : 4
          stacksize : 3
          flags     : 3
          code
             0x970067007d017c0080107401000000000000000000006402ac03a60100
             00ab0100000000000000007d007403000000000000000000007c00a60100
-            00ab010000000000000000723f7c00a00200000000000000000000000000
+            00ab010000000000000000725d7c00a00200000000000000000000000000
             00000000000000a6000000ab0000000000000000005c0200007d027d037c
-            0364016b030000000072027c037d017407000000000000000000007c02a6
-            010000ab01000000000000000072027c0153007403000000000000000000
-            007c00a6010000ab010000000000000000b03f7409000000000000000000
+            0364016b030000000072027c037d017407000000000000000000007c01a6
+            010000ab01000000000000000001007409000000000000000000007c02a6
+            010000ab01000000000000000072117407000000000000000000007c01a6
+            010000ab01000000000000000001007c0153007403000000000000000000
+            007c00a6010000ab010000000000000000b05d740b000000000000000000
             007c00a6010000ab01000000000000000001007c015300
          210           0 RESUME                   0
          
          217           2 BUILD_LIST               0
                        4 STORE_FAST               1 (values_all)
          
          218           6 LOAD_FAST                0 (win)
@@ -1240,15 +1242,15 @@
                       30 CALL                     1
                       40 STORE_FAST               0 (win)
          
          220     >>   42 LOAD_GLOBAL              3 (NULL + verify_window)
                       54 LOAD_FAST                0 (win)
                       56 PRECALL                  1
                       60 CALL                     1
-                      70 POP_JUMP_FORWARD_IF_FALSE    63 (to 198)
+                      70 POP_JUMP_FORWARD_IF_FALSE    93 (to 258)
          
          221     >>   72 LOAD_FAST                0 (win)
                       74 LOAD_METHOD              2 (read)
                       96 PRECALL                  0
                      100 CALL                     0
                      110 UNPACK_SEQUENCE          2
                      114 STORE_FAST               2 (event)
@@ -1258,99 +1260,111 @@
                      120 LOAD_CONST               1 (None)
                      122 COMPARE_OP               3 (!=)
                      128 POP_JUMP_FORWARD_IF_FALSE     2 (to 134)
          
          223         130 LOAD_FAST                3 (values)
                      132 STORE_FAST               1 (values_all)
          
-         224     >>  134 LOAD_GLOBAL              7 (NULL + win_closed)
-                     146 LOAD_FAST                2 (event)
+         224     >>  134 LOAD_GLOBAL              7 (NULL + print)
+                     146 LOAD_FAST                1 (values_all)
                      148 PRECALL                  1
                      152 CALL                     1
-                     162 POP_JUMP_FORWARD_IF_FALSE     2 (to 168)
+                     162 POP_TOP
          
-         225         164 LOAD_FAST                1 (values_all)
-                     166 RETURN_VALUE
+         225         164 LOAD_GLOBAL              9 (NULL + win_closed)
+                     176 LOAD_FAST                2 (event)
+                     178 PRECALL                  1
+                     182 CALL                     1
+                     192 POP_JUMP_FORWARD_IF_FALSE    17 (to 228)
+         
+         226         194 LOAD_GLOBAL              7 (NULL + print)
+                     206 LOAD_FAST                1 (values_all)
+                     208 PRECALL                  1
+                     212 CALL                     1
+                     222 POP_TOP
+         
+         227         224 LOAD_FAST                1 (values_all)
+                     226 RETURN_VALUE
+         
+         220     >>  228 LOAD_GLOBAL              3 (NULL + verify_window)
+                     240 LOAD_FAST                0 (win)
+                     242 PRECALL                  1
+                     246 CALL                     1
+                     256 POP_JUMP_BACKWARD_IF_TRUE    93 (to 72)
+         
+         229     >>  258 LOAD_GLOBAL             11 (NULL + close_window)
+                     270 LOAD_FAST                0 (win)
+                     272 PRECALL                  1
+                     276 CALL                     1
+                     286 POP_TOP
          
-         220     >>  168 LOAD_GLOBAL              3 (NULL + verify_window)
-                     180 LOAD_FAST                0 (win)
-                     182 PRECALL                  1
-                     186 CALL                     1
-                     196 POP_JUMP_BACKWARD_IF_TRUE    63 (to 72)
-         
-         227     >>  198 LOAD_GLOBAL              9 (NULL + close_window)
-                     210 LOAD_FAST                0 (win)
-                     212 PRECALL                  1
-                     216 CALL                     1
-                     226 POP_TOP
-         
-         228         228 LOAD_FAST                1 (values_all)
-                     230 RETURN_VALUE
+         230         288 LOAD_FAST                1 (values_all)
+                     290 RETURN_VALUE
          consts
             "\n    Executes a while loop for handling basic events in a PySimpleGUI window.\n\n    Args:\n        win: The window to handle events for. If not provided, it uses the 'window' global object.\n    "
             None
             'window'
             ('string',)
-         names      ('get_globes', 'verify_window', 'read', 'win_closed', 'close_window')
+         names      ('get_globes', 'verify_window', 'read', 'print', 'win_closed', 'close_window')
          varnames   ('win', 'values_all', 'event', 'values')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
          name       'while_basic'
          firstlineno 210
-         lnotab 0x02070401040120011e012e010c0104011e0104fb1e071e01
+         lnotab 0x02070401040120011e012e010c0104011e011e011e0104f91e091e01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 2
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000a60000
             00ab0000000000000000005c0200007d017d027c00a00100000000000000
             00000000000000000000000000a6000000ab00000000000000000001007c
             025300
-         230           0 RESUME                   0
+         232           0 RESUME                   0
          
-         240           2 LOAD_FAST                0 (win)
+         242           2 LOAD_FAST                0 (win)
                        4 LOAD_METHOD              0 (read)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 UNPACK_SEQUENCE          2
                       44 STORE_FAST               1 (event)
                       46 STORE_FAST               2 (values)
          
-         241          48 LOAD_FAST                0 (win)
+         243          48 LOAD_FAST                0 (win)
                       50 LOAD_METHOD              1 (close)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 POP_TOP
          
-         242          88 LOAD_FAST                2 (values)
+         244          88 LOAD_FAST                2 (values)
                       90 RETURN_VALUE
          consts
             '\n    Reads and closes a PySimpleGUI window, returning the captured values.\n\n    Args:\n        win: The window to read.\n\n    Returns:\n        dict: The captured values from the window.\n    '
          names      ('read', 'close')
          varnames   ('win', 'event', 'values')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
          name       'single_call'
-         firstlineno 230
+         firstlineno 232
          lnotab 0x020a2e012801
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             006402190000000000000000006403190000000000000000005300
-         244           0 RESUME                   0
+         246           0 RESUME                   0
          
-         251           2 LOAD_GLOBAL              1 (NULL + ret_globals)
+         253           2 LOAD_GLOBAL              1 (NULL + ret_globals)
                       14 LOAD_CONST               1 ('all_windows')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 LOAD_CONST               2 ('last_window')
                       32 BINARY_SUBSCR
                       42 LOAD_CONST               3 ('name')
                       44 BINARY_SUBSCR
@@ -1362,15 +1376,15 @@
             'name'
          names      ('ret_globals',)
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
          name       'get_last_window'
-         firstlineno 244
+         firstlineno 246
          lnotab 0x0207
       5
       'progress'
       'step'
       code
          argcount  : 4
          nlocals   : 6
@@ -1386,96 +1400,96 @@
             0200000000000000000000000000000000000000006402ac03a6010000ab
             0100000000000000000100740b000000000000000000007c0064047c01ac
             05a6030000ab03000000000000000001007c017c027a0d00007d01740d00
             000000000000000000640264067c01ac07a6030000ab0300000000000000
             0072057c0264087a1200007d027403000000000000000000007c00a60100
             00ab010000000000000000b08b740f000000000000000000007c00a60100
             00ab010000000000000000010064015300
-         253           0 RESUME                   0
+         255           0 RESUME                   0
          
-         263           2 LOAD_FAST                0 (win)
+         265           2 LOAD_FAST                0 (win)
                        4 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 34)
          
-         264           6 LOAD_GLOBAL              1 (NULL + get_last_window)
+         266           6 LOAD_GLOBAL              1 (NULL + get_last_window)
                       18 PRECALL                  0
                       22 CALL                     0
                       32 STORE_FAST               0 (win)
          
-         265     >>   34 LOAD_GLOBAL              3 (NULL + verify_window)
+         267     >>   34 LOAD_GLOBAL              3 (NULL + verify_window)
                       46 LOAD_FAST                0 (win)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 POP_JUMP_FORWARD_IF_FALSE   139 (to 342)
          
-         266     >>   64 LOAD_FAST                0 (win)
+         268     >>   64 LOAD_FAST                0 (win)
                       66 LOAD_METHOD              2 (read)
                       88 LOAD_CONST               2 (100)
                       90 KW_NAMES                 3
                       92 PRECALL                  1
                       96 CALL                     1
                      106 UNPACK_SEQUENCE          2
                      110 STORE_FAST               4 (event)
                      112 STORE_FAST               5 (values)
          
-         267         114 LOAD_GLOBAL              7 (NULL + win_closed)
+         269         114 LOAD_GLOBAL              7 (NULL + win_closed)
                      126 LOAD_FAST                4 (event)
                      128 PRECALL                  1
                      132 CALL                     1
                      142 POP_JUMP_FORWARD_IF_TRUE    15 (to 174)
                      144 LOAD_GLOBAL              9 (NULL + thread_alive)
                      156 LOAD_FAST                3 (thread)
                      158 PRECALL                  1
                      162 CALL                     1
                      172 POP_JUMP_FORWARD_IF_TRUE     1 (to 176)
          
-         268     >>  174 JUMP_FORWARD            83 (to 342)
+         270     >>  174 JUMP_FORWARD            83 (to 342)
          
-         269     >>  176 LOAD_FAST                0 (win)
+         271     >>  176 LOAD_FAST                0 (win)
                      178 LOAD_METHOD              2 (read)
                      200 LOAD_CONST               2 (100)
                      202 KW_NAMES                 3
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         270         220 LOAD_GLOBAL             11 (NULL + update_progress)
+         272         220 LOAD_GLOBAL             11 (NULL + update_progress)
                      232 LOAD_FAST                0 (win)
                      234 LOAD_CONST               4 ('bar')
                      236 LOAD_FAST                1 (progress)
                      238 KW_NAMES                 5
                      240 PRECALL                  3
                      244 CALL                     3
                      254 POP_TOP
          
-         271         256 LOAD_FAST                1 (progress)
+         273         256 LOAD_FAST                1 (progress)
                      258 LOAD_FAST                2 (step)
                      260 BINARY_OP               13 (+=)
                      264 STORE_FAST               1 (progress)
          
-         272         266 LOAD_GLOBAL             13 (NULL + out_of_bounds)
+         274         266 LOAD_GLOBAL             13 (NULL + out_of_bounds)
                      278 LOAD_CONST               2 (100)
                      280 LOAD_CONST               6 (0)
                      282 LOAD_FAST                1 (progress)
                      284 KW_NAMES                 7
                      286 PRECALL                  3
                      290 CALL                     3
                      300 POP_JUMP_FORWARD_IF_FALSE     5 (to 312)
          
-         273         302 LOAD_FAST                2 (step)
+         275         302 LOAD_FAST                2 (step)
                      304 LOAD_CONST               8 (-1)
                      306 BINARY_OP               18 (*=)
                      310 STORE_FAST               2 (step)
          
-         265     >>  312 LOAD_GLOBAL              3 (NULL + verify_window)
+         267     >>  312 LOAD_GLOBAL              3 (NULL + verify_window)
                      324 LOAD_FAST                0 (win)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 POP_JUMP_BACKWARD_IF_TRUE   139 (to 64)
          
-         274     >>  342 LOAD_GLOBAL             15 (NULL + close_window)
+         276     >>  342 LOAD_GLOBAL             15 (NULL + close_window)
                      354 LOAD_FAST                0 (win)
                      356 PRECALL                  1
                      360 CALL                     1
                      370 POP_TOP
                      372 LOAD_CONST               1 (None)
                      374 RETURN_VALUE
          consts
@@ -1490,15 +1504,15 @@
             -1
          names      ('get_last_window', 'verify_window', 'read', 'win_closed', 'thread_alive', 'update_progress', 'out_of_bounds', 'close_window')
          varnames   ('win', 'progress', 'step', 'thread', 'event', 'values')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
          name       'while_progress'
-         firstlineno 253
+         firstlineno 255
          lnotab 0x020a04011c011e0132013c0102012c0124010a0124010af81e09
       code
          argcount  : 3
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -1508,56 +1522,56 @@
             0000000000000001007405000000000000000000007c02a6010000ab0100
             00000000000000740600000000000000000000750072287c036401190000
             000000000000007c0119000000000000000000a001000000000000000000
             00000000000000000000007c02640319000000000000000000ac04a60100
             00ab010000000000000000010074090000000000000000000064057c0374
             0a00000000000000000000ac06a6030000ab030000000000000000010064
             075300
-         276           0 RESUME                   0
+         278           0 RESUME                   0
          
-         285           2 LOAD_GLOBAL              1 (NULL + get_all_windows)
+         287           2 LOAD_GLOBAL              1 (NULL + get_all_windows)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               3 (all_windows)
          
-         286          30 LOAD_FAST                3 (all_windows)
+         288          30 LOAD_FAST                3 (all_windows)
                       32 LOAD_CONST               1 ('last_window')
                       34 BINARY_SUBSCR
                       44 LOAD_FAST                1 (st)
                       46 BINARY_SUBSCR
                       56 LOAD_METHOD              1 (update)
                       78 LOAD_FAST                2 (obj)
                       80 KW_NAMES                 2
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_TOP
          
-         287          98 LOAD_GLOBAL              5 (NULL + type)
+         289          98 LOAD_GLOBAL              5 (NULL + type)
                      110 LOAD_FAST                2 (obj)
                      112 PRECALL                  1
                      116 CALL                     1
                      126 LOAD_GLOBAL              6 (list)
                      138 IS_OP                    0
                      140 POP_JUMP_FORWARD_IF_FALSE    40 (to 222)
          
-         288         142 LOAD_FAST                3 (all_windows)
+         290         142 LOAD_FAST                3 (all_windows)
                      144 LOAD_CONST               1 ('last_window')
                      146 BINARY_SUBSCR
                      156 LOAD_FAST                1 (st)
                      158 BINARY_SUBSCR
                      168 LOAD_METHOD              1 (update)
                      190 LOAD_FAST                2 (obj)
                      192 LOAD_CONST               3 (0)
                      194 BINARY_SUBSCR
                      204 KW_NAMES                 4
                      206 PRECALL                  1
                      210 CALL                     1
                      220 POP_TOP
          
-         289     >>  222 LOAD_GLOBAL              9 (NULL + update_registry)
+         291     >>  222 LOAD_GLOBAL              9 (NULL + update_registry)
                      234 LOAD_CONST               5 ('all_windows')
                      236 LOAD_FAST                3 (all_windows)
                      238 LOAD_GLOBAL             10 (registry_name)
                      250 KW_NAMES                 6
                      252 PRECALL                  3
                      256 CALL                     3
                      266 POP_TOP
@@ -1574,15 +1588,15 @@
             None
          names      ('get_all_windows', 'update', 'type', 'list', 'update_registry', 'registry_name')
          varnames   ('curr_win', 'st', 'obj', 'all_windows')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
          name       'update'
-         firstlineno 276
+         firstlineno 278
          lnotab 0x02091c0144012c015001
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -1590,145 +1604,145 @@
             027c007d037403000000000000000000007c00a6010000ab010000000000
             000000740300000000000000000000740500000000000000000000a60000
             00ab000000000000000000a6010000ab0100000000000000006b02000000
             0072117407000000000000000000007c00a6010000ab0100000000000000
             00010064017d037c027c00190000000000000000007d047c017c04640219
             0000000000000000007600720e7c046402190000000000000000007c0119
             000000000000000000530064035300
-         291           0 RESUME                   0
+         293           0 RESUME                   0
          
-         302           2 LOAD_GLOBAL              1 (NULL + get_all_windows)
+         304           2 LOAD_GLOBAL              1 (NULL + get_all_windows)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               2 (all_windows)
          
-         303          30 LOAD_FAST                0 (curr_win)
+         305          30 LOAD_FAST                0 (curr_win)
                       32 STORE_FAST               3 (win_name)
          
-         304          34 LOAD_GLOBAL              3 (NULL + type)
+         306          34 LOAD_GLOBAL              3 (NULL + type)
                       46 LOAD_FAST                0 (curr_win)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_GLOBAL              3 (NULL + type)
                       74 LOAD_GLOBAL              5 (NULL + get_window)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 PRECALL                  1
                      104 CALL                     1
                      114 COMPARE_OP               2 (==)
                      120 POP_JUMP_FORWARD_IF_FALSE    17 (to 156)
          
-         305         122 LOAD_GLOBAL              7 (NULL + update_read)
+         307         122 LOAD_GLOBAL              7 (NULL + update_read)
                      134 LOAD_FAST                0 (curr_win)
                      136 PRECALL                  1
                      140 CALL                     1
                      150 POP_TOP
          
-         306         152 LOAD_CONST               1 ('last_window')
+         308         152 LOAD_CONST               1 ('last_window')
                      154 STORE_FAST               3 (win_name)
          
-         307     >>  156 LOAD_FAST                2 (all_windows)
+         309     >>  156 LOAD_FAST                2 (all_windows)
                      158 LOAD_FAST                0 (curr_win)
                      160 BINARY_SUBSCR
                      170 STORE_FAST               4 (curr_js)
          
-         308         172 LOAD_FAST                1 (st)
+         310         172 LOAD_FAST                1 (st)
                      174 LOAD_FAST                4 (curr_js)
                      176 LOAD_CONST               2 ('values')
                      178 BINARY_SUBSCR
                      188 CONTAINS_OP              0
                      190 POP_JUMP_FORWARD_IF_FALSE    14 (to 220)
          
-         309         192 LOAD_FAST                4 (curr_js)
+         311         192 LOAD_FAST                4 (curr_js)
                      194 LOAD_CONST               2 ('values')
                      196 BINARY_SUBSCR
                      206 LOAD_FAST                1 (st)
                      208 BINARY_SUBSCR
                      218 RETURN_VALUE
          
-         308     >>  220 LOAD_CONST               3 (None)
+         310     >>  220 LOAD_CONST               3 (None)
                      222 RETURN_VALUE
          consts
             '\n    Retrieves the value of a specific element in the current window.\n\n    Args:\n        curr_win (str or type(get_window())): The current window to retrieve the value from. If not provided, it uses the last opened window.\n        st (str): The element to retrieve the value for.\n\n    Returns:\n        any: The retrieved value of the element.\n    '
             'last_window'
             'values'
             None
          names      ('get_all_windows', 'type', 'get_window', 'update_read')
          varnames   ('curr_win', 'st', 'all_windows', 'win_name', 'curr_js')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
          name       'get_value'
-         firstlineno 291
+         firstlineno 293
          lnotab 0x020b1c01040158011e010401100114011cff
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             027c007d037403000000000000000000007c00a6010000ab010000000000
             000000740300000000000000000000740500000000000000000000a60000
             00ab000000000000000000a6010000ab0100000000000000006b02000000
             0072117407000000000000000000007c00a6010000ab0100000000000000
             00010064017d037c027c03190000000000000000007d047c046402190000
             000000000000005300
-         311           0 RESUME                   0
+         313           0 RESUME                   0
          
-         322           2 LOAD_GLOBAL              1 (NULL + get_all_windows)
+         324           2 LOAD_GLOBAL              1 (NULL + get_all_windows)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               2 (all_windows)
          
-         323          30 LOAD_FAST                0 (curr_win)
+         325          30 LOAD_FAST                0 (curr_win)
                       32 STORE_FAST               3 (win_name)
          
-         324          34 LOAD_GLOBAL              3 (NULL + type)
+         326          34 LOAD_GLOBAL              3 (NULL + type)
                       46 LOAD_FAST                0 (curr_win)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 LOAD_GLOBAL              3 (NULL + type)
                       74 LOAD_GLOBAL              5 (NULL + get_window)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 PRECALL                  1
                      104 CALL                     1
                      114 COMPARE_OP               2 (==)
                      120 POP_JUMP_FORWARD_IF_FALSE    17 (to 156)
          
-         325         122 LOAD_GLOBAL              7 (NULL + update_read)
+         327         122 LOAD_GLOBAL              7 (NULL + update_read)
                      134 LOAD_FAST                0 (curr_win)
                      136 PRECALL                  1
                      140 CALL                     1
                      150 POP_TOP
          
-         326         152 LOAD_CONST               1 ('last_window')
+         328         152 LOAD_CONST               1 ('last_window')
                      154 STORE_FAST               3 (win_name)
          
-         327     >>  156 LOAD_FAST                2 (all_windows)
+         329     >>  156 LOAD_FAST                2 (all_windows)
                      158 LOAD_FAST                3 (win_name)
                      160 BINARY_SUBSCR
                      170 STORE_FAST               4 (curr_js)
          
-         328         172 LOAD_FAST                4 (curr_js)
+         330         172 LOAD_FAST                4 (curr_js)
                      174 LOAD_CONST               2 ('event')
                      176 BINARY_SUBSCR
                      186 RETURN_VALUE
          consts
             '\n    Retrieves the event of the current window or the specified window.\n\n    Args:\n        curr_win (str or type(get_window())): The current window to retrieve the event from. If not provided, it uses the last opened window.\n        st (str): Unused parameter for consistency with other functions.\n\n    Returns:\n        any: The retrieved event of the window.\n    '
             'last_window'
             'event'
          names      ('get_all_windows', 'type', 'get_window', 'update_read')
          varnames   ('curr_win', 'st', 'all_windows', 'win_name', 'curr_js')
          freevars   ()
          cellvars   ()
          filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
          name       'get_event'
-         firstlineno 311
+         firstlineno 313
          lnotab 0x020b1c01040158011e0104011001
       ((None, None),)
       (None,)
       ('',)
       ('', '')
       (False,)
       (100, 0, -1)
@@ -1740,9 +1754,9 @@
    freevars   ()
    cellvars   ()
    filename   'build/bdist.linux-x86_64/egg/abstract_gui/simple_gui/gui_template.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c01140108011a012a010e03280106030c04180d12100e
-      0a160d0e0c120d160e160e220e060f4615100e5e170814060e060912173c
+      0a160d0e0c120d160e160e220e060f4615100e5e170816060e060912173c
       0f3814
```

