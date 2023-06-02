# Comparing `tmp/netbox-is-risks-0.1.3.tar.gz` & `tmp/netbox-is-risks-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-is-risks-0.1.3.tar", last modified: Thu Sep 29 11:24:48 2022, max compression
+gzip compressed data, was "netbox-is-risks-0.1.4.tar", last modified: Fri Jun  2 09:11:58 2023, max compression
```

## Comparing `netbox-is-risks-0.1.3.tar` & `netbox-is-risks-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/
--rw-rw-r--   0 user      (1000) user      (1000)     1071 2022-05-24 10:38:36.000000 netbox-is-risks-0.1.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       30 2022-06-03 08:24:52.000000 netbox-is-risks-0.1.3/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     1527 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      922 2022-05-26 11:17:16.000000 netbox-is-risks-0.1.3/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/netbox_is_risks.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1527 2022-09-29 11:24:48.000000 netbox-is-risks-0.1.3/netbox_is_risks.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      712 2022-09-29 11:24:48.000000 netbox-is-risks-0.1.3/netbox_is_risks.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-29 11:24:48.000000 netbox-is-risks-0.1.3/netbox_is_risks.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-22 13:36:29.000000 netbox-is-risks-0.1.3/netbox_is_risks.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)        6 2022-09-29 11:24:48.000000 netbox-is-risks-0.1.3/netbox_is_risks.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/risks/
--rw-rw-r--   0 user      (1000) user      (1000)      350 2022-05-26 10:16:25.000000 netbox-is-risks-0.1.3/risks/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/risks/api/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-24 15:50:18.000000 netbox-is-risks-0.1.3/risks/api/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2843 2022-09-22 13:30:36.000000 netbox-is-risks-0.1.3/risks/api/serializers.py
--rw-rw-r--   0 user      (1000) user      (1000)      310 2022-05-24 21:19:33.000000 netbox-is-risks-0.1.3/risks/api/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)      757 2022-05-24 21:24:29.000000 netbox-is-risks-0.1.3/risks/api/views.py
--rw-rw-r--   0 user      (1000) user      (1000)      839 2022-05-24 21:23:56.000000 netbox-is-risks-0.1.3/risks/filtersets.py
--rw-rw-r--   0 user      (1000) user      (1000)      813 2022-05-26 10:45:43.000000 netbox-is-risks-0.1.3/risks/forms.py
--rw-rw-r--   0 user      (1000) user      (1000)      981 2022-05-26 10:39:11.000000 netbox-is-risks-0.1.3/risks/graphql.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/risks/migrations/
--rw-rw-r--   0 user      (1000) user      (1000)     3183 2022-05-26 10:39:26.000000 netbox-is-risks-0.1.3/risks/migrations/0001_initial.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-26 10:39:26.000000 netbox-is-risks-0.1.3/risks/migrations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2655 2022-09-29 10:04:37.000000 netbox-is-risks-0.1.3/risks/models.py
--rw-rw-r--   0 user      (1000) user      (1000)      823 2022-05-24 21:42:47.000000 netbox-is-risks-0.1.3/risks/navigation.py
--rw-rw-r--   0 user      (1000) user      (1000)     1323 2022-05-24 21:27:13.000000 netbox-is-risks-0.1.3/risks/tables.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2022-05-26 11:04:39.000000 netbox-is-risks-0.1.3/risks/template_content.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:24:48.105229 netbox-is-risks-0.1.3/risks/templates/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/risks/templates/risks/
--rw-rw-r--   0 user      (1000) user      (1000)      785 2022-05-26 10:44:39.000000 netbox-is-risks-0.1.3/risks/templates/risks/risk.html
--rw-rw-r--   0 user      (1000) user      (1000)     1439 2022-05-26 11:02:12.000000 netbox-is-risks-0.1.3/risks/templates/risks/risk_panel.html
--rw-rw-r--   0 user      (1000) user      (1000)      586 2022-05-24 21:39:23.000000 netbox-is-risks-0.1.3/risks/templates/risks/riskassignment_edit.html
--rw-rw-r--   0 user      (1000) user      (1000)      694 2022-05-24 17:47:12.000000 netbox-is-risks-0.1.3/risks/templates/risks/riskrelation.html
--rw-rw-r--   0 user      (1000) user      (1000)     1782 2022-05-24 21:37:29.000000 netbox-is-risks-0.1.3/risks/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     2526 2022-05-26 10:30:05.000000 netbox-is-risks-0.1.3/risks/views.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-09-29 11:24:48.109229 netbox-is-risks-0.1.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      954 2022-09-29 10:08:02.000000 netbox-is-risks-0.1.3/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:11:58.220787 netbox-is-risks-0.1.4/
+-rw-rw-r--   0 user      (1000) user      (1000)     1071 2022-05-24 10:38:36.000000 netbox-is-risks-0.1.4/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       30 2022-06-03 08:24:52.000000 netbox-is-risks-0.1.4/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     1527 2023-06-02 09:11:58.220787 netbox-is-risks-0.1.4/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      922 2022-05-26 11:17:16.000000 netbox-is-risks-0.1.4/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:11:58.212787 netbox-is-risks-0.1.4/netbox_is_risks.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1527 2023-06-02 09:11:58.000000 netbox-is-risks-0.1.4/netbox_is_risks.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-06-02 09:11:58.000000 netbox-is-risks-0.1.4/netbox_is_risks.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-02 09:11:58.000000 netbox-is-risks-0.1.4/netbox_is_risks.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-22 13:36:29.000000 netbox-is-risks-0.1.4/netbox_is_risks.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-06-02 09:11:58.000000 netbox-is-risks-0.1.4/netbox_is_risks.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:11:58.216787 netbox-is-risks-0.1.4/risks/
+-rw-rw-r--   0 user      (1000) user      (1000)      350 2022-05-26 10:16:25.000000 netbox-is-risks-0.1.4/risks/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:11:58.216787 netbox-is-risks-0.1.4/risks/api/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-24 15:50:18.000000 netbox-is-risks-0.1.4/risks/api/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2843 2022-09-22 13:30:36.000000 netbox-is-risks-0.1.4/risks/api/serializers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      310 2022-05-24 21:19:33.000000 netbox-is-risks-0.1.4/risks/api/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)      757 2022-05-24 21:24:29.000000 netbox-is-risks-0.1.4/risks/api/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)      839 2022-05-24 21:23:56.000000 netbox-is-risks-0.1.4/risks/filtersets.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-26 10:26:33.000000 netbox-is-risks-0.1.4/risks/forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)      981 2022-05-26 10:39:11.000000 netbox-is-risks-0.1.4/risks/graphql.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:11:58.220787 netbox-is-risks-0.1.4/risks/migrations/
+-rw-rw-r--   0 user      (1000) user      (1000)     3183 2022-05-26 10:39:26.000000 netbox-is-risks-0.1.4/risks/migrations/0001_initial.py
+-rw-rw-r--   0 user      (1000) user      (1000)      690 2023-01-16 14:28:25.000000 netbox-is-risks-0.1.4/risks/migrations/0002_alter_risk_custom_field_data_and_more.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-26 10:39:26.000000 netbox-is-risks-0.1.4/risks/migrations/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2655 2023-05-26 09:07:58.000000 netbox-is-risks-0.1.4/risks/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      823 2022-05-24 21:42:47.000000 netbox-is-risks-0.1.4/risks/navigation.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1323 2022-05-24 21:27:13.000000 netbox-is-risks-0.1.4/risks/tables.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2186 2023-01-16 15:12:52.000000 netbox-is-risks-0.1.4/risks/template_content.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:11:58.212787 netbox-is-risks-0.1.4/risks/templates/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:11:58.220787 netbox-is-risks-0.1.4/risks/templates/risks/
+-rw-rw-r--   0 user      (1000) user      (1000)      785 2022-05-26 10:44:39.000000 netbox-is-risks-0.1.4/risks/templates/risks/risk.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1439 2022-05-26 11:02:12.000000 netbox-is-risks-0.1.4/risks/templates/risks/risk_panel.html
+-rw-rw-r--   0 user      (1000) user      (1000)      586 2022-05-24 21:39:23.000000 netbox-is-risks-0.1.4/risks/templates/risks/riskassignment_edit.html
+-rw-rw-r--   0 user      (1000) user      (1000)      694 2022-05-24 17:47:12.000000 netbox-is-risks-0.1.4/risks/templates/risks/riskrelation.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1782 2022-05-24 21:37:29.000000 netbox-is-risks-0.1.4/risks/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2526 2022-05-26 10:30:05.000000 netbox-is-risks-0.1.4/risks/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-02 09:11:58.220787 netbox-is-risks-0.1.4/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      954 2023-06-02 09:11:36.000000 netbox-is-risks-0.1.4/setup.py
```

### Comparing `netbox-is-risks-0.1.3/LICENSE` & `netbox-is-risks-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/PKG-INFO` & `netbox-is-risks-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-is-risks
-Version: 0.1.3
+Version: 0.1.4
 Summary: Netbox plugin. Assign devices and virtual machines to information security risks
 Download-URL: https://pypi.org/project/netbox-is-risks/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
```

### Comparing `netbox-is-risks-0.1.3/README.md` & `netbox-is-risks-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/netbox_is_risks.egg-info/PKG-INFO` & `netbox-is-risks-0.1.4/netbox_is_risks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-is-risks
-Version: 0.1.3
+Version: 0.1.4
 Summary: Netbox plugin. Assign devices and virtual machines to information security risks
 Download-URL: https://pypi.org/project/netbox-is-risks/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
```

### Comparing `netbox-is-risks-0.1.3/netbox_is_risks.egg-info/SOURCES.txt` & `netbox-is-risks-0.1.4/netbox_is_risks.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 risks/urls.py
 risks/views.py
 risks/api/__init__.py
 risks/api/serializers.py
 risks/api/urls.py
 risks/api/views.py
 risks/migrations/0001_initial.py
+risks/migrations/0002_alter_risk_custom_field_data_and_more.py
 risks/migrations/__init__.py
 risks/templates/risks/risk.html
 risks/templates/risks/risk_panel.html
 risks/templates/risks/riskassignment_edit.html
 risks/templates/risks/riskrelation.html
```

### Comparing `netbox-is-risks-0.1.3/risks/api/serializers.py` & `netbox-is-risks-0.1.4/risks/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/api/views.py` & `netbox-is-risks-0.1.4/risks/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/filtersets.py` & `netbox-is-risks-0.1.4/risks/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/graphql.py` & `netbox-is-risks-0.1.4/risks/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/migrations/0001_initial.py` & `netbox-is-risks-0.1.4/risks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/models.py` & `netbox-is-risks-0.1.4/risks/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         # return 'reskrel'
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:risks:riskrelation', args=[self.pk])
 
 
-class RiskAssignment(WebhooksMixin, ChangeLoggedModel):
+class RiskAssignment(ChangeLoggedModel, WebhooksMixin):
     content_type = models.ForeignKey(
         to=ContentType,
         on_delete=models.CASCADE
     )
     object_id = models.PositiveBigIntegerField()
     object = GenericForeignKey(
         ct_field='content_type',
```

### Comparing `netbox-is-risks-0.1.3/risks/navigation.py` & `netbox-is-risks-0.1.4/risks/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/tables.py` & `netbox-is-risks-0.1.4/risks/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/template_content.py` & `netbox-is-risks-0.1.4/risks/template_content.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,36 @@
             })
 
         return self.render('risks/risk_panel.html', extra_context={
             'risks': risks
         })
 
 
+class RiskAppSystemPanel(PluginTemplateExtension):
+    model = 'netbox_app_systems.AppSystem'
+
+    def right_page(self):
+        app_system = self.context['object']
+        content_type_id = ContentType.objects.get_for_model(
+            model=app_system).id
+        risk_ass = RiskAssignment.objects.filter(
+            object_id=app_system.id, content_type=content_type_id)
+        risks = []
+        for r in risk_ass:
+            risks.append({
+                'assignment_id': r.id,
+                'name': r.risk,
+                'rel': r.relation.name
+            })
+
+        return self.render('risks/risk_panel.html', extra_context={
+            'risks': risks
+        })
+
+
 class RiskDevicePanel(PluginTemplateExtension):
     model = 'dcim.device'
 
     def right_page(self):
         device = self.context['object']
         content_type_id = ContentType.objects.get_for_model(model=device).id
         risk_ass = RiskAssignment.objects.filter(
@@ -41,8 +63,8 @@
             })
 
         return self.render('risks/risk_panel.html', extra_context={
             'risks': risks
         })
 
 
-template_extensions = [RiskVMPanel, RiskDevicePanel]
+template_extensions = [RiskVMPanel, RiskDevicePanel, RiskAppSystemPanel]
```

### Comparing `netbox-is-risks-0.1.3/risks/templates/risks/risk.html` & `netbox-is-risks-0.1.4/risks/templates/risks/risk.html`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/templates/risks/risk_panel.html` & `netbox-is-risks-0.1.4/risks/templates/risks/risk_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/templates/risks/riskassignment_edit.html` & `netbox-is-risks-0.1.4/risks/templates/risks/riskassignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/templates/risks/riskrelation.html` & `netbox-is-risks-0.1.4/risks/templates/risks/riskrelation.html`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/urls.py` & `netbox-is-risks-0.1.4/risks/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/risks/views.py` & `netbox-is-risks-0.1.4/risks/views.py`

 * *Files identical despite different names*

### Comparing `netbox-is-risks-0.1.3/setup.py` & `netbox-is-risks-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='netbox-is-risks',
-    version='0.1.3',
+    version='0.1.4',
     description='Netbox plugin. Assign devices and virtual machines to information security risks',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     download_url='https://pypi.org/project/netbox-is-risks/',
     packages=find_packages(),
     include_package_data=True,
```

