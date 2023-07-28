# Comparing `tmp/selectable_text-0.0.3.tar.gz` & `tmp/selectable_text-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selectable_text-0.0.3.tar", last modified: Fri Jul 21 21:43:04 2023, max compression
+gzip compressed data, was "selectable_text-0.0.4.tar", last modified: Fri Jul 28 04:14:42 2023, max compression
```

## Comparing `selectable_text-0.0.3.tar` & `selectable_text-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 21:43:04.996959 selectable_text-0.0.3/
--rw-r--r--   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:00:05.000000 selectable_text-0.0.3/LICENSE
--rw-r--r--   0 johnlithio   (501) staff       (20)      383 2023-07-21 20:00:05.000000 selectable_text-0.0.3/MANIFEST.in
--rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-21 21:43:04.996802 selectable_text-0.0.3/PKG-INFO
--rw-r--r--   0 johnlithio   (501) staff       (20)     3665 2023-07-21 20:00:05.000000 selectable_text-0.0.3/README.md
--rw-r--r--   0 johnlithio   (501) staff       (20)     1748 2023-07-21 21:41:30.000000 selectable_text-0.0.3/package.json
-drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 21:43:04.996076 selectable_text-0.0.3/selectable_text/
--rw-r--r--   0 johnlithio   (501) staff       (20)     1515 2023-07-21 21:43:00.000000 selectable_text-0.0.3/selectable_text/SelectableText.py
--rw-r--r--   0 johnlithio   (501) staff       (20)     2259 2023-07-21 20:00:05.000000 selectable_text-0.0.3/selectable_text/__init__.py
--rw-r--r--   0 johnlithio   (501) staff       (20)       78 2023-07-21 21:43:00.000000 selectable_text-0.0.3/selectable_text/_imports_.py
--rw-r--r--   0 johnlithio   (501) staff       (20)     1854 2023-07-21 21:43:00.000000 selectable_text-0.0.3/selectable_text/metadata.json
--rw-r--r--   0 johnlithio   (501) staff       (20)     1748 2023-07-21 21:43:00.000000 selectable_text-0.0.3/selectable_text/package-info.json
--rw-r--r--   0 johnlithio   (501) staff       (20)     4598 2023-07-21 21:42:59.000000 selectable_text-0.0.3/selectable_text/selectable_text.min.js
--rw-r--r--   0 johnlithio   (501) staff       (20)     9586 2023-07-21 21:42:59.000000 selectable_text-0.0.3/selectable_text/selectable_text.min.js.map
-drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-21 21:43:04.996590 selectable_text-0.0.3/selectable_text.egg-info/
--rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-21 21:43:04.000000 selectable_text-0.0.3/selectable_text.egg-info/PKG-INFO
--rw-r--r--   0 johnlithio   (501) staff       (20)      444 2023-07-21 21:43:04.000000 selectable_text-0.0.3/selectable_text.egg-info/SOURCES.txt
--rw-r--r--   0 johnlithio   (501) staff       (20)        1 2023-07-21 21:43:04.000000 selectable_text-0.0.3/selectable_text.egg-info/dependency_links.txt
--rw-r--r--   0 johnlithio   (501) staff       (20)       16 2023-07-21 21:43:04.000000 selectable_text-0.0.3/selectable_text.egg-info/top_level.txt
--rw-r--r--   0 johnlithio   (501) staff       (20)       38 2023-07-21 21:43:04.997010 selectable_text-0.0.3/setup.cfg
--rw-r--r--   0 johnlithio   (501) staff       (20)      510 2023-07-21 20:00:05.000000 selectable_text-0.0.3/setup.py
+drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-28 04:14:42.647129 selectable_text-0.0.4/
+-rw-r--r--   0 johnlithio   (501) staff       (20)        0 2023-07-21 20:00:05.000000 selectable_text-0.0.4/LICENSE
+-rw-r--r--   0 johnlithio   (501) staff       (20)      383 2023-07-21 20:00:05.000000 selectable_text-0.0.4/MANIFEST.in
+-rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-28 04:14:42.646972 selectable_text-0.0.4/PKG-INFO
+-rw-r--r--   0 johnlithio   (501) staff       (20)     3665 2023-07-21 20:00:05.000000 selectable_text-0.0.4/README.md
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1748 2023-07-28 04:12:43.000000 selectable_text-0.0.4/package.json
+drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-28 04:14:42.646117 selectable_text-0.0.4/selectable_text/
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1626 2023-07-28 04:12:53.000000 selectable_text-0.0.4/selectable_text/SelectableText.py
+-rw-r--r--   0 johnlithio   (501) staff       (20)     2259 2023-07-21 20:00:05.000000 selectable_text-0.0.4/selectable_text/__init__.py
+-rw-r--r--   0 johnlithio   (501) staff       (20)       78 2023-07-28 04:12:53.000000 selectable_text-0.0.4/selectable_text/_imports_.py
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1994 2023-07-28 04:12:53.000000 selectable_text-0.0.4/selectable_text/metadata.json
+-rw-r--r--   0 johnlithio   (501) staff       (20)     1748 2023-07-28 04:12:53.000000 selectable_text-0.0.4/selectable_text/package-info.json
+-rw-r--r--   0 johnlithio   (501) staff       (20)     4793 2023-07-28 04:12:52.000000 selectable_text-0.0.4/selectable_text/selectable_text.min.js
+-rw-r--r--   0 johnlithio   (501) staff       (20)    10117 2023-07-28 04:12:52.000000 selectable_text-0.0.4/selectable_text/selectable_text.min.js.map
+drwxr-xr-x   0 johnlithio   (501) staff       (20)        0 2023-07-28 04:14:42.646797 selectable_text-0.0.4/selectable_text.egg-info/
+-rw-r--r--   0 johnlithio   (501) staff       (20)      240 2023-07-28 04:14:42.000000 selectable_text-0.0.4/selectable_text.egg-info/PKG-INFO
+-rw-r--r--   0 johnlithio   (501) staff       (20)      444 2023-07-28 04:14:42.000000 selectable_text-0.0.4/selectable_text.egg-info/SOURCES.txt
+-rw-r--r--   0 johnlithio   (501) staff       (20)        1 2023-07-28 04:14:42.000000 selectable_text-0.0.4/selectable_text.egg-info/dependency_links.txt
+-rw-r--r--   0 johnlithio   (501) staff       (20)       16 2023-07-28 04:14:42.000000 selectable_text-0.0.4/selectable_text.egg-info/top_level.txt
+-rw-r--r--   0 johnlithio   (501) staff       (20)       38 2023-07-28 04:14:42.647178 selectable_text-0.0.4/setup.cfg
+-rw-r--r--   0 johnlithio   (501) staff       (20)      510 2023-07-21 20:00:05.000000 selectable_text-0.0.4/setup.py
```

### Comparing `selectable_text-0.0.3/README.md` & `selectable_text-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `selectable_text-0.0.3/package.json` & `selectable_text-0.0.4/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.4'"}*

```diff
@@ -42,9 +42,9 @@
         "build:backends": "dash-generate-components ./src/lib/components selectable_text -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `selectable_text-0.0.3/selectable_text/SelectableText.py` & `selectable_text-0.0.4/selectable_text/SelectableText.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,32 +7,34 @@
     """A SelectableText component.
 
 
 Keyword arguments:
 
 - id (string; optional)
 
+- rangetext (string; optional)
+
 - selected_text (string; optional)
 
 - selection_end (number; optional)
 
 - selection_start (number; optional)
 
-- text (string; required)
+- text (dash component; required)
 
 - width (string; optional)"""
-    _children_props = []
-    _base_nodes = ['children']
+    _children_props = ['text']
+    _base_nodes = ['text', 'children']
     _namespace = 'selectable_text'
     _type = 'SelectableText'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, width=Component.UNDEFINED, text=Component.REQUIRED, selected_text=Component.UNDEFINED, selection_start=Component.UNDEFINED, selection_end=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'selected_text', 'selection_end', 'selection_start', 'text', 'width']
+    def __init__(self, id=Component.UNDEFINED, width=Component.UNDEFINED, text=Component.REQUIRED, selected_text=Component.UNDEFINED, selection_start=Component.UNDEFINED, selection_end=Component.UNDEFINED, rangetext=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'rangetext', 'selected_text', 'selection_end', 'selection_start', 'text', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'selected_text', 'selection_end', 'selection_start', 'text', 'width']
+        self.available_properties = ['id', 'rangetext', 'selected_text', 'selection_end', 'selection_start', 'text', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['text']:
```

### Comparing `selectable_text-0.0.3/selectable_text/__init__.py` & `selectable_text-0.0.4/selectable_text/__init__.py`

 * *Files identical despite different names*

### Comparing `selectable_text-0.0.3/selectable_text/metadata.json` & `selectable_text-0.0.4/selectable_text/metadata.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9918619791666666%*

 * *Differences: {"'src/lib/components/SelectableText.react.js'": "{'props': {'text': {'type': {'name': "*

 * *                                                 "'element'}}, 'rangetext': OrderedDict([('type', "*

 * *                                                 "OrderedDict([('name', 'string')])), ('required', "*

 * *                                                 "False), ('description', '')])}}"}*

```diff
@@ -39,14 +39,21 @@
             "id": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
+            "rangetext": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
             "selected_text": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
@@ -71,15 +78,15 @@
                     "name": "func"
                 }
             },
             "text": {
                 "description": "",
                 "required": true,
                 "type": {
-                    "name": "string"
+                    "name": "element"
                 }
             },
             "width": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
```

### Comparing `selectable_text-0.0.3/selectable_text/package-info.json` & `selectable_text-0.0.4/selectable_text/package-info.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.4'"}*

```diff
@@ -42,9 +42,9 @@
         "build:backends": "dash-generate-components ./src/lib/components selectable_text -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

### Comparing `selectable_text-0.0.3/selectable_text/selectable_text.min.js` & `selectable_text-0.0.4/selectable_text/selectable_text.min.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -4,55 +4,55 @@
             n: e => {
                 var n = e && e.__esModule ? () => e.default : () => e;
                 return t.d(n, {
                     a: n
                 }), n
             },
             d: (e, n) => {
-                for (var r in n) t.o(n, r) && !t.o(e, r) && Object.defineProperty(e, r, {
+                for (var o in n) t.o(n, o) && !t.o(e, o) && Object.defineProperty(e, o, {
                     enumerable: !0,
-                    get: n[r]
+                    get: n[o]
                 })
             },
             o: (e, t) => Object.prototype.hasOwnProperty.call(e, t),
             r: e => {
                 "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
                     value: "Module"
                 }), Object.defineProperty(e, "__esModule", {
                     value: !0
                 })
             }
         },
         n = function() {
             var e = document.currentScript;
             if (!e) {
-                for (var t = document.getElementsByTagName("script"), n = [], r = 0; r < t.length; r++) n.push(t[r]);
+                for (var t = document.getElementsByTagName("script"), n = [], o = 0; o < t.length; o++) n.push(t[o]);
                 e = (n = n.filter((function(e) {
                     return !e.async && !e.text && !e.textContent
                 }))).slice(-1)[0]
             }
             return e
         };
     if (Object.defineProperty(t, "p", {
             get: (e = n().src.split("/").slice(0, -1).join("/") + "/", function() {
                 return e
             })
         }), "undefined" != typeof jsonpScriptSrc) {
-        var r = jsonpScriptSrc;
+        var o = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
-            var t, o = (t = n(), /\/_dash-component-suites\//.test(t.src)),
-                i = r(e);
-            if (!o) return i;
+            var t, r = (t = n(), /\/_dash-component-suites\//.test(t.src)),
+                i = o(e);
+            if (!r) return i;
             var c = i.split("/"),
                 u = c.slice(-1)[0].split(".");
-            return u.splice(1, 0, "v0_0_3m1689975780"), c.splice(-1, 1, u.join(".")), c.join("/")
+            return u.splice(1, 0, "v0_0_4m1690517573"), c.splice(-1, 1, u.join(".")), c.join("/")
         }
     }
-    var o = {};
-    t.r(o), t.d(o, {
+    var r = {};
+    t.r(r), t.d(r, {
         SelectableText: () => d
     });
     const i = window.React;
     var c = t.n(i);
     const u = window.PropTypes;
     var s = t.n(u);
 
@@ -60,35 +60,35 @@
         return l = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         }, l(e)
     }
 
-    function p(e, t) {
+    function f(e, t) {
         for (var n = 0; n < t.length; n++) {
-            var r = t[n];
-            r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, (void 0, o = function(e, t) {
+            var o = t[n];
+            o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, (void 0, r = function(e, t) {
                 if ("object" !== l(e) || null === e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
-                    var r = n.call(e, "string");
-                    if ("object" !== l(r)) return r;
+                    var o = n.call(e, "string");
+                    if ("object" !== l(o)) return o;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return String(e)
-            }(r.key), "symbol" === l(o) ? o : String(o)), r)
+            }(o.key), "symbol" === l(r) ? r : String(r)), o)
         }
-        var o
+        var r
     }
 
-    function f(e, t) {
-        return f = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+    function p(e, t) {
+        return p = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
             return e.__proto__ = t, e
-        }, f(e, t)
+        }, p(e, t)
     }
 
     function a(e) {
         return a = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         }, a(e)
     }
@@ -99,28 +99,28 @@
                 constructor: {
                     value: e,
                     writable: !0,
                     configurable: !0
                 }
             }), Object.defineProperty(e, "prototype", {
                 writable: !1
-            }), t && f(e, t)
+            }), t && p(e, t)
         }(u, e);
-        var t, n, r, o, i = (r = u, o = function() {
+        var t, n, o, r, i = (o = u, r = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }(), function() {
-            var e, t = a(r);
-            if (o) {
+            var e, t = a(o);
+            if (r) {
                 var n = a(this).constructor;
                 e = Reflect.construct(t, arguments, n)
             } else e = t.apply(this, arguments);
             return function(e, t) {
                 if (t && ("object" === l(t) || "function" == typeof t)) return t;
                 if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
                 return function(e) {
@@ -139,28 +139,31 @@
             key: "mouseEvent",
             value: function() {
                 var e = "";
                 if (window.getSelection && (e = window.getSelection().toString()), !e || !e.length) return !1;
                 this.props.setProps({
                     selected_text: e,
                     selection_start: window.getSelection().anchorOffset,
-                    selection_end: window.getSelection().focusOffset
+                    selection_end: window.getSelection().focusOffset,
+                    rangetext: window.getSelection().getRangeAt(0).toString(),
+                    startoffset: window.getSelection().getRangeAt(0).startoffset,
+                    endoffset: window.getSelection().getRangeAt(0).endOffset
                 })
             }
         }, {
             key: "onMouseUp",
             value: function(e) {
-                var t, n, r = this;
+                var t, n, o = this;
                 (t = function() {
-                    r.doucleckicked ? (r.doucleckicked = !1, r.dismissMouseUp++) : r.dismissMouseUp > 0 ? r.dismissMouseUp-- : r.mouseEvent.bind(r)()
+                    o.doucleckicked ? (o.doucleckicked = !1, o.dismissMouseUp++) : o.dismissMouseUp > 0 ? o.dismissMouseUp-- : o.mouseEvent.bind(o)()
                 }, 200, function() {
                     var e = this,
-                        r = arguments;
+                        o = arguments;
                     clearTimeout(n), n = setTimeout((function() {
-                        n = null, t.apply(e, r)
+                        n = null, t.apply(e, o)
                     }), 200)
                 }).bind(this)()
             }
         }, {
             key: "onDoubleClick",
             value: function(e) {
                 e.stopPropagation(), this.doucleckicked = !0, this.mouseEvent.bind(this)()
@@ -177,22 +180,23 @@
                         margin: "10px",
                         width: this.props.width
                     },
                     onMouseUp: this.onMouseUp.bind(this),
                     onDoubleClick: this.onDoubleClick.bind(this)
                 }, this.props.text)
             }
-        }], n && p(t.prototype, n), Object.defineProperty(t, "prototype", {
+        }], n && f(t.prototype, n), Object.defineProperty(t, "prototype", {
             writable: !1
         }), u
     }(i.Component);
     d.defaultProps = {}, d.propTypes = {
         id: s().string,
         width: s().string,
-        text: s().string.isRequired,
+        text: s().element.isRequired,
         selected_text: s().string,
         selection_start: s().number,
         selection_end: s().number,
+        rangetext: s().string,
         setProps: s().func
-    }, window.selectable_text = o
+    }, window.selectable_text = r
 })();
 //# sourceMappingURL=selectable_text.min.js.map
```

### Comparing `selectable_text-0.0.3/selectable_text/selectable_text.min.js.map` & `selectable_text-0.0.4/selectable_text/selectable_text.min.js.map`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8990960020371785%*

 * *Differences: {"'mappings'": "'mBACA,IC2BYA,ED3BRC,EAAsB,CEA1BA,EAAyBC,IACxB,IAAIC,EAASD,GAAUA,EAAOE,WAC7B,IAAOF,EAAiB,QACxB,IAAM,EAEP,OADAD,EAAoBI,EAAEF,EAAQ,CAAEG,EAAGH,IAC5BA,CAAM,ECLdF,EAAwB,CAACM,EAASC,KACjC,IAAI,IAAIC,KAAOD,EACXP,EAAoBS,EAAEF,EAAYC,KAASR,EAAoBS,EAAEH,EAASE,IAC5EE,OAAOC,eAAeL,EAASE,EAAK,CAAEI,YAAY,EAAMC,IAAKN,EAAWC,IAE1E,ECNDR,EAAwB,CAACc,EAAKC,IAAUL,OAAOM,UAAUC,eAAeC,KAAKJ,EAAKC,GCClFf,EAAyBM,IACH,oBAAXa,QAA0BA,OAAOC,aAC1CV,OAAOC,eAAeL,EAASa,OAAOC,YAAa,CAAEC,MAAO,WAE7DX,OAAOC,eAAeL,EAAS,aAAc,CAAEe, […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "selectable_text.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "url",
         "__webpack_require__",
         "module",
         "getter",
         "__esModule",
         "d",
@@ -66,14 +66,19 @@
         "props",
         "setProps",
         "selected_text",
         "selection_start",
         "anchorOffset",
         "selection_end",
         "focusOffset",
+        "rangetext",
+        "getRangeAt",
+        "startoffset",
+        "endoffset",
+        "endOffset",
         "event",
         "func",
         "timeout",
         "_this",
         "doucleckicked",
         "dismissMouseUp",
         "mouseEvent",
@@ -110,18 +115,18 @@
         "webpack:///webpack/runtime/make namespace object",
         "webpack:///external window \"React\"",
         "webpack:///external window \"PropTypes\"",
         "webpack:///./src/lib/components/SelectableText.react.js"
     ],
     "sourcesContent": [
         "// The require scope\nvar __webpack_require__ = {};\n\n",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_3m1689975780\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_4m1690517573\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"React\"];",
         "const __WEBPACK_NAMESPACE_OBJECT__ = window[\"PropTypes\"];",
-        "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n\nfunction debounce(func, wait, immediate) {\n    let timeout;\n\n    return function () {\n        const context = this, args = arguments;\n        const later = () => {\n            timeout = null;\n            if (!immediate) func.apply(context, args);\n        };\n        const callNow = immediate && !timeout;\n\n        clearTimeout(timeout);\n        timeout = setTimeout(later, wait);\n        if (callNow) func.apply(context, args);\n    };\n}\n\n\nexport default class SelectableText extends Component {\n\n    mouseEvent() {\n\n        let text = '';\n\n        if (window.getSelection) {\n            text = window.getSelection().toString();\n        }\n\n        if (!text || !text.length) {\n            return false;\n        }\n\n        this.props.setProps({\n            selected_text: text,\n            selection_start: window.getSelection().anchorOffset,\n            selection_end: window.getSelection().focusOffset,\n        })\n    }\n\n    onMouseUp(event) {\n        debounce(() => {\n            if (this.doucleckicked) {\n                this.doucleckicked = false;\n                this.dismissMouseUp++;\n            } else if (this.dismissMouseUp > 0) {\n                this.dismissMouseUp--;\n            } else {\n                this.mouseEvent.bind(this)();\n            }\n        }, 200).bind(this)();\n    }\n\n    onDoubleClick(event) {\n        event.stopPropagation();\n\n        this.doucleckicked = true;\n        this.mouseEvent.bind(this)();\n    }\n\n    render() {\n        return (\n            <div id={this.props.id}\n                style={{\n                    whiteSpace: 'pre-wrap',\n                    display: 'inline-block',\n                    verticalAlign: 'text-top',\n                    margin: '10px',\n                    width: this.props.width\n                }}\n                onMouseUp={this.onMouseUp.bind(this)}\n                onDoubleClick={this.onDoubleClick.bind(this)}>\n                {this.props.text}\n            </div>\n        );\n    }\n}\n\nSelectableText.defaultProps = {};\n\nSelectableText.propTypes = {\n    id: PropTypes.string,\n    width: PropTypes.string,\n    text: PropTypes.string.isRequired,\n    selected_text: PropTypes.string,\n    selection_start: PropTypes.number,\n    selection_end: PropTypes.number,\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};"
+        "import React, { Component } from 'react';\nimport PropTypes from 'prop-types';\n\n\nfunction debounce(func, wait, immediate) {\n    let timeout;\n\n    return function () {\n        const context = this, args = arguments;\n        const later = () => {\n            timeout = null;\n            if (!immediate) func.apply(context, args);\n        };\n        const callNow = immediate && !timeout;\n\n        clearTimeout(timeout);\n        timeout = setTimeout(later, wait);\n        if (callNow) func.apply(context, args);\n    };\n}\n\n\nexport default class SelectableText extends Component {\n\n    mouseEvent() {\n\n        let text = '';\n\n        if (window.getSelection) {\n            text = window.getSelection().toString();\n        }\n\n        if (!text || !text.length) {\n            return false;\n        }\n\n        this.props.setProps({\n            selected_text: text,\n            selection_start: window.getSelection().anchorOffset,\n            selection_end: window.getSelection().focusOffset,\n            rangetext: window.getSelection().getRangeAt(0).toString(),\n            startoffset: window.getSelection().getRangeAt(0).startoffset,\n            endoffset: window.getSelection().getRangeAt(0).endOffset,\n        })\n    }\n\n    onMouseUp(event) {\n        debounce(() => {\n            if (this.doucleckicked) {\n                this.doucleckicked = false;\n                this.dismissMouseUp++;\n            } else if (this.dismissMouseUp > 0) {\n                this.dismissMouseUp--;\n            } else {\n                this.mouseEvent.bind(this)();\n            }\n        }, 200).bind(this)();\n    }\n\n    onDoubleClick(event) {\n        event.stopPropagation();\n\n        this.doucleckicked = true;\n        this.mouseEvent.bind(this)();\n    }\n\n    render() {\n        return (\n            <div id={this.props.id}\n                style={{\n                    whiteSpace: 'pre-wrap',\n                    display: 'inline-block',\n                    verticalAlign: 'text-top',\n                    margin: '10px',\n                    width: this.props.width\n                }}\n                onMouseUp={this.onMouseUp.bind(this)}\n                onDoubleClick={this.onDoubleClick.bind(this)}>\n                {this.props.text}\n            </div>\n        );\n    }\n}\n\nSelectableText.defaultProps = {};\n\nSelectableText.propTypes = {\n    id: PropTypes.string,\n    width: PropTypes.string,\n    text: PropTypes.element.isRequired,\n    selected_text: PropTypes.string,\n    selection_start: PropTypes.number,\n    selection_end: PropTypes.number,\n    rangetext: PropTypes.string,\n    // startoffset: PropTypes.number,\n    // endoffset: PropTypes.number,\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};"
     ],
     "version": 3
 }
```

