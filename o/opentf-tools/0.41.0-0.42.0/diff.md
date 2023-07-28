# Comparing `tmp/opentf_tools-0.41.0-py3-none-any.whl.zip` & `tmp/opentf_tools-0.42.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 39576 bytes, number of entries: 14
--rw-r--r--  2.0 unx    27544 b- defN 23-Jul-11 10:24 opentf/tools/ctl.py
--rw-r--r--  2.0 unx     7773 b- defN 23-Jul-11 10:24 opentf/tools/ctlcommons.py
--rw-r--r--  2.0 unx    29452 b- defN 23-Jul-11 10:24 opentf/tools/ctlconfig.py
--rw-r--r--  2.0 unx     8138 b- defN 23-Jul-11 10:24 opentf/tools/ctlnetworking.py
--rw-r--r--  2.0 unx    10861 b- defN 23-Jul-11 10:24 opentf/tools/ctlqualitygate.py
--rw-r--r--  2.0 unx    29356 b- defN 23-Jul-11 10:24 opentf/tools/ctlworkflows.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Jul-11 10:24 opentf/tools/done.py
--rw-r--r--  2.0 unx     9391 b- defN 23-Jul-11 10:24 opentf/tools/ready.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1793 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1176 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/RECORD
-14 files, 140267 bytes uncompressed, 37624 bytes compressed:  73.2%
+Zip file size: 40055 bytes, number of entries: 14
+-rw-r--r--  2.0 unx    27544 b- defN 23-Jul-28 07:50 opentf/tools/ctl.py
+-rw-r--r--  2.0 unx     7773 b- defN 23-Jul-28 07:50 opentf/tools/ctlcommons.py
+-rw-r--r--  2.0 unx    29452 b- defN 23-Jul-28 07:50 opentf/tools/ctlconfig.py
+-rw-r--r--  2.0 unx     8878 b- defN 23-Jul-28 07:50 opentf/tools/ctlnetworking.py
+-rw-r--r--  2.0 unx    12037 b- defN 23-Jul-28 07:50 opentf/tools/ctlqualitygate.py
+-rw-r--r--  2.0 unx    29356 b- defN 23-Jul-28 07:50 opentf/tools/ctlworkflows.py
+-rw-r--r--  2.0 unx     3188 b- defN 23-Jul-28 07:50 opentf/tools/done.py
+-rw-r--r--  2.0 unx     9391 b- defN 23-Jul-28 07:50 opentf/tools/ready.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Jul-28 07:50 opentf_tools-0.42.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1793 b- defN 23-Jul-28 07:50 opentf_tools-0.42.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-28 07:50 opentf_tools-0.42.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      139 b- defN 23-Jul-28 07:50 opentf_tools-0.42.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-28 07:50 opentf_tools-0.42.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1176 b- defN 23-Jul-28 07:50 opentf_tools-0.42.0.dist-info/RECORD
+14 files, 142183 bytes uncompressed, 38103 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: opentf/tools/done.py
 Comment: 
 
 Filename: opentf/tools/ready.py
 Comment: 
 
-Filename: opentf_tools-0.41.0.dist-info/LICENSE
+Filename: opentf_tools-0.42.0.dist-info/LICENSE
 Comment: 
 
-Filename: opentf_tools-0.41.0.dist-info/METADATA
+Filename: opentf_tools-0.42.0.dist-info/METADATA
 Comment: 
 
-Filename: opentf_tools-0.41.0.dist-info/WHEEL
+Filename: opentf_tools-0.42.0.dist-info/WHEEL
 Comment: 
 
-Filename: opentf_tools-0.41.0.dist-info/entry_points.txt
+Filename: opentf_tools-0.42.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: opentf_tools-0.41.0.dist-info/top_level.txt
+Filename: opentf_tools-0.42.0.dist-info/top_level.txt
 Comment: 
 
-Filename: opentf_tools-0.41.0.dist-info/RECORD
+Filename: opentf_tools-0.42.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opentf/tools/ctlnetworking.py

```diff
@@ -187,16 +187,40 @@
 
 def _post(
     base_url: str,
     path: str = '',
     msg: Optional[str] = None,
     statuses=(200,),
     handler=None,
-    files=None,
-):
+    files: Optional[Dict[str, Any]] = None,
+) -> Dict[str, Any]:
+    """Post request.
+
+    If the query status is not in `statuses`, does not return.
+
+    If `handler` is specified, it is called with the `Response` object
+    when the query status code is not in `statuses`.  It is expected not
+    to return.
+
+    # Required parameters
+
+    - base_url: a string
+
+    # Optional parameters
+
+    - path: a string (an empty string by default)
+    - msg: a string or None (None by default)
+    - statuses: a tuple of integers (`(200,)`  by default)
+    - handler: a function of arity one or None (None by default)
+    - files: a dictionary or None (None by default)
+
+    # Returned value
+
+    A dictionary, the JSON content of the query.
+    """
     if msg is None:
         msg = f'Could not post to {base_url}{path}'
     try:
         what = requests.post(
             base_url + path,
             files=files,
             headers=HEADERS,
@@ -211,15 +235,15 @@
             sys.exit(1)
     except requests.exceptions.ConnectionError as err:
         _could_not_connect(base_url, err)
     except Exception as err:
         _error(msg + ': %s.', err)
         sys.exit(2)
 
-    return what
+    return what  # type: ignore
 
 
 def _delete(
     base_url: str,
     path: str = '',
     msg: Optional[str] = None,
     statuses=(200,),
```

## opentf/tools/ctlqualitygate.py

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, Dict, Iterable, List, Union
+from typing import Any, Dict, Iterable, List, NoReturn, Optional
 
 import sys
 
 from opentf.tools.ctlcommons import (
     _ensure_options,
     _is_command,
     _get_arg,
@@ -33,45 +33,47 @@
     _get_json,
     _post,
 )
 
 ########################################################################
 # Help messages
 
-GET_QUALITYGATE_HELP = '''Get qualitygate status for a workflow
+GET_QUALITYGATE_HELP = '''Get quality gate status for a workflow
 
 Examples:
   # Get the quality gate status of a workflow applying the specific quality gate from the definition file
   opentf-ctl get qualitygate 9ea3be45-ee90-4135-b47f-e66e4f793383 --using=my.qualitygate.yaml --mode=my.quality.gate
 
-  # Get the qualitygate status of a workflow applying the default strict quality gate (threshold=100%)
+  # Get the quality gate status of a workflow applying the default strict quality gate (threshold=100%)
   opentf-ctl get qualitygate 9ea3be45-ee90-4135-b47f-e66e4f793383
 
 Options:
-  --mode=my.quality.gate|strict|passing|... or -m=...: use the specific qualitygate from the definition file
+  --mode=my.quality.gate|strict|passing|... or -m=...: use the specific quality gate from the definition file
   or one of the default quality gates (strict with 100% threshold and passing with 0% threshold)
   --using=/path/to/definition.yaml: use the specific quality gate definition file.
+  --output=wide or -o wide: show additional information (rule threshold and scope).
+  --output=custom-columns= or -o custom-columns=: show specified information.
 
 Usage:
   opentf-ctl get qualitygate WORKFLOW_ID [--mode=mode] [options]
 
 Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
 '''
 
-DESCRIBE_QUALITYGATE_HELP = '''Get qualitygate status description for a workflow
+DESCRIBE_QUALITYGATE_HELP = '''Get quality gate status description for a workflow
 
 Examples:
   # Get the quality gate status description of a workflow applying the specific quality gate from the definition file
   opentf-ctl describe qualitygate 9ea3be45-ee90-4135-b47f-e66e4f793383 --using=my.qualitygate.yaml --mode=my.quality.gate
 
   # Get the qualitygate status description of a workflow applying the default strict quality gate (threshold=100%)
   opentf-ctl describe qualitygate 9ea3be45-ee90-4135-b47f-e66e4f793383
 
 Options:
-  --mode=my.quality.gate|strict|passing|... or -m=...: use the specific qualitygate from the definition file
+  --mode=my.quality.gate|strict|passing|... or -m=...: use the specific quality gate from the definition file
   or one of the default quality gates (strict with 100% threshold and passing with 0% threshold)
   --using=/path/to/definition.yaml: use the specific quality gate definition file.
 
 Usage:
   opentf-ctl describe qualitygate WORKFLOW_ID [--mode=mode] [options]
 
 Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
@@ -91,62 +93,82 @@
 WIDE_COLUMNS = (
     'RULE:rule',
     'RESULT:rule.result',
     'TESTS_IN_SCOPE:rule.tests_in_scope',
     'TESTS_FAILED:rule.tests_failed',
     'TESTS_PASSED:rule.tests_passed',
     'SUCCESS_RATIO:rule.success_ratio',
+    'THRESHOLD:rule.threshold',
     'SCOPE:rule.scope',
 )
 
+NOTEST = 'NOTEST'
+FAILURE = 'FAILURE'
+RUNNING = 'RUNNING'
+SUCCESS = 'SUCCESS'
+INVALIDSCOPE = 'INVALID_SCOPE'
+
+
 STATUS_TEMPLATES = {
-    'SUCCESS': 'Workflow {workflow_id} successfully passed the quality gate `{mode}` applying the rule `{rule}`.',
-    'FAILURE': 'Workflow {workflow_id} failed the quality gate `{mode}` applying the rule `{rule}`.',
-    'NOTEST': 'Workflow {workflow_id} contains no tests matching the quality gate `{mode}` rule `{rule}`.',
+    SUCCESS: 'Workflow {workflow_id} passed the quality gate `{mode}` applying the rule `{rule}`.',
+    FAILURE: 'Workflow {workflow_id} failed the quality gate `{mode}` applying the rule `{rule}`.',
+    NOTEST: 'Workflow {workflow_id} contains no tests matching the quality gate `{mode}` rule `{rule}`.',
+    INVALIDSCOPE: 'The quality gate `{mode}` rule `{rule}` scope `{scope}` is invalid.',
 }
 
+########################################################################
+
+
+def _fatal(*msg) -> NoReturn:
+    _error(*msg)
+    sys.exit(2)
+
 
 def _describe_qualitygate(workflow_id: str, mode: str, status: Dict[str, Any]) -> None:
     """Get quality gate results for a workflow in a pretty form."""
     for rule, data in status.items():
-        if data['result'] not in ('SUCCESS', 'NOTEST', 'FAILURE'):
+        if data['result'] not in (SUCCESS, NOTEST, FAILURE, INVALIDSCOPE):
             _error(
-                f'Unexpected quality gate result when applying rule `{rule}`: {data["result"]} (was expecting SUCCESS, FAILURE or NOTEST).'
+                f'Unexpected quality gate result when applying rule `{rule}`: {data["result"]} (was expecting {", ".join(STATUS_TEMPLATES)}).'
             )
             continue
         print(f'\n--------RESULTS: {mode}, {rule}--------\n')
-        print(_make_qualitygate_status_message(data['result'], workflow_id, mode, rule))
-        if data['result'] in ('SUCCESS', 'FAILURE'):
+        print(
+            _make_qualitygate_status_message(
+                data['result'], workflow_id, mode, rule, data.get('scope')
+            )
+        )
+        if data['result'] in (SUCCESS, FAILURE):
             print('\n    --------STATISTICS--------\n')
             print(f'    Tests in scope: {data["tests_in_scope"]}')
             print(f'    Tests failed:   {data["tests_failed"]}')
             print(f'    Tests passed:   {data["tests_passed"]}')
             print(f'    Success ratio:  {data["success_ratio"]}')
+            print(f'    Threshold:      {data["threshold"]}')
 
 
 def _make_qualitygate_status_message(
-    status: str, workflow_id: str, mode: str, rule: str
+    status: str, workflow_id: str, mode: str, rule: str, scope: Optional[str]
 ) -> str:
     return STATUS_TEMPLATES[status].format(
-        workflow_id=workflow_id, mode=mode, rule=rule
+        workflow_id=workflow_id, mode=mode, rule=rule, scope=scope
     )
 
 
-def _make_rule_row(name: str, definition, fields: List[str]) -> List[str]:
-    if definition['result'] not in ('SUCCESS', 'NOTEST', 'FAILURE'):
-        _error(
-            f'Unexpected quality gate result when applying rule `{name}`: {definition["result"]} (was expecting SUCCESS, FAILURE or NOTEST).'
+def _make_rule_row(name: str, data: Dict[str, Any], fields: List[str]) -> List[str]:
+    if data['result'] not in (SUCCESS, NOTEST, FAILURE, INVALIDSCOPE):
+        _fatal(
+            f'Unexpected quality gate result when applying rule `{name}`: {data["result"]} (was expecting {", ".join(STATUS_TEMPLATES)}).'
         )
-        sys.exit(2)
     row = []
     for field in fields:
         if field == 'rule':
             row.append(name)
-        elif field.startswith('rule.') and definition:
-            row.append(definition.get(field.split('.')[1], ''))
+        elif field.startswith('rule.') and data:
+            row.append(data.get(field.split('.')[1], ''))
         else:
             row.append('')
     return row
 
 
 def _generate_qualitygate_rows(
     status: Dict[str, Any], columns: Iterable[str]
@@ -154,113 +176,128 @@
     """Generate rows with quality gate results."""
     fields = [column.split(':')[1] for column in columns]
     return [
         _make_rule_row(name, definition, fields) for name, definition in status.items()
     ]
 
 
-def _get_qualitygate_status(workflow_id: str, mode: str) -> Union[str, Dict[str, Any]]:
-    _ensure_uuid(workflow_id)
-    result = _get_json(
-        _qualitygate(),
-        f'/workflows/{workflow_id}/qualitygate?mode={mode}',
-        statuses=(200, 404, 422),
-    )
-    return _process_qualitygate_result(result, workflow_id)
-
-
-def _process_qualitygate_result(result, workflow_id):
+def _process_qualitygate_result(
+    result: Dict[str, Any], workflow_id: str
+) -> Dict[str, Any]:
     if result.get('code') == 404:
-        _error(
+        _fatal(
             'Unknown workflow %s.  It is either too new, too old, or the provided '
             + 'workflow ID is incorrect.  You can use "opentf-ctl get workflows" to list '
             + 'the known workflow IDs.',
             workflow_id,
         )
-        sys.exit(2)
     if result.get('code') == 422:
-        _error(result.get('message'))
-        sys.exit(2)
+        _fatal(result.get('message'))
     if 'details' not in result or 'status' not in result.get('details', {}):
-        _error(
+        _fatal(
             'Unexpected response from qualitygate.  Was expecting a JSON object'
             + ' with a .details.status entry, got: %s.',
             str(result),
         )
-        sys.exit(2)
 
     return result['details']
 
 
-def _post_qualitygate_definition(workflow_id, using, mode):
-    _ensure_uuid(workflow_id)
+def _print_final_status(workflow_id, mode, status):
+    if status == FAILURE:
+        print(f'Workflow {workflow_id} failed the quality gate using mode {mode}.')
+        sys.exit(102)
+    if status == SUCCESS:
+        print(f'Workflow {workflow_id} passed the quality gate using mode {mode}.')
+    if status == NOTEST:
+        print(f'Workflow {workflow_id} contains no test matching quality gate scopes.')
+
+
+def _get_qualitygate_status(workflow_id: str, mode: str) -> Dict[str, Any]:
+    return _get_json(
+        _qualitygate(),
+        f'/workflows/{workflow_id}/qualitygate?mode={mode}',
+        statuses=(200, 404, 422),
+    )
+
+
+def _post_qualitygate_definition(workflow_id: str, using: str, mode: str):
     try:
         files = {'qualitygates': open(using, 'rb')}
-        result = _post(
+        return _post(
             _qualitygate(),
             f'/workflows/{workflow_id}/qualitygate?mode={mode}',
-            statuses=(200,),
+            statuses=(200, 404, 422),
             files=files,
         )
-        return _process_qualitygate_result(result, workflow_id)
     except FileNotFoundError as err:
         _file_not_found(using, err)
     except Exception as err:
-        _error(f'Exception while handling quality gate definition file: {err}')
-        sys.exit(2)
+        _fatal(f'Exception while handling quality gate definition file: {err}')
+
+
+def _query_qualitygate(
+    workflow_id: str, using: Optional[str], mode: str
+) -> Dict[str, Any]:
+    _ensure_uuid(workflow_id)
+    if using:
+        result = _post_qualitygate_definition(workflow_id, using, mode)
+    else:
+        result = _get_qualitygate_status(workflow_id, mode)
+    return _process_qualitygate_result(result, workflow_id)
 
 
-def get_qualitygate(workflow_id: str, mode: str, describe=False, using='') -> None:
+def get_qualitygate(
+    workflow_id: str, mode: str, describe: bool = False, using: Optional[str] = None
+) -> None:
     """Get qualitygate status.
 
     # Required parameter
 
     - workflow_id: a non-empty string (an UUID)
     - mode: a string
 
     # Raised exceptions
 
     Abort with an error code of 2 if the specified `workflow_id` is
     invalid or if an error occurred while contacting the orchestrator.
 
     Abort with an error code of 101 if the workflow is still running.
 
-    Abort with an error code of 102 if the qualitygate failed.
+    Abort with an error code of 102 if the quality gate failed.
     """
-    if using:
-        details = _post_qualitygate_definition(workflow_id, using, mode)
-    else:
-        details = _get_qualitygate_status(workflow_id, mode)
+    response = _query_qualitygate(workflow_id, using, mode)
 
-    status = details['status']
-    if status not in ('NOTEST', 'FAILURE', 'RUNNING', 'SUCCESS'):
-        _error(
-            'Unexpected workflow status from qualitygate service: %s (was expecting NOTEST,'
-            + ' SUCCESS, FAILURE, or RUNNING).',
+    status = response['status']
+    if status not in (NOTEST, FAILURE, RUNNING, SUCCESS, INVALIDSCOPE):
+        _fatal(
+            f'Unexpected workflow status from qualitygate service: %s (was expecting RUNNING, {", ".join(STATUS_TEMPLATES)}).',
             status,
         )
-        sys.exit(2)
-    if status == 'RUNNING':
+    if status == RUNNING:
         print(
             f'Workflow {workflow_id} is still running.  Please retry after workflow completion.'
         )
         sys.exit(101)
 
-    if (rules := details.get('rules')) is not None:
+    for msg in response.get('warnings', []):
+        _warning(msg)
+
+    if (rules := response.get('rules')) is not None:
+        for rule_name, rule in rules.items():
+            if rule['result'] == INVALIDSCOPE:
+                _error(f'Error in rule `{rule_name}`. {rule["message"]}')
+
         if describe:
             _describe_qualitygate(workflow_id, mode, rules)
         else:
             columns = _retrieve_columns_to_display(WIDE_COLUMNS, DEFAULT_COLUMNS)
             _emit_csv(_generate_qualitygate_rows(rules, columns), columns)
 
-    if status == 'FAILURE':
-        print(f'Workflow {workflow_id} failed the qualitygate using mode {mode}.')
-        sys.exit(102)
-    if status == 'NOTEST':
-        print(f'Workflow {workflow_id} contains no test matching quality gate scopes.')
+    _print_final_status(workflow_id, mode, status)
 
 
 ########################################################################
 # Helpers
 
 
 def print_qualitygate_help(args: List[str]):
```

## opentf/tools/ctlworkflows.py

```diff
@@ -428,15 +428,15 @@
             sys.exit(2)
 
 
 def _emit_prefix(event: Dict[str, Any], file=sys.stdout) -> None:
     cts = event['metadata'].get('creationTimestamp')
     job_id = event['metadata'].get('job_id')
     print(
-        f'[{cts[:-7] if cts else "":19}]',
+        f'[{cts[:19] if cts else "":19}]',
         f'[job {job_id}] ' if job_id else '',
         end='',
         file=file,
     )
 
 
 def _emit_command(
```

## Comparing `opentf_tools-0.41.0.dist-info/LICENSE` & `opentf_tools-0.42.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `opentf_tools-0.41.0.dist-info/METADATA` & `opentf_tools-0.42.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentf-tools
-Version: 0.41.0
+Version: 0.42.0
 Summary: OpenTestFactory Orchestrator Tools
 Home-page: https://opentestfactory.org/tools/
 Author: Martin Lafaix
 Author-email: mlafaix@henix.com
 Maintainer: Henix
 Maintainer-email: opentestfactory@henix.com
 License: Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)
```

