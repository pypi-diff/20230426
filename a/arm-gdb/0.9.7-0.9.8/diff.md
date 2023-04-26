# Comparing `tmp/arm-gdb-0.9.7.tar.gz` & `tmp/arm-gdb-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm-gdb-0.9.7.tar", last modified: Tue Apr 18 06:58:09 2023, max compression
+gzip compressed data, was "arm-gdb-0.9.8.tar", last modified: Wed Apr 26 20:41:41 2023, max compression
```

## Comparing `arm-gdb-0.9.7.tar` & `arm-gdb-0.9.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/
--rw-r--r--   0 pengi     (1000) pengi     (1000)     1058 2023-04-02 13:47:51.000000 arm-gdb-0.9.7/LICENSE
--rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/PKG-INFO
--rw-r--r--   0 pengi     (1000) pengi     (1000)    15872 2023-04-02 20:46:36.000000 arm-gdb-0.9.7/README.md
-drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/arm_gdb/
--rw-r--r--   0 pengi     (1000) pengi     (1000)     1738 2023-04-04 17:47:23.000000 arm-gdb-0.9.7/arm_gdb/__init__.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     7899 2023-04-02 20:46:36.000000 arm-gdb-0.9.7/arm_gdb/common.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     8636 2023-04-04 16:39:02.000000 arm-gdb-0.9.7/arm_gdb/fpu.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     3645 2023-04-04 18:03:54.000000 arm-gdb-0.9.7/arm_gdb/lib.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     7017 2023-04-04 16:39:02.000000 arm-gdb-0.9.7/arm_gdb/nvic.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)    33393 2023-04-04 19:56:32.000000 arm-gdb-0.9.7/arm_gdb/scb.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     8577 2023-04-04 16:39:02.000000 arm-gdb-0.9.7/arm_gdb/svd.py
--rw-r--r--   0 pengi     (1000) pengi     (1000)     2924 2023-04-04 19:39:03.000000 arm-gdb-0.9.7/arm_gdb/systick.py
-drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/arm_gdb.egg-info/
--rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/PKG-INFO
--rw-r--r--   0 pengi     (1000) pengi     (1000)      319 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/SOURCES.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)        1 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/dependency_links.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)       15 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/requires.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)        8 2023-04-18 06:58:09.000000 arm-gdb-0.9.7/arm_gdb.egg-info/top_level.txt
--rw-r--r--   0 pengi     (1000) pengi     (1000)      789 2023-04-04 17:47:23.000000 arm-gdb-0.9.7/pyproject.toml
--rw-r--r--   0 pengi     (1000) pengi     (1000)       38 2023-04-18 06:58:09.485230 arm-gdb-0.9.7/setup.cfg
+drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-26 20:41:41.957991 arm-gdb-0.9.8/
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     1058 2023-04-02 13:47:51.000000 arm-gdb-0.9.8/LICENSE
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-26 20:41:41.957991 arm-gdb-0.9.8/PKG-INFO
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    15872 2023-04-02 20:46:36.000000 arm-gdb-0.9.8/README.md
+drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-26 20:41:41.953991 arm-gdb-0.9.8/arm_gdb/
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     1738 2023-04-04 17:47:23.000000 arm-gdb-0.9.8/arm_gdb/__init__.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     7995 2023-04-25 13:09:31.000000 arm-gdb-0.9.8/arm_gdb/common.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     8636 2023-04-04 16:39:02.000000 arm-gdb-0.9.8/arm_gdb/fpu.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     3944 2023-04-25 13:13:02.000000 arm-gdb-0.9.8/arm_gdb/lib.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     7017 2023-04-04 16:39:02.000000 arm-gdb-0.9.8/arm_gdb/nvic.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    33393 2023-04-04 19:56:32.000000 arm-gdb-0.9.8/arm_gdb/scb.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    10105 2023-04-25 14:44:32.000000 arm-gdb-0.9.8/arm_gdb/svd.py
+-rw-r--r--   0 pengi     (1000) pengi     (1000)     2924 2023-04-04 19:39:03.000000 arm-gdb-0.9.8/arm_gdb/systick.py
+drwxr-xr-x   0 pengi     (1000) pengi     (1000)        0 2023-04-26 20:41:41.957991 arm-gdb-0.9.8/arm_gdb.egg-info/
+-rw-r--r--   0 pengi     (1000) pengi     (1000)    17667 2023-04-26 20:41:41.000000 arm-gdb-0.9.8/arm_gdb.egg-info/PKG-INFO
+-rw-r--r--   0 pengi     (1000) pengi     (1000)      319 2023-04-26 20:41:41.000000 arm-gdb-0.9.8/arm_gdb.egg-info/SOURCES.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)        1 2023-04-26 20:41:41.000000 arm-gdb-0.9.8/arm_gdb.egg-info/dependency_links.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)       15 2023-04-26 20:41:41.000000 arm-gdb-0.9.8/arm_gdb.egg-info/requires.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)        8 2023-04-26 20:41:41.000000 arm-gdb-0.9.8/arm_gdb.egg-info/top_level.txt
+-rw-r--r--   0 pengi     (1000) pengi     (1000)      789 2023-04-04 17:47:23.000000 arm-gdb-0.9.8/pyproject.toml
+-rw-r--r--   0 pengi     (1000) pengi     (1000)       38 2023-04-26 20:41:41.957991 arm-gdb-0.9.8/setup.cfg
```

### Comparing `arm-gdb-0.9.7/LICENSE` & `arm-gdb-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.7/PKG-INFO` & `arm-gdb-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-gdb
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python module for GDB to analyze ARM core registers
 Author-email: Max Sikström <max@pengi.se>
 License: Copyright (c) 2023 Max Sikström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `arm-gdb-0.9.7/README.md` & `arm-gdb-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.7/arm_gdb/__init__.py` & `arm-gdb-0.9.8/arm_gdb/__init__.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.7/arm_gdb/common.py` & `arm-gdb-0.9.8/arm_gdb/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-FileCopyrightText: 2023 Max Sikström
 # SPDX-License-Identifier: MIT
 
 # Copyright © 2023 Max Sikström
+# Copyright © 2023 Niklas Hauser
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -124,15 +125,15 @@
         ]
         print("Usage:", *args)
 
 
 class RegisterDef:
     def __init__(self, name, descr, addr, size, fields=[]):
         self.name = name
-        self.descr = descr
+        self.descr = norm_descr(descr) if descr else None
         self.addr = addr
         self.size = size
         self.fields = fields
 
     def dump(self, inf, include_descr=True, base=4, all=False):
         m_int = read_reg(inf, self.addr, self.size)
 
@@ -150,15 +151,15 @@
             if all or field.should_print(m_int):
                 field.print(m_int, include_descr, base=base)
 
 
 class Field:
     def __init__(self, name, descr=None, always=False):
         self.name = name
-        self.descr = descr
+        self.descr = norm_descr(descr) if descr else None
         self.always = always
 
     def should_print(self, value):
         return False
 
     def get_value(self, value):
         return 0
```

### Comparing `arm-gdb-0.9.7/arm_gdb/fpu.py` & `arm-gdb-0.9.8/arm_gdb/fpu.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.7/arm_gdb/lib.py` & `arm-gdb-0.9.8/arm_gdb/lib.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-FileCopyrightText: 2023 Max Sikström
 # SPDX-License-Identifier: MIT
 
 # Copyright © 2023 Max Sikström
+# Copyright © 2023 Niklas Hauser
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,14 +21,16 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 #
 # Library functions, that can be tested outside of gdb. used for type
 #
+import re
+
 def base_convert(val, base, bits):
     """
     Convert a value to string, given base
 
     The base is specified as 2**n, thus number of bits to group. And up to 2**4.
     Thus basically binary, octal and hex.
 
@@ -112,11 +115,21 @@
         if (
             tags is None or
             m is None or
             len(set(m.split(",")) & tags) > 0
         )
     ]
 
+def norm_descr(text):
+    """
+    Replace multiple successive line breaks, tabs and spaces a single space to
+    compactify descriptions.
+
+    >>> norm_descr('Hello\\n\\t     World')
+    'Hello World'
+    """
+    return re.sub(r"[\n\r\t ]+", " ", text)
+
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod(verbose=True)
```

### Comparing `arm-gdb-0.9.7/arm_gdb/nvic.py` & `arm-gdb-0.9.8/arm_gdb/nvic.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.7/arm_gdb/scb.py` & `arm-gdb-0.9.8/arm_gdb/scb.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.7/arm_gdb/svd.py` & `arm-gdb-0.9.8/arm_gdb/svd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-FileCopyrightText: 2023 Max Sikström
 # SPDX-License-Identifier: MIT
 
 # Copyright © 2023 Max Sikström
+# Copyright © 2023 Niklas Hauser
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the “Software”), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -56,39 +57,55 @@
         device = args[self.device_arg]
         for p in device.peripherals:
             if p.name == word:
                 return p
         return None
 
 
+class RegistersArgType(ArgType):
+    def __init__(self, name, peripheral_arg, optional=False):
+        super().__init__(name, optional=optional)
+        self.peripheral_arg = peripheral_arg
+
+    def complete(self, word, args={}):
+        return [r.name for r in args[self.peripheral_arg].registers
+                if r.name.startswith(word)]
+
+    def get(self, word, args={}):
+        return next((r for r in args[self.peripheral_arg].registers
+                     if r.name == word), None)
+
+
 class ArmToolsSVDList (ArgCommand):
     """List peripherals and registers from device
 
 Usage: arm list
 
 Lists loaded devices
 
 Usage: arm list <device>
 
 List peripherals from a device
 
-Usage: arm list <device> <peripheral>
+Usage: arm list <device> <peripheral> [<register>]
 
-List registers from a peripheral
+List one or all registers from a peripheral
 
 Examples:
     arm list
     arm list nrf52840
     arm list nrf52840 UARTE0
+    arm list nrf52840 UARTE0 EVENTS_RXDRDY
 """
 
     def __init__(self):
         super().__init__('arm list', gdb.COMMAND_SUPPORT)
         self.add_arg(DevicesArgType('device', optional=True))
         self.add_arg(PeripheralsArgType('peripheral', 'device', optional=True))
+        self.add_arg(RegistersArgType('register', 'peripheral', optional=True))
 
     def invoke(self, argument, from_tty):
         args = self.process_args(argument)
         if args is None:
             self.print_help()
             return
 
@@ -105,72 +122,90 @@
                         peripheral.name,
                         peripheral.base_address
                     )
                 )
         else:
             device = args['device']
             peripheral = args['peripheral']
-            print(
-                "Registers in %s @ 0x%08x:" % (
-                    peripheral.name,
-                    peripheral.base_address
+            if 'register' in args:
+                registers = [args['register']]
+                print(
+                    "Register %s in %s @ 0x%08x:" % (
+                        registers[0].name,
+                        peripheral.name,
+                        peripheral.base_address
+                    )
                 )
-            )
-            for register in peripheral.registers:
+            else:
+                registers = peripheral.registers
+                print(
+                    "Registers in %s @ 0x%08x:" % (
+                        peripheral.name,
+                        peripheral.base_address
+                    )
+                )
+
+            for register in sorted(registers, key=lambda r: r.address_offset):
                 print(
                     " - %s @ +0x%x" % (
                         register.name,
                         register.address_offset
                     )
                 )
-                for field in register._fields:
+                for field in sorted(register._fields, key=lambda f: f.bit_offset):
                     mask = "." * (32-field.bit_offset-field.bit_width) + \
                         "#" * field.bit_width + "." * field.bit_offset
 
                     print("        %s %s" % (mask, field.name))
 
 
 class ArmToolsSVDInspect (ArgCommand):
     """Dump register values from device peripheral
 
-Usage: arm inspect [/hab] <device> <peripheral>
+Usage: arm inspect [/hab] <device> <peripheral> [<register>]
 
 Modifier /h provides descriptions of names where available
 Modifier /a Print all fields, including default values
 Modifier /b prints bitmasks in binary instead of hex
 
     <device>     - Name of loaded device. See `help arm loadfile`
     <peripheral> - Name of peripheral
+    <register>   - Name of register (optional)
 
-Exmaple: arm inspect nrf52840 UARTE0
+Examples:
+    arm inspect nrf52840 UARTE0
+    arm inspect nrf52840 UARTE0 EVENTS_RXDRDY
 """
 
     def __init__(self):
         super().__init__('arm inspect', gdb.COMMAND_DATA)
         self.add_arg(DevicesArgType('device'))
         self.add_arg(PeripheralsArgType('peripheral', 'device'))
+        self.add_arg(RegistersArgType('register', 'peripheral', optional=True))
         self.add_mod('h', 'descr')
         self.add_mod('a', 'all')
         self.add_mod('b', 'binary')
 
     def invoke(self, argument, from_tty):
         args = self.process_args(argument)
         if args is None:
             self.print_help()
             return
 
         base = 1 if args['binary'] else 4
 
         peripheral = args['peripheral']
+        registers = [args['register']] if 'register' in args \
+                    else peripheral.registers
 
         inf = gdb.selected_inferior()
 
-        for register in peripheral.registers:
+        for register in sorted(registers, key=lambda r: r.address_offset):
             fields = []
-            for field in register._fields:
+            for field in sorted(register._fields, key=lambda f: f.bit_offset):
                 if field.is_enumerated_type:
                     fields.append(FieldBitfieldEnum(
                         field.name,
                         field.bit_offset,
                         field.bit_width,
                         [
                             (ev.value, ev.is_default, ev.name, ev.description)
```

### Comparing `arm-gdb-0.9.7/arm_gdb/systick.py` & `arm-gdb-0.9.8/arm_gdb/systick.py`

 * *Files identical despite different names*

### Comparing `arm-gdb-0.9.7/arm_gdb.egg-info/PKG-INFO` & `arm-gdb-0.9.8/arm_gdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-gdb
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python module for GDB to analyze ARM core registers
 Author-email: Max Sikström <max@pengi.se>
 License: Copyright (c) 2023 Max Sikström
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `arm-gdb-0.9.7/pyproject.toml` & `arm-gdb-0.9.8/pyproject.toml`

 * *Files identical despite different names*

