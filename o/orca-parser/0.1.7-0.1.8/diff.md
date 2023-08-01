# Comparing `tmp/orca_parser-0.1.7-py2.py3-none-any.whl.zip` & `tmp/orca_parser-0.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6998 bytes, number of entries: 8
+Zip file size: 7025 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3325 b- defN 23-Jul-06 09:45 orca_parser/HessianTools.py
--rw-rw-rw-  2.0 fat    12207 b- defN 23-Jul-28 23:40 orca_parser/ORCAParse.py
+-rw-rw-rw-  2.0 fat    12317 b- defN 23-Aug-01 20:49 orca_parser/ORCAParse.py
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-06 09:50 orca_parser/__init__.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-28 23:40 orca_parser-0.1.7.dist-info/RECORD
-8 files, 18309 bytes uncompressed, 5862 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      651 b- defN 23-Aug-01 20:50 orca_parser-0.1.8.dist-info/RECORD
+8 files, 18419 bytes uncompressed, 5889 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: orca_parser/ORCAParse.py
 Comment: 
 
 Filename: orca_parser/__init__.py
 Comment: 
 
-Filename: orca_parser-0.1.7.dist-info/LICENSE
+Filename: orca_parser-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: orca_parser-0.1.7.dist-info/METADATA
+Filename: orca_parser-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: orca_parser-0.1.7.dist-info/WHEEL
+Filename: orca_parser-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: orca_parser-0.1.7.dist-info/top_level.txt
+Filename: orca_parser-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: orca_parser-0.1.7.dist-info/RECORD
+Filename: orca_parser-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orca_parser/ORCAParse.py

```diff
@@ -190,29 +190,31 @@
         seconds = seconds + (miliseconds/1000)
         return seconds
     
     def parse_input(self):
         self.Z = int(round(float(self.raw.split("Sum of atomic charges:")[1].split("\n")[0])))
         self.Multiplicity = int(round(float(self.raw.split("* xyz")[1].replace("file","").split("\n")[0].split()[1])))
         self.orca_version = self.raw.split("Program Version ")[1].split()[0]
-        inp = self.raw.split("|  1>")[1].split("\n")[0]
+        inp = self.raw.split("INPUT FILE")[1].split("****END OF INPUT****")[0]
+        inp = inp.split("> !")[1].split("\n")[0]
         inp = inp.upper()
         inp = inp.replace("!", "")
         inp = inp.split()
         inp_dict = {"Job": None, 
                     "Freq": False,
                     "Solvation": "Gas",
                     "Dispersion": None,
                     "Charge": self.Z,
                     "defgrid": None,
                     "def2/J": None,
                     "Multiplicity": self.Multiplicity,
                     "orca_version": self.orca_version}
         i = 0
         while i < len(inp):
+            inp[i] = inp[i].upper()
             if inp[i] in ["SP", "OPT"]:
                 inp_dict["Job"] = inp[i]
                 del inp[i]
                 continue
             elif "FREQ" in inp[i]:
                 inp_dict["Freq"] = True
                 del inp[i]
```

## Comparing `orca_parser-0.1.7.dist-info/LICENSE` & `orca_parser-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

