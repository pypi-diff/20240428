# Comparing `tmp/peter_explains-0.0.10.tar.gz` & `tmp/peter-explains-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peter_explains-0.0.10.tar", last modified: Sun Apr 28 17:12:17 2024, max compression
+gzip compressed data, was "peter-explains-0.0.9.tar", last modified: Sun Mar 17 09:05:09 2024, max compression
```

## Comparing `peter_explains-0.0.10.tar` & `peter-explains-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:12:17.273509 peter_explains-0.0.10/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-28 17:12:13.000000 peter_explains-0.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-28 17:12:17.273509 peter_explains-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-28 17:12:13.000000 peter_explains-0.0.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:12:17.269509 peter_explains-0.0.10/peter_explains/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 17:12:13.000000 peter_explains-0.0.10/peter_explains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-28 17:12:13.000000 peter_explains-0.0.10/peter_explains/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-28 17:12:13.000000 peter_explains-0.0.10/peter_explains/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-28 17:12:13.000000 peter_explains-0.0.10/peter_explains/peter_ai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-04-28 17:12:13.000000 peter_explains-0.0.10/peter_explains/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 17:12:17.273509 peter_explains-0.0.10/peter_explains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-28 17:12:17.000000 peter_explains-0.0.10/peter_explains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-28 17:12:17.000000 peter_explains-0.0.10/peter_explains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 17:12:17.000000 peter_explains-0.0.10/peter_explains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-28 17:12:17.000000 peter_explains-0.0.10/peter_explains.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-28 17:12:17.000000 peter_explains-0.0.10/peter_explains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 17:12:17.000000 peter_explains-0.0.10/peter_explains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 17:12:17.273509 peter_explains-0.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-28 17:12:13.000000 peter_explains-0.0.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:09.224147 peter-explains-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-17 09:05:04.000000 peter-explains-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-17 09:05:09.224147 peter-explains-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-17 09:05:04.000000 peter-explains-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:09.224147 peter-explains-0.0.9/peter_explains/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/peter_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-03-17 09:05:04.000000 peter-explains-0.0.9/peter_explains/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 09:05:09.224147 peter-explains-0.0.9/peter_explains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-17 09:05:09.000000 peter-explains-0.0.9/peter_explains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 09:05:09.224147 peter-explains-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-17 09:05:04.000000 peter-explains-0.0.9/setup.py
```

### Comparing `peter_explains-0.0.10/LICENSE` & `peter-explains-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `peter_explains-0.0.10/PKG-INFO` & `peter-explains-0.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: peter-explains
-Version: 0.0.10
-Summary: Linux command explanations from Peter Griffin
-Home-page: https://github.com/atick-faisal/peter-explains
-Author: Atick Faisal
-Author-email: atickfaisal@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: diskcache
-Requires-Dist: json_repair
-Requires-Dist: google-generativeai
-
 ## **`peter`: Your Linux Command Translator (Peter Griffin Edition)**
 
-![Banner](docs/assets/banner.png)
+![Banner](https://github.com/atick-faisal/peter-explains/blob/823cc63c9950a2f1e38b9aebdda8837d88e18d4c/docs/assets/banner.png)
 
 Hey Lois, ever wanted to understand those geeky Linux commands but were afraid you'd end up more confused than a monkey trying to do its taxes? Well, fear no more! `peter` is here to break down those brainy terminal things in a way even I can understand (well, mostly).
 
-![Demo](docs/assets/demo.gif)
+![Demo](https://github.com/atick-faisal/peter-explains/blob/823cc63c9950a2f1e38b9aebdda8837d88e18d4c/docs/assets/demo.gif)
 
 ### **How the Heck Does This Work?**
 
-1. **You type somethin' like:** `peter ls` or `peter "grep hello world.txt"`
+1. **You type somethin' like:** `peter ls`
 2. **I whip out my trusty Gemini AI translator:** This thing's smarter than Stewie after a bowl of spinach, and it'll turn that boring 'ls' command into a hilarious hot mess of an explanation.
 3. **You laugh (or groan), but hey, at least you learn somethin':** Maybe you'll actually remember what those commands do instead of just blindly copying stuff from the internet like a parrot.
 
 ### **Gettin' Started (For Dummies Like Me)** <img src="https://github.com/atick-faisal/peter-explains/blob/823cc63c9950a2f1e38b9aebdda8837d88e18d4c/docs/assets/apikey.png" alt="Whatever" width="250" align="right">
 
 1. **Make sure you got that pip thing installed:** You know, for downloading packages and stuff. If you don't, Lois help you.
 2. **Use pip to install this amazingness:** `pip install peter-explains`
@@ -50,15 +35,15 @@
 
     $ peter --help
 
 Need more?
 
 <p align="center">
     <a href="http://atick.dev/peter-explains/">
-    <img src="docs/assets/docs.png" alt="Button description" width="400">
+    <img src="https://github.com/atick-faisal/peter-explains/blob/823cc63c9950a2f1e38b9aebdda8837d88e18d4c/docs/assets/docs.png" alt="Button description" width="400">
     </a>
 </p>
 
 ### **For the Brainiacs (a.k.a. Potential Contributors)**
 
 Hey Meg, turns out even _I_ can't make this thing perfect on my own. If you're the type who knows their way around Python and AI, feel free to poke around the code and make it even funnier (or, dare I say, _educational_).
```

#### html2text {}

```diff
@@ -1,36 +1,32 @@
-Metadata-Version: 2.1 Name: peter-explains Version: 0.0.10 Summary: Linux
-command explanations from Peter Griffin Home-page: https://github.com/atick-
-faisal/peter-explains Author: Atick Faisal Author-email: atickfaisal@gmail.com
-License: MIT Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: colorama Requires-Dist: diskcache Requires-Dist: json_repair
-Requires-Dist: google-generativeai ## **`peter`: Your Linux Command Translator
-(Peter Griffin Edition)** ![Banner](docs/assets/banner.png) Hey Lois, ever
+## **`peter`: Your Linux Command Translator (Peter Griffin Edition)** ![Banner]
+(https://github.com/atick-faisal/peter-explains/blob/
+823cc63c9950a2f1e38b9aebdda8837d88e18d4c/docs/assets/banner.png) Hey Lois, ever
 wanted to understand those geeky Linux commands but were afraid you'd end up
 more confused than a monkey trying to do its taxes? Well, fear no more! `peter`
 is here to break down those brainy terminal things in a way even I can
-understand (well, mostly). ![Demo](docs/assets/demo.gif) ### **How the Heck
-Does This Work?** 1. **You type somethin' like:** `peter ls` or `peter "grep
-hello world.txt"` 2. **I whip out my trusty Gemini AI translator:** This
-thing's smarter than Stewie after a bowl of spinach, and it'll turn that boring
-'ls' command into a hilarious hot mess of an explanation. 3. **You laugh (or
-groan), but hey, at least you learn somethin':** Maybe you'll actually remember
-what those commands do instead of just blindly copying stuff from the internet
-like a parrot. ### **Gettin' Started (For Dummies Like Me)** [Whatever]1.
-**Make sure you got that pip thing installed:** You know, for downloading
-packages and stuff. If you don't, Lois help you. 2. **Use pip to install this
-amazingness:** `pip install peter-explains` 3. **Boom! Unleash the Peter:** Try
-something like `peter grep`. Just don't ask me to explain it â that's the
-AI's job. ### Retep is gonna ruin your day if you try to use without the API
-KEY Don't worry. Meg's here to help. You need a FREE Google Gemini API KEY. -
-Get yours from here: [https://aistudio.google.com/app/](https://
-aistudio.google.com/app/) - Add the `API KEY` your Environment by running the
-following: $ export GOOGLE_API_KEY=YOUR_KEY - (Recommended) Add this line to
-your `.bashrc` or `.zshrc` ### Help Run the following for help $ peter --help
-Need more?
+understand (well, mostly). ![Demo](https://github.com/atick-faisal/peter-
+explains/blob/823cc63c9950a2f1e38b9aebdda8837d88e18d4c/docs/assets/demo.gif)
+### **How the Heck Does This Work?** 1. **You type somethin' like:** `peter ls`
+2. **I whip out my trusty Gemini AI translator:** This thing's smarter than
+Stewie after a bowl of spinach, and it'll turn that boring 'ls' command into a
+hilarious hot mess of an explanation. 3. **You laugh (or groan), but hey, at
+least you learn somethin':** Maybe you'll actually remember what those commands
+do instead of just blindly copying stuff from the internet like a parrot. ###
+**Gettin' Started (For Dummies Like Me)** [Whatever]1. **Make sure you got that
+pip thing installed:** You know, for downloading packages and stuff. If you
+don't, Lois help you. 2. **Use pip to install this amazingness:** `pip install
+peter-explains` 3. **Boom! Unleash the Peter:** Try something like `peter
+grep`. Just don't ask me to explain it â that's the AI's job. ### Retep is
+gonna ruin your day if you try to use without the API KEY Don't worry. Meg's
+here to help. You need a FREE Google Gemini API KEY. - Get yours from here:
+[https://aistudio.google.com/app/](https://aistudio.google.com/app/) - Add the
+`API KEY` your Environment by running the following: $ export
+GOOGLE_API_KEY=YOUR_KEY - (Recommended) Add this line to your `.bashrc` or
+`.zshrc` ### Help Run the following for help $ peter --help Need more?
                              _[_B_u_t_t_o_n_ _d_e_s_c_r_i_p_t_i_o_n_]
 ### **For the Brainiacs (a.k.a. Potential Contributors)** Hey Meg, turns out
 even _I_ can't make this thing perfect on my own. If you're the type who knows
 their way around Python and AI, feel free to poke around the code and make it
 even funnier (or, dare I say, _educational_). ### **Disclaimer** [Whatever]I
 ain't responsible if this tool makes you dumber, offends your delicate
 sensibilities, or causes your computer to explode. Use at your own risk, and
```

### Comparing `peter_explains-0.0.10/peter_explains/main.py` & `peter-explains-0.0.9/peter_explains/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,36 @@
 import asyncio
-from diskcache import Cache
 from .peter_ai import explain_command
 from .utils import (
     parse_arguments,
     stylize_output,
     show_loading_message,
     show_error_message,
-    get_cache_dir,
 )
 
-cache = Cache(get_cache_dir("peter_explains"))
-
 
 async def main():
     """
     Main function to run the Peter Explains CLI.
 
     This function is an async function that runs the main Peter Explains CLI.
     It uses the asyncio library to run the main Peter Explains CLI.
     """
     try:
         command = parse_arguments()
+        tasks = [
+            asyncio.create_task(show_loading_message()),
+            asyncio.create_task(explain_command(command)),
+        ]
+        done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
 
-        result = None
-
-        if command in cache:  # Check in cache
-            result = cache[command]
-
-        else:
-            tasks = [
-                asyncio.create_task(show_loading_message()),
-                asyncio.create_task(explain_command(command)),
-            ]
-            done, pending = await asyncio.wait(
-                tasks, return_when=asyncio.FIRST_COMPLETED
-            )
-
-            pending.pop().cancel()  # Cancel the loading message task
-            result = done.pop().result()  # Get the result of the explain_command task
-
-            cache[command] = result  # Save in cache
-
+        pending.pop().cancel()  # Cancel the loading message task
+        result = done.pop().result()  # Get the result of the explain_command task
         stylize_output(result)
-
-    except Exception:
+    except Exception as _:
         show_error_message()
 
 
 def peter():
     """
     Function to run the Peter Explains CLI.
```

### Comparing `peter_explains-0.0.10/peter_explains/utils.py` & `peter-explains-0.0.9/peter_explains/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import os
 import sys
+import json
 import random
 import asyncio
 import argparse
-import json_repair
 from colorama import Fore, Style
 from ._version import __version__
 
 
 loading_messages = [
     "Hang on, Lois, I'm tryin' to think here. This is harder than figuring out what's goin' on in Stewie's head.",
     "Jeez, this computer's slower than Quagmire after a night at The Clam.",
@@ -26,42 +25,14 @@
     "Alright, this might take longer than I thought. You got any beer in the fridge?",
     "Ugh, somethin' ain't right. Maybe I shoulda paid more attention to that computer class in high school.",
     "Aw jeez, I think I broke it. Don't tell Lois, she'll make me fix it.",
     "I swear, this thing's got more bugs than the Griffin house. And that's sayin' somethin'.",
 ]
 
 
-def get_cache_dir(app_name):
-    """
-    This function gets the cache directory for the Peter Explains CLI based on the operating system.
-
-    Args:
-    - app_name (str): The name of the Peter Explains CLI.
-
-    Returns:
-    - cache_dir (str): The cache directory for the Peter Explains CLI.
-    """
-    if os.name == "nt":  # Windows
-        cache_dir = os.path.join(os.getenv("LOCALAPPDATA"), app_name, "cache")
-    elif os.name == "posix":
-        home = os.path.expanduser("~")
-        if sys.platform == "darwin":  # macOS
-            cache_dir = os.path.join(
-                home, "Library", "Application Support", app_name, "cache"
-            )
-        else:  # Linux and other UNIX like
-            cache_dir = os.path.join(home, ".config", app_name, "cache")
-    else:
-        cache_dir = app_name
-
-    os.makedirs(cache_dir, exist_ok=True)
-
-    return cache_dir
-
-
 def forgot_api_key():
     """
     Function to display a message when the API key is missing.
     """
     print(
         Fore.RED
         + "Aw, c'mon! Where's the freakin' API key? You think this thing works by magic?"
@@ -92,57 +63,42 @@
     Stylize the output of the Peter Explains CLI.
 
     This function takes the output of the Peter Explains CLI and stylizes it for display in the terminal.
 
     Args:
     - output (str): The output of the Peter Explains CLI.
     """
-    data = json_repair.loads(output)
+    data = json.loads(output)
 
     # Headers
-    print(
-        Fore.CYAN
-        + "\nCommand:"
-        + Style.RESET_ALL
-        + Style.BRIGHT
-        + f" {data['command_name']}"
-        + Style.RESET_ALL
-        + "\n"
-    )
-    print(Fore.YELLOW + "Purpose:\n" + Style.RESET_ALL + f"{data['purpose']}")
+    print(Fore.CYAN + "\nCommand:" + Style.RESET_ALL + f" {data['command_name']}\n")
+    print(Fore.YELLOW + "Purpose:" + Style.RESET_ALL + f" {data['purpose']}\n")
 
     # Syntax
-    if "syntax" in data:  # Scenario 1: Full command explanation
-        print(Fore.YELLOW + "\nSyntax:" + Style.RESET_ALL)
-        # Colorama doesn't have built-in syntax highlighting, keep plain text here
-        print(data["syntax"] + Style.RESET_ALL + "\n")
-
-        # Options
-        print(Fore.YELLOW + "Options:" + Style.RESET_ALL)
-        for option in data["options"]:
-            print(Fore.BLUE + f"* {option}" + Style.RESET_ALL)
-
-        # Examples
-        print(Fore.YELLOW + "\nExamples:" + Style.RESET_ALL)
-        for example in data["examples"]:
-            print(Fore.GREEN + "* " + example + Style.RESET_ALL)
-
-    elif "breakdown" in data:  # Scenario 2: Command with arguments breakdown
-        print(Fore.YELLOW + "\nBreakdown:" + Style.RESET_ALL)
-        for explanation in data["breakdown"]:
-            print(Fore.GREEN + f"* {explanation}" + Style.RESET_ALL)
+    print(Fore.YELLOW + "Syntax:" + Style.RESET_ALL)
+    print(Fore.LIGHTBLACK_EX + data["syntax"] + Style.RESET_ALL + "\n")  # Dimmed syntax
+
+    # Options
+    print(Fore.YELLOW + "Options:" + Style.RESET_ALL)
+    for option, description in data["options"].items():
+        print(f"* {option}: {description}")
+
+    # Examples
+    print(Fore.YELLOW + "\nExamples:" + Style.RESET_ALL)
+    for example in data["examples"]:
+        print(Fore.GREEN + "* " + example + Style.RESET_ALL)
 
 
 async def show_loading_message():
     """
     Show a loading message while the Peter Explains CLI is running.
 
     This function uses the asyncio library to show a loading message while the Peter Explains CLI is running.
     """
-    for _ in range(10):
+    for _ in range(5):
         await asyncio.sleep(3.0)
         print(loading_messages[random.randint(0, len(loading_messages) - 1)])
 
     print("Peter's takin' too long. He's probably watchin' TV or somethin'.")
     sys.exit(0)
 
 
@@ -157,66 +113,65 @@
 
 def display_peter_help():
     """
     Display the help message for the Peter Explains CLI.
 
     This function displays the help message for the Peter Explains CLI.
     """
-    print(Fore.CYAN + "\nPeter Explains Linux (kinda)" + Style.RESET_ALL)
+    print(Fore.CYAN + "\nPeter Explains Linux (Kinda)" + Style.RESET_ALL)
     print(
         Fore.LIGHTBLACK_EX
         + "Hey numbnuts, looks like you need help figurin' out this thing. Here's the deal:\n"
         + Style.RESET_ALL
     )
 
     print(Fore.YELLOW + "How to Use This Pile of Junk:" + Style.RESET_ALL)
     print(
-        "* Type 'peter' and then the name of that Linux thing you need explanation for. Like, 'peter ls' or whatever."
+        "* Get an Explanation: Type 'peter' and then the name of that Linux thing you can't remember. Like, 'peter ls' or whatever.  I'll try my best to explain it in a way even you might understand."
     )
     print(
-        "* Feeling Stupid? Saw a fancy Linux command and don't know what it does? Type it inside \" \" like 'peter \"grep hello world.txt\"' \n"
+        "* Feeling Stupid? Get More Options:  If my explanation ain't enough (and let's be real, it probably won't be), try 'peter ls --options' for even more boring details.\n"
     )
 
     print(Fore.YELLOW + "Other Useless Crap:" + Style.RESET_ALL)
     print("* --help:  Yeah, yeah, that's what you're lookin' at right now, genius.")
     print(
         "* --version:  Who cares what version this is?  It probably ain't gonna work right anyway.\n"
     )
 
 
 def parse_arguments() -> str:
     """
-    This function parses arguments for the Peter Explains CLI.
+    This function parses arguments fot the Peter Explains CLI.
     """
     parser = argparse.ArgumentParser(
         description="Linux commands explained the Peter Griffin way. Seriously.",
         add_help=False,
     )
     parser.add_argument(
         "--version", action="version", version=f"Peter Explains (peter) v{__version__}"
     )
     parser.add_argument(
         "-h",
         "--help",
         action="store_true",
-        help="Display the help message",
     )
 
     parser.add_argument(
-        "explain_this", nargs="?", help="Explanation of the required argument"
+        "required_argument", nargs="?", help="Explanation of the required argument"
     )
 
     args = parser.parse_args()
 
     if args.help:
         display_peter_help()
         sys.exit(0)
 
     # Handle missing required argument
-    if not args.explain_this:
+    if not args.required_argument:
         display_peter_help()
         sys.exit(0)
 
     # TODO: Add more argument validation here
 
     else:
-        return args.explain_this.strip().lower()
+        return args.required_argument.strip().lower()
```

### Comparing `peter_explains-0.0.10/setup.py` & `peter-explains-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 setup(
     name="peter-explains",
     version=_version.__version__,
     description="Linux command explanations from Peter Griffin",
     author="Atick Faisal",
     author_email="atickfaisal@gmail.com",
     packages=find_packages(),
-    install_requires=["colorama", "diskcache", "json_repair", "google-generativeai"],
+    install_requires=["colorama", "google-generativeai"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "peter = peter_explains.main:peter",
         ],
     },
```
