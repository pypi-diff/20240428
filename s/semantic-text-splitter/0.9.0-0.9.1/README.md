# Comparing `tmp/semantic_text_splitter-0.9.0.tar.gz` & `tmp/semantic_text_splitter-0.9.1.tar.gz`

## Comparing `semantic_text_splitter-0.9.0.tar` & `semantic_text_splitter-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0     1001      127       40 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/.gitignore
--rw-r--r--   0     1001      127    12460 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/CHANGELOG.md
--rw-r--r--   0     1001      127     5229 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1072 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/LICENSE.txt
--rw-r--r--   0     1001      127     9928 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/README.md
--rw-r--r--   0     1001      127     3891 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/benches/chunk_size.rs
--rw-r--r--   0     1001      127      322 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/clippy.toml
--rw-r--r--   0     1001      127      952 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size/characters.rs
--rw-r--r--   0     1001      127     2689 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size/huggingface.rs
--rw-r--r--   0     1001      127     1300 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size/tiktoken.rs
--rw-r--r--   0     1001      127    13100 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/chunk_size.rs
--rw-r--r--   0     1001      127    12856 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/lib.rs
--rw-r--r--   0     1001      127    38979 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/markdown.rs
--rw-r--r--   0     1001      127    18431 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/src/text.rs
--rw-r--r--   0     1001      127     4356 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/tests/markdown.rs
--rw-r--r--   0     1001      127     2889 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/tests/text_splitter.rs
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      718 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/.gitignore
--rw-r--r--   0     1001      127     2876 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/CHANGELOG.md
--rw-r--r--   0     1001      127     6998 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/README.md
--rw-r--r--   0     1001      127    17938 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/semantic_text_splitter.pyi
--rw-r--r--   0     1001      127    26104 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127   711396 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/tests/bert-base-cased.json
--rw-r--r--   0     1001      127     5848 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/bindings/python/tests/test_integration.py
--rw-r--r--   0     1001      127    45485 2024-04-04 05:05:43.000000 semantic_text_splitter-0.9.0/Cargo.lock
--rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/Cargo.toml
--rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.0/PKG-INFO
+-rw-r--r--   0     1001      127       40 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/.gitignore
+-rw-r--r--   0     1001      127    13198 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/CHANGELOG.md
+-rw-r--r--   0     1001      127     5229 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1072 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/LICENSE.txt
+-rw-r--r--   0     1001      127     9928 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/README.md
+-rw-r--r--   0     1001      127     3891 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/benches/chunk_size.rs
+-rw-r--r--   0     1001      127      322 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/clippy.toml
+-rw-r--r--   0     1001      127      952 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/src/chunk_size/characters.rs
+-rw-r--r--   0     1001      127     2689 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/src/chunk_size/huggingface.rs
+-rw-r--r--   0     1001      127     1300 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/src/chunk_size/tiktoken.rs
+-rw-r--r--   0     1001      127    13100 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/src/chunk_size.rs
+-rw-r--r--   0     1001      127    12856 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/src/lib.rs
+-rw-r--r--   0     1001      127    38979 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/src/markdown.rs
+-rw-r--r--   0     1001      127    18431 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/src/text.rs
+-rw-r--r--   0     1001      127     4356 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/tests/markdown.rs
+-rw-r--r--   0     1001      127     2889 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/tests/text_splitter.rs
+-rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.1/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      718 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/bindings/python/.gitignore
+-rw-r--r--   0     1001      127     2876 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/bindings/python/CHANGELOG.md
+-rw-r--r--   0     1001      127     6998 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/bindings/python/README.md
+-rw-r--r--   0     1001      127    20252 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/bindings/python/semantic_text_splitter.pyi
+-rw-r--r--   0     1001      127    31110 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127   711396 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/bindings/python/tests/bert-base-cased.json
+-rw-r--r--   0     1001      127     7054 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/bindings/python/tests/test_integration.py
+-rw-r--r--   0     1001      127    45500 2024-04-04 16:25:23.000000 semantic_text_splitter-0.9.1/Cargo.lock
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.1/Cargo.toml
+-rw-r--r--   0        0        0      517 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7928 1970-01-01 00:00:00.000000 semantic_text_splitter-0.9.1/PKG-INFO
```

### Comparing `semantic_text_splitter-0.9.0/CHANGELOG.md` & `semantic_text_splitter-0.9.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## v0.9.1
+
+### What's New
+
+Python `TextSplitter` and `MarkdownSplitter` now both provide a new `chunk_indices` method that returns a list not only of chunks, but also their corresponding character offsets relative to the original text. This should allow for different string comparison and matching operations on the chunks.
+
+```python
+def chunk_indices(
+    self, text: str, chunk_capacity: Union[int, Tuple[int, int]]
+) -> List[Tuple[int, str]]:
+    ...
+```
+
+A similar method already existed on the Rust side. The key difference is that these offsets are **character** not **byte** offsets. For Rust strings, it is usually helpful to have the byte offset, but in Python, most string methods and operations deal with character indices.
+
 ## v0.9.0
 
 ### What's New
 
 [More robust handling of Hugging Face tokenizers as chunk sizers.](https://github.com/benbrandt/text-splitter/pull/131)
 
 - **Tokenizers with padding enabled no longer count padding tokens when generating chunks**. This caused some unexpected behavior, especially if the chunk capacity didn't perfectly line up with the padding size(s). Now, the tokenizer's padding token is ignored when counting the number of tokens generated in a chunk.
```

### Comparing `semantic_text_splitter-0.9.0/CODE_OF_CONDUCT.md` & `semantic_text_splitter-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/LICENSE.txt` & `semantic_text_splitter-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/README.md` & `semantic_text_splitter-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/benches/chunk_size.rs` & `semantic_text_splitter-0.9.1/benches/chunk_size.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/src/chunk_size/characters.rs` & `semantic_text_splitter-0.9.1/src/chunk_size/characters.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/src/chunk_size/huggingface.rs` & `semantic_text_splitter-0.9.1/src/chunk_size/huggingface.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/src/chunk_size/tiktoken.rs` & `semantic_text_splitter-0.9.1/src/chunk_size/tiktoken.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/src/chunk_size.rs` & `semantic_text_splitter-0.9.1/src/chunk_size.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/src/lib.rs` & `semantic_text_splitter-0.9.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/src/markdown.rs` & `semantic_text_splitter-0.9.1/src/markdown.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/src/text.rs` & `semantic_text_splitter-0.9.1/src/text.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/tests/markdown.rs` & `semantic_text_splitter-0.9.1/tests/markdown.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/tests/text_splitter.rs` & `semantic_text_splitter-0.9.1/tests/text_splitter.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/bindings/python/Cargo.toml` & `semantic_text_splitter-0.9.1/bindings/python/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "semantic_text_splitter"
 crate-type = ["cdylib"]
 
 [dependencies]
+auto_enums = "0.8.5"
 pyo3 = { version = "0.21.1", features = ["abi3-py38"] }
 text-splitter = { path = "../..", features = [
     "markdown",
     "tiktoken-rs",
     "tokenizers",
 ] }
 tiktoken-rs = "0.5.8"
```

### Comparing `semantic_text_splitter-0.9.0/bindings/python/.gitignore` & `semantic_text_splitter-0.9.1/bindings/python/.gitignore`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/bindings/python/CHANGELOG.md` & `semantic_text_splitter-0.9.1/bindings/python/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/bindings/python/README.md` & `semantic_text_splitter-0.9.1/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/bindings/python/semantic_text_splitter.pyi` & `semantic_text_splitter-0.9.1/bindings/python/semantic_text_splitter.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -198,14 +198,36 @@
                 up the chunk until the lower range is met.
 
         Returns:
             A list of strings, one for each chunk. If `trim_chunks` was specified in the text
             splitter, then each chunk will already be trimmed as well.
         """
 
+    def chunk_indices(
+        self, text: str, chunk_capacity: Union[int, Tuple[int, int]]
+    ) -> List[Tuple[int, str]]:
+        """Generate a list of chunks from a given text, along with their character offsets in the original text. Each chunk will be up to the `chunk_capacity`.
+
+        See `chunks` for more information.
+
+        Args:
+            text (str): Text to split.
+            chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+                single int, then chunks will be filled up as much as possible, without going over
+                that number. If a tuple of two integers is provided, a chunk will be considered
+                "full" once it is within the two numbers (inclusive range). So it will only fill
+                up the chunk until the lower range is met.
+
+        Returns:
+            A list of tuples, one for each chunk. The first item will be the character offset relative
+            to the original text. The second item is the chunk itself.
+            If `trim_chunks` was specified in the text splitter, then each chunk will already be
+            trimmed as well.
+        """
+
 
 class MarkdownSplitter:
     """Markdown splitter. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
 
     ### By Number of Characters
 
     ```python
@@ -410,7 +432,29 @@
                 "full" once it is within the two numbers (inclusive range). So it will only fill
                 up the chunk until the lower range is met.
 
         Returns:
             A list of strings, one for each chunk. If `trim_chunks` was specified in the text
             splitter, then each chunk will already be trimmed as well.
         """
+
+    def chunk_indices(
+        self, text: str, chunk_capacity: Union[int, Tuple[int, int]]
+    ) -> List[Tuple[int, str]]:
+        """Generate a list of chunks from a given text, along with their character offsets in the original text. Each chunk will be up to the `chunk_capacity`.
+
+        See `chunks` for more information.
+
+        Args:
+            text (str): Text to split.
+            chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+                single int, then chunks will be filled up as much as possible, without going over
+                that number. If a tuple of two integers is provided, a chunk will be considered
+                "full" once it is within the two numbers (inclusive range). So it will only fill
+                up the chunk until the lower range is met.
+
+        Returns:
+            A list of tuples, one for each chunk. The first item will be the character offset relative
+            to the original text. The second item is the chunk itself.
+            If `trim_chunks` was specified in the text splitter, then each chunk will already be
+            trimmed as well.
+        """
```

### Comparing `semantic_text_splitter-0.9.0/bindings/python/src/lib.rs` & `semantic_text_splitter-0.9.1/bindings/python/src/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     unused
 )]
 // pyo3 uses this
 #![allow(elided_lifetimes_in_paths)]
 
 use std::str::FromStr;
 
+use auto_enums::auto_enum;
 use pyo3::{exceptions::PyException, prelude::*, pybacked::PyBackedStr};
 use text_splitter::{
     Characters, ChunkCapacity, ChunkSize, ChunkSizer, MarkdownSplitter, TextSplitter,
 };
 use tiktoken_rs::{get_bpe_from_model, CoreBPE};
 use tokenizers::Tokenizer;
 
@@ -63,29 +64,76 @@
                 .unwrap();
 
             ChunkSize::from_size(size, capacity)
         })
     }
 }
 
+/// Keeps track of the corresponding byte to character offset in a text
+struct ByteToCharOffsetTracker<'text> {
+    byte_offset: usize,
+    char_offset: usize,
+    text: &'text str,
+}
+
+impl<'text> ByteToCharOffsetTracker<'text> {
+    fn new(text: &'text str) -> Self {
+        Self {
+            byte_offset: 0,
+            char_offset: 0,
+            text,
+        }
+    }
+
+    /// Updates the current offsets, but is able to cache previous results
+    fn map_byte_to_char(&mut self, (offset, chunk): (usize, &'text str)) -> (usize, &'text str) {
+        let prev_text = self
+            .text
+            .get(self.byte_offset..offset)
+            .expect("Invalid byte sequence");
+        self.byte_offset = offset;
+        self.char_offset += prev_text.chars().count();
+        (self.char_offset, chunk)
+    }
+}
+
 #[allow(clippy::large_enum_variant)]
 enum TextSplitterOptions {
     Characters(TextSplitter<Characters>),
     CustomCallback(TextSplitter<CustomCallback>),
     Huggingface(TextSplitter<Tokenizer>),
     Tiktoken(TextSplitter<CoreBPE>),
 }
 
 impl TextSplitterOptions {
-    fn chunks<'text>(&self, text: &'text str, chunk_capacity: PyChunkCapacity) -> Vec<&'text str> {
+    #[auto_enum(Iterator)]
+    fn chunks<'splitter, 'text: 'splitter>(
+        &'splitter self,
+        text: &'text str,
+        chunk_capacity: PyChunkCapacity,
+    ) -> impl Iterator<Item = &'text str> + 'splitter {
         match self {
-            Self::Characters(splitter) => splitter.chunks(text, chunk_capacity).collect(),
-            Self::CustomCallback(splitter) => splitter.chunks(text, chunk_capacity).collect(),
-            Self::Huggingface(splitter) => splitter.chunks(text, chunk_capacity).collect(),
-            Self::Tiktoken(splitter) => splitter.chunks(text, chunk_capacity).collect(),
+            Self::Characters(splitter) => splitter.chunks(text, chunk_capacity),
+            Self::CustomCallback(splitter) => splitter.chunks(text, chunk_capacity),
+            Self::Huggingface(splitter) => splitter.chunks(text, chunk_capacity),
+            Self::Tiktoken(splitter) => splitter.chunks(text, chunk_capacity),
+        }
+    }
+
+    #[auto_enum(Iterator)]
+    fn chunk_indices<'splitter, 'text: 'splitter>(
+        &'splitter self,
+        text: &'text str,
+        chunk_capacity: PyChunkCapacity,
+    ) -> impl Iterator<Item = (usize, &'text str)> + 'splitter {
+        match self {
+            Self::Characters(splitter) => splitter.chunk_indices(text, chunk_capacity),
+            Self::CustomCallback(splitter) => splitter.chunk_indices(text, chunk_capacity),
+            Self::Huggingface(splitter) => splitter.chunk_indices(text, chunk_capacity),
+            Self::Tiktoken(splitter) => splitter.chunk_indices(text, chunk_capacity),
         }
     }
 }
 
 /**
 Plain-text splitter. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
 
@@ -347,33 +395,83 @@
         splitter, then each chunk will already be trimmed as well.
     */
     fn chunks<'text, 'splitter: 'text>(
         &'splitter self,
         text: &'text str,
         chunk_capacity: PyChunkCapacity,
     ) -> Vec<&'text str> {
-        self.splitter.chunks(text, chunk_capacity)
+        self.splitter.chunks(text, chunk_capacity).collect()
+    }
+
+    /**
+    Generate a list of chunks from a given text, along with their character offsets in the original text. Each chunk will be up to the `chunk_capacity`.
+
+    See `chunks` for more information.
+
+    Args:
+        text (str): Text to split.
+        chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+            single int, then chunks will be filled up as much as possible, without going over
+            that number. If a tuple of two integers is provided, a chunk will be considered
+            "full" once it is within the two numbers (inclusive range). So it will only fill
+            up the chunk until the lower range is met.
+
+    Returns:
+        A list of tuples, one for each chunk. The first item will be the character offset relative
+        to the original text. The second item is the chunk itself.
+        If `trim_chunks` was specified in the text splitter, then each chunk will already be
+        trimmed as well.
+    */
+    fn chunk_indices<'text, 'splitter: 'text>(
+        &'splitter self,
+        text: &'text str,
+        chunk_capacity: PyChunkCapacity,
+    ) -> Vec<(usize, &'text str)> {
+        let mut offsets = ByteToCharOffsetTracker::new(text);
+        self.splitter
+            .chunk_indices(text, chunk_capacity)
+            .map(|c| offsets.map_byte_to_char(c))
+            .collect()
     }
 }
 
 #[allow(clippy::large_enum_variant)]
 enum MarkdownSplitterOptions {
     Characters(MarkdownSplitter<Characters>),
     CustomCallback(MarkdownSplitter<CustomCallback>),
     Huggingface(MarkdownSplitter<Tokenizer>),
     Tiktoken(MarkdownSplitter<CoreBPE>),
 }
 
 impl MarkdownSplitterOptions {
-    fn chunks<'text>(&self, text: &'text str, chunk_capacity: PyChunkCapacity) -> Vec<&'text str> {
+    #[auto_enum(Iterator)]
+    fn chunks<'splitter, 'text: 'splitter>(
+        &'splitter self,
+        text: &'text str,
+        chunk_capacity: PyChunkCapacity,
+    ) -> impl Iterator<Item = &'text str> + 'splitter {
+        match self {
+            Self::Characters(splitter) => splitter.chunks(text, chunk_capacity),
+            Self::CustomCallback(splitter) => splitter.chunks(text, chunk_capacity),
+            Self::Huggingface(splitter) => splitter.chunks(text, chunk_capacity),
+            Self::Tiktoken(splitter) => splitter.chunks(text, chunk_capacity),
+        }
+    }
+
+    #[auto_enum(Iterator)]
+    fn chunk_indices<'splitter, 'text: 'splitter>(
+        &'splitter self,
+        text: &'text str,
+        chunk_capacity: PyChunkCapacity,
+    ) -> impl Iterator<Item = (usize, &'text str)> + 'splitter {
         match self {
-            Self::Characters(splitter) => splitter.chunks(text, chunk_capacity).collect(),
-            Self::CustomCallback(splitter) => splitter.chunks(text, chunk_capacity).collect(),
-            Self::Huggingface(splitter) => splitter.chunks(text, chunk_capacity).collect(),
-            Self::Tiktoken(splitter) => splitter.chunks(text, chunk_capacity).collect(),
+            Self::Characters(splitter) => splitter.chunk_indices(text, chunk_capacity),
+            Self::CustomCallback(splitter) => splitter.chunk_indices(text, chunk_capacity),
+            Self::Huggingface(splitter) => splitter.chunk_indices(text, chunk_capacity),
+            Self::Tiktoken(splitter) => splitter.chunk_indices(text, chunk_capacity),
         }
     }
 }
 
 /**
 Markdown splitter. Recursively splits chunks into the largest semantic units that fit within the chunk size. Also will attempt to merge neighboring chunks if they can fit within the given chunk size.
 
@@ -661,15 +759,46 @@
         splitter, then each chunk will already be trimmed as well.
     */
     fn chunks<'text, 'splitter: 'text>(
         &'splitter self,
         text: &'text str,
         chunk_capacity: PyChunkCapacity,
     ) -> Vec<&'text str> {
-        self.splitter.chunks(text, chunk_capacity)
+        self.splitter.chunks(text, chunk_capacity).collect()
+    }
+
+    /**
+    Generate a list of chunks from a given text, along with their character offsets in the original text. Each chunk will be up to the `chunk_capacity`.
+
+    See `chunks` for more information.
+
+    Args:
+        text (str): Text to split.
+        chunk_capacity (int | (int, int)): The capacity of characters in each chunk. If a
+            single int, then chunks will be filled up as much as possible, without going over
+            that number. If a tuple of two integers is provided, a chunk will be considered
+            "full" once it is within the two numbers (inclusive range). So it will only fill
+            up the chunk until the lower range is met.
+
+    Returns:
+        A list of tuples, one for each chunk. The first item will be the character offset relative
+        to the original text. The second item is the chunk itself.
+        If `trim_chunks` was specified in the text splitter, then each chunk will already be
+        trimmed as well.
+    */
+    fn chunk_indices<'text, 'splitter: 'text>(
+        &'splitter self,
+        text: &'text str,
+        chunk_capacity: PyChunkCapacity,
+    ) -> Vec<(usize, &'text str)> {
+        let mut offsets = ByteToCharOffsetTracker::new(text);
+        self.splitter
+            .chunk_indices(text, chunk_capacity)
+            .map(|c| offsets.map_byte_to_char(c))
+            .collect()
     }
 }
 
 #[doc = include_str!("../README.md")]
 #[pymodule]
 fn semantic_text_splitter(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyTextSplitter>()?;
```

### Comparing `semantic_text_splitter-0.9.0/bindings/python/tests/bert-base-cased.json` & `semantic_text_splitter-0.9.1/bindings/python/tests/bert-base-cased.json`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/bindings/python/tests/test_integration.py` & `semantic_text_splitter-0.9.1/bindings/python/tests/test_integration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,189 +1,229 @@
 import pytest
 from semantic_text_splitter import MarkdownSplitter, TextSplitter
 from tokenizers import Tokenizer
 
 
-def test_chunks():
+def test_chunks() -> None:
     splitter = TextSplitter(trim_chunks=False)
     text = "123\n123"
     assert splitter.chunks(text, 4) == ["123\n", "123"]
 
 
-def test_chunks_range():
+def test_chunks_range() -> None:
     splitter = TextSplitter(trim_chunks=False)
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=(3, 4)) == [
         "123",
         "\n123",
     ]
 
 
-def test_chunks_trim():
+def test_chunks_trim() -> None:
     splitter = TextSplitter()
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=4) == ["123", "123"]
 
 
-def test_hugging_face():
+def test_hugging_face() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = TextSplitter.from_huggingface_tokenizer(tokenizer, trim_chunks=False)
     text = "123\n123"
     assert splitter.chunks(text, 1) == ["123\n", "123"]
 
 
-def test_hugging_face_range():
+def test_hugging_face_range() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = TextSplitter.from_huggingface_tokenizer(tokenizer, trim_chunks=False)
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=(1, 2)) == ["123\n", "123"]
 
 
-def test_hugging_face_trim():
+def test_hugging_face_trim() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = TextSplitter.from_huggingface_tokenizer(tokenizer)
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_hugging_face_from_str():
+def test_hugging_face_from_str() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = TextSplitter.from_huggingface_tokenizer_str(tokenizer.to_str())
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_hugging_face_from_file():
+def test_hugging_face_from_file() -> None:
     splitter = TextSplitter.from_huggingface_tokenizer_file(
         "tests/bert-base-cased.json"
     )
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_tiktoken():
+def test_tiktoken() -> None:
     splitter = TextSplitter.from_tiktoken_model(
         model="gpt-3.5-turbo", trim_chunks=False
     )
     text = "123\n123"
     assert splitter.chunks(text, 2) == ["123\n", "123"]
 
 
-def test_tiktoken_range():
+def test_tiktoken_range() -> None:
     splitter = TextSplitter.from_tiktoken_model(
         model="gpt-3.5-turbo", trim_chunks=False
     )
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=(2, 3)) == [
         "123\n",
         "123",
     ]
 
 
-def test_tiktoken_trim():
+def test_tiktoken_trim() -> None:
     splitter = TextSplitter.from_tiktoken_model("gpt-3.5-turbo")
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_tiktoken_model_error():
+def test_tiktoken_model_error() -> None:
     with pytest.raises(Exception):
         TextSplitter.from_tiktoken_model("random-model-name")
 
 
-def test_custom():
+def test_custom() -> None:
     splitter = TextSplitter.from_callback(lambda x: len(x))
     text = "123\n123"
     assert splitter.chunks(text=text, chunk_capacity=3) == ["123", "123"]
 
 
-def test_markdown_chunks():
+def test_markdown_chunks() -> None:
     splitter = MarkdownSplitter(trim_chunks=False)
     text = "123\n\n123"
     assert splitter.chunks(text, 4) == ["123\n", "\n123"]
 
 
-def test_markdown_chunks_range():
+def test_markdown_chunks_range() -> None:
     splitter = MarkdownSplitter(trim_chunks=False)
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=(3, 4)) == [
         "123\n",
         "\n123",
     ]
 
 
-def test_markdown_chunks_trim():
+def test_markdown_chunks_trim() -> None:
     splitter = MarkdownSplitter()
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=4) == ["123", "123"]
 
 
-def test_markdown_hugging_face():
+def test_markdown_hugging_face() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = MarkdownSplitter.from_huggingface_tokenizer(tokenizer, trim_chunks=False)
     text = "123\n\n123"
     assert splitter.chunks(text, 1) == ["123\n", "\n123"]
 
 
-def test_markdown_hugging_face_range():
+def test_markdown_hugging_face_range() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = MarkdownSplitter.from_huggingface_tokenizer(tokenizer, trim_chunks=False)
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=(1, 2)) == ["123\n", "\n123"]
 
 
-def test_markdown_hugging_face_trim():
+def test_markdown_hugging_face_trim() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = MarkdownSplitter.from_huggingface_tokenizer(tokenizer)
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_markdown_hugging_face_from_str():
+def test_markdown_hugging_face_from_str() -> None:
     tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
     splitter = MarkdownSplitter.from_huggingface_tokenizer_str(tokenizer.to_str())
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_markdown_hugging_face_from_file():
+def test_markdown_hugging_face_from_file() -> None:
     splitter = MarkdownSplitter.from_huggingface_tokenizer_file(
         "tests/bert-base-cased.json"
     )
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_markdown_tiktoken():
+def test_markdown_tiktoken() -> None:
     splitter = MarkdownSplitter.from_tiktoken_model(
         model="gpt-3.5-turbo", trim_chunks=False
     )
     text = "123\n\n123"
     assert splitter.chunks(text, 2) == ["123\n", "\n123"]
 
 
-def test_markdown_tiktoken_range():
+def test_markdown_tiktoken_range() -> None:
     splitter = MarkdownSplitter.from_tiktoken_model(
         model="gpt-3.5-turbo", trim_chunks=False
     )
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=(2, 3)) == [
         "123\n",
         "\n123",
     ]
 
 
-def test_markdown_tiktoken_trim():
+def test_markdown_tiktoken_trim() -> None:
     splitter = MarkdownSplitter.from_tiktoken_model("gpt-3.5-turbo")
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=1) == ["123", "123"]
 
 
-def test_markdown_tiktoken_model_error():
+def test_markdown_tiktoken_model_error() -> None:
     with pytest.raises(Exception):
         MarkdownSplitter.from_tiktoken_model("random-model-name")
 
 
-def test_markdown_custom():
+def test_markdown_custom() -> None:
     splitter = MarkdownSplitter.from_callback(lambda x: len(x))
     text = "123\n\n123"
     assert splitter.chunks(text=text, chunk_capacity=3) == ["123", "123"]
+
+
+def test_char_indices() -> None:
+    splitter = TextSplitter()
+    text = "123\n123"
+    assert splitter.chunk_indices(text=text, chunk_capacity=4) == [
+        (0, "123"),
+        (4, "123"),
+    ]
+
+
+def test_char_indices_with_multibyte_character() -> None:
+    splitter = TextSplitter()
+    text = "12ü\n123"
+    assert len("12ü\n") == 4
+    assert splitter.chunk_indices(text=text, chunk_capacity=4) == [
+        (0, "12ü"),
+        (4, "123"),
+    ]
+
+
+def test_markdown_char_indices() -> None:
+    splitter = MarkdownSplitter()
+    text = "123\n456\n789"
+    assert splitter.chunk_indices(text=text, chunk_capacity=4) == [
+        (0, "123"),
+        (4, "456"),
+        (8, "789"),
+    ]
+
+
+def test_markdown_char_indices_with_multibyte_character() -> None:
+    splitter = MarkdownSplitter()
+    text = "12ü\n12ü\n12ü"
+    assert len("12ü\n") == 4
+    assert splitter.chunk_indices(text=text, chunk_capacity=4) == [
+        (0, "12ü"),
+        (4, "12ü"),
+        (8, "12ü"),
+    ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `semantic_text_splitter-0.9.0/Cargo.lock` & `semantic_text_splitter-0.9.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1182,16 +1182,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semantic-text-splitter"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
+ "auto_enums",
  "pyo3",
  "text-splitter",
  "tiktoken-rs",
  "tokenizers",
 ]
 
 [[package]]
@@ -1315,15 +1316,15 @@
 dependencies = [
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "text-splitter"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "ahash",
  "auto_enums",
  "divan",
  "either",
  "fake",
  "insta",
```

### Comparing `semantic_text_splitter-0.9.0/Cargo.toml` & `semantic_text_splitter-0.9.1/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [workspace]
 members = ["bindings/*"]
 
 [workspace.package]
-version = "0.9.0"
+version = "0.9.1"
 authors = ["Ben Brandt <benjamin.j.brandt@gmail.com>"]
 edition = "2021"
 description = "Split text into semantic chunks, up to a desired chunk size. Supports calculating length by characters and tokens, and is callable from Rust and Python."
 repository = "https://github.com/benbrandt/text-splitter"
 license = "MIT"
 keywords = ["text", "split", "tokenizer", "nlp", "ai"]
 categories = ["text-processing"]
```

### Comparing `semantic_text_splitter-0.9.0/pyproject.toml` & `semantic_text_splitter-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.9.0/PKG-INFO` & `semantic_text_splitter-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: semantic-text-splitter
-Version: 0.9.0
+Version: 0.9.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: black ; extra == 'test'
 Requires-Dist: tokenizers ; extra == 'test'
 Requires-Dist: pdoc ; extra == 'docs'
```

