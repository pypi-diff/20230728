# Comparing `tmp/regfile_generics-0.0.3.tar.gz` & `tmp/regfile_generics-0.1.0.tar.gz`

## Comparing `regfile_generics-0.0.3.tar` & `regfile_generics-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/.editorconfig
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/makefile
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/tox.ini
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/.github/workflows/tox.yml
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/src/regfile_generics/__init__.py
--rw-r--r--   0        0        0    22739 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/src/regfile_generics/regfile.py
--rw-r--r--   0        0        0    12379 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/src/regfile_generics/regfile_device.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/tests/access_test.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/tests/fixtures.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/tests/lock_instance_test.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/tests/uvmlike_access_test.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/.gitignore
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/LICENSE
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/README.md
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 regfile_generics-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/makefile
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/tox.ini
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/.github/workflows/pypi-deploy.yml
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/.github/workflows/tox.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/src/regfile_generics/__init__.py
+-rw-r--r--   0        0        0    23290 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/src/regfile_generics/regfile.py
+-rw-r--r--   0        0        0    12711 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/src/regfile_generics/regfile_device.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/tests/access_test.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/tests/fixtures.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/tests/lock_instance_test.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/tests/uvmlike_access_test.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/README.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 regfile_generics-0.1.0/PKG-INFO
```

### Comparing `regfile_generics-0.0.3/.github/workflows/python-publish.yml` & `regfile_generics-0.1.0/.github/workflows/pypi-deploy.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This workflow will upload a Python Package using Twine when a release is created
 # For more information see: https://help.github.com/en/actions/language-and-framework-guides/using-python-with-github-actions#publishing-to-package-registries
 
-name: Upload Python Package
+name: PyPI Publish
 
 on:
-  release:
-    types: [created]
+  push:
+    tags:
+    - '**'
 
 jobs:
-  deploy:
-
+ pypi:
     runs-on: ubuntu-latest
-
+    # Specifying a GitHub environment is optional, but strongly encouraged
+    environment: release
+    permissions:
+      # IMPORTANT: this permission is mandatory for trusted publishing
+      id-token: write
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python
-      uses: actions/setup-python@v2
-      with:
-        python-version: '3.8'
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install setuptools wheel twine
-    - name: Build and publish
-      env:
-        TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-      run: |
-        python setup.py sdist bdist_wheel
-        twine upload dist/*
+      - uses: actions/checkout@v3
+      - name: Setup Python
+        uses: actions/setup-python@v3
+        with:
+          python-version: '3.11'
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip build
+      - name:
+        run: |
+          make build
+      - name: Publish
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `regfile_generics-0.0.3/.github/workflows/tox.yml` & `regfile_generics-0.1.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `regfile_generics-0.0.3/src/regfile_generics/regfile.py` & `regfile_generics-0.1.0/src/regfile_generics/regfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,30 @@
 Generic Regfile file access through names / items operator of the regfile class
 """
 
 import abc
 import traceback
 import warnings
 
+
 # pylint: disable=missing-class-docstring, missing-function-docstring
 
 
 class RegisterEntryAbstract(metaclass=abc.ABCMeta):
     """Abstract class handling dict-like access to Field of the register."""
 
     def __init__(self, **kwargs):
         """Constructor - Mandatory kwargs: regfile and address offset."""
         object.__setattr__(self, "_lock", False)
-        self.regfile = kwargs.pop('regfile')
-        self.addr = int(kwargs.pop('addr'))
+        self.regfile = kwargs.pop("regfile")
+        self.addr = int(kwargs.pop("addr"))
 
-        self.write_mask = int(kwargs.pop('write_mask', -1))
-        self._fields = kwargs.pop('fields', {})
-        self._writable_fieldnames = kwargs.pop('_writable_fieldnames', None)
+        self.write_mask = int(kwargs.pop("write_mask", -1))
+        self._fields = kwargs.pop("fields", {})
+        self._writable_fieldnames = kwargs.pop("_writable_fieldnames", None)
         self._userattributes = tuple(kwargs.keys())
 
         for attr, value in kwargs.items():
             self.__setattr__(attr, value)
         self._lock = True
 
     @abc.abstractmethod
@@ -73,50 +74,60 @@
         return self._fields.keys()
 
     def __getitem__(self, key):
         """Dict-like access to read a value from a field."""
         if key in self._fields:
             return self._fields[key].get_field(self._get_value())
 
-        raise KeyError(f"Field {key} does not exist. "
-                       f"Available fields: {list(self._fields.keys())}")  # pragma: nocover
+        raise KeyError(
+            f"Field {key} does not exist. "
+            f"Available fields: {list(self._fields.keys())}"
+        )  # pragma: nocover
 
     def __setattr__(self, name, value):
         if self._lock is True and name not in self.__dict__:
-            raise AttributeError(f"Unable to allocate attribute {name} - Instance is locked.")
+            raise AttributeError(
+                f"Unable to allocate attribute {name} - Instance is locked."
+            )
 
         super().__setattr__(name, value)
 
     def __setitem__(self, key, value):
         """Dict-like access to write a value to a field."""
         if key not in self._fields:
-            raise KeyError(f"Field {key} does not exist. "
-                           f"Available fields: {list(self.get_field_names())}")  # pragma: nocover
+            raise KeyError(
+                f"Field {key} does not exist. "
+                f"Available fields: {list(self.get_field_names())}"
+            )  # pragma: nocover
 
         field = self._fields[key]
         truncval = self._fit_fieldvalue_for_write(field, value)
         self._set_value(truncval << field.lsb, field.get_mask())
 
     def _fit_fieldvalue(self, field, value):
         """Truncate a value to fit into the field is necessary and raise a warning."""
         mask = field.get_mask()
         fieldmask = mask >> field.lsb
         truncval = value & fieldmask
 
         if value != truncval:
-            _regfile_warn_user(f"{field.name}: value 0x{value:x} is truncated to 0x{truncval:x} "
-                               f"(mask: 0x{fieldmask}).")
+            _regfile_warn_user(
+                f"{field.name}: value 0x{value:x} is truncated to 0x{truncval:x} "
+                f"(mask: 0x{fieldmask})."
+            )
         return truncval
 
     def _fit_fieldvalue_for_write(self, field, value):
         """Additional to the truncation, check if field is writable."""
         mask = field.get_mask()
         if mask & self.write_mask != mask:
-            _regfile_warn_user(f"Writing read-only field {field.name} (value: 0x{value:08x} -- "
-                               f"mask: 0x{mask:08x} write_mask: 0x{self.write_mask:08x}).")
+            _regfile_warn_user(
+                f"Writing read-only field {field.name} (value: 0x{value:08x} -- "
+                f"mask: 0x{mask:08x} write_mask: 0x{self.write_mask:08x})."
+            )
 
         return self._fit_fieldvalue(field, value)
 
     def get_dict(self, int_value=None):
         """Get dictionary field view of the register.
         If int_value is not specified a read will be executed,
         otherwise the int_value is decomposed to the fields"""
@@ -133,16 +144,17 @@
 
         if isinstance(field_dict, dict):
             value = 0
             for fieldname, fieldvalue in field_dict.items():
                 field = self._fields[fieldname]
                 value |= self._fit_fieldvalue(field, fieldvalue) << field.lsb
             return value
-        raise TypeError(f"Unable to get_value for type {type(value)} "
-                        f"-- {str(value)}.")  # pragma: nocover
+        raise TypeError(
+            f"Unable to get_value for type {type(value)} " f"-- {str(value)}."
+        )  # pragma: nocover
 
     def get_writable_fieldnames(self):
         """Return a copied list containing all writable fieldnames"""
         return list(self._writable_fieldnames)
 
     def writable_field_items(self):
         """Tuple of object over all writable fieldnames"""
@@ -152,62 +164,65 @@
             if field_mask & self.write_mask == field_mask:
                 writable_fields.append((name, field))
         return writable_fields
 
     def get_name(self):
         """Get the name of the register, if set otherwise return UNNAMED"""
         name = "UNNAMED"
-        if hasattr(self, 'name'):
+        if hasattr(self, "name"):
             name = self.name
 
         return name
 
     def __str__(self):
         """Read the register and format it decomposed as fields as well as integer value."""
         int_value = self._get_value()
         strfields = []
         for name, field in self.items():
             strfields.append(f"'{name}': 0x{field.get_field(int_value):x}")
-        return f"Register {self.get_name()}: {{{', '.join(strfields)}}} = 0x{int_value:x}"
+        return (
+            f"Register {self.get_name()}: {{{', '.join(strfields)}}} = 0x{int_value:x}"
+        )
 
-    def set_value(self, value=None, mask=None, **kwargs):
+    def set_value(self, value, mask=None):
         """Set the value of register. The value can be an integer a dict or
         a register object (e.g. obtained by 'read_entry()'."""
         if mask is None:
             mask = self.write_mask
 
-        if kwargs:
-            if value:
-                raise ValueError("Value has to be None, is kwargs are set.")
-            value = kwargs
-
         if isinstance(value, int):
             self._set_value(value, mask)
         elif isinstance(value, dict):
             writable_fieldnames = self.get_writable_fieldnames()
             write_value = 0
             for fieldname, fieldvalue in value.items():
                 if fieldname in writable_fieldnames:
                     writable_fieldnames.remove(fieldname)
                     field = self._fields[fieldname]
-                    write_value |= self._fit_fieldvalue_for_write(field, fieldvalue) << field.lsb
+                    write_value |= (
+                        self._fit_fieldvalue_for_write(field, fieldvalue) << field.lsb
+                    )
                 elif fieldname not in self.get_field_names():
                     _regfile_warn_user(
-                        f"Ignoring non existent Field {fieldname} for write.")
+                        f"Ignoring non existent Field {fieldname} for write."
+                    )
 
             if writable_fieldnames:
-                _regfile_warn_user(f"Field(s) {', '.join(writable_fieldnames)} were not explicitly "
-                                   f"set during write of register {self.get_name()}!")
+                _regfile_warn_user(
+                    f"Field(s) {', '.join(writable_fieldnames)} were not explicitly "
+                    f"set during write of register {self.get_name()}!"
+                )
 
             self._set_value(write_value, self.write_mask)
         elif isinstance(value, RegisterEntry):
             self._set_value(value.get_value(), self.write_mask)
         else:
-            raise TypeError(f"Unable to assign type {type(value)} "
-                            f"-- {str(value)}.")  # pragma: nocover
+            raise TypeError(
+                f"Unable to assign type {type(value)} " f"-- {str(value)}."
+            )  # pragma: nocover
 
     def __int__(self):
         """Integer conversion - executes a read"""
         return self.get_value()
 
     def __eq__(self, other):
         """Equal comparison with integer -executes a read"""
@@ -244,18 +259,18 @@
     """Register Entry class - adding .represent() initialization for fields
     and UVM-like access"""
 
     def __init__(self, **kwargs):
         """Constructor see also RegisterEntryAbstract"""
         super().__init__(**kwargs)
         self._lock = False
-        self._add_fields_mode = kwargs.pop('_add_fields_mode', False)
-        self.desired_value = kwargs.pop('desired_value', 0)
-        self.mirrored_value = kwargs.pop('mirrored_value', 0)
-        self._reset = kwargs.pop('_reset', 0)
+        self._add_fields_mode = kwargs.pop("_add_fields_mode", False)
+        self.desired_value = kwargs.pop("desired_value", 0)
+        self.mirrored_value = kwargs.pop("mirrored_value", 0)
+        self._reset = kwargs.pop("_reset", 0)
         self._lock = True
 
     def _get_value(self):
         """Get value returns the mirrored value."""
         return self.mirrored_value
 
     def _set_value(self, value, mask):
@@ -273,72 +288,84 @@
         return self
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         """Lock the register fields - sort-out the writable_fieldnames
         with the help of the write_mask"""
         # TODO: sanity check write mask
         self._add_fields_mode = False
-        self._writable_fieldnames = tuple(name for name, _ in self.writable_field_items())
+        self._writable_fieldnames = tuple(
+            name for name, _ in self.writable_field_items()
+        )
 
     def __getitem__(self, key):
         """Add the represent() logic to the dict-like access method"""
         if self._add_fields_mode:
+
             def represent(**kwargs):
-                bits = kwargs['bits'].split(':')
+                bits = kwargs["bits"].split(":")
                 msb = int(bits[0])
                 lsb = int(bits[1]) if len(bits) == 2 else msb
                 field = RegisterField(name=key, msb=msb, lsb=lsb, **kwargs)
                 self._fields[key] = field
                 if "reset" in kwargs:
-                    reset = int(kwargs['reset'], 0) << lsb
+                    reset = int(kwargs["reset"], 0) << lsb
 
                     truncreset = reset & field.get_mask()
                     if truncreset != reset:
-                        _regfile_warn_user(f"{key}: reset value 0x{reset >> lsb:x} "
-                                           f"is truncated to 0x{truncreset >> lsb:x}.")  \
-                            # pragma: nocover
+                        _regfile_warn_user(
+                            f"{key}: reset value 0x{reset >> lsb:x} "
+                            f"is truncated to 0x{truncreset >> lsb:x}."
+                        )  # pragma: nocover
 
                     self._reset |= truncreset
                     self.desired_value = self._reset
                     self.mirrored_value = self._reset
 
                 return field
 
             return SyntasticSugarRepresent(represent)
 
         return super().__getitem__(key)
 
     def get_reset_values(self):
         """Get iterator object of the tuple (fieldname, resetvalue) for writable fields only."""
-        return {fieldname: field.get_field(self._reset) for fieldname, field in self.writable_field_items()}
+        return {
+            fieldname: field.get_field(self._reset)
+            for fieldname, field in self.writable_field_items()
+        }
 
     def field(self, name):
-        """ Get the field by name and add callback for UVM-like set() method of fields"""
+        """Get the field by name and add callback for UVM-like set() method of fields"""
         field = self._fields[name]
         if not hasattr(field, "set"):
+
             def setfunc(value):
                 self.desired_value &= ~field.get_mask()
-                self.desired_value |= self._fit_fieldvalue_for_write(field, value) << field.lsb
+                self.desired_value |= (
+                    self._fit_fieldvalue_for_write(field, value) << field.lsb
+                )
 
             setattr(field, "set", setfunc)
 
         return field
 
     def __getattr__(self, name):
         """Allow member access of fields - must have '_f' as suffix (<FIELDNAME>_f)."""
-        if name[-2:] == '_f' and name[:-2] in self._fields:
+        if name[-2:] == "_f" and name[:-2] in self._fields:
             return self.field(name[:-2])
 
-        raise AttributeError(f"Attribute {name} does not exist nor is a valid fieldname. "
-                             f"Available fields: {list(self._fields.keys())}")
+        raise AttributeError(
+            f"Attribute {name} does not exist nor is a valid fieldname. "
+            f"Available fields: {list(self._fields.keys())}"
+        )
 
     def get_register_entry(self, value):
         """Return a new RegisterEntry (shallow copy)."""
         userattr = {}
-        for attr in ('regfile', 'addr', 'write_mask', '_fields', '_reset'):
+        for attr in ("regfile", "addr", "write_mask", "_fields", "_reset"):
             userattr[attr] = getattr(self, attr)
 
         for attr in self._userattributes:
             userattr[attr] = getattr(self, attr)
 
         return RegisterEntry(mirrored_value=value, desired_value=value, **userattr)
 
@@ -347,15 +374,15 @@
         return self.get_register_entry(self._get_value())
 
     def set(self, value):
         """UVM-like - Set the desired value for this register."""
         self.desired_value = value
 
     def get(self):
-        """UVM-like - Return thee desired value of the fields in the register."""
+        """UVM-like - Return the desired value of the fields in the register."""
         return self.desired_value
 
     def get_mirrored_value(self):
         """UVM-like - Return the mirrored value of the fields in the register."""
         return self.mirrored_value
 
     def get_mirrored_dict(self):
@@ -375,17 +402,23 @@
         self.desired_value = self._reset
         self.mirrored_value = self._reset
 
     def get_reset(self):
         """UVM-like - Get the specified reset value for this register."""
         return self._reset
 
-    def write(self, value=None, mask=None, **kwargs):
+    def write(self, *args, **kwargs):
         """UVM-like - Write the specified value in this register."""
-        self.set_value(value, mask, **kwargs)
+        if args and not kwargs:
+            if len(args) == 1:
+                self.set_value(args[0])
+        elif not args and kwargs:
+            self.set_value(kwargs)
+        else:
+            raise ValueError("write just takes one dict or kwargs as argument.")
 
     def read(self):
         """UVM-like - Read the current value from this register."""
         return self.get_value()
 
     def update(self):
         """UVM-like - Updates the content of the register in the design
@@ -400,47 +433,54 @@
         """UVM-like - Returns the offset of this register."""
         return self.addr
 
     def get_address(self):
         """UVM-like - Returns the base external physical address of this register"""
         return self.regfile.get_base_addr() + self.addr
 
-    def write_update(self, values=None, **kwargs):
+    def write_update(self, *args, **kwargs):
         """Wrapper function around set() fields defined by value[dict] and update()"""
-        if values:
-            for field_name, field_value in values.items():
-                self.field(field_name).set(field_value)
+        if args:
+            if len(args) == 1 and isinstance(args[0], dict):
+                for field_name, field_value in args[0].items():
+                    self.field(field_name).set(field_value)
+            else:
+                raise ValueError("write_update just takes one dict as argument.")
+
         for field_name, field_value in kwargs.items():
             self.field(field_name).set(field_value)
+
         self.update()
 
 
 class RegfileEntry(RegisterEntry):
     def _get_value(self):
         value = self.regfile.read(self)
         if self.needs_update():
-            _regfile_warn_user(f"Register {self.get_name()}: Desired value 0x{self.desired_value:x} "
-                               f"has never been written via update() "
-                               f" --> mirrored value is 0x{self.mirrored_value:x}.\n"
-                               f"Reseting desired/mirrored value by readvalue 0x{value:x}")
+            _regfile_warn_user(
+                f"Register {self.get_name()}: Desired value 0x{self.desired_value:x} "
+                f"has never been written via update() "
+                f" --> mirrored value is 0x{self.mirrored_value:x}.\n"
+                f"Reseting desired/mirrored value by readvalue 0x{value:x}"
+            )
 
         self.desired_value = value
         self.mirrored_value = value
         return value
 
     def _set_value(self, value, mask):
         super()._set_value(value, mask)
         self.regfile.write(self, value, mask)
 
 
 class RegisterField:
     def __init__(self, **kwargs):
-        self.name = kwargs.pop('name')
-        self.msb = kwargs.pop('msb')
-        self.lsb = kwargs.pop('lsb')
+        self.name = kwargs.pop("name")
+        self.msb = kwargs.pop("msb")
+        self.lsb = kwargs.pop("lsb")
 
         for key, value in kwargs.items():
             self.__setattr__(key, value)
 
         self.__mask = (1 << (self.msb + 1)) - (1 << self.lsb)
 
     def get_field(self, intvalue):
@@ -467,15 +507,15 @@
     def __init__(self, rfdev, base_addr=0x0, **kwargs):
         object.__setattr__(self, "_lock", False)
         self._dev = rfdev
         self.__value_mask = (1 << (8 * self._dev.n_word_bytes)) - 1
         self.__base_addr = base_addr
         self._entries = {}
         self.__add_entry_mode = False
-        self.name = kwargs.pop('name', f"{type(self).__name__}@0x{base_addr:x}")
+        self.name = kwargs.pop("name", f"{type(self).__name__}@0x{base_addr:x}")
         self._lock = True
 
     def __enter__(self):
         self.__add_entry_mode = True
         return self
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
@@ -483,17 +523,19 @@
 
     def read(self, entry):
         return self._dev.read(self.get_base_addr(), entry)
 
     def write(self, entry, value, mask):
         regvalue = value & self.__value_mask
         if value != regvalue:
-            _regfile_warn_user(f"Value 0x{value:x} is too large to fit into "
-                               f"the specified word size ({self._dev.n_word_bytes}), "
-                               f"truncated to 0x{regvalue:x} / 0x{self.__value_mask:x}.")
+            _regfile_warn_user(
+                f"Value 0x{value:x} is too large to fit into "
+                f"the specified word size ({self._dev.n_word_bytes}), "
+                f"truncated to 0x{regvalue:x} / 0x{self.__value_mask:x}."
+            )
         self._dev.write(self.get_base_addr(), entry, value, mask)
 
     def get_base_addr(self):
         return self.__base_addr
 
     def get_rfdev(self):
         return self._dev
@@ -512,30 +554,34 @@
 
     def values(self):
         return self._entries.values()
 
     def __getitem__(self, key):
         if key not in self._entries:
             if self.__add_entry_mode:
+
                 def represent(**kwargs):
-                    kwargs.setdefault('name', key)
+                    kwargs.setdefault("name", key)
                     self._entries[key] = RegfileEntry(regfile=self, **kwargs)
                     return self._entries[key]
+
                 return SyntasticSugarRepresent(represent)
             raise KeyError(f"Regfile has no entry named '{key}'.")
         return self._entries[key]
 
     def __setattr__(self, name, value):
         if self._lock is True and name not in self.__dict__:
-            raise AttributeError(f"Unable to allocate attribute {name} - Instance is locked.")
+            raise AttributeError(
+                f"Unable to allocate attribute {name} - Instance is locked."
+            )
 
         super().__setattr__(name, value)
 
     def __getattr__(self, name):
-        if name[-2:] == '_r' and name[:-2] in self._entries:
+        if name[-2:] == "_r" and name[:-2] in self._entries:
             return self._entries[name[:-2]]
         raise AttributeError(f"Attribute {name} does not exist")
 
     def __setitem__(self, key, value):
         if key not in self._entries:
             raise KeyError(f"Regfile has no entry named '{key}'.")
 
@@ -553,16 +599,16 @@
     def __init__(self, represent):
         self.represent = represent
 
 
 class RegfileMemAccess:
     def __init__(self, rfdev, base_addr, **kwargs):
         self._dev = rfdev
-        if kwargs['size']:
-            self.index_range = kwargs['size'] // self._dev.n_word_bytes
+        if kwargs["size"]:
+            self.index_range = kwargs["size"] // self._dev.n_word_bytes
             self.__check_idx_func = self.__check_idx
         else:
             self.__check_idx_func = lambda self, index: None
         self.__base_addr = base_addr
 
     def __check_idx(self, index):
         if index >= self.index_range:
@@ -571,15 +617,16 @@
     def __getitem__(self, index):
         self.__check_idx_func(index)
         return self._dev.rfdev_read(self.__base_addr + self._dev.n_word_bytes * index)
 
     def __setitem__(self, index, value):
         self.__check_idx_func(index)
         self._dev.rfdev_write(
-            self.__base_addr + self._dev.n_word_bytes * index, value, -1, -1)
+            self.__base_addr + self._dev.n_word_bytes * index, value, -1, -1
+        )
 
     def get_rfdev(self):
         return self._dev
 
     def set_rfdev(self, dev):
         self._dev = dev
```

### Comparing `regfile_generics-0.0.3/src/regfile_generics/regfile_device.py` & `regfile_generics-0.1.0/src/regfile_generics/regfile_device.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,48 +21,52 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 """
 Generic Device on which a regfile can operate
 """
 
-__version__ = "0.0.3"
-
 import logging
 import os
 import random
 import struct
 import sys
 import traceback
 
 # pylint: disable=missing-class-docstring, missing-function-docstring
 
 
-class RegfileDev():
+class RegfileDev:
     def __init__(self, **kwargs):
         super().__init__()
-        self.n_word_bytes = kwargs.pop('bytes_per_word', 4)
-        self.logger = kwargs.pop('logger', logging.getLogger(__name__))
-        self._prefix = kwargs.pop('prefix', '')
-        self._blockread = kwargs.pop('blockread', None)
-        self._blockwrite = kwargs.pop('blockwrite', None)
+        self.n_word_bytes = kwargs.pop("bytes_per_word", 4)
+        self.logger = kwargs.pop("logger", logging.getLogger(__name__))
+        self._prefix = kwargs.pop("prefix", "")
+        self._blockread = kwargs.pop("blockread", None)
+        self._blockwrite = kwargs.pop("blockwrite", None)
 
-        self.callback = kwargs.pop('callback', {})
+        self.callback = kwargs.pop("callback", {})
         if not isinstance(self.callback, dict):
-            raise TypeError("Argument 'callback' has to dict with name, callback function.")
+            raise TypeError(
+                "Argument 'callback' has to dict with name, callback function."
+            )
 
         if not set(self.callback) <= self.allowed_callbacks():
-            raise AttributeError(f"Only {self.allowed_callbacks} are allowed as callback functions.")
+            raise AttributeError(
+                f"Only {self.allowed_callbacks} are allowed as callback functions."
+            )
 
         for func in self.allowed_callbacks() - set(self.callback):
             if not hasattr(self, func):
-                raise TypeError(f"Function {func} has to be implemented or passed as callback function.")
+                raise TypeError(
+                    f"Function {func} has to be implemented or passed as callback function."
+                )
 
     def allowed_callbacks(self):
-        return {'rfdev_read', 'rfdev_write'}
+        return {"rfdev_read", "rfdev_write"}
 
     def readwrite_block(self, start_addr, values, write):
         if not write:
             if self._blockread:
                 for i, data in enumerate(self._blockread(start_addr, len(values))):
                     # Modifications are be done by reference
                     values[i] = data
@@ -73,59 +77,73 @@
         else:
             if self._blockwrite:
                 self._blockwrite(start_addr, values)
             else:
                 mask = (1 << (8 * self.n_word_bytes)) - 1
                 write_mask = mask
                 for i, value in enumerate(values):
-                    self.rfdev_write(start_addr + i * self.n_word_bytes, value, mask, write_mask)
+                    self.rfdev_write(
+                        start_addr + i * self.n_word_bytes, value, mask, write_mask
+                    )
 
     def rfdev_read(self, addr):
         """Read method could be overridden when deriving a new RegfileDev"""
-        return self.callback['rfdev_read'](addr)
+        return self.callback["rfdev_read"](addr)
 
     def read(self, baseaddr, entry):
         value = self.rfdev_read(baseaddr + entry.addr)
-        self.logger.debug("%sRegfileDevice reading entry %s from address "
-                          "0x%x = 0x%x", self._prefix, entry.name, entry.addr, value)
+        self.logger.debug(
+            "%sRegfileDevice reading entry %s from address 0x%x = 0x%x",
+            self._prefix,
+            entry.name,
+            entry.addr,
+            value,
+        )
         return value
 
     def rfdev_write(self, addr, value, mask, write_mask):
         """Read method could be overridden when deriving a new RegfileDev"""
-        self.callback['rfdev_write'](addr, value, mask, write_mask)
+        self.callback["rfdev_write"](addr, value, mask, write_mask)
 
     def write(self, baseaddr, entry, value, mask):
         addr = baseaddr + entry.addr
 
-        self.logger.debug("%sRegfileDevice initiate write of entry %s at address "
-                          "0x%x -- {value: 0x%x, mask 0x%x, write_mask: 0x%x}",
-                          self._prefix, entry.name, entry.addr, value, mask, entry.write_mask)
+        self.logger.debug(
+            "%sRegfileDevice initiate write of entry %s at address "
+            "0x%x -- {value: 0x%x, mask 0x%x, write_mask: 0x%x}",
+            self._prefix,
+            entry.name,
+            entry.addr,
+            value,
+            mask,
+            entry.write_mask,
+        )
         self.rfdev_write(addr, value, mask, entry.write_mask)
 
 
 class RegfileDevSimple(RegfileDev):
     def rfdev_write(self, addr, value, mask, write_mask):
         keep_mask = ~mask & write_mask
 
         if keep_mask == 0:
             self.rfdev_write_simple(addr, value)
         else:
             # read, modify, write
             rmw_value = self.rfdev_read(addr)
 
             rmw_value &= ~mask
-            rmw_value |= (value & mask)
+            rmw_value |= value & mask
 
             self.rfdev_write_simple(addr, rmw_value)
 
     def allowed_callbacks(self):
-        return {'rfdev_read', 'rfdev_write_simple'}
+        return {"rfdev_read", "rfdev_write_simple"}
 
     def rfdev_write_simple(self, addr, value):
-        self.callback['rfdev_write_simple'](addr, value)
+        self.callback["rfdev_write_simple"](addr, value)
 
 
 def regfile_dev_debug_getbits(interactive, default_value, promptprefix):
     if not interactive:
         print(f"{promptprefix} value: 0x{default_value:x}")
         return default_value
 
@@ -151,26 +169,29 @@
 
 class RegfileDevSimpleDebug(RegfileDevSimple):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mem = {}
         self.write_count = 0
         self.read_count = 0
-        kwargs.setdefault('interactive', False)
-        self.__interactive = kwargs['interactive']
+        kwargs.setdefault("interactive", False)
+        self.__interactive = kwargs["interactive"]
 
     def rfdev_read(self, addr):
         if addr not in self.mem:
             value = random.getrandbits(8 * self.n_word_bytes)
             print(f"Generating random regfile value {value}.")
         else:
             value = self.mem[addr]
 
-        value = regfile_dev_debug_getbits(self.__interactive, value,
-                                          f"{self._prefix}REGFILE-READING from addr 0x{addr:x}")
+        value = regfile_dev_debug_getbits(
+            self.__interactive,
+            value,
+            f"{self._prefix}REGFILE-READING from addr 0x{addr:x}",
+        )
         self.mem[addr] = value
 
         self.read_count += 1
         return value
 
     def rfdev_write_simple(self, addr, value):
         print(f"{self._prefix}REGFILE-WRITING to addr 0x{addr:x} value 0x{value:x}")
@@ -202,47 +223,53 @@
                 i_word_mask = subword_mask << (i * n_subword_bytes * 8)
 
                 # no keep bit would be overwritten? && all write bits are covered?
                 if ((keep_mask & i_word_mask) == 0) and ((mask & (~i_word_mask)) == 0):
                     subword_offset = i * n_subword_bytes
 
                     # call virtual method
-                    self.logger.debug("RegfileDevice: Subwrite address 0x%x -- "
-                                      "{value: 0x%x, n_subword_bytes: 0x%x}",
-                                      addr + subword_offset, value, n_subword_bytes)
-                    self.rfdev_write_subword(addr + subword_offset, value, n_subword_bytes)
+                    self.logger.debug(
+                        "RegfileDevice: Subwrite address 0x%x -- "
+                        "{value: 0x%x, n_subword_bytes: 0x%x}",
+                        addr + subword_offset,
+                        value,
+                        n_subword_bytes,
+                    )
+                    self.rfdev_write_subword(
+                        addr + subword_offset, value, n_subword_bytes
+                    )
                     # we are done here ...
                     return
 
             # reduce subword bytes - next half
             n_subword_bytes //= 2
             # reduce subword mask - throw away the other half
             subword_mask >>= n_subword_bytes * 8
 
         # no success?  - full read-modify-write
         rmw_value = self.rfdev_read(addr)
 
         rmw_value &= ~mask
-        rmw_value |= (value & mask)
+        rmw_value |= value & mask
 
         # call virtual method
         self.rfdev_write_subword(addr, rmw_value, self.n_word_bytes)
 
     def allowed_callbacks(self):
-        return {'rfdev_read', 'rfdev_write_subword'}
+        return {"rfdev_read", "rfdev_write_subword"}
 
     def rfdev_write_subword(self, addr, value, size):
-        self.callback['rfdev_write_subword'](addr, value, size)
+        self.callback["rfdev_write_subword"](addr, value, size)
 
 
 class RegfileDevSubwordDebug(RegfileDevSubword):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        kwargs.setdefault('interactive', False)
-        self.__interactive = kwargs['interactive']
+        kwargs.setdefault("interactive", False)
+        self.__interactive = kwargs["interactive"]
         self.mem = {}
         self.write_count = 0
         self.read_count = 0
 
     def getvalue(self, addr):
         word = []
         for i in range(self.n_word_bytes):
@@ -250,80 +277,87 @@
                 byte_value = random.getrandbits(8)
                 print(f"Generating random regfile value {byte_value}.")
                 self.mem[addr + i] = byte_value
 
             byte_value = self.mem[addr + i]
             word.append(byte_value)
 
-        return int.from_bytes(struct.pack(f"{self.n_word_bytes}B", *word), 'little')
+        return int.from_bytes(struct.pack(f"{self.n_word_bytes}B", *word), "little")
 
     def rfdev_read(self, addr):
         value = self.getvalue(addr)
 
-        value = regfile_dev_debug_getbits(self.__interactive, value,
-                                          f"{self._prefix}REGFILE-READING from addr 0x{addr:x}")
+        value = regfile_dev_debug_getbits(
+            self.__interactive,
+            value,
+            f"{self._prefix}REGFILE-READING from addr 0x{addr:x}",
+        )
         for i in range(self.n_word_bytes):
-            self.mem[addr + i] = (value >> (8 * i)) & 0xff
+            self.mem[addr + i] = (value >> (8 * i)) & 0xFF
 
         self.read_count += 1
         return value
 
     def rfdev_write_subword(self, addr, value, size):
-        print(f"{self._prefix}REGFILE-WRITING to addr 0x{addr:x} value 0x{value:x} size=0x{size:x}")
+        print(
+            f"{self._prefix}REGFILE-WRITING to addr 0x{addr:x} value 0x{value:x} size=0x{size:x}"
+        )
 
-        byte_values = value.to_bytes(self.n_word_bytes, 'little')
+        byte_values = value.to_bytes(self.n_word_bytes, "little")
         for i in range(size):
             self.mem[addr + i] = byte_values[i + addr & 0b11]
         self.write_count += 1
 
 
 class StringCmdRegfileDevSimple(RegfileDevSimple):
-    '''Forwards regfile operations to a function call with string command,
-       to do the regfile operations.
+    """Forwards regfile operations to a function call with string command,
+    to do the regfile operations.
 
-        Read:
-            r<NUMBITS> <address>
-                e.g. r32 0x1C
-
-        Write:
-            w<NUMBITS> <address> <value>
-                e.g. w32 0x80 0xF9852A
-     '''
+     Read:
+         r<NUMBITS> <address>
+             e.g. r32 0x1C
+
+     Write:
+         w<NUMBITS> <address> <value>
+             e.g. w32 0x80 0xF9852A
+    """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.execute = kwargs['execute']
+        self.execute = kwargs["execute"]
 
     def rfdev_read(self, addr):
         return int(self.execute(f"r{8*self.n_word_bytes} 0x{addr:x}"), 0)
 
     def rfdev_write_simple(self, addr, value):
         self.execute(f"w{8*self.n_word_bytes} 0x{addr:x} 0x{value:x}")
 
 
 class StringCmdRegfileDevSubword(RegfileDevSubword):
-    '''Forwards regfile operations to a function call with string command,
-       to do the regfile operations.
+    """Forwards regfile operations to a function call with string command,
+    to do the regfile operations.
 
-        Read:
-            r<NUMBITS> <address>
-                e.g. r32 0x1C
-
-        Write:
-            w<NUMBITS> <address> <value> [bsel]
-                e.g. w32 0x80 0xF9852A
-                     w32 0x80 0xF9852A 0x1
-     '''
+     Read:
+         r<NUMBITS> <address>
+             e.g. r32 0x1C
+
+     Write:
+         w<NUMBITS> <address> <value> [bsel]
+             e.g. w32 0x80 0xF9852A
+                  w32 0x80 0xF9852A 0x1
+    """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.execute = kwargs['execute']
+        self.execute = kwargs["execute"]
 
     def rfdev_read(self, addr):
         return int(self.execute(f"r{8*self.n_word_bytes} 0x{addr:x}"), 0)
 
     def rfdev_write_subword(self, addr, value, size):
         subword_addrbits = self.n_word_bytes.bit_length() - 1
         bsel = ((1 << size) - 1) << (addr & subword_addrbits)
         addr_aligned = addr & ~subword_addrbits
 
-        self.execute(f"w{8*self.n_word_bytes} 0x{addr_aligned:x} 0x{value:x} 0x{bsel:x}")
+        self.execute(
+            f"w{8*self.n_word_bytes} 0x{addr_aligned:x} 0x{value:x} 0x{bsel:x}"
+        )
```

### Comparing `regfile_generics-0.0.3/tests/access_test.py` & `regfile_generics-0.1.0/tests/access_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,170 @@
 """Regfile access tests"""
-# pylint: disable=unused-import,redefined-outer-name
-# flake8: noqa
 from pytest import warns
 
 # pylint: disable=line-too-long,missing-function-docstring
 
 
 def test_dict_access(sessionsubwordregfile):
     """dict like access"""
     regfile, rfdev = sessionsubwordregfile
 
     write_count = rfdev.write_count
-    regfile['reg1_high'] = {'cfg': 0x0ff,
-                            'cfg_trigger': 0x1,
-                            'cfg_trigger_mode': 0x0}
+    regfile["reg1_high"] = {"cfg": 0x0FF, "cfg_trigger": 0x1, "cfg_trigger_mode": 0x0}
 
     assert 0xF000_0008 in rfdev.mem.keys()
-    assert rfdev.getvalue(0xF000_0008) == 0x1ff
+    assert rfdev.getvalue(0xF000_0008) == 0x1FF
 
-    regfile['reg0'] = {'cfg': 0x11}
+    regfile["reg0"] = {"cfg": 0x11}
 
     read_count = rfdev.read_count
-    reg0 = dict(regfile['reg0'])
+    reg0 = dict(regfile["reg0"])
     print(f"Debug: dict-read: {reg0}")
 
-    assert reg0['cfg'] == 0x11
+    assert reg0["cfg"] == 0x11
     assert read_count + 1 == rfdev.read_count
     assert rfdev.getvalue(0xF000_0000) & 0b11111 == 0x11
 
     assert write_count + 2 == rfdev.write_count
 
 
 def test_str_cast(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
 
     write_count = rfdev.write_count
     read_count = rfdev.read_count
-    regfile['reg1_high'] = {'cfg': 0x0aa,
-                            'cfg_trigger': 0x0,
-                            'cfg_trigger_mode': 0x0}
+    regfile["reg1_high"] = {"cfg": 0x0AA, "cfg_trigger": 0x0, "cfg_trigger_mode": 0x0}
 
     print("Byte aligned - should no do read-modify-write...")
-    regfile['reg1_high']['cfg_trigger_mode'] = 0b11
+    regfile["reg1_high"]["cfg_trigger_mode"] = 0b11
 
     print("Reading register to string...")
     reg1_high_string = f"{regfile['reg1_high']}"
     print(reg1_high_string)
     expect_str = "Register reg1_high: {'cfg': 0xaa, 'cfg_trigger': 0x0, 'cfg_trigger_mode': 0x3} = 0x300aa"
     assert reg1_high_string == expect_str
     assert write_count + 2 == rfdev.write_count
     assert read_count + 1 == rfdev.read_count
-    assert str(regfile['reg1_high'].field('cfg')) == 'cfg'
+    assert str(regfile["reg1_high"].field("cfg")) == "cfg"
 
 
 def test_truncation_warning(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
 
-    with warns(UserWarning, match=r'Field\(s\) cfg_trigger_mode were not explicitly set during write '
-                                  'of register reg1_high!'):
-        regfile['reg1_high'] = {'cfg': 0x0bb,
-                                'cfg_trigger': 0x1}
-    assert rfdev.getvalue(0xF000_0008) == 0x1bb
-
-    with warns(UserWarning, match=r'^Ignoring non existent Field NOT_EXISTENT for write.$'):
-        regfile['reg1_high'] = {'NOT_EXISTENT': 0x0ff,
-                                'cfg_trigger': 0x1}
+    with warns(
+        UserWarning,
+        match=r"Field\(s\) cfg_trigger_mode were not explicitly set during write "
+        "of register reg1_high!",
+    ):
+        regfile["reg1_high"] = {"cfg": 0x0BB, "cfg_trigger": 0x1}
+    assert rfdev.getvalue(0xF000_0008) == 0x1BB
+
+    with warns(
+        UserWarning, match=r"^Ignoring non existent Field NOT_EXISTENT for write.$"
+    ):
+        regfile["reg1_high"] = {"NOT_EXISTENT": 0x0FF, "cfg_trigger": 0x1}
 
     assert rfdev.getvalue(0xF000_0008) == 0x100
 
-    with warns(UserWarning, match=r'^Writing read-only field status \(value: 0x00000100 -- mask: 0xffff0000 write_mask: 0x0000001f\).$'):
-        regfile['reg0']['status'] = 0x100
+    with warns(
+        UserWarning,
+        match=r"^Writing read-only field status \(value: 0x00000100 -- mask: 0xffff0000 write_mask: 0x0000001f\).$",
+    ):
+        regfile["reg0"]["status"] = 0x100
 
 
 def test_read_entry(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
     write_count = rfdev.write_count
     read_count = rfdev.read_count
 
-    regfile['reg1_high'] = {'cfg': 0x011,
-                            'cfg_trigger': 0x0,
-                            'cfg_trigger_mode': 0b01}
+    regfile["reg1_high"] = {"cfg": 0x011, "cfg_trigger": 0x0, "cfg_trigger_mode": 0b01}
 
-    entry = regfile['reg1_high'].read_entry()
+    entry = regfile["reg1_high"].read_entry()
     assert rfdev.getvalue(0xF000_0008) == 0x10011
 
-    entry['cfg'] = 0x22
-    entry['cfg_trigger'] = 0x1
-    entry['cfg_trigger_mode'] = 0x0
-    assert entry['cfg'] == 0x22
+    entry["cfg"] = 0x22
+    entry["cfg_trigger"] = 0x1
+    entry["cfg_trigger_mode"] = 0x0
+    assert entry["cfg"] == 0x22
 
-    regfile['reg1_high'] = entry
+    regfile["reg1_high"] = entry
     assert rfdev.getvalue(0xF000_0008) == 0x00122
-    assert {'cfg': 0x077,
-            'cfg_trigger': 0x0,
-            'cfg_trigger_mode': 0b10} == dict(regfile['reg1_high'].get_dict(0x20077))
-
-    assert regfile['reg1_high'].get_value({'cfg': 0x077,
-                                           'cfg_trigger': 0x0,
-                                           'cfg_trigger_mode': 0b10}) == 0x20077
+    assert {"cfg": 0x077, "cfg_trigger": 0x0, "cfg_trigger_mode": 0b10} == dict(
+        regfile["reg1_high"].get_dict(0x20077)
+    )
+
+    assert (
+        regfile["reg1_high"].get_value(
+            {"cfg": 0x077, "cfg_trigger": 0x0, "cfg_trigger_mode": 0b10}
+        )
+        == 0x20077
+    )
 
     assert write_count + 2 == rfdev.write_count
     assert read_count + 1 == rfdev.read_count
-    assert {'cfg': 0x22,
-            'cfg_trigger': 0x1,
-            'cfg_trigger_mode': 0x0} == dict(regfile['reg1_high'].get_dict())
+    assert {"cfg": 0x22, "cfg_trigger": 0x1, "cfg_trigger_mode": 0x0} == dict(
+        regfile["reg1_high"].get_dict()
+    )
     assert read_count + 2 == rfdev.read_count
 
 
 def test_int_access(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
 
     read_count = rfdev.read_count
     write_count = rfdev.write_count
 
-    regfile['reg1_low'] = 0xabcd1234
-    assert regfile['reg1_low']['cfg'] == 0xabcd1234
+    regfile["reg1_low"] = 0xABCD1234
+    assert regfile["reg1_low"]["cfg"] == 0xABCD1234
 
-    regfile['reg1_high'] = 0x1234abcd
-    assert {'cfg': 0xcd,
-            'cfg_trigger': 0x1,
-            'cfg_trigger_mode': 0x0} == dict(regfile['reg1_high'])
-
-    assert regfile['reg1_high'] == 0x1234abcd
-    assert int(regfile['reg1_low']) == 0xabcd1234
-    assert 0x1234abcc < regfile['reg1_high'] < 0x1234abce
-    assert 0x1234abcd <= regfile['reg1_high'] <= 0x1234abce
+    regfile["reg1_high"] = 0x1234ABCD
+    assert {"cfg": 0xCD, "cfg_trigger": 0x1, "cfg_trigger_mode": 0x0} == dict(
+        regfile["reg1_high"]
+    )
+
+    assert regfile["reg1_high"] == 0x1234ABCD
+    assert int(regfile["reg1_low"]) == 0xABCD1234
+    assert 0x1234ABCC < regfile["reg1_high"] < 0x1234ABCE
+    assert 0x1234ABCD <= regfile["reg1_high"] <= 0x1234ABCE
     assert write_count + 2 == rfdev.write_count
     assert read_count + 8 == rfdev.read_count
 
 
 def test_get_reset_values(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
-    assert dict(regfile['reg_addr40'].get_reset_values()) == {'start': 0, **{f'enable_feature{i}': (i + 1) & 0x1 for i in range(4)}}
+    assert dict(regfile["reg_addr40"].get_reset_values()) == {
+        "start": 0,
+        **{f"enable_feature{i}": (i + 1) & 0x1 for i in range(4)},
+    }
 
 
 def test_rfdev_simple(sessionsimpleregfile):
     regfile, rfdev = sessionsimpleregfile
 
     print("write")
-    regfile['reg1_high'] = {'cfg': 0x07a,
-                            'cfg_trigger': 0x1,
-                            'cfg_trigger_mode': 0x0}
+    regfile["reg1_high"] = {"cfg": 0x07A, "cfg_trigger": 0x1, "cfg_trigger_mode": 0x0}
 
     write_count = rfdev.write_count
     read_count = rfdev.read_count
 
     print("compare")
-    assert rfdev.getvalue(0xF000_0008) == 0x0000_017a
+    assert rfdev.getvalue(0xF000_0008) == 0x0000_017A
 
     # read-modify-write
-    regfile['reg1_high']['cfg'] = 0x7b
-    assert rfdev.getvalue(0xF000_0008) == 0x0000_017b
+    regfile["reg1_high"]["cfg"] = 0x7B
+    assert rfdev.getvalue(0xF000_0008) == 0x0000_017B
 
     # read-modify-write
-    regfile['reg1_high']['cfg_trigger_mode'] = 0x3
-    assert rfdev.getvalue(0xF000_0008) == 0x0003_017b
+    regfile["reg1_high"]["cfg_trigger_mode"] = 0x3
+    assert rfdev.getvalue(0xF000_0008) == 0x0003_017B
 
-    regfile['reg0']['cfg'] = 0x1c
+    regfile["reg0"]["cfg"] = 0x1C
 
-    assert rfdev.getvalue(0xF000_0000) & 0x1f == 0x1c
+    assert rfdev.getvalue(0xF000_0000) & 0x1F == 0x1C
 
     assert read_count + 2 == rfdev.read_count
     assert write_count + 3 == rfdev.write_count
 
 
 def test_mem(sessionmemregfile):
     regfile, rfdev = sessionmemregfile
```

### Comparing `regfile_generics-0.0.3/tests/fixtures.py` & `regfile_generics-0.1.0/tests/fixtures.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,76 @@
 #!/usr/bin/env python
 
 import pytest
-from regfile_generics import Regfile, RegfileDevSimpleDebug, RegfileDevSubwordDebug, RegfileMemAccess
+
+from regfile_generics import (
+    Regfile,
+    RegfileDevSimpleDebug,
+    RegfileDevSubwordDebug,
+    RegfileMemAccess,
+)
 
 # Specific registerfile description
 
 
 class submod_regfile(Regfile):
     def __init__(self, rfdev, base_addr):
         super().__init__(rfdev, base_addr)
 
         with self as r:
+            with r["reg0"].represent(addr=0x0000, write_mask=0x0000001F) as e:
+                e["cfg"].represent(
+                    bits="4:0", access="RW", reset="0x0", desc="Configure component"
+                )
+                e["status"].represent(bits="31:16", access="R", desc="Component status")
 
-            with r['reg0'].represent(addr=0x0000, write_mask=0x0000001F) as e:
-                e['cfg'].represent(
-                    bits="4:0",
-                    access="RW",
-                    reset="0x0",
-                    desc="Configure component")
-                e['status'].represent(
-                    bits="31:16", access="R", desc="Component status")
-
-            with r['reg1_low'].represent(addr=0x0004, write_mask=0xFFFFFFFF) as e:
-                e['cfg'].represent(
+            with r["reg1_low"].represent(addr=0x0004, write_mask=0xFFFFFFFF) as e:
+                e["cfg"].represent(
                     bits="31:0",
                     access="RW",
                     reset="0x0",
-                    desc="Configure submod part 0")
+                    desc="Configure submod part 0",
+                )
 
-            with r['reg1_high'].represent(addr=0x0008, write_mask=0x000301FF) as e:
-                e['cfg'].represent(
-                    bits="7:0",
-                    access="RW",
-                    reset="0x0",
-                    desc="Configure submod part 1")
-                e['cfg_trigger'].represent(
-                    bits="8", access="RWT", reset="0b0", desc="trigger config update")
-                e['cfg_trigger_mode'].represent(
-                    bits="17:16", access="RWT", reset="0b0", desc="trigger config update")
-
-            with r['reg2'].represent(addr=0x00C0, write_mask=0x000001F0) as e:
-                e['config'].represent(
-                    bits="8:4",
-                    access="RW",
-                    reset="0x0",
-                    desc="Configure component")
-                e['status'].represent(
-                    bits="31:16", access="R", desc="Component status")
-
-            with r['reg_addr40'].represent(addr=0x0040, write_mask=0x0000001F) as e:
-                e['start'].represent(
-                    bits="0",
-                    access="RW",
+            with r["reg1_high"].represent(addr=0x0008, write_mask=0x000301FF) as e:
+                e["cfg"].represent(
+                    bits="7:0", access="RW", reset="0x0", desc="Configure submod part 1"
+                )
+                e["cfg_trigger"].represent(
+                    bits="8", access="RWT", reset="0b0", desc="trigger config update"
+                )
+                e["cfg_trigger_mode"].represent(
+                    bits="17:16",
+                    access="RWT",
                     reset="0b0",
-                    desc="start's the module")
-                e['enable_feature0'].represent(
-                    bits="1", access="RW", reset="0b1", desc="enables feature0")
-                e['enable_feature1'].represent(
-                    bits="2", access="RW", reset="0b0", desc="enables feature1")
-                e['enable_feature2'].represent(
-                    bits="3", access="RW", reset="0b1", desc="enables feature2")
-                e['enable_feature3'].represent(
-                    bits="4", access="RW", reset="0b0", desc="enables feature3")
+                    desc="trigger config update",
+                )
+
+            with r["reg2"].represent(addr=0x00C0, write_mask=0x000001F0) as e:
+                e["config"].represent(
+                    bits="8:4", access="RW", reset="0x0", desc="Configure component"
+                )
+                e["status"].represent(bits="31:16", access="R", desc="Component status")
+
+            with r["reg_addr40"].represent(addr=0x0040, write_mask=0x0000001F) as e:
+                e["start"].represent(
+                    bits="0", access="RW", reset="0b0", desc="start's the module"
+                )
+                e["enable_feature0"].represent(
+                    bits="1", access="RW", reset="0b1", desc="enables feature0"
+                )
+                e["enable_feature1"].represent(
+                    bits="2", access="RW", reset="0b0", desc="enables feature1"
+                )
+                e["enable_feature2"].represent(
+                    bits="3", access="RW", reset="0b1", desc="enables feature2"
+                )
+                e["enable_feature3"].represent(
+                    bits="4", access="RW", reset="0b0", desc="enables feature3"
+                )
 
 
 """
 regfile devices could inherit from regfile_dev (-> implement rfdev_write // rfdev_read)
     or its highlevel classes (which are simplifing implementation as:
     - regfile_dev_simple  -> implementation of rfdev_write_simple(self, addr, value) // rfdev_read(self, addr)
     - regfile_dev_subword -> implementation of rfdev_write_subword(self, addr, value, size) // rfdev_read(self, addr) [note that addr is unaligned(!) to byteper_word]
```

### Comparing `regfile_generics-0.0.3/tests/lock_instance_test.py` & `regfile_generics-0.1.0/tests/lock_instance_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Regfile access tests"""
 
 import pytest
 
-# pylint: disable=unused-import,redefined-outer-name
-# flake8: noqa
-
 
 def test_regfile_attribute_exception(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
     with pytest.raises(Exception):
-        regfile.reg1_high_r = 0xdead
+        regfile.reg1_high_r = 0xDEAD
 
 
 def test_regfile_entry_attribute_exception(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
-    entry = regfile['reg1_high'].get_register_entry(0x1)
+    entry = regfile["reg1_high"].get_register_entry(0x1)
     with pytest.raises(Exception):
-        entry.cfg_f = 0xdead
+        entry.cfg_f = 0xDEAD
     with pytest.raises(Exception):
-        regfile.reg1_high_r.cfg_f = 0xdead
+        regfile.reg1_high_r.cfg_f = 0xDEAD
```

### Comparing `regfile_generics-0.0.3/tests/uvmlike_access_test.py` & `regfile_generics-0.1.0/tests/uvmlike_access_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,92 @@
 
-# pylint: disable=unused-import,redefined-outer-name
-# flake8: noqa
 from pytest import warns
 
 # pylint: disable=line-too-long,missing-function-docstring
 
 
 def test_uvm_write(sessionsubwordregfile):
     regfile, rfdev = sessionsubwordregfile
     regfile.reset_all()
     write_count = rfdev.write_count
     read_count = rfdev.read_count
 
     regfile.reg0_r.cfg_f.set(1)
     regfile.reg2_r.config_f.set(2)
-    regfile.reg0_r.get_field_by_name('cfg').set(3)
+    regfile.reg0_r.get_field_by_name("cfg").set(3)
     regfile.reg0_r.update()
     regfile.reg2_r.update()
 
-    assert regfile['reg_addr40'].get_mirrored_value() == 0b01010
-    with warns(UserWarning, match=r'enable_feature[2-3]: value 0x2 is truncated to 0x[0-1] \(mask: 0x1\).'):
+    assert regfile["reg_addr40"].get_mirrored_value() == 0b01010
+    with warns(
+        UserWarning,
+        match=r"enable_feature[2-3]: value 0x2 is truncated to 0x[0-1] \(mask: 0x1\).",
+    ):
         for i in range(3, 0, -1):
-            regfile['reg_addr40'].field(f'enable_feature{i}').set(i)
+            regfile["reg_addr40"].field(f"enable_feature{i}").set(i)
 
-    regfile['reg_addr40'].update()
+    regfile["reg_addr40"].update()
 
     assert rfdev.getvalue(0xF000_0000) == 0x3
     assert rfdev.getvalue(0xF000_00C0) == 0x2 << 4
     assert rfdev.getvalue(0xF000_0040) == 0b10110
     write_count += 3
-    assert regfile['reg_addr40'].get_mirrored_value() == 0b10110
+    assert regfile["reg_addr40"].get_mirrored_value() == 0b10110
 
     assert write_count == rfdev.write_count
 
-    regfile['reg_addr40'].set(0b01001)
+    regfile["reg_addr40"].set(0b01001)
     assert rfdev.getvalue(0xF000_0040) == 0b10110
-    assert regfile['reg_addr40'].needs_update() == True
-    assert regfile['reg_addr40'].get() == 0b01001
+    assert regfile["reg_addr40"].needs_update() == True
+    assert regfile["reg_addr40"].get() == 0b01001
 
-    assert regfile['reg_addr40'].get_mirrored_value() == 0b10110
-    regfile['reg_addr40'].update()
+    assert regfile["reg_addr40"].get_mirrored_value() == 0b10110
+    regfile["reg_addr40"].update()
     write_count += 1
     assert write_count == rfdev.write_count
 
     assert rfdev.getvalue(0xF000_0040) == 0b01001
-    assert regfile['reg_addr40'].get_mirrored_value() == 0b01001
-    assert regfile['reg_addr40'].get_reset() == 0b01010
-    assert regfile['reg_addr40'].read() == 0b01001
+    assert regfile["reg_addr40"].get_mirrored_value() == 0b01001
+    assert regfile["reg_addr40"].get_reset() == 0b01010
+    assert regfile["reg_addr40"].read() == 0b01001
 
-    mirrored_reg = regfile['reg_addr40'].get_mirrored_reg()
+    mirrored_reg = regfile["reg_addr40"].get_mirrored_reg()
     assert mirrored_reg.get_mirrored_value() == 0b01001
     assert mirrored_reg.get_reset() == 0b01010
     assert mirrored_reg.read() == 0b01001
 
     assert read_count + 1 == rfdev.read_count
     read_count += 1
-    assert regfile['reg_addr40'].get_offset() == 0x40
-    assert regfile['reg_addr40'].get_address() == 0xF000_0040
+    assert regfile["reg_addr40"].get_offset() == 0x40
+    assert regfile["reg_addr40"].get_address() == 0xF000_0040
 
     # write update
-    regfile.reg_addr40_r.write_update({'start': 0, 'enable_feature0': 1, 'enable_feature1': 1})
+    regfile.reg_addr40_r.write_update(
+        {"start": 0, "enable_feature0": 1, "enable_feature1": 1}
+    )
     write_count += 1
     assert rfdev.getvalue(0xF000_0040) == 0b01110
     assert read_count == rfdev.read_count
     assert write_count == rfdev.write_count
 
     regfile.reg_addr40_r.write_update(start=1, enable_feature0=0, enable_feature1=0)
     write_count += 1
     assert rfdev.getvalue(0xF000_0040) == 0b01001
     assert read_count == rfdev.read_count
     assert write_count == rfdev.write_count
 
     # write:
-    reg_addr40_v = {f'enable_feature{i}': i & 0x1 for i in range(4)}
-    reg_addr40_v['start'] = 0
+    reg_addr40_v = {f"enable_feature{i}": i & 0x1 for i in range(4)}
+    reg_addr40_v["start"] = 0
     regfile.reg_addr40_r.write_update(reg_addr40_v)
     write_count += 1
     assert rfdev.getvalue(0xF000_0040) == 0b10100
     assert read_count == rfdev.read_count
     assert write_count == rfdev.write_count
 
-    regfile.reg_addr40_r.write_update(start=1, **{f'enable_feature{i}': ~i & 0x1 for i in range(4)})
+    regfile.reg_addr40_r.write_update(
+        start=1, **{f"enable_feature{i}": ~i & 0x1 for i in range(4)}
+    )
     assert rfdev.getvalue(0xF000_0040) == 0b01011
     assert read_count == rfdev.read_count
     assert write_count + 1 == rfdev.write_count
     write_count += 1
```

### Comparing `regfile_generics-0.0.3/LICENSE` & `regfile_generics-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regfile_generics-0.0.3/pyproject.toml` & `regfile_generics-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 [build-system]
-requires = ["hatchling"]
+requires = [
+    "hatchling",
+    "hatch-vcs"
+]
 build-backend = "hatchling.build"
 
+[tool.hatch.version]
+source = "vcs"
+
 [project]
 name = "regfile_generics"
-version = "0.0.3"
+dynamic = ['version']
 description = "Python abstraction layer for registerfile access"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
+    {name = "Felix Neumärker", email = "felix.neumaerker@icglue.org"},
     {name = "Andreas Dixius", email = "andreas.dixius@icglue.org"},
+]
+maintainers = [
     {name = "Felix Neumärker", email = "felix.neumaerker@icglue.org"},
+    {name = "Andreas Dixius", email = "andreas.dixius@icglue.org"},
 ]
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
 keywords = ["registerfile"]
@@ -39,12 +49,10 @@
 
 [tool.pylint]
 max-line-length = 120
 
 [tool.autopep8]
 # E501 - Try to make lines fit within --max-line-length characters.
 ignore = ["E501"]
-
 [tool.isort]
-combine_as_imports = true
-multi_line_output = 1
+profile = "black"
 line_length = 120
```

