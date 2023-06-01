# Comparing `tmp/neon_phal_plugin_reset-0.1.1a2-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_reset-0.1.1a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11228 bytes, number of entries: 10
--rw-r--r--  2.0 unx    11178 b- defN 23-May-15 20:37 neon_phal_plugin_reset/__init__.py
--rw-r--r--  2.0 unx     2687 b- defN 23-May-15 20:37 neon_phal_plugin_reset/config.py
--rw-r--r--  2.0 unx     3873 b- defN 23-May-15 20:37 neon_phal_plugin_reset/create_media.py
--rw-r--r--  2.0 unx     1856 b- defN 23-May-15 20:37 neon_phal_plugin_reset/version.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-15 20:37 neon_phal_plugin_reset-0.1.1a2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1197 b- defN 23-May-15 20:37 neon_phal_plugin_reset-0.1.1a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 20:37 neon_phal_plugin_reset-0.1.1a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 23-May-15 20:37 neon_phal_plugin_reset-0.1.1a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-May-15 20:37 neon_phal_plugin_reset-0.1.1a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      952 b- defN 23-May-15 20:37 neon_phal_plugin_reset-0.1.1a2.dist-info/RECORD
-10 files, 23577 bytes uncompressed, 9564 bytes compressed:  59.4%
+Zip file size: 11276 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    11560 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/__init__.py
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/config.py
+-rw-r--r--  2.0 unx     3873 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/create_media.py
+-rw-r--r--  2.0 unx     1856 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/version.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      952 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/RECORD
+10 files, 23959 bytes uncompressed, 9612 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: neon_phal_plugin_reset/create_media.py
 Comment: 
 
 Filename: neon_phal_plugin_reset/version.py
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a2.dist-info/LICENSE.md
+Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a2.dist-info/METADATA
+Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a2.dist-info/WHEEL
+Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a2.dist-info/entry_points.txt
+Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a2.dist-info/top_level.txt
+Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a2.dist-info/RECORD
+Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_reset/__init__.py

```diff
@@ -25,15 +25,15 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from shutil import move, rmtree
 from subprocess import Popen
 from os import remove
-from os.path import isfile, join
+from os.path import isfile, join, isdir
 from threading import RLock
 from zipfile import BadZipFile
 
 from mycroft_bus_client import Message
 from ovos_utils.log import LOG
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_skill_installer import download_extract_zip
@@ -110,14 +110,20 @@
         try:
             if message.data.get('skill_config'):
                 LOG.debug("Updating skill config from default")
                 Popen(["/usr/bin/cp", "-r",
                        "/tmp/neon/neon-image-recipe/05_neon_core"
                        "/overlay/home/neon/.config/neon/skills",
                        "/home/neon/.config/neon/"])
+                if isdir("/tmp/neon/neon-image-recipe/05_neon_core/overlay/"
+                         "home/neon/.config/neon/apps"):
+                    Popen(["/usr/bin/cp", "-r",
+                           "/tmp/neon/neon-image-recipe/05_neon_core"
+                           "/overlay/home/neon/.config/neon/apps",
+                           "/home/neon/.config/neon/"])
                 Popen("chown -R neon:neon /home/neon", shell=True)
             if message.data.get('core_config'):
                 LOG.debug("Updating system config from default")
                 move("/tmp/neon/neon-image-recipe/05_neon_core/overlay"
                      "/etc/neon/neon.yaml", "/etc/neon/neon.yaml")
             LOG.info(f"Restored default configuration")
             rmtree("/tmp/neon/neon-image-recipe")
```

## neon_phal_plugin_reset/version.py

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a2"
+__version__ = "0.1.1a3"
```

## Comparing `neon_phal_plugin_reset-0.1.1a2.dist-info/LICENSE.md` & `neon_phal_plugin_reset-0.1.1a3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_reset-0.1.1a2.dist-info/METADATA` & `neon_phal_plugin_reset-0.1.1a3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

