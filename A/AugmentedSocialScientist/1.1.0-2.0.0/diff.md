# Comparing `tmp/AugmentedSocialScientist-1.1.0.tar.gz` & `tmp/AugmentedSocialScientist-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AugmentedSocialScientist-1.1.0.tar", last modified: Sun Jul 23 23:36:21 2023, max compression
+gzip compressed data, was "AugmentedSocialScientist-2.0.0.tar", last modified: Fri Jul 28 15:30:17 2023, max compression
```

## Comparing `AugmentedSocialScientist-1.1.0.tar` & `AugmentedSocialScientist-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,18 @@
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-23 23:36:21.677699 AugmentedSocialScientist-1.1.0/
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-23 23:36:21.673166 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/
--rw-r--r--   0 rubing     (501) staff       (20)    16710 2023-07-23 23:08:49.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/arabic_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16696 2023-07-14 20:35:01.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16751 2023-07-14 20:34:59.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/camembert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16696 2023-07-23 23:15:49.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/chinese_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16728 2023-07-14 20:34:58.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/german_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16706 2023-07-23 23:18:30.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/hindi_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16726 2023-07-23 23:11:56.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/italian_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16736 2023-07-23 23:10:31.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/portuguese_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16725 2023-07-23 23:14:58.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/russian_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16747 2023-07-14 20:34:57.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/spanish_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16714 2023-07-23 23:12:48.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/swedish_bert.py
--rw-r--r--   0 rubing     (501) staff       (20)    16756 2023-07-14 20:34:54.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/xlmroberta.py
-drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-23 23:36:21.677238 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/
--rw-r--r--   0 rubing     (501) staff       (20)     2535 2023-07-23 23:36:20.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)      800 2023-07-23 23:36:21.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/SOURCES.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-23 23:36:20.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/dependency_links.txt
--rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-23 23:36:20.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/not-zip-safe
--rw-r--r--   0 rubing     (501) staff       (20)       92 2023-07-23 23:36:21.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/requires.txt
--rw-r--r--   0 rubing     (501) staff       (20)       25 2023-07-23 23:36:21.000000 AugmentedSocialScientist-1.1.0/AugmentedSocialScientist.egg-info/top_level.txt
--rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-1.1.0/LICENSE
--rw-r--r--   0 rubing     (501) staff       (20)     2535 2023-07-23 23:36:21.677885 AugmentedSocialScientist-1.1.0/PKG-INFO
--rw-r--r--   0 rubing     (501) staff       (20)     2070 2023-07-23 23:36:07.000000 AugmentedSocialScientist-1.1.0/README.md
--rw-r--r--   0 rubing     (501) staff       (20)       79 2023-07-23 23:36:21.679037 AugmentedSocialScientist-1.1.0/setup.cfg
--rw-r--r--   0 rubing     (501) staff       (20)      910 2023-07-23 23:20:42.000000 AugmentedSocialScientist-1.1.0/setup.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 15:30:17.049722 AugmentedSocialScientist-2.0.0/
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 15:30:17.046973 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/
+-rw-r--r--   0 rubing     (501) staff       (20)      434 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/__init__.py
+-rw-r--r--   0 rubing     (501) staff       (20)     1221 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/bert_abc.py
+-rw-r--r--   0 rubing     (501) staff       (20)    19661 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/bert_base.py
+-rw-r--r--   0 rubing     (501) staff       (20)     4184 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/models.py
+drwxr-xr-x   0 rubing     (501) staff       (20)        0 2023-07-28 15:30:17.049360 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/
+-rw-r--r--   0 rubing     (501) staff       (20)     5723 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)      469 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/SOURCES.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/dependency_links.txt
+-rw-r--r--   0 rubing     (501) staff       (20)        1 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/not-zip-safe
+-rw-r--r--   0 rubing     (501) staff       (20)       63 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/requires.txt
+-rw-r--r--   0 rubing     (501) staff       (20)       25 2023-07-28 15:30:16.000000 AugmentedSocialScientist-2.0.0/AugmentedSocialScientist.egg-info/top_level.txt
+-rw-r--r--   0 rubing     (501) staff       (20)     1068 2023-07-14 19:52:59.000000 AugmentedSocialScientist-2.0.0/LICENSE
+-rw-r--r--   0 rubing     (501) staff       (20)     5723 2023-07-28 15:30:17.049900 AugmentedSocialScientist-2.0.0/PKG-INFO
+-rw-r--r--   0 rubing     (501) staff       (20)     5257 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/README.md
+-rw-r--r--   0 rubing     (501) staff       (20)       79 2023-07-28 15:30:17.050623 AugmentedSocialScientist-2.0.0/setup.cfg
+-rw-r--r--   0 rubing     (501) staff       (20)      853 2023-07-28 15:26:16.000000 AugmentedSocialScientist-2.0.0/setup.py
```

### Comparing `AugmentedSocialScientist-1.1.0/AugmentedSocialScientist/arabic_bert.py` & `AugmentedSocialScientist-2.0.0/AugmentedSocialScientist/bert_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,453 +1,516 @@
-import os
-import time
 import datetime
 import random
-from tqdm.auto import tqdm
-import pandas as pd
-import numpy as np
-from scipy.special import softmax
-from nltk.tokenize import sent_tokenize
-
-from sklearn.model_selection import train_test_split
-from sklearn.metrics import classification_report,precision_recall_fscore_support
+import time
+import os
 
+import numpy as np
 import torch
-from torch.utils.data import TensorDataset, DataLoader, RandomSampler, SequentialSampler
-from tensorflow.keras.preprocessing.sequence import pad_sequences
-from transformers import BertTokenizer, BertConfig,\
-                         BertForSequenceClassification,\
-                         AdamW, get_linear_schedule_with_warmup,\
-                         WEIGHTS_NAME, CONFIG_NAME
-
-# If there's a GPU available...
-if torch.cuda.is_available():
-
-    # Tell PyTorch to use the GPU.
-    device = torch.device("cuda")
-
-    print('There are %d GPU(s) available.' % torch.cuda.device_count())
-
-    print('We will use GPU {}:'.format(torch.cuda.current_device()), torch.cuda.get_device_name(torch.cuda.current_device()))
-
-# If not...
-else:
-    print('No GPU available, using the CPU instead.')
-    device = torch.device("cpu")
-
-
-tokenizer = BertTokenizer.from_pretrained("asafaya/bert-base-arabic")
-
-def encode(sentences, labels=None, tokenizer=tokenizer, batch_size=32, progress_bar=True):
-    """
-    Preprocessing of the training, test or prediction data.
-    The function will:
-        (1) tokenize the sentences and map tokens to theirs IDs;
-        (2) truncate or pad to 512 tokens (limit for BERT), create corresponding attention masks;
-        (3) return a pytorch dataloader object containing token ids, labels and attention masks.
-        
-    Parameters
-    ----------
-    sentences: 1D array-like
-        list of texts
-    
-    labels: 1D array-like or None, default=None
-        list of labels. None for unlabelled prediction data
-    
-    tokenizer: huggingface tokenizer, default=BertTokenizer.from_pretrained('bert-base-uncased')
-        tokenizer to use
-    
-    batch_size: int, default=32
-        batch size for pytorch dataloader
-    
-    progress_bar: bool, default=True
-        if True, print progress bar for the processing
-        
-        
-    Return
-    ------
-    dataloader:
-        pytorch dataloader object containing token ids, labels and attention masks
-    
-    """
-    input_ids = []
-    if progress_bar:
-        sent_loader = tqdm(sentences)
-    else:
-        sent_loader = sentences
-    for sent in sent_loader:
-        # `encode` will:
-        #   (1) Tokenize the sentence.
-        #   (2) Prepend the `[CLS]` token to the start.
-        #   (3) Append the `[SEP]` token to the end.
-        #   (4) Map tokens to their IDs.  
-        encoded_sent = tokenizer.encode(sent,                       # Sentence to encode.
-                                        add_special_tokens = True   # Add '[CLS]' and '[SEP]'
-                                        #max_length = 128,          # Truncate all sentences.
-                                        #return_tensors = 'pt',     # Return pytorch tensors.
-                                       )
-        input_ids.append(encoded_sent)
-        
-    MAX_LEN = min(max([len(sen) for sen in input_ids]), 512)
-
-    # Pad our input tokens with value 0.
-    # "post" indicates that we want to pad and truncate at the end of the sequence, as opposed to the beginning.
-    input_ids = pad_sequences(input_ids, maxlen=MAX_LEN, dtype="long", 
-                              value=0, truncating="post", padding="post")
-
-    # Create attention masks
-    attention_masks = []
-    if progress_bar:
-        input_loader = tqdm(input_ids)
-    else:
-        input_loader = input_ids
-    for sent in input_loader:
-        # Create the attention mask.
-        #   - If a token ID is 0, then it's padding, set the mask to 0.
-        #   - If a token ID is > 0, then it's a real token, set the mask to 1.
-        att_mask = [int(token_id > 0) for token_id in sent]
-
-        attention_masks.append(att_mask)
-    
-    if labels is None:
-        # Convert to pytorch tensors
-        inputs_tensors = torch.tensor(input_ids)
-        masks_tensors = torch.tensor(attention_masks)
-
-        # Create the DataLoader 
-        data = TensorDataset(inputs_tensors, masks_tensors)
-        sampler = SequentialSampler(data)
-        dataloader = DataLoader(data, sampler=sampler, batch_size=batch_size)
-        return dataloader        
-    else:
-        # Convert to pytorch tensors
-        inputs_tensors = torch.tensor(input_ids)
-        masks_tensors = torch.tensor(attention_masks)
-        labels_tensors = torch.tensor(labels)
-
-        # Create the DataLoader 
-        data = TensorDataset(inputs_tensors, masks_tensors, labels_tensors)
-        sampler = SequentialSampler(data)
-        dataloader = DataLoader(data, sampler=sampler, batch_size=batch_size)
-        return dataloader
-    
-def format_time(elapsed):
-    elapsed_rounded = int(round((elapsed)))
-    return str(datetime.timedelta(seconds=elapsed_rounded)) # Format as hh:mm:ss
-
-def run_training(train_dataloader, 
-                 test_dataloader, 
-                 n_epochs=3, 
-                 lr=5e-5, 
-                 random_state=2018,
-                 save_model_as=None):
-    """
-    Train, evaluate and save a BERT model
-    
-    Parameters
-    ----------
-    train_dataloader: dataloader
-        training dataloader obtained with encode()
-    
-    test_dataloader: dataloader
-        test dataloader obtained with encode()
-        
-    n_epochs: int, default=3
-        number of epochs
-        
-    lr: float, default=5e-5
-        learning rate
-        
-    random state: int, default=2018
-        random state (for replicability)
-        
-    save_model_as: str, default=None
-        the name of model saving folder. The model will be saved at ./models/<model_name>. If None, not saving the model after training
-       
-       
-    Return
-    ------
-    score: ndarray
-        evaluation scores of the model: precision, recall, f1-score and support for each category
-    """
-    
-    # Unpack all test labels for evaluation
-    test_labels = []
-    for batch in test_dataloader:
-        test_labels += batch[2].numpy().tolist()
-    num_labels = np.unique(test_labels).size
-    assert set(test_labels)==set(range(len(np.unique(test_labels)))), "The labels should be integers starting from 0: 0, 1, 2,..."
-
-    # Set the seed value all over the place to make this reproducible.
-    random.seed(random_state)
-    np.random.seed(random_state)
-    torch.manual_seed(random_state)
-    torch.cuda.manual_seed_all(random_state)
-    
-    # Load model
-    model = BertForSequenceClassification.from_pretrained("asafaya/bert-base-arabic", 
-                                                               num_labels = num_labels, 
-                                                               output_attentions = False, 
-                                                               output_hidden_states = False)
-    # Tell pytorch to run this model on the GPU.
-    if torch.cuda.is_available():
-        model.cuda()
-        
-    optimizer = AdamW(model.parameters(), lr = lr, eps = 1e-8)
-    # Create the learning rate scheduler.
-    scheduler = get_linear_schedule_with_warmup(optimizer,
-                                                num_warmup_steps=0,
-                                                num_training_steps=len(train_dataloader) * n_epochs)
-    #total number of training steps is number of batches * number of epochs.
-
-    # Store the average loss after each epoch so we can plot them.
-    train_loss_values = []
-    test_loss_values = []
-    
-    for i_epoch in range(n_epochs):
-    # each epoch
-        # ========================================
-        #               Training
-        # ========================================
-        # Perform one full pass over the training set.
-        
-        print("")
-        print('======== Epoch {:} / {:} ========'.format(i_epoch + 1, n_epochs))
-        print('Training...')
+from scipy.special import softmax
+from torch.utils.data import TensorDataset, SequentialSampler, DataLoader
+from tqdm.auto import tqdm
+from sklearn.metrics import classification_report, precision_recall_fscore_support
+from transformers import BertForSequenceClassification, BertTokenizer, AdamW, get_linear_schedule_with_warmup,\
+                            WEIGHTS_NAME, CONFIG_NAME
+
+from AugmentedSocialScientist.bert_abc import BertABC
+
+
+class BertBase(BertABC):
+    def __init__(
+            self,
+            model_name='bert-base-uncased',
+            tokenizer=BertTokenizer,
+            model_sequence_classifier=BertForSequenceClassification,
+            device=None,
+
+    ):
+        """
+            Parameters
+            ----------
+            model_name: str, default='bert-base-uncased'
+                    a model name from huggingface models: https://huggingface.co/models
+
+            tokenizer: huggingface tokenizer, default=BertTokenizer.from_pretrained('bert-base-uncased')
+                    tokenizer to use
+
+            model_sequence_classifier: huggingface sequence classifier, default=BertForSequenceClassification
+                    a huggingface sequence classifier that implements a from_pretrained() function
+
+            device: torch.Device, default=None
+                    device to use. If None, automatically set if presence of GPU is detected. CPU otherwise. 
+        """
+        self.model_name = model_name
+        self.tokenizer = tokenizer.from_pretrained(self.model_name)
+        self.model_sequence_classifier = model_sequence_classifier
+        self.dict_labels = None
+
+        # Users can set their device (flexibility),
+        # but device is set by default in case users are not familiar with Pytorch
+        self.device = device
+        if self.device is None:
+            # If there's a GPU available...
+            if torch.cuda.is_available():
+                # Tell PyTorch to use the GPU.
+                self.device = torch.device("cuda")
+                print('There are %d GPU(s) available.' % torch.cuda.device_count())
+                print('We will use GPU {}:'.format(torch.cuda.current_device()),
+                      torch.cuda.get_device_name(torch.cuda.current_device()))
+            # If not...
+            else:
+                self.device = torch.device("cpu")
+                print('No GPU available, using the CPU instead.')
+
+    def encode(
+            self,
+            sequences,
+            labels=None,
+            batch_size=32,
+            progress_bar=True
+    ):
+        """
+            Preprocessing of the training, test or prediction data.
+            The function will:
+                (1) tokenize the sequences and map tokens to theirs IDs;
+                (2) truncate or pad to 512 tokens (limit for BERT), create corresponding attention masks;
+                (3) return a pytorch dataloader object containing token ids, labels and attention masks.
+
+            Parameters
+            ----------
+            sequences: 1D array-like
+                list of texts
+
+            labels: 1D array-like or None, default=None
+                list of labels. None for unlabelled prediction data
+
+            batch_size: int, default=32
+                batch size for pytorch dataloader
+
+            progress_bar: bool, default=True
+                if True, print progress bar for the processing
+
+
+            Return
+            ------
+            dataloader:
+                pytorch dataloader object containing token ids, labels and attention masks
+
+            """
+        input_ids = []
+        if progress_bar:
+            sent_loader = tqdm(sequences)
+        else:
+            sent_loader = sequences
+        for sent in sent_loader:
+            # `encode` will:
+            #   (1) Tokenize the sequence.
+            #   (2) Prepend the `[CLS]` token to the start.
+            #   (3) Append the `[SEP]` token to the end.
+            #   (4) Map tokens to their IDs.
+            encoded_sent = self.tokenizer.encode(sent,  # Sequence to encode.
+                                            add_special_tokens=True  # Add '[CLS]' and '[SEP]'
+                                            # max_length = 128,          # Truncate all sequences.
+                                            # return_tensors = 'pt',     # Return pytorch tensors.
+                                            )
+            input_ids.append(encoded_sent)
+
+        max_len = min(max([len(sen) for sen in input_ids]), 512)
+
+        # Pad the input tokens with value 0 and truncate to MAX_LEN
+        pad = np.full((len(input_ids), max_len), 0, dtype='long')
+        for idx, s in enumerate(input_ids):
+            trunc = s[:max_len]
+            pad[idx, :len(trunc)] = trunc
+
+        input_ids = pad 
+
+        # Create attention masks
+        attention_masks = []
+        if progress_bar:
+            input_loader = tqdm(input_ids)
+        else:
+            input_loader = input_ids
+        for sent in input_loader:
+            # Create the attention mask.
+            #   - If a token ID is 0, then it's padded, set the mask to 0.
+            #   - If a token ID is > 0, then it's a real token, set the mask to 1.
+            att_mask = [int(token_id > 0) for token_id in sent]
+
+            attention_masks.append(att_mask)
+
+        if labels is None:
+            # Convert to pytorch tensors
+            inputs_tensors = torch.tensor(input_ids)
+            masks_tensors = torch.tensor(attention_masks)
+
+            # Create the DataLoader
+            data = TensorDataset(inputs_tensors, masks_tensors)
+            sampler = SequentialSampler(data)
+            dataloader = DataLoader(data, sampler=sampler, batch_size=batch_size)
+            return dataloader
+        else:
 
-        # Measure how long the training epoch takes.
-        t0 = time.time()
+            label_names = np.unique(labels) # unique label names in alphabetical order
+            self.dict_labels = dict(zip(label_names, range(len(label_names))))
 
-        # Reset the total train loss for this epoch.
-        total_train_loss = 0
-        total_test_loss = 0  # Reset the total train loss for this epoch.
-
-
-        # Put the model in training mode
-        model.train()
-
-        for step, train_batch in enumerate(train_dataloader):
-        # each batch
-            # Progress update every 40 batches.
-            if step % 40 == 0 and not step == 0:
-                # Calculate elapsed time in minutes.
-                elapsed = format_time(time.time() - t0)
-                # Report progress.
-                print('  Batch {:>5,}  of  {:>5,}.    Elapsed: {:}.'.format(step, len(train_dataloader), elapsed))
-
-            b_inputs = train_batch[0].to(device)
-            b_masks = train_batch[1].to(device)
-            b_labels = train_batch[2].to(device)
-
-            # Clear any previously calculated gradients before performing a
-            model.zero_grad()        
-
-            # Perform a forward pass (evaluate the model on this training batch).
-            # This will return the loss (rather than the model output) because we have provided the `labels`.
-            outputs = model(b_inputs, token_type_ids=None, attention_mask=b_masks,labels=b_labels)
-
-            # The call to `model` always returns a tuple, so we need to pull the loss value out of the tuple.
-            loss = outputs[0]
-
-            # Accumulate the training loss over all of the batches so that we can
-            # calculate the average loss at the end. `loss` is a Tensor containing a
-            # single value; the `.item()` function just returns the Python value 
-            # from the tensor.
-            total_train_loss += loss.item()
-
-            # Perform a backward pass to calculate the gradients.
-            loss.backward()
-
-            # Clip the norm of the gradients to 1. This is to help prevent the "exploding gradients" problem.
-            torch.nn.utils.clip_grad_norm_(model.parameters(), 1.0)
-
-            # Update parameters and take a step using the computed gradient.
-            optimizer.step()
-
-            # Update the learning rate.
-            scheduler.step()
-            
-            
-        # Calculate the average loss over the training data batches.
-        avg_train_loss = total_train_loss / len(train_dataloader)            
+            print(f"label ids: {self.dict_labels}")
 
-        # Store the loss value for plotting the learning curve.
-        train_loss_values.append(avg_train_loss)
+            # Convert to pytorch tensors
+            inputs_tensors = torch.tensor(input_ids)
+            masks_tensors = torch.tensor(attention_masks)
+            labels_tensors = torch.tensor([self.dict_labels[x] for x in labels])
+
+            # Create the DataLoader
+            data = TensorDataset(inputs_tensors, masks_tensors, labels_tensors)
+            sampler = SequentialSampler(data)
+            dataloader = DataLoader(data, sampler=sampler, batch_size=batch_size)
+            return dataloader
+
+    def run_training(
+            self,
+            train_dataloader,
+            test_dataloader,
+            n_epochs=3,
+            lr=5e-5,
+            random_state=42,
+            save_model_as=None
+    ):
+        """
+            Train, evaluate and save a BERT model.
+
+            Parameters
+            ----------
+            train_dataloader: torch.Dataloader 
+                training dataloader obtained with self.encode()
+
+            test_dataloader: torch.Dataloader 
+                test dataloader obtained with self.encode()
+
+            n_epochs: int, default=3
+                number of epochs
+
+            lr: float, default=5e-5
+                learning rate
+
+            random_state: int, default=42
+                random state (for replicability)
+
+            save_model_as: str, default=None
+                name of model to save as. The model will be saved at ./models/<model_name>. If None, not saving the model after training
+
+
+            Return
+            ------
+            scores: tuplet, 4 arrays of shape (n_labels,)
+                evaluation scores: precision, recall, f1-score and support for each label
+            """
+
+        # Unpack all test labels for evaluation
+        test_labels = []
+        for batch in test_dataloader:
+            test_labels += batch[2].numpy().tolist()
+        num_labels = np.unique(test_labels).size
 
-        print("")
-        print("  Average training loss: {0:.2f}".format(avg_train_loss))
-        print("  Training took: {:}".format(format_time(time.time() - t0)))
+        if self.dict_labels is None:
+            label_names = None
+        else:
+            label_names = [str(x[0]) for x in sorted(self.dict_labels.items(), key=lambda x: x[1])]
 
-        # ========================================
-        #               Validation
-        # ========================================
-        # After the completion of each training epoch, measure our performance on our validation set.
+        # Set the seed value all over the place to make this reproducible.
+        random.seed(random_state)
+        np.random.seed(random_state)
+        torch.manual_seed(random_state)
+        torch.cuda.manual_seed_all(random_state)
+
+        # Load model
+        model = self.model_sequence_classifier.from_pretrained(self.model_name,
+                                                               num_labels=num_labels,
+                                                               output_attentions=False,
+                                                               output_hidden_states=False)
+
+        # Tell pytorch to run this model on the GPU.
+        if torch.cuda.is_available():
+            model.cuda()
+
+        optimizer = AdamW(model.parameters(), lr=lr, eps=1e-8)
+        # Create the learning rate scheduler.
+        scheduler = get_linear_schedule_with_warmup(optimizer,
+                                                    num_warmup_steps=0,
+                                                    num_training_steps=len(train_dataloader) * n_epochs)
+        # total number of training steps is number of batches * number of epochs.
+
+        # Store the average loss after each epoch so we can plot them.
+        train_loss_values = []
+        test_loss_values = []
+
+        for i_epoch in range(n_epochs):
+            # each epoch
+            # ========================================
+            #               Training
+            # ========================================
+            # Perform one full pass over the training set.
+
+            print("")
+            print('======== Epoch {:} / {:} ========'.format(i_epoch + 1, n_epochs))
+            print('Training...')
+
+            # Measure how long the training epoch takes.
+            t0 = time.time()
+
+            # Reset the total train loss for this epoch.
+            total_train_loss = 0
+            total_test_loss = 0  # Reset the total train loss for this epoch.
+
+            # Put the model in training mode
+            model.train()
+
+            for step, train_batch in enumerate(train_dataloader):
+                # each batch
+                # Progress update every 40 batches.
+                if step % 40 == 0 and not step == 0:
+                    # Calculate elapsed time in minutes.
+                    elapsed = self.format_time(time.time() - t0)
+                    # Report progress.
+                    print('  Batch {:>5,}  of  {:>5,}.    Elapsed: {:}.'.format(step, len(train_dataloader), elapsed))
+
+                b_inputs = train_batch[0].to(self.device)
+                b_masks = train_batch[1].to(self.device)
+                b_labels = train_batch[2].to(self.device)
+
+                # Clear any previously calculated gradients before performing a
+                model.zero_grad()
+
+                # Perform a forward pass (evaluate the model on this training batch).
+                # This will return the loss (rather than the model output) because we have provided the `labels`.
+                outputs = model(b_inputs, token_type_ids=None, attention_mask=b_masks, labels=b_labels)
+
+                # The call to `model` always returns a tuple, so we need to pull the loss value out of the tuple.
+                loss = outputs[0]
+
+                # Accumulate the training loss over all of the batches so that we can
+                # calculate the average loss at the end. `loss` is a Tensor containing a
+                # single value; the `.item()` function just returns the Python value
+                # from the tensor.
+                total_train_loss += loss.item()
+
+                # Perform a backward pass to calculate the gradients.
+                loss.backward()
+
+                # Clip the norm of the gradients to 1. This is to help prevent the "exploding gradients" problem.
+                torch.nn.utils.clip_grad_norm_(model.parameters(), 1.0)
+
+                # Update parameters and take a step using the computed gradient.
+                optimizer.step()
+
+                # Update the learning rate.
+                scheduler.step()
+
+            # Calculate the average loss over the training data batches.
+            avg_train_loss = total_train_loss / len(train_dataloader)
+
+            # Store the loss value for plotting the learning curve.
+            train_loss_values.append(avg_train_loss)
+
+            print("")
+            print("  Average training loss: {0:.2f}".format(avg_train_loss))
+            print("  Training took: {:}".format(self.format_time(time.time() - t0)))
+
+            # ========================================
+            #               Validation
+            # ========================================
+            # After the completion of each training epoch, measure our performance on our validation set.
+
+            print("")
+            print("Running Validation...")
+
+            t0 = time.time()
+
+            # Put the model in evaluation mode--the dropout layers behave differently during evaluation.
+            model.eval()
+
+            logits_complete = []  # store logits of each batch
+
+            # Evaluate data for one epoch
+            for test_batch in test_dataloader:
+                # Add batch to GPU
+                b_inputs = test_batch[0].to(self.device)
+                b_masks = test_batch[1].to(self.device)
+                b_labels = test_batch[2].to(self.device)
+
+                # Telling the model not to compute or store gradients, saving memory and speeding up validation
+                with torch.no_grad():
+                    # Forward pass, calculate test loss and logit predictions.
+                    # token_type_ids = None : it's not 2-sentences task
+                    outputs = model(b_inputs, token_type_ids=None, attention_mask=b_masks, labels=b_labels)
+
+                loss = outputs[0].item()  # get loss
+                logits = outputs[1]  # get logits
+
+                # Move logits CPU
+                logits = logits.detach().cpu().numpy()
+                # labels_id = b_labels.to('cpu').numpy()
+
+                total_test_loss += loss
+                logits_complete.append(logits)
+
+            logits_complete = np.concatenate(logits_complete)
+
+            # Calculate the average loss over the test data batches.
+            avg_test_loss = total_test_loss / len(test_dataloader)
+            # Store the loss value for plotting the learning curve.
+            test_loss_values.append(avg_test_loss)
+
+            print("")
+            print("  Average test loss: {0:.2f}".format(avg_test_loss))
+            print("  Validation took: {:}".format(self.format_time(time.time() - t0)))
+            print(classification_report(test_labels, np.argmax(logits_complete, axis=1).flatten(), target_names = label_names))
+            scores = precision_recall_fscore_support(test_labels, np.argmax(logits_complete, axis=1).flatten())
 
+        # End of all epochs
         print("")
-        print("Running Validation...")
+        print("Training complete!")
 
-        t0 = time.time()
-
-        # Put the model in evaluation mode--the dropout layers behave differently during evaluation.
-        model.eval()
+        if save_model_as is not None:
+            # SAVE
+            output_dir = "./models/{}".format(save_model_as)
+            try:
+                os.makedirs(output_dir)
+            except:
+                pass
+            # Step 1: Save a model, configuration and vocabulary that you have fine-tuned
+
+            # If we have a distributed model, save only the encapsulated model
+            # (it was wrapped in PyTorch DistributedDataParallel or DataParallel)
+            model_to_save = model.module if hasattr(model, 'module') else model
+
+            # If we save using the predefined names, we can load using `from_pretrained`
+            output_model_file = os.path.join(output_dir, WEIGHTS_NAME)
+            output_config_file = os.path.join(output_dir, CONFIG_NAME)
+
+            torch.save(model_to_save.state_dict(), output_model_file)
+            model_to_save.config.to_json_file(output_config_file)
+            self.tokenizer.save_vocabulary(output_dir)
+
+        return scores
+
+
+    def predict(
+            self,
+            dataloader,
+            model,
+            proba=True,
+            progress_bar=True
+    ):
+        """
+        Prediction with a trained model.
+
+        Parameters
+        ----------
+        dataloader: torch.Dataloader 
+            prediction dataloader obtained with self.encode()
+
+        model: huggingface model
+            trained model
+
+        proba: bool, default=True
+            if True, return prediction probabilites; else, return logits
+
+        progress_bar: bool, defalut=True
+            if True, print progress bar of prediction
+
+        Return
+        ------
+        pred: ndarray of shape (n_samples, n_labels)
+            probabilities for each sequence (row) of belonging to each category (column)
+        """
+        logits_complete = []
+        # Evaluate data for one epoch
+        if progress_bar:
+            loader = tqdm(dataloader)
+        else:
+            loader = dataloader
 
-        logits_complete = [] # store logits of each batch
+        pred = None
+        for batch in loader:
 
-        # Evaluate data for one epoch
-        for test_batch in test_dataloader:
             # Add batch to GPU
-            b_inputs = test_batch[0].to(device)
-            b_masks = test_batch[1].to(device)
-            b_labels = test_batch[2].to(device)
-
-            # Telling the model not to compute or store gradients, saving memory and speeding up validation
-            with torch.no_grad():        
-                # Forward pass, calculate test loss and logit predictions.
-                # token_type_ids = None : it's not 2-sentences task
-                outputs = model(b_inputs, token_type_ids=None, attention_mask=b_masks,labels=b_labels)
-
-            loss = outputs[0].item() # get loss
-            logits = outputs[1]      # get logits
-            
-            # Move logits CPU
+            batch = tuple(t.to(self.device) for t in batch)
+
+            # Unpack the inputs from our dataloader
+            if len(batch) == 3:
+                b_input_ids, b_input_mask, _ = batch
+            else:
+                b_input_ids, b_input_mask = batch
+
+            # Telling the model not to compute or store gradients, saving memory andspeeding up validation
+            with torch.no_grad():
+                outputs = model(b_input_ids,
+                                token_type_ids=None,  # not a 2-sentence task
+                                attention_mask=b_input_mask)
+
+            # Get the "logits" output by the model. The "logits" are the output
+            # values prior to applying an activation function like the softmax.
+            logits = outputs[0]
+            # Move logits and labels to CPU
             logits = logits.detach().cpu().numpy()
-            #labels_id = b_labels.to('cpu').numpy()
-            
-            total_test_loss += loss
             logits_complete.append(logits)
-            
-        logits_complete = np.concatenate(logits_complete)
-        
-        # Calculate the average loss over the test data batches.
-        avg_test_loss = total_test_loss / len(test_dataloader)            
-        # Store the loss value for plotting the learning curve.
-        test_loss_values.append(avg_test_loss)
-        
-        print("")
-        print("  Average test loss: {0:.2f}".format(avg_test_loss))
-        print("  Validation took: {:}".format(format_time(time.time() - t0)))
-        print(classification_report(test_labels, np.argmax(logits_complete, axis=1).flatten()))
-        score = precision_recall_fscore_support(test_labels, np.argmax(logits_complete, axis=1).flatten())
-
-
-    
-        
-    # End of all epochs
-    print("")
-    print("Training complete!")
-    
-    
-    if save_model_as is not None:
-        # SAVE
-        output_dir = "./models/{}".format(save_model_as)
-        try:
-            os.makedirs(output_dir)
-        except:
-            pass
-        # Step 1: Save a model, configuration and vocabulary that you have fine-tuned
-
-        # If we have a distributed model, save only the encapsulated model
-        # (it was wrapped in PyTorch DistributedDataParallel or DataParallel)
-        model_to_save = model.module if hasattr(model, 'module') else model
-
-        # If we save using the predefined names, we can load using `from_pretrained`
-        output_model_file = os.path.join(output_dir, WEIGHTS_NAME)
-        output_config_file = os.path.join(output_dir, CONFIG_NAME)
-
-        torch.save(model_to_save.state_dict(), output_model_file)
-        model_to_save.config.to_json_file(output_config_file)
-        tokenizer.save_vocabulary(output_dir)
-
-
-    return score
-
-
-def predict(dataloader, model, proba=True, progress_bar=True):
-    """
-    Prediction with a trained model. 
-    
-    Parameters
-    ----------
-    dataloader: dataloader
-        prediction dataloader obtained with encode()
-        
-    model: huggingface model
-        trained model
-        
-    proba: bool, default=True
-        if True, return prediction probabilites; else, return logits
-    
-    progress_bar: bool, defalut=True
-        if True, print progress bar of prediction
-    
-    Return
-    ------
-    pred: ndarray of shape (n_samples, n_labels)
-        probabilities for each sentence (row) of belonging to each category (column)
-    """
-    logits_complete = []
-    # Evaluate data for one epoch
-    if progress_bar:
-        loader = tqdm(dataloader)
-    else:
-        loader = dataloader
-    for batch in loader:
-        
-        # Add batch to GPU
-        batch = tuple(t.to(device) for t in batch)
-
-        # Unpack the inputs from our dataloader
-        if len(batch)==3:
-            b_input_ids, b_input_mask, _ = batch
-        else:
-            b_input_ids, b_input_mask = batch
 
+            del outputs
+            torch.cuda.empty_cache()  # release GPU memory
+
+        pred = np.concatenate(logits_complete)  # flatten batches
+        print(f"label ids: {self.dict_labels}")
+
+        return softmax(pred, axis=1) if proba else pred
 
-        # Telling the model not to compute or store gradients, saving memory andspeeding up validation
-        with torch.no_grad():        
-            outputs = model(b_input_ids, 
-                            token_type_ids=None,  # not a 2-sentence task
-                            attention_mask=b_input_mask)
-
-        # Get the "logits" output by the model. The "logits" are the output
-        # values prior to applying an activation function like the softmax.
-        logits = outputs[0]
-        # Move logits and labels to CPU
-        logits = logits.detach().cpu().numpy()
-        logits_complete.append(logits)
-        
-        del outputs        
-        torch.cuda.empty_cache() #release GPU memory
-        
-        pred = np.concatenate(logits_complete) #flatten batches
-    if proba:
-        return softmax(pred, axis=1)
-    else:
-        return pred
-    
-def predict_with_model(dataloader, model_path, proba=True, progress_bar=True):
-    """
-    Prediction with a locally saved model. 
-    
-    Parameters
-    ----------
-    dataloader: dataloader
-        prediction dataloader obtained with encode()
-        
-    model_path: str
-        path to the saved model
-        
-    proba: bool, default=True
-        if True, return prediction probabilites; else, return logits
-    
-    progress_bar: bool, defalut=True
-        if True, print progress bar of prediction
-    
-    Return
-    ------
-    pred: ndarray of shape (n_samples, n_labels)
-        probabilities for each sentence (row) of belonging to each category (column)
-    """
-    model = BertForSequenceClassification.from_pretrained(model_path)
-    if torch.cuda.is_available():
-        model.cuda()
-    return predict(dataloader, model, proba, progress_bar)
+    def predict_with_model(
+            self,
+            dataloader,
+            model_path,
+            proba=True,
+            progress_bar=True
+    ):
+        """
+        Prediction with a locally saved model.
+
+        Parameters
+        ----------
+        dataloader: torch.Dataloader 
+            prediction dataloader obtained with self.encode()
+
+        model_path: str
+            path to the saved model
+
+        proba: bool, default=True
+            if True, return prediction probabilites; else, return logits
+
+        progress_bar: bool, defalut=True
+            if True, print progress bar of prediction
+
+        Return
+        ------
+        pred: ndarray of shape (n_samples, n_labels)
+            probabilities for each sequence (row) of belonging to each category (column)
+        """
+        model = self.model_sequence_classifier.from_pretrained(model_path)
+        if torch.cuda.is_available():
+            model.cuda()
+        return self.predict(dataloader, model, proba, progress_bar)
+
+ 
+    def format_time(
+            self,
+            elapsed: float | int
+    ):
+        """
+        Format a time to hh:mm:ss.
+
+        Parameters
+        ----------
+        elapsed: float, elapsed time
+
+        Returns
+        -------
+
+        """
+        elapsed_rounded = int(round(elapsed))
+        return str(datetime.timedelta(seconds=elapsed_rounded))  # Format as hh:mm:ss
```

### Comparing `AugmentedSocialScientist-1.1.0/LICENSE` & `AugmentedSocialScientist-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AugmentedSocialScientist-1.1.0/setup.py` & `AugmentedSocialScientist-2.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 from setuptools import setup
 
 environment = [
     'scikit-learn',
     'tqdm',
-    'pandas',
     'numpy',
     'scipy',
-    'nltk',
-    'keras',
-    'tensorflow',
     'torch',
     'transformers',
-    'sentencepiece',
+    'sentencepiece'
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(name='AugmentedSocialScientist',
       author='Rubing Shen',
       license='MIT',
       author_email='shenrubing1996@gmail.com',
       url='https://github.com/rubingshen/AugmentedSocialScientist',
-      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v1.1.0.tar.gz',
-      version='1.1.0',
-      description='A Simple Package to Train Bert-Like Model for Text Classification',
+      download_url='https://github.com/rubingshen/AugmentedSocialScientist/archive/refs/tags/v2.0.0.tar.gz',
+      version='2.0.0',
+      description='A Package to Easily Train Bert-Like Models for Text Classification',
       long_description=long_description,
       long_description_content_type="text/markdown",
       packages=['AugmentedSocialScientist'],
       zip_safe=False,
       install_requires=environment)
```

