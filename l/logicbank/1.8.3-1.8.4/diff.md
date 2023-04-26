# Comparing `tmp/logicbank-1.8.3.tar.gz` & `tmp/logicbank-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logicbank-1.8.3.tar", last modified: Sat Mar  4 19:37:06 2023, max compression
+gzip compressed data, was "logicbank-1.8.4.tar", last modified: Wed Apr 26 19:02:23 2023, max compression
```

## Comparing `logicbank-1.8.3.tar` & `logicbank-1.8.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.445326 logicbank-1.8.3/
--rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-22 20:44:43.000000 logicbank-1.8.3/LICENSE
--rw-r--r--   0 val        (502) staff       (20)    15441 2023-03-04 19:37:06.445182 logicbank-1.8.3/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)    14645 2022-08-22 20:44:43.000000 logicbank-1.8.3/README.md
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.437301 logicbank-1.8.3/logic_bank/
--rw-r--r--   0 val        (502) staff       (20)     1300 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/__init__.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.437635 logicbank-1.8.3/logic_bank/exec_row_logic/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/exec_row_logic/__init__.py
--rw-r--r--   0 val        (502) staff       (20)    54288 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/exec_row_logic/logic_row.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.441297 logicbank-1.8.3/logic_bank/exec_trans_logic/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/exec_trans_logic/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     5379 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/exec_trans_logic/listeners.py
--rw-r--r--   0 val        (502) staff       (20)     2524 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/exec_trans_logic/row_sets.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.442192 logicbank-1.8.3/logic_bank/extensions/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/extensions/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     4474 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/extensions/allocate.py
--rw-r--r--   0 val        (502) staff       (20)     1550 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/extensions/copy_children.py
--rw-r--r--   0 val        (502) staff       (20)     1882 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/extensions/copy_row.py
--rw-r--r--   0 val        (502) staff       (20)     3184 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/extensions/rule_extensions.py
--rw-r--r--   0 val        (502) staff       (20)    12917 2023-03-04 19:07:46.000000 logicbank-1.8.3/logic_bank/logic_bank.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.442734 logicbank-1.8.3/logic_bank/rule_bank/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_bank/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     2288 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_bank/rule_bank.py
--rw-r--r--   0 val        (502) staff       (20)     3628 2023-03-04 19:07:46.000000 logicbank-1.8.3/logic_bank/rule_bank/rule_bank_setup.py
--rw-r--r--   0 val        (502) staff       (20)     8686 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_bank/rule_bank_withdraw.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.444378 logicbank-1.8.3/logic_bank/rule_type/
--rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_type/__init__.py
--rw-r--r--   0 val        (502) staff       (20)     4582 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_type/abstractrule.py
--rw-r--r--   0 val        (502) staff       (20)    11754 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/rule_type/aggregate.py
--rw-r--r--   0 val        (502) staff       (20)     3288 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/rule_type/constraint.py
--rw-r--r--   0 val        (502) staff       (20)     2259 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/rule_type/copy.py
--rw-r--r--   0 val        (502) staff       (20)     2417 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/rule_type/count.py
--rw-r--r--   0 val        (502) staff       (20)      711 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/rule_type/derivation.py
--rw-r--r--   0 val        (502) staff       (20)     3394 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/rule_type/formula.py
--rw-r--r--   0 val        (502) staff       (20)     1048 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_type/parent_cascade.py
--rw-r--r--   0 val        (502) staff       (20)      686 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_type/parent_check.py
--rw-r--r--   0 val        (502) staff       (20)     1663 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/rule_type/row_event.py
--rw-r--r--   0 val        (502) staff       (20)     3135 2023-02-25 18:32:07.000000 logicbank-1.8.3/logic_bank/rule_type/sum.py
--rw-r--r--   0 val        (502) staff       (20)     5552 2022-08-22 20:44:43.000000 logicbank-1.8.3/logic_bank/util.py
-drwxr-xr-x   0 val        (502) staff       (20)        0 2023-03-04 19:37:06.445010 logicbank-1.8.3/logicbank.egg-info/
--rw-r--r--   0 val        (502) staff       (20)    15441 2023-03-04 19:37:06.000000 logicbank-1.8.3/logicbank.egg-info/PKG-INFO
--rw-r--r--   0 val        (502) staff       (20)     1222 2023-03-04 19:37:06.000000 logicbank-1.8.3/logicbank.egg-info/SOURCES.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-03-04 19:37:06.000000 logicbank-1.8.3/logicbank.egg-info/dependency_links.txt
--rw-r--r--   0 val        (502) staff       (20)        1 2023-03-04 19:37:06.000000 logicbank-1.8.3/logicbank.egg-info/not-zip-safe
--rw-r--r--   0 val        (502) staff       (20)       40 2023-03-04 19:37:06.000000 logicbank-1.8.3/logicbank.egg-info/requires.txt
--rw-r--r--   0 val        (502) staff       (20)       11 2023-03-04 19:37:06.000000 logicbank-1.8.3/logicbank.egg-info/top_level.txt
--rw-r--r--   0 val        (502) staff       (20)       38 2023-03-04 19:37:06.445358 logicbank-1.8.3/setup.cfg
--rw-r--r--   0 val        (502) staff       (20)     1814 2022-08-22 20:44:43.000000 logicbank-1.8.3/setup.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.400114 logicbank-1.8.4/
+-rw-r--r--   0 val        (502) staff       (20)     1485 2022-08-22 20:44:43.000000 logicbank-1.8.4/LICENSE
+-rw-r--r--   0 val        (502) staff       (20)    15441 2023-04-26 19:02:23.399939 logicbank-1.8.4/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)    14645 2023-04-16 15:33:22.000000 logicbank-1.8.4/README.md
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.394249 logicbank-1.8.4/logic_bank/
+-rw-r--r--   0 val        (502) staff       (20)     1300 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/__init__.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.394592 logicbank-1.8.4/logic_bank/exec_row_logic/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/exec_row_logic/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)    55066 2023-04-26 18:32:55.000000 logicbank-1.8.4/logic_bank/exec_row_logic/logic_row.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.395814 logicbank-1.8.4/logic_bank/exec_trans_logic/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/exec_trans_logic/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     5379 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/exec_trans_logic/listeners.py
+-rw-r--r--   0 val        (502) staff       (20)     2524 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/exec_trans_logic/row_sets.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.396529 logicbank-1.8.4/logic_bank/extensions/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/extensions/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     4474 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/extensions/allocate.py
+-rw-r--r--   0 val        (502) staff       (20)     1550 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/extensions/copy_children.py
+-rw-r--r--   0 val        (502) staff       (20)     1882 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/extensions/copy_row.py
+-rw-r--r--   0 val        (502) staff       (20)     3184 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/extensions/rule_extensions.py
+-rw-r--r--   0 val        (502) staff       (20)    13052 2023-04-26 18:54:01.000000 logicbank-1.8.4/logic_bank/logic_bank.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.396962 logicbank-1.8.4/logic_bank/rule_bank/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_bank/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     2288 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_bank/rule_bank.py
+-rw-r--r--   0 val        (502) staff       (20)     3628 2023-04-16 15:32:58.000000 logicbank-1.8.4/logic_bank/rule_bank/rule_bank_setup.py
+-rw-r--r--   0 val        (502) staff       (20)     8686 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_bank/rule_bank_withdraw.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.398807 logicbank-1.8.4/logic_bank/rule_type/
+-rw-r--r--   0 val        (502) staff       (20)        0 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_type/__init__.py
+-rw-r--r--   0 val        (502) staff       (20)     4582 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_type/abstractrule.py
+-rw-r--r--   0 val        (502) staff       (20)    11754 2023-02-25 18:32:07.000000 logicbank-1.8.4/logic_bank/rule_type/aggregate.py
+-rw-r--r--   0 val        (502) staff       (20)     3288 2023-02-25 18:32:07.000000 logicbank-1.8.4/logic_bank/rule_type/constraint.py
+-rw-r--r--   0 val        (502) staff       (20)     2259 2023-02-25 18:32:07.000000 logicbank-1.8.4/logic_bank/rule_type/copy.py
+-rw-r--r--   0 val        (502) staff       (20)     2417 2023-02-25 18:32:07.000000 logicbank-1.8.4/logic_bank/rule_type/count.py
+-rw-r--r--   0 val        (502) staff       (20)      711 2023-02-25 18:32:07.000000 logicbank-1.8.4/logic_bank/rule_type/derivation.py
+-rw-r--r--   0 val        (502) staff       (20)     3394 2023-02-25 18:32:07.000000 logicbank-1.8.4/logic_bank/rule_type/formula.py
+-rw-r--r--   0 val        (502) staff       (20)     1048 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_type/parent_cascade.py
+-rw-r--r--   0 val        (502) staff       (20)      686 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_type/parent_check.py
+-rw-r--r--   0 val        (502) staff       (20)     1663 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/rule_type/row_event.py
+-rw-r--r--   0 val        (502) staff       (20)     3135 2023-02-25 18:32:07.000000 logicbank-1.8.4/logic_bank/rule_type/sum.py
+-rw-r--r--   0 val        (502) staff       (20)     5552 2022-08-22 20:44:43.000000 logicbank-1.8.4/logic_bank/util.py
+drwxr-xr-x   0 val        (502) staff       (20)        0 2023-04-26 19:02:23.399710 logicbank-1.8.4/logicbank.egg-info/
+-rw-r--r--   0 val        (502) staff       (20)    15441 2023-04-26 19:02:23.000000 logicbank-1.8.4/logicbank.egg-info/PKG-INFO
+-rw-r--r--   0 val        (502) staff       (20)     1222 2023-04-26 19:02:23.000000 logicbank-1.8.4/logicbank.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-04-26 19:02:23.000000 logicbank-1.8.4/logicbank.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (502) staff       (20)        1 2023-04-26 19:02:23.000000 logicbank-1.8.4/logicbank.egg-info/not-zip-safe
+-rw-r--r--   0 val        (502) staff       (20)       40 2023-04-26 19:02:23.000000 logicbank-1.8.4/logicbank.egg-info/requires.txt
+-rw-r--r--   0 val        (502) staff       (20)       11 2023-04-26 19:02:23.000000 logicbank-1.8.4/logicbank.egg-info/top_level.txt
+-rw-r--r--   0 val        (502) staff       (20)       38 2023-04-26 19:02:23.400150 logicbank-1.8.4/setup.cfg
+-rw-r--r--   0 val        (502) staff       (20)     1814 2022-08-22 20:44:43.000000 logicbank-1.8.4/setup.py
```

### Comparing `logicbank-1.8.3/LICENSE` & `logicbank-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/PKG-INFO` & `logicbank-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logicbank
-Version: 1.8.3
+Version: 1.8.4
 Summary: Declare multi-table rules for SQLAlchemy update logic -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/logicbank
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://github.com/valhuber/logicbank/wiki
 Platform: any
```

### Comparing `logicbank-1.8.3/README.md` & `logicbank-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/__init__.py` & `logicbank-1.8.4/logic_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/exec_row_logic/logic_row.py` & `logicbank-1.8.4/logic_bank/exec_row_logic/logic_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 class LogicRow:
     """
     Wraps row and  old_row, plus methods for insert, update and delete - rule enforcement
 
     Passed to user logic, mainly to make updates - with logic, for example
 
         row = sqlalchemy read
+
         logic_row.update(row=row, msg="my log message")
 
     Additional instance variables: ins_upd_dlt, nest_level, session, etc.
 
     Helper Methods
         are_attributes_changed, set_same_named_attributes,
         get_parent_logic_row(role_name), get_derived_attributes, log, etc
@@ -48,14 +49,15 @@
         """
         self.session = a_session
         self.row = row  # type(base)
         """ mapped row """
         self.old_row = old_row
         """ old mapped row """
         self.ins_upd_dlt = ins_upd_dlt
+        """ values are 'ins', 'upd' or 'dlt' """
         self.ins_upd_dlt_initial = ins_upd_dlt  # order inserted, then adjusted
         self.nest_level = nest_level
         self.reason = "?"  # set by insert, update and delete
         """ if starts with cascade, triggers cascade processing """
 
         self.row_sets = row_sets
         fixme_set_processed_in_init = False
@@ -257,14 +259,26 @@
                     if attributes_copied == "":
                         attributes_copied = each_copy_rule._column
                     else:
                         attributes_copied += f', {each_copy_rule._column}'
                     each_copy_rule.execute(logic_row, parent_logic_row)
                 self.log(f'copy_rules for role: {role_name} - {attributes_copied}')
 
+    def is_inserted(self) -> bool:
+        """ return True if self.ins_upd_dlt == "ins" else False """
+        return True if self.ins_upd_dlt == "ins" else False
+
+    def is_updated(self) -> bool:
+        """ return True if self.ins_upd_dlt == "upd" else False """
+        return True if self.ins_upd_dlt == "upd" else False
+
+    def is_deleted(self) -> bool:
+        """ return True if self.ins_upd_dlt == "dlt" else False """
+        return True if self.ins_upd_dlt == "dlt" else False
+    
     def _get_parent_role_def(self, parent_role_name: str):
         """ returns sqlalchemy role_def """
         my_mapper = object_mapper(self.row)
         role_def = my_mapper.relationships.get(parent_role_name)
         if role_def is None:
             raise Exception(f"FIXME invalid role name {parent_role_name}")
         return role_def
@@ -694,16 +708,19 @@
                         break
                 else:
                     if getattr(row, column) != getattr(old_row, column):
                         is_dependent_changed = True
                         break
             result_prune = not (is_parent_changed or is_dependent_changed)
         if result_prune:
-            self.log("Prune Formula: " + formula._column +
-                     " [" + str(formula._dependencies) + "]")
+            log_text = "Prune Formula: " + formula._column + " [" + str(formula._dependencies) + "]"
+            if formula._no_prune:  # e.g., no attributes referenced, such as time/date stamp
+                result_prune = False
+                log_text = log_text.replace("Prune", "Pruned Formula retained per no_prune")
+            self.log(log_text)
         return result_prune
 
     def _formula_rules(self):
         """ execute un-pruned formulae, in dependency order """
         self.log_engine("formula_rules")
         formula_rules = rule_bank_withdraw.rules_of_class(self, Formula)
         formula_rules.sort(key=lambda formula: formula._exec_order)
```

### Comparing `logicbank-1.8.3/logic_bank/exec_trans_logic/listeners.py` & `logicbank-1.8.4/logic_bank/exec_trans_logic/listeners.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/exec_trans_logic/row_sets.py` & `logicbank-1.8.4/logic_bank/exec_trans_logic/row_sets.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/extensions/allocate.py` & `logicbank-1.8.4/logic_bank/extensions/allocate.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/extensions/copy_children.py` & `logicbank-1.8.4/logic_bank/extensions/copy_children.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/extensions/copy_row.py` & `logicbank-1.8.4/logic_bank/extensions/copy_row.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/extensions/rule_extensions.py` & `logicbank-1.8.4/logic_bank/extensions/rule_extensions.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/logic_bank.py` & `logicbank-1.8.4/logic_bank/logic_bank.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
         LogicBank.activate(session=session, activator=declare_logic)  # register LogicBank listeners to SQLAlchemy
 
     3. Execute them:
 
         session.commit()  # LogicBank listeners execute rules relevant for submitted changes
 
     .. _Rule Summary:
+   
+   https://apilogicserver.github.io/Docs/Logic/
+   
    https://github.com/valhuber/LogicBank/wiki/Rule-Summary
 
     """
 
     @staticmethod
     def activate(session: session, activator: callable, constraint_event: callable = None):
         """
@@ -196,14 +199,16 @@
 
         Example
           Rule.formula(derive=models.OrderDetail.Amount,
                        as_expression=lambda row: row.UnitPrice * row.Quantity)
 
         Unlike Copy rules, Parent changes are propagated to child row(s)
 
+        The `calling` function must return a value (else column is nullified)
+
         Args:
             derive: <class.attribute> being derived
             as_exp: string (for very short expressions - price * quantity)
             as_expression: lambda, passed row (for syntax checking)
             calling: function (for more complex formula, pass row, old_row, logic_row)
             no_prune: disable pruning (rarely used, default False)
         """
```

### Comparing `logicbank-1.8.3/logic_bank/rule_bank/rule_bank.py` & `logicbank-1.8.4/logic_bank/rule_bank/rule_bank.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_bank/rule_bank_setup.py` & `logicbank-1.8.4/logic_bank/rule_bank/rule_bank_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from logic_bank.rule_bank.rule_bank import RuleBank
 from logic_bank.rule_bank import rule_bank_withdraw
 from logic_bank.exec_trans_logic.listeners import before_flush, before_commit
 from sqlalchemy.orm import session
 import logging
 
-__version__ = "01.08.03"
+__version__ = "01.08.04"
 
 
 def setup(a_session: session):
     """
     Create the RuleBank
 
     Register before_flush listeners
```

### Comparing `logicbank-1.8.3/logic_bank/rule_bank/rule_bank_withdraw.py` & `logicbank-1.8.4/logic_bank/rule_bank/rule_bank_withdraw.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/abstractrule.py` & `logicbank-1.8.4/logic_bank/rule_type/abstractrule.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/aggregate.py` & `logicbank-1.8.4/logic_bank/rule_type/aggregate.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/constraint.py` & `logicbank-1.8.4/logic_bank/rule_type/constraint.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/copy.py` & `logicbank-1.8.4/logic_bank/rule_type/copy.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/count.py` & `logicbank-1.8.4/logic_bank/rule_type/count.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/derivation.py` & `logicbank-1.8.4/logic_bank/rule_type/derivation.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/formula.py` & `logicbank-1.8.4/logic_bank/rule_type/formula.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/parent_cascade.py` & `logicbank-1.8.4/logic_bank/rule_type/parent_cascade.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/parent_check.py` & `logicbank-1.8.4/logic_bank/rule_type/parent_check.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/row_event.py` & `logicbank-1.8.4/logic_bank/rule_type/row_event.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/rule_type/sum.py` & `logicbank-1.8.4/logic_bank/rule_type/sum.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logic_bank/util.py` & `logicbank-1.8.4/logic_bank/util.py`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/logicbank.egg-info/PKG-INFO` & `logicbank-1.8.4/logicbank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logicbank
-Version: 1.8.3
+Version: 1.8.4
 Summary: Declare multi-table rules for SQLAlchemy update logic -- 40X more concise, Python for extensibility.
 Home-page: https://github.com/valhuber/logicbank
 Author: Val Huber
 Author-email: valjhuber@gmail.com
 License: BSD
 Project-URL: Docs, https://github.com/valhuber/logicbank/wiki
 Platform: any
```

### Comparing `logicbank-1.8.3/logicbank.egg-info/SOURCES.txt` & `logicbank-1.8.4/logicbank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logicbank-1.8.3/setup.py` & `logicbank-1.8.4/setup.py`

 * *Files identical despite different names*

