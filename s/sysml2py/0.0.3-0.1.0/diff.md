# Comparing `tmp/sysml2py-0.0.3.tar.gz` & `tmp/sysml2py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysml2py-0.0.3.tar", last modified: Tue May 30 13:22:41 2023, max compression
+gzip compressed data, was "sysml2py-0.1.0.tar", last modified: Thu Jun  1 11:37:20 2023, max compression
```

## Comparing `sysml2py-0.0.3.tar` & `sysml2py-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:22:41.251485 sysml2py-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 13:22:08.000000 sysml2py-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 13:22:41.251485 sysml2py-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-30 13:22:08.000000 sysml2py-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-30 13:22:08.000000 sysml2py-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:22:41.251485 sysml2py-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:22:41.247485 sysml2py-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:22:41.247485 sysml2py-0.0.3/src/sysml2py/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 13:22:08.000000 sysml2py-0.0.3/src/sysml2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:22:41.247485 sysml2py-0.0.3/src/sysml2py/textx/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-30 13:22:08.000000 sysml2py-0.0.3/src/sysml2py/textx/xtext_to_textx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-30 13:22:08.000000 sysml2py-0.0.3/src/sysml2py/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:22:41.247485 sysml2py-0.0.3/src/sysml2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 13:22:41.000000 sysml2py-0.0.3/src/sysml2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-30 13:22:41.000000 sysml2py-0.0.3/src/sysml2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:22:41.000000 sysml2py-0.0.3/src/sysml2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 13:22:41.000000 sysml2py-0.0.3/src/sysml2py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:37:20.129270 sysml2py-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 11:36:58.000000 sysml2py-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 11:37:20.129270 sysml2py-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-01 11:36:58.000000 sysml2py-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 11:36:58.000000 sysml2py-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:37:20.129270 sysml2py-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:37:20.129270 sysml2py-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:37:20.129270 sysml2py-0.1.0/src/sysml2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-01 11:36:58.000000 sysml2py-0.1.0/src/sysml2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-01 11:36:58.000000 sysml2py-0.1.0/src/sysml2py/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:37:20.129270 sysml2py-0.1.0/src/sysml2py/textx/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-06-01 11:36:58.000000 sysml2py-0.1.0/src/sysml2py/textx/xtext_to_textx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 11:36:58.000000 sysml2py-0.1.0/src/sysml2py/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:37:20.129270 sysml2py-0.1.0/src/sysml2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-01 11:37:20.000000 sysml2py-0.1.0/src/sysml2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 11:37:20.000000 sysml2py-0.1.0/src/sysml2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:37:20.000000 sysml2py-0.1.0/src/sysml2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 11:37:20.000000 sysml2py-0.1.0/src/sysml2py.egg-info/top_level.txt
```

### Comparing `sysml2py-0.0.3/LICENSE` & `sysml2py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysml2py-0.0.3/pyproject.toml` & `sysml2py-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysml2py"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Christopher Cox", email="chris.cox@westfall.io" },
 ]
 description = "SysML v2.0 Parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sysml2py-0.0.3/src/sysml2py/textx/xtext_to_textx.py` & `sysml2py-0.1.0/src/sysml2py/textx/xtext_to_textx.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,64 +3,72 @@
 """
 Created on Wed May 24 16:41:15 2023
 
 @author: christophercox
 """
 import re
 
+
 def xtext_to_textx(rules):
-    
     # Remove grammar
-    rules = re.sub('grammar .*', '', rules)
-    
+    rules = re.sub("grammar .*", "", rules)
+
     # Remove imports
-    rules = re.sub('import .*', '', rules)
-    
+    rules = re.sub("import .*", "", rules)
+
     # Remove returns
-    rules = re.sub('returns .*', ':', rules)
-    
+    rules = re.sub("returns .*", ":", rules)
+
     # Remove terminal
-    rules = re.sub('terminal ', '', rules)
-    
+    rules = re.sub("terminal ", "", rules)
+
     # Remove fragments
-    rules = re.sub('fragment', '', rules)
-    rules = re.sub('enum', '', rules)
-    rules = re.sub(' ->', '', rules)
-    rules = re.sub('[\s]?=>', '', rules)
-    rules = re.sub('@Override','', rules)
-    
+    rules = re.sub("fragment", "", rules)
+    rules = re.sub("enum", "", rules)
+    rules = re.sub(" ->", "", rules)
+    rules = re.sub("[\s]?=>", "", rules)
+    rules = re.sub("@Override", "", rules)
+
     # Remove SysML object references
-    rules = re.sub('{SysML::[a-zA-Z]*}', '', rules)
-    rules = re.sub('{SysML::[a-zA-Z\.\+\=\s]*}','', rules)
-    
+    rules = re.sub("{SysML::[a-zA-Z]*}", "", rules)
+    rules = re.sub("{SysML::[a-zA-Z\.\+\=\s]*}", "", rules)
+
     # Remove more SysML object references
-    #rules = re.sub('SysML::Membership\|QualifiedName', 'QualifiedName', rules)
-    #rules = re.sub('SysML::Namespace\|QualifiedName', 'QualifiedName', rules)
-    #rules = re.sub('SysML::Element\|QualifiedName', 'QualifiedName', rules)
-    #rules = re.sub('SysML::Feature[\s]?\|[\s]?QualifiedName', 'QualifiedName', rules)
-    rules = re.sub('\[[\s]?SysML::[a-zA-Z]*[\s]?\|[\s]?QualifiedName[\s]?\]', '[QualifiedName]', rules)
-    rules = re.sub('SysML::ConjugatedPortDefinition | ConjugatedQualifiedName', 'ConjugatedQualifiedName', rules)
-    
+    # rules = re.sub('SysML::Membership\|QualifiedName', 'QualifiedName', rules)
+    # rules = re.sub('SysML::Namespace\|QualifiedName', 'QualifiedName', rules)
+    # rules = re.sub('SysML::Element\|QualifiedName', 'QualifiedName', rules)
+    # rules = re.sub('SysML::Feature[\s]?\|[\s]?QualifiedName', 'QualifiedName', rules)
+    rules = re.sub(
+        "\[[\s]?SysML::[a-zA-Z]*[\s]?\|[\s]?QualifiedName[\s]?\]",
+        "[QualifiedName]",
+        rules,
+    )
+    rules = re.sub(
+        "SysML::ConjugatedPortDefinition | ConjugatedQualifiedName",
+        "ConjugatedQualifiedName",
+        rules,
+    )
+
     # Fix doubles
-    rules = re.sub('\[QualifiedName | QualifiedName\]', '[QualifiedName]', rules)
-    rules = re.sub('\[QualifiedName\|QualifiedName\]', '[QualifiedName]', rules)
-    
+    rules = re.sub("\[QualifiedName | QualifiedName\]", "[QualifiedName]", rules)
+    rules = re.sub("\[QualifiedName\|QualifiedName\]", "[QualifiedName]", rules)
+
     # Special cases
-    good_str = r'''
+    good_str = r"""
 MultiplicityRelatedElement :
     (LiteralExpression | FeatureReferenceExpression)
 ;
     
 MultiplicityExpressionMember :
     ownedRelatedElement += MultiplicityRelatedElement
-;'''
-    
-    rules = re.sub('MultiplicityExpressionMember :[\s\S]*?;', good_str, rules)
-    
-    good_str = r'''
+;"""
+
+    rules = re.sub("MultiplicityExpressionMember :[\s\S]*?;", good_str, rules)
+
+    good_str = r"""
 ActionBodyItemTarget :
     ( BehaviorUsageMember | ActionNodeMember )
 ;
 
 ActionBodyItem :
 	  ownedRelationship += Import
 	| ownedRelationship += AliasMember
@@ -72,61 +80,93 @@
 	| ownedRelationship += InitialNodeMember
 	  ( ownedRelationship += TargetSuccessionMember )*
 	| ( ownedRelationship += EmptySuccessionMember )?
 	  ownedRelationship += ActionBodyItemTarget
 	  ( ownedRelationship += TargetSuccessionMember )*
 	| ownedRelationship += GuardedSuccessionMember
 ;
-'''
-    rules = re.sub('ActionBodyItem :[\s\S]*?;', good_str, rules)
-    
-    good_str = r'''    
+"""
+    rules = re.sub("ActionBodyItem :[\s\S]*?;", good_str, rules)
+
+    good_str = r"""    
 IfNodeElseMember :
     ( ActionBodyParameterMember | IfNodeParameterMember )
 ;
 
 IfNode :
 	ActionNodePrefix 
 	'if' ownedRelationship += ExpressionParameterMember
 	ownedRelationship += ActionBodyParameterMember
 	( 'else' ownedRelationship += IfNodeElseMember )?
 ;
-'''
-    rules = re.sub('IfNode :[\s\S]*?;', good_str, rules)
-    
-    good_str = r'''
+"""
+    rules = re.sub("IfNode :[\s\S]*?;", good_str, rules)
+
+    good_str = r"""
 ( isOrdered ?= 'ordered' isNonunique ?= 'nonunique'
    | isNonunique2 ?= 'nonunique' isOrdered2 ?= 'ordered'
 )
-'''
-    rules = re.sub("\( isOrdered[a-zA-Z0-9\?\=\s\'\|]*\)", good_str, rules)
-    
+"""
+    rules = re.sub("\( isOrdered[a-zA-Z0-9\?\=\s'\|]*\)", good_str, rules)
+
     # These are totally broken
-    empty_rule = 'LifeClass'
-    rules = re.sub(empty_rule+' :[\s\S]*?;', empty_rule+" ://This doesn't work.\n\t'"+empty_rule.lower()+"'\n;", rules)
-    empty_rule = 'EmptyTargetEnd'
-    rules = re.sub(empty_rule+' :[\s\S]*?;', empty_rule+" ://This doesn't work.\n\t'"+empty_rule.lower()+"'\n;", rules)
-    empty_rule = 'PortConjugation'
-    rules = re.sub(empty_rule+' :[\s\S]*?;', empty_rule+" ://This doesn't work.\n\t'"+empty_rule.lower()+"'\n;", rules)
-    empty_rule = 'EmptySourceEnd'
-    rules = re.sub(empty_rule+' :[\s\S]*?;', empty_rule+" ://This doesn't work.\n\t'"+empty_rule.lower()+"'\n;", rules)
-    empty_rule = 'EmptyUsage'
-    rules = re.sub(empty_rule+' :[\s\S]*?;', empty_rule+" ://This doesn't work.\n\t'"+empty_rule.lower()+"'\n;", rules)
-    empty_rule = 'EmptyActionUsage'
-    rules = re.sub(empty_rule+' :[\s\S]*?;', empty_rule+" ://This doesn't work.\n\t'"+empty_rule.lower()+"'\n;", rules)
-    empty_rule = 'EmptyFeature'
-    rules = re.sub(empty_rule+' :[\s\S]*?;', empty_rule+" ://This doesn't work.\n\t'"+empty_rule.lower()+"'\n;", rules)
-    
+    empty_rule = "LifeClass"
+    rules = re.sub(
+        empty_rule + " :[\s\S]*?;",
+        empty_rule + " ://This doesn't work.\n\t'" + empty_rule.lower() + "'\n;",
+        rules,
+    )
+    empty_rule = "EmptyTargetEnd"
+    rules = re.sub(
+        empty_rule + " :[\s\S]*?;",
+        empty_rule + " ://This doesn't work.\n\t'" + empty_rule.lower() + "'\n;",
+        rules,
+    )
+    empty_rule = "PortConjugation"
+    rules = re.sub(
+        empty_rule + " :[\s\S]*?;",
+        empty_rule + " ://This doesn't work.\n\t'" + empty_rule.lower() + "'\n;",
+        rules,
+    )
+    empty_rule = "EmptySourceEnd"
+    rules = re.sub(
+        empty_rule + " :[\s\S]*?;",
+        empty_rule + " ://This doesn't work.\n\t'" + empty_rule.lower() + "'\n;",
+        rules,
+    )
+    empty_rule = "EmptyUsage"
+    rules = re.sub(
+        empty_rule + " :[\s\S]*?;",
+        empty_rule + " ://This doesn't work.\n\t'" + empty_rule.lower() + "'\n;",
+        rules,
+    )
+    empty_rule = "EmptyActionUsage"
+    rules = re.sub(
+        empty_rule + " :[\s\S]*?;",
+        empty_rule + " ://This doesn't work.\n\t'" + empty_rule.lower() + "'\n;",
+        rules,
+    )
+    empty_rule = "EmptyFeature"
+    rules = re.sub(
+        empty_rule + " :[\s\S]*?;",
+        empty_rule + " ://This doesn't work.\n\t'" + empty_rule.lower() + "'\n;",
+        rules,
+    )
+
     # Base rules
-    rules = re.sub("DECIMAL_VALUE[\s]:[\s0-9\(\)\'\*\.]*;", 'DECIMAL_VALUE :\n   /[0-9]*/;', rules)
-    rules = re.sub("ID[\s]?:[\sa-zA-Z0-9_'|().*]*;", 'ID :\n   /[a-zA-Z_][a-zA-Z_0-9]*/;', rules)
-    #rules = re.sub("UNRESTRICTED_NAME[ ]?:[\sbtnfr\"!\\_'|().*]*;", 
+    rules = re.sub(
+        "DECIMAL_VALUE[\s]:[\s0-9\(\)'\*\.]*;", "DECIMAL_VALUE :\n   /[0-9]*/;", rules
+    )
+    rules = re.sub(
+        "ID[\s]?:[\sa-zA-Z0-9_'|().*]*;", "ID :\n   /[a-zA-Z_][a-zA-Z_0-9]*/;", rules
+    )
+    # rules = re.sub("UNRESTRICTED_NAME[ ]?:[\sbtnfr\"!\\_'|().*]*;",
     #    "UNRESTRICTED_NAME: \n   /'\'' ('\\' ('b' | 't' | 'n' | 'f' | 'r' | '"' | "'" | '\\') | !('\\' | '\''))* '\''/;", rules)
-    
-    final_rules = ''';
+
+    final_rules = """;
     
 ID :
    /[a-zA-Z_][a-zA-Z_0-9]*/;
 
 UNRESTRICTED_NAME :
 	/'\'' ('\\' ('b' | 't' | 'n' | 'f' | 'r' | '"' | "'" | '\\') | !('\\' | '\''))* '\''/;
 
@@ -140,42 +180,42 @@
 	/'\/*'->'*\/'/;
 
 SL_NOTE:
 	/'\/\/' (!('\n' | '\r') !('\n' | '\r')*)? ('\r'? '\n')?/;
 
 WS:
 	/(' ' | '\t' | '\r' | '\n')+/;
-'''
+"""
     rules = re.sub(";[\s]*ID[\s\S]*;", final_rules, rules)
     return rules
 
-if __name__ == '__main__':
-    with open('SysML.xtext', 'r') as f:
+
+if __name__ == "__main__":
+    with open("SysML.xtext", "r") as f:
         rules = f.read()
     f.close()
-    
+
     rules = xtext_to_textx(rules)
-    
-    with open('SysML.tx', 'w') as f:
-        f.write('import KerML\nimport KerMLExpressions\n'+rules)
+
+    with open("SysML.tx", "w") as f:
+        f.write("import KerML\nimport KerMLExpressions\n" + rules)
     f.close()
-    
-    with open('KerML.xtext', 'r') as f:
+
+    with open("KerML.xtext", "r") as f:
         rules = f.read()
     f.close()
-    
+
     rules = xtext_to_textx(rules)
-    
-    with open('KerML.tx', 'w') as f:
-        f.write('import KerMLExpressions\n'+rules)
+
+    with open("KerML.tx", "w") as f:
+        f.write("import KerMLExpressions\n" + rules)
     f.close()
-    
-    with open('KerMLExpressions.xtext', 'r') as f:
+
+    with open("KerMLExpressions.xtext", "r") as f:
         rules = f.read()
     f.close()
-    
+
     rules = xtext_to_textx(rules)
-    
-    with open('KerMLExpressions.tx', 'w') as f:
+
+    with open("KerMLExpressions.tx", "w") as f:
         f.write(rules)
     f.close()
-
```

