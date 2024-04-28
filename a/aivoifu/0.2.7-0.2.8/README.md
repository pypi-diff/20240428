# Comparing `tmp/aivoifu-0.2.7.tar.gz` & `tmp/aivoifu-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aivoifu-0.2.7.tar", max compression
+gzip compressed data, was "aivoifu-0.2.8.tar", max compression
```

## Comparing `aivoifu-0.2.7.tar` & `aivoifu-0.2.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2024-01-26 18:27:42.698418 aivoifu-0.2.7/AIvoifu/__init__.py
--rw-r--r--   0        0        0     1916 2024-03-22 22:49:09.929505 aivoifu-0.2.7/AIvoifu/client_pipeline.py
--rw-r--r--   0        0        0    12280 2024-03-23 00:46:51.845273 aivoifu-0.2.7/AIvoifu/tts/tts.py
--rw-r--r--   0        0        0        0 2024-01-26 18:27:42.699600 aivoifu-0.2.7/AIvoifu/tts/tts_base_models/__init__.py
--rw-r--r--   0        0        0     9737 2024-03-05 13:37:25.545859 aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/config.json
--rw-r--r--   0        0        0     3549 2024-03-05 13:37:25.524334 aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/config_se.json
--rw-r--r--   0        0        0       94 2024-03-05 13:37:25.542571 aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/language_ids.json
--rw-r--r--   0        0        0    10238 2024-03-05 13:37:25.524483 aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/nconfig.json
--rw-r--r--   0        0        0     1631 2024-03-05 13:37:26.884541 aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/speech.py
--rw-r--r--   0        0        0      209 2024-03-05 13:37:25.553382 aivoifu-0.2.7/AIvoifu/tts/tts_base_models/readme.md
--rw-r--r--   0        0        0      163 2024-03-05 13:37:25.545743 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/README.md
--rw-r--r--   0        0        0        0 2024-01-26 18:27:42.702144 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/__init__.py
--rw-r--r--   0        0        0     2674 2024-03-05 13:37:26.879074 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/config.py
--rw-r--r--   0        0        0    14454 2024-01-26 18:27:42.703047 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/attentions.py
--rw-r--r--   0        0        0     5151 2024-01-26 18:27:42.703474 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/commons.py
--rw-r--r--   0        0        0    33494 2024-03-05 13:37:27.456616 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/models.py
--rw-r--r--   0        0        0    28506 2024-03-05 13:37:27.400663 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/models_onnx.py
--rw-r--r--   0        0        0    16651 2024-03-18 11:05:25.959204 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/modules.py
--rw-r--r--   0        0        0     7253 2024-01-26 18:27:42.705499 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/transforms.py
--rw-r--r--   0        0        0   369004 2024-01-26 18:27:42.707744 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/poetry.lock
--rw-r--r--   0        0        0     1240 2024-01-26 18:27:42.708036 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/pyproject.toml
--rw-r--r--   0        0        0     5070 2024-03-20 03:15:46.427221 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/python_inference.py
--rw-r--r--   0        0        0      771 2024-01-26 18:27:42.708531 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/requirements.txt
--rw-r--r--   0        0        0    10966 2024-01-26 18:27:42.708898 aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/vc_infer_pipeline.py
--rw-r--r--   0        0        0      235 2024-03-05 13:37:25.532393 aivoifu-0.2.7/AIvoifu/voice_conversion/config.json
--rw-r--r--   0        0        0    11472 2024-03-18 11:05:25.847220 aivoifu-0.2.7/AIvoifu/voice_conversion/vc_inference.py
--rw-r--r--   0        0        0      553 2024-03-05 13:37:25.545906 aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/alice/meta.json
--rw-r--r--   0        0        0      568 2024-03-05 13:37:25.542480 aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/ayaka-jp/meta.json
--rw-r--r--   0        0        0      573 2024-03-05 13:37:25.543265 aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/kazuha-jp/meta.json
--rw-r--r--   0        0        0     1420 2024-03-05 13:37:25.542647 aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/readme.md
--rw-r--r--   0        0        0      569 2024-03-05 13:37:25.524265 aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/xiao-jp/meta.json
--rw-r--r--   0        0        0     1062 2024-01-24 20:17:40.512278 aivoifu-0.2.7/LICENSE
--rw-r--r--   0        0        0     2372 2024-03-05 14:04:45.976271 aivoifu-0.2.7/README.md
--rw-r--r--   0        0        0      761 2024-03-23 00:47:13.671845 aivoifu-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3469 1970-01-01 00:00:00.000000 aivoifu-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-26 18:27:42.698418 aivoifu-0.2.8/AIvoifu/__init__.py
+-rw-r--r--   0        0        0     2192 2024-04-28 05:25:32.210168 aivoifu-0.2.8/AIvoifu/client_pipeline.py
+-rw-r--r--   0        0        0    11138 2024-04-28 05:06:00.219313 aivoifu-0.2.8/AIvoifu/tts/tts.py
+-rw-r--r--   0        0        0        0 2024-01-26 18:27:42.699600 aivoifu-0.2.8/AIvoifu/tts/tts_base_models/__init__.py
+-rw-r--r--   0        0        0     9737 2024-03-05 13:37:25.545859 aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/config.json
+-rw-r--r--   0        0        0     3549 2024-03-05 13:37:25.524334 aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/config_se.json
+-rw-r--r--   0        0        0       94 2024-03-05 13:37:25.542571 aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/language_ids.json
+-rw-r--r--   0        0        0    10238 2024-03-05 13:37:25.524483 aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/nconfig.json
+-rw-r--r--   0        0        0     1631 2024-03-05 13:37:26.884541 aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/speech.py
+-rw-r--r--   0        0        0      209 2024-03-05 13:37:25.553382 aivoifu-0.2.8/AIvoifu/tts/tts_base_models/readme.md
+-rw-r--r--   0        0        0      163 2024-03-05 13:37:25.545743 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/README.md
+-rw-r--r--   0        0        0        0 2024-01-26 18:27:42.702144 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/__init__.py
+-rw-r--r--   0        0        0     2674 2024-03-05 13:37:26.879074 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/config.py
+-rw-r--r--   0        0        0    14454 2024-01-26 18:27:42.703047 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/attentions.py
+-rw-r--r--   0        0        0     5151 2024-01-26 18:27:42.703474 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/commons.py
+-rw-r--r--   0        0        0    33494 2024-03-05 13:37:27.456616 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/models.py
+-rw-r--r--   0        0        0    28506 2024-03-05 13:37:27.400663 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/models_onnx.py
+-rw-r--r--   0        0        0    16651 2024-03-18 11:05:25.959204 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/modules.py
+-rw-r--r--   0        0        0     7253 2024-01-26 18:27:42.705499 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/transforms.py
+-rw-r--r--   0        0        0   369004 2024-01-26 18:27:42.707744 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/poetry.lock
+-rw-r--r--   0        0        0     1240 2024-01-26 18:27:42.708036 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/pyproject.toml
+-rw-r--r--   0        0        0     5070 2024-04-28 05:07:46.117683 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/python_inference.py
+-rw-r--r--   0        0        0      771 2024-01-26 18:27:42.708531 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/requirements.txt
+-rw-r--r--   0        0        0    10966 2024-01-26 18:27:42.708898 aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/vc_infer_pipeline.py
+-rw-r--r--   0        0        0      235 2024-03-05 13:37:25.532393 aivoifu-0.2.8/AIvoifu/voice_conversion/config.json
+-rw-r--r--   0        0        0    11472 2024-04-28 05:25:34.342826 aivoifu-0.2.8/AIvoifu/voice_conversion/vc_inference.py
+-rw-r--r--   0        0        0      553 2024-03-05 13:37:25.545906 aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/alice/meta.json
+-rw-r--r--   0        0        0      568 2024-03-05 13:37:25.542480 aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/ayaka-jp/meta.json
+-rw-r--r--   0        0        0      573 2024-03-05 13:37:25.543265 aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/kazuha-jp/meta.json
+-rw-r--r--   0        0        0     1420 2024-03-05 13:37:25.542647 aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/readme.md
+-rw-r--r--   0        0        0      569 2024-03-05 13:37:25.524265 aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/xiao-jp/meta.json
+-rw-r--r--   0        0        0     1062 2024-01-24 20:17:40.512278 aivoifu-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2372 2024-03-05 14:04:45.976271 aivoifu-0.2.8/README.md
+-rw-r--r--   0        0        0      798 2024-04-28 05:28:21.434362 aivoifu-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 aivoifu-0.2.8/PKG-INFO
```

### Comparing `aivoifu-0.2.7/AIvoifu/client_pipeline.py` & `aivoifu-0.2.8/AIvoifu/client_pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,16 +24,20 @@
         self.model = tts.auto_tts(model_selection=tts_model_selection, **kwargs)
         if vc_model_selection and hubert_model:
             self.vc_model = vc.vc_inference(
                 selected_model_from_zoo=vc_model_selection,
                 hubert_model=hubert_model,
                 force_load_model=force_load_model,
             )
-        print("Loaded Waifu Vocal Pipeline")
+        if vc_model_selection and not hubert_model:
+            raise ValueError("Please Provide Hubert Model To Enable Voice Conversion")
+        elif not vc_model_selection and hubert_model:
+            raise ValueError("Please Provide VC Model To Enable Voice Conversion")
 
+        print("Loaded Waifu Vocal Pipeline")
     def tts(self, text, voice_conversion=True, save_path=None):
         # text to speech
         if not save_path:
             save_path = f"{self.cache_root}/dialog_cache.wav"
         self.model.tts(text, save_path)
         # voice conversion
         if voice_conversion and self.vc_model:
```

### Comparing `aivoifu-0.2.7/AIvoifu/tts/tts.py` & `aivoifu-0.2.8/AIvoifu/tts/tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,67 +256,28 @@
         # save to file using soundfile
         sf.write(out_path, audio_array, self.model.generation_config.sample_rate)
 
     def requested_additional_args(self, **kwargs) -> None:
         self.speaker = kwargs.get("speaker", None)
         return None
 
-
-class XTTS(BaseTTS):
-    """[Coqui TTS](
-    XTTS is a TTS model that run on Coqui TTS Api.\n
-    """
-
-    def __init__(self) -> None:
-        from TTS.api import TTS
-        import torch
-
-        os.environ["COQUI_TOS_AGREED"] = "1"  # agree to coqui TOS
-        self.model = TTS("xtts", gpu=torch.cuda.is_available())
-        self.model_name = "xtts"
-        self.speaker = None
-        self.sr = 24000
-
-    @staticmethod
-    def supported_languages(self) -> list:
-        return ["en"]
-
-    def tts(self, text, out_path, voice="Ana Florence", language="en"):
-        print("Perform XTTS TTS...")
-        print("text to audio...")
-        print(voice if self.speaker is None else self.speaker)
-        output = self.model.tts(
-            text=text,
-            speaker=self.speaker if self.speaker is not None else voice,
-            language=language,
-            split_sentences=True,
-        )
-        # write to file, 24kHz
-        sf.write(out_path, output, self.sr)
-
-    def requested_additional_args(self, **kwargs) -> None:
-        self.speaker = kwargs.get("speaker", None)
-        return None
-
-
 # add your tts model mapping 'key' here
 # possible_model = Literal['khanomtal11', 'key2', 'key3', ...]
-possible_model = Literal["gtts", "edge_tts", "bark", "xtts"]
+possible_model = Literal["gtts", "edge_tts", "bark",]
 
 
 class auto_tts:
     possible_model = possible_model  # allow auto_tts.possible_model access
 
     def __init__(self, model_selection: possible_model = None, **kwargs) -> None:
         self.model_mapping: Dict[possible_model, BaseTTS] = {
             # "khanomtal11": khanomtal11,
             "gtts": Gtts,
             "edge_tts": EdgeTTS,
             "bark": Bark,
-            "xtts": XTTS,
             # 'key' : your tts class
         }
 
         # manual model selection and validation if model existed
         if model_selection is None:
             print("---- Available TTS models: ---")
             for key in self.list_all_models():
```

### Comparing `aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/config.json` & `aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/config.json`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/config_se.json` & `aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/config_se.json`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/nconfig.json` & `aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/nconfig.json`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/tts/tts_base_models/khanomtal11/speech.py` & `aivoifu-0.2.8/AIvoifu/tts/tts_base_models/khanomtal11/speech.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/config.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/config.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/attentions.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/attentions.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/commons.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/commons.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/models.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/models.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/models_onnx.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/models_onnx.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/modules.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/modules.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/infer_pack/transforms.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/infer_pack/transforms.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/poetry.lock` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/poetry.lock`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/pyproject.toml` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/python_inference.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/python_inference.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/requirements.txt` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/requirements.txt`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/RVC/vc_infer_pipeline.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/RVC/vc_infer_pipeline.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/vc_inference.py` & `aivoifu-0.2.8/AIvoifu/voice_conversion/vc_inference.py`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/alice/meta.json` & `aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/alice/meta.json`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/ayaka-jp/meta.json` & `aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/ayaka-jp/meta.json`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/kazuha-jp/meta.json` & `aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/kazuha-jp/meta.json`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/readme.md` & `aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/readme.md`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/AIvoifu/voice_conversion/zoo/xiao-jp/meta.json` & `aivoifu-0.2.8/AIvoifu/voice_conversion/zoo/xiao-jp/meta.json`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/LICENSE` & `aivoifu-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/README.md` & `aivoifu-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `aivoifu-0.2.7/pyproject.toml` & `aivoifu-0.2.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "aivoifu"
-version = "0.2.7"
+version = "0.2.8"
 description = "Easy and fast AI Waifu voice generation"
 authors = ["HRNPH <hrnph@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "AIvoifu"}]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = "^3.10"
 gtts = "^2.5.0"
 torch = "^2.1.2"
 fairseq = "^0.12.2"
 wget = "^3.2"
 praat-parselmouth = "^0.4.3"
 pyworld = "^0.3.4"
 faiss-cpu = "^1.7.4"
 setuptools = "^69.0.3"
 edge-tts = "^6.1.10"
 fastapi = "^0.110.0"
 uvicorn = "^0.27.1"
 transformers = "^4.38.2"
 soundfile = "^0.12.1"
 optimum = "^1.17.1"
-tts = "^0.22.0"
 nomkl = "^0.0.3"
+deepspeed = "^0.14.2"
+scipy = "^1.13.0"
+librosa = "^0.10.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.4"
 requests-mock = "^1.11.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `aivoifu-0.2.7/PKG-INFO` & `aivoifu-0.2.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: aivoifu
-Version: 0.2.7
+Version: 0.2.8
 Summary: Easy and fast AI Waifu voice generation
 License: MIT
 Author: HRNPH
 Author-email: hrnph@protonmail.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: deepspeed (>=0.14.2,<0.15.0)
 Requires-Dist: edge-tts (>=6.1.10,<7.0.0)
 Requires-Dist: fairseq (>=0.12.2,<0.13.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: gtts (>=2.5.0,<3.0.0)
+Requires-Dist: librosa (>=0.10.1,<0.11.0)
 Requires-Dist: nomkl (>=0.0.3,<0.0.4)
 Requires-Dist: optimum (>=1.17.1,<2.0.0)
 Requires-Dist: praat-parselmouth (>=0.4.3,<0.5.0)
 Requires-Dist: pyworld (>=0.3.4,<0.4.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Requires-Dist: soundfile (>=0.12.1,<0.13.0)
 Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
-Requires-Dist: tts (>=0.22.0,<0.23.0)
 Requires-Dist: uvicorn (>=0.27.1,<0.28.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Description-Content-Type: text/markdown
 
 # AIwaifu Vocal Pipeline
 Waifu Voice - Made Easy
```

