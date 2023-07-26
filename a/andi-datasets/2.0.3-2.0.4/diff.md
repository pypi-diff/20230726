# Comparing `tmp/andi_datasets-2.0.3.tar.gz` & `tmp/andi_datasets-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andi_datasets-2.0.3.tar", last modified: Thu Nov 10 09:24:58 2022, max compression
+gzip compressed data, was "andi_datasets-2.0.4.tar", last modified: Wed Jul 26 07:34:04 2023, max compression
```

## Comparing `andi_datasets-2.0.3.tar` & `andi_datasets-2.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 gorka     (1000) gorka     (1000)        0 2022-11-10 09:24:58.398816 andi_datasets-2.0.3/
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)     1090 2021-10-14 12:57:52.000000 andi_datasets-2.0.3/LICENSE
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)      116 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/MANIFEST.in
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)     3458 2022-11-10 09:24:58.390818 andi_datasets-2.0.3/PKG-INFO
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)     2858 2022-11-10 09:24:11.000000 andi_datasets-2.0.3/README.md
-drwxrwxrwx   0 gorka     (1000) gorka     (1000)        0 2022-11-10 09:24:57.974579 andi_datasets-2.0.3/andi_datasets/
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)       23 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/__init__.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    37716 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/_modidx.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)     6611 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/analysis.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    37525 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/datasets_challenge.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    14002 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/datasets_phenom.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    28544 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/datasets_theory.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    59029 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/models_phenom.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    17415 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/models_theory.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    59756 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/utils_challenge.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    17921 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/utils_trajectories.py
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)    12633 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/andi_datasets/utils_videos.py
-drwxrwxrwx   0 gorka     (1000) gorka     (1000)        0 2022-11-10 09:24:58.341726 andi_datasets-2.0.3/andi_datasets.egg-info/
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)     3458 2022-11-10 09:24:56.000000 andi_datasets-2.0.3/andi_datasets.egg-info/PKG-INFO
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)      651 2022-11-10 09:24:57.000000 andi_datasets-2.0.3/andi_datasets.egg-info/SOURCES.txt
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)        1 2022-11-10 09:24:56.000000 andi_datasets-2.0.3/andi_datasets.egg-info/dependency_links.txt
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)       48 2022-11-10 09:24:56.000000 andi_datasets-2.0.3/andi_datasets.egg-info/entry_points.txt
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)        1 2022-11-10 09:05:32.000000 andi_datasets-2.0.3/andi_datasets.egg-info/not-zip-safe
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)       74 2022-11-10 09:24:56.000000 andi_datasets-2.0.3/andi_datasets.egg-info/requires.txt
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)       14 2022-11-10 09:24:56.000000 andi_datasets-2.0.3/andi_datasets.egg-info/top_level.txt
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)     1076 2022-11-10 09:24:42.000000 andi_datasets-2.0.3/settings.ini
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)       38 2022-11-10 09:24:58.401924 andi_datasets-2.0.3/setup.cfg
--rwxrwxrwx   0 gorka     (1000) gorka     (1000)     2594 2022-11-10 08:59:31.000000 andi_datasets-2.0.3/setup.py
+drwxrwxr-x   0 gorka     (1000) gorka     (1000)        0 2023-07-26 07:34:04.135378 andi_datasets-2.0.4/
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)     1069 2023-06-15 14:16:22.000000 andi_datasets-2.0.4/LICENSE
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)      111 2022-11-21 15:03:44.000000 andi_datasets-2.0.4/MANIFEST.in
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)     6086 2023-07-26 07:34:04.135378 andi_datasets-2.0.4/PKG-INFO
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)     5420 2023-07-26 07:31:32.000000 andi_datasets-2.0.4/README.md
+drwxrwxr-x   0 gorka     (1000) gorka     (1000)        0 2023-07-26 07:34:04.135378 andi_datasets-2.0.4/andi_datasets/
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)       22 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/__init__.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    37598 2023-07-26 07:31:27.000000 andi_datasets-2.0.4/andi_datasets/_modidx.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)     6944 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/analysis.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    36775 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/datasets_challenge.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    13682 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/datasets_phenom.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    27927 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/datasets_theory.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    57628 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/models_phenom.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    17039 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/models_theory.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    58236 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/utils_challenge.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    17485 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/utils_trajectories.py
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)    12246 2023-07-26 07:26:44.000000 andi_datasets-2.0.4/andi_datasets/utils_videos.py
+drwxrwxr-x   0 gorka     (1000) gorka     (1000)        0 2023-07-26 07:34:04.135378 andi_datasets-2.0.4/andi_datasets.egg-info/
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)     6086 2023-07-26 07:34:04.000000 andi_datasets-2.0.4/andi_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)      651 2023-07-26 07:34:04.000000 andi_datasets-2.0.4/andi_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)        1 2023-07-26 07:34:04.000000 andi_datasets-2.0.4/andi_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)       48 2023-07-26 07:34:04.000000 andi_datasets-2.0.4/andi_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)        1 2023-01-18 07:55:56.000000 andi_datasets-2.0.4/andi_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)       79 2023-07-26 07:34:04.000000 andi_datasets-2.0.4/andi_datasets.egg-info/requires.txt
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)       14 2023-07-26 07:34:04.000000 andi_datasets-2.0.4/andi_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)     1039 2023-07-26 07:06:08.000000 andi_datasets-2.0.4/settings.ini
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)       38 2023-07-26 07:34:04.135378 andi_datasets-2.0.4/setup.cfg
+-rw-rw-r--   0 gorka     (1000) gorka     (1000)     2539 2022-11-21 15:03:44.000000 andi_datasets-2.0.4/setup.py
```

### Comparing `andi_datasets-2.0.3/LICENSE` & `andi_datasets-2.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 Gorka Muñoz
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 Gorka Muñoz
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `andi_datasets-2.0.3/andi_datasets/datasets_challenge.py` & `andi_datasets-2.0.4/andi_datasets/datasets_challenge.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,750 +1,750 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/datasets_challenge.ipynb.
-
-# %% auto 0
-__all__ = ['challenge_theory_dataset', 'challenge_phenom_dataset']
-
-# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 2
-import numpy as np
-from tqdm.auto import tqdm
-import pandas as pd
-import os
-import csv
-
-from .utils_challenge import segs_inside_fov, label_continuous_to_list, extract_ensemble, label_filter, df_to_array, get_VIP
-from .datasets_phenom import datasets_phenom
-from .datasets_theory import datasets_theory
-from .utils_trajectories import normalize
-from .utils_videos import transform_to_video, psf_width
-
-# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 5
-def challenge_theory_dataset(N:np.ndarray|int = 1000, 
-                            max_T:int = 1000,
-                            min_T:int = 10,
-                            tasks:list|int = [1, 2, 3],
-                            dimensions:list|int = [1, 2, 3],
-                            load_dataset:{'True', 'False'} = False, 
-                            save_dataset:{'True', 'False'} = False, 
-                            path_datasets:str = '', 
-                            load_labels:{'True', 'False'} = True,
-                            load_trajectories:{'True', 'False'} = False,
-                            save_trajectories:{'True', 'False'} = False, 
-                            path_trajectories:str = 'datasets/',
-                            N_save:int = 1000, 
-                            t_save:int = 1000,
-                            return_noise:{'True', 'False'} = False):  
-    ''' 
-    Creates a dataset similar to the one given by in the ANDI 1 challenge. 
-    Check the webpage of the challenge for more details. The default values
-    are similar to the ones used to generate the available dataset.
-    
-    The function returns 6 variables, three variables for the trajectories and three 
-    for the corresponding labels. Each variable is a list of three lists. Each of the
-    three lists corresponds to a given dimension, in ascending order. If one of the
-    tasks/dimensions was not calculated, the given list will be empty. 
-        
-    See the tutorials in our Github repository to learn about this function.
-    
-    Parameters
-    ----------
-        N : 
-         Number of trajectories per class (i.e.size # models x # classes). If int, all classes have same number.
-        max_T :
-         Maximum length of the trajectories in the dataset.
-        min_T :
-         Minimum length of the trajectories in the dataset.
-        tasks :
-         Task(s) of the ANDI challenge I for which datasets will be generated.
-        dimensions :
-         Dimension(s) for which trajectories will be generated. Three possible values: 1, 2 and 3.
-        load_dataset :
-         If True, the module loads existing datasets from the files task{}.txt and ref{}.txt. 
-        save_dataset :
-         If True, the module saves the datasets in a .txt following the competition format.
-        path_datasets :
-         Path from where to load the dataset.
-        load_labels :
-         If False, only loads trajectories and avoids the files refX.txt.
-        load_trajectories :
-         If True, the module loads the trajectories of an .h5 file.  
-        save_trajectories :
-         If True, the module saves a .h5 file for each model considered, with N_save trajectories and T = T_save.
-        path_trajectories :
-         Path from where to load trajectories.
-        N_save :
-         Number of trajectories to save for each exponents/model. Advise: save at the beggining
-                  a big dataset (i.e. with default t_save N_save) which allows you to load any 
-                  other combiantionof T and N.
-        t_save :
-         Length of the trajectories to be saved. See comments on N_save.   
-        return_noise :
-         If True, returns the amplitudes of the noises added to the trajectories. 
-     
-    Returns
-    -------
-        x : multiple
-         Xn (lists): trajectories
-         Yn (lists): labels
-         loc_noise_tn (lists): localization noise amplitudes
-         diff_noise_tn (lists): variance of the diffusion noise    
-    
-    '''
-    
-   
-
-    print(f'Creating a dataset for task(s) {tasks} and dimension(s) {dimensions}.')
-
-    # Checking inputs for errors
-    if isinstance(dimensions, int) or isinstance(dimensions, float):
-        dimensions = [dimensions]
-    if isinstance(tasks, int) or isinstance(tasks, float):
-        tasks = [tasks]
-
-    # Define return datasets
-    X1 = [[],[],[]]; X2 = [[],[],[]]; X3 = [[],[],[]]
-    Y1 = [[],[],[]]; Y2 = [[],[],[]]; Y3 = [[],[],[]]
-
-    if return_noise:
-        loc_noise_t1 = [[],[],[]]; loc_noise_t2 = [[],[],[]]; loc_noise_t3 = [[],[],[]]
-        diff_noise_t1 = [[],[],[]]; diff_noise_t2 = [[],[],[]]; diff_noise_t3 = [[],[],[]]
-
-    if load_dataset or save_dataset:
-        # Define name of result files, if needed
-        task1 = path_datasets+'task1.txt'; ref1 = path_datasets+'ref1.txt'
-        task2 = path_datasets+'task2.txt'; ref2 = path_datasets+'ref2.txt'
-        task3 = path_datasets+'task3.txt'; ref3 = path_datasets+'ref3.txt'
-
-    # Loading the datasets if chosen.
-    if load_dataset:            
-        for idx, (task, lab) in enumerate(zip([task1, task2, task3], [ref1, ref2, ref3])):
-            if idx+1 in tasks:
-
-                try:
-                    t = csv.reader(open(task,'r'), delimiter=';', 
-                                    lineterminator='\n',quoting=csv.QUOTE_NONNUMERIC)
-                    if load_labels:
-                        l = csv.reader(open(lab,'r'), delimiter=';', 
-                                        lineterminator='\n',quoting=csv.QUOTE_NONNUMERIC)
-                except:
-                    raise FileNotFoundError(f'File for task {idx+1} not found.')
-
-
-                if load_labels:                    
-                    for trajs, labels in zip(t, l):   
-                        if task == task1:                            
-                            X1[int(trajs[0])-1].append(trajs[1:])
-                            Y1[int(trajs[0])-1].append(labels[1])
-                        if task == task2:
-                            X2[int(trajs[0])-1].append(trajs[1:])
-                            Y2[int(trajs[0])-1].append(labels[1])
-                        if task == task3:
-                            X3[int(trajs[0])-1].append(trajs[1:])
-                            Y3[int(trajs[0])-1].append(labels[1:]) 
-                else:
-                    for trajs in t:   
-                        if task == task1:                            
-                            X1[int(trajs[0])-1].append(trajs[1:])
-                        if task == task2:
-                            X2[int(trajs[0])-1].append(trajs[1:])
-                        if task == task3:
-                            X3[int(trajs[0])-1].append(trajs[1:])
-
-                # Checking that the dataset exists in the files
-                for dim in dimensions:
-                    if task == task1 and X1[dim-1] == []:
-                        raise FileNotFoundError('Dataset for dimension '+str(dim)+' not contained in file task1.txt.')
-                    if task == task2 and X2[dim-1] == []:
-                        raise FileNotFoundError('Dataset for dimension '+str(dim)+' not contained in file task2.txt.')
-                    if task == task3 and X3[dim-1] == []:
-                        raise FileNotFoundError('Dataset for dimension '+str(dim)+' not contained in file task3.txt.')
-        if load_labels:
-            return X1, Y1, X2, Y2, X3, Y3        
-        else: 
-            return X1, X2, X3     
-
-
-    exponents = np.arange(0.05, 2.01, 0.05)
-    n_exp = len(exponents)
-    # Trajectories per model and exponent. Arbitrarely chosen to obtain balanced classes
-    n_per_model = np.ceil(1.6*N/5)
-    subdif, superdif = n_exp//2, n_exp//2+1
-    n_per_class =  np.zeros((len(datasets_theory().avail_models_name), n_exp))
-    # ctrw, attm
-    n_per_class[:2, :subdif] = np.ceil(n_per_model/subdif)
-    # fbm
-    n_per_class[2, :] = np.ceil(n_per_model/(n_exp-1))
-    n_per_class[2, exponents == 2] = 0 # FBM can't be ballistic
-    # lw
-    n_per_class[3, subdif:] = np.ceil((n_per_model/superdif)*0.8)
-    # sbm
-    n_per_class[4, :] = np.ceil(n_per_model/n_exp)
-
-    # Define return datasets
-    X1 = [[],[],[]]; X2 = [[],[],[]]; X3 = [[],[],[]]
-    Y1 = [[],[],[]]; Y2 = [[],[],[]]; Y3 = [[],[],[]]  
-
-    # Initialize the files
-    if save_dataset:
-        if 1 in tasks:
-            csv.writer(open(task1,'w'), delimiter=';', lineterminator='\n',)
-            csv.writer(open(ref1,'w'), delimiter=';', lineterminator='\n',)
-        elif 2 in tasks:
-            csv.writer(open(task2,'w'), delimiter=';', lineterminator='\n',)
-            csv.writer(open(ref2,'w'), delimiter=';',lineterminator='\n',)
-        elif 3 in tasks:
-            csv.writer(open(task3,'w'), delimiter=';', lineterminator='\n',)
-            csv.writer(open(ref3,'w'), delimiter=';',lineterminator='\n',)
-
-    for dim in dimensions:             
-        # Generate the dataset of the given dimension
-        print(f'Generating dataset for dimension {dim}.')
-        dataset = datasets_theory().create_dataset(T = max_T, N_models = n_per_class, exponents = exponents, 
-                                       dimension = dim, models = np.arange(len(datasets_theory().avail_models_name)),
-                                       load_trajectories = False, save_trajectories = False, N_save = 100,
-                                       path = path_trajectories)            
-
-        # Normalize trajectories
-        n_traj = dataset.shape[0]
-        norm_trajs = normalize(dataset[:, 2:].reshape(n_traj*dim, max_T))
-        dataset[:, 2:] = norm_trajs.reshape(dataset[:, 2:].shape)
-
-        # Save unnoisy dataset for task3
-        dataset_t3 = dataset.copy()
-
-        # Add localization error, Gaussian noise with sigma = [0.1, 0.5, 1]                
-        loc_error_amplitude = np.random.choice(np.array([0.1, 0.5, 1]), size = n_traj).repeat(dim)
-        loc_error = (np.random.randn(n_traj*dim, int(max_T)).transpose()*loc_error_amplitude).transpose()                        
-        dataset = datasets_theory().create_noisy_localization_dataset(dataset, dimension = dim, T = max_T, noise_func = loc_error)
-
-
-        # Add random diffusion coefficients            
-        trajs = dataset[:, 2:].reshape(n_traj*dim, max_T)
-        displacements = trajs[:, 1:] - trajs[:, :-1]
-        # Get new diffusion coefficients and displacements
-        diffusion_coefficients = np.random.randn(n_traj).repeat(dim)
-        new_displacements = (displacements.transpose()*diffusion_coefficients).transpose()  
-        # Generate new trajectories and add to dataset
-        new_trajs = np.cumsum(new_displacements, axis = 1)
-        new_trajs = np.concatenate((np.zeros((new_trajs.shape[0], 1)), new_trajs), axis = 1)
-        dataset[:, 2:] = new_trajs.reshape(dataset[:, 2:].shape)
-
-
-
-        # Task 1 - Anomalous exponent
-        if 1 in tasks:         
-            # Creating semi-balanced datasets
-            n_exp_max = int(np.ceil(1.1*N/n_exp))
-            for exponent in exponents:
-                dataset_exp = dataset[dataset[:, 1] == exponent].copy()
-                dataset_exp = dataset_exp[:n_exp_max, :]
-                try:
-                    dataset_1 = np.concatenate((dataset_1, dataset_exp), axis = 0) 
-                except:
-                    dataset_1 = dataset_exp
-
-            # Shuffle trajectories and noise                
-            p = np.random.permutation(dataset_1.shape[0])                
-            diffusion_coefficients_t1 = diffusion_coefficients[p].copy()
-            loc_error_amplitude_t1 = loc_error_amplitude[p].copy()
-            dataset_1 = dataset_1[p]
-
-            # Saving noise with correct number of elements
-            if return_noise:
-                loc_noise_t1[dim-1] = loc_error_amplitude_t1[:N]
-                diff_noise_t1[dim-1] = diffusion_coefficients_t1[:N]
-
-            for traj in dataset_1[:N, :]:             
-                # Cutting trajectories
-                cut_T = np.random.randint(min_T, max_T) 
-                traj_cut = datasets_theory()._cut_trajectory(traj[2:], cut_T, dim=dim).tolist()                         
-                # Saving dataset
-                X1[dim-1].append(traj_cut)
-                Y1[dim-1].append(np.around(traj[1], 2))
-                if save_dataset:                        
-                    datasets_theory()._save_row(np.append(dim, traj_cut), task1)
-                    datasets_theory()._save_row(np.append(dim, np.around([traj[1]], 2)), ref1)
-
-        # Task 2 - Diffusion model
-        if 2 in tasks:   
-            # Creating semi-balanced datasets
-            # If number of traejectories N is too small, consider at least
-            # one trajectory per model
-            n_per_model = max(1, int(1.1*N/5))                    
-            for model in range(5):
-                dataset_mod = dataset[dataset[:, 0] == model].copy()
-                dataset_mod = dataset_mod[:n_per_model, :]
-                try:
-                    dataset_2 = np.concatenate((dataset_2, dataset_mod), axis = 0) 
-                except:
-                    dataset_2 = dataset_mod
-
-            # Shuffle trajectories and noise                
-            p = np.random.permutation(dataset_2.shape[0])                
-            diffusion_coefficients_t2 = diffusion_coefficients[p].copy()
-            loc_error_amplitude_t2 = loc_error_amplitude[p].copy()
-            dataset_2 = dataset_2[p]
-            # Saving noise wityh correct number of elements
-            if return_noise:
-                loc_noise_t2[dim-1] = loc_error_amplitude_t2[:N]
-                diff_noise_t2[dim-1] = diffusion_coefficients_t2[:N]
-
-            for traj in dataset_2[:N, :]:             
-                # Cutting trajectories
-                cut_T = np.random.randint(min_T, max_T) 
-                traj_cut = datasets_theory()._cut_trajectory(traj[2:], cut_T, dim=dim).tolist() 
-                # Saving dataset   
-                X2[dim-1].append(traj_cut)
-                Y2[dim-1].append(np.around(traj[0], 2))    
-                if save_dataset:
-                    datasets_theory()._save_row(np.append(dim, traj_cut), task2)
-                    datasets_theory()._save_row(np.append(dim, traj[0]), ref2)   
-
-
-        # Task 3 - Segmentated trajectories
-        if 3 in tasks:  
-            # Create a copy of the dataset and use it to create the 
-            # segmented dataset
-            dataset_copy1 = dataset_t3.copy()
-            dataset_copy2 = dataset_t3.copy()
-
-            # Shuffling the hard way
-            order_dataset1 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
-            order_dataset2 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
-            dataset_copy1 = dataset_copy1[order_dataset1] 
-            dataset_copy2 = dataset_copy1[order_dataset2] 
-
-            seg_dataset = datasets_theory().create_segmented_dataset(dataset_copy1, dataset_copy2, dimension = dim)        
-            seg_dataset = np.c_[np.ones(n_traj)*dim, seg_dataset]     
-
-            # Checking that there are no segmented trajectories with same exponent and model 
-            # in each segment. First we compute the difference between labels
-            diff = np.abs(seg_dataset[:, 2]-seg_dataset[:, 4]) + np.abs(seg_dataset[:, 3]-seg_dataset[:, 5])
-            # Then, if there are repeated labels, we eliminate those trajectories
-            while len(np.argwhere(diff == 0)) > 0: 
-                seg_dataset = np.delete(seg_dataset, np.argwhere(diff == 0), axis = 0)
-                # If the size of the dataset is too small, we generate new segmented trajectories
-                # and add them to the dataset
-                if seg_dataset.shape[0] < N:
-
-                    # Shuffling the hard way
-                    new_order_dataset1 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
-                    new_order_dataset2 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
-                    dataset_copy1 = dataset_copy1[new_order_dataset1] 
-                    dataset_copy2 = dataset_copy1[new_order_dataset2] 
-
-                    order_dataset1 = np.concatenate((order_dataset1, new_order_dataset1))
-                    order_dataset2 = np.concatenate((order_dataset2, new_order_dataset2))
-
-                    aux_seg_dataset = datasets_theory().create_segmented_dataset(dataset_copy1, dataset_copy2, dimension = dim) 
-                    aux_seg_dataset = np.c_[np.ones(aux_seg_dataset.shape[0])*dim, aux_seg_dataset] 
-                    seg_dataset = np.concatenate((seg_dataset, aux_seg_dataset), axis = 0)
-
-                    diff = np.abs(seg_dataset[:, 2]-seg_dataset[:, 4]) + np.abs(seg_dataset[:, 3]-seg_dataset[:, 5])
-                else:
-                    break 
-
-            # Add localization error, Gaussian noise with sigma = [0.1, 0.5, 1]                
-            loc_error_amplitude_t3 = np.random.choice(np.array([0.1, 0.5, 1]), size = seg_dataset.shape[0]).repeat(dim)
-            loc_error_t3 = (np.random.randn(seg_dataset.shape[0]*dim, 200).transpose()*loc_error_amplitude_t3).transpose()
-
-            seg_dataset[:, 4:] = datasets_theory().create_noisy_localization_dataset(seg_dataset[:, 4:], 
-                                                                        dimension = dim, T = 200, 
-                                                                        noise_func = loc_error_t3)
-
-
-            # Add random diffusion coefficients            
-            trajs = seg_dataset[:, 6:].reshape(seg_dataset.shape[0]*dim, 200)
-            displacements = trajs[:, 1:] - trajs[:, :-1]
-            # Get new diffusion coefficients and displacements
-            diffusion_coefficients_t3 = np.random.randn(seg_dataset.shape[0]).repeat(dim)
-            new_displacements = (displacements.transpose()*diffusion_coefficients_t3).transpose()  
-            # Generate new trajectories and add to dataset
-            new_trajs = np.cumsum(new_displacements, axis = 1)
-            new_trajs = np.concatenate((np.zeros((new_trajs.shape[0], 1)), new_trajs), axis = 1)
-            seg_dataset[:, 6:] = new_trajs.reshape(seg_dataset[:, 6:].shape)
-
-            if return_noise:
-                loc_noise_t3[dim-1] = loc_error_amplitude_t3[:N].tolist()
-                diff_noise_t3[dim-1] = diffusion_coefficients_t3[:N].tolist()
-
-
-
-
-            X3[dim-1] = seg_dataset[:N, 6:]
-            Y3[dim-1] = seg_dataset[:N, :6]
-
-            if save_dataset:
-                for label, traj in zip(seg_dataset[:N, :6], seg_dataset[:N, 6:]):
-                    datasets_theory()._save_row(np.append(dim, traj), task3)
-                    datasets_theory()._save_row(np.around(label, 2), ref3) 
-
-
-    if return_noise:
-        return [X1, Y1, loc_noise_t1, diff_noise_t1, 
-                X2, Y2, loc_noise_t2, diff_noise_t2, 
-                X3, Y3, loc_noise_t3, diff_noise_t3] 
-    else:
-        return X1, Y1, X2, Y2, X3, Y3
-
-# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 7
-class _defaults_andi2: 
-    '''
-    This class defines the default values set for the ANDI 2 challenge.
-    '''
-    def __init__(self):        
-        # General parameters
-
-        self.T = 500                   # Length of simulated trajectories
-        self._min_T = 20               # Minimal length of output trajectories
-        self.FOV_L = 128               # Length side of the FOV (px)
-        self.L = 1.8*self.FOV_L          # Length of the simulated environment
-        self.D = 1                     # Baseline diffusion coefficient (px^2/frame)
-        self.density = 2               # Particle density   
-        self.N = 50                    # Number of particle in the whole experiment
-        self.sigma_noise = 0.12        # Variance of the localization noise
-
-        self.label_filter = lambda x: label_filter(x, window_size = 5, min_seg = 3) 
-
-# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 9
-def _get_dic_andi2(model):
-    ''' 
-    Given the number label of diffusion model, returns a default
-    dictionary of the model's parameters to be fed to create_dataset
-    The numeration is as follow:
-            1: single state
-            2: N-state
-            3: immobilization
-            4: dimerization
-            5: confinement
-            
-    Parameters
-    ----------
-    model : int in [1,6]
-        Number of the diffusion model
-    
-    Returns
-    -------
-    dic : dictionary
-        Dictionary containing the default parameters for ANDI 2 of the indicated model.
-    '''
-
-    dic = {'N': _defaults_andi2().N,
-           'T': _defaults_andi2().T,
-           'L': _defaults_andi2().L}
-
-    # alpha and D for single-state and immobilization
-    if model == 1 or model == 3:    
-        dic.update({'Ds': [_defaults_andi2().D, _defaults_andi2().D*0.01], # mean and varianve for D
-                    'alphas': np.array([np.random.rand()*(1.5-0.5)+0.5, 0.01])})
-
-    # alphas and Ds for 2-state, confinement and dimerization
-    if model == 2 or model == 4 or model == 5:            
-
-        fast_D = _defaults_andi2().D + np.random.randn()*_defaults_andi2().D*0.01
-        slow_D = fast_D*np.random.rand()*(0.1-0.01)+0.01    
-
-        alpha1 = np.random.rand()*(1.2-0.8)+0.8
-        # The second state will be at least 0.2 afar. We make sure not being 
-        # outside [0,2]        
-        alpha2 = alpha1 - (np.random.rand()*(0.6-0.2)+0.2)
-
-        dic.update({'Ds': np.array([[fast_D, 0.01],
-                                    [slow_D, 0.01]]),
-                    'alphas': np.array([[alpha1, 0.01],
-                                        [alpha2, 0.01]])})
-
-    # Particle/trap radius and ninding and unbinding probs for dimerization and immobilization
-    if model == 3 or model == 4:
-        dic.update({'Pu': 0.01,                           # Unbinding probability
-                    'Pb': 1})                             # Binding probabilitiy
-
-    if model == 1:
-        dic.update({'model': datasets_phenom().avail_models_name[0]})
-
-    if model == 2:
-        dic.update({'model': datasets_phenom().avail_models_name[1],
-                    'M': np.array([[0.99, 0.01],            # Transition Matrix
-                                   [0.01, 0.99]]),
-                    'return_state_num': True              # To get the state numeration back, , hence labels.shape = TxNx4
-                   })
-    if model == 3:
-        dic.update({'model': datasets_phenom().avail_models_name[2],
-                    'Nt': 300,            # Number of traps (density = 1 currently)
-                    'r': 0.4}             # Size of trap
-                  )
-    if model == 4:
-        dic.update({'model': datasets_phenom().avail_models_name[3],
-                    'r': 0.6,                 # Size of particles
-                    'return_state_num': True  # To get the state numeration back, hence labels.shape = TxNx4
-                   })
-
-    if model == 5:
-        dic.update({'model': datasets_phenom().avail_models_name[4],
-                    'r': 5,
-                    'Nc': 30,
-                    'trans': 0.1})
-
-    return dic
-
-# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 11
-def challenge_phenom_dataset( 
-                              experiments = 5,
-                              dics = None,
-                              repeat_exp = True,
-                              num_fovs = 20,
-                              return_timestep_labs = False,
-                              save_data = False,
-                              path = 'data/',
-                              prefix = '',
-                              get_video = False, num_vip = None, get_video_masks = False
-                                ):
-    ''' 
-    Creates a datasets with same structure as ones given in the ANDI 2 challenge. 
-    Default values for the various diffusion models have been set such as to be in the same ranges as the ones expected for the
-    challenge.
-    For details, check the ANDI 2 challenge webpage (soon).
-    
-    This function will generate as many experiments (associated to one the diffusion models) as demanded.
-    There are two ways of defining that:
-        - Give number of experiments (and optional parameters such as repeat_exp) to create. The diffusion
-        parameters are then taken from the default values are taken from datasets_phenom._defaults_andi2.
-        - Feed a list of dictionaries (dics) from which data will be generated
-    For each experiment, as many field of view as wanted can be generated        
-
-    Parameters   
-    ----------
-    experiments : int, list
-            - if int: Number of experiments to generate. Each experiment is 
-            generated from one of the available diffusion models.  
-            - if list: diffusion models to generate (starting with 1!!!!!)
-    dics : dictionary, list of dics
-            If given, uses this to set the parameters of the experiments.
-            Must be of length equal to experiments. 
-            This overrides any info about chosen models, as the model is set by the dictionary.
-    repeat_exp : bool, list
-            -> Does not enter into play if experiments is list        
-            If True: picks at random the diffusion model from the pool.
-            If False: picks the diffusion in an ordered way from the pool.
-    num_fovs : int
-            Number of field of views to get trajectories from in each experiment.
-    return_timestep_labs : bool
-            If True, the output trajectories dataframes containing also the labels alpha, D and state at each time step.        
-    save_data : bool
-        If True, saves all pertinent data.
-    path : str
-        Path where to store the data.
-    prefix : str
-        Extra prefix that can be added in front of the files' names.    
-    get_video : bool
-        If true, get as output the videos generated with Deeptrack for the generated datasets (see utils_videos for details).
-    num_vip : int
-        Number of VIP highlighted in the videos.
-    get_video_masks : bool
-        If True, get masks of videos 
-
-    Returns
-    -------
-    tuple
-        - trajs_out:
-            List of lenght (experiments x num_fovs). Each elements are is dataframe
-            containing the trajectories of a particular experiment/fov, in order of 
-            generation (i.e. [exp1_fov1, exp1_fov2, ..., exp2_fov1 ....]).
-            If return_timestep_labs = True, the dataframes also contain the labels
-            at each time step.
-        - labels_traj_out:
-            list of same length of trajs_out containing the labels of the 
-            corresponding trajectories. Each element contains a list with the 
-            labels of each trajectory, following the scheme:
-            [idx_traj, D_1, alpha_1, state_1, CP_1, D_2, alpha_2, .... state_N]
-        - labels_ens_out:
-            list of same length of trajs_out containing the ensemble labels of 
-            given experiment. See description of output matrix in 
-            utils_challenge._extract_ensemble()
-        '''
-
-
-
-    # Set prefixes for saved files
-    if save_data:
-        if not os.path.exists(path):
-            os.makedirs(path)
-        pf_labs_traj = path+prefix+'traj_labs'
-        pf_labs_ens = path+prefix+'ens_labs'
-        pf_trajs = path+prefix+'trajs'
-        pf_videos = path+prefix+'videos'
-
-    if return_timestep_labs:
-        df_list = []
-
-    # Sets the models of the experiments that will be output by the function
-    if dics is None:
-        if isinstance(experiments, int):
-            if repeat_exp: # If experiments can be repeated, we just sample randomly
-                model_exp = np.random.randint(len(datasets_phenom().avail_models_name), size = experiments)
-            else: # If not, we sampled them in an ordered way
-                if experiments >= len(datasets_phenom().avail_models_name):
-                    num_repeats = (experiments % len(datasets_phenom().avail_models_name))+1
-                else:
-                    num_repeats = 1
-                model_exp = np.tile(np.arange(len(datasets_phenom().avail_models_name)), num_repeats)[:experiments]
-            # We add one to get into non-Python numeration
-            model_exp += 1
-        else:
-            model_exp = experiments
-    # If list of dics is given, then just create a list of length = len(dics)
-    else: 
-        model_exp = [0]*len(dics)
-
-    # Output lists
-    trajs_out, labels_traj_out, labels_ens_out = [], [], []
-    for idx_experiment, model in enumerate(tqdm(model_exp)):
-
-        ''' Generate the trajectories '''
-        if dics is None:
-            dic = _get_dic_andi2(model)
-        else:
-            dic = dics[idx_experiment]
-            # Overide the info about model
-            model = datasets_phenom().avail_models_name.index(dic['model'])+1        
-        
-        trajs, labels = datasets_phenom().create_dataset(dics = dic)     
-
-        ''' Apply the FOV '''
-        for fov in range(num_fovs):
-
-            # Checking if file exist and creating an error
-            if save_data:
-                if os.path.exists(pf_labs_traj+f'_exp_{idx_experiment}_fov_{fov}.txt') or os.path.exists(pf_labs_ens+f'_exp_{idx_experiment}_fov_{fov}.txt'):
-                    raise FileExistsError(f'Target files for experiment {idx_experiment} and FOV {fov}. Delete the file or change path/prefix.')            
-
-
-
-            # We take as min/max for the fovs a 5 % distance of L
-            dist = 0.05
-            min_fov = int(dist*_defaults_andi2().L)
-            max_fov = int((1-dist)*_defaults_andi2().L)-_defaults_andi2().FOV_L
-            # sample the position of the FOV
-            fov_origin = (np.random.randint(min_fov, max_fov), np.random.randint(min_fov, max_fov))
-
-            ''' Go over trajectories in FOV (copied from utils_trajectories for efficiency) '''
-            trajs_fov, array_labels_fov, list_labels_fov, idx_segs_fov, frames_fov = [], [], [], [], []
-            idx_seg = -1
-
-            # Total frames
-            frames = np.arange(trajs.shape[0])
-            # We save the correspondance between idx in FOV and idx in trajs dataset
-            for idx, (traj, label) in enumerate(zip(trajs[:, :, :].transpose(1,0,2),
-                                                    labels[:, :, :].transpose(1,0,2))):
-                nan_segms = segs_inside_fov(traj, 
-                                            fov_origin = fov_origin,
-                                            fov_length = _defaults_andi2().FOV_L,
-                                            cutoff_length = _defaults_andi2()._min_T)
-
-                if nan_segms is not None:
-                    for idx_nan in nan_segms:  
-                        idx_seg+= 1
-                        
-
-                        seg_x = traj[idx_nan[0]:idx_nan[1], 0]
-                        seg_y = traj[idx_nan[0]:idx_nan[1], 1]
-
-
-                        trajs_fov.append(np.vstack((seg_x, seg_y)).transpose())
-                        frames_fov.append(frames[idx_nan[0]:idx_nan[1]])
-
-                        lab_seg = []
-                        for idx_lab in range(labels.shape[-1]):
-                            lab_seg.append(_defaults_andi2().label_filter(label[idx_nan[0]:idx_nan[1], idx_lab]))
-                        lab_seg = np.vstack(lab_seg).transpose()                    
-                        array_labels_fov.append(lab_seg)
-
-                        # Tranform continuous labels to list for correct output
-                        if model == 2 or model == 4: 
-                            # if multi-state or dimerization, we get rid of the label of state numbering
-                            CP, alphas, Ds, states = label_continuous_to_list(lab_seg[:, :-1])
-                        else:
-                            CP, alphas, Ds, states = label_continuous_to_list(lab_seg)
-                        
-                        # Extract final point of trajectory 
-                        T = CP[-1]
-                        CP = CP[:-1]
-                        list_gt = [idx_seg, Ds[0], alphas[0], states[0]]
-                        for gtc, gta, gtd, gts in zip(CP, alphas[1:], Ds[1:], states[1:]):
-                            list_gt += [gtc, gtd, gta, gts]
-                        # Add end point of trajectory
-                        list_gt.append(T)
-                        list_labels_fov.append(list_gt)     
-
-                        if save_data:
-                            with open(pf_labs_traj+f'_exp_{idx_experiment}_fov_{fov}.txt', 'a') as f:
-                                writer = csv.writer(f, delimiter=',', lineterminator='\n',)
-                                writer.writerow(list_gt)
-
-                        # Save index of segment with its length to latter append in the dataframe    
-                        idx_segs_fov.append(np.ones_like(seg_x)*idx_seg)             
-            
-            '''Extract ensemble trajectories''' 
-            ensemble_fov = extract_ensemble(np.concatenate(array_labels_fov)[:, -1], dic)
-
-            df_data = np.hstack((np.expand_dims(np.concatenate(idx_segs_fov), axis=1),
-                                 np.expand_dims(np.concatenate(frames_fov), axis=1).astype(int),
-                                 np.concatenate(trajs_fov)))
-            df_traj = pd.DataFrame(df_data, columns = ['traj_idx', 'frame', 'x', 'y']) 
-            
-            
-            if get_video:
-                print(f'Generating video for EXP {idx_experiment} FOV {fov}')               
-                
-                pad = -20 #  padding has to be further enough from the FOV so that the PSF 
-                          # of particles does not enter in the videos
-                array_traj_fov = df_to_array(df_traj.copy(), pad = pad)
-                min_distance = psf_width()
-                idx_vip = get_VIP(array_traj_fov, num_vip = num_vip, min_distance = min_distance, pad = pad)  
-                
-                if not save_data:
-                    pf_videos = ''                
-                
-                video_fov = transform_to_video(array_traj_fov, # see that we insert the trajectories without noise!
-                                               optics_props={
-                                                   "output_region":[fov_origin[0], fov_origin[1],
-                                                                    fov_origin[0] + _defaults_andi2().FOV_L, fov_origin[1] + _defaults_andi2().FOV_L]
-                                                },
-                                               get_vip_particles=idx_vip,
-                                               with_masks = get_video_masks,
-                                               save_video = save_data, path = pf_videos+f'_exp_{idx_experiment}_fov_{fov}.tiff')
-                try:
-                    videos_out.append(video_fov)
-                except:
-                    videos_out = [video_fov] 
-                    
-            # Add noise to the trajectories (see that this has to be done
-            # after the videos, so these are not affected by the noise).
-            df_traj.x += np.random.randn(df_traj.shape[0])*_defaults_andi2().sigma_noise 
-            df_traj.y += np.random.randn(df_traj.shape[0])*_defaults_andi2().sigma_noise 
-                    
-            if return_timestep_labs:
-                array_labels_fov = np.concatenate(array_labels_fov)
-                df_traj['alpha'] = array_labels_fov[:, 0]
-                df_traj['D'] = array_labels_fov[:, 1]
-                df_traj['state'] = array_labels_fov[:, 2]
-
-            if save_data:
-                # Trajectories                    
-                df_traj.to_csv(pf_trajs+f'_exp_{idx_experiment}_fov_{fov}.csv', index = False)
-                # Ensemble labels
-                with open(pf_labs_ens+f'_exp_{idx_experiment}_fov_{fov}.txt', 'a') as f:
-                    if model == 2: num_states = dic['alphas'].shape[0]
-                    elif model == 1: num_states = 1
-                    else: num_states = 2
-                    model_n = dic['model']
-                    f.write(f'model: {model_n}; num_state: {num_states} \n')
-                    np.savetxt(f, ensemble_fov, delimiter = ';')
-                    
-            
-            # Add data to main lists (trajectories and lists with labels)   
-            trajs_out.append(df_traj)
-            labels_traj_out.append(list_labels_fov)
-            labels_ens_out.append(ensemble_fov)
-    if get_video:
-        return trajs_out, videos_out, labels_traj_out, labels_ens_out
-    else:
-        return trajs_out, labels_traj_out, labels_ens_out
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/datasets_challenge.ipynb.
+
+# %% auto 0
+__all__ = ['challenge_theory_dataset', 'challenge_phenom_dataset']
+
+# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 2
+import numpy as np
+from tqdm.auto import tqdm
+import pandas as pd
+import os
+import csv
+
+from .utils_challenge import segs_inside_fov, label_continuous_to_list, extract_ensemble, label_filter, df_to_array, get_VIP
+from .datasets_phenom import datasets_phenom
+from .datasets_theory import datasets_theory
+from .utils_trajectories import normalize
+from .utils_videos import transform_to_video, psf_width
+
+# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 5
+def challenge_theory_dataset(N:np.ndarray|int = 1000, 
+                            max_T:int = 1000,
+                            min_T:int = 10,
+                            tasks:list|int = [1, 2, 3],
+                            dimensions:list|int = [1, 2, 3],
+                            load_dataset:{'True', 'False'} = False, 
+                            save_dataset:{'True', 'False'} = False, 
+                            path_datasets:str = '', 
+                            load_labels:{'True', 'False'} = True,
+                            load_trajectories:{'True', 'False'} = False,
+                            save_trajectories:{'True', 'False'} = False, 
+                            path_trajectories:str = 'datasets/',
+                            N_save:int = 1000, 
+                            t_save:int = 1000,
+                            return_noise:{'True', 'False'} = False):  
+    ''' 
+    Creates a dataset similar to the one given by in the ANDI 1 challenge. 
+    Check the webpage of the challenge for more details. The default values
+    are similar to the ones used to generate the available dataset.
+    
+    The function returns 6 variables, three variables for the trajectories and three 
+    for the corresponding labels. Each variable is a list of three lists. Each of the
+    three lists corresponds to a given dimension, in ascending order. If one of the
+    tasks/dimensions was not calculated, the given list will be empty. 
+        
+    See the tutorials in our Github repository to learn about this function.
+    
+    Parameters
+    ----------
+        N : 
+         Number of trajectories per class (i.e.size # models x # classes). If int, all classes have same number.
+        max_T :
+         Maximum length of the trajectories in the dataset.
+        min_T :
+         Minimum length of the trajectories in the dataset.
+        tasks :
+         Task(s) of the ANDI challenge I for which datasets will be generated.
+        dimensions :
+         Dimension(s) for which trajectories will be generated. Three possible values: 1, 2 and 3.
+        load_dataset :
+         If True, the module loads existing datasets from the files task{}.txt and ref{}.txt. 
+        save_dataset :
+         If True, the module saves the datasets in a .txt following the competition format.
+        path_datasets :
+         Path from where to load the dataset.
+        load_labels :
+         If False, only loads trajectories and avoids the files refX.txt.
+        load_trajectories :
+         If True, the module loads the trajectories of an .h5 file.  
+        save_trajectories :
+         If True, the module saves a .h5 file for each model considered, with N_save trajectories and T = T_save.
+        path_trajectories :
+         Path from where to load trajectories.
+        N_save :
+         Number of trajectories to save for each exponents/model. Advise: save at the beggining
+                  a big dataset (i.e. with default t_save N_save) which allows you to load any 
+                  other combiantionof T and N.
+        t_save :
+         Length of the trajectories to be saved. See comments on N_save.   
+        return_noise :
+         If True, returns the amplitudes of the noises added to the trajectories. 
+     
+    Returns
+    -------
+        x : multiple
+         Xn (lists): trajectories
+         Yn (lists): labels
+         loc_noise_tn (lists): localization noise amplitudes
+         diff_noise_tn (lists): variance of the diffusion noise    
+    
+    '''
+    
+   
+
+    print(f'Creating a dataset for task(s) {tasks} and dimension(s) {dimensions}.')
+
+    # Checking inputs for errors
+    if isinstance(dimensions, int) or isinstance(dimensions, float):
+        dimensions = [dimensions]
+    if isinstance(tasks, int) or isinstance(tasks, float):
+        tasks = [tasks]
+
+    # Define return datasets
+    X1 = [[],[],[]]; X2 = [[],[],[]]; X3 = [[],[],[]]
+    Y1 = [[],[],[]]; Y2 = [[],[],[]]; Y3 = [[],[],[]]
+
+    if return_noise:
+        loc_noise_t1 = [[],[],[]]; loc_noise_t2 = [[],[],[]]; loc_noise_t3 = [[],[],[]]
+        diff_noise_t1 = [[],[],[]]; diff_noise_t2 = [[],[],[]]; diff_noise_t3 = [[],[],[]]
+
+    if load_dataset or save_dataset:
+        # Define name of result files, if needed
+        task1 = path_datasets+'task1.txt'; ref1 = path_datasets+'ref1.txt'
+        task2 = path_datasets+'task2.txt'; ref2 = path_datasets+'ref2.txt'
+        task3 = path_datasets+'task3.txt'; ref3 = path_datasets+'ref3.txt'
+
+    # Loading the datasets if chosen.
+    if load_dataset:            
+        for idx, (task, lab) in enumerate(zip([task1, task2, task3], [ref1, ref2, ref3])):
+            if idx+1 in tasks:
+
+                try:
+                    t = csv.reader(open(task,'r'), delimiter=';', 
+                                    lineterminator='\n',quoting=csv.QUOTE_NONNUMERIC)
+                    if load_labels:
+                        l = csv.reader(open(lab,'r'), delimiter=';', 
+                                        lineterminator='\n',quoting=csv.QUOTE_NONNUMERIC)
+                except:
+                    raise FileNotFoundError(f'File for task {idx+1} not found.')
+
+
+                if load_labels:                    
+                    for trajs, labels in zip(t, l):   
+                        if task == task1:                            
+                            X1[int(trajs[0])-1].append(trajs[1:])
+                            Y1[int(trajs[0])-1].append(labels[1])
+                        if task == task2:
+                            X2[int(trajs[0])-1].append(trajs[1:])
+                            Y2[int(trajs[0])-1].append(labels[1])
+                        if task == task3:
+                            X3[int(trajs[0])-1].append(trajs[1:])
+                            Y3[int(trajs[0])-1].append(labels[1:]) 
+                else:
+                    for trajs in t:   
+                        if task == task1:                            
+                            X1[int(trajs[0])-1].append(trajs[1:])
+                        if task == task2:
+                            X2[int(trajs[0])-1].append(trajs[1:])
+                        if task == task3:
+                            X3[int(trajs[0])-1].append(trajs[1:])
+
+                # Checking that the dataset exists in the files
+                for dim in dimensions:
+                    if task == task1 and X1[dim-1] == []:
+                        raise FileNotFoundError('Dataset for dimension '+str(dim)+' not contained in file task1.txt.')
+                    if task == task2 and X2[dim-1] == []:
+                        raise FileNotFoundError('Dataset for dimension '+str(dim)+' not contained in file task2.txt.')
+                    if task == task3 and X3[dim-1] == []:
+                        raise FileNotFoundError('Dataset for dimension '+str(dim)+' not contained in file task3.txt.')
+        if load_labels:
+            return X1, Y1, X2, Y2, X3, Y3        
+        else: 
+            return X1, X2, X3     
+
+
+    exponents = np.arange(0.05, 2.01, 0.05)
+    n_exp = len(exponents)
+    # Trajectories per model and exponent. Arbitrarely chosen to obtain balanced classes
+    n_per_model = np.ceil(1.6*N/5)
+    subdif, superdif = n_exp//2, n_exp//2+1
+    n_per_class =  np.zeros((len(datasets_theory().avail_models_name), n_exp))
+    # ctrw, attm
+    n_per_class[:2, :subdif] = np.ceil(n_per_model/subdif)
+    # fbm
+    n_per_class[2, :] = np.ceil(n_per_model/(n_exp-1))
+    n_per_class[2, exponents == 2] = 0 # FBM can't be ballistic
+    # lw
+    n_per_class[3, subdif:] = np.ceil((n_per_model/superdif)*0.8)
+    # sbm
+    n_per_class[4, :] = np.ceil(n_per_model/n_exp)
+
+    # Define return datasets
+    X1 = [[],[],[]]; X2 = [[],[],[]]; X3 = [[],[],[]]
+    Y1 = [[],[],[]]; Y2 = [[],[],[]]; Y3 = [[],[],[]]  
+
+    # Initialize the files
+    if save_dataset:
+        if 1 in tasks:
+            csv.writer(open(task1,'w'), delimiter=';', lineterminator='\n',)
+            csv.writer(open(ref1,'w'), delimiter=';', lineterminator='\n',)
+        elif 2 in tasks:
+            csv.writer(open(task2,'w'), delimiter=';', lineterminator='\n',)
+            csv.writer(open(ref2,'w'), delimiter=';',lineterminator='\n',)
+        elif 3 in tasks:
+            csv.writer(open(task3,'w'), delimiter=';', lineterminator='\n',)
+            csv.writer(open(ref3,'w'), delimiter=';',lineterminator='\n',)
+
+    for dim in dimensions:             
+        # Generate the dataset of the given dimension
+        print(f'Generating dataset for dimension {dim}.')
+        dataset = datasets_theory().create_dataset(T = max_T, N_models = n_per_class, exponents = exponents, 
+                                       dimension = dim, models = np.arange(len(datasets_theory().avail_models_name)),
+                                       load_trajectories = False, save_trajectories = False, N_save = 100,
+                                       path = path_trajectories)            
+
+        # Normalize trajectories
+        n_traj = dataset.shape[0]
+        norm_trajs = normalize(dataset[:, 2:].reshape(n_traj*dim, max_T))
+        dataset[:, 2:] = norm_trajs.reshape(dataset[:, 2:].shape)
+
+        # Save unnoisy dataset for task3
+        dataset_t3 = dataset.copy()
+
+        # Add localization error, Gaussian noise with sigma = [0.1, 0.5, 1]                
+        loc_error_amplitude = np.random.choice(np.array([0.1, 0.5, 1]), size = n_traj).repeat(dim)
+        loc_error = (np.random.randn(n_traj*dim, int(max_T)).transpose()*loc_error_amplitude).transpose()                        
+        dataset = datasets_theory().create_noisy_localization_dataset(dataset, dimension = dim, T = max_T, noise_func = loc_error)
+
+
+        # Add random diffusion coefficients            
+        trajs = dataset[:, 2:].reshape(n_traj*dim, max_T)
+        displacements = trajs[:, 1:] - trajs[:, :-1]
+        # Get new diffusion coefficients and displacements
+        diffusion_coefficients = np.random.randn(n_traj).repeat(dim)
+        new_displacements = (displacements.transpose()*diffusion_coefficients).transpose()  
+        # Generate new trajectories and add to dataset
+        new_trajs = np.cumsum(new_displacements, axis = 1)
+        new_trajs = np.concatenate((np.zeros((new_trajs.shape[0], 1)), new_trajs), axis = 1)
+        dataset[:, 2:] = new_trajs.reshape(dataset[:, 2:].shape)
+
+
+
+        # Task 1 - Anomalous exponent
+        if 1 in tasks:         
+            # Creating semi-balanced datasets
+            n_exp_max = int(np.ceil(1.1*N/n_exp))
+            for exponent in exponents:
+                dataset_exp = dataset[dataset[:, 1] == exponent].copy()
+                dataset_exp = dataset_exp[:n_exp_max, :]
+                try:
+                    dataset_1 = np.concatenate((dataset_1, dataset_exp), axis = 0) 
+                except:
+                    dataset_1 = dataset_exp
+
+            # Shuffle trajectories and noise                
+            p = np.random.permutation(dataset_1.shape[0])                
+            diffusion_coefficients_t1 = diffusion_coefficients[p].copy()
+            loc_error_amplitude_t1 = loc_error_amplitude[p].copy()
+            dataset_1 = dataset_1[p]
+
+            # Saving noise with correct number of elements
+            if return_noise:
+                loc_noise_t1[dim-1] = loc_error_amplitude_t1[:N]
+                diff_noise_t1[dim-1] = diffusion_coefficients_t1[:N]
+
+            for traj in dataset_1[:N, :]:             
+                # Cutting trajectories
+                cut_T = np.random.randint(min_T, max_T) 
+                traj_cut = datasets_theory()._cut_trajectory(traj[2:], cut_T, dim=dim).tolist()                         
+                # Saving dataset
+                X1[dim-1].append(traj_cut)
+                Y1[dim-1].append(np.around(traj[1], 2))
+                if save_dataset:                        
+                    datasets_theory()._save_row(np.append(dim, traj_cut), task1)
+                    datasets_theory()._save_row(np.append(dim, np.around([traj[1]], 2)), ref1)
+
+        # Task 2 - Diffusion model
+        if 2 in tasks:   
+            # Creating semi-balanced datasets
+            # If number of traejectories N is too small, consider at least
+            # one trajectory per model
+            n_per_model = max(1, int(1.1*N/5))                    
+            for model in range(5):
+                dataset_mod = dataset[dataset[:, 0] == model].copy()
+                dataset_mod = dataset_mod[:n_per_model, :]
+                try:
+                    dataset_2 = np.concatenate((dataset_2, dataset_mod), axis = 0) 
+                except:
+                    dataset_2 = dataset_mod
+
+            # Shuffle trajectories and noise                
+            p = np.random.permutation(dataset_2.shape[0])                
+            diffusion_coefficients_t2 = diffusion_coefficients[p].copy()
+            loc_error_amplitude_t2 = loc_error_amplitude[p].copy()
+            dataset_2 = dataset_2[p]
+            # Saving noise wityh correct number of elements
+            if return_noise:
+                loc_noise_t2[dim-1] = loc_error_amplitude_t2[:N]
+                diff_noise_t2[dim-1] = diffusion_coefficients_t2[:N]
+
+            for traj in dataset_2[:N, :]:             
+                # Cutting trajectories
+                cut_T = np.random.randint(min_T, max_T) 
+                traj_cut = datasets_theory()._cut_trajectory(traj[2:], cut_T, dim=dim).tolist() 
+                # Saving dataset   
+                X2[dim-1].append(traj_cut)
+                Y2[dim-1].append(np.around(traj[0], 2))    
+                if save_dataset:
+                    datasets_theory()._save_row(np.append(dim, traj_cut), task2)
+                    datasets_theory()._save_row(np.append(dim, traj[0]), ref2)   
+
+
+        # Task 3 - Segmentated trajectories
+        if 3 in tasks:  
+            # Create a copy of the dataset and use it to create the 
+            # segmented dataset
+            dataset_copy1 = dataset_t3.copy()
+            dataset_copy2 = dataset_t3.copy()
+
+            # Shuffling the hard way
+            order_dataset1 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
+            order_dataset2 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
+            dataset_copy1 = dataset_copy1[order_dataset1] 
+            dataset_copy2 = dataset_copy1[order_dataset2] 
+
+            seg_dataset = datasets_theory().create_segmented_dataset(dataset_copy1, dataset_copy2, dimension = dim)        
+            seg_dataset = np.c_[np.ones(n_traj)*dim, seg_dataset]     
+
+            # Checking that there are no segmented trajectories with same exponent and model 
+            # in each segment. First we compute the difference between labels
+            diff = np.abs(seg_dataset[:, 2]-seg_dataset[:, 4]) + np.abs(seg_dataset[:, 3]-seg_dataset[:, 5])
+            # Then, if there are repeated labels, we eliminate those trajectories
+            while len(np.argwhere(diff == 0)) > 0: 
+                seg_dataset = np.delete(seg_dataset, np.argwhere(diff == 0), axis = 0)
+                # If the size of the dataset is too small, we generate new segmented trajectories
+                # and add them to the dataset
+                if seg_dataset.shape[0] < N:
+
+                    # Shuffling the hard way
+                    new_order_dataset1 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
+                    new_order_dataset2 = np.random.choice(np.arange(n_traj), n_traj, replace = False)        
+                    dataset_copy1 = dataset_copy1[new_order_dataset1] 
+                    dataset_copy2 = dataset_copy1[new_order_dataset2] 
+
+                    order_dataset1 = np.concatenate((order_dataset1, new_order_dataset1))
+                    order_dataset2 = np.concatenate((order_dataset2, new_order_dataset2))
+
+                    aux_seg_dataset = datasets_theory().create_segmented_dataset(dataset_copy1, dataset_copy2, dimension = dim) 
+                    aux_seg_dataset = np.c_[np.ones(aux_seg_dataset.shape[0])*dim, aux_seg_dataset] 
+                    seg_dataset = np.concatenate((seg_dataset, aux_seg_dataset), axis = 0)
+
+                    diff = np.abs(seg_dataset[:, 2]-seg_dataset[:, 4]) + np.abs(seg_dataset[:, 3]-seg_dataset[:, 5])
+                else:
+                    break 
+
+            # Add localization error, Gaussian noise with sigma = [0.1, 0.5, 1]                
+            loc_error_amplitude_t3 = np.random.choice(np.array([0.1, 0.5, 1]), size = seg_dataset.shape[0]).repeat(dim)
+            loc_error_t3 = (np.random.randn(seg_dataset.shape[0]*dim, 200).transpose()*loc_error_amplitude_t3).transpose()
+
+            seg_dataset[:, 4:] = datasets_theory().create_noisy_localization_dataset(seg_dataset[:, 4:], 
+                                                                        dimension = dim, T = 200, 
+                                                                        noise_func = loc_error_t3)
+
+
+            # Add random diffusion coefficients            
+            trajs = seg_dataset[:, 6:].reshape(seg_dataset.shape[0]*dim, 200)
+            displacements = trajs[:, 1:] - trajs[:, :-1]
+            # Get new diffusion coefficients and displacements
+            diffusion_coefficients_t3 = np.random.randn(seg_dataset.shape[0]).repeat(dim)
+            new_displacements = (displacements.transpose()*diffusion_coefficients_t3).transpose()  
+            # Generate new trajectories and add to dataset
+            new_trajs = np.cumsum(new_displacements, axis = 1)
+            new_trajs = np.concatenate((np.zeros((new_trajs.shape[0], 1)), new_trajs), axis = 1)
+            seg_dataset[:, 6:] = new_trajs.reshape(seg_dataset[:, 6:].shape)
+
+            if return_noise:
+                loc_noise_t3[dim-1] = loc_error_amplitude_t3[:N].tolist()
+                diff_noise_t3[dim-1] = diffusion_coefficients_t3[:N].tolist()
+
+
+
+
+            X3[dim-1] = seg_dataset[:N, 6:]
+            Y3[dim-1] = seg_dataset[:N, :6]
+
+            if save_dataset:
+                for label, traj in zip(seg_dataset[:N, :6], seg_dataset[:N, 6:]):
+                    datasets_theory()._save_row(np.append(dim, traj), task3)
+                    datasets_theory()._save_row(np.around(label, 2), ref3) 
+
+
+    if return_noise:
+        return [X1, Y1, loc_noise_t1, diff_noise_t1, 
+                X2, Y2, loc_noise_t2, diff_noise_t2, 
+                X3, Y3, loc_noise_t3, diff_noise_t3] 
+    else:
+        return X1, Y1, X2, Y2, X3, Y3
+
+# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 7
+class _defaults_andi2: 
+    '''
+    This class defines the default values set for the ANDI 2 challenge.
+    '''
+    def __init__(self):        
+        # General parameters
+
+        self.T = 500                   # Length of simulated trajectories
+        self._min_T = 20               # Minimal length of output trajectories
+        self.FOV_L = 128               # Length side of the FOV (px)
+        self.L = 1.8*self.FOV_L          # Length of the simulated environment
+        self.D = 1                     # Baseline diffusion coefficient (px^2/frame)
+        self.density = 2               # Particle density   
+        self.N = 50                    # Number of particle in the whole experiment
+        self.sigma_noise = 0.12        # Variance of the localization noise
+
+        self.label_filter = lambda x: label_filter(x, window_size = 5, min_seg = 3) 
+
+# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 9
+def _get_dic_andi2(model):
+    ''' 
+    Given the number label of diffusion model, returns a default
+    dictionary of the model's parameters to be fed to create_dataset
+    The numeration is as follow:
+            1: single state
+            2: N-state
+            3: immobilization
+            4: dimerization
+            5: confinement
+            
+    Parameters
+    ----------
+    model : int in [1,6]
+        Number of the diffusion model
+    
+    Returns
+    -------
+    dic : dictionary
+        Dictionary containing the default parameters for ANDI 2 of the indicated model.
+    '''
+
+    dic = {'N': _defaults_andi2().N,
+           'T': _defaults_andi2().T,
+           'L': _defaults_andi2().L}
+
+    # alpha and D for single-state and immobilization
+    if model == 1 or model == 3:    
+        dic.update({'Ds': [_defaults_andi2().D, _defaults_andi2().D*0.01], # mean and varianve for D
+                    'alphas': np.array([np.random.rand()*(1.5-0.5)+0.5, 0.01])})
+
+    # alphas and Ds for 2-state, confinement and dimerization
+    if model == 2 or model == 4 or model == 5:            
+
+        fast_D = _defaults_andi2().D + np.random.randn()*_defaults_andi2().D*0.01
+        slow_D = fast_D*np.random.rand()*(0.1-0.01)+0.01    
+
+        alpha1 = np.random.rand()*(1.2-0.8)+0.8
+        # The second state will be at least 0.2 afar. We make sure not being 
+        # outside [0,2]        
+        alpha2 = alpha1 - (np.random.rand()*(0.6-0.2)+0.2)
+
+        dic.update({'Ds': np.array([[fast_D, 0.01],
+                                    [slow_D, 0.01]]),
+                    'alphas': np.array([[alpha1, 0.01],
+                                        [alpha2, 0.01]])})
+
+    # Particle/trap radius and ninding and unbinding probs for dimerization and immobilization
+    if model == 3 or model == 4:
+        dic.update({'Pu': 0.01,                           # Unbinding probability
+                    'Pb': 1})                             # Binding probabilitiy
+
+    if model == 1:
+        dic.update({'model': datasets_phenom().avail_models_name[0]})
+
+    if model == 2:
+        dic.update({'model': datasets_phenom().avail_models_name[1],
+                    'M': np.array([[0.99, 0.01],            # Transition Matrix
+                                   [0.01, 0.99]]),
+                    'return_state_num': True              # To get the state numeration back, , hence labels.shape = TxNx4
+                   })
+    if model == 3:
+        dic.update({'model': datasets_phenom().avail_models_name[2],
+                    'Nt': 300,            # Number of traps (density = 1 currently)
+                    'r': 0.4}             # Size of trap
+                  )
+    if model == 4:
+        dic.update({'model': datasets_phenom().avail_models_name[3],
+                    'r': 0.6,                 # Size of particles
+                    'return_state_num': True  # To get the state numeration back, hence labels.shape = TxNx4
+                   })
+
+    if model == 5:
+        dic.update({'model': datasets_phenom().avail_models_name[4],
+                    'r': 5,
+                    'Nc': 30,
+                    'trans': 0.1})
+
+    return dic
+
+# %% ../source_nbs/lib_nbs/datasets_challenge.ipynb 11
+def challenge_phenom_dataset( 
+                              experiments = 5,
+                              dics = None,
+                              repeat_exp = True,
+                              num_fovs = 20,
+                              return_timestep_labs = False,
+                              save_data = False,
+                              path = 'data/',
+                              prefix = '',
+                              get_video = False, num_vip = None, get_video_masks = False
+                                ):
+    ''' 
+    Creates a datasets with same structure as ones given in the ANDI 2 challenge. 
+    Default values for the various diffusion models have been set such as to be in the same ranges as the ones expected for the
+    challenge.
+    For details, check the ANDI 2 challenge webpage (soon).
+    
+    This function will generate as many experiments (associated to one the diffusion models) as demanded.
+    There are two ways of defining that:
+        - Give number of experiments (and optional parameters such as repeat_exp) to create. The diffusion
+        parameters are then taken from the default values are taken from datasets_phenom._defaults_andi2.
+        - Feed a list of dictionaries (dics) from which data will be generated
+    For each experiment, as many field of view as wanted can be generated        
+
+    Parameters   
+    ----------
+    experiments : int, list
+            - if int: Number of experiments to generate. Each experiment is 
+            generated from one of the available diffusion models.  
+            - if list: diffusion models to generate (starting with 1!!!!!)
+    dics : dictionary, list of dics
+            If given, uses this to set the parameters of the experiments.
+            Must be of length equal to experiments. 
+            This overrides any info about chosen models, as the model is set by the dictionary.
+    repeat_exp : bool, list
+            -> Does not enter into play if experiments is list        
+            If True: picks at random the diffusion model from the pool.
+            If False: picks the diffusion in an ordered way from the pool.
+    num_fovs : int
+            Number of field of views to get trajectories from in each experiment.
+    return_timestep_labs : bool
+            If True, the output trajectories dataframes containing also the labels alpha, D and state at each time step.        
+    save_data : bool
+        If True, saves all pertinent data.
+    path : str
+        Path where to store the data.
+    prefix : str
+        Extra prefix that can be added in front of the files' names.    
+    get_video : bool
+        If true, get as output the videos generated with Deeptrack for the generated datasets (see utils_videos for details).
+    num_vip : int
+        Number of VIP highlighted in the videos.
+    get_video_masks : bool
+        If True, get masks of videos 
+
+    Returns
+    -------
+    tuple
+        - trajs_out:
+            List of lenght (experiments x num_fovs). Each elements are is dataframe
+            containing the trajectories of a particular experiment/fov, in order of 
+            generation (i.e. [exp1_fov1, exp1_fov2, ..., exp2_fov1 ....]).
+            If return_timestep_labs = True, the dataframes also contain the labels
+            at each time step.
+        - labels_traj_out:
+            list of same length of trajs_out containing the labels of the 
+            corresponding trajectories. Each element contains a list with the 
+            labels of each trajectory, following the scheme:
+            [idx_traj, D_1, alpha_1, state_1, CP_1, D_2, alpha_2, .... state_N]
+        - labels_ens_out:
+            list of same length of trajs_out containing the ensemble labels of 
+            given experiment. See description of output matrix in 
+            utils_challenge._extract_ensemble()
+        '''
+
+
+
+    # Set prefixes for saved files
+    if save_data:
+        if not os.path.exists(path):
+            os.makedirs(path)
+        pf_labs_traj = path+prefix+'traj_labs'
+        pf_labs_ens = path+prefix+'ens_labs'
+        pf_trajs = path+prefix+'trajs'
+        pf_videos = path+prefix+'videos'
+
+    if return_timestep_labs:
+        df_list = []
+
+    # Sets the models of the experiments that will be output by the function
+    if dics is None:
+        if isinstance(experiments, int):
+            if repeat_exp: # If experiments can be repeated, we just sample randomly
+                model_exp = np.random.randint(len(datasets_phenom().avail_models_name), size = experiments)
+            else: # If not, we sampled them in an ordered way
+                if experiments >= len(datasets_phenom().avail_models_name):
+                    num_repeats = (experiments % len(datasets_phenom().avail_models_name))+1
+                else:
+                    num_repeats = 1
+                model_exp = np.tile(np.arange(len(datasets_phenom().avail_models_name)), num_repeats)[:experiments]
+            # We add one to get into non-Python numeration
+            model_exp += 1
+        else:
+            model_exp = experiments
+    # If list of dics is given, then just create a list of length = len(dics)
+    else: 
+        model_exp = [0]*len(dics)
+
+    # Output lists
+    trajs_out, labels_traj_out, labels_ens_out = [], [], []
+    for idx_experiment, model in enumerate(tqdm(model_exp)):
+
+        ''' Generate the trajectories '''
+        if dics is None:
+            dic = _get_dic_andi2(model)
+        else:
+            dic = dics[idx_experiment]
+            # Overide the info about model
+            model = datasets_phenom().avail_models_name.index(dic['model'])+1        
+        
+        trajs, labels = datasets_phenom().create_dataset(dics = dic)     
+
+        ''' Apply the FOV '''
+        for fov in range(num_fovs):
+
+            # Checking if file exist and creating an error
+            if save_data:
+                if os.path.exists(pf_labs_traj+f'_exp_{idx_experiment}_fov_{fov}.txt') or os.path.exists(pf_labs_ens+f'_exp_{idx_experiment}_fov_{fov}.txt'):
+                    raise FileExistsError(f'Target files for experiment {idx_experiment} and FOV {fov}. Delete the file or change path/prefix.')            
+
+
+
+            # We take as min/max for the fovs a 5 % distance of L
+            dist = 0.05
+            min_fov = int(dist*_defaults_andi2().L)
+            max_fov = int((1-dist)*_defaults_andi2().L)-_defaults_andi2().FOV_L
+            # sample the position of the FOV
+            fov_origin = (np.random.randint(min_fov, max_fov), np.random.randint(min_fov, max_fov))
+
+            ''' Go over trajectories in FOV (copied from utils_trajectories for efficiency) '''
+            trajs_fov, array_labels_fov, list_labels_fov, idx_segs_fov, frames_fov = [], [], [], [], []
+            idx_seg = -1
+
+            # Total frames
+            frames = np.arange(trajs.shape[0])
+            # We save the correspondance between idx in FOV and idx in trajs dataset
+            for idx, (traj, label) in enumerate(zip(trajs[:, :, :].transpose(1,0,2),
+                                                    labels[:, :, :].transpose(1,0,2))):
+                nan_segms = segs_inside_fov(traj, 
+                                            fov_origin = fov_origin,
+                                            fov_length = _defaults_andi2().FOV_L,
+                                            cutoff_length = _defaults_andi2()._min_T)
+
+                if nan_segms is not None:
+                    for idx_nan in nan_segms:  
+                        idx_seg+= 1
+                        
+
+                        seg_x = traj[idx_nan[0]:idx_nan[1], 0]
+                        seg_y = traj[idx_nan[0]:idx_nan[1], 1]
+
+
+                        trajs_fov.append(np.vstack((seg_x, seg_y)).transpose())
+                        frames_fov.append(frames[idx_nan[0]:idx_nan[1]])
+
+                        lab_seg = []
+                        for idx_lab in range(labels.shape[-1]):
+                            lab_seg.append(_defaults_andi2().label_filter(label[idx_nan[0]:idx_nan[1], idx_lab]))
+                        lab_seg = np.vstack(lab_seg).transpose()                    
+                        array_labels_fov.append(lab_seg)
+
+                        # Tranform continuous labels to list for correct output
+                        if model == 2 or model == 4: 
+                            # if multi-state or dimerization, we get rid of the label of state numbering
+                            CP, alphas, Ds, states = label_continuous_to_list(lab_seg[:, :-1])
+                        else:
+                            CP, alphas, Ds, states = label_continuous_to_list(lab_seg)
+                        
+                        # Extract final point of trajectory 
+                        T = CP[-1]
+                        CP = CP[:-1]
+                        list_gt = [idx_seg, Ds[0], alphas[0], states[0]]
+                        for gtc, gta, gtd, gts in zip(CP, alphas[1:], Ds[1:], states[1:]):
+                            list_gt += [gtc, gtd, gta, gts]
+                        # Add end point of trajectory
+                        list_gt.append(T)
+                        list_labels_fov.append(list_gt)     
+
+                        if save_data:
+                            with open(pf_labs_traj+f'_exp_{idx_experiment}_fov_{fov}.txt', 'a') as f:
+                                writer = csv.writer(f, delimiter=',', lineterminator='\n',)
+                                writer.writerow(list_gt)
+
+                        # Save index of segment with its length to latter append in the dataframe    
+                        idx_segs_fov.append(np.ones_like(seg_x)*idx_seg)             
+            
+            '''Extract ensemble trajectories''' 
+            ensemble_fov = extract_ensemble(np.concatenate(array_labels_fov)[:, -1], dic)
+
+            df_data = np.hstack((np.expand_dims(np.concatenate(idx_segs_fov), axis=1),
+                                 np.expand_dims(np.concatenate(frames_fov), axis=1).astype(int),
+                                 np.concatenate(trajs_fov)))
+            df_traj = pd.DataFrame(df_data, columns = ['traj_idx', 'frame', 'x', 'y']) 
+            
+            
+            if get_video:
+                print(f'Generating video for EXP {idx_experiment} FOV {fov}')               
+                
+                pad = -20 #  padding has to be further enough from the FOV so that the PSF 
+                          # of particles does not enter in the videos
+                array_traj_fov = df_to_array(df_traj.copy(), pad = pad)
+                min_distance = psf_width()
+                idx_vip = get_VIP(array_traj_fov, num_vip = num_vip, min_distance = min_distance, pad = pad)  
+                
+                if not save_data:
+                    pf_videos = ''                
+                
+                video_fov = transform_to_video(array_traj_fov, # see that we insert the trajectories without noise!
+                                               optics_props={
+                                                   "output_region":[fov_origin[0], fov_origin[1],
+                                                                    fov_origin[0] + _defaults_andi2().FOV_L, fov_origin[1] + _defaults_andi2().FOV_L]
+                                                },
+                                               get_vip_particles=idx_vip,
+                                               with_masks = get_video_masks,
+                                               save_video = save_data, path = pf_videos+f'_exp_{idx_experiment}_fov_{fov}.tiff')
+                try:
+                    videos_out.append(video_fov)
+                except:
+                    videos_out = [video_fov] 
+                    
+            # Add noise to the trajectories (see that this has to be done
+            # after the videos, so these are not affected by the noise).
+            df_traj.x += np.random.randn(df_traj.shape[0])*_defaults_andi2().sigma_noise 
+            df_traj.y += np.random.randn(df_traj.shape[0])*_defaults_andi2().sigma_noise 
+                    
+            if return_timestep_labs:
+                array_labels_fov = np.concatenate(array_labels_fov)
+                df_traj['alpha'] = array_labels_fov[:, 0]
+                df_traj['D'] = array_labels_fov[:, 1]
+                df_traj['state'] = array_labels_fov[:, 2]
+
+            if save_data:
+                # Trajectories                    
+                df_traj.to_csv(pf_trajs+f'_exp_{idx_experiment}_fov_{fov}.csv', index = False)
+                # Ensemble labels
+                with open(pf_labs_ens+f'_exp_{idx_experiment}_fov_{fov}.txt', 'a') as f:
+                    if model == 2: num_states = dic['alphas'].shape[0]
+                    elif model == 1: num_states = 1
+                    else: num_states = 2
+                    model_n = dic['model']
+                    f.write(f'model: {model_n}; num_state: {num_states} \n')
+                    np.savetxt(f, ensemble_fov, delimiter = ';')
+                    
+            
+            # Add data to main lists (trajectories and lists with labels)   
+            trajs_out.append(df_traj)
+            labels_traj_out.append(list_labels_fov)
+            labels_ens_out.append(ensemble_fov)
+    if get_video:
+        return trajs_out, videos_out, labels_traj_out, labels_ens_out
+    else:
+        return trajs_out, labels_traj_out, labels_ens_out
```

### Comparing `andi_datasets-2.0.3/andi_datasets/datasets_phenom.py` & `andi_datasets-2.0.4/andi_datasets/datasets_phenom.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,320 +1,320 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/datasets_phenom.ipynb.
-
-# %% auto 0
-__all__ = ['datasets_phenom']
-
-# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 2
-from .models_phenom import models_phenom
-
-import inspect
-import numpy as np
-import pandas as pd
-import csv
-from tqdm.auto import tqdm
-import copy
-
-import os
-import warnings
-
-# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 5
-class datasets_phenom():
-    def __init__(self,
-                models_class = models_phenom()):
-            ''' 
-            This class generates, saves and loads datasets of trajectories simulated from various phenomenological diffusion models (available at andi_datasets.models_phenom). 
-            '''
-            self.models_class = models_class
-            self._get_models()
-        
-    def _get_models(self):        
-        '''Loads the available models from the subclass'''
-
-        available_models = inspect.getmembers(self.models_class, inspect.ismethod)      
-        available_models = available_models[1:][::-1] # we need this to get rid of the init
-        self.avail_models_name = [x[0] for x in available_models]
-        self.avail_models_func = [x[1] for x in available_models]
-        
-    def _get_inputs_models(self, model, get_default_values = False):
-        
-        model_f = self.avail_models_func[self.avail_models_name.index(model)] 
-        defaults = inspect.getfullargspec(model_f).defaults
-        params = inspect.getfullargspec(model_f).args[1:]
-        if get_default_values:
-            return params, defaults
-        else:
-            return params
-        
-    def _get_states(self):
-        ''' Definition of the possible states found in the ANDI 2 challenge (phenom) and their 
-        assigned label:
-        0: immobile; 1: confined; 2: brownian; 3: anomalous '''
-        
-        self._states = ['immobile', 'confined', 'brownian', 'anomalous']
-        
-
-# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 7
-class datasets_phenom(datasets_phenom):
-                
-    def create_dataset(self,
-                       dics: list|dict|bool = False,
-                       T: None|int = None,
-                       N_model: None|int = None,  
-                       path: str = '',
-                       save: bool = False,
-                       load: bool = False):
-        ''' 
-        Given a list of dictionaries, generates trajectories of the demanded properties.
-        The only compulsory input for every dictionary is 'model', i.e. the model from which 
-        trajectories must be generated. The rest of inputs are optional.
-        You can see the input parameters of the different models in andi_datasets.models_phenom,
-        This function checks and handles the input dataset and the manages both the creation,
-        loading and saving of trajectories.
-        
-        Parameters
-        ----------
-        dics : list, dictionary, bool
-            - if list or dictionary: the function generates trajectories with the properties stated in each dictionary.
-            - if bool: the function generates trajectories with default parameters set for the ANDI 2 challenge (phenom) for every available diffusion model.
-        T : int, None
-            - if int: overrides the values of trajectory length in the dictionaries.
-            - if None: uses the trajectory length values in the dictionaries. 
-            Caution: the minim T of all dictionaries will be considered!
-        N_model : int, None
-            - if int: overrides the values of number of trajectories in the dictionaries.
-            - if None: uses the number of trajectories in the dictionaries
-        save : bool
-            If True, saves the generated dataset (see self._save_trajectories).
-        load : bool
-            If True, loads a dataset from path (see self._load_trajectories).
-        path : str
-            Path from where to save or load the dataset.
-            
-        Returns
-        -------
-        tuple
-            - trajs (array TxNx2): particles' position. N considers here the sum of all trajectories generated from the input dictionaries. 
-            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels) 
-        '''
-        
-        self.T = T
-        self.N_model = N_model
-        self.path = path
-        self.dics = dics
-        
-        '''Managing dictionaries'''
-        # If the input is a single dictionary, transform it to list
-        if isinstance(self.dics, dict): self.dics = [self.dics]
-        # if dics is False, we select trajectories from all models with default values
-        if self.dics is False: self.dics = [{'model': model} for model in self.avail_models_name]
-
-                    
-        '''Managing folders of the datasets'''  
-        self.save = save
-        self.load = load
-        if self.save or self.load:                
-            if self.load:
-                self.save = False            
-            if not os.path.exists(self.path) and self.load:
-                raise FileNotFoundError('The directory from where you want to load the dataset does not exist')                
-            if not os.path.exists(self.path) and self.save:
-                os.makedirs(self.path) 
-                
-                
-        '''Create trajectories'''
-        trajs, labels = self._create_trajectories()
-        
-        return trajs, labels                        
-
-# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 12
-class datasets_phenom(datasets_phenom):   
-    
-    def _create_trajectories(self): 
-        ''' 
-        Given a list of dictionaries, generates trajectories of the demanded properties.
-        First checks in the .csv of each demanded model if a dataset of similar properties exists. 
-        If it does, it loads it from the corresponding file.       
-        
-        Returns
-        ----------
-        tuple
-            data_t  array containing the generated trajectories
-            data_l  array containing the corresponding labels.
-        '''
-
-        for dic in copy.deepcopy(self.dics):
-            
-            df, dataset_idx = self._inspect_dic(dic)
-            
-            # If the dataset does not yet exists
-            if dataset_idx is False:
-                # Retrieve name and function of diffusion model
-                model_f = self.avail_models_func[self.avail_models_name.index(dic['model'])]
-                # Create dictionary with only arguments
-                dic_args = dict(dic); dic_args.pop('model')
-                
-                trajs, labels = model_f(**dic_args)
-                
-                # Save the trajectories if asked
-                if self.save:
-                    self._save_trajectories(trajs = trajs,
-                                            labels = labels,
-                                            dic = dic, 
-                                            df = df,
-                                            dataset_idx = dataset_idx,
-                                            path = self.path)                    
-            else:
-                trajs, labels = self._load_trajectories(model_name = dic['model'],
-                                                        dataset_idx = dataset_idx,
-                                                        path = self.path)
-                
-            # Stack dataset
-            try:
-                data_t = np.hstack((data_t, trajs))                    
-                data_l = np.hstack((data_l, labels))
-            except:
-                data_t = trajs
-                data_l = labels
-                    
-        return data_t, data_l  
-    
-    def _save_trajectories(self, trajs, labels, dic, df, dataset_idx, path):
-        ''' 
-        Given a set of trajectories and labels, saves two things:        
-            - In the .csv corresponding to the demanded model, all the input parameters of the generated dataset. This allows to keed that of what was created before.
-            - In a .npy file, the trajectories and labels generated.
-        '''
-        
-        file_name = path+dic['model']+'_'+str(df.shape[0])+'.npy'
-        
-        # Save information in CSV handler
-        df = df.append(dic, ignore_index = True) 
-        #print(dic)
-        #df = pd.concat([df, 
-        #                pd.DataFrame(dic)], 
-        #               ignore_index=True)        
-        df.to_csv(path+dic['model']+'.csv')
-        
-        # Save trajectories and labels
-        data = np.dstack((trajs, labels))
-        np.save(file_name, data)
-        
-    def _load_trajectories(self, model_name, dataset_idx, path):
-        ''' 
-        Given the path for a dataset, loads the trajectories and labels
-        '''
-        
-        file_name = path+model_name+'_'+str(dataset_idx)+'.npy'
-        data = np.load(file_name)
-        return data[:, :, :2], data[:, :  , 2:]
-    
-
-# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 21
-class datasets_phenom(datasets_phenom):   
-
-    def _inspect_dic(self, dic):
-        '''        
-        Checks the information of the input dictionaries so that they fulfil the constraints of the program , completes missing information
-        with default values and then decides about loading/saving depending on parameters.
-        
-        Parameters
-        ----------
-        dic : dict
-            Dictionary with the information of the trajectories we want to generate
-        
-        Returns
-        -----------
-        tuple
-            df: dataframe collecting the information of the dataset to load.
-            dataset_idx: location in the previous dataframe of the particular dataset we want to generate.
-            
-        '''        
-            
-        # Add time and number of trajectories information
-        if self.N_model is not None:
-            dic['N'] = self.N_model
-        if self.T is not None:
-            dic['T'] = self.T
-
-        # Check if CSV with information of dataset exists. If not, create it
-        model_m = dic['model']
-        model_f = self.avail_models_func[self.avail_models_name.index(model_m)]    
-        # Check arguments and defaults from model's function            
-        args = inspect.getfullargspec(model_f).args[1:]
-        defaults = inspect.getfullargspec(model_f).defaults
-        try:
-            df = pd.read_csv(self.path+model_m+'.csv', index_col=0)
-        except:                
-            # convert to dataframe and add model
-            df = pd.DataFrame(columns = args+['model'])   
-        # Assign missing keys in dic with default values
-        for arg, default in zip(args, defaults):
-            if arg not in dic.keys():
-                dic[arg] = default
-
-        # Check if updated keys of dic equal keys of csv.
-        if set(list(df.keys())) != set(list(dic.keys())):
-            raise ValueError('Input model dictionary does not match models properties')
-
-        # Check if the dataset already exists:
-        df_conditions = df.copy()
-        # Nones in dataframes are transformed into Nans. We change back this here
-        # but instead of putting None, we put False.
-        df_conditions = df_conditions.where(pd.notnull(df_conditions), False)
-        for key in dic:
-            # Transforming Nones to False in variables dictionaries (see problem with df just above) 
-            if dic[key] is None: dic[key] = False
-            # We need to transform it to str to do a fair comparison between matrices (e.g. transition matrix, Ds, alphas,...)
-            df_conditions = df_conditions.loc[(df_conditions[key].astype(str) == str(dic[key]))]
-            if len(df_conditions.index) == 0:                
-                break
-        
-        
-        # If dataset exists
-        if len(df_conditions.index) > 0:
-            # if the dataset exists and save was True, do not save but load
-            if self.save:
-                wrn_str = f'The dataset you want to save already exists (file: {model_m}_{df_conditions.index[0]}.npy). Switching to Load mode.'
-                warnings.warn(wrn_str)
-                dataset_idx = df_conditions.index[0] 
-            elif self.load:
-                dataset_idx = df_conditions.index[0]
-            else:
-                dataset_idx = False                 
-
-        # If dataset does no exists
-        else:         
-            if self.load:
-                raise ValueError('The dataset you want to load does not exist.')
-            else: # If the dataset does not exist, append empty string.
-                # This allows to mix saving and loading
-                dataset_idx = False
-                
-        return df, dataset_idx
-
-# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 34
-class datasets_phenom(datasets_phenom):  
-    def _get_args(self, model, return_defaults = False):
-        ''' 
-        Given the name of a diffusion model, return its inputs arguments.
-        
-        Parameters
-        ----------
-        model : str
-            Name of the diffusion model (see self.available_models_name)
-        return_defaults : bool
-            If True, the function will also return the default values of each input argument.
-            
-        Returns
-        -------
-        tuple
-            args (list): list of input arguments.
-            defaults (optional, list): list of default value for the input arguments.
-        '''
-        model_f = self.avail_models_func[self.avail_models_name.index(model)]    
-        # Check arguments and defaults from model's function            
-        args = inspect.getfullargspec(model_f).args[1:]
-        defaults = inspect.getfullargspec(model_f).defaults
-        if return_defaults:
-            return args, defaults
-        else:
-            return args
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/datasets_phenom.ipynb.
+
+# %% auto 0
+__all__ = ['datasets_phenom']
+
+# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 2
+from .models_phenom import models_phenom
+
+import inspect
+import numpy as np
+import pandas as pd
+import csv
+from tqdm.auto import tqdm
+import copy
+
+import os
+import warnings
+
+# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 5
+class datasets_phenom():
+    def __init__(self,
+                models_class = models_phenom()):
+            ''' 
+            This class generates, saves and loads datasets of trajectories simulated from various phenomenological diffusion models (available at andi_datasets.models_phenom). 
+            '''
+            self.models_class = models_class
+            self._get_models()
+        
+    def _get_models(self):        
+        '''Loads the available models from the subclass'''
+
+        available_models = inspect.getmembers(self.models_class, inspect.ismethod)      
+        available_models = available_models[1:][::-1] # we need this to get rid of the init
+        self.avail_models_name = [x[0] for x in available_models]
+        self.avail_models_func = [x[1] for x in available_models]
+        
+    def _get_inputs_models(self, model, get_default_values = False):
+        
+        model_f = self.avail_models_func[self.avail_models_name.index(model)] 
+        defaults = inspect.getfullargspec(model_f).defaults
+        params = inspect.getfullargspec(model_f).args[1:]
+        if get_default_values:
+            return params, defaults
+        else:
+            return params
+        
+    def _get_states(self):
+        ''' Definition of the possible states found in the ANDI 2 challenge (phenom) and their 
+        assigned label:
+        0: immobile; 1: confined; 2: brownian; 3: anomalous '''
+        
+        self._states = ['immobile', 'confined', 'brownian', 'anomalous']
+        
+
+# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 7
+class datasets_phenom(datasets_phenom):
+                
+    def create_dataset(self,
+                       dics: list|dict|bool = False,
+                       T: None|int = None,
+                       N_model: None|int = None,  
+                       path: str = '',
+                       save: bool = False,
+                       load: bool = False):
+        ''' 
+        Given a list of dictionaries, generates trajectories of the demanded properties.
+        The only compulsory input for every dictionary is 'model', i.e. the model from which 
+        trajectories must be generated. The rest of inputs are optional.
+        You can see the input parameters of the different models in andi_datasets.models_phenom,
+        This function checks and handles the input dataset and the manages both the creation,
+        loading and saving of trajectories.
+        
+        Parameters
+        ----------
+        dics : list, dictionary, bool
+            - if list or dictionary: the function generates trajectories with the properties stated in each dictionary.
+            - if bool: the function generates trajectories with default parameters set for the ANDI 2 challenge (phenom) for every available diffusion model.
+        T : int, None
+            - if int: overrides the values of trajectory length in the dictionaries.
+            - if None: uses the trajectory length values in the dictionaries. 
+            Caution: the minim T of all dictionaries will be considered!
+        N_model : int, None
+            - if int: overrides the values of number of trajectories in the dictionaries.
+            - if None: uses the number of trajectories in the dictionaries
+        save : bool
+            If True, saves the generated dataset (see self._save_trajectories).
+        load : bool
+            If True, loads a dataset from path (see self._load_trajectories).
+        path : str
+            Path from where to save or load the dataset.
+            
+        Returns
+        -------
+        tuple
+            - trajs (array TxNx2): particles' position. N considers here the sum of all trajectories generated from the input dictionaries. 
+            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels) 
+        '''
+        
+        self.T = T
+        self.N_model = N_model
+        self.path = path
+        self.dics = dics
+        
+        '''Managing dictionaries'''
+        # If the input is a single dictionary, transform it to list
+        if isinstance(self.dics, dict): self.dics = [self.dics]
+        # if dics is False, we select trajectories from all models with default values
+        if self.dics is False: self.dics = [{'model': model} for model in self.avail_models_name]
+
+                    
+        '''Managing folders of the datasets'''  
+        self.save = save
+        self.load = load
+        if self.save or self.load:                
+            if self.load:
+                self.save = False            
+            if not os.path.exists(self.path) and self.load:
+                raise FileNotFoundError('The directory from where you want to load the dataset does not exist')                
+            if not os.path.exists(self.path) and self.save:
+                os.makedirs(self.path) 
+                
+                
+        '''Create trajectories'''
+        trajs, labels = self._create_trajectories()
+        
+        return trajs, labels                        
+
+# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 12
+class datasets_phenom(datasets_phenom):   
+    
+    def _create_trajectories(self): 
+        ''' 
+        Given a list of dictionaries, generates trajectories of the demanded properties.
+        First checks in the .csv of each demanded model if a dataset of similar properties exists. 
+        If it does, it loads it from the corresponding file.       
+        
+        Returns
+        ----------
+        tuple
+            data_t  array containing the generated trajectories
+            data_l  array containing the corresponding labels.
+        '''
+
+        for dic in copy.deepcopy(self.dics):
+            
+            df, dataset_idx = self._inspect_dic(dic)
+            
+            # If the dataset does not yet exists
+            if dataset_idx is False:
+                # Retrieve name and function of diffusion model
+                model_f = self.avail_models_func[self.avail_models_name.index(dic['model'])]
+                # Create dictionary with only arguments
+                dic_args = dict(dic); dic_args.pop('model')
+                
+                trajs, labels = model_f(**dic_args)
+                
+                # Save the trajectories if asked
+                if self.save:
+                    self._save_trajectories(trajs = trajs,
+                                            labels = labels,
+                                            dic = dic, 
+                                            df = df,
+                                            dataset_idx = dataset_idx,
+                                            path = self.path)                    
+            else:
+                trajs, labels = self._load_trajectories(model_name = dic['model'],
+                                                        dataset_idx = dataset_idx,
+                                                        path = self.path)
+                
+            # Stack dataset
+            try:
+                data_t = np.hstack((data_t, trajs))                    
+                data_l = np.hstack((data_l, labels))
+            except:
+                data_t = trajs
+                data_l = labels
+                    
+        return data_t, data_l  
+    
+    def _save_trajectories(self, trajs, labels, dic, df, dataset_idx, path):
+        ''' 
+        Given a set of trajectories and labels, saves two things:        
+            - In the .csv corresponding to the demanded model, all the input parameters of the generated dataset. This allows to keed that of what was created before.
+            - In a .npy file, the trajectories and labels generated.
+        '''
+        
+        file_name = path+dic['model']+'_'+str(df.shape[0])+'.npy'
+        
+        # Save information in CSV handler
+        df = df.append(dic, ignore_index = True) 
+        #print(dic)
+        #df = pd.concat([df, 
+        #                pd.DataFrame(dic)], 
+        #               ignore_index=True)        
+        df.to_csv(path+dic['model']+'.csv')
+        
+        # Save trajectories and labels
+        data = np.dstack((trajs, labels))
+        np.save(file_name, data)
+        
+    def _load_trajectories(self, model_name, dataset_idx, path):
+        ''' 
+        Given the path for a dataset, loads the trajectories and labels
+        '''
+        
+        file_name = path+model_name+'_'+str(dataset_idx)+'.npy'
+        data = np.load(file_name)
+        return data[:, :, :2], data[:, :  , 2:]
+    
+
+# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 21
+class datasets_phenom(datasets_phenom):   
+
+    def _inspect_dic(self, dic):
+        '''        
+        Checks the information of the input dictionaries so that they fulfil the constraints of the program , completes missing information
+        with default values and then decides about loading/saving depending on parameters.
+        
+        Parameters
+        ----------
+        dic : dict
+            Dictionary with the information of the trajectories we want to generate
+        
+        Returns
+        -----------
+        tuple
+            df: dataframe collecting the information of the dataset to load.
+            dataset_idx: location in the previous dataframe of the particular dataset we want to generate.
+            
+        '''        
+            
+        # Add time and number of trajectories information
+        if self.N_model is not None:
+            dic['N'] = self.N_model
+        if self.T is not None:
+            dic['T'] = self.T
+
+        # Check if CSV with information of dataset exists. If not, create it
+        model_m = dic['model']
+        model_f = self.avail_models_func[self.avail_models_name.index(model_m)]    
+        # Check arguments and defaults from model's function            
+        args = inspect.getfullargspec(model_f).args[1:]
+        defaults = inspect.getfullargspec(model_f).defaults
+        try:
+            df = pd.read_csv(self.path+model_m+'.csv', index_col=0)
+        except:                
+            # convert to dataframe and add model
+            df = pd.DataFrame(columns = args+['model'])   
+        # Assign missing keys in dic with default values
+        for arg, default in zip(args, defaults):
+            if arg not in dic.keys():
+                dic[arg] = default
+
+        # Check if updated keys of dic equal keys of csv.
+        if set(list(df.keys())) != set(list(dic.keys())):
+            raise ValueError('Input model dictionary does not match models properties')
+
+        # Check if the dataset already exists:
+        df_conditions = df.copy()
+        # Nones in dataframes are transformed into Nans. We change back this here
+        # but instead of putting None, we put False.
+        df_conditions = df_conditions.where(pd.notnull(df_conditions), False)
+        for key in dic:
+            # Transforming Nones to False in variables dictionaries (see problem with df just above) 
+            if dic[key] is None: dic[key] = False
+            # We need to transform it to str to do a fair comparison between matrices (e.g. transition matrix, Ds, alphas,...)
+            df_conditions = df_conditions.loc[(df_conditions[key].astype(str) == str(dic[key]))]
+            if len(df_conditions.index) == 0:                
+                break
+        
+        
+        # If dataset exists
+        if len(df_conditions.index) > 0:
+            # if the dataset exists and save was True, do not save but load
+            if self.save:
+                wrn_str = f'The dataset you want to save already exists (file: {model_m}_{df_conditions.index[0]}.npy). Switching to Load mode.'
+                warnings.warn(wrn_str)
+                dataset_idx = df_conditions.index[0] 
+            elif self.load:
+                dataset_idx = df_conditions.index[0]
+            else:
+                dataset_idx = False                 
+
+        # If dataset does no exists
+        else:         
+            if self.load:
+                raise ValueError('The dataset you want to load does not exist.')
+            else: # If the dataset does not exist, append empty string.
+                # This allows to mix saving and loading
+                dataset_idx = False
+                
+        return df, dataset_idx
+
+# %% ../source_nbs/lib_nbs/datasets_phenom.ipynb 34
+class datasets_phenom(datasets_phenom):  
+    def _get_args(self, model, return_defaults = False):
+        ''' 
+        Given the name of a diffusion model, return its inputs arguments.
+        
+        Parameters
+        ----------
+        model : str
+            Name of the diffusion model (see self.available_models_name)
+        return_defaults : bool
+            If True, the function will also return the default values of each input argument.
+            
+        Returns
+        -------
+        tuple
+            args (list): list of input arguments.
+            defaults (optional, list): list of default value for the input arguments.
+        '''
+        model_f = self.avail_models_func[self.avail_models_name.index(model)]    
+        # Check arguments and defaults from model's function            
+        args = inspect.getfullargspec(model_f).args[1:]
+        defaults = inspect.getfullargspec(model_f).defaults
+        if return_defaults:
+            return args, defaults
+        else:
+            return args
```

### Comparing `andi_datasets-2.0.3/andi_datasets/datasets_theory.py` & `andi_datasets-2.0.4/andi_datasets/datasets_theory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,575 +1,575 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/datasets_theory.ipynb.
-
-# %% auto 0
-__all__ = ['datasets_theory']
-
-# %% ../source_nbs/lib_nbs/datasets_theory.ipynb 3
-import numpy as np
-import os
-import inspect
-import h5py
-from tqdm.auto import trange
-import csv
-
-# %% ../source_nbs/lib_nbs/datasets_theory.ipynb 4
-from .utils_trajectories import normalize
-from .models_theory import models_theory as models_theory
-
-# %% ../source_nbs/lib_nbs/datasets_theory.ipynb 6
-class datasets_theory():
-     
-    def __init__(self):        
-        '''
-        This class generates, saves and loads datasets of theoretical trajectories simulated 
-        from various diffusion models (available at andi_datasets.models_theory). 
-        '''
-        self._dimension = 1
-        self._get_models()
-        
-    def _get_models(self):        
-        '''Loading subclass of models'''
-        if self._dimension == 1:
-            self._models = models_theory._oneD()
-        elif self._dimension == 2:
-            self._models = models_theory._twoD()
-        elif self._dimension == 3:
-            self._models = models_theory._threeD()
-        else:
-            raise ValueError('Our current understanding of the physical world is three dimensional and so are the diffusion models available in this class')
-                
-        available_models = inspect.getmembers(self._models, inspect.ismethod)      
-        self.avail_models_name = [x[0] for x in available_models]
-        self.avail_models_func = [x[1] for x in available_models]
-    
-    def create_dataset(self, T, N_models, exponents, models,
-                       dimension = 1,
-                       save_trajectories = False, load_trajectories = False, 
-                       path = 'datasets/',
-                       N_save = 1000, t_save = 1000):        
-        ''' 
-        Creates a dataset of trajectories via the theoretical models defined in `.models_theory`. Check our tutorials for use cases of this function.
-        
-        Parameters
-        ----------
-        T : int
-            Length of the trajectories.   
-        N_models : int, numpy.array
-            - if int, number of trajectories per class (i.e. exponent and model) in the dataset.
-            - if numpy.array, number of trajectories per classes: size (number of models)x(number of classes)    
-        exponents : float, array
-            Anomalous exponents to include in the dataset. Allows for two digit precision.
-        models : bool, int, list
-            Labels of the models to include in the dataset. 
-            Correspodance between models and labels is given by self.label_correspodance, defined at init.
-            If int/list, choose the given models. If False, choose all of them.
-        dimensions : int
-            Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
-        save_trajectories : bool
-            If True, the module saves a .h5 file for each model considered, with N_save trajectories 
-            and T = T_save.
-        load_trajectories : bool
-            If True, the module loads the trajectories of an .h5 file.
-        path : str
-            Path to the folder where to save/load the trajectories dataset.
-        N_save : int
-            Number of trajectories to save for each exponents/model. 
-            Advise: save at the beggining a big dataset (t_save ~ 1e3 and N_save ~ 1e4) 
-            which then allows you to load any other combiantion of T and N_models.
-        t_save : int
-            Length of the trajectories to be saved. See comments on N_save.                
-        
-        Returns
-        -------
-        numpy.array
-                - Dataset of trajectories of lenght Nx(T+2), with the following structure:
-                    o First column: model label 
-                    o Second column: value of the anomalous exponent
-                    o 2:T columns: trajectories
-        '''
-                    
-        '''Managing probable errors in inputs'''
-        if T < 2:
-            raise ValueError('The time of the trajectories has to be bigger than 1.')       
-        if isinstance(exponents, int) or isinstance(exponents, float):
-            exponents = [exponents]
-        
-        '''Managing folders of the datasets'''       
-        if save_trajectories or load_trajectories:                
-            if load_trajectories:
-                save_trajectories = False            
-            if not os.path.exists(path) and load_trajectories:
-                raise FileNotFoundError('The directory from where you want to load the dataset does not exist')                
-            if not os.path.exists(path) and save_trajectories:
-                os.makedirs(path)  
-                
-        '''Establish dimensions and corresponding models'''
-        self._dimension = dimension
-        self._get_models()
-                
-        '''Managing models to load'''       
-        # Load from a list of models
-        if isinstance(models, list): 
-            self._models_name = [self.avail_models_name[idx] for idx in models]     
-            self._models_func = [self.avail_models_func[idx] for idx in models]
-        # Load from a single model
-        elif isinstance(models, int) and not isinstance(models, bool):
-            self._models_name = [self.avail_models_name[models]]
-            self._models_func = [self.avail_models_func[models]]
-        # Load all available models
-        else: 
-            self._models_name =  self.avail_models_name
-            self._models_func =  self.avail_models_func
-            
-        '''Managing number of trajectory per class:
-            - Defines array num_class as a function of N'''                            
-        if isinstance(N_models, int): 
-            n_per_class = N_models*np.ones((len(self._models_name), len(exponents)))
-            
-        elif type(N_models).__module__ == np.__name__: 
-            if len(self._models_name) != N_models.shape[0] or len(exponents) != N_models.shape[1]:
-                raise ValueError('Mismatch between the dimensions of N and the number of different classes.'+
-                                 f'N must be either an int (balanced classes) or an array of length {len(models)}x'
-                                 f'{len(exponents)} (inbalaced classes).') 
-            n_per_class = N_models
-        else:
-            raise TypeError('Type of variable N not recognized.')
-                    
-        '''Defining default values for saved datasets''' 
-        N_save = np.ones_like(n_per_class)*N_save
-        # If the number of class of a given class is bigger than N_save, we
-        # change the value of N_save for that particular class.
-        N_save = np.max([N_save, n_per_class], axis = 0)      
-                
-        ''' Loading/Saving/Creating datasets'''
-        if load_trajectories:
-            data_models = self._load_trajectories(T = T,
-                                                 exponents = exponents,
-                                                 models_name = self._models_name,
-                                                 dimension = self._dimension,
-                                                 n_per_class = n_per_class,
-                                                 path = path,
-                                                 N_save = N_save,
-                                                 t_save = t_save)
-        elif save_trajectories:
-            self._save_trajectories(exponents = exponents,
-                                   dimension = self._dimension,
-                                   models_name = self._models_name,
-                                   models_func = self._models_func,
-                                   path = path, 
-                                   n_per_class = n_per_class,
-                                   N_save = N_save,
-                                   t_save = t_save)
-            
-            data_models = self._load_trajectories(T = T,
-                                                 exponents = exponents,
-                                                 dimension = self._dimension,
-                                                 models_name = self._models_name,                                                 
-                                                 n_per_class = n_per_class,
-                                                 path = path,
-                                                 N_save = N_save,
-                                                 t_save = t_save)
-            
-        else:           
-            data_models = self._create_trajectories(T = T,                                                   
-                                                   exponents = exponents, 
-                                                   dimension = self._dimension,
-                                                   models_name = self._models_name,
-                                                   models_func = self._models_func,
-                                                   n_per_class = n_per_class)       
-            
-        return data_models
-    
-    def _load_trajectories(self, T, exponents, dimension, 
-                                models_name, n_per_class, 
-                                path, N_save = 1000, t_save = 1000):
-        ''' Load trajectories from a h5py file of the given path. The name of the datasets in the
-        file have the following structure: 
-            '(exponent with 2 digit_precision)_T_(lenght of trajectories in the dataset)_N_(number of trajectories in the dataset)'
-            
-        Arguments: 
-            :T (int):
-                - length of the trajectories.   
-            :exponents (array):
-                - anomalous exponents to include in the dataset. Allows for two digit precision.
-            :dimension (int):
-                - Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
-            :models_name (list of str):
-                - names of the models to include in the output dataset. 
-            :n_per_class:
-                - number of trajectories to consider per exponent/model.
-            :path (str):
-                - path to the folder from where to load the trajectories dataset.
-            :t_save (int):
-                - length of the trajectories in the datasets to load.
-            :N_save (array):
-                - number of trajectories contained in the datasets to load.                  
-        Return:
-            :dataset (numpy.array):
-                - Dataset of trajectories of lenght (number of models)x(T+2), with the following structure:
-                    o First column: model label 
-                    o Second column: value of the anomalous exponent
-                    o 2:T columns: trajectories'''
-                    
-        '''Establish dimensions and corresponding models'''
-        self._dimension = dimension
-        self._get_models()
-            
-        
-        if isinstance(models_name, int):
-            models_name = [models_name]
-               
-        for idx_m, name in enumerate(models_name):        
-            hf = h5py.File(path+name+'.h5', 'r+')
-            
-            for idx_e, exp  in enumerate(exponents):
-                
-                name_dataset = f'{exp:.2f}_T_{t_save}_N_'+ \
-                                str(int(N_save[idx_m, idx_e]))+f'_dim_{self._dimension}'  
-                
-                n = int(n_per_class[idx_m, idx_e])
-                if n == 0:
-                    continue
-                
-                try:
-                    data = (hf.get(name_dataset)[()][:n,:self._dimension*T]) 
-                except:
-                    raise TypeError('The dataset you want to load does not exist.')
-                    
-                
-                data = self._label_trajectories(trajs = data, model_name = name, exponent = exp)                
-                            
-                if idx_e + idx_m == 0:
-                    dataset = data
-                else:
-                    dataset = np.concatenate((dataset, data), axis = 0) 
-        return dataset
-     
-    def _save_trajectories(self, exponents, models_name, models_func, path, n_per_class,
-                          N_save = 1000, t_save = 1000, dimension = 1):
-        ''' Saves a dataset for the exponents and models considered. 
-        Arguments:   
-            :exponents (array):
-                - anomalous exponents to include in the dataset. Allows for two digit precision.
-            :models_name (list of str):
-                - names of the models to include in the output dataset. 
-            :models_func (list of funcs):
-                - function generating the models to include in the output dataset. 
-            :path (str):
-                - path to the folder where to save the trajectories dataset.
-            :t_save (int):
-                - length of the trajectories to save in the datasets.
-            :N_save (array):
-                - number of trajectories to include in the datasets saved.
-            :dimension (int):
-                - Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
-        No return           '''     
-    
-        '''Establish dimensions and corresponding models'''
-        self._dimension = dimension
-        self._get_models()        
-        
-        for idx_m, (name, func) in enumerate(zip(models_name, models_func)):
-            
-            if os.path.isfile(path+name+'.h5'):
-                action = 'r+'
-            else:
-                action = 'w'
-            with h5py.File(path+name+'.h5', action) as hf:
-                
-                for idx_e, exp in enumerate(exponents): 
-                    if n_per_class[idx_m, idx_e] == 0:
-                        continue
-                    
-                    n = int(N_save[idx_m, idx_e])                    
-                    name_dataset = f'{exp:.2f}_T_{t_save}_N_{n}_dim_{self._dimension}' 
-                    
-                    if name_dataset not in hf:  
-                        
-                        data = np.zeros((n, self._dimension*t_save))                           
-                        # TQDM variables
-                        tq = trange(n)
-                        tq.set_postfix(saving = True, model = name, exponent = exp)
-                        for i in tq:
-                            data[i, :] = func(t_save, exp)                           
-                            
-                        hf.create_dataset(name_dataset, data=data)
-                        
-                    else:
-                        print(f'The dataset for {name} with exponent {round(exp,3)}'
-                                +' already exists, no need of saving it again.')
-            
-        
-    def _create_trajectories(self, T, exponents, dimension, models_name, models_func, n_per_class):  
-        ''' create a dataset for the exponents and models considered. 
-        Arguments:  
-            :T (int):
-                - length of the trajectories.   
-            :exponents (array):
-                - anomalous exponents to include in the dataset. Allows for two digit precision.
-            :dimension (int):
-                - Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
-            :models_name (list of str):
-                - names of the models to include in the output dataset. 
-            :models_func (list of funcs):
-                - function generating the models to include in the output dataset. 
-            :n_per_class:
-                - number of trajectories to consider per exponent/model. 
-        Return:
-            :dataset (numpy.array):
-                - Dataset of trajectories of lenght (number of models)x(T+2), with the following structure:
-                    o First column: model label.
-                    o Second column: value of the anomalous exponent.
-                    o 2:T columns: trajectories.'''
-            
-        for idx_m, (name, func) in enumerate(zip(models_name, models_func)):
-            for idx_e, exp in enumerate(exponents):
-                
-                
-                n = int(n_per_class[idx_m, idx_e])
-                data = np.zeros((n, self._dimension*T))  
-                for i in range(n):
-                    data[i, :] = func(T, exp)
-                    
-                data = self._label_trajectories(trajs = data, model_name = name, exponent = exp)   
-                
-                if idx_e + idx_m == 0:
-                    dataset = data
-                else:
-                    dataset = np.concatenate((dataset, data), axis = 0)
-                
-        return dataset
-                
-            
-    def _label_trajectories(self, trajs, model_name, exponent):
-        ''' Labels given trajectories given the corresponding label for the model and exponent.
-        For models, the label correspond to the position of the model in self.avail_models_name.
-        For exponents, the label if the value of the exponent.
-        Arguments:
-            :trajs (numpy array):
-                - trajectories to label
-            :model_name (str):
-                - name of the model from which the trajectories are coming from.
-            :exponent (float):
-                - Anomalous exponent of the trajectories. 
-        Return:
-            :trajs (numpy array):
-                - Labelled trajectoreis, with the following structure:
-                    o First column: model label
-                    o Second columnd: exponent label
-                    o Rest of the array: trajectory.   '''
-        
-        label_model = self.avail_models_name.index(model_name)          
-         
-        labels_mod = np.ones((trajs.shape[0], 1))*label_model
-        labels_alpha = np.ones((trajs.shape[0], 1))*exponent
-        trajs = np.concatenate((labels_mod, labels_alpha, trajs), axis = 1)
-        
-        return trajs
-
-    def create_noisy_localization_dataset(self, 
-                                          dataset = False,
-                                          T = False, N = False, exponents = False, models = False, dimension = 1,
-                                          noise_func = False, sigma = 1, mu = 0,
-                                          save_trajectories = False, load_trajectories = False, 
-                                          path = 'datasets/',
-                                          N_save = 1000, t_save = 1000): 
-        ''' 
-        Create a dataset of noisy trajectories. 
-        This function creates trajectories with _create_trajectories and then adds given noise to them.        
-        All parameters are the same as _create_trajectories but noise_func.
-        
-        Parameters
-        ----------
-        dataset : bool, numpy array
-            If False, creates a dataset with the given parameters.
-            If numpy array, dataset to which the function applies the noise.
-        noise_func : bool, function
-            If False, the noise added to the trajectories will be Gaussian distributed, with 
-            variance sigma and mean value mu.
-            If function, uses the given function to generate noise to be added to the trajectory.
-            The function must have as input two ints, N and M and the output must be a matrix of size NxM.
-        
-        Returns
-        -------
-        numpy.array
-            Dataset of trajectories of lenght Nx(T+2), with the following structure:
-                o First column: model label 
-                o Second column: value of the anomalous exponent
-                o 2:T columns: trajectories'''
-                    
-        if not dataset.any():
-            dataset = self.create_dataset(T, N, exponents, models, dimension,
-                                                     save_trajectories, load_trajectories, 
-                                                     path,
-                                                     N_save, t_save)
-            
-        # Add the noise to the trajectories  
-        trajs = dataset[:, 2:].reshape(dataset.shape[0]*dimension, T)
-        trajs = self._add_noisy_localization(trajs, noise_func, sigma, mu)
-        
-        dataset[:, 2:] = trajs.reshape(dataset.shape[0], T*dimension)
-        
-        return dataset    
-    
-    def create_noisy_diffusion_dataset(self, 
-                                       dataset = False,
-                                       T = False, N = False, exponents = False, models = False, dimension = 1,
-                                       diffusion_coefficients = False, sigma = 1, mu = 0,
-                                       save_trajectories = False, load_trajectories = False, 
-                                       path = 'datasets/',
-                                       N_save = 1000, t_save = 1000): 
-        ''' 
-        Create a dataset of noisy trajectories. 
-        This function creates trajectories with `_create_trajectories` and then adds given noise to them.        
-        All arguments are the same as `_create_trajectories` but dataset and diffusion_coefficients.
-        
-        Parameters
-        ----------       
-        dataset : bool, numpy array
-                - If False, creates a dataset with the given parameters. 
-                - If numpy array, dataset to which the function applies the noise.
-        diffusion_coefficient : bool, function
-                - If False, the diffusion noise added to the trajectories will 
-                  be Gaussian distributed, with variance sigma and mean value mu.
-                - If numpy array, multiply the displacements by them.
-                
-        Returns
-        --------
-        data_models : numpy.array
-                Dataset of trajectories of lenght Nx(T+2), with the following structure:
-                    o First column: model label 
-                    o Second column: value of the anomalous exponent
-                    o 2:T columns: trajectories'''
-                    
-        if not dataset.any():
-            dataset = self.create_dataset(T, N, exponents, models, dimension,
-                                                     save_trajectories, load_trajectories, 
-                                                     path,
-                                                     N_save, t_save)
-        # Add the noise to the trajectories 
-        trajs = dataset[:, 2:].reshape(dataset.shape[0]*dimension, T)
-        trajs = self._add_noisy_diffusion(trajs, diffusion_coefficients, sigma = sigma, mu = mu)
-        
-        dataset[:, 2:] = trajs.reshape(dataset.shape[0], T*dimension)
-        
-        return dataset
-    
-    @staticmethod
-    def _add_noisy_localization(trajs, noise_func = False, sigma = 1, mu = 0):
-        
-        if isinstance(noise_func, np.ndarray):
-            noise_matrix = noise_func 
-        elif not noise_func:
-            noise_matrix = sigma*np.random.randn(trajs.shape)+mu
-        elif hasattr(noise_func, '__call__'):
-            noise_matrix = noise_func(trajs)             
-        else:
-            raise ValueError('noise_func has to be either False for Gaussian noise, a Python function or numpy array.')
-        
-        trajs += noise_matrix 
-        
-        return trajs
-    
-    @staticmethod
-    def _add_noisy_diffusion(trajs, diffusion_coefficients = False):
-        
-        # First normalize the trajectories
-        trajs = normalize(trajs)
-        # Check if diffusion coefficient are an array
-        if isinstance(diffusion_coefficients, np.ndarray):
-            pass
-        # If no new diffusion coefficients given, create new ones randonmly
-        elif not diffusion_coefficients:
-            diffusion_coefficients = np.random.randn(trajs.shape[0])
-        # Apply new diffusion coefficients
-        trajs = (trajs.transpose()*diffusion_coefficients).transpose()
-        
-        return trajs
-
-    @staticmethod
-    def create_segmented_dataset(dataset1, dataset2, dimension = 1, 
-                                 final_length = 200, random_shuffle = False):
-        ''' 
-        Creates a dataset with trajectories which change diffusive feature (either model or anomalous exponent) after a time 't_change'. 
-        
-        Parameters
-        ----------
-        dataset1 : numpy.array
-            Array of size Nx(t+2), where the first columns values correspond
-            to the labels of the model and anomalous exponent. The rest 
-            correspond to the trajectories of length t.
-        dataset2 : numpy.array
-            Same as dataset1
-        dimension : int
-            Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
-        final_length : int
-            Length of the output trajectories.
-        random_shuffle : bool
-            If True, shuffles the first axis of dataset1 and dataset2.
-            
-        Returns
-        -------
-        numpy.array
-                Array of size Nx(t+5) whose columns represent:
-                    o Column 0: changing time
-                    o Column 1,2: labels first part of the trajectory (model, exponent)
-                    o Column 3,4: labels second part of the trajectory (model, exponent)
-                    o Column 5:(t+5): trajectories of lenght t.
-        '''
-                    
-        '''Establish dimensions and corresponding models'''                    
-        
-        if dataset1.shape[0] != dataset2.shape[0]:
-            raise ValueError(f'Input datasets must have the same number of trajectories. Current ones have size {dataset1.shape[0]} and {dataset2.shape[0]}.')
-        if dataset1.shape[1]-2 < final_length or dataset2.shape[1]-2 < final_length:
-            raise ValueError(f'The trajectories in the input datasets are too short. They must be at least {final_length} steps long.')
-        
-        if random_shuffle:
-            np.random.shuffle(dataset1)
-            np.random.shuffle(dataset2)
-        
-        n_trajs = dataset1.shape[0]
-        trajs_1 = np.copy(dataset1[:, 2:].reshape(n_trajs, dimension, int((dataset1.shape[1]-2)/dimension)))
-        trajs_2 = np.copy(dataset2[:, 2:].reshape(n_trajs, dimension, int((dataset2.shape[1]-2)/dimension)))
-
-        trajs_1 = trajs_1[:, :, :final_length]
-        trajs_2 = trajs_2[:, :, :final_length]
-
-        t_change = np.random.randint(1, final_length, n_trajs)
-
-        seg_dataset = np.zeros((n_trajs, dimension*final_length+5))
-        for idx, (tC, traj1, traj2, label1, label2) in enumerate(zip(t_change, 
-                                                                      trajs_1, trajs_2,
-                                                                      dataset1[:, :2], dataset2[:, :2])):
-            seg_dataset[idx, 0] = tC
-            seg_dataset[idx, 1:5] = np.append(label1, label2)
-
-            if dimension == 1:
-                seg_dataset[idx, 5:tC+5] = traj1[:, :tC]
-                seg_dataset[idx, tC+5:] = traj2[:, tC:final_length]-traj2[:, tC]+traj1[:, tC]
-
-            elif dimension == 2 or dimension == 3:
-                traj2 = (traj2.transpose()-traj2[:, tC]+traj1[:, tC]).transpose()
-
-                traj1[:,tC:]  = 0
-                traj2[:, :tC] = 0
-
-                seg_dataset[idx, 5:] = (traj1 + traj2).reshape(dimension*final_length)            
-            
-        return seg_dataset
-    
-    @staticmethod
-    def _save_row(data:np.array, # Row to be appended to the filed
-                  file:str # File where to append data
-                 ):
-        ''' Auxiliary function to save append data in existing files using csv. '''
-        
-        with open(file, 'a') as f:
-            writer = csv.writer(f, delimiter=';', lineterminator='\n',)
-            writer.writerow(data)
-
-    @staticmethod
-    def _cut_trajectory(traj, t_cut, dim=1):
-        ''' Takes a trajectory and cuts it to `t_cut` length. '''
-        cut_traj = traj.reshape(dim, -1)[:, :t_cut]
-        return cut_traj.reshape(-1)    
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/datasets_theory.ipynb.
+
+# %% auto 0
+__all__ = ['datasets_theory']
+
+# %% ../source_nbs/lib_nbs/datasets_theory.ipynb 3
+import numpy as np
+import os
+import inspect
+import h5py
+from tqdm.auto import trange
+import csv
+
+# %% ../source_nbs/lib_nbs/datasets_theory.ipynb 4
+from .utils_trajectories import normalize
+from .models_theory import models_theory as models_theory
+
+# %% ../source_nbs/lib_nbs/datasets_theory.ipynb 6
+class datasets_theory():
+     
+    def __init__(self):        
+        '''
+        This class generates, saves and loads datasets of theoretical trajectories simulated 
+        from various diffusion models (available at andi_datasets.models_theory). 
+        '''
+        self._dimension = 1
+        self._get_models()
+        
+    def _get_models(self):        
+        '''Loading subclass of models'''
+        if self._dimension == 1:
+            self._models = models_theory._oneD()
+        elif self._dimension == 2:
+            self._models = models_theory._twoD()
+        elif self._dimension == 3:
+            self._models = models_theory._threeD()
+        else:
+            raise ValueError('Our current understanding of the physical world is three dimensional and so are the diffusion models available in this class')
+                
+        available_models = inspect.getmembers(self._models, inspect.ismethod)      
+        self.avail_models_name = [x[0] for x in available_models]
+        self.avail_models_func = [x[1] for x in available_models]
+    
+    def create_dataset(self, T, N_models, exponents, models,
+                       dimension = 1,
+                       save_trajectories = False, load_trajectories = False, 
+                       path = 'datasets/',
+                       N_save = 1000, t_save = 1000):        
+        ''' 
+        Creates a dataset of trajectories via the theoretical models defined in `.models_theory`. Check our tutorials for use cases of this function.
+        
+        Parameters
+        ----------
+        T : int
+            Length of the trajectories.   
+        N_models : int, numpy.array
+            - if int, number of trajectories per class (i.e. exponent and model) in the dataset.
+            - if numpy.array, number of trajectories per classes: size (number of models)x(number of classes)    
+        exponents : float, array
+            Anomalous exponents to include in the dataset. Allows for two digit precision.
+        models : bool, int, list
+            Labels of the models to include in the dataset. 
+            Correspodance between models and labels is given by self.label_correspodance, defined at init.
+            If int/list, choose the given models. If False, choose all of them.
+        dimensions : int
+            Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
+        save_trajectories : bool
+            If True, the module saves a .h5 file for each model considered, with N_save trajectories 
+            and T = T_save.
+        load_trajectories : bool
+            If True, the module loads the trajectories of an .h5 file.
+        path : str
+            Path to the folder where to save/load the trajectories dataset.
+        N_save : int
+            Number of trajectories to save for each exponents/model. 
+            Advise: save at the beggining a big dataset (t_save ~ 1e3 and N_save ~ 1e4) 
+            which then allows you to load any other combiantion of T and N_models.
+        t_save : int
+            Length of the trajectories to be saved. See comments on N_save.                
+        
+        Returns
+        -------
+        numpy.array
+                - Dataset of trajectories of lenght Nx(T+2), with the following structure:
+                    o First column: model label 
+                    o Second column: value of the anomalous exponent
+                    o 2:T columns: trajectories
+        '''
+                    
+        '''Managing probable errors in inputs'''
+        if T < 2:
+            raise ValueError('The time of the trajectories has to be bigger than 1.')       
+        if isinstance(exponents, int) or isinstance(exponents, float):
+            exponents = [exponents]
+        
+        '''Managing folders of the datasets'''       
+        if save_trajectories or load_trajectories:                
+            if load_trajectories:
+                save_trajectories = False            
+            if not os.path.exists(path) and load_trajectories:
+                raise FileNotFoundError('The directory from where you want to load the dataset does not exist')                
+            if not os.path.exists(path) and save_trajectories:
+                os.makedirs(path)  
+                
+        '''Establish dimensions and corresponding models'''
+        self._dimension = dimension
+        self._get_models()
+                
+        '''Managing models to load'''       
+        # Load from a list of models
+        if isinstance(models, list): 
+            self._models_name = [self.avail_models_name[idx] for idx in models]     
+            self._models_func = [self.avail_models_func[idx] for idx in models]
+        # Load from a single model
+        elif isinstance(models, int) and not isinstance(models, bool):
+            self._models_name = [self.avail_models_name[models]]
+            self._models_func = [self.avail_models_func[models]]
+        # Load all available models
+        else: 
+            self._models_name =  self.avail_models_name
+            self._models_func =  self.avail_models_func
+            
+        '''Managing number of trajectory per class:
+            - Defines array num_class as a function of N'''                            
+        if isinstance(N_models, int): 
+            n_per_class = N_models*np.ones((len(self._models_name), len(exponents)))
+            
+        elif type(N_models).__module__ == np.__name__: 
+            if len(self._models_name) != N_models.shape[0] or len(exponents) != N_models.shape[1]:
+                raise ValueError('Mismatch between the dimensions of N and the number of different classes.'+
+                                 f'N must be either an int (balanced classes) or an array of length {len(models)}x'
+                                 f'{len(exponents)} (inbalaced classes).') 
+            n_per_class = N_models
+        else:
+            raise TypeError('Type of variable N not recognized.')
+                    
+        '''Defining default values for saved datasets''' 
+        N_save = np.ones_like(n_per_class)*N_save
+        # If the number of class of a given class is bigger than N_save, we
+        # change the value of N_save for that particular class.
+        N_save = np.max([N_save, n_per_class], axis = 0)      
+                
+        ''' Loading/Saving/Creating datasets'''
+        if load_trajectories:
+            data_models = self._load_trajectories(T = T,
+                                                 exponents = exponents,
+                                                 models_name = self._models_name,
+                                                 dimension = self._dimension,
+                                                 n_per_class = n_per_class,
+                                                 path = path,
+                                                 N_save = N_save,
+                                                 t_save = t_save)
+        elif save_trajectories:
+            self._save_trajectories(exponents = exponents,
+                                   dimension = self._dimension,
+                                   models_name = self._models_name,
+                                   models_func = self._models_func,
+                                   path = path, 
+                                   n_per_class = n_per_class,
+                                   N_save = N_save,
+                                   t_save = t_save)
+            
+            data_models = self._load_trajectories(T = T,
+                                                 exponents = exponents,
+                                                 dimension = self._dimension,
+                                                 models_name = self._models_name,                                                 
+                                                 n_per_class = n_per_class,
+                                                 path = path,
+                                                 N_save = N_save,
+                                                 t_save = t_save)
+            
+        else:           
+            data_models = self._create_trajectories(T = T,                                                   
+                                                   exponents = exponents, 
+                                                   dimension = self._dimension,
+                                                   models_name = self._models_name,
+                                                   models_func = self._models_func,
+                                                   n_per_class = n_per_class)       
+            
+        return data_models
+    
+    def _load_trajectories(self, T, exponents, dimension, 
+                                models_name, n_per_class, 
+                                path, N_save = 1000, t_save = 1000):
+        ''' Load trajectories from a h5py file of the given path. The name of the datasets in the
+        file have the following structure: 
+            '(exponent with 2 digit_precision)_T_(lenght of trajectories in the dataset)_N_(number of trajectories in the dataset)'
+            
+        Arguments: 
+            :T (int):
+                - length of the trajectories.   
+            :exponents (array):
+                - anomalous exponents to include in the dataset. Allows for two digit precision.
+            :dimension (int):
+                - Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
+            :models_name (list of str):
+                - names of the models to include in the output dataset. 
+            :n_per_class:
+                - number of trajectories to consider per exponent/model.
+            :path (str):
+                - path to the folder from where to load the trajectories dataset.
+            :t_save (int):
+                - length of the trajectories in the datasets to load.
+            :N_save (array):
+                - number of trajectories contained in the datasets to load.                  
+        Return:
+            :dataset (numpy.array):
+                - Dataset of trajectories of lenght (number of models)x(T+2), with the following structure:
+                    o First column: model label 
+                    o Second column: value of the anomalous exponent
+                    o 2:T columns: trajectories'''
+                    
+        '''Establish dimensions and corresponding models'''
+        self._dimension = dimension
+        self._get_models()
+            
+        
+        if isinstance(models_name, int):
+            models_name = [models_name]
+               
+        for idx_m, name in enumerate(models_name):        
+            hf = h5py.File(path+name+'.h5', 'r+')
+            
+            for idx_e, exp  in enumerate(exponents):
+                
+                name_dataset = f'{exp:.2f}_T_{t_save}_N_'+ \
+                                str(int(N_save[idx_m, idx_e]))+f'_dim_{self._dimension}'  
+                
+                n = int(n_per_class[idx_m, idx_e])
+                if n == 0:
+                    continue
+                
+                try:
+                    data = (hf.get(name_dataset)[()][:n,:self._dimension*T]) 
+                except:
+                    raise TypeError('The dataset you want to load does not exist.')
+                    
+                
+                data = self._label_trajectories(trajs = data, model_name = name, exponent = exp)                
+                            
+                if idx_e + idx_m == 0:
+                    dataset = data
+                else:
+                    dataset = np.concatenate((dataset, data), axis = 0) 
+        return dataset
+     
+    def _save_trajectories(self, exponents, models_name, models_func, path, n_per_class,
+                          N_save = 1000, t_save = 1000, dimension = 1):
+        ''' Saves a dataset for the exponents and models considered. 
+        Arguments:   
+            :exponents (array):
+                - anomalous exponents to include in the dataset. Allows for two digit precision.
+            :models_name (list of str):
+                - names of the models to include in the output dataset. 
+            :models_func (list of funcs):
+                - function generating the models to include in the output dataset. 
+            :path (str):
+                - path to the folder where to save the trajectories dataset.
+            :t_save (int):
+                - length of the trajectories to save in the datasets.
+            :N_save (array):
+                - number of trajectories to include in the datasets saved.
+            :dimension (int):
+                - Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
+        No return           '''     
+    
+        '''Establish dimensions and corresponding models'''
+        self._dimension = dimension
+        self._get_models()        
+        
+        for idx_m, (name, func) in enumerate(zip(models_name, models_func)):
+            
+            if os.path.isfile(path+name+'.h5'):
+                action = 'r+'
+            else:
+                action = 'w'
+            with h5py.File(path+name+'.h5', action) as hf:
+                
+                for idx_e, exp in enumerate(exponents): 
+                    if n_per_class[idx_m, idx_e] == 0:
+                        continue
+                    
+                    n = int(N_save[idx_m, idx_e])                    
+                    name_dataset = f'{exp:.2f}_T_{t_save}_N_{n}_dim_{self._dimension}' 
+                    
+                    if name_dataset not in hf:  
+                        
+                        data = np.zeros((n, self._dimension*t_save))                           
+                        # TQDM variables
+                        tq = trange(n)
+                        tq.set_postfix(saving = True, model = name, exponent = exp)
+                        for i in tq:
+                            data[i, :] = func(t_save, exp)                           
+                            
+                        hf.create_dataset(name_dataset, data=data)
+                        
+                    else:
+                        print(f'The dataset for {name} with exponent {round(exp,3)}'
+                                +' already exists, no need of saving it again.')
+            
+        
+    def _create_trajectories(self, T, exponents, dimension, models_name, models_func, n_per_class):  
+        ''' create a dataset for the exponents and models considered. 
+        Arguments:  
+            :T (int):
+                - length of the trajectories.   
+            :exponents (array):
+                - anomalous exponents to include in the dataset. Allows for two digit precision.
+            :dimension (int):
+                - Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
+            :models_name (list of str):
+                - names of the models to include in the output dataset. 
+            :models_func (list of funcs):
+                - function generating the models to include in the output dataset. 
+            :n_per_class:
+                - number of trajectories to consider per exponent/model. 
+        Return:
+            :dataset (numpy.array):
+                - Dataset of trajectories of lenght (number of models)x(T+2), with the following structure:
+                    o First column: model label.
+                    o Second column: value of the anomalous exponent.
+                    o 2:T columns: trajectories.'''
+            
+        for idx_m, (name, func) in enumerate(zip(models_name, models_func)):
+            for idx_e, exp in enumerate(exponents):
+                
+                
+                n = int(n_per_class[idx_m, idx_e])
+                data = np.zeros((n, self._dimension*T))  
+                for i in range(n):
+                    data[i, :] = func(T, exp)
+                    
+                data = self._label_trajectories(trajs = data, model_name = name, exponent = exp)   
+                
+                if idx_e + idx_m == 0:
+                    dataset = data
+                else:
+                    dataset = np.concatenate((dataset, data), axis = 0)
+                
+        return dataset
+                
+            
+    def _label_trajectories(self, trajs, model_name, exponent):
+        ''' Labels given trajectories given the corresponding label for the model and exponent.
+        For models, the label correspond to the position of the model in self.avail_models_name.
+        For exponents, the label if the value of the exponent.
+        Arguments:
+            :trajs (numpy array):
+                - trajectories to label
+            :model_name (str):
+                - name of the model from which the trajectories are coming from.
+            :exponent (float):
+                - Anomalous exponent of the trajectories. 
+        Return:
+            :trajs (numpy array):
+                - Labelled trajectoreis, with the following structure:
+                    o First column: model label
+                    o Second columnd: exponent label
+                    o Rest of the array: trajectory.   '''
+        
+        label_model = self.avail_models_name.index(model_name)          
+         
+        labels_mod = np.ones((trajs.shape[0], 1))*label_model
+        labels_alpha = np.ones((trajs.shape[0], 1))*exponent
+        trajs = np.concatenate((labels_mod, labels_alpha, trajs), axis = 1)
+        
+        return trajs
+
+    def create_noisy_localization_dataset(self, 
+                                          dataset = False,
+                                          T = False, N = False, exponents = False, models = False, dimension = 1,
+                                          noise_func = False, sigma = 1, mu = 0,
+                                          save_trajectories = False, load_trajectories = False, 
+                                          path = 'datasets/',
+                                          N_save = 1000, t_save = 1000): 
+        ''' 
+        Create a dataset of noisy trajectories. 
+        This function creates trajectories with _create_trajectories and then adds given noise to them.        
+        All parameters are the same as _create_trajectories but noise_func.
+        
+        Parameters
+        ----------
+        dataset : bool, numpy array
+            If False, creates a dataset with the given parameters.
+            If numpy array, dataset to which the function applies the noise.
+        noise_func : bool, function
+            If False, the noise added to the trajectories will be Gaussian distributed, with 
+            variance sigma and mean value mu.
+            If function, uses the given function to generate noise to be added to the trajectory.
+            The function must have as input two ints, N and M and the output must be a matrix of size NxM.
+        
+        Returns
+        -------
+        numpy.array
+            Dataset of trajectories of lenght Nx(T+2), with the following structure:
+                o First column: model label 
+                o Second column: value of the anomalous exponent
+                o 2:T columns: trajectories'''
+                    
+        if not dataset.any():
+            dataset = self.create_dataset(T, N, exponents, models, dimension,
+                                                     save_trajectories, load_trajectories, 
+                                                     path,
+                                                     N_save, t_save)
+            
+        # Add the noise to the trajectories  
+        trajs = dataset[:, 2:].reshape(dataset.shape[0]*dimension, T)
+        trajs = self._add_noisy_localization(trajs, noise_func, sigma, mu)
+        
+        dataset[:, 2:] = trajs.reshape(dataset.shape[0], T*dimension)
+        
+        return dataset    
+    
+    def create_noisy_diffusion_dataset(self, 
+                                       dataset = False,
+                                       T = False, N = False, exponents = False, models = False, dimension = 1,
+                                       diffusion_coefficients = False,
+                                       save_trajectories = False, load_trajectories = False, 
+                                       path = 'datasets/',
+                                       N_save = 1000, t_save = 1000): 
+        ''' 
+        Create a dataset of noisy trajectories. 
+        This function creates trajectories with `_create_trajectories` and then adds given noise to them.        
+        All arguments are the same as `_create_trajectories` but dataset and diffusion_coefficients.
+        
+        Parameters
+        ----------       
+        dataset : bool, numpy array
+                - If False, creates a dataset with the given parameters. 
+                - If numpy array, dataset to which the function applies the noise.
+        diffusion_coefficient : bool, function
+                - If False, the diffusion noise added to the trajectories will 
+                  be Gaussian distributed, with variance sigma and mean value mu.
+                - If numpy array, multiply the displacements by them.
+                
+        Returns
+        --------
+        data_models : numpy.array
+                Dataset of trajectories of lenght Nx(T+2), with the following structure:
+                    o First column: model label 
+                    o Second column: value of the anomalous exponent
+                    o 2:T columns: trajectories'''
+                    
+        if not dataset.any():
+            dataset = self.create_dataset(T, N, exponents, models, dimension,
+                                                     save_trajectories, load_trajectories, 
+                                                     path,
+                                                     N_save, t_save)
+        # Add the noise to the trajectories 
+        trajs = dataset[:, 2:].reshape(dataset.shape[0]*dimension, T)
+        trajs = self._add_noisy_diffusion(trajs, diffusion_coefficients)
+        
+        dataset[:, 2:] = trajs.reshape(dataset.shape[0], T*dimension)
+        
+        return dataset
+    
+    @staticmethod
+    def _add_noisy_localization(trajs, noise_func = False, sigma = 1, mu = 0):
+        
+        if isinstance(noise_func, np.ndarray):
+            noise_matrix = noise_func 
+        elif not noise_func:
+            noise_matrix = sigma*np.random.randn(*trajs.shape)+mu
+        elif hasattr(noise_func, '__call__'):
+            noise_matrix = noise_func(trajs)             
+        else:
+            raise ValueError('noise_func has to be either False for Gaussian noise, a Python function or numpy array.')
+        
+        trajs += noise_matrix 
+        
+        return trajs
+    
+    @staticmethod
+    def _add_noisy_diffusion(trajs, diffusion_coefficients = False):
+        
+        # First normalize the trajectories
+        trajs = normalize(trajs)
+        # Check if diffusion coefficient are an array
+        if isinstance(diffusion_coefficients, np.ndarray):
+            pass
+        # If no new diffusion coefficients given, create new ones randonmly
+        elif not diffusion_coefficients:
+            diffusion_coefficients = np.random.randn(trajs.shape[0])
+        # Apply new diffusion coefficients
+        trajs = (trajs.transpose()*diffusion_coefficients).transpose()
+        
+        return trajs
+
+    @staticmethod
+    def create_segmented_dataset(dataset1, dataset2, dimension = 1, 
+                                 final_length = 200, random_shuffle = False):
+        ''' 
+        Creates a dataset with trajectories which change diffusive feature (either model or anomalous exponent) after a time 't_change'. 
+        
+        Parameters
+        ----------
+        dataset1 : numpy.array
+            Array of size Nx(t+2), where the first columns values correspond
+            to the labels of the model and anomalous exponent. The rest 
+            correspond to the trajectories of length t.
+        dataset2 : numpy.array
+            Same as dataset1
+        dimension : int
+            Dimensions of the generated trajectories. Three possible values: 1, 2 and 3.
+        final_length : int
+            Length of the output trajectories.
+        random_shuffle : bool
+            If True, shuffles the first axis of dataset1 and dataset2.
+            
+        Returns
+        -------
+        numpy.array
+                Array of size Nx(t+5) whose columns represent:
+                    o Column 0: changing time
+                    o Column 1,2: labels first part of the trajectory (model, exponent)
+                    o Column 3,4: labels second part of the trajectory (model, exponent)
+                    o Column 5:(t+5): trajectories of lenght t.
+        '''
+                    
+        '''Establish dimensions and corresponding models'''                    
+        
+        if dataset1.shape[0] != dataset2.shape[0]:
+            raise ValueError(f'Input datasets must have the same number of trajectories. Current ones have size {dataset1.shape[0]} and {dataset2.shape[0]}.')
+        if dataset1.shape[1]-2 < final_length or dataset2.shape[1]-2 < final_length:
+            raise ValueError(f'The trajectories in the input datasets are too short. They must be at least {final_length} steps long.')
+        
+        if random_shuffle:
+            np.random.shuffle(dataset1)
+            np.random.shuffle(dataset2)
+        
+        n_trajs = dataset1.shape[0]
+        trajs_1 = np.copy(dataset1[:, 2:].reshape(n_trajs, dimension, int((dataset1.shape[1]-2)/dimension)))
+        trajs_2 = np.copy(dataset2[:, 2:].reshape(n_trajs, dimension, int((dataset2.shape[1]-2)/dimension)))
+
+        trajs_1 = trajs_1[:, :, :final_length]
+        trajs_2 = trajs_2[:, :, :final_length]
+
+        t_change = np.random.randint(1, final_length, n_trajs)
+
+        seg_dataset = np.zeros((n_trajs, dimension*final_length+5))
+        for idx, (tC, traj1, traj2, label1, label2) in enumerate(zip(t_change, 
+                                                                      trajs_1, trajs_2,
+                                                                      dataset1[:, :2], dataset2[:, :2])):
+            seg_dataset[idx, 0] = tC
+            seg_dataset[idx, 1:5] = np.append(label1, label2)
+
+            if dimension == 1:
+                seg_dataset[idx, 5:tC+5] = traj1[:, :tC]
+                seg_dataset[idx, tC+5:] = traj2[:, tC:final_length]-traj2[:, tC]+traj1[:, tC]
+
+            elif dimension == 2 or dimension == 3:
+                traj2 = (traj2.transpose()-traj2[:, tC]+traj1[:, tC]).transpose()
+
+                traj1[:,tC:]  = 0
+                traj2[:, :tC] = 0
+
+                seg_dataset[idx, 5:] = (traj1 + traj2).reshape(dimension*final_length)            
+            
+        return seg_dataset
+    
+    @staticmethod
+    def _save_row(data:np.array, # Row to be appended to the filed
+                  file:str # File where to append data
+                 ):
+        ''' Auxiliary function to save append data in existing files using csv. '''
+        
+        with open(file, 'a') as f:
+            writer = csv.writer(f, delimiter=';', lineterminator='\n',)
+            writer.writerow(data)
+
+    @staticmethod
+    def _cut_trajectory(traj, t_cut, dim=1):
+        ''' Takes a trajectory and cuts it to `t_cut` length. '''
+        cut_traj = traj.reshape(dim, -1)[:, :t_cut]
+        return cut_traj.reshape(-1)
```

### Comparing `andi_datasets-2.0.3/andi_datasets/models_phenom.py` & `andi_datasets-2.0.4/andi_datasets/models_phenom.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,1401 +1,1401 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/models_phenom.ipynb.
-
-# %% auto 0
-__all__ = ['models_phenom']
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 2
-import numpy as np
-from stochastic.processes.noise import FractionalGaussianNoise as FGN
-from .utils_trajectories import gaussian
-import warnings
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 5
-class models_phenom():
-    def __init__(self):
-        '''
-        This class handles the generation of trajectories from different theoretical models. 
-        ''' 
-        # We define here the bounds of the anomalous exponent and diffusion coefficient
-        self.bound_D = [1e-12, 1e6]
-        self.bound_alpha = [0, 1.999]
-        
-        # We also define the value in which we consider directed motion
-        self.alpha_directed = 1.9
-        
-        # Diffusion state labels: the position of each type defines its numerical label
-        # i: immobile/trapped; c: confined; f: free-diffusive (normal and anomalous); d: directed
-        self.lab_state = ['i', 'c', 'f', 'd']
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 7
-class models_phenom(models_phenom):
-    
-    @staticmethod
-    def disp_fbm(alpha : float,
-                 D : float,
-                 T: int, 
-                 deltaT : int = 1):
-        ''' Generates normalized Fractional Gaussian noise. This means that, in 
-        general:
-        
-                            <x^2(t)> = 2Dt^alpha
-                            
-        and in particular:
-        
-                            <x^2(t = 1)> = 2D 
-        
-        Parameters
-        ----------
-        alpha : float in [0,2]
-            Anomalous exponent
-        D : float
-            Diffusion coefficient
-        T : int
-            Number of displacements to generate
-        deltaT : int, optional
-            Sampling time
-            
-        Returns
-        -------
-        numpy.array
-            Array containing T displacements of given parameters
-        
-        '''
-        
-        # Generate displacements
-        disp = FGN(hurst = alpha/2).sample(n = T)
-        # Normalization factor
-        disp *= np.sqrt(T)**(alpha)
-        # Add D
-        disp *= np.sqrt(2*D*deltaT)        
-        
-        return disp
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 15
-class models_phenom(models_phenom):
-    
-    @staticmethod
-    def _constraint_alpha(alpha_1, alpha_2, epsilon_a):
-        ''' Defines the metric for constraining the changes in anomalous
-        exponent'''
-        return alpha_1 - alpha_2 < epsilon_a
-    
-    @staticmethod
-    def _constraint_d(d1, d2, gamma_d):
-        ''' Defines the metric for constraining the changes in anomalous
-        exponent'''
-        if gamma_d < 1:
-            return d2 > d1*gamma_d
-        if gamma_d > 1:
-            return d2 < d1*gamma_d
-    
-    @staticmethod
-    def _sample_diff_parameters(alphas : list, # List containing the parameters to sample anomalous exponent in state (adapt to sampling function)
-                                Ds : list, # List containing the parameters to sample the diffusion coefficient in state (adapt to sampling function).
-                                num_states : int, # Number of diffusive states.
-                                epsilon_a : float, #  Minimum distance between anomalous exponents of various states.
-                                gamma_d : float, # Factor between diffusion coefficient of various states.
-                               ) : 
-        '''    
-        Given information of the anomalous exponents (alphas), diffusion coefficients (Ds), the function
-        samples these from a bounded Gaussian distribution with the indicated constraints (epsilon_a,
-        gamma_d). Outputs the list of demanded alphas and Ds.
-        
-        
-        Parameters
-        ----------
-        alphas : list
-        List containing the parameters to sample anomalous exponent in state (adapt to sampling function).
-        Ds : list
-        List containing the parameters to sample the diffusion coefficient in state (adapt to sampling function).
-        num_states : int
-        Number of diffusive states.
-        epsilon_a : float
-        Minimum distance between anomalous exponents of various states.            
-                epsilon workflow: we check val[i] - val[i-1] < epsilon
-                    if you want that val[i] > val[i-1]: epsilon has to be positive
-                    if you want that val[i] < val[i-1]: epsilon has to be negative
-                    if you don't care: epsilon = 0
-                
-        gamma_d : float
-        Factor between diffusion coefficient of various states.            
-                gamma workflow: 
-                    for gamma < 1: val[i] < val[i-1]*gamma
-                    for gamma > 1: val[i] > val[i-1]*gamma
-                    for gamma = 1: no check
-        Returns
-        -------
-            :alphas_traj (list): list of anomalous exponents
-            :Ds_traj (list): list of diffusion coefficients
-                      
-        '''
-
-        
-        alphas_traj = []
-        Ds_traj = []
-        for i in range(num_states): 
-
-            # for the first state we just sample normally
-            if i == 0:
-                alphas_traj.append(float(gaussian(alphas[i], bound = models_phenom().bound_alpha)))
-                Ds_traj.append(float(gaussian(Ds[i], bound = models_phenom().bound_D)))
-           
-            # For next states we take into account epsilon distance between diffusion
-            # parameter
-            else:
-                ## Checking alpha
-                alpha_state = float(gaussian(alphas[i], bound = models_phenom().bound_alpha))
-                D_state = float(gaussian(Ds[i], bound = models_phenom().bound_D))
-
-                if epsilon_a[i-1] != 0:
-                    idx_while = 0
-                    while models_phenom()._constraint_alpha(alphas_traj[-1], alpha_state, epsilon_a[i-1]):
-                    #alphas_traj[-1] - alpha_state < epsilon_a[i-1]:
-                        alpha_state = float(gaussian(alphas[i], bound = models_phenom().bound_alpha))                        
-                        idx_while += 1
-                        if idx_while > 100: # check that we are not stuck forever in the while loop
-                            raise FileNotFoundError(f'Could not find correct alpha for state {i} in 100 steps. State distributions probably too close.')
-
-                alphas_traj.append(alpha_state)
-                
-                ## Checking D
-                if gamma_d[i-1] != 1:    
-                    
-                    idx_while = 0
-                    while models_phenom()._constraint_d(Ds_traj[-1], D_state, gamma_d[i-1]):
-                        D_state = float(gaussian(Ds[i], bound = models_phenom().bound_D))
-                        idx_while += 1
-                        if idx_while > 100: # check that we are not stuck forever in the while loop
-                            raise FileNotFoundError(f'Could not find correct D for state {i} in 100 steps. State distributions probably too close.')
-               
-    
-                Ds_traj.append(D_state)
-                
-        return alphas_traj, Ds_traj
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 23
-class models_phenom(models_phenom):
-    
-    @staticmethod
-    def _single_state_traj(T :int = 200, 
-                          D : float = 1, 
-                          alpha : float = 1, 
-                          L : float = None,
-                          deltaT : int = 1):
-        '''
-        Generates a single state trajectory with given parameters. 
-        
-        Parameters
-        ----------
-        T : int
-            Length of the trajectory
-        D : float
-            Diffusion coefficient       
-        alpha : float
-            Anomalous exponent
-        L : float
-            Length of the box acting as the environment
-        deltaT : int, optional
-            Sampling time
-            
-        Returns
-        -------
-        tuple
-            - pos: position of the particle
-            - labels:  anomalous exponent, D and state at each timestep. State is always free here.
-            
-        '''
-        
-        
-        # Trajectory displacements
-        dispx, dispy = models_phenom().disp_fbm(alpha, D, T), models_phenom().disp_fbm(alpha, D, T)
-        # Labels
-        lab_diff_state = np.ones(T)*models_phenom().lab_state.index('f') if alpha < models_phenom().alpha_directed else np.ones(T)*models_phenom().lab_state.index('d')
-        labels = np.vstack((np.ones(T)*alpha, 
-                            np.ones(T)*D,
-                            lab_diff_state
-                           )).transpose()
-
-        # If there are no boundaries
-        if not L:
-            posx, posy = np.cumsum(dispx) - dispx[0], np.cumsum(dispy) - dispy[0]
-
-            return np.vstack((posx, posy)).transpose(), labels
-
-        # If there are, apply reflecting boundary conditions
-        else:
-            pos = np.zeros((T, 2))
-
-            # Initialize the particle in a random position of the box
-            pos[0, :] = np.random.rand(2)*L
-            for t in range(1, T):
-                pos[t, :] = [pos[t-1, 0]+dispx[t], pos[t-1, 1]+dispy[t]]            
-
-
-                # Reflecting boundary conditions
-                while np.max(pos[t, :])>L or np.min(pos[t, :])< 0: 
-                    pos[t, pos[t, :] > L] = pos[t, pos[t, :] > L] - 2*(pos[t, pos[t, :] > L] - L)
-                    pos[t, pos[t, :] < 0] = - pos[t, pos[t, :] < 0]
-
-            return pos, labels
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 27
-class models_phenom(models_phenom):
-    
-    
-    def single_state(self,
-                     N:int = 10,
-                     T:int = 200, 
-                     Ds:list = [1, 0], 
-                     alphas:list = [1, 0], 
-                     L:float = None):
-        '''
-        Generates a dataset made of single state trajectories with given parameters.
-        
-        Parameters
-        ----------
-        N : int, list
-            Number of trajectories in the dataset
-        T : int
-            Length of the trajectory
-        Ds : float
-            If list, mean and variance from which to sample the diffusion coefficient. If float, we consider variance = 0.
-        alphas : float
-            If list, mean and variance from which to sample the anomalous exponent. If float, we consider variance = 0.
-        L : float
-            Length of the box acting as the environment
-        deltaT : int, optional
-            Sampling time
-            
-        Returns
-        -------
-        tuple
-            - positions: position of the N trajectories.
-            - labels:  anomalous exponent, D and state at each timestep. State is always free here.         
-        '''
-
-        positions = np.zeros((T, N, 2))
-        labels = np.zeros((T, N, 3))
-
-        for n in range(N):
-            alpha_traj = gaussian(alphas, bound = self.bound_alpha)
-            D_traj = gaussian(Ds, bound = self.bound_D)
-            # Get trajectory from single traj function
-            pos, lab = self._single_state_traj(T = T, 
-                                   D = D_traj, 
-                                   alpha = alpha_traj, 
-                                   L = L)        
-            positions[:, n, :] = pos
-            labels[:, n, :] = lab
-
-        return positions, labels
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 33
-class models_phenom(models_phenom):
-    
-    @staticmethod
-    def _multiple_state_traj(T = 200, 
-                             M = [[0.95 , 0.05],[0.05 ,0.95]], 
-                             Ds = [1, 0.1], 
-                             alphas = [1, 1], 
-                             L = None,
-                             deltaT = 1,
-                             return_state_num = False, 
-                             init_state = None
-                            ):
-        
-        '''
-        Generates a 2D multi state trajectory with given parameters.        
-        
-        Parameters
-        ----------
-        T : int
-            Length of the trajectory
-        M : list, array
-            Transition matrix between diffusive states.        
-        Ds : list
-            Diffusion coefficients of the diffusive states. Must have as many Ds as states defined by M.
-        alphas : list
-            Anomalous exponents of the diffusive states. Must have as many alphas as states defined by M.
-        L : float
-            Length of the box acting as the environment
-        deltaT : int, optional
-            Sampling time
-        return_state_num : bool
-            If True, returns as label the number assigned to the state at each time step.
-        init_state : bool
-            If True, the particle starts in state 0. If not, sample initial state.
-            
-            
-        Returns
-        -------
-        tuple
-            - pos: position of the particle
-            - alphas_t: anomalous exponent at each  step
-            - Ds_t: diffusion coefficient at each step. 
-            - label_diff_state: particle's state (can be either free or directed for alpha ~ 2) at each step.
-            - state (optional): state label at each step.            
-        
-        '''
-        
-        # transform lists to numpy if needed
-        if isinstance(M, list):
-            M = np.array(M)
-        if isinstance(Ds, list):
-            Ds = np.array(Ds)
-        if isinstance(alphas, list):
-            alphas = np.array(alphas)
-
-
-        pos = np.zeros((T, 2))
-        if L: pos[0,:] = np.random.rand(2)*L
-
-        # Diffusing state of the particle
-        state = np.zeros(T).astype(int)
-        if init_state is None:
-            state[0] = np.random.randint(M.shape[0])
-        else: state[0] = init_state
-        
-        # Init alphas, Ds
-        alphas_t = np.array(alphas[state[0]]).repeat(T)
-        Ds_t = np.array(Ds[state[0]]).repeat(T)
-        
-        
-        # Trajectory displacements    
-        dispx, dispy = [models_phenom().disp_fbm(alphas_t[0], Ds_t[0], T),
-                        models_phenom().disp_fbm(alphas_t[0], Ds_t[0], T)]
-
-
-        for t in range(1, T):
-
-            pos[t, :] = [pos[t-1, 0]+dispx[t], pos[t-1, 1]+dispy[t]]  
-
-            # at each time, check new state
-            state[t] = np.random.choice(np.arange(M.shape[0]), p = M[state[t-1], :])
-
-
-            if state[t] != state[t-1]:
-                
-                alphas_t[t:] =  np.array(alphas[state[t]]).repeat(T-t)  
-                Ds_t[t:] = np.array(Ds[state[t]]).repeat(T-t)
-                
-                
-                # Recalculate new displacements for next steps
-                if len(dispx[t:]) > 1:                    
-                    dispx[t:], dispy[t:] = [models_phenom().disp_fbm(alphas_t[t], Ds_t[t], T-t),
-                                            models_phenom().disp_fbm(alphas_t[t], Ds_t[t], T-t)]
-                        
-                        
-                else: 
-                    dispx[t:], dispy[t:] = [np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn(), 
-                                            np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn()]
-                    
-
-            if L is not None:
-                # Reflecting boundary conditions
-                while np.max(pos[t, :])>L or np.min(pos[t, :])< 0: 
-                    pos[t, pos[t, :] > L] = pos[t, pos[t, :] > L] - 2*(pos[t, pos[t, :] > L] - L)
-                    pos[t, pos[t, :] < 0] = - pos[t, pos[t, :] < 0]
-                    
-        # Define state of particles based on values of alphas: either free or directed
-        label_diff_state = np.zeros_like(alphas_t)
-        label_diff_state[alphas_t  < models_phenom().alpha_directed] = models_phenom().lab_state.index('f')
-        label_diff_state[alphas_t >= models_phenom().alpha_directed] = models_phenom().lab_state.index('d')
-                    
-        if return_state_num:            
-            return pos, np.array((alphas_t,
-                                  Ds_t,
-                                  label_diff_state,
-                                  state)).transpose()
-        else: 
-            return pos, np.array((alphas_t,
-                                  Ds_t,
-                                  label_diff_state)).transpose()
-        
-
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 37
-class models_phenom(models_phenom):
-    def multi_state(self,
-                    N = 10,
-                    T = 200,
-                    M: np.array = [[0.9 , 0.1],[0.1 ,0.9]],
-                    Ds: np.array = [[1, 0], [0.1, 0]], 
-                    alphas: np.array = [[1, 0], [1, 0]], 
-                    gamma_d = [1], 
-                    epsilon_a = [0], 
-                    L = None,
-                    return_state_num = False,
-                    init_state = None): 
-        '''
-        Generates a dataset of 2D multi state trajectory with given parameters.
-        
-        Parameters
-        ----------
-        N : int
-            Number of trajectories
-        T : int
-            Length of the trajectory
-        M : list, array
-            Transition matrix between diffusive states
-        Ds : list
-            List of means and variances from which to sample the diffusion coefficient of each state. If element size is one, we consider variance = 0.
-        alphas : float
-            List of means and variances from which to sample the anomalous exponent of each state. If element size is one, we consider variance = 0.   
-        gamma_d : list
-            Minimum factor between D of diffusive states (see ._sampling_diff_parameters)
-        epsilon_a : list
-            Distance between alpha of diffusive states (see ._sampling_diff_parameters)
-        L : float
-            Length of the box acting as the environment
-        deltaT : int, optional
-            Sampling time
-        return_state_num : bool
-            If True, returns as label the number assigned to the state at each time step.
-        init_state : bool
-            If True, the particle starts in state 0. If not, sample initial state.
-            
-            
-        Returns
-        -------
-        tuple
-            - trajs (array TxNx2): particles' position
-            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels)           
-        
-        '''
-        
-        # transform lists to numpy if needed
-        if isinstance(M, list):
-            M = np.array(M)
-        if isinstance(Ds, list):
-            Ds = np.array(Ds)
-        if isinstance(alphas, list):
-            alphas = np.array(alphas)
-        
-        
-
-        trajs = np.zeros((T, N, 2))
-        if return_state_num:
-            labels = np.zeros((T, N, 4))
-        else:
-            labels = np.zeros((T, N, 3))
-
-        for n in range(N):
-            
-            ### Sampling diffusion parameters for each state
-            alphas_traj = []
-            Ds_traj = []
-            
-            alphas_traj, Ds_traj = self._sample_diff_parameters(alphas = alphas,
-                                                                Ds = Ds,
-                                                                num_states = M.shape[0],
-                                                                epsilon_a = epsilon_a,
-                                                                gamma_d = gamma_d)
-                    
-            #### Get trajectory from single traj function
-            traj, lab = self._multiple_state_traj(T = T,
-                                                  L = L,
-                                                  M = M,
-                                                  alphas = alphas_traj,
-                                                  Ds = Ds_traj,
-                                                  return_state_num = return_state_num,
-                                                  init_state = init_state
-                                                 )  
-                
-            trajs[:, n, :] = traj
-            labels[:, n, :] = lab 
-            
-        return trajs, labels
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 46
-class models_phenom(models_phenom):
-    @staticmethod
-    def _get_distance(x):
-        '''
-        Given a matrix of size Nx2, calculates the distance between the N particles.
-        
-        Parameters
-        ----------
-        x : array
-            Particles' positions
-            
-        Returns
-        -------
-        array
-            Distance between particles         
-        
-        '''
-        
-        M = np.reshape(np.repeat(x[ :, :], x.shape[0], axis = 0), (x.shape[0], x.shape[0], 2))
-        Mtrans = M.transpose(1,0,2)
-        distance = np.sqrt(np.square(M[:,:, 0]-Mtrans[:,:, 0])
-                         + np.square(M[:,:, 1]-Mtrans[:,:, 1]))  
-        return distance
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 49
-class models_phenom(models_phenom):
-    @staticmethod
-    def _make_escape(Pu, label, diff_state):
-        ''' 
-        Given an unbinding probablity (Pu), the current labeling of particles (label)
-        and the current state of particle (diff_state, either bound, 1, or unbound, 0), simulate an
-        stochastic binding mechanism. 
-        
-        Parameters
-        ----------
-        Pu : float
-            Unbinding probablity
-        label : array
-            Current labeling of the particles (i.e. to which condensate they belong)
-        diff_state : array
-            Current state of the particles
-            
-        Returns
-        -------
-        tuple
-            New labeling and diffusive state of the particles        
-        
-        '''
-
-        # if unbinding probability is zero
-        if Pu == 0:
-            return label, diff_state
-
-        label = label.copy()
-        diff_state = diff_state.copy()
-
-        label_dimers = np.unique(label[np.argwhere(diff_state == 1)])
-
-        for l in label_dimers:         
-
-            if np.random.rand() < Pu:
-                # give new label to escaping particles
-                diff_state[label == l] = 0
-                label[label == l] = np.max(label)+np.arange(2)+1
-
-        return label, diff_state
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 52
-class models_phenom(models_phenom):
-    @staticmethod
-    def _make_condensates(Pb, label, diff_state, r, distance, max_label):
-        '''
-        Given a binding probability Pb, the current label of particles (label),
-        their current diffusive state (diff_state), the particle size (r), their 
-        distances (distance) and the label from which binding is not possible 
-        (max_label), simulates a binding mechanism.
-                
-        Parameters
-        ----------
-        Pb : float
-            Binding probablity.
-        label : array
-            Current labeling of the particles (i.e. to which condensate they belong)
-        diff_state : array
-            Current state of the particles
-        r : float
-            Particle size.
-        distance : array
-            Distance between particles
-        max_label : int
-            Maximum label from which particles will not be considered for binding
-            
-        Returns
-        -------
-        tuple
-            New labeling and diffusive state of the particles
-        '''
-
-        label = label.copy()
-        diff_state = diff_state.copy()
-
-        # Keeping track of the ones that will dimerize
-        already_dimer = []
-
-        for n, l in enumerate(label):
-
-            # Consider conditions in which particles do not dimerize
-            if n in already_dimer or diff_state[n] == 1 or l > max_label:
-                continue
-
-            # Extract distances to current particle
-            distance_to_current = distance[n,:]
-            distance_to_current[n] == 0
-            close_particles = np.argwhere((distance_to_current < 2*r) & (distance_to_current > 0)).flatten()
-
-            # Loop over all posible dimerizing candidates
-            for chosen in close_particles:
-
-                # Consider conditions in which particles do not dimerize
-                if chosen in already_dimer or diff_state[chosen] == 1 or label[chosen] > max_label: 
-                    continue
-
-                # Draw coin to see if particle dimerizes
-                if np.random.rand() < Pb:                                 
-                    # Add dimerized particles to the new dimer counter
-                    already_dimer.append(chosen)
-                    already_dimer.append(n)
-                    # Update their diffusive state
-                    diff_state[n] = 1
-                    diff_state[chosen] = 1 
-
-                    # dimerize particles
-                    label[chosen] = l
-
-                    # if one particles dimers, not more clustering!
-                    break
-
-        return label, diff_state
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 57
-class models_phenom(models_phenom):
-    @staticmethod
-    def _stokes(D):
-        '''
-        Applies a Stokes-Einstein-like transformation to two diffusion coefficients.        
-                
-        Parameters
-        ----------
-        D : tuple
-            Diffusion coefficients of the two binding particles.
-            
-        Returns
-        -------
-        float
-            Resulting diffusion coefficient.
-        '''
-        
-        D1 = D[0]; D2 = D[1]
-        return 1/((1/D1)+(1/D2))
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 60
-class models_phenom(models_phenom):
-    def dimerization(self,
-                     N = 10,
-                     T = 200,                
-                     L = 100,
-                     r = 1,
-                     Pu = 0.1, 
-                     Pb = 0.01,
-                     Ds: np.array = [[1, 0], [0.1, 0]],
-                     alphas: np.array = [[1, 0], [1, 0]],
-                     epsilon_a = 0, stokes = False,
-                     return_state_num = False,
-                     deltaT = 1
-                     ):
-        '''
-        Generates a dataset of 2D trajectories of particles perfoming stochastic dimerization.
-        
-        Parameters
-        ----------
-        N : int
-            Number of trajectories
-        T : int
-            Length of the trajectory
-        L : float
-            Length of the box acting as the environment
-        r : float
-            Radius of particles.
-        Pu : float in [0,1]
-            Unbinding probability.
-        Pb : float in [0,1])
-            Binding probability.    
-        Ds : array
-            List of means and variances from which to sample the diffusion coefficient of each state. If element size is one, we consider variance = 0.
-        alphas : array
-            List of means and variances from which to sample the anomalous exponent of each state. If element size is one, we consider variance = 0.   
-        epsilon_a : float
-            Distance between alpha of diffusive states (see ._sampling_diff_parameters)           
-        stokes : bool
-            If True, applies a Stokes-Einstein like coefficient to calculate the diffusion coefficient of dimerized particles.  
-            If False, we use as D resulting from the dimerization the D assigned to the dimerized state of one of the two particles.
-        deltaT : int
-            Sampling time
-        return_state_num : bool
-            If True, returns as label the number assigned to the state at each time step.            
-            
-        Returns
-        -------
-        tuple
-            - trajs (array TxNx2): particles' position
-            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels)
-            
-        '''
-        
-        # transform lists to numpy if needed
-        if isinstance(Ds, list):
-            Ds = np.array(Ds)
-        if isinstance(alphas, list):
-            alphas = np.array(alphas)
-
-        # Info to save
-        pos = np.zeros((T, N, 2)) # position over time
-        label = np.zeros((T, N)).astype(int)
-        diff_state = np.zeros((T, N)).astype(int)
-
-        # Init position, labels     
-        pos[0, :, :] = np.random.rand(N, 2)*L    
-        label[0, :] = np.arange(pos.shape[1])
-        
-        # Init alphas, Ds
-        # Calculate alpha/D for each particle in each state
-        alphas_N = np.array([gaussian(alphas[0], size = N, bound = self.bound_alpha),
-                             gaussian(alphas[1], size = N, bound = self.bound_alpha)])
-        Ds_N = np.array([gaussian(Ds[0], size = N, bound = self.bound_D),
-                         gaussian(Ds[1], size = N, bound = self.bound_D)])
-        # define labels over time by means of state 0
-        alphas_t = alphas_N[0,:].repeat(T).reshape(N,T).transpose()
-        Ds_t = Ds_N[0,:].repeat(T).reshape(N,T).transpose()
-        
-                
-        # initial displacements (all free particles)
-        disps = np.zeros((T, N, 2))
-        for n in range(N):            
-            disps[:, n, 0] = models_phenom().disp_fbm(alphas_t[0, n], Ds_t[0, n], T, deltaT = deltaT)
-            disps[:, n, 1] = models_phenom().disp_fbm(alphas_t[0, n], Ds_t[0, n], T, deltaT = deltaT)
-   
-        for t in (range(1, T)):
-
-            # Find max label to account later for escaped
-            max_label = np.max(label[t-1, :])
-
-            # Make particles escape
-            label[t, :], diff_state[t, :] = self._make_escape(Pu,
-                                                              label[t-1, :], 
-                                                              diff_state[t-1, :])
-
-            lab, diff = label[t, :].copy(), diff_state[t, :].copy()
-
-            # get distance + increasing it for escaped to avoid reclustering
-            distance = self._get_distance(pos[t-1, :, :])
-
-            # Merge particles in condensates
-            label[t, :], diff_state[t, :] = self._make_condensates(Pb,
-                                                                 label[t, :],
-                                                                 diff_state[t, :],
-                                                                 r, distance, max_label)
-
-            # Find particles which changed state
-            label_changed, counts = np.unique(label[t, np.not_equal(diff_state[t-1,:], diff_state[t,:])], 
-                                              return_counts = True)
-
-            # Calculate new displacements for particles which changed state
-            for l, count in zip(label_changed, counts):
-
-                index = int(np.argwhere(label[t,:] == l)[0])
-                state = diff_state[t, index]
-                
-                
-                ### Calculating new diffusion parameters
-                # anomalous exponent
-                if epsilon_a != 0 and state == 1:                    
-                    new_alpha = gaussian(alphas[1], size = 1, bound = self.bound_alpha)
-                    idx_while = 0
-                    while models_phenom()._constraint_alpha(alphas_N[0, label[t, :] == l].min(), new_alpha, epsilon_a):
-                        new_alpha = gaussian(alphas[1], size = 1, bound = self.bound_alpha)
-                        idx_while += 1
-                        if idx_while > 100: # check that we are not stuck forever in the while loop
-                            raise FileNotFoundError(f'Could not find correct alpha in 100 steps. State distributions probably too close.')
-                    alphas_t[t:, label[t, :] == l] = new_alpha
-                else: 
-                    # if no epsilon is given, use the alpha of the first particle
-                    # While here it seems we take both, in the for loop where we assign the displacements below we only
-                    # sample with the first value.
-                    alphas_t[t:, label[t, :] == l] = alphas_N[state, label[t, :] == l].repeat(T-t).reshape(count, T-t).transpose()
-                    
-                # diffusion coefficient
-                if stokes and state == 1:
-                    Ds_t[t:, label[t, :] == l] = models_phenom()._stokes(Ds_t[t-1, label[t, :] == l])
-                else: # if no stokes is given, use the D assgined to the dimerized state of the first particle 
-                    Ds_t[t:, label[t, :] == l] = Ds_N[state, label[t, :] == l].repeat(T-t).reshape(count, T-t).transpose()
-                    
-                for idx, i in enumerate(np.argwhere(label[t,:] == l)):
-                    # We first calculate the displacements so dimers have same motion
-                    if idx == 0:                        
-                        if T-t > 1:                       
-                            disp_current_x = models_phenom().disp_fbm(float(alphas_t[t, i]), float(Ds_t[t, i]), T-t, deltaT = deltaT).reshape(T-t, 1)
-                            disp_current_y = models_phenom().disp_fbm(float(alphas_t[t, i]), float(Ds_t[t, i]), T-t, deltaT = deltaT).reshape(T-t, 1)
-                        else: 
-                            disp_current_x = np.sqrt(2*float(Ds_t[t, i])*deltaT)*np.random.randn(1)
-                            disp_current_y = np.sqrt(2*float(Ds_t[t, i])*deltaT)*np.random.randn(1)
-                            
-                    disps[t:, i, 0] = disp_current_x
-                    disps[t:, i, 1] = disp_current_y
-
-            # Update position
-            pos[t, :, :] = pos[t-1,:,:]+disps[t, :, :]
-            # Consider boundary conditions
-            if L is not None:
-                while np.max(pos[t,:, :])>L or np.min(pos[t,:, :])< 0: 
-                    pos[t, pos[t,:, :] > L] = pos[t, pos[t,:, :] > L] - 2*(pos[t, pos[t,:, :] > L] - L)
-                    pos[t, pos[t,:, :] < 0] = - pos[t, pos[t,:, :] < 0]  
-        
-        # Define state of particles based on values of alphas: either free or directed            
-        label_diff_state = np.zeros_like(alphas_t)
-        label_diff_state[alphas_t  < self.alpha_directed] = self.lab_state.index('f')
-        label_diff_state[alphas_t >= self.alpha_directed] = self.lab_state.index('d')
-        
-        if return_state_num:
-            return pos, np.array((alphas_t,
-                                  Ds_t, 
-                                  label_diff_state,
-                                  diff_state)).transpose(1,2,0)
-        else:
-            return pos, np.array((alphas_t,
-                                  Ds_t, 
-                                  label_diff_state
-                                 )).transpose(1,2,0)
-    
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 67
-class models_phenom(models_phenom):
-    @staticmethod
-    def _update_bound(mask, # Current binding array
-                      N, # Number of particles
-                      pos, # Position of particles
-                      Nt, # Number of traps
-                      traps_pos, # Position of traps
-                      Pb, # Binding probability
-                      Pu, # Unbinding probability
-                      r, # Trap radius
-                     ): # Updated binding array
-        '''
-        Binds and unbinds particles to traps based on their position and binding and unbinding probabilities
-        
-        Parameters
-        ----------
-        mask : array
-            Current binding array
-        N : int
-            Number of particles
-        pos : array
-            Position of particles
-        Nt : int
-            Number of traps
-        traps_pos : array
-            Position of traps
-        Pb : float in [0,1]
-            Binding probability
-        Pu : float in [0,1]
-            Unbinding probability
-        r : float
-            Trap radius
-            
-        Returns
-        -------
-        array
-            Updated binding array
-            
-        '''
-
-        # from the ones that are bound, get the ones that unbind. These will be descarted for binding in same time step
-        mask_new_free = np.array(1-(np.random.rand(N) < Pu)*mask).astype(bool)
-
-        # calculate the distance between traps and particles
-        d = models_phenom._get_distance(np.vstack((traps_pos, pos)))[Nt:, :Nt]
-        mask_close = (d < r).sum(1).astype(bool)
-
-        # get mask for binding
-        mask_new_bind = np.random.rand(N) < Pb
-
-        # update the bound vector with the previous conditions:
-        # first, the ones that unbind
-        mask *= mask_new_free
-        # then, the ones that are close + bind. Mask_new_free is added to avoid binding
-        # of the ones that just unbound
-        mask += mask_close*mask_new_bind*mask_new_free
-
-        return mask
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 69
-class models_phenom(models_phenom):
-
-    def immobile_traps(self,
-                       N = 10,
-                       T = 200,                
-                       L = 100,
-                       r = 1,
-                       Pu = 0.1, 
-                       Pb = 0.01, 
-                       Ds = [1, 0], 
-                       alphas = [1, 0], 
-                       Nt = 10,
-                       traps_pos: np.array = None,
-                       deltaT = 1
-                      ): 
-        '''
-        Generates a dataset of 2D trajectories of particles diffusing in an environment with immobilizing traps.
-        
-        Parameters
-        ----------
-        N : int
-            Number of trajectories
-        T : int
-            Length of the trajectory
-        L : float
-            Length of the box acting as the environment
-        r : float
-            Radius of particles.
-        Pu : float in [0,1]
-            Unbinding probability.
-        Pb : float in [0,1])
-            Binding probability.    
-        Ds : list, float
-            Mean and variance from which to sample the diffusion coefficient of the free state. If float, we consider variance = 0
-        alphas : list, float
-            Mean and variance from which to sample the anomalous exponent of the free state. If float, we consider variance = 0
-        Nt : int
-            Number of traps
-        traps_pos : array, None
-            Positions of the traps. Can be given by array or sampled randomly if None.
-        deltaT : int
-            Sampling time.            
-            
-        Returns
-        -------
-        tuple
-            - trajs (array TxNx2): particles' position
-            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels)
-            
-        '''
-
-        # Info to output
-        pos = np.zeros((T, N, 2)) # position over time
-        output_label = np.zeros((T, N, 3))        
-
-        disps = np.zeros((T, N, 2)) 
-        diff_state = np.zeros((T, N)).astype(int)
-        mask_bound = diff_state[0, :].astype(bool)
-
-        # Init position, labels     
-        pos[0, :, :] = np.random.rand(N, 2)*L
-        
-        # Init alphas, Ds
-        # Calculate alpha/D for each particle in state free state
-        alphas_N = gaussian(alphas, size = N, bound = self.bound_alpha)
-        Ds_N = gaussian(Ds, size = N, bound = self.bound_D)
-        
-        # Single particle case
-        if N == 1:
-            alphas_N = [alphas_N]
-            Ds_N = [Ds_N]
-
-        # Traps positions
-        if traps_pos is None:
-            traps_pos = np.random.rand(Nt, 2)*L              
-            
-        # Get displacement for every particle
-        for n in range(N):  
-            disps[:, n, 0] = models_phenom().disp_fbm(alphas_N[n], Ds_N[n], T, deltaT = deltaT)
-            disps[:, n, 1] = models_phenom().disp_fbm(alphas_N[n], Ds_N[n], T, deltaT = deltaT)
-            
-        # Set initial values of labels
-        output_label[0, :, 0] = alphas_N
-        output_label[0, :, 1] = Ds_N
-
-        for t in (range(1, T)):
-
-            mask_bound = self._update_bound(mask = mask_bound, # current bind vector
-                                         N = N, # number of particles
-                                         pos = pos[t-1, :, :], # position of particles
-                                         Nt = Nt, # number of traps
-                                         traps_pos = traps_pos, # position of traps
-                                         Pb = Pb, # binding probability
-                                         Pu = Pu, # unbinding probability
-                                         r = r, # trap radius
-                                         )
-            # Update the diffusive state
-            diff_state[t,:] = mask_bound
-
-            # Regenerate trajectories for untrapped particles
-            untrapped = np.argwhere((diff_state[t,:] - diff_state[t-1,:]) == -1).flatten()
-            for un_part in untrapped:
-                    if T-t > 1:
-                        # Recalculate new displacements for next steps                        
-                        disps[t:, un_part, 0] = models_phenom().disp_fbm(alphas_N[un_part], Ds_N[un_part], T-t, deltaT = deltaT)
-                        disps[t:, un_part, 1] = models_phenom().disp_fbm(alphas_N[un_part], Ds_N[un_part], T-t, deltaT = deltaT)
-
-                    else: 
-                        disps[t:, un_part, 0] = np.sqrt(2*Ds_N[un_part]*deltaT)*np.random.randn() 
-                        disps[t:, un_part, 1] = np.sqrt(2*Ds_N[un_part]*deltaT)*np.random.randn()
-
-            # Update the position
-            pos[t, :, :] = pos[t-1, :, :] + (1-mask_bound).reshape(N,1)*disps[t, :, :]
-
-            # Update labels
-            output_label[t, :, 0] = alphas_N*(1-mask_bound)
-            output_label[t, :, 1] = Ds_N*(1-mask_bound)
-
-            # Consider boundary conditions
-            if L is not None:
-                while np.max(pos[t,:, :])>L or np.min(pos[t,:, :])< 0: 
-                    pos[t, pos[t,:, :] > L] = pos[t, pos[t,:, :] > L] - 2*(pos[t, pos[t,:, :] > L] - L)
-                    pos[t, pos[t,:, :] < 0] = - pos[t, pos[t,:, :] < 0]
-                    
-        # Define state of particles based on values of Ds and alphas. Here, we use the fact 
-        # that alpha = 0 for immobilization
-        output_label[output_label[:,:,0] == 0, -1] = self.lab_state.index('i')
-        idx_f = np.argwhere
-        output_label[(output_label[:,:,0] > 0) & (output_label[:,:,0] < self.alpha_directed), -1] = self.lab_state.index('f')
-        output_label[output_label[:,:,0] > self.alpha_directed, -1] = self.lab_state.index('d')
-
-        return pos, output_label
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 76
-class models_phenom(models_phenom):
-    
-    @staticmethod
-    def _distribute_circular_compartments(Nc, r, L):
-        '''
-        Distributes circular compartments over an environment without overlapping. Raises a warning and stops when no more compartments can be inserted.                   
-        
-        Parameters
-        ----------
-        Nc : float
-            Number of compartments
-        r : float
-            Size of the compartments
-        L : float
-            Side length of the squared environment.
-            
-        Returns
-        -------
-        array
-            Position of the centers of the compartments
-        
-        '''
-
-        comp_center = np.random.rand(1, 2)*(L - 2*r) + r 
-        hardness = 0
-        while comp_center.shape[0] < Nc:
-
-            new_pos = np.random.rand(2)*(L - 2*r) + r
-
-            distance = np.linalg.norm(comp_center - new_pos, axis = 1)
-
-            if min(distance) > 2*r:
-                comp_center = np.vstack((comp_center, new_pos.reshape(1,2)))
-
-            hardness += 1
-            if hardness > Nc*100:
-                warn_str = f'Could accomodate {comp_center.shape[0]} circles of the {Nc} requested. Increase size of environment or decrease radius of compartments.'
-                warnings.warn(warn_str)
-                break
-        
-        return comp_center
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 80
-from .utils_trajectories import trigo
-
-class models_phenom(models_phenom):
-    
-    @staticmethod
-    def _reflected_position(circle_center, 
-                            circle_radius,
-                            beg, 
-                            end,
-                            precision_boundary = 1e-4):
-        '''
-        Given the begining and end of a segment crossing the boundary of a circle, calculates the new position considering that boundaries are fully reflective.
-        
-        Parameters
-        ----------
-        circle_center : float
-            Center of the circle            
-        circle_radius : float
-            Radius of the circle
-        beg : tuple
-            Position (in 2D) of the begining of the segment
-        end : tuple
-            Position (in 2D) of the begining of the segment
-        precision_boundary : float
-            Small area around the real boundary which is also considered as boundary. For numerical stability
-            
-        Returns
-        -------
-        tuple
-            - Reflected position
-            - Intersection point
-        
-        '''
-        
-        # If the begining of the segment is in the exact boundary, no intersection is found.
-        # In that case, we bring closer the point to the center of the cercle so it is
-        # at a distance 'precision_boundary' from the border
-        if np.linalg.norm(circle_center - beg) > circle_radius - precision_boundary:
-            vec = trigo.seg_to_vec([circle_center, beg])
-            beg = np.array(circle_center)+(circle_radius-precision_boundary)*(-np.array(vec)/np.dot(vec, vec)**0.5)
-            
-        # find the intersection between the line drawn by the displacement and the circle
-        intersect = trigo.circle_line_segment_intersection(circle_center = circle_center,
-                                                           circle_radius = circle_radius, 
-                                                           pt1 = beg,
-                                                           pt2 = end)[-1]
-        # Draw lines and calculate angles between radius and begining-intersection
-        line1 = [circle_center, intersect]
-        line2 = [beg, intersect]
-        angle = trigo.ang_line(line1, line2)
-        # Calculate distance between intersection and end of displacement
-        dist_int_end = np.linalg.norm(np.array(intersect) - end)
-        # Create radius vector and calculate the tangent vector
-        vec_radius = trigo.seg_to_vec([circle_center, intersect])
-        tangent = trigo.rotate_vec(vec_radius, np.pi/2) 
-        # Calculate the angle between the tangent and the displacement vector
-        angle_tan = trigo.ang_vec(tangent, trigo.seg_to_vec([beg, intersect]))
-        # Change sign to correct get the reflection
-        if angle_tan < np.pi/2: angle = - angle
-        # Rotate the radius vector with the reflection angle and normalize by magnitude
-        vec_bounce = trigo.rotate_vec(vec_radius, angle)
-        vec_bounce /= np.dot(vec_bounce, vec_bounce)**0.5
-        # Final point is the previous vector times the distance starting at the intersect point  
-        return np.array(intersect)+dist_int_end*np.array(vec_bounce), intersect
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 84
-class models_phenom(models_phenom):
-    
-    @staticmethod
-    def _confinement_traj(T = 200,
-                          L = 100,
-                          Ds = [1, 0.1],
-                          alphas = [1, 1],
-                          r = 1,
-                          comp_center = None,
-                          Nc = 10,
-                          trans = 0.1,
-                          deltaT = 1):
-        '''
-        Generates a 2D trajectory of particles diffusing in an environment with partially transmitting circular compartments.
-        
-        Parameters
-        ----------
-        T : int
-            Length of the trajectory
-        L : float
-            Length of the box acting as the environment 
-        Ds : list
-            Diffusion coefficients of the two diffusive states (first free, the confined). Size must be 2.
-        alphas : list
-            Anomalous exponents of the two diffusive states (first free, the confined). Size must be 2.
-        r : float
-            Radius of the compartments.             
-        comp_center : array, None
-            If given, center of the compartments. If None, centers are uniformly sampled.
-        Nc : int
-            Number of compartments
-        trans : float
-            Transmittance of the boundaries
-        deltaT : int
-            Sampling time.            
-            
-        Returns
-        -------
-        tuple
-            - pos (array Tx2): particle's position
-            - labels (array Tx2): particle's labels (see ._multi_state for details on labels)
-            
-        '''
-
-        
-        # transform lists to numpy if needed
-        if isinstance(Ds, list):
-            Ds = np.array(Ds)
-        if isinstance(alphas, list):
-            alphas = np.array(alphas)
-
-        # Traps positions
-        if comp_center is None:
-            comp_center = models_phenom._distribute_circular_compartments(Nc = Nc,
-                                                                          r = r,
-                                                                          L = L)
-        # Particle's properties
-        pos = np.zeros((T, 2)) 
-        pos[0,:] = np.random.rand(2)*L
-
-        state = np.zeros(T).astype(int)        
-        # Check if particle is compartment
-        distance_centers = np.linalg.norm(comp_center - pos[0, :], axis = 1)
-        if distance_centers.min() < r:
-            # we assign the state to the compartment the particle is on
-            compartment = distance_centers.argmin()
-            state[0] = 1
-
-        # Output labels
-        labels = np.zeros((T, 3))
-        labels[0, 0] = alphas[state[0]] 
-        labels[0, 1] = Ds[state[0]]         
-        
-
-        # Trajectory
-        dispx = models_phenom().disp_fbm(alphas[state[0]], Ds[state[0]], T, deltaT = deltaT)
-        dispy = models_phenom().disp_fbm(alphas[state[0]], Ds[state[0]], T, deltaT = deltaT)
-        disp_t = 0
-
-
-        for t in range(1, T):
-            pos[t, :] = [pos[t-1, 0]+dispx[disp_t], pos[t-1, 1]+dispy[disp_t]]  
-
-            # if the particle was inside a compartment
-            if state[t-1] == 1:
-
-                # check if it exited of the compartment
-                current_distance = np.linalg.norm(comp_center[compartment, :] - pos[t, :])                              
-                if current_distance > r:                    
-                    coin = np.random.rand()                    
-                    # particle escaping
-                    if coin < trans:                        
-                        # check that if we entered in a different comparmetn
-                        distance_centers = np.linalg.norm(comp_center - pos[t, :], axis = 1)
-                        if distance_centers.min() < r:
-                            # we assign the state to the compartment the particle is on
-                            compartment = distance_centers.argmin()
-                            state[t] = 1
-                        else: state[t] = 0
-
-                    # particle reflecting
-                    else:   
-                        beg = pos[t-1, :]
-                        while current_distance > r:
-
-                            pos[t, :], intersect = models_phenom._reflected_position(circle_center = comp_center[compartment, :],
-                                                                                     circle_radius = r,
-                                                                                     beg = beg,
-                                                                                     end = pos[t, :])
-                            beg = intersect
-                            distance_beg = np.linalg.norm(comp_center[compartment, :] - beg)    
-                            current_distance = np.linalg.norm(comp_center[compartment, :] - pos[t,:])  
-                        state[t] = 1
-                # if the particle stayed inside the compartment
-                else: state[t] = 1
-
-
-            # If particle was outside of the compartment
-            elif state[t-1] == 0:                
-                # Check if particle entered a new compartment
-                distance_centers = np.linalg.norm(comp_center - pos[t, :], axis = 1)
-                if distance_centers.min() < r:
-                    # we assign the state to the compartment the particle is on
-                    compartment = distance_centers.argmin()
-                    state[t] = 1
-                # if the particle stayed outside the comparments
-                else: state[t] = 0
-
-            # If the state changed
-            if state[t] != state[t-1]:
-                
-                if T-t > 1:
-                    dispx = models_phenom().disp_fbm(alphas[state[t]], Ds[state[t]], T-t, deltaT = deltaT)
-                    dispy = models_phenom().disp_fbm(alphas[state[t]], Ds[state[t]], T-t, deltaT = deltaT)
-                    
-                else: 
-                    dispx, dispy = [np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn(), 
-                                    np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn()]
-                disp_t = 0
-            # If the state did not change:
-            else: disp_t += 1
-            
-            # Boundary conditions
-            if L is not None:
-                # Reflecting boundary conditions
-                while np.max(pos[t, :])>L or np.min(pos[t, :])< 0: 
-                    pos[t, pos[t, :] > L] = pos[t, pos[t, :] > L] - 2*(pos[t, pos[t, :] > L] - L)
-                    pos[t, pos[t, :] < 0] = - pos[t, pos[t, :] < 0]
-
-
-            labels[t, 0] = alphas[state[t]] 
-            labels[t, 1] = Ds[state[t]] 
-            
-        # Define state of particles based on the state array. First free/directed
-        if alphas[0] < models_phenom().alpha_directed:
-            labels[state == 0, -1] = models_phenom().lab_state.index('f') 
-        else:
-            labels[state == 0, -1] = models_phenom().lab_state.index('d') 
-        # Then confined
-        labels[state == 1, -1] = models_phenom().lab_state.index('c')         
-        
-        return pos, labels
-        
-
-
-# %% ../source_nbs/lib_nbs/models_phenom.ipynb 88
-class models_phenom(models_phenom):
-    def confinement(self,
-                    N = 10,
-                    T = 200,
-                    L = 100,
-                    Ds = [[1, 0], [0.1, 0]], 
-                    alphas = [[1, 0], [1, 0]],
-                    gamma_d = [1], 
-                    epsilon_a = [0],
-                    r = 1,
-                    comp_center = None,
-                    Nc = 10,
-                    trans = 0.1, 
-                    deltaT = 1):
-        '''
-        Generates a dataset of 2D trajectories of particles diffusing in an environment with partially transmitting circular compartments.
-        
-        Parameters
-        ----------
-        N : int
-            Number of trajectories
-        T : int
-            Length of the trajectory
-        L : float
-            Length of the box acting as the environment 
-        Ds : list
-            List of means and variances from which to sample the diffusion coefficient of each state. If element size is one, we consider variance = 0.
-        alphas : float
-            List of means and variances from which to sample the anomalous exponent of each state. If element size is one, we consider variance = 0.       
-        gamma_d : list
-            Minimum factor between D of diffusive states (see ._sampling_diff_parameters). Size is number of states -1 (in this case size 1)
-        epsilon_a : list
-            Distance between alpha of diffusive states (see ._sampling_diff_parameters). Size is number of states -1 (in this case size 1)
-        r : float
-            Radius of the compartments.             
-        comp_center : array, None
-            If given, center of the compartments. If None, centers are uniformly sampled.
-        Nc : int
-            Number of compartments
-        trans : float
-            Transmittance of the boundaries
-        deltaT : int
-            Sampling time.  
-            
-        Returns
-        -------
-        tuple
-            - pos (array Tx2): particle's position
-            - labels (array Tx2): particle's labels (see ._multi_state for details on labels)
-            
-        '''
-       
-        if isinstance(Ds, list):
-            Ds = np.array(Ds)
-        if isinstance(alphas, list):
-            alphas = np.array(alphas)
-
-        data = np.zeros((T, N, 2))
-        labels = np.zeros((T, N, 3))
-
-        for n in range(N):
-            
-            # Defined physical parameters for each trajectory
-            alphas_traj, Ds_traj = self._sample_diff_parameters(alphas = alphas,
-                                                                Ds = Ds,
-                                                                num_states = 2,
-                                                                epsilon_a = epsilon_a,
-                                                                gamma_d = gamma_d)
-
-            # Get trajectory from single traj function
-            pos, lab = self._confinement_traj(T = T,
-                                              Ds = Ds_traj,
-                                              alphas = alphas_traj,
-                                              L = L,
-                                              deltaT = deltaT,
-                                              r = r,
-                                              comp_center = comp_center,
-                                              Nc = Nc,
-                                              trans = trans)
-            data[:, n, :] = pos
-            labels[:, n, :] = lab
-
-        return data, labels
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/models_phenom.ipynb.
+
+# %% auto 0
+__all__ = ['models_phenom']
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 2
+import numpy as np
+from stochastic.processes.noise import FractionalGaussianNoise as FGN
+from .utils_trajectories import gaussian
+import warnings
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 5
+class models_phenom():
+    def __init__(self):
+        '''
+        This class handles the generation of trajectories from different theoretical models. 
+        ''' 
+        # We define here the bounds of the anomalous exponent and diffusion coefficient
+        self.bound_D = [1e-12, 1e6]
+        self.bound_alpha = [0, 1.999]
+        
+        # We also define the value in which we consider directed motion
+        self.alpha_directed = 1.9
+        
+        # Diffusion state labels: the position of each type defines its numerical label
+        # i: immobile/trapped; c: confined; f: free-diffusive (normal and anomalous); d: directed
+        self.lab_state = ['i', 'c', 'f', 'd']
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 7
+class models_phenom(models_phenom):
+    
+    @staticmethod
+    def disp_fbm(alpha : float,
+                 D : float,
+                 T: int, 
+                 deltaT : int = 1):
+        ''' Generates normalized Fractional Gaussian noise. This means that, in 
+        general:
+        
+                            <x^2(t)> = 2Dt^alpha
+                            
+        and in particular:
+        
+                            <x^2(t = 1)> = 2D 
+        
+        Parameters
+        ----------
+        alpha : float in [0,2]
+            Anomalous exponent
+        D : float
+            Diffusion coefficient
+        T : int
+            Number of displacements to generate
+        deltaT : int, optional
+            Sampling time
+            
+        Returns
+        -------
+        numpy.array
+            Array containing T displacements of given parameters
+        
+        '''
+        
+        # Generate displacements
+        disp = FGN(hurst = alpha/2).sample(n = T)
+        # Normalization factor
+        disp *= np.sqrt(T)**(alpha)
+        # Add D
+        disp *= np.sqrt(2*D*deltaT)        
+        
+        return disp
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 15
+class models_phenom(models_phenom):
+    
+    @staticmethod
+    def _constraint_alpha(alpha_1, alpha_2, epsilon_a):
+        ''' Defines the metric for constraining the changes in anomalous
+        exponent'''
+        return alpha_1 - alpha_2 < epsilon_a
+    
+    @staticmethod
+    def _constraint_d(d1, d2, gamma_d):
+        ''' Defines the metric for constraining the changes in anomalous
+        exponent'''
+        if gamma_d < 1:
+            return d2 > d1*gamma_d
+        if gamma_d > 1:
+            return d2 < d1*gamma_d
+    
+    @staticmethod
+    def _sample_diff_parameters(alphas : list, # List containing the parameters to sample anomalous exponent in state (adapt to sampling function)
+                                Ds : list, # List containing the parameters to sample the diffusion coefficient in state (adapt to sampling function).
+                                num_states : int, # Number of diffusive states.
+                                epsilon_a : float, #  Minimum distance between anomalous exponents of various states.
+                                gamma_d : float, # Factor between diffusion coefficient of various states.
+                               ) : 
+        '''    
+        Given information of the anomalous exponents (alphas), diffusion coefficients (Ds), the function
+        samples these from a bounded Gaussian distribution with the indicated constraints (epsilon_a,
+        gamma_d). Outputs the list of demanded alphas and Ds.
+        
+        
+        Parameters
+        ----------
+        alphas : list
+        List containing the parameters to sample anomalous exponent in state (adapt to sampling function).
+        Ds : list
+        List containing the parameters to sample the diffusion coefficient in state (adapt to sampling function).
+        num_states : int
+        Number of diffusive states.
+        epsilon_a : float
+        Minimum distance between anomalous exponents of various states.            
+                epsilon workflow: we check val[i] - val[i-1] < epsilon
+                    if you want that val[i] > val[i-1]: epsilon has to be positive
+                    if you want that val[i] < val[i-1]: epsilon has to be negative
+                    if you don't care: epsilon = 0
+                
+        gamma_d : float
+        Factor between diffusion coefficient of various states.            
+                gamma workflow: 
+                    for gamma < 1: val[i] < val[i-1]*gamma
+                    for gamma > 1: val[i] > val[i-1]*gamma
+                    for gamma = 1: no check
+        Returns
+        -------
+            :alphas_traj (list): list of anomalous exponents
+            :Ds_traj (list): list of diffusion coefficients
+                      
+        '''
+
+        
+        alphas_traj = []
+        Ds_traj = []
+        for i in range(num_states): 
+
+            # for the first state we just sample normally
+            if i == 0:
+                alphas_traj.append(float(gaussian(alphas[i], bound = models_phenom().bound_alpha)))
+                Ds_traj.append(float(gaussian(Ds[i], bound = models_phenom().bound_D)))
+           
+            # For next states we take into account epsilon distance between diffusion
+            # parameter
+            else:
+                ## Checking alpha
+                alpha_state = float(gaussian(alphas[i], bound = models_phenom().bound_alpha))
+                D_state = float(gaussian(Ds[i], bound = models_phenom().bound_D))
+
+                if epsilon_a[i-1] != 0:
+                    idx_while = 0
+                    while models_phenom()._constraint_alpha(alphas_traj[-1], alpha_state, epsilon_a[i-1]):
+                    #alphas_traj[-1] - alpha_state < epsilon_a[i-1]:
+                        alpha_state = float(gaussian(alphas[i], bound = models_phenom().bound_alpha))                        
+                        idx_while += 1
+                        if idx_while > 100: # check that we are not stuck forever in the while loop
+                            raise FileNotFoundError(f'Could not find correct alpha for state {i} in 100 steps. State distributions probably too close.')
+
+                alphas_traj.append(alpha_state)
+                
+                ## Checking D
+                if gamma_d[i-1] != 1:    
+                    
+                    idx_while = 0
+                    while models_phenom()._constraint_d(Ds_traj[-1], D_state, gamma_d[i-1]):
+                        D_state = float(gaussian(Ds[i], bound = models_phenom().bound_D))
+                        idx_while += 1
+                        if idx_while > 100: # check that we are not stuck forever in the while loop
+                            raise FileNotFoundError(f'Could not find correct D for state {i} in 100 steps. State distributions probably too close.')
+               
+    
+                Ds_traj.append(D_state)
+                
+        return alphas_traj, Ds_traj
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 23
+class models_phenom(models_phenom):
+    
+    @staticmethod
+    def _single_state_traj(T :int = 200, 
+                          D : float = 1, 
+                          alpha : float = 1, 
+                          L : float = None,
+                          deltaT : int = 1):
+        '''
+        Generates a single state trajectory with given parameters. 
+        
+        Parameters
+        ----------
+        T : int
+            Length of the trajectory
+        D : float
+            Diffusion coefficient       
+        alpha : float
+            Anomalous exponent
+        L : float
+            Length of the box acting as the environment
+        deltaT : int, optional
+            Sampling time
+            
+        Returns
+        -------
+        tuple
+            - pos: position of the particle
+            - labels:  anomalous exponent, D and state at each timestep. State is always free here.
+            
+        '''
+        
+        
+        # Trajectory displacements
+        dispx, dispy = models_phenom().disp_fbm(alpha, D, T), models_phenom().disp_fbm(alpha, D, T)
+        # Labels
+        lab_diff_state = np.ones(T)*models_phenom().lab_state.index('f') if alpha < models_phenom().alpha_directed else np.ones(T)*models_phenom().lab_state.index('d')
+        labels = np.vstack((np.ones(T)*alpha, 
+                            np.ones(T)*D,
+                            lab_diff_state
+                           )).transpose()
+
+        # If there are no boundaries
+        if not L:
+            posx, posy = np.cumsum(dispx) - dispx[0], np.cumsum(dispy) - dispy[0]
+
+            return np.vstack((posx, posy)).transpose(), labels
+
+        # If there are, apply reflecting boundary conditions
+        else:
+            pos = np.zeros((T, 2))
+
+            # Initialize the particle in a random position of the box
+            pos[0, :] = np.random.rand(2)*L
+            for t in range(1, T):
+                pos[t, :] = [pos[t-1, 0]+dispx[t], pos[t-1, 1]+dispy[t]]            
+
+
+                # Reflecting boundary conditions
+                while np.max(pos[t, :])>L or np.min(pos[t, :])< 0: 
+                    pos[t, pos[t, :] > L] = pos[t, pos[t, :] > L] - 2*(pos[t, pos[t, :] > L] - L)
+                    pos[t, pos[t, :] < 0] = - pos[t, pos[t, :] < 0]
+
+            return pos, labels
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 27
+class models_phenom(models_phenom):
+    
+    
+    def single_state(self,
+                     N:int = 10,
+                     T:int = 200, 
+                     Ds:list = [1, 0], 
+                     alphas:list = [1, 0], 
+                     L:float = None):
+        '''
+        Generates a dataset made of single state trajectories with given parameters.
+        
+        Parameters
+        ----------
+        N : int, list
+            Number of trajectories in the dataset
+        T : int
+            Length of the trajectory
+        Ds : float
+            If list, mean and variance from which to sample the diffusion coefficient. If float, we consider variance = 0.
+        alphas : float
+            If list, mean and variance from which to sample the anomalous exponent. If float, we consider variance = 0.
+        L : float
+            Length of the box acting as the environment
+        deltaT : int, optional
+            Sampling time
+            
+        Returns
+        -------
+        tuple
+            - positions: position of the N trajectories.
+            - labels:  anomalous exponent, D and state at each timestep. State is always free here.         
+        '''
+
+        positions = np.zeros((T, N, 2))
+        labels = np.zeros((T, N, 3))
+
+        for n in range(N):
+            alpha_traj = gaussian(alphas, bound = self.bound_alpha)
+            D_traj = gaussian(Ds, bound = self.bound_D)
+            # Get trajectory from single traj function
+            pos, lab = self._single_state_traj(T = T, 
+                                   D = D_traj, 
+                                   alpha = alpha_traj, 
+                                   L = L)        
+            positions[:, n, :] = pos
+            labels[:, n, :] = lab
+
+        return positions, labels
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 33
+class models_phenom(models_phenom):
+    
+    @staticmethod
+    def _multiple_state_traj(T = 200, 
+                             M = [[0.95 , 0.05],[0.05 ,0.95]], 
+                             Ds = [1, 0.1], 
+                             alphas = [1, 1], 
+                             L = None,
+                             deltaT = 1,
+                             return_state_num = False, 
+                             init_state = None
+                            ):
+        
+        '''
+        Generates a 2D multi state trajectory with given parameters.        
+        
+        Parameters
+        ----------
+        T : int
+            Length of the trajectory
+        M : list, array
+            Transition matrix between diffusive states.        
+        Ds : list
+            Diffusion coefficients of the diffusive states. Must have as many Ds as states defined by M.
+        alphas : list
+            Anomalous exponents of the diffusive states. Must have as many alphas as states defined by M.
+        L : float
+            Length of the box acting as the environment
+        deltaT : int, optional
+            Sampling time
+        return_state_num : bool
+            If True, returns as label the number assigned to the state at each time step.
+        init_state : bool
+            If True, the particle starts in state 0. If not, sample initial state.
+            
+            
+        Returns
+        -------
+        tuple
+            - pos: position of the particle
+            - alphas_t: anomalous exponent at each  step
+            - Ds_t: diffusion coefficient at each step. 
+            - label_diff_state: particle's state (can be either free or directed for alpha ~ 2) at each step.
+            - state (optional): state label at each step.            
+        
+        '''
+        
+        # transform lists to numpy if needed
+        if isinstance(M, list):
+            M = np.array(M)
+        if isinstance(Ds, list):
+            Ds = np.array(Ds)
+        if isinstance(alphas, list):
+            alphas = np.array(alphas)
+
+
+        pos = np.zeros((T, 2))
+        if L: pos[0,:] = np.random.rand(2)*L
+
+        # Diffusing state of the particle
+        state = np.zeros(T).astype(int)
+        if init_state is None:
+            state[0] = np.random.randint(M.shape[0])
+        else: state[0] = init_state
+        
+        # Init alphas, Ds
+        alphas_t = np.array(alphas[state[0]]).repeat(T)
+        Ds_t = np.array(Ds[state[0]]).repeat(T)
+        
+        
+        # Trajectory displacements    
+        dispx, dispy = [models_phenom().disp_fbm(alphas_t[0], Ds_t[0], T),
+                        models_phenom().disp_fbm(alphas_t[0], Ds_t[0], T)]
+
+
+        for t in range(1, T):
+
+            pos[t, :] = [pos[t-1, 0]+dispx[t], pos[t-1, 1]+dispy[t]]  
+
+            # at each time, check new state
+            state[t] = np.random.choice(np.arange(M.shape[0]), p = M[state[t-1], :])
+
+
+            if state[t] != state[t-1]:
+                
+                alphas_t[t:] =  np.array(alphas[state[t]]).repeat(T-t)  
+                Ds_t[t:] = np.array(Ds[state[t]]).repeat(T-t)
+                
+                
+                # Recalculate new displacements for next steps
+                if len(dispx[t:]) > 1:                    
+                    dispx[t:], dispy[t:] = [models_phenom().disp_fbm(alphas_t[t], Ds_t[t], T-t),
+                                            models_phenom().disp_fbm(alphas_t[t], Ds_t[t], T-t)]
+                        
+                        
+                else: 
+                    dispx[t:], dispy[t:] = [np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn(), 
+                                            np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn()]
+                    
+
+            if L is not None:
+                # Reflecting boundary conditions
+                while np.max(pos[t, :])>L or np.min(pos[t, :])< 0: 
+                    pos[t, pos[t, :] > L] = pos[t, pos[t, :] > L] - 2*(pos[t, pos[t, :] > L] - L)
+                    pos[t, pos[t, :] < 0] = - pos[t, pos[t, :] < 0]
+                    
+        # Define state of particles based on values of alphas: either free or directed
+        label_diff_state = np.zeros_like(alphas_t)
+        label_diff_state[alphas_t  < models_phenom().alpha_directed] = models_phenom().lab_state.index('f')
+        label_diff_state[alphas_t >= models_phenom().alpha_directed] = models_phenom().lab_state.index('d')
+                    
+        if return_state_num:            
+            return pos, np.array((alphas_t,
+                                  Ds_t,
+                                  label_diff_state,
+                                  state)).transpose()
+        else: 
+            return pos, np.array((alphas_t,
+                                  Ds_t,
+                                  label_diff_state)).transpose()
+        
+
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 37
+class models_phenom(models_phenom):
+    def multi_state(self,
+                    N = 10,
+                    T = 200,
+                    M: np.array = [[0.9 , 0.1],[0.1 ,0.9]],
+                    Ds: np.array = [[1, 0], [0.1, 0]], 
+                    alphas: np.array = [[1, 0], [1, 0]], 
+                    gamma_d = [1], 
+                    epsilon_a = [0], 
+                    L = None,
+                    return_state_num = False,
+                    init_state = None): 
+        '''
+        Generates a dataset of 2D multi state trajectory with given parameters.
+        
+        Parameters
+        ----------
+        N : int
+            Number of trajectories
+        T : int
+            Length of the trajectory
+        M : list, array
+            Transition matrix between diffusive states
+        Ds : list
+            List of means and variances from which to sample the diffusion coefficient of each state. If element size is one, we consider variance = 0.
+        alphas : float
+            List of means and variances from which to sample the anomalous exponent of each state. If element size is one, we consider variance = 0.   
+        gamma_d : list
+            Minimum factor between D of diffusive states (see ._sampling_diff_parameters)
+        epsilon_a : list
+            Distance between alpha of diffusive states (see ._sampling_diff_parameters)
+        L : float
+            Length of the box acting as the environment
+        deltaT : int, optional
+            Sampling time
+        return_state_num : bool
+            If True, returns as label the number assigned to the state at each time step.
+        init_state : bool
+            If True, the particle starts in state 0. If not, sample initial state.
+            
+            
+        Returns
+        -------
+        tuple
+            - trajs (array TxNx2): particles' position
+            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels)           
+        
+        '''
+        
+        # transform lists to numpy if needed
+        if isinstance(M, list):
+            M = np.array(M)
+        if isinstance(Ds, list):
+            Ds = np.array(Ds)
+        if isinstance(alphas, list):
+            alphas = np.array(alphas)
+        
+        
+
+        trajs = np.zeros((T, N, 2))
+        if return_state_num:
+            labels = np.zeros((T, N, 4))
+        else:
+            labels = np.zeros((T, N, 3))
+
+        for n in range(N):
+            
+            ### Sampling diffusion parameters for each state
+            alphas_traj = []
+            Ds_traj = []
+            
+            alphas_traj, Ds_traj = self._sample_diff_parameters(alphas = alphas,
+                                                                Ds = Ds,
+                                                                num_states = M.shape[0],
+                                                                epsilon_a = epsilon_a,
+                                                                gamma_d = gamma_d)
+                    
+            #### Get trajectory from single traj function
+            traj, lab = self._multiple_state_traj(T = T,
+                                                  L = L,
+                                                  M = M,
+                                                  alphas = alphas_traj,
+                                                  Ds = Ds_traj,
+                                                  return_state_num = return_state_num,
+                                                  init_state = init_state
+                                                 )  
+                
+            trajs[:, n, :] = traj
+            labels[:, n, :] = lab 
+            
+        return trajs, labels
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 46
+class models_phenom(models_phenom):
+    @staticmethod
+    def _get_distance(x):
+        '''
+        Given a matrix of size Nx2, calculates the distance between the N particles.
+        
+        Parameters
+        ----------
+        x : array
+            Particles' positions
+            
+        Returns
+        -------
+        array
+            Distance between particles         
+        
+        '''
+        
+        M = np.reshape(np.repeat(x[ :, :], x.shape[0], axis = 0), (x.shape[0], x.shape[0], 2))
+        Mtrans = M.transpose(1,0,2)
+        distance = np.sqrt(np.square(M[:,:, 0]-Mtrans[:,:, 0])
+                         + np.square(M[:,:, 1]-Mtrans[:,:, 1]))  
+        return distance
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 49
+class models_phenom(models_phenom):
+    @staticmethod
+    def _make_escape(Pu, label, diff_state):
+        ''' 
+        Given an unbinding probablity (Pu), the current labeling of particles (label)
+        and the current state of particle (diff_state, either bound, 1, or unbound, 0), simulate an
+        stochastic binding mechanism. 
+        
+        Parameters
+        ----------
+        Pu : float
+            Unbinding probablity
+        label : array
+            Current labeling of the particles (i.e. to which condensate they belong)
+        diff_state : array
+            Current state of the particles
+            
+        Returns
+        -------
+        tuple
+            New labeling and diffusive state of the particles        
+        
+        '''
+
+        # if unbinding probability is zero
+        if Pu == 0:
+            return label, diff_state
+
+        label = label.copy()
+        diff_state = diff_state.copy()
+
+        label_dimers = np.unique(label[np.argwhere(diff_state == 1)])
+
+        for l in label_dimers:         
+
+            if np.random.rand() < Pu:
+                # give new label to escaping particles
+                diff_state[label == l] = 0
+                label[label == l] = np.max(label)+np.arange(2)+1
+
+        return label, diff_state
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 52
+class models_phenom(models_phenom):
+    @staticmethod
+    def _make_condensates(Pb, label, diff_state, r, distance, max_label):
+        '''
+        Given a binding probability Pb, the current label of particles (label),
+        their current diffusive state (diff_state), the particle size (r), their 
+        distances (distance) and the label from which binding is not possible 
+        (max_label), simulates a binding mechanism.
+                
+        Parameters
+        ----------
+        Pb : float
+            Binding probablity.
+        label : array
+            Current labeling of the particles (i.e. to which condensate they belong)
+        diff_state : array
+            Current state of the particles
+        r : float
+            Particle size.
+        distance : array
+            Distance between particles
+        max_label : int
+            Maximum label from which particles will not be considered for binding
+            
+        Returns
+        -------
+        tuple
+            New labeling and diffusive state of the particles
+        '''
+
+        label = label.copy()
+        diff_state = diff_state.copy()
+
+        # Keeping track of the ones that will dimerize
+        already_dimer = []
+
+        for n, l in enumerate(label):
+
+            # Consider conditions in which particles do not dimerize
+            if n in already_dimer or diff_state[n] == 1 or l > max_label:
+                continue
+
+            # Extract distances to current particle
+            distance_to_current = distance[n,:]
+            distance_to_current[n] == 0
+            close_particles = np.argwhere((distance_to_current < 2*r) & (distance_to_current > 0)).flatten()
+
+            # Loop over all posible dimerizing candidates
+            for chosen in close_particles:
+
+                # Consider conditions in which particles do not dimerize
+                if chosen in already_dimer or diff_state[chosen] == 1 or label[chosen] > max_label: 
+                    continue
+
+                # Draw coin to see if particle dimerizes
+                if np.random.rand() < Pb:                                 
+                    # Add dimerized particles to the new dimer counter
+                    already_dimer.append(chosen)
+                    already_dimer.append(n)
+                    # Update their diffusive state
+                    diff_state[n] = 1
+                    diff_state[chosen] = 1 
+
+                    # dimerize particles
+                    label[chosen] = l
+
+                    # if one particles dimers, not more clustering!
+                    break
+
+        return label, diff_state
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 57
+class models_phenom(models_phenom):
+    @staticmethod
+    def _stokes(D):
+        '''
+        Applies a Stokes-Einstein-like transformation to two diffusion coefficients.        
+                
+        Parameters
+        ----------
+        D : tuple
+            Diffusion coefficients of the two binding particles.
+            
+        Returns
+        -------
+        float
+            Resulting diffusion coefficient.
+        '''
+        
+        D1 = D[0]; D2 = D[1]
+        return 1/((1/D1)+(1/D2))
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 60
+class models_phenom(models_phenom):
+    def dimerization(self,
+                     N = 10,
+                     T = 200,                
+                     L = 100,
+                     r = 1,
+                     Pu = 0.1, 
+                     Pb = 0.01,
+                     Ds: np.array = [[1, 0], [0.1, 0]],
+                     alphas: np.array = [[1, 0], [1, 0]],
+                     epsilon_a = 0, stokes = False,
+                     return_state_num = False,
+                     deltaT = 1
+                     ):
+        '''
+        Generates a dataset of 2D trajectories of particles perfoming stochastic dimerization.
+        
+        Parameters
+        ----------
+        N : int
+            Number of trajectories
+        T : int
+            Length of the trajectory
+        L : float
+            Length of the box acting as the environment
+        r : float
+            Radius of particles.
+        Pu : float in [0,1]
+            Unbinding probability.
+        Pb : float in [0,1])
+            Binding probability.    
+        Ds : array
+            List of means and variances from which to sample the diffusion coefficient of each state. If element size is one, we consider variance = 0.
+        alphas : array
+            List of means and variances from which to sample the anomalous exponent of each state. If element size is one, we consider variance = 0.   
+        epsilon_a : float
+            Distance between alpha of diffusive states (see ._sampling_diff_parameters)           
+        stokes : bool
+            If True, applies a Stokes-Einstein like coefficient to calculate the diffusion coefficient of dimerized particles.  
+            If False, we use as D resulting from the dimerization the D assigned to the dimerized state of one of the two particles.
+        deltaT : int
+            Sampling time
+        return_state_num : bool
+            If True, returns as label the number assigned to the state at each time step.            
+            
+        Returns
+        -------
+        tuple
+            - trajs (array TxNx2): particles' position
+            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels)
+            
+        '''
+        
+        # transform lists to numpy if needed
+        if isinstance(Ds, list):
+            Ds = np.array(Ds)
+        if isinstance(alphas, list):
+            alphas = np.array(alphas)
+
+        # Info to save
+        pos = np.zeros((T, N, 2)) # position over time
+        label = np.zeros((T, N)).astype(int)
+        diff_state = np.zeros((T, N)).astype(int)
+
+        # Init position, labels     
+        pos[0, :, :] = np.random.rand(N, 2)*L    
+        label[0, :] = np.arange(pos.shape[1])
+        
+        # Init alphas, Ds
+        # Calculate alpha/D for each particle in each state
+        alphas_N = np.array([gaussian(alphas[0], size = N, bound = self.bound_alpha),
+                             gaussian(alphas[1], size = N, bound = self.bound_alpha)])
+        Ds_N = np.array([gaussian(Ds[0], size = N, bound = self.bound_D),
+                         gaussian(Ds[1], size = N, bound = self.bound_D)])
+        # define labels over time by means of state 0
+        alphas_t = alphas_N[0,:].repeat(T).reshape(N,T).transpose()
+        Ds_t = Ds_N[0,:].repeat(T).reshape(N,T).transpose()
+        
+                
+        # initial displacements (all free particles)
+        disps = np.zeros((T, N, 2))
+        for n in range(N):            
+            disps[:, n, 0] = models_phenom().disp_fbm(alphas_t[0, n], Ds_t[0, n], T, deltaT = deltaT)
+            disps[:, n, 1] = models_phenom().disp_fbm(alphas_t[0, n], Ds_t[0, n], T, deltaT = deltaT)
+   
+        for t in (range(1, T)):
+
+            # Find max label to account later for escaped
+            max_label = np.max(label[t-1, :])
+
+            # Make particles escape
+            label[t, :], diff_state[t, :] = self._make_escape(Pu,
+                                                              label[t-1, :], 
+                                                              diff_state[t-1, :])
+
+            lab, diff = label[t, :].copy(), diff_state[t, :].copy()
+
+            # get distance + increasing it for escaped to avoid reclustering
+            distance = self._get_distance(pos[t-1, :, :])
+
+            # Merge particles in condensates
+            label[t, :], diff_state[t, :] = self._make_condensates(Pb,
+                                                                 label[t, :],
+                                                                 diff_state[t, :],
+                                                                 r, distance, max_label)
+
+            # Find particles which changed state
+            label_changed, counts = np.unique(label[t, np.not_equal(diff_state[t-1,:], diff_state[t,:])], 
+                                              return_counts = True)
+
+            # Calculate new displacements for particles which changed state
+            for l, count in zip(label_changed, counts):
+
+                index = int(np.argwhere(label[t,:] == l)[0])
+                state = diff_state[t, index]
+                
+                
+                ### Calculating new diffusion parameters
+                # anomalous exponent
+                if epsilon_a != 0 and state == 1:                    
+                    new_alpha = gaussian(alphas[1], size = 1, bound = self.bound_alpha)
+                    idx_while = 0
+                    while models_phenom()._constraint_alpha(alphas_N[0, label[t, :] == l].min(), new_alpha, epsilon_a):
+                        new_alpha = gaussian(alphas[1], size = 1, bound = self.bound_alpha)
+                        idx_while += 1
+                        if idx_while > 100: # check that we are not stuck forever in the while loop
+                            raise FileNotFoundError(f'Could not find correct alpha in 100 steps. State distributions probably too close.')
+                    alphas_t[t:, label[t, :] == l] = new_alpha
+                else: 
+                    # if no epsilon is given, use the alpha of the first particle
+                    # While here it seems we take both, in the for loop where we assign the displacements below we only
+                    # sample with the first value.
+                    alphas_t[t:, label[t, :] == l] = alphas_N[state, label[t, :] == l].repeat(T-t).reshape(count, T-t).transpose()
+                    
+                # diffusion coefficient
+                if stokes and state == 1:
+                    Ds_t[t:, label[t, :] == l] = models_phenom()._stokes(Ds_t[t-1, label[t, :] == l])
+                else: # if no stokes is given, use the D assgined to the dimerized state of the first particle 
+                    Ds_t[t:, label[t, :] == l] = Ds_N[state, label[t, :] == l].repeat(T-t).reshape(count, T-t).transpose()
+                    
+                for idx, i in enumerate(np.argwhere(label[t,:] == l)):
+                    # We first calculate the displacements so dimers have same motion
+                    if idx == 0:                        
+                        if T-t > 1:                       
+                            disp_current_x = models_phenom().disp_fbm(float(alphas_t[t, i]), float(Ds_t[t, i]), T-t, deltaT = deltaT).reshape(T-t, 1)
+                            disp_current_y = models_phenom().disp_fbm(float(alphas_t[t, i]), float(Ds_t[t, i]), T-t, deltaT = deltaT).reshape(T-t, 1)
+                        else: 
+                            disp_current_x = np.sqrt(2*float(Ds_t[t, i])*deltaT)*np.random.randn(1)
+                            disp_current_y = np.sqrt(2*float(Ds_t[t, i])*deltaT)*np.random.randn(1)
+                            
+                    disps[t:, i, 0] = disp_current_x
+                    disps[t:, i, 1] = disp_current_y
+
+            # Update position
+            pos[t, :, :] = pos[t-1,:,:]+disps[t, :, :]
+            # Consider boundary conditions
+            if L is not None:
+                while np.max(pos[t,:, :])>L or np.min(pos[t,:, :])< 0: 
+                    pos[t, pos[t,:, :] > L] = pos[t, pos[t,:, :] > L] - 2*(pos[t, pos[t,:, :] > L] - L)
+                    pos[t, pos[t,:, :] < 0] = - pos[t, pos[t,:, :] < 0]  
+        
+        # Define state of particles based on values of alphas: either free or directed            
+        label_diff_state = np.zeros_like(alphas_t)
+        label_diff_state[alphas_t  < self.alpha_directed] = self.lab_state.index('f')
+        label_diff_state[alphas_t >= self.alpha_directed] = self.lab_state.index('d')
+        
+        if return_state_num:
+            return pos, np.array((alphas_t,
+                                  Ds_t, 
+                                  label_diff_state,
+                                  diff_state)).transpose(1,2,0)
+        else:
+            return pos, np.array((alphas_t,
+                                  Ds_t, 
+                                  label_diff_state
+                                 )).transpose(1,2,0)
+    
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 67
+class models_phenom(models_phenom):
+    @staticmethod
+    def _update_bound(mask, # Current binding array
+                      N, # Number of particles
+                      pos, # Position of particles
+                      Nt, # Number of traps
+                      traps_pos, # Position of traps
+                      Pb, # Binding probability
+                      Pu, # Unbinding probability
+                      r, # Trap radius
+                     ): # Updated binding array
+        '''
+        Binds and unbinds particles to traps based on their position and binding and unbinding probabilities
+        
+        Parameters
+        ----------
+        mask : array
+            Current binding array
+        N : int
+            Number of particles
+        pos : array
+            Position of particles
+        Nt : int
+            Number of traps
+        traps_pos : array
+            Position of traps
+        Pb : float in [0,1]
+            Binding probability
+        Pu : float in [0,1]
+            Unbinding probability
+        r : float
+            Trap radius
+            
+        Returns
+        -------
+        array
+            Updated binding array
+            
+        '''
+
+        # from the ones that are bound, get the ones that unbind. These will be descarted for binding in same time step
+        mask_new_free = np.array(1-(np.random.rand(N) < Pu)*mask).astype(bool)
+
+        # calculate the distance between traps and particles
+        d = models_phenom._get_distance(np.vstack((traps_pos, pos)))[Nt:, :Nt]
+        mask_close = (d < r).sum(1).astype(bool)
+
+        # get mask for binding
+        mask_new_bind = np.random.rand(N) < Pb
+
+        # update the bound vector with the previous conditions:
+        # first, the ones that unbind
+        mask *= mask_new_free
+        # then, the ones that are close + bind. Mask_new_free is added to avoid binding
+        # of the ones that just unbound
+        mask += mask_close*mask_new_bind*mask_new_free
+
+        return mask
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 69
+class models_phenom(models_phenom):
+
+    def immobile_traps(self,
+                       N = 10,
+                       T = 200,                
+                       L = 100,
+                       r = 1,
+                       Pu = 0.1, 
+                       Pb = 0.01, 
+                       Ds = [1, 0], 
+                       alphas = [1, 0], 
+                       Nt = 10,
+                       traps_pos: np.array = None,
+                       deltaT = 1
+                      ): 
+        '''
+        Generates a dataset of 2D trajectories of particles diffusing in an environment with immobilizing traps.
+        
+        Parameters
+        ----------
+        N : int
+            Number of trajectories
+        T : int
+            Length of the trajectory
+        L : float
+            Length of the box acting as the environment
+        r : float
+            Radius of particles.
+        Pu : float in [0,1]
+            Unbinding probability.
+        Pb : float in [0,1])
+            Binding probability.    
+        Ds : list, float
+            Mean and variance from which to sample the diffusion coefficient of the free state. If float, we consider variance = 0
+        alphas : list, float
+            Mean and variance from which to sample the anomalous exponent of the free state. If float, we consider variance = 0
+        Nt : int
+            Number of traps
+        traps_pos : array, None
+            Positions of the traps. Can be given by array or sampled randomly if None.
+        deltaT : int
+            Sampling time.            
+            
+        Returns
+        -------
+        tuple
+            - trajs (array TxNx2): particles' position
+            - labels (array TxNx2): particles' labels (see ._multi_state for details on labels)
+            
+        '''
+
+        # Info to output
+        pos = np.zeros((T, N, 2)) # position over time
+        output_label = np.zeros((T, N, 3))        
+
+        disps = np.zeros((T, N, 2)) 
+        diff_state = np.zeros((T, N)).astype(int)
+        mask_bound = diff_state[0, :].astype(bool)
+
+        # Init position, labels     
+        pos[0, :, :] = np.random.rand(N, 2)*L
+        
+        # Init alphas, Ds
+        # Calculate alpha/D for each particle in state free state
+        alphas_N = gaussian(alphas, size = N, bound = self.bound_alpha)
+        Ds_N = gaussian(Ds, size = N, bound = self.bound_D)
+        
+        # Single particle case
+        if N == 1:
+            alphas_N = [alphas_N]
+            Ds_N = [Ds_N]
+
+        # Traps positions
+        if traps_pos is None:
+            traps_pos = np.random.rand(Nt, 2)*L              
+            
+        # Get displacement for every particle
+        for n in range(N):  
+            disps[:, n, 0] = models_phenom().disp_fbm(alphas_N[n], Ds_N[n], T, deltaT = deltaT)
+            disps[:, n, 1] = models_phenom().disp_fbm(alphas_N[n], Ds_N[n], T, deltaT = deltaT)
+            
+        # Set initial values of labels
+        output_label[0, :, 0] = alphas_N
+        output_label[0, :, 1] = Ds_N
+
+        for t in (range(1, T)):
+
+            mask_bound = self._update_bound(mask = mask_bound, # current bind vector
+                                         N = N, # number of particles
+                                         pos = pos[t-1, :, :], # position of particles
+                                         Nt = Nt, # number of traps
+                                         traps_pos = traps_pos, # position of traps
+                                         Pb = Pb, # binding probability
+                                         Pu = Pu, # unbinding probability
+                                         r = r, # trap radius
+                                         )
+            # Update the diffusive state
+            diff_state[t,:] = mask_bound
+
+            # Regenerate trajectories for untrapped particles
+            untrapped = np.argwhere((diff_state[t,:] - diff_state[t-1,:]) == -1).flatten()
+            for un_part in untrapped:
+                    if T-t > 1:
+                        # Recalculate new displacements for next steps                        
+                        disps[t:, un_part, 0] = models_phenom().disp_fbm(alphas_N[un_part], Ds_N[un_part], T-t, deltaT = deltaT)
+                        disps[t:, un_part, 1] = models_phenom().disp_fbm(alphas_N[un_part], Ds_N[un_part], T-t, deltaT = deltaT)
+
+                    else: 
+                        disps[t:, un_part, 0] = np.sqrt(2*Ds_N[un_part]*deltaT)*np.random.randn() 
+                        disps[t:, un_part, 1] = np.sqrt(2*Ds_N[un_part]*deltaT)*np.random.randn()
+
+            # Update the position
+            pos[t, :, :] = pos[t-1, :, :] + (1-mask_bound).reshape(N,1)*disps[t, :, :]
+
+            # Update labels
+            output_label[t, :, 0] = alphas_N*(1-mask_bound)
+            output_label[t, :, 1] = Ds_N*(1-mask_bound)
+
+            # Consider boundary conditions
+            if L is not None:
+                while np.max(pos[t,:, :])>L or np.min(pos[t,:, :])< 0: 
+                    pos[t, pos[t,:, :] > L] = pos[t, pos[t,:, :] > L] - 2*(pos[t, pos[t,:, :] > L] - L)
+                    pos[t, pos[t,:, :] < 0] = - pos[t, pos[t,:, :] < 0]
+                    
+        # Define state of particles based on values of Ds and alphas. Here, we use the fact 
+        # that alpha = 0 for immobilization
+        output_label[output_label[:,:,0] == 0, -1] = self.lab_state.index('i')
+        idx_f = np.argwhere
+        output_label[(output_label[:,:,0] > 0) & (output_label[:,:,0] < self.alpha_directed), -1] = self.lab_state.index('f')
+        output_label[output_label[:,:,0] > self.alpha_directed, -1] = self.lab_state.index('d')
+
+        return pos, output_label
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 76
+class models_phenom(models_phenom):
+    
+    @staticmethod
+    def _distribute_circular_compartments(Nc, r, L):
+        '''
+        Distributes circular compartments over an environment without overlapping. Raises a warning and stops when no more compartments can be inserted.                   
+        
+        Parameters
+        ----------
+        Nc : float
+            Number of compartments
+        r : float
+            Size of the compartments
+        L : float
+            Side length of the squared environment.
+            
+        Returns
+        -------
+        array
+            Position of the centers of the compartments
+        
+        '''
+
+        comp_center = np.random.rand(1, 2)*(L - 2*r) + r 
+        hardness = 0
+        while comp_center.shape[0] < Nc:
+
+            new_pos = np.random.rand(2)*(L - 2*r) + r
+
+            distance = np.linalg.norm(comp_center - new_pos, axis = 1)
+
+            if min(distance) > 2*r:
+                comp_center = np.vstack((comp_center, new_pos.reshape(1,2)))
+
+            hardness += 1
+            if hardness > Nc*100:
+                warn_str = f'Could accomodate {comp_center.shape[0]} circles of the {Nc} requested. Increase size of environment or decrease radius of compartments.'
+                warnings.warn(warn_str)
+                break
+        
+        return comp_center
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 80
+from .utils_trajectories import trigo
+
+class models_phenom(models_phenom):
+    
+    @staticmethod
+    def _reflected_position(circle_center, 
+                            circle_radius,
+                            beg, 
+                            end,
+                            precision_boundary = 1e-4):
+        '''
+        Given the begining and end of a segment crossing the boundary of a circle, calculates the new position considering that boundaries are fully reflective.
+        
+        Parameters
+        ----------
+        circle_center : float
+            Center of the circle            
+        circle_radius : float
+            Radius of the circle
+        beg : tuple
+            Position (in 2D) of the begining of the segment
+        end : tuple
+            Position (in 2D) of the begining of the segment
+        precision_boundary : float
+            Small area around the real boundary which is also considered as boundary. For numerical stability
+            
+        Returns
+        -------
+        tuple
+            - Reflected position
+            - Intersection point
+        
+        '''
+        
+        # If the begining of the segment is in the exact boundary, no intersection is found.
+        # In that case, we bring closer the point to the center of the cercle so it is
+        # at a distance 'precision_boundary' from the border
+        if np.linalg.norm(circle_center - beg) > circle_radius - precision_boundary:
+            vec = trigo.seg_to_vec([circle_center, beg])
+            beg = np.array(circle_center)+(circle_radius-precision_boundary)*(-np.array(vec)/np.dot(vec, vec)**0.5)
+            
+        # find the intersection between the line drawn by the displacement and the circle
+        intersect = trigo.circle_line_segment_intersection(circle_center = circle_center,
+                                                           circle_radius = circle_radius, 
+                                                           pt1 = beg,
+                                                           pt2 = end)[-1]
+        # Draw lines and calculate angles between radius and begining-intersection
+        line1 = [circle_center, intersect]
+        line2 = [beg, intersect]
+        angle = trigo.ang_line(line1, line2)
+        # Calculate distance between intersection and end of displacement
+        dist_int_end = np.linalg.norm(np.array(intersect) - end)
+        # Create radius vector and calculate the tangent vector
+        vec_radius = trigo.seg_to_vec([circle_center, intersect])
+        tangent = trigo.rotate_vec(vec_radius, np.pi/2) 
+        # Calculate the angle between the tangent and the displacement vector
+        angle_tan = trigo.ang_vec(tangent, trigo.seg_to_vec([beg, intersect]))
+        # Change sign to correct get the reflection
+        if angle_tan < np.pi/2: angle = - angle
+        # Rotate the radius vector with the reflection angle and normalize by magnitude
+        vec_bounce = trigo.rotate_vec(vec_radius, angle)
+        vec_bounce /= np.dot(vec_bounce, vec_bounce)**0.5
+        # Final point is the previous vector times the distance starting at the intersect point  
+        return np.array(intersect)+dist_int_end*np.array(vec_bounce), intersect
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 84
+class models_phenom(models_phenom):
+    
+    @staticmethod
+    def _confinement_traj(T = 200,
+                          L = 100,
+                          Ds = [1, 0.1],
+                          alphas = [1, 1],
+                          r = 1,
+                          comp_center = None,
+                          Nc = 10,
+                          trans = 0.1,
+                          deltaT = 1):
+        '''
+        Generates a 2D trajectory of particles diffusing in an environment with partially transmitting circular compartments.
+        
+        Parameters
+        ----------
+        T : int
+            Length of the trajectory
+        L : float
+            Length of the box acting as the environment 
+        Ds : list
+            Diffusion coefficients of the two diffusive states (first free, the confined). Size must be 2.
+        alphas : list
+            Anomalous exponents of the two diffusive states (first free, the confined). Size must be 2.
+        r : float
+            Radius of the compartments.             
+        comp_center : array, None
+            If given, center of the compartments. If None, centers are uniformly sampled.
+        Nc : int
+            Number of compartments
+        trans : float
+            Transmittance of the boundaries
+        deltaT : int
+            Sampling time.            
+            
+        Returns
+        -------
+        tuple
+            - pos (array Tx2): particle's position
+            - labels (array Tx2): particle's labels (see ._multi_state for details on labels)
+            
+        '''
+
+        
+        # transform lists to numpy if needed
+        if isinstance(Ds, list):
+            Ds = np.array(Ds)
+        if isinstance(alphas, list):
+            alphas = np.array(alphas)
+
+        # Traps positions
+        if comp_center is None:
+            comp_center = models_phenom._distribute_circular_compartments(Nc = Nc,
+                                                                          r = r,
+                                                                          L = L)
+        # Particle's properties
+        pos = np.zeros((T, 2)) 
+        pos[0,:] = np.random.rand(2)*L
+
+        state = np.zeros(T).astype(int)        
+        # Check if particle is compartment
+        distance_centers = np.linalg.norm(comp_center - pos[0, :], axis = 1)
+        if distance_centers.min() < r:
+            # we assign the state to the compartment the particle is on
+            compartment = distance_centers.argmin()
+            state[0] = 1
+
+        # Output labels
+        labels = np.zeros((T, 3))
+        labels[0, 0] = alphas[state[0]] 
+        labels[0, 1] = Ds[state[0]]         
+        
+
+        # Trajectory
+        dispx = models_phenom().disp_fbm(alphas[state[0]], Ds[state[0]], T, deltaT = deltaT)
+        dispy = models_phenom().disp_fbm(alphas[state[0]], Ds[state[0]], T, deltaT = deltaT)
+        disp_t = 0
+
+
+        for t in range(1, T):
+            pos[t, :] = [pos[t-1, 0]+dispx[disp_t], pos[t-1, 1]+dispy[disp_t]]  
+
+            # if the particle was inside a compartment
+            if state[t-1] == 1:
+
+                # check if it exited of the compartment
+                current_distance = np.linalg.norm(comp_center[compartment, :] - pos[t, :])                              
+                if current_distance > r:                    
+                    coin = np.random.rand()                    
+                    # particle escaping
+                    if coin < trans:                        
+                        # check that if we entered in a different comparmetn
+                        distance_centers = np.linalg.norm(comp_center - pos[t, :], axis = 1)
+                        if distance_centers.min() < r:
+                            # we assign the state to the compartment the particle is on
+                            compartment = distance_centers.argmin()
+                            state[t] = 1
+                        else: state[t] = 0
+
+                    # particle reflecting
+                    else:   
+                        beg = pos[t-1, :]
+                        while current_distance > r:
+
+                            pos[t, :], intersect = models_phenom._reflected_position(circle_center = comp_center[compartment, :],
+                                                                                     circle_radius = r,
+                                                                                     beg = beg,
+                                                                                     end = pos[t, :])
+                            beg = intersect
+                            distance_beg = np.linalg.norm(comp_center[compartment, :] - beg)    
+                            current_distance = np.linalg.norm(comp_center[compartment, :] - pos[t,:])  
+                        state[t] = 1
+                # if the particle stayed inside the compartment
+                else: state[t] = 1
+
+
+            # If particle was outside of the compartment
+            elif state[t-1] == 0:                
+                # Check if particle entered a new compartment
+                distance_centers = np.linalg.norm(comp_center - pos[t, :], axis = 1)
+                if distance_centers.min() < r:
+                    # we assign the state to the compartment the particle is on
+                    compartment = distance_centers.argmin()
+                    state[t] = 1
+                # if the particle stayed outside the comparments
+                else: state[t] = 0
+
+            # If the state changed
+            if state[t] != state[t-1]:
+                
+                if T-t > 1:
+                    dispx = models_phenom().disp_fbm(alphas[state[t]], Ds[state[t]], T-t, deltaT = deltaT)
+                    dispy = models_phenom().disp_fbm(alphas[state[t]], Ds[state[t]], T-t, deltaT = deltaT)
+                    
+                else: 
+                    dispx, dispy = [np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn(), 
+                                    np.sqrt(2*Ds[state[t]]*deltaT)*np.random.randn()]
+                disp_t = 0
+            # If the state did not change:
+            else: disp_t += 1
+            
+            # Boundary conditions
+            if L is not None:
+                # Reflecting boundary conditions
+                while np.max(pos[t, :])>L or np.min(pos[t, :])< 0: 
+                    pos[t, pos[t, :] > L] = pos[t, pos[t, :] > L] - 2*(pos[t, pos[t, :] > L] - L)
+                    pos[t, pos[t, :] < 0] = - pos[t, pos[t, :] < 0]
+
+
+            labels[t, 0] = alphas[state[t]] 
+            labels[t, 1] = Ds[state[t]] 
+            
+        # Define state of particles based on the state array. First free/directed
+        if alphas[0] < models_phenom().alpha_directed:
+            labels[state == 0, -1] = models_phenom().lab_state.index('f') 
+        else:
+            labels[state == 0, -1] = models_phenom().lab_state.index('d') 
+        # Then confined
+        labels[state == 1, -1] = models_phenom().lab_state.index('c')         
+        
+        return pos, labels
+        
+
+
+# %% ../source_nbs/lib_nbs/models_phenom.ipynb 88
+class models_phenom(models_phenom):
+    def confinement(self,
+                    N = 10,
+                    T = 200,
+                    L = 100,
+                    Ds = [[1, 0], [0.1, 0]], 
+                    alphas = [[1, 0], [1, 0]],
+                    gamma_d = [1], 
+                    epsilon_a = [0],
+                    r = 1,
+                    comp_center = None,
+                    Nc = 10,
+                    trans = 0.1, 
+                    deltaT = 1):
+        '''
+        Generates a dataset of 2D trajectories of particles diffusing in an environment with partially transmitting circular compartments.
+        
+        Parameters
+        ----------
+        N : int
+            Number of trajectories
+        T : int
+            Length of the trajectory
+        L : float
+            Length of the box acting as the environment 
+        Ds : list
+            List of means and variances from which to sample the diffusion coefficient of each state. If element size is one, we consider variance = 0.
+        alphas : float
+            List of means and variances from which to sample the anomalous exponent of each state. If element size is one, we consider variance = 0.       
+        gamma_d : list
+            Minimum factor between D of diffusive states (see ._sampling_diff_parameters). Size is number of states -1 (in this case size 1)
+        epsilon_a : list
+            Distance between alpha of diffusive states (see ._sampling_diff_parameters). Size is number of states -1 (in this case size 1)
+        r : float
+            Radius of the compartments.             
+        comp_center : array, None
+            If given, center of the compartments. If None, centers are uniformly sampled.
+        Nc : int
+            Number of compartments
+        trans : float
+            Transmittance of the boundaries
+        deltaT : int
+            Sampling time.  
+            
+        Returns
+        -------
+        tuple
+            - pos (array Tx2): particle's position
+            - labels (array Tx2): particle's labels (see ._multi_state for details on labels)
+            
+        '''
+       
+        if isinstance(Ds, list):
+            Ds = np.array(Ds)
+        if isinstance(alphas, list):
+            alphas = np.array(alphas)
+
+        data = np.zeros((T, N, 2))
+        labels = np.zeros((T, N, 3))
+
+        for n in range(N):
+            
+            # Defined physical parameters for each trajectory
+            alphas_traj, Ds_traj = self._sample_diff_parameters(alphas = alphas,
+                                                                Ds = Ds,
+                                                                num_states = 2,
+                                                                epsilon_a = epsilon_a,
+                                                                gamma_d = gamma_d)
+
+            # Get trajectory from single traj function
+            pos, lab = self._confinement_traj(T = T,
+                                              Ds = Ds_traj,
+                                              alphas = alphas_traj,
+                                              L = L,
+                                              deltaT = deltaT,
+                                              r = r,
+                                              comp_center = comp_center,
+                                              Nc = Nc,
+                                              trans = trans)
+            data[:, n, :] = pos
+            labels[:, n, :] = lab
+
+        return data, labels
```

### Comparing `andi_datasets-2.0.3/andi_datasets/models_theory.py` & `andi_datasets-2.0.4/andi_datasets/models_theory.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/models_theory.ipynb.
-
-# %% auto 0
-__all__ = ['models_theory']
-
-# %% ../source_nbs/lib_nbs/models_theory.ipynb 3
-import numpy as np
-from stochastic.processes.continuous import FractionalBrownianMotion as fbm
-from math import pi as pi
-from scipy.special import erfcinv
-
-from .utils_trajectories import regularize, bm1D, sample_sphere
-
-# %% ../source_nbs/lib_nbs/models_theory.ipynb 5
-class models_theory(object):
-        
-    def __init__(self):
-        '''Constructor of the class''' 
-    
-    def attm(self, T, alpha, D = 1):
-        if D == 1: return self._oneD().attm(T, alpha)
-        elif D == 2: return self._twoD().attm(T, alpha)
-        elif D == 3: return self._threeD().attm(T, alpha)
-        else:
-            raise ValueError('Incorrect walk dimension')
-            
-    def sbm(self, T, alpha, D = 1):
-        if D == 1: return self._oneD().sbm(T, alpha)
-        elif D == 2: return self._twoD().sbm(T, alpha)
-        elif D == 3: return self._threeD().sbm(T, alpha)
-        else:
-            raise ValueError('Incorrect walk dimension')
-            
-    def ctrw(self, T, alpha, D = 1):
-        if D == 1: return self._oneD().ctrw(T, alpha)
-        elif D == 2: return self._twoD().ctrw(T, alpha)
-        elif D == 3: return self._threeD().ctrw(T, alpha)
-        else:
-            raise ValueError('Incorrect walk dimension')
-            
-    def fbm(self, T, alpha, D = 1):
-        if D == 1: return self._oneD().fbm(T, alpha)
-        elif D == 2: return self._twoD().fbm(T, alpha)
-        elif D == 3: return self._threeD().fbm(T, alpha)
-        else:
-            raise ValueError('Incorrect walk dimension')
-            
-    def lw(self, T, alpha, D = 1):
-        if D == 1: return self._oneD().lw(T, alpha)
-        elif D == 2: return self._twoD().lw(T, alpha)
-        elif D == 3: return self._threeD().lw(T, alpha)
-        else:
-            raise ValueError('Incorrect walk dimension')
-         
-
-# %% ../source_nbs/lib_nbs/models_theory.ipynb 7
-class models_theory(models_theory):  
-    
-    class _oneD():
-        '''Class cointaning one dimensional diffusion models'''                   
-            
-        def fbm(self, T, alpha):
-            ''' Creates a 1D fractional brownian motion trajectory'''            
-            H = alpha*0.5
-            return fbm(hurst=H).sample(int(T-1))
-        
-        def ctrw(self, T, alpha, regular_time = True):
-            ''' Creates a 1D continuous time tandom walk trajectory
-            Optional parameters:
-                :regular_time (bool):
-                    - True if to transform the trajectory to regular time. ''' 
-            if alpha > 1:
-                raise ValueError('Continuous random walks only allow for anomalous exponents <= 1.') 
-            # Generate the waiting times from power-law distribution
-            times = np.cumsum((1-np.random.rand(T))**(-1/alpha))      
-            times = times[:np.argmax(times>T)+1]
-            # Generate the positions of the walk
-            positions = np.cumsum(np.random.randn(len(times)))
-            positions -= positions[0]           
-            # Output
-            if regular_time:
-                return regularize(positions, times, T)
-            else:
-                return np.stack((times, positions))
-            
-        def lw(self, T, alpha):
-            ''' Creates a 1D Levy walk trajectory '''             
-            if alpha < 1:
-                raise ValueError('Levy walks only allow for anomalous exponents > 1.')
-            # Define exponents for the distribution of flight times                            
-            if alpha == 2:
-                sigma = np.random.rand()
-            else:
-                sigma = 3-alpha
-            dt = (1-np.random.rand(T))**(-1/sigma)
-            dt[dt > T] = T+1
-            # Define the velocity
-            v = 10*np.random.rand()                        
-            # Generate the trajectory
-            positions = np.empty(0)
-            for t in dt:
-                positions = np.append(positions, v*np.ones(int(t))*(2*np.random.randint(0,2)-1))
-                if len(positions) > T:
-                    break 
-            return np.cumsum(positions[:int(T)]) - positions[0]
-        
-        def attm(self, T, alpha, regime = 1):   
-            '''Creates a 1D trajectory following the annealed transient time model
-            Optional parameters:
-                :regime (int):
-                    - Defines the ATTM regime. Accepts three values: 0,1,2.'''
-            if regime not in [0,1,2]:
-                raise ValueError('ATTM has only three regimes: 0, 1 or 2.')
-            if alpha > 1:
-                raise ValueError('ATTM only allows for anomalous exponents <= 1.') 
-            # Gamma and sigma selection
-            if regime == 0:
-                sigma = 3*np.random.rand()
-                gamma = np.random.uniform(low = -5, high = sigma)
-                if alpha < 1:
-                    raise ValueError('ATTM regime 0 only allows for anomalous exponents = 1.') 
-            elif regime == 1:
-                sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
-                gamma = sigma/alpha
-                while sigma > gamma or gamma > sigma + 1:
-                    sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
-                    gamma = sigma/alpha
-            elif regime == 2:
-                gamma = 1/(1-alpha)
-                sigma = np.random.uniform(low = 1e-2, high = gamma-1)
-            # Generate the trajectory  
-            positions = np.array([0])
-            while len(positions) < T:
-                Ds =(1-np.random.uniform(low=0.1, high=0.99))**(1/sigma)  
-                ts = Ds**(-gamma)
-                if ts > T:
-                    ts = T
-                positions = np.append(positions, positions[-1]+bm1D(ts, Ds))
-            return positions[:T]-positions[0]
-        
-        
-        def sbm(self, T, alpha, sigma = 1):            
-            '''Creates a scaled brownian motion trajectory'''
-            msd = (sigma**2)*np.arange(T+1)**alpha
-            dx = np.sqrt(msd[1:]-msd[:-1])
-            dx = np.sqrt(2)*dx*erfcinv(2-2*np.random.rand(len(dx)))
-            return np.cumsum(dx)-dx[0]
-        
-    
-
-# %% ../source_nbs/lib_nbs/models_theory.ipynb 9
-class models_theory(models_theory):  
-
-    class _twoD():  
-            
-        def ctrw(self, T, alpha, regular_time = True):
-            ''' Creates a 2D continuous time tandom walk trajectory
-            Optional parameters:
-                :regular_time (bool):
-                    - True if to transform the trajectory to regular time. ''' 
-            if alpha > 1:
-                raise ValueError('Continuous random walks only allow for anomalous exponents <= 1.') 
-            # Generate the waiting times from power-law distribution            
-            times = np.cumsum((1-np.random.rand(T))**(-1/alpha))   
-            times = times[:np.argmax(times>T)+1]
-            # Generate the positions of the walk            
-            posX = np.cumsum(np.random.randn(len(times)))
-            posY = np.cumsum(np.random.randn(len(times)))            
-            posX -= posX[0] 
-            posY -= posY[0] 
-            # Regularize and output            
-            if regular_time:
-                regX = regularize(posX, times, T)
-                regY = regularize(posY, times, T)                
-                return np.concatenate((regX, regY))
-            else:
-                return np.stack((times, posX, posY))
-            
-        def fbm(self, T, alpha):
-            ''' Creates a 2D fractional brownian motion trajectory'''
-            # Defin Hurst exponent
-            H = alpha*0.5            
-            return np.concatenate((fbm(hurst=H).sample(int(T-1)), fbm(hurst=H).sample(int(T-1))))
-        
-            
-        def lw(self, T, alpha):
-            ''' Creates a 2D Levy walk trajectory '''             
-            if alpha < 1:
-                raise ValueError('Levy walks only allow for anomalous exponents > 1.')             
-            # Define exponents for the distribution of times              
-            if alpha == 2:
-                sigma = np.random.rand()
-            else:
-                sigma = 3-alpha
-            dt = (1-np.random.rand(T))**(-1/sigma)
-            dt[dt > T] = T+1
-            # Define the velocity
-            v = 10*np.random.rand()                        
-            # Define the array where we save step length
-            d= np.empty(0)
-            # Define the array where we save the angle of the step
-            angles = np.empty(0)
-            # Generate trajectory
-            for t in dt:
-                d = np.append(d, v*np.ones(int(t))*(2*np.random.randint(0,2)-1))                
-                angles = np.append(angles, np.random.uniform(low = 0, high = 2*pi)*np.ones(int(t)))
-                if len(d) > T:
-                    break
-            d = d[:int(T)]  
-            angles = angles[:int(T)] 
-            posX, posY = [d*np.cos(angles), d*np.sin(angles)]         
-            return np.concatenate((np.cumsum(posX)-posX[0], np.cumsum(posY)-posY[0]))
-        
-        
-        def attm(self, T, alpha, regime = 1):   
-            '''Creates a 2D trajectory following the annealed transient time model
-            Optional parameters:
-                :regime (int):
-                    - Defines the ATTM regime. Accepts three values: 0,1,2.'''
-            if regime not in [0,1,2]:
-                raise ValueError('ATTM has only three regimes: 0, 1 or 2.')
-            if alpha > 1:
-                raise ValueError('ATTM only allows for anomalous exponents <= 1.')                 
-            # Gamma and sigma selection
-            if regime == 0:
-                sigma = 3*np.random.rand()
-                gamma = np.random.uniform(low = -5, high = sigma)
-                if alpha < 1:
-                    raise ValueError('ATTM regime 0 only allows for anomalous exponents = 1.')  
-            elif regime == 1:
-                sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
-                gamma = sigma/alpha
-                while sigma > gamma or gamma > sigma + 1:
-                    sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
-                    gamma = sigma/alpha
-            elif regime == 2:
-                gamma = 1/(1-alpha)
-                sigma = np.random.uniform(low = 1e-2, high = gamma-1)
-            # Generate the trajectory  
-            posX = np.array([0])
-            posY = np.array([0])            
-            while len(posX) < T:
-                Ds =(1-np.random.uniform(low=0.1, high=0.99))**(1/sigma)  
-                ts = Ds**(-gamma)
-                if ts > T:
-                    ts = T                
-                posX = np.append(posX, posX[-1]+bm1D(ts, Ds))
-                posY = np.append(posY, posY[-1]+bm1D(ts, Ds))
-            return np.concatenate((posX[:T]-posX[0], posY[:T]-posY[0]))
-        
-        
-        def sbm(self, T, alpha, sigma = 1):            
-            '''Creates a scaled brownian motion trajectory'''
-            msd = (sigma**2)*np.arange(T+1)**alpha
-            deltas = np.sqrt(msd[1:]-msd[:-1])
-            dx = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas)))            
-            dy = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas)))  
-            return np.concatenate((np.cumsum(dx)-dx[0], np.cumsum(dy)-dy[0]))
-       
-
-# %% ../source_nbs/lib_nbs/models_theory.ipynb 11
-class models_theory(models_theory):  
-    
-    class _threeD():
-            
-        def ctrw(self, T, alpha, regular_time = True):
-            ''' Creates a 3D continuous time tandom walk trajectory
-            Optional parameters:
-                :regular_time (bool):
-                    - True if to transform the trajectory to regular time. ''' 
-            if alpha > 1:
-                raise ValueError('Continuous random walks only allow for anomalous exponents <= 1.') 
-            # Generate the waiting times from power-law distribution            
-            times = np.cumsum((1-np.random.rand(T))**(-1/alpha))
-            times = np.append(0, times)        
-            times = times[:np.argmax(times>T)+1]
-            # Generate the positions of the walk
-            lengths = np.random.randn(len(times))
-            posX, posY, posZ = np.cumsum(sample_sphere(len(times), lengths), axis=1)
-            posX = posX - posX[0]
-            posY = posY - posY[0]
-            posZ = posZ - posZ[0]    
-            # Regularize and output            
-            if regular_time:
-                regX = regularize(posX, times, T)
-                regY = regularize(posY, times, T) 
-                regZ = regularize(posZ, times, T)  
-                return np.concatenate((regX, regY, regZ))
-            else:
-                return np.stack((times, posX, posY, posZ))
-            
-        def fbm(self, T, alpha): 
-            ''' Creates a 3D fractional brownian motion trajectory'''
-            # Define Hurst exponent
-            H = alpha*0.5
-            return np.concatenate((fbm(hurst=H).sample(int(T-1)), fbm(hurst=H).sample(int(T-1)), fbm(hurst=H).sample(int(T-1))))
-        
-        
-        def lw(self, T, alpha, regular_time = True):
-            ''' Creates a 3D Levy walk trajectory '''             
-            if alpha < 1:
-                raise ValueError('Levy walks only allow for anomalous exponents > 1.')       
-            # Define exponents for the distribution of times
-            if alpha == 2:
-                sigma = np.random.rand()
-            else:
-                sigma = 3-alpha
-            dt = (1-np.random.rand(T))**(-1/sigma)
-            dt[dt>T] = T+1
-            # Define the velocity
-            v = 10*np.random.rand()                        
-            # Create the trajectory
-            posX = np.empty(0)
-            posY = np.empty(0)
-            posZ = np.empty(0)
-            for t in dt:
-                distX, distY, distZ = sample_sphere(1, v)
-                posX = np.append(posX, distX*np.ones(int(t)))
-                posY = np.append(posY, distY*np.ones(int(t)))
-                posZ = np.append(posZ, distZ*np.ones(int(t)))
-                if len(posX) > T:
-                    break
-            return np.concatenate((np.cumsum(posX[:T])-posX[0], 
-                                   np.cumsum(posY[:T])-posY[0],
-                                   np.cumsum(posZ[:T])-posZ[0]))
-        
-            
-        def attm(self, T, alpha, regime = 1):   
-            '''Creates a 3D trajectory following the annealed transient time model
-            Optional parameters:
-                :regime (int):
-                    - Defines the ATTM regime. Accepts three values: 0,1,2.'''
-            if regime not in [0,1,2]:
-                raise ValueError('ATTM has only three regimes: 0, 1 or 2.')
-            if alpha > 1:
-                raise ValueError('ATTM only allows for anomalous exponents <= 1.') 
-            # Parameter selection
-            if regime == 0:
-                sigma = 3*np.random.rand()
-                gamma = np.random.uniform(low = -5, high = sigma)
-                if alpha < 1:
-                    raise ValueError('ATTM Regime 0 can only produce trajectories with anomalous exponents = 1')
-            elif regime == 1:
-                sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
-                gamma = sigma/alpha
-                while sigma > gamma or gamma > sigma + 1:
-                    sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
-                    gamma = sigma/alpha
-            elif regime == 2:
-                gamma = 1/(1-alpha)
-                sigma = np.random.uniform(low = 1e-2, high = gamma-1)
-            # Create the trajectory  
-            posX = np.array([0])
-            posY = np.array([0])   
-            posZ = np.array([0])
-            while len(posX) < T:
-                Ds =(1-np.random.uniform(low=0.1, high=0.99))**(1/sigma)  
-                ts = Ds**(-gamma)
-                if ts > T:
-                    ts = T 
-                steps = np.sqrt(2*Ds)*np.random.randn(int(ts))
-                distX, distY, distZ = sample_sphere(len(steps), steps)
-                posX = np.append(posX, posX[-1]+distX)
-                posY = np.append(posY, posY[-1]+distY)
-                posZ = np.append(posZ, posZ[-1]+distZ)           
-            return np.concatenate((posX[:T]-posX[0], posY[:T]-posY[0], posZ[:T]-posZ[0]))
-        
-        
-        def sbm(self, T, alpha, sigma = 1):            
-            '''Creates a scaled brownian motion trajectory'''
-            msd = (sigma**2)*np.arange(T+1)**alpha
-            deltas = np.sqrt(msd[1:]-msd[:-1])
-            dx = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas)))            
-            dy = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas))) 
-            dz = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas))) 
-            return np.concatenate((np.cumsum(dx)-dx[0], np.cumsum(dy)-dy[0], np.cumsum(dz)-dz[0]))
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/models_theory.ipynb.
+
+# %% auto 0
+__all__ = ['models_theory']
+
+# %% ../source_nbs/lib_nbs/models_theory.ipynb 3
+import numpy as np
+from stochastic.processes.continuous import FractionalBrownianMotion as fbm
+from math import pi as pi
+from scipy.special import erfcinv
+
+from .utils_trajectories import regularize, bm1D, sample_sphere
+
+# %% ../source_nbs/lib_nbs/models_theory.ipynb 5
+class models_theory(object):
+        
+    def __init__(self):
+        '''Constructor of the class''' 
+    
+    def attm(self, T, alpha, D = 1):
+        if D == 1: return self._oneD().attm(T, alpha)
+        elif D == 2: return self._twoD().attm(T, alpha)
+        elif D == 3: return self._threeD().attm(T, alpha)
+        else:
+            raise ValueError('Incorrect walk dimension')
+            
+    def sbm(self, T, alpha, D = 1):
+        if D == 1: return self._oneD().sbm(T, alpha)
+        elif D == 2: return self._twoD().sbm(T, alpha)
+        elif D == 3: return self._threeD().sbm(T, alpha)
+        else:
+            raise ValueError('Incorrect walk dimension')
+            
+    def ctrw(self, T, alpha, D = 1):
+        if D == 1: return self._oneD().ctrw(T, alpha)
+        elif D == 2: return self._twoD().ctrw(T, alpha)
+        elif D == 3: return self._threeD().ctrw(T, alpha)
+        else:
+            raise ValueError('Incorrect walk dimension')
+            
+    def fbm(self, T, alpha, D = 1):
+        if D == 1: return self._oneD().fbm(T, alpha)
+        elif D == 2: return self._twoD().fbm(T, alpha)
+        elif D == 3: return self._threeD().fbm(T, alpha)
+        else:
+            raise ValueError('Incorrect walk dimension')
+            
+    def lw(self, T, alpha, D = 1):
+        if D == 1: return self._oneD().lw(T, alpha)
+        elif D == 2: return self._twoD().lw(T, alpha)
+        elif D == 3: return self._threeD().lw(T, alpha)
+        else:
+            raise ValueError('Incorrect walk dimension')
+         
+
+# %% ../source_nbs/lib_nbs/models_theory.ipynb 7
+class models_theory(models_theory):  
+    
+    class _oneD():
+        '''Class cointaning one dimensional diffusion models'''                   
+            
+        def fbm(self, T, alpha):
+            ''' Creates a 1D fractional brownian motion trajectory'''            
+            H = alpha*0.5
+            return fbm(hurst=H).sample(int(T-1))
+        
+        def ctrw(self, T, alpha, regular_time = True):
+            ''' Creates a 1D continuous time tandom walk trajectory
+            Optional parameters:
+                :regular_time (bool):
+                    - True if to transform the trajectory to regular time. ''' 
+            if alpha > 1:
+                raise ValueError('Continuous random walks only allow for anomalous exponents <= 1.') 
+            # Generate the waiting times from power-law distribution
+            times = np.cumsum((1-np.random.rand(T))**(-1/alpha))      
+            times = times[:np.argmax(times>T)+1]
+            # Generate the positions of the walk
+            positions = np.cumsum(np.random.randn(len(times)))
+            positions -= positions[0]           
+            # Output
+            if regular_time:
+                return regularize(positions, times, T)
+            else:
+                return np.stack((times, positions))
+            
+        def lw(self, T, alpha):
+            ''' Creates a 1D Levy walk trajectory '''             
+            if alpha < 1:
+                raise ValueError('Levy walks only allow for anomalous exponents > 1.')
+            # Define exponents for the distribution of flight times                            
+            if alpha == 2:
+                sigma = np.random.rand()
+            else:
+                sigma = 3-alpha
+            dt = (1-np.random.rand(T))**(-1/sigma)
+            dt[dt > T] = T+1
+            # Define the velocity
+            v = 10*np.random.rand()                        
+            # Generate the trajectory
+            positions = np.empty(0)
+            for t in dt:
+                positions = np.append(positions, v*np.ones(int(t))*(2*np.random.randint(0,2)-1))
+                if len(positions) > T:
+                    break 
+            return np.cumsum(positions[:int(T)]) - positions[0]
+        
+        def attm(self, T, alpha, regime = 1):   
+            '''Creates a 1D trajectory following the annealed transient time model
+            Optional parameters:
+                :regime (int):
+                    - Defines the ATTM regime. Accepts three values: 0,1,2.'''
+            if regime not in [0,1,2]:
+                raise ValueError('ATTM has only three regimes: 0, 1 or 2.')
+            if alpha > 1:
+                raise ValueError('ATTM only allows for anomalous exponents <= 1.') 
+            # Gamma and sigma selection
+            if regime == 0:
+                sigma = 3*np.random.rand()
+                gamma = np.random.uniform(low = -5, high = sigma)
+                if alpha < 1:
+                    raise ValueError('ATTM regime 0 only allows for anomalous exponents = 1.') 
+            elif regime == 1:
+                sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
+                gamma = sigma/alpha
+                while sigma > gamma or gamma > sigma + 1:
+                    sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
+                    gamma = sigma/alpha
+            elif regime == 2:
+                gamma = 1/(1-alpha)
+                sigma = np.random.uniform(low = 1e-2, high = gamma-1)
+            # Generate the trajectory  
+            positions = np.array([0])
+            while len(positions) < T:
+                Ds =(1-np.random.uniform(low=0.1, high=0.99))**(1/sigma)  
+                ts = Ds**(-gamma)
+                if ts > T:
+                    ts = T
+                positions = np.append(positions, positions[-1]+bm1D(ts, Ds))
+            return positions[:T]-positions[0]
+        
+        
+        def sbm(self, T, alpha, sigma = 1):            
+            '''Creates a scaled brownian motion trajectory'''
+            msd = (sigma**2)*np.arange(T+1)**alpha
+            dx = np.sqrt(msd[1:]-msd[:-1])
+            dx = np.sqrt(2)*dx*erfcinv(2-2*np.random.rand(len(dx)))
+            return np.cumsum(dx)-dx[0]
+        
+    
+
+# %% ../source_nbs/lib_nbs/models_theory.ipynb 9
+class models_theory(models_theory):  
+
+    class _twoD():  
+            
+        def ctrw(self, T, alpha, regular_time = True):
+            ''' Creates a 2D continuous time tandom walk trajectory
+            Optional parameters:
+                :regular_time (bool):
+                    - True if to transform the trajectory to regular time. ''' 
+            if alpha > 1:
+                raise ValueError('Continuous random walks only allow for anomalous exponents <= 1.') 
+            # Generate the waiting times from power-law distribution            
+            times = np.cumsum((1-np.random.rand(T))**(-1/alpha))   
+            times = times[:np.argmax(times>T)+1]
+            # Generate the positions of the walk            
+            posX = np.cumsum(np.random.randn(len(times)))
+            posY = np.cumsum(np.random.randn(len(times)))            
+            posX -= posX[0] 
+            posY -= posY[0] 
+            # Regularize and output            
+            if regular_time:
+                regX = regularize(posX, times, T)
+                regY = regularize(posY, times, T)                
+                return np.concatenate((regX, regY))
+            else:
+                return np.stack((times, posX, posY))
+            
+        def fbm(self, T, alpha):
+            ''' Creates a 2D fractional brownian motion trajectory'''
+            # Defin Hurst exponent
+            H = alpha*0.5            
+            return np.concatenate((fbm(hurst=H).sample(int(T-1)), fbm(hurst=H).sample(int(T-1))))
+        
+            
+        def lw(self, T, alpha):
+            ''' Creates a 2D Levy walk trajectory '''             
+            if alpha < 1:
+                raise ValueError('Levy walks only allow for anomalous exponents > 1.')             
+            # Define exponents for the distribution of times              
+            if alpha == 2:
+                sigma = np.random.rand()
+            else:
+                sigma = 3-alpha
+            dt = (1-np.random.rand(T))**(-1/sigma)
+            dt[dt > T] = T+1
+            # Define the velocity
+            v = 10*np.random.rand()                        
+            # Define the array where we save step length
+            d= np.empty(0)
+            # Define the array where we save the angle of the step
+            angles = np.empty(0)
+            # Generate trajectory
+            for t in dt:
+                d = np.append(d, v*np.ones(int(t))*(2*np.random.randint(0,2)-1))                
+                angles = np.append(angles, np.random.uniform(low = 0, high = 2*pi)*np.ones(int(t)))
+                if len(d) > T:
+                    break
+            d = d[:int(T)]  
+            angles = angles[:int(T)] 
+            posX, posY = [d*np.cos(angles), d*np.sin(angles)]         
+            return np.concatenate((np.cumsum(posX)-posX[0], np.cumsum(posY)-posY[0]))
+        
+        
+        def attm(self, T, alpha, regime = 1):   
+            '''Creates a 2D trajectory following the annealed transient time model
+            Optional parameters:
+                :regime (int):
+                    - Defines the ATTM regime. Accepts three values: 0,1,2.'''
+            if regime not in [0,1,2]:
+                raise ValueError('ATTM has only three regimes: 0, 1 or 2.')
+            if alpha > 1:
+                raise ValueError('ATTM only allows for anomalous exponents <= 1.')                 
+            # Gamma and sigma selection
+            if regime == 0:
+                sigma = 3*np.random.rand()
+                gamma = np.random.uniform(low = -5, high = sigma)
+                if alpha < 1:
+                    raise ValueError('ATTM regime 0 only allows for anomalous exponents = 1.')  
+            elif regime == 1:
+                sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
+                gamma = sigma/alpha
+                while sigma > gamma or gamma > sigma + 1:
+                    sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
+                    gamma = sigma/alpha
+            elif regime == 2:
+                gamma = 1/(1-alpha)
+                sigma = np.random.uniform(low = 1e-2, high = gamma-1)
+            # Generate the trajectory  
+            posX = np.array([0])
+            posY = np.array([0])            
+            while len(posX) < T:
+                Ds =(1-np.random.uniform(low=0.1, high=0.99))**(1/sigma)  
+                ts = Ds**(-gamma)
+                if ts > T:
+                    ts = T                
+                posX = np.append(posX, posX[-1]+bm1D(ts, Ds))
+                posY = np.append(posY, posY[-1]+bm1D(ts, Ds))
+            return np.concatenate((posX[:T]-posX[0], posY[:T]-posY[0]))
+        
+        
+        def sbm(self, T, alpha, sigma = 1):            
+            '''Creates a scaled brownian motion trajectory'''
+            msd = (sigma**2)*np.arange(T+1)**alpha
+            deltas = np.sqrt(msd[1:]-msd[:-1])
+            dx = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas)))            
+            dy = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas)))  
+            return np.concatenate((np.cumsum(dx)-dx[0], np.cumsum(dy)-dy[0]))
+       
+
+# %% ../source_nbs/lib_nbs/models_theory.ipynb 11
+class models_theory(models_theory):  
+    
+    class _threeD():
+            
+        def ctrw(self, T, alpha, regular_time = True):
+            ''' Creates a 3D continuous time tandom walk trajectory
+            Optional parameters:
+                :regular_time (bool):
+                    - True if to transform the trajectory to regular time. ''' 
+            if alpha > 1:
+                raise ValueError('Continuous random walks only allow for anomalous exponents <= 1.') 
+            # Generate the waiting times from power-law distribution            
+            times = np.cumsum((1-np.random.rand(T))**(-1/alpha))
+            times = np.append(0, times)        
+            times = times[:np.argmax(times>T)+1]
+            # Generate the positions of the walk
+            lengths = np.random.randn(len(times))
+            posX, posY, posZ = np.cumsum(sample_sphere(len(times), lengths), axis=1)
+            posX = posX - posX[0]
+            posY = posY - posY[0]
+            posZ = posZ - posZ[0]    
+            # Regularize and output            
+            if regular_time:
+                regX = regularize(posX, times, T)
+                regY = regularize(posY, times, T) 
+                regZ = regularize(posZ, times, T)  
+                return np.concatenate((regX, regY, regZ))
+            else:
+                return np.stack((times, posX, posY, posZ))
+            
+        def fbm(self, T, alpha): 
+            ''' Creates a 3D fractional brownian motion trajectory'''
+            # Define Hurst exponent
+            H = alpha*0.5
+            return np.concatenate((fbm(hurst=H).sample(int(T-1)), fbm(hurst=H).sample(int(T-1)), fbm(hurst=H).sample(int(T-1))))
+        
+        
+        def lw(self, T, alpha, regular_time = True):
+            ''' Creates a 3D Levy walk trajectory '''             
+            if alpha < 1:
+                raise ValueError('Levy walks only allow for anomalous exponents > 1.')       
+            # Define exponents for the distribution of times
+            if alpha == 2:
+                sigma = np.random.rand()
+            else:
+                sigma = 3-alpha
+            dt = (1-np.random.rand(T))**(-1/sigma)
+            dt[dt>T] = T+1
+            # Define the velocity
+            v = 10*np.random.rand()                        
+            # Create the trajectory
+            posX = np.empty(0)
+            posY = np.empty(0)
+            posZ = np.empty(0)
+            for t in dt:
+                distX, distY, distZ = sample_sphere(1, v)
+                posX = np.append(posX, distX*np.ones(int(t)))
+                posY = np.append(posY, distY*np.ones(int(t)))
+                posZ = np.append(posZ, distZ*np.ones(int(t)))
+                if len(posX) > T:
+                    break
+            return np.concatenate((np.cumsum(posX[:T])-posX[0], 
+                                   np.cumsum(posY[:T])-posY[0],
+                                   np.cumsum(posZ[:T])-posZ[0]))
+        
+            
+        def attm(self, T, alpha, regime = 1):   
+            '''Creates a 3D trajectory following the annealed transient time model
+            Optional parameters:
+                :regime (int):
+                    - Defines the ATTM regime. Accepts three values: 0,1,2.'''
+            if regime not in [0,1,2]:
+                raise ValueError('ATTM has only three regimes: 0, 1 or 2.')
+            if alpha > 1:
+                raise ValueError('ATTM only allows for anomalous exponents <= 1.') 
+            # Parameter selection
+            if regime == 0:
+                sigma = 3*np.random.rand()
+                gamma = np.random.uniform(low = -5, high = sigma)
+                if alpha < 1:
+                    raise ValueError('ATTM Regime 0 can only produce trajectories with anomalous exponents = 1')
+            elif regime == 1:
+                sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
+                gamma = sigma/alpha
+                while sigma > gamma or gamma > sigma + 1:
+                    sigma = 3*np.random.uniform(low = 1e-2, high = 1.1)
+                    gamma = sigma/alpha
+            elif regime == 2:
+                gamma = 1/(1-alpha)
+                sigma = np.random.uniform(low = 1e-2, high = gamma-1)
+            # Create the trajectory  
+            posX = np.array([0])
+            posY = np.array([0])   
+            posZ = np.array([0])
+            while len(posX) < T:
+                Ds =(1-np.random.uniform(low=0.1, high=0.99))**(1/sigma)  
+                ts = Ds**(-gamma)
+                if ts > T:
+                    ts = T 
+                steps = np.sqrt(2*Ds)*np.random.randn(int(ts))
+                distX, distY, distZ = sample_sphere(len(steps), steps)
+                posX = np.append(posX, posX[-1]+distX)
+                posY = np.append(posY, posY[-1]+distY)
+                posZ = np.append(posZ, posZ[-1]+distZ)           
+            return np.concatenate((posX[:T]-posX[0], posY[:T]-posY[0], posZ[:T]-posZ[0]))
+        
+        
+        def sbm(self, T, alpha, sigma = 1):            
+            '''Creates a scaled brownian motion trajectory'''
+            msd = (sigma**2)*np.arange(T+1)**alpha
+            deltas = np.sqrt(msd[1:]-msd[:-1])
+            dx = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas)))            
+            dy = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas))) 
+            dz = np.sqrt(2)*deltas*erfcinv(2-2*np.random.rand(len(deltas))) 
+            return np.concatenate((np.cumsum(dx)-dx[0], np.cumsum(dy)-dy[0], np.cumsum(dz)-dz[0]))
```

### Comparing `andi_datasets-2.0.3/andi_datasets/utils_challenge.py` & `andi_datasets-2.0.4/andi_datasets/utils_challenge.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,1520 +1,1520 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/utils_challenge.ipynb.
-
-# %% auto 0
-__all__ = ['majority_filter', 'label_filter', 'label_continuous_to_list', 'label_list_to_continuous', 'array_to_df',
-           'df_to_array', 'get_VIP', 'changepoint_assignment', 'changepoint_alpha_beta', 'jaccard_index',
-           'single_changepoint_error', 'ensemble_changepoint_error', 'create_binary_segment',
-           'jaccard_between_segments', 'segment_assignment', 'metric_anomalous_exponent',
-           'metric_diffusion_coefficient', 'metric_diffusive_state', 'check_no_changepoints', 'segment_property_errors',
-           'extract_ensemble', 'multimode_dist', 'distribution_distance', 'error_Ensemble_dataset',
-           'check_prediction_length', 'separate_prediction_values', 'load_file_to_df', 'error_SingleTraj_dataset',
-           'listdir_nohidden', 'codalab_scoring']
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 2
-import numpy as np
-from scipy.optimize import linear_sum_assignment
-import pandas
-from tqdm.auto import tqdm
-import warnings
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 6
-def majority_filter(seq, width):
-    '''
-    Given a vector, applies a majority filter of given width.
-    
-    Parameters
-    ----------
-    seq : list
-        Vector to filter.
-    width : int
-        Size of the window in which the filter is applied.
-    
-    Returns
-    -------
-    list
-        Filtered vector
-    '''
-    offset = width // 2
-    seq = [0] * offset + seq
-    return [max(set(a), key=a.count) 
-        for a in (seq[i:i+width] for i in range(len(seq) - offset))]
-
-def label_filter(label, 
-                 window_size = 5, 
-                 min_seg = 3):
-    '''
-    Given a vector of changing labels, applies a majority filter such that the minimum segment of a particular label is
-    bigger than the minimum set segment.
-    
-    Parameters
-    ----------
-    label : list
-        label vector to filter.
-    window_size : int
-        Size of the window in which the majority filter is applied.
-    min_seg : int
-        Minimum segment size after filtering.
-    
-    Returns
-    -------
-    np.array
-        Filtered label vector
-    '''
-    
-    if np.min(label) < 0:
-        raise ValueError('This function only works with positive labels')
-        
-    # if there are no changes:
-    if np.sum(label[1:] != label[:-1]) == 0:
-        return label
-    
-    # define dummy vector with all zeros and ones
-    values, dummy = np.unique(label, return_inverse = True)
-    
-    # check if there are segment smaller than minimal segment (min_seg)
-    cp = np.argwhere(dummy[1:] != dummy[:-1])
-    cp = np.append(0, cp)
-    current_min = (cp[1:]-cp[:-1]).flatten().min()
-
-    while (current_min < min_seg):
-
-        filt = majority_filter(dummy.tolist(), width = window_size)
-        filt = np.array(filt)
-        
-        # check if there are segment smaller than minimal segment (min_seg)
-        cp = np.argwhere(filt[1:] != filt[:-1])
-        
-        # If all changepoints were eliminated
-        if cp.size == 0:
-            break
-            
-        cp = np.append(0, cp)
-        current_min = (cp[1:]-cp[:-1]).flatten().min()
-        
-        if (dummy == filt).all():  
-            # If all failed and still have segments smaller than min_seg
-            seg_lengths = (cp[1:]-cp[:-1]).flatten().astype(int)
-            seg_smaller = np.argwhere(seg_lengths < min_seg).flatten()
-            
-            # We go over each segment and we asign the values 'by hand'
-            for idxsegs in seg_smaller:     
-                if seg_lengths[idxsegs] == 1:
-                    filt[(cp[idxsegs]+1)] = filt[cp[idxsegs]]     
-                elif seg_lengths[idxsegs] == 2:      
-                    filt[(cp[idxsegs]+1)] = filt[cp[idxsegs]]     
-                    filt[(cp[idxsegs]+2)] = filt[cp[idxsegs]+3]                     
-            
-            dummy = filt
-            break         
-        dummy = filt
-        
-        
-    # Check boundaries
-    if dummy[0] != dummy[1] or dummy[1] != dummy[2]:
-        dummy[:2] = dummy[2]
-    if dummy[-2] != dummy[-3] or dummy[-1] != dummy[-2]:
-        dummy[-3:] = dummy[-3]
-        
-    # reset to label values
-    dummy_ret = np.zeros_like(dummy).astype(float)
-    
-    for idx, v in enumerate(values):
-        dummy_ret[dummy == idx] = v
-
-    return dummy_ret
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 16
-def label_continuous_to_list(labs):
-    ''' 
-    Given an array of T x 2 labels containing the anomalous exponent and diffusion 
-    coefficient at each timestep, returns 3 arrays, each containing the changepoints, 
-    exponents and coefficient, respectively. 
-    If labs is size T x 3, then we consider that diffusive states are given and also
-    return those.
-    
-    Parameters
-    ----------
-    labs : array
-        T x 2  or T x 3 labels containing the anomalous exponent, diffusion 
-        and diffusive state.
-        
-    Returns
-    -------
-    tuple
-        - First element is the list of change points
-        - The rest are corresponding segment properties (order: alpha, Ds and states)        
-        '''
-    
-    # Check if states were given
-    are_states = False
-    if labs.shape[1] == 3:
-        are_states = True
-        
-    # Check in which variable there is changes
-    CP = np.argwhere((labs[:-1, :] != labs[1:, :]).sum(1) != 0).flatten()+1 
-    T = labs.shape[0] 
-
-    alphas = np.zeros(len(CP)+1)
-    Ds = np.zeros(len(CP)+1)
-    if are_states: states = np.zeros(len(CP)+1)
-        
-    for idx, cp in enumerate(np.append(CP, T)):
-        alphas[idx] = labs[cp-1, 0]
-        Ds[idx] = labs[cp-1, 1]
-        if are_states: states[idx] = labs[cp-1, 2]
-    
-    CP = np.append(CP, T)
-    
-    if are_states:
-        return CP, alphas, Ds, states
-    else:
-        return CP, alphas, Ds    
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 20
-def label_list_to_continuous(CP, label):
-    '''
-    Given a list of change points and the labels of the diffusion properties of the
-    resulting segments, generates and array of continuous labels. The last change point
-    indicates the array length.
-    
-    Parameters
-    ----------
-    CP : array, list
-        list of change points. Last change point indicates label length.
-    label : array, list
-        list of segment properties
-        
-    Returns
-    -------
-    array
-        Continuous label created from the given change points and segment properties
-    '''    
-    
-    if isinstance(label, list):
-        label = np.array(label)
-    segs = create_binary_segment(CP[:-1], CP[-1])
-    return (segs.transpose()*label).sum(1)
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 24
-from .utils_trajectories import segs_inside_fov
-
-
-def array_to_df(trajs, 
-               labels,
-               min_length = 10,
-               fov_origin = [0,0], fov_length= 100.0, cutoff_length = 10):
-    '''
-    Given arrays for the position and labels of trajectories, creates a dataframe with that
-    data. The function also applies the demanded FOV. If you don't want a field of view, chose a 
-    FOV length bigger (smaller) that your maximum (minimum) trajectory position.
-   
-    Parameters
-    ----------
-    trajs : array 
-        Trajectories to store in the df (dimension: T x N x 3)
-    labels : array
-        Labels to store in the df (dimension: T x N x 3)        
-    fov_origin : tuple
-        Bottom left point of the square defining the FOV.
-    fov_length : float
-        Size of the box defining the FOV.
-    cutoff_length : int
-        Minimum length of a trajectory inside the FOV to be considered in the output dataset.
-    
-    
-    Returns
-    -------
-    tuple
-        - df_in (dataframe): dataframe with trajectories
-        - df_out (datafram): dataframe with labels 
-    '''
-    
-    xs = []
-    ys = []
-    idxs = []   
-    
-    df_out = pandas.DataFrame(columns = ['traj_idx', 'Ds', 'alphas', 'states', 'changepoints']) 
-    
-    idx_t = 0
-    for traj, l_alpha, l_D, l_s in zip(tqdm(trajs), labels[:, :, 0], labels[:, :, 1], labels[:, :, 2]):
-
-        # Check FOV and 
-        idx_inside_segments = segs_inside_fov(traj, fov_origin, fov_length, cutoff_length)
-
-        if idx_inside_segments is not None:
-
-            for idx_in in idx_inside_segments:            
-                seg_x = traj[idx_in[0]:idx_in[1], 0]
-                seg_y = traj[idx_in[0]:idx_in[1], 1]
-                seg_alpha = l_alpha[idx_in[0]:idx_in[1]]
-                seg_D = l_D[idx_in[0]:idx_in[1]]
-                seg_state = l_s[idx_in[0]:idx_in[1]]
-
-                # Filtering
-                seg_alpha = label_filter(seg_alpha)
-                seg_D = label_filter(seg_D)
-                seg_state = label_filter(seg_state)
-                
-                
-                # Stacking data of input dataframe
-                xs += seg_x.tolist()
-                ys += seg_y.tolist()
-                idxs += (np.ones(len(seg_x))*idx_t).tolist()
-                
-                # Transforming to list of changepoints and physical properties
-                merge = np.hstack((seg_alpha.reshape(seg_alpha.shape[0], 1),
-                                   seg_D.reshape(seg_D.shape[0], 1),
-                                   seg_state.reshape(seg_state.shape[0], 1)))
-                
-                CP, alphas, Ds, states = label_continuous_to_list(merge)
-                
-                # Saving each segment info in output dataframe
-                df_out.loc[df_out.shape[0]] = [idx_t, Ds, alphas, states, CP]
-                
-                # Updating segment index
-                idx_t += 1
-
-    
-    # Saving trajectories in Dataframe
-    tr_to_df = np.vstack((idxs,
-                          xs,
-                          ys)).transpose()
-    df_in = pandas.DataFrame(tr_to_df, columns = ['traj_idx', 'x', 'y'])  
-    
-    return df_in, df_out
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 29
-def df_to_array(df, pad = -1):
-    '''
-    Transform a dataframe as the ones given in the ANDI 2 challenge (i.e. 4 columns:
-    traj_idx, frame, x, y) into a numpy array. To deal with irregular temporal supports,
-    we pad the array whenever the trajectory is not present.
-    The output array has the typical shape of ANDI datasets: TxNx2
-    
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe with four columns 'traj_idx': the trajectory index, 'frame' the time frame and 
-        'x' and 'y' the positions of the particle.
-    pad : int
-        Number to use as padding.
-    
-    Returns
-    -------
-    array
-        Array containing the trajectories from the dataframe, with usual ANDI shape (TxNx2).
-    
-    
-    '''
-
-    max_T = int(df.frame.max()+1)
-    num_part = int(df.iloc[-1].traj_idx)
-    array_trajs = np.ones((max_T, num_part+1, 2))*pad
-
-    for idx in np.unique(df.traj_idx).astype(int):
-
-        df_part = df.loc[df.traj_idx == idx]
-
-        array_trajs[df_part.frame.values.astype(int), idx, 0] = df_part.x.values
-        array_trajs[df_part.frame.values.astype(int), idx, 1] = df_part.y.values
-        
-    return array_trajs
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 31
-from scipy.spatial import distance
-
-
-def get_VIP(array_trajs, num_vip = 5, min_distance = 2, pad = -1):
-    '''
-    Given an array of trajectories, finds the particles VIP particles that participants will
-    need to characterize in the video trakcl.
-    
-    The function first finds the particles that exist at frame 0 (i.e. that their first value 
-    is different from pad). Then, iterates over this particles to find num_vip that are at 
-    distance > than min_distance in the first frame.
-    
-    Parameters
-    ----------
-    array_trajs : array
-        Position of the trajectories that will be considered for the VIP search.
-    num_vip : int
-        Number of VIP particles to flag.
-    min_distance : float
-        Minimum distance between two VIP particles.
-    pad : int
-        Number used to indicate in the temporal support that the particle is outside of the FOV.
-        
-    Returns
-    -------
-    list
-        List of indices of the chosen VIP particles
-    
-    '''
-    
-    candidates_vip = np.argwhere(array_trajs[0,:,0] != pad).flatten()
-    if len(candidates_vip) < num_vip:
-        raise ValueError('Number of VIP demanded is bigger than available particles.')
-
-    elected = []
-    count_while = 0
-    while len(elected) < num_vip:
-
-        elected = [np.random.choice(candidates_vip)]
-
-        for c_idx in candidates_vip:
-            if c_idx == elected[0]:
-                continue
-            if len(array_trajs[0, elected,:].shape) < 2:
-                all_rest = np.expand_dims(array_trajs[0, elected,:], 0)
-            else:
-                all_rest = array_trajs[0, elected,:]
-
-            dist = distance.cdist(np.expand_dims(array_trajs[0,c_idx,:], 0), all_rest, metric='euclidean').transpose()
-
-            if dist.min() > 2:
-                elected.append(c_idx)
-
-            if len(elected) == num_vip:
-                break
-
-
-        count_while += 1
-        if count_while > 100: 
-            raise ValueError('Could not find suitable VIP particles. This is due to either having to few particles or them being too close')
-            
-    return elected
-
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 34
-def changepoint_assignment(GT, preds):
-    ''' 
-    Given a list of groundtruth and predicted changepoints, solves the assignment problem via
-    the Munkres algorithm (aka Hungarian algorithm) and returns two arrays containing the index of the
-    paired groundtruth and predicted changepoints, respectively.
-    
-    The distance between change point is the Euclidean distance.
-    
-    Parameters
-    ----------
-    GT : list
-        List of groundtruth change points.
-    preds : list
-        List of predicted change points.
-    
-    Returns
-    -------
-    tuple
-        - tuple of two arrays, each corresponding to the assigned GT and pred changepoints
-        - Cost matrix
-    
-    '''
-    
-    cost_matrix = np.zeros((len(GT), len(preds)))
-
-    for idxg, gt in enumerate(GT):
-        for idxp, pred in enumerate(preds):
-            cost_matrix[idxg, idxp] = np.abs(gt-pred)
-            
-    return linear_sum_assignment(cost_matrix), cost_matrix
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 36
-def changepoint_alpha_beta(GT, preds, threshold = 10):
-    '''
-    Calculate the alpha and beta measure of paired changepoints.
-    Inspired from Supplemantary Note 3 in https://www.nature.com/articles/nmeth.2808
-    
-    Parameters
-    ----------
-    GT : list
-        List of groundtruth change points.
-    preds : list
-        List of predicted change points.
-    threshold : float
-        Distance from which predictions are considered to have failed. They are then assigned this number.
-    
-    Returns
-    -------
-    tuple
-        alpha, beta
-        
-    '''
-
-    assignment, _ = changepoint_assignment(GT, preds)
-    assignment = np.array(assignment)
-
-    threshold = 10
-    distance = np.abs(GT[assignment[0]] - preds[assignment[1]])
-    distance[distance > threshold] = threshold
-    distance = np.sum(distance)
-
-    d_x_phi = threshold*len(GT)
-    d_ybar_phi = max([0, (len(preds)-len(GT))*threshold])
-
-    alpha = 1-distance/d_x_phi
-    beta = (d_x_phi-distance)/(d_x_phi+d_ybar_phi)
-
-    return alpha, beta
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 38
-def jaccard_index(TP: int, # true positive
-                  FP: int, # false positive
-                  FN: int # false negative
-                 )-> float: # Jaccard Index
-    '''
-    Given the true positive, false positive and false negative rates, calculates the Jaccard Index
-    '''
-    return TP/(TP+FP+FN)
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 39
-def single_changepoint_error(GT, preds, threshold = 5):
-    '''
-    Given the groundtruth and predicted changepoints for a single trajectory, first solves the assignment problem between changepoints,
-    then calculates the RMSE of the true positive pairs and the Jaccard index.
-    
-    Parameters
-    ----------
-    GT : list
-        List of groundtruth change points.
-    preds : list
-        List of predicted change points.
-    threshold : float
-        Distance from which predictions are considered to have failed. They are then assigned this number.
-    
-    Returns
-    -------
-    tuple
-        - TP_rmse: root mean square error of the true positive change points.
-        - Jaccard Index of the ensemble predictions        
-        
-    '''
-    
-    assignment, _ = changepoint_assignment(GT, preds)
-    assignment = np.array(assignment)
-    
-    TP, FP, FN = 0, 0, 0
-    TP_rmse = []
-    for p in assignment.transpose():
-        
-        if np.abs(GT[p[0]] - preds[p[1]]) < threshold:
-            TP += 1
-            TP_rmse.append((GT[p[0]] - preds[p[1]])**2)
-        else:
-            FP += 1
-            FN += 1
-    # Calculating RMSE
-    TP_rmse = np.sqrt(np.mean(TP_rmse))
-
-    # Checking false positive and missed events
-    if len(preds) > len(GT):
-        FP += len(preds) - len(GT)
-    elif len(preds) < len(GT):
-        FN += len(GT) - len(preds)
-    
-    return TP_rmse, jaccard_index(TP, FP, FN)
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 40
-def ensemble_changepoint_error(GT_ensemble, pred_ensemble, threshold = 5):    
-    ''' 
-    Given an ensemble of groundtruth and predicted change points, iterates
-    over each trajectory's changepoints. For each, it solves the assignment problem 
-    between changepoints. Then, calculates the RMSE of the true positive pairs and
-    the Jaccard index over the ensemble of changepoints (i.e. not the mean of them 
-    w.r.t. to the trajectories)
-    
-    Parameters
-    ----------
-    GT_ensemble : list, array
-        Ensemble of groutruth change points.
-    pred_ensemble : list
-        Ensemble of predicted change points.
-    threshold : float
-        Distance from which predictions are considered to have failed. They are then assigned this number.
-    
-    Returns
-    -------
-    tuple
-        - TP_rmse: root mean square error of the true positive change points.
-        - Jaccard Index of the ensemble predictions
-    
-    '''
-    
-    TP, FP, FN = 0, 0, 0
-    TP_rmse = []
-    
-    for gt_traj, pred_traj in zip(GT_ensemble, pred_ensemble):
-        
-        assignment, _ = changepoint_assignment(gt_traj, pred_traj)
-        assignment = np.array(assignment)
-        
-        for p in assignment.transpose():
-            
-            if np.abs(gt_traj[p[0]] - pred_traj[p[1]]) < threshold:
-                TP += 1
-                TP_rmse.append((gt_traj[p[0]] - pred_traj[p[1]])**2)
-            else:
-                FP += 1
-                FN += 1    
-                
-        # Checking false positive and missed events
-        if len(pred_traj) > len(gt_traj):
-            FP += len(pred_traj) - len(gt_traj)
-        elif len(pred_traj) < len(gt_traj):
-            FN += len(gt_traj) - len(pred_traj)
-                
-    if TP+FP+FN == 0:
-        wrn_str = f'No segments found in this dataset.'
-        warnings.warn(wrn_str)
-        return threshold, 0
-        
-    # Calculating RMSE
-    TP_rmse = np.sqrt(np.mean(TP_rmse))
-
-    
-        
-    return TP_rmse, jaccard_index(TP, FP, FN)
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 43
-def create_binary_segment(CP: list, # list of changepoints
-                          T: int # length of the trajectory
-                         )-> list: # list of arrays with value 1 in the temporal support of the current segment.
-    '''
-    Given a set of changepoints and the lenght of the trajectory, create segments which are equal to one
-    if the segment takes place at that position and zero otherwise.
-    '''
-    segments = np.zeros((len(CP)+1, T))
-    CP = np.append(0, CP)
-    for idx, (cp1, cp2) in enumerate(zip(CP[:-1], CP[1:])):
-        segments[idx, cp1+1:cp2+1] = 1
-    segments[-1, CP[-1]+1:] = 1
-    segments[0, 0] = 1
-    return segments
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 45
-def jaccard_between_segments(gt, pred):
-    '''
-    Given two segments, calculates the Jaccard index between them by considering TP as correct labeling,
-    FN as missed events and FP leftover predictions.
-    
-    Parameters
-    ----------
-    gt : array
-        groundtruth segment, equal to one in the temporal support of the given segment, zero otherwise.
-    pred : array
-        predicted segment, equal to one in the temporal support of the given segment, zero otherwise.
-    
-    Returns
-    -------
-    float
-        Jaccard index between the given segments.
-    '''
-    
-    if len(gt) > len(pred):
-        pred = np.append(pred, np.zeros(len(gt) - len(pred)))
-    elif len(pred) > len(gt):                        
-        gt = np.append(gt, np.zeros(len(pred) - len(gt)))
-    
-    
-    tp = np.sum(np.logical_and(pred == 1, gt == 1))
-    fp = np.sum(np.logical_and(pred == 1, gt == 0))
-    fn = np.sum(np.logical_and(pred == 0, gt == 1))
-    
-    # special case for absence of changepoint
-    if tp+fp+fn == 0: return 0    
-    else: return jaccard_index(tp, fp, fn)
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 46
-def segment_assignment(GT, preds, T:int = None):
-    ''' 
-    Given a list of groundtruth and predicted changepoints, generates a set of segments. Then constructs 
-    a cost matrix by calculting the Jaccard Index between segments. From this cost matrix, we solve the 
-    assignment  problem via the Munkres algorithm (aka Hungarian algorithm) and returns two arrays 
-    containing the index of the groundtruth and predicted segments, respectively.
-    
-    If T = None, then we consider that GT and preds may have different lenghts. In that case, the end
-    of the segments is the the last CP of each set of CPs.
-    
-    Parameters
-    ----------
-    GT : list
-        List of groundtruth change points.
-    preds : list
-        List of predicted change points.
-    T : int, None
-        Length of the trajectory. If None, considers different GT and preds length.
-    
-    Returns
-    -------
-    tuple
-        - tuple of two arrays, each corresponding to the assigned GT and pred changepoints
-        - Cost matrix calculated via JI of segments   
-    
-    '''
-   
-    if T is not None:
-        T_gt = T_pred = T
-        # Check if the GT or predictions are a single integer or an empty array
-        if isinstance(GT, int): GT = [GT]
-        elif len(GT) == 0: GT = [T-1]
-
-        if isinstance(preds, int): preds = [preds]
-        elif len(preds) == 0: preds = [T-1]
-    else:
-        T_gt = GT[-1]
-        if len(GT) > 1:
-            GT = GT[:-1]            
-            
-        T_pred = preds[-1]
-        if len(preds) > 1:
-            preds = preds[:-1]
-        
-    
-    
-    seg_GT = create_binary_segment(GT, T_gt)
-    seg_preds = create_binary_segment(preds, T_pred)
-    
-    cost_matrix = np.zeros((seg_GT.shape[0], seg_preds.shape[0]))
-
-    for idxg, gt in enumerate(seg_GT):
-        for idxp, pred in enumerate(seg_preds):
-            cost_matrix[idxg, idxp] = 1-jaccard_between_segments(gt, pred)
-
-    return linear_sum_assignment(cost_matrix), cost_matrix
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 56
-from sklearn.metrics import mean_squared_log_error as msle, f1_score
-from .models_phenom import models_phenom
-
-def metric_anomalous_exponent(gt = None,
-                              pred = None,
-                              max_error = np.abs(models_phenom().bound_alpha[0]-models_phenom().bound_alpha[1])):
-    ''' 
-    Compute the mean absolute error (mae) between anomalous exponents.
-    Checks the current bounds of anomalous exponents from models_phenom to calculate the maximum error.
-    ''' 
-    error = np.mean(np.abs(gt-pred))
-    if error > max_error:
-        return max_error
-    else: 
-        return error
-
-def metric_diffusion_coefficient(gt = None, pred = None, 
-                                 threshold_min = models_phenom().bound_D[0],                               
-                                 max_error = msle([models_phenom().bound_D[0]],
-                                                  [models_phenom().bound_D[1]])):
-    ''' 
-    Compute the mean squared log error (msle) between diffusion coefficients.
-    Checks the current bounds of diffusion from models_phenom to calculate the maximum error. 
-    ''' 
-    
-     # considering the presence of zeros and negatives
-    pred = np.array(pred).copy(); gt = np.array(gt).copy()
-    pred[pred <= threshold_min] = threshold_min
-    gt[gt <= threshold_min] = threshold_min    
-    # mean squared log error
-    error = msle(gt, pred)
-    
-    if error > max_error:
-        return max_error
-    else: 
-        return error
-
-def metric_diffusive_state(gt = None, pred = None, max_error = False):
-    ''' 
-    Compute the F1 score between diffusive states. 
-    ''' 
-    return f1_score(gt.astype(int), pred.astype(int), average = 'micro')
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 60
-def check_no_changepoints(GT_cp, GT_alpha, GT_D, GT_s,
-                          preds_cp, preds_alpha, preds_D, preds_s,
-                          T:bool|int = None):
-    '''
-    Given predicionts over changepoints and variables, checks if in both GT and preds there is an 
-    absence of change point. If so, takes that into account to pair variables.
-    
-    Parameters
-    ----------
-    GT_cp : list, int, float
-        Groundtruth change points
-    GT_alpha : list, float
-        Groundtruth anomalous exponent
-    GT_D : list, float
-        Groundtruth diffusion coefficient
-    GT_s : list, float
-        Groundtruth diffusive state
-    preds_cp : list, int, float
-        Predicted change points
-    preds_alpha : list, float
-        Predicted anomalous exponent
-    preds_D : list, float
-        Predicted diffusion coefficient
-    preds_s : list, float
-        Predicted diffusive state
-    T : bool,int
-        (optional) Length of the trajectories. If none, last change point is length.
-    
-    Returns
-    -------
-    tuple
-        - False if there are change points. True if there were missing change points.
-        - Next three are either all Nones if change points were detected, or paired exponents, 
-        coefficient and states if some change points were missing.
-    
-    '''
-
-
-    if isinstance(GT_cp, int) or isinstance(GT_cp, float):
-        GT_cp = [GT_cp]
-    if isinstance(preds_cp, int) or isinstance(preds_cp, float):
-        preds_cp = [preds_cp]
-        
-    no_GT_cp = False; no_preds_cp = False
-    # CP always contain the final point of the trajectory, hence minimal length is one
-    if len(GT_cp) == 1: no_GT_cp = True
-    if len(preds_cp) == 1: no_preds_cp = True       
-        
-
-    if no_GT_cp + no_preds_cp == 0:
-        return False, None, None, None
-    
-    else:
-
-        [row_ind, col_ind], _ = segment_assignment(GT_cp, preds_cp, T)   
-
-        if no_GT_cp and not no_preds_cp:
-            paired_alpha = np.array([[GT_alpha[0], preds_alpha[col_ind[0]]]])
-            paired_D = np.array([[GT_D[0], preds_D[col_ind[0]]]])
-            paired_s = np.array([[GT_s[0], preds_s[col_ind[0]]]])
-
-        if no_preds_cp and not no_GT_cp:
-            row_position = np.argwhere(col_ind == 0).flatten()[0]            
-            paired_alpha = np.array([[GT_alpha[row_position], preds_alpha[col_ind[row_position]]]])
-            paired_D = np.array([[GT_D[row_position], preds_D[col_ind[row_position]]]])
-            paired_s = np.array([[GT_s[row_position], preds_s[col_ind[row_position]]]])
-            
-        if no_preds_cp and no_GT_cp: 
-            paired_alpha = np.array([[GT_alpha[0], preds_alpha[0]]])
-            paired_D = np.array([[GT_D[0], preds_D[0]]])
-            paired_s = np.array([[GT_s[0], preds_s[0]]])
-            
-
-        return True, paired_alpha, paired_D, paired_s
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 61
-def segment_property_errors(GT_cp, GT_alpha, GT_D, GT_s,
-                            preds_cp, preds_alpha, preds_D, preds_s,
-                            return_pairs = False,
-                            T = None):
-    '''
-    Given predicionts over change points and the value of diffusion parameters in the generated
-    segments, computes the defined metrics.
-    
-    Parameters
-    ----------
-    GT_cp : list, int, float
-        Groundtruth change points
-    GT_alpha : list, float
-        Groundtruth anomalous exponent
-    GT_D : list, float
-        Groundtruth diffusion coefficient
-    GT_s : list, float
-        Groundtruth diffusive state
-    preds_cp : list, int, float
-        Predicted change points
-    preds_alpha : list, float
-        Predicted anomalous exponent
-    preds_D : list, float
-        Predicted diffusion coefficient
-    preds_s : list, float
-        Predicted diffusive state
-    return_pairs : bool
-        If True, returns the assigment pairs for each diffusive property.
-    T : bool,int
-        (optional) Length of the trajectories. If none, last change point is length.
-    
-    Returns
-    -------
-    tuple
-        - if return_pairs = True, returns the assigned pairs of diffusive properties
-        - if return_pairs = False, returns the errors for each diffusive property
-    '''
-    
-    # Check cases in which changepoint where not detected or there were none in groundtruth
-    no_change_point_case, paired_alpha, paired_D, paired_s = check_no_changepoints(GT_cp, GT_alpha, GT_D, GT_s,
-                                                                                   preds_cp, preds_alpha, preds_D, preds_s, T)
-   
-    if not no_change_point_case:
-        # Solve the assignment problem
-        [row_ind, col_ind], _ = segment_assignment(GT_cp, preds_cp, T)
-   
-        # iterate over the groundtruth segments
-        paired_alpha, paired_D, paired_s = [], [], []
-        for idx_seg, (gt_alpha, gt_D) in enumerate(zip(GT_alpha, GT_D)):
-
-            row_position = np.argwhere(row_ind == idx_seg).flatten()
-
-            # if the GT segment was associated to a prediction
-            if len(row_position) > 0:
-                row_position = int(row_position)
-                # alpha                
-                gt_a_seg = GT_alpha[idx_seg]                
-                pred_a_seg = preds_alpha[col_ind[row_position]]
-                # d
-                gt_d_seg = GT_D[idx_seg]
-                pred_d_seg = preds_D[col_ind[row_position]]
-                # state
-                gt_s_seg = GT_s[idx_seg]
-                pred_s_seg = preds_s[col_ind[row_position]]
-
-                paired_alpha.append([gt_a_seg, pred_a_seg])
-                paired_D.append([gt_d_seg, pred_d_seg])
-                paired_s.append([gt_s_seg, pred_s_seg])
-
-        paired_alpha, paired_D, paired_s = np.array(paired_alpha), np.array(paired_D), np.array(paired_s) 
-    
-    if return_pairs:
-        return paired_alpha, paired_D, paired_s 
-    else:
-        error_alpha = metric_anomalous_exponent(paired_alpha[:,0], paired_alpha[:,1])
-        error_D = metric_diffusion_coefficient(paired_D[:,0], paired_D[:,1])
-        error_s = metric_diffusive_state(paired_s[:,0], paired_s[:,1])
-        return error_alpha, error_D, error_s
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 69
-from .models_phenom import models_phenom
-def extract_ensemble(state_label, dic):
-        ''' 
-        Given an array of the diffusive state and a dictionary with the diffusion information,
-        returns a summary of the ensemble properties for the current dataset.
-
-        Parameters
-        ----------
-        state_label : array
-            Array containing the diffusive state of the particles in the dataset.
-            For multi-state and dimerization, this must be the number associated to the
-            state (for dimerization, 0 is free, 1 is dimerized). For the rest, we follow
-            the numeration of models_phenom().lab_state.
-        dic : dict 
-            Dictionary containing the information of the input dataset.
-       
-       Returns
-       -------
-       array
-           Matrix containing the ensemble information of the input dataset. It has the following shape:
-            |mu_alpha1      mu_alpha2     ... |
-            |sigma_alpha1   sigma_alpha2  ... |
-            |mu_D1          mu_D1         ... | 
-            |sigma_D1       sigma_D2      ... |
-            |counts_state1  counts_state2 ... |
-        '''
-
-        # Single state
-        if dic['model'] == 'single_state': 
-            ensemble = np.vstack((dic['alphas'][0],
-                                   dic['alphas'][1],
-                                   dic['Ds'][0],
-                                   dic['Ds'][1],
-                                   len(state_label)
-                                   ))
-        # Multi-state
-        if dic['model'] == 'multi_state':
-            states, counts = np.unique(state_label, return_counts=True)    
-            # If the number of visited stated is not equal to the expected number of states
-            if len(states) != dic['alphas'].shape[0]:
-                states_corrected = np.ones(dic['alphas'].shape[0])
-                counts_corrected = np.ones(dic['alphas'].shape[0])
-                for s, c in zip(states, counts):
-                    counts_corrected[int(s)] = c
-            else: 
-                counts_corrected = counts
-
-            ensemble = np.vstack((dic['alphas'][:, 0],
-                                   dic['alphas'][:, 1],
-                                   dic['Ds'][:, 0],
-                                   dic['Ds'][:, 1],
-                                   counts_corrected
-                                   ))
-
-        # Immobile
-        if dic['model'] == 'immobile_traps':
-            counts = [len(state_label[state_label == models_phenom().lab_state.index('i')]),
-                      len(state_label[state_label == models_phenom().lab_state.index('f')])]  
-            ensemble = np.vstack(([0, dic['alphas'][0]],
-                                   [0, dic['alphas'][1]],
-                                   [0, dic['Ds'][0]],
-                                   [0, dic['Ds'][1]],
-                                   counts
-                                   ))
-        # dimerization    
-        if dic['model'] == 'dimerization':
-            counts = [len(state_label[state_label == 0]),
-                      len(state_label[state_label == 1])]           
-            ensemble = np.vstack((dic['alphas'][:, 0],
-                                   dic['alphas'][:, 1],
-                                   dic['Ds'][:, 0],
-                                   dic['Ds'][:, 1],
-                                   counts
-                                   ))
-
-        if dic['model'] == 'confinement':
-            counts = [len(state_label[state_label == models_phenom().lab_state.index('f')]),
-                      len(state_label[state_label == models_phenom().lab_state.index('c')])]   
-            ensemble = np.vstack((dic['alphas'][:, 0],
-                                   dic['alphas'][:, 1],
-                                   dic['Ds'][:, 0],
-                                   dic['Ds'][:, 1],
-                                   counts
-                                   ))
-        return ensemble
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 70
-import scipy.stats
-def multimode_dist(params, weights, bound, x, normalized = False):
-    '''
-    Generates a multimodal distribution with given parameters.
-    Also accounts for single mode if weight is float or int.
-    
-    Parameters
-    ----------
-    params : list
-        Mean and variances of every mode.
-    weights : list, float
-        Weight of every mode. If float, we consider a single mode.
-    bound : tuple
-        Bounds (min, max) of the functions support.
-    x : array
-        Support upon which the distribution is created.
-    normalize : bool
-        If True, returns the normalized distribution.
-    
-    Returns
-    -------
-    array
-        Value of the distribution in each point of the given support
-        
-    '''
-    func = scipy.stats.truncnorm
-    dist = np.zeros_like(x)
-    lower, upper = bound 
-   
-    # If we have single state, change values to list to still
-    # have a loop:
-    if isinstance(weights, float) or isinstance(weights, int):
-        params = [params]
-        weights = [weights]
-        
-    for param, w in zip(params, weights):
-        mean, var  = param  
-        # introduce a cutoff to avoid nan when var = 0
-        if var == 0: var = 1e-9
-        unimodal = func.pdf(x,
-                            (lower-mean)/np.sqrt(var),
-                            (upper-mean)/np.sqrt(var),
-                            loc = mean,
-                            scale = np.sqrt(var))
-        dist += w*unimodal
-    if normalized:
-        dist /= np.sum(dist)
-    return dist
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 71
-def distribution_distance(p:np.array, # distribution 1
-                          q:np.array # distribution 2
-                         )-> float:  # distance between distributions
-    ''' Calculates mean absolute error between two distributions. '''
-#     return np.sum(np.where(p != 0, p * np.log(p / q), 0))
-    return np.abs(p-q).mean()
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 74
-from .models_phenom import models_phenom
-
-def error_Ensemble_dataset(true_data, pred_data, return_distributions = False):
-    ''' 
-    Calculates the ensemble metrics for the ANDI 2 challenge. The input are matrices of shape:
-    
-    | col1 (state 1) | col2 (state 2) | col3 (state 3) | ... |
-    |:--------------:|:--------------:|:--------------:|:---:|
-    | $\mu_a^1$      | $\mu_a^2$      | $\mu_a^3$      | ... |
-    | $\sigma_a^1$   | $\sigma_a^2$   | $\sigma_a^3$   | ... |
-    | $\mu_D^1$      | $\mu_D^2$      | $\mu_D^3$      | ... |        
-    | $\sigma_D^1$   | $\sigma_D^2$   | $\sigma_D^3$   | ... |
-    | $N_1$          | $N_2$          | $N_3$          | ... |
-    
-    Parameters
-    ----------
-    true_data : array
-        Matrix containing the groundtruth data.
-    pred_data : array
-        Matrix containing the predicted data.
-    return_distributions : bool
-        If True, the function also outputs the generated distributions.
-    
-    Returns
-    -------
-    tuple
-        - distance_alpha: distance between anomalous exponents
-        - distance_D: distance between diffusion coefficients
-        - dists (if asked): distributions of both groundtruth and predicted data.        
-    
-    '''
-    
-    dists = []
-    for data in [true_data, pred_data]:
-        
-        if len(data.shape) > 1: # If we have more than one state
-            alpha_info = np.delete(data, [2,3, -1], 0)
-            d_info = data[2:-1,:]
-            weights = data[-1,:]
-            if weights.sum() > 1: weights /= weights.sum()
-        else: # If single state
-            alpha_info = data[:2]
-            d_info = data[2:-1]
-            weights = 1
-            
-        for idx, (var, bound) in enumerate(zip([alpha_info, d_info], 
-                                               [models_phenom().bound_alpha, models_phenom().bound_D])):
-            if idx == 0: x = np.linspace(bound[0], bound[1], 1000)
-            else: x = np.logspace(np.log10(bound[0]), np.log10(bound[1]), 1000)
-            dists.append(multimode_dist(var.T, weights, bound, x))
-            
-    # Distance between alpha dists
-    distance_alpha = distribution_distance(dists[0], dists[2])
-    distance_D = distribution_distance(dists[1], dists[3])
-    
-    if return_distributions:
-        return distance_alpha, distance_D, dists
-    else:
-        return distance_alpha, distance_D
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 76
-def check_prediction_length(pred):
-    '''
-    Given a trajectory segments prediction, checks whether it has C changepoints and C+1 segments properties values.
-    As it must also contain the index of the trajectory, this is summarized by being multiple of 4. 
-    In some cases, the user needs to also predict the final point of the trajectory. In this case, 
-    we will have a residu of 1.
-    '''
-    if len(pred) % 4 == 0 or len(pred) % 4 == 1 :
-        return True
-    else: 
-        return False
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 77
-def separate_prediction_values(pred):
-    '''
-    Given a prediction over trjaectory segments, extracts the predictions for each segment property
-    as well as the changepoint values.
-    '''        
-    Ds = pred[1::4]
-    alphas = pred[2::4]
-    states = pred[3::4]
-    cp = pred[4::4]    
-    return Ds, alphas, states, cp
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 78
-def load_file_to_df(path_file, 
-                    columns = ['traj_idx', 'Ds', 'alphas', 'states', 'changepoints']):
-    '''
-    Given the path of a .txt file, extract the segmentation predictions based on 
-    the rules of the ANDI 2 challenge022
-    '''
-
-    with open(path_file) as f:
-        lines_pred = f.read().splitlines()
-
-    df = pandas.DataFrame(columns = columns)
-
-    for line in lines_pred:
-        # Extract values with comma separator and transform to float
-        pred_traj = line.split(',')
-        pred = [float(i) for i in pred_traj]
-        
-        # Check that prediction has the correct shape
-        pred_correct = check_prediction_length(pred)
-        
-        # If correct size, then extract parameters and add it to dataframe
-        if pred_correct:
-            preds_D, preds_a, preds_s, preds_cp = separate_prediction_values(pred)
-
-            current_row = df.shape[0]
-            for param, pred_param in zip(columns, [pred[0], preds_D, preds_a, preds_s, preds_cp]):
-                df.loc[current_row, param] = pred_param
-                
-    return df
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 83
-def _get_error_bounds():
-    '''
-    Sets the current maximum errors we can do in the different diffusive properties.
-    '''
-    
-    threshold_error_alpha = 2
-    threshold_error_D = 1e5
-    threshold_error_s = -1
-    threshold_cp = 10
-    return threshold_error_alpha, threshold_error_D, threshold_error_s, threshold_cp
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 84
-def error_SingleTraj_dataset(df_pred, df_true, 
-                              threshold_error_alpha = 2, max_val_alpha = 2, min_val_alpha = 0, 
-                              threshold_error_D = 1e5, max_val_D = 1e6, min_val_D = 1e-6, 
-                              threshold_error_s = -1,
-                              threshold_cp = 10,
-                              prints = True, disable_tqdm = False
-                             ):
-    '''
-    Given two dataframes, corresponding to the predictions and true labels of a set
-    of trajectories from the ANDI 2 challenge022, calculates the corresponding metrics
-    Columns must be for both (no order needed):
-    traj_idx | alphas | Ds | changepoints | states
-    df_true must also contain a column 'T'.
-    
-    Parameters
-    ----------
-    df_pred : dataframe
-        Predictions
-    df_true : dataframe
-        Groundtruth
-    threshold_error_alpha : float
-        (same for D, s, cp) Maximum possible error allowed. If bigger, it is substituted by this error.
-    max_val_alpha : float
-        (same for D, s, cp) Maximum value of the parameter.
-    min_val_alpha : float
-        (same for D, s, cp) Minimum value of the parameter.
-    print : bool
-        If True, prints the results.
-    disable_tqdm : bool
-        If True, disables the progress bar.
-    
-    Returns
-    -------
-    tuple
-        - rmse_CP: root mean squared error change points
-        - JI: Jaccard index change points
-        - error_alpha: mean absolute error anomalous exponents
-        - error_D: mean square log error diffusion coefficients
-        - error_s: Jaccar index diffusive states
-    
-    '''
-    # Initiate counting missing trajectories
-    missing_traj = False
-    
-    # Deleter saving variables, just in case...
-    try: del paired_alpha, paired_D, paired_s
-    except: pass
-
-    # for every trajectory, we stack paired segment properties. We also store changepoints info
-    ensemble_pred_cp, ensemble_true_cp = [], []
-    for t_idx in tqdm(df_true['traj_idx'].values, disable = disable_tqdm):
-        
-        traj_trues = df_true.loc[df_true.traj_idx == t_idx]
-
-        traj_preds = df_pred.loc[df_pred.traj_idx == t_idx]    
-        if traj_preds.shape[0] == 0:
-            # If there is no trajectory, we give maximum error. To do so, we redefine predictions
-            # and trues so that they give maximum error
-            missing_traj += 1                       
-            
-            preds_cp, preds_alpha, preds_D, preds_s = [[10],
-                                                       [0],
-                                                       [1],
-                                                       [0]]
-
-            trues_cp, trues_alpha, trues_D, trues_s = [[10+threshold_cp],
-                                                       [threshold_error_alpha],
-                                                       [1+threshold_error_D],
-                                                       [10]]
-        
-        else:      
-
-            preds_cp, preds_alpha, preds_D, preds_s = [np.array(traj_preds.changepoints.values[0]).astype(int),
-                                                       traj_preds.alphas.values[0],
-                                                       traj_preds.Ds.values[0],
-                                                       traj_preds.states.values[0]]
-
-            trues_cp, trues_alpha, trues_D, trues_s = [np.array(traj_trues.changepoints.values[0]).astype(int),
-                                                       traj_trues.alphas.values[0],
-                                                       traj_trues.Ds.values[0],
-                                                       traj_trues.states.values[0]]
-
-
-        # Collecting changepoints for metric
-        # In this metric, we don't want to enter the final point of the trajectory
-        ensemble_pred_cp.append(preds_cp[:-1])
-        ensemble_true_cp.append(trues_cp[:-1])        
-        
-        # collecting segment properties error after segment assignment
-        pair_a, pair_d, pair_s = segment_property_errors(trues_cp, trues_alpha, trues_D, trues_s, 
-                                                         preds_cp, preds_alpha, preds_D, preds_s,
-                                                         return_pairs = True)
-        
-
-        
-        try:
-            paired_alpha = np.vstack((paired_alpha, pair_a))
-            paired_D = np.vstack((paired_D, pair_d))
-            paired_s = np.vstack((paired_s, pair_s))        
-        except:
-            paired_alpha = pair_a
-            paired_D = pair_d
-            paired_s = pair_s
-               
-    #### Calculate metrics from assembled properties   
-
-    # checking for nans and problems in predictions
-    wrong_alphas = np.argwhere(np.isnan(paired_alpha[:, 1]) | (paired_alpha[:, 1] > 2) | (paired_alpha[:, 1] < 0)).flatten()
-    paired_alpha[wrong_alphas, 1] = paired_alpha[wrong_alphas, 0] + threshold_error_alpha
-
-    wrong_ds = np.argwhere(np.isnan(paired_D[:, 1])).flatten()
-    paired_D = np.abs(paired_D)
-    paired_D[wrong_ds, 1] = paired_D[wrong_ds, 0] + threshold_error_D
-    
-    wrong_s = np.argwhere((paired_s[:, 1] > 4) | (paired_s[:, 1]<0))
-    paired_s[wrong_s, 1] = threshold_error_s    
-    
-    # Changepoints
-    rmse_CP, JI = ensemble_changepoint_error(ensemble_true_cp, ensemble_pred_cp, threshold = threshold_cp)
-
-    # Segment properties
-    error_alpha = metric_anomalous_exponent(paired_alpha[:,0], paired_alpha[:,1])
-    error_D = metric_diffusion_coefficient(paired_D[:,0], paired_D[:,1])
-    error_s = metric_diffusive_state(paired_s[:,0], paired_s[:,1])
-    
-    if prints:        
-        print(f'Summary of metrics assesments:')
-        if missing_traj is not False:            
-            print(f'\n{missing_traj} missing trajectory/ies. ')           
-        if rmse_CP == threshold_cp:
-            print(f'No change points found. RMSE set to max ({threshold_cp})')
-        print(f'\nChangepoint Metrics \nRMSE: {round(rmse_CP, 3)} \nJaccard Index: {round(JI, 3)}',
-              f'\n\nDiffusion property metrics \nMetric anomalous exponent: {error_alpha} \nMetric diffusion coefficient: {error_D} \nMetric diffusive state: {error_s}')
-              
-              
-
-    return rmse_CP, JI, error_alpha, error_D, error_s
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 96
-import re
-import sys
-import os
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 97
-def listdir_nohidden(path):
-    for f in os.listdir(path):
-        if not f.startswith(('.','_')):
-            yield f
-
-# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 98
-def codalab_scoring(input_dir , output_dir):
-    '''
-    Given an input directoy where predictions and groundtruths for the ANDI 2 challenge can be found,
-    calculates metrics and outputs the results in a file in the given output directory.
-    This code is prepared to be run in Codalab.
-    '''
-    
-    # Error bounds
-    threshold_error_alpha, threshold_error_D, threshold_error_s, threshold_cp = _get_error_bounds()
-    
-    ### Saving variables
-    # Track 1 - Videos
-    t1_ens = {'alpha': [],
-              'D': []}
-
-    t1_st = {'RMSE': [],
-             'JI': [],
-             'alpha': [],
-             'D': [],
-             'state': [],
-             'num_traj': [],
-             'num_traj_CP': []} # this last one takes into account no changepoint from single state
-
-    # Track 2 - Trajectories
-    t2_ens = {'alpha': [],
-              'D': []}
-
-    t2_st = {'RMSE': [],
-             'JI': [],
-             'alpha': [],
-             'D': [],
-             'state': [],
-             'num_traj': [],
-             'num_traj_CP': []} # this last one takes into account no changepoint from single state
-    
-    # Handling paths of input files
-    submit_dir = os.path.join(input_dir, 'pred')
-    truth_dir = os.path.join(input_dir, 'true')
-    if not os.path.isdir(submit_dir):
-        print( "%s doesn't exist", truth_dir)
-        
-    # Calculate metrics if directories exist
-    if os.path.isdir(submit_dir) and os.path.isdir(truth_dir):
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
-
-        # Extracts all files in reference directory
-        true_files_list = sorted(list(listdir_nohidden(truth_dir)))#os.listdir(truth_dir)
-
-        # Run over all files        
-        missing_tracks = []
-        for filename in tqdm(true_files_list):
-            task = re.search('_(.+?)_labs', filename).group(1)
-            exp = re.search('exp_(.+?)_', filename).group(1)
-            fov = re.search('fov_(.+?).', filename).group(1)
-            # check track and save found tracks
-            track = int(filename[1]) 
-            
-
-            true_file = os.path.join(truth_dir, filename)
-            corresponding_submission_file = os.path.join(submit_dir, filename)
-            
-            if not os.path.isfile(corresponding_submission_file):
-                if track not in missing_tracks:
-                    missing_tracks.append(track)
-                if len(missing_tracks) == 2:
-                    raise FileNotFoundError(f'Failed to find prediction files.')
-                else:
-                    continue
-            
-            # if not os.path.isfile(corresponding_submission_file) and missing_tracks == 1:
-            #     raise FileNotFoundError(f'Failed to find prediction files.')
-                # raise FileNotFoundError(f'Prediction file for: track {track}, task {task}, experiment {exp} and FOV {fov} not found.')
-            
-            # extract model
-            if task == 'ens':
-                model = np.genfromtxt(true_file, dtype='str', skip_footer=5)[1][:-1]
-            else:
-                file_ens = os.path.join(truth_dir, f't{track}_ens_labs_exp_{exp}_fov_{fov}.txt')
-                model = np.genfromtxt(file_ens, dtype='str', skip_footer=5)[1][:-1]
-            
-            # Ensemble
-            if task == 'ens':
-
-                true = np.loadtxt(true_file, skiprows=1, delimiter = ';')
-                pred = np.loadtxt(corresponding_submission_file, skiprows=1, delimiter = ';')
-
-                mae_alpha, mae_D, = error_Ensemble_dataset(true_data = true,
-                                                           pred_data = pred)
-
-                if track == 1:
-                    t1_ens['alpha'].append(mae_alpha)
-                    t1_ens['D'].append(mae_D)
-                if track == 2:                
-                    t2_ens['alpha'].append(mae_alpha)
-                    t2_ens['D'].append(mae_D)
-
-            # Single trajectory
-            if task == 'traj':    
-                df_true = load_file_to_df(true_file)
-                df_pred = load_file_to_df(corresponding_submission_file)
-
-                rmse_CP, JI, error_alpha, error_D, error_s = error_SingleTraj_dataset(df_true = df_true, df_pred = df_pred, 
-                                                                                      threshold_error_alpha = threshold_error_alpha,
-                                                                                      threshold_error_D = threshold_error_D, 
-                                                                                      threshold_error_s = threshold_error_s,
-                                                                                      threshold_cp = threshold_cp,
-                                                                                      prints = False, disable_tqdm = True)
-
-                if track == 1:
-                    # to avoid single state entering in CP metrics
-                    if model != 'single_state': 
-                        t1_st['RMSE'].append(rmse_CP)
-                        t1_st['JI'].append(JI)
-                        t1_st['num_traj_CP'].append(df_true.shape[0])
-                        
-                    t1_st['alpha'].append(error_alpha)
-                    t1_st['D'].append(error_D)
-                    t1_st['state'].append(error_s)                    
-                    t1_st['num_traj'].append(df_true.shape[0])
-                if track == 2:
-                    # to avoid single state entering in CP metrics
-                    if model != 'single_state': 
-                        t2_st['RMSE'].append(rmse_CP)
-                        t2_st['JI'].append(JI)
-                        t2_st['num_traj_CP'].append(df_true.shape[0])
-                    
-                    t2_st['alpha'].append(error_alpha)
-                    t2_st['D'].append(error_D)
-                    t2_st['state'].append(error_s)        
-                    t2_st['num_traj'].append(df_true.shape[0])
-
-            # print(f'Track {track}, Task {task}, Exp {exp}, FOV {fov}: OK!')
-       
-    ### Saving data
-    '''CHECK HOW TO DO THE MEAN!'''    
-    # Define output file
-    output_filename = os.path.join(output_dir, 'scores.txt')
-    output_file = open(output_filename, 'w')
-
-    # Single trajectory data
-    # We define a variable that gives the worst values for each metric. This is applied
-    # separetedly for every FOV
-    worst_value_st = {'RMSE': threshold_cp,
-                      'JI': 0,
-                      'alpha': threshold_error_alpha,
-                      'D': threshold_error_D,
-                      'state': 0}
-    # Run over all keys
-    for key in t1_st: 
-        
-        # Compare results with 
-        if key in ['RMSE', 'alpha', 'D']:            
-            if key == 'RMSE': avg_against = 'num_traj_CP'
-            else: avg_against = 'num_traj'
-            
-            if 1 not in missing_tracks:
-                
-                save_t1 = np.nanmin(np.vstack([t1_st[key],
-                                               np.ones_like(t1_st[key])*worst_value_st[key]]),
-                                    axis = 0)
-                save_t1 = np.average(save_t1, axis = 0, weights = t1_st[avg_against])
-                
-            if 2 not in missing_tracks:                     
-                save_t2 = np.nanmin(np.vstack([t2_st[key],
-                                               np.ones_like(t2_st[key])*worst_value_st[key]]),
-                                    axis = 0)            
-                save_t2 = np.average(save_t2, axis = 0, weights = t2_st[avg_against])
-            
-        elif key in ['JI', 'state']:                        
-            if key == 'JI': avg_against = 'num_traj_CP'
-            else: avg_against = 'num_traj'
-            
-            if 1 not in missing_tracks:
-                save_t1 = np.nanmax(np.vstack([t1_st[key],
-                                               np.ones_like(t1_st[key])*worst_value_st[key]]),
-                                    axis = 0)
-                save_t1 = np.average(save_t1, axis = 0, weights = t1_st[avg_against])
-                    
-            if 2 not in missing_tracks: 
-                save_t2 = np.nanmax(np.vstack([t2_st[key],
-                                               np.ones_like(t2_st[key])*worst_value_st[key]]),
-                                    axis = 0)           
-                save_t2 = np.average(save_t2, axis = 0, weights = t2_st[avg_against])
-
-        if 1 not in missing_tracks: 
-            output_file.write('T1_st_'+ key +f' : {save_t1}\n')    
-        if 2 not in missing_tracks: 
-            output_file.write('T2_st_'+ key +f' : {save_t2}\n')
-
-    ### Saving ensemble data
-    '''WHAT ARE THE THRESHOLDS FOR THIS?'''
-    worst_value_ens = {'alpha': 100,
-                       'D': 100}
-
-    for key in t1_ens: 
-        if key == 'num_traj': continue
-        
-        if 1 not in missing_tracks: 
-            save_t1 = np.nanmin(np.vstack([t1_ens[key],
-                                               np.ones_like(t1_ens[key])*worst_value_ens[key]]),
-                                    axis = 0).mean()
-        if 2 not in missing_tracks: 
-            save_t2 = np.nanmin(np.vstack([t2_ens[key],
-                                               np.ones_like(t2_ens[key])*worst_value_ens[key]]),
-                                    axis = 0).mean()
-
-        if 1 not in missing_tracks: 
-            output_file.write('T1_ens_'+ key +f' : {save_t1}\n')    
-        if 2 not in missing_tracks: 
-            output_file.write('T2_ens_'+ key +f' : {save_t2}\n')
-
-    output_file.close()
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/utils_challenge.ipynb.
+
+# %% auto 0
+__all__ = ['majority_filter', 'label_filter', 'label_continuous_to_list', 'label_list_to_continuous', 'array_to_df',
+           'df_to_array', 'get_VIP', 'changepoint_assignment', 'changepoint_alpha_beta', 'jaccard_index',
+           'single_changepoint_error', 'ensemble_changepoint_error', 'create_binary_segment',
+           'jaccard_between_segments', 'segment_assignment', 'metric_anomalous_exponent',
+           'metric_diffusion_coefficient', 'metric_diffusive_state', 'check_no_changepoints', 'segment_property_errors',
+           'extract_ensemble', 'multimode_dist', 'distribution_distance', 'error_Ensemble_dataset',
+           'check_prediction_length', 'separate_prediction_values', 'load_file_to_df', 'error_SingleTraj_dataset',
+           'listdir_nohidden', 'codalab_scoring']
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 2
+import numpy as np
+from scipy.optimize import linear_sum_assignment
+import pandas
+from tqdm.auto import tqdm
+import warnings
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 6
+def majority_filter(seq, width):
+    '''
+    Given a vector, applies a majority filter of given width.
+    
+    Parameters
+    ----------
+    seq : list
+        Vector to filter.
+    width : int
+        Size of the window in which the filter is applied.
+    
+    Returns
+    -------
+    list
+        Filtered vector
+    '''
+    offset = width // 2
+    seq = [0] * offset + seq
+    return [max(set(a), key=a.count) 
+        for a in (seq[i:i+width] for i in range(len(seq) - offset))]
+
+def label_filter(label, 
+                 window_size = 5, 
+                 min_seg = 3):
+    '''
+    Given a vector of changing labels, applies a majority filter such that the minimum segment of a particular label is
+    bigger than the minimum set segment.
+    
+    Parameters
+    ----------
+    label : list
+        label vector to filter.
+    window_size : int
+        Size of the window in which the majority filter is applied.
+    min_seg : int
+        Minimum segment size after filtering.
+    
+    Returns
+    -------
+    np.array
+        Filtered label vector
+    '''
+    
+    if np.min(label) < 0:
+        raise ValueError('This function only works with positive labels')
+        
+    # if there are no changes:
+    if np.sum(label[1:] != label[:-1]) == 0:
+        return label
+    
+    # define dummy vector with all zeros and ones
+    values, dummy = np.unique(label, return_inverse = True)
+    
+    # check if there are segment smaller than minimal segment (min_seg)
+    cp = np.argwhere(dummy[1:] != dummy[:-1])
+    cp = np.append(0, cp)
+    current_min = (cp[1:]-cp[:-1]).flatten().min()
+
+    while (current_min < min_seg):
+
+        filt = majority_filter(dummy.tolist(), width = window_size)
+        filt = np.array(filt)
+        
+        # check if there are segment smaller than minimal segment (min_seg)
+        cp = np.argwhere(filt[1:] != filt[:-1])
+        
+        # If all changepoints were eliminated
+        if cp.size == 0:
+            break
+            
+        cp = np.append(0, cp)
+        current_min = (cp[1:]-cp[:-1]).flatten().min()
+        
+        if (dummy == filt).all():  
+            # If all failed and still have segments smaller than min_seg
+            seg_lengths = (cp[1:]-cp[:-1]).flatten().astype(int)
+            seg_smaller = np.argwhere(seg_lengths < min_seg).flatten()
+            
+            # We go over each segment and we asign the values 'by hand'
+            for idxsegs in seg_smaller:     
+                if seg_lengths[idxsegs] == 1:
+                    filt[(cp[idxsegs]+1)] = filt[cp[idxsegs]]     
+                elif seg_lengths[idxsegs] == 2:      
+                    filt[(cp[idxsegs]+1)] = filt[cp[idxsegs]]     
+                    filt[(cp[idxsegs]+2)] = filt[cp[idxsegs]+3]                     
+            
+            dummy = filt
+            break         
+        dummy = filt
+        
+        
+    # Check boundaries
+    if dummy[0] != dummy[1] or dummy[1] != dummy[2]:
+        dummy[:2] = dummy[2]
+    if dummy[-2] != dummy[-3] or dummy[-1] != dummy[-2]:
+        dummy[-3:] = dummy[-3]
+        
+    # reset to label values
+    dummy_ret = np.zeros_like(dummy).astype(float)
+    
+    for idx, v in enumerate(values):
+        dummy_ret[dummy == idx] = v
+
+    return dummy_ret
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 16
+def label_continuous_to_list(labs):
+    ''' 
+    Given an array of T x 2 labels containing the anomalous exponent and diffusion 
+    coefficient at each timestep, returns 3 arrays, each containing the changepoints, 
+    exponents and coefficient, respectively. 
+    If labs is size T x 3, then we consider that diffusive states are given and also
+    return those.
+    
+    Parameters
+    ----------
+    labs : array
+        T x 2  or T x 3 labels containing the anomalous exponent, diffusion 
+        and diffusive state.
+        
+    Returns
+    -------
+    tuple
+        - First element is the list of change points
+        - The rest are corresponding segment properties (order: alpha, Ds and states)        
+        '''
+    
+    # Check if states were given
+    are_states = False
+    if labs.shape[1] == 3:
+        are_states = True
+        
+    # Check in which variable there is changes
+    CP = np.argwhere((labs[:-1, :] != labs[1:, :]).sum(1) != 0).flatten()+1 
+    T = labs.shape[0] 
+
+    alphas = np.zeros(len(CP)+1)
+    Ds = np.zeros(len(CP)+1)
+    if are_states: states = np.zeros(len(CP)+1)
+        
+    for idx, cp in enumerate(np.append(CP, T)):
+        alphas[idx] = labs[cp-1, 0]
+        Ds[idx] = labs[cp-1, 1]
+        if are_states: states[idx] = labs[cp-1, 2]
+    
+    CP = np.append(CP, T)
+    
+    if are_states:
+        return CP, alphas, Ds, states
+    else:
+        return CP, alphas, Ds    
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 20
+def label_list_to_continuous(CP, label):
+    '''
+    Given a list of change points and the labels of the diffusion properties of the
+    resulting segments, generates and array of continuous labels. The last change point
+    indicates the array length.
+    
+    Parameters
+    ----------
+    CP : array, list
+        list of change points. Last change point indicates label length.
+    label : array, list
+        list of segment properties
+        
+    Returns
+    -------
+    array
+        Continuous label created from the given change points and segment properties
+    '''    
+    
+    if isinstance(label, list):
+        label = np.array(label)
+    segs = create_binary_segment(CP[:-1], CP[-1])
+    return (segs.transpose()*label).sum(1)
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 24
+from .utils_trajectories import segs_inside_fov
+
+
+def array_to_df(trajs, 
+               labels,
+               min_length = 10,
+               fov_origin = [0,0], fov_length= 100.0, cutoff_length = 10):
+    '''
+    Given arrays for the position and labels of trajectories, creates a dataframe with that
+    data. The function also applies the demanded FOV. If you don't want a field of view, chose a 
+    FOV length bigger (smaller) that your maximum (minimum) trajectory position.
+   
+    Parameters
+    ----------
+    trajs : array 
+        Trajectories to store in the df (dimension: T x N x 3)
+    labels : array
+        Labels to store in the df (dimension: T x N x 3)        
+    fov_origin : tuple
+        Bottom left point of the square defining the FOV.
+    fov_length : float
+        Size of the box defining the FOV.
+    cutoff_length : int
+        Minimum length of a trajectory inside the FOV to be considered in the output dataset.
+    
+    
+    Returns
+    -------
+    tuple
+        - df_in (dataframe): dataframe with trajectories
+        - df_out (datafram): dataframe with labels 
+    '''
+    
+    xs = []
+    ys = []
+    idxs = []   
+    
+    df_out = pandas.DataFrame(columns = ['traj_idx', 'Ds', 'alphas', 'states', 'changepoints']) 
+    
+    idx_t = 0
+    for traj, l_alpha, l_D, l_s in zip(tqdm(trajs), labels[:, :, 0], labels[:, :, 1], labels[:, :, 2]):
+
+        # Check FOV and 
+        idx_inside_segments = segs_inside_fov(traj, fov_origin, fov_length, cutoff_length)
+
+        if idx_inside_segments is not None:
+
+            for idx_in in idx_inside_segments:            
+                seg_x = traj[idx_in[0]:idx_in[1], 0]
+                seg_y = traj[idx_in[0]:idx_in[1], 1]
+                seg_alpha = l_alpha[idx_in[0]:idx_in[1]]
+                seg_D = l_D[idx_in[0]:idx_in[1]]
+                seg_state = l_s[idx_in[0]:idx_in[1]]
+
+                # Filtering
+                seg_alpha = label_filter(seg_alpha)
+                seg_D = label_filter(seg_D)
+                seg_state = label_filter(seg_state)
+                
+                
+                # Stacking data of input dataframe
+                xs += seg_x.tolist()
+                ys += seg_y.tolist()
+                idxs += (np.ones(len(seg_x))*idx_t).tolist()
+                
+                # Transforming to list of changepoints and physical properties
+                merge = np.hstack((seg_alpha.reshape(seg_alpha.shape[0], 1),
+                                   seg_D.reshape(seg_D.shape[0], 1),
+                                   seg_state.reshape(seg_state.shape[0], 1)))
+                
+                CP, alphas, Ds, states = label_continuous_to_list(merge)
+                
+                # Saving each segment info in output dataframe
+                df_out.loc[df_out.shape[0]] = [idx_t, Ds, alphas, states, CP]
+                
+                # Updating segment index
+                idx_t += 1
+
+    
+    # Saving trajectories in Dataframe
+    tr_to_df = np.vstack((idxs,
+                          xs,
+                          ys)).transpose()
+    df_in = pandas.DataFrame(tr_to_df, columns = ['traj_idx', 'x', 'y'])  
+    
+    return df_in, df_out
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 29
+def df_to_array(df, pad = -1):
+    '''
+    Transform a dataframe as the ones given in the ANDI 2 challenge (i.e. 4 columns:
+    traj_idx, frame, x, y) into a numpy array. To deal with irregular temporal supports,
+    we pad the array whenever the trajectory is not present.
+    The output array has the typical shape of ANDI datasets: TxNx2
+    
+    Parameters
+    ----------
+    df : dataframe
+        Dataframe with four columns 'traj_idx': the trajectory index, 'frame' the time frame and 
+        'x' and 'y' the positions of the particle.
+    pad : int
+        Number to use as padding.
+    
+    Returns
+    -------
+    array
+        Array containing the trajectories from the dataframe, with usual ANDI shape (TxNx2).
+    
+    
+    '''
+
+    max_T = int(df.frame.max()+1)
+    num_part = int(df.iloc[-1].traj_idx)
+    array_trajs = np.ones((max_T, num_part+1, 2))*pad
+
+    for idx in np.unique(df.traj_idx).astype(int):
+
+        df_part = df.loc[df.traj_idx == idx]
+
+        array_trajs[df_part.frame.values.astype(int), idx, 0] = df_part.x.values
+        array_trajs[df_part.frame.values.astype(int), idx, 1] = df_part.y.values
+        
+    return array_trajs
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 31
+from scipy.spatial import distance
+
+
+def get_VIP(array_trajs, num_vip = 5, min_distance = 2, pad = -1):
+    '''
+    Given an array of trajectories, finds the particles VIP particles that participants will
+    need to characterize in the video trakcl.
+    
+    The function first finds the particles that exist at frame 0 (i.e. that their first value 
+    is different from pad). Then, iterates over this particles to find num_vip that are at 
+    distance > than min_distance in the first frame.
+    
+    Parameters
+    ----------
+    array_trajs : array
+        Position of the trajectories that will be considered for the VIP search.
+    num_vip : int
+        Number of VIP particles to flag.
+    min_distance : float
+        Minimum distance between two VIP particles.
+    pad : int
+        Number used to indicate in the temporal support that the particle is outside of the FOV.
+        
+    Returns
+    -------
+    list
+        List of indices of the chosen VIP particles
+    
+    '''
+    
+    candidates_vip = np.argwhere(array_trajs[0,:,0] != pad).flatten()
+    if len(candidates_vip) < num_vip:
+        raise ValueError('Number of VIP demanded is bigger than available particles.')
+
+    elected = []
+    count_while = 0
+    while len(elected) < num_vip:
+
+        elected = [np.random.choice(candidates_vip)]
+
+        for c_idx in candidates_vip:
+            if c_idx == elected[0]:
+                continue
+            if len(array_trajs[0, elected,:].shape) < 2:
+                all_rest = np.expand_dims(array_trajs[0, elected,:], 0)
+            else:
+                all_rest = array_trajs[0, elected,:]
+
+            dist = distance.cdist(np.expand_dims(array_trajs[0,c_idx,:], 0), all_rest, metric='euclidean').transpose()
+
+            if dist.min() > 2:
+                elected.append(c_idx)
+
+            if len(elected) == num_vip:
+                break
+
+
+        count_while += 1
+        if count_while > 100: 
+            raise ValueError('Could not find suitable VIP particles. This is due to either having to few particles or them being too close')
+            
+    return elected
+
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 34
+def changepoint_assignment(GT, preds):
+    ''' 
+    Given a list of groundtruth and predicted changepoints, solves the assignment problem via
+    the Munkres algorithm (aka Hungarian algorithm) and returns two arrays containing the index of the
+    paired groundtruth and predicted changepoints, respectively.
+    
+    The distance between change point is the Euclidean distance.
+    
+    Parameters
+    ----------
+    GT : list
+        List of groundtruth change points.
+    preds : list
+        List of predicted change points.
+    
+    Returns
+    -------
+    tuple
+        - tuple of two arrays, each corresponding to the assigned GT and pred changepoints
+        - Cost matrix
+    
+    '''
+    
+    cost_matrix = np.zeros((len(GT), len(preds)))
+
+    for idxg, gt in enumerate(GT):
+        for idxp, pred in enumerate(preds):
+            cost_matrix[idxg, idxp] = np.abs(gt-pred)
+            
+    return linear_sum_assignment(cost_matrix), cost_matrix
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 36
+def changepoint_alpha_beta(GT, preds, threshold = 10):
+    '''
+    Calculate the alpha and beta measure of paired changepoints.
+    Inspired from Supplemantary Note 3 in https://www.nature.com/articles/nmeth.2808
+    
+    Parameters
+    ----------
+    GT : list
+        List of groundtruth change points.
+    preds : list
+        List of predicted change points.
+    threshold : float
+        Distance from which predictions are considered to have failed. They are then assigned this number.
+    
+    Returns
+    -------
+    tuple
+        alpha, beta
+        
+    '''
+
+    assignment, _ = changepoint_assignment(GT, preds)
+    assignment = np.array(assignment)
+
+    threshold = 10
+    distance = np.abs(GT[assignment[0]] - preds[assignment[1]])
+    distance[distance > threshold] = threshold
+    distance = np.sum(distance)
+
+    d_x_phi = threshold*len(GT)
+    d_ybar_phi = max([0, (len(preds)-len(GT))*threshold])
+
+    alpha = 1-distance/d_x_phi
+    beta = (d_x_phi-distance)/(d_x_phi+d_ybar_phi)
+
+    return alpha, beta
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 38
+def jaccard_index(TP: int, # true positive
+                  FP: int, # false positive
+                  FN: int # false negative
+                 )-> float: # Jaccard Index
+    '''
+    Given the true positive, false positive and false negative rates, calculates the Jaccard Index
+    '''
+    return TP/(TP+FP+FN)
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 39
+def single_changepoint_error(GT, preds, threshold = 5):
+    '''
+    Given the groundtruth and predicted changepoints for a single trajectory, first solves the assignment problem between changepoints,
+    then calculates the RMSE of the true positive pairs and the Jaccard index.
+    
+    Parameters
+    ----------
+    GT : list
+        List of groundtruth change points.
+    preds : list
+        List of predicted change points.
+    threshold : float
+        Distance from which predictions are considered to have failed. They are then assigned this number.
+    
+    Returns
+    -------
+    tuple
+        - TP_rmse: root mean square error of the true positive change points.
+        - Jaccard Index of the ensemble predictions        
+        
+    '''
+    
+    assignment, _ = changepoint_assignment(GT, preds)
+    assignment = np.array(assignment)
+    
+    TP, FP, FN = 0, 0, 0
+    TP_rmse = []
+    for p in assignment.transpose():
+        
+        if np.abs(GT[p[0]] - preds[p[1]]) < threshold:
+            TP += 1
+            TP_rmse.append((GT[p[0]] - preds[p[1]])**2)
+        else:
+            FP += 1
+            FN += 1
+    # Calculating RMSE
+    TP_rmse = np.sqrt(np.mean(TP_rmse))
+
+    # Checking false positive and missed events
+    if len(preds) > len(GT):
+        FP += len(preds) - len(GT)
+    elif len(preds) < len(GT):
+        FN += len(GT) - len(preds)
+    
+    return TP_rmse, jaccard_index(TP, FP, FN)
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 40
+def ensemble_changepoint_error(GT_ensemble, pred_ensemble, threshold = 5):    
+    ''' 
+    Given an ensemble of groundtruth and predicted change points, iterates
+    over each trajectory's changepoints. For each, it solves the assignment problem 
+    between changepoints. Then, calculates the RMSE of the true positive pairs and
+    the Jaccard index over the ensemble of changepoints (i.e. not the mean of them 
+    w.r.t. to the trajectories)
+    
+    Parameters
+    ----------
+    GT_ensemble : list, array
+        Ensemble of groutruth change points.
+    pred_ensemble : list
+        Ensemble of predicted change points.
+    threshold : float
+        Distance from which predictions are considered to have failed. They are then assigned this number.
+    
+    Returns
+    -------
+    tuple
+        - TP_rmse: root mean square error of the true positive change points.
+        - Jaccard Index of the ensemble predictions
+    
+    '''
+    
+    TP, FP, FN = 0, 0, 0
+    TP_rmse = []
+    
+    for gt_traj, pred_traj in zip(GT_ensemble, pred_ensemble):
+        
+        assignment, _ = changepoint_assignment(gt_traj, pred_traj)
+        assignment = np.array(assignment)
+        
+        for p in assignment.transpose():
+            
+            if np.abs(gt_traj[p[0]] - pred_traj[p[1]]) < threshold:
+                TP += 1
+                TP_rmse.append((gt_traj[p[0]] - pred_traj[p[1]])**2)
+            else:
+                FP += 1
+                FN += 1    
+                
+        # Checking false positive and missed events
+        if len(pred_traj) > len(gt_traj):
+            FP += len(pred_traj) - len(gt_traj)
+        elif len(pred_traj) < len(gt_traj):
+            FN += len(gt_traj) - len(pred_traj)
+                
+    if TP+FP+FN == 0:
+        wrn_str = f'No segments found in this dataset.'
+        warnings.warn(wrn_str)
+        return threshold, 0
+        
+    # Calculating RMSE
+    TP_rmse = np.sqrt(np.mean(TP_rmse))
+
+    
+        
+    return TP_rmse, jaccard_index(TP, FP, FN)
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 43
+def create_binary_segment(CP: list, # list of changepoints
+                          T: int # length of the trajectory
+                         )-> list: # list of arrays with value 1 in the temporal support of the current segment.
+    '''
+    Given a set of changepoints and the lenght of the trajectory, create segments which are equal to one
+    if the segment takes place at that position and zero otherwise.
+    '''
+    segments = np.zeros((len(CP)+1, T))
+    CP = np.append(0, CP)
+    for idx, (cp1, cp2) in enumerate(zip(CP[:-1], CP[1:])):
+        segments[idx, cp1+1:cp2+1] = 1
+    segments[-1, CP[-1]+1:] = 1
+    segments[0, 0] = 1
+    return segments
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 45
+def jaccard_between_segments(gt, pred):
+    '''
+    Given two segments, calculates the Jaccard index between them by considering TP as correct labeling,
+    FN as missed events and FP leftover predictions.
+    
+    Parameters
+    ----------
+    gt : array
+        groundtruth segment, equal to one in the temporal support of the given segment, zero otherwise.
+    pred : array
+        predicted segment, equal to one in the temporal support of the given segment, zero otherwise.
+    
+    Returns
+    -------
+    float
+        Jaccard index between the given segments.
+    '''
+    
+    if len(gt) > len(pred):
+        pred = np.append(pred, np.zeros(len(gt) - len(pred)))
+    elif len(pred) > len(gt):                        
+        gt = np.append(gt, np.zeros(len(pred) - len(gt)))
+    
+    
+    tp = np.sum(np.logical_and(pred == 1, gt == 1))
+    fp = np.sum(np.logical_and(pred == 1, gt == 0))
+    fn = np.sum(np.logical_and(pred == 0, gt == 1))
+    
+    # special case for absence of changepoint
+    if tp+fp+fn == 0: return 0    
+    else: return jaccard_index(tp, fp, fn)
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 46
+def segment_assignment(GT, preds, T:int = None):
+    ''' 
+    Given a list of groundtruth and predicted changepoints, generates a set of segments. Then constructs 
+    a cost matrix by calculting the Jaccard Index between segments. From this cost matrix, we solve the 
+    assignment  problem via the Munkres algorithm (aka Hungarian algorithm) and returns two arrays 
+    containing the index of the groundtruth and predicted segments, respectively.
+    
+    If T = None, then we consider that GT and preds may have different lenghts. In that case, the end
+    of the segments is the the last CP of each set of CPs.
+    
+    Parameters
+    ----------
+    GT : list
+        List of groundtruth change points.
+    preds : list
+        List of predicted change points.
+    T : int, None
+        Length of the trajectory. If None, considers different GT and preds length.
+    
+    Returns
+    -------
+    tuple
+        - tuple of two arrays, each corresponding to the assigned GT and pred changepoints
+        - Cost matrix calculated via JI of segments   
+    
+    '''
+   
+    if T is not None:
+        T_gt = T_pred = T
+        # Check if the GT or predictions are a single integer or an empty array
+        if isinstance(GT, int): GT = [GT]
+        elif len(GT) == 0: GT = [T-1]
+
+        if isinstance(preds, int): preds = [preds]
+        elif len(preds) == 0: preds = [T-1]
+    else:
+        T_gt = GT[-1]
+        if len(GT) > 1:
+            GT = GT[:-1]            
+            
+        T_pred = preds[-1]
+        if len(preds) > 1:
+            preds = preds[:-1]
+        
+    
+    
+    seg_GT = create_binary_segment(GT, T_gt)
+    seg_preds = create_binary_segment(preds, T_pred)
+    
+    cost_matrix = np.zeros((seg_GT.shape[0], seg_preds.shape[0]))
+
+    for idxg, gt in enumerate(seg_GT):
+        for idxp, pred in enumerate(seg_preds):
+            cost_matrix[idxg, idxp] = 1-jaccard_between_segments(gt, pred)
+
+    return linear_sum_assignment(cost_matrix), cost_matrix
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 56
+from sklearn.metrics import mean_squared_log_error as msle, f1_score
+from .models_phenom import models_phenom
+
+def metric_anomalous_exponent(gt = None,
+                              pred = None,
+                              max_error = np.abs(models_phenom().bound_alpha[0]-models_phenom().bound_alpha[1])):
+    ''' 
+    Compute the mean absolute error (mae) between anomalous exponents.
+    Checks the current bounds of anomalous exponents from models_phenom to calculate the maximum error.
+    ''' 
+    error = np.mean(np.abs(gt-pred))
+    if error > max_error:
+        return max_error
+    else: 
+        return error
+
+def metric_diffusion_coefficient(gt = None, pred = None, 
+                                 threshold_min = models_phenom().bound_D[0],                               
+                                 max_error = msle([models_phenom().bound_D[0]],
+                                                  [models_phenom().bound_D[1]])):
+    ''' 
+    Compute the mean squared log error (msle) between diffusion coefficients.
+    Checks the current bounds of diffusion from models_phenom to calculate the maximum error. 
+    ''' 
+    
+     # considering the presence of zeros and negatives
+    pred = np.array(pred).copy(); gt = np.array(gt).copy()
+    pred[pred <= threshold_min] = threshold_min
+    gt[gt <= threshold_min] = threshold_min    
+    # mean squared log error
+    error = msle(gt, pred)
+    
+    if error > max_error:
+        return max_error
+    else: 
+        return error
+
+def metric_diffusive_state(gt = None, pred = None, max_error = False):
+    ''' 
+    Compute the F1 score between diffusive states. 
+    ''' 
+    return f1_score(gt.astype(int), pred.astype(int), average = 'micro')
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 60
+def check_no_changepoints(GT_cp, GT_alpha, GT_D, GT_s,
+                          preds_cp, preds_alpha, preds_D, preds_s,
+                          T:bool|int = None):
+    '''
+    Given predicionts over changepoints and variables, checks if in both GT and preds there is an 
+    absence of change point. If so, takes that into account to pair variables.
+    
+    Parameters
+    ----------
+    GT_cp : list, int, float
+        Groundtruth change points
+    GT_alpha : list, float
+        Groundtruth anomalous exponent
+    GT_D : list, float
+        Groundtruth diffusion coefficient
+    GT_s : list, float
+        Groundtruth diffusive state
+    preds_cp : list, int, float
+        Predicted change points
+    preds_alpha : list, float
+        Predicted anomalous exponent
+    preds_D : list, float
+        Predicted diffusion coefficient
+    preds_s : list, float
+        Predicted diffusive state
+    T : bool,int
+        (optional) Length of the trajectories. If none, last change point is length.
+    
+    Returns
+    -------
+    tuple
+        - False if there are change points. True if there were missing change points.
+        - Next three are either all Nones if change points were detected, or paired exponents, 
+        coefficient and states if some change points were missing.
+    
+    '''
+
+
+    if isinstance(GT_cp, int) or isinstance(GT_cp, float):
+        GT_cp = [GT_cp]
+    if isinstance(preds_cp, int) or isinstance(preds_cp, float):
+        preds_cp = [preds_cp]
+        
+    no_GT_cp = False; no_preds_cp = False
+    # CP always contain the final point of the trajectory, hence minimal length is one
+    if len(GT_cp) == 1: no_GT_cp = True
+    if len(preds_cp) == 1: no_preds_cp = True       
+        
+
+    if no_GT_cp + no_preds_cp == 0:
+        return False, None, None, None
+    
+    else:
+
+        [row_ind, col_ind], _ = segment_assignment(GT_cp, preds_cp, T)   
+
+        if no_GT_cp and not no_preds_cp:
+            paired_alpha = np.array([[GT_alpha[0], preds_alpha[col_ind[0]]]])
+            paired_D = np.array([[GT_D[0], preds_D[col_ind[0]]]])
+            paired_s = np.array([[GT_s[0], preds_s[col_ind[0]]]])
+
+        if no_preds_cp and not no_GT_cp:
+            row_position = np.argwhere(col_ind == 0).flatten()[0]            
+            paired_alpha = np.array([[GT_alpha[row_position], preds_alpha[col_ind[row_position]]]])
+            paired_D = np.array([[GT_D[row_position], preds_D[col_ind[row_position]]]])
+            paired_s = np.array([[GT_s[row_position], preds_s[col_ind[row_position]]]])
+            
+        if no_preds_cp and no_GT_cp: 
+            paired_alpha = np.array([[GT_alpha[0], preds_alpha[0]]])
+            paired_D = np.array([[GT_D[0], preds_D[0]]])
+            paired_s = np.array([[GT_s[0], preds_s[0]]])
+            
+
+        return True, paired_alpha, paired_D, paired_s
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 61
+def segment_property_errors(GT_cp, GT_alpha, GT_D, GT_s,
+                            preds_cp, preds_alpha, preds_D, preds_s,
+                            return_pairs = False,
+                            T = None):
+    '''
+    Given predicionts over change points and the value of diffusion parameters in the generated
+    segments, computes the defined metrics.
+    
+    Parameters
+    ----------
+    GT_cp : list, int, float
+        Groundtruth change points
+    GT_alpha : list, float
+        Groundtruth anomalous exponent
+    GT_D : list, float
+        Groundtruth diffusion coefficient
+    GT_s : list, float
+        Groundtruth diffusive state
+    preds_cp : list, int, float
+        Predicted change points
+    preds_alpha : list, float
+        Predicted anomalous exponent
+    preds_D : list, float
+        Predicted diffusion coefficient
+    preds_s : list, float
+        Predicted diffusive state
+    return_pairs : bool
+        If True, returns the assigment pairs for each diffusive property.
+    T : bool,int
+        (optional) Length of the trajectories. If none, last change point is length.
+    
+    Returns
+    -------
+    tuple
+        - if return_pairs = True, returns the assigned pairs of diffusive properties
+        - if return_pairs = False, returns the errors for each diffusive property
+    '''
+    
+    # Check cases in which changepoint where not detected or there were none in groundtruth
+    no_change_point_case, paired_alpha, paired_D, paired_s = check_no_changepoints(GT_cp, GT_alpha, GT_D, GT_s,
+                                                                                   preds_cp, preds_alpha, preds_D, preds_s, T)
+   
+    if not no_change_point_case:
+        # Solve the assignment problem
+        [row_ind, col_ind], _ = segment_assignment(GT_cp, preds_cp, T)
+   
+        # iterate over the groundtruth segments
+        paired_alpha, paired_D, paired_s = [], [], []
+        for idx_seg, (gt_alpha, gt_D) in enumerate(zip(GT_alpha, GT_D)):
+
+            row_position = np.argwhere(row_ind == idx_seg).flatten()
+
+            # if the GT segment was associated to a prediction
+            if len(row_position) > 0:
+                row_position = int(row_position)
+                # alpha                
+                gt_a_seg = GT_alpha[idx_seg]                
+                pred_a_seg = preds_alpha[col_ind[row_position]]
+                # d
+                gt_d_seg = GT_D[idx_seg]
+                pred_d_seg = preds_D[col_ind[row_position]]
+                # state
+                gt_s_seg = GT_s[idx_seg]
+                pred_s_seg = preds_s[col_ind[row_position]]
+
+                paired_alpha.append([gt_a_seg, pred_a_seg])
+                paired_D.append([gt_d_seg, pred_d_seg])
+                paired_s.append([gt_s_seg, pred_s_seg])
+
+        paired_alpha, paired_D, paired_s = np.array(paired_alpha), np.array(paired_D), np.array(paired_s) 
+    
+    if return_pairs:
+        return paired_alpha, paired_D, paired_s 
+    else:
+        error_alpha = metric_anomalous_exponent(paired_alpha[:,0], paired_alpha[:,1])
+        error_D = metric_diffusion_coefficient(paired_D[:,0], paired_D[:,1])
+        error_s = metric_diffusive_state(paired_s[:,0], paired_s[:,1])
+        return error_alpha, error_D, error_s
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 69
+from .models_phenom import models_phenom
+def extract_ensemble(state_label, dic):
+        ''' 
+        Given an array of the diffusive state and a dictionary with the diffusion information,
+        returns a summary of the ensemble properties for the current dataset.
+
+        Parameters
+        ----------
+        state_label : array
+            Array containing the diffusive state of the particles in the dataset.
+            For multi-state and dimerization, this must be the number associated to the
+            state (for dimerization, 0 is free, 1 is dimerized). For the rest, we follow
+            the numeration of models_phenom().lab_state.
+        dic : dict 
+            Dictionary containing the information of the input dataset.
+       
+       Returns
+       -------
+       array
+           Matrix containing the ensemble information of the input dataset. It has the following shape:
+            |mu_alpha1      mu_alpha2     ... |
+            |sigma_alpha1   sigma_alpha2  ... |
+            |mu_D1          mu_D1         ... | 
+            |sigma_D1       sigma_D2      ... |
+            |counts_state1  counts_state2 ... |
+        '''
+
+        # Single state
+        if dic['model'] == 'single_state': 
+            ensemble = np.vstack((dic['alphas'][0],
+                                   dic['alphas'][1],
+                                   dic['Ds'][0],
+                                   dic['Ds'][1],
+                                   len(state_label)
+                                   ))
+        # Multi-state
+        if dic['model'] == 'multi_state':
+            states, counts = np.unique(state_label, return_counts=True)    
+            # If the number of visited stated is not equal to the expected number of states
+            if len(states) != dic['alphas'].shape[0]:
+                states_corrected = np.ones(dic['alphas'].shape[0])
+                counts_corrected = np.ones(dic['alphas'].shape[0])
+                for s, c in zip(states, counts):
+                    counts_corrected[int(s)] = c
+            else: 
+                counts_corrected = counts
+
+            ensemble = np.vstack((dic['alphas'][:, 0],
+                                   dic['alphas'][:, 1],
+                                   dic['Ds'][:, 0],
+                                   dic['Ds'][:, 1],
+                                   counts_corrected
+                                   ))
+
+        # Immobile
+        if dic['model'] == 'immobile_traps':
+            counts = [len(state_label[state_label == models_phenom().lab_state.index('i')]),
+                      len(state_label[state_label == models_phenom().lab_state.index('f')])]  
+            ensemble = np.vstack(([0, dic['alphas'][0]],
+                                   [0, dic['alphas'][1]],
+                                   [0, dic['Ds'][0]],
+                                   [0, dic['Ds'][1]],
+                                   counts
+                                   ))
+        # dimerization    
+        if dic['model'] == 'dimerization':
+            counts = [len(state_label[state_label == 0]),
+                      len(state_label[state_label == 1])]           
+            ensemble = np.vstack((dic['alphas'][:, 0],
+                                   dic['alphas'][:, 1],
+                                   dic['Ds'][:, 0],
+                                   dic['Ds'][:, 1],
+                                   counts
+                                   ))
+
+        if dic['model'] == 'confinement':
+            counts = [len(state_label[state_label == models_phenom().lab_state.index('f')]),
+                      len(state_label[state_label == models_phenom().lab_state.index('c')])]   
+            ensemble = np.vstack((dic['alphas'][:, 0],
+                                   dic['alphas'][:, 1],
+                                   dic['Ds'][:, 0],
+                                   dic['Ds'][:, 1],
+                                   counts
+                                   ))
+        return ensemble
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 70
+import scipy.stats
+def multimode_dist(params, weights, bound, x, normalized = False):
+    '''
+    Generates a multimodal distribution with given parameters.
+    Also accounts for single mode if weight is float or int.
+    
+    Parameters
+    ----------
+    params : list
+        Mean and variances of every mode.
+    weights : list, float
+        Weight of every mode. If float, we consider a single mode.
+    bound : tuple
+        Bounds (min, max) of the functions support.
+    x : array
+        Support upon which the distribution is created.
+    normalize : bool
+        If True, returns the normalized distribution.
+    
+    Returns
+    -------
+    array
+        Value of the distribution in each point of the given support
+        
+    '''
+    func = scipy.stats.truncnorm
+    dist = np.zeros_like(x)
+    lower, upper = bound 
+   
+    # If we have single state, change values to list to still
+    # have a loop:
+    if isinstance(weights, float) or isinstance(weights, int):
+        params = [params]
+        weights = [weights]
+        
+    for param, w in zip(params, weights):
+        mean, var  = param  
+        # introduce a cutoff to avoid nan when var = 0
+        if var == 0: var = 1e-9
+        unimodal = func.pdf(x,
+                            (lower-mean)/np.sqrt(var),
+                            (upper-mean)/np.sqrt(var),
+                            loc = mean,
+                            scale = np.sqrt(var))
+        dist += w*unimodal
+    if normalized:
+        dist /= np.sum(dist)
+    return dist
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 71
+def distribution_distance(p:np.array, # distribution 1
+                          q:np.array # distribution 2
+                         )-> float:  # distance between distributions
+    ''' Calculates mean absolute error between two distributions. '''
+#     return np.sum(np.where(p != 0, p * np.log(p / q), 0))
+    return np.abs(p-q).mean()
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 74
+from .models_phenom import models_phenom
+
+def error_Ensemble_dataset(true_data, pred_data, return_distributions = False):
+    ''' 
+    Calculates the ensemble metrics for the ANDI 2 challenge. The input are matrices of shape:
+    
+    | col1 (state 1) | col2 (state 2) | col3 (state 3) | ... |
+    |:--------------:|:--------------:|:--------------:|:---:|
+    | $\mu_a^1$      | $\mu_a^2$      | $\mu_a^3$      | ... |
+    | $\sigma_a^1$   | $\sigma_a^2$   | $\sigma_a^3$   | ... |
+    | $\mu_D^1$      | $\mu_D^2$      | $\mu_D^3$      | ... |        
+    | $\sigma_D^1$   | $\sigma_D^2$   | $\sigma_D^3$   | ... |
+    | $N_1$          | $N_2$          | $N_3$          | ... |
+    
+    Parameters
+    ----------
+    true_data : array
+        Matrix containing the groundtruth data.
+    pred_data : array
+        Matrix containing the predicted data.
+    return_distributions : bool
+        If True, the function also outputs the generated distributions.
+    
+    Returns
+    -------
+    tuple
+        - distance_alpha: distance between anomalous exponents
+        - distance_D: distance between diffusion coefficients
+        - dists (if asked): distributions of both groundtruth and predicted data.        
+    
+    '''
+    
+    dists = []
+    for data in [true_data, pred_data]:
+        
+        if len(data.shape) > 1: # If we have more than one state
+            alpha_info = np.delete(data, [2,3, -1], 0)
+            d_info = data[2:-1,:]
+            weights = data[-1,:]
+            if weights.sum() > 1: weights /= weights.sum()
+        else: # If single state
+            alpha_info = data[:2]
+            d_info = data[2:-1]
+            weights = 1
+            
+        for idx, (var, bound) in enumerate(zip([alpha_info, d_info], 
+                                               [models_phenom().bound_alpha, models_phenom().bound_D])):
+            if idx == 0: x = np.linspace(bound[0], bound[1], 1000)
+            else: x = np.logspace(np.log10(bound[0]), np.log10(bound[1]), 1000)
+            dists.append(multimode_dist(var.T, weights, bound, x))
+            
+    # Distance between alpha dists
+    distance_alpha = distribution_distance(dists[0], dists[2])
+    distance_D = distribution_distance(dists[1], dists[3])
+    
+    if return_distributions:
+        return distance_alpha, distance_D, dists
+    else:
+        return distance_alpha, distance_D
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 76
+def check_prediction_length(pred):
+    '''
+    Given a trajectory segments prediction, checks whether it has C changepoints and C+1 segments properties values.
+    As it must also contain the index of the trajectory, this is summarized by being multiple of 4. 
+    In some cases, the user needs to also predict the final point of the trajectory. In this case, 
+    we will have a residu of 1.
+    '''
+    if len(pred) % 4 == 0 or len(pred) % 4 == 1 :
+        return True
+    else: 
+        return False
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 77
+def separate_prediction_values(pred):
+    '''
+    Given a prediction over trjaectory segments, extracts the predictions for each segment property
+    as well as the changepoint values.
+    '''        
+    Ds = pred[1::4]
+    alphas = pred[2::4]
+    states = pred[3::4]
+    cp = pred[4::4]    
+    return Ds, alphas, states, cp
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 78
+def load_file_to_df(path_file, 
+                    columns = ['traj_idx', 'Ds', 'alphas', 'states', 'changepoints']):
+    '''
+    Given the path of a .txt file, extract the segmentation predictions based on 
+    the rules of the ANDI 2 challenge022
+    '''
+
+    with open(path_file) as f:
+        lines_pred = f.read().splitlines()
+
+    df = pandas.DataFrame(columns = columns)
+
+    for line in lines_pred:
+        # Extract values with comma separator and transform to float
+        pred_traj = line.split(',')
+        pred = [float(i) for i in pred_traj]
+        
+        # Check that prediction has the correct shape
+        pred_correct = check_prediction_length(pred)
+        
+        # If correct size, then extract parameters and add it to dataframe
+        if pred_correct:
+            preds_D, preds_a, preds_s, preds_cp = separate_prediction_values(pred)
+
+            current_row = df.shape[0]
+            for param, pred_param in zip(columns, [pred[0], preds_D, preds_a, preds_s, preds_cp]):
+                df.loc[current_row, param] = pred_param
+                
+    return df
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 83
+def _get_error_bounds():
+    '''
+    Sets the current maximum errors we can do in the different diffusive properties.
+    '''
+    
+    threshold_error_alpha = 2
+    threshold_error_D = 1e5
+    threshold_error_s = -1
+    threshold_cp = 10
+    return threshold_error_alpha, threshold_error_D, threshold_error_s, threshold_cp
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 84
+def error_SingleTraj_dataset(df_pred, df_true, 
+                              threshold_error_alpha = 2, max_val_alpha = 2, min_val_alpha = 0, 
+                              threshold_error_D = 1e5, max_val_D = 1e6, min_val_D = 1e-6, 
+                              threshold_error_s = -1,
+                              threshold_cp = 10,
+                              prints = True, disable_tqdm = False
+                             ):
+    '''
+    Given two dataframes, corresponding to the predictions and true labels of a set
+    of trajectories from the ANDI 2 challenge022, calculates the corresponding metrics
+    Columns must be for both (no order needed):
+    traj_idx | alphas | Ds | changepoints | states
+    df_true must also contain a column 'T'.
+    
+    Parameters
+    ----------
+    df_pred : dataframe
+        Predictions
+    df_true : dataframe
+        Groundtruth
+    threshold_error_alpha : float
+        (same for D, s, cp) Maximum possible error allowed. If bigger, it is substituted by this error.
+    max_val_alpha : float
+        (same for D, s, cp) Maximum value of the parameter.
+    min_val_alpha : float
+        (same for D, s, cp) Minimum value of the parameter.
+    print : bool
+        If True, prints the results.
+    disable_tqdm : bool
+        If True, disables the progress bar.
+    
+    Returns
+    -------
+    tuple
+        - rmse_CP: root mean squared error change points
+        - JI: Jaccard index change points
+        - error_alpha: mean absolute error anomalous exponents
+        - error_D: mean square log error diffusion coefficients
+        - error_s: Jaccar index diffusive states
+    
+    '''
+    # Initiate counting missing trajectories
+    missing_traj = False
+    
+    # Deleter saving variables, just in case...
+    try: del paired_alpha, paired_D, paired_s
+    except: pass
+
+    # for every trajectory, we stack paired segment properties. We also store changepoints info
+    ensemble_pred_cp, ensemble_true_cp = [], []
+    for t_idx in tqdm(df_true['traj_idx'].values, disable = disable_tqdm):
+        
+        traj_trues = df_true.loc[df_true.traj_idx == t_idx]
+
+        traj_preds = df_pred.loc[df_pred.traj_idx == t_idx]    
+        if traj_preds.shape[0] == 0:
+            # If there is no trajectory, we give maximum error. To do so, we redefine predictions
+            # and trues so that they give maximum error
+            missing_traj += 1                       
+            
+            preds_cp, preds_alpha, preds_D, preds_s = [[10],
+                                                       [0],
+                                                       [1],
+                                                       [0]]
+
+            trues_cp, trues_alpha, trues_D, trues_s = [[10+threshold_cp],
+                                                       [threshold_error_alpha],
+                                                       [1+threshold_error_D],
+                                                       [10]]
+        
+        else:      
+
+            preds_cp, preds_alpha, preds_D, preds_s = [np.array(traj_preds.changepoints.values[0]).astype(int),
+                                                       traj_preds.alphas.values[0],
+                                                       traj_preds.Ds.values[0],
+                                                       traj_preds.states.values[0]]
+
+            trues_cp, trues_alpha, trues_D, trues_s = [np.array(traj_trues.changepoints.values[0]).astype(int),
+                                                       traj_trues.alphas.values[0],
+                                                       traj_trues.Ds.values[0],
+                                                       traj_trues.states.values[0]]
+
+
+        # Collecting changepoints for metric
+        # In this metric, we don't want to enter the final point of the trajectory
+        ensemble_pred_cp.append(preds_cp[:-1])
+        ensemble_true_cp.append(trues_cp[:-1])        
+        
+        # collecting segment properties error after segment assignment
+        pair_a, pair_d, pair_s = segment_property_errors(trues_cp, trues_alpha, trues_D, trues_s, 
+                                                         preds_cp, preds_alpha, preds_D, preds_s,
+                                                         return_pairs = True)
+        
+
+        
+        try:
+            paired_alpha = np.vstack((paired_alpha, pair_a))
+            paired_D = np.vstack((paired_D, pair_d))
+            paired_s = np.vstack((paired_s, pair_s))        
+        except:
+            paired_alpha = pair_a
+            paired_D = pair_d
+            paired_s = pair_s
+               
+    #### Calculate metrics from assembled properties   
+
+    # checking for nans and problems in predictions
+    wrong_alphas = np.argwhere(np.isnan(paired_alpha[:, 1]) | (paired_alpha[:, 1] > 2) | (paired_alpha[:, 1] < 0)).flatten()
+    paired_alpha[wrong_alphas, 1] = paired_alpha[wrong_alphas, 0] + threshold_error_alpha
+
+    wrong_ds = np.argwhere(np.isnan(paired_D[:, 1])).flatten()
+    paired_D = np.abs(paired_D)
+    paired_D[wrong_ds, 1] = paired_D[wrong_ds, 0] + threshold_error_D
+    
+    wrong_s = np.argwhere((paired_s[:, 1] > 4) | (paired_s[:, 1]<0))
+    paired_s[wrong_s, 1] = threshold_error_s    
+    
+    # Changepoints
+    rmse_CP, JI = ensemble_changepoint_error(ensemble_true_cp, ensemble_pred_cp, threshold = threshold_cp)
+
+    # Segment properties
+    error_alpha = metric_anomalous_exponent(paired_alpha[:,0], paired_alpha[:,1])
+    error_D = metric_diffusion_coefficient(paired_D[:,0], paired_D[:,1])
+    error_s = metric_diffusive_state(paired_s[:,0], paired_s[:,1])
+    
+    if prints:        
+        print(f'Summary of metrics assesments:')
+        if missing_traj is not False:            
+            print(f'\n{missing_traj} missing trajectory/ies. ')           
+        if rmse_CP == threshold_cp:
+            print(f'No change points found. RMSE set to max ({threshold_cp})')
+        print(f'\nChangepoint Metrics \nRMSE: {round(rmse_CP, 3)} \nJaccard Index: {round(JI, 3)}',
+              f'\n\nDiffusion property metrics \nMetric anomalous exponent: {error_alpha} \nMetric diffusion coefficient: {error_D} \nMetric diffusive state: {error_s}')
+              
+              
+
+    return rmse_CP, JI, error_alpha, error_D, error_s
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 96
+import re
+import sys
+import os
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 97
+def listdir_nohidden(path):
+    for f in os.listdir(path):
+        if not f.startswith(('.','_')):
+            yield f
+
+# %% ../source_nbs/lib_nbs/utils_challenge.ipynb 98
+def codalab_scoring(input_dir , output_dir):
+    '''
+    Given an input directoy where predictions and groundtruths for the ANDI 2 challenge can be found,
+    calculates metrics and outputs the results in a file in the given output directory.
+    This code is prepared to be run in Codalab.
+    '''
+    
+    # Error bounds
+    threshold_error_alpha, threshold_error_D, threshold_error_s, threshold_cp = _get_error_bounds()
+    
+    ### Saving variables
+    # Track 1 - Videos
+    t1_ens = {'alpha': [],
+              'D': []}
+
+    t1_st = {'RMSE': [],
+             'JI': [],
+             'alpha': [],
+             'D': [],
+             'state': [],
+             'num_traj': [],
+             'num_traj_CP': []} # this last one takes into account no changepoint from single state
+
+    # Track 2 - Trajectories
+    t2_ens = {'alpha': [],
+              'D': []}
+
+    t2_st = {'RMSE': [],
+             'JI': [],
+             'alpha': [],
+             'D': [],
+             'state': [],
+             'num_traj': [],
+             'num_traj_CP': []} # this last one takes into account no changepoint from single state
+    
+    # Handling paths of input files
+    submit_dir = os.path.join(input_dir, 'pred')
+    truth_dir = os.path.join(input_dir, 'true')
+    if not os.path.isdir(submit_dir):
+        print( "%s doesn't exist", truth_dir)
+        
+    # Calculate metrics if directories exist
+    if os.path.isdir(submit_dir) and os.path.isdir(truth_dir):
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+
+        # Extracts all files in reference directory
+        true_files_list = sorted(list(listdir_nohidden(truth_dir)))#os.listdir(truth_dir)
+
+        # Run over all files        
+        missing_tracks = []
+        for filename in tqdm(true_files_list):
+            task = re.search('_(.+?)_labs', filename).group(1)
+            exp = re.search('exp_(.+?)_', filename).group(1)
+            fov = re.search('fov_(.+?).', filename).group(1)
+            # check track and save found tracks
+            track = int(filename[1]) 
+            
+
+            true_file = os.path.join(truth_dir, filename)
+            corresponding_submission_file = os.path.join(submit_dir, filename)
+            
+            if not os.path.isfile(corresponding_submission_file):
+                if track not in missing_tracks:
+                    missing_tracks.append(track)
+                if len(missing_tracks) == 2:
+                    raise FileNotFoundError(f'Failed to find prediction files.')
+                else:
+                    continue
+            
+            # if not os.path.isfile(corresponding_submission_file) and missing_tracks == 1:
+            #     raise FileNotFoundError(f'Failed to find prediction files.')
+                # raise FileNotFoundError(f'Prediction file for: track {track}, task {task}, experiment {exp} and FOV {fov} not found.')
+            
+            # extract model
+            if task == 'ens':
+                model = np.genfromtxt(true_file, dtype='str', skip_footer=5)[1][:-1]
+            else:
+                file_ens = os.path.join(truth_dir, f't{track}_ens_labs_exp_{exp}_fov_{fov}.txt')
+                model = np.genfromtxt(file_ens, dtype='str', skip_footer=5)[1][:-1]
+            
+            # Ensemble
+            if task == 'ens':
+
+                true = np.loadtxt(true_file, skiprows=1, delimiter = ';')
+                pred = np.loadtxt(corresponding_submission_file, skiprows=1, delimiter = ';')
+
+                mae_alpha, mae_D, = error_Ensemble_dataset(true_data = true,
+                                                           pred_data = pred)
+
+                if track == 1:
+                    t1_ens['alpha'].append(mae_alpha)
+                    t1_ens['D'].append(mae_D)
+                if track == 2:                
+                    t2_ens['alpha'].append(mae_alpha)
+                    t2_ens['D'].append(mae_D)
+
+            # Single trajectory
+            if task == 'traj':    
+                df_true = load_file_to_df(true_file)
+                df_pred = load_file_to_df(corresponding_submission_file)
+
+                rmse_CP, JI, error_alpha, error_D, error_s = error_SingleTraj_dataset(df_true = df_true, df_pred = df_pred, 
+                                                                                      threshold_error_alpha = threshold_error_alpha,
+                                                                                      threshold_error_D = threshold_error_D, 
+                                                                                      threshold_error_s = threshold_error_s,
+                                                                                      threshold_cp = threshold_cp,
+                                                                                      prints = False, disable_tqdm = True)
+
+                if track == 1:
+                    # to avoid single state entering in CP metrics
+                    if model != 'single_state': 
+                        t1_st['RMSE'].append(rmse_CP)
+                        t1_st['JI'].append(JI)
+                        t1_st['num_traj_CP'].append(df_true.shape[0])
+                        
+                    t1_st['alpha'].append(error_alpha)
+                    t1_st['D'].append(error_D)
+                    t1_st['state'].append(error_s)                    
+                    t1_st['num_traj'].append(df_true.shape[0])
+                if track == 2:
+                    # to avoid single state entering in CP metrics
+                    if model != 'single_state': 
+                        t2_st['RMSE'].append(rmse_CP)
+                        t2_st['JI'].append(JI)
+                        t2_st['num_traj_CP'].append(df_true.shape[0])
+                    
+                    t2_st['alpha'].append(error_alpha)
+                    t2_st['D'].append(error_D)
+                    t2_st['state'].append(error_s)        
+                    t2_st['num_traj'].append(df_true.shape[0])
+
+            # print(f'Track {track}, Task {task}, Exp {exp}, FOV {fov}: OK!')
+       
+    ### Saving data
+    '''CHECK HOW TO DO THE MEAN!'''    
+    # Define output file
+    output_filename = os.path.join(output_dir, 'scores.txt')
+    output_file = open(output_filename, 'w')
+
+    # Single trajectory data
+    # We define a variable that gives the worst values for each metric. This is applied
+    # separetedly for every FOV
+    worst_value_st = {'RMSE': threshold_cp,
+                      'JI': 0,
+                      'alpha': threshold_error_alpha,
+                      'D': threshold_error_D,
+                      'state': 0}
+    # Run over all keys
+    for key in t1_st: 
+        
+        # Compare results with 
+        if key in ['RMSE', 'alpha', 'D']:            
+            if key == 'RMSE': avg_against = 'num_traj_CP'
+            else: avg_against = 'num_traj'
+            
+            if 1 not in missing_tracks:
+                
+                save_t1 = np.nanmin(np.vstack([t1_st[key],
+                                               np.ones_like(t1_st[key])*worst_value_st[key]]),
+                                    axis = 0)
+                save_t1 = np.average(save_t1, axis = 0, weights = t1_st[avg_against])
+                
+            if 2 not in missing_tracks:                     
+                save_t2 = np.nanmin(np.vstack([t2_st[key],
+                                               np.ones_like(t2_st[key])*worst_value_st[key]]),
+                                    axis = 0)            
+                save_t2 = np.average(save_t2, axis = 0, weights = t2_st[avg_against])
+            
+        elif key in ['JI', 'state']:                        
+            if key == 'JI': avg_against = 'num_traj_CP'
+            else: avg_against = 'num_traj'
+            
+            if 1 not in missing_tracks:
+                save_t1 = np.nanmax(np.vstack([t1_st[key],
+                                               np.ones_like(t1_st[key])*worst_value_st[key]]),
+                                    axis = 0)
+                save_t1 = np.average(save_t1, axis = 0, weights = t1_st[avg_against])
+                    
+            if 2 not in missing_tracks: 
+                save_t2 = np.nanmax(np.vstack([t2_st[key],
+                                               np.ones_like(t2_st[key])*worst_value_st[key]]),
+                                    axis = 0)           
+                save_t2 = np.average(save_t2, axis = 0, weights = t2_st[avg_against])
+
+        if 1 not in missing_tracks: 
+            output_file.write('T1_st_'+ key +f' : {save_t1}\n')    
+        if 2 not in missing_tracks: 
+            output_file.write('T2_st_'+ key +f' : {save_t2}\n')
+
+    ### Saving ensemble data
+    '''WHAT ARE THE THRESHOLDS FOR THIS?'''
+    worst_value_ens = {'alpha': 100,
+                       'D': 100}
+
+    for key in t1_ens: 
+        if key == 'num_traj': continue
+        
+        if 1 not in missing_tracks: 
+            save_t1 = np.nanmin(np.vstack([t1_ens[key],
+                                               np.ones_like(t1_ens[key])*worst_value_ens[key]]),
+                                    axis = 0).mean()
+        if 2 not in missing_tracks: 
+            save_t2 = np.nanmin(np.vstack([t2_ens[key],
+                                               np.ones_like(t2_ens[key])*worst_value_ens[key]]),
+                                    axis = 0).mean()
+
+        if 1 not in missing_tracks: 
+            output_file.write('T1_ens_'+ key +f' : {save_t1}\n')    
+        if 2 not in missing_tracks: 
+            output_file.write('T2_ens_'+ key +f' : {save_t2}\n')
+
+    output_file.close()
```

### Comparing `andi_datasets-2.0.3/andi_datasets/utils_trajectories.py` & `andi_datasets-2.0.4/andi_datasets/utils_trajectories.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,436 +1,436 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/utils_trajectories.ipynb.
-
-# %% auto 0
-__all__ = ['pert', 'gaussian', 'bm1D', 'regularize', 'sample_sphere', 'normalize', 'normalize_fGN', 'trigo', 'find_nan_segments',
-           'segs_inside_fov', 'inside_fov_dataset', 'plot_trajs']
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 2
-import numpy as np    
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 5
-def pert(params:list, # Pert parameters a, b, c
-         size:int = 1, # number of samples to get
-         lamb = 4 # lambda pert parameters
-        )-> np.array: # samples from the given Pert distribution
-    ''' 
-    Samples from a Pert distribution of given parameters
-    '''
-    if isinstance(params, float) or isinstance(params, int):
-        if size == 1:
-            return params
-        else:
-            return np.array(params).repeat(size)
-    
-    a, b, c = params
-    # if all parameters are the same, we consider it a delta distribution
-    if a == b == c:
-        return np.array([a]*size)
-    r = c - a
-    alpha = 1 + lamb * (b - a) / r
-    beta = 1 + lamb * (c - b) / r
-    return a + np.random.beta(alpha, beta, size=size) * r
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 7
-import scipy.stats
-def gaussian(params:list|int, # If list, mu and sigma of the gaussian. If int, we consider sigma = 0
-             size = 1,  # Number of samples to get.
-             bound = None # Bound of the Gaussian, if any.
-            )-> np.array: # Samples from the given Gaussian distribution
-    '''
-    Samples from a Gaussian distribution of given parameters.
-    '''
-    # if we are given a single number, we consider equal to mean and variance = 0
-    if isinstance(params, float) or isinstance(params, int):
-        if size == 1:
-            return params
-        else:
-            return np.array(params).repeat(size)
-    else:
-        mean, var = params        
-        if bound is None:
-            val = np.random.normal(mean, np.sqrt(var), size)
-        if bound is not None:
-            lower, upper = bound
-            if var == 0: 
-                if mean > upper or mean < lower:
-                    raise ValueError('Demanded value outside of range.')
-                val = np.ones(size)*mean
-            else:
-                val = scipy.stats.truncnorm.rvs((lower-mean)/np.sqrt(var),
-                                                (upper-mean)/np.sqrt(var),
-                                                loc = mean,
-                                                scale = np.sqrt(var),
-                                                size = size)
-        if size == 1:
-            return val[0]
-        else:
-            return val
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 11
-def bm1D(T:int, # Length of the trajecgory
-         D:float, # Diffusion coefficient
-         deltaT = False # Sampling time
-        )-> np.array: # Brownian motion trajectory
-    '''Creates a 1D Brownian motion trajectory'''
-    if D < 0:
-        raise ValueError('Only positive diffusion coefficients allowed.') 
-    if not deltaT:               
-        deltaT = 1
-    return np.cumsum(np.sqrt(2*D*deltaT)*np.random.randn(int(T)))        
-     
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 13
-def regularize(positions:np.array, # Positions of the trajectory to regularize
-               times:np.array, # Times at which previous positions were recorded
-               T:int # Length of the output trajectory
-              )->np.array: # Regularized trajectory.
-    '''
-    Regularizes a trajectory with irregular sampling times.
-    ''' 
-    times = np.append(0, times)
-    pos_r = np.zeros(T)
-    for idx in range(len(times)-1):
-        pos_r[int(times[idx]):int(times[idx+1])] = positions[idx]
-    pos_r -= pos_r[0]
-    return pos_r
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 15
-def sample_sphere(N:int, # Number of points to generate.
-                  # Radius of the sphere. If int, all points have
-                  # the same radius, if numpy.array, each number has different radius.
-                  R:int|list, 
-                 )->np.array: # Sampled numbers
-    '''
-    Samples random number that lay in the surface of a 3D sphere centered in 
-    zero and with radius R.
-    '''
-    vecs = np.random.randn(3, N)
-    vecs /= np.linalg.norm(vecs, axis=0)
-    return R*vecs
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 17
-def normalize(trajs):    
-    '''
-    Normalizes trajectories by substracting average and dividing by
-    SQRT of their standard deviation.
-    
-    Parameters
-    ----------
-    trajs : np.array
-        Array of length N x T or just T containing the ensemble or single trajectory to normalize. 
-    '''
-    # Checking and saving initial shape
-    initial_shape = trajs.shape
-    if len(trajs.shape) == 1: # single one d trajectory
-        trajs = trajs.reshape(1, trajs.shape[0], 1)
-    if len(trajs.shape) == 2: # ensemble of one d trajectories
-        trajs = trajs.reshape(trajs.shape[0], trajs.shape[1], 1)
-        
-    trajs = trajs - trajs.mean(axis=1, keepdims=True)
-    displacements = (trajs[:,1:,:] - trajs[:,:-1,:]).copy()    
-    variance = np.std(displacements, axis=1)
-    variance[variance == 0] = 1    
-    new_trajs = np.cumsum((displacements/np.expand_dims(variance, axis = 1)), axis = 1)
-    initial_zeros = np.expand_dims(np.zeros((new_trajs.shape[0], new_trajs.shape[-1])), axis = 1)
-    return np.concatenate((initial_zeros, new_trajs), axis = 1).reshape(initial_shape)
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 18
-def normalize_fGN(disp, alpha, D, T: int, deltaT : int = 1):
-    '''
-    Normalizes fractional Gaussian Noise created with `stochastic` library.
-
-    Parameters
-        ----------
-        disp : Array-like of shape N x T or just T containing the displacements to normalize.
-        alpha : float in [0,2] or array-like of length N x 1
-            Anomalous exponent
-        D : float or array-like of shape N x 1
-            Diffusion coefficient
-        T : int
-            Number of timesteps the displacements were generated with
-        deltaT : int, optional
-            Sampling time
-
-        Returns
-        -------
-            Array-like containing T displacements of given parameters
-    '''
-    return disp*np.sqrt(T)**(alpha)*np.sqrt(2*D*deltaT)
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 22
-import math
-
-class trigo():
-    
-    '''
-    This class gathers multiple useful trigonometric relations.
-    
-    Inspired from:
-    https://stackoverflow.com/questions/30844482/what-is-most-efficient-way-to-find-the-intersection-of-a-line-and-a-circle-in-py 
-    and http://mathworld.wolfram.com/Circle-LineIntersection.html'''
-
-    def circle_line_segment_intersection(circle_center, circle_radius, 
-                                         pt1, pt2, 
-                                         full_line=False, tangent_tol=1e-9):
-        """ 
-        Find the points at which a circle intersects a line-segment. This can happen at 0, 1, or 2 points.
-        
-        Parameters
-        ----------
-        circle_center : tuple
-            The (x, y) location of the circle center
-        circle_radius : float
-            The radius of the circle
-        pt1 : tuple
-            The (x, y) location of the first point of the segment
-        pt2 : tuple
-            The (x, y) location of the second point of the segment
-        full_line : bool
-            True to find intersections along full line - not just in the segment. 
-            False will just return intersections within the segment.
-        tangent_tol : float
-            Numerical tolerance at which we decide the intersections are close enough to consider it a tangent
-        
-        Returns
-        -------
-        Sequence[Tuple[float, float]]
-            A list of length 0, 1, or 2, where each element is a point at which the circle intercepts a line segment.
-
-        """
-
-        (p1x, p1y), (p2x, p2y), (cx, cy) = pt1, pt2, circle_center
-        (x1, y1), (x2, y2) = (p1x - cx, p1y - cy), (p2x - cx, p2y - cy)
-        dx, dy = (x2 - x1), (y2 - y1)
-        dr = (dx ** 2 + dy ** 2)**.5
-        big_d = x1 * y2 - x2 * y1
-        discriminant = circle_radius ** 2 * dr ** 2 - big_d ** 2
-
-        if discriminant < 0:  # No intersection between circle and line
-            return []
-        else:  # There may be 0, 1, or 2 intersections with the segment
-            intersections = [
-                (cx + (big_d * dy + sign * (-1 if dy < 0 else 1) * dx * discriminant**.5) / dr ** 2,
-                 cy + (-big_d * dx + sign * abs(dy) * discriminant**.5) / dr ** 2)
-                for sign in ((1, -1) if dy < 0 else (-1, 1))]  # This makes sure the order along the segment is correct
-            if not full_line:  # If only considering the segment, filter out intersections that do not fall within the segment
-                fraction_along_segment = [(xi - p1x) / dx if abs(dx) > abs(dy) else (yi - p1y) / dy for xi, yi in intersections]
-                intersections = [pt for pt, frac in zip(intersections, fraction_along_segment) if 0 <= frac <= 1]
-            if len(intersections) == 2 and abs(discriminant) <= tangent_tol:  # If line is tangent to circle, return just one point (as both intersections have same location)
-                return [intersections[0]]
-            else:
-                return intersections
-            
-    def seg_to_vec(seg):
-        ''' Find the vector given a segment created by two 2D points'''
-        return [(seg[0][0]-seg[1][0]), (seg[0][1]-seg[1][1])]
-
-    def ang_line(lineA, lineB):
-        ''' Calculates the angle between two lines/segments'''
-        # Get vector form
-        vA = trigo.seg_to_vec(lineA)
-        vB = trigo.seg_to_vec(lineB)
-        return trigo.ang_vec(vA, vB)
-
-    def ang_vec(vA, vB):
-        ''' Calculates the angle between two vectors'''
-        # Get dot prod
-        dot_prod = np.dot(vA, vB)
-        # Get magnitudes
-        magA = np.dot(vA, vA)**0.5
-        magB = np.dot(vB, vB)**0.5
-        # Get cosine value
-        cos_ = dot_prod/magA/magB
-        # Get angle in radians and then convert to degrees
-        return math.acos(dot_prod/magB/magA)    
-    
-    def rotate_vec(vec, angle):
-        return (vec[0]*np.cos(angle) + vec[1]*np.sin(angle), -vec[0]*np.sin(angle) + vec[1]*np.cos(angle))
-    
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 25
-def find_nan_segments(a, cutoff_length):    
-    ''' Extract all segments of nans bigger than the set cutoff_length. If no segments are found, returns None. 
-    For each segments, returns the begining and end index of it.
-    
-    Output: array of size (number of segments) x 2.
-    '''
-    mask = np.concatenate(([False],np.isnan(a),[False]))
-    if ~mask.any():
-        return None
-    else:
-        idx = np.nonzero(mask[1:] != mask[:-1])[0]
-        seg_length = (idx[1::2] - idx[::2])
-        idx_seg_long = np.argwhere(seg_length >= cutoff_length).flatten()
-        if idx_seg_long.shape[0] == 0: 
-            return None
-        else:
-            return np.array([idx[::2][idx_seg_long], idx[1::2][idx_seg_long]]).transpose()
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 26
-def segs_inside_fov(traj, fov_origin, fov_length, cutoff_length):
-    ''' 
-    Given a trajectory, finds the segments inside the field of view (FOV).
-    
-    Parameters
-    ----------
-    traj : array
-        Set of trajectories of size N x T (N: number trajectories, T: length).
-    fov_origin : tuple
-        Bottom right point of the square defining the FOV.
-    fov_length : float
-        Size of the box defining the FOV.
-    cutoff_length : float
-        Minimum length of a trajectory inside the FOV to be considered in the output dataset.
-    
-    Returns
-    -------
-    array
-         Set of segments inside the FOV.
-    '''
-    
-    import warnings
-    warnings.filterwarnings('ignore') # nanmin gives an undesired warning..
-    
-    fov_min_x, fov_min_y = fov_origin
-    fov_max_x, fov_max_y = np.array(fov_origin)+fov_length
-        
-    # extract components
-    x, y = traj[:, 0].copy(), traj[:, 1].copy()
-    
-    
-    # Interior points to the FOV are set to nans
-    x[np.argwhere((x > fov_min_x) & (x < fov_max_x))] = np.nan
-    y[np.argwhere((y > fov_min_y) & (y < fov_max_y))] = np.nan
-
-    # Compare the minimums of each array. This way, if at least one dimension
-    # is outside (i.e. not nan), the whole segment will be considered outside
-    merge_dims = np.nanmin(np.vstack((x, y)), axis = 0)
-    
-    # Find nan segments bigger than cutoff_length
-    nan_segms = find_nan_segments(merge_dims, cutoff_length = cutoff_length)
-    
-    return nan_segms
-    
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 27
-def inside_fov_dataset(trajs, labels, 
-                       fov_origin, fov_length, 
-                       cutoff_length = 10, 
-                       func_labels = None,
-                       return_frames = False):
-    ''' Given a dataset of trajectories with labels and a FOV parameters, returns a list of
-        trajectories with the corresponding labels inside the FOV
-    
-    Parameters
-    ----------
-    trajs : array
-        Set of trajectories with shape T x N x 2.
-    labels : array
-        Set of labels with shape T x N x 2.
-    fov_origin : tuple
-        Bottom left point of the square defining the FOV.
-    fov_length : float
-        Size of the box defining the FOV.
-    cutoff_length : float
-        Minimum length of a trajectory inside the FOV to be considered in the output dataset.
-    func_labels : func
-        (optional) Function to be applied to the labels to take advantage of the loop.
-    
-    Returns
-    -------
-    tuple
-        - trajs_fov (list): list 2D arrays containing the trajectories inside the field of view.
-        - labels_fov (list): corresponding labels of the trajectories.
-    '''
-    
-    trajs_fov, labels_fov = [], []
-    frames = np.arange(trajs.shape[0])
-    for idx, (traj, label) in enumerate(zip(trajs[:, :, :].transpose(1,0,2),
-                                            labels[:, :, :].transpose(1,0,2))):
-        nan_segms = segs_inside_fov(traj, fov_origin, fov_length, cutoff_length)
-    
-        if nan_segms is not None:
-            for idx_nan in nan_segms:  
-                
-                traj_x = traj[idx_nan[0]:idx_nan[1], 0]
-                traj_y = traj[idx_nan[0]:idx_nan[1], 1]
-                if return_frames:
-                    frames_cut = frames[idx_nan[0]:idx_nan[1]]
-                    trajs_fov.append(np.vstack((frames_cut, traj_x, traj_y)))
-                else:
-                    trajs_fov.append(np.vstack((traj_x, traj_y)))
-                
-                
-                lab_list = []
-                for idx_lab in range(label.shape[-1]):
-                    if func_labels is not None: # If feeded, apply func_label (mostly for smoothing)
-                        lab = func_labels(label[idx_nan[0]:idx_nan[1], idx_lab])
-                    else:
-                        lab = label[idx_nan[0]:idx_nan[1], idx_lab]
-                    lab_list.append(lab)        
-                    
-                labels_fov.append(np.vstack(lab_list))
-                
-    return trajs_fov, labels_fov
-            
-    
-    
-
-# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 33
-import matplotlib.pyplot as plt
-
-def plot_trajs(trajs, L , N, 
-               num_to_plot = 3,
-               labels = None,
-               plot_labels = False,
-               traps_positions = None,
-               comp_center = None, r_cercle = None
-              ):
-    
-    if plot_labels:
-        fig, axs = plt.subplots(3, num_to_plot, figsize = (num_to_plot*3, 3*3), tight_layout = True)
-    else:
-        fig, axs = plt.subplots(2, num_to_plot, figsize = (num_to_plot*3, 2*3), tight_layout = True)
-
-    for ax in axs.transpose():
-        
-        if traps_positions is not None:
-            ax[0].scatter(traps_positions[:,0], traps_positions[:,1], c = 'C1')
-            
-        if comp_center is not None:
-            for c in comp_center:
-                circle = plt.Circle((c[0], c[1]), r_cercle, facecolor = 'None', edgecolor = 'C1', zorder = 10)
-                ax[0].add_patch(circle) 
-
-        
-        part = np.random.randint(N)    
-        ax[0].set_title(f'Particle # {part}')
-        ax[0].plot(trajs[:, part, 0], trajs[:, part, 1], alpha = 0.8)
-        ax[0].axhline(L, ls = '--', alpha = 0.3, c = 'k', label = 'Boundary')
-        ax[0].axhline(0, ls = '--', alpha = 0.3, c = 'k')
-        ax[0].axvline(L, ls = '--', alpha = 0.3, c = 'k')
-        ax[0].axvline(0, ls = '--', alpha = 0.3, c = 'k')
-
-        ax[1].plot(trajs[:, part, 0], 'o-', label = 'X', ms = 3, lw = 0.1)
-        ax[1].plot(trajs[:, part, 1], 'o-', label = 'Y', ms = 3, lw = 0.1)
-        ax[1].axhline(L, ls = '--', alpha = 0.3, c = 'k')
-        ax[1].axhline(0, ls = '--', alpha = 0.3, c = 'k')
-        
-        if plot_labels:
-            ax[2].plot(labels[:, part, 0], 'o-', label = r'$\alpha$', ms = 3, lw = 0.1)
-            ax[2].plot(labels[:, part, 1], 'o-', label = r'$D$', ms = 3, lw = 0.1)
-
-
-    plt.setp(axs[0, :], xlabel = 'X', ylabel = 'Y')
-    axs[0, 0].legend()
-    axs[1, 0].legend()
-    plt.setp(axs[1, 0], ylabel = 'Position')
-    plt.setp(axs[1:-1, :], xticklabels = '')
-   
-    if plot_labels:
-        axs[2, 0].legend()
-        plt.setp(axs[2, 0], ylabel = 'Labels')
-        plt.setp(axs[2, :], xlabel = 'Time');
-    else:
-        plt.setp(axs[1, :], xlabel = 'Time');
-        
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/utils_trajectories.ipynb.
+
+# %% auto 0
+__all__ = ['pert', 'gaussian', 'bm1D', 'regularize', 'sample_sphere', 'normalize', 'normalize_fGN', 'trigo', 'find_nan_segments',
+           'segs_inside_fov', 'inside_fov_dataset', 'plot_trajs']
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 2
+import numpy as np    
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 5
+def pert(params:list, # Pert parameters a, b, c
+         size:int = 1, # number of samples to get
+         lamb = 4 # lambda pert parameters
+        )-> np.array: # samples from the given Pert distribution
+    ''' 
+    Samples from a Pert distribution of given parameters
+    '''
+    if isinstance(params, float) or isinstance(params, int):
+        if size == 1:
+            return params
+        else:
+            return np.array(params).repeat(size)
+    
+    a, b, c = params
+    # if all parameters are the same, we consider it a delta distribution
+    if a == b == c:
+        return np.array([a]*size)
+    r = c - a
+    alpha = 1 + lamb * (b - a) / r
+    beta = 1 + lamb * (c - b) / r
+    return a + np.random.beta(alpha, beta, size=size) * r
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 7
+import scipy.stats
+def gaussian(params:list|int, # If list, mu and sigma of the gaussian. If int, we consider sigma = 0
+             size = 1,  # Number of samples to get.
+             bound = None # Bound of the Gaussian, if any.
+            )-> np.array: # Samples from the given Gaussian distribution
+    '''
+    Samples from a Gaussian distribution of given parameters.
+    '''
+    # if we are given a single number, we consider equal to mean and variance = 0
+    if isinstance(params, float) or isinstance(params, int):
+        if size == 1:
+            return params
+        else:
+            return np.array(params).repeat(size)
+    else:
+        mean, var = params        
+        if bound is None:
+            val = np.random.normal(mean, np.sqrt(var), size)
+        if bound is not None:
+            lower, upper = bound
+            if var == 0: 
+                if mean > upper or mean < lower:
+                    raise ValueError('Demanded value outside of range.')
+                val = np.ones(size)*mean
+            else:
+                val = scipy.stats.truncnorm.rvs((lower-mean)/np.sqrt(var),
+                                                (upper-mean)/np.sqrt(var),
+                                                loc = mean,
+                                                scale = np.sqrt(var),
+                                                size = size)
+        if size == 1:
+            return val[0]
+        else:
+            return val
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 11
+def bm1D(T:int, # Length of the trajecgory
+         D:float, # Diffusion coefficient
+         deltaT = False # Sampling time
+        )-> np.array: # Brownian motion trajectory
+    '''Creates a 1D Brownian motion trajectory'''
+    if D < 0:
+        raise ValueError('Only positive diffusion coefficients allowed.') 
+    if not deltaT:               
+        deltaT = 1
+    return np.cumsum(np.sqrt(2*D*deltaT)*np.random.randn(int(T)))        
+     
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 13
+def regularize(positions:np.array, # Positions of the trajectory to regularize
+               times:np.array, # Times at which previous positions were recorded
+               T:int # Length of the output trajectory
+              )->np.array: # Regularized trajectory.
+    '''
+    Regularizes a trajectory with irregular sampling times.
+    ''' 
+    times = np.append(0, times)
+    pos_r = np.zeros(T)
+    for idx in range(len(times)-1):
+        pos_r[int(times[idx]):int(times[idx+1])] = positions[idx]
+    pos_r -= pos_r[0]
+    return pos_r
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 15
+def sample_sphere(N:int, # Number of points to generate.
+                  # Radius of the sphere. If int, all points have
+                  # the same radius, if numpy.array, each number has different radius.
+                  R:int|list, 
+                 )->np.array: # Sampled numbers
+    '''
+    Samples random number that lay in the surface of a 3D sphere centered in 
+    zero and with radius R.
+    '''
+    vecs = np.random.randn(3, N)
+    vecs /= np.linalg.norm(vecs, axis=0)
+    return R*vecs
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 17
+def normalize(trajs):    
+    '''
+    Normalizes trajectories by substracting average and dividing by
+    SQRT of their standard deviation.
+    
+    Parameters
+    ----------
+    trajs : np.array
+        Array of length N x T or just T containing the ensemble or single trajectory to normalize. 
+    '''
+    # Checking and saving initial shape
+    initial_shape = trajs.shape
+    if len(trajs.shape) == 1: # single one d trajectory
+        trajs = trajs.reshape(1, trajs.shape[0], 1)
+    if len(trajs.shape) == 2: # ensemble of one d trajectories
+        trajs = trajs.reshape(trajs.shape[0], trajs.shape[1], 1)
+        
+    trajs = trajs - trajs.mean(axis=1, keepdims=True)
+    displacements = (trajs[:,1:,:] - trajs[:,:-1,:]).copy()    
+    variance = np.std(displacements, axis=1)
+    variance[variance == 0] = 1    
+    new_trajs = np.cumsum((displacements/np.expand_dims(variance, axis = 1)), axis = 1)
+    initial_zeros = np.expand_dims(np.zeros((new_trajs.shape[0], new_trajs.shape[-1])), axis = 1)
+    return np.concatenate((initial_zeros, new_trajs), axis = 1).reshape(initial_shape)
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 18
+def normalize_fGN(disp, alpha, D, T: int, deltaT : int = 1):
+    '''
+    Normalizes fractional Gaussian Noise created with `stochastic` library.
+
+    Parameters
+        ----------
+        disp : Array-like of shape N x T or just T containing the displacements to normalize.
+        alpha : float in [0,2] or array-like of length N x 1
+            Anomalous exponent
+        D : float or array-like of shape N x 1
+            Diffusion coefficient
+        T : int
+            Number of timesteps the displacements were generated with
+        deltaT : int, optional
+            Sampling time
+
+        Returns
+        -------
+            Array-like containing T displacements of given parameters
+    '''
+    return disp*np.sqrt(T)**(alpha)*np.sqrt(2*D*deltaT)
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 22
+import math
+
+class trigo():
+    
+    '''
+    This class gathers multiple useful trigonometric relations.
+    
+    Inspired from:
+    https://stackoverflow.com/questions/30844482/what-is-most-efficient-way-to-find-the-intersection-of-a-line-and-a-circle-in-py 
+    and http://mathworld.wolfram.com/Circle-LineIntersection.html'''
+
+    def circle_line_segment_intersection(circle_center, circle_radius, 
+                                         pt1, pt2, 
+                                         full_line=False, tangent_tol=1e-9):
+        """ 
+        Find the points at which a circle intersects a line-segment. This can happen at 0, 1, or 2 points.
+        
+        Parameters
+        ----------
+        circle_center : tuple
+            The (x, y) location of the circle center
+        circle_radius : float
+            The radius of the circle
+        pt1 : tuple
+            The (x, y) location of the first point of the segment
+        pt2 : tuple
+            The (x, y) location of the second point of the segment
+        full_line : bool
+            True to find intersections along full line - not just in the segment. 
+            False will just return intersections within the segment.
+        tangent_tol : float
+            Numerical tolerance at which we decide the intersections are close enough to consider it a tangent
+        
+        Returns
+        -------
+        Sequence[Tuple[float, float]]
+            A list of length 0, 1, or 2, where each element is a point at which the circle intercepts a line segment.
+
+        """
+
+        (p1x, p1y), (p2x, p2y), (cx, cy) = pt1, pt2, circle_center
+        (x1, y1), (x2, y2) = (p1x - cx, p1y - cy), (p2x - cx, p2y - cy)
+        dx, dy = (x2 - x1), (y2 - y1)
+        dr = (dx ** 2 + dy ** 2)**.5
+        big_d = x1 * y2 - x2 * y1
+        discriminant = circle_radius ** 2 * dr ** 2 - big_d ** 2
+
+        if discriminant < 0:  # No intersection between circle and line
+            return []
+        else:  # There may be 0, 1, or 2 intersections with the segment
+            intersections = [
+                (cx + (big_d * dy + sign * (-1 if dy < 0 else 1) * dx * discriminant**.5) / dr ** 2,
+                 cy + (-big_d * dx + sign * abs(dy) * discriminant**.5) / dr ** 2)
+                for sign in ((1, -1) if dy < 0 else (-1, 1))]  # This makes sure the order along the segment is correct
+            if not full_line:  # If only considering the segment, filter out intersections that do not fall within the segment
+                fraction_along_segment = [(xi - p1x) / dx if abs(dx) > abs(dy) else (yi - p1y) / dy for xi, yi in intersections]
+                intersections = [pt for pt, frac in zip(intersections, fraction_along_segment) if 0 <= frac <= 1]
+            if len(intersections) == 2 and abs(discriminant) <= tangent_tol:  # If line is tangent to circle, return just one point (as both intersections have same location)
+                return [intersections[0]]
+            else:
+                return intersections
+            
+    def seg_to_vec(seg):
+        ''' Find the vector given a segment created by two 2D points'''
+        return [(seg[0][0]-seg[1][0]), (seg[0][1]-seg[1][1])]
+
+    def ang_line(lineA, lineB):
+        ''' Calculates the angle between two lines/segments'''
+        # Get vector form
+        vA = trigo.seg_to_vec(lineA)
+        vB = trigo.seg_to_vec(lineB)
+        return trigo.ang_vec(vA, vB)
+
+    def ang_vec(vA, vB):
+        ''' Calculates the angle between two vectors'''
+        # Get dot prod
+        dot_prod = np.dot(vA, vB)
+        # Get magnitudes
+        magA = np.dot(vA, vA)**0.5
+        magB = np.dot(vB, vB)**0.5
+        # Get cosine value
+        cos_ = dot_prod/magA/magB
+        # Get angle in radians and then convert to degrees
+        return math.acos(dot_prod/magB/magA)    
+    
+    def rotate_vec(vec, angle):
+        return (vec[0]*np.cos(angle) + vec[1]*np.sin(angle), -vec[0]*np.sin(angle) + vec[1]*np.cos(angle))
+    
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 25
+def find_nan_segments(a, cutoff_length):    
+    ''' Extract all segments of nans bigger than the set cutoff_length. If no segments are found, returns None. 
+    For each segments, returns the begining and end index of it.
+    
+    Output: array of size (number of segments) x 2.
+    '''
+    mask = np.concatenate(([False],np.isnan(a),[False]))
+    if ~mask.any():
+        return None
+    else:
+        idx = np.nonzero(mask[1:] != mask[:-1])[0]
+        seg_length = (idx[1::2] - idx[::2])
+        idx_seg_long = np.argwhere(seg_length >= cutoff_length).flatten()
+        if idx_seg_long.shape[0] == 0: 
+            return None
+        else:
+            return np.array([idx[::2][idx_seg_long], idx[1::2][idx_seg_long]]).transpose()
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 26
+def segs_inside_fov(traj, fov_origin, fov_length, cutoff_length):
+    ''' 
+    Given a trajectory, finds the segments inside the field of view (FOV).
+    
+    Parameters
+    ----------
+    traj : array
+        Set of trajectories of size N x T (N: number trajectories, T: length).
+    fov_origin : tuple
+        Bottom right point of the square defining the FOV.
+    fov_length : float
+        Size of the box defining the FOV.
+    cutoff_length : float
+        Minimum length of a trajectory inside the FOV to be considered in the output dataset.
+    
+    Returns
+    -------
+    array
+         Set of segments inside the FOV.
+    '''
+    
+    import warnings
+    warnings.filterwarnings('ignore') # nanmin gives an undesired warning..
+    
+    fov_min_x, fov_min_y = fov_origin
+    fov_max_x, fov_max_y = np.array(fov_origin)+fov_length
+        
+    # extract components
+    x, y = traj[:, 0].copy(), traj[:, 1].copy()
+    
+    
+    # Interior points to the FOV are set to nans
+    x[np.argwhere((x > fov_min_x) & (x < fov_max_x))] = np.nan
+    y[np.argwhere((y > fov_min_y) & (y < fov_max_y))] = np.nan
+
+    # Compare the minimums of each array. This way, if at least one dimension
+    # is outside (i.e. not nan), the whole segment will be considered outside
+    merge_dims = np.nanmin(np.vstack((x, y)), axis = 0)
+    
+    # Find nan segments bigger than cutoff_length
+    nan_segms = find_nan_segments(merge_dims, cutoff_length = cutoff_length)
+    
+    return nan_segms
+    
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 27
+def inside_fov_dataset(trajs, labels, 
+                       fov_origin, fov_length, 
+                       cutoff_length = 10, 
+                       func_labels = None,
+                       return_frames = False):
+    ''' Given a dataset of trajectories with labels and a FOV parameters, returns a list of
+        trajectories with the corresponding labels inside the FOV
+    
+    Parameters
+    ----------
+    trajs : array
+        Set of trajectories with shape T x N x 2.
+    labels : array
+        Set of labels with shape T x N x 2.
+    fov_origin : tuple
+        Bottom left point of the square defining the FOV.
+    fov_length : float
+        Size of the box defining the FOV.
+    cutoff_length : float
+        Minimum length of a trajectory inside the FOV to be considered in the output dataset.
+    func_labels : func
+        (optional) Function to be applied to the labels to take advantage of the loop.
+    
+    Returns
+    -------
+    tuple
+        - trajs_fov (list): list 2D arrays containing the trajectories inside the field of view.
+        - labels_fov (list): corresponding labels of the trajectories.
+    '''
+    
+    trajs_fov, labels_fov = [], []
+    frames = np.arange(trajs.shape[0])
+    for idx, (traj, label) in enumerate(zip(trajs[:, :, :].transpose(1,0,2),
+                                            labels[:, :, :].transpose(1,0,2))):
+        nan_segms = segs_inside_fov(traj, fov_origin, fov_length, cutoff_length)
+    
+        if nan_segms is not None:
+            for idx_nan in nan_segms:  
+                
+                traj_x = traj[idx_nan[0]:idx_nan[1], 0]
+                traj_y = traj[idx_nan[0]:idx_nan[1], 1]
+                if return_frames:
+                    frames_cut = frames[idx_nan[0]:idx_nan[1]]
+                    trajs_fov.append(np.vstack((frames_cut, traj_x, traj_y)))
+                else:
+                    trajs_fov.append(np.vstack((traj_x, traj_y)))
+                
+                
+                lab_list = []
+                for idx_lab in range(label.shape[-1]):
+                    if func_labels is not None: # If feeded, apply func_label (mostly for smoothing)
+                        lab = func_labels(label[idx_nan[0]:idx_nan[1], idx_lab])
+                    else:
+                        lab = label[idx_nan[0]:idx_nan[1], idx_lab]
+                    lab_list.append(lab)        
+                    
+                labels_fov.append(np.vstack(lab_list))
+                
+    return trajs_fov, labels_fov
+            
+    
+    
+
+# %% ../source_nbs/lib_nbs/utils_trajectories.ipynb 33
+import matplotlib.pyplot as plt
+
+def plot_trajs(trajs, L , N, 
+               num_to_plot = 3,
+               labels = None,
+               plot_labels = False,
+               traps_positions = None,
+               comp_center = None, r_cercle = None
+              ):
+    
+    if plot_labels:
+        fig, axs = plt.subplots(3, num_to_plot, figsize = (num_to_plot*3, 3*3), tight_layout = True)
+    else:
+        fig, axs = plt.subplots(2, num_to_plot, figsize = (num_to_plot*3, 2*3), tight_layout = True)
+
+    for ax in axs.transpose():
+        
+        if traps_positions is not None:
+            ax[0].scatter(traps_positions[:,0], traps_positions[:,1], c = 'C1')
+            
+        if comp_center is not None:
+            for c in comp_center:
+                circle = plt.Circle((c[0], c[1]), r_cercle, facecolor = 'None', edgecolor = 'C1', zorder = 10)
+                ax[0].add_patch(circle) 
+
+        
+        part = np.random.randint(N)    
+        ax[0].set_title(f'Particle # {part}')
+        ax[0].plot(trajs[:, part, 0], trajs[:, part, 1], alpha = 0.8)
+        ax[0].axhline(L, ls = '--', alpha = 0.3, c = 'k', label = 'Boundary')
+        ax[0].axhline(0, ls = '--', alpha = 0.3, c = 'k')
+        ax[0].axvline(L, ls = '--', alpha = 0.3, c = 'k')
+        ax[0].axvline(0, ls = '--', alpha = 0.3, c = 'k')
+
+        ax[1].plot(trajs[:, part, 0], 'o-', label = 'X', ms = 3, lw = 0.1)
+        ax[1].plot(trajs[:, part, 1], 'o-', label = 'Y', ms = 3, lw = 0.1)
+        ax[1].axhline(L, ls = '--', alpha = 0.3, c = 'k')
+        ax[1].axhline(0, ls = '--', alpha = 0.3, c = 'k')
+        
+        if plot_labels:
+            ax[2].plot(labels[:, part, 0], 'o-', label = r'$\alpha$', ms = 3, lw = 0.1)
+            ax[2].plot(labels[:, part, 1], 'o-', label = r'$D$', ms = 3, lw = 0.1)
+
+
+    plt.setp(axs[0, :], xlabel = 'X', ylabel = 'Y')
+    axs[0, 0].legend()
+    axs[1, 0].legend()
+    plt.setp(axs[1, 0], ylabel = 'Position')
+    plt.setp(axs[1:-1, :], xticklabels = '')
+   
+    if plot_labels:
+        axs[2, 0].legend()
+        plt.setp(axs[2, 0], ylabel = 'Labels')
+        plt.setp(axs[2, :], xlabel = 'Time');
+    else:
+        plt.setp(axs[1, :], xlabel = 'Time');
+
```

### Comparing `andi_datasets-2.0.3/andi_datasets/utils_videos.py` & `andi_datasets-2.0.4/andi_datasets/utils_videos.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/utils_videos.ipynb.
-
-# %% auto 0
-__all__ = ['play_video', 'convert_uint8', 'psf_width', 'func_poisson_noise', 'mask', 'transform_to_video']
-
-# %% ../source_nbs/lib_nbs/utils_videos.ipynb 2
-import matplotlib.animation as animation
-import matplotlib.pyplot as plt
-from IPython.display import HTML
-import numpy as np
-import imageio
-
-# Deeptrack is not automatically installed in andi_datasets
-# due to its load. 
-import warnings
-try:
-    import deeptrack as dt
-except:
-    warnings.warn('Deeptrack is currently not installed. Install if needed using pip install deeptrack.')
-
-# %% ../source_nbs/lib_nbs/utils_videos.ipynb 4
-def play_video(video, figsize=(5, 5), fps=10):
-    """
-    Displays a stack of images as a video inside jupyter notebooks.
-
-    Parameters
-    ----------
-    video : ndarray
-        Stack of images.
-    figsize : tuple, optional
-        Canvas size of the video.
-    fps : int, optional
-        Video frame rate.
-
-    Returns
-    -------
-    Video object
-        Returns a video player with input stack of images.
-    """
-    fig = plt.figure(figsize=figsize)
-    images = []
-    plt.axis("off")
-
-    for image in video:
-        images.append([plt.imshow(image[:, :, 0], cmap="gray")])
-
-    anim = animation.ArtistAnimation(
-        fig, images, interval=1e3 / fps, blit=True, repeat_delay=0
-    )
-
-    html = HTML(anim.to_jshtml())
-    display(html)
-    plt.close()
-
-# %% ../source_nbs/lib_nbs/utils_videos.ipynb 5
-def convert_uint8(vid, with_vips = False):
-    """
-    Converts a stack of images in to 8bit pixel format.
-    
-    This is a helper function for  `transform_to_video`
-
-    Parameters
-    ----------
-    vid : ndarray
-        Stack of images.
-    with_vips: bool, optional
-        Appends a mask of vip particles in the first frame to the converted video.
-    
-    Returns
-    -------
-    ndarray
-        Image stack in 8bit.
-    """
-    new_vid = []
-    for idx_im, im in enumerate(vid):
-        if idx_im == 0 and with_vips:
-            im[im == -1] = 255
-            new_vid.append(im.astype(np.uint8))
-        else:            
-            im = im[:,:,0]
-            im = im / im.max()
-            im = im * 255
-            im = im.astype(np.uint8)
-            new_vid.append(im)
-    return new_vid
-
-# %% ../source_nbs/lib_nbs/utils_videos.ipynb 6
-def psf_width(NA = 1.46, wavelength = 500e-9, resolution = 100e-9):
-    """
-    Computes the PSF width.
-
-    This is a helper function for `transform_to_video`
-    
-    Parameters
-    ----------
-    NA : float
-        Numerical aperture.
-    wavelength : float
-        Wavelength.
-    resolution : float
-        Resolution of the camera.
-    
-    Returns
-    -------
-    int
-        PSF width in pixels.
-    """
-    _psf = 1.22 * wavelength / (2 * NA)
-    return int(_psf / resolution)
-
-# %% ../source_nbs/lib_nbs/utils_videos.ipynb 7
-def func_poisson_noise():
-    """
-    Applies poisson noise to an image.
-
-    This is a custom DeepTrack feature, and a helper function for `transform_to_video`
-    """
-    def inner(image):
-        image[image<0] = 0
-        rescale = 1
-        noisy_image = np.random.poisson(image * rescale) / rescale
-        return noisy_image
-    return inner
-
-# %% ../source_nbs/lib_nbs/utils_videos.ipynb 8
-def mask(circle_radius, particle_list=[]):
-    """
-    Computes binary masks for particles in microscopy videos.
-
-    This is a custom DeepTrack feature, and a helper function for `transform_to_video`.
-
-    Parameters
-    ----------
-    particle_list: list of int
-        List of particles whose masks need to be created
-
-    """
-    def inner(image):
-        X, Y = np.mgrid[:2*circle_radius, :2*circle_radius]
-        CIRCLE = (X - circle_radius+0.5)**2 + (Y- circle_radius+0.5)**2 < circle_radius**2
-        CIRCLE = np.expand_dims(CIRCLE, axis=-1)
-        _index = image.get_property("replicate_index")[0]
-        if particle_list:
-            if _index in particle_list:
-                pix_val = (_index + 1) * CIRCLE
-            else:
-                pix_val = 0 * CIRCLE
-        else:
-            pix_val = (_index + 1) * CIRCLE
-        return pix_val
-    return inner
-
-# %% ../source_nbs/lib_nbs/utils_videos.ipynb 10
-def transform_to_video(
-    trajectory_data,
-    particle_props={},
-    optics_props={},
-    background_props={},
-    get_vip_particles=[],
-    with_masks=False,
-    save_video=False,
-    path="",
-):
-    """
-    Transforms trajectory data into microscopy imagery data.
-
-    Trajectories generated through phenomenological models in andi-datasets are imaged under a Fluorescence microscope to generate 2D timelapse videos.
-
-    Parameters
-    ----------
-    trajectory_data : ndarray
-        Generated through models_phenom. Array of the shape (T, N, 2) containing the trajectories.
-    particle_props : dict
-        Dictionary containing the properties of particles to be simulated as keyword arguments. Valid keys are:
-
-            '`particle_intensity`' : array_like[int, int]
-                Intensity distribution of particles within a frame given as mean and standard deviations.
-
-            '`intensity_variation`' : int
-                Intensity variation of particles in subsequent frames given as standard deviation.
-
-            '`z`' : float
-                Particle positions with respect to the focal plane in pixel units defined by the pixel size in **optics_props**. For example, particles will be at focus when `z=0`.
-
-            '`refractive_index`' : float
-                Refractive index of particle.
-
-    optics_props : dict
-        Dictionary containing the properties of microscope as keyword arguments. Valid keys are:
-
-            '`NA`': float
-                Numerical aperture of the microscope.
-
-            '`wavelength`' : float
-                Wavelength of light in meters.
-
-            '`resolution`' : float
-                Effective pixel size of the camera in meters.
-
-            '`magnification`' : float
-                Magnification of the optical system.
-
-            '`refractive_index_medium`' : float
-                Refractive index of the medium sorrounding the particles.
-
-            '`output_region`': array_like[int, int, int, int]
-                ROI of the image to output.
-                Given in the format : [x, y, x + width, y + height].
-
-    background_props : dict
-        Dictionary containing properties related to background intensity as keyword arguments. Valid keys are:
-
-            '`background_mean`' : int
-                Mean background intensity.
-
-            '`backgound_std`' : int
-                Standard deviation of the background intesity with subsequent frames of a video.
-
-    get_vip_particles : list of int
-        List of particles for which the masks are needed in the output.
-
-    with_masks : bool
-        If True, particle masks are returned in the output along with the video.
-        If False (default), only the video is returned in the output.
-
-    save_video : bool
-        If True, the generated video will be saved at the given path.
-    path : str
-        File path for saving the video, the path should be given along the video format.
-        For example: 'path' = './video.mp4' will save the video in the current folder.
-
-    Returns
-    -------
-    tuple | ndarray
-
-        Output type I 
-
-        If `with_masks = True`,
-        The function returns a tuple containing:
-            masks : ndarray
-            video : ndarray
-        Note: If `get_vip_particles` is a non-empty list, the masks will contain only the vip particle masks.
-
-        Output type II
-
-        If `with_masks = False`,
-        The function returns:
-            video : ndarray
-        Note: If `get_vip_particles` is a non-empty list, the first frame in the output will be the masks of the given vip particles in the first frame, else (default) the output will be a ndarray of just the video.
-
-    """
-
-    _particle_dict = {
-        "particle_intensity": [
-            500,
-            20,
-        ],  # Mean and standard deviation of the particle intensity
-        "intensity": lambda particle_intensity: particle_intensity[0]
-        + np.random.randn() * particle_intensity[1],
-        "intensity_variation": 0,  # Intensity variation of particle (in standard deviation)
-        "z": 0,  # Particles are always at focus
-        "refractive_index": 1.45,  # Refractive index of the particle
-        "position_unit": "pixel",
-    }
-
-    _optics_dict = {
-        "NA": 1.46,  # Numerical aperture
-        "wavelength": 500e-9,  # Wavelength
-        "resolution": 100e-9,  # Camera resolution or effective resolution
-        "magnification": 1,
-        "refractive_index_medium": 1.33,
-        "output_region": [0, 0, 128, 128],
-    }
-
-    # Background offset
-    _background_dict = {
-        "background_mean": 100,  # Mean background intensity
-        "background_std": 0,  # Standard deviation of background intensity within a video
-    }
-
-    # Update the dictionaries with the user-defined values
-    _particle_dict.update(particle_props)
-    _optics_dict.update(optics_props)
-    _background_dict.update(background_props)
-
-    # Reshape the trajectory
-    trajectory_data = np.moveaxis(trajectory_data, 0, 1)
-
-    # Generate point particles
-    particle = dt.PointParticle(
-        trajectories=trajectory_data,
-        replicate_index=lambda _ID: _ID,
-        trajectory=lambda replicate_index, trajectories: dt.units.pixel
-        * trajectories[replicate_index[-1]],
-        number_of_particles=trajectory_data.shape[0],
-        traj_length=trajectory_data.shape[1],
-        position=lambda trajectory: trajectory[0],
-        **_particle_dict,
-    )
-
-    # Intensity variation of particles - controlled by "intensity_variation"
-    def intensity_noise(previous_values, previous_value):
-        return (previous_values or [previous_value])[0] + _particle_dict[
-            "intensity_variation"
-        ] * np.random.randn()
-
-    # Make it sequential
-    sequential_particle = dt.Sequential(
-        particle,
-        position=lambda trajectory, sequence_step: trajectory[sequence_step],
-        intensity=intensity_noise,
-    )
-
-    # Adding background offset
-    background = dt.Add(
-        value=_background_dict["background_mean"]
-        + np.random.randn() * _background_dict["background_std"]
-    )
-
-    def background_variation(previous_values, previous_value):
-        return (previous_values or [previous_value])[
-            0
-        ] + np.random.randn() * _background_dict["background_std"]
-
-    ## This will change the background offset within a sequence with a given standard deviation
-    sequential_background = dt.Sequential(background, value=background_variation)
-
-    # Define optical setup
-    optics = dt.Fluorescence(**_optics_dict)
-
-    # Normalising image plane particle intensity
-    scale_factor = (
-        (
-            optics.magnification()
-            * optics.wavelength()
-            / (optics.NA() * optics.resolution())
-        )
-        ** 2
-    ) * (1 / np.pi)
-
-    # Poisson noise
-    poisson_noise = dt.Lambda(func_poisson_noise)
-
-    # Sample
-    sample = (
-        optics(sequential_particle ^ sequential_particle.number_of_particles)
-        >> dt.Multiply(scale_factor)
-        >> sequential_background
-        >> poisson_noise
-    )
-
-    # Masks
-    get_masks = dt.SampleToMasks(
-        lambda: mask(circle_radius=1, particle_list=get_vip_particles),
-        output_region=optics.output_region,
-        merge_method="add",
-    )
-
-    masks = sample >> get_masks >> dt.Add(-1)
-
-    # Sequential sample
-    sequential_sample = dt.Sequence(
-        (sample & masks),
-        trajectory=particle.trajectories,
-        sequence_length=particle.traj_length,
-    )
-
-    # Resolve the sample
-    _video, _masks = sequential_sample.update().resolve()
-
-    if with_masks == True:
-        final_output = (_video, _masks)
-    elif get_vip_particles:
-        final_output = (_masks[0], *_video)
-    else:
-        final_output = _video
-
-    if save_video:
-        if len(final_output) == 2:
-            video_8bit = convert_uint8(final_output[0])
-        else:
-            video_8bit = convert_uint8(final_output, with_vips=get_vip_particles)
-
-        imageio.mimwrite(path, video_8bit)
-
-    return final_output
-
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../source_nbs/lib_nbs/utils_videos.ipynb.
+
+# %% auto 0
+__all__ = ['play_video', 'convert_uint8', 'psf_width', 'func_poisson_noise', 'mask', 'transform_to_video']
+
+# %% ../source_nbs/lib_nbs/utils_videos.ipynb 2
+import matplotlib.animation as animation
+import matplotlib.pyplot as plt
+from IPython.display import HTML
+import numpy as np
+import imageio
+
+# Deeptrack is not automatically installed in andi_datasets
+# due to its load. 
+import warnings
+try:
+    import deeptrack as dt
+except:
+    warnings.warn('Deeptrack is currently not installed. Install if needed using pip install deeptrack.')
+
+# %% ../source_nbs/lib_nbs/utils_videos.ipynb 4
+def play_video(video, figsize=(5, 5), fps=10):
+    """
+    Displays a stack of images as a video inside jupyter notebooks.
+
+    Parameters
+    ----------
+    video : ndarray
+        Stack of images.
+    figsize : tuple, optional
+        Canvas size of the video.
+    fps : int, optional
+        Video frame rate.
+
+    Returns
+    -------
+    Video object
+        Returns a video player with input stack of images.
+    """
+    fig = plt.figure(figsize=figsize)
+    images = []
+    plt.axis("off")
+
+    for image in video:
+        images.append([plt.imshow(image[:, :, 0], cmap="gray")])
+
+    anim = animation.ArtistAnimation(
+        fig, images, interval=1e3 / fps, blit=True, repeat_delay=0
+    )
+
+    html = HTML(anim.to_jshtml())
+    display(html)
+    plt.close()
+
+# %% ../source_nbs/lib_nbs/utils_videos.ipynb 5
+def convert_uint8(vid, with_vips = False):
+    """
+    Converts a stack of images in to 8bit pixel format.
+    
+    This is a helper function for  `transform_to_video`
+
+    Parameters
+    ----------
+    vid : ndarray
+        Stack of images.
+    with_vips: bool, optional
+        Appends a mask of vip particles in the first frame to the converted video.
+    
+    Returns
+    -------
+    ndarray
+        Image stack in 8bit.
+    """
+    new_vid = []
+    for idx_im, im in enumerate(vid):
+        if idx_im == 0 and with_vips:
+            im[im == -1] = 255
+            new_vid.append(im.astype(np.uint8))
+        else:            
+            im = im[:,:,0]
+            im = im / im.max()
+            im = im * 255
+            im = im.astype(np.uint8)
+            new_vid.append(im)
+    return new_vid
+
+# %% ../source_nbs/lib_nbs/utils_videos.ipynb 6
+def psf_width(NA = 1.46, wavelength = 500e-9, resolution = 100e-9):
+    """
+    Computes the PSF width.
+
+    This is a helper function for `transform_to_video`
+    
+    Parameters
+    ----------
+    NA : float
+        Numerical aperture.
+    wavelength : float
+        Wavelength.
+    resolution : float
+        Resolution of the camera.
+    
+    Returns
+    -------
+    int
+        PSF width in pixels.
+    """
+    _psf = 1.22 * wavelength / (2 * NA)
+    return int(_psf / resolution)
+
+# %% ../source_nbs/lib_nbs/utils_videos.ipynb 7
+def func_poisson_noise():
+    """
+    Applies poisson noise to an image.
+
+    This is a custom DeepTrack feature, and a helper function for `transform_to_video`
+    """
+    def inner(image):
+        image[image<0] = 0
+        rescale = 1
+        noisy_image = np.random.poisson(image * rescale) / rescale
+        return noisy_image
+    return inner
+
+# %% ../source_nbs/lib_nbs/utils_videos.ipynb 8
+def mask(circle_radius, particle_list=[]):
+    """
+    Computes binary masks for particles in microscopy videos.
+
+    This is a custom DeepTrack feature, and a helper function for `transform_to_video`.
+
+    Parameters
+    ----------
+    particle_list: list of int
+        List of particles whose masks need to be created
+
+    """
+    def inner(image):
+        X, Y = np.mgrid[:2*circle_radius, :2*circle_radius]
+        CIRCLE = (X - circle_radius+0.5)**2 + (Y- circle_radius+0.5)**2 < circle_radius**2
+        CIRCLE = np.expand_dims(CIRCLE, axis=-1)
+        _index = image.get_property("replicate_index")[0]
+        if particle_list:
+            if _index in particle_list:
+                pix_val = (_index + 1) * CIRCLE
+            else:
+                pix_val = 0 * CIRCLE
+        else:
+            pix_val = (_index + 1) * CIRCLE
+        return pix_val
+    return inner
+
+# %% ../source_nbs/lib_nbs/utils_videos.ipynb 10
+def transform_to_video(
+    trajectory_data,
+    particle_props={},
+    optics_props={},
+    background_props={},
+    get_vip_particles=[],
+    with_masks=False,
+    save_video=False,
+    path="",
+):
+    """
+    Transforms trajectory data into microscopy imagery data.
+
+    Trajectories generated through phenomenological models in andi-datasets are imaged under a Fluorescence microscope to generate 2D timelapse videos.
+
+    Parameters
+    ----------
+    trajectory_data : ndarray
+        Generated through models_phenom. Array of the shape (T, N, 2) containing the trajectories.
+    particle_props : dict
+        Dictionary containing the properties of particles to be simulated as keyword arguments. Valid keys are:
+
+            '`particle_intensity`' : array_like[int, int]
+                Intensity distribution of particles within a frame given as mean and standard deviations.
+
+            '`intensity_variation`' : int
+                Intensity variation of particles in subsequent frames given as standard deviation.
+
+            '`z`' : float
+                Particle positions with respect to the focal plane in pixel units defined by the pixel size in **optics_props**. For example, particles will be at focus when `z=0`.
+
+            '`refractive_index`' : float
+                Refractive index of particle.
+
+    optics_props : dict
+        Dictionary containing the properties of microscope as keyword arguments. Valid keys are:
+
+            '`NA`': float
+                Numerical aperture of the microscope.
+
+            '`wavelength`' : float
+                Wavelength of light in meters.
+
+            '`resolution`' : float
+                Effective pixel size of the camera in meters.
+
+            '`magnification`' : float
+                Magnification of the optical system.
+
+            '`refractive_index_medium`' : float
+                Refractive index of the medium sorrounding the particles.
+
+            '`output_region`': array_like[int, int, int, int]
+                ROI of the image to output.
+                Given in the format : [x, y, x + width, y + height].
+
+    background_props : dict
+        Dictionary containing properties related to background intensity as keyword arguments. Valid keys are:
+
+            '`background_mean`' : int
+                Mean background intensity.
+
+            '`backgound_std`' : int
+                Standard deviation of the background intesity with subsequent frames of a video.
+
+    get_vip_particles : list of int
+        List of particles for which the masks are needed in the output.
+
+    with_masks : bool
+        If True, particle masks are returned in the output along with the video.
+        If False (default), only the video is returned in the output.
+
+    save_video : bool
+        If True, the generated video will be saved at the given path.
+    path : str
+        File path for saving the video, the path should be given along the video format.
+        For example: 'path' = './video.mp4' will save the video in the current folder.
+
+    Returns
+    -------
+    tuple | ndarray
+
+        Output type I 
+
+        If `with_masks = True`,
+        The function returns a tuple containing:
+            masks : ndarray
+            video : ndarray
+        Note: If `get_vip_particles` is a non-empty list, the masks will contain only the vip particle masks.
+
+        Output type II
+
+        If `with_masks = False`,
+        The function returns:
+            video : ndarray
+        Note: If `get_vip_particles` is a non-empty list, the first frame in the output will be the masks of the given vip particles in the first frame, else (default) the output will be a ndarray of just the video.
+
+    """
+
+    _particle_dict = {
+        "particle_intensity": [
+            500,
+            20,
+        ],  # Mean and standard deviation of the particle intensity
+        "intensity": lambda particle_intensity: particle_intensity[0]
+        + np.random.randn() * particle_intensity[1],
+        "intensity_variation": 0,  # Intensity variation of particle (in standard deviation)
+        "z": 0,  # Particles are always at focus
+        "refractive_index": 1.45,  # Refractive index of the particle
+        "position_unit": "pixel",
+    }
+
+    _optics_dict = {
+        "NA": 1.46,  # Numerical aperture
+        "wavelength": 500e-9,  # Wavelength
+        "resolution": 100e-9,  # Camera resolution or effective resolution
+        "magnification": 1,
+        "refractive_index_medium": 1.33,
+        "output_region": [0, 0, 128, 128],
+    }
+
+    # Background offset
+    _background_dict = {
+        "background_mean": 100,  # Mean background intensity
+        "background_std": 0,  # Standard deviation of background intensity within a video
+    }
+
+    # Update the dictionaries with the user-defined values
+    _particle_dict.update(particle_props)
+    _optics_dict.update(optics_props)
+    _background_dict.update(background_props)
+
+    # Reshape the trajectory
+    trajectory_data = np.moveaxis(trajectory_data, 0, 1)
+
+    # Generate point particles
+    particle = dt.PointParticle(
+        trajectories=trajectory_data,
+        replicate_index=lambda _ID: _ID,
+        trajectory=lambda replicate_index, trajectories: dt.units.pixel
+        * trajectories[replicate_index[-1]],
+        number_of_particles=trajectory_data.shape[0],
+        traj_length=trajectory_data.shape[1],
+        position=lambda trajectory: trajectory[0],
+        **_particle_dict,
+    )
+
+    # Intensity variation of particles - controlled by "intensity_variation"
+    def intensity_noise(previous_values, previous_value):
+        return (previous_values or [previous_value])[0] + _particle_dict[
+            "intensity_variation"
+        ] * np.random.randn()
+
+    # Make it sequential
+    sequential_particle = dt.Sequential(
+        particle,
+        position=lambda trajectory, sequence_step: trajectory[sequence_step],
+        intensity=intensity_noise,
+    )
+
+    # Adding background offset
+    background = dt.Add(
+        value=_background_dict["background_mean"]
+        + np.random.randn() * _background_dict["background_std"]
+    )
+
+    def background_variation(previous_values, previous_value):
+        return (previous_values or [previous_value])[
+            0
+        ] + np.random.randn() * _background_dict["background_std"]
+
+    ## This will change the background offset within a sequence with a given standard deviation
+    sequential_background = dt.Sequential(background, value=background_variation)
+
+    # Define optical setup
+    optics = dt.Fluorescence(**_optics_dict)
+
+    # Normalising image plane particle intensity
+    scale_factor = (
+        (
+            optics.magnification()
+            * optics.wavelength()
+            / (optics.NA() * optics.resolution())
+        )
+        ** 2
+    ) * (1 / np.pi)
+
+    # Poisson noise
+    poisson_noise = dt.Lambda(func_poisson_noise)
+
+    # Sample
+    sample = (
+        optics(sequential_particle ^ sequential_particle.number_of_particles)
+        >> dt.Multiply(scale_factor)
+        >> sequential_background
+        >> poisson_noise
+    )
+
+    # Masks
+    get_masks = dt.SampleToMasks(
+        lambda: mask(circle_radius=1, particle_list=get_vip_particles),
+        output_region=optics.output_region,
+        merge_method="add",
+    )
+
+    masks = sample >> get_masks >> dt.Add(-1)
+
+    # Sequential sample
+    sequential_sample = dt.Sequence(
+        (sample & masks),
+        trajectory=particle.trajectories,
+        sequence_length=particle.traj_length,
+    )
+
+    # Resolve the sample
+    _video, _masks = sequential_sample.update().resolve()
+
+    if with_masks == True:
+        final_output = (_video, _masks)
+    elif get_vip_particles:
+        final_output = (_masks[0], *_video)
+    else:
+        final_output = _video
+
+    if save_video:
+        if len(final_output) == 2:
+            video_8bit = convert_uint8(final_output[0])
+        else:
+            video_8bit = convert_uint8(final_output, with_vips=get_vip_particles)
+
+        imageio.mimwrite(path, video_8bit)
+
+    return final_output
+
```

### Comparing `andi_datasets-2.0.3/andi_datasets.egg-info/SOURCES.txt` & `andi_datasets-2.0.4/andi_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `andi_datasets-2.0.3/settings.ini` & `andi_datasets-2.0.4/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-[DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
-repo = andi_datasets
-lib_name = %(repo)s
-version = 2.0.3
-min_python = 3.10
-license = apache2
-
-### nbdev ###
-doc_path = docs
-lib_path = andi_datasets
-nbs_path = source_nbs
-recursive = True
-tst_flags = notest
-
-### Docs ###
-branch = master
-custom_sidebar = True
-custom_quarto_yml = True
-user = andichallenge
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(lib_name)s
-git_url = https://github.com/%(user)s/%(lib_name)s
-title = %(lib_name)s
-
-### PyPI ###
-audience = Developers
-author = Gorka Munoz-Gil
-author_email = munoz.gil.gorka@gmail.com
-copyright = 2019 onwards, %(author)s
-description = Generate, manage and analyze anomalous diffusion trajectories.
-keywords = anomalous diffusion
-language = English
-status = 3
-
-### Optional ###
-requirements = numpy stochastic tqdm scipy h5py pandas matplotlib sklearn imageio
-# dev_requirements =
-# console_scripts =
+[DEFAULT]
+# All sections below are required unless otherwise specified.
+# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
+
+### Python library ###
+repo = andi_datasets
+lib_name = %(repo)s
+version = 2.0.4
+min_python = 3.10
+license = apache2
+
+### nbdev ###
+doc_path = docs
+lib_path = andi_datasets
+nbs_path = source_nbs
+recursive = True
+tst_flags = notest
+
+### Docs ###
+branch = master
+custom_sidebar = True
+custom_quarto_yml = True
+user = andichallenge
+doc_host = https://%(user)s.github.io
+doc_baseurl = /%(lib_name)s
+git_url = https://github.com/%(user)s/%(lib_name)s
+title = %(lib_name)s
+
+### PyPI ###
+audience = Developers
+author = Gorka Munoz-Gil
+author_email = munoz.gil.gorka@gmail.com
+copyright = 2019 onwards, %(author)s
+description = Generate, manage and analyze anomalous diffusion trajectories.
+keywords = anomalous diffusion
+language = English
+status = 3
+
+### Optional ###
+requirements = numpy stochastic tqdm scipy h5py pandas matplotlib scikit-learn imageio
+# dev_requirements =
+# console_scripts =
```

### Comparing `andi_datasets-2.0.3/setup.py` & `andi_datasets-2.0.4/setup.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from pkg_resources import parse_version
-from configparser import ConfigParser
-import setuptools
-assert parse_version(setuptools.__version__)>=parse_version('36.2')
-
-# note: all settings are in settings.ini; edit there, not here
-config = ConfigParser(delimiters=['='])
-config.read('settings.ini')
-cfg = config['DEFAULT']
-
-cfg_keys = 'version description keywords author author_email'.split()
-expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
-for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
-setup_cfg = {o:cfg[o] for o in cfg_keys}
-
-licenses = {
-    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
-}
-statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
-    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
-
-requirements = cfg.get('requirements','').split()
-if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
-min_python = cfg['min_python']
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-dev_requirements = (cfg.get('dev_requirements') or '').split()
-
-setuptools.setup(
-    name = cfg['lib_name'],
-    license = lic[0],
-    classifiers = [
-        'Development Status :: ' + statuses[int(cfg['status'])],
-        'Intended Audience :: ' + cfg['audience'].title(),
-        'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
-    url = cfg['git_url'],
-    packages = setuptools.find_packages(),
-    include_package_data = True,
-    install_requires = requirements,
-    extras_require={ 'dev': dev_requirements },
-    dependency_links = cfg.get('dep_links','').split(),
-    python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md').read(),
-    long_description_content_type = 'text/markdown',
-    zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
-    **setup_cfg)
+from pkg_resources import parse_version
+from configparser import ConfigParser
+import setuptools
+assert parse_version(setuptools.__version__)>=parse_version('36.2')
+
+# note: all settings are in settings.ini; edit there, not here
+config = ConfigParser(delimiters=['='])
+config.read('settings.ini')
+cfg = config['DEFAULT']
+
+cfg_keys = 'version description keywords author author_email'.split()
+expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
+for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
+setup_cfg = {o:cfg[o] for o in cfg_keys}
+
+licenses = {
+    'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
+    'mit': ('MIT License', 'OSI Approved :: MIT License'),
+    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
+    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
+}
+statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
+    '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
+py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
+
+requirements = cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
+min_python = cfg['min_python']
+lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
+dev_requirements = (cfg.get('dev_requirements') or '').split()
+
+setuptools.setup(
+    name = cfg['lib_name'],
+    license = lic[0],
+    classifiers = [
+        'Development Status :: ' + statuses[int(cfg['status'])],
+        'Intended Audience :: ' + cfg['audience'].title(),
+        'Natural Language :: ' + cfg['language'].title(),
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
+    url = cfg['git_url'],
+    packages = setuptools.find_packages(),
+    include_package_data = True,
+    install_requires = requirements,
+    extras_require={ 'dev': dev_requirements },
+    dependency_links = cfg.get('dep_links','').split(),
+    python_requires  = '>=' + cfg['min_python'],
+    long_description = open('README.md').read(),
+    long_description_content_type = 'text/markdown',
+    zip_safe = False,
+    entry_points = {
+        'console_scripts': cfg.get('console_scripts','').split(),
+        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
+    },
+    **setup_cfg)
```

