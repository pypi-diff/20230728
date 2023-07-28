# Comparing `tmp/git_knapsack-2023.6.30.tar.gz` & `tmp/git_knapsack-2023.7.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_knapsack-2023.6.30.tar", last modified: Sat Jul  1 11:58:19 2023, max compression
+gzip compressed data, was "git_knapsack-2023.7.28.tar", last modified: Fri Jul 28 06:02:13 2023, max compression
```

## Comparing `git_knapsack-2023.6.30.tar` & `git_knapsack-2023.7.28.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-07-01 11:55:52.136941 git_knapsack-2023.6.30/LICENSE
--rw-r--r--   0        0        0      104 2023-07-01 11:55:52.136556 git_knapsack-2023.6.30/README.md
--rw-r--r--   0        0        0     1992 2023-07-01 11:55:52.136782 git_knapsack-2023.6.30/git_knapsack.py
--rw-r--r--   0        0        0      502 2023-07-01 11:58:19.266931 git_knapsack-2023.6.30/pyproject.toml
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 git_knapsack-2023.6.30/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-30 18:09:51.655569 git_knapsack-2023.7.28/LICENSE
+-rw-r--r--   0        0        0      104 2023-06-30 18:09:51.655457 git_knapsack-2023.7.28/README.md
+-rw-r--r--   0        0        0     2053 2023-07-28 05:54:10.042280 git_knapsack-2023.7.28/git_knapsack.py
+-rw-r--r--   0        0        0      523 2023-07-28 06:02:13.808774 git_knapsack-2023.7.28/pyproject.toml
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 git_knapsack-2023.7.28/PKG-INFO
```

### Comparing `git_knapsack-2023.6.30/LICENSE` & `git_knapsack-2023.7.28/LICENSE`

 * *Files identical despite different names*

### Comparing `git_knapsack-2023.6.30/git_knapsack.py` & `git_knapsack-2023.7.28/git_knapsack.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 """
 `git_knapsack.py`
 
 Knapsack untracked files in a git repository in many commits, so that each commit does not exceed 30 MB.
-Currently the knapsacking algorithm is extremely naive, and it does not expose any custom git features.
+Currently, the knapsacking algorithm is extremely naive, and it does not expose any custom git features.
 Effectively, this scripts performs git add, git commit and git push.
 
 Note that it also will commit and push any untracked file.
 If you run git status before this command and see anything you don't want committed,
 either delete it or add it to the .gitignore file.
 
 If any single file exceeds the git server's file limit or commit size limit, this script will not be able to help you.
 
 The dependencies of this script are gitpython and tqdm.
 """
 import os
 
+import appeal
 from git import Repo
 from tqdm import tqdm
 
-def main():
+
+app = appeal.Appeal()
+
+
+@app.global_command()
+def main(*, message="Knapsack into multiple commits", max_commit_size=1024 ** 2 * 30):
     repository = Repo(os.path.curdir)
     untracked_files = repository.untracked_files
 
     commit_size = 0
     untracked_file_batch = []
     for untracked_file in tqdm(untracked_files):
         current_file_size = os.stat(untracked_file).st_size
-        if commit_size + current_file_size > 1024 ** 2 * 30:  # keep commits below 30 MB
+        if commit_size + current_file_size > max_commit_size:  # keep commits below 30 MB
             repository.index.add(untracked_file_batch)
-            repository.index.commit("Knapsack into multiple commits")
+            repository.index.commit(message)
             # For many hosts, pushing after each commit is required.
             # Not only the commit and file size can be limited,
             # but often also the size of a push over HTTPS has a size limit
             origin = repository.remote('origin')
             origin.push()
             untracked_file_batch = [untracked_file]  # reset the batch
             commit_size = current_file_size  # reset the commit size
         else:
             untracked_file_batch.append(untracked_file)
             commit_size += current_file_size
 
     # Clean up any files in the queue
     repository.index.add(untracked_file_batch)
-    repository.index.commit("Knapsack into multiple commits")
+    repository.index.commit(message)
     origin = repository.remote('origin')
     origin.push()
 
 
-if __name__ == '__main__':
-    main()
+app.main()
```

