# Comparing `tmp/chromahackerweb-0.1.3.tar.gz` & `tmp/chromahackerweb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromahackerweb-0.1.3.tar", max compression
+gzip compressed data, was "chromahackerweb-0.2.0.tar", max compression
```

## Comparing `chromahackerweb-0.1.3.tar` & `chromahackerweb-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      918 2023-07-22 03:33:39.245500 chromahackerweb-0.1.3/README.md
--rw-r--r--   0        0        0     6148 2023-06-29 18:39:26.234949 chromahackerweb-0.1.3/chromahackerweb/.DS_Store
--rw-r--r--   0        0        0      859 2023-07-21 22:36:50.868048 chromahackerweb-0.1.3/chromahackerweb/__main__.py
--rw-r--r--   0        0        0     2246 2023-07-22 03:32:37.050291 chromahackerweb-0.1.3/chromahackerweb/static/script.js
--rw-r--r--   0        0        0     2399 2023-07-21 20:44:24.223814 chromahackerweb-0.1.3/chromahackerweb/static/style.css
--rw-r--r--   0        0        0      494 2023-07-21 20:33:05.082842 chromahackerweb-0.1.3/chromahackerweb/templates/index.html
--rw-r--r--   0        0        0      385 2023-07-22 03:34:51.028625 chromahackerweb-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 chromahackerweb-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-07-22 03:33:39.245500 chromahackerweb-0.2.0/README.md
+-rw-r--r--   0        0        0     6148 2023-06-29 18:39:26.234949 chromahackerweb-0.2.0/chromahackerweb/.DS_Store
+-rw-r--r--   0        0        0     2023 2023-07-28 02:20:16.687184 chromahackerweb-0.2.0/chromahackerweb/__main__.py
+-rw-r--r--   0        0        0     3019 2023-07-22 23:54:03.236722 chromahackerweb-0.2.0/chromahackerweb/static/script.js
+-rw-r--r--   0        0        0     2904 2023-07-23 00:40:20.435259 chromahackerweb-0.2.0/chromahackerweb/static/style.css
+-rw-r--r--   0        0        0     1034 2023-07-23 00:41:42.982740 chromahackerweb-0.2.0/chromahackerweb/templates/index.html
+-rw-r--r--   0        0        0      817 2023-07-22 04:24:21.139573 chromahackerweb-0.2.0/chromahackerweb/wezterm_import.py
+-rw-r--r--   0        0        0      385 2023-07-28 02:20:41.967346 chromahackerweb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 chromahackerweb-0.2.0/PKG-INFO
```

### Comparing `chromahackerweb-0.1.3/README.md` & `chromahackerweb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chromahackerweb-0.1.3/chromahackerweb/.DS_Store` & `chromahackerweb-0.2.0/chromahackerweb/.DS_Store`

 * *Files identical despite different names*

### Comparing `chromahackerweb-0.1.3/chromahackerweb/static/script.js` & `chromahackerweb-0.2.0/chromahackerweb/static/script.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-const myForm = document.getElementById('form');
+const myForm = document.getElementById('custom_form');
 const addButton = document.getElementById('addButton');
 const removeButton = document.getElementById('removeButton');
 
 function convertButtonToArg(str) {
     // Use a regular expression to match "button" followed by a number
     const regex = /^button(\d+)$/;
 
@@ -68,8 +68,29 @@
     div.appendChild(newInput);
     div.appendChild(newButton);
     myForm.appendChild(div);
 
 
     // Increment the input count
     inputCount++;
-});
+});
+
+function openForm(evt, name) {
+    // Declare all variables
+    var i, tabcontent, tablinks;
+
+    // Get all elements with class="tabcontent" and hide them
+    tabcontent = document.getElementsByTagName("form");
+    for (i = 0; i < tabcontent.length; i++) {
+        tabcontent[i].style.display = "none";
+    }
+
+    // Get all elements with class="tablinks" and remove the class "active"
+    tablinks = document.getElementsByClassName("tablinks");
+    for (i = 0; i < tablinks.length; i++) {
+        tablinks[i].className = tablinks[i].className.replace(" active", "");
+    }
+
+    // Show the current tab, and add an "active" class to the button that opened the tab
+    document.getElementById(name).style.display = "block";
+    evt.currentTarget.className += " active";
+}
```

### Comparing `chromahackerweb-0.1.3/chromahackerweb/static/style.css` & `chromahackerweb-0.2.0/chromahackerweb/static/style.css`

 * *Files 20% similar despite different names*

```diff
@@ -11,37 +11,59 @@
 h1 {
 	font-size: 40px;
 	text-align: center;
 	margin-bottom: 30px;
 	text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.8);
 }
 
+/* Optional styling for active button (you may have this in your CSS already) */
+.tab button.active {
+	background-color: #00cccc;
+}
+
+
 /* Form styles */
-#form {
+#custom_form, #premade_form {
+	max-width: 600px;
+	margin: 0 auto;
+}
+
+.tab {
+	display: flex;
+	justify-content: space-between;
 	max-width: 600px;
 	margin: 0 auto;
 }
 
+.tab button {
+	width: 50%;
+	box-sizing: border-box; /* Include padding and border in the width calculation */
+	padding: 10px; /* Adjust padding as needed */
+	border: none;
+	background-color: #f1f1f1; /* Set background color for buttons */
+}
+
 input[type="url"],
-input[type="color"] {
+input[type="text"] {
 	display: block;
 	width: 100%;
 	margin-bottom: 20px;
 	padding: 10px;
 	border: 2px solid #00ffcc;
 	border-radius: 5px;
 	background-color: #222;
 	color: #fff;
 }
 input[type="submit"], #addButton {
 	margin-top: 10px;
 	margin-bottom: 10px;
 }
 
-input[type="submit"] {
+input[type="submit"],
+.tab button {
 	display: block;
 	width: 100%;
 	padding: 10px;
 	border: none;
 	border-radius: 5px;
 	background-color: #00ffcc;
 	color: #111;
```

### Comparing `chromahackerweb-0.1.3/PKG-INFO` & `chromahackerweb-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: chromahackerweb
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
 Author: FaunuX
 Author-email: judahpspiegel@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: chromahacker (>=0.2.5,<0.3.0)
+Requires-Dist: chromahacker (>=0.3.0,<0.4.0)
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ChromaHacker
 
 ChromaHacker is a simple palettizer that takes in an image url and produces a version of the image using the specified palette.
```

