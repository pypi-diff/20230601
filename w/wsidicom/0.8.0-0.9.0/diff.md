# Comparing `tmp/wsidicom-0.8.0.tar.gz` & `tmp/wsidicom-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidicom-0.8.0.tar", max compression
+gzip compressed data, was "wsidicom-0.9.0.tar", max compression
```

## Comparing `wsidicom-0.8.0.tar` & `wsidicom-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,43 @@
--rw-r--r--   0        0        0     1074 2023-03-21 13:55:50.924342 wsidicom-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9337 2023-03-21 12:17:48.860546 wsidicom-0.8.0/README.md
--rw-r--r--   0        0        0     1126 2023-03-21 13:55:50.934924 wsidicom-0.8.0/wsidicom/__init__.py
--rw-r--r--   0        0        0    13085 2023-03-21 12:17:48.959087 wsidicom-0.8.0/wsidicom/conceptcode.py
--rw-r--r--   0        0        0     2469 2023-03-21 12:17:48.967976 wsidicom-0.8.0/wsidicom/config.py
--rw-r--r--   0        0        0    36800 2023-03-21 13:55:50.936921 wsidicom-0.8.0/wsidicom/dataset.py
--rw-r--r--   0        0        0     2675 2023-03-18 19:48:50.650475 wsidicom-0.8.0/wsidicom/errors.py
--rw-r--r--   0        0        0      716 2023-03-21 12:17:48.981961 wsidicom-0.8.0/wsidicom/file/__init__.py
--rw-r--r--   0        0        0     2737 2023-03-21 12:17:48.994042 wsidicom-0.8.0/wsidicom/file/base.py
--rw-r--r--   0        0        0    19354 2023-03-21 12:17:49.005675 wsidicom-0.8.0/wsidicom/file/file.py
--rw-r--r--   0        0        0    16983 2023-03-21 12:17:49.018501 wsidicom-0.8.0/wsidicom/file/writer.py
--rw-r--r--   0        0        0    18746 2023-03-21 13:55:50.937922 wsidicom-0.8.0/wsidicom/geometry.py
--rw-r--r--   0        0        0    57579 2023-03-21 12:17:49.030805 wsidicom-0.8.0/wsidicom/graphical_annotations.py
--rw-r--r--   0        0        0      685 2023-03-21 12:17:49.042000 wsidicom-0.8.0/wsidicom/image_data/__init__.py
--rw-r--r--   0        0        0    23235 2023-03-21 12:17:49.052000 wsidicom-0.8.0/wsidicom/image_data/dicom_image_data.py
--rw-r--r--   0        0        0    22329 2023-03-21 13:55:50.939958 wsidicom-0.8.0/wsidicom/image_data/image_data.py
--rw-r--r--   0        0        0     2524 2023-03-21 13:55:50.940923 wsidicom-0.8.0/wsidicom/image_data/pillow_image_data.py
--rw-r--r--   0        0        0    42573 2023-03-21 12:17:49.063996 wsidicom-0.8.0/wsidicom/instance.py
--rw-r--r--   0        0        0    22466 2023-03-21 12:17:49.074084 wsidicom-0.8.0/wsidicom/optical.py
--rw-r--r--   0        0        0    17825 2023-03-21 12:17:49.085969 wsidicom-0.8.0/wsidicom/series.py
--rw-r--r--   0        0        0     3494 2023-01-08 13:38:21.308937 wsidicom-0.8.0/wsidicom/stringprinting.py
--rw-r--r--   0        0        0     3971 2023-03-21 12:17:49.096192 wsidicom-0.8.0/wsidicom/uid.py
--rw-r--r--   0        0        0    25699 2023-03-21 12:17:49.156814 wsidicom-0.8.0/wsidicom/wsidicom.py
--rw-r--r--   0        0        0    10259 1970-01-01 00:00:00.000000 wsidicom-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1122 2023-03-31 13:10:47.122685 wsidicom-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    12076 2023-03-31 13:10:47.106694 wsidicom-0.9.0/README.md
+-rw-r--r--   0        0        0     1136 2023-03-31 13:10:47.211651 wsidicom-0.9.0/wsidicom/__init__.py
+-rw-r--r--   0        0        0    13435 2023-03-31 13:10:47.221649 wsidicom-0.9.0/wsidicom/conceptcode.py
+-rw-r--r--   0        0        0     2091 2023-03-31 13:10:47.233654 wsidicom-0.9.0/wsidicom/config.py
+-rw-r--r--   0        0        0     2779 2023-03-31 13:10:47.244679 wsidicom-0.9.0/wsidicom/errors.py
+-rw-r--r--   0        0        0      817 2023-03-31 13:10:47.256685 wsidicom-0.9.0/wsidicom/file/__init__.py
+-rw-r--r--   0        0        0    16553 2023-03-31 13:10:47.269759 wsidicom-0.9.0/wsidicom/file/wsidicom_file.py
+-rw-r--r--   0        0        0     3099 2023-03-31 13:10:47.281122 wsidicom-0.9.0/wsidicom/file/wsidicom_file_base.py
+-rw-r--r--   0        0        0     3417 2023-03-31 13:10:47.293668 wsidicom-0.9.0/wsidicom/file/wsidicom_file_image_data.py
+-rw-r--r--   0        0        0    11090 2023-03-31 13:10:47.294667 wsidicom-0.9.0/wsidicom/file/wsidicom_file_source.py
+-rw-r--r--   0        0        0    10141 2023-03-31 13:10:47.296667 wsidicom-0.9.0/wsidicom/file/wsidicom_file_target.py
+-rw-r--r--   0        0        0    16373 2023-03-31 13:10:47.307665 wsidicom-0.9.0/wsidicom/file/wsidicom_file_writer.py
+-rw-r--r--   0        0        0    18645 2023-03-31 13:10:47.318918 wsidicom-0.9.0/wsidicom/geometry.py
+-rw-r--r--   0        0        0    56178 2023-03-31 13:10:47.331705 wsidicom-0.9.0/wsidicom/graphical_annotations.py
+-rw-r--r--   0        0        0      764 2023-03-31 13:10:47.345682 wsidicom-0.9.0/wsidicom/group/__init__.py
+-rw-r--r--   0        0        0    16149 2023-03-31 13:10:47.360698 wsidicom-0.9.0/wsidicom/group/group.py
+-rw-r--r--   0        0        0     9344 2023-03-31 13:10:47.374668 wsidicom-0.9.0/wsidicom/group/level.py
+-rw-r--r--   0        0        0     1036 2023-03-31 13:10:47.388667 wsidicom-0.9.0/wsidicom/instance/__init__.py
+-rw-r--r--   0        0        0    32812 2023-03-31 13:10:47.408667 wsidicom-0.9.0/wsidicom/instance/dataset.py
+-rw-r--r--   0        0        0    20352 2023-03-31 13:10:47.422666 wsidicom-0.9.0/wsidicom/instance/image_data.py
+-rw-r--r--   0        0        0     3187 2023-03-31 13:10:47.444180 wsidicom-0.9.0/wsidicom/instance/image_origin.py
+-rw-r--r--   0        0        0     9841 2023-03-31 13:10:47.448730 wsidicom-0.9.0/wsidicom/instance/instance.py
+-rw-r--r--   0        0        0     2344 2023-03-31 13:10:47.466729 wsidicom-0.9.0/wsidicom/instance/pillow_image_data.py
+-rw-r--r--   0        0        0      827 2023-03-31 13:10:47.469223 wsidicom-0.9.0/wsidicom/instance/tile_index/__init__.py
+-rw-r--r--   0        0        0     6088 2023-03-31 13:10:47.486933 wsidicom-0.9.0/wsidicom/instance/tile_index/full_tile_index.py
+-rw-r--r--   0        0        0     6263 2023-03-31 13:10:47.496727 wsidicom-0.9.0/wsidicom/instance/tile_index/sparse_tile_index.py
+-rw-r--r--   0        0        0     6040 2023-03-31 13:10:47.514948 wsidicom-0.9.0/wsidicom/instance/tile_index/tile_index.py
+-rw-r--r--   0        0        0     5091 2023-03-31 13:10:47.516208 wsidicom-0.9.0/wsidicom/instance/wsidicom_image_data.py
+-rw-r--r--   0        0        0    22000 2023-03-31 13:10:47.547680 wsidicom-0.9.0/wsidicom/optical.py
+-rw-r--r--   0        0        0      790 2023-03-31 13:10:47.564679 wsidicom-0.9.0/wsidicom/series/__init__.py
+-rw-r--r--   0        0        0     7979 2023-03-31 13:10:47.585182 wsidicom-0.9.0/wsidicom/series/levels.py
+-rw-r--r--   0        0        0     5557 2023-03-31 13:10:47.605278 wsidicom-0.9.0/wsidicom/series/series.py
+-rw-r--r--   0        0        0     2284 2023-03-31 13:10:47.625904 wsidicom-0.9.0/wsidicom/source.py
+-rw-r--r--   0        0        0     3494 2023-01-08 13:38:21.308937 wsidicom-0.9.0/wsidicom/stringprinting.py
+-rw-r--r--   0        0        0     2721 2023-03-31 13:10:47.644242 wsidicom-0.9.0/wsidicom/target.py
+-rw-r--r--   0        0        0     3959 2023-03-31 13:10:47.668934 wsidicom-0.9.0/wsidicom/uid.py
+-rw-r--r--   0        0        0      816 2023-03-31 13:10:47.696676 wsidicom-0.9.0/wsidicom/web/__init__.py
+-rw-r--r--   0        0        0     4110 2023-03-31 13:10:47.767681 wsidicom-0.9.0/wsidicom/web/wsidicom_web_client.py
+-rw-r--r--   0        0        0     2284 2023-03-31 13:10:47.785828 wsidicom-0.9.0/wsidicom/web/wsidicom_web_image_data.py
+-rw-r--r--   0        0        0     4876 2023-03-31 13:10:47.809797 wsidicom-0.9.0/wsidicom/web/wsidicom_web_source.py
+-rw-r--r--   0        0        0    22222 2023-03-31 13:10:47.831220 wsidicom-0.9.0/wsidicom/wsidicom.py
+-rw-r--r--   0        0        0    12985 1970-01-01 00:00:00.000000 wsidicom-0.9.0/PKG-INFO
```

### Comparing `wsidicom-0.8.0/pyproject.toml` & `wsidicom-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wsidicom"
-version = "0.8.0"
+version = "0.9.0"
 description = "Tools for handling DICOM based whole scan images"
 authors = ["Erik O Gabrielsson <erik.o.gabrielsson@sectra.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/imi-bigpicture/wsidicom"
 keywords = ["whole slide image", "digital pathology", "annotations", "dicom"]
 classifiers = [
@@ -17,20 +17,22 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "^1.22.0"
 pydicom = "^2.1.0"
 Pillow = "^9.1.1"
+dicomweb-client = "^0.59.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-watch = "^4.2.0"
 xmltodict = "^0.12.0"
 shapely = "^1.7.0"
 pycodestyle = "^2.8.0"
+black = "^23.1.0"
 flake8 = "^4.0.1"
 parameterized = "^0.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wsidicom-0.8.0/README.md` & `wsidicom-0.9.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # *wsidicom*
 
-*wsidicom* is a Python package for reading [DICOM WSI](http://dicom.nema.org/Dicom/DICOMWSI/) file sets. The aims with the project are:
+*wsidicom* is a Python package for reading [DICOM WSI](http://dicom.nema.org/Dicom/DICOMWSI/). The aims with the project are:
 
-- Easy to use interface for reading and writing WSI DICOM images and annotations using the DICOM Media Storage Model.
+- Easy to use interface for reading and writing WSI DICOM images and annotations either from file or through DICOMWeb.
 - Support the latest and upcoming DICOM standards.
 - Platform independent installation via PyPI.
 
 ## Installing *wsidicom*
 
 *wsidicom* is available on PyPI:
 
@@ -22,15 +22,15 @@
 
 ## Important note
 
 Please note that this is an early release and the API is not frozen yet. Function names and functionality is prone to change.
 
 ## Requirements
 
-*wsidicom* uses pydicom, numpy and Pillow (with jpeg and jpeg2000 plugins).
+*wsidicom* uses pydicom, numpy, Pillow (with jpeg and jpeg2000 plugins), and dicomweb-client.
 
 ## Limitations
 
 Levels are required to have (close to) 2 factor scale and same tile size.
 
 Only JPEGBaseline8Bit, JPEG2000 and JPEG2000Lossless transfer syntax is supported.
 
@@ -41,120 +41,129 @@
 ***Load a WSI dataset from files in folder.***
 
 ```python
 from wsidicom import WsiDicom
 slide = WsiDicom.open(path_to_folder)
 ```
 
+***Or load a WSI dataset from DICOMWeb.***
+
+```python
+from wsidicom import WsiDicom, WsiDicomWebClient
+from requests.auth import HTTPBasicAuth
+
+auth = HTTPBasicAuth('username', 'password')
+client = WsiDicomWebClient(
+    'dicom_web_hostname',
+    '/qido',
+    '/wado,
+    auth
+)
+slide = WsiDicom.open_web(
+    client,
+    "study uid to open",
+    "series uid top open"
+)
+```
+
+***Use as a context manager.***
+
+```python
+from wsidicom import WsiDicom
+with WsiDicom.open(path_to_folder) as slide:
+    ...
+```
+
 ***Read a 200x200 px region starting from px 1000, 1000 at level 6.***
 
- ```python
+```python
 region = slide.read_region((1000, 1000), 6, (200, 200))
 ```
 
+***Read a 2000x2000 px region starting from px 1000, 1000 at level 4 using 4 threads.***
+
+```python
+region = slide.read_region((1000, 1000), 6, (200, 200), threads=4)
+```
+
 ***Read 3x3 mm region starting at 0, 0 mm at level 6.***
 
- ```python
+```python
 region_mm = slide.read_region_mm((0, 0), 6, (3, 3))
 ```
 
 ***Read 3x3 mm region starting at 0, 0 mm with pixel spacing 0.01 mm/px.***
 
- ```python
+```python
 region_mpp = slide.read_region_mpp((0, 0), 0.01, (3, 3))
 ```
 
 ***Read a thumbnail of the whole slide with maximum dimensions 200x200 px.***
 
- ```python
+```python
 thumbnail = slide.read_thumbnail(200, 200)
 ```
 
 ***Read an overview image (if available).***
 
- ```python
+```python
 overview = slide.read_overview()
 ```
 
 ***Read a label image (if available).***
 
- ```python
+```python
 label = slide.read_label()
 ```
 
 ***Read (decoded) tile from position 1, 1 in level 6.***
 
- ```python
+```python
 tile = slide.read_tile(6, (1, 1))
 ```
 
 ***Read (encoded) tile from position 1, 1 in level 6.***
 
- ```python
+```python
 tile_bytes = slide.read_encoded_tile(6, (1, 1))
 ```
 
 ***Close files***
 
- ```python
-slide.close()
-```
-
-## Settings
-
-*wsidicom* can be configured with the settings variable. For example, set the parsing of files to strict:
-
 ```python
-from wsidicom import settings
-settings.strict_uid_check = True
-settings._strict_attribute_check = True
+slide.close()
 ```
 
-## Data structure
-
-A WSI DICOM pyramid is in *wsidicom* represented by a hierarchy of objects of different classes, starting from bottom:
+## Saving files
 
-- *WsiDicomFile*, represents a WSI DICOM file, used for accessing DicomImageData and WsiDataset.
-- *DicomImageData*, represents the image data in one or several WSI DICOM files.
-- *WsiDataset*, represents the image metadata in one or several WSI DICOM files.
-- *WsiInstance*, represents image data and image metadata.
-- *WsiDicomLevel*, represents a group of instances with the same image size, i.e. of the same level.
-- *WsiDicomLevels*, represents a group of levels, i.e. the pyrimidal structure.
-- *WsiDicom*, represents a collection of levels, labels and overviews.
+An opened WsiDicom instance can be saved to a new path using the save()-method. The produced files will be:
 
-Labels and overviews are structured similarly to levels, but with somewhat different properties and restrictions.
+- Fully tiled. Any sparse tiles will be replaced with a blank tile with color depending on the photometric interpretation.
+- Have a basic offset table (or optionally an exteded offset table or no offset table).
+- Not be concatenated.
 
-The structure is easiest created using the open() helper functions, e.g. to create a WsiDicom-object:
+The frames are copied as-is, i.e. without re-compression.
 
 ```python
-slide = WsiDicom.open(path_to_folder)
+with WsiDicom.open(path_to_folder) as slide:
+    slide.save(path_to_output)
 ```
 
-But the structure can also be created manually from the bottom:
-
-```python
-file = WsiDicomFile(path_to_file)
-instance = WsiInstance(file.dataset, DicomImageData(files))
-level = WsiDicomLevel([instance])
-levels = WsiDicomLevels([level])
-slide = WsiDicom([levels])
-```
+The output folder must already exists. Be careful to specify a unique folder folder to avoid mixing files from diferent images.
 
-## Adding support for other file formats
+## Settings
 
-By subclassing *ImageData* and implementing the required properties (transfer_syntax, image_size, tile_size, and pixel_spacing) and methods (get_tile() and close()) *wsidicom* can be used to access wsi images in other file formats than DICOM. In addition to a ImageData-object, image data, specified in a DICOM dataset, must also be created. For example, assuming a implementation of MyImageData exists that takes a path to a image file as argument and create_dataset() produces a DICOM dataset (see is_wsi_dicom() of WsiDataset for required attributes), WsiInstancees could be created for each pyramidal level, label, or overview:
+*wsidicom* can be configured with the settings variable. For example, set the parsing of files to strict:
 
 ```python
-image_data = MyImageData('path_to_image_file')
-dataset = create_dataset()
-instance = WsiInstance(dataset, image_data)
+from wsidicom import settings
+settings.strict_uid_check = True
+settings._strict_attribute_check = True
 ```
 
-The created instances can then be arranged into levels etc, and opened as a WsiDicom-object as described in 'Data structure'.
-
 ## Annotation usage
 
 Annotations are structured in a hierarchy:
 
 - AnnotationInstance
     Represents a collection of AnnotationGroups. All the groups have the same frame of reference, i.e. annotations are from the same wsi stack.
 - AnnotationGroup
@@ -250,18 +259,72 @@
 
 To run integration tests:
 
 ```console
 poetry run pytest -m integration
 ```
 
+## Data structure
+
+A WSI DICOM pyramid is in *wsidicom* represented by a hierarchy of objects of different classes, starting from bottom:
+
+- *WsiDicomFile*, represents a WSI DICOM file, used for accessing WsiDicomFileImageData and WsiDataset.
+- *WsiDicomFileImageData*, represents the image data in one or several WSI DICOM files.
+- *WsiDataset*, represents the image metadata in one or several WSI DICOM files.
+- *WsiInstance*, represents image data and image metadata.
+- *Level*, represents a group of instances with the same image size, i.e. of the same level.
+- *Levels*, represents a group of levels, i.e. the pyrimidal structure.
+- *WsiDicom*, represents a collection of levels, labels and overviews.
+
+Labels and overviews are structured similarly to levels, but with somewhat different properties and restrictions. For DICOMWeb the WsiDicomFile\* classes are replaced with WsiDicomWeb\* classes.
+
+A Source is used to create WsiInstances, either from files (*WsiDicomFileSource*) or DICOMWeb (*WsiDicomWebSource*), and can be used to to initate a *WsiDicom* object. A source is easiest created with the open() and open_web() helper functions, e.g.:
+
+```python
+slide = WsiDicom.open(path_to_folder)
+```
+
+## Code structure
+
+- [wsidicom.py](wsidicom/wsidicom.py) - Main class with methods to open DICOM WSI objects.
+- [source.py](wsidicom/source.py) - Metaclass Source for serving WsiInstances to WsiDicom.
+- [series](wsidicom/series) - Series implementations Levels, Labels, and Overview.
+- [group](wsidicom/group) - Group implementations, e.g. Level.
+- [instance](wsidicom/instance) - Instance implementations WsiIsntance and WsiDataset, the metaclass ImageData and ImageData implementations WsiDicomImageData and PillowImageData.
+- [file](wsidicom/file) - Implementation for reading and writing DICOM WSI files.
+- [web](wsidicom/web) - Implementation for reading DICOM WSI from DICOMWeb.
+- [graphica_annotations](wsidicom/graphical_annotations.py) - Handling graphical annotations.
+- [conceptcode.py](wsidicom/conceptcode.py) - Handling of DICOM concept codes.
+- [config.py](wsidicom/config.py) - Handles configuration settings.
+- [errors.py](wsidicom/errors.py) - Custom errors.
+- [geometry.py](wsidicom/geometry.py) - Classes for geometry handling.
+- [optical.py](wsidicom/optical.py) - Handles optical paths.
+- [uid.py](wsidicom/uid.py) - Handles DICOM uids.
+- [stringprinting.py](wsidicom/stringprinting.py) - For nicer string printing of objects.
+
+## Adding support for other file formats
+
+Support for other formats (or methods to access DICOM data) can be implemented by creating a new Source implementation, that should create WsiInstances for the implemented formats. A format specific implementations of the *ImageData* is likely needed to access the WSI image data. Additionally a WsiDataset needs to be created that returns matching metadata for the WSI.
+
+The implemented Source can then create a instance from the implemented ImageData (and a method returning a WsiDataset):
+
+```python
+image_data = MyImageData('path_to_image_file')
+dataset = create_dataset_from_image_data(image_data)
+instance = WsiInstance(dataset, image_data)
+```
+
+The source should arrange the created instances and return them at the level_instances, label_instances, and overview_instances properties. WsiDicom can then open the source object and arrange the instances into levels etc as described in 'Data structure'.
+
 ## Other DICOM python tools
 
 - [pydicom](https://pydicom.github.io/)
 - [highdicom](https://github.com/MGHComputationalPathology/highdicom)
+- [wsidicomizer](https://github.com/imi-bigpicture/wsidicomizer)
+- [dicomslide](https://github.com/ImagingDataCommons/dicomslide)
 
 ## Contributing
 
 We welcome any contributions to help improve this tool for the WSI DICOM community!
 
 We recommend first creating an issue before creating potential contributions to check that the contribution is in line with the goals of the project. To submit your contribution, please issue a pull request on the imi-bigpicture/wsidicom repository with your changes for review.
```

### Comparing `wsidicom-0.8.0/wsidicom/__init__.py` & `wsidicom-0.9.0/wsidicom/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,26 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from wsidicom.image_data import ImageData
-from wsidicom.series import WsiDicomLabels, WsiDicomLevels, WsiDicomOverviews
-
-from .config import settings
-from .graphical_annotations import (
+from .wsidicom import WsiDicom
+from wsidicom.config import settings
+from wsidicom.graphical_annotations import (
     Annotation,
     AnnotationGroup,
     AnnotationInstance,
     Measurement,
     Point,
     PointAnnotationGroup,
     Polygon,
     PolygonAnnotationGroup,
     Polyline,
     PolylineAnnotationGroup,
 )
-from .instance import WsiDataset, WsiInstance
-from .wsidicom import WsiDicom
+from wsidicom.instance import ImageData, WsiDataset, WsiInstance
+from wsidicom.series import Labels, Levels, Overviews
+from wsidicom.web import WsiDicomWebClient
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
```

### Comparing `wsidicom-0.8.0/wsidicom/conceptcode.py` & `wsidicom-0.9.0/wsidicom/conceptcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,26 @@
             meaning=code.meaning,
             value=code.value,
             scheme_designator=code.scheme_designator,
             scheme_version=code.scheme_version
         )
 
     @classmethod
+    def from_code(cls, code_value: str) -> Code:
+        try:
+            return next(
+                (
+                    code for code in cls.cid.values()
+                    if code.value == code_value
+                 )
+            )
+        except StopIteration:
+            raise ValueError("Unsupported code.")
+
+    @classmethod
     def _from_cid(cls, meaning: str) -> Code:
         """Return ConceptCode from CID and meaning. For a list of CIDs, see
         http://dicom.nema.org/medical/dicom/current/output/chtml/part16/chapter_B.html # noqa
 
         Parameters
         ----------
         meaning: str
```

### Comparing `wsidicom-0.8.0/wsidicom/config.py` & `wsidicom-0.9.0/wsidicom/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+
 class Settings:
     """Class containing settings. Settings are to be accessed through the
     global variable settings."""
+
     def __init__(self) -> None:
         self._strict_uid_check = False
         self._strict_attribute_check = False
-        self._parse_pixel_data_on_load = True
         self._focal_plane_distance_threshold = 0.000001
 
     @property
     def strict_uid_check(self) -> bool:
         """If frame of reference uid needs to match."""
         return self._strict_uid_check
 
@@ -36,23 +37,14 @@
         return self._strict_attribute_check
 
     @strict_attribute_check.setter
     def strict_attribute_check(self, value: bool) -> None:
         self._strict_attribute_check = value
 
     @property
-    def parse_pixel_data_on_load(self) -> bool:
-        """If to parse pixel data for frame positions on file load."""
-        return self._parse_pixel_data_on_load
-
-    @parse_pixel_data_on_load.setter
-    def parse_pixel_data_on_load(self, value: bool) -> None:
-        self._parse_pixel_data_on_load = value
-
-    @property
     def focal_plane_distance_threshold(self) -> float:
         """Threshold in mm for which distances between focal planes are
         considered to be equal. Default is 1 nm, as distance between focal
         planes are likely larger than this.
         """
         return self._focal_plane_distance_threshold
```

### Comparing `wsidicom-0.8.0/wsidicom/dataset.py` & `wsidicom-0.9.0/wsidicom/instance/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2021, 2022 SECTRA AB
+#    Copyright 2021, 2022, 2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,14 +12,15 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import warnings
 from copy import deepcopy
 from dataclasses import dataclass
 from enum import Enum, IntEnum, auto
+from functools import cached_property
 from typing import Any, List, Optional, Sequence, Tuple, Union, cast
 
 from pydicom.dataset import Dataset
 from pydicom.pixel_data_handlers import pillow_handler
 from pydicom.sequence import Sequence as DicomSequence
 from pydicom.uid import JPEG2000, UID, JPEG2000Lossless, JPEGBaseline8Bit, generate_uid
 from pydicom.valuerep import DSfloat
@@ -29,15 +30,15 @@
     WsiDicomError,
     WsiDicomFileError,
     WsiDicomRequirementError,
     WsiDicomStrictRequirementError,
     WsiDicomUidDuplicateError,
 )
 from wsidicom.geometry import Size, SizeMm
-from wsidicom.image_data import ImageData
+from wsidicom.instance.image_data import ImageData
 from wsidicom.uid import WSI_SOP_CLASS_UID, FileUids, SlideUids
 
 
 class ImageType(Enum):
     VOLUME = "VOLUME"
     LABEL = "LABEL"
     OVERVIEW = "OVERVIEW"
@@ -173,238 +174,284 @@
     "DistanceBetweenFocalPlanes": WsiAttributeRequirement(
         Requirement.STANDARD, default=0.0
     ),
     "SliceThickness": WsiAttributeRequirement(Requirement.STANDARD),
 }
 
 
+class TileType(Enum):
+    FULL = "TILED_FULL"
+    SPARSE = "TILED_SPARSE"
+
+
 class WsiDataset(Dataset):
     """Extend pydicom.dataset.Dataset (containing WSI metadata) with simple
     parsers for attributes specific for WSI. Use snake case to avoid name
     collision with dicom fields (that are handled by pydicom.dataset.Dataset).
     """
 
-    def __init__(self, dataset: Dataset):
-        """A WsiDataset wrapping a pydicom Dataset.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            Pydicom dataset containing WSI data.
-
-        Returns
-        ----------
-        bool
-            True if same instance.
-        """
-        super().__init__(dataset)
-        self._uids = self._get_uids()
-        self._frame_offset = self._get_concatenation_offset()
-        self._frame_count = self._get_dicom_attribute("NumberOfFrames")
-        self._tile_type = self._get_tile_organization_type()
-        self._pixel_measure = self._get_pixel_measure()
-        self._pixel_spacing, self._spacing_between_slices = self._get_spacings(
-            self.pixel_measure
-        )
-        self._number_of_focal_planes = self._get_dicom_attribute(
-            "TotalPixelMatrixFocalPlanes"
-        )
-
-        self._frame_sequence = self._get_frame_sequence()
-        (
-            self._ext_depth_of_field,
-            self._ext_depth_of_field_planes,
-            self._ext_depth_of_field_plane_distance,
-        ) = self._get_ext_depth_of_field()
-
-        self._focus_method = self._get_dicom_attribute("FocusMethod")
-        (self._image_size, self._mm_size, self._mm_depth) = self._get_image_size()
-        self._tile_size = Size(self.Columns, self.Rows)
-        self._samples_per_pixel = self.SamplesPerPixel
-        self._photometric_interpretation = self.PhotometricInterpretation
-        self._optical_path_sequence = self._get_dicom_attribute("OpticalPathSequence")
-        self._slice_thickness = self._get_slice_thickness(self.pixel_measure)
-
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self})"
 
     def __str__(self) -> str:
         return f"{type(self).__name__} of dataset {self.uids.instance}"
 
-    @property
-    def instance_uid(self) -> UID:
-        """Return instance uid from dataset."""
-        return self.uids.instance
-
-    @property
-    def concatenation_uid(self) -> Optional[UID]:
-        """Return concatenation uid, if defined, from dataset. An instance that
-        is concatenated (split into several files) should have the same
-        concatenation uid."""
-        return self.uids.concatenation
+    @cached_property
+    def uids(self) -> FileUids:
+        """Return UIDs from dataset.
 
-    @property
-    def slide_uids(self) -> SlideUids:
-        """Return base uids (study, series, and frame of reference Uids)."""
-        return self.uids.slide
+        Returns
+        ----------
+        FileUids
+            Found UIDs from dataset.
+        """
+        instance_uid = UID(self.SOPInstanceUID)
+        concatenation_uid = self._get_dicom_attribute(
+            "SOPInstanceUIDOfConcatenationSource"
+        )
+        frame_of_reference_uid = self._get_dicom_attribute("FrameOfReferenceUID")
 
-    @property
-    def uids(self) -> FileUids:
-        """Return instance, concatenation, and base Uids."""
-        return self._uids
+        slide_uids = SlideUids(
+            self.StudyInstanceUID,
+            self.SeriesInstanceUID,
+            frame_of_reference_uid,
+        )
+        file_uids = FileUids(instance_uid, concatenation_uid, slide_uids)
+        return file_uids
 
-    @property
+    @cached_property
     def frame_offset(self) -> int:
         """Return frame offset (offset to first frame in instance if
-        concatenated). Is zero if non-catenated instance or first instance
-        in concatenated instance."""
-        return self._frame_offset
+        concatenated). Is zero if non-concatenated instance or first instance
+        in concatenated instance.
 
-    @property
+        Returns
+        ----------
+        int
+            Concatenation offset in number of frames.
+        """
+        if self.uids.concatenation is None:
+            return 0
+        try:
+            return int(self.ConcatenationFrameOffsetNumber)
+        except AttributeError:
+            raise WsiDicomError(
+                "Concatenated file missing concatenation frame offset" "number"
+            )
+
+    @cached_property
     def frame_count(self) -> int:
         """Return number of frames in instance."""
-        return cast(int, self._frame_count)
+        frame_count = self._get_dicom_attribute("NumberOfFrames")
+        return cast(int, frame_count)
 
-    @property
-    def tile_type(self) -> str:
-        """Return tiling type from dataset. Raises WsiDicomError if type
+    @cached_property
+    def tile_type(self) -> TileType:
+        """Return tiling type of dataset. Raises WsiDicomError if type
         is undetermined.
 
-        Parameters
-        ----------
-        ds: Dataset
-            Pydicom dataset.
-
         Returns
         ----------
-        str
+        TileType
             Tiling type
         """
-        return self._tile_type
+        tile_type = self._get_dicom_attribute("DimensionOrganizationType")
+        if tile_type == "TILED_FULL":
+            return TileType.FULL
+        elif "PerFrameFunctionalGroupsSequence" in self:
+            return TileType.SPARSE
+        raise WsiDicomError("Undetermined tile type.")
 
-    @property
+    @cached_property
     def pixel_measure(self) -> Optional[Dataset]:
-        """Return pixel measure from dataset."""
-        return self._pixel_measure
+        """Return Pixel measure dataset from dataset if found.
 
-    @property
+        Returns
+        ----------
+        Optional[Dataset]
+            Found Pixel measure dataset.
+        """
+        shared_functional_group = self._get_dicom_attribute(
+            "SharedFunctionalGroupsSequence"
+        )
+        if shared_functional_group is None:
+            return None
+        pixel_measure_sequence = self._get_dicom_attribute(
+            "PixelMeasuresSequence", shared_functional_group[0]
+        )
+        if pixel_measure_sequence is None:
+            return None
+        return pixel_measure_sequence[0]
+
+    @cached_property
     def pixel_spacing(self) -> Optional[SizeMm]:
         """Read pixel spacing from dicom dataset.
 
         Parameters
         ----------
         ds: Dataset
             Pydicom dataset
 
         Returns
         ----------
         SizeMm
             The pixel spacing in mm/pixel.
         """
-        return self._pixel_spacing
+        if self.pixel_measure is None:
+            return None
+        pixel_spacing_values = getattr(self.pixel_measure, "PixelSpacing", None)
+        if pixel_spacing_values is not None:
+            if any([spacing == 0 for spacing in pixel_spacing_values]):
+                raise WsiDicomError("Pixel spacing is zero")
+            return SizeMm.from_tuple(pixel_spacing_values)
+        return None
 
-    @property
+    @cached_property
     def spacing_between_slices(self) -> Optional[float]:
         """Return spacing between slices."""
-        if self._spacing_between_slices is None:
+        if self.pixel_measure is None:
             return None
-        return cast(float, self._spacing_between_slices)
+        return getattr(self.pixel_measure, "SpacingBetweenSlices", None)
 
-    @property
+    @cached_property
     def number_of_focal_planes(self) -> int:
         """Return number of focal planes."""
-        return cast(int, self._number_of_focal_planes)
+        number_of_focal_planes = self._get_dicom_attribute(
+            "TotalPixelMatrixFocalPlanes"
+        )
+        return cast(int, number_of_focal_planes)
 
-    @property
+    @cached_property
     def frame_sequence(self) -> DicomSequence:
-        """Return frame sequence from dataset."""
-        return self._frame_sequence
+        """Return per frame functional group sequene if present, otherwise
+        shared functional group sequence.
+
+        Returns
+        ----------
+        DicomSequence
+            Per frame or shared functional group sequence.
+        """
+        if "PerFrameFunctionalGroupsSequence" in self and (
+            "PlanePositionSlideSequence" in self.PerFrameFunctionalGroupsSequence[0]
+        ):
+            return self.PerFrameFunctionalGroupsSequence
+        elif "SharedFunctionalGroupsSequence" in self:
+            return self.SharedFunctionalGroupsSequence
+        return DicomSequence([])
 
     @property
     def ext_depth_of_field(self) -> bool:
         """Return true if instance has extended depth of field
         (several focal planes are combined to one plane)."""
-        return self._ext_depth_of_field
+        return self._ext_depth_of_field[0]
 
     @property
     def ext_depth_of_field_planes(self) -> Optional[int]:
         """Return number of focal planes used for extended depth of
         field."""
-        return self._ext_depth_of_field_planes
+        return self._ext_depth_of_field[1]
 
     @property
     def ext_depth_of_field_plane_distance(self) -> Optional[float]:
         """Return total focal depth used for extended depth of field."""
-        return self._ext_depth_of_field_plane_distance
+        return self._ext_depth_of_field[0]
 
-    @property
+    @cached_property
     def focus_method(self) -> str:
         """Return focus method."""
-        return str(self._focus_method)
+        focus_method = self._get_dicom_attribute("FocusMethod")
+        return str(focus_method)
 
-    @property
+    @cached_property
     def image_size(self) -> Size:
         """Read total pixel size from dataset.
 
         Returns
         ----------
         Size
             The image size
         """
-        return self._image_size
+        image_size = Size(self.TotalPixelMatrixColumns, self.TotalPixelMatrixRows)
+        if image_size.width == 0 or image_size.height == 0:
+            raise WsiDicomFileError(self.filepath, "Image size is zero")
+        return image_size
 
-    @property
+    @cached_property
     def mm_size(self) -> Optional[SizeMm]:
         """Read mm size from dataset.
 
         Returns
         ----------
         SizeMm
             The size of the image in mm
         """
-        return self._mm_size
+        mm_width = self._get_dicom_attribute("ImagedVolumeWidth")
+        mm_height = self._get_dicom_attribute("ImagedVolumeHeight")
+        if mm_width is None or mm_height is None:
+            mm_size = None
+        else:
+            mm_size = SizeMm(mm_width, mm_height)
+        return mm_size
 
-    @property
+    @cached_property
     def mm_depth(self) -> Optional[float]:
         """Return depth of image in mm."""
-        return self._mm_depth
+        return self._get_dicom_attribute("ImagedVolumeDepth")
 
-    @property
+    @cached_property
     def tile_size(self) -> Size:
         """Read tile size from from dataset.
 
         Returns
         ----------
         Size
             The tile size
         """
-        return self._tile_size
+        return Size(self.Columns, self.Rows)
 
     @property
     def samples_per_pixel(self) -> int:
         """Return samples per pixel (3 for RGB)."""
-        return self._samples_per_pixel
+        return self.SamplesPerPixel
 
     @property
     def photometric_interpretation(self) -> str:
         """Return photometric interpretation."""
-        return self._photometric_interpretation
+        return self.PhotometricInterpretation
 
-    @property
+    @cached_property
     def optical_path_sequence(self) -> Optional[DicomSequence]:
         """Return optical path sequence from dataset."""
-        return self._optical_path_sequence
+        return self._get_dicom_attribute("OpticalPathSequence")
 
     @property
     def slice_thickness(self) -> Optional[float]:
-        """Return slice thickness."""
-        return self._slice_thickness
+        """Return slice thickness spacing from pixel measure dataset.
 
-    @property
+        Returns
+        ----------
+        Optional[float]
+            Slice thickess or None if unkown.
+        """
+        try:
+            return self._get_dicom_attribute("SliceThickness", self.pixel_measure)
+        except AttributeError:
+            if self.mm_depth is not None:
+                return self.mm_depth / self.number_of_focal_planes
+        return None
+
+    @cached_property
     def image_type(self) -> ImageType:
+        """Return wsi flavour from wsi type tuple.
+
+        Returns
+        ----------
+        ImageType
+            Wsi flavour.
+        """
         return self._get_image_type(self.ImageType)
 
     @classmethod
     def is_supported_wsi_dicom(
         cls, dataset: Dataset, transfer_syntax: UID
     ) -> Optional[ImageType]:
         """Check if dataset is dicom wsi type and that required attributes
@@ -496,15 +543,15 @@
         """Check if instance is valid (Uids and tile size match).
         Base uids should match for instances in all types of series,
         tile size should only match for level series.
         """
         if tile_size is not None and tile_size != self.tile_size:
             return False
 
-        return self.slide_uids.matches(uids)
+        return self.uids.slide.matches(uids)
 
     def read_optical_path_identifier(self, frame: Dataset) -> str:
         """Return optical path identifier from frame, or from self if not
         found."""
         optical_sequence = getattr(
             frame, "OpticalPathIdentificationSequence", self.optical_path_sequence
         )
@@ -738,118 +785,16 @@
         if dataset is None:
             dataset = self
         value = getattr(dataset, name, None)
         if value is None:
             return WSI_ATTRIBUTES[name].get_default(self.image_type)
         return value
 
-    def _get_uids(self) -> FileUids:
-        """Return UIDs from dataset.
-
-        Returns
-        ----------
-        FileUids
-            Found UIDs from dataset.
-        """
-        instance_uid = UID(self.SOPInstanceUID)
-        concatenation_uid = self._get_dicom_attribute(
-            "SOPInstanceUIDOfConcatenationSource"
-        )
-        frame_of_reference_uid = self._get_dicom_attribute("FrameOfReferenceUID")
-
-        slide_uids = SlideUids(
-            self.StudyInstanceUID,
-            self.SeriesInstanceUID,
-            frame_of_reference_uid,
-        )
-        file_uids = FileUids(instance_uid, concatenation_uid, slide_uids)
-        return file_uids
-
-    def _get_concatenation_offset(self) -> int:
-        """Return concatenation offset (number of frames). Will be 0 if file
-        is not concatentated or first in concatenation.
-
-        Returns
-        ----------
-        int
-            Concatenation offset in number of frames.
-        """
-        if self.uids.concatenation is None:
-            return 0
-        try:
-            return int(self.ConcatenationFrameOffsetNumber)
-        except AttributeError:
-            raise WsiDicomError(
-                "Concatenated file missing concatenation frame offset" "number"
-            )
-
-    def _get_tile_organization_type(self) -> str:
-        """Return tile organization type ('TILLED_SPARSE' or 'TILED_FULL').
-
-        Returns
-        ----------
-        str
-            Tile organization type.
-        """
-        tile_type = self._get_dicom_attribute("DimensionOrganizationType")
-        if tile_type == "TILED_FULL":
-            return "TILED_FULL"
-        elif "PerFrameFunctionalGroupsSequence" in self:
-            return "TILED_SPARSE"
-        raise WsiDicomError("undetermined tile type")
-
-    def _get_pixel_measure(self) -> Optional[Dataset]:
-        """Return Pixel measure (sub)-dataset from dataset if found.
-
-        Returns
-        ----------
-        Optional[Dataset]
-            Found Pixel measure dataset.
-        """
-        shared_functional_group = self._get_dicom_attribute(
-            "SharedFunctionalGroupsSequence"
-        )
-        if shared_functional_group is None:
-            return None
-        pixel_measure_sequence = self._get_dicom_attribute(
-            "PixelMeasuresSequence", shared_functional_group[0]
-        )
-        if pixel_measure_sequence is None:
-            return None
-        return pixel_measure_sequence[0]
-
-    @staticmethod
-    def _get_spacings(
-        pixel_measure: Optional[Dataset],
-    ) -> Tuple[Optional[SizeMm], Optional[float]]:
-        """Return Pixel and slice spacing from pixel measure dataset.
-
-        Parameters
-        ----------
-        pixel_measure: Optional[Dataset]
-            Pixel measure dataset.
-
-        Returns
-        ----------
-        Tuple[Optional[SizeMm], Optional[float]]
-            Pixel spacing and slice spacing, or None.
-        """
-        if pixel_measure is None:
-            return None, None
-        pixel_spacing_values = getattr(pixel_measure, "PixelSpacing", None)
-        if pixel_spacing_values is not None:
-            if any([spacing == 0 for spacing in pixel_spacing_values]):
-                raise WsiDicomError("Pixel spacing is zero")
-            pixel_spacing = SizeMm.from_tuple(pixel_spacing_values)
-        else:
-            pixel_spacing = None
-        spacing_between_slices = getattr(pixel_measure, "SpacingBetweenSlices", None)
-        return pixel_spacing, spacing_between_slices
-
-    def _get_ext_depth_of_field(self) -> Tuple[bool, Optional[int], Optional[float]]:
+    @cached_property
+    def _ext_depth_of_field(self) -> Tuple[bool, Optional[int], Optional[float]]:
         """Return extended depth of field (enabled, number of focal planes,
         distance between focal planes) from dataset.
 
         Returns
         ----------
         Tuple[bool, Optional[int], Optional[float]]
             If extended depth of field is used, and if used number of focal
@@ -863,84 +808,14 @@
         if planes is None or distance is None:
             raise WsiDicomFileError(
                 self.filepath,
                 "Missing NumberOfFocalPlanes or DistanceBetweenFocalPlanes",
             )
         return True, planes, distance
 
-    def _get_image_size(self) -> Tuple[Size, Optional[SizeMm], Optional[float]]:
-        """Return image size and physical image size from dataset.
-
-        Returns
-        ----------
-        Tuple[Size, Optional[SizeMm], Optional[float]]:
-            Pixel image size, physical image size and physical depth.
-        """
-        image_size = Size(self.TotalPixelMatrixColumns, self.TotalPixelMatrixRows)
-        if image_size.width == 0 or image_size.height == 0:
-            raise WsiDicomFileError(self.filepath, "Image size is zero")
-
-        mm_width = self._get_dicom_attribute("ImagedVolumeWidth")
-        mm_height = self._get_dicom_attribute("ImagedVolumeHeight")
-        if mm_width is None or mm_height is None:
-            mm_size = None
-        else:
-            mm_size = SizeMm(mm_width, mm_height)
-        mm_depth = self._get_dicom_attribute("ImagedVolumeDepth")
-        return image_size, mm_size, mm_depth
-
-    def _get_slice_thickness(self, pixel_measure: Optional[Dataset]) -> Optional[float]:
-        """Return slice thickness spacing from pixel measure dataset.
-
-        Parameters
-        ----------
-        pixel_measure: Optional[Dataset]
-            Pixel measure dataset.
-
-        Returns
-        ----------
-        Optional[float]
-            Slice thickess or None if unkown.
-        """
-        try:
-            return self._get_dicom_attribute("SliceThickness", pixel_measure)
-        except AttributeError:
-            if self.mm_depth is not None:
-                return self.mm_depth / self.number_of_focal_planes
-        return None
-
-    def _get_frame_sequence(self) -> DicomSequence:
-        """Return per frame functional group sequene if present, otherwise
-        shared functional group sequence.
-
-        Returns
-        ----------
-        DicomSequence
-            Per frame or shared functional group sequence.
-        """
-        if "PerFrameFunctionalGroupsSequence" in self and (
-            "PlanePositionSlideSequence" in self.PerFrameFunctionalGroupsSequence[0]
-        ):
-            return self.PerFrameFunctionalGroupsSequence
-        elif "SharedFunctionalGroupsSequence" in self:
-            return self.SharedFunctionalGroupsSequence
-        return DicomSequence([])
-
-    @staticmethod
-    def _get_image_type(wsi_type: Tuple[str, str, str, str]) -> ImageType:
-        """Return wsi flavour from wsi type tuple.
-
-        Returns
-        ----------
-        str
-            Wsi flavour.
-        """
-        IMAGE_TYPE_INDEX_IN_WSI_TYPE = 2
-        return ImageType(wsi_type[IMAGE_TYPE_INDEX_IN_WSI_TYPE])
-
     @staticmethod
     def _get_spacing_between_slices_for_focal_planes(
         focal_planes: Sequence[float],
     ) -> float:
         """Return spacing between slices in mm for focal planes (defined in
         um). Spacing must be the same between all focal planes for TILED_FULL
         arrangement.
@@ -970,7 +845,19 @@
                     f"{spacing, this_spacing}, difference threshold: "
                     f"{settings.focal_plane_distance_threshold}, "
                     "not possible to encode as TILED_FULL"
                 )
         if spacing is None:
             raise ValueError("Could not calculate spacings.")
         return spacing / 1000.0
+
+    @staticmethod
+    def _get_image_type(wsi_type: Tuple[str, str, str, str]) -> ImageType:
+        """Return wsi flavour from wsi type tuple.
+
+        Returns
+        ----------
+        str
+            Wsi flavour.
+        """
+        IMAGE_TYPE_INDEX_IN_WSI_TYPE = 2
+        return ImageType(wsi_type[IMAGE_TYPE_INDEX_IN_WSI_TYPE])
```

### Comparing `wsidicom-0.8.0/wsidicom/errors.py` & `wsidicom-0.9.0/wsidicom/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,7 +87,11 @@
 class WsiDicomRequirementError(Exception):
     """Raised if required attribute is missing."""
 
 
 class WsiDicomNoResultionError(Exception):
     """Raised if method is not possible as resolution is missing in image
     data."""
+
+
+class WsiDicomNotSupportedError(Exception):
+    """Raised if opened instance is not supported."""
```

### Comparing `wsidicom-0.8.0/wsidicom/file/__init__.py` & `wsidicom-0.9.0/wsidicom/file/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,9 +8,11 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from wsidicom.file.file import WsiDicomFile
-from wsidicom.file.writer import WsiDicomFileWriter
+"""Module for handling DICOM WSI instances read from file."""
+
+from wsidicom.file.wsidicom_file_source import WsiDicomFileSource
+from wsidicom.file.wsidicom_file_target import WsiDicomFileTarget
```

### Comparing `wsidicom-0.8.0/wsidicom/file/base.py` & `wsidicom-0.9.0/wsidicom/file/wsidicom_file_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,36 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+from enum import Enum
 from pathlib import Path
 from typing import Optional
 
 from pydicom.filebase import DicomFile
 from pydicom.tag import BaseTag
 
 
+class OffsetTableType(Enum):
+    NONE = "none"
+    BASIC = "BOT"
+    EXTENDED = "EOT"
+
+    @classmethod
+    def from_string(cls, offset_table: Optional[str]) -> "OffsetTableType":
+        if offset_table is None:
+            return OffsetTableType.NONE
+        if offset_table.strip().lower() == "eot":
+            return OffsetTableType.EXTENDED
+        return OffsetTableType.BASIC
+
+
 class WsiDicomFileBase:
     def __init__(self, filepath: Path, mode: str):
         """Base class for reading or writing DICOM WSI file.
 
         Parameters
         ----------
         filepath: Path
@@ -42,37 +57,30 @@
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.filepath})"
 
     def __str__(self) -> str:
         return self.pretty_str()
 
-    def pretty_str(
-        self,
-        indent: int = 0,
-        depth: Optional[int] = None
-    ) -> str:
+    def pretty_str(self, indent: int = 0, depth: Optional[int] = None) -> str:
         return f"File with path: {self.filepath}"
 
     @property
     def filepath(self) -> Path:
         """Return filepath"""
         return self._filepath
 
     def _read_tag_length(self, with_vr: bool = True) -> int:
         if (not self._fp.is_implicit_VR) and with_vr:
             # Read VR
             self._fp.read_UL()
         return self._fp.read_UL()
 
     def _check_tag_and_length(
-        self,
-        tag: BaseTag,
-        length: int,
-        with_vr: bool = True
+        self, tag: BaseTag, length: int, with_vr: bool = True
     ) -> None:
         """Check if tag at position is expected tag with expected length.
 
         Parameters
         ----------
         tag: BaseTag
             Expected tag.
```

### Comparing `wsidicom-0.8.0/wsidicom/file/file.py` & `wsidicom-0.9.0/wsidicom/file/wsidicom_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,227 +9,187 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import threading
-import warnings
+from functools import cached_property
 from pathlib import Path
 from struct import unpack
-from typing import BinaryIO, Dict, List, Optional, Sequence, Tuple, Union, cast
+from typing import BinaryIO, List, Optional, Tuple, Union, cast
 
 from pydicom.filebase import DicomFileLike
 from pydicom.filereader import read_file_meta_info, read_partial
 from pydicom.misc import is_dicom
 from pydicom.tag import BaseTag, ItemTag, SequenceDelimiterTag, Tag
 from pydicom.uid import UID
 
-from wsidicom.config import settings
-from wsidicom.dataset import ImageType, WsiDataset
-from wsidicom.errors import WsiDicomFileError
-from wsidicom.geometry import Size
-from wsidicom.uid import FileUids, SlideUids
-from wsidicom.file.base import WsiDicomFileBase
+from wsidicom.errors import WsiDicomFileError, WsiDicomNotSupportedError
+from wsidicom.file.wsidicom_file_base import OffsetTableType, WsiDicomFileBase
+from wsidicom.instance import ImageType, WsiDataset
+from wsidicom.uid import FileUids
 
 
 class WsiDicomFile(WsiDicomFileBase):
-    """Represents a DICOM file (potentially) containing WSI image and metadata.
-    """
-    def __init__(
-        self,
-        filepath: Path,
-        parse_pixel_data: Optional[bool] = None
-    ):
+    """Represents a DICOM file (potentially) containing WSI image and metadata."""
+
+    def __init__(self, filepath: Path):
         """Open dicom file in filepath. If valid wsi type read required
         parameters. Parses frames in pixel data but does not read the frames.
 
         Parameters
         ----------
         filepath: Path
             Path to file to open
-        parse_pixel_data: Optional[bool] = None
-            If to parse pixel data on load. Overrides
-            setting.parse_pixel_data_on_load.
         """
-        if parse_pixel_data is None:
-            parse_pixel_data = settings.parse_pixel_data_on_load
         self._lock = threading.Lock()
 
         if not is_dicom(filepath):
             raise WsiDicomFileError(filepath, "is not a DICOM file")
 
         file_meta = read_file_meta_info(filepath)
         self._transfer_syntax_uid = UID(file_meta.TransferSyntaxUID)
 
-        super().__init__(filepath, mode='rb')
+        super().__init__(filepath, mode="rb")
         self._fp.is_little_endian = self._transfer_syntax_uid.is_little_endian
         self._fp.is_implicit_VR = self._transfer_syntax_uid.is_implicit_VR
-        pixel_data_tags = {
-            Tag('PixelData'),
-            Tag('ExtendedOffsetTable')
-        }
-
-        def _stop_at(
-            tag: BaseTag,
-            VR: Optional[str],
-            length: int
-        ) -> bool:
-            return tag in pixel_data_tags
+        extended_offset_table_tag = Tag("ExtendedOffsetTable")
+
+        def _stop_at(tag: BaseTag, VR: Optional[str], length: int) -> bool:
+            return tag >= extended_offset_table_tag
+
         dataset = read_partial(
             cast(BinaryIO, self._fp),
             _stop_at,
             defer_size=None,
             force=False,
             specific_tags=None,
         )
         self._pixel_data_position = self._fp.tell()
 
         self._image_type = WsiDataset.is_supported_wsi_dicom(
-            dataset,
-            self.transfer_syntax
+            dataset, self.transfer_syntax
         )
         if self._image_type is not None:
             self._dataset = WsiDataset(dataset)
-            instance_uid = self.dataset.uids.instance
-            concatenation_uid = self.dataset.uids.concatenation
-            slide_uids = self.dataset.uids.slide
-            self._uids = FileUids(instance_uid, concatenation_uid, slide_uids)
-
-            self._frame_offset = self.dataset.frame_offset
-            self._frame_count = self.dataset.frame_count
-            if parse_pixel_data:
-                (
-                    self._frame_positions,
-                    self._offset_table_type
-                ) = self._parse_pixel_data()
-            else:
-                self._frame_positions = None
-                self._offset_table_type = None
-
         else:
-            warnings.warn(f"Non-supported file {filepath}")
+            raise WsiDicomNotSupportedError(f"Non-supported file {filepath}")
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.filepath})"
 
     def __str__(self) -> str:
         return self.pretty_str()
 
-    @property
-    def offset_table_type(self) -> Optional[str]:
+    @cached_property
+    def offset_table_type(self) -> OffsetTableType:
         """Return type of the offset table, or None if not present."""
-        if self._offset_table_type is None:
-            self._offset_table_type = self._get_offset_table_type()
-        return self._offset_table_type
+        return self._get_offset_table_type()
 
     @property
     def dataset(self) -> WsiDataset:
         """Return pydicom dataset of file."""
         return self._dataset
 
     @property
     def image_type(self) -> Optional[ImageType]:
         return self._image_type
 
     @property
     def uids(self) -> FileUids:
         """Return uids"""
-        return self._uids
+        return self.dataset.uids
 
     @property
     def transfer_syntax(self) -> UID:
         """Return transfer syntax uid"""
         return self._transfer_syntax_uid
 
     @property
     def frame_offset(self) -> int:
         """Return frame offset (for concatenated file, 0 otherwise)"""
-        return self._frame_offset
+        return self.dataset.frame_offset
 
-    @property
+    @cached_property
     def frame_positions(self) -> List[Tuple[int, int]]:
         """Return frame positions and lengths"""
-        if self._frame_positions is None:
-            (
-                self._frame_positions,
-                self._offset_table_type
-            ) = self._parse_pixel_data()
-        return self._frame_positions
+        (frame_positions, offset_table_type) = self._parse_pixel_data()
+        self._offset_table_type = offset_table_type
+        return frame_positions
 
     @property
     def frame_count(self) -> int:
         """Return number of frames"""
-        return self._frame_count
+        return self.dataset.frame_count
 
-    def get_filepointer(
-        self,
-        frame_index: int
-    ) -> Tuple[DicomFileLike, int, int]:
+    def get_filepointer(self, frame_index: int) -> Tuple[DicomFileLike, int, int]:
         """Return file pointer, frame position, and frame length for frame
         number.
 
         Parameters
         ----------
         frame_index: int
             Frame, including concatenation offset, to get.
 
         Returns
         ----------
-        Tuple[DicomFileLike, int, int]:
+        Tuple[WsiDicomFileLike, int, int]:
             File pointer, frame offset and frame length in number of bytes
         """
         frame_index -= self.frame_offset
         frame_position, frame_length = self.frame_positions[frame_index]
         return self._fp, frame_position, frame_length
 
-    def _get_offset_table_type(self) -> Optional[str]:
+    def _get_offset_table_type(self) -> OffsetTableType:
         """
-        Parse file for basic or extended offset table.
+        Parse file for basic (BOT) or extended offset table (EOT). Return if file has
+        EOT and do not check that the BOT is empty (it should be empty according to
+        specifications, but we do not care if it not).
         """
         self._fp.seek(self._pixel_data_position)
         pixel_data_or_eot_tag = Tag(self._fp.read_tag())
-        if pixel_data_or_eot_tag == Tag('ExtendedOffsetTable'):
+        if pixel_data_or_eot_tag == Tag("ExtendedOffsetTable"):
             eot_length = self._read_tag_length()
             self._fp.seek(eot_length, 1)
             self._read_eot_lengths_tag()
-            return 'eot'
+            return OffsetTableType.EXTENDED
         self._validate_pixel_data_start(pixel_data_or_eot_tag)
         bot_length = self._read_bot_length()
         if bot_length is not None:
-            return 'bot'
-        return None
+            return OffsetTableType.BASIC
+        return OffsetTableType.NONE
 
     def _read_bot_length(self) -> Optional[int]:
         """Read the length of the basic table offset (BOT). Returns None if BOT
         is empty.
 
         Returns
         ----------
         Optional[int]
             BOT length.
         """
         BOT_BYTES = 4
         if self._fp.read_tag() != ItemTag:
             raise WsiDicomFileError(
-                self.filepath,
-                "Basic offset table did not start with an ItemTag"
+                self.filepath, "Basic offset table did not start with an ItemTag"
             )
         bot_length = self._fp.read_UL()
         if bot_length == 0:
             return None
         elif bot_length % BOT_BYTES:
             raise WsiDicomFileError(
                 self.filepath,
-                f"Basic offset table should be a multiple of {BOT_BYTES} bytes"
+                f"Basic offset table should be a multiple of {BOT_BYTES} bytes",
             )
         return bot_length
 
     def _read_bot(self) -> Optional[bytes]:
-        """Read basic table offset (BOT). Returns None if BOT is empty
+        """Read basic table offset (BOT). Returns None if BOT is empty. Filepoiter
+        should be positionen to pixel data.
 
         Returns
         ----------
         Optional[bytes]
             BOT in bytes.
         """
         bot_length = self._read_bot_length()
@@ -246,119 +206,114 @@
         int
             EOT length.
         """
         EOT_BYTES = 8
         eot_length = self._read_tag_length()
         if eot_length == 0:
             raise WsiDicomFileError(
-                self.filepath,
-                "Expected Extended offset table present but empty"
+                self.filepath, "Expected Extended offset table present but empty"
             )
         elif eot_length % EOT_BYTES:
             raise WsiDicomFileError(
                 self.filepath,
-                "Extended offset table should be a multiple of "
-                f"{EOT_BYTES} bytes"
+                "Extended offset table should be a multiple of " f"{EOT_BYTES} bytes",
             )
         return eot_length
 
     def _read_eot_lengths_tag(self):
-        """Skip over the length of the extended table offset lengths tag.
-        """
-        tag = self._fp.read_tag()
-        if tag != Tag('ExtendedOffsetTableLengths'):
+        """Skip over the length of the extended table offset lengths tag."""
+        eot_lenths_tag = self._fp.read_tag()
+        if eot_lenths_tag != Tag("ExtendedOffsetTableLengths"):
             raise WsiDicomFileError(
                 self.filepath,
                 "Expected Extended offset table lengths tag after reading "
-                f"Extended offset table, found {tag}"
+                f"Extended offset table, found {eot_lenths_tag}",
             )
         length = self._read_tag_length()
         # Jump over EOT lengths for now
         self._fp.seek(length, 1)
 
     def _read_eot(self) -> bytes:
-        """Read extended table offset (EOT) and EOT lengths.
+        """Read extended table offset (EOT) and EOT lengths. Filepointer should be
+        positionend to extended offset table.
 
         Returns
         ----------
         bytes
             EOT in bytes.
         """
+        eot_tag = Tag(self._fp.read_tag())
+        if eot_tag != Tag("ExtendedOffsetTable"):
+            raise ValueError(f"Expected ExtendedOffsetTable tag, got {eot_tag}")
         eot_length = self._read_eot_length()
         # Read the EOT into bytes
         eot = self._fp.read(eot_length)
         # Read EOT lengths tag
         self._read_eot_lengths_tag()
         return eot
 
     def _parse_table(
-        self,
-        table: bytes,
-        table_type: str,
-        pixels_start: int
+        self, table: bytes, table_type: OffsetTableType, pixels_start: int
     ) -> List[Tuple[int, int]]:
         """Parse table with offsets (BOT or EOT).
 
         Parameters
         ----------
         table: bytes
             BOT or EOT as bytes
-        table_type: str
+        table_type: OffsetTableType
             Type of table, 'bot' or 'eot'.
         pixels_start: int
             Position of first frame item in pixel data.
 
         Returns
         ----------
         List[Tuple[int, int]]
             A list with frame positions and frame lengths.
         """
         if self._fp.is_little_endian:
-            mode = '<'
+            mode = "<"
         else:
-            mode = '>'
-        if table_type == 'bot':
+            mode = ">"
+        if table_type == OffsetTableType.BASIC:
             bytes_per_item = 4
-            mode += 'L'
-        elif table_type == 'eot':
+            mode += "L"
+        elif table_type == OffsetTableType.EXTENDED:
             bytes_per_item = 8
-            mode = 'Q'
+            mode = "Q"
         else:
             raise ValueError("table type should be 'bot' or 'eot'")
         table_length = len(table)
         TAG_BYTES = 4
         LENGTH_BYTES = 4
         positions: List[Tuple[int, int]] = []
         # Read through table to get offset and length for all but last item
         # All read offsets are for item tag of frame and relative to first
         # frame in pixel data.
         this_offset: int = unpack(mode, table[0:bytes_per_item])[0]
         if this_offset != 0:
             raise ValueError("First item in table should be at offset 0")
         for index in range(bytes_per_item, table_length, bytes_per_item):
-            next_offset = unpack(mode, table[index:index+bytes_per_item])[0]
+            next_offset = unpack(mode, table[index : index + bytes_per_item])[0]
             offset = this_offset + TAG_BYTES + LENGTH_BYTES
             length = next_offset - offset
             if length == 0 or length % 2:
-                raise WsiDicomFileError(self.filepath, 'Invalid frame length')
-            positions.append((pixels_start+offset, length))
+                raise WsiDicomFileError(self.filepath, "Invalid frame length")
+            positions.append((pixels_start + offset, length))
             this_offset = next_offset
 
         # Go to last frame in pixel data and read the length of the frame
-        self._fp.seek(pixels_start+this_offset)
+        self._fp.seek(pixels_start + this_offset)
         if self._fp.read_tag() != ItemTag:
-            raise WsiDicomFileError(
-                self.filepath,
-                "Excepcted ItemTag in PixelData"
-            )
+            raise WsiDicomFileError(self.filepath, "Excepcted ItemTag in PixelData")
         length: int = self._fp.read_UL()
         if length == 0 or length % 2:
-            raise WsiDicomFileError(self.filepath, 'Invalid frame length')
-        offset = this_offset+TAG_BYTES+LENGTH_BYTES
-        positions.append((pixels_start+offset, length))
+            raise WsiDicomFileError(self.filepath, "Invalid frame length")
+        offset = this_offset + TAG_BYTES + LENGTH_BYTES
+        positions.append((pixels_start + offset, length))
 
         return positions
 
     def _read_positions_from_pixeldata(self) -> List[Tuple[int, int]]:
         """Get frame positions and length from sequence of frames that ends
         with a tag not equal to ItemTag. fp needs to be positioned after the
         BOT.
@@ -378,30 +333,30 @@
         positions: List[Tuple[int, int]] = []
         frame_position = self._fp.tell()
         # Read items until sequence delimiter
         while self._fp.read_tag() == ItemTag:
             # Read item length
             length: int = self._fp.read_UL()
             if length == 0 or length % 2:
-                raise WsiDicomFileError(self.filepath, 'Invalid frame length')
-            positions.append((frame_position+TAG_BYTES+LENGTH_BYTES, length))
+                raise WsiDicomFileError(self.filepath, "Invalid frame length")
+            positions.append((frame_position + TAG_BYTES + LENGTH_BYTES, length))
             # Jump to end of frame
             self._fp.seek(length, 1)
             frame_position = self._fp.tell()
         self._read_sequence_delimiter()
         return positions
 
     def _read_sequence_delimiter(self):
         """Check if last read tag was a sequence delimiter.
         Raises WsiDicomFileError otherwise.
         """
         TAG_BYTES = 4
         self._fp.seek(-TAG_BYTES, 1)
         if self._fp.read_tag() != SequenceDelimiterTag:
-            raise WsiDicomFileError(self.filepath, 'No sequence delimeter tag')
+            raise WsiDicomFileError(self.filepath, "No sequence delimeter tag")
 
     def read_frame(self, frame_index: int) -> bytes:
         """Return frame data from pixel data by frame index.
 
         Parameters
         ----------
         frame_index: int
@@ -423,138 +378,63 @@
         set as undefined. Raises WsiDicomFileError otherwise.
 
         Parameters
         ----------
         tag: Union[BaseTag, Tuple[int, int]]
             Tag that should be pixel data tag.
         """
-        if tag != Tag('PixelData'):
-            WsiDicomFileError(
-                self.filepath,
-                "Expected PixelData tag"
-            )
+        if tag != Tag("PixelData"):
+            WsiDicomFileError(self.filepath, "Expected PixelData tag")
         length = self._read_tag_length()
         if length != 0xFFFFFFFF:
             raise WsiDicomFileError(
-                self.filepath,
-                "Expected undefined length when reading Pixel data"
+                self.filepath, "Expected undefined length when reading Pixel data"
             )
 
-    def _parse_pixel_data(self) -> Tuple[List[Tuple[int, int]], Optional[str]]:
+    def _parse_pixel_data(self) -> Tuple[List[Tuple[int, int]], OffsetTableType]:
         """Parse file pixel data, reads frame positions.
-        Note that fp needs to be positionend at Extended offset table (EOT)
-        or Pixel data. An EOT can be present before the pixel data, and must
+
+        An EOT can be present before the pixel data, and must
         then not be empty. A BOT most always be the first item in the Pixel
-        data, but can be empty (zero length). If EOT is used BOT must be empty.
+        data, but can be empty (zero length). If EOT is used BOT should be empty.
+
+        First seach to pixel data position, which is either EOT tag or PixelData tag.
+        If EOT read the EOT. For all cases validate that the filepointer now is at the
+        PixelData tag. If BOT read the BOT, otherwise skip the BOT. If EOT nor BOT has
+        been read, parse frame positions from pixel data. Otherwise parse frame
+        positions from EOT or BOT. Finaly check that the number of read frames equals
+        the specified number of frames, otherwise frames are fragmented which we dont
+        support.
 
         Returns
         ----------
-        Tuple[List[Tuple[int, int]], Optional[str]]
+        Tuple[List[Tuple[int, int]], OffsetTableType]
             List of frame positions and lengths, and table type.
         """
+        table_type = self.offset_table_type
         table = None
-        table_type = 'bot'
-        pixel_data_or_eot_tag = Tag(self._fp.read_tag())
-        if pixel_data_or_eot_tag == Tag('ExtendedOffsetTable'):
-            table_type = 'eot'
+        self._fp.seek(self._pixel_data_position)
+        if table_type == OffsetTableType.EXTENDED:
             table = self._read_eot()
-            pixel_data_tag = Tag(self._fp.read_tag())
-        else:
-            pixel_data_tag = pixel_data_or_eot_tag
 
-        self._validate_pixel_data_start(pixel_data_tag)
-        bot = self._read_bot()
+        self._validate_pixel_data_start(Tag(self._fp.read_tag()))
+        if table_type == OffsetTableType.BASIC:
+            table = self._read_bot()
+        else:
+            self._read_bot_length()
 
-        if bot is not None:
-            if table is not None:
-                raise WsiDicomFileError(
-                    self.filepath,
-                    "Both BOT and EOT present"
-                )
-            table = bot
         if table is None:
             frame_positions = self._read_positions_from_pixeldata()
-            table_type = None
         else:
-            frame_positions = self._parse_table(
-                table,
-                table_type,
-                self._fp.tell()
-            )
+            frame_positions = self._parse_table(table, table_type, self._fp.tell())
 
         if self.frame_count != len(frame_positions):
             raise WsiDicomFileError(
                 self.filepath,
                 (
                     f"Frame count {self.frame_count} "
                     f"!= Fragments {len(frame_positions)}."
                     " Fragmented frames are not supported"
-                )
+                ),
             )
 
         return frame_positions, table_type
-
-    @staticmethod
-    def filter_files(
-        files: Sequence['WsiDicomFile'],
-        series_uids: SlideUids,
-        series_tile_size: Optional[Size] = None
-    ) -> List['WsiDicomFile']:
-        """Filter list of wsi dicom files to only include matching uids and
-        tile size if defined.
-
-        Parameters
-        ----------
-        files: Sequence['WsiDicomFile']
-            Wsi files to filter.
-        series_uids: Uids
-            Uids to check against.
-        series_tile_size: Optional[Size] = None
-            Tile size to check against.
-
-        Returns
-        ----------
-        List['WsiDicomFile']
-            List of matching wsi dicom files.
-        """
-        valid_files: List[WsiDicomFile] = []
-
-        for file in files:
-            if file.dataset.matches_series(
-                series_uids,
-                series_tile_size
-            ):
-                valid_files.append(file)
-            else:
-                warnings.warn(
-                    f'{file.filepath} with uids {file.uids.slide} '
-                    f'did not match series with {series_uids} '
-                    f'and tile size {series_tile_size}'
-                )
-                file.close()
-
-        return valid_files
-
-    @classmethod
-    def group_files(
-        cls,
-        files: Sequence['WsiDicomFile']
-    ) -> Dict[str, List['WsiDicomFile']]:
-        """Return files grouped by instance identifier (instances).
-
-        Parameters
-        ----------
-        files: Sequence[WsiDicomFile]
-            Files to group into instances
-
-        Returns
-        ----------
-        Dict[str, List[WsiDicomFile]]
-            Files grouped by instance, with instance identifier as key.
-        """
-        grouped_files: Dict[str, List[WsiDicomFile]] = {}
-        for file in files:
-            try:
-                grouped_files[file.uids.identifier].append(file)
-            except KeyError:
-                grouped_files[file.uids.identifier] = [file]
-        return grouped_files
```

### Comparing `wsidicom-0.8.0/wsidicom/file/writer.py` & `wsidicom-0.9.0/wsidicom/file/wsidicom_file_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2021, 2022 SECTRA AB
+#    Copyright 2021, 2022, 2023 SECTRA AB
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,54 +13,62 @@
 #    limitations under the License.
 
 
 from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime
 from pathlib import Path
 from struct import pack
-from typing import (Any, Dict, Generator, Iterable, List, Optional, Sequence,
-                    Tuple)
+from typing import (
+    Any,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+)
 
 from pydicom.dataset import Dataset, FileMetaDataset, validate_file_meta
 from pydicom.encaps import itemize_frame
 from pydicom.filewriter import write_dataset, write_file_meta_info
 from pydicom.tag import ItemTag, SequenceDelimiterTag, Tag
 from pydicom.uid import UID
 
-from wsidicom.file.base import WsiDicomFileBase
+from wsidicom.file.wsidicom_file_base import OffsetTableType, WsiDicomFileBase
 from wsidicom.geometry import Point, Region, Size
-from wsidicom.image_data import ImageData
+from wsidicom.instance import ImageData
 from wsidicom.uid import WSI_SOP_CLASS_UID
 
 
 class WsiDicomFileWriter(WsiDicomFileBase):
     def __init__(self, filepath: Path) -> None:
         """Return a dicom filepointer.
 
         Parameters
         ----------
         filepath: Path
             Path to filepointer.
 
         """
-        super().__init__(filepath, mode='w+b')
+        super().__init__(filepath, mode="w+b")
         self._fp.is_little_endian = True
         self._fp.is_implicit_VR = False
 
     def write(
         self,
         uid: UID,
         transfer_syntax: UID,
         dataset: Dataset,
         data: Dict[Tuple[str, float], ImageData],
         workers: int,
         chunk_size: int,
-        offset_table: Optional[str],
+        offset_table: OffsetTableType,
         instance_number: int,
-        scale: int = 1
+        scale: int = 1,
     ) -> None:
         """Writes data to file.
 
         Parameters
         ----------
         uid: UID
             Instance UID for file.
@@ -70,64 +78,53 @@
             Dataset to write (exluding pixel data).
         data: Dict[Tuple[str, float], ImageData]
             Pixel data to write.
         workers: int
             Number of workers to use for writing pixel data.
         chunk_size: int
             Number of frames to give each worker.
-        offset_table: Optional[str] = 'bot'
+        offset_table: OffsetTableType
             Offset table to use, 'bot' basic offset table, 'eot' extended
             offset table, None - no offset table.
         instance_number: int
             Instance number for file.
         scale: int = 1
             Scale factor.
 
         """
         self._write_preamble()
         self._write_file_meta(uid, transfer_syntax)
         dataset.SOPInstanceUID = uid
         dataset.InstanceNumber = instance_number
         self._write_base(dataset)
         table_start, pixels_start = self._write_pixel_data_start(
-            dataset.NumberOfFrames,
-            offset_table
+            dataset.NumberOfFrames, offset_table
         )
         frame_positions: List[int] = []
         for (path, z), image_data in sorted(data.items()):
             frame_positions += self._write_pixel_data(
-                image_data,
-                z,
-                path,
-                workers,
-                chunk_size,
-                scale
+                image_data, z, path, workers, chunk_size, scale
             )
         pixels_end = self._fp.tell()
         self._write_pixel_data_end()
 
-        if offset_table is not None:
+        if offset_table is not OffsetTableType.NONE:
             if table_start is None:
-                raise ValueError('Table start should not be None')
-            elif offset_table == 'eot':
-                self._write_eot(
-                    table_start,
-                    pixels_start,
-                    frame_positions,
-                    pixels_end
-                )
-            elif offset_table == 'bot':
+                raise ValueError("Table start should not be None")
+            elif offset_table == OffsetTableType.EXTENDED:
+                self._write_eot(table_start, pixels_start, frame_positions, pixels_end)
+            elif offset_table == OffsetTableType.BASIC:
                 self._write_bot(table_start, pixels_start, frame_positions)
         self.close()
 
     def _write_preamble(self) -> None:
         """Writes file preamble to file."""
-        preamble = b'\x00' * 128
+        preamble = b"\x00" * 128
         self._fp.write(preamble)
-        self._fp.write(b'DICM')
+        self._fp.write(b"DICM")
 
     def _write_file_meta(self, uid: UID, transfer_syntax: UID) -> None:
         """Writes file meta dataset to file.
 
         Parameters
         ----------
         uid: UID
@@ -147,23 +144,20 @@
 
         Parameters
         ----------
         dataset: Dataset
 
         """
         now = datetime.now()
-        dataset.ContentDate = datetime.date(now).strftime('%Y%m%d')
-        dataset.ContentTime = datetime.time(now).strftime('%H%M%S.%f')
+        dataset.ContentDate = datetime.date(now).strftime("%Y%m%d")
+        dataset.ContentTime = datetime.time(now).strftime("%H%M%S.%f")
         write_dataset(self._fp, dataset)
 
     def _write_tag(
-        self,
-        tag: str,
-        value_representation: str,
-        length: Optional[int] = None
+        self, tag: str, value_representation: str, length: Optional[int] = None
     ):
         """Write tag, tag VR and length.
 
         Parameters
         ----------
         tag: str
             Name of tag to write.
@@ -177,41 +171,35 @@
         self._fp.write(bytes(value_representation, "iso8859"))
         self._fp.write_leUS(0)
         if length is not None:
             self._fp.write_leUL(length)
         else:
             self._fp.write_leUL(0xFFFFFFFF)
 
-    def _reserve_eot(
-        self,
-        number_of_frames: int
-    ) -> int:
+    def _reserve_eot(self, number_of_frames: int) -> int:
         """Reserve space in file for extended offset table.
 
         Parameters
         ----------
         number_of_frames: int
             Number of frames to reserve space for.
 
         """
         table_start = self._fp.tell()
         BYTES_PER_ITEM = 8
         eot_length = BYTES_PER_ITEM * number_of_frames
-        self._write_tag('ExtendedOffsetTable', 'OV', eot_length)
+        self._write_tag("ExtendedOffsetTable", "OV", eot_length)
         for _ in range(number_of_frames):
             self._write_unsigned_long_long(0)
-        self._write_tag('ExtendedOffsetTableLengths', 'OV', eot_length)
+        self._write_tag("ExtendedOffsetTableLengths", "OV", eot_length)
         for _ in range(number_of_frames):
             self._write_unsigned_long_long(0)
         return table_start
 
-    def _reserve_bot(
-        self,
-        number_of_frames: int
-    ) -> int:
+    def _reserve_bot(self, number_of_frames: int) -> int:
         """Reserve space in file for basic offset table.
 
         Parameters
         ----------
         number_of_frames: int
             Number of frames to reserve space for.
 
@@ -222,17 +210,15 @@
         self._fp.write_tag(ItemTag)
         self._fp.write_leUL(tag_lengths)
         for _ in range(number_of_frames):
             self._fp.write_leUL(0)
         return table_start
 
     def _write_pixel_data_start(
-        self,
-        number_of_frames: int,
-        offset_table: Optional[str]
+        self, number_of_frames: int, offset_table: OffsetTableType
     ) -> Tuple[Optional[int], int]:
         """Writes tags starting pixel data and reserves space for BOT or EOT.
 
         Parameters
         ----------
         number_of_frames: int
             Number of frames to reserve space for in BOT or EOT.
@@ -242,35 +228,32 @@
 
         Returns
         ----------
         Tuple[Optional[int], int]
             Start of table (BOT or EOT) and start of pixel data (after BOT).
         """
         table_start: Optional[int] = None
-        if offset_table == 'eot':
+        if offset_table == OffsetTableType.EXTENDED:
             table_start = self._reserve_eot(number_of_frames)
 
         # Write pixel data tag
-        self._write_tag('PixelData', 'OB')
+        self._write_tag("PixelData", "OB")
 
-        if offset_table == 'bot':
+        if offset_table == OffsetTableType.BASIC:
             table_start = self._reserve_bot(number_of_frames)
         else:
             self._fp.write_tag(ItemTag)  # Empty BOT
             self._fp.write_leUL(0)
 
         pixel_data_start = self._fp.tell()
 
         return table_start, pixel_data_start
 
     def _write_bot(
-        self,
-        bot_start: int,
-        pixel_data_start: int,
-        frame_positions: Sequence[int]
+        self, bot_start: int, pixel_data_start: int, frame_positions: Sequence[int]
     ) -> None:
         """Writes BOT to file.
 
         Parameters
         ----------
         bot_start: int
             File position of BOT start
@@ -287,42 +270,37 @@
             raise NotImplementedError(
                 "Image data exceeds 2^32 - 1 bytes "
                 "An extended offset table should be used"
             )
 
         self._fp.seek(bot_start)  # Go to first BOT entry
         self._check_tag_and_length(
-            ItemTag,
-            BYTES_PER_ITEM*len(frame_positions),
-            False
+            ItemTag, BYTES_PER_ITEM * len(frame_positions), False
         )
 
         for frame_position in frame_positions:  # Write BOT
-            self._fp.write_leUL(frame_position-pixel_data_start)
+            self._fp.write_leUL(frame_position - pixel_data_start)
 
-    def _write_unsigned_long_long(
-        self,
-        value: int
-    ):
+    def _write_unsigned_long_long(self, value: int):
         """Write unsigned long long integer (64 bits) as little endian.
 
         Parameters
         ----------
         value: int
             Value to write.
 
         """
-        self._fp.write(pack('<Q', value))
+        self._fp.write(pack("<Q", value))
 
     def _write_eot(
         self,
         eot_start: int,
         pixel_data_start: int,
         frame_positions: Sequence[int],
-        last_frame_end: int
+        last_frame_end: int,
     ) -> None:
         """Writes EOT to file.
 
         Parameters
         ----------
         bot_start: int
             File position of EOT start
@@ -339,25 +317,23 @@
         last_entry = frame_positions[-1] - pixel_data_start
         if last_entry > 2**64 - 1:
             raise ValueError(
                 "Image data exceeds 2^64 - 1 bytes, likely something is wrong"
             )
         self._fp.seek(eot_start)  # Go to EOT table
         self._check_tag_and_length(
-            Tag('ExtendedOffsetTable'),
-            BYTES_PER_ITEM*len(frame_positions)
+            Tag("ExtendedOffsetTable"), BYTES_PER_ITEM * len(frame_positions)
         )
         for frame_position in frame_positions:  # Write EOT
-            relative_position = frame_position-pixel_data_start
+            relative_position = frame_position - pixel_data_start
             self._write_unsigned_long_long(relative_position)
 
         # EOT LENGTHS
         self._check_tag_and_length(
-            Tag('ExtendedOffsetTableLengths'),
-            BYTES_PER_ITEM*len(frame_positions)
+            Tag("ExtendedOffsetTableLengths"), BYTES_PER_ITEM * len(frame_positions)
         )
         frame_start = frame_positions[0]
         for frame_end in frame_positions[1:]:  # Write EOT lengths
             frame_length = frame_end - frame_start
             self._write_unsigned_long_long(frame_length)
             frame_start = frame_end
 
@@ -372,16 +348,16 @@
         self,
         image_data: ImageData,
         z: float,
         path: str,
         workers: int,
         chunk_size: int,
         scale: int = 1,
-        image_format: str = 'jpeg',
-        image_options: Optional[Dict[str, Any]] = None
+        image_format: str = "jpeg",
+        image_options: Optional[Dict[str, Any]] = None,
     ) -> List[int]:
         """Writes pixel data to file.
 
         Parameters
         ----------
         image_data: ImageData
             Image data to read pixel tiles from.
@@ -404,39 +380,34 @@
         Returns
         ----------
         List[int]
             List of frame position (position of ItemTag), relative to start of
             file.
         """
         if image_options is None:
-            image_options = {'quality': 95}
-        chunked_tile_points = self._chunk_tile_points(
-            image_data,
-            chunk_size,
-            scale
-        )
+            image_options = {"quality": 95}
+        chunked_tile_points = self._chunk_tile_points(image_data, chunk_size, scale)
 
         if scale == 1:
+
             def get_tiles_thread(tile_points: Iterable[Point]) -> List[bytes]:
                 """Thread function to get tiles as bytes."""
                 return image_data.get_encoded_tiles(tile_points, z, path)
+
             get_tiles = get_tiles_thread
         else:
+
             def get_scaled_tiles_thread(
-                scaled_tile_points: Iterable[Point]
+                scaled_tile_points: Iterable[Point],
             ) -> List[bytes]:
                 """Thread function to get scaled tiles as bytes."""
                 return image_data.get_scaled_encoded_tiles(
-                    scaled_tile_points,
-                    z,
-                    path,
-                    scale,
-                    image_format,
-                    image_options
+                    scaled_tile_points, z, path, scale, image_format, image_options
                 )
+
             get_tiles = get_scaled_tiles_thread
 
         def write_frame(frame: bytes) -> int:
             """Itemize and write frame to file. Return frame position."""
             position = self._fp.tell()
             self._fp.write(frame)
             return position
@@ -448,62 +419,50 @@
                 for tile in get_tiles(chunk)
                 for frame in itemize_frame(tile, 1)
             ]
 
         with ThreadPoolExecutor(max_workers=workers) as pool:
             return [
                 write_frame(frame)
-                for thread_result in pool.map(
-                    get_tiles,
-                    chunked_tile_points
-                )
+                for thread_result in pool.map(get_tiles, chunked_tile_points)
                 for tile in thread_result
                 for frame in itemize_frame(tile, 1)
             ]
 
     def _chunk_tile_points(
-        self,
-        image_data: ImageData,
-        chunk_size: int,
-        scale: int = 1
-    ) -> Generator[Generator[Point, None, None], None, None]:
+        self, image_data: ImageData, chunk_size: int, scale: int = 1
+    ) -> Iterator[Iterator[Point]]:
         """Divides tile positions in image_data into chunks.
 
         Parameters
         ----------
         image_data: ImageData
             Image data with tiles to chunk.
         chunk_size: int
             Requested chunk size
         scale: int = 1
             Scaling factor (1 = no scaling).
 
         Returns
         ----------
-        Generator[Generator[Point, None, None], None, None]
+        Iterator[Iterator[Point]]
             Chunked tile positions
         """
-        minimum_chunk_size = getattr(
-            image_data,
-            'suggested_minimum_chunk_size',
-            1
-        )
+        minimum_chunk_size = getattr(image_data, "suggested_minimum_chunk_size", 1)
         # If chunk_size is less than minimum_chunk_size, use minimum_chunk_size
         # Otherwise, set chunk_size to highest even multiple of
         # minimum_chunk_size
         chunk_size = max(
-            minimum_chunk_size,
-            chunk_size//minimum_chunk_size * minimum_chunk_size
+            minimum_chunk_size, chunk_size // minimum_chunk_size * minimum_chunk_size
         )
         new_tiled_size = image_data.tiled_size.ceil_div(scale)
         # Divide the image tiles up into chunk_size chunks (up to tiled size)
         chunked_tile_points = (
             Region(
-                Point(x, y),
-                Size(min(chunk_size, new_tiled_size.width - x), 1)
+                Point(x, y), Size(min(chunk_size, new_tiled_size.width - x), 1)
             ).iterate_all()
             for y in range(new_tiled_size.height)
             for x in range(0, new_tiled_size.width, chunk_size)
         )
         return chunked_tile_points
 
     def _write_pixel_data_end(self) -> None:
```

### Comparing `wsidicom-0.8.0/wsidicom/geometry.py` & `wsidicom-0.9.0/wsidicom/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import math
 from dataclasses import dataclass
-from typing import Generator, Tuple, Union, Sequence
+from typing import Iterator, Tuple, Union, Sequence
 
 
 @dataclass
 class SizeMm:
     width: float
     height: float
 
@@ -324,20 +324,19 @@
     def box(self) -> Tuple[int, int, int, int]:
         return self.start.x, self.start.y, self.end.x, self.end.y
 
     @property
     def box_from_origin(self) -> Tuple[int, int, int, int]:
         return 0, 0, self.size.width, self.size.height
 
-    def iterate_all(self, include_end: bool = False) -> Generator[Point, None, None]:
-        offset = 1 if include_end else 0
+    def iterate_all(self) -> Iterator[Point]:
         return (
             Point(x, y)
-            for y in range(self.start.y, self.end.y + offset)
-            for x in range(self.start.x, self.end.x + offset)
+            for y in range(self.start.y, self.end.y)
+            for x in range(self.start.x, self.end.x)
         )
 
     @classmethod
     def from_points(cls, point_1: "Point", point_2: "Point") -> "Region":
         return cls(
             position=point_1,
             size=Size(width=point_2.x - point_1.x, height=point_2.y - point_1.y),
```

### Comparing `wsidicom-0.8.0/wsidicom/graphical_annotations.py` & `wsidicom-0.9.0/wsidicom/graphical_annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,51 @@
 #    limitations under the License.
 
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path
-from typing import (Any, Callable, DefaultDict, Dict, Generator, Generic, List,
-                    Optional, Sequence, Set, Tuple, Type, TypeVar, Union)
+from typing import (
+    Any,
+    Callable,
+    DefaultDict,
+    Dict,
+    Generic,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import numpy as np
-from pydicom.dataset import (Dataset, FileDataset, FileMetaDataset,
-                             validate_file_meta)
+from pydicom.dataset import Dataset, FileDataset, FileMetaDataset, validate_file_meta
 from pydicom.filereader import dcmread
 from pydicom.filewriter import dcmwrite
 from pydicom.sequence import Sequence as DicomSequence
-from pydicom.uid import (ExplicitVRBigEndian, ExplicitVRLittleEndian,
-                         ImplicitVRLittleEndian, generate_uid)
+from pydicom.uid import (
+    ExplicitVRBigEndian,
+    ExplicitVRLittleEndian,
+    ImplicitVRLittleEndian,
+    generate_uid,
+)
 from pydicom.values import convert_numbers
 
-from wsidicom.conceptcode import (AnnotationCategoryCode, AnnotationTypeCode,
-                                  MeasurementCode, UnitCode)
+from wsidicom.conceptcode import (
+    AnnotationCategoryCode,
+    AnnotationTypeCode,
+    MeasurementCode,
+    UnitCode,
+)
 
 from .geometry import PointMm, RegionMm, SizeMm
 from .uid import ANN_SOP_CLASS_UID, UID, SlideUids
 
 
 @dataclass
 class LabColor:
@@ -55,19 +77,15 @@
         Struct format character.
 
     Returns
     ----------
     List[Any]
         List of values
     """
-    converted = convert_numbers(
-        item,
-        is_little_endian=True,
-        struct_format=format
-    )
+    converted = convert_numbers(item, is_little_endian=True, struct_format=format)
     if not isinstance(converted, list):
         return [converted]
     return converted
 
 
 @dataclass
 class Measurement:
@@ -101,65 +119,53 @@
             Other base to compare to.
 
         Returns
         ----------
         bool
             True if bases are same.
         """
-        return (
-            self.code == other_code and
-            self.unit == other_unit
-        )
+        return self.code == other_code and self.unit == other_unit
 
     @staticmethod
-    def _get_measurement_type_from_ds(
-        ds: Dataset
-    ) -> Tuple[MeasurementCode, UnitCode]:
+    def _get_measurement_type_from_ds(ds: Dataset) -> Tuple[MeasurementCode, UnitCode]:
         """Get measurement type from dataset.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing measurement sequence item (group).
 
         Returns
         ----------
         MeasurementType
             Measurement type of the measurement group.
         """
         code = MeasurementCode.from_ds(ds)
         if code is None:
-            raise ValueError(
-                f'Dataset is missing {MeasurementCode.sequence_name}.'
-            )
+            raise ValueError(f"Dataset is missing {MeasurementCode.sequence_name}.")
         unit = UnitCode.from_ds(ds)
         if unit is None:
-            raise ValueError(f'Dataset is missing {UnitCode.sequence_name}.')
+            raise ValueError(f"Dataset is missing {UnitCode.sequence_name}.")
         return code, unit
 
     @staticmethod
-    def _get_measurement_values_from_ds(
-        ds: Dataset
-    ) -> List[float]:
+    def _get_measurement_values_from_ds(ds: Dataset) -> List[float]:
         """Get measurement values from dataset.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing measurement sequence item (group).
 
         Returns
         ----------
         List[float]
             Measurement values of the measurement group.
         """
-        return dcm_to_list(
-            ds.MeasurementValuesSequence[0].FloatingPointValues,
-            'f'
-        )
+        return dcm_to_list(ds.MeasurementValuesSequence[0].FloatingPointValues, "f")
 
     @staticmethod
     def _get_measurement_indices_from_ds(
         ds: Dataset,
         annotation_count: int,
     ) -> List[int]:
         """Get measurement indices from dataset. Annotation index is stored as
@@ -175,63 +181,51 @@
 
         Returns
         ----------
         List[int]
             Measurement indices of the measurement group.
         """
         measurement_ds = ds.MeasurementValuesSequence[0]
-        if 'AnnotationIndexList' in measurement_ds:
-            indices = dcm_to_list(measurement_ds.AnnotationIndexList, 'l')
-            return [index-1 for index in indices]
+        if "AnnotationIndexList" in measurement_ds:
+            indices = dcm_to_list(measurement_ds.AnnotationIndexList, "l")
+            return [index - 1 for index in indices]
         return list(range(annotation_count))
 
     @classmethod
     def _iterate_measurement_sequence(
-        cls,
-        sequence: DicomSequence,
-        annotation_count: int
-    ) -> Generator[Tuple[int, 'Measurement'], None, None]:
+        cls, sequence: DicomSequence, annotation_count: int
+    ) -> Iterator[Tuple[int, "Measurement"]]:
         """Return generator for measurements in dataset. Yields a tuple of
         the index of the annotation for the measurement and the measurement.
 
         Parameters
         ----------
         sequence: DicomSequence
             Dicom measurement sequence.
         annotation_count: int
             Number of annotations in group.
 
         Returns
         ----------
-        Generator[Tuple[int, 'Measurement'], None, None]:
+        Iterator[Tuple[int, 'Measurement']]:
             Generator for annotation index and measurement.
         """
         for group_ds in sequence:
             code, unit = cls._get_measurement_type_from_ds(group_ds)
             values = cls._get_measurement_values_from_ds(group_ds)
-            indices = cls._get_measurement_indices_from_ds(
-                group_ds,
-                annotation_count
-            )
+            indices = cls._get_measurement_indices_from_ds(group_ds, annotation_count)
             if len(values) != len(indices):
-                raise ValueError(
-                    "number of indices needs to be same as measurements"
-                )
+                raise ValueError("number of indices needs to be same as measurements")
             for index, annotation_index in enumerate(indices):
-                yield (
-                    annotation_index,
-                    Measurement(code, values[index], unit)
-                )
+                yield (annotation_index, Measurement(code, values[index], unit))
 
     @classmethod
     def get_measurements_from_ds(
-        cls,
-        sequence: DicomSequence,
-        annotation_count: int
-    ) -> Dict[int, List['Measurement']]:
+        cls, sequence: DicomSequence, annotation_count: int
+    ) -> Dict[int, List["Measurement"]]:
         """Get measurements from dataset.
 
         Parameters
         ----------
         sequence: DicomSequence
             Dicom measurement sequence.
         annotation_count: int
@@ -240,16 +234,15 @@
         Returns
         ----------
         Dict[int, List[Measurement]]
             Dict of measurements grouped by annotation number as key.
         """
         measurements: DefaultDict[int, List[Measurement]] = defaultdict(list)
         for annotation_index, measurement in cls._iterate_measurement_sequence(
-            sequence,
-            annotation_count
+            sequence, annotation_count
         ):
             measurements[annotation_index].append(measurement)
         return dict(measurements)
 
 
 class Geometry(metaclass=ABCMeta):
     name: str
@@ -282,31 +275,27 @@
     @abstractmethod
     def __repr__(self) -> str:
         raise NotImplementedError()
 
     @classmethod
     @abstractmethod
     def from_coords(
-        cls,
-        coords: Union[Tuple[float, float], Sequence[Tuple[float, float]]]
-    ) -> 'Geometry':
+        cls, coords: Union[Tuple[float, float], Sequence[Tuple[float, float]]]
+    ) -> "Geometry":
         """Return geometry object created from list of coordinates"""
         raise NotImplementedError()
 
     @classmethod
     @abstractmethod
-    def from_list(cls, list: Sequence[float]) -> 'Geometry':
+    def from_list(cls, list: Sequence[float]) -> "Geometry":
         """Return geometry object created from list of floats"""
         raise NotImplementedError()
 
     @classmethod
-    def list_to_coords(
-        cls,
-        data: Sequence[float]
-    ) -> List[Tuple[float, float]]:
+    def list_to_coords(cls, data: Sequence[float]) -> List[Tuple[float, float]]:
         """Return cordinates in list of floats as list of tuple of floats
 
         Parameters
         ----------
         data: Sequence[float]
             List of float to convert.
 
@@ -314,27 +303,25 @@
         ----------
         List[Tuple[float, float]]
             List of coordinates (Tuple of floats).
         """
         x_indices = range(0, len(data), 2)
         y_indices = range(1, len(data), 2)
         coords: List[Tuple[float, float]] = [
-            (float(data[x]), float(data[y]))
-            for x, y in zip(x_indices, y_indices)
+            (float(data[x]), float(data[y])) for x, y in zip(x_indices, y_indices)
         ]
         return coords
 
     @staticmethod
     def _coordinates_from_dict(
         dictionary: Union[
-            Dict[str, Union[str, float]],
-            Sequence[Dict[str, Union[str, float]]]
+            Dict[str, Union[str, float]], Sequence[Dict[str, Union[str, float]]]
         ],
         x: str,
-        y: str
+        y: str,
     ) -> List[Tuple[float, float]]:
         """Return coordinates in dictionary as list of tuple of floats
 
         Parameters
         ----------
         dictionary: Union[
             Dict[str, Union[str, float]],
@@ -351,34 +338,30 @@
         List[Tuple[float, float]]
             List of coordinates (Tuple of floats).
         """
         if not isinstance(dictionary, Sequence):
             coords = [dictionary]
         else:
             coords = dictionary
-        return [
-            (float(coordinate[x]), float(coordinate[y]))
-            for coordinate in coords
-        ]
+        return [(float(coordinate[x]), float(coordinate[y])) for coordinate in coords]
 
     @classmethod
     @abstractmethod
     def from_dict(
         cls,
         dictionary: Union[
-            Dict[str, Union[str, float]],
-            Sequence[Dict[str, Union[str, float]]]
+            Dict[str, Union[str, float]], Sequence[Dict[str, Union[str, float]]]
         ],
         x: str,
         y: str,
-    ) -> 'Geometry':
+    ) -> "Geometry":
         raise NotImplementedError()
 
     @classmethod
-    def from_shapely_like(cls, object: Any) -> 'Geometry':
+    def from_shapely_like(cls, object: Any) -> "Geometry":
         """Return Geometry from shapely-like object. Object needs to have
         shapely-like attributes.
 
         Parameters
         ----------
         ojbect
             Object with shapely-like attributes.
@@ -398,18 +381,15 @@
             elif geometry_type == "LineString":
                 return Polyline(object.coords)
             raise NotImplementedError("Not a supported shapely like object")
         except AttributeError:
             raise ValueError("Not a shapely like object")
 
     @classmethod
-    def from_geojson(
-        cls,
-        dictionary: Dict[str, Any]
-    ) -> List['Geometry']:
+    def from_geojson(cls, dictionary: Dict[str, Any]) -> List["Geometry"]:
         """Return geometries from geojson geometry dictionary. Note that
         MultiPoint returns multiple points.
 
         Parameters
         ----------
         dictionary
             Geojson geometry dictionary.
@@ -420,43 +400,42 @@
             Geometry created from Geojson dictionary.
         """
         try:
             coordinates: List[Any] = dictionary["coordinates"]
             annotation_type: str = dictionary["type"]
         except KeyError:
             raise ValueError("Not a geojson object")
-        if(annotation_type == 'Point'):
+        if annotation_type == "Point":
             points: List[float] = coordinates
             return [Point.from_list(points)]
-        elif(annotation_type == 'MultiPoint'):
+        elif annotation_type == "MultiPoint":
             multipoints: List[List[float]] = coordinates
             return [Point.from_list(point) for point in multipoints]
-        elif(annotation_type == 'Polygon'):
+        elif annotation_type == "Polygon":
             polylines: List[List[Tuple[float, float]]] = coordinates
             return [Polygon.from_coords(polylines[0])]
-        elif(annotation_type == 'LineString'):
+        elif annotation_type == "LineString":
             polyline: List[Tuple[float, float]] = coordinates
             return [Polyline.from_coords(polyline)]
         raise NotImplementedError("Not supported geojson geometry")
 
 
 @dataclass
 class Point(Geometry):
     """Geometry consisting of a single point"""
-    name = 'POINT'
+
+    name = "POINT"
 
     def __init__(self, x: float, y: float):
         self.x = float(x)
         self.y = float(y)
 
-    def __eq__(self, point: 'Point') -> bool:
+    def __eq__(self, point: "Point") -> bool:
         if isinstance(point, Point):
-            return (
-                self.x == point.x and self.y == point.y
-            )
+            return self.x == point.x and self.y == point.y
         else:
             raise NotImplementedError("Comparing Point to non-Point")
 
     @property
     def data(self) -> List[float]:
         return [self.x, self.y]
 
@@ -477,64 +456,60 @@
         return [[self.x, self.y]]
 
     def __len__(self) -> int:
         return 1
 
     @classmethod
     def from_coords(
-        cls,
-        coords: Union[Tuple[float, float], List[Tuple[float, float]]]
-    ) -> 'Point':
+        cls, coords: Union[Tuple[float, float], List[Tuple[float, float]]]
+    ) -> "Point":
         if not isinstance(coords, tuple):
             if len(coords) != 1:
                 raise ValueError("Input has more than two points")
             coords = coords[0]
         return cls(*coords)
 
     @classmethod
-    def from_list(cls, list: List[float]) -> 'Point':
+    def from_list(cls, list: List[float]) -> "Point":
         coordinates = cls.list_to_coords(list)
         return cls.from_coords(coordinates)
 
     @classmethod
     def multiple_from_dict(
         cls,
         dictionary: Union[
-            Dict[str, Union[str, float]],
-            Sequence[Dict[str, Union[str, float]]]
+            Dict[str, Union[str, float]], Sequence[Dict[str, Union[str, float]]]
         ],
         x: str,
         y: str,
-    ) -> List['Point']:
+    ) -> List["Point"]:
         coords = cls._coordinates_from_dict(dictionary, x, y)
         return [cls.from_coords(point) for point in coords]
 
     @classmethod
     def from_dict(
         cls,
         dictionary: Union[
-            Dict[str, Union[str, float]],
-            Sequence[Dict[str, Union[str, float]]]
+            Dict[str, Union[str, float]], Sequence[Dict[str, Union[str, float]]]
         ],
         x: str,
         y: str,
-    ) -> 'Point':
+    ) -> "Point":
         coords = cls._coordinates_from_dict(dictionary, x, y)
         return cls.from_coords(coords)
 
 
 @dataclass
 class Polyline(Geometry):
     """Geometry consisting of connected lines."""
-    name = 'POLYLINE'
+
+    name = "POLYLINE"
 
     def __init__(self, points: Sequence[Tuple[float, float]]):
-        self.points: List[Point] = [
-            Point(point[0], point[1]) for point in points
-        ]
+        self.points: List[Point] = [Point(point[0], point[1]) for point in points]
 
     def __len__(self) -> int:
         return len(self.points)
 
     def __repr__(self) -> str:
         return f"Polyline({self.to_coords()})"
 
@@ -559,91 +534,83 @@
                 top = point.y
             elif point.y < bottom:
                 bottom = point.y
             if point.x > right:
                 right = point.x
             elif point.y < left:
                 left = point.x
-        return RegionMm(
-            PointMm(left, bottom),
-            SizeMm(right-left, top-bottom)
-        )
+        return RegionMm(PointMm(left, bottom), SizeMm(right - left, top - bottom))
 
     @classmethod
     def from_coords(
-        cls,
-        coords: Union[Tuple[float, float], Sequence[Tuple[float, float]]]
-    ) -> 'Polyline':
+        cls, coords: Union[Tuple[float, float], Sequence[Tuple[float, float]]]
+    ) -> "Polyline":
         if isinstance(coords, tuple):
             coords = [coords]
         return cls(coords)
 
     @classmethod
     def from_dict(
         cls,
         dictionary: Union[
-            Dict[str, Union[str, float]],
-            Sequence[Dict[str, Union[str, float]]]
+            Dict[str, Union[str, float]], Sequence[Dict[str, Union[str, float]]]
         ],
         x: str,
         y: str,
-    ) -> 'Polyline':
+    ) -> "Polyline":
         coords = cls._coordinates_from_dict(dictionary, x, y)
         return cls.from_coords(coords)
 
     @classmethod
-    def from_list(cls, list: Sequence[float]) -> 'Polyline':
+    def from_list(cls, list: Sequence[float]) -> "Polyline":
         coordinates = cls.list_to_coords(list)
         return cls.from_coords(coordinates)
 
 
 @dataclass
 class Polygon(Polyline):
     """Geometry consisting of connected lines implicity closed."""
-    name = 'POLYGON'
+
+    name = "POLYGON"
 
     def __init__(self, points: Sequence[Tuple[float, float]]):
         super().__init__(points)
 
     @classmethod
     def from_coords(
-        cls,
-        coords: Union[Tuple[float, float], Sequence[Tuple[float, float]]]
-    ) -> 'Polygon':
+        cls, coords: Union[Tuple[float, float], Sequence[Tuple[float, float]]]
+    ) -> "Polygon":
         if isinstance(coords, tuple):
             coords = [coords]
         return cls(coords)
 
     @classmethod
-    def from_list(cls, list: Sequence[float]) -> 'Polygon':
+    def from_list(cls, list: Sequence[float]) -> "Polygon":
         coordinates = cls.list_to_coords(list)
         return cls.from_coords(coordinates)
 
     @classmethod
     def from_dict(
         cls,
         dictionary: Union[
-            Dict[str, Union[str, float]],
-            Sequence[Dict[str, Union[str, float]]]
+            Dict[str, Union[str, float]], Sequence[Dict[str, Union[str, float]]]
         ],
         x: str,
         y: str,
-    ) -> 'Polygon':
+    ) -> "Polygon":
         coords = cls._coordinates_from_dict(dictionary, x, y)
         return cls.from_coords(coords)
 
     def __repr__(self) -> str:
         return f"Polygon({self.to_coords()})"
 
 
 class Annotation:
     def __init__(
-        self,
-        geometry: Geometry,
-        measurements: Optional[Sequence[Measurement]] = None
+        self, geometry: Geometry, measurements: Optional[Sequence[Measurement]] = None
     ):
         """Represents an annotation, with geometry and an optional list of
         measurements.
 
         Parameters
         ----------
         geometry: Geometry
@@ -656,34 +623,31 @@
         self._measurements: Sequence[Measurement] = []
         if measurements is not None:
             self._measurements = measurements
 
     def __repr__(self) -> str:
         return f"Annotation({self.geometry}, {self.measurements})"
 
-    def __eq__(self, other: 'Annotation') -> bool:
+    def __eq__(self, other: "Annotation") -> bool:
         if not isinstance(other, Annotation):
             return NotImplemented
         return (
-            self.geometry == other.geometry and
-            self.measurements == other.measurements
+            self.geometry == other.geometry and self.measurements == other.measurements
         )
 
     @property
     def geometry(self) -> Geometry:
         return self._geometry
 
     @property
     def measurements(self) -> Sequence[Measurement]:
         return self._measurements
 
     def get_measurements(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> List[Measurement]:
         """Return measurements of specified type.
 
         Parameters
         ----------
         code: MeasurementCode
             Code of measurement type to get.
@@ -698,17 +662,15 @@
         return [
             measurement
             for measurement in self.measurements
             if measurement.same_type(code, unit)
         ]
 
     def get_measurement_values(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> List[float]:
         """Return values for measurements of specified type.
 
         Parameters
         ----------
         code: MeasurementCode
             Code of measurement type to get.
@@ -717,36 +679,37 @@
 
         Returns
         ----------
         List[Measurement]
             List of values for measurements of specified type.
         """
         return [
-            measurement.value for measurement in self.measurements
+            measurement.value
+            for measurement in self.measurements
             if measurement.same_type(code, unit)
         ]
 
 
-GeometryType = TypeVar('GeometryType', bound=Geometry)
-AnnotationGroupType = TypeVar('AnnotationGroupType', bound='AnnotationGroup')
+GeometryType = TypeVar("GeometryType", bound=Geometry)
+AnnotationGroupType = TypeVar("AnnotationGroupType", bound="AnnotationGroup")
 
 
 class AnnotationGroup(Generic[GeometryType]):
     _geometry_type: Type[Geometry]
 
     def __init__(
         self,
         annotations: Sequence[Annotation],
         label: str,
         category_code: AnnotationCategoryCode,
         type_code: AnnotationTypeCode,
         description: Optional[str] = None,
         color: Optional[LabColor] = None,
         is_double: bool = True,
-        instance: Optional[UID] = None
+        instance: Optional[UID] = None,
     ):
         """Represents a group of annotations of the same type.
 
         Parameters
         ----------
         annotations: Sequence[Annotation]
             Annotations in the group.
@@ -790,25 +753,25 @@
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}({self.annotations}, {self.label}, "
             f"{self.category_code}, {self.type_code}, "
             f"{self.description}, {self._is_double})"
         )
 
-    def __eq__(self, other: 'AnnotationGroup') -> bool:
+    def __eq__(self, other: "AnnotationGroup") -> bool:
         if not isinstance(other, AnnotationGroup):
             return NotImplemented
         return (
-            self.annotations == other.annotations and
-            self.label == other.label and
-            self.type_code == other.type_code and
-            self.category_code == other.category_code and
-            self.description == other.description and
-            self.color == other.color and
-            self._is_double == other._is_double
+            self.annotations == other.annotations
+            and self.label == other.label
+            and self.type_code == other.type_code
+            and self.category_code == other.category_code
+            and self.description == other.description
+            and self.color == other.color
+            and self._is_double == other._is_double
         )
 
     @property
     def category_code(self) -> AnnotationCategoryCode:
         return self._category_code
 
     @property
@@ -861,26 +824,23 @@
         return self._geometry_type
 
     @property
     def annotation_type(self) -> str:
         return self._geometry_type.name
 
     def __getitem__(
-        self,
-        index: Union[int, Sequence[int]]
+        self, index: Union[int, Sequence[int]]
     ) -> Union[Annotation, List[Annotation]]:
         if isinstance(index, Sequence):
             return [self.annotations[i] for i in index]
         return self.annotations[index]
 
     @classmethod
     def from_ds(
-        cls: Type[AnnotationGroupType],
-        ds: Dataset,
-        instance: UID
+        cls: Type[AnnotationGroupType], ds: Dataset, instance: UID
     ) -> AnnotationGroupType:
         """Return annotation group from Annotation Group Sequence dataset.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
@@ -891,41 +851,37 @@
         ----------
         AnnotationGroupType
             Annotation group from dataset.
         """
         is_double = cls._is_ds_double(ds)
         annotations = cls._get_annotations_from_ds(ds)
         label = cls._get_label_from_ds(ds)
-        description = getattr(ds, 'AnnotationGroupDescription', None)
+        description = getattr(ds, "AnnotationGroupDescription", None)
         type_code = AnnotationTypeCode.from_ds(ds)
         if type_code is None:
-            raise ValueError(
-                f'Dataset is missing {AnnotationTypeCode.sequence_name}.'
-            )
+            raise ValueError(f"Dataset is missing {AnnotationTypeCode.sequence_name}.")
         category_code = AnnotationCategoryCode.from_ds(ds)
         if category_code is None:
             raise ValueError(
-                f'Dataset is missing {AnnotationCategoryCode.sequence_name}.'
+                f"Dataset is missing {AnnotationCategoryCode.sequence_name}."
             )
-        color = getattr(ds, 'RecommendedDisplayCIELabValue', None)
+        color = getattr(ds, "RecommendedDisplayCIELabValue", None)
         return cls(
             annotations,
             label,
             category_code,
             type_code,
             description,
             color,
             is_double,
-            instance
+            instance,
         )
 
     @staticmethod
-    def _get_label_from_ds(
-        ds: Dataset
-    ) -> str:
+    def _get_label_from_ds(ds: Dataset) -> str:
         """Return group label from dataset.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group label.
 
@@ -933,66 +889,60 @@
         ----------
         str
             Annotation group label from dataset.
         """
         return str(ds.AnnotationGroupLabel)
 
     @staticmethod
-    def _get_focal_planes_from_ds(
-        ds: Dataset
-    ) -> List[float]:
+    def _get_focal_planes_from_ds(ds: Dataset) -> List[float]:
         """Return focal planes from dataset. If annotation applies to all focal
         planes returns empty list.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group focal planes.
 
         Returns
         ----------
         List[float]
             Annotation group focal planes from dataset.
         """
-        if ds.AnnotationAppliesToAllZPlanes == 'YES':
+        if ds.AnnotationAppliesToAllZPlanes == "YES":
             return []
         try:
             z_planes: List[float] = ds.CommonZCoordinateValue
         except AttributeError:
             raise NotImplementedError(
-                'Only 3D annotations with common z coordinate is supported'
+                "Only 3D annotations with common z coordinate is supported"
             )
         return z_planes
 
     @staticmethod
-    def _get_optical_paths_from_ds(
-        ds: Dataset
-    ) -> List[str]:
+    def _get_optical_paths_from_ds(ds: Dataset) -> List[str]:
         """Return optical paths from dataset. If annotation applies to all
         optical paths returns empty list.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group optical paths.
 
         Returns
         ----------
         List[str]
             Annotation group optical paths from dataset.
         """
-        if ds.AnnotationAppliesToAllOpticalPaths == 'YES':
+        if ds.AnnotationAppliesToAllOpticalPaths == "YES":
             return []
         optical_paths: List[str] = ds.ReferencedOpticalPathIdentifier
         return optical_paths
 
     @staticmethod
-    def _get_count_from_ds(
-        ds: Dataset
-    ) -> int:
+    def _get_count_from_ds(ds: Dataset) -> int:
         """Return number of annotations in group.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
 
@@ -1016,69 +966,60 @@
             Dataset containing measurement sequence.
 
         Returns
         ----------
         Dict[int, List[Measurement]]:
             Measurements grouped by annotation index.
         """
-        if 'MeasurementsSequence' not in ds:
+        if "MeasurementsSequence" not in ds:
             return {}
         annotation_count = cls._get_count_from_ds(ds)
         return Measurement.get_measurements_from_ds(
-            ds.MeasurementsSequence,
-            annotation_count
+            ds.MeasurementsSequence, annotation_count
         )
 
     @staticmethod
-    def _is_ds_double(
-        ds: Dataset
-    ) -> bool:
+    def _is_ds_double(ds: Dataset) -> bool:
         """Return true if group in dataset stores coordinates as double float.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
 
         Returns
         ----------
         bool
             True if group uses double float.
         """
-        return 'DoublePointCoordinatesData' in ds
+        return "DoublePointCoordinatesData" in ds
 
     @classmethod
-    def _get_coordinates_from_ds(
-        cls,
-        ds: Dataset
-    ) -> List[Tuple[float, float]]:
+    def _get_coordinates_from_ds(cls, ds: Dataset) -> List[Tuple[float, float]]:
         """Return annotation coordinates.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
 
         Returns
         ----------
         List[float]
             The coordinates for the annotations in the group.
         """
         if cls._is_ds_double(ds):
-            data = dcm_to_list(ds.DoublePointCoordinatesData, 'd')
+            data = dcm_to_list(ds.DoublePointCoordinatesData, "d")
         else:
-            data = dcm_to_list(ds.PointCoordinatesData, 'f')
+            data = dcm_to_list(ds.PointCoordinatesData, "f")
         return Geometry.list_to_coords(data)
 
     @classmethod
     @abstractmethod
-    def _get_geometries_from_ds(
-        cls,
-        ds: Dataset
-    ) -> List[Geometry]:
+    def _get_geometries_from_ds(cls, ds: Dataset) -> List[Geometry]:
         """Abstract method for getting geometries from dataset.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
 
@@ -1086,18 +1027,15 @@
         ----------
         List[Geometry]
             Geometries in the annotation group.
         """
         raise NotImplementedError()
 
     @classmethod
-    def _get_annotations_from_ds(
-        cls,
-        ds: Dataset
-    ) -> List[Annotation]:
+    def _get_annotations_from_ds(cls, ds: Dataset) -> List[Annotation]:
         """Return annotation coordinates.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
 
@@ -1127,17 +1065,15 @@
         for annotation in self.annotations:
             for measurement in annotation.measurements:
                 pair = (measurement.code, measurement.unit)
                 pairs.add(pair)
         return list(pairs)
 
     def get_measurements(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> List[Measurement]:
         """Return measurements of specified code-unit-pair.
 
         Parameters
         ----------
         code: MeasurementCode
             Type of measurement type to get.
@@ -1151,17 +1087,15 @@
         """
         measurements: List[Measurement] = []
         for annotation in self.annotations:
             measurements += annotation.get_measurements(code, unit)
         return measurements
 
     def create_measurement_indices(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> np.ndarray:
         """Return measurement indicies for all measurements of specified type.
         Indices are stored starting at index 1.
 
         Parameters
         ----------
         code: MeasurementCode
@@ -1176,17 +1110,15 @@
         """
         indices: List[int] = []
         for i, annotation in enumerate(self.annotations):
             indices += [i + 1] * len(annotation.get_measurements(code, unit))
         return np.array(indices, dtype=np.int32)
 
     def _create_measurement_values(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> np.ndarray:
         """Return measurement values for all measurements of specified type.
 
         Parameters
         ----------
         code: MeasurementCode
             Code of measurement type to create.
@@ -1200,17 +1132,15 @@
         """
         values: List[float] = []
         for annotation in self.annotations:
             values += annotation.get_measurement_values(code, unit)
         return np.array(values, dtype=np.float32)
 
     def _measurements_is_one_to_one(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> bool:
         """Check if all annotations in group have strictly one measurement
         of specified type-unit-pair.
 
         Parameters
         ----------
         code: MeasurementCode
@@ -1226,17 +1156,15 @@
         """
         for annotation in self.annotations:
             if not len(annotation.get_measurements(code, unit)) == 1:
                 return False
         return True
 
     def _create_measurement_value_sequence(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> DicomSequence:
         """Return Measurement Value Sequence of measurements of specified
         code and unit.
 
         Parameters
         ----------
         code: MeasurementCode
@@ -1257,17 +1185,15 @@
             measurements_ds.AnnotationIndexList = indices
         values = self._create_measurement_values(code, unit)
         measurements_ds.FloatingPointValues = values
         measurement_value_sequence = DicomSequence([measurements_ds])
         return measurement_value_sequence
 
     def _create_measurement_sequence_item(
-        self,
-        code: MeasurementCode,
-        unit: UnitCode
+        self, code: MeasurementCode, unit: UnitCode
     ) -> Dataset:
         """Return Measurement Sequence item of measurements of specified code
         and unit.
 
         Parameters
         ----------
         code: MeasurementCode
@@ -1285,66 +1211,57 @@
         ds.MeasurementValuesSequence = self._create_measurement_value_sequence(
             code, unit
         )
         code.insert_into_ds(ds)
         unit.insert_into_ds(ds)
         return ds
 
-    def _set_planes_in_ds(
-        self,
-        ds: Dataset
-    ) -> Dataset:
+    def _set_planes_in_ds(self, ds: Dataset) -> Dataset:
         """Insert the group focal plane attributes into the Annotation Group
         Sequence.
 
         Parameters
         ----------
         ds: Dataset
             The Annotation Group Sequence.
 
         Returns
         ----------
         Dataset
             The Annotation Group Sequence with focal plane attributes.
         """
         if self._z_planes is []:
-            ds.AnnotationAppliesToAllZPlanes = 'YES'
+            ds.AnnotationAppliesToAllZPlanes = "YES"
         else:
-            ds.AnnotationAppliesToAllZPlanes = 'NO'
+            ds.AnnotationAppliesToAllZPlanes = "NO"
             ds.CommonZCoordinateValue = self._z_planes
         return ds
 
-    def _set_optical_paths_in_ds(
-        self,
-        ds: Dataset
-    ) -> Dataset:
+    def _set_optical_paths_in_ds(self, ds: Dataset) -> Dataset:
         """Insert the group optical path attributes into the Annotation Group
         Sequence.
 
         Parameters
         ----------
         ds: Dataset
             The Annotation Group Sequence.
 
         Returns
         ----------
         Dataset
             The Annotation Group Sequence with optical path attributes.
         """
         if self._optical_paths is []:
-            ds.AnnotationAppliesToAllOpticalPaths = 'YES'
+            ds.AnnotationAppliesToAllOpticalPaths = "YES"
         else:
-            ds.AnnotationAppliesToAllOpticalPaths = 'NO'
+            ds.AnnotationAppliesToAllOpticalPaths = "NO"
             ds.ReferencedOpticalPathIdentifier = self._optical_paths
         return ds
 
-    def _set_coordinates_data_in_ds(
-        self,
-        ds: Dataset
-    ) -> Dataset:
+    def _set_coordinates_data_in_ds(self, ds: Dataset) -> Dataset:
         """Insert the group point coordinates into the Annotation Group
         Sequence.
 
         Parameters
         ----------
         ds: Dataset
             The Annotation Group Sequence.
@@ -1356,35 +1273,30 @@
         """
         if self._is_double:
             ds.DoublePointCoordinatesData = self.point_coordinates_data
         else:
             ds.PointCoordinatesData = self.point_coordinates_data
         return ds
 
-    def _set_measurement_sequence_in_ds(
-        self,
-        ds: Dataset
-    ) -> Dataset:
+    def _set_measurement_sequence_in_ds(self, ds: Dataset) -> Dataset:
         """Insert group measurements into the Annotation Group Sequence.
 
         Parameters
         ----------
         ds: Dataset
             The Annotation Group Sequence.
 
         Returns
         ----------
         Dataset
             The Annotation Group Sequence with inserted measurements.
         """
         ds.MeasurementsSequence = DicomSequence(
             [
-                self._create_measurement_sequence_item(
-                    *measurement_type
-                )
+                self._create_measurement_sequence_item(*measurement_type)
                 for measurement_type in self.measurement_types
             ]
         )
         return ds
 
     def to_ds(self, group_number: int) -> Dataset:
         """Return annotation group as a Annotation Group Sequence
@@ -1414,41 +1326,37 @@
         ds = self._set_planes_in_ds(ds)
         ds = self._set_optical_paths_in_ds(ds)
         ds = self._set_measurement_sequence_in_ds(ds)
         if self.color is not None:
             ds.RecommendedDisplayCIELabValue = self.color
         # AUTOMATIC and SEMIAUTOMATIC requires a
         # Annotation Algorithm Identification Sequence
-        ds.AnnotationGroupGenerationType = 'MANUAL'
+        ds.AnnotationGroupGenerationType = "MANUAL"
         return ds
 
     @classmethod
-    def validate_type(
-        cls,
-        annotations: Sequence[Annotation]
-    ):
+    def validate_type(cls, annotations: Sequence[Annotation]):
         """Check that list of annotations are of the requested type.
 
         Parameters
         ----------
         annotations: Sequence[Annotation]
             List of annotations to check
         """
         for annotation in annotations:
             if not isinstance(annotation.geometry, cls._geometry_type):
                 raise TypeError(
-                    f'annotation type {type(annotation.geometry)}'
-                    f' does not match Group type code {cls._geometry_type}'
+                    f"annotation type {type(annotation.geometry)}"
+                    f" does not match Group type code {cls._geometry_type}"
                 )
 
     @classmethod
     def _get_group_type_by_geometry(
-        cls,
-        geometry_type: Type[Geometry]
-    ) -> Type['AnnotationGroup']:
+        cls, geometry_type: Type[Geometry]
+    ) -> Type["AnnotationGroup"]:
         """Return AnnotationGroup class for geometry type.
 
         Parameters
         ----------
         geometry_type: type
             The geometry type to get AnnotationGroup class for.
 
@@ -1464,16 +1372,16 @@
     @classmethod
     def from_geometries(
         cls,
         geometries: Sequence[Geometry],
         label: str,
         category_code: AnnotationCategoryCode,
         type_code: AnnotationTypeCode,
-        is_double: bool = True
-    ) -> 'AnnotationGroup':
+        is_double: bool = True,
+    ) -> "AnnotationGroup":
         """Return AnnotationGroup created from list of geometries. The group
         type is determined by the first geometry, and all geometries needs to
         have the same type.
 
         Parameters
         ----------
         geometries: Sequence[Geometries]
@@ -1494,44 +1402,40 @@
         geometry_type = type(geometries[0])
         group_type = cls._get_group_type_by_geometry(geometry_type)
         group: AnnotationGroup = group_type(
             annotations=[Annotation(geometry) for geometry in geometries],
             label=label,
             category_code=category_code,
             type_code=type_code,
-            is_double=is_double
+            is_double=is_double,
         )
         return group
 
 
 class PointAnnotationGroup(AnnotationGroup[Point]):
     """Point annotation group"""
+
     _geometry_type = Point
 
     @classmethod
-    def _get_geometries_from_ds(
-        cls,
-        ds: Dataset
-    ) -> List[Point]:
+    def _get_geometries_from_ds(cls, ds: Dataset) -> List[Point]:
         """Returns point geometries from dataset.
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
 
         Returns
         ----------
         List[Geometry]
             Point geometries in the annotation group.
         """
         coordinate_list = cls._get_coordinates_from_ds(ds)
-        points = [
-            Point.from_coords(coordinates) for coordinates in coordinate_list
-        ]
+        points = [Point.from_coords(coordinates) for coordinates in coordinate_list]
         return points
 
 
 class PolylineAnnotationGroupMeta(AnnotationGroup[GeometryType]):
     """Meta class for line annotation goup"""
 
     @property
@@ -1548,17 +1452,15 @@
         indices: List[int] = []
         for annotation in self.annotations:
             indices.append(index)
             index += len(annotation.geometry.data)
         return np.array(indices, dtype=np.int32)
 
     @staticmethod
-    def _get_indices_from_ds(
-        ds: Dataset
-    ) -> List[int]:
+    def _get_indices_from_ds(ds: Dataset) -> List[int]:
         """Return line start indices from sup 222 dataset. Indices are stored
         starting at with value 1, and are in relation to non-pared coordinates.
         Returned list starts at 0 and is in relation to paired coordinates.
 
         Parameters
         ----------
         ds: Dataset
@@ -1566,24 +1468,20 @@
 
         Returns
         ----------
         List[int]
             List of indices in dataset.
         """
         return [
-            (value - 1)//2
-            for value
-            in dcm_to_list(ds.LongPrimitivePointIndexList, 'l')
+            (value - 1) // 2
+            for value in dcm_to_list(ds.LongPrimitivePointIndexList, "l")
         ]
 
     @classmethod
-    def _get_geometries_from_ds(
-        cls,
-        ds: Dataset
-    ) -> List[GeometryType]:
+    def _get_geometries_from_ds(cls, ds: Dataset) -> List[GeometryType]:
         """Returns line geometries from dataset. Each line geometry consists of
         multiple points, and the first coordinate in the coordinate list is
 
         Parameters
         ----------
         ds: Dataset
             Dataset containing annotation group.
@@ -1600,15 +1498,15 @@
                 "Number of indices must be the same as number of geometries"
             )
         coordinates = cls._get_coordinates_from_ds(ds)
         indices += [len(coordinates)]  # Add end for last geometry
         geometries: List[GeometryType] = []
         for index in range(number_of_geometries):
             start = indices[index]
-            end = indices[index+1]
+            end = indices[index + 1]
             line_coordinates = coordinates[start:end]
             lines = cls._get_line_geometry_from_coords(line_coordinates)
             geometries.append(lines)
         return geometries
 
     @staticmethod
     @abstractmethod
@@ -1654,53 +1552,51 @@
 class AnnotationInstance:
     """Class for handling microscope bulk simple annotations according to
     sup-222. Point, polyline, and polygon graphic types are implemented,
     ellipse and rectangle graphic types are not implemented. Annotation must
     have common z-coordinate or apply to all z planes (annotation with 3D
     PointCoordinateData is not implemented.)
     """
+
     def __init__(
         self,
         groups: Sequence[AnnotationGroup],
         coordinate_type: str,
-        slide_uids: SlideUids
+        slide_uids: SlideUids,
     ):
         """Represents a collection of annotation groups.
 
         Parameters
         ----------
         annotations: Sequence[AnnotationGroup]
             List of annotations group
         coordinate_type: str
             If coordinates are volume-related ('volume') or image-related
             ('image').
         frame_of_referenc: Uid
             Frame of reference uid of image that the annotations belong to
         """
         self.groups = groups
-        if coordinate_type not in ['image', 'volume']:
+        if coordinate_type not in ["image", "volume"]:
             raise ValueError("Coordiante type should be 'image' or 'volume'")
         self.coordinate_type = coordinate_type
         self.slide_uids = slide_uids
         self.datetime = datetime.now()
-        self.modality = 'ANN'
+        self.modality = "ANN"
         self.series_number: int
 
     def __repr__(self) -> str:
-        return (
-            f"AnnotationInstance({self.groups}, "
-            f"{self.slide_uids})"
-        )
+        return f"AnnotationInstance({self.groups}, " f"{self.slide_uids})"
 
     def save(
         self,
         path: Union[str, Path],
         little_endian: bool = True,
         implicit_vr: bool = False,
-        uid_generator: Callable[..., UID] = generate_uid
+        uid_generator: Callable[..., UID] = generate_uid,
     ):
         """Write annotations to DICOM file according to sup 222.
         Note that the file will miss DICOM attributes that has not yet been
         implemented.
 
         Parameters
         ----------
@@ -1712,25 +1608,25 @@
             Write DICOM file with implicit value representation
         """
         ds = Dataset()
         ds.is_little_endian = little_endian
         ds.is_implicit_VR = implicit_vr
         bulk_sequence = DicomSequence()
         for index, annotation_group in enumerate(self.groups):
-            if(isinstance(annotation_group, AnnotationGroup)):
-                bulk_sequence.append(annotation_group.to_ds(index+1))
+            if isinstance(annotation_group, AnnotationGroup):
+                bulk_sequence.append(annotation_group.to_ds(index + 1))
             else:
                 raise NotImplementedError(
                     f"Group type: {type(annotation_group)} not supported"
                 )
         ds.AnnotationGroupSequence = bulk_sequence
-        if self.coordinate_type == 'image':
-            ds.AnnotationCoordinateType = '2D'
-        elif self.coordinate_type == 'volume':
-            ds.AnnotationCoordinateType = '3D'
+        if self.coordinate_type == "image":
+            ds.AnnotationCoordinateType = "2D"
+        elif self.coordinate_type == "volume":
+            ds.AnnotationCoordinateType = "3D"
         if self.slide_uids.frame_of_reference is not None:
             ds.FrameOfReferenceUID = self.slide_uids.frame_of_reference
         ds.StudyInstanceUID = self.slide_uids.study_instance
         ds.SeriesInstanceUID = self.slide_uids.series_instance
         ds.SOPInstanceUID = uid_generator()
         ds.SOPClassUID = ANN_SOP_CLASS_UID
 
@@ -1746,44 +1642,43 @@
 
         meta_ds.TransferSyntaxUID = transfer_syntax
         meta_ds.MediaStorageSOPInstanceUID = ds.SOPInstanceUID
         meta_ds.MediaStorageSOPClassUID = ANN_SOP_CLASS_UID
         meta_ds.FileMetaInformationGroupLength = 0  # Updated on write
         validate_file_meta(meta_ds)
         file_ds = FileDataset(
-            preamble=b'\x00' * 128,
+            preamble=b"\x00" * 128,
             filename_or_obj=path,
             file_meta=meta_ds,
             dataset=ds,
             is_implicit_VR=implicit_vr,
-            is_little_endian=little_endian
+            is_little_endian=little_endian,
         )
         dcmwrite(path, file_ds)
 
     @classmethod
     def open(
-        cls,
-        paths: Union[Sequence[str], Sequence[Path]]
-    ) -> List['AnnotationInstance']:
+        cls, paths: Union[Sequence[str], Sequence[Path]]
+    ) -> List["AnnotationInstance"]:
         """Read annotations from DICOM file according to sup 222.
 
         Parameters
         ----------
         paths: Sequence[str]
             Paths to DICOM annotation files to read.
         """
-        instances: List['AnnotationInstance'] = []
+        instances: List["AnnotationInstance"] = []
         for path in paths:
             ds = dcmread(path)
             instances.append(cls.open_dataset(ds))
 
         return instances
 
     @classmethod
-    def open_dataset(cls, dataset: Dataset) -> 'AnnotationInstance':
+    def open_dataset(cls, dataset: Dataset) -> "AnnotationInstance":
         """Read annotations from DICOM dataset according to sup 222.
 
         Parameters
         ----------
         dataset: Dataset
             DICOM annotation dataset to read.
 
@@ -1793,58 +1688,55 @@
             Annotation groups read from dataset.
         """
         groups: List[AnnotationGroup] = []
         slide_uids: Optional[SlideUids] = None
 
         if dataset.file_meta.MediaStorageSOPClassUID != ANN_SOP_CLASS_UID:
             raise ValueError("SOP Class UID of file is wrong")
-        frame_of_reference_uid = getattr(dataset, 'FrameOfReferenceUID', None)
-        if dataset.AnnotationCoordinateType == '2D':
-            coordinate_type = 'image'
-        elif dataset.AnnotationCoordinateType == '3D':
-            coordinate_type = 'volume'
+        frame_of_reference_uid = getattr(dataset, "FrameOfReferenceUID", None)
+        if dataset.AnnotationCoordinateType == "2D":
+            coordinate_type = "image"
+        elif dataset.AnnotationCoordinateType == "3D":
+            coordinate_type = "volume"
         else:
             raise ValueError("Unkown coordiante type")
-        if coordinate_type == 'volume' and frame_of_reference_uid is None:
+        if coordinate_type == "volume" and frame_of_reference_uid is None:
             raise ValueError(
-                'volume annotation corrindate type requires frame of reference'
+                "volume annotation corrindate type requires frame of reference"
             )
 
         instance = dataset.SOPInstanceUID
         if slide_uids is None:
             slide_uids = SlideUids(
                 dataset.StudyInstanceUID,
                 dataset.SeriesInstanceUID,
-                frame_of_reference_uid
+                frame_of_reference_uid,
             )
         else:
             if slide_uids != SlideUids(
                 dataset.StudyInstanceUID,
                 dataset.SeriesInstanceUID,
-                frame_of_reference_uid
+                frame_of_reference_uid,
             ):
                 raise ValueError("Base uids should match")
         for annotation_ds in dataset.AnnotationGroupSequence:
             annotation_type = annotation_ds.GraphicType
-            if(annotation_type == 'POINT'):
+            if annotation_type == "POINT":
                 annotation_class = PointAnnotationGroup
-            elif(annotation_type == 'POLYLINE'):
+            elif annotation_type == "POLYLINE":
                 annotation_class = PolylineAnnotationGroup
-            elif(annotation_type == 'POLYGON'):
+            elif annotation_type == "POLYGON":
                 annotation_class = PolygonAnnotationGroup
             else:
                 raise NotImplementedError("Unsupported Graphic type")
             annotation = annotation_class.from_ds(annotation_ds, instance)
             groups.append(annotation)
         return cls(groups, coordinate_type, slide_uids)
 
-    def __getitem__(
-        self,
-        index: int
-    ) -> AnnotationGroup:
+    def __getitem__(self, index: int) -> AnnotationGroup:
         """Return annotation group by index (group number).
 
         Parameters
         ----------
         index: int
             Group number of group to return
```

### Comparing `wsidicom-0.8.0/wsidicom/image_data/__init__.py` & `wsidicom-0.9.0/wsidicom/group/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,8 +8,11 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-from wsidicom.image_data.image_data import ImageData, ImageOrigin
+"""Module for handling group of instances, such as a level."""
+
+from wsidicom.group.group import Group
+from wsidicom.group.level import Level
```

### Comparing `wsidicom-0.8.0/wsidicom/image_data/dicom_image_data.py` & `wsidicom-0.9.0/wsidicom/instance/image_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,722 +10,602 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import io
 from abc import ABCMeta, abstractmethod
-from pathlib import Path
-from typing import (Dict, List, Optional, OrderedDict, Sequence, Set, Tuple,
-                    Union)
+from concurrent.futures import ThreadPoolExecutor
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 
-import numpy as np
 from PIL import Image
 from PIL.Image import Image as PILImage
-from pydicom.dataset import Dataset
-from pydicom.sequence import Sequence as DicomSequence
-from pydicom.uid import UID
+from pydicom.uid import JPEG2000, UID, JPEG2000Lossless, JPEGBaseline8Bit
 
-from wsidicom.errors import WsiDicomNotFoundError, WsiDicomOutOfBoundsError
-from wsidicom.file import WsiDicomFile
+from wsidicom.config import settings
+from wsidicom.errors import WsiDicomOutOfBoundsError
 from wsidicom.geometry import Point, Region, Size, SizeMm
-from wsidicom.image_data import ImageData, ImageOrigin
+from wsidicom.instance.image_origin import ImageOrigin
 
 
-class WsiDicomImageData(ImageData):
-    """Represents image data read from dicom file(s). Image data can
-    be sparsly or fully tiled and/or concatenated."""
-    def __init__(
-        self,
-        files: Union[WsiDicomFile, Sequence[WsiDicomFile]]
-    ) -> None:
-        """Create WsiDicomImageData from frame data in files.
-
-        Parameters
-        ----------
-        files: Union[WsiDicomFile, Sequence[WsiDicomFile]]
-            Single or list of WsiDicomFiles containing frame data.
-        """
-        if not isinstance(files, Sequence):
-            files = [files]
+class ImageData(metaclass=ABCMeta):
+    """Generic class for image data that can be inherited to implement support
+    for other image/file formats. Subclasses should implement properties to get
+    transfer_syntax, image_size, tile_size, pixel_spacing,  samples_per_pixel,
+    and photometric_interpretation and methods get_tile() and close().
+    Additionally properties focal_planes and/or optical_paths should be
+    overridden if multiple focal planes or optical paths are implemented."""
+
+    _default_z: Optional[float] = None
+    _blank_tile: Optional[PILImage] = None
+    _encoded_blank_tile: Optional[bytes] = None
 
-        # Key is frame offset
-        self._files = OrderedDict(
-            (file.frame_offset, file) for file
-            in sorted(files, key=lambda file: file.frame_offset)
-        )
+    @property
+    @abstractmethod
+    def transfer_syntax(self) -> UID:
+        """Should return the uid of the transfer syntax of the image."""
+        raise NotImplementedError()
 
-        base_file = files[0]
-        datasets = [file.dataset for file in self._files.values()]
-        if base_file.dataset.tile_type == 'TILED_FULL':
-            self.tiles = FullTileIndex(datasets)
-        else:
-            self.tiles = SparseTileIndex(datasets)
+    @property
+    @abstractmethod
+    def image_size(self) -> Size:
+        """Should return the pixel size of the image."""
+        raise NotImplementedError()
 
-        self._pixel_spacing = datasets[0].pixel_spacing
-        self._transfer_syntax = base_file.transfer_syntax
-        self._default_z: Optional[float] = None
-        self._photometric_interpretation = (
-            datasets[0].photometric_interpretation
-        )
-        self._samples_per_pixel = datasets[0].samples_per_pixel
-        self._image_origin = ImageOrigin.from_dataset(datasets[0])
+    @property
+    @abstractmethod
+    def tile_size(self) -> Size:
+        """Should return the pixel tile size of the image, or pixel size of
+        the image if not tiled."""
+        raise NotImplementedError()
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}({self._files.values()})"
+    @property
+    @abstractmethod
+    def pixel_spacing(self) -> Optional[SizeMm]:
+        """Should return the size of the pixels in mm/pixel."""
+        raise NotImplementedError()
 
-    def __str__(self) -> str:
-        return f"{type(self).__name__} of files {self._files.values()}"
+    @property
+    @abstractmethod
+    def samples_per_pixel(self) -> int:
+        """Should return number of samples per pixel (e.g. 3 for RGB)."""
+        raise NotImplementedError()
 
     @property
-    def files(self) -> List[Path]:
-        return [file.filepath for file in self._files.values()]
+    @abstractmethod
+    def photometric_interpretation(self) -> str:
+        """Should return the photophotometric interpretation of the image
+        data."""
+        raise NotImplementedError()
 
     @property
-    def transfer_syntax(self) -> UID:
-        """The uid of the transfer syntax of the image."""
-        return self._transfer_syntax
+    @abstractmethod
+    def image_origin(self) -> ImageOrigin:
+        """Should return the image origin of the image data."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _get_decoded_tile(self, tile_point: Point, z: float, path: str) -> PILImage:
+        """Should return Image for tile defined by tile (x, y), z,
+        and optical path."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _get_encoded_tile(self, tile: Point, z: float, path: str) -> bytes:
+        """Should return image bytes for tile defined by tile (x, y), z,
+        and optical path."""
+        raise NotImplementedError()
 
     @property
-    def image_size(self) -> Size:
-        """The pixel size of the image."""
-        return self.tiles.image_size
+    def tiled_size(self) -> Size:
+        """The size of the image when divided into tiles, e.g. number of
+        columns and rows of tiles. Equals (1, 1) if image is not tiled."""
+        return self.image_size.ceil_div(self.tile_size)
 
     @property
-    def tile_size(self) -> Size:
-        """The pixel tile size of the image."""
-        return self.tiles.tile_size
+    def image_region(self) -> Region:
+        return Region(Point(0, 0), self.image_size)
 
     @property
     def focal_planes(self) -> List[float]:
         """Focal planes avaiable in the image defined in um."""
-        return self.tiles.focal_planes
+        return [0.0]
 
     @property
     def optical_paths(self) -> List[str]:
         """Optical paths avaiable in the image."""
-        return self.tiles.optical_paths
+        return ["0"]
 
     @property
-    def pixel_spacing(self) -> Optional[SizeMm]:
-        """Size of the pixels in mm/pixel."""
-        return self._pixel_spacing
+    def image_mode(self) -> str:
+        """Return Pillow image mode (e.g. RGB) for image data"""
+        if self.samples_per_pixel == 1:
+            return "L"
+        elif self.samples_per_pixel == 3:
+            return "RGB"
+        raise NotImplementedError()
 
     @property
-    def photometric_interpretation(self) -> str:
-        """Return photometric interpretation."""
-        return self._photometric_interpretation
+    def blank_color(self) -> Tuple[int, int, int]:
+        """Return RGB background color."""
+        return self._get_blank_color(self.photometric_interpretation)
+
+    def pretty_str(self, indent: int = 0, depth: Optional[int] = None) -> str:
+        return str(self)
+
+    @property
+    def default_z(self) -> float:
+        """Return single defined focal plane (in um) if only one focal plane
+        defined. Return the middle focal plane if several focal planes are
+        defined."""
+        if self._default_z is None:
+            default = 0
+            if len(self.focal_planes) > 1:
+                smallest = min(self.focal_planes)
+                largest = max(self.focal_planes)
+                middle = (largest - smallest) / 2
+                default = min(
+                    range(len(self.focal_planes)),
+                    key=lambda i: abs(self.focal_planes[i] - middle),
+                )
+
+            self._default_z = self.focal_planes[default]
+
+        return self._default_z
 
     @property
-    def samples_per_pixel(self) -> int:
-        """Return samples per pixel (1 or 3)."""
-        return self._samples_per_pixel
+    def default_path(self) -> str:
+        """Return the first defined optical path as default optical path
+        identifier."""
+        return self.optical_paths[0]
 
     @property
-    def image_origin(self) -> ImageOrigin:
-        return self._image_origin
+    def plane_region(self) -> Region:
+        return Region(position=Point(0, 0), size=self.tiled_size)
 
-    def _get_encoded_tile(self, tile: Point, z: float, path: str) -> bytes:
-        frame_index = self._get_frame_index(tile, z, path)
-        if frame_index == -1:
-            return self.blank_encoded_tile
-        return self._get_tile_frame(frame_index)
+    @property
+    def blank_tile(self) -> PILImage:
+        """Return background tile."""
+        if self._blank_tile is None:
+            self._blank_tile = self._create_blank_tile()
+        return self._blank_tile
 
-    def _get_decoded_tile(
-        self,
-        tile_point: Point,
-        z: float,
-        path: str
-    ) -> PILImage:
-        frame_index = self._get_frame_index(tile_point, z, path)
-        if frame_index == -1:
-            return self.blank_tile
-        frame = self._get_tile_frame(frame_index)
-        return Image.open(io.BytesIO(frame))
+    @property
+    def blank_encoded_tile(self) -> bytes:
+        """Return encoded background tile."""
+        if self._encoded_blank_tile is None:
+            self._encoded_blank_tile = self.encode(self.blank_tile)
+        return self._encoded_blank_tile
 
-    def _get_file(self, frame_index: int) -> WsiDicomFile:
-        """Return file contaning frame index. Raises WsiDicomNotFoundError if
-        frame is not found.
+    def get_decoded_tiles(
+        self, tiles: Iterable[Point], z: float, path: str
+    ) -> List[PILImage]:
+        """Return tiles for tile defined by tile (x, y), z, and optical
+        path.
 
         Parameters
         ----------
-        frame_index: int
-             Frame index to get
+        tiles: Iterable[Point]
+            Tiles to get.
+        z: float
+            Z coordinate.
+        path: str
+            Optical path.
 
         Returns
         ----------
-        WsiDicomFile
-            File containing the frame
+        List[PILImage]
+            Tiles as Images.
         """
-        for frame_offset, file in self._files.items():
-            if (frame_index < frame_offset + file.frame_count and
-                    frame_index >= frame_offset):
-                return file
-
-        raise WsiDicomNotFoundError(f"Frame index {frame_index}", "instance")
+        return [self._get_decoded_tile(tile, z, path) for tile in tiles]
 
-    def _get_tile_frame(self, frame_index: int) -> bytes:
-        """Return tile frame for frame index.
+    def get_encoded_tiles(
+        self, tiles: Iterable[Point], z: float, path: str
+    ) -> List[bytes]:
+        """Return tiles for tile defined by tile (x, y), z, and optical
+        path.
 
         Parameters
         ----------
-        frame_index: int
-             Frame index to get
+        tiles: Iterable[Point]
+            Tiles to get.
+        z: float
+            Z coordinate.
+        path: str
+            Optical path.
 
         Returns
         ----------
-        bytes
-            The frame in bytes
+        List[bytes]
+            Tiles in bytes.
         """
-        file = self._get_file(frame_index)
-        tile_frame = file.read_frame(frame_index)
-        return tile_frame
+        return [self._get_encoded_tile(tile, z, path) for tile in tiles]
 
-    def _get_frame_index(self, tile: Point, z: float, path: str) -> int:
-        """Return frame index for tile. Raises WsiDicomOutOfBoundsError if
-        tile, z, or path is not valid.
+    def get_scaled_tile(
+        self,
+        scaled_tile_point: Point,
+        z: float,
+        path: str,
+        scale: int,
+        workers: int = 1,
+    ) -> PILImage:
+        """Return scaled tile defined by tile (x, y), z, optical
+        path and scale.
 
         Parameters
         ----------
-        tile: Point
-             Tile coordinate
+        scaled_tile_point: Point,
+            Scaled position of tile to get.
         z: float
-            Z coordinate
+            Z coordinate.
         path: str
-            Optical identifier
+            Optical path.
+        scale: int
+            Scale to use for downscaling.
+        workers: int = 1
+            Workers to use for threading. Default to not use threading as method is
+            likely already used in a threading context.
 
         Returns
         ----------
-        int
-            Tile frame index
-        """
-        tile_region = Region(position=tile, size=Size(0, 0))
-        if not self.valid_tiles(tile_region, z, path):
-            raise WsiDicomOutOfBoundsError(
-                f"Tile region {tile_region}",
-                f"plane {self.tiles.tiled_size}"
-            )
-        frame_index = self.tiles.get_frame_index(tile, z, path)
-        return frame_index
-
-    def is_sparse(self, tile: Point, z: float, path: str) -> bool:
-        return (self.tiles.get_frame_index(tile, z, path) == -1)
-
-    def close(self) -> None:
-        for file in self._files.values():
-            file.close()
-
-
-class SparseTilePlane:
-    """Hold frame indices for the tiles in a sparse tiled file. Empty (sparse)
-    frames are represented by -1."""
-    def __init__(self, tiled_size: Size):
-        """Create a SparseTilePlane of specified size.
-
-        Parameters
-        ----------
-        tiled_size: Size
-            Size of the tiling
-        """
-        self._shape = tiled_size
-        self.plane = np.full(tiled_size.to_tuple(), -1, dtype=np.dtype(int))
+        PILImage
+            Scaled tiled as Image.
+        """
+        image = Image.new(
+            mode=self.image_mode,
+            size=(self.tile_size * scale).to_tuple(),
+            color=self.blank_color[: self.samples_per_pixel],
+        )
+        # Get decoded tiles for the region covering the scaled tile
+        # in the image data
+        tile_points = Region(scaled_tile_point * scale, Size(1, 1) * scale)
+
+        def tile_paste(tile_point: Point) -> None:
+            if (tile_point.x < self.tiled_size.width) and (
+                tile_point.y < self.tiled_size.height
+            ):
+                tile = self._get_decoded_tile(tile_point, z, path)
+                image_coordinate = (tile_point - tile_points.start) * self.tile_size
+                image.paste(tile, image_coordinate.to_tuple())
 
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}({self._shape})"
+        self._paste_tiles(tile_points, tile_paste, workers)
 
-    def __str__(self) -> str:
-        return self.pretty_str()
+        return image.resize(
+            self.tile_size.to_tuple(), resample=Image.Resampling.BILINEAR
+        )
 
-    def __getitem__(self, position: Point) -> int:
-        """Get frame index from tile index at plane_position.
+    def get_scaled_encoded_tile(
+        self,
+        scaled_tile_point: Point,
+        z: float,
+        path: str,
+        scale: int,
+        image_format: str,
+        image_options: Dict[str, Any],
+    ) -> bytes:
+        """Return scaled encoded tile defined by tile (x, y), z, optical
+        path and scale.
 
         Parameters
         ----------
-        plane_position: Point
-            Position in plane to get the frame index from
+        scaled_tile_point: Point,
+            Scaled position of tile to get.
+        z: float
+            Z coordinate.
+        path: str
+            Optical path.
+        Scale: int
+            Scale to use for downscaling.
+        image_format: str
+            Image format, e.g. 'JPEG', for encoding.
+        image_options: Dict[str, Any].
+            Dictionary of options for encoding.
 
         Returns
         ----------
-        int
-            Frame index
-        """
-        frame_index = int(self.plane[position.x, position.y])
-        return frame_index
-
-    def __setitem__(self, position: Point, frame_index: int):
-        """Add frame index to tile index.
-
-        Parameters
-        ----------
-        plane_position: Point
-            Position in plane to add the frame index
-        frame_index: int
-            Frame index to add to the index
+        bytes
+            Scaled tile as bytes.
         """
-        self.plane[position.x, position.y] = frame_index
-
-    def pretty_str(
-        self,
-        indent: int = 0,
-        depth: Optional[int] = None
-    ) -> str:
-        return "Sparse tile plane"
-
+        image = self.get_scaled_tile(scaled_tile_point, z, path, scale)
+        with io.BytesIO() as buffer:
+            image.save(buffer, format=image_format, **image_options)
+            return buffer.getvalue()
 
-class TileIndex(metaclass=ABCMeta):
-    """Index for mapping tile position to frame number. Is subclassed into
-    FullTileIndex and SparseTileIndex."""
-    def __init__(
+    def get_scaled_encoded_tiles(
         self,
-        datasets: Sequence[Dataset]
-    ):
-        """Create tile index for frames in datasets. Requires equal tile
-        size for all tile planes.
-
-        Parameters
-        ----------
-        datasets: Sequence[Dataset]
-            List of datasets containing tiled image data.
-
-        """
-        base_dataset = datasets[0]
-        self._image_size = base_dataset.image_size
-        self._tile_size = base_dataset.tile_size
-        self._frame_count = self._read_frame_count_from_datasets(datasets)
-        self._optical_paths = self._read_optical_paths_from_datasets(datasets)
-        self._tiled_size = self.image_size.ceil_div(self.tile_size)
-
-    def __str__(self) -> str:
-        return (
-            f"{type(self).__name__} with image size {self.image_size}, "
-            f"tile size {self.tile_size}, tiled size {self.tiled_size}, "
-            f"optical paths {self.optical_paths}, "
-            f"focal planes {self.focal_planes}, "
-            f"and frame count {self.frame_count}"
-        )
-
-    @property
-    @abstractmethod
-    def focal_planes(self) -> List[float]:
-        """Return list of focal planes in index."""
-        raise NotImplementedError()
-
-    @property
-    def image_size(self) -> Size:
-        """Return image size in pixels."""
-        return self._image_size
-
-    @property
-    def tile_size(self) -> Size:
-        """Return tile size in pixels."""
-        return self._tile_size
-
-    @property
-    def tiled_size(self) -> Size:
-        """Return size of tiling (columns x rows)."""
-        return self._tiled_size
-
-    @property
-    def frame_count(self) -> int:
-        """Return total number of frames in index."""
-        return self._frame_count
-
-    @property
-    def optical_paths(self) -> List[str]:
-        """Return list of optical paths in index."""
-        return self._optical_paths
-
-    @abstractmethod
-    def pretty_str(
-        self,
-        indent: int = 0,
-        depth: Optional[int] = None
-    ) -> str:
-        raise NotImplementedError()
-
-    @abstractmethod
-    def get_frame_index(self, tile: Point, z: float, path: str) -> int:
-        """Abstract method for getting the frame index for a tile"""
-        raise NotImplementedError()
-
-    @staticmethod
-    def _read_frame_count_from_datasets(
-        datasets: Sequence[Dataset]
-    ) -> int:
-        """Return total frame count from files.
+        scaled_tile_points: Iterable[Point],
+        z: float,
+        path: str,
+        scale: int,
+        image_format: str,
+        image_options: Dict[str, Any],
+    ) -> List[bytes]:
+        """Return scaled encoded tiles defined by tile (x, y) positions, z,
+        optical path and scale.
 
         Parameters
         ----------
-        datasets: Sequence[Dataset]
-           List of datasets.
+        scaled_tile_points: Iterable[Point],
+            Scaled position of tiles to get.
+        z: float
+            Z coordinate.
+        path: str
+            Optical path.
+        Scale: int
+            Scale to use for downscaling.
+        image_format: str
+            Image format, e.g. 'JPEG', for encoding.
+        image_options: Dict[str, Any].
+            Dictionary of options for encoding.
 
         Returns
         ----------
-        int
-            Total frame count.
-
-        """
-        count = 0
-        for dataset in datasets:
-            count += dataset.frame_count
-        return count
+        List[bytes]
+            Scaled tiles as bytes.
+        """
+        return [
+            self.get_scaled_encoded_tile(
+                scaled_tile_point, z, path, scale, image_format, image_options
+            )
+            for scaled_tile_point in scaled_tile_points
+        ]
 
-    @classmethod
-    def _read_optical_paths_from_datasets(
-        cls,
-        datasets: Sequence[Dataset]
-    ) -> List[str]:
-        """Return list of optical path identifiers from files.
+    def get_tile(self, tile: Point, z: float, path: str) -> PILImage:
+        """Get tile image at tile coordinate x, y. If frame is inside tile
+        geometry but no tile exists in frame data (sparse) returns blank image. Crops
+        tile to be inside image boundary.
 
         Parameters
         ----------
-        datasets: Sequence[Dataset]
-           List of datasets.
+        tile: Point
+            Tile x, y coordinate.
+        z: float
+            Z coordinate.
+        path: str
+            Optical path.
+
 
         Returns
         ----------
-        List[str]
-            Optical identifiers.
-
+        PILImage
+            Tile image.
         """
-        paths: Set[str] = set()
-        for dataset in datasets:
-            paths.update(cls._get_path_identifers(
-                dataset.optical_path_sequence
-            ))
-        if len(paths) == 0:
-            return ['0']
-        return list(paths)
+        image = self._get_decoded_tile(tile, z, path)
+        tile_crop = self.image_region.inside_crop(tile, self.tile_size)
+        # Check if tile is an edge tile that should be cropped
+        if tile_crop.size != self.tile_size:
+            return image.crop(box=tile_crop.box)
+        return image
 
-    @staticmethod
-    def _get_path_identifers(
-        optical_path_sequence: Optional[DicomSequence]
-    ) -> List[str]:
-        """Parse optical path sequence and return list of optical path
-        identifiers
+    def get_encoded_tile(self, tile: Point, z: float, path: str) -> bytes:
+        """Get tile bytes at tile coordinate x, y. If frame is inside tile geometry
+        but no tile exists in frame data (sparse) returns encoded blank image. Crops
+        tile to be inside image boundary.
 
         Parameters
         ----------
-        optical_path_sequence: DicomSequence
-            Optical path sequence.
+        tile: Point
+            Tile x, y coordinate.
+        z: float
+            Z coordinate.
+        path: str
+            Optical path.
 
         Returns
         ----------
-        List[str]
-            List of optical path identifiers.
+        bytes
+            Tile image as bytes.
         """
-        if optical_path_sequence is None:
-            return ['0']
-        return list({
-            str(optical_ds.OpticalPathIdentifier)
-            for optical_ds in optical_path_sequence
-        })
+        tile_frame = self._get_encoded_tile(tile, z, path)
 
-    def _read_frame_coordinates(
-        self,
-        frame: Dataset
-    ) -> Tuple[Point, float]:
-        """Return frame coordinate (Point(x, y) and float z) of the frame.
-        In the Plane Position Slide Sequence x and y are defined in mm and z in
-        um.
+        # Check if tile is an edge tile that should be cropped
+        cropped_tile_region = self.image_region.inside_crop(tile, self.tile_size)
+        if cropped_tile_region.size != self.tile_size:
+            image = Image.open(io.BytesIO(tile_frame))
+            image.crop(box=cropped_tile_region.box_from_origin)
+            tile_frame = self.encode(image)
+        return tile_frame
+
+    def stitch_tiles(
+        self, region: Region, path: str, z: float, threads: int
+    ) -> PILImage:
+        """Stitches tiles together to form requested image.
 
         Parameters
         ----------
-        frame: Dataset
-            Pydicom frame sequence.
+        region: Region
+             Pixel region to stitch to image
+        path: str
+            Optical path
+        z: float
+            Z coordinate
+        threads: int
+            Number of threads to use for read.
 
         Returns
         ----------
-        Point, float
-            The frame xy coordinate and z coordinate
+        PILImage
+            Stitched image
         """
-        DECIMALS = 3
-        position = frame.PlanePositionSlideSequence[0]
-        y = int(position.RowPositionInTotalImagePixelMatrix) - 1
-        x = int(position.ColumnPositionInTotalImagePixelMatrix) - 1
-        z_offset = getattr(position, 'ZOffsetInSlideCoordinateSystem', 0.0)
-        z = round(float(z_offset), DECIMALS)
-        tile = Point(x=x, y=y) // self.tile_size
-        return tile, z
 
+        def get_and_crop_tile(tile_point: Point) -> PILImage:
+            tile = self._get_decoded_tile(tile_point, z, path)
+            tile_crop = region.inside_crop(tile_point, self.tile_size)
+            if tile_crop.size != self.tile_size:
+                tile = tile.crop(box=tile_crop.box)
+            return tile
+
+        tile_points = self._get_tile_range(region, z, path)
+        if tile_points.size.area == 1:
+            return get_and_crop_tile(tile_points.start)
+        image = Image.new(mode=self.image_mode, size=region.size.to_tuple())
+        # The tiles are cropped prior to pasting. This offset is the equal to the first
+        # (upper left) tiles size, and is added to the image coordinate for tiles not
+        # in the first row or column.
+        offset = (tile_points.start * self.tile_size) - region.start
+
+        # Method that pastes tile at point into image.
+        def tile_paste(tile_point: Point) -> None:
+            tile = get_and_crop_tile(tile_point)
+            image_coordinate = Point(
+                offset.x * (tile_point.x != tile_points.start.x),
+                offset.y * (tile_point.y != tile_points.start.y),
+            )
+            image_coordinate += (tile_point - tile_points.start) * self.tile_size
+            image.paste(tile, image_coordinate.to_tuple())
 
-class FullTileIndex(TileIndex):
-    """Index for mapping tile position to frame number for datasets containing
-    full tiles. Pixel data tiles are ordered by colum, row, z and path, thus
-    the frame index for a tile can directly be calculated."""
-    def __init__(
-        self,
-        datasets: Sequence[Dataset]
+        self._paste_tiles(tile_points, tile_paste, threads)
+        return image
+
+    @staticmethod
+    def _paste_tiles(
+        tile_region: Region, paste_method: Callable[[Point], None], threads: int
     ):
-        """Create full tile index for frames in datasets. Requires equal tile
-        size for all tile planes.
+        """Paste tiles in region using method. Use threading if number of tiles to paste
+        is larger than one and requested worker count is more than one.
 
         Parameters
         ----------
-        datasets: Sequence[Dataset]
-            List of datasets containing full tiled image data.
+        tile_region: Region
+            Tile region of tiles to paste.
+        paste_method: Callable[[Point], None]
+            Method that accepts a tile point to paste and returns None.
+        threads: int
+            Number of workers to use.
         """
-        super().__init__(datasets)
-        self._focal_planes = self._read_focal_planes_from_datasets(datasets)
-
-    @property
-    def focal_planes(self) -> List[float]:
-        return self._focal_planes
-
-    def __str__(self) -> str:
-        return self.pretty_str()
-
-    def pretty_str(
-        self,
-        indent: int = 0,
-        depth: Optional[int] = None
-    ) -> str:
-        string = (
-            f"Full tile index tile size: {self.tile_size}"
-            f", plane size: {self.tiled_size}"
-        )
-        if depth is not None:
-            depth -= 1
-            if(depth < 0):
-                return string
-        string += (
-            f" of z: {self.focal_planes} and path: {self.optical_paths}"
-        )
 
-        return string
+        if threads == 1:
+            for tile_point in tile_region.iterate_all():
+                paste_method(tile_point)
+        else:
+            with ThreadPoolExecutor(max_workers=threads) as pool:
+                pool.map(paste_method, tile_region.iterate_all())
 
-    def get_frame_index(self, tile: Point, z: float, path: str) -> int:
-        """Return frame index for a Point tile, z coordinate, and optical path
-        from full tile index. Assumes that tile, z, and path are valid.
+    def valid_tiles(self, region: Region, z: float, path: str) -> bool:
+        """Check if tile region is inside tile geometry and z coordinate and
+        optical path exists.
 
         Parameters
         ----------
-        tile: Point
-            Tile xy to get.
+        region: Region
+            Tile region.
         z: float
-            Z coordinate to get.
+            Z coordinate.
         path: str
-            ID of optical path to get.
-
-        Returns
-        ----------
-        int
-            Frame index.
+            Optical path.
         """
-        plane_offset = tile.x + self.tiled_size.width * tile.y
-        z_offset = self._get_focal_plane_index(z) * self.tiled_size.area
-        path_offset = (
-            self._get_optical_path_index(path)
-            * len(self._focal_planes) * self.tiled_size.area
+        return (
+            region.is_inside(self.plane_region)
+            and (z in self.focal_planes)
+            and (path in self.optical_paths)
         )
-        return plane_offset + z_offset + path_offset
 
-    def _read_focal_planes_from_datasets(
-        self,
-        datasets: Sequence[Dataset]
-    ) -> List[float]:
-        """Return list of focal planes in datasets. Values in Pixel Measures
-        Sequene are in mm.
+    def encode(self, image: PILImage) -> bytes:
+        """Encode image using transfer syntax.
 
         Parameters
         ----------
-        datasets: Sequence[Dataset]
-           List of datasets to read focal planes from.
+        image: PILImage
+            Image to encode
 
         Returns
         ----------
-        List[float]
-            Focal planes, specified in um.
-
-        """
-        MM_TO_MICRON = 1000.0
-        DECIMALS = 3
-        focal_planes: Set[float] = set()
-        for dataset in datasets:
-            slice_spacing = dataset.spacing_between_slices
-            number_of_focal_planes = dataset.number_of_focal_planes
-            if slice_spacing is None:
-                if number_of_focal_planes == 1:
-                    slice_spacing = 0.0
-                else:
-                    raise ValueError(
-                        "Slice spacing must be known if multple focal planes."
-                    )
-            elif slice_spacing == 0 and number_of_focal_planes != 1:
-                raise ValueError(
-                    "Slice spacing must be non-zero if multiple focal planes."
-                )
-
-            try:
-                z_offset = (
-                    dataset.SharedFunctionalGroupsSequence[0]
-                    .PlanePositionSlideSequence[0]
-                    .ZOffsetInSlideCoordinateSystem
-                )
-            except AttributeError:
-                z_offset = 0
-
-            for plane in range(number_of_focal_planes):
-                z = z_offset + round(
-                    plane * slice_spacing * MM_TO_MICRON, DECIMALS
-                )
-                focal_planes.add(z)
-        return sorted(list(focal_planes))
-
-    def _get_optical_path_index(self, path: str) -> int:
-        """Return index of the optical path in instance.
-        This assumes that all files in a concatenated set contains all the
-        optical path identifiers of the set.
-
-        Parameters
-        ----------
-        path: str
-            Optical path identifier to search for.
+        bytes
+            Encoded image as bytes
 
-        Returns
-        ----------
-        int
-            The index of the optical path identifier in the optical path
-            sequence.
         """
-        try:
-            return next(
-                (index for index, plane_path in enumerate(self._optical_paths)
-                 if plane_path == path)
-            )
-        except StopIteration:
-            raise WsiDicomNotFoundError(f"Optical path {path}", str(self))
+        image_format, image_options = self._image_settings(self.transfer_syntax)
+        with io.BytesIO() as buffer:
+            image.save(buffer, format=image_format, **image_options)
+            return buffer.getvalue()
 
-    def _get_focal_plane_index(self, z: float) -> int:
-        """Return index of the focal plane of z.
+    @staticmethod
+    def _image_settings(transfer_syntax: UID) -> Tuple[str, Dict[str, Any]]:
+        """Return image format and options for creating encoded tiles as in the
+        used transfer syntax.
 
         Parameters
         ----------
-        z: float
-            The z coordinate (in um) to search for.
+        transfer_syntax: pydicom.uid
+            Transfer syntax to match image format and options to
 
         Returns
         ----------
-        int
-            Focal plane index for z coordinate.
-        """
-        try:
-            return next(index for index, plane in enumerate(self.focal_planes)
-                        if plane == z)
-        except StopIteration:
-            raise WsiDicomNotFoundError(f"Z {z} in instance", str(self))
-
-
-class SparseTileIndex(TileIndex):
-    """Index for mapping tile position to frame number for datasets containing
-    sparse tiles. Frame indices are retrieved from tile position, z, and path
-    by finding the corresponding matching SparseTilePlane (z and path) and
-    returning the frame index at tile position. If the tile is missing (due to
-    the sparseness), -1 is returned."""
-    def __init__(
-        self,
-        datasets: Sequence[Dataset]
-    ):
-        """Create sparse tile index for frames in datasets. Requires equal tile
-        size for all tile planes. Pixel data tiles are identified by the Per
-        Frame Functional Groups Sequence that contains tile colum, row, z,
-        path, and frame index. These are stored in a SparseTilePlane
-        (one plane for every combination of z and path).
+        tuple[str, dict[str, int]]
+            image format and image options
 
-        Parameters
-        ----------
-        datasets: Sequence[Dataset]
-            List of datasets containing sparse tiled image data.
         """
-        super().__init__(datasets)
-        self._planes = self._read_planes_from_datasets(datasets)
-        self._focal_planes = self._get_focal_planes()
-
-    @property
-    def focal_planes(self) -> List[float]:
-        return self._focal_planes
-
-    def __str__(self) -> str:
-        return self.pretty_str()
-
-    def pretty_str(
-        self,
-        indent: int = 0,
-        depth: Optional[int] = None
-    ) -> str:
-        return (
-            f"Sparse tile index tile size: {self.tile_size}, "
-            f"plane size: {self.tiled_size}"
-        )
+        if transfer_syntax == JPEGBaseline8Bit:
+            image_format = "jpeg"
+            image_options = {"quality": 95}
+        elif transfer_syntax == JPEG2000:
+            image_format = "jpeg2000"
+            image_options = {"irreversible": True}
+        elif transfer_syntax == JPEG2000Lossless:
+            image_format = "jpeg2000"
+            image_options = {"irreversible": False}
+        else:
+            raise NotImplementedError("Only supports jpeg and jpeg2000")
+        return (image_format, image_options)
 
-    def get_frame_index(self, tile: Point, z: float, path: str) -> int:
-        """Return frame index for a Point tile, z coordinate, and optical
-        path.
+    @staticmethod
+    def _get_blank_color(photometric_interpretation: str) -> Tuple[int, int, int]:
+        """Return color to use blank tiles.
 
         Parameters
         ----------
-        tile: Point
-            Tile xy to get.
-        z: float
-            Z coordinate to get.
-        path: str
-            ID of optical path to get.
+        photometric_interpretation: str
+            The photomoetric interpretation of the dataset
 
         Returns
         ----------
-        int
-            Frame index.
+        Tuple[int, int, int]
+            RGB color,
+
         """
-        try:
-            plane = self._planes[(z, path)]
-        except KeyError:
-            raise WsiDicomNotFoundError(
-                f"Plane with z {z}, path {path}", str(self)
-            )
-        frame_index = plane[tile]
-        return frame_index
+        BLACK = 0
+        WHITE = 255
+        if photometric_interpretation == "MONOCHROME2":
+            return (BLACK, BLACK, BLACK)  # Monocrhome2 is black
+        return (WHITE, WHITE, WHITE)
 
-    def _get_focal_planes(self) -> List[float]:
-        """Return list of focal planes defiend in planes.
+    def _create_blank_tile(self) -> PILImage:
+        """Create blank tile for instance.
 
         Returns
         ----------
-        List[float]
-            Focal planes, specified in um.
+        PILImage
+            Blank tile image
         """
-        focal_planes: Set[float] = set()
-        for z, _ in self._planes.keys():
-            focal_planes.add(z)
-        return sorted(list(focal_planes))
+        return Image.new(
+            mode=self.image_mode,  # type: ignore
+            size=self.tile_size.to_tuple(),
+            color=self.blank_color[: self.samples_per_pixel],
+        )
 
-    def _read_planes_from_datasets(
-        self,
-        datasets: Sequence[Dataset]
-    ) -> Dict[Tuple[float, str], SparseTilePlane]:
-        """Return SparseTilePlane from planes in datasets.
+    def _get_tile_range(self, pixel_region: Region, z: float, path: str) -> Region:
+        """Return range of tiles to cover pixel region.
 
         Parameters
         ----------
-        datasets: Sequence[Dataset]
-           List of datasets to read planes from.
+        pixel_region: Region
+            Pixel region of tiles to get
+        z: float
+            Z coordinate of tiles to get
+        path: str
+            Optical path identifier of tiles to get
 
         Returns
         ----------
-        Dict[Tuple[float, str], SparseTilePlane]
-            Dict of planes with focal plane and optical identifier as key.
+        Region
+            Region of tiles for stitching image
         """
-        planes: Dict[Tuple[float, str], SparseTilePlane] = {}
-
-        for dataset in datasets:
-            frame_sequence = dataset.frame_sequence
-            for i, frame in enumerate(frame_sequence):
-                (tile, z) = self._read_frame_coordinates(frame)
-                identifier = dataset.read_optical_path_identifier(frame)
 
-                try:
-                    plane = planes[(z, identifier)]
-                except KeyError:
-                    plane = SparseTilePlane(self.tiled_size)
-                    planes[(z, identifier)] = plane
-                plane[tile] = i + dataset.frame_offset
-
-        return planes
+        tile_region = Region.from_points(
+            pixel_region.start // self.tile_size,
+            (pixel_region.end - 1) // self.tile_size + 1,
+        )
+        if not self.valid_tiles(tile_region, z, path):
+            raise WsiDicomOutOfBoundsError(
+                f"Tile region {tile_region}", f"tiled size {self.tiled_size}"
+            )
+        return tile_region
```

### Comparing `wsidicom-0.8.0/wsidicom/image_data/image_data.py` & `wsidicom-0.9.0/wsidicom/wsidicom.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,683 +8,653 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-import io
+import os
 import warnings
-from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Callable, List, Optional, Sequence, Tuple, Union
 
 from PIL import Image
 from PIL.Image import Image as PILImage
-from pydicom.dataset import Dataset
-from pydicom.sequence import Sequence as DicomSequence
-from pydicom.uid import JPEG2000, UID, JPEG2000Lossless, JPEGBaseline8Bit
-
-from wsidicom.errors import WsiDicomOutOfBoundsError
-from wsidicom.geometry import (
-    Orientation,
-    Point,
-    PointMm,
-    Region,
-    RegionMm,
-    Size,
-    SizeMm,
+from pydicom.uid import UID, JPEGBaseline8Bit, generate_uid
+
+from wsidicom.errors import (
+    WsiDicomMatchError,
+    WsiDicomNotFoundError,
+    WsiDicomOutOfBoundsError,
 )
+from wsidicom.file import WsiDicomFileSource, WsiDicomFileTarget
+from wsidicom.geometry import Point, PointMm, Region, RegionMm, Size, SizeMm
+from wsidicom.graphical_annotations import AnnotationInstance
+from wsidicom.instance import WsiDataset, WsiInstance
+from wsidicom.optical import OpticalManager
+from wsidicom.series import Labels, Levels, Overviews
+from wsidicom.source import Source
+from wsidicom.stringprinting import list_pretty_str
+from wsidicom.uid import SlideUids
+from wsidicom.web import WsiDicomWebClient, WsiDicomWebSource
+
 
+class WsiDicom:
+    """Represent a wsi slide containing pyramidal levels and optionally
+    labels and/or overviews."""
 
-class ImageOrigin:
     def __init__(
         self,
-        origin: Optional[PointMm] = None,
-        orientation: Optional[Orientation] = None,
+        source: Source,
+        label: Optional[Union[PILImage, str, Path]] = None,
     ):
-        if origin is None:
-            origin = PointMm(0, 0)
-        if orientation is None:
-            orientation = Orientation([0, 1, 0, 1, 0, 0])
-        self._origin = origin
-        self._orientation = orientation
-
-    @property
-    def origin(self) -> PointMm:
-        return self._origin
-
-    @property
-    def orientation(self) -> Orientation:
-        return self._orientation
-
-    @classmethod
-    def from_dataset(cls, dataset: Dataset):
-        try:
-            origin = PointMm(
-                dataset.TotalPixelMatrixOriginSequence[
-                    0
-                ].XOffsetInSlideCoordinateSystem,
-                dataset.TotalPixelMatrixOriginSequence[
-                    0
-                ].YOffsetInSlideCoordinateSystem,
-            )
-        except (AttributeError, IndexError):
-            warnings.warn(
-                "Using default image origin as TotalPixelMatrixOriginSequence "
-                "not set in file"
-            )
-            origin = None
-        try:
-            orientation = Orientation(dataset.ImageOrientationSlide)
-        except AttributeError:
-            warnings.warn(
-                "Using default image orientation as ImageOrientationSlide "
-                "not set in file"
-            )
-            orientation = None
-        return cls(origin, orientation)
+        """Holds wsi dicom levels, labels and overviews.
 
-    @property
-    def total_pixel_matrix_origin_sequence(self) -> DicomSequence:
-        """Return formatted TotalPixelMatrixOriginSequence."""
-        offset_item = Dataset()
-        offset_item.XOffsetInSlideCoordinateSystem = self.origin.x
-        offset_item.YOffsetInSlideCoordinateSystem = self.origin.y
-        return DicomSequence([offset_item])
+        Note that WsiDicom.open() should be used for opening dicom wsi files.
 
-    @property
-    def image_orientation_slide(
-        self,
-    ) -> List[float]:
-        """Return formatted ImageOrientationSlide."""
-        return list(self.orientation.orientation)
+        Parameters
+        ----------
+        source: Source
+            A source providing instances for the wsi to open.
+        label: Optional[Union[PILImage, str, Path]] = None
+            Optional label image to use instead of label found in source.
+        """
+        self._source = source
+        if label is None:
+            label_instances = source.label_instances
+        else:
+            label_instances = [
+                WsiInstance.create_label(
+                    label,
+                    source.base_dataset,
+                )
+            ]
+        self._levels = Levels.open(source.level_instances)
+        self._labels = Labels.open(label_instances)
+        self._overviews = Overviews.open(source.overview_instances)
+        self._annotations = list(source.annotation_instances)
+        self._uids = self._validate_collection()
 
-    @property
-    def rotation(self) -> float:
-        return self._orientation.rotation
+        self.optical = OpticalManager.open(
+            [instance for series in self.collection for instance in series.instances]
+        )
 
-    def transform_region(self, region: RegionMm) -> "RegionMm":
-        region.position = region.position - self._origin
-        return self._orientation.apply(region)
+        self.__enter__()
 
+    @classmethod
+    def open(
+        cls,
+        path: Union[str, Sequence[str], Path, Sequence[Path]],
+        label: Optional[Union[PILImage, str, Path]] = None,
+    ) -> "WsiDicom":
+        """Open valid wsi dicom files in path and return a WsiDicom object.
+        Non-valid files are ignored.
 
-class ImageData(metaclass=ABCMeta):
-    """Generic class for image data that can be inherited to implement support
-    for other image/file formats. Subclasses should implement properties to get
-    transfer_syntax, image_size, tile_size, pixel_spacing,  samples_per_pixel,
-    and photometric_interpretation and methods get_tile() and close().
-    Additionally properties focal_planes and/or optical_paths should be
-    overridden if multiple focal planes or optical paths are implemented."""
+        Parameters
+        ----------
+        path: Union[str, Sequence[str], Path, Sequence[Path]]
+            Path to files to open.
+        label: Optional[Union[PILImage, str, Path]] = None
+            Optional label image to use instead of label found in path.
 
-    _default_z: Optional[float] = None
-    _blank_tile: Optional[PILImage] = None
-    _encoded_blank_tile: Optional[bytes] = None
+        Returns
+        ----------
+        WsiDicom
+            WsiDicom created from wsi dicom files in path.
+        """
+        source = WsiDicomFileSource(path)
+        return cls(source, label)
 
-    @property
-    @abstractmethod
-    def files(self) -> List[Path]:
-        raise NotImplementedError()
+    @classmethod
+    def open_web(
+        cls,
+        client: WsiDicomWebClient,
+        study_uid: Union[str, UID],
+        series_uid: Union[str, UID],
+        requested_transfer_syntax: UID = JPEGBaseline8Bit,
+    ) -> "WsiDicom":
+        """Open wsi dicom instances using dicom web client.
 
-    @property
-    @abstractmethod
-    def transfer_syntax(self) -> UID:
-        """Should return the uid of the transfer syntax of the image."""
-        raise NotImplementedError()
+        Parameters
+        ----------
+        client: WsiDicomWebClient
+            Configured dicom web client.
+        study_uid: Union[str, UID]
+            Study uid of wsi to open.
+        series_uid: Union[str, UID]
+            Series uid of wsi to open
+        transfer_syntax: UID
+            Transfer syntax to request for image data, for example
+            UID("1.2.840.10008.1.2.4.50") for JPEGBaseline8Bit.
 
-    @property
-    @abstractmethod
-    def image_size(self) -> Size:
-        """Should return the pixel size of the image."""
-        raise NotImplementedError()
+        Returns
+        ----------
+        WsiDicom
+            WsiDicom created from wsi dicom files in study-series.
+        """
+        source = WsiDicomWebSource(
+            client, study_uid, series_uid, requested_transfer_syntax
+        )
+        return cls(source)
 
-    @property
-    @abstractmethod
-    def tile_size(self) -> Size:
-        """Should return the pixel tile size of the image, or pixel size of
-        the image if not tiled."""
-        raise NotImplementedError()
+    def __enter__(self):
+        return self
 
-    @property
-    @abstractmethod
-    def pixel_spacing(self) -> Optional[SizeMm]:
-        """Should return the size of the pixels in mm/pixel."""
-        raise NotImplementedError()
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
 
-    @property
-    @abstractmethod
-    def samples_per_pixel(self) -> int:
-        """Should return number of samples per pixel (e.g. 3 for RGB."""
-        raise NotImplementedError()
+    def __repr__(self) -> str:
+        return (
+            f"{type(self).__name__}({self.levels}, {self.labels}"
+            f"{self.overviews}, {self.annotations})"
+        )
 
-    @property
-    @abstractmethod
-    def photometric_interpretation(self) -> str:
-        """Should return the photophotometric interpretation of the image
-        data."""
-        raise NotImplementedError()
+    def __str__(self) -> str:
+        return self.pretty_str()
 
     @property
-    @abstractmethod
-    def image_origin(self) -> ImageOrigin:
-        """Should return the image origin of the image data."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def _get_decoded_tile(self, tile_point: Point, z: float, path: str) -> PILImage:
-        """Should return Image for tile defined by tile (x, y), z,
-        and optical path."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def _get_encoded_tile(self, tile: Point, z: float, path: str) -> bytes:
-        """Should return image bytes for tile defined by tile (x, y), z,
-        and optical path."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def close(self) -> None:
-        """Should close any open files."""
-        raise NotImplementedError()
+    def size(self) -> Size:
+        """Return pixel size of base level."""
+        return self.levels.size
 
     @property
-    def tiled_size(self) -> Size:
-        """The size of the image when divided into tiles, e.g. number of
-        columns and rows of tiles. Equals (1, 1) if image is not tiled."""
-        return self.image_size.ceil_div(self.tile_size)
+    def mm_size(self) -> SizeMm:
+        return self.levels.mm_size
 
     @property
-    def image_region(self) -> Region:
-        return Region(Point(0, 0), self.image_size)
+    def tile_size(self) -> Size:
+        """Return tile size of levels."""
+        return self.levels.tile_size
 
     @property
-    def focal_planes(self) -> List[float]:
-        """Focal planes avaiable in the image defined in um."""
-        return [0.0]
+    def pixel_spacing(self) -> SizeMm:
+        return self.levels.pixel_spacing
 
     @property
-    def optical_paths(self) -> List[str]:
-        """Optical paths avaiable in the image."""
-        return ["0"]
+    def mpp(self) -> SizeMm:
+        return self.levels.mpp
 
     @property
-    def image_mode(self) -> str:
-        """Return Pillow image mode (e.g. RGB) for image data"""
-        if self.samples_per_pixel == 1:
-            return "L"
-        elif self.samples_per_pixel == 3:
-            return "RGB"
-        raise NotImplementedError()
+    def uids(self) -> Optional[SlideUids]:
+        return self._uids
 
     @property
-    def blank_color(self) -> Tuple[int, int, int]:
-        """Return RGB background color."""
-        return self._get_blank_color(self.photometric_interpretation)
-
-    def pretty_str(self, indent: int = 0, depth: Optional[int] = None) -> str:
-        return str(self)
+    def levels(self) -> Levels:
+        """Return contained levels."""
+        if self._levels is not None:
+            return self._levels
+        raise WsiDicomNotFoundError("levels", str(self))
 
     @property
-    def default_z(self) -> float:
-        """Return single defined focal plane (in um) if only one focal plane
-        defined. Return the middle focal plane if several focal planes are
-        defined."""
-        if self._default_z is None:
-            default = 0
-            if len(self.focal_planes) > 1:
-                smallest = min(self.focal_planes)
-                largest = max(self.focal_planes)
-                middle = (largest - smallest) / 2
-                default = min(
-                    range(len(self.focal_planes)),
-                    key=lambda i: abs(self.focal_planes[i] - middle),
-                )
-
-            self._default_z = self.focal_planes[default]
-
-        return self._default_z
+    def labels(self) -> Optional[Labels]:
+        """Return contained labels."""
+        return self._labels
 
     @property
-    def default_path(self) -> str:
-        """Return the first defined optical path as default optical path
-        identifier."""
-        return self.optical_paths[0]
+    def overviews(self) -> Optional[Overviews]:
+        """Return contained overviews."""
+        return self._overviews
 
     @property
-    def plane_region(self) -> Region:
-        return Region(position=Point(0, 0), size=self.tiled_size - 1)
+    def annotations(self) -> List[AnnotationInstance]:
+        """Return contained annotations."""
+        return self._annotations
 
     @property
-    def blank_tile(self) -> PILImage:
-        """Return background tile."""
-        if self._blank_tile is None:
-            self._blank_tile = self._create_blank_tile()
-        return self._blank_tile
+    def collection(self) -> List[Union[Levels, Labels, Overviews]]:
+        collection: List[Optional[Union[Levels, Labels, Overviews]]] = [
+            self._levels,
+            self._labels,
+            self._overviews,
+        ]
+        return [series for series in collection if series is not None]
 
-    @property
-    def blank_encoded_tile(self) -> bytes:
-        """Return encoded background tile."""
-        if self._encoded_blank_tile is None:
-            self._encoded_blank_tile = self.encode(self.blank_tile)
-        return self._encoded_blank_tile
+    def pretty_str(self, indent: int = 0, depth: Optional[int] = None) -> str:
+        string = self.__class__.__name__
+        if depth is not None:
+            depth -= 1
+            if depth < 0:
+                return string
+        return (
+            string
+            + " of levels:\n"
+            + list_pretty_str(self.levels.groups, indent, depth, 0, 2)
+        )
 
-    def get_decoded_tiles(
-        self, tiles: Iterable[Point], z: float, path: str
-    ) -> List[PILImage]:
-        """Return tiles for tile defined by tile (x, y), z, and optical
-        path.
+    def read_label(self, index: int = 0) -> PILImage:
+        """Read label image of the whole slide. If several label
+        images are present, index can be used to select a specific image.
 
         Parameters
         ----------
-        tiles: Iterable[Point]
-            Tiles to get.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
+        index: int = 0
+            Index of the label image to read.
 
         Returns
         ----------
-        List[PILImage]
-            Tiles as Images.
+        PILImage
+            label as image.
         """
-        return [self._get_decoded_tile(tile, z, path) for tile in tiles]
+        if self.labels is None:
+            raise WsiDicomNotFoundError("label", str(self))
+        try:
+            label = self.labels[index]
+            return label.get_default_full()
+        except IndexError as exception:
+            raise WsiDicomNotFoundError("label", "series") from exception
 
-    def get_encoded_tiles(
-        self, tiles: Iterable[Point], z: float, path: str
-    ) -> List[bytes]:
-        """Return tiles for tile defined by tile (x, y), z, and optical
-        path.
+    def read_overview(self, index: int = 0) -> PILImage:
+        """Read overview image of the whole slide. If several overview
+        images are present, index can be used to select a specific image.
 
         Parameters
         ----------
-        tiles: Iterable[Point]
-            Tiles to get.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
+        index: int = 0
+            Index of the overview image to read.
 
         Returns
         ----------
-        List[bytes]
-            Tiles in bytes.
+        PILImage
+            Overview as image.
         """
-        return [self._get_encoded_tile(tile, z, path) for tile in tiles]
+        if self.overviews is None:
+            raise WsiDicomNotFoundError("overview", str(self))
+        try:
+            overview = self.overviews[index]
+            return overview.get_default_full()
+        except IndexError as exception:
+            raise WsiDicomNotFoundError("overview", "series") from exception
 
-    def get_scaled_tile(
-        self, scaled_tile_point: Point, z: float, path: str, scale: int
+    def read_thumbnail(
+        self,
+        size: Tuple[int, int] = (512, 512),
+        z: Optional[float] = None,
+        path: Optional[str] = None,
     ) -> PILImage:
-        """Return scaled tile defined by tile (x, y), z, optical
-        path and scale.
+        """Read thumbnail image of the whole slide with dimensions
+        no larger than given size.
 
         Parameters
         ----------
-        scaled_tile_point: Point,
-            Scaled position of tile to get.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
-        Scale: int
-            Scale to use for downscaling.
+        size: Tuple[int, int] = (512, 512)
+            Upper size limit for thumbnail.
+        z: Optional[float] = None
+            Z coordinate, optional.
+        path: Optional[str] = None
+            Optical path, optional.
 
         Returns
         ----------
         PILImage
-            Scaled tiled as Image.
+            Thumbnail as image,
         """
-        image = Image.new(
-            mode=self.image_mode,  # type: ignore
-            size=(self.tile_size * scale).to_tuple(),
-            color=self.blank_color[: self.samples_per_pixel],
-        )
-        # Get decoded tiles for the region covering the scaled tile
-        # in the image data
-        tile_points = Region(scaled_tile_point * scale, Size(1, 1) * scale)
-        origin = tile_points.start
-        for tile_point in tile_points.iterate_all():
-            if (tile_point.x < self.tiled_size.width) and (
-                tile_point.y < self.tiled_size.height
-            ):
-                tile = self._get_decoded_tile(tile_point, z, path)
-                image_coordinate = (tile_point - origin) * self.tile_size
-                image.paste(tile, image_coordinate.to_tuple())
-
-        return image.resize(
-            self.tile_size.to_tuple(), resample=Image.Resampling.BILINEAR
-        )
+        thumbnail_size = Size.from_tuple(size)
+        level = self.levels.get_closest_by_size(thumbnail_size)
+        region = Region(position=Point(0, 0), size=level.size)
+        image = level.get_region(region, z, path)
+        image.thumbnail((size), resample=Image.Resampling.BILINEAR)
+        return image
 
-    def get_scaled_encoded_tile(
+    def read_region(
         self,
-        scaled_tile_point: Point,
-        z: float,
-        path: str,
-        scale: int,
-        image_format: str,
-        image_options: Dict[str, Any],
-    ) -> bytes:
-        """Return scaled encoded tile defined by tile (x, y), z, optical
-        path and scale.
+        location: Tuple[int, int],
+        level: int,
+        size: Tuple[int, int],
+        z: Optional[float] = None,
+        path: Optional[str] = None,
+        threads: int = 1,
+    ) -> PILImage:
+        """Read region defined by pixels.
 
         Parameters
         ----------
-        scaled_tile_point: Point,
-            Scaled position of tile to get.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
-        Scale: int
-            Scale to use for downscaling.
-        image_format: str
-            Image format, e.g. 'JPEG', for encoding.
-        image_options: Dict[str, Any].
-            Dictionary of options for encoding.
+        location: Tuple[int, int]
+            Upper left corner of region in pixels.
+        level: int
+            Level in pyramid.
+        size: Tuple[int, int]
+            Size of region in pixels.
+        z: Optional[float] = None
+            Z coordinate, optional.
+        path: Optional[str] = None
+            Optical path, optional.
+        threads: int = 1
+            Number of threads to use for read.
 
         Returns
         ----------
-        bytes
-            Scaled tile as bytes.
+        PILImage
+            Region as image
         """
-        image = self.get_scaled_tile(scaled_tile_point, z, path, scale)
-        with io.BytesIO() as buffer:
-            image.save(buffer, format=image_format, **image_options)
-            return buffer.getvalue()
+        wsi_level = self.levels.get_closest_by_level(level)
+        scale_factor = wsi_level.calculate_scale(level)
+        scaled_region = (
+            Region(position=Point.from_tuple(location), size=Size.from_tuple(size))
+            * scale_factor
+        )
+
+        if not wsi_level.valid_pixels(scaled_region):
+            raise WsiDicomOutOfBoundsError(
+                f"Region {scaled_region}", f"level size {wsi_level.size}"
+            )
+        image = wsi_level.get_region(scaled_region, z, path, threads)
+        if scale_factor != 1:
+            image = image.resize((size), resample=Image.Resampling.BILINEAR)
+        return image
 
-    def get_scaled_encoded_tiles(
+    def read_region_mm(
         self,
-        scaled_tile_points: Iterable[Point],
-        z: float,
-        path: str,
-        scale: int,
-        image_format: str,
-        image_options: Dict[str, Any],
-    ) -> List[bytes]:
-        """Return scaled encoded tiles defined by tile (x, y) positions, z,
-        optical path and scale.
+        location: Tuple[float, float],
+        level: int,
+        size: Tuple[float, float],
+        z: Optional[float] = None,
+        path: Optional[str] = None,
+        slide_origin: bool = False,
+        threads: int = 1,
+    ) -> PILImage:
+        """Read image from region defined in mm.
 
         Parameters
         ----------
-        scaled_tile_points: Iterable[Point],
-            Scaled position of tiles to get.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
-        Scale: int
-            Scale to use for downscaling.
-        image_format: str
-            Image format, e.g. 'JPEG', for encoding.
-        image_options: Dict[str, Any].
-            Dictionary of options for encoding.
+        location: Tuple[float, float]
+            Upper left corner of region in mm, or lower left corner if using
+            slide origin.
+        level: int
+            Level in pyramid
+        size: Tuple[float, float].
+            Size of region in mm
+        z: Optional[float] = None
+            Z coordinate, optional
+        path: Optional[str] = None
+            optical path, optional
+        slide_origin: bool = False
+            If to use the slide origin instead of image origin.
+        threads: int = 1
+            Number of threads to use for read.
 
         Returns
         ----------
-        List[bytes]
-            Scaled tiles as bytes.
-        """
-        return [
-            self.get_scaled_encoded_tile(
-                scaled_tile_point, z, path, scale, image_format, image_options
-            )
-            for scaled_tile_point in scaled_tile_points
-        ]
+        PILImage
+            Region as image
+        """
+        wsi_level = self.levels.get_closest_by_level(level)
+        scale_factor = wsi_level.calculate_scale(level)
+        region = RegionMm(PointMm.from_tuple(location), SizeMm.from_tuple(size))
+        image = wsi_level.get_region_mm(region, z, path, slide_origin, threads)
+        image_size = Size(width=image.size[0], height=image.size[1]) // scale_factor
+        return image.resize(image_size.to_tuple(), resample=Image.Resampling.BILINEAR)
 
-    def valid_tiles(self, region: Region, z: float, path: str) -> bool:
-        """Check if tile region is inside tile geometry and z coordinate and
-        optical path exists.
+    def read_region_mpp(
+        self,
+        location: Tuple[float, float],
+        mpp: float,
+        size: Tuple[float, float],
+        z: Optional[float] = None,
+        path: Optional[str] = None,
+        slide_origin: bool = False,
+        threads: int = 1,
+    ) -> PILImage:
+        """Read image from region defined in mm with set pixel spacing.
 
         Parameters
         ----------
-        region: Region
-            Tile region.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
+        location: Tuple[float, float].
+            Upper left corner of region in mm, or lower left corner if using
+            slide origin.
+        mpp: float
+            Requested pixel spacing (um/pixel).
+        size: Tuple[float, float].
+            Size of region in mm.
+        z: Optional[float] = None
+            Z coordinate, optional.
+        path: Optional[str] = None
+            Optical path, optional.
+        slide_origin: bool = False
+            If to use the slide origin instead of image origin.
+        threads: int = 1
+            Number of threads to use for read.
+
+        Returns
+        -----------
+        PILImage
+            Region as image
         """
-        return (
-            region.is_inside(self.plane_region)
-            and (z in self.focal_planes)
-            and (path in self.optical_paths)
+        pixel_spacing = mpp / 1000.0
+        wsi_level = self.levels.get_closest_by_pixel_spacing(
+            SizeMm(pixel_spacing, pixel_spacing)
         )
+        region = RegionMm(PointMm.from_tuple(location), SizeMm.from_tuple(size))
+        image = wsi_level.get_region_mm(region, z, path, slide_origin, threads)
+        image_size = SizeMm.from_tuple(size) // pixel_spacing
+        return image.resize(image_size.to_tuple(), resample=Image.Resampling.BILINEAR)
 
-    def encode(self, image: PILImage) -> bytes:
-        """Encode image using transfer syntax.
+    def read_tile(
+        self,
+        level: int,
+        tile: Tuple[int, int],
+        z: Optional[float] = None,
+        path: Optional[str] = None,
+    ) -> PILImage:
+        """Read tile in pyramid level as image.
 
         Parameters
         ----------
-        image: PILImage
-            Image to encode
+        level: int
+            Pyramid level
+        tile: int, int
+            tile xy coordinate
+        z: Optional[float] = None
+            Z coordinate, optional
+        path: Optional[str] = None
+            optical path, optional
 
         Returns
         ----------
-        bytes
-            Encoded image as bytes
-
+        PILImage
+            Tile as image
         """
-        image_format, image_options = self._image_settings(self.transfer_syntax)
-        with io.BytesIO() as buffer:
-            image.save(buffer, format=image_format, **image_options)
-            return buffer.getvalue()
+        tile_point = Point.from_tuple(tile)
+        try:
+            wsi_level = self.levels.get_level(level)
+            return wsi_level.get_tile(tile_point, z, path)
+        except WsiDicomNotFoundError:
+            # Scale from closest level
+            wsi_level = self.levels.get_closest_by_level(level)
+            return wsi_level.get_scaled_tile(tile_point, level, z, path)
 
-    @staticmethod
-    def _image_settings(transfer_syntax: UID) -> Tuple[str, Dict[str, Any]]:
-        """Return image format and options for creating encoded tiles as in the
-        used transfer syntax.
+    def read_encoded_tile(
+        self,
+        level: int,
+        tile: Tuple[int, int],
+        z: Optional[float] = None,
+        path: Optional[str] = None,
+    ) -> bytes:
+        """Read tile in pyramid level as encoded bytes. For non-existing levels
+        the tile is scaled down from a lower level, using the similar encoding.
 
         Parameters
         ----------
-        transfer_syntax: pydicom.uid
-            Transfer syntax to match image format and options to
+        level: int
+            Pyramid level
+        tile: int, int
+            tile xy coordinate
+        z: Optional[float] = None
+            Z coordinate, optional
+        path: Optional[str] = None
+            optical path, optional
 
         Returns
         ----------
-        tuple[str, dict[str, int]]
-            image format and image options
-
+        bytes
+            Tile in file encoding.
         """
-        if transfer_syntax == JPEGBaseline8Bit:
-            image_format = "jpeg"
-            image_options = {"quality": 95}
-        elif transfer_syntax == JPEG2000:
-            image_format = "jpeg2000"
-            image_options = {"irreversible": True}
-        elif transfer_syntax == JPEG2000Lossless:
-            image_format = "jpeg2000"
-            image_options = {"irreversible": False}
-        else:
-            raise NotImplementedError("Only supports jpeg and jpeg2000")
-        return (image_format, image_options)
+        tile_point = Point.from_tuple(tile)
+        try:
+            wsi_level = self.levels.get_level(level)
+            return wsi_level.get_encoded_tile(tile_point, z, path)
+        except WsiDicomNotFoundError:
+            # Scale from closest level
+            wsi_level = self.levels.get_closest_by_level(level)
+            return wsi_level.get_scaled_encoded_tile(tile_point, level, z, path)
 
-    @staticmethod
-    def _get_blank_color(photometric_interpretation: str) -> Tuple[int, int, int]:
-        """Return color to use blank tiles.
+    def get_instance(
+        self, level: int, z: Optional[float] = None, path: Optional[str] = None
+    ) -> WsiInstance:
+        """Return instance fullfilling level, z and/or path.
 
         Parameters
         ----------
-        photometric_interpretation: str
-            The photomoetric interpretation of the dataset
+        level: int
+            Pyramid level
+        z: Optional[float] = None
+            Z coordinate, optional
+        path: Optional[str] = None
+            optical path, optional
 
         Returns
         ----------
-        Tuple[int, int, int]
-            RGB color,
-
+        WsiInstance:
+            Instance
         """
-        BLACK = 0
-        WHITE = 255
-        if photometric_interpretation == "MONOCHROME2":
-            return (BLACK, BLACK, BLACK)  # Monocrhome2 is black
-        return (WHITE, WHITE, WHITE)
+        wsi_level = self.levels.get_level(level)
+        return wsi_level.get_instance(z, path)
 
-    def _create_blank_tile(self) -> PILImage:
-        """Create blank tile for instance.
-
-        Returns
-        ----------
-        PILImage
-            Blank tile image
-        """
-        return Image.new(
-            mode=self.image_mode,  # type: ignore
-            size=self.tile_size.to_tuple(),
-            color=self.blank_color[: self.samples_per_pixel],
-        )
+    def close(self) -> None:
+        """Close source."""
+        self._source.close()
 
-    def stitch_tiles(self, region: Region, path: str, z: float) -> PILImage:
-        """Stitches tiles together to form requested image.
+    def save(
+        self,
+        output_path: Union[str, Path],
+        uid_generator: Callable[..., UID] = generate_uid,
+        workers: Optional[int] = None,
+        chunk_size: Optional[int] = None,
+        offset_table: Optional[str] = "bot",
+        add_missing_levels: bool = False,
+    ) -> List[Path]:
+        """Save wsi as DICOM-files in path. Instances for the same pyramid
+        level will be combined when possible to one file (e.g. not split
+        for optical paths or focal planes). If instances are sparse tiled they
+        will be converted to full tiled by inserting blank tiles. The PixelData
+        will contain a basic offset table. All instance uids will be changed.
 
         Parameters
         ----------
-        region: Region
-             Pixel region to stitch to image
-        path: str
-            Optical path
-        z: float
-            Z coordinate
+        output_path: Union[str, Path]
+        uid_generator: Callable[..., UID] = pydicom.uid.generate_uid
+             Function that can gernerate unique identifiers.
+        workers: Optional[int] = None
+            Maximum number of thread workers to use.
+        chunk_size: Optional[int] = None
+            Chunk size (number of tiles) to process at a time. Actual chunk
+            size also depends on minimun_chunk_size from image_data.
+        offset_table: Optional[str] = 'bot'
+            Offset table to use, 'bot' basic offset table, 'eot' extended
+            offset table, None - no offset table.
+        add_missing_levels: bool = False
+            If to add missing dyadic levels up to the single tile level.
 
         Returns
         ----------
-        PILImage
-            Stitched image
-        """
-
-        image = Image.new(
-            mode=self.image_mode, size=region.size.to_tuple()  # type: ignore
+        List[Path]
+            List of paths of created files.
+        """
+        if workers is None:
+            cpus = os.cpu_count()
+            if cpus is None:
+                workers = 1
+            else:
+                workers = cpus
+        if chunk_size is None:
+            chunk_size = 16
+        if isinstance(output_path, str):
+            output_path = Path(output_path)
+        target = WsiDicomFileTarget(
+            output_path,
+            uid_generator,
+            workers,
+            chunk_size,
+            offset_table,
+            add_missing_levels,
         )
-        stitching_tiles = self._get_tile_range(region, z, path)
+        target.save_levels(self.levels)
+        if self.overviews is not None:
+            target.save_overviews(self.overviews)
+        if self.labels is not None:
+            target.save_labels(self.labels)
+        return target.filepaths
 
-        write_index = Point(x=0, y=0)
-        tile = stitching_tiles.position
-        for tile in stitching_tiles.iterate_all(include_end=True):
-            tile_image = self.get_tile(tile, z, path, region)
-            image.paste(tile_image, write_index.to_tuple())
-            write_index = self._write_indexer(
-                write_index, Size.from_tuple(tile_image.size), region.size
-            )
-        return image
-
-    def _get_tile_range(self, pixel_region: Region, z: float, path: str) -> Region:
-        """Return range of tiles to cover pixel region.
-
-        Parameters
-        ----------
-        pixel_region: Region
-            Pixel region of tiles to get
-        z: float
-            Z coordinate of tiles to get
-        path: str
-            Optical path identifier of tiles to get
+    def _validate_collection(self) -> SlideUids:
+        """Check that no files or instance in collection is duplicate, and, if
+        strict, that all series have the same base uids.
+        Raises WsiDicomMatchError otherwise. Returns base uid for collection.
 
         Returns
         ----------
-        Region
-            Region of tiles for stitching image
+        SlideUids
+            Matching uids
         """
-        start = pixel_region.start // self.tile_size
-        end = pixel_region.end.ceil_div(self.tile_size) - 1
-        tile_region = Region.from_points(start, end)
-        if not self.valid_tiles(tile_region, z, path):
-            raise WsiDicomOutOfBoundsError(
-                f"Tile region {tile_region}", f"tiled size {self.tiled_size}"
-            )
-        return tile_region
+        datasets = [
+            dataset for collection in self.collection for dataset in collection.datasets
+        ]
+        WsiDataset.check_duplicate_dataset(datasets, self)
 
-    @staticmethod
-    def _write_indexer(index: Point, previous_size: Size, image_size: Size) -> Point:
-        """Increment index in x by previous width until index x exceds image
-        size. Then resets index x to 0 and increments index y by previous
-        height. Requires that tiles are scanned row by row.
+        instances = [
+            instance
+            for collection in self.collection
+            for instance in collection.instances
+        ]
 
-        Parameters
-        ----------
-        index: Point
-            The last write index position
-        previouis_size: Size
-            The size of the last written last tile
-        image_size: Size
-            The size of the image to be written
+        WsiInstance.check_duplicate_instance(instances, self)
 
-        Returns
-        ----------
-        Point
-            The position (upper right) in image to insert the next tile into
-        """
-        index.x += previous_size.width
-        if index.x >= image_size.width:
-            index.x = 0
-            index.y += previous_size.height
-        return index
+        try:
+            slide_uids = next(
+                series.uids for series in self.collection if series.uids is not None
+            )
+        except StopIteration as exception:
+            raise WsiDicomNotFoundError("Valid series", "in collection") from exception
+        for series in self.collection:
+            if series.uids is not None and series.uids != slide_uids:
+                raise WsiDicomMatchError(str(series), str(self))
+
+        if self.annotations != []:
+            for annotation in self.annotations:
+                if annotation.slide_uids != slide_uids:
+                    warnings.warn("Annotations uids does not match")
+        return slide_uids
 
-    def get_tile(
-        self, tile: Point, z: float, path: str, crop: Union[bool, Region] = True
-    ) -> PILImage:
-        """Get tile image at tile coordinate x, y. If frame is inside tile
-        geometry but no tile exists in frame data (sparse) returns blank image.
-        Optional crop tile to crop_region.
+    @classmethod
+    def is_ready_for_viewing(
+        cls, path: Union[str, Sequence[str], Path, Sequence[Path]]
+    ) -> Optional[bool]:
+        """Return true if files in path are formated for fast viewing, i.e.
+        have TILED_FULL tile arrangement and have an offset table.
 
         Parameters
         ----------
-        tile: Point
-            Tile x, y coordinate.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
-        crop: Union[bool, Region] = True
-            If to crop tile to image size (True, default) or to region.
+        path: Union[str, Sequence[str], Path, Sequence[Path]]
+            Path to files to test.
 
         Returns
-        ----------
-        PILImage
-            Tile image.
+            True if files in path are formated for fast viewing, None if no DICOM WSI
+            files are in the path.
         """
-        image = self._get_decoded_tile(tile, z, path)
-        if crop is False:
-            return image
-
-        if isinstance(crop, bool):
-            crop = self.image_region
-        tile_crop = crop.inside_crop(tile, self.tile_size)
-        if tile_crop.size == self.tile_size:
-            return image
-
-        return image.crop(box=tile_crop.box)
+        source = WsiDicomFileSource(path)
+        return source.is_ready_for_viewing
 
-    def get_encoded_tile(
-        self, tile: Point, z: float, path: str, crop: Union[bool, Region] = True
-    ) -> bytes:
-        """Get tile bytes at tile coordinate x, y
-        If frame is inside tile geometry but no tile exists in
-        frame data (sparse) returns encoded blank image.
+    @classmethod
+    def is_supported(
+        cls, path: Union[str, Sequence[str], Path, Sequence[Path]]
+    ) -> bool:
+        """Return true if files in path have at least one level that can be read with
+        WsiDicom.
 
         Parameters
         ----------
-        tile: Point
-            Tile x, y coordinate.
-        z: float
-            Z coordinate.
-        path: str
-            Optical path.
-        crop: Union[bool, Region] = True
-            If to crop tile to image size (True, default) or to region.
+        path: Union[str, Sequence[str], Path, Sequence[Path]]
+            Path to files to test.
 
         Returns
-        ----------
-        bytes
-            Tile image as bytes.
+            True if files in path have one level that can be read with WsiDicom.
         """
-        tile_frame = self._get_encoded_tile(tile, z, path)
-        if crop is False:
-            return tile_frame
-
-        if isinstance(crop, bool):
-            crop = self.image_region
-        # Check if tile is an edge tile that should be croped
-        cropped_tile_region = crop.inside_crop(tile, self.tile_size)
-        if cropped_tile_region.size != self.tile_size:
-            image = Image.open(io.BytesIO(tile_frame))
-            image.crop(box=cropped_tile_region.box_from_origin)
-            tile_frame = self.encode(image)
-        return tile_frame
+        source = WsiDicomFileSource(path)
+        return source.contains_levels
```

### Comparing `wsidicom-0.8.0/wsidicom/image_data/pillow_image_data.py` & `wsidicom-0.9.0/wsidicom/instance/pillow_image_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,41 +9,38 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from PIL import Image
 from PIL.Image import Image as PILImage
 from pydicom.uid import UID, JPEGBaseline8Bit
-
-from wsidicom.geometry import Point, Size, SizeMm
-from wsidicom.image_data import ImageData, ImageOrigin
+from wsidicom.geometry import (
+    Point,
+    Size,
+    SizeMm,
+)
+from wsidicom.instance.image_data import ImageData
+from wsidicom.instance.image_origin import ImageOrigin
 
 
 class PillowImageData(ImageData):
     def __init__(self, image: PILImage):
         self._image = image.convert("RGB")
 
     @classmethod
     def from_file(cls, file: Union[str, Path]) -> "PillowImageData":
         image = Image.open(file)
         return cls(image)
 
     @property
-    def files(self) -> List[Path]:
-        filename = getattr(self._image, "filename", None)
-        if filename is None:
-            return []
-        return [filename]
-
-    @property
     def transfer_syntax(self) -> UID:
         return JPEGBaseline8Bit
 
     @property
     def image_size(self) -> Size:
         return Size.from_tuple(self._image.size)
 
@@ -72,10 +69,7 @@
             raise ValueError("Can only get Point(0, 0) from non-tiled image.")
         return self._image
 
     def _get_encoded_tile(self, tile: Point, z: float, path: str) -> bytes:
         if tile != Point(0, 0):
             raise ValueError("Can only get Point(0, 0) from non-tiled image.")
         return self.encode(self._image)
-
-    def close(self):
-        self._image.close()
```

### Comparing `wsidicom-0.8.0/wsidicom/optical.py` & `wsidicom-0.9.0/wsidicom/optical.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,44 +18,50 @@
 from typing import Dict, List, Optional, Sequence
 
 import numpy as np
 from PIL.Image import Image as PILImage
 from pydicom.dataset import Dataset
 from pydicom.sequence import Sequence as DicomSequence
 
-from wsidicom.conceptcode import (ChannelDescriptionCode, ConceptCode,
-                                  IlluminationCode, IlluminationColorCode,
-                                  IlluminatorCode, ImagePathFilterCode,
-                                  LenseCode, LightPathFilterCode)
+from wsidicom.conceptcode import (
+    ChannelDescriptionCode,
+    ConceptCode,
+    IlluminationCode,
+    IlluminationColorCode,
+    IlluminatorCode,
+    ImagePathFilterCode,
+    LenseCode,
+    LightPathFilterCode,
+)
 from wsidicom.errors import WsiDicomNotFoundError
 from wsidicom.instance import WsiInstance
 
 
 class Lut:
     """Represents a LUT."""
+
     def __init__(self, lut_sequence: DicomSequence):
         """Read LUT from a DICOM LUT sequence.
 
         Parameters
         ----------
         size: int
             the number of entries in the table
         bits: int
             the bits for each entry (currently forced to 16)
         """
         self._lut_item = lut_sequence[0]
-        length, first, bits = \
-            self._lut_item.RedPaletteColorLookupTableDescriptor
+        length, first, bits = self._lut_item.RedPaletteColorLookupTableDescriptor
         self._length = length
         self._bits = bits
         if bits == 8:
             self._type = np.dtype(np.uint8)
         else:
             self._type = np.dtype(np.uint16)
-        self._byte_format = 'HHH'  # Do we need to set endianess?
+        self._byte_format = "HHH"  # Do we need to set endianess?
         self.table = self._parse_lut(self._lut_item)
 
     def array(self, mode: str) -> np.ndarray:
         """Return flattened representation of the lookup table with order
         suitable for use with Pillows point(). The lookup table is scaled to
         either 8 or 16 bit depending on mode.
 
@@ -65,19 +71,19 @@
             Image mode to produce lookup table for.
 
         Returns
         ----------
         np.ndarray
             Lookup table ordered by rgb, rgb ...
         """
-        if mode == 'L' or mode == 'I':
+        if mode == "L" or mode == "I":
             bits = 16
         else:
             bits = 8
-        return self.table.flatten()/(2**self._bits/2**bits)
+        return self.table.flatten() / (2**self._bits / 2**bits)
 
     def insert_into_ds(self, ds: Dataset) -> Dataset:
         """Codes and insert object into sequence in dataset.
 
         Parameters
         ----------
         ds: Dataset
@@ -89,16 +95,16 @@
             Dataset with object inserted.
 
         """
         ds.PaletteColorLookupTableSequence = DicomSequence([self._lut_item])
         return ds
 
     @classmethod
-    def from_ds(cls, ds: Dataset) -> Optional['Lut']:
-        if('PaletteColorLookupTableSequence' in ds):
+    def from_ds(cls, ds: Dataset) -> Optional["Lut"]:
+        if "PaletteColorLookupTableSequence" in ds:
             return cls(ds.PaletteColorLookupTableSequence)
         return None
 
     def get(self) -> np.ndarray:
         """Return 2D representation of the lookup table.
 
         Returns
@@ -106,35 +112,26 @@
         np.ndarray
             Lookup table ordered by color x entry
         """
         return self.table
 
     def _parse_color(self, segmented_lut_data: bytes):
         LENGTH = 6
-        parsed_table = np.ndarray((0, ), dtype=self._type)
-        for segment in range(int(len(segmented_lut_data)/LENGTH)):
+        parsed_table = np.ndarray((0,), dtype=self._type)
+        for segment in range(int(len(segmented_lut_data) / LENGTH)):
             segment_bytes = segmented_lut_data[
-                segment*LENGTH:segment*LENGTH+LENGTH
+                segment * LENGTH : segment * LENGTH + LENGTH
             ]
             lut_type, lut_length, lut_value = struct.unpack(
-                self._byte_format,
-                segment_bytes
+                self._byte_format, segment_bytes
             )
-            if(lut_type == 0):
-                parsed_table = self._add_discret(
-                    parsed_table,
-                    lut_length,
-                    lut_value
-                )
-            elif(lut_type == 1):
-                parsed_table = self._add_linear(
-                    parsed_table,
-                    lut_length,
-                    lut_value
-                )
+            if lut_type == 0:
+                parsed_table = self._add_discret(parsed_table, lut_length, lut_value)
+            elif lut_type == 1:
+                parsed_table = self._add_linear(parsed_table, lut_length, lut_value)
             else:
                 raise NotImplementedError("Unkown lut segment type")
         return parsed_table
 
     def _parse_lut(self, lut: Dataset) -> np.ndarray:
         """Parse a dicom Palette Color Lookup Table Sequence item.
 
@@ -205,34 +202,32 @@
         # first value in segment
         try:
             last_value = table[-1]
         except IndexError:
             last_value = 0
             start_position = 0
         segment = np.linspace(
-            start=last_value,
-            stop=value,
-            num=start_position+length,
-            dtype=table.dtype
+            start=last_value, stop=value, num=start_position + length, dtype=table.dtype
         )
         table = cls._insert(table, segment[start_position:])
         return table
 
 
 @dataclass
 class OpticalFilter(metaclass=ABCMeta):
     """Metaclass for filter conditions for optical path"""
+
     filters: Optional[List[ConceptCode]]
     nominal: Optional[float]
     low_pass: Optional[float]
     high_pass: Optional[float]
 
     @classmethod
     @abstractmethod
-    def from_ds(cls, ds: Dataset) -> 'OpticalFilter':
+    def from_ds(cls, ds: Dataset) -> "OpticalFilter":
         raise NotImplementedError()
 
     def insert_into_ds(self, ds: Dataset) -> Dataset:
         """Codes and insert object into dataset.
 
         Parameters
         ----------
@@ -244,105 +239,105 @@
         Dataset
             Dataset with object inserted.
 
         """
         if self.nominal is not None:
             ds.LightPathFilterPassBand = self.nominal
         if self.low_pass is not None and self.high_pass is not None:
-            ds.LightPathFilterPassThroughwavelength = [
-                self.low_pass,
-                self.high_pass
-            ]
+            ds.LightPathFilterPassThroughwavelength = [self.low_pass, self.high_pass]
         if self.filters is not None:
             for filter in self.filters:
                 ds = filter.insert_into_ds(ds)
         return ds
 
 
 @dataclass
 class LightPathFilter(OpticalFilter):
     """Set of light path filter conditions for optical path"""
+
     filters: Optional[List[LightPathFilterCode]]
 
     @classmethod
-    def from_ds(cls, ds: Dataset) -> 'LightPathFilter':
+    def from_ds(cls, ds: Dataset) -> "LightPathFilter":
         """Returns LightPathFilter object read from dataset
         (optical path sequence item).
 
         Parameters
         ----------
         ds: Dataset
            Optical path sequence item.
 
         Returns
         ----------
         LightPathFilter
             Object containing light path filter conditions for optical path.
 
         """
-        filter_band = getattr(ds, 'LightPathFilterPassBand', [None, None])
+        filter_band = getattr(ds, "LightPathFilterPassBand", [None, None])
         return cls(
             filters=LightPathFilterCode.from_ds(ds),
-            nominal=getattr(ds, 'LightPathFilterPassThroughwavelengthh', None),
+            nominal=getattr(ds, "LightPathFilterPassThroughwavelengthh", None),
             low_pass=filter_band[0],
-            high_pass=filter_band[1]
+            high_pass=filter_band[1],
         )
 
 
 @dataclass
 class ImagePathFilter(OpticalFilter):
     """Set of image path filter conditions for optical path"""
+
     filters: Optional[List[ImagePathFilterCode]]
 
     @classmethod
-    def from_ds(cls, ds: Dataset) -> 'ImagePathFilter':
+    def from_ds(cls, ds: Dataset) -> "ImagePathFilter":
         """Returns ImagePathFilter object read from dataset
         (optical path sequence item).
 
         Parameters
         ----------
         ds: Dataset
            Optical path sequence item.
 
         Returns
         ----------
         ImagePathFilter
             Object containing image path filter conditions for optical path.
 
         """
-        filter_band = getattr(ds, 'ImagePathFilterPassBand', [None, None])
+        filter_band = getattr(ds, "ImagePathFilterPassBand", [None, None])
         return cls(
             filters=ImagePathFilterCode.from_ds(ds),
-            nominal=getattr(ds, 'ImagePathFilterPassThroughwavelengthh', None),
+            nominal=getattr(ds, "ImagePathFilterPassThroughwavelengthh", None),
             low_pass=filter_band[0],
-            high_pass=filter_band[1]
+            high_pass=filter_band[1],
         )
 
 
 @dataclass
 class Illumination:
     """Set of illumination conditions for optical path"""
+
     def __init__(
         self,
         illumination_method: Optional[Sequence[IlluminationCode]] = None,
         illumination_wavelength: Optional[float] = None,
         illumination_color: Optional[IlluminationColorCode] = None,
-        illuminator: Optional[IlluminatorCode] = None
+        illuminator: Optional[IlluminatorCode] = None,
     ):
         if illumination_color is None and illumination_wavelength is None:
             raise ValueError("Illumination color or wavelength need to be set")
         if illumination_method is None:
             illumination_method = []
         self.illumination_method = illumination_method
         self.illumination_wavelength = illumination_wavelength
         self.illumination_color = illumination_color
         self.illuminator = illuminator
 
     @classmethod
-    def from_ds(cls, ds: Dataset) -> 'Illumination':
+    def from_ds(cls, ds: Dataset) -> "Illumination":
         """Returns Illuminatin object read from dataset (optical path sequence
         item).
 
         Parameters
         ----------
         ds: Dataset
            Optical path sequence item.
@@ -351,19 +346,17 @@
         ----------
         Illumination
             Object containing illumination conditions for optical path.
 
         """
         return cls(
             illumination_method=IlluminationCode.from_ds(ds),
-            illumination_wavelength=getattr(
-                ds, 'IlluminationWaveLength', None
-            ),
+            illumination_wavelength=getattr(ds, "IlluminationWaveLength", None),
             illumination_color=IlluminationColorCode.from_ds(ds),
-            illuminator=IlluminatorCode.from_ds(ds)
+            illuminator=IlluminatorCode.from_ds(ds),
         )
 
     def insert_into_ds(self, ds: Dataset) -> Dataset:
         """Codes and insert object into dataset.
 
         Parameters
         ----------
@@ -386,21 +379,22 @@
             ds = item.insert_into_ds(ds)
         return ds
 
 
 @dataclass
 class Lenses:
     """Set of lens conditions for optical path"""
+
     lenses: Optional[List[LenseCode]]
     condenser_power: Optional[float]
     objective_power: Optional[float]
     objective_na: Optional[float]
 
     @classmethod
-    def from_ds(cls, ds: Dataset) -> 'Lenses':
+    def from_ds(cls, ds: Dataset) -> "Lenses":
         """Returns Lenses object read from dataset (optical path sequence
         item).
 
         Parameters
         ----------
         ds: Dataset
            Optical path sequence item.
@@ -409,17 +403,17 @@
         ----------
         Lenses
             Object containing lense conditions for optical path.
 
         """
         return cls(
             lenses=LenseCode.from_ds(ds),
-            condenser_power=getattr(ds, 'CondenserLensPower', None),
-            objective_power=getattr(ds, 'ObjectiveLensPower', None),
-            objective_na=getattr(ds, 'ObjectiveLensNumericalAperture', None)
+            condenser_power=getattr(ds, "CondenserLensPower", None),
+            objective_power=getattr(ds, "ObjectiveLensPower", None),
+            objective_na=getattr(ds, "ObjectiveLensNumericalAperture", None),
         )
 
     def insert_into_ds(self, ds: Dataset) -> Dataset:
         """Codes and insert object into dataset.
 
         Parameters
         ----------
@@ -443,26 +437,27 @@
                 ds = lense.insert_into_ds(ds)
         return ds
 
 
 @dataclass
 class OpticalPath:
     """Represents an optical path"""
+
     def __init__(
         self,
         identifier: str,
         illumination: Illumination,
         photometric_interpretation: str,
         description: Optional[str] = None,
         icc_profile: Optional[bytes] = None,
         lut: Optional[Lut] = None,
         light_path_filter: Optional[LightPathFilter] = None,
         image_path_filter: Optional[ImagePathFilter] = None,
         channel_description: Optional[Sequence[ChannelDescriptionCode]] = None,
-        lenses: Optional[Lenses] = None
+        lenses: Optional[Lenses] = None,
     ):
         """Create a OpticalPath from identifier, illumination, photometric
         interpretation, and optional attributes.
 
         Parameters
         ----------
         identifier: str
@@ -496,15 +491,15 @@
         self.image_path_filter = image_path_filter
         self.channel_description = channel_description
         self.lenses = lenses
 
     def __str__(self):
         string = self.identifier
         if self.description is not None:
-            string += ' - ' + self.description
+            string += " - " + self.description
         return string
 
     def to_ds(self) -> Dataset:
         ds = Dataset()
         ds.OpticalPathIdentifier = self.identifier
         ds = self.illumination.insert_into_ds(ds)
         if self.description is not None:
@@ -521,19 +516,15 @@
             for item in self.channel_description:
                 ds = item.insert_into_ds(ds)
         if self.lenses is not None:
             ds = self.lenses.insert_into_ds(ds)
         return ds
 
     @classmethod
-    def from_ds(
-        cls,
-        ds: Dataset,
-        photometric_interpretation: str
-    ) -> 'OpticalPath':
+    def from_ds(cls, ds: Dataset, photometric_interpretation: str) -> "OpticalPath":
         """Create new optical path item populated with optical path
         identifier, description, icc profile name and lookup table.
 
         Parameters
         ----------
         optical_path: Dataset
             Optical path dataset containing the optical path data
@@ -545,46 +536,46 @@
         OpticalPath
             New optical path item
         """
         return OpticalPath(
             identifier=str(ds.OpticalPathIdentifier),
             illumination=Illumination.from_ds(ds),
             photometric_interpretation=photometric_interpretation,
-            description=getattr(ds, 'OpticalPathDescription', None),
-            icc_profile=getattr(ds, 'ICCProfile', None),
+            description=getattr(ds, "OpticalPathDescription", None),
+            icc_profile=getattr(ds, "ICCProfile", None),
             lut=Lut.from_ds(ds),
             light_path_filter=LightPathFilter.from_ds(ds),
             image_path_filter=ImagePathFilter.from_ds(ds),
             channel_description=ChannelDescriptionCode.from_ds(ds),
             lenses=Lenses.from_ds(ds),
         )
 
 
 class OpticalManager:
     """Store optical paths loaded from dicom files."""
+
     def __init__(
         self,
         optical_paths: Optional[Sequence[OpticalPath]] = None,
     ):
         """Create a OpticalManager from list of OpticalPaths.
 
         Parameters
         ----------
          optical_paths: Optional[Sequence[OpticalPath]] = None
             List of OpticalPaths.
         """
         if optical_paths is None:
             optical_paths = []
         self._optical_paths: Dict[str, OpticalPath] = {
-            optical_path.identifier: optical_path
-            for optical_path in optical_paths
+            optical_path.identifier: optical_path for optical_path in optical_paths
         }
 
     @classmethod
-    def open(cls, instances: Sequence[WsiInstance]) -> 'OpticalManager':
+    def open(cls, instances: Sequence[WsiInstance]) -> "OpticalManager":
         """Parse optical path sequence in listed instances and create an
         OpticalManager out of the found (unique) OpticalPaths.
 
         Parameters
         ----------
         files: Sequence[WsiInstance]
             List of WsiDicom instances to parse
@@ -600,16 +591,15 @@
                 optical_path_sequence = dataset.optical_path_sequence
                 if optical_path_sequence is None:
                     continue
                 for optical_path in optical_path_sequence:
                     identifier = str(optical_path.OpticalPathIdentifier)
                     if identifier not in optical_paths:
                         path = OpticalPath.from_ds(
-                            optical_path,
-                            dataset.PhotometricInterpretation
+                            optical_path, dataset.PhotometricInterpretation
                         )
                         optical_paths[identifier] = path
         return cls(list(optical_paths.values()))
 
     def insert_into_ds(self, ds: Dataset) -> Dataset:
         """Codes and insert object into dataset.
 
@@ -621,27 +611,25 @@
         Returns
         ----------
         Dataset
             Dataset with object inserted.
 
         """
         ds.NumberOfOpticalPaths = len(self._optical_paths)
-        ds.OpticalPathSequence = DicomSequence([
-            optical_path.to_ds()
-            for optical_path in self._optical_paths.values()
-        ])
+        ds.OpticalPathSequence = DicomSequence(
+            [optical_path.to_ds() for optical_path in self._optical_paths.values()]
+        )
         return ds
 
     def get(self, identifier: str) -> OpticalPath:
         try:
             return self._optical_paths[identifier]
         except KeyError:
             raise WsiDicomNotFoundError(
-                f"identifier {identifier}",
-                "optical path manager"
+                f"identifier {identifier}", "optical path manager"
             )
 
     def apply_lut(self, image: PILImage, identifier: str) -> PILImage:
         """Apply LUT of identifier to image. Converts gray scale image to RGB.
 
         Parameters
         ----------
@@ -656,13 +644,12 @@
             Image with LUT applied.
         """
 
         path = self.get(identifier)
         lut = path.lut
         if lut is None:
             raise WsiDicomNotFoundError(
-                f"Lut for identifier {identifier}",
-                "optical path manager"
+                f"Lut for identifier {identifier}", "optical path manager"
             )
         # if(image.mode == 'L'):
         #     image = image.convert('RGB')
         return image.point(lut.array(image.mode))
```

### Comparing `wsidicom-0.8.0/wsidicom/stringprinting.py` & `wsidicom-0.9.0/wsidicom/stringprinting.py`

 * *Files identical despite different names*

### Comparing `wsidicom-0.8.0/wsidicom/uid.py` & `wsidicom-0.9.0/wsidicom/uid.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,73 +16,74 @@
 from typing import Optional
 
 from pydicom.uid import UID
 
 from wsidicom.config import settings
 from wsidicom.errors import WsiDicomStrictRequirementError
 
-WSI_SOP_CLASS_UID = UID('1.2.840.10008.5.1.4.1.1.77.1.6')
-ANN_SOP_CLASS_UID = UID('1.2.840.10008.5.1.4.1.1.91.1')
+WSI_SOP_CLASS_UID = UID("1.2.840.10008.5.1.4.1.1.77.1.6")
+ANN_SOP_CLASS_UID = UID("1.2.840.10008.5.1.4.1.1.91.1")
 
 
 @dataclass
 class SlideUids:
     """Represents the UIDs that should be common for all files of a slide."""
+
     study_instance: UID
     series_instance: UID
     frame_of_reference: Optional[UID] = None
 
     def __init__(
         self,
         study_instance: UID,
         series_instance: UID,
-        frame_of_reference: Optional[UID] = None
+        frame_of_reference: Optional[UID] = None,
     ) -> None:
         if settings.strict_uid_check and frame_of_reference is None:
             raise WsiDicomStrictRequirementError(
-                'Frame of reference uid is missing and strict uid check is '
-                'enabled'
+                "Frame of reference uid is missing and strict uid check is " "enabled"
             )
         self.study_instance = study_instance
         self.series_instance = series_instance
         self.frame_of_reference = frame_of_reference
 
     def __str__(self) -> str:
         return (
             f"SlideUids study: {self.study_instance}, "
             f"series: {self.series_instance}, "
             f"frame of reference {self.frame_of_reference}"
         )
 
-    def __eq__(self, other: 'SlideUids') -> bool:
+    def __eq__(self, other: "SlideUids") -> bool:
         if isinstance(other, SlideUids):
             return (
-                self.study_instance == other.study_instance and
-                self.series_instance == other.series_instance and
-                (
-                    self.frame_of_reference == other.frame_of_reference or
-                    self.frame_of_reference is None or
-                    other.frame_of_reference is None
+                self.study_instance == other.study_instance
+                and self.series_instance == other.series_instance
+                and (
+                    self.frame_of_reference == other.frame_of_reference
+                    or self.frame_of_reference is None
+                    or other.frame_of_reference is None
                 )
             )
         return NotImplemented
 
-    def matches(self, other: 'SlideUids') -> bool:
+    def matches(self, other: "SlideUids") -> bool:
         if settings.strict_uid_check:
             return self == other
 
         return (
-            self.study_instance == other.study_instance and
-            self.series_instance == other.series_instance
+            self.study_instance == other.study_instance
+            and self.series_instance == other.series_instance
         )
 
 
 @dataclass
 class FileUids:
     """Represents the UIDs in a DICOM-file."""
+
     instance: UID
     concatenation: Optional[UID]
     slide: SlideUids
 
     @property
     def identifier(self) -> UID:
         """Return identifier for the instance the file belongs to. Either its
@@ -93,15 +94,15 @@
         UID
             Identifier uid for the instance the file belongs to.
         """
         if self.concatenation is not None:
             return self.concatenation
         return self.instance
 
-    def __eq__(self, other: 'FileUids') -> bool:
+    def __eq__(self, other: "FileUids") -> bool:
         """Return true if concatenation uid is not none, matches other
         concatenation uid and base uids match.
 
         Parameters
         ----------
         other: FileUids
             File uids to match to.
@@ -109,12 +110,12 @@
         Returns
         ----------
         bool
             True if concatenation is matching.
         """
         if isinstance(other, FileUids):
             return (
-                self.concatenation is not None and
-                self.concatenation == other.concatenation and
-                self.slide == other.slide
+                self.concatenation is not None
+                and self.concatenation == other.concatenation
+                and self.slide == other.slide
             )
         return NotImplemented
```

### Comparing `wsidicom-0.8.0/PKG-INFO` & `wsidicom-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsidicom
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools for handling DICOM based whole scan images
 Home-page: https://github.com/imi-bigpicture/wsidicom
 License: Apache-2.0
 Keywords: whole slide image,digital pathology,annotations,dicom
 Author: Erik O Gabrielsson
 Author-email: erik.o.gabrielsson@sectra.com
 Requires-Python: >=3.8,<3.12
@@ -17,24 +17,25 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Dist: Pillow (>=9.1.1,<10.0.0)
+Requires-Dist: dicomweb-client (>=0.59.1,<0.60.0)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: pydicom (>=2.1.0,<3.0.0)
 Project-URL: Repository, https://github.com/imi-bigpicture/wsidicom
 Description-Content-Type: text/markdown
 
 # *wsidicom*
 
-*wsidicom* is a Python package for reading [DICOM WSI](http://dicom.nema.org/Dicom/DICOMWSI/) file sets. The aims with the project are:
+*wsidicom* is a Python package for reading [DICOM WSI](http://dicom.nema.org/Dicom/DICOMWSI/). The aims with the project are:
 
-- Easy to use interface for reading and writing WSI DICOM images and annotations using the DICOM Media Storage Model.
+- Easy to use interface for reading and writing WSI DICOM images and annotations either from file or through DICOMWeb.
 - Support the latest and upcoming DICOM standards.
 - Platform independent installation via PyPI.
 
 ## Installing *wsidicom*
 
 *wsidicom* is available on PyPI:
 
@@ -50,15 +51,15 @@
 
 ## Important note
 
 Please note that this is an early release and the API is not frozen yet. Function names and functionality is prone to change.
 
 ## Requirements
 
-*wsidicom* uses pydicom, numpy and Pillow (with jpeg and jpeg2000 plugins).
+*wsidicom* uses pydicom, numpy, Pillow (with jpeg and jpeg2000 plugins), and dicomweb-client.
 
 ## Limitations
 
 Levels are required to have (close to) 2 factor scale and same tile size.
 
 Only JPEGBaseline8Bit, JPEG2000 and JPEG2000Lossless transfer syntax is supported.
 
@@ -69,120 +70,129 @@
 ***Load a WSI dataset from files in folder.***
 
 ```python
 from wsidicom import WsiDicom
 slide = WsiDicom.open(path_to_folder)
 ```
 
+***Or load a WSI dataset from DICOMWeb.***
+
+```python
+from wsidicom import WsiDicom, WsiDicomWebClient
+from requests.auth import HTTPBasicAuth
+
+auth = HTTPBasicAuth('username', 'password')
+client = WsiDicomWebClient(
+    'dicom_web_hostname',
+    '/qido',
+    '/wado,
+    auth
+)
+slide = WsiDicom.open_web(
+    client,
+    "study uid to open",
+    "series uid top open"
+)
+```
+
+***Use as a context manager.***
+
+```python
+from wsidicom import WsiDicom
+with WsiDicom.open(path_to_folder) as slide:
+    ...
+```
+
 ***Read a 200x200 px region starting from px 1000, 1000 at level 6.***
 
- ```python
+```python
 region = slide.read_region((1000, 1000), 6, (200, 200))
 ```
 
+***Read a 2000x2000 px region starting from px 1000, 1000 at level 4 using 4 threads.***
+
+```python
+region = slide.read_region((1000, 1000), 6, (200, 200), threads=4)
+```
+
 ***Read 3x3 mm region starting at 0, 0 mm at level 6.***
 
- ```python
+```python
 region_mm = slide.read_region_mm((0, 0), 6, (3, 3))
 ```
 
 ***Read 3x3 mm region starting at 0, 0 mm with pixel spacing 0.01 mm/px.***
 
- ```python
+```python
 region_mpp = slide.read_region_mpp((0, 0), 0.01, (3, 3))
 ```
 
 ***Read a thumbnail of the whole slide with maximum dimensions 200x200 px.***
 
- ```python
+```python
 thumbnail = slide.read_thumbnail(200, 200)
 ```
 
 ***Read an overview image (if available).***
 
- ```python
+```python
 overview = slide.read_overview()
 ```
 
 ***Read a label image (if available).***
 
- ```python
+```python
 label = slide.read_label()
 ```
 
 ***Read (decoded) tile from position 1, 1 in level 6.***
 
- ```python
+```python
 tile = slide.read_tile(6, (1, 1))
 ```
 
 ***Read (encoded) tile from position 1, 1 in level 6.***
 
- ```python
+```python
 tile_bytes = slide.read_encoded_tile(6, (1, 1))
 ```
 
 ***Close files***
 
- ```python
-slide.close()
-```
-
-## Settings
-
-*wsidicom* can be configured with the settings variable. For example, set the parsing of files to strict:
-
 ```python
-from wsidicom import settings
-settings.strict_uid_check = True
-settings._strict_attribute_check = True
+slide.close()
 ```
 
-## Data structure
-
-A WSI DICOM pyramid is in *wsidicom* represented by a hierarchy of objects of different classes, starting from bottom:
+## Saving files
 
-- *WsiDicomFile*, represents a WSI DICOM file, used for accessing DicomImageData and WsiDataset.
-- *DicomImageData*, represents the image data in one or several WSI DICOM files.
-- *WsiDataset*, represents the image metadata in one or several WSI DICOM files.
-- *WsiInstance*, represents image data and image metadata.
-- *WsiDicomLevel*, represents a group of instances with the same image size, i.e. of the same level.
-- *WsiDicomLevels*, represents a group of levels, i.e. the pyrimidal structure.
-- *WsiDicom*, represents a collection of levels, labels and overviews.
+An opened WsiDicom instance can be saved to a new path using the save()-method. The produced files will be:
 
-Labels and overviews are structured similarly to levels, but with somewhat different properties and restrictions.
+- Fully tiled. Any sparse tiles will be replaced with a blank tile with color depending on the photometric interpretation.
+- Have a basic offset table (or optionally an exteded offset table or no offset table).
+- Not be concatenated.
 
-The structure is easiest created using the open() helper functions, e.g. to create a WsiDicom-object:
+The frames are copied as-is, i.e. without re-compression.
 
 ```python
-slide = WsiDicom.open(path_to_folder)
+with WsiDicom.open(path_to_folder) as slide:
+    slide.save(path_to_output)
 ```
 
-But the structure can also be created manually from the bottom:
-
-```python
-file = WsiDicomFile(path_to_file)
-instance = WsiInstance(file.dataset, DicomImageData(files))
-level = WsiDicomLevel([instance])
-levels = WsiDicomLevels([level])
-slide = WsiDicom([levels])
-```
+The output folder must already exists. Be careful to specify a unique folder folder to avoid mixing files from diferent images.
 
-## Adding support for other file formats
+## Settings
 
-By subclassing *ImageData* and implementing the required properties (transfer_syntax, image_size, tile_size, and pixel_spacing) and methods (get_tile() and close()) *wsidicom* can be used to access wsi images in other file formats than DICOM. In addition to a ImageData-object, image data, specified in a DICOM dataset, must also be created. For example, assuming a implementation of MyImageData exists that takes a path to a image file as argument and create_dataset() produces a DICOM dataset (see is_wsi_dicom() of WsiDataset for required attributes), WsiInstancees could be created for each pyramidal level, label, or overview:
+*wsidicom* can be configured with the settings variable. For example, set the parsing of files to strict:
 
 ```python
-image_data = MyImageData('path_to_image_file')
-dataset = create_dataset()
-instance = WsiInstance(dataset, image_data)
+from wsidicom import settings
+settings.strict_uid_check = True
+settings._strict_attribute_check = True
 ```
 
-The created instances can then be arranged into levels etc, and opened as a WsiDicom-object as described in 'Data structure'.
-
 ## Annotation usage
 
 Annotations are structured in a hierarchy:
 
 - AnnotationInstance
     Represents a collection of AnnotationGroups. All the groups have the same frame of reference, i.e. annotations are from the same wsi stack.
 - AnnotationGroup
@@ -278,18 +288,72 @@
 
 To run integration tests:
 
 ```console
 poetry run pytest -m integration
 ```
 
+## Data structure
+
+A WSI DICOM pyramid is in *wsidicom* represented by a hierarchy of objects of different classes, starting from bottom:
+
+- *WsiDicomFile*, represents a WSI DICOM file, used for accessing WsiDicomFileImageData and WsiDataset.
+- *WsiDicomFileImageData*, represents the image data in one or several WSI DICOM files.
+- *WsiDataset*, represents the image metadata in one or several WSI DICOM files.
+- *WsiInstance*, represents image data and image metadata.
+- *Level*, represents a group of instances with the same image size, i.e. of the same level.
+- *Levels*, represents a group of levels, i.e. the pyrimidal structure.
+- *WsiDicom*, represents a collection of levels, labels and overviews.
+
+Labels and overviews are structured similarly to levels, but with somewhat different properties and restrictions. For DICOMWeb the WsiDicomFile\* classes are replaced with WsiDicomWeb\* classes.
+
+A Source is used to create WsiInstances, either from files (*WsiDicomFileSource*) or DICOMWeb (*WsiDicomWebSource*), and can be used to to initate a *WsiDicom* object. A source is easiest created with the open() and open_web() helper functions, e.g.:
+
+```python
+slide = WsiDicom.open(path_to_folder)
+```
+
+## Code structure
+
+- [wsidicom.py](wsidicom/wsidicom.py) - Main class with methods to open DICOM WSI objects.
+- [source.py](wsidicom/source.py) - Metaclass Source for serving WsiInstances to WsiDicom.
+- [series](wsidicom/series) - Series implementations Levels, Labels, and Overview.
+- [group](wsidicom/group) - Group implementations, e.g. Level.
+- [instance](wsidicom/instance) - Instance implementations WsiIsntance and WsiDataset, the metaclass ImageData and ImageData implementations WsiDicomImageData and PillowImageData.
+- [file](wsidicom/file) - Implementation for reading and writing DICOM WSI files.
+- [web](wsidicom/web) - Implementation for reading DICOM WSI from DICOMWeb.
+- [graphica_annotations](wsidicom/graphical_annotations.py) - Handling graphical annotations.
+- [conceptcode.py](wsidicom/conceptcode.py) - Handling of DICOM concept codes.
+- [config.py](wsidicom/config.py) - Handles configuration settings.
+- [errors.py](wsidicom/errors.py) - Custom errors.
+- [geometry.py](wsidicom/geometry.py) - Classes for geometry handling.
+- [optical.py](wsidicom/optical.py) - Handles optical paths.
+- [uid.py](wsidicom/uid.py) - Handles DICOM uids.
+- [stringprinting.py](wsidicom/stringprinting.py) - For nicer string printing of objects.
+
+## Adding support for other file formats
+
+Support for other formats (or methods to access DICOM data) can be implemented by creating a new Source implementation, that should create WsiInstances for the implemented formats. A format specific implementations of the *ImageData* is likely needed to access the WSI image data. Additionally a WsiDataset needs to be created that returns matching metadata for the WSI.
+
+The implemented Source can then create a instance from the implemented ImageData (and a method returning a WsiDataset):
+
+```python
+image_data = MyImageData('path_to_image_file')
+dataset = create_dataset_from_image_data(image_data)
+instance = WsiInstance(dataset, image_data)
+```
+
+The source should arrange the created instances and return them at the level_instances, label_instances, and overview_instances properties. WsiDicom can then open the source object and arrange the instances into levels etc as described in 'Data structure'.
+
 ## Other DICOM python tools
 
 - [pydicom](https://pydicom.github.io/)
 - [highdicom](https://github.com/MGHComputationalPathology/highdicom)
+- [wsidicomizer](https://github.com/imi-bigpicture/wsidicomizer)
+- [dicomslide](https://github.com/ImagingDataCommons/dicomslide)
 
 ## Contributing
 
 We welcome any contributions to help improve this tool for the WSI DICOM community!
 
 We recommend first creating an issue before creating potential contributions to check that the contribution is in line with the goals of the project. To submit your contribution, please issue a pull request on the imi-bigpicture/wsidicom repository with your changes for review.
```

