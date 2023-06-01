# Comparing `tmp/django-project-center-0.5.tar.gz` & `tmp/django-project-center-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-center-0.5.tar", last modified: Mon Mar  6 18:48:12 2023, max compression
+gzip compressed data, was "django-project-center-0.6.tar", last modified: Thu Jun  1 10:33:16 2023, max compression
```

## Comparing `django-project-center-0.5.tar` & `django-project-center-0.6.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.837904 django-project-center-0.5/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 django-project-center-0.5/LICENCE.txt
--rw-rw-rw-   0        0        0      365 2023-03-06 18:48:12.837904 django-project-center-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 django-project-center-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.766903 django-project-center-0.5/django_project_center.egg-info/
--rw-rw-rw-   0        0        0      365 2023-03-06 18:48:12.000000 django-project-center-0.5/django_project_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1422 2023-03-06 18:48:12.000000 django-project-center-0.5/django_project_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 18:48:12.000000 django-project-center-0.5/django_project_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-29 17:53:35.000000 django-project-center-0.5/django_project_center.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-03-06 18:48:12.000000 django-project-center-0.5/django_project_center.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.780903 django-project-center-0.5/project_center/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-0.5/project_center/__init__.py
--rw-rw-rw-   0        0        0    13635 2023-03-06 18:46:17.000000 django-project-center-0.5/project_center/admin.py
--rw-rw-rw-   0        0        0      202 2023-03-06 13:02:17.000000 django-project-center-0.5/project_center/apps.py
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.781903 django-project-center-0.5/project_center/management/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 django-project-center-0.5/project_center/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.790902 django-project-center-0.5/project_center/management/commands/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 django-project-center-0.5/project_center/management/commands/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-02-05 20:44:22.000000 django-project-center-0.5/project_center/management/commands/send_project_alert_email.py
--rw-rw-rw-   0        0        0     1738 2023-01-29 14:46:48.000000 django-project-center-0.5/project_center/management/commands/setup_project_center.py
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.833905 django-project-center-0.5/project_center/migrations/
--rw-rw-rw-   0        0        0    12997 2023-01-28 19:12:29.000000 django-project-center-0.5/project_center/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      405 2023-02-05 19:27:59.000000 django-project-center-0.5/project_center/migrations/0002_user_email_notify.py
--rw-rw-rw-   0        0        0      424 2023-02-15 11:57:39.000000 django-project-center-0.5/project_center/migrations/0003_projectactivity_notes.py
--rw-rw-rw-   0        0        0      424 2023-02-16 02:02:07.000000 django-project-center-0.5/project_center/migrations/0004_projectcategory_display.py
--rw-rw-rw-   0        0        0      424 2023-02-16 02:06:16.000000 django-project-center-0.5/project_center/migrations/0005_projectstatus_display.py
--rw-rw-rw-   0        0        0      421 2023-02-16 02:06:34.000000 django-project-center-0.5/project_center/migrations/0006_projectstage_display.py
--rw-rw-rw-   0        0        0      827 2023-03-03 02:55:14.000000 django-project-center-0.5/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py
--rw-rw-rw-   0        0        0     1744 2023-03-05 20:22:08.000000 django-project-center-0.5/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py
--rw-rw-rw-   0        0        0      861 2023-03-05 20:29:12.000000 django-project-center-0.5/project_center/migrations/0009_projectactivity_reply_file_and_more.py
--rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-0.5/project_center/migrations/__init__.py
--rw-rw-rw-   0        0        0    12643 2023-03-06 17:53:22.000000 django-project-center-0.5/project_center/models.py
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.835904 django-project-center-0.5/project_center/signals/
--rw-rw-rw-   0        0        0        0 2023-03-06 12:44:24.000000 django-project-center-0.5/project_center/signals/__init__.py
--rw-rw-rw-   0        0        0      367 2023-03-06 12:58:21.000000 django-project-center-0.5/project_center/signals/handlers.py
--rw-rw-rw-   0        0        0      188 2023-02-01 19:52:44.000000 django-project-center-0.5/project_center/storage_backends.py
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.835904 django-project-center-0.5/project_center/templates/
--rw-rw-rw-   0        0        0        0 2023-02-05 20:00:02.000000 django-project-center-0.5/project_center/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 18:48:12.836905 django-project-center-0.5/project_center/templates/email/
--rw-rw-rw-   0        0        0        0 2023-02-05 20:03:52.000000 django-project-center-0.5/project_center/templates/email/__init__.py
--rw-rw-rw-   0        0        0       63 2023-01-28 18:09:02.000000 django-project-center-0.5/project_center/tests.py
--rw-rw-rw-   0        0        0      193 2023-02-05 20:17:46.000000 django-project-center-0.5/project_center/utils.py
--rw-rw-rw-   0        0        0     1071 2023-03-05 17:48:01.000000 django-project-center-0.5/project_center/views.py
--rw-rw-rw-   0        0        0       42 2023-03-06 18:48:12.837904 django-project-center-0.5/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-03-06 18:47:39.000000 django-project-center-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.381231 django-project-center-0.6/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 django-project-center-0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0      365 2023-06-01 10:33:16.381231 django-project-center-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 django-project-center-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.286229 django-project-center-0.6/django_project_center.egg-info/
+-rw-rw-rw-   0        0        0      365 2023-06-01 10:33:16.000000 django-project-center-0.6/django_project_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1477 2023-06-01 10:33:16.000000 django-project-center-0.6/django_project_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 10:33:16.000000 django-project-center-0.6/django_project_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-29 17:53:35.000000 django-project-center-0.6/django_project_center.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2023-06-01 10:33:16.000000 django-project-center-0.6/django_project_center.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.317229 django-project-center-0.6/project_center/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-0.6/project_center/__init__.py
+-rw-rw-rw-   0        0        0    13608 2023-05-29 21:03:40.000000 django-project-center-0.6/project_center/admin.py
+-rw-rw-rw-   0        0        0      202 2023-03-06 13:02:17.000000 django-project-center-0.6/project_center/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.318230 django-project-center-0.6/project_center/management/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 django-project-center-0.6/project_center/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.333230 django-project-center-0.6/project_center/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 django-project-center-0.6/project_center/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1507 2023-04-09 00:02:35.000000 django-project-center-0.6/project_center/management/commands/check_aws_access.py
+-rw-rw-rw-   0        0        0     3694 2023-05-30 16:51:15.000000 django-project-center-0.6/project_center/management/commands/send_project_alert_email.py
+-rw-rw-rw-   0        0        0     1738 2023-05-29 21:02:54.000000 django-project-center-0.6/project_center/management/commands/setup_project_center.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.373231 django-project-center-0.6/project_center/migrations/
+-rw-rw-rw-   0        0        0    12997 2023-01-28 19:12:29.000000 django-project-center-0.6/project_center/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      405 2023-02-05 19:27:59.000000 django-project-center-0.6/project_center/migrations/0002_user_email_notify.py
+-rw-rw-rw-   0        0        0      424 2023-02-15 11:57:39.000000 django-project-center-0.6/project_center/migrations/0003_projectactivity_notes.py
+-rw-rw-rw-   0        0        0      424 2023-02-16 02:02:07.000000 django-project-center-0.6/project_center/migrations/0004_projectcategory_display.py
+-rw-rw-rw-   0        0        0      424 2023-02-16 02:06:16.000000 django-project-center-0.6/project_center/migrations/0005_projectstatus_display.py
+-rw-rw-rw-   0        0        0      421 2023-02-16 02:06:34.000000 django-project-center-0.6/project_center/migrations/0006_projectstage_display.py
+-rw-rw-rw-   0        0        0      827 2023-03-03 02:55:14.000000 django-project-center-0.6/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py
+-rw-rw-rw-   0        0        0     1744 2023-03-05 20:22:08.000000 django-project-center-0.6/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py
+-rw-rw-rw-   0        0        0      861 2023-03-05 20:29:12.000000 django-project-center-0.6/project_center/migrations/0009_projectactivity_reply_file_and_more.py
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:09:02.000000 django-project-center-0.6/project_center/migrations/__init__.py
+-rw-rw-rw-   0        0        0    12946 2023-05-31 16:16:39.000000 django-project-center-0.6/project_center/models.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.379229 django-project-center-0.6/project_center/signals/
+-rw-rw-rw-   0        0        0        0 2023-03-06 12:44:24.000000 django-project-center-0.6/project_center/signals/__init__.py
+-rw-rw-rw-   0        0        0      367 2023-03-06 12:58:21.000000 django-project-center-0.6/project_center/signals/handlers.py
+-rw-rw-rw-   0        0        0      188 2023-02-01 19:52:44.000000 django-project-center-0.6/project_center/storage_backends.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.380232 django-project-center-0.6/project_center/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-05 20:00:02.000000 django-project-center-0.6/project_center/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 10:33:16.380232 django-project-center-0.6/project_center/templates/email/
+-rw-rw-rw-   0        0        0        0 2023-02-05 20:03:52.000000 django-project-center-0.6/project_center/templates/email/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-01-28 18:09:02.000000 django-project-center-0.6/project_center/tests.py
+-rw-rw-rw-   0        0        0      193 2023-02-05 20:17:46.000000 django-project-center-0.6/project_center/utils.py
+-rw-rw-rw-   0        0        0     1071 2023-03-05 17:48:01.000000 django-project-center-0.6/project_center/views.py
+-rw-rw-rw-   0        0        0       42 2023-06-01 10:33:16.381231 django-project-center-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-06-01 10:32:11.000000 django-project-center-0.6/setup.py
```

### Comparing `django-project-center-0.5/django_project_center.egg-info/SOURCES.txt` & `django-project-center-0.6/django_project_center.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 project_center/models.py
 project_center/storage_backends.py
 project_center/tests.py
 project_center/utils.py
 project_center/views.py
 project_center/management/__init__.py
 project_center/management/commands/__init__.py
+project_center/management/commands/check_aws_access.py
 project_center/management/commands/send_project_alert_email.py
 project_center/management/commands/setup_project_center.py
 project_center/migrations/0001_initial.py
 project_center/migrations/0002_user_email_notify.py
 project_center/migrations/0003_projectactivity_notes.py
 project_center/migrations/0004_projectcategory_display.py
 project_center/migrations/0005_projectstatus_display.py
```

### Comparing `django-project-center-0.5/project_center/admin.py` & `django-project-center-0.6/project_center/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.utils.text import Truncator
 from django.conf import settings
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 from django.contrib.admin import RelatedOnlyFieldListFilter
 from django.utils import timezone
 
-from .models import User, Project, ProjectCategory, ProjectStatus, ProjectStage, ProjectActivity, Company, Activity
+from .models import User, Project, ProjectCategory, ProjectStatus, ProjectStage, ProjectActivity, Company
 
 class ProjectCenterUserForm(UserChangeForm):
     class Meta:
         model = User
         fields = '__all__'
         labels = {
             "is_staff": "Can Login"
@@ -116,14 +116,15 @@
         return False
 
 
 class ProjectAdmin(admin.ModelAdmin):
     list_display_links = ['id', 'title']
     list_display = ('id', 'title', 'date', 'company', 'last_activity', 'status', 'stage', 'category', 'internal')
     list_filter = ['company', 'category', 'status', 'stage', 'internal']
+    list_editable = ['category', 'status', 'stage', 'internal']
     search_fields = ['title', 'code', ]
     filter_horizontal = ['users']
     ordering = ['-date']
     inlines = [ProjectActivityInline]
     fieldsets = (
 
         (_("Project info"), {"fields": ("title", ("company", "category"), ("status", "stage", "internal"), 'date',
@@ -292,15 +293,15 @@
 
     project_link.short_description = 'Project'
 
     def user_link(self, obj):
         return mark_safe('<a href="{}">{}</a>'.format(
             reverse("admin:project_center_user_change", args=(obj.user.pk,)),
             obj.user.get_full_name()
-        ))
+        )) if obj.user else ''
 
     user_link.short_description = 'User'
 
     def activity_link(self, obj):
         return mark_safe('<a href="{}">{}</a>'.format(
             reverse("admin:project_center_activity_change", args=(obj.pk,)),
             obj.name()
@@ -346,12 +347,7 @@
 class ProjectStageAdmin(admin.ModelAdmin):
     list_display = ('id', 'name', 'display')
 
 
 admin.site.register(ProjectStage, ProjectStageAdmin)
 
 admin.site.register(User, ProjectCenterUserAdmin)
-
-class ActivityAdmin(ProjectActivityAdmin):
-    pass
-
-admin.site.register(Activity, ActivityAdmin)
```

### Comparing `django-project-center-0.5/project_center/management/commands/setup_project_center.py` & `django-project-center-0.6/project_center/management/commands/setup_project_center.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.5/project_center/migrations/0001_initial.py` & `django-project-center-0.6/project_center/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.5/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py` & `django-project-center-0.6/project_center/migrations/0007_alter_company_options_alter_user_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.5/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py` & `django-project-center-0.6/project_center/migrations/0008_activity_projectactivity_reply_alter_project_users_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.5/project_center/migrations/0009_projectactivity_reply_file_and_more.py` & `django-project-center-0.6/project_center/migrations/0009_projectactivity_reply_file_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.5/project_center/models.py` & `django-project-center-0.6/project_center/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -228,18 +228,31 @@
 
     def last_activity(self):
         return self.projectactivity_set.order_by('-date').first()
 
     def last_activity_date(self):
         return self.last_activity().date
 
+    def category_name(self):
+        return self.category.name if self.category else None
+
+    def get_absolute_url(self):
+        return reverse('project-detail', args=[self.id])
+
+    def send_group_alert(self, message=None):
+        for user in self.users.all():
+            print(user)
+
 
 def activity_file_directory_path(instance, filename):
     # file will be uploaded to MEDIA_ROOT/user_<id>/<filename>
-    return 'project_activity_files/{0}/{1}'.format(instance.project.slug, os.path.basename(filename))
+    try:
+        return 'project_activity_files/{0}/{1}'.format(instance.project.slug, os.path.basename(filename))
+    except:
+        return None
 
 
 class ProjectActivity(models.Model):
     import_id = models.IntegerField(_('Import ID'), blank=True, null=True, default=None, help_text='Import ID')
     name = models.CharField(_('Activity Name'), max_length=255, blank=False, help_text='Activity Name')
     user = models.ForeignKey(User, blank=True, null=True, default=None, on_delete=models.SET_NULL)
     project = models.ForeignKey(Project, blank=True, null=True, default=None, on_delete=models.CASCADE)
@@ -277,24 +290,19 @@
             return mark_safe(
                 '<a href="' + reverse('activity-download', args=[self.id]) + '">' + self.get_filename() + '</a>')
         else:
             return None
 
     get_download_link.short_description = 'Download Link'
 
+    @staticmethod
+    def autocomplete_search_fields():
+        return ("id__iexact", "name__icontains",)
+
     # def save(
     #     self, force_insert=False, force_update=False, using=None, update_fields=None
     # ):
     #
     #     if self.reply:
     #         return self
     #     else:
     #         return super()
-
-
-
-
-class Activity(ProjectActivity):
-    class Meta:
-        proxy = True
-        verbose_name = 'Activity'
-        verbose_name_plural = 'Activity'
```

### Comparing `django-project-center-0.5/project_center/views.py` & `django-project-center-0.6/project_center/views.py`

 * *Files identical despite different names*

### Comparing `django-project-center-0.5/setup.py` & `django-project-center-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = []
 
 setup(
     name='django-project-center',
-    version='0.5',
+    version='0.6',
     description='Project Management Module for Django',
     author='siteshell.net',
     author_email='pdbethke@siteshell.net',
     url='https://github.com/pdbethke/django-project-center',
     packages=find_packages(),
     license='LICENSE.txt',
     platforms=['OS Independent'],
```

