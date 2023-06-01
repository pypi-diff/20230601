# Comparing `tmp/PrimeBotFramework-1.0.29.tar.gz` & `tmp/PrimeBotFramework-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-l5_6bmd5/PrimeBotFramework-1.0.29.tar", last modified: Fri May 26 17:21:26 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-lolul7dg/PrimeBotFramework-1.0.31.tar", last modified: Thu Jun  1 14:12:20 2023, max compression
```

## Comparing `PrimeBotFramework-1.0.29.tar` & `PrimeBotFramework-1.0.31.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Cnab750/
--rw-rw-rw-   0 root         (0) root         (0)    10033 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Cnab750/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-26 17:21:26.861454 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      707 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-26 17:21:26.000000 PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-26 17:21:26.865454 PrimeBotFramework-1.0.29/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-05-26 17:21:15.000000 PrimeBotFramework-1.0.29/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-01 14:12:20.329182 PrimeBotFramework-1.0.31/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.321182 PrimeBotFramework-1.0.31/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10211 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.325182 PrimeBotFramework-1.0.31/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-01 14:12:20.329182 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      707 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-01 14:12:20.000000 PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-01 14:12:20.329182 PrimeBotFramework-1.0.31/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-01 14:12:08.000000 PrimeBotFramework-1.0.31/setup.py
```

### Comparing `PrimeBotFramework-1.0.29/PKG-INFO` & `PrimeBotFramework-1.0.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.29
+Version: 1.0.31
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/B2E/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/Cnab750/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/Cnab750/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,22 +92,24 @@
         Returns:
             list[dict]: lista de dicionarios contendo a informação de cada linha
         """
         dados = []
         for linha in linhas:
             versao_arquivo = self.identificar_versao_arquivo(linhas)
             codigo_registro = self.identificar_codigo_registro(linha)
+            if versao_arquivo == '':
+                raise Exception(f'Erro ao realizar a leitura! Versão do arquivo [{versao_arquivo}] não identificada')
             if codigo_registro == 'HEADER':
                 dados.append(self.leitura_header(versao_arquivo, tipo_arquivo, linha))
             elif codigo_registro == 'DETALHE':
                 dados.append(self.leitura_detalhe(versao_arquivo, tipo_arquivo, linha))
             elif codigo_registro == 'TRAILER':
                 dados.append(self.leitura_trailer(versao_arquivo, tipo_arquivo, linha))
             else:
-                raise('Erro ao realizar a leitura! COdigo de Registro de retorno não identificado.')
+                raise Exception(f'Erro ao realizar a leitura! Código de Registro [{codigo_registro}] não identificado.')
         return dados
             
     def leitura_header(self, versao_arquivo: str, tipo_arquivo: str, linha: str) -> dict:
         """Efetua a leitura do header
 
         Args:
             versao_arquivo (str): versão do layout CNAB750
```

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-1.0.31/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/D4Sign/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/IntegracaoSendGrid/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/ListenerECS/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/OracleDB/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.31/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.29
+Version: 1.0.31
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.29/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.31/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.29/setup.py` & `PrimeBotFramework-1.0.31/setup.py`

 * *Files identical despite different names*

