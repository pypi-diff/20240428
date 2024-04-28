# Comparing `tmp/gendazpack-0.1.0.tar.gz` & `tmp/gendazpack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gendazpack-0.1.0.tar", max compression
+gzip compressed data, was "gendazpack-0.1.1.tar", max compression
```

## Comparing `gendazpack-0.1.0.tar` & `gendazpack-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1085 2024-02-09 02:26:13.630670 gendazpack-0.1.0/LICENSE
--rw-r--r--   0        0        0      895 2024-02-09 02:18:21.196038 gendazpack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1766 2024-02-09 02:39:07.384572 gendazpack-0.1.0/README.rst
--rw-r--r--   0        0        0        0 2022-09-05 23:10:13.045452 gendazpack-0.1.0/src/gendazpack/__init__.py
--rw-r--r--   0        0        0     3738 2024-02-07 21:37:37.627177 gendazpack-0.1.0/src/gendazpack/__main__.py
--rw-r--r--   0        0        0      119 2023-12-10 04:29:09.239477 gendazpack-0.1.0/src/gendazpack/generator/__init__.py
--rw-r--r--   0        0        0     2709 2024-02-09 01:07:55.000901 gendazpack-0.1.0/src/gendazpack/generator/loadmetadata.py
--rw-r--r--   0        0        0     1190 2024-02-07 21:37:10.147721 gendazpack-0.1.0/src/gendazpack/generator/packagedata.py
--rw-r--r--   0        0        0    12398 2024-02-09 01:10:32.023496 gendazpack-0.1.0/src/gendazpack/generator/packagegenerator.py
--rw-r--r--   0        0        0      378 2023-11-19 02:25:00.738769 gendazpack-0.1.0/src/gendazpack/scrapers/__init__.py
--rw-r--r--   0        0        0     3465 2024-02-07 20:49:25.371542 gendazpack-0.1.0/src/gendazpack/scrapers/deviantart.py
--rw-r--r--   0        0        0     6021 2024-01-07 02:51:46.968034 gendazpack-0.1.0/src/gendazpack/scrapers/renderosity.py
--rw-r--r--   0        0        0     5108 2024-01-12 18:28:19.346355 gendazpack-0.1.0/src/gendazpack/scrapers/renderotica.py
--rw-r--r--   0        0        0     1208 2024-02-09 01:10:21.735323 gendazpack-0.1.0/src/gendazpack/scrapers/scraper.py
--rw-r--r--   0        0        0     5410 2024-01-22 05:40:17.071320 gendazpack-0.1.0/src/gendazpack/scrapers/sharecg.py
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 gendazpack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-02-09 02:26:13.630670 gendazpack-0.1.1/LICENSE
+-rw-r--r--   0        0        0      859 2024-04-28 21:13:50.588351 gendazpack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1767 2024-04-28 20:38:56.268546 gendazpack-0.1.1/README.rst
+-rw-r--r--   0        0        0        0 2022-09-05 23:10:13.045452 gendazpack-0.1.1/src/gendazpack/__init__.py
+-rw-r--r--   0        0        0     3740 2024-02-13 02:06:27.760553 gendazpack-0.1.1/src/gendazpack/__main__.py
+-rw-r--r--   0        0        0      119 2023-12-10 04:29:09.239477 gendazpack-0.1.1/src/gendazpack/generator/__init__.py
+-rw-r--r--   0        0        0     2709 2024-02-09 01:07:55.000901 gendazpack-0.1.1/src/gendazpack/generator/loadmetadata.py
+-rw-r--r--   0        0        0     1188 2024-04-17 01:26:13.824284 gendazpack-0.1.1/src/gendazpack/generator/packagedata.py
+-rw-r--r--   0        0        0    14343 2024-04-28 21:12:36.029210 gendazpack-0.1.1/src/gendazpack/generator/packagegenerator.py
+-rw-r--r--   0        0        0      378 2023-11-19 02:25:00.738769 gendazpack-0.1.1/src/gendazpack/scrapers/__init__.py
+-rw-r--r--   0        0        0     3465 2024-02-07 20:49:25.371542 gendazpack-0.1.1/src/gendazpack/scrapers/deviantart.py
+-rw-r--r--   0        0        0     3732 2024-03-16 04:19:22.216416 gendazpack-0.1.1/src/gendazpack/scrapers/renderhub.py
+-rw-r--r--   0        0        0     6021 2024-01-07 02:51:46.968034 gendazpack-0.1.1/src/gendazpack/scrapers/renderosity.py
+-rw-r--r--   0        0        0     5108 2024-03-03 21:53:38.586403 gendazpack-0.1.1/src/gendazpack/scrapers/renderotica.py
+-rw-r--r--   0        0        0     1208 2024-02-09 01:10:21.735323 gendazpack-0.1.1/src/gendazpack/scrapers/scraper.py
+-rw-r--r--   0        0        0     5410 2024-01-22 05:40:17.071320 gendazpack-0.1.1/src/gendazpack/scrapers/sharecg.py
+-rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 gendazpack-0.1.1/PKG-INFO
```

### Comparing `gendazpack-0.1.0/LICENSE` & `gendazpack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.0/pyproject.toml` & `gendazpack-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [tool.poetry]
 name = "gendazpack"
-version = "0.1.0"
+version = "0.1.1"
 description = "DAZ Content Package Generator"
 license = "MIT"
 authors = ["Omni Flux <omniflux@omniflux.com>"]
 readme = "README.rst"
 repository = "https://github.com/Omniflux/gendazpack"
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
 	"Operating System :: OS Independent",
 	"Programming Language :: Python :: 3 :: Only",
 	"Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.11"
-lxml = "^4.9.4"
+lxml = "^5.2.1"
 beautifulsoup4 = "^4.12.3"
-Pillow = "^10.2.0"
-weasyprint = "^60.1"
+Pillow = "^10.3.0"
+weasyprint = "^61.2"
 
 [tool.poetry.group.dev.dependencies]
-types-lxml = "^2023.10.21"
-types-pillow = "^10.2.0.20240206"
-types-beautifulsoup4 = "^4.12.0.20240106"
+types-lxml = "^2024.4.14"
+types-beautifulsoup4 = "^4.12.0.20240229"
 
 [tool.poetry.scripts]
 gendazpack = {reference = "gendazpack.__main__:_main", type = "console"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gendazpack-0.1.0/README.rst` & `gendazpack-0.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ==========
 
 ``gendazpack`` is a DAZ Studio content package generator.
 
 Supported Python versions
 -------------------------
 
-- Python 3.11
+- Python 3.11+
 
 Usage
 -----
 
 ``gendazpack [-h] [-g GLOBAL_ID] [-u URL] [-p PREFIX] [-s SKU] [-I ID] [-S STORE] [-n NAME] [-t <TAGS ...>] [-a <AUTHORS ...>] [-d DESCRIPTION] [-i IMAGE] [-r README] [-v] content_location``
 
 positional arguments:
```

### Comparing `gendazpack-0.1.0/src/gendazpack/__main__.py` & `gendazpack-0.1.1/src/gendazpack/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 	except ValueError as e:
 		raise ArgumentTypeError(e)
 
 	return url
 
 def _prefix(store: str) -> str:
 	if store in (reserved := ('IM', 'DZ', 'DAZ', 'DAZ3D', 'TAFI')):
-		raise ArgumentTypeError(f'Invalid store: {reserved} are reserved')	
+		raise ArgumentTypeError(f'Invalid prefix: {reserved} are reserved')	
 
 	pattern = r'[A-Z][0-9A-Z]{0,6}'
 	if not re.compile(pattern).fullmatch(store):
-		raise ArgumentTypeError(f'Invalid store: Must match regex: {pattern}')
+		raise ArgumentTypeError(f'Invalid prefix: Must match regex: {pattern}')
 
 	return store
 
 def _sku(sku: str) -> int:
 	try:
 		int_sku = int(sku)
 		if int_sku > 99999999:
```

### Comparing `gendazpack-0.1.0/src/gendazpack/generator/loadmetadata.py` & `gendazpack-0.1.1/src/gendazpack/generator/loadmetadata.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.0/src/gendazpack/generator/packagedata.py` & `gendazpack-0.1.1/src/gendazpack/generator/packagedata.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 @dataclass
 class PackageData:
     global_id: UUID | None = None
     prefix: str | None = None
     sku: int | None = None
     store: str | None = None
     name: str | None = None
-    tags: list[str] = field(default_factory=list)
+    tags: set[str] = field(default_factory=set)
     artists: list[str] = field(default_factory=list)
     description: str | None = None
     image: Path | HTTPResponse | None = None
     readme: bytes | Path | None = None
     assets: dict[str, AssetData] = field(default_factory=dict)
     objects: set[ObjectData] = field(default_factory=set)
```

### Comparing `gendazpack-0.1.0/src/gendazpack/generator/packagegenerator.py` & `gendazpack-0.1.1/src/gendazpack/generator/packagegenerator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,56 @@
 import gzip
 import re
 import sys
+import zipfile
 
 from dataclasses import dataclass, fields, KW_ONLY
 from http.client import HTTPResponse
 from mimetypes import guess_extension
 from pathlib import Path
 from urllib.parse import ParseResult
 from uuid import uuid4
-from zipfile import ZipFile, ZIP_DEFLATED
 from lxml import etree
 
 
 from .loadmetadata import load_metadata
 from .packagedata import PackageData
 from ..scrapers import scrape
 
 _CONTENT_DIR = 'Content'
 _SUPPORT_DIR = 'Runtime/Support'
 
+_USER_FACING_DAZ_EXTENSIONS = ('.daz', '.djl', '.duf', '.ds', '.dsa', '.dsb', '.dse')
+_OTHER_DAZ_EXTENSIONS = ('.dhdm', '.dsd', '.dsf', '.dsj', '.dso', '.dsv')
+_COMPRESSABLE_DAZ_EXTENSIONS = ('.dsf', '.duf')
+_NON_USER_FACING_DIRECTORIES = ('data', "readme's", 'runtime', 'uninstallers')
+
+_USER_FACING_POSER_EXTENSIONS = ('.pz3', '.pzz', '.cr2', '.crz', '.pz2', '.p2z', '.fc2', '.fcz', '.hr2', '.hrz', '.hd2', '.hdz', '.pp2', '.ppz', '.lt2', '.ltz', '.cm2', '.cmz', '.mc6', '.mcz', '.mt5', '.mz5')
+_OTHER_POSER_EXTENSIONS = ('.pmd',)
+_POSER_USER_FACING_DIRECTORIES = ('camera', 'character', 'collections', 'face', 'hair', 'hand', 'light', 'materials', 'pose', 'props', 'scene')
+
+_EXCLUDE_FILES = (x.lower() for x in ['.DS_Store', '._.DS_Store', 'InstallManagerFileRegister.json', 'Desktop.ini', 'Thumbs.db'])
+_EXCLUDE_SUFFIXES = ('.xmp',)
+
+
+# DIM does not support Unicode filenames in ZIP files due to using the minizip 1.01 library.
+# Examining offical DAZ packages reveals Windows-1252 encoding is used. Packages with
+# filenames using non ASCII characters may not extract correctly on OS X.
+Ascii_ZipInfo = zipfile.ZipInfo
+class Windows1252_ZipInfo(zipfile.ZipInfo):
+    def _encodeFilenameFlags(self):
+        try:
+            return self.filename.encode('Windows-1252'), self.flag_bits
+        except UnicodeEncodeError as e:
+            raise SystemExit(f'DIM does not support Unicode filenames: {self.filename}') from e
+
+_ENCODING_WARNING = ('WARNING: Non ASCII characters detected in file paths.\n'
+					 'Windows-1252 encoding used for compatibility with DIM.\n'
+					 'Archive may not extract correctly with normal ZIP tools.')
+
 @dataclass
 class PackageGenerator(PackageData):
 	id: int | None = None
 	url: ParseResult | None = None
 	verbose: bool = False
 	_: KW_ONLY
 	content_location: Path
@@ -73,39 +101,34 @@
 
 		etree.SubElement(manifest, 'File', TARGET='Content', ACTION='Install', VALUE=f'{_CONTENT_DIR}/{_SUPPORT_DIR}/{self.metadata_filename_base}.dsa')
 		etree.SubElement(manifest, 'File', TARGET='Content', ACTION='Install', VALUE=f'{_CONTENT_DIR}/{_SUPPORT_DIR}/{self.metadata_filename_base}.dsx')
 		if image_extension := self.metadata_image_extension:
 			etree.SubElement(manifest, 'File', TARGET='Content', ACTION='Install', VALUE=f'{_CONTENT_DIR}/{_SUPPORT_DIR}/{self.metadata_filename_base}{image_extension}')
 
 		etree.indent(manifest, space=' ')
-		return etree.tostring(manifest, pretty_print=True)
+		return etree.tostring(manifest, encoding='UTF-8', pretty_print=True)
 
 	@property
 	def supplement_file(self) -> bytes:
 		if self.verbose:
 			print('Generating Supplement')
 
 		if not self.name:
 			raise RuntimeError(f'Missing Product Name')
 
 		supplement = etree.Element('ProductSupplement', VERSION='0.1')
 		etree.SubElement(supplement, 'ProductName', VALUE=self.name)
 		etree.SubElement(supplement, 'InstallTypes', VALUE='Content')
-		etree.SubElement(supplement, 'ProductTags', VALUE=','.join(self.tags))
+		etree.SubElement(supplement, 'ProductTags', VALUE=','.join(sorted(self.tags)))
 
 		etree.indent(supplement, space=' ')
-		return etree.tostring(supplement, pretty_print=True)
+		return etree.tostring(supplement, encoding='UTF-8', pretty_print=True)
 
 	@property
 	def metadata_file(self) -> bytes:
-		_USER_FACING_DAZ_EXTENSIONS = ['.duf', '.ds', '.dsa', '.dsb', '.dse', '.daz']
-		_USER_FACING_POSER_EXTENSIONS = ['.pz3', '.pzz', '.cr2', '.crz', '.pz2', '.p2z', '.fc2', '.fcz', '.hr2', '.hrz', '.hd2', '.hdz', '.pp2', '.ppz', '.lt2', '.ltz', '.cm2', '.cmz', '.mc6', '.mcz']
-		_NON_USER_FACING_DIRECTORIES = ['data', "readme's", 'runtime', 'uninstallers']
-		_POSER_USER_FACING_DIRECTORIES = ['camera', 'character', 'face', 'hair', 'hand', 'light', 'materials', 'pose', 'props', 'scene']
-
 		if self.verbose:
 			print('Generating Metadata')
 
 		if not self.name:
 			raise RuntimeError(f'Missing Product Name')
 
 		metadata = etree.Element('ContentDBInstall', VERSION='1.0')
@@ -200,14 +223,27 @@
 	if( oAssetMgr )
 	{
 		oAssetMgr.queueDBMetaFile( oFile.baseName() );
 	}
 }
 '''
 
+	@property
+	def guess_tags(self) -> set[str]:
+		tags: set[str] = set()
+
+		if any(x for _, x in self._files() if x.suffix.lower() in _USER_FACING_DAZ_EXTENSIONS + _OTHER_DAZ_EXTENSIONS and not x.parent.as_posix().lower() == 'runtime/support'):
+			tags.add('DAZStudio4_5')
+
+		if any(x for _, x in self._files() if x.suffix.lower() in _USER_FACING_POSER_EXTENSIONS + _OTHER_POSER_EXTENSIONS and x.as_posix().lower().startswith('runtime/')):
+			tags.add('DAZStudio4_5')
+			tags.add('PoserLegacy')
+
+		return tags or set(('General',))
+
 	def __post_init__(self):
 		self._merge_package_data(load_metadata(self.content_location))
 
 		if self.url:
 			self._merge_package_data(scrape(self.url))
 
 		if not self.global_id:
@@ -215,18 +251,16 @@
 
 		if not self.prefix:
 			self.prefix = 'LOCAL'
 
 		if not self.store:
 			self.store = 'LOCAL USER'
 
-		if self.tags:
-			self.tags.sort()
-		else:
-			self.tags.append('DAZStudio4_5')
+		if not self.tags:
+			self.tags = self.guess_tags
 
 	def _merge_package_data(self, package_data: PackageData) -> None:
 		for field in fields(PackageData):
 			if (not getattr(self, field.name)):
 				setattr(self, field.name, getattr(package_data, field.name))
 
 	def _assert_required_vars(self) -> None:
@@ -248,38 +282,38 @@
 		if not self.sanitized_name:
 			exceptions.append(RuntimeError(f"Unable to generate sanitized product name from '{self.name}'"))
 
 		if exceptions:
 			raise ExceptionGroup('Required variables missing', exceptions)
 
 	def _files(self):
-		_EXCLUDE_FILES = [x.lower() for x in ['.DS_Store', '._.DS_Store', 'InstallManagerFileRegister.json', 'Desktop.ini', 'Thumbs.db']]
-		_EXCLUDE_SUFFIXES = ['.xmp']	# lowercase
-
 		for root, _, files in self.content_location.walk():
 			if not (rel_root := root.relative_to(self.content_location)).as_posix() == _SUPPORT_DIR:
 				for file in files:
 					path = Path(file)
 					if not '__MACOSX' in path.parts and not path.name.lower() in _EXCLUDE_FILES and not path.suffix.lower() in _EXCLUDE_SUFFIXES:
 						file_path = root / file
 						if not (path.suffix.lower() == '.rsr' and file_path.with_suffix('.png').exists()):
 							yield(file_path, rel_root / file)
 
 	def _create_zip(self) -> None:
 		_MANIFEST_FILE = 'Manifest.dsx'
 		_SUPPLEMENT_FILE = 'Supplement.dsx'
 		_README_FILE = 'ReadMe.pdf'
-		_DAZ_COMPRESSABLE_EXTENSIONS = ['.dsf', '.duf']	# lowercase
 
 		if self.verbose:
 			print('Generating ZIP file')
 
 		self._assert_required_vars()
 
-		with ZipFile(self.zip_filename, 'x', ZIP_DEFLATED) as zip_file:
+		# Use Windows-1252 encoding for filenames
+		zipfile.ZipInfo = Windows1252_ZipInfo
+		encoding_issue = self.metadata_filename_base.encode() != self.metadata_filename_base.encode('Windows-1252')
+
+		with zipfile.ZipFile(self.zip_filename, 'x', zipfile.ZIP_DEFLATED) as zip_file:
 			# DIM Package
 			zip_file.writestr(_MANIFEST_FILE, self.manifest_file)
 			zip_file.writestr(_SUPPLEMENT_FILE, self.supplement_file)
 
 			# ReadMe
 			if isinstance(self.readme, Path):
 				zip_file.write(self.readme, _README_FILE)
@@ -296,26 +330,35 @@
 					zip_file.writestr(f'{_CONTENT_DIR}/{_SUPPORT_DIR}/{self.metadata_filename_base}{image_extension}', self.image.read())
 
 			# Content
 			if self.verbose:
 				print('Adding Content')
 
 			for file_path, relative_file_path, in self._files():
+				if not encoding_issue and file_path.as_posix().encode() != file_path.as_posix().encode('Windows-1252', 'replace'):
+					encoding_issue = True
+
 				# Compress DAZ compressable files before adding to archive
-				if file_path.suffix.lower() in _DAZ_COMPRESSABLE_EXTENSIONS and file_path.stat().st_size:
+				if file_path.suffix.lower() in _COMPRESSABLE_DAZ_EXTENSIONS and file_path.stat().st_size:
 					with gzip.open(file_path) as f:
 						try:
 							f.read(1)
 							zip_file.write(file_path, _CONTENT_DIR / relative_file_path)
 						except gzip.BadGzipFile:
 							if self.verbose:
 								print (f'Compressing: {relative_file_path}')
 							with open(file_path, 'rb') as f:
 								zip_file.writestr((_CONTENT_DIR / relative_file_path).as_posix(), gzip.compress(f.read()))
 				else:
 					zip_file.write(file_path, _CONTENT_DIR / relative_file_path)
 
+		# Revert filename encoding
+		zipfile.ZipInfo = Ascii_ZipInfo
+
+		if encoding_issue:
+			print(_ENCODING_WARNING)
+
 	def make_package(self) -> None:
 		try:
 			self._create_zip()
 		except (FileExistsError) as e:
 			sys.exit(e)	# pyright: ignore[reportArgumentType]
```

### Comparing `gendazpack-0.1.0/src/gendazpack/scrapers/deviantart.py` & `gendazpack-0.1.1/src/gendazpack/scrapers/deviantart.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.0/src/gendazpack/scrapers/renderosity.py` & `gendazpack-0.1.1/src/gendazpack/scrapers/renderosity.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.0/src/gendazpack/scrapers/renderotica.py` & `gendazpack-0.1.1/src/gendazpack/scrapers/renderotica.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.0/src/gendazpack/scrapers/scraper.py` & `gendazpack-0.1.1/src/gendazpack/scrapers/scraper.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.0/src/gendazpack/scrapers/sharecg.py` & `gendazpack-0.1.1/src/gendazpack/scrapers/sharecg.py`

 * *Files identical despite different names*

### Comparing `gendazpack-0.1.0/PKG-INFO` & `gendazpack-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: gendazpack
-Version: 0.1.0
+Version: 0.1.1
 Summary: DAZ Content Package Generator
 Home-page: https://github.com/Omniflux/gendazpack
 License: MIT
 Author: Omni Flux
 Author-email: omniflux@omniflux.com
 Requires-Python: >=3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
-Requires-Dist: Pillow (>=10.2.0,<11.0.0)
+Requires-Dist: Pillow (>=10.3.0,<11.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
-Requires-Dist: lxml (>=4.9.4,<5.0.0)
-Requires-Dist: weasyprint (>=60.1,<61.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: weasyprint (>=61.2,<62.0)
 Project-URL: Repository, https://github.com/Omniflux/gendazpack
 Description-Content-Type: text/x-rst
 
 gendazpack
 ==========
 
 ``gendazpack`` is a DAZ Studio content package generator.
 
 Supported Python versions
 -------------------------
 
-- Python 3.11
+- Python 3.11+
 
 Usage
 -----
 
 ``gendazpack [-h] [-g GLOBAL_ID] [-u URL] [-p PREFIX] [-s SKU] [-I ID] [-S STORE] [-n NAME] [-t <TAGS ...>] [-a <AUTHORS ...>] [-d DESCRIPTION] [-i IMAGE] [-r README] [-v] content_location``
 
 positional arguments:
```

