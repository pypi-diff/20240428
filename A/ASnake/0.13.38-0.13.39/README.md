# Comparing `tmp/asnake-0.13.38.tar.gz` & `tmp/asnake-0.13.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asnake-0.13.38.tar", last modified: Thu Apr 18 16:22:45 2024, max compression
+gzip compressed data, was "asnake-0.13.39.tar", last modified: Sun Apr 28 01:50:00 2024, max compression
```

## Comparing `asnake-0.13.38.tar` & `asnake-0.13.39.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.694346 asnake-0.13.38/
--rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 asnake-0.13.38/LICENSE.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-18 16:22:45.694346 asnake-0.13.38/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 asnake-0.13.38/README.md
--rw-r--r--   0 ahri      (1002) ahri      (1002)     1495 2024-04-10 19:24:02.000000 asnake-0.13.38/pyproject.toml
--rw-r--r--   0 ahri      (1002) ahri      (1002)       38 2024-04-18 16:22:45.694346 asnake-0.13.38/setup.cfg
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.691013 asnake-0.13.38/src/
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.691013 asnake-0.13.38/src/ASnake/
--rwxr-xr-x   0 ahri      (1002) ahri      (1002)   526027 2024-04-18 16:12:15.000000 asnake-0.13.38/src/ASnake/ASnake.py
--rw-r--r--   0 ahri      (1002) ahri      (1002)        0 2024-04-10 18:46:25.000000 asnake-0.13.38/src/ASnake/__init__.py
--rw-r--r--   0 ahri      (1002) ahri      (1002)    19572 2024-04-11 22:48:22.000000 asnake-0.13.38/src/ASnake/__main__.py
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.694346 asnake-0.13.38/src/ASnake/data/
--rw-r--r--   0 ahri      (1002) ahri      (1002)       58 2024-04-10 18:07:02.000000 asnake-0.13.38/src/ASnake/data/ASnakeAlias.bat
--rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8841 2024-04-10 18:07:02.000000 asnake-0.13.38/src/ASnake/data/megaTest.asnake
--rw-r--r--   0 ahri      (1002) ahri      (1002)     3398 2024-04-10 18:07:02.000000 asnake-0.13.38/src/ASnake/data/setAlias.asnake
-drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-18 16:22:45.694346 asnake-0.13.38/src/ASnake.egg-info/
--rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/PKG-INFO
--rw-r--r--   0 ahri      (1002) ahri      (1002)      405 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/SOURCES.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/dependency_links.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       46 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/entry_points.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/requires.txt
--rw-r--r--   0 ahri      (1002) ahri      (1002)        7 2024-04-18 16:22:45.000000 asnake-0.13.38/src/ASnake.egg-info/top_level.txt
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-28 01:50:00.477104 asnake-0.13.39/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    11357 2021-09-03 10:06:02.000000 asnake-0.13.39/LICENSE.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-28 01:50:00.477104 asnake-0.13.39/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      814 2024-04-03 21:05:15.000000 asnake-0.13.39/README.md
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     1495 2024-04-10 19:24:02.000000 asnake-0.13.39/pyproject.toml
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       38 2024-04-28 01:50:00.477104 asnake-0.13.39/setup.cfg
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-28 01:50:00.473771 asnake-0.13.39/src/
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-28 01:50:00.473771 asnake-0.13.39/src/ASnake/
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)   539056 2024-04-28 01:49:08.000000 asnake-0.13.39/src/ASnake/ASnake.py
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        0 2024-04-10 18:46:25.000000 asnake-0.13.39/src/ASnake/__init__.py
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    19855 2024-04-18 16:28:25.000000 asnake-0.13.39/src/ASnake/__main__.py
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-28 01:50:00.477104 asnake-0.13.39/src/ASnake/data/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       58 2024-04-10 18:07:02.000000 asnake-0.13.39/src/ASnake/data/ASnakeAlias.bat
+-rwxr-xr-x   0 ahri      (1002) ahri      (1002)     8841 2024-04-10 18:07:02.000000 asnake-0.13.39/src/ASnake/data/megaTest.asnake
+-rw-r--r--   0 ahri      (1002) ahri      (1002)     3398 2024-04-10 18:07:02.000000 asnake-0.13.39/src/ASnake/data/setAlias.asnake
+drwxr-xr-x   0 ahri      (1002) ahri      (1002)        0 2024-04-28 01:50:00.477104 asnake-0.13.39/src/ASnake.egg-info/
+-rw-r--r--   0 ahri      (1002) ahri      (1002)    15023 2024-04-28 01:50:00.000000 asnake-0.13.39/src/ASnake.egg-info/PKG-INFO
+-rw-r--r--   0 ahri      (1002) ahri      (1002)      405 2024-04-28 01:50:00.000000 asnake-0.13.39/src/ASnake.egg-info/SOURCES.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        1 2024-04-28 01:50:00.000000 asnake-0.13.39/src/ASnake.egg-info/dependency_links.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       46 2024-04-28 01:50:00.000000 asnake-0.13.39/src/ASnake.egg-info/entry_points.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)       25 2024-04-28 01:50:00.000000 asnake-0.13.39/src/ASnake.egg-info/requires.txt
+-rw-r--r--   0 ahri      (1002) ahri      (1002)        7 2024-04-28 01:50:00.000000 asnake-0.13.39/src/ASnake.egg-info/top_level.txt
```

### Comparing `asnake-0.13.38/LICENSE.txt` & `asnake-0.13.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asnake-0.13.38/PKG-INFO` & `asnake-0.13.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.38
+Version: 0.13.39
 Summary: Python optimizing compiler for the ASnake programming language.
 Author: Ahri Fox
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `asnake-0.13.38/README.md` & `asnake-0.13.39/README.md`

 * *Files identical despite different names*

### Comparing `asnake-0.13.38/pyproject.toml` & `asnake-0.13.39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `asnake-0.13.38/src/ASnake/ASnake.py` & `asnake-0.13.39/src/ASnake/ASnake.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from re import compile as REcompile
 from re import search as REsearch
 from re import findall as REfindall
 from re import MULTILINE as REMULTILINE
 from keyword import iskeyword
 from unicodedata import category as unicodeCategory
 
-ASnakeVersion = 'v0.13.38'
+ASnakeVersion = 'v0.13.39'
 __version__ = ASnakeVersion[1:]
 
 def AS_SyntaxError(text=None,suggestion=None,lineNumber=0,code='',errorType='Syntax error'):
     showError=[]
     if text != None:
         showError.append(f'{errorType}:\n\t{text}')
     else:
@@ -133,17 +133,17 @@
     EQUAL   = r'==|equals?(?= |\t)'
     NOTIN   = r"isn'?t +in( |(?=\n))"
     NOTEQ   = r'!=|isnt|isn\'t|not +equal|unequal'
     LESSEQ  = r'(<=)|(=<)|≤'
     GREATEQ = r'(>=)|(=>)|≥'
     OR      = r'(\|\||or)(?= |\t)'
     BITWISE = r'(\^|~|\||&|(<<)|(>>))(?!=)'
+    ASSIGN  = r'''=|is( |(?=("|'|{|\[|\()))|(\+|-|\*\*?|\/\/?|:|%|>>|<<|\^|~|\||&)='''
     LESS    = r'<|((is )?less (than )?)|(lesser (than )?)'
     GREATER = r'>|((is )?greater (than )?)'
-    ASSIGN  = r'''=|is( |(?=("|'|{|\[|\()))|(\+|-|\*\*?|\/\/?|:|%|>>|<<|\^|~|\||&)='''
     ENDIF   = r': *'
     DEFFUNCT= r'(c|cp)?does(?= |\n|\t)'
     SCOPE   = r'(global|local|nonlocal) (\w* *,?)*'
     THEN    = r'((then|do|then +do|, +then|, +do|, +then +do)(?=\s))|;|(:(?=\n)+)'
     WITHAS  = r'(with|(?![^\w\d])as) '
     WHILE   = r'while '
     NOTHING = r'(pass|nothing,?)(?= |$|\n)'
@@ -518,19 +518,20 @@
                     if char == quoteType:
                         return newString
                     elif char == '\\':
                         escapeChar = True
                     else:
                         newString+=char
 
-    def isANegativeNumberTokens(lexIndex):
+    def isANegativeNumberTokens(suspectedMinusIndex):
         # arg should be suspected minus
-        if lex[lexIndex].type == 'MINUS' and lex[lexIndex+1].type == 'NUMBER' \
-        and lex[lexIndex-1].type not in {'ID','RPAREN','BUILTINF','NUMBER','STRING','RINDEX','LISTEND','RBRACKET'}:
+        if lex[suspectedMinusIndex].type == 'MINUS' and lex[suspectedMinusIndex+1].type == 'NUMBER' \
+        and lex[suspectedMinusIndex-1].type not in {'ID','RPAREN','BUILTINF','NUMBER','STRING','RINDEX','LISTEND','RBRACKET'}:
             return True
+        elif lex[suspectedMinusIndex].type == 'NUMBER' and lex[suspectedMinusIndex].value[0] == '-': return True
         return False
 
 
     def insertAtTopOfCodeIfItIsNotThere(line):
         nonlocal code
         if any(i for i in code if line in i):
             pass
@@ -620,14 +621,17 @@
                 returnValue = False
             else:
                 returnValue = True
         else:
             returnValue = not returnValue
         return returnValue
 
+    def debugPrintWholeScript():
+        [print(_.value, end=' ') for _ in lex if _.type != 'IGNORE']
+
 
 
     prettyIndent = 4
     # v converts leading tabs to space v
     leadingTabs = REcompile(r"""(?<=\n)\t+(?![\w\s]*('|"){3})""")
     while REsearch(leadingTabs, data):
         match = REsearch(leadingTabs, data)
@@ -1491,14 +1495,15 @@
         optStrFormatToFString=True
         optCompilerEval=True # pyfuzz indicates there is likely breaking behaviour
         optPow=True
         optDeadVariableElimination=True
         optNestedLoopItertoolsProduct=True
         optSplitMultiAssign=True
         optUnModAssignment=True
+        optCompressPrint=True
         # v these are done in main phase v
         optIfTrue=True # hybrid
         optSortedToSort=True
         optListPlusListToExtend=True
         optLoopToMap=True
         optFuncCache=True
 
@@ -1586,15 +1591,118 @@
                                     if metaCall.split('=')[-1].lower() == 'true':
                                         optimize = True
                                     elif metaCall.split('=')[-1].lower() == 'false':
                                         optimize = True
                                 else:
                                     optimize = not optimize
                     #if debug: print('!',blah,token,lex[token])
-                    if lex[token].type == 'ID':
+                    if optCompressPrint and lex[token].type in {'ID','FUNCTION'} and lex[token].value.startswith('print'):
+                        # combines current print with the print on the prior line, to reduce function calls
+                        # TODO handle defexp (when its print)
+                        # also fstrings (done when prior is, not current)
+                        tmpFound = False ; tmp2ndEndWith=tmpEndWith='\\n'
+                        tmpf=[] # the print's args
+                        if lex[token].type == 'ID' and lex[token+1].type == 'LPAREN':
+                              tmpStart=2
+                        else: tmpStart=1
+                        #for tmpi in range(token+tmpStart,len(lex)):
+                        #    if lex[tmpi].type in typeNewline: break
+                        #    else: tmpf.append(copy(lex[tmpi]))
+                        safe = False
+                        if lex[token+tmpStart].type == 'MINUS' and lex[token+tmpStart+1].type == 'NUMBER':
+                            tmpStart+=1
+                            lex[token+tmpStart-1].type='IGNORE'
+                            lex[token+tmpStart].value = '-'+lex[token+tmpStart].value
+                        if lex[token+tmpStart].type in {'STRING','NUMBER'}:
+                            tmpf = copy(lex[token+tmpStart])
+                            if lex[token+tmpStart+1].type in ('RPAREN',)+typeNewline: safe=True
+                            elif token+tmpStart+4 < len(lex)-1 and lex[token+tmpStart+1].type == 'COMMA' and lex[token+tmpStart+2].type == 'ID' and lex[token+tmpStart+2].value == 'end' \
+                            and lex[token+tmpStart+3].type == 'ASSIGN' and lex[token+tmpStart+4].type == 'STRING':
+                                safe=True ; tmp2ndEndWith=lex[token+tmpStart+4].value
+                            if lex[token+tmpStart].type == 'STRING' and lex[token+tmpStart].value[0] not in {'"',"'"}: safe=False
+                        if safe:
+                            # check backwards for print
+                            safe = False ; tmpPrintIndent=tmpCurrentIndent=None ; tmpFound=-1
+                            for tmpi in range(token-1, 0, -1):
+                                if lex[tmpi].type in typeNewline:
+                                    if lex[tmpi].type == 'NEWLINE':
+                                        tmpCurrentIndent = 0
+                                        if tmpPrintIndent == None: tmpPrintIndent=tmpCurrentIndent
+                                    elif lex[tmpi].type == 'TAB':
+                                        tmpCurrentIndent = lex[tmpi].value.count(' ')
+                                        if tmpPrintIndent == None: tmpPrintIndent=tmpCurrentIndent
+                                    if tmpCurrentIndent != tmpPrintIndent: break
+                                elif lex[tmpi].type in {'ID','FUNCTION'} and lex[tmpi].value.startswith('print') and lex[tmpi-1].type in typeNewline:
+                                    for tmpii in range(tmpi + 1, len(lex)):
+                                        if lex[tmpii].type in typeNewline: break
+                                        elif lex[tmpii].type in {'FSTR','STRING','NUMBER'} and lex[tmpii-1].type != 'ASSIGN' \
+                                        and ((lex[tmpii+1].type in typeNewline or (lex[tmpii+1].type == 'RPAREN' and lex[tmpii+2].type in typeNewline)) \
+                                        or (lex[tmpii+1].type == 'COMMA' and lex[tmpii+2].type == 'ID' and lex[tmpii+2].value == 'end' and lex[tmpii+3].type == 'ASSIGN')):
+                                            safe=True ; tmpFound=tmpii
+                                        elif lex[tmpii].type in {'FSTR','STRING'} and lex[tmpii-1].type == 'ASSIGN' and lex[tmpii-2].type == 'ID' and lex[tmpii-2].value == 'end' and lex[tmpii-3].type == 'COMMA':
+                                            tmpEndWith=lex[tmpii].value
+                                            if tmpEndWith.endswith("'''") or tmpEndWith.endswith('"""'):
+                                                tmpEndWith = tmpEndWith[3:-3]
+                                            else:
+                                                tmpEndWith = tmpEndWith[1:-1]
+                                    break
+                        if tmpFound and tmpf and (lex[tmpFound].value.endswith("'''") or lex[tmpFound].value.endswith('"""'))\
+                        and (tmpf.value.endswith("'''") or tmpf.value.endswith('"""')):
+                            safe=False # TODO: COULD be safe, I just don't feel like handling it rn
+                        if safe:
+                            # delete self
+                            for tmpi in range(token, len(lex)):
+                                if lex[tmpi].type in typeNewline: break
+                                else: lex[tmpi].type='IGNORE'
+                            # cull quotes
+                            tmpQuoteType=False
+                            if tmpf.type == 'STRING':
+                                if tmpf.value.endswith("'''") or tmpf.value.endswith('"""'):
+                                      tmpQuoteType = tmpf.value[-1]*3
+                                      tmpf.value = tmpf.value[3:-3]
+                                else: tmpf.value = tmpf.value[1:-1]
+                            # add to other print
+                            tmpStrType = ''
+                            if lex[tmpFound].type in {'FSTR','STRING'}:
+                                if lex[tmpFound].value.endswith("'''") or lex[tmpFound].value.endswith('"""'):
+                                    tmp=1
+                                    for _ in lex[tmpFound].value:
+                                        if _ in {'"',"'"}:
+                                            tmpQuoteType = _
+                                            break
+                                        tmp+=1 ; tmpStrType+=_
+                                    tmpFoundCutAmount=(tmp,3)
+                                elif lex[tmpFound].type == 'FSTR':
+                                    tmpFoundCutAmount = (0, 1) ; tmpQuoteType=lex[tmpFound].value[-1]
+                                else:
+                                    if not tmpQuoteType: tmpQuoteType="'" if lex[tmpFound].value[-1] == "'" else '"'
+                                    tmp=1
+                                    for _ in lex[tmpFound].value:
+                                        if _ in {'"', "'"}:
+                                            break
+                                        tmp += 1; tmpStrType += _
+                                    tmpFoundCutAmount = (tmp, 1)
+                                if lex[tmpFound].type == 'STRING':
+                                    lex[tmpFound].value=f"{tmpStrType}{tmpQuoteType}{lex[tmpFound].value[tmpFoundCutAmount[0]:-tmpFoundCutAmount[1]]}{tmpEndWith}{tmpf.value}{tmpQuoteType*tmpFoundCutAmount[1]}"
+                                else:
+                                    lex[tmpFound].value = f"{tmpStrType}{lex[tmpFound].value[tmpFoundCutAmount[0]:-tmpFoundCutAmount[1]]}{tmpEndWith}{tmpf.value}{tmpQuoteType * tmpFoundCutAmount[1]}"
+                            elif lex[tmpFound].type == 'NUMBER':
+                                if not tmpQuoteType: tmpQuoteType="'"
+                                lex[tmpFound].value = f"{tmpStrType}{tmpQuoteType}{lex[tmpFound].value}{tmpEndWith}{tmpf.value}{tmpQuoteType}"
+                                lex[tmpFound].type = 'STRING'
+                            if lex[tmpFound+1].type == 'COMMA' and lex[tmpFound+2].type == 'ID' and lex[tmpFound+2].value == 'end' \
+                            and lex[tmpFound+3].type == 'ASSIGN' and lex[tmpFound+4].type == 'STRING':
+                                if tmp2ndEndWith == '\\n':
+                                    lex[tmpFound+1].type=lex[tmpFound+2].type=lex[tmpFound+3].type=lex[tmpFound+4].type='IGNORE'
+                                else:
+                                    lex[tmpFound+4].value=tmp2ndEndWith
+                            newOptimization=True
+                            if debug: print(f'! combined print: {lex[tmpFound].value}')
+
+                    elif lex[token].type == 'ID':
                         if optConstantPropagation:
                             tmpi=None
                             if lex[token-1].type not in typeConditionals+('OR','AND','LOOP'):
                                 if lex[token+1].type in typeAssignables+('FSTR',) and lex[token+1].type != 'LISTEND' and lex[token+2].type not in {'PIPE','LISTCOMP'}:
                                     tmpi=1
                                 elif lex[token+1].type == 'ASSIGN' and lex[token+1].value.strip() in {'is','='} and lex[token+2].type in typeAssignables+('LPAREN','LBRACKET','FUNCTION','MINUS','INS','LINDEX','FSTR') and lex[token+2].type != 'LISTEND' and lex[token+3].type != 'LISTCOMP':
                                     tmpi=2
@@ -1697,14 +1805,16 @@
                                         tmpf=tmpf[::-1]
                                         if len(tmpf) > 1 and tmpf[-1].type!='LIST' and any(True for i in tmpf if i.type == 'LISTCOMP' )==False:
                                             tmptok=copy(lex[token]) ; tmptok.type='LPAREN' ; tmptok.value='(' ; tmpf.append(tmptok) ; del tmptok
                                             tmptok=copy(lex[token]) ; tmptok.type='RPAREN' ; tmptok.value=')' ; tmpf.insert(0,tmptok) ; del tmptok
                                         tmpListOfVarsInside=tuple([_.value for _ in tmpf if _.type == 'ID']) # for keeping track of vars inside that may change
                                     else: tmpf=[l for l in tmpf if tmpf.type != 'IGNORE']
 
+                                    linkType = True if (enforceTyping or compileTo == 'Cython') else False
+
                                     tmpindent = 0  # keeping track if constant is in indented block
                                     tmpFoundIndent = tmpFoundThen = tmpInTypeWrap = tmpCheckForDef = False
                                     # tmpCheckForDef when not False, checks to see if inside function before canceling optimization
                                     tmptmpIndent = 0  # keeping track of backwards current indent
                                     for tmpi in range(token - 1, 0, -1):
                                         # checks backwards to make sure its valid, also gets indent
                                         if lex[tmpi].type == 'TAB':
@@ -1731,33 +1841,35 @@
                                             tmpFoundThen = True
                                         elif lex[tmpi].type == 'TYPEWRAP':
                                             tmpInTypeWrap = True
                                         elif tmpindent > tmptmpIndent and lex[tmpi].type == 'ID' and lex[tmpi].value == lex[token].value:
                                             tmpCheckForDef = True  # previous version of self found on previous indent, bail!
                                         elif tmpCheckForDef and lex[tmpi].type in {'PYDEF', 'DEFFUNCT'}:
                                             tmpCheckForDef = False
+                                        elif lex[tmpi].type == 'PYCLASS':
+                                            linkType=False
                                         #print(lex[token].value, lex[tmpi].type, tmptmpIndent, tmpindent)
 
                                     def handleIgnoreOnNL():
                                         nonlocal tmpAddToIgnoresWhenNL, ignores, tmpi
                                         if tmpAddToIgnoresWhenNL > 0:
                                             ignores.append(tmpAddToIgnoresWhenNL)
                                             tmpAddToIgnoresWhenNL = 0
                                         elif tmpAddToIgnoresWhenNL < 0:
                                             # when tmpAddToIgnoresWhenNL is negative, use postive version as start and current tmpi as end
                                             ignores.append((-tmpAddToIgnoresWhenNL,tmpi))
                                             tmpAddToIgnoresWhenNL = 0
 
-                                    search=True ; linkType=True if (enforceTyping or compileTo == 'Cython') else False ; ignores=[] ; inDef=wasInDefs=inFrom=inCase=tmpInConditionalStatement=False
+                                    search=True ; ignores=[] ; inDef=wasInDefs=inFrom=inCase=tmpInConditionalStatement=False
                                     # wasInDefs is for determining if a later define could break behaviour inside of functions
                                     # inDef i think is for determining if its the name of a function??
                                     tmpIDshow=0 ; tmpAddToIgnoresWhenNL = 0
                                     #print('-----')
                                     for tmpi in range(valueStop+1,len(lex)): # check if we can determine its a constant
-                                        #print(lex[token].value,search,lex[tmpi].type,lex[tmpi].value,tmpIDshow)
+                                        #print(lex[token].value,search,lex[tmpi].type,lex[tmpi].value,ignores,tmpAddToIgnoresWhenNL,tmpi,tmpIDshow)
                                         if not search and (enforceTyping and not linkType): break
                                         if lex[tmpi].type=='INC' or (tmpi+1 < len(lex) and lex[tmpi+1].type=='LINDEX' and lex[tmpi].value in (lex[token].value,)+tmpListOfVarsInside) \
                                         or ((lex[tmpi].type in {'ID','INC'} and lex[tmpi].value.replace('++','').replace('--','') in (lex[token].value,)+tmpListOfVarsInside and (lex[tmpi-1].type not in {'ELIF','OF','IF','OR','AND','FSTR'})  ) and lex[tmpi+1].type in typeAssignables+('ASSIGN',) ):
                                             if (lex[tmpi+1].type == 'ASSIGN' and lex[tmpi+2].type == vartype) or lex[tmpi+1].type == vartype or (vartype=='NUMBER' and lex[tmpi].type=='INC'):
                                                 pass
                                             elif lex[tmpi+1].type == 'ASSIGN' and vartype == 'STRING' and lex[tmpi+1].value.strip() not in {'=','is',':='}: pass # if fold is string then only hard assigns arent safe
                                             else: linkType=False
@@ -1782,15 +1894,15 @@
                                                     else:
                                                         # set ignore point at end of line, so that it may still fold onto expression
                                                         for ii in range(tmpi,len(lex)-1):
                                                             if lex[ii].type in typeNewline:
                                                                 tmpAddToIgnoresWhenNL = ii
                                                                 break
 
-                                            if not wasInDefs and lex[tmpi+1].type in typeAssignables+('ASSIGN',):
+                                            if not wasInDefs and lex[tmpi+1].type in typeAssignables+('ASSIGN',) and not tmpAddToIgnoresWhenNL:
                                                 # wasInDefs used to not have the `not`, I think saying "if we are not in (another) function" makes sense.
                                                 # but because the prior intent is not clear, just be aware of this as a suspect if something breaks later.
                                                 tmpSafe=False
                                                 if lex[tmpi+1].type == 'ASSIGN' and 'is' in lex[tmpi+1].value and determineIfAssignOrEqual(tmpi+1):
                                                     tmpSafe=True ; tmpAddToIgnoresWhenNL=0
                                                 if not tmpSafe:
                                                     tmpAddToIgnoresWhenNL = tmpi
@@ -1935,15 +2047,15 @@
                                                     elif (isinstance(ignores[0], list) or isinstance(ignores[0], tuple)) and tmpi == ignores[0][0]:
                                                         ignore=True
                                                     if ignore and tmpi == ignores[0][1]:
                                                         ignore=False ; del ignores[0]
                                                     #if debug: print(tmpi,lex[tmpi].type,f'ignore={ignore}',f'skip/end={ignores}')
 
                                                 if search and ignore == False:
-                                                    #print(lex[token].value,lex[tmpi].type,lex[tmpi].value,search,linkType,ignores,tmpi, tmpLastIndent,tmpindent)
+                                                    #print('~',lex[token].value,lex[tmpi].type,lex[tmpi].value,search,linkType,ignores,tmpi, tmpLastIndent,tmpindent)
                                                     if lex[tmpi].type == 'ID' and lex[tmpi].value==lex[token].value and (lex[tmpi+1].type not in typeAssignables+('ASSIGN',) or (lex[tmpi-1].type in typeConditionals+('OR','AND','INS') and lex[tmpi-1].type!='ELSE') or (lex[tmpi+1].type == 'ASSIGN' and 'is' in lex[tmpi+1].value and determineIfAssignOrEqual(tmpi+1)) or (lex[tmpi+1].type == 'LIST' and lex[tmpi-1].type not in typeNewline+('TYPE','CONSTANT','ELSE')+typeAssignables)) and lex[tmpi-1].type not in {'FOR','LOOP'}:
                                                         if lex[tmpi-1].type in typeConditionals and lex[tmpi+1].type == 'ASSIGN' and ':' in lex[tmpi+1].value: continue
                                                         tmpsafe=True
                                                         if lex[tmpi-1].type in {'RBRACKET','RPAREN','LISTEND'} or lex[tmpi-2].type == 'COMMA':
                                                             for tmpii in range(tmpi,0,-1):
                                                                 if lex[tmpii].type == 'LOOP': tmpsafe=False ; break
                                                                 elif lex[tmpii].type in typeNewline: break
@@ -1982,15 +2094,15 @@
                                                             # so on instances where we know it doesn't break behaviour, we make a
                                                             # DEFEXP token to signify it is safe.
                                                             tmpStartOfline=0 ; tmpDefExp=True
                                                             for tt in range(tmpi,0,-1):
                                                                 if lex[tt].type in typeNewline: tmpStartOfline=tt ; break
                                                             for tt in range(tmpStartOfline+1,len(lex)-1):
                                                                 if lex[tt].type in typeNewline: break
-                                                                elif lex[tt].type == 'DEFEXP': tmpDefExp=tmpsafe=False ; break
+                                                                elif lex[tt].type == 'DEFEXP': tmpDefExp=False ; break
                                                                 elif lex[tt].type == 'ID' and lex[tt+1].type in typeAssignables: tmpDefExp=False
                                                                 elif lex[tt].type not in typePrintable: tmpDefExp=False
                                                             if tmpDefExp and tmpsafe:
                                                                 lex.insert(tmpStartOfline+1,makeToken(lex[0],'defExp','DEFEXP'))
                                                                 tmpi+=1
 
                                                         if tmpsafe and not isinstance(tmpf[0],str) and len([True for _ in tmpf if _.type == 'DICT']) > 0:
@@ -2939,30 +3051,49 @@
                                 if tmpType == 'list':
                                     lex[token].type='LIST' ; lex[token].value='['
                                     lex[token+1].type='LISTEND' ; lex[token+1].value=']'
                                 else:
                                     lex[token].type = 'LBRACKET' ; lex[token].value = '{'
                                     lex[token + 1].type = 'RBRACKET' ; lex[token + 1].value = '}'
 
-
-                            if optFuncTricksDict['roundFast'] and lex[token].value == 'round(' and lex[token+1].type in {'ID','NUMBER'} and lex[token+2].type == 'COMMA' and lex[token+3].type == 'NUMBER' and lex[token+4].type == 'RPAREN':
+                            if optFuncTricksDict['roundFast'] and (lex[token].value in {'round','round(','ASround(','ASround'} and lex[token+1].type in {'ID','NUMBER'} and lex[token+2].type == 'COMMA' and lex[token+3].type == 'NUMBER' and lex[token+4].type == 'RPAREN') \
+                            or (lex[token].value in {'round','round(','ASround(','ASround'} and lex[token+1].type == 'LPAREN'  and lex[token+2].type in {'ID','NUMBER'} and lex[token+3].type == 'COMMA' and lex[token+4].type == 'NUMBER' and lex[token+5].type == 'RPAREN'):
                                 # fast rounding, majorly accurate
                                 # forumula: int(some_float * (10 ** TOLERANCE) - (.5 if some_float < 0 else -.5)) / (10 ** TOLERANCE)
-                                lex[token+1].type=lex[token+2].type=lex[token+3].type='IGNORE'
+
+                                if lex[token+1].type == 'LPAREN':
+                                      tmpAdjust=1 ; lex[token+4].type='IGNORE'
+                                else: tmpAdjust=0
+
+
                                 if optLoopAttr and preAllocated and 'ASint' in (p[1] for p in preAllocated): lex[token].value='ASint('
                                 elif compileTo == 'Cython': lex[token].value = '<int>('
                                 else: lex[token].value='int('
-                                tmpFloat = lex[token+1].value
-                                tmpTolerance = 10**int(lex[token+3].value)
-                                tmp=f"{tmpFloat} * ({tmpTolerance}) - (.5 if {tmpFloat} < 0 else -.5)) / ({tmpTolerance}"
+                                if optCompilerEval and lex[token+1+tmpAdjust].type == 'NUMBER' == lex[token+3+tmpAdjust].type:
+                                    try: int(lex[token+3+tmpAdjust].value)
+                                    except ValueError:
+                                        tmpE=lex[token+3+tmpAdjust].value
+                                        return AS_SyntaxError(
+                                            f'You are rounding to {tmpE} instead of a integer.',
+                                            f'round({lex[token+1+tmpAdjust].value}, {tmpE.split(".")[0]})',
+                                            lex[token].lineno, data, 'Function Argument Error:')
+                                    tmpTolerance=lex[token+3+tmpAdjust].value ; tmpFloat = lex[token+1+tmpAdjust].value
+                                    tmp=f"{round(float(lex[token+1+tmpAdjust].value),int(lex[token+3+tmpAdjust].value))}"
+                                    lex[token].type = 'LPAREN' ; lex[token].value = '('
+                                else:
+                                    tmpFloat = lex[token+1+tmpAdjust].value
+                                    tmpTolerance = 10**int(lex[token+3+tmpAdjust].value)
+                                    tmp=f"{tmpFloat} * ({tmpTolerance}) - (.5 if {tmpFloat} < 0 else -.5)) / ({tmpTolerance}"
                                 if debug: print(f'! fast-round: round({tmpFloat},{tmpTolerance})  -->  {tmp}')
+                                lex[token + 1].type = lex[token + 2].type = lex[token + 3].type = 'IGNORE'
                                 autoMakeTokens(tmp, token)
                                 newOptimization=True
                                 lex.insert(token,makeToken(lex[token],'DONTDEXP','DONTDEXP'))
 
+
                             if optFuncTricksDict['insertMathConstants'] and lex[token].type == 'BUILTINF' and \
                             (  ((lex[token].value == 'pi' or lex[token].value == 'math.pi') and 'math.' in wasImported and 'pi' in wasImported['math.'])
                             or ((lex[token].value == 'e'  or lex[token].value == 'math.e' ) and 'math.' in wasImported and 'e'  in wasImported['math.'])
                                 ):
                                 # math.pi --> 3.141592653589793
                                 tmp='3.141592653589793' if lex[token].value.endswith('pi') else '2.718281828459045' # pi or e
                                 if debug: print(f'! insertMathConstants: {lex[token].value} --> {tmp}')
@@ -3464,15 +3595,19 @@
                                     tmp=tmpf[0][0].value
                                     if tmp.startswith('"""') or tmp.startswith("'''"):
                                         tmp=tmp[3:-3]
                                     else:
                                         tmp=tmp[1:-1]
                                     lex[token].value=lex[token].value.replace('%s',tmp,1)
                                 elif len(tmpf[0]) == 1 and tmpf[0][0].type == 'NUMBER':
+                                    if debug: tmp = lex[token].value
                                     lex[token].value=lex[token].value.replace('%s',tmpf[0][0].value,1)
+                                    if '{' not in lex[token].value and '}' not in lex[token].value: lex[token].value=lex[token].value[1:]
+                                    if debug: print('! converted to fstring:', tmp, '-->', lex[token].value)
+                                    newOptimization = True
                                 else:
                                     if debug: tmp = lex[token].value
                                     lex[token].value=lex[token].value.replace('%s','{%s}'%''.join([l.value+' ' for l in tmpf[0]]),1)
                                     if debug: print('! converted to fstring:',tmp,'-->',lex[token].value)
                                     newOptimization=True ; safe = True
                                 tmpf.pop(0)
                             if tmpf and '{' not in lex[token].value and '}' not in lex[token].value:
@@ -3675,19 +3810,30 @@
                         del lex[token] ; token-=2
                     if optCompilerEval and lex[token].type in {'STRING','NUMBER'}: # jumpy
                         # math or string evaluation
                         bitwiseOrderOps = {'~': 5, '<<': 4, '>>': 4, '&': 3, '^': 2, '|': 1}
                         tmpTypeSafe = typeNewline + ('RPAREN', 'ASSIGN', 'FUNCTION', 'LPAREN', 'ELSE', 'DEFEXP', 'LINDEX')
                         check=False
                         # these blocks help follow the order of operations for more accuracy
-                        if token+3 < len(lex)-1 and ((lex[token+3].type == 'PIPE' and lex[token+3].value == 'to') or lex[token+1].type in typeNewline or lex[token+2].type in typeNewline): pass
+                        if                                        (token+3 < len(lex)-1 and lex[token + 3].type == 'RPAREN' and lex[token - 3].type in {'LPAREN','FUNCTION'} and lex[token - 2].type == lex[token + 2].type == 'NUMBER' and lex[token - 1].type in orderOfOps and  lex[token + 1].type in orderOfOps and orderOfOps[lex[token - 1].type] == orderOfOps[lex[token + 1].type]) \
+                        or (isANegativeNumberTokens(token - 1) and token+4 < len(lex)-1 and lex[token + 3].type == 'RPAREN' and lex[token - 4].type in {'LPAREN','FUNCTION'} and lex[token - 3].type == lex[token + 2].type == 'NUMBER' and lex[token - 2].type in orderOfOps and  lex[token + 1].type in orderOfOps and orderOfOps[lex[token - 2].type] == orderOfOps[lex[token + 1].type]):
+                            # if order of ops is equal, preference goes towards left
+                            #print('#0',lex[token].value)
+                            if isANegativeNumberTokens(token - 1) and lex[token-4].type in {'LPAREN',}:
+                                lex.insert(token + 1, makeToken(lex[token], ')', 'RPAREN'))
+                                lex.insert(token - 4, makeToken(lex[token], '(', 'LPAREN'))
+                            else:
+                                lex.insert(token + 1, makeToken(lex[token], ')', 'RPAREN'))
+                                lex.insert(token - 3, makeToken(lex[token], '(', 'LPAREN'))
+                            newOptimization=True # needs another iteration
+                        elif token+3 < len(lex)-1 and ((lex[token+3].type == 'PIPE' and lex[token+3].value == 'to') or lex[token+1].type in typeNewline or lex[token+2].type in typeNewline): pass
                         elif lex[token-1].type in orderOfOps and lex[token+1].type in orderOfOps and not (lex[token-1].type == 'MINUS' and lex[token-2].type in tuple(orderOfOps)+tmpTypeSafe):
                             #print('#-1', lex[token].value)
                             if (lex[token-1].type in {'LPAREN','FUNCTION'} or (orderOfOps[lex[token-1].type] < orderOfOps[lex[token+1].type]) or (lex[token-1].type=='MINUS' and lex[token-2].type in orderOfOps and (lex[token-2].type=='LPAREN' or orderOfOps[lex[token-2].type] < orderOfOps[lex[token+1].type])) ) \
-                            and ((lex[token+3].type in typeNewline+('RPAREN',) or (isANegativeNumberTokens(token+2) and lex[token+4].type in typeNewline+('RPAREN',))) or not ((lex[token+3].type in orderOfOps and (orderOfOps[lex[token+3].type] >= orderOfOps[lex[token+1].type])) or (isANegativeNumberTokens(token+2) and lex[token+4].type in orderOfOps and orderOfOps[lex[token+4].type] >= orderOfOps[lex[token+1].type]))) \
+                            and token+4 < len(lex)-1 and ((lex[token+3].type in typeNewline+('RPAREN',) or (isANegativeNumberTokens(token+2) and lex[token+4].type in typeNewline+('RPAREN',))) or not ((lex[token+3].type in orderOfOps and (orderOfOps[lex[token+3].type] >= orderOfOps[lex[token+1].type])) or (isANegativeNumberTokens(token+2) and lex[token+4].type in orderOfOps and orderOfOps[lex[token+4].type] >= orderOfOps[lex[token+1].type]))) \
                             and not (token+3 < len(lex) and lex[token+1].type == 'EXPONENT' and lex[token+3].type == 'EXPONENT') and not (token+4 < len(lex) and lex[token+1].type == 'EXPONENT' and isANegativeNumberTokens(token+2) and lex[token+4].type == 'EXPONENT'):
                                 # 'normal'
                                 #print('#1', lex[token].value)
                                 tmppre=-1
                                 if lex[token-1].type == 'MINUS' and lex[token-2].type in orderOfOps and lex[token-2].type != 'LPAREN':
                                     tmppre = -2
                                 if lex[tmppre].type in orderOfOps:
@@ -3706,19 +3852,20 @@
                                         if isANegativeNumberTokens(token+2) and lex[token+4].type in orderOfOps and orderOfOps[lex[token+1].type] >= orderOfOps[lex[token+4].type]:
                                             check = True
                                         elif lex[token+3].type in orderOfOps and orderOfOps[lex[token+1].type] >= orderOfOps[lex[token+3].type]:
                                             check = True
                                         else:
                                             check = True
                                         #print('#1.2', lex[token].value)
+                                    
                                 else:
                                     check=True
                                     #print('#1.3',lex[token].value)
                             elif (lex[token].type == 'STRING' and ((lex[token+1].type == 'TIMES' and lex[token+2].type == 'NUMBER') or (lex[token+1].type == 'PLUS' and lex[token+2].type == 'STRING' and lex[token-1].type != 'TIMES'))) \
-                            or ((lex[token-1].type in {'LPAREN','FUNCTION'} or orderOfOps[lex[token-1].type] <= 2) and lex[token].type == 'NUMBER' and lex[token+1].type == 'TIMES' and lex[token+2].type == 'STRING'):
+                            or ((lex[token-1].type in {'LPAREN','FUNCTION'} or (lex[token-1].type in orderOfOps and orderOfOps[lex[token-1].type] <= 2)) and lex[token].type == 'NUMBER' and lex[token+1].type == 'TIMES' and lex[token+2].type == 'STRING'):
                                 # simple string eval
                                 #print("1.4", lex[token].value)
                                 check=True
                         elif (lex[token-1].type in tmpTypeSafe or (lex[token-1].type=='MINUS' and lex[token-2].type in tmpTypeSafe)) and lex[token+1].type in orderOfOps:
                             # when last token isnt operator, checks ahead and also handles bitwise
                             #print('#2', lex[token].value)
                             if isANegativeNumberTokens(token+2) and lex[token+4].type in orderOfOps:
@@ -3755,22 +3902,23 @@
                             check = False
                         if check and lex[token-1].type == 'BITWISE' and lex[token+1].type == 'BITWISE':
                             if bitwiseOrderOps[lex[token-1].value] > bitwiseOrderOps[lex[token+1].value]:
                                 check=False
 
                         if check:
                             if lex[token].type == 'NUMBER' and lex[token+1].type in typeOperators and (lex[token+2].type == 'NUMBER' or (lex[token+2].type == 'LPAREN' and lex[token+3].type == 'NUMBER') or isANegativeNumberTokens(token+2)):
-
                                 tmpf=[] ; tmpscope=0 ; tmpLastOperator=fail=False
                                 for tmpi in range(token,len(lex)-1):
                                     if lex[tmpi].type in typeOperators+('NUMBER','LPAREN','RPAREN'):
                                         if   lex[tmpi].type == 'LPAREN': tmpscope-=1 ; tmpLastOperator=False
                                         elif lex[tmpi].type == 'RPAREN': tmpscope+=1 ; tmpLastOperator=False
                                         elif lex[tmpi].type in typeOperators:
-                                            if tmpLastOperator and orderOfOps[lex[tmpi].type] >= orderOfOps[tmpLastOperator]:
+                                            if tmpLastOperator and lex[tmpi].type == 'MINUS' and lex[tmpi+1].type == 'NUMBER':
+                                                tmpf.append(lex[tmpi]) ; continue
+                                            elif tmpLastOperator and orderOfOps[lex[tmpi].type] >= orderOfOps[tmpLastOperator]:
                                                 break
                                             else:
                                                 tmpLastOperator = lex[tmpi].type
                                         tmpf.append(lex[tmpi])
                                     else:
                                         if tmpf[-1].type in typeOperators: del tmpf[-1]
                                         break
@@ -3852,24 +4000,25 @@
                                 lex[token].value = 'True'
                             else:
                                 lex[token].value = 'False'
                             lex[token].type = 'BOOL'
                             lex[token+1].type = 'IGNORE'
                             newOptimization = True
                     if optCompilerEval \
-                    and ((lex[token-1].type == 'LPAREN' and lex[token+1].type == 'RPAREN' and lex[token-2].type in ('LPAREN','ASSIGN','DEFEXP')+typeNewline+typeOperators and lex[token].type != 'FUNCTION') \
-                    or (lex[token-1].type == 'MINUS' and lex[token-2].type == 'LPAREN' and lex[token+1].type == 'RPAREN' and lex[token-3].type in ('LPAREN','ASSIGN','DEFEXP')+typeNewline+typeOperators and lex[token].type != 'FUNCTION')):
+                    and ((lex[token-1].type == 'LPAREN' and lex[token+1].type == 'RPAREN' and (lex[token-2].type in ('LPAREN','ASSIGN','DEFEXP')+typeNewline+typeOperators or (lex[token-2].type == 'FUNCTION' and lex[token-2].value[-1] == '(')) and lex[token].type != 'FUNCTION') \
+                    or (lex[token-1].type == 'MINUS' and lex[token-2].type == 'LPAREN' and lex[token+1].type == 'RPAREN' and (lex[token-3].type in ('LPAREN','ASSIGN','DEFEXP')+typeNewline+typeOperators or (lex[token-3].type == 'FUNCTION' and lex[token-3].value[-1] == '(')) and lex[token].type != 'FUNCTION')):
+                        # remove useless paren like:  (-12)
                         #print(lex[token-2].type,lex[token-1].type,lex[token].type,lex[token].value,lex[token+1].type,888888888888)
                         if lex[token-1].type == 'MINUS':
                             lex[token-2].type='IGNORE'
                         else:
                             lex[token-1].type='IGNORE'
                         lex[token+1].type='IGNORE'
+                        del lex[token+1]
                         token-=2
-
                     token+=1
 
         # last optimizations, run at the end (until no more optimization)
         newOptimization = True ; optRounds=0
         while newOptimization:
             if debug: print(f'\t- end optimization round = {optRounds} -')
             newOptimization = False
@@ -4266,30 +4415,30 @@
         # in function form so print without parenthesis can use it, and print.
         # currently for singular values only
         nonlocal storedVarsHistory, line
         check=False # for checking if printf needs to be imported
         tmpval=tok.value ; tmptype=tok.type
         if tok.value in storedVarsHistory and 'staticType' in storedVarsHistory[tok.value]:
             if storedVarsHistory[tok.value]['staticType'] == 'int':
-                line.append(f'{" "*(indent)}printf("%d\\n",{tmpval})\n')
+                line.append(f'{" "*(indent)}printf("%llu\\n",{tmpval})\n')
                 check=True
             else: line.append(f'{" "*(indent)}print({tmpval})')
         elif tmptype in {'STRING','STRLIT','STRRAW'}:
             if any(i for i in ('r','f') if i == tmpval[0]):
                 line.append(f'{" "*(indent)}printf({tmpval}.encode())\n')
                 line.append(f'{" "*(indent)}printf("\\n")')
             elif tmpval.startswith("'''") or tmpval.startswith('"""'):
                 tmpval=list(tmpval) ; tmpval.insert(-3,'\n')
                 tmpval=''.join(tmpval)
                 line.append(f'{" "*(indent)}printf({tmpval})\n')
             else: line.append(f'{" "*(indent)}printf("{tmpval[1:-1]}\\n")\n')
             check=True
         elif tmptype == 'NUMBER':
             if '.' in tmpval: line.append(f'{" "*(indent)}printf("%.14f",{tmpval})\n')
-            else: line.append(f'{" "*(indent)}printf("%d\\n",{tmpval})\n')
+            else: line.append(f'{" "*(indent)}printf("%llu\\n",{tmpval})\n')
             check=True
         else:
             if tmpval in storedCustomFunctions:
                 line.append(f'{" " * (indent)}print({tmpval}())')
             else:
                 line.append(f'{" "*(indent)}print({tmpval})')
 
@@ -7037,15 +7186,17 @@
                 elif tmpf in metaIgnoreIndent:
                     ignoreIndentation = metaHandling(tok.value, ignoreIndentation)
                 elif tmpf in metaPyFunc:
                     functionPassing = metaHandling(tok.value, functionPassing)
                 elif tmpf in metaPyIs:
                     pyIs = metaHandling(tok.value, pyIs)
                 elif tmpf in metaPyCompat:
-                    pyIs=True ; functionPassing=True ; expPrint.append('') ; autoEnumerate=False ; intVsStrDoLen=False
+                    pyCompatibility = metaHandling(metaCall, pyCompatibility)
+                    if pyCompatibility:
+                        pyIs=True ; functionPassing=True ; expPrint.append('') ; autoEnumerate=False ; intVsStrDoLen=False
                 elif tmpf in {'asnake','Asnake','ASnake'}:
                     pyIs=False ; functionPassing=False
                 elif tmpf in {'Cython','cython'}:
                     compileTo='Cython'
                 elif tmpf in {'Python','python'}:
                     compileTo='Python'
                 elif tmpf in inlineReplace:
```

### Comparing `asnake-0.13.38/src/ASnake/__main__.py` & `asnake-0.13.39/src/ASnake/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,18 @@
 
 
 if __name__ == '__main__':
     from argparse import ArgumentParser, FileType, ArgumentError
     from sys import stdin
     from os import rename, chdir, listdir
     def makeParser(error=False):
-        argParser=ArgumentParser(exit_on_error=error)
+        try:
+            argParser=ArgumentParser(exit_on_error=error)
+        except TypeError:
+            argParser = ArgumentParser()
         argParser.add_argument('-r', '--run', action='store_true', help="Compiles file in memory then runs it.")
         argParser.add_argument('-e', '--eval', action='store', help="Compiles ASnake in a string to Python and runs it.")
         argParser.add_argument('-v', '--version', action='store', help="Specify which Python version to compile to.")
         argParser.add_argument('-c', '--compile', action='store_true', help="Compiles file to .py and writes it on disk. On Cython will attempt to compile to .so file.")
         argParser.add_argument('-o', '--optimize', action='store_true', help="Toggles optimization on and off. On by default.")
         argParser.add_argument('-fm', '--format', action='store_true', help="Turns off code formatting if on, and turns it off if on.")
         argParser.add_argument('-f', '--fast', action='store_true', help="Turns off code formatting, and turns off optimization. Useful for fast compile times.")
@@ -130,22 +133,25 @@
             tmpHandle='' ; tmpArgs = ' '.join(argv[1:])
             if '.asnake' in tmpArgs: tmpHandle='asnake'
             elif '.py'   in tmpArgs: tmpHandle='py'
             if tmpHandle:
                 print('File not found. Perhaps try one of these files:')
                 print('\t'+('\n\t'.join([_ for _ in listdir() if _.endswith('.'+tmpHandle)])),end='')
                 print()
-            makeParser(True).parse_args()
+            from platform import python_version
+            tmpPyVer=python_version().split('.')
+            if tmpPyVer[0] == '3' and int(tmpPyVer[1]) >= 9: # exit_on_error added to argparse in 3.9
+                makeParser(True).parse_args()
         else:
             print(e)
         exit()
 
     data: str = ''
     if not stdin.isatty():
-        data = sys.stdin.read()
+        data = stdin.read()
         ASFile = False
     elif args.file == None or not path.isfile(args.file.name):
         if args.eval:
             data = args.eval
             ASFile = False
             runCode = True
         elif args.asnake_script:
```

### Comparing `asnake-0.13.38/src/ASnake/data/megaTest.asnake` & `asnake-0.13.39/src/ASnake/data/megaTest.asnake`

 * *Files identical despite different names*

### Comparing `asnake-0.13.38/src/ASnake/data/setAlias.asnake` & `asnake-0.13.39/src/ASnake/data/setAlias.asnake`

 * *Files identical despite different names*

### Comparing `asnake-0.13.38/src/ASnake.egg-info/PKG-INFO` & `asnake-0.13.39/src/ASnake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ASnake
-Version: 0.13.38
+Version: 0.13.39
 Summary: Python optimizing compiler for the ASnake programming language.
 Author: Ahri Fox
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

