# Comparing `tmp/rpa_cooperativa-1.0.54.tar.gz` & `tmp/rpa_cooperativa-1.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.54.tar", last modified: Fri May 19 18:59:18 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.55.tar", last modified: Thu Jun  1 16:55:33 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.54.tar` & `rpa_cooperativa-1.0.55.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.875618 rpa_cooperativa-1.0.54/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.54/LICENSE
--rw-rw-rw-   0        0        0     6875 2023-05-19 18:59:18.869056 rpa_cooperativa-1.0.54/PKG-INFO
--rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.54/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.437703 rpa_cooperativa-1.0.54/rpa_coop/
--rw-rw-rw-   0        0        0      585 2023-05-19 18:39:16.000000 rpa_cooperativa-1.0.54/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.748006 rpa_cooperativa-1.0.54/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.54/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.54/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.54/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.54/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.54/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.54/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    82582 2023-05-19 18:55:16.000000 rpa_cooperativa-1.0.54/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:59:18.853073 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6875 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-05-19 18:59:18.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 18:59:17.000000 rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 18:59:18.880302 rpa_cooperativa-1.0.54/setup.cfg
--rw-rw-rw-   0        0        0     2325 2023-05-19 18:38:52.000000 rpa_cooperativa-1.0.54/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.933443 rpa_cooperativa-1.0.55/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.55/LICENSE
+-rw-rw-rw-   0        0        0     6875 2023-06-01 16:55:33.928457 rpa_cooperativa-1.0.55/PKG-INFO
+-rw-rw-rw-   0        0        0     5730 2023-05-19 18:58:05.000000 rpa_cooperativa-1.0.55/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.683986 rpa_cooperativa-1.0.55/rpa_coop/
+-rw-rw-rw-   0        0        0      585 2023-05-22 15:25:02.000000 rpa_cooperativa-1.0.55/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.868452 rpa_cooperativa-1.0.55/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.55/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.55/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.55/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.55/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.55/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.55/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    87333 2023-06-01 16:51:46.000000 rpa_cooperativa-1.0.55/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:55:33.918993 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6875 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-06-01 16:55:33.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 16:55:32.000000 rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 16:55:33.935447 rpa_cooperativa-1.0.55/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-06-01 16:53:22.000000 rpa_cooperativa-1.0.55/setup.py
```

### Comparing `rpa_cooperativa-1.0.54/LICENSE` & `rpa_cooperativa-1.0.55/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/PKG-INFO` & `rpa_cooperativa-1.0.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.54
+Version: 1.0.55
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.54/README.md` & `rpa_cooperativa-1.0.55/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.55/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.55/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.55/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.55/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.55/rpa_coop/rpa_coop.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,20 +114,17 @@
         if id_usuario == 'Não encontrado': raise Exception('Usuário não encontrado')
         url = f'{self.url_api_adobe}users/{id_usuario}/state'
         headers = { "Authorization": f"{token_get_user}"}
         body = {"state": f"{status_usuario}", "comment": "desativado por rpa"}
         response = requests.put(url, headers=headers, json=body)
         return response
         
-        
-        
-  
+                
 class Dados:
     
-
     def __init__(self):
         self.ip_planning = str(os.getenv('ip_planning'))
         self.user_planning = str(os.getenv('user_planning'))
         self.pw_bd_planning = str(urllib.parse.quote_plus(os.getenv('pw_bd_planning'))) 
         
         self.user_planning_controles = str(gerador_pwd('user_planning_controles', 'senha'))
         self.pw_planning_controles = str(gerador_pwd('pw_planning_controles', 'senha'))
@@ -1109,48 +1106,33 @@
             if isinstance(destinatarios, str): todos_destinos.append(destinatarios)
             if isinstance(cco, list): todos_destinos.extend(cco)
             if isinstance(cco, str): todos_destinos.append(cco) 
             smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)
         else:
             if isinstance(destinatarios, list): todos_destinos.extend(destinatarios)
             if isinstance(destinatarios, str): todos_destinos.append(destinatarios)
-            smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)
-            
+            smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)        
         smtpserver.close()
         
-        
-        
-    # def ler_email(self):
-    #     from imap_tools import MailBox
-    #     serv_imap = self.smtpsrv.replace('smtp', 'imap')
-        
-    #     # get list of email bodies from INBOX folder
-    #     with MailBox(serv_imap).login(self.user_mail, self.password_mail, 'INBOX') as mailbox:
-    #         for msg in mailbox.fetch():
-    #             msg_de = str(msg.from_)
-    #             if 'edenilson' in msg_de:
-    #                 # print(msg.subject)
-    #                 # print(msg.text)
-    #                 return msg.text
-            
-        
-        
-                       
+                                        
 class Acc:
     import pyautogui as p
     import subprocess
     import pyperclip
     
     
     def __init__(self):
         self.usuario_acc = str(gerador_pwd('acc', 'usuario'))
         self.senha_acc = str(gerador_pwd('acc', 'senha'))
+        self.janela_sacg = 'janela'
+        self.janela_siat = 'janela'
+        self.janela_siac = 'janela'
 
     
-    def open_acclient(self, siat_siac_sacg, transacional=True):
+    def open_acclient_old(self, siat_siac_sacg, transacional=True):
         # Open AC Client
         try:
             self.p.sleep(1)
             os.system('taskkill /F /FI "WindowTitle eq C:\\ProgramData\\ac\\teoff-exe*" /T')
         except Exception:
             pass
         
@@ -1220,17 +1202,141 @@
             self.p.doubleClick()
         else:
             self.p.moveTo(janela.left + 48, janela.top + 245)
             self.p.doubleClick()
         time.sleep(7)
         
            
-    def select_menu_letras(self, letras):
+    def open_acclient(self, siat_siac_sacg: str | list, transacional=True):
+        ''' acc.open_acclient('siac') \n
+         acc.open_acclient(['siat', 'sacg'])'''
+        opcoes = []
+        if isinstance(siat_siac_sacg, str):
+            opcoes.append(siat_siac_sacg)
+        else:
+            opcoes = siat_siac_sacg
+            
+        # Open AC Client
+        try:
+            self.p.sleep(1)
+            os.system('taskkill /F /FI "WindowTitle eq C:\\ProgramData\\ac\\teoff-exe*" /T')
+        except Exception:
+            pass
+        
+        try:
+            os.system('taskkill /F /IM javaw_ac.exe')
+            self.p.sleep(1)
+        except Exception:
+            pass
+        
+        user_acc = self.usuario_acc
+        pw_acclient = self.senha_acc
+         
+        self.subprocess.Popen("C:\\Users\\Public\\Desktop\\AC Client.lnk",shell=True)
+        self.p.sleep(15)
+        
+
+        # pegar retangulo da janela pelo titulo parcial
+        janela = self.p.getWindowsWithTitle('Aplicações Core - Login')[0]
+        janela.activate()
+
+        self.p.press('tab')
+        self.p.press('tab')
+        # digitar usuario
+        self.p.typewrite(user_acc)
+        self.p.press('tab')
+        self.p.typewrite(pw_acclient)
+        self.p.press('tab')
+        self.p.press('enter')
+        print('passou do login')
+
+        self.p.sleep(12)
+        # pegar retangulo da janela pelo titulo parcial
+        janela = self.p.getWindowsWithTitle('AC Client')[0]
+        janela.activate()
+        janela.left
+        self.p.sleep(1)
+        self.p.press('pgdn')
+
+        # Selecionar o MENU SIAT
+        posicao = 0
+        pasta_imagens = user_site_packages +  '\\rpa_coop\\img\\'
+        
+                   
+        
+        if transacional:
+            self.p.moveTo(janela.left + 48, janela.top + 165)
+            time.sleep(1)
+            self.p.click()
+            # self.p.doubleClick()
+        else:
+            self.p.moveTo(janela.left + 48, janela.top + 245)
+            self.p.click()
+            # self.p.doubleClick()
+        time.sleep(3)
+            
+   
+
+        num_menu = 0
+        self.janela_sacg = janela
+        self.janela_siat = janela
+        self.janela_siac = janela
+        
+        opcoes = [x.upper() for x in opcoes]
+        
+        for menu in opcoes:
+            if menu == 'SACG':
+                # Abrir SACG
+                try:
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, grayscale=True)
+                except:
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, grayscale=True)
+                self.p.doubleClick(posicao)
+                time.sleep(7)
+                self.janela_sacg = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
+                print('clicou no menu: sacg')
+                janela.activate()
+            elif menu == 'SIAT':
+                # Abrir SIAT
+                try:
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, grayscale=True)
+                except:
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, grayscale=True)
+                self.p.doubleClick(posicao)
+                time.sleep(7)
+                self.janela_siat = self.p.getWindowsWithTitle('teoff-exe')[num_menu] 
+                print('clicou no menu: siat')
+                janela.activate()
+            elif menu == 'SIAC':
+                try:
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, grayscale=True)
+                except:
+                    posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, grayscale=True)
+                self.p.doubleClick(posicao)
+                time.sleep(7)
+                self.janela_siac = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
+                print('clicou no menu: siac')
+                janela.activate()
+            time.sleep(1)
+        return self.janela_sacg, self.janela_siat, self.janela_siac
+
+             
+    def select_menu_letras(self, letras, nome_janela=None):
+        '''acc.select_menu_letras(letras) \n
+         acc.select_menu_letras(letras, nome_janela='sacg')'''
         self.p.sleep(1)
-        janela = self.p.getWindowsWithTitle('teoff-exe')[0]
+        nome_janela = str(nome_janela).upper()
+        if nome_janela == 'SIAT':
+            janela = self.janela_siat
+        elif nome_janela == 'SIAC':
+            janela = self.janela_siac
+        elif nome_janela == 'SACG':
+            janela = self.janela_sacg
+        else:
+            janela = self.p.getWindowsWithTitle('teoff-exe')[0]
         janela.activate()
         # Selecionar o Menu de opções
         self.p.sleep(1)
         if len(letras) == 2:
             self.p.typewrite(letras[0])
             self.p.sleep(1)
             self.p.typewrite(letras[1])
@@ -1289,50 +1395,63 @@
             self.p.typewrite(letras[5])
             self.p.sleep(1)
             self.p.typewrite(letras[6])
             self.p.sleep(1)
         else:
             print('ops funcao entende apenas 2, 3, 4, 5, 6 ou 7 letras')
             
-                
-    def get_text(self, ini_linha=22, fim_linha=632, topo1=410, topo2=415):
+                  
+    def get_text(self, ini_linha=22, fim_linha=632, topo1=410, topo2=415, nome_janela=None):
+        ''' acc.get_text('Retorna ao Sistema')\n
+         acc.get_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
-        janela = self.p.getWindowsWithTitle('teoff-exe')[0]
+        nome_janela = str(nome_janela).upper()
+        if nome_janela == 'SIAT':
+            janela = self.janela_siat
+        elif nome_janela == 'SIAC':
+            janela = self.janela_siac
+        elif nome_janela == 'SACG':
+            janela = self.janela_sacg
+        else:
+            janela = self.p.getWindowsWithTitle('teoff-exe')[0]
+  
         time.sleep(1)
         janela.activate()
         self.p.moveTo(janela.left + ini_linha, janela.top + topo1)
         self.p.sleep(1)
         self.p.dragTo(janela.left + fim_linha, janela.top + topo2, 1.5, button='left')
         self.p.moveTo(janela.left + ini_linha, janela.top + topo2)
         self.p.rightClick()
         capturado = self.pyperclip.paste()
         print(f'texto capturado:{capturado}')
         return capturado            
             
             
-    def exist_text(self, texto_esperado, max_tentativas=7, segundos_entre_tentativas=3, ini_linha=22, fim_linha=632, topo1=412, topo2=412, continua_seerro=False):
+    def exist_text(self, texto_esperado, max_tentativas=7, segundos_entre_tentativas=3, ini_linha=22, fim_linha=632, topo1=412, topo2=412, continua_seerro=False, nome_janela=None):
+        ''' acc.exist_text('Retorna ao Sistema')\n
+         acc.exist_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
         self.pyperclip.copy('')
         tentativas = 0
         time.sleep(1)
-        captura = self.get_text(ini_linha, fim_linha, topo1, topo2)
+        captura = self.get_text(ini_linha, fim_linha, topo1, topo2, nome_janela = nome_janela)
         resultado = True
         while not texto_esperado in captura and tentativas < max_tentativas:
             print('esperando texto: ', texto_esperado)
             self.p.sleep(segundos_entre_tentativas)
-            captura = self.get_text(ini_linha, fim_linha, topo1, topo2)
+            captura = self.get_text(ini_linha, fim_linha, topo1, topo2, nome_janela = nome_janela)
             tentativas += 1
             if tentativas == max_tentativas:
                 resultado = False
         print(resultado)
         if resultado == False and continua_seerro == False:
             raise Exception(f'Execução pausada. O texto: "{texto_esperado}" não foi localizado durante a execução do robô.')
         return resultado
  
-           
+         
 class Monitorar:
         
     import socket
     import paramiko
     from dateutil.relativedelta import relativedelta
          
     def __init__(self):
@@ -1837,18 +1956,15 @@
             dia_util_proximo = dia_us
         else:
             dia_util_proximo = dia_br
             
         return dia_util_proximo
         
         
-        
-        
 
-# mail = Emails()
-# mail.ler_email()
+
```

### Comparing `rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.54
+Version: 1.0.55
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.55/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.54/setup.py` & `rpa_cooperativa-1.0.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.54",
+    version="1.0.55",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

