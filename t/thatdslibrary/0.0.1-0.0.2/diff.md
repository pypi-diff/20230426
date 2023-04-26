# Comparing `tmp/thatdslibrary-0.0.1.tar.gz` & `tmp/thatdslibrary-0.0.2.tar.gz`

## Comparing `thatdslibrary-0.0.1.tar` & `thatdslibrary-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/src/thatdslibrary/__init__.py
--rw-r--r--   0        0        0    13458 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/src/thatdslibrary/chart_plotting.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/src/thatdslibrary/data_preprocessing.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/src/thatdslibrary/hypo_testing.py
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/src/thatdslibrary/ml_helpers.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/LICENSE
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/README.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 thatdslibrary-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0  4835434 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/nbs/pima_indian_classification.ipynb
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/nbs/images/tree_depth_3_PID
+-rw-r--r--   0        0        0   155271 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/nbs/images/tree_depth_3_PID.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/src/thatdslibrary/__init__.py
+-rw-r--r--   0        0        0    13559 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/src/thatdslibrary/chart_plotting.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/src/thatdslibrary/data_preprocessing.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/src/thatdslibrary/hypo_testing.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/src/thatdslibrary/ml_helpers.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/LICENSE
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/README.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 thatdslibrary-0.0.2/PKG-INFO
```

### Comparing `thatdslibrary-0.0.1/src/thatdslibrary/chart_plotting.py` & `thatdslibrary-0.0.2/src/thatdslibrary/chart_plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from pathlib import Path
 import numpy as np
 from sklearn.metrics import confusion_matrix, ConfusionMatrixDisplay
 from sklearn.model_selection import learning_curve,validation_curve
 import matplotlib.pyplot as plt
 from sklearn.inspection import PartialDependenceDisplay, permutation_importance
 import pandas as pd
 import plotly.express as px
-from dtreeviz.trees import *
+import dtreeviz
 from sklearn.tree import export_graphviz
 import graphviz
 from matplotlib.cm import get_cmap
 import plotly.graph_objects as go
 
 def plot_learning_curve(
     estimator,
@@ -194,23 +195,27 @@
     scores = rs_df[f'mean_test_{scoring}'].values
     fig = px.scatter_3d(rs_df, x=f'param_{param1}', y=f'param_{param2}', z=f'param_{param3}',
                     color=f'mean_test_{scoring}',range_color=[scores.min(),scores.max()],
                        log_x = log_param1, log_y=log_param2, log_z=log_param3)
     fig.show()
 
 
-def plot_tree_dtreeviz(estimator,X,y,target_name,class_names,depth_range_to_display=None,fancy=False,new_window=False):
-    viz = dtreeviz(estimator,X,y,target_name=target_name,feature_names=X.columns.values,
-                   class_names=class_names,depth_range_to_display=depth_range_to_display,
-                  orientation='LR',instance_orientation='LR',fancy=fancy)
-    if new_window:
-        viz.view()
-    return viz
+def plot_tree_dtreeviz(estimator,X,y,target_name,class_names,tree_index=0,depth_range_to_display=None,fancy=False,scale=1.0):
+    viz = dtreeviz.model(estimator,X,y,tree_index=tree_index,target_name=target_name,
+                        feature_names=X.columns.values,
+                        class_names=class_names,
+                        )
+    # return viz
+    
+    return viz.view(depth_range_to_display=depth_range_to_display,
+         orientation='LR',
+         instance_orientation='LR',fancy=fancy,scale=scale)
+    
 
-def plot_tree_sklearn(estimator,feature_names,class_names,size=30,ratio=0.2,rotate=True,fname='tmp'):
+def plot_tree_sklearn(estimator,feature_names,class_names,rotate=True,fname='tmp'):
     s = export_graphviz(estimator,out_file=None,feature_names=feature_names,filled=True,class_names=class_names,
                        special_characters=True,rotate=rotate,rounded=True)
     graph = graphviz.Source(s,format='png')
     graph.render(Path('images')/fname)
 
 def plot_feature_importances(importances,col_names,figsize=(20,10),top_n=None):
     fea_imp_df = pd.DataFrame(data={'Feature':col_names,'Importance':importances}).set_index('Feature')
@@ -218,15 +223,15 @@
     if top_n is not None:
         fea_imp_df = fea_imp_df.head(top_n)
     fea_imp_df.plot(kind='barh',figsize=figsize)
     return fea_imp_df
 
 
 def plot_permutation_importances(best_model,X,y,scoring=['f1_macro'],n_repeats=10,seed=42,top_n=None,figsize=(20,10)):
-    r_multi = permutation_importance(best_model, X, y, n_repeats=n_repeats, random_state=42, scoring=scoring)
+    r_multi = permutation_importance(best_model, X, y, n_repeats=n_repeats, random_state=seed, scoring=scoring)
     fea_imp_dfs=[]
     for metric in r_multi.keys():
         print(f"{metric}")
         r = r_multi[metric]        
         fea_imp_df  = pd.DataFrame(data={'Feature':X.columns.values,'Importance':r['importances_mean'],'STD':r['importances_std']}).set_index('Feature')
         fea_imp_df = fea_imp_df.sort_values(['Importance'],ascending=True)
         if top_n is not None:
@@ -278,15 +283,15 @@
     fig.show()
     if save_name: fig.write_html(str(PATH/save_name)+ '.html')
 
     
 def pdp_numerical_only(best_model,df,num_features,y_class,y_colors=None,ncols=2,nrows=2,figsize=(20,16)):
     common_params = {
     "subsample": 40,
-    "n_jobs": 2,
+    "n_jobs": -1,
     "grid_resolution": 100,
     "random_state": 42,
     }
 
     features_info = {
         # features of interest
         "features": num_features,
@@ -357,15 +362,15 @@
         displays[i].plot(ax=axes[i],pdp_lim={1: (0, ymax)})
         axes[i].set_title(y_class[i])
     
 
 def plot_ice_pair(best_model,df,pair_features,class_idx,figsize=(10,4)):
     common_params = {
         "subsample": 40,
-        "n_jobs": 2,
+        "n_jobs": -1,
         "grid_resolution": 100,
         "random_state": 42,
     }
     fea_to_plot = pair_features
     features_info = {
         # features of interest
         "features": [fea_to_plot[0],fea_to_plot[1], fea_to_plot],
```

### Comparing `thatdslibrary-0.0.1/src/thatdslibrary/data_preprocessing.py` & `thatdslibrary-0.0.2/src/thatdslibrary/data_preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,15 @@
         fig,ax = plt.subplots(figsize=(10,10))
         dataplot = sns.heatmap(np.round(df.corr(),3), cmap="YlGnBu", annot=True)  
         # displaying heatmap
         plt.show()
 
     df_const = add_constant(df)    
     vif = pd.Series([variance_inflation_factor(df_const.values, i) 
-                    for i in range(df_const.shape[1])], 
-                index=df_const.columns)
-    print(vif)
+                    for i in range(df_const.shape[1])], index=df_const.columns)
     return vif
 
 
 ### preprocessing function ###
 def process_missing_values(X_train,X_test=None,miss_cols=[],missing_vals=np.NaN,strategy='median',**kwargs):
     if not len(miss_cols):
         return X_train,X_test
```

### Comparing `thatdslibrary-0.0.1/src/thatdslibrary/hypo_testing.py` & `thatdslibrary-0.0.2/src/thatdslibrary/hypo_testing.py`

 * *Files identical despite different names*

### Comparing `thatdslibrary-0.0.1/src/thatdslibrary/ml_helpers.py` & `thatdslibrary-0.0.2/src/thatdslibrary/ml_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,52 @@
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import GridSearchCV, RandomizedSearchCV, cross_validate, train_test_split
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import RandomForestClassifier,AdaBoostClassifier
 from sklearn.metrics import f1_score,accuracy_score,classification_report,log_loss
 import numpy as np
 import pandas as pd
-import statsmodels
-from chart_plotting import plot_confusion_matrix,plot_permutation_importances
+import statsmodels.api as sm
+from thatdslibrary.chart_plotting import plot_confusion_matrix,plot_permutation_importances
 
-def run_logistic_regression(df,y_col,multi_class='multinomial',solver='newton-cg',max_iter=10000):
-    # only for multinomial classification
-    y_true = df[y_col].values
-    df_trn = df.drop(y_col,axis=1)
-    model = LogisticRegression(random_state=0, multi_class=multi_class, penalty=None, solver=solver,max_iter=10000).fit(df_trn, y_true)
-    preds = model.predict(df_trn)
-    prob_preds = model.predict_proba(df_trn)
+def run_logistic_regression(X_trn,y_trn,multi_class='multinomial',solver='newton-cg',penalty=None,max_iter=10000):
+    model = LogisticRegression(random_state=0, multi_class=multi_class, 
+                               penalty=penalty, solver=solver,max_iter=max_iter).fit(X_trn, y_trn)
+    preds = model.predict(X_trn)
+    prob_preds = model.predict_proba(X_trn)
     print('-'*100)
     print('Intercept: \n', model.intercept_)
     print('Coefficients: \n', model.coef_)
     print('Coefficients exp :\n',np.exp(model.coef_))
 
     print('-'*100)
-    print('Log loss: ',log_loss(y_true,prob_preds))
+    print('Log loss: ',log_loss(y_trn,prob_preds))
     print('-'*100)
-    print(classification_report(y_true,preds))
-
-def run_multinomial_statmodel(df,y_col,add_constant=False):
-    y_trn = df[y_col].values
-    df_trn = df.drop(y_col,axis=1)
+    print(classification_report(y_trn,preds))
 
+def run_multinomial_statmodel(X_trn,y_trn,add_constant=False):
     if add_constant:
-        df_trn = statsmodels.api.add_constant(df_trn)
-    logit_model=statsmodels.api.MNLogit(y_trn,df_trn)
-    print(logit_model)
+        X_trn = sm.add_constant(X_trn)
+    logit_model=sm.MNLogit(y_trn,X_trn)
     result=logit_model.fit()
     stats1=result.summary()
     print(stats1)
     prob_preds = logit_model.predict(params = result.params.values)
     print('-'*100)
     print('Log loss: ',log_loss(y_trn,prob_preds))
     print('-'*100)
-    print(classification_report(y_trn,np.argmax(prob_preds,axis=1)+1))
+    print(classification_report(y_trn,np.argmax(prob_preds,axis=1)))
 
 
-def run_sklearn_classification_model(model_name,model_params,df,y_col,y_classes,val_ratio=0.2,seed=42,plot_fea_imp=True):
-    df = df.copy().reset_index(drop=True)
-    df_trn = df.drop(y_col,axis=1)
-    # trn_cols = df.drop(y_col,axis=1).columns.values
+def run_sklearn_classification_model(model_name,model_params,X_trn,y_trn,y_classes,val_ratio=0.2,seed=42,plot_fea_imp=True):
     np.random.seed(seed)
-    if val_ratio is None:
-        y_trn = df[y_col].values
-        X_trn = df_trn.values
-    else:
-        X_trn,X_test,y_trn,y_test = train_test_split(df_trn.values,df[y_col].values,test_size=val_ratio,random_state=seed)
+    if val_ratio is not None:
+        X_trn,X_test,y_trn,y_test = train_test_split(X_trn,y_trn,test_size=val_ratio,random_state=seed)
     
+
     if model_name=='DT':
         _model = DecisionTreeClassifier(random_state=seed,**model_params)
     elif model_name=='AdaBoost':
         dt_params={k.split('__')[1]:v for k,v in model_params.items() if 'base_estimator' in k}
         abc_params={k:v for k,v in model_params.items() if 'base_estimator' not in k}        
         print(f'Decision Tree params: {dt_params}')
         print(f'AdaBoost params: {abc_params}')
@@ -91,36 +80,32 @@
                            'Prediction Distribution':pd.Series(pred_val).value_counts(normalize=True).sort_index()}
                           )
         print(df2)
         plot_confusion_matrix(y_test,pred_val,y_classes)
     
     if plot_fea_imp:
         # plot_feature_importances(_model.feature_importances_,trn_df.columns.values)
-        _ = plot_permutation_importances(_model,df_trn,
-                                y_trn)
+        _ = plot_permutation_importances(_model,X_trn,y_trn)
     
     return _model,prob_trn
 
 
-def tune_sklearn_classification_model(model_name,param_grid,df,y_col,custom_cv=5,random_cv_iter=None,seed=42,rank_show=10):
-    y_trn = df[y_col].values
-    df_trn = df.drop(y_col,axis=1)
-
+def tune_sklearn_classification_model(model_name,param_grid,X_trn,y_trn,custom_cv=5,random_cv_iter=None,seed=42,rank_show=10):
     if model_name=='DT':
         _model = DecisionTreeClassifier(random_state=seed)
     elif model_name=='AdaBoost':
         dt = DecisionTreeClassifier(random_state=seed)
         _model = AdaBoostClassifier(base_estimator= dt,random_state=seed,algorithm='SAMME')
     elif model_name=='RF':
         _model = RandomForestClassifier(random_state=seed)
     else:
         print('Unsupported model')
         return
     
-    search_cv,default_cv = do_param_search(df_trn,y_trn,_model,param_grid,cv=custom_cv,scoring=['f1_macro','accuracy'],random_cv_iter = random_cv_iter,seed=seed)
+    search_cv,default_cv = do_param_search(X_trn,y_trn,_model,param_grid,cv=custom_cv,scoring=['f1_macro','accuracy'],random_cv_iter = random_cv_iter,seed=seed)
     show_both_cv(search_cv,default_cv,'f1_macro',rank_show)
     return search_cv
 
 
 ### hyperparam tuning
 
 def do_param_search(
```

### Comparing `thatdslibrary-0.0.1/LICENSE` & `thatdslibrary-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thatdslibrary-0.0.1/pyproject.toml` & `thatdslibrary-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thatdslibrary"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Quan Tran", email="quan.tran1@outlook.com" },
 ]
 description = "A useful package for EDA and quick ML model finetuning"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
@@ -21,15 +21,14 @@
 dependencies = [
         "numpy>=1.23.0",
         "scikit-learn>=1.2.0",
         "matplotlib>=3.7.0",
         "pandas>=1.5.0",
         "plotly>=5.14.0",
         "dtreeviz>=2.2",
-        "graphviz>=0.20",
         "seaborn>=0.12.0",
         "statsmodels>=0.13.0",
         "pingouin>=0.5.3",
     ]
 
 [project.urls]
 "Homepage" = "https://github.com/anhquan0412/that_ds_library"
```

### Comparing `thatdslibrary-0.0.1/PKG-INFO` & `thatdslibrary-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thatdslibrary
-Version: 0.0.1
+Version: 0.0.2
 Summary: A useful package for EDA and quick ML model finetuning
 Project-URL: Homepage, https://github.com/anhquan0412/that_ds_library
 Project-URL: Bug Tracker, https://github.com/anhquan0412/that_ds_library/issues
 Author-email: Quan Tran <quan.tran1@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Quan Tran
@@ -29,15 +29,14 @@
 License-File: LICENSE
 Keywords: auto finetuning,automation,finetune,machine learning,sklearn
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: dtreeviz>=2.2
-Requires-Dist: graphviz>=0.20
 Requires-Dist: matplotlib>=3.7.0
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: pingouin>=0.5.3
 Requires-Dist: plotly>=5.14.0
 Requires-Dist: scikit-learn>=1.2.0
 Requires-Dist: seaborn>=0.12.0
```

