# Comparing `tmp/probabilistic_word_embeddings-1.1.1.tar.gz` & `tmp/probabilistic_word_embeddings-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_word_embeddings-1.1.1.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.2.0.tar", max compression
```

## Comparing `probabilistic_word_embeddings-1.1.1.tar` & `probabilistic_word_embeddings-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      380 2023-03-23 10:38:19.773147 probabilistic_word_embeddings-1.1.1/README.md
--rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     7424 2023-04-03 10:42:26.292889 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0     9400 2023-04-04 13:40:34.971850 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0     9826 2023-04-17 09:54:17.143703 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3551 2023-03-28 11:37:58.307437 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     4915 2023-04-17 07:32:28.780974 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     3492 2023-03-23 10:38:08.130487 probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      567 2023-04-17 10:16:47.310751 probabilistic_word_embeddings-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.1.1/setup.py
--rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7424 2023-04-25 13:31:30.609859 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0     9733 2023-04-25 14:14:16.286882 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0     9826 2023-04-25 13:31:30.614433 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     4915 2023-04-25 13:31:30.615879 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     3492 2023-04-25 13:31:30.616555 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      473 2023-04-25 14:20:07.081905 probabilistic_word_embeddings-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.0/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.0/PKG-INFO
```

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/estimation.py` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                         print(f"Epoch {epoch} mean training loss after {batch_no} batches: {np.mean(epoch_training_loss)}")
 
     if early_stopping and valid_data is not None and best_valid_weights is not None:
         print("Assign the weights corresponding to the best validation loss")
         embedding.theta.assign(best_valid_weights)
     return embedding
 
-def mean_field_vi(embedding, data, model="cbow", ws=5, ns=5, batch_size=25000, epochs=5, evaluate=True, valid_data=None):
+def mean_field_vi(embedding, data, model="cbow", ws=5, ns=5, batch_size=25000, epochs=5, evaluate=True, valid_data=None, elbo_history=False):
     if not isinstance(embedding, Embedding):
         warnings.warn("embedding is not a subclass of probabilistic_word_embeddings.Embedding")
     if model not in ["sgns", "cbow"]:
         raise ValueError("model must be 'sgns' or 'cbow'")
 
     if not isinstance(data, tf.Tensor):
         data = tf.constant(data)
@@ -153,56 +153,61 @@
     q_mean = tf.Variable(tf.random.normal(e.theta.shape, dtype=tf.float64)* 0.00001)
     q_std_log =  tf.Variable(tf.random.normal(e.theta.shape, dtype=tf.float64)* 0.00001 - 3.0)
     
     opt_mean_var = optimizer.add_variable_from_reference(q_mean, "q_mean", initial_value=q_mean)
     opt_std_var = optimizer.add_variable_from_reference(q_std_log, "q_std_log", initial_value=q_std_log)
     optimizer.build([opt_mean_var, opt_std_var])
 
-    
+    elbo_history = []
     for epoch in range(epochs):
         print(f"Epoch {epoch}")
         # Shuffle the order of batches
         if evaluate:
             similarity = evaluate_word_similarity(embedding)
             print(similarity)
 
+        epoch_logprobs = []
         for batch in progressbar.progressbar(random.sample(range(batches),batches)):
             # Reparametrization trick, Q = mu + sigma * epsilon
             epsilon = tf.random.normal(q_std_log.shape, dtype=tf.float64)
             z = q_mean + tf.multiply(tf.math.exp(q_std_log), epsilon)
             embedding.theta.assign(z)
             
             start_ix = batch_size * batch
             i,j,x  = generate_batch(data, model=model, ws=ws, ns=ns, batch_size=batch_size, start_ix=start_ix)
 
             with tf.GradientTape() as tape:
                 if model == "cbow":
                     log_prob = tf.reduce_sum(cbow_likelihood(e, i, j, x=x)) + e.log_prob(batch_size, N)
                 elif model == "sgns":
                     log_prob = tf.reduce_sum(sgns_likelihood(e, i, j, x=x)) + e.log_prob(batch_size, N)
+                epoch_logprobs.append(log_prob)
                 d_l_d_theta = -tape.gradient(log_prob, embedding.theta) * N / batch_size
             
             d_l_d_q_mean = d_l_d_theta
             d_l_q_std_log = tf.multiply(tf.multiply(d_l_d_theta, epsilon), tf.math.exp(q_std_log))
 
             # Add the entropy term
             d_l_q_std_log = d_l_q_std_log - tf.ones(d_l_q_std_log.shape, dtype=tf.float64)
 
             optimizer.update_step(d_l_d_q_mean, opt_mean_var)
             optimizer.update_step(d_l_q_std_log, opt_std_var)
-            print(opt_mean_var)
-            print(opt_std_var)
             
             q_mean.assign(opt_mean_var)
             q_std_log.assign(opt_std_var)
 
-            
+        epoch_entropy = tf.reduce_sum(opt_std_var)
+        epoch_elbo = tf.reduce_mean(epoch_logprobs) + epoch_entropy
+        print(f"Epoch ELBO: {epoch_elbo.numpy()}")
         embedding.theta.assign(opt_mean_var)
+        elbo_history.append(epoch_elbo.numpy())
 
     embedding_q_mean = embedding
+    if elbo_history:
+        return embedding_q_mean, q_std_log, elbo_history
     return embedding_q_mean, q_std_log
```

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/evaluation.py` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/evaluation.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/models.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/preprocessing.py` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/preprocessing.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.1.1/probabilistic_word_embeddings/utils.py` & `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/utils.py`

 * *Files identical despite different names*

