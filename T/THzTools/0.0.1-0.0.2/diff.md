# Comparing `tmp/thztools-0.0.1.tar.gz` & `tmp/thztools-0.0.2.tar.gz`

## Comparing `thztools-0.0.1.tar` & `thztools-0.0.2.tar`

### file list

```diff
@@ -1,716 +1,716 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 thztools-0.0.1/.DS_Store
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 thztools-0.0.1/.gitattributes
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/other.xml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/thztools.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 thztools-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180412 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52444 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18271 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0    19674 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_csv.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_csv.meta.json
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    23905 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    23380 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60720 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0   137664 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/ast.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/ast.meta.json
--rw-r--r--   0        0        0  1130456 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123361 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109248 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0    29692 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/csv.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/csv.meta.json
--rw-r--r--   0        0        0    57789 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   142252 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0    90167 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0   132111 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22432 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0    85381 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    52555 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    87532 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44437 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75241 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   167589 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    14417 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28524 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49785 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0    27792 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   162208 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   148698 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0    19597 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64759 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    42853 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0   239676 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432278 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57889 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    23833 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0    75677 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/zipfile.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/zipfile.meta.json
--rw-r--r--   0        0        0    89098 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   408032 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129027 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12244 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25117 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79314 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30901 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70623 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64615 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91163 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    15423 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/json/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/json/__init__.meta.json
--rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/json/decoder.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/json/decoder.meta.json
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/json/encoder.data.json
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/json/encoder.meta.json
--rw-r--r--   0        0        0   144429 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/logging/__init__.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/logging/__init__.meta.json
--rw-r--r--   0        0        0  2217665 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/__init__.data.json
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/__init__.meta.json
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_version.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_version.meta.json
--rw-r--r--   0        0        0   112541 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/version.meta.json
--rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/__init__.data.json
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/__init__.meta.json
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    25436 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_array_like.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json
--rw-r--r--   0        0        0   256912 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_callable.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_callable.meta.json
--rw-r--r--   0        0        0    41750 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json
--rw-r--r--   0        0        0    30730 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    34767 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nbit.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json
--rw-r--r--   0        0        0    16797 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_scalars.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_shape.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_shape.meta.json
--rw-r--r--   0        0        0   261391 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/compat/__init__.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/compat/__init__.meta.json
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/compat/_inspect.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/compat/_inspect.meta.json
--rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/compat/py3k.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/compat/py3k.meta.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    13683 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    11255 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    28038 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   169698 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    36087 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0   330727 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    49588 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   301784 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   196469 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    44548 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    25179 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/overrides.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/overrides.meta.json
--rw-r--r--   0        0        0    52653 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/records.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/records.meta.json
--rw-r--r--   0        0        0    52786 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    21751 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   107815 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    27705 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   136790 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    23356 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    14308 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27027 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   252832 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    15496 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    67750 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   323551 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   114237 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0   322665 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/__init__.data.json
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/__init__.meta.json
--rw-r--r--   0        0        0   100879 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_typing.data.json
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_typing.meta.json
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/testing.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/testing.meta.json
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_config/__init__.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_config/__init__.meta.json
--rw-r--r--   0        0        0    56793 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_config/config.data.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_config/config.meta.json
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/__init__.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/__init__.meta.json
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/indexing.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/indexing.meta.json
--rw-r--r--   0        0        0   175959 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/interval.data.json
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/interval.meta.json
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/lib.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/lib.meta.json
--rw-r--r--   0        0        0    31747 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/missing.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/missing.meta.json
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/ops_dispatch.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/ops_dispatch.meta.json
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/properties.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/properties.meta.json
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.meta.json
--rw-r--r--   0        0        0    58580 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.meta.json
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.meta.json
--rw-r--r--   0        0        0   125210 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.data.json
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.meta.json
--rw-r--r--   0        0        0    92339 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/period.data.json
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/period.meta.json
--rw-r--r--   0        0        0   190061 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.data.json
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.meta.json
--rw-r--r--   0        0        0   148766 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.data.json
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.meta.json
--rw-r--r--   0        0        0    30709 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_testing/__init__.data.json
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/_testing/__init__.meta.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/__init__.meta.json
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/extensions/__init__.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/extensions/__init__.meta.json
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/indexers/__init__.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/indexers/__init__.meta.json
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/types/__init__.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/api/types/__init__.meta.json
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/arrays/__init__.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/arrays/__init__.meta.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/__init__.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/__init__.meta.json
--rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/accessor.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/accessor.meta.json
--rw-r--r--   0        0        0    30009 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/algorithms.data.json
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/algorithms.meta.json
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/api.data.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/api.meta.json
--rw-r--r--   0        0        0    37419 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arraylike.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arraylike.meta.json
--rw-r--r--   0        0        0    36633 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/base.data.json
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/base.meta.json
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/construction.data.json
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/construction.meta.json
--rw-r--r--   0        0        0   636494 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/frame.data.json
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/frame.meta.json
--rw-r--r--   0        0        0   125208 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/generic.data.json
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/generic.meta.json
--rw-r--r--   0        0        0    18226 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexers.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexers.meta.json
--rw-r--r--   0        0        0    26405 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexing.data.json
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexing.meta.json
--rw-r--r--   0        0        0    90504 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/resample.data.json
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/resample.meta.json
--rw-r--r--   0        0        0  1275823 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/series.data.json
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/series.meta.json
--rw-r--r--   0        0        0   130213 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/strings.data.json
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/strings.meta.json
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/__init__.data.json
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/__init__.meta.json
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow.meta.json
--rw-r--r--   0        0        0    33018 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/base.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/base.meta.json
--rw-r--r--   0        0        0    12401 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/boolean.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/boolean.meta.json
--rw-r--r--   0        0        0   102698 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/categorical.data.json
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/categorical.meta.json
--rw-r--r--   0        0        0    39620 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimelike.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimelike.meta.json
--rw-r--r--   0        0        0    27640 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimes.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimes.meta.json
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/floating.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/floating.meta.json
--rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/integer.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/integer.meta.json
--rw-r--r--   0        0        0    39175 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/interval.data.json
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/interval.meta.json
--rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/masked.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/masked.meta.json
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numeric.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numeric.meta.json
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numpy_.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numpy_.meta.json
--rw-r--r--   0        0        0    18332 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/period.data.json
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/period.meta.json
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/string_.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/string_.meta.json
--rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/timedeltas.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/timedeltas.meta.json
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.meta.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.meta.json
--rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.meta.json
--rw-r--r--   0        0        0    32253 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/array.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/array.meta.json
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.data.json
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.meta.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/__init__.meta.json
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/api.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/api.meta.json
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/eval.data.json
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/eval.meta.json
--rw-r--r--   0        0        0    23609 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/expr.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/expr.meta.json
--rw-r--r--   0        0        0    44801 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/ops.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/ops.meta.json
--rw-r--r--   0        0        0    43699 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/pytables.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/pytables.meta.json
--rw-r--r--   0        0        0    11682 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/scope.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/scope.meta.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/__init__.data.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/__init__.meta.json
--rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/api.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/api.meta.json
--rw-r--r--   0        0        0    14799 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/base.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/base.meta.json
--rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/common.data.json
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/common.meta.json
--rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/concat.data.json
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/concat.meta.json
--rw-r--r--   0        0        0    24363 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/dtypes.data.json
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/dtypes.meta.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/generic.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/generic.meta.json
--rw-r--r--   0        0        0    11384 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/inference.data.json
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/inference.meta.json
--rw-r--r--   0        0        0    22579 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/missing.data.json
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/missing.meta.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/__init__.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/__init__.meta.json
--rw-r--r--   0        0        0   245511 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/generic.data.json
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/generic.meta.json
--rw-r--r--   0        0        0    59252 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/groupby.data.json
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/groupby.meta.json
--rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/grouper.data.json
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/grouper.meta.json
--rw-r--r--   0        0        0    41348 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/ops.data.json
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/ops.meta.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/__init__.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/__init__.meta.json
--rw-r--r--   0        0        0   252673 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/accessors.data.json
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/accessors.meta.json
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/api.data.json
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/api.meta.json
--rw-r--r--   0        0        0   145219 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/base.data.json
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/base.meta.json
--rw-r--r--   0        0        0    20215 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/category.data.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/category.meta.json
--rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimelike.data.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimelike.meta.json
--rw-r--r--   0        0        0    39507 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimes.data.json
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimes.meta.json
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/extension.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/extension.meta.json
--rw-r--r--   0        0        0   201220 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/interval.data.json
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/interval.meta.json
--rw-r--r--   0        0        0    64788 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/multi.data.json
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/multi.meta.json
--rw-r--r--   0        0        0    32074 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/period.data.json
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/period.meta.json
--rw-r--r--   0        0        0    34018 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/range.data.json
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/range.meta.json
--rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/timedeltas.data.json
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/timedeltas.meta.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/__init__.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/__init__.meta.json
--rw-r--r--   0        0        0    56107 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.meta.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/__init__.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/__init__.meta.json
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/api.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/api.meta.json
--rw-r--r--   0        0        0    22894 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/concat.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/concat.meta.json
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/encoding.data.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/encoding.meta.json
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/melt.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/melt.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/merge.data.json
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/merge.meta.json
--rw-r--r--   0        0        0    40852 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/pivot.data.json
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/pivot.meta.json
--rw-r--r--   0        0        0    79047 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/tile.data.json
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/tile.meta.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/__init__.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/__init__.meta.json
--rw-r--r--   0        0        0    19830 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/datetimes.data.json
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/datetimes.meta.json
--rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/numeric.data.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/numeric.meta.json
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/timedeltas.data.json
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/timedeltas.meta.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/__init__.data.json
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/__init__.meta.json
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/hashing.data.json
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/hashing.meta.json
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/__init__.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/__init__.meta.json
--rw-r--r--   0        0        0    22745 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/ewm.data.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/ewm.meta.json
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/expanding.data.json
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/expanding.meta.json
--rw-r--r--   0        0        0    66490 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/rolling.data.json
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/rolling.meta.json
--rw-r--r--   0        0        0    29402 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/errors/__init__.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/errors/__init__.meta.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/__init__.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/__init__.meta.json
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/api.data.json
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/api.meta.json
--rw-r--r--   0        0        0    51839 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/clipboards.data.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/clipboards.meta.json
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/common.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/common.meta.json
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/feather_format.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/feather_format.meta.json
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/gbq.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/gbq.meta.json
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/html.data.json
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/html.meta.json
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/orc.data.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/orc.meta.json
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/parquet.data.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/parquet.meta.json
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/pickle.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/pickle.meta.json
--rw-r--r--   0        0        0    57844 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/pytables.data.json
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/pytables.meta.json
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/spss.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/spss.meta.json
--rw-r--r--   0        0        0    43579 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sql.data.json
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sql.meta.json
--rw-r--r--   0        0        0    32903 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/stata.data.json
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/stata.meta.json
--rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/xml.data.json
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/xml.meta.json
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/__init__.meta.json
--rw-r--r--   0        0        0    79643 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/_base.data.json
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/_base.meta.json
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/__init__.data.json
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/__init__.meta.json
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/format.meta.json
--rw-r--r--   0        0        0    80751 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style.data.json
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style.meta.json
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style_render.data.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style_render.meta.json
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/__init__.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/__init__.meta.json
--rw-r--r--   0        0        0    39700 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_json.data.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_json.meta.json
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_normalize.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_normalize.meta.json
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_table_schema.data.json
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_table_schema.meta.json
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/__init__.data.json
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/__init__.meta.json
--rw-r--r--   0        0        0   135774 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/readers.data.json
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/readers.meta.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/__init__.meta.json
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas7bdat.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas7bdat.meta.json
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas_xport.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas_xport.meta.json
--rw-r--r--   0        0        0    26707 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sasreader.data.json
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sasreader.meta.json
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/__init__.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/__init__.meta.json
--rw-r--r--   0        0        0   150951 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_core.data.json
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_core.meta.json
--rw-r--r--   0        0        0    18244 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_misc.data.json
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_misc.meta.json
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/__init__.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/__init__.meta.json
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/api.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/api.meta.json
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/frequencies.data.json
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/frequencies.meta.json
--rw-r--r--   0        0        0    36704 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/holiday.data.json
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/holiday.meta.json
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/offsets.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/offsets.meta.json
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/__init__.meta.json
--rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/_decorators.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/_decorators.meta.json
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/_print_versions.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/_print_versions.meta.json
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/_tester.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/pandas/util/_tester.meta.json
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sqlite3/__init__.data.json
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sqlite3/__init__.meta.json
--rw-r--r--   0        0        0   165256 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sqlite3/dbapi2.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/sqlite3/dbapi2.meta.json
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/tests/__init__.data.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/tests/__init__.meta.json
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/tests/consistency_test.data.json
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/tests/consistency_test.meta.json
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/tests/test_thzools.data.json
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/tests/test_thzools.meta.json
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/__about__.data.json
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/__about__.meta.json
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/__init__.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/__init__.meta.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/_util.data.json
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/_util.meta.json
--rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/thztools.data.json
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/thztools/thztools.meta.json
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/__init__.data.json
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/__init__.meta.json
--rw-r--r--   0        0        0    24112 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/_log.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/_log.meta.json
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/async_case.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/async_case.meta.json
--rw-r--r--   0        0        0   210198 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/case.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/case.meta.json
--rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/loader.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/loader.meta.json
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/main.data.json
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/main.meta.json
--rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/result.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/result.meta.json
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/runner.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/runner.meta.json
--rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/signals.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/signals.meta.json
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/suite.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 thztools-0.0.1/.mypy_cache/3.11/unittest/suite.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    59137 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/14f6e2943b324e9
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/19eb4dc3198b7596
--rw-r--r--   0        0        0    24586 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/1a47944f2ee50e57
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/21d7d90f768e061d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/2489146c9c65f567
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/25a23a381adbd7dc
--rw-r--r--   0        0        0    12600 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/27ac16db57cce60b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/2ac966be8abee2ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/36a1a17650d2dfa1
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/3d63d95d98e94a84
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/3f80f26e48fff3b9
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/416d77137606cbda
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/4448948485c70ed1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/46e2ada7eb15b40c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/548cc228a53b18a5
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/56b969a195ceb5bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/570264bdcf8403c5
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/587f16d197c00560
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/5e59e90f4a6610ae
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/5ff7b770a0424a48
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/6d641745ea6797b
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/6f15fce0c98cc954
--rw-r--r--   0        0        0    37978 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/6f1765f8409e0c71
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/70343190c55d1467
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/72ab51576de41248
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/7699f8385d3e8ad9
--rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/780a098b6a97fc9e
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/7deb5a6d9d02374
--rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/7e14ee9fb2ba88af
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/80828fea9567907b
--rw-r--r--   0        0        0    30580 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/89753c64299c4c16
--rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/8a285058467be843
--rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/8c06aade77eca546
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/8d40ef997999e5c0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/8e8b5a7a2416699
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/8f3375e559447e11
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/90c0976f06937b1a
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/946677cfaae5d078
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/95ff3cbdf9c9c4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/96f9a668fe5ce99
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/9faaf717898e7034
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/a24306571d8d9be7
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/a8022447c114b8da
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/ab14541dc83065aa
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/abf48d11c0afd9ef
--rw-r--r--   0        0        0    30352 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/ac982820098a0c6b
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/ad867f0bb8f9c9dc
--rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/ad90ede8303e1447
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/aef044181d2d5de7
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/b0448d2cb1c22a2e
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/b70dc04ea668b378
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/bac347fb4506c042
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/bacc2bb0dfbb7db1
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/bf063c6ce36565c
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/bf6f8221e6c1c812
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/c068bcc1830cc02
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/c2fae3237f5f1a4a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/c56e095cdea1456a
--rw-r--r--   0        0        0    30524 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/c753ff9e605d5bb8
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/ceb8a922afdc37f4
--rw-r--r--   0        0        0    67766 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/d2551b373b0a40ff
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/da5cccbe0375db71
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/db6089938babdddb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/e14a2a99e27ee9d0
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/e3874541bd014547
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/e46c2b97b92a413c
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/eb52cda4d1bf1d50
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/ec89cb2438d79a93
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/f556c70333c5b8f9
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/fa6062adf3c39eac
--rw-r--r--   0        0        0    30523 2020-02-02 00:00:00.000000 thztools-0.0.1/.ruff_cache/content/fb453ce093001723
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 thztools-0.0.1/envs/environment-dev.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.0.1/src/thztools/__about__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 thztools-0.0.1/src/thztools/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 thztools-0.0.1/src/thztools/_util.py
--rw-r--r--   0        0        0    29977 2020-02-02 00:00:00.000000 thztools-0.0.1/src/thztools/thztools.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 thztools-0.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.0.1/LICENSE
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 thztools-0.0.1/README.md
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 thztools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 thztools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 thztools-0.0.2/.DS_Store
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 thztools-0.0.2/.gitattributes
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/other.xml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/thztools.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 thztools-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180412 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52444 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18271 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0    19674 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_csv.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_csv.meta.json
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    23905 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13122 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    23380 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60720 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0   137664 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ast.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ast.meta.json
+-rw-r--r--   0        0        0  1130456 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123361 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109248 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0    29692 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/csv.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/csv.meta.json
+-rw-r--r--   0        0        0    57789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142252 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0    90167 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0   132111 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22432 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0    85381 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    52555 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    87532 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44437 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75241 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   167589 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    14417 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28524 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49785 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0    27792 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   162208 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0    19597 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64759 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    42853 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0   239676 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432278 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57889 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    23833 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0    75677 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/zipfile.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/zipfile.meta.json
+-rw-r--r--   0        0        0    89098 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   408032 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   129027 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12244 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7293 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25117 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79314 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30901 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70623 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64615 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91163 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    15423 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/__init__.meta.json
+-rw-r--r--   0        0        0    14548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/decoder.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/decoder.meta.json
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/encoder.data.json
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/json/encoder.meta.json
+-rw-r--r--   0        0        0   144429 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/logging/__init__.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/logging/__init__.meta.json
+-rw-r--r--   0        0        0  2217665 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/__init__.data.json
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/__init__.meta.json
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_pytesttester.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_pytesttester.meta.json
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_version.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_version.meta.json
+-rw-r--r--   0        0        0   112541 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ctypeslib.data.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ctypeslib.meta.json
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/version.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/version.meta.json
+-rw-r--r--   0        0        0    21388 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/__init__.data.json
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/__init__.meta.json
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json
+-rw-r--r--   0        0        0    25436 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_array_like.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json
+-rw-r--r--   0        0        0   256912 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_callable.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_callable.meta.json
+-rw-r--r--   0        0        0    41750 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json
+-rw-r--r--   0        0        0    30730 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json
+-rw-r--r--   0        0        0    34767 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nbit.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json
+-rw-r--r--   0        0        0    16797 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_scalars.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_shape.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_shape.meta.json
+-rw-r--r--   0        0        0   261391 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/__init__.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/__init__.meta.json
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/_inspect.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/_inspect.meta.json
+-rw-r--r--   0        0        0    11827 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/py3k.data.json
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/compat/py3k.meta.json
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/__init__.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/__init__.meta.json
+-rw-r--r--   0        0        0    13683 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_asarray.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_asarray.meta.json
+-rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_internal.data.json
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_internal.meta.json
+-rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_type_aliases.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json
+-rw-r--r--   0        0        0    11255 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json
+-rw-r--r--   0        0        0    28038 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/arrayprint.data.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/arrayprint.meta.json
+-rw-r--r--   0        0        0   169698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/defchararray.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/defchararray.meta.json
+-rw-r--r--   0        0        0    36087 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/einsumfunc.data.json
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json
+-rw-r--r--   0        0        0   330727 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/fromnumeric.data.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json
+-rw-r--r--   0        0        0    49588 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/function_base.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/function_base.meta.json
+-rw-r--r--   0        0        0   301784 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/multiarray.data.json
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/multiarray.meta.json
+-rw-r--r--   0        0        0   196469 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numeric.data.json
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numeric.meta.json
+-rw-r--r--   0        0        0    44548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numerictypes.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/numerictypes.meta.json
+-rw-r--r--   0        0        0    25179 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/overrides.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/overrides.meta.json
+-rw-r--r--   0        0        0    52653 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/records.data.json
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/records.meta.json
+-rw-r--r--   0        0        0    52786 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/shape_base.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/shape_base.meta.json
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/umath.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/core/umath.meta.json
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/__init__.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/__init__.meta.json
+-rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json
+-rw-r--r--   0        0        0    21751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/helper.data.json
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/fft/helper.meta.json
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/__init__.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/__init__.meta.json
+-rw-r--r--   0        0        0   107815 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/linalg.data.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/linalg.meta.json
+-rw-r--r--   0        0        0    27705 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/__init__.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/__init__.meta.json
+-rw-r--r--   0        0        0   136790 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/core.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/core.meta.json
+-rw-r--r--   0        0        0    23356 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/extras.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/extras.meta.json
+-rw-r--r--   0        0        0    14308 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/mrecords.data.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/ma/mrecords.meta.json
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/__init__.data.json
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json
+-rw-r--r--   0        0        0    27027 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json
+-rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json
+-rw-r--r--   0        0        0    14216 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite.data.json
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json
+-rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/legendre.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json
+-rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/__init__.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/__init__.meta.json
+-rw-r--r--   0        0        0   252832 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_generator.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_generator.meta.json
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_mt19937.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_mt19937.meta.json
+-rw-r--r--   0        0        0    15496 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_pcg64.data.json
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_pcg64.meta.json
+-rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_philox.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_philox.meta.json
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_sfc64.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/_sfc64.meta.json
+-rw-r--r--   0        0        0    67750 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/bit_generator.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/bit_generator.meta.json
+-rw-r--r--   0        0        0   323551 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/mtrand.data.json
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/random/mtrand.meta.json
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/__init__.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/__init__.meta.json
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json
+-rw-r--r--   0        0        0   114237 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/utils.data.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/typing/__init__.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/numpy/typing/__init__.meta.json
+-rw-r--r--   0        0        0   322665 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/__init__.data.json
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/__init__.meta.json
+-rw-r--r--   0        0        0   100879 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_typing.data.json
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_typing.meta.json
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/testing.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/testing.meta.json
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/__init__.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/__init__.meta.json
+-rw-r--r--   0        0        0    56793 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/config.data.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_config/config.meta.json
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/__init__.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/__init__.meta.json
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/indexing.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/indexing.meta.json
+-rw-r--r--   0        0        0   175959 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/interval.data.json
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/interval.meta.json
+-rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/lib.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/lib.meta.json
+-rw-r--r--   0        0        0    31747 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/missing.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/missing.meta.json
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/ops_dispatch.data.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/ops_dispatch.meta.json
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/properties.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/properties.meta.json
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.meta.json
+-rw-r--r--   0        0        0    58580 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.meta.json
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.meta.json
+-rw-r--r--   0        0        0   125210 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.data.json
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.meta.json
+-rw-r--r--   0        0        0    92339 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/period.data.json
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/period.meta.json
+-rw-r--r--   0        0        0   190061 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.data.json
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.meta.json
+-rw-r--r--   0        0        0   148766 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.data.json
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.meta.json
+-rw-r--r--   0        0        0    30709 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_testing/__init__.data.json
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/_testing/__init__.meta.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/__init__.data.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/__init__.meta.json
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/extensions/__init__.data.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/extensions/__init__.meta.json
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/indexers/__init__.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/indexers/__init__.meta.json
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/types/__init__.data.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/api/types/__init__.meta.json
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/arrays/__init__.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/arrays/__init__.meta.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/__init__.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/__init__.meta.json
+-rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/accessor.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/accessor.meta.json
+-rw-r--r--   0        0        0    30009 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/algorithms.data.json
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/algorithms.meta.json
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/api.data.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/api.meta.json
+-rw-r--r--   0        0        0    37419 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arraylike.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arraylike.meta.json
+-rw-r--r--   0        0        0    36633 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/base.data.json
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/base.meta.json
+-rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/construction.data.json
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/construction.meta.json
+-rw-r--r--   0        0        0   636494 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/frame.data.json
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/frame.meta.json
+-rw-r--r--   0        0        0   125208 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/generic.data.json
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/generic.meta.json
+-rw-r--r--   0        0        0    18226 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexers.data.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexers.meta.json
+-rw-r--r--   0        0        0    26405 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexing.data.json
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexing.meta.json
+-rw-r--r--   0        0        0    90504 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/resample.data.json
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/resample.meta.json
+-rw-r--r--   0        0        0  1275823 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/series.data.json
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/series.meta.json
+-rw-r--r--   0        0        0   130213 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/strings.data.json
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/strings.meta.json
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/__init__.data.json
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/__init__.meta.json
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow.data.json
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow.meta.json
+-rw-r--r--   0        0        0    33018 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/base.data.json
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/base.meta.json
+-rw-r--r--   0        0        0    12401 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/boolean.data.json
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/boolean.meta.json
+-rw-r--r--   0        0        0   102698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/categorical.data.json
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/categorical.meta.json
+-rw-r--r--   0        0        0    39620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimelike.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimelike.meta.json
+-rw-r--r--   0        0        0    27640 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimes.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimes.meta.json
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/floating.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/floating.meta.json
+-rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/integer.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/integer.meta.json
+-rw-r--r--   0        0        0    39175 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/interval.data.json
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/interval.meta.json
+-rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/masked.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/masked.meta.json
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numeric.data.json
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numeric.meta.json
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numpy_.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numpy_.meta.json
+-rw-r--r--   0        0        0    18332 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/period.data.json
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/period.meta.json
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/string_.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/string_.meta.json
+-rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/timedeltas.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/timedeltas.meta.json
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.meta.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.data.json
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.meta.json
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.data.json
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.meta.json
+-rw-r--r--   0        0        0    32253 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/array.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/array.meta.json
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.data.json
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.meta.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/__init__.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/__init__.meta.json
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/api.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/api.meta.json
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/eval.data.json
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/eval.meta.json
+-rw-r--r--   0        0        0    23609 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/expr.data.json
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/expr.meta.json
+-rw-r--r--   0        0        0    44801 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/ops.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/ops.meta.json
+-rw-r--r--   0        0        0    43699 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/pytables.data.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/pytables.meta.json
+-rw-r--r--   0        0        0    11682 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/scope.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/scope.meta.json
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/__init__.data.json
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/__init__.meta.json
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/api.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/api.meta.json
+-rw-r--r--   0        0        0    14799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/base.data.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/base.meta.json
+-rw-r--r--   0        0        0    21522 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/common.data.json
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/common.meta.json
+-rw-r--r--   0        0        0     4084 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/concat.data.json
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/concat.meta.json
+-rw-r--r--   0        0        0    24363 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/dtypes.data.json
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/dtypes.meta.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/generic.data.json
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/generic.meta.json
+-rw-r--r--   0        0        0    11384 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/inference.data.json
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/inference.meta.json
+-rw-r--r--   0        0        0    22579 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/missing.data.json
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/missing.meta.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/__init__.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/__init__.meta.json
+-rw-r--r--   0        0        0   245511 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/generic.data.json
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/generic.meta.json
+-rw-r--r--   0        0        0    59252 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/groupby.data.json
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/groupby.meta.json
+-rw-r--r--   0        0        0    20973 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/grouper.data.json
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/grouper.meta.json
+-rw-r--r--   0        0        0    41348 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/ops.data.json
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/ops.meta.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/__init__.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/__init__.meta.json
+-rw-r--r--   0        0        0   252673 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/accessors.data.json
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/accessors.meta.json
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/api.data.json
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/api.meta.json
+-rw-r--r--   0        0        0   145219 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/base.data.json
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/base.meta.json
+-rw-r--r--   0        0        0    20215 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/category.data.json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/category.meta.json
+-rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimelike.data.json
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimelike.meta.json
+-rw-r--r--   0        0        0    39507 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimes.data.json
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimes.meta.json
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/extension.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/extension.meta.json
+-rw-r--r--   0        0        0   201220 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/interval.data.json
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/interval.meta.json
+-rw-r--r--   0        0        0    64788 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/multi.data.json
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/multi.meta.json
+-rw-r--r--   0        0        0    32074 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/period.data.json
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/period.meta.json
+-rw-r--r--   0        0        0    34018 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/range.data.json
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/range.meta.json
+-rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/timedeltas.data.json
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/timedeltas.meta.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/__init__.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/__init__.meta.json
+-rw-r--r--   0        0        0    56107 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.meta.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/__init__.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/__init__.meta.json
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/api.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/api.meta.json
+-rw-r--r--   0        0        0    22894 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/concat.data.json
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/concat.meta.json
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/encoding.data.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/encoding.meta.json
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/melt.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/melt.meta.json
+-rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/merge.data.json
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/merge.meta.json
+-rw-r--r--   0        0        0    40852 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/pivot.data.json
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/pivot.meta.json
+-rw-r--r--   0        0        0    79047 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/tile.data.json
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/tile.meta.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/__init__.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/__init__.meta.json
+-rw-r--r--   0        0        0    19830 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/datetimes.data.json
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/datetimes.meta.json
+-rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/numeric.data.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/numeric.meta.json
+-rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/timedeltas.data.json
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/timedeltas.meta.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/__init__.data.json
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/__init__.meta.json
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/hashing.data.json
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/hashing.meta.json
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/__init__.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/__init__.meta.json
+-rw-r--r--   0        0        0    22745 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/ewm.data.json
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/ewm.meta.json
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/expanding.data.json
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/expanding.meta.json
+-rw-r--r--   0        0        0    66490 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/rolling.data.json
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/rolling.meta.json
+-rw-r--r--   0        0        0    29402 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/errors/__init__.data.json
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/errors/__init__.meta.json
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/__init__.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/__init__.meta.json
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/api.data.json
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/api.meta.json
+-rw-r--r--   0        0        0    51839 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/clipboards.data.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/clipboards.meta.json
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/common.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/common.meta.json
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/feather_format.data.json
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/feather_format.meta.json
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/gbq.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/gbq.meta.json
+-rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/html.data.json
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/html.meta.json
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/orc.data.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/orc.meta.json
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parquet.data.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parquet.meta.json
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pickle.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pickle.meta.json
+-rw-r--r--   0        0        0    57844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pytables.data.json
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/pytables.meta.json
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/spss.data.json
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/spss.meta.json
+-rw-r--r--   0        0        0    43579 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sql.data.json
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sql.meta.json
+-rw-r--r--   0        0        0    32903 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/stata.data.json
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/stata.meta.json
+-rw-r--r--   0        0        0     6049 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/xml.data.json
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/xml.meta.json
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/__init__.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/__init__.meta.json
+-rw-r--r--   0        0        0    79643 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/_base.data.json
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/_base.meta.json
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/__init__.data.json
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/__init__.meta.json
+-rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/format.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/format.meta.json
+-rw-r--r--   0        0        0    80751 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style.data.json
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style.meta.json
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style_render.data.json
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style_render.meta.json
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/__init__.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/__init__.meta.json
+-rw-r--r--   0        0        0    39700 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_json.data.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_json.meta.json
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_normalize.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_normalize.meta.json
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_table_schema.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_table_schema.meta.json
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/__init__.data.json
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/__init__.meta.json
+-rw-r--r--   0        0        0   135774 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/readers.data.json
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/readers.meta.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/__init__.meta.json
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas7bdat.data.json
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas7bdat.meta.json
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas_xport.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas_xport.meta.json
+-rw-r--r--   0        0        0    26707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sasreader.data.json
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sasreader.meta.json
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/__init__.data.json
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/__init__.meta.json
+-rw-r--r--   0        0        0   150951 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_core.data.json
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_core.meta.json
+-rw-r--r--   0        0        0    18244 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_misc.data.json
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_misc.meta.json
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/__init__.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/__init__.meta.json
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/api.data.json
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/api.meta.json
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/frequencies.data.json
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/frequencies.meta.json
+-rw-r--r--   0        0        0    36704 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/holiday.data.json
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/holiday.meta.json
+-rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/offsets.data.json
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/offsets.meta.json
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/__init__.data.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/__init__.meta.json
+-rw-r--r--   0        0        0    18351 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_decorators.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_decorators.meta.json
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_print_versions.data.json
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_print_versions.meta.json
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_tester.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/pandas/util/_tester.meta.json
+-rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/__init__.data.json
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/__init__.meta.json
+-rw-r--r--   0        0        0   165256 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/dbapi2.data.json
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/sqlite3/dbapi2.meta.json
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/__init__.data.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/__init__.meta.json
+-rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/consistency_test.data.json
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/consistency_test.meta.json
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/test_thzools.data.json
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/tests/test_thzools.meta.json
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__about__.data.json
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__about__.meta.json
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__init__.data.json
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/__init__.meta.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/_util.data.json
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/_util.meta.json
+-rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/thztools.data.json
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/thztools/thztools.meta.json
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/__init__.data.json
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/__init__.meta.json
+-rw-r--r--   0        0        0    24112 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/_log.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/_log.meta.json
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/async_case.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/async_case.meta.json
+-rw-r--r--   0        0        0   210198 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/case.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/case.meta.json
+-rw-r--r--   0        0        0    14662 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/loader.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/loader.meta.json
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/main.data.json
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/main.meta.json
+-rw-r--r--   0        0        0    20622 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/result.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/result.meta.json
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/runner.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/runner.meta.json
+-rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/signals.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/signals.meta.json
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/suite.data.json
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 thztools-0.0.2/.mypy_cache/3.11/unittest/suite.meta.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    59137 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/14f6e2943b324e9
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/19eb4dc3198b7596
+-rw-r--r--   0        0        0    24586 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/1a47944f2ee50e57
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/21d7d90f768e061d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/2489146c9c65f567
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/25a23a381adbd7dc
+-rw-r--r--   0        0        0    12600 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/27ac16db57cce60b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/2ac966be8abee2ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/36a1a17650d2dfa1
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/3d63d95d98e94a84
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/3f80f26e48fff3b9
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/416d77137606cbda
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/4448948485c70ed1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/46e2ada7eb15b40c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/548cc228a53b18a5
+-rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/56b969a195ceb5bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/570264bdcf8403c5
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/587f16d197c00560
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/5e59e90f4a6610ae
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/5ff7b770a0424a48
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/6d641745ea6797b
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/6f15fce0c98cc954
+-rw-r--r--   0        0        0    37978 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/6f1765f8409e0c71
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/70343190c55d1467
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/72ab51576de41248
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/7699f8385d3e8ad9
+-rw-r--r--   0        0        0    16606 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/780a098b6a97fc9e
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/7deb5a6d9d02374
+-rw-r--r--   0        0        0    15601 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/7e14ee9fb2ba88af
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/80828fea9567907b
+-rw-r--r--   0        0        0    30580 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/89753c64299c4c16
+-rw-r--r--   0        0        0    30392 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8a285058467be843
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8c06aade77eca546
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8d40ef997999e5c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8e8b5a7a2416699
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/8f3375e559447e11
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/90c0976f06937b1a
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/946677cfaae5d078
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/95ff3cbdf9c9c4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/96f9a668fe5ce99
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/9faaf717898e7034
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/a24306571d8d9be7
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/a8022447c114b8da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ab14541dc83065aa
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/abf48d11c0afd9ef
+-rw-r--r--   0        0        0    30352 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ac982820098a0c6b
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ad867f0bb8f9c9dc
+-rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ad90ede8303e1447
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/aef044181d2d5de7
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/b0448d2cb1c22a2e
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/b70dc04ea668b378
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bac347fb4506c042
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bacc2bb0dfbb7db1
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bf063c6ce36565c
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/bf6f8221e6c1c812
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c068bcc1830cc02
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c2fae3237f5f1a4a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c56e095cdea1456a
+-rw-r--r--   0        0        0    30524 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/c753ff9e605d5bb8
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ceb8a922afdc37f4
+-rw-r--r--   0        0        0    67766 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/d2551b373b0a40ff
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/da5cccbe0375db71
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/db6089938babdddb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/e14a2a99e27ee9d0
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/e3874541bd014547
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/e46c2b97b92a413c
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/eb52cda4d1bf1d50
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/ec89cb2438d79a93
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/f556c70333c5b8f9
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/fa6062adf3c39eac
+-rw-r--r--   0        0        0    30523 2020-02-02 00:00:00.000000 thztools-0.0.2/.ruff_cache/content/fb453ce093001723
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 thztools-0.0.2/envs/environment-dev.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/__about__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/_util.py
+-rw-r--r--   0        0        0    28925 2020-02-02 00:00:00.000000 thztools-0.0.2/src/thztools/thztools.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 thztools-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 thztools-0.0.2/README.md
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 thztools-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 thztools-0.0.2/PKG-INFO
```

### Comparing `thztools-0.0.1/.DS_Store` & `thztools-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.idea/thztools.iml` & `thztools-0.0.2/.idea/thztools.iml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `thztools-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/__future__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/__future__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_ast.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_ast.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_codecs.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_codecs.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_collections_abc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_collections_abc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_csv.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_csv.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_csv.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_csv.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_ctypes.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_ctypes.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_thread.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_thread.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_thread.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_warnings.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_warnings.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_warnings.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/abc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/abc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/array.data.json` & `thztools-0.0.2/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/array.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/ast.data.json` & `thztools-0.0.2/.mypy_cache/3.11/ast.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/ast.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/ast.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/builtins.data.json` & `thztools-0.0.2/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/builtins.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/codecs.data.json` & `thztools-0.0.2/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/codecs.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/contextlib.data.json` & `thztools-0.0.2/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/contextlib.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/csv.data.json` & `thztools-0.0.2/.mypy_cache/3.11/csv.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/csv.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/csv.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/dataclasses.data.json` & `thztools-0.0.2/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/dataclasses.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/datetime.data.json` & `thztools-0.0.2/.mypy_cache/3.11/datetime.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/datetime.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/datetime.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/enum.data.json` & `thztools-0.0.2/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/enum.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/functools.data.json` & `thztools-0.0.2/.mypy_cache/3.11/functools.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/functools.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/functools.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/genericpath.data.json` & `thztools-0.0.2/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/genericpath.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/io.data.json` & `thztools-0.0.2/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/io.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/math.data.json` & `thztools-0.0.2/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/math.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/math.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/mmap.data.json` & `thztools-0.0.2/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/mmap.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pathlib.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pathlib.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pickle.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pickle.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/posixpath.data.json` & `thztools-0.0.2/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/posixpath.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/re.data.json` & `thztools-0.0.2/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/re.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sre_compile.data.json` & `thztools-0.0.2/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sre_compile.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sre_constants.data.json` & `thztools-0.0.2/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sre_constants.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sre_parse.data.json` & `thztools-0.0.2/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sre_parse.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/string.data.json` & `thztools-0.0.2/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/string.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/string.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/subprocess.data.json` & `thztools-0.0.2/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/subprocess.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sys.data.json` & `thztools-0.0.2/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sys.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/textwrap.data.json` & `thztools-0.0.2/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/textwrap.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/textwrap.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/threading.data.json` & `thztools-0.0.2/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/threading.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/threading.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/time.data.json` & `thztools-0.0.2/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/time.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/time.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/types.data.json` & `thztools-0.0.2/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/types.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/typing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/typing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/typing_extensions.data.json` & `thztools-0.0.2/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/typing_extensions.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/warnings.data.json` & `thztools-0.0.2/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/warnings.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/warnings.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/zipfile.data.json` & `thztools-0.0.2/.mypy_cache/3.11/zipfile.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/zipfile.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/zipfile.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/collections/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/collections/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/collections/abc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/collections/abc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/ctypes/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/charset.data.json` & `thztools-0.0.2/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/charset.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/contentmanager.data.json` & `thztools-0.0.2/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/contentmanager.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/errors.data.json` & `thztools-0.0.2/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/errors.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/header.data.json` & `thztools-0.0.2/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/header.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/message.data.json` & `thztools-0.0.2/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/message.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/policy.data.json` & `thztools-0.0.2/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/email/policy.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/abc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/abc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/machinery.data.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/machinery.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/json/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/json/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/json/decoder.data.json` & `thztools-0.0.2/.mypy_cache/3.11/json/decoder.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/json/decoder.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/json/decoder.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/json/encoder.data.json` & `thztools-0.0.2/.mypy_cache/3.11/json/encoder.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/json/encoder.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/json/encoder.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/logging/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/logging/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/logging/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/logging/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_pytesttester.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_pytesttester.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_pytesttester.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_pytesttester.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_version.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_version.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_version.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_version.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ctypeslib.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ctypeslib.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ctypeslib.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ctypeslib.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/version.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/version.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/version.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/version.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_add_docstring.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_add_docstring.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_array_like.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_array_like.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_array_like.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_callable.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_callable.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_callable.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_callable.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_char_codes.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_char_codes.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_dtype_like.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_dtype_like.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_extended_precision.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_extended_precision.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_generic_alias.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_generic_alias.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nbit.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nbit.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nbit.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nested_sequence.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_nested_sequence.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_scalars.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_scalars.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_scalars.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_shape.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_shape.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_shape.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_shape.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_ufunc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/_typing/_ufunc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/compat/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/compat/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/compat/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/compat/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/compat/_inspect.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/compat/_inspect.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/compat/_inspect.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/compat/_inspect.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/compat/py3k.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/compat/py3k.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/compat/py3k.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/compat/py3k.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_asarray.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_asarray.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_asarray.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_asarray.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_internal.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_internal.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_internal.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_internal.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_type_aliases.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_type_aliases.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_type_aliases.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_ufunc_config.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/_ufunc_config.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/arrayprint.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/arrayprint.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/arrayprint.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/arrayprint.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/defchararray.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/defchararray.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/defchararray.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/defchararray.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/einsumfunc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/einsumfunc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/einsumfunc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/fromnumeric.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/fromnumeric.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/fromnumeric.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/function_base.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/function_base.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/function_base.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/function_base.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/multiarray.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/multiarray.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/multiarray.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/multiarray.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/numeric.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/numeric.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/numeric.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/numerictypes.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/numerictypes.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/numerictypes.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/numerictypes.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/overrides.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/overrides.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/overrides.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/overrides.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/records.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/records.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/records.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/records.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/shape_base.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/shape_base.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/shape_base.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/shape_base.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/umath.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/umath.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/core/umath.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/core/umath.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/fft/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/fft/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/fft/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/fft/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/fft/_pocketfft.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/fft/_pocketfft.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/fft/helper.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/fft/helper.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/fft/helper.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/fft/helper.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/linalg.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/linalg.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/linalg/linalg.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/linalg/linalg.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/core.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/core.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/core.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/core.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/extras.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/extras.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/extras.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/extras.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/mrecords.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/mrecords.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/ma/mrecords.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/ma/mrecords.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/defmatrix.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/matrixlib/defmatrix.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/_polybase.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/_polybase.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/chebyshev.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/chebyshev.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite_e.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/hermite_e.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/laguerre.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/laguerre.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/legendre.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/legendre.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/legendre.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polynomial.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polynomial.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polyutils.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/polynomial/polyutils.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_generator.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_generator.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_generator.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_generator.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_mt19937.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_mt19937.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_mt19937.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_mt19937.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_pcg64.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_pcg64.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_pcg64.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_pcg64.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_philox.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_philox.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_philox.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_philox.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_sfc64.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_sfc64.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/_sfc64.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/_sfc64.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/bit_generator.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/bit_generator.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/bit_generator.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/bit_generator.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/mtrand.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/mtrand.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/random/mtrand.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/random/mtrand.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/testing/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/testing/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/utils.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/utils.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/testing/_private/utils.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/typing/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/numpy/typing/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/numpy/typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/os/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/os/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/os/path.data.json` & `thztools-0.0.2/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/os/path.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_typing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_typing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_typing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_typing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/testing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/testing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/testing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/testing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_config/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_config/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_config/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_config/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_config/config.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_config/config.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_config/config.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_config/config.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/indexing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/indexing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/indexing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/indexing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/interval.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/interval.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/interval.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/interval.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/lib.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/lib.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/lib.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/lib.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/missing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/missing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/missing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/missing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/ops_dispatch.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/ops_dispatch.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/ops_dispatch.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/ops_dispatch.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/properties.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/properties.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/properties.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/properties.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/nattype.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/np_datetime.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/offsets.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/period.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/period.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/period.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/period.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_libs/tslibs/timestamps.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_testing/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_testing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/_testing/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/_testing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/extensions/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/extensions/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/extensions/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/extensions/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/indexers/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/indexers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/indexers/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/indexers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/types/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/types/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/api/types/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/api/types/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/arrays/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/arrays/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/arrays/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/arrays/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/accessor.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/accessor.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/accessor.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/accessor.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/algorithms.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/algorithms.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/algorithms.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/algorithms.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/api.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/api.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/api.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/api.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arraylike.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arraylike.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arraylike.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arraylike.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/base.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/base.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/base.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/base.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/construction.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/construction.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/construction.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/construction.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/frame.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/frame.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/frame.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/frame.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/generic.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/generic.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/generic.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/generic.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexers.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexers.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexers.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexers.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/resample.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/resample.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/resample.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/resample.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/series.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/series.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/series.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/series.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/strings.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/strings.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/strings.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/strings.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/base.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/base.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/base.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/base.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/boolean.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/boolean.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/boolean.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/boolean.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/categorical.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/categorical.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/categorical.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/categorical.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimelike.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimelike.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimelike.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimelike.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimes.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimes.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/datetimes.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/datetimes.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/floating.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/floating.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/floating.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/floating.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/integer.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/integer.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/integer.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/integer.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/interval.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/interval.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/interval.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/interval.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/masked.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/masked.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/masked.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/masked.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numeric.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numeric.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numeric.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numpy_.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numpy_.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/numpy_.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/numpy_.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/period.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/period.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/period.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/period.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/string_.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/string_.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/string_.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/string_.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/timedeltas.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/timedeltas.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/arrow/dtype.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/accessor.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/array.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/array.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/array.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/array.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/arrays/sparse/dtype.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/api.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/api.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/api.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/api.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/eval.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/eval.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/eval.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/eval.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/expr.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/expr.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/expr.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/expr.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/ops.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/ops.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/ops.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/ops.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/pytables.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/pytables.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/pytables.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/pytables.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/scope.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/scope.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/computation/scope.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/computation/scope.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/api.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/api.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/api.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/api.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/base.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/base.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/base.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/base.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/common.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/common.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/common.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/common.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/concat.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/concat.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/concat.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/concat.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/dtypes.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/dtypes.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/dtypes.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/dtypes.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/generic.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/generic.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/generic.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/generic.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/inference.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/inference.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/inference.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/inference.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/missing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/missing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/dtypes/missing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/dtypes/missing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/generic.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/generic.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/generic.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/generic.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/groupby.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/groupby.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/groupby.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/groupby.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/grouper.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/grouper.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/grouper.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/grouper.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/ops.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/ops.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/groupby/ops.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/groupby/ops.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/accessors.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/accessors.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/accessors.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/accessors.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/api.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/api.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/api.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/api.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/base.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/base.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/base.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/base.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/category.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/category.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/category.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/category.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimelike.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimelike.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimelike.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimelike.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimes.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimes.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/datetimes.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/datetimes.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/extension.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/extension.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/extension.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/extension.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/interval.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/interval.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/interval.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/interval.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/multi.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/multi.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/multi.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/multi.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/period.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/period.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/period.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/period.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/range.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/range.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/range.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/range.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/timedeltas.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/indexes/timedeltas.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/indexes/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/interchange/dataframe_protocol.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/api.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/api.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/api.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/api.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/concat.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/concat.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/concat.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/concat.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/encoding.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/encoding.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/encoding.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/encoding.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/melt.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/melt.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/melt.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/melt.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/merge.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/merge.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/merge.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/merge.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/pivot.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/pivot.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/pivot.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/pivot.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/tile.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/tile.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/reshape/tile.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/reshape/tile.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/datetimes.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/datetimes.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/datetimes.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/datetimes.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/numeric.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/numeric.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/numeric.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/numeric.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/timedeltas.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/timedeltas.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/tools/timedeltas.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/tools/timedeltas.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/hashing.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/hashing.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/util/hashing.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/util/hashing.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/ewm.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/ewm.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/ewm.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/ewm.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/expanding.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/expanding.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/expanding.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/expanding.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/rolling.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/rolling.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/core/window/rolling.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/core/window/rolling.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/errors/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/errors/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/errors/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/errors/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/api.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/api.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/api.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/api.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/clipboards.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/clipboards.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/clipboards.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/clipboards.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/common.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/common.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/common.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/common.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/feather_format.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/feather_format.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/feather_format.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/feather_format.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/gbq.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/gbq.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/gbq.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/gbq.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/html.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/html.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/html.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/html.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/orc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/orc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/orc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/orc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/parquet.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/parquet.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/parquet.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/parquet.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/pickle.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/pickle.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/pickle.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/pytables.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/pytables.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/pytables.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/pytables.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/spss.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/spss.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/spss.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/spss.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sql.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sql.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sql.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sql.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/stata.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/stata.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/stata.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/stata.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/xml.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/xml.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/xml.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/xml.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/_base.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/_base.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/excel/_base.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/excel/_base.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/format.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/format.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/format.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/format.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style_render.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style_render.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/formats/style_render.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/formats/style_render.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_json.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_json.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_json.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_json.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_normalize.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_normalize.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_normalize.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_normalize.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_table_schema.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_table_schema.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/json/_table_schema.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/json/_table_schema.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/readers.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/readers.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/parsers/readers.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/parsers/readers.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas7bdat.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas7bdat.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas7bdat.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas7bdat.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas_xport.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas_xport.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sas_xport.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sas_xport.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sasreader.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sasreader.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/io/sas/sasreader.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/io/sas/sasreader.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_core.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_core.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_core.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_core.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_misc.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_misc.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/plotting/_misc.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/plotting/_misc.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/api.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/api.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/api.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/api.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/frequencies.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/frequencies.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/frequencies.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/frequencies.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/holiday.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/holiday.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/holiday.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/holiday.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/offsets.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/offsets.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/tseries/offsets.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/tseries/offsets.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/_decorators.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/_decorators.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/_decorators.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/_decorators.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/_print_versions.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/_print_versions.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/_print_versions.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/_print_versions.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/_tester.data.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/_tester.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/pandas/util/_tester.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/pandas/util/_tester.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sqlite3/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/sqlite3/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sqlite3/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/sqlite3/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sqlite3/dbapi2.data.json` & `thztools-0.0.2/.mypy_cache/3.11/sqlite3/dbapi2.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/sqlite3/dbapi2.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/sqlite3/dbapi2.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/tests/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/tests/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/tests/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/tests/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/tests/consistency_test.data.json` & `thztools-0.0.2/.mypy_cache/3.11/tests/consistency_test.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/tests/consistency_test.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/tests/consistency_test.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/tests/test_thzools.data.json` & `thztools-0.0.2/.mypy_cache/3.11/tests/test_thzools.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/tests/test_thzools.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/tests/test_thzools.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/__about__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/__about__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/__about__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/__about__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/_util.data.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/_util.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/_util.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/_util.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/thztools.data.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/thztools.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/thztools/thztools.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/thztools/thztools.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/__init__.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/__init__.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/__init__.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/_log.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/_log.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/_log.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/_log.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/async_case.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/async_case.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/async_case.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/async_case.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/case.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/case.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/case.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/case.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/loader.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/loader.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/loader.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/loader.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/main.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/main.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/main.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/main.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/result.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/result.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/result.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/result.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/runner.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/runner.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/runner.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/runner.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/signals.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/signals.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/signals.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/signals.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/suite.data.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/suite.data.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.mypy_cache/3.11/unittest/suite.meta.json` & `thztools-0.0.2/.mypy_cache/3.11/unittest/suite.meta.json`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/14f6e2943b324e9` & `thztools-0.0.2/.ruff_cache/content/14f6e2943b324e9`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/1a47944f2ee50e57` & `thztools-0.0.2/.ruff_cache/content/1a47944f2ee50e57`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/21d7d90f768e061d` & `thztools-0.0.2/.ruff_cache/content/21d7d90f768e061d`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/27ac16db57cce60b` & `thztools-0.0.2/.ruff_cache/content/27ac16db57cce60b`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/3d63d95d98e94a84` & `thztools-0.0.2/.ruff_cache/content/3d63d95d98e94a84`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/416d77137606cbda` & `thztools-0.0.2/.ruff_cache/content/416d77137606cbda`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/56b969a195ceb5bc` & `thztools-0.0.2/.ruff_cache/content/56b969a195ceb5bc`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/587f16d197c00560` & `thztools-0.0.2/.ruff_cache/content/587f16d197c00560`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/5e59e90f4a6610ae` & `thztools-0.0.2/.ruff_cache/content/5e59e90f4a6610ae`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/5ff7b770a0424a48` & `thztools-0.0.2/.ruff_cache/content/5ff7b770a0424a48`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/6f15fce0c98cc954` & `thztools-0.0.2/.ruff_cache/content/6f15fce0c98cc954`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/6f1765f8409e0c71` & `thztools-0.0.2/.ruff_cache/content/6f1765f8409e0c71`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/780a098b6a97fc9e` & `thztools-0.0.2/.ruff_cache/content/780a098b6a97fc9e`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/7deb5a6d9d02374` & `thztools-0.0.2/.ruff_cache/content/7deb5a6d9d02374`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/7e14ee9fb2ba88af` & `thztools-0.0.2/.ruff_cache/content/7e14ee9fb2ba88af`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/89753c64299c4c16` & `thztools-0.0.2/.ruff_cache/content/89753c64299c4c16`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/8a285058467be843` & `thztools-0.0.2/.ruff_cache/content/8a285058467be843`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/8c06aade77eca546` & `thztools-0.0.2/.ruff_cache/content/8c06aade77eca546`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/8f3375e559447e11` & `thztools-0.0.2/.ruff_cache/content/8f3375e559447e11`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/946677cfaae5d078` & `thztools-0.0.2/.ruff_cache/content/946677cfaae5d078`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/9faaf717898e7034` & `thztools-0.0.2/.ruff_cache/content/9faaf717898e7034`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/a8022447c114b8da` & `thztools-0.0.2/.ruff_cache/content/a8022447c114b8da`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/abf48d11c0afd9ef` & `thztools-0.0.2/.ruff_cache/content/abf48d11c0afd9ef`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/ac982820098a0c6b` & `thztools-0.0.2/.ruff_cache/content/ac982820098a0c6b`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/ad90ede8303e1447` & `thztools-0.0.2/.ruff_cache/content/ad90ede8303e1447`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/b0448d2cb1c22a2e` & `thztools-0.0.2/.ruff_cache/content/b0448d2cb1c22a2e`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/b70dc04ea668b378` & `thztools-0.0.2/.ruff_cache/content/b70dc04ea668b378`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/bac347fb4506c042` & `thztools-0.0.2/.ruff_cache/content/bac347fb4506c042`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/c068bcc1830cc02` & `thztools-0.0.2/.ruff_cache/content/c068bcc1830cc02`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/c2fae3237f5f1a4a` & `thztools-0.0.2/.ruff_cache/content/c2fae3237f5f1a4a`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/c753ff9e605d5bb8` & `thztools-0.0.2/.ruff_cache/content/c753ff9e605d5bb8`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/d2551b373b0a40ff` & `thztools-0.0.2/.ruff_cache/content/d2551b373b0a40ff`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/fa6062adf3c39eac` & `thztools-0.0.2/.ruff_cache/content/fa6062adf3c39eac`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/.ruff_cache/content/fb453ce093001723` & `thztools-0.0.2/.ruff_cache/content/fb453ce093001723`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/src/thztools/_util.py` & `thztools-0.0.2/src/thztools/_util.py`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/src/thztools/thztools.py` & `thztools-0.0.2/src/thztools/thztools.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,1052 +1,1052 @@
-import warnings
-
-import numpy as np
-import pandas as pd
-import scipy.linalg  # type: ignore
-from numpy.fft import irfft, rfft, rfftfreq
-from scipy.optimize import minimize  # type: ignore
-
-
-def fftfreq(n, t):
-    """Computes the positive and negative frequencies sampled in the Fast
-    Fourier Transform.
-
-    Parameters
-    ----------
-    n : int
-        Number of time samples
-    t: float
-        Sampling time
-
-    Returns
-    -------
-    f : ndarray
-        Frequency vector (1/ts) of length n containing the sample frequencies.
-    """
-
-    if n % 2 == 1:
-        f = np.fft.fftfreq(n, t)
-    else:
-        f = np.fft.fftfreq(n, t)
-        f[int(n / 2)] = -f[int(n / 2)]
-
-    return f
-
-
-def noisevar(sigma, mu, ts):
-    r"""
-    Noisevar computes the time-domain noise variance for noise parameters
-    sigma, with a signal mu and sampling interval T. There are three noise
-    parameters: the first corresponds to amplitude noise, in signal units (
-    i.e, the same units as mu) ;  the second corresponds to multiplicative
-    noise, which is dimensionless; and the third corresponds to timebase
-    noise, in units of signal/time, where the units for time are the same as
-    for T. The output, Vmu, is given in units that are the square of the
-    signal units.
-
-    Parameters
-    ----------
-    sigma : ndarray
-        (3, ) array  containing noise parameters
-    mu : ndarray
-        (n, ) array  containing  signal vector
-    ts : float
-        Sampling time
-
-    Returns
-    --------
-    vmu : ndarray
-        Noise variance
-    """
-
-    n = mu.shape[0]
-    w = 2 * np.pi * rfftfreq(n, ts)
-    mudot = irfft(1j * w * rfft(mu), n=n)
-
-    return sigma[0] ** 2 + (sigma[1] * mu) ** 2 + (sigma[2] * mudot) ** 2
-
-
-def noiseamp(sigma, mu, ts):
-    r"""
-    noiseamp computes the time-domain noise amplitudes for noise parameters
-    sigma, with a signal mu and sampling interval t.  There are three noise
-    parameters: the first corresponds to amplitude noise, in signal units (
-    ie, the same units as mu); the second corresponds to multiplicative
-    noise, which is dimensionless; and the third corresponds to timebase
-    noise, in units of signal/time, where the units for time are the same as
-    for t. The output, sigmamu, is given in signal units.
-
-    Parameters
-    ----------
-    sigma : ndarray
-        (3, ) array  containing noise parameters
-    mu :  signal vector
-        (n, ) array  containing  signal vector
-    ts : float
-        sampling time
-
-    Returns
-    -------
-    sigmamu : ndarray
-        (n, ) array containing noise amplitude
-    """
-
-    return np.sqrt(noisevar(sigma, mu, ts))
-
-
-def thzgen(n, ts, t0, a=1.0, taur=0.3, tauc=0.1, fwhm=0.05):
-    r"""Generate a terahertz pulse.
-
-    Returns an idealized waveform with n points at sampling interval t and
-    centered at t0.
-
-    Parameters
-    ----------
-
-    n : int
-        number of sampled points.
-
-    ts : float
-        sampling time
-
-    t0 : float
-        pulse center
-
-    a : float, optional
-        Peak amplitude.
-
-    taur : float, optional
-        Current pulse rise time.
-
-    tauc : float, optional
-        Current pulse decay time.
-
-    fwhm : float, optional
-        Laser pulse FWHM.
-
-    Returns
-    -------
-
-    y : ndarray
-        signal (u.a)
-
-    t : float
-        timebase
-
-    """
-
-    taul = fwhm / np.sqrt(2 * np.log(2))
-
-    f = rfftfreq(n, ts)
-
-    w = 2 * np.pi * f
-    ell = np.exp(-((w * taul) ** 2) / 2) / np.sqrt(2 * np.pi * taul ** 2)
-    r = 1 / (1 / taur - 1j * w) - 1 / (1 / taur + 1 / tauc - 1j * w)
-    s = -1j * w * (ell * r) ** 2 * np.exp(1j * w * t0)
-
-    t2 = ts * np.arange(n)
-
-    y = irfft(np.conj(s), n=n)
-    y = a * y / np.max(y)
-
-    return [y, t2]
-
-
-class DataPulse:
-    def __init__(self, filename=""):
-        self.AcquisitionTime = None
-        self.Description = None
-        self.TimeConstant = None
-        self.WaitTime = None
-        self.setPoint = None
-        self.scanOffset = None
-        self.temperature = None
-        self.time = None
-        self.amplitude = None
-        self.ChannelAMaximum = None
-        self.ChannelAMinimum = None
-        self.ChannelAVariance = None
-        self.ChannelASlope = None
-        self.ChannelAOffset = None
-        self.ChannelBMaximum = None
-        self.ChannelBMinimum = None
-        self.ChannelBVariance = None
-        self.ChannelBSlope = None
-        self.ChannelBOffset = None
-        self.ChannelCMaximum = None
-        self.ChannelCMinimum = None
-        self.ChannelCVariance = None
-        self.ChannelCSlope = None
-        self.ChannelCOffset = None
-        self.ChannelDMaximum = None
-        self.ChannelDMinimum = None
-        self.ChannelDVariance = None
-        self.ChannelDSlope = None
-        self.ChannelDOffset = None
-        self.dirname = None
-        self.file = None
-        self.filename = filename
-        self.frequency = None
-
-        if filename is not None:
-            data = pd.read_csv(filename, header=None, delimiter="\t")
-
-            ind = 0
-            for i in range(data.shape[0]):
-                try:
-                    float(data[0][i])
-                except ValueError:
-                    ind = i + 1
-                pass
-
-            keys = data[0][0:ind].to_list()
-            vals = data[1][0:ind].to_list()
-
-            for k in range(len(keys)):
-                if keys[k] in list(self.__dict__.keys()):
-                    try:
-                        float(vals[k])
-                        setattr(self, keys[k], float(vals[k]))
-                    except ValueError:
-                        setattr(self, keys[k], vals[k])
-
-                else:
-                    msg = "The data key is not defied"
-                    raise Warning(msg)
-
-            self.time = data[0][ind:].to_numpy(dtype=float)
-            self.amplitude = data[1][ind:].to_numpy(dtype=float)
-
-            # Calculate frequency range
-            self.frequency = (
-                                     np.arange(
-                                         np.floor(len(self.time))) / 2 - 1
-                             ).T / (self.time[-1] - self.time[0])
-
-            # Calculate fft
-            famp = np.fft.fft(self.amplitude)
-            self.famp = famp[0: int(np.floor(len(famp) / 2))]
-
-
-def shiftmtx(tau, n, ts):
-    """
-    Shiftmtx computes the n by n transfer matrix for a continuous time-shift.
-
-    Parameters
-    -----------
-
-    tau : float
-        Input parameters for the function
-
-    n : int
-        Number of time samples
-
-    ts: int
-        sampling time
-
-    Returns
-    -------
-    h: ndarray or matrix
-        (n, n) Transfer matrix
-
-    """
-
-    # Fourier method
-    f = rfftfreq(n, ts)
-    w = 2 * np.pi * f
-
-    imp = irfft(np.exp(-1j * w * tau), n=n)
-
-    # computes the n by n transformation matrix
-    h = scipy.linalg.toeplitz(imp, np.roll(np.flipud(imp), 1))
-
-    return h
-
-
-def airscancorrect(x, param):
-    """Airscancorrect rescales and shifts each column of the data matrix x,
-    assuming that each column is related to a common signal by an amplitude A
-    and a delay eta.
-
-    Parameters
-    ----------
-    x : ndarray or matrix
-        (n,m) data matrix
-
-
-    param: dict
-        Parameter dictionary including:
-            A : ndarray
-                (m, ) array containing amplitude vector
-            eta : ndarray
-                (m, ) array containing delay vector
-            ts : float
-                sampling time
-
-
-
-    Returns
-    -------
-    xadj : ndarray or matrix
-        Adjusted data matrix
-
-    """
-
-    # Parse function inputs
-    [n, m] = x.shape
-
-    # Parse parameter structure
-    pfields = param.keys()
-    if "a" in pfields and param.get("a") is not None:
-        a = param.get("a").T
-    else:
-        a = np.ones((m, 1))
-        # Ignore.A = true
-    if "eta" in pfields and param.get("eta") is not None:
-        eta = param.get("eta")
-    else:
-        eta = np.zeros((m, 1))
-    if "ts" in pfields:
-        ts = param["ts"]
-    else:
-        ts = 1
-
-    xadj = np.zeros((n, m))
-    for i in np.arange(m):
-        s = shiftmtx(-eta[i], n, ts)
-        xadj[:, i] = s @ (x[:, i] / a[i])
-
-    return xadj
-
-
-def costfunlsq(fun, theta, xx, yy, sigmax, sigmay, ts):
-    r"""Computes the maximum likelihood cost function.
-
-    Parameters
-    ----------
-        fun : callable
-            Transfer function, in the form fun(theta,w), -iwt convention.
-
-        theta : ndarray
-            Input parameters for the function.
-
-        xx : ndarray
-            Measured input signal.
-
-        yy : ndarray
-            Measured output signal.
-
-        sigmax : ndarray or matrix
-            Noise covariance matrix of the input signal.
-
-        sigmay : nadarray
-            Noise covariance matrix of the output signal.
-
-        ts : float
-            Sampling time.
-
-    Returns
-    -------
-    res : callable
-
-
-    """
-    n = xx.shape[0]
-    wfft = 2 * np.pi * rfftfreq(n, ts)
-    h = np.conj(fun(theta, wfft))
-
-    ry = yy - irfft(rfft(xx) * h, n=n)
-    vy = np.diag(sigmay ** 2)
-
-    htilde = irfft(h, n=n)
-
-    uy = np.zeros((n, n))
-    for k in np.arange(n):
-        a = np.reshape(np.roll(htilde, k), (n, 1))
-        b = np.reshape(np.conj(np.roll(htilde, k)), (1, n))
-        uy = uy + np.real(np.dot(a, b)) * sigmax[k] ** 2
-        # uy = uy + np.real(np.roll(htilde, k-1) @ np.roll(htilde, k-1).T) @
-        # sigmax[k]**2
-
-    w = np.dot(np.eye(n), scipy.linalg.inv(scipy.linalg.sqrtm(uy + vy)))
-    res = np.dot(w, ry)
-
-    return res
-
-
-def tdtf(fun, theta, n, ts):
-    """
-    Returns the transfer matrix for a given function.
-
-    It computes the n-by-n transfer matrix for the given function fun with
-    input parameter theta. Note that the transfer function should be written
-    using the physicist's -iwt convention, and that it should be in the
-    format fun(theta,w), where theta
-    is a vector of the function parameters. The transfer function must be
-    Hermitian.
-
-    Parameters
-    ----------
-        fun : callable
-            Transfer function, in the form fun(theta,w), -iwt convention.
-
-        theta : ndarray
-            Input parameters for the function.
-
-        n : int
-            Number of time samples.
-
-        ts : ndarray
-            Sampling time.
-
-    Returns
-    -------
-        h : ndarray or matrix
-            Transfer matrix with size (n,n).
-
-    """
-
-    # compute the transfer function over positive frequencies
-    if not isinstance(ts, np.ndarray):
-        ts = np.array([ts])
-    else:
-        ts = ts
-
-    fs = 1 / (ts * n)
-    fp = fs * np.arange(0, (n - 1) // 2 + 1)
-    wp = 2 * np.pi * fp
-    tfunp = fun(theta, wp)
-
-    # The transfer function is Hermitian, so we evaluate negative frequencies
-    # by taking the complex conjugate of the corresponding positive frequency.
-    # Include the value of the transfer function at the Nyquist frequency for
-    # even n.
-    if n % 2 != 0:
-        tfun = np.concatenate((tfunp, np.conj(np.flipud(tfunp[1:]))))
-
-    else:
-        wny = np.pi * n * fs
-        # print('tfunp', tfunp)
-        tfun = np.concatenate(
-            (
-                tfunp,
-                np.conj(
-                    np.concatenate((fun(theta, wny), np.flipud(tfunp[1:])))
-                ),
-            )
-        )
-
-    # Evaluate the impulse response by taking the inverse Fourier transform,
-    # taking the complex conjugate first to convert to ... +iwt convention
-
-    imp = np.real(np.fft.ifft(np.conj(tfun)))
-    h = scipy.linalg.toeplitz(imp, np.roll(np.flipud(imp), 1))
-
-    return h
-
-
-def tdnll(x, param, fix):
-    r"""Computes negative log-likelihood for the time-domain noise model.
-
-    Computes the negative log-likelihood function for obtaining the
-     data matrix x, given the parameter dictionary param.
-
-    Parameters
-    ----------
-    x : ndarray or matrix
-        Data matrix
-    param : dict
-        A dictionary containing parameters including:
-        logv : ndarray
-            Array of size (3, ) containing log of noise parameters.
-        mu : ndarray
-            Signal vector of size (n,).
-        a: ndarray
-            Amplitude vector of size (m,).
-        eta : ndarray
-            Delay vector of size (m,).
-        ts : float
-            Sampling time.
-        d : ndarray or matrix
-            n-by-n derivative matrix.
-    fix : dict
-        A dictionary containing variables to fix for the gradient calculation.
-        logv : bool
-            Log of noise parameters.
-        mu : bool
-            Signal vector.
-        a : bool
-            Amplitude vector.
-        eta : bool
-            Delay vector.
-
-    Returns
-    -------
-    nll : callable
-        Negative log-likelihood function
-    gradnll : ndarray
-        Gradient of the negative log-likelihood function
-    """
-    # Parse function inputs
-    [n, m] = x.shape
-
-    # Parse parameter dictionary
-    pfields = param.keys()
-    ignore = {}
-    if "logv" in pfields:
-        v = np.exp(param["logv"])
-        v = np.reshape(v, (len(v), 1))
-    else:
-        msg = "Tdnll requires Param structure with logv field"
-        raise ValueError(msg)
-
-    if "mu" in pfields:
-        mu = param["mu"]
-        mu = np.reshape(mu, (len(mu), 1))
-    else:
-        msg = "Tdnll requires param structure with mu field"
-        raise ValueError(msg)
-    pass
-
-    if "a" in pfields and param["a"] != []:
-        a = param["a"]
-        a = np.reshape(a, (len(a), 1))
-        ignore["a"] = False
-    else:
-        a = np.ones((m, 1))
-        ignore["a"] = True
-    pass
-
-    if "eta" in pfields and param["eta"] != []:
-        eta = param["eta"]
-        eta = np.reshape(eta, (len(eta), 1))
-        ignore["eta"] = False
-    else:
-        eta = np.zeros((m, 1))
-        ignore["eta"] = True
-    pass
-
-    if "ts" in pfields:
-        ts = param["ts"]
-    else:
-        ts = 1
-        warnings.warn(
-            "TDNLL received Param structure without ts field; set to one",
-            stacklevel=2,
-        )
-    pass
-
-    if "d" in pfields:
-        d = param["d"]
-    else:
-        # Compute derivative matrix
-        def fun(_, _w):
-            return -1j * _w
-
-        d = tdtf(fun, 0, n, ts)
-    pass
-
-    # Compute frequency vector and Fourier coefficients of mu
-    f = fftfreq(n, ts)
-    w = 2 * np.pi * f
-    w = w.reshape(len(w), 1)
-    mu_f = np.fft.fft(mu.flatten()).reshape(len(mu), 1)
-
-    gradcalc = np.logical_not(
-        [
-            [fix["logv"]],
-            [fix["mu"]],
-            [fix["a"] or ignore["a"]],
-            [fix["eta"] or ignore["eta"]],
-        ]
-    )
-
-    if ignore["eta"]:
-        zeta = mu * np.conj(a).T
-        zeta_f = np.fft.fft(zeta, axis=0)
-    else:
-        exp_iweta = np.exp(1j * np.tile(w, m) * np.conj(np.tile(eta, n)).T)
-        zeta_f = (
-                np.conj(np.tile(a, n)).T * np.conj(exp_iweta) * np.tile(mu_f,
-                                                                        m)
-        )
-        zeta = np.real(np.fft.ifft(zeta_f, axis=0))
-
-    # Compute negative - log likelihood and gradient
-
-    # Compute residuals and their squares for subsequent computations
-    res = x - zeta
-    ressq = res ** 2
-
-    # Simplest case: just variance and signal parameters, A and eta fixed at
-    # defaults
-    if ignore["a"] and ignore["eta"]:
-        dmu = np.real(np.fft.ifft(1j * w * mu_f, axis=0))
-        valpha = v[0]
-        vbeta = v[1] * mu ** 2
-        vtau = v[2] * dmu ** 2
-        vtot = valpha + vbeta + vtau
-
-        resnormsq = ressq / np.tile(vtot, m)
-        nll = (
-                m * n * np.log(2 * np.pi) / 2
-                + (m / 2) * np.sum(np.log(vtot))
-                + np.sum(resnormsq) / 2
-        )
-
-        # Compute gradient if requested
-        # if nargout > 1:
-        ngrad = np.sum(gradcalc[0:2] * [[3], [n]])
-        gradnll = np.zeros((ngrad, 1))
-        nstart = 0
-        dvar = (vtot - np.mean(ressq, axis=1).reshape(n, 1)) / vtot ** 2
-        if gradcalc[0]:
-            gradnll[nstart] = (m / 2) * np.sum(dvar) * v[0]
-            gradnll[nstart + 1] = (m / 2) * np.sum(mu ** 2 * dvar) * v[1]
-            gradnll[nstart + 2] = (m / 2) * np.sum(dmu ** 2.0 * dvar) * v[2]
-            nstart = nstart + 3
-        if gradcalc[1]:
-            # print('mu shape : ', mu.shape)
-            # print('dvar shape: ', dvar.shape)
-            # print('d shape: ', d.shape)
-            # print('Dmu shape: ', dmu.shape)
-            gradnll[nstart: nstart + n] = m * (
-                    v[1] * mu * dvar
-                    + v[2] * np.dot(d.T, (dmu * dvar))
-                    - np.mean(res, axis=1).reshape(n, 1) / vtot
-            )
-
-    # Alternative case: A, eta, or both are not set to defaults
-    else:
-        dzeta = np.real(np.fft.ifft(1j * np.tile(w, m) * zeta_f, axis=0))
-
-        valpha = v[0]
-        vbeta = v[1] * zeta ** 2
-        vtau = v[2] * dzeta ** 2
-        vtot = valpha + vbeta + vtau
-
-        resnormsq = ressq / vtot
-        nll = (
-                m * n * np.log(2 * np.pi) / 2
-                + np.sum(np.log(vtot)) / 2
-                + np.sum(resnormsq) / 2
-        )
-
-        # Compute gradient if requested
-        # if nargout > 1:
-        ngrad = np.sum(gradcalc * [[3], [n], [m], [m]])
-        gradnll = np.zeros((ngrad, 1))
-        nstart = 0
-        reswt = res / vtot
-        dvar = (vtot - ressq) / vtot ** 2
-        if gradcalc[0]:
-            # Gradient wrt logv
-            gradnll[nstart] = 0.5 * np.sum(dvar) * v[0]
-            gradnll[nstart + 1] = (
-                    0.5 * np.sum(zeta.flatten() ** 2 * dvar.flatten()) * v[1]
-            )
-            gradnll[nstart + 2] = (
-                    0.5 * np.sum(dzeta.flatten() ** 2 * dvar.flatten()) * v[2]
-            )
-            nstart = nstart + 3
-        if gradcalc[1]:
-            # Gradient wrt mu
-            p = np.fft.fft(v[1] * dvar * zeta - reswt, axis=0) - 1j * v[
-                2
-            ] * w * np.fft.fft(dvar * dzeta, axis=0)
-            gradnll[nstart: nstart + n] = np.sum(
-                np.conj(a).T * np.real(np.fft.ifft(exp_iweta * p, axis=0)),
-                axis=1,
-            ).reshape(n, 1)
-            nstart = nstart + n
-        if gradcalc[2]:
-            # Gradient wrt A
-            term = (vtot - valpha) * dvar - reswt * zeta
-            if np.any(np.isclose(a, 0)):
-                msg = (
-                    "One or more elements of the amplitude vector are "
-                    "close to zero "
-                )
-                raise ValueError(msg)
-            gradnll[nstart: nstart + m] = (
-                    np.conj(np.sum(term, axis=0)).reshape(m, 1) / a
-            )
-            if not fix["mu"]:
-                gradnll = np.delete(gradnll, nstart)
-                nstart = nstart + m - 1
-            else:
-                nstart = nstart + m
-        if gradcalc[3]:
-            # Gradient wrt eta
-            ddzeta = np.real(np.fft.ifft(-np.tile(w, m) ** 2 * zeta_f, axis=0))
-            gradnll = np.squeeze(gradnll)
-            gradnll[nstart: nstart + m] = -np.sum(
-                dvar * (zeta * dzeta * v[1] + dzeta * ddzeta * v[2])
-                - reswt * dzeta,
-                axis=0,
-            ).reshape(
-                m,
-            )
-
-            if not fix["mu"]:
-                gradnll = np.delete(gradnll, nstart)
-    gradnll = gradnll.flatten()
-
-    return nll, gradnll
-
-
-def tdnoisefit(
-        x,
-        param,
-        fix={"logv": False, "mu": False, "a": True, "eta": True},
-        ignore={"a": True, "eta": True},
-):
-    """Computes time-domain noise model parameters.
-
-    Computes the noise parameters sigma and the underlying signal vector mu
-    for the data matrix x, where the columns of x are each noisy
-    measurements of mu.
-
-    Parameters
-    ----------
-    x : ndarray or matrix
-        Data matrix.
-    param : dict
-        A dictionary containing initial guess for the parameters:
-        v0 : ndarray
-            Initial guess, noise model parameters. Array of real elements of
-            size (3, )
-        mu0 : ndarray
-            Initial guess, signal vector. Array of real elements of size  (n, )
-        a0 : ndarray
-            Initial guess, amplitude vector. Array of real elements of size
-            (m, )
-        eta0 : ndarray
-            Initial guess, delay vector. Array of real elements of size (m, )
-        ts : float
-            Sampling time
-    fix : dict, optional
-        A dictionary containing variables to fix for the minimization.
-        logv : bool
-            Log of noise parameters.
-        mu : bool
-            Signal vector.
-        a : bool
-            Amplitude vector.
-        eta : bool
-            Delay vector.
-        If not given, chosen to set free all the variables.
-    ignore : dict
-        A dictionary containing variables to ignore for the minimization.
-        a : bool
-            Amplitude vector.
-        eta : bool
-            Delay vector.
-        If not given, chosen to ignore both amplitude and delay.
-
-    Returns
-    --------
-    p : dict
-        Output parameter dictionary containing:
-            eta : ndarray
-                Delay vector.
-            a : ndarray
-                Amplitude vector.
-            mu : ndarray
-                Signal vector.
-            var : ndarray
-                Log of noise parameters
-    fval : float
-        Value of NLL cost function from FMINUNC
-    Diagnostic : dict
-        Dictionary containing diagnostic information
-            err : dic
-                Dictionary containing  error of the parameters.
-            grad : ndarray
-                Negative loglikelihood cost function gradient from
-                scipy.optimize.minimize BFGS method.
-            hessian : ndarray
-                Negative loglikelihood cost function hessian from
-                scipy.optimize.minimize BFGS method.
-    """
-    n, m = x.shape
-
-    # Parse Inputs
-    if "v0" in param:
-        v0 = param["v0"]
-    else:
-        v0 = np.mean(np.var(x, 1)) * np.array([1, 1, 1])
-        param["v0"] = v0
-
-    if "mu0" in param:
-        mu0 = param["mu0"]
-    else:
-        mu0 = np.mean(x, 1)
-        param["mu0"] = mu0
-
-    if "a0" in param:
-        a0 = param["a0"]
-    else:
-        a0 = np.ones(m)
-        param["a0"] = a0
-
-    if "eta0" in param:
-        eta0 = param["eta0"]
-    else:
-        eta0 = np.zeros(m)
-        param["eta0"] = eta0
-
-    if "ts" in param:
-        param["ts"]
-    else:
-        param["ts"] = 1
-
-    mle = {"x0": np.array([])}
-    idxstart = 0
-    idxrange = {}
-
-    # If fix['logv'], return log(v0); otherwise return logv parameters
-    if fix["logv"]:
-
-        def setplogv(_):
-            return np.log(param["v0"])
-
-    else:
-        mle["x0"] = np.concatenate((mle["x0"], np.log(param["v0"])))
-        idxend = idxstart + 3
-        idxrange["logv"] = np.arange(idxstart, idxend)
-
-        def setplogv(_p):
-            return _p[idxrange["logv"]]
-
-        idxstart = idxend
-    pass
-
-    # If Fix['mu'], return mu0, otherwise, return mu parameters
-    if fix["mu"]:
-
-        def setpmu(_):
-            return param["mu0"]
-
-    else:
-        mle["x0"] = np.concatenate((mle["x0"], param["mu0"]))
-        idxend = idxstart + n
-        idxrange["mu"] = np.arange(idxstart, idxend)
-
-        def setpmu(_p):
-            return _p[idxrange["mu"]]
-
-        idxstart = idxend
-    pass
-
-    # If ignore A, return []; if Fix['A'], return A0; if ~Fix.A & Fix.mu,
-    # return all A parameters;
-    # If ~Fix.A & ~Fix.mu, return all A parameters but first
-
-    if ignore["a"]:
-
-        def setpa(_):
-            return []
-
-    elif fix["a"]:
-
-        def setpa(_):
-            return param["a0"]
-
-    elif fix["mu"]:
-        mle["x0"] = np.concatenate((mle["x0"], param["a0"]))
-        idxend = idxstart + m
-        idxrange["a"] = np.arange(idxstart, idxend)
-
-        def setpa(_p):
-            return _p[idxrange["a"]]
-
-        idxstart = idxend
-    else:
-        mle["x0"] = np.concatenate(
-            (mle["x0"], param["a0"][1:] / param["a0"][0])
-        )
-        idxend = idxstart + m - 1
-        idxrange["a"] = np.arange(idxstart, idxend)
-
-        def setpa(_p):
-            return np.concatenate(([1], _p[idxrange["a"]]), axis=0)
-
-        idxstart = idxend
-    pass
-
-    # If Ignore.eta, return []; if Fix.eta, return eta0; if ~Fix.eta &
-    # Fix.mu,return all eta parameters;
-    # if ~Fix.eta & ~Fix.mu, return all eta parameters but first
-
-    if ignore["eta"]:
-
-        def setpeta(_):
-            return []
-
-    elif fix["eta"]:
-
-        def setpeta(_):
-            return param["eta0"]
-
-    elif fix["mu"]:
-        mle["x0"] = np.concatenate((mle["x0"], param["eta0"]))
-        idxend = idxstart + m
-        idxrange["eta"] = np.arange(idxstart, idxend)
-
-        def setpeta(_p):
-            return _p[idxrange["eta"]]
-
-    else:
-        mle["x0"] = np.concatenate(
-            (mle["x0"], param["eta0"][1:] - param["eta0"][0])
-        )
-        idxend = idxstart + m - 1
-        idxrange["eta"] = np.arange(idxstart, idxend)
-
-        def setpeta(_p):
-            return np.concatenate(([0], _p[idxrange["eta"]]), axis=0)
-
-    pass
-
-    def fun(_, _w):
-        return -1j * _w
-
-    d = tdtf(fun, 0, n, param["ts"])
-
-    def parsein(_p):
-        return {
-            "logv": setplogv(_p),
-            "mu": setpmu(_p),
-            "a": setpa(_p),
-            "eta": setpeta(_p),
-            "ts": param["ts"],
-            "d": d,
-        }
-
-    def objective(_p):
-        return tdnll(x, parsein(_p), fix)[0]
-
-    def jacobian(_p):
-        return tdnll(x, parsein(_p), fix)[1]
-
-    mle["objective"] = objective
-    out = minimize(mle["objective"], mle["x0"], method="BFGS", jac=jacobian)
-
-    # The trust-region algorithm returns the Hessian for the next-to-last
-    # iterate, which may not be near the final point. To check, test for
-    # positive definiteness by attempting to Cholesky factorize it. If it
-    # returns an error, rerun the optimization with the quasi-Newton algorithm
-    # from the current optimal point.
-
-    try:
-        np.linalg.cholesky(np.linalg.inv(out.hess_inv))
-        hess = np.linalg.inv(out.hess_inv)
-    except np.linalg.LinAlgError:
-        print(
-            "Hessian returned by FMINUNC is not positive definite;\n"
-            "recalculating with quasi-Newton algorithm"
-        )
-
-        mle["x0"] = out.x
-        out2 = minimize(
-            mle["objective"], mle["x0"], method="BFGS", jac=jacobian
-        )
-        hess = np.linalg.inv(out2.hess_inv)
-
-    # Parse output
-    p = {}
-    idxrange = {}
-    idxstart = 0
-
-    if fix["logv"]:
-        p["var"] = param["v0"]
-    else:
-        idxend = idxstart + 3
-        idxrange["logv"] = np.arange(idxstart, idxend)
-        idxstart = idxend
-        p["var"] = np.exp(out.x[idxrange["logv"]])
-    pass
-
-    if fix["mu"]:
-        p["mu"] = param["mu0"]
-    else:
-        idxend = idxstart + n
-        idxrange["mu"] = np.arange(idxstart, idxend)
-        idxstart = idxend
-        p["mu"] = out.x[idxrange["mu"]]
-    pass
-
-    if ignore["a"] or fix["a"]:
-        p["a"] = param["a0"]
-    elif fix["mu"]:
-        idxend = idxstart + m
-        idxrange["a"] = np.arange(idxstart, idxend)
-        idxstart = idxend
-        p["a"] = out.x[idxrange["a"]]
-    else:
-        idxend = idxstart + m - 1
-        idxrange["a"] = np.arange(idxstart, idxend)
-        idxstart = idxend
-        p["a"] = np.concatenate(([1], out.x[idxrange["a"]]), axis=0)
-    pass
-
-    if ignore["eta"] or fix["eta"]:
-        p["eta"] = param["eta0"]
-    elif fix["mu"]:
-        idxend = idxstart + m
-        idxrange["eta"] = np.arange(idxstart, idxend)
-        p["eta"] = out.x[idxrange["eta"]]
-    else:
-        idxend = idxstart + m - 1
-        idxrange["eta"] = np.arange(idxstart, idxend)
-        p["eta"] = np.concatenate(([0], out.x[idxrange["eta"]]), axis=0)
-    pass
-
-    p["ts"] = param["ts"]
-
-    vary_param = np.logical_not(
-        [
-            fix["logv"],
-            fix["mu"],
-            fix["a"] or ignore["a"],
-            fix["eta"] or ignore["eta"],
-        ]
-    )
-    diagnostic = {
-        "grad": out.jac,
-        "hessian": hess,
-        "err": {"var": [], "mu": [], "a": [], "eta": []},
-    }
-    v = np.dot(np.eye(hess.shape[0]), scipy.linalg.inv(hess))
-    err = np.sqrt(np.diag(v))
-    idxstart = 0
-    if vary_param[0]:
-        diagnostic["err"]["var"] = np.sqrt(
-            np.diag(np.diag(p["var"]) * v[0:3, 0:3]) * np.diag(p["var"])
-        )
-        idxstart = idxstart + 3
-    pass
-
-    if vary_param[1]:
-        diagnostic["err"]["mu"] = err[idxstart: idxstart + n]
-        idxstart = idxstart + n
-    pass
-
-    if vary_param[2]:
-        if vary_param[1]:
-            diagnostic["err"]["a"] = err[idxstart: idxstart + m - 1]
-            idxstart = idxstart + m - 1
-        else:
-            diagnostic["err"]["a"] = err[idxstart: idxstart + m]
-            idxstart = idxstart + m
-    pass
-
-    if vary_param[3]:
-        if vary_param[1]:
-            diagnostic["err"]["eta"] = err[idxstart: idxstart + m - 1]
-        else:
-            diagnostic["err"]["eta"] = err[idxstart: idxstart + m]
-    pass
-
-    return [p, out.fun, diagnostic]
+import warnings
+
+import numpy as np
+import pandas as pd
+import scipy.linalg  # type: ignore
+from numpy.fft import irfft, rfft, rfftfreq
+from scipy.optimize import minimize  # type: ignore
+
+
+def fftfreq(n, t):
+    """Computes the positive and negative frequencies sampled in the Fast
+    Fourier Transform.
+
+    Parameters
+    ----------
+    n : int
+        Number of time samples
+    t: float
+        Sampling time
+
+    Returns
+    -------
+    f : ndarray
+        Frequency vector (1/ts) of length n containing the sample frequencies.
+    """
+
+    if n % 2 == 1:
+        f = np.fft.fftfreq(n, t)
+    else:
+        f = np.fft.fftfreq(n, t)
+        f[int(n / 2)] = -f[int(n / 2)]
+
+    return f
+
+
+def noisevar(sigma, mu, ts):
+    r"""
+    Noisevar computes the time-domain noise variance for noise parameters
+    sigma, with a signal mu and sampling interval T. There are three noise
+    parameters: the first corresponds to amplitude noise, in signal units (
+    i.e, the same units as mu) ;  the second corresponds to multiplicative
+    noise, which is dimensionless; and the third corresponds to timebase
+    noise, in units of signal/time, where the units for time are the same as
+    for T. The output, Vmu, is given in units that are the square of the
+    signal units.
+
+    Parameters
+    ----------
+    sigma : ndarray
+        (3, ) array  containing noise parameters
+    mu : ndarray
+        (n, ) array  containing  signal vector
+    ts : float
+        Sampling time
+
+    Returns
+    --------
+    vmu : ndarray
+        Noise variance
+    """
+
+    n = mu.shape[0]
+    w = 2 * np.pi * rfftfreq(n, ts)
+    mudot = irfft(1j * w * rfft(mu), n=n)
+
+    return sigma[0] ** 2 + (sigma[1] * mu) ** 2 + (sigma[2] * mudot) ** 2
+
+
+def noiseamp(sigma, mu, ts):
+    r"""
+    noiseamp computes the time-domain noise amplitudes for noise parameters
+    sigma, with a signal mu and sampling interval t.  There are three noise
+    parameters: the first corresponds to amplitude noise, in signal units (
+    ie, the same units as mu); the second corresponds to multiplicative
+    noise, which is dimensionless; and the third corresponds to timebase
+    noise, in units of signal/time, where the units for time are the same as
+    for t. The output, sigmamu, is given in signal units.
+
+    Parameters
+    ----------
+    sigma : ndarray
+        (3, ) array  containing noise parameters
+    mu :  signal vector
+        (n, ) array  containing  signal vector
+    ts : float
+        sampling time
+
+    Returns
+    -------
+    sigmamu : ndarray
+        (n, ) array containing noise amplitude
+    """
+
+    return np.sqrt(noisevar(sigma, mu, ts))
+
+
+def thzgen(n, ts, t0, a=1.0, taur=0.3, tauc=0.1, fwhm=0.05):
+    r"""Generate a terahertz pulse.
+
+    Returns an idealized waveform with n points at sampling interval t and
+    centered at t0.
+
+    Parameters
+    ----------
+
+    n : int
+        number of sampled points.
+
+    ts : float
+        sampling time
+
+    t0 : float
+        pulse center
+
+    a : float, optional
+        Peak amplitude.
+
+    taur : float, optional
+        Current pulse rise time.
+
+    tauc : float, optional
+        Current pulse decay time.
+
+    fwhm : float, optional
+        Laser pulse FWHM.
+
+    Returns
+    -------
+
+    y : ndarray
+        signal (u.a)
+
+    t : float
+        timebase
+
+    """
+
+    taul = fwhm / np.sqrt(2 * np.log(2))
+
+    f = rfftfreq(n, ts)
+
+    w = 2 * np.pi * f
+    ell = np.exp(-((w * taul) ** 2) / 2) / np.sqrt(2 * np.pi * taul ** 2)
+    r = 1 / (1 / taur - 1j * w) - 1 / (1 / taur + 1 / tauc - 1j * w)
+    s = -1j * w * (ell * r) ** 2 * np.exp(1j * w * t0)
+
+    t2 = ts * np.arange(n)
+
+    y = irfft(np.conj(s), n=n)
+    y = a * y / np.max(y)
+
+    return [y, t2]
+
+
+class DataPulse:
+    def __init__(self, filename=""):
+        self.AcquisitionTime = None
+        self.Description = None
+        self.TimeConstant = None
+        self.WaitTime = None
+        self.setPoint = None
+        self.scanOffset = None
+        self.temperature = None
+        self.time = None
+        self.amplitude = None
+        self.ChannelAMaximum = None
+        self.ChannelAMinimum = None
+        self.ChannelAVariance = None
+        self.ChannelASlope = None
+        self.ChannelAOffset = None
+        self.ChannelBMaximum = None
+        self.ChannelBMinimum = None
+        self.ChannelBVariance = None
+        self.ChannelBSlope = None
+        self.ChannelBOffset = None
+        self.ChannelCMaximum = None
+        self.ChannelCMinimum = None
+        self.ChannelCVariance = None
+        self.ChannelCSlope = None
+        self.ChannelCOffset = None
+        self.ChannelDMaximum = None
+        self.ChannelDMinimum = None
+        self.ChannelDVariance = None
+        self.ChannelDSlope = None
+        self.ChannelDOffset = None
+        self.dirname = None
+        self.file = None
+        self.filename = filename
+        self.frequency = None
+
+        if filename is not None:
+            data = pd.read_csv(filename, header=None, delimiter="\t")
+
+            ind = 0
+            for i in range(data.shape[0]):
+                try:
+                    float(data[0][i])
+                except ValueError:
+                    ind = i + 1
+                pass
+
+            keys = data[0][0:ind].to_list()
+            vals = data[1][0:ind].to_list()
+
+            for k in range(len(keys)):
+                if keys[k] in list(self.__dict__.keys()):
+                    try:
+                        float(vals[k])
+                        setattr(self, keys[k], float(vals[k]))
+                    except ValueError:
+                        setattr(self, keys[k], vals[k])
+
+                else:
+                    msg = "The data key is not defied"
+                    raise Warning(msg)
+
+            self.time = data[0][ind:].to_numpy(dtype=float)
+            self.amplitude = data[1][ind:].to_numpy(dtype=float)
+
+            # Calculate frequency range
+            self.frequency = (
+                                     np.arange(
+                                         np.floor(len(self.time))) / 2 - 1
+                             ).T / (self.time[-1] - self.time[0])
+
+            # Calculate fft
+            famp = np.fft.fft(self.amplitude)
+            self.famp = famp[0: int(np.floor(len(famp) / 2))]
+
+
+def shiftmtx(tau, n, ts):
+    """
+    Shiftmtx computes the n by n transfer matrix for a continuous time-shift.
+
+    Parameters
+    -----------
+
+    tau : float
+        Input parameters for the function
+
+    n : int
+        Number of time samples
+
+    ts: int
+        sampling time
+
+    Returns
+    -------
+    h: ndarray or matrix
+        (n, n) Transfer matrix
+
+    """
+
+    # Fourier method
+    f = rfftfreq(n, ts)
+    w = 2 * np.pi * f
+
+    imp = irfft(np.exp(-1j * w * tau), n=n)
+
+    # computes the n by n transformation matrix
+    h = scipy.linalg.toeplitz(imp, np.roll(np.flipud(imp), 1))
+
+    return h
+
+
+def airscancorrect(x, param):
+    """Airscancorrect rescales and shifts each column of the data matrix x,
+    assuming that each column is related to a common signal by an amplitude A
+    and a delay eta.
+
+    Parameters
+    ----------
+    x : ndarray or matrix
+        (n,m) data matrix
+
+
+    param: dict
+        Parameter dictionary including:
+            A : ndarray
+                (m, ) array containing amplitude vector
+            eta : ndarray
+                (m, ) array containing delay vector
+            ts : float
+                sampling time
+
+
+
+    Returns
+    -------
+    xadj : ndarray or matrix
+        Adjusted data matrix
+
+    """
+
+    # Parse function inputs
+    [n, m] = x.shape
+
+    # Parse parameter structure
+    pfields = param.keys()
+    if "a" in pfields and param.get("a") is not None:
+        a = param.get("a").T
+    else:
+        a = np.ones((m, 1))
+        # Ignore.A = true
+    if "eta" in pfields and param.get("eta") is not None:
+        eta = param.get("eta")
+    else:
+        eta = np.zeros((m, 1))
+    if "ts" in pfields:
+        ts = param["ts"]
+    else:
+        ts = 1
+
+    xadj = np.zeros((n, m))
+    for i in np.arange(m):
+        s = shiftmtx(-eta[i], n, ts)
+        xadj[:, i] = s @ (x[:, i] / a[i])
+
+    return xadj
+
+
+def costfunlsq(fun, theta, xx, yy, sigmax, sigmay, ts):
+    r"""Computes the maximum likelihood cost function.
+
+    Parameters
+    ----------
+        fun : callable
+            Transfer function, in the form fun(theta,w), -iwt convention.
+
+        theta : ndarray
+            Input parameters for the function.
+
+        xx : ndarray
+            Measured input signal.
+
+        yy : ndarray
+            Measured output signal.
+
+        sigmax : ndarray or matrix
+            Noise covariance matrix of the input signal.
+
+        sigmay : nadarray
+            Noise covariance matrix of the output signal.
+
+        ts : float
+            Sampling time.
+
+    Returns
+    -------
+    res : callable
+
+
+    """
+    n = xx.shape[0]
+    wfft = 2 * np.pi * rfftfreq(n, ts)
+    h = np.conj(fun(theta, wfft))
+
+    ry = yy - irfft(rfft(xx) * h, n=n)
+    vy = np.diag(sigmay ** 2)
+
+    htilde = irfft(h, n=n)
+
+    uy = np.zeros((n, n))
+    for k in np.arange(n):
+        a = np.reshape(np.roll(htilde, k), (n, 1))
+        b = np.reshape(np.conj(np.roll(htilde, k)), (1, n))
+        uy = uy + np.real(np.dot(a, b)) * sigmax[k] ** 2
+        # uy = uy + np.real(np.roll(htilde, k-1) @ np.roll(htilde, k-1).T) @
+        # sigmax[k]**2
+
+    w = np.dot(np.eye(n), scipy.linalg.inv(scipy.linalg.sqrtm(uy + vy)))
+    res = np.dot(w, ry)
+
+    return res
+
+
+def tdtf(fun, theta, n, ts):
+    """
+    Returns the transfer matrix for a given function.
+
+    It computes the n-by-n transfer matrix for the given function fun with
+    input parameter theta. Note that the transfer function should be written
+    using the physicist's -iwt convention, and that it should be in the
+    format fun(theta,w), where theta
+    is a vector of the function parameters. The transfer function must be
+    Hermitian.
+
+    Parameters
+    ----------
+        fun : callable
+            Transfer function, in the form fun(theta,w), -iwt convention.
+
+        theta : ndarray
+            Input parameters for the function.
+
+        n : int
+            Number of time samples.
+
+        ts : ndarray
+            Sampling time.
+
+    Returns
+    -------
+        h : ndarray or matrix
+            Transfer matrix with size (n,n).
+
+    """
+
+    # compute the transfer function over positive frequencies
+    if not isinstance(ts, np.ndarray):
+        ts = np.array([ts])
+    else:
+        ts = ts
+
+    fs = 1 / (ts * n)
+    fp = fs * np.arange(0, (n - 1) // 2 + 1)
+    wp = 2 * np.pi * fp
+    tfunp = fun(theta, wp)
+
+    # The transfer function is Hermitian, so we evaluate negative frequencies
+    # by taking the complex conjugate of the corresponding positive frequency.
+    # Include the value of the transfer function at the Nyquist frequency for
+    # even n.
+    if n % 2 != 0:
+        tfun = np.concatenate((tfunp, np.conj(np.flipud(tfunp[1:]))))
+
+    else:
+        wny = np.pi * n * fs
+        # print('tfunp', tfunp)
+        tfun = np.concatenate(
+            (
+                tfunp,
+                np.conj(
+                    np.concatenate((fun(theta, wny), np.flipud(tfunp[1:])))
+                ),
+            )
+        )
+
+    # Evaluate the impulse response by taking the inverse Fourier transform,
+    # taking the complex conjugate first to convert to ... +iwt convention
+
+    imp = np.real(np.fft.ifft(np.conj(tfun)))
+    h = scipy.linalg.toeplitz(imp, np.roll(np.flipud(imp), 1))
+
+    return h
+
+
+def tdnll(x, param, fix):
+    r"""Computes negative log-likelihood for the time-domain noise model.
+
+    Computes the negative log-likelihood function for obtaining the
+     data matrix x, given the parameter dictionary param.
+
+    Parameters
+    ----------
+    x : ndarray or matrix
+        Data matrix
+    param : dict
+        A dictionary containing parameters including:
+        logv : ndarray
+            Array of size (3, ) containing log of noise parameters.
+        mu : ndarray
+            Signal vector of size (n,).
+        a: ndarray
+            Amplitude vector of size (m,).
+        eta : ndarray
+            Delay vector of size (m,).
+        ts : float
+            Sampling time.
+        d : ndarray or matrix
+            n-by-n derivative matrix.
+    fix : dict
+        A dictionary containing variables to fix for the gradient calculation.
+        logv : bool
+            Log of noise parameters.
+        mu : bool
+            Signal vector.
+        a : bool
+            Amplitude vector.
+        eta : bool
+            Delay vector.
+
+    Returns
+    -------
+    nll : callable
+        Negative log-likelihood function
+    gradnll : ndarray
+        Gradient of the negative log-likelihood function
+    """
+    # Parse function inputs
+    [n, m] = x.shape
+
+    # Parse parameter dictionary
+    pfields = param.keys()
+    ignore = {}
+    if "logv" in pfields:
+        v = np.exp(param["logv"])
+        v = np.reshape(v, (len(v), 1))
+    else:
+        msg = "Tdnll requires Param structure with logv field"
+        raise ValueError(msg)
+
+    if "mu" in pfields:
+        mu = param["mu"]
+        mu = np.reshape(mu, (len(mu), 1))
+    else:
+        msg = "Tdnll requires param structure with mu field"
+        raise ValueError(msg)
+    pass
+
+    if "a" in pfields and param["a"] != []:
+        a = param["a"]
+        a = np.reshape(a, (len(a), 1))
+        ignore["a"] = False
+    else:
+        a = np.ones((m, 1))
+        ignore["a"] = True
+    pass
+
+    if "eta" in pfields and param["eta"] != []:
+        eta = param["eta"]
+        eta = np.reshape(eta, (len(eta), 1))
+        ignore["eta"] = False
+    else:
+        eta = np.zeros((m, 1))
+        ignore["eta"] = True
+    pass
+
+    if "ts" in pfields:
+        ts = param["ts"]
+    else:
+        ts = 1
+        warnings.warn(
+            "TDNLL received Param structure without ts field; set to one",
+            stacklevel=2,
+        )
+    pass
+
+    if "d" in pfields:
+        d = param["d"]
+    else:
+        # Compute derivative matrix
+        def fun(_, _w):
+            return -1j * _w
+
+        d = tdtf(fun, 0, n, ts)
+    pass
+
+    # Compute frequency vector and Fourier coefficients of mu
+    f = fftfreq(n, ts)
+    w = 2 * np.pi * f
+    w = w.reshape(len(w), 1)
+    mu_f = np.fft.fft(mu.flatten()).reshape(len(mu), 1)
+
+    gradcalc = np.logical_not(
+        [
+            [fix["logv"]],
+            [fix["mu"]],
+            [fix["a"] or ignore["a"]],
+            [fix["eta"] or ignore["eta"]],
+        ]
+    )
+
+    if ignore["eta"]:
+        zeta = mu * np.conj(a).T
+        zeta_f = np.fft.fft(zeta, axis=0)
+    else:
+        exp_iweta = np.exp(1j * np.tile(w, m) * np.conj(np.tile(eta, n)).T)
+        zeta_f = (
+                np.conj(np.tile(a, n)).T * np.conj(exp_iweta) * np.tile(mu_f,
+                                                                        m)
+        )
+        zeta = np.real(np.fft.ifft(zeta_f, axis=0))
+
+    # Compute negative - log likelihood and gradient
+
+    # Compute residuals and their squares for subsequent computations
+    res = x - zeta
+    ressq = res ** 2
+
+    # Simplest case: just variance and signal parameters, A and eta fixed at
+    # defaults
+    if ignore["a"] and ignore["eta"]:
+        dmu = np.real(np.fft.ifft(1j * w * mu_f, axis=0))
+        valpha = v[0]
+        vbeta = v[1] * mu ** 2
+        vtau = v[2] * dmu ** 2
+        vtot = valpha + vbeta + vtau
+
+        resnormsq = ressq / np.tile(vtot, m)
+        nll = (
+                m * n * np.log(2 * np.pi) / 2
+                + (m / 2) * np.sum(np.log(vtot))
+                + np.sum(resnormsq) / 2
+        )
+
+        # Compute gradient if requested
+        # if nargout > 1:
+        ngrad = np.sum(gradcalc[0:2] * [[3], [n]])
+        gradnll = np.zeros((ngrad, 1))
+        nstart = 0
+        dvar = (vtot - np.mean(ressq, axis=1).reshape(n, 1)) / vtot ** 2
+        if gradcalc[0]:
+            gradnll[nstart] = (m / 2) * np.sum(dvar) * v[0]
+            gradnll[nstart + 1] = (m / 2) * np.sum(mu ** 2 * dvar) * v[1]
+            gradnll[nstart + 2] = (m / 2) * np.sum(dmu ** 2.0 * dvar) * v[2]
+            nstart = nstart + 3
+        if gradcalc[1]:
+            # print('mu shape : ', mu.shape)
+            # print('dvar shape: ', dvar.shape)
+            # print('d shape: ', d.shape)
+            # print('Dmu shape: ', dmu.shape)
+            gradnll[nstart: nstart + n] = m * (
+                    v[1] * mu * dvar
+                    + v[2] * np.dot(d.T, (dmu * dvar))
+                    - np.mean(res, axis=1).reshape(n, 1) / vtot
+            )
+
+    # Alternative case: A, eta, or both are not set to defaults
+    else:
+        dzeta = np.real(np.fft.ifft(1j * np.tile(w, m) * zeta_f, axis=0))
+
+        valpha = v[0]
+        vbeta = v[1] * zeta ** 2
+        vtau = v[2] * dzeta ** 2
+        vtot = valpha + vbeta + vtau
+
+        resnormsq = ressq / vtot
+        nll = (
+                m * n * np.log(2 * np.pi) / 2
+                + np.sum(np.log(vtot)) / 2
+                + np.sum(resnormsq) / 2
+        )
+
+        # Compute gradient if requested
+        # if nargout > 1:
+        ngrad = np.sum(gradcalc * [[3], [n], [m], [m]])
+        gradnll = np.zeros((ngrad, 1))
+        nstart = 0
+        reswt = res / vtot
+        dvar = (vtot - ressq) / vtot ** 2
+        if gradcalc[0]:
+            # Gradient wrt logv
+            gradnll[nstart] = 0.5 * np.sum(dvar) * v[0]
+            gradnll[nstart + 1] = (
+                    0.5 * np.sum(zeta.flatten() ** 2 * dvar.flatten()) * v[1]
+            )
+            gradnll[nstart + 2] = (
+                    0.5 * np.sum(dzeta.flatten() ** 2 * dvar.flatten()) * v[2]
+            )
+            nstart = nstart + 3
+        if gradcalc[1]:
+            # Gradient wrt mu
+            p = np.fft.fft(v[1] * dvar * zeta - reswt, axis=0) - 1j * v[
+                2
+            ] * w * np.fft.fft(dvar * dzeta, axis=0)
+            gradnll[nstart: nstart + n] = np.sum(
+                np.conj(a).T * np.real(np.fft.ifft(exp_iweta * p, axis=0)),
+                axis=1,
+            ).reshape(n, 1)
+            nstart = nstart + n
+        if gradcalc[2]:
+            # Gradient wrt A
+            term = (vtot - valpha) * dvar - reswt * zeta
+            if np.any(np.isclose(a, 0)):
+                msg = (
+                    "One or more elements of the amplitude vector are "
+                    "close to zero "
+                )
+                raise ValueError(msg)
+            gradnll[nstart: nstart + m] = (
+                    np.conj(np.sum(term, axis=0)).reshape(m, 1) / a
+            )
+            if not fix["mu"]:
+                gradnll = np.delete(gradnll, nstart)
+                nstart = nstart + m - 1
+            else:
+                nstart = nstart + m
+        if gradcalc[3]:
+            # Gradient wrt eta
+            ddzeta = np.real(np.fft.ifft(-np.tile(w, m) ** 2 * zeta_f, axis=0))
+            gradnll = np.squeeze(gradnll)
+            gradnll[nstart: nstart + m] = -np.sum(
+                dvar * (zeta * dzeta * v[1] + dzeta * ddzeta * v[2])
+                - reswt * dzeta,
+                axis=0,
+            ).reshape(
+                m,
+            )
+
+            if not fix["mu"]:
+                gradnll = np.delete(gradnll, nstart)
+    gradnll = gradnll.flatten()
+
+    return nll, gradnll
+
+
+def tdnoisefit(
+        x,
+        param,
+        fix={"logv": False, "mu": False, "a": True, "eta": True},
+        ignore={"a": True, "eta": True},
+):
+    """Computes time-domain noise model parameters.
+
+    Computes the noise parameters sigma and the underlying signal vector mu
+    for the data matrix x, where the columns of x are each noisy
+    measurements of mu.
+
+    Parameters
+    ----------
+    x : ndarray or matrix
+        Data matrix.
+    param : dict
+        A dictionary containing initial guess for the parameters:
+        v0 : ndarray
+            Initial guess, noise model parameters. Array of real elements of
+            size (3, )
+        mu0 : ndarray
+            Initial guess, signal vector. Array of real elements of size  (n, )
+        a0 : ndarray
+            Initial guess, amplitude vector. Array of real elements of size
+            (m, )
+        eta0 : ndarray
+            Initial guess, delay vector. Array of real elements of size (m, )
+        ts : float
+            Sampling time
+    fix : dict, optional
+        A dictionary containing variables to fix for the minimization.
+        logv : bool
+            Log of noise parameters.
+        mu : bool
+            Signal vector.
+        a : bool
+            Amplitude vector.
+        eta : bool
+            Delay vector.
+        If not given, chosen to set free all the variables.
+    ignore : dict
+        A dictionary containing variables to ignore for the minimization.
+        a : bool
+            Amplitude vector.
+        eta : bool
+            Delay vector.
+        If not given, chosen to ignore both amplitude and delay.
+
+    Returns
+    --------
+    p : dict
+        Output parameter dictionary containing:
+            eta : ndarray
+                Delay vector.
+            a : ndarray
+                Amplitude vector.
+            mu : ndarray
+                Signal vector.
+            var : ndarray
+                Log of noise parameters
+    fval : float
+        Value of NLL cost function from FMINUNC
+    Diagnostic : dict
+        Dictionary containing diagnostic information
+            err : dic
+                Dictionary containing  error of the parameters.
+            grad : ndarray
+                Negative loglikelihood cost function gradient from
+                scipy.optimize.minimize BFGS method.
+            hessian : ndarray
+                Negative loglikelihood cost function hessian from
+                scipy.optimize.minimize BFGS method.
+    """
+    n, m = x.shape
+
+    # Parse Inputs
+    if "v0" in param:
+        v0 = param["v0"]
+    else:
+        v0 = np.mean(np.var(x, 1)) * np.array([1, 1, 1])
+        param["v0"] = v0
+
+    if "mu0" in param:
+        mu0 = param["mu0"]
+    else:
+        mu0 = np.mean(x, 1)
+        param["mu0"] = mu0
+
+    if "a0" in param:
+        a0 = param["a0"]
+    else:
+        a0 = np.ones(m)
+        param["a0"] = a0
+
+    if "eta0" in param:
+        eta0 = param["eta0"]
+    else:
+        eta0 = np.zeros(m)
+        param["eta0"] = eta0
+
+    if "ts" in param:
+        param["ts"]
+    else:
+        param["ts"] = 1
+
+    mle = {"x0": np.array([])}
+    idxstart = 0
+    idxrange = {}
+
+    # If fix['logv'], return log(v0); otherwise return logv parameters
+    if fix["logv"]:
+
+        def setplogv(_):
+            return np.log(param["v0"])
+
+    else:
+        mle["x0"] = np.concatenate((mle["x0"], np.log(param["v0"])))
+        idxend = idxstart + 3
+        idxrange["logv"] = np.arange(idxstart, idxend)
+
+        def setplogv(_p):
+            return _p[idxrange["logv"]]
+
+        idxstart = idxend
+    pass
+
+    # If Fix['mu'], return mu0, otherwise, return mu parameters
+    if fix["mu"]:
+
+        def setpmu(_):
+            return param["mu0"]
+
+    else:
+        mle["x0"] = np.concatenate((mle["x0"], param["mu0"]))
+        idxend = idxstart + n
+        idxrange["mu"] = np.arange(idxstart, idxend)
+
+        def setpmu(_p):
+            return _p[idxrange["mu"]]
+
+        idxstart = idxend
+    pass
+
+    # If ignore A, return []; if Fix['A'], return A0; if ~Fix.A & Fix.mu,
+    # return all A parameters;
+    # If ~Fix.A & ~Fix.mu, return all A parameters but first
+
+    if ignore["a"]:
+
+        def setpa(_):
+            return []
+
+    elif fix["a"]:
+
+        def setpa(_):
+            return param["a0"]
+
+    elif fix["mu"]:
+        mle["x0"] = np.concatenate((mle["x0"], param["a0"]))
+        idxend = idxstart + m
+        idxrange["a"] = np.arange(idxstart, idxend)
+
+        def setpa(_p):
+            return _p[idxrange["a"]]
+
+        idxstart = idxend
+    else:
+        mle["x0"] = np.concatenate(
+            (mle["x0"], param["a0"][1:] / param["a0"][0])
+        )
+        idxend = idxstart + m - 1
+        idxrange["a"] = np.arange(idxstart, idxend)
+
+        def setpa(_p):
+            return np.concatenate(([1], _p[idxrange["a"]]), axis=0)
+
+        idxstart = idxend
+    pass
+
+    # If Ignore.eta, return []; if Fix.eta, return eta0; if ~Fix.eta &
+    # Fix.mu,return all eta parameters;
+    # if ~Fix.eta & ~Fix.mu, return all eta parameters but first
+
+    if ignore["eta"]:
+
+        def setpeta(_):
+            return []
+
+    elif fix["eta"]:
+
+        def setpeta(_):
+            return param["eta0"]
+
+    elif fix["mu"]:
+        mle["x0"] = np.concatenate((mle["x0"], param["eta0"]))
+        idxend = idxstart + m
+        idxrange["eta"] = np.arange(idxstart, idxend)
+
+        def setpeta(_p):
+            return _p[idxrange["eta"]]
+
+    else:
+        mle["x0"] = np.concatenate(
+            (mle["x0"], param["eta0"][1:] - param["eta0"][0])
+        )
+        idxend = idxstart + m - 1
+        idxrange["eta"] = np.arange(idxstart, idxend)
+
+        def setpeta(_p):
+            return np.concatenate(([0], _p[idxrange["eta"]]), axis=0)
+
+    pass
+
+    def fun(_, _w):
+        return -1j * _w
+
+    d = tdtf(fun, 0, n, param["ts"])
+
+    def parsein(_p):
+        return {
+            "logv": setplogv(_p),
+            "mu": setpmu(_p),
+            "a": setpa(_p),
+            "eta": setpeta(_p),
+            "ts": param["ts"],
+            "d": d,
+        }
+
+    def objective(_p):
+        return tdnll(x, parsein(_p), fix)[0]
+
+    def jacobian(_p):
+        return tdnll(x, parsein(_p), fix)[1]
+
+    mle["objective"] = objective
+    out = minimize(mle["objective"], mle["x0"], method="BFGS", jac=jacobian)
+
+    # The trust-region algorithm returns the Hessian for the next-to-last
+    # iterate, which may not be near the final point. To check, test for
+    # positive definiteness by attempting to Cholesky factorize it. If it
+    # returns an error, rerun the optimization with the quasi-Newton algorithm
+    # from the current optimal point.
+
+    try:
+        np.linalg.cholesky(np.linalg.inv(out.hess_inv))
+        hess = np.linalg.inv(out.hess_inv)
+    except np.linalg.LinAlgError:
+        print(
+            "Hessian returned by FMINUNC is not positive definite;\n"
+            "recalculating with quasi-Newton algorithm"
+        )
+
+        mle["x0"] = out.x
+        out2 = minimize(
+            mle["objective"], mle["x0"], method="BFGS", jac=jacobian
+        )
+        hess = np.linalg.inv(out2.hess_inv)
+
+    # Parse output
+    p = {}
+    idxrange = {}
+    idxstart = 0
+
+    if fix["logv"]:
+        p["var"] = param["v0"]
+    else:
+        idxend = idxstart + 3
+        idxrange["logv"] = np.arange(idxstart, idxend)
+        idxstart = idxend
+        p["var"] = np.exp(out.x[idxrange["logv"]])
+    pass
+
+    if fix["mu"]:
+        p["mu"] = param["mu0"]
+    else:
+        idxend = idxstart + n
+        idxrange["mu"] = np.arange(idxstart, idxend)
+        idxstart = idxend
+        p["mu"] = out.x[idxrange["mu"]]
+    pass
+
+    if ignore["a"] or fix["a"]:
+        p["a"] = param["a0"]
+    elif fix["mu"]:
+        idxend = idxstart + m
+        idxrange["a"] = np.arange(idxstart, idxend)
+        idxstart = idxend
+        p["a"] = out.x[idxrange["a"]]
+    else:
+        idxend = idxstart + m - 1
+        idxrange["a"] = np.arange(idxstart, idxend)
+        idxstart = idxend
+        p["a"] = np.concatenate(([1], out.x[idxrange["a"]]), axis=0)
+    pass
+
+    if ignore["eta"] or fix["eta"]:
+        p["eta"] = param["eta0"]
+    elif fix["mu"]:
+        idxend = idxstart + m
+        idxrange["eta"] = np.arange(idxstart, idxend)
+        p["eta"] = out.x[idxrange["eta"]]
+    else:
+        idxend = idxstart + m - 1
+        idxrange["eta"] = np.arange(idxstart, idxend)
+        p["eta"] = np.concatenate(([0], out.x[idxrange["eta"]]), axis=0)
+    pass
+
+    p["ts"] = param["ts"]
+
+    vary_param = np.logical_not(
+        [
+            fix["logv"],
+            fix["mu"],
+            fix["a"] or ignore["a"],
+            fix["eta"] or ignore["eta"],
+        ]
+    )
+    diagnostic = {
+        "grad": out.jac,
+        "hessian": hess,
+        "err": {"var": [], "mu": [], "a": [], "eta": []},
+    }
+    v = np.dot(np.eye(hess.shape[0]), scipy.linalg.inv(hess))
+    err = np.sqrt(np.diag(v))
+    idxstart = 0
+    if vary_param[0]:
+        diagnostic["err"]["var"] = np.sqrt(
+            np.diag(np.diag(p["var"]) * v[0:3, 0:3]) * np.diag(p["var"])
+        )
+        idxstart = idxstart + 3
+    pass
+
+    if vary_param[1]:
+        diagnostic["err"]["mu"] = err[idxstart: idxstart + n]
+        idxstart = idxstart + n
+    pass
+
+    if vary_param[2]:
+        if vary_param[1]:
+            diagnostic["err"]["a"] = err[idxstart: idxstart + m - 1]
+            idxstart = idxstart + m - 1
+        else:
+            diagnostic["err"]["a"] = err[idxstart: idxstart + m]
+            idxstart = idxstart + m
+    pass
+
+    if vary_param[3]:
+        if vary_param[1]:
+            diagnostic["err"]["eta"] = err[idxstart: idxstart + m - 1]
+        else:
+            diagnostic["err"]["eta"] = err[idxstart: idxstart + m]
+    pass
+
+    return [p, out.fun, diagnostic]
```

### Comparing `thztools-0.0.1/.gitignore` & `thztools-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/LICENSE` & `thztools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thztools-0.0.1/pyproject.toml` & `thztools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "jupyter",
     "matplotlib",
     "pandas",
     "scipy",
 ]
 
 [project.urls]
-Documentation = "https://pages.github.com/dodge-research-group/thztools"
+Documentation = "https://dodge-research-group.github.io/thztools/"
 Issues = "https://github.com/dodge-research-group/thztools/issues"
 Source = "https://github.com/dodge-research-group/thztools"
 
 [tool.hatch.version]
 path = "src/thztools/__about__.py"
 
 [tool.hatch.envs.default]
```

