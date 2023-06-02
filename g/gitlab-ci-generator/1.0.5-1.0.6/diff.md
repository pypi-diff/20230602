# Comparing `tmp/gitlab-ci-generator-1.0.5.tar.gz` & `tmp/gitlab-ci-generator-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-ci-generator-1.0.5.tar", last modified: Tue May 16 20:16:36 2023, max compression
+gzip compressed data, was "gitlab-ci-generator-1.0.6.tar", last modified: Fri Jun  2 18:47:23 2023, max compression
```

## Comparing `gitlab-ci-generator-1.0.5.tar` & `gitlab-ci-generator-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/
--rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/MANIFEST.in
--rw-r--r--   0 developer  (9999) developer  (9999)     8787 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/PKG-INFO
--rw-rw-rw-   0 developer  (9999) developer  (9999)     8438 2023-05-16 20:16:20.000000 gitlab-ci-generator-1.0.5/README.md
--rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/VERSION.txt
--rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/setup.cfg
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/setup.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/
--rw-r--r--   0 developer  (9999) developer  (9999)     8787 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/PKG-INFO
--rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/entry_points.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/requires.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/
--rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/__init__.py
--rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/gitlab_ci_generator.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/templates/
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1933 2023-05-16 20:06:50.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/MANIFEST.in
+-rw-r--r--   0 developer  (9999) developer  (9999)     9571 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/PKG-INFO
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     9222 2023-06-02 18:47:08.000000 gitlab-ci-generator-1.0.6/README.md
+-rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/VERSION.txt
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/setup.cfg
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/setup.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/
+-rw-r--r--   0 developer  (9999) developer  (9999)     9571 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/requires.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/__init__.py
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/gitlab_ci_generator.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/templates/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     2045 2023-06-02 18:47:08.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
```

### Comparing `gitlab-ci-generator-1.0.5/PKG-INFO` & `gitlab-ci-generator-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.5
+Version: 1.0.6
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
 Description-Content-Type: text/markdown
@@ -20,20 +20,20 @@
 This installs like an executable and you can simply run: 
 ```
 gitlab-ci-generator
 ```
 
 ## Usage
 The project takes the following parameters:
-|Name|Parameter|Description|Required|
-|-----|--------|-----------|--------|
-|Input File|--inputfile/-f|The yaml file that will be used to render the gitlab ci file.|Yes|
-|Output File|--outputfile/-o|The yaml file that is rendered using the jinja2 template with data from the input yaml file.|No|
-|Template File|--templatefile/-t|A jinja2 file that can be used to override default templating|No|
-|Help|-h|Displays help info|No|
+| Name          | Parameter         | Description                                                                                  | Required |
+| ------------- | ----------------- | -------------------------------------------------------------------------------------------- | -------- |
+| Input File    | --inputfile/-f    | The yaml file that will be used to render the gitlab ci file.                                | Yes      |
+| Output File   | --outputfile/-o   | The yaml file that is rendered using the jinja2 template with data from the input yaml file. | No       |
+| Template File | --templatefile/-t | A jinja2 file that can be used to override default templating                                | No       |
+| Help          | -h                | Displays help info                                                                           | No       |
 
 This program will load the input yaml file into two distinct dictionaries that are available to the template:
 * pipeline_info
 * jobs
 
 To run without specifying an output file you can write stdout to a redirect file like so: 
 ```
@@ -43,14 +43,17 @@
 ### pipeline_info
 This section is gets loaded as is into a dictionary so you can easily extend it for your needs.  The built-in template uses the following:
 ```
 pipeline_info:
   shared_includes: <<-- Used by the template to build the include: section of the gitlab ci file.
     - name: rules <<-- List of includes and can be of type local or project.  The rules example here is used in the template in concert with the share_reference_rules: section to define dynamic rules for jobs.
       local: "example/example-config/rules.yml" 
+  shared_variables: << -- Used by the template to build the variables: section of the gitlab ci under each job.
+    - name: MYVAR <-- The variable name to include
+      value: MYVAR_VALUE <-- The value string or a variable for the value 
   shared_reference_rules: <<-- Used by the template to build the rules: section of the gitlab ci under each job.
     - rule_name: standard-rule-if <- The rule_source and rule_name will create a !reference[rule_source, rule_name] value under the rules section of each job.
       rule_source: .job_changes_rules
       only_changes: true
   final_job: <<-- Optional section that can be used to specify a final trigger job to run at the end of your pipeline.
     name: <<-- The name of the final job.
     stage: <<-- The stage that you want the final job to run in.
@@ -81,14 +84,17 @@
 This sample can also be found in the gitlab repo for this project at the location [example/example-config/job-dependency.yml](https://gitlab.com/gary.schaetz/public/gitlab-ci-generator/-/blob/main/example/example-config/job-dependency.yml)
 ```
 ---
 pipeline_info:
   shared_includes:
     - name: rules
       local: "example/example-config/rules.yml"
+  shared_variables:
+    - name: MYVAR
+      value: MYVAR_VALUE
   shared_reference_rules:
     - rule_name: standard-rule-if
       rule_source: .job_changes_rules
       only_changes: true
     - rule_name:  manual-rule-if
       rule_source: .job_changes_rules
       when: manual
@@ -128,14 +134,15 @@
   - post-deploy
 
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
     PROJECT_JOB_NAME: example-1
+    MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
       changes:
@@ -146,14 +153,15 @@
     strategy: depend
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
+    MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
```

### Comparing `gitlab-ci-generator-1.0.5/README.md` & `gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: gitlab-ci-generator
+Version: 1.0.6
+Summary: Generates a mono-repo ci file.
+Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
+Author: Gary Schaetz
+Author-email: gary@schaetzkc.com
+License: MIT
+Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
+Description-Content-Type: text/markdown
+
 # gitlab-ci-generator
 This project builds a dynamic gitlab ci file that is intended to be used for monorepos.  The concept is to simplify the amount of work that is needed to manage the monorepo.
 
 ## Installation
 You can download and run directly with python or install using:
 ```
 pip install gitlab-ci-generator
@@ -9,20 +20,20 @@
 This installs like an executable and you can simply run: 
 ```
 gitlab-ci-generator
 ```
 
 ## Usage
 The project takes the following parameters:
-|Name|Parameter|Description|Required|
-|-----|--------|-----------|--------|
-|Input File|--inputfile/-f|The yaml file that will be used to render the gitlab ci file.|Yes|
-|Output File|--outputfile/-o|The yaml file that is rendered using the jinja2 template with data from the input yaml file.|No|
-|Template File|--templatefile/-t|A jinja2 file that can be used to override default templating|No|
-|Help|-h|Displays help info|No|
+| Name          | Parameter         | Description                                                                                  | Required |
+| ------------- | ----------------- | -------------------------------------------------------------------------------------------- | -------- |
+| Input File    | --inputfile/-f    | The yaml file that will be used to render the gitlab ci file.                                | Yes      |
+| Output File   | --outputfile/-o   | The yaml file that is rendered using the jinja2 template with data from the input yaml file. | No       |
+| Template File | --templatefile/-t | A jinja2 file that can be used to override default templating                                | No       |
+| Help          | -h                | Displays help info                                                                           | No       |
 
 This program will load the input yaml file into two distinct dictionaries that are available to the template:
 * pipeline_info
 * jobs
 
 To run without specifying an output file you can write stdout to a redirect file like so: 
 ```
@@ -32,14 +43,17 @@
 ### pipeline_info
 This section is gets loaded as is into a dictionary so you can easily extend it for your needs.  The built-in template uses the following:
 ```
 pipeline_info:
   shared_includes: <<-- Used by the template to build the include: section of the gitlab ci file.
     - name: rules <<-- List of includes and can be of type local or project.  The rules example here is used in the template in concert with the share_reference_rules: section to define dynamic rules for jobs.
       local: "example/example-config/rules.yml" 
+  shared_variables: << -- Used by the template to build the variables: section of the gitlab ci under each job.
+    - name: MYVAR <-- The variable name to include
+      value: MYVAR_VALUE <-- The value string or a variable for the value 
   shared_reference_rules: <<-- Used by the template to build the rules: section of the gitlab ci under each job.
     - rule_name: standard-rule-if <- The rule_source and rule_name will create a !reference[rule_source, rule_name] value under the rules section of each job.
       rule_source: .job_changes_rules
       only_changes: true
   final_job: <<-- Optional section that can be used to specify a final trigger job to run at the end of your pipeline.
     name: <<-- The name of the final job.
     stage: <<-- The stage that you want the final job to run in.
@@ -70,14 +84,17 @@
 This sample can also be found in the gitlab repo for this project at the location [example/example-config/job-dependency.yml](https://gitlab.com/gary.schaetz/public/gitlab-ci-generator/-/blob/main/example/example-config/job-dependency.yml)
 ```
 ---
 pipeline_info:
   shared_includes:
     - name: rules
       local: "example/example-config/rules.yml"
+  shared_variables:
+    - name: MYVAR
+      value: MYVAR_VALUE
   shared_reference_rules:
     - rule_name: standard-rule-if
       rule_source: .job_changes_rules
       only_changes: true
     - rule_name:  manual-rule-if
       rule_source: .job_changes_rules
       when: manual
@@ -117,14 +134,15 @@
   - post-deploy
 
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
     PROJECT_JOB_NAME: example-1
+    MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
       changes:
@@ -135,14 +153,15 @@
     strategy: depend
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
+    MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
@@ -216,8 +235,8 @@
     strategy: depend
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
-MIT License
+MIT License
```

### Comparing `gitlab-ci-generator-1.0.5/setup.py` & `gitlab-ci-generator-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/PKG-INFO` & `gitlab-ci-generator-1.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: gitlab-ci-generator
-Version: 1.0.5
-Summary: Generates a mono-repo ci file.
-Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
-Author: Gary Schaetz
-Author-email: gary@schaetzkc.com
-License: MIT
-Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
-Description-Content-Type: text/markdown
-
 # gitlab-ci-generator
 This project builds a dynamic gitlab ci file that is intended to be used for monorepos.  The concept is to simplify the amount of work that is needed to manage the monorepo.
 
 ## Installation
 You can download and run directly with python or install using:
 ```
 pip install gitlab-ci-generator
@@ -20,20 +9,20 @@
 This installs like an executable and you can simply run: 
 ```
 gitlab-ci-generator
 ```
 
 ## Usage
 The project takes the following parameters:
-|Name|Parameter|Description|Required|
-|-----|--------|-----------|--------|
-|Input File|--inputfile/-f|The yaml file that will be used to render the gitlab ci file.|Yes|
-|Output File|--outputfile/-o|The yaml file that is rendered using the jinja2 template with data from the input yaml file.|No|
-|Template File|--templatefile/-t|A jinja2 file that can be used to override default templating|No|
-|Help|-h|Displays help info|No|
+| Name          | Parameter         | Description                                                                                  | Required |
+| ------------- | ----------------- | -------------------------------------------------------------------------------------------- | -------- |
+| Input File    | --inputfile/-f    | The yaml file that will be used to render the gitlab ci file.                                | Yes      |
+| Output File   | --outputfile/-o   | The yaml file that is rendered using the jinja2 template with data from the input yaml file. | No       |
+| Template File | --templatefile/-t | A jinja2 file that can be used to override default templating                                | No       |
+| Help          | -h                | Displays help info                                                                           | No       |
 
 This program will load the input yaml file into two distinct dictionaries that are available to the template:
 * pipeline_info
 * jobs
 
 To run without specifying an output file you can write stdout to a redirect file like so: 
 ```
@@ -43,14 +32,17 @@
 ### pipeline_info
 This section is gets loaded as is into a dictionary so you can easily extend it for your needs.  The built-in template uses the following:
 ```
 pipeline_info:
   shared_includes: <<-- Used by the template to build the include: section of the gitlab ci file.
     - name: rules <<-- List of includes and can be of type local or project.  The rules example here is used in the template in concert with the share_reference_rules: section to define dynamic rules for jobs.
       local: "example/example-config/rules.yml" 
+  shared_variables: << -- Used by the template to build the variables: section of the gitlab ci under each job.
+    - name: MYVAR <-- The variable name to include
+      value: MYVAR_VALUE <-- The value string or a variable for the value 
   shared_reference_rules: <<-- Used by the template to build the rules: section of the gitlab ci under each job.
     - rule_name: standard-rule-if <- The rule_source and rule_name will create a !reference[rule_source, rule_name] value under the rules section of each job.
       rule_source: .job_changes_rules
       only_changes: true
   final_job: <<-- Optional section that can be used to specify a final trigger job to run at the end of your pipeline.
     name: <<-- The name of the final job.
     stage: <<-- The stage that you want the final job to run in.
@@ -81,14 +73,17 @@
 This sample can also be found in the gitlab repo for this project at the location [example/example-config/job-dependency.yml](https://gitlab.com/gary.schaetz/public/gitlab-ci-generator/-/blob/main/example/example-config/job-dependency.yml)
 ```
 ---
 pipeline_info:
   shared_includes:
     - name: rules
       local: "example/example-config/rules.yml"
+  shared_variables:
+    - name: MYVAR
+      value: MYVAR_VALUE
   shared_reference_rules:
     - rule_name: standard-rule-if
       rule_source: .job_changes_rules
       only_changes: true
     - rule_name:  manual-rule-if
       rule_source: .job_changes_rules
       when: manual
@@ -128,14 +123,15 @@
   - post-deploy
 
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
     PROJECT_JOB_NAME: example-1
+    MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
       changes:
@@ -146,14 +142,15 @@
     strategy: depend
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
+    MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
@@ -227,8 +224,8 @@
     strategy: depend
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
-MIT License
+MIT License
```

### Comparing `gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/gitlab_ci_generator.py` & `gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/gitlab_ci_generator.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/templates/gitlab-template.jinja` & `gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/templates/gitlab-template.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
 {% for job in jobs %}
 {{ job.name }}:
   stage: build
   variables:
     PROJECT_SUBDIR: {{ job.folder }}
     PROJECT_JOB_NAME: {{ job.name }}
+{% for variable in pipeline_info.shared_variables %}
+    {{ variable.name }}: {{ variable.value }}
+{% endfor %}
   rules:
 {% for rule in pipeline_info.shared_reference_rules %}
     - if: !reference [{{ rule.rule_source }},{{ rule.rule_name }}]
 {% if rule.when %}
       when: {{ rule.when }}
 {% endif -%}
 {% if rule.only_changes == true %}
```

