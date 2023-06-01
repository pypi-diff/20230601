# Comparing `tmp/django-modshib-CERTIC-0.1.2.tar.gz` & `tmp/django_modshib_certic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-modshib-CERTIC-0.1.2.tar", max compression
+gzip compressed data, was "django_modshib_certic-0.1.3.tar", max compression
```

## Comparing `django-modshib-CERTIC-0.1.2.tar` & `django_modshib_certic-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.653227 django-modshib-CERTIC-0.1.2/modshib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-19 06:10:59.654166 django-modshib-CERTIC-0.1.2/modshib/admin.py
--rw-r--r--   0        0        0      146 2023-05-24 09:58:37.360521 django-modshib-CERTIC-0.1.2/modshib/apps.py
--rw-r--r--   0        0        0      310 2023-05-26 07:17:40.682916 django-modshib-CERTIC-0.1.2/modshib/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-19 06:10:59.656283 django-modshib-CERTIC-0.1.2/modshib/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-05-19 06:10:59.655746 django-modshib-CERTIC-0.1.2/modshib/models.py
--rw-r--r--   0        0        0      897 2023-05-26 08:00:55.045522 django-modshib-CERTIC-0.1.2/modshib/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1315 2023-05-24 08:51:31.235141 django-modshib-CERTIC-0.1.2/modshib/templates/registration/login.html
--rw-r--r--   0        0        0      838 2023-05-19 07:02:49.960081 django-modshib-CERTIC-0.1.2/modshib/templates/registration/reg_base.html
--rw-r--r--   0        0        0      794 2023-05-24 08:22:05.742051 django-modshib-CERTIC-0.1.2/modshib/templates/registration/sso_fail.html
--rw-r--r--   0        0        0      813 2023-05-24 09:54:48.646844 django-modshib-CERTIC-0.1.2/modshib/templates/registration/sso_no_account.html
--rw-r--r--   0        0        0       60 2023-05-19 06:10:59.655994 django-modshib-CERTIC-0.1.2/modshib/tests.py
--rw-r--r--   0        0        0      117 2023-05-22 09:06:53.828987 django-modshib-CERTIC-0.1.2/modshib/urls.py
--rw-r--r--   0        0        0     2761 2023-05-26 06:27:37.660477 django-modshib-CERTIC-0.1.2/modshib/views.py
--rw-r--r--   0        0        0      551 2023-05-26 08:01:29.464166 django-modshib-CERTIC-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      722 2023-05-26 08:09:47.354958 django-modshib-CERTIC-0.1.2/setup.py
--rw-r--r--   0        0        0      700 2023-05-26 08:09:47.355192 django-modshib-CERTIC-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.3/modshib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.3/modshib/admin.py
+-rw-r--r--   0        0        0      146 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.3/modshib/apps.py
+-rw-r--r--   0        0        0      400 2023-06-01 08:51:10.568109 django_modshib_certic-0.1.3/modshib/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.3/modshib/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-24 14:07:03.820594 django_modshib_certic-0.1.3/modshib/models.py
+-rw-r--r--   0        0        0      917 2023-05-31 23:35:50.748471 django_modshib_certic-0.1.3/modshib/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1334 2023-06-01 08:51:10.568109 django_modshib_certic-0.1.3/modshib/templates/registration/login.html
+-rw-r--r--   0        0        0     1012 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.3/modshib/templates/registration/reg_base.html
+-rw-r--r--   0        0        0      811 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.3/modshib/templates/registration/sso_fail.html
+-rw-r--r--   0        0        0      830 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.3/modshib/templates/registration/sso_no_account.html
+-rw-r--r--   0        0        0       60 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.3/modshib/tests.py
+-rw-r--r--   0        0        0      117 2023-05-24 14:07:03.824594 django_modshib_certic-0.1.3/modshib/urls.py
+-rw-r--r--   0        0        0     2746 2023-06-01 08:51:10.572109 django_modshib_certic-0.1.3/modshib/views.py
+-rw-r--r--   0        0        0      550 2023-06-01 09:00:19.076127 django_modshib_certic-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 django_modshib_certic-0.1.3/PKG-INFO
```

### Comparing `django-modshib-CERTIC-0.1.2/modshib/templates/registration/logged_out.html` & `django_modshib_certic-0.1.3/modshib/templates/registration/login.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 {% extends "registration/reg_base.html" %}
 {% load i18n %}
-{% block head_title %}{% translate "Déconnexion" %}{% endblock head_title %}
+{% block head_title %}{% translate "Connexion" %}{% endblock head_title %}
 {% block content %}
     <div class="d-flex flex-column min-vh-100 justify-content-center align-items-center">
         <div class="card" style="margin: 2em">
             <div class="card-body">
-                <h5 class="card-title">{{ site_name }}</h5>
-                <h6 class="card-subtitle mb-2 text-muted">{% translate "Déconnexion" %}</h6>
-                <div class="card-text">
-                    {% translate "Vous êtes déconnecté." %}
+                <h5 class="card-title">{% translate MODSHIB_FORMS_TITLE %}</h5>
+                <h6 class="card-subtitle mb-2 text-muted">{% translate "Connexion" %}</h6>
+                <div class="card-text d-grid gap-2">
+                    <a href="{% url "modshib_sso" %}" class="btn btn-primary">{% translate "Connexion via SSO" %}</a>
+                </div>
+                <div class="card-text" style="margin-top: 1em;">
+                    ou:
+                </div>
+                <div class="card-text" id="localForm">
+                    <form method="post" class="d-grid gap-2">
+                        {% csrf_token %}
+                        <table class="table">
+                            {{ form.as_table }}
+                        </table>
+                        <button class="btn btn-secondary" type="submit">{% translate "Connexion avec mot de passe" %}</button>
+                    </form>
                 </div>
-                <a href="/">{% translate "Retour à l'accueil" %}</a>
             </div>
         </div>
     </div>
-    {% if MODSHIB_SP_LOGOUT_URL %}
-        <iframe src="{{ MODSHIB_SP_LOGOUT_URL }}" style="display:none" title="SP Logout"></iframe>
-    {% endif %}
 {% endblock content %}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
 {% extends "registration/reg_base.html" %} {% load i18n %} {% block head_title
-%}{% translate "DÃ©connexion" %}{% endblock head_title %} {% block content %}
-** {{ site_name }} **
-* {% translate "DÃ©connexion" %} *
-{% translate "Vous Ãªtes dÃ©connectÃ©." %}
-{%_translate_"Retour_Ã _l'accueil"_%}
-{% if MODSHIB_SP_LOGOUT_URL %}  {% endif %} {% endblock content %}
+%}{% translate "Connexion" %}{% endblock head_title %} {% block content %}
+** {% translate MODSHIB_FORMS_TITLE %} **
+* {% translate "Connexion" %} *
+ %}" class="btn btn-primary">{% translate "Connexion via SSO" %}
+ou:
+{% csrf_token %}
+{% translate "Connexion avec mot de passe" %}
+{% endblock content %}
```

### Comparing `django-modshib-CERTIC-0.1.2/modshib/templates/registration/login.html` & `django_modshib_certic-0.1.3/modshib/templates/registration/logged_out.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 {% extends "registration/reg_base.html" %}
 {% load i18n %}
-{% block head_title %}{% translate "Connexion" %}{% endblock head_title %}
+{% block head_title %}{% translate "Déconnexion" %}{% endblock head_title %}
 {% block content %}
     <div class="d-flex flex-column min-vh-100 justify-content-center align-items-center">
         <div class="card" style="margin: 2em">
             <div class="card-body">
-                <h5 class="card-title">{{ site_name }}</h5>
-                <h6 class="card-subtitle mb-2 text-muted">{% translate "Connexion" %}</h6>
-                <div class="card-text d-grid gap-2">
-                    <a href="{% url "modshib_sso" %}" class="btn btn-primary">{% translate "Connection via SSO" %}</a>
-                </div>
-                <div class="card-text" style="margin-top: 1em;">
-                    ou:
-                </div>
-                <div class="card-text" id="localForm">
-                    <form method="post" class="d-grid gap-2">
-                        {% csrf_token %}
-                        <table class="table">
-                            {{ form.as_table }}
-                        </table>
-                        <button class="btn btn-secondary" type="submit">{% translate "Connexion avec mot de passe" %}</button>
-                    </form>
+                <h5 class="card-title">{% translate MODSHIB_FORMS_TITLE %}</h5>
+                <h6 class="card-subtitle mb-2 text-muted">{% translate "Déconnexion" %}</h6>
+                <div class="card-text">
+                    {% translate "Vous êtes déconnecté." %}
                 </div>
+                <a href="/">{% translate "Retour à l'accueil" %}</a>
             </div>
         </div>
     </div>
+    {% if MODSHIB_SP_LOGOUT_URL %}
+        <iframe src="{{ MODSHIB_SP_LOGOUT_URL }}" style="display:none" title="SP Logout"></iframe>
+    {% endif %}
 {% endblock content %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,9 +1,7 @@
 {% extends "registration/reg_base.html" %} {% load i18n %} {% block head_title
-%}{% translate "Connexion" %}{% endblock head_title %} {% block content %}
-** {{ site_name }} **
-* {% translate "Connexion" %} *
- %}" class="btn btn-primary">{% translate "Connection via SSO" %}
-ou:
-{% csrf_token %}
-{% translate "Connexion avec mot de passe" %}
-{% endblock content %}
+%}{% translate "DÃ©connexion" %}{% endblock head_title %} {% block content %}
+** {% translate MODSHIB_FORMS_TITLE %} **
+* {% translate "DÃ©connexion" %} *
+{% translate "Vous Ãªtes dÃ©connectÃ©." %}
+{%_translate_"Retour_Ã _l'accueil"_%}
+{% if MODSHIB_SP_LOGOUT_URL %}  {% endif %} {% endblock content %}
```

### Comparing `django-modshib-CERTIC-0.1.2/modshib/templates/registration/reg_base.html` & `django_modshib_certic-0.1.3/modshib/templates/registration/reg_base.html`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <title>{% block head_title %}Titre{% endblock head_title %} - {{ site_name }}</title>
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet"
           integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"
             integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4"
             crossorigin="anonymous"></script>
+    {% if MODSHIB_STYLESHEET_URL is not null %}
+        <link href="{{ MODSHIB_STYLESHEET_URL }}" rel="stylesheet" crossorigin="anonymous">
+    {% endif %}
 </head>
-<body>
+<body id="modshib-auth">
 {% block content %}
     Contenu ici
 {% endblock content %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,3 +1,5 @@
 {% load i18n %}
 
+ {% if MODSHIB_STYLESHEET_URL is not null %}
+ {% endif %}
 {% block content %} Contenu ici {% endblock content %}
```

### Comparing `django-modshib-CERTIC-0.1.2/modshib/templates/registration/sso_fail.html` & `django_modshib_certic-0.1.3/modshib/templates/registration/sso_fail.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% extends "registration/reg_base.html" %}
 {% load i18n %}
 {% block head_title %}{% translate "Connexion SSO" %}{% endblock head_title %}
 {% block content %}
     <div class="d-flex flex-column min-vh-100 justify-content-center align-items-center">
         <div class="card" style="margin: 2em">
             <div class="card-body">
-                <h5 class="card-title">{{ site_name }}</h5>
+                <h5 class="card-title">{% translate MODSHIB_FORMS_TITLE %}</h5>
                 <h6 class="card-subtitle mb-2 text-muted">{% translate "Connexion SSO" %}</h6>
                 <div class="card-text">
                     {% translate "Le SSO ne peut pas être contacté." %}
                 </div>
-                <a href="{{login_redirect}}">{% translate "Retour à la page d'authentification" %}</a>
+                <a href="{{ login_url }}">{% translate "Retour à la page d'authentification" %}</a>
             </div>
         </div>
     </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% extends "registration/reg_base.html" %} {% load i18n %} {% block head_title
 %}{% translate "Connexion SSO" %}{% endblock head_title %} {% block content %}
-** {{ site_name }} **
+** {% translate MODSHIB_FORMS_TITLE %} **
 * {% translate "Connexion SSO" %} *
 {% translate "Le SSO ne peut pas Ãªtre contactÃ©." %}
 {%_translate_"Retour_Ã _la_page_d'authentification"_%}
 {% endblock content %}
```

### Comparing `django-modshib-CERTIC-0.1.2/modshib/views.py` & `django_modshib_certic-0.1.3/modshib/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+from logging import Logger, INFO
+
 from django.conf import settings
-from django.http import HttpRequest, HttpResponse, HttpResponseRedirect
 from django.contrib.auth import login
 from django.contrib.auth.models import User, Group
+from django.http import HttpRequest, HttpResponse, HttpResponseRedirect
 from django.shortcuts import render
-from logging import Logger, INFO
 
 logger = Logger(name=__name__, level=INFO)
 
-
 try:
     CREATE_ACCOUNT = bool(settings.MODSHIB_CREATE_ACCOUNT)
 except AttributeError:
     CREATE_ACCOUNT = False
 
 try:
     ACTIVATE_ACCOUNT = bool(settings.MODSHIB_ACTIVATE_ACCOUNT)
 except AttributeError:
     ACTIVATE_ACCOUNT = False
 
+context = {"login_url": settings.LOGIN_URL}
+
 
 def sso(request: HttpRequest) -> HttpResponse:
     # nothing to do here...
     if request.user.is_authenticated:
         logger.info(
             f"User already authenticated, redirecting to {settings.LOGIN_REDIRECT_URL}"
         )
@@ -31,19 +33,15 @@
     eppn = request.META.get("HTTP_EPPN", None)
     supann_etablissement = request.META.get("HTTP_SUPANNETABLISSEMENT", None)
     # display_name = request.META.get("HTTP_DISPLAYNAME", None)
     mail = request.META.get("HTTP_MAIL", None)
     last_name = request.META.get("HTTP_SN", None)
     first_name = request.META.get("HTTP_GIVENNAME", None)
     if not eppn:
-        return render(
-            request,
-            "registration/sso_fail.html",
-            {"login_redirect": settings.LOGIN_URL},
-        )
+        return render(request, "registration/sso_fail.html", context)
 
     # find account
     eppn = eppn.strip()
     user = User.objects.filter(username=eppn).first()
     if not user and CREATE_ACCOUNT:
         logger.info(f"user {eppn} not found, creating account")
         user = User.objects.create_user(eppn)
@@ -58,20 +56,20 @@
         if supann_etablissement:
             group, created = Group.objects.get_or_create(
                 name=f"supann_{supann_etablissement}"
             )
             user.groups.add(group)
     if not user:
         logger.info(f"user {eppn} not found, rejecting auth")
-        return render(request, "registration/sso_no_account.html")
+        return render(request, "registration/sso_no_account.html", context)
     if not user.is_active and ACTIVATE_ACCOUNT:
         logger.info(f"user {eppn} not active, activating")
         user.is_active = True
         user.save()
     if not user.is_active:
         logger.info(f"user {eppn} inactive, rejecting auth")
-        return render(request, "registration/sso_no_account.html")
+        return render(request, "registration/sso_no_account.html", context)
     if user and user.is_active:
         logger.info(f"active user {eppn} found, login")
         request.session["auth_is_from_modshib"] = True
         login(request, user)
         return HttpResponseRedirect(settings.LOGIN_REDIRECT_URL)
```

### Comparing `django-modshib-CERTIC-0.1.2/pyproject.toml` & `django_modshib_certic-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "django-modshib-CERTIC"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Mickaël Desfrênes <mickael.desfrenes@unicaen.fr>"]
 license = "Cecill-B"
 packages = [
     { include = "modshib"},
 ]
 homepage = "https://www.certic.unicaen.fr"
 repository = "https://git.unicaen.fr/certic/django-modshib"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = "^3.9"
 Django = ">=4.0"
 django-auth-cli-certic = ">=0.1.3"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 
 [build-system]
```

### Comparing `django-modshib-CERTIC-0.1.2/PKG-INFO` & `django_modshib_certic-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: django-modshib-certic
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://www.certic.unicaen.fr
 License: CECILL-B
 Author: Mickaël Desfrênes
 Author-email: mickael.desfrenes@unicaen.fr
-Requires-Python: >=3.7
+Requires-Python: >=3.9,<4.0
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=4.0)
 Requires-Dist: django-auth-cli-certic (>=0.1.3)
 Project-URL: Repository, https://git.unicaen.fr/certic/django-modshib
```

