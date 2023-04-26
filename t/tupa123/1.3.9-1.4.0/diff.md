# Comparing `tmp/tupa123-1.3.9.tar.gz` & `tmp/tupa123-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.3.9.tar", last modified: Tue Apr 18 13:59:36 2023, max compression
+gzip compressed data, was "tupa123-1.4.0.tar", last modified: Wed Apr 26 19:22:20 2023, max compression
```

## Comparing `tupa123-1.3.9.tar` & `tupa123-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:59:36.358947 tupa123-1.3.9/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.3.9/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-04-18 13:59:36.357591 tupa123-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.3.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-18 13:59:36.358947 tupa123-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-18 13:54:58.000000 tupa123-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:59:36.346616 tupa123-1.3.9/tupa123/
--rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.3.9/tupa123/__init__.py
--rw-rw-rw-   0        0        0    59976 2023-04-17 20:49:14.000000 tupa123-1.3.9/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:59:36.355558 tupa123-1.3.9/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 13:59:36.000000 tupa123-1.3.9/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 19:22:20.012606 tupa123-1.4.0/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-04-26 19:22:20.012606 tupa123-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 19:22:20.012606 tupa123-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-26 19:21:23.000000 tupa123-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:22:19.996984 tupa123-1.4.0/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-03-27 17:38:15.000000 tupa123-1.4.0/tupa123/__init__.py
+-rw-rw-rw-   0        0        0    67785 2023-04-26 19:06:25.000000 tupa123-1.4.0/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:22:20.012606 tupa123-1.4.0/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 19:22:19.000000 tupa123-1.4.0/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.3.9/LICENSE.txt` & `tupa123-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.9/PKG-INFO` & `tupa123-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.9
+Version: 1.4.0
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.3.9/README.md` & `tupa123-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.3.9/setup.py` & `tupa123-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.3.9',
+    version='1.4.0',
     license = 'MIT',
     license_files=('LICENSE.txt',),    
     packages=['tupa123'],
     install_requires=['numpy','matplotlib','pandas'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
     description= 'fully connected neural network with four layers',
```

### Comparing `tupa123-1.3.9/tupa123/tupa123.py` & `tupa123-1.4.0/tupa123/tupa123.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,86 +3,100 @@
 import numpy as np 
 import time
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 
 
 
-
-
-
+###############################################################
+###############################################################
+#########  Auxliar function interface excel  ##################
+###############################################################
+###############################################################
 
 #load data from an excel spreadsheet
 def ExcelMatrix(namearq, namesheet, Lineini, Columini, columnquantity, linesquantity):
     print('Loading data...')
     df = pd.read_excel(namearq, sheet_name=namesheet, header=None)
     Matriz = df.iloc[Lineini-1:Lineini+linesquantity-1, Columini-1:Columini+columnquantity-1].values.astype(np.float64)
     print('Loading data = ok')
     return Matriz
 
 
 
-
+###############################################################
+###############################################################
+#########  Auxliar function to statistics   ###################
+###############################################################
+###############################################################
 
 
 
 #Make basic comparative statistics between two sets of data
 def Statistics(Calculated, Targeted):
     
     numdata,numevar = Calculated.shape
     
     print('------------------------')
     print ('Statistics between predictor variables and target variables:')
     print('------------------------')
+    print('')
       
     for j in range(0,numevar):
         
         erroari = Calculated[:,j] - Targeted[:,j]
         erroper = ( ( Calculated[:,j] - Targeted[:,j] ) / (Targeted[:,j] + 1e-7)  )*100
         coefcorrelacao = np.corrcoef(Targeted[:,j], Calculated[:,j])[1][0]
         
-        print ('Correlation coefficient, variable ' + str(j+1) +' = ' + str(coefcorrelacao))
+        print ('Correlation coefficient between Calculated and Target, variable ' + str(j+1) +' = ' + str(coefcorrelacao))
+        print('')
+        print('----- About error = Calculated - Target --------')
         print('')
         print ('Mean difference, variable ' + str(j+1) +' = ' + str(np.mean(erroari)) + ' (' + str(np.mean(erroper)) + '%)')
         print('')
         print ('Standard deviation, variable ' + str(j+1) +' = ' + str(np.std(erroari)) + ' (' + str(np.std(erroper)) + '%)')
         print('')
         print ('Biggest absolute point difference, variable ' + str(j+1) +' = ' + str(np.max(abs(erroari))) + ' ('  + str(np.max(abs(erroper))) + '%)' )
         print('')
 
         conta=0
         for i in range(0,numdata):
             if abs(erroari[i]) <= 0.1:
                 conta=conta+1
         result = 100*conta/numdata
-        print('For classification 0 to 1, number of hits for a maximum difference of 10% = ' + str(result) + '%' )
-
-        print('------------------------')
-
+        print('------ Only for classification 0 or 1 -----')
+        print('')
+        print('Number of hits for a maximum difference of 10% = ' + str(result) + '%' )
+        print('')
 
 
 
+###############################################################
+###############################################################
+#########  Auxliar function to graphs   #######################
+###############################################################
+###############################################################
 
 
 
 #Plot two variables ifferences in a sequential series
 def PlotComparative(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
 
     for j in range(0,numevar):    
         eixoY1= Targeted[:,j]
         eixoY2= Calculated[:,j]
     
         plt.figure(figsize=(12, 5))
-        plt.title('Comparison chart calculated variable vs targeted')
+        plt.title('Comparison calculated variable vs target')
         plt.xlabel('Sequence of events')
         plt.ylabel('Target and predicted variable ' + str(j+1))
-        plt.plot(eixoX, eixoY1, marker = '', label='Targeted')  
+        plt.plot(eixoX, eixoY1, marker = '', label='Target')  
         plt.plot(eixoX, eixoY2, marker = '', label='Calculated')
         #plt.plot(eixoX, eixoY2, c='black', marker = '.', label='Calculated', alpha=0.33)
         plt.legend(loc = "upper left")
         plt.show()
 
 
 
@@ -102,18 +116,18 @@
         
         eixoY3 = eixoY2 - eixoY1
 
         # preparação para a média móvel
         rolling_mean = pd.Series(eixoY3).rolling(window_size).mean()
 
         plt.figure(figsize=(12, 5))
-        plt.title('Comparison chart calculated variable vs targeted')
+        plt.title('Comparison calculated variable vs target')
         plt.xlabel('Sequence of events')
-        plt.ylabel('Error, Calculated - Targeted ' + str(j+1))
-        plt.plot(eixoX, eixoY3, marker = '', color = 'darkblue', label='Targeted')
+        plt.ylabel('Error, Calculated - Target ' + str(j+1))
+        plt.plot(eixoX, eixoY3, marker = '', color = 'darkblue', label='Target')
         # plota a med movel
         plt.plot(eixoX, rolling_mean, marker='', color = mcolors.to_hex((1, 0, 0)), label='Rolling mean', linestyle='dashed') 
 
         plt.legend(loc = "upper left")
         plt.show()
 
 
@@ -133,28 +147,28 @@
         eixoY2= Calculated[:,j]
 
         # Cálculo do erro médio e desvio padrão
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
     
         plt.figure(figsize=(12, 5))
-        plt.title('Comparison chart calculated variable vs targeted')
+        plt.title('Calculated variable vs target, sigmas range about error = calculated-target')
         plt.xlabel('Sequence of events')
         plt.ylabel('Target and predicted variable ' + str(j+1))
-        plt.plot(eixoX, eixoY1, marker = '',  label='Targeted')  
+        plt.plot(eixoX, eixoY1, marker = '',  label='Target')  
         plt.plot(eixoX, eixoY2, linestyle='none', c='black', marker = '.', label='Calculated', alpha=0.33)
         plt.legend(loc = "upper right")
 
         # Preenchendo a área entre as curvas
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - sigma, eixoY1 + erro_medio + sigma, color='gray', alpha=0.3)
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 2*sigma, eixoY1 + erro_medio + 2*sigma, color='gray', alpha=0.2)
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 3*sigma, eixoY1 + erro_medio + 3*sigma, color='gray', alpha=0.1)
 
         # Adicionando o valor do desvio padrão ao canto superior esquerdo do gráfico
-        plt.text(0.025, 0.95, "sigma = {:.2f}".format(sigma) + ", average = {:.2f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
+        plt.text(0.025, 0.95, "sigma = {:.3f}".format(sigma) + ", average = {:.3f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
         
         plt.show()
 
 
 
 
 
@@ -172,49 +186,89 @@
         eixoY2= Calculated[:,j]
 
         # Cálculo do erro médio e desvio padrão
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
     
         plt.figure(figsize=(12, 5))
-        plt.title('Comparison chart calculated variable vs targeted')
+        plt.title('Calculated variable vs target, sigmas range about error = calculated-target')
         plt.xlabel('Sequence of events')
         plt.ylabel('Target and predicted variable ' + str(j+1))
-        plt.plot(eixoX, eixoY1, marker = '',  label='Targeted')
+        plt.plot(eixoX, eixoY1, marker = '',  label='Target')
 
         plt.plot(eixoX, eixoY1 + erro_medio - 2*sigma, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected minimum, -2S')
         plt.plot(eixoX, eixoY1 + erro_medio + 2*sigma, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected maximum, +2S')
         plt.fill_between(np.arange(len(eixoY1)), eixoY1 + erro_medio - 2*sigma, eixoY1 + erro_medio + 2*sigma, color='gray', alpha=0.1)
                 
         #plt.plot(eixoX, eixoY2, linestyle='none', c='black', marker = '.', label='Calculated', alpha=0.33)
         plt.legend(loc = "upper right")
 
         # Adicionando o valor do desvio padrão ao canto superior esquerdo do gráfico
-        plt.text(0.025, 0.95, "sigma = {:.2f}".format(sigma) + ", average = {:.2f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
+        plt.text(0.025, 0.95, "sigma = {:.3f}".format(sigma) + ", average = {:.3f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
         
         plt.show()
 
 
         
 
 
 
+
+
+#Plot 2 sigma lines of proportion
+def PlotComparative5(Calculated, Targeted):
+
+    numdata,numevar = Calculated.shape
+    eixoX = np.arange(0, numdata, dtype=int)
+
+    for j in range(0,numevar):    
+        eixoY1= Targeted[:,j]
+        eixoY2= Calculated[:,j]
+
+        # Cálculo do erro médio e desvio padrão
+        erro_medio = np.mean(eixoY2 / eixoY1)
+        sigma = np.std(eixoY2 / eixoY1)
+    
+        plt.figure(figsize=(12, 5))
+        plt.title('Calculated variable vs target, sigmas range about proportional error = calculated/target')
+        plt.xlabel('Sequence of events')
+        plt.ylabel('Target and predicted variable ' + str(j+1))
+        plt.plot(eixoX, eixoY1, marker = '',  label='Target')
+
+        plt.plot(eixoX, eixoY1*erro_medio - 2*sigma*eixoY1, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected minimum, -2S')
+        plt.plot(eixoX, eixoY1*erro_medio + 2*sigma*eixoY1, marker = '', c='black', alpha=0.5, linestyle='dashed', label='Expected maximum, +2S')
+        plt.fill_between(np.arange(len(eixoY1)),eixoY1*erro_medio - 2*sigma*eixoY1, eixoY1*erro_medio + 2*sigma*eixoY1, color='gray', alpha=0.1)
+                
+        #plt.plot(eixoX, eixoY2, linestyle='none', c='black', marker = '.', label='Calculated', alpha=0.33)
+        plt.legend(loc = "upper right")
+
+        # Adicionando o valor do desvio padrão ao canto superior esquerdo do gráfico
+        plt.text(0.025, 0.95, "sigma = {:.3f}".format(sigma) + ", average = {:.3f}".format(erro_medio), transform=plt.gca().transAxes, fontsize=12, verticalalignment='top')
+        
+        plt.show()
+
+
+
+
+
+
+
 #Plot correlation between calculated variables and objectives
 def PlotCorrelation(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
 
     for j in range(0,numevar):    
         eixoY1= Targeted[:,j]
         eixoY2= Calculated[:,j]        
         coefcorrelacao = np.corrcoef(eixoY1,eixoY2)[1][0]
         plt.title('Correlation coefficient variable '+ str(j+1)+' = ' + str(coefcorrelacao))
         plt.scatter(eixoY1,eixoY2,color='blue',s=15,edgecolor='red') #grafico de correlação entre as variaveis procuradas e alvo---
-        plt.xlabel('Targeted')
+        plt.xlabel('Target')
         plt.ylabel('Calculated')    
         plt.show()
 
 
 
 
 
@@ -233,15 +287,15 @@
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
         valormax = np.max(eixoY1)
         valormin = np.min(eixoY1)
         
         plt.title('Correlation coefficient variable '+ str(j+1)+' = ' + str(coefcorrelacao))
         plt.scatter(eixoY1,eixoY2,color='blue',s=15,edgecolor='red') #grafico de correlação entre as variaveis procuradas e alvo---
-        plt.xlabel('Targeted')
+        plt.xlabel('Target')
         plt.ylabel('Calculated')    
 
         plt.plot([valormin,valormax], [valormin,valormax], color='black', alpha=0.9)
         
         plt.plot([valormin,valormax], [valormin+erro_medio-sigma,valormax+erro_medio-sigma], color='red', linestyle='dashed', alpha=0.5)
         plt.plot([valormin,valormax], [valormin+erro_medio+sigma,valormax+erro_medio+sigma], color='red', linestyle='dashed', alpha=0.5)
         
@@ -257,14 +311,17 @@
 
 
 
 
 
 
 
+
+
+
 #Plota o erro em relação ao alvo,que é o centro do grafico
 def PlotDispe(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
 
     for j in range(0,numevar):    
@@ -289,62 +346,100 @@
         # Preenchendo a área entre as curvas
         plt.fill_between((-1,1), erro_medio - sigma, erro_medio + sigma, color='gray', alpha=0.3)
         plt.fill_between((-1,1), erro_medio - 2*sigma, erro_medio + 2*sigma, color='gray', alpha=0.2)
         plt.fill_between((-1,1), erro_medio - 3*sigma, erro_medio + 3*sigma, color='gray', alpha=0.1)
         
         plt.title('Dispersion plot, 3 sigma gray gradients, variable '+ str(j+1))
         plt.xlabel('Variable normalized: -1,1')
-        plt.ylabel('Variable error (calculated-targeted)')
+        plt.ylabel('Variable error = calculated-target')
         
         plt.show()
 
+
+
+
+
+
+
+#Plota o erro em relação ao alvo,que é o centro do grafico
+def PlotDispe2(Calculated, Targeted):
+
+    numdata,numevar = Calculated.shape
+    eixoX = np.arange(0, numdata, dtype=int)
+
+    for j in range(0,numevar):    
+        eixoY1 = Targeted[:,j]
+        eixoY2 = Calculated[:,j]
         
+        erro = eixoY2 / eixoY1        
+        erro_medio = np.mean(eixoY2 / eixoY1)
+        sigma = np.std(eixoY2 / eixoY1)
 
+        valormax = np.max(eixoY1)
+        valormin = np.min(eixoY1)
+        volormed =(valormin+valormax)/2
+        eixoY1norma = (eixoY1 - volormed)/(valormax - volormed)
+        
+        plt.figure(figsize=(15, 5))
+        
+        plt.scatter(eixoY1norma, erro ,color='blue', s=15, edgecolor='red')
+        
+        plt.plot([-1,1], [1,1], color='black', alpha=0.9, linestyle='dashed')                
+
+        # Preenchendo a área entre as curvas
+        plt.fill_between((-1,1), erro_medio - sigma, erro_medio + sigma, color='gray', alpha=0.3)
+        plt.fill_between((-1,1), erro_medio - 2*sigma, erro_medio + 2*sigma, color='gray', alpha=0.2)
+        plt.fill_between((-1,1), erro_medio - 3*sigma, erro_medio + 3*sigma, color='gray', alpha=0.1) 
+        
+        
+        plt.title('Dispersion plot, 3 sigma gray gradients, variable '+ str(j+1))
+        plt.xlabel('Variable normalized: -1,1')
+        plt.ylabel('Variable proportional error = calculated/target')
+        
+        plt.show()
 
 
 
 
 
 
 #Plota o erro em relação ao alvo,que é o centro do grafico
-def PlotDispe2(Calculated, Targeted):
+def PlotDispe3(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
     eixoX = np.arange(0, numdata, dtype=int)
 
     for j in range(0,numevar):    
         eixoY1 = Targeted[:,j]
         eixoY2 = Calculated[:,j]
 
         razao=  eixoY2/eixoY1
         
         eixoY3 = eixoY2 - eixoY1        
         erro_medio = np.mean(eixoY2 - eixoY1)
         sigma = np.std(eixoY2 - eixoY1)
-        eixoY4 = eixoY3/sigma
-        
-                        
-        plt.title('Target vs sniper, variable '+ str(j+1))
+        eixoY4 = (erro_medio/sigma) + eixoY3/sigma
+                                
+        plt.title('Accuracy Trend Graph, variable '+ str(j+1))
         plt.scatter(eixoY4,razao,color='red', s=15 , marker = '.', alpha=0.1) #grafico de correlação entre as variaveis procuradas e alvo---
         plt.xlabel('Standard deviation sigma')
-        plt.ylabel('Proportion = calculated/targeted')
+        plt.ylabel('Proportion error = calculated/target')
 
         plt.plot([-1,1], [1,1], color='black', alpha=0.9, linestyle='dashed')
         plt.plot([0,0], [1-(np.max(razao)-1)*0.5,1+(np.max(razao)-1)*0.5], color='black', alpha=0.9, linestyle='dashed')
         
         plt.show()
 
 
 
 
 
 
 
 
-
 #Plota histograma do erro %
 def PlotHisto(Calculated, Targeted):
 
     numdata,numevar = Calculated.shape
 
     for j in range(0,numevar):    
         eixoY1= Targeted[:,j]
@@ -353,15 +448,15 @@
         eixoY3 = eixoY2 - eixoY1 #erro
 
         fig, ax = plt.subplots()
         
         desviopad = np.std(eixoY3) #devio padrão do erro
         erromedio = np.mean(eixoY3) #erro medio
         
-        textstr = '\n'.join((r'$\mathrm{average}=%.2f$' % (erromedio, ),r'$\sigma=%.2f$' % (desviopad, )))
+        textstr = '\n'.join((r'$\mathrm{average}=%.3f$' % (erromedio, ),r'$\sigma=%.3f$' % (desviopad, )))
 
         ax.hist(eixoY3, bins=20, rwidth=0.9, color='blue', alpha=0.7, edgecolor='black')
         # these are matplotlib.patch.Patch properties
         props = dict(boxstyle='round', facecolor='wheat', alpha=0.5)
 
         # place a text box in upper left in axes coords
         ax.text(0.05, 0.95, textstr, transform=ax.transAxes, fontsize=14, verticalalignment='top', bbox=props)
@@ -371,22 +466,27 @@
         plt.ylabel('Frequency', fontsize=12)
 
         plt.show()
 
 
 
 
+###############################################################
+###############################################################
+#########  Neural network   ###################################
+###############################################################
+###############################################################
 
 
 
 #Neural network 4 layers--------------------------------------------------------------------------------------------------------------------
 class nnet4:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1):
+    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.nn4c=nn4c
         self.rate=rate
         self.epochs=epochs
@@ -396,16 +496,26 @@
         self.norma=norma
         self.coef=coef
         self.normout=normout
         self.cost=cost
         self.regu=regu
         self.namenet=namenet
         self.shift=shift
+        self.iteconv=iteconv
+        self.conv=conv
+        self.sbw=sbw
+        self.c1=c1 
+
 
 
+###############################################################
+###############################################################
+#########  Auxliar function to normalization   ################
+###############################################################
+###############################################################
 
 
 
     #data normalization by calculating maximums and minimums-----------------------------------------------
     def Normalize(self, data, maxiname, mininame, medianame, desvioname):          
 
         #=-1, standardization
@@ -436,34 +546,34 @@
             
         if (self.norma==2) or (self.norma==5):    
             normalized = (data - vetormed) / (vetormax - vetormed)
 
         if (self.norma==6) or (self.norma==-1):
             normalized = (data - media)/desvio
 
-        np.savetxt(maxiname, vetormax)
-        np.savetxt(mininame, vetormin)
-        np.savetxt(medianame, media)
-        np.savetxt(desvioname, desvio)
+        np.save(maxiname, vetormax)
+        np.save(mininame, vetormin)
+        np.save(medianame, media)
+        np.save(desvioname, desvio)
         
         return normalized
 
 
 
 
 
 
     #normalizing the data by entering maximums and minimums-----------------------------------------------
     def Normalize2(self, data, maxiname, mininame, medianame, desvioname):         
 
-        vetormax = np.loadtxt(maxiname) 
-        vetormin = np.loadtxt(mininame) 
+        vetormax = np.load(maxiname) 
+        vetormin = np.load(mininame) 
         vetormed = (vetormax+vetormin)/2
-        media = np.loadtxt(medianame)
-        desvio = np.loadtxt(desvioname)  
+        media = np.load(medianame)
+        desvio = np.load(desvioname)  
 
         if (self.norma>=3): 
             data = np.log(data + self.coef)
         normalized = data*1
                                                 
         if (self.norma==1) or (self.norma==4):  
             normalized = (data - vetormin) / (vetormax - vetormin)
@@ -481,19 +591,19 @@
 
 
 
 
     #data denormalization-------------------------------------------------------------------
     def DesNormalize(self, normalized, maxiname, mininame, medianame, desvioname):         
 
-        vetormax = np.loadtxt(maxiname) 
-        vetormin = np.loadtxt(mininame) 
+        vetormax = np.load(maxiname) 
+        vetormin = np.load(mininame) 
         vetormed = (vetormax+vetormin)/2
-        media = np.loadtxt(medianame)
-        desvio = np.loadtxt(desvioname) 
+        media = np.load(medianame)
+        desvio = np.load(desvioname) 
         
         desnorma = normalized*1
                             
         if (self.norma==1) or (self.norma==4):  
             desnorma = normalized * (vetormax - vetormin) + vetormin
             
         if (self.norma==2) or (self.norma==5):  
@@ -506,15 +616,19 @@
             desnorma = np.exp(desnorma) - self.coef
                                
         return desnorma
 
 
 
 
-
+###############################################################
+###############################################################
+################ Activation functions   #######################
+###############################################################
+###############################################################
 
 
 
     #Definition of activation functions---------------------------------------------------------
     def Activation(self, typee, x):
 
         if (typee==0): #linear (-inf,inf)
@@ -538,15 +652,15 @@
             return y
 
         if (typee==5): #tanh (-1,1)
             y = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             return y
 
         if (typee==6): #LReLU (-inf,inf)
-            y=np.where(x < 0, x*0.5, x)
+            y=np.where(x <= 0, x*0.01, x)
             return y
         
         if (typee==7): #arctan (-inf, inf)
             y = np.arctan(x)
             return y
 
         if (typee==8): #exp (-inf, inf)
@@ -565,28 +679,33 @@
             y=np.where(x >= 0, x, np.exp(x)-1)
             return y
       
         if (typee==12): #logsigmoide (0,1)
             y = np.log( 1/(1+np.exp(-x)) )
             return y
 
-        if (typee==13): #x^2 (inf,inf)
-            y = x*x
+        if (typee==13): #x^n (inf,inf)
+            y = x**self.c1
             return y
 
-        if (typee==14): #x^3 (inf,inf)
-            y = x*x*x
+        if (typee==14): #ELU (-1,inf)
+            y=np.where(x <= 0, 1e-8 + 0.1*(np.exp(x)-1), x)
             return y
 
-        if (typee==15): # Simetric Rectified Linear (inf,inf)
-            y2 = np.where(x > 1, x*0.25, x)
-            y = np.where(y2 < -1, y2*0.25, y2)
+        if (typee==15): # GoldRelU (inf,inf)
+            y = np.where(x > 0, x*1.61803398, x*0.61803398)
             return y
 
+        if (typee==16): # Metallic mean (inf,inf)
+            y = (x + (x**2 + 4)**0.5)/2
+            return y
 
+        if (typee==17): #NoiseReLU (0,inf)            
+            y=np.where(x < 1e-8, 1e-8, x + np.random.normal(0,0.1) )
+            return y
 
 
     def DeActivation(self, typee,x):
 
         if (typee==0): #linear (-inf,inf)
             y = 1
             return y    
@@ -610,15 +729,15 @@
 
         if (typee==5): #tanh (-1,1)
             w = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             y = 1 - w**2
             return y
     
         if (typee==6): #LReLU (-inf,inf)
-            y=np.where(x < 0, 0.5, 1)        
+            y=np.where(x <= 0, 0.01, 1)        
             return y
     
         if (typee==7): #arctan (-inf, inf)
             y = 1/(1+x**2)
             return y
 
         if (typee==8): #exp (-inf, inf)
@@ -626,47 +745,56 @@
             return y
 
         if (typee==9): #seno (-inf, inf)
             y = np.cos(x)
             return y  
 
         if (typee==10): #swish (0, inf)
-            y = (x/(1+np.exp(-x))) + (1/(1+np.exp(-x)))*(1 - (x/(1+np.exp(-x))) )         
+            y = (x/(1+np.exp(-x))) + (1/(1+np.exp(-x)))*(1 - (x/(1+np.exp(-x))) )
             return y
 
         if (typee==11): #selu (-1, inf)
             y = np.where(x >= 0, 1, np.exp(x))        
             return y        
 
         if (typee==12): #logsigmoide (0,1)
             y = np.exp(-x)/(1+np.exp(-x))
             return y
 
-        if (typee==13): #x^2 (inf,inf)
-            y = 2*x
+        if (typee==13): #x^n (inf,inf)
+            y = self.c1*(x**(self.c1-1))
             return y
 
-        if (typee==14): #x^3 (inf,inf)
-            y = 3*x*x
+        if (typee==14): #ELU (inf,inf)
+            y=np.where(x <= 0, 0.1*np.exp(x), 1)
             return y
 
-        if (typee==15): # Simetric Rectified Linear (inf,inf)
-            y2 = np.where(x > 1, 0.25, 1)
-            y = np.where(y2 < -1, 0.25, 1)
+        if (typee==15): # GoldRelU (inf,inf)
+            y = np.where(x > 0, 1.61803398, 0.61803398)
             return y
 
+        if (typee==16): # Metallic mean (inf,inf)
+            y = 0.5*((x/((x**2 + 4)**0.5))+1)            
+            return y
 
+        if (typee==17): #RandReLU (0,inf)
+            y=np.where(x < 1e-8, 1e-8, 1)
+            return y
 
 
-
-
+###############################################################
+###############################################################
+################ Machine learning   ###########################
+###############################################################
+###############################################################
+        
 
     #machine learning,  single batch with ADAM accelerator-----------------------------------------------------
-    def Fit_ADAM(self, matX, matY):
-
+    def Fit_ADAM(self, matX, matY, matX2=[0], matY2=[0]):
+        
         tinicio = time.time()
         
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
         P23 = np.zeros((self.nn2c,self.nn3c))
@@ -747,128 +875,138 @@
             if not os.path.exists(self.namenet):
                 os.mkdir(self.namenet)
 
 
 
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
     
-            if self.nn1c ==1: #garante o formato matricial 
-                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
-            else:
-                P12 = np.loadtxt(nomepasta + "P12.txt")
-
-            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P12 = P12aux.T
-            
-            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
-                P23 = P23aux.T
-            else:
-                P23 = np.loadtxt(nomepasta + "P23.txt") 
-            
-            if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
-                P34 = P34aux.T
-            else:
-                P34 = np.loadtxt(nomepasta + "P34.txt")              
-
-            if self.nn2c ==1: #garante o formato matricial 
-                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
-            else:
-                B2 = np.loadtxt(nomepasta + "B2.txt")
-                
-            if self.nn3c ==1: #garante o formato matricial 
-                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
-            else:
-                B3 = np.loadtxt(nomepasta + "B3.txt")
-                
-            if self.nn4c ==1: #garante o formato matricial 
-                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
-            else:
-                B4 = np.loadtxt(nomepasta + "B4.txt")  
+            P12 = np.load(nomepasta + "P12.npy")
+            P23 = np.load(nomepasta + "P23.npy")            
+            P34 = np.load(nomepasta + "P34.npy")             
+            B2 = np.load(nomepasta + "B2.npy")
+            B3 = np.load(nomepasta + "B3.npy")
+            B4 = np.load(nomepasta + "B4.npy")  
 
         except: #Inicializa randomicamente-------------------------------
 
             B2 = -0.1 + 2*0.1*(np.random.rand(self.nn2c))
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))
             B4 = -0.1 + 2*0.1*(np.random.rand(self.nn4c))    
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
-        matX = self.Normalize(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt")
+        matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
         if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.txt",nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt")
+            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
 
+        #Para validacao cruzada, não é necessario salvar esse arquivos apenas normalizar conforme tipo de norma especificada
+        if (len(matX2)>1):            
+            matX2 = self.Normalize(matX2,nomepasta + "vmax_in2.npy",nomepasta + "vmin_in2.npy",nomepasta + "media_in2.npy",nomepasta + "desvio_in2.npy")                
+            if (self.normout==1):
+                matY2 = self.Normalize(matY2,nomepasta + "vmax_out2.npy",nomepasta + "vmin_out2.npy",nomepasta + "media_out2.npy",nomepasta + "desvio_out2.npy")            
+            #deleta os arquivos criados da validação cruzada que não sao uteis
+            os.remove(nomepasta + "vmax_in2.npy")
+            os.remove(nomepasta + "vmin_in2.npy")
+            os.remove(nomepasta + "media_in2.npy")
+            os.remove(nomepasta + "desvio_in2.npy")
+            os.remove(nomepasta + "vmax_out2.npy")
+            os.remove(nomepasta + "vmin_out2.npy")
+            os.remove(nomepasta + "media_out2.npy")
+            os.remove(nomepasta + "desvio_out2.npy")
+                      
+            
 
-        #Processo de aprendizado------------------------------------------------------------
 
-        VetorErro = np.zeros((self.epochs+1))
+        #Processo de aprendizado------------------------------------------------------------
+        
+        VetorErro = [0]
         MenorErro = 999999999
-
+        
         NumdataEstudo = len(matX)
+        if (len(matX2)==1):
+            NumdataEstudo2 = NumdataEstudo            
+        else:            
+            NumdataEstudo2 = len(matX2)
 
         monit=0
+        iteconv = self.iteconv
         for ite in range(0,self.epochs): #Processo iterativo global, epocas, cada epoca passa por todos os dados de aprendizagem-----------------
             Tempo = ite+1
     
             if ite > (self.epochs*monit/100): #só um monitor de progresso
                 print(str(monit) + '%')
                 monit=monit+10
-
-
-            #Calculo do erro----------------------------
-
-            EMQ = 0
-            for caso in range (0, NumdataEstudo): #Verificação do aprendizado---
-
-                #Camada 1, data de entrada
-                c1 = matX[caso,:self.nn1c]
-                R = matY[caso,:]  
-                
-                #propagacao sinal
-                c2 = np.dot(c1,P12)- B2        
-                c2 = self.Activation(self.fa2c,c2)
-
-                c3 = np.dot(c2,P23)- B3
-                c3 = self.Activation(self.fa3c,c3)
-        
-                c4 = np.dot(c3,P34)- B4
-                c4 = self.Activation(self.fa4c,c4)         
+           
+            if (self.sbw==1): #Calculo do erro-----------------------------------
 
                 regulariza=0
                 if (self.regu!=0): #adiciona a regularização se houver                    
                     regulariza = self.regu*( np.sum(P12*P12) + np.sum(P23*P23) + np.sum(P34*P34) + np.sum(B2*B2) + np.sum(B3*B3) + np.sum(B4*B4) )
+    
+                EMQ = 0
+                for caso in range (0, NumdataEstudo2): #Verificação do aprendizado---
 
-                #calculo efetivo do erro ------------
-                if (self.cost==0):#erro medio quadratico                   
-                    m_aux = 0.5*((R - c4))**2 + regulariza
-                else: #BCE, entropia cruzada binaria
-                    m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
-                
-                EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)                    
-
+                    #Camada 1, data de entrada
+                    if (len(matX2)==1):
+                        c1 = matX[caso,:self.nn1c]
+                        R = matY[caso,:]
+                    else:
+                        c1 = matX2[caso,:self.nn1c]
+                        R = matY2[caso,:]                    
+                
+                    #propagacao sinal
+                    c2 = np.dot(c1,P12)- B2        
+                    c2 = self.Activation(self.fa2c,c2)
+
+                    c3 = np.dot(c2,P23)- B3
+                    c3 = self.Activation(self.fa3c,c3)
+        
+                    c4 = np.dot(c3,P34)- B4
+                    c4 = self.Activation(self.fa4c,c4)         
+
+                    #calculo efetivo do erro ------------
+                    if (self.cost==0):#erro medio quadratico                   
+                        m_aux = 0.5*((R - c4))**2 + regulariza
+                    else: #BCE, entropia cruzada binaria
+                        m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
                 
-            VetorErro[ite+1] = EMQ 
-
+                    EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)
             
-            #memorização dos melhores pesos-----------
-            if (EMQ < MenorErro):
-                itememo = ite+1
-                MenorErro = EMQ
-                P12m = P12*1
-                P23m = P23*1
-                P34m = P34*1
-                B2m = B2*1
-                B3m = B3*1
-                B4m = B4*1
+                VetorErro.append(EMQ)
+                                               
+
+                #memorização dos melhores pesos-----------
+                if (EMQ < MenorErro):
+                    itememo = ite+1
+                    MenorErro = EMQ
+                    P12m = P12*1
+                    P23m = P23*1
+                    P34m = P34*1
+                    B2m = B2*1
+                    B3m = B3*1
+                    B4m = B4*1
+
+
+                #encerra o processamento se atender o criterio de convergencia apos n iteracoes---------            
+                if (self.conv!=0):
+                    if (ite>iteconv):          
+                        convcalc = VetorErro[ite+1]/VetorErro[ite+1-self.iteconv]                    
+                        iteconv  += self.iteconv                    
+                        if (convcalc>=self.conv and convcalc<1):                        
+                            break
+
+
+            #começa os ajustes dos pesos-------------------
+            regulariza=0
+            if (self.regu!=0): #adiciona a regularização se houver                    
+                regulariza = 2*self.regu*( np.sum(P12) + np.sum(P23) + np.sum(P34) + np.sum(B2) + np.sum(B3) + np.sum(B4) )
 
-        
             for caso in range (0, NumdataEstudo): #varredura em todos os casos de estudo--------
 
                 #Camada 1, data de entrada
                 c1 = matX[caso,:self.nn1c]
                 R = matY[caso,:]                        
                 
                 #propagacao sinal
@@ -880,18 +1018,14 @@
                 d3 = self.DeActivation(self.fa3c,c3)
                 c3 = self.Activation(self.fa3c,c3)
         
                 c4 = np.dot(c3,P34)- B4
                 d4 = self.DeActivation(self.fa4c,c4)
                 c4 = self.Activation(self.fa4c,c4)          
 
-                regulariza=0
-                if (self.regu!=0): #adiciona a regularização se houver                    
-                    regulariza = 2*self.regu*( np.sum(P12) + np.sum(P23) + np.sum(P34) + np.sum(B2) + np.sum(B3) + np.sum(B4) )
-
                 #Calcula o erro da ultima camada
                 if (self.cost==0):#EMQ
                     e4 = d4 * ( (R - c4) + regulariza )
                 else: #BCE
                     e4 = d4 * ( (R/(c4 +1e-7)) - ((1-R)/(1-c4 +1e-7)) + regulariza )
                 
                 #Propagação do erro para traz, backprop     
@@ -954,44 +1088,47 @@
             VB2= np.zeros((self.nn2c))
             VB3= np.zeros((self.nn3c))
             VB4= np.zeros((self.nn4c))
 
 
         print('100%')
 
-        P12 = P12m*1
-        P23 = P23m*1
-        P34 = P34m*1
-        B2 = B2m*1
-        B3 = B3m*1
-        B4 = B4m*1
+        if (self.sbw==1): 
+            P12 = P12m*1
+            P23 = P23m*1
+            P34 = P34m*1
+            B2 = B2m*1
+            B3 = B3m*1
+            B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
-        np.savetxt(nomepasta + "P12.txt", P12)
-        np.savetxt(nomepasta + "P23.txt", P23)
-        np.savetxt(nomepasta + "P34.txt", P34)
-        np.savetxt(nomepasta + "B2.txt", B2)
-        np.savetxt(nomepasta + "B3.txt", B3)
-        np.savetxt(nomepasta + "B4.txt", B4)
-        VetorErro[0] = itememo
-        np.savetxt(nomepasta + "Convergencia.txt", VetorErro)
+        np.save(nomepasta + "P12.npy", P12)
+        np.save(nomepasta + "P23.npy", P23)
+        np.save(nomepasta + "P34.npy", P34)
+        np.save(nomepasta + "B2.npy", B2)
+        np.save(nomepasta + "B3.npy", B3)
+        np.save(nomepasta + "B4.npy", B4)
+
+        if (self.sbw==1):
+            VetorErro[0] = itememo
+            np.save(nomepasta + "Convergencia.npy", VetorErro)
 
         tfim = time.time()
         print('runtime(s) = ' , tfim-tinicio)
 
 
 
 
 
 
 
 
     #machine learning stochastic case by case------------------------------------------------------
-    def Fit_STOC(self, matX, matY):
+    def Fit_STOC(self, matX, matY, matX2=[0], matY2=[0]):
 
         tinicio = time.time()
         
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
@@ -1042,125 +1179,132 @@
             nomepasta = self.namenet + '/'
             if not os.path.exists(self.namenet):
                 os.mkdir(self.namenet)
 
 
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
     
-            if self.nn1c ==1: #garante o formato matricial 
-                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
-            else:
-                P12 = np.loadtxt(nomepasta + "P12.txt")
-
-            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P12 = P12aux.T
-            
-            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
-                P23 = P23aux.T
-            else:
-                P23 = np.loadtxt(nomepasta + "P23.txt") 
-            
-            if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
-                P34 = P34aux.T
-            else:
-                P34 = np.loadtxt(nomepasta + "P34.txt")              
-
-            if self.nn2c ==1: #garante o formato matricial 
-                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
-            else:
-                B2 = np.loadtxt(nomepasta + "B2.txt")
-                
-            if self.nn3c ==1: #garante o formato matricial 
-                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
-            else:
-                B3 = np.loadtxt(nomepasta + "B3.txt")
-                
-            if self.nn4c ==1: #garante o formato matricial 
-                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
-            else:
-                B4 = np.loadtxt(nomepasta + "B4.txt")  
+            P12 = np.load(nomepasta + "P12.npy")
+            P23 = np.load(nomepasta + "P23.npy")            
+            P34 = np.load(nomepasta + "P34.npy")             
+            B2 = np.load(nomepasta + "B2.npy")
+            B3 = np.load(nomepasta + "B3.npy")
+            B4 = np.load(nomepasta + "B4.npy")  
 
         except: #Inicializa randomicamente-------------------------------
 
             B2 = -0.1 + 2*0.1*(np.random.rand(self.nn2c))
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))
             B4 = -0.1 + 2*0.1*(np.random.rand(self.nn4c))    
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
-        matX = self.Normalize(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt")
+        matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
         if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.txt",nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt") 
+            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+
+        #Para validacao cruzada, não é necessario salvar esse arquivos apenas normalizar conforme tipo de norma especificada
+        if (len(matX2)>1):
+            matX2 = self.Normalize(matX2,nomepasta + "vmax_in2.npy",nomepasta + "vmin_in2.npy",nomepasta + "media_in2.npy",nomepasta + "desvio_in2.npy")                
+            if (self.normout==1):
+                matY2 = self.Normalize(matY2,nomepasta + "vmax_out2.npy",nomepasta + "vmin_out2.npy",nomepasta + "media_out2.npy",nomepasta + "desvio_out2.npy")            
+            #deleta os arquivos criados
+            os.remove(nomepasta + "vmax_in2.npy")
+            os.remove(nomepasta + "vmin_in2.npy")
+            os.remove(nomepasta + "media_in2.npy")
+            os.remove(nomepasta + "desvio_in2.npy")
+            os.remove(nomepasta + "vmax_out2.npy")
+            os.remove(nomepasta + "vmin_out2.npy")
+            os.remove(nomepasta + "media_out2.npy")
+            os.remove(nomepasta + "desvio_out2.npy")
+
+
 
 
         #Processo de aprendizado------------------------------------------------------------
 
-        VetorErro = np.zeros((self.epochs+1))
+        VetorErro = [0]
         MenorErro = 999999999
 
         NumdataEstudo = len(matX)
+        if (len(matX2)==1):
+            NumdataEstudo2 = NumdataEstudo            
+        else:            
+            NumdataEstudo2 = len(matX2)
 
         monit=0
-        for ite in range(0,self.epochs): #iteração global, cada epoca varred todos os casos de estudo-------------------------
+        iteconv = self.iteconv
+        for ite in range(0,self.epochs): #Processo iterativo global, epocas, cada epoca passa por todos os dados de aprendizagem-----------------
             Tempo = ite+1
     
             if ite > (self.epochs*monit/100): #só um monitor de progresso
                 print(str(monit) + '%')
                 monit=monit+10
 
 
-            #Calculo do erro---------------------------
-
-            EMQ = 0
-            for caso in range (0, NumdataEstudo): #Verificação do aprendizado-------
-
-                #Camada 1, data de entrada
-                c1 = matX[caso,:self.nn1c]
-                R = matY[caso,:]  
-                
-                #propagacao sinal
-                c2 = np.dot(c1,P12)- B2        
-                c2 = self.Activation(self.fa2c,c2)
-
-                c3 = np.dot(c2,P23)- B3
-                c3 = self.Activation(self.fa3c,c3)
-        
-                c4 = np.dot(c3,P34)- B4
-                c4 = self.Activation(self.fa4c,c4)         
-
+            if (self.sbw==1): #Calculo do erro-----------------------------------
+            
                 regulariza=0
                 if (self.regu!=0): #adiciona a regularização se houver                    
                     regulariza = self.regu*( np.sum(P12*P12) + np.sum(P23*P23) + np.sum(P34*P34) + np.sum(B2*B2) + np.sum(B3*B3) + np.sum(B4*B4) )
 
-                #calculo efetivo do erro ------------
-                if (self.cost==0):#erro medio quadratico                   
-                    m_aux = 0.5*((R - c4))**2 + regulariza
-                else: #BCE, entropia cruzada binaria
-                    m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
+                EMQ = 0
+                for caso in range (0, NumdataEstudo2): #Verificação do aprendizado---
+
+                    #Camada 1, data de entrada
+                    if (len(matX2)==1):
+                        c1 = matX[caso,:self.nn1c]
+                        R = matY[caso,:]
+                    else:
+                        c1 = matX2[caso,:self.nn1c]
+                        R = matY2[caso,:]              
+                
+                    #propagacao sinal
+                    c2 = np.dot(c1,P12)- B2        
+                    c2 = self.Activation(self.fa2c,c2)
+
+                    c3 = np.dot(c2,P23)- B3
+                    c3 = self.Activation(self.fa3c,c3)
+        
+                    c4 = np.dot(c3,P34)- B4
+                    c4 = self.Activation(self.fa4c,c4)         
+
+                    #calculo efetivo do erro ------------
+                    if (self.cost==0):#erro medio quadratico                   
+                        m_aux = 0.5*((R - c4))**2 + regulariza
+                    else: #BCE, entropia cruzada binaria
+                        m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
                
-                EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)
+                    EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)
                    
-            VetorErro[ite+1] = EMQ 
-
+                VetorErro.append(EMQ)
+                      
  
-            #memorização dos melhores pesos------------
-            if (EMQ < MenorErro):
-                itememo = ite+1
-                MenorErro = EMQ
-                P12m = P12*1
-                P23m = P23*1
-                P34m = P34*1
-                B2m = B2*1
-                B3m = B3*1
-                B4m = B4*1
+                #memorização dos melhores pesos------------
+                if (EMQ < MenorErro):
+                    itememo = ite+1
+                    MenorErro = EMQ
+                    P12m = P12*1
+                    P23m = P23*1
+                    P34m = P34*1
+                    B2m = B2*1
+                    B3m = B3*1
+                    B4m = B4*1
+
+
+                #encerra o processamento se atender o criterio de convergencia apos n iteracoes---------            
+                if (self.conv!=0):
+                    if (ite>iteconv):          
+                        convcalc = VetorErro[ite+1]/VetorErro[ite+1-self.iteconv]                    
+                        iteconv  += self.iteconv                    
+                        if (convcalc>=self.conv and convcalc<1):                        
+                            break
 
 
             for caso in range (0, NumdataEstudo): #varredura em todos os casos, mas no estocastico, atualiza os pesos caso a caso---
 
                 #Camada 1, data de entrada
                 c1 = matX[caso,:self.nn1c]
                 R = matY[caso,:]                        
@@ -1202,154 +1346,47 @@
                 B2 += - self.rate * e2
                 B3 += - self.rate * e3
                 B4 += - self.rate * e4
         
 
         print('100%')
 
-        P12 = P12m*1
-        P23 = P23m*1
-        P34 = P34m*1
-        B2 = B2m*1
-        B3 = B3m*1
-        B4 = B4m*1
+        if (self.sbw==1):
+            P12 = P12m*1
+            P23 = P23m*1
+            P34 = P34m*1
+            B2 = B2m*1
+            B3 = B3m*1
+            B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
-        np.savetxt(nomepasta + "P12.txt", P12)
-        np.savetxt(nomepasta + "P23.txt", P23)
-        np.savetxt(nomepasta + "P34.txt", P34)
-        np.savetxt(nomepasta + "B2.txt", B2)
-        np.savetxt(nomepasta + "B3.txt", B3)
-        np.savetxt(nomepasta + "B4.txt", B4)
-        VetorErro[0] = itememo
-        np.savetxt(nomepasta + "Convergencia.txt", VetorErro)
+        np.save(nomepasta + "P12.npy", P12)
+        np.save(nomepasta + "P23.npy", P23)
+        np.save(nomepasta + "P34.npy", P34)
+        np.save(nomepasta + "B2.npy", B2)
+        np.save(nomepasta + "B3.npy", B3)
+        np.save(nomepasta + "B4.npy", B4)
+
+        if (self.sbw==1):
+            VetorErro[0] = itememo
+            np.save(nomepasta + "Convergencia.npy", VetorErro)
 
         tfim = time.time()
         print('runtime(s) = ' , tfim-tinicio)
 
 
 
 
 
 
 
 
-
-
-    #make prediction----------------------------------------------------------
-    def Predict(self, matX):
-        
-        #pesos
-        P12 = np.zeros((self.nn1c,self.nn2c))
-        P23 = np.zeros((self.nn2c,self.nn3c))
-        P34 = np.zeros((self.nn3c,self.nn4c))
-        #bias
-        B2= np.zeros((self.nn2c))
-        B3= np.zeros((self.nn3c))
-        B4= np.zeros((self.nn4c))
-        #camadas
-        c1= np.zeros((self.nn1c))
-        c2= np.zeros((self.nn2c))
-        c3= np.zeros((self.nn3c))
-        c4= np.zeros((self.nn4c))
-
-
-        #ajuste do local de salvamento, se especificado
-        if (self.namenet==''):
-            nomepasta=''
-        else:
-            nomepasta = self.namenet + '/'
-            
-
-        try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
-    
-            if self.nn1c ==1: #garante o formato matricial 
-                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
-            else:
-                P12 = np.loadtxt(nomepasta + "P12.txt")
-
-            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P12 = P12aux.T
-            
-            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
-                P23 = P23aux.T
-            else:
-                P23 = np.loadtxt(nomepasta + "P23.txt") 
-            
-            if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
-                P34 = P34aux.T
-            else:
-                P34 = np.loadtxt(nomepasta + "P34.txt")              
-
-            if self.nn2c ==1: #garante o formato matricial 
-                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
-            else:
-                B2 = np.loadtxt(nomepasta + "B2.txt")
-                
-            if self.nn3c ==1: #garante o formato matricial 
-                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
-            else:
-                B3 = np.loadtxt(nomepasta + "B3.txt")
-                
-            if self.nn4c ==1: #garante o formato matricial 
-                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
-            else:
-                B4 = np.loadtxt(nomepasta + "B4.txt")
-                
-        except: #se nao tem pesos salvos encerra o programa-------------------------------
-
-           input('No saved weight files')
-           exit()
-
-        #Normaliza a entrada de data----------------------
-        matX = self.Normalize2(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt") 
-
-        
-        #Predição----------------------------
-        numdata = len(matX)
-        Calculated = np.zeros((numdata, self.nn4c)) #inicializa a matriz dos resultados Calculated
-        
-        for caso in range (0, numdata):
-
-            #Camada 1, data de entrada
-            c1 = matX[caso,:self.nn1c]                     
-                
-            #propagacao sinal
-            c2 = np.dot(c1,P12)- B2     
-            c2 = self.Activation(self.fa2c,c2)
-
-            c3 = np.dot(c2,P23)- B3
-            c3 = self.Activation(self.fa3c,c3)
-        
-            c4 = np.dot(c3,P34)- B4
-            c4 = self.Activation(self.fa4c,c4)         
-
-            # saida----------------------------
-            Calculated[caso][:] = c4[:]
-
-        if (self.normout==1):            
-            Calculated = self.DesNormalize(Calculated, nomepasta + "vmax_out.txt", nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt") 
-
-        return Calculated
-
-
-
-
-
-
-
-
-
-
-
     #machine learning,  single batch with ADAM accelerator-----------------------------------------------------
-    def Fit_STOC_ADAM(self, matX, matY):
+    def Fit_STOC_ADAM(self, matX, matY, matX2=[0], matY2=[0]):
 
         tinicio = time.time()
         
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
@@ -1431,126 +1468,132 @@
             if not os.path.exists(self.namenet):
                 os.mkdir(self.namenet)
 
 
 
         try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
     
-            if self.nn1c ==1: #garante o formato matricial 
-                P12 = np.array([np.loadtxt(nomepasta + "P12.txt")])        
-            else:
-                P12 = np.loadtxt(nomepasta + "P12.txt")
-
-            if self.nn2c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P12 = P12aux.T
-            
-            if self.nn3c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P23aux = np.array([np.loadtxt(nomepasta + "P23.txt")])
-                P23 = P23aux.T
-            else:
-                P23 = np.loadtxt(nomepasta + "P23.txt") 
-            
-            if self.nn4c ==1: #uma linha de data ele sempre le como vetor de colunas, e a transposta disso precisa de um esquema especial
-                P34aux = np.array([np.loadtxt(nomepasta + "P34.txt")])
-                P34 = P34aux.T
-            else:
-                P34 = np.loadtxt(nomepasta + "P34.txt")              
-
-            if self.nn2c ==1: #garante o formato matricial 
-                B2 = np.array([np.loadtxt(nomepasta + "B2.txt")])        
-            else:
-                B2 = np.loadtxt(nomepasta + "B2.txt")
-                
-            if self.nn3c ==1: #garante o formato matricial 
-                B3 = np.array([np.loadtxt(nomepasta + "B3.txt")])        
-            else:
-                B3 = np.loadtxt(nomepasta + "B3.txt")
-                
-            if self.nn4c ==1: #garante o formato matricial 
-                B4 = np.array([np.loadtxt(nomepasta + "B4.txt")])        
-            else:
-                B4 = np.loadtxt(nomepasta + "B4.txt")  
+            P12 = np.load(nomepasta + "P12.npy")
+            P23 = np.load(nomepasta + "P23.npy")            
+            P34 = np.load(nomepasta + "P34.npy")             
+            B2 = np.load(nomepasta + "B2.npy")
+            B3 = np.load(nomepasta + "B3.npy")
+            B4 = np.load(nomepasta + "B4.npy")  
 
         except: #Inicializa randomicamente-------------------------------
 
             B2 = -0.1 + 2*0.1*(np.random.rand(self.nn2c))
             B3 = -0.1 + 2*0.1*(np.random.rand(self.nn3c))
             B4 = -0.1 + 2*0.1*(np.random.rand(self.nn4c))    
             P12 = -0.1 + 2*0.1*(np.random.rand(self.nn1c,self.nn2c))
             P23 = -0.1 + 2*0.1*(np.random.rand(self.nn2c,self.nn3c))
             P34 = -0.1 + 2*0.1*(np.random.rand(self.nn3c,self.nn4c))
 
 
         #Normaliza os parametros-------------------------
-        matX = self.Normalize(matX,nomepasta + "vmax_in.txt",nomepasta + "vmin_in.txt",nomepasta + "media_in.txt",nomepasta + "desvio_in.txt")
+        matX = self.Normalize(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy")                
         if (self.normout==1):
-            matY = self.Normalize(matY,nomepasta + "vmax_out.txt",nomepasta + "vmin_out.txt",nomepasta + "media_out.txt",nomepasta + "desvio_out.txt")
+            matY = self.Normalize(matY,nomepasta + "vmax_out.npy",nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy")
+
+        #Para validacao cruzada, não é necessario salvar esse arquivos apenas normalizar conforme tipo de norma especificada
+        if (len(matX2)>1):
+            matX2 = self.Normalize(matX2,nomepasta + "vmax_in2.npy",nomepasta + "vmin_in2.npy",nomepasta + "media_in2.npy",nomepasta + "desvio_in2.npy")                
+            if (self.normout==1):
+                matY2 = self.Normalize(matY2,nomepasta + "vmax_out2.npy",nomepasta + "vmin_out2.npy",nomepasta + "media_out2.npy",nomepasta + "desvio_out2.npy")            
+            #deleta os arquivos criados
+            os.remove(nomepasta + "vmax_in2.npy")
+            os.remove(nomepasta + "vmin_in2.npy")
+            os.remove(nomepasta + "media_in2.npy")
+            os.remove(nomepasta + "desvio_in2.npy")
+            os.remove(nomepasta + "vmax_out2.npy")
+            os.remove(nomepasta + "vmin_out2.npy")
+            os.remove(nomepasta + "media_out2.npy")
+            os.remove(nomepasta + "desvio_out2.npy")
+
 
 
         #Processo de aprendizado------------------------------------------------------------
 
-        VetorErro = np.zeros((self.epochs+1))
+        VetorErro = [0]
         MenorErro = 999999999
 
         NumdataEstudo = len(matX)
+        if (len(matX2)==1):
+            NumdataEstudo2 = NumdataEstudo            
+        else:            
+            NumdataEstudo2 = len(matX2)
 
         monit=0
+        iteconv = self.iteconv
         for ite in range(0,self.epochs): #Processo iterativo global, epocas, cada epoca passa por todos os dados de aprendizagem-----------------
             Tempo = ite+1
     
             if ite > (self.epochs*monit/100): #só um monitor de progresso
                 print(str(monit) + '%')
                 monit=monit+10
 
 
-            #Calculo do erro----------------------------
-
-            EMQ = 0
-            for caso in range (0, NumdataEstudo): #Verificação do aprendizado---
-
-                #Camada 1, data de entrada
-                c1 = matX[caso,:self.nn1c]
-                R = matY[caso,:]  
-                
-                #propagacao sinal
-                c2 = np.dot(c1,P12)- B2        
-                c2 = self.Activation(self.fa2c,c2)
-
-                c3 = np.dot(c2,P23)- B3
-                c3 = self.Activation(self.fa3c,c3)
-        
-                c4 = np.dot(c3,P34)- B4
-                c4 = self.Activation(self.fa4c,c4)         
-
+            if (self.sbw==1): #Calculo do erro-----------------------------------
+            
                 regulariza=0
                 if (self.regu!=0): #adiciona a regularização se houver                    
                     regulariza = self.regu*( np.sum(P12*P12) + np.sum(P23*P23) + np.sum(P34*P34) + np.sum(B2*B2) + np.sum(B3*B3) + np.sum(B4*B4) )
 
-                #calculo efetivo do erro ------------
-                if (self.cost==0):#erro medio quadratico                   
-                    m_aux = 0.5*((R - c4))**2 + regulariza
-                else: #BCE, entropia cruzada binaria
-                    m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
-                
-                EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)                    
-
-                
-            VetorErro[ite+1] = EMQ 
+                EMQ = 0
+                for caso in range (0, NumdataEstudo2): #Verificação do aprendizado---
 
-            
-            #memorização dos melhores pesos-----------
-            if (EMQ < MenorErro):
-                itememo = ite+1
-                MenorErro = EMQ
-                P12m = P12*1
-                P23m = P23*1
-                P34m = P34*1
-                B2m = B2*1
-                B3m = B3*1
-                B4m = B4*1
+                    #Camada 1, data de entrada
+                    if (len(matX2)==1):
+                        c1 = matX[caso,:self.nn1c]
+                        R = matY[caso,:]
+                    else:
+                        c1 = matX2[caso,:self.nn1c]
+                        R = matY2[caso,:]              
+                
+                    #propagacao sinal
+                    c2 = np.dot(c1,P12)- B2        
+                    c2 = self.Activation(self.fa2c,c2)
+
+                    c3 = np.dot(c2,P23)- B3
+                    c3 = self.Activation(self.fa3c,c3)
+        
+                    c4 = np.dot(c3,P34)- B4
+                    c4 = self.Activation(self.fa4c,c4)         
+
+                    #calculo efetivo do erro ------------
+                    if (self.cost==0):#erro medio quadratico                   
+                        m_aux = 0.5*((R - c4))**2 + regulariza
+                    else: #BCE, entropia cruzada binaria
+                        m_aux = -1*(R*np.log(c4 +1e-10)+(1-R)*np.log((1-c4) +1e-10)) + regulariza
+                
+                    EMQ = EMQ + np.sum(m_aux)/(NumdataEstudo*self.nn4c)                    
+
+                
+                VetorErro.append(EMQ)
+
+
+                #memorização dos melhores pesos-----------
+                if (EMQ < MenorErro):
+                    itememo = ite+1
+                    MenorErro = EMQ
+                    P12m = P12*1
+                    P23m = P23*1
+                    P34m = P34*1
+                    B2m = B2*1
+                    B3m = B3*1
+                    B4m = B4*1
+
+
+                #encerra o processamento se atender o criterio de convergencia apos n iteracoes---------            
+                if (self.conv!=0):
+                    if (ite>iteconv):          
+                        convcalc = VetorErro[ite+1]/VetorErro[ite+1-self.iteconv]                    
+                        iteconv  += self.iteconv                    
+                        if (convcalc>=self.conv and convcalc<1):                        
+                            break
 
         
             for caso in range (0, NumdataEstudo): #varredura em todos os casos de estudo--------
 
                 #Camada 1, data de entrada
                 c1 = matX[caso,:self.nn1c]
                 R = matY[caso,:]                        
@@ -1622,77 +1665,170 @@
                 B2 = B2 + self.rate*( (massaB2/aux1) / np.sqrt(veloB2/aux2) )
                 B3 = B3 + self.rate*( (massaB3/aux1) / np.sqrt(veloB3/aux2) )
                 B4 = B4 + self.rate*( (massaB4/aux1) / np.sqrt(veloB4/aux2) )
  
 
         print('100%')
 
-        P12 = P12m*1
-        P23 = P23m*1
-        P34 = P34m*1
-        B2 = B2m*1
-        B3 = B3m*1
-        B4 = B4m*1
+        if (self.sbw==1):            
+            P12 = P12m*1
+            P23 = P23m*1
+            P34 = P34m*1
+            B2 = B2m*1
+            B3 = B3m*1
+            B4 = B4m*1
 
 
         #Salva os pesos e bias em arquivos txt----------------------------------------------------------
-        np.savetxt(nomepasta + "P12.txt", P12)
-        np.savetxt(nomepasta + "P23.txt", P23)
-        np.savetxt(nomepasta + "P34.txt", P34)
-        np.savetxt(nomepasta + "B2.txt", B2)
-        np.savetxt(nomepasta + "B3.txt", B3)
-        np.savetxt(nomepasta + "B4.txt", B4)
-        VetorErro[0] = itememo
-        np.savetxt(nomepasta + "Convergencia.txt", VetorErro)
+        np.save(nomepasta + "P12.npy", P12)
+        np.save(nomepasta + "P23.npy", P23)
+        np.save(nomepasta + "P34.npy", P34)
+        np.save(nomepasta + "B2.npy", B2)
+        np.save(nomepasta + "B3.npy", B3)
+        np.save(nomepasta + "B4.npy", B4)
+
+        if (self.sbw==1):
+            VetorErro[0] = itememo
+            np.save(nomepasta + "Convergencia.npy", VetorErro)
 
         tfim = time.time()
         print('runtime(s) = ' , tfim-tinicio)
 
 
 
 
 
 
 
 
 
+###############################################################
+###############################################################
+################ Aplication of NN   ###########################
+###############################################################
+###############################################################
 
 
 
 
-
-    #Plota a convergencia ----------------------------------------------------------
-    def Plotconv(self):
+    #make prediction----------------------------------------------------------
+    def Predict(self, matX):
+        
+        #pesos
+        P12 = np.zeros((self.nn1c,self.nn2c))
+        P23 = np.zeros((self.nn2c,self.nn3c))
+        P34 = np.zeros((self.nn3c,self.nn4c))
+        #bias
+        B2= np.zeros((self.nn2c))
+        B3= np.zeros((self.nn3c))
+        B4= np.zeros((self.nn4c))
+        #camadas
+        c1= np.zeros((self.nn1c))
+        c2= np.zeros((self.nn2c))
+        c3= np.zeros((self.nn3c))
+        c4= np.zeros((self.nn4c))
 
 
         #ajuste do local de salvamento, se especificado
         if (self.namenet==''):
             nomepasta=''
         else:
             nomepasta = self.namenet + '/'
-
             
-        #grafico da convergencia
-        Conve = np.loadtxt(nomepasta + "Convergencia.txt")
-        tamanho = len(Conve)
+
+        try: #Inicializa com pesos ja salvos, se existir esses arquivos-------------------------------------
+    
+            P12 = np.load(nomepasta + "P12.npy")
+            P23 = np.load(nomepasta + "P23.npy")            
+            P34 = np.load(nomepasta + "P34.npy")             
+            B2 = np.load(nomepasta + "B2.npy")
+            B3 = np.load(nomepasta + "B3.npy")
+            B4 = np.load(nomepasta + "B4.npy")  
+                
+        except: #se nao tem pesos salvos encerra o programa-------------------------------
+
+           input('No saved weight files')
+           exit()
+
+        #Normaliza a entrada de data----------------------
+        matX = self.Normalize2(matX,nomepasta + "vmax_in.npy",nomepasta + "vmin_in.npy",nomepasta + "media_in.npy",nomepasta + "desvio_in.npy") 
+
         
-        MenorErro = np.min(Conve)
-        itemenorerro = Conve[0]
+        #Predição----------------------------
+        numdata = len(matX)
+        Calculated = np.zeros((numdata, self.nn4c)) #inicializa a matriz dos resultados Calculated
+        
+        for caso in range (0, numdata):
+
+            #Camada 1, data de entrada
+            c1 = matX[caso,:self.nn1c]                     
+                
+            #propagacao sinal
+            c2 = np.dot(c1,P12)- B2     
+            c2 = self.Activation(self.fa2c,c2)
+
+            c3 = np.dot(c2,P23)- B3
+            c3 = self.Activation(self.fa3c,c3)
+        
+            c4 = np.dot(c3,P34)- B4
+            c4 = self.Activation(self.fa4c,c4)         
+
+            # saida----------------------------
+            Calculated[caso][:] = c4[:]
+
+        if (self.normout==1):            
+            Calculated = self.DesNormalize(Calculated, nomepasta + "vmax_out.npy", nomepasta + "vmin_out.npy",nomepasta + "media_out.npy",nomepasta + "desvio_out.npy") 
+
+        return Calculated
+
+
+
+
+
 
-        eixoX = np.zeros((tamanho-1)) 
-        eixoY = np.zeros((tamanho-1))
 
-        eixoX = np.arange(0, tamanho-1, dtype=int)
-        eixoY = Conve[1:tamanho]
-    
-        plt.figure(figsize=(12, 5))
-        plt.title('Mean squared error = ' + str(MenorErro) + ', iteration number = ' + str(itemenorerro))
-        plt.xlabel('Study data')
-        plt.ylabel('Error, mse')
-        plt.plot(eixoX, eixoY, marker = '', color = 'darkblue')  
-        plt.show()
 
 
+###############################################################
+###############################################################
+################ Auxliliar plot   #############################
+###############################################################
+###############################################################
+
+
+
+
+    #Plota a convergencia ----------------------------------------------------------
+    def Plotconv(self):
+
+        if (self.sbw==1):
+            
+            #ajuste do local de salvamento, se especificado
+            if (self.namenet==''):
+                nomepasta=''
+            else:
+                nomepasta = self.namenet + '/'
+
+            
+            #grafico da convergencia
+            Conve = np.load(nomepasta + "Convergencia.npy")
+            tamanho = len(Conve)
+        
+            MenorErro = np.min(Conve)
+            itemenorerro = Conve[0]
+
+            eixoX = np.zeros((tamanho-1)) 
+            eixoY = np.zeros((tamanho-1))
+
+            eixoX = np.arange(0, tamanho-1, dtype=int)
+            eixoY = Conve[1:tamanho]
+    
+            plt.figure(figsize=(12, 5))
+            plt.title('Mean squared error = ' + str(MenorErro) + ', iteration number = ' + str(itemenorerro))
+            plt.xlabel('Study data')
+            plt.ylabel('Error, mse')
+            plt.plot(eixoX, eixoY, marker = '', color = 'darkblue')  
+            plt.show()
```

### Comparing `tupa123-1.3.9/tupa123.egg-info/PKG-INFO` & `tupa123-1.4.0/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.3.9
+Version: 1.4.0
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

