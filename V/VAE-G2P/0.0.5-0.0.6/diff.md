# Comparing `tmp/VAE_G2P-0.0.5.tar.gz` & `tmp/VAE_G2P-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VAE_G2P-0.0.5.tar", last modified: Wed Apr  5 06:00:38 2023, max compression
+gzip compressed data, was "VAE_G2P-0.0.6.tar", last modified: Wed Apr 26 05:32:33 2023, max compression
```

## Comparing `VAE_G2P-0.0.5.tar` & `VAE_G2P-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-05 06:00:38.507404 VAE_G2P-0.0.5/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-05 06:00:38.507273 VAE_G2P-0.0.5/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.0.5/README.md
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-05 06:00:38.506397 VAE_G2P-0.0.5/VAE_G2P/
--rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.0.5/VAE_G2P/__init__.py
--rw-r--r--   0 davidblair   (501) staff       (20)    19614 2023-04-05 04:47:05.000000 VAE_G2P-0.0.5/VAE_G2P/basic_g2p.py
--rw-r--r--   0 davidblair   (501) staff       (20)    13488 2023-04-05 04:47:18.000000 VAE_G2P-0.0.5/VAE_G2P/cvae_model.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15203 2023-04-04 23:35:20.000000 VAE_G2P-0.0.5/VAE_G2P/data.py
--rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.0.5/VAE_G2P/data_wrapper.py
--rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.0.5/VAE_G2P/networks.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15046 2023-04-05 04:47:50.000000 VAE_G2P-0.0.5/VAE_G2P/optim.py
--rw-r--r--   0 davidblair   (501) staff       (20)    23552 2023-04-05 05:59:49.000000 VAE_G2P-0.0.5/VAE_G2P/vae_g2p.py
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-05 06:00:38.507101 VAE_G2P-0.0.5/VAE_G2P.egg-info/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-05 06:00:38.000000 VAE_G2P-0.0.5/VAE_G2P.egg-info/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-04-05 06:00:38.000000 VAE_G2P-0.0.5/VAE_G2P.egg-info/SOURCES.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-04-05 06:00:38.000000 VAE_G2P-0.0.5/VAE_G2P.egg-info/dependency_links.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-04-05 06:00:38.000000 VAE_G2P-0.0.5/VAE_G2P.egg-info/requires.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-04-05 06:00:38.000000 VAE_G2P-0.0.5/VAE_G2P.egg-info/top_level.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-04-05 06:00:38.507441 VAE_G2P-0.0.5/setup.cfg
--rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.0.5/setup.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-26 05:32:33.955181 VAE_G2P-0.0.6/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-26 05:32:33.955046 VAE_G2P-0.0.6/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.0.6/README.md
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-26 05:32:33.953983 VAE_G2P-0.0.6/VAE_G2P/
+-rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.0.6/VAE_G2P/__init__.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    19614 2023-04-05 04:47:05.000000 VAE_G2P-0.0.6/VAE_G2P/basic_g2p.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    13488 2023-04-05 04:47:18.000000 VAE_G2P-0.0.6/VAE_G2P/cvae_model.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    15876 2023-04-26 05:24:52.000000 VAE_G2P-0.0.6/VAE_G2P/data.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.0.6/VAE_G2P/data_wrapper.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.0.6/VAE_G2P/networks.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    15046 2023-04-05 04:47:50.000000 VAE_G2P-0.0.6/VAE_G2P/optim.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    23311 2023-04-26 05:29:45.000000 VAE_G2P-0.0.6/VAE_G2P/vae_g2p.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-26 05:32:33.954870 VAE_G2P-0.0.6/VAE_G2P.egg-info/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/SOURCES.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/dependency_links.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/requires.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-04-26 05:32:33.000000 VAE_G2P-0.0.6/VAE_G2P.egg-info/top_level.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-04-26 05:32:33.955218 VAE_G2P-0.0.6/setup.cfg
+-rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.0.6/setup.py
```

### Comparing `VAE_G2P-0.0.5/VAE_G2P/basic_g2p.py` & `VAE_G2P-0.0.6/VAE_G2P/basic_g2p.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.5/VAE_G2P/cvae_model.py` & `VAE_G2P-0.0.6/VAE_G2P/cvae_model.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.5/VAE_G2P/data.py` & `VAE_G2P-0.0.6/VAE_G2P/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,26 @@
 					assert len(all_unique)>1, "Must have at least 2 categories for one-hot variable."
 					idx_map=dict(zip(all_unique,list(range(len(all_unique)))))
 					self.aux_gene_info_table.loc[col]['idx_map']=idx_map
 					self.aux_gene_info_table.loc[col]['inv_idx_map']=dict(zip(idx_map.values(),idx_map.keys()))
 					self.gene_info_table[col]=self.gene_info_table[col].apply(lambda x: idx_map[x])
 					self.aux_gene_info_table.loc[col,'return_dim']=len(idx_map)-1
 	
+	def _ProcessSymptomCounts(self, symptom_freq_info,prior_count):
+		if isinstance(symptom_freq_info,tuple):
+			num=symptom_freq_info[0]
+			denom=symptom_freq_info[1]
+			freq_estimate=((num+prior_count)/(denom+prior_count*2.0))
+			for i,cp in enumerate(self.ordinal_cut_points):
+				if freq_estimate<=cp:
+					return i
+		else:
+			return self.ordinal_freq_map[symptom_freq_info]
 
-	def __init__(self,disease_labels,symptom_freq_pairs,disease_associated_genes,gene_info_table,ordinal_freq_map,training_data_fraction,validation_data_fraction,missing_label='NA'):
+	def __init__(self,disease_labels,symptom_freq_pairs,disease_associated_genes,gene_info_table,ordinal_freq_upperlimits,training_data_fraction,validation_data_fraction,missing_label='NA',preprocess_symptom_counts=True,symptom_count_prior=1.0):
 		"""Dataset that stores disease-symptom annotations as a sparse array that can be used for disease embedding.
 		
 		Args:
 		    disease_labels (Array of Strings): Strings that make up the index of the disease dataset
 		    symptom_freq_pairs (Array of iterables): Each list contains the symptoms-frequency pairs annotated to each disease. Symptoms-frequencies are stored as a tuple.
 		    ordinal_freq_map (Dictionary): Dictionary providing ordinal rank of each frequency used to describe the symptoms. 
 		    missing_label (str, optional): String used to denote missing frequency information.
@@ -65,24 +75,28 @@
 		self.disease_table=pd.DataFrame(columns=['SympFreqs','MappedGenes'],index=disease_labels)
 		orig_symp_values = pd.Series(symptom_freq_pairs,index=disease_labels)
 		all_unique_symptoms=sorted(list(set().union(*orig_symp_values.apply(lambda x:[y[0] for y in x]).values)))
 		self.symptom_map=dict(zip(all_unique_symptoms,range(len(all_unique_symptoms))))
 		self.inverse_symptom_map=dict(zip(self.symptom_map.values(),self.symptom_map.keys()))
 		self.num_symptoms=len(self.symptom_map)
 		
-		self.ordinal_freq_map=ordinal_freq_map
-		assert -1 not in ordinal_freq_map.values(),"-1 is not allowed as ordinal value for symptom frequency. This represents missing data and is reserved for this purpose."
+		self.ordinal_cut_points=np.array(list(ordinal_freq_upperlimits.values()))
+		self.ordinal_freq_map=dict(zip(np.array(list(ordinal_freq_upperlimits.keys()))[np.argsort(self.ordinal_cut_points)],np.arange(self.ordinal_cut_points.shape[0])))
 		self.ordinal_freq_map[missing_label]=-1
 		self.num_ordinal_freqs = len(self.ordinal_freq_map)-1
 		self.missing_label=missing_label
 
 		self.gene_info_table=gene_info_table
+		self.symptom_count_prior=symptom_count_prior
 
-		new_symptoms = orig_symp_values.apply(lambda x: [(self.symptom_map[y[0]],self.ordinal_freq_map[y[1]]) for y in x])
-		self.disease_table['SympFreqs']=new_symptoms
+		if preprocess_symptom_counts:
+			new_symptoms = orig_symp_values.apply(lambda x: [(self.symptom_map[y[0]],self._ProcessSymptomCounts(y[1],symptom_count_prior)) for y in x])
+			self.disease_table['SympFreqs']=new_symptoms
+		else:
+			raise ValueError("Direct modeling of symptoms counts not yet supported.")
 		orig_gene_values=pd.Series(disease_associated_genes,index=disease_labels)
 		self.gene_map=dict(zip(self.gene_info_table.index,range(self.gene_info_table.index.shape[0])))
 		self.inverse_gene_map=dict(zip(self.gene_map.values(),self.gene_map.keys()))
 		self.num_total_genes = len(self.gene_map)
 		self.disease_table['MappedGenes']=orig_gene_values.apply(lambda x: self.gene_map[x])
 
 
@@ -278,8 +292,8 @@
 	omim_table=pd.read_pickle('../../../Data/OMIM_HPO_Table/OMIMSingleGeneInNetworkHPOUnrolled.pth')
 	pp_embed=pd.read_csv('../../../Data/PrimeKG/NetworkEmbeddings/PrimeKG_protein_protein_Dim8.txt',sep=' ',header=None,skiprows=[0])
 	pp_embed.set_index(0,inplace=True)
 	gene_table=pd.read_pickle('../../../Data/PrimeKG/PrimeKG_ProteinFeatures.pth')
 	gene_table.loc[gene_table.index,'net_embed']=pd.Series([x for x in pp_embed.loc[gene_table.index].values],index=gene_table.index)
 
 
-	self=GeneToPhenotypeDataset(omim_table.index,omim_table.HPO_wFreq,omim_table['GENE/INHERIT'].apply(lambda x:x[0]),gene_table,{'VR':0,'OC':1,'F':2,'VF':3,'O':4},0.6,0.15,missing_label='NA')
+	self=GeneToPhenotypeDataset(omim_table.index,omim_table.HPO_wFreq,omim_table['GENE/INHERIT'].apply(lambda x:x[0]),gene_table,{'VR':0.04,'OC':0.3,'F':0.8,'VF':0.99,'O':1.0},0.6,0.15,missing_label='NA')
```

### Comparing `VAE_G2P-0.0.5/VAE_G2P/data_wrapper.py` & `VAE_G2P-0.0.6/VAE_G2P/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.5/VAE_G2P/networks.py` & `VAE_G2P-0.0.6/VAE_G2P/networks.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.5/VAE_G2P/optim.py` & `VAE_G2P-0.0.6/VAE_G2P/optim.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.5/VAE_G2P/vae_g2p.py` & `VAE_G2P-0.0.6/VAE_G2P/vae_g2p.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import copy
 
 from .cvae_model import DiseaseCondVAE
 from .basic_g2p import BasicG2PModel
 from .data import GeneToPhenotypeDataset
 from .optim import AutoEncoderOptimizer
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 class VAE_G2P:
 
 	def _readModelFromFile(self,fName):
 		with open(fName,'rb') as f:
 			model_dict = torch.load(f,map_location='cpu')
@@ -34,23 +34,18 @@
 			self.all_model_kwargs['encoder_hyperparameters']={'n_layers' : 2, 'n_hidden' : 64, 'dropout_rate': 0.1, 'use_batch_norm':True}
 		if 'decoder_hyperparameters' not in self.all_model_kwargs.keys():
 			self.all_model_kwargs['decoder_hyperparameters']={'n_layers' : 2, 'n_hidden' : 64, 'dropout_rate': 0.1, 'use_batch_norm':True}
 
 		if 'missing_freq_priors' not in self.all_model_kwargs.keys():
 			self.all_model_kwargs['missing_freq_priors']=[0.0,3.0]
 
-		if 'frequency_cut_points' not in self.all_model_kwargs.keys():
-			self.all_model_kwargs['frequency_cut_points']=[0.04,0.3,0.8,0.99]
-
-		assert (len(self.all_model_kwargs['frequency_cut_points'])+1)==self.diseaseGeneDataset.num_ordinal_freqs, "Number of model cutpoints must equal number frequency classes in dataset, excluding the Unknown class"
-
 	
-		self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],cut_points=self.all_model_kwargs['frequency_cut_points'])
+		self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
 
-		self.vae_g2p_model=DiseaseCondVAE(self.numSymptoms,self.numFreqCats,self.nLatentDim,self.basic_g2p,isLinear=self.isLinear,encoder_hyperparameters=self.all_model_kwargs['encoder_hyperparameters'],decoder_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],missing_freq_prior_mean=self.all_model_kwargs['missing_freq_priors'][0],missing_freq_prior_scale=self.all_model_kwargs['missing_freq_priors'][1],cut_points=self.all_model_kwargs['frequency_cut_points'])
+		self.vae_g2p_model=DiseaseCondVAE(self.numSymptoms,self.numFreqCats,self.nLatentDim,self.basic_g2p,isLinear=self.isLinear,encoder_hyperparameters=self.all_model_kwargs['encoder_hyperparameters'],decoder_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],missing_freq_prior_mean=self.all_model_kwargs['missing_freq_priors'][0],missing_freq_prior_scale=self.all_model_kwargs['missing_freq_priors'][1],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
 
 
 	def Fit(self,batch_size,logFile=None,verbose=True,monitor_validation=True,prior_model_state=None,**kwargs):
 		"""
 
 
 		Parameters
@@ -223,15 +218,15 @@
 		if len(gene_list)<len(hpo_freq_pairs):
 			gene_list=gene_list*len(hpo_freq_pairs)
 		elif len(gene_list)>len(hpo_freq_pairs):
 			hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
 
 		for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
 			idx_vec=[self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec]
-			freq_vec=[self.diseaseGeneDataset.ordinal_freq_map[x[1]] for x in hpo_freq_vec]
+			freq_vec=[self.diseaseGeneDataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
 			annot_array[t,idx_vec]=1.0
 			freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
 
 		data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
 
 		elbo=self.vae_g2p_model.per_datum_ELBO(*data,num_particles=num_particles)
 		return elbo.detach().numpy().ravel()
@@ -264,15 +259,15 @@
 		if len(gene_list)<len(hpo_freq_pairs):
 			gene_list=gene_list*len(hpo_freq_pairs)
 		elif len(gene_list)>len(hpo_freq_pairs):
 			hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
 
 		for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
 			idx_vec=[self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec]
-			freq_vec=[self.diseaseGeneDataset.ordinal_freq_map[x[1]] for x in hpo_freq_vec]
+			freq_vec=[self.diseaseGeneDataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
 			annot_array[t,idx_vec]=1.0
 			freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
 
 		data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
 		p_m,p_std=self.vae_g2p_model.posterior_latent_state(*data)
 
 		if index is None:
@@ -297,15 +292,15 @@
 		if len(gene_list)<len(hpo_freq_pairs):
 			gene_list=gene_list*len(hpo_freq_pairs)
 		elif len(gene_list)>len(hpo_freq_pairs):
 			hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
 
 		for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
 			idx_vec=[self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec]
-			freq_vec=[self.diseaseGeneDataset.ordinal_freq_map[x[1]] for x in hpo_freq_vec]
+			freq_vec=[self.diseaseGeneDataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
 			annot_array[t,idx_vec]=1.0
 			freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
 
 		data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
 		p_m,p_std=self.vae_g2p_model.posterior_latent_state(*data)
 
 		if returnStdErrors:
@@ -412,26 +407,26 @@
 
 		"""
 		if not isinstance(stored_model,dict):
 			assert isinstance(stored_model,str),"Expects file name if not provided with dictionary."
 			stored_model = self._readModelFromFile(stored_model)
 
 		assert set(stored_model.keys())==set(['model_state','meta_data','variational_post_params','baseline_g2p_model']),"Model dictionary must contain the following elements: 'model_state','meta_data','baseline_g2p_model'"
-		self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=stored_model['meta_data']['all_model_kwargs']['decoder_hyperparameters'],cut_points=stored_model['meta_data']['all_model_kwargs']['frequency_cut_points'])
+		self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=stored_model['meta_data']['all_model_kwargs']['decoder_hyperparameters'],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
 		self.vae_g2p_model=DiseaseCondVAE(
 			stored_model['meta_data']['numSymptoms'],
 			stored_model['meta_data']['numFreqCats'],
 			stored_model['meta_data']['nLatentDim'],
 			self.basic_g2p,
 			isLinear=stored_model['meta_data']['isLinear'],
 			encoder_hyperparameters=stored_model['meta_data']['all_model_kwargs']['encoder_hyperparameters'],
 			decoder_hyperparameters=stored_model['meta_data']['all_model_kwargs']['decoder_hyperparameters'],
 			missing_freq_prior_mean=stored_model['meta_data']['all_model_kwargs']['missing_freq_priors'][0],
 			missing_freq_prior_scale=stored_model['meta_data']['all_model_kwargs']['missing_freq_priors'][1],
-			cut_points=stored_model['meta_data']['all_model_kwargs']['frequency_cut_points']
+			cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1]
 			)
 		self.vae_g2p_model.load_state(stored_model)
 	
 
 
 	def SaveModel(self,fName=None):
 		"""
```

### Comparing `VAE_G2P-0.0.5/setup.py` & `VAE_G2P-0.0.6/setup.py`

 * *Files identical despite different names*

