# Comparing `tmp/ocrd_wrap-0.1.7.tar.gz` & `tmp/ocrd_wrap-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_wrap-0.1.7.tar", last modified: Sun Mar  7 17:31:13 2021, max compression
+gzip compressed data, was "dist/ocrd_wrap-0.1.8.tar", last modified: Thu Jun  1 16:42:59 2023, max compression
```

## Comparing `ocrd_wrap-0.1.7.tar` & `ocrd_wrap-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/
-drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap.egg-info/
--rw-r--r--   0 xbert     (1000) xbert     (1000)      419 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap.egg-info/SOURCES.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)       10 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap.egg-info/top_level.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)    22497 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap.egg-info/PKG-INFO
--rw-r--r--   0 xbert     (1000) xbert     (1000)       77 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap.egg-info/requires.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)        1 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap.egg-info/dependency_links.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)      325 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap.egg-info/entry_points.txt
-drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/ocrd_wrap/
--rw-r--r--   0 xbert     (1000) xbert     (1000)     9001 2020-11-01 16:44:46.000000 ocrd_wrap-0.1.7/ocrd_wrap/skimage_denoise_raw.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     8660 2021-03-07 17:28:11.000000 ocrd_wrap-0.1.7/ocrd_wrap/skimage_denoise.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)      138 2020-06-08 19:07:42.000000 ocrd_wrap-0.1.7/ocrd_wrap/config.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     1062 2020-06-09 21:45:51.000000 ocrd_wrap-0.1.7/ocrd_wrap/cli.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)    10786 2020-11-03 11:46:12.000000 ocrd_wrap-0.1.7/ocrd_wrap/shell.py
--rw-rw-r--   0 xbert     (1000) xbert     (1000)       71 2020-06-08 18:51:28.000000 ocrd_wrap-0.1.7/ocrd_wrap/__init__.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     9299 2020-11-03 11:45:18.000000 ocrd_wrap-0.1.7/ocrd_wrap/skimage_normalize.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     8641 2020-11-01 16:44:46.000000 ocrd_wrap-0.1.7/ocrd_wrap/skimage_binarize.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)    18692 2020-11-01 16:44:46.000000 ocrd_wrap-0.1.7/README.md
--rw-rw-r--   0 xbert     (1000) xbert     (1000)     1446 2020-06-09 21:45:29.000000 ocrd_wrap-0.1.7/setup.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)    22497 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/PKG-INFO
--rw-r--r--   0 xbert     (1000) xbert     (1000)       38 2021-03-07 17:31:13.000000 ocrd_wrap-0.1.7/setup.cfg
+drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-06-01 16:42:59.519815 ocrd_wrap-0.1.8/
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)     1060 2023-05-31 13:27:51.000000 ocrd_wrap-0.1.8/LICENSE
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    19016 2023-06-01 16:42:59.519815 ocrd_wrap-0.1.8/PKG-INFO
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    18692 2023-05-31 13:27:51.000000 ocrd_wrap-0.1.8/README.md
+drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-06-01 16:42:59.515814 ocrd_wrap-0.1.8/ocrd_wrap/
+-rw-r--r--   0 xbert     (1000) xbert     (1000)       71 2020-06-10 08:10:57.000000 ocrd_wrap-0.1.8/ocrd_wrap/__init__.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     1062 2020-06-10 08:10:57.000000 ocrd_wrap-0.1.8/ocrd_wrap/cli.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      138 2020-06-10 08:10:57.000000 ocrd_wrap-0.1.8/ocrd_wrap/config.py
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    10834 2023-06-01 16:41:56.000000 ocrd_wrap-0.1.8/ocrd_wrap/ocrd-tool.json
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      552 2020-06-10 08:10:57.000000 ocrd_wrap-0.1.8/ocrd_wrap/param_im6convert-denoise-raw.json
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      704 2020-06-10 08:10:57.000000 ocrd_wrap-0.1.8/ocrd_wrap/param_scribo-cli-binarize-sauvola-ms-split.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    10786 2023-05-31 13:27:51.000000 ocrd_wrap-0.1.8/ocrd_wrap/shell.py
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)     8641 2023-05-31 13:27:51.000000 ocrd_wrap-0.1.8/ocrd_wrap/skimage_binarize.py
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)     8776 2023-06-01 16:40:17.000000 ocrd_wrap-0.1.8/ocrd_wrap/skimage_denoise.py
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)     9001 2023-05-31 13:27:51.000000 ocrd_wrap-0.1.8/ocrd_wrap/skimage_denoise_raw.py
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)     9299 2023-05-31 13:27:51.000000 ocrd_wrap-0.1.8/ocrd_wrap/skimage_normalize.py
+drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-06-01 16:42:59.519815 ocrd_wrap-0.1.8/ocrd_wrap.egg-info/
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    19016 2023-06-01 16:42:59.000000 ocrd_wrap-0.1.8/ocrd_wrap.egg-info/PKG-INFO
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      554 2023-06-01 16:42:59.000000 ocrd_wrap-0.1.8/ocrd_wrap.egg-info/SOURCES.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)        1 2023-06-01 16:42:59.000000 ocrd_wrap-0.1.8/ocrd_wrap.egg-info/dependency_links.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      324 2023-06-01 16:42:59.000000 ocrd_wrap-0.1.8/ocrd_wrap.egg-info/entry_points.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)       77 2023-06-01 16:42:59.000000 ocrd_wrap-0.1.8/ocrd_wrap.egg-info/requires.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)       10 2023-06-01 16:42:59.000000 ocrd_wrap-0.1.8/ocrd_wrap.egg-info/top_level.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)       38 2023-06-01 16:42:59.519815 ocrd_wrap-0.1.8/setup.cfg
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     1446 2020-06-10 08:10:57.000000 ocrd_wrap-0.1.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ocrd_wrap-0.1.7/ocrd_wrap.egg-info/PKG-INFO` & `ocrd_wrap-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,445 +1,445 @@
 Metadata-Version: 2.1
-Name: ocrd-wrap
-Version: 0.1.7
+Name: ocrd_wrap
+Version: 0.1.8
 Summary: OCR-D wrapper for arbitrary coords-preserving image operations
 Home-page: https://github.com/bertsky/ocrd_wrap
 Author: Robert Sachunsky
 Author-email: sachunsky@informatik.uni-leipzig.de
 License: MIT
-Description: [![PyPI version](https://badge.fury.io/py/ocrd-wrap.svg)](https://badge.fury.io/py/ocrd-wrap)
-        
-        # ocrd_wrap
-        
-            OCR-D wrapper for arbitrary coords-preserving image operations
-        
-          * [Introduction](#introduction)
-          * [Installation](#installation)
-          * [Usage](#usage)
-             * [OCR-D processor interface ocrd-preprocess-image](#ocr-d-processor-interface-ocrd-preprocess-image)
-             * [OCR-D processor interface ocrd-skimage-normalize](#ocr-d-processor-interface-ocrd-skimage-normalize)
-             * [OCR-D processor interface ocrd-skimage-denoise-raw](#ocr-d-processor-interface-ocrd-skimage-denoise-raw)
-             * [OCR-D processor interface ocrd-skimage-binarize](#ocr-d-processor-interface-ocrd-skimage-binarize)
-             * [OCR-D processor interface ocrd-skimage-denoise](#ocr-d-processor-interface-ocrd-skimage-denoise)
-          * [Testing](#testing)
-        
-        
-        ## Introduction
-        
-        This offers [OCR-D](https://ocr-d.de) compliant [workspace processors](https://ocr-d.de/en/spec/cli) for
-        any image processing tools which have some (usable) CLI
-        and do not modify/invalidate image coordinates.
-        
-        It thus _wraps_ them for OCR-D without the need
-        to write and manage code for each of them individually
-        (exposing/passing/documenting their parameters and usage,
-        managing releases etc). It shifts all the burden to
-        **workflow configuration** (i.e. defining a suitable
-        parameter set on how to call what program on what data,
-        and installing all the required tools).
-        
-        It is itself written in Python, and relies heavily on the
-        [OCR-D core API](https://github.com/OCR-D/core). This is
-        responsible for handling METS/PAGE, and providing the OCR-D
-        CLI.
-        
-        In addition, this aims to wrap existing Python packages
-        for preprocessing as OCR-D processors (one at a time).
-        
-        ## Installation
-        
-        Create and activate a [virtual environment](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments) as usual.
-        
-        To install Python dependencies:
-        
-            make deps
-        
-        Which is the equivalent of:
-        
-            pip install -r requirements.txt
-        
-        To install this module, then do:
-        
-            make install
-        
-        Which is the equivalent of:
-        
-            pip install .
-        
-        ## Usage
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-preprocess-image`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-preprocess-image [OPTIONS]
-        
-          Convert or enhance images
-        
-          > Performs coords-preserving image operations via runtime shell calls
-          > anywhere.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing.
-        
-          > If ``input_feature_selector`` and/or ``input_feature_filter`` is
-          > non-empty, then select/filter among the @imageFilename image and the
-          > available AlternativeImages the last one which contains all of the
-          > selected, but none of the filtered features (i.e. @comments
-          > classes), or raise an error.
-        
-          > Then write that image into a temporary PNG file, create a new METS
-          > file ID for the result image (based on the segment ID and the
-          > operation to be run), along with a local path for it, and pass
-          > ``command`` to the shell after replacing: - the string ``@INFILE``
-          > with that input image path, and - the string ``@OUTFILE`` with that
-          > output image path.
-        
-          > If the shell returns with a failure, skip that segment with an
-          > approriate error message. Otherwise, add the new image to the
-          > workspace along with the output fileGrp, and using a file ID with
-          > suffix ``.IMG-``, and further identification of the input element.
-        
-          > Reference it as AlternativeImage in the element, adding
-          > ``output_feature_added`` to its @comments.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "input_feature_selector" [string - ""]
-            comma-separated list of required image features (e.g.
-            binarized,despeckled)
-           "input_feature_filter" [string - ""]
-            comma-separated list of forbidden image features (e.g.
-            binarized,despeckled)
-           "output_feature_added" [string - REQUIRED]
-            image feature(s) to be added after this operation (if multiple,
-            separate by comma)
-           "input_mimetype" [string - "image/png"]
-            File format to save input images to (tool's expected input)
-            Possible values: ["image/bmp", "application/postscript", "image/gif",
-            "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
-            "image/tiff"]
-           "output_mimetype" [string - "image/png"]
-            File format to load output images from (tool's expected output)
-            Possible values: ["image/bmp", "application/postscript", "image/gif",
-            "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
-            "image/tiff"]
-           "command" [string - REQUIRED]
-            shell command to operate on image files, with @INFILE as place-holder
-            for the input file path, and @OUTFILE as place-holder for the output
-            file path
-        ```
-        
-        #### presets
-        
-        The following example recipes are included in the distribution:
-        - enhancement/conversion/denoising using
-          - [x] ImageMagick: [param_im6convert-denoise-raw](ocrd_wrap/param_im6convert-denoise-raw.json)
-          - [ ] GIMP [script-fu](https://gitlab.gnome.org/GNOME/gimp/-/tree/master/plug-ins/script-fu/scripts)
-          - [ ] ...
-        - binarization using 
-          - [x] Olena/Scribo: [param_scribo-cli-binarize-sauvola-ms-split](ocrd_wrap/param_scribo-cli-binarize-sauvola-ms-split.json)
-          - [ ] https://github.com/ajgallego/document-image-binarization ...
-          - [ ] https://github.com/qurator-spk/sbb_binarization ...
-          - [ ] https://github.com/masyagin1998/robin ...
-          - [ ] ...
-        - text/non-text segmentation using
-          - [ ] Olena/Scribo ...
-          - [ ] ...
-        - ...
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-normalize`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-normalize [OPTIONS]
-        
-          Equalize contrast/exposure of images with Scikit-image; stretches the color value/tone to the full dynamic range
-        
-          > Performs contrast-enhancing equalization of segment or page images
-          > with scikit-image on the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing), in raw (non-binarized) form.
-        
-          > Next, normalize the image according to ``method`` in skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-NRM`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "black-point" [number - 1.0]
-            black point point in percent of luminance/value/tone histogram; up to
-            ``black-point`` darkest pixels will be clipped to black when
-            stretching
-           "white-point" [number - 7.0]
-            white point in percent of luminance/value/tone histogram; up to
-            ``white-point`` brightest pixels will be clipped to white when
-            stretching
-           "method" [string - "stretch"]
-            contrast-enhancing transformation to use after clipping; ``stretch``
-            uses ``skimage.exposure.rescale_intensity`` (globally linearly
-            stretching to full dynamic range) and ``adapthist`` uses
-            ``skimage.exposure.equalize_adapthist`` (applying over tiles with
-            context from 1/8th of the image's width)
-            Possible values: ["stretch", "adapthist"]
-        ```
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise-raw`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-denoise-raw [OPTIONS]
-        
-          Denoise raw images with Scikit-image
-        
-          > Performs raw denoising of segment or page images with scikit-image
-          > on the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing), in raw (non-binarized) form.
-        
-          > Next, denoise the image with a Wavelet transform scheme according to
-          > ``method`` in skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "method" [string - "VisuShrink"]
-            Wavelet filtering scheme to use
-            Possible values: ["BayesShrink", "VisuShrink"]
-        ```
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-binarize`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-binarize [OPTIONS]
-        
-          Binarize images with Scikit-image
-        
-          > Performs binarization of segment or page images with scikit-image on
-          > the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing).
-        
-          > Next, binarize the image according to ``method`` with skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-BIN`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "method" [string - "sauvola"]
-            Thresholding algorithm to use
-            Possible values: ["sauvola", "niblack", "otsu", "gauss", "yen", "li"]
-           "window_size" [number - 0]
-            For Sauvola/Niblack/Gauss, the (odd) window size in pixels; when zero
-            (default), set to DPI
-           "k" [number - 0.34]
-            For Sauvola/Niblack, formula parameter influencing the threshold
-            bias; larger is lighter foreground
-        ```
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-denoise [OPTIONS]
-        
-          Denoise binarized images with Scikit-image
-        
-          > Performs binary denoising of segment or page images with scikit-
-          > image on the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing), in binarized form.
-        
-          > Next, denoise the image by removing too small connected components
-          > with skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "maxsize" [number - 3]
-            maximum component size of (bg holes or fg specks) noise in pt
-        ```
-        
-        ## Testing
-        
-        none yet
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/ocrd-wrap.svg)](https://badge.fury.io/py/ocrd-wrap)
+
+# ocrd_wrap
+
+    OCR-D wrapper for arbitrary coords-preserving image operations
+
+  * [Introduction](#introduction)
+  * [Installation](#installation)
+  * [Usage](#usage)
+     * [OCR-D processor interface ocrd-preprocess-image](#ocr-d-processor-interface-ocrd-preprocess-image)
+     * [OCR-D processor interface ocrd-skimage-normalize](#ocr-d-processor-interface-ocrd-skimage-normalize)
+     * [OCR-D processor interface ocrd-skimage-denoise-raw](#ocr-d-processor-interface-ocrd-skimage-denoise-raw)
+     * [OCR-D processor interface ocrd-skimage-binarize](#ocr-d-processor-interface-ocrd-skimage-binarize)
+     * [OCR-D processor interface ocrd-skimage-denoise](#ocr-d-processor-interface-ocrd-skimage-denoise)
+  * [Testing](#testing)
+
+
+## Introduction
+
+This offers [OCR-D](https://ocr-d.de) compliant [workspace processors](https://ocr-d.de/en/spec/cli) for
+any image processing tools which have some (usable) CLI
+and do not modify/invalidate image coordinates.
+
+It thus _wraps_ them for OCR-D without the need
+to write and manage code for each of them individually
+(exposing/passing/documenting their parameters and usage,
+managing releases etc). It shifts all the burden to
+**workflow configuration** (i.e. defining a suitable
+parameter set on how to call what program on what data,
+and installing all the required tools).
+
+It is itself written in Python, and relies heavily on the
+[OCR-D core API](https://github.com/OCR-D/core). This is
+responsible for handling METS/PAGE, and providing the OCR-D
+CLI.
+
+In addition, this aims to wrap existing Python packages
+for preprocessing as OCR-D processors (one at a time).
+
+## Installation
+
+Create and activate a [virtual environment](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments) as usual.
+
+To install Python dependencies:
+
+    make deps
+
+Which is the equivalent of:
+
+    pip install -r requirements.txt
+
+To install this module, then do:
+
+    make install
+
+Which is the equivalent of:
+
+    pip install .
+
+## Usage
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-preprocess-image`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-preprocess-image [OPTIONS]
+
+  Convert or enhance images
+
+  > Performs coords-preserving image operations via runtime shell calls
+  > anywhere.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing.
+
+  > If ``input_feature_selector`` and/or ``input_feature_filter`` is
+  > non-empty, then select/filter among the @imageFilename image and the
+  > available AlternativeImages the last one which contains all of the
+  > selected, but none of the filtered features (i.e. @comments
+  > classes), or raise an error.
+
+  > Then write that image into a temporary PNG file, create a new METS
+  > file ID for the result image (based on the segment ID and the
+  > operation to be run), along with a local path for it, and pass
+  > ``command`` to the shell after replacing: - the string ``@INFILE``
+  > with that input image path, and - the string ``@OUTFILE`` with that
+  > output image path.
+
+  > If the shell returns with a failure, skip that segment with an
+  > approriate error message. Otherwise, add the new image to the
+  > workspace along with the output fileGrp, and using a file ID with
+  > suffix ``.IMG-``, and further identification of the input element.
+
+  > Reference it as AlternativeImage in the element, adding
+  > ``output_feature_added`` to its @comments.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "input_feature_selector" [string - ""]
+    comma-separated list of required image features (e.g.
+    binarized,despeckled)
+   "input_feature_filter" [string - ""]
+    comma-separated list of forbidden image features (e.g.
+    binarized,despeckled)
+   "output_feature_added" [string - REQUIRED]
+    image feature(s) to be added after this operation (if multiple,
+    separate by comma)
+   "input_mimetype" [string - "image/png"]
+    File format to save input images to (tool's expected input)
+    Possible values: ["image/bmp", "application/postscript", "image/gif",
+    "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
+    "image/tiff"]
+   "output_mimetype" [string - "image/png"]
+    File format to load output images from (tool's expected output)
+    Possible values: ["image/bmp", "application/postscript", "image/gif",
+    "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
+    "image/tiff"]
+   "command" [string - REQUIRED]
+    shell command to operate on image files, with @INFILE as place-holder
+    for the input file path, and @OUTFILE as place-holder for the output
+    file path
+```
+
+#### presets
+
+The following example recipes are included in the distribution:
+- enhancement/conversion/denoising using
+  - [x] ImageMagick: [param_im6convert-denoise-raw](ocrd_wrap/param_im6convert-denoise-raw.json)
+  - [ ] GIMP [script-fu](https://gitlab.gnome.org/GNOME/gimp/-/tree/master/plug-ins/script-fu/scripts)
+  - [ ] ...
+- binarization using 
+  - [x] Olena/Scribo: [param_scribo-cli-binarize-sauvola-ms-split](ocrd_wrap/param_scribo-cli-binarize-sauvola-ms-split.json)
+  - [ ] https://github.com/ajgallego/document-image-binarization ...
+  - [ ] https://github.com/qurator-spk/sbb_binarization ...
+  - [ ] https://github.com/masyagin1998/robin ...
+  - [ ] ...
+- text/non-text segmentation using
+  - [ ] Olena/Scribo ...
+  - [ ] ...
+- ...
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-normalize`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-normalize [OPTIONS]
+
+  Equalize contrast/exposure of images with Scikit-image; stretches the color value/tone to the full dynamic range
+
+  > Performs contrast-enhancing equalization of segment or page images
+  > with scikit-image on the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing), in raw (non-binarized) form.
+
+  > Next, normalize the image according to ``method`` in skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-NRM`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "black-point" [number - 1.0]
+    black point point in percent of luminance/value/tone histogram; up to
+    ``black-point`` darkest pixels will be clipped to black when
+    stretching
+   "white-point" [number - 7.0]
+    white point in percent of luminance/value/tone histogram; up to
+    ``white-point`` brightest pixels will be clipped to white when
+    stretching
+   "method" [string - "stretch"]
+    contrast-enhancing transformation to use after clipping; ``stretch``
+    uses ``skimage.exposure.rescale_intensity`` (globally linearly
+    stretching to full dynamic range) and ``adapthist`` uses
+    ``skimage.exposure.equalize_adapthist`` (applying over tiles with
+    context from 1/8th of the image's width)
+    Possible values: ["stretch", "adapthist"]
+```
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise-raw`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-denoise-raw [OPTIONS]
+
+  Denoise raw images with Scikit-image
+
+  > Performs raw denoising of segment or page images with scikit-image
+  > on the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing), in raw (non-binarized) form.
+
+  > Next, denoise the image with a Wavelet transform scheme according to
+  > ``method`` in skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "method" [string - "VisuShrink"]
+    Wavelet filtering scheme to use
+    Possible values: ["BayesShrink", "VisuShrink"]
+```
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-binarize`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-binarize [OPTIONS]
+
+  Binarize images with Scikit-image
+
+  > Performs binarization of segment or page images with scikit-image on
+  > the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing).
+
+  > Next, binarize the image according to ``method`` with skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-BIN`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "method" [string - "sauvola"]
+    Thresholding algorithm to use
+    Possible values: ["sauvola", "niblack", "otsu", "gauss", "yen", "li"]
+   "window_size" [number - 0]
+    For Sauvola/Niblack/Gauss, the (odd) window size in pixels; when zero
+    (default), set to DPI
+   "k" [number - 0.34]
+    For Sauvola/Niblack, formula parameter influencing the threshold
+    bias; larger is lighter foreground
+```
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-denoise [OPTIONS]
+
+  Denoise binarized images with Scikit-image
+
+  > Performs binary denoising of segment or page images with scikit-
+  > image on the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing), in binarized form.
+
+  > Next, denoise the image by removing too small connected components
+  > with skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "maxsize" [number - 3]
+    maximum component size of (bg holes or fg specks) noise in pt
+```
+
+## Testing
+
+none yet
+
```

### Comparing `ocrd_wrap-0.1.7/ocrd_wrap/skimage_denoise_raw.py` & `ocrd_wrap-0.1.8/ocrd_wrap/skimage_denoise_raw.py`

 * *Files identical despite different names*

### Comparing `ocrd_wrap-0.1.7/ocrd_wrap/skimage_denoise.py` & `ocrd_wrap-0.1.8/ocrd_wrap/skimage_denoise.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,25 +149,29 @@
         features = coords['features'] # features already applied to image
         features += ',despeckled'
         maxsize = self.parameter['maxsize']
         maxsize *= dpi/72 # in px instead of pt
         maxsize **= 2 # area
         protect = self.parameter['protect']
         protect *= dpi/72 # in px instead of pt
-        array = ~np.array(image).astype(np.bool)
+        array = np.array(image)
+        dtype = array.dtype
+        scale = array.max()
+        array = ~array.astype(bool)
         # suppress bg specks in fg (holes in binary-inverted)
         array1 = remove_small_holes(array, area_threshold=maxsize)
         # suppress fg specks in bg (blobs in binary-inverted)
         array2 = ~remove_small_holes(~array1, area_threshold=maxsize)
         if protect:
             # reconstruct fragments of larger objects
             recons = binary_dilation(array2, disk(protect))
             recons = reconstruction(recons & array1, array1)
-            array2 |= recons.astype(np.bool)
-        image = Image.fromarray(~array2)
+            array2 |= recons.astype(bool)
+        array = ~array2
+        image = Image.fromarray(array.astype(dtype) * scale)
         # annotate results
         file_path = self.workspace.save_image_file(
             image,
             file_id,
             file_grp=self.output_file_grp,
             page_id=page_id)
         segment.add_AlternativeImage(AlternativeImageType(
```

### Comparing `ocrd_wrap-0.1.7/ocrd_wrap/cli.py` & `ocrd_wrap-0.1.8/ocrd_wrap/cli.py`

 * *Files identical despite different names*

### Comparing `ocrd_wrap-0.1.7/ocrd_wrap/shell.py` & `ocrd_wrap-0.1.8/ocrd_wrap/shell.py`

 * *Files identical despite different names*

### Comparing `ocrd_wrap-0.1.7/ocrd_wrap/skimage_normalize.py` & `ocrd_wrap-0.1.8/ocrd_wrap/skimage_normalize.py`

 * *Files identical despite different names*

### Comparing `ocrd_wrap-0.1.7/ocrd_wrap/skimage_binarize.py` & `ocrd_wrap-0.1.8/ocrd_wrap/skimage_binarize.py`

 * *Files identical despite different names*

### Comparing `ocrd_wrap-0.1.7/README.md` & `ocrd_wrap-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ocrd_wrap-0.1.7/setup.py` & `ocrd_wrap-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `ocrd_wrap-0.1.7/PKG-INFO` & `ocrd_wrap-0.1.8/ocrd_wrap.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,445 +1,445 @@
 Metadata-Version: 2.1
-Name: ocrd_wrap
-Version: 0.1.7
+Name: ocrd-wrap
+Version: 0.1.8
 Summary: OCR-D wrapper for arbitrary coords-preserving image operations
 Home-page: https://github.com/bertsky/ocrd_wrap
 Author: Robert Sachunsky
 Author-email: sachunsky@informatik.uni-leipzig.de
 License: MIT
-Description: [![PyPI version](https://badge.fury.io/py/ocrd-wrap.svg)](https://badge.fury.io/py/ocrd-wrap)
-        
-        # ocrd_wrap
-        
-            OCR-D wrapper for arbitrary coords-preserving image operations
-        
-          * [Introduction](#introduction)
-          * [Installation](#installation)
-          * [Usage](#usage)
-             * [OCR-D processor interface ocrd-preprocess-image](#ocr-d-processor-interface-ocrd-preprocess-image)
-             * [OCR-D processor interface ocrd-skimage-normalize](#ocr-d-processor-interface-ocrd-skimage-normalize)
-             * [OCR-D processor interface ocrd-skimage-denoise-raw](#ocr-d-processor-interface-ocrd-skimage-denoise-raw)
-             * [OCR-D processor interface ocrd-skimage-binarize](#ocr-d-processor-interface-ocrd-skimage-binarize)
-             * [OCR-D processor interface ocrd-skimage-denoise](#ocr-d-processor-interface-ocrd-skimage-denoise)
-          * [Testing](#testing)
-        
-        
-        ## Introduction
-        
-        This offers [OCR-D](https://ocr-d.de) compliant [workspace processors](https://ocr-d.de/en/spec/cli) for
-        any image processing tools which have some (usable) CLI
-        and do not modify/invalidate image coordinates.
-        
-        It thus _wraps_ them for OCR-D without the need
-        to write and manage code for each of them individually
-        (exposing/passing/documenting their parameters and usage,
-        managing releases etc). It shifts all the burden to
-        **workflow configuration** (i.e. defining a suitable
-        parameter set on how to call what program on what data,
-        and installing all the required tools).
-        
-        It is itself written in Python, and relies heavily on the
-        [OCR-D core API](https://github.com/OCR-D/core). This is
-        responsible for handling METS/PAGE, and providing the OCR-D
-        CLI.
-        
-        In addition, this aims to wrap existing Python packages
-        for preprocessing as OCR-D processors (one at a time).
-        
-        ## Installation
-        
-        Create and activate a [virtual environment](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments) as usual.
-        
-        To install Python dependencies:
-        
-            make deps
-        
-        Which is the equivalent of:
-        
-            pip install -r requirements.txt
-        
-        To install this module, then do:
-        
-            make install
-        
-        Which is the equivalent of:
-        
-            pip install .
-        
-        ## Usage
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-preprocess-image`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-preprocess-image [OPTIONS]
-        
-          Convert or enhance images
-        
-          > Performs coords-preserving image operations via runtime shell calls
-          > anywhere.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing.
-        
-          > If ``input_feature_selector`` and/or ``input_feature_filter`` is
-          > non-empty, then select/filter among the @imageFilename image and the
-          > available AlternativeImages the last one which contains all of the
-          > selected, but none of the filtered features (i.e. @comments
-          > classes), or raise an error.
-        
-          > Then write that image into a temporary PNG file, create a new METS
-          > file ID for the result image (based on the segment ID and the
-          > operation to be run), along with a local path for it, and pass
-          > ``command`` to the shell after replacing: - the string ``@INFILE``
-          > with that input image path, and - the string ``@OUTFILE`` with that
-          > output image path.
-        
-          > If the shell returns with a failure, skip that segment with an
-          > approriate error message. Otherwise, add the new image to the
-          > workspace along with the output fileGrp, and using a file ID with
-          > suffix ``.IMG-``, and further identification of the input element.
-        
-          > Reference it as AlternativeImage in the element, adding
-          > ``output_feature_added`` to its @comments.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "input_feature_selector" [string - ""]
-            comma-separated list of required image features (e.g.
-            binarized,despeckled)
-           "input_feature_filter" [string - ""]
-            comma-separated list of forbidden image features (e.g.
-            binarized,despeckled)
-           "output_feature_added" [string - REQUIRED]
-            image feature(s) to be added after this operation (if multiple,
-            separate by comma)
-           "input_mimetype" [string - "image/png"]
-            File format to save input images to (tool's expected input)
-            Possible values: ["image/bmp", "application/postscript", "image/gif",
-            "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
-            "image/tiff"]
-           "output_mimetype" [string - "image/png"]
-            File format to load output images from (tool's expected output)
-            Possible values: ["image/bmp", "application/postscript", "image/gif",
-            "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
-            "image/tiff"]
-           "command" [string - REQUIRED]
-            shell command to operate on image files, with @INFILE as place-holder
-            for the input file path, and @OUTFILE as place-holder for the output
-            file path
-        ```
-        
-        #### presets
-        
-        The following example recipes are included in the distribution:
-        - enhancement/conversion/denoising using
-          - [x] ImageMagick: [param_im6convert-denoise-raw](ocrd_wrap/param_im6convert-denoise-raw.json)
-          - [ ] GIMP [script-fu](https://gitlab.gnome.org/GNOME/gimp/-/tree/master/plug-ins/script-fu/scripts)
-          - [ ] ...
-        - binarization using 
-          - [x] Olena/Scribo: [param_scribo-cli-binarize-sauvola-ms-split](ocrd_wrap/param_scribo-cli-binarize-sauvola-ms-split.json)
-          - [ ] https://github.com/ajgallego/document-image-binarization ...
-          - [ ] https://github.com/qurator-spk/sbb_binarization ...
-          - [ ] https://github.com/masyagin1998/robin ...
-          - [ ] ...
-        - text/non-text segmentation using
-          - [ ] Olena/Scribo ...
-          - [ ] ...
-        - ...
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-normalize`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-normalize [OPTIONS]
-        
-          Equalize contrast/exposure of images with Scikit-image; stretches the color value/tone to the full dynamic range
-        
-          > Performs contrast-enhancing equalization of segment or page images
-          > with scikit-image on the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing), in raw (non-binarized) form.
-        
-          > Next, normalize the image according to ``method`` in skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-NRM`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "black-point" [number - 1.0]
-            black point point in percent of luminance/value/tone histogram; up to
-            ``black-point`` darkest pixels will be clipped to black when
-            stretching
-           "white-point" [number - 7.0]
-            white point in percent of luminance/value/tone histogram; up to
-            ``white-point`` brightest pixels will be clipped to white when
-            stretching
-           "method" [string - "stretch"]
-            contrast-enhancing transformation to use after clipping; ``stretch``
-            uses ``skimage.exposure.rescale_intensity`` (globally linearly
-            stretching to full dynamic range) and ``adapthist`` uses
-            ``skimage.exposure.equalize_adapthist`` (applying over tiles with
-            context from 1/8th of the image's width)
-            Possible values: ["stretch", "adapthist"]
-        ```
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise-raw`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-denoise-raw [OPTIONS]
-        
-          Denoise raw images with Scikit-image
-        
-          > Performs raw denoising of segment or page images with scikit-image
-          > on the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing), in raw (non-binarized) form.
-        
-          > Next, denoise the image with a Wavelet transform scheme according to
-          > ``method`` in skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "method" [string - "VisuShrink"]
-            Wavelet filtering scheme to use
-            Possible values: ["BayesShrink", "VisuShrink"]
-        ```
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-binarize`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-binarize [OPTIONS]
-        
-          Binarize images with Scikit-image
-        
-          > Performs binarization of segment or page images with scikit-image on
-          > the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing).
-        
-          > Next, binarize the image according to ``method`` with skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-BIN`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "method" [string - "sauvola"]
-            Thresholding algorithm to use
-            Possible values: ["sauvola", "niblack", "otsu", "gauss", "yen", "li"]
-           "window_size" [number - 0]
-            For Sauvola/Niblack/Gauss, the (odd) window size in pixels; when zero
-            (default), set to DPI
-           "k" [number - 0.34]
-            For Sauvola/Niblack, formula parameter influencing the threshold
-            bias; larger is lighter foreground
-        ```
-        
-        ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise`
-        
-        To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
-        
-        ```
-        Usage: ocrd-skimage-denoise [OPTIONS]
-        
-          Denoise binarized images with Scikit-image
-        
-          > Performs binary denoising of segment or page images with scikit-
-          > image on the workspace.
-        
-          > Open and deserialize PAGE input files and their respective images,
-          > then iterate over the element hierarchy down to the requested
-          > ``level-of-operation`` in the element hierarchy.
-        
-          > For each segment element, retrieve a segment image according to the
-          > layout annotation (from an existing AlternativeImage, or by cropping
-          > via coordinates into the higher-level image, and - when applicable -
-          > deskewing), in binarized form.
-        
-          > Next, denoise the image by removing too small connected components
-          > with skimage.
-        
-          > Then write the new image to the workspace along with the output
-          > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
-          > identification of the input element.
-        
-          > Produce a new PAGE output file by serialising the resulting
-          > hierarchy.
-        
-        Options:
-          -I, --input-file-grp USE        File group(s) used as input
-          -O, --output-file-grp USE       File group(s) used as output
-          -g, --page-id ID                Physical page ID(s) to process
-          --overwrite                     Remove existing output pages/images
-                                          (with --page-id, remove only those)
-          -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
-                                          or JSON file path
-          -P, --param-override KEY VAL    Override a single JSON object key-value pair,
-                                          taking precedence over --parameter
-          -m, --mets URL-PATH             URL or file path of METS to process
-          -w, --working-dir PATH          Working directory of local workspace
-          -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
-                                          Log level
-          -J, --dump-json                 Dump tool description as JSON and exit
-          -h, --help                      This help message
-          -V, --version                   Show version
-        
-        Parameters:
-           "level-of-operation" [string - "page"]
-            PAGE XML hierarchy level to operate on
-            Possible values: ["page", "region", "line", "word", "glyph"]
-           "dpi" [number - 0]
-            pixel density in dots per inch (overrides any meta-data in the
-            images); disabled when zero
-           "maxsize" [number - 3]
-            maximum component size of (bg holes or fg specks) noise in pt
-        ```
-        
-        ## Testing
-        
-        none yet
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/ocrd-wrap.svg)](https://badge.fury.io/py/ocrd-wrap)
+
+# ocrd_wrap
+
+    OCR-D wrapper for arbitrary coords-preserving image operations
+
+  * [Introduction](#introduction)
+  * [Installation](#installation)
+  * [Usage](#usage)
+     * [OCR-D processor interface ocrd-preprocess-image](#ocr-d-processor-interface-ocrd-preprocess-image)
+     * [OCR-D processor interface ocrd-skimage-normalize](#ocr-d-processor-interface-ocrd-skimage-normalize)
+     * [OCR-D processor interface ocrd-skimage-denoise-raw](#ocr-d-processor-interface-ocrd-skimage-denoise-raw)
+     * [OCR-D processor interface ocrd-skimage-binarize](#ocr-d-processor-interface-ocrd-skimage-binarize)
+     * [OCR-D processor interface ocrd-skimage-denoise](#ocr-d-processor-interface-ocrd-skimage-denoise)
+  * [Testing](#testing)
+
+
+## Introduction
+
+This offers [OCR-D](https://ocr-d.de) compliant [workspace processors](https://ocr-d.de/en/spec/cli) for
+any image processing tools which have some (usable) CLI
+and do not modify/invalidate image coordinates.
+
+It thus _wraps_ them for OCR-D without the need
+to write and manage code for each of them individually
+(exposing/passing/documenting their parameters and usage,
+managing releases etc). It shifts all the burden to
+**workflow configuration** (i.e. defining a suitable
+parameter set on how to call what program on what data,
+and installing all the required tools).
+
+It is itself written in Python, and relies heavily on the
+[OCR-D core API](https://github.com/OCR-D/core). This is
+responsible for handling METS/PAGE, and providing the OCR-D
+CLI.
+
+In addition, this aims to wrap existing Python packages
+for preprocessing as OCR-D processors (one at a time).
+
+## Installation
+
+Create and activate a [virtual environment](https://packaging.python.org/tutorials/installing-packages/#creating-virtual-environments) as usual.
+
+To install Python dependencies:
+
+    make deps
+
+Which is the equivalent of:
+
+    pip install -r requirements.txt
+
+To install this module, then do:
+
+    make install
+
+Which is the equivalent of:
+
+    pip install .
+
+## Usage
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-preprocess-image`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-preprocess-image [OPTIONS]
+
+  Convert or enhance images
+
+  > Performs coords-preserving image operations via runtime shell calls
+  > anywhere.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing.
+
+  > If ``input_feature_selector`` and/or ``input_feature_filter`` is
+  > non-empty, then select/filter among the @imageFilename image and the
+  > available AlternativeImages the last one which contains all of the
+  > selected, but none of the filtered features (i.e. @comments
+  > classes), or raise an error.
+
+  > Then write that image into a temporary PNG file, create a new METS
+  > file ID for the result image (based on the segment ID and the
+  > operation to be run), along with a local path for it, and pass
+  > ``command`` to the shell after replacing: - the string ``@INFILE``
+  > with that input image path, and - the string ``@OUTFILE`` with that
+  > output image path.
+
+  > If the shell returns with a failure, skip that segment with an
+  > approriate error message. Otherwise, add the new image to the
+  > workspace along with the output fileGrp, and using a file ID with
+  > suffix ``.IMG-``, and further identification of the input element.
+
+  > Reference it as AlternativeImage in the element, adding
+  > ``output_feature_added`` to its @comments.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "input_feature_selector" [string - ""]
+    comma-separated list of required image features (e.g.
+    binarized,despeckled)
+   "input_feature_filter" [string - ""]
+    comma-separated list of forbidden image features (e.g.
+    binarized,despeckled)
+   "output_feature_added" [string - REQUIRED]
+    image feature(s) to be added after this operation (if multiple,
+    separate by comma)
+   "input_mimetype" [string - "image/png"]
+    File format to save input images to (tool's expected input)
+    Possible values: ["image/bmp", "application/postscript", "image/gif",
+    "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
+    "image/tiff"]
+   "output_mimetype" [string - "image/png"]
+    File format to load output images from (tool's expected output)
+    Possible values: ["image/bmp", "application/postscript", "image/gif",
+    "image/jpeg", "image/jp2", "image/png", "image/x-portable-pixmap",
+    "image/tiff"]
+   "command" [string - REQUIRED]
+    shell command to operate on image files, with @INFILE as place-holder
+    for the input file path, and @OUTFILE as place-holder for the output
+    file path
+```
+
+#### presets
+
+The following example recipes are included in the distribution:
+- enhancement/conversion/denoising using
+  - [x] ImageMagick: [param_im6convert-denoise-raw](ocrd_wrap/param_im6convert-denoise-raw.json)
+  - [ ] GIMP [script-fu](https://gitlab.gnome.org/GNOME/gimp/-/tree/master/plug-ins/script-fu/scripts)
+  - [ ] ...
+- binarization using 
+  - [x] Olena/Scribo: [param_scribo-cli-binarize-sauvola-ms-split](ocrd_wrap/param_scribo-cli-binarize-sauvola-ms-split.json)
+  - [ ] https://github.com/ajgallego/document-image-binarization ...
+  - [ ] https://github.com/qurator-spk/sbb_binarization ...
+  - [ ] https://github.com/masyagin1998/robin ...
+  - [ ] ...
+- text/non-text segmentation using
+  - [ ] Olena/Scribo ...
+  - [ ] ...
+- ...
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-normalize`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-normalize [OPTIONS]
+
+  Equalize contrast/exposure of images with Scikit-image; stretches the color value/tone to the full dynamic range
+
+  > Performs contrast-enhancing equalization of segment or page images
+  > with scikit-image on the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing), in raw (non-binarized) form.
+
+  > Next, normalize the image according to ``method`` in skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-NRM`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "black-point" [number - 1.0]
+    black point point in percent of luminance/value/tone histogram; up to
+    ``black-point`` darkest pixels will be clipped to black when
+    stretching
+   "white-point" [number - 7.0]
+    white point in percent of luminance/value/tone histogram; up to
+    ``white-point`` brightest pixels will be clipped to white when
+    stretching
+   "method" [string - "stretch"]
+    contrast-enhancing transformation to use after clipping; ``stretch``
+    uses ``skimage.exposure.rescale_intensity`` (globally linearly
+    stretching to full dynamic range) and ``adapthist`` uses
+    ``skimage.exposure.equalize_adapthist`` (applying over tiles with
+    context from 1/8th of the image's width)
+    Possible values: ["stretch", "adapthist"]
+```
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise-raw`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-denoise-raw [OPTIONS]
+
+  Denoise raw images with Scikit-image
+
+  > Performs raw denoising of segment or page images with scikit-image
+  > on the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing), in raw (non-binarized) form.
+
+  > Next, denoise the image with a Wavelet transform scheme according to
+  > ``method`` in skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "method" [string - "VisuShrink"]
+    Wavelet filtering scheme to use
+    Possible values: ["BayesShrink", "VisuShrink"]
+```
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-binarize`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-binarize [OPTIONS]
+
+  Binarize images with Scikit-image
+
+  > Performs binarization of segment or page images with scikit-image on
+  > the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing).
+
+  > Next, binarize the image according to ``method`` with skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-BIN`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "method" [string - "sauvola"]
+    Thresholding algorithm to use
+    Possible values: ["sauvola", "niblack", "otsu", "gauss", "yen", "li"]
+   "window_size" [number - 0]
+    For Sauvola/Niblack/Gauss, the (odd) window size in pixels; when zero
+    (default), set to DPI
+   "k" [number - 0.34]
+    For Sauvola/Niblack, formula parameter influencing the threshold
+    bias; larger is lighter foreground
+```
+
+### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-skimage-denoise`
+
+To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
+
+```
+Usage: ocrd-skimage-denoise [OPTIONS]
+
+  Denoise binarized images with Scikit-image
+
+  > Performs binary denoising of segment or page images with scikit-
+  > image on the workspace.
+
+  > Open and deserialize PAGE input files and their respective images,
+  > then iterate over the element hierarchy down to the requested
+  > ``level-of-operation`` in the element hierarchy.
+
+  > For each segment element, retrieve a segment image according to the
+  > layout annotation (from an existing AlternativeImage, or by cropping
+  > via coordinates into the higher-level image, and - when applicable -
+  > deskewing), in binarized form.
+
+  > Next, denoise the image by removing too small connected components
+  > with skimage.
+
+  > Then write the new image to the workspace along with the output
+  > fileGrp, and using a file ID with suffix ``.IMG-DEN`` with further
+  > identification of the input element.
+
+  > Produce a new PAGE output file by serialising the resulting
+  > hierarchy.
+
+Options:
+  -I, --input-file-grp USE        File group(s) used as input
+  -O, --output-file-grp USE       File group(s) used as output
+  -g, --page-id ID                Physical page ID(s) to process
+  --overwrite                     Remove existing output pages/images
+                                  (with --page-id, remove only those)
+  -p, --parameter JSON-PATH       Parameters, either verbatim JSON string
+                                  or JSON file path
+  -P, --param-override KEY VAL    Override a single JSON object key-value pair,
+                                  taking precedence over --parameter
+  -m, --mets URL-PATH             URL or file path of METS to process
+  -w, --working-dir PATH          Working directory of local workspace
+  -l, --log-level [OFF|ERROR|WARN|INFO|DEBUG|TRACE]
+                                  Log level
+  -J, --dump-json                 Dump tool description as JSON and exit
+  -h, --help                      This help message
+  -V, --version                   Show version
+
+Parameters:
+   "level-of-operation" [string - "page"]
+    PAGE XML hierarchy level to operate on
+    Possible values: ["page", "region", "line", "word", "glyph"]
+   "dpi" [number - 0]
+    pixel density in dots per inch (overrides any meta-data in the
+    images); disabled when zero
+   "maxsize" [number - 3]
+    maximum component size of (bg holes or fg specks) noise in pt
+```
+
+## Testing
+
+none yet
+
```

