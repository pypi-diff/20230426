# Comparing `tmp/transtab-0.0.3.tar.gz` & `tmp/transtab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transtab-0.0.3.tar", last modified: Thu Jan  5 05:27:57 2023, max compression
+gzip compressed data, was "dist/transtab-0.0.4.tar", last modified: Tue Apr 25 15:32:20 2023, max compression
```

## Comparing `transtab-0.0.3.tar` & `transtab-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-05 05:27:57.000000 transtab-0.0.3/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-01-05 04:33:25.000000 transtab-0.0.3/LICENSE
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5145 2023-01-05 05:27:57.000000 transtab-0.0.3/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4475 2023-01-05 05:17:42.000000 transtab-0.0.3/README.md
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-01-05 05:27:57.000000 transtab-0.0.3/setup.cfg
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1202 2023-01-05 05:18:05.000000 transtab-0.0.3/setup.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-05 05:27:57.000000 transtab-0.0.3/transtab/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       61 2023-01-05 05:17:51.000000 transtab-0.0.3/transtab/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      368 2023-01-05 04:33:25.000000 transtab-0.0.3/transtab/constants.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10943 2023-01-05 04:33:25.000000 transtab-0.0.3/transtab/dataset.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5835 2023-01-05 04:50:18.000000 transtab-0.0.3/transtab/evaluator.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    49949 2023-01-05 05:14:08.000000 transtab-0.0.3/transtab/modeling_transtab.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13644 2023-01-05 04:33:25.000000 transtab-0.0.3/transtab/trainer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7764 2023-01-05 04:33:25.000000 transtab-0.0.3/transtab/trainer_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15248 2023-01-05 05:10:44.000000 transtab-0.0.3/transtab/transtab.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-05 05:27:57.000000 transtab-0.0.3/transtab.egg-info/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5145 2023-01-05 05:27:57.000000 transtab-0.0.3/transtab.egg-info/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      367 2023-01-05 05:27:57.000000 transtab-0.0.3/transtab.egg-info/SOURCES.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-01-05 05:27:57.000000 transtab-0.0.3/transtab.egg-info/dependency_links.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       95 2023-01-05 05:27:57.000000 transtab-0.0.3/transtab.egg-info/requires.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        9 2023-01-05 05:27:57.000000 transtab-0.0.3/transtab.egg-info/top_level.txt
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 15:32:20.000000 transtab-0.0.4/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2022-08-23 14:54:33.000000 transtab-0.0.4/LICENSE
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5145 2023-04-25 15:32:20.000000 transtab-0.0.4/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4475 2023-02-03 17:30:10.000000 transtab-0.0.4/README.md
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-04-25 15:32:20.000000 transtab-0.0.4/setup.cfg
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1202 2023-04-25 15:31:30.000000 transtab-0.0.4/setup.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       61 2023-04-25 15:30:33.000000 transtab-0.0.4/transtab/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      368 2022-08-31 18:57:31.000000 transtab-0.0.4/transtab/constants.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10943 2022-08-31 18:28:18.000000 transtab-0.0.4/transtab/dataset.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5835 2023-02-03 17:30:10.000000 transtab-0.0.4/transtab/evaluator.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    50323 2023-02-03 17:47:03.000000 transtab-0.0.4/transtab/modeling_transtab.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13825 2023-02-03 17:54:22.000000 transtab-0.0.4/transtab/trainer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7764 2022-08-26 01:52:18.000000 transtab-0.0.4/transtab/trainer_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15248 2022-09-05 21:13:13.000000 transtab-0.0.4/transtab/transtab.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5145 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      367 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/SOURCES.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/dependency_links.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       84 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/requires.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        9 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/top_level.txt
```

### Comparing `transtab-0.0.3/LICENSE` & `transtab-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `transtab-0.0.3/PKG-INFO` & `transtab-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transtab
-Version: 0.0.3
+Version: 0.0.4
 Summary: A flexible tabular prediction model that handles variable-column input tables.
 Home-page: https://github.com/RyanWangZf/transtab
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
 Keywords: tabular data,machine learning,data mining,data science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `transtab-0.0.3/README.md` & `transtab-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `transtab-0.0.3/setup.py` & `transtab-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # read the contents of requirements.txt
 with open(os.path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name = 'transtab',
-    version = '0.0.3',
+    version = '0.0.4',
     author = 'Zifeng Wang',
     author_email = 'zifengw2@illinois.edu',
     description = 'A flexible tabular prediction model that handles variable-column input tables.',
     url = 'https://github.com/RyanWangZf/transtab',
     keywords=['tabular data', 'machine learning', 'data mining', 'data science'],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `transtab-0.0.3/transtab/dataset.py` & `transtab-0.0.4/transtab/dataset.py`

 * *Files identical despite different names*

### Comparing `transtab-0.0.3/transtab/evaluator.py` & `transtab-0.0.4/transtab/evaluator.py`

 * *Files identical despite different names*

### Comparing `transtab-0.0.3/transtab/modeling_transtab.py` & `transtab-0.0.4/transtab/modeling_transtab.py`

 * *Files 2% similar despite different names*

```diff
@@ -830,17 +830,15 @@
         self.input_encoder.feature_extractor.update(**col_map)
         self.binary_columns = self.input_encoder.feature_extractor.binary_columns
         self.categorical_columns = self.input_encoder.feature_extractor.categorical_columns
         self.numerical_columns = self.input_encoder.feature_extractor.numerical_columns
 
         if 'num_class' in config:
             num_class = config['num_class']
-            self.clf = TransTabLinearClassifier(num_class, hidden_dim=self.cls_token.hidden_dim)
-            self.clf.to(self.device)
-            logger.info(f'Build a new classifier with num {num_class} classes outputs, need further finetune to work.')
+            self._adapt_to_new_num_class(num_class)
 
         return None
 
     def _check_column_overlap(self, cat_cols=None, num_cols=None, bin_cols=None):
         all_cols = []
         if cat_cols is not None: all_cols.extend(cat_cols)
         if num_cols is not None: all_cols.extend(num_cols)
@@ -859,14 +857,25 @@
             if col in self.numerical_columns:
                 self.numerical_columns.remove(col)
                 self.numerical_columns.append(f'[num]{col}')
             if col in self.binary_columns:
                 self.binary_columns.remove(col)
                 self.binary_columns.append(f'[bin]{col}')
 
+    def _adapt_to_new_num_class(self, num_class):
+        if num_class != self.num_class:
+            self.num_class = num_class
+            self.clf = TransTabLinearClassifier(num_class, hidden_dim=self.cls_token.hidden_dim)
+            self.clf.to(self.device)
+            if self.num_class > 2:
+                self.loss_fn = nn.CrossEntropyLoss(reduction='none')
+            else:
+                self.loss_fn = nn.BCEWithLogitsLoss(reduction='none')
+            logger.info(f'Build a new classifier with num {num_class} classes outputs, need further finetune to work.')
+
 
 class TransTabClassifier(TransTabModel):
     '''The classifier model subclass from :class:`transtab.modeling_transtab.TransTabModel`.
 
     Parameters
     ----------
     categorical_columns: list
```

### Comparing `transtab-0.0.3/transtab/trainer.py` & `transtab-0.0.4/transtab/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,19 @@
     def evaluate(self):
         # evaluate in each epoch
         self.model.eval()
         eval_res_list = []
         for dataindex in range(len(self.testloader_list)):
             y_test, pred_list, loss_list = [], [], []
             for data in self.testloader_list[dataindex]:
-                y_test.append(data[1])
+                if data[1] is not None:
+                    label = data[1]
+                    if isinstance(label, pd.Series):
+                        label = label.values
+                    y_test.append(label)
                 with torch.no_grad():
                     logits, loss = self.model(data[0], data[1])
                 if loss is not None:
                     loss_list.append(loss.item())
                 if logits is not None:
                     if logits.shape[-1] == 1: # binary classification
                         pred_list.append(logits.sigmoid().detach().cpu().numpy())
@@ -162,15 +166,15 @@
                 pred_all = np.concatenate(pred_list, 0)
                 if logits.shape[-1] == 1:
                     pred_all = pred_all.flatten()
 
             if self.args['eval_metric_name'] == 'val_loss':
                 eval_res = np.mean(loss_list)
             else:
-                y_test = pd.concat(y_test, 0)
+                y_test = np.concatenate(y_test, 0)
                 eval_res = self.args['eval_metric'](y_test, pred_all)
 
             eval_res_list.append(eval_res)
 
         return eval_res_list
 
     def train_no_dataloader(self,
```

### Comparing `transtab-0.0.3/transtab/trainer_utils.py` & `transtab-0.0.4/transtab/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `transtab-0.0.3/transtab/transtab.py` & `transtab-0.0.4/transtab/transtab.py`

 * *Files identical despite different names*

### Comparing `transtab-0.0.3/transtab.egg-info/PKG-INFO` & `transtab-0.0.4/transtab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transtab
-Version: 0.0.3
+Version: 0.0.4
 Summary: A flexible tabular prediction model that handles variable-column input tables.
 Home-page: https://github.com/RyanWangZf/transtab
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
 Keywords: tabular data,machine learning,data mining,data science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

