# Comparing `tmp/bring_order-0.3.2.tar.gz` & `tmp/bring_order-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bring_order-0.3.2.tar", max compression
+gzip compressed data, was "bring_order-0.4.2.tar", max compression
```

## Comparing `bring_order-0.3.2.tar` & `bring_order-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-06-29 13:58:00.702863 bring_order-0.3.2/LICENSE
--rw-r--r--   0        0        0     3792 2023-06-29 13:58:00.702863 bring_order-0.3.2/README.md
--rw-r--r--   0        0        0       46 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/__init__.py
--rw-r--r--   0        0        0     8154 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/bodi.py
--rw-r--r--   0        0        0     3394 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/bogui.py
--rw-r--r--   0        0        0     9124 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/boutils.py
--rw-r--r--   0        0        0     2542 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/bringorder.py
--rw-r--r--   0        0        0    14410 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/deductive.py
--rw-r--r--   0        0        0    10184 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/inductive.py
--rw-r--r--   0        0        0        0 2023-06-29 13:58:00.702863 bring_order-0.3.2/bring_order/untitled
--rw-r--r--   0        0        0      568 2023-06-29 13:58:36.914316 bring_order-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4521 1970-01-01 00:00:00.000000 bring_order-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-28 17:07:08.121595 bring_order-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3792 2023-07-28 17:07:08.121595 bring_order-0.4.2/README.md
+-rw-r--r--   0        0        0       46 2023-07-28 17:07:08.121595 bring_order-0.4.2/bring_order/__init__.py
+-rw-r--r--   0        0        0    14497 2023-07-28 17:07:08.121595 bring_order-0.4.2/bring_order/bodi.py
+-rw-r--r--   0        0        0     3778 2023-07-28 17:07:08.121595 bring_order-0.4.2/bring_order/bogui.py
+-rw-r--r--   0        0        0     9124 2023-07-28 17:07:08.121595 bring_order-0.4.2/bring_order/boutils.py
+-rw-r--r--   0        0        0     4502 2023-07-28 17:07:08.125594 bring_order-0.4.2/bring_order/bringorder.py
+-rw-r--r--   0        0        0    18547 2023-07-28 17:07:08.125594 bring_order-0.4.2/bring_order/deductive.py
+-rw-r--r--   0        0        0    13334 2023-07-28 17:07:08.125594 bring_order-0.4.2/bring_order/inductive.py
+-rw-r--r--   0        0        0     2147 2023-07-28 17:07:08.125594 bring_order-0.4.2/bring_order/next_analysis.py
+-rw-r--r--   0        0        0     1040 2023-07-28 17:08:15.689787 bring_order-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4822 1970-01-01 00:00:00.000000 bring_order-0.4.2/PKG-INFO
```

### Comparing `bring_order-0.3.2/LICENSE` & `bring_order-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bring_order-0.3.2/README.md` & `bring_order-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bring_order-0.3.2/bring_order/bogui.py` & `bring_order-0.4.2/bring_order/bogui.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Methods for creating widgets"""
 from ipywidgets import widgets
+from ipyfilechooser import FileChooser
+
 
 class BOGui:
     """General methods for creating widgets"""
     def __init__(self):
         """Class constructor"""
 
     def create_button(self, desc: str, command, style='success', tooltip=''):
@@ -22,30 +24,32 @@
 
         returns:
             dictionary containing the buttons
 
         """
         button_list = {}
         for button in buttons:
-            new_button = self.create_button(desc=button[0],
-                                                  command=button[1],
-                                                  style=button[2])
+            new_button = self.create_button(
+                desc=button[1],
+                command=button[2],
+                style=button[3]
+            )
             button_list[button[0]] = new_button
         return button_list
 
     def create_message(self, value, style={'font_size': '15px'}):
         """Creates HTML"""
         message = widgets.HTML(value=value, style=style)
         return message
 
-    def create_error_message(self, value=''):
+    def create_error_message(self, value='', color='red'):
         """Creates HTML, color: red"""
         error = self.create_message(value=value,
                                     style={'font_size': '12px',
-                                           'text_color': 'red'})
+                                           'text_color': color})
         return error
 
     def create_input_field(self, default_value='', placeholder=''):
         """Creates input field"""
         input_field = widgets.Text(value=default_value, placeholder=placeholder)
         return input_field
 
@@ -93,7 +97,22 @@
             description=desc,
             disabled=False,
             font_size ="15px",
             layout={'width': 'max-content'}
         )
 
         return radiobuttons
+
+    def create_checkbox(self, desc):
+        '''Create checkbox'''
+        checkbox = widgets.Checkbox(
+            value=False, description=desc,
+            disabled=False, indent=False
+        )
+
+        return checkbox
+
+    def create_file_chooser(self):
+        """Creates a FileChooser object"""
+        file_chooser = FileChooser()
+
+        return file_chooser
```

### Comparing `bring_order-0.3.2/bring_order/boutils.py` & `bring_order-0.4.2/bring_order/boutils.py`

 * *Files identical despite different names*

### Comparing `bring_order-0.3.2/bring_order/deductive.py` & `bring_order-0.4.2/bring_order/deductive.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 """Deductive class"""
+import spacy
+import os
+#import en_core_web_sm
 from ipywidgets import widgets
 from IPython.display import display, Javascript, clear_output
 
 class Deductive:
     """Class that guides deductive analysis"""
-    def __init__(self, bogui, boutils, start_new):
+    def __init__(self, bogui, boutils, next_step):
         """Class constructor
         
         Args:
             bogui (BOGui)
             boutils (BOUtils)
-            start_new (function): Function to start new analysis with same data
+            next_step ([]): State variable that tracks the next step for the program 
         """
         self.cell_count = 0
-        self.start_new = start_new
+        self.next_step = next_step
         self.bogui = bogui
         self.boutils = boutils
         self.buttons = self.bogui.init_buttons(self.button_list)
         self.theory_desc = self.bogui.create_text_area('','Theory')
         #List of hypotheses: 0 = hypothesis, 1 = null hypothesis
         self.hypotheses = [
             self.bogui.create_input_field(),
             self.bogui.create_input_field()
         ]
         self.add_cells_int = self.bogui.create_int_text()
         self.conclusion = None
         self.data_limitations = [self.bogui.create_input_field('Data limitations missing')]
         self.result_description = self.bogui.create_text_area('','Results')
+        wd = os.getcwd()
+        cache_dir=os.getenv("cache_dir", wd)
+        model_path="en_core_web_sm/en_core_web_sm-3.6.0"
+        self.nlp = spacy.load(os.path.join(cache_dir,model_path))
 
     @property
     def button_list(self):
         """Buttons for deductive class.
 
         Returns:
-            list of tuples in format (description: str, command: func, style: str)"""
-        button_list = [('Open cells', self.open_cells, 'primary'),
-                       ('Delete last cell', self.delete_last_cell, 'danger'),
-                       ('Save', self.check_theory_and_hypotheses, 'success'),
-                       ('Clear hypotheses', self.clear_hypotheses, 'warning'),
-                       ('Yes', self.save_theory_and_hypotheses, 'success'),
-                       ('No', self.bad_hypotheses, 'warning'),
-                       ('Run cells', self.run_cells, 'warning'),
-                       ('Clear cells', self.clear_cells, 'danger'),
-                       ('New analysis', self.start_new_analysis, 'success'),
-                       ('Prepare new data', self.start_analysis_with_new_data, 'success'),
-                       ('All done', self.all_done, 'success'),
-                       ('Export to pdf', self.export_to_pdf, 'success'),
-                       ('Close BringOrder', self.no_export, 'success'),
-                       ('Clear theory', self.clear_theory, 'warning')]
+            list of tuples in format (tag: str, description: str, command: func, style: str)
+        """
+
+        button_list = [
+            ('open', 'Open cells', self.open_cells, 'primary'),
+            ('delete', 'Delete last cell', self.delete_last_cell, 'danger'),
+            ('save', 'Save and continue', self.submit_theory_and_hypotheses, 'success'),
+            ('validate', 'Validate input', self.__validate_theory_and_hypotheses, 'primary'),
+            ('clear_hypo', 'Clear hypotheses', self.clear_hypotheses, 'warning'),
+            ('yes', 'Yes', self.save_theory_and_hypotheses, 'success'),
+            ('no', 'No', self.bad_hypotheses, 'warning'),
+            ('run', 'Run cells', self.run_cells, 'warning'),
+            ('clear', 'Clear cells', self.clear_cells, 'danger'),
+            ('clear_theory', 'Clear theory', self.clear_theory, 'warning'),
+            ('save_results', 'Save', self.save_results, 'success')
+        ]
 
         return button_list
 
-    def __create_hypotheses_grid(self, empty_hypo_error='', empty_null_error=''):
+    def __create_hypotheses_grid(self, hypo_error='',
+                                null_error='',
+                                hypo_error_color='red',
+                                null_error_color='red'):
         """Creates the view for setting hypotheses
         
         Args:
             empty_hypo_error (str): error message for empty hypothesis, optional
             empty_null_error (str): error message for empty null hypothesis, optional
         """
         grid = widgets.AppLayout(
@@ -63,41 +74,43 @@
             left_sidebar = widgets.VBox([
                 self.bogui.create_label('Hypothesis (H1):'),
                 self.bogui.create_label('Null hypothesis (H0):')
             ]),
             center = widgets.VBox([
                 widgets.HBox([
                     self.hypotheses[0],
-                    self.bogui.create_error_message(empty_hypo_error)
+                    self.bogui.create_error_message(hypo_error, hypo_error_color)
+
                 ]),
                 widgets.HBox([
                     self.hypotheses[1],
-                    self.bogui.create_error_message(empty_null_error)
+                    self.bogui.create_error_message(null_error, null_error_color)
+
                 ]),
-                self.buttons['Clear hypotheses']
+                self.buttons['clear_hypo']
             ]),
-            footer = self.buttons['Save'],
+            footer = widgets.HBox([self.buttons['validate'], self.buttons['save']]),
             pane_widths = [1, 6, 0],
             grid_gap = '18px'
         )
 
         return grid
 
-    def __create_theory_grid(self, error=''):
+    def __create_theory_grid(self, error='', color='red'):
         """Creates the view for summarizing theory
         
         Args:
             error (str): error message, optional
         """
         grid = widgets.AppLayout(
             header=self.bogui.create_message('Describe the theory and insights:'),
             center=widgets.VBox([
                 self.theory_desc,
-                self.bogui.create_error_message(error),
-                self.buttons['Clear theory']
+                self.bogui.create_error_message(error, color),
+                self.buttons['clear_theory']
             ]),
             pane_widths=[1, 6, 0],
             grid_gap='12px'
         )
 
         return grid
 
@@ -130,29 +143,70 @@
             if item.value == '':
                 item.focus()
                 focused = item
                 break
 
         return focused
 
-    def get_error_messages(self):
-        """Returns error messages for empty theory, hypothesis, and null hypothesis
+    def _get_error_messages(self):
+
+        theory_error = 'The theory must be at least 8 characters and\
+             not contain special characters'
+        hypo_error= 'The hypothesis must be at least 8 characters and\
+             not contain special characters'
+        null_error = 'The null hypothesis must be at least 8 characters and\
+             not contain special characters'
+
+        if self._is_min_length(self.theory_desc.value)\
+            and self._is_not_al_num(self.theory_desc.value):
+            theory_error = ''
+        if self._is_min_length(self.hypotheses[0].value)\
+            and self._is_not_al_num(self.hypotheses[0].value):
+            hypo_error = ''
+        if self._is_min_length(self.hypotheses[1].value)\
+            and self._is_not_al_num(self.hypotheses[1].value):
+            null_error = ''
+
+        return (theory_error, hypo_error, null_error)
+
+    def _get_warning_messages(self):
+        """Calls functions that validate that both theory, hypothesis,
+        and null hypothesis includes a subject, a predicate and an object.
+        Returns error messages based on nlp validation.
         
         Returns:
             errors (tuple)
         """
-        empty_theory = 'You must describe your theory and insights'
-        empty_hypo = 'Hypothesis missing'
-        empty_null = 'Null hypothesis missing'
-
-        theory_error = empty_theory if self.theory_desc.value == '' else ''
-        empty_hypo_error = empty_hypo if self.hypotheses[0].value == '' else ''
-        empty_null_error = empty_null if self.hypotheses[1].value == '' else ''
+        theory_warning = 'Warning! The theory does not fill criteria of\
+             including a subject, a predicate and an object.'
+        hypo_warning = 'Warning! The hypothesis does not fill criteria of\
+             including a subject, a predicate and an object.'
+        null_warning = 'Warning! The null hypothesis does not fill criteria of\
+             including a subject, a predicate and an object.'
+
+        subject = 'nsubj'
+        subject_passive = 'nsubjpass'
+        predicate = 'V'
+        prep_object = 'pobj'
+        direct_object = 'dobj'
+
+        if self._nlp(self.theory_desc.value, subject, subject_passive)\
+            and self._nlp_predicate(self.theory_desc.value, predicate)\
+            and self._nlp(self.theory_desc.value, prep_object, direct_object):
+            theory_warning = ''
+        if self._nlp(self.hypotheses[0].value, subject, subject_passive)\
+            and self._nlp_predicate(self.hypotheses[0].value, predicate)\
+            and self._nlp(self.hypotheses[0].value, prep_object, direct_object):
+            hypo_warning = ''
+        if self._nlp(self.hypotheses[1].value, subject, subject_passive)\
+            and self._nlp_predicate(self.hypotheses[1].value, predicate)\
+            and self._nlp(self.hypotheses[1].value, prep_object, direct_object):
+            null_warning = ''
 
-        return (theory_error, empty_hypo_error, empty_null_error)
+        return (theory_warning, hypo_warning, null_warning)
 
     def __create_limitation_prompt(self):
         """Creates limitation prompt grid"""
 
         hypothesis_text = self.bogui.create_message(
             f'You have set hypothesis (H1): {self.hypotheses[0].value}'
         )
@@ -169,42 +223,80 @@
             '</br>'+ '<h4> Do the hypotheses fit within the limitations of the data set? </h4>' 
              + limitations)
 
         limitation_prompt = widgets.VBox([
             hypothesis_text,
             null_text,
             limitation_prompt_text,
-            widgets.HBox([self.buttons['Yes'], self.buttons['No']])
+            widgets.HBox([self.buttons['yes'], self.buttons['no']])
         ])
 
         return limitation_prompt
 
-    def check_theory_and_hypotheses(self, _=None):
+    def __implement_error_messages(self, error, warning):
+
+        if error:
+            return (error, 'red')
+        if warning:
+            return (warning, 'orange')
+        return ('','red')
+
+    def submit_theory_and_hypotheses(self, _=None):
+        """Calls check theory and hypothesis -
+            function with paramenter False indicating Save -button is clicked
+        """
+        self.check_theory_and_hypotheses(False)
+
+    def __validate_theory_and_hypotheses(self, _=None):
+        """Calls check theory and hypothesis -
+            function with paramenter False indicating Validate input -button is clicked
+        """
+        self.check_theory_and_hypotheses(True)
+
+    def check_theory_and_hypotheses(self, is_validate):
         """Checks theory and hypotheses and displays the prompt for
         the check against data limitations
         
         Returns:
             True/False: True if theory, hypothesis, and null hypothesis are all filled
         """
+        empty_theory_error, empty_hypo_error, empty_null_error = self._get_error_messages()
+        theory_warning, hypo_warning, null_warning = self._get_warning_messages()
 
-        # Set error messages
-        theory_error, empty_hypo_error, empty_null_error = self.get_error_messages()
-        theory_grid = self.__create_theory_grid(theory_error)
-        hypotheses_grid = self.__create_hypotheses_grid(empty_hypo_error, empty_null_error)
+        theory_error, theory_error_color = self.__implement_error_messages(empty_theory_error,
+                                                                        theory_warning)
+        hypo_error, hypo_error_color = self.__implement_error_messages(empty_hypo_error,
+                                                                    hypo_warning)
+        null_error, null_error_color = self.__implement_error_messages(empty_null_error,
+                                                                    null_warning)
+
+        theory_grid = self.__create_theory_grid(theory_error, theory_error_color)
+        hypotheses_grid = self.__create_hypotheses_grid(hypo_error, null_error,
+                                                        hypo_error_color, null_error_color)
+
+        is_show_limitation_prompt = True
+
+        # If errors exist in any of the fields
+        if len(empty_theory_error + empty_hypo_error + empty_null_error) > 0:
+            is_show_limitation_prompt=False
+
+        # If Validate - button is clicked and warnings exist
+        elif is_validate:
+            if len(theory_warning + hypo_warning + null_warning ) > 0:
+                is_show_limitation_prompt=False
 
-        # Show error messages if any of the required values are empty
-        if len(theory_error + empty_hypo_error + empty_null_error) > 0:
+        # Show errors or/and warnings
+        if not is_show_limitation_prompt:
             clear_output(wait=True)
             display(theory_grid)
             display(hypotheses_grid)
             self.focus_first_empty([self.theory_desc] + self.hypotheses)
-
             return False
 
-        # Show limitation prompt if all values are ok
+        # Show limitation prompt - all values are ok
         limitation_prompt = self.__create_limitation_prompt()
         clear_output(wait=True)
         display(limitation_prompt)
 
         return True
 
     def bad_hypotheses(self, _=None):
@@ -212,32 +304,32 @@
         theory_grid = self.__create_theory_grid()
         hypotheses_grid = self.__create_hypotheses_grid('Hypotheses must fit data limitations')
         clear_output(wait=True)
         display(theory_grid)
         display(hypotheses_grid)
         self.clear_hypotheses()
 
-    def format_hypotheses_and_theory(self):
+    def _format_hypotheses_and_theory(self):
         """Formats hypotheses and theory for markdown
         
         Returns:
             formatted_text (str)
         """
-        formatted_text = f'# Deductive analysis: {self.hypotheses[0].value}\\n'
+        formatted_text = f'## Testing hypothesis: {self.hypotheses[0].value}\\n'
         formatted_theory = '<br />'.join(self.theory_desc.value.split('\n'))
-        formatted_text += f'## Theory and insights\\n{formatted_theory}\\n'
+        formatted_text += f'### Theory and insights\\n{formatted_theory}\\n'
         hypotheses = f'- Hypothesis (H1): {self.hypotheses[0].value}\
         \\n- Null hypothesis (H0): {self.hypotheses[1].value}'
-        formatted_text += f'## Hypotheses\\n{hypotheses}\\n## Data analysis'
+        formatted_text += f'### Hypotheses\\n{hypotheses}\\n### Data analysis'
 
         return formatted_text
 
     def save_theory_and_hypotheses(self, _=None):
         """Saves theory and hypotheses and displays buttons for running code"""
-        text = self.format_hypotheses_and_theory()
+        text = self._format_hypotheses_and_theory()
         self.boutils.create_markdown_cells_above(1, text=text)
         cell_operations = self.__create_cell_operations_grid()
         clear_output(wait=True)
         display(cell_operations)
         self.add_cells_int.focus()
 
     def clear_hypotheses(self, _=None):
@@ -256,17 +348,17 @@
         """Button function for deleting the last code cell"""
         if self.cell_count > 0:
             self.boutils.delete_cell_above()
             self.cell_count -= 1
 
     def deactivate_cell_operations(self):
         """Deactivates buttons after runnig code block"""
-        self.buttons['Open cells'].disabled = True
-        self.buttons['Clear cells'].disabled = True
-        self.buttons['Delete last cell'].disabled = True
+        self.buttons['open'].disabled = True
+        self.buttons['clear'].disabled = True
+        self.buttons['delete'].disabled = True
 
     def __create_conclusion_grid(self):
         question = self.bogui.create_message(value='What happened?')
         conclusion_label = self.bogui.create_message(value='Accepted hypothesis:')
         self.conclusion = self.bogui.create_radiobuttons(
             options=[f'H1: {self.hypotheses[0].value}',
                      f'H0: {self.hypotheses[1].value}'])
@@ -276,19 +368,15 @@
         grid = widgets.AppLayout(
             header=question,
             left_sidebar=conclusion_label,
             center=self.conclusion,
             footer=widgets.VBox([
                 notes_label,
                 self.result_description,
-                widgets.HBox([
-                    self.buttons['New analysis'],
-                    self.buttons['Prepare new data'],
-                    self.buttons['All done']
-                ])
+                self.buttons['save_results']
             ]),
             pane_widths=['150px', 1, 0],
             pane_heights=['20px', '40px', 1],
             grid_gap='12px'
         )
 
         return grid
@@ -314,60 +402,76 @@
         """Creates widget grid"""
         cell_number_label = self.bogui.create_label('Add code cells for your analysis:')
 
         grid = widgets.GridspecLayout(2, 2, justify_items='center',
                                      width='70%', align_items='center')
         grid[1, 0] = widgets.HBox([cell_number_label, self.add_cells_int])
         grid[1, 1] = widgets.TwoByTwoLayout(
-            top_left=self.buttons['Open cells'],
-            bottom_left=self.buttons['Run cells'],
-            top_right=self.buttons['Delete last cell'],
-            bottom_right=self.buttons['Clear cells'])
+            top_left=self.buttons['open'],
+            bottom_left=self.buttons['run'],
+            top_right=self.buttons['delete'],
+            bottom_right=self.buttons['clear'])
 
         return grid
 
-    def save_results(self):
+    def save_results(self, _=None):
         """Prints results as markdown and hides widgets"""
-
+        clear_output(wait=True)
         text = (f'## Conclusion\\n### Accepted hypothesis: {self.conclusion.value[4:]}\\n'
                 f'The hypotheses were:\\n- Hypothesis (H1): {self.hypotheses[0].value}\\n'
                 f'- Null hypothesis (H0): {self.hypotheses[1].value}\\n')
 
         if self.result_description.value:
             formatted_description = '<br />'.join(self.result_description.value.split('\n'))
             text += f'### Notes\\n {formatted_description}'
 
         self.boutils.create_markdown_cells_above(1, text=text)
-        clear_output(wait=True)
+        self.next_step[0] = 'analysis_done'
 
-    def start_new_analysis(self, _=None):
-        """Button function to save results and star new analysis"""
-        self.save_results()
-        self.start_new()
-
-    def start_analysis_with_new_data(self, _=None):
-        """Button function to start over with new data"""
-        self.save_results()
-        self.boutils.execute_cell_from_current(1, 'BringOrder()')
-
-    def all_done(self, _=None):
-        """Button function to save results when ready."""
-        self.save_results()
-        export_view = widgets.HBox([
-            self.buttons['Export to pdf'],
-            self.buttons['Close BringOrder']
-        ])
-        display(export_view)
+    def _is_min_length(self, text):
+        if not text:
+            return False
+        text.replace(" ", "")
+        if len(text) < 8:
+            return False
+        return True
+
+    def _is_not_al_num(self, text):
+        if not text:
+            return False
+        special_characters = "[{]}@#^\\*()+_=<>/"
+        if any(c in special_characters for c in text):
+            return False
+        return True
+
+    def _nlp_predicate(self, text, sentence_element):
+        '''Checks that string contains at least one predicate.
+
+            Args:
+                text(str)
+            Return:
+                true: if sentence contain at least one verb
+                false: if value is empty or not contain verb
+        '''
+        words = self.nlp(text)
+        if any(word.tag_[0] == sentence_element for word in words):
+            return True
+
+        return False
+
+    def _nlp(self, text, sentence_element1, sentence_element2):
+        '''Checks that string contains at least one of the desired sentence elements.
+
+            Args:
+                text(str)
+            Return:
+                true: if sentence contain at least one verb
+                false: if value is empty or not contain verb
+        '''
+        words = self.nlp(text)
+        if any(word.dep_ == sentence_element1 or sentence_element2 for word in words):
+            return True
 
-    def export_to_pdf(self, _=None):
-        """Button function to export the notebook to pdf."""
-        #os.system('jupyter nbconvert Untitled.ipynb --to pdf')
-        clear_output(wait=False)
-        display(Javascript('print()'))
-        self.boutils.delete_cell_from_current(0)
-
-    def no_export(self, _=None):
-        """Button function to close widgets without exporting."""
-        self.boutils.delete_cell_from_current(0)
+        return False
 
     def __repr__(self):
         return ''
```

### Comparing `bring_order-0.3.2/bring_order/inductive.py` & `bring_order-0.4.2/bring_order/inductive.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,203 @@
 """Class for Inductive analysis"""
 from ipywidgets import widgets
 from IPython.display import display, clear_output, Javascript
 
 class Inductive:
     """Class that guides inductive analysis"""
-    def __init__(self, bogui, boutils, start_new):
+
+    def __init__(self, bogui, boutils, next_step):
         """Class constructor."""
+
         self.bogui = bogui
         self.utils = boutils
-        self.start_new = start_new
+        self.next_step = next_step
         self._cell_count = 0
         self.buttons = self.bogui.init_buttons(self.button_list)
+        self.preconceptions = [self.bogui.create_input_field('', 'Preconception 1')]
         self._add_cells_int = self.bogui.create_int_text()
         self._notes = self.bogui.create_text_area()
         self.conclusion = None
         self.summary = self.bogui.create_text_area('', 'Summary')
         self.empty_notes_error = self.bogui.create_error_message()
         self.observations = []
-        self.new_analysis_view = widgets.HBox([
-            self.buttons['New analysis'],
-            self.buttons['Prepare new data'],
-            self.buttons['All done']]
-        )
-        self.export_view = widgets.HBox([self.buttons['Export to pdf'],
-                                         self.buttons['Close BringOrder']])
 
     @property
     def button_list(self):
         """Buttons for Inductive class.
 
         Returns:
-            list of tuples in format (description: str, command: func, style: str) """
-        button_list = [('Open cells', self._open_cells, 'warning'),
-                   ('Delete last cell', self._delete_last_cell, 'danger'),
-                   ('Clear cells', self._clear_cells, 'danger'),
-                   ('Run cells', self._run_cells, 'primary'),
-                   ('New analysis', self._start_new_analysis, 'success'),
-                   ('Ready to summarize', self._execute_ready, 'primary'),
-                   ('Submit observation', self._new_observation, 'warning'),
-                   ('Submit summary', self._submit_summary, 'success'),
-                   ('Prepare new data', self._prepare_new_data_pressed, 'success'),
-                   ('All done', self._all_done, 'success'),
-                   ('Export to pdf', self._export_to_pdf, 'success'),
-                   ('Close BringOrder', self._no_export, 'success')]
+            list of tuples in format (tag: str, description: str, command: func, style: str)
+        """
+
+        button_list = [
+            ('add', 'Add preconception', self._add_preconception, 'primary'),
+            ('save', 'Save preconceptions', self._save_preconceptions, 'success'),
+            ('open', 'Open cells', self._open_cells, 'warning'),
+            ('delete', 'Delete last cell', self._delete_last_cell, 'danger'),
+            ('clear', 'Clear cells', self._clear_cells, 'danger'),
+            ('run', 'Run cells', self._run_cells, 'primary'),
+            ('ready', 'Ready to summarize', self._execute_ready, 'primary'),
+            ('submit_obs', 'Submit observation', self._new_observation, 'warning'),
+            ('submit_sum', 'Submit summary', self._submit_summary, 'success'),
+            ('lock', 'Lock evaluation', self._lock_evaluation_pressed, 'success'),
+            ('save_results', 'Save', self._save_results, 'success')
+        ]
 
         return button_list
 
+    def start_inductive_analysis(self):
+        """Starts inductive analysis."""
+
+        self.utils.create_markdown_cells_above(1, '## Data exploration')
+        display(self._create_preconception_grid())
+
+    def _add_preconception(self, _=None):
+        """Button function to add new preconception."""
+
+        self.preconceptions.append(
+            self.bogui.create_input_field('', f'Preconception {len(self.preconceptions) + 1}')
+        )
+
+        clear_output(wait=True)
+        display(self._create_preconception_grid())
+
+    def _check_preconceptions(self):
+        """Checks that at least one of the preconceptions has a non-empty value."""
+
+        for item in self.preconceptions:
+            if item.value != '':
+                return True
+
+        return False
+
+    def _format_preconceptions(self):
+        """Formats preconceptions for markdown.
+
+        Returns:
+            formatted_preconceptions (str)
+        """
+
+        formatted_preconceptions = '### Preconceptions\\n'
+        for item in self.preconceptions:
+            preconception_text = f'- {item.value}\\n'
+            formatted_preconceptions += preconception_text
+
+        formatted_preconceptions += '### Data analysis'
+        return formatted_preconceptions
+
+    def _save_preconceptions(self, _=None):
+        """Button function to save preconceptions as markdown and show cell operation buttons."""
+
+        clear_output(wait=True)
+
+        if self._check_preconceptions():
+            # Remove empty preconceptions from the list
+            self.preconceptions = list(filter(
+                lambda text_input: text_input.value != '',
+                self.preconceptions
+            ))
+
+            self.utils.create_markdown_cells_above(
+                how_many=1,
+                text=self._format_preconceptions()
+            )
+
+            display(self._create_cell_operations())
+
+        else:
+            display(self._create_preconception_grid(
+                error='You must name at least one preconception')
+            )
+
+    def _create_preconception_grid(self, error=''):
+        """Creates the grid with input fields and buttons to add and save preconceptions."""
+
+        preconceptions_label = self.bogui.create_message(
+                value='Write about your preconceptions concerning the data set:')
+
+        preconception_grid = widgets.AppLayout(
+            header=preconceptions_label,
+            center=widgets.VBox(self.preconceptions),
+            footer=widgets.VBox([
+                self.bogui.create_error_message(error),
+                widgets.HBox([
+                    self.buttons['add'],
+                    self.buttons['save']
+                ])
+            ]),
+            pane_heights=['30px', 1, '70px'],
+            grid_gap='12px'
+        )
+
+        return preconception_grid
+
     def _open_cells(self, _=None):
-        """Open cells button function that opens the selected
-        number of code cells"""
+        """Open cells button function that opens the selected number of code cells."""
+
         if self._add_cells_int.value > 0:
             self._cell_count += self._add_cells_int.value
             self.utils.create_code_cells_above(self._add_cells_int.value)
 
     def _delete_last_cell(self, _=None):
-        """Delete last cell-button function"""
+        """Delete last cell button function."""
+
         if self._cell_count > 0:
             self.utils.delete_cell_above()
             self._cell_count -= 1
 
     def _clear_cells(self, _=None):
         """Clears all code cells above."""
+
         self.utils.clear_code_cells_above(self._cell_count)
 
     def _buttons_disabled(self, disabled):
-        """Activates/deactivates buttons
+        """Activates/deactivates buttons.
         
         Args:
             disbled (bool): True to disable, False to activate
         """
 
-        self.buttons['Open cells'].disabled = disabled
-        self.buttons['Clear cells'].disabled = disabled
-        self.buttons['Delete last cell'].disabled = disabled
-        self.buttons['Ready to summarize'].disabled = disabled
+        self.buttons['open'].disabled = disabled
+        self.buttons['clear'].disabled = disabled
+        self.buttons['delete'].disabled = disabled
+        self.buttons['ready'].disabled = disabled
 
     def _run_cells(self, _=None):
         """Executes cells above and displays text area for observations of analysis."""
-        if self._cell_count == 0:
+
+        if self._cell_count <= 0:
             return
 
         self.utils.run_cells_above(self._cell_count)
         if self.conclusion:
             self.conclusion.close()
 
         self._buttons_disabled(True)
 
         notes_label = self.bogui.create_label(value='Explain what you observed:')
         self.conclusion = widgets.VBox([
             widgets.HBox([notes_label, self._notes]),
             self.empty_notes_error,
-            self.buttons['Submit observation']
+            self.buttons['submit_obs']
         ])
 
         display(self.conclusion)
 
     def _get_first_words(self, word_list):
         """Takes a word list and returns a string that has the first sentence or
         the first five words and three dots if the sentence is longer.
         
         Args:
             word_list (list)
             
         Returns:
             first_words (str)
         """
+
         first_words = f'{word_list[0]}'
 
         for word in word_list[1:5]:
             first_words += f' {word}'
             if any(mark in word for mark in ['.', '?', '!']):
                 return first_words.strip('.')
 
@@ -120,157 +209,175 @@
 
     def _format_observation(self):
         """Formats observation for markdown.
         
         Returns:
             formatted_obs (str)
         """
-        formatted_obs = f'## Observation {len(self.observations)}: '
+
+        formatted_obs = f'#### Observation {len(self.observations)}: '
 
         notes_list = self._notes.value.split('\n')
         first_line_list = notes_list[0].split(' ')
         first_words = self._get_first_words(first_line_list)
         formatted_obs += f'{first_words}\\n'
 
         notes = '<br />'.join(notes_list)
         formatted_obs += notes
 
         return formatted_obs
 
     def _new_observation(self, _=None):
-        """Checks new observation, saves it, and resets cell count"""
-        if self._check_notes():
+        """Checks new observation, saves it, and resets cell count."""
+
+        if self._check_value_not_empty(self._notes.value):
             self.observations.append(self._notes.value)
             text = self._format_observation()
             self.utils.create_markdown_cells_above(1, text=text)
             self._buttons_disabled(False)
             self.empty_notes_error.value = ''
             self.conclusion.close()
             self._notes.value = ''
             self._cell_count = 0
 
         else:
             self.empty_notes_error.value = 'Observation field can not be empty'
 
-    def _start_new_analysis(self, _=None):
-        """Starts new bringorder object with old data"""
-        clear_output(wait=True)
-        self.start_new()
-
-    def _prepare_new_data_pressed(self, _=None):
-        '''Starts new analysis with importing new data'''
-        self.utils.execute_cell_from_current(0, 'BringOrder()')
-
     def _execute_ready(self, _=None):
-        """Executes code cells after Ready to summarize button is clicked."""
-        clear_output(wait=True)
+        """Button function for Ready to summarize button."""
+
         self._display_summary()
 
     def _display_summary(self, error=''):
-        """Prints all observations and asks for summary"""
-        clear_output(wait=True)
+        """Prints all observations and asks for summary."""
 
         observations = "<ul>\n"
         observations += "\n".join(["<li>" + observation + "</li>"
                                  for observation in self.observations])
         observations += "\n</ul>"
 
         observation_list = widgets.HTML(
             '</br>'+'<h4>All your observations from the data:</h4>'+observations)
 
-        # observation_string = '\n'.join((f"Observation {i+1}: {observation}\n") for i, observation
-        #          in enumerate(self.observations))
-        # text = f'All your observations from the data:\n\n{observation_string}'
-        # print(text)
-
         summary_label = self.bogui.create_label('What do these observations mean?')
         error_message = self.bogui.create_error_message(value=error)
         grid = widgets.VBox([
             observation_list,
             widgets.HBox([summary_label, self.summary]),
             error_message,
-            self.buttons['Submit summary']
+            self.buttons['submit_sum']
         ])
+
+        clear_output(wait=True)
         display(grid)
 
     def _format_summary(self):
-        """Formats summary for markdown
+        """Formats summary for markdown.
         
         Returns:
             formatted_summary (str)
         """
-        formatted_summary = '## Summary: '
+
+        formatted_summary = '### Summary: '
 
         summary_list = self.summary.value.split('\n')
         first_line_list = summary_list[0].split(' ')
         first_words = self._get_first_words(first_line_list)
         formatted_summary += f'{first_words}\\n'
 
         summary = '<br />'.join(summary_list)
         formatted_summary += summary
 
         return formatted_summary
 
     def _submit_summary(self, _=None):
-        """Button function to submit summary"""
-        if self.summary.value == '':
+        """Button function to submit summary."""
+
+        if not self._check_value_not_empty(self.summary.value):
             self._display_summary(error='You must write some kind of summary')
             return
 
         text = self._format_summary()
         self.utils.create_markdown_cells_above(1, text=text)
+        self._evaluation_of_analysis()
+
+    def _evaluation_of_analysis(self, _=None):
+        self.buttons['submit_sum'].disabled = True
         clear_output(wait=False)
-        self.new_analysis()
+        grid = widgets.AppLayout(
+            header = self.bogui.create_message(
+                        'Evaluate how confident you are that analysis meet preconceptions?'),
+            center = widgets.IntSlider(value=50, min=0, max=100, step=5,
+                                        description='', disabled=False,
+                                        continuous_update=False,
+                                        orientation='horizontal',
+                                        readout=True, readout_format='d'
+                                        ),
+            right_sidebar = self.buttons['lock'],
+            footer = None
+            )
+        display(grid)
 
-    def _check_notes(self):
-        """Checks that text field was filled"""
-        if self._notes.value == '':
+    def _lock_evaluation_pressed(self, _=None):
+        clear_output(wait=False)
+        label = self.bogui.create_message('Did the analysis meet preconceptions?')
+        checkboxes = [widgets.Checkbox(
+                        description=prec.value, value=False,) for prec in self.preconceptions]
+        output = widgets.VBox(checkboxes)
+        display(label, output)
+        grid = widgets.AppLayout(
+            header = self.bogui.create_message('Overall how satisfied you are in the analysis?'),
+            center = widgets.SelectionSlider(
+                options=['Very dissatisfied','Dissatisfied','Neutral','Satisfied','Very satisfied'],
+                value = 'Neutral',
+                description='',
+                disabled=False, continuous_update=False,
+                orientation='horizontal', readout=True
+            ),
+            footer = None)
+        display(grid)
+        display(self.buttons['save_results'])
+    
+    def _save_results(self, _=None):
+        clear_output(wait=True)
+        self.next_step[0] = 'analysis_done'
+
+    def _checkbox_preconceptions(self):
+        clear_output(wait=False)
+        checkboxes = [self.bogui.create_checkbox(prec) for prec in self.preconceptions]
+        output = widgets.VBox(children=checkboxes)
+        display(output)
+
+    def _check_value_not_empty(self, value):
+        """Checks that text field was filled.
+            Args: string
+            Returns:
+                True: if string not empty
+                False: if string is empty
+        """
+        if value == '':
             return False
+
         return True
 
     def _create_cell_operations(self):
-        """Displays buttons for operations in inductive analysis"""
-        self.buttons['Ready to summarize'].disabled = True
+        """Displays buttons for operations in inductive analysis."""
+
+        self.buttons['ready'].disabled = True
         cell_number_label = self.bogui.create_label('Add code cells for your analysis:')
 
         cell_buttons = widgets.TwoByTwoLayout(
-            top_left=self.buttons['Open cells'],
-            bottom_left=self.buttons['Run cells'],
-            top_right=self.buttons['Delete last cell'],
-            bottom_right=self.buttons['Clear cells']
+            top_left=self.buttons['open'],
+            bottom_left=self.buttons['run'],
+            top_right=self.buttons['delete'],
+            bottom_right=self.buttons['clear']
         )
 
         grid = widgets.GridspecLayout(2, 3, height='auto', width='100%')
         grid[0, 0] = widgets.HBox([cell_number_label, self._add_cells_int])
         grid[:, 1] = cell_buttons
-        grid[1, 2] = self.buttons['Ready to summarize']
+        grid[1, 2] = self.buttons['ready']
 
         return grid
 
-    def start_inductive_analysis(self):
-        """Starts inductive analysis"""
-        self.utils.create_markdown_cells_above(1, '# Inductive analysis')
-        display(self._create_cell_operations())
-
-    def _all_done(self, _=None):
-        """Button function to display the export/close phase."""
-        #self.boutils.delete_cell_from_current(1)
-        self.new_analysis_view.close()
-        display(self.export_view)
-
-    def _export_to_pdf(self, _=None):
-        """Button function to export the notebook to pdf."""
-        #os.system('jupyter nbconvert Untitled.ipynb --to pdf')
-        self.export_view.close()
-        display(Javascript('print()'))
-        self.utils.delete_cell_from_current(0)
-
-    def _no_export(self, _=None):
-        """Button function to close widgets without exporting."""
-        self.utils.delete_cell_from_current(0)
-
-    def new_analysis(self):
-        """Display buttons to start a new analysis or prepare new data for analysis"""
-        display(self.new_analysis_view)
-
     def __repr__(self):
         return ''
```

### Comparing `bring_order-0.3.2/PKG-INFO` & `bring_order-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: bring-order
-Version: 0.3.2
+Version: 0.4.2
 Summary: 
 Author: BringOrder team
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: display (>=1.0.0,<2.0.0)
+Requires-Dist: en-core-web-sm-mirror (>=2.2.5,<3.0.0)
 Requires-Dist: invoke (>=2.1.2,<3.0.0)
+Requires-Dist: ipyfilechooser (>=0.6.0,<0.7.0)
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
+Requires-Dist: jupyter-ui-poll (>=0.2.2,<0.3.0)
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: notebook (>=6.5.4,<7.0.0)
 Requires-Dist: npx (>=0.1.1,<0.2.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: playwright (>=1.35.0,<2.0.0)
 Requires-Dist: py2nb (>=1.0.0,<2.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
+Requires-Dist: scipy (>=1.7.1,<2.0.0)
+Requires-Dist: spacy (>=3.6.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # bring-order
 ![GitHub Actions](https://github.com/Order-Team/bring-order/workflows/CI/badge.svg)
 [![codecov](https://codecov.io/gh/Order-team/bring-order/branch/main/graph/badge.svg?token=e8bdd46f-46b0-410c-820b-84ffca9ca53c)](https://codecov.io/gh/Order-team/bring-order)
 [![GitHub](https://img.shields.io/github/license/Order-Team/bring-order)](LICENSE.md)
```

