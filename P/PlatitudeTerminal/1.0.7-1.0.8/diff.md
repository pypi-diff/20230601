# Comparing `tmp/PlatitudeTerminal-1.0.7.tar.gz` & `tmp/PlatitudeTerminal-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PlatitudeTerminal-1.0.7.tar", last modified: Mon May  8 21:17:30 2023, max compression
+gzip compressed data, was "PlatitudeTerminal-1.0.8.tar", last modified: Thu Jun  1 07:34:36 2023, max compression
```

## Comparing `PlatitudeTerminal-1.0.7.tar` & `PlatitudeTerminal-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/
--rw-r--r--   0 louis      (501) staff       (20)      224 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PKG-INFO
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)      224 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      417 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)       44 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/entry_points.txt
--rw-r--r--   0 louis      (501) staff       (20)       10 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/PlatitudeTerminal.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)      527 2023-05-03 03:52:08.000000 PlatitudeTerminal-1.0.7/pyproject.toml
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/peregrine/
--rw-r--r--   0 louis      (501) staff       (20)     2738 2023-05-07 20:21:08.000000 PlatitudeTerminal-1.0.7/peregrine/client.py
--rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.7/peregrine/colorutils.py
--rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.7/peregrine/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     2990 2023-05-03 05:17:22.000000 PlatitudeTerminal-1.0.7/peregrine/stateutils.py
--rw-r--r--   0 louis      (501) staff       (20)    30407 2023-05-08 21:12:51.000000 PlatitudeTerminal-1.0.7/peregrine/cli.py
--rw-r--r--   0 louis      (501) staff       (20)       21 2023-05-08 21:17:02.000000 PlatitudeTerminal-1.0.7/peregrine/install.py
--rw-r--r--   0 louis      (501) staff       (20)      275 2023-05-07 20:27:54.000000 PlatitudeTerminal-1.0.7/peregrine/errors.py
--rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.7/peregrine/main.py
--rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.7/README.md
--rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.7/setup.py
--rw-r--r--   0 louis      (501) staff       (20)      277 2023-05-08 21:17:30.000000 PlatitudeTerminal-1.0.7/setup.cfg
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-06-01 07:34:36.772606 PlatitudeTerminal-1.0.8/
+-rw-r--r--   0 louis      (501) staff       (20)     2273 2023-06-01 07:34:36.772661 PlatitudeTerminal-1.0.8/PKG-INFO
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-06-01 07:34:36.770043 PlatitudeTerminal-1.0.8/PlatitudeTerminal.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     2273 2023-06-01 07:34:36.000000 PlatitudeTerminal-1.0.8/PlatitudeTerminal.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      457 2023-06-01 07:34:36.000000 PlatitudeTerminal-1.0.8/PlatitudeTerminal.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-06-01 07:34:36.000000 PlatitudeTerminal-1.0.8/PlatitudeTerminal.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       43 2023-06-01 07:34:36.000000 PlatitudeTerminal-1.0.8/PlatitudeTerminal.egg-info/entry_points.txt
+-rw-r--r--   0 louis      (501) staff       (20)      154 2023-06-01 07:34:36.000000 PlatitudeTerminal-1.0.8/PlatitudeTerminal.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       10 2023-06-01 07:34:36.000000 PlatitudeTerminal-1.0.8/PlatitudeTerminal.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)     2079 2023-05-02 17:40:54.000000 PlatitudeTerminal-1.0.8/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-06-01 07:34:36.772405 PlatitudeTerminal-1.0.8/peregrine/
+-rw-r--r--   0 louis      (501) staff       (20)        0 2023-04-17 02:58:31.000000 PlatitudeTerminal-1.0.8/peregrine/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    30298 2023-06-01 07:22:24.000000 PlatitudeTerminal-1.0.8/peregrine/cli.py
+-rw-r--r--   0 louis      (501) staff       (20)     2738 2023-05-07 20:21:08.000000 PlatitudeTerminal-1.0.8/peregrine/client.py
+-rw-r--r--   0 louis      (501) staff       (20)      980 2023-04-22 18:06:19.000000 PlatitudeTerminal-1.0.8/peregrine/colorutils.py
+-rw-r--r--   0 louis      (501) staff       (20)      275 2023-05-07 20:27:54.000000 PlatitudeTerminal-1.0.8/peregrine/errors.py
+-rw-r--r--   0 louis      (501) staff       (20)       21 2023-06-01 07:23:50.000000 PlatitudeTerminal-1.0.8/peregrine/install.py
+-rw-r--r--   0 louis      (501) staff       (20)       87 2023-03-30 08:54:25.000000 PlatitudeTerminal-1.0.8/peregrine/main.py
+-rw-r--r--   0 louis      (501) staff       (20)     2990 2023-05-03 05:17:22.000000 PlatitudeTerminal-1.0.8/peregrine/stateutils.py
+-rw-r--r--   0 louis      (501) staff       (20)      527 2023-05-03 03:52:08.000000 PlatitudeTerminal-1.0.8/pyproject.toml
+-rw-r--r--   0 louis      (501) staff       (20)      277 2023-06-01 07:34:36.772881 PlatitudeTerminal-1.0.8/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)       37 2023-04-18 06:28:45.000000 PlatitudeTerminal-1.0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PlatitudeTerminal-1.0.7/pyproject.toml` & `PlatitudeTerminal-1.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.7/peregrine/client.py` & `PlatitudeTerminal-1.0.8/peregrine/client.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.7/peregrine/colorutils.py` & `PlatitudeTerminal-1.0.8/peregrine/colorutils.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.7/peregrine/stateutils.py` & `PlatitudeTerminal-1.0.8/peregrine/stateutils.py`

 * *Files identical despite different names*

### Comparing `PlatitudeTerminal-1.0.7/peregrine/cli.py` & `PlatitudeTerminal-1.0.8/peregrine/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Print Platitude.ai subscriber info and token usage stats.
     """
     
     ctx.ensure_object(AppState)
     state = ctx.obj
 
     if not checkTier(state, 1):
-        typer.echo("Not subscribed, usage information is not available.")
+        typer.echo("Not subscribed, token usage information is not available.")
 
 
     else:
         (idT, _) = stateutils.loadUserTokens()
         email = stateutils.loadUserEmail()
         typer.echo(f"Logged in as: {email}")
 
@@ -162,15 +162,15 @@
         typer.echo(f"{colorutils.colors.OKGREEN}\nResponse: {colorutils.colors.ENDC} {chat_response}\n")
 
     return chat_response
 
 
 def checkTier(state: AppState, min_tier: int):
     if min_tier > 0 and state.env["TIER"] != stateutils.tier.PAID:
-        typer.echo("This function is only available to subscribers! Subscribe to Platitude.ai for as little as $1/mo plan to access this function and more! To do so, run `ai subscribe`.")
+        typer.echo("Subscribe to Platitude.ai to access this function and more! To do so, run `ai subscribe`.")
         return False
     else:
         full_tier = fetchTier(state.env["UID"], state.idToken, full=True)
 
         if min_tier > full_tier:
             if min_tier == 2:
                 typer.echo(f"This function is only available to Enthusiast or Professional tier subscribers. Use `ai manage` to upgrade your account.")
@@ -368,23 +368,23 @@
             email = stateutils.loadUserEmail()
 
             p = fetchPricing(uid=uid, idT=idToken)
             
 
             typer.echo(
                 f'''
-                                    {colorutils.colors.BOLD}      Select your plan  {colorutils.colors.ENDC}
+                                    {colorutils.colors.HEADER}      Select your plan  {colorutils.colors.ENDC}
                 ===================================================================
                         All Platitude.ai Plans come with a 7 day free trial!
 
           {colorutils.colors.BOLD}             Starter               Enthusiast              Professional {colorutils.colors.ENDC}
                 ====================    ====================    ====================   
-                |                  |    |                  |    |                  |                                        
+                |                  |    |                  |    |                  | 
                 |    ${p['1']['price']} / month    |    |    ${p['2']['price']} / month    |    |    ${p['3']['price']} / month    |
-                |    ~{int(p['1']['tokens']/100)} queries   |    |   ~{int(p['2']['tokens']/100)} queries   |    |   ~{int(p['3']['tokens']/100)} queries   |
+                |    ~{int(p['1']['tokens']/100)} queries  |    |   ~{int(p['2']['tokens']/100)} queries   |    |   ~{int(p['3']['tokens']/100)} queries  |
                 |                  |    |                  |    |                  |
                 |                  |    |   MOST POPULAR   |    |    BEST VALUE    |
                 ====================    ====================    ====================
    {colorutils.colors.BOLD}                     [1]                     [2]                     [3]          {colorutils.colors.ENDC}
```

### Comparing `PlatitudeTerminal-1.0.7/README.md` & `PlatitudeTerminal-1.0.8/README.md`

 * *Files identical despite different names*

