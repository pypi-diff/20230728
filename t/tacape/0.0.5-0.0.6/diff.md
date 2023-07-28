# Comparing `tmp/tacape-0.0.5-py3-none-any.whl.zip` & `tmp/tacape-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 11493 bytes, number of entries: 17
+Zip file size: 11592 bytes, number of entries: 17
 -rw-rw-r--  2.0 unx      232 b- defN 23-Apr-06 13:15 tacape/__init__.py
 -rw-rw-r--  2.0 unx      266 b- defN 23-Apr-06 13:15 tacape/logo.py
--rw-rw-r--  2.0 unx     1872 b- defN 23-Jul-21 12:20 tacape/run_classifier.py
--rw-rw-r--  2.0 unx     4736 b- defN 23-Jul-21 12:48 tacape/run_generator.py
--rw-rw-r--  2.0 unx     3810 b- defN 23-Jul-21 12:37 tacape/train_classifier.py
--rw-rw-r--  2.0 unx     3614 b- defN 23-Jul-21 12:38 tacape/train_generator.py
+-rw-rw-r--  2.0 unx     1914 b- defN 23-Jul-28 18:14 tacape/run_classifier.py
+-rw-rw-r--  2.0 unx     4841 b- defN 23-Jul-28 18:18 tacape/run_generator.py
+-rw-rw-r--  2.0 unx     3856 b- defN 23-Jul-28 17:33 tacape/train_classifier.py
+-rw-rw-r--  2.0 unx     3656 b- defN 23-Jul-28 17:33 tacape/train_generator.py
 -rw-rw-r--  2.0 unx       30 b- defN 23-Mar-30 15:33 tacape/models/__init__.py
 -rw-rw-r--  2.0 unx     1530 b- defN 23-Mar-30 15:24 tacape/models/layers.py
 -rw-rw-r--  2.0 unx     1167 b- defN 23-Apr-03 18:33 tacape/models/model.py
 -rw-rw-r--  2.0 unx       18 b- defN 23-Apr-03 17:27 tacape/utils/__init__.py
 -rw-rw-r--  2.0 unx      321 b- defN 23-Apr-03 17:27 tacape/utils/load.py
--rw-rw-r--  2.0 unx     1064 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7907 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx      215 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1339 b- defN 23-Jul-21 13:04 tacape-0.0.5.dist-info/RECORD
-17 files, 28220 bytes uncompressed, 9305 bytes compressed:  67.0%
+-rw-rw-r--  2.0 unx     1064 b- defN 23-Jul-28 18:19 tacape-0.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7907 b- defN 23-Jul-28 18:19 tacape-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-28 18:19 tacape-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      215 b- defN 23-Jul-28 18:19 tacape-0.0.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-28 18:19 tacape-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1339 b- defN 23-Jul-28 18:19 tacape-0.0.6.dist-info/RECORD
+17 files, 28455 bytes uncompressed, 9404 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: tacape/utils/__init__.py
 Comment: 
 
 Filename: tacape/utils/load.py
 Comment: 
 
-Filename: tacape-0.0.5.dist-info/LICENSE
+Filename: tacape-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: tacape-0.0.5.dist-info/METADATA
+Filename: tacape-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: tacape-0.0.5.dist-info/WHEEL
+Filename: tacape-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: tacape-0.0.5.dist-info/entry_points.txt
+Filename: tacape-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: tacape-0.0.5.dist-info/top_level.txt
+Filename: tacape-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: tacape-0.0.5.dist-info/RECORD
+Filename: tacape-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tacape/run_classifier.py

```diff
@@ -33,15 +33,15 @@
         tokenizer = pickle.loads(reader.read())
 
     with open(model_prefix + '.le', 'rb') as reader:
         le = pickle.loads(reader.read())
 
     X = keras.preprocessing.sequence.pad_sequences(tokenizer.texts_to_sequences(load_data(input, format)), maxlen = config['max_peptide_length'])
 
-    model  = build_model(output_shape=(len(le.classes_)))
+    model  = build_model(vocab_size=len(tokenizer.word_index) + 1, output_shape=(len(le.classes_)))
     model.load_weights(model_prefix + '.weights')
     y_pred = model.predict(X)[:,1]
 
     print(y_pred)
 
     df_output = pd.DataFrame()
     df_output['sequence'] = load_data(input, format)
```

## tacape/run_generator.py

```diff
@@ -36,26 +36,26 @@
 
     with open(generator_prefix + '.tokenizer', 'rb') as reader:
         generator_tokenizer = pickle.loads(reader.read())
 
     with open(generator_prefix + '.le', 'rb') as reader:
         generator_le = pickle.loads(reader.read())    
 
-    generator_model  = build_model(output_shape=(len(generator_le.classes_)))
+    generator_model  = build_model(vocab_size=len(generator_tokenizer.word_index) + 1, output_shape=(len(generator_le.classes_)))
     generator_model.load_weights(generator_prefix + '.weights').expect_partial()
 
     if classifier_prefix:
 
         with open(classifier_prefix + '.tokenizer', 'rb') as reader:
             classifier_tokenizer = pickle.loads(reader.read())
 
         with open(classifier_prefix + '.le', 'rb') as reader:
             classifier_le = pickle.loads(reader.read())
 
-        classifier_model  = build_model(output_shape=(len(classifier_le.classes_)))
+        classifier_model  = build_model(vocab_size=len(classifier_tokenizer.word_index) + 1, output_shape=(len(classifier_le.classes_)))
         classifier_model.load_weights(classifier_prefix + '.weights')
 
     number_of_generated_sequences = 0
 
     progress_bar = tqdm(total=number_of_sequences)
 
     with open(output, 'w') as writer:
```

## tacape/train_classifier.py

```diff
@@ -76,14 +76,14 @@
         patience=5,
         verbose=0,
         mode="auto",
         baseline=None,
         restore_best_weights=True,
         start_from_epoch=0,
     )]
-
-    model = build_model(output_shape=(len(le.classes_)))
+    
+    model = build_model(vocab_size=len(tokenizer.word_index) + 1, output_shape=(len(le.classes_)))
     model.fit(X_train, y_train_encode, validation_data=(X_test, y_test_encode), epochs=epochs, callbacks=callbacks)
     model.save_weights(output + '.weights')
 
 if __name__ == '__main__':
     main()
```

## tacape/train_generator.py

```diff
@@ -88,13 +88,13 @@
         verbose=0,
         mode="auto",
         baseline=None,
         restore_best_weights=True,
         start_from_epoch=0,
     )]
 
-    model = build_model(output_shape=(len(le.classes_)))
+    model = build_model(vocab_size=len(tokenizer.word_index) + 1, output_shape=(len(le.classes_)))
     model.fit(X_train_tokens, y_train_encode, validation_data=(X_test_tokens, y_test_encode), epochs=epochs, callbacks=callbacks)
     model.save_weights(output + '.weights')
 
 if __name__ == '__main__':
     main()
```

## Comparing `tacape-0.0.5.dist-info/LICENSE` & `tacape-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tacape-0.0.5.dist-info/METADATA` & `tacape-0.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tacape
-Version: 0.0.5
+Version: 0.0.6
 Summary: TACaPe: Transformed-based Anti-Cancer Peptide Classification and Generation
 Home-page: https://github.com/omixlab/anticancer-peptide
 Author: Isadora Leitzke Guidotti, Frederico Schmitt Kremer
 Author-email: fred.s.kremer@gmail.com
 License: UNKNOWN
 Keywords: bioinformatics machine-learning data science drug discovery QSAR
 Platform: UNKNOWN
```

## Comparing `tacape-0.0.5.dist-info/RECORD` & `tacape-0.0.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 tacape/__init__.py,sha256=djG1eYXbcqwm5Gr_K3wQSs9MlzmDkePC1hp4OP0HGKA,232
 tacape/logo.py,sha256=tdtlyP3-qkmrWodSjxazRQRw101ok6sRV9lMYkDTgS4,266
-tacape/run_classifier.py,sha256=Vgb0vZaD7WmpdfNBR4JmMx8gWdYOUKaTzobus7zJcbo,1872
-tacape/run_generator.py,sha256=-MiEYFb5DED3vXEpS5v6_8ZetMzw_ie0LyayoOBQ8T4,4736
-tacape/train_classifier.py,sha256=U0-nT0LYroMjj4kt2MjNOnAIweezttyqWKrxJIQhv5Y,3810
-tacape/train_generator.py,sha256=hB20eOpK0a7Pedh1vnWTJmhQotJNke2_Qwr_f5sKAso,3614
+tacape/run_classifier.py,sha256=NzP6GYW4BtnzFmjRCdOQrf1pmGKQDmP9uh1amwhxu1U,1914
+tacape/run_generator.py,sha256=Il5KvkSjDialNqN1xI7zsgfKanyWoU0esqlNDNKeOGE,4841
+tacape/train_classifier.py,sha256=oDuNzgIOnuAht1j2hUd5ePuG8ebvD9ABwuOE1mpLQEQ,3856
+tacape/train_generator.py,sha256=TSu7HwJPf-_7hO9_FlhWw0BZLSd8RlQIm3D30ddeGOY,3656
 tacape/models/__init__.py,sha256=B_zIwHcareHucr4JqgdnFAVvDfFijR__w-SsyunG2xw,30
 tacape/models/layers.py,sha256=xgp0RICRpUgrbn_18tsvaWkA_D_dZ8CLz43xRDggNCo,1530
 tacape/models/model.py,sha256=e8boh62n5oNWCIe2pawyiC5wYPqj7eWnaITujOwVZdY,1167
 tacape/utils/__init__.py,sha256=AQT2L8X2AdWB_Wk__JStBuwtUvfTGz8wTFcR94_81Zo,18
 tacape/utils/load.py,sha256=XknlskZOrjcd5Z5M9ER5yxzDLqhxiU5YAPp9s388JDg,321
-tacape-0.0.5.dist-info/LICENSE,sha256=lL6wJjUrwH3bCmb2msANo8SHV4OUCyoWfR9FeG-T4XU,1064
-tacape-0.0.5.dist-info/METADATA,sha256=leKJ0FVUhphIdRuJprBKkSTHGSZHGh7KBkhtQSl54d4,7907
-tacape-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tacape-0.0.5.dist-info/entry_points.txt,sha256=TfKUjYa52O20d8pXWYEm76xX5T7w0xm-V4d4pkUcSCc,215
-tacape-0.0.5.dist-info/top_level.txt,sha256=2LcJzKwy0vqun3FbnQSXQGlBqZdxGMypEu26pZtvWQ0,7
-tacape-0.0.5.dist-info/RECORD,,
+tacape-0.0.6.dist-info/LICENSE,sha256=lL6wJjUrwH3bCmb2msANo8SHV4OUCyoWfR9FeG-T4XU,1064
+tacape-0.0.6.dist-info/METADATA,sha256=fLrcNI8_2-ISoksMnhgR1xjqndpO0K-OTD8OeKI4aEw,7907
+tacape-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tacape-0.0.6.dist-info/entry_points.txt,sha256=TfKUjYa52O20d8pXWYEm76xX5T7w0xm-V4d4pkUcSCc,215
+tacape-0.0.6.dist-info/top_level.txt,sha256=2LcJzKwy0vqun3FbnQSXQGlBqZdxGMypEu26pZtvWQ0,7
+tacape-0.0.6.dist-info/RECORD,,
```

