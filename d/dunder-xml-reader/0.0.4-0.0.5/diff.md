# Comparing `tmp/dunder_xml_reader-0.0.4.tar.gz` & `tmp/dunder_xml_reader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dunder_xml_reader-0.0.4.tar", last modified: Thu Jul 27 03:03:04 2023, max compression
+gzip compressed data, was "dunder_xml_reader-0.0.5.tar", last modified: Fri Jul 28 15:29:34 2023, max compression
```

## Comparing `dunder_xml_reader-0.0.4.tar` & `dunder_xml_reader-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    52880 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/dunder_xml_reader/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/safe_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    52880 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 03:03:04.000000 dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-27 03:03:04.132629 dunder_xml_reader-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:03:04.128629 dunder_xml_reader-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/test/test_safe_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/test/test_xml_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-27 03:02:41.000000 dunder_xml_reader-0.0.4/test/test_xml_node_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:29:34.459928 dunder_xml_reader-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    53950 2023-07-28 15:29:34.459928 dunder_xml_reader-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13539 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:29:34.455928 dunder_xml_reader-0.0.5/dunder_xml_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/dunder_xml_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/dunder_xml_reader/safe_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/dunder_xml_reader/xml_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/dunder_xml_reader/xml_node_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:29:34.455928 dunder_xml_reader-0.0.5/dunder_xml_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    53950 2023-07-28 15:29:34.000000 dunder_xml_reader-0.0.5/dunder_xml_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-28 15:29:34.000000 dunder_xml_reader-0.0.5/dunder_xml_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 15:29:34.000000 dunder_xml_reader-0.0.5/dunder_xml_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 15:29:34.000000 dunder_xml_reader-0.0.5/dunder_xml_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-28 15:29:34.459928 dunder_xml_reader-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 15:29:34.459928 dunder_xml_reader-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/test/test_extract_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/test/test_safe_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/test/test_xml_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-28 15:29:06.000000 dunder_xml_reader-0.0.5/test/test_xml_node_list.py
```

### Comparing `dunder_xml_reader-0.0.4/LICENSE` & `dunder_xml_reader-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.4/PKG-INFO` & `dunder_xml_reader-0.0.5/dunder_xml_reader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dunder_xml_reader
-Version: 0.0.4
+Name: dunder-xml-reader
+Version: 0.0.5
 Summary: Pythonic XML parsing/reading
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,49 +696,49 @@
             </To>
         </Header>
     </cXML>
 
 It can be easily nagivated with the following Python code:
 
     >>> with open('order_request.xml') as infile:
-    ...     cxml = dunder_xml_reader.parse_xml(infile.read())
+    ...     xml = dunder_xml_reader.parse_xml(infile.read())
     >>>
-    >>> print(cxml['payloadID'])
+    >>> print(xml['payloadID'])
     1233444-2001@premier.workchairs.com
     >>>
-    >>> print(cxml.Header.To.Credential[0].Identity.text())
+    >>> print(xml.Header.To.Credential[0].Identity.text())
     bigadmin@marketplace.org
     >>>
 
-As you can see, the property `payloadID` is accessed as if it were a dictionary key of the `cxml`
+As you can see, the property `payloadID` is accessed as if it were a dictionary key of the `xml`
 object.  Likewise, the `Header` child node of the cXML document is accessed as if it were an
-attribute of the `cxml` object.
+attribute of the `xml` object.
 
 The Python object(s) returned by `parse_xml()` use Python _dunder methods_ to fulfill
 functionality provided by other Python built-ins:
 
     >>> # Python's "in" operator
     >>>
-    >>> 'payloadID' in cxml
+    >>> 'payloadID' in xml
     True
-    >>> 'someOtherThing' in cxml
+    >>> 'someOtherThing' in xml
     False
     >>>
 
     >>> # Python's "hasattr" function
     >>>
-    >>> hasattr(cxml, 'Header')
+    >>> hasattr(xml, 'Header')
     True
-    >> hasattr(cxml, 'Footer')
+    >> hasattr(xml, 'Footer')
     False
     >>>
 
     >>> # Python's "len" function
     >>>
-    >>> len(cxml.Header.To.Credential)
+    >>> len(xml.Header.To.Credential)
     2
     >>>
 
 The Python objects returns by `parse_xml()` have the following methods:
 
 * `tag()` - Returns the XML element tag (i.e. "&lt;cXML&gt;" returns 'cXML')
 * `text()` - Returns the text between the tag and it's closer (i.e. "&lt;p&gt;blah&lt;/p&gt;"
@@ -770,81 +770,81 @@
 
 ### Some Examples ###
 
 The following are some examples of how you can use the Python objects returns by `parse_xml()`:
 
 #### <a id="dict"></a> Getting property values by dereferencing as a dictionary ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> payload_id = cxml['payloadID']
+    >>> xml = parse_xml(raw_xml_text)
+    >>> payload_id = xml['payloadID']
     >>> print(payload_id)
     1233444-2001@premier.workchairs.com
     >>>
 
 You can even check to see if a property exists using Python's built-in `in` operator
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> 'payloadID' in cxml
+    >>> xml = parse_xml(raw_xml_text)
+    >>> 'payloadID' in xml
     True
-    >>> 'someOtherWeirdThing` in cxml
+    >>> 'someOtherWeirdThing` in xml
     False
 
 #### <a id="list"></a> Getting siblings by dereferencing as a list ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> second_credential = cxml.Header.To.Credential[1]
+    >>> xml = parse_xml(raw_xml_text)
+    >>> second_credential = xml.Header.To.Credential[1]
     >>> print(second_credential.Identity.text())
     admin@acme.com
     >>>
 
 A nice side effect of being able to dereference an CxmlNode as a list is that you can for-loop
 over CxmlNodes:
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> for cred in cxml.Header.To.Credential
+    >>> xml = parse_xml(raw_xml_text)
+    >>> for cred in xml.Header.To.Credential
     ...   print(cred['domain'], cred.Identity.text())
     ...
     AribaNetworkUserId bigadmin@marketplace.org
     AribaNetworkUserId admin@acme.com
     >>>
 
 You can also use the built-in `len()` function with CxmlNodes:
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(len(cxml.Header.To.Credential))
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(len(xml.Header.To.Credential))
     2
     >>>
 
 #### <a id="tag"></a> Looking up the original element name with the `.tag()` method ####
 
     >>> request = parse_xml(raw_xml_text).Request.ConfirmationRequest
     >>> print(request.tag())
     ConfirmationRequest
     >>>
 
 #### <a id="text"></a> Getting the inner-text of the element with the `.text()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> node = cxml.Header.From.Credential.Identity
+    >>> xml = parse_xml(raw_xml_text)
+    >>> node = xml.Header.From.Credential.Identity
     >>> print(node.text())
     942888711
     >>>
 
 #### <a id="first"></a> Getting the first of a list of siblings with the `.first()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> node = cxml.Header.To.Credential.first()
+    >>> xml = parse_xml(raw_xml_text)
+    >>> node = xml.Header.To.Credential.first()
     >>> print node['type']
     marketplace
     >>>
 
 #### <a id="last"></a> Getting the last of a list of siblings with the `.last()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(cxml.Header.To.Credential.last().Identity.text())
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(xml.Header.To.Credential.last().Identity.text())
     admin@acme.com
     >>>
 
 #### <a id="filter"></a> Filtering nodes with the `.filter()` method ####
 
     >>> extrinsics = parse_xml(raw_xml_text).Request.OrderRequest.OrderRequestHeader.Extrinsic
     >>> user_nodes = extrinsics.filter(lambda n: n['name'].startswith('User'))
@@ -898,23 +898,23 @@
     >>> print(address.PostalAddress.Street.join_text("\n"))
     1231 West Main Street
     Suite 6a
     >>>
 
 #### <a id="join_prop"></a> String joining with the `.join_prop()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(cxml.Header.From.Credential.join_prop('domain'))
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(xml.Header.From.Credential.join_prop('domain'))
     DUNS, CompanyName, InteropKey
     >>>
 
 ### XML with namespaces ###
 
 The `dunder_xml_reader` package can handle XML with varying defined namespaces.  It does
-this by optionally replacing namespaces in tags with a alias prefix.  Take the following XML
+this by optionally replacing namespaces in tags with an alias prefix.  Take the following XML
 for example:
 
     <?xml version="1.0" encoding="UTF-8"?>
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
         <ReceiveClaimResponse xmlns="http://insurance.com/webservices/ReceiveClaim.job">
           <ClaimResponse>
@@ -954,56 +954,81 @@
 graph for that matter) that will prevent errors like:
 
     TypeError: 'NoneType' object is not subscriptable
     AttributeError: 'NoneType' object has no attribute 'blah'
 
 A quick example.  Say you want to issue the following line of code:
 
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
 
-But, the XML that was parsed in order to create the `cxml` object doesn't have a `BillTo`
+But, the XML that was parsed in order to create the `xml` object doesn't have a `BillTo`
 element.  You'd expect to get the following exception:
 
     AttributeError: 'OrderRequestHeader' object has no attribute 'BillTo'
 
 Now you could test your way through the graph heirchy (aka _look-before-you-leap_):
 
-    >>> if hasattr(cxml, 'Request') and \
-    ...    hasattr(cxml.Request, 'OrderRequest') and \
-    ...    hasattr(cxml.Request.OrderRequest, 'OrderRequestHeader') and \
-    ...    hasattr(cxml.Request.OrderRequest.OrderRequestHeader, 'BillTo'):
-    ...   x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> if hasattr(xml, 'Request') and \
+    ...    hasattr(xml.Request, 'OrderRequest') and \
+    ...    hasattr(xml.Request.OrderRequest, 'OrderRequestHeader') and \
+    ...    hasattr(xml.Request.OrderRequest.OrderRequestHeader, 'BillTo'):
+    ...   x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     ... else:
     ...   x = ''
 
 Or, you could just wrap your assignment in a try/except (aka _ask-for-forgiveness_):
 
     >>> try:
-    ...   x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    ...   x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     ... except AttributeError:
     ...   x = ''
 
 But in both cases you're writing a lot of "check to see if it's really there"-type code.  The
 goal of SafeReference is to prevent that code from needing to be written in the first place.
 If your object-graph is wrapped in a SafeReference instance, it will check at each level
 for the requested attribute to be there or missing.  If it's there, it will return the
 requested attribute.  However, if it's not there, it will return a default-value.  Here's
 an example:
 
-    >>> cxml = parse_cxml(raw_xml_text_thats_missing_a_BillTo_element)
-    >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = safe_cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> xml = parse_xml(raw_xml_text_thats_missing_a_BillTo_element)
+    >>> safe_xml = safe_reference(xml, 'n/a')
+    >>> x = safe_xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     n/a
     >>>
 
 This result of `n/a` will be the result no matter what item is missing (`Request`, `OrderRequest`,
 `OrderRequestHeader`, `BillTo`, etc.) along the way.  If any of the objects in that long
 dereferencing are missing, the default will be returned.  However, if nothing is missing, the
 actual graph value will be returned.
 
-    >>> cxml = parse_cxml(raw_xml_text_with_nothing_missing)
-    >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> xml = parse_xml(raw_xml_text_with_nothing_missing)
+    >>> safe_xml = safe_reference(xml, 'n/a')
+    >>> x = safe_xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     New York
     >>>
+
+
+## Bonus 2: extract_namespaces() ##
+
+If you have a chunk of XML or a SOAP message that conains numerous namespace references, figuring
+our what the namespaces are (so you can pass them as an argument to the `parse_xml()`), you can use
+the `extract_namespaces()` function:
+
+    >>> from dunder_xml_reader import extract_namespaces
+    >>> xml = """
+    ...     <section xmlns="http://www.ibm.com/events" xmlns:bk="urn:loc.gov:books" xmlns:pi="urn:personalInformation"
+    ...              xmlns:isbn='urn:ISBN:0-395-36341-6'>
+    ...         <title>Book-Signing Event</title>
+    ...         <signing>
+    ...             <bk:author pi:title="Mr" pi:name="Jim Ross"/>
+    ...             <book bk:title="Writing COBOL for Fun and Profit" isbn:number="0426070806"/>
+    ...             <comment xmlns=''>What a great issue!</comment>
+    ...         </signing>
+    ...     </section>
+    ...  """
+    ...
+    >>> ns = extract_namespaces(xml)
+    >>> print(ns)
+    {(None, 'http://www.ibm.com/events'), ('bk', 'urn:loc.gov:books'), ('pi', 'urn:personalInformation'), ('isbn', 'urn:ISBN:0-395-36341-6') }
+    >>>
```

### Comparing `dunder_xml_reader-0.0.4/README.md` & `dunder_xml_reader-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,49 +20,49 @@
             </To>
         </Header>
     </cXML>
 
 It can be easily nagivated with the following Python code:
 
     >>> with open('order_request.xml') as infile:
-    ...     cxml = dunder_xml_reader.parse_xml(infile.read())
+    ...     xml = dunder_xml_reader.parse_xml(infile.read())
     >>>
-    >>> print(cxml['payloadID'])
+    >>> print(xml['payloadID'])
     1233444-2001@premier.workchairs.com
     >>>
-    >>> print(cxml.Header.To.Credential[0].Identity.text())
+    >>> print(xml.Header.To.Credential[0].Identity.text())
     bigadmin@marketplace.org
     >>>
 
-As you can see, the property `payloadID` is accessed as if it were a dictionary key of the `cxml`
+As you can see, the property `payloadID` is accessed as if it were a dictionary key of the `xml`
 object.  Likewise, the `Header` child node of the cXML document is accessed as if it were an
-attribute of the `cxml` object.
+attribute of the `xml` object.
 
 The Python object(s) returned by `parse_xml()` use Python _dunder methods_ to fulfill
 functionality provided by other Python built-ins:
 
     >>> # Python's "in" operator
     >>>
-    >>> 'payloadID' in cxml
+    >>> 'payloadID' in xml
     True
-    >>> 'someOtherThing' in cxml
+    >>> 'someOtherThing' in xml
     False
     >>>
 
     >>> # Python's "hasattr" function
     >>>
-    >>> hasattr(cxml, 'Header')
+    >>> hasattr(xml, 'Header')
     True
-    >> hasattr(cxml, 'Footer')
+    >> hasattr(xml, 'Footer')
     False
     >>>
 
     >>> # Python's "len" function
     >>>
-    >>> len(cxml.Header.To.Credential)
+    >>> len(xml.Header.To.Credential)
     2
     >>>
 
 The Python objects returns by `parse_xml()` have the following methods:
 
 * `tag()` - Returns the XML element tag (i.e. "&lt;cXML&gt;" returns 'cXML')
 * `text()` - Returns the text between the tag and it's closer (i.e. "&lt;p&gt;blah&lt;/p&gt;"
@@ -94,81 +94,81 @@
 
 ### Some Examples ###
 
 The following are some examples of how you can use the Python objects returns by `parse_xml()`:
 
 #### <a id="dict"></a> Getting property values by dereferencing as a dictionary ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> payload_id = cxml['payloadID']
+    >>> xml = parse_xml(raw_xml_text)
+    >>> payload_id = xml['payloadID']
     >>> print(payload_id)
     1233444-2001@premier.workchairs.com
     >>>
 
 You can even check to see if a property exists using Python's built-in `in` operator
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> 'payloadID' in cxml
+    >>> xml = parse_xml(raw_xml_text)
+    >>> 'payloadID' in xml
     True
-    >>> 'someOtherWeirdThing` in cxml
+    >>> 'someOtherWeirdThing` in xml
     False
 
 #### <a id="list"></a> Getting siblings by dereferencing as a list ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> second_credential = cxml.Header.To.Credential[1]
+    >>> xml = parse_xml(raw_xml_text)
+    >>> second_credential = xml.Header.To.Credential[1]
     >>> print(second_credential.Identity.text())
     admin@acme.com
     >>>
 
 A nice side effect of being able to dereference an CxmlNode as a list is that you can for-loop
 over CxmlNodes:
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> for cred in cxml.Header.To.Credential
+    >>> xml = parse_xml(raw_xml_text)
+    >>> for cred in xml.Header.To.Credential
     ...   print(cred['domain'], cred.Identity.text())
     ...
     AribaNetworkUserId bigadmin@marketplace.org
     AribaNetworkUserId admin@acme.com
     >>>
 
 You can also use the built-in `len()` function with CxmlNodes:
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(len(cxml.Header.To.Credential))
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(len(xml.Header.To.Credential))
     2
     >>>
 
 #### <a id="tag"></a> Looking up the original element name with the `.tag()` method ####
 
     >>> request = parse_xml(raw_xml_text).Request.ConfirmationRequest
     >>> print(request.tag())
     ConfirmationRequest
     >>>
 
 #### <a id="text"></a> Getting the inner-text of the element with the `.text()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> node = cxml.Header.From.Credential.Identity
+    >>> xml = parse_xml(raw_xml_text)
+    >>> node = xml.Header.From.Credential.Identity
     >>> print(node.text())
     942888711
     >>>
 
 #### <a id="first"></a> Getting the first of a list of siblings with the `.first()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> node = cxml.Header.To.Credential.first()
+    >>> xml = parse_xml(raw_xml_text)
+    >>> node = xml.Header.To.Credential.first()
     >>> print node['type']
     marketplace
     >>>
 
 #### <a id="last"></a> Getting the last of a list of siblings with the `.last()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(cxml.Header.To.Credential.last().Identity.text())
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(xml.Header.To.Credential.last().Identity.text())
     admin@acme.com
     >>>
 
 #### <a id="filter"></a> Filtering nodes with the `.filter()` method ####
 
     >>> extrinsics = parse_xml(raw_xml_text).Request.OrderRequest.OrderRequestHeader.Extrinsic
     >>> user_nodes = extrinsics.filter(lambda n: n['name'].startswith('User'))
@@ -222,23 +222,23 @@
     >>> print(address.PostalAddress.Street.join_text("\n"))
     1231 West Main Street
     Suite 6a
     >>>
 
 #### <a id="join_prop"></a> String joining with the `.join_prop()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(cxml.Header.From.Credential.join_prop('domain'))
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(xml.Header.From.Credential.join_prop('domain'))
     DUNS, CompanyName, InteropKey
     >>>
 
 ### XML with namespaces ###
 
 The `dunder_xml_reader` package can handle XML with varying defined namespaces.  It does
-this by optionally replacing namespaces in tags with a alias prefix.  Take the following XML
+this by optionally replacing namespaces in tags with an alias prefix.  Take the following XML
 for example:
 
     <?xml version="1.0" encoding="UTF-8"?>
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
         <ReceiveClaimResponse xmlns="http://insurance.com/webservices/ReceiveClaim.job">
           <ClaimResponse>
@@ -278,56 +278,81 @@
 graph for that matter) that will prevent errors like:
 
     TypeError: 'NoneType' object is not subscriptable
     AttributeError: 'NoneType' object has no attribute 'blah'
 
 A quick example.  Say you want to issue the following line of code:
 
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
 
-But, the XML that was parsed in order to create the `cxml` object doesn't have a `BillTo`
+But, the XML that was parsed in order to create the `xml` object doesn't have a `BillTo`
 element.  You'd expect to get the following exception:
 
     AttributeError: 'OrderRequestHeader' object has no attribute 'BillTo'
 
 Now you could test your way through the graph heirchy (aka _look-before-you-leap_):
 
-    >>> if hasattr(cxml, 'Request') and \
-    ...    hasattr(cxml.Request, 'OrderRequest') and \
-    ...    hasattr(cxml.Request.OrderRequest, 'OrderRequestHeader') and \
-    ...    hasattr(cxml.Request.OrderRequest.OrderRequestHeader, 'BillTo'):
-    ...   x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> if hasattr(xml, 'Request') and \
+    ...    hasattr(xml.Request, 'OrderRequest') and \
+    ...    hasattr(xml.Request.OrderRequest, 'OrderRequestHeader') and \
+    ...    hasattr(xml.Request.OrderRequest.OrderRequestHeader, 'BillTo'):
+    ...   x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     ... else:
     ...   x = ''
 
 Or, you could just wrap your assignment in a try/except (aka _ask-for-forgiveness_):
 
     >>> try:
-    ...   x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    ...   x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     ... except AttributeError:
     ...   x = ''
 
 But in both cases you're writing a lot of "check to see if it's really there"-type code.  The
 goal of SafeReference is to prevent that code from needing to be written in the first place.
 If your object-graph is wrapped in a SafeReference instance, it will check at each level
 for the requested attribute to be there or missing.  If it's there, it will return the
 requested attribute.  However, if it's not there, it will return a default-value.  Here's
 an example:
 
-    >>> cxml = parse_cxml(raw_xml_text_thats_missing_a_BillTo_element)
-    >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = safe_cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> xml = parse_xml(raw_xml_text_thats_missing_a_BillTo_element)
+    >>> safe_xml = safe_reference(xml, 'n/a')
+    >>> x = safe_xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     n/a
     >>>
 
 This result of `n/a` will be the result no matter what item is missing (`Request`, `OrderRequest`,
 `OrderRequestHeader`, `BillTo`, etc.) along the way.  If any of the objects in that long
 dereferencing are missing, the default will be returned.  However, if nothing is missing, the
 actual graph value will be returned.
 
-    >>> cxml = parse_cxml(raw_xml_text_with_nothing_missing)
-    >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> xml = parse_xml(raw_xml_text_with_nothing_missing)
+    >>> safe_xml = safe_reference(xml, 'n/a')
+    >>> x = safe_xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     New York
     >>>
+
+
+## Bonus 2: extract_namespaces() ##
+
+If you have a chunk of XML or a SOAP message that conains numerous namespace references, figuring
+our what the namespaces are (so you can pass them as an argument to the `parse_xml()`), you can use
+the `extract_namespaces()` function:
+
+    >>> from dunder_xml_reader import extract_namespaces
+    >>> xml = """
+    ...     <section xmlns="http://www.ibm.com/events" xmlns:bk="urn:loc.gov:books" xmlns:pi="urn:personalInformation"
+    ...              xmlns:isbn='urn:ISBN:0-395-36341-6'>
+    ...         <title>Book-Signing Event</title>
+    ...         <signing>
+    ...             <bk:author pi:title="Mr" pi:name="Jim Ross"/>
+    ...             <book bk:title="Writing COBOL for Fun and Profit" isbn:number="0426070806"/>
+    ...             <comment xmlns=''>What a great issue!</comment>
+    ...         </signing>
+    ...     </section>
+    ...  """
+    ...
+    >>> ns = extract_namespaces(xml)
+    >>> print(ns)
+    {(None, 'http://www.ibm.com/events'), ('bk', 'urn:loc.gov:books'), ('pi', 'urn:personalInformation'), ('isbn', 'urn:ISBN:0-395-36341-6') }
+    >>>
```

### Comparing `dunder_xml_reader-0.0.4/dunder_xml_reader/__init__.py` & `dunder_xml_reader-0.0.5/dunder_xml_reader/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -30,34 +30,47 @@
     >>>
     >>> safe_order = xml_doc.safe_reference(xml_doc, 'n/a')
     >>> print(safe_order.Header.MissingNode.Credential[0].text())
     n/a
     >>>
 
 """
+import re
 import xml.etree.ElementTree
 
-from dunder_xml_reader.xml_node import XmlNode
 from dunder_xml_reader.safe_reference import SafeReference
+from dunder_xml_reader.xml_node import XmlNode
 
 
 def parse_xml(raw_text: str, namespaces=None) -> XmlNode:
     """
     Parse raw_text as XML and return a XmlNode instance of the root.
     :param raw_text: string holding valid XML
     :param namespaces: dict of namespaces
     :return: XmlNode instance pointing to root of XML
     """
     node = xml.etree.ElementTree.fromstring(raw_text)
-    
-    return XmlNode(node=node, parent_node=None, raw_text=raw_text, \
-                   namespaces=namespaces)
+
+    return XmlNode(node=node, parent_node=None, raw_text=raw_text, namespaces=namespaces)
 
 
-def safe_reference(object, default='') -> SafeReference:
+def safe_reference(object, default='', wrap_methods=True) -> SafeReference:
     """
     Wrap object graph in a SafeReference instance.
     :param object: The object to wrap
     :param default: What should be returned instead of throwing Exception
+    :param wrap_methods: Should calls to methods return a SafeReference or the actual result?
     :return: SafeReference instance
     """
-    return SafeReference(object, default)
+    return SafeReference(object, default, wrap_methods)
+
+
+def extract_namespaces(xml: str) -> set:
+    namespaces = set()
+    pattern = r'xmlns(:[a-zA-Z0-9-]+)?=("|\')([^("|\')]+)("|\')'
+    matches = re.findall(pattern, xml)
+    for match in matches:
+        prefix, _, uri, _ = match
+        prefix = prefix.replace(':', '')
+        prefix = None if not prefix else prefix
+        namespaces.add((prefix, uri))
+    return namespaces
```

### Comparing `dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node.py` & `dunder_xml_reader-0.0.5/dunder_xml_reader/xml_node.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.4/dunder_xml_reader/xml_node_list.py` & `dunder_xml_reader-0.0.5/dunder_xml_reader/xml_node_list.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.4/dunder_xml_reader.egg-info/PKG-INFO` & `dunder_xml_reader-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dunder-xml-reader
-Version: 0.0.4
+Name: dunder_xml_reader
+Version: 0.0.5
 Summary: Pythonic XML parsing/reading
 Author-email: Steve Brettschneider <steve@bluehousefamily.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,49 +696,49 @@
             </To>
         </Header>
     </cXML>
 
 It can be easily nagivated with the following Python code:
 
     >>> with open('order_request.xml') as infile:
-    ...     cxml = dunder_xml_reader.parse_xml(infile.read())
+    ...     xml = dunder_xml_reader.parse_xml(infile.read())
     >>>
-    >>> print(cxml['payloadID'])
+    >>> print(xml['payloadID'])
     1233444-2001@premier.workchairs.com
     >>>
-    >>> print(cxml.Header.To.Credential[0].Identity.text())
+    >>> print(xml.Header.To.Credential[0].Identity.text())
     bigadmin@marketplace.org
     >>>
 
-As you can see, the property `payloadID` is accessed as if it were a dictionary key of the `cxml`
+As you can see, the property `payloadID` is accessed as if it were a dictionary key of the `xml`
 object.  Likewise, the `Header` child node of the cXML document is accessed as if it were an
-attribute of the `cxml` object.
+attribute of the `xml` object.
 
 The Python object(s) returned by `parse_xml()` use Python _dunder methods_ to fulfill
 functionality provided by other Python built-ins:
 
     >>> # Python's "in" operator
     >>>
-    >>> 'payloadID' in cxml
+    >>> 'payloadID' in xml
     True
-    >>> 'someOtherThing' in cxml
+    >>> 'someOtherThing' in xml
     False
     >>>
 
     >>> # Python's "hasattr" function
     >>>
-    >>> hasattr(cxml, 'Header')
+    >>> hasattr(xml, 'Header')
     True
-    >> hasattr(cxml, 'Footer')
+    >> hasattr(xml, 'Footer')
     False
     >>>
 
     >>> # Python's "len" function
     >>>
-    >>> len(cxml.Header.To.Credential)
+    >>> len(xml.Header.To.Credential)
     2
     >>>
 
 The Python objects returns by `parse_xml()` have the following methods:
 
 * `tag()` - Returns the XML element tag (i.e. "&lt;cXML&gt;" returns 'cXML')
 * `text()` - Returns the text between the tag and it's closer (i.e. "&lt;p&gt;blah&lt;/p&gt;"
@@ -770,81 +770,81 @@
 
 ### Some Examples ###
 
 The following are some examples of how you can use the Python objects returns by `parse_xml()`:
 
 #### <a id="dict"></a> Getting property values by dereferencing as a dictionary ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> payload_id = cxml['payloadID']
+    >>> xml = parse_xml(raw_xml_text)
+    >>> payload_id = xml['payloadID']
     >>> print(payload_id)
     1233444-2001@premier.workchairs.com
     >>>
 
 You can even check to see if a property exists using Python's built-in `in` operator
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> 'payloadID' in cxml
+    >>> xml = parse_xml(raw_xml_text)
+    >>> 'payloadID' in xml
     True
-    >>> 'someOtherWeirdThing` in cxml
+    >>> 'someOtherWeirdThing` in xml
     False
 
 #### <a id="list"></a> Getting siblings by dereferencing as a list ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> second_credential = cxml.Header.To.Credential[1]
+    >>> xml = parse_xml(raw_xml_text)
+    >>> second_credential = xml.Header.To.Credential[1]
     >>> print(second_credential.Identity.text())
     admin@acme.com
     >>>
 
 A nice side effect of being able to dereference an CxmlNode as a list is that you can for-loop
 over CxmlNodes:
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> for cred in cxml.Header.To.Credential
+    >>> xml = parse_xml(raw_xml_text)
+    >>> for cred in xml.Header.To.Credential
     ...   print(cred['domain'], cred.Identity.text())
     ...
     AribaNetworkUserId bigadmin@marketplace.org
     AribaNetworkUserId admin@acme.com
     >>>
 
 You can also use the built-in `len()` function with CxmlNodes:
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(len(cxml.Header.To.Credential))
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(len(xml.Header.To.Credential))
     2
     >>>
 
 #### <a id="tag"></a> Looking up the original element name with the `.tag()` method ####
 
     >>> request = parse_xml(raw_xml_text).Request.ConfirmationRequest
     >>> print(request.tag())
     ConfirmationRequest
     >>>
 
 #### <a id="text"></a> Getting the inner-text of the element with the `.text()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> node = cxml.Header.From.Credential.Identity
+    >>> xml = parse_xml(raw_xml_text)
+    >>> node = xml.Header.From.Credential.Identity
     >>> print(node.text())
     942888711
     >>>
 
 #### <a id="first"></a> Getting the first of a list of siblings with the `.first()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> node = cxml.Header.To.Credential.first()
+    >>> xml = parse_xml(raw_xml_text)
+    >>> node = xml.Header.To.Credential.first()
     >>> print node['type']
     marketplace
     >>>
 
 #### <a id="last"></a> Getting the last of a list of siblings with the `.last()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(cxml.Header.To.Credential.last().Identity.text())
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(xml.Header.To.Credential.last().Identity.text())
     admin@acme.com
     >>>
 
 #### <a id="filter"></a> Filtering nodes with the `.filter()` method ####
 
     >>> extrinsics = parse_xml(raw_xml_text).Request.OrderRequest.OrderRequestHeader.Extrinsic
     >>> user_nodes = extrinsics.filter(lambda n: n['name'].startswith('User'))
@@ -898,23 +898,23 @@
     >>> print(address.PostalAddress.Street.join_text("\n"))
     1231 West Main Street
     Suite 6a
     >>>
 
 #### <a id="join_prop"></a> String joining with the `.join_prop()` method ####
 
-    >>> cxml = parse_xml(raw_xml_text)
-    >>> print(cxml.Header.From.Credential.join_prop('domain'))
+    >>> xml = parse_xml(raw_xml_text)
+    >>> print(xml.Header.From.Credential.join_prop('domain'))
     DUNS, CompanyName, InteropKey
     >>>
 
 ### XML with namespaces ###
 
 The `dunder_xml_reader` package can handle XML with varying defined namespaces.  It does
-this by optionally replacing namespaces in tags with a alias prefix.  Take the following XML
+this by optionally replacing namespaces in tags with an alias prefix.  Take the following XML
 for example:
 
     <?xml version="1.0" encoding="UTF-8"?>
     <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
       <soapenv:Body>
         <ReceiveClaimResponse xmlns="http://insurance.com/webservices/ReceiveClaim.job">
           <ClaimResponse>
@@ -954,56 +954,81 @@
 graph for that matter) that will prevent errors like:
 
     TypeError: 'NoneType' object is not subscriptable
     AttributeError: 'NoneType' object has no attribute 'blah'
 
 A quick example.  Say you want to issue the following line of code:
 
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
 
-But, the XML that was parsed in order to create the `cxml` object doesn't have a `BillTo`
+But, the XML that was parsed in order to create the `xml` object doesn't have a `BillTo`
 element.  You'd expect to get the following exception:
 
     AttributeError: 'OrderRequestHeader' object has no attribute 'BillTo'
 
 Now you could test your way through the graph heirchy (aka _look-before-you-leap_):
 
-    >>> if hasattr(cxml, 'Request') and \
-    ...    hasattr(cxml.Request, 'OrderRequest') and \
-    ...    hasattr(cxml.Request.OrderRequest, 'OrderRequestHeader') and \
-    ...    hasattr(cxml.Request.OrderRequest.OrderRequestHeader, 'BillTo'):
-    ...   x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> if hasattr(xml, 'Request') and \
+    ...    hasattr(xml.Request, 'OrderRequest') and \
+    ...    hasattr(xml.Request.OrderRequest, 'OrderRequestHeader') and \
+    ...    hasattr(xml.Request.OrderRequest.OrderRequestHeader, 'BillTo'):
+    ...   x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     ... else:
     ...   x = ''
 
 Or, you could just wrap your assignment in a try/except (aka _ask-for-forgiveness_):
 
     >>> try:
-    ...   x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    ...   x = xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     ... except AttributeError:
     ...   x = ''
 
 But in both cases you're writing a lot of "check to see if it's really there"-type code.  The
 goal of SafeReference is to prevent that code from needing to be written in the first place.
 If your object-graph is wrapped in a SafeReference instance, it will check at each level
 for the requested attribute to be there or missing.  If it's there, it will return the
 requested attribute.  However, if it's not there, it will return a default-value.  Here's
 an example:
 
-    >>> cxml = parse_cxml(raw_xml_text_thats_missing_a_BillTo_element)
-    >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = safe_cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> xml = parse_xml(raw_xml_text_thats_missing_a_BillTo_element)
+    >>> safe_xml = safe_reference(xml, 'n/a')
+    >>> x = safe_xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     n/a
     >>>
 
 This result of `n/a` will be the result no matter what item is missing (`Request`, `OrderRequest`,
 `OrderRequestHeader`, `BillTo`, etc.) along the way.  If any of the objects in that long
 dereferencing are missing, the default will be returned.  However, if nothing is missing, the
 actual graph value will be returned.
 
-    >>> cxml = parse_cxml(raw_xml_text_with_nothing_missing)
-    >>> safe_cxml = safe_reference(cxml, 'n/a')
-    >>> x = cxml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
+    >>> xml = parse_xml(raw_xml_text_with_nothing_missing)
+    >>> safe_xml = safe_reference(xml, 'n/a')
+    >>> x = safe_xml.Request.OrderRequest.OrderRequestHeader.BillTo.Address.PostalAddress.City.text()
     >>> print(x)
     New York
     >>>
+
+
+## Bonus 2: extract_namespaces() ##
+
+If you have a chunk of XML or a SOAP message that conains numerous namespace references, figuring
+our what the namespaces are (so you can pass them as an argument to the `parse_xml()`), you can use
+the `extract_namespaces()` function:
+
+    >>> from dunder_xml_reader import extract_namespaces
+    >>> xml = """
+    ...     <section xmlns="http://www.ibm.com/events" xmlns:bk="urn:loc.gov:books" xmlns:pi="urn:personalInformation"
+    ...              xmlns:isbn='urn:ISBN:0-395-36341-6'>
+    ...         <title>Book-Signing Event</title>
+    ...         <signing>
+    ...             <bk:author pi:title="Mr" pi:name="Jim Ross"/>
+    ...             <book bk:title="Writing COBOL for Fun and Profit" isbn:number="0426070806"/>
+    ...             <comment xmlns=''>What a great issue!</comment>
+    ...         </signing>
+    ...     </section>
+    ...  """
+    ...
+    >>> ns = extract_namespaces(xml)
+    >>> print(ns)
+    {(None, 'http://www.ibm.com/events'), ('bk', 'urn:loc.gov:books'), ('pi', 'urn:personalInformation'), ('isbn', 'urn:ISBN:0-395-36341-6') }
+    >>>
```

### Comparing `dunder_xml_reader-0.0.4/pyproject.toml` & `dunder_xml_reader-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dunder_xml_reader"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Steve Brettschneider", email="steve@bluehousefamily.com" },
 ]
 description = "Pythonic XML parsing/reading"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dunder_xml_reader-0.0.4/test/test_safe_reference.py` & `dunder_xml_reader-0.0.5/test/test_safe_reference.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Unit tests for the safe_get module"""
 
 import pytest
 
-from dunder_xml_reader import parse_xml, safe_reference
+from dunder_xml_reader import parse_xml, safe_reference, SafeReference
 
 
 @pytest.fixture
 def xml_doc(sample_xml_text):
     return parse_xml(sample_xml_text)
 
 
@@ -138,7 +138,25 @@
         result.append(item.identity.text())
 
     # Then
     assert result == ['bigadmin@marketplace.org', 'admin@acme.com']
     assert sut.Header.To.Credential[2] == "isnt-there"  # Doesn't exist in the XML
 
 
+def test_safe_reference_wrap_methods_true(xml_doc):
+    # Given
+    sut = safe_reference(xml_doc)
+    # When
+    result = sut.Header.From.Credential[0].Identity.text()
+
+    # Then
+    assert isinstance(result, SafeReference)
+
+
+def test_safe_reference_wrap_methods_false(xml_doc):
+    # Given
+    sut = safe_reference(xml_doc, wrap_methods=False)
+    # When
+    result = sut.Header.From.Credential[0].Identity.text()
+
+    # Then
+    assert isinstance(result, str)
```

### Comparing `dunder_xml_reader-0.0.4/test/test_xml_node.py` & `dunder_xml_reader-0.0.5/test/test_xml_node.py`

 * *Files identical despite different names*

### Comparing `dunder_xml_reader-0.0.4/test/test_xml_node_list.py` & `dunder_xml_reader-0.0.5/test/test_xml_node_list.py`

 * *Files identical despite different names*

