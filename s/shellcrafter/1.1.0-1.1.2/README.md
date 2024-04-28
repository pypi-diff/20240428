# Comparing `tmp/shellcrafter-1.1.0.tar.gz` & `tmp/shellcrafter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcrafter-1.1.0.tar", last modified: Sun Apr 14 01:52:25 2024, max compression
+gzip compressed data, was "shellcrafter-1.1.2.tar", last modified: Sun Apr 28 12:33:39 2024, max compression
```

## Comparing `shellcrafter-1.1.0.tar` & `shellcrafter-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 01:52:25.260633 shellcrafter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-14 01:52:25.260633 shellcrafter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 01:52:25.260633 shellcrafter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 01:52:25.256633 shellcrafter-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 01:52:25.260633 shellcrafter-1.1.0/src/shellcrafter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/src/shellcrafter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/src/shellcrafter/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/src/shellcrafter/find_gadgets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5588 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/src/shellcrafter/keyst_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9652 2024-04-14 01:52:14.000000 shellcrafter-1.1.0/src/shellcrafter/shellcode_procedure_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 01:52:25.260633 shellcrafter-1.1.0/src/shellcrafter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-14 01:52:25.000000 shellcrafter-1.1.0/src/shellcrafter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-14 01:52:25.000000 shellcrafter-1.1.0/src/shellcrafter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 01:52:25.000000 shellcrafter-1.1.0/src/shellcrafter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 01:52:25.000000 shellcrafter-1.1.0/src/shellcrafter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 01:52:25.000000 shellcrafter-1.1.0/src/shellcrafter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 01:52:25.000000 shellcrafter-1.1.0/src/shellcrafter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.181477 shellcrafter-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 12:33:39.181477 shellcrafter-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/src/shellcrafter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13367 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/find_gadgets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11174 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/keyst_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/peutils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10063 2024-04-28 12:33:23.000000 shellcrafter-1.1.2/src/shellcrafter/shellcode_procedure_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 12:33:39.177477 shellcrafter-1.1.2/src/shellcrafter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 12:33:39.000000 shellcrafter-1.1.2/src/shellcrafter.egg-info/top_level.txt
```

### Comparing `shellcrafter-1.1.0/PKG-INFO` & `shellcrafter-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.0
+Version: 1.1.2
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: keystone-engine
 Requires-Dist: termcolor
 Requires-Dist: rich
 Requires-Dist: ropper
 Requires-Dist: capstone
 Requires-Dist: typer
+Requires-Dist: pefile
 
 # Shellcrafter
 
 Shellcrafter is a comprehensive toolkit designed for shellcode development and gadget finding. It integrates several utilities to assist in the generation of shellcode from assembly instructions, conversion of ASCII text to hexadecimal stack push instructions, loading of DLLs, finding ROP gadgets, and more.
 
 ## Installation
```

### Comparing `shellcrafter-1.1.0/README.md` & `shellcrafter-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.0/setup.py` & `shellcrafter-1.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-version = "1.1.0"
+version = "1.1.2"
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 REPO_URL = 'https://github.com/totekuh/shellcrafter'
@@ -29,14 +29,15 @@
     install_requires=[
         "numpy",  # Depending on your CLI, some of these may no longer be necessary
         "keystone-engine",
         "termcolor",
         "rich",
         "ropper",
         "capstone",
-        "typer",  # Added Typer to the list of required packages
+        "typer",
+        "pefile"
     ],
     project_urls={  # Optional
         'Bug Reports': f'{REPO_URL}/issues',
         'Source': REPO_URL,
     },
 )
```

### Comparing `shellcrafter-1.1.0/src/shellcrafter/cli.py` & `shellcrafter-1.1.2/src/shellcrafter/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 #!/usr/bin/env python3
 from pprint import pprint
 import os
 import sys
-from keystone import *
 from typer import Typer, Option, Exit, Argument, echo
 
 module_path = os.path.dirname(__file__)
 sys.path.append(module_path)
 
-from keyst_api import print_shellcode, run_shellcode, eprint
-from keyst_api import OUTPUT_FORMAT_PYTHON, X86_ARCH, X64_ARCH
+from keyst_api import ShellcodeCompiler, ShellcodeRunner, get_instructions, print_shellcode
+from keyst_api import OUTPUT_FORMAT_PYTHON, X86_ARCH
 from shellcode_procedure_generator import str_to_hex_little_endian_push, \
     data_types, \
     print_hash_algorithm, \
     compute_hash, \
     generate_load_library, \
     write_to_memory
 from find_gadgets import do_find_gadgets
+from peutils import *
 
 app = Typer(help="Shellcrafter: A tool for shellcode development and gadget finding.", add_completion=False)
 
 shellcode_app = Typer(add_completion=False)
 app.add_typer(shellcode_app, name="shellcode", help="Shellcode-related operations.")
 
 codegen_app = Typer(help="Code generation utilities.")
 app.add_typer(codegen_app, name="codegen")
 
 gadgets_app = Typer(help="Searches for clean, categorized gadgets from a given list of files.")
 app.add_typer(gadgets_app, name="gadgets")
 
-DEFAULT_VAR_NAME = "shellcode"
+# Creating a sub-command group for iat operations
+pe_app = Typer(help="PE related operations")
 
+# Adding the iat sub-command group to the main app
+app.add_typer(pe_app, name="pe")
 
-def read_instructions_from_file(filepath: str) -> str:
-    if os.path.exists(filepath):
-        with open(filepath, 'r', encoding='utf-8', errors='ignore') as f:
-            return f.read()
-    else:
-        print(f"The given file {filepath} doesn't exist")
-        raise Exit(code=1)
+DEFAULT_VAR_NAME = "shellcode"
 
 
 @codegen_app.command(help="Displays a list of common data types used in Windows programming with their descriptions.")
 def print_data_types():
     """
     This command prints a detailed list of data types with their corresponding type, size, and a brief description.
     It is useful for developers needing quick reference to these types during Windows API programming or similar tasks.
@@ -77,15 +74,14 @@
 
 
 @codegen_app.command("write", help="Writes a string to a specific memory address, "
                                    "formatting it in hexadecimal and optionally avoiding NULL bytes.")
 def write(ascii_string: str = ascii_option,
           write_addr: str = write_addr_option,
           null_free: bool = null_free_option):
-    print(f"push_str:  ;# push the '{ascii_string}' onto the stack")
     write_to_memory(s=ascii_string, write_addr=write_addr, null_free=null_free)
 
 
 @codegen_app.command("push-ascii", help="Converts an ASCII string to hexadecimal "
                                         "in little-endian for stack pushing.")
 def push_for_ascii(
         ascii_string: str = ascii_option,
@@ -153,68 +149,75 @@
                     arch=arch,
                     output=output,
                     color=color,
                     skip_rp=skip_rp)
 
 
 @shellcode_app.command("compile",
-                       help="Compiles assembly instructions into executable shellcode, "
-                            "with options to execute or print it.")
-def compile_shellcode(instructions: str = Option(None, "--instructions", "-i",
-                                                 help="Assembly instructions to generate the shellcode"),
-                      instructions_file: str = Option(None, "--instructions-file", "-if",
-                                                      help="File with assembly instructions to generate the shellcode"),
-                      run: bool = Option(False, "--run", "-r", help="Execute the shellcode after compiling"),
-                      var_name: str = Option(DEFAULT_VAR_NAME, "--var-name", "-vn",
-                                             help="Variable name for the shellcode"),
+                       help="Compiles assembly instructions into executable shellcode.")
+def compile_shellcode(instructions: str = Option(None, "--instructions", "-i"),
+                      instructions_file: str = Option(None, "--instructions-file", "-if"),
+                      var_name: str = Option(DEFAULT_VAR_NAME, "--var-name", "-vn"),
                       interval: int = Option(48, "--interval",
-                                             help="Number of opcodes per line while printing the shellcode", min=0,
-                                             max=192),
-                      interactive: bool = Option(False, "--interactive", is_flag=True,
-                                                 help="Wait for user input before executing the shellcode"),
-                      output_format: str = Option(OUTPUT_FORMAT_PYTHON, "--output-format",
-                                                  help="Output format of the shellcode: 'python', 'c-array', or 'bin'."),
-                      arch: str = Option(X86_ARCH, "--arch",
-                                         help=f"Architecture for the assembly: '{X64_ARCH}' or '{X86_ARCH}'.")):
-    """
-    Compiles assembly instructions into shellcode and optionally executes it.
-    """
-    if instructions and instructions_file:
-        echo("Either the --instructions-file or --instructions option must be given, not both.", err=True)
-        raise Exit(code=1)
-    if not instructions and not instructions_file:
-        echo("Either the --instructions-file or --instructions option must be given.", err=True)
-        raise Exit(code=1)
-
-    if instructions_file:
-        instructions = read_instructions_from_file(instructions_file)
-
-    # Determine the architecture and mode for the Keystone engine
-    if arch == X86_ARCH:
-        ks_arch = KS_ARCH_X86
-        ks_mode = KS_MODE_32
-    elif arch == X64_ARCH:
-        ks_arch = KS_ARCH_X86
-        ks_mode = KS_MODE_64
-    else:
-        eprint(f"Unsupported architecture: {arch}")
-        sys.exit(1)
-
-    ks = Ks(ks_arch, ks_mode)
-
-    try:
-        shellcode_assembled, count = ks.asm(instructions)
-        eprint(f"[+] {count} instructions have been encoded")
-    except KsError as ks_error:
-        eprint(f"Shellcode compilation failed: {ks_error}", err=True)
-        raise Exit(code=1)
-
-    if run:
-        run_shellcode(encoding=shellcode_assembled,
-                      interactive=interactive,
-                      arch=arch)
-    else:
-        print_shellcode(shellcode_assembled, var_name=var_name, interval=interval, output_format=output_format)
+                                             help="Number of opcodes per line while printing the shellcode"),
+                      output_format: str = Option(OUTPUT_FORMAT_PYTHON, "--output-format"),
+                      arch: str = Option(X86_ARCH, "--arch")):
+    shellcode_compiler = ShellcodeCompiler(arch=arch)
+    shellcode_assembled, count = shellcode_compiler.assemble_instructions(
+        instructions=get_instructions(instructions, instructions_file))
+    print_shellcode(shellcode_assembled, var_name=var_name, interval=interval, output_format=output_format)
+
+
+@shellcode_app.command("run", help="Executes the compiled shellcode on the detected platform.")
+def run_shellcode_command(instructions: str = Option(None, "--instructions", "-i"),
+                          instructions_file: str = Option(None, "--instructions-file", "-if"),
+                          interactive: bool = Option(False, "--interactive"),
+                          arch: str = Option(X86_ARCH, "--arch")):
+    shellcode_runner = ShellcodeRunner(arch=arch)
+    shellcode_compiler = ShellcodeCompiler(arch=arch)
+
+    shellcode_assembled, count = shellcode_compiler.assemble_instructions(
+        instructions=get_instructions(instructions, instructions_file))
+
+    shellcode_runner.run_shellcode(shellcode_assembled, interactive=interactive)
+
+
+@pe_app.command(name="rva-offset-find", help="Convert RVA to file offset in a PE file.")
+def find_rva_offset_(file: str,
+                     rva: str = typer.Argument(...,
+                                               help='RVA to convert. Supports "0x" prefix for hexadecimal values.'),
+                     section_name: Optional[str] = typer.Option(None, "--section-name", "-sn",
+                                                                help='Optional. The name of the section to search through for the given --rva offset.')):
+    find_rva_offset(file=file, rva=rva, section_name=section_name)
+
+
+@pe_app.command(name="iat-print", help="Print the Import Address Table (IAT), "
+                                       "optionally filtering by DLL name and/or function name.")
+def iat_print_(file: str,
+               dll: Optional[str] = typer.Option(None, help="Filter by DLL name, case-insensitive."),
+               function: Optional[str] = typer.Option(None, help="Filter by function name, case-insensitive.")):
+    iat_print(file=file, dll=dll, function=function)
+
+
+@pe_app.command(name="bytes-display", help="Display bytes from a file starting at a specified offset.")
+def display_bytes_(file: str = typer.Argument(..., help="The path to the binary file."),
+                          offset: str = typer.Option(..., help="Offset in the file to start reading bytes."),
+                          length: int = typer.Option(..., help="Number of bytes to read and display.")):
+    display_bytes(file=file, offset=offset, length=length)
+
+@pe_app.command(name="bytes-search", help="Search for a sequence of bytes in a file.")
+def bytes_search(file: str = typer.Argument(..., help="The path to the binary file."),
+                 byte_sequence: str = typer.Option(..., help="Byte sequence to search for, e.g., '\\x41\\x42\\x43'")):
+    search_bytes(file=file, byte_sequence=byte_sequence)
+
+
+@pe_app.command(name="eat-print", help="Parse the Export Address Table (EAT) and print it.")
+def eat_print_(file: str):
+    parse_eat(file=file)
+
+@pe_app.command(name="sections-print", help="Print details of each section in the PE file.")
+def print_sections_(file: str = typer.Argument(..., help="The path to the PE file.")):
+    print_sections(file=file)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `shellcrafter-1.1.0/src/shellcrafter/find_gadgets.py` & `shellcrafter-1.1.2/src/shellcrafter/find_gadgets.py`

 * *Files identical despite different names*

### Comparing `shellcrafter-1.1.0/src/shellcrafter/shellcode_procedure_generator.py` & `shellcrafter-1.1.2/src/shellcrafter/shellcode_procedure_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,142 +3,169 @@
 import os
 import sys
 
 module_path = os.path.dirname(__file__)
 sys.path.append(module_path)
 import numpy
 
+LPCSTR = "LPCSTR"
+LPVOID = "LPVOID"
+LPBOOL = "LPBOOL"
+DWORD = "DWORD"
+LPPROGRESS_ROUTINE = "LPPROGRESS_ROUTINE"
+BOOL = "BOOL"
+BYTE = "BYTE"
+WORD = "WORD"
+LONG = "LONG"
+WCHAR = "WCHAR"
+LPWSTR = "LPWSTR"
+HANDLE = "HANDLE"
+HWND = "HWND"
+HINSTANCE = "HINSTANCE"
+UINT = "UINT"
+SHORT = "SHORT"
+FLOAT = "FLOAT"
+DOUBLE = "DOUBLE"
+LPDWORD = "LPDWORD"
+LPLONG = "LPLONG"
+HDC = "HDC"
+HBITMAP = "HBITMAP"
+HBRUSH = "HBRUSH"
+HCURSOR = "HCURSOR"
+HICON = "HICON"
+HMENU = "HMENU"
+
 # Define data types
 data_types = {
-    "LPCSTR": {
+    LPCSTR: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Long Pointer to a Constant String. Used for C-style null-terminated strings."
     },
-    "LPVOID": {
+    LPVOID: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Long Pointer to Void. Can point to any type of data."
     },
-    "LPBOOL": {
+    LPBOOL: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Long Pointer to BOOL. Used for passing boolean values by reference."
     },
-    "DWORD": {
+    DWORD: {
         "type": "integer",
         "size": 4,  # 32-bit integer size
         "description": "Double Word. A 32-bit unsigned integer."
     },
-    "LPPROGRESS_ROUTINE": {
+    LPPROGRESS_ROUTINE: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Long Pointer to PROGRESS_ROUTINE. Used for callback functions."
     },
-    "BOOL": {
+    BOOL: {
         "type": "integer",
         "size": 4,  # 32-bit integer size
         "description": "Boolean. Used for true/false values."
     },
-    "BYTE": {
+    BYTE: {
         "type": "integer",
         "size": 1,  # 8-bit integer size
         "description": "Byte. An 8-bit unsigned integer."
     },
-    "WORD": {
+    WORD: {
         "type": "integer",
         "size": 2,  # 16-bit integer size
         "description": "Word. A 16-bit unsigned integer."
     },
-    "LONG": {
+    LONG: {
         "type": "integer",
         "size": 4,  # 32-bit integer size
         "description": "Long. A 32-bit signed integer."
     },
-    "WCHAR": {
+    WCHAR: {
         "type": "integer",
         "size": 2,  # 16-bit integer size
         "description": "Wide Character. Used for Unicode characters."
     },
-    "LPWSTR": {
+    LPWSTR: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Long Pointer to a Wide String. Used for Unicode C-style null-terminated strings."
     },
-    "HANDLE": {
+    HANDLE: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle. Used as a reference to a system resource."
     },
-    "HWND": {
+    HWND: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to a Window. Used as a reference to a window object."
     },
-    "HINSTANCE": {
+    HINSTANCE: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to an Instance. Used as a reference to an application instance."
     },
-    "UINT": {
+    UINT: {
         "type": "integer",
         "size": 4,  # 32-bit integer size
         "description": "Unsigned Integer. A 32-bit unsigned integer."
     },
-    "SHORT": {
+    SHORT: {
         "type": "integer",
         "size": 2,  # 16-bit integer size
         "description": "Short. A 16-bit signed integer."
     },
-    "FLOAT": {
+    FLOAT: {
         "type": "float",
         "size": 4,  # 32-bit float size
         "description": "Float. A 32-bit floating point number."
     },
-    "DOUBLE": {
+    DOUBLE: {
         "type": "float",
         "size": 8,  # 64-bit double size
         "description": "Double. A 64-bit floating point number."
     },
-    "LPDWORD": {
+    LPDWORD: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Long Pointer to DWORD. Used for passing DWORD values by reference."
     },
-    "LPLONG": {
+    LPLONG: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Long Pointer to LONG. Used for passing LONG values by reference."
     },
-    "HDC": {
+    HDC: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to a Device Context. Used as a reference to a device context."
     },
-    "HBITMAP": {
+    HBITMAP: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to a Bitmap. Used as a reference to a bitmap object."
     },
-    "HBRUSH": {
+    HBRUSH: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to a Brush. Used as a reference to a brush object."
     },
-    "HCURSOR": {
+    HCURSOR: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to a Cursor. Used as a reference to a cursor object."
     },
-    "HICON": {
+    HICON: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to an Icon. Used as a reference to an icon object."
     },
-    "HMENU": {
+    HMENU: {
         "type": "pointer",
         "size": 4,  # 32-bit pointer size
         "description": "Handle to a Menu. Used as a reference to a menu object."
     }
 }
 
 def print_hash_algorithm():
```

### Comparing `shellcrafter-1.1.0/src/shellcrafter.egg-info/PKG-INFO` & `shellcrafter-1.1.2/src/shellcrafter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: shellcrafter
-Version: 1.1.0
+Version: 1.1.2
 Summary: A package containing scripts for developing and generating shellcode
 Home-page: https://github.com/totekuh/shellcrafter
 Author: totekuh
 Author-email: totekuh@protonmail.com
 Project-URL: Bug Reports, https://github.com/totekuh/shellcrafter/issues
 Project-URL: Source, https://github.com/totekuh/shellcrafter
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: keystone-engine
 Requires-Dist: termcolor
 Requires-Dist: rich
 Requires-Dist: ropper
 Requires-Dist: capstone
 Requires-Dist: typer
+Requires-Dist: pefile
 
 # Shellcrafter
 
 Shellcrafter is a comprehensive toolkit designed for shellcode development and gadget finding. It integrates several utilities to assist in the generation of shellcode from assembly instructions, conversion of ASCII text to hexadecimal stack push instructions, loading of DLLs, finding ROP gadgets, and more.
 
 ## Installation
```

