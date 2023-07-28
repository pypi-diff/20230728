# Comparing `tmp/rfidtools-0.1.3.tar.gz` & `tmp/rfidtools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfidtools-0.1.3.tar", max compression
+gzip compressed data, was "rfidtools-1.0.0.tar", max compression
```

## Comparing `rfidtools-0.1.3.tar` & `rfidtools-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-0.1.3/README.md
--rw-r--r--   0        0        0      320 2023-07-26 20:36:27.544302 rfidtools-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-24 04:50:43.162336 rfidtools-0.1.3/rfidtools/__init__.py
--rw-r--r--   0        0        0       32 2023-07-24 04:52:17.037566 rfidtools-0.1.3/rfidtools/__main__.py
--rw-r--r--   0        0        0     2974 2023-07-26 14:32:55.094303 rfidtools-0.1.3/rfidtools/core.py
--rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-0.1.3/rfidtools/labels/__init__.py
--rw-r--r--   0        0        0      163 2023-07-26 19:15:14.875504 rfidtools-0.1.3/rfidtools/labels/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7936 2023-07-26 20:33:25.931028 rfidtools-0.1.3/rfidtools/labels/__pycache__/add.cpython-311.pyc
--rw-r--r--   0        0        0    10351 2023-07-26 20:36:12.647367 rfidtools-0.1.3/rfidtools/labels/__pycache__/print.cpython-311.pyc
--rw-r--r--   0        0        0     7750 2023-07-26 20:32:58.520534 rfidtools-0.1.3/rfidtools/labels/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     3538 2023-07-26 20:33:23.944326 rfidtools-0.1.3/rfidtools/labels/add.py
--rw-r--r--   0        0        0     4854 2023-07-26 20:36:09.493976 rfidtools-0.1.3/rfidtools/labels/print.py
--rw-r--r--   0        0        0     4214 2023-07-26 20:32:17.296459 rfidtools-0.1.3/rfidtools/labels/utils.py
--rw-r--r--   0        0        0       30 2023-07-26 20:17:32.484082 rfidtools-0.1.3/rfidtools/rfidtool.py
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 rfidtools-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-30 14:23:06.683090 rfidtools-1.0.0/README.md
+-rw-r--r--   0        0        0      395 2023-07-28 04:31:46.697230 rfidtools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-07-28 05:15:27.059364 rfidtools-1.0.0/rfidtools/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-28 01:49:38.456817 rfidtools-1.0.0/rfidtools/__main__.py
+-rw-r--r--   0        0        0      678 2023-07-28 05:19:44.057505 rfidtools-1.0.0/rfidtools/config_template.yaml
+-rw-r--r--   0        0        0     2940 2023-07-28 06:34:27.526785 rfidtools-1.0.0/rfidtools/core.py
+-rw-r--r--   0        0        0        1 2023-07-25 17:56:32.452671 rfidtools-1.0.0/rfidtools/labels/__init__.py
+-rw-r--r--   0        0        0     5456 2023-07-28 06:17:38.834926 rfidtools-1.0.0/rfidtools/labels/add.py
+-rw-r--r--   0        0        0     4661 2023-07-28 03:39:58.341496 rfidtools-1.0.0/rfidtools/labels/print.py
+-rw-r--r--   0        0        0     5218 2023-07-28 05:49:48.863916 rfidtools-1.0.0/rfidtools/labels/utils.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 rfidtools-1.0.0/PKG-INFO
```

### Comparing `rfidtools-0.1.3/rfidtools/core.py` & `rfidtools-1.0.0/rfidtools/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-from rfidtools.labels import add
-from rfidtools.labels import print
 import tkinter as tk
 from tkinter import ttk
 
+from rfidtools.labels import add
+from rfidtools.labels import print
+
 
 class Mainframe(ttk.Frame):
     def __init__(self, parent):
         super().__init__(parent, padding=(5))
 
         self.grid(row=0, column=0, sticky='nsew')
         self.rowconfigure(0, weight=1, minsize=0)
         self.columnconfigure(0, weight=1, minsize=0)
 
     def main_menu(self):
         self.clear()
 
-        frame = ttk.LabelFrame(self, text='Menu')
-        frame.grid(row=0, column=0)
-        ttk.Button(frame, text='Add Porcelain Labels', command=self.add_porcelain).grid(row=0, column=0)
-        ttk.Button(frame, text='Add Slab Labels', command=self.add_slabs).grid(row=1, column=0)
-        ttk.Button(frame, text='Print Porcelain Labels', command=self.print_porcelain).grid(row=2, column=0)
-        ttk.Button(frame, text='Print Slab Labels', command=self.print_slabs).grid(row=3, column=0)
+        add_frame = ttk.LabelFrame(self, text='Add')
+        add_frame.grid(row=0, column=0, pady=80)
+        ttk.Button(add_frame, text='Add Porcelain Labels', command=self.add_porcelain).grid(row=0, column=0)
+        ttk.Button(add_frame, text='Add Slab Labels', command=self.add_slabs).grid(row=1, column=0)
+
+        print_frame = ttk.LabelFrame(self, text='Print')
+        print_frame.grid(row=1, column=0, pady=80)
+        ttk.Button(print_frame, text='Print Porcelain Labels', command=self.print_porcelain).grid(row=2, column=0)
+        ttk.Button(print_frame, text='Print Slab Labels', command=self.print_slabs).grid(row=3, column=0)
 
     def print_porcelain(self):
         self.clear()
 
         print.Porcelain(self).draw()
 
     def print_slabs(self):
@@ -69,18 +73,15 @@
         self.mainframe.main_menu()
 
         self._menu_bar()
 
     def _menu_bar(self):
         self.menubar = tk.Menu(self)
 
-        filemenu = tk.Menu(self.menubar, tearoff=False)
-        filemenu.add_command(label='Main Menu', command=self.mainframe.main_menu)
-        filemenu.add_command(label='TODO', state='disabled')
-        self.menubar.add_cascade(menu=filemenu, label='File')
+        self.menubar.add_command(label='Menu', command=self.mainframe.main_menu)
 
         addmenu = tk.Menu(self.menubar, tearoff=False)
         addmenu.add_command(label='Porcelain', command=self.mainframe.add_porcelain)
         addmenu.add_command(label='Slabs', command=self.mainframe.add_slabs)
         self.menubar.add_cascade(menu=addmenu, label='Add')
 
         printmenu = tk.Menu(self.menubar, tearoff=False)
```

### Comparing `rfidtools-0.1.3/rfidtools/labels/add.py` & `rfidtools-1.0.0/rfidtools/labels/add.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,113 @@
 import tkinter as tk
 from tkinter import ttk
 from tkinter import messagebox
 
-
-from . import utils
+from rfidtools.labels import utils
 
 
 class Add(ttk.LabelFrame):
     def __init__(self, parent, text):
         super().__init__(parent, text=text)
 
         self.type = type(self).__name__.lower()
         self.logs = utils.listlogs(self.type)
 
     def _update_logs(self):
         self.logs = utils.listlogs(self.type)
         self.logChoices.set(self.logs)
 
+    def _get_selected_log(self) -> str or None:
+        try:
+            log = self.logs[self.logsListBox.curselection()[0]]
+
+        except IndexError:
+            messagebox.showerror('Error', 'No log is selected.')
+            return None
+
+        return log
+
     def draw(self):
         self.grid(row=0, column=0, sticky='nsew')
         self.rowconfigure(0, weight=1)
-        self.rowconfigure(1, weight=0)
-        self.rowconfigure(2, weight=1)
-        self.rowconfigure(3, weight=0)
+        self.rowconfigure(1, weight=1)
+        self.rowconfigure(2, weight=0)
+        self.rowconfigure(3, weight=1)
+        self.rowconfigure(4, weight=0)
         self.columnconfigure(0, weight=1)
         self.columnconfigure(1, weight=1)
 
         self.logChoices = tk.StringVar(value=self.logs)
         self.logsListBox = tk.Listbox(self, listvariable=self.logChoices, selectmode='single')
-        self.logsListBox.grid(row=0, column=0, rowspan=3, sticky='nsew')
+        self.logsListBox.grid(row=0, column=0, rowspan=4, sticky='nsew')
+
+        ttk.Button(self, text='View Log', command=self.view_log).grid(row=0, column=1)
 
-        ttk.Label(self, text='Bin:').grid(row=0, column=1, sticky='s')
+        ttk.Label(self, text='Bin:').grid(row=1, column=1, sticky='s')
         self.bin = tk.StringVar()
         self.binEntry = ttk.Entry(self, textvariable=self.bin, state=tk.DISABLED)
-        self.binEntry.grid(row=1, column=1)
+        self.binEntry.grid(row=2, column=1)
         self.useBin = tk.BooleanVar(value=False)
         ttk.Checkbutton(self,
                         text='Use bin?',
                         command=lambda: self.binEntry.config(state=tk.NORMAL) if self.useBin.get() else self.binEntry.config(state=tk.DISABLED),
                         variable=self.useBin,
                         onvalue=True,
                         offvalue=False
-                        ).grid(row=2, column=1, sticky='n')
+                        ).grid(row=3, column=1, sticky='n')
+
+        ttk.Button(self,
+                   text='Remove Log',
+                   command=lambda: self.remove_log()
+                   ).grid(row=4, column=0, pady=5)
 
         ttk.Button(self,
                    text='Add Labels',
-                   command=lambda: self.add_labels(self.logs[self.logsListBox.curselection()[0]])
-                   ).grid(row=3, column=1)
+                   command=lambda: self.add_labels
+                   ).grid(row=4, column=1, pady=5)
+
+    def view_log(self) -> None:
+        log = self._get_selected_log()
+        if log is None:
+            return
+
+        view = tk.Toplevel()
+        view.title('Viewing: ' + log)
+        if view.tk.call('tk', 'windowingsystem') == 'x11':
+            view.attributes('-type', 'utility')
+
+        data = utils.read_log(log)
+
+        ttk.Button(view, text='Close', command=view.destroy).grid(row=len(data), column=len(data[0]) // 2 - 1, columnspan=2, stick='ew')
+
+        for i, colname in enumerate(data[0]):
+            ttk.Label(view, text=colname).grid(row=0, column=i, padx=50)
+        data = data[1:]
+
+        for i, row in enumerate(data):
+            for j, col in enumerate(row):
+                ttk.Label(view, text=col).grid(row=i + 1, column=j)
+
+    def remove_log(self) -> None:
+        log = self._get_selected_log()
+        if log is None:
+            return
+
+        if messagebox.askyesno(message=f'You are about to delete\n{log}\nAre you sure?'):
+            if utils.rmlog(log):
+                messagebox.showwarning('Deletion', 'The selected log was deleted.')
+                self._update_logs()
+            else:
+                messagebox.showerror('Error', 'Something went wrong, log could not be removed.')
+
+    def add_labels(self, query) -> None:
+        log = self._get_selected_log()
+        if log is None:
+            return
 
-    def add_labels(self, log, query) -> None:
         bin = self.bin.get() if self.useBin.get() else None
 
         data = utils.parse_log(self.type, log, bin)
         if len(data) == 0:
             messagebox.showerror('Error', 'File was empty or no data was read.')
             return
 
@@ -60,42 +115,42 @@
             if utils.archive(log):
                 messagebox.showinfo(log, 'Successfully commited logged labels to database and moved log to archives.')
 
             else:
                 messagebox.showerror('Error', 'Archival error.')
 
         else:
-            messagebox.showwarning('Error', 'Database error.')
+            messagebox.showerror('Error', 'Database error.\nIt\'s possible one of the labels is already in the database.\nOr there is a connection issue.')
 
         self._update_logs()
 
 
 class Porcelain(Add):
     def __init__(self, parent) -> None:
         super().__init__(parent, 'Porcelain: Add Labels')
 
     def draw(self) -> None:
         super().draw()
 
-    def add_labels(self, log) -> None:
+    def add_labels(self) -> None:
         INSERT_QUERY = """\
                 INSERT INTO porcelain_stock(ProductTagID, WarehouseCode, Status, ReceivedDateTimeStamp, CreatedBy, Bin, ProductTagName, ProductCode)
                 VALUES(?, ?, ?, ?, ?, ?, ?, ?)\
                 """
 
-        super().add_labels(log, INSERT_QUERY)
+        super().add_labels(INSERT_QUERY)
 
 
 class Slabs(Add):
     def __init__(self, parent) -> None:
         super().__init__(parent, 'Slabs: Add Labels')
 
     def draw(self) -> None:
         super().draw()
 
-    def add_labels(self, log) -> None:
+    def add_labels(self) -> None:
         INSERT_QUERY = """\
                 INSERT INTO Stock(Barcode, TagID, ProductCode, BlockNumber, SlabNumber, Length, Width, WarehouseCode, LocationCode, StatusID, ReceivedDateTimeStamp)
                 VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)\
                 """
 
-        super().add_labels(log, INSERT_QUERY)
+        super().add_labels(INSERT_QUERY)
```

### Comparing `rfidtools-0.1.3/rfidtools/labels/print.py` & `rfidtools-1.0.0/rfidtools/labels/print.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tkinter as tk
 from tkinter import ttk
 from tkinter import messagebox
 
-from . import utils
+from rfidtools.labels import utils
 
 
 class Print(ttk.LabelFrame):
     def __init__(self, parent, text):
         self.parent = parent
         super().__init__(self.parent, text=text, padding=(3, 3, 12, 12))
 
@@ -23,31 +23,28 @@
         self.rowconfigure(2, weight=1)
         self.rowconfigure(3, weight=1)
         self.rowconfigure(4, weight=1)
         self.rowconfigure(5, weight=1)
         self.columnconfigure(0, weight=1)
         self.columnconfigure(1, weight=1)
 
-        self.add_labels = tk.BooleanVar(value=True)
-        ttk.Checkbutton(self.parent, text='Add labels?', variable=self.add_labels, onvalue=True, offvalue=False).grid(row=1, column=0)
+        ttk.Label(self.parent, text='Serial: ').grid(row=1, column=0, sticky='e')
+        ttk.Entry(self.parent, textvariable=self.serial, width=3).grid(row=1, column=1, sticky='w')
 
-        ttk.Label(self.parent, text='Serial: ').grid(row=1, column=1, sticky='e', padx=(20, 0))
-        ttk.Entry(self.parent, textvariable=self.serial, width=3).grid(row=1, column=2, sticky='w')
+        ttk.Label(self.parent, text='Serial Numbers: ').grid(row=1, column=2, sticky='e', padx=(20, 0))
+        ttk.Entry(self.parent, textvariable=self.serial_numbers, width=3).grid(row=1, column=3, sticky='w')
 
-        ttk.Label(self.parent, text='Serial Numbers: ').grid(row=1, column=3, sticky='e', padx=(20, 0))
-        ttk.Entry(self.parent, textvariable=self.serial_numbers, width=3).grid(row=1, column=4, sticky='w')
-
-        ttk.Button(self.parent, text='Print', command=self.print_labels).grid(row=1, column=5, padx=10, pady=5)
+        ttk.Button(self.parent, text='Print', command=self.print_labels).grid(row=1, column=4, padx=20, pady=5)
 
     def print_labels(self, payload):
         if utils.send_print(self.type, payload):
             messagebox.showinfo('Success', 'Print job was sent successfully.')
 
         else:
-            messagebox.showwarning('Error', 'Error sending sending print job.')
+            messagebox.showerror('Error', 'Error sending sending print job.')
 
 
 class Porcelain(Print):
     def __init__(self, parent) -> None:
         super().__init__(parent, 'Porcelain: Print Labels')
 
         self.code = tk.StringVar()
@@ -76,15 +73,15 @@
 
         ttk.Label(self, text='Thickness:').grid(row=4, column=0, columnspan=2, sticky='s')
         ttk.Entry(self, textvariable=self.thickness, width=2).grid(row=5, column=0, columnspan=2, sticky='n')
 
 
 class Slabs(Print):
     def __init__(self, parent) -> None:
-        super().__init__(parent, 'Porcelain: Print Labels')
+        super().__init__(parent, 'Slabs: Print Labels')
 
         self.code = tk.StringVar()
         self.desc = tk.StringVar()
         self.dim_x = tk.IntVar()
         self.dim_y = tk.IntVar()
         self.lot = tk.StringVar()
```

### Comparing `rfidtools-0.1.3/rfidtools/labels/utils.py` & `rfidtools-1.0.0/rfidtools/labels/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 import re
 import csv
-import webbrowser
 from datetime import datetime
 
 import pyodbc as db
 from fabric import Connection
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
 
-PRINT_LOGS_PATH = 'C:\\Print_Logs\\'
-PRINT_ARCHIVES_PATH = 'C:\\Print_Archives\\'
+from rfidtools import DB_SERVER, DB_TABLE, DB_USER, DB_PASS
+from rfidtools import SSH_SERVER, SSH_USER, SSH_PASS, SSH_LOGS_PATH, SSH_ARCHIVES_PATH
+
+PRINT_LOGS_PATH = SSH_LOGS_PATH
+PRINT_ARCHIVES_PATH = SSH_ARCHIVES_PATH
 
 # SQL connection
-sql_connection = 'Driver={ODBC Driver 18 for SQL Server};Server=192.168.2.67;Database=DataWhseCiot;UID=SA;PWD=Passw0rd;Encrypt=no'
+sql_connection = f'Driver={{ODBC Driver 18 for SQL Server}};Server={DB_SERVER};Database={DB_TABLE};UID={DB_USER};PWD={DB_PASS}'
 
 # SSH connection
-ssh_kwargs = {'host': '192.168.2.67', 'user': 'RFIDAdmin', 'connect_timeout': 10, 'connect_kwargs': {'password': 'Passw0rd2987'}}
+ssh_kwargs = {'host': SSH_SERVER, 'user': SSH_USER, 'connect_timeout': 10, 'connect_kwargs': {'password': SSH_PASS}}
 
 
 def listlogs(type) -> list:
     if type not in {'porcelain', 'slabs'}:
         print('Something went very wrong.\nInvalid type argument, object has impossible name.')
         raise TypeError
 
     with Connection(**ssh_kwargs) as c, c.sftp() as sftp:
         sftp.chdir(PRINT_LOGS_PATH)
         logs = sftp.listdir()
 
     return [log for log in logs if re.search(f'^{type}_[0-9]*.txt', log) or re.search(f'^{type}_nf_[0-9]*.txt', log)]
 
 
+def rmlog(log) -> bool:
+    try:
+        with Connection(**ssh_kwargs) as c, c.sftp() as sftp:
+            sftp.remove(PRINT_LOGS_PATH + log)
+        return True
+
+    except Exception as e:
+        print('File may not be found, or connection is bad.\n' + str(e))
+        return False
+
+
 def parse_log(type, log, bin) -> list[tuple]:
     data = list()
 
     if type == 'porcelain':
         def label(row) -> tuple:
             return (
                 row['rfid'],  # ProductTagID
@@ -69,42 +84,59 @@
             rows = csv.DictReader(csvfile, dialect='unix')
             for row in rows:
                 data.append(label(row))
 
     return data
 
 
+def read_log(log) -> list:
+    with Connection(**ssh_kwargs) as c, c.sftp() as sftp:
+        with sftp.open(PRINT_LOGS_PATH + log, mode='r') as csvfile:
+            csvfile.prefetch()
+            reader = csv.reader(csvfile)
+            data = list(reader)
+
+    return data
+
+
 def send_print(type, payload) -> bool:
     if type == 'porcelain':
         url = 'http://192.168.2.67:8080/bartender/print/rfid_templates/porcelain_nf.btw?'
         for key, value in payload.items():
             if isinstance(value, str) is str:
                 value = value.replace(' ', '%20')
 
             url += f'{key}={value}&'
         url = url[:-1]
 
-        webbrowser.open(url)
-
     elif type == 'slabs':
         url = 'http://192.168.2.67:8080/bartender/print/rfid_templates/slabs_nf.btw?'
         for key, value in payload.items():
             if isinstance(value, str) is str:
                 value = value.replace(' ', '%20')
 
             url += f'{key}={value}&'
         url = url[:-1]
 
-        webbrowser.open(url)
-
     else:
         print('Something went very wrong.\nInvalid type argument, object has impossible name.')
         raise TypeError
         return False
 
+    opts = Options()
+    opts.add_argument('--headless')
+    driver = webdriver.Chrome(options=opts)
+    try:
+        driver.get(url)
+
+    except Exception as e:
+        print('Something went wrong with the browser automation.\nMaybe chrome isn\'t installed?\n' + str(e))
+        return False
+    driver.close()
+
     return True
 
 
 def query(data, query) -> bool:
     connection = db.connect(sql_connection)
     cursor = connection.cursor()
     try:
```

