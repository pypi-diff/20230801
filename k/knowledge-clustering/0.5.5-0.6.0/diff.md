# Comparing `tmp/knowledge-clustering-0.5.5.tar.gz` & `tmp/knowledge-clustering-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge-clustering-0.5.5.tar", last modified: Wed Mar  8 23:52:21 2023, max compression
+gzip compressed data, was "knowledge-clustering-0.6.0.tar", last modified: Tue Aug  1 20:02:23 2023, max compression
```

## Comparing `knowledge-clustering-0.5.5.tar` & `knowledge-clustering-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:21.665323 knowledge-clustering-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-03-08 23:52:21.665323 knowledge-clustering-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:21.661323 knowledge-clustering-0.5.5/knowledge_clustering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/add_anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/add_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/autofinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/cst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:21.665323 knowledge-clustering-0.5.5/knowledge_clustering/data/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/data/english.ini
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/data/french.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/diagnose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/file_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/knowledges.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/scope_meaning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:21.665323 knowledge-clustering-0.5.5/knowledge_clustering/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/scripts/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/knowledge_clustering/tex_document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:21.665323 knowledge-clustering-0.5.5/knowledge_clustering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-03-08 23:52:21.000000 knowledge-clustering-0.5.5/knowledge_clustering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-08 23:52:21.000000 knowledge-clustering-0.5.5/knowledge_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 23:52:21.000000 knowledge-clustering-0.5.5/knowledge_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-08 23:52:21.000000 knowledge-clustering-0.5.5/knowledge_clustering.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-08 23:52:21.000000 knowledge-clustering-0.5.5/knowledge_clustering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-08 23:52:21.000000 knowledge-clustering-0.5.5/knowledge_clustering.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-08 23:52:21.669323 knowledge-clustering-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 23:52:21.665323 knowledge-clustering-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/tests/test_addquotes.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/tests/test_anchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-03-08 23:52:12.000000 knowledge-clustering-0.5.5/tests/test_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:23.339315 knowledge-clustering-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-08-01 20:02:23.339315 knowledge-clustering-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:23.339315 knowledge-clustering-0.6.0/knowledge_clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/add_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10851 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/add_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/autofinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/cst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:23.339315 knowledge-clustering-0.6.0/knowledge_clustering/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/data/english.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/data/french.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/diagnose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/file_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/knowledges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/scope_meaning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:23.339315 knowledge-clustering-0.6.0/knowledge_clustering/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/scripts/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/knowledge_clustering/tex_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:23.339315 knowledge-clustering-0.6.0/knowledge_clustering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-08-01 20:02:23.000000 knowledge-clustering-0.6.0/knowledge_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-01 20:02:23.000000 knowledge-clustering-0.6.0/knowledge_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:02:23.000000 knowledge-clustering-0.6.0/knowledge_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 20:02:23.000000 knowledge-clustering-0.6.0/knowledge_clustering.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 20:02:23.000000 knowledge-clustering-0.6.0/knowledge_clustering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 20:02:23.000000 knowledge-clustering-0.6.0/knowledge_clustering.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-01 20:02:23.343315 knowledge-clustering-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:02:23.339315 knowledge-clustering-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/tests/test_addquotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/tests/test_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-08-01 20:02:06.000000 knowledge-clustering-0.6.0/tests/test_clustering.py
```

### Comparing `knowledge-clustering-0.5.5/LICENSE.md` & `knowledge-clustering-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/PKG-INFO` & `knowledge-clustering-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge-clustering
-Version: 0.5.5
+Version: 0.6.0
 Summary: Automated notion clustering for the knowledge LaTeX package
 Home-page: https://github.com/remimorvan/knowledge-clustering
 Author: Rémi Morvan
 Author-email: remi@morvan.xyz
 Project-URL: Bug Tracker, https://github.com/remimorvan/knowledge-clustering/issues
 Keywords: knowledge :: latex :: clustering
 Classifier: Programming Language :: Python :: 3
@@ -29,104 +29,122 @@
 the [knowledge package](https://ctan.org/pkg/knowledge).
 It has three features:
 
   - **Clustering**: provide suggestions to the user of what notions should be grouped together.
   - **Add quotes**: find where you might have missed some quotes in your document.
   - **Anchor points**: find where you might have missed anchor points in your document.
 
-The **clustering** algorithm is meant to be use while writing your document, while the last two tools
+The **clustering** algorithm is meant to be used while writing your document, while the last two tools
 should be used when your document is (nearly) ready to be published, to check if everything is right.
 
 ## Installation
 
-To install (or upgrade) `knowledge-clustering`, run
+To install (or upgrade) `knowledge-clustering`, you need to have Python 3.9 (or a more recent version), and then run
 
     pip3 install --upgrade knowledge-clustering
 
 and then
 
     knowledge init
+    
+To check if you have the latest version of `knowledge-clustering`, you can run
+
+    knowledge --version
 
 ## Clustering notions 
 
 ### Syntax
 
 ```
 Usage: knowledge cluster [OPTIONS]
 
-  Edit a NOTION file using the knowledges present in a DIAGNOSE file.
+  Defines, as a comment and in the knowledge files, all the knowledges
+  occuring in the file.
 
 Options:
   -k, --knowledge FILE      File containing the knowledges that are already
-                            defined.  [required]
+                            defined. Multiple files are allowed; new
+                            knowledges will be written in the last one.
+                            [required]
   -d, --diagnose FILE       Diagnose file produced by LaTeX.  [required]
   -l, --lang [en|fr]        Language of your TeX document.
-  -S, --scope / --no-scope  Print the scopes defined in the notion file and
+  -S, --scope / --no-scope  Print the scopes defined in the knowledge file and
                             print the possible meaning of those scope inferred
                             by knowledge-clustering.
   -c, --config-file TEXT    Specify the configuration file. By default the
                             configuration file in the folder
-                            <knowledge-clustering-installation-
-                            folder>/knowledge_clustering/data/ corresponding
+                            <knowledge-clustering-installation-folder>/data corresponding
                             to your language is used.
   --help                    Show this message and exit.
 ```
 
 ### Example
 
 Example files can be found in the `examples/` folder.
 
-While writing some document, you have defined some knowledges in a file called `ordinal-kl.tex` (distinct
+While writing some document, you have defined some knowledges in a file called `ordinal.kl` (distinct
 from your main `LaTeX`).
 You continued writing your `LaTeX` document (not provided in the `examples/` folder)
 for some time, and used some knowledges that were undefined.
 When compiling, `LaTeX` and the [`knowledge package`](https://ctan.org/pkg/knowledge) gives you a warning
 and writes in a `.diagnose` file some information explaining what went wrong. This `.diagnose` file contains
 a section called "Undefined knowledges" containing all knowledges used in your main `LaTeX` file but not
-defined in `ordinal-kl.tex`. We reproduced this section
+defined in `ordinal.kl`. We reproduced this section
 in the `ordinal.diagnose` file.
 
-![Screenshot of the `small.tex` and `small.diagnose` files before running knowledge-clustering. `small.tex` contains four knowledges, while `small.diagnose` contains five undefined knowledges.](img/small-before.png "Files `small.tex` and `small.diagnose` before running knowledge-clustering")
+![Screenshot of the `ordinal.kl` and `ordinal.diagnose` files before running knowledge-clustering. `ordinal.kl` contains four knowledges, while `ordinal.diagnose` contains five undefined knowledges.](img/small-before.png "Files `ordinal.kl` and `ordinal.diagnose` before running knowledge-clustering")
 
 Normally, you would add every undefined knowledge, one after the other, in your
-`oridnal-kl.tex`. This is quite burdensome and can
+`oridnal.kl`. This is quite burdensome and can
 largely be automated. This is precisely what `knowledge-clustering` does: after running
 
-    knowledge cluster -k small.tex -d small.diagnose
+    knowledge cluster -k ordinal.kl -d ordinal.diagnose
 
 your file `ordinal.diagnose` is left unchanged
-but `ordinal-kl.tex` is updated with comments.
+but `ordinal.kl` is updated with comments.
 
-The `cluster` command is optional: you can also write `knowledge -k ordinal-kl.tex -d ordinal.diagnose`.
+The `cluster` command is optional: you can also write `knowledge -k ordinal.kl -d ordinal.diagnose`.
 
-![After running knowledge-clustering, the five undefined knowledges are included in the `small.tex` file as comments.](img/small-after.png "Files `ordinal-kl.tex` and `ordinal.diagnose` after running knowledge-clustering`")
+![After running knowledge-clustering, the five undefined knowledges are included in the `ordinal.kl` file as comments.](img/small-after.png "Files `ordinal.kl` and `ordinal.diagnose` after running knowledge-clustering`")
 
-Now you simply have to check that the recommandations of `knowledge-clustering` are
+Now you simply have to check that the recommendations of `knowledge-clustering` are
 correct, and uncomment those lines.
 
+### Multiple knowledge files
+
+If you have **multiple knowledge files**, you can use the `-k` option multiple times.
+For instance, you could write:
+
+	knowledge cluster -k 1.kl -k 2.kl -d ordinal.diagnose
+
+Synonyms of knowledges defined in `1.kl` (resp. `2.kl`) will be defined, as comments,
+in `1.kl` (resp. `2.kl`). New knowledges will always be added, as comments, to the last
+file, which is `2.kl` in the example.
+
 ## Adding quotes
 
 ```
 Usage: knowledge addquotes [OPTIONS]
 
-  Finds knowledges defined in KNOWLEDGE that appear in TEX without quote
-  symbols. Proposes to add quotes around them.
+  Finds knowledges defined in the knowledge files that appear in tex file
+  without quote symbols. Proposes to add quotes around them.
 
 Options:
   -t, --tex FILE        Your TeX file.  [required]
   -k, --knowledge FILE  File containing the knowledges that are already
-                        defined.  [required]
+                        defined. Multiple files are allowed; new knowledges
+                        will be written in the last one.  [required]
   -p, --print INTEGER   When finding a match, number of lines (preceding the
                         match) that are printed in the prompt to the user.
   --help                Show this message and exit.
 ```
 
 After running 
 
-    knowledge addquotes -t mydocument.tex -k knowledges.tex
+    knowledge addquotes -t mydocument.tex -k knowledges1.kl -k knowledges2.kl
 
 your prompt will propose to add quotes around defined knowledges,
 and to define synonyms of knowledges that occur in your TeX file. For instance, if
 "algorithm" is a defined knowledge and "algorithms" occurs in your TeX file, then
 it will propose to you to define "algorithms" as a synonym of the knowledge "algorithm",
 and to add a pair of quotes around the string "algorithms" that occurs in your TeX file.
 
@@ -182,14 +200,18 @@
 python3 -m venv kl.venv
 source ./kl.venv/bin/activate.fish
 pip3 install --editable .
 ```
 
 ## FAQ
 
+- `knowledge: command not found` after installing `knowledge-clustering`
+
+  **Solution**: make sure you have Python>=3.9.
+  
 - When running `knowledge`, I obtain a long message error indicating "Resource punkt not found."
 
   **Solution**: run `knowledge init`.
 
 - My shell doesn't autocomplete the command `knowledge`.
 
   **Solution**: depending on whether you use `zsh` or `bash` write
@@ -197,15 +219,15 @@
        eval "`pip completion --<shellname>`"
 
   (where `<shellname>` is either `zsh` or `bash`)
   in your `.zshrc` (or `.bashrc`) file and then,
   either launch a new terminal or run `source ~/.zshrc`
   (or `source ~/.bashrc`).
 
-- I've updated `knowledge-clustering` but I still don't have the last version:
+- I've updated `knowledge-clustering` but I still don't have the last version (which can be checked using `knowledge --version`):
 
   This can happen if you have multiple versions of `python` (and multiple versions
   of `knowledge-clustering`).
   **Solution**: Type `where python3`, and uninstall `knowledge-clustering`
   from everywhere (using `<path>/python3 -m pip uninstall knowledge-clustering`)
   except your main version of python. Try to then upgrade `knowledge-clustering`
   by running `pip3 install --upgrade knowledge-clustering`.
```

### Comparing `knowledge-clustering-0.5.5/README.md` & `knowledge-clustering-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,104 +12,122 @@
 the [knowledge package](https://ctan.org/pkg/knowledge).
 It has three features:
 
   - **Clustering**: provide suggestions to the user of what notions should be grouped together.
   - **Add quotes**: find where you might have missed some quotes in your document.
   - **Anchor points**: find where you might have missed anchor points in your document.
 
-The **clustering** algorithm is meant to be use while writing your document, while the last two tools
+The **clustering** algorithm is meant to be used while writing your document, while the last two tools
 should be used when your document is (nearly) ready to be published, to check if everything is right.
 
 ## Installation
 
-To install (or upgrade) `knowledge-clustering`, run
+To install (or upgrade) `knowledge-clustering`, you need to have Python 3.9 (or a more recent version), and then run
 
     pip3 install --upgrade knowledge-clustering
 
 and then
 
     knowledge init
+    
+To check if you have the latest version of `knowledge-clustering`, you can run
+
+    knowledge --version
 
 ## Clustering notions 
 
 ### Syntax
 
 ```
 Usage: knowledge cluster [OPTIONS]
 
-  Edit a NOTION file using the knowledges present in a DIAGNOSE file.
+  Defines, as a comment and in the knowledge files, all the knowledges
+  occuring in the file.
 
 Options:
   -k, --knowledge FILE      File containing the knowledges that are already
-                            defined.  [required]
+                            defined. Multiple files are allowed; new
+                            knowledges will be written in the last one.
+                            [required]
   -d, --diagnose FILE       Diagnose file produced by LaTeX.  [required]
   -l, --lang [en|fr]        Language of your TeX document.
-  -S, --scope / --no-scope  Print the scopes defined in the notion file and
+  -S, --scope / --no-scope  Print the scopes defined in the knowledge file and
                             print the possible meaning of those scope inferred
                             by knowledge-clustering.
   -c, --config-file TEXT    Specify the configuration file. By default the
                             configuration file in the folder
-                            <knowledge-clustering-installation-
-                            folder>/knowledge_clustering/data/ corresponding
+                            <knowledge-clustering-installation-folder>/data corresponding
                             to your language is used.
   --help                    Show this message and exit.
 ```
 
 ### Example
 
 Example files can be found in the `examples/` folder.
 
-While writing some document, you have defined some knowledges in a file called `ordinal-kl.tex` (distinct
+While writing some document, you have defined some knowledges in a file called `ordinal.kl` (distinct
 from your main `LaTeX`).
 You continued writing your `LaTeX` document (not provided in the `examples/` folder)
 for some time, and used some knowledges that were undefined.
 When compiling, `LaTeX` and the [`knowledge package`](https://ctan.org/pkg/knowledge) gives you a warning
 and writes in a `.diagnose` file some information explaining what went wrong. This `.diagnose` file contains
 a section called "Undefined knowledges" containing all knowledges used in your main `LaTeX` file but not
-defined in `ordinal-kl.tex`. We reproduced this section
+defined in `ordinal.kl`. We reproduced this section
 in the `ordinal.diagnose` file.
 
-![Screenshot of the `small.tex` and `small.diagnose` files before running knowledge-clustering. `small.tex` contains four knowledges, while `small.diagnose` contains five undefined knowledges.](img/small-before.png "Files `small.tex` and `small.diagnose` before running knowledge-clustering")
+![Screenshot of the `ordinal.kl` and `ordinal.diagnose` files before running knowledge-clustering. `ordinal.kl` contains four knowledges, while `ordinal.diagnose` contains five undefined knowledges.](img/small-before.png "Files `ordinal.kl` and `ordinal.diagnose` before running knowledge-clustering")
 
 Normally, you would add every undefined knowledge, one after the other, in your
-`oridnal-kl.tex`. This is quite burdensome and can
+`oridnal.kl`. This is quite burdensome and can
 largely be automated. This is precisely what `knowledge-clustering` does: after running
 
-    knowledge cluster -k small.tex -d small.diagnose
+    knowledge cluster -k ordinal.kl -d ordinal.diagnose
 
 your file `ordinal.diagnose` is left unchanged
-but `ordinal-kl.tex` is updated with comments.
+but `ordinal.kl` is updated with comments.
 
-The `cluster` command is optional: you can also write `knowledge -k ordinal-kl.tex -d ordinal.diagnose`.
+The `cluster` command is optional: you can also write `knowledge -k ordinal.kl -d ordinal.diagnose`.
 
-![After running knowledge-clustering, the five undefined knowledges are included in the `small.tex` file as comments.](img/small-after.png "Files `ordinal-kl.tex` and `ordinal.diagnose` after running knowledge-clustering`")
+![After running knowledge-clustering, the five undefined knowledges are included in the `ordinal.kl` file as comments.](img/small-after.png "Files `ordinal.kl` and `ordinal.diagnose` after running knowledge-clustering`")
 
-Now you simply have to check that the recommandations of `knowledge-clustering` are
+Now you simply have to check that the recommendations of `knowledge-clustering` are
 correct, and uncomment those lines.
 
+### Multiple knowledge files
+
+If you have **multiple knowledge files**, you can use the `-k` option multiple times.
+For instance, you could write:
+
+	knowledge cluster -k 1.kl -k 2.kl -d ordinal.diagnose
+
+Synonyms of knowledges defined in `1.kl` (resp. `2.kl`) will be defined, as comments,
+in `1.kl` (resp. `2.kl`). New knowledges will always be added, as comments, to the last
+file, which is `2.kl` in the example.
+
 ## Adding quotes
 
 ```
 Usage: knowledge addquotes [OPTIONS]
 
-  Finds knowledges defined in KNOWLEDGE that appear in TEX without quote
-  symbols. Proposes to add quotes around them.
+  Finds knowledges defined in the knowledge files that appear in tex file
+  without quote symbols. Proposes to add quotes around them.
 
 Options:
   -t, --tex FILE        Your TeX file.  [required]
   -k, --knowledge FILE  File containing the knowledges that are already
-                        defined.  [required]
+                        defined. Multiple files are allowed; new knowledges
+                        will be written in the last one.  [required]
   -p, --print INTEGER   When finding a match, number of lines (preceding the
                         match) that are printed in the prompt to the user.
   --help                Show this message and exit.
 ```
 
 After running 
 
-    knowledge addquotes -t mydocument.tex -k knowledges.tex
+    knowledge addquotes -t mydocument.tex -k knowledges1.kl -k knowledges2.kl
 
 your prompt will propose to add quotes around defined knowledges,
 and to define synonyms of knowledges that occur in your TeX file. For instance, if
 "algorithm" is a defined knowledge and "algorithms" occurs in your TeX file, then
 it will propose to you to define "algorithms" as a synonym of the knowledge "algorithm",
 and to add a pair of quotes around the string "algorithms" that occurs in your TeX file.
 
@@ -165,14 +183,18 @@
 python3 -m venv kl.venv
 source ./kl.venv/bin/activate.fish
 pip3 install --editable .
 ```
 
 ## FAQ
 
+- `knowledge: command not found` after installing `knowledge-clustering`
+
+  **Solution**: make sure you have Python>=3.9.
+  
 - When running `knowledge`, I obtain a long message error indicating "Resource punkt not found."
 
   **Solution**: run `knowledge init`.
 
 - My shell doesn't autocomplete the command `knowledge`.
 
   **Solution**: depending on whether you use `zsh` or `bash` write
@@ -180,15 +202,15 @@
        eval "`pip completion --<shellname>`"
 
   (where `<shellname>` is either `zsh` or `bash`)
   in your `.zshrc` (or `.bashrc`) file and then,
   either launch a new terminal or run `source ~/.zshrc`
   (or `source ~/.bashrc`).
 
-- I've updated `knowledge-clustering` but I still don't have the last version:
+- I've updated `knowledge-clustering` but I still don't have the last version (which can be checked using `knowledge --version`):
 
   This can happen if you have multiple versions of `python` (and multiple versions
   of `knowledge-clustering`).
   **Solution**: Type `where python3`, and uninstall `knowledge-clustering`
   from everywhere (using `<path>/python3 -m pip uninstall knowledge-clustering`)
   except your main version of python. Try to then upgrade `knowledge-clustering`
   by running `pip3 install --upgrade knowledge-clustering`.
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/add_anchor.py` & `knowledge-clustering-0.6.0/knowledge_clustering/add_anchor.py`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/add_quotes.py` & `knowledge-clustering-0.6.0/knowledge_clustering/add_quotes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from __future__ import annotations  # Support of `|` for type union in Python 3.9
 
 import re  # Regular expressions
 from typing import NamedTuple, TextIO
 import sys
 
-from knowledge_clustering.knowledges import Knowledges
+from knowledge_clustering.knowledges import KnowledgesList
 from knowledge_clustering.tex_document import TexDocument
 from knowledge_clustering import file_updater, misc, cst
 
 
 class NewKL(NamedTuple):
     """
     Object storing a new knowledge, together with its starting and ending point in some TeX
@@ -46,43 +46,43 @@
     print(message, file=out)
     ans = inp.readline().rstrip("\n")
     return ans.lower() in ["y", "yes"]
 
 
 def app(
     tex_filename: str,
-    kl_filename: str,
+    kl_filenames: list[str],
     print_line: int,
     inp: TextIO = sys.stdin,
     out: TextIO = sys.stdout,
 ):
     """
     Finds knowledges defined in the knowledge file that appear in tex file without quote
     symbols. Proposes to add quotes around them.
     Args:
         tex_filename: the name of the tex file.
-        kl_filename: the name of the knowledge file.
+        kl_filenames: the names of the knowledge files.
         print_line: an integer specifying how many lines of the tex file should be printed.
         inp: input stream.
         out: output stream.
     """
     tex_hash = file_updater.hash_file(tex_filename)
     with open(tex_filename, "r", encoding="utf-8") as f:
         tex_doc = TexDocument(f.read())
     f.close()
-    kl = Knowledges(kl_filename)
+    kls = KnowledgesList(kl_filenames)
     tex_document_new, new_knowledges = quote_maximal_substrings(
-        tex_doc, kl, print_line, inp, out
+        tex_doc, kls, print_line, inp, out
     )
     with file_updater.AtomicUpdate(tex_filename, original_hash=tex_hash) as f:
         f.write(tex_document_new)
     f.close()
     for known_kl, new_kl in new_knowledges:
-        kl.define_synonym_of(new_kl, known_kl)
-    kl.write_knowledges_in_file(nocomment=True)
+        kls.define_synonym_of(new_kl, known_kl)
+    kls.write_knowledges_in_file(nocomment=True)
 
 
 def add_quote(
     tex_doc: TexDocument,
     operations: list[NewKL | AddQuote],
     print_line: int,
     inp: TextIO,
@@ -183,51 +183,51 @@
         file=out,
     )
     return result, new_knowledges
 
 
 def quote_maximal_substrings(
     tex_doc: TexDocument,
-    kl: Knowledges,
+    kls: KnowledgesList,
     print_line: int,
     inp: TextIO,
     out: TextIO,
 ) -> tuple[str, list[tuple[str, str]]]:
     """
     Finds knowledges defined in the knowledge file that appear in tex file without quote
     symbols. Proposes to add quotes around them.
 
     Args:
         tex_doc: a TeX document.
-        kl: knowledges.
+        kls: list of knowledges.
         print_line: an integer specifying how many lines of the tex file should be printed.
         inp: input stream.
         out: output stream.
     """
 
     def stop_expanding(char):
         return not char.isalpha()
 
     ignore_position = [False] * tex_doc.length
     add_quote_location: list[NewKL | AddQuote] = []
     for ignore_case in [False, True]:
         # Start the algo by being case sensitive, then run it while being insensitive.
-        for s1 in kl.all_knowledges_sorted:
+        for s1 in kls.get_sorted_knowledges():
             match_list = (
                 re.finditer(re.escape(s1), tex_doc.tex_cleaned, re.IGNORECASE)
                 if ignore_case
                 else re.finditer(re.escape(s1), tex_doc.tex_cleaned)
             )
             for match in match_list:
                 start, end = match.start(), match.end() - 1
                 if not ignore_position[start]:
                     # Ignore every infix of s1 that is also a substring of the list
                     for i in range(start, end + 1):
                         ignore_position[i] = True
-                    for s2 in kl.dependency[s1]:
+                    for s2 in kls.dependency[s1]:
                         for submatch in re.finditer(
                             re.escape(s2), tex_doc.tex_cleaned[start : end + 1]
                         ):
                             ignore_position[start + submatch.start()] = True
                     # Check if s1 is precedeed by quotes, if not, either check
                     # if we can define a new knowledge, or add the match to the
                     # list of quotes to add.
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/autofinder.py` & `knowledge-clustering-0.6.0/knowledge_clustering/autofinder.py`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/clustering.py` & `knowledge-clustering-0.6.0/knowledge_clustering/clustering.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 """Clustering algorithm."""
 
 from __future__ import annotations  # Support of `|` for type union in Python 3.9
 
 import copy
 
 from knowledge_clustering import distance, config, scope_meaning, diagnose, cst
-from knowledge_clustering.knowledges import Knowledges
+from knowledge_clustering.knowledges import KnowledgesList
 
 
 def app(
-    kl_filename: str,
+    kl_filename: list[str],
     dg_filename: str,
     scope: bool,
     lang: str,
     config_filename: None | str,
 ):
     """
     Defines, as a comment and in the knowledge file, all the knowledges occuring in the diagnose file.
     Args:
         kl_filename: the name of the knowledge file.
         dg_filename: the name of the diagnose file.
         scope: a boolean specifying whether the scopes meaning should be printed.
         lang: the langage of the document.
         config_filename: a configuration file, specifying prefixes to ignore.
     """
-    kl = Knowledges(kl_filename)
+    kls = KnowledgesList(kl_filename)
 
     if config_filename is None:
         config_filename = cst.CONFIG_FILE[lang]
 
     list_prefixes = config.parse(config_filename)
 
     scopes_meaning = scope_meaning.infer_all_scopes(
-        kl.get_all_bags(), cst.NLTK_LANG[lang]
+        kls.get_all_bags(), cst.NLTK_LANG[lang]
     )
     if scope:
         scope_meaning.print_scopes(scopes_meaning, print_meaning=True)
-
     unknown_knowledges = diagnose.parse(dg_filename)
 
     if len(unknown_knowledges) == 0:
         return
 
     # update `kl` using the clustering algorithm
     clustering(
-        kl,
+        kls,
         unknown_knowledges,
         cst.ALPHA,
         list_prefixes,
         scopes_meaning,
         cst.NLTK_LANG[lang],
     )
     print(
-        f"Found a solution by adding {len(kl.get_new_bags())} new bag"
-        + ("s" if len(kl.get_new_bags()) >= 2 else "")
+        f"Found a solution by adding {len(kls.get_new_bags())} new bag"
+        + ("s" if len(kls.get_new_bags()) >= 2 else "")
         + "."
     )
-    kl.write_knowledges_in_file()
+    kls.write_knowledges_in_file()
 
 
 def clustering(
-    kls: Knowledges,
+    kls: KnowledgesList,
     unknown_kl: list[str],
     alpha: float,
     list_prefixes: list[str],
     scopes_meaning: dict[str, list[list[str]]],
     lang: str,
 ):
     """
@@ -73,15 +72,15 @@
     The invariant satisfied by the algorithm is the following:
         any two notions in the same bag are near, where near either means:
             - both in the same bag of knowledges at the beggining of the algorithm ;
             - at distance (from module "dist") at most alpha if at least one of
                 the two notions initially belongs to unknown_kls.
 
     Args:
-        kl: known knowledges.
+        kls: known knowledges.
         unknown_kl: a list of unknown knowledges.
         alpha: a threshold indicating the maximal distance allowed for clustering
             two knowkledges together.
         list_prefixes: a list of prefixes that are ignored when computing the
             distance between two knowledges.
         scope_meaning: a dictionnary, assigning to every scope a list of
             its possible meanings, each possible meaning being a list of words;
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/config.py` & `knowledge-clustering-0.6.0/knowledge_clustering/config.py`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/cst.py` & `knowledge-clustering-0.6.0/knowledge_clustering/cst.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     "\\^",
     '\\"',
     "\\~",
     "\\=",
     "\\.",
 ]  # LaTeX accents defined using non-alphanumerical commands
 IGNORE_CHAR = ["\\-", "{", "}"]
+SPACE_CHAR = ["~"]
 
 DISCARD_LINE = "%%%%% NEW KNOWLEDGES "
 
 BEGIN_EMPH: str = "\033[1m\033[95m"
 BEGIN_EMPH_ALT: str = "\033[1m\033[92m"
 BEGIN_EMPH_BOLD: str = "\033[1m"
 END_EMPH: str = "\033[0m"
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/diagnose.py` & `knowledge-clustering-0.6.0/knowledge_clustering/diagnose.py`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/distance.py` & `knowledge-clustering-0.6.0/knowledge_clustering/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,18 @@
     """
     if "@" in notion:
         s = notion.split("@", 1)
         return s[0], s[1]
     return notion, ""
 
 
-def normalise_notion(notion):
+def normalise_notion(notion: str) -> str:
     """
-    Returns the substring of a notion obtained by removing math and commands.
+    Returns the substring of a notion obtained by removing math, commands, accents
+    and non-brekable spaces.
     """
     notion_norm = notion
     while "$" in notion_norm:
         sp = notion_norm.split("$", 2)
         if len(sp) <= 1:
             break
         notion_norm = sp[0] + sp[2]
@@ -95,14 +96,19 @@
             i += 1
         notion_norm = pref + suff[i:]
     for remove_char in cst.IGNORE_CHAR:
         while remove_char in notion_norm:
             # If the notion contains remove_char, remove it.
             sp = notion_norm.split(remove_char, 1)
             notion_norm = sp[0] + sp[1]
+    for space_char in cst.SPACE_CHAR:
+        while space_char in notion_norm:
+            # If the notion contains remove_char, replace it with a space.
+            sp = notion_norm.split(space_char, 1)
+            notion_norm = sp[0] + " " + sp[1]
     return unidecode(notion_norm)  # Ascii-fy (in particular, remove accents) the result
 
 
 def breakup_notion(notion, lang):
     """
     Takes a notion, and a language, and returns
     a set of words contained in the notion.
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/file_updater.py` & `knowledge-clustering-0.6.0/knowledge_clustering/file_updater.py`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/knowledges.py` & `knowledge-clustering-0.6.0/knowledge_clustering/knowledges.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,36 +27,36 @@
     """Flattens a list of list into a single list."""
     return [x for y in list_of_list for x in y]
 
 
 class Knowledges:
     def __init__(self, filename):
         """
-        Reads a tex file from a file descriptor f.
+        Reads a knowledge file from a file descriptor f.
 
         Args:
             filename: the name of a file containing knowledges.
 
         Computes:
             self.original_hash: the hash of the document ;
             self.document: a list of records, either of the form:
-                {
-                    "type"="tex",
-                    "lines"= list of strings (the lines)
-                }
-                or {
-                    "type"="knowledge",
-                    "lines"= list of strings (the lines)
-                    "command" = string representing the line introducing the knowledge,
-                    "number" = the number of the knowledge
-                }
+                    {
+                            "type"="tex",
+                            "lines"= list of strings (the lines)
+                    }
+                    or {
+                            "type"="knowledge",
+                            "lines"= list of strings (the lines)
+                            "command" = string representing the line introducing the knowledge,
+                            "number" = the number of the knowledge
+                    }
             self.known_knowledges: a list of list of strings.
-                Each list of strings contains strings corresponding to the same knowledge.
-                The position in the string corresponds to the "number" field in the above
-                document description.
+                    Each list of strings contains strings corresponding to the same knowledge.
+                    The position in the string corresponds to the "number" field in the above
+                    document description.
         """
         self.bags: list[list[str]] = []  # Lists of lists, containing knowledges.
         self.filename: str = filename
         self.original_hash = fu.hash_file(filename)
         with open(filename, encoding="utf-8") as file:
             lines: list[str] = file.readlines()
 
@@ -141,19 +141,17 @@
                 elif reading_mode == "tex":
                     current_block.append(line)
             push_block()
             self.document = document
             self.bags = knowledges
             self.nb_known_bags: int = len(self.bags)
             self.length_known_bags: list[int] = [len(bag) for bag in self.bags]
-            self.compute_dependency_graph()
 
     def get_all_bags(self) -> list[list[str]]:
-        """Returns all bags that were not added since the last checkpoint,
-        as a list of lists of strings."""
+        """Returns all bags as a list of lists of strings."""
         return self.bags
 
     def get_new_bags(self) -> list[list[str]]:
         """Returns all bags that were not added since the last checkpoint,
         as a list of lists of strings."""
         return self.bags[self.nb_known_bags :]
 
@@ -186,34 +184,14 @@
         """
         for b_id, bag in enumerate(self.bags):
             if kl2 in bag:
                 self.bags[b_id].append(kl1)
                 return
         print(f"Error: {kl2} is not a knowledge.")
 
-    def compute_dependency_graph(self) -> None:
-        """
-        Computes the dependency graph of all knowledges, for the substring relation.
-        Then, sort all knowledges using topological sorting.
-        Result are stored in self.dependency and self.all_knowledges_sorted.
-        """
-        dependency: dict[str, set[str]] = {}
-        dependency_reversed: dict[str, set[str]] = {}
-        for s1 in self.get_all_knowledges():
-            dependency[s1] = {
-                s2 for s2 in self.get_all_knowledges() if s2 in s1 and s1 != s2
-            }
-            dependency_reversed[s1] = {
-                s2 for s2 in self.get_all_knowledges() if s1 in s2 and s1 != s2
-            }
-        self.dependency: dict[str, set[str]] = dependency
-        self.all_knowledges_sorted: list[str] = list(
-            toposort.toposort_flatten(dependency_reversed)
-        )
-
     def write_knowledges_in_file(self, nocomment: bool = False) -> None:
         """
         Writes the new synonyms and new knowledges in the file containing the knowledges.
         """
         with fu.AtomicUpdate(self.filename, original_hash=self.original_hash) as file:
             for b in self.document:
                 if isinstance(b, DocInfoTex):
@@ -229,7 +207,86 @@
                 file.write(cst.DISCARD_LINE + "\n")
                 for bag in self.get_new_bags():
                     if len(bag) > 0:
                         file.write("%\n")
                         file.write("%\\knowledge{notion}\n")
                         for kl in bag:
                             file.write((f" | {kl}\n" if nocomment else f"%  | {kl}\n"))
+
+
+class KnowledgesList:
+    def __init__(self, kls_list: list[str]):
+        """
+        Reads a list of knowledge files.
+
+        Args:
+            kls_list: the list of filenames containing knowledges.
+        """
+        self.nb_file: int = len(kls_list)
+        self.kls_list: list[Knowledges] = [
+            Knowledges(filename) for filename in kls_list
+        ]
+        self.compute_dependency_graph()
+
+    def default_kls(self) -> Knowledges:
+        """Returns the default kls."""
+        return self.kls_list[self.nb_file - 1]
+
+    def get_all_bags(self) -> list[list[str]]:
+        """Returns all bags as a list of lists of strings."""
+        return flat([kls.get_all_bags() for kls in self.kls_list])
+
+    def get_all_knowledges(self) -> list[str]:
+        """Returns all knowledges, as a list of strings."""
+        return flat([kls.get_all_knowledges() for kls in self.kls_list])
+
+    def get_sorted_knowledges(self) -> list[str]:
+        """Returns all knowledges, sorted by topological sort."""
+        return self.all_knowledges_sorted
+
+    def add_new_bag(self, kl: str) -> None:
+        """Adds a new bag that contains only the string `kl`."""
+        self.default_kls().add_new_bag(kl)
+
+    def define_synonym_of(self, kl1: str, kl2: str) -> None:
+        """
+        Defines a new knowledge (string) `kl1` as a new synonym of the already
+        existing knowledge (string) `kl2`.
+        """
+        for kls in self.kls_list:
+            for b_id, bag in enumerate(kls.bags):
+                if kl2 in bag:
+                    kls.bags[b_id].append(kl1)
+                    return
+        print(f"Error: {kl2} is not a knowledge.")
+
+    def write_knowledges_in_file(self, nocomment: bool = False) -> None:
+        """
+        Writes the new synonyms and new knowledges in the file containing the knowledges.
+        """
+        for kls in self.kls_list:
+            kls.write_knowledges_in_file(nocomment)
+
+    def get_new_bags(self) -> list[list[str]]:
+        """Returns all bags that were not added since the last checkpoint,
+        as a list of lists of strings."""
+        return self.default_kls().get_new_bags()
+
+    def compute_dependency_graph(self) -> None:
+        """
+        Computes the dependency graph of all knowledges, for the substring relation.
+        Then, sort all knowledges using topological sorting.
+        Result are stored in self.dependency and self.all_knowledges_sorted.
+        """
+        dependency: dict[str, set[str]] = {}
+        dependency_reversed: dict[str, set[str]] = {}
+        for s1 in self.get_all_knowledges():
+            dependency[s1] = {
+                s2 for s2 in self.get_all_knowledges() if s2 in s1 and s1 != s2
+            }
+            dependency_reversed[s1] = {
+                s2 for s2 in self.get_all_knowledges() if s1 in s2 and s1 != s2
+            }
+        self.dependency: dict[str, set[str]] = dependency
+        self.all_knowledges_sorted: list[str] = list(
+            toposort.toposort_flatten(dependency_reversed)
+        )
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/scope_meaning.py` & `knowledge-clustering-0.6.0/knowledge_clustering/scope_meaning.py`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/scripts/app.py` & `knowledge-clustering-0.6.0/knowledge_clustering/scripts/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 
 
 @cli.command()
 @click.option(
     "--knowledge",
     "-k",
     "kl_filename",
+    multiple=True,
     type=click.Path(
         exists=True, file_okay=True, dir_okay=False, writable=True, readable=True
     ),
-    help="File containing the knowledges that are already defined.",
+    help="File containing the knowledges that are already defined. Multiple files are allowed; new knowledges will be written in the last one.",
     required=True,
 )
 @click.option(
     "--diagnose",
     "-d",
     "dg_filename",
     type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
@@ -65,24 +66,24 @@
     "-c",
     "config_filename",
     default=None,
     help=f"Specify the configuration file. By default the configuration file in the folder {cst.CONFIG_DIR} \
 corresponding to your language is used.",
 )
 def cluster(
-    kl_filename: str,
+    kl_filename: tuple[str],
     dg_filename: str,
     scope: bool,
     lang: str,
     config_filename: None | str,
 ):
     """
-    Defines, as a comment and in the knowledge file, all the knowledges occuring in the diagnose file.
+    Defines, as a comment and in the knowledge files, all the knowledges occuring in the file.
     """
-    clustering.app(kl_filename, dg_filename, scope, lang, config_filename)
+    clustering.app(list(kl_filename), dg_filename, scope, lang, config_filename)
 
 
 @cli.command()
 @click.option(
     "--tex",
     "-t",
     "tex_filename",
@@ -92,34 +93,35 @@
     help="Your TeX file.",
     required=True,
 )
 @click.option(
     "--knowledge",
     "-k",
     "kl_filename",
+    multiple=True,
     type=click.Path(
         exists=True, file_okay=True, dir_okay=False, writable=True, readable=True
     ),
-    help="File containing the knowledges that are already defined.",
+    help="File containing the knowledges that are already defined. Multiple files are allowed; new knowledges will be written in the last one.",
     required=True,
 )
 @click.option(
     "--print",
     "-p",
     "print_line",
     type=int,
     default=1,
     help="When finding a match, number of lines (preceding the match) that are printed in the prompt to the user.",
 )
 def addquotes(tex_filename: str, kl_filename: str, print_line: int):
     """
-    Finds knowledges defined in the knowledge file that appear in tex file without quote
+    Finds knowledges defined in the knowledge files that appear in tex file without quote
     symbols. Proposes to add quotes around them.
     """
-    return add_quotes.app(tex_filename, kl_filename, print_line)
+    return add_quotes.app(tex_filename, list(kl_filename), print_line)
 
 
 @cli.command()
 @click.option(
     "--tex",
     "-t",
     "tex_filename",
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering/tex_document.py` & `knowledge-clustering-0.6.0/knowledge_clustering/tex_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 
 from knowledge_clustering import misc
 
 
 class TexDocument:
     """Class for handling a tex document."""
 
-    def __init__(self, tex_code: str, size_tab: int = 4) -> None:
+    def __init__(self, tex_code: str) -> None:
         self.tex_code: str = tex_code
         self.lines: list[str] = self.tex_code.split("\n")
-        self.size_tab: int = size_tab
         self.__update_col_line()
         self.__clean()
         self.length: int = len(self.tex_cleaned)
 
     def __update_col_line(self) -> None:
         """
         Compute two arrays, saying for each index i of self.text, at what column and
@@ -27,17 +26,15 @@
         line: int = 1
         col: int = 1
         for (position, letter) in enumerate(self.tex_code):
             self.find_line[position] = line
             self.find_col[position] = col
             if letter == "\n":
                 line += 1
-                col = 0
-            if letter == "\t":
-                col += self.size_tab
+                col = 1
             else:
                 col += 1
 
     def __clean(self):
         """
         Reads self.tex_code (the original tex file), given as a single string.
         Converts spaces, tabulations and new lines into a single space, except
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering.egg-info/PKG-INFO` & `knowledge-clustering-0.6.0/knowledge_clustering.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge-clustering
-Version: 0.5.5
+Version: 0.6.0
 Summary: Automated notion clustering for the knowledge LaTeX package
 Home-page: https://github.com/remimorvan/knowledge-clustering
 Author: Rémi Morvan
 Author-email: remi@morvan.xyz
 Project-URL: Bug Tracker, https://github.com/remimorvan/knowledge-clustering/issues
 Keywords: knowledge :: latex :: clustering
 Classifier: Programming Language :: Python :: 3
@@ -29,104 +29,122 @@
 the [knowledge package](https://ctan.org/pkg/knowledge).
 It has three features:
 
   - **Clustering**: provide suggestions to the user of what notions should be grouped together.
   - **Add quotes**: find where you might have missed some quotes in your document.
   - **Anchor points**: find where you might have missed anchor points in your document.
 
-The **clustering** algorithm is meant to be use while writing your document, while the last two tools
+The **clustering** algorithm is meant to be used while writing your document, while the last two tools
 should be used when your document is (nearly) ready to be published, to check if everything is right.
 
 ## Installation
 
-To install (or upgrade) `knowledge-clustering`, run
+To install (or upgrade) `knowledge-clustering`, you need to have Python 3.9 (or a more recent version), and then run
 
     pip3 install --upgrade knowledge-clustering
 
 and then
 
     knowledge init
+    
+To check if you have the latest version of `knowledge-clustering`, you can run
+
+    knowledge --version
 
 ## Clustering notions 
 
 ### Syntax
 
 ```
 Usage: knowledge cluster [OPTIONS]
 
-  Edit a NOTION file using the knowledges present in a DIAGNOSE file.
+  Defines, as a comment and in the knowledge files, all the knowledges
+  occuring in the file.
 
 Options:
   -k, --knowledge FILE      File containing the knowledges that are already
-                            defined.  [required]
+                            defined. Multiple files are allowed; new
+                            knowledges will be written in the last one.
+                            [required]
   -d, --diagnose FILE       Diagnose file produced by LaTeX.  [required]
   -l, --lang [en|fr]        Language of your TeX document.
-  -S, --scope / --no-scope  Print the scopes defined in the notion file and
+  -S, --scope / --no-scope  Print the scopes defined in the knowledge file and
                             print the possible meaning of those scope inferred
                             by knowledge-clustering.
   -c, --config-file TEXT    Specify the configuration file. By default the
                             configuration file in the folder
-                            <knowledge-clustering-installation-
-                            folder>/knowledge_clustering/data/ corresponding
+                            <knowledge-clustering-installation-folder>/data corresponding
                             to your language is used.
   --help                    Show this message and exit.
 ```
 
 ### Example
 
 Example files can be found in the `examples/` folder.
 
-While writing some document, you have defined some knowledges in a file called `ordinal-kl.tex` (distinct
+While writing some document, you have defined some knowledges in a file called `ordinal.kl` (distinct
 from your main `LaTeX`).
 You continued writing your `LaTeX` document (not provided in the `examples/` folder)
 for some time, and used some knowledges that were undefined.
 When compiling, `LaTeX` and the [`knowledge package`](https://ctan.org/pkg/knowledge) gives you a warning
 and writes in a `.diagnose` file some information explaining what went wrong. This `.diagnose` file contains
 a section called "Undefined knowledges" containing all knowledges used in your main `LaTeX` file but not
-defined in `ordinal-kl.tex`. We reproduced this section
+defined in `ordinal.kl`. We reproduced this section
 in the `ordinal.diagnose` file.
 
-![Screenshot of the `small.tex` and `small.diagnose` files before running knowledge-clustering. `small.tex` contains four knowledges, while `small.diagnose` contains five undefined knowledges.](img/small-before.png "Files `small.tex` and `small.diagnose` before running knowledge-clustering")
+![Screenshot of the `ordinal.kl` and `ordinal.diagnose` files before running knowledge-clustering. `ordinal.kl` contains four knowledges, while `ordinal.diagnose` contains five undefined knowledges.](img/small-before.png "Files `ordinal.kl` and `ordinal.diagnose` before running knowledge-clustering")
 
 Normally, you would add every undefined knowledge, one after the other, in your
-`oridnal-kl.tex`. This is quite burdensome and can
+`oridnal.kl`. This is quite burdensome and can
 largely be automated. This is precisely what `knowledge-clustering` does: after running
 
-    knowledge cluster -k small.tex -d small.diagnose
+    knowledge cluster -k ordinal.kl -d ordinal.diagnose
 
 your file `ordinal.diagnose` is left unchanged
-but `ordinal-kl.tex` is updated with comments.
+but `ordinal.kl` is updated with comments.
 
-The `cluster` command is optional: you can also write `knowledge -k ordinal-kl.tex -d ordinal.diagnose`.
+The `cluster` command is optional: you can also write `knowledge -k ordinal.kl -d ordinal.diagnose`.
 
-![After running knowledge-clustering, the five undefined knowledges are included in the `small.tex` file as comments.](img/small-after.png "Files `ordinal-kl.tex` and `ordinal.diagnose` after running knowledge-clustering`")
+![After running knowledge-clustering, the five undefined knowledges are included in the `ordinal.kl` file as comments.](img/small-after.png "Files `ordinal.kl` and `ordinal.diagnose` after running knowledge-clustering`")
 
-Now you simply have to check that the recommandations of `knowledge-clustering` are
+Now you simply have to check that the recommendations of `knowledge-clustering` are
 correct, and uncomment those lines.
 
+### Multiple knowledge files
+
+If you have **multiple knowledge files**, you can use the `-k` option multiple times.
+For instance, you could write:
+
+	knowledge cluster -k 1.kl -k 2.kl -d ordinal.diagnose
+
+Synonyms of knowledges defined in `1.kl` (resp. `2.kl`) will be defined, as comments,
+in `1.kl` (resp. `2.kl`). New knowledges will always be added, as comments, to the last
+file, which is `2.kl` in the example.
+
 ## Adding quotes
 
 ```
 Usage: knowledge addquotes [OPTIONS]
 
-  Finds knowledges defined in KNOWLEDGE that appear in TEX without quote
-  symbols. Proposes to add quotes around them.
+  Finds knowledges defined in the knowledge files that appear in tex file
+  without quote symbols. Proposes to add quotes around them.
 
 Options:
   -t, --tex FILE        Your TeX file.  [required]
   -k, --knowledge FILE  File containing the knowledges that are already
-                        defined.  [required]
+                        defined. Multiple files are allowed; new knowledges
+                        will be written in the last one.  [required]
   -p, --print INTEGER   When finding a match, number of lines (preceding the
                         match) that are printed in the prompt to the user.
   --help                Show this message and exit.
 ```
 
 After running 
 
-    knowledge addquotes -t mydocument.tex -k knowledges.tex
+    knowledge addquotes -t mydocument.tex -k knowledges1.kl -k knowledges2.kl
 
 your prompt will propose to add quotes around defined knowledges,
 and to define synonyms of knowledges that occur in your TeX file. For instance, if
 "algorithm" is a defined knowledge and "algorithms" occurs in your TeX file, then
 it will propose to you to define "algorithms" as a synonym of the knowledge "algorithm",
 and to add a pair of quotes around the string "algorithms" that occurs in your TeX file.
 
@@ -182,14 +200,18 @@
 python3 -m venv kl.venv
 source ./kl.venv/bin/activate.fish
 pip3 install --editable .
 ```
 
 ## FAQ
 
+- `knowledge: command not found` after installing `knowledge-clustering`
+
+  **Solution**: make sure you have Python>=3.9.
+  
 - When running `knowledge`, I obtain a long message error indicating "Resource punkt not found."
 
   **Solution**: run `knowledge init`.
 
 - My shell doesn't autocomplete the command `knowledge`.
 
   **Solution**: depending on whether you use `zsh` or `bash` write
@@ -197,15 +219,15 @@
        eval "`pip completion --<shellname>`"
 
   (where `<shellname>` is either `zsh` or `bash`)
   in your `.zshrc` (or `.bashrc`) file and then,
   either launch a new terminal or run `source ~/.zshrc`
   (or `source ~/.bashrc`).
 
-- I've updated `knowledge-clustering` but I still don't have the last version:
+- I've updated `knowledge-clustering` but I still don't have the last version (which can be checked using `knowledge --version`):
 
   This can happen if you have multiple versions of `python` (and multiple versions
   of `knowledge-clustering`).
   **Solution**: Type `where python3`, and uninstall `knowledge-clustering`
   from everywhere (using `<path>/python3 -m pip uninstall knowledge-clustering`)
   except your main version of python. Try to then upgrade `knowledge-clustering`
   by running `pip3 install --upgrade knowledge-clustering`.
```

### Comparing `knowledge-clustering-0.5.5/knowledge_clustering.egg-info/SOURCES.txt` & `knowledge-clustering-0.6.0/knowledge_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/setup.cfg` & `knowledge-clustering-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/tests/test_addquotes.py` & `knowledge-clustering-0.6.0/tests/test_addquotes.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Tests the addquotes command."""
     shutil.copy("tests/.ordinal.tex.original", "tests/ordinal.tex")
     shutil.copy("tests/.ordinal-kl.tex.original", "tests/ordinal-kl.tex")
     with open("tests/yes.txt", "w", encoding="utf-8") as yes:
         yes.write("y\n" * 100)
     with open("tests/yes.txt", "r", encoding="utf-8") as inp:
         with open("tests/output_addquotes.txt", "w", encoding="utf-8") as out:
-            app_addquotes("tests/ordinal.tex", "tests/ordinal-kl.tex", 1, inp, out)
+            app_addquotes("tests/ordinal.tex", ["tests/ordinal-kl.tex"], 1, inp, out)
     with open("tests/output_addquotes.txt", "r", encoding="utf-8") as out:
         nb_line_output = sum(1 for _ in out)
     b: bool = nb_line_output == 7
     os.remove("tests/yes.txt")
     os.remove("tests/ordinal.tex")
     os.remove("tests/ordinal-kl.tex")
     os.remove("tests/output_addquotes.txt")
```

### Comparing `knowledge-clustering-0.5.5/tests/test_anchor.py` & `knowledge-clustering-0.6.0/tests/test_anchor.py`

 * *Files identical despite different names*

### Comparing `knowledge-clustering-0.5.5/tests/test_clustering.py` & `knowledge-clustering-0.6.0/tests/test_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,17 @@
     assert compare(kls.get_all_bags(), solution)
 
 
 def test_app_clustering() -> None:
     """Tests the cluster command."""
     for filename in ["ordinal-kl.tex", "ordinal.diagnose"]:
         shutil.copy(f"tests/.{filename}.original", f"tests/{filename}")
-    app_clustering("tests/ordinal-kl.tex", "tests/ordinal.diagnose", False, "en", None)
+    app_clustering(
+        ["tests/ordinal-kl.tex"], "tests/ordinal.diagnose", False, "en", None
+    )
     # Diagnose file should be left unchanged…
     assert filecmp.cmp(
         "tests/ordinal.diagnose", "tests/.ordinal.diagnose.original", shallow=False
     )
     # Check if knowledge file has good content
     assert filecmp.cmp(
         "tests/ordinal-kl.tex", "tests/.ordinal-kl.tex.solution", shallow=False
```

