# Comparing `tmp/japanese_address_parser_py-0.1.0b15.tar.gz` & `tmp/japanese_address_parser_py-0.1.0b17.tar.gz`

## Comparing `japanese_address_parser_py-0.1.0b15.tar` & `japanese_address_parser_py-0.1.0b17.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0     1001      127      749 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/Cargo.toml
--rw-r--r--   0     1001      127     1065 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/LICENSE
--rw-r--r--   0     1001      127     4410 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/api/city_master_api.rs
--rw-r--r--   0     1001      127     4915 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/api/prefecture_master_api.rs
--rw-r--r--   0     1001      127     2775 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/api.rs
--rw-r--r--   0     1001      127     1794 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/entity.rs
--rw-r--r--   0     1001      127     1326 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/err.rs
--rw-r--r--   0     1001      127       64 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/lib.rs
--rw-r--r--   0     1001      127     3131 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/orthographical_variant_adapter.rs
--rw-r--r--   0     1001      127     2794 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/vague_expression_adapter.rs
--rw-r--r--   0     1001      127       74 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/adapter.rs
--rw-r--r--   0     1001      127      570 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter/fullwidth_character.rs
--rw-r--r--   0     1001      127     7292 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter/invalid_town_name_format.rs
--rw-r--r--   0     1001      127     3393 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter/non_kanji_block_number.rs
--rw-r--r--   0     1001      127      162 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter.rs
--rw-r--r--   0     1001      127     3769 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_city.rs
--rw-r--r--   0     1001      127     2293 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_house_number.rs
--rw-r--r--   0     1001      127     1739 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_prefecture.rs
--rw-r--r--   0     1001      127     7124 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_town.rs
--rw-r--r--   0     1001      127     9275 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser.rs
--rw-r--r--   0     1001      127     3695 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/util/converter.rs
--rw-r--r--   0     1001      127     8133 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/util/sequence_matcher.rs
--rw-r--r--   0     1001      127       45 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/util.rs
--rw-r--r--   0     1001      127     2826 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/README.md
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/python/Cargo.toml
--rw-r--r--   0     1001      127     3282 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/python/README.md
--rw-r--r--   0     1001      127      823 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/python/japanese_address_parser_py.pyi
--rw-r--r--   0     1001      127     1426 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/python/src/lib.rs
--rw-r--r--   0     1001      127    35920 2024-04-21 12:02:46.000000 japanese_address_parser_py-0.1.0b15/Cargo.lock
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/Cargo.toml
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/pyproject.toml
--rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/PKG-INFO
+-rw-r--r--   0     1001      127      788 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/Cargo.toml
+-rw-r--r--   0     1001      127     1065 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/LICENSE
+-rw-r--r--   0     1001      127     4500 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/api/city_master_api.rs
+-rw-r--r--   0     1001      127     4988 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/api/prefecture_master_api.rs
+-rw-r--r--   0     1001      127     2094 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/api.rs
+-rw-r--r--   0     1001      127     1794 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/entity.rs
+-rw-r--r--   0     1001      127     1326 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/err.rs
+-rw-r--r--   0     1001      127      206 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/lib.rs
+-rw-r--r--   0     1001      127     3131 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/orthographical_variant_adapter.rs
+-rw-r--r--   0     1001      127     2794 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/vague_expression_adapter.rs
+-rw-r--r--   0     1001      127       74 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/adapter.rs
+-rw-r--r--   0     1001      127      570 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter/fullwidth_character.rs
+-rw-r--r--   0     1001      127     7292 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter/invalid_town_name_format.rs
+-rw-r--r--   0     1001      127     3393 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter/non_kanji_block_number.rs
+-rw-r--r--   0     1001      127      162 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/filter.rs
+-rw-r--r--   0     1001      127     3739 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_city.rs
+-rw-r--r--   0     1001      127     2293 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_house_number.rs
+-rw-r--r--   0     1001      127     1739 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_prefecture.rs
+-rw-r--r--   0     1001      127     7090 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser/read_town.rs
+-rw-r--r--   0     1001      127    10962 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/parser.rs
+-rw-r--r--   0     1001      127     3695 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/util/converter.rs
+-rw-r--r--   0     1001      127     8133 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/util/sequence_matcher.rs
+-rw-r--r--   0     1001      127       45 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/core/src/util.rs
+-rw-r--r--   0     1001      127     2794 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/README.md
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/python/Cargo.toml
+-rw-r--r--   0     1001      127     3302 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/python/README.md
+-rw-r--r--   0     1001      127     1265 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/python/japanese_address_parser_py.pyi
+-rw-r--r--   0     1001      127     1703 2024-04-28 17:41:03.000000 japanese_address_parser_py-0.1.0b17/python/src/lib.rs
+-rw-r--r--   0     1001      127    35921 2024-04-28 17:41:07.000000 japanese_address_parser_py-0.1.0b17/Cargo.lock
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/Cargo.toml
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/pyproject.toml
+-rw-r--r--   0        0        0     3833 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b17/PKG-INFO
```

### Comparing `japanese_address_parser_py-0.1.0b15/core/Cargo.toml` & `japanese_address_parser_py-0.1.0b17/core/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 description.workspace = true
 repository.workspace = true
 authors.workspace = true
 license.workspace = true
 readme = "../README.md"
 keywords.workspace = true
 categories.workspace = true
-rust-version = "1.64.0"
+rust-version = "1.73.0"
 
 [lib]
 crate-type = ["rlib", "cdylib"]
 
+[features]
+default = []
+blocking = []
+
 [dependencies]
 itertools = "0.12.0"
 js-sys = "0.3.67"
 nom = "7.1.3"
 rapidfuzz = "0.5.0"
 regex = "1.10.2"
 reqwest = { version = "0.12.3", default-features = false, features = ["json", "rustls-tls", "blocking"] }
```

### Comparing `japanese_address_parser_py-0.1.0b15/core/LICENSE` & `japanese_address_parser_py-0.1.0b17/core/LICENSE`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/api/city_master_api.rs` & `japanese_address_parser_py-0.1.0b17/core/src/api/city_master_api.rs`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 }),
                 Err(_) => Err(Error::new_api_error(ApiErrorKind::Deserialize(endpoint))),
             }
         } else {
             Err(Error::new_api_error(ApiErrorKind::Fetch(endpoint)))
         }
     }
-    #[cfg(not(target_arch = "wasm32"))]
+    #[cfg(feature = "blocking")]
     pub fn get_blocking(&self, prefecture_name: &str, city_name: &str) -> Result<City, Error> {
         let endpoint = format!("{}/{}/{}.json", self.server_url, prefecture_name, city_name);
         let response = match reqwest::blocking::get(&endpoint) {
             Ok(result) => result,
             Err(_) => return Err(Error::new_api_error(ApiErrorKind::Fetch(endpoint))),
         };
         if response.status() == 200 {
@@ -41,15 +41,15 @@
             }
         } else {
             Err(Error::new_api_error(ApiErrorKind::Fetch(endpoint)))
         }
     }
 }
 
-#[cfg(test)]
+#[cfg(all(test, not(feature = "blocking")))]
 mod tests {
     use crate::api::city_master_api::CityMasterApi;
     use crate::entity::Town;
 
     #[tokio::test]
     async fn 非同期_石川県羽咋郡志賀町_成功() {
         let city_master_api = CityMasterApi {
@@ -63,15 +63,36 @@
             koaza: "千古".to_string(),
             lat: Some(37.006235),
             lng: Some(136.779155),
         };
         assert!(city.towns.contains(&town));
     }
 
-    #[cfg(not(target_arch = "wasm32"))]
+    #[tokio::test]
+    async fn 非同期_誤った市区町村名_失敗() {
+        let city_master_api = CityMasterApi {
+            server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
+        };
+        let result = city_master_api.get("石川県", "敦賀市").await;
+        assert!(result.is_err());
+        assert_eq!(
+            result.err().unwrap().error_message,
+            format!(
+                "{}/石川県/敦賀市.jsonを取得できませんでした",
+                city_master_api.server_url
+            )
+        );
+    }
+}
+
+#[cfg(all(test, feature = "blocking"))]
+mod blocking_tests {
+    use crate::api::city_master_api::CityMasterApi;
+    use crate::entity::Town;
+
     #[test]
     fn 同期_石川県羽咋郡志賀町_成功() {
         let city_master_api = CityMasterApi {
             server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
         };
         let result = city_master_api.get_blocking("石川県", "羽咋郡志賀町");
         let city = result.unwrap();
@@ -81,31 +102,14 @@
             koaza: "千古".to_string(),
             lat: Some(37.006235),
             lng: Some(136.779155),
         };
         assert!(city.towns.contains(&town));
     }
 
-    #[tokio::test]
-    async fn 非同期_誤った市区町村名_失敗() {
-        let city_master_api = CityMasterApi {
-            server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
-        };
-        let result = city_master_api.get("石川県", "敦賀市").await;
-        assert!(result.is_err());
-        assert_eq!(
-            result.err().unwrap().error_message,
-            format!(
-                "{}/石川県/敦賀市.jsonを取得できませんでした",
-                city_master_api.server_url
-            )
-        );
-    }
-
-    #[cfg(not(target_arch = "wasm32"))]
     #[test]
     fn 同期_誤った市区町村名_失敗() {
         let city_master_api = CityMasterApi {
             server_url: "https://geolonia.github.io/japanese-addresses/api/ja",
         };
         let result = city_master_api.get_blocking("石川県", "敦賀市");
         assert!(result.is_err());
```

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/api/prefecture_master_api.rs` & `japanese_address_parser_py-0.1.0b17/core/src/api/prefecture_master_api.rs`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 Ok(result) => Ok(result),
                 Err(_) => Err(Error::new_api_error(ApiErrorKind::Deserialize(endpoint))),
             }
         } else {
             Err(Error::new_api_error(ApiErrorKind::Fetch(endpoint)))
         }
     }
-    #[cfg(not(target_arch = "wasm32"))]
+    #[cfg(feature = "blocking")]
     pub fn get_blocking(&self, prefecture_name: &str) -> Result<Prefecture, Error> {
         let endpoint = format!("{}/{}/master.json", self.server_url, prefecture_name);
         let response = match reqwest::blocking::get(&endpoint) {
             Ok(result) => result,
             Err(_) => return Err(Error::new_api_error(ApiErrorKind::Fetch(endpoint))),
         };
         if response.status() == 200 {
@@ -35,15 +35,15 @@
             }
         } else {
             Err(Error::new_api_error(ApiErrorKind::Fetch(endpoint)))
         }
     }
 }
 
-#[cfg(test)]
+#[cfg(all(test, not(feature = "blocking")))]
 mod tests {
     use crate::api::prefecture_master_api::PrefectureMasterApi;
 
     #[tokio::test]
     async fn 非同期_富山県_成功() {
         let prefecture_master_api = PrefectureMasterApi {
             server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
@@ -69,15 +69,35 @@
             "下新川郡朝日町",
         ];
         for city in cities {
             assert!(prefecture.cities.contains(&city.to_string()));
         }
     }
 
-    #[cfg(not(target_arch = "wasm32"))]
+    #[tokio::test]
+    async fn 非同期_誤った都道府県名_失敗() {
+        let prefecture_master_api = PrefectureMasterApi {
+            server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
+        };
+        let result = prefecture_master_api.get("大阪都").await;
+        assert!(result.is_err());
+        assert_eq!(
+            result.err().unwrap().error_message,
+            format!(
+                "{}/大阪都/master.jsonを取得できませんでした",
+                prefecture_master_api.server_url
+            )
+        );
+    }
+}
+
+#[cfg(all(test, feature = "blocking"))]
+mod blocking_tests {
+    use crate::api::prefecture_master_api::PrefectureMasterApi;
+
     #[test]
     fn 同期_富山県_成功() {
         let prefecture_master_api = PrefectureMasterApi {
             server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
         };
         let result = prefecture_master_api.get_blocking("富山県");
         let prefecture = result.unwrap();
@@ -100,31 +120,14 @@
             "下新川郡朝日町",
         ];
         for city in cities {
             assert!(prefecture.cities.contains(&city.to_string()));
         }
     }
 
-    #[tokio::test]
-    async fn 非同期_誤った都道府県名_失敗() {
-        let prefecture_master_api = PrefectureMasterApi {
-            server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
-        };
-        let result = prefecture_master_api.get("大阪都").await;
-        assert!(result.is_err());
-        assert_eq!(
-            result.err().unwrap().error_message,
-            format!(
-                "{}/大阪都/master.jsonを取得できませんでした",
-                prefecture_master_api.server_url
-            )
-        );
-    }
-
-    #[cfg(not(target_arch = "wasm32"))]
     #[test]
     fn 同期_誤った都道府県名_失敗() {
         let prefecture_master_api = PrefectureMasterApi {
             server_url: "https://yuukitoriyama.github.io/geolonia-japanese-addresses-accompanist",
         };
         let result = prefecture_master_api.get_blocking("大阪都");
         assert!(result.is_err());
```

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/entity.rs` & `japanese_address_parser_py-0.1.0b17/core/src/entity.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/err.rs` & `japanese_address_parser_py-0.1.0b17/core/src/err.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/orthographical_variant_adapter.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/orthographical_variant_adapter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/vague_expression_adapter.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/adapter/vague_expression_adapter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/filter/fullwidth_character.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/filter/fullwidth_character.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/filter/invalid_town_name_format.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/filter/invalid_town_name_format.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/filter/non_kanji_block_number.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/filter/non_kanji_block_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/read_city.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/read_city.rs`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     if let Some(result) = vague_expression_adapter.apply(input, &prefecture.cities) {
         return Some(result);
     }
 
     None
 }
 
-#[cfg(all(test, not(target_arch = "wasm32")))]
+#[cfg(all(test, feature = "blocking"))]
 mod tests {
-    use crate::api::{BlockingApi, BlockingApiImpl};
+    use crate::api::BlockingApi;
     use crate::parser::read_city::read_city;
     use test_case::test_case;
 
     #[test_case("京都府", "京都市山科区椥辻池尻町14-2", "京都市山科区"; "success_京都市山科区")]
     #[test_case("神奈川県", "茅ヶ崎市香川5丁目1", "茅ヶ崎市"; "success_茅ヶ崎市")]
     #[test_case("神奈川県", "茅ケ崎市香川5丁目1", "茅ヶ崎市"; "success_茅ケ崎市_表記ゆれ")]
     #[test_case("神奈川県", "横浜市保土ケ谷区川辺町2番地9", "横浜市保土ケ谷区"; "success_横浜市保土ケ谷区")]
@@ -58,13 +58,13 @@
     #[test_case("茨城県", "龍ヶ崎市佐貫町647", "龍ヶ崎市"; "success_龍ヶ崎市")]
     #[test_case("茨城県", "龍ケ崎市佐貫町647", "龍ヶ崎市"; "success_龍ケ崎市_表記ゆれ")]
     #[test_case("茨城県", "竜ヶ崎市佐貫町647", "龍ヶ崎市"; "success_竜ヶ崎市_表記ゆれ")]
     #[test_case("茨城県", "竜ケ崎市佐貫町647", "龍ヶ崎市"; "success_竜ケ崎市_表記ゆれ")]
     #[test_case("群馬県", "みなかみ町後閑318", "利根郡みなかみ町"; "success_利根郡みなかみ町_郡名が省略されている")]
     #[test_case("埼玉県", "東秩父村大字御堂634番地", "秩父郡東秩父村"; "success_秩父郡東秩父村_郡名が省略されている")]
     fn test_read_city(prefecture_name: &str, input: &str, expected: &str) {
-        let api = BlockingApiImpl::new();
+        let api = BlockingApi::new();
         let prefecture = api.get_prefecture_master(prefecture_name).unwrap();
         let (_, city_name) = read_city(input, prefecture).unwrap();
         assert_eq!(city_name, expected);
     }
 }
```

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/read_house_number.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/read_house_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/read_prefecture.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/read_prefecture.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser/read_town.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser/read_town.rs`

 * *Files 5% similar despite different names*

```diff
@@ -52,17 +52,17 @@
         if let Some(result) = adapter.apply(input, &town.name) {
             return Some(result);
         };
     }
     None
 }
 
-#[cfg(all(test, not(target_arch = "wasm32")))]
+#[cfg(all(test, feature = "blocking"))]
 mod tests {
-    use crate::api::{BlockingApi, BlockingApiImpl};
+    use crate::api::BlockingApi;
     use crate::entity::{City, Town};
     use crate::parser::read_town::read_town;
 
     #[test]
     fn read_town_成功_静岡市清水区旭町() {
         let city = City {
             name: "静岡市清水区".to_string(),
@@ -149,15 +149,15 @@
         assert_eq!(town, "薮田南二丁目");
         let (_, town) = read_town("籔田南二丁目", &city).unwrap();
         assert_eq!(town, "薮田南二丁目");
     }
 
     #[test]
     fn read_town_丁目が算用数字の場合_京都府京都市東山区n丁目() {
-        let client = BlockingApiImpl::new();
+        let client = BlockingApi::new();
         let city = client.get_city_master("京都府", "京都市東山区").unwrap();
         let test_cases = vec![
             ("本町1丁目45番", "本町一丁目"),
             ("本町2丁目64番", "本町二丁目"),
             ("本町10丁目169番", "本町十丁目"),
             ("本町12丁目224番", "本町十二丁目"),
             ("本町20丁目435番", "本町二十丁目"),
@@ -167,15 +167,15 @@
             let (_, town) = read_town(input, &city).unwrap();
             assert_eq!(town, town_name);
         }
     }
 
     #[test]
     fn read_town_大字の省略_東京都西多摩郡日の出町大字平井() {
-        let blocking_api = BlockingApiImpl::new();
+        let blocking_api = BlockingApi::new();
         let city = blocking_api
             .get_city_master("東京都", "西多摩郡日の出町")
             .unwrap();
 
         let (rest, town) = read_town("大字平井2780番地", &city).unwrap();
         assert_eq!(town, "大字平井");
         assert_eq!(rest, "2780番地");
```

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/parser.rs` & `japanese_address_parser_py-0.1.0b17/core/src/parser.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,77 @@
-use crate::api::Api;
-#[cfg(not(target_arch = "wasm32"))]
+use std::sync::Arc;
+
+use crate::api::AsyncApi;
+#[cfg(feature = "blocking")]
 use crate::api::BlockingApi;
 use crate::entity::{Address, ParseResult};
 use crate::err::{Error, ParseErrorKind};
 use crate::parser::read_city::read_city;
 use crate::parser::read_prefecture::read_prefecture;
 use crate::parser::read_town::read_town;
 
 mod adapter;
 mod filter;
 mod read_city;
 mod read_house_number;
 mod read_prefecture;
 mod read_town;
 
-pub async fn parse<T: Api>(api: T, input: &str) -> ParseResult {
+/// An asynchronous `Parser` to process addresses.
+///
+/// # Example
+/// ```
+/// use japanese_address_parser::parser::Parser;
+///
+/// async fn example() {
+///     let parser = Parser::new();
+///     let result = parser.parse("東京都新宿区西新宿2-8-1").await;
+///     println!("{:?}", result);
+/// }
+/// ```
+pub struct Parser {
+    async_api: Arc<AsyncApi>,
+    #[cfg(feature = "blocking")]
+    blocking_api: Arc<BlockingApi>,
+}
+
+impl Parser {
+    /// Constructs a new `Parser`.
+    #[cfg(feature = "blocking")]
+    pub fn new() -> Self {
+        Parser {
+            async_api: Arc::new(AsyncApi::new()),
+            blocking_api: Arc::new(BlockingApi::new()),
+        }
+    }
+
+    /// Constructs a new `Parser`.
+    #[cfg(not(feature = "blocking"))]
+    pub fn new() -> Self {
+        Parser {
+            async_api: Arc::new(AsyncApi::new()),
+        }
+    }
+
+    /// Parses the given `address` asynchronously.
+    pub async fn parse(&self, address: &str) -> ParseResult {
+        parse(self.async_api.clone(), address).await
+    }
+
+    /// Parses the given `address` synchronously.
+    #[cfg(feature = "blocking")]
+    pub fn parse_blocking(&self, address: &str) -> ParseResult {
+        parse_blocking(self.blocking_api.clone(), address)
+    }
+}
+
+/// A function to parse the given address asynchronously.
+///
+/// publicにしていますが、直接の使用は推奨されません。[Parser]の利用を検討してください。
+pub async fn parse(api: Arc<AsyncApi>, input: &str) -> ParseResult {
     // 都道府県を特定
     let (rest, prefecture_name) = if let Some(result) = read_prefecture(input) {
         result
     } else {
         return ParseResult {
             address: Address::new("", "", "", input),
             error: Some(Error::new_parse_error(ParseErrorKind::Prefecture)),
@@ -65,87 +118,87 @@
 
     ParseResult {
         address: Address::new(prefecture_name, &city_name, &town_name, &rest),
         error: None,
     }
 }
 
-#[cfg(test)]
-mod non_blocking_tests {
+#[cfg(all(test, not(feature = "blocking")))]
+mod tests {
     use crate::api::city_master_api::CityMasterApi;
     use crate::api::prefecture_master_api::PrefectureMasterApi;
-    use crate::api::{Api, ApiImpl};
+    use crate::api::AsyncApi;
     use crate::err::ParseErrorKind;
     use crate::parser::parse;
     use wasm_bindgen_test::{wasm_bindgen_test, wasm_bindgen_test_configure};
 
     #[tokio::test]
     async fn 都道府県名が誤っている場合() {
-        let api = ApiImpl::new();
-        let result = parse(api, "青盛県青森市長島１丁目１−１").await;
+        let api = AsyncApi::new();
+        let result = parse(api.into(), "青盛県青森市長島１丁目１−１").await;
         assert_eq!(result.address.prefecture, "");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "青盛県青森市長島１丁目１−１");
         assert_eq!(result.error.is_some(), true);
         assert_eq!(
             result.error.unwrap().error_message,
             ParseErrorKind::Prefecture.to_string()
         );
     }
 
     #[tokio::test]
     async fn 都道府県マスタが取得できない場合() {
-        let mut api = ApiImpl::new();
+        let mut api = AsyncApi::new();
         api.prefecture_master_api = PrefectureMasterApi {
             server_url: "https://example.com/invalid_url/api/",
         };
 
-        let result = parse(api, "青森県青森市長島１丁目１−１").await;
+        let result = parse(api.into(), "青森県青森市長島１丁目１−１").await;
         assert_eq!(result.error.is_some(), true);
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "青森市長島１丁目１−１");
     }
 
     #[tokio::test]
     async fn 市区町村名が誤っている場合() {
-        let api = ApiImpl::new();
-        let result = parse(api, "青森県青盛市長島１丁目１−１").await;
+        let api = AsyncApi::new();
+        let result = parse(api.into(), "青森県青盛市長島１丁目１−１").await;
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "青盛市長島１丁目１−１");
         assert_eq!(result.error.is_some(), true);
         assert_eq!(
             result.error.unwrap().error_message,
             ParseErrorKind::City.to_string()
         );
     }
 
     #[tokio::test]
     async fn 市区町村マスタが取得できない場合() {
-        let mut api = ApiImpl::new();
+        let mut api = AsyncApi::new();
         api.city_master_api = CityMasterApi {
             server_url: "https://example.com/invalid_url/api/",
         };
 
-        let result = parse(api, "青森県青森市長島１丁目１−１").await;
+        let result = parse(api.into(), "青森県青森市長島１丁目１−１").await;
         assert_eq!(result.error.is_some(), true);
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "青森市");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "長島１丁目１−１");
     }
 
     #[tokio::test]
     async fn 町名が誤っている場合() {
-        let api = ApiImpl::new();
-        let result = parse(api, "青森県青森市永嶋１丁目１−１").await;
+        let api = AsyncApi::new();
+        let result = parse(api.into(), "青森県青森市永嶋１丁目１−１").await;
         assert_eq!(result.address.prefecture, "青森県");
         assert_eq!(result.address.city, "青森市");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "永嶋１丁目１−１");
         assert_eq!(result.error.is_some(), true);
         assert_eq!(
             result.error.unwrap().error_message,
@@ -153,26 +206,29 @@
         );
     }
 
     wasm_bindgen_test_configure!(run_in_browser);
 
     #[wasm_bindgen_test]
     async fn parse_wasm_success() {
-        let api = ApiImpl::new();
-        let result = parse(api, "兵庫県淡路市生穂新島8番地").await;
+        let api = AsyncApi::new();
+        let result = parse(api.into(), "兵庫県淡路市生穂新島8番地").await;
         assert_eq!(result.address.prefecture, "兵庫県".to_string());
         assert_eq!(result.address.city, "淡路市".to_string());
         assert_eq!(result.address.town, "生穂".to_string());
         assert_eq!(result.address.rest, "新島8番地".to_string());
         assert_eq!(result.error, None);
     }
 }
 
-#[cfg(not(target_arch = "wasm32"))]
-pub fn parse_blocking<T: BlockingApi>(api: T, input: &str) -> ParseResult {
+/// A function to parse the given address synchronously.
+///
+/// publicにしていますが、直接の使用は推奨されません。[Parser]の利用を検討してください。
+#[cfg(feature = "blocking")]
+pub fn parse_blocking(api: Arc<BlockingApi>, input: &str) -> ParseResult {
     let (rest, prefecture_name) = match read_prefecture(input) {
         None => {
             return ParseResult {
                 address: Address::new("", "", "", input),
                 error: Some(Error::new_parse_error(ParseErrorKind::Prefecture)),
             };
         }
@@ -217,35 +273,35 @@
 
     ParseResult {
         address: Address::new(prefecture_name, &city_name, &town_name, &rest),
         error: None,
     }
 }
 
-#[cfg(all(test, not(target_arch = "wasm32")))]
+#[cfg(all(test, feature = "blocking"))]
 mod blocking_tests {
-    use crate::api::{BlockingApi, BlockingApiImpl};
+    use crate::api::BlockingApi;
     use crate::err::ParseErrorKind;
     use crate::parser::parse_blocking;
 
     #[test]
     fn parse_blocking_success_埼玉県秩父市熊木町8番15号() {
-        let client = BlockingApiImpl::new();
-        let result = parse_blocking(client, "埼玉県秩父市熊木町8番15号");
+        let client = BlockingApi::new();
+        let result = parse_blocking(client.into(), "埼玉県秩父市熊木町8番15号");
         assert_eq!(result.address.prefecture, "埼玉県");
         assert_eq!(result.address.city, "秩父市");
         assert_eq!(result.address.town, "熊木町");
         assert_eq!(result.address.rest, "8番15号");
         assert_eq!(result.error, None);
     }
 
     #[test]
     fn parse_blocking_fail_市町村名が間違っている場合() {
-        let client = BlockingApiImpl::new();
-        let result = parse_blocking(client, "埼玉県秩父柿熊木町8番15号");
+        let client = BlockingApi::new();
+        let result = parse_blocking(client.into(), "埼玉県秩父柿熊木町8番15号");
         assert_eq!(result.address.prefecture, "埼玉県");
         assert_eq!(result.address.city, "");
         assert_eq!(result.address.town, "");
         assert_eq!(result.address.rest, "秩父柿熊木町8番15号");
         assert_eq!(
             result.error.unwrap().error_message,
             ParseErrorKind::City.to_string()
```

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/util/converter.rs` & `japanese_address_parser_py-0.1.0b17/core/src/util/converter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/core/src/util/sequence_matcher.rs` & `japanese_address_parser_py-0.1.0b17/core/src/util/sequence_matcher.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b15/README.md` & `japanese_address_parser_py-0.1.0b17/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # japanese-address-parser
 
 [![Docs](https://docs.rs/japanese-address-parser/badge.svg)](https://docs.rs/japanese-address-parser)
 [![Crates.io (latest)](https://img.shields.io/crates/v/japanese-address-parser)](https://crates.io/crates/japanese-address-parser)
-![Rust Version](https://img.shields.io/badge/rust%20version-%3E%3D1.64.0-orange)
+![Rust Version](https://img.shields.io/badge/rust%20version-%3E%3D1.73.0-orange)
 [![Unit test & Code check](https://github.com/YuukiToriyama/japanese-address-parser/actions/workflows/code-check.yaml/badge.svg)](https://github.com/YuukiToriyama/japanese-address-parser/actions/workflows/code-check.yaml)
 
 A Rust Library to parse japanese addresses.
 
 ## Usage
 
 Add this to your `Cargo.toml`
 
 ```bash
 cargo add japanese-address-parser
+# or
+cargo add japanese-address-parser -F blocking
 ```
 
-### Async Api
+### Async Version
 
 ```rust
-use japanese_address_parser::api::{Api, ApiImpl};
-use japanese_address_parser::parser::parse;
+use japanese_address_parser::parser::Parser;
 
 #[tokio::main]
 async fn main() {
-    let async_api = ApiImpl::new();
-    let parse_result = parse(async_api, "東京都千代田区丸の内1-1-1").await;
+    let parser = Parser::new();
+    let parse_result = parser.parse("東京都千代田区丸の内1-1-1").await;
     println!("{:?}", parse_result);
 }
 ```
 
-### Blocking Api
+### Blocking Version
 
 ```rust
-use japanese_address_parser::api::{BlockingApi, BlockingApiImpl};
-use japanese_address_parser::parser::parse_blocking;
+use japanese_address_parser::parser::Parser;
 
 fn main() {
-    let blocking_api = BlockingApiImpl::new();
-    let parse_result = parse_blocking(blocking_api, "東京都千代田区丸の内1-1-1");
+    let parser = Parser::new();
+    let parse_result = parser.parse_blocking("東京都千代田区丸の内1-1-1"); // `parse_blocking()` is available on `blocking` feature only
     println!("{:?}", parse_result);
 }
 ```
 
 ## Wasm support
 
 [![npmjs](https://img.shields.io/npm/v/%40toriyama/japanese-address-parser)](https://www.npmjs.com/package/@toriyama/japanese-address-parser)
```

### Comparing `japanese_address_parser_py-0.1.0b15/python/README.md` & `japanese_address_parser_py-0.1.0b17/python/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,40 +13,42 @@
 ```bash
 pip install japanese-address-parser-py
 ```
 
 ## Usage
 
 ```python
-import japanese_address_parser_py
+from japanese_address_parser_py import Parser
 
 address_list = [
     "埼玉県さいたま市浦和区高砂3-15-1",
     "千葉県千葉市中央区市場町1-1",
     "東京都新宿区西新宿2-8-1",
     "神奈川県横浜市中区日本大通1"
 ]
+parser = Parser()
 for address in address_list:
-    parse_result = japanese_address_parser_py.parse(address)
+    parse_result = parser.parse(address)
     print(parse_result.address)
 ```
 
 ```text
 {'prefecture': '埼玉県', 'town': '高砂三丁目', 'rest': '15-1', 'city': 'さいたま市浦和区'}
 {'rest': '1-1', 'town': '市場町', 'prefecture': '千葉県', 'city': '千葉市中央区'}
 {'prefecture': '東京都', 'rest': '8-1', 'town': '西新宿二丁目', 'city': '新宿区'}
 {'town': '日本大通', 'city': '横浜市中区', 'prefecture': '神奈川県', 'rest': '1'}
 ```
 
 
 ```python
-import japanese_address_parser_py
+from japanese_address_parser_py import Parser
 
+parser = Parser()
 address = "神奈川県横浜市中区本町6丁目50-10"
-parse_result = japanese_address_parser_py.parse(address)
+parse_result = parser.parse(address)
 print(parse_result.address["prefecture"])
 print(parse_result.address["city"])
 print(parse_result.address["town"])
 print(parse_result.address["rest"])
 ```
 
 ```text
```

### Comparing `japanese_address_parser_py-0.1.0b15/python/japanese_address_parser_py.pyi` & `japanese_address_parser_py-0.1.0b17/python/japanese_address_parser_py.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -25,7 +25,28 @@
     Format informal address into formal style
 
     入力された住所を正式な表記に整形します。
 
     :param address: 住所
     :return: ParseResult
     """
+
+
+class Parser:
+    def __new__(cls) -> Parser:
+        """
+        Construct a parser.
+    
+        パーサーを生成します。
+
+        :return: JapaneseAddressParser
+        """
+
+    def parse(cls, address: str) -> ParseResult:
+        """
+        Format informal address into formal style
+
+        入力された住所を正式な表記に整形します。
+
+        :param address: 住所
+        :return: ParseResult
+        """
```

### Comparing `japanese_address_parser_py-0.1.0b15/python/src/lib.rs` & `japanese_address_parser_py-0.1.0b17/python/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-use japanese_address_parser::api::{BlockingApi, BlockingApiImpl};
-use japanese_address_parser::entity::ParseResult;
-use japanese_address_parser::parser::parse_blocking;
-use pyo3::prelude::*;
 use std::collections::HashMap;
 
+use pyo3::prelude::*;
+
+use japanese_address_parser::entity::ParseResult;
+use japanese_address_parser::parser::Parser;
+
 #[pyclass(name = "ParseResult")]
 struct PyParseResult {
     #[pyo3(get)]
     address: HashMap<String, String>,
     #[pyo3(get)]
     error: HashMap<String, String>,
 }
@@ -24,20 +25,40 @@
             error.insert(String::from("error_type"), err.error_type);
             error.insert(String::from("error_message"), err.error_message);
         }
         Self { address, error }
     }
 }
 
+#[pyclass(name = "Parser")]
+struct PyParser {
+    parser: Parser,
+}
+
+#[pymethods]
+impl PyParser {
+    #[new]
+    fn default() -> Self {
+        PyParser {
+            parser: Parser::new(),
+        }
+    }
+
+    fn parse(&self, address: &str) -> PyParseResult {
+        self.parser.parse_blocking(address).into()
+    }
+}
+
 #[pyfunction]
 fn parse(address: &str) -> PyParseResult {
-    let api = BlockingApiImpl::new();
-    parse_blocking(api, address).into()
+    let parser = Parser::new();
+    parser.parse_blocking(address).into()
 }
 
 #[pymodule]
 #[pyo3(name = "japanese_address_parser_py")]
 fn python_module(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyParseResult>()?;
+    m.add_class::<PyParser>()?;
     m.add_function(wrap_pyfunction!(parse, m)?)?;
     Ok(())
 }
```

### Comparing `japanese_address_parser_py-0.1.0b15/Cargo.lock` & `japanese_address_parser_py-0.1.0b17/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
@@ -345,15 +345,15 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "japanese-address-parser"
-version = "0.1.0-beta.15"
+version = "0.1.0-beta.17"
 dependencies = [
  "itertools",
  "js-sys",
  "nom",
  "rapidfuzz",
  "regex",
  "reqwest",
@@ -376,17 +376,17 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -474,33 +474,33 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -613,15 +613,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python"
-version = "0.1.0-beta.15"
+version = "0.1.0-beta.17"
 dependencies = [
  "japanese-address-parser",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -636,17 +636,17 @@
 name = "rapidfuzz"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "270e04e5ea61d40841942bb15e451c29ee1618637bcf97fc7ede5dd4a9b1601b"
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
@@ -761,23 +761,23 @@
 dependencies = [
  "base64",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
@@ -796,17 +796,17 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.6.5"
@@ -816,17 +816,17 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -943,15 +943,15 @@
  "quote",
  "syn",
  "test-case-core",
 ]
 
 [[package]]
 name = "tests"
-version = "0.1.0-beta.15"
+version = "0.1.0-beta.17"
 dependencies = [
  "csv",
  "japanese-address-parser",
  "serde",
  "tokio",
 ]
 
@@ -1120,15 +1120,15 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm"
-version = "0.1.0-beta.15"
+version = "0.1.0-beta.17"
 dependencies = [
  "console_error_panic_hook",
  "japanese-address-parser",
  "serde-wasm-bindgen",
  "wasm-bindgen",
  "wasm-bindgen-futures",
 ]
```

### Comparing `japanese_address_parser_py-0.1.0b15/PKG-INFO` & `japanese_address_parser_py-0.1.0b17/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: japanese-address-parser-py
-Version: 0.1.0b15
+Version: 0.1.0b17
 Classifier: Topic :: Text Processing
 Classifier: Programming Language :: Rust
 Classifier: Typing :: Typed
 Summary: A Rust Library to parse japanese addresses.
 Keywords: converter,utility,geo,rust
 Author: Yuuki Toriyama <github@toriyama.dev>
 Author-email: Yuuki Toriyama <github@toriyama.dev>
@@ -27,40 +27,42 @@
 ```bash
 pip install japanese-address-parser-py
 ```
 
 ## Usage
 
 ```python
-import japanese_address_parser_py
+from japanese_address_parser_py import Parser
 
 address_list = [
     "埼玉県さいたま市浦和区高砂3-15-1",
     "千葉県千葉市中央区市場町1-1",
     "東京都新宿区西新宿2-8-1",
     "神奈川県横浜市中区日本大通1"
 ]
+parser = Parser()
 for address in address_list:
-    parse_result = japanese_address_parser_py.parse(address)
+    parse_result = parser.parse(address)
     print(parse_result.address)
 ```
 
 ```text
 {'prefecture': '埼玉県', 'town': '高砂三丁目', 'rest': '15-1', 'city': 'さいたま市浦和区'}
 {'rest': '1-1', 'town': '市場町', 'prefecture': '千葉県', 'city': '千葉市中央区'}
 {'prefecture': '東京都', 'rest': '8-1', 'town': '西新宿二丁目', 'city': '新宿区'}
 {'town': '日本大通', 'city': '横浜市中区', 'prefecture': '神奈川県', 'rest': '1'}
 ```
 
 
 ```python
-import japanese_address_parser_py
+from japanese_address_parser_py import Parser
 
+parser = Parser()
 address = "神奈川県横浜市中区本町6丁目50-10"
-parse_result = japanese_address_parser_py.parse(address)
+parse_result = parser.parse(address)
 print(parse_result.address["prefecture"])
 print(parse_result.address["city"])
 print(parse_result.address["town"])
 print(parse_result.address["rest"])
 ```
 
 ```text
```

