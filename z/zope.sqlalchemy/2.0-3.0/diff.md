# Comparing `tmp/zope.sqlalchemy-2.0.tar.gz` & `tmp/zope.sqlalchemy-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.sqlalchemy-2.0.tar", last modified: Mon Feb  6 10:40:54 2023, max compression
+gzip compressed data, was "zope.sqlalchemy-3.0.tar", last modified: Thu Jun  1 15:51:26 2023, max compression
```

## Comparing `zope.sqlalchemy-2.0.tar` & `zope.sqlalchemy-3.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-06 10:40:54.020796 zope.sqlalchemy-2.0/
--rw-r--r--   0 mac        (513) staff       (20)     7499 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      805 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)      342 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/CREDITS.rst
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      331 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    17296 2023-02-06 10:40:54.020957 zope.sqlalchemy-2.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      264 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      265 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      236 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/github_actions.cfg
--rw-r--r--   0 mac        (513) staff       (20)      274 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/mysql.cfg
--rw-r--r--   0 mac        (513) staff       (20)      845 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/oracle.cfg
--rw-r--r--   0 mac        (513) staff       (20)      686 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/postgres.cfg
--rw-r--r--   0 mac        (513) staff       (20)      436 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/pysqlite.cfg
--rw-r--r--   0 mac        (513) staff       (20)      473 2023-02-06 10:40:54.021714 zope.sqlalchemy-2.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     1912 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-06 10:40:54.009672 zope.sqlalchemy-2.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-06 10:40:54.014981 zope.sqlalchemy-2.0/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       56 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-06 10:40:54.020491 zope.sqlalchemy-2.0/src/zope/sqlalchemy/
--rw-r--r--   0 mac        (513) staff       (20)     8663 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope/sqlalchemy/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      926 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope/sqlalchemy/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)    12905 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope/sqlalchemy/datamanager.py
--rw-r--r--   0 mac        (513) staff       (20)    26910 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope/sqlalchemy/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-06 10:40:54.018788 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    17296 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      650 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      148 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     2398 2023-02-06 10:40:53.000000 zope.sqlalchemy-2.0/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-01 15:51:26.964730 zope.sqlalchemy-3.0/
+-rw-r--r--   0 mac        (513) staff       (20)     8270 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      805 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)      342 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/CREDITS.rst
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      383 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)    18143 2023-06-01 15:51:26.964886 zope.sqlalchemy-3.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      264 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      265 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      245 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/github_actions.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      339 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/github_actions20.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      274 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/mysql.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      845 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/oracle.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      687 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/postgres.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      652 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/postgres20.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      436 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/pysqlite.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      473 2023-06-01 15:51:26.965640 zope.sqlalchemy-3.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     1930 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-01 15:51:26.954901 zope.sqlalchemy-3.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-01 15:51:26.960729 zope.sqlalchemy-3.0/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-01 15:51:26.964410 zope.sqlalchemy-3.0/src/zope/sqlalchemy/
+-rw-r--r--   0 mac        (513) staff       (20)     8739 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope/sqlalchemy/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      926 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope/sqlalchemy/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    13224 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope/sqlalchemy/datamanager.py
+-rw-r--r--   0 mac        (513) staff       (20)    29217 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope/sqlalchemy/tests.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-06-01 15:51:26.963139 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)    18143 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      686 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      155 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     3109 2023-06-01 15:51:26.000000 zope.sqlalchemy-3.0/tox.ini
```

### Comparing `zope.sqlalchemy-2.0/CHANGES.rst` & `zope.sqlalchemy-3.0/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 Changes
 =======
 
+3.0 (2023-06-01)
+----------------
+
+- Add support for SQLAlchemy 2.0 and for new psycopg v3 backend.
+  (`#79 <https://github.com/zopefoundation/zope.sqlalchemy/pull/79>`_)
+
+**Breaking Changes**
+
+- No longer allow calling ``session.commit()`` within a manual nested database
+  transaction (a savepoint). If you want to use savepoints directly in code that is
+  not aware of ``transaction.savepoint()`` with ``session.begin_nested()`` then
+  use the savepoint returned by the function to commit just the nested transaction
+  i.e. ``savepoint = session.begin_nested(); savepoint.commit()`` or use it as a
+  context manager i.e. ``with session.begin_nested():``.
+  (`for details see #79 <https://github.com/zopefoundation/zope.sqlalchemy/pull/79#issuecomment-1516069841>`_)
+
+
 2.0 (2023-02-06)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Drop support for ``SQLAlchemy < 1.1``
   (`#65 <https://github.com/zopefoundation/zope.sqlalchemy/issues/65>`_)
```

### Comparing `zope.sqlalchemy-2.0/CONTRIBUTING.md` & `zope.sqlalchemy-3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.sqlalchemy-2.0/LICENSE.txt` & `zope.sqlalchemy-3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.sqlalchemy-2.0/PKG-INFO` & `zope.sqlalchemy-3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.sqlalchemy
-Version: 2.0
+Version: 3.0
 Summary: Minimal Zope/SQLAlchemy transaction integration
 Home-page: https://github.com/zopefoundation/zope.sqlalchemy
 Author: Laurence Rowe
 Author-email: laurence@lrowe.co.uk
 License: ZPL 2.1
 Keywords: zope zope3 sqlalchemy
 Classifier: Development Status :: 5 - Production/Stable
@@ -105,43 +105,44 @@
 
 Instantiated sessions commits and rollbacks will now be integrated with Zope
 transactions.
 
 .. code-block:: python
 
     import transaction
+    from sqlalchemy.sql import text
 
     session = DBSession()
 
-    result = session.execute("DELETE FROM objects WHERE id=:id", {"id": 2})
+    result = session.execute(text("DELETE FROM objects WHERE id=:id"), {"id": 2})
     row = result.fetchone()
 
     transaction.commit()
 
 
 Full Example
 ============
 
 This example is lifted directly from the SQLAlchemy declarative documentation.
 First the necessary imports.
 
     >>> from sqlalchemy import *
-    >>> from sqlalchemy.ext.declarative import declarative_base
-    >>> from sqlalchemy.orm import scoped_session, sessionmaker, relation
+    >>> from sqlalchemy.orm import declarative_base, scoped_session, sessionmaker, relationship
+    >>> from sqlalchemy.sql import text
     >>> from zope.sqlalchemy import register
     >>> import transaction
 
 Now to define the mapper classes.
 
     >>> Base = declarative_base()
     >>> class User(Base):
     ...     __tablename__ = 'test_users'
     ...     id = Column('id', Integer, primary_key=True)
     ...     name = Column('name', String(50))
-    ...     addresses = relation("Address", backref="user")
+    ...     addresses = relationship("Address", backref="user")
     >>> class Address(Base):
     ...     __tablename__ = 'test_addresses'
     ...     id = Column('id', Integer, primary_key=True)
     ...     email = Column('email', String(50))
     ...     user_id = Column('user_id', Integer, ForeignKey('test_users.id'))
 
 Create an engine and setup the tables. Note that for this example to work a
@@ -171,15 +172,15 @@
 machinery, just as Zope's publisher would.
 
     >>> session.add(User(id=1, name='bob'))
     >>> transaction.commit()
 
 Engine level connections are outside the scope of the transaction integration.
 
-    >>> engine.connect().execute('SELECT * FROM test_users').fetchall()
+    >>> engine.connect().execute(text('SELECT * FROM test_users')).fetchall()
     [(1, ...'bob')]
 
 A new transaction requires a new session. Let's add an address.
 
     >>> session = Session()
     >>> bob = session.query(User).all()[0]
     >>> str(bob.name)
@@ -212,15 +213,15 @@
 possible to guess whether such an operation is a read or a write. Therefore we
 must manually mark the session as changed when manual SQL statements write
 to the DB.
 
     >>> session = Session()
     >>> conn = session.connection()
     >>> users = Base.metadata.tables['test_users']
-    >>> conn.execute(users.update(users.c.name=='bob'), name='ben')
+    >>> conn.execute(users.update().where(users.c.name=='bob'), {'name': 'ben'})
     <sqlalchemy.engine... object at ...>
     >>> from zope.sqlalchemy import mark_changed
     >>> mark_changed(session)
     >>> transaction.commit()
     >>> session = Session()
     >>> str(session.query(User).all()[0].name)
     'ben'
@@ -230,15 +231,15 @@
 session in the 'changed' state initially.
 
     >>> Session.remove()
     >>> register(Session, 'changed')
     <zope.sqlalchemy.datamanager.ZopeTransactionEvents object at ...>
     >>> session = Session()
     >>> conn = session.connection()
-    >>> conn.execute(users.update(users.c.name=='ben'), name='bob')
+    >>> conn.execute(users.update().where(users.c.name=='ben'), {'name': 'bob'})
     <sqlalchemy.engine... object at ...>
     >>> transaction.commit()
     >>> session = Session()
     >>> str(session.query(User).all()[0].name)
     'bob'
     >>> transaction.abort()
 
@@ -295,14 +296,31 @@
 
 `GIT version <https://github.com/zopefoundation/zope.sqlalchemy>`_
 
 
 Changes
 =======
 
+3.0 (2023-06-01)
+----------------
+
+- Add support for SQLAlchemy 2.0 and for new psycopg v3 backend.
+  (`#79 <https://github.com/zopefoundation/zope.sqlalchemy/pull/79>`_)
+
+**Breaking Changes**
+
+- No longer allow calling ``session.commit()`` within a manual nested database
+  transaction (a savepoint). If you want to use savepoints directly in code that is
+  not aware of ``transaction.savepoint()`` with ``session.begin_nested()`` then
+  use the savepoint returned by the function to commit just the nested transaction
+  i.e. ``savepoint = session.begin_nested(); savepoint.commit()`` or use it as a
+  context manager i.e. ``with session.begin_nested():``.
+  (`for details see #79 <https://github.com/zopefoundation/zope.sqlalchemy/pull/79#issuecomment-1516069841>`_)
+
+
 2.0 (2023-02-06)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Drop support for ``SQLAlchemy < 1.1``
   (`#65 <https://github.com/zopefoundation/zope.sqlalchemy/issues/65>`_)
```

### Comparing `zope.sqlalchemy-2.0/oracle.cfg` & `zope.sqlalchemy-3.0/oracle.cfg`

 * *Files identical despite different names*

### Comparing `zope.sqlalchemy-2.0/postgres.cfg` & `zope.sqlalchemy-3.0/postgres.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,25 @@
 [buildout]
 extends = buildout.cfg
 find-links = http://initd.org/pub/software/psycopg/
 parts +=
     testpg
     testpg2
 
-[test]
-eggs += psycopg2
-
 [testpg]
 <= test
+eggs += psycopg2
 environment = pgenv
 
 [testpg2]
 <= testpg
 environment = pgenv2
 
 [scripts]
 eggs += psycopg2
 
 [pgenv]
-TEST_DSN = postgresql:///zope_sqlalchemy_tests
+TEST_DSN = postgresql+psycopg2:///zope_sqlalchemy_tests
 
 [pgenv2]
 <= pgenv
 TEST_TWOPHASE=True
```

### Comparing `zope.sqlalchemy-2.0/setup.py` & `zope.sqlalchemy-3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 
 tests_require = ['zope.testing']
 
 setup(
     name='zope.sqlalchemy',
-    version='2.0',
+    version='3.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     namespace_packages=['zope'],
     test_suite='zope.sqlalchemy.tests.test_suite',
     author='Laurence Rowe',
@@ -42,15 +42,16 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Database",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires='>=3.7',
     install_requires=[
+        'packaging',
         'setuptools',
-        'SQLAlchemy>=1.1,!=1.4.0,!=1.4.1,!=1.4.2,!=1.4.3,!=1.4.4,!=1.4.5,!=1.4.6,<2',  # noqa: E501 line too long
+        'SQLAlchemy>=1.1,!=1.4.0,!=1.4.1,!=1.4.2,!=1.4.3,!=1.4.4,!=1.4.5,!=1.4.6',  # noqa: E501 line too long
         'transaction>=1.6.0',
         'zope.interface>=3.6.0',
     ],
     extras_require={'test': tests_require},
     tests_require=tests_require,
 )
```

### Comparing `zope.sqlalchemy-2.0/src/zope/sqlalchemy/README.rst` & `zope.sqlalchemy-3.0/src/zope/sqlalchemy/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -76,43 +76,44 @@
 
 Instantiated sessions commits and rollbacks will now be integrated with Zope
 transactions.
 
 .. code-block:: python
 
     import transaction
+    from sqlalchemy.sql import text
 
     session = DBSession()
 
-    result = session.execute("DELETE FROM objects WHERE id=:id", {"id": 2})
+    result = session.execute(text("DELETE FROM objects WHERE id=:id"), {"id": 2})
     row = result.fetchone()
 
     transaction.commit()
 
 
 Full Example
 ============
 
 This example is lifted directly from the SQLAlchemy declarative documentation.
 First the necessary imports.
 
     >>> from sqlalchemy import *
-    >>> from sqlalchemy.ext.declarative import declarative_base
-    >>> from sqlalchemy.orm import scoped_session, sessionmaker, relation
+    >>> from sqlalchemy.orm import declarative_base, scoped_session, sessionmaker, relationship
+    >>> from sqlalchemy.sql import text
     >>> from zope.sqlalchemy import register
     >>> import transaction
 
 Now to define the mapper classes.
 
     >>> Base = declarative_base()
     >>> class User(Base):
     ...     __tablename__ = 'test_users'
     ...     id = Column('id', Integer, primary_key=True)
     ...     name = Column('name', String(50))
-    ...     addresses = relation("Address", backref="user")
+    ...     addresses = relationship("Address", backref="user")
     >>> class Address(Base):
     ...     __tablename__ = 'test_addresses'
     ...     id = Column('id', Integer, primary_key=True)
     ...     email = Column('email', String(50))
     ...     user_id = Column('user_id', Integer, ForeignKey('test_users.id'))
 
 Create an engine and setup the tables. Note that for this example to work a
@@ -142,15 +143,15 @@
 machinery, just as Zope's publisher would.
 
     >>> session.add(User(id=1, name='bob'))
     >>> transaction.commit()
 
 Engine level connections are outside the scope of the transaction integration.
 
-    >>> engine.connect().execute('SELECT * FROM test_users').fetchall()
+    >>> engine.connect().execute(text('SELECT * FROM test_users')).fetchall()
     [(1, ...'bob')]
 
 A new transaction requires a new session. Let's add an address.
 
     >>> session = Session()
     >>> bob = session.query(User).all()[0]
     >>> str(bob.name)
@@ -183,15 +184,15 @@
 possible to guess whether such an operation is a read or a write. Therefore we
 must manually mark the session as changed when manual SQL statements write
 to the DB.
 
     >>> session = Session()
     >>> conn = session.connection()
     >>> users = Base.metadata.tables['test_users']
-    >>> conn.execute(users.update(users.c.name=='bob'), name='ben')
+    >>> conn.execute(users.update().where(users.c.name=='bob'), {'name': 'ben'})
     <sqlalchemy.engine... object at ...>
     >>> from zope.sqlalchemy import mark_changed
     >>> mark_changed(session)
     >>> transaction.commit()
     >>> session = Session()
     >>> str(session.query(User).all()[0].name)
     'ben'
@@ -201,15 +202,15 @@
 session in the 'changed' state initially.
 
     >>> Session.remove()
     >>> register(Session, 'changed')
     <zope.sqlalchemy.datamanager.ZopeTransactionEvents object at ...>
     >>> session = Session()
     >>> conn = session.connection()
-    >>> conn.execute(users.update(users.c.name=='ben'), name='bob')
+    >>> conn.execute(users.update().where(users.c.name=='ben'), {'name': 'bob'})
     <sqlalchemy.engine... object at ...>
     >>> transaction.commit()
     >>> session = Session()
     >>> str(session.query(User).all()[0].name)
     'bob'
     >>> transaction.abort()
```

### Comparing `zope.sqlalchemy-2.0/src/zope/sqlalchemy/__init__.py` & `zope.sqlalchemy-3.0/src/zope/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.sqlalchemy-2.0/src/zope/sqlalchemy/datamanager.py` & `zope.sqlalchemy-3.0/src/zope/sqlalchemy/datamanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # FOR A PARTICULAR PURPOSE
 #
 ##############################################################################
 
 
 from weakref import WeakKeyDictionary
 
-from pkg_resources import parse_version
-
 import transaction as zope_transaction
+from packaging.version import Version as parse_version
 from sqlalchemy import __version__ as sqlalchemy_version
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.orm.exc import ConcurrentModificationError
 from transaction._transaction import Status as ZopeStatus
 from transaction.interfaces import IDataManagerSavepoint
 from transaction.interfaces import ISavepointDataManager
@@ -33,14 +32,26 @@
     import psycopg2.extensions
 except ImportError:
     pass
 else:
     _retryable_errors.append(
         (psycopg2.extensions.TransactionRollbackError, None))
 
+# Error Class 40: Transaction Rollback, for details
+# see https://www.psycopg.org/psycopg3/docs/api/errors.html
+try:
+    import psycopg.errors
+except ImportError:
+    pass
+else:
+    _retryable_errors.append(
+        (psycopg.errors.OperationalError,
+         lambda e: e.sqlstate.startswith('40'))
+    )
+
 # ORA-08177: can't serialize access for this transaction
 try:
     import cx_Oracle
 except ImportError:
     pass
 else:
     _retryable_errors.append(
```

### Comparing `zope.sqlalchemy-2.0/src/zope/sqlalchemy/tests.py` & `zope.sqlalchemy-3.0/src/zope/sqlalchemy/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,24 +27,27 @@
 import os
 import threading
 import time
 import unittest
 
 import sqlalchemy as sa
 import transaction
+from packaging.version import Version as parse_version
+from sqlalchemy import __version__ as sqlalchemy_version
 from sqlalchemy import exc
 from sqlalchemy import orm
 from sqlalchemy import sql
 from transaction._transaction import Status as ZopeStatus
 from transaction.interfaces import TransactionFailedError
 
 from zope.sqlalchemy import datamanager as tx
 from zope.sqlalchemy import mark_changed
 
 
+SA_GE_20 = parse_version(sqlalchemy_version) >= parse_version('2.0.0')
 TEST_TWOPHASE = bool(os.environ.get("TEST_TWOPHASE"))
 TEST_DSN = os.environ.get("TEST_DSN", "sqlite:///:memory:")
 
 
 class SimpleModel:
     def __init__(self, **kw):
         for k, v in kw.items():
@@ -61,15 +64,14 @@
 
 
 class Skill(SimpleModel):
     pass
 
 
 engine = sa.create_engine(TEST_DSN)
-engine2 = sa.create_engine(TEST_DSN)
 
 # See https://code.google.com/p/pysqlite-static-env/
 HAS_PATCHED_PYSQLITE = False
 if engine.url.drivername == "sqlite":
     try:
         from pysqlite2.dbapi2 import Connection
     except ImportError:
@@ -123,53 +125,79 @@
     metadata,
     sa.Column("id", sa.Integer, primary_key=True),
     sa.Column("user_id", sa.Integer),
     sa.Column("name", sa.VARCHAR(255)),
     sa.ForeignKeyConstraint(("user_id",), ("test_users.id",)),
 )
 
-bound_metadata1 = sa.MetaData(engine)
-bound_metadata2 = sa.MetaData(engine2)
+if SA_GE_20:
+    # bound metadata does no longer exist in SQLAlchemy 2.0
+    test_one = sa.Table(
+        "test_one",
+        metadata,
+        sa.Column("id", sa.Integer, primary_key=True)
+    )
+    test_two = sa.Table(
+        "test_two",
+        metadata,
+        sa.Column("id", sa.Integer, primary_key=True)
+    )
+else:
+    engine2 = sa.create_engine(TEST_DSN)
 
-test_one = sa.Table(
-    "test_one", bound_metadata1, sa.Column("id", sa.Integer, primary_key=True)
-)
-test_two = sa.Table(
-    "test_two", bound_metadata2, sa.Column("id", sa.Integer, primary_key=True)
-)
+    bound_metadata1 = sa.MetaData(engine)
+    bound_metadata2 = sa.MetaData(engine2)
+
+    test_one = sa.Table(
+        "test_one",
+        bound_metadata1,
+        sa.Column("id", sa.Integer, primary_key=True)
+    )
+    test_two = sa.Table(
+        "test_two",
+        bound_metadata2,
+        sa.Column("id", sa.Integer, primary_key=True)
+    )
 
 
 class TestOne(SimpleModel):
     pass
 
 
 class TestTwo(SimpleModel):
     pass
 
 
 def setup_mappers():
     orm.clear_mappers()
     # Other tests can clear mappers by calling clear_mappers(),
     # be more robust by setting up mappers in the test setup.
-    m1 = orm.mapper(
+
+    if SA_GE_20:
+        mapper_reg = orm.registry()
+        mapper = mapper_reg.map_imperatively
+    else:
+        mapper = orm.mapper
+
+    m1 = mapper(
         User,
         test_users,
         properties={
-            "skills": orm.relation(
+            "skills": orm.relationship(
                 Skill,
                 primaryjoin=(
                     test_users.columns["id"] == test_skills.columns["user_id"]
                 ),
             )
         },
     )
-    m2 = orm.mapper(Skill, test_skills)
+    m2 = mapper(Skill, test_skills)
 
-    m3 = orm.mapper(TestOne, test_one)
-    m4 = orm.mapper(TestTwo, test_two)
+    m3 = mapper(TestOne, test_one)
+    m4 = mapper(TestTwo, test_two)
     return [m1, m2, m3, m4]
 
 
 class DummyException(Exception):
     pass
 
 
@@ -218,19 +246,22 @@
 
 
 class ZopeSQLAlchemyTests(unittest.TestCase):
     def setUp(self):
         self.mappers = setup_mappers()
         metadata.drop_all(engine)
         metadata.create_all(engine)
+        # a connection which bypasses the session/transaction machinery
+        self.conn = engine.connect()
 
     def tearDown(self):
         transaction.abort()
         metadata.drop_all(engine)
         orm.clear_mappers()
+        self.conn.close()
 
     def testMarkUnknownSession(self):
         import zope.sqlalchemy.datamanager
 
         DummyDataManager(key="dummy.first")
         session = Session()
         mark_changed(session)
@@ -249,15 +280,15 @@
             # But abort must succeed (and rollback the base connection)
             transaction.abort()
             pass
         # Or the next transaction will not be able to start!
         transaction.begin()
         session = Session()
         conn = session.connection()
-        conn.execute("SELECT 1 FROM test_users")
+        conn.execute(sql.text("SELECT 1 FROM test_users"))
         mark_changed(session)
         transaction.commit()
 
     def testAbortAfterCommit(self):
         # This is a regression test which used to wedge the transaction
         # machinery when using PostgreSQL (and perhaps other) connections.
         # Basically, if a commit failed, there was no way to abort the
@@ -276,15 +307,15 @@
             # But abort must succed (and actually rollback the base connection)
             transaction.abort()
             pass
         # Or the next transaction will not be able to start!
         transaction.begin()
         session = Session()
         conn = session.connection()
-        conn.execute("SELECT 1 FROM test_users")
+        conn.execute(sql.text("SELECT 1 FROM test_users"))
         mark_changed(session)
         transaction.commit()
 
     def testSimplePopulation(self):
         session = Session()
         query = session.query(User)
         rows = query.all()
@@ -298,15 +329,19 @@
         self.assertEqual(len(rows), 2)
         row1 = rows[0]
         d = row1.asDict()
         self.assertEqual(
             d, {"firstname": "udo", "lastname": "juergens", "id": 1})
 
         # bypass the session machinery
-        stmt = sql.select(test_users.columns).order_by("id")
+        if SA_GE_20:
+            stmt = sql.select(*test_users.columns).order_by("id")
+        else:
+            stmt = sql.select(test_users.columns).order_by("id")
+
         conn = session.connection()
         results = conn.execute(stmt)
         self.assertEqual(
             results.fetchall(), [(1, "udo", "juergens"), (2, "heino", "n/a")]
         )
 
     def testRelations(self):
@@ -379,15 +414,15 @@
 
         s1.rollback()
         self.assertFalse(query.all(), "Users table should be empty")
 
     def testRollbackAttributes(self):
         use_savepoint = engine.url.drivername not in tx.NO_SAVEPOINT_SUPPORT
         if not use_savepoint:
-            return  # sqlite databases do not support savepoints
+            self.skipTest('No savepoint support')
 
         t = transaction.get()
         session = Session()
         query = session.query(User)
         self.assertFalse(query.all(), "Users table should be empty")
 
         t.savepoint()
@@ -445,20 +480,21 @@
         self.assertEqual(len(rows), 2)
         row1 = rows[0]
         d = row1.asDict()
         self.assertEqual(
             d, {"firstname": "udo", "lastname": "juergens", "id": 1})
 
         # bypass the session (and transaction) machinery
-        results = engine.connect().execute(test_users.select())
-        self.assertEqual(len(results.fetchall()), 2)
+        with self.conn.begin():
+            results = self.conn.execute(test_users.select())
+            self.assertEqual(len(results.fetchall()), 2)
 
     def testCommitWithSavepoint(self):
         if engine.url.drivername in tx.NO_SAVEPOINT_SUPPORT:
-            return
+            self.skipTest('No savepoint support')
         session = Session()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         session.add(User(id=2, firstname="heino", lastname="n/a"))
         session.flush()
         transaction.commit()
 
         session = Session()
@@ -469,37 +505,38 @@
 
         t.savepoint()
         session.delete(rows[1])
         session.flush()
         transaction.commit()
 
         # bypass the session machinery
-        results = engine.connect().execute(test_users.select())
-        self.assertEqual(len(results.fetchall()), 1)
+        with self.conn.begin():
+            results = self.conn.execute(test_users.select())
+            self.assertEqual(len(results.fetchall()), 1)
 
-    def testNestedSessionCommitAllowed(self):
+    def testSessionSavepointCommitAllowed(self):
         # Existing code might use nested transactions
         if engine.url.drivername in tx.NO_SAVEPOINT_SUPPORT:
-            return
+            self.skipTest('No save point support')
         session = Session()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
-        session.begin_nested()
+        savepoint = session.begin_nested()
         session.add(User(id=2, firstname="heino", lastname="n/a"))
-        session.commit()
+        savepoint.commit()
         transaction.commit()
 
     def testSessionCommitDisallowed(self):
         session = Session()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         self.assertRaises(AssertionError, session.commit)
 
     def testTwoPhase(self):
         session = Session()
         if not session.twophase:
-            return
+            self.skipTest('No two phase transaction support')
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         session.add(User(id=2, firstname="heino", lastname="n/a"))
         session.flush()
         transaction.commit()
 
         # Test that we clean up after a tpc_abort
         t = transaction.get()
@@ -577,53 +614,57 @@
         session = Session()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         session.add(User(id=2, firstname="heino", lastname="n/a"))
         transaction.commit()
         session = Session()
         session.query(User).delete()
         transaction.commit()
-        results = engine.connect().execute(test_users.select())
-        self.assertEqual(len(results.fetchall()), 0)
+        with self.conn.begin():
+            results = self.conn.execute(test_users.select())
+            self.assertEqual(len(results.fetchall()), 0)
 
     def testBulkUpdate(self):
         session = Session()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         session.add(User(id=2, firstname="heino", lastname="n/a"))
         transaction.commit()
         session = Session()
         session.query(User).update(dict(lastname="smith"))
         transaction.commit()
-        results = engine.connect().execute(
-            test_users.select(test_users.c.lastname == "smith")
-        )
-        self.assertEqual(len(results.fetchall()), 2)
+        with self.conn.begin():
+            results = self.conn.execute(
+                test_users.select().where(test_users.c.lastname == "smith")
+            )
+            self.assertEqual(len(results.fetchall()), 2)
 
     def testBulkDeleteUsingRegister(self):
         session = EventSession()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         session.add(User(id=2, firstname="heino", lastname="n/a"))
         transaction.commit()
         session = EventSession()
         session.query(User).delete()
         transaction.commit()
-        results = engine.connect().execute(test_users.select())
-        self.assertEqual(len(results.fetchall()), 0)
+        with self.conn.begin():
+            results = self.conn.execute(test_users.select())
+            self.assertEqual(len(results.fetchall()), 0)
 
     def testBulkUpdateUsingRegister(self):
         session = EventSession()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         session.add(User(id=2, firstname="heino", lastname="n/a"))
         transaction.commit()
         session = EventSession()
         session.query(User).update(dict(lastname="smith"))
         transaction.commit()
-        results = engine.connect().execute(
-            test_users.select(test_users.c.lastname == "smith")
-        )
-        self.assertEqual(len(results.fetchall()), 2)
+        with self.conn.begin():
+            results = self.conn.execute(
+                test_users.select().where(test_users.c.lastname == "smith")
+            )
+            self.assertEqual(len(results.fetchall()), 2)
 
     def testFailedJoin(self):
         # When a join is issued while the transaction is in COMMITFAILED, the
         # session is never closed and the session id stays in _SESSION_STATE,
         # which means the session won't be joined in the future either. This
         # causes the session to stay open forever, potentially accumulating
         # data, but never issuing a commit.
@@ -655,15 +696,18 @@
     def testKeepSession(self):
         session = KeepSession()
 
         try:
             with transaction.manager:
                 session.add(User(id=1, firstname="foo", lastname="bar"))
 
-            user = session.query(User).get(1)
+            if SA_GE_20:
+                user = session.get(User, 1)
+            else:
+                user = session.query(User).get(1)
 
             # if the keep_session works correctly, this transaction will not
             # close the session after commit
             with transaction.manager:
                 user.firstname = "super"
                 session.flush()
 
@@ -676,59 +720,73 @@
 
     def testExpireAll(self):
         session = Session()
         session.add(User(id=1, firstname="udo", lastname="juergens"))
         transaction.commit()
 
         session = Session()
-        instance = session.query(User).get(1)
+        if SA_GE_20:
+            instance = session.get(User, 1)
+        else:
+            instance = session.query(User).get(1)
         transaction.commit()  # No work, session.close()
 
         self.assertEqual(sa.inspect(instance).expired, True)
 
 
 class RetryTests(unittest.TestCase):
     def setUp(self):
         self.mappers = setup_mappers()
         metadata.drop_all(engine)
         metadata.create_all(engine)
         self.tm1 = transaction.TransactionManager()
         self.tm2 = transaction.TransactionManager()
         # With psycopg2 you might supply isolation_level='SERIALIZABLE' here,
         # unfortunately that is not supported by cx_Oracle.
-        e1 = sa.create_engine(TEST_DSN)
-        e2 = sa.create_engine(TEST_DSN)
-        self.s1 = orm.sessionmaker(bind=e1, twophase=TEST_TWOPHASE)()
+        self.e1 = sa.create_engine(TEST_DSN)
+        self.e2 = sa.create_engine(TEST_DSN)
+        self.s1 = orm.sessionmaker(bind=self.e1, twophase=TEST_TWOPHASE)()
         tx.register(self.s1, transaction_manager=self.tm1)
-        self.s2 = orm.sessionmaker(bind=e2, twophase=TEST_TWOPHASE)()
+        self.s2 = orm.sessionmaker(bind=self.e2, twophase=TEST_TWOPHASE)()
         tx.register(self.s2, transaction_manager=self.tm2)
         self.tm1.begin()
         self.s1.add(User(id=1, firstname="udo", lastname="juergens"))
         self.tm1.commit()
 
     def tearDown(self):
         self.tm1.abort()
         self.tm2.abort()
         metadata.drop_all(engine)
         orm.clear_mappers()
+        # ensure any open connections on the temporary engines get closed
+        # if we don't do this we get a `ResourceWarning` in psycopg v3
+        self.e1.dispose()
+        self.e2.dispose()
+        self.e1 = None
+        self.e2 = None
+        self.s1 = None
+        self.s2 = None
 
     def testRetry(self):
         # sqlite is unable to run this test as the databse is locked
         tm1, tm2, s1, s2 = self.tm1, self.tm2, self.s1, self.s2
         # make sure we actually start a session.
         tm1.begin()
         self.assertTrue(
             len(s1.query(User).all()) == 1, "Users table should have one row"
         )
         tm2.begin()
         self.assertTrue(
             len(s2.query(User).all()) == 1, "Users table should have one row"
         )
         s1.query(User).delete()
-        user = s2.query(User).get(1)
+        if SA_GE_20:
+            user = s2.get(User, 1)
+        else:
+            user = s2.query(User).get(1)
         user.lastname = "smith"
         tm1.commit()
         raised = False
         try:
             s2.flush()
         except orm.exc.ConcurrentModificationError as e:
             # This error is thrown when the number of updated rows is not as
@@ -742,41 +800,51 @@
         tm1, tm2, s1, s2 = self.tm1, self.tm2, self.s1, self.s2
         # make sure we actually start a session.
         tm1.begin()
         self.assertTrue(
             len(s1.query(User).all()) == 1, "Users table should have one row"
         )
         tm2.begin()
-        s2.connection().execute("SET TRANSACTION ISOLATION LEVEL SERIALIZABLE")
+        s2.connection().execute(sql.text(
+            "SET TRANSACTION ISOLATION LEVEL SERIALIZABLE"
+        ))
         self.assertTrue(
             len(s2.query(User).all()) == 1, "Users table should have one row"
         )
         s1.query(User).delete()
         raised = False
 
         def target():
             time.sleep(0.2)
             tm1.commit()
 
         thread = threading.Thread(target=target)
         thread.start()
         try:
-            s2.query(User).with_for_update().get(1)
+            if SA_GE_20:
+                s2.query(User).with_for_update().filter(User.id == 1).one()
+            else:
+                s2.query(User).with_for_update().get(1)
         except exc.DBAPIError as e:
             # This error wraps the underlying DBAPI module error, some of which
             # are retryable
             raised = True
             retryable = tm2._retryable(type(e), e)
             self.assertTrue(retryable, "Error should be retryable")
         self.assertTrue(raised, "Did not raise expected error")
         thread.join()  # well, we must have joined by now
 
 
 class MultipleEngineTests(unittest.TestCase):
     def setUp(self):
+        if SA_GE_20:
+            self.skipTest(
+                'Bound metadata is not supported in SQLAlchemy 2.0'
+            )
+
         self.mappers = setup_mappers()
         bound_metadata1.drop_all()
         bound_metadata1.create_all()
         bound_metadata2.drop_all()
         bound_metadata2.create_all()
 
     def tearDown(self):
@@ -811,16 +879,19 @@
 
     optionflags = doctest.NORMALIZE_WHITESPACE | doctest.ELLIPSIS
     suite = TestSuite()
     suite.addTest(makeSuite(ZopeSQLAlchemyTests))
     suite.addTest(makeSuite(MultipleEngineTests))
     if TEST_DSN.startswith("postgres") or TEST_DSN.startswith("oracle"):
         suite.addTest(makeSuite(RetryTests))
-    suite.addTest(
-        doctest.DocFileSuite(
-            "README.rst",
-            optionflags=optionflags,
-            tearDown=tearDownReadMe,
-            globs={"TEST_DSN": TEST_DSN, "TEST_TWOPHASE": TEST_TWOPHASE},
+
+    # examples in docs are only correct for SQLAlchemy >=1.4
+    if parse_version(sqlalchemy_version) >= parse_version('1.4.0'):
+        suite.addTest(
+            doctest.DocFileSuite(
+                "README.rst",
+                optionflags=optionflags,
+                tearDown=tearDownReadMe,
+                globs={"TEST_DSN": TEST_DSN, "TEST_TWOPHASE": TEST_TWOPHASE},
+            )
         )
-    )
     return suite
```

### Comparing `zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/PKG-INFO` & `zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.sqlalchemy
-Version: 2.0
+Version: 3.0
 Summary: Minimal Zope/SQLAlchemy transaction integration
 Home-page: https://github.com/zopefoundation/zope.sqlalchemy
 Author: Laurence Rowe
 Author-email: laurence@lrowe.co.uk
 License: ZPL 2.1
 Keywords: zope zope3 sqlalchemy
 Classifier: Development Status :: 5 - Production/Stable
@@ -105,43 +105,44 @@
 
 Instantiated sessions commits and rollbacks will now be integrated with Zope
 transactions.
 
 .. code-block:: python
 
     import transaction
+    from sqlalchemy.sql import text
 
     session = DBSession()
 
-    result = session.execute("DELETE FROM objects WHERE id=:id", {"id": 2})
+    result = session.execute(text("DELETE FROM objects WHERE id=:id"), {"id": 2})
     row = result.fetchone()
 
     transaction.commit()
 
 
 Full Example
 ============
 
 This example is lifted directly from the SQLAlchemy declarative documentation.
 First the necessary imports.
 
     >>> from sqlalchemy import *
-    >>> from sqlalchemy.ext.declarative import declarative_base
-    >>> from sqlalchemy.orm import scoped_session, sessionmaker, relation
+    >>> from sqlalchemy.orm import declarative_base, scoped_session, sessionmaker, relationship
+    >>> from sqlalchemy.sql import text
     >>> from zope.sqlalchemy import register
     >>> import transaction
 
 Now to define the mapper classes.
 
     >>> Base = declarative_base()
     >>> class User(Base):
     ...     __tablename__ = 'test_users'
     ...     id = Column('id', Integer, primary_key=True)
     ...     name = Column('name', String(50))
-    ...     addresses = relation("Address", backref="user")
+    ...     addresses = relationship("Address", backref="user")
     >>> class Address(Base):
     ...     __tablename__ = 'test_addresses'
     ...     id = Column('id', Integer, primary_key=True)
     ...     email = Column('email', String(50))
     ...     user_id = Column('user_id', Integer, ForeignKey('test_users.id'))
 
 Create an engine and setup the tables. Note that for this example to work a
@@ -171,15 +172,15 @@
 machinery, just as Zope's publisher would.
 
     >>> session.add(User(id=1, name='bob'))
     >>> transaction.commit()
 
 Engine level connections are outside the scope of the transaction integration.
 
-    >>> engine.connect().execute('SELECT * FROM test_users').fetchall()
+    >>> engine.connect().execute(text('SELECT * FROM test_users')).fetchall()
     [(1, ...'bob')]
 
 A new transaction requires a new session. Let's add an address.
 
     >>> session = Session()
     >>> bob = session.query(User).all()[0]
     >>> str(bob.name)
@@ -212,15 +213,15 @@
 possible to guess whether such an operation is a read or a write. Therefore we
 must manually mark the session as changed when manual SQL statements write
 to the DB.
 
     >>> session = Session()
     >>> conn = session.connection()
     >>> users = Base.metadata.tables['test_users']
-    >>> conn.execute(users.update(users.c.name=='bob'), name='ben')
+    >>> conn.execute(users.update().where(users.c.name=='bob'), {'name': 'ben'})
     <sqlalchemy.engine... object at ...>
     >>> from zope.sqlalchemy import mark_changed
     >>> mark_changed(session)
     >>> transaction.commit()
     >>> session = Session()
     >>> str(session.query(User).all()[0].name)
     'ben'
@@ -230,15 +231,15 @@
 session in the 'changed' state initially.
 
     >>> Session.remove()
     >>> register(Session, 'changed')
     <zope.sqlalchemy.datamanager.ZopeTransactionEvents object at ...>
     >>> session = Session()
     >>> conn = session.connection()
-    >>> conn.execute(users.update(users.c.name=='ben'), name='bob')
+    >>> conn.execute(users.update().where(users.c.name=='ben'), {'name': 'bob'})
     <sqlalchemy.engine... object at ...>
     >>> transaction.commit()
     >>> session = Session()
     >>> str(session.query(User).all()[0].name)
     'bob'
     >>> transaction.abort()
 
@@ -295,14 +296,31 @@
 
 `GIT version <https://github.com/zopefoundation/zope.sqlalchemy>`_
 
 
 Changes
 =======
 
+3.0 (2023-06-01)
+----------------
+
+- Add support for SQLAlchemy 2.0 and for new psycopg v3 backend.
+  (`#79 <https://github.com/zopefoundation/zope.sqlalchemy/pull/79>`_)
+
+**Breaking Changes**
+
+- No longer allow calling ``session.commit()`` within a manual nested database
+  transaction (a savepoint). If you want to use savepoints directly in code that is
+  not aware of ``transaction.savepoint()`` with ``session.begin_nested()`` then
+  use the savepoint returned by the function to commit just the nested transaction
+  i.e. ``savepoint = session.begin_nested(); savepoint.commit()`` or use it as a
+  context manager i.e. ``with session.begin_nested():``.
+  (`for details see #79 <https://github.com/zopefoundation/zope.sqlalchemy/pull/79#issuecomment-1516069841>`_)
+
+
 2.0 (2023-02-06)
 ----------------
 
 - Drop support for Python 2.7, 3.5, 3.6.
 
 - Drop support for ``SQLAlchemy < 1.1``
   (`#65 <https://github.com/zopefoundation/zope.sqlalchemy/issues/65>`_)
```

### Comparing `zope.sqlalchemy-2.0/src/zope.sqlalchemy.egg-info/SOURCES.txt` & `zope.sqlalchemy-3.0/src/zope.sqlalchemy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 COPYRIGHT.txt
 CREDITS.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 buildout.cfg
 github_actions.cfg
+github_actions20.cfg
 mysql.cfg
 oracle.cfg
 postgres.cfg
+postgres20.cfg
 pysqlite.cfg
 setup.cfg
 setup.py
 tox.ini
 src/zope/__init__.py
 src/zope.sqlalchemy.egg-info/PKG-INFO
 src/zope.sqlalchemy.egg-info/SOURCES.txt
```

### Comparing `zope.sqlalchemy-2.0/tox.ini` & `zope.sqlalchemy-3.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -8,34 +8,40 @@
     py38
     py39
     py310
     py311
     coverage
     py{37,38,39}-sqlalchemy11
     py{37,38,39,310}-sqlalchemy{12,13}
-    py{37,38,39,310,311}-sqlalchemy{14}
+    py{37,38,39,310,311}-sqlalchemy{14,20}
 
 [testenv]
 skip_install = true
 deps =
     zc.buildout >= 3.0.1
     wheel > 0.37
     sqlalchemy11: SQLAlchemy==1.1.*
     sqlalchemy12: SQLAlchemy==1.2.*
     sqlalchemy13: SQLAlchemy==1.3.*
     sqlalchemy14: SQLAlchemy==1.4.*
+    sqlalchemy20: SQLAlchemy==2.0.*
 commands_pre =
-    sh -c 'if [ '{env:CI:false}' = 'true' ]; then {envbindir}/buildout -nc {toxinidir}/github_actions.cfg buildout:directory={envdir} buildout:develop={toxinidir} ; fi'
-    sh -c 'if [ '{env:CI:false}' != 'true' ]; then {envbindir}/buildout -nc {toxinidir}/postgres.cfg buildout:directory={envdir} buildout:develop={toxinidir} ; fi'
+    !sqlalchemy20: sh -c 'if [ '{env:CI:false}' = 'true' ]; then {envbindir}/buildout -nc {toxinidir}/github_actions.cfg buildout:directory={envdir} buildout:develop={toxinidir} ; fi'
+    !sqlalchemy20: sh -c 'if [ '{env:CI:false}' != 'true' ]; then {envbindir}/buildout -nc {toxinidir}/postgres.cfg buildout:directory={envdir} buildout:develop={toxinidir} ; fi'
+    sqlalchemy20: sh -c 'if [ '{env:CI:false}' = 'true' ]; then {envbindir}/buildout -nc {toxinidir}/github_actions20.cfg buildout:directory={envdir} buildout:develop={toxinidir} ; fi'
+    sqlalchemy20: sh -c 'if [ '{env:CI:false}' != 'true' ]; then {envbindir}/buildout -nc {toxinidir}/postgres20.cfg buildout:directory={envdir} buildout:develop={toxinidir} ; fi'
 commands =
     {envbindir}/test {posargs:-cv}
-    sh -c 'if [ '{env:CI:false}' = 'true' ]; then {envbindir}/testpg {posargs:-cv} ; fi'
-    sh -c 'if [ '{env:CI:false}' = 'true' ]; then {envbindir}/testpg2 {posargs:-cv} ; fi'
+    sh -c 'if [ '{env:TEST_PG:{env:CI:false}}' = 'true' ]; then {envbindir}/testpg {posargs:-cv} ; fi'
+    sh -c 'if [ '{env:TEST_PG:{env:CI:false}}' = 'true' ]; then {envbindir}/testpg2 {posargs:-cv} ; fi'
+    sqlalchemy20: sh -c 'if [ '{env:TEST_PG:{env:CI:false}}' = 'true' ]; then {envbindir}/testpg3 {posargs:-cv} ; fi'
+    sqlalchemy20: sh -c 'if [ '{env:TEST_PG:{env:CI:false}}' = 'true' ]; then {envbindir}/testpg32 {posargs:-cv} ; fi'
 passenv =
     CI
+    TEST_PG
 allowlist_externals =
     sh
 
 [testenv:lint]
 basepython = python3
 commands_pre =
     mkdir -p {toxinidir}/parts/flake8
@@ -73,15 +79,15 @@
 deps =
     {[testenv]deps}
     coverage
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run {envdir}/bin/test {posargs:-cv}
     coverage html
-    coverage report -m --fail-under=70
+    coverage report -m --fail-under=65
 
 [coverage:run]
 branch = True
 source = zope.sqlalchemy
 
 [coverage:report]
 precision = 2
```

