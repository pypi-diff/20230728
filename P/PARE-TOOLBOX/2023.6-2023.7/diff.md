# Comparing `tmp/PARE_TOOLBOX-2023.6.tar.gz` & `tmp/PARE_TOOLBOX-2023.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PARE_TOOLBOX-2023.6.tar", last modified: Tue Jul 25 12:28:23 2023, max compression
+gzip compressed data, was "PARE_TOOLBOX-2023.7.tar", last modified: Fri Jul 28 18:54:49 2023, max compression
```

## Comparing `PARE_TOOLBOX-2023.6.tar` & `PARE_TOOLBOX-2023.7.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 12:28:23.518617 PARE_TOOLBOX-2023.6/
-drwxrwxrwx   0        0        0        0 2023-07-25 12:28:23.501866 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/
--rw-rw-rw-   0        0        0     7905 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/PARE.py
--rw-rw-rw-   0        0        0     2992 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/ZIPPER.py
--rw-rw-rw-   0        0        0       42 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 12:28:23.517617 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/
--rw-rw-rw-   0        0        0      644 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-25 12:28:23.000000 PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2023-07-25 12:28:23.518617 PARE_TOOLBOX-2023.6/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-07-25 12:00:06.000000 PARE_TOOLBOX-2023.6/license.md
--rw-rw-rw-   0        0        0       42 2023-07-25 12:28:23.518617 PARE_TOOLBOX-2023.6/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-07-25 12:28:07.000000 PARE_TOOLBOX-2023.6/setup.py
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-07-28 18:54:49.444910 PARE_TOOLBOX-2023.7/
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-07-28 18:54:49.440910 PARE_TOOLBOX-2023.7/PARE_TOOLBOX/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     9190 2023-07-28 18:44:27.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX/PARE.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     2888 2023-07-28 16:45:18.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX/ZIPPER.py
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       41 2023-07-28 16:45:18.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX/__init__.py
+drwxrwxr-x   0 wanderlei  (1000) wanderlei  (1000)        0 2023-07-28 18:54:49.444910 PARE_TOOLBOX-2023.7/PARE_TOOLBOX.egg-info/
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      633 2023-07-28 18:54:49.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      256 2023-07-28 18:54:49.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)        1 2023-07-28 18:54:49.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       19 2023-07-28 18:54:49.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX.egg-info/requires.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       13 2023-07-28 18:54:49.000000 PARE_TOOLBOX-2023.7/PARE_TOOLBOX.egg-info/top_level.txt
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)      633 2023-07-28 18:54:49.444910 PARE_TOOLBOX-2023.7/PKG-INFO
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)       38 2023-07-28 18:54:49.444910 PARE_TOOLBOX-2023.7/setup.cfg
+-rw-rw-r--   0 wanderlei  (1000) wanderlei  (1000)     1325 2023-07-28 18:54:39.000000 PARE_TOOLBOX-2023.7/setup.py
```

### Comparing `PARE_TOOLBOX-2023.6/PARE_TOOLBOX/PARE.py` & `PARE_TOOLBOX-2023.7/PARE_TOOLBOX/PARE.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,195 +1,242 @@
-import numpy as np
-import random
-import pandas as pd
-import json
-import time
-from datetime import datetime
-from scipy.stats.distributions import norm
-from scipy.stats.distributions import gumbel_r
-from scipy.stats.distributions import gumbel_l
-from scipy.stats.distributions import lognorm
-from scipy.stats.distributions import uniform
-from scipy.stats.distributions import triang
-import multiprocessing
-from multiprocessing import Pool
-import PARE_TOOLBOX.ZIPPER as z
-
-
-def SAMPLING(**kwargs):
-    """ 
-    This algorithm generates a set of random numbers according to a type distribution.
-
-    See documentation in wmpjrufg.github.io/RASDPY/
-    """
-    if len(kwargs) != 4:
-        raise ValueError("this fuction require four inputs!")
-
-    # Creating variables
-    N_POP = kwargs['N_POP']
-    D = kwargs['D']
-    MODEL = kwargs['MODEL']
-    VARS = kwargs['VARS']
-    RANDOM_STATE = random.sample(range(1, 1000), D)
-    RANDOM_SAMPLING = np.zeros((N_POP, D))
-    
-    # Monte Carlo sampling
-    if MODEL.upper() == 'MCS':
-        for I in range(D):
-            # Type of distribution, mean and standard deviation
-            TYPE = VARS[I][0].upper()
-            MEAN = VARS[I][1]
-            STD = VARS[I][2]
-            # Normal or Gaussian
-            if TYPE == 'GAUSSIAN' or TYPE == 'NORMAL':
-                RANDOM_SAMPLING[:, I] = norm.rvs(loc = MEAN, scale = STD, size = N_POP, random_state = RANDOM_STATE[I])
-            # Gumbel right or Gumbel maximum
-            elif TYPE == 'GUMBEL MAX':
-                RANDOM_SAMPLING[:, I] = gumbel_r.rvs(loc = MEAN, scale = STD, size = N_POP, random_state = RANDOM_STATE[I])
-            # Gumbel left or Gumbel minimum
-            elif TYPE == 'GUMBEL MIN':
-                RANDOM_SAMPLING[:, I] = gumbel_l.rvs(loc = MEAN, scale = STD, size = N_POP, random_state = RANDOM_STATE[I])
-            # Lognormal
-            elif TYPE == 'LOGNORMAL':
-                RANDOM_SAMPLING[:, I] = lognorm.rvs(s = STD, loc = MEAN, scale = np.exp(MEAN), size = N_POP, random_state = RANDOM_STATE[I])
-            # Uniform
-            elif TYPE == 'UNIFORM':
-                RANDOM_SAMPLING[:, I] = uniform.rvs(loc = MEAN, scale=STD, size = N_POP, random_state = RANDOM_STATE[I])
-            # Triangular
-            elif TYPE == 'TRIANGULAR':
-                LOC = VARS[I][1]
-                SCALE = VARS[I][2]
-                C = VARS[I][3]
-                #loc is the start, scale is the base width, c is the mode percentage
-                RANDOM_SAMPLING[:, I] = triang.rvs(loc = LOC, scale = SCALE, c = (C - LOC) / (SCALE - LOC), size = N_POP, random_state = RANDOM_STATE[I])
-
-    return RANDOM_SAMPLING, RANDOM_STATE
-
-def EVALUATION_MODEL(INFO):
-    SAMPLE = INFO[0]
-    OF_FUNCTION = INFO[1]
-    NULL_DIC = INFO[2]
-    R, S, G = OF_FUNCTION(SAMPLE, NULL_DIC)
-    RESULTS = [R, S, G]
-    return RESULTS
-
-def MCS_LHS_ALGORITHM(SETUP, OF_FUNCTION):
-    """
-    This function creates the samples and evaluates the limit state functions.
-    
-    See documentation in wmpjrufg.github.io/RASDPY/
-    """ 
-    
-    # Initial setup
-    INIT = time.time()
-    N_POP = SETUP['N_POP']
-    D = SETUP['D']
-    MODEL = SETUP['MODEL']
-    VARS = SETUP['VARS']
-    N_G = SETUP['N_G']
-    STEP = 1000
-    NULL_DIC = SETUP['NULL_DIC']
-    RESULTS_R = np.zeros((N_POP, N_G))
-    RESULTS_S = np.zeros((N_POP, N_G))
-    RESULTS_G = np.zeros((N_POP, N_G))
-    RESULTS_I = np.zeros((N_POP, N_G))  
-    MODEL_NAME = 'MCS_LHS'
-    TYPE_PROCESS = 'PARALLEL'
-    
-    # BETA_DF = RASD_CL.PROBABILITY_OF_FAILURE() - Vamos mudar esse calc aqui para uma derivada numérica vou pensar em como fazer
-
-    # Creating samples   
-    DATASET_X, RANDOM_STATE = SAMPLING(N_POP = N_POP, D = D, MODEL = MODEL, VARS = VARS)   
-
-    # Multiprocess Objective Function evaluation
-    if TYPE_PROCESS == 'PARALLEL':
-        POOLS = multiprocessing.cpu_count() - 1   
-        INFO = [[list(I), OF_FUNCTION, NULL_DIC] for I in DATASET_X]
-        with Pool(processes = POOLS) as pool:
-            RESULT = pool.map_async(EVALUATION_MODEL, INFO)
-            RESULT = RESULT.get()
-        for K in range(N_POP):
-            RESULTS_R[K, :] = RESULT[K][0]
-            RESULTS_S[K, :] = RESULT[K][1]
-            RESULTS_G[K, :] = RESULT[K][2]
-            RESULTS_I[K, :] = [0 if value <= 0 else 1 for value in RESULT[K][2]]
-    # Singleprocess Objective Function evaluation
-    elif TYPE_PROCESS == 'SERIAL':
-        RESULT = []
-        for I in DATASET_X:
-            INFO = [I, OF_FUNCTION, NULL_DIC]
-            RES = EVALUATION_MODEL(INFO)
-            RESULT.append(RES)
-        for K in range(N_POP):
-            RESULTS_R[K, :] = RESULT[K][0]
-            RESULTS_S[K, :] = RESULT[K][1]
-            RESULTS_G[K, :] = RESULT[K][2]
-            RESULTS_I[K, :] = [0 if value <= 0 else 1 for value in RESULT[K][2]] 
-            
-    # Storage all results
-    AUX = np.hstack((DATASET_X, RESULTS_R, RESULTS_S, RESULTS_G, RESULTS_I))
-    RESULTS_RASD = pd.DataFrame(AUX)          
-    # Rename columns in dataframe 
-    COLUMNS_NAMES = []
-    for L in range(D):
-        COLUMNS_NAMES.append('X_' + str(L))
-    for L in range(N_G):
-        COLUMNS_NAMES.append('R_' + str(L))  
-    for L in range(N_G):
-        COLUMNS_NAMES.append('S_' + str(L))
-    for L in range(N_G):
-        COLUMNS_NAMES.append('G_' + str(L))
-    for L in range(N_G):
-        COLUMNS_NAMES.append('I_' + str(L))
-    RESULTS_RASD.columns = COLUMNS_NAMES
-    
-    # Resume data 
-    # Creates data for .json type output considering the chosen step
-    VALUES = list(np.arange(1, N_POP, STEP, dtype = int))
-    if VALUES[-1] != N_POP:
-        VALUES.append(N_POP)
-    VALUES = [int(X) for X in VALUES]
-    RESUME_DATA = {'seeds': RANDOM_STATE, 'number of samples': VALUES, 'results': {}}
-    for L in range(N_G):
-        KEY = f'I_{L}' 
-        N_F = []
-        P_F = []
-        for I in VALUES:
-            LINES = RESULTS_RASD[:I]
-            # Failure probability
-            N_FAILURE = int(LINES[KEY].sum())
-            P_FVALUE = N_FAILURE / I
-            N_F.append(N_FAILURE)
-            P_F.append(P_FVALUE)
-        RESUME_DATA['results'][KEY] = {'NF': N_F, 'PF': P_F}
-
-    # Resume process (Time and outputs)
-    END = time.time()
-    # Emoji unicode: https://apps.timwhitlock.info/emoji/tables/unicode
-    print('PAREpy report: \n') 
-    NAME = MODEL_NAME + '_' + str(datetime.now().strftime('%Y%m%d-%H%M%S'))
-    print(f' \U00003299 ID report: {NAME} \n') 
-    print(' \U0001F680' + f' Process Time {TYPE_PROCESS} version ' + '\U000023F0' + ' %.2f' % (END - INIT), 'Seconds \n') 
-    with open(NAME + '.json', 'w') as FILE:
-        json.dump(RESUME_DATA, FILE)  
-        print(' \U0001F197' + ' Save results in .json file! \n')
-    RESULTS_RASD.to_csv(NAME + '.txt', sep = '\t', index = False)
-    print(' \U0001F197' + ' Save dataset in .txt file!')
-    z.ZIPPER(NAME)
-    z.UNZIPPER(NAME)
-    print('\n \U0001F4C1' + ' Files into the folder' +  ' ' + NAME) 
-
-    """
-    BETA_DF = pd.read_csv('RASD_TOOLBOX/beta_df.txt', delimiter = ";",  names = ['PF' ,'BETA'])
-    BETA_APROX = round(P_FVALUE,5)
-    BETA_VALUE_INDEX = (BETA_DF['PF'].sub(P_FVALUE).abs().idxmin())
-    BETA_VALUE = BETA_DF['BETA'][BETA_VALUE_INDEX]   
-    BETA_F.append(BETA_VALUE)
-
-    # Save results
-    RESULTS_REP = {'TOTAL RESULTS': RESULTS_RASD, 'NUMBER OF FAILURES': N_F, 'PROBABILITY OF FAILURE': P_F, 'BETA INDEX': BETA_F}
-    RESULTS.append(RESULTS_REP)
-    NAME = 'RASD_' + MODEL + '_REP_' + str(J) + '_SAMPLES_' + str(N_POP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')) + '.txt'
-    HEADER_NAMES =  ';'.join(COLUMNS_NAMES)
-    np.savetxt(NAME, RESULTS_RASD, fmt = '%1.5f', delimiter = ';' , header = HEADER_NAMES)
-    """
+import numpy as np
+import random
+import pandas as pd
+import json
+import time
+from datetime import datetime
+from scipy.stats.distributions import norm
+from scipy.stats.distributions import gumbel_r
+from scipy.stats.distributions import gumbel_l
+from scipy.stats.distributions import lognorm
+from scipy.stats.distributions import uniform
+from scipy.stats.distributions import triang
+import multiprocessing
+from multiprocessing import Pool
+import PARE_TOOLBOX.ZIPPER as z
+
+
+
+def SAMPLING(**kwargs):
+    """ 
+    This algorithm generates a set of random numbers according to a type distribution.
+
+    See documentation in wmpjrufg.github.io/RASDPY/
+    """
+    if len(kwargs) != 4:
+        raise ValueError("this fuction require four inputs!")
+
+    # Creating variables
+    N_POP = kwargs['N_POP']
+    D = kwargs['D']
+    MODEL = kwargs['MODEL']
+    VARS = kwargs['VARS']
+    RANDOM_STATE = random.sample(range(1, 1000), D)
+    RANDOM_SAMPLING = np.zeros((N_POP, D))
+    
+    # Monte Carlo sampling
+    if MODEL.upper() == 'MCS':
+        for I in range(D):
+            # Type of distribution, mean and standard deviation
+            TYPE = VARS[I][0].upper()
+            MEAN = VARS[I][1]
+            STD = VARS[I][2]
+            # Normal or Gaussian
+            if TYPE == 'GAUSSIAN' or TYPE == 'NORMAL':
+                RANDOM_SAMPLING[:, I] = norm.rvs(loc = MEAN, scale = STD, size = N_POP, random_state = RANDOM_STATE[I])
+            # Gumbel right or Gumbel maximum
+            elif TYPE == 'GUMBEL MAX':
+                RANDOM_SAMPLING[:, I] = gumbel_r.rvs(loc = MEAN, scale = STD, size = N_POP, random_state = RANDOM_STATE[I])
+            # Gumbel left or Gumbel minimum
+            elif TYPE == 'GUMBEL MIN':
+                RANDOM_SAMPLING[:, I] = gumbel_l.rvs(loc = MEAN, scale = STD, size = N_POP, random_state = RANDOM_STATE[I])
+            # Lognormal
+            elif TYPE == 'LOGNORMAL':
+                RANDOM_SAMPLING[:, I] = lognorm.rvs(s = STD, loc = MEAN, scale = np.exp(MEAN), size = N_POP, random_state = RANDOM_STATE[I])
+            # Uniform
+            elif TYPE == 'UNIFORM':
+                RANDOM_SAMPLING[:, I] = uniform.rvs(loc = MEAN, scale=STD, size = N_POP, random_state = RANDOM_STATE[I])
+            # Triangular
+            elif TYPE == 'TRIANGULAR':
+                LOC = VARS[I][1]
+                SCALE = VARS[I][2]
+                C = VARS[I][3]
+                #loc is the start, scale is the base width, c is the mode percentage
+                RANDOM_SAMPLING[:, I] = triang.rvs(loc = LOC, scale = SCALE, c = (C - LOC) / (SCALE - LOC), size = N_POP, random_state = RANDOM_STATE[I])
+
+    return RANDOM_SAMPLING, RANDOM_STATE
+
+def EVALUATION_MODEL(INFO):
+    SAMPLE = INFO[0]
+    OF_FUNCTION = INFO[1]
+    NULL_DIC = INFO[2]
+    R, S, G = OF_FUNCTION(SAMPLE, NULL_DIC)
+    RESULTS = [R, S, G]
+    return RESULTS
+
+def GET_TYPE_PROCESS(SETUP, OF_FUNCTION, SAMPLING, EVALUATION_MODEL):
+    """ 
+    This function gets the type of process.
+    It executes the function with a dataset of 10 samples. 
+    The return is a string with the type of process. 
+    The NPOP always is 10.
+    """
+
+    # Initial setup
+    N_POP = 10
+    D = SETUP['D']
+    MODEL = SETUP['MODEL']
+    VARS = SETUP['VARS']
+    NULL_DIC = SETUP['NULL_DIC']
+   
+    DATASET_X, _ = SAMPLING(N_POP = N_POP, D = D, MODEL = MODEL, VARS = VARS)   
+
+    INIT_TIME = time.time()
+    POOLS = multiprocessing.cpu_count() - 1   
+    INFO = [[list(I), OF_FUNCTION, NULL_DIC] for I in DATASET_X]
+    with Pool(processes = POOLS) as pool:
+        RESULT = pool.map_async(EVALUATION_MODEL, INFO)
+        RESULT = RESULT.get()
+    FINISH_TIME = time.time() 
+    
+    INIT_TIME2 = time.time()
+    RESULT = []
+    for I in DATASET_X:
+        INFO = [I, OF_FUNCTION, NULL_DIC]
+        INIT_TIME_FO = time.time()
+        RES = EVALUATION_MODEL(INFO)
+        END_TIME_FO = time.time()
+        RESULT.append(RES)
+    FINISH_TIME2 = time.time()
+    FO_TIME = (END_TIME_FO - INIT_TIME_FO)  
+
+    if(FINISH_TIME - INIT_TIME) < (FINISH_TIME2 - INIT_TIME2):
+        TYPE_PROCESS = 'PARALLEL'
+    else:
+        TYPE_PROCESS = 'SERIAL'
+
+    return TYPE_PROCESS, FO_TIME
+
+
+def MCS_LHS_ALGORITHM(SETUP, OF_FUNCTION):
+    """
+    This function creates the samples and evaluates the limit state functions.
+    
+    See documentation in wmpjrufg.github.io/RASDPY/
+    """ 
+    
+    # Initial setup
+    INIT = time.time()
+    N_POP = SETUP['N_POP']
+    D = SETUP['D']
+    MODEL = SETUP['MODEL']
+    VARS = SETUP['VARS']
+    N_G = SETUP['N_G']
+    STEP = 1000
+    NULL_DIC = SETUP['NULL_DIC']
+    RESULTS_R = np.zeros((N_POP, N_G))
+    RESULTS_S = np.zeros((N_POP, N_G))
+    RESULTS_G = np.zeros((N_POP, N_G))
+    RESULTS_I = np.zeros((N_POP, N_G))  
+    MODEL_NAME = 'MCS_LHS'
+    
+    # BETA_DF = RASD_CL.PROBABILITY_OF_FAILURE() - Vamos mudar esse calc aqui para uma derivada numérica vou pensar em como fazer
+
+    # Creating samples   
+    DATASET_X, RANDOM_STATE = SAMPLING(N_POP = N_POP, D = D, MODEL = MODEL, VARS = VARS)   
+
+    TYPE_PROCESS, FO_TIME = GET_TYPE_PROCESS(SETUP, OF_FUNCTION, SAMPLING, EVALUATION_MODEL)
+
+    # Multiprocess Objective Function evaluation
+    if TYPE_PROCESS == 'PARALLEL':
+        POOLS = multiprocessing.cpu_count() - 1   
+        INFO = [[list(I), OF_FUNCTION, NULL_DIC] for I in DATASET_X]
+        with Pool(processes = POOLS) as pool:
+            RESULT = pool.map_async(EVALUATION_MODEL, INFO)
+            RESULT = RESULT.get()
+        for K in range(N_POP):
+            RESULTS_R[K, :] = RESULT[K][0]
+            RESULTS_S[K, :] = RESULT[K][1]
+            RESULTS_G[K, :] = RESULT[K][2]
+            RESULTS_I[K, :] = [0 if value <= 0 else 1 for value in RESULT[K][2]]
+    # Singleprocess Objective Function evaluation
+    elif TYPE_PROCESS == 'SERIAL':
+        RESULT = []
+        for I in DATASET_X:
+            INFO = [I, OF_FUNCTION, NULL_DIC]
+            RES = EVALUATION_MODEL(INFO)
+            RESULT.append(RES)
+        for K in range(N_POP):
+            RESULTS_R[K, :] = RESULT[K][0]
+            RESULTS_S[K, :] = RESULT[K][1]
+            RESULTS_G[K, :] = RESULT[K][2]
+            RESULTS_I[K, :] = [0 if value <= 0 else 1 for value in RESULT[K][2]] 
+            
+    # Storage all results
+    AUX = np.hstack((DATASET_X, RESULTS_R, RESULTS_S, RESULTS_G, RESULTS_I))
+    RESULTS_RASD = pd.DataFrame(AUX)          
+    # Rename columns in dataframe 
+    COLUMNS_NAMES = []
+    for L in range(D):
+        COLUMNS_NAMES.append('X_' + str(L))
+    for L in range(N_G):
+        COLUMNS_NAMES.append('R_' + str(L))  
+    for L in range(N_G):
+        COLUMNS_NAMES.append('S_' + str(L))
+    for L in range(N_G):
+        COLUMNS_NAMES.append('G_' + str(L))
+    for L in range(N_G):
+        COLUMNS_NAMES.append('I_' + str(L))
+    RESULTS_RASD.columns = COLUMNS_NAMES
+    
+    # Resume data 
+    # Creates data for .json type output considering the chosen step
+    VALUES = list(np.arange(1, N_POP, STEP, dtype = int))
+    if VALUES[-1] != N_POP:
+        VALUES.append(N_POP)
+    VALUES = [int(X) for X in VALUES]
+    RESUME_DATA = {'seeds': RANDOM_STATE, 'number of samples': VALUES, 'results': {}}
+    for L in range(N_G):
+        KEY = f'I_{L}' 
+        N_F = []
+        P_F = []
+        for I in VALUES:
+            LINES = RESULTS_RASD[:I]
+            # Failure probability
+            N_FAILURE = int(LINES[KEY].sum())
+            P_FVALUE = N_FAILURE / I
+            N_F.append(N_FAILURE)
+            P_F.append(P_FVALUE)
+        RESUME_DATA['results'][KEY] = {'NF': N_F, 'PF': P_F}
+
+    # Resume process (Time and outputs)
+    END = time.time()
+    # Emoji unicode: https://apps.timwhitlock.info/emoji/tables/unicode
+    print('PAREpy report: \n') 
+    NAME = MODEL_NAME + '_' + str(datetime.now().strftime('%Y%m%d-%H%M%S'))
+    print(f' \U0001F202 ID report: {NAME} \n') 
+    print(' \U0001F680' + f' Process Time ({TYPE_PROCESS} version) ' + '\U000023F0' + ' %.2f' % (END - INIT), 'seconds \n') 
+    print(' \U0001F550' + ' Objective function time evaluation per sample: ' + ' %.4f' % FO_TIME + ' seconds\n') 
+    with open(NAME + '.json', 'w') as FILE:
+        json.dump(RESUME_DATA, FILE)  
+        print(' \U0001F197' + ' Save results in .json file! \n')
+    RESULTS_RASD.to_csv(NAME + '.txt', sep = '\t', index = False)
+    print(' \U0001F197' + ' Save dataset in .txt file!')
+    z.ZIPPER(NAME)
+    z.UNZIPPER(NAME)
+    print('\n \U0001F4C1' + ' Files into the folder' +  ' ' + NAME) 
+
+    """
+    BETA_DF = pd.read_csv('RASD_TOOLBOX/beta_df.txt', delimiter = ";",  names = ['PF' ,'BETA'])
+    BETA_APROX = round(P_FVALUE,5)
+    BETA_VALUE_INDEX = (BETA_DF['PF'].sub(P_FVALUE).abs().idxmin())
+    BETA_VALUE = BETA_DF['BETA'][BETA_VALUE_INDEX]   
+    BETA_F.append(BETA_VALUE)
+
+    # Save results
+    RESULTS_REP = {'TOTAL RESULTS': RESULTS_RASD, 'NUMBER OF FAILURES': N_F, 'PROBABILITY OF FAILURE': P_F, 'BETA INDEX': BETA_F}
+    RESULTS.append(RESULTS_REP)
+    NAME = 'RASD_' + MODEL + '_REP_' + str(J) + '_SAMPLES_' + str(N_POP) + '_' + str(datetime.now().strftime('%Y%m%d %H%M%S')) + '.txt'
+    HEADER_NAMES =  ';'.join(COLUMNS_NAMES)
+    np.savetxt(NAME, RESULTS_RASD, fmt = '%1.5f', delimiter = ';' , header = HEADER_NAMES)
+    """
     return RESULTS_RASD
```

### Comparing `PARE_TOOLBOX-2023.6/PARE_TOOLBOX/ZIPPER.py` & `PARE_TOOLBOX-2023.7/PARE_TOOLBOX/ZIPPER.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-import shutil
-import os.path
-import json
-
-
-def LIST_ALL_FILES(PATH = './'):
-    return os.listdir(PATH) 
-
-def FOLDER_CREATOR(NAME, PATH='./'):
-    """
-    You can insert the file name with extension or without extension, don't need the path (The path is the current directory).
-    """
-    
-    if '.json' in NAME or '.txt' in NAME:
-        NAME = NAME.split('.')[0]  
-    FOLDER_NAME = NAME
-    os.mkdir(FOLDER_NAME)
-
-    return PATH + FOLDER_NAME
-
-
-def FOLDER_MOVER(NAME, PATH='./'):
-    """
-    You can insert the file name with extension or without extension, don't need the path (The path is the current directory).
-    """
-    
-    if '.json' in NAME or '.txt' in NAME:
-        NAME = NAME.split('.')[0]
-    FOLDER_NAME = NAME
-    TXT_FILE = NAME + '.txt'
-    JSON_FILE = NAME + '.json'
-    
-    shutil.move(TXT_FILE, PATH + FOLDER_NAME)
-    shutil.move(JSON_FILE, PATH + FOLDER_NAME)
-
-    return PATH + FOLDER_NAME
-
-
-def FOLDER_REMOVER(NAME, PATH='./'):
-    if '.json' in NAME or '.txt' in NAME:
-        NAME = NAME.split('.')[0]
-    
-    shutil.rmtree(NAME)
-    return PATH + NAME
-
-
-def ZIPPER(NAME, PATH = './'):
-    """
-    You can insert the file name with extension or without extension, don't need the path (zipping on the root directory).
-    """
-    
-    FOLDER_CREATOR(NAME)
-    FOLDER_MOVER(NAME)
-
-    if '.json' in NAME or '.txt' in NAME:
-        NAME = NAME.split('.')[0]
-    
-    ZIP_NAME = PATH + NAME
-    shutil.make_archive(ZIP_NAME, 'zip', root_dir = PATH, base_dir=ZIP_NAME, verbose=0, dry_run=False, owner=None, group=None, logger=None)
-    FOLDER_REMOVER(NAME)
-    print('\n \U0001F197'+' Zip file created: ', ZIP_NAME)
-    
-    return PATH + ZIP_NAME
-    
-
-def UNZIPPER(NAME, PATH = './'):
-    """
-    You can insert the file name with extension or without extension, don't need the path (unzipping on the root directory).
-    """
-    if not 'zip' in NAME:
-        NAME = NAME + '.zip'
-
-    shutil.unpack_archive(NAME, PATH, 'zip')
-
-def READ_MCS_LHS_FOLDERS(PATH='./'):
-    FILES = os.listdir(PATH)
-    FOLDERS = []
-    for FILE in FILES:
-        if 'MCS_LHS' in FILE and not '.zip' in FILE:
-            FOLDERS.append(FILE)
-    
-    return FOLDERS
-
-
-def CONCAT_RESULTS(PATH = './'):
-    
-    FOLDERS = READ_MCS_LHS_FOLDERS(PATH)
-    PRINT_TITLE = True
-
-    for FOLDER in FOLDERS:
-        
-        FILES = os.listdir(PATH+FOLDER)
-        JSON_FILE = [FILE for FILE in FILES if '.json' in FILE][0]
-        TXT_FILE = [FILE for FILE in FILES if '.txt' in FILE][0]    
-        
-        with open(PATH+FOLDER+'/'+TXT_FILE) as F:
-            TXT_DATA = F.readlines()
-            
-            with open(PATH + 'concat_result.txt', 'a') as F:
-                if(PRINT_TITLE):
-                    F.writelines(TXT_DATA)
-                    PRINT_TITLE = False
-                else:
-                    TXT_DATA = TXT_DATA[1:]
+import shutil
+import os.path
+import json
+
+
+def LIST_ALL_FILES(PATH = './'):
+    return os.listdir(PATH) 
+
+def FOLDER_CREATOR(NAME, PATH='./'):
+    """
+    You can insert the file name with extension or without extension, don't need the path (The path is the current directory).
+    """
+    
+    if '.json' in NAME or '.txt' in NAME:
+        NAME = NAME.split('.')[0]  
+    FOLDER_NAME = NAME
+    os.mkdir(FOLDER_NAME)
+
+    return PATH + FOLDER_NAME
+
+
+def FOLDER_MOVER(NAME, PATH='./'):
+    """
+    You can insert the file name with extension or without extension, don't need the path (The path is the current directory).
+    """
+    
+    if '.json' in NAME or '.txt' in NAME:
+        NAME = NAME.split('.')[0]
+    FOLDER_NAME = NAME
+    TXT_FILE = NAME + '.txt'
+    JSON_FILE = NAME + '.json'
+    
+    shutil.move(TXT_FILE, PATH + FOLDER_NAME)
+    shutil.move(JSON_FILE, PATH + FOLDER_NAME)
+
+    return PATH + FOLDER_NAME
+
+
+def FOLDER_REMOVER(NAME, PATH='./'):
+    if '.json' in NAME or '.txt' in NAME:
+        NAME = NAME.split('.')[0]
+    
+    shutil.rmtree(NAME)
+    return PATH + NAME
+
+
+def ZIPPER(NAME, PATH = './'):
+    """
+    You can insert the file name with extension or without extension, don't need the path (zipping on the root directory).
+    """
+    
+    FOLDER_CREATOR(NAME)
+    FOLDER_MOVER(NAME)
+
+    if '.json' in NAME or '.txt' in NAME:
+        NAME = NAME.split('.')[0]
+    
+    ZIP_NAME = PATH + NAME
+    shutil.make_archive(ZIP_NAME, 'zip', root_dir = PATH, base_dir=ZIP_NAME, verbose=0, dry_run=False, owner=None, group=None, logger=None)
+    FOLDER_REMOVER(NAME)
+    print('\n \U0001F197'+' Zip file created: ', ZIP_NAME)
+    
+    return PATH + ZIP_NAME
+    
+
+def UNZIPPER(NAME, PATH = './'):
+    """
+    You can insert the file name with extension or without extension, don't need the path (unzipping on the root directory).
+    """
+    if not 'zip' in NAME:
+        NAME = NAME + '.zip'
+
+    shutil.unpack_archive(NAME, PATH, 'zip')
+
+def READ_MCS_LHS_FOLDERS(PATH='./'):
+    FILES = os.listdir(PATH)
+    FOLDERS = []
+    for FILE in FILES:
+        if 'MCS_LHS' in FILE and not '.zip' in FILE:
+            FOLDERS.append(FILE)
+    
+    return FOLDERS
+
+
+def CONCAT_RESULTS(PATH = './'):
+    
+    FOLDERS = READ_MCS_LHS_FOLDERS(PATH)
+    PRINT_TITLE = True
+
+    for FOLDER in FOLDERS:
+        
+        FILES = os.listdir(PATH+FOLDER)
+        JSON_FILE = [FILE for FILE in FILES if '.json' in FILE][0]
+        TXT_FILE = [FILE for FILE in FILES if '.txt' in FILE][0]    
+        
+        with open(PATH+FOLDER+'/'+TXT_FILE) as F:
+            TXT_DATA = F.readlines()
+            
+            with open(PATH + 'concat_result.txt', 'a') as F:
+                if(PRINT_TITLE):
+                    F.writelines(TXT_DATA)
+                    PRINT_TITLE = False
+                else:
+                    TXT_DATA = TXT_DATA[1:]
                     F.writelines(TXT_DATA)
```

### Comparing `PARE_TOOLBOX-2023.6/PARE_TOOLBOX.egg-info/PKG-INFO` & `PARE_TOOLBOX-2023.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.1
-Name: PARE-TOOLBOX
-Version: 2023.6
-Summary: The PAREpy is an easy-to-use environment for applying probabilistic modeling.
-Home-page: https://wmpjrufg.github.io/PAREPY/
-Author: ['Wanderlei Malaquias Pereira Junior', 'Donizetti Aparecido de Souza Junior', 'Romes Antônio Borges', 'Mateus Pereira da Silva']
-Author-email: wanderlei_junior@ufcat.edu.br
-License: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-License-File: license.md
+Metadata-Version: 2.1
+Name: PARE_TOOLBOX
+Version: 2023.7
+Summary: The PAREpy is an easy-to-use environment for applying probabilistic modeling.
+Home-page: https://wmpjrufg.github.io/PAREPY/
+Author: ['Wanderlei Malaquias Pereira Junior', 'Donizetti Aparecido de Souza Junior', 'Romes Antônio Borges', 'Mateus Pereira da Silva']
+Author-email: wanderlei_junior@ufcat.edu.br
+License: MIT License
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+
+UNKNOWN
+
```

### Comparing `PARE_TOOLBOX-2023.6/PKG-INFO` & `PARE_TOOLBOX-2023.7/PARE_TOOLBOX.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-Metadata-Version: 2.1
-Name: PARE_TOOLBOX
-Version: 2023.6
-Summary: The PAREpy is an easy-to-use environment for applying probabilistic modeling.
-Home-page: https://wmpjrufg.github.io/PAREPY/
-Author: ['Wanderlei Malaquias Pereira Junior', 'Donizetti Aparecido de Souza Junior', 'Romes Antônio Borges', 'Mateus Pereira da Silva']
-Author-email: wanderlei_junior@ufcat.edu.br
-License: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-License-File: license.md
+Metadata-Version: 2.1
+Name: PARE-TOOLBOX
+Version: 2023.7
+Summary: The PAREpy is an easy-to-use environment for applying probabilistic modeling.
+Home-page: https://wmpjrufg.github.io/PAREPY/
+Author: ['Wanderlei Malaquias Pereira Junior', 'Donizetti Aparecido de Souza Junior', 'Romes Antônio Borges', 'Mateus Pereira da Silva']
+Author-email: wanderlei_junior@ufcat.edu.br
+License: MIT License
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Education
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+
+UNKNOWN
+
```

### Comparing `PARE_TOOLBOX-2023.6/setup.py` & `PARE_TOOLBOX-2023.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from setuptools import setup, find_packages
-# from pathlib import Path
-# this_directory = Path(__file__).resolve().parent
-# readme_path = this_directory / "readme.md"
-# long_description = readme_path.read_text(encoding = 'utf-8')
-
-setup(
-    	name = 'PARE_TOOLBOX',
-    	version = '2023.6',
-		url = 'https://wmpjrufg.github.io/PAREPY/',
-        description = 'The PAREpy is an easy-to-use environment for applying probabilistic modeling.',
-		# long_description = long_description,
-		# long_description_content_type='text/markdown',   
-    	license = 'MIT License',
-        author = ['Wanderlei Malaquias Pereira Junior', 
-                  'Donizetti Aparecido de Souza Junior', 
-                  'Romes Antônio Borges',
-                  'Mateus Pereira da Silva'],
-    	author_email = 'wanderlei_junior@ufcat.edu.br',
-        install_requires = ["numpy", "scipy", "pandas"],
-		classifiers = [	
-            			'Development Status :: 4 - Beta',
-            			'Topic :: Education',
-                        'Topic :: Scientific/Engineering',
-                        'License :: OSI Approved :: MIT License',
-						'Programming Language :: Python',
-                        ],
-        packages = find_packages()
-     )
-
-# https://pypi.org/classifiers/
+from setuptools import setup, find_packages
+# from pathlib import Path
+# this_directory = Path(__file__).resolve().parent
+# readme_path = this_directory / "readme.md"
+# long_description = readme_path.read_text(encoding = 'utf-8')
+
+setup(
+    	name = 'PARE_TOOLBOX',
+    	version = '2023.7',
+		url = 'https://wmpjrufg.github.io/PAREPY/',
+        description = 'The PAREpy is an easy-to-use environment for applying probabilistic modeling.',
+		# long_description = long_description,
+		# long_description_content_type='text/markdown',   
+    	license = 'MIT License',
+        author = ['Wanderlei Malaquias Pereira Junior', 
+                  'Donizetti Aparecido de Souza Junior', 
+                  'Romes Antônio Borges',
+                  'Mateus Pereira da Silva'],
+    	author_email = 'wanderlei_junior@ufcat.edu.br',
+        install_requires = ["numpy", "scipy", "pandas"],
+		classifiers = [	
+            			'Development Status :: 4 - Beta',
+            			'Topic :: Education',
+                        'Topic :: Scientific/Engineering',
+                        'License :: OSI Approved :: MIT License',
+						'Programming Language :: Python',
+                        ],
+        packages = find_packages()
+     )
+
+# https://pypi.org/classifiers/
 # https://www.alura.com.br/artigos/como-publicar-seu-codigo-python-no-pypi
```

