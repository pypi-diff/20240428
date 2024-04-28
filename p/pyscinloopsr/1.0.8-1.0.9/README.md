# Comparing `tmp/pyscinloopsr-1.0.8.tar.gz` & `tmp/pyscinloopsr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscinloopsr-1.0.8.tar", last modified: Fri Apr 26 23:39:55 2024, max compression
+gzip compressed data, was "pyscinloopsr-1.0.9.tar", last modified: Fri Apr 26 23:52:53 2024, max compression
```

## Comparing `pyscinloopsr-1.0.8.tar` & `pyscinloopsr-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 23:39:55.232065 pyscinloopsr-1.0.8/
--rw-rw-rw-   0        0        0       42 2024-04-05 06:04:28.000000 pyscinloopsr-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      815 2024-04-26 23:39:55.232065 pyscinloopsr-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 05:31:15.000000 pyscinloopsr-1.0.8/README.md
--rw-rw-rw-   0        0        0     1427 2024-04-26 23:39:27.000000 pyscinloopsr-1.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-26 23:39:55.200809 pyscinloopsr-1.0.8/pyscinloopsr/
--rw-rw-rw-   0        0        0        0 2024-04-05 05:31:53.000000 pyscinloopsr-1.0.8/pyscinloopsr/__init__.py
--rw-rw-rw-   0        0        0      508 2024-04-05 09:45:13.000000 pyscinloopsr-1.0.8/pyscinloopsr/__main__.py
--rw-rw-rw-   0        0        0    12830 2024-04-26 23:39:20.000000 pyscinloopsr-1.0.8/pyscinloopsr/before.py
--rw-rw-rw-   0        0        0      211 2024-04-25 20:59:05.000000 pyscinloopsr-1.0.8/pyscinloopsr/test_before.py
-drwxrwxrwx   0        0        0        0 2024-04-26 23:39:55.216434 pyscinloopsr-1.0.8/pyscinloopsr.egg-info/
--rw-rw-rw-   0        0        0      815 2024-04-26 23:39:55.000000 pyscinloopsr-1.0.8/pyscinloopsr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-04-26 23:39:55.000000 pyscinloopsr-1.0.8/pyscinloopsr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 23:39:55.000000 pyscinloopsr-1.0.8/pyscinloopsr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-26 23:39:55.000000 pyscinloopsr-1.0.8/pyscinloopsr.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2024-04-26 23:39:55.000000 pyscinloopsr-1.0.8/pyscinloopsr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-26 23:39:55.000000 pyscinloopsr-1.0.8/pyscinloopsr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-26 23:39:55.232065 pyscinloopsr-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      449 2024-04-26 23:39:32.000000 pyscinloopsr-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:52:53.533640 pyscinloopsr-1.0.9/
+-rw-rw-rw-   0        0        0       42 2024-04-05 06:04:28.000000 pyscinloopsr-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      815 2024-04-26 23:52:53.533640 pyscinloopsr-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 05:31:15.000000 pyscinloopsr-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1427 2024-04-26 23:52:33.000000 pyscinloopsr-1.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-26 23:52:53.518011 pyscinloopsr-1.0.9/pyscinloopsr/
+-rw-rw-rw-   0        0        0        0 2024-04-05 05:31:53.000000 pyscinloopsr-1.0.9/pyscinloopsr/__init__.py
+-rw-rw-rw-   0        0        0      508 2024-04-05 09:45:13.000000 pyscinloopsr-1.0.9/pyscinloopsr/__main__.py
+-rw-rw-rw-   0        0        0    12845 2024-04-26 23:52:27.000000 pyscinloopsr-1.0.9/pyscinloopsr/before.py
+-rw-rw-rw-   0        0        0      211 2024-04-25 20:59:05.000000 pyscinloopsr-1.0.9/pyscinloopsr/test_before.py
+drwxrwxrwx   0        0        0        0 2024-04-26 23:52:53.533640 pyscinloopsr-1.0.9/pyscinloopsr.egg-info/
+-rw-rw-rw-   0        0        0      815 2024-04-26 23:52:53.000000 pyscinloopsr-1.0.9/pyscinloopsr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-04-26 23:52:53.000000 pyscinloopsr-1.0.9/pyscinloopsr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 23:52:53.000000 pyscinloopsr-1.0.9/pyscinloopsr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-26 23:52:53.000000 pyscinloopsr-1.0.9/pyscinloopsr.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-04-26 23:52:53.000000 pyscinloopsr-1.0.9/pyscinloopsr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-26 23:52:53.000000 pyscinloopsr-1.0.9/pyscinloopsr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 23:52:53.533640 pyscinloopsr-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      449 2024-04-26 23:52:38.000000 pyscinloopsr-1.0.9/setup.py
```

### Comparing `pyscinloopsr-1.0.8/PKG-INFO` & `pyscinloopsr-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscinloopsr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Read the latest PyScInLoopSr tutorials
 Author: Djalma Pereira
 Author-email: Djalma Pereira <pereirajunio@gmail.com>
 Project-URL: Homepage, https://github.com/realpython/reader
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyscinloopsr-1.0.8/pyproject.toml` & `pyscinloopsr-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyscinloopsr"
-version = "1.0.8"
+version = "1.0.9"
 description = "Read the latest PyScInLoopSr tutorials"
 readme = "README.md"
 authors = [{ name = "Djalma Pereira", email = "pereirajunio@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyscinloopsr-1.0.8/pyscinloopsr/before.py` & `pyscinloopsr-1.0.9/pyscinloopsr/before.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,122 +681,123 @@
 00002a80: 696e 696e 6754 696d 6522 5d0d 0a0d 0a0d  iningTime"].....
 00002a90: 0a0d 0a20 2020 206a 203d 2031 0d0a 2020  ...    j = 1..  
 00002aa0: 2020 666f 7220 6920 696e 206d 6f64 656c    for i in model
 00002ab0: 733a 0d0a 2020 2020 2020 2020 7468 656e  s:..        then
 00002ac0: 203d 2064 6174 6574 696d 652e 6e6f 7728   = datetime.now(
 00002ad0: 290d 0a0d 0a20 2020 2020 2020 2069 2e66  )....        i.f
 00002ae0: 6974 2858 5f74 7261 696e 2c20 795f 7472  it(X_train, y_tr
-00002af0: 6169 6e29 0d0a 2020 2020 2020 2020 795f  ain)..        y_
-00002b00: 7265 7320 3d20 692e 7072 6564 6963 7428  res = i.predict(
-00002b10: 585f 7465 7374 290d 0a0d 0a20 2020 2020  X_test)....     
-00002b20: 2020 206e 6f77 203d 2064 6174 6574 696d     now = datetim
-00002b30: 652e 6e6f 7728 290d 0a20 2020 2020 2020  e.now()..       
-00002b40: 2070 7269 6e74 2028 2254 656d 706f 2064   print ("Tempo d
-00002b50: 6520 7072 6f63 6573 7361 6d65 6e74 6f20  e processamento 
-00002b60: 646f 2022 2c74 7970 6528 6929 2e5f 5f6e  do ",type(i).__n
-00002b70: 616d 655f 5f2c 223a 2022 2c20 6e6f 772d  ame__,": ", now-
-00002b80: 7468 656e 290d 0a20 2020 2020 2020 206d  then)..        m
-00002b90: 7365 203d 206d 6561 6e5f 7371 7561 7265  se = mean_square
-00002ba0: 645f 6572 726f 7228 795f 7465 7374 2c20  d_error(y_test, 
-00002bb0: 795f 7265 7329 0d0a 2020 2020 2020 2020  y_res)..        
-00002bc0: 7232 203d 206d 6574 7269 6373 2e72 325f  r2 = metrics.r2_
-00002bd0: 7363 6f72 6528 795f 7465 7374 2c20 795f  score(y_test, y_
-00002be0: 7265 7329 0d0a 2020 2020 2020 2020 7363  res)..        sc
-00002bf0: 6f72 6520 3d20 692e 7363 6f72 6528 585f  ore = i.score(X_
-00002c00: 7465 7374 2c20 795f 7465 7374 290d 0a0d  test, y_test)...
-00002c10: 0a20 2020 2020 2020 206e 6577 4c69 6e65  .        newLine
-00002c20: 203d 205b 7479 7065 2869 292e 5f5f 6e61   = [type(i).__na
-00002c30: 6d65 5f5f 2c20 666f 726d 6174 286d 7365  me__, format(mse
-00002c40: 2c20 272c 2e32 6627 292c 2066 6f72 6d61  , ',.2f'), forma
-00002c50: 7428 7363 6f72 652c 2027 2e32 6627 292c  t(score, '.2f'),
-00002c60: 2066 6f72 6d61 7428 7232 2c20 272e 3266   format(r2, '.2f
-00002c70: 2729 2c20 6e6f 772d 7468 656e 5d0d 0a0d  '), now-then]...
-00002c80: 0a20 2020 2020 2020 2069 6620 7232 3e30  .        if r2>0
-00002c90: 2e39 3a0d 0a20 2020 2020 2020 2020 206e  .9:..          n
-00002ca0: 6577 4c69 6e65 5b33 5d20 3d20 436f 6e73  ewLine[3] = Cons
-00002cb0: 6f6c 6543 6f6c 6f72 2e42 4c55 4520 2b20  oleColor.BLUE + 
-00002cc0: 6e65 774c 696e 655b 335d 202b 2043 6f6e  newLine[3] + Con
-00002cd0: 736f 6c65 436f 6c6f 722e 454e 440d 0a20  soleColor.END.. 
-00002ce0: 2020 2020 2020 2065 6c69 6620 7232 3e30         elif r2>0
-00002cf0: 2e38 3a0d 0a20 2020 2020 2020 2020 206e  .8:..          n
-00002d00: 6577 4c69 6e65 5b33 5d20 3d20 436f 6e73  ewLine[3] = Cons
-00002d10: 6f6c 6543 6f6c 6f72 2e47 5245 454e 202b  oleColor.GREEN +
-00002d20: 206e 6577 4c69 6e65 5b33 5d20 2b20 436f   newLine[3] + Co
-00002d30: 6e73 6f6c 6543 6f6c 6f72 2e45 4e44 0d0a  nsoleColor.END..
-00002d40: 2020 2020 2020 2020 656c 6966 2072 323e          elif r2>
-00002d50: 302e 363a 0d0a 2020 2020 2020 2020 2020  0.6:..          
-00002d60: 6e65 774c 696e 655b 335d 203d 2043 6f6e  newLine[3] = Con
-00002d70: 736f 6c65 436f 6c6f 722e 5055 5250 4c45  soleColor.PURPLE
-00002d80: 202b 206e 6577 4c69 6e65 5b33 5d20 2b20   + newLine[3] + 
-00002d90: 436f 6e73 6f6c 6543 6f6c 6f72 2e45 4e44  ConsoleColor.END
-00002da0: 0d0a 2020 2020 2020 2020 656c 6966 2072  ..        elif r
-00002db0: 323e 302e 343a 0d0a 2020 2020 2020 2020  2>0.4:..        
-00002dc0: 2020 6e65 774c 696e 655b 335d 203d 2043    newLine[3] = C
-00002dd0: 6f6e 736f 6c65 436f 6c6f 722e 5245 4420  onsoleColor.RED 
-00002de0: 2b20 6e65 774c 696e 655b 335d 202b 2043  + newLine[3] + C
-00002df0: 6f6e 736f 6c65 436f 6c6f 722e 454e 440d  onsoleColor.END.
-00002e00: 0a0d 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020  ...........     
-00002e10: 2020 2074 6162 6c65 2e61 6464 5f72 6f77     table.add_row
-00002e20: 286e 6577 4c69 6e65 290d 0a0d 0a0d 0a20  (newLine)...... 
-00002e30: 2020 2020 2020 2023 6d79 7461 626c 6520         #mytable 
-00002e40: 3d20 5072 6574 7479 5461 626c 6528 5b27  = PrettyTable(['
-00002e50: 4e61 6d65 272c 2027 4167 6527 2c20 2743  Name', 'Age', 'C
-00002e60: 6974 7927 2c20 2753 6578 272c 2027 4d61  ity', 'Sex', 'Ma
-00002e70: 7269 7461 6c27 2c20 2750 686f 6e65 4e6f  rital', 'PhoneNo
-00002e80: 275d 290d 0a20 2020 2020 2020 2023 666f  '])..        #fo
-00002e90: 7220 7820 696e 2070 656f 706c 653a 0d0a  r x in people:..
-00002ea0: 2020 2020 2020 2020 236c 6973 203d 205b          #lis = [
-00002eb0: 7820 666f 7220 7820 696e 2070 656f 706c  x for x in peopl
-00002ec0: 655d 0d0a 2020 2020 2020 2020 236c 6920  e]..        #li 
-00002ed0: 3d20 5b79 2066 6f72 2078 2c20 7920 696e  = [y for x, y in
-00002ee0: 2070 656f 706c 655b 785d 2e69 7465 6d73   people[x].items
-00002ef0: 2829 5d0d 0a20 2020 2020 2020 2023 6c69  ()]..        #li
-00002f00: 5b31 5d20 3d20 436f 6e73 6f6c 6543 6f6c  [1] = ConsoleCol
-00002f10: 6f72 2e47 5245 454e 202b 206c 695b 315d  or.GREEN + li[1]
-00002f20: 202b 2043 6f6e 736f 6c65 436f 6c6f 722e   + ConsoleColor.
-00002f30: 454e 440d 0a20 2020 2020 2020 2023 6d79  END..        #my
-00002f40: 7461 626c 652e 6164 645f 726f 7728 6c69  table.add_row(li
-00002f50: 290d 0a20 2020 2020 2020 2023 7461 626c  )..        #tabl
-00002f60: 652e 6164 645f 726f 7728 5b74 7970 6528  e.add_row([type(
-00002f70: 6929 2e5f 5f6e 616d 655f 5f2c 2066 6f72  i).__name__, for
-00002f80: 6d61 7428 6d73 652c 2027 2c2e 3266 2729  mat(mse, ',.2f')
-00002f90: 2c20 666f 726d 6174 2873 636f 7265 2c20  , format(score, 
-00002fa0: 272e 3266 2729 2c20 666f 726d 6174 2872  '.2f'), format(r
-00002fb0: 322c 2027 2e32 6627 292c 206e 6f77 2d74  2, '.2f'), now-t
-00002fc0: 6865 6e5d 290d 0a0d 0a20 2020 2020 2020  hen])....       
-00002fd0: 2023 6d6f 6465 6c5f 7361 7665 5f6e 616d   #model_save_nam
-00002fe0: 6520 3d20 7479 7065 286d 6f64 656c 292e  e = type(model).
-00002ff0: 5f5f 6e61 6d65 5f5f 202b 2073 7472 2869  __name__ + str(i
-00003000: 2920 2b20 225f 6578 6563 315f 7365 6d54  ) + "_exec1_semT
-00003010: 7261 7461 6d65 6e74 6f73 2e70 7422 0d0a  ratamentos.pt"..
-00003020: 2020 2020 2020 2020 2370 6174 6820 3d20          #path = 
-00003030: 4622 2f63 6f6e 7465 6e74 2f64 7269 7665  F"/content/drive
-00003040: 2f4d 7944 7269 7665 2f64 6174 612f 6469  /MyDrive/data/di
-00003050: 7373 6572 7461 6361 6f2f 6d6f 6e69 7175  ssertacao/moniqu
-00003060: 6555 6661 6263 2f56 322f 5341 5645 442f  eUfabc/V2/SAVED/
-00003070: 6379 636c 6531 2f7b 6d6f 6465 6c5f 7361  cycle1/{model_sa
-00003080: 7665 5f6e 616d 657d 220d 0a20 2020 2020  ve_name}"..     
-00003090: 2020 2023 7261 697a 203d 2022 2f63 6f6e     #raiz = "/con
-000030a0: 7465 6e74 2f64 7269 7665 2f4d 7944 7269  tent/drive/MyDri
-000030b0: 7665 2f64 6174 612f 6469 7373 6572 7461  ve/data/disserta
-000030c0: 6361 6f2f 6d6f 6e69 7175 6555 6661 6263  cao/moniqueUfabc
-000030d0: 2f56 3222 0d0a 2020 2020 2020 2020 2363  /V2"..        #c
-000030e0: 7963 6c65 203d 2022 2f63 7963 6c65 3122  ycle = "/cycle1"
-000030f0: 2020 2020 2020 2020 2023 2059 4f55 2048           # YOU H
-00003100: 4156 4520 544f 2041 444a 5553 5420 544f  AVE TO ADJUST TO
-00003110: 2054 4845 2043 5552 5245 4e54 2043 5943   THE CURRENT CYC
-00003120: 4c45 2028 4e4f 5420 4f56 4552 5752 4954  LE (NOT OVERWRIT
-00003130: 4529 2041 4e44 2054 4845 4e20 554e 434f  E) AND THEN UNCO
-00003140: 4d4d 454e 540d 0a20 2020 2020 2020 2023  MMENT..        #
-00003150: 7061 7468 203d 2046 2222 2b28 7261 697a  path = F""+(raiz
-00003160: 2b22 2f53 4156 4544 222b 6379 636c 652b  +"/SAVED"+cycle+
-00003170: 222f 7b6d 6f64 656c 5f73 6176 655f 6e61  "/{model_save_na
-00003180: 6d65 7d22 290d 0a20 2020 2020 2020 2023  me}")..        #
-00003190: 746f 7263 682e 7361 7665 286d 6f64 656c  torch.save(model
-000031a0: 2c20 7061 7468 290d 0a0d 0a0d 0a20 2020  , path)......   
-000031b0: 2020 2020 206a 203d 206a 202b 2031 0d0a       j = j + 1..
-000031c0: 0d0a 0d0a 2020 2020 7365 6c66 2e70 7265  ....    self.pre
-000031d0: 7474 7974 6162 6c65 203d 2074 6162 6c65  ttytable = table
-000031e0: 0d0a 2020 2020 7072 696e 7428 7365 6c66  ..    print(self
-000031f0: 2e70 7265 7474 7974 6162 6c65 290d 0a0d  .prettytable)...
-00003200: 0a20 2020 2072 6574 7572 6e20 7365 6c66  .    return self
-00003210: 2e70 7265 7474 7974 6162 6c65 0d0a       .prettytable..
+00002af0: 6169 6e2e 7661 6c75 6573 2e72 6176 656c  ain.values.ravel
+00002b00: 2829 290d 0a20 2020 2020 2020 2079 5f72  ())..        y_r
+00002b10: 6573 203d 2069 2e70 7265 6469 6374 2858  es = i.predict(X
+00002b20: 5f74 6573 7429 0d0a 0d0a 2020 2020 2020  _test)....      
+00002b30: 2020 6e6f 7720 3d20 6461 7465 7469 6d65    now = datetime
+00002b40: 2e6e 6f77 2829 0d0a 2020 2020 2020 2020  .now()..        
+00002b50: 7072 696e 7420 2822 5465 6d70 6f20 6465  print ("Tempo de
+00002b60: 2070 726f 6365 7373 616d 656e 746f 2064   processamento d
+00002b70: 6f20 222c 7479 7065 2869 292e 5f5f 6e61  o ",type(i).__na
+00002b80: 6d65 5f5f 2c22 3a20 222c 206e 6f77 2d74  me__,": ", now-t
+00002b90: 6865 6e29 0d0a 2020 2020 2020 2020 6d73  hen)..        ms
+00002ba0: 6520 3d20 6d65 616e 5f73 7175 6172 6564  e = mean_squared
+00002bb0: 5f65 7272 6f72 2879 5f74 6573 742c 2079  _error(y_test, y
+00002bc0: 5f72 6573 290d 0a20 2020 2020 2020 2072  _res)..        r
+00002bd0: 3220 3d20 6d65 7472 6963 732e 7232 5f73  2 = metrics.r2_s
+00002be0: 636f 7265 2879 5f74 6573 742c 2079 5f72  core(y_test, y_r
+00002bf0: 6573 290d 0a20 2020 2020 2020 2073 636f  es)..        sco
+00002c00: 7265 203d 2069 2e73 636f 7265 2858 5f74  re = i.score(X_t
+00002c10: 6573 742c 2079 5f74 6573 7429 0d0a 0d0a  est, y_test)....
+00002c20: 2020 2020 2020 2020 6e65 774c 696e 6520          newLine 
+00002c30: 3d20 5b74 7970 6528 6929 2e5f 5f6e 616d  = [type(i).__nam
+00002c40: 655f 5f2c 2066 6f72 6d61 7428 6d73 652c  e__, format(mse,
+00002c50: 2027 2c2e 3266 2729 2c20 666f 726d 6174   ',.2f'), format
+00002c60: 2873 636f 7265 2c20 272e 3266 2729 2c20  (score, '.2f'), 
+00002c70: 666f 726d 6174 2872 322c 2027 2e32 6627  format(r2, '.2f'
+00002c80: 292c 206e 6f77 2d74 6865 6e5d 0d0a 0d0a  ), now-then]....
+00002c90: 2020 2020 2020 2020 6966 2072 323e 302e          if r2>0.
+00002ca0: 393a 0d0a 2020 2020 2020 2020 2020 6e65  9:..          ne
+00002cb0: 774c 696e 655b 335d 203d 2043 6f6e 736f  wLine[3] = Conso
+00002cc0: 6c65 436f 6c6f 722e 424c 5545 202b 206e  leColor.BLUE + n
+00002cd0: 6577 4c69 6e65 5b33 5d20 2b20 436f 6e73  ewLine[3] + Cons
+00002ce0: 6f6c 6543 6f6c 6f72 2e45 4e44 0d0a 2020  oleColor.END..  
+00002cf0: 2020 2020 2020 656c 6966 2072 323e 302e        elif r2>0.
+00002d00: 383a 0d0a 2020 2020 2020 2020 2020 6e65  8:..          ne
+00002d10: 774c 696e 655b 335d 203d 2043 6f6e 736f  wLine[3] = Conso
+00002d20: 6c65 436f 6c6f 722e 4752 4545 4e20 2b20  leColor.GREEN + 
+00002d30: 6e65 774c 696e 655b 335d 202b 2043 6f6e  newLine[3] + Con
+00002d40: 736f 6c65 436f 6c6f 722e 454e 440d 0a20  soleColor.END.. 
+00002d50: 2020 2020 2020 2065 6c69 6620 7232 3e30         elif r2>0
+00002d60: 2e36 3a0d 0a20 2020 2020 2020 2020 206e  .6:..          n
+00002d70: 6577 4c69 6e65 5b33 5d20 3d20 436f 6e73  ewLine[3] = Cons
+00002d80: 6f6c 6543 6f6c 6f72 2e50 5552 504c 4520  oleColor.PURPLE 
+00002d90: 2b20 6e65 774c 696e 655b 335d 202b 2043  + newLine[3] + C
+00002da0: 6f6e 736f 6c65 436f 6c6f 722e 454e 440d  onsoleColor.END.
+00002db0: 0a20 2020 2020 2020 2065 6c69 6620 7232  .        elif r2
+00002dc0: 3e30 2e34 3a0d 0a20 2020 2020 2020 2020  >0.4:..         
+00002dd0: 206e 6577 4c69 6e65 5b33 5d20 3d20 436f   newLine[3] = Co
+00002de0: 6e73 6f6c 6543 6f6c 6f72 2e52 4544 202b  nsoleColor.RED +
+00002df0: 206e 6577 4c69 6e65 5b33 5d20 2b20 436f   newLine[3] + Co
+00002e00: 6e73 6f6c 6543 6f6c 6f72 2e45 4e44 0d0a  nsoleColor.END..
+00002e10: 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020 2020  ..........      
+00002e20: 2020 7461 626c 652e 6164 645f 726f 7728    table.add_row(
+00002e30: 6e65 774c 696e 6529 0d0a 0d0a 0d0a 2020  newLine)......  
+00002e40: 2020 2020 2020 236d 7974 6162 6c65 203d        #mytable =
+00002e50: 2050 7265 7474 7954 6162 6c65 285b 274e   PrettyTable(['N
+00002e60: 616d 6527 2c20 2741 6765 272c 2027 4369  ame', 'Age', 'Ci
+00002e70: 7479 272c 2027 5365 7827 2c20 274d 6172  ty', 'Sex', 'Mar
+00002e80: 6974 616c 272c 2027 5068 6f6e 654e 6f27  ital', 'PhoneNo'
+00002e90: 5d29 0d0a 2020 2020 2020 2020 2366 6f72  ])..        #for
+00002ea0: 2078 2069 6e20 7065 6f70 6c65 3a0d 0a20   x in people:.. 
+00002eb0: 2020 2020 2020 2023 6c69 7320 3d20 5b78         #lis = [x
+00002ec0: 2066 6f72 2078 2069 6e20 7065 6f70 6c65   for x in people
+00002ed0: 5d0d 0a20 2020 2020 2020 2023 6c69 203d  ]..        #li =
+00002ee0: 205b 7920 666f 7220 782c 2079 2069 6e20   [y for x, y in 
+00002ef0: 7065 6f70 6c65 5b78 5d2e 6974 656d 7328  people[x].items(
+00002f00: 295d 0d0a 2020 2020 2020 2020 236c 695b  )]..        #li[
+00002f10: 315d 203d 2043 6f6e 736f 6c65 436f 6c6f  1] = ConsoleColo
+00002f20: 722e 4752 4545 4e20 2b20 6c69 5b31 5d20  r.GREEN + li[1] 
+00002f30: 2b20 436f 6e73 6f6c 6543 6f6c 6f72 2e45  + ConsoleColor.E
+00002f40: 4e44 0d0a 2020 2020 2020 2020 236d 7974  ND..        #myt
+00002f50: 6162 6c65 2e61 6464 5f72 6f77 286c 6929  able.add_row(li)
+00002f60: 0d0a 2020 2020 2020 2020 2374 6162 6c65  ..        #table
+00002f70: 2e61 6464 5f72 6f77 285b 7479 7065 2869  .add_row([type(i
+00002f80: 292e 5f5f 6e61 6d65 5f5f 2c20 666f 726d  ).__name__, form
+00002f90: 6174 286d 7365 2c20 272c 2e32 6627 292c  at(mse, ',.2f'),
+00002fa0: 2066 6f72 6d61 7428 7363 6f72 652c 2027   format(score, '
+00002fb0: 2e32 6627 292c 2066 6f72 6d61 7428 7232  .2f'), format(r2
+00002fc0: 2c20 272e 3266 2729 2c20 6e6f 772d 7468  , '.2f'), now-th
+00002fd0: 656e 5d29 0d0a 0d0a 2020 2020 2020 2020  en])....        
+00002fe0: 236d 6f64 656c 5f73 6176 655f 6e61 6d65  #model_save_name
+00002ff0: 203d 2074 7970 6528 6d6f 6465 6c29 2e5f   = type(model)._
+00003000: 5f6e 616d 655f 5f20 2b20 7374 7228 6929  _name__ + str(i)
+00003010: 202b 2022 5f65 7865 6331 5f73 656d 5472   + "_exec1_semTr
+00003020: 6174 616d 656e 746f 732e 7074 220d 0a20  atamentos.pt".. 
+00003030: 2020 2020 2020 2023 7061 7468 203d 2046         #path = F
+00003040: 222f 636f 6e74 656e 742f 6472 6976 652f  "/content/drive/
+00003050: 4d79 4472 6976 652f 6461 7461 2f64 6973  MyDrive/data/dis
+00003060: 7365 7274 6163 616f 2f6d 6f6e 6971 7565  sertacao/monique
+00003070: 5566 6162 632f 5632 2f53 4156 4544 2f63  Ufabc/V2/SAVED/c
+00003080: 7963 6c65 312f 7b6d 6f64 656c 5f73 6176  ycle1/{model_sav
+00003090: 655f 6e61 6d65 7d22 0d0a 2020 2020 2020  e_name}"..      
+000030a0: 2020 2372 6169 7a20 3d20 222f 636f 6e74    #raiz = "/cont
+000030b0: 656e 742f 6472 6976 652f 4d79 4472 6976  ent/drive/MyDriv
+000030c0: 652f 6461 7461 2f64 6973 7365 7274 6163  e/data/dissertac
+000030d0: 616f 2f6d 6f6e 6971 7565 5566 6162 632f  ao/moniqueUfabc/
+000030e0: 5632 220d 0a20 2020 2020 2020 2023 6379  V2"..        #cy
+000030f0: 636c 6520 3d20 222f 6379 636c 6531 2220  cle = "/cycle1" 
+00003100: 2020 2020 2020 2020 2320 594f 5520 4841          # YOU HA
+00003110: 5645 2054 4f20 4144 4a55 5354 2054 4f20  VE TO ADJUST TO 
+00003120: 5448 4520 4355 5252 454e 5420 4359 434c  THE CURRENT CYCL
+00003130: 4520 284e 4f54 204f 5645 5257 5249 5445  E (NOT OVERWRITE
+00003140: 2920 414e 4420 5448 454e 2055 4e43 4f4d  ) AND THEN UNCOM
+00003150: 4d45 4e54 0d0a 2020 2020 2020 2020 2370  MENT..        #p
+00003160: 6174 6820 3d20 4622 222b 2872 6169 7a2b  ath = F""+(raiz+
+00003170: 222f 5341 5645 4422 2b63 7963 6c65 2b22  "/SAVED"+cycle+"
+00003180: 2f7b 6d6f 6465 6c5f 7361 7665 5f6e 616d  /{model_save_nam
+00003190: 657d 2229 0d0a 2020 2020 2020 2020 2374  e}")..        #t
+000031a0: 6f72 6368 2e73 6176 6528 6d6f 6465 6c2c  orch.save(model,
+000031b0: 2070 6174 6829 0d0a 0d0a 0d0a 2020 2020   path)......    
+000031c0: 2020 2020 6a20 3d20 6a20 2b20 310d 0a0d      j = j + 1...
+000031d0: 0a0d 0a20 2020 2073 656c 662e 7072 6574  ...    self.pret
+000031e0: 7479 7461 626c 6520 3d20 7461 626c 650d  tytable = table.
+000031f0: 0a20 2020 2070 7269 6e74 2873 656c 662e  .    print(self.
+00003200: 7072 6574 7479 7461 626c 6529 0d0a 0d0a  prettytable)....
+00003210: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00003220: 7072 6574 7479 7461 626c 650d 0a         prettytable..
```

### Comparing `pyscinloopsr-1.0.8/pyscinloopsr.egg-info/PKG-INFO` & `pyscinloopsr-1.0.9/pyscinloopsr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscinloopsr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Read the latest PyScInLoopSr tutorials
 Author: Djalma Pereira
 Author-email: Djalma Pereira <pereirajunio@gmail.com>
 Project-URL: Homepage, https://github.com/realpython/reader
 Keywords: feed,reader,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

