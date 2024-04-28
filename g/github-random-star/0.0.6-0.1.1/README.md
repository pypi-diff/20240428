# Comparing `tmp/github_random_star-0.0.6.tar.gz` & `tmp/github_random_star-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_random_star-0.0.6.tar", max compression
+gzip compressed data, was "github_random_star-0.1.1.tar", max compression
```

## Comparing `github_random_star-0.0.6.tar` & `github_random_star-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1060 2024-04-25 15:20:51.729971 github_random_star-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     3288 2024-04-25 15:20:51.729971 github_random_star-0.0.6/README.md
--rw-r--r--   0        0        0      250 2024-04-25 15:20:51.729971 github_random_star-0.0.6/github_random_star/__init__.py
--rw-r--r--   0        0        0     7690 2024-04-25 15:20:51.729971 github_random_star-0.0.6/github_random_star/__main__.py
--rw-r--r--   0        0        0     1500 2024-04-25 15:20:51.729971 github_random_star-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 github_random_star-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-28 12:20:26.236211 github_random_star-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     2676 2024-04-28 12:20:26.236211 github_random_star-0.1.1/README.md
+-rw-r--r--   0        0        0      253 2024-04-28 12:20:26.236211 github_random_star-0.1.1/github_random_star/__init__.py
+-rw-r--r--   0        0        0     5615 2024-04-28 12:20:26.236211 github_random_star-0.1.1/github_random_star/__main__.py
+-rw-r--r--   0        0        0     7509 2024-04-28 12:20:26.236211 github_random_star-0.1.1/github_random_star/api.py
+-rw-r--r--   0        0        0     1132 2024-04-28 12:20:26.236211 github_random_star-0.1.1/github_random_star/version.py
+-rw-r--r--   0        0        0     1607 2024-04-28 12:20:26.236211 github_random_star-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3863 1970-01-01 00:00:00.000000 github_random_star-0.1.1/PKG-INFO
```

### Comparing `github_random_star-0.0.6/LICENSE.md` & `github_random_star-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `github_random_star-0.0.6/README.md` & `github_random_star-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,74 +2,59 @@
 
 <a href="https://pypi.org/project/github-random-star"><img src="https://img.shields.io/pypi/v/github_random_star?style=for-the-badge&logo=pypi" /></a>
 <a href=""><img src="https://img.shields.io/github/actions/workflow/status/ddkasa/github-random-star/pypi-publish.yml?style=for-the-badge"/></a>
 <a href="https://pypi.org/project/github-random-star"><img src="https://img.shields.io/pypi/dm/github-random-star?style=for-the-badge" /></a>
 
 ![](docs/example_image.png?raw=true)
 
-If you have starred way too many GitHub repositories and need a way of keeping track of them. This simple CLI tool throws you quasi random starred repos to look at and explore.
+If you have starred way too many GitHub repositories and need a way of keeping track of them. This simple CLI tool throws you quasi random starred repos at you to look at and explore.
 
 ## Installation
 
 ### Preferred
 
 Install with [Pipx](https://github.com/pypa/pipx).
 
-`pipx install github-random-star`
+`$ pipx install github-random-star`
 
 ### Other
 
-Install from [PyPi](https://pypi.org/project/github-random-star)/[GitHub](https://github.com/ddkasa/github-random-star) with `pip` or clone this repository and install requirements through [Poetry](pyproject.toml) or the provided [requirements](requirements.txt) file.
-
-<details>
-    <summary>If using poetry.</summary>
-    <code>$ git clone https://github.com/ddkasa/github-random-star</code><br>
-    <code>$ cd github-random-star</code><br>
-    <code>$ poetry shell</code><br>
-    <code>$ poetry install</code>
-</details>
-<details>
-    <summary>If using requirements.txt.</summary>
-    <code>$ git clone https://github.com/ddkasa/github-random-star</code><br>
-    <code>$ cd github-random-star</code><br>
-    <code>$ virtualenv -p python3.12 .venv</code><br>
-    <code>$ source .venv/bin/activate</code><br>
-    <code>$ pip install -r requirements.txt</code>
-</details>
+Install from [PyPi](https://pypi.org/project/github-random-star)/[GitHub](https://github.com/ddkasa/github-random-star) with pip or clone this repository and install with pip/pipx locally.
 
 ## Usage
 
 1. Setup GitHub API token as the `GITHUB_ACCESS_TOKEN` environment variable. _If this is not setup it will use the public access point with lower rates._
-2. Run the script through `gh-star <flags>`, `python github_random_star/main.py <flags>` or if using Poetry `poetry run gh-star <flags>`
+2. Run the script through `$ gh-star <flags>`, `$ python github_random_star/main.py <flags>` or if using Poetry `$ poetry run gh-star <flags>`
 
 ### Flags
 
 - `-a, --account` Username of the GitHub account to retrieve the starred items from. `--account` is required or `GH_STAR_ACCOUNT` environment variable needs to be set.
 - `-t, --total` Total amount of random items you want to pick from. Defaults to 3.
 - `-r, --refresh` Whether to fetch new cached data or not. Will re fetch all starred items instead of using cache.
 - `--max-history` The amount of historic choices to cache. Defaults to 100. Set to **-1** to keep history unlimited. `GH_STAR_MAX_HISTORY` environment variable can be used to override this value.
 - `-i, --ignore` If to use a list of repositories to ignore. Defaults to true.
 - `--max_results` The amount of starred items to retrieve from GitHub. Defaults to all.
+- `-h --help` Show this help message inside the terminal.
 
 ### Examples
 
-- `gh-star -a ddkasa`
-- `gh-star -a ddkasa -t 5`
-- `gh-star -a ddkasa -r -t 5`
+- `$ gh-star -a ddkasa`
+- `$ gh-star -a ddkasa -t 5`
+- `$ gh-star -a ddkasa -r -t 5`
 
-### Development
+## Development
 
 Development is run through [Poetry](https://github.com/python-poetry/poetry).
 
-#### Basic Setup
+### Basic Setup
 1. `$ git clone https://github.com/ddkasa/github-random-star`
 2. `$ cd github-random-star`
 3. `$ poetry shell`
 4. `$ poetry install`
 
-#### Testing
-- Use `poetry run pytest` for all tests.
-- Use `pytest -m unit` for unit tests.
-- Use `pytest -m integration` for integration tests.
+### Testing
+- Use `$ pytest` for all tests.
+- Use `$ pytest -m unit` for unit tests.
+- Use `$ pytest -m integration` for integration tests.
 
 ## License
 MIT. Look at the [LICENSE](LICENSE.md) for details.
```

#### html2text {}

```diff
@@ -1,42 +1,33 @@
 # â­ï¸ GitHub Random Star â­ï¸ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
 _g_i_t_h_u_b___r_a_n_d_o_m___s_t_a_r_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_][https://img.shields.io/
 github/actions/workflow/status/ddkasa/github-random-star/pypi-
 publish.yml?style=for-the-badge]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_g_i_t_h_u_b_-_r_a_n_d_o_m_-
 _s_t_a_r_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]![](docs/example_image.png?raw=true) If you have
 starred way too many GitHub repositories and need a way of keeping track of
-them. This simple CLI tool throws you quasi random starred repos to look at and
-explore. ## Installation ### Preferred Install with [Pipx](https://github.com/
-pypa/pipx). `pipx install github-random-star` ### Other Install from [PyPi]
-(https://pypi.org/project/github-random-star)/[GitHub](https://github.com/
-ddkasa/github-random-star) with `pip` or clone this repository and install
-requirements through [Poetry](pyproject.toml) or the provided [requirements]
-(requirements.txt) file. If using poetry. $ git clone https://github.com/
-ddkasa/github-random-star
-$ cd github-random-star
-$ poetry shell
-$ poetry install If using requirements.txt. $ git clone https://github.com/
-ddkasa/github-random-star
-$ cd github-random-star
-$ virtualenv -p python3.12 .venv
-$ source .venv/bin/activate
-$ pip install -r requirements.txt ## Usage 1. Setup GitHub API token as the
+them. This simple CLI tool throws you quasi random starred repos at you to look
+at and explore. ## Installation ### Preferred Install with [Pipx](https://
+github.com/pypa/pipx). `$ pipx install github-random-star` ### Other Install
+from [PyPi](https://pypi.org/project/github-random-star)/[GitHub](https://
+github.com/ddkasa/github-random-star) with pip or clone this repository and
+install with pip/pipx locally. ## Usage 1. Setup GitHub API token as the
 `GITHUB_ACCESS_TOKEN` environment variable. _If this is not setup it will use
-the public access point with lower rates._ 2. Run the script through `gh-star
-`, `python github_random_star/main.py ` or if using Poetry `poetry run gh-star
-` ### Flags - `-a, --account` Username of the GitHub account to retrieve the
-starred items from. `--account` is required or `GH_STAR_ACCOUNT` environment
-variable needs to be set. - `-t, --total` Total amount of random items you want
-to pick from. Defaults to 3. - `-r, --refresh` Whether to fetch new cached data
-or not. Will re fetch all starred items instead of using cache. - `--max-
-history` The amount of historic choices to cache. Defaults to 100. Set to **-
-1** to keep history unlimited. `GH_STAR_MAX_HISTORY` environment variable can
-be used to override this value. - `-i, --ignore` If to use a list of
+the public access point with lower rates._ 2. Run the script through `$ gh-star
+`, `$ python github_random_star/main.py ` or if using Poetry `$ poetry run gh-
+star ` ### Flags - `-a, --account` Username of the GitHub account to retrieve
+the starred items from. `--account` is required or `GH_STAR_ACCOUNT`
+environment variable needs to be set. - `-t, --total` Total amount of random
+items you want to pick from. Defaults to 3. - `-r, --refresh` Whether to fetch
+new cached data or not. Will re fetch all starred items instead of using cache.
+- `--max-history` The amount of historic choices to cache. Defaults to 100. Set
+to **-1** to keep history unlimited. `GH_STAR_MAX_HISTORY` environment variable
+can be used to override this value. - `-i, --ignore` If to use a list of
 repositories to ignore. Defaults to true. - `--max_results` The amount of
-starred items to retrieve from GitHub. Defaults to all. ### Examples - `gh-star
--a ddkasa` - `gh-star -a ddkasa -t 5` - `gh-star -a ddkasa -r -t 5` ###
-Development Development is run through [Poetry](https://github.com/python-
-poetry/poetry). #### Basic Setup 1. `$ git clone https://github.com/ddkasa/
-github-random-star` 2. `$ cd github-random-star` 3. `$ poetry shell` 4. `$
-poetry install` #### Testing - Use `poetry run pytest` for all tests. - Use
-`pytest -m unit` for unit tests. - Use `pytest -m integration` for integration
-tests. ## License MIT. Look at the [LICENSE](LICENSE.md) for details.
+starred items to retrieve from GitHub. Defaults to all. - `-h --help` Show this
+help message inside the terminal. ### Examples - `$ gh-star -a ddkasa` - `$ gh-
+star -a ddkasa -t 5` - `$ gh-star -a ddkasa -r -t 5` ## Development Development
+is run through [Poetry](https://github.com/python-poetry/poetry). ### Basic
+Setup 1. `$ git clone https://github.com/ddkasa/github-random-star` 2. `$ cd
+github-random-star` 3. `$ poetry shell` 4. `$ poetry install` ### Testing - Use
+`$ pytest` for all tests. - Use `$ pytest -m unit` for unit tests. - Use `$
+pytest -m integration` for integration tests. ## License MIT. Look at the
+[LICENSE](LICENSE.md) for details.
```

### Comparing `github_random_star-0.0.6/github_random_star/__main__.py` & `github_random_star-0.1.1/github_random_star/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,158 @@
 import json
-import logging as log
+import logging
 import os
 import random
 import subprocess
-from datetime import datetime
 from pathlib import Path
-from typing import NamedTuple, Optional
+from typing import Optional
 
 import fire
-import httpx
 
-USER_API_URL = "https://api.github.com/users/{user}/starred?page={page}&per_page=30"
+from github_random_star.api import GithubAPI
 
-if os.getenv("PYTEST_TESTING"):
-    CACHE_PATH = Path("tests/files")
-
-elif os.name != "nt":
-    CACHE_PATH = Path.home() / Path(".cache")
-else:
-    env = os.getenv("APPDATA")
-    if isinstance(env, str):
-        CACHE_PATH = Path(env)
-    else:
-        CACHE_PATH = Path.home()
-
-CACHE_PATH = CACHE_PATH / Path("github_random_star/")
-
-CACHE_PATH.mkdir(parents=True, exist_ok=True)
-CACHE_FILE = CACHE_PATH / Path("cache.json")
-
-SELECTION_CACHE = CACHE_PATH / Path("selections.json")
-
-IGNORE_FILE = CACHE_PATH / Path("ignore.json")
+log = logging.getLogger("GitHub Random Star")
 
 
 class AccountMissingError(TypeError):
     "GitHub account was not provided through flags or an environment variable."
 
 
-class StarredItem(NamedTuple):
-    repo_id: int
-    name: str
-    url: str
-
-
-def retrieve_cache(
-    account: str,
-    *,
-    refresh: bool = False,
-    max_results: Optional[int] = None,
-) -> set[StarredItem]:
-    """Retrieves data for choosing a random starred item from GitHub.
-
-    Args:
-        account: Github account the starred items will be retrieved from.
-        refresh: Whether or not to refresh the cache. Defaults to False.
-
-    Raises:
-        ConnectionError: If the outgoing request was not successful.
-
-    Returns:
-        set(StarredItem): Set of starred items from GitHub.
-    """
-    if CACHE_FILE.exists() and not refresh:
-        with CACHE_FILE.open("r", encoding="utf-8") as file:
-            cache_data = json.load(file)
-
-        log.info(
-            "Cache last refreshed on the %s.",
-            datetime.fromisoformat(cache_data["date"]).date().isoformat(),
-        )
-        if cache_data.get("account") == account:
-            cache_data = {StarredItem(*item) for item in cache_data["data"]}
-            # TODO: Multiple cache file for different accounts.
-            return cache_data
-
-        log.warning("Cache is storing a different account.")
-
-    log.info("Requesting data from Github")
-
-    headers = {"X-GitHub-Api-Version": "2022-11-28"}
-    API_TOKEN = os.environ.get("GITHUB_ACCESS_TOKEN")
-    if API_TOKEN:
-        log.info("Using provided GitHub API token")
-        headers["Authorization"] = f"Bearer {API_TOKEN}"
-    else:
-        log.warning(
-            "No GitHub API token provided. Using public access with a smaller rate limit."
-        )
-
-    data = set()
-
-    page = 1
-    while True:
-        log.info("Requesting starred items page %s", page)
-        formatted_url = USER_API_URL.format(user=account, page=page)
-        request = httpx.get(formatted_url, timeout=20, headers=headers)
-
-        if request.status_code != 200:
-            err = "Connection failed to get starred items for %s. \
-                Status Code: %s"
-            log.error(err, account, request.status_code)
-            raise ConnectionError(err % account, request.status_code)
-
-        response: list = request.json()
-        if not response:
-            break
-
-        for item in response:
-            tp = StarredItem(item["id"], item["full_name"], item["html_url"])
-            data.add(tp)
-            if max_results and len(data) >= max_results:
-                break
-
-        if max_results and len(data) >= max_results:
-            break
-
-        page += 1
-
-    with CACHE_FILE.open("w", encoding="utf-8") as file:
-        container = {
-            "account": account,
-            "date": datetime.now().isoformat(),
-            "data": tuple(data),
-        }
-        json.dump(container, file)
-
-    return data
-
-
-def extract_selection(path: Path) -> list[StarredItem]:
+def extract_selection(path: Path) -> list[str]:
     """Extracts selections from a JSON file.
 
     Args:
         path: Path to the JSON file.
 
     Returns:
         list(StarredItem): List of starred items from the JSON file. Needs to
             stay a list in order to preserve order when keeping history.
     """
+
     data = []
     if path.exists():
         with path.open("r", encoding="utf-8") as file:
             selections = json.load(file)
             if "data" in selections:
                 selections = selections["data"]
 
-        data = [StarredItem(*item) for item in selections]
-
     return data
 
 
-def item_selection(
-    starred_items: set[StarredItem],
-    *,
+def user_selection(
+    starred_items: set[str],
     total: int,
-    max_history: int = 100,
-    ignore: bool = True,
-) -> None:
+) -> tuple[str, float]:
     """Selection function where the user chooses a random starred item.
 
     Args:
         starred_items: Set of starred items from GitHub.
-        total: Total of choices the user can pick from.
-        max_history: Maximum amount of items to keep in history.
-            Defaults to 100. Set to 0 to disable history or -1 to keep all.
-        ignore: Whether or not to ignore previously selected items.
-            Defaults to True.
-    """
-    og_len = len(starred_items)
-
-    selections = extract_selection(SELECTION_CACHE)
-    if max_history != -1:
-        starred_items = starred_items - starred_items.intersection(selections)
+        total: Number of items to select from.
 
-    if IGNORE_FILE.exists():
-        if ignore:
-            ignore_list = extract_selection(IGNORE_FILE)
-            starred_items = starred_items - starred_items.intersection(ignore_list)
-    else:
-        with IGNORE_FILE.open("w", encoding="utf-8") as file:
-            json.dump([], file)
+    Returns:
+        tuple(StarredItem, float): Selected item and the selection number for
+            further processing
 
+    """
     items = random.sample(tuple(starred_items), total)
 
     print("Which item would you like to select today?")
+    print("Note: Add .1 to number to add to ignore list")
+    # TODO: Add a way of removing a starred item from a user if api key is present.
     while True:
         for i, star in enumerate(items, start=1):
-            if not isinstance(star, StarredItem):
-                star = StarredItem(*star)
-
-            print(f"{i}. {star.name}")
+            print(f"{i}. {star}")
 
         try:
-            selection = int(input("> "))
-            if selection - 1 in range(total):
+            selection = float(input("> "))
+            if int(selection - 1) in range(total):
                 break
         except ValueError:
             pass
 
         print(f"Select an item within the range of 1 and {total}")
 
-    selected_item = StarredItem(*items[selection - 1])
+    selected_item = items[int(selection - 1)]
+
+    return selected_item, selection
 
-    log.info("Opening %s", selected_item.url)
 
+def item_selection(
+    data: dict,
+    cache_path: Path,
+    *,
+    total: int,
+    max_history: int = 100,
+    ignore: bool = True,
+) -> dict:
+    """Selection function where the user chooses a random starred item.
+
+    Args:
+        starred_items: Set of starred items from GitHub.
+        cache_path: Path to the cache directory.
+        total: Total of choices the user can pick from.
+        max_history: Maximum amount of items to keep in history.
+            Defaults to 100. Set to 0 to disable history or -1 to keep all.
+        ignore: Whether or not to ignore previously selected items.
+            Defaults to True.
+    """
+
+    starred_items = set(data["data"])
+
+    # TODO: Need a way of avoiding keeping enough items in the history.
+    if max_history != -1:
+        starred_items -= starred_items.intersection(set(data["history"]))
+
+    if ignore:
+        starred_items -= starred_items.intersection(set(data["ignore"]))
+
+    selected_item, selection = user_selection(starred_items, total)
+
+    gh_url = "https://github.com/" + selected_item
+
+    log.info("Opening %s", gh_url)
     subprocess.run(
-        ["python", "-m", "webbrowser", "-t", selected_item.url],
+        ["python", "-m", "webbrowser", "-t", gh_url],
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
 
-    selections.insert(0, selected_item)
-    if len(selections) > max_history and max_history > 0:
-        selections = selections[: -(len(selections) - max_history)]
+    if round(selection % 1, 1) == 0.1:
+        log.info("Adding %s to ignore list", selected_item)
+        data["ignore"].append(selected_item)
+
+    data["history"].insert(0, selected_item)
+    if len(data["history"]) > max_history and max_history > 0:
+        data["history"] = data["history"][: -(len(data["history"]) - max_history)]
+
+    return data
+
+
+def generate_cache_directory():
+    """Setup for cache directory depending on the OS.
+
+    Returns:
+        Path: Path to the cache directory.
+    """
+    if os.getenv("PYTEST_TESTING"):
+        CACHE_PATH = Path("tests/files")
+
+    elif os.name != "nt":
+        CACHE_PATH = Path.home() / Path(".cache")
+    else:
+        env = os.getenv("APPDATA")
+        if isinstance(env, str):
+            CACHE_PATH = Path(env)
+        else:
+            CACHE_PATH = Path.home()
 
-    if og_len == len(starred_items) and max_history == -1:
-        selections = []
+    CACHE_PATH = CACHE_PATH / Path("github_random_star/")
+    CACHE_PATH.mkdir(parents=True, exist_ok=True)
 
-    with SELECTION_CACHE.open("w", encoding="utf-8") as file:
-        json.dump(selections, file)
+    return CACHE_PATH
 
 
 def main(
     account: Optional[str] = None,
     total: int = 3,
     refresh: bool = False,
     max_history: Optional[int] = None,
@@ -232,40 +161,49 @@
 ) -> None:
     """Basic entrypoint for the CLI script.
 
     Raises:
         AccountMissingError: If the GitHub account was not provided through
             flags or an environment variables.
     """
-    log.basicConfig(
+    logging.basicConfig(
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
-        level=log.INFO,
+        level=logging.INFO,
     )
+    cache_path = generate_cache_directory()
 
     if account is None:
         account = os.environ.get("GH_STAR_ACCOUNT")
         if account is None:
             raise AccountMissingError()
 
     if max_history is None:
         max_history = int(os.environ.get("GH_STAR_MAX_HISTORY", 100))
 
-    starred_items = retrieve_cache(
+    token = os.environ.get("GITHUB_ACCESS_TOKEN")
+    github_api = GithubAPI(
         account,
+        cache_path,
         refresh=refresh,
         max_results=max_results,
+        token=token,
     )
 
+    starred_items = github_api.collect_starred_items()
+
     log.info("Total amount of starred items: %s", len(starred_items))
 
-    item_selection(
+    data = item_selection(
         starred_items,
+        cache_path,
         total=total,
         max_history=max_history,
         ignore=ignore,
     )
 
+    github_api.save_cached_items(data["data"], data)
+
     log.info("Done!")
 
 
 if __name__ == "__main__":
     fire.Fire(main)
```

### Comparing `github_random_star-0.0.6/pyproject.toml` & `github_random_star-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "github-random-star"
-version = "0.0.6"
+version = "0.1.1"
 description = "Simple CLI tool to fetch random starred items from a users GitHub profile."
 authors = ["David Kasakaitis <davidkasakaitis@proton.me>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.12",
@@ -56,7 +56,11 @@
 [tool.pytest.ini_options]
 env = [
     "PYTEST_TESTING=True",
 ]
 pythonpath = [
   "."
 ]
+markers = [
+    "unit: Basic unit tests using local cache.",
+    "integration: Tests that use the API.",
+]
```

### Comparing `github_random_star-0.0.6/PKG-INFO` & `github_random_star-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-random-star
-Version: 0.0.6
+Version: 0.1.1
 Summary: Simple CLI tool to fetch random starred items from a users GitHub profile.
 License: MIT
 Keywords: python,python3,cli,github,git
 Author: David Kasakaitis
 Author-email: davidkasakaitis@proton.me
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,75 +30,60 @@
 
 <a href="https://pypi.org/project/github-random-star"><img src="https://img.shields.io/pypi/v/github_random_star?style=for-the-badge&logo=pypi" /></a>
 <a href=""><img src="https://img.shields.io/github/actions/workflow/status/ddkasa/github-random-star/pypi-publish.yml?style=for-the-badge"/></a>
 <a href="https://pypi.org/project/github-random-star"><img src="https://img.shields.io/pypi/dm/github-random-star?style=for-the-badge" /></a>
 
 ![](docs/example_image.png?raw=true)
 
-If you have starred way too many GitHub repositories and need a way of keeping track of them. This simple CLI tool throws you quasi random starred repos to look at and explore.
+If you have starred way too many GitHub repositories and need a way of keeping track of them. This simple CLI tool throws you quasi random starred repos at you to look at and explore.
 
 ## Installation
 
 ### Preferred
 
 Install with [Pipx](https://github.com/pypa/pipx).
 
-`pipx install github-random-star`
+`$ pipx install github-random-star`
 
 ### Other
 
-Install from [PyPi](https://pypi.org/project/github-random-star)/[GitHub](https://github.com/ddkasa/github-random-star) with `pip` or clone this repository and install requirements through [Poetry](pyproject.toml) or the provided [requirements](requirements.txt) file.
-
-<details>
-    <summary>If using poetry.</summary>
-    <code>$ git clone https://github.com/ddkasa/github-random-star</code><br>
-    <code>$ cd github-random-star</code><br>
-    <code>$ poetry shell</code><br>
-    <code>$ poetry install</code>
-</details>
-<details>
-    <summary>If using requirements.txt.</summary>
-    <code>$ git clone https://github.com/ddkasa/github-random-star</code><br>
-    <code>$ cd github-random-star</code><br>
-    <code>$ virtualenv -p python3.12 .venv</code><br>
-    <code>$ source .venv/bin/activate</code><br>
-    <code>$ pip install -r requirements.txt</code>
-</details>
+Install from [PyPi](https://pypi.org/project/github-random-star)/[GitHub](https://github.com/ddkasa/github-random-star) with pip or clone this repository and install with pip/pipx locally.
 
 ## Usage
 
 1. Setup GitHub API token as the `GITHUB_ACCESS_TOKEN` environment variable. _If this is not setup it will use the public access point with lower rates._
-2. Run the script through `gh-star <flags>`, `python github_random_star/main.py <flags>` or if using Poetry `poetry run gh-star <flags>`
+2. Run the script through `$ gh-star <flags>`, `$ python github_random_star/main.py <flags>` or if using Poetry `$ poetry run gh-star <flags>`
 
 ### Flags
 
 - `-a, --account` Username of the GitHub account to retrieve the starred items from. `--account` is required or `GH_STAR_ACCOUNT` environment variable needs to be set.
 - `-t, --total` Total amount of random items you want to pick from. Defaults to 3.
 - `-r, --refresh` Whether to fetch new cached data or not. Will re fetch all starred items instead of using cache.
 - `--max-history` The amount of historic choices to cache. Defaults to 100. Set to **-1** to keep history unlimited. `GH_STAR_MAX_HISTORY` environment variable can be used to override this value.
 - `-i, --ignore` If to use a list of repositories to ignore. Defaults to true.
 - `--max_results` The amount of starred items to retrieve from GitHub. Defaults to all.
+- `-h --help` Show this help message inside the terminal.
 
 ### Examples
 
-- `gh-star -a ddkasa`
-- `gh-star -a ddkasa -t 5`
-- `gh-star -a ddkasa -r -t 5`
+- `$ gh-star -a ddkasa`
+- `$ gh-star -a ddkasa -t 5`
+- `$ gh-star -a ddkasa -r -t 5`
 
-### Development
+## Development
 
 Development is run through [Poetry](https://github.com/python-poetry/poetry).
 
-#### Basic Setup
+### Basic Setup
 1. `$ git clone https://github.com/ddkasa/github-random-star`
 2. `$ cd github-random-star`
 3. `$ poetry shell`
 4. `$ poetry install`
 
-#### Testing
-- Use `poetry run pytest` for all tests.
-- Use `pytest -m unit` for unit tests.
-- Use `pytest -m integration` for integration tests.
+### Testing
+- Use `$ pytest` for all tests.
+- Use `$ pytest -m unit` for unit tests.
+- Use `$ pytest -m integration` for integration tests.
 
 ## License
 MIT. Look at the [LICENSE](LICENSE.md) for details.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: github-random-star Version: 0.0.6 Summary: Simple
+Metadata-Version: 2.1 Name: github-random-star Version: 0.1.1 Summary: Simple
 CLI tool to fetch random starred items from a users GitHub profile. License:
 MIT Keywords: python,python3,cli,github,git Author: David Kasakaitis Author-
 email: davidkasakaitis@proton.me Requires-Python: >=3.12,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
@@ -16,42 +16,34 @@
 random-star Description-Content-Type: text/markdown # â­ï¸ GitHub Random Star
 â­ï¸ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_i_t_h_u_b___r_a_n_d_o_m___s_t_a_r_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
 _b_a_d_g_e_&_l_o_g_o_=_p_y_p_i_][https://img.shields.io/github/actions/workflow/status/ddkasa/
 github-random-star/pypi-publish.yml?style=for-the-badge]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_g_i_t_h_u_b_-_r_a_n_d_o_m_-_s_t_a_r_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]![](docs/
 example_image.png?raw=true) If you have starred way too many GitHub
 repositories and need a way of keeping track of them. This simple CLI tool
-throws you quasi random starred repos to look at and explore. ## Installation
-### Preferred Install with [Pipx](https://github.com/pypa/pipx). `pipx install
-github-random-star` ### Other Install from [PyPi](https://pypi.org/project/
-github-random-star)/[GitHub](https://github.com/ddkasa/github-random-star) with
-`pip` or clone this repository and install requirements through [Poetry]
-(pyproject.toml) or the provided [requirements](requirements.txt) file. If
-using poetry. $ git clone https://github.com/ddkasa/github-random-star
-$ cd github-random-star
-$ poetry shell
-$ poetry install If using requirements.txt. $ git clone https://github.com/
-ddkasa/github-random-star
-$ cd github-random-star
-$ virtualenv -p python3.12 .venv
-$ source .venv/bin/activate
-$ pip install -r requirements.txt ## Usage 1. Setup GitHub API token as the
-`GITHUB_ACCESS_TOKEN` environment variable. _If this is not setup it will use
-the public access point with lower rates._ 2. Run the script through `gh-star
-`, `python github_random_star/main.py ` or if using Poetry `poetry run gh-star
-` ### Flags - `-a, --account` Username of the GitHub account to retrieve the
-starred items from. `--account` is required or `GH_STAR_ACCOUNT` environment
-variable needs to be set. - `-t, --total` Total amount of random items you want
-to pick from. Defaults to 3. - `-r, --refresh` Whether to fetch new cached data
-or not. Will re fetch all starred items instead of using cache. - `--max-
-history` The amount of historic choices to cache. Defaults to 100. Set to **-
-1** to keep history unlimited. `GH_STAR_MAX_HISTORY` environment variable can
-be used to override this value. - `-i, --ignore` If to use a list of
-repositories to ignore. Defaults to true. - `--max_results` The amount of
-starred items to retrieve from GitHub. Defaults to all. ### Examples - `gh-star
--a ddkasa` - `gh-star -a ddkasa -t 5` - `gh-star -a ddkasa -r -t 5` ###
-Development Development is run through [Poetry](https://github.com/python-
-poetry/poetry). #### Basic Setup 1. `$ git clone https://github.com/ddkasa/
-github-random-star` 2. `$ cd github-random-star` 3. `$ poetry shell` 4. `$
-poetry install` #### Testing - Use `poetry run pytest` for all tests. - Use
-`pytest -m unit` for unit tests. - Use `pytest -m integration` for integration
-tests. ## License MIT. Look at the [LICENSE](LICENSE.md) for details.
+throws you quasi random starred repos at you to look at and explore. ##
+Installation ### Preferred Install with [Pipx](https://github.com/pypa/pipx).
+`$ pipx install github-random-star` ### Other Install from [PyPi](https://
+pypi.org/project/github-random-star)/[GitHub](https://github.com/ddkasa/github-
+random-star) with pip or clone this repository and install with pip/pipx
+locally. ## Usage 1. Setup GitHub API token as the `GITHUB_ACCESS_TOKEN`
+environment variable. _If this is not setup it will use the public access point
+with lower rates._ 2. Run the script through `$ gh-star `, `$ python
+github_random_star/main.py ` or if using Poetry `$ poetry run gh-star ` ###
+Flags - `-a, --account` Username of the GitHub account to retrieve the starred
+items from. `--account` is required or `GH_STAR_ACCOUNT` environment variable
+needs to be set. - `-t, --total` Total amount of random items you want to pick
+from. Defaults to 3. - `-r, --refresh` Whether to fetch new cached data or not.
+Will re fetch all starred items instead of using cache. - `--max-history` The
+amount of historic choices to cache. Defaults to 100. Set to **-1** to keep
+history unlimited. `GH_STAR_MAX_HISTORY` environment variable can be used to
+override this value. - `-i, --ignore` If to use a list of repositories to
+ignore. Defaults to true. - `--max_results` The amount of starred items to
+retrieve from GitHub. Defaults to all. - `-h --help` Show this help message
+inside the terminal. ### Examples - `$ gh-star -a ddkasa` - `$ gh-star -
+a ddkasa -t 5` - `$ gh-star -a ddkasa -r -t 5` ## Development Development is
+run through [Poetry](https://github.com/python-poetry/poetry). ### Basic Setup
+1. `$ git clone https://github.com/ddkasa/github-random-star` 2. `$ cd github-
+random-star` 3. `$ poetry shell` 4. `$ poetry install` ### Testing - Use `$
+pytest` for all tests. - Use `$ pytest -m unit` for unit tests. - Use `$ pytest
+-m integration` for integration tests. ## License MIT. Look at the [LICENSE]
+(LICENSE.md) for details.
```

