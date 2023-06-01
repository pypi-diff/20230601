# Comparing `tmp/python_docx_ng-0.9.3.tar.gz` & `tmp/python_docx_ng-0.9.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_docx_ng-0.9.3.tar", max compression
+gzip compressed data, was "python_docx_ng-0.9.4.dev0.tar", max compression
```

## Comparing `python_docx_ng-0.9.3.tar` & `python_docx_ng-0.9.4.dev0.tar`

### file list

```diff
@@ -1,111 +1,127 @@
--rw-r--r--   0        0        0     1150 2022-12-02 13:25:58.613622 python_docx_ng-0.9.3/LICENSE
--rw-r--r--   0        0        0     3059 2023-01-06 10:26:33.573148 python_docx_ng-0.9.3/README.md
--rw-r--r--   0        0        0     1535 2023-01-27 07:18:56.696211 python_docx_ng-0.9.3/docx/__init__.py
--rw-r--r--   0        0        0     1221 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/api.py
--rw-r--r--   0        0        0     2511 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/blkcntnr.py
--rw-r--r--   0        0        0     1043 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/compat.py
--rw-r--r--   0        0        0        0 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/dml/__init__.py
--rw-r--r--   0        0        0     3978 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/dml/color.py
--rw-r--r--   0        0        0     7497 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/document.py
--rw-r--r--   0        0        0      343 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/__init__.py
--rw-r--r--   0        0        0    11080 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/base.py
--rw-r--r--   0        0        0     3533 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/dml.py
--rw-r--r--   0        0        0     2666 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/section.py
--rw-r--r--   0        0        0      475 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/shape.py
--rw-r--r--   0        0        0    12189 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/style.py
--rw-r--r--   0        0        0     3929 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/table.py
--rw-r--r--   0        0        0    10689 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/enum/text.py
--rw-r--r--   0        0        0      503 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/exceptions.py
--rw-r--r--   0        0        0      819 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/__init__.py
--rw-r--r--   0        0        0     1512 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/bmp.py
--rw-r--r--   0        0        0     3497 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/constants.py
--rw-r--r--   0        0        0      432 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/exceptions.py
--rw-r--r--   0        0        0     1260 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/gif.py
--rw-r--r--   0        0        0     3286 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/helpers.py
--rw-r--r--   0        0        0     8029 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/image.py
--rw-r--r--   0        0        0    16099 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/jpeg.py
--rw-r--r--   0        0        0     8789 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/png.py
--rw-r--r--   0        0        0     1296 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/svg.py
--rw-r--r--   0        0        0    11140 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/image/tiff.py
--rw-r--r--   0        0        0        0 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/__init__.py
--rw-r--r--   0        0        0     1327 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/compat.py
--rw-r--r--   0        0        0    20400 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/constants.py
--rw-r--r--   0        0        0     3246 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/coreprops.py
--rw-r--r--   0        0        0      302 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/exceptions.py
--rw-r--r--   0        0        0     8540 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/oxml.py
--rw-r--r--   0        0        0     8510 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/package.py
--rw-r--r--   0        0        0     3880 2022-12-02 13:25:58.617622 python_docx_ng-0.9.3/docx/opc/packuri.py
--rw-r--r--   0        0        0     8157 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/part.py
--rw-r--r--   0        0        0        0 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/parts/__init__.py
--rw-r--r--   0        0        0     1664 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/parts/coreprops.py
--rw-r--r--   0        0        0     4452 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/phys_pkg.py
--rw-r--r--   0        0        0    10107 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/pkgreader.py
--rw-r--r--   0        0        0     4601 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/pkgwriter.py
--rw-r--r--   0        0        0     5415 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/rel.py
--rw-r--r--   0        0        0     1453 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/shared.py
--rw-r--r--   0        0        0      716 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/opc/spec.py
--rw-r--r--   0        0        0    12022 2023-01-06 08:05:12.794418 python_docx_ng-0.9.3/docx/oxml/__init__.py
--rw-r--r--   0        0        0    10278 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/coreprops.py
--rw-r--r--   0        0        0     2769 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/document.py
--rw-r--r--   0        0        0      290 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/exceptions.py
--rw-r--r--   0        0        0     3848 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/ns.py
--rw-r--r--   0        0        0     4976 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/numbering.py
--rw-r--r--   0        0        0    11114 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/section.py
--rw-r--r--   0        0        0     3491 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/settings.py
--rw-r--r--   0        0        0     9131 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/shape.py
--rw-r--r--   0        0        0     1623 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/shared.py
--rw-r--r--   0        0        0    14160 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/simpletypes.py
--rw-r--r--   0        0        0    11218 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/styles.py
--rw-r--r--   0        0        0    32007 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/table.py
--rw-r--r--   0        0        0        0 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/text/__init__.py
--rw-r--r--   0        0        0    11424 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/text/font.py
--rw-r--r--   0        0        0     2839 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/text/form.py
--rw-r--r--   0        0        0     1908 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/text/paragraph.py
--rw-r--r--   0        0        0    11093 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/text/parfmt.py
--rw-r--r--   0        0        0     4888 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/text/run.py
--rw-r--r--   0        0        0    24857 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/oxml/xmlchemy.py
--rw-r--r--   0        0        0     3868 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/package.py
--rw-r--r--   0        0        0        0 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/__init__.py
--rw-r--r--   0        0        0     1285 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/altchunk.py
--rw-r--r--   0        0        0     5325 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/document.py
--rw-r--r--   0        0        0     1717 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/hdrftr.py
--rw-r--r--   0        0        0     2668 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/image.py
--rw-r--r--   0        0        0     1230 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/numbering.py
--rw-r--r--   0        0        0     1465 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/settings.py
--rw-r--r--   0        0        0     3201 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/parts/story.py
--rw-r--r--   0        0        0     1428 2022-12-05 08:57:17.138503 python_docx_ng-0.9.3/docx/parts/styles.py
--rw-r--r--   0        0        0    16201 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/section.py
--rw-r--r--   0        0        0      780 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/settings.py
--rw-r--r--   0        0        0     2811 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/shape.py
--rw-r--r--   0        0        0     6791 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/shared.py
--rw-r--r--   0        0        0     1500 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/styles/__init__.py
--rw-r--r--   0        0        0     7549 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/styles/latent.py
--rw-r--r--   0        0        0     7987 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/styles/style.py
--rw-r--r--   0        0        0     5766 2022-12-05 10:23:36.444259 python_docx_ng-0.9.3/docx/styles/styles.py
--rw-r--r--   0        0        0    20241 2022-12-02 13:25:58.621622 python_docx_ng-0.9.3/docx/table.py
--rw-r--r--   0        0        0     1445 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/[Content_Types].xml
--rw-r--r--   0        0        0      590 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/_rels/.rels
--rw-r--r--   0        0        0      709 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/docProps/app.xml
--rw-r--r--   0        0        0      727 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/docProps/core.xml
--rw-r--r--   0        0        0      950 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/_rels/document.xml.rels
--rw-r--r--   0        0        0     2870 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/document.xml
--rw-r--r--   0        0        0     2723 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/fontTable.xml
--rw-r--r--   0        0        0    15658 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/numbering.xml
--rw-r--r--   0        0        0     3668 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/settings.xml
--rw-r--r--   0        0        0    44249 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/styles.xml
--rw-r--r--   0        0        0     8393 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/theme/theme1.xml
--rw-r--r--   0        0        0      894 1979-12-31 23:00:00.000000 python_docx_ng-0.9.3/docx/templates/default-docx-template/word/webSettings.xml
--rw-r--r--   0        0        0     1395 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/templates/default-footer.xml
--rw-r--r--   0        0        0     1395 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/templates/default-header.xml
--rw-r--r--   0        0        0     1640 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/templates/default-settings.xml
--rw-r--r--   0        0        0    32959 2022-12-05 09:58:56.469207 python_docx_ng-0.9.3/docx/templates/default-styles.xml
--rw-r--r--   0        0        0    15636 2022-12-05 10:46:04.068223 python_docx_ng-0.9.3/docx/templates/default.docx
--rw-r--r--   0        0        0        0 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/text/__init__.py
--rw-r--r--   0        0        0    12544 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/text/font.py
--rw-r--r--   0        0        0     4820 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/text/paragraph.py
--rw-r--r--   0        0        0    11190 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/text/parfmt.py
--rw-r--r--   0        0        0     6988 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/text/run.py
--rw-r--r--   0        0        0     4183 2022-12-02 13:25:58.625622 python_docx_ng-0.9.3/docx/text/tabstops.py
--rw-r--r--   0        0        0      515 2023-01-27 07:17:53.236473 python_docx_ng-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 python_docx_ng-0.9.3/setup.py
--rw-r--r--   0        0        0     3646 1970-01-01 00:00:00.000000 python_docx_ng-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1150 2023-06-01 12:54:13.968597 python_docx_ng-0.9.4.dev0/LICENSE
+-rw-r--r--   0        0        0     4888 2023-06-01 12:54:13.968597 python_docx_ng-0.9.4.dev0/README.md
+-rw-r--r--   0        0        0     1949 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/__init__.py
+-rw-r--r--   0        0        0     1754 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/api.py
+-rw-r--r--   0        0        0     2959 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/blkcntnr.py
+-rw-r--r--   0        0        0     1043 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/compat.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/dml/__init__.py
+-rw-r--r--   0        0        0     3978 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/dml/color.py
+-rw-r--r--   0        0        0     8610 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/document.py
+-rw-r--r--   0        0        0      343 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/__init__.py
+-rw-r--r--   0        0        0    11080 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/base.py
+-rw-r--r--   0        0        0     3533 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/dml.py
+-rw-r--r--   0        0        0     2666 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/section.py
+-rw-r--r--   0        0        0      475 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/shape.py
+-rw-r--r--   0        0        0    12189 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/style.py
+-rw-r--r--   0        0        0     3929 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/table.py
+-rw-r--r--   0        0        0    10689 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/enum/text.py
+-rw-r--r--   0        0        0      503 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/exceptions.py
+-rw-r--r--   0        0        0     1002 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/__init__.py
+-rw-r--r--   0        0        0     1512 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/bmp.py
+-rw-r--r--   0        0        0     3541 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/constants.py
+-rw-r--r--   0        0        0     2010 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/emf.py
+-rw-r--r--   0        0        0      432 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/exceptions.py
+-rw-r--r--   0        0        0     1260 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/gif.py
+-rw-r--r--   0        0        0     3286 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/helpers.py
+-rw-r--r--   0        0        0     8029 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/image.py
+-rw-r--r--   0        0        0    16099 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/jpeg.py
+-rw-r--r--   0        0        0     8789 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/png.py
+-rw-r--r--   0        0        0     1296 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/svg.py
+-rw-r--r--   0        0        0    11140 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/tiff.py
+-rw-r--r--   0        0        0     1516 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/image/wmf.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/opc/__init__.py
+-rw-r--r--   0        0        0     1327 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/opc/compat.py
+-rw-r--r--   0        0        0    20400 2023-06-01 12:54:13.976597 python_docx_ng-0.9.4.dev0/docx/opc/constants.py
+-rw-r--r--   0        0        0     3246 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/coreprops.py
+-rw-r--r--   0        0        0      302 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/exceptions.py
+-rw-r--r--   0        0        0     2429 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/extendedprops.py
+-rw-r--r--   0        0        0     8540 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/oxml.py
+-rw-r--r--   0        0        0    10293 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/package.py
+-rw-r--r--   0        0        0     3880 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/packuri.py
+-rw-r--r--   0        0        0     8157 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/part.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/parts/__init__.py
+-rw-r--r--   0        0        0     1664 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/parts/coreprops.py
+-rw-r--r--   0        0        0     1588 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/parts/extendedprops.py
+-rw-r--r--   0        0        0     4452 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/phys_pkg.py
+-rw-r--r--   0        0        0    10107 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/pkgreader.py
+-rw-r--r--   0        0        0     4601 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/pkgwriter.py
+-rw-r--r--   0        0        0     5415 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/rel.py
+-rw-r--r--   0        0        0     1453 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/shared.py
+-rw-r--r--   0        0        0      716 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/opc/spec.py
+-rw-r--r--   0        0        0    13177 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/__init__.py
+-rw-r--r--   0        0        0     3292 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/comment.py
+-rw-r--r--   0        0        0    10278 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/coreprops.py
+-rw-r--r--   0        0        0     2769 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/document.py
+-rw-r--r--   0        0        0      290 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/exceptions.py
+-rw-r--r--   0        0        0     5934 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/extendedprops.py
+-rw-r--r--   0        0        0     2207 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/footnote.py
+-rw-r--r--   0        0        0     4017 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/ns.py
+-rw-r--r--   0        0        0     5181 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/numbering.py
+-rw-r--r--   0        0        0    11114 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/section.py
+-rw-r--r--   0        0        0     3491 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/settings.py
+-rw-r--r--   0        0        0     9131 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/shape.py
+-rw-r--r--   0        0        0     1623 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/shared.py
+-rw-r--r--   0        0        0    14160 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/simpletypes.py
+-rw-r--r--   0        0        0    11670 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/styles.py
+-rw-r--r--   0        0        0    33584 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/table.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/text/__init__.py
+-rw-r--r--   0        0        0    12707 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/text/font.py
+-rw-r--r--   0        0        0     2839 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/text/form.py
+-rw-r--r--   0        0        0     3832 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/text/paragraph.py
+-rw-r--r--   0        0        0    12405 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/text/parfmt.py
+-rw-r--r--   0        0        0     7894 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/text/run.py
+-rw-r--r--   0        0        0    24857 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/oxml/xmlchemy.py
+-rw-r--r--   0        0        0     3868 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/package.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/__init__.py
+-rw-r--r--   0        0        0     1285 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/altchunk.py
+-rw-r--r--   0        0        0      812 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/comment.py
+-rw-r--r--   0        0        0     5646 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/document.py
+-rw-r--r--   0        0        0      820 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/footnote.py
+-rw-r--r--   0        0        0     1717 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/hdrftr.py
+-rw-r--r--   0        0        0     2668 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/image.py
+-rw-r--r--   0        0        0     1230 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/numbering.py
+-rw-r--r--   0        0        0     1465 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/settings.py
+-rw-r--r--   0        0        0     3282 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/story.py
+-rw-r--r--   0        0        0     1428 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/parts/styles.py
+-rw-r--r--   0        0        0    17290 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/section.py
+-rw-r--r--   0        0        0      780 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/settings.py
+-rw-r--r--   0        0        0     2811 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/shape.py
+-rw-r--r--   0        0        0     6791 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/shared.py
+-rw-r--r--   0        0        0     1500 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/styles/__init__.py
+-rw-r--r--   0        0        0     7549 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/styles/latent.py
+-rw-r--r--   0        0        0     7987 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/styles/style.py
+-rw-r--r--   0        0        0     5766 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/styles/styles.py
+-rw-r--r--   0        0        0    21294 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/table.py
+-rw-r--r--   0        0        0     1427 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/templates/default-comments.xml
+-rw-r--r--   0        0        0     1444 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/[Content_Types].xml
+-rw-r--r--   0        0        0      589 2023-06-01 12:54:13.980597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/_rels/.rels
+-rw-r--r--   0        0        0      300 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/customXml/_rels/item1.xml.rels
+-rw-r--r--   0        0        0      262 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/customXml/item1.xml
+-rw-r--r--   0        0        0      354 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/customXml/itemProps1.xml
+-rw-r--r--   0        0        0      708 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/docProps/app.xml
+-rw-r--r--   0        0        0      726 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/docProps/core.xml
+-rw-r--r--   0        0        0     8324 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/docProps/thumbnail.jpeg
+-rw-r--r--   0        0        0      949 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/_rels/document.xml.rels
+-rw-r--r--   0        0        0     2869 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/document.xml
+-rw-r--r--   0        0        0     2722 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/fontTable.xml
+-rw-r--r--   0        0        0    15657 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/numbering.xml
+-rw-r--r--   0        0        0     3667 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/settings.xml
+-rw-r--r--   0        0        0    44248 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/styles.xml
+-rw-r--r--   0        0        0   438131 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/stylesWithEffects.xml
+-rw-r--r--   0        0        0     8392 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/theme/theme1.xml
+-rw-r--r--   0        0        0      893 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/webSettings.xml
+-rw-r--r--   0        0        0     1395 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-footer.xml
+-rw-r--r--   0        0        0     1905 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-footnotes.xml
+-rw-r--r--   0        0        0     1395 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-header.xml
+-rw-r--r--   0        0        0     1640 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-settings.xml
+-rw-r--r--   0        0        0    32959 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default-styles.xml
+-rw-r--r--   0        0        0    15636 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/templates/default.docx
+-rw-r--r--   0        0        0        0 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/text/__init__.py
+-rw-r--r--   0        0        0      527 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/text/comment.py
+-rw-r--r--   0        0        0    13134 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/text/font.py
+-rw-r--r--   0        0        0     7694 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/text/paragraph.py
+-rw-r--r--   0        0        0    11643 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/text/parfmt.py
+-rw-r--r--   0        0        0    10569 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/text/run.py
+-rw-r--r--   0        0        0     4183 2023-06-01 12:54:13.984597 python_docx_ng-0.9.4.dev0/docx/text/tabstops.py
+-rw-r--r--   0        0        0      519 2023-06-01 12:54:14.008598 python_docx_ng-0.9.4.dev0/pyproject.toml
+-rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 python_docx_ng-0.9.4.dev0/PKG-INFO
```

### Comparing `python_docx_ng-0.9.3/LICENSE` & `python_docx_ng-0.9.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/__init__.py` & `python_docx_ng-0.9.4.dev0/docx/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,61 @@
 # encoding: utf-8
 
 from docx.api import Document  # noqa
 
-__version__ = "0.9.3"
+__version__ = "0.9.4-dev"
 
 
 # register custom Part classes with opc package reader
 
 from docx.opc.constants import CONTENT_TYPE as CT, RELATIONSHIP_TYPE as RT
 from docx.opc.part import PartFactory
 from docx.opc.parts.coreprops import CorePropertiesPart
+from docx.opc.parts.extendedprops import ExtendedPropertiesPart
 
 from docx.parts.document import DocumentPart
 from docx.parts.hdrftr import FooterPart, HeaderPart
 from docx.parts.image import ImagePart
 from docx.parts.altchunk import AltchunkPart
 from docx.parts.numbering import NumberingPart
 from docx.parts.settings import SettingsPart
 from docx.parts.styles import StylesPart
+from docx.parts.comment import CommentPart
+from docx.parts.footnote import FootnotePart
 
 
 def part_class_selector(content_type, reltype):
     if reltype == RT.A_F_CHUNK:
         return AltchunkPart
     if reltype == RT.IMAGE:
         return ImagePart
     return None
 
 
 PartFactory.part_class_selector = part_class_selector
+PartFactory.part_type_for[CT.WML_COMMENTS] = CommentPart
 PartFactory.part_type_for[CT.OPC_CORE_PROPERTIES] = CorePropertiesPart
+PartFactory.part_type_for[CT.OFC_EXTENDED_PROPERTIES] = ExtendedPropertiesPart
 PartFactory.part_type_for[CT.WML_DOCUMENT_MAIN] = DocumentPart
 PartFactory.part_type_for[CT.WML_DOCUMENT_MACRO_ENABLED_MAIN] = DocumentPart
 PartFactory.part_type_for[CT.WML_FOOTER] = FooterPart
 PartFactory.part_type_for[CT.WML_HEADER] = HeaderPart
 PartFactory.part_type_for[CT.WML_NUMBERING] = NumberingPart
 PartFactory.part_type_for[CT.WML_SETTINGS] = SettingsPart
 PartFactory.part_type_for[CT.WML_STYLES] = StylesPart
+PartFactory.part_type_for[CT.WML_FOOTNOTES] = FootnotePart
 
 del (
     CT,
     CorePropertiesPart,
+    ExtendedPropertiesPart,
     DocumentPart,
     FooterPart,
     HeaderPart,
+    FootnotePart,
+    CommentPart,
     NumberingPart,
     PartFactory,
     SettingsPart,
     StylesPart,
     part_class_selector,
 )
```

### Comparing `python_docx_ng-0.9.3/docx/api.py` & `python_docx_ng-0.9.4.dev0/docx/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -31,7 +31,19 @@
 
 def _default_docx_path():
     """
     Return the path to the built-in default .docx package.
     """
     _thisdir = os.path.split(__file__)[0]
     return os.path.join(_thisdir, 'templates', 'default.docx')
+
+# TBD: review
+def element(single_element, part):
+    if str(type(single_element)) == "<class 'docx.oxml.text.paragraph.CT_P'>":
+        from .text.paragraph import Paragraph
+        return Paragraph(single_element, part)
+    elif str(type(single_element)) == "<class 'docx.oxml.table.CT_Tbl'>":
+        from .table import Table
+        return Table(single_element, part)
+    elif str(type(single_element)) == "<class 'docx.oxml.section.CT_SectPr'>":
+        from .section import Section
+        return Section(single_element, part)
```

### Comparing `python_docx_ng-0.9.3/docx/blkcntnr.py` & `python_docx_ng-0.9.4.dev0/docx/blkcntnr.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 Block level items are things like paragraph and table, although there are a few other
 specialized ones like structured document tags.
 """
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from docx.oxml.table import CT_Tbl
+from docx.oxml.ns import qn
 from docx.shared import Parented
 from docx.text.paragraph import Paragraph
-
+from docx.api import element
 
 class BlockItemContainer(Parented):
     """Base class for proxy objects that can contain block items.
 
     These containers include _Body, _Cell, header, footer, footnote, endnote, comment,
     and text box objects. Provides the shared functionality to add a block item like
     a paragraph or table.
@@ -63,13 +64,24 @@
         """
         A list containing the tables in this container, in document order.
         Read-only.
         """
         from .table import Table
         return [Table(tbl, self) for tbl in self._element.tbl_lst]
 
+    @property
+    def elements(self):
+        """
+        A list containing the elements in this container (paragraph and tables), in document order.
+        """
+        return [element(item,self.part) for item in self._element.getchildren()]
+
+    @property
+    def abstractNumIds(self):
+        return [numId for numId in self.part.numbering_part.element.iterchildren(qn('w:abstractNum'))]
+
     def _add_paragraph(self):
         """
         Return a paragraph newly added to the end of the content in this
         container.
         """
         return Paragraph(self._element.add_p(), self)
```

### Comparing `python_docx_ng-0.9.3/docx/compat.py` & `python_docx_ng-0.9.4.dev0/docx/compat.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/dml/color.py` & `python_docx_ng-0.9.4.dev0/docx/dml/color.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/document.py` & `python_docx_ng-0.9.4.dev0/docx/document.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # encoding: utf-8
 
 """|Document| and closely related objects"""
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
+from docx.oxml.ns import qn
+
 from docx.blkcntnr import BlockItemContainer
 from docx.enum.section import WD_SECTION
 from docx.enum.text import WD_BREAK
 from docx.section import Section, Sections
 from docx.shared import ElementProxy, Emu
 
 
@@ -97,14 +99,39 @@
     def core_properties(self):
         """
         A |CoreProperties| object providing read/write access to the core
         properties of this document.
         """
         return self._part.core_properties
 
+
+    @property
+    def extended_properties(self):
+        """
+        A |AppProperties| object providing read/write access to the app
+        properties of this document.
+        """
+        return self._part.extended_properties
+
+    @property
+    def comments_part(self):
+        """
+        A |Comments| object providing read/write access to the core
+        properties of this document.
+        """
+        return self.part.comments_part
+
+    # @property
+    # def footnotes_part(self):
+    #     """
+    #     A |Footnotes| object providing read/write access to the core
+    #     properties of this document.
+    #     """
+    #     return self.part._footnotes_part
+
     @property
     def inline_shapes(self):
         """
         An |InlineShapes| object providing access to the inline shapes in
         this document. An inline shape is a graphical object, such as
         a picture, contained in a run of text and behaving like a character
         glyph, being flowed like other text in a paragraph.
@@ -162,14 +189,31 @@
         top level of the document appear in this list; a table nested inside
         a table cell does not appear. A table within revision marks such as
         ``<w:ins>`` or ``<w:del>`` will also not appear in the list.
         """
         return self._body.tables
 
     @property
+    def elements(self):
+        return self._body.elements
+
+    @property
+    def abstractNumIds(self):
+        """
+        Returns list of all the 'w:abstarctNumId' of this document
+        """
+        return self._body.abstractNumIds
+
+    @property
+    def last_abs_num(self):
+        last = self.abstractNumIds[-1]
+        val = last.attrib.get(qn('w:abstractNumId'))
+        return  last, val
+
+    @property
     def _block_width(self):
         """
         Return a |Length| object specifying the width of available "writing"
         space between the margins of the last section of this document.
         """
         section = self.sections[-1]
         return Emu(
```

### Comparing `python_docx_ng-0.9.3/docx/enum/base.py` & `python_docx_ng-0.9.4.dev0/docx/enum/base.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/enum/dml.py` & `python_docx_ng-0.9.4.dev0/docx/enum/dml.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/enum/section.py` & `python_docx_ng-0.9.4.dev0/docx/enum/section.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/enum/style.py` & `python_docx_ng-0.9.4.dev0/docx/enum/style.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/enum/table.py` & `python_docx_ng-0.9.4.dev0/docx/enum/table.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/enum/text.py` & `python_docx_ng-0.9.4.dev0/docx/enum/text.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/__init__.py` & `python_docx_ng-0.9.4.dev0/docx/image/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 )
 
 from docx.image.bmp import Bmp
 from docx.image.gif import Gif
 from docx.image.jpeg import Exif, Jfif
 from docx.image.png import Png
 from docx.image.tiff import Tiff
+from docx.image.emf import Emf
 from docx.image.svg import Svg
+from docx.image.wmf import Wmf
 
 
 SIGNATURES = (
     # class, offset, signature_bytes
     (Png,  0, b'\x89PNG\x0D\x0A\x1A\x0A'),
     (Jfif, 6, b'JFIF'),
     (Exif, 6, b'Exif'),
     (Gif,  0, b'GIF87a'),
     (Gif,  0, b'GIF89a'),
     (Tiff, 0, b'MM\x00*'),  # big-endian (Motorola) TIFF
     (Tiff, 0, b'II*\x00'),  # little-endian (Intel) TIFF
     (Bmp,  0, b'BM'),
+    (Emf,  40, b' EMF'),
     (Svg,  0, b'<?xml version='),
+    (Wmf, 0, b'\xd7\xcd\xc6\x9a\x00\x00'),  # require wmf with Aldus Placeable Metafiles header
 )
```

### Comparing `python_docx_ng-0.9.3/docx/image/bmp.py` & `python_docx_ng-0.9.4.dev0/docx/image/bmp.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/constants.py` & `python_docx_ng-0.9.4.dev0/docx/image/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,17 @@
     Image content types
     """
     BMP = 'image/bmp'
     GIF = 'image/gif'
     JPEG = 'image/jpeg'
     PNG = 'image/png'
     TIFF = 'image/tiff'
+    EMF = 'image/emf'
     SVG = 'image/svg+xml'
+    WMF = 'image/wmf'
 
 
 class PNG_CHUNK_TYPE(object):
     """
     PNG chunk type names
     """
     IHDR = 'IHDR'
```

### Comparing `python_docx_ng-0.9.3/docx/image/gif.py` & `python_docx_ng-0.9.4.dev0/docx/image/gif.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/helpers.py` & `python_docx_ng-0.9.4.dev0/docx/image/helpers.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/image.py` & `python_docx_ng-0.9.4.dev0/docx/image/image.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/jpeg.py` & `python_docx_ng-0.9.4.dev0/docx/image/jpeg.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/png.py` & `python_docx_ng-0.9.4.dev0/docx/image/png.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/svg.py` & `python_docx_ng-0.9.4.dev0/docx/image/svg.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/image/tiff.py` & `python_docx_ng-0.9.4.dev0/docx/image/tiff.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/compat.py` & `python_docx_ng-0.9.4.dev0/docx/opc/compat.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/constants.py` & `python_docx_ng-0.9.4.dev0/docx/opc/constants.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/coreprops.py` & `python_docx_ng-0.9.4.dev0/docx/opc/coreprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/oxml.py` & `python_docx_ng-0.9.4.dev0/docx/opc/oxml.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/package.py` & `python_docx_ng-0.9.4.dev0/docx/opc/package.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.opc.packuri import PACKAGE_URI, PackURI
 from docx.opc.part import PartFactory
 from docx.opc.parts.coreprops import CorePropertiesPart
+from docx.opc.parts.extendedprops import ExtendedPropertiesPart
 from docx.opc.pkgreader import PackageReader
 from docx.opc.pkgwriter import PackageWriter
+from docx.parts.comment import CommentPart
+from docx.parts.footnote import FootnotePart
 from docx.opc.rel import Relationships
 from docx.opc.shared import lazyproperty
 
 
 class OpcPackage(object):
     """Main API class for |python-opc|.
 
@@ -37,14 +40,22 @@
     def core_properties(self):
         """
         |CoreProperties| object providing read/write access to the Dublin
         Core properties for this document.
         """
         return self._core_properties_part.core_properties
 
+    @property
+    def extended_properties(self):
+        """
+        |AppProperties| object providing read/write access to the Dublin
+        App properties for this document.
+        """
+        return self._extended_properties_part.extended_properties
+
     def iter_rels(self):
         """
         Generate exactly one reference to each relationship in the package by
         performing a depth-first traversal of the rels graph.
         """
         def walk_rels(source, visited=None):
             visited = [] if visited is None else visited
@@ -180,14 +191,53 @@
         try:
             return self.part_related_by(RT.CORE_PROPERTIES)
         except KeyError:
             core_properties_part = CorePropertiesPart.default(self)
             self.relate_to(core_properties_part, RT.CORE_PROPERTIES)
             return core_properties_part
 
+    @property
+    def _extended_properties_part(self):
+        """
+        |ExtendedPropertiesPart| object related to this package. Creates
+        a default app properties part if one is not present (not common).
+        """
+        try:
+            return self.part_related_by(RT.EXTENDED_PROPERTIES)
+        except KeyError:
+            extended_properties_part = ExtendedPropertiesPart.default(self)
+            self.relate_to(extended_properties_part, RT.EXTENDED_PROPERTIES)
+            return extended_properties_part
+
+    @property
+    def _comments_part(self):
+        """
+        |CommentsPart| object related to this package. Creates
+        a default Comments part if one is not present.
+        """
+        try:
+            return self.part_related_by(RT.COMMENTS)
+        except KeyError:
+            comments_part = CommentsPart.default(self)
+            self.relate_to(comments_part, RT.COMMENTS)
+            return comments_part
+
+    @property
+    def _footnotes_part(self):
+        """
+        |FootnotesPart| object related to this package. Creates
+        a default Comments part if one is not present.
+        """
+        try:
+            return self.part_related_by(RT.FOOTNOTES)
+        except KeyError:
+            footnotes_part = FootnotesPart.default(self)
+            self.relate_to(footnotes_part, RT.FOOTNOTES)
+            return footnotes_part
+
 
 class Unmarshaller(object):
     """Hosts static methods for unmarshalling a package from a |PackageReader|."""
 
     @staticmethod
     def unmarshal(pkg_reader, package, part_factory):
         """
```

### Comparing `python_docx_ng-0.9.3/docx/opc/packuri.py` & `python_docx_ng-0.9.4.dev0/docx/opc/packuri.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/part.py` & `python_docx_ng-0.9.4.dev0/docx/opc/part.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/parts/coreprops.py` & `python_docx_ng-0.9.4.dev0/docx/opc/parts/coreprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/phys_pkg.py` & `python_docx_ng-0.9.4.dev0/docx/opc/phys_pkg.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/pkgreader.py` & `python_docx_ng-0.9.4.dev0/docx/opc/pkgreader.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/pkgwriter.py` & `python_docx_ng-0.9.4.dev0/docx/opc/pkgwriter.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/rel.py` & `python_docx_ng-0.9.4.dev0/docx/opc/rel.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/shared.py` & `python_docx_ng-0.9.4.dev0/docx/opc/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/opc/spec.py` & `python_docx_ng-0.9.4.dev0/docx/opc/spec.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/__init__.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,14 +68,17 @@
 register_element_cls("w:evenAndOddHeaders", CT_OnOff)
 register_element_cls("w:titlePg", CT_OnOff)
 
 
 from .coreprops import CT_CoreProperties  # noqa
 register_element_cls('cp:coreProperties', CT_CoreProperties)
 
+from .extendedprops import CT_ExtendedProperties  # noqa
+register_element_cls('ep:Properties', CT_ExtendedProperties)
+
 from .document import CT_Body, CT_Document, CT_altChunk  # noqa
 register_element_cls('w:body',     CT_Body)
 register_element_cls('w:document', CT_Document)
 register_element_cls("w:altChunk", CT_altChunk)
 
 from .numbering import CT_Num, CT_Numbering, CT_NumLvl, CT_NumPr, CT_Lvl, CT_AbstractNum  # noqa
 register_element_cls('w:abstractNum',   CT_AbstractNum)
@@ -142,16 +145,19 @@
 register_element_cls('pic:nvPicPr',   CT_PictureNonVisual)
 register_element_cls('pic:pic',       CT_Picture)
 register_element_cls('pic:spPr',      CT_ShapeProperties)
 register_element_cls('wp:docPr',      CT_NonVisualDrawingProps)
 register_element_cls('wp:extent',     CT_PositiveSize2D)
 register_element_cls('wp:inline',     CT_Inline)
 
-from .styles import CT_LatentStyles, CT_LsdException, CT_Style, CT_Styles  # noqa
+from .styles import CT_DocDefaults, CT_RPrDefault, CT_PPrDefault, CT_LatentStyles, CT_LsdException, CT_Style, CT_Styles  # noqa
 register_element_cls('w:basedOn',        CT_String)
+register_element_cls('w:docDefaults',   CT_DocDefaults)
+register_element_cls('w:rPrDefault',   CT_RPrDefault)
+register_element_cls('w:pPrDefault',   CT_PPrDefault)
 register_element_cls('w:latentStyles',   CT_LatentStyles)
 register_element_cls('w:locked',         CT_OnOff)
 register_element_cls('w:lsdException',   CT_LsdException)
 register_element_cls('w:name',           CT_String)
 register_element_cls('w:next',           CT_String)
 register_element_cls('w:outlineLvl',     CT_DecimalNumber)
 register_element_cls('w:qFormat',        CT_OnOff)
@@ -170,26 +176,30 @@
     CT_TblLayoutType,
     CT_TblPr,
     CT_TblWidth,
     CT_Tc,
     CT_TcPr,
     CT_TrPr,
     CT_VMerge,
+    CT_TblMar,
     CT_VerticalJc,
+    CT_Bottom,
     CT_Border,
     CT_TcBorders,
     CT_TblBorders
 )
 register_element_cls('w:bidiVisual', CT_OnOff)
 register_element_cls('w:gridCol',    CT_TblGridCol)
 register_element_cls('w:gridSpan',   CT_DecimalNumber)
 register_element_cls('w:tbl',        CT_Tbl)
 register_element_cls('w:tblGrid',    CT_TblGrid)
 register_element_cls('w:tblLayout',  CT_TblLayoutType)
 register_element_cls('w:tblPr',      CT_TblPr)
+register_element_cls('w:tblW',       CT_TblWidth)
+register_element_cls('w:tblCellMar', CT_TblMar)
 register_element_cls('w:tblStyle',   CT_String)
 register_element_cls('w:tblCaption',   CT_String)
 register_element_cls('w:tblDescription',   CT_String)
 register_element_cls('w:tc',         CT_Tc)
 register_element_cls('w:tcPr',       CT_TcPr)
 register_element_cls('w:tcW',        CT_TblWidth)
 register_element_cls('w:tr',         CT_Row)
@@ -256,33 +266,37 @@
 register_element_cls('w:p', CT_P)
 
 from .text.parfmt import (  # noqa
     CT_Ind,
     CT_Jc,
     CT_PPr,
     CT_Spacing,
+    CT_Shading,
     CT_TabStop,
     CT_TabStops,
 )
 register_element_cls('w:ind',             CT_Ind)
 register_element_cls('w:jc',              CT_Jc)
 register_element_cls('w:keepLines',       CT_OnOff)
 register_element_cls('w:keepNext',        CT_OnOff)
 register_element_cls('w:pageBreakBefore', CT_OnOff)
 register_element_cls('w:pPr',             CT_PPr)
 register_element_cls('w:pStyle',          CT_String)
 register_element_cls('w:spacing',         CT_Spacing)
+register_element_cls('w:shd',             CT_Shading)
 register_element_cls('w:tab',             CT_TabStop)
 register_element_cls('w:tabs',            CT_TabStops)
 register_element_cls('w:widowControl',    CT_OnOff)
 
 from .text.run import CT_Br, CT_R, CT_Text  # noqa
 register_element_cls('w:br', CT_Br)
 register_element_cls('w:r',  CT_R)
 register_element_cls('w:t',  CT_Text)
+register_element_cls('w:rPr', CT_RPr)
+
 
 from .text.form import (
     CT_SimpleField,
     CT_FldChar,
     ST_FldCharType,
     CT_FFData,
     CT_FFDDList,
@@ -311,7 +325,23 @@
 register_element_cls('w:checked', CT_OnOff)
 register_element_cls('w:enabled', CT_OnOff)
 register_element_cls('w:calcOnExit', CT_OnOff)
 register_element_cls('w:maxLength', CT_DecimalNumber)
 register_element_cls('w:tabIndex', CT_DecimalNumber)
 register_element_cls('w:format', CT_String)
 register_element_cls('w:type', CT_FFTextType)
+
+
+from .comment import CT_Comments,CT_Com, CT_CRE, CT_CRS, CT_CRef
+register_element_cls('w:comments', CT_Comments)
+register_element_cls('w:comment', CT_Com)
+register_element_cls('w:commentRangeStart', CT_CRS)
+register_element_cls('w:commentRangeEnd', CT_CRE)
+register_element_cls('w:commentReference', CT_CRef)
+
+
+from .footnote import CT_Footnotes, CT_Footnote, CT_FNR, CT_FootnoteRef
+
+register_element_cls('w:footnotes', CT_Footnotes)
+register_element_cls('w:footnote', CT_Footnote)
+register_element_cls('w:footnoteReference', CT_FNR)
+register_element_cls('w:footnoteRef', CT_FootnoteRef)
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/coreprops.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/coreprops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/document.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/document.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/ns.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/ns.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from __future__ import absolute_import, print_function, unicode_literals
 
 
 nsmap = {
     "a": "http://schemas.openxmlformats.org/drawingml/2006/main",
     "c": "http://schemas.openxmlformats.org/drawingml/2006/chart",
     "cp": "http://schemas.openxmlformats.org/package/2006/metadata/core-properties",
+    "ep": "http://schemas.openxmlformats.org/officeDocument/2006/extended-properties",
+    "vt": "http://schemas.openxmlformats.org/officeDocument/2006/docPropsVTypes",
     "dc": "http://purl.org/dc/elements/1.1/",
     "dcmitype": "http://purl.org/dc/dcmitype/",
     "dcterms": "http://purl.org/dc/terms/",
     "dgm": "http://schemas.openxmlformats.org/drawingml/2006/diagram",
     "m": "http://schemas.openxmlformats.org/officeDocument/2006/math",
     "pic": "http://schemas.openxmlformats.org/drawingml/2006/picture",
     "r": "http://schemas.openxmlformats.org/officeDocument/2006/relationships",
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/numbering.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/numbering.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 
 class CT_Numbering(BaseOxmlElement):
     """
     ``<w:numbering>`` element, the root element of a numbering part, i.e.
     numbering.xml
     """
+    abstractNum = ZeroOrMore('w:abstractNum', successors=('w:num',))
     num = ZeroOrMore('w:num', successors=('w:numIdMacAtCleanup',))
 
     def add_num(self, abstractNum_id):
         """
         Return a newly added CT_Num (<w:num>) element referencing the
         abstract numbering definition identified by *abstractNum_id*.
         """
@@ -129,16 +130,18 @@
             if num not in num_ids:
                 break
         return num
 
 
 class CT_AbstractNum(BaseOxmlElement):
     """
-    ``<w:abstractNum>`` element, which represents a concrete list definition
+    ``<w:abstractNum>`` element, which represents an abstract numbering
+        definition that defines most of the formatting details.
     """
+    # abstractNumId = RequiredAttribute('w:abstractNumId', ST_DecimalNumber)
     abstractNumId = OneAndOnlyOne('w:abstractNumId')
     lvl = ZeroOrOne('w:lvl')
 
 
 class CT_Lvl(BaseOxmlElement):
     """
     ``<w:lvl>`` element, which represents a numbering level definition
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/section.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/section.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/settings.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/settings.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/shape.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/shape.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/shared.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/simpletypes.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/simpletypes.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/styles.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/styles.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,25 @@
         'heading 6': 'Heading6',
         'heading 7': 'Heading7',
         'heading 8': 'Heading8',
         'heading 9': 'Heading9',
     }.get(name, name.replace(' ', ''))
 
 
+class CT_DocDefaults(BaseOxmlElement):
+    _tag_seq = ('w:rPrDefault', 'w:pPrDefault')
+    rPrDefault = ZeroOrOne('w:rPrDefault', successors=(_tag_seq[1:]))
+    pPrDefault = ZeroOrOne('w:pPrDefault', successors=())
+
+class CT_RPrDefault(BaseOxmlElement):
+    rPr = ZeroOrOne('w:rPr', successors=())
+
+class CT_PPrDefault(BaseOxmlElement):
+    pPr = ZeroOrOne('w:pPr', successors=())
+
 class CT_LatentStyles(BaseOxmlElement):
     """
     `w:latentStyles` element, defining behavior defaults for latent styles
     and containing `w:lsdException` child elements that each override those
     defaults for a named latent style.
     """
     lsdException = ZeroOrMore('w:lsdException', successors=())
@@ -300,14 +311,15 @@
 
 class CT_Styles(BaseOxmlElement):
     """
     ``<w:styles>`` element, the root element of a styles part, i.e.
     styles.xml
     """
     _tag_seq = ('w:docDefaults', 'w:latentStyles', 'w:style')
+    docDefaults = ZeroOrOne('w:docDefaults', successors=_tag_seq[1:])
     latentStyles = ZeroOrOne('w:latentStyles', successors=_tag_seq[2:])
     style = ZeroOrMore('w:style', successors=())
     del _tag_seq
 
     def add_style_of_type(self, name, style_type, builtin):
         """
         Return a newly added `w:style` element having *name* and
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/table.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 """Custom element classes for tables"""
 
 from __future__ import (
     absolute_import, division, print_function, unicode_literals
 )
 
 from . import parse_xml
+from . import OxmlElement
 from ..enum.table import WD_CELL_VERTICAL_ALIGNMENT, WD_ROW_HEIGHT_RULE
 from ..exceptions import InvalidSpanError
-from .ns import nsdecls, qn
+from .ns import nsdecls, qn, nsmap
 from ..shared import Emu, Twips
 from .simpletypes import (
     ST_Merge, ST_TblLayoutType, ST_TblWidth, ST_TwipsMeasure, XsdInt, ST_Border,
-    ST_HexColor, ST_EighthPointMeasure, ST_PointMeasure
+    ST_HexColor, ST_EighthPointMeasure, ST_PointMeasure, ST_String
 )
 from .xmlchemy import (
     BaseOxmlElement, OneAndOnlyOne, OneOrMore, OptionalAttribute,
     RequiredAttribute, ZeroOrOne, ZeroOrMore
 )
 
 
@@ -230,14 +231,28 @@
                 '        <w:tcW w:type="dxa" w:w="%d"/>\n'
                 '      </w:tcPr>\n'
                 '      <w:p/>\n'
                 '    </w:tc>\n'
             ) % col_width.twips
         return xml
 
+    @property
+    def _section(self):
+        body = self.getparent()
+        sections = body.findall('.//w:sectPr', {'w':nsmap['w']})
+        if len(sections) == 1:
+            return sections[0]
+        else:
+            tbl_index = body.index(self)
+            for i,sect in enumerate(sections):
+                if i == len(sections) - 1 :
+                    return sect
+                else:
+                    if body.index(sect.getparent().getparent()) > tbl_index:
+                        return sect
 
 class CT_TblGrid(BaseOxmlElement):
     """
     ``<w:tblGrid>`` element, child of ``<w:tbl>``, holds ``<w:gridCol>``
     elements that define column count, width, etc.
     """
     gridCol = ZeroOrMore('w:gridCol', successors=('w:tblGridChange',))
@@ -273,18 +288,20 @@
     define table properties such as style and borders.
     """
     _tag_seq = (
         'w:tblStyle', 'w:tblpPr', 'w:tblOverlap', 'w:bidiVisual',
         'w:tblStyleRowBandSize', 'w:tblStyleColBandSize', 'w:tblW', 'w:jc',
         'w:tblCellSpacing', 'w:tblInd', 'w:tblBorders', 'w:shd',
         'w:tblLayout', 'w:tblCellMar', 'w:tblLook', 'w:tblCaption',
-        'w:tblDescription', 'w:tblPrChange'
+        'w:tblDescription', 'w:tblPrChange', 'w:tblPr'
     )
     tblStyle = ZeroOrOne('w:tblStyle', successors=_tag_seq[1:])
     bidiVisual = ZeroOrOne('w:bidiVisual', successors=_tag_seq[4:])
+    tblW = ZeroOrOne ('w:tblW', successors=_tag_seq[19:])
+    tblCellMar = ZeroOrOne('w:tblCellMar', successors=_tag_seq[19:])
     jc = ZeroOrOne('w:jc', successors=_tag_seq[8:])
     tblBorders = ZeroOrOne('w:tblBorders', successors=_tag_seq[11:])
     tblLayout = ZeroOrOne('w:tblLayout', successors=_tag_seq[13:])
     del _tag_seq
 
     @property
     def alignment(self):
@@ -538,17 +555,19 @@
             if top_tc is not self:
                 return ST_Merge.CONTINUE
             if height == 1:
                 return None
             return ST_Merge.RESTART
 
         top_tc = self if top_tc is None else top_tc
-        self._span_to_width(width, top_tc, vMerge_val(top_tc))
-        if height > 1:
-            self._tc_below._grow_to(width, height-1, top_tc)
+        for sigle_height in range(height):
+            self._span_to_width(width, top_tc, vMerge_val(top_tc))
+        # LEGACY
+        #if height > 1:
+        #    self._tc_below._grow_to(width, height-1, top_tc)
 
     def _insert_tcPr(self, tcPr):
         """
         ``tcPr`` has a bunch of successors, but it comes first if it appears,
         so just overriding and using insert(0, ...) rather than spelling out
         successors.
         """
@@ -960,19 +979,24 @@
                 element.sz = sz
             if space:
                 element.space = space
             if color:
                 element.color = color
             return element
 
+    def add_bottom_border(self, val, sz):
+        bottom = CT_Bottom.new(val, sz)
+        return self._insert_bottom(bottom)
+
     def remove_border(self, name):
         remove_method = getattr(self, '_remove_%s' % name, None)
         if remove_method:
             remove_method()
 
+
 class CT_TblBorders(BaseOxmlElement):
     _tag_seq = ('w:top', 'w:start', 'w:bottom', 'w:end', 'w:insideH', 'w:insideV')
     top = ZeroOrOne('w:top', successors=_tag_seq[1:])
     start = ZeroOrOne('w:start', successors=_tag_seq[2:])
     bottom = ZeroOrOne('w:bottom', successors=_tag_seq[3:])
     end = ZeroOrOne('w:end', successors=_tag_seq[4:])
     insideH = ZeroOrOne('w:insideH', successors=_tag_seq[5:])
@@ -1004,7 +1028,35 @@
                 element.color = color
             return element
 
     def remove_border(self, name):
         remove_method = getattr(self, '_remove_%s' % name, None)
         if remove_method:
             remove_method()
+
+
+class CT_TblMar(BaseOxmlElement):
+    """
+    ``<w:tblCellMar>`` element
+    """
+    left = ZeroOrOne('w:left', successors=('w:tblCellMar',))
+    right = ZeroOrOne('w:write', successors=('w:tblCellMar',))
+
+
+class CT_Bottom(BaseOxmlElement):
+    """
+    <w:bottom> element
+    """
+    val= OptionalAttribute('w:val', ST_String)
+    sz= OptionalAttribute('w:sz', ST_String)
+    space = OptionalAttribute('w:space', ST_String)
+    color = OptionalAttribute('w:color', ST_String)
+
+    @classmethod
+    def new(cls, val, sz):
+        bottom = OxmlElement('w:bottom')
+        bottom.val = val
+        bottom.sz = sz
+        bottom.space = "0"
+        bottom.color = "auto"
+
+        return bottom
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/text/font.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/text/font.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 class CT_Fonts(BaseOxmlElement):
     """
     ``<w:rFonts>`` element, specifying typeface name for the various language
     types.
     """
     ascii = OptionalAttribute('w:ascii', ST_String)
     hAnsi = OptionalAttribute('w:hAnsi', ST_String)
+    asciiTheme = OptionalAttribute('w:asciiTheme', ST_String)
+    hAnsiTheme = OptionalAttribute('w:hAnsiTheme', ST_String)
 
 
 class CT_Highlight(BaseOxmlElement):
     """
     `w:highlight` element, specifying font highlighting/background color.
     """
     val = RequiredAttribute('w:val', WD_COLOR)
@@ -187,14 +189,52 @@
     def rFonts_hAnsi(self, value):
         if value is None and self.rFonts is None:
             return
         rFonts = self.get_or_add_rFonts()
         rFonts.hAnsi = value
 
     @property
+    def rFonts_asciiTheme(self):
+        """
+        The value of `w:rFonts/@w:asciiTheme` or |None| if not present. Represents
+        the assigned typeface Theme. The rFonts element also specifies other
+        special-case typeface Theme; this method handles the case where just
+        the common Theme is required.
+        """
+        rFonts = self.rFonts
+        if rFonts is None:
+            return None
+        return rFonts.asciiTheme
+
+    @rFonts_asciiTheme.setter
+    def rFonts_asciiTheme(self, value):
+        if value is None:
+            self._remove_rFonts()
+            return
+        rFonts = self.get_or_add_rFonts()
+        rFonts.asciiTheme = value
+
+    @property
+    def rFonts_hAnsiTheme(self):
+        """
+        The value of `w:rFonts/@w:hAnsiTheme` or |None| if not present.
+        """
+        rFonts = self.rFonts
+        if rFonts is None:
+            return None
+        return rFonts.hAnsiTheme
+
+    @rFonts_hAnsiTheme.setter
+    def rFonts_hAnsiTheme(self, value):
+        if value is None and self.rFonts is None:
+            return
+        rFonts = self.get_or_add_rFonts()
+        rFonts.hAnsiTheme = value
+
+    @property
     def style(self):
         """
         String contained in <w:rStyle> child, or None if that element is not
         present.
         """
         rStyle = self.rStyle
         if rStyle is None:
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/text/form.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/text/form.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/oxml/text/paragraph.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/text/paragraph.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,14 +23,53 @@
         """
         Return a new ``<w:p>`` element inserted directly prior to this one.
         """
         new_p = OxmlElement('w:p')
         self.addprevious(new_p)
         return new_p
 
+    def link_comment(self, _id, rangeStart=0, rangeEnd=0):
+        rStart = OxmlElement('w:commentRangeStart')
+        rStart._id = _id
+        rEnd = OxmlElement('w:commentRangeEnd')
+        rEnd._id = _id
+        if rangeStart == 0 and rangeEnd == 0:
+            self.insert(0,rStart)
+            self.append(rEnd)
+        else:
+            self.insert(rangeStart,rStart)
+            if rangeEnd == len(self.getchildren() ) - 1 :
+                self.append(rEnd)
+            else:
+                self.insert(rangeEnd+1, rEnd)
+
+    def add_comm(self, author, comment_part, initials, dtime, comment_text, rangeStart, rangeEnd):
+        comment = comment_part.add_comment(author, initials, dtime)
+        comment._add_p(comment_text)
+        _r = self.add_r()
+        _r.add_comment_reference(comment._id)
+        self.link_comment(comment._id, rangeStart=rangeStart, rangeEnd=rangeEnd)
+
+        return comment
+
+    def add_fn(self, text, footnotes_part):
+        footnote = footnotes_part.add_footnote()
+        footnote._add_p(' '+text)
+        _r = self.add_r()
+        _r.add_footnote_reference(footnote._id)
+
+        return footnote
+
+    def footnote_style(self):
+        pPr = self.get_or_add_pPr()
+        rstyle = pPr.get_or_add_pStyle()
+        rstyle.val = 'FootnoteText'
+
+        return self
+
     @property
     def alignment(self):
         """
         The value of the ``<w:jc>`` grandchild element or |None| if not
         present.
         """
         pPr = self.pPr
@@ -57,22 +96,47 @@
         Unconditionally replace or add *sectPr* as a grandchild in the
         correct sequence.
         """
         pPr = self.get_or_add_pPr()
         pPr._remove_sectPr()
         pPr._insert_sectPr(sectPr)
 
+    def has_sectPr(self):
+        """
+        If has <w:sectPr>, return True, else return False
+        """
+        pPr = self.pPr
+        if pPr is None:
+            return False
+        return pPr.sectPr is not None
+
     @property
     def style(self):
         """
         String contained in w:val attribute of ./w:pPr/w:pStyle grandchild,
         or |None| if not present.
         """
         pPr = self.pPr
         if pPr is None:
             return None
         return pPr.style
 
+    @property
+    def comment_id(self):
+        _id = self.xpath('./w:commentRangeStart/@w:id')
+        if len(_id) > 1 or len(_id) == 0:
+            return None
+        else:
+            return int(_id[0])
+
+    @property
+    def footnote_ids(self):
+        _id = self.xpath('./w:r/w:footnoteReference/@w:id')
+        if  len(_id) == 0 :
+            return None
+        else:
+            return _id
+
     @style.setter
     def style(self, style):
         pPr = self.get_or_add_pPr()
         pPr.style = style
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/text/parfmt.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/text/parfmt.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 Custom element classes related to paragraph properties (CT_PPr).
 """
 
 from ...enum.text import (
     WD_ALIGN_PARAGRAPH, WD_LINE_SPACING, WD_TAB_ALIGNMENT, WD_TAB_LEADER
 )
 from ...shared import Length
-from ..simpletypes import ST_SignedTwipsMeasure, ST_TwipsMeasure
+from ..simpletypes import (
+    ST_SignedTwipsMeasure, ST_TwipsMeasure, ST_HexColor, ST_String
+)
 from ..xmlchemy import (
     BaseOxmlElement, OneOrMore, OptionalAttribute, RequiredAttribute,
     ZeroOrOne
 )
 
 
 class CT_Ind(BaseOxmlElement):
@@ -49,19 +51,21 @@
     )
     pStyle = ZeroOrOne('w:pStyle', successors=_tag_seq[1:])
     keepNext = ZeroOrOne('w:keepNext', successors=_tag_seq[2:])
     keepLines = ZeroOrOne('w:keepLines', successors=_tag_seq[3:])
     pageBreakBefore = ZeroOrOne('w:pageBreakBefore', successors=_tag_seq[4:])
     widowControl = ZeroOrOne('w:widowControl', successors=_tag_seq[6:])
     numPr = ZeroOrOne('w:numPr', successors=_tag_seq[7:])
+    shading = ZeroOrOne('w:shd', successors=_tag_seq[10:])
     tabs = ZeroOrOne('w:tabs', successors=_tag_seq[11:])
     spacing = ZeroOrOne('w:spacing', successors=_tag_seq[22:])
     ind = ZeroOrOne('w:ind', successors=_tag_seq[23:])
     jc = ZeroOrOne('w:jc', successors=_tag_seq[27:])
     outlineLvl = ZeroOrOne('w:outlineLvl', successors=_tag_seq[31:])
+    rPr = ZeroOrOne('w:rPr', successors=_tag_seq[34:])
     sectPr = ZeroOrOne('w:sectPr', successors=_tag_seq[36:])
     del _tag_seq
 
     @property
     def first_line_indent(self):
         """
         A |Length| value calculated from the values of `w:ind/@w:firstLine`
@@ -209,14 +213,46 @@
     def pageBreakBefore_val(self, value):
         if value is None:
             self._remove_pageBreakBefore()
         else:
             self.get_or_add_pageBreakBefore().val = value
 
     @property
+    def shading_color(self):
+        """
+        Value of `w:shd/@color` attribute, specifying foreground
+        color, or `None`.
+        """
+        shading = self.shading
+        if shading is None:
+            return None
+        return shading.color
+
+    @shading_color.setter
+    def shading_color(self, value):
+        highlight = self.get_or_add_shading()
+        highlight.color = value
+
+    @property
+    def shading_fill(self):
+        """
+        Value of `w:shd/@fill` attribute, specifying background
+        color, or `None`.
+        """
+        shading = self.shading
+        if shading is None:
+            return None
+        return shading.fill
+
+    @shading_fill.setter
+    def shading_fill(self, value):
+        shading = self.get_or_add_shading()
+        shading.fill = value
+
+    @property
     def spacing_after(self):
         """
         The value of `w:spacing/@w:after` or |None| if not present.
         """
         spacing = self.spacing
         if spacing is None:
             return None
@@ -321,14 +357,24 @@
     def widowControl_val(self, value):
         if value is None:
             self._remove_widowControl()
         else:
             self.get_or_add_widowControl().val = value
 
 
+class CT_Shading(BaseOxmlElement):
+    """
+    ``<w:shd>`` element, specifying Paragraph shading/background color and foreground pattern.
+    """
+    #val = OptionalAttribute('w:val', ST_String)
+    #color = OptionalAttribute('w:color', ST_HexColor)
+    fill = RequiredAttribute('w:fill', ST_HexColor)
+    #val = RequiredAttribute('w:val', WD_COLOR)
+
+
 class CT_Spacing(BaseOxmlElement):
     """
     ``<w:spacing>`` element, specifying paragraph spacing attributes such as
     space before and line spacing.
     """
     after = OptionalAttribute('w:after', ST_TwipsMeasure)
     before = OptionalAttribute('w:before', ST_TwipsMeasure)
```

### Comparing `python_docx_ng-0.9.3/docx/oxml/xmlchemy.py` & `python_docx_ng-0.9.4.dev0/docx/oxml/xmlchemy.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/package.py` & `python_docx_ng-0.9.4.dev0/docx/package.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/parts/altchunk.py` & `python_docx_ng-0.9.4.dev0/docx/parts/altchunk.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/parts/document.py` & `python_docx_ng-0.9.4.dev0/docx/parts/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from docx.document import Document
 from docx.opc.constants import RELATIONSHIP_TYPE as RT
 from docx.parts.hdrftr import FooterPart, HeaderPart
 from docx.parts.numbering import NumberingPart
 from docx.parts.settings import SettingsPart
 from docx.parts.story import BaseStoryPart
 from docx.parts.styles import StylesPart
+from docx.parts.comment import CommentPart
+from docx.parts.footnotes import FootnotesPart
 from docx.shape import InlineShapes
 from docx.shared import lazyproperty
 
 
 class DocumentPart(BaseStoryPart):
     """Main document part of a WordprocessingML (WML) package, aka a .docx file.
 
@@ -41,14 +43,22 @@
         """
         A |CoreProperties| object providing read/write access to the core
         properties of this document.
         """
         return self.package.core_properties
 
     @property
+    def extended_properties(self):
+        """
+        A |AppProperties| object providing read/write access to the app
+        properties of this document.
+        """
+        return self.package.extended_properties
+
+    @property
     def document(self):
         """
         A |Document| object providing access to the content of this document.
         """
         return Document(self._element, self)
 
     def drop_header_part(self, rId):
```

### Comparing `python_docx_ng-0.9.3/docx/parts/hdrftr.py` & `python_docx_ng-0.9.4.dev0/docx/parts/hdrftr.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/parts/image.py` & `python_docx_ng-0.9.4.dev0/docx/parts/image.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/parts/numbering.py` & `python_docx_ng-0.9.4.dev0/docx/parts/numbering.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/parts/settings.py` & `python_docx_ng-0.9.4.dev0/docx/parts/settings.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/parts/story.py` & `python_docx_ng-0.9.4.dev0/docx/parts/story.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,20 +57,21 @@
         cx, cy = image.scaled_dimensions(width, height)
         shape_id, filename = self.next_id, image.filename
         return CT_Inline.new_pic_inline(shape_id, rId, filename, cx, cy)
 
     @property
     def next_id(self):
         """
-        The next available positive integer id value in this document. Gaps
+        The next available positive integer id value in this document.
+        The value is determined by incrementing the maximum existing id value. Gaps
         in id sequence are filled. The id attribute value is unique in the
         document, without regard to the element type it appears on.
         """
         id_str_lst = self._element.xpath('//@id')
-        used_ids = [int(id_str) for id_str in id_str_lst if id_str.isdigit() and int(id_str)>100000]
+        used_ids = [int(id_str) for id_str in id_str_lst if id_str.isdigit() and int(id_str) > 100000]
         for n in range(100001, len(used_ids)+100002):
             if n not in used_ids:
                 return n
 
     @lazyproperty
     def _document_part(self):
         """|DocumentPart| object for this package."""
```

### Comparing `python_docx_ng-0.9.3/docx/parts/styles.py` & `python_docx_ng-0.9.4.dev0/docx/parts/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/section.py` & `python_docx_ng-0.9.4.dev0/docx/section.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 from docx.blkcntnr import BlockItemContainer
 from docx.compat import Sequence
 from docx.enum.section import WD_HEADER_FOOTER
 from docx.shared import lazyproperty
+from docx.text.paragraph import Paragraph
 
 
 class Sections(Sequence):
     """Sequence of |Section| objects corresponding to the sections in the document.
 
     Supports ``len()``, iteration, and indexed access.
     """
@@ -254,14 +255,44 @@
         """
         return self._sectPr.top_margin
 
     @top_margin.setter
     def top_margin(self, value):
         self._sectPr.top_margin = value
 
+    @property
+    def paragraphs(self):
+        """
+        Get paragraphs in this section
+        """
+        from docx.oxml.document import CT_Body
+
+        paragraphs = []
+        if isinstance(self._sectPr.getparent(), CT_Body):
+            # last section
+            return self._paragraphs_until_section_break(self._sectPr)
+        else:
+            # user custom section
+            return self._paragraphs_until_section_break(self._sectPr.getparent().getparent())
+
+    @staticmethod
+    def _paragraphs_until_section_break(start):
+        from docx.oxml.text.paragraph import CT_P
+        paragraphs = [Paragraph(start, start.getparent())] if isinstance(start, CT_P) else []
+        start = start.getprevious()
+
+        while start is not None:
+            if isinstance(start, CT_P):
+                paragraph = Paragraph(start, start.getparent())
+                if paragraph.is_section_break():
+                    break
+                paragraphs.insert(0, paragraph)
+            start = start.getprevious()
+        return paragraphs
+
 
 class _BaseHeaderFooter(BlockItemContainer):
     """Base class for header and footer classes"""
 
     def __init__(self, sectPr, document_part, header_footer_index):
         self._sectPr = sectPr
         self._document_part = document_part
```

### Comparing `python_docx_ng-0.9.3/docx/settings.py` & `python_docx_ng-0.9.4.dev0/docx/settings.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/shape.py` & `python_docx_ng-0.9.4.dev0/docx/shape.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/shared.py` & `python_docx_ng-0.9.4.dev0/docx/shared.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/styles/__init__.py` & `python_docx_ng-0.9.4.dev0/docx/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/styles/latent.py` & `python_docx_ng-0.9.4.dev0/docx/styles/latent.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/styles/style.py` & `python_docx_ng-0.9.4.dev0/docx/styles/style.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/styles/styles.py` & `python_docx_ng-0.9.4.dev0/docx/styles/styles.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/table.py` & `python_docx_ng-0.9.4.dev0/docx/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from __future__ import absolute_import, print_function, unicode_literals
 
 from .blkcntnr import BlockItemContainer
 from .enum.style import WD_STYLE_TYPE
 from .oxml.simpletypes import ST_Merge
 from .shared import Inches, lazyproperty, Parented
+from .section import Section
 
 
 class Table(Parented):
     """
     Proxy class for a WordprocessingML ``<w:tbl>`` element.
     """
     def __init__(self, tbl, parent):
@@ -45,14 +46,18 @@
         for gridCol in tbl.tblGrid.gridCol_lst:
             tc = tr.add_tc()
             tc.width = gridCol.w
         self._update_cache = True
         return _Row(tr, self)
 
     @property
+    def section(self):
+        return Section(self._element._section, self.part)
+
+    @property
     def alignment(self):
         """
         Read/write. A member of :ref:`WdRowAlignment` or None, specifying the
         positioning of this table between the page margins. |None| if no
         setting is specified, causing the effective value to be inherited
         from the style hierarchy.
         """
@@ -77,41 +82,47 @@
         self._tblPr.autofit = value
 
     def cell(self, row_idx, col_idx):
         """
         Return |_Cell| instance correponding to table cell at *row_idx*,
         *col_idx* intersection, where (0, 0) is the top, left-most cell.
         """
-        cell_idx = col_idx + (row_idx * self._column_count)
-        return self._cells[cell_idx]
+        # LEGACY: leave here to see original code
+        # cell_idx = col_idx + (row_idx * self._column_count)
+        # return self._cells[cell_idx]
+        return self._cells[row_idx][col_idx]
 
     def column_cells(self, column_idx):
         """
         Sequence of cells in the column at *column_idx* in this table.
         """
         cells = self._cells
-        idxs = range(column_idx, len(cells), self._column_count)
-        return [cells[idx] for idx in idxs]
+        # LEGACY: leave here to see original code
+        # idxs = range(column_idx, len(cells), self._column_count)
+        # return [cells[idx] for idx in idxs]
+        return [cells[row_idx][column_idx] for row_idx in range(0, len(cells))]
 
     @lazyproperty
     def columns(self):
         """
         |_Columns| instance representing the sequence of columns in this
         table.
         """
         return _Columns(self._tbl, self)
 
     def row_cells(self, row_idx):
         """
         Sequence of cells in the row at *row_idx* in this table.
         """
-        column_count = self._column_count
-        start = row_idx * column_count
-        end = start + column_count
-        return self._cells[start:end]
+        # LEGACY: leave here to see original code
+        # column_count = self._column_count
+        # start = row_idx * column_count
+        # end = start + column_count
+        # return self._cells[start:end]
+        return self._cells[row_idx]
 
     @lazyproperty
     def rows(self):
         """
         |_Rows| instance containing the sequence of rows in this table.
         """
         return _Rows(self._tbl, self)
@@ -161,34 +172,46 @@
     @table_direction.setter
     def table_direction(self, value):
         self._element.bidiVisual_val = value
 
     @property
     def _cells(self):
         """
-        A sequence of |_Cell| objects, one for each cell of the layout grid.
+        A matrix of |_Cell| objects, one for each cell of the layout grid.
         If the table contains a span, one or more |_Cell| object references
         are repeated.
         """
         if not self._update_cache:
             return self._cached_cells
-        col_count = self._column_count
+        # LEGACY: leave here to see original code
+        # col_count = self._column_count
         cells = []
-        for tc in self._tbl.iter_tcs():
-            for grid_span_idx in range(tc.grid_span):
-                if tc.vMerge == ST_Merge.CONTINUE:
-                    cells.append(cells[-col_count])
-                elif grid_span_idx > 0:
-                    cells.append(cells[-1])
-                else:
-                    cells.append(_Cell(tc, self))
-        self._cached_cells = cells
-        self._update_cache = False
+        # for tc in self._tbl.iter_tcs():
+        #     for grid_span_idx in range(tc.grid_span):
+        #         if tc.vMerge == ST_Merge.CONTINUE:
+        #             cells.append(cells[-col_count])
+        #         elif grid_span_idx > 0:
+        #             cells.append(cells[-1])
+        #         else:
+        #             cells.append(_Cell(tc, self))
+        # self._cached_cells = cells
+        # self._update_cache = False
+        for row_idx, tr in enumerate(self._tbl.tr_lst):
+            cells.append([])
+            for col_idx, tc in enumerate(tr.tc_lst):
+                for grid_span_idx in range(tc.grid_span):
+                    if tc.vMerge == ST_Merge.CONTINUE:
+                        cells[row_idx].append(cells[row_idx - 1][col_idx])
+                    elif grid_span_idx > 0:
+                        cells[row_idx].append(cells[row_idx][col_idx])
+                    else:
+                        cells[row_idx].append(_Cell(tc, self))
         return cells
 
+
     @property
     def _column_count(self):
         """
         The number of grid columns in this table.
         """
         return self._tbl.col_count
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/[Content_Types].xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/[Content_Types].xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (1388), with CRLF line terminators*

 * *Files 1% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 5479 7065 7320  "yes"?>..<Types 
-00000040: 786d 6c6e 733d 2268 7474 703a 2f2f 7363  xmlns="http://sc
-00000050: 6865 6d61 732e 6f70 656e 786d 6c66 6f72  hemas.openxmlfor
-00000060: 6d61 7473 2e6f 7267 2f70 6163 6b61 6765  mats.org/package
-00000070: 2f32 3030 362f 636f 6e74 656e 742d 7479  /2006/content-ty
-00000080: 7065 7322 3e3c 4465 6661 756c 7420 4578  pes"><Default Ex
-00000090: 7465 6e73 696f 6e3d 2272 656c 7322 2043  tension="rels" C
-000000a0: 6f6e 7465 6e74 5479 7065 3d22 6170 706c  ontentType="appl
-000000b0: 6963 6174 696f 6e2f 766e 642e 6f70 656e  ication/vnd.open
-000000c0: 786d 6c66 6f72 6d61 7473 2d70 6163 6b61  xmlformats-packa
-000000d0: 6765 2e72 656c 6174 696f 6e73 6869 7073  ge.relationships
-000000e0: 2b78 6d6c 222f 3e3c 4465 6661 756c 7420  +xml"/><Default 
-000000f0: 4578 7465 6e73 696f 6e3d 2278 6d6c 2220  Extension="xml" 
-00000100: 436f 6e74 656e 7454 7970 653d 2261 7070  ContentType="app
-00000110: 6c69 6361 7469 6f6e 2f78 6d6c 222f 3e3c  lication/xml"/><
-00000120: 4f76 6572 7269 6465 2050 6172 744e 616d  Override PartNam
-00000130: 653d 222f 776f 7264 2f64 6f63 756d 656e  e="/word/documen
-00000140: 742e 786d 6c22 2043 6f6e 7465 6e74 5479  t.xml" ContentTy
-00000150: 7065 3d22 6170 706c 6963 6174 696f 6e2f  pe="application/
-00000160: 766e 642e 6f70 656e 786d 6c66 6f72 6d61  vnd.openxmlforma
-00000170: 7473 2d6f 6666 6963 6564 6f63 756d 656e  ts-officedocumen
-00000180: 742e 776f 7264 7072 6f63 6573 7369 6e67  t.wordprocessing
-00000190: 6d6c 2e64 6f63 756d 656e 742e 6d61 696e  ml.document.main
-000001a0: 2b78 6d6c 222f 3e3c 4f76 6572 7269 6465  +xml"/><Override
-000001b0: 2050 6172 744e 616d 653d 222f 776f 7264   PartName="/word
-000001c0: 2f6e 756d 6265 7269 6e67 2e78 6d6c 2220  /numbering.xml" 
-000001d0: 436f 6e74 656e 7454 7970 653d 2261 7070  ContentType="app
-000001e0: 6c69 6361 7469 6f6e 2f76 6e64 2e6f 7065  lication/vnd.ope
-000001f0: 6e78 6d6c 666f 726d 6174 732d 6f66 6669  nxmlformats-offi
-00000200: 6365 646f 6375 6d65 6e74 2e77 6f72 6470  cedocument.wordp
-00000210: 726f 6365 7373 696e 676d 6c2e 6e75 6d62  rocessingml.numb
-00000220: 6572 696e 672b 786d 6c22 2f3e 3c4f 7665  ering+xml"/><Ove
-00000230: 7272 6964 6520 5061 7274 4e61 6d65 3d22  rride PartName="
-00000240: 2f77 6f72 642f 7374 796c 6573 2e78 6d6c  /word/styles.xml
-00000250: 2220 436f 6e74 656e 7454 7970 653d 2261  " ContentType="a
-00000260: 7070 6c69 6361 7469 6f6e 2f76 6e64 2e6f  pplication/vnd.o
-00000270: 7065 6e78 6d6c 666f 726d 6174 732d 6f66  penxmlformats-of
-00000280: 6669 6365 646f 6375 6d65 6e74 2e77 6f72  ficedocument.wor
-00000290: 6470 726f 6365 7373 696e 676d 6c2e 7374  dprocessingml.st
-000002a0: 796c 6573 2b78 6d6c 222f 3e3c 4f76 6572  yles+xml"/><Over
-000002b0: 7269 6465 2050 6172 744e 616d 653d 222f  ride PartName="/
-000002c0: 776f 7264 2f73 6574 7469 6e67 732e 786d  word/settings.xm
-000002d0: 6c22 2043 6f6e 7465 6e74 5479 7065 3d22  l" ContentType="
-000002e0: 6170 706c 6963 6174 696f 6e2f 766e 642e  application/vnd.
-000002f0: 6f70 656e 786d 6c66 6f72 6d61 7473 2d6f  openxmlformats-o
-00000300: 6666 6963 6564 6f63 756d 656e 742e 776f  fficedocument.wo
-00000310: 7264 7072 6f63 6573 7369 6e67 6d6c 2e73  rdprocessingml.s
-00000320: 6574 7469 6e67 732b 786d 6c22 2f3e 3c4f  ettings+xml"/><O
-00000330: 7665 7272 6964 6520 5061 7274 4e61 6d65  verride PartName
-00000340: 3d22 2f77 6f72 642f 7765 6253 6574 7469  ="/word/webSetti
-00000350: 6e67 732e 786d 6c22 2043 6f6e 7465 6e74  ngs.xml" Content
-00000360: 5479 7065 3d22 6170 706c 6963 6174 696f  Type="applicatio
-00000370: 6e2f 766e 642e 6f70 656e 786d 6c66 6f72  n/vnd.openxmlfor
-00000380: 6d61 7473 2d6f 6666 6963 6564 6f63 756d  mats-officedocum
-00000390: 656e 742e 776f 7264 7072 6f63 6573 7369  ent.wordprocessi
-000003a0: 6e67 6d6c 2e77 6562 5365 7474 696e 6773  ngml.webSettings
-000003b0: 2b78 6d6c 222f 3e3c 4f76 6572 7269 6465  +xml"/><Override
-000003c0: 2050 6172 744e 616d 653d 222f 776f 7264   PartName="/word
-000003d0: 2f66 6f6e 7454 6162 6c65 2e78 6d6c 2220  /fontTable.xml" 
-000003e0: 436f 6e74 656e 7454 7970 653d 2261 7070  ContentType="app
-000003f0: 6c69 6361 7469 6f6e 2f76 6e64 2e6f 7065  lication/vnd.ope
-00000400: 6e78 6d6c 666f 726d 6174 732d 6f66 6669  nxmlformats-offi
-00000410: 6365 646f 6375 6d65 6e74 2e77 6f72 6470  cedocument.wordp
-00000420: 726f 6365 7373 696e 676d 6c2e 666f 6e74  rocessingml.font
-00000430: 5461 626c 652b 786d 6c22 2f3e 3c4f 7665  Table+xml"/><Ove
-00000440: 7272 6964 6520 5061 7274 4e61 6d65 3d22  rride PartName="
-00000450: 2f77 6f72 642f 7468 656d 652f 7468 656d  /word/theme/them
-00000460: 6531 2e78 6d6c 2220 436f 6e74 656e 7454  e1.xml" ContentT
-00000470: 7970 653d 2261 7070 6c69 6361 7469 6f6e  ype="application
-00000480: 2f76 6e64 2e6f 7065 6e78 6d6c 666f 726d  /vnd.openxmlform
-00000490: 6174 732d 6f66 6669 6365 646f 6375 6d65  ats-officedocume
-000004a0: 6e74 2e74 6865 6d65 2b78 6d6c 222f 3e3c  nt.theme+xml"/><
-000004b0: 4f76 6572 7269 6465 2050 6172 744e 616d  Override PartNam
-000004c0: 653d 222f 646f 6350 726f 7073 2f63 6f72  e="/docProps/cor
-000004d0: 652e 786d 6c22 2043 6f6e 7465 6e74 5479  e.xml" ContentTy
-000004e0: 7065 3d22 6170 706c 6963 6174 696f 6e2f  pe="application/
-000004f0: 766e 642e 6f70 656e 786d 6c66 6f72 6d61  vnd.openxmlforma
-00000500: 7473 2d70 6163 6b61 6765 2e63 6f72 652d  ts-package.core-
-00000510: 7072 6f70 6572 7469 6573 2b78 6d6c 222f  properties+xml"/
-00000520: 3e3c 4f76 6572 7269 6465 2050 6172 744e  ><Override PartN
-00000530: 616d 653d 222f 646f 6350 726f 7073 2f61  ame="/docProps/a
-00000540: 7070 2e78 6d6c 2220 436f 6e74 656e 7454  pp.xml" ContentT
-00000550: 7970 653d 2261 7070 6c69 6361 7469 6f6e  ype="application
-00000560: 2f76 6e64 2e6f 7065 6e78 6d6c 666f 726d  /vnd.openxmlform
-00000570: 6174 732d 6f66 6669 6365 646f 6375 6d65  ats-officedocume
-00000580: 6e74 2e65 7874 656e 6465 642d 7072 6f70  nt.extended-prop
-00000590: 6572 7469 6573 2b78 6d6c 222f 3e3c 2f54  erties+xml"/></T
-000005a0: 7970 6573 3e                             ypes>
+00000030: 2279 6573 223f 3e0a 3c54 7970 6573 2078  "yes"?>.<Types x
+00000040: 6d6c 6e73 3d22 6874 7470 3a2f 2f73 6368  mlns="http://sch
+00000050: 656d 6173 2e6f 7065 6e78 6d6c 666f 726d  emas.openxmlform
+00000060: 6174 732e 6f72 672f 7061 636b 6167 652f  ats.org/package/
+00000070: 3230 3036 2f63 6f6e 7465 6e74 2d74 7970  2006/content-typ
+00000080: 6573 223e 3c44 6566 6175 6c74 2045 7874  es"><Default Ext
+00000090: 656e 7369 6f6e 3d22 7265 6c73 2220 436f  ension="rels" Co
+000000a0: 6e74 656e 7454 7970 653d 2261 7070 6c69  ntentType="appli
+000000b0: 6361 7469 6f6e 2f76 6e64 2e6f 7065 6e78  cation/vnd.openx
+000000c0: 6d6c 666f 726d 6174 732d 7061 636b 6167  mlformats-packag
+000000d0: 652e 7265 6c61 7469 6f6e 7368 6970 732b  e.relationships+
+000000e0: 786d 6c22 2f3e 3c44 6566 6175 6c74 2045  xml"/><Default E
+000000f0: 7874 656e 7369 6f6e 3d22 786d 6c22 2043  xtension="xml" C
+00000100: 6f6e 7465 6e74 5479 7065 3d22 6170 706c  ontentType="appl
+00000110: 6963 6174 696f 6e2f 786d 6c22 2f3e 3c4f  ication/xml"/><O
+00000120: 7665 7272 6964 6520 5061 7274 4e61 6d65  verride PartName
+00000130: 3d22 2f77 6f72 642f 646f 6375 6d65 6e74  ="/word/document
+00000140: 2e78 6d6c 2220 436f 6e74 656e 7454 7970  .xml" ContentTyp
+00000150: 653d 2261 7070 6c69 6361 7469 6f6e 2f76  e="application/v
+00000160: 6e64 2e6f 7065 6e78 6d6c 666f 726d 6174  nd.openxmlformat
+00000170: 732d 6f66 6669 6365 646f 6375 6d65 6e74  s-officedocument
+00000180: 2e77 6f72 6470 726f 6365 7373 696e 676d  .wordprocessingm
+00000190: 6c2e 646f 6375 6d65 6e74 2e6d 6169 6e2b  l.document.main+
+000001a0: 786d 6c22 2f3e 3c4f 7665 7272 6964 6520  xml"/><Override 
+000001b0: 5061 7274 4e61 6d65 3d22 2f77 6f72 642f  PartName="/word/
+000001c0: 6e75 6d62 6572 696e 672e 786d 6c22 2043  numbering.xml" C
+000001d0: 6f6e 7465 6e74 5479 7065 3d22 6170 706c  ontentType="appl
+000001e0: 6963 6174 696f 6e2f 766e 642e 6f70 656e  ication/vnd.open
+000001f0: 786d 6c66 6f72 6d61 7473 2d6f 6666 6963  xmlformats-offic
+00000200: 6564 6f63 756d 656e 742e 776f 7264 7072  edocument.wordpr
+00000210: 6f63 6573 7369 6e67 6d6c 2e6e 756d 6265  ocessingml.numbe
+00000220: 7269 6e67 2b78 6d6c 222f 3e3c 4f76 6572  ring+xml"/><Over
+00000230: 7269 6465 2050 6172 744e 616d 653d 222f  ride PartName="/
+00000240: 776f 7264 2f73 7479 6c65 732e 786d 6c22  word/styles.xml"
+00000250: 2043 6f6e 7465 6e74 5479 7065 3d22 6170   ContentType="ap
+00000260: 706c 6963 6174 696f 6e2f 766e 642e 6f70  plication/vnd.op
+00000270: 656e 786d 6c66 6f72 6d61 7473 2d6f 6666  enxmlformats-off
+00000280: 6963 6564 6f63 756d 656e 742e 776f 7264  icedocument.word
+00000290: 7072 6f63 6573 7369 6e67 6d6c 2e73 7479  processingml.sty
+000002a0: 6c65 732b 786d 6c22 2f3e 3c4f 7665 7272  les+xml"/><Overr
+000002b0: 6964 6520 5061 7274 4e61 6d65 3d22 2f77  ide PartName="/w
+000002c0: 6f72 642f 7365 7474 696e 6773 2e78 6d6c  ord/settings.xml
+000002d0: 2220 436f 6e74 656e 7454 7970 653d 2261  " ContentType="a
+000002e0: 7070 6c69 6361 7469 6f6e 2f76 6e64 2e6f  pplication/vnd.o
+000002f0: 7065 6e78 6d6c 666f 726d 6174 732d 6f66  penxmlformats-of
+00000300: 6669 6365 646f 6375 6d65 6e74 2e77 6f72  ficedocument.wor
+00000310: 6470 726f 6365 7373 696e 676d 6c2e 7365  dprocessingml.se
+00000320: 7474 696e 6773 2b78 6d6c 222f 3e3c 4f76  ttings+xml"/><Ov
+00000330: 6572 7269 6465 2050 6172 744e 616d 653d  erride PartName=
+00000340: 222f 776f 7264 2f77 6562 5365 7474 696e  "/word/webSettin
+00000350: 6773 2e78 6d6c 2220 436f 6e74 656e 7454  gs.xml" ContentT
+00000360: 7970 653d 2261 7070 6c69 6361 7469 6f6e  ype="application
+00000370: 2f76 6e64 2e6f 7065 6e78 6d6c 666f 726d  /vnd.openxmlform
+00000380: 6174 732d 6f66 6669 6365 646f 6375 6d65  ats-officedocume
+00000390: 6e74 2e77 6f72 6470 726f 6365 7373 696e  nt.wordprocessin
+000003a0: 676d 6c2e 7765 6253 6574 7469 6e67 732b  gml.webSettings+
+000003b0: 786d 6c22 2f3e 3c4f 7665 7272 6964 6520  xml"/><Override 
+000003c0: 5061 7274 4e61 6d65 3d22 2f77 6f72 642f  PartName="/word/
+000003d0: 666f 6e74 5461 626c 652e 786d 6c22 2043  fontTable.xml" C
+000003e0: 6f6e 7465 6e74 5479 7065 3d22 6170 706c  ontentType="appl
+000003f0: 6963 6174 696f 6e2f 766e 642e 6f70 656e  ication/vnd.open
+00000400: 786d 6c66 6f72 6d61 7473 2d6f 6666 6963  xmlformats-offic
+00000410: 6564 6f63 756d 656e 742e 776f 7264 7072  edocument.wordpr
+00000420: 6f63 6573 7369 6e67 6d6c 2e66 6f6e 7454  ocessingml.fontT
+00000430: 6162 6c65 2b78 6d6c 222f 3e3c 4f76 6572  able+xml"/><Over
+00000440: 7269 6465 2050 6172 744e 616d 653d 222f  ride PartName="/
+00000450: 776f 7264 2f74 6865 6d65 2f74 6865 6d65  word/theme/theme
+00000460: 312e 786d 6c22 2043 6f6e 7465 6e74 5479  1.xml" ContentTy
+00000470: 7065 3d22 6170 706c 6963 6174 696f 6e2f  pe="application/
+00000480: 766e 642e 6f70 656e 786d 6c66 6f72 6d61  vnd.openxmlforma
+00000490: 7473 2d6f 6666 6963 6564 6f63 756d 656e  ts-officedocumen
+000004a0: 742e 7468 656d 652b 786d 6c22 2f3e 3c4f  t.theme+xml"/><O
+000004b0: 7665 7272 6964 6520 5061 7274 4e61 6d65  verride PartName
+000004c0: 3d22 2f64 6f63 5072 6f70 732f 636f 7265  ="/docProps/core
+000004d0: 2e78 6d6c 2220 436f 6e74 656e 7454 7970  .xml" ContentTyp
+000004e0: 653d 2261 7070 6c69 6361 7469 6f6e 2f76  e="application/v
+000004f0: 6e64 2e6f 7065 6e78 6d6c 666f 726d 6174  nd.openxmlformat
+00000500: 732d 7061 636b 6167 652e 636f 7265 2d70  s-package.core-p
+00000510: 726f 7065 7274 6965 732b 786d 6c22 2f3e  roperties+xml"/>
+00000520: 3c4f 7665 7272 6964 6520 5061 7274 4e61  <Override PartNa
+00000530: 6d65 3d22 2f64 6f63 5072 6f70 732f 6170  me="/docProps/ap
+00000540: 702e 786d 6c22 2043 6f6e 7465 6e74 5479  p.xml" ContentTy
+00000550: 7065 3d22 6170 706c 6963 6174 696f 6e2f  pe="application/
+00000560: 766e 642e 6f70 656e 786d 6c66 6f72 6d61  vnd.openxmlforma
+00000570: 7473 2d6f 6666 6963 6564 6f63 756d 656e  ts-officedocumen
+00000580: 742e 6578 7465 6e64 6564 2d70 726f 7065  t.extended-prope
+00000590: 7274 6965 732b 786d 6c22 2f3e 3c2f 5479  rties+xml"/></Ty
+000005a0: 7065 733e                                pes>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/_rels/.rels` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/_rels/.rels`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (533), with CRLF line terminators*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 5265 6c61 7469  "yes"?>..<Relati
-00000040: 6f6e 7368 6970 7320 786d 6c6e 733d 2268  onships xmlns="h
-00000050: 7474 703a 2f2f 7363 6865 6d61 732e 6f70  ttp://schemas.op
-00000060: 656e 786d 6c66 6f72 6d61 7473 2e6f 7267  enxmlformats.org
-00000070: 2f70 6163 6b61 6765 2f32 3030 362f 7265  /package/2006/re
-00000080: 6c61 7469 6f6e 7368 6970 7322 3e3c 5265  lationships"><Re
-00000090: 6c61 7469 6f6e 7368 6970 2049 643d 2272  lationship Id="r
-000000a0: 4964 3322 2054 7970 653d 2268 7474 703a  Id3" Type="http:
-000000b0: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
-000000c0: 6c66 6f72 6d61 7473 2e6f 7267 2f6f 6666  lformats.org/off
-000000d0: 6963 6544 6f63 756d 656e 742f 3230 3036  iceDocument/2006
-000000e0: 2f72 656c 6174 696f 6e73 6869 7073 2f65  /relationships/e
-000000f0: 7874 656e 6465 642d 7072 6f70 6572 7469  xtended-properti
-00000100: 6573 2220 5461 7267 6574 3d22 646f 6350  es" Target="docP
-00000110: 726f 7073 2f61 7070 2e78 6d6c 222f 3e3c  rops/app.xml"/><
-00000120: 5265 6c61 7469 6f6e 7368 6970 2049 643d  Relationship Id=
-00000130: 2272 4964 3222 2054 7970 653d 2268 7474  "rId2" Type="htt
-00000140: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
-00000150: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f70  xmlformats.org/p
-00000160: 6163 6b61 6765 2f32 3030 362f 7265 6c61  ackage/2006/rela
-00000170: 7469 6f6e 7368 6970 732f 6d65 7461 6461  tionships/metada
-00000180: 7461 2f63 6f72 652d 7072 6f70 6572 7469  ta/core-properti
-00000190: 6573 2220 5461 7267 6574 3d22 646f 6350  es" Target="docP
-000001a0: 726f 7073 2f63 6f72 652e 786d 6c22 2f3e  rops/core.xml"/>
-000001b0: 3c52 656c 6174 696f 6e73 6869 7020 4964  <Relationship Id
-000001c0: 3d22 7249 6431 2220 5479 7065 3d22 6874  ="rId1" Type="ht
-000001d0: 7470 3a2f 2f73 6368 656d 6173 2e6f 7065  tp://schemas.ope
-000001e0: 6e78 6d6c 666f 726d 6174 732e 6f72 672f  nxmlformats.org/
-000001f0: 6f66 6669 6365 446f 6375 6d65 6e74 2f32  officeDocument/2
-00000200: 3030 362f 7265 6c61 7469 6f6e 7368 6970  006/relationship
-00000210: 732f 6f66 6669 6365 446f 6375 6d65 6e74  s/officeDocument
-00000220: 2220 5461 7267 6574 3d22 776f 7264 2f64  " Target="word/d
-00000230: 6f63 756d 656e 742e 786d 6c22 2f3e 3c2f  ocument.xml"/></
-00000240: 5265 6c61 7469 6f6e 7368 6970 733e       Relationships>
+00000030: 2279 6573 223f 3e0a 3c52 656c 6174 696f  "yes"?>.<Relatio
+00000040: 6e73 6869 7073 2078 6d6c 6e73 3d22 6874  nships xmlns="ht
+00000050: 7470 3a2f 2f73 6368 656d 6173 2e6f 7065  tp://schemas.ope
+00000060: 6e78 6d6c 666f 726d 6174 732e 6f72 672f  nxmlformats.org/
+00000070: 7061 636b 6167 652f 3230 3036 2f72 656c  package/2006/rel
+00000080: 6174 696f 6e73 6869 7073 223e 3c52 656c  ationships"><Rel
+00000090: 6174 696f 6e73 6869 7020 4964 3d22 7249  ationship Id="rI
+000000a0: 6433 2220 5479 7065 3d22 6874 7470 3a2f  d3" Type="http:/
+000000b0: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
+000000c0: 666f 726d 6174 732e 6f72 672f 6f66 6669  formats.org/offi
+000000d0: 6365 446f 6375 6d65 6e74 2f32 3030 362f  ceDocument/2006/
+000000e0: 7265 6c61 7469 6f6e 7368 6970 732f 6578  relationships/ex
+000000f0: 7465 6e64 6564 2d70 726f 7065 7274 6965  tended-propertie
+00000100: 7322 2054 6172 6765 743d 2264 6f63 5072  s" Target="docPr
+00000110: 6f70 732f 6170 702e 786d 6c22 2f3e 3c52  ops/app.xml"/><R
+00000120: 656c 6174 696f 6e73 6869 7020 4964 3d22  elationship Id="
+00000130: 7249 6432 2220 5479 7065 3d22 6874 7470  rId2" Type="http
+00000140: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
+00000150: 6d6c 666f 726d 6174 732e 6f72 672f 7061  mlformats.org/pa
+00000160: 636b 6167 652f 3230 3036 2f72 656c 6174  ckage/2006/relat
+00000170: 696f 6e73 6869 7073 2f6d 6574 6164 6174  ionships/metadat
+00000180: 612f 636f 7265 2d70 726f 7065 7274 6965  a/core-propertie
+00000190: 7322 2054 6172 6765 743d 2264 6f63 5072  s" Target="docPr
+000001a0: 6f70 732f 636f 7265 2e78 6d6c 222f 3e3c  ops/core.xml"/><
+000001b0: 5265 6c61 7469 6f6e 7368 6970 2049 643d  Relationship Id=
+000001c0: 2272 4964 3122 2054 7970 653d 2268 7474  "rId1" Type="htt
+000001d0: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
+000001e0: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f6f  xmlformats.org/o
+000001f0: 6666 6963 6544 6f63 756d 656e 742f 3230  fficeDocument/20
+00000200: 3036 2f72 656c 6174 696f 6e73 6869 7073  06/relationships
+00000210: 2f6f 6666 6963 6544 6f63 756d 656e 7422  /officeDocument"
+00000220: 2054 6172 6765 743d 2277 6f72 642f 646f   Target="word/do
+00000230: 6375 6d65 6e74 2e78 6d6c 222f 3e3c 2f52  cument.xml"/></R
+00000240: 656c 6174 696f 6e73 6869 7073 3e         elationships>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/docProps/app.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/docProps/app.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (652), with CRLF line terminators*

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 5072 6f70 6572  "yes"?>..<Proper
-00000040: 7469 6573 2078 6d6c 6e73 3d22 6874 7470  ties xmlns="http
-00000050: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
-00000060: 6d6c 666f 726d 6174 732e 6f72 672f 6f66  mlformats.org/of
-00000070: 6669 6365 446f 6375 6d65 6e74 2f32 3030  ficeDocument/200
-00000080: 362f 6578 7465 6e64 6564 2d70 726f 7065  6/extended-prope
-00000090: 7274 6965 7322 2078 6d6c 6e73 3a76 743d  rties" xmlns:vt=
-000000a0: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-000000b0: 6f70 656e 786d 6c66 6f72 6d61 7473 2e6f  openxmlformats.o
-000000c0: 7267 2f6f 6666 6963 6544 6f63 756d 656e  rg/officeDocumen
-000000d0: 742f 3230 3036 2f64 6f63 5072 6f70 7356  t/2006/docPropsV
-000000e0: 5479 7065 7322 3e3c 5465 6d70 6c61 7465  Types"><Template
-000000f0: 3e4e 6f72 6d61 6c2e 646f 746d 3c2f 5465  >Normal.dotm</Te
-00000100: 6d70 6c61 7465 3e3c 546f 7461 6c54 696d  mplate><TotalTim
-00000110: 653e 303c 2f54 6f74 616c 5469 6d65 3e3c  e>0</TotalTime><
-00000120: 5061 6765 733e 313c 2f50 6167 6573 3e3c  Pages>1</Pages><
-00000130: 576f 7264 733e 303c 2f57 6f72 6473 3e3c  Words>0</Words><
-00000140: 4368 6172 6163 7465 7273 3e30 3c2f 4368  Characters>0</Ch
-00000150: 6172 6163 7465 7273 3e3c 4170 706c 6963  aracters><Applic
-00000160: 6174 696f 6e3e 4d69 6372 6f73 6f66 7420  ation>Microsoft 
-00000170: 4f66 6669 6365 2057 6f72 643c 2f41 7070  Office Word</App
-00000180: 6c69 6361 7469 6f6e 3e3c 446f 6353 6563  lication><DocSec
-00000190: 7572 6974 793e 303c 2f44 6f63 5365 6375  urity>0</DocSecu
-000001a0: 7269 7479 3e3c 4c69 6e65 733e 303c 2f4c  rity><Lines>0</L
-000001b0: 696e 6573 3e3c 5061 7261 6772 6170 6873  ines><Paragraphs
-000001c0: 3e30 3c2f 5061 7261 6772 6170 6873 3e3c  >0</Paragraphs><
-000001d0: 5363 616c 6543 726f 703e 6661 6c73 653c  ScaleCrop>false<
-000001e0: 2f53 6361 6c65 4372 6f70 3e3c 436f 6d70  /ScaleCrop><Comp
-000001f0: 616e 793e 3c2f 436f 6d70 616e 793e 3c4c  any></Company><L
-00000200: 696e 6b73 5570 546f 4461 7465 3e66 616c  inksUpToDate>fal
-00000210: 7365 3c2f 4c69 6e6b 7355 7054 6f44 6174  se</LinksUpToDat
-00000220: 653e 3c43 6861 7261 6374 6572 7357 6974  e><CharactersWit
-00000230: 6853 7061 6365 733e 303c 2f43 6861 7261  hSpaces>0</Chara
-00000240: 6374 6572 7357 6974 6853 7061 6365 733e  ctersWithSpaces>
-00000250: 3c53 6861 7265 6444 6f63 3e66 616c 7365  <SharedDoc>false
-00000260: 3c2f 5368 6172 6564 446f 633e 3c48 7970  </SharedDoc><Hyp
-00000270: 6572 6c69 6e6b 7343 6861 6e67 6564 3e66  erlinksChanged>f
-00000280: 616c 7365 3c2f 4879 7065 726c 696e 6b73  alse</Hyperlinks
-00000290: 4368 616e 6765 643e 3c41 7070 5665 7273  Changed><AppVers
-000002a0: 696f 6e3e 3136 2e30 3030 303c 2f41 7070  ion>16.0000</App
-000002b0: 5665 7273 696f 6e3e 3c2f 5072 6f70 6572  Version></Proper
-000002c0: 7469 6573 3e                             ties>
+00000030: 2279 6573 223f 3e0a 3c50 726f 7065 7274  "yes"?>.<Propert
+00000040: 6965 7320 786d 6c6e 733d 2268 7474 703a  ies xmlns="http:
+00000050: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
+00000060: 6c66 6f72 6d61 7473 2e6f 7267 2f6f 6666  lformats.org/off
+00000070: 6963 6544 6f63 756d 656e 742f 3230 3036  iceDocument/2006
+00000080: 2f65 7874 656e 6465 642d 7072 6f70 6572  /extended-proper
+00000090: 7469 6573 2220 786d 6c6e 733a 7674 3d22  ties" xmlns:vt="
+000000a0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6f  http://schemas.o
+000000b0: 7065 6e78 6d6c 666f 726d 6174 732e 6f72  penxmlformats.or
+000000c0: 672f 6f66 6669 6365 446f 6375 6d65 6e74  g/officeDocument
+000000d0: 2f32 3030 362f 646f 6350 726f 7073 5654  /2006/docPropsVT
+000000e0: 7970 6573 223e 3c54 656d 706c 6174 653e  ypes"><Template>
+000000f0: 4e6f 726d 616c 2e64 6f74 6d3c 2f54 656d  Normal.dotm</Tem
+00000100: 706c 6174 653e 3c54 6f74 616c 5469 6d65  plate><TotalTime
+00000110: 3e30 3c2f 546f 7461 6c54 696d 653e 3c50  >0</TotalTime><P
+00000120: 6167 6573 3e31 3c2f 5061 6765 733e 3c57  ages>1</Pages><W
+00000130: 6f72 6473 3e30 3c2f 576f 7264 733e 3c43  ords>0</Words><C
+00000140: 6861 7261 6374 6572 733e 303c 2f43 6861  haracters>0</Cha
+00000150: 7261 6374 6572 733e 3c41 7070 6c69 6361  racters><Applica
+00000160: 7469 6f6e 3e4d 6963 726f 736f 6674 204f  tion>Microsoft O
+00000170: 6666 6963 6520 576f 7264 3c2f 4170 706c  ffice Word</Appl
+00000180: 6963 6174 696f 6e3e 3c44 6f63 5365 6375  ication><DocSecu
+00000190: 7269 7479 3e30 3c2f 446f 6353 6563 7572  rity>0</DocSecur
+000001a0: 6974 793e 3c4c 696e 6573 3e30 3c2f 4c69  ity><Lines>0</Li
+000001b0: 6e65 733e 3c50 6172 6167 7261 7068 733e  nes><Paragraphs>
+000001c0: 303c 2f50 6172 6167 7261 7068 733e 3c53  0</Paragraphs><S
+000001d0: 6361 6c65 4372 6f70 3e66 616c 7365 3c2f  caleCrop>false</
+000001e0: 5363 616c 6543 726f 703e 3c43 6f6d 7061  ScaleCrop><Compa
+000001f0: 6e79 3e3c 2f43 6f6d 7061 6e79 3e3c 4c69  ny></Company><Li
+00000200: 6e6b 7355 7054 6f44 6174 653e 6661 6c73  nksUpToDate>fals
+00000210: 653c 2f4c 696e 6b73 5570 546f 4461 7465  e</LinksUpToDate
+00000220: 3e3c 4368 6172 6163 7465 7273 5769 7468  ><CharactersWith
+00000230: 5370 6163 6573 3e30 3c2f 4368 6172 6163  Spaces>0</Charac
+00000240: 7465 7273 5769 7468 5370 6163 6573 3e3c  tersWithSpaces><
+00000250: 5368 6172 6564 446f 633e 6661 6c73 653c  SharedDoc>false<
+00000260: 2f53 6861 7265 6444 6f63 3e3c 4879 7065  /SharedDoc><Hype
+00000270: 726c 696e 6b73 4368 616e 6765 643e 6661  rlinksChanged>fa
+00000280: 6c73 653c 2f48 7970 6572 6c69 6e6b 7343  lse</HyperlinksC
+00000290: 6861 6e67 6564 3e3c 4170 7056 6572 7369  hanged><AppVersi
+000002a0: 6f6e 3e31 362e 3030 3030 3c2f 4170 7056  on>16.0000</AppV
+000002b0: 6572 7369 6f6e 3e3c 2f50 726f 7065 7274  ersion></Propert
+000002c0: 6965 733e                                ies>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/docProps/core.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/docProps/core.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (670), with CRLF line terminators*

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 6370 3a63 6f72  "yes"?>..<cp:cor
-00000040: 6550 726f 7065 7274 6965 7320 786d 6c6e  eProperties xmln
-00000050: 733a 6370 3d22 6874 7470 3a2f 2f73 6368  s:cp="http://sch
-00000060: 656d 6173 2e6f 7065 6e78 6d6c 666f 726d  emas.openxmlform
-00000070: 6174 732e 6f72 672f 7061 636b 6167 652f  ats.org/package/
-00000080: 3230 3036 2f6d 6574 6164 6174 612f 636f  2006/metadata/co
-00000090: 7265 2d70 726f 7065 7274 6965 7322 2078  re-properties" x
-000000a0: 6d6c 6e73 3a64 633d 2268 7474 703a 2f2f  mlns:dc="http://
-000000b0: 7075 726c 2e6f 7267 2f64 632f 656c 656d  purl.org/dc/elem
-000000c0: 656e 7473 2f31 2e31 2f22 2078 6d6c 6e73  ents/1.1/" xmlns
-000000d0: 3a64 6374 6572 6d73 3d22 6874 7470 3a2f  :dcterms="http:/
-000000e0: 2f70 7572 6c2e 6f72 672f 6463 2f74 6572  /purl.org/dc/ter
-000000f0: 6d73 2f22 2078 6d6c 6e73 3a64 636d 6974  ms/" xmlns:dcmit
-00000100: 7970 653d 2268 7474 703a 2f2f 7075 726c  ype="http://purl
-00000110: 2e6f 7267 2f64 632f 6463 6d69 7479 7065  .org/dc/dcmitype
-00000120: 2f22 2078 6d6c 6e73 3a78 7369 3d22 6874  /" xmlns:xsi="ht
-00000130: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00000140: 3230 3031 2f58 4d4c 5363 6865 6d61 2d69  2001/XMLSchema-i
-00000150: 6e73 7461 6e63 6522 3e3c 6463 3a74 6974  nstance"><dc:tit
-00000160: 6c65 3e3c 2f64 633a 7469 746c 653e 3c64  le></dc:title><d
-00000170: 633a 7375 626a 6563 743e 3c2f 6463 3a73  c:subject></dc:s
-00000180: 7562 6a65 6374 3e3c 6463 3a63 7265 6174  ubject><dc:creat
-00000190: 6f72 3e3c 2f64 633a 6372 6561 746f 723e  or></dc:creator>
-000001a0: 3c63 703a 6b65 7977 6f72 6473 3e3c 2f63  <cp:keywords></c
-000001b0: 703a 6b65 7977 6f72 6473 3e3c 6463 3a64  p:keywords><dc:d
-000001c0: 6573 6372 6970 7469 6f6e 3e3c 2f64 633a  escription></dc:
-000001d0: 6465 7363 7269 7074 696f 6e3e 3c63 703a  description><cp:
-000001e0: 6c61 7374 4d6f 6469 6669 6564 4279 3e3c  lastModifiedBy><
-000001f0: 2f63 703a 6c61 7374 4d6f 6469 6669 6564  /cp:lastModified
-00000200: 4279 3e3c 6370 3a72 6576 6973 696f 6e3e  By><cp:revision>
-00000210: 313c 2f63 703a 7265 7669 7369 6f6e 3e3c  1</cp:revision><
-00000220: 6463 7465 726d 733a 6372 6561 7465 6420  dcterms:created 
-00000230: 7873 693a 7479 7065 3d22 6463 7465 726d  xsi:type="dcterm
-00000240: 733a 5733 4344 5446 223e 3230 3232 2d31  s:W3CDTF">2022-1
-00000250: 322d 3035 5431 303a 3436 3a30 305a 3c2f  2-05T10:46:00Z</
-00000260: 6463 7465 726d 733a 6372 6561 7465 643e  dcterms:created>
-00000270: 3c64 6374 6572 6d73 3a6d 6f64 6966 6965  <dcterms:modifie
-00000280: 6420 7873 693a 7479 7065 3d22 6463 7465  d xsi:type="dcte
-00000290: 726d 733a 5733 4344 5446 223e 3230 3232  rms:W3CDTF">2022
-000002a0: 2d31 322d 3035 5431 303a 3436 3a30 305a  -12-05T10:46:00Z
-000002b0: 3c2f 6463 7465 726d 733a 6d6f 6469 6669  </dcterms:modifi
-000002c0: 6564 3e3c 2f63 703a 636f 7265 5072 6f70  ed></cp:coreProp
-000002d0: 6572 7469 6573 3e                        erties>
+00000030: 2279 6573 223f 3e0a 3c63 703a 636f 7265  "yes"?>.<cp:core
+00000040: 5072 6f70 6572 7469 6573 2078 6d6c 6e73  Properties xmlns
+00000050: 3a63 703d 2268 7474 703a 2f2f 7363 6865  :cp="http://sche
+00000060: 6d61 732e 6f70 656e 786d 6c66 6f72 6d61  mas.openxmlforma
+00000070: 7473 2e6f 7267 2f70 6163 6b61 6765 2f32  ts.org/package/2
+00000080: 3030 362f 6d65 7461 6461 7461 2f63 6f72  006/metadata/cor
+00000090: 652d 7072 6f70 6572 7469 6573 2220 786d  e-properties" xm
+000000a0: 6c6e 733a 6463 3d22 6874 7470 3a2f 2f70  lns:dc="http://p
+000000b0: 7572 6c2e 6f72 672f 6463 2f65 6c65 6d65  url.org/dc/eleme
+000000c0: 6e74 732f 312e 312f 2220 786d 6c6e 733a  nts/1.1/" xmlns:
+000000d0: 6463 7465 726d 733d 2268 7474 703a 2f2f  dcterms="http://
+000000e0: 7075 726c 2e6f 7267 2f64 632f 7465 726d  purl.org/dc/term
+000000f0: 732f 2220 786d 6c6e 733a 6463 6d69 7479  s/" xmlns:dcmity
+00000100: 7065 3d22 6874 7470 3a2f 2f70 7572 6c2e  pe="http://purl.
+00000110: 6f72 672f 6463 2f64 636d 6974 7970 652f  org/dc/dcmitype/
+00000120: 2220 786d 6c6e 733a 7873 693d 2268 7474  " xmlns:xsi="htt
+00000130: 703a 2f2f 7777 772e 7733 2e6f 7267 2f32  p://www.w3.org/2
+00000140: 3030 312f 584d 4c53 6368 656d 612d 696e  001/XMLSchema-in
+00000150: 7374 616e 6365 223e 3c64 633a 7469 746c  stance"><dc:titl
+00000160: 653e 3c2f 6463 3a74 6974 6c65 3e3c 6463  e></dc:title><dc
+00000170: 3a73 7562 6a65 6374 3e3c 2f64 633a 7375  :subject></dc:su
+00000180: 626a 6563 743e 3c64 633a 6372 6561 746f  bject><dc:creato
+00000190: 723e 3c2f 6463 3a63 7265 6174 6f72 3e3c  r></dc:creator><
+000001a0: 6370 3a6b 6579 776f 7264 733e 3c2f 6370  cp:keywords></cp
+000001b0: 3a6b 6579 776f 7264 733e 3c64 633a 6465  :keywords><dc:de
+000001c0: 7363 7269 7074 696f 6e3e 3c2f 6463 3a64  scription></dc:d
+000001d0: 6573 6372 6970 7469 6f6e 3e3c 6370 3a6c  escription><cp:l
+000001e0: 6173 744d 6f64 6966 6965 6442 793e 3c2f  astModifiedBy></
+000001f0: 6370 3a6c 6173 744d 6f64 6966 6965 6442  cp:lastModifiedB
+00000200: 793e 3c63 703a 7265 7669 7369 6f6e 3e31  y><cp:revision>1
+00000210: 3c2f 6370 3a72 6576 6973 696f 6e3e 3c64  </cp:revision><d
+00000220: 6374 6572 6d73 3a63 7265 6174 6564 2078  cterms:created x
+00000230: 7369 3a74 7970 653d 2264 6374 6572 6d73  si:type="dcterms
+00000240: 3a57 3343 4454 4622 3e32 3032 322d 3132  :W3CDTF">2022-12
+00000250: 2d30 3554 3130 3a34 363a 3030 5a3c 2f64  -05T10:46:00Z</d
+00000260: 6374 6572 6d73 3a63 7265 6174 6564 3e3c  cterms:created><
+00000270: 6463 7465 726d 733a 6d6f 6469 6669 6564  dcterms:modified
+00000280: 2078 7369 3a74 7970 653d 2264 6374 6572   xsi:type="dcter
+00000290: 6d73 3a57 3343 4454 4622 3e32 3032 322d  ms:W3CDTF">2022-
+000002a0: 3132 2d30 3554 3130 3a34 363a 3030 5a3c  12-05T10:46:00Z<
+000002b0: 2f64 6374 6572 6d73 3a6d 6f64 6966 6965  /dcterms:modifie
+000002c0: 643e 3c2f 6370 3a63 6f72 6550 726f 7065  d></cp:corePrope
+000002d0: 7274 6965 733e                           rties>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/_rels/document.xml.rels` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/_rels/document.xml.rels`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (893), with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 5265 6c61 7469  "yes"?>..<Relati
-00000040: 6f6e 7368 6970 7320 786d 6c6e 733d 2268  onships xmlns="h
-00000050: 7474 703a 2f2f 7363 6865 6d61 732e 6f70  ttp://schemas.op
-00000060: 656e 786d 6c66 6f72 6d61 7473 2e6f 7267  enxmlformats.org
-00000070: 2f70 6163 6b61 6765 2f32 3030 362f 7265  /package/2006/re
-00000080: 6c61 7469 6f6e 7368 6970 7322 3e3c 5265  lationships"><Re
-00000090: 6c61 7469 6f6e 7368 6970 2049 643d 2272  lationship Id="r
-000000a0: 4964 3322 2054 7970 653d 2268 7474 703a  Id3" Type="http:
-000000b0: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
-000000c0: 6c66 6f72 6d61 7473 2e6f 7267 2f6f 6666  lformats.org/off
-000000d0: 6963 6544 6f63 756d 656e 742f 3230 3036  iceDocument/2006
-000000e0: 2f72 656c 6174 696f 6e73 6869 7073 2f73  /relationships/s
-000000f0: 6574 7469 6e67 7322 2054 6172 6765 743d  ettings" Target=
-00000100: 2273 6574 7469 6e67 732e 786d 6c22 2f3e  "settings.xml"/>
-00000110: 3c52 656c 6174 696f 6e73 6869 7020 4964  <Relationship Id
-00000120: 3d22 7249 6432 2220 5479 7065 3d22 6874  ="rId2" Type="ht
-00000130: 7470 3a2f 2f73 6368 656d 6173 2e6f 7065  tp://schemas.ope
-00000140: 6e78 6d6c 666f 726d 6174 732e 6f72 672f  nxmlformats.org/
-00000150: 6f66 6669 6365 446f 6375 6d65 6e74 2f32  officeDocument/2
-00000160: 3030 362f 7265 6c61 7469 6f6e 7368 6970  006/relationship
-00000170: 732f 7374 796c 6573 2220 5461 7267 6574  s/styles" Target
-00000180: 3d22 7374 796c 6573 2e78 6d6c 222f 3e3c  ="styles.xml"/><
-00000190: 5265 6c61 7469 6f6e 7368 6970 2049 643d  Relationship Id=
-000001a0: 2272 4964 3122 2054 7970 653d 2268 7474  "rId1" Type="htt
-000001b0: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
-000001c0: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f6f  xmlformats.org/o
-000001d0: 6666 6963 6544 6f63 756d 656e 742f 3230  fficeDocument/20
-000001e0: 3036 2f72 656c 6174 696f 6e73 6869 7073  06/relationships
-000001f0: 2f6e 756d 6265 7269 6e67 2220 5461 7267  /numbering" Targ
-00000200: 6574 3d22 6e75 6d62 6572 696e 672e 786d  et="numbering.xm
-00000210: 6c22 2f3e 3c52 656c 6174 696f 6e73 6869  l"/><Relationshi
-00000220: 7020 4964 3d22 7249 6436 2220 5479 7065  p Id="rId6" Type
-00000230: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000240: 2e6f 7065 6e78 6d6c 666f 726d 6174 732e  .openxmlformats.
-00000250: 6f72 672f 6f66 6669 6365 446f 6375 6d65  org/officeDocume
-00000260: 6e74 2f32 3030 362f 7265 6c61 7469 6f6e  nt/2006/relation
-00000270: 7368 6970 732f 7468 656d 6522 2054 6172  ships/theme" Tar
-00000280: 6765 743d 2274 6865 6d65 2f74 6865 6d65  get="theme/theme
-00000290: 312e 786d 6c22 2f3e 3c52 656c 6174 696f  1.xml"/><Relatio
-000002a0: 6e73 6869 7020 4964 3d22 7249 6435 2220  nship Id="rId5" 
-000002b0: 5479 7065 3d22 6874 7470 3a2f 2f73 6368  Type="http://sch
-000002c0: 656d 6173 2e6f 7065 6e78 6d6c 666f 726d  emas.openxmlform
-000002d0: 6174 732e 6f72 672f 6f66 6669 6365 446f  ats.org/officeDo
-000002e0: 6375 6d65 6e74 2f32 3030 362f 7265 6c61  cument/2006/rela
-000002f0: 7469 6f6e 7368 6970 732f 666f 6e74 5461  tionships/fontTa
-00000300: 626c 6522 2054 6172 6765 743d 2266 6f6e  ble" Target="fon
-00000310: 7454 6162 6c65 2e78 6d6c 222f 3e3c 5265  tTable.xml"/><Re
-00000320: 6c61 7469 6f6e 7368 6970 2049 643d 2272  lationship Id="r
-00000330: 4964 3422 2054 7970 653d 2268 7474 703a  Id4" Type="http:
-00000340: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
-00000350: 6c66 6f72 6d61 7473 2e6f 7267 2f6f 6666  lformats.org/off
-00000360: 6963 6544 6f63 756d 656e 742f 3230 3036  iceDocument/2006
-00000370: 2f72 656c 6174 696f 6e73 6869 7073 2f77  /relationships/w
-00000380: 6562 5365 7474 696e 6773 2220 5461 7267  ebSettings" Targ
-00000390: 6574 3d22 7765 6253 6574 7469 6e67 732e  et="webSettings.
-000003a0: 786d 6c22 2f3e 3c2f 5265 6c61 7469 6f6e  xml"/></Relation
-000003b0: 7368 6970 733e                           ships>
+00000030: 2279 6573 223f 3e0a 3c52 656c 6174 696f  "yes"?>.<Relatio
+00000040: 6e73 6869 7073 2078 6d6c 6e73 3d22 6874  nships xmlns="ht
+00000050: 7470 3a2f 2f73 6368 656d 6173 2e6f 7065  tp://schemas.ope
+00000060: 6e78 6d6c 666f 726d 6174 732e 6f72 672f  nxmlformats.org/
+00000070: 7061 636b 6167 652f 3230 3036 2f72 656c  package/2006/rel
+00000080: 6174 696f 6e73 6869 7073 223e 3c52 656c  ationships"><Rel
+00000090: 6174 696f 6e73 6869 7020 4964 3d22 7249  ationship Id="rI
+000000a0: 6433 2220 5479 7065 3d22 6874 7470 3a2f  d3" Type="http:/
+000000b0: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
+000000c0: 666f 726d 6174 732e 6f72 672f 6f66 6669  formats.org/offi
+000000d0: 6365 446f 6375 6d65 6e74 2f32 3030 362f  ceDocument/2006/
+000000e0: 7265 6c61 7469 6f6e 7368 6970 732f 7365  relationships/se
+000000f0: 7474 696e 6773 2220 5461 7267 6574 3d22  ttings" Target="
+00000100: 7365 7474 696e 6773 2e78 6d6c 222f 3e3c  settings.xml"/><
+00000110: 5265 6c61 7469 6f6e 7368 6970 2049 643d  Relationship Id=
+00000120: 2272 4964 3222 2054 7970 653d 2268 7474  "rId2" Type="htt
+00000130: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
+00000140: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f6f  xmlformats.org/o
+00000150: 6666 6963 6544 6f63 756d 656e 742f 3230  fficeDocument/20
+00000160: 3036 2f72 656c 6174 696f 6e73 6869 7073  06/relationships
+00000170: 2f73 7479 6c65 7322 2054 6172 6765 743d  /styles" Target=
+00000180: 2273 7479 6c65 732e 786d 6c22 2f3e 3c52  "styles.xml"/><R
+00000190: 656c 6174 696f 6e73 6869 7020 4964 3d22  elationship Id="
+000001a0: 7249 6431 2220 5479 7065 3d22 6874 7470  rId1" Type="http
+000001b0: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
+000001c0: 6d6c 666f 726d 6174 732e 6f72 672f 6f66  mlformats.org/of
+000001d0: 6669 6365 446f 6375 6d65 6e74 2f32 3030  ficeDocument/200
+000001e0: 362f 7265 6c61 7469 6f6e 7368 6970 732f  6/relationships/
+000001f0: 6e75 6d62 6572 696e 6722 2054 6172 6765  numbering" Targe
+00000200: 743d 226e 756d 6265 7269 6e67 2e78 6d6c  t="numbering.xml
+00000210: 222f 3e3c 5265 6c61 7469 6f6e 7368 6970  "/><Relationship
+00000220: 2049 643d 2272 4964 3622 2054 7970 653d   Id="rId6" Type=
+00000230: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+00000240: 6f70 656e 786d 6c66 6f72 6d61 7473 2e6f  openxmlformats.o
+00000250: 7267 2f6f 6666 6963 6544 6f63 756d 656e  rg/officeDocumen
+00000260: 742f 3230 3036 2f72 656c 6174 696f 6e73  t/2006/relations
+00000270: 6869 7073 2f74 6865 6d65 2220 5461 7267  hips/theme" Targ
+00000280: 6574 3d22 7468 656d 652f 7468 656d 6531  et="theme/theme1
+00000290: 2e78 6d6c 222f 3e3c 5265 6c61 7469 6f6e  .xml"/><Relation
+000002a0: 7368 6970 2049 643d 2272 4964 3522 2054  ship Id="rId5" T
+000002b0: 7970 653d 2268 7474 703a 2f2f 7363 6865  ype="http://sche
+000002c0: 6d61 732e 6f70 656e 786d 6c66 6f72 6d61  mas.openxmlforma
+000002d0: 7473 2e6f 7267 2f6f 6666 6963 6544 6f63  ts.org/officeDoc
+000002e0: 756d 656e 742f 3230 3036 2f72 656c 6174  ument/2006/relat
+000002f0: 696f 6e73 6869 7073 2f66 6f6e 7454 6162  ionships/fontTab
+00000300: 6c65 2220 5461 7267 6574 3d22 666f 6e74  le" Target="font
+00000310: 5461 626c 652e 786d 6c22 2f3e 3c52 656c  Table.xml"/><Rel
+00000320: 6174 696f 6e73 6869 7020 4964 3d22 7249  ationship Id="rI
+00000330: 6434 2220 5479 7065 3d22 6874 7470 3a2f  d4" Type="http:/
+00000340: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
+00000350: 666f 726d 6174 732e 6f72 672f 6f66 6669  formats.org/offi
+00000360: 6365 446f 6375 6d65 6e74 2f32 3030 362f  ceDocument/2006/
+00000370: 7265 6c61 7469 6f6e 7368 6970 732f 7765  relationships/we
+00000380: 6253 6574 7469 6e67 7322 2054 6172 6765  bSettings" Targe
+00000390: 743d 2277 6562 5365 7474 696e 6773 2e78  t="webSettings.x
+000003a0: 6d6c 222f 3e3c 2f52 656c 6174 696f 6e73  ml"/></Relations
+000003b0: 6869 7073 3e                             hips>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/document.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/document.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (2813), with CRLF line terminators*

 * *Files 1% similar despite different names*

```diff
@@ -1,180 +1,180 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 773a 646f 6375  "yes"?>..<w:docu
-00000040: 6d65 6e74 2078 6d6c 6e73 3a77 7063 3d22  ment xmlns:wpc="
-00000050: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
-00000060: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
-00000070: 6963 652f 776f 7264 2f32 3031 302f 776f  ice/word/2010/wo
-00000080: 7264 7072 6f63 6573 7369 6e67 4361 6e76  rdprocessingCanv
-00000090: 6173 2220 786d 6c6e 733a 6378 3d22 6874  as" xmlns:cx="ht
-000000a0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
-000000b0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
-000000c0: 652f 6472 6177 696e 672f 3230 3134 2f63  e/drawing/2014/c
-000000d0: 6861 7274 6578 2220 786d 6c6e 733a 6378  hartex" xmlns:cx
-000000e0: 313d 2268 7474 703a 2f2f 7363 6865 6d61  1="http://schema
-000000f0: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
-00000100: 6f66 6669 6365 2f64 7261 7769 6e67 2f32  office/drawing/2
-00000110: 3031 352f 392f 382f 6368 6172 7465 7822  015/9/8/chartex"
-00000120: 2078 6d6c 6e73 3a63 7832 3d22 6874 7470   xmlns:cx2="http
-00000130: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-00000140: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-00000150: 6472 6177 696e 672f 3230 3135 2f31 302f  drawing/2015/10/
-00000160: 3231 2f63 6861 7274 6578 2220 786d 6c6e  21/chartex" xmln
-00000170: 733a 6378 333d 2268 7474 703a 2f2f 7363  s:cx3="http://sc
-00000180: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
-00000190: 636f 6d2f 6f66 6669 6365 2f64 7261 7769  com/office/drawi
-000001a0: 6e67 2f32 3031 362f 352f 392f 6368 6172  ng/2016/5/9/char
-000001b0: 7465 7822 2078 6d6c 6e73 3a63 7834 3d22  tex" xmlns:cx4="
-000001c0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
-000001d0: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
-000001e0: 6963 652f 6472 6177 696e 672f 3230 3136  ice/drawing/2016
-000001f0: 2f35 2f31 302f 6368 6172 7465 7822 2078  /5/10/chartex" x
-00000200: 6d6c 6e73 3a63 7835 3d22 6874 7470 3a2f  mlns:cx5="http:/
-00000210: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
-00000220: 6674 2e63 6f6d 2f6f 6666 6963 652f 6472  ft.com/office/dr
-00000230: 6177 696e 672f 3230 3136 2f35 2f31 312f  awing/2016/5/11/
-00000240: 6368 6172 7465 7822 2078 6d6c 6e73 3a63  chartex" xmlns:c
-00000250: 7836 3d22 6874 7470 3a2f 2f73 6368 656d  x6="http://schem
-00000260: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-00000270: 2f6f 6666 6963 652f 6472 6177 696e 672f  /office/drawing/
-00000280: 3230 3136 2f35 2f31 322f 6368 6172 7465  2016/5/12/charte
-00000290: 7822 2078 6d6c 6e73 3a63 7837 3d22 6874  x" xmlns:cx7="ht
-000002a0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
-000002b0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
-000002c0: 652f 6472 6177 696e 672f 3230 3136 2f35  e/drawing/2016/5
-000002d0: 2f31 332f 6368 6172 7465 7822 2078 6d6c  /13/chartex" xml
-000002e0: 6e73 3a63 7838 3d22 6874 7470 3a2f 2f73  ns:cx8="http://s
-000002f0: 6368 656d 6173 2e6d 6963 726f 736f 6674  chemas.microsoft
-00000300: 2e63 6f6d 2f6f 6666 6963 652f 6472 6177  .com/office/draw
-00000310: 696e 672f 3230 3136 2f35 2f31 342f 6368  ing/2016/5/14/ch
-00000320: 6172 7465 7822 2078 6d6c 6e73 3a6d 633d  artex" xmlns:mc=
-00000330: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-00000340: 6f70 656e 786d 6c66 6f72 6d61 7473 2e6f  openxmlformats.o
-00000350: 7267 2f6d 6172 6b75 702d 636f 6d70 6174  rg/markup-compat
-00000360: 6962 696c 6974 792f 3230 3036 2220 786d  ibility/2006" xm
-00000370: 6c6e 733a 6169 6e6b 3d22 6874 7470 3a2f  lns:aink="http:/
-00000380: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
-00000390: 6674 2e63 6f6d 2f6f 6666 6963 652f 6472  ft.com/office/dr
-000003a0: 6177 696e 672f 3230 3136 2f69 6e6b 2220  awing/2016/ink" 
-000003b0: 786d 6c6e 733a 616d 3364 3d22 6874 7470  xmlns:am3d="http
-000003c0: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-000003d0: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-000003e0: 6472 6177 696e 672f 3230 3137 2f6d 6f64  drawing/2017/mod
-000003f0: 656c 3364 2220 786d 6c6e 733a 6f3d 2275  el3d" xmlns:o="u
-00000400: 726e 3a73 6368 656d 6173 2d6d 6963 726f  rn:schemas-micro
-00000410: 736f 6674 2d63 6f6d 3a6f 6666 6963 653a  soft-com:office:
-00000420: 6f66 6669 6365 2220 786d 6c6e 733a 6f65  office" xmlns:oe
-00000430: 6c3d 2268 7474 703a 2f2f 7363 6865 6d61  l="http://schema
-00000440: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
-00000450: 6f66 6669 6365 2f32 3031 392f 6578 746c  office/2019/extl
-00000460: 7374 2220 786d 6c6e 733a 723d 2268 7474  st" xmlns:r="htt
-00000470: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
-00000480: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f6f  xmlformats.org/o
-00000490: 6666 6963 6544 6f63 756d 656e 742f 3230  fficeDocument/20
-000004a0: 3036 2f72 656c 6174 696f 6e73 6869 7073  06/relationships
-000004b0: 2220 786d 6c6e 733a 6d3d 2268 7474 703a  " xmlns:m="http:
-000004c0: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
-000004d0: 6c66 6f72 6d61 7473 2e6f 7267 2f6f 6666  lformats.org/off
-000004e0: 6963 6544 6f63 756d 656e 742f 3230 3036  iceDocument/2006
-000004f0: 2f6d 6174 6822 2078 6d6c 6e73 3a76 3d22  /math" xmlns:v="
-00000500: 7572 6e3a 7363 6865 6d61 732d 6d69 6372  urn:schemas-micr
-00000510: 6f73 6f66 742d 636f 6d3a 766d 6c22 2078  osoft-com:vml" x
-00000520: 6d6c 6e73 3a77 7031 343d 2268 7474 703a  mlns:wp14="http:
-00000530: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
-00000540: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
-00000550: 6f72 642f 3230 3130 2f77 6f72 6470 726f  ord/2010/wordpro
-00000560: 6365 7373 696e 6744 7261 7769 6e67 2220  cessingDrawing" 
-00000570: 786d 6c6e 733a 7770 3d22 6874 7470 3a2f  xmlns:wp="http:/
-00000580: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
-00000590: 666f 726d 6174 732e 6f72 672f 6472 6177  formats.org/draw
-000005a0: 696e 676d 6c2f 3230 3036 2f77 6f72 6470  ingml/2006/wordp
-000005b0: 726f 6365 7373 696e 6744 7261 7769 6e67  rocessingDrawing
-000005c0: 2220 786d 6c6e 733a 7731 303d 2275 726e  " xmlns:w10="urn
-000005d0: 3a73 6368 656d 6173 2d6d 6963 726f 736f  :schemas-microso
-000005e0: 6674 2d63 6f6d 3a6f 6666 6963 653a 776f  ft-com:office:wo
-000005f0: 7264 2220 786d 6c6e 733a 773d 2268 7474  rd" xmlns:w="htt
-00000600: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
-00000610: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f77  xmlformats.org/w
-00000620: 6f72 6470 726f 6365 7373 696e 676d 6c2f  ordprocessingml/
-00000630: 3230 3036 2f6d 6169 6e22 2078 6d6c 6e73  2006/main" xmlns
-00000640: 3a77 3134 3d22 6874 7470 3a2f 2f73 6368  :w14="http://sch
-00000650: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
-00000660: 6f6d 2f6f 6666 6963 652f 776f 7264 2f32  om/office/word/2
-00000670: 3031 302f 776f 7264 6d6c 2220 786d 6c6e  010/wordml" xmln
-00000680: 733a 7731 353d 2268 7474 703a 2f2f 7363  s:w15="http://sc
-00000690: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
-000006a0: 636f 6d2f 6f66 6669 6365 2f77 6f72 642f  com/office/word/
-000006b0: 3230 3132 2f77 6f72 646d 6c22 2078 6d6c  2012/wordml" xml
-000006c0: 6e73 3a77 3136 6365 783d 2268 7474 703a  ns:w16cex="http:
-000006d0: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
-000006e0: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
-000006f0: 6f72 642f 3230 3138 2f77 6f72 646d 6c2f  ord/2018/wordml/
-00000700: 6365 7822 2078 6d6c 6e73 3a77 3136 6369  cex" xmlns:w16ci
-00000710: 643d 2268 7474 703a 2f2f 7363 6865 6d61  d="http://schema
-00000720: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
-00000730: 6f66 6669 6365 2f77 6f72 642f 3230 3136  office/word/2016
-00000740: 2f77 6f72 646d 6c2f 6369 6422 2078 6d6c  /wordml/cid" xml
-00000750: 6e73 3a77 3136 3d22 6874 7470 3a2f 2f73  ns:w16="http://s
-00000760: 6368 656d 6173 2e6d 6963 726f 736f 6674  chemas.microsoft
-00000770: 2e63 6f6d 2f6f 6666 6963 652f 776f 7264  .com/office/word
-00000780: 2f32 3031 382f 776f 7264 6d6c 2220 786d  /2018/wordml" xm
-00000790: 6c6e 733a 7731 3673 6474 6468 3d22 6874  lns:w16sdtdh="ht
-000007a0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
-000007b0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
-000007c0: 652f 776f 7264 2f32 3032 302f 776f 7264  e/word/2020/word
-000007d0: 6d6c 2f73 6474 6461 7461 6861 7368 2220  ml/sdtdatahash" 
-000007e0: 786d 6c6e 733a 7731 3673 653d 2268 7474  xmlns:w16se="htt
-000007f0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
-00000800: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
-00000810: 2f77 6f72 642f 3230 3135 2f77 6f72 646d  /word/2015/wordm
-00000820: 6c2f 7379 6d65 7822 2078 6d6c 6e73 3a77  l/symex" xmlns:w
-00000830: 7067 3d22 6874 7470 3a2f 2f73 6368 656d  pg="http://schem
-00000840: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-00000850: 2f6f 6666 6963 652f 776f 7264 2f32 3031  /office/word/201
-00000860: 302f 776f 7264 7072 6f63 6573 7369 6e67  0/wordprocessing
-00000870: 4772 6f75 7022 2078 6d6c 6e73 3a77 7069  Group" xmlns:wpi
-00000880: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000890: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
-000008a0: 6666 6963 652f 776f 7264 2f32 3031 302f  ffice/word/2010/
-000008b0: 776f 7264 7072 6f63 6573 7369 6e67 496e  wordprocessingIn
-000008c0: 6b22 2078 6d6c 6e73 3a77 6e65 3d22 6874  k" xmlns:wne="ht
-000008d0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
-000008e0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
-000008f0: 652f 776f 7264 2f32 3030 362f 776f 7264  e/word/2006/word
-00000900: 6d6c 2220 786d 6c6e 733a 7770 733d 2268  ml" xmlns:wps="h
-00000910: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-00000920: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-00000930: 6365 2f77 6f72 642f 3230 3130 2f77 6f72  ce/word/2010/wor
-00000940: 6470 726f 6365 7373 696e 6753 6861 7065  dprocessingShape
-00000950: 2220 6d63 3a49 676e 6f72 6162 6c65 3d22  " mc:Ignorable="
-00000960: 7731 3420 7731 3520 7731 3673 6520 7731  w14 w15 w16se w1
-00000970: 3663 6964 2077 3136 2077 3136 6365 7820  6cid w16 w16cex 
-00000980: 7731 3673 6474 6468 2077 7031 3422 3e3c  w16sdtdh wp14"><
-00000990: 773a 626f 6479 3e3c 773a 7020 7731 343a  w:body><w:p w14:
-000009a0: 7061 7261 4964 3d22 3636 3536 4533 3330  paraId="6656E330
-000009b0: 2220 7731 343a 7465 7874 4964 3d22 3234  " w14:textId="24
-000009c0: 3042 3146 3335 2220 773a 7273 6964 523d  0B1F35" w:rsidR=
-000009d0: 2230 3044 3732 3535 4122 2077 3a72 7369  "00D7255A" w:rsi
-000009e0: 6452 5072 3d22 3030 3336 3236 4534 2220  dRPr="003626E4" 
-000009f0: 773a 7273 6964 5244 6566 6175 6c74 3d22  w:rsidRDefault="
-00000a00: 3030 4437 3235 3541 2220 773a 7273 6964  00D7255A" w:rsid
-00000a10: 503d 2230 3033 3632 3645 3422 2f3e 3c77  P="003626E4"/><w
-00000a20: 3a73 6563 7450 7220 773a 7273 6964 523d  :sectPr w:rsidR=
-00000a30: 2230 3044 3732 3535 4122 2077 3a72 7369  "00D7255A" w:rsi
-00000a40: 6452 5072 3d22 3030 3336 3236 4534 223e  dRPr="003626E4">
-00000a50: 3c77 3a70 6753 7a20 773a 773d 2231 3139  <w:pgSz w:w="119
-00000a60: 3036 2220 773a 683d 2231 3638 3338 222f  06" w:h="16838"/
-00000a70: 3e3c 773a 7067 4d61 7220 773a 746f 703d  ><w:pgMar w:top=
-00000a80: 2231 3434 3022 2077 3a72 6967 6874 3d22  "1440" w:right="
-00000a90: 3134 3430 2220 773a 626f 7474 6f6d 3d22  1440" w:bottom="
-00000aa0: 3134 3430 2220 773a 6c65 6674 3d22 3134  1440" w:left="14
-00000ab0: 3430 2220 773a 6865 6164 6572 3d22 3730  40" w:header="70
-00000ac0: 3822 2077 3a66 6f6f 7465 723d 2237 3038  8" w:footer="708
-00000ad0: 2220 773a 6775 7474 6572 3d22 3022 2f3e  " w:gutter="0"/>
-00000ae0: 3c77 3a63 6f6c 7320 773a 7370 6163 653d  <w:cols w:space=
-00000af0: 2237 3038 222f 3e3c 773a 646f 6347 7269  "708"/><w:docGri
-00000b00: 6420 773a 6c69 6e65 5069 7463 683d 2233  d w:linePitch="3
-00000b10: 3630 222f 3e3c 2f77 3a73 6563 7450 723e  60"/></w:sectPr>
-00000b20: 3c2f 773a 626f 6479 3e3c 2f77 3a64 6f63  </w:body></w:doc
-00000b30: 756d 656e 743e                           ument>
+00000030: 2279 6573 223f 3e0a 3c77 3a64 6f63 756d  "yes"?>.<w:docum
+00000040: 656e 7420 786d 6c6e 733a 7770 633d 2268  ent xmlns:wpc="h
+00000050: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
+00000060: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
+00000070: 6365 2f77 6f72 642f 3230 3130 2f77 6f72  ce/word/2010/wor
+00000080: 6470 726f 6365 7373 696e 6743 616e 7661  dprocessingCanva
+00000090: 7322 2078 6d6c 6e73 3a63 783d 2268 7474  s" xmlns:cx="htt
+000000a0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
+000000b0: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
+000000c0: 2f64 7261 7769 6e67 2f32 3031 342f 6368  /drawing/2014/ch
+000000d0: 6172 7465 7822 2078 6d6c 6e73 3a63 7831  artex" xmlns:cx1
+000000e0: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
+000000f0: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
+00000100: 6666 6963 652f 6472 6177 696e 672f 3230  ffice/drawing/20
+00000110: 3135 2f39 2f38 2f63 6861 7274 6578 2220  15/9/8/chartex" 
+00000120: 786d 6c6e 733a 6378 323d 2268 7474 703a  xmlns:cx2="http:
+00000130: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+00000140: 6f66 742e 636f 6d2f 6f66 6669 6365 2f64  oft.com/office/d
+00000150: 7261 7769 6e67 2f32 3031 352f 3130 2f32  rawing/2015/10/2
+00000160: 312f 6368 6172 7465 7822 2078 6d6c 6e73  1/chartex" xmlns
+00000170: 3a63 7833 3d22 6874 7470 3a2f 2f73 6368  :cx3="http://sch
+00000180: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
+00000190: 6f6d 2f6f 6666 6963 652f 6472 6177 696e  om/office/drawin
+000001a0: 672f 3230 3136 2f35 2f39 2f63 6861 7274  g/2016/5/9/chart
+000001b0: 6578 2220 786d 6c6e 733a 6378 343d 2268  ex" xmlns:cx4="h
+000001c0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
+000001d0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
+000001e0: 6365 2f64 7261 7769 6e67 2f32 3031 362f  ce/drawing/2016/
+000001f0: 352f 3130 2f63 6861 7274 6578 2220 786d  5/10/chartex" xm
+00000200: 6c6e 733a 6378 353d 2268 7474 703a 2f2f  lns:cx5="http://
+00000210: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
+00000220: 742e 636f 6d2f 6f66 6669 6365 2f64 7261  t.com/office/dra
+00000230: 7769 6e67 2f32 3031 362f 352f 3131 2f63  wing/2016/5/11/c
+00000240: 6861 7274 6578 2220 786d 6c6e 733a 6378  hartex" xmlns:cx
+00000250: 363d 2268 7474 703a 2f2f 7363 6865 6d61  6="http://schema
+00000260: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+00000270: 6f66 6669 6365 2f64 7261 7769 6e67 2f32  office/drawing/2
+00000280: 3031 362f 352f 3132 2f63 6861 7274 6578  016/5/12/chartex
+00000290: 2220 786d 6c6e 733a 6378 373d 2268 7474  " xmlns:cx7="htt
+000002a0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
+000002b0: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
+000002c0: 2f64 7261 7769 6e67 2f32 3031 362f 352f  /drawing/2016/5/
+000002d0: 3133 2f63 6861 7274 6578 2220 786d 6c6e  13/chartex" xmln
+000002e0: 733a 6378 383d 2268 7474 703a 2f2f 7363  s:cx8="http://sc
+000002f0: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
+00000300: 636f 6d2f 6f66 6669 6365 2f64 7261 7769  com/office/drawi
+00000310: 6e67 2f32 3031 362f 352f 3134 2f63 6861  ng/2016/5/14/cha
+00000320: 7274 6578 2220 786d 6c6e 733a 6d63 3d22  rtex" xmlns:mc="
+00000330: 6874 7470 3a2f 2f73 6368 656d 6173 2e6f  http://schemas.o
+00000340: 7065 6e78 6d6c 666f 726d 6174 732e 6f72  penxmlformats.or
+00000350: 672f 6d61 726b 7570 2d63 6f6d 7061 7469  g/markup-compati
+00000360: 6269 6c69 7479 2f32 3030 3622 2078 6d6c  bility/2006" xml
+00000370: 6e73 3a61 696e 6b3d 2268 7474 703a 2f2f  ns:aink="http://
+00000380: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
+00000390: 742e 636f 6d2f 6f66 6669 6365 2f64 7261  t.com/office/dra
+000003a0: 7769 6e67 2f32 3031 362f 696e 6b22 2078  wing/2016/ink" x
+000003b0: 6d6c 6e73 3a61 6d33 643d 2268 7474 703a  mlns:am3d="http:
+000003c0: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+000003d0: 6f66 742e 636f 6d2f 6f66 6669 6365 2f64  oft.com/office/d
+000003e0: 7261 7769 6e67 2f32 3031 372f 6d6f 6465  rawing/2017/mode
+000003f0: 6c33 6422 2078 6d6c 6e73 3a6f 3d22 7572  l3d" xmlns:o="ur
+00000400: 6e3a 7363 6865 6d61 732d 6d69 6372 6f73  n:schemas-micros
+00000410: 6f66 742d 636f 6d3a 6f66 6669 6365 3a6f  oft-com:office:o
+00000420: 6666 6963 6522 2078 6d6c 6e73 3a6f 656c  ffice" xmlns:oel
+00000430: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
+00000440: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
+00000450: 6666 6963 652f 3230 3139 2f65 7874 6c73  ffice/2019/extls
+00000460: 7422 2078 6d6c 6e73 3a72 3d22 6874 7470  t" xmlns:r="http
+00000470: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
+00000480: 6d6c 666f 726d 6174 732e 6f72 672f 6f66  mlformats.org/of
+00000490: 6669 6365 446f 6375 6d65 6e74 2f32 3030  ficeDocument/200
+000004a0: 362f 7265 6c61 7469 6f6e 7368 6970 7322  6/relationships"
+000004b0: 2078 6d6c 6e73 3a6d 3d22 6874 7470 3a2f   xmlns:m="http:/
+000004c0: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
+000004d0: 666f 726d 6174 732e 6f72 672f 6f66 6669  formats.org/offi
+000004e0: 6365 446f 6375 6d65 6e74 2f32 3030 362f  ceDocument/2006/
+000004f0: 6d61 7468 2220 786d 6c6e 733a 763d 2275  math" xmlns:v="u
+00000500: 726e 3a73 6368 656d 6173 2d6d 6963 726f  rn:schemas-micro
+00000510: 736f 6674 2d63 6f6d 3a76 6d6c 2220 786d  soft-com:vml" xm
+00000520: 6c6e 733a 7770 3134 3d22 6874 7470 3a2f  lns:wp14="http:/
+00000530: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
+00000540: 6674 2e63 6f6d 2f6f 6666 6963 652f 776f  ft.com/office/wo
+00000550: 7264 2f32 3031 302f 776f 7264 7072 6f63  rd/2010/wordproc
+00000560: 6573 7369 6e67 4472 6177 696e 6722 2078  essingDrawing" x
+00000570: 6d6c 6e73 3a77 703d 2268 7474 703a 2f2f  mlns:wp="http://
+00000580: 7363 6865 6d61 732e 6f70 656e 786d 6c66  schemas.openxmlf
+00000590: 6f72 6d61 7473 2e6f 7267 2f64 7261 7769  ormats.org/drawi
+000005a0: 6e67 6d6c 2f32 3030 362f 776f 7264 7072  ngml/2006/wordpr
+000005b0: 6f63 6573 7369 6e67 4472 6177 696e 6722  ocessingDrawing"
+000005c0: 2078 6d6c 6e73 3a77 3130 3d22 7572 6e3a   xmlns:w10="urn:
+000005d0: 7363 6865 6d61 732d 6d69 6372 6f73 6f66  schemas-microsof
+000005e0: 742d 636f 6d3a 6f66 6669 6365 3a77 6f72  t-com:office:wor
+000005f0: 6422 2078 6d6c 6e73 3a77 3d22 6874 7470  d" xmlns:w="http
+00000600: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
+00000610: 6d6c 666f 726d 6174 732e 6f72 672f 776f  mlformats.org/wo
+00000620: 7264 7072 6f63 6573 7369 6e67 6d6c 2f32  rdprocessingml/2
+00000630: 3030 362f 6d61 696e 2220 786d 6c6e 733a  006/main" xmlns:
+00000640: 7731 343d 2268 7474 703a 2f2f 7363 6865  w14="http://sche
+00000650: 6d61 732e 6d69 6372 6f73 6f66 742e 636f  mas.microsoft.co
+00000660: 6d2f 6f66 6669 6365 2f77 6f72 642f 3230  m/office/word/20
+00000670: 3130 2f77 6f72 646d 6c22 2078 6d6c 6e73  10/wordml" xmlns
+00000680: 3a77 3135 3d22 6874 7470 3a2f 2f73 6368  :w15="http://sch
+00000690: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
+000006a0: 6f6d 2f6f 6666 6963 652f 776f 7264 2f32  om/office/word/2
+000006b0: 3031 322f 776f 7264 6d6c 2220 786d 6c6e  012/wordml" xmln
+000006c0: 733a 7731 3663 6578 3d22 6874 7470 3a2f  s:w16cex="http:/
+000006d0: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
+000006e0: 6674 2e63 6f6d 2f6f 6666 6963 652f 776f  ft.com/office/wo
+000006f0: 7264 2f32 3031 382f 776f 7264 6d6c 2f63  rd/2018/wordml/c
+00000700: 6578 2220 786d 6c6e 733a 7731 3663 6964  ex" xmlns:w16cid
+00000710: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
+00000720: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
+00000730: 6666 6963 652f 776f 7264 2f32 3031 362f  ffice/word/2016/
+00000740: 776f 7264 6d6c 2f63 6964 2220 786d 6c6e  wordml/cid" xmln
+00000750: 733a 7731 363d 2268 7474 703a 2f2f 7363  s:w16="http://sc
+00000760: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
+00000770: 636f 6d2f 6f66 6669 6365 2f77 6f72 642f  com/office/word/
+00000780: 3230 3138 2f77 6f72 646d 6c22 2078 6d6c  2018/wordml" xml
+00000790: 6e73 3a77 3136 7364 7464 683d 2268 7474  ns:w16sdtdh="htt
+000007a0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
+000007b0: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
+000007c0: 2f77 6f72 642f 3230 3230 2f77 6f72 646d  /word/2020/wordm
+000007d0: 6c2f 7364 7464 6174 6168 6173 6822 2078  l/sdtdatahash" x
+000007e0: 6d6c 6e73 3a77 3136 7365 3d22 6874 7470  mlns:w16se="http
+000007f0: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
+00000800: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
+00000810: 776f 7264 2f32 3031 352f 776f 7264 6d6c  word/2015/wordml
+00000820: 2f73 796d 6578 2220 786d 6c6e 733a 7770  /symex" xmlns:wp
+00000830: 673d 2268 7474 703a 2f2f 7363 6865 6d61  g="http://schema
+00000840: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+00000850: 6f66 6669 6365 2f77 6f72 642f 3230 3130  office/word/2010
+00000860: 2f77 6f72 6470 726f 6365 7373 696e 6747  /wordprocessingG
+00000870: 726f 7570 2220 786d 6c6e 733a 7770 693d  roup" xmlns:wpi=
+00000880: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+00000890: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
+000008a0: 6669 6365 2f77 6f72 642f 3230 3130 2f77  fice/word/2010/w
+000008b0: 6f72 6470 726f 6365 7373 696e 6749 6e6b  ordprocessingInk
+000008c0: 2220 786d 6c6e 733a 776e 653d 2268 7474  " xmlns:wne="htt
+000008d0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
+000008e0: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
+000008f0: 2f77 6f72 642f 3230 3036 2f77 6f72 646d  /word/2006/wordm
+00000900: 6c22 2078 6d6c 6e73 3a77 7073 3d22 6874  l" xmlns:wps="ht
+00000910: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+00000920: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+00000930: 652f 776f 7264 2f32 3031 302f 776f 7264  e/word/2010/word
+00000940: 7072 6f63 6573 7369 6e67 5368 6170 6522  processingShape"
+00000950: 206d 633a 4967 6e6f 7261 626c 653d 2277   mc:Ignorable="w
+00000960: 3134 2077 3135 2077 3136 7365 2077 3136  14 w15 w16se w16
+00000970: 6369 6420 7731 3620 7731 3663 6578 2077  cid w16 w16cex w
+00000980: 3136 7364 7464 6820 7770 3134 223e 3c77  16sdtdh wp14"><w
+00000990: 3a62 6f64 793e 3c77 3a70 2077 3134 3a70  :body><w:p w14:p
+000009a0: 6172 6149 643d 2236 3635 3645 3333 3022  araId="6656E330"
+000009b0: 2077 3134 3a74 6578 7449 643d 2232 3430   w14:textId="240
+000009c0: 4231 4633 3522 2077 3a72 7369 6452 3d22  B1F35" w:rsidR="
+000009d0: 3030 4437 3235 3541 2220 773a 7273 6964  00D7255A" w:rsid
+000009e0: 5250 723d 2230 3033 3632 3645 3422 2077  RPr="003626E4" w
+000009f0: 3a72 7369 6452 4465 6661 756c 743d 2230  :rsidRDefault="0
+00000a00: 3044 3732 3535 4122 2077 3a72 7369 6450  0D7255A" w:rsidP
+00000a10: 3d22 3030 3336 3236 4534 222f 3e3c 773a  ="003626E4"/><w:
+00000a20: 7365 6374 5072 2077 3a72 7369 6452 3d22  sectPr w:rsidR="
+00000a30: 3030 4437 3235 3541 2220 773a 7273 6964  00D7255A" w:rsid
+00000a40: 5250 723d 2230 3033 3632 3645 3422 3e3c  RPr="003626E4"><
+00000a50: 773a 7067 537a 2077 3a77 3d22 3131 3930  w:pgSz w:w="1190
+00000a60: 3622 2077 3a68 3d22 3136 3833 3822 2f3e  6" w:h="16838"/>
+00000a70: 3c77 3a70 674d 6172 2077 3a74 6f70 3d22  <w:pgMar w:top="
+00000a80: 3134 3430 2220 773a 7269 6768 743d 2231  1440" w:right="1
+00000a90: 3434 3022 2077 3a62 6f74 746f 6d3d 2231  440" w:bottom="1
+00000aa0: 3434 3022 2077 3a6c 6566 743d 2231 3434  440" w:left="144
+00000ab0: 3022 2077 3a68 6561 6465 723d 2237 3038  0" w:header="708
+00000ac0: 2220 773a 666f 6f74 6572 3d22 3730 3822  " w:footer="708"
+00000ad0: 2077 3a67 7574 7465 723d 2230 222f 3e3c   w:gutter="0"/><
+00000ae0: 773a 636f 6c73 2077 3a73 7061 6365 3d22  w:cols w:space="
+00000af0: 3730 3822 2f3e 3c77 3a64 6f63 4772 6964  708"/><w:docGrid
+00000b00: 2077 3a6c 696e 6550 6974 6368 3d22 3336   w:linePitch="36
+00000b10: 3022 2f3e 3c2f 773a 7365 6374 5072 3e3c  0"/></w:sectPr><
+00000b20: 2f77 3a62 6f64 793e 3c2f 773a 646f 6375  /w:body></w:docu
+00000b30: 6d65 6e74 3e                             ment>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/fontTable.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/fontTable.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (2666), with CRLF line terminators*

 * *Files 4% similar despite different names*

```diff
@@ -1,171 +1,171 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 773a 666f 6e74  "yes"?>..<w:font
-00000040: 7320 786d 6c6e 733a 6d63 3d22 6874 7470  s xmlns:mc="http
-00000050: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
-00000060: 6d6c 666f 726d 6174 732e 6f72 672f 6d61  mlformats.org/ma
-00000070: 726b 7570 2d63 6f6d 7061 7469 6269 6c69  rkup-compatibili
-00000080: 7479 2f32 3030 3622 2078 6d6c 6e73 3a72  ty/2006" xmlns:r
-00000090: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-000000a0: 2e6f 7065 6e78 6d6c 666f 726d 6174 732e  .openxmlformats.
-000000b0: 6f72 672f 6f66 6669 6365 446f 6375 6d65  org/officeDocume
-000000c0: 6e74 2f32 3030 362f 7265 6c61 7469 6f6e  nt/2006/relation
-000000d0: 7368 6970 7322 2078 6d6c 6e73 3a77 3d22  ships" xmlns:w="
-000000e0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6f  http://schemas.o
-000000f0: 7065 6e78 6d6c 666f 726d 6174 732e 6f72  penxmlformats.or
-00000100: 672f 776f 7264 7072 6f63 6573 7369 6e67  g/wordprocessing
-00000110: 6d6c 2f32 3030 362f 6d61 696e 2220 786d  ml/2006/main" xm
-00000120: 6c6e 733a 7731 343d 2268 7474 703a 2f2f  lns:w14="http://
-00000130: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
-00000140: 742e 636f 6d2f 6f66 6669 6365 2f77 6f72  t.com/office/wor
-00000150: 642f 3230 3130 2f77 6f72 646d 6c22 2078  d/2010/wordml" x
-00000160: 6d6c 6e73 3a77 3135 3d22 6874 7470 3a2f  mlns:w15="http:/
-00000170: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
-00000180: 6674 2e63 6f6d 2f6f 6666 6963 652f 776f  ft.com/office/wo
-00000190: 7264 2f32 3031 322f 776f 7264 6d6c 2220  rd/2012/wordml" 
-000001a0: 786d 6c6e 733a 7731 3663 6578 3d22 6874  xmlns:w16cex="ht
-000001b0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
-000001c0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
-000001d0: 652f 776f 7264 2f32 3031 382f 776f 7264  e/word/2018/word
-000001e0: 6d6c 2f63 6578 2220 786d 6c6e 733a 7731  ml/cex" xmlns:w1
-000001f0: 3663 6964 3d22 6874 7470 3a2f 2f73 6368  6cid="http://sch
-00000200: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
-00000210: 6f6d 2f6f 6666 6963 652f 776f 7264 2f32  om/office/word/2
-00000220: 3031 362f 776f 7264 6d6c 2f63 6964 2220  016/wordml/cid" 
-00000230: 786d 6c6e 733a 7731 363d 2268 7474 703a  xmlns:w16="http:
-00000240: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
-00000250: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
-00000260: 6f72 642f 3230 3138 2f77 6f72 646d 6c22  ord/2018/wordml"
-00000270: 2078 6d6c 6e73 3a77 3136 7364 7464 683d   xmlns:w16sdtdh=
-00000280: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-00000290: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
-000002a0: 6669 6365 2f77 6f72 642f 3230 3230 2f77  fice/word/2020/w
-000002b0: 6f72 646d 6c2f 7364 7464 6174 6168 6173  ordml/sdtdatahas
-000002c0: 6822 2078 6d6c 6e73 3a77 3136 7365 3d22  h" xmlns:w16se="
-000002d0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
-000002e0: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
-000002f0: 6963 652f 776f 7264 2f32 3031 352f 776f  ice/word/2015/wo
-00000300: 7264 6d6c 2f73 796d 6578 2220 6d63 3a49  rdml/symex" mc:I
-00000310: 676e 6f72 6162 6c65 3d22 7731 3420 7731  gnorable="w14 w1
-00000320: 3520 7731 3673 6520 7731 3663 6964 2077  5 w16se w16cid w
-00000330: 3136 2077 3136 6365 7820 7731 3673 6474  16 w16cex w16sdt
-00000340: 6468 223e 3c77 3a66 6f6e 7420 773a 6e61  dh"><w:font w:na
-00000350: 6d65 3d22 5379 6d62 6f6c 223e 3c77 3a70  me="Symbol"><w:p
-00000360: 616e 6f73 6531 2077 3a76 616c 3d22 3035  anose1 w:val="05
-00000370: 3035 3031 3032 3031 3037 3036 3032 3035  0501020107060205
-00000380: 3037 222f 3e3c 773a 6368 6172 7365 7420  07"/><w:charset 
-00000390: 773a 7661 6c3d 2230 3222 2f3e 3c77 3a66  w:val="02"/><w:f
-000003a0: 616d 696c 7920 773a 7661 6c3d 2272 6f6d  amily w:val="rom
-000003b0: 616e 222f 3e3c 773a 7069 7463 6820 773a  an"/><w:pitch w:
-000003c0: 7661 6c3d 2276 6172 6961 626c 6522 2f3e  val="variable"/>
-000003d0: 3c77 3a73 6967 2077 3a75 7362 303d 2230  <w:sig w:usb0="0
-000003e0: 3030 3030 3030 3022 2077 3a75 7362 313d  0000000" w:usb1=
-000003f0: 2231 3030 3030 3030 3022 2077 3a75 7362  "10000000" w:usb
-00000400: 323d 2230 3030 3030 3030 3022 2077 3a75  2="00000000" w:u
-00000410: 7362 333d 2230 3030 3030 3030 3022 2077  sb3="00000000" w
-00000420: 3a63 7362 303d 2238 3030 3030 3030 3022  :csb0="80000000"
-00000430: 2077 3a63 7362 313d 2230 3030 3030 3030   w:csb1="0000000
-00000440: 3022 2f3e 3c2f 773a 666f 6e74 3e3c 773a  0"/></w:font><w:
-00000450: 666f 6e74 2077 3a6e 616d 653d 2254 696d  font w:name="Tim
-00000460: 6573 204e 6577 2052 6f6d 616e 223e 3c77  es New Roman"><w
-00000470: 3a70 616e 6f73 6531 2077 3a76 616c 3d22  :panose1 w:val="
-00000480: 3032 3032 3036 3033 3035 3034 3035 3032  0202060305040502
-00000490: 3033 3034 222f 3e3c 773a 6368 6172 7365  0304"/><w:charse
-000004a0: 7420 773a 7661 6c3d 2230 3022 2f3e 3c77  t w:val="00"/><w
-000004b0: 3a66 616d 696c 7920 773a 7661 6c3d 2272  :family w:val="r
-000004c0: 6f6d 616e 222f 3e3c 773a 7069 7463 6820  oman"/><w:pitch 
-000004d0: 773a 7661 6c3d 2276 6172 6961 626c 6522  w:val="variable"
-000004e0: 2f3e 3c77 3a73 6967 2077 3a75 7362 303d  /><w:sig w:usb0=
-000004f0: 2245 3030 3032 4546 4622 2077 3a75 7362  "E0002EFF" w:usb
-00000500: 313d 2243 3030 3037 3835 4222 2077 3a75  1="C000785B" w:u
-00000510: 7362 323d 2230 3030 3030 3030 3922 2077  sb2="00000009" w
-00000520: 3a75 7362 333d 2230 3030 3030 3030 3022  :usb3="00000000"
-00000530: 2077 3a63 7362 303d 2230 3030 3030 3146   w:csb0="000001F
-00000540: 4622 2077 3a63 7362 313d 2230 3030 3030  F" w:csb1="00000
-00000550: 3030 3022 2f3e 3c2f 773a 666f 6e74 3e3c  000"/></w:font><
-00000560: 773a 666f 6e74 2077 3a6e 616d 653d 2243  w:font w:name="C
-00000570: 6f75 7269 6572 204e 6577 223e 3c77 3a70  ourier New"><w:p
-00000580: 616e 6f73 6531 2077 3a76 616c 3d22 3032  anose1 w:val="02
-00000590: 3037 3033 3039 3032 3032 3035 3032 3034  0703090202050204
-000005a0: 3034 222f 3e3c 773a 6368 6172 7365 7420  04"/><w:charset 
-000005b0: 773a 7661 6c3d 2230 3022 2f3e 3c77 3a66  w:val="00"/><w:f
-000005c0: 616d 696c 7920 773a 7661 6c3d 226d 6f64  amily w:val="mod
-000005d0: 6572 6e22 2f3e 3c77 3a70 6974 6368 2077  ern"/><w:pitch w
-000005e0: 3a76 616c 3d22 6669 7865 6422 2f3e 3c77  :val="fixed"/><w
-000005f0: 3a73 6967 2077 3a75 7362 303d 2245 3030  :sig w:usb0="E00
-00000600: 3032 4546 4622 2077 3a75 7362 313d 2243  02EFF" w:usb1="C
-00000610: 3030 3037 3834 3322 2077 3a75 7362 323d  0007843" w:usb2=
-00000620: 2230 3030 3030 3030 3922 2077 3a75 7362  "00000009" w:usb
-00000630: 333d 2230 3030 3030 3030 3022 2077 3a63  3="00000000" w:c
-00000640: 7362 303d 2230 3030 3030 3146 4622 2077  sb0="000001FF" w
-00000650: 3a63 7362 313d 2230 3030 3030 3030 3022  :csb1="00000000"
-00000660: 2f3e 3c2f 773a 666f 6e74 3e3c 773a 666f  /></w:font><w:fo
-00000670: 6e74 2077 3a6e 616d 653d 2257 696e 6764  nt w:name="Wingd
-00000680: 696e 6773 223e 3c77 3a70 616e 6f73 6531  ings"><w:panose1
-00000690: 2077 3a76 616c 3d22 3035 3030 3030 3030   w:val="05000000
-000006a0: 3030 3030 3030 3030 3030 3030 222f 3e3c  000000000000"/><
-000006b0: 773a 6368 6172 7365 7420 773a 7661 6c3d  w:charset w:val=
-000006c0: 2230 3222 2f3e 3c77 3a66 616d 696c 7920  "02"/><w:family 
-000006d0: 773a 7661 6c3d 2261 7574 6f22 2f3e 3c77  w:val="auto"/><w
-000006e0: 3a70 6974 6368 2077 3a76 616c 3d22 7661  :pitch w:val="va
-000006f0: 7269 6162 6c65 222f 3e3c 773a 7369 6720  riable"/><w:sig 
-00000700: 773a 7573 6230 3d22 3030 3030 3030 3030  w:usb0="00000000
-00000710: 2220 773a 7573 6231 3d22 3130 3030 3030  " w:usb1="100000
-00000720: 3030 2220 773a 7573 6232 3d22 3030 3030  00" w:usb2="0000
-00000730: 3030 3030 2220 773a 7573 6233 3d22 3030  0000" w:usb3="00
-00000740: 3030 3030 3030 2220 773a 6373 6230 3d22  000000" w:csb0="
-00000750: 3830 3030 3030 3030 2220 773a 6373 6231  80000000" w:csb1
-00000760: 3d22 3030 3030 3030 3030 222f 3e3c 2f77  ="00000000"/></w
-00000770: 3a66 6f6e 743e 3c77 3a66 6f6e 7420 773a  :font><w:font w:
-00000780: 6e61 6d65 3d22 4361 6c69 6272 6922 3e3c  name="Calibri"><
-00000790: 773a 7061 6e6f 7365 3120 773a 7661 6c3d  w:panose1 w:val=
-000007a0: 2230 3230 4630 3530 3230 3230 3230 3430  "020F05020202040
-000007b0: 3330 3230 3422 2f3e 3c77 3a63 6861 7273  30204"/><w:chars
-000007c0: 6574 2077 3a76 616c 3d22 3030 222f 3e3c  et w:val="00"/><
-000007d0: 773a 6661 6d69 6c79 2077 3a76 616c 3d22  w:family w:val="
-000007e0: 7377 6973 7322 2f3e 3c77 3a70 6974 6368  swiss"/><w:pitch
-000007f0: 2077 3a76 616c 3d22 7661 7269 6162 6c65   w:val="variable
-00000800: 222f 3e3c 773a 7369 6720 773a 7573 6230  "/><w:sig w:usb0
-00000810: 3d22 4534 3030 3245 4646 2220 773a 7573  ="E4002EFF" w:us
-00000820: 6231 3d22 4330 3030 3234 3742 2220 773a  b1="C000247B" w:
-00000830: 7573 6232 3d22 3030 3030 3030 3039 2220  usb2="00000009" 
-00000840: 773a 7573 6233 3d22 3030 3030 3030 3030  w:usb3="00000000
-00000850: 2220 773a 6373 6230 3d22 3030 3030 3031  " w:csb0="000001
-00000860: 4646 2220 773a 6373 6231 3d22 3030 3030  FF" w:csb1="0000
-00000870: 3030 3030 222f 3e3c 2f77 3a66 6f6e 743e  0000"/></w:font>
-00000880: 3c77 3a66 6f6e 7420 773a 6e61 6d65 3d22  <w:font w:name="
-00000890: 4361 6c69 6272 6920 4c69 6768 7422 3e3c  Calibri Light"><
-000008a0: 773a 7061 6e6f 7365 3120 773a 7661 6c3d  w:panose1 w:val=
-000008b0: 2230 3230 4630 3330 3230 3230 3230 3430  "020F03020202040
-000008c0: 3330 3230 3422 2f3e 3c77 3a63 6861 7273  30204"/><w:chars
-000008d0: 6574 2077 3a76 616c 3d22 3030 222f 3e3c  et w:val="00"/><
-000008e0: 773a 6661 6d69 6c79 2077 3a76 616c 3d22  w:family w:val="
-000008f0: 7377 6973 7322 2f3e 3c77 3a70 6974 6368  swiss"/><w:pitch
-00000900: 2077 3a76 616c 3d22 7661 7269 6162 6c65   w:val="variable
-00000910: 222f 3e3c 773a 7369 6720 773a 7573 6230  "/><w:sig w:usb0
-00000920: 3d22 4534 3030 3245 4646 2220 773a 7573  ="E4002EFF" w:us
-00000930: 6231 3d22 4330 3030 3234 3742 2220 773a  b1="C000247B" w:
-00000940: 7573 6232 3d22 3030 3030 3030 3039 2220  usb2="00000009" 
-00000950: 773a 7573 6233 3d22 3030 3030 3030 3030  w:usb3="00000000
-00000960: 2220 773a 6373 6230 3d22 3030 3030 3031  " w:csb0="000001
-00000970: 4646 2220 773a 6373 6231 3d22 3030 3030  FF" w:csb1="0000
-00000980: 3030 3030 222f 3e3c 2f77 3a66 6f6e 743e  0000"/></w:font>
-00000990: 3c77 3a66 6f6e 7420 773a 6e61 6d65 3d22  <w:font w:name="
-000009a0: 436f 6e73 6f6c 6173 223e 3c77 3a70 616e  Consolas"><w:pan
-000009b0: 6f73 6531 2077 3a76 616c 3d22 3032 3042  ose1 w:val="020B
-000009c0: 3036 3039 3032 3032 3034 3033 3032 3034  0609020204030204
-000009d0: 222f 3e3c 773a 6368 6172 7365 7420 773a  "/><w:charset w:
-000009e0: 7661 6c3d 2230 3022 2f3e 3c77 3a66 616d  val="00"/><w:fam
-000009f0: 696c 7920 773a 7661 6c3d 226d 6f64 6572  ily w:val="moder
-00000a00: 6e22 2f3e 3c77 3a70 6974 6368 2077 3a76  n"/><w:pitch w:v
-00000a10: 616c 3d22 6669 7865 6422 2f3e 3c77 3a73  al="fixed"/><w:s
-00000a20: 6967 2077 3a75 7362 303d 2245 3030 3030  ig w:usb0="E0000
-00000a30: 3646 4622 2077 3a75 7362 313d 2230 3030  6FF" w:usb1="000
-00000a40: 3046 4346 4622 2077 3a75 7362 323d 2230  0FCFF" w:usb2="0
-00000a50: 3030 3030 3030 3122 2077 3a75 7362 333d  0000001" w:usb3=
-00000a60: 2230 3030 3030 3030 3022 2077 3a63 7362  "00000000" w:csb
-00000a70: 303d 2230 3030 3030 3139 4622 2077 3a63  0="0000019F" w:c
-00000a80: 7362 313d 2230 3030 3030 3030 3022 2f3e  sb1="00000000"/>
-00000a90: 3c2f 773a 666f 6e74 3e3c 2f77 3a66 6f6e  </w:font></w:fon
-00000aa0: 7473 3e                                  ts>
+00000030: 2279 6573 223f 3e0a 3c77 3a66 6f6e 7473  "yes"?>.<w:fonts
+00000040: 2078 6d6c 6e73 3a6d 633d 2268 7474 703a   xmlns:mc="http:
+00000050: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
+00000060: 6c66 6f72 6d61 7473 2e6f 7267 2f6d 6172  lformats.org/mar
+00000070: 6b75 702d 636f 6d70 6174 6962 696c 6974  kup-compatibilit
+00000080: 792f 3230 3036 2220 786d 6c6e 733a 723d  y/2006" xmlns:r=
+00000090: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+000000a0: 6f70 656e 786d 6c66 6f72 6d61 7473 2e6f  openxmlformats.o
+000000b0: 7267 2f6f 6666 6963 6544 6f63 756d 656e  rg/officeDocumen
+000000c0: 742f 3230 3036 2f72 656c 6174 696f 6e73  t/2006/relations
+000000d0: 6869 7073 2220 786d 6c6e 733a 773d 2268  hips" xmlns:w="h
+000000e0: 7474 703a 2f2f 7363 6865 6d61 732e 6f70  ttp://schemas.op
+000000f0: 656e 786d 6c66 6f72 6d61 7473 2e6f 7267  enxmlformats.org
+00000100: 2f77 6f72 6470 726f 6365 7373 696e 676d  /wordprocessingm
+00000110: 6c2f 3230 3036 2f6d 6169 6e22 2078 6d6c  l/2006/main" xml
+00000120: 6e73 3a77 3134 3d22 6874 7470 3a2f 2f73  ns:w14="http://s
+00000130: 6368 656d 6173 2e6d 6963 726f 736f 6674  chemas.microsoft
+00000140: 2e63 6f6d 2f6f 6666 6963 652f 776f 7264  .com/office/word
+00000150: 2f32 3031 302f 776f 7264 6d6c 2220 786d  /2010/wordml" xm
+00000160: 6c6e 733a 7731 353d 2268 7474 703a 2f2f  lns:w15="http://
+00000170: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
+00000180: 742e 636f 6d2f 6f66 6669 6365 2f77 6f72  t.com/office/wor
+00000190: 642f 3230 3132 2f77 6f72 646d 6c22 2078  d/2012/wordml" x
+000001a0: 6d6c 6e73 3a77 3136 6365 783d 2268 7474  mlns:w16cex="htt
+000001b0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
+000001c0: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
+000001d0: 2f77 6f72 642f 3230 3138 2f77 6f72 646d  /word/2018/wordm
+000001e0: 6c2f 6365 7822 2078 6d6c 6e73 3a77 3136  l/cex" xmlns:w16
+000001f0: 6369 643d 2268 7474 703a 2f2f 7363 6865  cid="http://sche
+00000200: 6d61 732e 6d69 6372 6f73 6f66 742e 636f  mas.microsoft.co
+00000210: 6d2f 6f66 6669 6365 2f77 6f72 642f 3230  m/office/word/20
+00000220: 3136 2f77 6f72 646d 6c2f 6369 6422 2078  16/wordml/cid" x
+00000230: 6d6c 6e73 3a77 3136 3d22 6874 7470 3a2f  mlns:w16="http:/
+00000240: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
+00000250: 6674 2e63 6f6d 2f6f 6666 6963 652f 776f  ft.com/office/wo
+00000260: 7264 2f32 3031 382f 776f 7264 6d6c 2220  rd/2018/wordml" 
+00000270: 786d 6c6e 733a 7731 3673 6474 6468 3d22  xmlns:w16sdtdh="
+00000280: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
+00000290: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
+000002a0: 6963 652f 776f 7264 2f32 3032 302f 776f  ice/word/2020/wo
+000002b0: 7264 6d6c 2f73 6474 6461 7461 6861 7368  rdml/sdtdatahash
+000002c0: 2220 786d 6c6e 733a 7731 3673 653d 2268  " xmlns:w16se="h
+000002d0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
+000002e0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
+000002f0: 6365 2f77 6f72 642f 3230 3135 2f77 6f72  ce/word/2015/wor
+00000300: 646d 6c2f 7379 6d65 7822 206d 633a 4967  dml/symex" mc:Ig
+00000310: 6e6f 7261 626c 653d 2277 3134 2077 3135  norable="w14 w15
+00000320: 2077 3136 7365 2077 3136 6369 6420 7731   w16se w16cid w1
+00000330: 3620 7731 3663 6578 2077 3136 7364 7464  6 w16cex w16sdtd
+00000340: 6822 3e3c 773a 666f 6e74 2077 3a6e 616d  h"><w:font w:nam
+00000350: 653d 2253 796d 626f 6c22 3e3c 773a 7061  e="Symbol"><w:pa
+00000360: 6e6f 7365 3120 773a 7661 6c3d 2230 3530  nose1 w:val="050
+00000370: 3530 3130 3230 3130 3730 3630 3230 3530  5010201070602050
+00000380: 3722 2f3e 3c77 3a63 6861 7273 6574 2077  7"/><w:charset w
+00000390: 3a76 616c 3d22 3032 222f 3e3c 773a 6661  :val="02"/><w:fa
+000003a0: 6d69 6c79 2077 3a76 616c 3d22 726f 6d61  mily w:val="roma
+000003b0: 6e22 2f3e 3c77 3a70 6974 6368 2077 3a76  n"/><w:pitch w:v
+000003c0: 616c 3d22 7661 7269 6162 6c65 222f 3e3c  al="variable"/><
+000003d0: 773a 7369 6720 773a 7573 6230 3d22 3030  w:sig w:usb0="00
+000003e0: 3030 3030 3030 2220 773a 7573 6231 3d22  000000" w:usb1="
+000003f0: 3130 3030 3030 3030 2220 773a 7573 6232  10000000" w:usb2
+00000400: 3d22 3030 3030 3030 3030 2220 773a 7573  ="00000000" w:us
+00000410: 6233 3d22 3030 3030 3030 3030 2220 773a  b3="00000000" w:
+00000420: 6373 6230 3d22 3830 3030 3030 3030 2220  csb0="80000000" 
+00000430: 773a 6373 6231 3d22 3030 3030 3030 3030  w:csb1="00000000
+00000440: 222f 3e3c 2f77 3a66 6f6e 743e 3c77 3a66  "/></w:font><w:f
+00000450: 6f6e 7420 773a 6e61 6d65 3d22 5469 6d65  ont w:name="Time
+00000460: 7320 4e65 7720 526f 6d61 6e22 3e3c 773a  s New Roman"><w:
+00000470: 7061 6e6f 7365 3120 773a 7661 6c3d 2230  panose1 w:val="0
+00000480: 3230 3230 3630 3330 3530 3430 3530 3230  2020603050405020
+00000490: 3330 3422 2f3e 3c77 3a63 6861 7273 6574  304"/><w:charset
+000004a0: 2077 3a76 616c 3d22 3030 222f 3e3c 773a   w:val="00"/><w:
+000004b0: 6661 6d69 6c79 2077 3a76 616c 3d22 726f  family w:val="ro
+000004c0: 6d61 6e22 2f3e 3c77 3a70 6974 6368 2077  man"/><w:pitch w
+000004d0: 3a76 616c 3d22 7661 7269 6162 6c65 222f  :val="variable"/
+000004e0: 3e3c 773a 7369 6720 773a 7573 6230 3d22  ><w:sig w:usb0="
+000004f0: 4530 3030 3245 4646 2220 773a 7573 6231  E0002EFF" w:usb1
+00000500: 3d22 4330 3030 3738 3542 2220 773a 7573  ="C000785B" w:us
+00000510: 6232 3d22 3030 3030 3030 3039 2220 773a  b2="00000009" w:
+00000520: 7573 6233 3d22 3030 3030 3030 3030 2220  usb3="00000000" 
+00000530: 773a 6373 6230 3d22 3030 3030 3031 4646  w:csb0="000001FF
+00000540: 2220 773a 6373 6231 3d22 3030 3030 3030  " w:csb1="000000
+00000550: 3030 222f 3e3c 2f77 3a66 6f6e 743e 3c77  00"/></w:font><w
+00000560: 3a66 6f6e 7420 773a 6e61 6d65 3d22 436f  :font w:name="Co
+00000570: 7572 6965 7220 4e65 7722 3e3c 773a 7061  urier New"><w:pa
+00000580: 6e6f 7365 3120 773a 7661 6c3d 2230 3230  nose1 w:val="020
+00000590: 3730 3330 3930 3230 3230 3530 3230 3430  7030902020502040
+000005a0: 3422 2f3e 3c77 3a63 6861 7273 6574 2077  4"/><w:charset w
+000005b0: 3a76 616c 3d22 3030 222f 3e3c 773a 6661  :val="00"/><w:fa
+000005c0: 6d69 6c79 2077 3a76 616c 3d22 6d6f 6465  mily w:val="mode
+000005d0: 726e 222f 3e3c 773a 7069 7463 6820 773a  rn"/><w:pitch w:
+000005e0: 7661 6c3d 2266 6978 6564 222f 3e3c 773a  val="fixed"/><w:
+000005f0: 7369 6720 773a 7573 6230 3d22 4530 3030  sig w:usb0="E000
+00000600: 3245 4646 2220 773a 7573 6231 3d22 4330  2EFF" w:usb1="C0
+00000610: 3030 3738 3433 2220 773a 7573 6232 3d22  007843" w:usb2="
+00000620: 3030 3030 3030 3039 2220 773a 7573 6233  00000009" w:usb3
+00000630: 3d22 3030 3030 3030 3030 2220 773a 6373  ="00000000" w:cs
+00000640: 6230 3d22 3030 3030 3031 4646 2220 773a  b0="000001FF" w:
+00000650: 6373 6231 3d22 3030 3030 3030 3030 222f  csb1="00000000"/
+00000660: 3e3c 2f77 3a66 6f6e 743e 3c77 3a66 6f6e  ></w:font><w:fon
+00000670: 7420 773a 6e61 6d65 3d22 5769 6e67 6469  t w:name="Wingdi
+00000680: 6e67 7322 3e3c 773a 7061 6e6f 7365 3120  ngs"><w:panose1 
+00000690: 773a 7661 6c3d 2230 3530 3030 3030 3030  w:val="050000000
+000006a0: 3030 3030 3030 3030 3030 3022 2f3e 3c77  00000000000"/><w
+000006b0: 3a63 6861 7273 6574 2077 3a76 616c 3d22  :charset w:val="
+000006c0: 3032 222f 3e3c 773a 6661 6d69 6c79 2077  02"/><w:family w
+000006d0: 3a76 616c 3d22 6175 746f 222f 3e3c 773a  :val="auto"/><w:
+000006e0: 7069 7463 6820 773a 7661 6c3d 2276 6172  pitch w:val="var
+000006f0: 6961 626c 6522 2f3e 3c77 3a73 6967 2077  iable"/><w:sig w
+00000700: 3a75 7362 303d 2230 3030 3030 3030 3022  :usb0="00000000"
+00000710: 2077 3a75 7362 313d 2231 3030 3030 3030   w:usb1="1000000
+00000720: 3022 2077 3a75 7362 323d 2230 3030 3030  0" w:usb2="00000
+00000730: 3030 3022 2077 3a75 7362 333d 2230 3030  000" w:usb3="000
+00000740: 3030 3030 3022 2077 3a63 7362 303d 2238  00000" w:csb0="8
+00000750: 3030 3030 3030 3022 2077 3a63 7362 313d  0000000" w:csb1=
+00000760: 2230 3030 3030 3030 3022 2f3e 3c2f 773a  "00000000"/></w:
+00000770: 666f 6e74 3e3c 773a 666f 6e74 2077 3a6e  font><w:font w:n
+00000780: 616d 653d 2243 616c 6962 7269 223e 3c77  ame="Calibri"><w
+00000790: 3a70 616e 6f73 6531 2077 3a76 616c 3d22  :panose1 w:val="
+000007a0: 3032 3046 3035 3032 3032 3032 3034 3033  020F050202020403
+000007b0: 3032 3034 222f 3e3c 773a 6368 6172 7365  0204"/><w:charse
+000007c0: 7420 773a 7661 6c3d 2230 3022 2f3e 3c77  t w:val="00"/><w
+000007d0: 3a66 616d 696c 7920 773a 7661 6c3d 2273  :family w:val="s
+000007e0: 7769 7373 222f 3e3c 773a 7069 7463 6820  wiss"/><w:pitch 
+000007f0: 773a 7661 6c3d 2276 6172 6961 626c 6522  w:val="variable"
+00000800: 2f3e 3c77 3a73 6967 2077 3a75 7362 303d  /><w:sig w:usb0=
+00000810: 2245 3430 3032 4546 4622 2077 3a75 7362  "E4002EFF" w:usb
+00000820: 313d 2243 3030 3032 3437 4222 2077 3a75  1="C000247B" w:u
+00000830: 7362 323d 2230 3030 3030 3030 3922 2077  sb2="00000009" w
+00000840: 3a75 7362 333d 2230 3030 3030 3030 3022  :usb3="00000000"
+00000850: 2077 3a63 7362 303d 2230 3030 3030 3146   w:csb0="000001F
+00000860: 4622 2077 3a63 7362 313d 2230 3030 3030  F" w:csb1="00000
+00000870: 3030 3022 2f3e 3c2f 773a 666f 6e74 3e3c  000"/></w:font><
+00000880: 773a 666f 6e74 2077 3a6e 616d 653d 2243  w:font w:name="C
+00000890: 616c 6962 7269 204c 6967 6874 223e 3c77  alibri Light"><w
+000008a0: 3a70 616e 6f73 6531 2077 3a76 616c 3d22  :panose1 w:val="
+000008b0: 3032 3046 3033 3032 3032 3032 3034 3033  020F030202020403
+000008c0: 3032 3034 222f 3e3c 773a 6368 6172 7365  0204"/><w:charse
+000008d0: 7420 773a 7661 6c3d 2230 3022 2f3e 3c77  t w:val="00"/><w
+000008e0: 3a66 616d 696c 7920 773a 7661 6c3d 2273  :family w:val="s
+000008f0: 7769 7373 222f 3e3c 773a 7069 7463 6820  wiss"/><w:pitch 
+00000900: 773a 7661 6c3d 2276 6172 6961 626c 6522  w:val="variable"
+00000910: 2f3e 3c77 3a73 6967 2077 3a75 7362 303d  /><w:sig w:usb0=
+00000920: 2245 3430 3032 4546 4622 2077 3a75 7362  "E4002EFF" w:usb
+00000930: 313d 2243 3030 3032 3437 4222 2077 3a75  1="C000247B" w:u
+00000940: 7362 323d 2230 3030 3030 3030 3922 2077  sb2="00000009" w
+00000950: 3a75 7362 333d 2230 3030 3030 3030 3022  :usb3="00000000"
+00000960: 2077 3a63 7362 303d 2230 3030 3030 3146   w:csb0="000001F
+00000970: 4622 2077 3a63 7362 313d 2230 3030 3030  F" w:csb1="00000
+00000980: 3030 3022 2f3e 3c2f 773a 666f 6e74 3e3c  000"/></w:font><
+00000990: 773a 666f 6e74 2077 3a6e 616d 653d 2243  w:font w:name="C
+000009a0: 6f6e 736f 6c61 7322 3e3c 773a 7061 6e6f  onsolas"><w:pano
+000009b0: 7365 3120 773a 7661 6c3d 2230 3230 4230  se1 w:val="020B0
+000009c0: 3630 3930 3230 3230 3430 3330 3230 3422  609020204030204"
+000009d0: 2f3e 3c77 3a63 6861 7273 6574 2077 3a76  /><w:charset w:v
+000009e0: 616c 3d22 3030 222f 3e3c 773a 6661 6d69  al="00"/><w:fami
+000009f0: 6c79 2077 3a76 616c 3d22 6d6f 6465 726e  ly w:val="modern
+00000a00: 222f 3e3c 773a 7069 7463 6820 773a 7661  "/><w:pitch w:va
+00000a10: 6c3d 2266 6978 6564 222f 3e3c 773a 7369  l="fixed"/><w:si
+00000a20: 6720 773a 7573 6230 3d22 4530 3030 3036  g w:usb0="E00006
+00000a30: 4646 2220 773a 7573 6231 3d22 3030 3030  FF" w:usb1="0000
+00000a40: 4643 4646 2220 773a 7573 6232 3d22 3030  FCFF" w:usb2="00
+00000a50: 3030 3030 3031 2220 773a 7573 6233 3d22  000001" w:usb3="
+00000a60: 3030 3030 3030 3030 2220 773a 6373 6230  00000000" w:csb0
+00000a70: 3d22 3030 3030 3031 3946 2220 773a 6373  ="0000019F" w:cs
+00000a80: 6231 3d22 3030 3030 3030 3030 222f 3e3c  b1="00000000"/><
+00000a90: 2f77 3a66 6f6e 743e 3c2f 773a 666f 6e74  /w:font></w:font
+00000aa0: 733e                                     s>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/numbering.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/numbering.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with very long lines (15567), with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -1,979 +1,979 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 773a 6e75 6d62  "yes"?>..<w:numb
-00000040: 6572 696e 6720 786d 6c6e 733a 7770 633d  ering xmlns:wpc=
-00000050: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-00000060: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
-00000070: 6669 6365 2f77 6f72 642f 3230 3130 2f77  fice/word/2010/w
-00000080: 6f72 6470 726f 6365 7373 696e 6743 616e  ordprocessingCan
-00000090: 7661 7322 2078 6d6c 6e73 3a63 783d 2268  vas" xmlns:cx="h
-000000a0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-000000b0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-000000c0: 6365 2f64 7261 7769 6e67 2f32 3031 342f  ce/drawing/2014/
-000000d0: 6368 6172 7465 7822 2078 6d6c 6e73 3a63  chartex" xmlns:c
-000000e0: 7831 3d22 6874 7470 3a2f 2f73 6368 656d  x1="http://schem
-000000f0: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-00000100: 2f6f 6666 6963 652f 6472 6177 696e 672f  /office/drawing/
-00000110: 3230 3135 2f39 2f38 2f63 6861 7274 6578  2015/9/8/chartex
-00000120: 2220 786d 6c6e 733a 6378 323d 2268 7474  " xmlns:cx2="htt
-00000130: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
-00000140: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
-00000150: 2f64 7261 7769 6e67 2f32 3031 352f 3130  /drawing/2015/10
-00000160: 2f32 312f 6368 6172 7465 7822 2078 6d6c  /21/chartex" xml
-00000170: 6e73 3a63 7833 3d22 6874 7470 3a2f 2f73  ns:cx3="http://s
-00000180: 6368 656d 6173 2e6d 6963 726f 736f 6674  chemas.microsoft
-00000190: 2e63 6f6d 2f6f 6666 6963 652f 6472 6177  .com/office/draw
-000001a0: 696e 672f 3230 3136 2f35 2f39 2f63 6861  ing/2016/5/9/cha
-000001b0: 7274 6578 2220 786d 6c6e 733a 6378 343d  rtex" xmlns:cx4=
-000001c0: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-000001d0: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
-000001e0: 6669 6365 2f64 7261 7769 6e67 2f32 3031  fice/drawing/201
-000001f0: 362f 352f 3130 2f63 6861 7274 6578 2220  6/5/10/chartex" 
-00000200: 786d 6c6e 733a 6378 353d 2268 7474 703a  xmlns:cx5="http:
-00000210: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
-00000220: 6f66 742e 636f 6d2f 6f66 6669 6365 2f64  oft.com/office/d
-00000230: 7261 7769 6e67 2f32 3031 362f 352f 3131  rawing/2016/5/11
-00000240: 2f63 6861 7274 6578 2220 786d 6c6e 733a  /chartex" xmlns:
-00000250: 6378 363d 2268 7474 703a 2f2f 7363 6865  cx6="http://sche
-00000260: 6d61 732e 6d69 6372 6f73 6f66 742e 636f  mas.microsoft.co
-00000270: 6d2f 6f66 6669 6365 2f64 7261 7769 6e67  m/office/drawing
-00000280: 2f32 3031 362f 352f 3132 2f63 6861 7274  /2016/5/12/chart
-00000290: 6578 2220 786d 6c6e 733a 6378 373d 2268  ex" xmlns:cx7="h
-000002a0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-000002b0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-000002c0: 6365 2f64 7261 7769 6e67 2f32 3031 362f  ce/drawing/2016/
-000002d0: 352f 3133 2f63 6861 7274 6578 2220 786d  5/13/chartex" xm
-000002e0: 6c6e 733a 6378 383d 2268 7474 703a 2f2f  lns:cx8="http://
-000002f0: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
-00000300: 742e 636f 6d2f 6f66 6669 6365 2f64 7261  t.com/office/dra
-00000310: 7769 6e67 2f32 3031 362f 352f 3134 2f63  wing/2016/5/14/c
-00000320: 6861 7274 6578 2220 786d 6c6e 733a 6d63  hartex" xmlns:mc
-00000330: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000340: 2e6f 7065 6e78 6d6c 666f 726d 6174 732e  .openxmlformats.
-00000350: 6f72 672f 6d61 726b 7570 2d63 6f6d 7061  org/markup-compa
-00000360: 7469 6269 6c69 7479 2f32 3030 3622 2078  tibility/2006" x
-00000370: 6d6c 6e73 3a61 696e 6b3d 2268 7474 703a  mlns:aink="http:
-00000380: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
-00000390: 6f66 742e 636f 6d2f 6f66 6669 6365 2f64  oft.com/office/d
-000003a0: 7261 7769 6e67 2f32 3031 362f 696e 6b22  rawing/2016/ink"
-000003b0: 2078 6d6c 6e73 3a61 6d33 643d 2268 7474   xmlns:am3d="htt
-000003c0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
-000003d0: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
-000003e0: 2f64 7261 7769 6e67 2f32 3031 372f 6d6f  /drawing/2017/mo
-000003f0: 6465 6c33 6422 2078 6d6c 6e73 3a6f 3d22  del3d" xmlns:o="
-00000400: 7572 6e3a 7363 6865 6d61 732d 6d69 6372  urn:schemas-micr
-00000410: 6f73 6f66 742d 636f 6d3a 6f66 6669 6365  osoft-com:office
-00000420: 3a6f 6666 6963 6522 2078 6d6c 6e73 3a6f  :office" xmlns:o
-00000430: 656c 3d22 6874 7470 3a2f 2f73 6368 656d  el="http://schem
-00000440: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-00000450: 2f6f 6666 6963 652f 3230 3139 2f65 7874  /office/2019/ext
-00000460: 6c73 7422 2078 6d6c 6e73 3a72 3d22 6874  lst" xmlns:r="ht
-00000470: 7470 3a2f 2f73 6368 656d 6173 2e6f 7065  tp://schemas.ope
-00000480: 6e78 6d6c 666f 726d 6174 732e 6f72 672f  nxmlformats.org/
-00000490: 6f66 6669 6365 446f 6375 6d65 6e74 2f32  officeDocument/2
-000004a0: 3030 362f 7265 6c61 7469 6f6e 7368 6970  006/relationship
-000004b0: 7322 2078 6d6c 6e73 3a6d 3d22 6874 7470  s" xmlns:m="http
-000004c0: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
-000004d0: 6d6c 666f 726d 6174 732e 6f72 672f 6f66  mlformats.org/of
-000004e0: 6669 6365 446f 6375 6d65 6e74 2f32 3030  ficeDocument/200
-000004f0: 362f 6d61 7468 2220 786d 6c6e 733a 763d  6/math" xmlns:v=
-00000500: 2275 726e 3a73 6368 656d 6173 2d6d 6963  "urn:schemas-mic
-00000510: 726f 736f 6674 2d63 6f6d 3a76 6d6c 2220  rosoft-com:vml" 
-00000520: 786d 6c6e 733a 7770 3134 3d22 6874 7470  xmlns:wp14="http
-00000530: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-00000540: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-00000550: 776f 7264 2f32 3031 302f 776f 7264 7072  word/2010/wordpr
-00000560: 6f63 6573 7369 6e67 4472 6177 696e 6722  ocessingDrawing"
-00000570: 2078 6d6c 6e73 3a77 703d 2268 7474 703a   xmlns:wp="http:
-00000580: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
-00000590: 6c66 6f72 6d61 7473 2e6f 7267 2f64 7261  lformats.org/dra
-000005a0: 7769 6e67 6d6c 2f32 3030 362f 776f 7264  wingml/2006/word
-000005b0: 7072 6f63 6573 7369 6e67 4472 6177 696e  processingDrawin
-000005c0: 6722 2078 6d6c 6e73 3a77 3130 3d22 7572  g" xmlns:w10="ur
-000005d0: 6e3a 7363 6865 6d61 732d 6d69 6372 6f73  n:schemas-micros
-000005e0: 6f66 742d 636f 6d3a 6f66 6669 6365 3a77  oft-com:office:w
-000005f0: 6f72 6422 2078 6d6c 6e73 3a77 3d22 6874  ord" xmlns:w="ht
-00000600: 7470 3a2f 2f73 6368 656d 6173 2e6f 7065  tp://schemas.ope
-00000610: 6e78 6d6c 666f 726d 6174 732e 6f72 672f  nxmlformats.org/
-00000620: 776f 7264 7072 6f63 6573 7369 6e67 6d6c  wordprocessingml
-00000630: 2f32 3030 362f 6d61 696e 2220 786d 6c6e  /2006/main" xmln
-00000640: 733a 7731 343d 2268 7474 703a 2f2f 7363  s:w14="http://sc
-00000650: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
-00000660: 636f 6d2f 6f66 6669 6365 2f77 6f72 642f  com/office/word/
-00000670: 3230 3130 2f77 6f72 646d 6c22 2078 6d6c  2010/wordml" xml
-00000680: 6e73 3a77 3135 3d22 6874 7470 3a2f 2f73  ns:w15="http://s
-00000690: 6368 656d 6173 2e6d 6963 726f 736f 6674  chemas.microsoft
-000006a0: 2e63 6f6d 2f6f 6666 6963 652f 776f 7264  .com/office/word
-000006b0: 2f32 3031 322f 776f 7264 6d6c 2220 786d  /2012/wordml" xm
-000006c0: 6c6e 733a 7731 3663 6578 3d22 6874 7470  lns:w16cex="http
-000006d0: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-000006e0: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-000006f0: 776f 7264 2f32 3031 382f 776f 7264 6d6c  word/2018/wordml
-00000700: 2f63 6578 2220 786d 6c6e 733a 7731 3663  /cex" xmlns:w16c
-00000710: 6964 3d22 6874 7470 3a2f 2f73 6368 656d  id="http://schem
-00000720: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-00000730: 2f6f 6666 6963 652f 776f 7264 2f32 3031  /office/word/201
-00000740: 362f 776f 7264 6d6c 2f63 6964 2220 786d  6/wordml/cid" xm
-00000750: 6c6e 733a 7731 363d 2268 7474 703a 2f2f  lns:w16="http://
-00000760: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
-00000770: 742e 636f 6d2f 6f66 6669 6365 2f77 6f72  t.com/office/wor
-00000780: 642f 3230 3138 2f77 6f72 646d 6c22 2078  d/2018/wordml" x
-00000790: 6d6c 6e73 3a77 3136 7364 7464 683d 2268  mlns:w16sdtdh="h
-000007a0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-000007b0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-000007c0: 6365 2f77 6f72 642f 3230 3230 2f77 6f72  ce/word/2020/wor
-000007d0: 646d 6c2f 7364 7464 6174 6168 6173 6822  dml/sdtdatahash"
-000007e0: 2078 6d6c 6e73 3a77 3136 7365 3d22 6874   xmlns:w16se="ht
-000007f0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
-00000800: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
-00000810: 652f 776f 7264 2f32 3031 352f 776f 7264  e/word/2015/word
-00000820: 6d6c 2f73 796d 6578 2220 786d 6c6e 733a  ml/symex" xmlns:
-00000830: 7770 673d 2268 7474 703a 2f2f 7363 6865  wpg="http://sche
-00000840: 6d61 732e 6d69 6372 6f73 6f66 742e 636f  mas.microsoft.co
-00000850: 6d2f 6f66 6669 6365 2f77 6f72 642f 3230  m/office/word/20
-00000860: 3130 2f77 6f72 6470 726f 6365 7373 696e  10/wordprocessin
-00000870: 6747 726f 7570 2220 786d 6c6e 733a 7770  gGroup" xmlns:wp
-00000880: 693d 2268 7474 703a 2f2f 7363 6865 6d61  i="http://schema
-00000890: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
-000008a0: 6f66 6669 6365 2f77 6f72 642f 3230 3130  office/word/2010
-000008b0: 2f77 6f72 6470 726f 6365 7373 696e 6749  /wordprocessingI
-000008c0: 6e6b 2220 786d 6c6e 733a 776e 653d 2268  nk" xmlns:wne="h
-000008d0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-000008e0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-000008f0: 6365 2f77 6f72 642f 3230 3036 2f77 6f72  ce/word/2006/wor
-00000900: 646d 6c22 2078 6d6c 6e73 3a77 7073 3d22  dml" xmlns:wps="
-00000910: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
-00000920: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
-00000930: 6963 652f 776f 7264 2f32 3031 302f 776f  ice/word/2010/wo
-00000940: 7264 7072 6f63 6573 7369 6e67 5368 6170  rdprocessingShap
-00000950: 6522 206d 633a 4967 6e6f 7261 626c 653d  e" mc:Ignorable=
-00000960: 2277 3134 2077 3135 2077 3136 7365 2077  "w14 w15 w16se w
-00000970: 3136 6369 6420 7731 3620 7731 3663 6578  16cid w16 w16cex
-00000980: 2077 3136 7364 7464 6820 7770 3134 223e   w16sdtdh wp14">
-00000990: 3c77 3a61 6273 7472 6163 744e 756d 2077  <w:abstractNum w
-000009a0: 3a61 6273 7472 6163 744e 756d 4964 3d22  :abstractNumId="
-000009b0: 3022 2077 3135 3a72 6573 7461 7274 4e75  0" w15:restartNu
-000009c0: 6d62 6572 696e 6741 6674 6572 4272 6561  mberingAfterBrea
-000009d0: 6b3d 2230 223e 3c77 3a6e 7369 6420 773a  k="0"><w:nsid w:
-000009e0: 7661 6c3d 2246 4646 4646 4637 4322 2f3e  val="FFFFFF7C"/>
-000009f0: 3c77 3a6d 756c 7469 4c65 7665 6c54 7970  <w:multiLevelTyp
-00000a00: 6520 773a 7661 6c3d 2273 696e 676c 654c  e w:val="singleL
-00000a10: 6576 656c 222f 3e3c 773a 746d 706c 2077  evel"/><w:tmpl w
-00000a20: 3a76 616c 3d22 3243 3938 3336 4243 222f  :val="2C9836BC"/
-00000a30: 3e3c 773a 6c76 6c20 773a 696c 766c 3d22  ><w:lvl w:ilvl="
-00000a40: 3022 3e3c 773a 7374 6172 7420 773a 7661  0"><w:start w:va
-00000a50: 6c3d 2231 222f 3e3c 773a 6e75 6d46 6d74  l="1"/><w:numFmt
-00000a60: 2077 3a76 616c 3d22 6465 6369 6d61 6c22   w:val="decimal"
-00000a70: 2f3e 3c77 3a6c 766c 5465 7874 2077 3a76  /><w:lvlText w:v
-00000a80: 616c 3d22 2531 2e22 2f3e 3c77 3a6c 766c  al="%1."/><w:lvl
-00000a90: 4a63 2077 3a76 616c 3d22 6c65 6674 222f  Jc w:val="left"/
-00000aa0: 3e3c 773a 7050 723e 3c77 3a74 6162 733e  ><w:pPr><w:tabs>
-00000ab0: 3c77 3a74 6162 2077 3a76 616c 3d22 6e75  <w:tab w:val="nu
-00000ac0: 6d22 2077 3a70 6f73 3d22 3134 3932 222f  m" w:pos="1492"/
-00000ad0: 3e3c 2f77 3a74 6162 733e 3c77 3a69 6e64  ></w:tabs><w:ind
-00000ae0: 2077 3a6c 6566 743d 2231 3439 3222 2077   w:left="1492" w
-00000af0: 3a68 616e 6769 6e67 3d22 3336 3022 2f3e  :hanging="360"/>
-00000b00: 3c2f 773a 7050 723e 3c2f 773a 6c76 6c3e  </w:pPr></w:lvl>
-00000b10: 3c2f 773a 6162 7374 7261 6374 4e75 6d3e  </w:abstractNum>
-00000b20: 3c77 3a61 6273 7472 6163 744e 756d 2077  <w:abstractNum w
-00000b30: 3a61 6273 7472 6163 744e 756d 4964 3d22  :abstractNumId="
-00000b40: 3122 2077 3135 3a72 6573 7461 7274 4e75  1" w15:restartNu
-00000b50: 6d62 6572 696e 6741 6674 6572 4272 6561  mberingAfterBrea
-00000b60: 6b3d 2230 223e 3c77 3a6e 7369 6420 773a  k="0"><w:nsid w:
-00000b70: 7661 6c3d 2246 4646 4646 4637 4422 2f3e  val="FFFFFF7D"/>
-00000b80: 3c77 3a6d 756c 7469 4c65 7665 6c54 7970  <w:multiLevelTyp
-00000b90: 6520 773a 7661 6c3d 2273 696e 676c 654c  e w:val="singleL
-00000ba0: 6576 656c 222f 3e3c 773a 746d 706c 2077  evel"/><w:tmpl w
-00000bb0: 3a76 616c 3d22 3239 3132 3031 4530 222f  :val="291201E0"/
-00000bc0: 3e3c 773a 6c76 6c20 773a 696c 766c 3d22  ><w:lvl w:ilvl="
-00000bd0: 3022 3e3c 773a 7374 6172 7420 773a 7661  0"><w:start w:va
-00000be0: 6c3d 2231 222f 3e3c 773a 6e75 6d46 6d74  l="1"/><w:numFmt
-00000bf0: 2077 3a76 616c 3d22 6465 6369 6d61 6c22   w:val="decimal"
-00000c00: 2f3e 3c77 3a6c 766c 5465 7874 2077 3a76  /><w:lvlText w:v
-00000c10: 616c 3d22 2531 2e22 2f3e 3c77 3a6c 766c  al="%1."/><w:lvl
-00000c20: 4a63 2077 3a76 616c 3d22 6c65 6674 222f  Jc w:val="left"/
-00000c30: 3e3c 773a 7050 723e 3c77 3a74 6162 733e  ><w:pPr><w:tabs>
-00000c40: 3c77 3a74 6162 2077 3a76 616c 3d22 6e75  <w:tab w:val="nu
-00000c50: 6d22 2077 3a70 6f73 3d22 3132 3039 222f  m" w:pos="1209"/
-00000c60: 3e3c 2f77 3a74 6162 733e 3c77 3a69 6e64  ></w:tabs><w:ind
-00000c70: 2077 3a6c 6566 743d 2231 3230 3922 2077   w:left="1209" w
-00000c80: 3a68 616e 6769 6e67 3d22 3336 3022 2f3e  :hanging="360"/>
-00000c90: 3c2f 773a 7050 723e 3c2f 773a 6c76 6c3e  </w:pPr></w:lvl>
-00000ca0: 3c2f 773a 6162 7374 7261 6374 4e75 6d3e  </w:abstractNum>
-00000cb0: 3c77 3a61 6273 7472 6163 744e 756d 2077  <w:abstractNum w
-00000cc0: 3a61 6273 7472 6163 744e 756d 4964 3d22  :abstractNumId="
-00000cd0: 3222 2077 3135 3a72 6573 7461 7274 4e75  2" w15:restartNu
-00000ce0: 6d62 6572 696e 6741 6674 6572 4272 6561  mberingAfterBrea
-00000cf0: 6b3d 2230 223e 3c77 3a6e 7369 6420 773a  k="0"><w:nsid w:
-00000d00: 7661 6c3d 2246 4646 4646 4637 4522 2f3e  val="FFFFFF7E"/>
-00000d10: 3c77 3a6d 756c 7469 4c65 7665 6c54 7970  <w:multiLevelTyp
-00000d20: 6520 773a 7661 6c3d 2273 696e 676c 654c  e w:val="singleL
-00000d30: 6576 656c 222f 3e3c 773a 746d 706c 2077  evel"/><w:tmpl w
-00000d40: 3a76 616c 3d22 4432 3541 3730 4345 222f  :val="D25A70CE"/
-00000d50: 3e3c 773a 6c76 6c20 773a 696c 766c 3d22  ><w:lvl w:ilvl="
-00000d60: 3022 3e3c 773a 7374 6172 7420 773a 7661  0"><w:start w:va
-00000d70: 6c3d 2231 222f 3e3c 773a 6e75 6d46 6d74  l="1"/><w:numFmt
-00000d80: 2077 3a76 616c 3d22 6465 6369 6d61 6c22   w:val="decimal"
-00000d90: 2f3e 3c77 3a6c 766c 5465 7874 2077 3a76  /><w:lvlText w:v
-00000da0: 616c 3d22 2531 2e22 2f3e 3c77 3a6c 766c  al="%1."/><w:lvl
-00000db0: 4a63 2077 3a76 616c 3d22 6c65 6674 222f  Jc w:val="left"/
-00000dc0: 3e3c 773a 7050 723e 3c77 3a74 6162 733e  ><w:pPr><w:tabs>
-00000dd0: 3c77 3a74 6162 2077 3a76 616c 3d22 6e75  <w:tab w:val="nu
-00000de0: 6d22 2077 3a70 6f73 3d22 3932 3622 2f3e  m" w:pos="926"/>
-00000df0: 3c2f 773a 7461 6273 3e3c 773a 696e 6420  </w:tabs><w:ind 
-00000e00: 773a 6c65 6674 3d22 3932 3622 2077 3a68  w:left="926" w:h
-00000e10: 616e 6769 6e67 3d22 3336 3022 2f3e 3c2f  anging="360"/></
-00000e20: 773a 7050 723e 3c2f 773a 6c76 6c3e 3c2f  w:pPr></w:lvl></
-00000e30: 773a 6162 7374 7261 6374 4e75 6d3e 3c77  w:abstractNum><w
-00000e40: 3a61 6273 7472 6163 744e 756d 2077 3a61  :abstractNum w:a
-00000e50: 6273 7472 6163 744e 756d 4964 3d22 3322  bstractNumId="3"
-00000e60: 2077 3135 3a72 6573 7461 7274 4e75 6d62   w15:restartNumb
-00000e70: 6572 696e 6741 6674 6572 4272 6561 6b3d  eringAfterBreak=
-00000e80: 2230 223e 3c77 3a6e 7369 6420 773a 7661  "0"><w:nsid w:va
-00000e90: 6c3d 2246 4646 4646 4637 4622 2f3e 3c77  l="FFFFFF7F"/><w
-00000ea0: 3a6d 756c 7469 4c65 7665 6c54 7970 6520  :multiLevelType 
-00000eb0: 773a 7661 6c3d 2273 696e 676c 654c 6576  w:val="singleLev
-00000ec0: 656c 222f 3e3c 773a 746d 706c 2077 3a76  el"/><w:tmpl w:v
-00000ed0: 616c 3d22 3143 3934 4134 3730 222f 3e3c  al="1C94A470"/><
-00000ee0: 773a 6c76 6c20 773a 696c 766c 3d22 3022  w:lvl w:ilvl="0"
-00000ef0: 3e3c 773a 7374 6172 7420 773a 7661 6c3d  ><w:start w:val=
-00000f00: 2231 222f 3e3c 773a 6e75 6d46 6d74 2077  "1"/><w:numFmt w
-00000f10: 3a76 616c 3d22 6465 6369 6d61 6c22 2f3e  :val="decimal"/>
-00000f20: 3c77 3a6c 766c 5465 7874 2077 3a76 616c  <w:lvlText w:val
-00000f30: 3d22 2531 2e22 2f3e 3c77 3a6c 766c 4a63  ="%1."/><w:lvlJc
-00000f40: 2077 3a76 616c 3d22 6c65 6674 222f 3e3c   w:val="left"/><
-00000f50: 773a 7050 723e 3c77 3a74 6162 733e 3c77  w:pPr><w:tabs><w
-00000f60: 3a74 6162 2077 3a76 616c 3d22 6e75 6d22  :tab w:val="num"
-00000f70: 2077 3a70 6f73 3d22 3634 3322 2f3e 3c2f   w:pos="643"/></
-00000f80: 773a 7461 6273 3e3c 773a 696e 6420 773a  w:tabs><w:ind w:
-00000f90: 6c65 6674 3d22 3634 3322 2077 3a68 616e  left="643" w:han
-00000fa0: 6769 6e67 3d22 3336 3022 2f3e 3c2f 773a  ging="360"/></w:
-00000fb0: 7050 723e 3c2f 773a 6c76 6c3e 3c2f 773a  pPr></w:lvl></w:
-00000fc0: 6162 7374 7261 6374 4e75 6d3e 3c77 3a61  abstractNum><w:a
-00000fd0: 6273 7472 6163 744e 756d 2077 3a61 6273  bstractNum w:abs
-00000fe0: 7472 6163 744e 756d 4964 3d22 3422 2077  tractNumId="4" w
-00000ff0: 3135 3a72 6573 7461 7274 4e75 6d62 6572  15:restartNumber
-00001000: 696e 6741 6674 6572 4272 6561 6b3d 2230  ingAfterBreak="0
-00001010: 223e 3c77 3a6e 7369 6420 773a 7661 6c3d  "><w:nsid w:val=
-00001020: 2246 4646 4646 4638 3022 2f3e 3c77 3a6d  "FFFFFF80"/><w:m
-00001030: 756c 7469 4c65 7665 6c54 7970 6520 773a  ultiLevelType w:
-00001040: 7661 6c3d 2273 696e 676c 654c 6576 656c  val="singleLevel
-00001050: 222f 3e3c 773a 746d 706c 2077 3a76 616c  "/><w:tmpl w:val
-00001060: 3d22 3644 3636 3644 3745 222f 3e3c 773a  ="6D666D7E"/><w:
-00001070: 6c76 6c20 773a 696c 766c 3d22 3022 3e3c  lvl w:ilvl="0"><
-00001080: 773a 7374 6172 7420 773a 7661 6c3d 2231  w:start w:val="1
-00001090: 222f 3e3c 773a 6e75 6d46 6d74 2077 3a76  "/><w:numFmt w:v
-000010a0: 616c 3d22 6275 6c6c 6574 222f 3e3c 773a  al="bullet"/><w:
-000010b0: 6c76 6c54 6578 7420 773a 7661 6c3d 22ef  lvlText w:val=".
-000010c0: 82b7 222f 3e3c 773a 6c76 6c4a 6320 773a  .."/><w:lvlJc w:
-000010d0: 7661 6c3d 226c 6566 7422 2f3e 3c77 3a70  val="left"/><w:p
-000010e0: 5072 3e3c 773a 7461 6273 3e3c 773a 7461  Pr><w:tabs><w:ta
-000010f0: 6220 773a 7661 6c3d 226e 756d 2220 773a  b w:val="num" w:
-00001100: 706f 733d 2231 3439 3222 2f3e 3c2f 773a  pos="1492"/></w:
-00001110: 7461 6273 3e3c 773a 696e 6420 773a 6c65  tabs><w:ind w:le
-00001120: 6674 3d22 3134 3932 2220 773a 6861 6e67  ft="1492" w:hang
-00001130: 696e 673d 2233 3630 222f 3e3c 2f77 3a70  ing="360"/></w:p
-00001140: 5072 3e3c 773a 7250 723e 3c77 3a72 466f  Pr><w:rPr><w:rFo
-00001150: 6e74 7320 773a 6173 6369 693d 2253 796d  nts w:ascii="Sym
-00001160: 626f 6c22 2077 3a68 416e 7369 3d22 5379  bol" w:hAnsi="Sy
-00001170: 6d62 6f6c 2220 773a 6869 6e74 3d22 6465  mbol" w:hint="de
-00001180: 6661 756c 7422 2f3e 3c2f 773a 7250 723e  fault"/></w:rPr>
-00001190: 3c2f 773a 6c76 6c3e 3c2f 773a 6162 7374  </w:lvl></w:abst
-000011a0: 7261 6374 4e75 6d3e 3c77 3a61 6273 7472  ractNum><w:abstr
-000011b0: 6163 744e 756d 2077 3a61 6273 7472 6163  actNum w:abstrac
-000011c0: 744e 756d 4964 3d22 3522 2077 3135 3a72  tNumId="5" w15:r
-000011d0: 6573 7461 7274 4e75 6d62 6572 696e 6741  estartNumberingA
-000011e0: 6674 6572 4272 6561 6b3d 2230 223e 3c77  fterBreak="0"><w
-000011f0: 3a6e 7369 6420 773a 7661 6c3d 2246 4646  :nsid w:val="FFF
-00001200: 4646 4638 3122 2f3e 3c77 3a6d 756c 7469  FFF81"/><w:multi
-00001210: 4c65 7665 6c54 7970 6520 773a 7661 6c3d  LevelType w:val=
-00001220: 2273 696e 676c 654c 6576 656c 222f 3e3c  "singleLevel"/><
-00001230: 773a 746d 706c 2077 3a76 616c 3d22 4537  w:tmpl w:val="E7
-00001240: 3941 3830 3241 222f 3e3c 773a 6c76 6c20  9A802A"/><w:lvl 
-00001250: 773a 696c 766c 3d22 3022 3e3c 773a 7374  w:ilvl="0"><w:st
-00001260: 6172 7420 773a 7661 6c3d 2231 222f 3e3c  art w:val="1"/><
-00001270: 773a 6e75 6d46 6d74 2077 3a76 616c 3d22  w:numFmt w:val="
-00001280: 6275 6c6c 6574 222f 3e3c 773a 6c76 6c54  bullet"/><w:lvlT
-00001290: 6578 7420 773a 7661 6c3d 22ef 82b7 222f  ext w:val="..."/
-000012a0: 3e3c 773a 6c76 6c4a 6320 773a 7661 6c3d  ><w:lvlJc w:val=
-000012b0: 226c 6566 7422 2f3e 3c77 3a70 5072 3e3c  "left"/><w:pPr><
-000012c0: 773a 7461 6273 3e3c 773a 7461 6220 773a  w:tabs><w:tab w:
-000012d0: 7661 6c3d 226e 756d 2220 773a 706f 733d  val="num" w:pos=
-000012e0: 2231 3230 3922 2f3e 3c2f 773a 7461 6273  "1209"/></w:tabs
-000012f0: 3e3c 773a 696e 6420 773a 6c65 6674 3d22  ><w:ind w:left="
-00001300: 3132 3039 2220 773a 6861 6e67 696e 673d  1209" w:hanging=
-00001310: 2233 3630 222f 3e3c 2f77 3a70 5072 3e3c  "360"/></w:pPr><
-00001320: 773a 7250 723e 3c77 3a72 466f 6e74 7320  w:rPr><w:rFonts 
-00001330: 773a 6173 6369 693d 2253 796d 626f 6c22  w:ascii="Symbol"
-00001340: 2077 3a68 416e 7369 3d22 5379 6d62 6f6c   w:hAnsi="Symbol
-00001350: 2220 773a 6869 6e74 3d22 6465 6661 756c  " w:hint="defaul
-00001360: 7422 2f3e 3c2f 773a 7250 723e 3c2f 773a  t"/></w:rPr></w:
-00001370: 6c76 6c3e 3c2f 773a 6162 7374 7261 6374  lvl></w:abstract
-00001380: 4e75 6d3e 3c77 3a61 6273 7472 6163 744e  Num><w:abstractN
-00001390: 756d 2077 3a61 6273 7472 6163 744e 756d  um w:abstractNum
-000013a0: 4964 3d22 3622 2077 3135 3a72 6573 7461  Id="6" w15:resta
-000013b0: 7274 4e75 6d62 6572 696e 6741 6674 6572  rtNumberingAfter
-000013c0: 4272 6561 6b3d 2230 223e 3c77 3a6e 7369  Break="0"><w:nsi
-000013d0: 6420 773a 7661 6c3d 2246 4646 4646 4638  d w:val="FFFFFF8
-000013e0: 3222 2f3e 3c77 3a6d 756c 7469 4c65 7665  2"/><w:multiLeve
-000013f0: 6c54 7970 6520 773a 7661 6c3d 2273 696e  lType w:val="sin
-00001400: 676c 654c 6576 656c 222f 3e3c 773a 746d  gleLevel"/><w:tm
-00001410: 706c 2077 3a76 616c 3d22 4639 4645 3144  pl w:val="F9FE1D
-00001420: 3843 222f 3e3c 773a 6c76 6c20 773a 696c  8C"/><w:lvl w:il
-00001430: 766c 3d22 3022 3e3c 773a 7374 6172 7420  vl="0"><w:start 
-00001440: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
-00001450: 6d46 6d74 2077 3a76 616c 3d22 6275 6c6c  mFmt w:val="bull
-00001460: 6574 222f 3e3c 773a 6c76 6c54 6578 7420  et"/><w:lvlText 
-00001470: 773a 7661 6c3d 22ef 82b7 222f 3e3c 773a  w:val="..."/><w:
-00001480: 6c76 6c4a 6320 773a 7661 6c3d 226c 6566  lvlJc w:val="lef
-00001490: 7422 2f3e 3c77 3a70 5072 3e3c 773a 7461  t"/><w:pPr><w:ta
-000014a0: 6273 3e3c 773a 7461 6220 773a 7661 6c3d  bs><w:tab w:val=
-000014b0: 226e 756d 2220 773a 706f 733d 2239 3236  "num" w:pos="926
-000014c0: 222f 3e3c 2f77 3a74 6162 733e 3c77 3a69  "/></w:tabs><w:i
-000014d0: 6e64 2077 3a6c 6566 743d 2239 3236 2220  nd w:left="926" 
-000014e0: 773a 6861 6e67 696e 673d 2233 3630 222f  w:hanging="360"/
-000014f0: 3e3c 2f77 3a70 5072 3e3c 773a 7250 723e  ></w:pPr><w:rPr>
-00001500: 3c77 3a72 466f 6e74 7320 773a 6173 6369  <w:rFonts w:asci
-00001510: 693d 2253 796d 626f 6c22 2077 3a68 416e  i="Symbol" w:hAn
-00001520: 7369 3d22 5379 6d62 6f6c 2220 773a 6869  si="Symbol" w:hi
-00001530: 6e74 3d22 6465 6661 756c 7422 2f3e 3c2f  nt="default"/></
-00001540: 773a 7250 723e 3c2f 773a 6c76 6c3e 3c2f  w:rPr></w:lvl></
-00001550: 773a 6162 7374 7261 6374 4e75 6d3e 3c77  w:abstractNum><w
-00001560: 3a61 6273 7472 6163 744e 756d 2077 3a61  :abstractNum w:a
-00001570: 6273 7472 6163 744e 756d 4964 3d22 3722  bstractNumId="7"
-00001580: 2077 3135 3a72 6573 7461 7274 4e75 6d62   w15:restartNumb
-00001590: 6572 696e 6741 6674 6572 4272 6561 6b3d  eringAfterBreak=
-000015a0: 2230 223e 3c77 3a6e 7369 6420 773a 7661  "0"><w:nsid w:va
-000015b0: 6c3d 2246 4646 4646 4638 3322 2f3e 3c77  l="FFFFFF83"/><w
-000015c0: 3a6d 756c 7469 4c65 7665 6c54 7970 6520  :multiLevelType 
-000015d0: 773a 7661 6c3d 2273 696e 676c 654c 6576  w:val="singleLev
-000015e0: 656c 222f 3e3c 773a 746d 706c 2077 3a76  el"/><w:tmpl w:v
-000015f0: 616c 3d22 4237 3936 3732 3643 222f 3e3c  al="B796726C"/><
-00001600: 773a 6c76 6c20 773a 696c 766c 3d22 3022  w:lvl w:ilvl="0"
-00001610: 3e3c 773a 7374 6172 7420 773a 7661 6c3d  ><w:start w:val=
-00001620: 2231 222f 3e3c 773a 6e75 6d46 6d74 2077  "1"/><w:numFmt w
-00001630: 3a76 616c 3d22 6275 6c6c 6574 222f 3e3c  :val="bullet"/><
-00001640: 773a 6c76 6c54 6578 7420 773a 7661 6c3d  w:lvlText w:val=
-00001650: 22ef 82b7 222f 3e3c 773a 6c76 6c4a 6320  "..."/><w:lvlJc 
-00001660: 773a 7661 6c3d 226c 6566 7422 2f3e 3c77  w:val="left"/><w
-00001670: 3a70 5072 3e3c 773a 7461 6273 3e3c 773a  :pPr><w:tabs><w:
-00001680: 7461 6220 773a 7661 6c3d 226e 756d 2220  tab w:val="num" 
-00001690: 773a 706f 733d 2236 3433 222f 3e3c 2f77  w:pos="643"/></w
-000016a0: 3a74 6162 733e 3c77 3a69 6e64 2077 3a6c  :tabs><w:ind w:l
-000016b0: 6566 743d 2236 3433 2220 773a 6861 6e67  eft="643" w:hang
-000016c0: 696e 673d 2233 3630 222f 3e3c 2f77 3a70  ing="360"/></w:p
-000016d0: 5072 3e3c 773a 7250 723e 3c77 3a72 466f  Pr><w:rPr><w:rFo
-000016e0: 6e74 7320 773a 6173 6369 693d 2253 796d  nts w:ascii="Sym
-000016f0: 626f 6c22 2077 3a68 416e 7369 3d22 5379  bol" w:hAnsi="Sy
-00001700: 6d62 6f6c 2220 773a 6869 6e74 3d22 6465  mbol" w:hint="de
-00001710: 6661 756c 7422 2f3e 3c2f 773a 7250 723e  fault"/></w:rPr>
-00001720: 3c2f 773a 6c76 6c3e 3c2f 773a 6162 7374  </w:lvl></w:abst
-00001730: 7261 6374 4e75 6d3e 3c77 3a61 6273 7472  ractNum><w:abstr
-00001740: 6163 744e 756d 2077 3a61 6273 7472 6163  actNum w:abstrac
-00001750: 744e 756d 4964 3d22 3822 2077 3135 3a72  tNumId="8" w15:r
-00001760: 6573 7461 7274 4e75 6d62 6572 696e 6741  estartNumberingA
-00001770: 6674 6572 4272 6561 6b3d 2230 223e 3c77  fterBreak="0"><w
-00001780: 3a6e 7369 6420 773a 7661 6c3d 2246 4646  :nsid w:val="FFF
-00001790: 4646 4638 3822 2f3e 3c77 3a6d 756c 7469  FFF88"/><w:multi
-000017a0: 4c65 7665 6c54 7970 6520 773a 7661 6c3d  LevelType w:val=
-000017b0: 2273 696e 676c 654c 6576 656c 222f 3e3c  "singleLevel"/><
-000017c0: 773a 746d 706c 2077 3a76 616c 3d22 4244  w:tmpl w:val="BD
-000017d0: 3943 4239 3334 222f 3e3c 773a 6c76 6c20  9CB934"/><w:lvl 
-000017e0: 773a 696c 766c 3d22 3022 3e3c 773a 7374  w:ilvl="0"><w:st
-000017f0: 6172 7420 773a 7661 6c3d 2231 222f 3e3c  art w:val="1"/><
-00001800: 773a 6e75 6d46 6d74 2077 3a76 616c 3d22  w:numFmt w:val="
-00001810: 6465 6369 6d61 6c22 2f3e 3c77 3a70 5374  decimal"/><w:pSt
-00001820: 796c 6520 773a 7661 6c3d 224c 6973 744e  yle w:val="ListN
-00001830: 756d 6265 7222 2f3e 3c77 3a6c 766c 5465  umber"/><w:lvlTe
-00001840: 7874 2077 3a76 616c 3d22 2531 2e22 2f3e  xt w:val="%1."/>
-00001850: 3c77 3a6c 766c 4a63 2077 3a76 616c 3d22  <w:lvlJc w:val="
-00001860: 6c65 6674 222f 3e3c 773a 7050 723e 3c77  left"/><w:pPr><w
-00001870: 3a74 6162 733e 3c77 3a74 6162 2077 3a76  :tabs><w:tab w:v
-00001880: 616c 3d22 6e75 6d22 2077 3a70 6f73 3d22  al="num" w:pos="
-00001890: 3336 3022 2f3e 3c2f 773a 7461 6273 3e3c  360"/></w:tabs><
-000018a0: 773a 696e 6420 773a 6c65 6674 3d22 3336  w:ind w:left="36
-000018b0: 3022 2077 3a68 616e 6769 6e67 3d22 3336  0" w:hanging="36
-000018c0: 3022 2f3e 3c2f 773a 7050 723e 3c2f 773a  0"/></w:pPr></w:
-000018d0: 6c76 6c3e 3c2f 773a 6162 7374 7261 6374  lvl></w:abstract
-000018e0: 4e75 6d3e 3c77 3a61 6273 7472 6163 744e  Num><w:abstractN
-000018f0: 756d 2077 3a61 6273 7472 6163 744e 756d  um w:abstractNum
-00001900: 4964 3d22 3922 2077 3135 3a72 6573 7461  Id="9" w15:resta
-00001910: 7274 4e75 6d62 6572 696e 6741 6674 6572  rtNumberingAfter
-00001920: 4272 6561 6b3d 2230 223e 3c77 3a6e 7369  Break="0"><w:nsi
-00001930: 6420 773a 7661 6c3d 2246 4646 4646 4638  d w:val="FFFFFF8
-00001940: 3922 2f3e 3c77 3a6d 756c 7469 4c65 7665  9"/><w:multiLeve
-00001950: 6c54 7970 6520 773a 7661 6c3d 2273 696e  lType w:val="sin
-00001960: 676c 654c 6576 656c 222f 3e3c 773a 746d  gleLevel"/><w:tm
-00001970: 706c 2077 3a76 616c 3d22 3030 3038 3944  pl w:val="00089D
-00001980: 3245 222f 3e3c 773a 6c76 6c20 773a 696c  2E"/><w:lvl w:il
-00001990: 766c 3d22 3022 3e3c 773a 7374 6172 7420  vl="0"><w:start 
-000019a0: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
-000019b0: 6d46 6d74 2077 3a76 616c 3d22 6275 6c6c  mFmt w:val="bull
-000019c0: 6574 222f 3e3c 773a 7053 7479 6c65 2077  et"/><w:pStyle w
-000019d0: 3a76 616c 3d22 4c69 7374 4275 6c6c 6574  :val="ListBullet
-000019e0: 222f 3e3c 773a 6c76 6c54 6578 7420 773a  "/><w:lvlText w:
-000019f0: 7661 6c3d 22ef 82b7 222f 3e3c 773a 6c76  val="..."/><w:lv
-00001a00: 6c4a 6320 773a 7661 6c3d 226c 6566 7422  lJc w:val="left"
-00001a10: 2f3e 3c77 3a70 5072 3e3c 773a 7461 6273  /><w:pPr><w:tabs
-00001a20: 3e3c 773a 7461 6220 773a 7661 6c3d 226e  ><w:tab w:val="n
-00001a30: 756d 2220 773a 706f 733d 2233 3630 222f  um" w:pos="360"/
-00001a40: 3e3c 2f77 3a74 6162 733e 3c77 3a69 6e64  ></w:tabs><w:ind
-00001a50: 2077 3a6c 6566 743d 2233 3630 2220 773a   w:left="360" w:
-00001a60: 6861 6e67 696e 673d 2233 3630 222f 3e3c  hanging="360"/><
-00001a70: 2f77 3a70 5072 3e3c 773a 7250 723e 3c77  /w:pPr><w:rPr><w
-00001a80: 3a72 466f 6e74 7320 773a 6173 6369 693d  :rFonts w:ascii=
-00001a90: 2253 796d 626f 6c22 2077 3a68 416e 7369  "Symbol" w:hAnsi
-00001aa0: 3d22 5379 6d62 6f6c 2220 773a 6869 6e74  ="Symbol" w:hint
-00001ab0: 3d22 6465 6661 756c 7422 2f3e 3c2f 773a  ="default"/></w:
-00001ac0: 7250 723e 3c2f 773a 6c76 6c3e 3c2f 773a  rPr></w:lvl></w:
-00001ad0: 6162 7374 7261 6374 4e75 6d3e 3c77 3a61  abstractNum><w:a
-00001ae0: 6273 7472 6163 744e 756d 2077 3a61 6273  bstractNum w:abs
-00001af0: 7472 6163 744e 756d 4964 3d22 3130 2220  tractNumId="10" 
-00001b00: 7731 353a 7265 7374 6172 744e 756d 6265  w15:restartNumbe
-00001b10: 7269 6e67 4166 7465 7242 7265 616b 3d22  ringAfterBreak="
-00001b20: 3022 3e3c 773a 6e73 6964 2077 3a76 616c  0"><w:nsid w:val
-00001b30: 3d22 3246 3437 3633 4342 222f 3e3c 773a  ="2F4763CB"/><w:
-00001b40: 6d75 6c74 694c 6576 656c 5479 7065 2077  multiLevelType w
-00001b50: 3a76 616c 3d22 6879 6272 6964 4d75 6c74  :val="hybridMult
-00001b60: 696c 6576 656c 222f 3e3c 773a 746d 706c  ilevel"/><w:tmpl
-00001b70: 2077 3a76 616c 3d22 3734 3341 3534 3141   w:val="743A541A
-00001b80: 222f 3e3c 773a 6c76 6c20 773a 696c 766c  "/><w:lvl w:ilvl
-00001b90: 3d22 3022 2077 3a74 706c 633d 2232 3030  ="0" w:tplc="200
-00001ba0: 3030 3030 3122 3e3c 773a 7374 6172 7420  00001"><w:start 
-00001bb0: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
-00001bc0: 6d46 6d74 2077 3a76 616c 3d22 6275 6c6c  mFmt w:val="bull
-00001bd0: 6574 222f 3e3c 773a 6c76 6c54 6578 7420  et"/><w:lvlText 
-00001be0: 773a 7661 6c3d 22ef 82b7 222f 3e3c 773a  w:val="..."/><w:
-00001bf0: 6c76 6c4a 6320 773a 7661 6c3d 226c 6566  lvlJc w:val="lef
-00001c00: 7422 2f3e 3c77 3a70 5072 3e3c 773a 696e  t"/><w:pPr><w:in
-00001c10: 6420 773a 6c65 6674 3d22 3732 3022 2077  d w:left="720" w
-00001c20: 3a68 616e 6769 6e67 3d22 3336 3022 2f3e  :hanging="360"/>
-00001c30: 3c2f 773a 7050 723e 3c77 3a72 5072 3e3c  </w:pPr><w:rPr><
-00001c40: 773a 7246 6f6e 7473 2077 3a61 7363 6969  w:rFonts w:ascii
-00001c50: 3d22 5379 6d62 6f6c 2220 773a 6841 6e73  ="Symbol" w:hAns
-00001c60: 693d 2253 796d 626f 6c22 2077 3a68 696e  i="Symbol" w:hin
-00001c70: 743d 2264 6566 6175 6c74 222f 3e3c 2f77  t="default"/></w
-00001c80: 3a72 5072 3e3c 2f77 3a6c 766c 3e3c 773a  :rPr></w:lvl><w:
-00001c90: 6c76 6c20 773a 696c 766c 3d22 3122 2077  lvl w:ilvl="1" w
-00001ca0: 3a74 706c 633d 2232 3030 3030 3030 3322  :tplc="20000003"
-00001cb0: 2077 3a74 656e 7461 7469 7665 3d22 3122   w:tentative="1"
-00001cc0: 3e3c 773a 7374 6172 7420 773a 7661 6c3d  ><w:start w:val=
-00001cd0: 2231 222f 3e3c 773a 6e75 6d46 6d74 2077  "1"/><w:numFmt w
-00001ce0: 3a76 616c 3d22 6275 6c6c 6574 222f 3e3c  :val="bullet"/><
-00001cf0: 773a 6c76 6c54 6578 7420 773a 7661 6c3d  w:lvlText w:val=
-00001d00: 226f 222f 3e3c 773a 6c76 6c4a 6320 773a  "o"/><w:lvlJc w:
-00001d10: 7661 6c3d 226c 6566 7422 2f3e 3c77 3a70  val="left"/><w:p
-00001d20: 5072 3e3c 773a 696e 6420 773a 6c65 6674  Pr><w:ind w:left
-00001d30: 3d22 3134 3430 2220 773a 6861 6e67 696e  ="1440" w:hangin
-00001d40: 673d 2233 3630 222f 3e3c 2f77 3a70 5072  g="360"/></w:pPr
-00001d50: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
-00001d60: 7320 773a 6173 6369 693d 2243 6f75 7269  s w:ascii="Couri
-00001d70: 6572 204e 6577 2220 773a 6841 6e73 693d  er New" w:hAnsi=
-00001d80: 2243 6f75 7269 6572 204e 6577 2220 773a  "Courier New" w:
-00001d90: 6373 3d22 436f 7572 6965 7220 4e65 7722  cs="Courier New"
-00001da0: 2077 3a68 696e 743d 2264 6566 6175 6c74   w:hint="default
-00001db0: 222f 3e3c 2f77 3a72 5072 3e3c 2f77 3a6c  "/></w:rPr></w:l
-00001dc0: 766c 3e3c 773a 6c76 6c20 773a 696c 766c  vl><w:lvl w:ilvl
-00001dd0: 3d22 3222 2077 3a74 706c 633d 2232 3030  ="2" w:tplc="200
-00001de0: 3030 3030 3522 2077 3a74 656e 7461 7469  00005" w:tentati
-00001df0: 7665 3d22 3122 3e3c 773a 7374 6172 7420  ve="1"><w:start 
-00001e00: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
-00001e10: 6d46 6d74 2077 3a76 616c 3d22 6275 6c6c  mFmt w:val="bull
-00001e20: 6574 222f 3e3c 773a 6c76 6c54 6578 7420  et"/><w:lvlText 
-00001e30: 773a 7661 6c3d 22ef 82a7 222f 3e3c 773a  w:val="..."/><w:
-00001e40: 6c76 6c4a 6320 773a 7661 6c3d 226c 6566  lvlJc w:val="lef
-00001e50: 7422 2f3e 3c77 3a70 5072 3e3c 773a 696e  t"/><w:pPr><w:in
-00001e60: 6420 773a 6c65 6674 3d22 3231 3630 2220  d w:left="2160" 
-00001e70: 773a 6861 6e67 696e 673d 2233 3630 222f  w:hanging="360"/
-00001e80: 3e3c 2f77 3a70 5072 3e3c 773a 7250 723e  ></w:pPr><w:rPr>
-00001e90: 3c77 3a72 466f 6e74 7320 773a 6173 6369  <w:rFonts w:asci
-00001ea0: 693d 2257 696e 6764 696e 6773 2220 773a  i="Wingdings" w:
-00001eb0: 6841 6e73 693d 2257 696e 6764 696e 6773  hAnsi="Wingdings
-00001ec0: 2220 773a 6869 6e74 3d22 6465 6661 756c  " w:hint="defaul
-00001ed0: 7422 2f3e 3c2f 773a 7250 723e 3c2f 773a  t"/></w:rPr></w:
-00001ee0: 6c76 6c3e 3c77 3a6c 766c 2077 3a69 6c76  lvl><w:lvl w:ilv
-00001ef0: 6c3d 2233 2220 773a 7470 6c63 3d22 3230  l="3" w:tplc="20
-00001f00: 3030 3030 3031 2220 773a 7465 6e74 6174  000001" w:tentat
-00001f10: 6976 653d 2231 223e 3c77 3a73 7461 7274  ive="1"><w:start
-00001f20: 2077 3a76 616c 3d22 3122 2f3e 3c77 3a6e   w:val="1"/><w:n
-00001f30: 756d 466d 7420 773a 7661 6c3d 2262 756c  umFmt w:val="bul
-00001f40: 6c65 7422 2f3e 3c77 3a6c 766c 5465 7874  let"/><w:lvlText
-00001f50: 2077 3a76 616c 3d22 ef82 b722 2f3e 3c77   w:val="..."/><w
-00001f60: 3a6c 766c 4a63 2077 3a76 616c 3d22 6c65  :lvlJc w:val="le
-00001f70: 6674 222f 3e3c 773a 7050 723e 3c77 3a69  ft"/><w:pPr><w:i
-00001f80: 6e64 2077 3a6c 6566 743d 2232 3838 3022  nd w:left="2880"
-00001f90: 2077 3a68 616e 6769 6e67 3d22 3336 3022   w:hanging="360"
-00001fa0: 2f3e 3c2f 773a 7050 723e 3c77 3a72 5072  /></w:pPr><w:rPr
-00001fb0: 3e3c 773a 7246 6f6e 7473 2077 3a61 7363  ><w:rFonts w:asc
-00001fc0: 6969 3d22 5379 6d62 6f6c 2220 773a 6841  ii="Symbol" w:hA
-00001fd0: 6e73 693d 2253 796d 626f 6c22 2077 3a68  nsi="Symbol" w:h
-00001fe0: 696e 743d 2264 6566 6175 6c74 222f 3e3c  int="default"/><
-00001ff0: 2f77 3a72 5072 3e3c 2f77 3a6c 766c 3e3c  /w:rPr></w:lvl><
-00002000: 773a 6c76 6c20 773a 696c 766c 3d22 3422  w:lvl w:ilvl="4"
-00002010: 2077 3a74 706c 633d 2232 3030 3030 3030   w:tplc="2000000
-00002020: 3322 2077 3a74 656e 7461 7469 7665 3d22  3" w:tentative="
-00002030: 3122 3e3c 773a 7374 6172 7420 773a 7661  1"><w:start w:va
-00002040: 6c3d 2231 222f 3e3c 773a 6e75 6d46 6d74  l="1"/><w:numFmt
-00002050: 2077 3a76 616c 3d22 6275 6c6c 6574 222f   w:val="bullet"/
-00002060: 3e3c 773a 6c76 6c54 6578 7420 773a 7661  ><w:lvlText w:va
-00002070: 6c3d 226f 222f 3e3c 773a 6c76 6c4a 6320  l="o"/><w:lvlJc 
-00002080: 773a 7661 6c3d 226c 6566 7422 2f3e 3c77  w:val="left"/><w
-00002090: 3a70 5072 3e3c 773a 696e 6420 773a 6c65  :pPr><w:ind w:le
-000020a0: 6674 3d22 3336 3030 2220 773a 6861 6e67  ft="3600" w:hang
-000020b0: 696e 673d 2233 3630 222f 3e3c 2f77 3a70  ing="360"/></w:p
-000020c0: 5072 3e3c 773a 7250 723e 3c77 3a72 466f  Pr><w:rPr><w:rFo
-000020d0: 6e74 7320 773a 6173 6369 693d 2243 6f75  nts w:ascii="Cou
-000020e0: 7269 6572 204e 6577 2220 773a 6841 6e73  rier New" w:hAns
-000020f0: 693d 2243 6f75 7269 6572 204e 6577 2220  i="Courier New" 
-00002100: 773a 6373 3d22 436f 7572 6965 7220 4e65  w:cs="Courier Ne
-00002110: 7722 2077 3a68 696e 743d 2264 6566 6175  w" w:hint="defau
-00002120: 6c74 222f 3e3c 2f77 3a72 5072 3e3c 2f77  lt"/></w:rPr></w
-00002130: 3a6c 766c 3e3c 773a 6c76 6c20 773a 696c  :lvl><w:lvl w:il
-00002140: 766c 3d22 3522 2077 3a74 706c 633d 2232  vl="5" w:tplc="2
-00002150: 3030 3030 3030 3522 2077 3a74 656e 7461  0000005" w:tenta
-00002160: 7469 7665 3d22 3122 3e3c 773a 7374 6172  tive="1"><w:star
-00002170: 7420 773a 7661 6c3d 2231 222f 3e3c 773a  t w:val="1"/><w:
-00002180: 6e75 6d46 6d74 2077 3a76 616c 3d22 6275  numFmt w:val="bu
-00002190: 6c6c 6574 222f 3e3c 773a 6c76 6c54 6578  llet"/><w:lvlTex
-000021a0: 7420 773a 7661 6c3d 22ef 82a7 222f 3e3c  t w:val="..."/><
-000021b0: 773a 6c76 6c4a 6320 773a 7661 6c3d 226c  w:lvlJc w:val="l
-000021c0: 6566 7422 2f3e 3c77 3a70 5072 3e3c 773a  eft"/><w:pPr><w:
-000021d0: 696e 6420 773a 6c65 6674 3d22 3433 3230  ind w:left="4320
-000021e0: 2220 773a 6861 6e67 696e 673d 2233 3630  " w:hanging="360
-000021f0: 222f 3e3c 2f77 3a70 5072 3e3c 773a 7250  "/></w:pPr><w:rP
-00002200: 723e 3c77 3a72 466f 6e74 7320 773a 6173  r><w:rFonts w:as
-00002210: 6369 693d 2257 696e 6764 696e 6773 2220  cii="Wingdings" 
-00002220: 773a 6841 6e73 693d 2257 696e 6764 696e  w:hAnsi="Wingdin
-00002230: 6773 2220 773a 6869 6e74 3d22 6465 6661  gs" w:hint="defa
-00002240: 756c 7422 2f3e 3c2f 773a 7250 723e 3c2f  ult"/></w:rPr></
-00002250: 773a 6c76 6c3e 3c77 3a6c 766c 2077 3a69  w:lvl><w:lvl w:i
-00002260: 6c76 6c3d 2236 2220 773a 7470 6c63 3d22  lvl="6" w:tplc="
-00002270: 3230 3030 3030 3031 2220 773a 7465 6e74  20000001" w:tent
-00002280: 6174 6976 653d 2231 223e 3c77 3a73 7461  ative="1"><w:sta
-00002290: 7274 2077 3a76 616c 3d22 3122 2f3e 3c77  rt w:val="1"/><w
-000022a0: 3a6e 756d 466d 7420 773a 7661 6c3d 2262  :numFmt w:val="b
-000022b0: 756c 6c65 7422 2f3e 3c77 3a6c 766c 5465  ullet"/><w:lvlTe
-000022c0: 7874 2077 3a76 616c 3d22 ef82 b722 2f3e  xt w:val="..."/>
-000022d0: 3c77 3a6c 766c 4a63 2077 3a76 616c 3d22  <w:lvlJc w:val="
-000022e0: 6c65 6674 222f 3e3c 773a 7050 723e 3c77  left"/><w:pPr><w
-000022f0: 3a69 6e64 2077 3a6c 6566 743d 2235 3034  :ind w:left="504
-00002300: 3022 2077 3a68 616e 6769 6e67 3d22 3336  0" w:hanging="36
-00002310: 3022 2f3e 3c2f 773a 7050 723e 3c77 3a72  0"/></w:pPr><w:r
-00002320: 5072 3e3c 773a 7246 6f6e 7473 2077 3a61  Pr><w:rFonts w:a
-00002330: 7363 6969 3d22 5379 6d62 6f6c 2220 773a  scii="Symbol" w:
-00002340: 6841 6e73 693d 2253 796d 626f 6c22 2077  hAnsi="Symbol" w
-00002350: 3a68 696e 743d 2264 6566 6175 6c74 222f  :hint="default"/
-00002360: 3e3c 2f77 3a72 5072 3e3c 2f77 3a6c 766c  ></w:rPr></w:lvl
-00002370: 3e3c 773a 6c76 6c20 773a 696c 766c 3d22  ><w:lvl w:ilvl="
-00002380: 3722 2077 3a74 706c 633d 2232 3030 3030  7" w:tplc="20000
-00002390: 3030 3322 2077 3a74 656e 7461 7469 7665  003" w:tentative
-000023a0: 3d22 3122 3e3c 773a 7374 6172 7420 773a  ="1"><w:start w:
-000023b0: 7661 6c3d 2231 222f 3e3c 773a 6e75 6d46  val="1"/><w:numF
-000023c0: 6d74 2077 3a76 616c 3d22 6275 6c6c 6574  mt w:val="bullet
-000023d0: 222f 3e3c 773a 6c76 6c54 6578 7420 773a  "/><w:lvlText w:
-000023e0: 7661 6c3d 226f 222f 3e3c 773a 6c76 6c4a  val="o"/><w:lvlJ
-000023f0: 6320 773a 7661 6c3d 226c 6566 7422 2f3e  c w:val="left"/>
-00002400: 3c77 3a70 5072 3e3c 773a 696e 6420 773a  <w:pPr><w:ind w:
-00002410: 6c65 6674 3d22 3537 3630 2220 773a 6861  left="5760" w:ha
-00002420: 6e67 696e 673d 2233 3630 222f 3e3c 2f77  nging="360"/></w
-00002430: 3a70 5072 3e3c 773a 7250 723e 3c77 3a72  :pPr><w:rPr><w:r
-00002440: 466f 6e74 7320 773a 6173 6369 693d 2243  Fonts w:ascii="C
-00002450: 6f75 7269 6572 204e 6577 2220 773a 6841  ourier New" w:hA
-00002460: 6e73 693d 2243 6f75 7269 6572 204e 6577  nsi="Courier New
-00002470: 2220 773a 6373 3d22 436f 7572 6965 7220  " w:cs="Courier 
-00002480: 4e65 7722 2077 3a68 696e 743d 2264 6566  New" w:hint="def
-00002490: 6175 6c74 222f 3e3c 2f77 3a72 5072 3e3c  ault"/></w:rPr><
-000024a0: 2f77 3a6c 766c 3e3c 773a 6c76 6c20 773a  /w:lvl><w:lvl w:
-000024b0: 696c 766c 3d22 3822 2077 3a74 706c 633d  ilvl="8" w:tplc=
-000024c0: 2232 3030 3030 3030 3522 2077 3a74 656e  "20000005" w:ten
-000024d0: 7461 7469 7665 3d22 3122 3e3c 773a 7374  tative="1"><w:st
-000024e0: 6172 7420 773a 7661 6c3d 2231 222f 3e3c  art w:val="1"/><
-000024f0: 773a 6e75 6d46 6d74 2077 3a76 616c 3d22  w:numFmt w:val="
-00002500: 6275 6c6c 6574 222f 3e3c 773a 6c76 6c54  bullet"/><w:lvlT
-00002510: 6578 7420 773a 7661 6c3d 22ef 82a7 222f  ext w:val="..."/
-00002520: 3e3c 773a 6c76 6c4a 6320 773a 7661 6c3d  ><w:lvlJc w:val=
-00002530: 226c 6566 7422 2f3e 3c77 3a70 5072 3e3c  "left"/><w:pPr><
-00002540: 773a 696e 6420 773a 6c65 6674 3d22 3634  w:ind w:left="64
-00002550: 3830 2220 773a 6861 6e67 696e 673d 2233  80" w:hanging="3
-00002560: 3630 222f 3e3c 2f77 3a70 5072 3e3c 773a  60"/></w:pPr><w:
-00002570: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
-00002580: 6173 6369 693d 2257 696e 6764 696e 6773  ascii="Wingdings
-00002590: 2220 773a 6841 6e73 693d 2257 696e 6764  " w:hAnsi="Wingd
-000025a0: 696e 6773 2220 773a 6869 6e74 3d22 6465  ings" w:hint="de
-000025b0: 6661 756c 7422 2f3e 3c2f 773a 7250 723e  fault"/></w:rPr>
-000025c0: 3c2f 773a 6c76 6c3e 3c2f 773a 6162 7374  </w:lvl></w:abst
-000025d0: 7261 6374 4e75 6d3e 3c77 3a61 6273 7472  ractNum><w:abstr
-000025e0: 6163 744e 756d 2077 3a61 6273 7472 6163  actNum w:abstrac
-000025f0: 744e 756d 4964 3d22 3131 2220 7731 353a  tNumId="11" w15:
-00002600: 7265 7374 6172 744e 756d 6265 7269 6e67  restartNumbering
-00002610: 4166 7465 7242 7265 616b 3d22 3022 3e3c  AfterBreak="0"><
-00002620: 773a 6e73 6964 2077 3a76 616c 3d22 3346  w:nsid w:val="3F
-00002630: 4339 3533 4330 222f 3e3c 773a 6d75 6c74  C953C0"/><w:mult
-00002640: 694c 6576 656c 5479 7065 2077 3a76 616c  iLevelType w:val
-00002650: 3d22 6879 6272 6964 4d75 6c74 696c 6576  ="hybridMultilev
-00002660: 656c 222f 3e3c 773a 746d 706c 2077 3a76  el"/><w:tmpl w:v
-00002670: 616c 3d22 3730 3734 3741 3332 222f 3e3c  al="70747A32"/><
-00002680: 773a 6c76 6c20 773a 696c 766c 3d22 3022  w:lvl w:ilvl="0"
-00002690: 2077 3a74 706c 633d 2232 3030 3030 3030   w:tplc="2000000
-000026a0: 4622 3e3c 773a 7374 6172 7420 773a 7661  F"><w:start w:va
-000026b0: 6c3d 2231 222f 3e3c 773a 6e75 6d46 6d74  l="1"/><w:numFmt
-000026c0: 2077 3a76 616c 3d22 6465 6369 6d61 6c22   w:val="decimal"
-000026d0: 2f3e 3c77 3a6c 766c 5465 7874 2077 3a76  /><w:lvlText w:v
-000026e0: 616c 3d22 2531 2e22 2f3e 3c77 3a6c 766c  al="%1."/><w:lvl
-000026f0: 4a63 2077 3a76 616c 3d22 6c65 6674 222f  Jc w:val="left"/
-00002700: 3e3c 773a 7050 723e 3c77 3a69 6e64 2077  ><w:pPr><w:ind w
-00002710: 3a6c 6566 743d 2237 3230 2220 773a 6861  :left="720" w:ha
-00002720: 6e67 696e 673d 2233 3630 222f 3e3c 2f77  nging="360"/></w
-00002730: 3a70 5072 3e3c 2f77 3a6c 766c 3e3c 773a  :pPr></w:lvl><w:
-00002740: 6c76 6c20 773a 696c 766c 3d22 3122 2077  lvl w:ilvl="1" w
-00002750: 3a74 706c 633d 2232 3030 3030 3031 3922  :tplc="20000019"
-00002760: 3e3c 773a 7374 6172 7420 773a 7661 6c3d  ><w:start w:val=
-00002770: 2231 222f 3e3c 773a 6e75 6d46 6d74 2077  "1"/><w:numFmt w
-00002780: 3a76 616c 3d22 6c6f 7765 724c 6574 7465  :val="lowerLette
-00002790: 7222 2f3e 3c77 3a6c 766c 5465 7874 2077  r"/><w:lvlText w
-000027a0: 3a76 616c 3d22 2532 2e22 2f3e 3c77 3a6c  :val="%2."/><w:l
-000027b0: 766c 4a63 2077 3a76 616c 3d22 6c65 6674  vlJc w:val="left
-000027c0: 222f 3e3c 773a 7050 723e 3c77 3a69 6e64  "/><w:pPr><w:ind
-000027d0: 2077 3a6c 6566 743d 2231 3434 3022 2077   w:left="1440" w
-000027e0: 3a68 616e 6769 6e67 3d22 3336 3022 2f3e  :hanging="360"/>
-000027f0: 3c2f 773a 7050 723e 3c2f 773a 6c76 6c3e  </w:pPr></w:lvl>
-00002800: 3c77 3a6c 766c 2077 3a69 6c76 6c3d 2232  <w:lvl w:ilvl="2
-00002810: 2220 773a 7470 6c63 3d22 3230 3030 3030  " w:tplc="200000
-00002820: 3142 2220 773a 7465 6e74 6174 6976 653d  1B" w:tentative=
-00002830: 2231 223e 3c77 3a73 7461 7274 2077 3a76  "1"><w:start w:v
-00002840: 616c 3d22 3122 2f3e 3c77 3a6e 756d 466d  al="1"/><w:numFm
-00002850: 7420 773a 7661 6c3d 226c 6f77 6572 526f  t w:val="lowerRo
-00002860: 6d61 6e22 2f3e 3c77 3a6c 766c 5465 7874  man"/><w:lvlText
-00002870: 2077 3a76 616c 3d22 2533 2e22 2f3e 3c77   w:val="%3."/><w
-00002880: 3a6c 766c 4a63 2077 3a76 616c 3d22 7269  :lvlJc w:val="ri
-00002890: 6768 7422 2f3e 3c77 3a70 5072 3e3c 773a  ght"/><w:pPr><w:
-000028a0: 696e 6420 773a 6c65 6674 3d22 3231 3630  ind w:left="2160
-000028b0: 2220 773a 6861 6e67 696e 673d 2231 3830  " w:hanging="180
-000028c0: 222f 3e3c 2f77 3a70 5072 3e3c 2f77 3a6c  "/></w:pPr></w:l
-000028d0: 766c 3e3c 773a 6c76 6c20 773a 696c 766c  vl><w:lvl w:ilvl
-000028e0: 3d22 3322 2077 3a74 706c 633d 2232 3030  ="3" w:tplc="200
-000028f0: 3030 3030 4622 2077 3a74 656e 7461 7469  0000F" w:tentati
-00002900: 7665 3d22 3122 3e3c 773a 7374 6172 7420  ve="1"><w:start 
-00002910: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
-00002920: 6d46 6d74 2077 3a76 616c 3d22 6465 6369  mFmt w:val="deci
-00002930: 6d61 6c22 2f3e 3c77 3a6c 766c 5465 7874  mal"/><w:lvlText
-00002940: 2077 3a76 616c 3d22 2534 2e22 2f3e 3c77   w:val="%4."/><w
-00002950: 3a6c 766c 4a63 2077 3a76 616c 3d22 6c65  :lvlJc w:val="le
-00002960: 6674 222f 3e3c 773a 7050 723e 3c77 3a69  ft"/><w:pPr><w:i
-00002970: 6e64 2077 3a6c 6566 743d 2232 3838 3022  nd w:left="2880"
-00002980: 2077 3a68 616e 6769 6e67 3d22 3336 3022   w:hanging="360"
-00002990: 2f3e 3c2f 773a 7050 723e 3c2f 773a 6c76  /></w:pPr></w:lv
-000029a0: 6c3e 3c77 3a6c 766c 2077 3a69 6c76 6c3d  l><w:lvl w:ilvl=
-000029b0: 2234 2220 773a 7470 6c63 3d22 3230 3030  "4" w:tplc="2000
-000029c0: 3030 3139 2220 773a 7465 6e74 6174 6976  0019" w:tentativ
-000029d0: 653d 2231 223e 3c77 3a73 7461 7274 2077  e="1"><w:start w
-000029e0: 3a76 616c 3d22 3122 2f3e 3c77 3a6e 756d  :val="1"/><w:num
-000029f0: 466d 7420 773a 7661 6c3d 226c 6f77 6572  Fmt w:val="lower
-00002a00: 4c65 7474 6572 222f 3e3c 773a 6c76 6c54  Letter"/><w:lvlT
-00002a10: 6578 7420 773a 7661 6c3d 2225 352e 222f  ext w:val="%5."/
-00002a20: 3e3c 773a 6c76 6c4a 6320 773a 7661 6c3d  ><w:lvlJc w:val=
-00002a30: 226c 6566 7422 2f3e 3c77 3a70 5072 3e3c  "left"/><w:pPr><
-00002a40: 773a 696e 6420 773a 6c65 6674 3d22 3336  w:ind w:left="36
-00002a50: 3030 2220 773a 6861 6e67 696e 673d 2233  00" w:hanging="3
-00002a60: 3630 222f 3e3c 2f77 3a70 5072 3e3c 2f77  60"/></w:pPr></w
-00002a70: 3a6c 766c 3e3c 773a 6c76 6c20 773a 696c  :lvl><w:lvl w:il
-00002a80: 766c 3d22 3522 2077 3a74 706c 633d 2232  vl="5" w:tplc="2
-00002a90: 3030 3030 3031 4222 2077 3a74 656e 7461  000001B" w:tenta
-00002aa0: 7469 7665 3d22 3122 3e3c 773a 7374 6172  tive="1"><w:star
-00002ab0: 7420 773a 7661 6c3d 2231 222f 3e3c 773a  t w:val="1"/><w:
-00002ac0: 6e75 6d46 6d74 2077 3a76 616c 3d22 6c6f  numFmt w:val="lo
-00002ad0: 7765 7252 6f6d 616e 222f 3e3c 773a 6c76  werRoman"/><w:lv
-00002ae0: 6c54 6578 7420 773a 7661 6c3d 2225 362e  lText w:val="%6.
-00002af0: 222f 3e3c 773a 6c76 6c4a 6320 773a 7661  "/><w:lvlJc w:va
-00002b00: 6c3d 2272 6967 6874 222f 3e3c 773a 7050  l="right"/><w:pP
-00002b10: 723e 3c77 3a69 6e64 2077 3a6c 6566 743d  r><w:ind w:left=
-00002b20: 2234 3332 3022 2077 3a68 616e 6769 6e67  "4320" w:hanging
-00002b30: 3d22 3138 3022 2f3e 3c2f 773a 7050 723e  ="180"/></w:pPr>
-00002b40: 3c2f 773a 6c76 6c3e 3c77 3a6c 766c 2077  </w:lvl><w:lvl w
-00002b50: 3a69 6c76 6c3d 2236 2220 773a 7470 6c63  :ilvl="6" w:tplc
-00002b60: 3d22 3230 3030 3030 3046 2220 773a 7465  ="2000000F" w:te
-00002b70: 6e74 6174 6976 653d 2231 223e 3c77 3a73  ntative="1"><w:s
-00002b80: 7461 7274 2077 3a76 616c 3d22 3122 2f3e  tart w:val="1"/>
-00002b90: 3c77 3a6e 756d 466d 7420 773a 7661 6c3d  <w:numFmt w:val=
-00002ba0: 2264 6563 696d 616c 222f 3e3c 773a 6c76  "decimal"/><w:lv
-00002bb0: 6c54 6578 7420 773a 7661 6c3d 2225 372e  lText w:val="%7.
-00002bc0: 222f 3e3c 773a 6c76 6c4a 6320 773a 7661  "/><w:lvlJc w:va
-00002bd0: 6c3d 226c 6566 7422 2f3e 3c77 3a70 5072  l="left"/><w:pPr
-00002be0: 3e3c 773a 696e 6420 773a 6c65 6674 3d22  ><w:ind w:left="
-00002bf0: 3530 3430 2220 773a 6861 6e67 696e 673d  5040" w:hanging=
-00002c00: 2233 3630 222f 3e3c 2f77 3a70 5072 3e3c  "360"/></w:pPr><
-00002c10: 2f77 3a6c 766c 3e3c 773a 6c76 6c20 773a  /w:lvl><w:lvl w:
-00002c20: 696c 766c 3d22 3722 2077 3a74 706c 633d  ilvl="7" w:tplc=
-00002c30: 2232 3030 3030 3031 3922 2077 3a74 656e  "20000019" w:ten
-00002c40: 7461 7469 7665 3d22 3122 3e3c 773a 7374  tative="1"><w:st
-00002c50: 6172 7420 773a 7661 6c3d 2231 222f 3e3c  art w:val="1"/><
-00002c60: 773a 6e75 6d46 6d74 2077 3a76 616c 3d22  w:numFmt w:val="
-00002c70: 6c6f 7765 724c 6574 7465 7222 2f3e 3c77  lowerLetter"/><w
-00002c80: 3a6c 766c 5465 7874 2077 3a76 616c 3d22  :lvlText w:val="
-00002c90: 2538 2e22 2f3e 3c77 3a6c 766c 4a63 2077  %8."/><w:lvlJc w
-00002ca0: 3a76 616c 3d22 6c65 6674 222f 3e3c 773a  :val="left"/><w:
-00002cb0: 7050 723e 3c77 3a69 6e64 2077 3a6c 6566  pPr><w:ind w:lef
-00002cc0: 743d 2235 3736 3022 2077 3a68 616e 6769  t="5760" w:hangi
-00002cd0: 6e67 3d22 3336 3022 2f3e 3c2f 773a 7050  ng="360"/></w:pP
-00002ce0: 723e 3c2f 773a 6c76 6c3e 3c77 3a6c 766c  r></w:lvl><w:lvl
-00002cf0: 2077 3a69 6c76 6c3d 2238 2220 773a 7470   w:ilvl="8" w:tp
-00002d00: 6c63 3d22 3230 3030 3030 3142 2220 773a  lc="2000001B" w:
-00002d10: 7465 6e74 6174 6976 653d 2231 223e 3c77  tentative="1"><w
-00002d20: 3a73 7461 7274 2077 3a76 616c 3d22 3122  :start w:val="1"
-00002d30: 2f3e 3c77 3a6e 756d 466d 7420 773a 7661  /><w:numFmt w:va
-00002d40: 6c3d 226c 6f77 6572 526f 6d61 6e22 2f3e  l="lowerRoman"/>
-00002d50: 3c77 3a6c 766c 5465 7874 2077 3a76 616c  <w:lvlText w:val
-00002d60: 3d22 2539 2e22 2f3e 3c77 3a6c 766c 4a63  ="%9."/><w:lvlJc
-00002d70: 2077 3a76 616c 3d22 7269 6768 7422 2f3e   w:val="right"/>
-00002d80: 3c77 3a70 5072 3e3c 773a 696e 6420 773a  <w:pPr><w:ind w:
-00002d90: 6c65 6674 3d22 3634 3830 2220 773a 6861  left="6480" w:ha
-00002da0: 6e67 696e 673d 2231 3830 222f 3e3c 2f77  nging="180"/></w
-00002db0: 3a70 5072 3e3c 2f77 3a6c 766c 3e3c 2f77  :pPr></w:lvl></w
-00002dc0: 3a61 6273 7472 6163 744e 756d 3e3c 773a  :abstractNum><w:
-00002dd0: 6162 7374 7261 6374 4e75 6d20 773a 6162  abstractNum w:ab
-00002de0: 7374 7261 6374 4e75 6d49 643d 2231 3222  stractNumId="12"
-00002df0: 2077 3135 3a72 6573 7461 7274 4e75 6d62   w15:restartNumb
-00002e00: 6572 696e 6741 6674 6572 4272 6561 6b3d  eringAfterBreak=
-00002e10: 2230 223e 3c77 3a6e 7369 6420 773a 7661  "0"><w:nsid w:va
-00002e20: 6c3d 2236 4542 3134 3436 3822 2f3e 3c77  l="6EB14468"/><w
-00002e30: 3a6d 756c 7469 4c65 7665 6c54 7970 6520  :multiLevelType 
-00002e40: 773a 7661 6c3d 2268 7962 7269 644d 756c  w:val="hybridMul
-00002e50: 7469 6c65 7665 6c22 2f3e 3c77 3a74 6d70  tilevel"/><w:tmp
-00002e60: 6c20 773a 7661 6c3d 2233 4242 3442 4538  l w:val="3BB4BE8
-00002e70: 4122 2f3e 3c77 3a6c 766c 2077 3a69 6c76  A"/><w:lvl w:ilv
-00002e80: 6c3d 2230 2220 773a 7470 6c63 3d22 3230  l="0" w:tplc="20
-00002e90: 3030 3030 3031 223e 3c77 3a73 7461 7274  000001"><w:start
-00002ea0: 2077 3a76 616c 3d22 3122 2f3e 3c77 3a6e   w:val="1"/><w:n
-00002eb0: 756d 466d 7420 773a 7661 6c3d 2262 756c  umFmt w:val="bul
-00002ec0: 6c65 7422 2f3e 3c77 3a6c 766c 5465 7874  let"/><w:lvlText
-00002ed0: 2077 3a76 616c 3d22 ef82 b722 2f3e 3c77   w:val="..."/><w
-00002ee0: 3a6c 766c 4a63 2077 3a76 616c 3d22 6c65  :lvlJc w:val="le
-00002ef0: 6674 222f 3e3c 773a 7050 723e 3c77 3a69  ft"/><w:pPr><w:i
-00002f00: 6e64 2077 3a6c 6566 743d 2237 3230 2220  nd w:left="720" 
-00002f10: 773a 6861 6e67 696e 673d 2233 3630 222f  w:hanging="360"/
-00002f20: 3e3c 2f77 3a70 5072 3e3c 773a 7250 723e  ></w:pPr><w:rPr>
-00002f30: 3c77 3a72 466f 6e74 7320 773a 6173 6369  <w:rFonts w:asci
-00002f40: 693d 2253 796d 626f 6c22 2077 3a68 416e  i="Symbol" w:hAn
-00002f50: 7369 3d22 5379 6d62 6f6c 2220 773a 6869  si="Symbol" w:hi
-00002f60: 6e74 3d22 6465 6661 756c 7422 2f3e 3c2f  nt="default"/></
-00002f70: 773a 7250 723e 3c2f 773a 6c76 6c3e 3c77  w:rPr></w:lvl><w
-00002f80: 3a6c 766c 2077 3a69 6c76 6c3d 2231 2220  :lvl w:ilvl="1" 
-00002f90: 773a 7470 6c63 3d22 3230 3030 3030 3033  w:tplc="20000003
-00002fa0: 2220 773a 7465 6e74 6174 6976 653d 2231  " w:tentative="1
-00002fb0: 223e 3c77 3a73 7461 7274 2077 3a76 616c  "><w:start w:val
-00002fc0: 3d22 3122 2f3e 3c77 3a6e 756d 466d 7420  ="1"/><w:numFmt 
-00002fd0: 773a 7661 6c3d 2262 756c 6c65 7422 2f3e  w:val="bullet"/>
-00002fe0: 3c77 3a6c 766c 5465 7874 2077 3a76 616c  <w:lvlText w:val
-00002ff0: 3d22 6f22 2f3e 3c77 3a6c 766c 4a63 2077  ="o"/><w:lvlJc w
-00003000: 3a76 616c 3d22 6c65 6674 222f 3e3c 773a  :val="left"/><w:
-00003010: 7050 723e 3c77 3a69 6e64 2077 3a6c 6566  pPr><w:ind w:lef
-00003020: 743d 2231 3434 3022 2077 3a68 616e 6769  t="1440" w:hangi
-00003030: 6e67 3d22 3336 3022 2f3e 3c2f 773a 7050  ng="360"/></w:pP
-00003040: 723e 3c77 3a72 5072 3e3c 773a 7246 6f6e  r><w:rPr><w:rFon
-00003050: 7473 2077 3a61 7363 6969 3d22 436f 7572  ts w:ascii="Cour
-00003060: 6965 7220 4e65 7722 2077 3a68 416e 7369  ier New" w:hAnsi
-00003070: 3d22 436f 7572 6965 7220 4e65 7722 2077  ="Courier New" w
-00003080: 3a63 733d 2243 6f75 7269 6572 204e 6577  :cs="Courier New
-00003090: 2220 773a 6869 6e74 3d22 6465 6661 756c  " w:hint="defaul
-000030a0: 7422 2f3e 3c2f 773a 7250 723e 3c2f 773a  t"/></w:rPr></w:
-000030b0: 6c76 6c3e 3c77 3a6c 766c 2077 3a69 6c76  lvl><w:lvl w:ilv
-000030c0: 6c3d 2232 2220 773a 7470 6c63 3d22 3230  l="2" w:tplc="20
-000030d0: 3030 3030 3035 2220 773a 7465 6e74 6174  000005" w:tentat
-000030e0: 6976 653d 2231 223e 3c77 3a73 7461 7274  ive="1"><w:start
-000030f0: 2077 3a76 616c 3d22 3122 2f3e 3c77 3a6e   w:val="1"/><w:n
-00003100: 756d 466d 7420 773a 7661 6c3d 2262 756c  umFmt w:val="bul
-00003110: 6c65 7422 2f3e 3c77 3a6c 766c 5465 7874  let"/><w:lvlText
-00003120: 2077 3a76 616c 3d22 ef82 a722 2f3e 3c77   w:val="..."/><w
-00003130: 3a6c 766c 4a63 2077 3a76 616c 3d22 6c65  :lvlJc w:val="le
-00003140: 6674 222f 3e3c 773a 7050 723e 3c77 3a69  ft"/><w:pPr><w:i
-00003150: 6e64 2077 3a6c 6566 743d 2232 3136 3022  nd w:left="2160"
-00003160: 2077 3a68 616e 6769 6e67 3d22 3336 3022   w:hanging="360"
-00003170: 2f3e 3c2f 773a 7050 723e 3c77 3a72 5072  /></w:pPr><w:rPr
-00003180: 3e3c 773a 7246 6f6e 7473 2077 3a61 7363  ><w:rFonts w:asc
-00003190: 6969 3d22 5769 6e67 6469 6e67 7322 2077  ii="Wingdings" w
-000031a0: 3a68 416e 7369 3d22 5769 6e67 6469 6e67  :hAnsi="Wingding
-000031b0: 7322 2077 3a68 696e 743d 2264 6566 6175  s" w:hint="defau
-000031c0: 6c74 222f 3e3c 2f77 3a72 5072 3e3c 2f77  lt"/></w:rPr></w
-000031d0: 3a6c 766c 3e3c 773a 6c76 6c20 773a 696c  :lvl><w:lvl w:il
-000031e0: 766c 3d22 3322 2077 3a74 706c 633d 2232  vl="3" w:tplc="2
-000031f0: 3030 3030 3030 3122 2077 3a74 656e 7461  0000001" w:tenta
-00003200: 7469 7665 3d22 3122 3e3c 773a 7374 6172  tive="1"><w:star
-00003210: 7420 773a 7661 6c3d 2231 222f 3e3c 773a  t w:val="1"/><w:
-00003220: 6e75 6d46 6d74 2077 3a76 616c 3d22 6275  numFmt w:val="bu
-00003230: 6c6c 6574 222f 3e3c 773a 6c76 6c54 6578  llet"/><w:lvlTex
-00003240: 7420 773a 7661 6c3d 22ef 82b7 222f 3e3c  t w:val="..."/><
-00003250: 773a 6c76 6c4a 6320 773a 7661 6c3d 226c  w:lvlJc w:val="l
-00003260: 6566 7422 2f3e 3c77 3a70 5072 3e3c 773a  eft"/><w:pPr><w:
-00003270: 696e 6420 773a 6c65 6674 3d22 3238 3830  ind w:left="2880
-00003280: 2220 773a 6861 6e67 696e 673d 2233 3630  " w:hanging="360
-00003290: 222f 3e3c 2f77 3a70 5072 3e3c 773a 7250  "/></w:pPr><w:rP
-000032a0: 723e 3c77 3a72 466f 6e74 7320 773a 6173  r><w:rFonts w:as
-000032b0: 6369 693d 2253 796d 626f 6c22 2077 3a68  cii="Symbol" w:h
-000032c0: 416e 7369 3d22 5379 6d62 6f6c 2220 773a  Ansi="Symbol" w:
-000032d0: 6869 6e74 3d22 6465 6661 756c 7422 2f3e  hint="default"/>
-000032e0: 3c2f 773a 7250 723e 3c2f 773a 6c76 6c3e  </w:rPr></w:lvl>
-000032f0: 3c77 3a6c 766c 2077 3a69 6c76 6c3d 2234  <w:lvl w:ilvl="4
-00003300: 2220 773a 7470 6c63 3d22 3230 3030 3030  " w:tplc="200000
-00003310: 3033 2220 773a 7465 6e74 6174 6976 653d  03" w:tentative=
-00003320: 2231 223e 3c77 3a73 7461 7274 2077 3a76  "1"><w:start w:v
-00003330: 616c 3d22 3122 2f3e 3c77 3a6e 756d 466d  al="1"/><w:numFm
-00003340: 7420 773a 7661 6c3d 2262 756c 6c65 7422  t w:val="bullet"
-00003350: 2f3e 3c77 3a6c 766c 5465 7874 2077 3a76  /><w:lvlText w:v
-00003360: 616c 3d22 6f22 2f3e 3c77 3a6c 766c 4a63  al="o"/><w:lvlJc
-00003370: 2077 3a76 616c 3d22 6c65 6674 222f 3e3c   w:val="left"/><
-00003380: 773a 7050 723e 3c77 3a69 6e64 2077 3a6c  w:pPr><w:ind w:l
-00003390: 6566 743d 2233 3630 3022 2077 3a68 616e  eft="3600" w:han
-000033a0: 6769 6e67 3d22 3336 3022 2f3e 3c2f 773a  ging="360"/></w:
-000033b0: 7050 723e 3c77 3a72 5072 3e3c 773a 7246  pPr><w:rPr><w:rF
-000033c0: 6f6e 7473 2077 3a61 7363 6969 3d22 436f  onts w:ascii="Co
-000033d0: 7572 6965 7220 4e65 7722 2077 3a68 416e  urier New" w:hAn
-000033e0: 7369 3d22 436f 7572 6965 7220 4e65 7722  si="Courier New"
-000033f0: 2077 3a63 733d 2243 6f75 7269 6572 204e   w:cs="Courier N
-00003400: 6577 2220 773a 6869 6e74 3d22 6465 6661  ew" w:hint="defa
-00003410: 756c 7422 2f3e 3c2f 773a 7250 723e 3c2f  ult"/></w:rPr></
-00003420: 773a 6c76 6c3e 3c77 3a6c 766c 2077 3a69  w:lvl><w:lvl w:i
-00003430: 6c76 6c3d 2235 2220 773a 7470 6c63 3d22  lvl="5" w:tplc="
-00003440: 3230 3030 3030 3035 2220 773a 7465 6e74  20000005" w:tent
-00003450: 6174 6976 653d 2231 223e 3c77 3a73 7461  ative="1"><w:sta
-00003460: 7274 2077 3a76 616c 3d22 3122 2f3e 3c77  rt w:val="1"/><w
-00003470: 3a6e 756d 466d 7420 773a 7661 6c3d 2262  :numFmt w:val="b
-00003480: 756c 6c65 7422 2f3e 3c77 3a6c 766c 5465  ullet"/><w:lvlTe
-00003490: 7874 2077 3a76 616c 3d22 ef82 a722 2f3e  xt w:val="..."/>
-000034a0: 3c77 3a6c 766c 4a63 2077 3a76 616c 3d22  <w:lvlJc w:val="
-000034b0: 6c65 6674 222f 3e3c 773a 7050 723e 3c77  left"/><w:pPr><w
-000034c0: 3a69 6e64 2077 3a6c 6566 743d 2234 3332  :ind w:left="432
-000034d0: 3022 2077 3a68 616e 6769 6e67 3d22 3336  0" w:hanging="36
-000034e0: 3022 2f3e 3c2f 773a 7050 723e 3c77 3a72  0"/></w:pPr><w:r
-000034f0: 5072 3e3c 773a 7246 6f6e 7473 2077 3a61  Pr><w:rFonts w:a
-00003500: 7363 6969 3d22 5769 6e67 6469 6e67 7322  scii="Wingdings"
-00003510: 2077 3a68 416e 7369 3d22 5769 6e67 6469   w:hAnsi="Wingdi
-00003520: 6e67 7322 2077 3a68 696e 743d 2264 6566  ngs" w:hint="def
-00003530: 6175 6c74 222f 3e3c 2f77 3a72 5072 3e3c  ault"/></w:rPr><
-00003540: 2f77 3a6c 766c 3e3c 773a 6c76 6c20 773a  /w:lvl><w:lvl w:
-00003550: 696c 766c 3d22 3622 2077 3a74 706c 633d  ilvl="6" w:tplc=
-00003560: 2232 3030 3030 3030 3122 2077 3a74 656e  "20000001" w:ten
-00003570: 7461 7469 7665 3d22 3122 3e3c 773a 7374  tative="1"><w:st
-00003580: 6172 7420 773a 7661 6c3d 2231 222f 3e3c  art w:val="1"/><
-00003590: 773a 6e75 6d46 6d74 2077 3a76 616c 3d22  w:numFmt w:val="
-000035a0: 6275 6c6c 6574 222f 3e3c 773a 6c76 6c54  bullet"/><w:lvlT
-000035b0: 6578 7420 773a 7661 6c3d 22ef 82b7 222f  ext w:val="..."/
-000035c0: 3e3c 773a 6c76 6c4a 6320 773a 7661 6c3d  ><w:lvlJc w:val=
-000035d0: 226c 6566 7422 2f3e 3c77 3a70 5072 3e3c  "left"/><w:pPr><
-000035e0: 773a 696e 6420 773a 6c65 6674 3d22 3530  w:ind w:left="50
-000035f0: 3430 2220 773a 6861 6e67 696e 673d 2233  40" w:hanging="3
-00003600: 3630 222f 3e3c 2f77 3a70 5072 3e3c 773a  60"/></w:pPr><w:
-00003610: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
-00003620: 6173 6369 693d 2253 796d 626f 6c22 2077  ascii="Symbol" w
-00003630: 3a68 416e 7369 3d22 5379 6d62 6f6c 2220  :hAnsi="Symbol" 
-00003640: 773a 6869 6e74 3d22 6465 6661 756c 7422  w:hint="default"
-00003650: 2f3e 3c2f 773a 7250 723e 3c2f 773a 6c76  /></w:rPr></w:lv
-00003660: 6c3e 3c77 3a6c 766c 2077 3a69 6c76 6c3d  l><w:lvl w:ilvl=
-00003670: 2237 2220 773a 7470 6c63 3d22 3230 3030  "7" w:tplc="2000
-00003680: 3030 3033 2220 773a 7465 6e74 6174 6976  0003" w:tentativ
-00003690: 653d 2231 223e 3c77 3a73 7461 7274 2077  e="1"><w:start w
-000036a0: 3a76 616c 3d22 3122 2f3e 3c77 3a6e 756d  :val="1"/><w:num
-000036b0: 466d 7420 773a 7661 6c3d 2262 756c 6c65  Fmt w:val="bulle
-000036c0: 7422 2f3e 3c77 3a6c 766c 5465 7874 2077  t"/><w:lvlText w
-000036d0: 3a76 616c 3d22 6f22 2f3e 3c77 3a6c 766c  :val="o"/><w:lvl
-000036e0: 4a63 2077 3a76 616c 3d22 6c65 6674 222f  Jc w:val="left"/
-000036f0: 3e3c 773a 7050 723e 3c77 3a69 6e64 2077  ><w:pPr><w:ind w
-00003700: 3a6c 6566 743d 2235 3736 3022 2077 3a68  :left="5760" w:h
-00003710: 616e 6769 6e67 3d22 3336 3022 2f3e 3c2f  anging="360"/></
-00003720: 773a 7050 723e 3c77 3a72 5072 3e3c 773a  w:pPr><w:rPr><w:
-00003730: 7246 6f6e 7473 2077 3a61 7363 6969 3d22  rFonts w:ascii="
-00003740: 436f 7572 6965 7220 4e65 7722 2077 3a68  Courier New" w:h
-00003750: 416e 7369 3d22 436f 7572 6965 7220 4e65  Ansi="Courier Ne
-00003760: 7722 2077 3a63 733d 2243 6f75 7269 6572  w" w:cs="Courier
-00003770: 204e 6577 2220 773a 6869 6e74 3d22 6465   New" w:hint="de
-00003780: 6661 756c 7422 2f3e 3c2f 773a 7250 723e  fault"/></w:rPr>
-00003790: 3c2f 773a 6c76 6c3e 3c77 3a6c 766c 2077  </w:lvl><w:lvl w
-000037a0: 3a69 6c76 6c3d 2238 2220 773a 7470 6c63  :ilvl="8" w:tplc
-000037b0: 3d22 3230 3030 3030 3035 2220 773a 7465  ="20000005" w:te
-000037c0: 6e74 6174 6976 653d 2231 223e 3c77 3a73  ntative="1"><w:s
-000037d0: 7461 7274 2077 3a76 616c 3d22 3122 2f3e  tart w:val="1"/>
-000037e0: 3c77 3a6e 756d 466d 7420 773a 7661 6c3d  <w:numFmt w:val=
-000037f0: 2262 756c 6c65 7422 2f3e 3c77 3a6c 766c  "bullet"/><w:lvl
-00003800: 5465 7874 2077 3a76 616c 3d22 ef82 a722  Text w:val="..."
-00003810: 2f3e 3c77 3a6c 766c 4a63 2077 3a76 616c  /><w:lvlJc w:val
-00003820: 3d22 6c65 6674 222f 3e3c 773a 7050 723e  ="left"/><w:pPr>
-00003830: 3c77 3a69 6e64 2077 3a6c 6566 743d 2236  <w:ind w:left="6
-00003840: 3438 3022 2077 3a68 616e 6769 6e67 3d22  480" w:hanging="
-00003850: 3336 3022 2f3e 3c2f 773a 7050 723e 3c77  360"/></w:pPr><w
-00003860: 3a72 5072 3e3c 773a 7246 6f6e 7473 2077  :rPr><w:rFonts w
-00003870: 3a61 7363 6969 3d22 5769 6e67 6469 6e67  :ascii="Wingding
-00003880: 7322 2077 3a68 416e 7369 3d22 5769 6e67  s" w:hAnsi="Wing
-00003890: 6469 6e67 7322 2077 3a68 696e 743d 2264  dings" w:hint="d
-000038a0: 6566 6175 6c74 222f 3e3c 2f77 3a72 5072  efault"/></w:rPr
-000038b0: 3e3c 2f77 3a6c 766c 3e3c 2f77 3a61 6273  ></w:lvl></w:abs
-000038c0: 7472 6163 744e 756d 3e3c 773a 6e75 6d20  tractNum><w:num 
-000038d0: 773a 6e75 6d49 643d 2231 2220 7731 3663  w:numId="1" w16c
-000038e0: 6964 3a64 7572 6162 6c65 4964 3d22 3337  id:durableId="37
-000038f0: 3232 3733 3631 3522 3e3c 773a 6162 7374  2273615"><w:abst
-00003900: 7261 6374 4e75 6d49 6420 773a 7661 6c3d  ractNumId w:val=
-00003910: 2231 3222 2f3e 3c2f 773a 6e75 6d3e 3c77  "12"/></w:num><w
-00003920: 3a6e 756d 2077 3a6e 756d 4964 3d22 3222  :num w:numId="2"
-00003930: 2077 3136 6369 643a 6475 7261 626c 6549   w16cid:durableI
-00003940: 643d 2231 3636 3035 3737 3735 3322 3e3c  d="1660577753"><
-00003950: 773a 6162 7374 7261 6374 4e75 6d49 6420  w:abstractNumId 
-00003960: 773a 7661 6c3d 2231 3122 2f3e 3c2f 773a  w:val="11"/></w:
-00003970: 6e75 6d3e 3c77 3a6e 756d 2077 3a6e 756d  num><w:num w:num
-00003980: 4964 3d22 3322 2077 3136 6369 643a 6475  Id="3" w16cid:du
-00003990: 7261 626c 6549 643d 2231 3932 3336 3431  rableId="1923641
-000039a0: 3832 3722 3e3c 773a 6162 7374 7261 6374  827"><w:abstract
-000039b0: 4e75 6d49 6420 773a 7661 6c3d 2239 222f  NumId w:val="9"/
-000039c0: 3e3c 2f77 3a6e 756d 3e3c 773a 6e75 6d20  ></w:num><w:num 
-000039d0: 773a 6e75 6d49 643d 2234 2220 7731 3663  w:numId="4" w16c
-000039e0: 6964 3a64 7572 6162 6c65 4964 3d22 3133  id:durableId="13
-000039f0: 3838 3338 3336 3737 223e 3c77 3a61 6273  88383677"><w:abs
-00003a00: 7472 6163 744e 756d 4964 2077 3a76 616c  tractNumId w:val
-00003a10: 3d22 3130 222f 3e3c 2f77 3a6e 756d 3e3c  ="10"/></w:num><
-00003a20: 773a 6e75 6d20 773a 6e75 6d49 643d 2235  w:num w:numId="5
-00003a30: 2220 7731 3663 6964 3a64 7572 6162 6c65  " w16cid:durable
-00003a40: 4964 3d22 3136 3132 3636 3431 3335 223e  Id="1612664135">
-00003a50: 3c77 3a61 6273 7472 6163 744e 756d 4964  <w:abstractNumId
-00003a60: 2077 3a76 616c 3d22 3722 2f3e 3c2f 773a   w:val="7"/></w:
-00003a70: 6e75 6d3e 3c77 3a6e 756d 2077 3a6e 756d  num><w:num w:num
-00003a80: 4964 3d22 3622 2077 3136 6369 643a 6475  Id="6" w16cid:du
-00003a90: 7261 626c 6549 643d 2231 3636 3532 3736  rableId="1665276
-00003aa0: 3433 3622 3e3c 773a 6162 7374 7261 6374  436"><w:abstract
-00003ab0: 4e75 6d49 6420 773a 7661 6c3d 2236 222f  NumId w:val="6"/
-00003ac0: 3e3c 2f77 3a6e 756d 3e3c 773a 6e75 6d20  ></w:num><w:num 
-00003ad0: 773a 6e75 6d49 643d 2237 2220 7731 3663  w:numId="7" w16c
-00003ae0: 6964 3a64 7572 6162 6c65 4964 3d22 3136  id:durableId="16
-00003af0: 3035 3936 3238 3437 223e 3c77 3a61 6273  05962847"><w:abs
-00003b00: 7472 6163 744e 756d 4964 2077 3a76 616c  tractNumId w:val
-00003b10: 3d22 3522 2f3e 3c2f 773a 6e75 6d3e 3c77  ="5"/></w:num><w
-00003b20: 3a6e 756d 2077 3a6e 756d 4964 3d22 3822  :num w:numId="8"
-00003b30: 2077 3136 6369 643a 6475 7261 626c 6549   w16cid:durableI
-00003b40: 643d 2236 3139 3333 3734 3733 223e 3c77  d="619337473"><w
-00003b50: 3a61 6273 7472 6163 744e 756d 4964 2077  :abstractNumId w
-00003b60: 3a76 616c 3d22 3422 2f3e 3c2f 773a 6e75  :val="4"/></w:nu
-00003b70: 6d3e 3c77 3a6e 756d 2077 3a6e 756d 4964  m><w:num w:numId
-00003b80: 3d22 3922 2077 3136 6369 643a 6475 7261  ="9" w16cid:dura
-00003b90: 626c 6549 643d 2232 3033 3832 3339 3536  bleId="203823956
-00003ba0: 3522 3e3c 773a 6162 7374 7261 6374 4e75  5"><w:abstractNu
-00003bb0: 6d49 6420 773a 7661 6c3d 2238 222f 3e3c  mId w:val="8"/><
-00003bc0: 2f77 3a6e 756d 3e3c 773a 6e75 6d20 773a  /w:num><w:num w:
-00003bd0: 6e75 6d49 643d 2231 3022 2077 3136 6369  numId="10" w16ci
-00003be0: 643a 6475 7261 626c 6549 643d 2231 3833  d:durableId="183
-00003bf0: 3832 3330 3531 3722 3e3c 773a 6162 7374  8230517"><w:abst
-00003c00: 7261 6374 4e75 6d49 6420 773a 7661 6c3d  ractNumId w:val=
-00003c10: 2233 222f 3e3c 2f77 3a6e 756d 3e3c 773a  "3"/></w:num><w:
-00003c20: 6e75 6d20 773a 6e75 6d49 643d 2231 3122  num w:numId="11"
-00003c30: 2077 3136 6369 643a 6475 7261 626c 6549   w16cid:durableI
-00003c40: 643d 2231 3633 3735 3633 3232 3222 3e3c  d="1637563222"><
-00003c50: 773a 6162 7374 7261 6374 4e75 6d49 6420  w:abstractNumId 
-00003c60: 773a 7661 6c3d 2232 222f 3e3c 2f77 3a6e  w:val="2"/></w:n
-00003c70: 756d 3e3c 773a 6e75 6d20 773a 6e75 6d49  um><w:num w:numI
-00003c80: 643d 2231 3222 2077 3136 6369 643a 6475  d="12" w16cid:du
-00003c90: 7261 626c 6549 643d 2237 3433 3435 3436  rableId="7434546
-00003ca0: 3939 223e 3c77 3a61 6273 7472 6163 744e  99"><w:abstractN
-00003cb0: 756d 4964 2077 3a76 616c 3d22 3122 2f3e  umId w:val="1"/>
-00003cc0: 3c2f 773a 6e75 6d3e 3c77 3a6e 756d 2077  </w:num><w:num w
-00003cd0: 3a6e 756d 4964 3d22 3133 2220 7731 3663  :numId="13" w16c
-00003ce0: 6964 3a64 7572 6162 6c65 4964 3d22 3432  id:durableId="42
-00003cf0: 3630 3532 3236 223e 3c77 3a61 6273 7472  605226"><w:abstr
-00003d00: 6163 744e 756d 4964 2077 3a76 616c 3d22  actNumId w:val="
-00003d10: 3022 2f3e 3c2f 773a 6e75 6d3e 3c2f 773a  0"/></w:num></w:
-00003d20: 6e75 6d62 6572 696e 673e                 numbering>
+00000030: 2279 6573 223f 3e0a 3c77 3a6e 756d 6265  "yes"?>.<w:numbe
+00000040: 7269 6e67 2078 6d6c 6e73 3a77 7063 3d22  ring xmlns:wpc="
+00000050: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
+00000060: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
+00000070: 6963 652f 776f 7264 2f32 3031 302f 776f  ice/word/2010/wo
+00000080: 7264 7072 6f63 6573 7369 6e67 4361 6e76  rdprocessingCanv
+00000090: 6173 2220 786d 6c6e 733a 6378 3d22 6874  as" xmlns:cx="ht
+000000a0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+000000b0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+000000c0: 652f 6472 6177 696e 672f 3230 3134 2f63  e/drawing/2014/c
+000000d0: 6861 7274 6578 2220 786d 6c6e 733a 6378  hartex" xmlns:cx
+000000e0: 313d 2268 7474 703a 2f2f 7363 6865 6d61  1="http://schema
+000000f0: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+00000100: 6f66 6669 6365 2f64 7261 7769 6e67 2f32  office/drawing/2
+00000110: 3031 352f 392f 382f 6368 6172 7465 7822  015/9/8/chartex"
+00000120: 2078 6d6c 6e73 3a63 7832 3d22 6874 7470   xmlns:cx2="http
+00000130: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
+00000140: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
+00000150: 6472 6177 696e 672f 3230 3135 2f31 302f  drawing/2015/10/
+00000160: 3231 2f63 6861 7274 6578 2220 786d 6c6e  21/chartex" xmln
+00000170: 733a 6378 333d 2268 7474 703a 2f2f 7363  s:cx3="http://sc
+00000180: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
+00000190: 636f 6d2f 6f66 6669 6365 2f64 7261 7769  com/office/drawi
+000001a0: 6e67 2f32 3031 362f 352f 392f 6368 6172  ng/2016/5/9/char
+000001b0: 7465 7822 2078 6d6c 6e73 3a63 7834 3d22  tex" xmlns:cx4="
+000001c0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
+000001d0: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
+000001e0: 6963 652f 6472 6177 696e 672f 3230 3136  ice/drawing/2016
+000001f0: 2f35 2f31 302f 6368 6172 7465 7822 2078  /5/10/chartex" x
+00000200: 6d6c 6e73 3a63 7835 3d22 6874 7470 3a2f  mlns:cx5="http:/
+00000210: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
+00000220: 6674 2e63 6f6d 2f6f 6666 6963 652f 6472  ft.com/office/dr
+00000230: 6177 696e 672f 3230 3136 2f35 2f31 312f  awing/2016/5/11/
+00000240: 6368 6172 7465 7822 2078 6d6c 6e73 3a63  chartex" xmlns:c
+00000250: 7836 3d22 6874 7470 3a2f 2f73 6368 656d  x6="http://schem
+00000260: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
+00000270: 2f6f 6666 6963 652f 6472 6177 696e 672f  /office/drawing/
+00000280: 3230 3136 2f35 2f31 322f 6368 6172 7465  2016/5/12/charte
+00000290: 7822 2078 6d6c 6e73 3a63 7837 3d22 6874  x" xmlns:cx7="ht
+000002a0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+000002b0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+000002c0: 652f 6472 6177 696e 672f 3230 3136 2f35  e/drawing/2016/5
+000002d0: 2f31 332f 6368 6172 7465 7822 2078 6d6c  /13/chartex" xml
+000002e0: 6e73 3a63 7838 3d22 6874 7470 3a2f 2f73  ns:cx8="http://s
+000002f0: 6368 656d 6173 2e6d 6963 726f 736f 6674  chemas.microsoft
+00000300: 2e63 6f6d 2f6f 6666 6963 652f 6472 6177  .com/office/draw
+00000310: 696e 672f 3230 3136 2f35 2f31 342f 6368  ing/2016/5/14/ch
+00000320: 6172 7465 7822 2078 6d6c 6e73 3a6d 633d  artex" xmlns:mc=
+00000330: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+00000340: 6f70 656e 786d 6c66 6f72 6d61 7473 2e6f  openxmlformats.o
+00000350: 7267 2f6d 6172 6b75 702d 636f 6d70 6174  rg/markup-compat
+00000360: 6962 696c 6974 792f 3230 3036 2220 786d  ibility/2006" xm
+00000370: 6c6e 733a 6169 6e6b 3d22 6874 7470 3a2f  lns:aink="http:/
+00000380: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
+00000390: 6674 2e63 6f6d 2f6f 6666 6963 652f 6472  ft.com/office/dr
+000003a0: 6177 696e 672f 3230 3136 2f69 6e6b 2220  awing/2016/ink" 
+000003b0: 786d 6c6e 733a 616d 3364 3d22 6874 7470  xmlns:am3d="http
+000003c0: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
+000003d0: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
+000003e0: 6472 6177 696e 672f 3230 3137 2f6d 6f64  drawing/2017/mod
+000003f0: 656c 3364 2220 786d 6c6e 733a 6f3d 2275  el3d" xmlns:o="u
+00000400: 726e 3a73 6368 656d 6173 2d6d 6963 726f  rn:schemas-micro
+00000410: 736f 6674 2d63 6f6d 3a6f 6666 6963 653a  soft-com:office:
+00000420: 6f66 6669 6365 2220 786d 6c6e 733a 6f65  office" xmlns:oe
+00000430: 6c3d 2268 7474 703a 2f2f 7363 6865 6d61  l="http://schema
+00000440: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+00000450: 6f66 6669 6365 2f32 3031 392f 6578 746c  office/2019/extl
+00000460: 7374 2220 786d 6c6e 733a 723d 2268 7474  st" xmlns:r="htt
+00000470: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
+00000480: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f6f  xmlformats.org/o
+00000490: 6666 6963 6544 6f63 756d 656e 742f 3230  fficeDocument/20
+000004a0: 3036 2f72 656c 6174 696f 6e73 6869 7073  06/relationships
+000004b0: 2220 786d 6c6e 733a 6d3d 2268 7474 703a  " xmlns:m="http:
+000004c0: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
+000004d0: 6c66 6f72 6d61 7473 2e6f 7267 2f6f 6666  lformats.org/off
+000004e0: 6963 6544 6f63 756d 656e 742f 3230 3036  iceDocument/2006
+000004f0: 2f6d 6174 6822 2078 6d6c 6e73 3a76 3d22  /math" xmlns:v="
+00000500: 7572 6e3a 7363 6865 6d61 732d 6d69 6372  urn:schemas-micr
+00000510: 6f73 6f66 742d 636f 6d3a 766d 6c22 2078  osoft-com:vml" x
+00000520: 6d6c 6e73 3a77 7031 343d 2268 7474 703a  mlns:wp14="http:
+00000530: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+00000540: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
+00000550: 6f72 642f 3230 3130 2f77 6f72 6470 726f  ord/2010/wordpro
+00000560: 6365 7373 696e 6744 7261 7769 6e67 2220  cessingDrawing" 
+00000570: 786d 6c6e 733a 7770 3d22 6874 7470 3a2f  xmlns:wp="http:/
+00000580: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
+00000590: 666f 726d 6174 732e 6f72 672f 6472 6177  formats.org/draw
+000005a0: 696e 676d 6c2f 3230 3036 2f77 6f72 6470  ingml/2006/wordp
+000005b0: 726f 6365 7373 696e 6744 7261 7769 6e67  rocessingDrawing
+000005c0: 2220 786d 6c6e 733a 7731 303d 2275 726e  " xmlns:w10="urn
+000005d0: 3a73 6368 656d 6173 2d6d 6963 726f 736f  :schemas-microso
+000005e0: 6674 2d63 6f6d 3a6f 6666 6963 653a 776f  ft-com:office:wo
+000005f0: 7264 2220 786d 6c6e 733a 773d 2268 7474  rd" xmlns:w="htt
+00000600: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
+00000610: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f77  xmlformats.org/w
+00000620: 6f72 6470 726f 6365 7373 696e 676d 6c2f  ordprocessingml/
+00000630: 3230 3036 2f6d 6169 6e22 2078 6d6c 6e73  2006/main" xmlns
+00000640: 3a77 3134 3d22 6874 7470 3a2f 2f73 6368  :w14="http://sch
+00000650: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
+00000660: 6f6d 2f6f 6666 6963 652f 776f 7264 2f32  om/office/word/2
+00000670: 3031 302f 776f 7264 6d6c 2220 786d 6c6e  010/wordml" xmln
+00000680: 733a 7731 353d 2268 7474 703a 2f2f 7363  s:w15="http://sc
+00000690: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
+000006a0: 636f 6d2f 6f66 6669 6365 2f77 6f72 642f  com/office/word/
+000006b0: 3230 3132 2f77 6f72 646d 6c22 2078 6d6c  2012/wordml" xml
+000006c0: 6e73 3a77 3136 6365 783d 2268 7474 703a  ns:w16cex="http:
+000006d0: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+000006e0: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
+000006f0: 6f72 642f 3230 3138 2f77 6f72 646d 6c2f  ord/2018/wordml/
+00000700: 6365 7822 2078 6d6c 6e73 3a77 3136 6369  cex" xmlns:w16ci
+00000710: 643d 2268 7474 703a 2f2f 7363 6865 6d61  d="http://schema
+00000720: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+00000730: 6f66 6669 6365 2f77 6f72 642f 3230 3136  office/word/2016
+00000740: 2f77 6f72 646d 6c2f 6369 6422 2078 6d6c  /wordml/cid" xml
+00000750: 6e73 3a77 3136 3d22 6874 7470 3a2f 2f73  ns:w16="http://s
+00000760: 6368 656d 6173 2e6d 6963 726f 736f 6674  chemas.microsoft
+00000770: 2e63 6f6d 2f6f 6666 6963 652f 776f 7264  .com/office/word
+00000780: 2f32 3031 382f 776f 7264 6d6c 2220 786d  /2018/wordml" xm
+00000790: 6c6e 733a 7731 3673 6474 6468 3d22 6874  lns:w16sdtdh="ht
+000007a0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+000007b0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+000007c0: 652f 776f 7264 2f32 3032 302f 776f 7264  e/word/2020/word
+000007d0: 6d6c 2f73 6474 6461 7461 6861 7368 2220  ml/sdtdatahash" 
+000007e0: 786d 6c6e 733a 7731 3673 653d 2268 7474  xmlns:w16se="htt
+000007f0: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
+00000800: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
+00000810: 2f77 6f72 642f 3230 3135 2f77 6f72 646d  /word/2015/wordm
+00000820: 6c2f 7379 6d65 7822 2078 6d6c 6e73 3a77  l/symex" xmlns:w
+00000830: 7067 3d22 6874 7470 3a2f 2f73 6368 656d  pg="http://schem
+00000840: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
+00000850: 2f6f 6666 6963 652f 776f 7264 2f32 3031  /office/word/201
+00000860: 302f 776f 7264 7072 6f63 6573 7369 6e67  0/wordprocessing
+00000870: 4772 6f75 7022 2078 6d6c 6e73 3a77 7069  Group" xmlns:wpi
+00000880: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
+00000890: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
+000008a0: 6666 6963 652f 776f 7264 2f32 3031 302f  ffice/word/2010/
+000008b0: 776f 7264 7072 6f63 6573 7369 6e67 496e  wordprocessingIn
+000008c0: 6b22 2078 6d6c 6e73 3a77 6e65 3d22 6874  k" xmlns:wne="ht
+000008d0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+000008e0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+000008f0: 652f 776f 7264 2f32 3030 362f 776f 7264  e/word/2006/word
+00000900: 6d6c 2220 786d 6c6e 733a 7770 733d 2268  ml" xmlns:wps="h
+00000910: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
+00000920: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
+00000930: 6365 2f77 6f72 642f 3230 3130 2f77 6f72  ce/word/2010/wor
+00000940: 6470 726f 6365 7373 696e 6753 6861 7065  dprocessingShape
+00000950: 2220 6d63 3a49 676e 6f72 6162 6c65 3d22  " mc:Ignorable="
+00000960: 7731 3420 7731 3520 7731 3673 6520 7731  w14 w15 w16se w1
+00000970: 3663 6964 2077 3136 2077 3136 6365 7820  6cid w16 w16cex 
+00000980: 7731 3673 6474 6468 2077 7031 3422 3e3c  w16sdtdh wp14"><
+00000990: 773a 6162 7374 7261 6374 4e75 6d20 773a  w:abstractNum w:
+000009a0: 6162 7374 7261 6374 4e75 6d49 643d 2230  abstractNumId="0
+000009b0: 2220 7731 353a 7265 7374 6172 744e 756d  " w15:restartNum
+000009c0: 6265 7269 6e67 4166 7465 7242 7265 616b  beringAfterBreak
+000009d0: 3d22 3022 3e3c 773a 6e73 6964 2077 3a76  ="0"><w:nsid w:v
+000009e0: 616c 3d22 4646 4646 4646 3743 222f 3e3c  al="FFFFFF7C"/><
+000009f0: 773a 6d75 6c74 694c 6576 656c 5479 7065  w:multiLevelType
+00000a00: 2077 3a76 616c 3d22 7369 6e67 6c65 4c65   w:val="singleLe
+00000a10: 7665 6c22 2f3e 3c77 3a74 6d70 6c20 773a  vel"/><w:tmpl w:
+00000a20: 7661 6c3d 2232 4339 3833 3642 4322 2f3e  val="2C9836BC"/>
+00000a30: 3c77 3a6c 766c 2077 3a69 6c76 6c3d 2230  <w:lvl w:ilvl="0
+00000a40: 223e 3c77 3a73 7461 7274 2077 3a76 616c  "><w:start w:val
+00000a50: 3d22 3122 2f3e 3c77 3a6e 756d 466d 7420  ="1"/><w:numFmt 
+00000a60: 773a 7661 6c3d 2264 6563 696d 616c 222f  w:val="decimal"/
+00000a70: 3e3c 773a 6c76 6c54 6578 7420 773a 7661  ><w:lvlText w:va
+00000a80: 6c3d 2225 312e 222f 3e3c 773a 6c76 6c4a  l="%1."/><w:lvlJ
+00000a90: 6320 773a 7661 6c3d 226c 6566 7422 2f3e  c w:val="left"/>
+00000aa0: 3c77 3a70 5072 3e3c 773a 7461 6273 3e3c  <w:pPr><w:tabs><
+00000ab0: 773a 7461 6220 773a 7661 6c3d 226e 756d  w:tab w:val="num
+00000ac0: 2220 773a 706f 733d 2231 3439 3222 2f3e  " w:pos="1492"/>
+00000ad0: 3c2f 773a 7461 6273 3e3c 773a 696e 6420  </w:tabs><w:ind 
+00000ae0: 773a 6c65 6674 3d22 3134 3932 2220 773a  w:left="1492" w:
+00000af0: 6861 6e67 696e 673d 2233 3630 222f 3e3c  hanging="360"/><
+00000b00: 2f77 3a70 5072 3e3c 2f77 3a6c 766c 3e3c  /w:pPr></w:lvl><
+00000b10: 2f77 3a61 6273 7472 6163 744e 756d 3e3c  /w:abstractNum><
+00000b20: 773a 6162 7374 7261 6374 4e75 6d20 773a  w:abstractNum w:
+00000b30: 6162 7374 7261 6374 4e75 6d49 643d 2231  abstractNumId="1
+00000b40: 2220 7731 353a 7265 7374 6172 744e 756d  " w15:restartNum
+00000b50: 6265 7269 6e67 4166 7465 7242 7265 616b  beringAfterBreak
+00000b60: 3d22 3022 3e3c 773a 6e73 6964 2077 3a76  ="0"><w:nsid w:v
+00000b70: 616c 3d22 4646 4646 4646 3744 222f 3e3c  al="FFFFFF7D"/><
+00000b80: 773a 6d75 6c74 694c 6576 656c 5479 7065  w:multiLevelType
+00000b90: 2077 3a76 616c 3d22 7369 6e67 6c65 4c65   w:val="singleLe
+00000ba0: 7665 6c22 2f3e 3c77 3a74 6d70 6c20 773a  vel"/><w:tmpl w:
+00000bb0: 7661 6c3d 2232 3931 3230 3145 3022 2f3e  val="291201E0"/>
+00000bc0: 3c77 3a6c 766c 2077 3a69 6c76 6c3d 2230  <w:lvl w:ilvl="0
+00000bd0: 223e 3c77 3a73 7461 7274 2077 3a76 616c  "><w:start w:val
+00000be0: 3d22 3122 2f3e 3c77 3a6e 756d 466d 7420  ="1"/><w:numFmt 
+00000bf0: 773a 7661 6c3d 2264 6563 696d 616c 222f  w:val="decimal"/
+00000c00: 3e3c 773a 6c76 6c54 6578 7420 773a 7661  ><w:lvlText w:va
+00000c10: 6c3d 2225 312e 222f 3e3c 773a 6c76 6c4a  l="%1."/><w:lvlJ
+00000c20: 6320 773a 7661 6c3d 226c 6566 7422 2f3e  c w:val="left"/>
+00000c30: 3c77 3a70 5072 3e3c 773a 7461 6273 3e3c  <w:pPr><w:tabs><
+00000c40: 773a 7461 6220 773a 7661 6c3d 226e 756d  w:tab w:val="num
+00000c50: 2220 773a 706f 733d 2231 3230 3922 2f3e  " w:pos="1209"/>
+00000c60: 3c2f 773a 7461 6273 3e3c 773a 696e 6420  </w:tabs><w:ind 
+00000c70: 773a 6c65 6674 3d22 3132 3039 2220 773a  w:left="1209" w:
+00000c80: 6861 6e67 696e 673d 2233 3630 222f 3e3c  hanging="360"/><
+00000c90: 2f77 3a70 5072 3e3c 2f77 3a6c 766c 3e3c  /w:pPr></w:lvl><
+00000ca0: 2f77 3a61 6273 7472 6163 744e 756d 3e3c  /w:abstractNum><
+00000cb0: 773a 6162 7374 7261 6374 4e75 6d20 773a  w:abstractNum w:
+00000cc0: 6162 7374 7261 6374 4e75 6d49 643d 2232  abstractNumId="2
+00000cd0: 2220 7731 353a 7265 7374 6172 744e 756d  " w15:restartNum
+00000ce0: 6265 7269 6e67 4166 7465 7242 7265 616b  beringAfterBreak
+00000cf0: 3d22 3022 3e3c 773a 6e73 6964 2077 3a76  ="0"><w:nsid w:v
+00000d00: 616c 3d22 4646 4646 4646 3745 222f 3e3c  al="FFFFFF7E"/><
+00000d10: 773a 6d75 6c74 694c 6576 656c 5479 7065  w:multiLevelType
+00000d20: 2077 3a76 616c 3d22 7369 6e67 6c65 4c65   w:val="singleLe
+00000d30: 7665 6c22 2f3e 3c77 3a74 6d70 6c20 773a  vel"/><w:tmpl w:
+00000d40: 7661 6c3d 2244 3235 4137 3043 4522 2f3e  val="D25A70CE"/>
+00000d50: 3c77 3a6c 766c 2077 3a69 6c76 6c3d 2230  <w:lvl w:ilvl="0
+00000d60: 223e 3c77 3a73 7461 7274 2077 3a76 616c  "><w:start w:val
+00000d70: 3d22 3122 2f3e 3c77 3a6e 756d 466d 7420  ="1"/><w:numFmt 
+00000d80: 773a 7661 6c3d 2264 6563 696d 616c 222f  w:val="decimal"/
+00000d90: 3e3c 773a 6c76 6c54 6578 7420 773a 7661  ><w:lvlText w:va
+00000da0: 6c3d 2225 312e 222f 3e3c 773a 6c76 6c4a  l="%1."/><w:lvlJ
+00000db0: 6320 773a 7661 6c3d 226c 6566 7422 2f3e  c w:val="left"/>
+00000dc0: 3c77 3a70 5072 3e3c 773a 7461 6273 3e3c  <w:pPr><w:tabs><
+00000dd0: 773a 7461 6220 773a 7661 6c3d 226e 756d  w:tab w:val="num
+00000de0: 2220 773a 706f 733d 2239 3236 222f 3e3c  " w:pos="926"/><
+00000df0: 2f77 3a74 6162 733e 3c77 3a69 6e64 2077  /w:tabs><w:ind w
+00000e00: 3a6c 6566 743d 2239 3236 2220 773a 6861  :left="926" w:ha
+00000e10: 6e67 696e 673d 2233 3630 222f 3e3c 2f77  nging="360"/></w
+00000e20: 3a70 5072 3e3c 2f77 3a6c 766c 3e3c 2f77  :pPr></w:lvl></w
+00000e30: 3a61 6273 7472 6163 744e 756d 3e3c 773a  :abstractNum><w:
+00000e40: 6162 7374 7261 6374 4e75 6d20 773a 6162  abstractNum w:ab
+00000e50: 7374 7261 6374 4e75 6d49 643d 2233 2220  stractNumId="3" 
+00000e60: 7731 353a 7265 7374 6172 744e 756d 6265  w15:restartNumbe
+00000e70: 7269 6e67 4166 7465 7242 7265 616b 3d22  ringAfterBreak="
+00000e80: 3022 3e3c 773a 6e73 6964 2077 3a76 616c  0"><w:nsid w:val
+00000e90: 3d22 4646 4646 4646 3746 222f 3e3c 773a  ="FFFFFF7F"/><w:
+00000ea0: 6d75 6c74 694c 6576 656c 5479 7065 2077  multiLevelType w
+00000eb0: 3a76 616c 3d22 7369 6e67 6c65 4c65 7665  :val="singleLeve
+00000ec0: 6c22 2f3e 3c77 3a74 6d70 6c20 773a 7661  l"/><w:tmpl w:va
+00000ed0: 6c3d 2231 4339 3441 3437 3022 2f3e 3c77  l="1C94A470"/><w
+00000ee0: 3a6c 766c 2077 3a69 6c76 6c3d 2230 223e  :lvl w:ilvl="0">
+00000ef0: 3c77 3a73 7461 7274 2077 3a76 616c 3d22  <w:start w:val="
+00000f00: 3122 2f3e 3c77 3a6e 756d 466d 7420 773a  1"/><w:numFmt w:
+00000f10: 7661 6c3d 2264 6563 696d 616c 222f 3e3c  val="decimal"/><
+00000f20: 773a 6c76 6c54 6578 7420 773a 7661 6c3d  w:lvlText w:val=
+00000f30: 2225 312e 222f 3e3c 773a 6c76 6c4a 6320  "%1."/><w:lvlJc 
+00000f40: 773a 7661 6c3d 226c 6566 7422 2f3e 3c77  w:val="left"/><w
+00000f50: 3a70 5072 3e3c 773a 7461 6273 3e3c 773a  :pPr><w:tabs><w:
+00000f60: 7461 6220 773a 7661 6c3d 226e 756d 2220  tab w:val="num" 
+00000f70: 773a 706f 733d 2236 3433 222f 3e3c 2f77  w:pos="643"/></w
+00000f80: 3a74 6162 733e 3c77 3a69 6e64 2077 3a6c  :tabs><w:ind w:l
+00000f90: 6566 743d 2236 3433 2220 773a 6861 6e67  eft="643" w:hang
+00000fa0: 696e 673d 2233 3630 222f 3e3c 2f77 3a70  ing="360"/></w:p
+00000fb0: 5072 3e3c 2f77 3a6c 766c 3e3c 2f77 3a61  Pr></w:lvl></w:a
+00000fc0: 6273 7472 6163 744e 756d 3e3c 773a 6162  bstractNum><w:ab
+00000fd0: 7374 7261 6374 4e75 6d20 773a 6162 7374  stractNum w:abst
+00000fe0: 7261 6374 4e75 6d49 643d 2234 2220 7731  ractNumId="4" w1
+00000ff0: 353a 7265 7374 6172 744e 756d 6265 7269  5:restartNumberi
+00001000: 6e67 4166 7465 7242 7265 616b 3d22 3022  ngAfterBreak="0"
+00001010: 3e3c 773a 6e73 6964 2077 3a76 616c 3d22  ><w:nsid w:val="
+00001020: 4646 4646 4646 3830 222f 3e3c 773a 6d75  FFFFFF80"/><w:mu
+00001030: 6c74 694c 6576 656c 5479 7065 2077 3a76  ltiLevelType w:v
+00001040: 616c 3d22 7369 6e67 6c65 4c65 7665 6c22  al="singleLevel"
+00001050: 2f3e 3c77 3a74 6d70 6c20 773a 7661 6c3d  /><w:tmpl w:val=
+00001060: 2236 4436 3636 4437 4522 2f3e 3c77 3a6c  "6D666D7E"/><w:l
+00001070: 766c 2077 3a69 6c76 6c3d 2230 223e 3c77  vl w:ilvl="0"><w
+00001080: 3a73 7461 7274 2077 3a76 616c 3d22 3122  :start w:val="1"
+00001090: 2f3e 3c77 3a6e 756d 466d 7420 773a 7661  /><w:numFmt w:va
+000010a0: 6c3d 2262 756c 6c65 7422 2f3e 3c77 3a6c  l="bullet"/><w:l
+000010b0: 766c 5465 7874 2077 3a76 616c 3d22 ef82  vlText w:val="..
+000010c0: b722 2f3e 3c77 3a6c 766c 4a63 2077 3a76  ."/><w:lvlJc w:v
+000010d0: 616c 3d22 6c65 6674 222f 3e3c 773a 7050  al="left"/><w:pP
+000010e0: 723e 3c77 3a74 6162 733e 3c77 3a74 6162  r><w:tabs><w:tab
+000010f0: 2077 3a76 616c 3d22 6e75 6d22 2077 3a70   w:val="num" w:p
+00001100: 6f73 3d22 3134 3932 222f 3e3c 2f77 3a74  os="1492"/></w:t
+00001110: 6162 733e 3c77 3a69 6e64 2077 3a6c 6566  abs><w:ind w:lef
+00001120: 743d 2231 3439 3222 2077 3a68 616e 6769  t="1492" w:hangi
+00001130: 6e67 3d22 3336 3022 2f3e 3c2f 773a 7050  ng="360"/></w:pP
+00001140: 723e 3c77 3a72 5072 3e3c 773a 7246 6f6e  r><w:rPr><w:rFon
+00001150: 7473 2077 3a61 7363 6969 3d22 5379 6d62  ts w:ascii="Symb
+00001160: 6f6c 2220 773a 6841 6e73 693d 2253 796d  ol" w:hAnsi="Sym
+00001170: 626f 6c22 2077 3a68 696e 743d 2264 6566  bol" w:hint="def
+00001180: 6175 6c74 222f 3e3c 2f77 3a72 5072 3e3c  ault"/></w:rPr><
+00001190: 2f77 3a6c 766c 3e3c 2f77 3a61 6273 7472  /w:lvl></w:abstr
+000011a0: 6163 744e 756d 3e3c 773a 6162 7374 7261  actNum><w:abstra
+000011b0: 6374 4e75 6d20 773a 6162 7374 7261 6374  ctNum w:abstract
+000011c0: 4e75 6d49 643d 2235 2220 7731 353a 7265  NumId="5" w15:re
+000011d0: 7374 6172 744e 756d 6265 7269 6e67 4166  startNumberingAf
+000011e0: 7465 7242 7265 616b 3d22 3022 3e3c 773a  terBreak="0"><w:
+000011f0: 6e73 6964 2077 3a76 616c 3d22 4646 4646  nsid w:val="FFFF
+00001200: 4646 3831 222f 3e3c 773a 6d75 6c74 694c  FF81"/><w:multiL
+00001210: 6576 656c 5479 7065 2077 3a76 616c 3d22  evelType w:val="
+00001220: 7369 6e67 6c65 4c65 7665 6c22 2f3e 3c77  singleLevel"/><w
+00001230: 3a74 6d70 6c20 773a 7661 6c3d 2245 3739  :tmpl w:val="E79
+00001240: 4138 3032 4122 2f3e 3c77 3a6c 766c 2077  A802A"/><w:lvl w
+00001250: 3a69 6c76 6c3d 2230 223e 3c77 3a73 7461  :ilvl="0"><w:sta
+00001260: 7274 2077 3a76 616c 3d22 3122 2f3e 3c77  rt w:val="1"/><w
+00001270: 3a6e 756d 466d 7420 773a 7661 6c3d 2262  :numFmt w:val="b
+00001280: 756c 6c65 7422 2f3e 3c77 3a6c 766c 5465  ullet"/><w:lvlTe
+00001290: 7874 2077 3a76 616c 3d22 ef82 b722 2f3e  xt w:val="..."/>
+000012a0: 3c77 3a6c 766c 4a63 2077 3a76 616c 3d22  <w:lvlJc w:val="
+000012b0: 6c65 6674 222f 3e3c 773a 7050 723e 3c77  left"/><w:pPr><w
+000012c0: 3a74 6162 733e 3c77 3a74 6162 2077 3a76  :tabs><w:tab w:v
+000012d0: 616c 3d22 6e75 6d22 2077 3a70 6f73 3d22  al="num" w:pos="
+000012e0: 3132 3039 222f 3e3c 2f77 3a74 6162 733e  1209"/></w:tabs>
+000012f0: 3c77 3a69 6e64 2077 3a6c 6566 743d 2231  <w:ind w:left="1
+00001300: 3230 3922 2077 3a68 616e 6769 6e67 3d22  209" w:hanging="
+00001310: 3336 3022 2f3e 3c2f 773a 7050 723e 3c77  360"/></w:pPr><w
+00001320: 3a72 5072 3e3c 773a 7246 6f6e 7473 2077  :rPr><w:rFonts w
+00001330: 3a61 7363 6969 3d22 5379 6d62 6f6c 2220  :ascii="Symbol" 
+00001340: 773a 6841 6e73 693d 2253 796d 626f 6c22  w:hAnsi="Symbol"
+00001350: 2077 3a68 696e 743d 2264 6566 6175 6c74   w:hint="default
+00001360: 222f 3e3c 2f77 3a72 5072 3e3c 2f77 3a6c  "/></w:rPr></w:l
+00001370: 766c 3e3c 2f77 3a61 6273 7472 6163 744e  vl></w:abstractN
+00001380: 756d 3e3c 773a 6162 7374 7261 6374 4e75  um><w:abstractNu
+00001390: 6d20 773a 6162 7374 7261 6374 4e75 6d49  m w:abstractNumI
+000013a0: 643d 2236 2220 7731 353a 7265 7374 6172  d="6" w15:restar
+000013b0: 744e 756d 6265 7269 6e67 4166 7465 7242  tNumberingAfterB
+000013c0: 7265 616b 3d22 3022 3e3c 773a 6e73 6964  reak="0"><w:nsid
+000013d0: 2077 3a76 616c 3d22 4646 4646 4646 3832   w:val="FFFFFF82
+000013e0: 222f 3e3c 773a 6d75 6c74 694c 6576 656c  "/><w:multiLevel
+000013f0: 5479 7065 2077 3a76 616c 3d22 7369 6e67  Type w:val="sing
+00001400: 6c65 4c65 7665 6c22 2f3e 3c77 3a74 6d70  leLevel"/><w:tmp
+00001410: 6c20 773a 7661 6c3d 2246 3946 4531 4438  l w:val="F9FE1D8
+00001420: 4322 2f3e 3c77 3a6c 766c 2077 3a69 6c76  C"/><w:lvl w:ilv
+00001430: 6c3d 2230 223e 3c77 3a73 7461 7274 2077  l="0"><w:start w
+00001440: 3a76 616c 3d22 3122 2f3e 3c77 3a6e 756d  :val="1"/><w:num
+00001450: 466d 7420 773a 7661 6c3d 2262 756c 6c65  Fmt w:val="bulle
+00001460: 7422 2f3e 3c77 3a6c 766c 5465 7874 2077  t"/><w:lvlText w
+00001470: 3a76 616c 3d22 ef82 b722 2f3e 3c77 3a6c  :val="..."/><w:l
+00001480: 766c 4a63 2077 3a76 616c 3d22 6c65 6674  vlJc w:val="left
+00001490: 222f 3e3c 773a 7050 723e 3c77 3a74 6162  "/><w:pPr><w:tab
+000014a0: 733e 3c77 3a74 6162 2077 3a76 616c 3d22  s><w:tab w:val="
+000014b0: 6e75 6d22 2077 3a70 6f73 3d22 3932 3622  num" w:pos="926"
+000014c0: 2f3e 3c2f 773a 7461 6273 3e3c 773a 696e  /></w:tabs><w:in
+000014d0: 6420 773a 6c65 6674 3d22 3932 3622 2077  d w:left="926" w
+000014e0: 3a68 616e 6769 6e67 3d22 3336 3022 2f3e  :hanging="360"/>
+000014f0: 3c2f 773a 7050 723e 3c77 3a72 5072 3e3c  </w:pPr><w:rPr><
+00001500: 773a 7246 6f6e 7473 2077 3a61 7363 6969  w:rFonts w:ascii
+00001510: 3d22 5379 6d62 6f6c 2220 773a 6841 6e73  ="Symbol" w:hAns
+00001520: 693d 2253 796d 626f 6c22 2077 3a68 696e  i="Symbol" w:hin
+00001530: 743d 2264 6566 6175 6c74 222f 3e3c 2f77  t="default"/></w
+00001540: 3a72 5072 3e3c 2f77 3a6c 766c 3e3c 2f77  :rPr></w:lvl></w
+00001550: 3a61 6273 7472 6163 744e 756d 3e3c 773a  :abstractNum><w:
+00001560: 6162 7374 7261 6374 4e75 6d20 773a 6162  abstractNum w:ab
+00001570: 7374 7261 6374 4e75 6d49 643d 2237 2220  stractNumId="7" 
+00001580: 7731 353a 7265 7374 6172 744e 756d 6265  w15:restartNumbe
+00001590: 7269 6e67 4166 7465 7242 7265 616b 3d22  ringAfterBreak="
+000015a0: 3022 3e3c 773a 6e73 6964 2077 3a76 616c  0"><w:nsid w:val
+000015b0: 3d22 4646 4646 4646 3833 222f 3e3c 773a  ="FFFFFF83"/><w:
+000015c0: 6d75 6c74 694c 6576 656c 5479 7065 2077  multiLevelType w
+000015d0: 3a76 616c 3d22 7369 6e67 6c65 4c65 7665  :val="singleLeve
+000015e0: 6c22 2f3e 3c77 3a74 6d70 6c20 773a 7661  l"/><w:tmpl w:va
+000015f0: 6c3d 2242 3739 3637 3236 4322 2f3e 3c77  l="B796726C"/><w
+00001600: 3a6c 766c 2077 3a69 6c76 6c3d 2230 223e  :lvl w:ilvl="0">
+00001610: 3c77 3a73 7461 7274 2077 3a76 616c 3d22  <w:start w:val="
+00001620: 3122 2f3e 3c77 3a6e 756d 466d 7420 773a  1"/><w:numFmt w:
+00001630: 7661 6c3d 2262 756c 6c65 7422 2f3e 3c77  val="bullet"/><w
+00001640: 3a6c 766c 5465 7874 2077 3a76 616c 3d22  :lvlText w:val="
+00001650: ef82 b722 2f3e 3c77 3a6c 766c 4a63 2077  ..."/><w:lvlJc w
+00001660: 3a76 616c 3d22 6c65 6674 222f 3e3c 773a  :val="left"/><w:
+00001670: 7050 723e 3c77 3a74 6162 733e 3c77 3a74  pPr><w:tabs><w:t
+00001680: 6162 2077 3a76 616c 3d22 6e75 6d22 2077  ab w:val="num" w
+00001690: 3a70 6f73 3d22 3634 3322 2f3e 3c2f 773a  :pos="643"/></w:
+000016a0: 7461 6273 3e3c 773a 696e 6420 773a 6c65  tabs><w:ind w:le
+000016b0: 6674 3d22 3634 3322 2077 3a68 616e 6769  ft="643" w:hangi
+000016c0: 6e67 3d22 3336 3022 2f3e 3c2f 773a 7050  ng="360"/></w:pP
+000016d0: 723e 3c77 3a72 5072 3e3c 773a 7246 6f6e  r><w:rPr><w:rFon
+000016e0: 7473 2077 3a61 7363 6969 3d22 5379 6d62  ts w:ascii="Symb
+000016f0: 6f6c 2220 773a 6841 6e73 693d 2253 796d  ol" w:hAnsi="Sym
+00001700: 626f 6c22 2077 3a68 696e 743d 2264 6566  bol" w:hint="def
+00001710: 6175 6c74 222f 3e3c 2f77 3a72 5072 3e3c  ault"/></w:rPr><
+00001720: 2f77 3a6c 766c 3e3c 2f77 3a61 6273 7472  /w:lvl></w:abstr
+00001730: 6163 744e 756d 3e3c 773a 6162 7374 7261  actNum><w:abstra
+00001740: 6374 4e75 6d20 773a 6162 7374 7261 6374  ctNum w:abstract
+00001750: 4e75 6d49 643d 2238 2220 7731 353a 7265  NumId="8" w15:re
+00001760: 7374 6172 744e 756d 6265 7269 6e67 4166  startNumberingAf
+00001770: 7465 7242 7265 616b 3d22 3022 3e3c 773a  terBreak="0"><w:
+00001780: 6e73 6964 2077 3a76 616c 3d22 4646 4646  nsid w:val="FFFF
+00001790: 4646 3838 222f 3e3c 773a 6d75 6c74 694c  FF88"/><w:multiL
+000017a0: 6576 656c 5479 7065 2077 3a76 616c 3d22  evelType w:val="
+000017b0: 7369 6e67 6c65 4c65 7665 6c22 2f3e 3c77  singleLevel"/><w
+000017c0: 3a74 6d70 6c20 773a 7661 6c3d 2242 4439  :tmpl w:val="BD9
+000017d0: 4342 3933 3422 2f3e 3c77 3a6c 766c 2077  CB934"/><w:lvl w
+000017e0: 3a69 6c76 6c3d 2230 223e 3c77 3a73 7461  :ilvl="0"><w:sta
+000017f0: 7274 2077 3a76 616c 3d22 3122 2f3e 3c77  rt w:val="1"/><w
+00001800: 3a6e 756d 466d 7420 773a 7661 6c3d 2264  :numFmt w:val="d
+00001810: 6563 696d 616c 222f 3e3c 773a 7053 7479  ecimal"/><w:pSty
+00001820: 6c65 2077 3a76 616c 3d22 4c69 7374 4e75  le w:val="ListNu
+00001830: 6d62 6572 222f 3e3c 773a 6c76 6c54 6578  mber"/><w:lvlTex
+00001840: 7420 773a 7661 6c3d 2225 312e 222f 3e3c  t w:val="%1."/><
+00001850: 773a 6c76 6c4a 6320 773a 7661 6c3d 226c  w:lvlJc w:val="l
+00001860: 6566 7422 2f3e 3c77 3a70 5072 3e3c 773a  eft"/><w:pPr><w:
+00001870: 7461 6273 3e3c 773a 7461 6220 773a 7661  tabs><w:tab w:va
+00001880: 6c3d 226e 756d 2220 773a 706f 733d 2233  l="num" w:pos="3
+00001890: 3630 222f 3e3c 2f77 3a74 6162 733e 3c77  60"/></w:tabs><w
+000018a0: 3a69 6e64 2077 3a6c 6566 743d 2233 3630  :ind w:left="360
+000018b0: 2220 773a 6861 6e67 696e 673d 2233 3630  " w:hanging="360
+000018c0: 222f 3e3c 2f77 3a70 5072 3e3c 2f77 3a6c  "/></w:pPr></w:l
+000018d0: 766c 3e3c 2f77 3a61 6273 7472 6163 744e  vl></w:abstractN
+000018e0: 756d 3e3c 773a 6162 7374 7261 6374 4e75  um><w:abstractNu
+000018f0: 6d20 773a 6162 7374 7261 6374 4e75 6d49  m w:abstractNumI
+00001900: 643d 2239 2220 7731 353a 7265 7374 6172  d="9" w15:restar
+00001910: 744e 756d 6265 7269 6e67 4166 7465 7242  tNumberingAfterB
+00001920: 7265 616b 3d22 3022 3e3c 773a 6e73 6964  reak="0"><w:nsid
+00001930: 2077 3a76 616c 3d22 4646 4646 4646 3839   w:val="FFFFFF89
+00001940: 222f 3e3c 773a 6d75 6c74 694c 6576 656c  "/><w:multiLevel
+00001950: 5479 7065 2077 3a76 616c 3d22 7369 6e67  Type w:val="sing
+00001960: 6c65 4c65 7665 6c22 2f3e 3c77 3a74 6d70  leLevel"/><w:tmp
+00001970: 6c20 773a 7661 6c3d 2230 3030 3839 4432  l w:val="00089D2
+00001980: 4522 2f3e 3c77 3a6c 766c 2077 3a69 6c76  E"/><w:lvl w:ilv
+00001990: 6c3d 2230 223e 3c77 3a73 7461 7274 2077  l="0"><w:start w
+000019a0: 3a76 616c 3d22 3122 2f3e 3c77 3a6e 756d  :val="1"/><w:num
+000019b0: 466d 7420 773a 7661 6c3d 2262 756c 6c65  Fmt w:val="bulle
+000019c0: 7422 2f3e 3c77 3a70 5374 796c 6520 773a  t"/><w:pStyle w:
+000019d0: 7661 6c3d 224c 6973 7442 756c 6c65 7422  val="ListBullet"
+000019e0: 2f3e 3c77 3a6c 766c 5465 7874 2077 3a76  /><w:lvlText w:v
+000019f0: 616c 3d22 ef82 b722 2f3e 3c77 3a6c 766c  al="..."/><w:lvl
+00001a00: 4a63 2077 3a76 616c 3d22 6c65 6674 222f  Jc w:val="left"/
+00001a10: 3e3c 773a 7050 723e 3c77 3a74 6162 733e  ><w:pPr><w:tabs>
+00001a20: 3c77 3a74 6162 2077 3a76 616c 3d22 6e75  <w:tab w:val="nu
+00001a30: 6d22 2077 3a70 6f73 3d22 3336 3022 2f3e  m" w:pos="360"/>
+00001a40: 3c2f 773a 7461 6273 3e3c 773a 696e 6420  </w:tabs><w:ind 
+00001a50: 773a 6c65 6674 3d22 3336 3022 2077 3a68  w:left="360" w:h
+00001a60: 616e 6769 6e67 3d22 3336 3022 2f3e 3c2f  anging="360"/></
+00001a70: 773a 7050 723e 3c77 3a72 5072 3e3c 773a  w:pPr><w:rPr><w:
+00001a80: 7246 6f6e 7473 2077 3a61 7363 6969 3d22  rFonts w:ascii="
+00001a90: 5379 6d62 6f6c 2220 773a 6841 6e73 693d  Symbol" w:hAnsi=
+00001aa0: 2253 796d 626f 6c22 2077 3a68 696e 743d  "Symbol" w:hint=
+00001ab0: 2264 6566 6175 6c74 222f 3e3c 2f77 3a72  "default"/></w:r
+00001ac0: 5072 3e3c 2f77 3a6c 766c 3e3c 2f77 3a61  Pr></w:lvl></w:a
+00001ad0: 6273 7472 6163 744e 756d 3e3c 773a 6162  bstractNum><w:ab
+00001ae0: 7374 7261 6374 4e75 6d20 773a 6162 7374  stractNum w:abst
+00001af0: 7261 6374 4e75 6d49 643d 2231 3022 2077  ractNumId="10" w
+00001b00: 3135 3a72 6573 7461 7274 4e75 6d62 6572  15:restartNumber
+00001b10: 696e 6741 6674 6572 4272 6561 6b3d 2230  ingAfterBreak="0
+00001b20: 223e 3c77 3a6e 7369 6420 773a 7661 6c3d  "><w:nsid w:val=
+00001b30: 2232 4634 3736 3343 4222 2f3e 3c77 3a6d  "2F4763CB"/><w:m
+00001b40: 756c 7469 4c65 7665 6c54 7970 6520 773a  ultiLevelType w:
+00001b50: 7661 6c3d 2268 7962 7269 644d 756c 7469  val="hybridMulti
+00001b60: 6c65 7665 6c22 2f3e 3c77 3a74 6d70 6c20  level"/><w:tmpl 
+00001b70: 773a 7661 6c3d 2237 3433 4135 3431 4122  w:val="743A541A"
+00001b80: 2f3e 3c77 3a6c 766c 2077 3a69 6c76 6c3d  /><w:lvl w:ilvl=
+00001b90: 2230 2220 773a 7470 6c63 3d22 3230 3030  "0" w:tplc="2000
+00001ba0: 3030 3031 223e 3c77 3a73 7461 7274 2077  0001"><w:start w
+00001bb0: 3a76 616c 3d22 3122 2f3e 3c77 3a6e 756d  :val="1"/><w:num
+00001bc0: 466d 7420 773a 7661 6c3d 2262 756c 6c65  Fmt w:val="bulle
+00001bd0: 7422 2f3e 3c77 3a6c 766c 5465 7874 2077  t"/><w:lvlText w
+00001be0: 3a76 616c 3d22 ef82 b722 2f3e 3c77 3a6c  :val="..."/><w:l
+00001bf0: 766c 4a63 2077 3a76 616c 3d22 6c65 6674  vlJc w:val="left
+00001c00: 222f 3e3c 773a 7050 723e 3c77 3a69 6e64  "/><w:pPr><w:ind
+00001c10: 2077 3a6c 6566 743d 2237 3230 2220 773a   w:left="720" w:
+00001c20: 6861 6e67 696e 673d 2233 3630 222f 3e3c  hanging="360"/><
+00001c30: 2f77 3a70 5072 3e3c 773a 7250 723e 3c77  /w:pPr><w:rPr><w
+00001c40: 3a72 466f 6e74 7320 773a 6173 6369 693d  :rFonts w:ascii=
+00001c50: 2253 796d 626f 6c22 2077 3a68 416e 7369  "Symbol" w:hAnsi
+00001c60: 3d22 5379 6d62 6f6c 2220 773a 6869 6e74  ="Symbol" w:hint
+00001c70: 3d22 6465 6661 756c 7422 2f3e 3c2f 773a  ="default"/></w:
+00001c80: 7250 723e 3c2f 773a 6c76 6c3e 3c77 3a6c  rPr></w:lvl><w:l
+00001c90: 766c 2077 3a69 6c76 6c3d 2231 2220 773a  vl w:ilvl="1" w:
+00001ca0: 7470 6c63 3d22 3230 3030 3030 3033 2220  tplc="20000003" 
+00001cb0: 773a 7465 6e74 6174 6976 653d 2231 223e  w:tentative="1">
+00001cc0: 3c77 3a73 7461 7274 2077 3a76 616c 3d22  <w:start w:val="
+00001cd0: 3122 2f3e 3c77 3a6e 756d 466d 7420 773a  1"/><w:numFmt w:
+00001ce0: 7661 6c3d 2262 756c 6c65 7422 2f3e 3c77  val="bullet"/><w
+00001cf0: 3a6c 766c 5465 7874 2077 3a76 616c 3d22  :lvlText w:val="
+00001d00: 6f22 2f3e 3c77 3a6c 766c 4a63 2077 3a76  o"/><w:lvlJc w:v
+00001d10: 616c 3d22 6c65 6674 222f 3e3c 773a 7050  al="left"/><w:pP
+00001d20: 723e 3c77 3a69 6e64 2077 3a6c 6566 743d  r><w:ind w:left=
+00001d30: 2231 3434 3022 2077 3a68 616e 6769 6e67  "1440" w:hanging
+00001d40: 3d22 3336 3022 2f3e 3c2f 773a 7050 723e  ="360"/></w:pPr>
+00001d50: 3c77 3a72 5072 3e3c 773a 7246 6f6e 7473  <w:rPr><w:rFonts
+00001d60: 2077 3a61 7363 6969 3d22 436f 7572 6965   w:ascii="Courie
+00001d70: 7220 4e65 7722 2077 3a68 416e 7369 3d22  r New" w:hAnsi="
+00001d80: 436f 7572 6965 7220 4e65 7722 2077 3a63  Courier New" w:c
+00001d90: 733d 2243 6f75 7269 6572 204e 6577 2220  s="Courier New" 
+00001da0: 773a 6869 6e74 3d22 6465 6661 756c 7422  w:hint="default"
+00001db0: 2f3e 3c2f 773a 7250 723e 3c2f 773a 6c76  /></w:rPr></w:lv
+00001dc0: 6c3e 3c77 3a6c 766c 2077 3a69 6c76 6c3d  l><w:lvl w:ilvl=
+00001dd0: 2232 2220 773a 7470 6c63 3d22 3230 3030  "2" w:tplc="2000
+00001de0: 3030 3035 2220 773a 7465 6e74 6174 6976  0005" w:tentativ
+00001df0: 653d 2231 223e 3c77 3a73 7461 7274 2077  e="1"><w:start w
+00001e00: 3a76 616c 3d22 3122 2f3e 3c77 3a6e 756d  :val="1"/><w:num
+00001e10: 466d 7420 773a 7661 6c3d 2262 756c 6c65  Fmt w:val="bulle
+00001e20: 7422 2f3e 3c77 3a6c 766c 5465 7874 2077  t"/><w:lvlText w
+00001e30: 3a76 616c 3d22 ef82 a722 2f3e 3c77 3a6c  :val="..."/><w:l
+00001e40: 766c 4a63 2077 3a76 616c 3d22 6c65 6674  vlJc w:val="left
+00001e50: 222f 3e3c 773a 7050 723e 3c77 3a69 6e64  "/><w:pPr><w:ind
+00001e60: 2077 3a6c 6566 743d 2232 3136 3022 2077   w:left="2160" w
+00001e70: 3a68 616e 6769 6e67 3d22 3336 3022 2f3e  :hanging="360"/>
+00001e80: 3c2f 773a 7050 723e 3c77 3a72 5072 3e3c  </w:pPr><w:rPr><
+00001e90: 773a 7246 6f6e 7473 2077 3a61 7363 6969  w:rFonts w:ascii
+00001ea0: 3d22 5769 6e67 6469 6e67 7322 2077 3a68  ="Wingdings" w:h
+00001eb0: 416e 7369 3d22 5769 6e67 6469 6e67 7322  Ansi="Wingdings"
+00001ec0: 2077 3a68 696e 743d 2264 6566 6175 6c74   w:hint="default
+00001ed0: 222f 3e3c 2f77 3a72 5072 3e3c 2f77 3a6c  "/></w:rPr></w:l
+00001ee0: 766c 3e3c 773a 6c76 6c20 773a 696c 766c  vl><w:lvl w:ilvl
+00001ef0: 3d22 3322 2077 3a74 706c 633d 2232 3030  ="3" w:tplc="200
+00001f00: 3030 3030 3122 2077 3a74 656e 7461 7469  00001" w:tentati
+00001f10: 7665 3d22 3122 3e3c 773a 7374 6172 7420  ve="1"><w:start 
+00001f20: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
+00001f30: 6d46 6d74 2077 3a76 616c 3d22 6275 6c6c  mFmt w:val="bull
+00001f40: 6574 222f 3e3c 773a 6c76 6c54 6578 7420  et"/><w:lvlText 
+00001f50: 773a 7661 6c3d 22ef 82b7 222f 3e3c 773a  w:val="..."/><w:
+00001f60: 6c76 6c4a 6320 773a 7661 6c3d 226c 6566  lvlJc w:val="lef
+00001f70: 7422 2f3e 3c77 3a70 5072 3e3c 773a 696e  t"/><w:pPr><w:in
+00001f80: 6420 773a 6c65 6674 3d22 3238 3830 2220  d w:left="2880" 
+00001f90: 773a 6861 6e67 696e 673d 2233 3630 222f  w:hanging="360"/
+00001fa0: 3e3c 2f77 3a70 5072 3e3c 773a 7250 723e  ></w:pPr><w:rPr>
+00001fb0: 3c77 3a72 466f 6e74 7320 773a 6173 6369  <w:rFonts w:asci
+00001fc0: 693d 2253 796d 626f 6c22 2077 3a68 416e  i="Symbol" w:hAn
+00001fd0: 7369 3d22 5379 6d62 6f6c 2220 773a 6869  si="Symbol" w:hi
+00001fe0: 6e74 3d22 6465 6661 756c 7422 2f3e 3c2f  nt="default"/></
+00001ff0: 773a 7250 723e 3c2f 773a 6c76 6c3e 3c77  w:rPr></w:lvl><w
+00002000: 3a6c 766c 2077 3a69 6c76 6c3d 2234 2220  :lvl w:ilvl="4" 
+00002010: 773a 7470 6c63 3d22 3230 3030 3030 3033  w:tplc="20000003
+00002020: 2220 773a 7465 6e74 6174 6976 653d 2231  " w:tentative="1
+00002030: 223e 3c77 3a73 7461 7274 2077 3a76 616c  "><w:start w:val
+00002040: 3d22 3122 2f3e 3c77 3a6e 756d 466d 7420  ="1"/><w:numFmt 
+00002050: 773a 7661 6c3d 2262 756c 6c65 7422 2f3e  w:val="bullet"/>
+00002060: 3c77 3a6c 766c 5465 7874 2077 3a76 616c  <w:lvlText w:val
+00002070: 3d22 6f22 2f3e 3c77 3a6c 766c 4a63 2077  ="o"/><w:lvlJc w
+00002080: 3a76 616c 3d22 6c65 6674 222f 3e3c 773a  :val="left"/><w:
+00002090: 7050 723e 3c77 3a69 6e64 2077 3a6c 6566  pPr><w:ind w:lef
+000020a0: 743d 2233 3630 3022 2077 3a68 616e 6769  t="3600" w:hangi
+000020b0: 6e67 3d22 3336 3022 2f3e 3c2f 773a 7050  ng="360"/></w:pP
+000020c0: 723e 3c77 3a72 5072 3e3c 773a 7246 6f6e  r><w:rPr><w:rFon
+000020d0: 7473 2077 3a61 7363 6969 3d22 436f 7572  ts w:ascii="Cour
+000020e0: 6965 7220 4e65 7722 2077 3a68 416e 7369  ier New" w:hAnsi
+000020f0: 3d22 436f 7572 6965 7220 4e65 7722 2077  ="Courier New" w
+00002100: 3a63 733d 2243 6f75 7269 6572 204e 6577  :cs="Courier New
+00002110: 2220 773a 6869 6e74 3d22 6465 6661 756c  " w:hint="defaul
+00002120: 7422 2f3e 3c2f 773a 7250 723e 3c2f 773a  t"/></w:rPr></w:
+00002130: 6c76 6c3e 3c77 3a6c 766c 2077 3a69 6c76  lvl><w:lvl w:ilv
+00002140: 6c3d 2235 2220 773a 7470 6c63 3d22 3230  l="5" w:tplc="20
+00002150: 3030 3030 3035 2220 773a 7465 6e74 6174  000005" w:tentat
+00002160: 6976 653d 2231 223e 3c77 3a73 7461 7274  ive="1"><w:start
+00002170: 2077 3a76 616c 3d22 3122 2f3e 3c77 3a6e   w:val="1"/><w:n
+00002180: 756d 466d 7420 773a 7661 6c3d 2262 756c  umFmt w:val="bul
+00002190: 6c65 7422 2f3e 3c77 3a6c 766c 5465 7874  let"/><w:lvlText
+000021a0: 2077 3a76 616c 3d22 ef82 a722 2f3e 3c77   w:val="..."/><w
+000021b0: 3a6c 766c 4a63 2077 3a76 616c 3d22 6c65  :lvlJc w:val="le
+000021c0: 6674 222f 3e3c 773a 7050 723e 3c77 3a69  ft"/><w:pPr><w:i
+000021d0: 6e64 2077 3a6c 6566 743d 2234 3332 3022  nd w:left="4320"
+000021e0: 2077 3a68 616e 6769 6e67 3d22 3336 3022   w:hanging="360"
+000021f0: 2f3e 3c2f 773a 7050 723e 3c77 3a72 5072  /></w:pPr><w:rPr
+00002200: 3e3c 773a 7246 6f6e 7473 2077 3a61 7363  ><w:rFonts w:asc
+00002210: 6969 3d22 5769 6e67 6469 6e67 7322 2077  ii="Wingdings" w
+00002220: 3a68 416e 7369 3d22 5769 6e67 6469 6e67  :hAnsi="Wingding
+00002230: 7322 2077 3a68 696e 743d 2264 6566 6175  s" w:hint="defau
+00002240: 6c74 222f 3e3c 2f77 3a72 5072 3e3c 2f77  lt"/></w:rPr></w
+00002250: 3a6c 766c 3e3c 773a 6c76 6c20 773a 696c  :lvl><w:lvl w:il
+00002260: 766c 3d22 3622 2077 3a74 706c 633d 2232  vl="6" w:tplc="2
+00002270: 3030 3030 3030 3122 2077 3a74 656e 7461  0000001" w:tenta
+00002280: 7469 7665 3d22 3122 3e3c 773a 7374 6172  tive="1"><w:star
+00002290: 7420 773a 7661 6c3d 2231 222f 3e3c 773a  t w:val="1"/><w:
+000022a0: 6e75 6d46 6d74 2077 3a76 616c 3d22 6275  numFmt w:val="bu
+000022b0: 6c6c 6574 222f 3e3c 773a 6c76 6c54 6578  llet"/><w:lvlTex
+000022c0: 7420 773a 7661 6c3d 22ef 82b7 222f 3e3c  t w:val="..."/><
+000022d0: 773a 6c76 6c4a 6320 773a 7661 6c3d 226c  w:lvlJc w:val="l
+000022e0: 6566 7422 2f3e 3c77 3a70 5072 3e3c 773a  eft"/><w:pPr><w:
+000022f0: 696e 6420 773a 6c65 6674 3d22 3530 3430  ind w:left="5040
+00002300: 2220 773a 6861 6e67 696e 673d 2233 3630  " w:hanging="360
+00002310: 222f 3e3c 2f77 3a70 5072 3e3c 773a 7250  "/></w:pPr><w:rP
+00002320: 723e 3c77 3a72 466f 6e74 7320 773a 6173  r><w:rFonts w:as
+00002330: 6369 693d 2253 796d 626f 6c22 2077 3a68  cii="Symbol" w:h
+00002340: 416e 7369 3d22 5379 6d62 6f6c 2220 773a  Ansi="Symbol" w:
+00002350: 6869 6e74 3d22 6465 6661 756c 7422 2f3e  hint="default"/>
+00002360: 3c2f 773a 7250 723e 3c2f 773a 6c76 6c3e  </w:rPr></w:lvl>
+00002370: 3c77 3a6c 766c 2077 3a69 6c76 6c3d 2237  <w:lvl w:ilvl="7
+00002380: 2220 773a 7470 6c63 3d22 3230 3030 3030  " w:tplc="200000
+00002390: 3033 2220 773a 7465 6e74 6174 6976 653d  03" w:tentative=
+000023a0: 2231 223e 3c77 3a73 7461 7274 2077 3a76  "1"><w:start w:v
+000023b0: 616c 3d22 3122 2f3e 3c77 3a6e 756d 466d  al="1"/><w:numFm
+000023c0: 7420 773a 7661 6c3d 2262 756c 6c65 7422  t w:val="bullet"
+000023d0: 2f3e 3c77 3a6c 766c 5465 7874 2077 3a76  /><w:lvlText w:v
+000023e0: 616c 3d22 6f22 2f3e 3c77 3a6c 766c 4a63  al="o"/><w:lvlJc
+000023f0: 2077 3a76 616c 3d22 6c65 6674 222f 3e3c   w:val="left"/><
+00002400: 773a 7050 723e 3c77 3a69 6e64 2077 3a6c  w:pPr><w:ind w:l
+00002410: 6566 743d 2235 3736 3022 2077 3a68 616e  eft="5760" w:han
+00002420: 6769 6e67 3d22 3336 3022 2f3e 3c2f 773a  ging="360"/></w:
+00002430: 7050 723e 3c77 3a72 5072 3e3c 773a 7246  pPr><w:rPr><w:rF
+00002440: 6f6e 7473 2077 3a61 7363 6969 3d22 436f  onts w:ascii="Co
+00002450: 7572 6965 7220 4e65 7722 2077 3a68 416e  urier New" w:hAn
+00002460: 7369 3d22 436f 7572 6965 7220 4e65 7722  si="Courier New"
+00002470: 2077 3a63 733d 2243 6f75 7269 6572 204e   w:cs="Courier N
+00002480: 6577 2220 773a 6869 6e74 3d22 6465 6661  ew" w:hint="defa
+00002490: 756c 7422 2f3e 3c2f 773a 7250 723e 3c2f  ult"/></w:rPr></
+000024a0: 773a 6c76 6c3e 3c77 3a6c 766c 2077 3a69  w:lvl><w:lvl w:i
+000024b0: 6c76 6c3d 2238 2220 773a 7470 6c63 3d22  lvl="8" w:tplc="
+000024c0: 3230 3030 3030 3035 2220 773a 7465 6e74  20000005" w:tent
+000024d0: 6174 6976 653d 2231 223e 3c77 3a73 7461  ative="1"><w:sta
+000024e0: 7274 2077 3a76 616c 3d22 3122 2f3e 3c77  rt w:val="1"/><w
+000024f0: 3a6e 756d 466d 7420 773a 7661 6c3d 2262  :numFmt w:val="b
+00002500: 756c 6c65 7422 2f3e 3c77 3a6c 766c 5465  ullet"/><w:lvlTe
+00002510: 7874 2077 3a76 616c 3d22 ef82 a722 2f3e  xt w:val="..."/>
+00002520: 3c77 3a6c 766c 4a63 2077 3a76 616c 3d22  <w:lvlJc w:val="
+00002530: 6c65 6674 222f 3e3c 773a 7050 723e 3c77  left"/><w:pPr><w
+00002540: 3a69 6e64 2077 3a6c 6566 743d 2236 3438  :ind w:left="648
+00002550: 3022 2077 3a68 616e 6769 6e67 3d22 3336  0" w:hanging="36
+00002560: 3022 2f3e 3c2f 773a 7050 723e 3c77 3a72  0"/></w:pPr><w:r
+00002570: 5072 3e3c 773a 7246 6f6e 7473 2077 3a61  Pr><w:rFonts w:a
+00002580: 7363 6969 3d22 5769 6e67 6469 6e67 7322  scii="Wingdings"
+00002590: 2077 3a68 416e 7369 3d22 5769 6e67 6469   w:hAnsi="Wingdi
+000025a0: 6e67 7322 2077 3a68 696e 743d 2264 6566  ngs" w:hint="def
+000025b0: 6175 6c74 222f 3e3c 2f77 3a72 5072 3e3c  ault"/></w:rPr><
+000025c0: 2f77 3a6c 766c 3e3c 2f77 3a61 6273 7472  /w:lvl></w:abstr
+000025d0: 6163 744e 756d 3e3c 773a 6162 7374 7261  actNum><w:abstra
+000025e0: 6374 4e75 6d20 773a 6162 7374 7261 6374  ctNum w:abstract
+000025f0: 4e75 6d49 643d 2231 3122 2077 3135 3a72  NumId="11" w15:r
+00002600: 6573 7461 7274 4e75 6d62 6572 696e 6741  estartNumberingA
+00002610: 6674 6572 4272 6561 6b3d 2230 223e 3c77  fterBreak="0"><w
+00002620: 3a6e 7369 6420 773a 7661 6c3d 2233 4643  :nsid w:val="3FC
+00002630: 3935 3343 3022 2f3e 3c77 3a6d 756c 7469  953C0"/><w:multi
+00002640: 4c65 7665 6c54 7970 6520 773a 7661 6c3d  LevelType w:val=
+00002650: 2268 7962 7269 644d 756c 7469 6c65 7665  "hybridMultileve
+00002660: 6c22 2f3e 3c77 3a74 6d70 6c20 773a 7661  l"/><w:tmpl w:va
+00002670: 6c3d 2237 3037 3437 4133 3222 2f3e 3c77  l="70747A32"/><w
+00002680: 3a6c 766c 2077 3a69 6c76 6c3d 2230 2220  :lvl w:ilvl="0" 
+00002690: 773a 7470 6c63 3d22 3230 3030 3030 3046  w:tplc="2000000F
+000026a0: 223e 3c77 3a73 7461 7274 2077 3a76 616c  "><w:start w:val
+000026b0: 3d22 3122 2f3e 3c77 3a6e 756d 466d 7420  ="1"/><w:numFmt 
+000026c0: 773a 7661 6c3d 2264 6563 696d 616c 222f  w:val="decimal"/
+000026d0: 3e3c 773a 6c76 6c54 6578 7420 773a 7661  ><w:lvlText w:va
+000026e0: 6c3d 2225 312e 222f 3e3c 773a 6c76 6c4a  l="%1."/><w:lvlJ
+000026f0: 6320 773a 7661 6c3d 226c 6566 7422 2f3e  c w:val="left"/>
+00002700: 3c77 3a70 5072 3e3c 773a 696e 6420 773a  <w:pPr><w:ind w:
+00002710: 6c65 6674 3d22 3732 3022 2077 3a68 616e  left="720" w:han
+00002720: 6769 6e67 3d22 3336 3022 2f3e 3c2f 773a  ging="360"/></w:
+00002730: 7050 723e 3c2f 773a 6c76 6c3e 3c77 3a6c  pPr></w:lvl><w:l
+00002740: 766c 2077 3a69 6c76 6c3d 2231 2220 773a  vl w:ilvl="1" w:
+00002750: 7470 6c63 3d22 3230 3030 3030 3139 223e  tplc="20000019">
+00002760: 3c77 3a73 7461 7274 2077 3a76 616c 3d22  <w:start w:val="
+00002770: 3122 2f3e 3c77 3a6e 756d 466d 7420 773a  1"/><w:numFmt w:
+00002780: 7661 6c3d 226c 6f77 6572 4c65 7474 6572  val="lowerLetter
+00002790: 222f 3e3c 773a 6c76 6c54 6578 7420 773a  "/><w:lvlText w:
+000027a0: 7661 6c3d 2225 322e 222f 3e3c 773a 6c76  val="%2."/><w:lv
+000027b0: 6c4a 6320 773a 7661 6c3d 226c 6566 7422  lJc w:val="left"
+000027c0: 2f3e 3c77 3a70 5072 3e3c 773a 696e 6420  /><w:pPr><w:ind 
+000027d0: 773a 6c65 6674 3d22 3134 3430 2220 773a  w:left="1440" w:
+000027e0: 6861 6e67 696e 673d 2233 3630 222f 3e3c  hanging="360"/><
+000027f0: 2f77 3a70 5072 3e3c 2f77 3a6c 766c 3e3c  /w:pPr></w:lvl><
+00002800: 773a 6c76 6c20 773a 696c 766c 3d22 3222  w:lvl w:ilvl="2"
+00002810: 2077 3a74 706c 633d 2232 3030 3030 3031   w:tplc="2000001
+00002820: 4222 2077 3a74 656e 7461 7469 7665 3d22  B" w:tentative="
+00002830: 3122 3e3c 773a 7374 6172 7420 773a 7661  1"><w:start w:va
+00002840: 6c3d 2231 222f 3e3c 773a 6e75 6d46 6d74  l="1"/><w:numFmt
+00002850: 2077 3a76 616c 3d22 6c6f 7765 7252 6f6d   w:val="lowerRom
+00002860: 616e 222f 3e3c 773a 6c76 6c54 6578 7420  an"/><w:lvlText 
+00002870: 773a 7661 6c3d 2225 332e 222f 3e3c 773a  w:val="%3."/><w:
+00002880: 6c76 6c4a 6320 773a 7661 6c3d 2272 6967  lvlJc w:val="rig
+00002890: 6874 222f 3e3c 773a 7050 723e 3c77 3a69  ht"/><w:pPr><w:i
+000028a0: 6e64 2077 3a6c 6566 743d 2232 3136 3022  nd w:left="2160"
+000028b0: 2077 3a68 616e 6769 6e67 3d22 3138 3022   w:hanging="180"
+000028c0: 2f3e 3c2f 773a 7050 723e 3c2f 773a 6c76  /></w:pPr></w:lv
+000028d0: 6c3e 3c77 3a6c 766c 2077 3a69 6c76 6c3d  l><w:lvl w:ilvl=
+000028e0: 2233 2220 773a 7470 6c63 3d22 3230 3030  "3" w:tplc="2000
+000028f0: 3030 3046 2220 773a 7465 6e74 6174 6976  000F" w:tentativ
+00002900: 653d 2231 223e 3c77 3a73 7461 7274 2077  e="1"><w:start w
+00002910: 3a76 616c 3d22 3122 2f3e 3c77 3a6e 756d  :val="1"/><w:num
+00002920: 466d 7420 773a 7661 6c3d 2264 6563 696d  Fmt w:val="decim
+00002930: 616c 222f 3e3c 773a 6c76 6c54 6578 7420  al"/><w:lvlText 
+00002940: 773a 7661 6c3d 2225 342e 222f 3e3c 773a  w:val="%4."/><w:
+00002950: 6c76 6c4a 6320 773a 7661 6c3d 226c 6566  lvlJc w:val="lef
+00002960: 7422 2f3e 3c77 3a70 5072 3e3c 773a 696e  t"/><w:pPr><w:in
+00002970: 6420 773a 6c65 6674 3d22 3238 3830 2220  d w:left="2880" 
+00002980: 773a 6861 6e67 696e 673d 2233 3630 222f  w:hanging="360"/
+00002990: 3e3c 2f77 3a70 5072 3e3c 2f77 3a6c 766c  ></w:pPr></w:lvl
+000029a0: 3e3c 773a 6c76 6c20 773a 696c 766c 3d22  ><w:lvl w:ilvl="
+000029b0: 3422 2077 3a74 706c 633d 2232 3030 3030  4" w:tplc="20000
+000029c0: 3031 3922 2077 3a74 656e 7461 7469 7665  019" w:tentative
+000029d0: 3d22 3122 3e3c 773a 7374 6172 7420 773a  ="1"><w:start w:
+000029e0: 7661 6c3d 2231 222f 3e3c 773a 6e75 6d46  val="1"/><w:numF
+000029f0: 6d74 2077 3a76 616c 3d22 6c6f 7765 724c  mt w:val="lowerL
+00002a00: 6574 7465 7222 2f3e 3c77 3a6c 766c 5465  etter"/><w:lvlTe
+00002a10: 7874 2077 3a76 616c 3d22 2535 2e22 2f3e  xt w:val="%5."/>
+00002a20: 3c77 3a6c 766c 4a63 2077 3a76 616c 3d22  <w:lvlJc w:val="
+00002a30: 6c65 6674 222f 3e3c 773a 7050 723e 3c77  left"/><w:pPr><w
+00002a40: 3a69 6e64 2077 3a6c 6566 743d 2233 3630  :ind w:left="360
+00002a50: 3022 2077 3a68 616e 6769 6e67 3d22 3336  0" w:hanging="36
+00002a60: 3022 2f3e 3c2f 773a 7050 723e 3c2f 773a  0"/></w:pPr></w:
+00002a70: 6c76 6c3e 3c77 3a6c 766c 2077 3a69 6c76  lvl><w:lvl w:ilv
+00002a80: 6c3d 2235 2220 773a 7470 6c63 3d22 3230  l="5" w:tplc="20
+00002a90: 3030 3030 3142 2220 773a 7465 6e74 6174  00001B" w:tentat
+00002aa0: 6976 653d 2231 223e 3c77 3a73 7461 7274  ive="1"><w:start
+00002ab0: 2077 3a76 616c 3d22 3122 2f3e 3c77 3a6e   w:val="1"/><w:n
+00002ac0: 756d 466d 7420 773a 7661 6c3d 226c 6f77  umFmt w:val="low
+00002ad0: 6572 526f 6d61 6e22 2f3e 3c77 3a6c 766c  erRoman"/><w:lvl
+00002ae0: 5465 7874 2077 3a76 616c 3d22 2536 2e22  Text w:val="%6."
+00002af0: 2f3e 3c77 3a6c 766c 4a63 2077 3a76 616c  /><w:lvlJc w:val
+00002b00: 3d22 7269 6768 7422 2f3e 3c77 3a70 5072  ="right"/><w:pPr
+00002b10: 3e3c 773a 696e 6420 773a 6c65 6674 3d22  ><w:ind w:left="
+00002b20: 3433 3230 2220 773a 6861 6e67 696e 673d  4320" w:hanging=
+00002b30: 2231 3830 222f 3e3c 2f77 3a70 5072 3e3c  "180"/></w:pPr><
+00002b40: 2f77 3a6c 766c 3e3c 773a 6c76 6c20 773a  /w:lvl><w:lvl w:
+00002b50: 696c 766c 3d22 3622 2077 3a74 706c 633d  ilvl="6" w:tplc=
+00002b60: 2232 3030 3030 3030 4622 2077 3a74 656e  "2000000F" w:ten
+00002b70: 7461 7469 7665 3d22 3122 3e3c 773a 7374  tative="1"><w:st
+00002b80: 6172 7420 773a 7661 6c3d 2231 222f 3e3c  art w:val="1"/><
+00002b90: 773a 6e75 6d46 6d74 2077 3a76 616c 3d22  w:numFmt w:val="
+00002ba0: 6465 6369 6d61 6c22 2f3e 3c77 3a6c 766c  decimal"/><w:lvl
+00002bb0: 5465 7874 2077 3a76 616c 3d22 2537 2e22  Text w:val="%7."
+00002bc0: 2f3e 3c77 3a6c 766c 4a63 2077 3a76 616c  /><w:lvlJc w:val
+00002bd0: 3d22 6c65 6674 222f 3e3c 773a 7050 723e  ="left"/><w:pPr>
+00002be0: 3c77 3a69 6e64 2077 3a6c 6566 743d 2235  <w:ind w:left="5
+00002bf0: 3034 3022 2077 3a68 616e 6769 6e67 3d22  040" w:hanging="
+00002c00: 3336 3022 2f3e 3c2f 773a 7050 723e 3c2f  360"/></w:pPr></
+00002c10: 773a 6c76 6c3e 3c77 3a6c 766c 2077 3a69  w:lvl><w:lvl w:i
+00002c20: 6c76 6c3d 2237 2220 773a 7470 6c63 3d22  lvl="7" w:tplc="
+00002c30: 3230 3030 3030 3139 2220 773a 7465 6e74  20000019" w:tent
+00002c40: 6174 6976 653d 2231 223e 3c77 3a73 7461  ative="1"><w:sta
+00002c50: 7274 2077 3a76 616c 3d22 3122 2f3e 3c77  rt w:val="1"/><w
+00002c60: 3a6e 756d 466d 7420 773a 7661 6c3d 226c  :numFmt w:val="l
+00002c70: 6f77 6572 4c65 7474 6572 222f 3e3c 773a  owerLetter"/><w:
+00002c80: 6c76 6c54 6578 7420 773a 7661 6c3d 2225  lvlText w:val="%
+00002c90: 382e 222f 3e3c 773a 6c76 6c4a 6320 773a  8."/><w:lvlJc w:
+00002ca0: 7661 6c3d 226c 6566 7422 2f3e 3c77 3a70  val="left"/><w:p
+00002cb0: 5072 3e3c 773a 696e 6420 773a 6c65 6674  Pr><w:ind w:left
+00002cc0: 3d22 3537 3630 2220 773a 6861 6e67 696e  ="5760" w:hangin
+00002cd0: 673d 2233 3630 222f 3e3c 2f77 3a70 5072  g="360"/></w:pPr
+00002ce0: 3e3c 2f77 3a6c 766c 3e3c 773a 6c76 6c20  ></w:lvl><w:lvl 
+00002cf0: 773a 696c 766c 3d22 3822 2077 3a74 706c  w:ilvl="8" w:tpl
+00002d00: 633d 2232 3030 3030 3031 4222 2077 3a74  c="2000001B" w:t
+00002d10: 656e 7461 7469 7665 3d22 3122 3e3c 773a  entative="1"><w:
+00002d20: 7374 6172 7420 773a 7661 6c3d 2231 222f  start w:val="1"/
+00002d30: 3e3c 773a 6e75 6d46 6d74 2077 3a76 616c  ><w:numFmt w:val
+00002d40: 3d22 6c6f 7765 7252 6f6d 616e 222f 3e3c  ="lowerRoman"/><
+00002d50: 773a 6c76 6c54 6578 7420 773a 7661 6c3d  w:lvlText w:val=
+00002d60: 2225 392e 222f 3e3c 773a 6c76 6c4a 6320  "%9."/><w:lvlJc 
+00002d70: 773a 7661 6c3d 2272 6967 6874 222f 3e3c  w:val="right"/><
+00002d80: 773a 7050 723e 3c77 3a69 6e64 2077 3a6c  w:pPr><w:ind w:l
+00002d90: 6566 743d 2236 3438 3022 2077 3a68 616e  eft="6480" w:han
+00002da0: 6769 6e67 3d22 3138 3022 2f3e 3c2f 773a  ging="180"/></w:
+00002db0: 7050 723e 3c2f 773a 6c76 6c3e 3c2f 773a  pPr></w:lvl></w:
+00002dc0: 6162 7374 7261 6374 4e75 6d3e 3c77 3a61  abstractNum><w:a
+00002dd0: 6273 7472 6163 744e 756d 2077 3a61 6273  bstractNum w:abs
+00002de0: 7472 6163 744e 756d 4964 3d22 3132 2220  tractNumId="12" 
+00002df0: 7731 353a 7265 7374 6172 744e 756d 6265  w15:restartNumbe
+00002e00: 7269 6e67 4166 7465 7242 7265 616b 3d22  ringAfterBreak="
+00002e10: 3022 3e3c 773a 6e73 6964 2077 3a76 616c  0"><w:nsid w:val
+00002e20: 3d22 3645 4231 3434 3638 222f 3e3c 773a  ="6EB14468"/><w:
+00002e30: 6d75 6c74 694c 6576 656c 5479 7065 2077  multiLevelType w
+00002e40: 3a76 616c 3d22 6879 6272 6964 4d75 6c74  :val="hybridMult
+00002e50: 696c 6576 656c 222f 3e3c 773a 746d 706c  ilevel"/><w:tmpl
+00002e60: 2077 3a76 616c 3d22 3342 4234 4245 3841   w:val="3BB4BE8A
+00002e70: 222f 3e3c 773a 6c76 6c20 773a 696c 766c  "/><w:lvl w:ilvl
+00002e80: 3d22 3022 2077 3a74 706c 633d 2232 3030  ="0" w:tplc="200
+00002e90: 3030 3030 3122 3e3c 773a 7374 6172 7420  00001"><w:start 
+00002ea0: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
+00002eb0: 6d46 6d74 2077 3a76 616c 3d22 6275 6c6c  mFmt w:val="bull
+00002ec0: 6574 222f 3e3c 773a 6c76 6c54 6578 7420  et"/><w:lvlText 
+00002ed0: 773a 7661 6c3d 22ef 82b7 222f 3e3c 773a  w:val="..."/><w:
+00002ee0: 6c76 6c4a 6320 773a 7661 6c3d 226c 6566  lvlJc w:val="lef
+00002ef0: 7422 2f3e 3c77 3a70 5072 3e3c 773a 696e  t"/><w:pPr><w:in
+00002f00: 6420 773a 6c65 6674 3d22 3732 3022 2077  d w:left="720" w
+00002f10: 3a68 616e 6769 6e67 3d22 3336 3022 2f3e  :hanging="360"/>
+00002f20: 3c2f 773a 7050 723e 3c77 3a72 5072 3e3c  </w:pPr><w:rPr><
+00002f30: 773a 7246 6f6e 7473 2077 3a61 7363 6969  w:rFonts w:ascii
+00002f40: 3d22 5379 6d62 6f6c 2220 773a 6841 6e73  ="Symbol" w:hAns
+00002f50: 693d 2253 796d 626f 6c22 2077 3a68 696e  i="Symbol" w:hin
+00002f60: 743d 2264 6566 6175 6c74 222f 3e3c 2f77  t="default"/></w
+00002f70: 3a72 5072 3e3c 2f77 3a6c 766c 3e3c 773a  :rPr></w:lvl><w:
+00002f80: 6c76 6c20 773a 696c 766c 3d22 3122 2077  lvl w:ilvl="1" w
+00002f90: 3a74 706c 633d 2232 3030 3030 3030 3322  :tplc="20000003"
+00002fa0: 2077 3a74 656e 7461 7469 7665 3d22 3122   w:tentative="1"
+00002fb0: 3e3c 773a 7374 6172 7420 773a 7661 6c3d  ><w:start w:val=
+00002fc0: 2231 222f 3e3c 773a 6e75 6d46 6d74 2077  "1"/><w:numFmt w
+00002fd0: 3a76 616c 3d22 6275 6c6c 6574 222f 3e3c  :val="bullet"/><
+00002fe0: 773a 6c76 6c54 6578 7420 773a 7661 6c3d  w:lvlText w:val=
+00002ff0: 226f 222f 3e3c 773a 6c76 6c4a 6320 773a  "o"/><w:lvlJc w:
+00003000: 7661 6c3d 226c 6566 7422 2f3e 3c77 3a70  val="left"/><w:p
+00003010: 5072 3e3c 773a 696e 6420 773a 6c65 6674  Pr><w:ind w:left
+00003020: 3d22 3134 3430 2220 773a 6861 6e67 696e  ="1440" w:hangin
+00003030: 673d 2233 3630 222f 3e3c 2f77 3a70 5072  g="360"/></w:pPr
+00003040: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
+00003050: 7320 773a 6173 6369 693d 2243 6f75 7269  s w:ascii="Couri
+00003060: 6572 204e 6577 2220 773a 6841 6e73 693d  er New" w:hAnsi=
+00003070: 2243 6f75 7269 6572 204e 6577 2220 773a  "Courier New" w:
+00003080: 6373 3d22 436f 7572 6965 7220 4e65 7722  cs="Courier New"
+00003090: 2077 3a68 696e 743d 2264 6566 6175 6c74   w:hint="default
+000030a0: 222f 3e3c 2f77 3a72 5072 3e3c 2f77 3a6c  "/></w:rPr></w:l
+000030b0: 766c 3e3c 773a 6c76 6c20 773a 696c 766c  vl><w:lvl w:ilvl
+000030c0: 3d22 3222 2077 3a74 706c 633d 2232 3030  ="2" w:tplc="200
+000030d0: 3030 3030 3522 2077 3a74 656e 7461 7469  00005" w:tentati
+000030e0: 7665 3d22 3122 3e3c 773a 7374 6172 7420  ve="1"><w:start 
+000030f0: 773a 7661 6c3d 2231 222f 3e3c 773a 6e75  w:val="1"/><w:nu
+00003100: 6d46 6d74 2077 3a76 616c 3d22 6275 6c6c  mFmt w:val="bull
+00003110: 6574 222f 3e3c 773a 6c76 6c54 6578 7420  et"/><w:lvlText 
+00003120: 773a 7661 6c3d 22ef 82a7 222f 3e3c 773a  w:val="..."/><w:
+00003130: 6c76 6c4a 6320 773a 7661 6c3d 226c 6566  lvlJc w:val="lef
+00003140: 7422 2f3e 3c77 3a70 5072 3e3c 773a 696e  t"/><w:pPr><w:in
+00003150: 6420 773a 6c65 6674 3d22 3231 3630 2220  d w:left="2160" 
+00003160: 773a 6861 6e67 696e 673d 2233 3630 222f  w:hanging="360"/
+00003170: 3e3c 2f77 3a70 5072 3e3c 773a 7250 723e  ></w:pPr><w:rPr>
+00003180: 3c77 3a72 466f 6e74 7320 773a 6173 6369  <w:rFonts w:asci
+00003190: 693d 2257 696e 6764 696e 6773 2220 773a  i="Wingdings" w:
+000031a0: 6841 6e73 693d 2257 696e 6764 696e 6773  hAnsi="Wingdings
+000031b0: 2220 773a 6869 6e74 3d22 6465 6661 756c  " w:hint="defaul
+000031c0: 7422 2f3e 3c2f 773a 7250 723e 3c2f 773a  t"/></w:rPr></w:
+000031d0: 6c76 6c3e 3c77 3a6c 766c 2077 3a69 6c76  lvl><w:lvl w:ilv
+000031e0: 6c3d 2233 2220 773a 7470 6c63 3d22 3230  l="3" w:tplc="20
+000031f0: 3030 3030 3031 2220 773a 7465 6e74 6174  000001" w:tentat
+00003200: 6976 653d 2231 223e 3c77 3a73 7461 7274  ive="1"><w:start
+00003210: 2077 3a76 616c 3d22 3122 2f3e 3c77 3a6e   w:val="1"/><w:n
+00003220: 756d 466d 7420 773a 7661 6c3d 2262 756c  umFmt w:val="bul
+00003230: 6c65 7422 2f3e 3c77 3a6c 766c 5465 7874  let"/><w:lvlText
+00003240: 2077 3a76 616c 3d22 ef82 b722 2f3e 3c77   w:val="..."/><w
+00003250: 3a6c 766c 4a63 2077 3a76 616c 3d22 6c65  :lvlJc w:val="le
+00003260: 6674 222f 3e3c 773a 7050 723e 3c77 3a69  ft"/><w:pPr><w:i
+00003270: 6e64 2077 3a6c 6566 743d 2232 3838 3022  nd w:left="2880"
+00003280: 2077 3a68 616e 6769 6e67 3d22 3336 3022   w:hanging="360"
+00003290: 2f3e 3c2f 773a 7050 723e 3c77 3a72 5072  /></w:pPr><w:rPr
+000032a0: 3e3c 773a 7246 6f6e 7473 2077 3a61 7363  ><w:rFonts w:asc
+000032b0: 6969 3d22 5379 6d62 6f6c 2220 773a 6841  ii="Symbol" w:hA
+000032c0: 6e73 693d 2253 796d 626f 6c22 2077 3a68  nsi="Symbol" w:h
+000032d0: 696e 743d 2264 6566 6175 6c74 222f 3e3c  int="default"/><
+000032e0: 2f77 3a72 5072 3e3c 2f77 3a6c 766c 3e3c  /w:rPr></w:lvl><
+000032f0: 773a 6c76 6c20 773a 696c 766c 3d22 3422  w:lvl w:ilvl="4"
+00003300: 2077 3a74 706c 633d 2232 3030 3030 3030   w:tplc="2000000
+00003310: 3322 2077 3a74 656e 7461 7469 7665 3d22  3" w:tentative="
+00003320: 3122 3e3c 773a 7374 6172 7420 773a 7661  1"><w:start w:va
+00003330: 6c3d 2231 222f 3e3c 773a 6e75 6d46 6d74  l="1"/><w:numFmt
+00003340: 2077 3a76 616c 3d22 6275 6c6c 6574 222f   w:val="bullet"/
+00003350: 3e3c 773a 6c76 6c54 6578 7420 773a 7661  ><w:lvlText w:va
+00003360: 6c3d 226f 222f 3e3c 773a 6c76 6c4a 6320  l="o"/><w:lvlJc 
+00003370: 773a 7661 6c3d 226c 6566 7422 2f3e 3c77  w:val="left"/><w
+00003380: 3a70 5072 3e3c 773a 696e 6420 773a 6c65  :pPr><w:ind w:le
+00003390: 6674 3d22 3336 3030 2220 773a 6861 6e67  ft="3600" w:hang
+000033a0: 696e 673d 2233 3630 222f 3e3c 2f77 3a70  ing="360"/></w:p
+000033b0: 5072 3e3c 773a 7250 723e 3c77 3a72 466f  Pr><w:rPr><w:rFo
+000033c0: 6e74 7320 773a 6173 6369 693d 2243 6f75  nts w:ascii="Cou
+000033d0: 7269 6572 204e 6577 2220 773a 6841 6e73  rier New" w:hAns
+000033e0: 693d 2243 6f75 7269 6572 204e 6577 2220  i="Courier New" 
+000033f0: 773a 6373 3d22 436f 7572 6965 7220 4e65  w:cs="Courier Ne
+00003400: 7722 2077 3a68 696e 743d 2264 6566 6175  w" w:hint="defau
+00003410: 6c74 222f 3e3c 2f77 3a72 5072 3e3c 2f77  lt"/></w:rPr></w
+00003420: 3a6c 766c 3e3c 773a 6c76 6c20 773a 696c  :lvl><w:lvl w:il
+00003430: 766c 3d22 3522 2077 3a74 706c 633d 2232  vl="5" w:tplc="2
+00003440: 3030 3030 3030 3522 2077 3a74 656e 7461  0000005" w:tenta
+00003450: 7469 7665 3d22 3122 3e3c 773a 7374 6172  tive="1"><w:star
+00003460: 7420 773a 7661 6c3d 2231 222f 3e3c 773a  t w:val="1"/><w:
+00003470: 6e75 6d46 6d74 2077 3a76 616c 3d22 6275  numFmt w:val="bu
+00003480: 6c6c 6574 222f 3e3c 773a 6c76 6c54 6578  llet"/><w:lvlTex
+00003490: 7420 773a 7661 6c3d 22ef 82a7 222f 3e3c  t w:val="..."/><
+000034a0: 773a 6c76 6c4a 6320 773a 7661 6c3d 226c  w:lvlJc w:val="l
+000034b0: 6566 7422 2f3e 3c77 3a70 5072 3e3c 773a  eft"/><w:pPr><w:
+000034c0: 696e 6420 773a 6c65 6674 3d22 3433 3230  ind w:left="4320
+000034d0: 2220 773a 6861 6e67 696e 673d 2233 3630  " w:hanging="360
+000034e0: 222f 3e3c 2f77 3a70 5072 3e3c 773a 7250  "/></w:pPr><w:rP
+000034f0: 723e 3c77 3a72 466f 6e74 7320 773a 6173  r><w:rFonts w:as
+00003500: 6369 693d 2257 696e 6764 696e 6773 2220  cii="Wingdings" 
+00003510: 773a 6841 6e73 693d 2257 696e 6764 696e  w:hAnsi="Wingdin
+00003520: 6773 2220 773a 6869 6e74 3d22 6465 6661  gs" w:hint="defa
+00003530: 756c 7422 2f3e 3c2f 773a 7250 723e 3c2f  ult"/></w:rPr></
+00003540: 773a 6c76 6c3e 3c77 3a6c 766c 2077 3a69  w:lvl><w:lvl w:i
+00003550: 6c76 6c3d 2236 2220 773a 7470 6c63 3d22  lvl="6" w:tplc="
+00003560: 3230 3030 3030 3031 2220 773a 7465 6e74  20000001" w:tent
+00003570: 6174 6976 653d 2231 223e 3c77 3a73 7461  ative="1"><w:sta
+00003580: 7274 2077 3a76 616c 3d22 3122 2f3e 3c77  rt w:val="1"/><w
+00003590: 3a6e 756d 466d 7420 773a 7661 6c3d 2262  :numFmt w:val="b
+000035a0: 756c 6c65 7422 2f3e 3c77 3a6c 766c 5465  ullet"/><w:lvlTe
+000035b0: 7874 2077 3a76 616c 3d22 ef82 b722 2f3e  xt w:val="..."/>
+000035c0: 3c77 3a6c 766c 4a63 2077 3a76 616c 3d22  <w:lvlJc w:val="
+000035d0: 6c65 6674 222f 3e3c 773a 7050 723e 3c77  left"/><w:pPr><w
+000035e0: 3a69 6e64 2077 3a6c 6566 743d 2235 3034  :ind w:left="504
+000035f0: 3022 2077 3a68 616e 6769 6e67 3d22 3336  0" w:hanging="36
+00003600: 3022 2f3e 3c2f 773a 7050 723e 3c77 3a72  0"/></w:pPr><w:r
+00003610: 5072 3e3c 773a 7246 6f6e 7473 2077 3a61  Pr><w:rFonts w:a
+00003620: 7363 6969 3d22 5379 6d62 6f6c 2220 773a  scii="Symbol" w:
+00003630: 6841 6e73 693d 2253 796d 626f 6c22 2077  hAnsi="Symbol" w
+00003640: 3a68 696e 743d 2264 6566 6175 6c74 222f  :hint="default"/
+00003650: 3e3c 2f77 3a72 5072 3e3c 2f77 3a6c 766c  ></w:rPr></w:lvl
+00003660: 3e3c 773a 6c76 6c20 773a 696c 766c 3d22  ><w:lvl w:ilvl="
+00003670: 3722 2077 3a74 706c 633d 2232 3030 3030  7" w:tplc="20000
+00003680: 3030 3322 2077 3a74 656e 7461 7469 7665  003" w:tentative
+00003690: 3d22 3122 3e3c 773a 7374 6172 7420 773a  ="1"><w:start w:
+000036a0: 7661 6c3d 2231 222f 3e3c 773a 6e75 6d46  val="1"/><w:numF
+000036b0: 6d74 2077 3a76 616c 3d22 6275 6c6c 6574  mt w:val="bullet
+000036c0: 222f 3e3c 773a 6c76 6c54 6578 7420 773a  "/><w:lvlText w:
+000036d0: 7661 6c3d 226f 222f 3e3c 773a 6c76 6c4a  val="o"/><w:lvlJ
+000036e0: 6320 773a 7661 6c3d 226c 6566 7422 2f3e  c w:val="left"/>
+000036f0: 3c77 3a70 5072 3e3c 773a 696e 6420 773a  <w:pPr><w:ind w:
+00003700: 6c65 6674 3d22 3537 3630 2220 773a 6861  left="5760" w:ha
+00003710: 6e67 696e 673d 2233 3630 222f 3e3c 2f77  nging="360"/></w
+00003720: 3a70 5072 3e3c 773a 7250 723e 3c77 3a72  :pPr><w:rPr><w:r
+00003730: 466f 6e74 7320 773a 6173 6369 693d 2243  Fonts w:ascii="C
+00003740: 6f75 7269 6572 204e 6577 2220 773a 6841  ourier New" w:hA
+00003750: 6e73 693d 2243 6f75 7269 6572 204e 6577  nsi="Courier New
+00003760: 2220 773a 6373 3d22 436f 7572 6965 7220  " w:cs="Courier 
+00003770: 4e65 7722 2077 3a68 696e 743d 2264 6566  New" w:hint="def
+00003780: 6175 6c74 222f 3e3c 2f77 3a72 5072 3e3c  ault"/></w:rPr><
+00003790: 2f77 3a6c 766c 3e3c 773a 6c76 6c20 773a  /w:lvl><w:lvl w:
+000037a0: 696c 766c 3d22 3822 2077 3a74 706c 633d  ilvl="8" w:tplc=
+000037b0: 2232 3030 3030 3030 3522 2077 3a74 656e  "20000005" w:ten
+000037c0: 7461 7469 7665 3d22 3122 3e3c 773a 7374  tative="1"><w:st
+000037d0: 6172 7420 773a 7661 6c3d 2231 222f 3e3c  art w:val="1"/><
+000037e0: 773a 6e75 6d46 6d74 2077 3a76 616c 3d22  w:numFmt w:val="
+000037f0: 6275 6c6c 6574 222f 3e3c 773a 6c76 6c54  bullet"/><w:lvlT
+00003800: 6578 7420 773a 7661 6c3d 22ef 82a7 222f  ext w:val="..."/
+00003810: 3e3c 773a 6c76 6c4a 6320 773a 7661 6c3d  ><w:lvlJc w:val=
+00003820: 226c 6566 7422 2f3e 3c77 3a70 5072 3e3c  "left"/><w:pPr><
+00003830: 773a 696e 6420 773a 6c65 6674 3d22 3634  w:ind w:left="64
+00003840: 3830 2220 773a 6861 6e67 696e 673d 2233  80" w:hanging="3
+00003850: 3630 222f 3e3c 2f77 3a70 5072 3e3c 773a  60"/></w:pPr><w:
+00003860: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
+00003870: 6173 6369 693d 2257 696e 6764 696e 6773  ascii="Wingdings
+00003880: 2220 773a 6841 6e73 693d 2257 696e 6764  " w:hAnsi="Wingd
+00003890: 696e 6773 2220 773a 6869 6e74 3d22 6465  ings" w:hint="de
+000038a0: 6661 756c 7422 2f3e 3c2f 773a 7250 723e  fault"/></w:rPr>
+000038b0: 3c2f 773a 6c76 6c3e 3c2f 773a 6162 7374  </w:lvl></w:abst
+000038c0: 7261 6374 4e75 6d3e 3c77 3a6e 756d 2077  ractNum><w:num w
+000038d0: 3a6e 756d 4964 3d22 3122 2077 3136 6369  :numId="1" w16ci
+000038e0: 643a 6475 7261 626c 6549 643d 2233 3732  d:durableId="372
+000038f0: 3237 3336 3135 223e 3c77 3a61 6273 7472  273615"><w:abstr
+00003900: 6163 744e 756d 4964 2077 3a76 616c 3d22  actNumId w:val="
+00003910: 3132 222f 3e3c 2f77 3a6e 756d 3e3c 773a  12"/></w:num><w:
+00003920: 6e75 6d20 773a 6e75 6d49 643d 2232 2220  num w:numId="2" 
+00003930: 7731 3663 6964 3a64 7572 6162 6c65 4964  w16cid:durableId
+00003940: 3d22 3136 3630 3537 3737 3533 223e 3c77  ="1660577753"><w
+00003950: 3a61 6273 7472 6163 744e 756d 4964 2077  :abstractNumId w
+00003960: 3a76 616c 3d22 3131 222f 3e3c 2f77 3a6e  :val="11"/></w:n
+00003970: 756d 3e3c 773a 6e75 6d20 773a 6e75 6d49  um><w:num w:numI
+00003980: 643d 2233 2220 7731 3663 6964 3a64 7572  d="3" w16cid:dur
+00003990: 6162 6c65 4964 3d22 3139 3233 3634 3138  ableId="19236418
+000039a0: 3237 223e 3c77 3a61 6273 7472 6163 744e  27"><w:abstractN
+000039b0: 756d 4964 2077 3a76 616c 3d22 3922 2f3e  umId w:val="9"/>
+000039c0: 3c2f 773a 6e75 6d3e 3c77 3a6e 756d 2077  </w:num><w:num w
+000039d0: 3a6e 756d 4964 3d22 3422 2077 3136 6369  :numId="4" w16ci
+000039e0: 643a 6475 7261 626c 6549 643d 2231 3338  d:durableId="138
+000039f0: 3833 3833 3637 3722 3e3c 773a 6162 7374  8383677"><w:abst
+00003a00: 7261 6374 4e75 6d49 6420 773a 7661 6c3d  ractNumId w:val=
+00003a10: 2231 3022 2f3e 3c2f 773a 6e75 6d3e 3c77  "10"/></w:num><w
+00003a20: 3a6e 756d 2077 3a6e 756d 4964 3d22 3522  :num w:numId="5"
+00003a30: 2077 3136 6369 643a 6475 7261 626c 6549   w16cid:durableI
+00003a40: 643d 2231 3631 3236 3634 3133 3522 3e3c  d="1612664135"><
+00003a50: 773a 6162 7374 7261 6374 4e75 6d49 6420  w:abstractNumId 
+00003a60: 773a 7661 6c3d 2237 222f 3e3c 2f77 3a6e  w:val="7"/></w:n
+00003a70: 756d 3e3c 773a 6e75 6d20 773a 6e75 6d49  um><w:num w:numI
+00003a80: 643d 2236 2220 7731 3663 6964 3a64 7572  d="6" w16cid:dur
+00003a90: 6162 6c65 4964 3d22 3136 3635 3237 3634  ableId="16652764
+00003aa0: 3336 223e 3c77 3a61 6273 7472 6163 744e  36"><w:abstractN
+00003ab0: 756d 4964 2077 3a76 616c 3d22 3622 2f3e  umId w:val="6"/>
+00003ac0: 3c2f 773a 6e75 6d3e 3c77 3a6e 756d 2077  </w:num><w:num w
+00003ad0: 3a6e 756d 4964 3d22 3722 2077 3136 6369  :numId="7" w16ci
+00003ae0: 643a 6475 7261 626c 6549 643d 2231 3630  d:durableId="160
+00003af0: 3539 3632 3834 3722 3e3c 773a 6162 7374  5962847"><w:abst
+00003b00: 7261 6374 4e75 6d49 6420 773a 7661 6c3d  ractNumId w:val=
+00003b10: 2235 222f 3e3c 2f77 3a6e 756d 3e3c 773a  "5"/></w:num><w:
+00003b20: 6e75 6d20 773a 6e75 6d49 643d 2238 2220  num w:numId="8" 
+00003b30: 7731 3663 6964 3a64 7572 6162 6c65 4964  w16cid:durableId
+00003b40: 3d22 3631 3933 3337 3437 3322 3e3c 773a  ="619337473"><w:
+00003b50: 6162 7374 7261 6374 4e75 6d49 6420 773a  abstractNumId w:
+00003b60: 7661 6c3d 2234 222f 3e3c 2f77 3a6e 756d  val="4"/></w:num
+00003b70: 3e3c 773a 6e75 6d20 773a 6e75 6d49 643d  ><w:num w:numId=
+00003b80: 2239 2220 7731 3663 6964 3a64 7572 6162  "9" w16cid:durab
+00003b90: 6c65 4964 3d22 3230 3338 3233 3935 3635  leId="2038239565
+00003ba0: 223e 3c77 3a61 6273 7472 6163 744e 756d  "><w:abstractNum
+00003bb0: 4964 2077 3a76 616c 3d22 3822 2f3e 3c2f  Id w:val="8"/></
+00003bc0: 773a 6e75 6d3e 3c77 3a6e 756d 2077 3a6e  w:num><w:num w:n
+00003bd0: 756d 4964 3d22 3130 2220 7731 3663 6964  umId="10" w16cid
+00003be0: 3a64 7572 6162 6c65 4964 3d22 3138 3338  :durableId="1838
+00003bf0: 3233 3035 3137 223e 3c77 3a61 6273 7472  230517"><w:abstr
+00003c00: 6163 744e 756d 4964 2077 3a76 616c 3d22  actNumId w:val="
+00003c10: 3322 2f3e 3c2f 773a 6e75 6d3e 3c77 3a6e  3"/></w:num><w:n
+00003c20: 756d 2077 3a6e 756d 4964 3d22 3131 2220  um w:numId="11" 
+00003c30: 7731 3663 6964 3a64 7572 6162 6c65 4964  w16cid:durableId
+00003c40: 3d22 3136 3337 3536 3332 3232 223e 3c77  ="1637563222"><w
+00003c50: 3a61 6273 7472 6163 744e 756d 4964 2077  :abstractNumId w
+00003c60: 3a76 616c 3d22 3222 2f3e 3c2f 773a 6e75  :val="2"/></w:nu
+00003c70: 6d3e 3c77 3a6e 756d 2077 3a6e 756d 4964  m><w:num w:numId
+00003c80: 3d22 3132 2220 7731 3663 6964 3a64 7572  ="12" w16cid:dur
+00003c90: 6162 6c65 4964 3d22 3734 3334 3534 3639  ableId="74345469
+00003ca0: 3922 3e3c 773a 6162 7374 7261 6374 4e75  9"><w:abstractNu
+00003cb0: 6d49 6420 773a 7661 6c3d 2231 222f 3e3c  mId w:val="1"/><
+00003cc0: 2f77 3a6e 756d 3e3c 773a 6e75 6d20 773a  /w:num><w:num w:
+00003cd0: 6e75 6d49 643d 2231 3322 2077 3136 6369  numId="13" w16ci
+00003ce0: 643a 6475 7261 626c 6549 643d 2234 3236  d:durableId="426
+00003cf0: 3035 3232 3622 3e3c 773a 6162 7374 7261  05226"><w:abstra
+00003d00: 6374 4e75 6d49 6420 773a 7661 6c3d 2230  ctNumId w:val="0
+00003d10: 222f 3e3c 2f77 3a6e 756d 3e3c 2f77 3a6e  "/></w:num></w:n
+00003d20: 756d 6265 7269 6e67 3e                   umbering>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/settings.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/settings.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (3611), with CRLF line terminators*

 * *Files 1% similar despite different names*

```diff
@@ -1,230 +1,230 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 773a 7365 7474  "yes"?>..<w:sett
-00000040: 696e 6773 2078 6d6c 6e73 3a6d 633d 2268  ings xmlns:mc="h
-00000050: 7474 703a 2f2f 7363 6865 6d61 732e 6f70  ttp://schemas.op
-00000060: 656e 786d 6c66 6f72 6d61 7473 2e6f 7267  enxmlformats.org
-00000070: 2f6d 6172 6b75 702d 636f 6d70 6174 6962  /markup-compatib
-00000080: 696c 6974 792f 3230 3036 2220 786d 6c6e  ility/2006" xmln
-00000090: 733a 6f3d 2275 726e 3a73 6368 656d 6173  s:o="urn:schemas
-000000a0: 2d6d 6963 726f 736f 6674 2d63 6f6d 3a6f  -microsoft-com:o
-000000b0: 6666 6963 653a 6f66 6669 6365 2220 786d  ffice:office" xm
-000000c0: 6c6e 733a 723d 2268 7474 703a 2f2f 7363  lns:r="http://sc
-000000d0: 6865 6d61 732e 6f70 656e 786d 6c66 6f72  hemas.openxmlfor
-000000e0: 6d61 7473 2e6f 7267 2f6f 6666 6963 6544  mats.org/officeD
-000000f0: 6f63 756d 656e 742f 3230 3036 2f72 656c  ocument/2006/rel
-00000100: 6174 696f 6e73 6869 7073 2220 786d 6c6e  ationships" xmln
-00000110: 733a 6d3d 2268 7474 703a 2f2f 7363 6865  s:m="http://sche
-00000120: 6d61 732e 6f70 656e 786d 6c66 6f72 6d61  mas.openxmlforma
-00000130: 7473 2e6f 7267 2f6f 6666 6963 6544 6f63  ts.org/officeDoc
-00000140: 756d 656e 742f 3230 3036 2f6d 6174 6822  ument/2006/math"
-00000150: 2078 6d6c 6e73 3a76 3d22 7572 6e3a 7363   xmlns:v="urn:sc
-00000160: 6865 6d61 732d 6d69 6372 6f73 6f66 742d  hemas-microsoft-
-00000170: 636f 6d3a 766d 6c22 2078 6d6c 6e73 3a77  com:vml" xmlns:w
-00000180: 3130 3d22 7572 6e3a 7363 6865 6d61 732d  10="urn:schemas-
-00000190: 6d69 6372 6f73 6f66 742d 636f 6d3a 6f66  microsoft-com:of
-000001a0: 6669 6365 3a77 6f72 6422 2078 6d6c 6e73  fice:word" xmlns
-000001b0: 3a77 3d22 6874 7470 3a2f 2f73 6368 656d  :w="http://schem
-000001c0: 6173 2e6f 7065 6e78 6d6c 666f 726d 6174  as.openxmlformat
-000001d0: 732e 6f72 672f 776f 7264 7072 6f63 6573  s.org/wordproces
-000001e0: 7369 6e67 6d6c 2f32 3030 362f 6d61 696e  singml/2006/main
-000001f0: 2220 786d 6c6e 733a 7731 343d 2268 7474  " xmlns:w14="htt
-00000200: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
-00000210: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
-00000220: 2f77 6f72 642f 3230 3130 2f77 6f72 646d  /word/2010/wordm
-00000230: 6c22 2078 6d6c 6e73 3a77 3135 3d22 6874  l" xmlns:w15="ht
-00000240: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
-00000250: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
-00000260: 652f 776f 7264 2f32 3031 322f 776f 7264  e/word/2012/word
-00000270: 6d6c 2220 786d 6c6e 733a 7731 3663 6578  ml" xmlns:w16cex
-00000280: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000290: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
-000002a0: 6666 6963 652f 776f 7264 2f32 3031 382f  ffice/word/2018/
-000002b0: 776f 7264 6d6c 2f63 6578 2220 786d 6c6e  wordml/cex" xmln
-000002c0: 733a 7731 3663 6964 3d22 6874 7470 3a2f  s:w16cid="http:/
-000002d0: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
-000002e0: 6674 2e63 6f6d 2f6f 6666 6963 652f 776f  ft.com/office/wo
-000002f0: 7264 2f32 3031 362f 776f 7264 6d6c 2f63  rd/2016/wordml/c
-00000300: 6964 2220 786d 6c6e 733a 7731 363d 2268  id" xmlns:w16="h
-00000310: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-00000320: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-00000330: 6365 2f77 6f72 642f 3230 3138 2f77 6f72  ce/word/2018/wor
-00000340: 646d 6c22 2078 6d6c 6e73 3a77 3136 7364  dml" xmlns:w16sd
-00000350: 7464 683d 2268 7474 703a 2f2f 7363 6865  tdh="http://sche
-00000360: 6d61 732e 6d69 6372 6f73 6f66 742e 636f  mas.microsoft.co
-00000370: 6d2f 6f66 6669 6365 2f77 6f72 642f 3230  m/office/word/20
-00000380: 3230 2f77 6f72 646d 6c2f 7364 7464 6174  20/wordml/sdtdat
-00000390: 6168 6173 6822 2078 6d6c 6e73 3a77 3136  ahash" xmlns:w16
-000003a0: 7365 3d22 6874 7470 3a2f 2f73 6368 656d  se="http://schem
-000003b0: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-000003c0: 2f6f 6666 6963 652f 776f 7264 2f32 3031  /office/word/201
-000003d0: 352f 776f 7264 6d6c 2f73 796d 6578 2220  5/wordml/symex" 
-000003e0: 786d 6c6e 733a 736c 3d22 6874 7470 3a2f  xmlns:sl="http:/
-000003f0: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
-00000400: 666f 726d 6174 732e 6f72 672f 7363 6865  formats.org/sche
-00000410: 6d61 4c69 6272 6172 792f 3230 3036 2f6d  maLibrary/2006/m
-00000420: 6169 6e22 206d 633a 4967 6e6f 7261 626c  ain" mc:Ignorabl
-00000430: 653d 2277 3134 2077 3135 2077 3136 7365  e="w14 w15 w16se
-00000440: 2077 3136 6369 6420 7731 3620 7731 3663   w16cid w16 w16c
-00000450: 6578 2077 3136 7364 7464 6822 3e3c 773a  ex w16sdtdh"><w:
-00000460: 7a6f 6f6d 2077 3a70 6572 6365 6e74 3d22  zoom w:percent="
-00000470: 3130 3022 2f3e 3c77 3a72 656d 6f76 6550  100"/><w:removeP
-00000480: 6572 736f 6e61 6c49 6e66 6f72 6d61 7469  ersonalInformati
-00000490: 6f6e 2f3e 3c77 3a72 656d 6f76 6544 6174  on/><w:removeDat
-000004a0: 6541 6e64 5469 6d65 2f3e 3c77 3a73 7479  eAndTime/><w:sty
-000004b0: 6c65 5061 6e65 466f 726d 6174 4669 6c74  lePaneFormatFilt
-000004c0: 6572 2077 3a76 616c 3d22 3134 3234 2220  er w:val="1424" 
-000004d0: 773a 616c 6c53 7479 6c65 733d 2230 2220  w:allStyles="0" 
-000004e0: 773a 6375 7374 6f6d 5374 796c 6573 3d22  w:customStyles="
-000004f0: 3022 2077 3a6c 6174 656e 7453 7479 6c65  0" w:latentStyle
-00000500: 733d 2231 2220 773a 7374 796c 6573 496e  s="1" w:stylesIn
-00000510: 5573 653d 2230 2220 773a 6865 6164 696e  Use="0" w:headin
-00000520: 6753 7479 6c65 733d 2231 2220 773a 6e75  gStyles="1" w:nu
-00000530: 6d62 6572 696e 6753 7479 6c65 733d 2230  mberingStyles="0
-00000540: 2220 773a 7461 626c 6553 7479 6c65 733d  " w:tableStyles=
-00000550: 2230 2220 773a 6469 7265 6374 466f 726d  "0" w:directForm
-00000560: 6174 7469 6e67 4f6e 5275 6e73 3d22 3022  attingOnRuns="0"
-00000570: 2077 3a64 6972 6563 7446 6f72 6d61 7474   w:directFormatt
-00000580: 696e 674f 6e50 6172 6167 7261 7068 733d  ingOnParagraphs=
-00000590: 2230 2220 773a 6469 7265 6374 466f 726d  "0" w:directForm
-000005a0: 6174 7469 6e67 4f6e 4e75 6d62 6572 696e  attingOnNumberin
-000005b0: 673d 2231 2220 773a 6469 7265 6374 466f  g="1" w:directFo
-000005c0: 726d 6174 7469 6e67 4f6e 5461 626c 6573  rmattingOnTables
-000005d0: 3d22 3022 2077 3a63 6c65 6172 466f 726d  ="0" w:clearForm
-000005e0: 6174 7469 6e67 3d22 3122 2077 3a74 6f70  atting="1" w:top
-000005f0: 3348 6561 6469 6e67 5374 796c 6573 3d22  3HeadingStyles="
-00000600: 3022 2077 3a76 6973 6962 6c65 5374 796c  0" w:visibleStyl
-00000610: 6573 3d22 3022 2077 3a61 6c74 6572 6e61  es="0" w:alterna
-00000620: 7465 5374 796c 654e 616d 6573 3d22 3022  teStyleNames="0"
-00000630: 2f3e 3c77 3a64 6566 6175 6c74 5461 6253  /><w:defaultTabS
-00000640: 746f 7020 773a 7661 6c3d 2237 3230 222f  top w:val="720"/
-00000650: 3e3c 773a 6368 6172 6163 7465 7253 7061  ><w:characterSpa
-00000660: 6369 6e67 436f 6e74 726f 6c20 773a 7661  cingControl w:va
-00000670: 6c3d 2264 6f4e 6f74 436f 6d70 7265 7373  l="doNotCompress
-00000680: 222f 3e3c 773a 636f 6d70 6174 3e3c 773a  "/><w:compat><w:
-00000690: 636f 6d70 6174 5365 7474 696e 6720 773a  compatSetting w:
-000006a0: 6e61 6d65 3d22 636f 6d70 6174 6962 696c  name="compatibil
-000006b0: 6974 794d 6f64 6522 2077 3a75 7269 3d22  ityMode" w:uri="
-000006c0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
-000006d0: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
-000006e0: 6963 652f 776f 7264 2220 773a 7661 6c3d  ice/word" w:val=
-000006f0: 2231 3522 2f3e 3c77 3a63 6f6d 7061 7453  "15"/><w:compatS
-00000700: 6574 7469 6e67 2077 3a6e 616d 653d 226f  etting w:name="o
-00000710: 7665 7272 6964 6554 6162 6c65 5374 796c  verrideTableStyl
-00000720: 6546 6f6e 7453 697a 6541 6e64 4a75 7374  eFontSizeAndJust
-00000730: 6966 6963 6174 696f 6e22 2077 3a75 7269  ification" w:uri
-00000740: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000750: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
-00000760: 6666 6963 652f 776f 7264 2220 773a 7661  ffice/word" w:va
-00000770: 6c3d 2231 222f 3e3c 773a 636f 6d70 6174  l="1"/><w:compat
-00000780: 5365 7474 696e 6720 773a 6e61 6d65 3d22  Setting w:name="
-00000790: 656e 6162 6c65 4f70 656e 5479 7065 4665  enableOpenTypeFe
-000007a0: 6174 7572 6573 2220 773a 7572 693d 2268  atures" w:uri="h
-000007b0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-000007c0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-000007d0: 6365 2f77 6f72 6422 2077 3a76 616c 3d22  ce/word" w:val="
-000007e0: 3122 2f3e 3c77 3a63 6f6d 7061 7453 6574  1"/><w:compatSet
-000007f0: 7469 6e67 2077 3a6e 616d 653d 2264 6f4e  ting w:name="doN
-00000800: 6f74 466c 6970 4d69 7272 6f72 496e 6465  otFlipMirrorInde
-00000810: 6e74 7322 2077 3a75 7269 3d22 6874 7470  nts" w:uri="http
-00000820: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-00000830: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-00000840: 776f 7264 2220 773a 7661 6c3d 2231 222f  word" w:val="1"/
-00000850: 3e3c 773a 636f 6d70 6174 5365 7474 696e  ><w:compatSettin
-00000860: 6720 773a 6e61 6d65 3d22 6469 6666 6572  g w:name="differ
-00000870: 656e 7469 6174 654d 756c 7469 726f 7754  entiateMultirowT
-00000880: 6162 6c65 4865 6164 6572 7322 2077 3a75  ableHeaders" w:u
-00000890: 7269 3d22 6874 7470 3a2f 2f73 6368 656d  ri="http://schem
-000008a0: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-000008b0: 2f6f 6666 6963 652f 776f 7264 2220 773a  /office/word" w:
-000008c0: 7661 6c3d 2231 222f 3e3c 773a 636f 6d70  val="1"/><w:comp
-000008d0: 6174 5365 7474 696e 6720 773a 6e61 6d65  atSetting w:name
-000008e0: 3d22 7573 6557 6f72 6432 3031 3354 7261  ="useWord2013Tra
-000008f0: 636b 426f 7474 6f6d 4879 7068 656e 6174  ckBottomHyphenat
-00000900: 696f 6e22 2077 3a75 7269 3d22 6874 7470  ion" w:uri="http
-00000910: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-00000920: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-00000930: 776f 7264 2220 773a 7661 6c3d 2230 222f  word" w:val="0"/
-00000940: 3e3c 2f77 3a63 6f6d 7061 743e 3c77 3a72  ></w:compat><w:r
-00000950: 7369 6473 3e3c 773a 7273 6964 526f 6f74  sids><w:rsidRoot
-00000960: 2077 3a76 616c 3d22 3030 3546 3443 3532   w:val="005F4C52
-00000970: 222f 3e3c 773a 7273 6964 2077 3a76 616c  "/><w:rsid w:val
-00000980: 3d22 3030 3035 3144 3334 222f 3e3c 773a  ="00051D34"/><w:
-00000990: 7273 6964 2077 3a76 616c 3d22 3030 3042  rsid w:val="000B
-000009a0: 3746 3733 222f 3e3c 773a 7273 6964 2077  7F73"/><w:rsid w
-000009b0: 3a76 616c 3d22 3030 3136 3333 3736 222f  :val="00163376"/
-000009c0: 3e3c 773a 7273 6964 2077 3a76 616c 3d22  ><w:rsid w:val="
-000009d0: 3030 3144 3438 4246 222f 3e3c 773a 7273  001D48BF"/><w:rs
-000009e0: 6964 2077 3a76 616c 3d22 3030 3336 3236  id w:val="003626
-000009f0: 4534 222f 3e3c 773a 7273 6964 2077 3a76  E4"/><w:rsid w:v
-00000a00: 616c 3d22 3030 3546 3443 3532 222f 3e3c  al="005F4C52"/><
-00000a10: 773a 7273 6964 2077 3a76 616c 3d22 3030  w:rsid w:val="00
-00000a20: 3733 3431 4634 222f 3e3c 773a 7273 6964  7341F4"/><w:rsid
-00000a30: 2077 3a76 616c 3d22 3030 3736 3544 3735   w:val="00765D75
-00000a40: 222f 3e3c 773a 7273 6964 2077 3a76 616c  "/><w:rsid w:val
-00000a50: 3d22 3030 3745 3443 3439 222f 3e3c 773a  ="007E4C49"/><w:
-00000a60: 7273 6964 2077 3a76 616c 3d22 3030 3834  rsid w:val="0084
-00000a70: 3238 3844 222f 3e3c 773a 7273 6964 2077  288D"/><w:rsid w
-00000a80: 3a76 616c 3d22 3030 3938 3632 3338 222f  :val="00986238"/
-00000a90: 3e3c 773a 7273 6964 2077 3a76 616c 3d22  ><w:rsid w:val="
-00000aa0: 3030 3944 3035 3733 222f 3e3c 773a 7273  009D0573"/><w:rs
-00000ab0: 6964 2077 3a76 616c 3d22 3030 3945 3636  id w:val="009E66
-00000ac0: 3345 222f 3e3c 773a 7273 6964 2077 3a76  3E"/><w:rsid w:v
-00000ad0: 616c 3d22 3030 4437 3235 3541 222f 3e3c  al="00D7255A"/><
-00000ae0: 2f77 3a72 7369 6473 3e3c 6d3a 6d61 7468  /w:rsids><m:math
-00000af0: 5072 3e3c 6d3a 6d61 7468 466f 6e74 206d  Pr><m:mathFont m
-00000b00: 3a76 616c 3d22 4361 6d62 7269 6120 4d61  :val="Cambria Ma
-00000b10: 7468 222f 3e3c 6d3a 6272 6b42 696e 206d  th"/><m:brkBin m
-00000b20: 3a76 616c 3d22 6265 666f 7265 222f 3e3c  :val="before"/><
-00000b30: 6d3a 6272 6b42 696e 5375 6220 6d3a 7661  m:brkBinSub m:va
-00000b40: 6c3d 222d 2d22 2f3e 3c6d 3a73 6d61 6c6c  l="--"/><m:small
-00000b50: 4672 6163 206d 3a76 616c 3d22 3022 2f3e  Frac m:val="0"/>
-00000b60: 3c6d 3a64 6973 7044 6566 2f3e 3c6d 3a6c  <m:dispDef/><m:l
-00000b70: 4d61 7267 696e 206d 3a76 616c 3d22 3022  Margin m:val="0"
-00000b80: 2f3e 3c6d 3a72 4d61 7267 696e 206d 3a76  /><m:rMargin m:v
-00000b90: 616c 3d22 3022 2f3e 3c6d 3a64 6566 4a63  al="0"/><m:defJc
-00000ba0: 206d 3a76 616c 3d22 6365 6e74 6572 4772   m:val="centerGr
-00000bb0: 6f75 7022 2f3e 3c6d 3a77 7261 7049 6e64  oup"/><m:wrapInd
-00000bc0: 656e 7420 6d3a 7661 6c3d 2231 3434 3022  ent m:val="1440"
-00000bd0: 2f3e 3c6d 3a69 6e74 4c69 6d20 6d3a 7661  /><m:intLim m:va
-00000be0: 6c3d 2273 7562 5375 7022 2f3e 3c6d 3a6e  l="subSup"/><m:n
-00000bf0: 6172 794c 696d 206d 3a76 616c 3d22 756e  aryLim m:val="un
-00000c00: 644f 7672 222f 3e3c 2f6d 3a6d 6174 6850  dOvr"/></m:mathP
-00000c10: 723e 3c77 3a74 6865 6d65 466f 6e74 4c61  r><w:themeFontLa
-00000c20: 6e67 2077 3a76 616c 3d22 656e 2d44 4522  ng w:val="en-DE"
-00000c30: 2f3e 3c77 3a63 6c72 5363 6865 6d65 4d61  /><w:clrSchemeMa
-00000c40: 7070 696e 6720 773a 6267 313d 226c 6967  pping w:bg1="lig
-00000c50: 6874 3122 2077 3a74 313d 2264 6172 6b31  ht1" w:t1="dark1
-00000c60: 2220 773a 6267 323d 226c 6967 6874 3222  " w:bg2="light2"
-00000c70: 2077 3a74 323d 2264 6172 6b32 2220 773a   w:t2="dark2" w:
-00000c80: 6163 6365 6e74 313d 2261 6363 656e 7431  accent1="accent1
-00000c90: 2220 773a 6163 6365 6e74 323d 2261 6363  " w:accent2="acc
-00000ca0: 656e 7432 2220 773a 6163 6365 6e74 333d  ent2" w:accent3=
-00000cb0: 2261 6363 656e 7433 2220 773a 6163 6365  "accent3" w:acce
-00000cc0: 6e74 343d 2261 6363 656e 7434 2220 773a  nt4="accent4" w:
-00000cd0: 6163 6365 6e74 353d 2261 6363 656e 7435  accent5="accent5
-00000ce0: 2220 773a 6163 6365 6e74 363d 2261 6363  " w:accent6="acc
-00000cf0: 656e 7436 2220 773a 6879 7065 726c 696e  ent6" w:hyperlin
-00000d00: 6b3d 2268 7970 6572 6c69 6e6b 2220 773a  k="hyperlink" w:
-00000d10: 666f 6c6c 6f77 6564 4879 7065 726c 696e  followedHyperlin
-00000d20: 6b3d 2266 6f6c 6c6f 7765 6448 7970 6572  k="followedHyper
-00000d30: 6c69 6e6b 222f 3e3c 773a 7368 6170 6544  link"/><w:shapeD
-00000d40: 6566 6175 6c74 733e 3c6f 3a73 6861 7065  efaults><o:shape
-00000d50: 6465 6661 756c 7473 2076 3a65 7874 3d22  defaults v:ext="
-00000d60: 6564 6974 2220 7370 6964 6d61 783d 2231  edit" spidmax="1
-00000d70: 3032 3622 2f3e 3c6f 3a73 6861 7065 6c61  026"/><o:shapela
-00000d80: 796f 7574 2076 3a65 7874 3d22 6564 6974  yout v:ext="edit
-00000d90: 223e 3c6f 3a69 646d 6170 2076 3a65 7874  "><o:idmap v:ext
-00000da0: 3d22 6564 6974 2220 6461 7461 3d22 3122  ="edit" data="1"
-00000db0: 2f3e 3c2f 6f3a 7368 6170 656c 6179 6f75  /></o:shapelayou
-00000dc0: 743e 3c2f 773a 7368 6170 6544 6566 6175  t></w:shapeDefau
-00000dd0: 6c74 733e 3c77 3a64 6563 696d 616c 5379  lts><w:decimalSy
-00000de0: 6d62 6f6c 2077 3a76 616c 3d22 2c22 2f3e  mbol w:val=","/>
-00000df0: 3c77 3a6c 6973 7453 6570 6172 6174 6f72  <w:listSeparator
-00000e00: 2077 3a76 616c 3d22 2c22 2f3e 3c77 3134   w:val=","/><w14
-00000e10: 3a64 6f63 4964 2077 3134 3a76 616c 3d22  :docId w14:val="
-00000e20: 3334 4643 3634 3945 222f 3e3c 7731 353a  34FC649E"/><w15:
-00000e30: 6368 6172 7454 7261 636b 696e 6752 6566  chartTrackingRef
-00000e40: 4261 7365 642f 3e3c 2f77 3a73 6574 7469  Based/></w:setti
-00000e50: 6e67 733e                                ngs>
+00000030: 2279 6573 223f 3e0a 3c77 3a73 6574 7469  "yes"?>.<w:setti
+00000040: 6e67 7320 786d 6c6e 733a 6d63 3d22 6874  ngs xmlns:mc="ht
+00000050: 7470 3a2f 2f73 6368 656d 6173 2e6f 7065  tp://schemas.ope
+00000060: 6e78 6d6c 666f 726d 6174 732e 6f72 672f  nxmlformats.org/
+00000070: 6d61 726b 7570 2d63 6f6d 7061 7469 6269  markup-compatibi
+00000080: 6c69 7479 2f32 3030 3622 2078 6d6c 6e73  lity/2006" xmlns
+00000090: 3a6f 3d22 7572 6e3a 7363 6865 6d61 732d  :o="urn:schemas-
+000000a0: 6d69 6372 6f73 6f66 742d 636f 6d3a 6f66  microsoft-com:of
+000000b0: 6669 6365 3a6f 6666 6963 6522 2078 6d6c  fice:office" xml
+000000c0: 6e73 3a72 3d22 6874 7470 3a2f 2f73 6368  ns:r="http://sch
+000000d0: 656d 6173 2e6f 7065 6e78 6d6c 666f 726d  emas.openxmlform
+000000e0: 6174 732e 6f72 672f 6f66 6669 6365 446f  ats.org/officeDo
+000000f0: 6375 6d65 6e74 2f32 3030 362f 7265 6c61  cument/2006/rela
+00000100: 7469 6f6e 7368 6970 7322 2078 6d6c 6e73  tionships" xmlns
+00000110: 3a6d 3d22 6874 7470 3a2f 2f73 6368 656d  :m="http://schem
+00000120: 6173 2e6f 7065 6e78 6d6c 666f 726d 6174  as.openxmlformat
+00000130: 732e 6f72 672f 6f66 6669 6365 446f 6375  s.org/officeDocu
+00000140: 6d65 6e74 2f32 3030 362f 6d61 7468 2220  ment/2006/math" 
+00000150: 786d 6c6e 733a 763d 2275 726e 3a73 6368  xmlns:v="urn:sch
+00000160: 656d 6173 2d6d 6963 726f 736f 6674 2d63  emas-microsoft-c
+00000170: 6f6d 3a76 6d6c 2220 786d 6c6e 733a 7731  om:vml" xmlns:w1
+00000180: 303d 2275 726e 3a73 6368 656d 6173 2d6d  0="urn:schemas-m
+00000190: 6963 726f 736f 6674 2d63 6f6d 3a6f 6666  icrosoft-com:off
+000001a0: 6963 653a 776f 7264 2220 786d 6c6e 733a  ice:word" xmlns:
+000001b0: 773d 2268 7474 703a 2f2f 7363 6865 6d61  w="http://schema
+000001c0: 732e 6f70 656e 786d 6c66 6f72 6d61 7473  s.openxmlformats
+000001d0: 2e6f 7267 2f77 6f72 6470 726f 6365 7373  .org/wordprocess
+000001e0: 696e 676d 6c2f 3230 3036 2f6d 6169 6e22  ingml/2006/main"
+000001f0: 2078 6d6c 6e73 3a77 3134 3d22 6874 7470   xmlns:w14="http
+00000200: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
+00000210: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
+00000220: 776f 7264 2f32 3031 302f 776f 7264 6d6c  word/2010/wordml
+00000230: 2220 786d 6c6e 733a 7731 353d 2268 7474  " xmlns:w15="htt
+00000240: 703a 2f2f 7363 6865 6d61 732e 6d69 6372  p://schemas.micr
+00000250: 6f73 6f66 742e 636f 6d2f 6f66 6669 6365  osoft.com/office
+00000260: 2f77 6f72 642f 3230 3132 2f77 6f72 646d  /word/2012/wordm
+00000270: 6c22 2078 6d6c 6e73 3a77 3136 6365 783d  l" xmlns:w16cex=
+00000280: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+00000290: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
+000002a0: 6669 6365 2f77 6f72 642f 3230 3138 2f77  fice/word/2018/w
+000002b0: 6f72 646d 6c2f 6365 7822 2078 6d6c 6e73  ordml/cex" xmlns
+000002c0: 3a77 3136 6369 643d 2268 7474 703a 2f2f  :w16cid="http://
+000002d0: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
+000002e0: 742e 636f 6d2f 6f66 6669 6365 2f77 6f72  t.com/office/wor
+000002f0: 642f 3230 3136 2f77 6f72 646d 6c2f 6369  d/2016/wordml/ci
+00000300: 6422 2078 6d6c 6e73 3a77 3136 3d22 6874  d" xmlns:w16="ht
+00000310: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+00000320: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+00000330: 652f 776f 7264 2f32 3031 382f 776f 7264  e/word/2018/word
+00000340: 6d6c 2220 786d 6c6e 733a 7731 3673 6474  ml" xmlns:w16sdt
+00000350: 6468 3d22 6874 7470 3a2f 2f73 6368 656d  dh="http://schem
+00000360: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
+00000370: 2f6f 6666 6963 652f 776f 7264 2f32 3032  /office/word/202
+00000380: 302f 776f 7264 6d6c 2f73 6474 6461 7461  0/wordml/sdtdata
+00000390: 6861 7368 2220 786d 6c6e 733a 7731 3673  hash" xmlns:w16s
+000003a0: 653d 2268 7474 703a 2f2f 7363 6865 6d61  e="http://schema
+000003b0: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+000003c0: 6f66 6669 6365 2f77 6f72 642f 3230 3135  office/word/2015
+000003d0: 2f77 6f72 646d 6c2f 7379 6d65 7822 2078  /wordml/symex" x
+000003e0: 6d6c 6e73 3a73 6c3d 2268 7474 703a 2f2f  mlns:sl="http://
+000003f0: 7363 6865 6d61 732e 6f70 656e 786d 6c66  schemas.openxmlf
+00000400: 6f72 6d61 7473 2e6f 7267 2f73 6368 656d  ormats.org/schem
+00000410: 614c 6962 7261 7279 2f32 3030 362f 6d61  aLibrary/2006/ma
+00000420: 696e 2220 6d63 3a49 676e 6f72 6162 6c65  in" mc:Ignorable
+00000430: 3d22 7731 3420 7731 3520 7731 3673 6520  ="w14 w15 w16se 
+00000440: 7731 3663 6964 2077 3136 2077 3136 6365  w16cid w16 w16ce
+00000450: 7820 7731 3673 6474 6468 223e 3c77 3a7a  x w16sdtdh"><w:z
+00000460: 6f6f 6d20 773a 7065 7263 656e 743d 2231  oom w:percent="1
+00000470: 3030 222f 3e3c 773a 7265 6d6f 7665 5065  00"/><w:removePe
+00000480: 7273 6f6e 616c 496e 666f 726d 6174 696f  rsonalInformatio
+00000490: 6e2f 3e3c 773a 7265 6d6f 7665 4461 7465  n/><w:removeDate
+000004a0: 416e 6454 696d 652f 3e3c 773a 7374 796c  AndTime/><w:styl
+000004b0: 6550 616e 6546 6f72 6d61 7446 696c 7465  ePaneFormatFilte
+000004c0: 7220 773a 7661 6c3d 2231 3432 3422 2077  r w:val="1424" w
+000004d0: 3a61 6c6c 5374 796c 6573 3d22 3022 2077  :allStyles="0" w
+000004e0: 3a63 7573 746f 6d53 7479 6c65 733d 2230  :customStyles="0
+000004f0: 2220 773a 6c61 7465 6e74 5374 796c 6573  " w:latentStyles
+00000500: 3d22 3122 2077 3a73 7479 6c65 7349 6e55  ="1" w:stylesInU
+00000510: 7365 3d22 3022 2077 3a68 6561 6469 6e67  se="0" w:heading
+00000520: 5374 796c 6573 3d22 3122 2077 3a6e 756d  Styles="1" w:num
+00000530: 6265 7269 6e67 5374 796c 6573 3d22 3022  beringStyles="0"
+00000540: 2077 3a74 6162 6c65 5374 796c 6573 3d22   w:tableStyles="
+00000550: 3022 2077 3a64 6972 6563 7446 6f72 6d61  0" w:directForma
+00000560: 7474 696e 674f 6e52 756e 733d 2230 2220  ttingOnRuns="0" 
+00000570: 773a 6469 7265 6374 466f 726d 6174 7469  w:directFormatti
+00000580: 6e67 4f6e 5061 7261 6772 6170 6873 3d22  ngOnParagraphs="
+00000590: 3022 2077 3a64 6972 6563 7446 6f72 6d61  0" w:directForma
+000005a0: 7474 696e 674f 6e4e 756d 6265 7269 6e67  ttingOnNumbering
+000005b0: 3d22 3122 2077 3a64 6972 6563 7446 6f72  ="1" w:directFor
+000005c0: 6d61 7474 696e 674f 6e54 6162 6c65 733d  mattingOnTables=
+000005d0: 2230 2220 773a 636c 6561 7246 6f72 6d61  "0" w:clearForma
+000005e0: 7474 696e 673d 2231 2220 773a 746f 7033  tting="1" w:top3
+000005f0: 4865 6164 696e 6753 7479 6c65 733d 2230  HeadingStyles="0
+00000600: 2220 773a 7669 7369 626c 6553 7479 6c65  " w:visibleStyle
+00000610: 733d 2230 2220 773a 616c 7465 726e 6174  s="0" w:alternat
+00000620: 6553 7479 6c65 4e61 6d65 733d 2230 222f  eStyleNames="0"/
+00000630: 3e3c 773a 6465 6661 756c 7454 6162 5374  ><w:defaultTabSt
+00000640: 6f70 2077 3a76 616c 3d22 3732 3022 2f3e  op w:val="720"/>
+00000650: 3c77 3a63 6861 7261 6374 6572 5370 6163  <w:characterSpac
+00000660: 696e 6743 6f6e 7472 6f6c 2077 3a76 616c  ingControl w:val
+00000670: 3d22 646f 4e6f 7443 6f6d 7072 6573 7322  ="doNotCompress"
+00000680: 2f3e 3c77 3a63 6f6d 7061 743e 3c77 3a63  /><w:compat><w:c
+00000690: 6f6d 7061 7453 6574 7469 6e67 2077 3a6e  ompatSetting w:n
+000006a0: 616d 653d 2263 6f6d 7061 7469 6269 6c69  ame="compatibili
+000006b0: 7479 4d6f 6465 2220 773a 7572 693d 2268  tyMode" w:uri="h
+000006c0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
+000006d0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
+000006e0: 6365 2f77 6f72 6422 2077 3a76 616c 3d22  ce/word" w:val="
+000006f0: 3135 222f 3e3c 773a 636f 6d70 6174 5365  15"/><w:compatSe
+00000700: 7474 696e 6720 773a 6e61 6d65 3d22 6f76  tting w:name="ov
+00000710: 6572 7269 6465 5461 626c 6553 7479 6c65  errideTableStyle
+00000720: 466f 6e74 5369 7a65 416e 644a 7573 7469  FontSizeAndJusti
+00000730: 6669 6361 7469 6f6e 2220 773a 7572 693d  fication" w:uri=
+00000740: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+00000750: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
+00000760: 6669 6365 2f77 6f72 6422 2077 3a76 616c  fice/word" w:val
+00000770: 3d22 3122 2f3e 3c77 3a63 6f6d 7061 7453  ="1"/><w:compatS
+00000780: 6574 7469 6e67 2077 3a6e 616d 653d 2265  etting w:name="e
+00000790: 6e61 626c 654f 7065 6e54 7970 6546 6561  nableOpenTypeFea
+000007a0: 7475 7265 7322 2077 3a75 7269 3d22 6874  tures" w:uri="ht
+000007b0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+000007c0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+000007d0: 652f 776f 7264 2220 773a 7661 6c3d 2231  e/word" w:val="1
+000007e0: 222f 3e3c 773a 636f 6d70 6174 5365 7474  "/><w:compatSett
+000007f0: 696e 6720 773a 6e61 6d65 3d22 646f 4e6f  ing w:name="doNo
+00000800: 7446 6c69 704d 6972 726f 7249 6e64 656e  tFlipMirrorInden
+00000810: 7473 2220 773a 7572 693d 2268 7474 703a  ts" w:uri="http:
+00000820: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+00000830: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
+00000840: 6f72 6422 2077 3a76 616c 3d22 3122 2f3e  ord" w:val="1"/>
+00000850: 3c77 3a63 6f6d 7061 7453 6574 7469 6e67  <w:compatSetting
+00000860: 2077 3a6e 616d 653d 2264 6966 6665 7265   w:name="differe
+00000870: 6e74 6961 7465 4d75 6c74 6972 6f77 5461  ntiateMultirowTa
+00000880: 626c 6548 6561 6465 7273 2220 773a 7572  bleHeaders" w:ur
+00000890: 693d 2268 7474 703a 2f2f 7363 6865 6d61  i="http://schema
+000008a0: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+000008b0: 6f66 6669 6365 2f77 6f72 6422 2077 3a76  office/word" w:v
+000008c0: 616c 3d22 3122 2f3e 3c77 3a63 6f6d 7061  al="1"/><w:compa
+000008d0: 7453 6574 7469 6e67 2077 3a6e 616d 653d  tSetting w:name=
+000008e0: 2275 7365 576f 7264 3230 3133 5472 6163  "useWord2013Trac
+000008f0: 6b42 6f74 746f 6d48 7970 6865 6e61 7469  kBottomHyphenati
+00000900: 6f6e 2220 773a 7572 693d 2268 7474 703a  on" w:uri="http:
+00000910: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+00000920: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
+00000930: 6f72 6422 2077 3a76 616c 3d22 3022 2f3e  ord" w:val="0"/>
+00000940: 3c2f 773a 636f 6d70 6174 3e3c 773a 7273  </w:compat><w:rs
+00000950: 6964 733e 3c77 3a72 7369 6452 6f6f 7420  ids><w:rsidRoot 
+00000960: 773a 7661 6c3d 2230 3035 4634 4335 3222  w:val="005F4C52"
+00000970: 2f3e 3c77 3a72 7369 6420 773a 7661 6c3d  /><w:rsid w:val=
+00000980: 2230 3030 3531 4433 3422 2f3e 3c77 3a72  "00051D34"/><w:r
+00000990: 7369 6420 773a 7661 6c3d 2230 3030 4237  sid w:val="000B7
+000009a0: 4637 3322 2f3e 3c77 3a72 7369 6420 773a  F73"/><w:rsid w:
+000009b0: 7661 6c3d 2230 3031 3633 3337 3622 2f3e  val="00163376"/>
+000009c0: 3c77 3a72 7369 6420 773a 7661 6c3d 2230  <w:rsid w:val="0
+000009d0: 3031 4434 3842 4622 2f3e 3c77 3a72 7369  01D48BF"/><w:rsi
+000009e0: 6420 773a 7661 6c3d 2230 3033 3632 3645  d w:val="003626E
+000009f0: 3422 2f3e 3c77 3a72 7369 6420 773a 7661  4"/><w:rsid w:va
+00000a00: 6c3d 2230 3035 4634 4335 3222 2f3e 3c77  l="005F4C52"/><w
+00000a10: 3a72 7369 6420 773a 7661 6c3d 2230 3037  :rsid w:val="007
+00000a20: 3334 3146 3422 2f3e 3c77 3a72 7369 6420  341F4"/><w:rsid 
+00000a30: 773a 7661 6c3d 2230 3037 3635 4437 3522  w:val="00765D75"
+00000a40: 2f3e 3c77 3a72 7369 6420 773a 7661 6c3d  /><w:rsid w:val=
+00000a50: 2230 3037 4534 4334 3922 2f3e 3c77 3a72  "007E4C49"/><w:r
+00000a60: 7369 6420 773a 7661 6c3d 2230 3038 3432  sid w:val="00842
+00000a70: 3838 4422 2f3e 3c77 3a72 7369 6420 773a  88D"/><w:rsid w:
+00000a80: 7661 6c3d 2230 3039 3836 3233 3822 2f3e  val="00986238"/>
+00000a90: 3c77 3a72 7369 6420 773a 7661 6c3d 2230  <w:rsid w:val="0
+00000aa0: 3039 4430 3537 3322 2f3e 3c77 3a72 7369  09D0573"/><w:rsi
+00000ab0: 6420 773a 7661 6c3d 2230 3039 4536 3633  d w:val="009E663
+00000ac0: 4522 2f3e 3c77 3a72 7369 6420 773a 7661  E"/><w:rsid w:va
+00000ad0: 6c3d 2230 3044 3732 3535 4122 2f3e 3c2f  l="00D7255A"/></
+00000ae0: 773a 7273 6964 733e 3c6d 3a6d 6174 6850  w:rsids><m:mathP
+00000af0: 723e 3c6d 3a6d 6174 6846 6f6e 7420 6d3a  r><m:mathFont m:
+00000b00: 7661 6c3d 2243 616d 6272 6961 204d 6174  val="Cambria Mat
+00000b10: 6822 2f3e 3c6d 3a62 726b 4269 6e20 6d3a  h"/><m:brkBin m:
+00000b20: 7661 6c3d 2262 6566 6f72 6522 2f3e 3c6d  val="before"/><m
+00000b30: 3a62 726b 4269 6e53 7562 206d 3a76 616c  :brkBinSub m:val
+00000b40: 3d22 2d2d 222f 3e3c 6d3a 736d 616c 6c46  ="--"/><m:smallF
+00000b50: 7261 6320 6d3a 7661 6c3d 2230 222f 3e3c  rac m:val="0"/><
+00000b60: 6d3a 6469 7370 4465 662f 3e3c 6d3a 6c4d  m:dispDef/><m:lM
+00000b70: 6172 6769 6e20 6d3a 7661 6c3d 2230 222f  argin m:val="0"/
+00000b80: 3e3c 6d3a 724d 6172 6769 6e20 6d3a 7661  ><m:rMargin m:va
+00000b90: 6c3d 2230 222f 3e3c 6d3a 6465 664a 6320  l="0"/><m:defJc 
+00000ba0: 6d3a 7661 6c3d 2263 656e 7465 7247 726f  m:val="centerGro
+00000bb0: 7570 222f 3e3c 6d3a 7772 6170 496e 6465  up"/><m:wrapInde
+00000bc0: 6e74 206d 3a76 616c 3d22 3134 3430 222f  nt m:val="1440"/
+00000bd0: 3e3c 6d3a 696e 744c 696d 206d 3a76 616c  ><m:intLim m:val
+00000be0: 3d22 7375 6253 7570 222f 3e3c 6d3a 6e61  ="subSup"/><m:na
+00000bf0: 7279 4c69 6d20 6d3a 7661 6c3d 2275 6e64  ryLim m:val="und
+00000c00: 4f76 7222 2f3e 3c2f 6d3a 6d61 7468 5072  Ovr"/></m:mathPr
+00000c10: 3e3c 773a 7468 656d 6546 6f6e 744c 616e  ><w:themeFontLan
+00000c20: 6720 773a 7661 6c3d 2265 6e2d 4445 222f  g w:val="en-DE"/
+00000c30: 3e3c 773a 636c 7253 6368 656d 654d 6170  ><w:clrSchemeMap
+00000c40: 7069 6e67 2077 3a62 6731 3d22 6c69 6768  ping w:bg1="ligh
+00000c50: 7431 2220 773a 7431 3d22 6461 726b 3122  t1" w:t1="dark1"
+00000c60: 2077 3a62 6732 3d22 6c69 6768 7432 2220   w:bg2="light2" 
+00000c70: 773a 7432 3d22 6461 726b 3222 2077 3a61  w:t2="dark2" w:a
+00000c80: 6363 656e 7431 3d22 6163 6365 6e74 3122  ccent1="accent1"
+00000c90: 2077 3a61 6363 656e 7432 3d22 6163 6365   w:accent2="acce
+00000ca0: 6e74 3222 2077 3a61 6363 656e 7433 3d22  nt2" w:accent3="
+00000cb0: 6163 6365 6e74 3322 2077 3a61 6363 656e  accent3" w:accen
+00000cc0: 7434 3d22 6163 6365 6e74 3422 2077 3a61  t4="accent4" w:a
+00000cd0: 6363 656e 7435 3d22 6163 6365 6e74 3522  ccent5="accent5"
+00000ce0: 2077 3a61 6363 656e 7436 3d22 6163 6365   w:accent6="acce
+00000cf0: 6e74 3622 2077 3a68 7970 6572 6c69 6e6b  nt6" w:hyperlink
+00000d00: 3d22 6879 7065 726c 696e 6b22 2077 3a66  ="hyperlink" w:f
+00000d10: 6f6c 6c6f 7765 6448 7970 6572 6c69 6e6b  ollowedHyperlink
+00000d20: 3d22 666f 6c6c 6f77 6564 4879 7065 726c  ="followedHyperl
+00000d30: 696e 6b22 2f3e 3c77 3a73 6861 7065 4465  ink"/><w:shapeDe
+00000d40: 6661 756c 7473 3e3c 6f3a 7368 6170 6564  faults><o:shaped
+00000d50: 6566 6175 6c74 7320 763a 6578 743d 2265  efaults v:ext="e
+00000d60: 6469 7422 2073 7069 646d 6178 3d22 3130  dit" spidmax="10
+00000d70: 3236 222f 3e3c 6f3a 7368 6170 656c 6179  26"/><o:shapelay
+00000d80: 6f75 7420 763a 6578 743d 2265 6469 7422  out v:ext="edit"
+00000d90: 3e3c 6f3a 6964 6d61 7020 763a 6578 743d  ><o:idmap v:ext=
+00000da0: 2265 6469 7422 2064 6174 613d 2231 222f  "edit" data="1"/
+00000db0: 3e3c 2f6f 3a73 6861 7065 6c61 796f 7574  ></o:shapelayout
+00000dc0: 3e3c 2f77 3a73 6861 7065 4465 6661 756c  ></w:shapeDefaul
+00000dd0: 7473 3e3c 773a 6465 6369 6d61 6c53 796d  ts><w:decimalSym
+00000de0: 626f 6c20 773a 7661 6c3d 222c 222f 3e3c  bol w:val=","/><
+00000df0: 773a 6c69 7374 5365 7061 7261 746f 7220  w:listSeparator 
+00000e00: 773a 7661 6c3d 222c 222f 3e3c 7731 343a  w:val=","/><w14:
+00000e10: 646f 6349 6420 7731 343a 7661 6c3d 2233  docId w14:val="3
+00000e20: 3446 4336 3439 4522 2f3e 3c77 3135 3a63  4FC649E"/><w15:c
+00000e30: 6861 7274 5472 6163 6b69 6e67 5265 6642  hartTrackingRefB
+00000e40: 6173 6564 2f3e 3c2f 773a 7365 7474 696e  ased/></w:settin
+00000e50: 6773 3e                                  gs>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/styles.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/styles.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (44192), with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -1,2766 +1,2766 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 773a 7374 796c  "yes"?>..<w:styl
-00000040: 6573 2078 6d6c 6e73 3a6d 633d 2268 7474  es xmlns:mc="htt
-00000050: 703a 2f2f 7363 6865 6d61 732e 6f70 656e  p://schemas.open
-00000060: 786d 6c66 6f72 6d61 7473 2e6f 7267 2f6d  xmlformats.org/m
-00000070: 6172 6b75 702d 636f 6d70 6174 6962 696c  arkup-compatibil
-00000080: 6974 792f 3230 3036 2220 786d 6c6e 733a  ity/2006" xmlns:
-00000090: 723d 2268 7474 703a 2f2f 7363 6865 6d61  r="http://schema
-000000a0: 732e 6f70 656e 786d 6c66 6f72 6d61 7473  s.openxmlformats
-000000b0: 2e6f 7267 2f6f 6666 6963 6544 6f63 756d  .org/officeDocum
-000000c0: 656e 742f 3230 3036 2f72 656c 6174 696f  ent/2006/relatio
-000000d0: 6e73 6869 7073 2220 786d 6c6e 733a 773d  nships" xmlns:w=
-000000e0: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-000000f0: 6f70 656e 786d 6c66 6f72 6d61 7473 2e6f  openxmlformats.o
-00000100: 7267 2f77 6f72 6470 726f 6365 7373 696e  rg/wordprocessin
-00000110: 676d 6c2f 3230 3036 2f6d 6169 6e22 2078  gml/2006/main" x
-00000120: 6d6c 6e73 3a77 3134 3d22 6874 7470 3a2f  mlns:w14="http:/
-00000130: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
-00000140: 6674 2e63 6f6d 2f6f 6666 6963 652f 776f  ft.com/office/wo
-00000150: 7264 2f32 3031 302f 776f 7264 6d6c 2220  rd/2010/wordml" 
-00000160: 786d 6c6e 733a 7731 353d 2268 7474 703a  xmlns:w15="http:
-00000170: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
-00000180: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
-00000190: 6f72 642f 3230 3132 2f77 6f72 646d 6c22  ord/2012/wordml"
-000001a0: 2078 6d6c 6e73 3a77 3136 6365 783d 2268   xmlns:w16cex="h
-000001b0: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-000001c0: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-000001d0: 6365 2f77 6f72 642f 3230 3138 2f77 6f72  ce/word/2018/wor
-000001e0: 646d 6c2f 6365 7822 2078 6d6c 6e73 3a77  dml/cex" xmlns:w
-000001f0: 3136 6369 643d 2268 7474 703a 2f2f 7363  16cid="http://sc
-00000200: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
-00000210: 636f 6d2f 6f66 6669 6365 2f77 6f72 642f  com/office/word/
-00000220: 3230 3136 2f77 6f72 646d 6c2f 6369 6422  2016/wordml/cid"
-00000230: 2078 6d6c 6e73 3a77 3136 3d22 6874 7470   xmlns:w16="http
-00000240: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-00000250: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-00000260: 776f 7264 2f32 3031 382f 776f 7264 6d6c  word/2018/wordml
-00000270: 2220 786d 6c6e 733a 7731 3673 6474 6468  " xmlns:w16sdtdh
-00000280: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000290: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6f  .microsoft.com/o
-000002a0: 6666 6963 652f 776f 7264 2f32 3032 302f  ffice/word/2020/
-000002b0: 776f 7264 6d6c 2f73 6474 6461 7461 6861  wordml/sdtdataha
-000002c0: 7368 2220 786d 6c6e 733a 7731 3673 653d  sh" xmlns:w16se=
-000002d0: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-000002e0: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
-000002f0: 6669 6365 2f77 6f72 642f 3230 3135 2f77  fice/word/2015/w
-00000300: 6f72 646d 6c2f 7379 6d65 7822 206d 633a  ordml/symex" mc:
-00000310: 4967 6e6f 7261 626c 653d 2277 3134 2077  Ignorable="w14 w
-00000320: 3135 2077 3136 7365 2077 3136 6369 6420  15 w16se w16cid 
-00000330: 7731 3620 7731 3663 6578 2077 3136 7364  w16 w16cex w16sd
-00000340: 7464 6822 3e3c 773a 646f 6344 6566 6175  tdh"><w:docDefau
-00000350: 6c74 733e 3c77 3a72 5072 4465 6661 756c  lts><w:rPrDefaul
-00000360: 743e 3c77 3a72 5072 3e3c 773a 7246 6f6e  t><w:rPr><w:rFon
-00000370: 7473 2077 3a61 7363 6969 5468 656d 653d  ts w:asciiTheme=
-00000380: 226d 696e 6f72 4841 6e73 6922 2077 3a65  "minorHAnsi" w:e
-00000390: 6173 7441 7369 6154 6865 6d65 3d22 6d69  astAsiaTheme="mi
-000003a0: 6e6f 7248 416e 7369 2220 773a 6841 6e73  norHAnsi" w:hAns
-000003b0: 6954 6865 6d65 3d22 6d69 6e6f 7248 416e  iTheme="minorHAn
-000003c0: 7369 2220 773a 6373 7468 656d 653d 226d  si" w:cstheme="m
-000003d0: 696e 6f72 4269 6469 222f 3e3c 773a 737a  inorBidi"/><w:sz
-000003e0: 2077 3a76 616c 3d22 3232 222f 3e3c 773a   w:val="22"/><w:
-000003f0: 737a 4373 2077 3a76 616c 3d22 3232 222f  szCs w:val="22"/
-00000400: 3e3c 773a 6c61 6e67 2077 3a76 616c 3d22  ><w:lang w:val="
-00000410: 656e 2d44 4522 2077 3a65 6173 7441 7369  en-DE" w:eastAsi
-00000420: 613d 2265 6e2d 5553 2220 773a 6269 6469  a="en-US" w:bidi
-00000430: 3d22 6172 2d53 4122 2f3e 3c2f 773a 7250  ="ar-SA"/></w:rP
-00000440: 723e 3c2f 773a 7250 7244 6566 6175 6c74  r></w:rPrDefault
-00000450: 3e3c 773a 7050 7244 6566 6175 6c74 3e3c  ><w:pPrDefault><
-00000460: 773a 7050 723e 3c77 3a73 7061 6369 6e67  w:pPr><w:spacing
-00000470: 2077 3a61 6674 6572 3d22 3136 3022 2077   w:after="160" w
-00000480: 3a6c 696e 653d 2232 3539 2220 773a 6c69  :line="259" w:li
-00000490: 6e65 5275 6c65 3d22 6175 746f 222f 3e3c  neRule="auto"/><
-000004a0: 2f77 3a70 5072 3e3c 2f77 3a70 5072 4465  /w:pPr></w:pPrDe
-000004b0: 6661 756c 743e 3c2f 773a 646f 6344 6566  fault></w:docDef
-000004c0: 6175 6c74 733e 3c77 3a6c 6174 656e 7453  aults><w:latentS
-000004d0: 7479 6c65 7320 773a 6465 664c 6f63 6b65  tyles w:defLocke
-000004e0: 6453 7461 7465 3d22 3022 2077 3a64 6566  dState="0" w:def
-000004f0: 5549 5072 696f 7269 7479 3d22 3939 2220  UIPriority="99" 
-00000500: 773a 6465 6653 656d 6948 6964 6465 6e3d  w:defSemiHidden=
-00000510: 2230 2220 773a 6465 6655 6e68 6964 6557  "0" w:defUnhideW
-00000520: 6865 6e55 7365 643d 2230 2220 773a 6465  henUsed="0" w:de
-00000530: 6651 466f 726d 6174 3d22 3022 2077 3a63  fQFormat="0" w:c
-00000540: 6f75 6e74 3d22 3337 3622 3e3c 773a 6c73  ount="376"><w:ls
-00000550: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00000560: 653d 224e 6f72 6d61 6c22 2077 3a75 6950  e="Normal" w:uiP
-00000570: 7269 6f72 6974 793d 2230 2220 773a 7146  riority="0" w:qF
-00000580: 6f72 6d61 743d 2231 222f 3e3c 773a 6c73  ormat="1"/><w:ls
-00000590: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000005a0: 653d 2268 6561 6469 6e67 2031 2220 773a  e="heading 1" w:
-000005b0: 7569 5072 696f 7269 7479 3d22 3922 2077  uiPriority="9" w
-000005c0: 3a71 466f 726d 6174 3d22 3122 2f3e 3c77  :qFormat="1"/><w
-000005d0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000005e0: 6e61 6d65 3d22 6865 6164 696e 6720 3222  name="heading 2"
-000005f0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00000600: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00000610: 3922 2077 3a75 6e68 6964 6557 6865 6e55  9" w:unhideWhenU
-00000620: 7365 643d 2231 2220 773a 7146 6f72 6d61  sed="1" w:qForma
-00000630: 743d 2231 222f 3e3c 773a 6c73 6445 7863  t="1"/><w:lsdExc
-00000640: 6570 7469 6f6e 2077 3a6e 616d 653d 2268  eption w:name="h
-00000650: 6561 6469 6e67 2033 2220 773a 7365 6d69  eading 3" w:semi
-00000660: 4869 6464 656e 3d22 3122 2077 3a75 6950  Hidden="1" w:uiP
-00000670: 7269 6f72 6974 793d 2239 2220 773a 756e  riority="9" w:un
-00000680: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00000690: 2077 3a71 466f 726d 6174 3d22 3122 2f3e   w:qFormat="1"/>
-000006a0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-000006b0: 773a 6e61 6d65 3d22 6865 6164 696e 6720  w:name="heading 
-000006c0: 3422 2077 3a73 656d 6948 6964 6465 6e3d  4" w:semiHidden=
-000006d0: 2231 2220 773a 7569 5072 696f 7269 7479  "1" w:uiPriority
-000006e0: 3d22 3922 2077 3a75 6e68 6964 6557 6865  ="9" w:unhideWhe
-000006f0: 6e55 7365 643d 2231 2220 773a 7146 6f72  nUsed="1" w:qFor
-00000700: 6d61 743d 2231 222f 3e3c 773a 6c73 6445  mat="1"/><w:lsdE
-00000710: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00000720: 2268 6561 6469 6e67 2035 2220 773a 7365  "heading 5" w:se
-00000730: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-00000740: 6950 7269 6f72 6974 793d 2239 2220 773a  iPriority="9" w:
-00000750: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
-00000760: 3122 2077 3a71 466f 726d 6174 3d22 3122  1" w:qFormat="1"
-00000770: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00000780: 6e20 773a 6e61 6d65 3d22 6865 6164 696e  n w:name="headin
-00000790: 6720 3622 2077 3a73 656d 6948 6964 6465  g 6" w:semiHidde
-000007a0: 6e3d 2231 2220 773a 7569 5072 696f 7269  n="1" w:uiPriori
-000007b0: 7479 3d22 3922 2077 3a75 6e68 6964 6557  ty="9" w:unhideW
-000007c0: 6865 6e55 7365 643d 2231 2220 773a 7146  henUsed="1" w:qF
-000007d0: 6f72 6d61 743d 2231 222f 3e3c 773a 6c73  ormat="1"/><w:ls
-000007e0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000007f0: 653d 2268 6561 6469 6e67 2037 2220 773a  e="heading 7" w:
-00000800: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00000810: 3a75 6950 7269 6f72 6974 793d 2239 2220  :uiPriority="9" 
-00000820: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000830: 3d22 3122 2077 3a71 466f 726d 6174 3d22  ="1" w:qFormat="
-00000840: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-00000850: 696f 6e20 773a 6e61 6d65 3d22 6865 6164  ion w:name="head
-00000860: 696e 6720 3822 2077 3a73 656d 6948 6964  ing 8" w:semiHid
-00000870: 6465 6e3d 2231 2220 773a 7569 5072 696f  den="1" w:uiPrio
-00000880: 7269 7479 3d22 3922 2077 3a75 6e68 6964  rity="9" w:unhid
-00000890: 6557 6865 6e55 7365 643d 2231 2220 773a  eWhenUsed="1" w:
-000008a0: 7146 6f72 6d61 743d 2231 222f 3e3c 773a  qFormat="1"/><w:
-000008b0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000008c0: 616d 653d 2268 6561 6469 6e67 2039 2220  ame="heading 9" 
-000008d0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-000008e0: 2077 3a75 6950 7269 6f72 6974 793d 2239   w:uiPriority="9
-000008f0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00000900: 6564 3d22 3122 2077 3a71 466f 726d 6174  ed="1" w:qFormat
-00000910: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000920: 7074 696f 6e20 773a 6e61 6d65 3d22 696e  ption w:name="in
-00000930: 6465 7820 3122 2077 3a73 656d 6948 6964  dex 1" w:semiHid
-00000940: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00000950: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000960: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000970: 6e61 6d65 3d22 696e 6465 7820 3222 2077  name="index 2" w
-00000980: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-00000990: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-000009a0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-000009b0: 7074 696f 6e20 773a 6e61 6d65 3d22 696e  ption w:name="in
-000009c0: 6465 7820 3322 2077 3a73 656d 6948 6964  dex 3" w:semiHid
-000009d0: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-000009e0: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-000009f0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000a00: 6e61 6d65 3d22 696e 6465 7820 3422 2077  name="index 4" w
-00000a10: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-00000a20: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000a30: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000a40: 7074 696f 6e20 773a 6e61 6d65 3d22 696e  ption w:name="in
-00000a50: 6465 7820 3522 2077 3a73 656d 6948 6964  dex 5" w:semiHid
-00000a60: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00000a70: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000a80: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000a90: 6e61 6d65 3d22 696e 6465 7820 3622 2077  name="index 6" w
-00000aa0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-00000ab0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000ac0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000ad0: 7074 696f 6e20 773a 6e61 6d65 3d22 696e  ption w:name="in
-00000ae0: 6465 7820 3722 2077 3a73 656d 6948 6964  dex 7" w:semiHid
-00000af0: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00000b00: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000b10: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000b20: 6e61 6d65 3d22 696e 6465 7820 3822 2077  name="index 8" w
-00000b30: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-00000b40: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000b50: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000b60: 7074 696f 6e20 773a 6e61 6d65 3d22 696e  ption w:name="in
-00000b70: 6465 7820 3922 2077 3a73 656d 6948 6964  dex 9" w:semiHid
-00000b80: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00000b90: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000ba0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000bb0: 6e61 6d65 3d22 746f 6320 3122 2077 3a73  name="toc 1" w:s
-00000bc0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00000bd0: 7569 5072 696f 7269 7479 3d22 3339 2220  uiPriority="39" 
-00000be0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000bf0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000c00: 7074 696f 6e20 773a 6e61 6d65 3d22 746f  ption w:name="to
-00000c10: 6320 3222 2077 3a73 656d 6948 6964 6465  c 2" w:semiHidde
-00000c20: 6e3d 2231 2220 773a 7569 5072 696f 7269  n="1" w:uiPriori
-00000c30: 7479 3d22 3339 2220 773a 756e 6869 6465  ty="39" w:unhide
-00000c40: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000c50: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000c60: 6e61 6d65 3d22 746f 6320 3322 2077 3a73  name="toc 3" w:s
-00000c70: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00000c80: 7569 5072 696f 7269 7479 3d22 3339 2220  uiPriority="39" 
-00000c90: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000ca0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000cb0: 7074 696f 6e20 773a 6e61 6d65 3d22 746f  ption w:name="to
-00000cc0: 6320 3422 2077 3a73 656d 6948 6964 6465  c 4" w:semiHidde
-00000cd0: 6e3d 2231 2220 773a 7569 5072 696f 7269  n="1" w:uiPriori
-00000ce0: 7479 3d22 3339 2220 773a 756e 6869 6465  ty="39" w:unhide
-00000cf0: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000d00: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000d10: 6e61 6d65 3d22 746f 6320 3522 2077 3a73  name="toc 5" w:s
-00000d20: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00000d30: 7569 5072 696f 7269 7479 3d22 3339 2220  uiPriority="39" 
-00000d40: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000d50: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000d60: 7074 696f 6e20 773a 6e61 6d65 3d22 746f  ption w:name="to
-00000d70: 6320 3622 2077 3a73 656d 6948 6964 6465  c 6" w:semiHidde
-00000d80: 6e3d 2231 2220 773a 7569 5072 696f 7269  n="1" w:uiPriori
-00000d90: 7479 3d22 3339 2220 773a 756e 6869 6465  ty="39" w:unhide
-00000da0: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000db0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000dc0: 6e61 6d65 3d22 746f 6320 3722 2077 3a73  name="toc 7" w:s
-00000dd0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00000de0: 7569 5072 696f 7269 7479 3d22 3339 2220  uiPriority="39" 
-00000df0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000e00: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000e10: 7074 696f 6e20 773a 6e61 6d65 3d22 746f  ption w:name="to
-00000e20: 6320 3822 2077 3a73 656d 6948 6964 6465  c 8" w:semiHidde
-00000e30: 6e3d 2231 2220 773a 7569 5072 696f 7269  n="1" w:uiPriori
-00000e40: 7479 3d22 3339 2220 773a 756e 6869 6465  ty="39" w:unhide
-00000e50: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00000e60: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00000e70: 6e61 6d65 3d22 746f 6320 3922 2077 3a73  name="toc 9" w:s
-00000e80: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00000e90: 7569 5072 696f 7269 7479 3d22 3339 2220  uiPriority="39" 
-00000ea0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00000eb0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00000ec0: 7074 696f 6e20 773a 6e61 6d65 3d22 4e6f  ption w:name="No
-00000ed0: 726d 616c 2049 6e64 656e 7422 2077 3a73  rmal Indent" w:s
-00000ee0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00000ef0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
-00000f00: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-00000f10: 696f 6e20 773a 6e61 6d65 3d22 666f 6f74  ion w:name="foot
-00000f20: 6e6f 7465 2074 6578 7422 2077 3a73 656d  note text" w:sem
-00000f30: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
-00000f40: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00000f50: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00000f60: 6e20 773a 6e61 6d65 3d22 616e 6e6f 7461  n w:name="annota
-00000f70: 7469 6f6e 2074 6578 7422 2077 3a73 656d  tion text" w:sem
-00000f80: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
-00000f90: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00000fa0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00000fb0: 6e20 773a 6e61 6d65 3d22 6865 6164 6572  n w:name="header
-00000fc0: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00000fd0: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00000fe0: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00000ff0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00001000: 2266 6f6f 7465 7222 2077 3a73 656d 6948  "footer" w:semiH
-00001010: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
-00001020: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
-00001030: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00001040: 773a 6e61 6d65 3d22 696e 6465 7820 6865  w:name="index he
-00001050: 6164 696e 6722 2077 3a73 656d 6948 6964  ading" w:semiHid
-00001060: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00001070: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00001080: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00001090: 6e61 6d65 3d22 6361 7074 696f 6e22 2077  name="caption" w
-000010a0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-000010b0: 773a 7569 5072 696f 7269 7479 3d22 3335  w:uiPriority="35
-000010c0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-000010d0: 6564 3d22 3122 2077 3a71 466f 726d 6174  ed="1" w:qFormat
-000010e0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-000010f0: 7074 696f 6e20 773a 6e61 6d65 3d22 7461  ption w:name="ta
-00001100: 626c 6520 6f66 2066 6967 7572 6573 2220  ble of figures" 
-00001110: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00001120: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00001130: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00001140: 6570 7469 6f6e 2077 3a6e 616d 653d 2265  eption w:name="e
-00001150: 6e76 656c 6f70 6520 6164 6472 6573 7322  nvelope address"
-00001160: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00001170: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00001180: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00001190: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-000011a0: 656e 7665 6c6f 7065 2072 6574 7572 6e22  envelope return"
-000011b0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-000011c0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-000011d0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-000011e0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-000011f0: 666f 6f74 6e6f 7465 2072 6566 6572 656e  footnote referen
-00001200: 6365 2220 773a 7365 6d69 4869 6464 656e  ce" w:semiHidden
-00001210: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
-00001220: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
-00001230: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00001240: 653d 2261 6e6e 6f74 6174 696f 6e20 7265  e="annotation re
-00001250: 6665 7265 6e63 6522 2077 3a73 656d 6948  ference" w:semiH
-00001260: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
-00001270: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
-00001280: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00001290: 773a 6e61 6d65 3d22 6c69 6e65 206e 756d  w:name="line num
-000012a0: 6265 7222 2077 3a73 656d 6948 6964 6465  ber" w:semiHidde
-000012b0: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
-000012c0: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
-000012d0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-000012e0: 6d65 3d22 7061 6765 206e 756d 6265 7222  me="page number"
-000012f0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00001300: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00001310: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00001320: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00001330: 656e 646e 6f74 6520 7265 6665 7265 6e63  endnote referenc
-00001340: 6522 2077 3a73 656d 6948 6964 6465 6e3d  e" w:semiHidden=
-00001350: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00001360: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00001370: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00001380: 3d22 656e 646e 6f74 6520 7465 7874 2220  ="endnote text" 
-00001390: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-000013a0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-000013b0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-000013c0: 6570 7469 6f6e 2077 3a6e 616d 653d 2274  eption w:name="t
-000013d0: 6162 6c65 206f 6620 6175 7468 6f72 6974  able of authorit
-000013e0: 6965 7322 2077 3a73 656d 6948 6964 6465  ies" w:semiHidde
-000013f0: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
-00001400: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
-00001410: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00001420: 6d65 3d22 6d61 6372 6f22 2077 3a73 656d  me="macro" w:sem
-00001430: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
-00001440: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00001450: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00001460: 6e20 773a 6e61 6d65 3d22 746f 6120 6865  n w:name="toa he
-00001470: 6164 696e 6722 2077 3a73 656d 6948 6964  ading" w:semiHid
-00001480: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00001490: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-000014a0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000014b0: 6e61 6d65 3d22 4c69 7374 2220 773a 7365  name="List" w:se
-000014c0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-000014d0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
-000014e0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-000014f0: 6f6e 2077 3a6e 616d 653d 224c 6973 7420  on w:name="List 
-00001500: 4275 6c6c 6574 2220 773a 7365 6d69 4869  Bullet" w:semiHi
-00001510: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
-00001520: 6557 6865 6e55 7365 643d 2231 2220 773a  eWhenUsed="1" w:
-00001530: 7146 6f72 6d61 743d 2231 222f 3e3c 773a  qFormat="1"/><w:
-00001540: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00001550: 616d 653d 224c 6973 7420 4e75 6d62 6572  ame="List Number
-00001560: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00001570: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00001580: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00001590: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000015a0: 224c 6973 7420 3222 2077 3a73 656d 6948  "List 2" w:semiH
-000015b0: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
-000015c0: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
-000015d0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-000015e0: 773a 6e61 6d65 3d22 4c69 7374 2033 2220  w:name="List 3" 
-000015f0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00001600: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00001610: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00001620: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-00001630: 6973 7420 3422 2077 3a73 656d 6948 6964  ist 4" w:semiHid
-00001640: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00001650: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00001660: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00001670: 6e61 6d65 3d22 4c69 7374 2035 2220 773a  name="List 5" w:
-00001680: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00001690: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-000016a0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-000016b0: 7469 6f6e 2077 3a6e 616d 653d 224c 6973  tion w:name="Lis
-000016c0: 7420 4275 6c6c 6574 2032 2220 773a 7365  t Bullet 2" w:se
-000016d0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-000016e0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
-000016f0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00001700: 6f6e 2077 3a6e 616d 653d 224c 6973 7420  on w:name="List 
-00001710: 4275 6c6c 6574 2033 2220 773a 7365 6d69  Bullet 3" w:semi
-00001720: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
-00001730: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
-00001740: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00001750: 2077 3a6e 616d 653d 224c 6973 7420 4275   w:name="List Bu
-00001760: 6c6c 6574 2034 2220 773a 7365 6d69 4869  llet 4" w:semiHi
-00001770: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
-00001780: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
-00001790: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-000017a0: 3a6e 616d 653d 224c 6973 7420 4275 6c6c  :name="List Bull
-000017b0: 6574 2035 2220 773a 7365 6d69 4869 6464  et 5" w:semiHidd
-000017c0: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
-000017d0: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
-000017e0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000017f0: 616d 653d 224c 6973 7420 4e75 6d62 6572  ame="List Number
-00001800: 2032 2220 773a 7365 6d69 4869 6464 656e   2" w:semiHidden
-00001810: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
-00001820: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
-00001830: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00001840: 653d 224c 6973 7420 4e75 6d62 6572 2033  e="List Number 3
-00001850: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00001860: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00001870: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00001880: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00001890: 224c 6973 7420 4e75 6d62 6572 2034 2220  "List Number 4" 
-000018a0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-000018b0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-000018c0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-000018d0: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-000018e0: 6973 7420 4e75 6d62 6572 2035 2220 773a  ist Number 5" w:
-000018f0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00001900: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00001910: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00001920: 7469 6f6e 2077 3a6e 616d 653d 2254 6974  tion w:name="Tit
-00001930: 6c65 2220 773a 7569 5072 696f 7269 7479  le" w:uiPriority
-00001940: 3d22 3130 2220 773a 7146 6f72 6d61 743d  ="10" w:qFormat=
-00001950: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00001960: 7469 6f6e 2077 3a6e 616d 653d 2243 6c6f  tion w:name="Clo
-00001970: 7369 6e67 2220 773a 7365 6d69 4869 6464  sing" w:semiHidd
-00001980: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
-00001990: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
-000019a0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000019b0: 616d 653d 2253 6967 6e61 7475 7265 2220  ame="Signature" 
-000019c0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-000019d0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-000019e0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-000019f0: 6570 7469 6f6e 2077 3a6e 616d 653d 2244  eption w:name="D
-00001a00: 6566 6175 6c74 2050 6172 6167 7261 7068  efault Paragraph
-00001a10: 2046 6f6e 7422 2077 3a73 656d 6948 6964   Font" w:semiHid
-00001a20: 6465 6e3d 2231 2220 773a 7569 5072 696f  den="1" w:uiPrio
-00001a30: 7269 7479 3d22 3122 2077 3a75 6e68 6964  rity="1" w:unhid
-00001a40: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
-00001a50: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00001a60: 3a6e 616d 653d 2242 6f64 7920 5465 7874  :name="Body Text
-00001a70: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00001a80: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00001a90: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00001aa0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00001ab0: 2242 6f64 7920 5465 7874 2049 6e64 656e  "Body Text Inden
-00001ac0: 7422 2077 3a73 656d 6948 6964 6465 6e3d  t" w:semiHidden=
-00001ad0: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00001ae0: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00001af0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00001b00: 3d22 4c69 7374 2043 6f6e 7469 6e75 6522  ="List Continue"
-00001b10: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00001b20: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00001b30: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00001b40: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00001b50: 4c69 7374 2043 6f6e 7469 6e75 6520 3222  List Continue 2"
-00001b60: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00001b70: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00001b80: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00001b90: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00001ba0: 4c69 7374 2043 6f6e 7469 6e75 6520 3322  List Continue 3"
-00001bb0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00001bc0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00001bd0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00001be0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00001bf0: 4c69 7374 2043 6f6e 7469 6e75 6520 3422  List Continue 4"
-00001c00: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00001c10: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00001c20: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00001c30: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00001c40: 4c69 7374 2043 6f6e 7469 6e75 6520 3522  List Continue 5"
-00001c50: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00001c60: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00001c70: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00001c80: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00001c90: 4d65 7373 6167 6520 4865 6164 6572 2220  Message Header" 
-00001ca0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00001cb0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00001cc0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00001cd0: 6570 7469 6f6e 2077 3a6e 616d 653d 2253  eption w:name="S
-00001ce0: 7562 7469 746c 6522 2077 3a75 6950 7269  ubtitle" w:uiPri
-00001cf0: 6f72 6974 793d 2231 3122 2077 3a71 466f  ority="11" w:qFo
-00001d00: 726d 6174 3d22 3122 2f3e 3c77 3a6c 7364  rmat="1"/><w:lsd
-00001d10: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00001d20: 3d22 5361 6c75 7461 7469 6f6e 2220 773a  ="Salutation" w:
-00001d30: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00001d40: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00001d50: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00001d60: 7469 6f6e 2077 3a6e 616d 653d 2244 6174  tion w:name="Dat
-00001d70: 6522 2077 3a73 656d 6948 6964 6465 6e3d  e" w:semiHidden=
-00001d80: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00001d90: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00001da0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00001db0: 3d22 426f 6479 2054 6578 7420 4669 7273  ="Body Text Firs
-00001dc0: 7420 496e 6465 6e74 2220 773a 7365 6d69  t Indent" w:semi
-00001dd0: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
-00001de0: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
-00001df0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00001e00: 2077 3a6e 616d 653d 2242 6f64 7920 5465   w:name="Body Te
-00001e10: 7874 2046 6972 7374 2049 6e64 656e 7420  xt First Indent 
-00001e20: 3222 2077 3a73 656d 6948 6964 6465 6e3d  2" w:semiHidden=
-00001e30: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00001e40: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00001e50: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00001e60: 3d22 4e6f 7465 2048 6561 6469 6e67 2220  ="Note Heading" 
-00001e70: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00001e80: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00001e90: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00001ea0: 6570 7469 6f6e 2077 3a6e 616d 653d 2242  eption w:name="B
-00001eb0: 6f64 7920 5465 7874 2032 2220 773a 7365  ody Text 2" w:se
-00001ec0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-00001ed0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
-00001ee0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00001ef0: 6f6e 2077 3a6e 616d 653d 2242 6f64 7920  on w:name="Body 
-00001f00: 5465 7874 2033 2220 773a 7365 6d69 4869  Text 3" w:semiHi
-00001f10: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
-00001f20: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
-00001f30: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00001f40: 3a6e 616d 653d 2242 6f64 7920 5465 7874  :name="Body Text
-00001f50: 2049 6e64 656e 7420 3222 2077 3a73 656d   Indent 2" w:sem
-00001f60: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
-00001f70: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00001f80: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00001f90: 6e20 773a 6e61 6d65 3d22 426f 6479 2054  n w:name="Body T
-00001fa0: 6578 7420 496e 6465 6e74 2033 2220 773a  ext Indent 3" w:
-00001fb0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00001fc0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00001fd0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00001fe0: 7469 6f6e 2077 3a6e 616d 653d 2242 6c6f  tion w:name="Blo
-00001ff0: 636b 2054 6578 7422 2077 3a73 656d 6948  ck Text" w:semiH
-00002000: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
-00002010: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
-00002020: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00002030: 773a 6e61 6d65 3d22 4879 7065 726c 696e  w:name="Hyperlin
-00002040: 6b22 2077 3a73 656d 6948 6964 6465 6e3d  k" w:semiHidden=
-00002050: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00002060: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00002070: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00002080: 3d22 466f 6c6c 6f77 6564 4879 7065 726c  ="FollowedHyperl
-00002090: 696e 6b22 2077 3a73 656d 6948 6964 6465  ink" w:semiHidde
-000020a0: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
-000020b0: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
-000020c0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-000020d0: 6d65 3d22 5374 726f 6e67 2220 773a 7569  me="Strong" w:ui
-000020e0: 5072 696f 7269 7479 3d22 3232 2220 773a  Priority="22" w:
-000020f0: 7146 6f72 6d61 743d 2231 222f 3e3c 773a  qFormat="1"/><w:
-00002100: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00002110: 616d 653d 2245 6d70 6861 7369 7322 2077  ame="Emphasis" w
-00002120: 3a75 6950 7269 6f72 6974 793d 2232 3022  :uiPriority="20"
-00002130: 2077 3a71 466f 726d 6174 3d22 3122 2f3e   w:qFormat="1"/>
-00002140: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00002150: 773a 6e61 6d65 3d22 446f 6375 6d65 6e74  w:name="Document
-00002160: 204d 6170 2220 773a 7365 6d69 4869 6464   Map" w:semiHidd
-00002170: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
-00002180: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
-00002190: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000021a0: 616d 653d 2250 6c61 696e 2054 6578 7422  ame="Plain Text"
-000021b0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-000021c0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-000021d0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-000021e0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-000021f0: 452d 6d61 696c 2053 6967 6e61 7475 7265  E-mail Signature
-00002200: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00002210: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00002220: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00002230: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00002240: 2248 544d 4c20 546f 7020 6f66 2046 6f72  "HTML Top of For
-00002250: 6d22 2077 3a73 656d 6948 6964 6465 6e3d  m" w:semiHidden=
-00002260: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00002270: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00002280: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00002290: 3d22 4854 4d4c 2042 6f74 746f 6d20 6f66  ="HTML Bottom of
-000022a0: 2046 6f72 6d22 2077 3a73 656d 6948 6964   Form" w:semiHid
-000022b0: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-000022c0: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-000022d0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000022e0: 6e61 6d65 3d22 4e6f 726d 616c 2028 5765  name="Normal (We
-000022f0: 6229 2220 773a 7365 6d69 4869 6464 656e  b)" w:semiHidden
-00002300: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
-00002310: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
-00002320: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00002330: 653d 2248 544d 4c20 4163 726f 6e79 6d22  e="HTML Acronym"
-00002340: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00002350: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00002360: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002370: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002380: 4854 4d4c 2041 6464 7265 7373 2220 773a  HTML Address" w:
-00002390: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-000023a0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-000023b0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-000023c0: 7469 6f6e 2077 3a6e 616d 653d 2248 544d  tion w:name="HTM
-000023d0: 4c20 4369 7465 2220 773a 7365 6d69 4869  L Cite" w:semiHi
-000023e0: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
-000023f0: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
-00002400: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00002410: 3a6e 616d 653d 2248 544d 4c20 436f 6465  :name="HTML Code
-00002420: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00002430: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00002440: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00002450: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00002460: 2248 544d 4c20 4465 6669 6e69 7469 6f6e  "HTML Definition
-00002470: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00002480: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00002490: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-000024a0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000024b0: 2248 544d 4c20 4b65 7962 6f61 7264 2220  "HTML Keyboard" 
-000024c0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-000024d0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-000024e0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-000024f0: 6570 7469 6f6e 2077 3a6e 616d 653d 2248  eption w:name="H
-00002500: 544d 4c20 5072 6566 6f72 6d61 7474 6564  TML Preformatted
-00002510: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00002520: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00002530: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00002540: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00002550: 2248 544d 4c20 5361 6d70 6c65 2220 773a  "HTML Sample" w:
-00002560: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00002570: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00002580: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00002590: 7469 6f6e 2077 3a6e 616d 653d 2248 544d  tion w:name="HTM
-000025a0: 4c20 5479 7065 7772 6974 6572 2220 773a  L Typewriter" w:
-000025b0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-000025c0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-000025d0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-000025e0: 7469 6f6e 2077 3a6e 616d 653d 2248 544d  tion w:name="HTM
-000025f0: 4c20 5661 7269 6162 6c65 2220 773a 7365  L Variable" w:se
-00002600: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-00002610: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
-00002620: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00002630: 6f6e 2077 3a6e 616d 653d 224e 6f72 6d61  on w:name="Norma
-00002640: 6c20 5461 626c 6522 2077 3a73 656d 6948  l Table" w:semiH
-00002650: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
-00002660: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
-00002670: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00002680: 773a 6e61 6d65 3d22 616e 6e6f 7461 7469  w:name="annotati
-00002690: 6f6e 2073 7562 6a65 6374 2220 773a 7365  on subject" w:se
-000026a0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-000026b0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
-000026c0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-000026d0: 6f6e 2077 3a6e 616d 653d 224e 6f20 4c69  on w:name="No Li
-000026e0: 7374 2220 773a 7365 6d69 4869 6464 656e  st" w:semiHidden
-000026f0: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
-00002700: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
-00002710: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00002720: 653d 224f 7574 6c69 6e65 204c 6973 7420  e="Outline List 
-00002730: 3122 2077 3a73 656d 6948 6964 6465 6e3d  1" w:semiHidden=
-00002740: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00002750: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00002760: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00002770: 3d22 4f75 746c 696e 6520 4c69 7374 2032  ="Outline List 2
-00002780: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00002790: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-000027a0: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-000027b0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000027c0: 224f 7574 6c69 6e65 204c 6973 7420 3322  "Outline List 3"
-000027d0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-000027e0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-000027f0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002800: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002810: 5461 626c 6520 5369 6d70 6c65 2031 2220  Table Simple 1" 
-00002820: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00002830: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00002840: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00002850: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
-00002860: 6162 6c65 2053 696d 706c 6520 3222 2077  able Simple 2" w
-00002870: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-00002880: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00002890: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-000028a0: 7074 696f 6e20 773a 6e61 6d65 3d22 5461  ption w:name="Ta
-000028b0: 626c 6520 5369 6d70 6c65 2033 2220 773a  ble Simple 3" w:
-000028c0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-000028d0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-000028e0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-000028f0: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
-00002900: 6c65 2043 6c61 7373 6963 2031 2220 773a  le Classic 1" w:
-00002910: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00002920: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00002930: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00002940: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
-00002950: 6c65 2043 6c61 7373 6963 2032 2220 773a  le Classic 2" w:
-00002960: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00002970: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00002980: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00002990: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
-000029a0: 6c65 2043 6c61 7373 6963 2033 2220 773a  le Classic 3" w:
-000029b0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-000029c0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-000029d0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-000029e0: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
-000029f0: 6c65 2043 6c61 7373 6963 2034 2220 773a  le Classic 4" w:
-00002a00: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00002a10: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00002a20: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00002a30: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
-00002a40: 6c65 2043 6f6c 6f72 6675 6c20 3122 2077  le Colorful 1" w
-00002a50: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-00002a60: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00002a70: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00002a80: 7074 696f 6e20 773a 6e61 6d65 3d22 5461  ption w:name="Ta
-00002a90: 626c 6520 436f 6c6f 7266 756c 2032 2220  ble Colorful 2" 
-00002aa0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00002ab0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00002ac0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00002ad0: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
-00002ae0: 6162 6c65 2043 6f6c 6f72 6675 6c20 3322  able Colorful 3"
-00002af0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00002b00: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00002b10: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002b20: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002b30: 5461 626c 6520 436f 6c75 6d6e 7320 3122  Table Columns 1"
-00002b40: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00002b50: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00002b60: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002b70: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002b80: 5461 626c 6520 436f 6c75 6d6e 7320 3222  Table Columns 2"
-00002b90: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00002ba0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00002bb0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002bc0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002bd0: 5461 626c 6520 436f 6c75 6d6e 7320 3322  Table Columns 3"
-00002be0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00002bf0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00002c00: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002c10: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002c20: 5461 626c 6520 436f 6c75 6d6e 7320 3422  Table Columns 4"
-00002c30: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00002c40: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00002c50: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002c60: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002c70: 5461 626c 6520 436f 6c75 6d6e 7320 3522  Table Columns 5"
-00002c80: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00002c90: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00002ca0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00002cb0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00002cc0: 5461 626c 6520 4772 6964 2031 2220 773a  Table Grid 1" w:
-00002cd0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00002ce0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00002cf0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00002d00: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
-00002d10: 6c65 2047 7269 6420 3222 2077 3a73 656d  le Grid 2" w:sem
-00002d20: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
-00002d30: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00002d40: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00002d50: 6e20 773a 6e61 6d65 3d22 5461 626c 6520  n w:name="Table 
-00002d60: 4772 6964 2033 2220 773a 7365 6d69 4869  Grid 3" w:semiHi
-00002d70: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
-00002d80: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
-00002d90: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00002da0: 3a6e 616d 653d 2254 6162 6c65 2047 7269  :name="Table Gri
-00002db0: 6420 3422 2077 3a73 656d 6948 6964 6465  d 4" w:semiHidde
-00002dc0: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
-00002dd0: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
-00002de0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00002df0: 6d65 3d22 5461 626c 6520 4772 6964 2035  me="Table Grid 5
-00002e00: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00002e10: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
-00002e20: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
-00002e30: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00002e40: 2254 6162 6c65 2047 7269 6420 3622 2077  "Table Grid 6" w
-00002e50: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
-00002e60: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
-00002e70: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
-00002e80: 7074 696f 6e20 773a 6e61 6d65 3d22 5461  ption w:name="Ta
-00002e90: 626c 6520 4772 6964 2037 2220 773a 7365  ble Grid 7" w:se
-00002ea0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-00002eb0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
-00002ec0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00002ed0: 6f6e 2077 3a6e 616d 653d 2254 6162 6c65  on w:name="Table
-00002ee0: 2047 7269 6420 3822 2077 3a73 656d 6948   Grid 8" w:semiH
-00002ef0: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
-00002f00: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
-00002f10: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00002f20: 773a 6e61 6d65 3d22 5461 626c 6520 4c69  w:name="Table Li
-00002f30: 7374 2031 2220 773a 7365 6d69 4869 6464  st 1" w:semiHidd
-00002f40: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
-00002f50: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
-00002f60: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00002f70: 616d 653d 2254 6162 6c65 204c 6973 7420  ame="Table List 
-00002f80: 3222 2077 3a73 656d 6948 6964 6465 6e3d  2" w:semiHidden=
-00002f90: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
-00002fa0: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
-00002fb0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00002fc0: 3d22 5461 626c 6520 4c69 7374 2033 2220  ="Table List 3" 
-00002fd0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00002fe0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00002ff0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00003000: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
-00003010: 6162 6c65 204c 6973 7420 3422 2077 3a73  able List 4" w:s
-00003020: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00003030: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
-00003040: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-00003050: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
-00003060: 6520 4c69 7374 2035 2220 773a 7365 6d69  e List 5" w:semi
-00003070: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
-00003080: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
-00003090: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-000030a0: 2077 3a6e 616d 653d 2254 6162 6c65 204c   w:name="Table L
-000030b0: 6973 7420 3622 2077 3a73 656d 6948 6964  ist 6" w:semiHid
-000030c0: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-000030d0: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-000030e0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000030f0: 6e61 6d65 3d22 5461 626c 6520 4c69 7374  name="Table List
-00003100: 2037 2220 773a 7365 6d69 4869 6464 656e   7" w:semiHidden
-00003110: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
-00003120: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
-00003130: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00003140: 653d 2254 6162 6c65 204c 6973 7420 3822  e="Table List 8"
-00003150: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-00003160: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
-00003170: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
-00003180: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00003190: 5461 626c 6520 3344 2065 6666 6563 7473  Table 3D effects
-000031a0: 2031 2220 773a 7365 6d69 4869 6464 656e   1" w:semiHidden
-000031b0: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
-000031c0: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
-000031d0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000031e0: 653d 2254 6162 6c65 2033 4420 6566 6665  e="Table 3D effe
-000031f0: 6374 7320 3222 2077 3a73 656d 6948 6964  cts 2" w:semiHid
-00003200: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
-00003210: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
-00003220: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00003230: 6e61 6d65 3d22 5461 626c 6520 3344 2065  name="Table 3D e
-00003240: 6666 6563 7473 2033 2220 773a 7365 6d69  ffects 3" w:semi
-00003250: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
-00003260: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
-00003270: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00003280: 2077 3a6e 616d 653d 2254 6162 6c65 2043   w:name="Table C
-00003290: 6f6e 7465 6d70 6f72 6172 7922 2077 3a73  ontemporary" w:s
-000032a0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-000032b0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
-000032c0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-000032d0: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
-000032e0: 6520 456c 6567 616e 7422 2077 3a73 656d  e Elegant" w:sem
-000032f0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
-00003300: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00003310: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00003320: 6e20 773a 6e61 6d65 3d22 5461 626c 6520  n w:name="Table 
-00003330: 5072 6f66 6573 7369 6f6e 616c 2220 773a  Professional" w:
-00003340: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
-00003350: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
-00003360: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
-00003370: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
-00003380: 6c65 2053 7562 746c 6520 3122 2077 3a73  le Subtle 1" w:s
-00003390: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-000033a0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
-000033b0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-000033c0: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
-000033d0: 6520 5375 6274 6c65 2032 2220 773a 7365  e Subtle 2" w:se
-000033e0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
-000033f0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
-00003400: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00003410: 6f6e 2077 3a6e 616d 653d 2254 6162 6c65  on w:name="Table
-00003420: 2057 6562 2031 2220 773a 7365 6d69 4869   Web 1" w:semiHi
-00003430: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
-00003440: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
-00003450: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00003460: 3a6e 616d 653d 2254 6162 6c65 2057 6562  :name="Table Web
-00003470: 2032 2220 773a 7365 6d69 4869 6464 656e   2" w:semiHidden
-00003480: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
-00003490: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
-000034a0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000034b0: 653d 2254 6162 6c65 2057 6562 2033 2220  e="Table Web 3" 
-000034c0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-000034d0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-000034e0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-000034f0: 6570 7469 6f6e 2077 3a6e 616d 653d 2242  eption w:name="B
-00003500: 616c 6c6f 6f6e 2054 6578 7422 2077 3a73  alloon Text" w:s
-00003510: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00003520: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
-00003530: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-00003540: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
-00003550: 6520 4772 6964 2220 773a 7569 5072 696f  e Grid" w:uiPrio
-00003560: 7269 7479 3d22 3339 222f 3e3c 773a 6c73  rity="39"/><w:ls
-00003570: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00003580: 653d 2254 6162 6c65 2054 6865 6d65 2220  e="Table Theme" 
-00003590: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-000035a0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-000035b0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-000035c0: 6570 7469 6f6e 2077 3a6e 616d 653d 2250  eption w:name="P
-000035d0: 6c61 6365 686f 6c64 6572 2054 6578 7422  laceholder Text"
-000035e0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
-000035f0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00003600: 6f6e 2077 3a6e 616d 653d 224e 6f20 5370  on w:name="No Sp
-00003610: 6163 696e 6722 2077 3a75 6950 7269 6f72  acing" w:uiPrior
-00003620: 6974 793d 2231 2220 773a 7146 6f72 6d61  ity="1" w:qForma
-00003630: 743d 2231 222f 3e3c 773a 6c73 6445 7863  t="1"/><w:lsdExc
-00003640: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-00003650: 6967 6874 2053 6861 6469 6e67 2220 773a  ight Shading" w:
-00003660: 7569 5072 696f 7269 7479 3d22 3630 222f  uiPriority="60"/
-00003670: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00003680: 2077 3a6e 616d 653d 224c 6967 6874 204c   w:name="Light L
-00003690: 6973 7422 2077 3a75 6950 7269 6f72 6974  ist" w:uiPriorit
-000036a0: 793d 2236 3122 2f3e 3c77 3a6c 7364 4578  y="61"/><w:lsdEx
-000036b0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-000036c0: 4c69 6768 7420 4772 6964 2220 773a 7569  Light Grid" w:ui
-000036d0: 5072 696f 7269 7479 3d22 3632 222f 3e3c  Priority="62"/><
-000036e0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-000036f0: 3a6e 616d 653d 224d 6564 6975 6d20 5368  :name="Medium Sh
-00003700: 6164 696e 6720 3122 2077 3a75 6950 7269  ading 1" w:uiPri
-00003710: 6f72 6974 793d 2236 3322 2f3e 3c77 3a6c  ority="63"/><w:l
-00003720: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00003730: 6d65 3d22 4d65 6469 756d 2053 6861 6469  me="Medium Shadi
-00003740: 6e67 2032 2220 773a 7569 5072 696f 7269  ng 2" w:uiPriori
-00003750: 7479 3d22 3634 222f 3e3c 773a 6c73 6445  ty="64"/><w:lsdE
-00003760: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00003770: 224d 6564 6975 6d20 4c69 7374 2031 2220  "Medium List 1" 
-00003780: 773a 7569 5072 696f 7269 7479 3d22 3635  w:uiPriority="65
-00003790: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-000037a0: 6f6e 2077 3a6e 616d 653d 224d 6564 6975  on w:name="Mediu
-000037b0: 6d20 4c69 7374 2032 2220 773a 7569 5072  m List 2" w:uiPr
-000037c0: 696f 7269 7479 3d22 3636 222f 3e3c 773a  iority="66"/><w:
-000037d0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000037e0: 616d 653d 224d 6564 6975 6d20 4772 6964  ame="Medium Grid
-000037f0: 2031 2220 773a 7569 5072 696f 7269 7479   1" w:uiPriority
-00003800: 3d22 3637 222f 3e3c 773a 6c73 6445 7863  ="67"/><w:lsdExc
-00003810: 6570 7469 6f6e 2077 3a6e 616d 653d 224d  eption w:name="M
-00003820: 6564 6975 6d20 4772 6964 2032 2220 773a  edium Grid 2" w:
-00003830: 7569 5072 696f 7269 7479 3d22 3638 222f  uiPriority="68"/
-00003840: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00003850: 2077 3a6e 616d 653d 224d 6564 6975 6d20   w:name="Medium 
-00003860: 4772 6964 2033 2220 773a 7569 5072 696f  Grid 3" w:uiPrio
-00003870: 7269 7479 3d22 3639 222f 3e3c 773a 6c73  rity="69"/><w:ls
-00003880: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00003890: 653d 2244 6172 6b20 4c69 7374 2220 773a  e="Dark List" w:
-000038a0: 7569 5072 696f 7269 7479 3d22 3730 222f  uiPriority="70"/
-000038b0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-000038c0: 2077 3a6e 616d 653d 2243 6f6c 6f72 6675   w:name="Colorfu
-000038d0: 6c20 5368 6164 696e 6722 2077 3a75 6950  l Shading" w:uiP
-000038e0: 7269 6f72 6974 793d 2237 3122 2f3e 3c77  riority="71"/><w
-000038f0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00003900: 6e61 6d65 3d22 436f 6c6f 7266 756c 204c  name="Colorful L
-00003910: 6973 7422 2077 3a75 6950 7269 6f72 6974  ist" w:uiPriorit
-00003920: 793d 2237 3222 2f3e 3c77 3a6c 7364 4578  y="72"/><w:lsdEx
-00003930: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00003940: 436f 6c6f 7266 756c 2047 7269 6422 2077  Colorful Grid" w
-00003950: 3a75 6950 7269 6f72 6974 793d 2237 3322  :uiPriority="73"
-00003960: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00003970: 6e20 773a 6e61 6d65 3d22 4c69 6768 7420  n w:name="Light 
-00003980: 5368 6164 696e 6720 4163 6365 6e74 2031  Shading Accent 1
-00003990: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-000039a0: 3630 222f 3e3c 773a 6c73 6445 7863 6570  60"/><w:lsdExcep
-000039b0: 7469 6f6e 2077 3a6e 616d 653d 224c 6967  tion w:name="Lig
-000039c0: 6874 204c 6973 7420 4163 6365 6e74 2031  ht List Accent 1
-000039d0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-000039e0: 3631 222f 3e3c 773a 6c73 6445 7863 6570  61"/><w:lsdExcep
-000039f0: 7469 6f6e 2077 3a6e 616d 653d 224c 6967  tion w:name="Lig
-00003a00: 6874 2047 7269 6420 4163 6365 6e74 2031  ht Grid Accent 1
-00003a10: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00003a20: 3632 222f 3e3c 773a 6c73 6445 7863 6570  62"/><w:lsdExcep
-00003a30: 7469 6f6e 2077 3a6e 616d 653d 224d 6564  tion w:name="Med
-00003a40: 6975 6d20 5368 6164 696e 6720 3120 4163  ium Shading 1 Ac
-00003a50: 6365 6e74 2031 2220 773a 7569 5072 696f  cent 1" w:uiPrio
-00003a60: 7269 7479 3d22 3633 222f 3e3c 773a 6c73  rity="63"/><w:ls
-00003a70: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00003a80: 653d 224d 6564 6975 6d20 5368 6164 696e  e="Medium Shadin
-00003a90: 6720 3220 4163 6365 6e74 2031 2220 773a  g 2 Accent 1" w:
-00003aa0: 7569 5072 696f 7269 7479 3d22 3634 222f  uiPriority="64"/
-00003ab0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00003ac0: 2077 3a6e 616d 653d 224d 6564 6975 6d20   w:name="Medium 
-00003ad0: 4c69 7374 2031 2041 6363 656e 7420 3122  List 1 Accent 1"
-00003ae0: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
-00003af0: 3522 2f3e 3c77 3a6c 7364 4578 6365 7074  5"/><w:lsdExcept
-00003b00: 696f 6e20 773a 6e61 6d65 3d22 5265 7669  ion w:name="Revi
-00003b10: 7369 6f6e 2220 773a 7365 6d69 4869 6464  sion" w:semiHidd
-00003b20: 656e 3d22 3122 2f3e 3c77 3a6c 7364 4578  en="1"/><w:lsdEx
-00003b30: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00003b40: 4c69 7374 2050 6172 6167 7261 7068 2220  List Paragraph" 
-00003b50: 773a 7569 5072 696f 7269 7479 3d22 3334  w:uiPriority="34
-00003b60: 2220 773a 7146 6f72 6d61 743d 2231 222f  " w:qFormat="1"/
-00003b70: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00003b80: 2077 3a6e 616d 653d 2251 756f 7465 2220   w:name="Quote" 
-00003b90: 773a 7569 5072 696f 7269 7479 3d22 3239  w:uiPriority="29
-00003ba0: 2220 773a 7146 6f72 6d61 743d 2231 222f  " w:qFormat="1"/
-00003bb0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00003bc0: 2077 3a6e 616d 653d 2249 6e74 656e 7365   w:name="Intense
-00003bd0: 2051 756f 7465 2220 773a 7569 5072 696f   Quote" w:uiPrio
-00003be0: 7269 7479 3d22 3330 2220 773a 7146 6f72  rity="30" w:qFor
-00003bf0: 6d61 743d 2231 222f 3e3c 773a 6c73 6445  mat="1"/><w:lsdE
-00003c00: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00003c10: 224d 6564 6975 6d20 4c69 7374 2032 2041  "Medium List 2 A
-00003c20: 6363 656e 7420 3122 2077 3a75 6950 7269  ccent 1" w:uiPri
-00003c30: 6f72 6974 793d 2236 3622 2f3e 3c77 3a6c  ority="66"/><w:l
-00003c40: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00003c50: 6d65 3d22 4d65 6469 756d 2047 7269 6420  me="Medium Grid 
-00003c60: 3120 4163 6365 6e74 2031 2220 773a 7569  1 Accent 1" w:ui
-00003c70: 5072 696f 7269 7479 3d22 3637 222f 3e3c  Priority="67"/><
-00003c80: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00003c90: 3a6e 616d 653d 224d 6564 6975 6d20 4772  :name="Medium Gr
-00003ca0: 6964 2032 2041 6363 656e 7420 3122 2077  id 2 Accent 1" w
-00003cb0: 3a75 6950 7269 6f72 6974 793d 2236 3822  :uiPriority="68"
-00003cc0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00003cd0: 6e20 773a 6e61 6d65 3d22 4d65 6469 756d  n w:name="Medium
-00003ce0: 2047 7269 6420 3320 4163 6365 6e74 2031   Grid 3 Accent 1
-00003cf0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00003d00: 3639 222f 3e3c 773a 6c73 6445 7863 6570  69"/><w:lsdExcep
-00003d10: 7469 6f6e 2077 3a6e 616d 653d 2244 6172  tion w:name="Dar
-00003d20: 6b20 4c69 7374 2041 6363 656e 7420 3122  k List Accent 1"
-00003d30: 2077 3a75 6950 7269 6f72 6974 793d 2237   w:uiPriority="7
-00003d40: 3022 2f3e 3c77 3a6c 7364 4578 6365 7074  0"/><w:lsdExcept
-00003d50: 696f 6e20 773a 6e61 6d65 3d22 436f 6c6f  ion w:name="Colo
-00003d60: 7266 756c 2053 6861 6469 6e67 2041 6363  rful Shading Acc
-00003d70: 656e 7420 3122 2077 3a75 6950 7269 6f72  ent 1" w:uiPrior
-00003d80: 6974 793d 2237 3122 2f3e 3c77 3a6c 7364  ity="71"/><w:lsd
-00003d90: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00003da0: 3d22 436f 6c6f 7266 756c 204c 6973 7420  ="Colorful List 
-00003db0: 4163 6365 6e74 2031 2220 773a 7569 5072  Accent 1" w:uiPr
-00003dc0: 696f 7269 7479 3d22 3732 222f 3e3c 773a  iority="72"/><w:
-00003dd0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00003de0: 616d 653d 2243 6f6c 6f72 6675 6c20 4772  ame="Colorful Gr
-00003df0: 6964 2041 6363 656e 7420 3122 2077 3a75  id Accent 1" w:u
-00003e00: 6950 7269 6f72 6974 793d 2237 3322 2f3e  iPriority="73"/>
-00003e10: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00003e20: 773a 6e61 6d65 3d22 4c69 6768 7420 5368  w:name="Light Sh
-00003e30: 6164 696e 6720 4163 6365 6e74 2032 2220  ading Accent 2" 
-00003e40: 773a 7569 5072 696f 7269 7479 3d22 3630  w:uiPriority="60
-00003e50: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00003e60: 6f6e 2077 3a6e 616d 653d 224c 6967 6874  on w:name="Light
-00003e70: 204c 6973 7420 4163 6365 6e74 2032 2220   List Accent 2" 
-00003e80: 773a 7569 5072 696f 7269 7479 3d22 3631  w:uiPriority="61
-00003e90: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00003ea0: 6f6e 2077 3a6e 616d 653d 224c 6967 6874  on w:name="Light
-00003eb0: 2047 7269 6420 4163 6365 6e74 2032 2220   Grid Accent 2" 
-00003ec0: 773a 7569 5072 696f 7269 7479 3d22 3632  w:uiPriority="62
-00003ed0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00003ee0: 6f6e 2077 3a6e 616d 653d 224d 6564 6975  on w:name="Mediu
-00003ef0: 6d20 5368 6164 696e 6720 3120 4163 6365  m Shading 1 Acce
-00003f00: 6e74 2032 2220 773a 7569 5072 696f 7269  nt 2" w:uiPriori
-00003f10: 7479 3d22 3633 222f 3e3c 773a 6c73 6445  ty="63"/><w:lsdE
-00003f20: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00003f30: 224d 6564 6975 6d20 5368 6164 696e 6720  "Medium Shading 
-00003f40: 3220 4163 6365 6e74 2032 2220 773a 7569  2 Accent 2" w:ui
-00003f50: 5072 696f 7269 7479 3d22 3634 222f 3e3c  Priority="64"/><
-00003f60: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00003f70: 3a6e 616d 653d 224d 6564 6975 6d20 4c69  :name="Medium Li
-00003f80: 7374 2031 2041 6363 656e 7420 3222 2077  st 1 Accent 2" w
-00003f90: 3a75 6950 7269 6f72 6974 793d 2236 3522  :uiPriority="65"
-00003fa0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00003fb0: 6e20 773a 6e61 6d65 3d22 4d65 6469 756d  n w:name="Medium
-00003fc0: 204c 6973 7420 3220 4163 6365 6e74 2032   List 2 Accent 2
-00003fd0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00003fe0: 3636 222f 3e3c 773a 6c73 6445 7863 6570  66"/><w:lsdExcep
-00003ff0: 7469 6f6e 2077 3a6e 616d 653d 224d 6564  tion w:name="Med
-00004000: 6975 6d20 4772 6964 2031 2041 6363 656e  ium Grid 1 Accen
-00004010: 7420 3222 2077 3a75 6950 7269 6f72 6974  t 2" w:uiPriorit
-00004020: 793d 2236 3722 2f3e 3c77 3a6c 7364 4578  y="67"/><w:lsdEx
-00004030: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00004040: 4d65 6469 756d 2047 7269 6420 3220 4163  Medium Grid 2 Ac
-00004050: 6365 6e74 2032 2220 773a 7569 5072 696f  cent 2" w:uiPrio
-00004060: 7269 7479 3d22 3638 222f 3e3c 773a 6c73  rity="68"/><w:ls
-00004070: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00004080: 653d 224d 6564 6975 6d20 4772 6964 2033  e="Medium Grid 3
-00004090: 2041 6363 656e 7420 3222 2077 3a75 6950   Accent 2" w:uiP
-000040a0: 7269 6f72 6974 793d 2236 3922 2f3e 3c77  riority="69"/><w
-000040b0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000040c0: 6e61 6d65 3d22 4461 726b 204c 6973 7420  name="Dark List 
-000040d0: 4163 6365 6e74 2032 2220 773a 7569 5072  Accent 2" w:uiPr
-000040e0: 696f 7269 7479 3d22 3730 222f 3e3c 773a  iority="70"/><w:
-000040f0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00004100: 616d 653d 2243 6f6c 6f72 6675 6c20 5368  ame="Colorful Sh
-00004110: 6164 696e 6720 4163 6365 6e74 2032 2220  ading Accent 2" 
-00004120: 773a 7569 5072 696f 7269 7479 3d22 3731  w:uiPriority="71
-00004130: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00004140: 6f6e 2077 3a6e 616d 653d 2243 6f6c 6f72  on w:name="Color
-00004150: 6675 6c20 4c69 7374 2041 6363 656e 7420  ful List Accent 
-00004160: 3222 2077 3a75 6950 7269 6f72 6974 793d  2" w:uiPriority=
-00004170: 2237 3222 2f3e 3c77 3a6c 7364 4578 6365  "72"/><w:lsdExce
-00004180: 7074 696f 6e20 773a 6e61 6d65 3d22 436f  ption w:name="Co
-00004190: 6c6f 7266 756c 2047 7269 6420 4163 6365  lorful Grid Acce
-000041a0: 6e74 2032 2220 773a 7569 5072 696f 7269  nt 2" w:uiPriori
-000041b0: 7479 3d22 3733 222f 3e3c 773a 6c73 6445  ty="73"/><w:lsdE
-000041c0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000041d0: 224c 6967 6874 2053 6861 6469 6e67 2041  "Light Shading A
-000041e0: 6363 656e 7420 3322 2077 3a75 6950 7269  ccent 3" w:uiPri
-000041f0: 6f72 6974 793d 2236 3022 2f3e 3c77 3a6c  ority="60"/><w:l
-00004200: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00004210: 6d65 3d22 4c69 6768 7420 4c69 7374 2041  me="Light List A
-00004220: 6363 656e 7420 3322 2077 3a75 6950 7269  ccent 3" w:uiPri
-00004230: 6f72 6974 793d 2236 3122 2f3e 3c77 3a6c  ority="61"/><w:l
-00004240: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00004250: 6d65 3d22 4c69 6768 7420 4772 6964 2041  me="Light Grid A
-00004260: 6363 656e 7420 3322 2077 3a75 6950 7269  ccent 3" w:uiPri
-00004270: 6f72 6974 793d 2236 3222 2f3e 3c77 3a6c  ority="62"/><w:l
-00004280: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00004290: 6d65 3d22 4d65 6469 756d 2053 6861 6469  me="Medium Shadi
-000042a0: 6e67 2031 2041 6363 656e 7420 3322 2077  ng 1 Accent 3" w
-000042b0: 3a75 6950 7269 6f72 6974 793d 2236 3322  :uiPriority="63"
-000042c0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-000042d0: 6e20 773a 6e61 6d65 3d22 4d65 6469 756d  n w:name="Medium
-000042e0: 2053 6861 6469 6e67 2032 2041 6363 656e   Shading 2 Accen
-000042f0: 7420 3322 2077 3a75 6950 7269 6f72 6974  t 3" w:uiPriorit
-00004300: 793d 2236 3422 2f3e 3c77 3a6c 7364 4578  y="64"/><w:lsdEx
-00004310: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00004320: 4d65 6469 756d 204c 6973 7420 3120 4163  Medium List 1 Ac
-00004330: 6365 6e74 2033 2220 773a 7569 5072 696f  cent 3" w:uiPrio
-00004340: 7269 7479 3d22 3635 222f 3e3c 773a 6c73  rity="65"/><w:ls
-00004350: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00004360: 653d 224d 6564 6975 6d20 4c69 7374 2032  e="Medium List 2
-00004370: 2041 6363 656e 7420 3322 2077 3a75 6950   Accent 3" w:uiP
-00004380: 7269 6f72 6974 793d 2236 3622 2f3e 3c77  riority="66"/><w
-00004390: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000043a0: 6e61 6d65 3d22 4d65 6469 756d 2047 7269  name="Medium Gri
-000043b0: 6420 3120 4163 6365 6e74 2033 2220 773a  d 1 Accent 3" w:
-000043c0: 7569 5072 696f 7269 7479 3d22 3637 222f  uiPriority="67"/
-000043d0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-000043e0: 2077 3a6e 616d 653d 224d 6564 6975 6d20   w:name="Medium 
-000043f0: 4772 6964 2032 2041 6363 656e 7420 3322  Grid 2 Accent 3"
-00004400: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
-00004410: 3822 2f3e 3c77 3a6c 7364 4578 6365 7074  8"/><w:lsdExcept
-00004420: 696f 6e20 773a 6e61 6d65 3d22 4d65 6469  ion w:name="Medi
-00004430: 756d 2047 7269 6420 3320 4163 6365 6e74  um Grid 3 Accent
-00004440: 2033 2220 773a 7569 5072 696f 7269 7479   3" w:uiPriority
-00004450: 3d22 3639 222f 3e3c 773a 6c73 6445 7863  ="69"/><w:lsdExc
-00004460: 6570 7469 6f6e 2077 3a6e 616d 653d 2244  eption w:name="D
-00004470: 6172 6b20 4c69 7374 2041 6363 656e 7420  ark List Accent 
-00004480: 3322 2077 3a75 6950 7269 6f72 6974 793d  3" w:uiPriority=
-00004490: 2237 3022 2f3e 3c77 3a6c 7364 4578 6365  "70"/><w:lsdExce
-000044a0: 7074 696f 6e20 773a 6e61 6d65 3d22 436f  ption w:name="Co
-000044b0: 6c6f 7266 756c 2053 6861 6469 6e67 2041  lorful Shading A
-000044c0: 6363 656e 7420 3322 2077 3a75 6950 7269  ccent 3" w:uiPri
-000044d0: 6f72 6974 793d 2237 3122 2f3e 3c77 3a6c  ority="71"/><w:l
-000044e0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-000044f0: 6d65 3d22 436f 6c6f 7266 756c 204c 6973  me="Colorful Lis
-00004500: 7420 4163 6365 6e74 2033 2220 773a 7569  t Accent 3" w:ui
-00004510: 5072 696f 7269 7479 3d22 3732 222f 3e3c  Priority="72"/><
-00004520: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00004530: 3a6e 616d 653d 2243 6f6c 6f72 6675 6c20  :name="Colorful 
-00004540: 4772 6964 2041 6363 656e 7420 3322 2077  Grid Accent 3" w
-00004550: 3a75 6950 7269 6f72 6974 793d 2237 3322  :uiPriority="73"
-00004560: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00004570: 6e20 773a 6e61 6d65 3d22 4c69 6768 7420  n w:name="Light 
-00004580: 5368 6164 696e 6720 4163 6365 6e74 2034  Shading Accent 4
-00004590: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-000045a0: 3630 222f 3e3c 773a 6c73 6445 7863 6570  60"/><w:lsdExcep
-000045b0: 7469 6f6e 2077 3a6e 616d 653d 224c 6967  tion w:name="Lig
-000045c0: 6874 204c 6973 7420 4163 6365 6e74 2034  ht List Accent 4
-000045d0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-000045e0: 3631 222f 3e3c 773a 6c73 6445 7863 6570  61"/><w:lsdExcep
-000045f0: 7469 6f6e 2077 3a6e 616d 653d 224c 6967  tion w:name="Lig
-00004600: 6874 2047 7269 6420 4163 6365 6e74 2034  ht Grid Accent 4
-00004610: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00004620: 3632 222f 3e3c 773a 6c73 6445 7863 6570  62"/><w:lsdExcep
-00004630: 7469 6f6e 2077 3a6e 616d 653d 224d 6564  tion w:name="Med
-00004640: 6975 6d20 5368 6164 696e 6720 3120 4163  ium Shading 1 Ac
-00004650: 6365 6e74 2034 2220 773a 7569 5072 696f  cent 4" w:uiPrio
-00004660: 7269 7479 3d22 3633 222f 3e3c 773a 6c73  rity="63"/><w:ls
-00004670: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00004680: 653d 224d 6564 6975 6d20 5368 6164 696e  e="Medium Shadin
-00004690: 6720 3220 4163 6365 6e74 2034 2220 773a  g 2 Accent 4" w:
-000046a0: 7569 5072 696f 7269 7479 3d22 3634 222f  uiPriority="64"/
-000046b0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-000046c0: 2077 3a6e 616d 653d 224d 6564 6975 6d20   w:name="Medium 
-000046d0: 4c69 7374 2031 2041 6363 656e 7420 3422  List 1 Accent 4"
-000046e0: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
-000046f0: 3522 2f3e 3c77 3a6c 7364 4578 6365 7074  5"/><w:lsdExcept
-00004700: 696f 6e20 773a 6e61 6d65 3d22 4d65 6469  ion w:name="Medi
-00004710: 756d 204c 6973 7420 3220 4163 6365 6e74  um List 2 Accent
-00004720: 2034 2220 773a 7569 5072 696f 7269 7479   4" w:uiPriority
-00004730: 3d22 3636 222f 3e3c 773a 6c73 6445 7863  ="66"/><w:lsdExc
-00004740: 6570 7469 6f6e 2077 3a6e 616d 653d 224d  eption w:name="M
-00004750: 6564 6975 6d20 4772 6964 2031 2041 6363  edium Grid 1 Acc
-00004760: 656e 7420 3422 2077 3a75 6950 7269 6f72  ent 4" w:uiPrior
-00004770: 6974 793d 2236 3722 2f3e 3c77 3a6c 7364  ity="67"/><w:lsd
-00004780: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00004790: 3d22 4d65 6469 756d 2047 7269 6420 3220  ="Medium Grid 2 
-000047a0: 4163 6365 6e74 2034 2220 773a 7569 5072  Accent 4" w:uiPr
-000047b0: 696f 7269 7479 3d22 3638 222f 3e3c 773a  iority="68"/><w:
-000047c0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000047d0: 616d 653d 224d 6564 6975 6d20 4772 6964  ame="Medium Grid
-000047e0: 2033 2041 6363 656e 7420 3422 2077 3a75   3 Accent 4" w:u
-000047f0: 6950 7269 6f72 6974 793d 2236 3922 2f3e  iPriority="69"/>
-00004800: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00004810: 773a 6e61 6d65 3d22 4461 726b 204c 6973  w:name="Dark Lis
-00004820: 7420 4163 6365 6e74 2034 2220 773a 7569  t Accent 4" w:ui
-00004830: 5072 696f 7269 7479 3d22 3730 222f 3e3c  Priority="70"/><
-00004840: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00004850: 3a6e 616d 653d 2243 6f6c 6f72 6675 6c20  :name="Colorful 
-00004860: 5368 6164 696e 6720 4163 6365 6e74 2034  Shading Accent 4
-00004870: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00004880: 3731 222f 3e3c 773a 6c73 6445 7863 6570  71"/><w:lsdExcep
-00004890: 7469 6f6e 2077 3a6e 616d 653d 2243 6f6c  tion w:name="Col
-000048a0: 6f72 6675 6c20 4c69 7374 2041 6363 656e  orful List Accen
-000048b0: 7420 3422 2077 3a75 6950 7269 6f72 6974  t 4" w:uiPriorit
-000048c0: 793d 2237 3222 2f3e 3c77 3a6c 7364 4578  y="72"/><w:lsdEx
-000048d0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-000048e0: 436f 6c6f 7266 756c 2047 7269 6420 4163  Colorful Grid Ac
-000048f0: 6365 6e74 2034 2220 773a 7569 5072 696f  cent 4" w:uiPrio
-00004900: 7269 7479 3d22 3733 222f 3e3c 773a 6c73  rity="73"/><w:ls
-00004910: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00004920: 653d 224c 6967 6874 2053 6861 6469 6e67  e="Light Shading
-00004930: 2041 6363 656e 7420 3522 2077 3a75 6950   Accent 5" w:uiP
-00004940: 7269 6f72 6974 793d 2236 3022 2f3e 3c77  riority="60"/><w
-00004950: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00004960: 6e61 6d65 3d22 4c69 6768 7420 4c69 7374  name="Light List
-00004970: 2041 6363 656e 7420 3522 2077 3a75 6950   Accent 5" w:uiP
-00004980: 7269 6f72 6974 793d 2236 3122 2f3e 3c77  riority="61"/><w
-00004990: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000049a0: 6e61 6d65 3d22 4c69 6768 7420 4772 6964  name="Light Grid
-000049b0: 2041 6363 656e 7420 3522 2077 3a75 6950   Accent 5" w:uiP
-000049c0: 7269 6f72 6974 793d 2236 3222 2f3e 3c77  riority="62"/><w
-000049d0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000049e0: 6e61 6d65 3d22 4d65 6469 756d 2053 6861  name="Medium Sha
-000049f0: 6469 6e67 2031 2041 6363 656e 7420 3522  ding 1 Accent 5"
-00004a00: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
-00004a10: 3322 2f3e 3c77 3a6c 7364 4578 6365 7074  3"/><w:lsdExcept
-00004a20: 696f 6e20 773a 6e61 6d65 3d22 4d65 6469  ion w:name="Medi
-00004a30: 756d 2053 6861 6469 6e67 2032 2041 6363  um Shading 2 Acc
-00004a40: 656e 7420 3522 2077 3a75 6950 7269 6f72  ent 5" w:uiPrior
-00004a50: 6974 793d 2236 3422 2f3e 3c77 3a6c 7364  ity="64"/><w:lsd
-00004a60: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00004a70: 3d22 4d65 6469 756d 204c 6973 7420 3120  ="Medium List 1 
-00004a80: 4163 6365 6e74 2035 2220 773a 7569 5072  Accent 5" w:uiPr
-00004a90: 696f 7269 7479 3d22 3635 222f 3e3c 773a  iority="65"/><w:
-00004aa0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00004ab0: 616d 653d 224d 6564 6975 6d20 4c69 7374  ame="Medium List
-00004ac0: 2032 2041 6363 656e 7420 3522 2077 3a75   2 Accent 5" w:u
-00004ad0: 6950 7269 6f72 6974 793d 2236 3622 2f3e  iPriority="66"/>
-00004ae0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00004af0: 773a 6e61 6d65 3d22 4d65 6469 756d 2047  w:name="Medium G
-00004b00: 7269 6420 3120 4163 6365 6e74 2035 2220  rid 1 Accent 5" 
-00004b10: 773a 7569 5072 696f 7269 7479 3d22 3637  w:uiPriority="67
-00004b20: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00004b30: 6f6e 2077 3a6e 616d 653d 224d 6564 6975  on w:name="Mediu
-00004b40: 6d20 4772 6964 2032 2041 6363 656e 7420  m Grid 2 Accent 
-00004b50: 3522 2077 3a75 6950 7269 6f72 6974 793d  5" w:uiPriority=
-00004b60: 2236 3822 2f3e 3c77 3a6c 7364 4578 6365  "68"/><w:lsdExce
-00004b70: 7074 696f 6e20 773a 6e61 6d65 3d22 4d65  ption w:name="Me
-00004b80: 6469 756d 2047 7269 6420 3320 4163 6365  dium Grid 3 Acce
-00004b90: 6e74 2035 2220 773a 7569 5072 696f 7269  nt 5" w:uiPriori
-00004ba0: 7479 3d22 3639 222f 3e3c 773a 6c73 6445  ty="69"/><w:lsdE
-00004bb0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00004bc0: 2244 6172 6b20 4c69 7374 2041 6363 656e  "Dark List Accen
-00004bd0: 7420 3522 2077 3a75 6950 7269 6f72 6974  t 5" w:uiPriorit
-00004be0: 793d 2237 3022 2f3e 3c77 3a6c 7364 4578  y="70"/><w:lsdEx
-00004bf0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00004c00: 436f 6c6f 7266 756c 2053 6861 6469 6e67  Colorful Shading
-00004c10: 2041 6363 656e 7420 3522 2077 3a75 6950   Accent 5" w:uiP
-00004c20: 7269 6f72 6974 793d 2237 3122 2f3e 3c77  riority="71"/><w
-00004c30: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00004c40: 6e61 6d65 3d22 436f 6c6f 7266 756c 204c  name="Colorful L
-00004c50: 6973 7420 4163 6365 6e74 2035 2220 773a  ist Accent 5" w:
-00004c60: 7569 5072 696f 7269 7479 3d22 3732 222f  uiPriority="72"/
-00004c70: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00004c80: 2077 3a6e 616d 653d 2243 6f6c 6f72 6675   w:name="Colorfu
-00004c90: 6c20 4772 6964 2041 6363 656e 7420 3522  l Grid Accent 5"
-00004ca0: 2077 3a75 6950 7269 6f72 6974 793d 2237   w:uiPriority="7
-00004cb0: 3322 2f3e 3c77 3a6c 7364 4578 6365 7074  3"/><w:lsdExcept
-00004cc0: 696f 6e20 773a 6e61 6d65 3d22 4c69 6768  ion w:name="Ligh
-00004cd0: 7420 5368 6164 696e 6720 4163 6365 6e74  t Shading Accent
-00004ce0: 2036 2220 773a 7569 5072 696f 7269 7479   6" w:uiPriority
-00004cf0: 3d22 3630 222f 3e3c 773a 6c73 6445 7863  ="60"/><w:lsdExc
-00004d00: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-00004d10: 6967 6874 204c 6973 7420 4163 6365 6e74  ight List Accent
-00004d20: 2036 2220 773a 7569 5072 696f 7269 7479   6" w:uiPriority
-00004d30: 3d22 3631 222f 3e3c 773a 6c73 6445 7863  ="61"/><w:lsdExc
-00004d40: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-00004d50: 6967 6874 2047 7269 6420 4163 6365 6e74  ight Grid Accent
-00004d60: 2036 2220 773a 7569 5072 696f 7269 7479   6" w:uiPriority
-00004d70: 3d22 3632 222f 3e3c 773a 6c73 6445 7863  ="62"/><w:lsdExc
-00004d80: 6570 7469 6f6e 2077 3a6e 616d 653d 224d  eption w:name="M
-00004d90: 6564 6975 6d20 5368 6164 696e 6720 3120  edium Shading 1 
-00004da0: 4163 6365 6e74 2036 2220 773a 7569 5072  Accent 6" w:uiPr
-00004db0: 696f 7269 7479 3d22 3633 222f 3e3c 773a  iority="63"/><w:
-00004dc0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00004dd0: 616d 653d 224d 6564 6975 6d20 5368 6164  ame="Medium Shad
-00004de0: 696e 6720 3220 4163 6365 6e74 2036 2220  ing 2 Accent 6" 
-00004df0: 773a 7569 5072 696f 7269 7479 3d22 3634  w:uiPriority="64
-00004e00: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00004e10: 6f6e 2077 3a6e 616d 653d 224d 6564 6975  on w:name="Mediu
-00004e20: 6d20 4c69 7374 2031 2041 6363 656e 7420  m List 1 Accent 
-00004e30: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
-00004e40: 2236 3522 2f3e 3c77 3a6c 7364 4578 6365  "65"/><w:lsdExce
-00004e50: 7074 696f 6e20 773a 6e61 6d65 3d22 4d65  ption w:name="Me
-00004e60: 6469 756d 204c 6973 7420 3220 4163 6365  dium List 2 Acce
-00004e70: 6e74 2036 2220 773a 7569 5072 696f 7269  nt 6" w:uiPriori
-00004e80: 7479 3d22 3636 222f 3e3c 773a 6c73 6445  ty="66"/><w:lsdE
-00004e90: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00004ea0: 224d 6564 6975 6d20 4772 6964 2031 2041  "Medium Grid 1 A
-00004eb0: 6363 656e 7420 3622 2077 3a75 6950 7269  ccent 6" w:uiPri
-00004ec0: 6f72 6974 793d 2236 3722 2f3e 3c77 3a6c  ority="67"/><w:l
-00004ed0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00004ee0: 6d65 3d22 4d65 6469 756d 2047 7269 6420  me="Medium Grid 
-00004ef0: 3220 4163 6365 6e74 2036 2220 773a 7569  2 Accent 6" w:ui
-00004f00: 5072 696f 7269 7479 3d22 3638 222f 3e3c  Priority="68"/><
-00004f10: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00004f20: 3a6e 616d 653d 224d 6564 6975 6d20 4772  :name="Medium Gr
-00004f30: 6964 2033 2041 6363 656e 7420 3622 2077  id 3 Accent 6" w
-00004f40: 3a75 6950 7269 6f72 6974 793d 2236 3922  :uiPriority="69"
-00004f50: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00004f60: 6e20 773a 6e61 6d65 3d22 4461 726b 204c  n w:name="Dark L
-00004f70: 6973 7420 4163 6365 6e74 2036 2220 773a  ist Accent 6" w:
-00004f80: 7569 5072 696f 7269 7479 3d22 3730 222f  uiPriority="70"/
-00004f90: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00004fa0: 2077 3a6e 616d 653d 2243 6f6c 6f72 6675   w:name="Colorfu
-00004fb0: 6c20 5368 6164 696e 6720 4163 6365 6e74  l Shading Accent
-00004fc0: 2036 2220 773a 7569 5072 696f 7269 7479   6" w:uiPriority
-00004fd0: 3d22 3731 222f 3e3c 773a 6c73 6445 7863  ="71"/><w:lsdExc
-00004fe0: 6570 7469 6f6e 2077 3a6e 616d 653d 2243  eption w:name="C
-00004ff0: 6f6c 6f72 6675 6c20 4c69 7374 2041 6363  olorful List Acc
-00005000: 656e 7420 3622 2077 3a75 6950 7269 6f72  ent 6" w:uiPrior
-00005010: 6974 793d 2237 3222 2f3e 3c77 3a6c 7364  ity="72"/><w:lsd
-00005020: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00005030: 3d22 436f 6c6f 7266 756c 2047 7269 6420  ="Colorful Grid 
-00005040: 4163 6365 6e74 2036 2220 773a 7569 5072  Accent 6" w:uiPr
-00005050: 696f 7269 7479 3d22 3733 222f 3e3c 773a  iority="73"/><w:
-00005060: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00005070: 616d 653d 2253 7562 746c 6520 456d 7068  ame="Subtle Emph
-00005080: 6173 6973 2220 773a 7569 5072 696f 7269  asis" w:uiPriori
-00005090: 7479 3d22 3139 2220 773a 7146 6f72 6d61  ty="19" w:qForma
-000050a0: 743d 2231 222f 3e3c 773a 6c73 6445 7863  t="1"/><w:lsdExc
-000050b0: 6570 7469 6f6e 2077 3a6e 616d 653d 2249  eption w:name="I
-000050c0: 6e74 656e 7365 2045 6d70 6861 7369 7322  ntense Emphasis"
-000050d0: 2077 3a75 6950 7269 6f72 6974 793d 2232   w:uiPriority="2
-000050e0: 3122 2077 3a71 466f 726d 6174 3d22 3122  1" w:qFormat="1"
-000050f0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00005100: 6e20 773a 6e61 6d65 3d22 5375 6274 6c65  n w:name="Subtle
-00005110: 2052 6566 6572 656e 6365 2220 773a 7569   Reference" w:ui
-00005120: 5072 696f 7269 7479 3d22 3331 2220 773a  Priority="31" w:
-00005130: 7146 6f72 6d61 743d 2231 222f 3e3c 773a  qFormat="1"/><w:
-00005140: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00005150: 616d 653d 2249 6e74 656e 7365 2052 6566  ame="Intense Ref
-00005160: 6572 656e 6365 2220 773a 7569 5072 696f  erence" w:uiPrio
-00005170: 7269 7479 3d22 3332 2220 773a 7146 6f72  rity="32" w:qFor
-00005180: 6d61 743d 2231 222f 3e3c 773a 6c73 6445  mat="1"/><w:lsdE
-00005190: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000051a0: 2242 6f6f 6b20 5469 746c 6522 2077 3a75  "Book Title" w:u
-000051b0: 6950 7269 6f72 6974 793d 2233 3322 2077  iPriority="33" w
-000051c0: 3a71 466f 726d 6174 3d22 3122 2f3e 3c77  :qFormat="1"/><w
-000051d0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000051e0: 6e61 6d65 3d22 4269 626c 696f 6772 6170  name="Bibliograp
-000051f0: 6879 2220 773a 7365 6d69 4869 6464 656e  hy" w:semiHidden
-00005200: 3d22 3122 2077 3a75 6950 7269 6f72 6974  ="1" w:uiPriorit
-00005210: 793d 2233 3722 2077 3a75 6e68 6964 6557  y="37" w:unhideW
-00005220: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
-00005230: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00005240: 616d 653d 2254 4f43 2048 6561 6469 6e67  ame="TOC Heading
-00005250: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
-00005260: 3122 2077 3a75 6950 7269 6f72 6974 793d  1" w:uiPriority=
-00005270: 2233 3922 2077 3a75 6e68 6964 6557 6865  "39" w:unhideWhe
-00005280: 6e55 7365 643d 2231 2220 773a 7146 6f72  nUsed="1" w:qFor
-00005290: 6d61 743d 2231 222f 3e3c 773a 6c73 6445  mat="1"/><w:lsdE
-000052a0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000052b0: 2250 6c61 696e 2054 6162 6c65 2031 2220  "Plain Table 1" 
-000052c0: 773a 7569 5072 696f 7269 7479 3d22 3431  w:uiPriority="41
-000052d0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-000052e0: 6f6e 2077 3a6e 616d 653d 2250 6c61 696e  on w:name="Plain
-000052f0: 2054 6162 6c65 2032 2220 773a 7569 5072   Table 2" w:uiPr
-00005300: 696f 7269 7479 3d22 3432 222f 3e3c 773a  iority="42"/><w:
-00005310: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00005320: 616d 653d 2250 6c61 696e 2054 6162 6c65  ame="Plain Table
-00005330: 2033 2220 773a 7569 5072 696f 7269 7479   3" w:uiPriority
-00005340: 3d22 3433 222f 3e3c 773a 6c73 6445 7863  ="43"/><w:lsdExc
-00005350: 6570 7469 6f6e 2077 3a6e 616d 653d 2250  eption w:name="P
-00005360: 6c61 696e 2054 6162 6c65 2034 2220 773a  lain Table 4" w:
-00005370: 7569 5072 696f 7269 7479 3d22 3434 222f  uiPriority="44"/
-00005380: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00005390: 2077 3a6e 616d 653d 2250 6c61 696e 2054   w:name="Plain T
-000053a0: 6162 6c65 2035 2220 773a 7569 5072 696f  able 5" w:uiPrio
-000053b0: 7269 7479 3d22 3435 222f 3e3c 773a 6c73  rity="45"/><w:ls
-000053c0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000053d0: 653d 2247 7269 6420 5461 626c 6520 4c69  e="Grid Table Li
-000053e0: 6768 7422 2077 3a75 6950 7269 6f72 6974  ght" w:uiPriorit
-000053f0: 793d 2234 3022 2f3e 3c77 3a6c 7364 4578  y="40"/><w:lsdEx
-00005400: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00005410: 4772 6964 2054 6162 6c65 2031 204c 6967  Grid Table 1 Lig
-00005420: 6874 2220 773a 7569 5072 696f 7269 7479  ht" w:uiPriority
-00005430: 3d22 3436 222f 3e3c 773a 6c73 6445 7863  ="46"/><w:lsdExc
-00005440: 6570 7469 6f6e 2077 3a6e 616d 653d 2247  eption w:name="G
-00005450: 7269 6420 5461 626c 6520 3222 2077 3a75  rid Table 2" w:u
-00005460: 6950 7269 6f72 6974 793d 2234 3722 2f3e  iPriority="47"/>
-00005470: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00005480: 773a 6e61 6d65 3d22 4772 6964 2054 6162  w:name="Grid Tab
-00005490: 6c65 2033 2220 773a 7569 5072 696f 7269  le 3" w:uiPriori
-000054a0: 7479 3d22 3438 222f 3e3c 773a 6c73 6445  ty="48"/><w:lsdE
-000054b0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000054c0: 2247 7269 6420 5461 626c 6520 3422 2077  "Grid Table 4" w
-000054d0: 3a75 6950 7269 6f72 6974 793d 2234 3922  :uiPriority="49"
-000054e0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-000054f0: 6e20 773a 6e61 6d65 3d22 4772 6964 2054  n w:name="Grid T
-00005500: 6162 6c65 2035 2044 6172 6b22 2077 3a75  able 5 Dark" w:u
-00005510: 6950 7269 6f72 6974 793d 2235 3022 2f3e  iPriority="50"/>
-00005520: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00005530: 773a 6e61 6d65 3d22 4772 6964 2054 6162  w:name="Grid Tab
-00005540: 6c65 2036 2043 6f6c 6f72 6675 6c22 2077  le 6 Colorful" w
-00005550: 3a75 6950 7269 6f72 6974 793d 2235 3122  :uiPriority="51"
-00005560: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00005570: 6e20 773a 6e61 6d65 3d22 4772 6964 2054  n w:name="Grid T
-00005580: 6162 6c65 2037 2043 6f6c 6f72 6675 6c22  able 7 Colorful"
-00005590: 2077 3a75 6950 7269 6f72 6974 793d 2235   w:uiPriority="5
-000055a0: 3222 2f3e 3c77 3a6c 7364 4578 6365 7074  2"/><w:lsdExcept
-000055b0: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
-000055c0: 2054 6162 6c65 2031 204c 6967 6874 2041   Table 1 Light A
-000055d0: 6363 656e 7420 3122 2077 3a75 6950 7269  ccent 1" w:uiPri
-000055e0: 6f72 6974 793d 2234 3622 2f3e 3c77 3a6c  ority="46"/><w:l
-000055f0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00005600: 6d65 3d22 4772 6964 2054 6162 6c65 2032  me="Grid Table 2
-00005610: 2041 6363 656e 7420 3122 2077 3a75 6950   Accent 1" w:uiP
-00005620: 7269 6f72 6974 793d 2234 3722 2f3e 3c77  riority="47"/><w
-00005630: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00005640: 6e61 6d65 3d22 4772 6964 2054 6162 6c65  name="Grid Table
-00005650: 2033 2041 6363 656e 7420 3122 2077 3a75   3 Accent 1" w:u
-00005660: 6950 7269 6f72 6974 793d 2234 3822 2f3e  iPriority="48"/>
-00005670: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00005680: 773a 6e61 6d65 3d22 4772 6964 2054 6162  w:name="Grid Tab
-00005690: 6c65 2034 2041 6363 656e 7420 3122 2077  le 4 Accent 1" w
-000056a0: 3a75 6950 7269 6f72 6974 793d 2234 3922  :uiPriority="49"
-000056b0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-000056c0: 6e20 773a 6e61 6d65 3d22 4772 6964 2054  n w:name="Grid T
-000056d0: 6162 6c65 2035 2044 6172 6b20 4163 6365  able 5 Dark Acce
-000056e0: 6e74 2031 2220 773a 7569 5072 696f 7269  nt 1" w:uiPriori
-000056f0: 7479 3d22 3530 222f 3e3c 773a 6c73 6445  ty="50"/><w:lsdE
-00005700: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00005710: 2247 7269 6420 5461 626c 6520 3620 436f  "Grid Table 6 Co
-00005720: 6c6f 7266 756c 2041 6363 656e 7420 3122  lorful Accent 1"
-00005730: 2077 3a75 6950 7269 6f72 6974 793d 2235   w:uiPriority="5
-00005740: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-00005750: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
-00005760: 2054 6162 6c65 2037 2043 6f6c 6f72 6675   Table 7 Colorfu
-00005770: 6c20 4163 6365 6e74 2031 2220 773a 7569  l Accent 1" w:ui
-00005780: 5072 696f 7269 7479 3d22 3532 222f 3e3c  Priority="52"/><
-00005790: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-000057a0: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
-000057b0: 6520 3120 4c69 6768 7420 4163 6365 6e74  e 1 Light Accent
-000057c0: 2032 2220 773a 7569 5072 696f 7269 7479   2" w:uiPriority
-000057d0: 3d22 3436 222f 3e3c 773a 6c73 6445 7863  ="46"/><w:lsdExc
-000057e0: 6570 7469 6f6e 2077 3a6e 616d 653d 2247  eption w:name="G
-000057f0: 7269 6420 5461 626c 6520 3220 4163 6365  rid Table 2 Acce
-00005800: 6e74 2032 2220 773a 7569 5072 696f 7269  nt 2" w:uiPriori
-00005810: 7479 3d22 3437 222f 3e3c 773a 6c73 6445  ty="47"/><w:lsdE
-00005820: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00005830: 2247 7269 6420 5461 626c 6520 3320 4163  "Grid Table 3 Ac
-00005840: 6365 6e74 2032 2220 773a 7569 5072 696f  cent 2" w:uiPrio
-00005850: 7269 7479 3d22 3438 222f 3e3c 773a 6c73  rity="48"/><w:ls
-00005860: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00005870: 653d 2247 7269 6420 5461 626c 6520 3420  e="Grid Table 4 
-00005880: 4163 6365 6e74 2032 2220 773a 7569 5072  Accent 2" w:uiPr
-00005890: 696f 7269 7479 3d22 3439 222f 3e3c 773a  iority="49"/><w:
-000058a0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000058b0: 616d 653d 2247 7269 6420 5461 626c 6520  ame="Grid Table 
-000058c0: 3520 4461 726b 2041 6363 656e 7420 3222  5 Dark Accent 2"
-000058d0: 2077 3a75 6950 7269 6f72 6974 793d 2235   w:uiPriority="5
-000058e0: 3022 2f3e 3c77 3a6c 7364 4578 6365 7074  0"/><w:lsdExcept
-000058f0: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
-00005900: 2054 6162 6c65 2036 2043 6f6c 6f72 6675   Table 6 Colorfu
-00005910: 6c20 4163 6365 6e74 2032 2220 773a 7569  l Accent 2" w:ui
-00005920: 5072 696f 7269 7479 3d22 3531 222f 3e3c  Priority="51"/><
-00005930: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00005940: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
-00005950: 6520 3720 436f 6c6f 7266 756c 2041 6363  e 7 Colorful Acc
-00005960: 656e 7420 3222 2077 3a75 6950 7269 6f72  ent 2" w:uiPrior
-00005970: 6974 793d 2235 3222 2f3e 3c77 3a6c 7364  ity="52"/><w:lsd
-00005980: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00005990: 3d22 4772 6964 2054 6162 6c65 2031 204c  ="Grid Table 1 L
-000059a0: 6967 6874 2041 6363 656e 7420 3322 2077  ight Accent 3" w
-000059b0: 3a75 6950 7269 6f72 6974 793d 2234 3622  :uiPriority="46"
-000059c0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-000059d0: 6e20 773a 6e61 6d65 3d22 4772 6964 2054  n w:name="Grid T
-000059e0: 6162 6c65 2032 2041 6363 656e 7420 3322  able 2 Accent 3"
-000059f0: 2077 3a75 6950 7269 6f72 6974 793d 2234   w:uiPriority="4
-00005a00: 3722 2f3e 3c77 3a6c 7364 4578 6365 7074  7"/><w:lsdExcept
-00005a10: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
-00005a20: 2054 6162 6c65 2033 2041 6363 656e 7420   Table 3 Accent 
-00005a30: 3322 2077 3a75 6950 7269 6f72 6974 793d  3" w:uiPriority=
-00005a40: 2234 3822 2f3e 3c77 3a6c 7364 4578 6365  "48"/><w:lsdExce
-00005a50: 7074 696f 6e20 773a 6e61 6d65 3d22 4772  ption w:name="Gr
-00005a60: 6964 2054 6162 6c65 2034 2041 6363 656e  id Table 4 Accen
-00005a70: 7420 3322 2077 3a75 6950 7269 6f72 6974  t 3" w:uiPriorit
-00005a80: 793d 2234 3922 2f3e 3c77 3a6c 7364 4578  y="49"/><w:lsdEx
-00005a90: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00005aa0: 4772 6964 2054 6162 6c65 2035 2044 6172  Grid Table 5 Dar
-00005ab0: 6b20 4163 6365 6e74 2033 2220 773a 7569  k Accent 3" w:ui
-00005ac0: 5072 696f 7269 7479 3d22 3530 222f 3e3c  Priority="50"/><
-00005ad0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00005ae0: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
-00005af0: 6520 3620 436f 6c6f 7266 756c 2041 6363  e 6 Colorful Acc
-00005b00: 656e 7420 3322 2077 3a75 6950 7269 6f72  ent 3" w:uiPrior
-00005b10: 6974 793d 2235 3122 2f3e 3c77 3a6c 7364  ity="51"/><w:lsd
-00005b20: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00005b30: 3d22 4772 6964 2054 6162 6c65 2037 2043  ="Grid Table 7 C
-00005b40: 6f6c 6f72 6675 6c20 4163 6365 6e74 2033  olorful Accent 3
-00005b50: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00005b60: 3532 222f 3e3c 773a 6c73 6445 7863 6570  52"/><w:lsdExcep
-00005b70: 7469 6f6e 2077 3a6e 616d 653d 2247 7269  tion w:name="Gri
-00005b80: 6420 5461 626c 6520 3120 4c69 6768 7420  d Table 1 Light 
-00005b90: 4163 6365 6e74 2034 2220 773a 7569 5072  Accent 4" w:uiPr
-00005ba0: 696f 7269 7479 3d22 3436 222f 3e3c 773a  iority="46"/><w:
-00005bb0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00005bc0: 616d 653d 2247 7269 6420 5461 626c 6520  ame="Grid Table 
-00005bd0: 3220 4163 6365 6e74 2034 2220 773a 7569  2 Accent 4" w:ui
-00005be0: 5072 696f 7269 7479 3d22 3437 222f 3e3c  Priority="47"/><
-00005bf0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00005c00: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
-00005c10: 6520 3320 4163 6365 6e74 2034 2220 773a  e 3 Accent 4" w:
-00005c20: 7569 5072 696f 7269 7479 3d22 3438 222f  uiPriority="48"/
-00005c30: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00005c40: 2077 3a6e 616d 653d 2247 7269 6420 5461   w:name="Grid Ta
-00005c50: 626c 6520 3420 4163 6365 6e74 2034 2220  ble 4 Accent 4" 
-00005c60: 773a 7569 5072 696f 7269 7479 3d22 3439  w:uiPriority="49
-00005c70: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00005c80: 6f6e 2077 3a6e 616d 653d 2247 7269 6420  on w:name="Grid 
-00005c90: 5461 626c 6520 3520 4461 726b 2041 6363  Table 5 Dark Acc
-00005ca0: 656e 7420 3422 2077 3a75 6950 7269 6f72  ent 4" w:uiPrior
-00005cb0: 6974 793d 2235 3022 2f3e 3c77 3a6c 7364  ity="50"/><w:lsd
-00005cc0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00005cd0: 3d22 4772 6964 2054 6162 6c65 2036 2043  ="Grid Table 6 C
-00005ce0: 6f6c 6f72 6675 6c20 4163 6365 6e74 2034  olorful Accent 4
-00005cf0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00005d00: 3531 222f 3e3c 773a 6c73 6445 7863 6570  51"/><w:lsdExcep
-00005d10: 7469 6f6e 2077 3a6e 616d 653d 2247 7269  tion w:name="Gri
-00005d20: 6420 5461 626c 6520 3720 436f 6c6f 7266  d Table 7 Colorf
-00005d30: 756c 2041 6363 656e 7420 3422 2077 3a75  ul Accent 4" w:u
-00005d40: 6950 7269 6f72 6974 793d 2235 3222 2f3e  iPriority="52"/>
-00005d50: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00005d60: 773a 6e61 6d65 3d22 4772 6964 2054 6162  w:name="Grid Tab
-00005d70: 6c65 2031 204c 6967 6874 2041 6363 656e  le 1 Light Accen
-00005d80: 7420 3522 2077 3a75 6950 7269 6f72 6974  t 5" w:uiPriorit
-00005d90: 793d 2234 3622 2f3e 3c77 3a6c 7364 4578  y="46"/><w:lsdEx
-00005da0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00005db0: 4772 6964 2054 6162 6c65 2032 2041 6363  Grid Table 2 Acc
-00005dc0: 656e 7420 3522 2077 3a75 6950 7269 6f72  ent 5" w:uiPrior
-00005dd0: 6974 793d 2234 3722 2f3e 3c77 3a6c 7364  ity="47"/><w:lsd
-00005de0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00005df0: 3d22 4772 6964 2054 6162 6c65 2033 2041  ="Grid Table 3 A
-00005e00: 6363 656e 7420 3522 2077 3a75 6950 7269  ccent 5" w:uiPri
-00005e10: 6f72 6974 793d 2234 3822 2f3e 3c77 3a6c  ority="48"/><w:l
-00005e20: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00005e30: 6d65 3d22 4772 6964 2054 6162 6c65 2034  me="Grid Table 4
-00005e40: 2041 6363 656e 7420 3522 2077 3a75 6950   Accent 5" w:uiP
-00005e50: 7269 6f72 6974 793d 2234 3922 2f3e 3c77  riority="49"/><w
-00005e60: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00005e70: 6e61 6d65 3d22 4772 6964 2054 6162 6c65  name="Grid Table
-00005e80: 2035 2044 6172 6b20 4163 6365 6e74 2035   5 Dark Accent 5
-00005e90: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00005ea0: 3530 222f 3e3c 773a 6c73 6445 7863 6570  50"/><w:lsdExcep
-00005eb0: 7469 6f6e 2077 3a6e 616d 653d 2247 7269  tion w:name="Gri
-00005ec0: 6420 5461 626c 6520 3620 436f 6c6f 7266  d Table 6 Colorf
-00005ed0: 756c 2041 6363 656e 7420 3522 2077 3a75  ul Accent 5" w:u
-00005ee0: 6950 7269 6f72 6974 793d 2235 3122 2f3e  iPriority="51"/>
-00005ef0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00005f00: 773a 6e61 6d65 3d22 4772 6964 2054 6162  w:name="Grid Tab
-00005f10: 6c65 2037 2043 6f6c 6f72 6675 6c20 4163  le 7 Colorful Ac
-00005f20: 6365 6e74 2035 2220 773a 7569 5072 696f  cent 5" w:uiPrio
-00005f30: 7269 7479 3d22 3532 222f 3e3c 773a 6c73  rity="52"/><w:ls
-00005f40: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-00005f50: 653d 2247 7269 6420 5461 626c 6520 3120  e="Grid Table 1 
-00005f60: 4c69 6768 7420 4163 6365 6e74 2036 2220  Light Accent 6" 
-00005f70: 773a 7569 5072 696f 7269 7479 3d22 3436  w:uiPriority="46
-00005f80: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00005f90: 6f6e 2077 3a6e 616d 653d 2247 7269 6420  on w:name="Grid 
-00005fa0: 5461 626c 6520 3220 4163 6365 6e74 2036  Table 2 Accent 6
-00005fb0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00005fc0: 3437 222f 3e3c 773a 6c73 6445 7863 6570  47"/><w:lsdExcep
-00005fd0: 7469 6f6e 2077 3a6e 616d 653d 2247 7269  tion w:name="Gri
-00005fe0: 6420 5461 626c 6520 3320 4163 6365 6e74  d Table 3 Accent
-00005ff0: 2036 2220 773a 7569 5072 696f 7269 7479   6" w:uiPriority
-00006000: 3d22 3438 222f 3e3c 773a 6c73 6445 7863  ="48"/><w:lsdExc
-00006010: 6570 7469 6f6e 2077 3a6e 616d 653d 2247  eption w:name="G
-00006020: 7269 6420 5461 626c 6520 3420 4163 6365  rid Table 4 Acce
-00006030: 6e74 2036 2220 773a 7569 5072 696f 7269  nt 6" w:uiPriori
-00006040: 7479 3d22 3439 222f 3e3c 773a 6c73 6445  ty="49"/><w:lsdE
-00006050: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00006060: 2247 7269 6420 5461 626c 6520 3520 4461  "Grid Table 5 Da
-00006070: 726b 2041 6363 656e 7420 3622 2077 3a75  rk Accent 6" w:u
-00006080: 6950 7269 6f72 6974 793d 2235 3022 2f3e  iPriority="50"/>
-00006090: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-000060a0: 773a 6e61 6d65 3d22 4772 6964 2054 6162  w:name="Grid Tab
-000060b0: 6c65 2036 2043 6f6c 6f72 6675 6c20 4163  le 6 Colorful Ac
-000060c0: 6365 6e74 2036 2220 773a 7569 5072 696f  cent 6" w:uiPrio
-000060d0: 7269 7479 3d22 3531 222f 3e3c 773a 6c73  rity="51"/><w:ls
-000060e0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000060f0: 653d 2247 7269 6420 5461 626c 6520 3720  e="Grid Table 7 
-00006100: 436f 6c6f 7266 756c 2041 6363 656e 7420  Colorful Accent 
-00006110: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
-00006120: 2235 3222 2f3e 3c77 3a6c 7364 4578 6365  "52"/><w:lsdExce
-00006130: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
-00006140: 7374 2054 6162 6c65 2031 204c 6967 6874  st Table 1 Light
-00006150: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00006160: 3436 222f 3e3c 773a 6c73 6445 7863 6570  46"/><w:lsdExcep
-00006170: 7469 6f6e 2077 3a6e 616d 653d 224c 6973  tion w:name="Lis
-00006180: 7420 5461 626c 6520 3222 2077 3a75 6950  t Table 2" w:uiP
-00006190: 7269 6f72 6974 793d 2234 3722 2f3e 3c77  riority="47"/><w
-000061a0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000061b0: 6e61 6d65 3d22 4c69 7374 2054 6162 6c65  name="List Table
-000061c0: 2033 2220 773a 7569 5072 696f 7269 7479   3" w:uiPriority
-000061d0: 3d22 3438 222f 3e3c 773a 6c73 6445 7863  ="48"/><w:lsdExc
-000061e0: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-000061f0: 6973 7420 5461 626c 6520 3422 2077 3a75  ist Table 4" w:u
-00006200: 6950 7269 6f72 6974 793d 2234 3922 2f3e  iPriority="49"/>
-00006210: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00006220: 773a 6e61 6d65 3d22 4c69 7374 2054 6162  w:name="List Tab
-00006230: 6c65 2035 2044 6172 6b22 2077 3a75 6950  le 5 Dark" w:uiP
-00006240: 7269 6f72 6974 793d 2235 3022 2f3e 3c77  riority="50"/><w
-00006250: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00006260: 6e61 6d65 3d22 4c69 7374 2054 6162 6c65  name="List Table
-00006270: 2036 2043 6f6c 6f72 6675 6c22 2077 3a75   6 Colorful" w:u
-00006280: 6950 7269 6f72 6974 793d 2235 3122 2f3e  iPriority="51"/>
-00006290: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-000062a0: 773a 6e61 6d65 3d22 4c69 7374 2054 6162  w:name="List Tab
-000062b0: 6c65 2037 2043 6f6c 6f72 6675 6c22 2077  le 7 Colorful" w
-000062c0: 3a75 6950 7269 6f72 6974 793d 2235 3222  :uiPriority="52"
-000062d0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-000062e0: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
-000062f0: 6162 6c65 2031 204c 6967 6874 2041 6363  able 1 Light Acc
-00006300: 656e 7420 3122 2077 3a75 6950 7269 6f72  ent 1" w:uiPrior
-00006310: 6974 793d 2234 3622 2f3e 3c77 3a6c 7364  ity="46"/><w:lsd
-00006320: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00006330: 3d22 4c69 7374 2054 6162 6c65 2032 2041  ="List Table 2 A
-00006340: 6363 656e 7420 3122 2077 3a75 6950 7269  ccent 1" w:uiPri
-00006350: 6f72 6974 793d 2234 3722 2f3e 3c77 3a6c  ority="47"/><w:l
-00006360: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00006370: 6d65 3d22 4c69 7374 2054 6162 6c65 2033  me="List Table 3
-00006380: 2041 6363 656e 7420 3122 2077 3a75 6950   Accent 1" w:uiP
-00006390: 7269 6f72 6974 793d 2234 3822 2f3e 3c77  riority="48"/><w
-000063a0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-000063b0: 6e61 6d65 3d22 4c69 7374 2054 6162 6c65  name="List Table
-000063c0: 2034 2041 6363 656e 7420 3122 2077 3a75   4 Accent 1" w:u
-000063d0: 6950 7269 6f72 6974 793d 2234 3922 2f3e  iPriority="49"/>
-000063e0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-000063f0: 773a 6e61 6d65 3d22 4c69 7374 2054 6162  w:name="List Tab
-00006400: 6c65 2035 2044 6172 6b20 4163 6365 6e74  le 5 Dark Accent
-00006410: 2031 2220 773a 7569 5072 696f 7269 7479   1" w:uiPriority
-00006420: 3d22 3530 222f 3e3c 773a 6c73 6445 7863  ="50"/><w:lsdExc
-00006430: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-00006440: 6973 7420 5461 626c 6520 3620 436f 6c6f  ist Table 6 Colo
-00006450: 7266 756c 2041 6363 656e 7420 3122 2077  rful Accent 1" w
-00006460: 3a75 6950 7269 6f72 6974 793d 2235 3122  :uiPriority="51"
-00006470: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00006480: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
-00006490: 6162 6c65 2037 2043 6f6c 6f72 6675 6c20  able 7 Colorful 
-000064a0: 4163 6365 6e74 2031 2220 773a 7569 5072  Accent 1" w:uiPr
-000064b0: 696f 7269 7479 3d22 3532 222f 3e3c 773a  iority="52"/><w:
-000064c0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-000064d0: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
-000064e0: 3120 4c69 6768 7420 4163 6365 6e74 2032  1 Light Accent 2
-000064f0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00006500: 3436 222f 3e3c 773a 6c73 6445 7863 6570  46"/><w:lsdExcep
-00006510: 7469 6f6e 2077 3a6e 616d 653d 224c 6973  tion w:name="Lis
-00006520: 7420 5461 626c 6520 3220 4163 6365 6e74  t Table 2 Accent
-00006530: 2032 2220 773a 7569 5072 696f 7269 7479   2" w:uiPriority
-00006540: 3d22 3437 222f 3e3c 773a 6c73 6445 7863  ="47"/><w:lsdExc
-00006550: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-00006560: 6973 7420 5461 626c 6520 3320 4163 6365  ist Table 3 Acce
-00006570: 6e74 2032 2220 773a 7569 5072 696f 7269  nt 2" w:uiPriori
-00006580: 7479 3d22 3438 222f 3e3c 773a 6c73 6445  ty="48"/><w:lsdE
-00006590: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-000065a0: 224c 6973 7420 5461 626c 6520 3420 4163  "List Table 4 Ac
-000065b0: 6365 6e74 2032 2220 773a 7569 5072 696f  cent 2" w:uiPrio
-000065c0: 7269 7479 3d22 3439 222f 3e3c 773a 6c73  rity="49"/><w:ls
-000065d0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000065e0: 653d 224c 6973 7420 5461 626c 6520 3520  e="List Table 5 
-000065f0: 4461 726b 2041 6363 656e 7420 3222 2077  Dark Accent 2" w
-00006600: 3a75 6950 7269 6f72 6974 793d 2235 3022  :uiPriority="50"
-00006610: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00006620: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
-00006630: 6162 6c65 2036 2043 6f6c 6f72 6675 6c20  able 6 Colorful 
-00006640: 4163 6365 6e74 2032 2220 773a 7569 5072  Accent 2" w:uiPr
-00006650: 696f 7269 7479 3d22 3531 222f 3e3c 773a  iority="51"/><w:
-00006660: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00006670: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
-00006680: 3720 436f 6c6f 7266 756c 2041 6363 656e  7 Colorful Accen
-00006690: 7420 3222 2077 3a75 6950 7269 6f72 6974  t 2" w:uiPriorit
-000066a0: 793d 2235 3222 2f3e 3c77 3a6c 7364 4578  y="52"/><w:lsdEx
-000066b0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-000066c0: 4c69 7374 2054 6162 6c65 2031 204c 6967  List Table 1 Lig
-000066d0: 6874 2041 6363 656e 7420 3322 2077 3a75  ht Accent 3" w:u
-000066e0: 6950 7269 6f72 6974 793d 2234 3622 2f3e  iPriority="46"/>
-000066f0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
-00006700: 773a 6e61 6d65 3d22 4c69 7374 2054 6162  w:name="List Tab
-00006710: 6c65 2032 2041 6363 656e 7420 3322 2077  le 2 Accent 3" w
-00006720: 3a75 6950 7269 6f72 6974 793d 2234 3722  :uiPriority="47"
-00006730: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
-00006740: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
-00006750: 6162 6c65 2033 2041 6363 656e 7420 3322  able 3 Accent 3"
-00006760: 2077 3a75 6950 7269 6f72 6974 793d 2234   w:uiPriority="4
-00006770: 3822 2f3e 3c77 3a6c 7364 4578 6365 7074  8"/><w:lsdExcept
-00006780: 696f 6e20 773a 6e61 6d65 3d22 4c69 7374  ion w:name="List
-00006790: 2054 6162 6c65 2034 2041 6363 656e 7420   Table 4 Accent 
-000067a0: 3322 2077 3a75 6950 7269 6f72 6974 793d  3" w:uiPriority=
-000067b0: 2234 3922 2f3e 3c77 3a6c 7364 4578 6365  "49"/><w:lsdExce
-000067c0: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
-000067d0: 7374 2054 6162 6c65 2035 2044 6172 6b20  st Table 5 Dark 
-000067e0: 4163 6365 6e74 2033 2220 773a 7569 5072  Accent 3" w:uiPr
-000067f0: 696f 7269 7479 3d22 3530 222f 3e3c 773a  iority="50"/><w:
-00006800: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00006810: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
-00006820: 3620 436f 6c6f 7266 756c 2041 6363 656e  6 Colorful Accen
-00006830: 7420 3322 2077 3a75 6950 7269 6f72 6974  t 3" w:uiPriorit
-00006840: 793d 2235 3122 2f3e 3c77 3a6c 7364 4578  y="51"/><w:lsdEx
-00006850: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00006860: 4c69 7374 2054 6162 6c65 2037 2043 6f6c  List Table 7 Col
-00006870: 6f72 6675 6c20 4163 6365 6e74 2033 2220  orful Accent 3" 
-00006880: 773a 7569 5072 696f 7269 7479 3d22 3532  w:uiPriority="52
-00006890: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-000068a0: 6f6e 2077 3a6e 616d 653d 224c 6973 7420  on w:name="List 
-000068b0: 5461 626c 6520 3120 4c69 6768 7420 4163  Table 1 Light Ac
-000068c0: 6365 6e74 2034 2220 773a 7569 5072 696f  cent 4" w:uiPrio
-000068d0: 7269 7479 3d22 3436 222f 3e3c 773a 6c73  rity="46"/><w:ls
-000068e0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
-000068f0: 653d 224c 6973 7420 5461 626c 6520 3220  e="List Table 2 
-00006900: 4163 6365 6e74 2034 2220 773a 7569 5072  Accent 4" w:uiPr
-00006910: 696f 7269 7479 3d22 3437 222f 3e3c 773a  iority="47"/><w:
-00006920: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
-00006930: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
-00006940: 3320 4163 6365 6e74 2034 2220 773a 7569  3 Accent 4" w:ui
-00006950: 5072 696f 7269 7479 3d22 3438 222f 3e3c  Priority="48"/><
-00006960: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
-00006970: 3a6e 616d 653d 224c 6973 7420 5461 626c  :name="List Tabl
-00006980: 6520 3420 4163 6365 6e74 2034 2220 773a  e 4 Accent 4" w:
-00006990: 7569 5072 696f 7269 7479 3d22 3439 222f  uiPriority="49"/
-000069a0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-000069b0: 2077 3a6e 616d 653d 224c 6973 7420 5461   w:name="List Ta
-000069c0: 626c 6520 3520 4461 726b 2041 6363 656e  ble 5 Dark Accen
-000069d0: 7420 3422 2077 3a75 6950 7269 6f72 6974  t 4" w:uiPriorit
-000069e0: 793d 2235 3022 2f3e 3c77 3a6c 7364 4578  y="50"/><w:lsdEx
-000069f0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00006a00: 4c69 7374 2054 6162 6c65 2036 2043 6f6c  List Table 6 Col
-00006a10: 6f72 6675 6c20 4163 6365 6e74 2034 2220  orful Accent 4" 
-00006a20: 773a 7569 5072 696f 7269 7479 3d22 3531  w:uiPriority="51
-00006a30: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00006a40: 6f6e 2077 3a6e 616d 653d 224c 6973 7420  on w:name="List 
-00006a50: 5461 626c 6520 3720 436f 6c6f 7266 756c  Table 7 Colorful
-00006a60: 2041 6363 656e 7420 3422 2077 3a75 6950   Accent 4" w:uiP
-00006a70: 7269 6f72 6974 793d 2235 3222 2f3e 3c77  riority="52"/><w
-00006a80: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00006a90: 6e61 6d65 3d22 4c69 7374 2054 6162 6c65  name="List Table
-00006aa0: 2031 204c 6967 6874 2041 6363 656e 7420   1 Light Accent 
-00006ab0: 3522 2077 3a75 6950 7269 6f72 6974 793d  5" w:uiPriority=
-00006ac0: 2234 3622 2f3e 3c77 3a6c 7364 4578 6365  "46"/><w:lsdExce
-00006ad0: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
-00006ae0: 7374 2054 6162 6c65 2032 2041 6363 656e  st Table 2 Accen
-00006af0: 7420 3522 2077 3a75 6950 7269 6f72 6974  t 5" w:uiPriorit
-00006b00: 793d 2234 3722 2f3e 3c77 3a6c 7364 4578  y="47"/><w:lsdEx
-00006b10: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
-00006b20: 4c69 7374 2054 6162 6c65 2033 2041 6363  List Table 3 Acc
-00006b30: 656e 7420 3522 2077 3a75 6950 7269 6f72  ent 5" w:uiPrior
-00006b40: 6974 793d 2234 3822 2f3e 3c77 3a6c 7364  ity="48"/><w:lsd
-00006b50: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
-00006b60: 3d22 4c69 7374 2054 6162 6c65 2034 2041  ="List Table 4 A
-00006b70: 6363 656e 7420 3522 2077 3a75 6950 7269  ccent 5" w:uiPri
-00006b80: 6f72 6974 793d 2234 3922 2f3e 3c77 3a6c  ority="49"/><w:l
-00006b90: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00006ba0: 6d65 3d22 4c69 7374 2054 6162 6c65 2035  me="List Table 5
-00006bb0: 2044 6172 6b20 4163 6365 6e74 2035 2220   Dark Accent 5" 
-00006bc0: 773a 7569 5072 696f 7269 7479 3d22 3530  w:uiPriority="50
-00006bd0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00006be0: 6f6e 2077 3a6e 616d 653d 224c 6973 7420  on w:name="List 
-00006bf0: 5461 626c 6520 3620 436f 6c6f 7266 756c  Table 6 Colorful
-00006c00: 2041 6363 656e 7420 3522 2077 3a75 6950   Accent 5" w:uiP
-00006c10: 7269 6f72 6974 793d 2235 3122 2f3e 3c77  riority="51"/><w
-00006c20: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00006c30: 6e61 6d65 3d22 4c69 7374 2054 6162 6c65  name="List Table
-00006c40: 2037 2043 6f6c 6f72 6675 6c20 4163 6365   7 Colorful Acce
-00006c50: 6e74 2035 2220 773a 7569 5072 696f 7269  nt 5" w:uiPriori
-00006c60: 7479 3d22 3532 222f 3e3c 773a 6c73 6445  ty="52"/><w:lsdE
-00006c70: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00006c80: 224c 6973 7420 5461 626c 6520 3120 4c69  "List Table 1 Li
-00006c90: 6768 7420 4163 6365 6e74 2036 2220 773a  ght Accent 6" w:
-00006ca0: 7569 5072 696f 7269 7479 3d22 3436 222f  uiPriority="46"/
-00006cb0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
-00006cc0: 2077 3a6e 616d 653d 224c 6973 7420 5461   w:name="List Ta
-00006cd0: 626c 6520 3220 4163 6365 6e74 2036 2220  ble 2 Accent 6" 
-00006ce0: 773a 7569 5072 696f 7269 7479 3d22 3437  w:uiPriority="47
-00006cf0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
-00006d00: 6f6e 2077 3a6e 616d 653d 224c 6973 7420  on w:name="List 
-00006d10: 5461 626c 6520 3320 4163 6365 6e74 2036  Table 3 Accent 6
-00006d20: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
-00006d30: 3438 222f 3e3c 773a 6c73 6445 7863 6570  48"/><w:lsdExcep
-00006d40: 7469 6f6e 2077 3a6e 616d 653d 224c 6973  tion w:name="Lis
-00006d50: 7420 5461 626c 6520 3420 4163 6365 6e74  t Table 4 Accent
-00006d60: 2036 2220 773a 7569 5072 696f 7269 7479   6" w:uiPriority
-00006d70: 3d22 3439 222f 3e3c 773a 6c73 6445 7863  ="49"/><w:lsdExc
-00006d80: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
-00006d90: 6973 7420 5461 626c 6520 3520 4461 726b  ist Table 5 Dark
-00006da0: 2041 6363 656e 7420 3622 2077 3a75 6950   Accent 6" w:uiP
-00006db0: 7269 6f72 6974 793d 2235 3022 2f3e 3c77  riority="50"/><w
-00006dc0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
-00006dd0: 6e61 6d65 3d22 4c69 7374 2054 6162 6c65  name="List Table
-00006de0: 2036 2043 6f6c 6f72 6675 6c20 4163 6365   6 Colorful Acce
-00006df0: 6e74 2036 2220 773a 7569 5072 696f 7269  nt 6" w:uiPriori
-00006e00: 7479 3d22 3531 222f 3e3c 773a 6c73 6445  ty="51"/><w:lsdE
-00006e10: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
-00006e20: 224c 6973 7420 5461 626c 6520 3720 436f  "List Table 7 Co
-00006e30: 6c6f 7266 756c 2041 6363 656e 7420 3622  lorful Accent 6"
-00006e40: 2077 3a75 6950 7269 6f72 6974 793d 2235   w:uiPriority="5
-00006e50: 3222 2f3e 3c77 3a6c 7364 4578 6365 7074  2"/><w:lsdExcept
-00006e60: 696f 6e20 773a 6e61 6d65 3d22 4d65 6e74  ion w:name="Ment
-00006e70: 696f 6e22 2077 3a73 656d 6948 6964 6465  ion" w:semiHidde
-00006e80: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
-00006e90: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
-00006ea0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00006eb0: 6d65 3d22 536d 6172 7420 4879 7065 726c  me="Smart Hyperl
-00006ec0: 696e 6b22 2077 3a73 656d 6948 6964 6465  ink" w:semiHidde
-00006ed0: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
-00006ee0: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
-00006ef0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
-00006f00: 6d65 3d22 4861 7368 7461 6722 2077 3a73  me="Hashtag" w:s
-00006f10: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
-00006f20: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
-00006f30: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
-00006f40: 696f 6e20 773a 6e61 6d65 3d22 556e 7265  ion w:name="Unre
-00006f50: 736f 6c76 6564 204d 656e 7469 6f6e 2220  solved Mention" 
-00006f60: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
-00006f70: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
-00006f80: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
-00006f90: 6570 7469 6f6e 2077 3a6e 616d 653d 2253  eption w:name="S
-00006fa0: 6d61 7274 204c 696e 6b22 2077 3a73 656d  mart Link" w:sem
-00006fb0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
-00006fc0: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
-00006fd0: 2f3e 3c2f 773a 6c61 7465 6e74 5374 796c  /></w:latentStyl
-00006fe0: 6573 3e3c 773a 7374 796c 6520 773a 7479  es><w:style w:ty
-00006ff0: 7065 3d22 7061 7261 6772 6170 6822 2077  pe="paragraph" w
-00007000: 3a64 6566 6175 6c74 3d22 3122 2077 3a73  :default="1" w:s
-00007010: 7479 6c65 4964 3d22 4e6f 726d 616c 223e  tyleId="Normal">
-00007020: 3c77 3a6e 616d 6520 773a 7661 6c3d 224e  <w:name w:val="N
-00007030: 6f72 6d61 6c22 2f3e 3c77 3a71 466f 726d  ormal"/><w:qForm
-00007040: 6174 2f3e 3c77 3a72 7369 6420 773a 7661  at/><w:rsid w:va
-00007050: 6c3d 2230 3037 3334 3146 3422 2f3e 3c2f  l="007341F4"/></
-00007060: 773a 7374 796c 653e 3c77 3a73 7479 6c65  w:style><w:style
-00007070: 2077 3a74 7970 653d 2270 6172 6167 7261   w:type="paragra
-00007080: 7068 2220 773a 7374 796c 6549 643d 2248  ph" w:styleId="H
-00007090: 6561 6469 6e67 3122 3e3c 773a 6e61 6d65  eading1"><w:name
-000070a0: 2077 3a76 616c 3d22 6865 6164 696e 6720   w:val="heading 
-000070b0: 3122 2f3e 3c77 3a62 6173 6564 4f6e 2077  1"/><w:basedOn w
-000070c0: 3a76 616c 3d22 4e6f 726d 616c 222f 3e3c  :val="Normal"/><
-000070d0: 773a 6e65 7874 2077 3a76 616c 3d22 4e6f  w:next w:val="No
-000070e0: 726d 616c 222f 3e3c 773a 6c69 6e6b 2077  rmal"/><w:link w
-000070f0: 3a76 616c 3d22 4865 6164 696e 6731 4368  :val="Heading1Ch
-00007100: 6172 222f 3e3c 773a 7569 5072 696f 7269  ar"/><w:uiPriori
-00007110: 7479 2077 3a76 616c 3d22 3922 2f3e 3c77  ty w:val="9"/><w
-00007120: 3a71 466f 726d 6174 2f3e 3c77 3a72 7369  :qFormat/><w:rsi
-00007130: 6420 773a 7661 6c3d 2230 3039 3836 3233  d w:val="0098623
-00007140: 3822 2f3e 3c77 3a70 5072 3e3c 773a 6b65  8"/><w:pPr><w:ke
-00007150: 6570 4e65 7874 2f3e 3c77 3a6b 6565 704c  epNext/><w:keepL
-00007160: 696e 6573 2f3e 3c77 3a73 7061 6369 6e67  ines/><w:spacing
-00007170: 2077 3a62 6566 6f72 653d 2232 3430 2220   w:before="240" 
-00007180: 773a 6166 7465 723d 2230 222f 3e3c 773a  w:after="0"/><w:
-00007190: 6f75 746c 696e 654c 766c 2077 3a76 616c  outlineLvl w:val
-000071a0: 3d22 3022 2f3e 3c2f 773a 7050 723e 3c77  ="0"/></w:pPr><w
-000071b0: 3a72 5072 3e3c 773a 7246 6f6e 7473 2077  :rPr><w:rFonts w
-000071c0: 3a61 7363 6969 5468 656d 653d 226d 616a  :asciiTheme="maj
-000071d0: 6f72 4841 6e73 6922 2077 3a65 6173 7441  orHAnsi" w:eastA
-000071e0: 7369 6154 6865 6d65 3d22 6d61 6a6f 7245  siaTheme="majorE
-000071f0: 6173 7441 7369 6122 2077 3a68 416e 7369  astAsia" w:hAnsi
-00007200: 5468 656d 653d 226d 616a 6f72 4841 6e73  Theme="majorHAns
-00007210: 6922 2077 3a63 7374 6865 6d65 3d22 6d61  i" w:cstheme="ma
-00007220: 6a6f 7242 6964 6922 2f3e 3c77 3a63 6f6c  jorBidi"/><w:col
-00007230: 6f72 2077 3a76 616c 3d22 3246 3534 3936  or w:val="2F5496
-00007240: 2220 773a 7468 656d 6543 6f6c 6f72 3d22  " w:themeColor="
-00007250: 6163 6365 6e74 3122 2077 3a74 6865 6d65  accent1" w:theme
-00007260: 5368 6164 653d 2242 4622 2f3e 3c77 3a73  Shade="BF"/><w:s
-00007270: 7a20 773a 7661 6c3d 2233 3222 2f3e 3c77  z w:val="32"/><w
-00007280: 3a73 7a43 7320 773a 7661 6c3d 2233 3222  :szCs w:val="32"
-00007290: 2f3e 3c2f 773a 7250 723e 3c2f 773a 7374  /></w:rPr></w:st
-000072a0: 796c 653e 3c77 3a73 7479 6c65 2077 3a74  yle><w:style w:t
-000072b0: 7970 653d 2270 6172 6167 7261 7068 2220  ype="paragraph" 
-000072c0: 773a 7374 796c 6549 643d 2248 6561 6469  w:styleId="Headi
-000072d0: 6e67 3222 3e3c 773a 6e61 6d65 2077 3a76  ng2"><w:name w:v
-000072e0: 616c 3d22 6865 6164 696e 6720 3222 2f3e  al="heading 2"/>
-000072f0: 3c77 3a62 6173 6564 4f6e 2077 3a76 616c  <w:basedOn w:val
-00007300: 3d22 4e6f 726d 616c 222f 3e3c 773a 6e65  ="Normal"/><w:ne
-00007310: 7874 2077 3a76 616c 3d22 4e6f 726d 616c  xt w:val="Normal
-00007320: 222f 3e3c 773a 6c69 6e6b 2077 3a76 616c  "/><w:link w:val
-00007330: 3d22 4865 6164 696e 6732 4368 6172 222f  ="Heading2Char"/
-00007340: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
-00007350: 3a76 616c 3d22 3922 2f3e 3c77 3a75 6e68  :val="9"/><w:unh
-00007360: 6964 6557 6865 6e55 7365 642f 3e3c 773a  ideWhenUsed/><w:
-00007370: 7146 6f72 6d61 742f 3e3c 773a 7273 6964  qFormat/><w:rsid
-00007380: 2077 3a76 616c 3d22 3030 3938 3632 3338   w:val="00986238
-00007390: 222f 3e3c 773a 7050 723e 3c77 3a6b 6565  "/><w:pPr><w:kee
-000073a0: 704e 6578 742f 3e3c 773a 6b65 6570 4c69  pNext/><w:keepLi
-000073b0: 6e65 732f 3e3c 773a 7370 6163 696e 6720  nes/><w:spacing 
-000073c0: 773a 6265 666f 7265 3d22 3430 2220 773a  w:before="40" w:
-000073d0: 6166 7465 723d 2230 222f 3e3c 773a 6f75  after="0"/><w:ou
-000073e0: 746c 696e 654c 766c 2077 3a76 616c 3d22  tlineLvl w:val="
-000073f0: 3122 2f3e 3c2f 773a 7050 723e 3c77 3a72  1"/></w:pPr><w:r
-00007400: 5072 3e3c 773a 7246 6f6e 7473 2077 3a61  Pr><w:rFonts w:a
-00007410: 7363 6969 5468 656d 653d 226d 616a 6f72  sciiTheme="major
-00007420: 4841 6e73 6922 2077 3a65 6173 7441 7369  HAnsi" w:eastAsi
-00007430: 6154 6865 6d65 3d22 6d61 6a6f 7245 6173  aTheme="majorEas
-00007440: 7441 7369 6122 2077 3a68 416e 7369 5468  tAsia" w:hAnsiTh
-00007450: 656d 653d 226d 616a 6f72 4841 6e73 6922  eme="majorHAnsi"
-00007460: 2077 3a63 7374 6865 6d65 3d22 6d61 6a6f   w:cstheme="majo
-00007470: 7242 6964 6922 2f3e 3c77 3a63 6f6c 6f72  rBidi"/><w:color
-00007480: 2077 3a76 616c 3d22 3246 3534 3936 2220   w:val="2F5496" 
-00007490: 773a 7468 656d 6543 6f6c 6f72 3d22 6163  w:themeColor="ac
-000074a0: 6365 6e74 3122 2077 3a74 6865 6d65 5368  cent1" w:themeSh
-000074b0: 6164 653d 2242 4622 2f3e 3c77 3a73 7a20  ade="BF"/><w:sz 
-000074c0: 773a 7661 6c3d 2232 3622 2f3e 3c77 3a73  w:val="26"/><w:s
-000074d0: 7a43 7320 773a 7661 6c3d 2232 3622 2f3e  zCs w:val="26"/>
-000074e0: 3c2f 773a 7250 723e 3c2f 773a 7374 796c  </w:rPr></w:styl
-000074f0: 653e 3c77 3a73 7479 6c65 2077 3a74 7970  e><w:style w:typ
-00007500: 653d 2270 6172 6167 7261 7068 2220 773a  e="paragraph" w:
-00007510: 7374 796c 6549 643d 2248 6561 6469 6e67  styleId="Heading
-00007520: 3322 3e3c 773a 6e61 6d65 2077 3a76 616c  3"><w:name w:val
-00007530: 3d22 6865 6164 696e 6720 3322 2f3e 3c77  ="heading 3"/><w
-00007540: 3a62 6173 6564 4f6e 2077 3a76 616c 3d22  :basedOn w:val="
-00007550: 4e6f 726d 616c 222f 3e3c 773a 6e65 7874  Normal"/><w:next
-00007560: 2077 3a76 616c 3d22 4e6f 726d 616c 222f   w:val="Normal"/
-00007570: 3e3c 773a 6c69 6e6b 2077 3a76 616c 3d22  ><w:link w:val="
-00007580: 4865 6164 696e 6733 4368 6172 222f 3e3c  Heading3Char"/><
-00007590: 773a 7569 5072 696f 7269 7479 2077 3a76  w:uiPriority w:v
-000075a0: 616c 3d22 3922 2f3e 3c77 3a75 6e68 6964  al="9"/><w:unhid
-000075b0: 6557 6865 6e55 7365 642f 3e3c 773a 7146  eWhenUsed/><w:qF
-000075c0: 6f72 6d61 742f 3e3c 773a 7273 6964 2077  ormat/><w:rsid w
-000075d0: 3a76 616c 3d22 3030 3938 3632 3338 222f  :val="00986238"/
-000075e0: 3e3c 773a 7050 723e 3c77 3a6b 6565 704e  ><w:pPr><w:keepN
-000075f0: 6578 742f 3e3c 773a 6b65 6570 4c69 6e65  ext/><w:keepLine
-00007600: 732f 3e3c 773a 7370 6163 696e 6720 773a  s/><w:spacing w:
-00007610: 6265 666f 7265 3d22 3430 2220 773a 6166  before="40" w:af
-00007620: 7465 723d 2230 222f 3e3c 773a 6f75 746c  ter="0"/><w:outl
-00007630: 696e 654c 766c 2077 3a76 616c 3d22 3222  ineLvl w:val="2"
-00007640: 2f3e 3c2f 773a 7050 723e 3c77 3a72 5072  /></w:pPr><w:rPr
-00007650: 3e3c 773a 7246 6f6e 7473 2077 3a61 7363  ><w:rFonts w:asc
-00007660: 6969 5468 656d 653d 226d 616a 6f72 4841  iiTheme="majorHA
-00007670: 6e73 6922 2077 3a65 6173 7441 7369 6154  nsi" w:eastAsiaT
-00007680: 6865 6d65 3d22 6d61 6a6f 7245 6173 7441  heme="majorEastA
-00007690: 7369 6122 2077 3a68 416e 7369 5468 656d  sia" w:hAnsiThem
-000076a0: 653d 226d 616a 6f72 4841 6e73 6922 2077  e="majorHAnsi" w
-000076b0: 3a63 7374 6865 6d65 3d22 6d61 6a6f 7242  :cstheme="majorB
-000076c0: 6964 6922 2f3e 3c77 3a63 6f6c 6f72 2077  idi"/><w:color w
-000076d0: 3a76 616c 3d22 3146 3337 3633 2220 773a  :val="1F3763" w:
-000076e0: 7468 656d 6543 6f6c 6f72 3d22 6163 6365  themeColor="acce
-000076f0: 6e74 3122 2077 3a74 6865 6d65 5368 6164  nt1" w:themeShad
-00007700: 653d 2237 4622 2f3e 3c77 3a73 7a20 773a  e="7F"/><w:sz w:
-00007710: 7661 6c3d 2232 3422 2f3e 3c77 3a73 7a43  val="24"/><w:szC
-00007720: 7320 773a 7661 6c3d 2232 3422 2f3e 3c2f  s w:val="24"/></
-00007730: 773a 7250 723e 3c2f 773a 7374 796c 653e  w:rPr></w:style>
-00007740: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
-00007750: 2270 6172 6167 7261 7068 2220 773a 7374  "paragraph" w:st
-00007760: 796c 6549 643d 2248 6561 6469 6e67 3422  yleId="Heading4"
-00007770: 3e3c 773a 6e61 6d65 2077 3a76 616c 3d22  ><w:name w:val="
-00007780: 6865 6164 696e 6720 3422 2f3e 3c77 3a62  heading 4"/><w:b
-00007790: 6173 6564 4f6e 2077 3a76 616c 3d22 4e6f  asedOn w:val="No
-000077a0: 726d 616c 222f 3e3c 773a 6e65 7874 2077  rmal"/><w:next w
-000077b0: 3a76 616c 3d22 4e6f 726d 616c 222f 3e3c  :val="Normal"/><
-000077c0: 773a 6c69 6e6b 2077 3a76 616c 3d22 4865  w:link w:val="He
-000077d0: 6164 696e 6734 4368 6172 222f 3e3c 773a  ading4Char"/><w:
-000077e0: 7569 5072 696f 7269 7479 2077 3a76 616c  uiPriority w:val
-000077f0: 3d22 3922 2f3e 3c77 3a75 6e68 6964 6557  ="9"/><w:unhideW
-00007800: 6865 6e55 7365 642f 3e3c 773a 7146 6f72  henUsed/><w:qFor
-00007810: 6d61 742f 3e3c 773a 7273 6964 2077 3a76  mat/><w:rsid w:v
-00007820: 616c 3d22 3030 3938 3632 3338 222f 3e3c  al="00986238"/><
-00007830: 773a 7050 723e 3c77 3a6b 6565 704e 6578  w:pPr><w:keepNex
-00007840: 742f 3e3c 773a 6b65 6570 4c69 6e65 732f  t/><w:keepLines/
-00007850: 3e3c 773a 7370 6163 696e 6720 773a 6265  ><w:spacing w:be
-00007860: 666f 7265 3d22 3430 2220 773a 6166 7465  fore="40" w:afte
-00007870: 723d 2230 222f 3e3c 773a 6f75 746c 696e  r="0"/><w:outlin
-00007880: 654c 766c 2077 3a76 616c 3d22 3322 2f3e  eLvl w:val="3"/>
-00007890: 3c2f 773a 7050 723e 3c77 3a72 5072 3e3c  </w:pPr><w:rPr><
-000078a0: 773a 7246 6f6e 7473 2077 3a61 7363 6969  w:rFonts w:ascii
-000078b0: 5468 656d 653d 226d 616a 6f72 4841 6e73  Theme="majorHAns
-000078c0: 6922 2077 3a65 6173 7441 7369 6154 6865  i" w:eastAsiaThe
-000078d0: 6d65 3d22 6d61 6a6f 7245 6173 7441 7369  me="majorEastAsi
-000078e0: 6122 2077 3a68 416e 7369 5468 656d 653d  a" w:hAnsiTheme=
-000078f0: 226d 616a 6f72 4841 6e73 6922 2077 3a63  "majorHAnsi" w:c
-00007900: 7374 6865 6d65 3d22 6d61 6a6f 7242 6964  stheme="majorBid
-00007910: 6922 2f3e 3c77 3a69 2f3e 3c77 3a69 4373  i"/><w:i/><w:iCs
-00007920: 2f3e 3c77 3a63 6f6c 6f72 2077 3a76 616c  /><w:color w:val
-00007930: 3d22 3246 3534 3936 2220 773a 7468 656d  ="2F5496" w:them
-00007940: 6543 6f6c 6f72 3d22 6163 6365 6e74 3122  eColor="accent1"
-00007950: 2077 3a74 6865 6d65 5368 6164 653d 2242   w:themeShade="B
-00007960: 4622 2f3e 3c2f 773a 7250 723e 3c2f 773a  F"/></w:rPr></w:
-00007970: 7374 796c 653e 3c77 3a73 7479 6c65 2077  style><w:style w
-00007980: 3a74 7970 653d 2270 6172 6167 7261 7068  :type="paragraph
-00007990: 2220 773a 7374 796c 6549 643d 2248 6561  " w:styleId="Hea
-000079a0: 6469 6e67 3522 3e3c 773a 6e61 6d65 2077  ding5"><w:name w
-000079b0: 3a76 616c 3d22 6865 6164 696e 6720 3522  :val="heading 5"
-000079c0: 2f3e 3c77 3a62 6173 6564 4f6e 2077 3a76  /><w:basedOn w:v
-000079d0: 616c 3d22 4e6f 726d 616c 222f 3e3c 773a  al="Normal"/><w:
-000079e0: 6e65 7874 2077 3a76 616c 3d22 4e6f 726d  next w:val="Norm
-000079f0: 616c 222f 3e3c 773a 6c69 6e6b 2077 3a76  al"/><w:link w:v
-00007a00: 616c 3d22 4865 6164 696e 6735 4368 6172  al="Heading5Char
-00007a10: 222f 3e3c 773a 7569 5072 696f 7269 7479  "/><w:uiPriority
-00007a20: 2077 3a76 616c 3d22 3922 2f3e 3c77 3a75   w:val="9"/><w:u
-00007a30: 6e68 6964 6557 6865 6e55 7365 642f 3e3c  nhideWhenUsed/><
-00007a40: 773a 7146 6f72 6d61 742f 3e3c 773a 7273  w:qFormat/><w:rs
-00007a50: 6964 2077 3a76 616c 3d22 3030 3938 3632  id w:val="009862
-00007a60: 3338 222f 3e3c 773a 7050 723e 3c77 3a6b  38"/><w:pPr><w:k
-00007a70: 6565 704e 6578 742f 3e3c 773a 6b65 6570  eepNext/><w:keep
-00007a80: 4c69 6e65 732f 3e3c 773a 7370 6163 696e  Lines/><w:spacin
-00007a90: 6720 773a 6265 666f 7265 3d22 3430 2220  g w:before="40" 
-00007aa0: 773a 6166 7465 723d 2230 222f 3e3c 773a  w:after="0"/><w:
-00007ab0: 6f75 746c 696e 654c 766c 2077 3a76 616c  outlineLvl w:val
-00007ac0: 3d22 3422 2f3e 3c2f 773a 7050 723e 3c77  ="4"/></w:pPr><w
-00007ad0: 3a72 5072 3e3c 773a 7246 6f6e 7473 2077  :rPr><w:rFonts w
-00007ae0: 3a61 7363 6969 5468 656d 653d 226d 616a  :asciiTheme="maj
-00007af0: 6f72 4841 6e73 6922 2077 3a65 6173 7441  orHAnsi" w:eastA
-00007b00: 7369 6154 6865 6d65 3d22 6d61 6a6f 7245  siaTheme="majorE
-00007b10: 6173 7441 7369 6122 2077 3a68 416e 7369  astAsia" w:hAnsi
-00007b20: 5468 656d 653d 226d 616a 6f72 4841 6e73  Theme="majorHAns
-00007b30: 6922 2077 3a63 7374 6865 6d65 3d22 6d61  i" w:cstheme="ma
-00007b40: 6a6f 7242 6964 6922 2f3e 3c77 3a63 6f6c  jorBidi"/><w:col
-00007b50: 6f72 2077 3a76 616c 3d22 3246 3534 3936  or w:val="2F5496
-00007b60: 2220 773a 7468 656d 6543 6f6c 6f72 3d22  " w:themeColor="
-00007b70: 6163 6365 6e74 3122 2077 3a74 6865 6d65  accent1" w:theme
-00007b80: 5368 6164 653d 2242 4622 2f3e 3c2f 773a  Shade="BF"/></w:
-00007b90: 7250 723e 3c2f 773a 7374 796c 653e 3c77  rPr></w:style><w
-00007ba0: 3a73 7479 6c65 2077 3a74 7970 653d 2263  :style w:type="c
-00007bb0: 6861 7261 6374 6572 2220 773a 6465 6661  haracter" w:defa
-00007bc0: 756c 743d 2231 2220 773a 7374 796c 6549  ult="1" w:styleI
-00007bd0: 643d 2244 6566 6175 6c74 5061 7261 6772  d="DefaultParagr
-00007be0: 6170 6846 6f6e 7422 3e3c 773a 6e61 6d65  aphFont"><w:name
-00007bf0: 2077 3a76 616c 3d22 4465 6661 756c 7420   w:val="Default 
-00007c00: 5061 7261 6772 6170 6820 466f 6e74 222f  Paragraph Font"/
-00007c10: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
-00007c20: 3a76 616c 3d22 3122 2f3e 3c77 3a73 656d  :val="1"/><w:sem
-00007c30: 6948 6964 6465 6e2f 3e3c 773a 756e 6869  iHidden/><w:unhi
-00007c40: 6465 5768 656e 5573 6564 2f3e 3c2f 773a  deWhenUsed/></w:
-00007c50: 7374 796c 653e 3c77 3a73 7479 6c65 2077  style><w:style w
-00007c60: 3a74 7970 653d 2274 6162 6c65 2220 773a  :type="table" w:
-00007c70: 6465 6661 756c 743d 2231 2220 773a 7374  default="1" w:st
-00007c80: 796c 6549 643d 2254 6162 6c65 4e6f 726d  yleId="TableNorm
-00007c90: 616c 223e 3c77 3a6e 616d 6520 773a 7661  al"><w:name w:va
-00007ca0: 6c3d 224e 6f72 6d61 6c20 5461 626c 6522  l="Normal Table"
-00007cb0: 2f3e 3c77 3a75 6950 7269 6f72 6974 7920  /><w:uiPriority 
-00007cc0: 773a 7661 6c3d 2239 3922 2f3e 3c77 3a73  w:val="99"/><w:s
-00007cd0: 656d 6948 6964 6465 6e2f 3e3c 773a 756e  emiHidden/><w:un
-00007ce0: 6869 6465 5768 656e 5573 6564 2f3e 3c77  hideWhenUsed/><w
-00007cf0: 3a74 626c 5072 3e3c 773a 7462 6c49 6e64  :tblPr><w:tblInd
-00007d00: 2077 3a77 3d22 3022 2077 3a74 7970 653d   w:w="0" w:type=
-00007d10: 2264 7861 222f 3e3c 773a 7462 6c43 656c  "dxa"/><w:tblCel
-00007d20: 6c4d 6172 3e3c 773a 746f 7020 773a 773d  lMar><w:top w:w=
-00007d30: 2230 2220 773a 7479 7065 3d22 6478 6122  "0" w:type="dxa"
-00007d40: 2f3e 3c77 3a6c 6566 7420 773a 773d 2231  /><w:left w:w="1
-00007d50: 3038 2220 773a 7479 7065 3d22 6478 6122  08" w:type="dxa"
-00007d60: 2f3e 3c77 3a62 6f74 746f 6d20 773a 773d  /><w:bottom w:w=
-00007d70: 2230 2220 773a 7479 7065 3d22 6478 6122  "0" w:type="dxa"
-00007d80: 2f3e 3c77 3a72 6967 6874 2077 3a77 3d22  /><w:right w:w="
-00007d90: 3130 3822 2077 3a74 7970 653d 2264 7861  108" w:type="dxa
-00007da0: 222f 3e3c 2f77 3a74 626c 4365 6c6c 4d61  "/></w:tblCellMa
-00007db0: 723e 3c2f 773a 7462 6c50 723e 3c2f 773a  r></w:tblPr></w:
-00007dc0: 7374 796c 653e 3c77 3a73 7479 6c65 2077  style><w:style w
-00007dd0: 3a74 7970 653d 226e 756d 6265 7269 6e67  :type="numbering
-00007de0: 2220 773a 6465 6661 756c 743d 2231 2220  " w:default="1" 
-00007df0: 773a 7374 796c 6549 643d 224e 6f4c 6973  w:styleId="NoLis
-00007e00: 7422 3e3c 773a 6e61 6d65 2077 3a76 616c  t"><w:name w:val
-00007e10: 3d22 4e6f 204c 6973 7422 2f3e 3c77 3a75  ="No List"/><w:u
-00007e20: 6950 7269 6f72 6974 7920 773a 7661 6c3d  iPriority w:val=
-00007e30: 2239 3922 2f3e 3c77 3a73 656d 6948 6964  "99"/><w:semiHid
-00007e40: 6465 6e2f 3e3c 773a 756e 6869 6465 5768  den/><w:unhideWh
-00007e50: 656e 5573 6564 2f3e 3c2f 773a 7374 796c  enUsed/></w:styl
-00007e60: 653e 3c77 3a73 7479 6c65 2077 3a74 7970  e><w:style w:typ
-00007e70: 653d 2270 6172 6167 7261 7068 2220 773a  e="paragraph" w:
-00007e80: 7374 796c 6549 643d 2254 6974 6c65 223e  styleId="Title">
-00007e90: 3c77 3a6e 616d 6520 773a 7661 6c3d 2254  <w:name w:val="T
-00007ea0: 6974 6c65 222f 3e3c 773a 6261 7365 644f  itle"/><w:basedO
-00007eb0: 6e20 773a 7661 6c3d 224e 6f72 6d61 6c22  n w:val="Normal"
-00007ec0: 2f3e 3c77 3a6e 6578 7420 773a 7661 6c3d  /><w:next w:val=
-00007ed0: 224e 6f72 6d61 6c22 2f3e 3c77 3a6c 696e  "Normal"/><w:lin
-00007ee0: 6b20 773a 7661 6c3d 2254 6974 6c65 4368  k w:val="TitleCh
-00007ef0: 6172 222f 3e3c 773a 7569 5072 696f 7269  ar"/><w:uiPriori
-00007f00: 7479 2077 3a76 616c 3d22 3130 222f 3e3c  ty w:val="10"/><
-00007f10: 773a 7146 6f72 6d61 742f 3e3c 773a 7273  w:qFormat/><w:rs
-00007f20: 6964 2077 3a76 616c 3d22 3030 3736 3544  id w:val="00765D
-00007f30: 3735 222f 3e3c 773a 7050 723e 3c77 3a73  75"/><w:pPr><w:s
-00007f40: 7061 6369 6e67 2077 3a61 6674 6572 3d22  pacing w:after="
-00007f50: 3022 2077 3a6c 696e 653d 2232 3430 2220  0" w:line="240" 
-00007f60: 773a 6c69 6e65 5275 6c65 3d22 6175 746f  w:lineRule="auto
-00007f70: 222f 3e3c 773a 636f 6e74 6578 7475 616c  "/><w:contextual
-00007f80: 5370 6163 696e 672f 3e3c 2f77 3a70 5072  Spacing/></w:pPr
-00007f90: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
-00007fa0: 7320 773a 6173 6369 6954 6865 6d65 3d22  s w:asciiTheme="
-00007fb0: 6d61 6a6f 7248 416e 7369 2220 773a 6561  majorHAnsi" w:ea
-00007fc0: 7374 4173 6961 5468 656d 653d 226d 616a  stAsiaTheme="maj
-00007fd0: 6f72 4561 7374 4173 6961 2220 773a 6841  orEastAsia" w:hA
-00007fe0: 6e73 6954 6865 6d65 3d22 6d61 6a6f 7248  nsiTheme="majorH
-00007ff0: 416e 7369 2220 773a 6373 7468 656d 653d  Ansi" w:cstheme=
-00008000: 226d 616a 6f72 4269 6469 222f 3e3c 773a  "majorBidi"/><w:
-00008010: 7370 6163 696e 6720 773a 7661 6c3d 222d  spacing w:val="-
-00008020: 3130 222f 3e3c 773a 6b65 726e 2077 3a76  10"/><w:kern w:v
-00008030: 616c 3d22 3238 222f 3e3c 773a 737a 2077  al="28"/><w:sz w
-00008040: 3a76 616c 3d22 3536 222f 3e3c 773a 737a  :val="56"/><w:sz
-00008050: 4373 2077 3a76 616c 3d22 3536 222f 3e3c  Cs w:val="56"/><
-00008060: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
-00008070: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
-00008080: 3d22 6368 6172 6163 7465 7222 2077 3a63  ="character" w:c
-00008090: 7573 746f 6d53 7479 6c65 3d22 3122 2077  ustomStyle="1" w
-000080a0: 3a73 7479 6c65 4964 3d22 5469 746c 6543  :styleId="TitleC
-000080b0: 6861 7222 3e3c 773a 6e61 6d65 2077 3a76  har"><w:name w:v
-000080c0: 616c 3d22 5469 746c 6520 4368 6172 222f  al="Title Char"/
-000080d0: 3e3c 773a 6261 7365 644f 6e20 773a 7661  ><w:basedOn w:va
-000080e0: 6c3d 2244 6566 6175 6c74 5061 7261 6772  l="DefaultParagr
-000080f0: 6170 6846 6f6e 7422 2f3e 3c77 3a6c 696e  aphFont"/><w:lin
-00008100: 6b20 773a 7661 6c3d 2254 6974 6c65 222f  k w:val="Title"/
-00008110: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
-00008120: 3a76 616c 3d22 3130 222f 3e3c 773a 7273  :val="10"/><w:rs
-00008130: 6964 2077 3a76 616c 3d22 3030 3736 3544  id w:val="00765D
-00008140: 3735 222f 3e3c 773a 7250 723e 3c77 3a72  75"/><w:rPr><w:r
-00008150: 466f 6e74 7320 773a 6173 6369 6954 6865  Fonts w:asciiThe
-00008160: 6d65 3d22 6d61 6a6f 7248 416e 7369 2220  me="majorHAnsi" 
-00008170: 773a 6561 7374 4173 6961 5468 656d 653d  w:eastAsiaTheme=
-00008180: 226d 616a 6f72 4561 7374 4173 6961 2220  "majorEastAsia" 
-00008190: 773a 6841 6e73 6954 6865 6d65 3d22 6d61  w:hAnsiTheme="ma
-000081a0: 6a6f 7248 416e 7369 2220 773a 6373 7468  jorHAnsi" w:csth
-000081b0: 656d 653d 226d 616a 6f72 4269 6469 222f  eme="majorBidi"/
-000081c0: 3e3c 773a 7370 6163 696e 6720 773a 7661  ><w:spacing w:va
-000081d0: 6c3d 222d 3130 222f 3e3c 773a 6b65 726e  l="-10"/><w:kern
-000081e0: 2077 3a76 616c 3d22 3238 222f 3e3c 773a   w:val="28"/><w:
-000081f0: 737a 2077 3a76 616c 3d22 3536 222f 3e3c  sz w:val="56"/><
-00008200: 773a 737a 4373 2077 3a76 616c 3d22 3536  w:szCs w:val="56
-00008210: 222f 3e3c 2f77 3a72 5072 3e3c 2f77 3a73  "/></w:rPr></w:s
-00008220: 7479 6c65 3e3c 773a 7374 796c 6520 773a  tyle><w:style w:
-00008230: 7479 7065 3d22 6368 6172 6163 7465 7222  type="character"
-00008240: 2077 3a63 7573 746f 6d53 7479 6c65 3d22   w:customStyle="
-00008250: 3122 2077 3a73 7479 6c65 4964 3d22 4865  1" w:styleId="He
-00008260: 6164 696e 6731 4368 6172 223e 3c77 3a6e  ading1Char"><w:n
-00008270: 616d 6520 773a 7661 6c3d 2248 6561 6469  ame w:val="Headi
-00008280: 6e67 2031 2043 6861 7222 2f3e 3c77 3a62  ng 1 Char"/><w:b
-00008290: 6173 6564 4f6e 2077 3a76 616c 3d22 4465  asedOn w:val="De
-000082a0: 6661 756c 7450 6172 6167 7261 7068 466f  faultParagraphFo
-000082b0: 6e74 222f 3e3c 773a 6c69 6e6b 2077 3a76  nt"/><w:link w:v
-000082c0: 616c 3d22 4865 6164 696e 6731 222f 3e3c  al="Heading1"/><
-000082d0: 773a 7569 5072 696f 7269 7479 2077 3a76  w:uiPriority w:v
-000082e0: 616c 3d22 3922 2f3e 3c77 3a72 7369 6420  al="9"/><w:rsid 
-000082f0: 773a 7661 6c3d 2230 3039 3836 3233 3822  w:val="00986238"
-00008300: 2f3e 3c77 3a72 5072 3e3c 773a 7246 6f6e  /><w:rPr><w:rFon
-00008310: 7473 2077 3a61 7363 6969 5468 656d 653d  ts w:asciiTheme=
-00008320: 226d 616a 6f72 4841 6e73 6922 2077 3a65  "majorHAnsi" w:e
-00008330: 6173 7441 7369 6154 6865 6d65 3d22 6d61  astAsiaTheme="ma
-00008340: 6a6f 7245 6173 7441 7369 6122 2077 3a68  jorEastAsia" w:h
-00008350: 416e 7369 5468 656d 653d 226d 616a 6f72  AnsiTheme="major
-00008360: 4841 6e73 6922 2077 3a63 7374 6865 6d65  HAnsi" w:cstheme
-00008370: 3d22 6d61 6a6f 7242 6964 6922 2f3e 3c77  ="majorBidi"/><w
-00008380: 3a63 6f6c 6f72 2077 3a76 616c 3d22 3246  :color w:val="2F
-00008390: 3534 3936 2220 773a 7468 656d 6543 6f6c  5496" w:themeCol
-000083a0: 6f72 3d22 6163 6365 6e74 3122 2077 3a74  or="accent1" w:t
-000083b0: 6865 6d65 5368 6164 653d 2242 4622 2f3e  hemeShade="BF"/>
-000083c0: 3c77 3a73 7a20 773a 7661 6c3d 2233 3222  <w:sz w:val="32"
-000083d0: 2f3e 3c77 3a73 7a43 7320 773a 7661 6c3d  /><w:szCs w:val=
-000083e0: 2233 3222 2f3e 3c2f 773a 7250 723e 3c2f  "32"/></w:rPr></
-000083f0: 773a 7374 796c 653e 3c77 3a73 7479 6c65  w:style><w:style
-00008400: 2077 3a74 7970 653d 2263 6861 7261 6374   w:type="charact
-00008410: 6572 2220 773a 6375 7374 6f6d 5374 796c  er" w:customStyl
-00008420: 653d 2231 2220 773a 7374 796c 6549 643d  e="1" w:styleId=
-00008430: 2248 6561 6469 6e67 3243 6861 7222 3e3c  "Heading2Char"><
-00008440: 773a 6e61 6d65 2077 3a76 616c 3d22 4865  w:name w:val="He
-00008450: 6164 696e 6720 3220 4368 6172 222f 3e3c  ading 2 Char"/><
-00008460: 773a 6261 7365 644f 6e20 773a 7661 6c3d  w:basedOn w:val=
-00008470: 2244 6566 6175 6c74 5061 7261 6772 6170  "DefaultParagrap
-00008480: 6846 6f6e 7422 2f3e 3c77 3a6c 696e 6b20  hFont"/><w:link 
-00008490: 773a 7661 6c3d 2248 6561 6469 6e67 3222  w:val="Heading2"
-000084a0: 2f3e 3c77 3a75 6950 7269 6f72 6974 7920  /><w:uiPriority 
-000084b0: 773a 7661 6c3d 2239 222f 3e3c 773a 7273  w:val="9"/><w:rs
-000084c0: 6964 2077 3a76 616c 3d22 3030 3938 3632  id w:val="009862
-000084d0: 3338 222f 3e3c 773a 7250 723e 3c77 3a72  38"/><w:rPr><w:r
-000084e0: 466f 6e74 7320 773a 6173 6369 6954 6865  Fonts w:asciiThe
-000084f0: 6d65 3d22 6d61 6a6f 7248 416e 7369 2220  me="majorHAnsi" 
-00008500: 773a 6561 7374 4173 6961 5468 656d 653d  w:eastAsiaTheme=
-00008510: 226d 616a 6f72 4561 7374 4173 6961 2220  "majorEastAsia" 
-00008520: 773a 6841 6e73 6954 6865 6d65 3d22 6d61  w:hAnsiTheme="ma
-00008530: 6a6f 7248 416e 7369 2220 773a 6373 7468  jorHAnsi" w:csth
-00008540: 656d 653d 226d 616a 6f72 4269 6469 222f  eme="majorBidi"/
-00008550: 3e3c 773a 636f 6c6f 7220 773a 7661 6c3d  ><w:color w:val=
-00008560: 2232 4635 3439 3622 2077 3a74 6865 6d65  "2F5496" w:theme
-00008570: 436f 6c6f 723d 2261 6363 656e 7431 2220  Color="accent1" 
-00008580: 773a 7468 656d 6553 6861 6465 3d22 4246  w:themeShade="BF
-00008590: 222f 3e3c 773a 737a 2077 3a76 616c 3d22  "/><w:sz w:val="
-000085a0: 3236 222f 3e3c 773a 737a 4373 2077 3a76  26"/><w:szCs w:v
-000085b0: 616c 3d22 3236 222f 3e3c 2f77 3a72 5072  al="26"/></w:rPr
-000085c0: 3e3c 2f77 3a73 7479 6c65 3e3c 773a 7374  ></w:style><w:st
-000085d0: 796c 6520 773a 7479 7065 3d22 6368 6172  yle w:type="char
-000085e0: 6163 7465 7222 2077 3a63 7573 746f 6d53  acter" w:customS
-000085f0: 7479 6c65 3d22 3122 2077 3a73 7479 6c65  tyle="1" w:style
-00008600: 4964 3d22 4865 6164 696e 6733 4368 6172  Id="Heading3Char
-00008610: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
-00008620: 2248 6561 6469 6e67 2033 2043 6861 7222  "Heading 3 Char"
-00008630: 2f3e 3c77 3a62 6173 6564 4f6e 2077 3a76  /><w:basedOn w:v
-00008640: 616c 3d22 4465 6661 756c 7450 6172 6167  al="DefaultParag
-00008650: 7261 7068 466f 6e74 222f 3e3c 773a 6c69  raphFont"/><w:li
-00008660: 6e6b 2077 3a76 616c 3d22 4865 6164 696e  nk w:val="Headin
-00008670: 6733 222f 3e3c 773a 7569 5072 696f 7269  g3"/><w:uiPriori
-00008680: 7479 2077 3a76 616c 3d22 3922 2f3e 3c77  ty w:val="9"/><w
-00008690: 3a72 7369 6420 773a 7661 6c3d 2230 3039  :rsid w:val="009
-000086a0: 3836 3233 3822 2f3e 3c77 3a72 5072 3e3c  86238"/><w:rPr><
-000086b0: 773a 7246 6f6e 7473 2077 3a61 7363 6969  w:rFonts w:ascii
-000086c0: 5468 656d 653d 226d 616a 6f72 4841 6e73  Theme="majorHAns
-000086d0: 6922 2077 3a65 6173 7441 7369 6154 6865  i" w:eastAsiaThe
-000086e0: 6d65 3d22 6d61 6a6f 7245 6173 7441 7369  me="majorEastAsi
-000086f0: 6122 2077 3a68 416e 7369 5468 656d 653d  a" w:hAnsiTheme=
-00008700: 226d 616a 6f72 4841 6e73 6922 2077 3a63  "majorHAnsi" w:c
-00008710: 7374 6865 6d65 3d22 6d61 6a6f 7242 6964  stheme="majorBid
-00008720: 6922 2f3e 3c77 3a63 6f6c 6f72 2077 3a76  i"/><w:color w:v
-00008730: 616c 3d22 3146 3337 3633 2220 773a 7468  al="1F3763" w:th
-00008740: 656d 6543 6f6c 6f72 3d22 6163 6365 6e74  emeColor="accent
-00008750: 3122 2077 3a74 6865 6d65 5368 6164 653d  1" w:themeShade=
-00008760: 2237 4622 2f3e 3c77 3a73 7a20 773a 7661  "7F"/><w:sz w:va
-00008770: 6c3d 2232 3422 2f3e 3c77 3a73 7a43 7320  l="24"/><w:szCs 
-00008780: 773a 7661 6c3d 2232 3422 2f3e 3c2f 773a  w:val="24"/></w:
-00008790: 7250 723e 3c2f 773a 7374 796c 653e 3c77  rPr></w:style><w
-000087a0: 3a73 7479 6c65 2077 3a74 7970 653d 2263  :style w:type="c
-000087b0: 6861 7261 6374 6572 2220 773a 6375 7374  haracter" w:cust
-000087c0: 6f6d 5374 796c 653d 2231 2220 773a 7374  omStyle="1" w:st
-000087d0: 796c 6549 643d 2248 6561 6469 6e67 3443  yleId="Heading4C
-000087e0: 6861 7222 3e3c 773a 6e61 6d65 2077 3a76  har"><w:name w:v
-000087f0: 616c 3d22 4865 6164 696e 6720 3420 4368  al="Heading 4 Ch
-00008800: 6172 222f 3e3c 773a 6261 7365 644f 6e20  ar"/><w:basedOn 
-00008810: 773a 7661 6c3d 2244 6566 6175 6c74 5061  w:val="DefaultPa
-00008820: 7261 6772 6170 6846 6f6e 7422 2f3e 3c77  ragraphFont"/><w
-00008830: 3a6c 696e 6b20 773a 7661 6c3d 2248 6561  :link w:val="Hea
-00008840: 6469 6e67 3422 2f3e 3c77 3a75 6950 7269  ding4"/><w:uiPri
-00008850: 6f72 6974 7920 773a 7661 6c3d 2239 222f  ority w:val="9"/
-00008860: 3e3c 773a 7273 6964 2077 3a76 616c 3d22  ><w:rsid w:val="
-00008870: 3030 3938 3632 3338 222f 3e3c 773a 7250  00986238"/><w:rP
-00008880: 723e 3c77 3a72 466f 6e74 7320 773a 6173  r><w:rFonts w:as
-00008890: 6369 6954 6865 6d65 3d22 6d61 6a6f 7248  ciiTheme="majorH
-000088a0: 416e 7369 2220 773a 6561 7374 4173 6961  Ansi" w:eastAsia
-000088b0: 5468 656d 653d 226d 616a 6f72 4561 7374  Theme="majorEast
-000088c0: 4173 6961 2220 773a 6841 6e73 6954 6865  Asia" w:hAnsiThe
-000088d0: 6d65 3d22 6d61 6a6f 7248 416e 7369 2220  me="majorHAnsi" 
-000088e0: 773a 6373 7468 656d 653d 226d 616a 6f72  w:cstheme="major
-000088f0: 4269 6469 222f 3e3c 773a 692f 3e3c 773a  Bidi"/><w:i/><w:
-00008900: 6943 732f 3e3c 773a 636f 6c6f 7220 773a  iCs/><w:color w:
-00008910: 7661 6c3d 2232 4635 3439 3622 2077 3a74  val="2F5496" w:t
-00008920: 6865 6d65 436f 6c6f 723d 2261 6363 656e  hemeColor="accen
-00008930: 7431 2220 773a 7468 656d 6553 6861 6465  t1" w:themeShade
-00008940: 3d22 4246 222f 3e3c 2f77 3a72 5072 3e3c  ="BF"/></w:rPr><
-00008950: 2f77 3a73 7479 6c65 3e3c 773a 7374 796c  /w:style><w:styl
-00008960: 6520 773a 7479 7065 3d22 6368 6172 6163  e w:type="charac
-00008970: 7465 7222 2077 3a63 7573 746f 6d53 7479  ter" w:customSty
-00008980: 6c65 3d22 3122 2077 3a73 7479 6c65 4964  le="1" w:styleId
-00008990: 3d22 4865 6164 696e 6735 4368 6172 223e  ="Heading5Char">
-000089a0: 3c77 3a6e 616d 6520 773a 7661 6c3d 2248  <w:name w:val="H
-000089b0: 6561 6469 6e67 2035 2043 6861 7222 2f3e  eading 5 Char"/>
-000089c0: 3c77 3a62 6173 6564 4f6e 2077 3a76 616c  <w:basedOn w:val
-000089d0: 3d22 4465 6661 756c 7450 6172 6167 7261  ="DefaultParagra
-000089e0: 7068 466f 6e74 222f 3e3c 773a 6c69 6e6b  phFont"/><w:link
-000089f0: 2077 3a76 616c 3d22 4865 6164 696e 6735   w:val="Heading5
-00008a00: 222f 3e3c 773a 7569 5072 696f 7269 7479  "/><w:uiPriority
-00008a10: 2077 3a76 616c 3d22 3922 2f3e 3c77 3a72   w:val="9"/><w:r
-00008a20: 7369 6420 773a 7661 6c3d 2230 3039 3836  sid w:val="00986
-00008a30: 3233 3822 2f3e 3c77 3a72 5072 3e3c 773a  238"/><w:rPr><w:
-00008a40: 7246 6f6e 7473 2077 3a61 7363 6969 5468  rFonts w:asciiTh
-00008a50: 656d 653d 226d 616a 6f72 4841 6e73 6922  eme="majorHAnsi"
-00008a60: 2077 3a65 6173 7441 7369 6154 6865 6d65   w:eastAsiaTheme
-00008a70: 3d22 6d61 6a6f 7245 6173 7441 7369 6122  ="majorEastAsia"
-00008a80: 2077 3a68 416e 7369 5468 656d 653d 226d   w:hAnsiTheme="m
-00008a90: 616a 6f72 4841 6e73 6922 2077 3a63 7374  ajorHAnsi" w:cst
-00008aa0: 6865 6d65 3d22 6d61 6a6f 7242 6964 6922  heme="majorBidi"
-00008ab0: 2f3e 3c77 3a63 6f6c 6f72 2077 3a76 616c  /><w:color w:val
-00008ac0: 3d22 3246 3534 3936 2220 773a 7468 656d  ="2F5496" w:them
-00008ad0: 6543 6f6c 6f72 3d22 6163 6365 6e74 3122  eColor="accent1"
-00008ae0: 2077 3a74 6865 6d65 5368 6164 653d 2242   w:themeShade="B
-00008af0: 4622 2f3e 3c2f 773a 7250 723e 3c2f 773a  F"/></w:rPr></w:
-00008b00: 7374 796c 653e 3c77 3a73 7479 6c65 2077  style><w:style w
-00008b10: 3a74 7970 653d 2270 6172 6167 7261 7068  :type="paragraph
-00008b20: 2220 773a 7374 796c 6549 643d 2253 7562  " w:styleId="Sub
-00008b30: 7469 746c 6522 3e3c 773a 6e61 6d65 2077  title"><w:name w
-00008b40: 3a76 616c 3d22 5375 6274 6974 6c65 222f  :val="Subtitle"/
-00008b50: 3e3c 773a 6261 7365 644f 6e20 773a 7661  ><w:basedOn w:va
-00008b60: 6c3d 224e 6f72 6d61 6c22 2f3e 3c77 3a6e  l="Normal"/><w:n
-00008b70: 6578 7420 773a 7661 6c3d 224e 6f72 6d61  ext w:val="Norma
-00008b80: 6c22 2f3e 3c77 3a6c 696e 6b20 773a 7661  l"/><w:link w:va
-00008b90: 6c3d 2253 7562 7469 746c 6543 6861 7222  l="SubtitleChar"
-00008ba0: 2f3e 3c77 3a75 6950 7269 6f72 6974 7920  /><w:uiPriority 
-00008bb0: 773a 7661 6c3d 2231 3122 2f3e 3c77 3a71  w:val="11"/><w:q
-00008bc0: 466f 726d 6174 2f3e 3c77 3a72 7369 6420  Format/><w:rsid 
-00008bd0: 773a 7661 6c3d 2230 3039 3836 3233 3822  w:val="00986238"
-00008be0: 2f3e 3c77 3a70 5072 3e3c 773a 6e75 6d50  /><w:pPr><w:numP
-00008bf0: 723e 3c77 3a69 6c76 6c20 773a 7661 6c3d  r><w:ilvl w:val=
-00008c00: 2231 222f 3e3c 2f77 3a6e 756d 5072 3e3c  "1"/></w:numPr><
-00008c10: 2f77 3a70 5072 3e3c 773a 7250 723e 3c77  /w:pPr><w:rPr><w
-00008c20: 3a72 466f 6e74 7320 773a 6561 7374 4173  :rFonts w:eastAs
-00008c30: 6961 5468 656d 653d 226d 696e 6f72 4561  iaTheme="minorEa
-00008c40: 7374 4173 6961 222f 3e3c 773a 636f 6c6f  stAsia"/><w:colo
-00008c50: 7220 773a 7661 6c3d 2235 4135 4135 4122  r w:val="5A5A5A"
-00008c60: 2077 3a74 6865 6d65 436f 6c6f 723d 2274   w:themeColor="t
-00008c70: 6578 7431 2220 773a 7468 656d 6554 696e  ext1" w:themeTin
-00008c80: 743d 2241 3522 2f3e 3c77 3a73 7061 6369  t="A5"/><w:spaci
-00008c90: 6e67 2077 3a76 616c 3d22 3135 222f 3e3c  ng w:val="15"/><
-00008ca0: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
-00008cb0: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
-00008cc0: 3d22 6368 6172 6163 7465 7222 2077 3a63  ="character" w:c
-00008cd0: 7573 746f 6d53 7479 6c65 3d22 3122 2077  ustomStyle="1" w
-00008ce0: 3a73 7479 6c65 4964 3d22 5375 6274 6974  :styleId="Subtit
-00008cf0: 6c65 4368 6172 223e 3c77 3a6e 616d 6520  leChar"><w:name 
-00008d00: 773a 7661 6c3d 2253 7562 7469 746c 6520  w:val="Subtitle 
-00008d10: 4368 6172 222f 3e3c 773a 6261 7365 644f  Char"/><w:basedO
-00008d20: 6e20 773a 7661 6c3d 2244 6566 6175 6c74  n w:val="Default
-00008d30: 5061 7261 6772 6170 6846 6f6e 7422 2f3e  ParagraphFont"/>
-00008d40: 3c77 3a6c 696e 6b20 773a 7661 6c3d 2253  <w:link w:val="S
-00008d50: 7562 7469 746c 6522 2f3e 3c77 3a75 6950  ubtitle"/><w:uiP
-00008d60: 7269 6f72 6974 7920 773a 7661 6c3d 2231  riority w:val="1
-00008d70: 3122 2f3e 3c77 3a72 7369 6420 773a 7661  1"/><w:rsid w:va
-00008d80: 6c3d 2230 3039 3836 3233 3822 2f3e 3c77  l="00986238"/><w
-00008d90: 3a72 5072 3e3c 773a 7246 6f6e 7473 2077  :rPr><w:rFonts w
-00008da0: 3a65 6173 7441 7369 6154 6865 6d65 3d22  :eastAsiaTheme="
-00008db0: 6d69 6e6f 7245 6173 7441 7369 6122 2f3e  minorEastAsia"/>
-00008dc0: 3c77 3a63 6f6c 6f72 2077 3a76 616c 3d22  <w:color w:val="
-00008dd0: 3541 3541 3541 2220 773a 7468 656d 6543  5A5A5A" w:themeC
-00008de0: 6f6c 6f72 3d22 7465 7874 3122 2077 3a74  olor="text1" w:t
-00008df0: 6865 6d65 5469 6e74 3d22 4135 222f 3e3c  hemeTint="A5"/><
-00008e00: 773a 7370 6163 696e 6720 773a 7661 6c3d  w:spacing w:val=
-00008e10: 2231 3522 2f3e 3c2f 773a 7250 723e 3c2f  "15"/></w:rPr></
-00008e20: 773a 7374 796c 653e 3c77 3a73 7479 6c65  w:style><w:style
-00008e30: 2077 3a74 7970 653d 2263 6861 7261 6374   w:type="charact
-00008e40: 6572 2220 773a 7374 796c 6549 643d 2253  er" w:styleId="S
-00008e50: 7562 746c 6545 6d70 6861 7369 7322 3e3c  ubtleEmphasis"><
-00008e60: 773a 6e61 6d65 2077 3a76 616c 3d22 5375  w:name w:val="Su
-00008e70: 6274 6c65 2045 6d70 6861 7369 7322 2f3e  btle Emphasis"/>
-00008e80: 3c77 3a62 6173 6564 4f6e 2077 3a76 616c  <w:basedOn w:val
-00008e90: 3d22 4465 6661 756c 7450 6172 6167 7261  ="DefaultParagra
-00008ea0: 7068 466f 6e74 222f 3e3c 773a 7569 5072  phFont"/><w:uiPr
-00008eb0: 696f 7269 7479 2077 3a76 616c 3d22 3139  iority w:val="19
-00008ec0: 222f 3e3c 773a 7146 6f72 6d61 742f 3e3c  "/><w:qFormat/><
-00008ed0: 773a 7273 6964 2077 3a76 616c 3d22 3030  w:rsid w:val="00
-00008ee0: 3938 3632 3338 222f 3e3c 773a 7250 723e  986238"/><w:rPr>
-00008ef0: 3c77 3a69 2f3e 3c77 3a69 4373 2f3e 3c77  <w:i/><w:iCs/><w
-00008f00: 3a63 6f6c 6f72 2077 3a76 616c 3d22 3430  :color w:val="40
-00008f10: 3430 3430 2220 773a 7468 656d 6543 6f6c  4040" w:themeCol
-00008f20: 6f72 3d22 7465 7874 3122 2077 3a74 6865  or="text1" w:the
-00008f30: 6d65 5469 6e74 3d22 4246 222f 3e3c 2f77  meTint="BF"/></w
-00008f40: 3a72 5072 3e3c 2f77 3a73 7479 6c65 3e3c  :rPr></w:style><
-00008f50: 773a 7374 796c 6520 773a 7479 7065 3d22  w:style w:type="
-00008f60: 6368 6172 6163 7465 7222 2077 3a73 7479  character" w:sty
-00008f70: 6c65 4964 3d22 456d 7068 6173 6973 223e  leId="Emphasis">
-00008f80: 3c77 3a6e 616d 6520 773a 7661 6c3d 2245  <w:name w:val="E
-00008f90: 6d70 6861 7369 7322 2f3e 3c77 3a62 6173  mphasis"/><w:bas
-00008fa0: 6564 4f6e 2077 3a76 616c 3d22 4465 6661  edOn w:val="Defa
-00008fb0: 756c 7450 6172 6167 7261 7068 466f 6e74  ultParagraphFont
-00008fc0: 222f 3e3c 773a 7569 5072 696f 7269 7479  "/><w:uiPriority
-00008fd0: 2077 3a76 616c 3d22 3230 222f 3e3c 773a   w:val="20"/><w:
-00008fe0: 7146 6f72 6d61 742f 3e3c 773a 7273 6964  qFormat/><w:rsid
-00008ff0: 2077 3a76 616c 3d22 3030 3938 3632 3338   w:val="00986238
-00009000: 222f 3e3c 773a 7250 723e 3c77 3a69 2f3e  "/><w:rPr><w:i/>
-00009010: 3c77 3a69 4373 2f3e 3c2f 773a 7250 723e  <w:iCs/></w:rPr>
-00009020: 3c2f 773a 7374 796c 653e 3c77 3a73 7479  </w:style><w:sty
-00009030: 6c65 2077 3a74 7970 653d 2263 6861 7261  le w:type="chara
-00009040: 6374 6572 2220 773a 7374 796c 6549 643d  cter" w:styleId=
-00009050: 2249 6e74 656e 7365 456d 7068 6173 6973  "IntenseEmphasis
-00009060: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
-00009070: 2249 6e74 656e 7365 2045 6d70 6861 7369  "Intense Emphasi
-00009080: 7322 2f3e 3c77 3a62 6173 6564 4f6e 2077  s"/><w:basedOn w
-00009090: 3a76 616c 3d22 4465 6661 756c 7450 6172  :val="DefaultPar
-000090a0: 6167 7261 7068 466f 6e74 222f 3e3c 773a  agraphFont"/><w:
-000090b0: 7569 5072 696f 7269 7479 2077 3a76 616c  uiPriority w:val
-000090c0: 3d22 3231 222f 3e3c 773a 7146 6f72 6d61  ="21"/><w:qForma
-000090d0: 742f 3e3c 773a 7273 6964 2077 3a76 616c  t/><w:rsid w:val
-000090e0: 3d22 3030 3938 3632 3338 222f 3e3c 773a  ="00986238"/><w:
-000090f0: 7250 723e 3c77 3a69 2f3e 3c77 3a69 4373  rPr><w:i/><w:iCs
-00009100: 2f3e 3c77 3a63 6f6c 6f72 2077 3a76 616c  /><w:color w:val
-00009110: 3d22 3434 3732 4334 2220 773a 7468 656d  ="4472C4" w:them
-00009120: 6543 6f6c 6f72 3d22 6163 6365 6e74 3122  eColor="accent1"
-00009130: 2f3e 3c2f 773a 7250 723e 3c2f 773a 7374  /></w:rPr></w:st
-00009140: 796c 653e 3c77 3a73 7479 6c65 2077 3a74  yle><w:style w:t
-00009150: 7970 653d 2263 6861 7261 6374 6572 2220  ype="character" 
-00009160: 773a 7374 796c 6549 643d 2253 7472 6f6e  w:styleId="Stron
-00009170: 6722 3e3c 773a 6e61 6d65 2077 3a76 616c  g"><w:name w:val
-00009180: 3d22 5374 726f 6e67 222f 3e3c 773a 6261  ="Strong"/><w:ba
-00009190: 7365 644f 6e20 773a 7661 6c3d 2244 6566  sedOn w:val="Def
-000091a0: 6175 6c74 5061 7261 6772 6170 6846 6f6e  aultParagraphFon
-000091b0: 7422 2f3e 3c77 3a75 6950 7269 6f72 6974  t"/><w:uiPriorit
-000091c0: 7920 773a 7661 6c3d 2232 3222 2f3e 3c77  y w:val="22"/><w
-000091d0: 3a71 466f 726d 6174 2f3e 3c77 3a72 7369  :qFormat/><w:rsi
-000091e0: 6420 773a 7661 6c3d 2230 3039 3836 3233  d w:val="0098623
-000091f0: 3822 2f3e 3c77 3a72 5072 3e3c 773a 622f  8"/><w:rPr><w:b/
-00009200: 3e3c 773a 6243 732f 3e3c 2f77 3a72 5072  ><w:bCs/></w:rPr
-00009210: 3e3c 2f77 3a73 7479 6c65 3e3c 773a 7374  ></w:style><w:st
-00009220: 796c 6520 773a 7479 7065 3d22 7061 7261  yle w:type="para
-00009230: 6772 6170 6822 2077 3a73 7479 6c65 4964  graph" w:styleId
-00009240: 3d22 5175 6f74 6522 3e3c 773a 6e61 6d65  ="Quote"><w:name
-00009250: 2077 3a76 616c 3d22 5175 6f74 6522 2f3e   w:val="Quote"/>
-00009260: 3c77 3a62 6173 6564 4f6e 2077 3a76 616c  <w:basedOn w:val
-00009270: 3d22 4e6f 726d 616c 222f 3e3c 773a 6e65  ="Normal"/><w:ne
-00009280: 7874 2077 3a76 616c 3d22 4e6f 726d 616c  xt w:val="Normal
-00009290: 222f 3e3c 773a 6c69 6e6b 2077 3a76 616c  "/><w:link w:val
-000092a0: 3d22 5175 6f74 6543 6861 7222 2f3e 3c77  ="QuoteChar"/><w
-000092b0: 3a75 6950 7269 6f72 6974 7920 773a 7661  :uiPriority w:va
-000092c0: 6c3d 2232 3922 2f3e 3c77 3a71 466f 726d  l="29"/><w:qForm
-000092d0: 6174 2f3e 3c77 3a72 7369 6420 773a 7661  at/><w:rsid w:va
-000092e0: 6c3d 2230 3039 3836 3233 3822 2f3e 3c77  l="00986238"/><w
-000092f0: 3a70 5072 3e3c 773a 7370 6163 696e 6720  :pPr><w:spacing 
-00009300: 773a 6265 666f 7265 3d22 3230 3022 2f3e  w:before="200"/>
-00009310: 3c77 3a69 6e64 2077 3a6c 6566 743d 2238  <w:ind w:left="8
-00009320: 3634 2220 773a 7269 6768 743d 2238 3634  64" w:right="864
-00009330: 222f 3e3c 773a 6a63 2077 3a76 616c 3d22  "/><w:jc w:val="
-00009340: 6365 6e74 6572 222f 3e3c 2f77 3a70 5072  center"/></w:pPr
-00009350: 3e3c 773a 7250 723e 3c77 3a69 2f3e 3c77  ><w:rPr><w:i/><w
-00009360: 3a69 4373 2f3e 3c77 3a63 6f6c 6f72 2077  :iCs/><w:color w
-00009370: 3a76 616c 3d22 3430 3430 3430 2220 773a  :val="404040" w:
-00009380: 7468 656d 6543 6f6c 6f72 3d22 7465 7874  themeColor="text
-00009390: 3122 2077 3a74 6865 6d65 5469 6e74 3d22  1" w:themeTint="
-000093a0: 4246 222f 3e3c 2f77 3a72 5072 3e3c 2f77  BF"/></w:rPr></w
-000093b0: 3a73 7479 6c65 3e3c 773a 7374 796c 6520  :style><w:style 
-000093c0: 773a 7479 7065 3d22 6368 6172 6163 7465  w:type="characte
-000093d0: 7222 2077 3a63 7573 746f 6d53 7479 6c65  r" w:customStyle
-000093e0: 3d22 3122 2077 3a73 7479 6c65 4964 3d22  ="1" w:styleId="
-000093f0: 5175 6f74 6543 6861 7222 3e3c 773a 6e61  QuoteChar"><w:na
-00009400: 6d65 2077 3a76 616c 3d22 5175 6f74 6520  me w:val="Quote 
-00009410: 4368 6172 222f 3e3c 773a 6261 7365 644f  Char"/><w:basedO
-00009420: 6e20 773a 7661 6c3d 2244 6566 6175 6c74  n w:val="Default
-00009430: 5061 7261 6772 6170 6846 6f6e 7422 2f3e  ParagraphFont"/>
-00009440: 3c77 3a6c 696e 6b20 773a 7661 6c3d 2251  <w:link w:val="Q
-00009450: 756f 7465 222f 3e3c 773a 7569 5072 696f  uote"/><w:uiPrio
-00009460: 7269 7479 2077 3a76 616c 3d22 3239 222f  rity w:val="29"/
-00009470: 3e3c 773a 7273 6964 2077 3a76 616c 3d22  ><w:rsid w:val="
-00009480: 3030 3938 3632 3338 222f 3e3c 773a 7250  00986238"/><w:rP
-00009490: 723e 3c77 3a69 2f3e 3c77 3a69 4373 2f3e  r><w:i/><w:iCs/>
-000094a0: 3c77 3a63 6f6c 6f72 2077 3a76 616c 3d22  <w:color w:val="
-000094b0: 3430 3430 3430 2220 773a 7468 656d 6543  404040" w:themeC
-000094c0: 6f6c 6f72 3d22 7465 7874 3122 2077 3a74  olor="text1" w:t
-000094d0: 6865 6d65 5469 6e74 3d22 4246 222f 3e3c  hemeTint="BF"/><
-000094e0: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
-000094f0: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
-00009500: 3d22 7061 7261 6772 6170 6822 2077 3a73  ="paragraph" w:s
-00009510: 7479 6c65 4964 3d22 496e 7465 6e73 6551  tyleId="IntenseQ
-00009520: 756f 7465 223e 3c77 3a6e 616d 6520 773a  uote"><w:name w:
-00009530: 7661 6c3d 2249 6e74 656e 7365 2051 756f  val="Intense Quo
-00009540: 7465 222f 3e3c 773a 6261 7365 644f 6e20  te"/><w:basedOn 
-00009550: 773a 7661 6c3d 224e 6f72 6d61 6c22 2f3e  w:val="Normal"/>
-00009560: 3c77 3a6e 6578 7420 773a 7661 6c3d 224e  <w:next w:val="N
-00009570: 6f72 6d61 6c22 2f3e 3c77 3a6c 696e 6b20  ormal"/><w:link 
-00009580: 773a 7661 6c3d 2249 6e74 656e 7365 5175  w:val="IntenseQu
-00009590: 6f74 6543 6861 7222 2f3e 3c77 3a75 6950  oteChar"/><w:uiP
-000095a0: 7269 6f72 6974 7920 773a 7661 6c3d 2233  riority w:val="3
-000095b0: 3022 2f3e 3c77 3a71 466f 726d 6174 2f3e  0"/><w:qFormat/>
-000095c0: 3c77 3a72 7369 6420 773a 7661 6c3d 2230  <w:rsid w:val="0
-000095d0: 3039 4536 3633 4522 2f3e 3c77 3a70 5072  09E663E"/><w:pPr
-000095e0: 3e3c 773a 7042 6472 3e3c 773a 746f 7020  ><w:pBdr><w:top 
-000095f0: 773a 7661 6c3d 2273 696e 676c 6522 2077  w:val="single" w
-00009600: 3a73 7a3d 2234 2220 773a 7370 6163 653d  :sz="4" w:space=
-00009610: 2231 3022 2077 3a63 6f6c 6f72 3d22 3434  "10" w:color="44
-00009620: 3732 4334 2220 773a 7468 656d 6543 6f6c  72C4" w:themeCol
-00009630: 6f72 3d22 6163 6365 6e74 3122 2f3e 3c77  or="accent1"/><w
-00009640: 3a62 6f74 746f 6d20 773a 7661 6c3d 2273  :bottom w:val="s
-00009650: 696e 676c 6522 2077 3a73 7a3d 2234 2220  ingle" w:sz="4" 
-00009660: 773a 7370 6163 653d 2231 3022 2077 3a63  w:space="10" w:c
-00009670: 6f6c 6f72 3d22 3434 3732 4334 2220 773a  olor="4472C4" w:
-00009680: 7468 656d 6543 6f6c 6f72 3d22 6163 6365  themeColor="acce
-00009690: 6e74 3122 2f3e 3c2f 773a 7042 6472 3e3c  nt1"/></w:pBdr><
-000096a0: 773a 7370 6163 696e 6720 773a 6265 666f  w:spacing w:befo
-000096b0: 7265 3d22 3336 3022 2077 3a61 6674 6572  re="360" w:after
-000096c0: 3d22 3336 3022 2f3e 3c77 3a69 6e64 2077  ="360"/><w:ind w
-000096d0: 3a6c 6566 743d 2238 3634 2220 773a 7269  :left="864" w:ri
-000096e0: 6768 743d 2238 3634 222f 3e3c 773a 6a63  ght="864"/><w:jc
-000096f0: 2077 3a76 616c 3d22 6365 6e74 6572 222f   w:val="center"/
-00009700: 3e3c 2f77 3a70 5072 3e3c 773a 7250 723e  ></w:pPr><w:rPr>
-00009710: 3c77 3a69 2f3e 3c77 3a69 4373 2f3e 3c77  <w:i/><w:iCs/><w
-00009720: 3a63 6f6c 6f72 2077 3a76 616c 3d22 3434  :color w:val="44
-00009730: 3732 4334 2220 773a 7468 656d 6543 6f6c  72C4" w:themeCol
-00009740: 6f72 3d22 6163 6365 6e74 3122 2f3e 3c2f  or="accent1"/></
-00009750: 773a 7250 723e 3c2f 773a 7374 796c 653e  w:rPr></w:style>
-00009760: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
-00009770: 2263 6861 7261 6374 6572 2220 773a 6375  "character" w:cu
-00009780: 7374 6f6d 5374 796c 653d 2231 2220 773a  stomStyle="1" w:
-00009790: 7374 796c 6549 643d 2249 6e74 656e 7365  styleId="Intense
-000097a0: 5175 6f74 6543 6861 7222 3e3c 773a 6e61  QuoteChar"><w:na
-000097b0: 6d65 2077 3a76 616c 3d22 496e 7465 6e73  me w:val="Intens
-000097c0: 6520 5175 6f74 6520 4368 6172 222f 3e3c  e Quote Char"/><
-000097d0: 773a 6261 7365 644f 6e20 773a 7661 6c3d  w:basedOn w:val=
-000097e0: 2244 6566 6175 6c74 5061 7261 6772 6170  "DefaultParagrap
-000097f0: 6846 6f6e 7422 2f3e 3c77 3a6c 696e 6b20  hFont"/><w:link 
-00009800: 773a 7661 6c3d 2249 6e74 656e 7365 5175  w:val="IntenseQu
-00009810: 6f74 6522 2f3e 3c77 3a75 6950 7269 6f72  ote"/><w:uiPrior
-00009820: 6974 7920 773a 7661 6c3d 2233 3022 2f3e  ity w:val="30"/>
-00009830: 3c77 3a72 7369 6420 773a 7661 6c3d 2230  <w:rsid w:val="0
-00009840: 3039 4536 3633 4522 2f3e 3c77 3a72 5072  09E663E"/><w:rPr
-00009850: 3e3c 773a 692f 3e3c 773a 6943 732f 3e3c  ><w:i/><w:iCs/><
-00009860: 773a 636f 6c6f 7220 773a 7661 6c3d 2234  w:color w:val="4
-00009870: 3437 3243 3422 2077 3a74 6865 6d65 436f  472C4" w:themeCo
-00009880: 6c6f 723d 2261 6363 656e 7431 222f 3e3c  lor="accent1"/><
-00009890: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
-000098a0: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
-000098b0: 3d22 6368 6172 6163 7465 7222 2077 3a73  ="character" w:s
-000098c0: 7479 6c65 4964 3d22 5375 6274 6c65 5265  tyleId="SubtleRe
-000098d0: 6665 7265 6e63 6522 3e3c 773a 6e61 6d65  ference"><w:name
-000098e0: 2077 3a76 616c 3d22 5375 6274 6c65 2052   w:val="Subtle R
-000098f0: 6566 6572 656e 6365 222f 3e3c 773a 6261  eference"/><w:ba
-00009900: 7365 644f 6e20 773a 7661 6c3d 2244 6566  sedOn w:val="Def
-00009910: 6175 6c74 5061 7261 6772 6170 6846 6f6e  aultParagraphFon
-00009920: 7422 2f3e 3c77 3a75 6950 7269 6f72 6974  t"/><w:uiPriorit
-00009930: 7920 773a 7661 6c3d 2233 3122 2f3e 3c77  y w:val="31"/><w
-00009940: 3a71 466f 726d 6174 2f3e 3c77 3a72 7369  :qFormat/><w:rsi
-00009950: 6420 773a 7661 6c3d 2230 3039 4536 3633  d w:val="009E663
-00009960: 4522 2f3e 3c77 3a72 5072 3e3c 773a 736d  E"/><w:rPr><w:sm
-00009970: 616c 6c43 6170 732f 3e3c 773a 636f 6c6f  allCaps/><w:colo
-00009980: 7220 773a 7661 6c3d 2235 4135 4135 4122  r w:val="5A5A5A"
-00009990: 2077 3a74 6865 6d65 436f 6c6f 723d 2274   w:themeColor="t
-000099a0: 6578 7431 2220 773a 7468 656d 6554 696e  ext1" w:themeTin
-000099b0: 743d 2241 3522 2f3e 3c2f 773a 7250 723e  t="A5"/></w:rPr>
-000099c0: 3c2f 773a 7374 796c 653e 3c77 3a73 7479  </w:style><w:sty
-000099d0: 6c65 2077 3a74 7970 653d 2263 6861 7261  le w:type="chara
-000099e0: 6374 6572 2220 773a 7374 796c 6549 643d  cter" w:styleId=
-000099f0: 2249 6e74 656e 7365 5265 6665 7265 6e63  "IntenseReferenc
-00009a00: 6522 3e3c 773a 6e61 6d65 2077 3a76 616c  e"><w:name w:val
-00009a10: 3d22 496e 7465 6e73 6520 5265 6665 7265  ="Intense Refere
-00009a20: 6e63 6522 2f3e 3c77 3a62 6173 6564 4f6e  nce"/><w:basedOn
-00009a30: 2077 3a76 616c 3d22 4465 6661 756c 7450   w:val="DefaultP
-00009a40: 6172 6167 7261 7068 466f 6e74 222f 3e3c  aragraphFont"/><
-00009a50: 773a 7569 5072 696f 7269 7479 2077 3a76  w:uiPriority w:v
-00009a60: 616c 3d22 3332 222f 3e3c 773a 7146 6f72  al="32"/><w:qFor
-00009a70: 6d61 742f 3e3c 773a 7273 6964 2077 3a76  mat/><w:rsid w:v
-00009a80: 616c 3d22 3030 3945 3636 3345 222f 3e3c  al="009E663E"/><
-00009a90: 773a 7250 723e 3c77 3a62 2f3e 3c77 3a62  w:rPr><w:b/><w:b
-00009aa0: 4373 2f3e 3c77 3a73 6d61 6c6c 4361 7073  Cs/><w:smallCaps
-00009ab0: 2f3e 3c77 3a63 6f6c 6f72 2077 3a76 616c  /><w:color w:val
-00009ac0: 3d22 3434 3732 4334 2220 773a 7468 656d  ="4472C4" w:them
-00009ad0: 6543 6f6c 6f72 3d22 6163 6365 6e74 3122  eColor="accent1"
-00009ae0: 2f3e 3c77 3a73 7061 6369 6e67 2077 3a76  /><w:spacing w:v
-00009af0: 616c 3d22 3522 2f3e 3c2f 773a 7250 723e  al="5"/></w:rPr>
-00009b00: 3c2f 773a 7374 796c 653e 3c77 3a73 7479  </w:style><w:sty
-00009b10: 6c65 2077 3a74 7970 653d 2263 6861 7261  le w:type="chara
-00009b20: 6374 6572 2220 773a 7374 796c 6549 643d  cter" w:styleId=
-00009b30: 2242 6f6f 6b54 6974 6c65 223e 3c77 3a6e  "BookTitle"><w:n
-00009b40: 616d 6520 773a 7661 6c3d 2242 6f6f 6b20  ame w:val="Book 
-00009b50: 5469 746c 6522 2f3e 3c77 3a62 6173 6564  Title"/><w:based
-00009b60: 4f6e 2077 3a76 616c 3d22 4465 6661 756c  On w:val="Defaul
-00009b70: 7450 6172 6167 7261 7068 466f 6e74 222f  tParagraphFont"/
-00009b80: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
-00009b90: 3a76 616c 3d22 3333 222f 3e3c 773a 7146  :val="33"/><w:qF
-00009ba0: 6f72 6d61 742f 3e3c 773a 7273 6964 2077  ormat/><w:rsid w
-00009bb0: 3a76 616c 3d22 3030 3945 3636 3345 222f  :val="009E663E"/
-00009bc0: 3e3c 773a 7250 723e 3c77 3a62 2f3e 3c77  ><w:rPr><w:b/><w
-00009bd0: 3a62 4373 2f3e 3c77 3a69 2f3e 3c77 3a69  :bCs/><w:i/><w:i
-00009be0: 4373 2f3e 3c77 3a73 7061 6369 6e67 2077  Cs/><w:spacing w
-00009bf0: 3a76 616c 3d22 3522 2f3e 3c2f 773a 7250  :val="5"/></w:rP
-00009c00: 723e 3c2f 773a 7374 796c 653e 3c77 3a73  r></w:style><w:s
-00009c10: 7479 6c65 2077 3a74 7970 653d 2270 6172  tyle w:type="par
-00009c20: 6167 7261 7068 2220 773a 7374 796c 6549  agraph" w:styleI
-00009c30: 643d 224c 6973 7450 6172 6167 7261 7068  d="ListParagraph
-00009c40: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
-00009c50: 224c 6973 7420 5061 7261 6772 6170 6822  "List Paragraph"
-00009c60: 2f3e 3c77 3a62 6173 6564 4f6e 2077 3a76  /><w:basedOn w:v
-00009c70: 616c 3d22 4e6f 726d 616c 222f 3e3c 773a  al="Normal"/><w:
-00009c80: 7569 5072 696f 7269 7479 2077 3a76 616c  uiPriority w:val
-00009c90: 3d22 3334 222f 3e3c 773a 7146 6f72 6d61  ="34"/><w:qForma
-00009ca0: 742f 3e3c 773a 7273 6964 2077 3a76 616c  t/><w:rsid w:val
-00009cb0: 3d22 3030 3945 3636 3345 222f 3e3c 773a  ="009E663E"/><w:
-00009cc0: 7050 723e 3c77 3a69 6e64 2077 3a6c 6566  pPr><w:ind w:lef
-00009cd0: 743d 2237 3230 222f 3e3c 773a 636f 6e74  t="720"/><w:cont
-00009ce0: 6578 7475 616c 5370 6163 696e 672f 3e3c  extualSpacing/><
-00009cf0: 2f77 3a70 5072 3e3c 2f77 3a73 7479 6c65  /w:pPr></w:style
-00009d00: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
-00009d10: 3d22 7061 7261 6772 6170 6822 2077 3a73  ="paragraph" w:s
-00009d20: 7479 6c65 4964 3d22 4e6f 5370 6163 696e  tyleId="NoSpacin
-00009d30: 6722 3e3c 773a 6e61 6d65 2077 3a76 616c  g"><w:name w:val
-00009d40: 3d22 4e6f 2053 7061 6369 6e67 222f 3e3c  ="No Spacing"/><
-00009d50: 773a 7569 5072 696f 7269 7479 2077 3a76  w:uiPriority w:v
-00009d60: 616c 3d22 3122 2f3e 3c77 3a71 466f 726d  al="1"/><w:qForm
-00009d70: 6174 2f3e 3c77 3a72 7369 6420 773a 7661  at/><w:rsid w:va
-00009d80: 6c3d 2230 3039 4536 3633 4522 2f3e 3c77  l="009E663E"/><w
-00009d90: 3a70 5072 3e3c 773a 7370 6163 696e 6720  :pPr><w:spacing 
-00009da0: 773a 6166 7465 723d 2230 2220 773a 6c69  w:after="0" w:li
-00009db0: 6e65 3d22 3234 3022 2077 3a6c 696e 6552  ne="240" w:lineR
-00009dc0: 756c 653d 2261 7574 6f22 2f3e 3c2f 773a  ule="auto"/></w:
-00009dd0: 7050 723e 3c2f 773a 7374 796c 653e 3c77  pPr></w:style><w
-00009de0: 3a73 7479 6c65 2077 3a74 7970 653d 2270  :style w:type="p
-00009df0: 6172 6167 7261 7068 2220 773a 7374 796c  aragraph" w:styl
-00009e00: 6549 643d 224c 6973 744e 756d 6265 7222  eId="ListNumber"
-00009e10: 3e3c 773a 6e61 6d65 2077 3a76 616c 3d22  ><w:name w:val="
-00009e20: 4c69 7374 204e 756d 6265 7222 2f3e 3c77  List Number"/><w
-00009e30: 3a62 6173 6564 4f6e 2077 3a76 616c 3d22  :basedOn w:val="
-00009e40: 4e6f 726d 616c 222f 3e3c 773a 7569 5072  Normal"/><w:uiPr
-00009e50: 696f 7269 7479 2077 3a76 616c 3d22 3939  iority w:val="99
-00009e60: 222f 3e3c 773a 756e 6869 6465 5768 656e  "/><w:unhideWhen
-00009e70: 5573 6564 2f3e 3c77 3a72 7369 6420 773a  Used/><w:rsid w:
-00009e80: 7661 6c3d 2230 3044 3732 3535 4122 2f3e  val="00D7255A"/>
-00009e90: 3c77 3a70 5072 3e3c 773a 6e75 6d50 723e  <w:pPr><w:numPr>
-00009ea0: 3c77 3a6e 756d 4964 2077 3a76 616c 3d22  <w:numId w:val="
-00009eb0: 3922 2f3e 3c2f 773a 6e75 6d50 723e 3c77  9"/></w:numPr><w
-00009ec0: 3a63 6f6e 7465 7874 7561 6c53 7061 6369  :contextualSpaci
-00009ed0: 6e67 2f3e 3c2f 773a 7050 723e 3c2f 773a  ng/></w:pPr></w:
-00009ee0: 7374 796c 653e 3c77 3a73 7479 6c65 2077  style><w:style w
-00009ef0: 3a74 7970 653d 2270 6172 6167 7261 7068  :type="paragraph
-00009f00: 2220 773a 7374 796c 6549 643d 224c 6973  " w:styleId="Lis
-00009f10: 7442 756c 6c65 7422 3e3c 773a 6e61 6d65  tBullet"><w:name
-00009f20: 2077 3a76 616c 3d22 4c69 7374 2042 756c   w:val="List Bul
-00009f30: 6c65 7422 2f3e 3c77 3a62 6173 6564 4f6e  let"/><w:basedOn
-00009f40: 2077 3a76 616c 3d22 4e6f 726d 616c 222f   w:val="Normal"/
-00009f50: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
-00009f60: 3a76 616c 3d22 3939 222f 3e3c 773a 756e  :val="99"/><w:un
-00009f70: 6869 6465 5768 656e 5573 6564 2f3e 3c77  hideWhenUsed/><w
-00009f80: 3a71 466f 726d 6174 2f3e 3c77 3a72 7369  :qFormat/><w:rsi
-00009f90: 6420 773a 7661 6c3d 2230 3037 4534 4334  d w:val="007E4C4
-00009fa0: 3922 2f3e 3c77 3a70 5072 3e3c 773a 6e75  9"/><w:pPr><w:nu
-00009fb0: 6d50 723e 3c77 3a6e 756d 4964 2077 3a76  mPr><w:numId w:v
-00009fc0: 616c 3d22 3322 2f3e 3c2f 773a 6e75 6d50  al="3"/></w:numP
-00009fd0: 723e 3c77 3a63 6f6e 7465 7874 7561 6c53  r><w:contextualS
-00009fe0: 7061 6369 6e67 2f3e 3c2f 773a 7050 723e  pacing/></w:pPr>
-00009ff0: 3c2f 773a 7374 796c 653e 3c77 3a73 7479  </w:style><w:sty
-0000a000: 6c65 2077 3a74 7970 653d 2270 6172 6167  le w:type="parag
-0000a010: 7261 7068 2220 773a 7374 796c 6549 643d  raph" w:styleId=
-0000a020: 224d 6163 726f 5465 7874 223e 3c77 3a6e  "MacroText"><w:n
-0000a030: 616d 6520 773a 7661 6c3d 226d 6163 726f  ame w:val="macro
-0000a040: 222f 3e3c 773a 6c69 6e6b 2077 3a76 616c  "/><w:link w:val
-0000a050: 3d22 4d61 6372 6f54 6578 7443 6861 7222  ="MacroTextChar"
-0000a060: 2f3e 3c77 3a75 6950 7269 6f72 6974 7920  /><w:uiPriority 
-0000a070: 773a 7661 6c3d 2239 3922 2f3e 3c77 3a75  w:val="99"/><w:u
-0000a080: 6e68 6964 6557 6865 6e55 7365 642f 3e3c  nhideWhenUsed/><
-0000a090: 773a 7273 6964 2077 3a76 616c 3d22 3030  w:rsid w:val="00
-0000a0a0: 4437 3235 3541 222f 3e3c 773a 7050 723e  D7255A"/><w:pPr>
-0000a0b0: 3c77 3a74 6162 733e 3c77 3a74 6162 2077  <w:tabs><w:tab w
-0000a0c0: 3a76 616c 3d22 6c65 6674 2220 773a 706f  :val="left" w:po
-0000a0d0: 733d 2234 3830 222f 3e3c 773a 7461 6220  s="480"/><w:tab 
-0000a0e0: 773a 7661 6c3d 226c 6566 7422 2077 3a70  w:val="left" w:p
-0000a0f0: 6f73 3d22 3936 3022 2f3e 3c77 3a74 6162  os="960"/><w:tab
-0000a100: 2077 3a76 616c 3d22 6c65 6674 2220 773a   w:val="left" w:
-0000a110: 706f 733d 2231 3434 3022 2f3e 3c77 3a74  pos="1440"/><w:t
-0000a120: 6162 2077 3a76 616c 3d22 6c65 6674 2220  ab w:val="left" 
-0000a130: 773a 706f 733d 2231 3932 3022 2f3e 3c77  w:pos="1920"/><w
-0000a140: 3a74 6162 2077 3a76 616c 3d22 6c65 6674  :tab w:val="left
-0000a150: 2220 773a 706f 733d 2232 3430 3022 2f3e  " w:pos="2400"/>
-0000a160: 3c77 3a74 6162 2077 3a76 616c 3d22 6c65  <w:tab w:val="le
-0000a170: 6674 2220 773a 706f 733d 2232 3838 3022  ft" w:pos="2880"
-0000a180: 2f3e 3c77 3a74 6162 2077 3a76 616c 3d22  /><w:tab w:val="
-0000a190: 6c65 6674 2220 773a 706f 733d 2233 3336  left" w:pos="336
-0000a1a0: 3022 2f3e 3c77 3a74 6162 2077 3a76 616c  0"/><w:tab w:val
-0000a1b0: 3d22 6c65 6674 2220 773a 706f 733d 2233  ="left" w:pos="3
-0000a1c0: 3834 3022 2f3e 3c77 3a74 6162 2077 3a76  840"/><w:tab w:v
-0000a1d0: 616c 3d22 6c65 6674 2220 773a 706f 733d  al="left" w:pos=
-0000a1e0: 2234 3332 3022 2f3e 3c2f 773a 7461 6273  "4320"/></w:tabs
-0000a1f0: 3e3c 773a 7370 6163 696e 6720 773a 6166  ><w:spacing w:af
-0000a200: 7465 723d 2230 222f 3e3c 2f77 3a70 5072  ter="0"/></w:pPr
-0000a210: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
-0000a220: 7320 773a 6173 6369 693d 2243 6f6e 736f  s w:ascii="Conso
-0000a230: 6c61 7322 2077 3a68 416e 7369 3d22 436f  las" w:hAnsi="Co
-0000a240: 6e73 6f6c 6173 222f 3e3c 773a 737a 2077  nsolas"/><w:sz w
-0000a250: 3a76 616c 3d22 3230 222f 3e3c 773a 737a  :val="20"/><w:sz
-0000a260: 4373 2077 3a76 616c 3d22 3230 222f 3e3c  Cs w:val="20"/><
-0000a270: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
-0000a280: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
-0000a290: 3d22 6368 6172 6163 7465 7222 2077 3a63  ="character" w:c
-0000a2a0: 7573 746f 6d53 7479 6c65 3d22 3122 2077  ustomStyle="1" w
-0000a2b0: 3a73 7479 6c65 4964 3d22 4d61 6372 6f54  :styleId="MacroT
-0000a2c0: 6578 7443 6861 7222 3e3c 773a 6e61 6d65  extChar"><w:name
-0000a2d0: 2077 3a76 616c 3d22 4d61 6372 6f20 5465   w:val="Macro Te
-0000a2e0: 7874 2043 6861 7222 2f3e 3c77 3a62 6173  xt Char"/><w:bas
-0000a2f0: 6564 4f6e 2077 3a76 616c 3d22 4465 6661  edOn w:val="Defa
-0000a300: 756c 7450 6172 6167 7261 7068 466f 6e74  ultParagraphFont
-0000a310: 222f 3e3c 773a 6c69 6e6b 2077 3a76 616c  "/><w:link w:val
-0000a320: 3d22 4d61 6372 6f54 6578 7422 2f3e 3c77  ="MacroText"/><w
-0000a330: 3a75 6950 7269 6f72 6974 7920 773a 7661  :uiPriority w:va
-0000a340: 6c3d 2239 3922 2f3e 3c77 3a72 7369 6420  l="99"/><w:rsid 
-0000a350: 773a 7661 6c3d 2230 3044 3732 3535 4122  w:val="00D7255A"
-0000a360: 2f3e 3c77 3a72 5072 3e3c 773a 7246 6f6e  /><w:rPr><w:rFon
-0000a370: 7473 2077 3a61 7363 6969 3d22 436f 6e73  ts w:ascii="Cons
-0000a380: 6f6c 6173 2220 773a 6841 6e73 693d 2243  olas" w:hAnsi="C
-0000a390: 6f6e 736f 6c61 7322 2f3e 3c77 3a73 7a20  onsolas"/><w:sz 
-0000a3a0: 773a 7661 6c3d 2232 3022 2f3e 3c77 3a73  w:val="20"/><w:s
-0000a3b0: 7a43 7320 773a 7661 6c3d 2232 3022 2f3e  zCs w:val="20"/>
-0000a3c0: 3c2f 773a 7250 723e 3c2f 773a 7374 796c  </w:rPr></w:styl
-0000a3d0: 653e 3c77 3a73 7479 6c65 2077 3a74 7970  e><w:style w:typ
-0000a3e0: 653d 2263 6861 7261 6374 6572 2220 773a  e="character" w:
-0000a3f0: 7374 796c 6549 643d 224d 656e 7469 6f6e  styleId="Mention
-0000a400: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
-0000a410: 224d 656e 7469 6f6e 222f 3e3c 773a 6261  "Mention"/><w:ba
-0000a420: 7365 644f 6e20 773a 7661 6c3d 2244 6566  sedOn w:val="Def
-0000a430: 6175 6c74 5061 7261 6772 6170 6846 6f6e  aultParagraphFon
-0000a440: 7422 2f3e 3c77 3a75 6950 7269 6f72 6974  t"/><w:uiPriorit
-0000a450: 7920 773a 7661 6c3d 2239 3922 2f3e 3c77  y w:val="99"/><w
-0000a460: 3a75 6e68 6964 6557 6865 6e55 7365 642f  :unhideWhenUsed/
-0000a470: 3e3c 773a 7273 6964 2077 3a76 616c 3d22  ><w:rsid w:val="
-0000a480: 3030 4437 3235 3541 222f 3e3c 773a 7250  00D7255A"/><w:rP
-0000a490: 723e 3c77 3a63 6f6c 6f72 2077 3a76 616c  r><w:color w:val
-0000a4a0: 3d22 3242 3537 3941 222f 3e3c 773a 7368  ="2B579A"/><w:sh
-0000a4b0: 6420 773a 7661 6c3d 2263 6c65 6172 2220  d w:val="clear" 
-0000a4c0: 773a 636f 6c6f 723d 2261 7574 6f22 2077  w:color="auto" w
-0000a4d0: 3a66 696c 6c3d 2245 3144 4644 4422 2f3e  :fill="E1DFDD"/>
-0000a4e0: 3c2f 773a 7250 723e 3c2f 773a 7374 796c  </w:rPr></w:styl
-0000a4f0: 653e 3c77 3a73 7479 6c65 2077 3a74 7970  e><w:style w:typ
-0000a500: 653d 2270 6172 6167 7261 7068 2220 773a  e="paragraph" w:
-0000a510: 7374 796c 6549 643d 224d 6573 7361 6765  styleId="Message
-0000a520: 4865 6164 6572 223e 3c77 3a6e 616d 6520  Header"><w:name 
-0000a530: 773a 7661 6c3d 224d 6573 7361 6765 2048  w:val="Message H
-0000a540: 6561 6465 7222 2f3e 3c77 3a62 6173 6564  eader"/><w:based
-0000a550: 4f6e 2077 3a76 616c 3d22 4e6f 726d 616c  On w:val="Normal
-0000a560: 222f 3e3c 773a 6c69 6e6b 2077 3a76 616c  "/><w:link w:val
-0000a570: 3d22 4d65 7373 6167 6548 6561 6465 7243  ="MessageHeaderC
-0000a580: 6861 7222 2f3e 3c77 3a75 6950 7269 6f72  har"/><w:uiPrior
-0000a590: 6974 7920 773a 7661 6c3d 2239 3922 2f3e  ity w:val="99"/>
-0000a5a0: 3c77 3a75 6e68 6964 6557 6865 6e55 7365  <w:unhideWhenUse
-0000a5b0: 642f 3e3c 773a 7273 6964 2077 3a76 616c  d/><w:rsid w:val
-0000a5c0: 3d22 3030 4437 3235 3541 222f 3e3c 773a  ="00D7255A"/><w:
-0000a5d0: 7050 723e 3c77 3a70 4264 723e 3c77 3a74  pPr><w:pBdr><w:t
-0000a5e0: 6f70 2077 3a76 616c 3d22 7369 6e67 6c65  op w:val="single
-0000a5f0: 2220 773a 737a 3d22 3622 2077 3a73 7061  " w:sz="6" w:spa
-0000a600: 6365 3d22 3122 2077 3a63 6f6c 6f72 3d22  ce="1" w:color="
-0000a610: 6175 746f 222f 3e3c 773a 6c65 6674 2077  auto"/><w:left w
-0000a620: 3a76 616c 3d22 7369 6e67 6c65 2220 773a  :val="single" w:
-0000a630: 737a 3d22 3622 2077 3a73 7061 6365 3d22  sz="6" w:space="
-0000a640: 3122 2077 3a63 6f6c 6f72 3d22 6175 746f  1" w:color="auto
-0000a650: 222f 3e3c 773a 626f 7474 6f6d 2077 3a76  "/><w:bottom w:v
-0000a660: 616c 3d22 7369 6e67 6c65 2220 773a 737a  al="single" w:sz
-0000a670: 3d22 3622 2077 3a73 7061 6365 3d22 3122  ="6" w:space="1"
-0000a680: 2077 3a63 6f6c 6f72 3d22 6175 746f 222f   w:color="auto"/
-0000a690: 3e3c 773a 7269 6768 7420 773a 7661 6c3d  ><w:right w:val=
-0000a6a0: 2273 696e 676c 6522 2077 3a73 7a3d 2236  "single" w:sz="6
-0000a6b0: 2220 773a 7370 6163 653d 2231 2220 773a  " w:space="1" w:
-0000a6c0: 636f 6c6f 723d 2261 7574 6f22 2f3e 3c2f  color="auto"/></
-0000a6d0: 773a 7042 6472 3e3c 773a 7368 6420 773a  w:pBdr><w:shd w:
-0000a6e0: 7661 6c3d 2270 6374 3230 2220 773a 636f  val="pct20" w:co
-0000a6f0: 6c6f 723d 2261 7574 6f22 2077 3a66 696c  lor="auto" w:fil
-0000a700: 6c3d 2261 7574 6f22 2f3e 3c77 3a73 7061  l="auto"/><w:spa
-0000a710: 6369 6e67 2077 3a61 6674 6572 3d22 3022  cing w:after="0"
-0000a720: 2077 3a6c 696e 653d 2232 3430 2220 773a   w:line="240" w:
-0000a730: 6c69 6e65 5275 6c65 3d22 6175 746f 222f  lineRule="auto"/
-0000a740: 3e3c 773a 696e 6420 773a 6c65 6674 3d22  ><w:ind w:left="
-0000a750: 3131 3334 2220 773a 6861 6e67 696e 673d  1134" w:hanging=
-0000a760: 2231 3133 3422 2f3e 3c2f 773a 7050 723e  "1134"/></w:pPr>
-0000a770: 3c77 3a72 5072 3e3c 773a 7246 6f6e 7473  <w:rPr><w:rFonts
-0000a780: 2077 3a61 7363 6969 5468 656d 653d 226d   w:asciiTheme="m
-0000a790: 616a 6f72 4841 6e73 6922 2077 3a65 6173  ajorHAnsi" w:eas
-0000a7a0: 7441 7369 6154 6865 6d65 3d22 6d61 6a6f  tAsiaTheme="majo
-0000a7b0: 7245 6173 7441 7369 6122 2077 3a68 416e  rEastAsia" w:hAn
-0000a7c0: 7369 5468 656d 653d 226d 616a 6f72 4841  siTheme="majorHA
-0000a7d0: 6e73 6922 2077 3a63 7374 6865 6d65 3d22  nsi" w:cstheme="
-0000a7e0: 6d61 6a6f 7242 6964 6922 2f3e 3c77 3a73  majorBidi"/><w:s
-0000a7f0: 7a20 773a 7661 6c3d 2232 3422 2f3e 3c77  z w:val="24"/><w
-0000a800: 3a73 7a43 7320 773a 7661 6c3d 2232 3422  :szCs w:val="24"
-0000a810: 2f3e 3c2f 773a 7250 723e 3c2f 773a 7374  /></w:rPr></w:st
-0000a820: 796c 653e 3c77 3a73 7479 6c65 2077 3a74  yle><w:style w:t
-0000a830: 7970 653d 2263 6861 7261 6374 6572 2220  ype="character" 
-0000a840: 773a 6375 7374 6f6d 5374 796c 653d 2231  w:customStyle="1
-0000a850: 2220 773a 7374 796c 6549 643d 224d 6573  " w:styleId="Mes
-0000a860: 7361 6765 4865 6164 6572 4368 6172 223e  sageHeaderChar">
-0000a870: 3c77 3a6e 616d 6520 773a 7661 6c3d 224d  <w:name w:val="M
-0000a880: 6573 7361 6765 2048 6561 6465 7220 4368  essage Header Ch
-0000a890: 6172 222f 3e3c 773a 6261 7365 644f 6e20  ar"/><w:basedOn 
-0000a8a0: 773a 7661 6c3d 2244 6566 6175 6c74 5061  w:val="DefaultPa
-0000a8b0: 7261 6772 6170 6846 6f6e 7422 2f3e 3c77  ragraphFont"/><w
-0000a8c0: 3a6c 696e 6b20 773a 7661 6c3d 224d 6573  :link w:val="Mes
-0000a8d0: 7361 6765 4865 6164 6572 222f 3e3c 773a  sageHeader"/><w:
-0000a8e0: 7569 5072 696f 7269 7479 2077 3a76 616c  uiPriority w:val
-0000a8f0: 3d22 3939 222f 3e3c 773a 7273 6964 2077  ="99"/><w:rsid w
-0000a900: 3a76 616c 3d22 3030 4437 3235 3541 222f  :val="00D7255A"/
-0000a910: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
-0000a920: 7320 773a 6173 6369 6954 6865 6d65 3d22  s w:asciiTheme="
-0000a930: 6d61 6a6f 7248 416e 7369 2220 773a 6561  majorHAnsi" w:ea
-0000a940: 7374 4173 6961 5468 656d 653d 226d 616a  stAsiaTheme="maj
-0000a950: 6f72 4561 7374 4173 6961 2220 773a 6841  orEastAsia" w:hA
-0000a960: 6e73 6954 6865 6d65 3d22 6d61 6a6f 7248  nsiTheme="majorH
-0000a970: 416e 7369 2220 773a 6373 7468 656d 653d  Ansi" w:cstheme=
-0000a980: 226d 616a 6f72 4269 6469 222f 3e3c 773a  "majorBidi"/><w:
-0000a990: 737a 2077 3a76 616c 3d22 3234 222f 3e3c  sz w:val="24"/><
-0000a9a0: 773a 737a 4373 2077 3a76 616c 3d22 3234  w:szCs w:val="24
-0000a9b0: 222f 3e3c 773a 7368 6420 773a 7661 6c3d  "/><w:shd w:val=
-0000a9c0: 2270 6374 3230 2220 773a 636f 6c6f 723d  "pct20" w:color=
-0000a9d0: 2261 7574 6f22 2077 3a66 696c 6c3d 2261  "auto" w:fill="a
-0000a9e0: 7574 6f22 2f3e 3c2f 773a 7250 723e 3c2f  uto"/></w:rPr></
-0000a9f0: 773a 7374 796c 653e 3c77 3a73 7479 6c65  w:style><w:style
-0000aa00: 2077 3a74 7970 653d 2270 6172 6167 7261   w:type="paragra
-0000aa10: 7068 2220 773a 7374 796c 6549 643d 2250  ph" w:styleId="P
-0000aa20: 6c61 696e 5465 7874 223e 3c77 3a6e 616d  lainText"><w:nam
-0000aa30: 6520 773a 7661 6c3d 2250 6c61 696e 2054  e w:val="Plain T
-0000aa40: 6578 7422 2f3e 3c77 3a62 6173 6564 4f6e  ext"/><w:basedOn
-0000aa50: 2077 3a76 616c 3d22 4e6f 726d 616c 222f   w:val="Normal"/
-0000aa60: 3e3c 773a 6c69 6e6b 2077 3a76 616c 3d22  ><w:link w:val="
-0000aa70: 506c 6169 6e54 6578 7443 6861 7222 2f3e  PlainTextChar"/>
-0000aa80: 3c77 3a75 6950 7269 6f72 6974 7920 773a  <w:uiPriority w:
-0000aa90: 7661 6c3d 2239 3922 2f3e 3c77 3a75 6e68  val="99"/><w:unh
-0000aaa0: 6964 6557 6865 6e55 7365 642f 3e3c 773a  ideWhenUsed/><w:
-0000aab0: 7273 6964 2077 3a76 616c 3d22 3030 4437  rsid w:val="00D7
-0000aac0: 3235 3541 222f 3e3c 773a 7050 723e 3c77  255A"/><w:pPr><w
-0000aad0: 3a73 7061 6369 6e67 2077 3a61 6674 6572  :spacing w:after
-0000aae0: 3d22 3022 2077 3a6c 696e 653d 2232 3430  ="0" w:line="240
-0000aaf0: 2220 773a 6c69 6e65 5275 6c65 3d22 6175  " w:lineRule="au
-0000ab00: 746f 222f 3e3c 2f77 3a70 5072 3e3c 773a  to"/></w:pPr><w:
-0000ab10: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
-0000ab20: 6173 6369 693d 2243 6f6e 736f 6c61 7322  ascii="Consolas"
-0000ab30: 2077 3a68 416e 7369 3d22 436f 6e73 6f6c   w:hAnsi="Consol
-0000ab40: 6173 222f 3e3c 773a 737a 2077 3a76 616c  as"/><w:sz w:val
-0000ab50: 3d22 3231 222f 3e3c 773a 737a 4373 2077  ="21"/><w:szCs w
-0000ab60: 3a76 616c 3d22 3231 222f 3e3c 2f77 3a72  :val="21"/></w:r
-0000ab70: 5072 3e3c 2f77 3a73 7479 6c65 3e3c 773a  Pr></w:style><w:
-0000ab80: 7374 796c 6520 773a 7479 7065 3d22 6368  style w:type="ch
-0000ab90: 6172 6163 7465 7222 2077 3a63 7573 746f  aracter" w:custo
-0000aba0: 6d53 7479 6c65 3d22 3122 2077 3a73 7479  mStyle="1" w:sty
-0000abb0: 6c65 4964 3d22 506c 6169 6e54 6578 7443  leId="PlainTextC
-0000abc0: 6861 7222 3e3c 773a 6e61 6d65 2077 3a76  har"><w:name w:v
-0000abd0: 616c 3d22 506c 6169 6e20 5465 7874 2043  al="Plain Text C
-0000abe0: 6861 7222 2f3e 3c77 3a62 6173 6564 4f6e  har"/><w:basedOn
-0000abf0: 2077 3a76 616c 3d22 4465 6661 756c 7450   w:val="DefaultP
-0000ac00: 6172 6167 7261 7068 466f 6e74 222f 3e3c  aragraphFont"/><
-0000ac10: 773a 6c69 6e6b 2077 3a76 616c 3d22 506c  w:link w:val="Pl
-0000ac20: 6169 6e54 6578 7422 2f3e 3c77 3a75 6950  ainText"/><w:uiP
-0000ac30: 7269 6f72 6974 7920 773a 7661 6c3d 2239  riority w:val="9
-0000ac40: 3922 2f3e 3c77 3a72 7369 6420 773a 7661  9"/><w:rsid w:va
-0000ac50: 6c3d 2230 3044 3732 3535 4122 2f3e 3c77  l="00D7255A"/><w
-0000ac60: 3a72 5072 3e3c 773a 7246 6f6e 7473 2077  :rPr><w:rFonts w
-0000ac70: 3a61 7363 6969 3d22 436f 6e73 6f6c 6173  :ascii="Consolas
-0000ac80: 2220 773a 6841 6e73 693d 2243 6f6e 736f  " w:hAnsi="Conso
-0000ac90: 6c61 7322 2f3e 3c77 3a73 7a20 773a 7661  las"/><w:sz w:va
-0000aca0: 6c3d 2232 3122 2f3e 3c77 3a73 7a43 7320  l="21"/><w:szCs 
-0000acb0: 773a 7661 6c3d 2232 3122 2f3e 3c2f 773a  w:val="21"/></w:
-0000acc0: 7250 723e 3c2f 773a 7374 796c 653e 3c2f  rPr></w:style></
-0000acd0: 773a 7374 796c 6573 3e                   w:styles>
+00000030: 2279 6573 223f 3e0a 3c77 3a73 7479 6c65  "yes"?>.<w:style
+00000040: 7320 786d 6c6e 733a 6d63 3d22 6874 7470  s xmlns:mc="http
+00000050: 3a2f 2f73 6368 656d 6173 2e6f 7065 6e78  ://schemas.openx
+00000060: 6d6c 666f 726d 6174 732e 6f72 672f 6d61  mlformats.org/ma
+00000070: 726b 7570 2d63 6f6d 7061 7469 6269 6c69  rkup-compatibili
+00000080: 7479 2f32 3030 3622 2078 6d6c 6e73 3a72  ty/2006" xmlns:r
+00000090: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
+000000a0: 2e6f 7065 6e78 6d6c 666f 726d 6174 732e  .openxmlformats.
+000000b0: 6f72 672f 6f66 6669 6365 446f 6375 6d65  org/officeDocume
+000000c0: 6e74 2f32 3030 362f 7265 6c61 7469 6f6e  nt/2006/relation
+000000d0: 7368 6970 7322 2078 6d6c 6e73 3a77 3d22  ships" xmlns:w="
+000000e0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6f  http://schemas.o
+000000f0: 7065 6e78 6d6c 666f 726d 6174 732e 6f72  penxmlformats.or
+00000100: 672f 776f 7264 7072 6f63 6573 7369 6e67  g/wordprocessing
+00000110: 6d6c 2f32 3030 362f 6d61 696e 2220 786d  ml/2006/main" xm
+00000120: 6c6e 733a 7731 343d 2268 7474 703a 2f2f  lns:w14="http://
+00000130: 7363 6865 6d61 732e 6d69 6372 6f73 6f66  schemas.microsof
+00000140: 742e 636f 6d2f 6f66 6669 6365 2f77 6f72  t.com/office/wor
+00000150: 642f 3230 3130 2f77 6f72 646d 6c22 2078  d/2010/wordml" x
+00000160: 6d6c 6e73 3a77 3135 3d22 6874 7470 3a2f  mlns:w15="http:/
+00000170: 2f73 6368 656d 6173 2e6d 6963 726f 736f  /schemas.microso
+00000180: 6674 2e63 6f6d 2f6f 6666 6963 652f 776f  ft.com/office/wo
+00000190: 7264 2f32 3031 322f 776f 7264 6d6c 2220  rd/2012/wordml" 
+000001a0: 786d 6c6e 733a 7731 3663 6578 3d22 6874  xmlns:w16cex="ht
+000001b0: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+000001c0: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+000001d0: 652f 776f 7264 2f32 3031 382f 776f 7264  e/word/2018/word
+000001e0: 6d6c 2f63 6578 2220 786d 6c6e 733a 7731  ml/cex" xmlns:w1
+000001f0: 3663 6964 3d22 6874 7470 3a2f 2f73 6368  6cid="http://sch
+00000200: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
+00000210: 6f6d 2f6f 6666 6963 652f 776f 7264 2f32  om/office/word/2
+00000220: 3031 362f 776f 7264 6d6c 2f63 6964 2220  016/wordml/cid" 
+00000230: 786d 6c6e 733a 7731 363d 2268 7474 703a  xmlns:w16="http:
+00000240: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+00000250: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
+00000260: 6f72 642f 3230 3138 2f77 6f72 646d 6c22  ord/2018/wordml"
+00000270: 2078 6d6c 6e73 3a77 3136 7364 7464 683d   xmlns:w16sdtdh=
+00000280: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+00000290: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
+000002a0: 6669 6365 2f77 6f72 642f 3230 3230 2f77  fice/word/2020/w
+000002b0: 6f72 646d 6c2f 7364 7464 6174 6168 6173  ordml/sdtdatahas
+000002c0: 6822 2078 6d6c 6e73 3a77 3136 7365 3d22  h" xmlns:w16se="
+000002d0: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
+000002e0: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
+000002f0: 6963 652f 776f 7264 2f32 3031 352f 776f  ice/word/2015/wo
+00000300: 7264 6d6c 2f73 796d 6578 2220 6d63 3a49  rdml/symex" mc:I
+00000310: 676e 6f72 6162 6c65 3d22 7731 3420 7731  gnorable="w14 w1
+00000320: 3520 7731 3673 6520 7731 3663 6964 2077  5 w16se w16cid w
+00000330: 3136 2077 3136 6365 7820 7731 3673 6474  16 w16cex w16sdt
+00000340: 6468 223e 3c77 3a64 6f63 4465 6661 756c  dh"><w:docDefaul
+00000350: 7473 3e3c 773a 7250 7244 6566 6175 6c74  ts><w:rPrDefault
+00000360: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
+00000370: 7320 773a 6173 6369 6954 6865 6d65 3d22  s w:asciiTheme="
+00000380: 6d69 6e6f 7248 416e 7369 2220 773a 6561  minorHAnsi" w:ea
+00000390: 7374 4173 6961 5468 656d 653d 226d 696e  stAsiaTheme="min
+000003a0: 6f72 4841 6e73 6922 2077 3a68 416e 7369  orHAnsi" w:hAnsi
+000003b0: 5468 656d 653d 226d 696e 6f72 4841 6e73  Theme="minorHAns
+000003c0: 6922 2077 3a63 7374 6865 6d65 3d22 6d69  i" w:cstheme="mi
+000003d0: 6e6f 7242 6964 6922 2f3e 3c77 3a73 7a20  norBidi"/><w:sz 
+000003e0: 773a 7661 6c3d 2232 3222 2f3e 3c77 3a73  w:val="22"/><w:s
+000003f0: 7a43 7320 773a 7661 6c3d 2232 3222 2f3e  zCs w:val="22"/>
+00000400: 3c77 3a6c 616e 6720 773a 7661 6c3d 2265  <w:lang w:val="e
+00000410: 6e2d 4445 2220 773a 6561 7374 4173 6961  n-DE" w:eastAsia
+00000420: 3d22 656e 2d55 5322 2077 3a62 6964 693d  ="en-US" w:bidi=
+00000430: 2261 722d 5341 222f 3e3c 2f77 3a72 5072  "ar-SA"/></w:rPr
+00000440: 3e3c 2f77 3a72 5072 4465 6661 756c 743e  ></w:rPrDefault>
+00000450: 3c77 3a70 5072 4465 6661 756c 743e 3c77  <w:pPrDefault><w
+00000460: 3a70 5072 3e3c 773a 7370 6163 696e 6720  :pPr><w:spacing 
+00000470: 773a 6166 7465 723d 2231 3630 2220 773a  w:after="160" w:
+00000480: 6c69 6e65 3d22 3235 3922 2077 3a6c 696e  line="259" w:lin
+00000490: 6552 756c 653d 2261 7574 6f22 2f3e 3c2f  eRule="auto"/></
+000004a0: 773a 7050 723e 3c2f 773a 7050 7244 6566  w:pPr></w:pPrDef
+000004b0: 6175 6c74 3e3c 2f77 3a64 6f63 4465 6661  ault></w:docDefa
+000004c0: 756c 7473 3e3c 773a 6c61 7465 6e74 5374  ults><w:latentSt
+000004d0: 796c 6573 2077 3a64 6566 4c6f 636b 6564  yles w:defLocked
+000004e0: 5374 6174 653d 2230 2220 773a 6465 6655  State="0" w:defU
+000004f0: 4950 7269 6f72 6974 793d 2239 3922 2077  IPriority="99" w
+00000500: 3a64 6566 5365 6d69 4869 6464 656e 3d22  :defSemiHidden="
+00000510: 3022 2077 3a64 6566 556e 6869 6465 5768  0" w:defUnhideWh
+00000520: 656e 5573 6564 3d22 3022 2077 3a64 6566  enUsed="0" w:def
+00000530: 5146 6f72 6d61 743d 2230 2220 773a 636f  QFormat="0" w:co
+00000540: 756e 743d 2233 3736 223e 3c77 3a6c 7364  unt="376"><w:lsd
+00000550: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00000560: 3d22 4e6f 726d 616c 2220 773a 7569 5072  ="Normal" w:uiPr
+00000570: 696f 7269 7479 3d22 3022 2077 3a71 466f  iority="0" w:qFo
+00000580: 726d 6174 3d22 3122 2f3e 3c77 3a6c 7364  rmat="1"/><w:lsd
+00000590: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000005a0: 3d22 6865 6164 696e 6720 3122 2077 3a75  ="heading 1" w:u
+000005b0: 6950 7269 6f72 6974 793d 2239 2220 773a  iPriority="9" w:
+000005c0: 7146 6f72 6d61 743d 2231 222f 3e3c 773a  qFormat="1"/><w:
+000005d0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000005e0: 616d 653d 2268 6561 6469 6e67 2032 2220  ame="heading 2" 
+000005f0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00000600: 2077 3a75 6950 7269 6f72 6974 793d 2239   w:uiPriority="9
+00000610: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00000620: 6564 3d22 3122 2077 3a71 466f 726d 6174  ed="1" w:qFormat
+00000630: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00000640: 7074 696f 6e20 773a 6e61 6d65 3d22 6865  ption w:name="he
+00000650: 6164 696e 6720 3322 2077 3a73 656d 6948  ading 3" w:semiH
+00000660: 6964 6465 6e3d 2231 2220 773a 7569 5072  idden="1" w:uiPr
+00000670: 696f 7269 7479 3d22 3922 2077 3a75 6e68  iority="9" w:unh
+00000680: 6964 6557 6865 6e55 7365 643d 2231 2220  ideWhenUsed="1" 
+00000690: 773a 7146 6f72 6d61 743d 2231 222f 3e3c  w:qFormat="1"/><
+000006a0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+000006b0: 3a6e 616d 653d 2268 6561 6469 6e67 2034  :name="heading 4
+000006c0: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+000006d0: 3122 2077 3a75 6950 7269 6f72 6974 793d  1" w:uiPriority=
+000006e0: 2239 2220 773a 756e 6869 6465 5768 656e  "9" w:unhideWhen
+000006f0: 5573 6564 3d22 3122 2077 3a71 466f 726d  Used="1" w:qForm
+00000700: 6174 3d22 3122 2f3e 3c77 3a6c 7364 4578  at="1"/><w:lsdEx
+00000710: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00000720: 6865 6164 696e 6720 3522 2077 3a73 656d  heading 5" w:sem
+00000730: 6948 6964 6465 6e3d 2231 2220 773a 7569  iHidden="1" w:ui
+00000740: 5072 696f 7269 7479 3d22 3922 2077 3a75  Priority="9" w:u
+00000750: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
+00000760: 2220 773a 7146 6f72 6d61 743d 2231 222f  " w:qFormat="1"/
+00000770: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00000780: 2077 3a6e 616d 653d 2268 6561 6469 6e67   w:name="heading
+00000790: 2036 2220 773a 7365 6d69 4869 6464 656e   6" w:semiHidden
+000007a0: 3d22 3122 2077 3a75 6950 7269 6f72 6974  ="1" w:uiPriorit
+000007b0: 793d 2239 2220 773a 756e 6869 6465 5768  y="9" w:unhideWh
+000007c0: 656e 5573 6564 3d22 3122 2077 3a71 466f  enUsed="1" w:qFo
+000007d0: 726d 6174 3d22 3122 2f3e 3c77 3a6c 7364  rmat="1"/><w:lsd
+000007e0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000007f0: 3d22 6865 6164 696e 6720 3722 2077 3a73  ="heading 7" w:s
+00000800: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00000810: 7569 5072 696f 7269 7479 3d22 3922 2077  uiPriority="9" w
+00000820: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000830: 2231 2220 773a 7146 6f72 6d61 743d 2231  "1" w:qFormat="1
+00000840: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00000850: 6f6e 2077 3a6e 616d 653d 2268 6561 6469  on w:name="headi
+00000860: 6e67 2038 2220 773a 7365 6d69 4869 6464  ng 8" w:semiHidd
+00000870: 656e 3d22 3122 2077 3a75 6950 7269 6f72  en="1" w:uiPrior
+00000880: 6974 793d 2239 2220 773a 756e 6869 6465  ity="9" w:unhide
+00000890: 5768 656e 5573 6564 3d22 3122 2077 3a71  WhenUsed="1" w:q
+000008a0: 466f 726d 6174 3d22 3122 2f3e 3c77 3a6c  Format="1"/><w:l
+000008b0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000008c0: 6d65 3d22 6865 6164 696e 6720 3922 2077  me="heading 9" w
+000008d0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+000008e0: 773a 7569 5072 696f 7269 7479 3d22 3922  w:uiPriority="9"
+000008f0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00000900: 643d 2231 2220 773a 7146 6f72 6d61 743d  d="1" w:qFormat=
+00000910: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000920: 7469 6f6e 2077 3a6e 616d 653d 2269 6e64  tion w:name="ind
+00000930: 6578 2031 2220 773a 7365 6d69 4869 6464  ex 1" w:semiHidd
+00000940: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00000950: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000960: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000970: 616d 653d 2269 6e64 6578 2032 2220 773a  ame="index 2" w:
+00000980: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+00000990: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+000009a0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+000009b0: 7469 6f6e 2077 3a6e 616d 653d 2269 6e64  tion w:name="ind
+000009c0: 6578 2033 2220 773a 7365 6d69 4869 6464  ex 3" w:semiHidd
+000009d0: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+000009e0: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+000009f0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000a00: 616d 653d 2269 6e64 6578 2034 2220 773a  ame="index 4" w:
+00000a10: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+00000a20: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000a30: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000a40: 7469 6f6e 2077 3a6e 616d 653d 2269 6e64  tion w:name="ind
+00000a50: 6578 2035 2220 773a 7365 6d69 4869 6464  ex 5" w:semiHidd
+00000a60: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00000a70: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000a80: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000a90: 616d 653d 2269 6e64 6578 2036 2220 773a  ame="index 6" w:
+00000aa0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+00000ab0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000ac0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000ad0: 7469 6f6e 2077 3a6e 616d 653d 2269 6e64  tion w:name="ind
+00000ae0: 6578 2037 2220 773a 7365 6d69 4869 6464  ex 7" w:semiHidd
+00000af0: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00000b00: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000b10: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000b20: 616d 653d 2269 6e64 6578 2038 2220 773a  ame="index 8" w:
+00000b30: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+00000b40: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000b50: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000b60: 7469 6f6e 2077 3a6e 616d 653d 2269 6e64  tion w:name="ind
+00000b70: 6578 2039 2220 773a 7365 6d69 4869 6464  ex 9" w:semiHidd
+00000b80: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00000b90: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000ba0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000bb0: 616d 653d 2274 6f63 2031 2220 773a 7365  ame="toc 1" w:se
+00000bc0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00000bd0: 6950 7269 6f72 6974 793d 2233 3922 2077  iPriority="39" w
+00000be0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000bf0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000c00: 7469 6f6e 2077 3a6e 616d 653d 2274 6f63  tion w:name="toc
+00000c10: 2032 2220 773a 7365 6d69 4869 6464 656e   2" w:semiHidden
+00000c20: 3d22 3122 2077 3a75 6950 7269 6f72 6974  ="1" w:uiPriorit
+00000c30: 793d 2233 3922 2077 3a75 6e68 6964 6557  y="39" w:unhideW
+00000c40: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000c50: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000c60: 616d 653d 2274 6f63 2033 2220 773a 7365  ame="toc 3" w:se
+00000c70: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00000c80: 6950 7269 6f72 6974 793d 2233 3922 2077  iPriority="39" w
+00000c90: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000ca0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000cb0: 7469 6f6e 2077 3a6e 616d 653d 2274 6f63  tion w:name="toc
+00000cc0: 2034 2220 773a 7365 6d69 4869 6464 656e   4" w:semiHidden
+00000cd0: 3d22 3122 2077 3a75 6950 7269 6f72 6974  ="1" w:uiPriorit
+00000ce0: 793d 2233 3922 2077 3a75 6e68 6964 6557  y="39" w:unhideW
+00000cf0: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000d00: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000d10: 616d 653d 2274 6f63 2035 2220 773a 7365  ame="toc 5" w:se
+00000d20: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00000d30: 6950 7269 6f72 6974 793d 2233 3922 2077  iPriority="39" w
+00000d40: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000d50: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000d60: 7469 6f6e 2077 3a6e 616d 653d 2274 6f63  tion w:name="toc
+00000d70: 2036 2220 773a 7365 6d69 4869 6464 656e   6" w:semiHidden
+00000d80: 3d22 3122 2077 3a75 6950 7269 6f72 6974  ="1" w:uiPriorit
+00000d90: 793d 2233 3922 2077 3a75 6e68 6964 6557  y="39" w:unhideW
+00000da0: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000db0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000dc0: 616d 653d 2274 6f63 2037 2220 773a 7365  ame="toc 7" w:se
+00000dd0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00000de0: 6950 7269 6f72 6974 793d 2233 3922 2077  iPriority="39" w
+00000df0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000e00: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000e10: 7469 6f6e 2077 3a6e 616d 653d 2274 6f63  tion w:name="toc
+00000e20: 2038 2220 773a 7365 6d69 4869 6464 656e   8" w:semiHidden
+00000e30: 3d22 3122 2077 3a75 6950 7269 6f72 6974  ="1" w:uiPriorit
+00000e40: 793d 2233 3922 2077 3a75 6e68 6964 6557  y="39" w:unhideW
+00000e50: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00000e60: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00000e70: 616d 653d 2274 6f63 2039 2220 773a 7365  ame="toc 9" w:se
+00000e80: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00000e90: 6950 7269 6f72 6974 793d 2233 3922 2077  iPriority="39" w
+00000ea0: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00000eb0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00000ec0: 7469 6f6e 2077 3a6e 616d 653d 224e 6f72  tion w:name="Nor
+00000ed0: 6d61 6c20 496e 6465 6e74 2220 773a 7365  mal Indent" w:se
+00000ee0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00000ef0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
+00000f00: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00000f10: 6f6e 2077 3a6e 616d 653d 2266 6f6f 746e  on w:name="footn
+00000f20: 6f74 6520 7465 7874 2220 773a 7365 6d69  ote text" w:semi
+00000f30: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
+00000f40: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
+00000f50: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00000f60: 2077 3a6e 616d 653d 2261 6e6e 6f74 6174   w:name="annotat
+00000f70: 696f 6e20 7465 7874 2220 773a 7365 6d69  ion text" w:semi
+00000f80: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
+00000f90: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
+00000fa0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00000fb0: 2077 3a6e 616d 653d 2268 6561 6465 7222   w:name="header"
+00000fc0: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00000fd0: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00000fe0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00000ff0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00001000: 666f 6f74 6572 2220 773a 7365 6d69 4869  footer" w:semiHi
+00001010: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
+00001020: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
+00001030: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00001040: 3a6e 616d 653d 2269 6e64 6578 2068 6561  :name="index hea
+00001050: 6469 6e67 2220 773a 7365 6d69 4869 6464  ding" w:semiHidd
+00001060: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00001070: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00001080: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00001090: 616d 653d 2263 6170 7469 6f6e 2220 773a  ame="caption" w:
+000010a0: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+000010b0: 3a75 6950 7269 6f72 6974 793d 2233 3522  :uiPriority="35"
+000010c0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+000010d0: 643d 2231 2220 773a 7146 6f72 6d61 743d  d="1" w:qFormat=
+000010e0: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+000010f0: 7469 6f6e 2077 3a6e 616d 653d 2274 6162  tion w:name="tab
+00001100: 6c65 206f 6620 6669 6775 7265 7322 2077  le of figures" w
+00001110: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00001120: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00001130: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00001140: 7074 696f 6e20 773a 6e61 6d65 3d22 656e  ption w:name="en
+00001150: 7665 6c6f 7065 2061 6464 7265 7373 2220  velope address" 
+00001160: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00001170: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00001180: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00001190: 6570 7469 6f6e 2077 3a6e 616d 653d 2265  eption w:name="e
+000011a0: 6e76 656c 6f70 6520 7265 7475 726e 2220  nvelope return" 
+000011b0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+000011c0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+000011d0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+000011e0: 6570 7469 6f6e 2077 3a6e 616d 653d 2266  eption w:name="f
+000011f0: 6f6f 746e 6f74 6520 7265 6665 7265 6e63  ootnote referenc
+00001200: 6522 2077 3a73 656d 6948 6964 6465 6e3d  e" w:semiHidden=
+00001210: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
+00001220: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
+00001230: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00001240: 3d22 616e 6e6f 7461 7469 6f6e 2072 6566  ="annotation ref
+00001250: 6572 656e 6365 2220 773a 7365 6d69 4869  erence" w:semiHi
+00001260: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
+00001270: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
+00001280: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00001290: 3a6e 616d 653d 226c 696e 6520 6e75 6d62  :name="line numb
+000012a0: 6572 2220 773a 7365 6d69 4869 6464 656e  er" w:semiHidden
+000012b0: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
+000012c0: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
+000012d0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+000012e0: 653d 2270 6167 6520 6e75 6d62 6572 2220  e="page number" 
+000012f0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00001300: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00001310: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00001320: 6570 7469 6f6e 2077 3a6e 616d 653d 2265  eption w:name="e
+00001330: 6e64 6e6f 7465 2072 6566 6572 656e 6365  ndnote reference
+00001340: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00001350: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00001360: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00001370: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00001380: 2265 6e64 6e6f 7465 2074 6578 7422 2077  "endnote text" w
+00001390: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+000013a0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+000013b0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+000013c0: 7074 696f 6e20 773a 6e61 6d65 3d22 7461  ption w:name="ta
+000013d0: 626c 6520 6f66 2061 7574 686f 7269 7469  ble of authoriti
+000013e0: 6573 2220 773a 7365 6d69 4869 6464 656e  es" w:semiHidden
+000013f0: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
+00001400: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
+00001410: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00001420: 653d 226d 6163 726f 2220 773a 7365 6d69  e="macro" w:semi
+00001430: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
+00001440: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
+00001450: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00001460: 2077 3a6e 616d 653d 2274 6f61 2068 6561   w:name="toa hea
+00001470: 6469 6e67 2220 773a 7365 6d69 4869 6464  ding" w:semiHidd
+00001480: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00001490: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+000014a0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000014b0: 616d 653d 224c 6973 7422 2077 3a73 656d  ame="List" w:sem
+000014c0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
+000014d0: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
+000014e0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+000014f0: 6e20 773a 6e61 6d65 3d22 4c69 7374 2042  n w:name="List B
+00001500: 756c 6c65 7422 2077 3a73 656d 6948 6964  ullet" w:semiHid
+00001510: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
+00001520: 5768 656e 5573 6564 3d22 3122 2077 3a71  WhenUsed="1" w:q
+00001530: 466f 726d 6174 3d22 3122 2f3e 3c77 3a6c  Format="1"/><w:l
+00001540: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00001550: 6d65 3d22 4c69 7374 204e 756d 6265 7222  me="List Number"
+00001560: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00001570: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00001580: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00001590: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000015a0: 4c69 7374 2032 2220 773a 7365 6d69 4869  List 2" w:semiHi
+000015b0: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
+000015c0: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
+000015d0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+000015e0: 3a6e 616d 653d 224c 6973 7420 3322 2077  :name="List 3" w
+000015f0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00001600: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00001610: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00001620: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+00001630: 7374 2034 2220 773a 7365 6d69 4869 6464  st 4" w:semiHidd
+00001640: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00001650: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00001660: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00001670: 616d 653d 224c 6973 7420 3522 2077 3a73  ame="List 5" w:s
+00001680: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00001690: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+000016a0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+000016b0: 696f 6e20 773a 6e61 6d65 3d22 4c69 7374  ion w:name="List
+000016c0: 2042 756c 6c65 7420 3222 2077 3a73 656d   Bullet 2" w:sem
+000016d0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
+000016e0: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
+000016f0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00001700: 6e20 773a 6e61 6d65 3d22 4c69 7374 2042  n w:name="List B
+00001710: 756c 6c65 7420 3322 2077 3a73 656d 6948  ullet 3" w:semiH
+00001720: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
+00001730: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
+00001740: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00001750: 773a 6e61 6d65 3d22 4c69 7374 2042 756c  w:name="List Bul
+00001760: 6c65 7420 3422 2077 3a73 656d 6948 6964  let 4" w:semiHid
+00001770: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
+00001780: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
+00001790: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+000017a0: 6e61 6d65 3d22 4c69 7374 2042 756c 6c65  name="List Bulle
+000017b0: 7420 3522 2077 3a73 656d 6948 6964 6465  t 5" w:semiHidde
+000017c0: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
+000017d0: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
+000017e0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000017f0: 6d65 3d22 4c69 7374 204e 756d 6265 7220  me="List Number 
+00001800: 3222 2077 3a73 656d 6948 6964 6465 6e3d  2" w:semiHidden=
+00001810: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
+00001820: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
+00001830: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00001840: 3d22 4c69 7374 204e 756d 6265 7220 3322  ="List Number 3"
+00001850: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00001860: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00001870: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00001880: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00001890: 4c69 7374 204e 756d 6265 7220 3422 2077  List Number 4" w
+000018a0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+000018b0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+000018c0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+000018d0: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+000018e0: 7374 204e 756d 6265 7220 3522 2077 3a73  st Number 5" w:s
+000018f0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00001900: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00001910: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00001920: 696f 6e20 773a 6e61 6d65 3d22 5469 746c  ion w:name="Titl
+00001930: 6522 2077 3a75 6950 7269 6f72 6974 793d  e" w:uiPriority=
+00001940: 2231 3022 2077 3a71 466f 726d 6174 3d22  "10" w:qFormat="
+00001950: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00001960: 696f 6e20 773a 6e61 6d65 3d22 436c 6f73  ion w:name="Clos
+00001970: 696e 6722 2077 3a73 656d 6948 6964 6465  ing" w:semiHidde
+00001980: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
+00001990: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
+000019a0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000019b0: 6d65 3d22 5369 676e 6174 7572 6522 2077  me="Signature" w
+000019c0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+000019d0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+000019e0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+000019f0: 7074 696f 6e20 773a 6e61 6d65 3d22 4465  ption w:name="De
+00001a00: 6661 756c 7420 5061 7261 6772 6170 6820  fault Paragraph 
+00001a10: 466f 6e74 2220 773a 7365 6d69 4869 6464  Font" w:semiHidd
+00001a20: 656e 3d22 3122 2077 3a75 6950 7269 6f72  en="1" w:uiPrior
+00001a30: 6974 793d 2231 2220 773a 756e 6869 6465  ity="1" w:unhide
+00001a40: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
+00001a50: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00001a60: 6e61 6d65 3d22 426f 6479 2054 6578 7422  name="Body Text"
+00001a70: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00001a80: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00001a90: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00001aa0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00001ab0: 426f 6479 2054 6578 7420 496e 6465 6e74  Body Text Indent
+00001ac0: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00001ad0: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00001ae0: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00001af0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00001b00: 224c 6973 7420 436f 6e74 696e 7565 2220  "List Continue" 
+00001b10: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00001b20: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00001b30: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00001b40: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00001b50: 6973 7420 436f 6e74 696e 7565 2032 2220  ist Continue 2" 
+00001b60: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00001b70: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00001b80: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00001b90: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00001ba0: 6973 7420 436f 6e74 696e 7565 2033 2220  ist Continue 3" 
+00001bb0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00001bc0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00001bd0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00001be0: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00001bf0: 6973 7420 436f 6e74 696e 7565 2034 2220  ist Continue 4" 
+00001c00: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00001c10: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00001c20: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00001c30: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00001c40: 6973 7420 436f 6e74 696e 7565 2035 2220  ist Continue 5" 
+00001c50: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00001c60: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00001c70: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00001c80: 6570 7469 6f6e 2077 3a6e 616d 653d 224d  eption w:name="M
+00001c90: 6573 7361 6765 2048 6561 6465 7222 2077  essage Header" w
+00001ca0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00001cb0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00001cc0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00001cd0: 7074 696f 6e20 773a 6e61 6d65 3d22 5375  ption w:name="Su
+00001ce0: 6274 6974 6c65 2220 773a 7569 5072 696f  btitle" w:uiPrio
+00001cf0: 7269 7479 3d22 3131 2220 773a 7146 6f72  rity="11" w:qFor
+00001d00: 6d61 743d 2231 222f 3e3c 773a 6c73 6445  mat="1"/><w:lsdE
+00001d10: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00001d20: 2253 616c 7574 6174 696f 6e22 2077 3a73  "Salutation" w:s
+00001d30: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00001d40: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00001d50: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00001d60: 696f 6e20 773a 6e61 6d65 3d22 4461 7465  ion w:name="Date
+00001d70: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00001d80: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00001d90: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00001da0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00001db0: 2242 6f64 7920 5465 7874 2046 6972 7374  "Body Text First
+00001dc0: 2049 6e64 656e 7422 2077 3a73 656d 6948   Indent" w:semiH
+00001dd0: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
+00001de0: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
+00001df0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00001e00: 773a 6e61 6d65 3d22 426f 6479 2054 6578  w:name="Body Tex
+00001e10: 7420 4669 7273 7420 496e 6465 6e74 2032  t First Indent 2
+00001e20: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00001e30: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00001e40: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00001e50: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00001e60: 224e 6f74 6520 4865 6164 696e 6722 2077  "Note Heading" w
+00001e70: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00001e80: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00001e90: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00001ea0: 7074 696f 6e20 773a 6e61 6d65 3d22 426f  ption w:name="Bo
+00001eb0: 6479 2054 6578 7420 3222 2077 3a73 656d  dy Text 2" w:sem
+00001ec0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
+00001ed0: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
+00001ee0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00001ef0: 6e20 773a 6e61 6d65 3d22 426f 6479 2054  n w:name="Body T
+00001f00: 6578 7420 3322 2077 3a73 656d 6948 6964  ext 3" w:semiHid
+00001f10: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
+00001f20: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
+00001f30: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00001f40: 6e61 6d65 3d22 426f 6479 2054 6578 7420  name="Body Text 
+00001f50: 496e 6465 6e74 2032 2220 773a 7365 6d69  Indent 2" w:semi
+00001f60: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
+00001f70: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
+00001f80: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00001f90: 2077 3a6e 616d 653d 2242 6f64 7920 5465   w:name="Body Te
+00001fa0: 7874 2049 6e64 656e 7420 3322 2077 3a73  xt Indent 3" w:s
+00001fb0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00001fc0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00001fd0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00001fe0: 696f 6e20 773a 6e61 6d65 3d22 426c 6f63  ion w:name="Bloc
+00001ff0: 6b20 5465 7874 2220 773a 7365 6d69 4869  k Text" w:semiHi
+00002000: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
+00002010: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
+00002020: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00002030: 3a6e 616d 653d 2248 7970 6572 6c69 6e6b  :name="Hyperlink
+00002040: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00002050: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00002060: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00002070: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00002080: 2246 6f6c 6c6f 7765 6448 7970 6572 6c69  "FollowedHyperli
+00002090: 6e6b 2220 773a 7365 6d69 4869 6464 656e  nk" w:semiHidden
+000020a0: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
+000020b0: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
+000020c0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+000020d0: 653d 2253 7472 6f6e 6722 2077 3a75 6950  e="Strong" w:uiP
+000020e0: 7269 6f72 6974 793d 2232 3222 2077 3a71  riority="22" w:q
+000020f0: 466f 726d 6174 3d22 3122 2f3e 3c77 3a6c  Format="1"/><w:l
+00002100: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00002110: 6d65 3d22 456d 7068 6173 6973 2220 773a  me="Emphasis" w:
+00002120: 7569 5072 696f 7269 7479 3d22 3230 2220  uiPriority="20" 
+00002130: 773a 7146 6f72 6d61 743d 2231 222f 3e3c  w:qFormat="1"/><
+00002140: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00002150: 3a6e 616d 653d 2244 6f63 756d 656e 7420  :name="Document 
+00002160: 4d61 7022 2077 3a73 656d 6948 6964 6465  Map" w:semiHidde
+00002170: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
+00002180: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
+00002190: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000021a0: 6d65 3d22 506c 6169 6e20 5465 7874 2220  me="Plain Text" 
+000021b0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+000021c0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+000021d0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+000021e0: 6570 7469 6f6e 2077 3a6e 616d 653d 2245  eption w:name="E
+000021f0: 2d6d 6169 6c20 5369 676e 6174 7572 6522  -mail Signature"
+00002200: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00002210: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00002220: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00002230: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00002240: 4854 4d4c 2054 6f70 206f 6620 466f 726d  HTML Top of Form
+00002250: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00002260: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00002270: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00002280: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00002290: 2248 544d 4c20 426f 7474 6f6d 206f 6620  "HTML Bottom of 
+000022a0: 466f 726d 2220 773a 7365 6d69 4869 6464  Form" w:semiHidd
+000022b0: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+000022c0: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+000022d0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000022e0: 616d 653d 224e 6f72 6d61 6c20 2857 6562  ame="Normal (Web
+000022f0: 2922 2077 3a73 656d 6948 6964 6465 6e3d  )" w:semiHidden=
+00002300: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
+00002310: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
+00002320: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00002330: 3d22 4854 4d4c 2041 6372 6f6e 796d 2220  ="HTML Acronym" 
+00002340: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00002350: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00002360: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002370: 6570 7469 6f6e 2077 3a6e 616d 653d 2248  eption w:name="H
+00002380: 544d 4c20 4164 6472 6573 7322 2077 3a73  TML Address" w:s
+00002390: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+000023a0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+000023b0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+000023c0: 696f 6e20 773a 6e61 6d65 3d22 4854 4d4c  ion w:name="HTML
+000023d0: 2043 6974 6522 2077 3a73 656d 6948 6964   Cite" w:semiHid
+000023e0: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
+000023f0: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
+00002400: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00002410: 6e61 6d65 3d22 4854 4d4c 2043 6f64 6522  name="HTML Code"
+00002420: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00002430: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00002440: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00002450: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00002460: 4854 4d4c 2044 6566 696e 6974 696f 6e22  HTML Definition"
+00002470: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00002480: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00002490: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+000024a0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000024b0: 4854 4d4c 204b 6579 626f 6172 6422 2077  HTML Keyboard" w
+000024c0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+000024d0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+000024e0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+000024f0: 7074 696f 6e20 773a 6e61 6d65 3d22 4854  ption w:name="HT
+00002500: 4d4c 2050 7265 666f 726d 6174 7465 6422  ML Preformatted"
+00002510: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00002520: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00002530: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00002540: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00002550: 4854 4d4c 2053 616d 706c 6522 2077 3a73  HTML Sample" w:s
+00002560: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00002570: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00002580: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00002590: 696f 6e20 773a 6e61 6d65 3d22 4854 4d4c  ion w:name="HTML
+000025a0: 2054 7970 6577 7269 7465 7222 2077 3a73   Typewriter" w:s
+000025b0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+000025c0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+000025d0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+000025e0: 696f 6e20 773a 6e61 6d65 3d22 4854 4d4c  ion w:name="HTML
+000025f0: 2056 6172 6961 626c 6522 2077 3a73 656d   Variable" w:sem
+00002600: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
+00002610: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
+00002620: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00002630: 6e20 773a 6e61 6d65 3d22 4e6f 726d 616c  n w:name="Normal
+00002640: 2054 6162 6c65 2220 773a 7365 6d69 4869   Table" w:semiHi
+00002650: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
+00002660: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
+00002670: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00002680: 3a6e 616d 653d 2261 6e6e 6f74 6174 696f  :name="annotatio
+00002690: 6e20 7375 626a 6563 7422 2077 3a73 656d  n subject" w:sem
+000026a0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
+000026b0: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
+000026c0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+000026d0: 6e20 773a 6e61 6d65 3d22 4e6f 204c 6973  n w:name="No Lis
+000026e0: 7422 2077 3a73 656d 6948 6964 6465 6e3d  t" w:semiHidden=
+000026f0: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
+00002700: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
+00002710: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00002720: 3d22 4f75 746c 696e 6520 4c69 7374 2031  ="Outline List 1
+00002730: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00002740: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00002750: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00002760: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00002770: 224f 7574 6c69 6e65 204c 6973 7420 3222  "Outline List 2"
+00002780: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00002790: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+000027a0: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+000027b0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000027c0: 4f75 746c 696e 6520 4c69 7374 2033 2220  Outline List 3" 
+000027d0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+000027e0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+000027f0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002800: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00002810: 6162 6c65 2053 696d 706c 6520 3122 2077  able Simple 1" w
+00002820: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00002830: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00002840: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00002850: 7074 696f 6e20 773a 6e61 6d65 3d22 5461  ption w:name="Ta
+00002860: 626c 6520 5369 6d70 6c65 2032 2220 773a  ble Simple 2" w:
+00002870: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+00002880: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00002890: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+000028a0: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
+000028b0: 6c65 2053 696d 706c 6520 3322 2077 3a73  le Simple 3" w:s
+000028c0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+000028d0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+000028e0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+000028f0: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
+00002900: 6520 436c 6173 7369 6320 3122 2077 3a73  e Classic 1" w:s
+00002910: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00002920: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00002930: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00002940: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
+00002950: 6520 436c 6173 7369 6320 3222 2077 3a73  e Classic 2" w:s
+00002960: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00002970: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00002980: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00002990: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
+000029a0: 6520 436c 6173 7369 6320 3322 2077 3a73  e Classic 3" w:s
+000029b0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+000029c0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+000029d0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+000029e0: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
+000029f0: 6520 436c 6173 7369 6320 3422 2077 3a73  e Classic 4" w:s
+00002a00: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00002a10: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00002a20: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00002a30: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
+00002a40: 6520 436f 6c6f 7266 756c 2031 2220 773a  e Colorful 1" w:
+00002a50: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+00002a60: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00002a70: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00002a80: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
+00002a90: 6c65 2043 6f6c 6f72 6675 6c20 3222 2077  le Colorful 2" w
+00002aa0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00002ab0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00002ac0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00002ad0: 7074 696f 6e20 773a 6e61 6d65 3d22 5461  ption w:name="Ta
+00002ae0: 626c 6520 436f 6c6f 7266 756c 2033 2220  ble Colorful 3" 
+00002af0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00002b00: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00002b10: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002b20: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00002b30: 6162 6c65 2043 6f6c 756d 6e73 2031 2220  able Columns 1" 
+00002b40: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00002b50: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00002b60: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002b70: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00002b80: 6162 6c65 2043 6f6c 756d 6e73 2032 2220  able Columns 2" 
+00002b90: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00002ba0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00002bb0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002bc0: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00002bd0: 6162 6c65 2043 6f6c 756d 6e73 2033 2220  able Columns 3" 
+00002be0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00002bf0: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00002c00: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002c10: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00002c20: 6162 6c65 2043 6f6c 756d 6e73 2034 2220  able Columns 4" 
+00002c30: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00002c40: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00002c50: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002c60: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00002c70: 6162 6c65 2043 6f6c 756d 6e73 2035 2220  able Columns 5" 
+00002c80: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00002c90: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00002ca0: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00002cb0: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00002cc0: 6162 6c65 2047 7269 6420 3122 2077 3a73  able Grid 1" w:s
+00002cd0: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00002ce0: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00002cf0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00002d00: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
+00002d10: 6520 4772 6964 2032 2220 773a 7365 6d69  e Grid 2" w:semi
+00002d20: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
+00002d30: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
+00002d40: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00002d50: 2077 3a6e 616d 653d 2254 6162 6c65 2047   w:name="Table G
+00002d60: 7269 6420 3322 2077 3a73 656d 6948 6964  rid 3" w:semiHid
+00002d70: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
+00002d80: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
+00002d90: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00002da0: 6e61 6d65 3d22 5461 626c 6520 4772 6964  name="Table Grid
+00002db0: 2034 2220 773a 7365 6d69 4869 6464 656e   4" w:semiHidden
+00002dc0: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
+00002dd0: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
+00002de0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00002df0: 653d 2254 6162 6c65 2047 7269 6420 3522  e="Table Grid 5"
+00002e00: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00002e10: 2220 773a 756e 6869 6465 5768 656e 5573  " w:unhideWhenUs
+00002e20: 6564 3d22 3122 2f3e 3c77 3a6c 7364 4578  ed="1"/><w:lsdEx
+00002e30: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00002e40: 5461 626c 6520 4772 6964 2036 2220 773a  Table Grid 6" w:
+00002e50: 7365 6d69 4869 6464 656e 3d22 3122 2077  semiHidden="1" w
+00002e60: 3a75 6e68 6964 6557 6865 6e55 7365 643d  :unhideWhenUsed=
+00002e70: 2231 222f 3e3c 773a 6c73 6445 7863 6570  "1"/><w:lsdExcep
+00002e80: 7469 6f6e 2077 3a6e 616d 653d 2254 6162  tion w:name="Tab
+00002e90: 6c65 2047 7269 6420 3722 2077 3a73 656d  le Grid 7" w:sem
+00002ea0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
+00002eb0: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
+00002ec0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00002ed0: 6e20 773a 6e61 6d65 3d22 5461 626c 6520  n w:name="Table 
+00002ee0: 4772 6964 2038 2220 773a 7365 6d69 4869  Grid 8" w:semiHi
+00002ef0: 6464 656e 3d22 3122 2077 3a75 6e68 6964  dden="1" w:unhid
+00002f00: 6557 6865 6e55 7365 643d 2231 222f 3e3c  eWhenUsed="1"/><
+00002f10: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00002f20: 3a6e 616d 653d 2254 6162 6c65 204c 6973  :name="Table Lis
+00002f30: 7420 3122 2077 3a73 656d 6948 6964 6465  t 1" w:semiHidde
+00002f40: 6e3d 2231 2220 773a 756e 6869 6465 5768  n="1" w:unhideWh
+00002f50: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
+00002f60: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00002f70: 6d65 3d22 5461 626c 6520 4c69 7374 2032  me="Table List 2
+00002f80: 2220 773a 7365 6d69 4869 6464 656e 3d22  " w:semiHidden="
+00002f90: 3122 2077 3a75 6e68 6964 6557 6865 6e55  1" w:unhideWhenU
+00002fa0: 7365 643d 2231 222f 3e3c 773a 6c73 6445  sed="1"/><w:lsdE
+00002fb0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00002fc0: 2254 6162 6c65 204c 6973 7420 3322 2077  "Table List 3" w
+00002fd0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00002fe0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00002ff0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00003000: 7074 696f 6e20 773a 6e61 6d65 3d22 5461  ption w:name="Ta
+00003010: 626c 6520 4c69 7374 2034 2220 773a 7365  ble List 4" w:se
+00003020: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00003030: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
+00003040: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00003050: 6f6e 2077 3a6e 616d 653d 2254 6162 6c65  on w:name="Table
+00003060: 204c 6973 7420 3522 2077 3a73 656d 6948   List 5" w:semiH
+00003070: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
+00003080: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
+00003090: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+000030a0: 773a 6e61 6d65 3d22 5461 626c 6520 4c69  w:name="Table Li
+000030b0: 7374 2036 2220 773a 7365 6d69 4869 6464  st 6" w:semiHidd
+000030c0: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+000030d0: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+000030e0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000030f0: 616d 653d 2254 6162 6c65 204c 6973 7420  ame="Table List 
+00003100: 3722 2077 3a73 656d 6948 6964 6465 6e3d  7" w:semiHidden=
+00003110: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
+00003120: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
+00003130: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00003140: 3d22 5461 626c 6520 4c69 7374 2038 2220  ="Table List 8" 
+00003150: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+00003160: 2077 3a75 6e68 6964 6557 6865 6e55 7365   w:unhideWhenUse
+00003170: 643d 2231 222f 3e3c 773a 6c73 6445 7863  d="1"/><w:lsdExc
+00003180: 6570 7469 6f6e 2077 3a6e 616d 653d 2254  eption w:name="T
+00003190: 6162 6c65 2033 4420 6566 6665 6374 7320  able 3D effects 
+000031a0: 3122 2077 3a73 656d 6948 6964 6465 6e3d  1" w:semiHidden=
+000031b0: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
+000031c0: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
+000031d0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000031e0: 3d22 5461 626c 6520 3344 2065 6666 6563  ="Table 3D effec
+000031f0: 7473 2032 2220 773a 7365 6d69 4869 6464  ts 2" w:semiHidd
+00003200: 656e 3d22 3122 2077 3a75 6e68 6964 6557  en="1" w:unhideW
+00003210: 6865 6e55 7365 643d 2231 222f 3e3c 773a  henUsed="1"/><w:
+00003220: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00003230: 616d 653d 2254 6162 6c65 2033 4420 6566  ame="Table 3D ef
+00003240: 6665 6374 7320 3322 2077 3a73 656d 6948  fects 3" w:semiH
+00003250: 6964 6465 6e3d 2231 2220 773a 756e 6869  idden="1" w:unhi
+00003260: 6465 5768 656e 5573 6564 3d22 3122 2f3e  deWhenUsed="1"/>
+00003270: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00003280: 773a 6e61 6d65 3d22 5461 626c 6520 436f  w:name="Table Co
+00003290: 6e74 656d 706f 7261 7279 2220 773a 7365  ntemporary" w:se
+000032a0: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+000032b0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
+000032c0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+000032d0: 6f6e 2077 3a6e 616d 653d 2254 6162 6c65  on w:name="Table
+000032e0: 2045 6c65 6761 6e74 2220 773a 7365 6d69   Elegant" w:semi
+000032f0: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
+00003300: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
+00003310: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00003320: 2077 3a6e 616d 653d 2254 6162 6c65 2050   w:name="Table P
+00003330: 726f 6665 7373 696f 6e61 6c22 2077 3a73  rofessional" w:s
+00003340: 656d 6948 6964 6465 6e3d 2231 2220 773a  emiHidden="1" w:
+00003350: 756e 6869 6465 5768 656e 5573 6564 3d22  unhideWhenUsed="
+00003360: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00003370: 696f 6e20 773a 6e61 6d65 3d22 5461 626c  ion w:name="Tabl
+00003380: 6520 5375 6274 6c65 2031 2220 773a 7365  e Subtle 1" w:se
+00003390: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+000033a0: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
+000033b0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+000033c0: 6f6e 2077 3a6e 616d 653d 2254 6162 6c65  on w:name="Table
+000033d0: 2053 7562 746c 6520 3222 2077 3a73 656d   Subtle 2" w:sem
+000033e0: 6948 6964 6465 6e3d 2231 2220 773a 756e  iHidden="1" w:un
+000033f0: 6869 6465 5768 656e 5573 6564 3d22 3122  hideWhenUsed="1"
+00003400: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00003410: 6e20 773a 6e61 6d65 3d22 5461 626c 6520  n w:name="Table 
+00003420: 5765 6220 3122 2077 3a73 656d 6948 6964  Web 1" w:semiHid
+00003430: 6465 6e3d 2231 2220 773a 756e 6869 6465  den="1" w:unhide
+00003440: 5768 656e 5573 6564 3d22 3122 2f3e 3c77  WhenUsed="1"/><w
+00003450: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00003460: 6e61 6d65 3d22 5461 626c 6520 5765 6220  name="Table Web 
+00003470: 3222 2077 3a73 656d 6948 6964 6465 6e3d  2" w:semiHidden=
+00003480: 2231 2220 773a 756e 6869 6465 5768 656e  "1" w:unhideWhen
+00003490: 5573 6564 3d22 3122 2f3e 3c77 3a6c 7364  Used="1"/><w:lsd
+000034a0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000034b0: 3d22 5461 626c 6520 5765 6220 3322 2077  ="Table Web 3" w
+000034c0: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+000034d0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+000034e0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+000034f0: 7074 696f 6e20 773a 6e61 6d65 3d22 4261  ption w:name="Ba
+00003500: 6c6c 6f6f 6e20 5465 7874 2220 773a 7365  lloon Text" w:se
+00003510: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00003520: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
+00003530: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00003540: 6f6e 2077 3a6e 616d 653d 2254 6162 6c65  on w:name="Table
+00003550: 2047 7269 6422 2077 3a75 6950 7269 6f72   Grid" w:uiPrior
+00003560: 6974 793d 2233 3922 2f3e 3c77 3a6c 7364  ity="39"/><w:lsd
+00003570: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00003580: 3d22 5461 626c 6520 5468 656d 6522 2077  ="Table Theme" w
+00003590: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+000035a0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+000035b0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+000035c0: 7074 696f 6e20 773a 6e61 6d65 3d22 506c  ption w:name="Pl
+000035d0: 6163 6568 6f6c 6465 7220 5465 7874 2220  aceholder Text" 
+000035e0: 773a 7365 6d69 4869 6464 656e 3d22 3122  w:semiHidden="1"
+000035f0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00003600: 6e20 773a 6e61 6d65 3d22 4e6f 2053 7061  n w:name="No Spa
+00003610: 6369 6e67 2220 773a 7569 5072 696f 7269  cing" w:uiPriori
+00003620: 7479 3d22 3122 2077 3a71 466f 726d 6174  ty="1" w:qFormat
+00003630: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00003640: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+00003650: 6768 7420 5368 6164 696e 6722 2077 3a75  ght Shading" w:u
+00003660: 6950 7269 6f72 6974 793d 2236 3022 2f3e  iPriority="60"/>
+00003670: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00003680: 773a 6e61 6d65 3d22 4c69 6768 7420 4c69  w:name="Light Li
+00003690: 7374 2220 773a 7569 5072 696f 7269 7479  st" w:uiPriority
+000036a0: 3d22 3631 222f 3e3c 773a 6c73 6445 7863  ="61"/><w:lsdExc
+000036b0: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+000036c0: 6967 6874 2047 7269 6422 2077 3a75 6950  ight Grid" w:uiP
+000036d0: 7269 6f72 6974 793d 2236 3222 2f3e 3c77  riority="62"/><w
+000036e0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+000036f0: 6e61 6d65 3d22 4d65 6469 756d 2053 6861  name="Medium Sha
+00003700: 6469 6e67 2031 2220 773a 7569 5072 696f  ding 1" w:uiPrio
+00003710: 7269 7479 3d22 3633 222f 3e3c 773a 6c73  rity="63"/><w:ls
+00003720: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00003730: 653d 224d 6564 6975 6d20 5368 6164 696e  e="Medium Shadin
+00003740: 6720 3222 2077 3a75 6950 7269 6f72 6974  g 2" w:uiPriorit
+00003750: 793d 2236 3422 2f3e 3c77 3a6c 7364 4578  y="64"/><w:lsdEx
+00003760: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00003770: 4d65 6469 756d 204c 6973 7420 3122 2077  Medium List 1" w
+00003780: 3a75 6950 7269 6f72 6974 793d 2236 3522  :uiPriority="65"
+00003790: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+000037a0: 6e20 773a 6e61 6d65 3d22 4d65 6469 756d  n w:name="Medium
+000037b0: 204c 6973 7420 3222 2077 3a75 6950 7269   List 2" w:uiPri
+000037c0: 6f72 6974 793d 2236 3622 2f3e 3c77 3a6c  ority="66"/><w:l
+000037d0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000037e0: 6d65 3d22 4d65 6469 756d 2047 7269 6420  me="Medium Grid 
+000037f0: 3122 2077 3a75 6950 7269 6f72 6974 793d  1" w:uiPriority=
+00003800: 2236 3722 2f3e 3c77 3a6c 7364 4578 6365  "67"/><w:lsdExce
+00003810: 7074 696f 6e20 773a 6e61 6d65 3d22 4d65  ption w:name="Me
+00003820: 6469 756d 2047 7269 6420 3222 2077 3a75  dium Grid 2" w:u
+00003830: 6950 7269 6f72 6974 793d 2236 3822 2f3e  iPriority="68"/>
+00003840: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00003850: 773a 6e61 6d65 3d22 4d65 6469 756d 2047  w:name="Medium G
+00003860: 7269 6420 3322 2077 3a75 6950 7269 6f72  rid 3" w:uiPrior
+00003870: 6974 793d 2236 3922 2f3e 3c77 3a6c 7364  ity="69"/><w:lsd
+00003880: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00003890: 3d22 4461 726b 204c 6973 7422 2077 3a75  ="Dark List" w:u
+000038a0: 6950 7269 6f72 6974 793d 2237 3022 2f3e  iPriority="70"/>
+000038b0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+000038c0: 773a 6e61 6d65 3d22 436f 6c6f 7266 756c  w:name="Colorful
+000038d0: 2053 6861 6469 6e67 2220 773a 7569 5072   Shading" w:uiPr
+000038e0: 696f 7269 7479 3d22 3731 222f 3e3c 773a  iority="71"/><w:
+000038f0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00003900: 616d 653d 2243 6f6c 6f72 6675 6c20 4c69  ame="Colorful Li
+00003910: 7374 2220 773a 7569 5072 696f 7269 7479  st" w:uiPriority
+00003920: 3d22 3732 222f 3e3c 773a 6c73 6445 7863  ="72"/><w:lsdExc
+00003930: 6570 7469 6f6e 2077 3a6e 616d 653d 2243  eption w:name="C
+00003940: 6f6c 6f72 6675 6c20 4772 6964 2220 773a  olorful Grid" w:
+00003950: 7569 5072 696f 7269 7479 3d22 3733 222f  uiPriority="73"/
+00003960: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00003970: 2077 3a6e 616d 653d 224c 6967 6874 2053   w:name="Light S
+00003980: 6861 6469 6e67 2041 6363 656e 7420 3122  hading Accent 1"
+00003990: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+000039a0: 3022 2f3e 3c77 3a6c 7364 4578 6365 7074  0"/><w:lsdExcept
+000039b0: 696f 6e20 773a 6e61 6d65 3d22 4c69 6768  ion w:name="Ligh
+000039c0: 7420 4c69 7374 2041 6363 656e 7420 3122  t List Accent 1"
+000039d0: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+000039e0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+000039f0: 696f 6e20 773a 6e61 6d65 3d22 4c69 6768  ion w:name="Ligh
+00003a00: 7420 4772 6964 2041 6363 656e 7420 3122  t Grid Accent 1"
+00003a10: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+00003a20: 3222 2f3e 3c77 3a6c 7364 4578 6365 7074  2"/><w:lsdExcept
+00003a30: 696f 6e20 773a 6e61 6d65 3d22 4d65 6469  ion w:name="Medi
+00003a40: 756d 2053 6861 6469 6e67 2031 2041 6363  um Shading 1 Acc
+00003a50: 656e 7420 3122 2077 3a75 6950 7269 6f72  ent 1" w:uiPrior
+00003a60: 6974 793d 2236 3322 2f3e 3c77 3a6c 7364  ity="63"/><w:lsd
+00003a70: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00003a80: 3d22 4d65 6469 756d 2053 6861 6469 6e67  ="Medium Shading
+00003a90: 2032 2041 6363 656e 7420 3122 2077 3a75   2 Accent 1" w:u
+00003aa0: 6950 7269 6f72 6974 793d 2236 3422 2f3e  iPriority="64"/>
+00003ab0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00003ac0: 773a 6e61 6d65 3d22 4d65 6469 756d 204c  w:name="Medium L
+00003ad0: 6973 7420 3120 4163 6365 6e74 2031 2220  ist 1 Accent 1" 
+00003ae0: 773a 7569 5072 696f 7269 7479 3d22 3635  w:uiPriority="65
+00003af0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00003b00: 6f6e 2077 3a6e 616d 653d 2252 6576 6973  on w:name="Revis
+00003b10: 696f 6e22 2077 3a73 656d 6948 6964 6465  ion" w:semiHidde
+00003b20: 6e3d 2231 222f 3e3c 773a 6c73 6445 7863  n="1"/><w:lsdExc
+00003b30: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00003b40: 6973 7420 5061 7261 6772 6170 6822 2077  ist Paragraph" w
+00003b50: 3a75 6950 7269 6f72 6974 793d 2233 3422  :uiPriority="34"
+00003b60: 2077 3a71 466f 726d 6174 3d22 3122 2f3e   w:qFormat="1"/>
+00003b70: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00003b80: 773a 6e61 6d65 3d22 5175 6f74 6522 2077  w:name="Quote" w
+00003b90: 3a75 6950 7269 6f72 6974 793d 2232 3922  :uiPriority="29"
+00003ba0: 2077 3a71 466f 726d 6174 3d22 3122 2f3e   w:qFormat="1"/>
+00003bb0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00003bc0: 773a 6e61 6d65 3d22 496e 7465 6e73 6520  w:name="Intense 
+00003bd0: 5175 6f74 6522 2077 3a75 6950 7269 6f72  Quote" w:uiPrior
+00003be0: 6974 793d 2233 3022 2077 3a71 466f 726d  ity="30" w:qForm
+00003bf0: 6174 3d22 3122 2f3e 3c77 3a6c 7364 4578  at="1"/><w:lsdEx
+00003c00: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00003c10: 4d65 6469 756d 204c 6973 7420 3220 4163  Medium List 2 Ac
+00003c20: 6365 6e74 2031 2220 773a 7569 5072 696f  cent 1" w:uiPrio
+00003c30: 7269 7479 3d22 3636 222f 3e3c 773a 6c73  rity="66"/><w:ls
+00003c40: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00003c50: 653d 224d 6564 6975 6d20 4772 6964 2031  e="Medium Grid 1
+00003c60: 2041 6363 656e 7420 3122 2077 3a75 6950   Accent 1" w:uiP
+00003c70: 7269 6f72 6974 793d 2236 3722 2f3e 3c77  riority="67"/><w
+00003c80: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00003c90: 6e61 6d65 3d22 4d65 6469 756d 2047 7269  name="Medium Gri
+00003ca0: 6420 3220 4163 6365 6e74 2031 2220 773a  d 2 Accent 1" w:
+00003cb0: 7569 5072 696f 7269 7479 3d22 3638 222f  uiPriority="68"/
+00003cc0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00003cd0: 2077 3a6e 616d 653d 224d 6564 6975 6d20   w:name="Medium 
+00003ce0: 4772 6964 2033 2041 6363 656e 7420 3122  Grid 3 Accent 1"
+00003cf0: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+00003d00: 3922 2f3e 3c77 3a6c 7364 4578 6365 7074  9"/><w:lsdExcept
+00003d10: 696f 6e20 773a 6e61 6d65 3d22 4461 726b  ion w:name="Dark
+00003d20: 204c 6973 7420 4163 6365 6e74 2031 2220   List Accent 1" 
+00003d30: 773a 7569 5072 696f 7269 7479 3d22 3730  w:uiPriority="70
+00003d40: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00003d50: 6f6e 2077 3a6e 616d 653d 2243 6f6c 6f72  on w:name="Color
+00003d60: 6675 6c20 5368 6164 696e 6720 4163 6365  ful Shading Acce
+00003d70: 6e74 2031 2220 773a 7569 5072 696f 7269  nt 1" w:uiPriori
+00003d80: 7479 3d22 3731 222f 3e3c 773a 6c73 6445  ty="71"/><w:lsdE
+00003d90: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00003da0: 2243 6f6c 6f72 6675 6c20 4c69 7374 2041  "Colorful List A
+00003db0: 6363 656e 7420 3122 2077 3a75 6950 7269  ccent 1" w:uiPri
+00003dc0: 6f72 6974 793d 2237 3222 2f3e 3c77 3a6c  ority="72"/><w:l
+00003dd0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00003de0: 6d65 3d22 436f 6c6f 7266 756c 2047 7269  me="Colorful Gri
+00003df0: 6420 4163 6365 6e74 2031 2220 773a 7569  d Accent 1" w:ui
+00003e00: 5072 696f 7269 7479 3d22 3733 222f 3e3c  Priority="73"/><
+00003e10: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00003e20: 3a6e 616d 653d 224c 6967 6874 2053 6861  :name="Light Sha
+00003e30: 6469 6e67 2041 6363 656e 7420 3222 2077  ding Accent 2" w
+00003e40: 3a75 6950 7269 6f72 6974 793d 2236 3022  :uiPriority="60"
+00003e50: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00003e60: 6e20 773a 6e61 6d65 3d22 4c69 6768 7420  n w:name="Light 
+00003e70: 4c69 7374 2041 6363 656e 7420 3222 2077  List Accent 2" w
+00003e80: 3a75 6950 7269 6f72 6974 793d 2236 3122  :uiPriority="61"
+00003e90: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00003ea0: 6e20 773a 6e61 6d65 3d22 4c69 6768 7420  n w:name="Light 
+00003eb0: 4772 6964 2041 6363 656e 7420 3222 2077  Grid Accent 2" w
+00003ec0: 3a75 6950 7269 6f72 6974 793d 2236 3222  :uiPriority="62"
+00003ed0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00003ee0: 6e20 773a 6e61 6d65 3d22 4d65 6469 756d  n w:name="Medium
+00003ef0: 2053 6861 6469 6e67 2031 2041 6363 656e   Shading 1 Accen
+00003f00: 7420 3222 2077 3a75 6950 7269 6f72 6974  t 2" w:uiPriorit
+00003f10: 793d 2236 3322 2f3e 3c77 3a6c 7364 4578  y="63"/><w:lsdEx
+00003f20: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00003f30: 4d65 6469 756d 2053 6861 6469 6e67 2032  Medium Shading 2
+00003f40: 2041 6363 656e 7420 3222 2077 3a75 6950   Accent 2" w:uiP
+00003f50: 7269 6f72 6974 793d 2236 3422 2f3e 3c77  riority="64"/><w
+00003f60: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00003f70: 6e61 6d65 3d22 4d65 6469 756d 204c 6973  name="Medium Lis
+00003f80: 7420 3120 4163 6365 6e74 2032 2220 773a  t 1 Accent 2" w:
+00003f90: 7569 5072 696f 7269 7479 3d22 3635 222f  uiPriority="65"/
+00003fa0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00003fb0: 2077 3a6e 616d 653d 224d 6564 6975 6d20   w:name="Medium 
+00003fc0: 4c69 7374 2032 2041 6363 656e 7420 3222  List 2 Accent 2"
+00003fd0: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+00003fe0: 3622 2f3e 3c77 3a6c 7364 4578 6365 7074  6"/><w:lsdExcept
+00003ff0: 696f 6e20 773a 6e61 6d65 3d22 4d65 6469  ion w:name="Medi
+00004000: 756d 2047 7269 6420 3120 4163 6365 6e74  um Grid 1 Accent
+00004010: 2032 2220 773a 7569 5072 696f 7269 7479   2" w:uiPriority
+00004020: 3d22 3637 222f 3e3c 773a 6c73 6445 7863  ="67"/><w:lsdExc
+00004030: 6570 7469 6f6e 2077 3a6e 616d 653d 224d  eption w:name="M
+00004040: 6564 6975 6d20 4772 6964 2032 2041 6363  edium Grid 2 Acc
+00004050: 656e 7420 3222 2077 3a75 6950 7269 6f72  ent 2" w:uiPrior
+00004060: 6974 793d 2236 3822 2f3e 3c77 3a6c 7364  ity="68"/><w:lsd
+00004070: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00004080: 3d22 4d65 6469 756d 2047 7269 6420 3320  ="Medium Grid 3 
+00004090: 4163 6365 6e74 2032 2220 773a 7569 5072  Accent 2" w:uiPr
+000040a0: 696f 7269 7479 3d22 3639 222f 3e3c 773a  iority="69"/><w:
+000040b0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000040c0: 616d 653d 2244 6172 6b20 4c69 7374 2041  ame="Dark List A
+000040d0: 6363 656e 7420 3222 2077 3a75 6950 7269  ccent 2" w:uiPri
+000040e0: 6f72 6974 793d 2237 3022 2f3e 3c77 3a6c  ority="70"/><w:l
+000040f0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00004100: 6d65 3d22 436f 6c6f 7266 756c 2053 6861  me="Colorful Sha
+00004110: 6469 6e67 2041 6363 656e 7420 3222 2077  ding Accent 2" w
+00004120: 3a75 6950 7269 6f72 6974 793d 2237 3122  :uiPriority="71"
+00004130: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00004140: 6e20 773a 6e61 6d65 3d22 436f 6c6f 7266  n w:name="Colorf
+00004150: 756c 204c 6973 7420 4163 6365 6e74 2032  ul List Accent 2
+00004160: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00004170: 3732 222f 3e3c 773a 6c73 6445 7863 6570  72"/><w:lsdExcep
+00004180: 7469 6f6e 2077 3a6e 616d 653d 2243 6f6c  tion w:name="Col
+00004190: 6f72 6675 6c20 4772 6964 2041 6363 656e  orful Grid Accen
+000041a0: 7420 3222 2077 3a75 6950 7269 6f72 6974  t 2" w:uiPriorit
+000041b0: 793d 2237 3322 2f3e 3c77 3a6c 7364 4578  y="73"/><w:lsdEx
+000041c0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000041d0: 4c69 6768 7420 5368 6164 696e 6720 4163  Light Shading Ac
+000041e0: 6365 6e74 2033 2220 773a 7569 5072 696f  cent 3" w:uiPrio
+000041f0: 7269 7479 3d22 3630 222f 3e3c 773a 6c73  rity="60"/><w:ls
+00004200: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00004210: 653d 224c 6967 6874 204c 6973 7420 4163  e="Light List Ac
+00004220: 6365 6e74 2033 2220 773a 7569 5072 696f  cent 3" w:uiPrio
+00004230: 7269 7479 3d22 3631 222f 3e3c 773a 6c73  rity="61"/><w:ls
+00004240: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00004250: 653d 224c 6967 6874 2047 7269 6420 4163  e="Light Grid Ac
+00004260: 6365 6e74 2033 2220 773a 7569 5072 696f  cent 3" w:uiPrio
+00004270: 7269 7479 3d22 3632 222f 3e3c 773a 6c73  rity="62"/><w:ls
+00004280: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00004290: 653d 224d 6564 6975 6d20 5368 6164 696e  e="Medium Shadin
+000042a0: 6720 3120 4163 6365 6e74 2033 2220 773a  g 1 Accent 3" w:
+000042b0: 7569 5072 696f 7269 7479 3d22 3633 222f  uiPriority="63"/
+000042c0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+000042d0: 2077 3a6e 616d 653d 224d 6564 6975 6d20   w:name="Medium 
+000042e0: 5368 6164 696e 6720 3220 4163 6365 6e74  Shading 2 Accent
+000042f0: 2033 2220 773a 7569 5072 696f 7269 7479   3" w:uiPriority
+00004300: 3d22 3634 222f 3e3c 773a 6c73 6445 7863  ="64"/><w:lsdExc
+00004310: 6570 7469 6f6e 2077 3a6e 616d 653d 224d  eption w:name="M
+00004320: 6564 6975 6d20 4c69 7374 2031 2041 6363  edium List 1 Acc
+00004330: 656e 7420 3322 2077 3a75 6950 7269 6f72  ent 3" w:uiPrior
+00004340: 6974 793d 2236 3522 2f3e 3c77 3a6c 7364  ity="65"/><w:lsd
+00004350: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00004360: 3d22 4d65 6469 756d 204c 6973 7420 3220  ="Medium List 2 
+00004370: 4163 6365 6e74 2033 2220 773a 7569 5072  Accent 3" w:uiPr
+00004380: 696f 7269 7479 3d22 3636 222f 3e3c 773a  iority="66"/><w:
+00004390: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000043a0: 616d 653d 224d 6564 6975 6d20 4772 6964  ame="Medium Grid
+000043b0: 2031 2041 6363 656e 7420 3322 2077 3a75   1 Accent 3" w:u
+000043c0: 6950 7269 6f72 6974 793d 2236 3722 2f3e  iPriority="67"/>
+000043d0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+000043e0: 773a 6e61 6d65 3d22 4d65 6469 756d 2047  w:name="Medium G
+000043f0: 7269 6420 3220 4163 6365 6e74 2033 2220  rid 2 Accent 3" 
+00004400: 773a 7569 5072 696f 7269 7479 3d22 3638  w:uiPriority="68
+00004410: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00004420: 6f6e 2077 3a6e 616d 653d 224d 6564 6975  on w:name="Mediu
+00004430: 6d20 4772 6964 2033 2041 6363 656e 7420  m Grid 3 Accent 
+00004440: 3322 2077 3a75 6950 7269 6f72 6974 793d  3" w:uiPriority=
+00004450: 2236 3922 2f3e 3c77 3a6c 7364 4578 6365  "69"/><w:lsdExce
+00004460: 7074 696f 6e20 773a 6e61 6d65 3d22 4461  ption w:name="Da
+00004470: 726b 204c 6973 7420 4163 6365 6e74 2033  rk List Accent 3
+00004480: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00004490: 3730 222f 3e3c 773a 6c73 6445 7863 6570  70"/><w:lsdExcep
+000044a0: 7469 6f6e 2077 3a6e 616d 653d 2243 6f6c  tion w:name="Col
+000044b0: 6f72 6675 6c20 5368 6164 696e 6720 4163  orful Shading Ac
+000044c0: 6365 6e74 2033 2220 773a 7569 5072 696f  cent 3" w:uiPrio
+000044d0: 7269 7479 3d22 3731 222f 3e3c 773a 6c73  rity="71"/><w:ls
+000044e0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+000044f0: 653d 2243 6f6c 6f72 6675 6c20 4c69 7374  e="Colorful List
+00004500: 2041 6363 656e 7420 3322 2077 3a75 6950   Accent 3" w:uiP
+00004510: 7269 6f72 6974 793d 2237 3222 2f3e 3c77  riority="72"/><w
+00004520: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00004530: 6e61 6d65 3d22 436f 6c6f 7266 756c 2047  name="Colorful G
+00004540: 7269 6420 4163 6365 6e74 2033 2220 773a  rid Accent 3" w:
+00004550: 7569 5072 696f 7269 7479 3d22 3733 222f  uiPriority="73"/
+00004560: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00004570: 2077 3a6e 616d 653d 224c 6967 6874 2053   w:name="Light S
+00004580: 6861 6469 6e67 2041 6363 656e 7420 3422  hading Accent 4"
+00004590: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+000045a0: 3022 2f3e 3c77 3a6c 7364 4578 6365 7074  0"/><w:lsdExcept
+000045b0: 696f 6e20 773a 6e61 6d65 3d22 4c69 6768  ion w:name="Ligh
+000045c0: 7420 4c69 7374 2041 6363 656e 7420 3422  t List Accent 4"
+000045d0: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+000045e0: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+000045f0: 696f 6e20 773a 6e61 6d65 3d22 4c69 6768  ion w:name="Ligh
+00004600: 7420 4772 6964 2041 6363 656e 7420 3422  t Grid Accent 4"
+00004610: 2077 3a75 6950 7269 6f72 6974 793d 2236   w:uiPriority="6
+00004620: 3222 2f3e 3c77 3a6c 7364 4578 6365 7074  2"/><w:lsdExcept
+00004630: 696f 6e20 773a 6e61 6d65 3d22 4d65 6469  ion w:name="Medi
+00004640: 756d 2053 6861 6469 6e67 2031 2041 6363  um Shading 1 Acc
+00004650: 656e 7420 3422 2077 3a75 6950 7269 6f72  ent 4" w:uiPrior
+00004660: 6974 793d 2236 3322 2f3e 3c77 3a6c 7364  ity="63"/><w:lsd
+00004670: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00004680: 3d22 4d65 6469 756d 2053 6861 6469 6e67  ="Medium Shading
+00004690: 2032 2041 6363 656e 7420 3422 2077 3a75   2 Accent 4" w:u
+000046a0: 6950 7269 6f72 6974 793d 2236 3422 2f3e  iPriority="64"/>
+000046b0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+000046c0: 773a 6e61 6d65 3d22 4d65 6469 756d 204c  w:name="Medium L
+000046d0: 6973 7420 3120 4163 6365 6e74 2034 2220  ist 1 Accent 4" 
+000046e0: 773a 7569 5072 696f 7269 7479 3d22 3635  w:uiPriority="65
+000046f0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00004700: 6f6e 2077 3a6e 616d 653d 224d 6564 6975  on w:name="Mediu
+00004710: 6d20 4c69 7374 2032 2041 6363 656e 7420  m List 2 Accent 
+00004720: 3422 2077 3a75 6950 7269 6f72 6974 793d  4" w:uiPriority=
+00004730: 2236 3622 2f3e 3c77 3a6c 7364 4578 6365  "66"/><w:lsdExce
+00004740: 7074 696f 6e20 773a 6e61 6d65 3d22 4d65  ption w:name="Me
+00004750: 6469 756d 2047 7269 6420 3120 4163 6365  dium Grid 1 Acce
+00004760: 6e74 2034 2220 773a 7569 5072 696f 7269  nt 4" w:uiPriori
+00004770: 7479 3d22 3637 222f 3e3c 773a 6c73 6445  ty="67"/><w:lsdE
+00004780: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00004790: 224d 6564 6975 6d20 4772 6964 2032 2041  "Medium Grid 2 A
+000047a0: 6363 656e 7420 3422 2077 3a75 6950 7269  ccent 4" w:uiPri
+000047b0: 6f72 6974 793d 2236 3822 2f3e 3c77 3a6c  ority="68"/><w:l
+000047c0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000047d0: 6d65 3d22 4d65 6469 756d 2047 7269 6420  me="Medium Grid 
+000047e0: 3320 4163 6365 6e74 2034 2220 773a 7569  3 Accent 4" w:ui
+000047f0: 5072 696f 7269 7479 3d22 3639 222f 3e3c  Priority="69"/><
+00004800: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00004810: 3a6e 616d 653d 2244 6172 6b20 4c69 7374  :name="Dark List
+00004820: 2041 6363 656e 7420 3422 2077 3a75 6950   Accent 4" w:uiP
+00004830: 7269 6f72 6974 793d 2237 3022 2f3e 3c77  riority="70"/><w
+00004840: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00004850: 6e61 6d65 3d22 436f 6c6f 7266 756c 2053  name="Colorful S
+00004860: 6861 6469 6e67 2041 6363 656e 7420 3422  hading Accent 4"
+00004870: 2077 3a75 6950 7269 6f72 6974 793d 2237   w:uiPriority="7
+00004880: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00004890: 696f 6e20 773a 6e61 6d65 3d22 436f 6c6f  ion w:name="Colo
+000048a0: 7266 756c 204c 6973 7420 4163 6365 6e74  rful List Accent
+000048b0: 2034 2220 773a 7569 5072 696f 7269 7479   4" w:uiPriority
+000048c0: 3d22 3732 222f 3e3c 773a 6c73 6445 7863  ="72"/><w:lsdExc
+000048d0: 6570 7469 6f6e 2077 3a6e 616d 653d 2243  eption w:name="C
+000048e0: 6f6c 6f72 6675 6c20 4772 6964 2041 6363  olorful Grid Acc
+000048f0: 656e 7420 3422 2077 3a75 6950 7269 6f72  ent 4" w:uiPrior
+00004900: 6974 793d 2237 3322 2f3e 3c77 3a6c 7364  ity="73"/><w:lsd
+00004910: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00004920: 3d22 4c69 6768 7420 5368 6164 696e 6720  ="Light Shading 
+00004930: 4163 6365 6e74 2035 2220 773a 7569 5072  Accent 5" w:uiPr
+00004940: 696f 7269 7479 3d22 3630 222f 3e3c 773a  iority="60"/><w:
+00004950: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00004960: 616d 653d 224c 6967 6874 204c 6973 7420  ame="Light List 
+00004970: 4163 6365 6e74 2035 2220 773a 7569 5072  Accent 5" w:uiPr
+00004980: 696f 7269 7479 3d22 3631 222f 3e3c 773a  iority="61"/><w:
+00004990: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000049a0: 616d 653d 224c 6967 6874 2047 7269 6420  ame="Light Grid 
+000049b0: 4163 6365 6e74 2035 2220 773a 7569 5072  Accent 5" w:uiPr
+000049c0: 696f 7269 7479 3d22 3632 222f 3e3c 773a  iority="62"/><w:
+000049d0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000049e0: 616d 653d 224d 6564 6975 6d20 5368 6164  ame="Medium Shad
+000049f0: 696e 6720 3120 4163 6365 6e74 2035 2220  ing 1 Accent 5" 
+00004a00: 773a 7569 5072 696f 7269 7479 3d22 3633  w:uiPriority="63
+00004a10: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00004a20: 6f6e 2077 3a6e 616d 653d 224d 6564 6975  on w:name="Mediu
+00004a30: 6d20 5368 6164 696e 6720 3220 4163 6365  m Shading 2 Acce
+00004a40: 6e74 2035 2220 773a 7569 5072 696f 7269  nt 5" w:uiPriori
+00004a50: 7479 3d22 3634 222f 3e3c 773a 6c73 6445  ty="64"/><w:lsdE
+00004a60: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00004a70: 224d 6564 6975 6d20 4c69 7374 2031 2041  "Medium List 1 A
+00004a80: 6363 656e 7420 3522 2077 3a75 6950 7269  ccent 5" w:uiPri
+00004a90: 6f72 6974 793d 2236 3522 2f3e 3c77 3a6c  ority="65"/><w:l
+00004aa0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00004ab0: 6d65 3d22 4d65 6469 756d 204c 6973 7420  me="Medium List 
+00004ac0: 3220 4163 6365 6e74 2035 2220 773a 7569  2 Accent 5" w:ui
+00004ad0: 5072 696f 7269 7479 3d22 3636 222f 3e3c  Priority="66"/><
+00004ae0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00004af0: 3a6e 616d 653d 224d 6564 6975 6d20 4772  :name="Medium Gr
+00004b00: 6964 2031 2041 6363 656e 7420 3522 2077  id 1 Accent 5" w
+00004b10: 3a75 6950 7269 6f72 6974 793d 2236 3722  :uiPriority="67"
+00004b20: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00004b30: 6e20 773a 6e61 6d65 3d22 4d65 6469 756d  n w:name="Medium
+00004b40: 2047 7269 6420 3220 4163 6365 6e74 2035   Grid 2 Accent 5
+00004b50: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00004b60: 3638 222f 3e3c 773a 6c73 6445 7863 6570  68"/><w:lsdExcep
+00004b70: 7469 6f6e 2077 3a6e 616d 653d 224d 6564  tion w:name="Med
+00004b80: 6975 6d20 4772 6964 2033 2041 6363 656e  ium Grid 3 Accen
+00004b90: 7420 3522 2077 3a75 6950 7269 6f72 6974  t 5" w:uiPriorit
+00004ba0: 793d 2236 3922 2f3e 3c77 3a6c 7364 4578  y="69"/><w:lsdEx
+00004bb0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00004bc0: 4461 726b 204c 6973 7420 4163 6365 6e74  Dark List Accent
+00004bd0: 2035 2220 773a 7569 5072 696f 7269 7479   5" w:uiPriority
+00004be0: 3d22 3730 222f 3e3c 773a 6c73 6445 7863  ="70"/><w:lsdExc
+00004bf0: 6570 7469 6f6e 2077 3a6e 616d 653d 2243  eption w:name="C
+00004c00: 6f6c 6f72 6675 6c20 5368 6164 696e 6720  olorful Shading 
+00004c10: 4163 6365 6e74 2035 2220 773a 7569 5072  Accent 5" w:uiPr
+00004c20: 696f 7269 7479 3d22 3731 222f 3e3c 773a  iority="71"/><w:
+00004c30: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00004c40: 616d 653d 2243 6f6c 6f72 6675 6c20 4c69  ame="Colorful Li
+00004c50: 7374 2041 6363 656e 7420 3522 2077 3a75  st Accent 5" w:u
+00004c60: 6950 7269 6f72 6974 793d 2237 3222 2f3e  iPriority="72"/>
+00004c70: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00004c80: 773a 6e61 6d65 3d22 436f 6c6f 7266 756c  w:name="Colorful
+00004c90: 2047 7269 6420 4163 6365 6e74 2035 2220   Grid Accent 5" 
+00004ca0: 773a 7569 5072 696f 7269 7479 3d22 3733  w:uiPriority="73
+00004cb0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00004cc0: 6f6e 2077 3a6e 616d 653d 224c 6967 6874  on w:name="Light
+00004cd0: 2053 6861 6469 6e67 2041 6363 656e 7420   Shading Accent 
+00004ce0: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
+00004cf0: 2236 3022 2f3e 3c77 3a6c 7364 4578 6365  "60"/><w:lsdExce
+00004d00: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+00004d10: 6768 7420 4c69 7374 2041 6363 656e 7420  ght List Accent 
+00004d20: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
+00004d30: 2236 3122 2f3e 3c77 3a6c 7364 4578 6365  "61"/><w:lsdExce
+00004d40: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+00004d50: 6768 7420 4772 6964 2041 6363 656e 7420  ght Grid Accent 
+00004d60: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
+00004d70: 2236 3222 2f3e 3c77 3a6c 7364 4578 6365  "62"/><w:lsdExce
+00004d80: 7074 696f 6e20 773a 6e61 6d65 3d22 4d65  ption w:name="Me
+00004d90: 6469 756d 2053 6861 6469 6e67 2031 2041  dium Shading 1 A
+00004da0: 6363 656e 7420 3622 2077 3a75 6950 7269  ccent 6" w:uiPri
+00004db0: 6f72 6974 793d 2236 3322 2f3e 3c77 3a6c  ority="63"/><w:l
+00004dc0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00004dd0: 6d65 3d22 4d65 6469 756d 2053 6861 6469  me="Medium Shadi
+00004de0: 6e67 2032 2041 6363 656e 7420 3622 2077  ng 2 Accent 6" w
+00004df0: 3a75 6950 7269 6f72 6974 793d 2236 3422  :uiPriority="64"
+00004e00: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00004e10: 6e20 773a 6e61 6d65 3d22 4d65 6469 756d  n w:name="Medium
+00004e20: 204c 6973 7420 3120 4163 6365 6e74 2036   List 1 Accent 6
+00004e30: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00004e40: 3635 222f 3e3c 773a 6c73 6445 7863 6570  65"/><w:lsdExcep
+00004e50: 7469 6f6e 2077 3a6e 616d 653d 224d 6564  tion w:name="Med
+00004e60: 6975 6d20 4c69 7374 2032 2041 6363 656e  ium List 2 Accen
+00004e70: 7420 3622 2077 3a75 6950 7269 6f72 6974  t 6" w:uiPriorit
+00004e80: 793d 2236 3622 2f3e 3c77 3a6c 7364 4578  y="66"/><w:lsdEx
+00004e90: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00004ea0: 4d65 6469 756d 2047 7269 6420 3120 4163  Medium Grid 1 Ac
+00004eb0: 6365 6e74 2036 2220 773a 7569 5072 696f  cent 6" w:uiPrio
+00004ec0: 7269 7479 3d22 3637 222f 3e3c 773a 6c73  rity="67"/><w:ls
+00004ed0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00004ee0: 653d 224d 6564 6975 6d20 4772 6964 2032  e="Medium Grid 2
+00004ef0: 2041 6363 656e 7420 3622 2077 3a75 6950   Accent 6" w:uiP
+00004f00: 7269 6f72 6974 793d 2236 3822 2f3e 3c77  riority="68"/><w
+00004f10: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00004f20: 6e61 6d65 3d22 4d65 6469 756d 2047 7269  name="Medium Gri
+00004f30: 6420 3320 4163 6365 6e74 2036 2220 773a  d 3 Accent 6" w:
+00004f40: 7569 5072 696f 7269 7479 3d22 3639 222f  uiPriority="69"/
+00004f50: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00004f60: 2077 3a6e 616d 653d 2244 6172 6b20 4c69   w:name="Dark Li
+00004f70: 7374 2041 6363 656e 7420 3622 2077 3a75  st Accent 6" w:u
+00004f80: 6950 7269 6f72 6974 793d 2237 3022 2f3e  iPriority="70"/>
+00004f90: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00004fa0: 773a 6e61 6d65 3d22 436f 6c6f 7266 756c  w:name="Colorful
+00004fb0: 2053 6861 6469 6e67 2041 6363 656e 7420   Shading Accent 
+00004fc0: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
+00004fd0: 2237 3122 2f3e 3c77 3a6c 7364 4578 6365  "71"/><w:lsdExce
+00004fe0: 7074 696f 6e20 773a 6e61 6d65 3d22 436f  ption w:name="Co
+00004ff0: 6c6f 7266 756c 204c 6973 7420 4163 6365  lorful List Acce
+00005000: 6e74 2036 2220 773a 7569 5072 696f 7269  nt 6" w:uiPriori
+00005010: 7479 3d22 3732 222f 3e3c 773a 6c73 6445  ty="72"/><w:lsdE
+00005020: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00005030: 2243 6f6c 6f72 6675 6c20 4772 6964 2041  "Colorful Grid A
+00005040: 6363 656e 7420 3622 2077 3a75 6950 7269  ccent 6" w:uiPri
+00005050: 6f72 6974 793d 2237 3322 2f3e 3c77 3a6c  ority="73"/><w:l
+00005060: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00005070: 6d65 3d22 5375 6274 6c65 2045 6d70 6861  me="Subtle Empha
+00005080: 7369 7322 2077 3a75 6950 7269 6f72 6974  sis" w:uiPriorit
+00005090: 793d 2231 3922 2077 3a71 466f 726d 6174  y="19" w:qFormat
+000050a0: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+000050b0: 7074 696f 6e20 773a 6e61 6d65 3d22 496e  ption w:name="In
+000050c0: 7465 6e73 6520 456d 7068 6173 6973 2220  tense Emphasis" 
+000050d0: 773a 7569 5072 696f 7269 7479 3d22 3231  w:uiPriority="21
+000050e0: 2220 773a 7146 6f72 6d61 743d 2231 222f  " w:qFormat="1"/
+000050f0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00005100: 2077 3a6e 616d 653d 2253 7562 746c 6520   w:name="Subtle 
+00005110: 5265 6665 7265 6e63 6522 2077 3a75 6950  Reference" w:uiP
+00005120: 7269 6f72 6974 793d 2233 3122 2077 3a71  riority="31" w:q
+00005130: 466f 726d 6174 3d22 3122 2f3e 3c77 3a6c  Format="1"/><w:l
+00005140: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00005150: 6d65 3d22 496e 7465 6e73 6520 5265 6665  me="Intense Refe
+00005160: 7265 6e63 6522 2077 3a75 6950 7269 6f72  rence" w:uiPrior
+00005170: 6974 793d 2233 3222 2077 3a71 466f 726d  ity="32" w:qForm
+00005180: 6174 3d22 3122 2f3e 3c77 3a6c 7364 4578  at="1"/><w:lsdEx
+00005190: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000051a0: 426f 6f6b 2054 6974 6c65 2220 773a 7569  Book Title" w:ui
+000051b0: 5072 696f 7269 7479 3d22 3333 2220 773a  Priority="33" w:
+000051c0: 7146 6f72 6d61 743d 2231 222f 3e3c 773a  qFormat="1"/><w:
+000051d0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000051e0: 616d 653d 2242 6962 6c69 6f67 7261 7068  ame="Bibliograph
+000051f0: 7922 2077 3a73 656d 6948 6964 6465 6e3d  y" w:semiHidden=
+00005200: 2231 2220 773a 7569 5072 696f 7269 7479  "1" w:uiPriority
+00005210: 3d22 3337 2220 773a 756e 6869 6465 5768  ="37" w:unhideWh
+00005220: 656e 5573 6564 3d22 3122 2f3e 3c77 3a6c  enUsed="1"/><w:l
+00005230: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00005240: 6d65 3d22 544f 4320 4865 6164 696e 6722  me="TOC Heading"
+00005250: 2077 3a73 656d 6948 6964 6465 6e3d 2231   w:semiHidden="1
+00005260: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00005270: 3339 2220 773a 756e 6869 6465 5768 656e  39" w:unhideWhen
+00005280: 5573 6564 3d22 3122 2077 3a71 466f 726d  Used="1" w:qForm
+00005290: 6174 3d22 3122 2f3e 3c77 3a6c 7364 4578  at="1"/><w:lsdEx
+000052a0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000052b0: 506c 6169 6e20 5461 626c 6520 3122 2077  Plain Table 1" w
+000052c0: 3a75 6950 7269 6f72 6974 793d 2234 3122  :uiPriority="41"
+000052d0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+000052e0: 6e20 773a 6e61 6d65 3d22 506c 6169 6e20  n w:name="Plain 
+000052f0: 5461 626c 6520 3222 2077 3a75 6950 7269  Table 2" w:uiPri
+00005300: 6f72 6974 793d 2234 3222 2f3e 3c77 3a6c  ority="42"/><w:l
+00005310: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00005320: 6d65 3d22 506c 6169 6e20 5461 626c 6520  me="Plain Table 
+00005330: 3322 2077 3a75 6950 7269 6f72 6974 793d  3" w:uiPriority=
+00005340: 2234 3322 2f3e 3c77 3a6c 7364 4578 6365  "43"/><w:lsdExce
+00005350: 7074 696f 6e20 773a 6e61 6d65 3d22 506c  ption w:name="Pl
+00005360: 6169 6e20 5461 626c 6520 3422 2077 3a75  ain Table 4" w:u
+00005370: 6950 7269 6f72 6974 793d 2234 3422 2f3e  iPriority="44"/>
+00005380: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00005390: 773a 6e61 6d65 3d22 506c 6169 6e20 5461  w:name="Plain Ta
+000053a0: 626c 6520 3522 2077 3a75 6950 7269 6f72  ble 5" w:uiPrior
+000053b0: 6974 793d 2234 3522 2f3e 3c77 3a6c 7364  ity="45"/><w:lsd
+000053c0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000053d0: 3d22 4772 6964 2054 6162 6c65 204c 6967  ="Grid Table Lig
+000053e0: 6874 2220 773a 7569 5072 696f 7269 7479  ht" w:uiPriority
+000053f0: 3d22 3430 222f 3e3c 773a 6c73 6445 7863  ="40"/><w:lsdExc
+00005400: 6570 7469 6f6e 2077 3a6e 616d 653d 2247  eption w:name="G
+00005410: 7269 6420 5461 626c 6520 3120 4c69 6768  rid Table 1 Ligh
+00005420: 7422 2077 3a75 6950 7269 6f72 6974 793d  t" w:uiPriority=
+00005430: 2234 3622 2f3e 3c77 3a6c 7364 4578 6365  "46"/><w:lsdExce
+00005440: 7074 696f 6e20 773a 6e61 6d65 3d22 4772  ption w:name="Gr
+00005450: 6964 2054 6162 6c65 2032 2220 773a 7569  id Table 2" w:ui
+00005460: 5072 696f 7269 7479 3d22 3437 222f 3e3c  Priority="47"/><
+00005470: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00005480: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
+00005490: 6520 3322 2077 3a75 6950 7269 6f72 6974  e 3" w:uiPriorit
+000054a0: 793d 2234 3822 2f3e 3c77 3a6c 7364 4578  y="48"/><w:lsdEx
+000054b0: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000054c0: 4772 6964 2054 6162 6c65 2034 2220 773a  Grid Table 4" w:
+000054d0: 7569 5072 696f 7269 7479 3d22 3439 222f  uiPriority="49"/
+000054e0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+000054f0: 2077 3a6e 616d 653d 2247 7269 6420 5461   w:name="Grid Ta
+00005500: 626c 6520 3520 4461 726b 2220 773a 7569  ble 5 Dark" w:ui
+00005510: 5072 696f 7269 7479 3d22 3530 222f 3e3c  Priority="50"/><
+00005520: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00005530: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
+00005540: 6520 3620 436f 6c6f 7266 756c 2220 773a  e 6 Colorful" w:
+00005550: 7569 5072 696f 7269 7479 3d22 3531 222f  uiPriority="51"/
+00005560: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00005570: 2077 3a6e 616d 653d 2247 7269 6420 5461   w:name="Grid Ta
+00005580: 626c 6520 3720 436f 6c6f 7266 756c 2220  ble 7 Colorful" 
+00005590: 773a 7569 5072 696f 7269 7479 3d22 3532  w:uiPriority="52
+000055a0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+000055b0: 6f6e 2077 3a6e 616d 653d 2247 7269 6420  on w:name="Grid 
+000055c0: 5461 626c 6520 3120 4c69 6768 7420 4163  Table 1 Light Ac
+000055d0: 6365 6e74 2031 2220 773a 7569 5072 696f  cent 1" w:uiPrio
+000055e0: 7269 7479 3d22 3436 222f 3e3c 773a 6c73  rity="46"/><w:ls
+000055f0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00005600: 653d 2247 7269 6420 5461 626c 6520 3220  e="Grid Table 2 
+00005610: 4163 6365 6e74 2031 2220 773a 7569 5072  Accent 1" w:uiPr
+00005620: 696f 7269 7479 3d22 3437 222f 3e3c 773a  iority="47"/><w:
+00005630: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00005640: 616d 653d 2247 7269 6420 5461 626c 6520  ame="Grid Table 
+00005650: 3320 4163 6365 6e74 2031 2220 773a 7569  3 Accent 1" w:ui
+00005660: 5072 696f 7269 7479 3d22 3438 222f 3e3c  Priority="48"/><
+00005670: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00005680: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
+00005690: 6520 3420 4163 6365 6e74 2031 2220 773a  e 4 Accent 1" w:
+000056a0: 7569 5072 696f 7269 7479 3d22 3439 222f  uiPriority="49"/
+000056b0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+000056c0: 2077 3a6e 616d 653d 2247 7269 6420 5461   w:name="Grid Ta
+000056d0: 626c 6520 3520 4461 726b 2041 6363 656e  ble 5 Dark Accen
+000056e0: 7420 3122 2077 3a75 6950 7269 6f72 6974  t 1" w:uiPriorit
+000056f0: 793d 2235 3022 2f3e 3c77 3a6c 7364 4578  y="50"/><w:lsdEx
+00005700: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00005710: 4772 6964 2054 6162 6c65 2036 2043 6f6c  Grid Table 6 Col
+00005720: 6f72 6675 6c20 4163 6365 6e74 2031 2220  orful Accent 1" 
+00005730: 773a 7569 5072 696f 7269 7479 3d22 3531  w:uiPriority="51
+00005740: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00005750: 6f6e 2077 3a6e 616d 653d 2247 7269 6420  on w:name="Grid 
+00005760: 5461 626c 6520 3720 436f 6c6f 7266 756c  Table 7 Colorful
+00005770: 2041 6363 656e 7420 3122 2077 3a75 6950   Accent 1" w:uiP
+00005780: 7269 6f72 6974 793d 2235 3222 2f3e 3c77  riority="52"/><w
+00005790: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+000057a0: 6e61 6d65 3d22 4772 6964 2054 6162 6c65  name="Grid Table
+000057b0: 2031 204c 6967 6874 2041 6363 656e 7420   1 Light Accent 
+000057c0: 3222 2077 3a75 6950 7269 6f72 6974 793d  2" w:uiPriority=
+000057d0: 2234 3622 2f3e 3c77 3a6c 7364 4578 6365  "46"/><w:lsdExce
+000057e0: 7074 696f 6e20 773a 6e61 6d65 3d22 4772  ption w:name="Gr
+000057f0: 6964 2054 6162 6c65 2032 2041 6363 656e  id Table 2 Accen
+00005800: 7420 3222 2077 3a75 6950 7269 6f72 6974  t 2" w:uiPriorit
+00005810: 793d 2234 3722 2f3e 3c77 3a6c 7364 4578  y="47"/><w:lsdEx
+00005820: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00005830: 4772 6964 2054 6162 6c65 2033 2041 6363  Grid Table 3 Acc
+00005840: 656e 7420 3222 2077 3a75 6950 7269 6f72  ent 2" w:uiPrior
+00005850: 6974 793d 2234 3822 2f3e 3c77 3a6c 7364  ity="48"/><w:lsd
+00005860: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00005870: 3d22 4772 6964 2054 6162 6c65 2034 2041  ="Grid Table 4 A
+00005880: 6363 656e 7420 3222 2077 3a75 6950 7269  ccent 2" w:uiPri
+00005890: 6f72 6974 793d 2234 3922 2f3e 3c77 3a6c  ority="49"/><w:l
+000058a0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000058b0: 6d65 3d22 4772 6964 2054 6162 6c65 2035  me="Grid Table 5
+000058c0: 2044 6172 6b20 4163 6365 6e74 2032 2220   Dark Accent 2" 
+000058d0: 773a 7569 5072 696f 7269 7479 3d22 3530  w:uiPriority="50
+000058e0: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+000058f0: 6f6e 2077 3a6e 616d 653d 2247 7269 6420  on w:name="Grid 
+00005900: 5461 626c 6520 3620 436f 6c6f 7266 756c  Table 6 Colorful
+00005910: 2041 6363 656e 7420 3222 2077 3a75 6950   Accent 2" w:uiP
+00005920: 7269 6f72 6974 793d 2235 3122 2f3e 3c77  riority="51"/><w
+00005930: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00005940: 6e61 6d65 3d22 4772 6964 2054 6162 6c65  name="Grid Table
+00005950: 2037 2043 6f6c 6f72 6675 6c20 4163 6365   7 Colorful Acce
+00005960: 6e74 2032 2220 773a 7569 5072 696f 7269  nt 2" w:uiPriori
+00005970: 7479 3d22 3532 222f 3e3c 773a 6c73 6445  ty="52"/><w:lsdE
+00005980: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00005990: 2247 7269 6420 5461 626c 6520 3120 4c69  "Grid Table 1 Li
+000059a0: 6768 7420 4163 6365 6e74 2033 2220 773a  ght Accent 3" w:
+000059b0: 7569 5072 696f 7269 7479 3d22 3436 222f  uiPriority="46"/
+000059c0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+000059d0: 2077 3a6e 616d 653d 2247 7269 6420 5461   w:name="Grid Ta
+000059e0: 626c 6520 3220 4163 6365 6e74 2033 2220  ble 2 Accent 3" 
+000059f0: 773a 7569 5072 696f 7269 7479 3d22 3437  w:uiPriority="47
+00005a00: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00005a10: 6f6e 2077 3a6e 616d 653d 2247 7269 6420  on w:name="Grid 
+00005a20: 5461 626c 6520 3320 4163 6365 6e74 2033  Table 3 Accent 3
+00005a30: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00005a40: 3438 222f 3e3c 773a 6c73 6445 7863 6570  48"/><w:lsdExcep
+00005a50: 7469 6f6e 2077 3a6e 616d 653d 2247 7269  tion w:name="Gri
+00005a60: 6420 5461 626c 6520 3420 4163 6365 6e74  d Table 4 Accent
+00005a70: 2033 2220 773a 7569 5072 696f 7269 7479   3" w:uiPriority
+00005a80: 3d22 3439 222f 3e3c 773a 6c73 6445 7863  ="49"/><w:lsdExc
+00005a90: 6570 7469 6f6e 2077 3a6e 616d 653d 2247  eption w:name="G
+00005aa0: 7269 6420 5461 626c 6520 3520 4461 726b  rid Table 5 Dark
+00005ab0: 2041 6363 656e 7420 3322 2077 3a75 6950   Accent 3" w:uiP
+00005ac0: 7269 6f72 6974 793d 2235 3022 2f3e 3c77  riority="50"/><w
+00005ad0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00005ae0: 6e61 6d65 3d22 4772 6964 2054 6162 6c65  name="Grid Table
+00005af0: 2036 2043 6f6c 6f72 6675 6c20 4163 6365   6 Colorful Acce
+00005b00: 6e74 2033 2220 773a 7569 5072 696f 7269  nt 3" w:uiPriori
+00005b10: 7479 3d22 3531 222f 3e3c 773a 6c73 6445  ty="51"/><w:lsdE
+00005b20: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00005b30: 2247 7269 6420 5461 626c 6520 3720 436f  "Grid Table 7 Co
+00005b40: 6c6f 7266 756c 2041 6363 656e 7420 3322  lorful Accent 3"
+00005b50: 2077 3a75 6950 7269 6f72 6974 793d 2235   w:uiPriority="5
+00005b60: 3222 2f3e 3c77 3a6c 7364 4578 6365 7074  2"/><w:lsdExcept
+00005b70: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
+00005b80: 2054 6162 6c65 2031 204c 6967 6874 2041   Table 1 Light A
+00005b90: 6363 656e 7420 3422 2077 3a75 6950 7269  ccent 4" w:uiPri
+00005ba0: 6f72 6974 793d 2234 3622 2f3e 3c77 3a6c  ority="46"/><w:l
+00005bb0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00005bc0: 6d65 3d22 4772 6964 2054 6162 6c65 2032  me="Grid Table 2
+00005bd0: 2041 6363 656e 7420 3422 2077 3a75 6950   Accent 4" w:uiP
+00005be0: 7269 6f72 6974 793d 2234 3722 2f3e 3c77  riority="47"/><w
+00005bf0: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00005c00: 6e61 6d65 3d22 4772 6964 2054 6162 6c65  name="Grid Table
+00005c10: 2033 2041 6363 656e 7420 3422 2077 3a75   3 Accent 4" w:u
+00005c20: 6950 7269 6f72 6974 793d 2234 3822 2f3e  iPriority="48"/>
+00005c30: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00005c40: 773a 6e61 6d65 3d22 4772 6964 2054 6162  w:name="Grid Tab
+00005c50: 6c65 2034 2041 6363 656e 7420 3422 2077  le 4 Accent 4" w
+00005c60: 3a75 6950 7269 6f72 6974 793d 2234 3922  :uiPriority="49"
+00005c70: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00005c80: 6e20 773a 6e61 6d65 3d22 4772 6964 2054  n w:name="Grid T
+00005c90: 6162 6c65 2035 2044 6172 6b20 4163 6365  able 5 Dark Acce
+00005ca0: 6e74 2034 2220 773a 7569 5072 696f 7269  nt 4" w:uiPriori
+00005cb0: 7479 3d22 3530 222f 3e3c 773a 6c73 6445  ty="50"/><w:lsdE
+00005cc0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00005cd0: 2247 7269 6420 5461 626c 6520 3620 436f  "Grid Table 6 Co
+00005ce0: 6c6f 7266 756c 2041 6363 656e 7420 3422  lorful Accent 4"
+00005cf0: 2077 3a75 6950 7269 6f72 6974 793d 2235   w:uiPriority="5
+00005d00: 3122 2f3e 3c77 3a6c 7364 4578 6365 7074  1"/><w:lsdExcept
+00005d10: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
+00005d20: 2054 6162 6c65 2037 2043 6f6c 6f72 6675   Table 7 Colorfu
+00005d30: 6c20 4163 6365 6e74 2034 2220 773a 7569  l Accent 4" w:ui
+00005d40: 5072 696f 7269 7479 3d22 3532 222f 3e3c  Priority="52"/><
+00005d50: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00005d60: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
+00005d70: 6520 3120 4c69 6768 7420 4163 6365 6e74  e 1 Light Accent
+00005d80: 2035 2220 773a 7569 5072 696f 7269 7479   5" w:uiPriority
+00005d90: 3d22 3436 222f 3e3c 773a 6c73 6445 7863  ="46"/><w:lsdExc
+00005da0: 6570 7469 6f6e 2077 3a6e 616d 653d 2247  eption w:name="G
+00005db0: 7269 6420 5461 626c 6520 3220 4163 6365  rid Table 2 Acce
+00005dc0: 6e74 2035 2220 773a 7569 5072 696f 7269  nt 5" w:uiPriori
+00005dd0: 7479 3d22 3437 222f 3e3c 773a 6c73 6445  ty="47"/><w:lsdE
+00005de0: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00005df0: 2247 7269 6420 5461 626c 6520 3320 4163  "Grid Table 3 Ac
+00005e00: 6365 6e74 2035 2220 773a 7569 5072 696f  cent 5" w:uiPrio
+00005e10: 7269 7479 3d22 3438 222f 3e3c 773a 6c73  rity="48"/><w:ls
+00005e20: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00005e30: 653d 2247 7269 6420 5461 626c 6520 3420  e="Grid Table 4 
+00005e40: 4163 6365 6e74 2035 2220 773a 7569 5072  Accent 5" w:uiPr
+00005e50: 696f 7269 7479 3d22 3439 222f 3e3c 773a  iority="49"/><w:
+00005e60: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00005e70: 616d 653d 2247 7269 6420 5461 626c 6520  ame="Grid Table 
+00005e80: 3520 4461 726b 2041 6363 656e 7420 3522  5 Dark Accent 5"
+00005e90: 2077 3a75 6950 7269 6f72 6974 793d 2235   w:uiPriority="5
+00005ea0: 3022 2f3e 3c77 3a6c 7364 4578 6365 7074  0"/><w:lsdExcept
+00005eb0: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
+00005ec0: 2054 6162 6c65 2036 2043 6f6c 6f72 6675   Table 6 Colorfu
+00005ed0: 6c20 4163 6365 6e74 2035 2220 773a 7569  l Accent 5" w:ui
+00005ee0: 5072 696f 7269 7479 3d22 3531 222f 3e3c  Priority="51"/><
+00005ef0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00005f00: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
+00005f10: 6520 3720 436f 6c6f 7266 756c 2041 6363  e 7 Colorful Acc
+00005f20: 656e 7420 3522 2077 3a75 6950 7269 6f72  ent 5" w:uiPrior
+00005f30: 6974 793d 2235 3222 2f3e 3c77 3a6c 7364  ity="52"/><w:lsd
+00005f40: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+00005f50: 3d22 4772 6964 2054 6162 6c65 2031 204c  ="Grid Table 1 L
+00005f60: 6967 6874 2041 6363 656e 7420 3622 2077  ight Accent 6" w
+00005f70: 3a75 6950 7269 6f72 6974 793d 2234 3622  :uiPriority="46"
+00005f80: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00005f90: 6e20 773a 6e61 6d65 3d22 4772 6964 2054  n w:name="Grid T
+00005fa0: 6162 6c65 2032 2041 6363 656e 7420 3622  able 2 Accent 6"
+00005fb0: 2077 3a75 6950 7269 6f72 6974 793d 2234   w:uiPriority="4
+00005fc0: 3722 2f3e 3c77 3a6c 7364 4578 6365 7074  7"/><w:lsdExcept
+00005fd0: 696f 6e20 773a 6e61 6d65 3d22 4772 6964  ion w:name="Grid
+00005fe0: 2054 6162 6c65 2033 2041 6363 656e 7420   Table 3 Accent 
+00005ff0: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
+00006000: 2234 3822 2f3e 3c77 3a6c 7364 4578 6365  "48"/><w:lsdExce
+00006010: 7074 696f 6e20 773a 6e61 6d65 3d22 4772  ption w:name="Gr
+00006020: 6964 2054 6162 6c65 2034 2041 6363 656e  id Table 4 Accen
+00006030: 7420 3622 2077 3a75 6950 7269 6f72 6974  t 6" w:uiPriorit
+00006040: 793d 2234 3922 2f3e 3c77 3a6c 7364 4578  y="49"/><w:lsdEx
+00006050: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00006060: 4772 6964 2054 6162 6c65 2035 2044 6172  Grid Table 5 Dar
+00006070: 6b20 4163 6365 6e74 2036 2220 773a 7569  k Accent 6" w:ui
+00006080: 5072 696f 7269 7479 3d22 3530 222f 3e3c  Priority="50"/><
+00006090: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+000060a0: 3a6e 616d 653d 2247 7269 6420 5461 626c  :name="Grid Tabl
+000060b0: 6520 3620 436f 6c6f 7266 756c 2041 6363  e 6 Colorful Acc
+000060c0: 656e 7420 3622 2077 3a75 6950 7269 6f72  ent 6" w:uiPrior
+000060d0: 6974 793d 2235 3122 2f3e 3c77 3a6c 7364  ity="51"/><w:lsd
+000060e0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000060f0: 3d22 4772 6964 2054 6162 6c65 2037 2043  ="Grid Table 7 C
+00006100: 6f6c 6f72 6675 6c20 4163 6365 6e74 2036  olorful Accent 6
+00006110: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00006120: 3532 222f 3e3c 773a 6c73 6445 7863 6570  52"/><w:lsdExcep
+00006130: 7469 6f6e 2077 3a6e 616d 653d 224c 6973  tion w:name="Lis
+00006140: 7420 5461 626c 6520 3120 4c69 6768 7422  t Table 1 Light"
+00006150: 2077 3a75 6950 7269 6f72 6974 793d 2234   w:uiPriority="4
+00006160: 3622 2f3e 3c77 3a6c 7364 4578 6365 7074  6"/><w:lsdExcept
+00006170: 696f 6e20 773a 6e61 6d65 3d22 4c69 7374  ion w:name="List
+00006180: 2054 6162 6c65 2032 2220 773a 7569 5072   Table 2" w:uiPr
+00006190: 696f 7269 7479 3d22 3437 222f 3e3c 773a  iority="47"/><w:
+000061a0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000061b0: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
+000061c0: 3322 2077 3a75 6950 7269 6f72 6974 793d  3" w:uiPriority=
+000061d0: 2234 3822 2f3e 3c77 3a6c 7364 4578 6365  "48"/><w:lsdExce
+000061e0: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+000061f0: 7374 2054 6162 6c65 2034 2220 773a 7569  st Table 4" w:ui
+00006200: 5072 696f 7269 7479 3d22 3439 222f 3e3c  Priority="49"/><
+00006210: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00006220: 3a6e 616d 653d 224c 6973 7420 5461 626c  :name="List Tabl
+00006230: 6520 3520 4461 726b 2220 773a 7569 5072  e 5 Dark" w:uiPr
+00006240: 696f 7269 7479 3d22 3530 222f 3e3c 773a  iority="50"/><w:
+00006250: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00006260: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
+00006270: 3620 436f 6c6f 7266 756c 2220 773a 7569  6 Colorful" w:ui
+00006280: 5072 696f 7269 7479 3d22 3531 222f 3e3c  Priority="51"/><
+00006290: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+000062a0: 3a6e 616d 653d 224c 6973 7420 5461 626c  :name="List Tabl
+000062b0: 6520 3720 436f 6c6f 7266 756c 2220 773a  e 7 Colorful" w:
+000062c0: 7569 5072 696f 7269 7479 3d22 3532 222f  uiPriority="52"/
+000062d0: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+000062e0: 2077 3a6e 616d 653d 224c 6973 7420 5461   w:name="List Ta
+000062f0: 626c 6520 3120 4c69 6768 7420 4163 6365  ble 1 Light Acce
+00006300: 6e74 2031 2220 773a 7569 5072 696f 7269  nt 1" w:uiPriori
+00006310: 7479 3d22 3436 222f 3e3c 773a 6c73 6445  ty="46"/><w:lsdE
+00006320: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00006330: 224c 6973 7420 5461 626c 6520 3220 4163  "List Table 2 Ac
+00006340: 6365 6e74 2031 2220 773a 7569 5072 696f  cent 1" w:uiPrio
+00006350: 7269 7479 3d22 3437 222f 3e3c 773a 6c73  rity="47"/><w:ls
+00006360: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00006370: 653d 224c 6973 7420 5461 626c 6520 3320  e="List Table 3 
+00006380: 4163 6365 6e74 2031 2220 773a 7569 5072  Accent 1" w:uiPr
+00006390: 696f 7269 7479 3d22 3438 222f 3e3c 773a  iority="48"/><w:
+000063a0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+000063b0: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
+000063c0: 3420 4163 6365 6e74 2031 2220 773a 7569  4 Accent 1" w:ui
+000063d0: 5072 696f 7269 7479 3d22 3439 222f 3e3c  Priority="49"/><
+000063e0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+000063f0: 3a6e 616d 653d 224c 6973 7420 5461 626c  :name="List Tabl
+00006400: 6520 3520 4461 726b 2041 6363 656e 7420  e 5 Dark Accent 
+00006410: 3122 2077 3a75 6950 7269 6f72 6974 793d  1" w:uiPriority=
+00006420: 2235 3022 2f3e 3c77 3a6c 7364 4578 6365  "50"/><w:lsdExce
+00006430: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+00006440: 7374 2054 6162 6c65 2036 2043 6f6c 6f72  st Table 6 Color
+00006450: 6675 6c20 4163 6365 6e74 2031 2220 773a  ful Accent 1" w:
+00006460: 7569 5072 696f 7269 7479 3d22 3531 222f  uiPriority="51"/
+00006470: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00006480: 2077 3a6e 616d 653d 224c 6973 7420 5461   w:name="List Ta
+00006490: 626c 6520 3720 436f 6c6f 7266 756c 2041  ble 7 Colorful A
+000064a0: 6363 656e 7420 3122 2077 3a75 6950 7269  ccent 1" w:uiPri
+000064b0: 6f72 6974 793d 2235 3222 2f3e 3c77 3a6c  ority="52"/><w:l
+000064c0: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+000064d0: 6d65 3d22 4c69 7374 2054 6162 6c65 2031  me="List Table 1
+000064e0: 204c 6967 6874 2041 6363 656e 7420 3222   Light Accent 2"
+000064f0: 2077 3a75 6950 7269 6f72 6974 793d 2234   w:uiPriority="4
+00006500: 3622 2f3e 3c77 3a6c 7364 4578 6365 7074  6"/><w:lsdExcept
+00006510: 696f 6e20 773a 6e61 6d65 3d22 4c69 7374  ion w:name="List
+00006520: 2054 6162 6c65 2032 2041 6363 656e 7420   Table 2 Accent 
+00006530: 3222 2077 3a75 6950 7269 6f72 6974 793d  2" w:uiPriority=
+00006540: 2234 3722 2f3e 3c77 3a6c 7364 4578 6365  "47"/><w:lsdExce
+00006550: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+00006560: 7374 2054 6162 6c65 2033 2041 6363 656e  st Table 3 Accen
+00006570: 7420 3222 2077 3a75 6950 7269 6f72 6974  t 2" w:uiPriorit
+00006580: 793d 2234 3822 2f3e 3c77 3a6c 7364 4578  y="48"/><w:lsdEx
+00006590: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+000065a0: 4c69 7374 2054 6162 6c65 2034 2041 6363  List Table 4 Acc
+000065b0: 656e 7420 3222 2077 3a75 6950 7269 6f72  ent 2" w:uiPrior
+000065c0: 6974 793d 2234 3922 2f3e 3c77 3a6c 7364  ity="49"/><w:lsd
+000065d0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000065e0: 3d22 4c69 7374 2054 6162 6c65 2035 2044  ="List Table 5 D
+000065f0: 6172 6b20 4163 6365 6e74 2032 2220 773a  ark Accent 2" w:
+00006600: 7569 5072 696f 7269 7479 3d22 3530 222f  uiPriority="50"/
+00006610: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00006620: 2077 3a6e 616d 653d 224c 6973 7420 5461   w:name="List Ta
+00006630: 626c 6520 3620 436f 6c6f 7266 756c 2041  ble 6 Colorful A
+00006640: 6363 656e 7420 3222 2077 3a75 6950 7269  ccent 2" w:uiPri
+00006650: 6f72 6974 793d 2235 3122 2f3e 3c77 3a6c  ority="51"/><w:l
+00006660: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00006670: 6d65 3d22 4c69 7374 2054 6162 6c65 2037  me="List Table 7
+00006680: 2043 6f6c 6f72 6675 6c20 4163 6365 6e74   Colorful Accent
+00006690: 2032 2220 773a 7569 5072 696f 7269 7479   2" w:uiPriority
+000066a0: 3d22 3532 222f 3e3c 773a 6c73 6445 7863  ="52"/><w:lsdExc
+000066b0: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+000066c0: 6973 7420 5461 626c 6520 3120 4c69 6768  ist Table 1 Ligh
+000066d0: 7420 4163 6365 6e74 2033 2220 773a 7569  t Accent 3" w:ui
+000066e0: 5072 696f 7269 7479 3d22 3436 222f 3e3c  Priority="46"/><
+000066f0: 773a 6c73 6445 7863 6570 7469 6f6e 2077  w:lsdException w
+00006700: 3a6e 616d 653d 224c 6973 7420 5461 626c  :name="List Tabl
+00006710: 6520 3220 4163 6365 6e74 2033 2220 773a  e 2 Accent 3" w:
+00006720: 7569 5072 696f 7269 7479 3d22 3437 222f  uiPriority="47"/
+00006730: 3e3c 773a 6c73 6445 7863 6570 7469 6f6e  ><w:lsdException
+00006740: 2077 3a6e 616d 653d 224c 6973 7420 5461   w:name="List Ta
+00006750: 626c 6520 3320 4163 6365 6e74 2033 2220  ble 3 Accent 3" 
+00006760: 773a 7569 5072 696f 7269 7479 3d22 3438  w:uiPriority="48
+00006770: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00006780: 6f6e 2077 3a6e 616d 653d 224c 6973 7420  on w:name="List 
+00006790: 5461 626c 6520 3420 4163 6365 6e74 2033  Table 4 Accent 3
+000067a0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+000067b0: 3439 222f 3e3c 773a 6c73 6445 7863 6570  49"/><w:lsdExcep
+000067c0: 7469 6f6e 2077 3a6e 616d 653d 224c 6973  tion w:name="Lis
+000067d0: 7420 5461 626c 6520 3520 4461 726b 2041  t Table 5 Dark A
+000067e0: 6363 656e 7420 3322 2077 3a75 6950 7269  ccent 3" w:uiPri
+000067f0: 6f72 6974 793d 2235 3022 2f3e 3c77 3a6c  ority="50"/><w:l
+00006800: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00006810: 6d65 3d22 4c69 7374 2054 6162 6c65 2036  me="List Table 6
+00006820: 2043 6f6c 6f72 6675 6c20 4163 6365 6e74   Colorful Accent
+00006830: 2033 2220 773a 7569 5072 696f 7269 7479   3" w:uiPriority
+00006840: 3d22 3531 222f 3e3c 773a 6c73 6445 7863  ="51"/><w:lsdExc
+00006850: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00006860: 6973 7420 5461 626c 6520 3720 436f 6c6f  ist Table 7 Colo
+00006870: 7266 756c 2041 6363 656e 7420 3322 2077  rful Accent 3" w
+00006880: 3a75 6950 7269 6f72 6974 793d 2235 3222  :uiPriority="52"
+00006890: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+000068a0: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
+000068b0: 6162 6c65 2031 204c 6967 6874 2041 6363  able 1 Light Acc
+000068c0: 656e 7420 3422 2077 3a75 6950 7269 6f72  ent 4" w:uiPrior
+000068d0: 6974 793d 2234 3622 2f3e 3c77 3a6c 7364  ity="46"/><w:lsd
+000068e0: 4578 6365 7074 696f 6e20 773a 6e61 6d65  Exception w:name
+000068f0: 3d22 4c69 7374 2054 6162 6c65 2032 2041  ="List Table 2 A
+00006900: 6363 656e 7420 3422 2077 3a75 6950 7269  ccent 4" w:uiPri
+00006910: 6f72 6974 793d 2234 3722 2f3e 3c77 3a6c  ority="47"/><w:l
+00006920: 7364 4578 6365 7074 696f 6e20 773a 6e61  sdException w:na
+00006930: 6d65 3d22 4c69 7374 2054 6162 6c65 2033  me="List Table 3
+00006940: 2041 6363 656e 7420 3422 2077 3a75 6950   Accent 4" w:uiP
+00006950: 7269 6f72 6974 793d 2234 3822 2f3e 3c77  riority="48"/><w
+00006960: 3a6c 7364 4578 6365 7074 696f 6e20 773a  :lsdException w:
+00006970: 6e61 6d65 3d22 4c69 7374 2054 6162 6c65  name="List Table
+00006980: 2034 2041 6363 656e 7420 3422 2077 3a75   4 Accent 4" w:u
+00006990: 6950 7269 6f72 6974 793d 2234 3922 2f3e  iPriority="49"/>
+000069a0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+000069b0: 773a 6e61 6d65 3d22 4c69 7374 2054 6162  w:name="List Tab
+000069c0: 6c65 2035 2044 6172 6b20 4163 6365 6e74  le 5 Dark Accent
+000069d0: 2034 2220 773a 7569 5072 696f 7269 7479   4" w:uiPriority
+000069e0: 3d22 3530 222f 3e3c 773a 6c73 6445 7863  ="50"/><w:lsdExc
+000069f0: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00006a00: 6973 7420 5461 626c 6520 3620 436f 6c6f  ist Table 6 Colo
+00006a10: 7266 756c 2041 6363 656e 7420 3422 2077  rful Accent 4" w
+00006a20: 3a75 6950 7269 6f72 6974 793d 2235 3122  :uiPriority="51"
+00006a30: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00006a40: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
+00006a50: 6162 6c65 2037 2043 6f6c 6f72 6675 6c20  able 7 Colorful 
+00006a60: 4163 6365 6e74 2034 2220 773a 7569 5072  Accent 4" w:uiPr
+00006a70: 696f 7269 7479 3d22 3532 222f 3e3c 773a  iority="52"/><w:
+00006a80: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00006a90: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
+00006aa0: 3120 4c69 6768 7420 4163 6365 6e74 2035  1 Light Accent 5
+00006ab0: 2220 773a 7569 5072 696f 7269 7479 3d22  " w:uiPriority="
+00006ac0: 3436 222f 3e3c 773a 6c73 6445 7863 6570  46"/><w:lsdExcep
+00006ad0: 7469 6f6e 2077 3a6e 616d 653d 224c 6973  tion w:name="Lis
+00006ae0: 7420 5461 626c 6520 3220 4163 6365 6e74  t Table 2 Accent
+00006af0: 2035 2220 773a 7569 5072 696f 7269 7479   5" w:uiPriority
+00006b00: 3d22 3437 222f 3e3c 773a 6c73 6445 7863  ="47"/><w:lsdExc
+00006b10: 6570 7469 6f6e 2077 3a6e 616d 653d 224c  eption w:name="L
+00006b20: 6973 7420 5461 626c 6520 3320 4163 6365  ist Table 3 Acce
+00006b30: 6e74 2035 2220 773a 7569 5072 696f 7269  nt 5" w:uiPriori
+00006b40: 7479 3d22 3438 222f 3e3c 773a 6c73 6445  ty="48"/><w:lsdE
+00006b50: 7863 6570 7469 6f6e 2077 3a6e 616d 653d  xception w:name=
+00006b60: 224c 6973 7420 5461 626c 6520 3420 4163  "List Table 4 Ac
+00006b70: 6365 6e74 2035 2220 773a 7569 5072 696f  cent 5" w:uiPrio
+00006b80: 7269 7479 3d22 3439 222f 3e3c 773a 6c73  rity="49"/><w:ls
+00006b90: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00006ba0: 653d 224c 6973 7420 5461 626c 6520 3520  e="List Table 5 
+00006bb0: 4461 726b 2041 6363 656e 7420 3522 2077  Dark Accent 5" w
+00006bc0: 3a75 6950 7269 6f72 6974 793d 2235 3022  :uiPriority="50"
+00006bd0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00006be0: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
+00006bf0: 6162 6c65 2036 2043 6f6c 6f72 6675 6c20  able 6 Colorful 
+00006c00: 4163 6365 6e74 2035 2220 773a 7569 5072  Accent 5" w:uiPr
+00006c10: 696f 7269 7479 3d22 3531 222f 3e3c 773a  iority="51"/><w:
+00006c20: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00006c30: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
+00006c40: 3720 436f 6c6f 7266 756c 2041 6363 656e  7 Colorful Accen
+00006c50: 7420 3522 2077 3a75 6950 7269 6f72 6974  t 5" w:uiPriorit
+00006c60: 793d 2235 3222 2f3e 3c77 3a6c 7364 4578  y="52"/><w:lsdEx
+00006c70: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00006c80: 4c69 7374 2054 6162 6c65 2031 204c 6967  List Table 1 Lig
+00006c90: 6874 2041 6363 656e 7420 3622 2077 3a75  ht Accent 6" w:u
+00006ca0: 6950 7269 6f72 6974 793d 2234 3622 2f3e  iPriority="46"/>
+00006cb0: 3c77 3a6c 7364 4578 6365 7074 696f 6e20  <w:lsdException 
+00006cc0: 773a 6e61 6d65 3d22 4c69 7374 2054 6162  w:name="List Tab
+00006cd0: 6c65 2032 2041 6363 656e 7420 3622 2077  le 2 Accent 6" w
+00006ce0: 3a75 6950 7269 6f72 6974 793d 2234 3722  :uiPriority="47"
+00006cf0: 2f3e 3c77 3a6c 7364 4578 6365 7074 696f  /><w:lsdExceptio
+00006d00: 6e20 773a 6e61 6d65 3d22 4c69 7374 2054  n w:name="List T
+00006d10: 6162 6c65 2033 2041 6363 656e 7420 3622  able 3 Accent 6"
+00006d20: 2077 3a75 6950 7269 6f72 6974 793d 2234   w:uiPriority="4
+00006d30: 3822 2f3e 3c77 3a6c 7364 4578 6365 7074  8"/><w:lsdExcept
+00006d40: 696f 6e20 773a 6e61 6d65 3d22 4c69 7374  ion w:name="List
+00006d50: 2054 6162 6c65 2034 2041 6363 656e 7420   Table 4 Accent 
+00006d60: 3622 2077 3a75 6950 7269 6f72 6974 793d  6" w:uiPriority=
+00006d70: 2234 3922 2f3e 3c77 3a6c 7364 4578 6365  "49"/><w:lsdExce
+00006d80: 7074 696f 6e20 773a 6e61 6d65 3d22 4c69  ption w:name="Li
+00006d90: 7374 2054 6162 6c65 2035 2044 6172 6b20  st Table 5 Dark 
+00006da0: 4163 6365 6e74 2036 2220 773a 7569 5072  Accent 6" w:uiPr
+00006db0: 696f 7269 7479 3d22 3530 222f 3e3c 773a  iority="50"/><w:
+00006dc0: 6c73 6445 7863 6570 7469 6f6e 2077 3a6e  lsdException w:n
+00006dd0: 616d 653d 224c 6973 7420 5461 626c 6520  ame="List Table 
+00006de0: 3620 436f 6c6f 7266 756c 2041 6363 656e  6 Colorful Accen
+00006df0: 7420 3622 2077 3a75 6950 7269 6f72 6974  t 6" w:uiPriorit
+00006e00: 793d 2235 3122 2f3e 3c77 3a6c 7364 4578  y="51"/><w:lsdEx
+00006e10: 6365 7074 696f 6e20 773a 6e61 6d65 3d22  ception w:name="
+00006e20: 4c69 7374 2054 6162 6c65 2037 2043 6f6c  List Table 7 Col
+00006e30: 6f72 6675 6c20 4163 6365 6e74 2036 2220  orful Accent 6" 
+00006e40: 773a 7569 5072 696f 7269 7479 3d22 3532  w:uiPriority="52
+00006e50: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00006e60: 6f6e 2077 3a6e 616d 653d 224d 656e 7469  on w:name="Menti
+00006e70: 6f6e 2220 773a 7365 6d69 4869 6464 656e  on" w:semiHidden
+00006e80: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
+00006e90: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
+00006ea0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00006eb0: 653d 2253 6d61 7274 2048 7970 6572 6c69  e="Smart Hyperli
+00006ec0: 6e6b 2220 773a 7365 6d69 4869 6464 656e  nk" w:semiHidden
+00006ed0: 3d22 3122 2077 3a75 6e68 6964 6557 6865  ="1" w:unhideWhe
+00006ee0: 6e55 7365 643d 2231 222f 3e3c 773a 6c73  nUsed="1"/><w:ls
+00006ef0: 6445 7863 6570 7469 6f6e 2077 3a6e 616d  dException w:nam
+00006f00: 653d 2248 6173 6874 6167 2220 773a 7365  e="Hashtag" w:se
+00006f10: 6d69 4869 6464 656e 3d22 3122 2077 3a75  miHidden="1" w:u
+00006f20: 6e68 6964 6557 6865 6e55 7365 643d 2231  nhideWhenUsed="1
+00006f30: 222f 3e3c 773a 6c73 6445 7863 6570 7469  "/><w:lsdExcepti
+00006f40: 6f6e 2077 3a6e 616d 653d 2255 6e72 6573  on w:name="Unres
+00006f50: 6f6c 7665 6420 4d65 6e74 696f 6e22 2077  olved Mention" w
+00006f60: 3a73 656d 6948 6964 6465 6e3d 2231 2220  :semiHidden="1" 
+00006f70: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+00006f80: 3d22 3122 2f3e 3c77 3a6c 7364 4578 6365  ="1"/><w:lsdExce
+00006f90: 7074 696f 6e20 773a 6e61 6d65 3d22 536d  ption w:name="Sm
+00006fa0: 6172 7420 4c69 6e6b 2220 773a 7365 6d69  art Link" w:semi
+00006fb0: 4869 6464 656e 3d22 3122 2077 3a75 6e68  Hidden="1" w:unh
+00006fc0: 6964 6557 6865 6e55 7365 643d 2231 222f  ideWhenUsed="1"/
+00006fd0: 3e3c 2f77 3a6c 6174 656e 7453 7479 6c65  ></w:latentStyle
+00006fe0: 733e 3c77 3a73 7479 6c65 2077 3a74 7970  s><w:style w:typ
+00006ff0: 653d 2270 6172 6167 7261 7068 2220 773a  e="paragraph" w:
+00007000: 6465 6661 756c 743d 2231 2220 773a 7374  default="1" w:st
+00007010: 796c 6549 643d 224e 6f72 6d61 6c22 3e3c  yleId="Normal"><
+00007020: 773a 6e61 6d65 2077 3a76 616c 3d22 4e6f  w:name w:val="No
+00007030: 726d 616c 222f 3e3c 773a 7146 6f72 6d61  rmal"/><w:qForma
+00007040: 742f 3e3c 773a 7273 6964 2077 3a76 616c  t/><w:rsid w:val
+00007050: 3d22 3030 3733 3431 4634 222f 3e3c 2f77  ="007341F4"/></w
+00007060: 3a73 7479 6c65 3e3c 773a 7374 796c 6520  :style><w:style 
+00007070: 773a 7479 7065 3d22 7061 7261 6772 6170  w:type="paragrap
+00007080: 6822 2077 3a73 7479 6c65 4964 3d22 4865  h" w:styleId="He
+00007090: 6164 696e 6731 223e 3c77 3a6e 616d 6520  ading1"><w:name 
+000070a0: 773a 7661 6c3d 2268 6561 6469 6e67 2031  w:val="heading 1
+000070b0: 222f 3e3c 773a 6261 7365 644f 6e20 773a  "/><w:basedOn w:
+000070c0: 7661 6c3d 224e 6f72 6d61 6c22 2f3e 3c77  val="Normal"/><w
+000070d0: 3a6e 6578 7420 773a 7661 6c3d 224e 6f72  :next w:val="Nor
+000070e0: 6d61 6c22 2f3e 3c77 3a6c 696e 6b20 773a  mal"/><w:link w:
+000070f0: 7661 6c3d 2248 6561 6469 6e67 3143 6861  val="Heading1Cha
+00007100: 7222 2f3e 3c77 3a75 6950 7269 6f72 6974  r"/><w:uiPriorit
+00007110: 7920 773a 7661 6c3d 2239 222f 3e3c 773a  y w:val="9"/><w:
+00007120: 7146 6f72 6d61 742f 3e3c 773a 7273 6964  qFormat/><w:rsid
+00007130: 2077 3a76 616c 3d22 3030 3938 3632 3338   w:val="00986238
+00007140: 222f 3e3c 773a 7050 723e 3c77 3a6b 6565  "/><w:pPr><w:kee
+00007150: 704e 6578 742f 3e3c 773a 6b65 6570 4c69  pNext/><w:keepLi
+00007160: 6e65 732f 3e3c 773a 7370 6163 696e 6720  nes/><w:spacing 
+00007170: 773a 6265 666f 7265 3d22 3234 3022 2077  w:before="240" w
+00007180: 3a61 6674 6572 3d22 3022 2f3e 3c77 3a6f  :after="0"/><w:o
+00007190: 7574 6c69 6e65 4c76 6c20 773a 7661 6c3d  utlineLvl w:val=
+000071a0: 2230 222f 3e3c 2f77 3a70 5072 3e3c 773a  "0"/></w:pPr><w:
+000071b0: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
+000071c0: 6173 6369 6954 6865 6d65 3d22 6d61 6a6f  asciiTheme="majo
+000071d0: 7248 416e 7369 2220 773a 6561 7374 4173  rHAnsi" w:eastAs
+000071e0: 6961 5468 656d 653d 226d 616a 6f72 4561  iaTheme="majorEa
+000071f0: 7374 4173 6961 2220 773a 6841 6e73 6954  stAsia" w:hAnsiT
+00007200: 6865 6d65 3d22 6d61 6a6f 7248 416e 7369  heme="majorHAnsi
+00007210: 2220 773a 6373 7468 656d 653d 226d 616a  " w:cstheme="maj
+00007220: 6f72 4269 6469 222f 3e3c 773a 636f 6c6f  orBidi"/><w:colo
+00007230: 7220 773a 7661 6c3d 2232 4635 3439 3622  r w:val="2F5496"
+00007240: 2077 3a74 6865 6d65 436f 6c6f 723d 2261   w:themeColor="a
+00007250: 6363 656e 7431 2220 773a 7468 656d 6553  ccent1" w:themeS
+00007260: 6861 6465 3d22 4246 222f 3e3c 773a 737a  hade="BF"/><w:sz
+00007270: 2077 3a76 616c 3d22 3332 222f 3e3c 773a   w:val="32"/><w:
+00007280: 737a 4373 2077 3a76 616c 3d22 3332 222f  szCs w:val="32"/
+00007290: 3e3c 2f77 3a72 5072 3e3c 2f77 3a73 7479  ></w:rPr></w:sty
+000072a0: 6c65 3e3c 773a 7374 796c 6520 773a 7479  le><w:style w:ty
+000072b0: 7065 3d22 7061 7261 6772 6170 6822 2077  pe="paragraph" w
+000072c0: 3a73 7479 6c65 4964 3d22 4865 6164 696e  :styleId="Headin
+000072d0: 6732 223e 3c77 3a6e 616d 6520 773a 7661  g2"><w:name w:va
+000072e0: 6c3d 2268 6561 6469 6e67 2032 222f 3e3c  l="heading 2"/><
+000072f0: 773a 6261 7365 644f 6e20 773a 7661 6c3d  w:basedOn w:val=
+00007300: 224e 6f72 6d61 6c22 2f3e 3c77 3a6e 6578  "Normal"/><w:nex
+00007310: 7420 773a 7661 6c3d 224e 6f72 6d61 6c22  t w:val="Normal"
+00007320: 2f3e 3c77 3a6c 696e 6b20 773a 7661 6c3d  /><w:link w:val=
+00007330: 2248 6561 6469 6e67 3243 6861 7222 2f3e  "Heading2Char"/>
+00007340: 3c77 3a75 6950 7269 6f72 6974 7920 773a  <w:uiPriority w:
+00007350: 7661 6c3d 2239 222f 3e3c 773a 756e 6869  val="9"/><w:unhi
+00007360: 6465 5768 656e 5573 6564 2f3e 3c77 3a71  deWhenUsed/><w:q
+00007370: 466f 726d 6174 2f3e 3c77 3a72 7369 6420  Format/><w:rsid 
+00007380: 773a 7661 6c3d 2230 3039 3836 3233 3822  w:val="00986238"
+00007390: 2f3e 3c77 3a70 5072 3e3c 773a 6b65 6570  /><w:pPr><w:keep
+000073a0: 4e65 7874 2f3e 3c77 3a6b 6565 704c 696e  Next/><w:keepLin
+000073b0: 6573 2f3e 3c77 3a73 7061 6369 6e67 2077  es/><w:spacing w
+000073c0: 3a62 6566 6f72 653d 2234 3022 2077 3a61  :before="40" w:a
+000073d0: 6674 6572 3d22 3022 2f3e 3c77 3a6f 7574  fter="0"/><w:out
+000073e0: 6c69 6e65 4c76 6c20 773a 7661 6c3d 2231  lineLvl w:val="1
+000073f0: 222f 3e3c 2f77 3a70 5072 3e3c 773a 7250  "/></w:pPr><w:rP
+00007400: 723e 3c77 3a72 466f 6e74 7320 773a 6173  r><w:rFonts w:as
+00007410: 6369 6954 6865 6d65 3d22 6d61 6a6f 7248  ciiTheme="majorH
+00007420: 416e 7369 2220 773a 6561 7374 4173 6961  Ansi" w:eastAsia
+00007430: 5468 656d 653d 226d 616a 6f72 4561 7374  Theme="majorEast
+00007440: 4173 6961 2220 773a 6841 6e73 6954 6865  Asia" w:hAnsiThe
+00007450: 6d65 3d22 6d61 6a6f 7248 416e 7369 2220  me="majorHAnsi" 
+00007460: 773a 6373 7468 656d 653d 226d 616a 6f72  w:cstheme="major
+00007470: 4269 6469 222f 3e3c 773a 636f 6c6f 7220  Bidi"/><w:color 
+00007480: 773a 7661 6c3d 2232 4635 3439 3622 2077  w:val="2F5496" w
+00007490: 3a74 6865 6d65 436f 6c6f 723d 2261 6363  :themeColor="acc
+000074a0: 656e 7431 2220 773a 7468 656d 6553 6861  ent1" w:themeSha
+000074b0: 6465 3d22 4246 222f 3e3c 773a 737a 2077  de="BF"/><w:sz w
+000074c0: 3a76 616c 3d22 3236 222f 3e3c 773a 737a  :val="26"/><w:sz
+000074d0: 4373 2077 3a76 616c 3d22 3236 222f 3e3c  Cs w:val="26"/><
+000074e0: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
+000074f0: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
+00007500: 3d22 7061 7261 6772 6170 6822 2077 3a73  ="paragraph" w:s
+00007510: 7479 6c65 4964 3d22 4865 6164 696e 6733  tyleId="Heading3
+00007520: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
+00007530: 2268 6561 6469 6e67 2033 222f 3e3c 773a  "heading 3"/><w:
+00007540: 6261 7365 644f 6e20 773a 7661 6c3d 224e  basedOn w:val="N
+00007550: 6f72 6d61 6c22 2f3e 3c77 3a6e 6578 7420  ormal"/><w:next 
+00007560: 773a 7661 6c3d 224e 6f72 6d61 6c22 2f3e  w:val="Normal"/>
+00007570: 3c77 3a6c 696e 6b20 773a 7661 6c3d 2248  <w:link w:val="H
+00007580: 6561 6469 6e67 3343 6861 7222 2f3e 3c77  eading3Char"/><w
+00007590: 3a75 6950 7269 6f72 6974 7920 773a 7661  :uiPriority w:va
+000075a0: 6c3d 2239 222f 3e3c 773a 756e 6869 6465  l="9"/><w:unhide
+000075b0: 5768 656e 5573 6564 2f3e 3c77 3a71 466f  WhenUsed/><w:qFo
+000075c0: 726d 6174 2f3e 3c77 3a72 7369 6420 773a  rmat/><w:rsid w:
+000075d0: 7661 6c3d 2230 3039 3836 3233 3822 2f3e  val="00986238"/>
+000075e0: 3c77 3a70 5072 3e3c 773a 6b65 6570 4e65  <w:pPr><w:keepNe
+000075f0: 7874 2f3e 3c77 3a6b 6565 704c 696e 6573  xt/><w:keepLines
+00007600: 2f3e 3c77 3a73 7061 6369 6e67 2077 3a62  /><w:spacing w:b
+00007610: 6566 6f72 653d 2234 3022 2077 3a61 6674  efore="40" w:aft
+00007620: 6572 3d22 3022 2f3e 3c77 3a6f 7574 6c69  er="0"/><w:outli
+00007630: 6e65 4c76 6c20 773a 7661 6c3d 2232 222f  neLvl w:val="2"/
+00007640: 3e3c 2f77 3a70 5072 3e3c 773a 7250 723e  ></w:pPr><w:rPr>
+00007650: 3c77 3a72 466f 6e74 7320 773a 6173 6369  <w:rFonts w:asci
+00007660: 6954 6865 6d65 3d22 6d61 6a6f 7248 416e  iTheme="majorHAn
+00007670: 7369 2220 773a 6561 7374 4173 6961 5468  si" w:eastAsiaTh
+00007680: 656d 653d 226d 616a 6f72 4561 7374 4173  eme="majorEastAs
+00007690: 6961 2220 773a 6841 6e73 6954 6865 6d65  ia" w:hAnsiTheme
+000076a0: 3d22 6d61 6a6f 7248 416e 7369 2220 773a  ="majorHAnsi" w:
+000076b0: 6373 7468 656d 653d 226d 616a 6f72 4269  cstheme="majorBi
+000076c0: 6469 222f 3e3c 773a 636f 6c6f 7220 773a  di"/><w:color w:
+000076d0: 7661 6c3d 2231 4633 3736 3322 2077 3a74  val="1F3763" w:t
+000076e0: 6865 6d65 436f 6c6f 723d 2261 6363 656e  hemeColor="accen
+000076f0: 7431 2220 773a 7468 656d 6553 6861 6465  t1" w:themeShade
+00007700: 3d22 3746 222f 3e3c 773a 737a 2077 3a76  ="7F"/><w:sz w:v
+00007710: 616c 3d22 3234 222f 3e3c 773a 737a 4373  al="24"/><w:szCs
+00007720: 2077 3a76 616c 3d22 3234 222f 3e3c 2f77   w:val="24"/></w
+00007730: 3a72 5072 3e3c 2f77 3a73 7479 6c65 3e3c  :rPr></w:style><
+00007740: 773a 7374 796c 6520 773a 7479 7065 3d22  w:style w:type="
+00007750: 7061 7261 6772 6170 6822 2077 3a73 7479  paragraph" w:sty
+00007760: 6c65 4964 3d22 4865 6164 696e 6734 223e  leId="Heading4">
+00007770: 3c77 3a6e 616d 6520 773a 7661 6c3d 2268  <w:name w:val="h
+00007780: 6561 6469 6e67 2034 222f 3e3c 773a 6261  eading 4"/><w:ba
+00007790: 7365 644f 6e20 773a 7661 6c3d 224e 6f72  sedOn w:val="Nor
+000077a0: 6d61 6c22 2f3e 3c77 3a6e 6578 7420 773a  mal"/><w:next w:
+000077b0: 7661 6c3d 224e 6f72 6d61 6c22 2f3e 3c77  val="Normal"/><w
+000077c0: 3a6c 696e 6b20 773a 7661 6c3d 2248 6561  :link w:val="Hea
+000077d0: 6469 6e67 3443 6861 7222 2f3e 3c77 3a75  ding4Char"/><w:u
+000077e0: 6950 7269 6f72 6974 7920 773a 7661 6c3d  iPriority w:val=
+000077f0: 2239 222f 3e3c 773a 756e 6869 6465 5768  "9"/><w:unhideWh
+00007800: 656e 5573 6564 2f3e 3c77 3a71 466f 726d  enUsed/><w:qForm
+00007810: 6174 2f3e 3c77 3a72 7369 6420 773a 7661  at/><w:rsid w:va
+00007820: 6c3d 2230 3039 3836 3233 3822 2f3e 3c77  l="00986238"/><w
+00007830: 3a70 5072 3e3c 773a 6b65 6570 4e65 7874  :pPr><w:keepNext
+00007840: 2f3e 3c77 3a6b 6565 704c 696e 6573 2f3e  /><w:keepLines/>
+00007850: 3c77 3a73 7061 6369 6e67 2077 3a62 6566  <w:spacing w:bef
+00007860: 6f72 653d 2234 3022 2077 3a61 6674 6572  ore="40" w:after
+00007870: 3d22 3022 2f3e 3c77 3a6f 7574 6c69 6e65  ="0"/><w:outline
+00007880: 4c76 6c20 773a 7661 6c3d 2233 222f 3e3c  Lvl w:val="3"/><
+00007890: 2f77 3a70 5072 3e3c 773a 7250 723e 3c77  /w:pPr><w:rPr><w
+000078a0: 3a72 466f 6e74 7320 773a 6173 6369 6954  :rFonts w:asciiT
+000078b0: 6865 6d65 3d22 6d61 6a6f 7248 416e 7369  heme="majorHAnsi
+000078c0: 2220 773a 6561 7374 4173 6961 5468 656d  " w:eastAsiaThem
+000078d0: 653d 226d 616a 6f72 4561 7374 4173 6961  e="majorEastAsia
+000078e0: 2220 773a 6841 6e73 6954 6865 6d65 3d22  " w:hAnsiTheme="
+000078f0: 6d61 6a6f 7248 416e 7369 2220 773a 6373  majorHAnsi" w:cs
+00007900: 7468 656d 653d 226d 616a 6f72 4269 6469  theme="majorBidi
+00007910: 222f 3e3c 773a 692f 3e3c 773a 6943 732f  "/><w:i/><w:iCs/
+00007920: 3e3c 773a 636f 6c6f 7220 773a 7661 6c3d  ><w:color w:val=
+00007930: 2232 4635 3439 3622 2077 3a74 6865 6d65  "2F5496" w:theme
+00007940: 436f 6c6f 723d 2261 6363 656e 7431 2220  Color="accent1" 
+00007950: 773a 7468 656d 6553 6861 6465 3d22 4246  w:themeShade="BF
+00007960: 222f 3e3c 2f77 3a72 5072 3e3c 2f77 3a73  "/></w:rPr></w:s
+00007970: 7479 6c65 3e3c 773a 7374 796c 6520 773a  tyle><w:style w:
+00007980: 7479 7065 3d22 7061 7261 6772 6170 6822  type="paragraph"
+00007990: 2077 3a73 7479 6c65 4964 3d22 4865 6164   w:styleId="Head
+000079a0: 696e 6735 223e 3c77 3a6e 616d 6520 773a  ing5"><w:name w:
+000079b0: 7661 6c3d 2268 6561 6469 6e67 2035 222f  val="heading 5"/
+000079c0: 3e3c 773a 6261 7365 644f 6e20 773a 7661  ><w:basedOn w:va
+000079d0: 6c3d 224e 6f72 6d61 6c22 2f3e 3c77 3a6e  l="Normal"/><w:n
+000079e0: 6578 7420 773a 7661 6c3d 224e 6f72 6d61  ext w:val="Norma
+000079f0: 6c22 2f3e 3c77 3a6c 696e 6b20 773a 7661  l"/><w:link w:va
+00007a00: 6c3d 2248 6561 6469 6e67 3543 6861 7222  l="Heading5Char"
+00007a10: 2f3e 3c77 3a75 6950 7269 6f72 6974 7920  /><w:uiPriority 
+00007a20: 773a 7661 6c3d 2239 222f 3e3c 773a 756e  w:val="9"/><w:un
+00007a30: 6869 6465 5768 656e 5573 6564 2f3e 3c77  hideWhenUsed/><w
+00007a40: 3a71 466f 726d 6174 2f3e 3c77 3a72 7369  :qFormat/><w:rsi
+00007a50: 6420 773a 7661 6c3d 2230 3039 3836 3233  d w:val="0098623
+00007a60: 3822 2f3e 3c77 3a70 5072 3e3c 773a 6b65  8"/><w:pPr><w:ke
+00007a70: 6570 4e65 7874 2f3e 3c77 3a6b 6565 704c  epNext/><w:keepL
+00007a80: 696e 6573 2f3e 3c77 3a73 7061 6369 6e67  ines/><w:spacing
+00007a90: 2077 3a62 6566 6f72 653d 2234 3022 2077   w:before="40" w
+00007aa0: 3a61 6674 6572 3d22 3022 2f3e 3c77 3a6f  :after="0"/><w:o
+00007ab0: 7574 6c69 6e65 4c76 6c20 773a 7661 6c3d  utlineLvl w:val=
+00007ac0: 2234 222f 3e3c 2f77 3a70 5072 3e3c 773a  "4"/></w:pPr><w:
+00007ad0: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
+00007ae0: 6173 6369 6954 6865 6d65 3d22 6d61 6a6f  asciiTheme="majo
+00007af0: 7248 416e 7369 2220 773a 6561 7374 4173  rHAnsi" w:eastAs
+00007b00: 6961 5468 656d 653d 226d 616a 6f72 4561  iaTheme="majorEa
+00007b10: 7374 4173 6961 2220 773a 6841 6e73 6954  stAsia" w:hAnsiT
+00007b20: 6865 6d65 3d22 6d61 6a6f 7248 416e 7369  heme="majorHAnsi
+00007b30: 2220 773a 6373 7468 656d 653d 226d 616a  " w:cstheme="maj
+00007b40: 6f72 4269 6469 222f 3e3c 773a 636f 6c6f  orBidi"/><w:colo
+00007b50: 7220 773a 7661 6c3d 2232 4635 3439 3622  r w:val="2F5496"
+00007b60: 2077 3a74 6865 6d65 436f 6c6f 723d 2261   w:themeColor="a
+00007b70: 6363 656e 7431 2220 773a 7468 656d 6553  ccent1" w:themeS
+00007b80: 6861 6465 3d22 4246 222f 3e3c 2f77 3a72  hade="BF"/></w:r
+00007b90: 5072 3e3c 2f77 3a73 7479 6c65 3e3c 773a  Pr></w:style><w:
+00007ba0: 7374 796c 6520 773a 7479 7065 3d22 6368  style w:type="ch
+00007bb0: 6172 6163 7465 7222 2077 3a64 6566 6175  aracter" w:defau
+00007bc0: 6c74 3d22 3122 2077 3a73 7479 6c65 4964  lt="1" w:styleId
+00007bd0: 3d22 4465 6661 756c 7450 6172 6167 7261  ="DefaultParagra
+00007be0: 7068 466f 6e74 223e 3c77 3a6e 616d 6520  phFont"><w:name 
+00007bf0: 773a 7661 6c3d 2244 6566 6175 6c74 2050  w:val="Default P
+00007c00: 6172 6167 7261 7068 2046 6f6e 7422 2f3e  aragraph Font"/>
+00007c10: 3c77 3a75 6950 7269 6f72 6974 7920 773a  <w:uiPriority w:
+00007c20: 7661 6c3d 2231 222f 3e3c 773a 7365 6d69  val="1"/><w:semi
+00007c30: 4869 6464 656e 2f3e 3c77 3a75 6e68 6964  Hidden/><w:unhid
+00007c40: 6557 6865 6e55 7365 642f 3e3c 2f77 3a73  eWhenUsed/></w:s
+00007c50: 7479 6c65 3e3c 773a 7374 796c 6520 773a  tyle><w:style w:
+00007c60: 7479 7065 3d22 7461 626c 6522 2077 3a64  type="table" w:d
+00007c70: 6566 6175 6c74 3d22 3122 2077 3a73 7479  efault="1" w:sty
+00007c80: 6c65 4964 3d22 5461 626c 654e 6f72 6d61  leId="TableNorma
+00007c90: 6c22 3e3c 773a 6e61 6d65 2077 3a76 616c  l"><w:name w:val
+00007ca0: 3d22 4e6f 726d 616c 2054 6162 6c65 222f  ="Normal Table"/
+00007cb0: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
+00007cc0: 3a76 616c 3d22 3939 222f 3e3c 773a 7365  :val="99"/><w:se
+00007cd0: 6d69 4869 6464 656e 2f3e 3c77 3a75 6e68  miHidden/><w:unh
+00007ce0: 6964 6557 6865 6e55 7365 642f 3e3c 773a  ideWhenUsed/><w:
+00007cf0: 7462 6c50 723e 3c77 3a74 626c 496e 6420  tblPr><w:tblInd 
+00007d00: 773a 773d 2230 2220 773a 7479 7065 3d22  w:w="0" w:type="
+00007d10: 6478 6122 2f3e 3c77 3a74 626c 4365 6c6c  dxa"/><w:tblCell
+00007d20: 4d61 723e 3c77 3a74 6f70 2077 3a77 3d22  Mar><w:top w:w="
+00007d30: 3022 2077 3a74 7970 653d 2264 7861 222f  0" w:type="dxa"/
+00007d40: 3e3c 773a 6c65 6674 2077 3a77 3d22 3130  ><w:left w:w="10
+00007d50: 3822 2077 3a74 7970 653d 2264 7861 222f  8" w:type="dxa"/
+00007d60: 3e3c 773a 626f 7474 6f6d 2077 3a77 3d22  ><w:bottom w:w="
+00007d70: 3022 2077 3a74 7970 653d 2264 7861 222f  0" w:type="dxa"/
+00007d80: 3e3c 773a 7269 6768 7420 773a 773d 2231  ><w:right w:w="1
+00007d90: 3038 2220 773a 7479 7065 3d22 6478 6122  08" w:type="dxa"
+00007da0: 2f3e 3c2f 773a 7462 6c43 656c 6c4d 6172  /></w:tblCellMar
+00007db0: 3e3c 2f77 3a74 626c 5072 3e3c 2f77 3a73  ></w:tblPr></w:s
+00007dc0: 7479 6c65 3e3c 773a 7374 796c 6520 773a  tyle><w:style w:
+00007dd0: 7479 7065 3d22 6e75 6d62 6572 696e 6722  type="numbering"
+00007de0: 2077 3a64 6566 6175 6c74 3d22 3122 2077   w:default="1" w
+00007df0: 3a73 7479 6c65 4964 3d22 4e6f 4c69 7374  :styleId="NoList
+00007e00: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
+00007e10: 224e 6f20 4c69 7374 222f 3e3c 773a 7569  "No List"/><w:ui
+00007e20: 5072 696f 7269 7479 2077 3a76 616c 3d22  Priority w:val="
+00007e30: 3939 222f 3e3c 773a 7365 6d69 4869 6464  99"/><w:semiHidd
+00007e40: 656e 2f3e 3c77 3a75 6e68 6964 6557 6865  en/><w:unhideWhe
+00007e50: 6e55 7365 642f 3e3c 2f77 3a73 7479 6c65  nUsed/></w:style
+00007e60: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
+00007e70: 3d22 7061 7261 6772 6170 6822 2077 3a73  ="paragraph" w:s
+00007e80: 7479 6c65 4964 3d22 5469 746c 6522 3e3c  tyleId="Title"><
+00007e90: 773a 6e61 6d65 2077 3a76 616c 3d22 5469  w:name w:val="Ti
+00007ea0: 746c 6522 2f3e 3c77 3a62 6173 6564 4f6e  tle"/><w:basedOn
+00007eb0: 2077 3a76 616c 3d22 4e6f 726d 616c 222f   w:val="Normal"/
+00007ec0: 3e3c 773a 6e65 7874 2077 3a76 616c 3d22  ><w:next w:val="
+00007ed0: 4e6f 726d 616c 222f 3e3c 773a 6c69 6e6b  Normal"/><w:link
+00007ee0: 2077 3a76 616c 3d22 5469 746c 6543 6861   w:val="TitleCha
+00007ef0: 7222 2f3e 3c77 3a75 6950 7269 6f72 6974  r"/><w:uiPriorit
+00007f00: 7920 773a 7661 6c3d 2231 3022 2f3e 3c77  y w:val="10"/><w
+00007f10: 3a71 466f 726d 6174 2f3e 3c77 3a72 7369  :qFormat/><w:rsi
+00007f20: 6420 773a 7661 6c3d 2230 3037 3635 4437  d w:val="00765D7
+00007f30: 3522 2f3e 3c77 3a70 5072 3e3c 773a 7370  5"/><w:pPr><w:sp
+00007f40: 6163 696e 6720 773a 6166 7465 723d 2230  acing w:after="0
+00007f50: 2220 773a 6c69 6e65 3d22 3234 3022 2077  " w:line="240" w
+00007f60: 3a6c 696e 6552 756c 653d 2261 7574 6f22  :lineRule="auto"
+00007f70: 2f3e 3c77 3a63 6f6e 7465 7874 7561 6c53  /><w:contextualS
+00007f80: 7061 6369 6e67 2f3e 3c2f 773a 7050 723e  pacing/></w:pPr>
+00007f90: 3c77 3a72 5072 3e3c 773a 7246 6f6e 7473  <w:rPr><w:rFonts
+00007fa0: 2077 3a61 7363 6969 5468 656d 653d 226d   w:asciiTheme="m
+00007fb0: 616a 6f72 4841 6e73 6922 2077 3a65 6173  ajorHAnsi" w:eas
+00007fc0: 7441 7369 6154 6865 6d65 3d22 6d61 6a6f  tAsiaTheme="majo
+00007fd0: 7245 6173 7441 7369 6122 2077 3a68 416e  rEastAsia" w:hAn
+00007fe0: 7369 5468 656d 653d 226d 616a 6f72 4841  siTheme="majorHA
+00007ff0: 6e73 6922 2077 3a63 7374 6865 6d65 3d22  nsi" w:cstheme="
+00008000: 6d61 6a6f 7242 6964 6922 2f3e 3c77 3a73  majorBidi"/><w:s
+00008010: 7061 6369 6e67 2077 3a76 616c 3d22 2d31  pacing w:val="-1
+00008020: 3022 2f3e 3c77 3a6b 6572 6e20 773a 7661  0"/><w:kern w:va
+00008030: 6c3d 2232 3822 2f3e 3c77 3a73 7a20 773a  l="28"/><w:sz w:
+00008040: 7661 6c3d 2235 3622 2f3e 3c77 3a73 7a43  val="56"/><w:szC
+00008050: 7320 773a 7661 6c3d 2235 3622 2f3e 3c2f  s w:val="56"/></
+00008060: 773a 7250 723e 3c2f 773a 7374 796c 653e  w:rPr></w:style>
+00008070: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
+00008080: 2263 6861 7261 6374 6572 2220 773a 6375  "character" w:cu
+00008090: 7374 6f6d 5374 796c 653d 2231 2220 773a  stomStyle="1" w:
+000080a0: 7374 796c 6549 643d 2254 6974 6c65 4368  styleId="TitleCh
+000080b0: 6172 223e 3c77 3a6e 616d 6520 773a 7661  ar"><w:name w:va
+000080c0: 6c3d 2254 6974 6c65 2043 6861 7222 2f3e  l="Title Char"/>
+000080d0: 3c77 3a62 6173 6564 4f6e 2077 3a76 616c  <w:basedOn w:val
+000080e0: 3d22 4465 6661 756c 7450 6172 6167 7261  ="DefaultParagra
+000080f0: 7068 466f 6e74 222f 3e3c 773a 6c69 6e6b  phFont"/><w:link
+00008100: 2077 3a76 616c 3d22 5469 746c 6522 2f3e   w:val="Title"/>
+00008110: 3c77 3a75 6950 7269 6f72 6974 7920 773a  <w:uiPriority w:
+00008120: 7661 6c3d 2231 3022 2f3e 3c77 3a72 7369  val="10"/><w:rsi
+00008130: 6420 773a 7661 6c3d 2230 3037 3635 4437  d w:val="00765D7
+00008140: 3522 2f3e 3c77 3a72 5072 3e3c 773a 7246  5"/><w:rPr><w:rF
+00008150: 6f6e 7473 2077 3a61 7363 6969 5468 656d  onts w:asciiThem
+00008160: 653d 226d 616a 6f72 4841 6e73 6922 2077  e="majorHAnsi" w
+00008170: 3a65 6173 7441 7369 6154 6865 6d65 3d22  :eastAsiaTheme="
+00008180: 6d61 6a6f 7245 6173 7441 7369 6122 2077  majorEastAsia" w
+00008190: 3a68 416e 7369 5468 656d 653d 226d 616a  :hAnsiTheme="maj
+000081a0: 6f72 4841 6e73 6922 2077 3a63 7374 6865  orHAnsi" w:csthe
+000081b0: 6d65 3d22 6d61 6a6f 7242 6964 6922 2f3e  me="majorBidi"/>
+000081c0: 3c77 3a73 7061 6369 6e67 2077 3a76 616c  <w:spacing w:val
+000081d0: 3d22 2d31 3022 2f3e 3c77 3a6b 6572 6e20  ="-10"/><w:kern 
+000081e0: 773a 7661 6c3d 2232 3822 2f3e 3c77 3a73  w:val="28"/><w:s
+000081f0: 7a20 773a 7661 6c3d 2235 3622 2f3e 3c77  z w:val="56"/><w
+00008200: 3a73 7a43 7320 773a 7661 6c3d 2235 3622  :szCs w:val="56"
+00008210: 2f3e 3c2f 773a 7250 723e 3c2f 773a 7374  /></w:rPr></w:st
+00008220: 796c 653e 3c77 3a73 7479 6c65 2077 3a74  yle><w:style w:t
+00008230: 7970 653d 2263 6861 7261 6374 6572 2220  ype="character" 
+00008240: 773a 6375 7374 6f6d 5374 796c 653d 2231  w:customStyle="1
+00008250: 2220 773a 7374 796c 6549 643d 2248 6561  " w:styleId="Hea
+00008260: 6469 6e67 3143 6861 7222 3e3c 773a 6e61  ding1Char"><w:na
+00008270: 6d65 2077 3a76 616c 3d22 4865 6164 696e  me w:val="Headin
+00008280: 6720 3120 4368 6172 222f 3e3c 773a 6261  g 1 Char"/><w:ba
+00008290: 7365 644f 6e20 773a 7661 6c3d 2244 6566  sedOn w:val="Def
+000082a0: 6175 6c74 5061 7261 6772 6170 6846 6f6e  aultParagraphFon
+000082b0: 7422 2f3e 3c77 3a6c 696e 6b20 773a 7661  t"/><w:link w:va
+000082c0: 6c3d 2248 6561 6469 6e67 3122 2f3e 3c77  l="Heading1"/><w
+000082d0: 3a75 6950 7269 6f72 6974 7920 773a 7661  :uiPriority w:va
+000082e0: 6c3d 2239 222f 3e3c 773a 7273 6964 2077  l="9"/><w:rsid w
+000082f0: 3a76 616c 3d22 3030 3938 3632 3338 222f  :val="00986238"/
+00008300: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
+00008310: 7320 773a 6173 6369 6954 6865 6d65 3d22  s w:asciiTheme="
+00008320: 6d61 6a6f 7248 416e 7369 2220 773a 6561  majorHAnsi" w:ea
+00008330: 7374 4173 6961 5468 656d 653d 226d 616a  stAsiaTheme="maj
+00008340: 6f72 4561 7374 4173 6961 2220 773a 6841  orEastAsia" w:hA
+00008350: 6e73 6954 6865 6d65 3d22 6d61 6a6f 7248  nsiTheme="majorH
+00008360: 416e 7369 2220 773a 6373 7468 656d 653d  Ansi" w:cstheme=
+00008370: 226d 616a 6f72 4269 6469 222f 3e3c 773a  "majorBidi"/><w:
+00008380: 636f 6c6f 7220 773a 7661 6c3d 2232 4635  color w:val="2F5
+00008390: 3439 3622 2077 3a74 6865 6d65 436f 6c6f  496" w:themeColo
+000083a0: 723d 2261 6363 656e 7431 2220 773a 7468  r="accent1" w:th
+000083b0: 656d 6553 6861 6465 3d22 4246 222f 3e3c  emeShade="BF"/><
+000083c0: 773a 737a 2077 3a76 616c 3d22 3332 222f  w:sz w:val="32"/
+000083d0: 3e3c 773a 737a 4373 2077 3a76 616c 3d22  ><w:szCs w:val="
+000083e0: 3332 222f 3e3c 2f77 3a72 5072 3e3c 2f77  32"/></w:rPr></w
+000083f0: 3a73 7479 6c65 3e3c 773a 7374 796c 6520  :style><w:style 
+00008400: 773a 7479 7065 3d22 6368 6172 6163 7465  w:type="characte
+00008410: 7222 2077 3a63 7573 746f 6d53 7479 6c65  r" w:customStyle
+00008420: 3d22 3122 2077 3a73 7479 6c65 4964 3d22  ="1" w:styleId="
+00008430: 4865 6164 696e 6732 4368 6172 223e 3c77  Heading2Char"><w
+00008440: 3a6e 616d 6520 773a 7661 6c3d 2248 6561  :name w:val="Hea
+00008450: 6469 6e67 2032 2043 6861 7222 2f3e 3c77  ding 2 Char"/><w
+00008460: 3a62 6173 6564 4f6e 2077 3a76 616c 3d22  :basedOn w:val="
+00008470: 4465 6661 756c 7450 6172 6167 7261 7068  DefaultParagraph
+00008480: 466f 6e74 222f 3e3c 773a 6c69 6e6b 2077  Font"/><w:link w
+00008490: 3a76 616c 3d22 4865 6164 696e 6732 222f  :val="Heading2"/
+000084a0: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
+000084b0: 3a76 616c 3d22 3922 2f3e 3c77 3a72 7369  :val="9"/><w:rsi
+000084c0: 6420 773a 7661 6c3d 2230 3039 3836 3233  d w:val="0098623
+000084d0: 3822 2f3e 3c77 3a72 5072 3e3c 773a 7246  8"/><w:rPr><w:rF
+000084e0: 6f6e 7473 2077 3a61 7363 6969 5468 656d  onts w:asciiThem
+000084f0: 653d 226d 616a 6f72 4841 6e73 6922 2077  e="majorHAnsi" w
+00008500: 3a65 6173 7441 7369 6154 6865 6d65 3d22  :eastAsiaTheme="
+00008510: 6d61 6a6f 7245 6173 7441 7369 6122 2077  majorEastAsia" w
+00008520: 3a68 416e 7369 5468 656d 653d 226d 616a  :hAnsiTheme="maj
+00008530: 6f72 4841 6e73 6922 2077 3a63 7374 6865  orHAnsi" w:csthe
+00008540: 6d65 3d22 6d61 6a6f 7242 6964 6922 2f3e  me="majorBidi"/>
+00008550: 3c77 3a63 6f6c 6f72 2077 3a76 616c 3d22  <w:color w:val="
+00008560: 3246 3534 3936 2220 773a 7468 656d 6543  2F5496" w:themeC
+00008570: 6f6c 6f72 3d22 6163 6365 6e74 3122 2077  olor="accent1" w
+00008580: 3a74 6865 6d65 5368 6164 653d 2242 4622  :themeShade="BF"
+00008590: 2f3e 3c77 3a73 7a20 773a 7661 6c3d 2232  /><w:sz w:val="2
+000085a0: 3622 2f3e 3c77 3a73 7a43 7320 773a 7661  6"/><w:szCs w:va
+000085b0: 6c3d 2232 3622 2f3e 3c2f 773a 7250 723e  l="26"/></w:rPr>
+000085c0: 3c2f 773a 7374 796c 653e 3c77 3a73 7479  </w:style><w:sty
+000085d0: 6c65 2077 3a74 7970 653d 2263 6861 7261  le w:type="chara
+000085e0: 6374 6572 2220 773a 6375 7374 6f6d 5374  cter" w:customSt
+000085f0: 796c 653d 2231 2220 773a 7374 796c 6549  yle="1" w:styleI
+00008600: 643d 2248 6561 6469 6e67 3343 6861 7222  d="Heading3Char"
+00008610: 3e3c 773a 6e61 6d65 2077 3a76 616c 3d22  ><w:name w:val="
+00008620: 4865 6164 696e 6720 3320 4368 6172 222f  Heading 3 Char"/
+00008630: 3e3c 773a 6261 7365 644f 6e20 773a 7661  ><w:basedOn w:va
+00008640: 6c3d 2244 6566 6175 6c74 5061 7261 6772  l="DefaultParagr
+00008650: 6170 6846 6f6e 7422 2f3e 3c77 3a6c 696e  aphFont"/><w:lin
+00008660: 6b20 773a 7661 6c3d 2248 6561 6469 6e67  k w:val="Heading
+00008670: 3322 2f3e 3c77 3a75 6950 7269 6f72 6974  3"/><w:uiPriorit
+00008680: 7920 773a 7661 6c3d 2239 222f 3e3c 773a  y w:val="9"/><w:
+00008690: 7273 6964 2077 3a76 616c 3d22 3030 3938  rsid w:val="0098
+000086a0: 3632 3338 222f 3e3c 773a 7250 723e 3c77  6238"/><w:rPr><w
+000086b0: 3a72 466f 6e74 7320 773a 6173 6369 6954  :rFonts w:asciiT
+000086c0: 6865 6d65 3d22 6d61 6a6f 7248 416e 7369  heme="majorHAnsi
+000086d0: 2220 773a 6561 7374 4173 6961 5468 656d  " w:eastAsiaThem
+000086e0: 653d 226d 616a 6f72 4561 7374 4173 6961  e="majorEastAsia
+000086f0: 2220 773a 6841 6e73 6954 6865 6d65 3d22  " w:hAnsiTheme="
+00008700: 6d61 6a6f 7248 416e 7369 2220 773a 6373  majorHAnsi" w:cs
+00008710: 7468 656d 653d 226d 616a 6f72 4269 6469  theme="majorBidi
+00008720: 222f 3e3c 773a 636f 6c6f 7220 773a 7661  "/><w:color w:va
+00008730: 6c3d 2231 4633 3736 3322 2077 3a74 6865  l="1F3763" w:the
+00008740: 6d65 436f 6c6f 723d 2261 6363 656e 7431  meColor="accent1
+00008750: 2220 773a 7468 656d 6553 6861 6465 3d22  " w:themeShade="
+00008760: 3746 222f 3e3c 773a 737a 2077 3a76 616c  7F"/><w:sz w:val
+00008770: 3d22 3234 222f 3e3c 773a 737a 4373 2077  ="24"/><w:szCs w
+00008780: 3a76 616c 3d22 3234 222f 3e3c 2f77 3a72  :val="24"/></w:r
+00008790: 5072 3e3c 2f77 3a73 7479 6c65 3e3c 773a  Pr></w:style><w:
+000087a0: 7374 796c 6520 773a 7479 7065 3d22 6368  style w:type="ch
+000087b0: 6172 6163 7465 7222 2077 3a63 7573 746f  aracter" w:custo
+000087c0: 6d53 7479 6c65 3d22 3122 2077 3a73 7479  mStyle="1" w:sty
+000087d0: 6c65 4964 3d22 4865 6164 696e 6734 4368  leId="Heading4Ch
+000087e0: 6172 223e 3c77 3a6e 616d 6520 773a 7661  ar"><w:name w:va
+000087f0: 6c3d 2248 6561 6469 6e67 2034 2043 6861  l="Heading 4 Cha
+00008800: 7222 2f3e 3c77 3a62 6173 6564 4f6e 2077  r"/><w:basedOn w
+00008810: 3a76 616c 3d22 4465 6661 756c 7450 6172  :val="DefaultPar
+00008820: 6167 7261 7068 466f 6e74 222f 3e3c 773a  agraphFont"/><w:
+00008830: 6c69 6e6b 2077 3a76 616c 3d22 4865 6164  link w:val="Head
+00008840: 696e 6734 222f 3e3c 773a 7569 5072 696f  ing4"/><w:uiPrio
+00008850: 7269 7479 2077 3a76 616c 3d22 3922 2f3e  rity w:val="9"/>
+00008860: 3c77 3a72 7369 6420 773a 7661 6c3d 2230  <w:rsid w:val="0
+00008870: 3039 3836 3233 3822 2f3e 3c77 3a72 5072  0986238"/><w:rPr
+00008880: 3e3c 773a 7246 6f6e 7473 2077 3a61 7363  ><w:rFonts w:asc
+00008890: 6969 5468 656d 653d 226d 616a 6f72 4841  iiTheme="majorHA
+000088a0: 6e73 6922 2077 3a65 6173 7441 7369 6154  nsi" w:eastAsiaT
+000088b0: 6865 6d65 3d22 6d61 6a6f 7245 6173 7441  heme="majorEastA
+000088c0: 7369 6122 2077 3a68 416e 7369 5468 656d  sia" w:hAnsiThem
+000088d0: 653d 226d 616a 6f72 4841 6e73 6922 2077  e="majorHAnsi" w
+000088e0: 3a63 7374 6865 6d65 3d22 6d61 6a6f 7242  :cstheme="majorB
+000088f0: 6964 6922 2f3e 3c77 3a69 2f3e 3c77 3a69  idi"/><w:i/><w:i
+00008900: 4373 2f3e 3c77 3a63 6f6c 6f72 2077 3a76  Cs/><w:color w:v
+00008910: 616c 3d22 3246 3534 3936 2220 773a 7468  al="2F5496" w:th
+00008920: 656d 6543 6f6c 6f72 3d22 6163 6365 6e74  emeColor="accent
+00008930: 3122 2077 3a74 6865 6d65 5368 6164 653d  1" w:themeShade=
+00008940: 2242 4622 2f3e 3c2f 773a 7250 723e 3c2f  "BF"/></w:rPr></
+00008950: 773a 7374 796c 653e 3c77 3a73 7479 6c65  w:style><w:style
+00008960: 2077 3a74 7970 653d 2263 6861 7261 6374   w:type="charact
+00008970: 6572 2220 773a 6375 7374 6f6d 5374 796c  er" w:customStyl
+00008980: 653d 2231 2220 773a 7374 796c 6549 643d  e="1" w:styleId=
+00008990: 2248 6561 6469 6e67 3543 6861 7222 3e3c  "Heading5Char"><
+000089a0: 773a 6e61 6d65 2077 3a76 616c 3d22 4865  w:name w:val="He
+000089b0: 6164 696e 6720 3520 4368 6172 222f 3e3c  ading 5 Char"/><
+000089c0: 773a 6261 7365 644f 6e20 773a 7661 6c3d  w:basedOn w:val=
+000089d0: 2244 6566 6175 6c74 5061 7261 6772 6170  "DefaultParagrap
+000089e0: 6846 6f6e 7422 2f3e 3c77 3a6c 696e 6b20  hFont"/><w:link 
+000089f0: 773a 7661 6c3d 2248 6561 6469 6e67 3522  w:val="Heading5"
+00008a00: 2f3e 3c77 3a75 6950 7269 6f72 6974 7920  /><w:uiPriority 
+00008a10: 773a 7661 6c3d 2239 222f 3e3c 773a 7273  w:val="9"/><w:rs
+00008a20: 6964 2077 3a76 616c 3d22 3030 3938 3632  id w:val="009862
+00008a30: 3338 222f 3e3c 773a 7250 723e 3c77 3a72  38"/><w:rPr><w:r
+00008a40: 466f 6e74 7320 773a 6173 6369 6954 6865  Fonts w:asciiThe
+00008a50: 6d65 3d22 6d61 6a6f 7248 416e 7369 2220  me="majorHAnsi" 
+00008a60: 773a 6561 7374 4173 6961 5468 656d 653d  w:eastAsiaTheme=
+00008a70: 226d 616a 6f72 4561 7374 4173 6961 2220  "majorEastAsia" 
+00008a80: 773a 6841 6e73 6954 6865 6d65 3d22 6d61  w:hAnsiTheme="ma
+00008a90: 6a6f 7248 416e 7369 2220 773a 6373 7468  jorHAnsi" w:csth
+00008aa0: 656d 653d 226d 616a 6f72 4269 6469 222f  eme="majorBidi"/
+00008ab0: 3e3c 773a 636f 6c6f 7220 773a 7661 6c3d  ><w:color w:val=
+00008ac0: 2232 4635 3439 3622 2077 3a74 6865 6d65  "2F5496" w:theme
+00008ad0: 436f 6c6f 723d 2261 6363 656e 7431 2220  Color="accent1" 
+00008ae0: 773a 7468 656d 6553 6861 6465 3d22 4246  w:themeShade="BF
+00008af0: 222f 3e3c 2f77 3a72 5072 3e3c 2f77 3a73  "/></w:rPr></w:s
+00008b00: 7479 6c65 3e3c 773a 7374 796c 6520 773a  tyle><w:style w:
+00008b10: 7479 7065 3d22 7061 7261 6772 6170 6822  type="paragraph"
+00008b20: 2077 3a73 7479 6c65 4964 3d22 5375 6274   w:styleId="Subt
+00008b30: 6974 6c65 223e 3c77 3a6e 616d 6520 773a  itle"><w:name w:
+00008b40: 7661 6c3d 2253 7562 7469 746c 6522 2f3e  val="Subtitle"/>
+00008b50: 3c77 3a62 6173 6564 4f6e 2077 3a76 616c  <w:basedOn w:val
+00008b60: 3d22 4e6f 726d 616c 222f 3e3c 773a 6e65  ="Normal"/><w:ne
+00008b70: 7874 2077 3a76 616c 3d22 4e6f 726d 616c  xt w:val="Normal
+00008b80: 222f 3e3c 773a 6c69 6e6b 2077 3a76 616c  "/><w:link w:val
+00008b90: 3d22 5375 6274 6974 6c65 4368 6172 222f  ="SubtitleChar"/
+00008ba0: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
+00008bb0: 3a76 616c 3d22 3131 222f 3e3c 773a 7146  :val="11"/><w:qF
+00008bc0: 6f72 6d61 742f 3e3c 773a 7273 6964 2077  ormat/><w:rsid w
+00008bd0: 3a76 616c 3d22 3030 3938 3632 3338 222f  :val="00986238"/
+00008be0: 3e3c 773a 7050 723e 3c77 3a6e 756d 5072  ><w:pPr><w:numPr
+00008bf0: 3e3c 773a 696c 766c 2077 3a76 616c 3d22  ><w:ilvl w:val="
+00008c00: 3122 2f3e 3c2f 773a 6e75 6d50 723e 3c2f  1"/></w:numPr></
+00008c10: 773a 7050 723e 3c77 3a72 5072 3e3c 773a  w:pPr><w:rPr><w:
+00008c20: 7246 6f6e 7473 2077 3a65 6173 7441 7369  rFonts w:eastAsi
+00008c30: 6154 6865 6d65 3d22 6d69 6e6f 7245 6173  aTheme="minorEas
+00008c40: 7441 7369 6122 2f3e 3c77 3a63 6f6c 6f72  tAsia"/><w:color
+00008c50: 2077 3a76 616c 3d22 3541 3541 3541 2220   w:val="5A5A5A" 
+00008c60: 773a 7468 656d 6543 6f6c 6f72 3d22 7465  w:themeColor="te
+00008c70: 7874 3122 2077 3a74 6865 6d65 5469 6e74  xt1" w:themeTint
+00008c80: 3d22 4135 222f 3e3c 773a 7370 6163 696e  ="A5"/><w:spacin
+00008c90: 6720 773a 7661 6c3d 2231 3522 2f3e 3c2f  g w:val="15"/></
+00008ca0: 773a 7250 723e 3c2f 773a 7374 796c 653e  w:rPr></w:style>
+00008cb0: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
+00008cc0: 2263 6861 7261 6374 6572 2220 773a 6375  "character" w:cu
+00008cd0: 7374 6f6d 5374 796c 653d 2231 2220 773a  stomStyle="1" w:
+00008ce0: 7374 796c 6549 643d 2253 7562 7469 746c  styleId="Subtitl
+00008cf0: 6543 6861 7222 3e3c 773a 6e61 6d65 2077  eChar"><w:name w
+00008d00: 3a76 616c 3d22 5375 6274 6974 6c65 2043  :val="Subtitle C
+00008d10: 6861 7222 2f3e 3c77 3a62 6173 6564 4f6e  har"/><w:basedOn
+00008d20: 2077 3a76 616c 3d22 4465 6661 756c 7450   w:val="DefaultP
+00008d30: 6172 6167 7261 7068 466f 6e74 222f 3e3c  aragraphFont"/><
+00008d40: 773a 6c69 6e6b 2077 3a76 616c 3d22 5375  w:link w:val="Su
+00008d50: 6274 6974 6c65 222f 3e3c 773a 7569 5072  btitle"/><w:uiPr
+00008d60: 696f 7269 7479 2077 3a76 616c 3d22 3131  iority w:val="11
+00008d70: 222f 3e3c 773a 7273 6964 2077 3a76 616c  "/><w:rsid w:val
+00008d80: 3d22 3030 3938 3632 3338 222f 3e3c 773a  ="00986238"/><w:
+00008d90: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
+00008da0: 6561 7374 4173 6961 5468 656d 653d 226d  eastAsiaTheme="m
+00008db0: 696e 6f72 4561 7374 4173 6961 222f 3e3c  inorEastAsia"/><
+00008dc0: 773a 636f 6c6f 7220 773a 7661 6c3d 2235  w:color w:val="5
+00008dd0: 4135 4135 4122 2077 3a74 6865 6d65 436f  A5A5A" w:themeCo
+00008de0: 6c6f 723d 2274 6578 7431 2220 773a 7468  lor="text1" w:th
+00008df0: 656d 6554 696e 743d 2241 3522 2f3e 3c77  emeTint="A5"/><w
+00008e00: 3a73 7061 6369 6e67 2077 3a76 616c 3d22  :spacing w:val="
+00008e10: 3135 222f 3e3c 2f77 3a72 5072 3e3c 2f77  15"/></w:rPr></w
+00008e20: 3a73 7479 6c65 3e3c 773a 7374 796c 6520  :style><w:style 
+00008e30: 773a 7479 7065 3d22 6368 6172 6163 7465  w:type="characte
+00008e40: 7222 2077 3a73 7479 6c65 4964 3d22 5375  r" w:styleId="Su
+00008e50: 6274 6c65 456d 7068 6173 6973 223e 3c77  btleEmphasis"><w
+00008e60: 3a6e 616d 6520 773a 7661 6c3d 2253 7562  :name w:val="Sub
+00008e70: 746c 6520 456d 7068 6173 6973 222f 3e3c  tle Emphasis"/><
+00008e80: 773a 6261 7365 644f 6e20 773a 7661 6c3d  w:basedOn w:val=
+00008e90: 2244 6566 6175 6c74 5061 7261 6772 6170  "DefaultParagrap
+00008ea0: 6846 6f6e 7422 2f3e 3c77 3a75 6950 7269  hFont"/><w:uiPri
+00008eb0: 6f72 6974 7920 773a 7661 6c3d 2231 3922  ority w:val="19"
+00008ec0: 2f3e 3c77 3a71 466f 726d 6174 2f3e 3c77  /><w:qFormat/><w
+00008ed0: 3a72 7369 6420 773a 7661 6c3d 2230 3039  :rsid w:val="009
+00008ee0: 3836 3233 3822 2f3e 3c77 3a72 5072 3e3c  86238"/><w:rPr><
+00008ef0: 773a 692f 3e3c 773a 6943 732f 3e3c 773a  w:i/><w:iCs/><w:
+00008f00: 636f 6c6f 7220 773a 7661 6c3d 2234 3034  color w:val="404
+00008f10: 3034 3022 2077 3a74 6865 6d65 436f 6c6f  040" w:themeColo
+00008f20: 723d 2274 6578 7431 2220 773a 7468 656d  r="text1" w:them
+00008f30: 6554 696e 743d 2242 4622 2f3e 3c2f 773a  eTint="BF"/></w:
+00008f40: 7250 723e 3c2f 773a 7374 796c 653e 3c77  rPr></w:style><w
+00008f50: 3a73 7479 6c65 2077 3a74 7970 653d 2263  :style w:type="c
+00008f60: 6861 7261 6374 6572 2220 773a 7374 796c  haracter" w:styl
+00008f70: 6549 643d 2245 6d70 6861 7369 7322 3e3c  eId="Emphasis"><
+00008f80: 773a 6e61 6d65 2077 3a76 616c 3d22 456d  w:name w:val="Em
+00008f90: 7068 6173 6973 222f 3e3c 773a 6261 7365  phasis"/><w:base
+00008fa0: 644f 6e20 773a 7661 6c3d 2244 6566 6175  dOn w:val="Defau
+00008fb0: 6c74 5061 7261 6772 6170 6846 6f6e 7422  ltParagraphFont"
+00008fc0: 2f3e 3c77 3a75 6950 7269 6f72 6974 7920  /><w:uiPriority 
+00008fd0: 773a 7661 6c3d 2232 3022 2f3e 3c77 3a71  w:val="20"/><w:q
+00008fe0: 466f 726d 6174 2f3e 3c77 3a72 7369 6420  Format/><w:rsid 
+00008ff0: 773a 7661 6c3d 2230 3039 3836 3233 3822  w:val="00986238"
+00009000: 2f3e 3c77 3a72 5072 3e3c 773a 692f 3e3c  /><w:rPr><w:i/><
+00009010: 773a 6943 732f 3e3c 2f77 3a72 5072 3e3c  w:iCs/></w:rPr><
+00009020: 2f77 3a73 7479 6c65 3e3c 773a 7374 796c  /w:style><w:styl
+00009030: 6520 773a 7479 7065 3d22 6368 6172 6163  e w:type="charac
+00009040: 7465 7222 2077 3a73 7479 6c65 4964 3d22  ter" w:styleId="
+00009050: 496e 7465 6e73 6545 6d70 6861 7369 7322  IntenseEmphasis"
+00009060: 3e3c 773a 6e61 6d65 2077 3a76 616c 3d22  ><w:name w:val="
+00009070: 496e 7465 6e73 6520 456d 7068 6173 6973  Intense Emphasis
+00009080: 222f 3e3c 773a 6261 7365 644f 6e20 773a  "/><w:basedOn w:
+00009090: 7661 6c3d 2244 6566 6175 6c74 5061 7261  val="DefaultPara
+000090a0: 6772 6170 6846 6f6e 7422 2f3e 3c77 3a75  graphFont"/><w:u
+000090b0: 6950 7269 6f72 6974 7920 773a 7661 6c3d  iPriority w:val=
+000090c0: 2232 3122 2f3e 3c77 3a71 466f 726d 6174  "21"/><w:qFormat
+000090d0: 2f3e 3c77 3a72 7369 6420 773a 7661 6c3d  /><w:rsid w:val=
+000090e0: 2230 3039 3836 3233 3822 2f3e 3c77 3a72  "00986238"/><w:r
+000090f0: 5072 3e3c 773a 692f 3e3c 773a 6943 732f  Pr><w:i/><w:iCs/
+00009100: 3e3c 773a 636f 6c6f 7220 773a 7661 6c3d  ><w:color w:val=
+00009110: 2234 3437 3243 3422 2077 3a74 6865 6d65  "4472C4" w:theme
+00009120: 436f 6c6f 723d 2261 6363 656e 7431 222f  Color="accent1"/
+00009130: 3e3c 2f77 3a72 5072 3e3c 2f77 3a73 7479  ></w:rPr></w:sty
+00009140: 6c65 3e3c 773a 7374 796c 6520 773a 7479  le><w:style w:ty
+00009150: 7065 3d22 6368 6172 6163 7465 7222 2077  pe="character" w
+00009160: 3a73 7479 6c65 4964 3d22 5374 726f 6e67  :styleId="Strong
+00009170: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
+00009180: 2253 7472 6f6e 6722 2f3e 3c77 3a62 6173  "Strong"/><w:bas
+00009190: 6564 4f6e 2077 3a76 616c 3d22 4465 6661  edOn w:val="Defa
+000091a0: 756c 7450 6172 6167 7261 7068 466f 6e74  ultParagraphFont
+000091b0: 222f 3e3c 773a 7569 5072 696f 7269 7479  "/><w:uiPriority
+000091c0: 2077 3a76 616c 3d22 3232 222f 3e3c 773a   w:val="22"/><w:
+000091d0: 7146 6f72 6d61 742f 3e3c 773a 7273 6964  qFormat/><w:rsid
+000091e0: 2077 3a76 616c 3d22 3030 3938 3632 3338   w:val="00986238
+000091f0: 222f 3e3c 773a 7250 723e 3c77 3a62 2f3e  "/><w:rPr><w:b/>
+00009200: 3c77 3a62 4373 2f3e 3c2f 773a 7250 723e  <w:bCs/></w:rPr>
+00009210: 3c2f 773a 7374 796c 653e 3c77 3a73 7479  </w:style><w:sty
+00009220: 6c65 2077 3a74 7970 653d 2270 6172 6167  le w:type="parag
+00009230: 7261 7068 2220 773a 7374 796c 6549 643d  raph" w:styleId=
+00009240: 2251 756f 7465 223e 3c77 3a6e 616d 6520  "Quote"><w:name 
+00009250: 773a 7661 6c3d 2251 756f 7465 222f 3e3c  w:val="Quote"/><
+00009260: 773a 6261 7365 644f 6e20 773a 7661 6c3d  w:basedOn w:val=
+00009270: 224e 6f72 6d61 6c22 2f3e 3c77 3a6e 6578  "Normal"/><w:nex
+00009280: 7420 773a 7661 6c3d 224e 6f72 6d61 6c22  t w:val="Normal"
+00009290: 2f3e 3c77 3a6c 696e 6b20 773a 7661 6c3d  /><w:link w:val=
+000092a0: 2251 756f 7465 4368 6172 222f 3e3c 773a  "QuoteChar"/><w:
+000092b0: 7569 5072 696f 7269 7479 2077 3a76 616c  uiPriority w:val
+000092c0: 3d22 3239 222f 3e3c 773a 7146 6f72 6d61  ="29"/><w:qForma
+000092d0: 742f 3e3c 773a 7273 6964 2077 3a76 616c  t/><w:rsid w:val
+000092e0: 3d22 3030 3938 3632 3338 222f 3e3c 773a  ="00986238"/><w:
+000092f0: 7050 723e 3c77 3a73 7061 6369 6e67 2077  pPr><w:spacing w
+00009300: 3a62 6566 6f72 653d 2232 3030 222f 3e3c  :before="200"/><
+00009310: 773a 696e 6420 773a 6c65 6674 3d22 3836  w:ind w:left="86
+00009320: 3422 2077 3a72 6967 6874 3d22 3836 3422  4" w:right="864"
+00009330: 2f3e 3c77 3a6a 6320 773a 7661 6c3d 2263  /><w:jc w:val="c
+00009340: 656e 7465 7222 2f3e 3c2f 773a 7050 723e  enter"/></w:pPr>
+00009350: 3c77 3a72 5072 3e3c 773a 692f 3e3c 773a  <w:rPr><w:i/><w:
+00009360: 6943 732f 3e3c 773a 636f 6c6f 7220 773a  iCs/><w:color w:
+00009370: 7661 6c3d 2234 3034 3034 3022 2077 3a74  val="404040" w:t
+00009380: 6865 6d65 436f 6c6f 723d 2274 6578 7431  hemeColor="text1
+00009390: 2220 773a 7468 656d 6554 696e 743d 2242  " w:themeTint="B
+000093a0: 4622 2f3e 3c2f 773a 7250 723e 3c2f 773a  F"/></w:rPr></w:
+000093b0: 7374 796c 653e 3c77 3a73 7479 6c65 2077  style><w:style w
+000093c0: 3a74 7970 653d 2263 6861 7261 6374 6572  :type="character
+000093d0: 2220 773a 6375 7374 6f6d 5374 796c 653d  " w:customStyle=
+000093e0: 2231 2220 773a 7374 796c 6549 643d 2251  "1" w:styleId="Q
+000093f0: 756f 7465 4368 6172 223e 3c77 3a6e 616d  uoteChar"><w:nam
+00009400: 6520 773a 7661 6c3d 2251 756f 7465 2043  e w:val="Quote C
+00009410: 6861 7222 2f3e 3c77 3a62 6173 6564 4f6e  har"/><w:basedOn
+00009420: 2077 3a76 616c 3d22 4465 6661 756c 7450   w:val="DefaultP
+00009430: 6172 6167 7261 7068 466f 6e74 222f 3e3c  aragraphFont"/><
+00009440: 773a 6c69 6e6b 2077 3a76 616c 3d22 5175  w:link w:val="Qu
+00009450: 6f74 6522 2f3e 3c77 3a75 6950 7269 6f72  ote"/><w:uiPrior
+00009460: 6974 7920 773a 7661 6c3d 2232 3922 2f3e  ity w:val="29"/>
+00009470: 3c77 3a72 7369 6420 773a 7661 6c3d 2230  <w:rsid w:val="0
+00009480: 3039 3836 3233 3822 2f3e 3c77 3a72 5072  0986238"/><w:rPr
+00009490: 3e3c 773a 692f 3e3c 773a 6943 732f 3e3c  ><w:i/><w:iCs/><
+000094a0: 773a 636f 6c6f 7220 773a 7661 6c3d 2234  w:color w:val="4
+000094b0: 3034 3034 3022 2077 3a74 6865 6d65 436f  04040" w:themeCo
+000094c0: 6c6f 723d 2274 6578 7431 2220 773a 7468  lor="text1" w:th
+000094d0: 656d 6554 696e 743d 2242 4622 2f3e 3c2f  emeTint="BF"/></
+000094e0: 773a 7250 723e 3c2f 773a 7374 796c 653e  w:rPr></w:style>
+000094f0: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
+00009500: 2270 6172 6167 7261 7068 2220 773a 7374  "paragraph" w:st
+00009510: 796c 6549 643d 2249 6e74 656e 7365 5175  yleId="IntenseQu
+00009520: 6f74 6522 3e3c 773a 6e61 6d65 2077 3a76  ote"><w:name w:v
+00009530: 616c 3d22 496e 7465 6e73 6520 5175 6f74  al="Intense Quot
+00009540: 6522 2f3e 3c77 3a62 6173 6564 4f6e 2077  e"/><w:basedOn w
+00009550: 3a76 616c 3d22 4e6f 726d 616c 222f 3e3c  :val="Normal"/><
+00009560: 773a 6e65 7874 2077 3a76 616c 3d22 4e6f  w:next w:val="No
+00009570: 726d 616c 222f 3e3c 773a 6c69 6e6b 2077  rmal"/><w:link w
+00009580: 3a76 616c 3d22 496e 7465 6e73 6551 756f  :val="IntenseQuo
+00009590: 7465 4368 6172 222f 3e3c 773a 7569 5072  teChar"/><w:uiPr
+000095a0: 696f 7269 7479 2077 3a76 616c 3d22 3330  iority w:val="30
+000095b0: 222f 3e3c 773a 7146 6f72 6d61 742f 3e3c  "/><w:qFormat/><
+000095c0: 773a 7273 6964 2077 3a76 616c 3d22 3030  w:rsid w:val="00
+000095d0: 3945 3636 3345 222f 3e3c 773a 7050 723e  9E663E"/><w:pPr>
+000095e0: 3c77 3a70 4264 723e 3c77 3a74 6f70 2077  <w:pBdr><w:top w
+000095f0: 3a76 616c 3d22 7369 6e67 6c65 2220 773a  :val="single" w:
+00009600: 737a 3d22 3422 2077 3a73 7061 6365 3d22  sz="4" w:space="
+00009610: 3130 2220 773a 636f 6c6f 723d 2234 3437  10" w:color="447
+00009620: 3243 3422 2077 3a74 6865 6d65 436f 6c6f  2C4" w:themeColo
+00009630: 723d 2261 6363 656e 7431 222f 3e3c 773a  r="accent1"/><w:
+00009640: 626f 7474 6f6d 2077 3a76 616c 3d22 7369  bottom w:val="si
+00009650: 6e67 6c65 2220 773a 737a 3d22 3422 2077  ngle" w:sz="4" w
+00009660: 3a73 7061 6365 3d22 3130 2220 773a 636f  :space="10" w:co
+00009670: 6c6f 723d 2234 3437 3243 3422 2077 3a74  lor="4472C4" w:t
+00009680: 6865 6d65 436f 6c6f 723d 2261 6363 656e  hemeColor="accen
+00009690: 7431 222f 3e3c 2f77 3a70 4264 723e 3c77  t1"/></w:pBdr><w
+000096a0: 3a73 7061 6369 6e67 2077 3a62 6566 6f72  :spacing w:befor
+000096b0: 653d 2233 3630 2220 773a 6166 7465 723d  e="360" w:after=
+000096c0: 2233 3630 222f 3e3c 773a 696e 6420 773a  "360"/><w:ind w:
+000096d0: 6c65 6674 3d22 3836 3422 2077 3a72 6967  left="864" w:rig
+000096e0: 6874 3d22 3836 3422 2f3e 3c77 3a6a 6320  ht="864"/><w:jc 
+000096f0: 773a 7661 6c3d 2263 656e 7465 7222 2f3e  w:val="center"/>
+00009700: 3c2f 773a 7050 723e 3c77 3a72 5072 3e3c  </w:pPr><w:rPr><
+00009710: 773a 692f 3e3c 773a 6943 732f 3e3c 773a  w:i/><w:iCs/><w:
+00009720: 636f 6c6f 7220 773a 7661 6c3d 2234 3437  color w:val="447
+00009730: 3243 3422 2077 3a74 6865 6d65 436f 6c6f  2C4" w:themeColo
+00009740: 723d 2261 6363 656e 7431 222f 3e3c 2f77  r="accent1"/></w
+00009750: 3a72 5072 3e3c 2f77 3a73 7479 6c65 3e3c  :rPr></w:style><
+00009760: 773a 7374 796c 6520 773a 7479 7065 3d22  w:style w:type="
+00009770: 6368 6172 6163 7465 7222 2077 3a63 7573  character" w:cus
+00009780: 746f 6d53 7479 6c65 3d22 3122 2077 3a73  tomStyle="1" w:s
+00009790: 7479 6c65 4964 3d22 496e 7465 6e73 6551  tyleId="IntenseQ
+000097a0: 756f 7465 4368 6172 223e 3c77 3a6e 616d  uoteChar"><w:nam
+000097b0: 6520 773a 7661 6c3d 2249 6e74 656e 7365  e w:val="Intense
+000097c0: 2051 756f 7465 2043 6861 7222 2f3e 3c77   Quote Char"/><w
+000097d0: 3a62 6173 6564 4f6e 2077 3a76 616c 3d22  :basedOn w:val="
+000097e0: 4465 6661 756c 7450 6172 6167 7261 7068  DefaultParagraph
+000097f0: 466f 6e74 222f 3e3c 773a 6c69 6e6b 2077  Font"/><w:link w
+00009800: 3a76 616c 3d22 496e 7465 6e73 6551 756f  :val="IntenseQuo
+00009810: 7465 222f 3e3c 773a 7569 5072 696f 7269  te"/><w:uiPriori
+00009820: 7479 2077 3a76 616c 3d22 3330 222f 3e3c  ty w:val="30"/><
+00009830: 773a 7273 6964 2077 3a76 616c 3d22 3030  w:rsid w:val="00
+00009840: 3945 3636 3345 222f 3e3c 773a 7250 723e  9E663E"/><w:rPr>
+00009850: 3c77 3a69 2f3e 3c77 3a69 4373 2f3e 3c77  <w:i/><w:iCs/><w
+00009860: 3a63 6f6c 6f72 2077 3a76 616c 3d22 3434  :color w:val="44
+00009870: 3732 4334 2220 773a 7468 656d 6543 6f6c  72C4" w:themeCol
+00009880: 6f72 3d22 6163 6365 6e74 3122 2f3e 3c2f  or="accent1"/></
+00009890: 773a 7250 723e 3c2f 773a 7374 796c 653e  w:rPr></w:style>
+000098a0: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
+000098b0: 2263 6861 7261 6374 6572 2220 773a 7374  "character" w:st
+000098c0: 796c 6549 643d 2253 7562 746c 6552 6566  yleId="SubtleRef
+000098d0: 6572 656e 6365 223e 3c77 3a6e 616d 6520  erence"><w:name 
+000098e0: 773a 7661 6c3d 2253 7562 746c 6520 5265  w:val="Subtle Re
+000098f0: 6665 7265 6e63 6522 2f3e 3c77 3a62 6173  ference"/><w:bas
+00009900: 6564 4f6e 2077 3a76 616c 3d22 4465 6661  edOn w:val="Defa
+00009910: 756c 7450 6172 6167 7261 7068 466f 6e74  ultParagraphFont
+00009920: 222f 3e3c 773a 7569 5072 696f 7269 7479  "/><w:uiPriority
+00009930: 2077 3a76 616c 3d22 3331 222f 3e3c 773a   w:val="31"/><w:
+00009940: 7146 6f72 6d61 742f 3e3c 773a 7273 6964  qFormat/><w:rsid
+00009950: 2077 3a76 616c 3d22 3030 3945 3636 3345   w:val="009E663E
+00009960: 222f 3e3c 773a 7250 723e 3c77 3a73 6d61  "/><w:rPr><w:sma
+00009970: 6c6c 4361 7073 2f3e 3c77 3a63 6f6c 6f72  llCaps/><w:color
+00009980: 2077 3a76 616c 3d22 3541 3541 3541 2220   w:val="5A5A5A" 
+00009990: 773a 7468 656d 6543 6f6c 6f72 3d22 7465  w:themeColor="te
+000099a0: 7874 3122 2077 3a74 6865 6d65 5469 6e74  xt1" w:themeTint
+000099b0: 3d22 4135 222f 3e3c 2f77 3a72 5072 3e3c  ="A5"/></w:rPr><
+000099c0: 2f77 3a73 7479 6c65 3e3c 773a 7374 796c  /w:style><w:styl
+000099d0: 6520 773a 7479 7065 3d22 6368 6172 6163  e w:type="charac
+000099e0: 7465 7222 2077 3a73 7479 6c65 4964 3d22  ter" w:styleId="
+000099f0: 496e 7465 6e73 6552 6566 6572 656e 6365  IntenseReference
+00009a00: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
+00009a10: 2249 6e74 656e 7365 2052 6566 6572 656e  "Intense Referen
+00009a20: 6365 222f 3e3c 773a 6261 7365 644f 6e20  ce"/><w:basedOn 
+00009a30: 773a 7661 6c3d 2244 6566 6175 6c74 5061  w:val="DefaultPa
+00009a40: 7261 6772 6170 6846 6f6e 7422 2f3e 3c77  ragraphFont"/><w
+00009a50: 3a75 6950 7269 6f72 6974 7920 773a 7661  :uiPriority w:va
+00009a60: 6c3d 2233 3222 2f3e 3c77 3a71 466f 726d  l="32"/><w:qForm
+00009a70: 6174 2f3e 3c77 3a72 7369 6420 773a 7661  at/><w:rsid w:va
+00009a80: 6c3d 2230 3039 4536 3633 4522 2f3e 3c77  l="009E663E"/><w
+00009a90: 3a72 5072 3e3c 773a 622f 3e3c 773a 6243  :rPr><w:b/><w:bC
+00009aa0: 732f 3e3c 773a 736d 616c 6c43 6170 732f  s/><w:smallCaps/
+00009ab0: 3e3c 773a 636f 6c6f 7220 773a 7661 6c3d  ><w:color w:val=
+00009ac0: 2234 3437 3243 3422 2077 3a74 6865 6d65  "4472C4" w:theme
+00009ad0: 436f 6c6f 723d 2261 6363 656e 7431 222f  Color="accent1"/
+00009ae0: 3e3c 773a 7370 6163 696e 6720 773a 7661  ><w:spacing w:va
+00009af0: 6c3d 2235 222f 3e3c 2f77 3a72 5072 3e3c  l="5"/></w:rPr><
+00009b00: 2f77 3a73 7479 6c65 3e3c 773a 7374 796c  /w:style><w:styl
+00009b10: 6520 773a 7479 7065 3d22 6368 6172 6163  e w:type="charac
+00009b20: 7465 7222 2077 3a73 7479 6c65 4964 3d22  ter" w:styleId="
+00009b30: 426f 6f6b 5469 746c 6522 3e3c 773a 6e61  BookTitle"><w:na
+00009b40: 6d65 2077 3a76 616c 3d22 426f 6f6b 2054  me w:val="Book T
+00009b50: 6974 6c65 222f 3e3c 773a 6261 7365 644f  itle"/><w:basedO
+00009b60: 6e20 773a 7661 6c3d 2244 6566 6175 6c74  n w:val="Default
+00009b70: 5061 7261 6772 6170 6846 6f6e 7422 2f3e  ParagraphFont"/>
+00009b80: 3c77 3a75 6950 7269 6f72 6974 7920 773a  <w:uiPriority w:
+00009b90: 7661 6c3d 2233 3322 2f3e 3c77 3a71 466f  val="33"/><w:qFo
+00009ba0: 726d 6174 2f3e 3c77 3a72 7369 6420 773a  rmat/><w:rsid w:
+00009bb0: 7661 6c3d 2230 3039 4536 3633 4522 2f3e  val="009E663E"/>
+00009bc0: 3c77 3a72 5072 3e3c 773a 622f 3e3c 773a  <w:rPr><w:b/><w:
+00009bd0: 6243 732f 3e3c 773a 692f 3e3c 773a 6943  bCs/><w:i/><w:iC
+00009be0: 732f 3e3c 773a 7370 6163 696e 6720 773a  s/><w:spacing w:
+00009bf0: 7661 6c3d 2235 222f 3e3c 2f77 3a72 5072  val="5"/></w:rPr
+00009c00: 3e3c 2f77 3a73 7479 6c65 3e3c 773a 7374  ></w:style><w:st
+00009c10: 796c 6520 773a 7479 7065 3d22 7061 7261  yle w:type="para
+00009c20: 6772 6170 6822 2077 3a73 7479 6c65 4964  graph" w:styleId
+00009c30: 3d22 4c69 7374 5061 7261 6772 6170 6822  ="ListParagraph"
+00009c40: 3e3c 773a 6e61 6d65 2077 3a76 616c 3d22  ><w:name w:val="
+00009c50: 4c69 7374 2050 6172 6167 7261 7068 222f  List Paragraph"/
+00009c60: 3e3c 773a 6261 7365 644f 6e20 773a 7661  ><w:basedOn w:va
+00009c70: 6c3d 224e 6f72 6d61 6c22 2f3e 3c77 3a75  l="Normal"/><w:u
+00009c80: 6950 7269 6f72 6974 7920 773a 7661 6c3d  iPriority w:val=
+00009c90: 2233 3422 2f3e 3c77 3a71 466f 726d 6174  "34"/><w:qFormat
+00009ca0: 2f3e 3c77 3a72 7369 6420 773a 7661 6c3d  /><w:rsid w:val=
+00009cb0: 2230 3039 4536 3633 4522 2f3e 3c77 3a70  "009E663E"/><w:p
+00009cc0: 5072 3e3c 773a 696e 6420 773a 6c65 6674  Pr><w:ind w:left
+00009cd0: 3d22 3732 3022 2f3e 3c77 3a63 6f6e 7465  ="720"/><w:conte
+00009ce0: 7874 7561 6c53 7061 6369 6e67 2f3e 3c2f  xtualSpacing/></
+00009cf0: 773a 7050 723e 3c2f 773a 7374 796c 653e  w:pPr></w:style>
+00009d00: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
+00009d10: 2270 6172 6167 7261 7068 2220 773a 7374  "paragraph" w:st
+00009d20: 796c 6549 643d 224e 6f53 7061 6369 6e67  yleId="NoSpacing
+00009d30: 223e 3c77 3a6e 616d 6520 773a 7661 6c3d  "><w:name w:val=
+00009d40: 224e 6f20 5370 6163 696e 6722 2f3e 3c77  "No Spacing"/><w
+00009d50: 3a75 6950 7269 6f72 6974 7920 773a 7661  :uiPriority w:va
+00009d60: 6c3d 2231 222f 3e3c 773a 7146 6f72 6d61  l="1"/><w:qForma
+00009d70: 742f 3e3c 773a 7273 6964 2077 3a76 616c  t/><w:rsid w:val
+00009d80: 3d22 3030 3945 3636 3345 222f 3e3c 773a  ="009E663E"/><w:
+00009d90: 7050 723e 3c77 3a73 7061 6369 6e67 2077  pPr><w:spacing w
+00009da0: 3a61 6674 6572 3d22 3022 2077 3a6c 696e  :after="0" w:lin
+00009db0: 653d 2232 3430 2220 773a 6c69 6e65 5275  e="240" w:lineRu
+00009dc0: 6c65 3d22 6175 746f 222f 3e3c 2f77 3a70  le="auto"/></w:p
+00009dd0: 5072 3e3c 2f77 3a73 7479 6c65 3e3c 773a  Pr></w:style><w:
+00009de0: 7374 796c 6520 773a 7479 7065 3d22 7061  style w:type="pa
+00009df0: 7261 6772 6170 6822 2077 3a73 7479 6c65  ragraph" w:style
+00009e00: 4964 3d22 4c69 7374 4e75 6d62 6572 223e  Id="ListNumber">
+00009e10: 3c77 3a6e 616d 6520 773a 7661 6c3d 224c  <w:name w:val="L
+00009e20: 6973 7420 4e75 6d62 6572 222f 3e3c 773a  ist Number"/><w:
+00009e30: 6261 7365 644f 6e20 773a 7661 6c3d 224e  basedOn w:val="N
+00009e40: 6f72 6d61 6c22 2f3e 3c77 3a75 6950 7269  ormal"/><w:uiPri
+00009e50: 6f72 6974 7920 773a 7661 6c3d 2239 3922  ority w:val="99"
+00009e60: 2f3e 3c77 3a75 6e68 6964 6557 6865 6e55  /><w:unhideWhenU
+00009e70: 7365 642f 3e3c 773a 7273 6964 2077 3a76  sed/><w:rsid w:v
+00009e80: 616c 3d22 3030 4437 3235 3541 222f 3e3c  al="00D7255A"/><
+00009e90: 773a 7050 723e 3c77 3a6e 756d 5072 3e3c  w:pPr><w:numPr><
+00009ea0: 773a 6e75 6d49 6420 773a 7661 6c3d 2239  w:numId w:val="9
+00009eb0: 222f 3e3c 2f77 3a6e 756d 5072 3e3c 773a  "/></w:numPr><w:
+00009ec0: 636f 6e74 6578 7475 616c 5370 6163 696e  contextualSpacin
+00009ed0: 672f 3e3c 2f77 3a70 5072 3e3c 2f77 3a73  g/></w:pPr></w:s
+00009ee0: 7479 6c65 3e3c 773a 7374 796c 6520 773a  tyle><w:style w:
+00009ef0: 7479 7065 3d22 7061 7261 6772 6170 6822  type="paragraph"
+00009f00: 2077 3a73 7479 6c65 4964 3d22 4c69 7374   w:styleId="List
+00009f10: 4275 6c6c 6574 223e 3c77 3a6e 616d 6520  Bullet"><w:name 
+00009f20: 773a 7661 6c3d 224c 6973 7420 4275 6c6c  w:val="List Bull
+00009f30: 6574 222f 3e3c 773a 6261 7365 644f 6e20  et"/><w:basedOn 
+00009f40: 773a 7661 6c3d 224e 6f72 6d61 6c22 2f3e  w:val="Normal"/>
+00009f50: 3c77 3a75 6950 7269 6f72 6974 7920 773a  <w:uiPriority w:
+00009f60: 7661 6c3d 2239 3922 2f3e 3c77 3a75 6e68  val="99"/><w:unh
+00009f70: 6964 6557 6865 6e55 7365 642f 3e3c 773a  ideWhenUsed/><w:
+00009f80: 7146 6f72 6d61 742f 3e3c 773a 7273 6964  qFormat/><w:rsid
+00009f90: 2077 3a76 616c 3d22 3030 3745 3443 3439   w:val="007E4C49
+00009fa0: 222f 3e3c 773a 7050 723e 3c77 3a6e 756d  "/><w:pPr><w:num
+00009fb0: 5072 3e3c 773a 6e75 6d49 6420 773a 7661  Pr><w:numId w:va
+00009fc0: 6c3d 2233 222f 3e3c 2f77 3a6e 756d 5072  l="3"/></w:numPr
+00009fd0: 3e3c 773a 636f 6e74 6578 7475 616c 5370  ><w:contextualSp
+00009fe0: 6163 696e 672f 3e3c 2f77 3a70 5072 3e3c  acing/></w:pPr><
+00009ff0: 2f77 3a73 7479 6c65 3e3c 773a 7374 796c  /w:style><w:styl
+0000a000: 6520 773a 7479 7065 3d22 7061 7261 6772  e w:type="paragr
+0000a010: 6170 6822 2077 3a73 7479 6c65 4964 3d22  aph" w:styleId="
+0000a020: 4d61 6372 6f54 6578 7422 3e3c 773a 6e61  MacroText"><w:na
+0000a030: 6d65 2077 3a76 616c 3d22 6d61 6372 6f22  me w:val="macro"
+0000a040: 2f3e 3c77 3a6c 696e 6b20 773a 7661 6c3d  /><w:link w:val=
+0000a050: 224d 6163 726f 5465 7874 4368 6172 222f  "MacroTextChar"/
+0000a060: 3e3c 773a 7569 5072 696f 7269 7479 2077  ><w:uiPriority w
+0000a070: 3a76 616c 3d22 3939 222f 3e3c 773a 756e  :val="99"/><w:un
+0000a080: 6869 6465 5768 656e 5573 6564 2f3e 3c77  hideWhenUsed/><w
+0000a090: 3a72 7369 6420 773a 7661 6c3d 2230 3044  :rsid w:val="00D
+0000a0a0: 3732 3535 4122 2f3e 3c77 3a70 5072 3e3c  7255A"/><w:pPr><
+0000a0b0: 773a 7461 6273 3e3c 773a 7461 6220 773a  w:tabs><w:tab w:
+0000a0c0: 7661 6c3d 226c 6566 7422 2077 3a70 6f73  val="left" w:pos
+0000a0d0: 3d22 3438 3022 2f3e 3c77 3a74 6162 2077  ="480"/><w:tab w
+0000a0e0: 3a76 616c 3d22 6c65 6674 2220 773a 706f  :val="left" w:po
+0000a0f0: 733d 2239 3630 222f 3e3c 773a 7461 6220  s="960"/><w:tab 
+0000a100: 773a 7661 6c3d 226c 6566 7422 2077 3a70  w:val="left" w:p
+0000a110: 6f73 3d22 3134 3430 222f 3e3c 773a 7461  os="1440"/><w:ta
+0000a120: 6220 773a 7661 6c3d 226c 6566 7422 2077  b w:val="left" w
+0000a130: 3a70 6f73 3d22 3139 3230 222f 3e3c 773a  :pos="1920"/><w:
+0000a140: 7461 6220 773a 7661 6c3d 226c 6566 7422  tab w:val="left"
+0000a150: 2077 3a70 6f73 3d22 3234 3030 222f 3e3c   w:pos="2400"/><
+0000a160: 773a 7461 6220 773a 7661 6c3d 226c 6566  w:tab w:val="lef
+0000a170: 7422 2077 3a70 6f73 3d22 3238 3830 222f  t" w:pos="2880"/
+0000a180: 3e3c 773a 7461 6220 773a 7661 6c3d 226c  ><w:tab w:val="l
+0000a190: 6566 7422 2077 3a70 6f73 3d22 3333 3630  eft" w:pos="3360
+0000a1a0: 222f 3e3c 773a 7461 6220 773a 7661 6c3d  "/><w:tab w:val=
+0000a1b0: 226c 6566 7422 2077 3a70 6f73 3d22 3338  "left" w:pos="38
+0000a1c0: 3430 222f 3e3c 773a 7461 6220 773a 7661  40"/><w:tab w:va
+0000a1d0: 6c3d 226c 6566 7422 2077 3a70 6f73 3d22  l="left" w:pos="
+0000a1e0: 3433 3230 222f 3e3c 2f77 3a74 6162 733e  4320"/></w:tabs>
+0000a1f0: 3c77 3a73 7061 6369 6e67 2077 3a61 6674  <w:spacing w:aft
+0000a200: 6572 3d22 3022 2f3e 3c2f 773a 7050 723e  er="0"/></w:pPr>
+0000a210: 3c77 3a72 5072 3e3c 773a 7246 6f6e 7473  <w:rPr><w:rFonts
+0000a220: 2077 3a61 7363 6969 3d22 436f 6e73 6f6c   w:ascii="Consol
+0000a230: 6173 2220 773a 6841 6e73 693d 2243 6f6e  as" w:hAnsi="Con
+0000a240: 736f 6c61 7322 2f3e 3c77 3a73 7a20 773a  solas"/><w:sz w:
+0000a250: 7661 6c3d 2232 3022 2f3e 3c77 3a73 7a43  val="20"/><w:szC
+0000a260: 7320 773a 7661 6c3d 2232 3022 2f3e 3c2f  s w:val="20"/></
+0000a270: 773a 7250 723e 3c2f 773a 7374 796c 653e  w:rPr></w:style>
+0000a280: 3c77 3a73 7479 6c65 2077 3a74 7970 653d  <w:style w:type=
+0000a290: 2263 6861 7261 6374 6572 2220 773a 6375  "character" w:cu
+0000a2a0: 7374 6f6d 5374 796c 653d 2231 2220 773a  stomStyle="1" w:
+0000a2b0: 7374 796c 6549 643d 224d 6163 726f 5465  styleId="MacroTe
+0000a2c0: 7874 4368 6172 223e 3c77 3a6e 616d 6520  xtChar"><w:name 
+0000a2d0: 773a 7661 6c3d 224d 6163 726f 2054 6578  w:val="Macro Tex
+0000a2e0: 7420 4368 6172 222f 3e3c 773a 6261 7365  t Char"/><w:base
+0000a2f0: 644f 6e20 773a 7661 6c3d 2244 6566 6175  dOn w:val="Defau
+0000a300: 6c74 5061 7261 6772 6170 6846 6f6e 7422  ltParagraphFont"
+0000a310: 2f3e 3c77 3a6c 696e 6b20 773a 7661 6c3d  /><w:link w:val=
+0000a320: 224d 6163 726f 5465 7874 222f 3e3c 773a  "MacroText"/><w:
+0000a330: 7569 5072 696f 7269 7479 2077 3a76 616c  uiPriority w:val
+0000a340: 3d22 3939 222f 3e3c 773a 7273 6964 2077  ="99"/><w:rsid w
+0000a350: 3a76 616c 3d22 3030 4437 3235 3541 222f  :val="00D7255A"/
+0000a360: 3e3c 773a 7250 723e 3c77 3a72 466f 6e74  ><w:rPr><w:rFont
+0000a370: 7320 773a 6173 6369 693d 2243 6f6e 736f  s w:ascii="Conso
+0000a380: 6c61 7322 2077 3a68 416e 7369 3d22 436f  las" w:hAnsi="Co
+0000a390: 6e73 6f6c 6173 222f 3e3c 773a 737a 2077  nsolas"/><w:sz w
+0000a3a0: 3a76 616c 3d22 3230 222f 3e3c 773a 737a  :val="20"/><w:sz
+0000a3b0: 4373 2077 3a76 616c 3d22 3230 222f 3e3c  Cs w:val="20"/><
+0000a3c0: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
+0000a3d0: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
+0000a3e0: 3d22 6368 6172 6163 7465 7222 2077 3a73  ="character" w:s
+0000a3f0: 7479 6c65 4964 3d22 4d65 6e74 696f 6e22  tyleId="Mention"
+0000a400: 3e3c 773a 6e61 6d65 2077 3a76 616c 3d22  ><w:name w:val="
+0000a410: 4d65 6e74 696f 6e22 2f3e 3c77 3a62 6173  Mention"/><w:bas
+0000a420: 6564 4f6e 2077 3a76 616c 3d22 4465 6661  edOn w:val="Defa
+0000a430: 756c 7450 6172 6167 7261 7068 466f 6e74  ultParagraphFont
+0000a440: 222f 3e3c 773a 7569 5072 696f 7269 7479  "/><w:uiPriority
+0000a450: 2077 3a76 616c 3d22 3939 222f 3e3c 773a   w:val="99"/><w:
+0000a460: 756e 6869 6465 5768 656e 5573 6564 2f3e  unhideWhenUsed/>
+0000a470: 3c77 3a72 7369 6420 773a 7661 6c3d 2230  <w:rsid w:val="0
+0000a480: 3044 3732 3535 4122 2f3e 3c77 3a72 5072  0D7255A"/><w:rPr
+0000a490: 3e3c 773a 636f 6c6f 7220 773a 7661 6c3d  ><w:color w:val=
+0000a4a0: 2232 4235 3739 4122 2f3e 3c77 3a73 6864  "2B579A"/><w:shd
+0000a4b0: 2077 3a76 616c 3d22 636c 6561 7222 2077   w:val="clear" w
+0000a4c0: 3a63 6f6c 6f72 3d22 6175 746f 2220 773a  :color="auto" w:
+0000a4d0: 6669 6c6c 3d22 4531 4446 4444 222f 3e3c  fill="E1DFDD"/><
+0000a4e0: 2f77 3a72 5072 3e3c 2f77 3a73 7479 6c65  /w:rPr></w:style
+0000a4f0: 3e3c 773a 7374 796c 6520 773a 7479 7065  ><w:style w:type
+0000a500: 3d22 7061 7261 6772 6170 6822 2077 3a73  ="paragraph" w:s
+0000a510: 7479 6c65 4964 3d22 4d65 7373 6167 6548  tyleId="MessageH
+0000a520: 6561 6465 7222 3e3c 773a 6e61 6d65 2077  eader"><w:name w
+0000a530: 3a76 616c 3d22 4d65 7373 6167 6520 4865  :val="Message He
+0000a540: 6164 6572 222f 3e3c 773a 6261 7365 644f  ader"/><w:basedO
+0000a550: 6e20 773a 7661 6c3d 224e 6f72 6d61 6c22  n w:val="Normal"
+0000a560: 2f3e 3c77 3a6c 696e 6b20 773a 7661 6c3d  /><w:link w:val=
+0000a570: 224d 6573 7361 6765 4865 6164 6572 4368  "MessageHeaderCh
+0000a580: 6172 222f 3e3c 773a 7569 5072 696f 7269  ar"/><w:uiPriori
+0000a590: 7479 2077 3a76 616c 3d22 3939 222f 3e3c  ty w:val="99"/><
+0000a5a0: 773a 756e 6869 6465 5768 656e 5573 6564  w:unhideWhenUsed
+0000a5b0: 2f3e 3c77 3a72 7369 6420 773a 7661 6c3d  /><w:rsid w:val=
+0000a5c0: 2230 3044 3732 3535 4122 2f3e 3c77 3a70  "00D7255A"/><w:p
+0000a5d0: 5072 3e3c 773a 7042 6472 3e3c 773a 746f  Pr><w:pBdr><w:to
+0000a5e0: 7020 773a 7661 6c3d 2273 696e 676c 6522  p w:val="single"
+0000a5f0: 2077 3a73 7a3d 2236 2220 773a 7370 6163   w:sz="6" w:spac
+0000a600: 653d 2231 2220 773a 636f 6c6f 723d 2261  e="1" w:color="a
+0000a610: 7574 6f22 2f3e 3c77 3a6c 6566 7420 773a  uto"/><w:left w:
+0000a620: 7661 6c3d 2273 696e 676c 6522 2077 3a73  val="single" w:s
+0000a630: 7a3d 2236 2220 773a 7370 6163 653d 2231  z="6" w:space="1
+0000a640: 2220 773a 636f 6c6f 723d 2261 7574 6f22  " w:color="auto"
+0000a650: 2f3e 3c77 3a62 6f74 746f 6d20 773a 7661  /><w:bottom w:va
+0000a660: 6c3d 2273 696e 676c 6522 2077 3a73 7a3d  l="single" w:sz=
+0000a670: 2236 2220 773a 7370 6163 653d 2231 2220  "6" w:space="1" 
+0000a680: 773a 636f 6c6f 723d 2261 7574 6f22 2f3e  w:color="auto"/>
+0000a690: 3c77 3a72 6967 6874 2077 3a76 616c 3d22  <w:right w:val="
+0000a6a0: 7369 6e67 6c65 2220 773a 737a 3d22 3622  single" w:sz="6"
+0000a6b0: 2077 3a73 7061 6365 3d22 3122 2077 3a63   w:space="1" w:c
+0000a6c0: 6f6c 6f72 3d22 6175 746f 222f 3e3c 2f77  olor="auto"/></w
+0000a6d0: 3a70 4264 723e 3c77 3a73 6864 2077 3a76  :pBdr><w:shd w:v
+0000a6e0: 616c 3d22 7063 7432 3022 2077 3a63 6f6c  al="pct20" w:col
+0000a6f0: 6f72 3d22 6175 746f 2220 773a 6669 6c6c  or="auto" w:fill
+0000a700: 3d22 6175 746f 222f 3e3c 773a 7370 6163  ="auto"/><w:spac
+0000a710: 696e 6720 773a 6166 7465 723d 2230 2220  ing w:after="0" 
+0000a720: 773a 6c69 6e65 3d22 3234 3022 2077 3a6c  w:line="240" w:l
+0000a730: 696e 6552 756c 653d 2261 7574 6f22 2f3e  ineRule="auto"/>
+0000a740: 3c77 3a69 6e64 2077 3a6c 6566 743d 2231  <w:ind w:left="1
+0000a750: 3133 3422 2077 3a68 616e 6769 6e67 3d22  134" w:hanging="
+0000a760: 3131 3334 222f 3e3c 2f77 3a70 5072 3e3c  1134"/></w:pPr><
+0000a770: 773a 7250 723e 3c77 3a72 466f 6e74 7320  w:rPr><w:rFonts 
+0000a780: 773a 6173 6369 6954 6865 6d65 3d22 6d61  w:asciiTheme="ma
+0000a790: 6a6f 7248 416e 7369 2220 773a 6561 7374  jorHAnsi" w:east
+0000a7a0: 4173 6961 5468 656d 653d 226d 616a 6f72  AsiaTheme="major
+0000a7b0: 4561 7374 4173 6961 2220 773a 6841 6e73  EastAsia" w:hAns
+0000a7c0: 6954 6865 6d65 3d22 6d61 6a6f 7248 416e  iTheme="majorHAn
+0000a7d0: 7369 2220 773a 6373 7468 656d 653d 226d  si" w:cstheme="m
+0000a7e0: 616a 6f72 4269 6469 222f 3e3c 773a 737a  ajorBidi"/><w:sz
+0000a7f0: 2077 3a76 616c 3d22 3234 222f 3e3c 773a   w:val="24"/><w:
+0000a800: 737a 4373 2077 3a76 616c 3d22 3234 222f  szCs w:val="24"/
+0000a810: 3e3c 2f77 3a72 5072 3e3c 2f77 3a73 7479  ></w:rPr></w:sty
+0000a820: 6c65 3e3c 773a 7374 796c 6520 773a 7479  le><w:style w:ty
+0000a830: 7065 3d22 6368 6172 6163 7465 7222 2077  pe="character" w
+0000a840: 3a63 7573 746f 6d53 7479 6c65 3d22 3122  :customStyle="1"
+0000a850: 2077 3a73 7479 6c65 4964 3d22 4d65 7373   w:styleId="Mess
+0000a860: 6167 6548 6561 6465 7243 6861 7222 3e3c  ageHeaderChar"><
+0000a870: 773a 6e61 6d65 2077 3a76 616c 3d22 4d65  w:name w:val="Me
+0000a880: 7373 6167 6520 4865 6164 6572 2043 6861  ssage Header Cha
+0000a890: 7222 2f3e 3c77 3a62 6173 6564 4f6e 2077  r"/><w:basedOn w
+0000a8a0: 3a76 616c 3d22 4465 6661 756c 7450 6172  :val="DefaultPar
+0000a8b0: 6167 7261 7068 466f 6e74 222f 3e3c 773a  agraphFont"/><w:
+0000a8c0: 6c69 6e6b 2077 3a76 616c 3d22 4d65 7373  link w:val="Mess
+0000a8d0: 6167 6548 6561 6465 7222 2f3e 3c77 3a75  ageHeader"/><w:u
+0000a8e0: 6950 7269 6f72 6974 7920 773a 7661 6c3d  iPriority w:val=
+0000a8f0: 2239 3922 2f3e 3c77 3a72 7369 6420 773a  "99"/><w:rsid w:
+0000a900: 7661 6c3d 2230 3044 3732 3535 4122 2f3e  val="00D7255A"/>
+0000a910: 3c77 3a72 5072 3e3c 773a 7246 6f6e 7473  <w:rPr><w:rFonts
+0000a920: 2077 3a61 7363 6969 5468 656d 653d 226d   w:asciiTheme="m
+0000a930: 616a 6f72 4841 6e73 6922 2077 3a65 6173  ajorHAnsi" w:eas
+0000a940: 7441 7369 6154 6865 6d65 3d22 6d61 6a6f  tAsiaTheme="majo
+0000a950: 7245 6173 7441 7369 6122 2077 3a68 416e  rEastAsia" w:hAn
+0000a960: 7369 5468 656d 653d 226d 616a 6f72 4841  siTheme="majorHA
+0000a970: 6e73 6922 2077 3a63 7374 6865 6d65 3d22  nsi" w:cstheme="
+0000a980: 6d61 6a6f 7242 6964 6922 2f3e 3c77 3a73  majorBidi"/><w:s
+0000a990: 7a20 773a 7661 6c3d 2232 3422 2f3e 3c77  z w:val="24"/><w
+0000a9a0: 3a73 7a43 7320 773a 7661 6c3d 2232 3422  :szCs w:val="24"
+0000a9b0: 2f3e 3c77 3a73 6864 2077 3a76 616c 3d22  /><w:shd w:val="
+0000a9c0: 7063 7432 3022 2077 3a63 6f6c 6f72 3d22  pct20" w:color="
+0000a9d0: 6175 746f 2220 773a 6669 6c6c 3d22 6175  auto" w:fill="au
+0000a9e0: 746f 222f 3e3c 2f77 3a72 5072 3e3c 2f77  to"/></w:rPr></w
+0000a9f0: 3a73 7479 6c65 3e3c 773a 7374 796c 6520  :style><w:style 
+0000aa00: 773a 7479 7065 3d22 7061 7261 6772 6170  w:type="paragrap
+0000aa10: 6822 2077 3a73 7479 6c65 4964 3d22 506c  h" w:styleId="Pl
+0000aa20: 6169 6e54 6578 7422 3e3c 773a 6e61 6d65  ainText"><w:name
+0000aa30: 2077 3a76 616c 3d22 506c 6169 6e20 5465   w:val="Plain Te
+0000aa40: 7874 222f 3e3c 773a 6261 7365 644f 6e20  xt"/><w:basedOn 
+0000aa50: 773a 7661 6c3d 224e 6f72 6d61 6c22 2f3e  w:val="Normal"/>
+0000aa60: 3c77 3a6c 696e 6b20 773a 7661 6c3d 2250  <w:link w:val="P
+0000aa70: 6c61 696e 5465 7874 4368 6172 222f 3e3c  lainTextChar"/><
+0000aa80: 773a 7569 5072 696f 7269 7479 2077 3a76  w:uiPriority w:v
+0000aa90: 616c 3d22 3939 222f 3e3c 773a 756e 6869  al="99"/><w:unhi
+0000aaa0: 6465 5768 656e 5573 6564 2f3e 3c77 3a72  deWhenUsed/><w:r
+0000aab0: 7369 6420 773a 7661 6c3d 2230 3044 3732  sid w:val="00D72
+0000aac0: 3535 4122 2f3e 3c77 3a70 5072 3e3c 773a  55A"/><w:pPr><w:
+0000aad0: 7370 6163 696e 6720 773a 6166 7465 723d  spacing w:after=
+0000aae0: 2230 2220 773a 6c69 6e65 3d22 3234 3022  "0" w:line="240"
+0000aaf0: 2077 3a6c 696e 6552 756c 653d 2261 7574   w:lineRule="aut
+0000ab00: 6f22 2f3e 3c2f 773a 7050 723e 3c77 3a72  o"/></w:pPr><w:r
+0000ab10: 5072 3e3c 773a 7246 6f6e 7473 2077 3a61  Pr><w:rFonts w:a
+0000ab20: 7363 6969 3d22 436f 6e73 6f6c 6173 2220  scii="Consolas" 
+0000ab30: 773a 6841 6e73 693d 2243 6f6e 736f 6c61  w:hAnsi="Consola
+0000ab40: 7322 2f3e 3c77 3a73 7a20 773a 7661 6c3d  s"/><w:sz w:val=
+0000ab50: 2232 3122 2f3e 3c77 3a73 7a43 7320 773a  "21"/><w:szCs w:
+0000ab60: 7661 6c3d 2232 3122 2f3e 3c2f 773a 7250  val="21"/></w:rP
+0000ab70: 723e 3c2f 773a 7374 796c 653e 3c77 3a73  r></w:style><w:s
+0000ab80: 7479 6c65 2077 3a74 7970 653d 2263 6861  tyle w:type="cha
+0000ab90: 7261 6374 6572 2220 773a 6375 7374 6f6d  racter" w:custom
+0000aba0: 5374 796c 653d 2231 2220 773a 7374 796c  Style="1" w:styl
+0000abb0: 6549 643d 2250 6c61 696e 5465 7874 4368  eId="PlainTextCh
+0000abc0: 6172 223e 3c77 3a6e 616d 6520 773a 7661  ar"><w:name w:va
+0000abd0: 6c3d 2250 6c61 696e 2054 6578 7420 4368  l="Plain Text Ch
+0000abe0: 6172 222f 3e3c 773a 6261 7365 644f 6e20  ar"/><w:basedOn 
+0000abf0: 773a 7661 6c3d 2244 6566 6175 6c74 5061  w:val="DefaultPa
+0000ac00: 7261 6772 6170 6846 6f6e 7422 2f3e 3c77  ragraphFont"/><w
+0000ac10: 3a6c 696e 6b20 773a 7661 6c3d 2250 6c61  :link w:val="Pla
+0000ac20: 696e 5465 7874 222f 3e3c 773a 7569 5072  inText"/><w:uiPr
+0000ac30: 696f 7269 7479 2077 3a76 616c 3d22 3939  iority w:val="99
+0000ac40: 222f 3e3c 773a 7273 6964 2077 3a76 616c  "/><w:rsid w:val
+0000ac50: 3d22 3030 4437 3235 3541 222f 3e3c 773a  ="00D7255A"/><w:
+0000ac60: 7250 723e 3c77 3a72 466f 6e74 7320 773a  rPr><w:rFonts w:
+0000ac70: 6173 6369 693d 2243 6f6e 736f 6c61 7322  ascii="Consolas"
+0000ac80: 2077 3a68 416e 7369 3d22 436f 6e73 6f6c   w:hAnsi="Consol
+0000ac90: 6173 222f 3e3c 773a 737a 2077 3a76 616c  as"/><w:sz w:val
+0000aca0: 3d22 3231 222f 3e3c 773a 737a 4373 2077  ="21"/><w:szCs w
+0000acb0: 3a76 616c 3d22 3231 222f 3e3c 2f77 3a72  :val="21"/></w:r
+0000acc0: 5072 3e3c 2f77 3a73 7479 6c65 3e3c 2f77  Pr></w:style></w
+0000acd0: 3a73 7479 6c65 733e                      :styles>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/theme/theme1.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/theme/theme1.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, Unicode text, UTF-8 text, with very long lines (8280), with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -1,525 +1,525 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 613a 7468 656d  "yes"?>..<a:them
-00000040: 6520 786d 6c6e 733a 613d 2268 7474 703a  e xmlns:a="http:
-00000050: 2f2f 7363 6865 6d61 732e 6f70 656e 786d  //schemas.openxm
-00000060: 6c66 6f72 6d61 7473 2e6f 7267 2f64 7261  lformats.org/dra
-00000070: 7769 6e67 6d6c 2f32 3030 362f 6d61 696e  wingml/2006/main
-00000080: 2220 6e61 6d65 3d22 4f66 6669 6365 2054  " name="Office T
-00000090: 6865 6d65 223e 3c61 3a74 6865 6d65 456c  heme"><a:themeEl
-000000a0: 656d 656e 7473 3e3c 613a 636c 7253 6368  ements><a:clrSch
-000000b0: 656d 6520 6e61 6d65 3d22 4f66 6669 6365  eme name="Office
-000000c0: 223e 3c61 3a64 6b31 3e3c 613a 7379 7343  "><a:dk1><a:sysC
-000000d0: 6c72 2076 616c 3d22 7769 6e64 6f77 5465  lr val="windowTe
-000000e0: 7874 2220 6c61 7374 436c 723d 2230 3030  xt" lastClr="000
-000000f0: 3030 3022 2f3e 3c2f 613a 646b 313e 3c61  000"/></a:dk1><a
-00000100: 3a6c 7431 3e3c 613a 7379 7343 6c72 2076  :lt1><a:sysClr v
-00000110: 616c 3d22 7769 6e64 6f77 2220 6c61 7374  al="window" last
-00000120: 436c 723d 2246 4646 4646 4622 2f3e 3c2f  Clr="FFFFFF"/></
-00000130: 613a 6c74 313e 3c61 3a64 6b32 3e3c 613a  a:lt1><a:dk2><a:
-00000140: 7372 6762 436c 7220 7661 6c3d 2234 3435  srgbClr val="445
-00000150: 3436 4122 2f3e 3c2f 613a 646b 323e 3c61  46A"/></a:dk2><a
-00000160: 3a6c 7432 3e3c 613a 7372 6762 436c 7220  :lt2><a:srgbClr 
-00000170: 7661 6c3d 2245 3745 3645 3622 2f3e 3c2f  val="E7E6E6"/></
-00000180: 613a 6c74 323e 3c61 3a61 6363 656e 7431  a:lt2><a:accent1
-00000190: 3e3c 613a 7372 6762 436c 7220 7661 6c3d  ><a:srgbClr val=
-000001a0: 2234 3437 3243 3422 2f3e 3c2f 613a 6163  "4472C4"/></a:ac
-000001b0: 6365 6e74 313e 3c61 3a61 6363 656e 7432  cent1><a:accent2
-000001c0: 3e3c 613a 7372 6762 436c 7220 7661 6c3d  ><a:srgbClr val=
-000001d0: 2245 4437 4433 3122 2f3e 3c2f 613a 6163  "ED7D31"/></a:ac
-000001e0: 6365 6e74 323e 3c61 3a61 6363 656e 7433  cent2><a:accent3
-000001f0: 3e3c 613a 7372 6762 436c 7220 7661 6c3d  ><a:srgbClr val=
-00000200: 2241 3541 3541 3522 2f3e 3c2f 613a 6163  "A5A5A5"/></a:ac
-00000210: 6365 6e74 333e 3c61 3a61 6363 656e 7434  cent3><a:accent4
-00000220: 3e3c 613a 7372 6762 436c 7220 7661 6c3d  ><a:srgbClr val=
-00000230: 2246 4643 3030 3022 2f3e 3c2f 613a 6163  "FFC000"/></a:ac
-00000240: 6365 6e74 343e 3c61 3a61 6363 656e 7435  cent4><a:accent5
-00000250: 3e3c 613a 7372 6762 436c 7220 7661 6c3d  ><a:srgbClr val=
-00000260: 2235 4239 4244 3522 2f3e 3c2f 613a 6163  "5B9BD5"/></a:ac
-00000270: 6365 6e74 353e 3c61 3a61 6363 656e 7436  cent5><a:accent6
-00000280: 3e3c 613a 7372 6762 436c 7220 7661 6c3d  ><a:srgbClr val=
-00000290: 2237 3041 4434 3722 2f3e 3c2f 613a 6163  "70AD47"/></a:ac
-000002a0: 6365 6e74 363e 3c61 3a68 6c69 6e6b 3e3c  cent6><a:hlink><
-000002b0: 613a 7372 6762 436c 7220 7661 6c3d 2230  a:srgbClr val="0
-000002c0: 3536 3343 3122 2f3e 3c2f 613a 686c 696e  563C1"/></a:hlin
-000002d0: 6b3e 3c61 3a66 6f6c 486c 696e 6b3e 3c61  k><a:folHlink><a
-000002e0: 3a73 7267 6243 6c72 2076 616c 3d22 3935  :srgbClr val="95
-000002f0: 3446 3732 222f 3e3c 2f61 3a66 6f6c 486c  4F72"/></a:folHl
-00000300: 696e 6b3e 3c2f 613a 636c 7253 6368 656d  ink></a:clrSchem
-00000310: 653e 3c61 3a66 6f6e 7453 6368 656d 6520  e><a:fontScheme 
-00000320: 6e61 6d65 3d22 4f66 6669 6365 223e 3c61  name="Office"><a
-00000330: 3a6d 616a 6f72 466f 6e74 3e3c 613a 6c61  :majorFont><a:la
-00000340: 7469 6e20 7479 7065 6661 6365 3d22 4361  tin typeface="Ca
-00000350: 6c69 6272 6920 4c69 6768 7422 2070 616e  libri Light" pan
-00000360: 6f73 653d 2230 3230 4630 3330 3230 3230  ose="020F0302020
-00000370: 3230 3430 3330 3230 3422 2f3e 3c61 3a65  204030204"/><a:e
-00000380: 6120 7479 7065 6661 6365 3d22 222f 3e3c  a typeface=""/><
-00000390: 613a 6373 2074 7970 6566 6163 653d 2222  a:cs typeface=""
-000003a0: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-000003b0: 3d22 4a70 616e 2220 7479 7065 6661 6365  ="Jpan" typeface
-000003c0: 3d22 e6b8 b8e3 82b4 e382 b7e3 8383 e382  ="..............
-000003d0: af20 4c69 6768 7422 2f3e 3c61 3a66 6f6e  . Light"/><a:fon
-000003e0: 7420 7363 7269 7074 3d22 4861 6e67 2220  t script="Hang" 
-000003f0: 7479 7065 6661 6365 3d22 eba7 91ec 9d80  typeface="......
-00000400: 20ea b3a0 eb94 9522 2f3e 3c61 3a66 6f6e   ......"/><a:fon
-00000410: 7420 7363 7269 7074 3d22 4861 6e73 2220  t script="Hans" 
-00000420: 7479 7065 6661 6365 3d22 e7ad 89e7 babf  typeface="......
-00000430: 204c 6967 6874 222f 3e3c 613a 666f 6e74   Light"/><a:font
-00000440: 2073 6372 6970 743d 2248 616e 7422 2074   script="Hant" t
-00000450: 7970 6566 6163 653d 22e6 96b0 e7b4 b0e6  ypeface=".......
-00000460: 988e e9ab 9422 2f3e 3c61 3a66 6f6e 7420  ....."/><a:font 
-00000470: 7363 7269 7074 3d22 4172 6162 2220 7479  script="Arab" ty
-00000480: 7065 6661 6365 3d22 5469 6d65 7320 4e65  peface="Times Ne
-00000490: 7720 526f 6d61 6e22 2f3e 3c61 3a66 6f6e  w Roman"/><a:fon
-000004a0: 7420 7363 7269 7074 3d22 4865 6272 2220  t script="Hebr" 
-000004b0: 7479 7065 6661 6365 3d22 5469 6d65 7320  typeface="Times 
-000004c0: 4e65 7720 526f 6d61 6e22 2f3e 3c61 3a66  New Roman"/><a:f
-000004d0: 6f6e 7420 7363 7269 7074 3d22 5468 6169  ont script="Thai
-000004e0: 2220 7479 7065 6661 6365 3d22 416e 6773  " typeface="Angs
-000004f0: 616e 6120 4e65 7722 2f3e 3c61 3a66 6f6e  ana New"/><a:fon
-00000500: 7420 7363 7269 7074 3d22 4574 6869 2220  t script="Ethi" 
-00000510: 7479 7065 6661 6365 3d22 4e79 616c 6122  typeface="Nyala"
-00000520: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-00000530: 3d22 4265 6e67 2220 7479 7065 6661 6365  ="Beng" typeface
-00000540: 3d22 5672 696e 6461 222f 3e3c 613a 666f  ="Vrinda"/><a:fo
-00000550: 6e74 2073 6372 6970 743d 2247 756a 7222  nt script="Gujr"
-00000560: 2074 7970 6566 6163 653d 2253 6872 7574   typeface="Shrut
-00000570: 6922 2f3e 3c61 3a66 6f6e 7420 7363 7269  i"/><a:font scri
-00000580: 7074 3d22 4b68 6d72 2220 7479 7065 6661  pt="Khmr" typefa
-00000590: 6365 3d22 4d6f 6f6c 426f 7261 6e22 2f3e  ce="MoolBoran"/>
-000005a0: 3c61 3a66 6f6e 7420 7363 7269 7074 3d22  <a:font script="
-000005b0: 4b6e 6461 2220 7479 7065 6661 6365 3d22  Knda" typeface="
-000005c0: 5475 6e67 6122 2f3e 3c61 3a66 6f6e 7420  Tunga"/><a:font 
-000005d0: 7363 7269 7074 3d22 4775 7275 2220 7479  script="Guru" ty
-000005e0: 7065 6661 6365 3d22 5261 6176 6922 2f3e  peface="Raavi"/>
-000005f0: 3c61 3a66 6f6e 7420 7363 7269 7074 3d22  <a:font script="
-00000600: 4361 6e73 2220 7479 7065 6661 6365 3d22  Cans" typeface="
-00000610: 4575 7068 656d 6961 222f 3e3c 613a 666f  Euphemia"/><a:fo
-00000620: 6e74 2073 6372 6970 743d 2243 6865 7222  nt script="Cher"
-00000630: 2074 7970 6566 6163 653d 2250 6c61 6e74   typeface="Plant
-00000640: 6167 656e 6574 2043 6865 726f 6b65 6522  agenet Cherokee"
-00000650: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-00000660: 3d22 5969 6969 2220 7479 7065 6661 6365  ="Yiii" typeface
-00000670: 3d22 4d69 6372 6f73 6f66 7420 5969 2042  ="Microsoft Yi B
-00000680: 6169 7469 222f 3e3c 613a 666f 6e74 2073  aiti"/><a:font s
-00000690: 6372 6970 743d 2254 6962 7422 2074 7970  cript="Tibt" typ
-000006a0: 6566 6163 653d 224d 6963 726f 736f 6674  eface="Microsoft
-000006b0: 2048 696d 616c 6179 6122 2f3e 3c61 3a66   Himalaya"/><a:f
-000006c0: 6f6e 7420 7363 7269 7074 3d22 5468 6161  ont script="Thaa
-000006d0: 2220 7479 7065 6661 6365 3d22 4d56 2042  " typeface="MV B
-000006e0: 6f6c 6922 2f3e 3c61 3a66 6f6e 7420 7363  oli"/><a:font sc
-000006f0: 7269 7074 3d22 4465 7661 2220 7479 7065  ript="Deva" type
-00000700: 6661 6365 3d22 4d61 6e67 616c 222f 3e3c  face="Mangal"/><
-00000710: 613a 666f 6e74 2073 6372 6970 743d 2254  a:font script="T
-00000720: 656c 7522 2074 7970 6566 6163 653d 2247  elu" typeface="G
-00000730: 6175 7461 6d69 222f 3e3c 613a 666f 6e74  autami"/><a:font
-00000740: 2073 6372 6970 743d 2254 616d 6c22 2074   script="Taml" t
-00000750: 7970 6566 6163 653d 224c 6174 6861 222f  ypeface="Latha"/
-00000760: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
-00000770: 2253 7972 6322 2074 7970 6566 6163 653d  "Syrc" typeface=
-00000780: 2245 7374 7261 6e67 656c 6f20 4564 6573  "Estrangelo Edes
-00000790: 7361 222f 3e3c 613a 666f 6e74 2073 6372  sa"/><a:font scr
-000007a0: 6970 743d 224f 7279 6122 2074 7970 6566  ipt="Orya" typef
-000007b0: 6163 653d 224b 616c 696e 6761 222f 3e3c  ace="Kalinga"/><
-000007c0: 613a 666f 6e74 2073 6372 6970 743d 224d  a:font script="M
-000007d0: 6c79 6d22 2074 7970 6566 6163 653d 224b  lym" typeface="K
-000007e0: 6172 7469 6b61 222f 3e3c 613a 666f 6e74  artika"/><a:font
-000007f0: 2073 6372 6970 743d 224c 616f 6f22 2074   script="Laoo" t
-00000800: 7970 6566 6163 653d 2244 6f6b 4368 616d  ypeface="DokCham
-00000810: 7061 222f 3e3c 613a 666f 6e74 2073 6372  pa"/><a:font scr
-00000820: 6970 743d 2253 696e 6822 2074 7970 6566  ipt="Sinh" typef
-00000830: 6163 653d 2249 736b 6f6f 6c61 2050 6f74  ace="Iskoola Pot
-00000840: 6122 2f3e 3c61 3a66 6f6e 7420 7363 7269  a"/><a:font scri
-00000850: 7074 3d22 4d6f 6e67 2220 7479 7065 6661  pt="Mong" typefa
-00000860: 6365 3d22 4d6f 6e67 6f6c 6961 6e20 4261  ce="Mongolian Ba
-00000870: 6974 6922 2f3e 3c61 3a66 6f6e 7420 7363  iti"/><a:font sc
-00000880: 7269 7074 3d22 5669 6574 2220 7479 7065  ript="Viet" type
-00000890: 6661 6365 3d22 5469 6d65 7320 4e65 7720  face="Times New 
-000008a0: 526f 6d61 6e22 2f3e 3c61 3a66 6f6e 7420  Roman"/><a:font 
-000008b0: 7363 7269 7074 3d22 5569 6768 2220 7479  script="Uigh" ty
-000008c0: 7065 6661 6365 3d22 4d69 6372 6f73 6f66  peface="Microsof
-000008d0: 7420 5569 6768 7572 222f 3e3c 613a 666f  t Uighur"/><a:fo
-000008e0: 6e74 2073 6372 6970 743d 2247 656f 7222  nt script="Geor"
-000008f0: 2074 7970 6566 6163 653d 2253 796c 6661   typeface="Sylfa
-00000900: 656e 222f 3e3c 613a 666f 6e74 2073 6372  en"/><a:font scr
-00000910: 6970 743d 2241 726d 6e22 2074 7970 6566  ipt="Armn" typef
-00000920: 6163 653d 2241 7269 616c 222f 3e3c 613a  ace="Arial"/><a:
-00000930: 666f 6e74 2073 6372 6970 743d 2242 7567  font script="Bug
-00000940: 6922 2074 7970 6566 6163 653d 224c 6565  i" typeface="Lee
-00000950: 6c61 7761 6465 6520 5549 222f 3e3c 613a  lawadee UI"/><a:
-00000960: 666f 6e74 2073 6372 6970 743d 2242 6f70  font script="Bop
-00000970: 6f22 2074 7970 6566 6163 653d 224d 6963  o" typeface="Mic
-00000980: 726f 736f 6674 204a 6865 6e67 4865 6922  rosoft JhengHei"
-00000990: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-000009a0: 3d22 4a61 7661 2220 7479 7065 6661 6365  ="Java" typeface
-000009b0: 3d22 4a61 7661 6e65 7365 2054 6578 7422  ="Javanese Text"
-000009c0: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-000009d0: 3d22 4c69 7375 2220 7479 7065 6661 6365  ="Lisu" typeface
-000009e0: 3d22 5365 676f 6520 5549 222f 3e3c 613a  ="Segoe UI"/><a:
-000009f0: 666f 6e74 2073 6372 6970 743d 224d 796d  font script="Mym
-00000a00: 7222 2074 7970 6566 6163 653d 224d 7961  r" typeface="Mya
-00000a10: 6e6d 6172 2054 6578 7422 2f3e 3c61 3a66  nmar Text"/><a:f
-00000a20: 6f6e 7420 7363 7269 7074 3d22 4e6b 6f6f  ont script="Nkoo
-00000a30: 2220 7479 7065 6661 6365 3d22 4562 7269  " typeface="Ebri
-00000a40: 6d61 222f 3e3c 613a 666f 6e74 2073 6372  ma"/><a:font scr
-00000a50: 6970 743d 224f 6c63 6b22 2074 7970 6566  ipt="Olck" typef
-00000a60: 6163 653d 224e 6972 6d61 6c61 2055 4922  ace="Nirmala UI"
-00000a70: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-00000a80: 3d22 4f73 6d61 2220 7479 7065 6661 6365  ="Osma" typeface
-00000a90: 3d22 4562 7269 6d61 222f 3e3c 613a 666f  ="Ebrima"/><a:fo
-00000aa0: 6e74 2073 6372 6970 743d 2250 6861 6722  nt script="Phag"
-00000ab0: 2074 7970 6566 6163 653d 2250 6861 6773   typeface="Phags
-00000ac0: 7061 222f 3e3c 613a 666f 6e74 2073 6372  pa"/><a:font scr
-00000ad0: 6970 743d 2253 7972 6e22 2074 7970 6566  ipt="Syrn" typef
-00000ae0: 6163 653d 2245 7374 7261 6e67 656c 6f20  ace="Estrangelo 
-00000af0: 4564 6573 7361 222f 3e3c 613a 666f 6e74  Edessa"/><a:font
-00000b00: 2073 6372 6970 743d 2253 7972 6a22 2074   script="Syrj" t
-00000b10: 7970 6566 6163 653d 2245 7374 7261 6e67  ypeface="Estrang
-00000b20: 656c 6f20 4564 6573 7361 222f 3e3c 613a  elo Edessa"/><a:
-00000b30: 666f 6e74 2073 6372 6970 743d 2253 7972  font script="Syr
-00000b40: 6522 2074 7970 6566 6163 653d 2245 7374  e" typeface="Est
-00000b50: 7261 6e67 656c 6f20 4564 6573 7361 222f  rangelo Edessa"/
-00000b60: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
-00000b70: 2253 6f72 6122 2074 7970 6566 6163 653d  "Sora" typeface=
-00000b80: 224e 6972 6d61 6c61 2055 4922 2f3e 3c61  "Nirmala UI"/><a
-00000b90: 3a66 6f6e 7420 7363 7269 7074 3d22 5461  :font script="Ta
-00000ba0: 6c65 2220 7479 7065 6661 6365 3d22 4d69  le" typeface="Mi
-00000bb0: 6372 6f73 6f66 7420 5461 6920 4c65 222f  crosoft Tai Le"/
-00000bc0: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
-00000bd0: 2254 616c 7522 2074 7970 6566 6163 653d  "Talu" typeface=
-00000be0: 224d 6963 726f 736f 6674 204e 6577 2054  "Microsoft New T
-00000bf0: 6169 204c 7565 222f 3e3c 613a 666f 6e74  ai Lue"/><a:font
-00000c00: 2073 6372 6970 743d 2254 666e 6722 2074   script="Tfng" t
-00000c10: 7970 6566 6163 653d 2245 6272 696d 6122  ypeface="Ebrima"
-00000c20: 2f3e 3c2f 613a 6d61 6a6f 7246 6f6e 743e  /></a:majorFont>
-00000c30: 3c61 3a6d 696e 6f72 466f 6e74 3e3c 613a  <a:minorFont><a:
-00000c40: 6c61 7469 6e20 7479 7065 6661 6365 3d22  latin typeface="
-00000c50: 4361 6c69 6272 6922 2070 616e 6f73 653d  Calibri" panose=
-00000c60: 2230 3230 4630 3530 3230 3230 3230 3430  "020F05020202040
-00000c70: 3330 3230 3422 2f3e 3c61 3a65 6120 7479  30204"/><a:ea ty
-00000c80: 7065 6661 6365 3d22 222f 3e3c 613a 6373  peface=""/><a:cs
-00000c90: 2074 7970 6566 6163 653d 2222 2f3e 3c61   typeface=""/><a
-00000ca0: 3a66 6f6e 7420 7363 7269 7074 3d22 4a70  :font script="Jp
-00000cb0: 616e 2220 7479 7065 6661 6365 3d22 e6b8  an" typeface="..
-00000cc0: b8e6 988e e69c 9d22 2f3e 3c61 3a66 6f6e  ......."/><a:fon
-00000cd0: 7420 7363 7269 7074 3d22 4861 6e67 2220  t script="Hang" 
-00000ce0: 7479 7065 6661 6365 3d22 eba7 91ec 9d80  typeface="......
-00000cf0: 20ea b3a0 eb94 9522 2f3e 3c61 3a66 6f6e   ......"/><a:fon
-00000d00: 7420 7363 7269 7074 3d22 4861 6e73 2220  t script="Hans" 
-00000d10: 7479 7065 6661 6365 3d22 e7ad 89e7 babf  typeface="......
-00000d20: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
-00000d30: 743d 2248 616e 7422 2074 7970 6566 6163  t="Hant" typefac
-00000d40: 653d 22e6 96b0 e7b4 b0e6 988e e9ab 9422  e="............"
-00000d50: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-00000d60: 3d22 4172 6162 2220 7479 7065 6661 6365  ="Arab" typeface
-00000d70: 3d22 4172 6961 6c22 2f3e 3c61 3a66 6f6e  ="Arial"/><a:fon
-00000d80: 7420 7363 7269 7074 3d22 4865 6272 2220  t script="Hebr" 
-00000d90: 7479 7065 6661 6365 3d22 4172 6961 6c22  typeface="Arial"
-00000da0: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-00000db0: 3d22 5468 6169 2220 7479 7065 6661 6365  ="Thai" typeface
-00000dc0: 3d22 436f 7264 6961 204e 6577 222f 3e3c  ="Cordia New"/><
-00000dd0: 613a 666f 6e74 2073 6372 6970 743d 2245  a:font script="E
-00000de0: 7468 6922 2074 7970 6566 6163 653d 224e  thi" typeface="N
-00000df0: 7961 6c61 222f 3e3c 613a 666f 6e74 2073  yala"/><a:font s
-00000e00: 6372 6970 743d 2242 656e 6722 2074 7970  cript="Beng" typ
-00000e10: 6566 6163 653d 2256 7269 6e64 6122 2f3e  eface="Vrinda"/>
-00000e20: 3c61 3a66 6f6e 7420 7363 7269 7074 3d22  <a:font script="
-00000e30: 4775 6a72 2220 7479 7065 6661 6365 3d22  Gujr" typeface="
-00000e40: 5368 7275 7469 222f 3e3c 613a 666f 6e74  Shruti"/><a:font
-00000e50: 2073 6372 6970 743d 224b 686d 7222 2074   script="Khmr" t
-00000e60: 7970 6566 6163 653d 2244 6175 6e50 656e  ypeface="DaunPen
-00000e70: 6822 2f3e 3c61 3a66 6f6e 7420 7363 7269  h"/><a:font scri
-00000e80: 7074 3d22 4b6e 6461 2220 7479 7065 6661  pt="Knda" typefa
-00000e90: 6365 3d22 5475 6e67 6122 2f3e 3c61 3a66  ce="Tunga"/><a:f
-00000ea0: 6f6e 7420 7363 7269 7074 3d22 4775 7275  ont script="Guru
-00000eb0: 2220 7479 7065 6661 6365 3d22 5261 6176  " typeface="Raav
-00000ec0: 6922 2f3e 3c61 3a66 6f6e 7420 7363 7269  i"/><a:font scri
-00000ed0: 7074 3d22 4361 6e73 2220 7479 7065 6661  pt="Cans" typefa
-00000ee0: 6365 3d22 4575 7068 656d 6961 222f 3e3c  ce="Euphemia"/><
-00000ef0: 613a 666f 6e74 2073 6372 6970 743d 2243  a:font script="C
-00000f00: 6865 7222 2074 7970 6566 6163 653d 2250  her" typeface="P
-00000f10: 6c61 6e74 6167 656e 6574 2043 6865 726f  lantagenet Chero
-00000f20: 6b65 6522 2f3e 3c61 3a66 6f6e 7420 7363  kee"/><a:font sc
-00000f30: 7269 7074 3d22 5969 6969 2220 7479 7065  ript="Yiii" type
-00000f40: 6661 6365 3d22 4d69 6372 6f73 6f66 7420  face="Microsoft 
-00000f50: 5969 2042 6169 7469 222f 3e3c 613a 666f  Yi Baiti"/><a:fo
-00000f60: 6e74 2073 6372 6970 743d 2254 6962 7422  nt script="Tibt"
-00000f70: 2074 7970 6566 6163 653d 224d 6963 726f   typeface="Micro
-00000f80: 736f 6674 2048 696d 616c 6179 6122 2f3e  soft Himalaya"/>
-00000f90: 3c61 3a66 6f6e 7420 7363 7269 7074 3d22  <a:font script="
-00000fa0: 5468 6161 2220 7479 7065 6661 6365 3d22  Thaa" typeface="
-00000fb0: 4d56 2042 6f6c 6922 2f3e 3c61 3a66 6f6e  MV Boli"/><a:fon
-00000fc0: 7420 7363 7269 7074 3d22 4465 7661 2220  t script="Deva" 
-00000fd0: 7479 7065 6661 6365 3d22 4d61 6e67 616c  typeface="Mangal
-00000fe0: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
-00000ff0: 743d 2254 656c 7522 2074 7970 6566 6163  t="Telu" typefac
-00001000: 653d 2247 6175 7461 6d69 222f 3e3c 613a  e="Gautami"/><a:
-00001010: 666f 6e74 2073 6372 6970 743d 2254 616d  font script="Tam
-00001020: 6c22 2074 7970 6566 6163 653d 224c 6174  l" typeface="Lat
-00001030: 6861 222f 3e3c 613a 666f 6e74 2073 6372  ha"/><a:font scr
-00001040: 6970 743d 2253 7972 6322 2074 7970 6566  ipt="Syrc" typef
-00001050: 6163 653d 2245 7374 7261 6e67 656c 6f20  ace="Estrangelo 
-00001060: 4564 6573 7361 222f 3e3c 613a 666f 6e74  Edessa"/><a:font
-00001070: 2073 6372 6970 743d 224f 7279 6122 2074   script="Orya" t
-00001080: 7970 6566 6163 653d 224b 616c 696e 6761  ypeface="Kalinga
-00001090: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
-000010a0: 743d 224d 6c79 6d22 2074 7970 6566 6163  t="Mlym" typefac
-000010b0: 653d 224b 6172 7469 6b61 222f 3e3c 613a  e="Kartika"/><a:
-000010c0: 666f 6e74 2073 6372 6970 743d 224c 616f  font script="Lao
-000010d0: 6f22 2074 7970 6566 6163 653d 2244 6f6b  o" typeface="Dok
-000010e0: 4368 616d 7061 222f 3e3c 613a 666f 6e74  Champa"/><a:font
-000010f0: 2073 6372 6970 743d 2253 696e 6822 2074   script="Sinh" t
-00001100: 7970 6566 6163 653d 2249 736b 6f6f 6c61  ypeface="Iskoola
-00001110: 2050 6f74 6122 2f3e 3c61 3a66 6f6e 7420   Pota"/><a:font 
-00001120: 7363 7269 7074 3d22 4d6f 6e67 2220 7479  script="Mong" ty
-00001130: 7065 6661 6365 3d22 4d6f 6e67 6f6c 6961  peface="Mongolia
-00001140: 6e20 4261 6974 6922 2f3e 3c61 3a66 6f6e  n Baiti"/><a:fon
-00001150: 7420 7363 7269 7074 3d22 5669 6574 2220  t script="Viet" 
-00001160: 7479 7065 6661 6365 3d22 4172 6961 6c22  typeface="Arial"
-00001170: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
-00001180: 3d22 5569 6768 2220 7479 7065 6661 6365  ="Uigh" typeface
-00001190: 3d22 4d69 6372 6f73 6f66 7420 5569 6768  ="Microsoft Uigh
-000011a0: 7572 222f 3e3c 613a 666f 6e74 2073 6372  ur"/><a:font scr
-000011b0: 6970 743d 2247 656f 7222 2074 7970 6566  ipt="Geor" typef
-000011c0: 6163 653d 2253 796c 6661 656e 222f 3e3c  ace="Sylfaen"/><
-000011d0: 613a 666f 6e74 2073 6372 6970 743d 2241  a:font script="A
-000011e0: 726d 6e22 2074 7970 6566 6163 653d 2241  rmn" typeface="A
-000011f0: 7269 616c 222f 3e3c 613a 666f 6e74 2073  rial"/><a:font s
-00001200: 6372 6970 743d 2242 7567 6922 2074 7970  cript="Bugi" typ
-00001210: 6566 6163 653d 224c 6565 6c61 7761 6465  eface="Leelawade
-00001220: 6520 5549 222f 3e3c 613a 666f 6e74 2073  e UI"/><a:font s
-00001230: 6372 6970 743d 2242 6f70 6f22 2074 7970  cript="Bopo" typ
-00001240: 6566 6163 653d 224d 6963 726f 736f 6674  eface="Microsoft
-00001250: 204a 6865 6e67 4865 6922 2f3e 3c61 3a66   JhengHei"/><a:f
-00001260: 6f6e 7420 7363 7269 7074 3d22 4a61 7661  ont script="Java
-00001270: 2220 7479 7065 6661 6365 3d22 4a61 7661  " typeface="Java
-00001280: 6e65 7365 2054 6578 7422 2f3e 3c61 3a66  nese Text"/><a:f
-00001290: 6f6e 7420 7363 7269 7074 3d22 4c69 7375  ont script="Lisu
-000012a0: 2220 7479 7065 6661 6365 3d22 5365 676f  " typeface="Sego
-000012b0: 6520 5549 222f 3e3c 613a 666f 6e74 2073  e UI"/><a:font s
-000012c0: 6372 6970 743d 224d 796d 7222 2074 7970  cript="Mymr" typ
-000012d0: 6566 6163 653d 224d 7961 6e6d 6172 2054  eface="Myanmar T
-000012e0: 6578 7422 2f3e 3c61 3a66 6f6e 7420 7363  ext"/><a:font sc
-000012f0: 7269 7074 3d22 4e6b 6f6f 2220 7479 7065  ript="Nkoo" type
-00001300: 6661 6365 3d22 4562 7269 6d61 222f 3e3c  face="Ebrima"/><
-00001310: 613a 666f 6e74 2073 6372 6970 743d 224f  a:font script="O
-00001320: 6c63 6b22 2074 7970 6566 6163 653d 224e  lck" typeface="N
-00001330: 6972 6d61 6c61 2055 4922 2f3e 3c61 3a66  irmala UI"/><a:f
-00001340: 6f6e 7420 7363 7269 7074 3d22 4f73 6d61  ont script="Osma
-00001350: 2220 7479 7065 6661 6365 3d22 4562 7269  " typeface="Ebri
-00001360: 6d61 222f 3e3c 613a 666f 6e74 2073 6372  ma"/><a:font scr
-00001370: 6970 743d 2250 6861 6722 2074 7970 6566  ipt="Phag" typef
-00001380: 6163 653d 2250 6861 6773 7061 222f 3e3c  ace="Phagspa"/><
-00001390: 613a 666f 6e74 2073 6372 6970 743d 2253  a:font script="S
-000013a0: 7972 6e22 2074 7970 6566 6163 653d 2245  yrn" typeface="E
-000013b0: 7374 7261 6e67 656c 6f20 4564 6573 7361  strangelo Edessa
-000013c0: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
-000013d0: 743d 2253 7972 6a22 2074 7970 6566 6163  t="Syrj" typefac
-000013e0: 653d 2245 7374 7261 6e67 656c 6f20 4564  e="Estrangelo Ed
-000013f0: 6573 7361 222f 3e3c 613a 666f 6e74 2073  essa"/><a:font s
-00001400: 6372 6970 743d 2253 7972 6522 2074 7970  cript="Syre" typ
-00001410: 6566 6163 653d 2245 7374 7261 6e67 656c  eface="Estrangel
-00001420: 6f20 4564 6573 7361 222f 3e3c 613a 666f  o Edessa"/><a:fo
-00001430: 6e74 2073 6372 6970 743d 2253 6f72 6122  nt script="Sora"
-00001440: 2074 7970 6566 6163 653d 224e 6972 6d61   typeface="Nirma
-00001450: 6c61 2055 4922 2f3e 3c61 3a66 6f6e 7420  la UI"/><a:font 
-00001460: 7363 7269 7074 3d22 5461 6c65 2220 7479  script="Tale" ty
-00001470: 7065 6661 6365 3d22 4d69 6372 6f73 6f66  peface="Microsof
-00001480: 7420 5461 6920 4c65 222f 3e3c 613a 666f  t Tai Le"/><a:fo
-00001490: 6e74 2073 6372 6970 743d 2254 616c 7522  nt script="Talu"
-000014a0: 2074 7970 6566 6163 653d 224d 6963 726f   typeface="Micro
-000014b0: 736f 6674 204e 6577 2054 6169 204c 7565  soft New Tai Lue
-000014c0: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
-000014d0: 743d 2254 666e 6722 2074 7970 6566 6163  t="Tfng" typefac
-000014e0: 653d 2245 6272 696d 6122 2f3e 3c2f 613a  e="Ebrima"/></a:
-000014f0: 6d69 6e6f 7246 6f6e 743e 3c2f 613a 666f  minorFont></a:fo
-00001500: 6e74 5363 6865 6d65 3e3c 613a 666d 7453  ntScheme><a:fmtS
-00001510: 6368 656d 6520 6e61 6d65 3d22 4f66 6669  cheme name="Offi
-00001520: 6365 223e 3c61 3a66 696c 6c53 7479 6c65  ce"><a:fillStyle
-00001530: 4c73 743e 3c61 3a73 6f6c 6964 4669 6c6c  Lst><a:solidFill
-00001540: 3e3c 613a 7363 6865 6d65 436c 7220 7661  ><a:schemeClr va
-00001550: 6c3d 2270 6843 6c72 222f 3e3c 2f61 3a73  l="phClr"/></a:s
-00001560: 6f6c 6964 4669 6c6c 3e3c 613a 6772 6164  olidFill><a:grad
-00001570: 4669 6c6c 2072 6f74 5769 7468 5368 6170  Fill rotWithShap
-00001580: 653d 2231 223e 3c61 3a67 734c 7374 3e3c  e="1"><a:gsLst><
-00001590: 613a 6773 2070 6f73 3d22 3022 3e3c 613a  a:gs pos="0"><a:
-000015a0: 7363 6865 6d65 436c 7220 7661 6c3d 2270  schemeClr val="p
-000015b0: 6843 6c72 223e 3c61 3a6c 756d 4d6f 6420  hClr"><a:lumMod 
-000015c0: 7661 6c3d 2231 3130 3030 3022 2f3e 3c61  val="110000"/><a
-000015d0: 3a73 6174 4d6f 6420 7661 6c3d 2231 3035  :satMod val="105
-000015e0: 3030 3022 2f3e 3c61 3a74 696e 7420 7661  000"/><a:tint va
-000015f0: 6c3d 2236 3730 3030 222f 3e3c 2f61 3a73  l="67000"/></a:s
-00001600: 6368 656d 6543 6c72 3e3c 2f61 3a67 733e  chemeClr></a:gs>
-00001610: 3c61 3a67 7320 706f 733d 2235 3030 3030  <a:gs pos="50000
-00001620: 223e 3c61 3a73 6368 656d 6543 6c72 2076  "><a:schemeClr v
-00001630: 616c 3d22 7068 436c 7222 3e3c 613a 6c75  al="phClr"><a:lu
-00001640: 6d4d 6f64 2076 616c 3d22 3130 3530 3030  mMod val="105000
-00001650: 222f 3e3c 613a 7361 744d 6f64 2076 616c  "/><a:satMod val
-00001660: 3d22 3130 3330 3030 222f 3e3c 613a 7469  ="103000"/><a:ti
-00001670: 6e74 2076 616c 3d22 3733 3030 3022 2f3e  nt val="73000"/>
-00001680: 3c2f 613a 7363 6865 6d65 436c 723e 3c2f  </a:schemeClr></
-00001690: 613a 6773 3e3c 613a 6773 2070 6f73 3d22  a:gs><a:gs pos="
-000016a0: 3130 3030 3030 223e 3c61 3a73 6368 656d  100000"><a:schem
-000016b0: 6543 6c72 2076 616c 3d22 7068 436c 7222  eClr val="phClr"
-000016c0: 3e3c 613a 6c75 6d4d 6f64 2076 616c 3d22  ><a:lumMod val="
-000016d0: 3130 3530 3030 222f 3e3c 613a 7361 744d  105000"/><a:satM
-000016e0: 6f64 2076 616c 3d22 3130 3930 3030 222f  od val="109000"/
-000016f0: 3e3c 613a 7469 6e74 2076 616c 3d22 3831  ><a:tint val="81
-00001700: 3030 3022 2f3e 3c2f 613a 7363 6865 6d65  000"/></a:scheme
-00001710: 436c 723e 3c2f 613a 6773 3e3c 2f61 3a67  Clr></a:gs></a:g
-00001720: 734c 7374 3e3c 613a 6c69 6e20 616e 673d  sLst><a:lin ang=
-00001730: 2235 3430 3030 3030 2220 7363 616c 6564  "5400000" scaled
-00001740: 3d22 3022 2f3e 3c2f 613a 6772 6164 4669  ="0"/></a:gradFi
-00001750: 6c6c 3e3c 613a 6772 6164 4669 6c6c 2072  ll><a:gradFill r
-00001760: 6f74 5769 7468 5368 6170 653d 2231 223e  otWithShape="1">
-00001770: 3c61 3a67 734c 7374 3e3c 613a 6773 2070  <a:gsLst><a:gs p
-00001780: 6f73 3d22 3022 3e3c 613a 7363 6865 6d65  os="0"><a:scheme
-00001790: 436c 7220 7661 6c3d 2270 6843 6c72 223e  Clr val="phClr">
-000017a0: 3c61 3a73 6174 4d6f 6420 7661 6c3d 2231  <a:satMod val="1
-000017b0: 3033 3030 3022 2f3e 3c61 3a6c 756d 4d6f  03000"/><a:lumMo
-000017c0: 6420 7661 6c3d 2231 3032 3030 3022 2f3e  d val="102000"/>
-000017d0: 3c61 3a74 696e 7420 7661 6c3d 2239 3430  <a:tint val="940
-000017e0: 3030 222f 3e3c 2f61 3a73 6368 656d 6543  00"/></a:schemeC
-000017f0: 6c72 3e3c 2f61 3a67 733e 3c61 3a67 7320  lr></a:gs><a:gs 
-00001800: 706f 733d 2235 3030 3030 223e 3c61 3a73  pos="50000"><a:s
-00001810: 6368 656d 6543 6c72 2076 616c 3d22 7068  chemeClr val="ph
-00001820: 436c 7222 3e3c 613a 7361 744d 6f64 2076  Clr"><a:satMod v
-00001830: 616c 3d22 3131 3030 3030 222f 3e3c 613a  al="110000"/><a:
-00001840: 6c75 6d4d 6f64 2076 616c 3d22 3130 3030  lumMod val="1000
-00001850: 3030 222f 3e3c 613a 7368 6164 6520 7661  00"/><a:shade va
-00001860: 6c3d 2231 3030 3030 3022 2f3e 3c2f 613a  l="100000"/></a:
-00001870: 7363 6865 6d65 436c 723e 3c2f 613a 6773  schemeClr></a:gs
-00001880: 3e3c 613a 6773 2070 6f73 3d22 3130 3030  ><a:gs pos="1000
-00001890: 3030 223e 3c61 3a73 6368 656d 6543 6c72  00"><a:schemeClr
-000018a0: 2076 616c 3d22 7068 436c 7222 3e3c 613a   val="phClr"><a:
-000018b0: 6c75 6d4d 6f64 2076 616c 3d22 3939 3030  lumMod val="9900
-000018c0: 3022 2f3e 3c61 3a73 6174 4d6f 6420 7661  0"/><a:satMod va
-000018d0: 6c3d 2231 3230 3030 3022 2f3e 3c61 3a73  l="120000"/><a:s
-000018e0: 6861 6465 2076 616c 3d22 3738 3030 3022  hade val="78000"
-000018f0: 2f3e 3c2f 613a 7363 6865 6d65 436c 723e  /></a:schemeClr>
-00001900: 3c2f 613a 6773 3e3c 2f61 3a67 734c 7374  </a:gs></a:gsLst
-00001910: 3e3c 613a 6c69 6e20 616e 673d 2235 3430  ><a:lin ang="540
-00001920: 3030 3030 2220 7363 616c 6564 3d22 3022  0000" scaled="0"
-00001930: 2f3e 3c2f 613a 6772 6164 4669 6c6c 3e3c  /></a:gradFill><
-00001940: 2f61 3a66 696c 6c53 7479 6c65 4c73 743e  /a:fillStyleLst>
-00001950: 3c61 3a6c 6e53 7479 6c65 4c73 743e 3c61  <a:lnStyleLst><a
-00001960: 3a6c 6e20 773d 2236 3335 3022 2063 6170  :ln w="6350" cap
-00001970: 3d22 666c 6174 2220 636d 7064 3d22 736e  ="flat" cmpd="sn
-00001980: 6722 2061 6c67 6e3d 2263 7472 223e 3c61  g" algn="ctr"><a
-00001990: 3a73 6f6c 6964 4669 6c6c 3e3c 613a 7363  :solidFill><a:sc
-000019a0: 6865 6d65 436c 7220 7661 6c3d 2270 6843  hemeClr val="phC
-000019b0: 6c72 222f 3e3c 2f61 3a73 6f6c 6964 4669  lr"/></a:solidFi
-000019c0: 6c6c 3e3c 613a 7072 7374 4461 7368 2076  ll><a:prstDash v
-000019d0: 616c 3d22 736f 6c69 6422 2f3e 3c61 3a6d  al="solid"/><a:m
-000019e0: 6974 6572 206c 696d 3d22 3830 3030 3030  iter lim="800000
-000019f0: 222f 3e3c 2f61 3a6c 6e3e 3c61 3a6c 6e20  "/></a:ln><a:ln 
-00001a00: 773d 2231 3237 3030 2220 6361 703d 2266  w="12700" cap="f
-00001a10: 6c61 7422 2063 6d70 643d 2273 6e67 2220  lat" cmpd="sng" 
-00001a20: 616c 676e 3d22 6374 7222 3e3c 613a 736f  algn="ctr"><a:so
-00001a30: 6c69 6446 696c 6c3e 3c61 3a73 6368 656d  lidFill><a:schem
-00001a40: 6543 6c72 2076 616c 3d22 7068 436c 7222  eClr val="phClr"
-00001a50: 2f3e 3c2f 613a 736f 6c69 6446 696c 6c3e  /></a:solidFill>
-00001a60: 3c61 3a70 7273 7444 6173 6820 7661 6c3d  <a:prstDash val=
-00001a70: 2273 6f6c 6964 222f 3e3c 613a 6d69 7465  "solid"/><a:mite
-00001a80: 7220 6c69 6d3d 2238 3030 3030 3022 2f3e  r lim="800000"/>
-00001a90: 3c2f 613a 6c6e 3e3c 613a 6c6e 2077 3d22  </a:ln><a:ln w="
-00001aa0: 3139 3035 3022 2063 6170 3d22 666c 6174  19050" cap="flat
-00001ab0: 2220 636d 7064 3d22 736e 6722 2061 6c67  " cmpd="sng" alg
-00001ac0: 6e3d 2263 7472 223e 3c61 3a73 6f6c 6964  n="ctr"><a:solid
-00001ad0: 4669 6c6c 3e3c 613a 7363 6865 6d65 436c  Fill><a:schemeCl
-00001ae0: 7220 7661 6c3d 2270 6843 6c72 222f 3e3c  r val="phClr"/><
-00001af0: 2f61 3a73 6f6c 6964 4669 6c6c 3e3c 613a  /a:solidFill><a:
-00001b00: 7072 7374 4461 7368 2076 616c 3d22 736f  prstDash val="so
-00001b10: 6c69 6422 2f3e 3c61 3a6d 6974 6572 206c  lid"/><a:miter l
-00001b20: 696d 3d22 3830 3030 3030 222f 3e3c 2f61  im="800000"/></a
-00001b30: 3a6c 6e3e 3c2f 613a 6c6e 5374 796c 654c  :ln></a:lnStyleL
-00001b40: 7374 3e3c 613a 6566 6665 6374 5374 796c  st><a:effectStyl
-00001b50: 654c 7374 3e3c 613a 6566 6665 6374 5374  eLst><a:effectSt
-00001b60: 796c 653e 3c61 3a65 6666 6563 744c 7374  yle><a:effectLst
-00001b70: 2f3e 3c2f 613a 6566 6665 6374 5374 796c  /></a:effectStyl
-00001b80: 653e 3c61 3a65 6666 6563 7453 7479 6c65  e><a:effectStyle
-00001b90: 3e3c 613a 6566 6665 6374 4c73 742f 3e3c  ><a:effectLst/><
-00001ba0: 2f61 3a65 6666 6563 7453 7479 6c65 3e3c  /a:effectStyle><
-00001bb0: 613a 6566 6665 6374 5374 796c 653e 3c61  a:effectStyle><a
-00001bc0: 3a65 6666 6563 744c 7374 3e3c 613a 6f75  :effectLst><a:ou
-00001bd0: 7465 7253 6864 7720 626c 7572 5261 643d  terShdw blurRad=
-00001be0: 2235 3731 3530 2220 6469 7374 3d22 3139  "57150" dist="19
-00001bf0: 3035 3022 2064 6972 3d22 3534 3030 3030  050" dir="540000
-00001c00: 3022 2061 6c67 6e3d 2263 7472 2220 726f  0" algn="ctr" ro
-00001c10: 7457 6974 6853 6861 7065 3d22 3022 3e3c  tWithShape="0"><
-00001c20: 613a 7372 6762 436c 7220 7661 6c3d 2230  a:srgbClr val="0
-00001c30: 3030 3030 3022 3e3c 613a 616c 7068 6120  00000"><a:alpha 
-00001c40: 7661 6c3d 2236 3330 3030 222f 3e3c 2f61  val="63000"/></a
-00001c50: 3a73 7267 6243 6c72 3e3c 2f61 3a6f 7574  :srgbClr></a:out
-00001c60: 6572 5368 6477 3e3c 2f61 3a65 6666 6563  erShdw></a:effec
-00001c70: 744c 7374 3e3c 2f61 3a65 6666 6563 7453  tLst></a:effectS
-00001c80: 7479 6c65 3e3c 2f61 3a65 6666 6563 7453  tyle></a:effectS
-00001c90: 7479 6c65 4c73 743e 3c61 3a62 6746 696c  tyleLst><a:bgFil
-00001ca0: 6c53 7479 6c65 4c73 743e 3c61 3a73 6f6c  lStyleLst><a:sol
-00001cb0: 6964 4669 6c6c 3e3c 613a 7363 6865 6d65  idFill><a:scheme
-00001cc0: 436c 7220 7661 6c3d 2270 6843 6c72 222f  Clr val="phClr"/
-00001cd0: 3e3c 2f61 3a73 6f6c 6964 4669 6c6c 3e3c  ></a:solidFill><
-00001ce0: 613a 736f 6c69 6446 696c 6c3e 3c61 3a73  a:solidFill><a:s
-00001cf0: 6368 656d 6543 6c72 2076 616c 3d22 7068  chemeClr val="ph
-00001d00: 436c 7222 3e3c 613a 7469 6e74 2076 616c  Clr"><a:tint val
-00001d10: 3d22 3935 3030 3022 2f3e 3c61 3a73 6174  ="95000"/><a:sat
-00001d20: 4d6f 6420 7661 6c3d 2231 3730 3030 3022  Mod val="170000"
-00001d30: 2f3e 3c2f 613a 7363 6865 6d65 436c 723e  /></a:schemeClr>
-00001d40: 3c2f 613a 736f 6c69 6446 696c 6c3e 3c61  </a:solidFill><a
-00001d50: 3a67 7261 6446 696c 6c20 726f 7457 6974  :gradFill rotWit
-00001d60: 6853 6861 7065 3d22 3122 3e3c 613a 6773  hShape="1"><a:gs
-00001d70: 4c73 743e 3c61 3a67 7320 706f 733d 2230  Lst><a:gs pos="0
-00001d80: 223e 3c61 3a73 6368 656d 6543 6c72 2076  "><a:schemeClr v
-00001d90: 616c 3d22 7068 436c 7222 3e3c 613a 7469  al="phClr"><a:ti
-00001da0: 6e74 2076 616c 3d22 3933 3030 3022 2f3e  nt val="93000"/>
-00001db0: 3c61 3a73 6174 4d6f 6420 7661 6c3d 2231  <a:satMod val="1
-00001dc0: 3530 3030 3022 2f3e 3c61 3a73 6861 6465  50000"/><a:shade
-00001dd0: 2076 616c 3d22 3938 3030 3022 2f3e 3c61   val="98000"/><a
-00001de0: 3a6c 756d 4d6f 6420 7661 6c3d 2231 3032  :lumMod val="102
-00001df0: 3030 3022 2f3e 3c2f 613a 7363 6865 6d65  000"/></a:scheme
-00001e00: 436c 723e 3c2f 613a 6773 3e3c 613a 6773  Clr></a:gs><a:gs
-00001e10: 2070 6f73 3d22 3530 3030 3022 3e3c 613a   pos="50000"><a:
-00001e20: 7363 6865 6d65 436c 7220 7661 6c3d 2270  schemeClr val="p
-00001e30: 6843 6c72 223e 3c61 3a74 696e 7420 7661  hClr"><a:tint va
-00001e40: 6c3d 2239 3830 3030 222f 3e3c 613a 7361  l="98000"/><a:sa
-00001e50: 744d 6f64 2076 616c 3d22 3133 3030 3030  tMod val="130000
-00001e60: 222f 3e3c 613a 7368 6164 6520 7661 6c3d  "/><a:shade val=
-00001e70: 2239 3030 3030 222f 3e3c 613a 6c75 6d4d  "90000"/><a:lumM
-00001e80: 6f64 2076 616c 3d22 3130 3330 3030 222f  od val="103000"/
-00001e90: 3e3c 2f61 3a73 6368 656d 6543 6c72 3e3c  ></a:schemeClr><
-00001ea0: 2f61 3a67 733e 3c61 3a67 7320 706f 733d  /a:gs><a:gs pos=
-00001eb0: 2231 3030 3030 3022 3e3c 613a 7363 6865  "100000"><a:sche
-00001ec0: 6d65 436c 7220 7661 6c3d 2270 6843 6c72  meClr val="phClr
-00001ed0: 223e 3c61 3a73 6861 6465 2076 616c 3d22  "><a:shade val="
-00001ee0: 3633 3030 3022 2f3e 3c61 3a73 6174 4d6f  63000"/><a:satMo
-00001ef0: 6420 7661 6c3d 2231 3230 3030 3022 2f3e  d val="120000"/>
-00001f00: 3c2f 613a 7363 6865 6d65 436c 723e 3c2f  </a:schemeClr></
-00001f10: 613a 6773 3e3c 2f61 3a67 734c 7374 3e3c  a:gs></a:gsLst><
-00001f20: 613a 6c69 6e20 616e 673d 2235 3430 3030  a:lin ang="54000
-00001f30: 3030 2220 7363 616c 6564 3d22 3022 2f3e  00" scaled="0"/>
-00001f40: 3c2f 613a 6772 6164 4669 6c6c 3e3c 2f61  </a:gradFill></a
-00001f50: 3a62 6746 696c 6c53 7479 6c65 4c73 743e  :bgFillStyleLst>
-00001f60: 3c2f 613a 666d 7453 6368 656d 653e 3c2f  </a:fmtScheme></
-00001f70: 613a 7468 656d 6545 6c65 6d65 6e74 733e  a:themeElements>
-00001f80: 3c61 3a6f 626a 6563 7444 6566 6175 6c74  <a:objectDefault
-00001f90: 732f 3e3c 613a 6578 7472 6143 6c72 5363  s/><a:extraClrSc
-00001fa0: 6865 6d65 4c73 742f 3e3c 613a 6578 744c  hemeLst/><a:extL
-00001fb0: 7374 3e3c 613a 6578 7420 7572 693d 227b  st><a:ext uri="{
-00001fc0: 3035 4134 4332 3543 2d30 3835 452d 3433  05A4C25C-085E-43
-00001fd0: 3430 2d38 3541 332d 4135 3533 3145 3531  40-85A3-A5531E51
-00001fe0: 3044 4232 7d22 3e3c 7468 6d31 353a 7468  0DB2}"><thm15:th
-00001ff0: 656d 6546 616d 696c 7920 786d 6c6e 733a  emeFamily xmlns:
-00002000: 7468 6d31 353d 2268 7474 703a 2f2f 7363  thm15="http://sc
-00002010: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
-00002020: 636f 6d2f 6f66 6669 6365 2f74 6865 6d65  com/office/theme
-00002030: 6d6c 2f32 3031 322f 6d61 696e 2220 6e61  ml/2012/main" na
-00002040: 6d65 3d22 4f66 6669 6365 2054 6865 6d65  me="Office Theme
-00002050: 2220 6964 3d22 7b36 3246 3933 3942 362d  " id="{62F939B6-
-00002060: 3933 4146 2d34 4442 382d 3943 3642 2d44  93AF-4DB8-9C6B-D
-00002070: 3643 3744 4644 4335 3839 467d 2220 7669  6C7DFDC589F}" vi
-00002080: 643d 227b 3441 3343 3436 4538 2d36 3143  d="{4A3C46E8-61C
-00002090: 432d 3436 3033 2d41 3538 392d 3734 3232  C-4603-A589-7422
-000020a0: 4134 3741 3845 3441 7d22 2f3e 3c2f 613a  A47A8E4A}"/></a:
-000020b0: 6578 743e 3c2f 613a 6578 744c 7374 3e3c  ext></a:extLst><
-000020c0: 2f61 3a74 6865 6d65 3e                   /a:theme>
+00000030: 2279 6573 223f 3e0a 3c61 3a74 6865 6d65  "yes"?>.<a:theme
+00000040: 2078 6d6c 6e73 3a61 3d22 6874 7470 3a2f   xmlns:a="http:/
+00000050: 2f73 6368 656d 6173 2e6f 7065 6e78 6d6c  /schemas.openxml
+00000060: 666f 726d 6174 732e 6f72 672f 6472 6177  formats.org/draw
+00000070: 696e 676d 6c2f 3230 3036 2f6d 6169 6e22  ingml/2006/main"
+00000080: 206e 616d 653d 224f 6666 6963 6520 5468   name="Office Th
+00000090: 656d 6522 3e3c 613a 7468 656d 6545 6c65  eme"><a:themeEle
+000000a0: 6d65 6e74 733e 3c61 3a63 6c72 5363 6865  ments><a:clrSche
+000000b0: 6d65 206e 616d 653d 224f 6666 6963 6522  me name="Office"
+000000c0: 3e3c 613a 646b 313e 3c61 3a73 7973 436c  ><a:dk1><a:sysCl
+000000d0: 7220 7661 6c3d 2277 696e 646f 7754 6578  r val="windowTex
+000000e0: 7422 206c 6173 7443 6c72 3d22 3030 3030  t" lastClr="0000
+000000f0: 3030 222f 3e3c 2f61 3a64 6b31 3e3c 613a  00"/></a:dk1><a:
+00000100: 6c74 313e 3c61 3a73 7973 436c 7220 7661  lt1><a:sysClr va
+00000110: 6c3d 2277 696e 646f 7722 206c 6173 7443  l="window" lastC
+00000120: 6c72 3d22 4646 4646 4646 222f 3e3c 2f61  lr="FFFFFF"/></a
+00000130: 3a6c 7431 3e3c 613a 646b 323e 3c61 3a73  :lt1><a:dk2><a:s
+00000140: 7267 6243 6c72 2076 616c 3d22 3434 3534  rgbClr val="4454
+00000150: 3641 222f 3e3c 2f61 3a64 6b32 3e3c 613a  6A"/></a:dk2><a:
+00000160: 6c74 323e 3c61 3a73 7267 6243 6c72 2076  lt2><a:srgbClr v
+00000170: 616c 3d22 4537 4536 4536 222f 3e3c 2f61  al="E7E6E6"/></a
+00000180: 3a6c 7432 3e3c 613a 6163 6365 6e74 313e  :lt2><a:accent1>
+00000190: 3c61 3a73 7267 6243 6c72 2076 616c 3d22  <a:srgbClr val="
+000001a0: 3434 3732 4334 222f 3e3c 2f61 3a61 6363  4472C4"/></a:acc
+000001b0: 656e 7431 3e3c 613a 6163 6365 6e74 323e  ent1><a:accent2>
+000001c0: 3c61 3a73 7267 6243 6c72 2076 616c 3d22  <a:srgbClr val="
+000001d0: 4544 3744 3331 222f 3e3c 2f61 3a61 6363  ED7D31"/></a:acc
+000001e0: 656e 7432 3e3c 613a 6163 6365 6e74 333e  ent2><a:accent3>
+000001f0: 3c61 3a73 7267 6243 6c72 2076 616c 3d22  <a:srgbClr val="
+00000200: 4135 4135 4135 222f 3e3c 2f61 3a61 6363  A5A5A5"/></a:acc
+00000210: 656e 7433 3e3c 613a 6163 6365 6e74 343e  ent3><a:accent4>
+00000220: 3c61 3a73 7267 6243 6c72 2076 616c 3d22  <a:srgbClr val="
+00000230: 4646 4330 3030 222f 3e3c 2f61 3a61 6363  FFC000"/></a:acc
+00000240: 656e 7434 3e3c 613a 6163 6365 6e74 353e  ent4><a:accent5>
+00000250: 3c61 3a73 7267 6243 6c72 2076 616c 3d22  <a:srgbClr val="
+00000260: 3542 3942 4435 222f 3e3c 2f61 3a61 6363  5B9BD5"/></a:acc
+00000270: 656e 7435 3e3c 613a 6163 6365 6e74 363e  ent5><a:accent6>
+00000280: 3c61 3a73 7267 6243 6c72 2076 616c 3d22  <a:srgbClr val="
+00000290: 3730 4144 3437 222f 3e3c 2f61 3a61 6363  70AD47"/></a:acc
+000002a0: 656e 7436 3e3c 613a 686c 696e 6b3e 3c61  ent6><a:hlink><a
+000002b0: 3a73 7267 6243 6c72 2076 616c 3d22 3035  :srgbClr val="05
+000002c0: 3633 4331 222f 3e3c 2f61 3a68 6c69 6e6b  63C1"/></a:hlink
+000002d0: 3e3c 613a 666f 6c48 6c69 6e6b 3e3c 613a  ><a:folHlink><a:
+000002e0: 7372 6762 436c 7220 7661 6c3d 2239 3534  srgbClr val="954
+000002f0: 4637 3222 2f3e 3c2f 613a 666f 6c48 6c69  F72"/></a:folHli
+00000300: 6e6b 3e3c 2f61 3a63 6c72 5363 6865 6d65  nk></a:clrScheme
+00000310: 3e3c 613a 666f 6e74 5363 6865 6d65 206e  ><a:fontScheme n
+00000320: 616d 653d 224f 6666 6963 6522 3e3c 613a  ame="Office"><a:
+00000330: 6d61 6a6f 7246 6f6e 743e 3c61 3a6c 6174  majorFont><a:lat
+00000340: 696e 2074 7970 6566 6163 653d 2243 616c  in typeface="Cal
+00000350: 6962 7269 204c 6967 6874 2220 7061 6e6f  ibri Light" pano
+00000360: 7365 3d22 3032 3046 3033 3032 3032 3032  se="020F03020202
+00000370: 3034 3033 3032 3034 222f 3e3c 613a 6561  04030204"/><a:ea
+00000380: 2074 7970 6566 6163 653d 2222 2f3e 3c61   typeface=""/><a
+00000390: 3a63 7320 7479 7065 6661 6365 3d22 222f  :cs typeface=""/
+000003a0: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+000003b0: 224a 7061 6e22 2074 7970 6566 6163 653d  "Jpan" typeface=
+000003c0: 22e6 b8b8 e382 b4e3 82b7 e383 83e3 82af  "...............
+000003d0: 204c 6967 6874 222f 3e3c 613a 666f 6e74   Light"/><a:font
+000003e0: 2073 6372 6970 743d 2248 616e 6722 2074   script="Hang" t
+000003f0: 7970 6566 6163 653d 22eb a791 ec9d 8020  ypeface="...... 
+00000400: eab3 a0eb 9495 222f 3e3c 613a 666f 6e74  ......"/><a:font
+00000410: 2073 6372 6970 743d 2248 616e 7322 2074   script="Hans" t
+00000420: 7970 6566 6163 653d 22e7 ad89 e7ba bf20  ypeface="...... 
+00000430: 4c69 6768 7422 2f3e 3c61 3a66 6f6e 7420  Light"/><a:font 
+00000440: 7363 7269 7074 3d22 4861 6e74 2220 7479  script="Hant" ty
+00000450: 7065 6661 6365 3d22 e696 b0e7 b4b0 e698  peface="........
+00000460: 8ee9 ab94 222f 3e3c 613a 666f 6e74 2073  ...."/><a:font s
+00000470: 6372 6970 743d 2241 7261 6222 2074 7970  cript="Arab" typ
+00000480: 6566 6163 653d 2254 696d 6573 204e 6577  eface="Times New
+00000490: 2052 6f6d 616e 222f 3e3c 613a 666f 6e74   Roman"/><a:font
+000004a0: 2073 6372 6970 743d 2248 6562 7222 2074   script="Hebr" t
+000004b0: 7970 6566 6163 653d 2254 696d 6573 204e  ypeface="Times N
+000004c0: 6577 2052 6f6d 616e 222f 3e3c 613a 666f  ew Roman"/><a:fo
+000004d0: 6e74 2073 6372 6970 743d 2254 6861 6922  nt script="Thai"
+000004e0: 2074 7970 6566 6163 653d 2241 6e67 7361   typeface="Angsa
+000004f0: 6e61 204e 6577 222f 3e3c 613a 666f 6e74  na New"/><a:font
+00000500: 2073 6372 6970 743d 2245 7468 6922 2074   script="Ethi" t
+00000510: 7970 6566 6163 653d 224e 7961 6c61 222f  ypeface="Nyala"/
+00000520: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+00000530: 2242 656e 6722 2074 7970 6566 6163 653d  "Beng" typeface=
+00000540: 2256 7269 6e64 6122 2f3e 3c61 3a66 6f6e  "Vrinda"/><a:fon
+00000550: 7420 7363 7269 7074 3d22 4775 6a72 2220  t script="Gujr" 
+00000560: 7479 7065 6661 6365 3d22 5368 7275 7469  typeface="Shruti
+00000570: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
+00000580: 743d 224b 686d 7222 2074 7970 6566 6163  t="Khmr" typefac
+00000590: 653d 224d 6f6f 6c42 6f72 616e 222f 3e3c  e="MoolBoran"/><
+000005a0: 613a 666f 6e74 2073 6372 6970 743d 224b  a:font script="K
+000005b0: 6e64 6122 2074 7970 6566 6163 653d 2254  nda" typeface="T
+000005c0: 756e 6761 222f 3e3c 613a 666f 6e74 2073  unga"/><a:font s
+000005d0: 6372 6970 743d 2247 7572 7522 2074 7970  cript="Guru" typ
+000005e0: 6566 6163 653d 2252 6161 7669 222f 3e3c  eface="Raavi"/><
+000005f0: 613a 666f 6e74 2073 6372 6970 743d 2243  a:font script="C
+00000600: 616e 7322 2074 7970 6566 6163 653d 2245  ans" typeface="E
+00000610: 7570 6865 6d69 6122 2f3e 3c61 3a66 6f6e  uphemia"/><a:fon
+00000620: 7420 7363 7269 7074 3d22 4368 6572 2220  t script="Cher" 
+00000630: 7479 7065 6661 6365 3d22 506c 616e 7461  typeface="Planta
+00000640: 6765 6e65 7420 4368 6572 6f6b 6565 222f  genet Cherokee"/
+00000650: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+00000660: 2259 6969 6922 2074 7970 6566 6163 653d  "Yiii" typeface=
+00000670: 224d 6963 726f 736f 6674 2059 6920 4261  "Microsoft Yi Ba
+00000680: 6974 6922 2f3e 3c61 3a66 6f6e 7420 7363  iti"/><a:font sc
+00000690: 7269 7074 3d22 5469 6274 2220 7479 7065  ript="Tibt" type
+000006a0: 6661 6365 3d22 4d69 6372 6f73 6f66 7420  face="Microsoft 
+000006b0: 4869 6d61 6c61 7961 222f 3e3c 613a 666f  Himalaya"/><a:fo
+000006c0: 6e74 2073 6372 6970 743d 2254 6861 6122  nt script="Thaa"
+000006d0: 2074 7970 6566 6163 653d 224d 5620 426f   typeface="MV Bo
+000006e0: 6c69 222f 3e3c 613a 666f 6e74 2073 6372  li"/><a:font scr
+000006f0: 6970 743d 2244 6576 6122 2074 7970 6566  ipt="Deva" typef
+00000700: 6163 653d 224d 616e 6761 6c22 2f3e 3c61  ace="Mangal"/><a
+00000710: 3a66 6f6e 7420 7363 7269 7074 3d22 5465  :font script="Te
+00000720: 6c75 2220 7479 7065 6661 6365 3d22 4761  lu" typeface="Ga
+00000730: 7574 616d 6922 2f3e 3c61 3a66 6f6e 7420  utami"/><a:font 
+00000740: 7363 7269 7074 3d22 5461 6d6c 2220 7479  script="Taml" ty
+00000750: 7065 6661 6365 3d22 4c61 7468 6122 2f3e  peface="Latha"/>
+00000760: 3c61 3a66 6f6e 7420 7363 7269 7074 3d22  <a:font script="
+00000770: 5379 7263 2220 7479 7065 6661 6365 3d22  Syrc" typeface="
+00000780: 4573 7472 616e 6765 6c6f 2045 6465 7373  Estrangelo Edess
+00000790: 6122 2f3e 3c61 3a66 6f6e 7420 7363 7269  a"/><a:font scri
+000007a0: 7074 3d22 4f72 7961 2220 7479 7065 6661  pt="Orya" typefa
+000007b0: 6365 3d22 4b61 6c69 6e67 6122 2f3e 3c61  ce="Kalinga"/><a
+000007c0: 3a66 6f6e 7420 7363 7269 7074 3d22 4d6c  :font script="Ml
+000007d0: 796d 2220 7479 7065 6661 6365 3d22 4b61  ym" typeface="Ka
+000007e0: 7274 696b 6122 2f3e 3c61 3a66 6f6e 7420  rtika"/><a:font 
+000007f0: 7363 7269 7074 3d22 4c61 6f6f 2220 7479  script="Laoo" ty
+00000800: 7065 6661 6365 3d22 446f 6b43 6861 6d70  peface="DokChamp
+00000810: 6122 2f3e 3c61 3a66 6f6e 7420 7363 7269  a"/><a:font scri
+00000820: 7074 3d22 5369 6e68 2220 7479 7065 6661  pt="Sinh" typefa
+00000830: 6365 3d22 4973 6b6f 6f6c 6120 506f 7461  ce="Iskoola Pota
+00000840: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
+00000850: 743d 224d 6f6e 6722 2074 7970 6566 6163  t="Mong" typefac
+00000860: 653d 224d 6f6e 676f 6c69 616e 2042 6169  e="Mongolian Bai
+00000870: 7469 222f 3e3c 613a 666f 6e74 2073 6372  ti"/><a:font scr
+00000880: 6970 743d 2256 6965 7422 2074 7970 6566  ipt="Viet" typef
+00000890: 6163 653d 2254 696d 6573 204e 6577 2052  ace="Times New R
+000008a0: 6f6d 616e 222f 3e3c 613a 666f 6e74 2073  oman"/><a:font s
+000008b0: 6372 6970 743d 2255 6967 6822 2074 7970  cript="Uigh" typ
+000008c0: 6566 6163 653d 224d 6963 726f 736f 6674  eface="Microsoft
+000008d0: 2055 6967 6875 7222 2f3e 3c61 3a66 6f6e   Uighur"/><a:fon
+000008e0: 7420 7363 7269 7074 3d22 4765 6f72 2220  t script="Geor" 
+000008f0: 7479 7065 6661 6365 3d22 5379 6c66 6165  typeface="Sylfae
+00000900: 6e22 2f3e 3c61 3a66 6f6e 7420 7363 7269  n"/><a:font scri
+00000910: 7074 3d22 4172 6d6e 2220 7479 7065 6661  pt="Armn" typefa
+00000920: 6365 3d22 4172 6961 6c22 2f3e 3c61 3a66  ce="Arial"/><a:f
+00000930: 6f6e 7420 7363 7269 7074 3d22 4275 6769  ont script="Bugi
+00000940: 2220 7479 7065 6661 6365 3d22 4c65 656c  " typeface="Leel
+00000950: 6177 6164 6565 2055 4922 2f3e 3c61 3a66  awadee UI"/><a:f
+00000960: 6f6e 7420 7363 7269 7074 3d22 426f 706f  ont script="Bopo
+00000970: 2220 7479 7065 6661 6365 3d22 4d69 6372  " typeface="Micr
+00000980: 6f73 6f66 7420 4a68 656e 6748 6569 222f  osoft JhengHei"/
+00000990: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+000009a0: 224a 6176 6122 2074 7970 6566 6163 653d  "Java" typeface=
+000009b0: 224a 6176 616e 6573 6520 5465 7874 222f  "Javanese Text"/
+000009c0: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+000009d0: 224c 6973 7522 2074 7970 6566 6163 653d  "Lisu" typeface=
+000009e0: 2253 6567 6f65 2055 4922 2f3e 3c61 3a66  "Segoe UI"/><a:f
+000009f0: 6f6e 7420 7363 7269 7074 3d22 4d79 6d72  ont script="Mymr
+00000a00: 2220 7479 7065 6661 6365 3d22 4d79 616e  " typeface="Myan
+00000a10: 6d61 7220 5465 7874 222f 3e3c 613a 666f  mar Text"/><a:fo
+00000a20: 6e74 2073 6372 6970 743d 224e 6b6f 6f22  nt script="Nkoo"
+00000a30: 2074 7970 6566 6163 653d 2245 6272 696d   typeface="Ebrim
+00000a40: 6122 2f3e 3c61 3a66 6f6e 7420 7363 7269  a"/><a:font scri
+00000a50: 7074 3d22 4f6c 636b 2220 7479 7065 6661  pt="Olck" typefa
+00000a60: 6365 3d22 4e69 726d 616c 6120 5549 222f  ce="Nirmala UI"/
+00000a70: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+00000a80: 224f 736d 6122 2074 7970 6566 6163 653d  "Osma" typeface=
+00000a90: 2245 6272 696d 6122 2f3e 3c61 3a66 6f6e  "Ebrima"/><a:fon
+00000aa0: 7420 7363 7269 7074 3d22 5068 6167 2220  t script="Phag" 
+00000ab0: 7479 7065 6661 6365 3d22 5068 6167 7370  typeface="Phagsp
+00000ac0: 6122 2f3e 3c61 3a66 6f6e 7420 7363 7269  a"/><a:font scri
+00000ad0: 7074 3d22 5379 726e 2220 7479 7065 6661  pt="Syrn" typefa
+00000ae0: 6365 3d22 4573 7472 616e 6765 6c6f 2045  ce="Estrangelo E
+00000af0: 6465 7373 6122 2f3e 3c61 3a66 6f6e 7420  dessa"/><a:font 
+00000b00: 7363 7269 7074 3d22 5379 726a 2220 7479  script="Syrj" ty
+00000b10: 7065 6661 6365 3d22 4573 7472 616e 6765  peface="Estrange
+00000b20: 6c6f 2045 6465 7373 6122 2f3e 3c61 3a66  lo Edessa"/><a:f
+00000b30: 6f6e 7420 7363 7269 7074 3d22 5379 7265  ont script="Syre
+00000b40: 2220 7479 7065 6661 6365 3d22 4573 7472  " typeface="Estr
+00000b50: 616e 6765 6c6f 2045 6465 7373 6122 2f3e  angelo Edessa"/>
+00000b60: 3c61 3a66 6f6e 7420 7363 7269 7074 3d22  <a:font script="
+00000b70: 536f 7261 2220 7479 7065 6661 6365 3d22  Sora" typeface="
+00000b80: 4e69 726d 616c 6120 5549 222f 3e3c 613a  Nirmala UI"/><a:
+00000b90: 666f 6e74 2073 6372 6970 743d 2254 616c  font script="Tal
+00000ba0: 6522 2074 7970 6566 6163 653d 224d 6963  e" typeface="Mic
+00000bb0: 726f 736f 6674 2054 6169 204c 6522 2f3e  rosoft Tai Le"/>
+00000bc0: 3c61 3a66 6f6e 7420 7363 7269 7074 3d22  <a:font script="
+00000bd0: 5461 6c75 2220 7479 7065 6661 6365 3d22  Talu" typeface="
+00000be0: 4d69 6372 6f73 6f66 7420 4e65 7720 5461  Microsoft New Ta
+00000bf0: 6920 4c75 6522 2f3e 3c61 3a66 6f6e 7420  i Lue"/><a:font 
+00000c00: 7363 7269 7074 3d22 5466 6e67 2220 7479  script="Tfng" ty
+00000c10: 7065 6661 6365 3d22 4562 7269 6d61 222f  peface="Ebrima"/
+00000c20: 3e3c 2f61 3a6d 616a 6f72 466f 6e74 3e3c  ></a:majorFont><
+00000c30: 613a 6d69 6e6f 7246 6f6e 743e 3c61 3a6c  a:minorFont><a:l
+00000c40: 6174 696e 2074 7970 6566 6163 653d 2243  atin typeface="C
+00000c50: 616c 6962 7269 2220 7061 6e6f 7365 3d22  alibri" panose="
+00000c60: 3032 3046 3035 3032 3032 3032 3034 3033  020F050202020403
+00000c70: 3032 3034 222f 3e3c 613a 6561 2074 7970  0204"/><a:ea typ
+00000c80: 6566 6163 653d 2222 2f3e 3c61 3a63 7320  eface=""/><a:cs 
+00000c90: 7479 7065 6661 6365 3d22 222f 3e3c 613a  typeface=""/><a:
+00000ca0: 666f 6e74 2073 6372 6970 743d 224a 7061  font script="Jpa
+00000cb0: 6e22 2074 7970 6566 6163 653d 22e6 b8b8  n" typeface="...
+00000cc0: e698 8ee6 9c9d 222f 3e3c 613a 666f 6e74  ......"/><a:font
+00000cd0: 2073 6372 6970 743d 2248 616e 6722 2074   script="Hang" t
+00000ce0: 7970 6566 6163 653d 22eb a791 ec9d 8020  ypeface="...... 
+00000cf0: eab3 a0eb 9495 222f 3e3c 613a 666f 6e74  ......"/><a:font
+00000d00: 2073 6372 6970 743d 2248 616e 7322 2074   script="Hans" t
+00000d10: 7970 6566 6163 653d 22e7 ad89 e7ba bf22  ypeface="......"
+00000d20: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
+00000d30: 3d22 4861 6e74 2220 7479 7065 6661 6365  ="Hant" typeface
+00000d40: 3d22 e696 b0e7 b4b0 e698 8ee9 ab94 222f  ="............"/
+00000d50: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+00000d60: 2241 7261 6222 2074 7970 6566 6163 653d  "Arab" typeface=
+00000d70: 2241 7269 616c 222f 3e3c 613a 666f 6e74  "Arial"/><a:font
+00000d80: 2073 6372 6970 743d 2248 6562 7222 2074   script="Hebr" t
+00000d90: 7970 6566 6163 653d 2241 7269 616c 222f  ypeface="Arial"/
+00000da0: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+00000db0: 2254 6861 6922 2074 7970 6566 6163 653d  "Thai" typeface=
+00000dc0: 2243 6f72 6469 6120 4e65 7722 2f3e 3c61  "Cordia New"/><a
+00000dd0: 3a66 6f6e 7420 7363 7269 7074 3d22 4574  :font script="Et
+00000de0: 6869 2220 7479 7065 6661 6365 3d22 4e79  hi" typeface="Ny
+00000df0: 616c 6122 2f3e 3c61 3a66 6f6e 7420 7363  ala"/><a:font sc
+00000e00: 7269 7074 3d22 4265 6e67 2220 7479 7065  ript="Beng" type
+00000e10: 6661 6365 3d22 5672 696e 6461 222f 3e3c  face="Vrinda"/><
+00000e20: 613a 666f 6e74 2073 6372 6970 743d 2247  a:font script="G
+00000e30: 756a 7222 2074 7970 6566 6163 653d 2253  ujr" typeface="S
+00000e40: 6872 7574 6922 2f3e 3c61 3a66 6f6e 7420  hruti"/><a:font 
+00000e50: 7363 7269 7074 3d22 4b68 6d72 2220 7479  script="Khmr" ty
+00000e60: 7065 6661 6365 3d22 4461 756e 5065 6e68  peface="DaunPenh
+00000e70: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
+00000e80: 743d 224b 6e64 6122 2074 7970 6566 6163  t="Knda" typefac
+00000e90: 653d 2254 756e 6761 222f 3e3c 613a 666f  e="Tunga"/><a:fo
+00000ea0: 6e74 2073 6372 6970 743d 2247 7572 7522  nt script="Guru"
+00000eb0: 2074 7970 6566 6163 653d 2252 6161 7669   typeface="Raavi
+00000ec0: 222f 3e3c 613a 666f 6e74 2073 6372 6970  "/><a:font scrip
+00000ed0: 743d 2243 616e 7322 2074 7970 6566 6163  t="Cans" typefac
+00000ee0: 653d 2245 7570 6865 6d69 6122 2f3e 3c61  e="Euphemia"/><a
+00000ef0: 3a66 6f6e 7420 7363 7269 7074 3d22 4368  :font script="Ch
+00000f00: 6572 2220 7479 7065 6661 6365 3d22 506c  er" typeface="Pl
+00000f10: 616e 7461 6765 6e65 7420 4368 6572 6f6b  antagenet Cherok
+00000f20: 6565 222f 3e3c 613a 666f 6e74 2073 6372  ee"/><a:font scr
+00000f30: 6970 743d 2259 6969 6922 2074 7970 6566  ipt="Yiii" typef
+00000f40: 6163 653d 224d 6963 726f 736f 6674 2059  ace="Microsoft Y
+00000f50: 6920 4261 6974 6922 2f3e 3c61 3a66 6f6e  i Baiti"/><a:fon
+00000f60: 7420 7363 7269 7074 3d22 5469 6274 2220  t script="Tibt" 
+00000f70: 7479 7065 6661 6365 3d22 4d69 6372 6f73  typeface="Micros
+00000f80: 6f66 7420 4869 6d61 6c61 7961 222f 3e3c  oft Himalaya"/><
+00000f90: 613a 666f 6e74 2073 6372 6970 743d 2254  a:font script="T
+00000fa0: 6861 6122 2074 7970 6566 6163 653d 224d  haa" typeface="M
+00000fb0: 5620 426f 6c69 222f 3e3c 613a 666f 6e74  V Boli"/><a:font
+00000fc0: 2073 6372 6970 743d 2244 6576 6122 2074   script="Deva" t
+00000fd0: 7970 6566 6163 653d 224d 616e 6761 6c22  ypeface="Mangal"
+00000fe0: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
+00000ff0: 3d22 5465 6c75 2220 7479 7065 6661 6365  ="Telu" typeface
+00001000: 3d22 4761 7574 616d 6922 2f3e 3c61 3a66  ="Gautami"/><a:f
+00001010: 6f6e 7420 7363 7269 7074 3d22 5461 6d6c  ont script="Taml
+00001020: 2220 7479 7065 6661 6365 3d22 4c61 7468  " typeface="Lath
+00001030: 6122 2f3e 3c61 3a66 6f6e 7420 7363 7269  a"/><a:font scri
+00001040: 7074 3d22 5379 7263 2220 7479 7065 6661  pt="Syrc" typefa
+00001050: 6365 3d22 4573 7472 616e 6765 6c6f 2045  ce="Estrangelo E
+00001060: 6465 7373 6122 2f3e 3c61 3a66 6f6e 7420  dessa"/><a:font 
+00001070: 7363 7269 7074 3d22 4f72 7961 2220 7479  script="Orya" ty
+00001080: 7065 6661 6365 3d22 4b61 6c69 6e67 6122  peface="Kalinga"
+00001090: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
+000010a0: 3d22 4d6c 796d 2220 7479 7065 6661 6365  ="Mlym" typeface
+000010b0: 3d22 4b61 7274 696b 6122 2f3e 3c61 3a66  ="Kartika"/><a:f
+000010c0: 6f6e 7420 7363 7269 7074 3d22 4c61 6f6f  ont script="Laoo
+000010d0: 2220 7479 7065 6661 6365 3d22 446f 6b43  " typeface="DokC
+000010e0: 6861 6d70 6122 2f3e 3c61 3a66 6f6e 7420  hampa"/><a:font 
+000010f0: 7363 7269 7074 3d22 5369 6e68 2220 7479  script="Sinh" ty
+00001100: 7065 6661 6365 3d22 4973 6b6f 6f6c 6120  peface="Iskoola 
+00001110: 506f 7461 222f 3e3c 613a 666f 6e74 2073  Pota"/><a:font s
+00001120: 6372 6970 743d 224d 6f6e 6722 2074 7970  cript="Mong" typ
+00001130: 6566 6163 653d 224d 6f6e 676f 6c69 616e  eface="Mongolian
+00001140: 2042 6169 7469 222f 3e3c 613a 666f 6e74   Baiti"/><a:font
+00001150: 2073 6372 6970 743d 2256 6965 7422 2074   script="Viet" t
+00001160: 7970 6566 6163 653d 2241 7269 616c 222f  ypeface="Arial"/
+00001170: 3e3c 613a 666f 6e74 2073 6372 6970 743d  ><a:font script=
+00001180: 2255 6967 6822 2074 7970 6566 6163 653d  "Uigh" typeface=
+00001190: 224d 6963 726f 736f 6674 2055 6967 6875  "Microsoft Uighu
+000011a0: 7222 2f3e 3c61 3a66 6f6e 7420 7363 7269  r"/><a:font scri
+000011b0: 7074 3d22 4765 6f72 2220 7479 7065 6661  pt="Geor" typefa
+000011c0: 6365 3d22 5379 6c66 6165 6e22 2f3e 3c61  ce="Sylfaen"/><a
+000011d0: 3a66 6f6e 7420 7363 7269 7074 3d22 4172  :font script="Ar
+000011e0: 6d6e 2220 7479 7065 6661 6365 3d22 4172  mn" typeface="Ar
+000011f0: 6961 6c22 2f3e 3c61 3a66 6f6e 7420 7363  ial"/><a:font sc
+00001200: 7269 7074 3d22 4275 6769 2220 7479 7065  ript="Bugi" type
+00001210: 6661 6365 3d22 4c65 656c 6177 6164 6565  face="Leelawadee
+00001220: 2055 4922 2f3e 3c61 3a66 6f6e 7420 7363   UI"/><a:font sc
+00001230: 7269 7074 3d22 426f 706f 2220 7479 7065  ript="Bopo" type
+00001240: 6661 6365 3d22 4d69 6372 6f73 6f66 7420  face="Microsoft 
+00001250: 4a68 656e 6748 6569 222f 3e3c 613a 666f  JhengHei"/><a:fo
+00001260: 6e74 2073 6372 6970 743d 224a 6176 6122  nt script="Java"
+00001270: 2074 7970 6566 6163 653d 224a 6176 616e   typeface="Javan
+00001280: 6573 6520 5465 7874 222f 3e3c 613a 666f  ese Text"/><a:fo
+00001290: 6e74 2073 6372 6970 743d 224c 6973 7522  nt script="Lisu"
+000012a0: 2074 7970 6566 6163 653d 2253 6567 6f65   typeface="Segoe
+000012b0: 2055 4922 2f3e 3c61 3a66 6f6e 7420 7363   UI"/><a:font sc
+000012c0: 7269 7074 3d22 4d79 6d72 2220 7479 7065  ript="Mymr" type
+000012d0: 6661 6365 3d22 4d79 616e 6d61 7220 5465  face="Myanmar Te
+000012e0: 7874 222f 3e3c 613a 666f 6e74 2073 6372  xt"/><a:font scr
+000012f0: 6970 743d 224e 6b6f 6f22 2074 7970 6566  ipt="Nkoo" typef
+00001300: 6163 653d 2245 6272 696d 6122 2f3e 3c61  ace="Ebrima"/><a
+00001310: 3a66 6f6e 7420 7363 7269 7074 3d22 4f6c  :font script="Ol
+00001320: 636b 2220 7479 7065 6661 6365 3d22 4e69  ck" typeface="Ni
+00001330: 726d 616c 6120 5549 222f 3e3c 613a 666f  rmala UI"/><a:fo
+00001340: 6e74 2073 6372 6970 743d 224f 736d 6122  nt script="Osma"
+00001350: 2074 7970 6566 6163 653d 2245 6272 696d   typeface="Ebrim
+00001360: 6122 2f3e 3c61 3a66 6f6e 7420 7363 7269  a"/><a:font scri
+00001370: 7074 3d22 5068 6167 2220 7479 7065 6661  pt="Phag" typefa
+00001380: 6365 3d22 5068 6167 7370 6122 2f3e 3c61  ce="Phagspa"/><a
+00001390: 3a66 6f6e 7420 7363 7269 7074 3d22 5379  :font script="Sy
+000013a0: 726e 2220 7479 7065 6661 6365 3d22 4573  rn" typeface="Es
+000013b0: 7472 616e 6765 6c6f 2045 6465 7373 6122  trangelo Edessa"
+000013c0: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
+000013d0: 3d22 5379 726a 2220 7479 7065 6661 6365  ="Syrj" typeface
+000013e0: 3d22 4573 7472 616e 6765 6c6f 2045 6465  ="Estrangelo Ede
+000013f0: 7373 6122 2f3e 3c61 3a66 6f6e 7420 7363  ssa"/><a:font sc
+00001400: 7269 7074 3d22 5379 7265 2220 7479 7065  ript="Syre" type
+00001410: 6661 6365 3d22 4573 7472 616e 6765 6c6f  face="Estrangelo
+00001420: 2045 6465 7373 6122 2f3e 3c61 3a66 6f6e   Edessa"/><a:fon
+00001430: 7420 7363 7269 7074 3d22 536f 7261 2220  t script="Sora" 
+00001440: 7479 7065 6661 6365 3d22 4e69 726d 616c  typeface="Nirmal
+00001450: 6120 5549 222f 3e3c 613a 666f 6e74 2073  a UI"/><a:font s
+00001460: 6372 6970 743d 2254 616c 6522 2074 7970  cript="Tale" typ
+00001470: 6566 6163 653d 224d 6963 726f 736f 6674  eface="Microsoft
+00001480: 2054 6169 204c 6522 2f3e 3c61 3a66 6f6e   Tai Le"/><a:fon
+00001490: 7420 7363 7269 7074 3d22 5461 6c75 2220  t script="Talu" 
+000014a0: 7479 7065 6661 6365 3d22 4d69 6372 6f73  typeface="Micros
+000014b0: 6f66 7420 4e65 7720 5461 6920 4c75 6522  oft New Tai Lue"
+000014c0: 2f3e 3c61 3a66 6f6e 7420 7363 7269 7074  /><a:font script
+000014d0: 3d22 5466 6e67 2220 7479 7065 6661 6365  ="Tfng" typeface
+000014e0: 3d22 4562 7269 6d61 222f 3e3c 2f61 3a6d  ="Ebrima"/></a:m
+000014f0: 696e 6f72 466f 6e74 3e3c 2f61 3a66 6f6e  inorFont></a:fon
+00001500: 7453 6368 656d 653e 3c61 3a66 6d74 5363  tScheme><a:fmtSc
+00001510: 6865 6d65 206e 616d 653d 224f 6666 6963  heme name="Offic
+00001520: 6522 3e3c 613a 6669 6c6c 5374 796c 654c  e"><a:fillStyleL
+00001530: 7374 3e3c 613a 736f 6c69 6446 696c 6c3e  st><a:solidFill>
+00001540: 3c61 3a73 6368 656d 6543 6c72 2076 616c  <a:schemeClr val
+00001550: 3d22 7068 436c 7222 2f3e 3c2f 613a 736f  ="phClr"/></a:so
+00001560: 6c69 6446 696c 6c3e 3c61 3a67 7261 6446  lidFill><a:gradF
+00001570: 696c 6c20 726f 7457 6974 6853 6861 7065  ill rotWithShape
+00001580: 3d22 3122 3e3c 613a 6773 4c73 743e 3c61  ="1"><a:gsLst><a
+00001590: 3a67 7320 706f 733d 2230 223e 3c61 3a73  :gs pos="0"><a:s
+000015a0: 6368 656d 6543 6c72 2076 616c 3d22 7068  chemeClr val="ph
+000015b0: 436c 7222 3e3c 613a 6c75 6d4d 6f64 2076  Clr"><a:lumMod v
+000015c0: 616c 3d22 3131 3030 3030 222f 3e3c 613a  al="110000"/><a:
+000015d0: 7361 744d 6f64 2076 616c 3d22 3130 3530  satMod val="1050
+000015e0: 3030 222f 3e3c 613a 7469 6e74 2076 616c  00"/><a:tint val
+000015f0: 3d22 3637 3030 3022 2f3e 3c2f 613a 7363  ="67000"/></a:sc
+00001600: 6865 6d65 436c 723e 3c2f 613a 6773 3e3c  hemeClr></a:gs><
+00001610: 613a 6773 2070 6f73 3d22 3530 3030 3022  a:gs pos="50000"
+00001620: 3e3c 613a 7363 6865 6d65 436c 7220 7661  ><a:schemeClr va
+00001630: 6c3d 2270 6843 6c72 223e 3c61 3a6c 756d  l="phClr"><a:lum
+00001640: 4d6f 6420 7661 6c3d 2231 3035 3030 3022  Mod val="105000"
+00001650: 2f3e 3c61 3a73 6174 4d6f 6420 7661 6c3d  /><a:satMod val=
+00001660: 2231 3033 3030 3022 2f3e 3c61 3a74 696e  "103000"/><a:tin
+00001670: 7420 7661 6c3d 2237 3330 3030 222f 3e3c  t val="73000"/><
+00001680: 2f61 3a73 6368 656d 6543 6c72 3e3c 2f61  /a:schemeClr></a
+00001690: 3a67 733e 3c61 3a67 7320 706f 733d 2231  :gs><a:gs pos="1
+000016a0: 3030 3030 3022 3e3c 613a 7363 6865 6d65  00000"><a:scheme
+000016b0: 436c 7220 7661 6c3d 2270 6843 6c72 223e  Clr val="phClr">
+000016c0: 3c61 3a6c 756d 4d6f 6420 7661 6c3d 2231  <a:lumMod val="1
+000016d0: 3035 3030 3022 2f3e 3c61 3a73 6174 4d6f  05000"/><a:satMo
+000016e0: 6420 7661 6c3d 2231 3039 3030 3022 2f3e  d val="109000"/>
+000016f0: 3c61 3a74 696e 7420 7661 6c3d 2238 3130  <a:tint val="810
+00001700: 3030 222f 3e3c 2f61 3a73 6368 656d 6543  00"/></a:schemeC
+00001710: 6c72 3e3c 2f61 3a67 733e 3c2f 613a 6773  lr></a:gs></a:gs
+00001720: 4c73 743e 3c61 3a6c 696e 2061 6e67 3d22  Lst><a:lin ang="
+00001730: 3534 3030 3030 3022 2073 6361 6c65 643d  5400000" scaled=
+00001740: 2230 222f 3e3c 2f61 3a67 7261 6446 696c  "0"/></a:gradFil
+00001750: 6c3e 3c61 3a67 7261 6446 696c 6c20 726f  l><a:gradFill ro
+00001760: 7457 6974 6853 6861 7065 3d22 3122 3e3c  tWithShape="1"><
+00001770: 613a 6773 4c73 743e 3c61 3a67 7320 706f  a:gsLst><a:gs po
+00001780: 733d 2230 223e 3c61 3a73 6368 656d 6543  s="0"><a:schemeC
+00001790: 6c72 2076 616c 3d22 7068 436c 7222 3e3c  lr val="phClr"><
+000017a0: 613a 7361 744d 6f64 2076 616c 3d22 3130  a:satMod val="10
+000017b0: 3330 3030 222f 3e3c 613a 6c75 6d4d 6f64  3000"/><a:lumMod
+000017c0: 2076 616c 3d22 3130 3230 3030 222f 3e3c   val="102000"/><
+000017d0: 613a 7469 6e74 2076 616c 3d22 3934 3030  a:tint val="9400
+000017e0: 3022 2f3e 3c2f 613a 7363 6865 6d65 436c  0"/></a:schemeCl
+000017f0: 723e 3c2f 613a 6773 3e3c 613a 6773 2070  r></a:gs><a:gs p
+00001800: 6f73 3d22 3530 3030 3022 3e3c 613a 7363  os="50000"><a:sc
+00001810: 6865 6d65 436c 7220 7661 6c3d 2270 6843  hemeClr val="phC
+00001820: 6c72 223e 3c61 3a73 6174 4d6f 6420 7661  lr"><a:satMod va
+00001830: 6c3d 2231 3130 3030 3022 2f3e 3c61 3a6c  l="110000"/><a:l
+00001840: 756d 4d6f 6420 7661 6c3d 2231 3030 3030  umMod val="10000
+00001850: 3022 2f3e 3c61 3a73 6861 6465 2076 616c  0"/><a:shade val
+00001860: 3d22 3130 3030 3030 222f 3e3c 2f61 3a73  ="100000"/></a:s
+00001870: 6368 656d 6543 6c72 3e3c 2f61 3a67 733e  chemeClr></a:gs>
+00001880: 3c61 3a67 7320 706f 733d 2231 3030 3030  <a:gs pos="10000
+00001890: 3022 3e3c 613a 7363 6865 6d65 436c 7220  0"><a:schemeClr 
+000018a0: 7661 6c3d 2270 6843 6c72 223e 3c61 3a6c  val="phClr"><a:l
+000018b0: 756d 4d6f 6420 7661 6c3d 2239 3930 3030  umMod val="99000
+000018c0: 222f 3e3c 613a 7361 744d 6f64 2076 616c  "/><a:satMod val
+000018d0: 3d22 3132 3030 3030 222f 3e3c 613a 7368  ="120000"/><a:sh
+000018e0: 6164 6520 7661 6c3d 2237 3830 3030 222f  ade val="78000"/
+000018f0: 3e3c 2f61 3a73 6368 656d 6543 6c72 3e3c  ></a:schemeClr><
+00001900: 2f61 3a67 733e 3c2f 613a 6773 4c73 743e  /a:gs></a:gsLst>
+00001910: 3c61 3a6c 696e 2061 6e67 3d22 3534 3030  <a:lin ang="5400
+00001920: 3030 3022 2073 6361 6c65 643d 2230 222f  000" scaled="0"/
+00001930: 3e3c 2f61 3a67 7261 6446 696c 6c3e 3c2f  ></a:gradFill></
+00001940: 613a 6669 6c6c 5374 796c 654c 7374 3e3c  a:fillStyleLst><
+00001950: 613a 6c6e 5374 796c 654c 7374 3e3c 613a  a:lnStyleLst><a:
+00001960: 6c6e 2077 3d22 3633 3530 2220 6361 703d  ln w="6350" cap=
+00001970: 2266 6c61 7422 2063 6d70 643d 2273 6e67  "flat" cmpd="sng
+00001980: 2220 616c 676e 3d22 6374 7222 3e3c 613a  " algn="ctr"><a:
+00001990: 736f 6c69 6446 696c 6c3e 3c61 3a73 6368  solidFill><a:sch
+000019a0: 656d 6543 6c72 2076 616c 3d22 7068 436c  emeClr val="phCl
+000019b0: 7222 2f3e 3c2f 613a 736f 6c69 6446 696c  r"/></a:solidFil
+000019c0: 6c3e 3c61 3a70 7273 7444 6173 6820 7661  l><a:prstDash va
+000019d0: 6c3d 2273 6f6c 6964 222f 3e3c 613a 6d69  l="solid"/><a:mi
+000019e0: 7465 7220 6c69 6d3d 2238 3030 3030 3022  ter lim="800000"
+000019f0: 2f3e 3c2f 613a 6c6e 3e3c 613a 6c6e 2077  /></a:ln><a:ln w
+00001a00: 3d22 3132 3730 3022 2063 6170 3d22 666c  ="12700" cap="fl
+00001a10: 6174 2220 636d 7064 3d22 736e 6722 2061  at" cmpd="sng" a
+00001a20: 6c67 6e3d 2263 7472 223e 3c61 3a73 6f6c  lgn="ctr"><a:sol
+00001a30: 6964 4669 6c6c 3e3c 613a 7363 6865 6d65  idFill><a:scheme
+00001a40: 436c 7220 7661 6c3d 2270 6843 6c72 222f  Clr val="phClr"/
+00001a50: 3e3c 2f61 3a73 6f6c 6964 4669 6c6c 3e3c  ></a:solidFill><
+00001a60: 613a 7072 7374 4461 7368 2076 616c 3d22  a:prstDash val="
+00001a70: 736f 6c69 6422 2f3e 3c61 3a6d 6974 6572  solid"/><a:miter
+00001a80: 206c 696d 3d22 3830 3030 3030 222f 3e3c   lim="800000"/><
+00001a90: 2f61 3a6c 6e3e 3c61 3a6c 6e20 773d 2231  /a:ln><a:ln w="1
+00001aa0: 3930 3530 2220 6361 703d 2266 6c61 7422  9050" cap="flat"
+00001ab0: 2063 6d70 643d 2273 6e67 2220 616c 676e   cmpd="sng" algn
+00001ac0: 3d22 6374 7222 3e3c 613a 736f 6c69 6446  ="ctr"><a:solidF
+00001ad0: 696c 6c3e 3c61 3a73 6368 656d 6543 6c72  ill><a:schemeClr
+00001ae0: 2076 616c 3d22 7068 436c 7222 2f3e 3c2f   val="phClr"/></
+00001af0: 613a 736f 6c69 6446 696c 6c3e 3c61 3a70  a:solidFill><a:p
+00001b00: 7273 7444 6173 6820 7661 6c3d 2273 6f6c  rstDash val="sol
+00001b10: 6964 222f 3e3c 613a 6d69 7465 7220 6c69  id"/><a:miter li
+00001b20: 6d3d 2238 3030 3030 3022 2f3e 3c2f 613a  m="800000"/></a:
+00001b30: 6c6e 3e3c 2f61 3a6c 6e53 7479 6c65 4c73  ln></a:lnStyleLs
+00001b40: 743e 3c61 3a65 6666 6563 7453 7479 6c65  t><a:effectStyle
+00001b50: 4c73 743e 3c61 3a65 6666 6563 7453 7479  Lst><a:effectSty
+00001b60: 6c65 3e3c 613a 6566 6665 6374 4c73 742f  le><a:effectLst/
+00001b70: 3e3c 2f61 3a65 6666 6563 7453 7479 6c65  ></a:effectStyle
+00001b80: 3e3c 613a 6566 6665 6374 5374 796c 653e  ><a:effectStyle>
+00001b90: 3c61 3a65 6666 6563 744c 7374 2f3e 3c2f  <a:effectLst/></
+00001ba0: 613a 6566 6665 6374 5374 796c 653e 3c61  a:effectStyle><a
+00001bb0: 3a65 6666 6563 7453 7479 6c65 3e3c 613a  :effectStyle><a:
+00001bc0: 6566 6665 6374 4c73 743e 3c61 3a6f 7574  effectLst><a:out
+00001bd0: 6572 5368 6477 2062 6c75 7252 6164 3d22  erShdw blurRad="
+00001be0: 3537 3135 3022 2064 6973 743d 2231 3930  57150" dist="190
+00001bf0: 3530 2220 6469 723d 2235 3430 3030 3030  50" dir="5400000
+00001c00: 2220 616c 676e 3d22 6374 7222 2072 6f74  " algn="ctr" rot
+00001c10: 5769 7468 5368 6170 653d 2230 223e 3c61  WithShape="0"><a
+00001c20: 3a73 7267 6243 6c72 2076 616c 3d22 3030  :srgbClr val="00
+00001c30: 3030 3030 223e 3c61 3a61 6c70 6861 2076  0000"><a:alpha v
+00001c40: 616c 3d22 3633 3030 3022 2f3e 3c2f 613a  al="63000"/></a:
+00001c50: 7372 6762 436c 723e 3c2f 613a 6f75 7465  srgbClr></a:oute
+00001c60: 7253 6864 773e 3c2f 613a 6566 6665 6374  rShdw></a:effect
+00001c70: 4c73 743e 3c2f 613a 6566 6665 6374 5374  Lst></a:effectSt
+00001c80: 796c 653e 3c2f 613a 6566 6665 6374 5374  yle></a:effectSt
+00001c90: 796c 654c 7374 3e3c 613a 6267 4669 6c6c  yleLst><a:bgFill
+00001ca0: 5374 796c 654c 7374 3e3c 613a 736f 6c69  StyleLst><a:soli
+00001cb0: 6446 696c 6c3e 3c61 3a73 6368 656d 6543  dFill><a:schemeC
+00001cc0: 6c72 2076 616c 3d22 7068 436c 7222 2f3e  lr val="phClr"/>
+00001cd0: 3c2f 613a 736f 6c69 6446 696c 6c3e 3c61  </a:solidFill><a
+00001ce0: 3a73 6f6c 6964 4669 6c6c 3e3c 613a 7363  :solidFill><a:sc
+00001cf0: 6865 6d65 436c 7220 7661 6c3d 2270 6843  hemeClr val="phC
+00001d00: 6c72 223e 3c61 3a74 696e 7420 7661 6c3d  lr"><a:tint val=
+00001d10: 2239 3530 3030 222f 3e3c 613a 7361 744d  "95000"/><a:satM
+00001d20: 6f64 2076 616c 3d22 3137 3030 3030 222f  od val="170000"/
+00001d30: 3e3c 2f61 3a73 6368 656d 6543 6c72 3e3c  ></a:schemeClr><
+00001d40: 2f61 3a73 6f6c 6964 4669 6c6c 3e3c 613a  /a:solidFill><a:
+00001d50: 6772 6164 4669 6c6c 2072 6f74 5769 7468  gradFill rotWith
+00001d60: 5368 6170 653d 2231 223e 3c61 3a67 734c  Shape="1"><a:gsL
+00001d70: 7374 3e3c 613a 6773 2070 6f73 3d22 3022  st><a:gs pos="0"
+00001d80: 3e3c 613a 7363 6865 6d65 436c 7220 7661  ><a:schemeClr va
+00001d90: 6c3d 2270 6843 6c72 223e 3c61 3a74 696e  l="phClr"><a:tin
+00001da0: 7420 7661 6c3d 2239 3330 3030 222f 3e3c  t val="93000"/><
+00001db0: 613a 7361 744d 6f64 2076 616c 3d22 3135  a:satMod val="15
+00001dc0: 3030 3030 222f 3e3c 613a 7368 6164 6520  0000"/><a:shade 
+00001dd0: 7661 6c3d 2239 3830 3030 222f 3e3c 613a  val="98000"/><a:
+00001de0: 6c75 6d4d 6f64 2076 616c 3d22 3130 3230  lumMod val="1020
+00001df0: 3030 222f 3e3c 2f61 3a73 6368 656d 6543  00"/></a:schemeC
+00001e00: 6c72 3e3c 2f61 3a67 733e 3c61 3a67 7320  lr></a:gs><a:gs 
+00001e10: 706f 733d 2235 3030 3030 223e 3c61 3a73  pos="50000"><a:s
+00001e20: 6368 656d 6543 6c72 2076 616c 3d22 7068  chemeClr val="ph
+00001e30: 436c 7222 3e3c 613a 7469 6e74 2076 616c  Clr"><a:tint val
+00001e40: 3d22 3938 3030 3022 2f3e 3c61 3a73 6174  ="98000"/><a:sat
+00001e50: 4d6f 6420 7661 6c3d 2231 3330 3030 3022  Mod val="130000"
+00001e60: 2f3e 3c61 3a73 6861 6465 2076 616c 3d22  /><a:shade val="
+00001e70: 3930 3030 3022 2f3e 3c61 3a6c 756d 4d6f  90000"/><a:lumMo
+00001e80: 6420 7661 6c3d 2231 3033 3030 3022 2f3e  d val="103000"/>
+00001e90: 3c2f 613a 7363 6865 6d65 436c 723e 3c2f  </a:schemeClr></
+00001ea0: 613a 6773 3e3c 613a 6773 2070 6f73 3d22  a:gs><a:gs pos="
+00001eb0: 3130 3030 3030 223e 3c61 3a73 6368 656d  100000"><a:schem
+00001ec0: 6543 6c72 2076 616c 3d22 7068 436c 7222  eClr val="phClr"
+00001ed0: 3e3c 613a 7368 6164 6520 7661 6c3d 2236  ><a:shade val="6
+00001ee0: 3330 3030 222f 3e3c 613a 7361 744d 6f64  3000"/><a:satMod
+00001ef0: 2076 616c 3d22 3132 3030 3030 222f 3e3c   val="120000"/><
+00001f00: 2f61 3a73 6368 656d 6543 6c72 3e3c 2f61  /a:schemeClr></a
+00001f10: 3a67 733e 3c2f 613a 6773 4c73 743e 3c61  :gs></a:gsLst><a
+00001f20: 3a6c 696e 2061 6e67 3d22 3534 3030 3030  :lin ang="540000
+00001f30: 3022 2073 6361 6c65 643d 2230 222f 3e3c  0" scaled="0"/><
+00001f40: 2f61 3a67 7261 6446 696c 6c3e 3c2f 613a  /a:gradFill></a:
+00001f50: 6267 4669 6c6c 5374 796c 654c 7374 3e3c  bgFillStyleLst><
+00001f60: 2f61 3a66 6d74 5363 6865 6d65 3e3c 2f61  /a:fmtScheme></a
+00001f70: 3a74 6865 6d65 456c 656d 656e 7473 3e3c  :themeElements><
+00001f80: 613a 6f62 6a65 6374 4465 6661 756c 7473  a:objectDefaults
+00001f90: 2f3e 3c61 3a65 7874 7261 436c 7253 6368  /><a:extraClrSch
+00001fa0: 656d 654c 7374 2f3e 3c61 3a65 7874 4c73  emeLst/><a:extLs
+00001fb0: 743e 3c61 3a65 7874 2075 7269 3d22 7b30  t><a:ext uri="{0
+00001fc0: 3541 3443 3235 432d 3038 3545 2d34 3334  5A4C25C-085E-434
+00001fd0: 302d 3835 4133 2d41 3535 3331 4535 3130  0-85A3-A5531E510
+00001fe0: 4442 327d 223e 3c74 686d 3135 3a74 6865  DB2}"><thm15:the
+00001ff0: 6d65 4661 6d69 6c79 2078 6d6c 6e73 3a74  meFamily xmlns:t
+00002000: 686d 3135 3d22 6874 7470 3a2f 2f73 6368  hm15="http://sch
+00002010: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
+00002020: 6f6d 2f6f 6666 6963 652f 7468 656d 656d  om/office/themem
+00002030: 6c2f 3230 3132 2f6d 6169 6e22 206e 616d  l/2012/main" nam
+00002040: 653d 224f 6666 6963 6520 5468 656d 6522  e="Office Theme"
+00002050: 2069 643d 227b 3632 4639 3339 4236 2d39   id="{62F939B6-9
+00002060: 3341 462d 3444 4238 2d39 4336 422d 4436  3AF-4DB8-9C6B-D6
+00002070: 4337 4446 4443 3538 3946 7d22 2076 6964  C7DFDC589F}" vid
+00002080: 3d22 7b34 4133 4334 3645 382d 3631 4343  ="{4A3C46E8-61CC
+00002090: 2d34 3630 332d 4135 3839 2d37 3432 3241  -4603-A589-7422A
+000020a0: 3437 4138 4534 417d 222f 3e3c 2f61 3a65  47A8E4A}"/></a:e
+000020b0: 7874 3e3c 2f61 3a65 7874 4c73 743e 3c2f  xt></a:extLst></
+000020c0: 613a 7468 656d 653e                      a:theme>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-docx-template/word/webSettings.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-docx-template/word/webSettings.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text, with very long lines (837), with CRLF line terminators*

 * *Files 1% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
-00000030: 2279 6573 223f 3e0d 0a3c 773a 7765 6253  "yes"?>..<w:webS
-00000040: 6574 7469 6e67 7320 786d 6c6e 733a 6d63  ettings xmlns:mc
-00000050: 3d22 6874 7470 3a2f 2f73 6368 656d 6173  ="http://schemas
-00000060: 2e6f 7065 6e78 6d6c 666f 726d 6174 732e  .openxmlformats.
-00000070: 6f72 672f 6d61 726b 7570 2d63 6f6d 7061  org/markup-compa
-00000080: 7469 6269 6c69 7479 2f32 3030 3622 2078  tibility/2006" x
-00000090: 6d6c 6e73 3a72 3d22 6874 7470 3a2f 2f73  mlns:r="http://s
-000000a0: 6368 656d 6173 2e6f 7065 6e78 6d6c 666f  chemas.openxmlfo
-000000b0: 726d 6174 732e 6f72 672f 6f66 6669 6365  rmats.org/office
-000000c0: 446f 6375 6d65 6e74 2f32 3030 362f 7265  Document/2006/re
-000000d0: 6c61 7469 6f6e 7368 6970 7322 2078 6d6c  lationships" xml
-000000e0: 6e73 3a77 3d22 6874 7470 3a2f 2f73 6368  ns:w="http://sch
-000000f0: 656d 6173 2e6f 7065 6e78 6d6c 666f 726d  emas.openxmlform
-00000100: 6174 732e 6f72 672f 776f 7264 7072 6f63  ats.org/wordproc
-00000110: 6573 7369 6e67 6d6c 2f32 3030 362f 6d61  essingml/2006/ma
-00000120: 696e 2220 786d 6c6e 733a 7731 343d 2268  in" xmlns:w14="h
-00000130: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
-00000140: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
-00000150: 6365 2f77 6f72 642f 3230 3130 2f77 6f72  ce/word/2010/wor
-00000160: 646d 6c22 2078 6d6c 6e73 3a77 3135 3d22  dml" xmlns:w15="
-00000170: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
-00000180: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
-00000190: 6963 652f 776f 7264 2f32 3031 322f 776f  ice/word/2012/wo
-000001a0: 7264 6d6c 2220 786d 6c6e 733a 7731 3663  rdml" xmlns:w16c
-000001b0: 6578 3d22 6874 7470 3a2f 2f73 6368 656d  ex="http://schem
-000001c0: 6173 2e6d 6963 726f 736f 6674 2e63 6f6d  as.microsoft.com
-000001d0: 2f6f 6666 6963 652f 776f 7264 2f32 3031  /office/word/201
-000001e0: 382f 776f 7264 6d6c 2f63 6578 2220 786d  8/wordml/cex" xm
-000001f0: 6c6e 733a 7731 3663 6964 3d22 6874 7470  lns:w16cid="http
-00000200: 3a2f 2f73 6368 656d 6173 2e6d 6963 726f  ://schemas.micro
-00000210: 736f 6674 2e63 6f6d 2f6f 6666 6963 652f  soft.com/office/
-00000220: 776f 7264 2f32 3031 362f 776f 7264 6d6c  word/2016/wordml
-00000230: 2f63 6964 2220 786d 6c6e 733a 7731 363d  /cid" xmlns:w16=
-00000240: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
-00000250: 6d69 6372 6f73 6f66 742e 636f 6d2f 6f66  microsoft.com/of
-00000260: 6669 6365 2f77 6f72 642f 3230 3138 2f77  fice/word/2018/w
-00000270: 6f72 646d 6c22 2078 6d6c 6e73 3a77 3136  ordml" xmlns:w16
-00000280: 7364 7464 683d 2268 7474 703a 2f2f 7363  sdtdh="http://sc
-00000290: 6865 6d61 732e 6d69 6372 6f73 6f66 742e  hemas.microsoft.
-000002a0: 636f 6d2f 6f66 6669 6365 2f77 6f72 642f  com/office/word/
-000002b0: 3230 3230 2f77 6f72 646d 6c2f 7364 7464  2020/wordml/sdtd
-000002c0: 6174 6168 6173 6822 2078 6d6c 6e73 3a77  atahash" xmlns:w
-000002d0: 3136 7365 3d22 6874 7470 3a2f 2f73 6368  16se="http://sch
-000002e0: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
-000002f0: 6f6d 2f6f 6666 6963 652f 776f 7264 2f32  om/office/word/2
-00000300: 3031 352f 776f 7264 6d6c 2f73 796d 6578  015/wordml/symex
-00000310: 2220 6d63 3a49 676e 6f72 6162 6c65 3d22  " mc:Ignorable="
-00000320: 7731 3420 7731 3520 7731 3673 6520 7731  w14 w15 w16se w1
-00000330: 3663 6964 2077 3136 2077 3136 6365 7820  6cid w16 w16cex 
-00000340: 7731 3673 6474 6468 223e 3c77 3a6f 7074  w16sdtdh"><w:opt
-00000350: 696d 697a 6546 6f72 4272 6f77 7365 722f  imizeForBrowser/
-00000360: 3e3c 773a 616c 6c6f 7750 4e47 2f3e 3c2f  ><w:allowPNG/></
-00000370: 773a 7765 6253 6574 7469 6e67 733e       w:webSettings>
+00000030: 2279 6573 223f 3e0a 3c77 3a77 6562 5365  "yes"?>.<w:webSe
+00000040: 7474 696e 6773 2078 6d6c 6e73 3a6d 633d  ttings xmlns:mc=
+00000050: 2268 7474 703a 2f2f 7363 6865 6d61 732e  "http://schemas.
+00000060: 6f70 656e 786d 6c66 6f72 6d61 7473 2e6f  openxmlformats.o
+00000070: 7267 2f6d 6172 6b75 702d 636f 6d70 6174  rg/markup-compat
+00000080: 6962 696c 6974 792f 3230 3036 2220 786d  ibility/2006" xm
+00000090: 6c6e 733a 723d 2268 7474 703a 2f2f 7363  lns:r="http://sc
+000000a0: 6865 6d61 732e 6f70 656e 786d 6c66 6f72  hemas.openxmlfor
+000000b0: 6d61 7473 2e6f 7267 2f6f 6666 6963 6544  mats.org/officeD
+000000c0: 6f63 756d 656e 742f 3230 3036 2f72 656c  ocument/2006/rel
+000000d0: 6174 696f 6e73 6869 7073 2220 786d 6c6e  ationships" xmln
+000000e0: 733a 773d 2268 7474 703a 2f2f 7363 6865  s:w="http://sche
+000000f0: 6d61 732e 6f70 656e 786d 6c66 6f72 6d61  mas.openxmlforma
+00000100: 7473 2e6f 7267 2f77 6f72 6470 726f 6365  ts.org/wordproce
+00000110: 7373 696e 676d 6c2f 3230 3036 2f6d 6169  ssingml/2006/mai
+00000120: 6e22 2078 6d6c 6e73 3a77 3134 3d22 6874  n" xmlns:w14="ht
+00000130: 7470 3a2f 2f73 6368 656d 6173 2e6d 6963  tp://schemas.mic
+00000140: 726f 736f 6674 2e63 6f6d 2f6f 6666 6963  rosoft.com/offic
+00000150: 652f 776f 7264 2f32 3031 302f 776f 7264  e/word/2010/word
+00000160: 6d6c 2220 786d 6c6e 733a 7731 353d 2268  ml" xmlns:w15="h
+00000170: 7474 703a 2f2f 7363 6865 6d61 732e 6d69  ttp://schemas.mi
+00000180: 6372 6f73 6f66 742e 636f 6d2f 6f66 6669  crosoft.com/offi
+00000190: 6365 2f77 6f72 642f 3230 3132 2f77 6f72  ce/word/2012/wor
+000001a0: 646d 6c22 2078 6d6c 6e73 3a77 3136 6365  dml" xmlns:w16ce
+000001b0: 783d 2268 7474 703a 2f2f 7363 6865 6d61  x="http://schema
+000001c0: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
+000001d0: 6f66 6669 6365 2f77 6f72 642f 3230 3138  office/word/2018
+000001e0: 2f77 6f72 646d 6c2f 6365 7822 2078 6d6c  /wordml/cex" xml
+000001f0: 6e73 3a77 3136 6369 643d 2268 7474 703a  ns:w16cid="http:
+00000200: 2f2f 7363 6865 6d61 732e 6d69 6372 6f73  //schemas.micros
+00000210: 6f66 742e 636f 6d2f 6f66 6669 6365 2f77  oft.com/office/w
+00000220: 6f72 642f 3230 3136 2f77 6f72 646d 6c2f  ord/2016/wordml/
+00000230: 6369 6422 2078 6d6c 6e73 3a77 3136 3d22  cid" xmlns:w16="
+00000240: 6874 7470 3a2f 2f73 6368 656d 6173 2e6d  http://schemas.m
+00000250: 6963 726f 736f 6674 2e63 6f6d 2f6f 6666  icrosoft.com/off
+00000260: 6963 652f 776f 7264 2f32 3031 382f 776f  ice/word/2018/wo
+00000270: 7264 6d6c 2220 786d 6c6e 733a 7731 3673  rdml" xmlns:w16s
+00000280: 6474 6468 3d22 6874 7470 3a2f 2f73 6368  dtdh="http://sch
+00000290: 656d 6173 2e6d 6963 726f 736f 6674 2e63  emas.microsoft.c
+000002a0: 6f6d 2f6f 6666 6963 652f 776f 7264 2f32  om/office/word/2
+000002b0: 3032 302f 776f 7264 6d6c 2f73 6474 6461  020/wordml/sdtda
+000002c0: 7461 6861 7368 2220 786d 6c6e 733a 7731  tahash" xmlns:w1
+000002d0: 3673 653d 2268 7474 703a 2f2f 7363 6865  6se="http://sche
+000002e0: 6d61 732e 6d69 6372 6f73 6f66 742e 636f  mas.microsoft.co
+000002f0: 6d2f 6f66 6669 6365 2f77 6f72 642f 3230  m/office/word/20
+00000300: 3135 2f77 6f72 646d 6c2f 7379 6d65 7822  15/wordml/symex"
+00000310: 206d 633a 4967 6e6f 7261 626c 653d 2277   mc:Ignorable="w
+00000320: 3134 2077 3135 2077 3136 7365 2077 3136  14 w15 w16se w16
+00000330: 6369 6420 7731 3620 7731 3663 6578 2077  cid w16 w16cex w
+00000340: 3136 7364 7464 6822 3e3c 773a 6f70 7469  16sdtdh"><w:opti
+00000350: 6d69 7a65 466f 7242 726f 7773 6572 2f3e  mizeForBrowser/>
+00000360: 3c77 3a61 6c6c 6f77 504e 472f 3e3c 2f77  <w:allowPNG/></w
+00000370: 3a77 6562 5365 7474 696e 6773 3e         :webSettings>
```

### Comparing `python_docx_ng-0.9.3/docx/templates/default-footer.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-footer.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/templates/default-header.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-header.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/templates/default-settings.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-settings.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/templates/default-styles.xml` & `python_docx_ng-0.9.4.dev0/docx/templates/default-styles.xml`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/templates/default.docx` & `python_docx_ng-0.9.4.dev0/docx/templates/default.docx`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/docx/text/font.py` & `python_docx_ng-0.9.4.dev0/docx/text/font.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,33 @@
     @name.setter
     def name(self, value):
         rPr = self._element.get_or_add_rPr()
         rPr.rFonts_ascii = value
         rPr.rFonts_hAnsi = value
 
     @property
+    def theme(self):
+        """
+        Get or set the typeface theme for this |Font| instance, causing the
+        text it controls to appear in the themed font, if a matching font is
+        found. |None| indicates the typeface is inherited from the style
+        hierarchy.
+        """
+        rPr = self._element.rPr
+        if rPr is None:
+            return None
+        return rPr.rFonts_asciiTheme
+
+    @theme.setter
+    def theme(self, value):
+        rPr = self._element.get_or_add_rPr()
+        rPr.rFonts_asciiTheme = value
+        rPr.rFonts_hAnsiTheme = value
+
+    @property
     def no_proof(self):
         """
         Read/write tri-state value. When |True|, specifies that the contents
         of this run should not report any errors when the document is scanned
         for spelling and grammar.
         """
         return self._get_bool_prop('noProof')
```

### Comparing `python_docx_ng-0.9.3/docx/text/parfmt.py` & `python_docx_ng-0.9.4.dev0/docx/text/parfmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,30 @@
 
     @right_indent.setter
     def right_indent(self, value):
         pPr = self._element.get_or_add_pPr()
         pPr.ind_right = value
 
     @property
+    def shading_fill(self):
+        """
+        A member of :ref:`WdColorIndex` indicating the color of highlighting
+        applied, or `None` if no highlighting is applied.
+        """
+        pPr = self._element.pPr
+        if pPr is None:
+            return None
+        return pPr.shading_fill
+
+    @shading_fill.setter
+    def shading_fill(self, value):
+        pPr = self._element.get_or_add_pPr()
+        pPr.shading_fill = value
+
+    @property
     def space_after(self):
         """
         |Length| value specifying the spacing to appear between this
         paragraph and the subsequent paragraph. |None| indicates this value
         is inherited from the style hierarchy. |Length| objects provide
         convenience properties, such as :attr:`~.Length.pt` and
         :attr:`~.Length.inches`, that allow easy conversion to various length
```

### Comparing `python_docx_ng-0.9.3/docx/text/run.py` & `python_docx_ng-0.9.4.dev0/docx/text/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # encoding: utf-8
 
 """
 Run-related proxy objects for python-docx, Run in particular.
 """
 
 from __future__ import absolute_import, print_function, unicode_literals
+from datetime import datetime
+
+from docx.oxml.ns import qn
+from docx.opc.part import PackURI, Part
 
 from ..enum.style import WD_STYLE_TYPE
 from ..enum.text import WD_BREAK
 from .font import Font
 from ..shape import InlineShape
 from ..shared import Parented
 
+from .comment import Comment
+
 
 class Run(Parented):
     """
     Proxy object wrapping ``<w:r>`` element. Several of the properties on Run
     take a tri-state value, |True|, |False|, or |None|. |True| and |False|
     correspond to on and off respectively. |None| indicates the property is
     not specified directly on the run and its effective value is taken from
@@ -76,14 +82,22 @@
         ``<w:t>`` child element) to the run, containing *text*. Compare with
         the possibly more friendly approach of assigning text to the
         :attr:`Run.text` property.
         """
         t = self._r.add_t(text)
         return _Text(t)
 
+    def add_comment(self, text, author='python-docx', initials='pd', dtime=None):
+        comment_part = self.part._comments_part.element
+        if dtime is None:
+            dtime = str(datetime.now()).replace(' ', 'T')
+        comment = self._r.add_comm(author, comment_part, initials, dtime, text)
+
+        return comment
+
     @property
     def bold(self):
         """
         Read/write. Causes the text of the run to appear in bold.
         """
         return self.font.bold
 
@@ -177,14 +191,99 @@
         """
         return self.font.underline
 
     @underline.setter
     def underline(self, value):
         self.font.underline = value
 
+    @property
+    def footnote(self):
+        _id = self._r.footnote_id
+
+        if _id is not None:
+            footnotes_part = self._parent._parent.part._footnotes_part.element
+            footnote = footnotes_part.get_footnote_by_id(_id)
+            return footnote.paragraph.text
+        else:
+            return None
+
+    @property
+    def is_hyperlink(self):
+        '''
+        checks if the run is nested inside a hyperlink element
+        '''
+        return self.element.getparent().tag.split('}')[1] == 'hyperlink'
+
+    def get_hyperlink(self):
+        """
+        returns the text of the hyperlink of the run in case of the run has a hyperlink
+        """
+        document = self._parent._parent.document
+        parent = self.element.getparent()
+        linkText = ''
+        if self.is_hyperlink:
+            if parent.attrib.__contains__(qn('r:id')):
+                rId = parent.get(qn('r:id'))
+                linkText = document._part._rels[rId].target_ref
+                return linkText, True
+            elif parent.attrib.__contains__(qn('w:anchor')):
+                linkText = parent.get(qn('w:anchor'))
+                return linkText, False
+            else:
+                # TBD: review... no prints!
+                print('No link in hyperlink!')
+                print(self.text)
+                return '', False
+        else:
+            return ''
+
+    @property
+    def comments(self):
+        comment_part = self._parent._parent.part._comments_part.element
+        comment_refs = self._element.findall(qn('w:commentReference'))
+        ids = [int(ref.get(qn('w:id'))) for ref in comment_refs]
+        coms = [com for com in comment_part if com._id in ids]
+        return [Comment(com, comment_part) for com in coms]
+
+    def add_ole_object_to_run(self, ole_object_path):
+        """
+        Add saved OLE Object in the disk to an run and retun the newly created relationship ID
+        Note: OLE Objects must be stored in the disc as `.bin` file
+        """
+        reltype: str = "http://schemas.openxmlformats.org/officeDocument/2006/relationships/oleObject"
+        pack_path: str = "/word/embeddings/" + ole_object_path.split("\\")[-1]
+        partname = PackURI(pack_path)
+        content_type: str = "application/vnd.openxmlformats-officedocument.oleObject"
+
+        with open(ole_object_path, "rb") as f:
+            blob = f.read()
+        target_part = Part(partname=partname, content_type=content_type, blob=blob)
+        rel_id: str = self.part.rels._next_rId
+        self.part.rels.add_relationship(reltype=reltype, target=target_part, rId=rel_id)
+        return rel_id
+
+    def add_fldChar(self, fldCharType, fldLock: bool = False, dirty: bool = False):
+
+        fldChar = self._r.add_fldChar(fldCharType, fldLock, dirty)
+        return fldChar
+
+    @property
+    def instr_text(self):
+        return self._r.instr_text
+
+    @instr_text.setter
+    def instr_text(self, instr_text_val):
+        self._r.instr_text = instr_text_val
+
+    def remove_instr_text(self):
+        if self.instr_text is None:
+            return None
+        else:
+            self._r._remove_instr_text()
+
 
 class _Text(object):
     """
     Proxy object wrapping ``<w:t>`` element.
     """
     def __init__(self, t_elm):
         super(_Text, self).__init__()
```

### Comparing `python_docx_ng-0.9.3/docx/text/tabstops.py` & `python_docx_ng-0.9.4.dev0/docx/text/tabstops.py`

 * *Files identical despite different names*

### Comparing `python_docx_ng-0.9.3/pyproject.toml` & `python_docx_ng-0.9.4.dev0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-docx-ng"
-version = "0.9.3"
+version = "0.9.4-dev"
 description = "python-docx-ng is a Python library for creating and updating Microsoft Word (.docx) files."
 authors = ["toxicphreAK <pentesting.laboratories@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "docx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `python_docx_ng-0.9.3/setup.py` & `python_docx_ng-0.9.4.dev0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,63 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# python-docx-ng
 
-packages = \
-['docx',
- 'docx.dml',
- 'docx.enum',
- 'docx.image',
- 'docx.opc',
- 'docx.opc.parts',
- 'docx.oxml',
- 'docx.oxml.text',
- 'docx.parts',
- 'docx.styles',
- 'docx.text']
-
-package_data = \
-{'': ['*'],
- 'docx': ['templates/*',
-          'templates/default-docx-template/*',
-          'templates/default-docx-template/_rels/*',
-          'templates/default-docx-template/docProps/*',
-          'templates/default-docx-template/word/*',
-          'templates/default-docx-template/word/_rels/*',
-          'templates/default-docx-template/word/theme/*']}
-
-install_requires = \
-['behave>=1.2.6,<2.0.0', 'lxml>=4.9.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'python-docx-ng',
-    'version': '0.9.3',
-    'description': 'python-docx-ng is a Python library for creating and updating Microsoft Word (.docx) files.',
-    'long_description': '# python-docx-ng\n\n*python-docx-ng* is a Python library for creating and updating Microsoft Word (.docx) files.\nIt was originally designed and developed by [scanny](https://github.com/scanny) as [python-docx](https://github.com/python-openxml/python-docx).\nAs he is not actively developing his repo and there are soo many useful pull requests, bringing together a more powerful tool.\nThis repo should merge a lot of those things and create a more powerful version, hopefully bearing the original structure of scanny in mind.\n\nA new documentation section will be build up soon based on Markdown in the [docs](docs) section.\nExamples can be found here: [examples](docs/examples)\nOlder information is available in the [python-docx Documentation](https://python-docx.readthedocs.org/en/latest/).\n\n## Installation\n\n```commandline\npip install python-docx-ng\n```\n\n> Hint: The library is called `docx` in python scripts, so use imports like `import docx`. \n\n## Features\n\n+ [x] Word 16 (Office 2019) Template ([54a1269](https://github.com/toxicphreAK/python-docx-ng/commit/54a1269a3608239adfef079840f69389235c88b8))\n+ [x] Faster & improved tables ([#1](https://github.com/toxicphreAK/python-docx-ng/pull/1))\n+ [x] SVG support ([#4](https://github.com/toxicphreAK/python-docx-ng/pull/4))\n+ [x] Font scaling ([#6](https://github.com/toxicphreAK/python-docx-ng/pull/6))\n+ [x] Outline level ([#7](https://github.com/toxicphreAK/python-docx-ng/pull/7)) - shows outline in navigation (e.g. Word or PDF application - not affecting the document itself)\n+ [x] RGB color font highlighting ([#14](https://github.com/toxicphreAK/python-docx-ng/pull/14))\n+ [x] Hyperlink text ([#16](https://github.com/toxicphreAK/python-docx-ng/pull/16))\n+ [x] `.docm` file support ([#19](https://github.com/toxicphreAK/python-docx-ng/pull/16)) - enables marco documents\n+ [x] Form fields & AltChunk support ([#20](https://github.com/toxicphreAK/python-docx-ng/pull/20))\n+ [x] Custom namespaces ([#21](https://github.com/toxicphreAK/python-docx-ng/pull/21))\n+ [x] Performance improvements\n  + Paragraph.text ([#3}(https://github.com/toxicphreAK/python-docx-ng/pull/3)\n  + Cache for table cells ([#8](https://github.com/toxicphreAK/python-docx-ng/pull/8))\n+ [x] Fixes\n  + add_picture ([#10](https://github.com/toxicphreAK/python-docx-ng/pull/10)) - fix next_id to support multiple pictures\n  + `Heading 1` key error due to style capitalization (e.g. in LibreOffice) ([#12](https://github.com/toxicphreAK/python-docx-ng/pull/12))\n  + Fix XPath for sectPr in document ([#15](https://github.com/toxicphreAK/python-docx-ng/pull/15))\n  + Reproducible documents ([#17](https://github.com/toxicphreAK/python-docx-ng/pull/17)) - same binary output with same data\n  + AttValue too long in etree xml parser ([#24](https://github.com/toxicphreAK/python-docx-ng/pull/24))\n\n## Roadmap\n\n+ [ ] Document all functionallities building a new sample document with *all* (most) features included\n+ [ ] Remove code references to original repo of python-docx\n+ [ ] Setup new docs (markdown based)\n+ [ ] Add missing tests\n',
-    'author': 'toxicphreAK',
-    'author_email': 'pentesting.laboratories@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
+*python-docx-ng* is a Python library for creating and updating Microsoft Word (.docx) files.
+It was originally designed and developed by [scanny](https://github.com/scanny) as [python-docx](https://github.com/python-openxml/python-docx).
+As he is not actively developing his repo and there are soo many useful pull requests, bringing together a more powerful tool.
+This repo should merge a lot of those things and create a more powerful version, hopefully bearing the original structure of scanny in mind.
+
+A new documentation section will be build up soon based on Markdown in the [docs](docs) section.
+Examples can be found here: [examples](docs/examples)
+Older information is available in the [python-docx Documentation](https://python-docx.readthedocs.org/en/latest/).
+
+## Installation
+
+```commandline
+pip install python-docx-ng
+```
+
+> Hint: The library is called `docx` in python scripts, so use imports like `import docx`. 
+
+## Features
+
++ [x] Extended Properties support [python-docx #1206](https://github.com/python-openxml/python-docx/pull/1206)
++ [x] Word 16 (Office 2019) Template ([54a1269](https://github.com/toxicphreAK/python-docx-ng/commit/54a1269a3608239adfef079840f69389235c88b8))
++ [x] Faster & improved tables ([#1](https://github.com/toxicphreAK/python-docx-ng/pull/1))
++ [x] SVG support ([#4](https://github.com/toxicphreAK/python-docx-ng/pull/4))
++ [x] EMF support ([85a30f1](https://github.com/toxicphreAK/python-docx-ng/commit/85a30f16a1f49767e331525346d8220926ecde39))
++ [x] WMF support ([9288ec9](https://github.com/toxicphreAK/python-docx-ng/commit/9288ec96db4faed53e46221e61100106e82934d8))
++ [x] Font scaling ([#6](https://github.com/toxicphreAK/python-docx-ng/pull/6))
++ [x] Outline level ([#7](https://github.com/toxicphreAK/python-docx-ng/pull/7)) - shows outline in navigation (e.g. Word or PDF application - not affecting the document itself)
++ [x] RGB color font highlighting ([#14](https://github.com/toxicphreAK/python-docx-ng/pull/14))
++ [x] Hyperlink text ([#16](https://github.com/toxicphreAK/python-docx-ng/pull/16))
++ [x] `.docm` file support ([#19](https://github.com/toxicphreAK/python-docx-ng/pull/16)) - enables marco documents
++ [x] Form fields & AltChunk support ([#20](https://github.com/toxicphreAK/python-docx-ng/pull/20))
++ [x] Custom namespaces ([#21](https://github.com/toxicphreAK/python-docx-ng/pull/21))
++ [x] Comment support ([85a30f1](https://github.com/toxicphreAK/python-docx-ng/commit/85a30f16a1f49767e331525346d8220926ecde39))
++ [x] Footnote support ([85a30f1](https://github.com/toxicphreAK/python-docx-ng/commit/85a30f16a1f49767e331525346d8220926ecde39))
++ [x] Shading support ([9288ec9](https://github.com/toxicphreAK/python-docx-ng/commit/9288ec96db4faed53e46221e61100106e82934d8))
++ [x] Performance improvements
+  + Paragraph.text ([#3}(https://github.com/toxicphreAK/python-docx-ng/pull/3)
+  + Cache for table cells ([#8](https://github.com/toxicphreAK/python-docx-ng/pull/8))
++ [x] Fixes
+  + Fix table issue [python-docx#1196](https://github.com/python-openxml/python-docx/pull/1196) - as table columns were not assigned correctly, see [python-docx#1193](https://github.com/python-openxml/python-docx/issues/1193)
+  + Fix table merging recusion [https://github.com/python-openxml/python-docx/issues/1208](https://github.com/python-openxml/python-docx/issues/1208) - replace recursion with for loop
+  + add_picture ([#10](https://github.com/toxicphreAK/python-docx-ng/pull/10)) - fix next_id to support multiple pictures
+  + `Heading 1` key error due to style capitalization (e.g. in LibreOffice) ([#12](https://github.com/toxicphreAK/python-docx-ng/pull/12))
+  + Fix XPath for sectPr in document ([#15](https://github.com/toxicphreAK/python-docx-ng/pull/15))
+  + Reproducible documents ([#17](https://github.com/toxicphreAK/python-docx-ng/pull/17)) - same binary output with same data
+  + AttValue too long in etree xml parser ([#24](https://github.com/toxicphreAK/python-docx-ng/pull/24))
+
+## Roadmap
+
++ [ ] Document all functionallities building a new sample document with *all* (most) features included
+  + [ ] Go through *all* Issues of python-docx repo
+    + Open & To Be Implemented:
+      + [ ] media file path issue - https://github.com/python-openxml/python-docx/pull/1205
+      + [ ] automatically update table of contents - https://github.com/python-openxml/python-docx/issues/1207
+      + [ ] specify table location (not at end of document) - https://github.com/python-openxml/python-docx/issues/1204
+      + [ ] read information from activex elements - https://github.com/python-openxml/python-docx/issues/1197
+      + [ ] begin new list numbering - https://github.com/python-openxml/python-docx/issues/1194
+  + [ ] Search on stackoverflow and document solutions
++ [ ] Remove code references to original repo of python-docx
++ [ ] Setup new docs (markdown based)
++ [ ] Add missing tests
```

