# Comparing `tmp/spl_widgets-1.7.4.tar.gz` & `tmp/spl_widgets-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spl_widgets-1.7.4.tar", last modified: Wed Jul 26 19:18:35 2023, max compression
+gzip compressed data, was "spl_widgets-1.7.5.tar", last modified: Fri Jul 28 18:55:43 2023, max compression
```

## Comparing `spl_widgets-1.7.4.tar` & `spl_widgets-1.7.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:18:35.018310 spl_widgets-1.7.4/
--rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.4/LICENSE
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:18:35.018186 spl_widgets-1.7.4/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.4/README.md
--rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.4/pyproject.toml
--rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-26 19:18:35.018345 spl_widgets-1.7.4/setup.cfg
--rw-r--r--   0 colin      (501) staff       (20)     1240 2023-07-26 19:18:29.000000 spl_widgets-1.7.4/setup.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:18:35.009992 spl_widgets-1.7.4/src/
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:18:35.012221 spl_widgets-1.7.4/src/spl_widgets/
--rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.4/src/spl_widgets/__init__.py
--rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.4/src/spl_widgets/__main__.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:18:35.013460 spl_widgets-1.7.4/src/spl_widgets/autoscorer/
--rw-r--r--   0 colin      (501) staff       (20)    14003 2023-07-26 19:15:08.000000 spl_widgets-1.7.4/src/spl_widgets/autoscorer/autoscore.py
--rw-r--r--   0 colin      (501) staff       (20)    18685 2023-07-26 19:00:37.000000 spl_widgets-1.7.4/src/spl_widgets/autoscorer/autoscorer_gui.py
--rw-r--r--   0 colin      (501) staff       (20)     5389 2023-07-26 19:06:46.000000 spl_widgets-1.7.4/src/spl_widgets/autoscorer/tokenize_to_ipa.py
--rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.4/src/spl_widgets/batch_tune.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:18:35.017676 spl_widgets-1.7.4/src/spl_widgets/data/
--rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.4/src/spl_widgets/data/cmudict.sqlite
--rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-26 16:35:15.000000 spl_widgets-1.7.4/src/spl_widgets/data/help_text.json
--rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.4/src/spl_widgets/gorilla_clean.py
--rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.4/src/spl_widgets/jukemake.py
--rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.4/src/spl_widgets/misc_util.py
--rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.4/src/spl_widgets/stk_swx.py
--rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.4/src/spl_widgets/tune_freq.py
--rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.4/src/spl_widgets/tuner.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:18:35.018007 spl_widgets-1.7.4/src/spl_widgets/util/
--rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.4/src/spl_widgets/util/color_util.py
--rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:35:15.000000 spl_widgets-1.7.4/src/spl_widgets/util/gui_util.py
--rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.4/src/spl_widgets/util/sqlite_db.py
-drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-26 19:18:35.013054 spl_widgets-1.7.4/src/spl_widgets.egg-info/
--rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-26 19:18:35.000000 spl_widgets-1.7.4/src/spl_widgets.egg-info/PKG-INFO
--rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-26 19:18:35.000000 spl_widgets-1.7.4/src/spl_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-26 19:18:35.000000 spl_widgets-1.7.4/src/spl_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-26 19:18:35.000000 spl_widgets-1.7.4/src/spl_widgets.egg-info/entry_points.txt
--rw-r--r--   0 colin      (501) staff       (20)       43 2023-07-26 19:18:35.000000 spl_widgets-1.7.4/src/spl_widgets.egg-info/requires.txt
--rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-26 19:18:35.000000 spl_widgets-1.7.4/src/spl_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.345169 spl_widgets-1.7.5/
+-rw-r--r--   0 colin      (501) staff       (20)     1073 2021-11-03 16:44:37.000000 spl_widgets-1.7.5/LICENSE
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-28 18:55:43.345029 spl_widgets-1.7.5/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)     2101 2022-06-26 15:02:40.000000 spl_widgets-1.7.5/README.md
+-rw-r--r--   0 colin      (501) staff       (20)      103 2021-11-03 16:36:22.000000 spl_widgets-1.7.5/pyproject.toml
+-rw-r--r--   0 colin      (501) staff       (20)       38 2023-07-28 18:55:43.345208 spl_widgets-1.7.5/setup.cfg
+-rw-r--r--   0 colin      (501) staff       (20)     1240 2023-07-28 18:54:56.000000 spl_widgets-1.7.5/setup.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.330898 spl_widgets-1.7.5/src/
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.334104 spl_widgets-1.7.5/src/spl_widgets/
+-rw-r--r--   0 colin      (501) staff       (20)      279 2022-06-26 16:32:08.000000 spl_widgets-1.7.5/src/spl_widgets/__init__.py
+-rw-r--r--   0 colin      (501) staff       (20)        0 2022-06-26 14:59:05.000000 spl_widgets-1.7.5/src/spl_widgets/__main__.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.335874 spl_widgets-1.7.5/src/spl_widgets/autoscorer/
+-rw-r--r--   0 colin      (501) staff       (20)    15383 2023-07-27 21:36:42.000000 spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscore.py
+-rw-r--r--   0 colin      (501) staff       (20)    18830 2023-07-27 18:42:32.000000 spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscorer_gui.py
+-rw-r--r--   0 colin      (501) staff       (20)     5361 2023-07-28 18:55:30.000000 spl_widgets-1.7.5/src/spl_widgets/autoscorer/tokenize_to_ipa.py
+-rw-r--r--   0 colin      (501) staff       (20)     3722 2023-05-26 16:24:48.000000 spl_widgets-1.7.5/src/spl_widgets/batch_tune.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.342174 spl_widgets-1.7.5/src/spl_widgets/data/
+-rw-r--r--   0 colin      (501) staff       (20)  9670656 2023-05-26 16:25:12.000000 spl_widgets-1.7.5/src/spl_widgets/data/cmudict.sqlite
+-rw-r--r--   0 colin      (501) staff       (20)       73 2023-07-26 16:35:15.000000 spl_widgets-1.7.5/src/spl_widgets/data/help_text.json
+-rwxr-xr-x   0 colin      (501) staff       (20)     5378 2022-10-21 13:14:40.000000 spl_widgets-1.7.5/src/spl_widgets/gorilla_clean.py
+-rw-r--r--   0 colin      (501) staff       (20)     2483 2022-12-17 21:45:28.000000 spl_widgets-1.7.5/src/spl_widgets/jukemake.py
+-rw-r--r--   0 colin      (501) staff       (20)     4166 2023-05-25 22:28:36.000000 spl_widgets-1.7.5/src/spl_widgets/misc_util.py
+-rwxr-xr-x   0 colin      (501) staff       (20)     3598 2023-04-14 19:27:21.000000 spl_widgets-1.7.5/src/spl_widgets/stk_swx.py
+-rw-r--r--   0 colin      (501) staff       (20)     3614 2023-04-23 14:58:27.000000 spl_widgets-1.7.5/src/spl_widgets/tune_freq.py
+-rw-r--r--   0 colin      (501) staff       (20)    17694 2023-05-26 16:20:21.000000 spl_widgets-1.7.5/src/spl_widgets/tuner.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.344797 spl_widgets-1.7.5/src/spl_widgets/util/
+-rw-r--r--   0 colin      (501) staff       (20)     1169 2023-07-10 17:51:43.000000 spl_widgets-1.7.5/src/spl_widgets/util/color_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     5635 2023-07-26 16:35:15.000000 spl_widgets-1.7.5/src/spl_widgets/util/gui_util.py
+-rw-r--r--   0 colin      (501) staff       (20)     3642 2023-05-26 16:25:13.000000 spl_widgets-1.7.5/src/spl_widgets/util/sqlite_db.py
+drwxr-xr-x   0 colin      (501) staff       (20)        0 2023-07-28 18:55:43.335057 spl_widgets-1.7.5/src/spl_widgets.egg-info/
+-rw-r--r--   0 colin      (501) staff       (20)      411 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 colin      (501) staff       (20)      839 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 colin      (501) staff       (20)        1 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 colin      (501) staff       (20)      265 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 colin      (501) staff       (20)       43 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/requires.txt
+-rw-r--r--   0 colin      (501) staff       (20)       12 2023-07-28 18:55:43.000000 spl_widgets-1.7.5/src/spl_widgets.egg-info/top_level.txt
```

### Comparing `spl_widgets-1.7.4/LICENSE` & `spl_widgets-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/README.md` & `spl_widgets-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/setup.py` & `spl_widgets-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
     name="spl_widgets",
-    version="1.7.4",
+    version="1.7.5",
     author="Colin Simon-Fellowes",
     author_email="colin.tsf@gmail.com",
     description="Widgets for the Barnard Speech Perception Laboratory",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/clntsf/spl_widgets",
     classifiers=[
```

### Comparing `spl_widgets-1.7.4/src/spl_widgets/autoscorer/autoscore.py` & `spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscore.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
 # this is probably not incredibly elegant (the colorizing part) but it does its job, and it shouldn't ever need to
 # be changed too much functionally (except to add more features) because the data structure it gets from score() will stay the same
 def output_scoring(
     sentence_ipa: list[str],
     transcription_ipa: list[str],
     results: tuple[ int, AutoscorerTokens ]
-    ) -> tuple[int,int,str]:
+    ) -> tuple[int,int,str, list[int]]:
     """
     Takes the results of score_transcription() and outputs them as formatted strings
     containing the autoscorer's evaluation and score for the transcription
 
     Parameters
     ----------
         @param sentence_ipa ( list[str] ): the input IPA (tokenized) of the target sentence
@@ -186,14 +186,26 @@
     CLEARSTYLE = "\C"
 
     score, prev_scored = results
 
     best_poss_score = sum( map(str.isalpha, sentence_ipa) )
     transcription_chars = [*transcription_ipa]                  # split the string
 
+    # produce score by phoneme
+    score_by_phoneme = []
+    for (token, idx, is_valid) in prev_scored:
+        if is_valid is False: # extraneous
+            continue
+        if is_valid is True:  # included
+            score_by_phoneme.append(1)
+            continue
+
+        tok_len = len([*filter(str.isalpha, tokenize_ipa(token))])
+        score_by_phoneme.extend([0]*tok_len)
+
     # separate tokens into included and omitted for the two formatting passes
     included_tokens = [*filter(lambda n: n[2] is not None, prev_scored)]
     omitted_tokens = [*filter(lambda n: n[2] is None, prev_scored)]
 
     # included tokens can be edited in-place
     for (token, idx, is_valid) in included_tokens:
         token_color = (GREEN if is_valid else YELLOW)
@@ -208,15 +220,15 @@
         transcription_chars.insert(
             idx+incr,
             f"({RED}{token}{CLEARSTYLE})"
         )
         incr += 1
 
     evaluation = "".join(transcription_chars)   # combine all tokens for evaluation
-    return (score, best_poss_score, evaluation)
+    return (score, best_poss_score, evaluation, score_by_phoneme)
 
 def get_results(
     sentence_ipa: str,
     transcription: str,
     scoring_mode: ScoringMode
     ) -> tuple[ list[str], tuple[int, AutoscorerTokens] ]:
     
@@ -234,15 +246,15 @@
         return max(poss_results, key = lambda n: n[1][0])
 
 def process_inputs(
     inputs: list[tuple[str,str]],
     ws: Worksheet,
     scoring_mode: ScoringMode,
     ideal_ipa: list[str] = ...
-    ) -> None:
+    ) -> tuple[dict[str, list[int]], list[list[str]]]:
     
     # utility function to make populating rows of the output file faster
     def fill_row(row: int, values: tuple[str,...]):
         for i, col in enumerate("ABCDEF"):
             ws[f"{col}{row}"] = values[i]
 
     # write header
@@ -262,27 +274,31 @@
 
     (sentences, transcriptions) = [*zip(*inputs)]
     if ideal_ipa is ...:
         sentence_ipas = [*map(str_to_ipa, sentences)]
     else:
         sentence_ipas = [*map(tokenize_ipa, ideal_ipa)]
 
+    phoneme_scores_by_sentence = {}
+
     # iterate over the target-transcription pairs
     row=2                                               # doing it this way to use row outside of the loop's scope after
     for (sentence, sentence_ipa, transcription) in zip(sentences, sentence_ipas, transcriptions):
 
         # debug
         # print(f"TARGET: {sentence} | {sentence_ipa}", f"\nSUBJECT: {transcription} | {transcription_ipa}\n\n")
 
         transcription_ipa, results = get_results(sentence_ipa, transcription, scoring_mode)
 
-        score, best_poss_score, evaluation = output_scoring(                # format the results
+        score, best_poss_score, evaluation, score_by_phoneme = output_scoring(                # format the results
             sentence_ipa, transcription_ipa, results
         )
 
+        phoneme_scores_by_sentence[sentence] = score_by_phoneme
+
         display_sentence_ipa = "".join(sentence_ipa)
         display_transcription_ipa = "".join(transcription_ipa)
 
         total_score[0] += score
         total_score[1] += best_poss_score
 
         formatted_score = f"{score}/{best_poss_score}"
@@ -308,14 +324,16 @@
     for col in "ABCDEF":
         dim_holder[col] = dimensions.ColumnDimension(
             ws, col, width=col_width, bestFit = True
         )
 
     ws.column_dimensions = dim_holder
 
+    return phoneme_scores_by_sentence, sentence_ipas
+
 def main(
     df: pd.DataFrame = ...,
     out_dir: str = ...,
     out_fn: str = ...,
     ideal_ipa: list[str] = ...,
     scoring_mode: ScoringMode = "preferred-transcription"
     ):
@@ -340,19 +358,33 @@
         if out_fn is None:
             out_fn = fp.name[:-5] + "_autoscored"
 
         df = pd.read_excel(fp)
 
     target = df["Target"]   # get target sentences
 
+    user_sentence_phoneme_scores: dict[str, dict[str,str|list[int]]] = {}
     # iterate through subject columns
     for col in df.columns[1:]:
         ws = wb.create_sheet(col)
 
         inputs: list[tuple[str,str]] = [ *zip(target, df[col]) ]
-        process_inputs(inputs, ws, scoring_mode, ideal_ipa)
+        phoneme_scores_by_sentence, sentence_ipas = process_inputs(inputs, ws, scoring_mode, ideal_ipa)    # write to worksheet & return phoneme scores
+
+        for (sentence, score) in phoneme_scores_by_sentence.items():
+            user_sentence_phoneme_scores.setdefault(sentence, {})
+            user_sentence_phoneme_scores[sentence][col] = score
 
     outpath = Path(out_dir, f"{out_fn}.xlsx")
     wb.save(outpath)
 
+    dfs = {}
+
+    with pd.ExcelWriter(Path(out_dir, f"{out_fn}_PER_SEGMENT.xlsx"), engine="openpyxl") as writer:
+        for (i, (sentence,scores)) in enumerate(user_sentence_phoneme_scores.items()):
+            tokens = [*filter(str.isalpha, sentence_ipas[i])]
+            df = pd.DataFrame(scores, index=tokens).T
+        
+            df.to_excel(writer, sheet_name=sentence[:31])
+    
 if __name__ == "__main__":
     main()
```

### Comparing `spl_widgets-1.7.4/src/spl_widgets/autoscorer/autoscorer_gui.py` & `spl_widgets-1.7.5/src/spl_widgets/autoscorer/autoscorer_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,17 +360,20 @@
             onclick=self.focus_help_tab,
             text="Autoscored Output File(s)"
         )
         output_data_label.pack_frame(pady=(0,5))
 
         def add_output_file(listbox: MarginListBox, data: dict, filepath: Path):
             fn = filepath.name
+            fn2 = f"{filepath.stem}_PER_SEGMENT.xlsx"
 
             listbox.insert(tk.END, fn)
+            listbox.insert(tk.END, fn2)
             data[fn] = filepath
+            data[fn2] = Path(filepath.parent, fn2)
 
         self.output_data_listbox = MarginListBox(
             output_frame,
             add_output_file,
             None,
             include_minus_button=False,
             pack_args={"expand": True},
```

### Comparing `spl_widgets-1.7.4/src/spl_widgets/autoscorer/tokenize_to_ipa.py` & `spl_widgets-1.7.5/src/spl_widgets/autoscorer/tokenize_to_ipa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 from spl_widgets.util.sqlite_db import SQLiteDB
 import pkg_resources
 
 database_fp = pkg_resources.resource_filename("spl_widgets", "data/cmudict.sqlite")
 dba = SQLiteDB(database_fp, silent=True)
 
+PUNCT_RE = r"(\W*)([\w\']*)(\W*)"
+
 # https://en.wikipedia.org/wiki/ARPABET#Symbols
 phonemes = {
   "AA": "ɑ",
   "AE": "æ",
   "AH": "ʌ",
   "AO": "ɔ",
   "AW": "ɑʊ",
@@ -56,28 +58,28 @@
   "WH": "ʍ",
   "Y": "j",
   "Z": "z",
   "ZH": "ʒ"
 }
 
 def get_arpabet(word: str) -> list[list[str]]|str:
-    data = dba.execute_read_query(f"SELECT transcriptions FROM phones WHERE word = '{word}'")
+    data = dba.execute_read_query(f'SELECT transcriptions FROM phones WHERE word = "{word}"')
     
     if data == []:                          # invalid word
         # ('*'*word.isalpha()) only flags all-alpha invalid words, not just floating punctuation
         # invalid all-alpha words must be flagged so they are ignored by the scorer
         return ('*'*word.isalpha()) + word
     
     transcriptions = eval(data[0][0])
     return transcriptions
 
 def to_arpabet(sentence: str, keep_punct: bool = True) -> list[str]:
 
     arpa_words = []
-    PUNCT_RE = r"(\W*)(\w*)(\W*)"
+    
 
     for wd in sentence.split(" "):
 
         if keep_punct:
             prepunct, word, postpunct = re.match(PUNCT_RE, wd).groups(0)
         else:
             prepunct = postpunct = ""
@@ -94,15 +96,14 @@
         word_arpa = filter(None, [prepunct, *word_arpa, postpunct, " "])
         arpa_words.extend(word_arpa)
 
     return arpa_words[:-1]  # remove last added space to simplify the logic
 
 def to_arpabet_all(sentence: str, keep_punct: bool = True) -> list[list[str]]:
     arpa_sentences: list[list[str]] = []
-    PUNCT_RE = r"(\W*)(\w*)(\W*)"
 
     for wd in sentence.split(" "):
 
         if keep_punct:
             prepunct, word, postpunct = re.match(PUNCT_RE, wd).groups(0)
         else:
             prepunct = postpunct = ""
```

### Comparing `spl_widgets-1.7.4/src/spl_widgets/batch_tune.py` & `spl_widgets-1.7.5/src/spl_widgets/batch_tune.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/data/cmudict.sqlite` & `spl_widgets-1.7.5/src/spl_widgets/data/cmudict.sqlite`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/gorilla_clean.py` & `spl_widgets-1.7.5/src/spl_widgets/gorilla_clean.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/jukemake.py` & `spl_widgets-1.7.5/src/spl_widgets/jukemake.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/misc_util.py` & `spl_widgets-1.7.5/src/spl_widgets/misc_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/stk_swx.py` & `spl_widgets-1.7.5/src/spl_widgets/stk_swx.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/tune_freq.py` & `spl_widgets-1.7.5/src/spl_widgets/tune_freq.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/tuner.py` & `spl_widgets-1.7.5/src/spl_widgets/tuner.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/util/color_util.py` & `spl_widgets-1.7.5/src/spl_widgets/util/color_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/util/gui_util.py` & `spl_widgets-1.7.5/src/spl_widgets/util/gui_util.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets/util/sqlite_db.py` & `spl_widgets-1.7.5/src/spl_widgets/util/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `spl_widgets-1.7.4/src/spl_widgets.egg-info/SOURCES.txt` & `spl_widgets-1.7.5/src/spl_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

